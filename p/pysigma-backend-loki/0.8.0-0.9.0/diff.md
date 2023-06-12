# Comparing `tmp/pysigma_backend_loki-0.8.0.tar.gz` & `tmp/pysigma_backend_loki-0.9.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pysigma_backend_loki-0.8.0.tar", max compression
+gzip compressed data, was "pysigma_backend_loki-0.9.0.tar", max compression
```

## Comparing `pysigma_backend_loki-0.8.0.tar` & `pysigma_backend_loki-0.9.0.tar`

### file list

```diff
@@ -1,9 +1,9 @@
--rw-r--r--   0        0        0      598 2023-04-21 13:25:19.469689 pysigma_backend_loki-0.8.0/LICENSE
--rw-r--r--   0        0        0     4428 2023-04-21 13:25:19.469689 pysigma_backend_loki-0.8.0/README.md
--rw-r--r--   0        0        0      809 2023-04-21 13:25:19.473689 pysigma_backend_loki-0.8.0/pyproject.toml
--rw-r--r--   0        0        0      102 2023-04-21 13:25:19.473689 pysigma_backend_loki-0.8.0/sigma/backends/loki/__init__.py
--rw-r--r--   0        0        0    43538 2023-04-21 13:25:19.473689 pysigma_backend_loki-0.8.0/sigma/backends/loki/loki.py
--rw-r--r--   0        0        0      533 2023-04-21 13:25:19.473689 pysigma_backend_loki-0.8.0/sigma/pipelines/loki/__init__.py
--rw-r--r--   0        0        0     8382 2023-04-21 13:25:19.473689 pysigma_backend_loki-0.8.0/sigma/pipelines/loki/loki.py
--rw-r--r--   0        0        0     5192 1970-01-01 00:00:00.000000 pysigma_backend_loki-0.8.0/setup.py
--rw-r--r--   0        0        0     5158 1970-01-01 00:00:00.000000 pysigma_backend_loki-0.8.0/PKG-INFO
+-rw-r--r--   0        0        0      598 2023-06-12 10:21:13.673885 pysigma_backend_loki-0.9.0/LICENSE
+-rw-r--r--   0        0        0     5382 2023-06-12 10:21:13.673885 pysigma_backend_loki-0.9.0/README.md
+-rw-r--r--   0        0        0      777 2023-06-12 10:21:13.673885 pysigma_backend_loki-0.9.0/pyproject.toml
+-rw-r--r--   0        0        0      102 2023-06-12 10:21:13.673885 pysigma_backend_loki-0.9.0/sigma/backends/loki/__init__.py
+-rw-r--r--   0        0        0    44996 2023-06-12 10:21:13.677885 pysigma_backend_loki-0.9.0/sigma/backends/loki/loki.py
+-rw-r--r--   0        0        0      494 2023-06-12 10:21:13.677885 pysigma_backend_loki-0.9.0/sigma/pipelines/loki/__init__.py
+-rw-r--r--   0        0        0     8361 2023-06-12 10:21:13.677885 pysigma_backend_loki-0.9.0/sigma/pipelines/loki/loki.py
+-rw-r--r--   0        0        0     6147 1970-01-01 00:00:00.000000 pysigma_backend_loki-0.9.0/setup.py
+-rw-r--r--   0        0        0     6107 1970-01-01 00:00:00.000000 pysigma_backend_loki-0.9.0/PKG-INFO
```

### Comparing `pysigma_backend_loki-0.8.0/LICENSE` & `pysigma_backend_loki-0.9.0/LICENSE`

 * *Files identical despite different names*

### Comparing `pysigma_backend_loki-0.8.0/README.md` & `pysigma_backend_loki-0.9.0/README.md`

 * *Files 15% similar despite different names*

```diff
@@ -15,17 +15,23 @@
 
 * `SetCustomAttributeTransformation`: adds a specified custom attribute to a rule, which can be used to introduce a [stream selector](https://grafana.com/docs/loki/latest/logql/log_queries/#log-stream-selector) or [parser expression](https://grafana.com/docs/loki/latest/logql/log_queries/#parser-expression) into the generated query
   * The `LokiCustomAttributes` enum contains the relevant custom attribute names used by the backend
 
 Further, it contains the processing pipelines in `sigma.pipelines.loki`:
 
 * `loki_log_parser`: converts field names to logfmt labels used by Grafana
-* `loki_promtail_sysmon_message`: parse and adjust field names for Windows sysmon data produced by promtail
+* `loki_promtail_sysmon`: parse and adjust field names for Windows sysmon data produced by promtail
   * Note: most rules lack the `sysmon` service tag, and hence this pipeline should be used in combination with the [generic sysmon pipeline](https://github.com/SigmaHQ/pySigma-pipeline-sysmon)
-* `loki_okta_system_log_json`: parse the Okta System Log event json, adjusting field-names appropriately
+* `loki_okta_system_log`: parse the Okta System Log event json, adjusting field-names appropriately
+
+When converting rules into queries, the backend has the following optional arguments:
+
+* `add_line_filters` (boolean, default: `False`): if `True`, attempts to infer and add new line filters to queries without line filters, to [improve Loki query performance](https://grafana.com/docs/loki/latest/logql/log_queries/#line-filter-expression)
+* `case_insensitive` (boolean, default: `True`): if `False`, defaults to generating case-sensitive query filters, instead of case-insensitive filters that [the Sigma specification expects](https://github.com/SigmaHQ/sigma-specification/blob/main/Sigma_specification.md#general), trading between Loki query performance and potentially missing data with unexpected casing
+  * Note: if the generated query will be executed on Loki v2.8.2 or older, this argument **should** be set to `False`, as these versions of Loki may contain issues with case-insensitive filters, which cause such queries to fail to match desired data
 
 This backend is currently maintained by:
 
 * [Nick Moore](https://github.com/kelnage)
 * [Mostafa Moradian](https://github.com/mostafa)
 
 ## Installation
```

### Comparing `pysigma_backend_loki-0.8.0/pyproject.toml` & `pysigma_backend_loki-0.9.0/pyproject.toml`

 * *Files 12% similar despite different names*

```diff
@@ -1,32 +1,30 @@
 [tool.poetry]
 name = "pySigma-backend-loki"
-version = "0.8.0"
+version = "0.9.0"
 description = "pySigma Loki backend"
 readme = "README.md"
 authors = ["Nick Moore <nicholas.moore@grafana.com>", "Mostafa Moradian <mostafa.moradian@grafana.com>"]
 license = "AGPL-3.0-only"
 repository = "https://github.com/grafana/pySigma-backend-loki"
 packages = [
     { include = "sigma" }
 ]
 
 [tool.poetry.dependencies]
 python = "^3.8"
-pysigma = "^0.9.6"
+pysigma = "^0.9.11"
 pysigma-pipeline-sysmon = "^1.0.1"
 
-[tool.poetry.dev-dependencies]
-
 [tool.poetry.group.dev.dependencies]
 pytest = "^7.3.1"
-pytest-cov = "^4.0.0"
-coverage = "^7.2.3"
-mypy = "^1.2.0"
-pytest-mypy = "^0.10.1"
-types-pyyaml = "6.0.12.9"
+pytest-cov = "^4.1.0"
+coverage = "^7.2.6"
+mypy = "^1.3.0"
+pytest-mypy = "^0.10.3"
+types-pyyaml = "6.0.12.10"
 flake8 = "^5.0.4"
-black = "^23.1.0"
+black = "^23.3.0"
 
 [build-system]
 requires = ["poetry-core>=1.0.0"]
 build-backend = "poetry.core.masonry.api"
```

### Comparing `pysigma_backend_loki-0.8.0/sigma/backends/loki/loki.py` & `pysigma_backend_loki-0.9.0/sigma/backends/loki/loki.py`

 * *Files 3% similar despite different names*

```diff
@@ -124,24 +124,31 @@
 
 @dataclass
 class LogQLDeferredOrUnboundExpression(DeferredQueryExpression):
     """'Defer' unbounded OR matching to pipelined command **BEFORE** main search expression."""
 
     exprs: List[Union[SigmaString, SigmaRegularExpression]]
     op: str = "|~"  # default to matching
+    case_insensitive: bool = True
 
     def negate(self) -> DeferredQueryExpression:
         self.op = LogQLBackend.negated_line_filter_operator[self.op]
         return self
 
     def finalize_expression(self) -> str:
+        # This makes the regex case insensitive if any values are SigmaStrings
+        # or if any of the regexes are case insensitive
+        # TODO: can we make this more precise?
         case_insensitive = any(
-            val.regexp.startswith("(?i)")
+            (isinstance(val, SigmaString) and self.case_insensitive)
+            or (
+                isinstance(val, SigmaRegularExpression)
+                and val.regexp.startswith("(?i)")
+            )
             for val in self.exprs
-            if isinstance(val, SigmaRegularExpression)
         )
         or_value = "|".join(
             (
                 re.escape(str(val))
                 if isinstance(val, SigmaString)
                 else re.sub("^\\(\\?i\\)", "", val.regexp)
                 for val in self.exprs
@@ -263,31 +270,36 @@
 
     deferred_start: ClassVar[str] = ""
     deferred_separator: ClassVar[str] = " "
     deferred_only_query: ClassVar[str] = ""
 
     # Loki-specific functionality
     add_line_filters: bool = False
+    case_insensitive: bool = True
 
     def __init__(
         self,
         processing_pipeline: Optional[ProcessingPipeline] = None,
         collect_errors: bool = False,
         add_line_filters: bool = False,
+        case_insensitive: bool = True,
     ):
         super().__init__(processing_pipeline, collect_errors)
         self.add_line_filters = add_line_filters
+        self.case_insensitive = case_insensitive
 
     # Loki-specific functions
     # When converting values to regexes, we need to escape the string to prevent use of
     # non-wildcard metacharacters
     # As str equality is case-insensitive in Sigma, but LogQL regexes are case-sensitive,
-    # we also prepend with (?i)
-    def convert_wildcard_to_re(self, value: SigmaString) -> SigmaRegularExpression:
-        """Convert a SigmaString value that contains wildcards into a regular expression"""
+    # we need to do the same for *ALL* string values and prepend with (?i)
+    def convert_str_to_re(self, value: SigmaString) -> SigmaRegularExpression:
+        """Convert a SigmaString into a regular expression, replacing any
+        wildcards with equivalent regular expression operators, and enforcing
+        case-insensitive matching"""
         return SigmaRegularExpression(
             "(?i)" + re.escape(str(value)).replace("\\?", ".").replace("\\*", ".*")
         )
 
     def select_log_parser(self, rule: SigmaRule) -> Union[str, LogQLLogParser]:
         """Select a relevant log parser based on common approaches to ingesting data into Loki.
         Currently defaults to logfmt, but will use the json parser for Windows, Azure and Zeek
@@ -551,27 +563,30 @@
         self, condition: ParentChainMixin, negated: bool = False
     ) -> ParentChainMixin:
         """Do a depth-first recursive search of the parsed items and update conditions
         to meet LogQL's structural requirements:
 
         - LogQL does not support wildcards in strings, so we convert them instead to
           regular expressions
+        - LogQL does case sensitive searches by default, but Sigma strings are case
+          insensitive, so to be fully spec compliant, we have to convert them into
+          regular expressions with a leading (?i) flag
+          - Can be disabled by setting the instance variable case_insensitive to False
         - LogQL does not support NOT operators, so we use De Morgan's law to push the
           negation down the tree (flipping ANDs and ORs and swapping operators, i.e.,
           = becomes !=, etc.)
         """
         if isinstance(
             condition,
             (ConditionFieldEqualsValueExpression, ConditionValueExpression),
         ):
-            if (
-                isinstance(condition.value, SigmaString)
-                and condition.value.contains_special()
+            if isinstance(condition.value, SigmaString) and (
+                self.case_insensitive or condition.value.contains_special()
             ):
-                condition.value = self.convert_wildcard_to_re(condition.value)
+                condition.value = self.convert_str_to_re(condition.value)
         if isinstance(condition, ConditionItem):
             if isinstance(condition, ConditionNOT):
                 negated = not negated
                 # Remove the ConditionNOT as the parent
                 condition.args[0].parent = condition.parent
                 return self.update_parsed_conditions(condition.args[0], negated)
             elif isinstance(condition, (ConditionAND, ConditionOR)):
@@ -732,15 +747,15 @@
         unbound_deferred_or = None
         for arg in cond.args:
             if isinstance(arg, ConditionValueExpression) and isinstance(
                 arg.value, (SigmaString, SigmaRegularExpression)
             ):
                 if unbound_deferred_or is None:
                     unbound_deferred_or = LogQLDeferredOrUnboundExpression(
-                        state, [], "|~"
+                        state, [], "|~", self.case_insensitive
                     )
                     if getattr(cond, "negated", False):
                         unbound_deferred_or.negate()
                 unbound_deferred_or.exprs.append(arg.value)
             elif unbound_deferred_or is not None:
                 raise SigmaFeatureNotSupportedByBackendError(
                     "Operator 'or' not supported by the backend for unbound conditions combined "
@@ -800,14 +815,22 @@
     ) -> Union[str, DeferredQueryExpression]:
         """Adjust the expression templates based on whether the condition is negated,
         prior to converting it. Not required for convert_condition_val, as they use
         deferred expressions, which use a different approach."""
         LogQLBackend.set_expression_templates(getattr(cond, "negated", False))
         return super().convert_condition_field_eq_val(cond, state)
 
+    def convert_condition_field_eq_val_str(
+        self, cond: ConditionFieldEqualsValueExpression, state: ConversionState
+    ) -> Union[str, DeferredQueryExpression]:
+        if self.case_insensitive and len(cond.value) > 0:
+            cond.value = self.convert_str_to_re(cond.value)
+            return super().convert_condition_field_eq_val_re(cond, state)
+        return super().convert_condition_field_eq_val_str(cond, state)
+
     def convert_condition_val_str(
         self, cond: ConditionValueExpression, state: ConversionState
     ) -> Union[str, DeferredQueryExpression]:
         """Converts all unbound wildcard conditions into regular expression queries,
         replacing wildcards with appropriate regex metacharacters."""
         expr = LogQLDeferredUnboundStrExpression(
             state, self.convert_value_str(cond.value, state)
@@ -950,14 +973,16 @@
         alert = self.field_replace_pattern.sub("_", rule.title).strip("_")
         ruler = {
             "alert": alert,
             "annotations": {"description": rule.description, "summary": rule.title},
             "expr": f"sum(count_over_time({query} [1m])) or vector(0) > 0",
             "labels": {},
         }
+        if rule.author:
+            ruler["annotations"]["author"] = rule.author
         if rule.level:
             ruler["labels"]["severity"] = rule.level.name.lower()  # type: ignore
         return ruler
 
     def finalize_output_ruler(self, queries: List[Dict[str, Any]]) -> str:
         """Produce a collection of alert queries bundled together in a single Loki ruler
         YAML format."""
```

### Comparing `pysigma_backend_loki-0.8.0/sigma/pipelines/loki/loki.py` & `pysigma_backend_loki-0.9.0/sigma/pipelines/loki/loki.py`

 * *Files 2% similar despite different names*

```diff
@@ -58,15 +58,15 @@
                     }
                 ),
             )
         ],
     )
 
 
-def loki_promtail_sysmon_message() -> ProcessingPipeline:
+def loki_promtail_sysmon() -> ProcessingPipeline:
     return ProcessingPipeline(
         name="Loki Promtail Windows Sysmon Message Parser",
         priority=20,
         allowed_backends=frozenset({"loki"}),
         items=[
             ProcessingItem(
                 identifier="loki_promtail_sysmon_field_mapping",
@@ -93,15 +93,15 @@
                         "UserData": "user_data",
                         "EventData": "event_data",
                         "Message": "message",
                     }
                 ),
             ),
             ProcessingItem(
-                identifier="loki_promtail_sysmon_message_parser",
+                identifier="loki_promtail_sysmon_parser",
                 transformation=SetCustomAttributeTransformation(
                     attribute=LokiCustomAttributes.PARSER.value,
                     value='json | label_format Message=`{{ .message | replace "\\\\" "\\\\\\\\" | replace "\\"" "\\\\\\"" }}` '  # noqa: E501
                     '| line_format `{{ regexReplaceAll "([^:]+): ?((?:[^\\\\r]*|$))(\\r\\n|$)" .Message "${1}=\\"${2}\\" "}}` '  # noqa: E501
                     "| logfmt",
                 ),
                 rule_conditions=[
@@ -111,15 +111,15 @@
                     )
                 ],
             ),
         ],
     )
 
 
-def loki_okta_system_log_json() -> ProcessingPipeline:
+def loki_okta_system_log() -> ProcessingPipeline:
     return ProcessingPipeline(
         name="Loki Okta System Log json",
         priority=20,
         allowed_backends=frozenset({"loki"}),
         items=[
             ProcessingItem(
                 identifier="loki_okta_event_json_formatter",
```

### Comparing `pysigma_backend_loki-0.8.0/setup.py` & `pysigma_backend_loki-0.9.0/setup.py`

 * *Files 8% similar despite different names*

```diff
@@ -4,21 +4,21 @@
 packages = \
 ['sigma', 'sigma.backends.loki', 'sigma.pipelines.loki']
 
 package_data = \
 {'': ['*']}
 
 install_requires = \
-['pysigma-pipeline-sysmon>=1.0.1,<2.0.0', 'pysigma>=0.9.6,<0.10.0']
+['pysigma-pipeline-sysmon>=1.0.1,<2.0.0', 'pysigma>=0.9.11,<0.10.0']
 
 setup_kwargs = {
     'name': 'pysigma-backend-loki',
-    'version': '0.8.0',
+    'version': '0.9.0',
     'description': 'pySigma Loki backend',
-    'long_description': '![PyPI](https://img.shields.io/pypi/v/pysigma-backend-loki)\n![Tests](https://github.com/grafana/pySigma-backend-loki/actions/workflows/test.yml/badge.svg)\n[![Coverage Status](https://coveralls.io/repos/github/grafana/pySigma-backend-loki/badge.svg?branch=main&t=lvM1Ns)](https://coveralls.io/github/grafana/pySigma-backend-loki?branch=main)\n\n# pySigma Loki Backend\n\nThis is the Loki backend for pySigma. It provides the package `sigma.backends.loki` with the `LogQLBackend` class.\n\nIt supports the following output formats:\n\n* `default`: plain Loki LogQL queries\n* `ruler`: creates Loki LogQL queries in the ruler (YAML) format for generating alerts\n\nIt includes the following pipeline transformations in `sigma.pipelines.loki`:\n\n* `SetCustomAttributeTransformation`: adds a specified custom attribute to a rule, which can be used to introduce a [stream selector](https://grafana.com/docs/loki/latest/logql/log_queries/#log-stream-selector) or [parser expression](https://grafana.com/docs/loki/latest/logql/log_queries/#parser-expression) into the generated query\n  * The `LokiCustomAttributes` enum contains the relevant custom attribute names used by the backend\n\nFurther, it contains the processing pipelines in `sigma.pipelines.loki`:\n\n* `loki_log_parser`: converts field names to logfmt labels used by Grafana\n* `loki_promtail_sysmon_message`: parse and adjust field names for Windows sysmon data produced by promtail\n  * Note: most rules lack the `sysmon` service tag, and hence this pipeline should be used in combination with the [generic sysmon pipeline](https://github.com/SigmaHQ/pySigma-pipeline-sysmon)\n* `loki_okta_system_log_json`: parse the Okta System Log event json, adjusting field-names appropriately\n\nThis backend is currently maintained by:\n\n* [Nick Moore](https://github.com/kelnage)\n* [Mostafa Moradian](https://github.com/mostafa)\n\n## Installation\n\nTo get started developing/testing pySigma-backend-loki, these steps may help you get started:\n\n1. [Install poetry](https://python-poetry.org/docs/#installation)\n2. Clone this repository and open a terminal/shell in the top-level directory\n3. Run `poetry install` to install the Python dependencies\n4. Run `poetry shell` to activate the poetry environment\n5. Check it all works by running `poetry run pytest`\n6. (Optional) If you wish to validate the generated rules using sigma\\_backend\\_tester.py, install\n   [LogCLI](https://grafana.com/docs/loki/latest/tools/logcli/)\n7. (Optional, but recommended) To enable the Git hooks, run the following command from the root directory of the repository:\n```sh\ngit config --local core.hooksPath .githooks/\n```\n\n## Releasing\n\nTo release new versions of pySigma-backend-loki, we use GitHub actions to update PyPI. When the main branch is in state that is ready to release, the process is as follows:\n\n1. Determine the correct version number using the [Semantic Versioning](https://semver.org/) methodology. All version numbers should be in the format `\\d+\\.\\d+\\.\\d+(-[0-9A-Za-z-]+)?`\n2. Update [pyproject.toml](https://github.com/grafana/pySigma-backend-loki/blob/main/pyproject.toml) with the new version number\n3. Commit and push the change to GitHub, and validate that the GitHub actions tests pass\n4. Create a signed tag for the release, named the version number prefixed with a v, e.g., `git tag --sign --message="Release vX.X.X" vX.X.X`\n5. Push the tag to GitHub, e.g., `git push --tags`, and validate that the release to the test instance of PyPI is successful\n6. Run `poetry build` to produce distributable versions in `dist/`\n7. Create a release in GitHub against the appropriate tag. If the version number starts with `v0`, or ends with `-alpha/beta` etc., mark it as a pre-release, and attach the distributable files to the release\n8. Validate that the release to PyPI GitHub action is successful\n\n## Work in progress\n\nThese features are currently either WIP or are planned to be implemented in the near future.\n\n* Various processing pipelines for other applications and log sources\n* Generating more accurate log stream selectors based on logsource\n* Translate field names in Sigma signatures into relevant labels for Loki using pipelines\n\n## Won\'t implement (probably)\n\nThese features are not easily supported by the backend, and hence are unlikely to be implemented.\n\n* More complex keyword/line filter searches than ANDs of ORs\n',
+    'long_description': '![PyPI](https://img.shields.io/pypi/v/pysigma-backend-loki)\n![Tests](https://github.com/grafana/pySigma-backend-loki/actions/workflows/test.yml/badge.svg)\n[![Coverage Status](https://coveralls.io/repos/github/grafana/pySigma-backend-loki/badge.svg?branch=main&t=lvM1Ns)](https://coveralls.io/github/grafana/pySigma-backend-loki?branch=main)\n\n# pySigma Loki Backend\n\nThis is the Loki backend for pySigma. It provides the package `sigma.backends.loki` with the `LogQLBackend` class.\n\nIt supports the following output formats:\n\n* `default`: plain Loki LogQL queries\n* `ruler`: creates Loki LogQL queries in the ruler (YAML) format for generating alerts\n\nIt includes the following pipeline transformations in `sigma.pipelines.loki`:\n\n* `SetCustomAttributeTransformation`: adds a specified custom attribute to a rule, which can be used to introduce a [stream selector](https://grafana.com/docs/loki/latest/logql/log_queries/#log-stream-selector) or [parser expression](https://grafana.com/docs/loki/latest/logql/log_queries/#parser-expression) into the generated query\n  * The `LokiCustomAttributes` enum contains the relevant custom attribute names used by the backend\n\nFurther, it contains the processing pipelines in `sigma.pipelines.loki`:\n\n* `loki_log_parser`: converts field names to logfmt labels used by Grafana\n* `loki_promtail_sysmon`: parse and adjust field names for Windows sysmon data produced by promtail\n  * Note: most rules lack the `sysmon` service tag, and hence this pipeline should be used in combination with the [generic sysmon pipeline](https://github.com/SigmaHQ/pySigma-pipeline-sysmon)\n* `loki_okta_system_log`: parse the Okta System Log event json, adjusting field-names appropriately\n\nWhen converting rules into queries, the backend has the following optional arguments:\n\n* `add_line_filters` (boolean, default: `False`): if `True`, attempts to infer and add new line filters to queries without line filters, to [improve Loki query performance](https://grafana.com/docs/loki/latest/logql/log_queries/#line-filter-expression)\n* `case_insensitive` (boolean, default: `True`): if `False`, defaults to generating case-sensitive query filters, instead of case-insensitive filters that [the Sigma specification expects](https://github.com/SigmaHQ/sigma-specification/blob/main/Sigma_specification.md#general), trading between Loki query performance and potentially missing data with unexpected casing\n  * Note: if the generated query will be executed on Loki v2.8.2 or older, this argument **should** be set to `False`, as these versions of Loki may contain issues with case-insensitive filters, which cause such queries to fail to match desired data\n\nThis backend is currently maintained by:\n\n* [Nick Moore](https://github.com/kelnage)\n* [Mostafa Moradian](https://github.com/mostafa)\n\n## Installation\n\nTo get started developing/testing pySigma-backend-loki, these steps may help you get started:\n\n1. [Install poetry](https://python-poetry.org/docs/#installation)\n2. Clone this repository and open a terminal/shell in the top-level directory\n3. Run `poetry install` to install the Python dependencies\n4. Run `poetry shell` to activate the poetry environment\n5. Check it all works by running `poetry run pytest`\n6. (Optional) If you wish to validate the generated rules using sigma\\_backend\\_tester.py, install\n   [LogCLI](https://grafana.com/docs/loki/latest/tools/logcli/)\n7. (Optional, but recommended) To enable the Git hooks, run the following command from the root directory of the repository:\n```sh\ngit config --local core.hooksPath .githooks/\n```\n\n## Releasing\n\nTo release new versions of pySigma-backend-loki, we use GitHub actions to update PyPI. When the main branch is in state that is ready to release, the process is as follows:\n\n1. Determine the correct version number using the [Semantic Versioning](https://semver.org/) methodology. All version numbers should be in the format `\\d+\\.\\d+\\.\\d+(-[0-9A-Za-z-]+)?`\n2. Update [pyproject.toml](https://github.com/grafana/pySigma-backend-loki/blob/main/pyproject.toml) with the new version number\n3. Commit and push the change to GitHub, and validate that the GitHub actions tests pass\n4. Create a signed tag for the release, named the version number prefixed with a v, e.g., `git tag --sign --message="Release vX.X.X" vX.X.X`\n5. Push the tag to GitHub, e.g., `git push --tags`, and validate that the release to the test instance of PyPI is successful\n6. Run `poetry build` to produce distributable versions in `dist/`\n7. Create a release in GitHub against the appropriate tag. If the version number starts with `v0`, or ends with `-alpha/beta` etc., mark it as a pre-release, and attach the distributable files to the release\n8. Validate that the release to PyPI GitHub action is successful\n\n## Work in progress\n\nThese features are currently either WIP or are planned to be implemented in the near future.\n\n* Various processing pipelines for other applications and log sources\n* Generating more accurate log stream selectors based on logsource\n* Translate field names in Sigma signatures into relevant labels for Loki using pipelines\n\n## Won\'t implement (probably)\n\nThese features are not easily supported by the backend, and hence are unlikely to be implemented.\n\n* More complex keyword/line filter searches than ANDs of ORs\n',
     'author': 'Nick Moore',
     'author_email': 'nicholas.moore@grafana.com',
     'maintainer': 'None',
     'maintainer_email': 'None',
     'url': 'https://github.com/grafana/pySigma-backend-loki',
     'packages': packages,
     'package_data': package_data,
```

### Comparing `pysigma_backend_loki-0.8.0/PKG-INFO` & `pysigma_backend_loki-0.9.0/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,23 +1,23 @@
 Metadata-Version: 2.1
 Name: pysigma-backend-loki
-Version: 0.8.0
+Version: 0.9.0
 Summary: pySigma Loki backend
 Home-page: https://github.com/grafana/pySigma-backend-loki
 License: AGPL-3.0-only
 Author: Nick Moore
 Author-email: nicholas.moore@grafana.com
 Requires-Python: >=3.8,<4.0
 Classifier: License :: OSI Approved :: GNU Affero General Public License v3
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
-Requires-Dist: pysigma (>=0.9.6,<0.10.0)
+Requires-Dist: pysigma (>=0.9.11,<0.10.0)
 Requires-Dist: pysigma-pipeline-sysmon (>=1.0.1,<2.0.0)
 Project-URL: Repository, https://github.com/grafana/pySigma-backend-loki
 Description-Content-Type: text/markdown
 
 ![PyPI](https://img.shields.io/pypi/v/pysigma-backend-loki)
 ![Tests](https://github.com/grafana/pySigma-backend-loki/actions/workflows/test.yml/badge.svg)
 [![Coverage Status](https://coveralls.io/repos/github/grafana/pySigma-backend-loki/badge.svg?branch=main&t=lvM1Ns)](https://coveralls.io/github/grafana/pySigma-backend-loki?branch=main)
@@ -35,17 +35,23 @@
 
 * `SetCustomAttributeTransformation`: adds a specified custom attribute to a rule, which can be used to introduce a [stream selector](https://grafana.com/docs/loki/latest/logql/log_queries/#log-stream-selector) or [parser expression](https://grafana.com/docs/loki/latest/logql/log_queries/#parser-expression) into the generated query
   * The `LokiCustomAttributes` enum contains the relevant custom attribute names used by the backend
 
 Further, it contains the processing pipelines in `sigma.pipelines.loki`:
 
 * `loki_log_parser`: converts field names to logfmt labels used by Grafana
-* `loki_promtail_sysmon_message`: parse and adjust field names for Windows sysmon data produced by promtail
+* `loki_promtail_sysmon`: parse and adjust field names for Windows sysmon data produced by promtail
   * Note: most rules lack the `sysmon` service tag, and hence this pipeline should be used in combination with the [generic sysmon pipeline](https://github.com/SigmaHQ/pySigma-pipeline-sysmon)
-* `loki_okta_system_log_json`: parse the Okta System Log event json, adjusting field-names appropriately
+* `loki_okta_system_log`: parse the Okta System Log event json, adjusting field-names appropriately
+
+When converting rules into queries, the backend has the following optional arguments:
+
+* `add_line_filters` (boolean, default: `False`): if `True`, attempts to infer and add new line filters to queries without line filters, to [improve Loki query performance](https://grafana.com/docs/loki/latest/logql/log_queries/#line-filter-expression)
+* `case_insensitive` (boolean, default: `True`): if `False`, defaults to generating case-sensitive query filters, instead of case-insensitive filters that [the Sigma specification expects](https://github.com/SigmaHQ/sigma-specification/blob/main/Sigma_specification.md#general), trading between Loki query performance and potentially missing data with unexpected casing
+  * Note: if the generated query will be executed on Loki v2.8.2 or older, this argument **should** be set to `False`, as these versions of Loki may contain issues with case-insensitive filters, which cause such queries to fail to match desired data
 
 This backend is currently maintained by:
 
 * [Nick Moore](https://github.com/kelnage)
 * [Mostafa Moradian](https://github.com/mostafa)
 
 ## Installation
```

