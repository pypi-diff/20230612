# Comparing `tmp/cyclonedx_editor_validator-0.6.0.tar.gz` & `tmp/cyclonedx_editor_validator-0.6.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "cyclonedx_editor_validator-0.6.0.tar", max compression
+gzip compressed data, was "cyclonedx_editor_validator-0.6.1.tar", max compression
```

## Comparing `cyclonedx_editor_validator-0.6.0.tar` & `cyclonedx_editor_validator-0.6.1.tar`

### file list

```diff
@@ -1,49 +1,49 @@
--rw-r--r--   0        0        0    35114 2023-06-12 07:13:51.172301 cyclonedx_editor_validator-0.6.0/LICENSE
--rw-r--r--   0        0        0     2234 2023-06-12 07:13:51.172301 cyclonedx_editor_validator-0.6.0/README.md
--rw-r--r--   0        0        0       34 2023-06-12 07:13:51.172301 cyclonedx_editor_validator-0.6.0/cdxev/__init__.py
--rw-r--r--   0        0        0    20098 2023-06-12 07:13:51.172301 cyclonedx_editor_validator-0.6.0/cdxev/__main__.py
--rw-r--r--   0        0        0      410 2023-06-12 07:13:51.172301 cyclonedx_editor_validator-0.6.0/cdxev/amend/__init__.py
--rw-r--r--   0        0        0     1218 2023-06-12 07:13:51.172301 cyclonedx_editor_validator-0.6.0/cdxev/amend/command.py
--rw-r--r--   0        0        0    59830 2023-06-12 07:13:51.172301 cyclonedx_editor_validator-0.6.0/cdxev/amend/license_name_id_map.json
--rw-r--r--   0        0        0     6560 2023-06-12 07:13:51.172301 cyclonedx_editor_validator-0.6.0/cdxev/amend/operations.py
--rw-r--r--   0        0        0     2062 2023-06-12 07:13:51.176301 cyclonedx_editor_validator-0.6.0/cdxev/amend/replace_license_name_with_id.py
--rw-r--r--   0        0        0        0 2023-06-12 07:13:51.176301 cyclonedx_editor_validator-0.6.0/cdxev/auxiliary/__init__.py
--rw-r--r--   0        0        0     5793 2023-06-12 07:13:51.176301 cyclonedx_editor_validator-0.6.0/cdxev/auxiliary/identity.py
--rw-r--r--   0        0        0     3854 2023-06-12 07:13:51.176301 cyclonedx_editor_validator-0.6.0/cdxev/auxiliary/output.py
--rw-r--r--   0        0        0    10454 2023-06-12 07:13:51.176301 cyclonedx_editor_validator-0.6.0/cdxev/auxiliary/sbomFunctions.py
--rw-r--r--   0        0        0        0 2023-06-12 07:13:51.176301 cyclonedx_editor_validator-0.6.0/cdxev/auxiliary/schema/__init__.py
--rw-r--r--   0        0        0    13619 2023-06-12 07:13:51.176301 cyclonedx_editor_validator-0.6.0/cdxev/auxiliary/schema/bom-1.0.xsd
--rw-r--r--   0        0        0    39484 2023-06-12 07:13:51.176301 cyclonedx_editor_validator-0.6.0/cdxev/auxiliary/schema/bom-1.1.xsd
--rw-r--r--   0        0        0    37056 2023-06-12 07:13:51.176301 cyclonedx_editor_validator-0.6.0/cdxev/auxiliary/schema/bom-1.2-strict.schema.json
--rw-r--r--   0        0        0    36058 2023-06-12 07:13:51.176301 cyclonedx_editor_validator-0.6.0/cdxev/auxiliary/schema/bom-1.2.schema.json
--rw-r--r--   0        0        0    76147 2023-06-12 07:13:51.176301 cyclonedx_editor_validator-0.6.0/cdxev/auxiliary/schema/bom-1.2.xsd
--rw-r--r--   0        0        0    43822 2023-06-12 07:13:51.176301 cyclonedx_editor_validator-0.6.0/cdxev/auxiliary/schema/bom-1.3-custom.schema.json
--rw-r--r--   0        0        0    40239 2023-06-12 07:13:51.176301 cyclonedx_editor_validator-0.6.0/cdxev/auxiliary/schema/bom-1.3-strict.schema.json
--rw-r--r--   0        0        0    23176 2023-06-12 07:13:51.176301 cyclonedx_editor_validator-0.6.0/cdxev/auxiliary/schema/bom-1.3.proto
--rw-r--r--   0        0        0    39180 2023-06-12 07:13:51.176301 cyclonedx_editor_validator-0.6.0/cdxev/auxiliary/schema/bom-1.3.schema.json
--rw-r--r--   0        0        0    88384 2023-06-12 07:13:51.176301 cyclonedx_editor_validator-0.6.0/cdxev/auxiliary/schema/bom-1.3.xsd
--rw-r--r--   0        0        0    76794 2023-06-12 07:13:51.176301 cyclonedx_editor_validator-0.6.0/cdxev/auxiliary/schema/bom-1.4-custom.schema.json
--rw-r--r--   0        0        0    34897 2023-06-12 07:13:51.176301 cyclonedx_editor_validator-0.6.0/cdxev/auxiliary/schema/bom-1.4.proto
--rw-r--r--   0        0        0    72249 2023-06-12 07:13:51.176301 cyclonedx_editor_validator-0.6.0/cdxev/auxiliary/schema/bom-1.4.schema.json
--rw-r--r--   0        0        0   133616 2023-06-12 07:13:51.176301 cyclonedx_editor_validator-0.6.0/cdxev/auxiliary/schema/bom-1.4.xsd
--rw-r--r--   0        0        0     9063 2023-06-12 07:13:51.176301 cyclonedx_editor_validator-0.6.0/cdxev/auxiliary/schema/ext/bom-descriptor-0.9.xsd
--rw-r--r--   0        0        0     8233 2023-06-12 07:13:51.176301 cyclonedx_editor_validator-0.6.0/cdxev/auxiliary/schema/ext/bom-descriptor-1.0.xsd
--rw-r--r--   0        0        0     3146 2023-06-12 07:13:51.176301 cyclonedx_editor_validator-0.6.0/cdxev/auxiliary/schema/ext/dependency-graph-1.0.xsd
--rw-r--r--   0        0        0     6380 2023-06-12 07:13:51.176301 cyclonedx_editor_validator-0.6.0/cdxev/auxiliary/schema/ext/vulnerability-1.0-SNAPSHOT.schema.json
--rw-r--r--   0        0        0    14195 2023-06-12 07:13:51.176301 cyclonedx_editor_validator-0.6.0/cdxev/auxiliary/schema/ext/vulnerability-1.0.xsd
--rw-r--r--   0        0        0     8210 2023-06-12 07:13:51.176301 cyclonedx_editor_validator-0.6.0/cdxev/auxiliary/schema/jsf-0.82.schema.json
--rw-r--r--   0        0        0    10482 2023-06-12 07:13:51.176301 cyclonedx_editor_validator-0.6.0/cdxev/auxiliary/schema/spdx.schema.json
--rw-r--r--   0        0        0   125048 2023-06-12 07:13:51.176301 cyclonedx_editor_validator-0.6.0/cdxev/auxiliary/schema/spdx.xsd
--rw-r--r--   0        0        0     5646 2023-06-12 07:13:51.176301 cyclonedx_editor_validator-0.6.0/cdxev/build_public_bom.py
--rw-r--r--   0        0        0     2642 2023-06-12 07:13:51.176301 cyclonedx_editor_validator-0.6.0/cdxev/error.py
--rw-r--r--   0        0        0     2763 2023-06-12 07:13:51.176301 cyclonedx_editor_validator-0.6.0/cdxev/log.py
--rw-r--r--   0        0        0    18104 2023-06-12 07:13:51.176301 cyclonedx_editor_validator-0.6.0/cdxev/merge.py
--rw-r--r--   0        0        0     2702 2023-06-12 07:13:51.176301 cyclonedx_editor_validator-0.6.0/cdxev/mergeVex.py
--rw-r--r--   0        0        0      135 2023-06-12 07:13:51.176301 cyclonedx_editor_validator-0.6.0/cdxev/pkg.py
--rw-r--r--   0        0        0     7211 2023-06-12 07:13:51.176301 cyclonedx_editor_validator-0.6.0/cdxev/set.py
--rw-r--r--   0        0        0       65 2023-06-12 07:13:51.176301 cyclonedx_editor_validator-0.6.0/cdxev/validator/__init__.py
--rw-r--r--   0        0        0     3766 2023-06-12 07:13:51.176301 cyclonedx_editor_validator-0.6.0/cdxev/validator/helper.py
--rw-r--r--   0        0        0     7098 2023-06-12 07:13:51.176301 cyclonedx_editor_validator-0.6.0/cdxev/validator/validate.py
--rw-r--r--   0        0        0     3022 2023-06-12 07:13:51.176301 cyclonedx_editor_validator-0.6.0/cdxev/validator/warningsngreport.py
--rw-r--r--   0        0        0     1684 2023-06-12 07:14:08.605377 cyclonedx_editor_validator-0.6.0/pyproject.toml
--rw-r--r--   0        0        0     3228 1970-01-01 00:00:00.000000 cyclonedx_editor_validator-0.6.0/PKG-INFO
+-rw-r--r--   0        0        0    35114 2023-06-12 07:30:48.257530 cyclonedx_editor_validator-0.6.1/LICENSE
+-rw-r--r--   0        0        0     2429 2023-06-12 07:30:48.257530 cyclonedx_editor_validator-0.6.1/README.md
+-rw-r--r--   0        0        0       34 2023-06-12 07:30:48.257530 cyclonedx_editor_validator-0.6.1/cdxev/__init__.py
+-rw-r--r--   0        0        0    20098 2023-06-12 07:30:48.257530 cyclonedx_editor_validator-0.6.1/cdxev/__main__.py
+-rw-r--r--   0        0        0      410 2023-06-12 07:30:48.257530 cyclonedx_editor_validator-0.6.1/cdxev/amend/__init__.py
+-rw-r--r--   0        0        0     1218 2023-06-12 07:30:48.257530 cyclonedx_editor_validator-0.6.1/cdxev/amend/command.py
+-rw-r--r--   0        0        0    59830 2023-06-12 07:30:48.257530 cyclonedx_editor_validator-0.6.1/cdxev/amend/license_name_id_map.json
+-rw-r--r--   0        0        0     6560 2023-06-12 07:30:48.257530 cyclonedx_editor_validator-0.6.1/cdxev/amend/operations.py
+-rw-r--r--   0        0        0     2062 2023-06-12 07:30:48.257530 cyclonedx_editor_validator-0.6.1/cdxev/amend/replace_license_name_with_id.py
+-rw-r--r--   0        0        0        0 2023-06-12 07:30:48.257530 cyclonedx_editor_validator-0.6.1/cdxev/auxiliary/__init__.py
+-rw-r--r--   0        0        0     5793 2023-06-12 07:30:48.257530 cyclonedx_editor_validator-0.6.1/cdxev/auxiliary/identity.py
+-rw-r--r--   0        0        0     3854 2023-06-12 07:30:48.257530 cyclonedx_editor_validator-0.6.1/cdxev/auxiliary/output.py
+-rw-r--r--   0        0        0    10454 2023-06-12 07:30:48.257530 cyclonedx_editor_validator-0.6.1/cdxev/auxiliary/sbomFunctions.py
+-rw-r--r--   0        0        0        0 2023-06-12 07:30:48.257530 cyclonedx_editor_validator-0.6.1/cdxev/auxiliary/schema/__init__.py
+-rw-r--r--   0        0        0    13619 2023-06-12 07:30:48.257530 cyclonedx_editor_validator-0.6.1/cdxev/auxiliary/schema/bom-1.0.xsd
+-rw-r--r--   0        0        0    39484 2023-06-12 07:30:48.257530 cyclonedx_editor_validator-0.6.1/cdxev/auxiliary/schema/bom-1.1.xsd
+-rw-r--r--   0        0        0    37056 2023-06-12 07:30:48.257530 cyclonedx_editor_validator-0.6.1/cdxev/auxiliary/schema/bom-1.2-strict.schema.json
+-rw-r--r--   0        0        0    36058 2023-06-12 07:30:48.257530 cyclonedx_editor_validator-0.6.1/cdxev/auxiliary/schema/bom-1.2.schema.json
+-rw-r--r--   0        0        0    76147 2023-06-12 07:30:48.257530 cyclonedx_editor_validator-0.6.1/cdxev/auxiliary/schema/bom-1.2.xsd
+-rw-r--r--   0        0        0    43822 2023-06-12 07:30:48.257530 cyclonedx_editor_validator-0.6.1/cdxev/auxiliary/schema/bom-1.3-custom.schema.json
+-rw-r--r--   0        0        0    40239 2023-06-12 07:30:48.257530 cyclonedx_editor_validator-0.6.1/cdxev/auxiliary/schema/bom-1.3-strict.schema.json
+-rw-r--r--   0        0        0    23176 2023-06-12 07:30:48.257530 cyclonedx_editor_validator-0.6.1/cdxev/auxiliary/schema/bom-1.3.proto
+-rw-r--r--   0        0        0    39180 2023-06-12 07:30:48.257530 cyclonedx_editor_validator-0.6.1/cdxev/auxiliary/schema/bom-1.3.schema.json
+-rw-r--r--   0        0        0    88384 2023-06-12 07:30:48.257530 cyclonedx_editor_validator-0.6.1/cdxev/auxiliary/schema/bom-1.3.xsd
+-rw-r--r--   0        0        0    76794 2023-06-12 07:30:48.261530 cyclonedx_editor_validator-0.6.1/cdxev/auxiliary/schema/bom-1.4-custom.schema.json
+-rw-r--r--   0        0        0    34897 2023-06-12 07:30:48.261530 cyclonedx_editor_validator-0.6.1/cdxev/auxiliary/schema/bom-1.4.proto
+-rw-r--r--   0        0        0    72249 2023-06-12 07:30:48.261530 cyclonedx_editor_validator-0.6.1/cdxev/auxiliary/schema/bom-1.4.schema.json
+-rw-r--r--   0        0        0   133616 2023-06-12 07:30:48.261530 cyclonedx_editor_validator-0.6.1/cdxev/auxiliary/schema/bom-1.4.xsd
+-rw-r--r--   0        0        0     9063 2023-06-12 07:30:48.261530 cyclonedx_editor_validator-0.6.1/cdxev/auxiliary/schema/ext/bom-descriptor-0.9.xsd
+-rw-r--r--   0        0        0     8233 2023-06-12 07:30:48.261530 cyclonedx_editor_validator-0.6.1/cdxev/auxiliary/schema/ext/bom-descriptor-1.0.xsd
+-rw-r--r--   0        0        0     3146 2023-06-12 07:30:48.261530 cyclonedx_editor_validator-0.6.1/cdxev/auxiliary/schema/ext/dependency-graph-1.0.xsd
+-rw-r--r--   0        0        0     6380 2023-06-12 07:30:48.261530 cyclonedx_editor_validator-0.6.1/cdxev/auxiliary/schema/ext/vulnerability-1.0-SNAPSHOT.schema.json
+-rw-r--r--   0        0        0    14195 2023-06-12 07:30:48.261530 cyclonedx_editor_validator-0.6.1/cdxev/auxiliary/schema/ext/vulnerability-1.0.xsd
+-rw-r--r--   0        0        0     8210 2023-06-12 07:30:48.261530 cyclonedx_editor_validator-0.6.1/cdxev/auxiliary/schema/jsf-0.82.schema.json
+-rw-r--r--   0        0        0    10482 2023-06-12 07:30:48.261530 cyclonedx_editor_validator-0.6.1/cdxev/auxiliary/schema/spdx.schema.json
+-rw-r--r--   0        0        0   125048 2023-06-12 07:30:48.261530 cyclonedx_editor_validator-0.6.1/cdxev/auxiliary/schema/spdx.xsd
+-rw-r--r--   0        0        0     5646 2023-06-12 07:30:48.261530 cyclonedx_editor_validator-0.6.1/cdxev/build_public_bom.py
+-rw-r--r--   0        0        0     2642 2023-06-12 07:30:48.261530 cyclonedx_editor_validator-0.6.1/cdxev/error.py
+-rw-r--r--   0        0        0     2763 2023-06-12 07:30:48.261530 cyclonedx_editor_validator-0.6.1/cdxev/log.py
+-rw-r--r--   0        0        0    18104 2023-06-12 07:30:48.261530 cyclonedx_editor_validator-0.6.1/cdxev/merge.py
+-rw-r--r--   0        0        0     2702 2023-06-12 07:30:48.261530 cyclonedx_editor_validator-0.6.1/cdxev/mergeVex.py
+-rw-r--r--   0        0        0      135 2023-06-12 07:30:48.261530 cyclonedx_editor_validator-0.6.1/cdxev/pkg.py
+-rw-r--r--   0        0        0     7211 2023-06-12 07:30:48.261530 cyclonedx_editor_validator-0.6.1/cdxev/set.py
+-rw-r--r--   0        0        0       65 2023-06-12 07:30:48.261530 cyclonedx_editor_validator-0.6.1/cdxev/validator/__init__.py
+-rw-r--r--   0        0        0     3766 2023-06-12 07:30:48.261530 cyclonedx_editor_validator-0.6.1/cdxev/validator/helper.py
+-rw-r--r--   0        0        0     7098 2023-06-12 07:30:48.261530 cyclonedx_editor_validator-0.6.1/cdxev/validator/validate.py
+-rw-r--r--   0        0        0     3022 2023-06-12 07:30:48.261530 cyclonedx_editor_validator-0.6.1/cdxev/validator/warningsngreport.py
+-rw-r--r--   0        0        0     1684 2023-06-12 07:31:06.265780 cyclonedx_editor_validator-0.6.1/pyproject.toml
+-rw-r--r--   0        0        0     3423 1970-01-01 00:00:00.000000 cyclonedx_editor_validator-0.6.1/PKG-INFO
```

### Comparing `cyclonedx_editor_validator-0.6.0/LICENSE` & `cyclonedx_editor_validator-0.6.1/LICENSE`

 * *Files identical despite different names*

### Comparing `cyclonedx_editor_validator-0.6.0/README.md` & `cyclonedx_editor_validator-0.6.1/README.md`

 * *Files 11% similar despite different names*

```diff
@@ -8,20 +8,20 @@
 # CycloneDX Editor/Validator
 
 This command-line tool performs various actions on [CycloneDX](https://cyclonedx.org/) SBOMs. It allows you to modify and validate your SBOMs.
 
 ## Documentation
 
 * [Official documentation](https://festo-se.github.io/cyclonedx-editor-validator).
-* [Available commands](docs/available_commands.md).
-* [Known Limitations](docs/known_limitations.md).
+* [Available commands](https://github.com/Festo-se/cyclonedx-editor-validator/blob/main/docs/available_commands.md).
+* [Known Limitations](https://github.com/Festo-se/cyclonedx-editor-validator/blob/main/docs/known_limitations.md).
 
 ## Contributing
 
-See our [Contributing guidelines](docs/CONTRIBUTING.md).
+See our [Contributing guidelines](https://github.com/Festo-se/cyclonedx-editor-validator/blob/main/docs/CONTRIBUTING.md).
 
 ## To-do
 
 * **Add possibility for adding a configuration-file.** This could be useful for e.g. configuration of validator as the used flags remain the same.
 * **Add plausibility check.** This would be used for e.g. finding orphaned `bom-refs`. One further use case would be plausibility check of VEX.
 * **Use model from ["official" python lib](https://github.com/CycloneDX/cyclonedx-python-lib/tree/main).** This helps working on classes instead of dicts, which would make our code more robust.
 * **Add function for initialization of a SBOM.** Create initial SBOM, so that somebody creating a SBOM manually has a first draft.
```

### Comparing `cyclonedx_editor_validator-0.6.0/cdxev/__main__.py` & `cyclonedx_editor_validator-0.6.1/cdxev/__main__.py`

 * *Files identical despite different names*

### Comparing `cyclonedx_editor_validator-0.6.0/cdxev/amend/command.py` & `cyclonedx_editor_validator-0.6.1/cdxev/amend/command.py`

 * *Files identical despite different names*

### Comparing `cyclonedx_editor_validator-0.6.0/cdxev/amend/license_name_id_map.json` & `cyclonedx_editor_validator-0.6.1/cdxev/amend/license_name_id_map.json`

 * *Files identical despite different names*

### Comparing `cyclonedx_editor_validator-0.6.0/cdxev/amend/operations.py` & `cyclonedx_editor_validator-0.6.1/cdxev/amend/operations.py`

 * *Files identical despite different names*

### Comparing `cyclonedx_editor_validator-0.6.0/cdxev/amend/replace_license_name_with_id.py` & `cyclonedx_editor_validator-0.6.1/cdxev/amend/replace_license_name_with_id.py`

 * *Files identical despite different names*

### Comparing `cyclonedx_editor_validator-0.6.0/cdxev/auxiliary/identity.py` & `cyclonedx_editor_validator-0.6.1/cdxev/auxiliary/identity.py`

 * *Files identical despite different names*

### Comparing `cyclonedx_editor_validator-0.6.0/cdxev/auxiliary/output.py` & `cyclonedx_editor_validator-0.6.1/cdxev/auxiliary/output.py`

 * *Files identical despite different names*

### Comparing `cyclonedx_editor_validator-0.6.0/cdxev/auxiliary/sbomFunctions.py` & `cyclonedx_editor_validator-0.6.1/cdxev/auxiliary/sbomFunctions.py`

 * *Files identical despite different names*

### Comparing `cyclonedx_editor_validator-0.6.0/cdxev/auxiliary/schema/bom-1.0.xsd` & `cyclonedx_editor_validator-0.6.1/cdxev/auxiliary/schema/bom-1.0.xsd`

 * *Files identical despite different names*

### Comparing `cyclonedx_editor_validator-0.6.0/cdxev/auxiliary/schema/bom-1.1.xsd` & `cyclonedx_editor_validator-0.6.1/cdxev/auxiliary/schema/bom-1.1.xsd`

 * *Files identical despite different names*

### Comparing `cyclonedx_editor_validator-0.6.0/cdxev/auxiliary/schema/bom-1.2-strict.schema.json` & `cyclonedx_editor_validator-0.6.1/cdxev/auxiliary/schema/bom-1.2-strict.schema.json`

 * *Files identical despite different names*

### Comparing `cyclonedx_editor_validator-0.6.0/cdxev/auxiliary/schema/bom-1.2.schema.json` & `cyclonedx_editor_validator-0.6.1/cdxev/auxiliary/schema/bom-1.2.schema.json`

 * *Files identical despite different names*

### Comparing `cyclonedx_editor_validator-0.6.0/cdxev/auxiliary/schema/bom-1.2.xsd` & `cyclonedx_editor_validator-0.6.1/cdxev/auxiliary/schema/bom-1.2.xsd`

 * *Files identical despite different names*

### Comparing `cyclonedx_editor_validator-0.6.0/cdxev/auxiliary/schema/bom-1.3-custom.schema.json` & `cyclonedx_editor_validator-0.6.1/cdxev/auxiliary/schema/bom-1.3-custom.schema.json`

 * *Files identical despite different names*

### Comparing `cyclonedx_editor_validator-0.6.0/cdxev/auxiliary/schema/bom-1.3-strict.schema.json` & `cyclonedx_editor_validator-0.6.1/cdxev/auxiliary/schema/bom-1.3-strict.schema.json`

 * *Files identical despite different names*

### Comparing `cyclonedx_editor_validator-0.6.0/cdxev/auxiliary/schema/bom-1.3.proto` & `cyclonedx_editor_validator-0.6.1/cdxev/auxiliary/schema/bom-1.3.proto`

 * *Files identical despite different names*

### Comparing `cyclonedx_editor_validator-0.6.0/cdxev/auxiliary/schema/bom-1.3.schema.json` & `cyclonedx_editor_validator-0.6.1/cdxev/auxiliary/schema/bom-1.3.schema.json`

 * *Files identical despite different names*

### Comparing `cyclonedx_editor_validator-0.6.0/cdxev/auxiliary/schema/bom-1.3.xsd` & `cyclonedx_editor_validator-0.6.1/cdxev/auxiliary/schema/bom-1.3.xsd`

 * *Files identical despite different names*

### Comparing `cyclonedx_editor_validator-0.6.0/cdxev/auxiliary/schema/bom-1.4-custom.schema.json` & `cyclonedx_editor_validator-0.6.1/cdxev/auxiliary/schema/bom-1.4-custom.schema.json`

 * *Files identical despite different names*

### Comparing `cyclonedx_editor_validator-0.6.0/cdxev/auxiliary/schema/bom-1.4.proto` & `cyclonedx_editor_validator-0.6.1/cdxev/auxiliary/schema/bom-1.4.proto`

 * *Files identical despite different names*

### Comparing `cyclonedx_editor_validator-0.6.0/cdxev/auxiliary/schema/bom-1.4.schema.json` & `cyclonedx_editor_validator-0.6.1/cdxev/auxiliary/schema/bom-1.4.schema.json`

 * *Files identical despite different names*

### Comparing `cyclonedx_editor_validator-0.6.0/cdxev/auxiliary/schema/bom-1.4.xsd` & `cyclonedx_editor_validator-0.6.1/cdxev/auxiliary/schema/bom-1.4.xsd`

 * *Files identical despite different names*

### Comparing `cyclonedx_editor_validator-0.6.0/cdxev/auxiliary/schema/ext/bom-descriptor-0.9.xsd` & `cyclonedx_editor_validator-0.6.1/cdxev/auxiliary/schema/ext/bom-descriptor-0.9.xsd`

 * *Files identical despite different names*

### Comparing `cyclonedx_editor_validator-0.6.0/cdxev/auxiliary/schema/ext/bom-descriptor-1.0.xsd` & `cyclonedx_editor_validator-0.6.1/cdxev/auxiliary/schema/ext/bom-descriptor-1.0.xsd`

 * *Files identical despite different names*

### Comparing `cyclonedx_editor_validator-0.6.0/cdxev/auxiliary/schema/ext/dependency-graph-1.0.xsd` & `cyclonedx_editor_validator-0.6.1/cdxev/auxiliary/schema/ext/dependency-graph-1.0.xsd`

 * *Files identical despite different names*

### Comparing `cyclonedx_editor_validator-0.6.0/cdxev/auxiliary/schema/ext/vulnerability-1.0-SNAPSHOT.schema.json` & `cyclonedx_editor_validator-0.6.1/cdxev/auxiliary/schema/ext/vulnerability-1.0-SNAPSHOT.schema.json`

 * *Files identical despite different names*

### Comparing `cyclonedx_editor_validator-0.6.0/cdxev/auxiliary/schema/ext/vulnerability-1.0.xsd` & `cyclonedx_editor_validator-0.6.1/cdxev/auxiliary/schema/ext/vulnerability-1.0.xsd`

 * *Files identical despite different names*

### Comparing `cyclonedx_editor_validator-0.6.0/cdxev/auxiliary/schema/jsf-0.82.schema.json` & `cyclonedx_editor_validator-0.6.1/cdxev/auxiliary/schema/jsf-0.82.schema.json`

 * *Files identical despite different names*

### Comparing `cyclonedx_editor_validator-0.6.0/cdxev/auxiliary/schema/spdx.schema.json` & `cyclonedx_editor_validator-0.6.1/cdxev/auxiliary/schema/spdx.schema.json`

 * *Files identical despite different names*

### Comparing `cyclonedx_editor_validator-0.6.0/cdxev/auxiliary/schema/spdx.xsd` & `cyclonedx_editor_validator-0.6.1/cdxev/auxiliary/schema/spdx.xsd`

 * *Files identical despite different names*

### Comparing `cyclonedx_editor_validator-0.6.0/cdxev/build_public_bom.py` & `cyclonedx_editor_validator-0.6.1/cdxev/build_public_bom.py`

 * *Files identical despite different names*

### Comparing `cyclonedx_editor_validator-0.6.0/cdxev/error.py` & `cyclonedx_editor_validator-0.6.1/cdxev/error.py`

 * *Files identical despite different names*

### Comparing `cyclonedx_editor_validator-0.6.0/cdxev/log.py` & `cyclonedx_editor_validator-0.6.1/cdxev/log.py`

 * *Files identical despite different names*

### Comparing `cyclonedx_editor_validator-0.6.0/cdxev/merge.py` & `cyclonedx_editor_validator-0.6.1/cdxev/merge.py`

 * *Files identical despite different names*

### Comparing `cyclonedx_editor_validator-0.6.0/cdxev/mergeVex.py` & `cyclonedx_editor_validator-0.6.1/cdxev/mergeVex.py`

 * *Files identical despite different names*

### Comparing `cyclonedx_editor_validator-0.6.0/cdxev/set.py` & `cyclonedx_editor_validator-0.6.1/cdxev/set.py`

 * *Files identical despite different names*

### Comparing `cyclonedx_editor_validator-0.6.0/cdxev/validator/helper.py` & `cyclonedx_editor_validator-0.6.1/cdxev/validator/helper.py`

 * *Files identical despite different names*

### Comparing `cyclonedx_editor_validator-0.6.0/cdxev/validator/validate.py` & `cyclonedx_editor_validator-0.6.1/cdxev/validator/validate.py`

 * *Files identical despite different names*

### Comparing `cyclonedx_editor_validator-0.6.0/cdxev/validator/warningsngreport.py` & `cyclonedx_editor_validator-0.6.1/cdxev/validator/warningsngreport.py`

 * *Files identical despite different names*

### Comparing `cyclonedx_editor_validator-0.6.0/pyproject.toml` & `cyclonedx_editor_validator-0.6.1/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "cyclonedx-editor-validator"
-version = "v0.6.0"
+version = "v0.6.1"
 description = "Tool for creating, modifying and validating CycloneDX SBOMs."
 authors = [
     "Aleg Vilinski <aleg.vilinski@festo.com>",
     "Christian Beck <christian.beck@festo.com>",
     "Moritz Marseu <moritz.marseu@festo.com>"
 ]
 license = "GPL-3.0-only"
```

### Comparing `cyclonedx_editor_validator-0.6.0/PKG-INFO` & `cyclonedx_editor_validator-0.6.1/PKG-INFO`

 * *Files 9% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cyclonedx-editor-validator
-Version: 0.6.0
+Version: 0.6.1
 Summary: Tool for creating, modifying and validating CycloneDX SBOMs.
 License: GPL-3.0-only
 Author: Aleg Vilinski
 Author-email: aleg.vilinski@festo.com
 Requires-Python: >=3.9.0,<4.0.0
 Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
 Classifier: Programming Language :: Python :: 3
@@ -29,20 +29,20 @@
 # CycloneDX Editor/Validator
 
 This command-line tool performs various actions on [CycloneDX](https://cyclonedx.org/) SBOMs. It allows you to modify and validate your SBOMs.
 
 ## Documentation
 
 * [Official documentation](https://festo-se.github.io/cyclonedx-editor-validator).
-* [Available commands](docs/available_commands.md).
-* [Known Limitations](docs/known_limitations.md).
+* [Available commands](https://github.com/Festo-se/cyclonedx-editor-validator/blob/main/docs/available_commands.md).
+* [Known Limitations](https://github.com/Festo-se/cyclonedx-editor-validator/blob/main/docs/known_limitations.md).
 
 ## Contributing
 
-See our [Contributing guidelines](docs/CONTRIBUTING.md).
+See our [Contributing guidelines](https://github.com/Festo-se/cyclonedx-editor-validator/blob/main/docs/CONTRIBUTING.md).
 
 ## To-do
 
 * **Add possibility for adding a configuration-file.** This could be useful for e.g. configuration of validator as the used flags remain the same.
 * **Add plausibility check.** This would be used for e.g. finding orphaned `bom-refs`. One further use case would be plausibility check of VEX.
 * **Use model from ["official" python lib](https://github.com/CycloneDX/cyclonedx-python-lib/tree/main).** This helps working on classes instead of dicts, which would make our code more robust.
 * **Add function for initialization of a SBOM.** Create initial SBOM, so that somebody creating a SBOM manually has a first draft.
```

