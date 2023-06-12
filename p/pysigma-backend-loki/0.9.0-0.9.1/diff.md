# Comparing `tmp/pysigma_backend_loki-0.9.0.tar.gz` & `tmp/pysigma_backend_loki-0.9.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pysigma_backend_loki-0.9.0.tar", max compression
+gzip compressed data, was "pysigma_backend_loki-0.9.1.tar", max compression
```

## Comparing `pysigma_backend_loki-0.9.0.tar` & `pysigma_backend_loki-0.9.1.tar`

### file list

```diff
@@ -1,9 +1,9 @@
--rw-r--r--   0        0        0      598 2023-06-12 10:21:13.673885 pysigma_backend_loki-0.9.0/LICENSE
--rw-r--r--   0        0        0     5382 2023-06-12 10:21:13.673885 pysigma_backend_loki-0.9.0/README.md
--rw-r--r--   0        0        0      777 2023-06-12 10:21:13.673885 pysigma_backend_loki-0.9.0/pyproject.toml
--rw-r--r--   0        0        0      102 2023-06-12 10:21:13.673885 pysigma_backend_loki-0.9.0/sigma/backends/loki/__init__.py
--rw-r--r--   0        0        0    44996 2023-06-12 10:21:13.677885 pysigma_backend_loki-0.9.0/sigma/backends/loki/loki.py
--rw-r--r--   0        0        0      494 2023-06-12 10:21:13.677885 pysigma_backend_loki-0.9.0/sigma/pipelines/loki/__init__.py
--rw-r--r--   0        0        0     8361 2023-06-12 10:21:13.677885 pysigma_backend_loki-0.9.0/sigma/pipelines/loki/loki.py
--rw-r--r--   0        0        0     6147 1970-01-01 00:00:00.000000 pysigma_backend_loki-0.9.0/setup.py
--rw-r--r--   0        0        0     6107 1970-01-01 00:00:00.000000 pysigma_backend_loki-0.9.0/PKG-INFO
+-rw-r--r--   0        0        0      598 2023-06-12 16:03:42.745792 pysigma_backend_loki-0.9.1/LICENSE
+-rw-r--r--   0        0        0     5382 2023-06-12 16:03:42.745792 pysigma_backend_loki-0.9.1/README.md
+-rw-r--r--   0        0        0      777 2023-06-12 16:03:42.749792 pysigma_backend_loki-0.9.1/pyproject.toml
+-rw-r--r--   0        0        0      102 2023-06-12 16:03:42.749792 pysigma_backend_loki-0.9.1/sigma/backends/loki/__init__.py
+-rw-r--r--   0        0        0    46230 2023-06-12 16:03:42.749792 pysigma_backend_loki-0.9.1/sigma/backends/loki/loki.py
+-rw-r--r--   0        0        0      494 2023-06-12 16:03:42.749792 pysigma_backend_loki-0.9.1/sigma/pipelines/loki/__init__.py
+-rw-r--r--   0        0        0     8361 2023-06-12 16:03:42.749792 pysigma_backend_loki-0.9.1/sigma/pipelines/loki/loki.py
+-rw-r--r--   0        0        0     6147 1970-01-01 00:00:00.000000 pysigma_backend_loki-0.9.1/setup.py
+-rw-r--r--   0        0        0     6107 1970-01-01 00:00:00.000000 pysigma_backend_loki-0.9.1/PKG-INFO
```

### Comparing `pysigma_backend_loki-0.9.0/LICENSE` & `pysigma_backend_loki-0.9.1/LICENSE`

 * *Files identical despite different names*

### Comparing `pysigma_backend_loki-0.9.0/README.md` & `pysigma_backend_loki-0.9.1/README.md`

 * *Files identical despite different names*

### Comparing `pysigma_backend_loki-0.9.0/pyproject.toml` & `pysigma_backend_loki-0.9.1/pyproject.toml`

 * *Files 17% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "pySigma-backend-loki"
-version = "0.9.0"
+version = "0.9.1"
 description = "pySigma Loki backend"
 readme = "README.md"
 authors = ["Nick Moore <nicholas.moore@grafana.com>", "Mostafa Moradian <mostafa.moradian@grafana.com>"]
 license = "AGPL-3.0-only"
 repository = "https://github.com/grafana/pySigma-backend-loki"
 packages = [
     { include = "sigma" }
```

### Comparing `pysigma_backend_loki-0.9.0/sigma/backends/loki/loki.py` & `pysigma_backend_loki-0.9.1/sigma/backends/loki/loki.py`

 * *Files 5% similar despite different names*

```diff
@@ -31,14 +31,15 @@
 from sigma.conversion.state import ConversionState
 from sigma.exceptions import SigmaFeatureNotSupportedByBackendError, SigmaError
 from sigma.pipelines.loki import LokiCustomAttributes
 from sigma.processing.pipeline import ProcessingPipeline
 from sigma.rule import SigmaRule
 from sigma.types import (
     SigmaBool,
+    SigmaCasedString,
     SigmaCompareExpression,
     SigmaCIDRExpression,
     SigmaRegularExpression,
     SigmaString,
     SigmaNull,
     SigmaNumber,
 )
@@ -135,15 +136,19 @@
         return self
 
     def finalize_expression(self) -> str:
         # This makes the regex case insensitive if any values are SigmaStrings
         # or if any of the regexes are case insensitive
         # TODO: can we make this more precise?
         case_insensitive = any(
-            (isinstance(val, SigmaString) and self.case_insensitive)
+            (
+                isinstance(val, SigmaString)
+                and self.case_insensitive
+                and not isinstance(val, SigmaCasedString)
+            )
             or (
                 isinstance(val, SigmaRegularExpression)
                 and val.regexp.startswith("(?i)")
             )
             for val in self.exprs
         )
         or_value = "|".join(
@@ -215,14 +220,15 @@
     # Leave this to be set by the below function
     eq_token: ClassVar[str]
     field_null_expression: ClassVar[str]
     re_expression: ClassVar[str]
     cidr_expression: ClassVar[str]
     compare_op_expression: ClassVar[str]
     compare_operators: ClassVar[Dict[SigmaCompareExpression.CompareOperators, str]]
+    case_sensitive_match_expression: ClassVar[str]
 
     @staticmethod
     def set_expression_templates(negated: bool) -> None:
         """When converting field expressions, the TextBackend class uses the below
         variables to format the rule. As LogQL applies negation directly via
         expressions, we need to dynamically update these depending on whether the
         expression was negated or not."""
@@ -235,25 +241,27 @@
             LogQLBackend.cidr_expression = '{field}=ip("{value}")'
             LogQLBackend.compare_operators = {
                 SigmaCompareExpression.CompareOperators.LT: "<",
                 SigmaCompareExpression.CompareOperators.LTE: "<=",
                 SigmaCompareExpression.CompareOperators.GT: ">",
                 SigmaCompareExpression.CompareOperators.GTE: ">=",
             }
+            LogQLBackend.case_sensitive_match_expression = "{field}={value}"
         else:
             LogQLBackend.eq_token = "!="
             LogQLBackend.field_null_expression = "{field}!=``"
             LogQLBackend.re_expression = "{field}!~{regex}"
             LogQLBackend.cidr_expression = '{field}!=ip("{value}")'
             LogQLBackend.compare_operators = {
                 SigmaCompareExpression.CompareOperators.LT: ">=",
                 SigmaCompareExpression.CompareOperators.LTE: ">",
                 SigmaCompareExpression.CompareOperators.GT: "<=",
                 SigmaCompareExpression.CompareOperators.GTE: "<",
             }
+            LogQLBackend.case_sensitive_match_expression = "{field}!={value}"
         # Cache the state of these variables so we don't keep setting them needlessly
         LogQLBackend.current_templates = negated
 
     # LogQL does not support wildcards, but we convert them to regular expressions
     # Character used as multi-character wildcard (replaced with .*)
     wildcard_multi: ClassVar[str] = "*"
     # Character used as single-character wildcard (replaced with .)
@@ -288,20 +296,23 @@
         self.case_insensitive = case_insensitive
 
     # Loki-specific functions
     # When converting values to regexes, we need to escape the string to prevent use of
     # non-wildcard metacharacters
     # As str equality is case-insensitive in Sigma, but LogQL regexes are case-sensitive,
     # we need to do the same for *ALL* string values and prepend with (?i)
-    def convert_str_to_re(self, value: SigmaString) -> SigmaRegularExpression:
+    def convert_str_to_re(
+        self, value: SigmaString, case_insensitive: bool = True
+    ) -> SigmaRegularExpression:
         """Convert a SigmaString into a regular expression, replacing any
         wildcards with equivalent regular expression operators, and enforcing
         case-insensitive matching"""
         return SigmaRegularExpression(
-            "(?i)" + re.escape(str(value)).replace("\\?", ".").replace("\\*", ".*")
+            ("(?i)" if case_insensitive else "")
+            + re.escape(str(value)).replace("\\?", ".").replace("\\*", ".*")
         )
 
     def select_log_parser(self, rule: SigmaRule) -> Union[str, LogQLLogParser]:
         """Select a relevant log parser based on common approaches to ingesting data into Loki.
         Currently defaults to logfmt, but will use the json parser for Windows, Azure and Zeek
         signatures."""
         if LokiCustomAttributes.PARSER.value in rule.custom_attributes:
@@ -575,16 +586,18 @@
           negation down the tree (flipping ANDs and ORs and swapping operators, i.e.,
           = becomes !=, etc.)
         """
         if isinstance(
             condition,
             (ConditionFieldEqualsValueExpression, ConditionValueExpression),
         ):
-            if isinstance(condition.value, SigmaString) and (
-                self.case_insensitive or condition.value.contains_special()
+            if (
+                isinstance(condition.value, SigmaString)
+                and (self.case_insensitive or condition.value.contains_special())
+                and not isinstance(condition.value, SigmaCasedString)
             ):
                 condition.value = self.convert_str_to_re(condition.value)
         if isinstance(condition, ConditionItem):
             if isinstance(condition, ConditionNOT):
                 negated = not negated
                 # Remove the ConditionNOT as the parent
                 condition.args[0].parent = condition.parent
@@ -823,14 +836,25 @@
         self, cond: ConditionFieldEqualsValueExpression, state: ConversionState
     ) -> Union[str, DeferredQueryExpression]:
         if self.case_insensitive and len(cond.value) > 0:
             cond.value = self.convert_str_to_re(cond.value)
             return super().convert_condition_field_eq_val_re(cond, state)
         return super().convert_condition_field_eq_val_str(cond, state)
 
+    def convert_condition_field_eq_val_str_case_sensitive(
+        self, cond: ConditionFieldEqualsValueExpression, state: ConversionState
+    ) -> Union[str, DeferredQueryExpression]:
+        """If the cased modifier is combined with startswith/endswith/contains
+        modifiers, Sigma introduces wildcards that are then not handled correctly
+        by Loki. So, in those cases, we convert the string to a regular expression."""
+        if cond.value.contains_special():
+            cond.value = self.convert_str_to_re(cond.value, False)
+            return super().convert_condition_field_eq_val_re(cond, state)
+        return super().convert_condition_field_eq_val_str_case_sensitive(cond, state)
+
     def convert_condition_val_str(
         self, cond: ConditionValueExpression, state: ConversionState
     ) -> Union[str, DeferredQueryExpression]:
         """Converts all unbound wildcard conditions into regular expression queries,
         replacing wildcards with appropriate regex metacharacters."""
         expr = LogQLDeferredUnboundStrExpression(
             state, self.convert_value_str(cond.value, state)
```

### Comparing `pysigma_backend_loki-0.9.0/sigma/pipelines/loki/loki.py` & `pysigma_backend_loki-0.9.1/sigma/pipelines/loki/loki.py`

 * *Files identical despite different names*

### Comparing `pysigma_backend_loki-0.9.0/setup.py` & `pysigma_backend_loki-0.9.1/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -8,15 +8,15 @@
 {'': ['*']}
 
 install_requires = \
 ['pysigma-pipeline-sysmon>=1.0.1,<2.0.0', 'pysigma>=0.9.11,<0.10.0']
 
 setup_kwargs = {
     'name': 'pysigma-backend-loki',
-    'version': '0.9.0',
+    'version': '0.9.1',
     'description': 'pySigma Loki backend',
     'long_description': '![PyPI](https://img.shields.io/pypi/v/pysigma-backend-loki)\n![Tests](https://github.com/grafana/pySigma-backend-loki/actions/workflows/test.yml/badge.svg)\n[![Coverage Status](https://coveralls.io/repos/github/grafana/pySigma-backend-loki/badge.svg?branch=main&t=lvM1Ns)](https://coveralls.io/github/grafana/pySigma-backend-loki?branch=main)\n\n# pySigma Loki Backend\n\nThis is the Loki backend for pySigma. It provides the package `sigma.backends.loki` with the `LogQLBackend` class.\n\nIt supports the following output formats:\n\n* `default`: plain Loki LogQL queries\n* `ruler`: creates Loki LogQL queries in the ruler (YAML) format for generating alerts\n\nIt includes the following pipeline transformations in `sigma.pipelines.loki`:\n\n* `SetCustomAttributeTransformation`: adds a specified custom attribute to a rule, which can be used to introduce a [stream selector](https://grafana.com/docs/loki/latest/logql/log_queries/#log-stream-selector) or [parser expression](https://grafana.com/docs/loki/latest/logql/log_queries/#parser-expression) into the generated query\n  * The `LokiCustomAttributes` enum contains the relevant custom attribute names used by the backend\n\nFurther, it contains the processing pipelines in `sigma.pipelines.loki`:\n\n* `loki_log_parser`: converts field names to logfmt labels used by Grafana\n* `loki_promtail_sysmon`: parse and adjust field names for Windows sysmon data produced by promtail\n  * Note: most rules lack the `sysmon` service tag, and hence this pipeline should be used in combination with the [generic sysmon pipeline](https://github.com/SigmaHQ/pySigma-pipeline-sysmon)\n* `loki_okta_system_log`: parse the Okta System Log event json, adjusting field-names appropriately\n\nWhen converting rules into queries, the backend has the following optional arguments:\n\n* `add_line_filters` (boolean, default: `False`): if `True`, attempts to infer and add new line filters to queries without line filters, to [improve Loki query performance](https://grafana.com/docs/loki/latest/logql/log_queries/#line-filter-expression)\n* `case_insensitive` (boolean, default: `True`): if `False`, defaults to generating case-sensitive query filters, instead of case-insensitive filters that [the Sigma specification expects](https://github.com/SigmaHQ/sigma-specification/blob/main/Sigma_specification.md#general), trading between Loki query performance and potentially missing data with unexpected casing\n  * Note: if the generated query will be executed on Loki v2.8.2 or older, this argument **should** be set to `False`, as these versions of Loki may contain issues with case-insensitive filters, which cause such queries to fail to match desired data\n\nThis backend is currently maintained by:\n\n* [Nick Moore](https://github.com/kelnage)\n* [Mostafa Moradian](https://github.com/mostafa)\n\n## Installation\n\nTo get started developing/testing pySigma-backend-loki, these steps may help you get started:\n\n1. [Install poetry](https://python-poetry.org/docs/#installation)\n2. Clone this repository and open a terminal/shell in the top-level directory\n3. Run `poetry install` to install the Python dependencies\n4. Run `poetry shell` to activate the poetry environment\n5. Check it all works by running `poetry run pytest`\n6. (Optional) If you wish to validate the generated rules using sigma\\_backend\\_tester.py, install\n   [LogCLI](https://grafana.com/docs/loki/latest/tools/logcli/)\n7. (Optional, but recommended) To enable the Git hooks, run the following command from the root directory of the repository:\n```sh\ngit config --local core.hooksPath .githooks/\n```\n\n## Releasing\n\nTo release new versions of pySigma-backend-loki, we use GitHub actions to update PyPI. When the main branch is in state that is ready to release, the process is as follows:\n\n1. Determine the correct version number using the [Semantic Versioning](https://semver.org/) methodology. All version numbers should be in the format `\\d+\\.\\d+\\.\\d+(-[0-9A-Za-z-]+)?`\n2. Update [pyproject.toml](https://github.com/grafana/pySigma-backend-loki/blob/main/pyproject.toml) with the new version number\n3. Commit and push the change to GitHub, and validate that the GitHub actions tests pass\n4. Create a signed tag for the release, named the version number prefixed with a v, e.g., `git tag --sign --message="Release vX.X.X" vX.X.X`\n5. Push the tag to GitHub, e.g., `git push --tags`, and validate that the release to the test instance of PyPI is successful\n6. Run `poetry build` to produce distributable versions in `dist/`\n7. Create a release in GitHub against the appropriate tag. If the version number starts with `v0`, or ends with `-alpha/beta` etc., mark it as a pre-release, and attach the distributable files to the release\n8. Validate that the release to PyPI GitHub action is successful\n\n## Work in progress\n\nThese features are currently either WIP or are planned to be implemented in the near future.\n\n* Various processing pipelines for other applications and log sources\n* Generating more accurate log stream selectors based on logsource\n* Translate field names in Sigma signatures into relevant labels for Loki using pipelines\n\n## Won\'t implement (probably)\n\nThese features are not easily supported by the backend, and hence are unlikely to be implemented.\n\n* More complex keyword/line filter searches than ANDs of ORs\n',
     'author': 'Nick Moore',
     'author_email': 'nicholas.moore@grafana.com',
     'maintainer': 'None',
     'maintainer_email': 'None',
     'url': 'https://github.com/grafana/pySigma-backend-loki',
```

### Comparing `pysigma_backend_loki-0.9.0/PKG-INFO` & `pysigma_backend_loki-0.9.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pysigma-backend-loki
-Version: 0.9.0
+Version: 0.9.1
 Summary: pySigma Loki backend
 Home-page: https://github.com/grafana/pySigma-backend-loki
 License: AGPL-3.0-only
 Author: Nick Moore
 Author-email: nicholas.moore@grafana.com
 Requires-Python: >=3.8,<4.0
 Classifier: License :: OSI Approved :: GNU Affero General Public License v3
```

