# Comparing `tmp/django-clone-5.3.2.tar.gz` & `tmp/django-clone-5.3.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "/home/runner/work/django-clone/django-clone/dist/.tmp-5v93ez8j/django-clone-5.3.2.tar", last modified: Mon May 29 04:14:09 2023, max compression
+gzip compressed data, was "/home/runner/work/django-clone/django-clone/dist/.tmp-ambl9w5f/django-clone-5.3.3.tar", last modified: Mon Jun 12 13:09:13 2023, max compression
```

## Comparing `django-clone-5.3.2.tar` & `django-clone-5.3.3.tar`

### file list

```diff
@@ -1,30 +1,30 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-29 04:14:09.000000 django-clone-5.3.2/
--rw-r--r--   0 runner    (1001) docker     (123)   108930 2023-05-29 04:13:41.000000 django-clone-5.3.2/CHANGELOG.md
--rw-r--r--   0 runner    (1001) docker     (123)     5218 2023-05-29 04:13:41.000000 django-clone-5.3.2/CODE_OF_CONDUCT.md
--rw-r--r--   0 runner    (1001) docker     (123)     1067 2023-05-29 04:13:41.000000 django-clone-5.3.2/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)      731 2023-05-29 04:13:41.000000 django-clone-5.3.2/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)    17086 2023-05-29 04:14:09.000000 django-clone-5.3.2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    15396 2023-05-29 04:13:41.000000 django-clone-5.3.2/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-29 04:14:09.000000 django-clone-5.3.2/django_clone.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    17086 2023-05-29 04:14:09.000000 django-clone-5.3.2/django_clone.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      566 2023-05-29 04:14:09.000000 django-clone-5.3.2/django_clone.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-29 04:14:09.000000 django-clone-5.3.2/django_clone.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-29 04:14:09.000000 django-clone-5.3.2/django_clone.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)      404 2023-05-29 04:14:09.000000 django-clone-5.3.2/django_clone.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       12 2023-05-29 04:14:09.000000 django-clone-5.3.2/django_clone.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-29 04:14:09.000000 django-clone-5.3.2/model_clone/
--rw-r--r--   0 runner    (1001) docker     (123)      405 2023-05-29 04:13:57.000000 django-clone-5.3.2/model_clone/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2884 2023-05-29 04:13:41.000000 django-clone-5.3.2/model_clone/admin.py
--rw-r--r--   0 runner    (1001) docker     (123)       96 2023-05-29 04:13:41.000000 django-clone-5.3.2/model_clone/apps.py
--rw-r--r--   0 runner    (1001) docker     (123)    28928 2023-05-29 04:13:41.000000 django-clone-5.3.2/model_clone/mixin.py
--rw-r--r--   0 runner    (1001) docker     (123)      157 2023-05-29 04:13:41.000000 django-clone-5.3.2/model_clone/models.py
--rw-r--r--   0 runner    (1001) docker     (123)      145 2023-05-29 04:13:41.000000 django-clone-5.3.2/model_clone/signals.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-29 04:14:09.000000 django-clone-5.3.2/model_clone/templates/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-29 04:14:09.000000 django-clone-5.3.2/model_clone/templates/admin/
--rw-r--r--   0 runner    (1001) docker     (123)      282 2023-05-29 04:13:41.000000 django-clone-5.3.2/model_clone/templates/admin/change_form_object_tools.html
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-29 04:14:09.000000 django-clone-5.3.2/model_clone/templates/clone/
--rw-r--r--   0 runner    (1001) docker     (123)      250 2023-05-29 04:13:41.000000 django-clone-5.3.2/model_clone/templates/clone/change_form.html
--rw-r--r--   0 runner    (1001) docker     (123)    10732 2023-05-29 04:13:41.000000 django-clone-5.3.2/model_clone/utils.py
--rw-r--r--   0 runner    (1001) docker     (123)      322 2023-05-29 04:13:41.000000 django-clone-5.3.2/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (123)      189 2023-05-29 04:14:09.000000 django-clone-5.3.2/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     3109 2023-05-29 04:13:57.000000 django-clone-5.3.2/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-12 13:09:13.000000 django-clone-5.3.3/
+-rw-r--r--   0 runner    (1001) docker     (123)   113126 2023-06-12 13:08:47.000000 django-clone-5.3.3/CHANGELOG.md
+-rw-r--r--   0 runner    (1001) docker     (123)     5218 2023-06-12 13:08:47.000000 django-clone-5.3.3/CODE_OF_CONDUCT.md
+-rw-r--r--   0 runner    (1001) docker     (123)     1067 2023-06-12 13:08:47.000000 django-clone-5.3.3/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)      731 2023-06-12 13:08:47.000000 django-clone-5.3.3/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)    17125 2023-06-12 13:09:13.000000 django-clone-5.3.3/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    15396 2023-06-12 13:08:47.000000 django-clone-5.3.3/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-12 13:09:13.000000 django-clone-5.3.3/django_clone.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    17125 2023-06-12 13:09:13.000000 django-clone-5.3.3/django_clone.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      566 2023-06-12 13:09:13.000000 django-clone-5.3.3/django_clone.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-12 13:09:13.000000 django-clone-5.3.3/django_clone.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-12 13:09:13.000000 django-clone-5.3.3/django_clone.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)      404 2023-06-12 13:09:13.000000 django-clone-5.3.3/django_clone.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       12 2023-06-12 13:09:13.000000 django-clone-5.3.3/django_clone.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-12 13:09:13.000000 django-clone-5.3.3/model_clone/
+-rw-r--r--   0 runner    (1001) docker     (123)      405 2023-06-12 13:09:01.000000 django-clone-5.3.3/model_clone/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2884 2023-06-12 13:08:47.000000 django-clone-5.3.3/model_clone/admin.py
+-rw-r--r--   0 runner    (1001) docker     (123)       96 2023-06-12 13:08:47.000000 django-clone-5.3.3/model_clone/apps.py
+-rw-r--r--   0 runner    (1001) docker     (123)    28928 2023-06-12 13:08:47.000000 django-clone-5.3.3/model_clone/mixin.py
+-rw-r--r--   0 runner    (1001) docker     (123)      157 2023-06-12 13:08:47.000000 django-clone-5.3.3/model_clone/models.py
+-rw-r--r--   0 runner    (1001) docker     (123)      145 2023-06-12 13:08:47.000000 django-clone-5.3.3/model_clone/signals.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-12 13:09:13.000000 django-clone-5.3.3/model_clone/templates/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-12 13:09:13.000000 django-clone-5.3.3/model_clone/templates/admin/
+-rw-r--r--   0 runner    (1001) docker     (123)      282 2023-06-12 13:08:47.000000 django-clone-5.3.3/model_clone/templates/admin/change_form_object_tools.html
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-12 13:09:13.000000 django-clone-5.3.3/model_clone/templates/clone/
+-rw-r--r--   0 runner    (1001) docker     (123)      250 2023-06-12 13:08:47.000000 django-clone-5.3.3/model_clone/templates/clone/change_form.html
+-rw-r--r--   0 runner    (1001) docker     (123)    10732 2023-06-12 13:08:47.000000 django-clone-5.3.3/model_clone/utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)      322 2023-06-12 13:08:47.000000 django-clone-5.3.3/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      189 2023-06-12 13:09:13.000000 django-clone-5.3.3/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     3147 2023-06-12 13:09:01.000000 django-clone-5.3.3/setup.py
```

### Comparing `django-clone-5.3.2/CHANGELOG.md` & `django-clone-5.3.3/CHANGELOG.md`

 * *Files 0% similar despite different names*

```diff
@@ -1,19 +1,50 @@
 # Changelog
 
-## [v5.3.1](https://github.com/tj-django/django-clone/tree/v5.3.1) (2023-03-18)
+## [v5.3.2](https://github.com/tj-django/django-clone/tree/v5.3.2) (2023-05-27)
 
-[Full Changelog](https://github.com/tj-django/django-clone/compare/v5.3.0...v5.3.1)
+[Full Changelog](https://github.com/tj-django/django-clone/compare/v5.3.1...v5.3.2)
 
 **Closed issues:**
 
 - Dependency Dashboard [\#198](https://github.com/tj-django/django-clone/issues/198)
 
 **Merged pull requests:**
 
+- chore\(deps\): update dependency asgiref to v3.7.2 [\#796](https://github.com/tj-django/django-clone/pull/796) ([renovate[bot]](https://github.com/apps/renovate))
+- chore\(deps\): update dependency asgiref to v3.7.1 [\#795](https://github.com/tj-django/django-clone/pull/795) ([renovate[bot]](https://github.com/apps/renovate))
+- chore\(deps\): update dependency asgiref to v3.7.0 [\#794](https://github.com/tj-django/django-clone/pull/794) ([renovate[bot]](https://github.com/apps/renovate))
+- \[pre-commit.ci\] pre-commit autoupdate [\#793](https://github.com/tj-django/django-clone/pull/793) ([pre-commit-ci[bot]](https://github.com/apps/pre-commit-ci))
+- chore\(deps\): update codecov/codecov-action action to v3.1.4 [\#792](https://github.com/tj-django/django-clone/pull/792) ([renovate[bot]](https://github.com/apps/renovate))
+- chore\(deps\): update dependency django to v4.2.1 [\#791](https://github.com/tj-django/django-clone/pull/791) ([renovate[bot]](https://github.com/apps/renovate))
+- chore\(deps\): update peter-evans/create-pull-request action to v5.0.1 [\#790](https://github.com/tj-django/django-clone/pull/790) ([renovate[bot]](https://github.com/apps/renovate))
+- chore\(deps\): update codecov/codecov-action action to v3.1.3 [\#789](https://github.com/tj-django/django-clone/pull/789) ([renovate[bot]](https://github.com/apps/renovate))
+- chore\(deps\): update dependency sqlparse to v0.4.4 [\#788](https://github.com/tj-django/django-clone/pull/788) ([renovate[bot]](https://github.com/apps/renovate))
+- \[pre-commit.ci\] pre-commit autoupdate [\#787](https://github.com/tj-django/django-clone/pull/787) ([pre-commit-ci[bot]](https://github.com/apps/pre-commit-ci))
+- Updated docs [\#786](https://github.com/tj-django/django-clone/pull/786) ([github-actions[bot]](https://github.com/apps/github-actions))
+- Updated README.md [\#785](https://github.com/tj-django/django-clone/pull/785) ([jackton1](https://github.com/jackton1))
+- chore\(deps\): update actions/checkout action to v3.5.2 [\#784](https://github.com/tj-django/django-clone/pull/784) ([renovate[bot]](https://github.com/apps/renovate))
+- chore\(deps\): update actions/checkout action to v3.5.1 [\#783](https://github.com/tj-django/django-clone/pull/783) ([renovate[bot]](https://github.com/apps/renovate))
+- chore\(deps\): update codecov/codecov-action action to v3.1.2 [\#782](https://github.com/tj-django/django-clone/pull/782) ([renovate[bot]](https://github.com/apps/renovate))
+- Updated docs [\#781](https://github.com/tj-django/django-clone/pull/781) ([github-actions[bot]](https://github.com/apps/github-actions))
+- chore\(deps\): update peter-evans/create-pull-request action to v5 [\#780](https://github.com/tj-django/django-clone/pull/780) ([renovate[bot]](https://github.com/apps/renovate))
+- \[pre-commit.ci\] pre-commit autoupdate [\#779](https://github.com/tj-django/django-clone/pull/779) ([pre-commit-ci[bot]](https://github.com/apps/pre-commit-ci))
+- chore\(deps\): update dependency django to v4.2 [\#778](https://github.com/tj-django/django-clone/pull/778) ([renovate[bot]](https://github.com/apps/renovate))
+- chore\(deps\): update peaceiris/actions-gh-pages action to v3.9.3 [\#777](https://github.com/tj-django/django-clone/pull/777) ([renovate[bot]](https://github.com/apps/renovate))
+- \[pre-commit.ci\] pre-commit autoupdate \(\#776\)Co-authored-by: pre-commit-ci\[bot\] \<66853113+pre-commit-ci\[bot\]@users.noreply.github.com\> [\#776](https://github.com/tj-django/django-clone/pull/776) ([pre-commit-ci[bot]](https://github.com/apps/pre-commit-ci))
+- chore\(deps\): update actions/checkout action to v3.5.0 [\#775](https://github.com/tj-django/django-clone/pull/775) ([renovate[bot]](https://github.com/apps/renovate))
+- Updated docs [\#774](https://github.com/tj-django/django-clone/pull/774) ([github-actions[bot]](https://github.com/apps/github-actions))
+- Upgraded v5.3.0 → v5.3.1 [\#773](https://github.com/tj-django/django-clone/pull/773) ([jackton1](https://github.com/jackton1))
+
+## [v5.3.1](https://github.com/tj-django/django-clone/tree/v5.3.1) (2023-03-18)
+
+[Full Changelog](https://github.com/tj-django/django-clone/compare/v5.3.0...v5.3.1)
+
+**Merged pull requests:**
+
 - chore\(deps\): update tj-actions/verify-changed-files action to v14 [\#772](https://github.com/tj-django/django-clone/pull/772) ([renovate[bot]](https://github.com/apps/renovate))
 - chore\(deps\): update actions/checkout action to v3.4.0 [\#771](https://github.com/tj-django/django-clone/pull/771) ([renovate[bot]](https://github.com/apps/renovate))
 - chore\(deps\): update peter-evans/create-pull-request action to v4.2.4 [\#770](https://github.com/tj-django/django-clone/pull/770) ([renovate[bot]](https://github.com/apps/renovate))
 - \[pre-commit.ci\] pre-commit autoupdate [\#769](https://github.com/tj-django/django-clone/pull/769) ([pre-commit-ci[bot]](https://github.com/apps/pre-commit-ci))
 - chore\(deps\): update tj-actions/github-changelog-generator action to v1.18 [\#768](https://github.com/tj-django/django-clone/pull/768) ([renovate[bot]](https://github.com/apps/renovate))
 - chore\(deps\): update codacy/codacy-analysis-cli-action action to v4.3.0 [\#767](https://github.com/tj-django/django-clone/pull/767) ([renovate[bot]](https://github.com/apps/renovate))
 - Updated docs [\#766](https://github.com/tj-django/django-clone/pull/766) ([github-actions[bot]](https://github.com/apps/github-actions))
```

### Comparing `django-clone-5.3.2/CODE_OF_CONDUCT.md` & `django-clone-5.3.3/CODE_OF_CONDUCT.md`

 * *Files identical despite different names*

### Comparing `django-clone-5.3.2/LICENSE` & `django-clone-5.3.3/LICENSE`

 * *Files identical despite different names*

### Comparing `django-clone-5.3.2/MANIFEST.in` & `django-clone-5.3.3/MANIFEST.in`

 * *Files identical despite different names*

### Comparing `django-clone-5.3.2/PKG-INFO` & `django-clone-5.3.3/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: django-clone
-Version: 5.3.2
+Version: 5.3.3
 Summary: Create a clone of a django model instance.
 Home-page: https://github.com/tj-django/django-clone.git
 Author: Tonye Jack
 Author-email: jtonye@ymail.com
 Maintainer: Tonye Jack
 Maintainer-email: jtonye@ymail.com
 License: MIT/Apache-2.0
@@ -28,14 +28,15 @@
 Classifier: Framework :: Django :: 2.1
 Classifier: Framework :: Django :: 2.2
 Classifier: Framework :: Django :: 3.0
 Classifier: Framework :: Django :: 3.1
 Classifier: Framework :: Django :: 3.2
 Classifier: Framework :: Django :: 4.0
 Classifier: Framework :: Django :: 4.1
+Classifier: Framework :: Django :: 4.2
 Requires-Python: >=3.6
 Description-Content-Type: text/markdown
 Provides-Extra: development
 Provides-Extra: test
 Provides-Extra: deploy
 License-File: LICENSE
```

### Comparing `django-clone-5.3.2/README.md` & `django-clone-5.3.3/README.md`

 * *Files identical despite different names*

### Comparing `django-clone-5.3.2/django_clone.egg-info/PKG-INFO` & `django-clone-5.3.3/django_clone.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: django-clone
-Version: 5.3.2
+Version: 5.3.3
 Summary: Create a clone of a django model instance.
 Home-page: https://github.com/tj-django/django-clone.git
 Author: Tonye Jack
 Author-email: jtonye@ymail.com
 Maintainer: Tonye Jack
 Maintainer-email: jtonye@ymail.com
 License: MIT/Apache-2.0
@@ -28,14 +28,15 @@
 Classifier: Framework :: Django :: 2.1
 Classifier: Framework :: Django :: 2.2
 Classifier: Framework :: Django :: 3.0
 Classifier: Framework :: Django :: 3.1
 Classifier: Framework :: Django :: 3.2
 Classifier: Framework :: Django :: 4.0
 Classifier: Framework :: Django :: 4.1
+Classifier: Framework :: Django :: 4.2
 Requires-Python: >=3.6
 Description-Content-Type: text/markdown
 Provides-Extra: development
 Provides-Extra: test
 Provides-Extra: deploy
 License-File: LICENSE
```

### Comparing `django-clone-5.3.2/django_clone.egg-info/SOURCES.txt` & `django-clone-5.3.3/django_clone.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `django-clone-5.3.2/model_clone/admin.py` & `django-clone-5.3.3/model_clone/admin.py`

 * *Files identical despite different names*

### Comparing `django-clone-5.3.2/model_clone/mixin.py` & `django-clone-5.3.3/model_clone/mixin.py`

 * *Files identical despite different names*

### Comparing `django-clone-5.3.2/model_clone/utils.py` & `django-clone-5.3.3/model_clone/utils.py`

 * *Files identical despite different names*

### Comparing `django-clone-5.3.2/setup.py` & `django-clone-5.3.3/setup.py`

 * *Files 8% similar despite different names*

```diff
@@ -50,15 +50,15 @@
     with io.open(README_PATH, encoding="utf-8") as f:
         LONG_DESCRIPTION = f.read()
 else:
     LONG_DESCRIPTION = ""
 
 setup(
     name="django-clone",
-    version="5.3.2",
+    version="5.3.3",
     description="Create a clone of a django model instance.",
     python_requires=">=3.6",
     long_description=LONG_DESCRIPTION,
     long_description_content_type=LONG_DESCRIPTION_TYPE,
     author="Tonye Jack",
     author_email="jtonye@ymail.com",
     maintainer="Tonye Jack",
@@ -97,14 +97,15 @@
         "Framework :: Django :: 2.1",
         "Framework :: Django :: 2.2",
         "Framework :: Django :: 3.0",
         "Framework :: Django :: 3.1",
         "Framework :: Django :: 3.2",
         "Framework :: Django :: 4.0",
         "Framework :: Django :: 4.1",
+        "Framework :: Django :: 4.2",
     ],
     install_requires=install_requires,
     tests_require=["coverage"],
     extras_require=extras_require,
     packages=find_namespace_packages(
         include=[
             "model_clone.templates.admin",
```

