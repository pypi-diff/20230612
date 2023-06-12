# Comparing `tmp/tapipy-1.4.0a6.tar.gz` & `tmp/tapipy-1.4.0a7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "tapipy-1.4.0a6.tar", max compression
+gzip compressed data, was "tapipy-1.4.0a7.tar", max compression
```

## Comparing `tapipy-1.4.0a6.tar` & `tapipy-1.4.0a7.tar`

### file list

```diff
@@ -1,41 +1,41 @@
--rw-r--r--   0        0        0     1539 2023-06-08 15:22:35.013634 tapipy-1.4.0a6/LICENSE.md
--rw-r--r--   0        0        0     8639 2023-06-08 15:22:20.913795 tapipy-1.4.0a6/README.md
--rw-r--r--   0        0        0      973 2023-06-09 22:08:39.053961 tapipy-1.4.0a6/pyproject.toml
--rw-r--r--   0        0        0       22 2023-06-08 15:21:55.962079 tapipy-1.4.0a6/tapipy/__init__.py
--rw-r--r--   0        0        0    13502 2023-06-08 15:21:46.714184 tapipy-1.4.0a6/tapipy/actors.py
--rw-r--r--   0        0        0     2071 2023-06-08 15:21:58.470050 tapipy-1.4.0a6/tapipy/errors.py
--rw-r--r--   0        0        0    38703 2023-06-08 03:44:21.351648 tapipy-1.4.0a6/tapipy/resources/openapi_v3-actors.yml
--rw-r--r--   0        0        0    65816 2023-06-09 22:07:08.254769 tapipy-1.4.0a6/tapipy/resources/openapi_v3-apps.yml
--rw-r--r--   0        0        0    23782 2023-06-08 03:44:21.935642 tapipy-1.4.0a6/tapipy/resources/openapi_v3-authenticator.yml
--rw-r--r--   0        0        0    74553 2023-06-09 22:07:03.266813 tapipy-1.4.0a6/tapipy/resources/openapi_v3-files.yml
--rw-r--r--   0        0        0    65915 2023-06-08 03:44:29.879560 tapipy-1.4.0a6/tapipy/resources/openapi_v3-jobs.yml
--rw-r--r--   0        0        0    28625 2023-06-08 03:44:22.571636 tapipy-1.4.0a6/tapipy/resources/openapi_v3-meta.yml
--rw-r--r--   0        0        0    52671 2023-06-09 22:07:10.198752 tapipy-1.4.0a6/tapipy/resources/openapi_v3-notifications.yml
--rw-r--r--   0        0        0    33814 2023-06-08 03:44:28.195577 tapipy-1.4.0a6/tapipy/resources/openapi_v3-pgrest.yml
--rw-r--r--   0        0        0    62115 2023-06-09 22:07:07.006780 tapipy-1.4.0a6/tapipy/resources/openapi_v3-pods.yml
--rw-r--r--   0        0        0   145319 2023-06-08 03:44:24.443616 tapipy-1.4.0a6/tapipy/resources/openapi_v3-sk.yml
--rw-r--r--   0        0        0   108752 2023-06-08 03:44:25.403606 tapipy-1.4.0a6/tapipy/resources/openapi_v3-streams.yml
--rw-r--r--   0        0        0    97327 2023-06-09 22:07:04.766800 tapipy-1.4.0a6/tapipy/resources/openapi_v3-systems.yml
--rw-r--r--   0        0        0    25448 2023-06-08 03:44:26.931591 tapipy-1.4.0a6/tapipy/resources/openapi_v3-tenants.yml
--rw-r--r--   0        0        0     8406 2023-06-08 03:44:27.499585 tapipy-1.4.0a6/tapipy/resources/openapi_v3-tokens.yml
--rw-r--r--   0        0        0    87200 2023-06-09 22:07:09.574757 tapipy-1.4.0a6/tapipy/resources/openapi_v3-workflows.yml
--rw-r--r--   0        0        0      907 2023-06-09 22:07:10.198752 tapipy-1.4.0a6/tapipy/resources/resource_etags.json
--rw-r--r--   0        0        0    60738 2023-06-09 22:07:10.902746 tapipy-1.4.0a6/tapipy/specs/tapis-project-tapipy-main-tapipy-resources-openapi_v3-pods.pickle
--rw-r--r--   0        0        0    27037 2023-06-09 22:07:10.390750 tapipy-1.4.0a6/tapipy/specs/tapis-project-tapipy-prod-tapipy-resources-openapi_v3-actors.pickle
--rw-r--r--   0        0        0    72389 2023-06-09 22:07:11.034744 tapipy-1.4.0a6/tapipy/specs/tapis-project-tapipy-prod-tapipy-resources-openapi_v3-apps.pickle
--rw-r--r--   0        0        0    17736 2023-06-09 22:07:10.434750 tapipy-1.4.0a6/tapipy/specs/tapis-project-tapipy-prod-tapipy-resources-openapi_v3-authenticator.pickle
--rw-r--r--   0        0        0    56087 2023-06-09 22:07:10.522749 tapipy-1.4.0a6/tapipy/specs/tapis-project-tapipy-prod-tapipy-resources-openapi_v3-files.pickle
--rw-r--r--   0        0        0    57550 2023-06-09 22:07:10.966745 tapipy-1.4.0a6/tapipy/specs/tapis-project-tapipy-prod-tapipy-resources-openapi_v3-jobs.pickle
--rw-r--r--   0        0        0    14366 2023-06-09 22:07:10.462750 tapipy-1.4.0a6/tapipy/specs/tapis-project-tapipy-prod-tapipy-resources-openapi_v3-meta.pickle
--rw-r--r--   0        0        0    39185 2023-06-09 22:07:11.078744 tapipy-1.4.0a6/tapipy/specs/tapis-project-tapipy-prod-tapipy-resources-openapi_v3-notifications.pickle
--rw-r--r--   0        0        0    23333 2023-06-09 22:07:10.838746 tapipy-1.4.0a6/tapipy/specs/tapis-project-tapipy-prod-tapipy-resources-openapi_v3-pgrest.pickle
--rw-r--r--   0        0        0    99591 2023-06-09 22:07:10.598748 tapipy-1.4.0a6/tapipy/specs/tapis-project-tapipy-prod-tapipy-resources-openapi_v3-sk.pickle
--rw-r--r--   0        0        0    75745 2023-06-09 22:07:10.678748 tapipy-1.4.0a6/tapipy/specs/tapis-project-tapipy-prod-tapipy-resources-openapi_v3-streams.pickle
--rw-r--r--   0        0        0    81811 2023-06-09 22:07:10.754747 tapipy-1.4.0a6/tapipy/specs/tapis-project-tapipy-prod-tapipy-resources-openapi_v3-systems.pickle
--rw-r--r--   0        0        0    20306 2023-06-09 22:07:10.786747 tapipy-1.4.0a6/tapipy/specs/tapis-project-tapipy-prod-tapipy-resources-openapi_v3-tenants.pickle
--rw-r--r--   0        0        0     5985 2023-06-09 22:07:10.810747 tapipy-1.4.0a6/tapipy/specs/tapis-project-tapipy-prod-tapipy-resources-openapi_v3-tokens.pickle
--rw-r--r--   0        0        0   155856 2023-06-09 22:07:11.558740 tapipy-1.4.0a6/tapipy/specs/tapis-project-tapipy-prod-tapipy-resources-openapi_v3-workflows.pickle
--rw-r--r--   0        0        0    71651 2023-06-09 22:06:05.507326 tapipy-1.4.0a6/tapipy/tapis.py
--rw-r--r--   0        0        0     3297 2023-06-09 21:45:11.241467 tapipy-1.4.0a6/tapipy/util.py
--rw-r--r--   0        0        0    10016 1970-01-01 00:00:00.000000 tapipy-1.4.0a6/setup.py
--rw-r--r--   0        0        0     9999 1970-01-01 00:00:00.000000 tapipy-1.4.0a6/PKG-INFO
+-rw-r--r--   0        0        0     1539 2023-06-08 15:22:35.013634 tapipy-1.4.0a7/LICENSE.md
+-rw-r--r--   0        0        0     8639 2023-06-08 15:22:20.913795 tapipy-1.4.0a7/README.md
+-rw-r--r--   0        0        0     1000 2023-06-12 16:20:35.567186 tapipy-1.4.0a7/pyproject.toml
+-rw-r--r--   0        0        0       22 2023-06-08 15:21:55.962079 tapipy-1.4.0a7/tapipy/__init__.py
+-rw-r--r--   0        0        0    13502 2023-06-08 15:21:46.714184 tapipy-1.4.0a7/tapipy/actors.py
+-rw-r--r--   0        0        0     2071 2023-06-08 15:21:58.470050 tapipy-1.4.0a7/tapipy/errors.py
+-rw-r--r--   0        0        0    38703 2023-06-08 03:44:21.351648 tapipy-1.4.0a7/tapipy/resources/openapi_v3-actors.yml
+-rw-r--r--   0        0        0    65816 2023-06-12 16:14:56.623316 tapipy-1.4.0a7/tapipy/resources/openapi_v3-apps.yml
+-rw-r--r--   0        0        0    23782 2023-06-08 03:44:21.935642 tapipy-1.4.0a7/tapipy/resources/openapi_v3-authenticator.yml
+-rw-r--r--   0        0        0    74553 2023-06-12 16:14:52.039374 tapipy-1.4.0a7/tapipy/resources/openapi_v3-files.yml
+-rw-r--r--   0        0        0    65915 2023-06-08 03:44:29.879560 tapipy-1.4.0a7/tapipy/resources/openapi_v3-jobs.yml
+-rw-r--r--   0        0        0    28625 2023-06-08 03:44:22.571636 tapipy-1.4.0a7/tapipy/resources/openapi_v3-meta.yml
+-rw-r--r--   0        0        0    52671 2023-06-12 16:14:58.367294 tapipy-1.4.0a7/tapipy/resources/openapi_v3-notifications.yml
+-rw-r--r--   0        0        0    33814 2023-06-08 03:44:28.195577 tapipy-1.4.0a7/tapipy/resources/openapi_v3-pgrest.yml
+-rw-r--r--   0        0        0    62115 2023-06-12 16:14:55.663328 tapipy-1.4.0a7/tapipy/resources/openapi_v3-pods.yml
+-rw-r--r--   0        0        0   145319 2023-06-08 03:44:24.443616 tapipy-1.4.0a7/tapipy/resources/openapi_v3-sk.yml
+-rw-r--r--   0        0        0   108752 2023-06-08 03:44:25.403606 tapipy-1.4.0a7/tapipy/resources/openapi_v3-streams.yml
+-rw-r--r--   0        0        0    97327 2023-06-12 16:14:53.367357 tapipy-1.4.0a7/tapipy/resources/openapi_v3-systems.yml
+-rw-r--r--   0        0        0    25448 2023-06-08 03:44:26.931591 tapipy-1.4.0a7/tapipy/resources/openapi_v3-tenants.yml
+-rw-r--r--   0        0        0     8406 2023-06-08 03:44:27.499585 tapipy-1.4.0a7/tapipy/resources/openapi_v3-tokens.yml
+-rw-r--r--   0        0        0    87200 2023-06-12 16:14:57.731302 tapipy-1.4.0a7/tapipy/resources/openapi_v3-workflows.yml
+-rw-r--r--   0        0        0      907 2023-06-12 16:14:58.367294 tapipy-1.4.0a7/tapipy/resources/resource_etags.json
+-rw-r--r--   0        0        0    60738 2023-06-12 16:14:59.083285 tapipy-1.4.0a7/tapipy/specs/tapis-project-tapipy-main-tapipy-resources-openapi_v3-pods.pickle
+-rw-r--r--   0        0        0    27037 2023-06-12 16:14:58.567291 tapipy-1.4.0a7/tapipy/specs/tapis-project-tapipy-prod-tapipy-resources-openapi_v3-actors.pickle
+-rw-r--r--   0        0        0    72389 2023-06-12 16:14:59.219283 tapipy-1.4.0a7/tapipy/specs/tapis-project-tapipy-prod-tapipy-resources-openapi_v3-apps.pickle
+-rw-r--r--   0        0        0    17736 2023-06-12 16:14:58.611291 tapipy-1.4.0a7/tapipy/specs/tapis-project-tapipy-prod-tapipy-resources-openapi_v3-authenticator.pickle
+-rw-r--r--   0        0        0    56087 2023-06-12 16:14:58.703290 tapipy-1.4.0a7/tapipy/specs/tapis-project-tapipy-prod-tapipy-resources-openapi_v3-files.pickle
+-rw-r--r--   0        0        0    57550 2023-06-12 16:14:59.147284 tapipy-1.4.0a7/tapipy/specs/tapis-project-tapipy-prod-tapipy-resources-openapi_v3-jobs.pickle
+-rw-r--r--   0        0        0    14366 2023-06-12 16:14:58.647290 tapipy-1.4.0a7/tapipy/specs/tapis-project-tapipy-prod-tapipy-resources-openapi_v3-meta.pickle
+-rw-r--r--   0        0        0    39185 2023-06-12 16:14:59.263283 tapipy-1.4.0a7/tapipy/specs/tapis-project-tapipy-prod-tapipy-resources-openapi_v3-notifications.pickle
+-rw-r--r--   0        0        0    23333 2023-06-12 16:14:59.027285 tapipy-1.4.0a7/tapipy/specs/tapis-project-tapipy-prod-tapipy-resources-openapi_v3-pgrest.pickle
+-rw-r--r--   0        0        0    99591 2023-06-12 16:14:58.779289 tapipy-1.4.0a7/tapipy/specs/tapis-project-tapipy-prod-tapipy-resources-openapi_v3-sk.pickle
+-rw-r--r--   0        0        0    75745 2023-06-12 16:14:58.867287 tapipy-1.4.0a7/tapipy/specs/tapis-project-tapipy-prod-tapipy-resources-openapi_v3-streams.pickle
+-rw-r--r--   0        0        0    81811 2023-06-12 16:14:58.947286 tapipy-1.4.0a7/tapipy/specs/tapis-project-tapipy-prod-tapipy-resources-openapi_v3-systems.pickle
+-rw-r--r--   0        0        0    20306 2023-06-12 16:14:58.979286 tapipy-1.4.0a7/tapipy/specs/tapis-project-tapipy-prod-tapipy-resources-openapi_v3-tenants.pickle
+-rw-r--r--   0        0        0     5985 2023-06-12 16:14:58.999286 tapipy-1.4.0a7/tapipy/specs/tapis-project-tapipy-prod-tapipy-resources-openapi_v3-tokens.pickle
+-rw-r--r--   0        0        0   155856 2023-06-12 16:14:59.731277 tapipy-1.4.0a7/tapipy/specs/tapis-project-tapipy-prod-tapipy-resources-openapi_v3-workflows.pickle
+-rw-r--r--   0        0        0    70583 2023-06-12 16:20:08.143509 tapipy-1.4.0a7/tapipy/tapis.py
+-rw-r--r--   0        0        0     3949 2023-06-12 16:20:02.467577 tapipy-1.4.0a7/tapipy/util.py
+-rw-r--r--   0        0        0    10042 1970-01-01 00:00:00.000000 tapipy-1.4.0a7/setup.py
+-rw-r--r--   0        0        0    10039 1970-01-01 00:00:00.000000 tapipy-1.4.0a7/PKG-INFO
```

### Comparing `tapipy-1.4.0a6/LICENSE.md` & `tapipy-1.4.0a7/LICENSE.md`

 * *Files identical despite different names*

### Comparing `tapipy-1.4.0a6/README.md` & `tapipy-1.4.0a7/README.md`

 * *Files identical despite different names*

### Comparing `tapipy-1.4.0a6/pyproject.toml` & `tapipy-1.4.0a7/pyproject.toml`

 * *Files 12% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "tapipy"
-version = "1.4.0a6"
+version = "1.4.0a7"
 description = "Python lib for interacting with an instance of the Tapis API Framework"
 license = "BSD-4-Clause"
 authors = ["Joe Stubbs <jstubbs@tacc.utexas.edu>"]
 maintainers = ["Joe Stubbs <jstubbs@tacc.utexas.edu>",
 			   "Christian Garcia <cgarcia@tacc.utexas.edu>"]
 readme = "README.md"
 repository = "https://github.com/tapis-project/tapipy"
@@ -17,14 +17,15 @@
 six = "^1.10"
 python_dateutil = "^2.5.3"
 setuptools = ">= 21.0.0"
 urllib3 = "^1.26.5"
 PyJWT = ">= 1.7.1"
 openapi_core = "0.16.0"
 openapi_spec_validator = "^0.5.0"
+typing_extensions = "<4.6"
 requests = "^2.20.0"
 atomicwrites = "^1.4.0"
 cryptography = ">= 3.3.2"
 # jsonschema from 4.0.0 -> 4.3.0 slows tapipy import to 8+ seconds.
 jsonschema = ">= 3.2.0"
 pyyaml = ">= 5.4"
 cloudpickle = ">= 1.6.0"
```

### Comparing `tapipy-1.4.0a6/tapipy/actors.py` & `tapipy-1.4.0a7/tapipy/actors.py`

 * *Files identical despite different names*

### Comparing `tapipy-1.4.0a6/tapipy/errors.py` & `tapipy-1.4.0a7/tapipy/errors.py`

 * *Files identical despite different names*

### Comparing `tapipy-1.4.0a6/tapipy/resources/openapi_v3-actors.yml` & `tapipy-1.4.0a7/tapipy/resources/openapi_v3-actors.yml`

 * *Files identical despite different names*

### Comparing `tapipy-1.4.0a6/tapipy/resources/openapi_v3-apps.yml` & `tapipy-1.4.0a7/tapipy/resources/openapi_v3-apps.yml`

 * *Files identical despite different names*

### Comparing `tapipy-1.4.0a6/tapipy/resources/openapi_v3-authenticator.yml` & `tapipy-1.4.0a7/tapipy/resources/openapi_v3-authenticator.yml`

 * *Files identical despite different names*

### Comparing `tapipy-1.4.0a6/tapipy/resources/openapi_v3-files.yml` & `tapipy-1.4.0a7/tapipy/resources/openapi_v3-files.yml`

 * *Files identical despite different names*

### Comparing `tapipy-1.4.0a6/tapipy/resources/openapi_v3-jobs.yml` & `tapipy-1.4.0a7/tapipy/resources/openapi_v3-jobs.yml`

 * *Files identical despite different names*

### Comparing `tapipy-1.4.0a6/tapipy/resources/openapi_v3-meta.yml` & `tapipy-1.4.0a7/tapipy/resources/openapi_v3-meta.yml`

 * *Files identical despite different names*

### Comparing `tapipy-1.4.0a6/tapipy/resources/openapi_v3-notifications.yml` & `tapipy-1.4.0a7/tapipy/resources/openapi_v3-notifications.yml`

 * *Files identical despite different names*

### Comparing `tapipy-1.4.0a6/tapipy/resources/openapi_v3-pgrest.yml` & `tapipy-1.4.0a7/tapipy/resources/openapi_v3-pgrest.yml`

 * *Files identical despite different names*

### Comparing `tapipy-1.4.0a6/tapipy/resources/openapi_v3-pods.yml` & `tapipy-1.4.0a7/tapipy/resources/openapi_v3-pods.yml`

 * *Files identical despite different names*

### Comparing `tapipy-1.4.0a6/tapipy/resources/openapi_v3-sk.yml` & `tapipy-1.4.0a7/tapipy/resources/openapi_v3-sk.yml`

 * *Files identical despite different names*

### Comparing `tapipy-1.4.0a6/tapipy/resources/openapi_v3-streams.yml` & `tapipy-1.4.0a7/tapipy/resources/openapi_v3-streams.yml`

 * *Files identical despite different names*

### Comparing `tapipy-1.4.0a6/tapipy/resources/openapi_v3-systems.yml` & `tapipy-1.4.0a7/tapipy/resources/openapi_v3-systems.yml`

 * *Files identical despite different names*

### Comparing `tapipy-1.4.0a6/tapipy/resources/openapi_v3-tenants.yml` & `tapipy-1.4.0a7/tapipy/resources/openapi_v3-tenants.yml`

 * *Files identical despite different names*

### Comparing `tapipy-1.4.0a6/tapipy/resources/openapi_v3-tokens.yml` & `tapipy-1.4.0a7/tapipy/resources/openapi_v3-tokens.yml`

 * *Files identical despite different names*

### Comparing `tapipy-1.4.0a6/tapipy/resources/openapi_v3-workflows.yml` & `tapipy-1.4.0a7/tapipy/resources/openapi_v3-workflows.yml`

 * *Files identical despite different names*

### Comparing `tapipy-1.4.0a6/tapipy/resources/resource_etags.json` & `tapipy-1.4.0a7/tapipy/resources/resource_etags.json`

 * *Files identical despite different names*

### Comparing `tapipy-1.4.0a6/tapipy/specs/tapis-project-tapipy-main-tapipy-resources-openapi_v3-pods.pickle` & `tapipy-1.4.0a7/tapipy/specs/tapis-project-tapipy-main-tapipy-resources-openapi_v3-pods.pickle`

 * *Files identical despite different names*

### Comparing `tapipy-1.4.0a6/tapipy/specs/tapis-project-tapipy-prod-tapipy-resources-openapi_v3-actors.pickle` & `tapipy-1.4.0a7/tapipy/specs/tapis-project-tapipy-prod-tapipy-resources-openapi_v3-actors.pickle`

 * *Files identical despite different names*

### Comparing `tapipy-1.4.0a6/tapipy/specs/tapis-project-tapipy-prod-tapipy-resources-openapi_v3-apps.pickle` & `tapipy-1.4.0a7/tapipy/specs/tapis-project-tapipy-prod-tapipy-resources-openapi_v3-apps.pickle`

 * *Files identical despite different names*

### Comparing `tapipy-1.4.0a6/tapipy/specs/tapis-project-tapipy-prod-tapipy-resources-openapi_v3-authenticator.pickle` & `tapipy-1.4.0a7/tapipy/specs/tapis-project-tapipy-prod-tapipy-resources-openapi_v3-authenticator.pickle`

 * *Files identical despite different names*

### Comparing `tapipy-1.4.0a6/tapipy/specs/tapis-project-tapipy-prod-tapipy-resources-openapi_v3-files.pickle` & `tapipy-1.4.0a7/tapipy/specs/tapis-project-tapipy-prod-tapipy-resources-openapi_v3-files.pickle`

 * *Files identical despite different names*

### Comparing `tapipy-1.4.0a6/tapipy/specs/tapis-project-tapipy-prod-tapipy-resources-openapi_v3-jobs.pickle` & `tapipy-1.4.0a7/tapipy/specs/tapis-project-tapipy-prod-tapipy-resources-openapi_v3-jobs.pickle`

 * *Files identical despite different names*

### Comparing `tapipy-1.4.0a6/tapipy/specs/tapis-project-tapipy-prod-tapipy-resources-openapi_v3-meta.pickle` & `tapipy-1.4.0a7/tapipy/specs/tapis-project-tapipy-prod-tapipy-resources-openapi_v3-meta.pickle`

 * *Files identical despite different names*

### Comparing `tapipy-1.4.0a6/tapipy/specs/tapis-project-tapipy-prod-tapipy-resources-openapi_v3-notifications.pickle` & `tapipy-1.4.0a7/tapipy/specs/tapis-project-tapipy-prod-tapipy-resources-openapi_v3-notifications.pickle`

 * *Files identical despite different names*

### Comparing `tapipy-1.4.0a6/tapipy/specs/tapis-project-tapipy-prod-tapipy-resources-openapi_v3-pgrest.pickle` & `tapipy-1.4.0a7/tapipy/specs/tapis-project-tapipy-prod-tapipy-resources-openapi_v3-pgrest.pickle`

 * *Files identical despite different names*

### Comparing `tapipy-1.4.0a6/tapipy/specs/tapis-project-tapipy-prod-tapipy-resources-openapi_v3-sk.pickle` & `tapipy-1.4.0a7/tapipy/specs/tapis-project-tapipy-prod-tapipy-resources-openapi_v3-sk.pickle`

 * *Files identical despite different names*

### Comparing `tapipy-1.4.0a6/tapipy/specs/tapis-project-tapipy-prod-tapipy-resources-openapi_v3-streams.pickle` & `tapipy-1.4.0a7/tapipy/specs/tapis-project-tapipy-prod-tapipy-resources-openapi_v3-streams.pickle`

 * *Files identical despite different names*

### Comparing `tapipy-1.4.0a6/tapipy/specs/tapis-project-tapipy-prod-tapipy-resources-openapi_v3-systems.pickle` & `tapipy-1.4.0a7/tapipy/specs/tapis-project-tapipy-prod-tapipy-resources-openapi_v3-systems.pickle`

 * *Files identical despite different names*

### Comparing `tapipy-1.4.0a6/tapipy/specs/tapis-project-tapipy-prod-tapipy-resources-openapi_v3-tenants.pickle` & `tapipy-1.4.0a7/tapipy/specs/tapis-project-tapipy-prod-tapipy-resources-openapi_v3-tenants.pickle`

 * *Files identical despite different names*

### Comparing `tapipy-1.4.0a6/tapipy/specs/tapis-project-tapipy-prod-tapipy-resources-openapi_v3-tokens.pickle` & `tapipy-1.4.0a7/tapipy/specs/tapis-project-tapipy-prod-tapipy-resources-openapi_v3-tokens.pickle`

 * *Files identical despite different names*

### Comparing `tapipy-1.4.0a6/tapipy/specs/tapis-project-tapipy-prod-tapipy-resources-openapi_v3-workflows.pickle` & `tapipy-1.4.0a7/tapipy/specs/tapis-project-tapipy-prod-tapipy-resources-openapi_v3-workflows.pickle`

 * *Files identical despite different names*

### Comparing `tapipy-1.4.0a6/tapipy/tapis.py` & `tapipy-1.4.0a7/tapipy/tapis.py`

 * *Files 1% similar despite different names*

```diff
@@ -168,41 +168,16 @@
         # This has a serious 1+ import, so we only import when needed.
         from openapi_core import Spec
         POOL_SIZE = os.environ.get('POOL_SIZE', 16)
         with concurrent.futures.ThreadPoolExecutor(max_workers=POOL_SIZE) as executor:
             executor.map(_thread_download_spec_dict, urls_to_download)
 
 
-### This rewrites BaseFilePathHandler.__call__ as Python3.8+ treats Protocol
-### differently than Python3.7 which causes 3.7 to break.
-from jsonschema_spec.handlers.file import BaseFilePathHandler
-from urllib.parse import urlparse
-def new_call(self, uri):
-    if hasattr(uri, 'read'):
-        return super(BaseFilePathHandler, self).__call__(uri)
-    parsed_url = urlparse(uri)
-    if parsed_url.scheme not in self.allowed_schemes:
-        raise ValueError("Not allowed scheme")
-    return self._open(uri)
-BaseFilePathHandler.__call__ = new_call
 
 
-### This rewrites DataClassFactory so that when it makes the validated Dataclass it's not frozen.
-from openapi_core.extensions.models.factories import DataClassFactory
-from openapi_core.extensions.models.types import Field
-from typing import Iterable, Type, Any
-from dataclasses import make_dataclass
-def new_create(
-    self,
-    fields: Iterable[Field],
-    name: str = "Model",
-) -> Type[Any]:
-    return make_dataclass(name, fields, frozen=False) #<-- only change is frozen=False
-DataClassFactory.create = new_create
-
 
 def _thread_download_spec_dict(resource_info: ResourceInfo) -> None:
     """
     Function that multiprocessing pool calls to download and store pickled
     spec dicts. Gets spec dict, if it's valid, stores it at 'spec_path',
     else it does nothing.
     """
```

### Comparing `tapipy-1.4.0a6/tapipy/util.py` & `tapipy-1.4.0a7/tapipy/util.py`

 * *Files 13% similar despite different names*

```diff
@@ -74,8 +74,22 @@
                     new_spec[key].append(item)
         # If the value at the current key is neither a dictionary nor a list,
         # copy it directly to new_spec
         else:
             new_spec[key] = spec_obj[key]
 
     # Return the new dictionary containing the dereferenced schema
-    return new_spec
+    return new_spec
+
+# ### https://github.com/p1c2u/jsonschema-spec/issues/14
+# ### This rewrites BaseFilePathHandler.__call__ as Python3.8+ treats Protocol
+# ### differently than Python3.7 which causes 3.7 to break when dereferencing spec.
+# from jsonschema_spec.handlers.file import BaseFilePathHandler
+# from urllib.parse import urlparse
+# def new_call(self, uri):
+#     if hasattr(uri, 'read'):
+#         return super(BaseFilePathHandler, self).__call__(uri)
+#     parsed_url = urlparse(uri)
+#     if parsed_url.scheme not in self.allowed_schemes:
+#         raise ValueError("Not allowed scheme")
+#     return self._open(uri)
+# BaseFilePathHandler.__call__ = new_call
```

### Comparing `tapipy-1.4.0a6/setup.py` & `tapipy-1.4.0a7/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -17,19 +17,20 @@
  'openapi_core==0.16.0',
  'openapi_spec_validator>=0.5.0,<0.6.0',
  'python_dateutil>=2.5.3,<3.0.0',
  'pyyaml>=5.4',
  'requests>=2.20.0,<3.0.0',
  'setuptools>=21.0.0',
  'six>=1.10,<2.0',
+ 'typing_extensions<4.6',
  'urllib3>=1.26.5,<2.0.0']
 
 setup_kwargs = {
     'name': 'tapipy',
-    'version': '1.4.0a6',
+    'version': '1.4.0a7',
     'description': 'Python lib for interacting with an instance of the Tapis API Framework',
     'long_description': '# tapipy - Tapis V3 Python SDK\n\nPython library for interacting with an instance of the Tapis API Framework.\n\nThe library is automatically generated by referencing the OpenAPI spec files which  a `Tapis` object built from the OpenAPI spec files from TACC\'s Tapis services. With this functionality a user is able to authorize itself with the `Tapis` object and have a \'live\' library in order to interact with Tapis services.\n\n## Development\n\nThis project is under active development, exploring different approaches to SDK generation.\n\n## Installation\nTapipy is packaged on [pypi](https://pypi.org/project/tapipy/) and can be installed with pip.\n\n```\npip install tapipy\n```\n\n\n## Usage\nTapipy\'s Tapis object first must be initialized in order to be used.\nA basic example of logging in with a user account is below.\n\n```\n# Import the Tapis object\nfrom tapipy.tapis import Tapis\n\n# Log into you the Tapis service by providing user/pass and the base url of your tenant. For example, to interact with the tacc tenant --\nt = Tapis(base_url=\'https://tacc.tapis.io\',\n          username=\'myuser\',\n          password=\'mypass\')\n\t  \n# Get tokens that will be used for authentication function calls\nt.get_tokens()\n```\n\nNow you have a Tapis object that is authenticated and able to call Tapis service endpoints. It\'s useful to know that the Tapis object will automatically refresh it\'s token if it is deemed appropriate, so the object should stay in the good graces of Tapis indefinitely.\n\nNow in order to use the Tapis object you can reference the [Tapis Framework](https://tapis-project.github.io/live-docs/) to browse all functions. For example, if I wanted to use the SK service in order to check if a user has a specific role I would find the function on the site (which is just a better way to look at the json specs).\n\nWith the site I can see that I need to use my Tapis object, initialized as `t`, access `sk`, and then use the `hasRole` function with the required inputs as follows.\n```\nt.sk.hasRole(tenant=\'dev\', user=\'_testuser\', roleName=\'Do you have this role?\')\n```\n\n### Special Query Parameters and Headers\nFor the most part, arguments that can or should be passed to a Tapis endpoint are described in the OpenAPI \ndefinition files and recognized automatically by `tapipy`. However, due to limitations in what can be expressed\nin OpenAPI, there are some paramaters that are not defined in the definition files; for example, the search\nparameters for various endpoints.\n\nTo accommodate these cases, `tapipy` recognizes two special keyword arguments to all of its methods that\ncorrespond to Tapis API calls (i.e., all of its "operations"). They are:\n\n  * `_tapis_headers` -- dictionary-like object of header names (keys) and vales.\n  * `_tapis_query_parameters` -- dictionary-like object of query parameter names (keys) and values.\n\nUse the above two special arguments for passing headers (respectively, query parameters) that are not specified\nin the OpenAPI definition of an endpoint.\n\nFor example, I can issue a search using the following syntax:\n\n```\nt.jobs.getJobSearchList(limit=5, orderBy=\'lastUpdated(desc),name(asc)\', _tapis_query_parameters={\'key\': \'value\'})\n```\n\n# Development Docs\n## Running the tests\n\nTests resources are contained within the `test` directory. `Dockerfile-tests` is at root.\n1. Build the test docker image: `docker build -t tapis/tapipy-tests -f Dockerfile-tests .`\n2. Run these tests using the built docker image: `docker run -it --rm -e username=<dev_user> -e password=<dev_pass> tapis/tapipy-tests`\n\n\n## Important Parameters to Know\n\nThe `tapipy` package allows for spec file customization in Tapis object initialization:\n* resource_set: str \n\t* Determines which set of resource to use, master or dev, defaults to master.\n\t* Important to note that if a custom_spec_dictionary is used, it is appended to this resource_set.\n\t\t* For example, you would set master and then specify a custom specs that will be added on.\n* custom_spec_dict: {resource_name: str, resource_url: str}\n\t* Allows users to modify the base resource set urls.\n\t\t* e.g. I can specify actor as a resource name and change the url.\n\t* Also allows users to add new resources to the set.\n\t\t* e.g. I can add a new resource named "test" with a  custom url.\n\t\t* Important that know that any new specs will be downloaded and added to the cache\n\t\t\t* No need to specify download_latest_specs or update spec files.\n\t* ALLOWS LOCAL RESOURCES!\n\t\t* Specify an absolute path in the dict with `local:` prefixing it and tapipy will load in a local OpenAPI v3 yml spec file.\n\t\t* `custom_spec_dict={\'cactus\': \'local: /home/tapis/myfolder/cactusSpec.yml\'}`\n* download_latest_specs: bool\n\t* Allows users to re-download all specs regardless on if they already exist in the cache. Defaulted to False\n\t* This will happen every time the Tapis object is initialized, it\'s a tad slower, and can cause live updates to specs.\n\t\t* As such, be warned. There are functions to update spec files below.\n* spec_dir: str\n\t* Allows users to specify folder to save specs to. Defaults to none which uses Tapipy\'s package folder.\n\t* If you are updating specs it\'s wise to use a different folder in order to not modify the base specs.\n\nThe following is an example of some custom parameter setting. As you can see, the abaco resource will now use the spec at `URL#1`, overwriting the resource definition in the master resource set, it\'ll download it if it doesn\'t exist. The same for the longhorn resource. This means that the Tapis object will now have access to all specs in master like normal, but with a modified abaco and with a new longhorn resource. All of these are stored at the new spec_dir because I don\'t want to accidentally overwrite any base specs if I call `update_spec_cache()` later (talked about in the next section).\n```\nfrom tapipy.tapis import Tapis\n\nt = Tapis(base_url=\'https://admin.develop.tapis.io\',\n          tenant_id=\'admin\',\n          username=\'username\',\n          account_type=\'user\',\n          password=\'password\',\n          resource_set=\'admin\',\n          custom_spec_dict={\'abaco\': \'URL#1\',\n                            \'longhorn\': \'URL#2\'},\n                            \'cactus\': \'local: /home/tapis/myfolder/cactusSpec.yml\'},\n          spec_dir=\'/home/username/tapipy_specs\')\nt.get_tokens()\n```\n\n## Update Specs Files\n\nThe Tapipy package now uses a cache to organize spec dictionaries as pickled files and has the ability to accept custom spec files. By default Tapipy keeps a set of base spec files in the `%tapipy%/specs` folder. These specs are pre-pickled at package creation time.\n\nIn order to update all default spec files a user can use the `update_spec_cache()` function. Said function\'s definition is below. If no resources are provided the function will download all default spec urls in the RESOURCES object in `%tapipy%/tapipy/tapis.py` file.\n```\nResources = Dict[ResourceName, ResourceUrl]\nupdate_spec_cache(resources: Resources = None, spec_dir: str = None)\n```\nUsers are able to specify custom resources to download by providing their own resource dictionary. For example, providing `{\'actors\': \'URLToMyActorDictionary\'}` would update that spec.\n\nUsers can also specify here where to update the spec with the `spec_dir` variable.\n\nThe Tapis object itself also has a `update_spec_cache()` function that takes the Tapis parameters given at startup and updates the spec cache. Meaning that if the Tapis object was given a custom dictionary, the `update_spec_cache()` function would update it without the need for setting parameters.\n```\nt.update_spec_cache()\n```\n\n## Build instructions\n\nBuilding is done with poetry as follows:\n```\npip install poetry\npoetry install\n```\nThis installs `tapipy` to a virtual environment. Run a shell in this environment with:\n```\npoetry shell\n```\n\nTo install locally (not in a virtual environment):\n```\npip install poetry\npoetry build\ncd dists\npip install *.whl\n```\n\n## PyPi Push Instructions\n\n```\npoetry build\npoetry publish\n```\n\n## Archive Usage\nTODO - provide working examples, e.g., \n```\nimport tapipy\nt = tapipy.Tapis(base_url=\'http://localhost:5001\')\nreq = t.tokens.NewTokenRequest(token_type=\'service\', token_tenant_id=\'dev\', token_username=\'admin\')\nt.tokens.create_token(req)\n\nimport openapi_client\nconfiguration = openapi_client.Configuration()\nconfiguration.host = \'http://localhost:5001\'\napi_instance = openapi_client.TokensApi(openapi_client.ApiClient(configuration))\n\nnew_token = openapi_client.NewTokenRequest(token_type=\'service\', token_tenant_id=\'dev\', token_username=\'admin\')\n\nresp = api_instance.create_token(new_token)\njwt = resp.get(\'result\').get(\'access_token\').get(\'access_token\')\n```\n',
     'author': 'Joe Stubbs',
     'author_email': 'jstubbs@tacc.utexas.edu',
     'maintainer': 'Joe Stubbs',
     'maintainer_email': 'jstubbs@tacc.utexas.edu',
     'url': 'https://github.com/tapis-project/tapipy',
```

### Comparing `tapipy-1.4.0a6/PKG-INFO` & `tapipy-1.4.0a7/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: tapipy
-Version: 1.4.0a6
+Version: 1.4.0a7
 Summary: Python lib for interacting with an instance of the Tapis API Framework
 Home-page: https://github.com/tapis-project/tapipy
 License: BSD-4-Clause
 Author: Joe Stubbs
 Author-email: jstubbs@tacc.utexas.edu
 Maintainer: Joe Stubbs
 Maintainer-email: jstubbs@tacc.utexas.edu
@@ -25,14 +25,15 @@
 Requires-Dist: openapi_core (==0.16.0)
 Requires-Dist: openapi_spec_validator (>=0.5.0,<0.6.0)
 Requires-Dist: python_dateutil (>=2.5.3,<3.0.0)
 Requires-Dist: pyyaml (>=5.4)
 Requires-Dist: requests (>=2.20.0,<3.0.0)
 Requires-Dist: setuptools (>=21.0.0)
 Requires-Dist: six (>=1.10,<2.0)
+Requires-Dist: typing_extensions (<4.6)
 Requires-Dist: urllib3 (>=1.26.5,<2.0.0)
 Project-URL: Repository, https://github.com/tapis-project/tapipy
 Description-Content-Type: text/markdown
 
 # tapipy - Tapis V3 Python SDK
 
 Python library for interacting with an instance of the Tapis API Framework.
```

