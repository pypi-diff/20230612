# Comparing `tmp/django-expanded-test-cases-0.3.0.tar.gz` & `tmp/django-expanded-test-cases-0.4.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "django-expanded-test-cases-0.3.0.tar", last modified: Thu Jun  8 07:14:47 2023, max compression
+gzip compressed data, was "django-expanded-test-cases-0.4.0.tar", last modified: Mon Jun 12 20:22:26 2023, max compression
```

## Comparing `django-expanded-test-cases-0.3.0.tar` & `django-expanded-test-cases-0.4.0.tar`

### file list

```diff
@@ -1,41 +1,41 @@
-drwxrwxr-x   0 brodriguez  (1000) brodriguez  (1000)        0 2023-06-08 07:14:47.733480 django-expanded-test-cases-0.3.0/
--rw-rw-r--   0 brodriguez  (1000) brodriguez  (1000)     1074 2023-05-23 04:12:24.000000 django-expanded-test-cases-0.3.0/LICENSE
--rw-rw-r--   0 brodriguez  (1000) brodriguez  (1000)       91 2023-05-23 04:25:19.000000 django-expanded-test-cases-0.3.0/MANIFEST.in
--rw-rw-r--   0 brodriguez  (1000) brodriguez  (1000)     5168 2023-06-08 07:14:47.733480 django-expanded-test-cases-0.3.0/PKG-INFO
-drwxrwxr-x   0 brodriguez  (1000) brodriguez  (1000)        0 2023-06-08 07:14:47.729480 django-expanded-test-cases-0.3.0/django_expanded_test_cases/
--rw-rw-r--   0 brodriguez  (1000) brodriguez  (1000)      181 2023-05-23 04:12:47.000000 django-expanded-test-cases-0.3.0/django_expanded_test_cases/__init__.py
--rw-rw-r--   0 brodriguez  (1000) brodriguez  (1000)     8697 2023-06-08 01:04:49.000000 django-expanded-test-cases-0.3.0/django_expanded_test_cases/constants.py
-drwxrwxr-x   0 brodriguez  (1000) brodriguez  (1000)        0 2023-06-08 07:14:47.729480 django-expanded-test-cases-0.3.0/django_expanded_test_cases/mixins/
--rw-rw-r--   0 brodriguez  (1000) brodriguez  (1000)      325 2023-05-23 04:25:19.000000 django-expanded-test-cases-0.3.0/django_expanded_test_cases/mixins/__init__.py
--rw-rw-r--   0 brodriguez  (1000) brodriguez  (1000)    37346 2023-06-08 04:10:33.000000 django-expanded-test-cases-0.3.0/django_expanded_test_cases/mixins/core_mixin.py
--rw-rw-r--   0 brodriguez  (1000) brodriguez  (1000)    29317 2023-06-08 03:30:55.000000 django-expanded-test-cases-0.3.0/django_expanded_test_cases/mixins/response_mixin.py
-drwxrwxr-x   0 brodriguez  (1000) brodriguez  (1000)        0 2023-06-08 07:14:47.729480 django-expanded-test-cases-0.3.0/django_expanded_test_cases/templates/
-drwxrwxr-x   0 brodriguez  (1000) brodriguez  (1000)        0 2023-06-08 07:14:47.729480 django-expanded-test-cases-0.3.0/django_expanded_test_cases/templates/django_expanded_test_cases/
--rw-rw-r--   0 brodriguez  (1000) brodriguez  (1000)      528 2023-05-23 04:25:19.000000 django-expanded-test-cases-0.3.0/django_expanded_test_cases/templates/django_expanded_test_cases/index.html
-drwxrwxr-x   0 brodriguez  (1000) brodriguez  (1000)        0 2023-06-08 07:14:47.733480 django-expanded-test-cases-0.3.0/django_expanded_test_cases/test_cases/
--rw-rw-r--   0 brodriguez  (1000) brodriguez  (1000)     1376 2023-05-23 04:25:19.000000 django-expanded-test-cases-0.3.0/django_expanded_test_cases/test_cases/__init__.py
--rw-rw-r--   0 brodriguez  (1000) brodriguez  (1000)    16682 2023-05-23 04:25:19.000000 django-expanded-test-cases-0.3.0/django_expanded_test_cases/test_cases/base_test_case.py
--rw-rw-r--   0 brodriguez  (1000) brodriguez  (1000)    56799 2023-06-08 05:09:20.000000 django-expanded-test-cases-0.3.0/django_expanded_test_cases/test_cases/integration_test_case.py
--rw-rw-r--   0 brodriguez  (1000) brodriguez  (1000)     7790 2023-05-23 04:25:19.000000 django-expanded-test-cases-0.3.0/django_expanded_test_cases/test_cases/live_server_test_case.py
--rw-rw-r--   0 brodriguez  (1000) brodriguez  (1000)     1093 2023-05-23 04:25:19.000000 django-expanded-test-cases-0.3.0/django_expanded_test_cases/test_urls.py
-drwxrwxr-x   0 brodriguez  (1000) brodriguez  (1000)        0 2023-06-08 07:14:47.729480 django-expanded-test-cases-0.3.0/django_expanded_test_cases.egg-info/
--rw-rw-r--   0 brodriguez  (1000) brodriguez  (1000)     5168 2023-06-08 07:14:47.000000 django-expanded-test-cases-0.3.0/django_expanded_test_cases.egg-info/PKG-INFO
--rw-rw-r--   0 brodriguez  (1000) brodriguez  (1000)     1116 2023-06-08 07:14:47.000000 django-expanded-test-cases-0.3.0/django_expanded_test_cases.egg-info/SOURCES.txt
--rw-rw-r--   0 brodriguez  (1000) brodriguez  (1000)        1 2023-06-08 07:14:47.000000 django-expanded-test-cases-0.3.0/django_expanded_test_cases.egg-info/dependency_links.txt
--rw-rw-r--   0 brodriguez  (1000) brodriguez  (1000)      112 2023-06-08 07:14:47.000000 django-expanded-test-cases-0.3.0/django_expanded_test_cases.egg-info/requires.txt
--rw-rw-r--   0 brodriguez  (1000) brodriguez  (1000)       33 2023-06-08 07:14:47.000000 django-expanded-test-cases-0.3.0/django_expanded_test_cases.egg-info/top_level.txt
--rw-rw-r--   0 brodriguez  (1000) brodriguez  (1000)     1781 2023-06-08 07:13:39.000000 django-expanded-test-cases-0.3.0/pyproject.toml
--rw-rw-r--   0 brodriguez  (1000) brodriguez  (1000)     2335 2023-05-23 04:25:19.000000 django-expanded-test-cases-0.3.0/readme.md
--rw-rw-r--   0 brodriguez  (1000) brodriguez  (1000)     1192 2023-06-08 07:14:47.733480 django-expanded-test-cases-0.3.0/setup.cfg
-drwxrwxr-x   0 brodriguez  (1000) brodriguez  (1000)        0 2023-06-08 07:14:47.733480 django-expanded-test-cases-0.3.0/tests/
--rw-rw-r--   0 brodriguez  (1000) brodriguez  (1000)        0 2022-05-23 23:45:09.000000 django-expanded-test-cases-0.3.0/tests/__init__.py
--rw-rw-r--   0 brodriguez  (1000) brodriguez  (1000)      198 2023-05-23 04:25:19.000000 django-expanded-test-cases-0.3.0/tests/apps.py
--rw-rw-r--   0 brodriguez  (1000) brodriguez  (1000)      360 2023-05-23 04:25:19.000000 django-expanded-test-cases-0.3.0/tests/asgi.py
--rw-rw-r--   0 brodriguez  (1000) brodriguez  (1000)     3527 2023-05-23 04:25:20.000000 django-expanded-test-cases-0.3.0/tests/settings.py
-drwxrwxr-x   0 brodriguez  (1000) brodriguez  (1000)        0 2023-06-08 07:14:47.733480 django-expanded-test-cases-0.3.0/tests/test_cases/
--rw-rw-r--   0 brodriguez  (1000) brodriguez  (1000)        0 2023-05-23 04:12:47.000000 django-expanded-test-cases-0.3.0/tests/test_cases/__init__.py
--rw-rw-r--   0 brodriguez  (1000) brodriguez  (1000)    96771 2023-05-23 04:25:20.000000 django-expanded-test-cases-0.3.0/tests/test_cases/test_base_case.py
--rw-rw-r--   0 brodriguez  (1000) brodriguez  (1000)   300247 2023-06-08 06:24:32.000000 django-expanded-test-cases-0.3.0/tests/test_cases/test_integration_case.py
--rw-rw-r--   0 brodriguez  (1000) brodriguez  (1000)     2230 2023-05-23 04:25:20.000000 django-expanded-test-cases-0.3.0/tests/test_cases/test_live_server_case.py
--rw-rw-r--   0 brodriguez  (1000) brodriguez  (1000)      316 2023-05-23 04:25:20.000000 django-expanded-test-cases-0.3.0/tests/urls.py
--rw-rw-r--   0 brodriguez  (1000) brodriguez  (1000)     3964 2023-05-23 04:25:20.000000 django-expanded-test-cases-0.3.0/tests/views.py
+drwxrwxr-x   0 brodriguez  (1000) brodriguez  (1000)        0 2023-06-12 20:22:26.726703 django-expanded-test-cases-0.4.0/
+-rw-rw-r--   0 brodriguez  (1000) brodriguez  (1000)     1074 2022-06-03 17:01:28.000000 django-expanded-test-cases-0.4.0/LICENSE
+-rw-rw-r--   0 brodriguez  (1000) brodriguez  (1000)       91 2023-06-12 17:34:53.000000 django-expanded-test-cases-0.4.0/MANIFEST.in
+-rw-rw-r--   0 brodriguez  (1000) brodriguez  (1000)     5168 2023-06-12 20:22:26.726703 django-expanded-test-cases-0.4.0/PKG-INFO
+drwxrwxr-x   0 brodriguez  (1000) brodriguez  (1000)        0 2023-06-12 20:22:26.726703 django-expanded-test-cases-0.4.0/django_expanded_test_cases/
+-rw-rw-r--   0 brodriguez  (1000) brodriguez  (1000)      181 2022-06-13 15:23:33.000000 django-expanded-test-cases-0.4.0/django_expanded_test_cases/__init__.py
+-rw-rw-r--   0 brodriguez  (1000) brodriguez  (1000)    10124 2023-06-12 20:21:48.000000 django-expanded-test-cases-0.4.0/django_expanded_test_cases/constants.py
+drwxrwxr-x   0 brodriguez  (1000) brodriguez  (1000)        0 2023-06-12 20:22:26.726703 django-expanded-test-cases-0.4.0/django_expanded_test_cases/mixins/
+-rw-rw-r--   0 brodriguez  (1000) brodriguez  (1000)      325 2022-06-24 03:18:02.000000 django-expanded-test-cases-0.4.0/django_expanded_test_cases/mixins/__init__.py
+-rw-rw-r--   0 brodriguez  (1000) brodriguez  (1000)    37636 2023-06-12 20:21:48.000000 django-expanded-test-cases-0.4.0/django_expanded_test_cases/mixins/core_mixin.py
+-rw-rw-r--   0 brodriguez  (1000) brodriguez  (1000)    29825 2023-06-12 20:21:48.000000 django-expanded-test-cases-0.4.0/django_expanded_test_cases/mixins/response_mixin.py
+drwxrwxr-x   0 brodriguez  (1000) brodriguez  (1000)        0 2023-06-12 20:22:26.726703 django-expanded-test-cases-0.4.0/django_expanded_test_cases/templates/
+drwxrwxr-x   0 brodriguez  (1000) brodriguez  (1000)        0 2023-06-12 20:22:26.726703 django-expanded-test-cases-0.4.0/django_expanded_test_cases/templates/django_expanded_test_cases/
+-rw-rw-r--   0 brodriguez  (1000) brodriguez  (1000)      528 2023-06-12 17:34:53.000000 django-expanded-test-cases-0.4.0/django_expanded_test_cases/templates/django_expanded_test_cases/index.html
+drwxrwxr-x   0 brodriguez  (1000) brodriguez  (1000)        0 2023-06-12 20:22:26.726703 django-expanded-test-cases-0.4.0/django_expanded_test_cases/test_cases/
+-rw-rw-r--   0 brodriguez  (1000) brodriguez  (1000)     1376 2023-06-12 17:34:53.000000 django-expanded-test-cases-0.4.0/django_expanded_test_cases/test_cases/__init__.py
+-rw-rw-r--   0 brodriguez  (1000) brodriguez  (1000)    16722 2023-06-12 20:21:48.000000 django-expanded-test-cases-0.4.0/django_expanded_test_cases/test_cases/base_test_case.py
+-rw-rw-r--   0 brodriguez  (1000) brodriguez  (1000)    57283 2023-06-12 20:21:48.000000 django-expanded-test-cases-0.4.0/django_expanded_test_cases/test_cases/integration_test_case.py
+-rw-rw-r--   0 brodriguez  (1000) brodriguez  (1000)     7790 2023-06-12 17:34:53.000000 django-expanded-test-cases-0.4.0/django_expanded_test_cases/test_cases/live_server_test_case.py
+-rw-rw-r--   0 brodriguez  (1000) brodriguez  (1000)     1093 2023-06-12 17:34:53.000000 django-expanded-test-cases-0.4.0/django_expanded_test_cases/test_urls.py
+drwxrwxr-x   0 brodriguez  (1000) brodriguez  (1000)        0 2023-06-12 20:22:26.726703 django-expanded-test-cases-0.4.0/django_expanded_test_cases.egg-info/
+-rw-rw-r--   0 brodriguez  (1000) brodriguez  (1000)     5168 2023-06-12 20:22:26.000000 django-expanded-test-cases-0.4.0/django_expanded_test_cases.egg-info/PKG-INFO
+-rw-rw-r--   0 brodriguez  (1000) brodriguez  (1000)     1116 2023-06-12 20:22:26.000000 django-expanded-test-cases-0.4.0/django_expanded_test_cases.egg-info/SOURCES.txt
+-rw-rw-r--   0 brodriguez  (1000) brodriguez  (1000)        1 2023-06-12 20:22:26.000000 django-expanded-test-cases-0.4.0/django_expanded_test_cases.egg-info/dependency_links.txt
+-rw-rw-r--   0 brodriguez  (1000) brodriguez  (1000)      112 2023-06-12 20:22:26.000000 django-expanded-test-cases-0.4.0/django_expanded_test_cases.egg-info/requires.txt
+-rw-rw-r--   0 brodriguez  (1000) brodriguez  (1000)       33 2023-06-12 20:22:26.000000 django-expanded-test-cases-0.4.0/django_expanded_test_cases.egg-info/top_level.txt
+-rw-rw-r--   0 brodriguez  (1000) brodriguez  (1000)     1781 2023-06-12 20:21:48.000000 django-expanded-test-cases-0.4.0/pyproject.toml
+-rw-rw-r--   0 brodriguez  (1000) brodriguez  (1000)     2335 2023-06-12 17:34:53.000000 django-expanded-test-cases-0.4.0/readme.md
+-rw-rw-r--   0 brodriguez  (1000) brodriguez  (1000)     1192 2023-06-12 20:22:26.726703 django-expanded-test-cases-0.4.0/setup.cfg
+drwxrwxr-x   0 brodriguez  (1000) brodriguez  (1000)        0 2023-06-12 20:22:26.726703 django-expanded-test-cases-0.4.0/tests/
+-rw-rw-r--   0 brodriguez  (1000) brodriguez  (1000)        0 2023-03-01 21:20:22.000000 django-expanded-test-cases-0.4.0/tests/__init__.py
+-rw-rw-r--   0 brodriguez  (1000) brodriguez  (1000)      198 2023-06-12 17:34:53.000000 django-expanded-test-cases-0.4.0/tests/apps.py
+-rw-rw-r--   0 brodriguez  (1000) brodriguez  (1000)      360 2023-06-12 17:34:53.000000 django-expanded-test-cases-0.4.0/tests/asgi.py
+-rw-rw-r--   0 brodriguez  (1000) brodriguez  (1000)     3527 2023-06-12 17:34:53.000000 django-expanded-test-cases-0.4.0/tests/settings.py
+drwxrwxr-x   0 brodriguez  (1000) brodriguez  (1000)        0 2023-06-12 20:22:26.726703 django-expanded-test-cases-0.4.0/tests/test_cases/
+-rw-rw-r--   0 brodriguez  (1000) brodriguez  (1000)        0 2023-03-01 21:20:22.000000 django-expanded-test-cases-0.4.0/tests/test_cases/__init__.py
+-rw-rw-r--   0 brodriguez  (1000) brodriguez  (1000)   100821 2023-06-12 20:21:48.000000 django-expanded-test-cases-0.4.0/tests/test_cases/test_base_case.py
+-rw-rw-r--   0 brodriguez  (1000) brodriguez  (1000)   300318 2023-06-12 20:21:48.000000 django-expanded-test-cases-0.4.0/tests/test_cases/test_integration_case.py
+-rw-rw-r--   0 brodriguez  (1000) brodriguez  (1000)     2230 2023-06-12 17:34:53.000000 django-expanded-test-cases-0.4.0/tests/test_cases/test_live_server_case.py
+-rw-rw-r--   0 brodriguez  (1000) brodriguez  (1000)      316 2023-06-12 17:34:53.000000 django-expanded-test-cases-0.4.0/tests/urls.py
+-rw-rw-r--   0 brodriguez  (1000) brodriguez  (1000)     3964 2023-06-12 17:34:53.000000 django-expanded-test-cases-0.4.0/tests/views.py
```

### Comparing `django-expanded-test-cases-0.3.0/LICENSE` & `django-expanded-test-cases-0.4.0/LICENSE`

 * *Files identical despite different names*

### Comparing `django-expanded-test-cases-0.3.0/PKG-INFO` & `django-expanded-test-cases-0.4.0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: django-expanded-test-cases
-Version: 0.3.0
+Version: 0.4.0
 Summary: Expands the existing Django TestCase class with extra functionality.
 Home-page: https://github.com/brodriguez8774/django-expanded-test-cases
 Author: Brandon Rodriguez
 Author-email: Brandon Rodriguez <brodriguez8774@gmail.com>
 Maintainer-email: Brandon Rodriguez <brodriguez8774@gmail.com>
 License: MIT License
```

### Comparing `django-expanded-test-cases-0.3.0/django_expanded_test_cases/constants.py` & `django-expanded-test-cases-0.4.0/django_expanded_test_cases/constants.py`

 * *Files 26% similar despite different names*

```diff
@@ -13,93 +13,135 @@
 
 
 # Underline style definition for debug printing.
 UNDERLINE = '\u001b[4m'
 UNDERLINE_RESET = '\u001b[0m'
 
 
-# General output format settings.
-OUTPUT_ERROR = str(getattr(
+# General output/color format settings.
+ETC_OUTPUT_ERROR_COLOR = str(getattr(
     settings,
-    'DJANGO_EXPANDED_TESTCASES_OUTPUT_ERROR_HEADER',
+    'DJANGO_EXPANDED_TESTCASES_OUTPUT_ERROR_HEADER_COLOR',
     '{0}{1}{2}'.format(Fore.RED, Back.RESET, Style.NORMAL) if COLORAMA_PRESENT else '',
 ))
-OUTPUT_EXPECTED_MATCH = str(getattr(
+ETC_OUTPUT_EXPECTED_MATCH_COLOR = str(getattr(
     settings,
-    'DJANGO_EXPANDED_TESTCASES_OUTPUT_EXPECTED_MATCH',
+    'DJANGO_EXPANDED_TESTCASES_OUTPUT_EXPECTED_MATCH_COLOR',
     '{0}{1}{2}'.format(Fore.CYAN, Back.RESET, Style.NORMAL) if COLORAMA_PRESENT else '',
 ))
-OUTPUT_EXPECTED_ERROR = str(getattr(
+ETC_OUTPUT_EXPECTED_ERROR_COLOR = str(getattr(
     settings,
-    'DJANGO_EXPANDED_TESTCASES_OUTPUT_EXPECTED_ERROR',
+    'DJANGO_EXPANDED_TESTCASES_OUTPUT_EXPECTED_ERROR_COLOR',
     '{0}{1}{2}'.format(Fore.BLACK, Back.CYAN, Style.NORMAL) if COLORAMA_PRESENT else '',
 ))
-OUTPUT_ACTUALS_MATCH = str(getattr(
+ETC_OUTPUT_ACTUALS_MATCH_COLOR = str(getattr(
     settings,
-    'DJANGO_EXPANDED_TESTCASES_OUTPUT_ACTUALS_MATCH',
+    'DJANGO_EXPANDED_TESTCASES_OUTPUT_ACTUALS_MATCH_COLOR',
     '{0}{1}{2}'.format(Fore.MAGENTA, Back.RESET, Style.NORMAL) if COLORAMA_PRESENT else '',
 ))
-OUTPUT_ACTUALS_ERROR = str(getattr(
+ETC_OUTPUT_ACTUALS_ERROR_COLOR = str(getattr(
     settings,
-    'DJANGO_EXPANDED_TESTCASES_OUTPUT_ACTUALS_ERROR',
+    'DJANGO_EXPANDED_TESTCASES_OUTPUT_ACTUALS_ERROR_COLOR',
     '{0}{1}{2}'.format(Fore.BLACK, Back.MAGENTA, Style.NORMAL) if COLORAMA_PRESENT else '',
 ))
-OUTPUT_EMPHASIS = str(getattr(
+ETC_OUTPUT_EMPHASIS_COLOR = str(getattr(
     settings,
-    'DJANGO_EXPANDED_TESTCASES_OUTPUT_EMPHASIS',
+    'DJANGO_EXPANDED_TESTCASES_OUTPUT_EMPHASIS_COLOR',
     (Style.BRIGHT if COLORAMA_PRESENT else '') + UNDERLINE,
 ))
-OUTPUT_RESET = str(getattr(
+ETC_OUTPUT_RESET_COLOR = str(getattr(
     settings,
-    'DJANGO_EXPANDED_TESTCASES_OUTPUT_RESET',
+    'DJANGO_EXPANDED_TESTCASES_OUTPUT_RESET_COLOR',
     Style.RESET_ALL if COLORAMA_PRESENT else UNDERLINE_RESET,
 ))
 
-# Output formatting for response sections.
-RESPONSE_DEBUG_URL = str(getattr(
+# Output/color formatting for response sections.
+ETC_RESPONSE_DEBUG_URL_COLOR = str(getattr(
     settings,
-    'DJANGO_EXPANDED_TESTCASES_RESPONSE_OUTPUT_URL',
+    'DJANGO_EXPANDED_TESTCASES_RESPONSE_OUTPUT_URL_COLOR',
     Fore.YELLOW if COLORAMA_PRESENT else '',
 ))
-RESPONSE_DEBUG_CONTENT = str(getattr(
+ETC_RESPONSE_DEBUG_CONTENT_COLOR = str(getattr(
     settings,
-    'DJANGO_EXPANDED_TESTCASES_RESPONSE_OUTPUT_CONTENT',
+    'DJANGO_EXPANDED_TESTCASES_RESPONSE_OUTPUT_CONTENT_COLOR',
     Fore.WHITE if COLORAMA_PRESENT else '',
 ))
-RESPONSE_DEBUG_HEADERS = str(getattr(
+ETC_RESPONSE_DEBUG_HEADER_COLOR = str(getattr(
     settings,
-    'DJANGO_EXPANDED_TESTCASES_RESPONSE_OUTPUT_HEADERS',
+    'DJANGO_EXPANDED_TESTCASES_RESPONSE_OUTPUT_HEADER_COLOR',
     Fore.CYAN if COLORAMA_PRESENT else '',
 ))
-RESPONSE_DEBUG_CONTEXT = str(getattr(
+ETC_RESPONSE_DEBUG_CONTEXT_COLOR = str(getattr(
     settings,
-    'DJANGO_EXPANDED_TESTCASES_RESPONSE_OUTPUT_CONTEXT',
+    'DJANGO_EXPANDED_TESTCASES_RESPONSE_OUTPUT_CONTEXT_COLOR',
     Fore.BLUE if COLORAMA_PRESENT else '',
 ))
-RESPONSE_DEBUG_SESSION = str(getattr(
+ETC_RESPONSE_DEBUG_SESSION_COLOR = str(getattr(
     settings,
-    'DJANGO_EXPANDED_TESTCASES_RESPONSE_OUTPUT_SESSION',
+    'DJANGO_EXPANDED_TESTCASES_RESPONSE_OUTPUT_SESSION_COLOR',
     Fore.MAGENTA if COLORAMA_PRESENT else '',
 ))
-RESPONSE_DEBUG_MESSAGES = str(getattr(
+ETC_RESPONSE_DEBUG_MESSAGE_COLOR = str(getattr(
     settings,
-    'DJANGO_EXPANDED_TESTCASES_RESPONSE_OUTPUT_MESSAGES',
+    'DJANGO_EXPANDED_TESTCASES_RESPONSE_OUTPUT_MESSAGES_COLOR',
     Fore.CYAN if COLORAMA_PRESENT else '',
 ))
-RESPONSE_DEBUG_FORMS = str(getattr(
+ETC_RESPONSE_DEBUG_FORM_COLOR = str(getattr(
     settings,
-    'DJANGO_EXPANDED_TESTCASES_RESPONSE_OUTPUT_FORMS',
+    'DJANGO_EXPANDED_TESTCASES_RESPONSE_OUTPUT_FORMS_COLOR',
     Fore.BLUE if COLORAMA_PRESENT else '',
 ))
-RESPONSE_DEBUG_USER_INFO = str(getattr(
+ETC_RESPONSE_DEBUG_USER_INFO_COLOR = str(getattr(
     settings,
-    'DJANGO_EXPANDED_TESTCASES_RESPONSE_OUTPUT_USER_INFO',
+    'DJANGO_EXPANDED_TESTCASES_RESPONSE_OUTPUT_USER_INFO_COLOR',
     Fore.MAGENTA if COLORAMA_PRESENT else '',
 ))
 
+# Enabling/disabling output of specific sections.
+ETC_INCLUDE_RESPONSE_DEBUG_URL = bool(getattr(
+    settings,
+    'DJANGO_EXPANDED_TESTCASES_INCLUDE_RESPONSE_DEBUG_URL',
+    True,
+))
+ETC_INCLUDE_RESPONSE_DEBUG_CONTENT = bool(getattr(
+    settings,
+    'DJANGO_EXPANDED_TESTCASES_INCLUDE_RESPONSE_DEBUG_CONTENT',
+    True,
+))
+ETC_INCLUDE_RESPONSE_DEBUG_HEADER = bool(getattr(
+    settings,
+    'DJANGO_EXPANDED_TESTCASES_INCLUDE_RESPONSE_DEBUG_HEADER',
+    True,
+))
+ETC_INCLUDE_RESPONSE_DEBUG_CONTEXT = bool(getattr(
+    settings,
+    'DJANGO_EXPANDED_TESTCASES_INCLUDE_RESPONSE_DEBUG_CONTEXT',
+    True,
+))
+ETC_INCLUDE_RESPONSE_DEBUG_SESSION = bool(getattr(
+    settings,
+    'DJANGO_EXPANDED_TESTCASES_INCLUDE_RESPONSE_DEBUG_SESSION',
+    True,
+))
+ETC_INCLUDE_RESPONSE_DEBUG_MESSAGES = bool(getattr(
+    settings,
+    'DJANGO_EXPANDED_TESTCASES_INCLUDE_RESPONSE_DEBUG_MESSAGES',
+    True,
+))
+ETC_INCLUDE_RESPONSE_DEBUG_FORMS = bool(getattr(
+    settings,
+    'DJANGO_EXPANDED_TESTCASES_INCLUDE_RESPONSE_DEBUG_FORMS',
+    True,
+))
+ETC_INCLUDE_RESPONSE_DEBUG_USER_INFO = bool(getattr(
+    settings,
+    'DJANGO_EXPANDED_TESTCASES_INCLUDE_RESPONSE_DEBUG_USER_INFO',
+    True,
+))
+
 
 # Void element list as defined at:
 # https://www.w3.org/TR/2011/WD-html-markup-20110113/syntax.html#void-element
 # TLDR: A "void element" is an HTML element that does not require a closing tag.
 # Used in the "repeating element" logic.
 VOID_ELEMENT_LIST = [
     'area',
```

### Comparing `django-expanded-test-cases-0.3.0/django_expanded_test_cases/mixins/core_mixin.py` & `django-expanded-test-cases-0.4.0/django_expanded_test_cases/mixins/core_mixin.py`

 * *Files 3% similar despite different names*

```diff
@@ -19,35 +19,35 @@
     ETC_USER_MODEL_IDENTIFIER,
     ETC_DEFAULT_SUPER_USER_IDENTIFIER,
     ETC_DEFAULT_ADMIN_USER_IDENTIFIER,
     ETC_DEFAULT_STANDARD_USER_IDENTIFIER,
     ETC_DEFAULT_INACTIVE_USER_IDENTIFIER,
     ETC_DEFAULT_USER_PASSWORD,
     ETC_GENERATE_USERS_WITH_REAL_NAMES,
-    OUTPUT_ACTUALS_ERROR,
-    OUTPUT_ACTUALS_MATCH,
-    OUTPUT_ERROR,
-    OUTPUT_EXPECTED_ERROR,
-    OUTPUT_EXPECTED_MATCH,
-    OUTPUT_RESET,
+    ETC_OUTPUT_ACTUALS_ERROR_COLOR,
+    ETC_OUTPUT_ACTUALS_MATCH_COLOR,
+    ETC_OUTPUT_ERROR_COLOR,
+    ETC_OUTPUT_EXPECTED_ERROR_COLOR,
+    ETC_OUTPUT_EXPECTED_MATCH_COLOR,
+    ETC_OUTPUT_RESET_COLOR,
 )
 
 
 # region Debug Print Wrapper Logic
 
 def wrapper(method):
     """Wrapper logic to intercept all functions on AssertionError and print error at bottom of output."""
     @wraps(method)
     def wrapped(*args, **kwargs):
         try:
             return method(*args, **kwargs)
         except AssertionError as err:
             if ETC_DEBUG_PRINT:
                 print('\n')
-                print('{0}{1}{2}'.format(OUTPUT_ERROR, err, OUTPUT_RESET))
+                print('{0}{1}{2}'.format(ETC_OUTPUT_ERROR_COLOR, err, ETC_OUTPUT_RESET_COLOR))
                 print('')
             raise err
     return wrapped
 
 
 class DebugPrintMetaClass(type):
     """Courtesy of https://stackoverflow.com/a/11350487"""
@@ -255,15 +255,15 @@
         Mostly used for internal testcase logic.
         """
         if self._debug_print_bool:
             print(fore, end='')
             print(back, end='')
             print(style, end='')
             print(*args, **kwargs, end='')
-            print(OUTPUT_RESET)
+            print(ETC_OUTPUT_RESET_COLOR)
 
     # region Custom Assertions
 
     def assertText(self, expected_text, actual_text, strip=True):
         """Wrapper for assertEqual(), that prints full values to console on mismatch.
 
         :param expected_text: Expected text value to check against.
@@ -318,43 +318,43 @@
                         curr_actual_line = '\n{0}'.format(curr_actual_line)
                 except IndexError:
                     curr_actual_line = None
                 append_newline = False
 
                 if curr_expected_line == curr_actual_line:
                     # Line is full match and correct.
-                    curr_expected_line = '{0}{1}{2}\n'.format(OUTPUT_EXPECTED_MATCH, curr_expected_line, OUTPUT_RESET)
-                    curr_actual_line = '{0}{1}{2}\n'.format(OUTPUT_ACTUALS_MATCH, curr_actual_line, OUTPUT_RESET)
+                    curr_expected_line = '{0}{1}{2}\n'.format(ETC_OUTPUT_EXPECTED_MATCH_COLOR, curr_expected_line, ETC_OUTPUT_RESET_COLOR)
+                    curr_actual_line = '{0}{1}{2}\n'.format(ETC_OUTPUT_ACTUALS_MATCH_COLOR, curr_actual_line, ETC_OUTPUT_RESET_COLOR)
                 elif curr_expected_line is None:
                     # "Actual" output is longer than "expected" output. Impossible to match current line.
                     curr_expected_line = ''
                     curr_actual_line = '{0}{1}{2}\n'.format(
-                        OUTPUT_ACTUALS_ERROR,
+                        ETC_OUTPUT_ACTUALS_ERROR_COLOR,
                         curr_actual_line,
-                        OUTPUT_RESET,
+                        ETC_OUTPUT_RESET_COLOR,
                     )
                 elif curr_actual_line is None:
                     # "Expected" output is longer than "actual" output. Impossible to match current line.
                     curr_expected_line = '{0}{1}{2}\n'.format(
-                        OUTPUT_EXPECTED_ERROR,
+                        ETC_OUTPUT_EXPECTED_ERROR_COLOR,
                         curr_expected_line,
-                        OUTPUT_RESET,
+                        ETC_OUTPUT_RESET_COLOR,
                     )
                     curr_actual_line = ''
                 else:
                     # Both lines are populated but do not match.
                     # Determine which one is longer.
                     if len(curr_actual_line) > len(curr_expected_line):
                         max_chars = len(curr_actual_line)
                     else:
                         max_chars = len(curr_expected_line)
 
                     # Check each character and determine where non-match happens.
-                    curr_expected_color = OUTPUT_RESET
-                    curr_actual_color = OUTPUT_RESET
+                    curr_expected_color = ETC_OUTPUT_RESET_COLOR
+                    curr_actual_color = ETC_OUTPUT_RESET_COLOR
                     curr_expected_char_line = ''
                     curr_actual_char_line = ''
                     for char_index in range(max_chars):
                         # Grab current character.
                         try:
                             expected_char = curr_expected_line[char_index]
                         except IndexError:
@@ -363,27 +363,27 @@
                             actual_char = curr_actual_line[char_index]
                         except IndexError:
                             actual_char = ''
 
                         # Format based on match.
                         if expected_char == actual_char:
                             # Match.
-                            if curr_expected_color != OUTPUT_EXPECTED_MATCH:
-                                curr_expected_color = OUTPUT_EXPECTED_MATCH
+                            if curr_expected_color != ETC_OUTPUT_EXPECTED_MATCH_COLOR:
+                                curr_expected_color = ETC_OUTPUT_EXPECTED_MATCH_COLOR
                                 curr_expected_char_line += curr_expected_color
-                            if curr_actual_color != OUTPUT_ACTUALS_MATCH:
-                                curr_actual_color = OUTPUT_ACTUALS_MATCH
+                            if curr_actual_color != ETC_OUTPUT_ACTUALS_MATCH_COLOR:
+                                curr_actual_color = ETC_OUTPUT_ACTUALS_MATCH_COLOR
                                 curr_actual_char_line += curr_actual_color
                         else:
                             # Non-match.
-                            if curr_expected_color != OUTPUT_EXPECTED_ERROR:
-                                curr_expected_color = OUTPUT_EXPECTED_ERROR
+                            if curr_expected_color != ETC_OUTPUT_EXPECTED_ERROR_COLOR:
+                                curr_expected_color = ETC_OUTPUT_EXPECTED_ERROR_COLOR
                                 curr_expected_char_line += curr_expected_color
-                            if curr_actual_color != OUTPUT_ACTUALS_ERROR:
-                                curr_actual_color = OUTPUT_ACTUALS_ERROR
+                            if curr_actual_color != ETC_OUTPUT_ACTUALS_ERROR_COLOR:
+                                curr_actual_color = ETC_OUTPUT_ACTUALS_ERROR_COLOR
                                 curr_actual_char_line += curr_actual_color
 
                         curr_expected_char_line += '{0}'.format(expected_char)
                         curr_actual_char_line += '{0}'.format(actual_char)
 
                     # Update output strings.
                     append_newline = True
@@ -394,19 +394,19 @@
                 # Update output strings.
                 formatted_expected_output += curr_expected_line
                 formatted_actual_output += curr_actual_line
 
             # Finally print actual debug output.
             self._debug_print('')
             self._debug_print('')
-            self._debug_print('EXPECTED:', fore=OUTPUT_EXPECTED_MATCH)
+            self._debug_print('EXPECTED:', fore=ETC_OUTPUT_EXPECTED_MATCH_COLOR)
             self._debug_print(formatted_expected_output)
             self._debug_print('')
             self._debug_print('')
-            self._debug_print('ACTUAL:', fore=OUTPUT_ACTUALS_MATCH)
+            self._debug_print('ACTUAL:', fore=ETC_OUTPUT_ACTUALS_MATCH_COLOR)
             self._debug_print(formatted_actual_output)
             self._debug_print('')
             self._debug_print('')
 
             # Raise original error.
             raise AssertionError(err) from err
```

### Comparing `django-expanded-test-cases-0.3.0/django_expanded_test_cases/mixins/response_mixin.py` & `django-expanded-test-cases-0.4.0/django_expanded_test_cases/mixins/response_mixin.py`

 * *Files 6% similar despite different names*

```diff
@@ -9,23 +9,23 @@
 from bs4 import BeautifulSoup
 from django.contrib.auth import get_user_model
 from django.http.response import HttpResponseBase
 
 # Internal Imports.
 from . import CoreTestCaseMixin
 from django_expanded_test_cases.constants import (
-    OUTPUT_ERROR,
-    RESPONSE_DEBUG_CONTENT,
-    RESPONSE_DEBUG_HEADERS,
-    RESPONSE_DEBUG_CONTEXT,
-    RESPONSE_DEBUG_MESSAGES,
-    RESPONSE_DEBUG_SESSION,
-    RESPONSE_DEBUG_FORMS,
-    RESPONSE_DEBUG_USER_INFO,
-    OUTPUT_EMPHASIS,
+    ETC_OUTPUT_ERROR_COLOR,
+    ETC_RESPONSE_DEBUG_CONTENT_COLOR,
+    ETC_RESPONSE_DEBUG_HEADER_COLOR,
+    ETC_RESPONSE_DEBUG_CONTEXT_COLOR,
+    ETC_RESPONSE_DEBUG_MESSAGE_COLOR,
+    ETC_RESPONSE_DEBUG_SESSION_COLOR,
+    ETC_RESPONSE_DEBUG_FORM_COLOR,
+    ETC_RESPONSE_DEBUG_USER_INFO_COLOR,
+    ETC_OUTPUT_EMPHASIS_COLOR,
 )
 
 
 # Initialize logging.
 logger = logging.getLogger(__name__)
 
 
@@ -60,16 +60,16 @@
         # Standardize output for easier analysis.
         response_content = self.standardize_characters(response_content)
         response_content = self.standardize_newlines(response_content)
 
         self._debug_print()
         self._debug_print(
             '{0} {1} {0}'.format('=' * 10, 'response.content'),
-            fore=RESPONSE_DEBUG_CONTENT,
-            style=OUTPUT_EMPHASIS,
+            fore=ETC_RESPONSE_DEBUG_CONTENT_COLOR,
+            style=ETC_OUTPUT_EMPHASIS_COLOR,
         )
 
         # Print out data, if present.
         if response_content:
             self._debug_print(response_content)
             self._debug_print()
 
@@ -87,22 +87,22 @@
                 response_headers = response_headers._headers
             else:
                 response_headers = None
 
         self._debug_print()
         self._debug_print(
             '{0} {1} {0}'.format('=' * 10, 'response.headers'),
-            fore=RESPONSE_DEBUG_HEADERS,
-            style=OUTPUT_EMPHASIS,
+            fore=ETC_RESPONSE_DEBUG_HEADER_COLOR,
+            style=ETC_OUTPUT_EMPHASIS_COLOR,
         )
 
         # Print out data, if present.
         if response_headers is not None and len(response_headers) > 0:
             for key, value in response_headers.items():
-                self._debug_print('    * "{0}": "{1}"'.format(key, value), fore=RESPONSE_DEBUG_HEADERS)
+                self._debug_print('    * "{0}": "{1}"'.format(key, value), fore=ETC_RESPONSE_DEBUG_HEADER_COLOR)
         else:
             self._debug_print('    No response headers found.')
         self._debug_print()
 
     def show_debug_context(self, response_context):
         """Prints debug response context data."""
 
@@ -124,196 +124,196 @@
                 for context in response_context:
                     temp_dict = {**temp_dict, **context}
                 response_context = temp_dict
 
         self._debug_print()
         self._debug_print(
             '{0} {1} {0}'.format('=' * 10, 'response.context'),
-            fore=RESPONSE_DEBUG_CONTEXT,
-            style=OUTPUT_EMPHASIS,
+            fore=ETC_RESPONSE_DEBUG_CONTEXT_COLOR,
+            style=ETC_OUTPUT_EMPHASIS_COLOR,
         )
 
         # NOTE: Response context object is strange, in that it's basically a dictionary,
         # and it allows .keys() but not .values(). Thus, iterate on keys only and pull respective value.
         if response_context is not None and len(response_context.keys()) > 0:
             # pass
             for key in response_context.keys():
                 context_value = str(response_context.get(key))
                 # Truncate display if very long.
                 if len(context_value) > 80:
                     context_value = '"{0}"..."{1}"'.format(context_value[:40], context_value[-40:])
-                self._debug_print('    * {0}: {1}'.format(key, context_value), fore=RESPONSE_DEBUG_CONTEXT)
+                self._debug_print('    * {0}: {1}'.format(key, context_value), fore=ETC_RESPONSE_DEBUG_CONTEXT_COLOR)
         else:
-            self._debug_print('    No context data found.', fore=RESPONSE_DEBUG_CONTEXT)
+            self._debug_print('    No context data found.', fore=ETC_RESPONSE_DEBUG_CONTEXT_COLOR)
         self._debug_print()
 
     def show_debug_session_data(self, client):
         """Prints debug response session data."""
 
         # Handle for potential param types.
         if isinstance(client, HttpResponseBase):
             client = client.client
 
         self._debug_print()
         self._debug_print(
             '{0} {1} {0}'.format('=' * 10, 'client.session'),
-            fore=RESPONSE_DEBUG_SESSION,
-            style=OUTPUT_EMPHASIS,
+            fore=ETC_RESPONSE_DEBUG_SESSION_COLOR,
+            style=ETC_OUTPUT_EMPHASIS_COLOR,
         )
 
         if client is not None and len(client.session.items()) > 0:
             for key, value in client.session.items():
-                self._debug_print('    * {0}: {1}'.format(key, value), fore=RESPONSE_DEBUG_SESSION)
+                self._debug_print('    * {0}: {1}'.format(key, value), fore=ETC_RESPONSE_DEBUG_SESSION_COLOR)
         else:
-            self._debug_print('    No session data found.', fore=RESPONSE_DEBUG_SESSION)
+            self._debug_print('    No session data found.', fore=ETC_RESPONSE_DEBUG_SESSION_COLOR)
         self._debug_print()
 
     def show_debug_messages(self, response_context):
         """Prints debug response message data."""
 
         # Handle for potential param types.
         if isinstance(response_context, HttpResponseBase):
             response_context = response_context.context
 
         self._debug_print()
         self._debug_print(
             '{0} {1} {0}'.format('=' * 10, 'response.context["messages"]'),
-            fore=RESPONSE_DEBUG_MESSAGES,
-            style=OUTPUT_EMPHASIS,
+            fore=ETC_RESPONSE_DEBUG_MESSAGE_COLOR,
+            style=ETC_OUTPUT_EMPHASIS_COLOR,
         )
 
         # Print out data, if present.
         if response_context is not None and 'messages' in response_context:
             messages = response_context['messages']
             if len(messages) > 0:
                 for message in messages:
-                    self._debug_print('    * "{0}"'.format(message), fore=RESPONSE_DEBUG_MESSAGES)
+                    self._debug_print('    * "{0}"'.format(message), fore=ETC_RESPONSE_DEBUG_MESSAGE_COLOR)
             else:
-                self._debug_print('    No context messages found.', fore=RESPONSE_DEBUG_MESSAGES)
+                self._debug_print('    No context messages found.', fore=ETC_RESPONSE_DEBUG_MESSAGE_COLOR)
         else:
-            self._debug_print('    No context messages found.', fore=RESPONSE_DEBUG_MESSAGES)
+            self._debug_print('    No context messages found.', fore=ETC_RESPONSE_DEBUG_MESSAGE_COLOR)
         self._debug_print()
 
     def show_debug_form_data(self, response_context):
         """Prints debug response form data."""
 
         # Handle for potential param types.
         if isinstance(response_context, HttpResponseBase):
             response_context = response_context.context
 
         self._debug_print()
         self._debug_print(
             '{0} {1} {0}'.format('=' * 10, 'Form Data'),
-            fore=RESPONSE_DEBUG_FORMS,
-            style=OUTPUT_EMPHASIS,
+            fore=ETC_RESPONSE_DEBUG_FORM_COLOR,
+            style=ETC_OUTPUT_EMPHASIS_COLOR,
         )
 
         # Check if form or formset data is actually present.
         if 'form' in response_context or 'formset' in response_context:
             # Form or formset present on page.
 
             # Attempt to get form data.
             form_present = False
             if 'form' in response_context:
                 form_present = True
                 form = response_context['form']
 
                 # Print general form data.
-                self._debug_print('    Provided Form Fields:', fore=RESPONSE_DEBUG_FORMS)
+                self._debug_print('    Provided Form Fields:', fore=ETC_RESPONSE_DEBUG_FORM_COLOR)
                 fields_submitted = False
                 for key, value in form.data.items():
-                    self._debug_print('        {0}: {1}'.format(key, value), fore=RESPONSE_DEBUG_FORMS)
+                    self._debug_print('        {0}: {1}'.format(key, value), fore=ETC_RESPONSE_DEBUG_FORM_COLOR)
                     fields_submitted = True
                 if not fields_submitted:
-                    self._debug_print('        No form field data submitted.', fore=RESPONSE_DEBUG_FORMS)
+                    self._debug_print('        No form field data submitted.', fore=ETC_RESPONSE_DEBUG_FORM_COLOR)
 
                 # Print form data errors if present.
                 if not form.is_valid():
                     self._debug_print()
                     if len(form.errors) > 0 or len(form.non_field_errors()) > 0:
-                        self._debug_print('    Form Invalid:'.format(not form.is_valid()), fore=RESPONSE_DEBUG_FORMS)
+                        self._debug_print('    Form Invalid:'.format(not form.is_valid()), fore=ETC_RESPONSE_DEBUG_FORM_COLOR)
                         if len(form.non_field_errors()) > 0:
-                            self._debug_print('        Non-field Frrors:', fore=RESPONSE_DEBUG_FORMS)
+                            self._debug_print('        Non-field Frrors:', fore=ETC_RESPONSE_DEBUG_FORM_COLOR)
                             for error in form.non_field_errors():
-                                self._debug_print('            {0}'.format(error), fore=RESPONSE_DEBUG_FORMS)
+                                self._debug_print('            {0}'.format(error), fore=ETC_RESPONSE_DEBUG_FORM_COLOR)
 
                         if len(form.errors) > 0:
-                            self._debug_print('        Field Errors:', fore=RESPONSE_DEBUG_FORMS)
+                            self._debug_print('        Field Errors:', fore=ETC_RESPONSE_DEBUG_FORM_COLOR)
                             for error in form.errors:
-                                self._debug_print('            {0}'.format(error), fore=RESPONSE_DEBUG_FORMS)
+                                self._debug_print('            {0}'.format(error), fore=ETC_RESPONSE_DEBUG_FORM_COLOR)
 
                 else:
-                    self._debug_print('    Form found and valid.', fore=RESPONSE_DEBUG_FORMS)
+                    self._debug_print('    Form found and valid.', fore=ETC_RESPONSE_DEBUG_FORM_COLOR)
 
             # Attempt to get formset data.
             if 'formset' in response_context:
                 if form_present:
                     self._debug_print()
                 formset = response_context['formset']
 
                 for form in formset:
                     self._debug_print('Form(set) Errors:')
                     for error in form.non_field_errors():
-                        self._debug_print('    {0}'.format(error), fore=RESPONSE_DEBUG_FORMS)
+                        self._debug_print('    {0}'.format(error), fore=ETC_RESPONSE_DEBUG_FORM_COLOR)
                     for error in form.errors:
-                        self._debug_print('    {0}'.format(error), fore=RESPONSE_DEBUG_FORMS)
+                        self._debug_print('    {0}'.format(error), fore=ETC_RESPONSE_DEBUG_FORM_COLOR)
         else:
             # No identifiable form or formset data present on page.
-            self._debug_print('    No form data found.', fore=RESPONSE_DEBUG_FORMS)
+            self._debug_print('    No form data found.', fore=ETC_RESPONSE_DEBUG_FORM_COLOR)
 
         self._debug_print()
 
     def show_debug_user_info(self, user):
         """Prints debug user data."""
 
         # Imported here to prevent potential "Apps aren't loaded yet" error.
         from django.contrib.auth.models import AnonymousUser
 
         self._debug_print()
         self._debug_print(
             '{0} {1} {0}'.format('=' * 10, 'User Info'),
-            fore=RESPONSE_DEBUG_USER_INFO,
-            style=OUTPUT_EMPHASIS,
+            fore=ETC_RESPONSE_DEBUG_USER_INFO_COLOR,
+            style=ETC_OUTPUT_EMPHASIS_COLOR,
         )
 
         # Only proceed if we got a proper user model.
         if isinstance(user, get_user_model()):
 
             # General user information.
-            self._debug_print('    * pk: "{0}"'.format(user.pk), fore=RESPONSE_DEBUG_USER_INFO)
-            self._debug_print('    * Username: "{0}"'.format(user.username), fore=RESPONSE_DEBUG_USER_INFO)
-            self._debug_print('    * First: "{0}"'.format(user.first_name), fore=RESPONSE_DEBUG_USER_INFO)
-            self._debug_print('    * Last: "{0}"'.format(user.last_name), fore=RESPONSE_DEBUG_USER_INFO)
-            self._debug_print('    * Email: "{0}"'.format(user.email), fore=RESPONSE_DEBUG_USER_INFO)
+            self._debug_print('    * pk: "{0}"'.format(user.pk), fore=ETC_RESPONSE_DEBUG_USER_INFO_COLOR)
+            self._debug_print('    * Username: "{0}"'.format(user.username), fore=ETC_RESPONSE_DEBUG_USER_INFO_COLOR)
+            self._debug_print('    * First: "{0}"'.format(user.first_name), fore=ETC_RESPONSE_DEBUG_USER_INFO_COLOR)
+            self._debug_print('    * Last: "{0}"'.format(user.last_name), fore=ETC_RESPONSE_DEBUG_USER_INFO_COLOR)
+            self._debug_print('    * Email: "{0}"'.format(user.email), fore=ETC_RESPONSE_DEBUG_USER_INFO_COLOR)
 
             # User auth data.
             self._debug_print(
                 '    * is_authenticated: {0}'.format(user.is_authenticated),
-                fore=RESPONSE_DEBUG_USER_INFO,
+                fore=ETC_RESPONSE_DEBUG_USER_INFO_COLOR,
             )
 
             # User groups.
-            self._debug_print('    * User Groups: {0}'.format(user.groups.all()), fore=RESPONSE_DEBUG_USER_INFO)
+            self._debug_print('    * User Groups: {0}'.format(user.groups.all()), fore=ETC_RESPONSE_DEBUG_USER_INFO_COLOR)
 
             # User permissions.
             self._debug_print(
                 '    * User Permissions: {0}'.format(user.user_permissions.all()),
-                fore=RESPONSE_DEBUG_USER_INFO,
+                fore=ETC_RESPONSE_DEBUG_USER_INFO_COLOR,
             )
 
         elif isinstance(user, AnonymousUser):
 
-            self._debug_print('    Anonymous user. No user is logged in.', fore=RESPONSE_DEBUG_USER_INFO)
+            self._debug_print('    Anonymous user. No user is logged in.', fore=ETC_RESPONSE_DEBUG_USER_INFO_COLOR)
 
         else:
             self._debug_print('    * Invalid user "{0}" of type "{1}". Expected "{2}".'.format(
                 user,
                 type(user),
                 type(get_user_model()),
-            ), fore=OUTPUT_ERROR)
+            ), fore=ETC_OUTPUT_ERROR_COLOR)
         self._debug_print()
         self._debug_print()
 
     # endregion Debug Output Functions.
 
     def standardize_html_tags(self, value):
         """Standardizes spacing around html-esque elements, to remove unnecessary spacing.
```

### Comparing `django-expanded-test-cases-0.3.0/django_expanded_test_cases/templates/django_expanded_test_cases/index.html` & `django-expanded-test-cases-0.4.0/django_expanded_test_cases/templates/django_expanded_test_cases/index.html`

 * *Files identical despite different names*

### Comparing `django-expanded-test-cases-0.3.0/django_expanded_test_cases/test_cases/__init__.py` & `django-expanded-test-cases-0.4.0/django_expanded_test_cases/test_cases/__init__.py`

 * *Files identical despite different names*

### Comparing `django-expanded-test-cases-0.3.0/django_expanded_test_cases/test_cases/base_test_case.py` & `django-expanded-test-cases-0.4.0/django_expanded_test_cases/test_cases/base_test_case.py`

 * *Files 1% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 Testing class for generalized logic.
 """
 
 # Third-Party Imports.
 from django.test import TestCase
 
 # Internal Imports.
-from django_expanded_test_cases.constants import OUTPUT_EMPHASIS, OUTPUT_ERROR
+from django_expanded_test_cases.constants import ETC_OUTPUT_EMPHASIS_COLOR, ETC_OUTPUT_ERROR_COLOR
 from django_expanded_test_cases.mixins import CoreTestCaseMixin
 
 
 class BaseTestCase(TestCase, CoreTestCaseMixin):
     """Generalized testing functionality. Builds upon Django's default TestCase class."""
 
     @classmethod
@@ -55,16 +55,16 @@
             # Print error to both logging and standard console output.
             self._debug_print(
                 '{0} {1} UnitTesting {2} {0}'.format(
                     ('=' * 10),
                     self.__class__.__name__,
                     type(err).__name__,
                 ),
-                fore=OUTPUT_ERROR,
-                style=OUTPUT_EMPHASIS,
+                fore=ETC_OUTPUT_ERROR_COLOR,
+                style=ETC_OUTPUT_EMPHASIS_COLOR,
             )
             self._debug_print('{0}\n\n'.format(str(err)))
 
             # Save that we have output error.
             self._error_displayed = True
 
     # region Default Test Function Overrides
```

### Comparing `django-expanded-test-cases-0.3.0/django_expanded_test_cases/test_cases/integration_test_case.py` & `django-expanded-test-cases-0.4.0/django_expanded_test_cases/test_cases/integration_test_case.py`

 * *Files 2% similar despite different names*

```diff
@@ -11,19 +11,27 @@
 from django.http.response import HttpResponseBase
 from django.urls import reverse
 from django.urls.exceptions import NoReverseMatch
 
 # Internal Imports.
 from .base_test_case import BaseTestCase
 from django_expanded_test_cases.constants import (
+    ETC_INCLUDE_RESPONSE_DEBUG_CONTENT,
+    ETC_INCLUDE_RESPONSE_DEBUG_CONTEXT,
+    ETC_INCLUDE_RESPONSE_DEBUG_FORMS,
+    ETC_INCLUDE_RESPONSE_DEBUG_HEADER,
+    ETC_INCLUDE_RESPONSE_DEBUG_MESSAGES,
+    ETC_INCLUDE_RESPONSE_DEBUG_SESSION,
+    ETC_INCLUDE_RESPONSE_DEBUG_URL,
+    ETC_INCLUDE_RESPONSE_DEBUG_USER_INFO,
     ETC_ALLOW_MESSAGE_PARTIALS,
     ETC_REQUEST_USER_STRICTNESS,
     ETC_DEFAULT_STANDARD_USER_IDENTIFIER,
-    RESPONSE_DEBUG_URL,
-    OUTPUT_EMPHASIS,
+    ETC_RESPONSE_DEBUG_URL_COLOR,
+    ETC_OUTPUT_EMPHASIS_COLOR,
     VOID_ELEMENT_LIST,
 )
 from django_expanded_test_cases.mixins import ResponseTestCaseMixin
 
 
 class IntegrationTestCase(BaseTestCase, ResponseTestCaseMixin):
     """Testing functionality for views and other multi-part components."""
@@ -100,21 +108,28 @@
             user_permissions=user_permissions,
             user_groups=user_groups,
             **kwargs,
         )
 
         # Optionally output all debug info for found response.
         if self._debug_print_bool:
-            self.show_debug_content(response)
-            self.show_debug_headers(response)
-            self.show_debug_context(response)
-            self.show_debug_session_data(response)
-            self.show_debug_messages(response)
-            self.show_debug_form_data(response)
-            self.show_debug_user_info(response.user)
+            if ETC_INCLUDE_RESPONSE_DEBUG_CONTENT:
+                self.show_debug_content(response)
+            if ETC_INCLUDE_RESPONSE_DEBUG_HEADER:
+                self.show_debug_headers(response)
+            if ETC_INCLUDE_RESPONSE_DEBUG_CONTEXT:
+                self.show_debug_context(response)
+            if ETC_INCLUDE_RESPONSE_DEBUG_SESSION:
+                self.show_debug_session_data(response)
+            if ETC_INCLUDE_RESPONSE_DEBUG_MESSAGES:
+                self.show_debug_messages(response)
+            if ETC_INCLUDE_RESPONSE_DEBUG_FORMS:
+                self.show_debug_form_data(response)
+            if ETC_INCLUDE_RESPONSE_DEBUG_USER_INFO:
+                self.show_debug_user_info(response.user)
 
         # Optional hook for running custom pre-builtin-test logic.
         self._assertResponse__pre_builtin_tests(
             url, *args,
             response=response,
             get=get, data=data,
             expected_redirect_url=expected_redirect_url, expected_status=expected_status,
@@ -733,63 +748,49 @@
         :param user:
         :param auto_login:
         :return:
         """
         # Django imports here to avoid situational "Apps aren't loaded yet" error.
         from django.contrib.auth.models import AnonymousUser
 
-        print('\n\n\n\n')
-        print('User: {0}'.format(user))
-
         # If user is None, attempt to fallback to class-user.
         if user is None:
             class_user = getattr(self, 'user', None)
             if class_user != AnonymousUser and class_user != AnonymousUser():
                 user = class_user
 
-        print('User: {0}'.format(user))
-
         # Proceed if user still None.
         if user is None:
             # Handle if default mode is "anonymous" and no user provided.
             if ETC_REQUEST_USER_STRICTNESS == 'anonymous':
-                print('Strictness: Anonymous')
                 user = AnonymousUser()
 
             # Handle if default mode is "relaxed" and no user provided.
             elif ETC_REQUEST_USER_STRICTNESS == 'relaxed':
-                print('Strictness: Relaxed')
                 user = ETC_DEFAULT_STANDARD_USER_IDENTIFIER
 
             # Handle if default mode is "strict" and no user provided.
             elif ETC_REQUEST_USER_STRICTNESS == 'strict':
                 # Handle for logging in a user.
-                print('Strictness: Strict')
                 if auto_login:
                     raise ValidationError(
                         'ETC_REQUEST_USER_STRICTNESS is set to "strict" but auto_login is True and no user was provided. '
                         'Please either set auto_login to False OR explicitly provide a user to authenticate with.'
                     )
 
             else:
                 raise ValueError(
                     'Invalid value provided for EXPANDED_TEST_CASES_REQUEST_USER_STRICTNESS setting. '
                     'Must be one of: ["anonymous", "relaxed", "strict"].'
                 )
 
-        print('User: {0}'.format(user))
-
         # Use anonymous user if not set to auto-login.
         if not auto_login:
             user = AnonymousUser()
 
-        print('User: {0}'.format(user))
-
-        print('\n\n\n\n')
-
         # Return calculated user.
         return user
 
     def _get_page_response(
         self,
         url,
         *args,
@@ -890,18 +891,20 @@
 
         # Log url we're attempting to access.
         if self.site_root_url is not None:
             current_site = '{0}{1}'.format(self.site_root_url, url)
         else:
             current_site = '127.0.0.1{0}'.format(url)
         message = 'Attempting to access url "{0}"'.format(current_site)
+
         self._debug_print('\n\n')
-        self._debug_print('{0}'.format('-' * len(message)), fore=RESPONSE_DEBUG_URL, style=OUTPUT_EMPHASIS)
-        self._debug_print(message, fore=RESPONSE_DEBUG_URL, style=OUTPUT_EMPHASIS)
-        self._debug_print('{0}'.format('-' * len(message)), fore=RESPONSE_DEBUG_URL, style=OUTPUT_EMPHASIS)
+        if ETC_INCLUDE_RESPONSE_DEBUG_URL:
+            self._debug_print('{0}'.format('-' * len(message)), fore=ETC_RESPONSE_DEBUG_URL_COLOR, style=ETC_OUTPUT_EMPHASIS_COLOR)
+            self._debug_print(message, fore=ETC_RESPONSE_DEBUG_URL_COLOR, style=ETC_OUTPUT_EMPHASIS_COLOR)
+            self._debug_print('{0}'.format('-' * len(message)), fore=ETC_RESPONSE_DEBUG_URL_COLOR, style=ETC_OUTPUT_EMPHASIS_COLOR)
 
         # Get response object.
         if bool(get):
             response = self.client.get(url, data=data, follow=True)
         else:
             response = self.client.post(url, data=data, follow=True)
```

### Comparing `django-expanded-test-cases-0.3.0/django_expanded_test_cases/test_cases/live_server_test_case.py` & `django-expanded-test-cases-0.4.0/django_expanded_test_cases/test_cases/live_server_test_case.py`

 * *Files identical despite different names*

### Comparing `django-expanded-test-cases-0.3.0/django_expanded_test_cases/test_urls.py` & `django-expanded-test-cases-0.4.0/django_expanded_test_cases/test_urls.py`

 * *Files identical despite different names*

### Comparing `django-expanded-test-cases-0.3.0/django_expanded_test_cases.egg-info/PKG-INFO` & `django-expanded-test-cases-0.4.0/django_expanded_test_cases.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: django-expanded-test-cases
-Version: 0.3.0
+Version: 0.4.0
 Summary: Expands the existing Django TestCase class with extra functionality.
 Home-page: https://github.com/brodriguez8774/django-expanded-test-cases
 Author: Brandon Rodriguez
 Author-email: Brandon Rodriguez <brodriguez8774@gmail.com>
 Maintainer-email: Brandon Rodriguez <brodriguez8774@gmail.com>
 License: MIT License
```

### Comparing `django-expanded-test-cases-0.3.0/django_expanded_test_cases.egg-info/SOURCES.txt` & `django-expanded-test-cases-0.4.0/django_expanded_test_cases.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `django-expanded-test-cases-0.3.0/pyproject.toml` & `django-expanded-test-cases-0.4.0/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ['setuptools>=40.8.0', 'wheel']
 build-backend = 'setuptools.build_meta:__legacy__'
 
 [project]
 name = "django-expanded-test-cases"
-version = "0.3.0"
+version = "0.4.0"
 description = "Expands the existing Django TestCase class with extra functionality."
 readme = "readme.md"
 authors = [
     { name = "Brandon Rodriguez", email = "brodriguez8774@gmail.com" },
 ]
 maintainers = [
     { name = "Brandon Rodriguez", email = "brodriguez8774@gmail.com" },
```

### Comparing `django-expanded-test-cases-0.3.0/readme.md` & `django-expanded-test-cases-0.4.0/readme.md`

 * *Files identical despite different names*

### Comparing `django-expanded-test-cases-0.3.0/setup.cfg` & `django-expanded-test-cases-0.4.0/setup.cfg`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [metadata]
 name = django-expanded-test-cases
-version = 0.3.0
+version = 0.4.0
 description = Expands the existing Django TestCase class with extra functionality.
 long_description = file: readme.md
 url = https://github.com/brodriguez8774/django-expanded-test-cases
 author = Brandon Rodriguez
 author_email = brodriguez8774@gmail.com
 license = MIT License
 classifiers =
```

### Comparing `django-expanded-test-cases-0.3.0/tests/settings.py` & `django-expanded-test-cases-0.4.0/tests/settings.py`

 * *Files identical despite different names*

### Comparing `django-expanded-test-cases-0.3.0/tests/test_cases/test_base_case.py` & `django-expanded-test-cases-0.4.0/tests/test_cases/test_base_case.py`

 * *Files 15% similar despite different names*

```diff
@@ -11,19 +11,19 @@
 from django.contrib.auth.models import Group, Permission
 from django.contrib.contenttypes.models import ContentType
 from django.test import override_settings
 
 # Internal Imports.
 from django_expanded_test_cases import BaseTestCase
 from django_expanded_test_cases.constants import (
-    OUTPUT_ACTUALS_MATCH,
-    OUTPUT_ACTUALS_ERROR,
-    OUTPUT_EXPECTED_MATCH,
-    OUTPUT_EXPECTED_ERROR,
-    OUTPUT_RESET,
+    ETC_OUTPUT_ACTUALS_MATCH_COLOR,
+    ETC_OUTPUT_ACTUALS_ERROR_COLOR,
+    ETC_OUTPUT_EXPECTED_MATCH_COLOR,
+    ETC_OUTPUT_EXPECTED_ERROR_COLOR,
+    ETC_OUTPUT_RESET_COLOR,
 )
 
 
 lorem_str = """
 Lorem ipsum dolor sit amet, consectetur adipiscing elit. Donec dui ex, convallis eu nulla dignissim, pretium luctus
 tellus. In hac habitasse platea dictumst. Interdum et malesuada fames ac ante ipsum primis in faucibus. Pellentesque
 porttitor accumsan dapibus. Nulla gravida malesuada suscipit. Ut diam ante, viverra nec tincidunt sit amet, pulvinar
@@ -211,161 +211,161 @@
             with redirect_stdout(std_out):
                 with self.assertRaises(AssertionError):
                     self.assertText('', 'Actuals has values here. Expected does not.')
             std_out_lines = std_out.getvalue().split('\n')[3:]
 
             # Test all line values.
             self.assertEqual(std_out_lines[0], '')
-            self.assertEqual(std_out_lines[1], OUTPUT_RESET)
-            self.assertEqual(std_out_lines[2], OUTPUT_RESET)
-            self.assertEqual(std_out_lines[3], OUTPUT_RESET)
-            self.assertEqual(std_out_lines[4], '{0}EXPECTED:{1}'.format(OUTPUT_EXPECTED_MATCH, OUTPUT_RESET))
-            self.assertEqual(std_out_lines[5], OUTPUT_RESET)
-            self.assertEqual(std_out_lines[6], OUTPUT_RESET)
-            self.assertEqual(std_out_lines[7], OUTPUT_RESET)
-            self.assertEqual(std_out_lines[8], '{0}ACTUAL:{1}'.format(OUTPUT_ACTUALS_MATCH, OUTPUT_RESET))
+            self.assertEqual(std_out_lines[1], ETC_OUTPUT_RESET_COLOR)
+            self.assertEqual(std_out_lines[2], ETC_OUTPUT_RESET_COLOR)
+            self.assertEqual(std_out_lines[3], ETC_OUTPUT_RESET_COLOR)
+            self.assertEqual(std_out_lines[4], '{0}EXPECTED:{1}'.format(ETC_OUTPUT_EXPECTED_MATCH_COLOR, ETC_OUTPUT_RESET_COLOR))
+            self.assertEqual(std_out_lines[5], ETC_OUTPUT_RESET_COLOR)
+            self.assertEqual(std_out_lines[6], ETC_OUTPUT_RESET_COLOR)
+            self.assertEqual(std_out_lines[7], ETC_OUTPUT_RESET_COLOR)
+            self.assertEqual(std_out_lines[8], '{0}ACTUAL:{1}'.format(ETC_OUTPUT_ACTUALS_MATCH_COLOR, ETC_OUTPUT_RESET_COLOR))
             self.assertEqual(
                 std_out_lines[9],
-                '{0}Actuals has values here. Expected does not.{1}'.format(OUTPUT_ACTUALS_ERROR, OUTPUT_RESET),
-            )
-            self.assertEqual(std_out_lines[10], OUTPUT_RESET)
-            self.assertEqual(std_out_lines[11], OUTPUT_RESET)
-            self.assertEqual(std_out_lines[12], OUTPUT_RESET)
+                '{0}Actuals has values here. Expected does not.{1}'.format(ETC_OUTPUT_ACTUALS_ERROR_COLOR, ETC_OUTPUT_RESET_COLOR),
+            )
+            self.assertEqual(std_out_lines[10], ETC_OUTPUT_RESET_COLOR)
+            self.assertEqual(std_out_lines[11], ETC_OUTPUT_RESET_COLOR)
+            self.assertEqual(std_out_lines[12], ETC_OUTPUT_RESET_COLOR)
             self.assertEqual(std_out_lines[13], '')
 
         with self.subTest('With actuals as empty'):
             std_out = StringIO()
             with redirect_stdout(std_out):
                 with self.assertRaises(AssertionError):
                     self.assertText('Expected has values here. Actuals does not.', '')
             std_out_lines = std_out.getvalue().split('\n')[5:]
 
             # Test all line values.
             self.assertEqual(std_out_lines[0], '')
-            self.assertEqual(std_out_lines[1], OUTPUT_RESET)
-            self.assertEqual(std_out_lines[2], OUTPUT_RESET)
-            self.assertEqual(std_out_lines[3], OUTPUT_RESET)
-            self.assertEqual(std_out_lines[4], '{0}EXPECTED:{1}'.format(OUTPUT_EXPECTED_MATCH, OUTPUT_RESET))
+            self.assertEqual(std_out_lines[1], ETC_OUTPUT_RESET_COLOR)
+            self.assertEqual(std_out_lines[2], ETC_OUTPUT_RESET_COLOR)
+            self.assertEqual(std_out_lines[3], ETC_OUTPUT_RESET_COLOR)
+            self.assertEqual(std_out_lines[4], '{0}EXPECTED:{1}'.format(ETC_OUTPUT_EXPECTED_MATCH_COLOR, ETC_OUTPUT_RESET_COLOR))
             self.assertEqual(
                 std_out_lines[5],
-                '{0}Expected has values here. Actuals does not.{1}'.format(OUTPUT_EXPECTED_ERROR, OUTPUT_RESET),
-            )
-            self.assertEqual(std_out_lines[6], OUTPUT_RESET)
-            self.assertEqual(std_out_lines[7], OUTPUT_RESET)
-            self.assertEqual(std_out_lines[8], OUTPUT_RESET)
-            self.assertEqual(std_out_lines[9], '{0}ACTUAL:{1}'.format(OUTPUT_ACTUALS_MATCH, OUTPUT_RESET))
-            self.assertEqual(std_out_lines[10], OUTPUT_RESET)
-            self.assertEqual(std_out_lines[11], OUTPUT_RESET)
-            self.assertEqual(std_out_lines[12], OUTPUT_RESET)
+                '{0}Expected has values here. Actuals does not.{1}'.format(ETC_OUTPUT_EXPECTED_ERROR_COLOR, ETC_OUTPUT_RESET_COLOR),
+            )
+            self.assertEqual(std_out_lines[6], ETC_OUTPUT_RESET_COLOR)
+            self.assertEqual(std_out_lines[7], ETC_OUTPUT_RESET_COLOR)
+            self.assertEqual(std_out_lines[8], ETC_OUTPUT_RESET_COLOR)
+            self.assertEqual(std_out_lines[9], '{0}ACTUAL:{1}'.format(ETC_OUTPUT_ACTUALS_MATCH_COLOR, ETC_OUTPUT_RESET_COLOR))
+            self.assertEqual(std_out_lines[10], ETC_OUTPUT_RESET_COLOR)
+            self.assertEqual(std_out_lines[11], ETC_OUTPUT_RESET_COLOR)
+            self.assertEqual(std_out_lines[12], ETC_OUTPUT_RESET_COLOR)
             self.assertEqual(std_out_lines[13], '')
 
         with self.subTest('With expected as empty and actuals as multi-line'):
             std_out = StringIO()
             with redirect_stdout(std_out):
                 with self.assertRaises(AssertionError):
                     self.assertText('', 'Actuals has values here.\nExpected does not.')
             std_out_lines = std_out.getvalue().split('\n')[4:]
 
             # Test all line values.
             self.assertEqual(std_out_lines[0], '')
-            self.assertEqual(std_out_lines[1], OUTPUT_RESET)
-            self.assertEqual(std_out_lines[2], OUTPUT_RESET)
-            self.assertEqual(std_out_lines[3], OUTPUT_RESET)
-            self.assertEqual(std_out_lines[4], '{0}EXPECTED:{1}'.format(OUTPUT_EXPECTED_MATCH, OUTPUT_RESET))
-            self.assertEqual(std_out_lines[5], OUTPUT_RESET)
-            self.assertEqual(std_out_lines[6], OUTPUT_RESET)
-            self.assertEqual(std_out_lines[7], OUTPUT_RESET)
-            self.assertEqual(std_out_lines[8], '{0}ACTUAL:{1}'.format(OUTPUT_ACTUALS_MATCH, OUTPUT_RESET))
-            self.assertEqual(
-                std_out_lines[9],
-                '{0}Actuals has values here.{1}'.format(OUTPUT_ACTUALS_ERROR, OUTPUT_RESET),
-            )
-            self.assertEqual(std_out_lines[10], '{0}Expected does not.{1}'.format(OUTPUT_ACTUALS_ERROR, OUTPUT_RESET))
-            self.assertEqual(std_out_lines[11], OUTPUT_RESET)
-            self.assertEqual(std_out_lines[12], OUTPUT_RESET)
-            self.assertEqual(std_out_lines[13], OUTPUT_RESET)
+            self.assertEqual(std_out_lines[1], ETC_OUTPUT_RESET_COLOR)
+            self.assertEqual(std_out_lines[2], ETC_OUTPUT_RESET_COLOR)
+            self.assertEqual(std_out_lines[3], ETC_OUTPUT_RESET_COLOR)
+            self.assertEqual(std_out_lines[4], '{0}EXPECTED:{1}'.format(ETC_OUTPUT_EXPECTED_MATCH_COLOR, ETC_OUTPUT_RESET_COLOR))
+            self.assertEqual(std_out_lines[5], ETC_OUTPUT_RESET_COLOR)
+            self.assertEqual(std_out_lines[6], ETC_OUTPUT_RESET_COLOR)
+            self.assertEqual(std_out_lines[7], ETC_OUTPUT_RESET_COLOR)
+            self.assertEqual(std_out_lines[8], '{0}ACTUAL:{1}'.format(ETC_OUTPUT_ACTUALS_MATCH_COLOR, ETC_OUTPUT_RESET_COLOR))
+            self.assertEqual(
+                std_out_lines[9],
+                '{0}Actuals has values here.{1}'.format(ETC_OUTPUT_ACTUALS_ERROR_COLOR, ETC_OUTPUT_RESET_COLOR),
+            )
+            self.assertEqual(std_out_lines[10], '{0}Expected does not.{1}'.format(ETC_OUTPUT_ACTUALS_ERROR_COLOR, ETC_OUTPUT_RESET_COLOR))
+            self.assertEqual(std_out_lines[11], ETC_OUTPUT_RESET_COLOR)
+            self.assertEqual(std_out_lines[12], ETC_OUTPUT_RESET_COLOR)
+            self.assertEqual(std_out_lines[13], ETC_OUTPUT_RESET_COLOR)
             self.assertEqual(std_out_lines[14], '')
 
         with self.subTest('With actuals as empty and expected as multi-line'):
             std_out = StringIO()
             with redirect_stdout(std_out):
                 with self.assertRaises(AssertionError):
                     self.assertText('Expected has values here.\nActuals does not.', '')
             std_out_lines = std_out.getvalue().split('\n')[4:]
 
             # Test all line values.
             self.assertEqual(std_out_lines[0], '')
-            self.assertEqual(std_out_lines[1], OUTPUT_RESET)
-            self.assertEqual(std_out_lines[2], OUTPUT_RESET)
-            self.assertEqual(std_out_lines[3], OUTPUT_RESET)
-            self.assertEqual(std_out_lines[4], '{0}EXPECTED:{1}'.format(OUTPUT_EXPECTED_MATCH, OUTPUT_RESET))
-            self.assertEqual(
-                std_out_lines[5],
-                '{0}Expected has values here.{1}'.format(OUTPUT_EXPECTED_ERROR, OUTPUT_RESET),
-            )
-            self.assertEqual(std_out_lines[6], '{0}Actuals does not.{1}'.format(OUTPUT_EXPECTED_ERROR, OUTPUT_RESET))
-            self.assertEqual(std_out_lines[7], OUTPUT_RESET)
-            self.assertEqual(std_out_lines[8], OUTPUT_RESET)
-            self.assertEqual(std_out_lines[9], OUTPUT_RESET)
-            self.assertEqual(std_out_lines[10], '{0}ACTUAL:{1}'.format(OUTPUT_ACTUALS_MATCH, OUTPUT_RESET))
-            self.assertEqual(std_out_lines[11], OUTPUT_RESET)
-            self.assertEqual(std_out_lines[12], OUTPUT_RESET)
-            self.assertEqual(std_out_lines[13], OUTPUT_RESET)
+            self.assertEqual(std_out_lines[1], ETC_OUTPUT_RESET_COLOR)
+            self.assertEqual(std_out_lines[2], ETC_OUTPUT_RESET_COLOR)
+            self.assertEqual(std_out_lines[3], ETC_OUTPUT_RESET_COLOR)
+            self.assertEqual(std_out_lines[4], '{0}EXPECTED:{1}'.format(ETC_OUTPUT_EXPECTED_MATCH_COLOR, ETC_OUTPUT_RESET_COLOR))
+            self.assertEqual(
+                std_out_lines[5],
+                '{0}Expected has values here.{1}'.format(ETC_OUTPUT_EXPECTED_ERROR_COLOR, ETC_OUTPUT_RESET_COLOR),
+            )
+            self.assertEqual(std_out_lines[6], '{0}Actuals does not.{1}'.format(ETC_OUTPUT_EXPECTED_ERROR_COLOR, ETC_OUTPUT_RESET_COLOR))
+            self.assertEqual(std_out_lines[7], ETC_OUTPUT_RESET_COLOR)
+            self.assertEqual(std_out_lines[8], ETC_OUTPUT_RESET_COLOR)
+            self.assertEqual(std_out_lines[9], ETC_OUTPUT_RESET_COLOR)
+            self.assertEqual(std_out_lines[10], '{0}ACTUAL:{1}'.format(ETC_OUTPUT_ACTUALS_MATCH_COLOR, ETC_OUTPUT_RESET_COLOR))
+            self.assertEqual(std_out_lines[11], ETC_OUTPUT_RESET_COLOR)
+            self.assertEqual(std_out_lines[12], ETC_OUTPUT_RESET_COLOR)
+            self.assertEqual(std_out_lines[13], ETC_OUTPUT_RESET_COLOR)
             self.assertEqual(std_out_lines[14], '')
 
         with self.subTest('With expected as one line less - At end'):
             std_out = StringIO()
             with redirect_stdout(std_out):
                 with self.assertRaises(AssertionError):
                     self.assertText('One line.', 'One line.\nTwo line.')
             print('std_out.getvalue():')
             print(std_out.getvalue())
             std_out_lines = std_out.getvalue().split('\n')[6:]
 
             # Test all line values.
             self.assertEqual(std_out_lines[0], '')
-            self.assertEqual(std_out_lines[1], OUTPUT_RESET)
-            self.assertEqual(std_out_lines[2], OUTPUT_RESET)
-            self.assertEqual(std_out_lines[3], OUTPUT_RESET)
-            self.assertEqual(std_out_lines[4], '{0}EXPECTED:{1}'.format(OUTPUT_EXPECTED_MATCH, OUTPUT_RESET))
-            self.assertEqual(std_out_lines[5], '{0}One line.{1}'.format(OUTPUT_EXPECTED_MATCH, OUTPUT_RESET))
-            self.assertEqual(std_out_lines[6], OUTPUT_RESET)
-            self.assertEqual(std_out_lines[7], OUTPUT_RESET)
-            self.assertEqual(std_out_lines[8], OUTPUT_RESET)
-            self.assertEqual(std_out_lines[9], '{0}ACTUAL:{1}'.format(OUTPUT_ACTUALS_MATCH, OUTPUT_RESET))
-            self.assertEqual(std_out_lines[10], '{0}One line.{1}'.format(OUTPUT_ACTUALS_MATCH, OUTPUT_RESET))
-            self.assertEqual(std_out_lines[11], '{0}Two line.{1}'.format(OUTPUT_ACTUALS_ERROR, OUTPUT_RESET))
-            self.assertEqual(std_out_lines[12], OUTPUT_RESET)
-            self.assertEqual(std_out_lines[13], OUTPUT_RESET)
-            self.assertEqual(std_out_lines[14], OUTPUT_RESET)
+            self.assertEqual(std_out_lines[1], ETC_OUTPUT_RESET_COLOR)
+            self.assertEqual(std_out_lines[2], ETC_OUTPUT_RESET_COLOR)
+            self.assertEqual(std_out_lines[3], ETC_OUTPUT_RESET_COLOR)
+            self.assertEqual(std_out_lines[4], '{0}EXPECTED:{1}'.format(ETC_OUTPUT_EXPECTED_MATCH_COLOR, ETC_OUTPUT_RESET_COLOR))
+            self.assertEqual(std_out_lines[5], '{0}One line.{1}'.format(ETC_OUTPUT_EXPECTED_MATCH_COLOR, ETC_OUTPUT_RESET_COLOR))
+            self.assertEqual(std_out_lines[6], ETC_OUTPUT_RESET_COLOR)
+            self.assertEqual(std_out_lines[7], ETC_OUTPUT_RESET_COLOR)
+            self.assertEqual(std_out_lines[8], ETC_OUTPUT_RESET_COLOR)
+            self.assertEqual(std_out_lines[9], '{0}ACTUAL:{1}'.format(ETC_OUTPUT_ACTUALS_MATCH_COLOR, ETC_OUTPUT_RESET_COLOR))
+            self.assertEqual(std_out_lines[10], '{0}One line.{1}'.format(ETC_OUTPUT_ACTUALS_MATCH_COLOR, ETC_OUTPUT_RESET_COLOR))
+            self.assertEqual(std_out_lines[11], '{0}Two line.{1}'.format(ETC_OUTPUT_ACTUALS_ERROR_COLOR, ETC_OUTPUT_RESET_COLOR))
+            self.assertEqual(std_out_lines[12], ETC_OUTPUT_RESET_COLOR)
+            self.assertEqual(std_out_lines[13], ETC_OUTPUT_RESET_COLOR)
+            self.assertEqual(std_out_lines[14], ETC_OUTPUT_RESET_COLOR)
             self.assertEqual(std_out_lines[15], '')
 
         with self.subTest('With actuals as one line less - At end'):
             std_out = StringIO()
             with redirect_stdout(std_out):
                 with self.assertRaises(AssertionError):
                     self.assertText('One line.\nTwo line.', 'One line.')
             std_out_lines = std_out.getvalue().split('\n')[5:]
 
             # Test all line values.
             self.assertEqual(std_out_lines[0], '')
-            self.assertEqual(std_out_lines[1], OUTPUT_RESET)
-            self.assertEqual(std_out_lines[2], OUTPUT_RESET)
-            self.assertEqual(std_out_lines[3], OUTPUT_RESET)
-            self.assertEqual(std_out_lines[4], '{0}EXPECTED:{1}'.format(OUTPUT_EXPECTED_MATCH, OUTPUT_RESET))
-            self.assertEqual(std_out_lines[5], '{0}One line.{1}'.format(OUTPUT_EXPECTED_MATCH, OUTPUT_RESET))
-            self.assertEqual(std_out_lines[6], '{0}Two line.{1}'.format(OUTPUT_EXPECTED_ERROR, OUTPUT_RESET))
-            self.assertEqual(std_out_lines[7], OUTPUT_RESET)
-            self.assertEqual(std_out_lines[8], OUTPUT_RESET)
-            self.assertEqual(std_out_lines[9], OUTPUT_RESET)
-            self.assertEqual(std_out_lines[10], '{0}ACTUAL:{1}'.format(OUTPUT_ACTUALS_MATCH, OUTPUT_RESET))
-            self.assertEqual(std_out_lines[11], '{0}One line.{1}'.format(OUTPUT_ACTUALS_MATCH, OUTPUT_RESET))
-            self.assertEqual(std_out_lines[12], OUTPUT_RESET)
-            self.assertEqual(std_out_lines[13], OUTPUT_RESET)
-            self.assertEqual(std_out_lines[14], OUTPUT_RESET)
+            self.assertEqual(std_out_lines[1], ETC_OUTPUT_RESET_COLOR)
+            self.assertEqual(std_out_lines[2], ETC_OUTPUT_RESET_COLOR)
+            self.assertEqual(std_out_lines[3], ETC_OUTPUT_RESET_COLOR)
+            self.assertEqual(std_out_lines[4], '{0}EXPECTED:{1}'.format(ETC_OUTPUT_EXPECTED_MATCH_COLOR, ETC_OUTPUT_RESET_COLOR))
+            self.assertEqual(std_out_lines[5], '{0}One line.{1}'.format(ETC_OUTPUT_EXPECTED_MATCH_COLOR, ETC_OUTPUT_RESET_COLOR))
+            self.assertEqual(std_out_lines[6], '{0}Two line.{1}'.format(ETC_OUTPUT_EXPECTED_ERROR_COLOR, ETC_OUTPUT_RESET_COLOR))
+            self.assertEqual(std_out_lines[7], ETC_OUTPUT_RESET_COLOR)
+            self.assertEqual(std_out_lines[8], ETC_OUTPUT_RESET_COLOR)
+            self.assertEqual(std_out_lines[9], ETC_OUTPUT_RESET_COLOR)
+            self.assertEqual(std_out_lines[10], '{0}ACTUAL:{1}'.format(ETC_OUTPUT_ACTUALS_MATCH_COLOR, ETC_OUTPUT_RESET_COLOR))
+            self.assertEqual(std_out_lines[11], '{0}One line.{1}'.format(ETC_OUTPUT_ACTUALS_MATCH_COLOR, ETC_OUTPUT_RESET_COLOR))
+            self.assertEqual(std_out_lines[12], ETC_OUTPUT_RESET_COLOR)
+            self.assertEqual(std_out_lines[13], ETC_OUTPUT_RESET_COLOR)
+            self.assertEqual(std_out_lines[14], ETC_OUTPUT_RESET_COLOR)
             self.assertEqual(std_out_lines[15], '')
 
     def test__assertText_coloring__missing_characters(self):
         """Tests assertText() function color output, when assertion fails due to inccorect character counts.
 
         All tests here should have equal line counts, but char counts per-line won't match.
         For lines that have equal char counts, the characters should fully match.
@@ -375,339 +375,339 @@
             with redirect_stdout(std_out):
                 with self.assertRaises(AssertionError):
                     self.assertText('esting.', 'Testing.')
             std_out_lines = std_out.getvalue().split('\n')[6:]
 
             # Test all line values.
             self.assertEqual(std_out_lines[0], '')
-            self.assertEqual(std_out_lines[1], OUTPUT_RESET)
-            self.assertEqual(std_out_lines[2], OUTPUT_RESET)
-            self.assertEqual(std_out_lines[3], OUTPUT_RESET)
-            self.assertEqual(std_out_lines[4], '{0}EXPECTED:{1}'.format(OUTPUT_EXPECTED_MATCH, OUTPUT_RESET))
+            self.assertEqual(std_out_lines[1], ETC_OUTPUT_RESET_COLOR)
+            self.assertEqual(std_out_lines[2], ETC_OUTPUT_RESET_COLOR)
+            self.assertEqual(std_out_lines[3], ETC_OUTPUT_RESET_COLOR)
+            self.assertEqual(std_out_lines[4], '{0}EXPECTED:{1}'.format(ETC_OUTPUT_EXPECTED_MATCH_COLOR, ETC_OUTPUT_RESET_COLOR))
             self.assertEqual(
                 std_out_lines[5],
-                '{0}esting.{1}'.format(OUTPUT_EXPECTED_ERROR, OUTPUT_RESET),
+                '{0}esting.{1}'.format(ETC_OUTPUT_EXPECTED_ERROR_COLOR, ETC_OUTPUT_RESET_COLOR),
             )
-            self.assertEqual(std_out_lines[6], OUTPUT_RESET)
-            self.assertEqual(std_out_lines[7], OUTPUT_RESET)
-            self.assertEqual(std_out_lines[8], '{0}ACTUAL:{1}'.format(OUTPUT_ACTUALS_MATCH, OUTPUT_RESET))
+            self.assertEqual(std_out_lines[6], ETC_OUTPUT_RESET_COLOR)
+            self.assertEqual(std_out_lines[7], ETC_OUTPUT_RESET_COLOR)
+            self.assertEqual(std_out_lines[8], '{0}ACTUAL:{1}'.format(ETC_OUTPUT_ACTUALS_MATCH_COLOR, ETC_OUTPUT_RESET_COLOR))
             self.assertEqual(
                 std_out_lines[9],
-                '{0}Testing.{1}'.format(OUTPUT_ACTUALS_ERROR, OUTPUT_RESET),
+                '{0}Testing.{1}'.format(ETC_OUTPUT_ACTUALS_ERROR_COLOR, ETC_OUTPUT_RESET_COLOR),
             )
-            self.assertEqual(std_out_lines[10], OUTPUT_RESET)
-            self.assertEqual(std_out_lines[11], OUTPUT_RESET)
+            self.assertEqual(std_out_lines[10], ETC_OUTPUT_RESET_COLOR)
+            self.assertEqual(std_out_lines[11], ETC_OUTPUT_RESET_COLOR)
             self.assertEqual(std_out_lines[12], '')
 
         with self.subTest('With actuals as one char missing - At start'):
             std_out = StringIO()
             with redirect_stdout(std_out):
                 with self.assertRaises(AssertionError):
                     self.assertText('Testing.', 'esting.')
             std_out_lines = std_out.getvalue().split('\n')[6:]
 
             # Test all line values.
             self.assertEqual(std_out_lines[0], '')
-            self.assertEqual(std_out_lines[1], OUTPUT_RESET)
-            self.assertEqual(std_out_lines[2], OUTPUT_RESET)
-            self.assertEqual(std_out_lines[3], OUTPUT_RESET)
-            self.assertEqual(std_out_lines[4], '{0}EXPECTED:{1}'.format(OUTPUT_EXPECTED_MATCH, OUTPUT_RESET))
+            self.assertEqual(std_out_lines[1], ETC_OUTPUT_RESET_COLOR)
+            self.assertEqual(std_out_lines[2], ETC_OUTPUT_RESET_COLOR)
+            self.assertEqual(std_out_lines[3], ETC_OUTPUT_RESET_COLOR)
+            self.assertEqual(std_out_lines[4], '{0}EXPECTED:{1}'.format(ETC_OUTPUT_EXPECTED_MATCH_COLOR, ETC_OUTPUT_RESET_COLOR))
             self.assertEqual(
                 std_out_lines[5],
-                '{0}Testing.{1}'.format(OUTPUT_EXPECTED_ERROR, OUTPUT_RESET),
+                '{0}Testing.{1}'.format(ETC_OUTPUT_EXPECTED_ERROR_COLOR, ETC_OUTPUT_RESET_COLOR),
             )
-            self.assertEqual(std_out_lines[6], OUTPUT_RESET)
-            self.assertEqual(std_out_lines[7], OUTPUT_RESET)
-            self.assertEqual(std_out_lines[8], '{0}ACTUAL:{1}'.format(OUTPUT_ACTUALS_MATCH, OUTPUT_RESET))
+            self.assertEqual(std_out_lines[6], ETC_OUTPUT_RESET_COLOR)
+            self.assertEqual(std_out_lines[7], ETC_OUTPUT_RESET_COLOR)
+            self.assertEqual(std_out_lines[8], '{0}ACTUAL:{1}'.format(ETC_OUTPUT_ACTUALS_MATCH_COLOR, ETC_OUTPUT_RESET_COLOR))
             self.assertEqual(
                 std_out_lines[9],
-                '{0}esting.{1}'.format(OUTPUT_ACTUALS_ERROR, OUTPUT_RESET),
+                '{0}esting.{1}'.format(ETC_OUTPUT_ACTUALS_ERROR_COLOR, ETC_OUTPUT_RESET_COLOR),
             )
-            self.assertEqual(std_out_lines[10], OUTPUT_RESET)
-            self.assertEqual(std_out_lines[11], OUTPUT_RESET)
+            self.assertEqual(std_out_lines[10], ETC_OUTPUT_RESET_COLOR)
+            self.assertEqual(std_out_lines[11], ETC_OUTPUT_RESET_COLOR)
             self.assertEqual(std_out_lines[12], '')
 
         with self.subTest('With expected as multiple characters missing - At start'):
             std_out = StringIO()
             with redirect_stdout(std_out):
                 with self.assertRaises(AssertionError):
                     self.assertText('sting.', 'Testing.')
             std_out_lines = std_out.getvalue().split('\n')[6:]
 
             # Test all line values.
             self.assertEqual(std_out_lines[0], '')
-            self.assertEqual(std_out_lines[1], OUTPUT_RESET)
-            self.assertEqual(std_out_lines[2], OUTPUT_RESET)
-            self.assertEqual(std_out_lines[3], OUTPUT_RESET)
-            self.assertEqual(std_out_lines[4], '{0}EXPECTED:{1}'.format(OUTPUT_EXPECTED_MATCH, OUTPUT_RESET))
+            self.assertEqual(std_out_lines[1], ETC_OUTPUT_RESET_COLOR)
+            self.assertEqual(std_out_lines[2], ETC_OUTPUT_RESET_COLOR)
+            self.assertEqual(std_out_lines[3], ETC_OUTPUT_RESET_COLOR)
+            self.assertEqual(std_out_lines[4], '{0}EXPECTED:{1}'.format(ETC_OUTPUT_EXPECTED_MATCH_COLOR, ETC_OUTPUT_RESET_COLOR))
             self.assertEqual(
                 std_out_lines[5],
-                '{0}sting.{1}'.format(OUTPUT_EXPECTED_ERROR, OUTPUT_RESET),
+                '{0}sting.{1}'.format(ETC_OUTPUT_EXPECTED_ERROR_COLOR, ETC_OUTPUT_RESET_COLOR),
             )
-            self.assertEqual(std_out_lines[6], OUTPUT_RESET)
-            self.assertEqual(std_out_lines[7], OUTPUT_RESET)
-            self.assertEqual(std_out_lines[8], '{0}ACTUAL:{1}'.format(OUTPUT_ACTUALS_MATCH, OUTPUT_RESET))
+            self.assertEqual(std_out_lines[6], ETC_OUTPUT_RESET_COLOR)
+            self.assertEqual(std_out_lines[7], ETC_OUTPUT_RESET_COLOR)
+            self.assertEqual(std_out_lines[8], '{0}ACTUAL:{1}'.format(ETC_OUTPUT_ACTUALS_MATCH_COLOR, ETC_OUTPUT_RESET_COLOR))
             self.assertEqual(
                 std_out_lines[9],
-                '{0}Testing.{1}'.format(OUTPUT_ACTUALS_ERROR, OUTPUT_RESET),
+                '{0}Testing.{1}'.format(ETC_OUTPUT_ACTUALS_ERROR_COLOR, ETC_OUTPUT_RESET_COLOR),
             )
-            self.assertEqual(std_out_lines[10], OUTPUT_RESET)
-            self.assertEqual(std_out_lines[11], OUTPUT_RESET)
+            self.assertEqual(std_out_lines[10], ETC_OUTPUT_RESET_COLOR)
+            self.assertEqual(std_out_lines[11], ETC_OUTPUT_RESET_COLOR)
             self.assertEqual(std_out_lines[12], '')
 
         with self.subTest('With actuals as multiple characters missing - At start'):
             std_out = StringIO()
             with redirect_stdout(std_out):
                 with self.assertRaises(AssertionError):
                     self.assertText('Testing.', 'sting.')
             std_out_lines = std_out.getvalue().split('\n')[6:]
 
             # Test all line values.
             self.assertEqual(std_out_lines[0], '')
-            self.assertEqual(std_out_lines[1], OUTPUT_RESET)
-            self.assertEqual(std_out_lines[2], OUTPUT_RESET)
-            self.assertEqual(std_out_lines[3], OUTPUT_RESET)
-            self.assertEqual(std_out_lines[4], '{0}EXPECTED:{1}'.format(OUTPUT_EXPECTED_MATCH, OUTPUT_RESET))
+            self.assertEqual(std_out_lines[1], ETC_OUTPUT_RESET_COLOR)
+            self.assertEqual(std_out_lines[2], ETC_OUTPUT_RESET_COLOR)
+            self.assertEqual(std_out_lines[3], ETC_OUTPUT_RESET_COLOR)
+            self.assertEqual(std_out_lines[4], '{0}EXPECTED:{1}'.format(ETC_OUTPUT_EXPECTED_MATCH_COLOR, ETC_OUTPUT_RESET_COLOR))
             self.assertEqual(
                 std_out_lines[5],
-                '{0}Testing.{1}'.format(OUTPUT_EXPECTED_ERROR, OUTPUT_RESET),
+                '{0}Testing.{1}'.format(ETC_OUTPUT_EXPECTED_ERROR_COLOR, ETC_OUTPUT_RESET_COLOR),
             )
-            self.assertEqual(std_out_lines[6], OUTPUT_RESET)
-            self.assertEqual(std_out_lines[7], OUTPUT_RESET)
-            self.assertEqual(std_out_lines[8], '{0}ACTUAL:{1}'.format(OUTPUT_ACTUALS_MATCH, OUTPUT_RESET))
+            self.assertEqual(std_out_lines[6], ETC_OUTPUT_RESET_COLOR)
+            self.assertEqual(std_out_lines[7], ETC_OUTPUT_RESET_COLOR)
+            self.assertEqual(std_out_lines[8], '{0}ACTUAL:{1}'.format(ETC_OUTPUT_ACTUALS_MATCH_COLOR, ETC_OUTPUT_RESET_COLOR))
             self.assertEqual(
                 std_out_lines[9],
-                '{0}sting.{1}'.format(OUTPUT_ACTUALS_ERROR, OUTPUT_RESET),
+                '{0}sting.{1}'.format(ETC_OUTPUT_ACTUALS_ERROR_COLOR, ETC_OUTPUT_RESET_COLOR),
             )
-            self.assertEqual(std_out_lines[10], OUTPUT_RESET)
-            self.assertEqual(std_out_lines[11], OUTPUT_RESET)
+            self.assertEqual(std_out_lines[10], ETC_OUTPUT_RESET_COLOR)
+            self.assertEqual(std_out_lines[11], ETC_OUTPUT_RESET_COLOR)
             self.assertEqual(std_out_lines[12], '')
 
         with self.subTest('With expected as one char missing - At middle'):
             std_out = StringIO()
             with redirect_stdout(std_out):
                 with self.assertRaises(AssertionError):
                     self.assertText('Tesing.', 'Testing.')
             std_out_lines = std_out.getvalue().split('\n')[6:]
 
             # Test all line values.
             self.assertEqual(std_out_lines[0], '')
-            self.assertEqual(std_out_lines[1], OUTPUT_RESET)
-            self.assertEqual(std_out_lines[2], OUTPUT_RESET)
-            self.assertEqual(std_out_lines[3], OUTPUT_RESET)
-            self.assertEqual(std_out_lines[4], '{0}EXPECTED:{1}'.format(OUTPUT_EXPECTED_MATCH, OUTPUT_RESET))
+            self.assertEqual(std_out_lines[1], ETC_OUTPUT_RESET_COLOR)
+            self.assertEqual(std_out_lines[2], ETC_OUTPUT_RESET_COLOR)
+            self.assertEqual(std_out_lines[3], ETC_OUTPUT_RESET_COLOR)
+            self.assertEqual(std_out_lines[4], '{0}EXPECTED:{1}'.format(ETC_OUTPUT_EXPECTED_MATCH_COLOR, ETC_OUTPUT_RESET_COLOR))
             self.assertEqual(
                 std_out_lines[5],
-                '{0}Tes{1}ing.{2}'.format(OUTPUT_EXPECTED_MATCH, OUTPUT_EXPECTED_ERROR, OUTPUT_RESET),
+                '{0}Tes{1}ing.{2}'.format(ETC_OUTPUT_EXPECTED_MATCH_COLOR, ETC_OUTPUT_EXPECTED_ERROR_COLOR, ETC_OUTPUT_RESET_COLOR),
             )
-            self.assertEqual(std_out_lines[6], OUTPUT_RESET)
-            self.assertEqual(std_out_lines[7], OUTPUT_RESET)
-            self.assertEqual(std_out_lines[8], '{0}ACTUAL:{1}'.format(OUTPUT_ACTUALS_MATCH, OUTPUT_RESET))
+            self.assertEqual(std_out_lines[6], ETC_OUTPUT_RESET_COLOR)
+            self.assertEqual(std_out_lines[7], ETC_OUTPUT_RESET_COLOR)
+            self.assertEqual(std_out_lines[8], '{0}ACTUAL:{1}'.format(ETC_OUTPUT_ACTUALS_MATCH_COLOR, ETC_OUTPUT_RESET_COLOR))
             self.assertEqual(
                 std_out_lines[9],
-                '{0}Tes{1}ting.{2}'.format(OUTPUT_ACTUALS_MATCH, OUTPUT_ACTUALS_ERROR, OUTPUT_RESET),
+                '{0}Tes{1}ting.{2}'.format(ETC_OUTPUT_ACTUALS_MATCH_COLOR, ETC_OUTPUT_ACTUALS_ERROR_COLOR, ETC_OUTPUT_RESET_COLOR),
             )
-            self.assertEqual(std_out_lines[10], OUTPUT_RESET)
-            self.assertEqual(std_out_lines[11], OUTPUT_RESET)
+            self.assertEqual(std_out_lines[10], ETC_OUTPUT_RESET_COLOR)
+            self.assertEqual(std_out_lines[11], ETC_OUTPUT_RESET_COLOR)
             self.assertEqual(std_out_lines[12], '')
 
         with self.subTest('With actuals as one char missing - At middle'):
             std_out = StringIO()
             with redirect_stdout(std_out):
                 with self.assertRaises(AssertionError):
                     self.assertText('Testing.', 'Tesing.')
             std_out_lines = std_out.getvalue().split('\n')[6:]
 
             # Test all line values.
             self.assertEqual(std_out_lines[0], '')
-            self.assertEqual(std_out_lines[1], OUTPUT_RESET)
-            self.assertEqual(std_out_lines[2], OUTPUT_RESET)
-            self.assertEqual(std_out_lines[3], OUTPUT_RESET)
-            self.assertEqual(std_out_lines[4], '{0}EXPECTED:{1}'.format(OUTPUT_EXPECTED_MATCH, OUTPUT_RESET))
+            self.assertEqual(std_out_lines[1], ETC_OUTPUT_RESET_COLOR)
+            self.assertEqual(std_out_lines[2], ETC_OUTPUT_RESET_COLOR)
+            self.assertEqual(std_out_lines[3], ETC_OUTPUT_RESET_COLOR)
+            self.assertEqual(std_out_lines[4], '{0}EXPECTED:{1}'.format(ETC_OUTPUT_EXPECTED_MATCH_COLOR, ETC_OUTPUT_RESET_COLOR))
             self.assertEqual(
                 std_out_lines[5],
-                '{0}Tes{1}ting.{2}'.format(OUTPUT_EXPECTED_MATCH, OUTPUT_EXPECTED_ERROR, OUTPUT_RESET),
+                '{0}Tes{1}ting.{2}'.format(ETC_OUTPUT_EXPECTED_MATCH_COLOR, ETC_OUTPUT_EXPECTED_ERROR_COLOR, ETC_OUTPUT_RESET_COLOR),
             )
-            self.assertEqual(std_out_lines[6], OUTPUT_RESET)
-            self.assertEqual(std_out_lines[7], OUTPUT_RESET)
-            self.assertEqual(std_out_lines[8], '{0}ACTUAL:{1}'.format(OUTPUT_ACTUALS_MATCH, OUTPUT_RESET))
+            self.assertEqual(std_out_lines[6], ETC_OUTPUT_RESET_COLOR)
+            self.assertEqual(std_out_lines[7], ETC_OUTPUT_RESET_COLOR)
+            self.assertEqual(std_out_lines[8], '{0}ACTUAL:{1}'.format(ETC_OUTPUT_ACTUALS_MATCH_COLOR, ETC_OUTPUT_RESET_COLOR))
             self.assertEqual(
                 std_out_lines[9],
-                '{0}Tes{1}ing.{2}'.format(OUTPUT_ACTUALS_MATCH, OUTPUT_ACTUALS_ERROR, OUTPUT_RESET),
+                '{0}Tes{1}ing.{2}'.format(ETC_OUTPUT_ACTUALS_MATCH_COLOR, ETC_OUTPUT_ACTUALS_ERROR_COLOR, ETC_OUTPUT_RESET_COLOR),
             )
-            self.assertEqual(std_out_lines[10], OUTPUT_RESET)
-            self.assertEqual(std_out_lines[11], OUTPUT_RESET)
+            self.assertEqual(std_out_lines[10], ETC_OUTPUT_RESET_COLOR)
+            self.assertEqual(std_out_lines[11], ETC_OUTPUT_RESET_COLOR)
             self.assertEqual(std_out_lines[12], '')
 
         with self.subTest('With expected as multiple characters missing - At middle'):
             std_out = StringIO()
             with redirect_stdout(std_out):
                 with self.assertRaises(AssertionError):
                     self.assertText('Teng.', 'Testing.')
             std_out_lines = std_out.getvalue().split('\n')[6:]
 
             # Test all line values.
             self.assertEqual(std_out_lines[0], '')
-            self.assertEqual(std_out_lines[1], OUTPUT_RESET)
-            self.assertEqual(std_out_lines[2], OUTPUT_RESET)
-            self.assertEqual(std_out_lines[3], OUTPUT_RESET)
-            self.assertEqual(std_out_lines[4], '{0}EXPECTED:{1}'.format(OUTPUT_EXPECTED_MATCH, OUTPUT_RESET))
+            self.assertEqual(std_out_lines[1], ETC_OUTPUT_RESET_COLOR)
+            self.assertEqual(std_out_lines[2], ETC_OUTPUT_RESET_COLOR)
+            self.assertEqual(std_out_lines[3], ETC_OUTPUT_RESET_COLOR)
+            self.assertEqual(std_out_lines[4], '{0}EXPECTED:{1}'.format(ETC_OUTPUT_EXPECTED_MATCH_COLOR, ETC_OUTPUT_RESET_COLOR))
             self.assertEqual(
                 std_out_lines[5],
-                '{0}Te{1}ng.{2}'.format(OUTPUT_EXPECTED_MATCH, OUTPUT_EXPECTED_ERROR, OUTPUT_RESET),
+                '{0}Te{1}ng.{2}'.format(ETC_OUTPUT_EXPECTED_MATCH_COLOR, ETC_OUTPUT_EXPECTED_ERROR_COLOR, ETC_OUTPUT_RESET_COLOR),
             )
-            self.assertEqual(std_out_lines[6], OUTPUT_RESET)
-            self.assertEqual(std_out_lines[7], OUTPUT_RESET)
-            self.assertEqual(std_out_lines[8], '{0}ACTUAL:{1}'.format(OUTPUT_ACTUALS_MATCH, OUTPUT_RESET))
+            self.assertEqual(std_out_lines[6], ETC_OUTPUT_RESET_COLOR)
+            self.assertEqual(std_out_lines[7], ETC_OUTPUT_RESET_COLOR)
+            self.assertEqual(std_out_lines[8], '{0}ACTUAL:{1}'.format(ETC_OUTPUT_ACTUALS_MATCH_COLOR, ETC_OUTPUT_RESET_COLOR))
             self.assertEqual(
                 std_out_lines[9],
-                '{0}Te{1}sting.{2}'.format(OUTPUT_ACTUALS_MATCH, OUTPUT_ACTUALS_ERROR, OUTPUT_RESET),
+                '{0}Te{1}sting.{2}'.format(ETC_OUTPUT_ACTUALS_MATCH_COLOR, ETC_OUTPUT_ACTUALS_ERROR_COLOR, ETC_OUTPUT_RESET_COLOR),
             )
-            self.assertEqual(std_out_lines[10], OUTPUT_RESET)
-            self.assertEqual(std_out_lines[11], OUTPUT_RESET)
+            self.assertEqual(std_out_lines[10], ETC_OUTPUT_RESET_COLOR)
+            self.assertEqual(std_out_lines[11], ETC_OUTPUT_RESET_COLOR)
             self.assertEqual(std_out_lines[12], '')
 
         with self.subTest('With actuals as multiple characters missing - At middle'):
             std_out = StringIO()
             with redirect_stdout(std_out):
                 with self.assertRaises(AssertionError):
                     self.assertText('Testing.', 'Teng.')
             std_out_lines = std_out.getvalue().split('\n')[6:]
 
             # Test all line values.
             self.assertEqual(std_out_lines[0], '')
-            self.assertEqual(std_out_lines[1], OUTPUT_RESET)
-            self.assertEqual(std_out_lines[2], OUTPUT_RESET)
-            self.assertEqual(std_out_lines[3], OUTPUT_RESET)
-            self.assertEqual(std_out_lines[4], '{0}EXPECTED:{1}'.format(OUTPUT_EXPECTED_MATCH, OUTPUT_RESET))
+            self.assertEqual(std_out_lines[1], ETC_OUTPUT_RESET_COLOR)
+            self.assertEqual(std_out_lines[2], ETC_OUTPUT_RESET_COLOR)
+            self.assertEqual(std_out_lines[3], ETC_OUTPUT_RESET_COLOR)
+            self.assertEqual(std_out_lines[4], '{0}EXPECTED:{1}'.format(ETC_OUTPUT_EXPECTED_MATCH_COLOR, ETC_OUTPUT_RESET_COLOR))
             self.assertEqual(
                 std_out_lines[5],
-                '{0}Te{1}sting.{2}'.format(OUTPUT_EXPECTED_MATCH, OUTPUT_EXPECTED_ERROR, OUTPUT_RESET),
+                '{0}Te{1}sting.{2}'.format(ETC_OUTPUT_EXPECTED_MATCH_COLOR, ETC_OUTPUT_EXPECTED_ERROR_COLOR, ETC_OUTPUT_RESET_COLOR),
             )
-            self.assertEqual(std_out_lines[6], OUTPUT_RESET)
-            self.assertEqual(std_out_lines[7], OUTPUT_RESET)
-            self.assertEqual(std_out_lines[8], '{0}ACTUAL:{1}'.format(OUTPUT_ACTUALS_MATCH, OUTPUT_RESET))
+            self.assertEqual(std_out_lines[6], ETC_OUTPUT_RESET_COLOR)
+            self.assertEqual(std_out_lines[7], ETC_OUTPUT_RESET_COLOR)
+            self.assertEqual(std_out_lines[8], '{0}ACTUAL:{1}'.format(ETC_OUTPUT_ACTUALS_MATCH_COLOR, ETC_OUTPUT_RESET_COLOR))
             self.assertEqual(
                 std_out_lines[9],
-                '{0}Te{1}ng.{2}'.format(OUTPUT_ACTUALS_MATCH, OUTPUT_ACTUALS_ERROR, OUTPUT_RESET),
+                '{0}Te{1}ng.{2}'.format(ETC_OUTPUT_ACTUALS_MATCH_COLOR, ETC_OUTPUT_ACTUALS_ERROR_COLOR, ETC_OUTPUT_RESET_COLOR),
             )
-            self.assertEqual(std_out_lines[10], OUTPUT_RESET)
-            self.assertEqual(std_out_lines[11], OUTPUT_RESET)
+            self.assertEqual(std_out_lines[10], ETC_OUTPUT_RESET_COLOR)
+            self.assertEqual(std_out_lines[11], ETC_OUTPUT_RESET_COLOR)
             self.assertEqual(std_out_lines[12], '')
 
         with self.subTest('With expected as one char missing - At end'):
             std_out = StringIO()
             with redirect_stdout(std_out):
                 with self.assertRaises(AssertionError):
                     self.assertText('Testing', 'Testing.')
             std_out_lines = std_out.getvalue().split('\n')[6:]
 
             # Test all line values.
             self.assertEqual(std_out_lines[0], '')
-            self.assertEqual(std_out_lines[1], OUTPUT_RESET)
-            self.assertEqual(std_out_lines[2], OUTPUT_RESET)
-            self.assertEqual(std_out_lines[3], OUTPUT_RESET)
-            self.assertEqual(std_out_lines[4], '{0}EXPECTED:{1}'.format(OUTPUT_EXPECTED_MATCH, OUTPUT_RESET))
+            self.assertEqual(std_out_lines[1], ETC_OUTPUT_RESET_COLOR)
+            self.assertEqual(std_out_lines[2], ETC_OUTPUT_RESET_COLOR)
+            self.assertEqual(std_out_lines[3], ETC_OUTPUT_RESET_COLOR)
+            self.assertEqual(std_out_lines[4], '{0}EXPECTED:{1}'.format(ETC_OUTPUT_EXPECTED_MATCH_COLOR, ETC_OUTPUT_RESET_COLOR))
             self.assertEqual(
                 std_out_lines[5],
-                '{0}Testing{1}{2}'.format(OUTPUT_EXPECTED_MATCH, OUTPUT_EXPECTED_ERROR, OUTPUT_RESET),
+                '{0}Testing{1}{2}'.format(ETC_OUTPUT_EXPECTED_MATCH_COLOR, ETC_OUTPUT_EXPECTED_ERROR_COLOR, ETC_OUTPUT_RESET_COLOR),
             )
-            self.assertEqual(std_out_lines[6], OUTPUT_RESET)
-            self.assertEqual(std_out_lines[7], OUTPUT_RESET)
-            self.assertEqual(std_out_lines[8], '{0}ACTUAL:{1}'.format(OUTPUT_ACTUALS_MATCH, OUTPUT_RESET))
+            self.assertEqual(std_out_lines[6], ETC_OUTPUT_RESET_COLOR)
+            self.assertEqual(std_out_lines[7], ETC_OUTPUT_RESET_COLOR)
+            self.assertEqual(std_out_lines[8], '{0}ACTUAL:{1}'.format(ETC_OUTPUT_ACTUALS_MATCH_COLOR, ETC_OUTPUT_RESET_COLOR))
             self.assertEqual(
                 std_out_lines[9],
-                '{0}Testing{1}.{2}'.format(OUTPUT_ACTUALS_MATCH, OUTPUT_ACTUALS_ERROR, OUTPUT_RESET),
+                '{0}Testing{1}.{2}'.format(ETC_OUTPUT_ACTUALS_MATCH_COLOR, ETC_OUTPUT_ACTUALS_ERROR_COLOR, ETC_OUTPUT_RESET_COLOR),
             )
-            self.assertEqual(std_out_lines[10], OUTPUT_RESET)
-            self.assertEqual(std_out_lines[11], OUTPUT_RESET)
+            self.assertEqual(std_out_lines[10], ETC_OUTPUT_RESET_COLOR)
+            self.assertEqual(std_out_lines[11], ETC_OUTPUT_RESET_COLOR)
             self.assertEqual(std_out_lines[12], '')
 
         with self.subTest('With actuals as one char missing - At end'):
             std_out = StringIO()
             with redirect_stdout(std_out):
                 with self.assertRaises(AssertionError):
                     self.assertText('Testing.', 'Testing')
             std_out_lines = std_out.getvalue().split('\n')[6:]
 
             # Test all line values.
             self.assertEqual(std_out_lines[0], '')
-            self.assertEqual(std_out_lines[1], OUTPUT_RESET)
-            self.assertEqual(std_out_lines[2], OUTPUT_RESET)
-            self.assertEqual(std_out_lines[3], OUTPUT_RESET)
-            self.assertEqual(std_out_lines[4], '{0}EXPECTED:{1}'.format(OUTPUT_EXPECTED_MATCH, OUTPUT_RESET))
+            self.assertEqual(std_out_lines[1], ETC_OUTPUT_RESET_COLOR)
+            self.assertEqual(std_out_lines[2], ETC_OUTPUT_RESET_COLOR)
+            self.assertEqual(std_out_lines[3], ETC_OUTPUT_RESET_COLOR)
+            self.assertEqual(std_out_lines[4], '{0}EXPECTED:{1}'.format(ETC_OUTPUT_EXPECTED_MATCH_COLOR, ETC_OUTPUT_RESET_COLOR))
             self.assertEqual(
                 std_out_lines[5],
-                '{0}Testing{1}.{2}'.format(OUTPUT_EXPECTED_MATCH, OUTPUT_EXPECTED_ERROR, OUTPUT_RESET),
+                '{0}Testing{1}.{2}'.format(ETC_OUTPUT_EXPECTED_MATCH_COLOR, ETC_OUTPUT_EXPECTED_ERROR_COLOR, ETC_OUTPUT_RESET_COLOR),
             )
-            self.assertEqual(std_out_lines[6], OUTPUT_RESET)
-            self.assertEqual(std_out_lines[7], OUTPUT_RESET)
-            self.assertEqual(std_out_lines[8], '{0}ACTUAL:{1}'.format(OUTPUT_ACTUALS_MATCH, OUTPUT_RESET))
+            self.assertEqual(std_out_lines[6], ETC_OUTPUT_RESET_COLOR)
+            self.assertEqual(std_out_lines[7], ETC_OUTPUT_RESET_COLOR)
+            self.assertEqual(std_out_lines[8], '{0}ACTUAL:{1}'.format(ETC_OUTPUT_ACTUALS_MATCH_COLOR, ETC_OUTPUT_RESET_COLOR))
             self.assertEqual(
                 std_out_lines[9],
-                '{0}Testing{1}{2}'.format(OUTPUT_ACTUALS_MATCH, OUTPUT_ACTUALS_ERROR, OUTPUT_RESET),
+                '{0}Testing{1}{2}'.format(ETC_OUTPUT_ACTUALS_MATCH_COLOR, ETC_OUTPUT_ACTUALS_ERROR_COLOR, ETC_OUTPUT_RESET_COLOR),
             )
-            self.assertEqual(std_out_lines[10], OUTPUT_RESET)
-            self.assertEqual(std_out_lines[11], OUTPUT_RESET)
+            self.assertEqual(std_out_lines[10], ETC_OUTPUT_RESET_COLOR)
+            self.assertEqual(std_out_lines[11], ETC_OUTPUT_RESET_COLOR)
             self.assertEqual(std_out_lines[12], '')
 
         with self.subTest('With expected as multiple characters missing - At end'):
             std_out = StringIO()
             with redirect_stdout(std_out):
                 with self.assertRaises(AssertionError):
                     self.assertText('Test', 'Testing.')
             std_out_lines = std_out.getvalue().split('\n')[5:]
 
             # Test all line values.
             self.assertEqual(std_out_lines[0], '')
-            self.assertEqual(std_out_lines[1], OUTPUT_RESET)
-            self.assertEqual(std_out_lines[2], OUTPUT_RESET)
-            self.assertEqual(std_out_lines[3], OUTPUT_RESET)
-            self.assertEqual(std_out_lines[4], '{0}EXPECTED:{1}'.format(OUTPUT_EXPECTED_MATCH, OUTPUT_RESET))
+            self.assertEqual(std_out_lines[1], ETC_OUTPUT_RESET_COLOR)
+            self.assertEqual(std_out_lines[2], ETC_OUTPUT_RESET_COLOR)
+            self.assertEqual(std_out_lines[3], ETC_OUTPUT_RESET_COLOR)
+            self.assertEqual(std_out_lines[4], '{0}EXPECTED:{1}'.format(ETC_OUTPUT_EXPECTED_MATCH_COLOR, ETC_OUTPUT_RESET_COLOR))
             self.assertEqual(
                 std_out_lines[5],
-                '{0}Test{1}{2}'.format(OUTPUT_EXPECTED_MATCH, OUTPUT_EXPECTED_ERROR, OUTPUT_RESET),
+                '{0}Test{1}{2}'.format(ETC_OUTPUT_EXPECTED_MATCH_COLOR, ETC_OUTPUT_EXPECTED_ERROR_COLOR, ETC_OUTPUT_RESET_COLOR),
             )
-            self.assertEqual(std_out_lines[6], OUTPUT_RESET)
-            self.assertEqual(std_out_lines[7], OUTPUT_RESET)
-            self.assertEqual(std_out_lines[8], '{0}ACTUAL:{1}'.format(OUTPUT_ACTUALS_MATCH, OUTPUT_RESET))
+            self.assertEqual(std_out_lines[6], ETC_OUTPUT_RESET_COLOR)
+            self.assertEqual(std_out_lines[7], ETC_OUTPUT_RESET_COLOR)
+            self.assertEqual(std_out_lines[8], '{0}ACTUAL:{1}'.format(ETC_OUTPUT_ACTUALS_MATCH_COLOR, ETC_OUTPUT_RESET_COLOR))
             self.assertEqual(
                 std_out_lines[9],
-                '{0}Test{1}ing.{2}'.format(OUTPUT_ACTUALS_MATCH, OUTPUT_ACTUALS_ERROR, OUTPUT_RESET),
+                '{0}Test{1}ing.{2}'.format(ETC_OUTPUT_ACTUALS_MATCH_COLOR, ETC_OUTPUT_ACTUALS_ERROR_COLOR, ETC_OUTPUT_RESET_COLOR),
             )
-            self.assertEqual(std_out_lines[10], OUTPUT_RESET)
-            self.assertEqual(std_out_lines[11], OUTPUT_RESET)
+            self.assertEqual(std_out_lines[10], ETC_OUTPUT_RESET_COLOR)
+            self.assertEqual(std_out_lines[11], ETC_OUTPUT_RESET_COLOR)
             self.assertEqual(std_out_lines[12], '')
 
         with self.subTest('With actuals as multiple characters missing - At end'):
             std_out = StringIO()
             with redirect_stdout(std_out):
                 with self.assertRaises(AssertionError):
                     self.assertText('Testing.', 'Test')
             std_out_lines = std_out.getvalue().split('\n')[5:]
 
             # Test all line values.
             self.assertEqual(std_out_lines[0], '')
-            self.assertEqual(std_out_lines[1], OUTPUT_RESET)
-            self.assertEqual(std_out_lines[2], OUTPUT_RESET)
-            self.assertEqual(std_out_lines[3], OUTPUT_RESET)
-            self.assertEqual(std_out_lines[4], '{0}EXPECTED:{1}'.format(OUTPUT_EXPECTED_MATCH, OUTPUT_RESET))
+            self.assertEqual(std_out_lines[1], ETC_OUTPUT_RESET_COLOR)
+            self.assertEqual(std_out_lines[2], ETC_OUTPUT_RESET_COLOR)
+            self.assertEqual(std_out_lines[3], ETC_OUTPUT_RESET_COLOR)
+            self.assertEqual(std_out_lines[4], '{0}EXPECTED:{1}'.format(ETC_OUTPUT_EXPECTED_MATCH_COLOR, ETC_OUTPUT_RESET_COLOR))
             self.assertEqual(
                 std_out_lines[5],
-                '{0}Test{1}ing.{2}'.format(OUTPUT_EXPECTED_MATCH, OUTPUT_EXPECTED_ERROR, OUTPUT_RESET),
+                '{0}Test{1}ing.{2}'.format(ETC_OUTPUT_EXPECTED_MATCH_COLOR, ETC_OUTPUT_EXPECTED_ERROR_COLOR, ETC_OUTPUT_RESET_COLOR),
             )
-            self.assertEqual(std_out_lines[6], OUTPUT_RESET)
-            self.assertEqual(std_out_lines[7], OUTPUT_RESET)
-            self.assertEqual(std_out_lines[8], '{0}ACTUAL:{1}'.format(OUTPUT_ACTUALS_MATCH, OUTPUT_RESET))
+            self.assertEqual(std_out_lines[6], ETC_OUTPUT_RESET_COLOR)
+            self.assertEqual(std_out_lines[7], ETC_OUTPUT_RESET_COLOR)
+            self.assertEqual(std_out_lines[8], '{0}ACTUAL:{1}'.format(ETC_OUTPUT_ACTUALS_MATCH_COLOR, ETC_OUTPUT_RESET_COLOR))
             self.assertEqual(
                 std_out_lines[9],
-                '{0}Test{1}{2}'.format(OUTPUT_ACTUALS_MATCH, OUTPUT_ACTUALS_ERROR, OUTPUT_RESET),
+                '{0}Test{1}{2}'.format(ETC_OUTPUT_ACTUALS_MATCH_COLOR, ETC_OUTPUT_ACTUALS_ERROR_COLOR, ETC_OUTPUT_RESET_COLOR),
             )
-            self.assertEqual(std_out_lines[10], OUTPUT_RESET)
-            self.assertEqual(std_out_lines[11], OUTPUT_RESET)
+            self.assertEqual(std_out_lines[10], ETC_OUTPUT_RESET_COLOR)
+            self.assertEqual(std_out_lines[11], ETC_OUTPUT_RESET_COLOR)
             self.assertEqual(std_out_lines[12], '')
 
     def test__assertText_coloring__wrong_characters(self):
         """Tests assertText() function color output, when assertion fails due incorrect characters.
 
         All tests here should have equal line counts and char counts per-line.
         """
@@ -716,219 +716,219 @@
             with redirect_stdout(std_out):
                 with self.assertRaises(AssertionError):
                     self.assertText('aBC', 'ABC')
             std_out_lines = std_out.getvalue().split('\n')[7:]
 
             # Test all line values.
             self.assertEqual(std_out_lines[0], '')
-            self.assertEqual(std_out_lines[1], OUTPUT_RESET)
-            self.assertEqual(std_out_lines[2], OUTPUT_RESET)
-            self.assertEqual(std_out_lines[3], OUTPUT_RESET)
-            self.assertEqual(std_out_lines[4], '{0}EXPECTED:{1}'.format(OUTPUT_EXPECTED_MATCH, OUTPUT_RESET))
+            self.assertEqual(std_out_lines[1], ETC_OUTPUT_RESET_COLOR)
+            self.assertEqual(std_out_lines[2], ETC_OUTPUT_RESET_COLOR)
+            self.assertEqual(std_out_lines[3], ETC_OUTPUT_RESET_COLOR)
+            self.assertEqual(std_out_lines[4], '{0}EXPECTED:{1}'.format(ETC_OUTPUT_EXPECTED_MATCH_COLOR, ETC_OUTPUT_RESET_COLOR))
             self.assertEqual(
                 std_out_lines[5],
                 '{0}a{1}BC{2}'.format(
-                    OUTPUT_EXPECTED_ERROR,
-                    OUTPUT_EXPECTED_MATCH,
-                    OUTPUT_RESET,
+                    ETC_OUTPUT_EXPECTED_ERROR_COLOR,
+                    ETC_OUTPUT_EXPECTED_MATCH_COLOR,
+                    ETC_OUTPUT_RESET_COLOR,
                 ),
             )
-            self.assertEqual(std_out_lines[6], OUTPUT_RESET)
-            self.assertEqual(std_out_lines[7], OUTPUT_RESET)
-            self.assertEqual(std_out_lines[8], '{0}ACTUAL:{1}'.format(OUTPUT_ACTUALS_MATCH, OUTPUT_RESET))
+            self.assertEqual(std_out_lines[6], ETC_OUTPUT_RESET_COLOR)
+            self.assertEqual(std_out_lines[7], ETC_OUTPUT_RESET_COLOR)
+            self.assertEqual(std_out_lines[8], '{0}ACTUAL:{1}'.format(ETC_OUTPUT_ACTUALS_MATCH_COLOR, ETC_OUTPUT_RESET_COLOR))
             self.assertEqual(
                 std_out_lines[9],
                 '{0}A{1}BC{2}'.format(
-                    OUTPUT_ACTUALS_ERROR,
-                    OUTPUT_ACTUALS_MATCH,
-                    OUTPUT_RESET,
+                    ETC_OUTPUT_ACTUALS_ERROR_COLOR,
+                    ETC_OUTPUT_ACTUALS_MATCH_COLOR,
+                    ETC_OUTPUT_RESET_COLOR,
                 ),
             )
-            self.assertEqual(std_out_lines[10], OUTPUT_RESET)
-            self.assertEqual(std_out_lines[11], OUTPUT_RESET)
+            self.assertEqual(std_out_lines[10], ETC_OUTPUT_RESET_COLOR)
+            self.assertEqual(std_out_lines[11], ETC_OUTPUT_RESET_COLOR)
             self.assertEqual(std_out_lines[12], '')
 
         with self.subTest('With wrong characters at start - Larger str'):
             std_out = StringIO()
             with redirect_stdout(std_out):
                 with self.assertRaises(AssertionError):
                     self.assertText('tHIS is a test value.', 'This is a test value.')
             std_out_lines = std_out.getvalue().split('\n')[7:]
 
             # Test all line values.
             self.assertEqual(std_out_lines[0], '')
-            self.assertEqual(std_out_lines[1], OUTPUT_RESET)
-            self.assertEqual(std_out_lines[2], OUTPUT_RESET)
-            self.assertEqual(std_out_lines[3], OUTPUT_RESET)
-            self.assertEqual(std_out_lines[4], '{0}EXPECTED:{1}'.format(OUTPUT_EXPECTED_MATCH, OUTPUT_RESET))
+            self.assertEqual(std_out_lines[1], ETC_OUTPUT_RESET_COLOR)
+            self.assertEqual(std_out_lines[2], ETC_OUTPUT_RESET_COLOR)
+            self.assertEqual(std_out_lines[3], ETC_OUTPUT_RESET_COLOR)
+            self.assertEqual(std_out_lines[4], '{0}EXPECTED:{1}'.format(ETC_OUTPUT_EXPECTED_MATCH_COLOR, ETC_OUTPUT_RESET_COLOR))
             self.assertEqual(
                 std_out_lines[5],
                 '{0}tHIS{1} is a test value.{2}'.format(
-                    OUTPUT_EXPECTED_ERROR,
-                    OUTPUT_EXPECTED_MATCH,
-                    OUTPUT_RESET,
+                    ETC_OUTPUT_EXPECTED_ERROR_COLOR,
+                    ETC_OUTPUT_EXPECTED_MATCH_COLOR,
+                    ETC_OUTPUT_RESET_COLOR,
                 ),
             )
-            self.assertEqual(std_out_lines[6], OUTPUT_RESET)
-            self.assertEqual(std_out_lines[7], OUTPUT_RESET)
-            self.assertEqual(std_out_lines[8], '{0}ACTUAL:{1}'.format(OUTPUT_ACTUALS_MATCH, OUTPUT_RESET))
+            self.assertEqual(std_out_lines[6], ETC_OUTPUT_RESET_COLOR)
+            self.assertEqual(std_out_lines[7], ETC_OUTPUT_RESET_COLOR)
+            self.assertEqual(std_out_lines[8], '{0}ACTUAL:{1}'.format(ETC_OUTPUT_ACTUALS_MATCH_COLOR, ETC_OUTPUT_RESET_COLOR))
             self.assertEqual(
                 std_out_lines[9],
                 '{0}This{1} is a test value.{2}'.format(
-                    OUTPUT_ACTUALS_ERROR,
-                    OUTPUT_ACTUALS_MATCH,
-                    OUTPUT_RESET,
+                    ETC_OUTPUT_ACTUALS_ERROR_COLOR,
+                    ETC_OUTPUT_ACTUALS_MATCH_COLOR,
+                    ETC_OUTPUT_RESET_COLOR,
                 ),
             )
-            self.assertEqual(std_out_lines[10], OUTPUT_RESET)
-            self.assertEqual(std_out_lines[11], OUTPUT_RESET)
+            self.assertEqual(std_out_lines[10], ETC_OUTPUT_RESET_COLOR)
+            self.assertEqual(std_out_lines[11], ETC_OUTPUT_RESET_COLOR)
             self.assertEqual(std_out_lines[12], '')
 
         with self.subTest('With wrong character at middle - Small str'):
             std_out = StringIO()
             with redirect_stdout(std_out):
                 with self.assertRaises(AssertionError):
                     self.assertText('AbC', 'ABC')
             std_out_lines = std_out.getvalue().split('\n')[7:]
 
             # Test all line values.
             self.assertEqual(std_out_lines[0], '')
-            self.assertEqual(std_out_lines[1], OUTPUT_RESET)
-            self.assertEqual(std_out_lines[2], OUTPUT_RESET)
-            self.assertEqual(std_out_lines[3], OUTPUT_RESET)
-            self.assertEqual(std_out_lines[4], '{0}EXPECTED:{1}'.format(OUTPUT_EXPECTED_MATCH, OUTPUT_RESET))
+            self.assertEqual(std_out_lines[1], ETC_OUTPUT_RESET_COLOR)
+            self.assertEqual(std_out_lines[2], ETC_OUTPUT_RESET_COLOR)
+            self.assertEqual(std_out_lines[3], ETC_OUTPUT_RESET_COLOR)
+            self.assertEqual(std_out_lines[4], '{0}EXPECTED:{1}'.format(ETC_OUTPUT_EXPECTED_MATCH_COLOR, ETC_OUTPUT_RESET_COLOR))
             self.assertEqual(
                 std_out_lines[5],
                 '{0}A{1}b{0}C{2}'.format(
-                    OUTPUT_EXPECTED_MATCH,
-                    OUTPUT_EXPECTED_ERROR,
-                    OUTPUT_RESET,
+                    ETC_OUTPUT_EXPECTED_MATCH_COLOR,
+                    ETC_OUTPUT_EXPECTED_ERROR_COLOR,
+                    ETC_OUTPUT_RESET_COLOR,
                 ),
             )
-            self.assertEqual(std_out_lines[6], OUTPUT_RESET)
-            self.assertEqual(std_out_lines[7], OUTPUT_RESET)
-            self.assertEqual(std_out_lines[8], '{0}ACTUAL:{1}'.format(OUTPUT_ACTUALS_MATCH, OUTPUT_RESET))
+            self.assertEqual(std_out_lines[6], ETC_OUTPUT_RESET_COLOR)
+            self.assertEqual(std_out_lines[7], ETC_OUTPUT_RESET_COLOR)
+            self.assertEqual(std_out_lines[8], '{0}ACTUAL:{1}'.format(ETC_OUTPUT_ACTUALS_MATCH_COLOR, ETC_OUTPUT_RESET_COLOR))
             self.assertEqual(
                 std_out_lines[9],
                 '{0}A{1}B{0}C{2}'.format(
-                    OUTPUT_ACTUALS_MATCH,
-                    OUTPUT_ACTUALS_ERROR,
-                    OUTPUT_RESET,
+                    ETC_OUTPUT_ACTUALS_MATCH_COLOR,
+                    ETC_OUTPUT_ACTUALS_ERROR_COLOR,
+                    ETC_OUTPUT_RESET_COLOR,
                 ),
             )
-            self.assertEqual(std_out_lines[10], OUTPUT_RESET)
-            self.assertEqual(std_out_lines[11], OUTPUT_RESET)
+            self.assertEqual(std_out_lines[10], ETC_OUTPUT_RESET_COLOR)
+            self.assertEqual(std_out_lines[11], ETC_OUTPUT_RESET_COLOR)
             self.assertEqual(std_out_lines[12], '')
 
         with self.subTest('With wrong character at middle - Larger str'):
             std_out = StringIO()
             with redirect_stdout(std_out):
                 with self.assertRaises(AssertionError):
                     self.assertText('This IS A TEST value.', 'This is a test value.')
             std_out_lines = std_out.getvalue().split('\n')[5:]
 
             # Test all line values.
             self.assertEqual(std_out_lines[0], '')
-            self.assertEqual(std_out_lines[1], OUTPUT_RESET)
-            self.assertEqual(std_out_lines[2], OUTPUT_RESET)
-            self.assertEqual(std_out_lines[3], OUTPUT_RESET)
-            self.assertEqual(std_out_lines[4], '{0}EXPECTED:{1}'.format(OUTPUT_EXPECTED_MATCH, OUTPUT_RESET))
+            self.assertEqual(std_out_lines[1], ETC_OUTPUT_RESET_COLOR)
+            self.assertEqual(std_out_lines[2], ETC_OUTPUT_RESET_COLOR)
+            self.assertEqual(std_out_lines[3], ETC_OUTPUT_RESET_COLOR)
+            self.assertEqual(std_out_lines[4], '{0}EXPECTED:{1}'.format(ETC_OUTPUT_EXPECTED_MATCH_COLOR, ETC_OUTPUT_RESET_COLOR))
             self.assertEqual(
                 std_out_lines[5],
                 '{0}This {1}IS{0} {1}A{0} {1}TEST{0} value.{2}'.format(
-                    OUTPUT_EXPECTED_MATCH,
-                    OUTPUT_EXPECTED_ERROR,
-                    OUTPUT_RESET,
+                    ETC_OUTPUT_EXPECTED_MATCH_COLOR,
+                    ETC_OUTPUT_EXPECTED_ERROR_COLOR,
+                    ETC_OUTPUT_RESET_COLOR,
                 ),
             )
-            self.assertEqual(std_out_lines[6], OUTPUT_RESET)
-            self.assertEqual(std_out_lines[7], OUTPUT_RESET)
-            self.assertEqual(std_out_lines[8], '{0}ACTUAL:{1}'.format(OUTPUT_ACTUALS_MATCH, OUTPUT_RESET))
+            self.assertEqual(std_out_lines[6], ETC_OUTPUT_RESET_COLOR)
+            self.assertEqual(std_out_lines[7], ETC_OUTPUT_RESET_COLOR)
+            self.assertEqual(std_out_lines[8], '{0}ACTUAL:{1}'.format(ETC_OUTPUT_ACTUALS_MATCH_COLOR, ETC_OUTPUT_RESET_COLOR))
             self.assertEqual(
                 std_out_lines[9],
                 '{0}This {1}is{0} {1}a{0} {1}test{0} value.{2}'.format(
-                    OUTPUT_ACTUALS_MATCH,
-                    OUTPUT_ACTUALS_ERROR,
-                    OUTPUT_RESET,
+                    ETC_OUTPUT_ACTUALS_MATCH_COLOR,
+                    ETC_OUTPUT_ACTUALS_ERROR_COLOR,
+                    ETC_OUTPUT_RESET_COLOR,
                 ),
             )
-            self.assertEqual(std_out_lines[10], OUTPUT_RESET)
-            self.assertEqual(std_out_lines[11], OUTPUT_RESET)
+            self.assertEqual(std_out_lines[10], ETC_OUTPUT_RESET_COLOR)
+            self.assertEqual(std_out_lines[11], ETC_OUTPUT_RESET_COLOR)
             self.assertEqual(std_out_lines[12], '')
 
         with self.subTest('With wrong character at end - Small str'):
             std_out = StringIO()
             with redirect_stdout(std_out):
                 with self.assertRaises(AssertionError):
                     self.assertText('ABc', 'ABC')
             std_out_lines = std_out.getvalue().split('\n')[7:]
 
             # Test all line values.
             self.assertEqual(std_out_lines[0], '')
-            self.assertEqual(std_out_lines[1], OUTPUT_RESET)
-            self.assertEqual(std_out_lines[2], OUTPUT_RESET)
-            self.assertEqual(std_out_lines[3], OUTPUT_RESET)
-            self.assertEqual(std_out_lines[4], '{0}EXPECTED:{1}'.format(OUTPUT_EXPECTED_MATCH, OUTPUT_RESET))
+            self.assertEqual(std_out_lines[1], ETC_OUTPUT_RESET_COLOR)
+            self.assertEqual(std_out_lines[2], ETC_OUTPUT_RESET_COLOR)
+            self.assertEqual(std_out_lines[3], ETC_OUTPUT_RESET_COLOR)
+            self.assertEqual(std_out_lines[4], '{0}EXPECTED:{1}'.format(ETC_OUTPUT_EXPECTED_MATCH_COLOR, ETC_OUTPUT_RESET_COLOR))
             self.assertEqual(
                 std_out_lines[5],
                 '{0}AB{1}c{2}'.format(
-                    OUTPUT_EXPECTED_MATCH,
-                    OUTPUT_EXPECTED_ERROR,
-                    OUTPUT_RESET,
+                    ETC_OUTPUT_EXPECTED_MATCH_COLOR,
+                    ETC_OUTPUT_EXPECTED_ERROR_COLOR,
+                    ETC_OUTPUT_RESET_COLOR,
                 ),
             )
-            self.assertEqual(std_out_lines[6], OUTPUT_RESET)
-            self.assertEqual(std_out_lines[7], OUTPUT_RESET)
-            self.assertEqual(std_out_lines[8], '{0}ACTUAL:{1}'.format(OUTPUT_ACTUALS_MATCH, OUTPUT_RESET))
+            self.assertEqual(std_out_lines[6], ETC_OUTPUT_RESET_COLOR)
+            self.assertEqual(std_out_lines[7], ETC_OUTPUT_RESET_COLOR)
+            self.assertEqual(std_out_lines[8], '{0}ACTUAL:{1}'.format(ETC_OUTPUT_ACTUALS_MATCH_COLOR, ETC_OUTPUT_RESET_COLOR))
             self.assertEqual(
                 std_out_lines[9],
                 '{0}AB{1}C{2}'.format(
-                    OUTPUT_ACTUALS_MATCH,
-                    OUTPUT_ACTUALS_ERROR,
-                    OUTPUT_RESET,
+                    ETC_OUTPUT_ACTUALS_MATCH_COLOR,
+                    ETC_OUTPUT_ACTUALS_ERROR_COLOR,
+                    ETC_OUTPUT_RESET_COLOR,
                 ),
             )
-            self.assertEqual(std_out_lines[10], OUTPUT_RESET)
-            self.assertEqual(std_out_lines[11], OUTPUT_RESET)
+            self.assertEqual(std_out_lines[10], ETC_OUTPUT_RESET_COLOR)
+            self.assertEqual(std_out_lines[11], ETC_OUTPUT_RESET_COLOR)
             self.assertEqual(std_out_lines[12], '')
 
         with self.subTest('With wrong characters at end - Larger str'):
             std_out = StringIO()
             with redirect_stdout(std_out):
                 with self.assertRaises(AssertionError):
                     self.assertText('This is a test VALUE!', 'This is a test value.')
             std_out_lines = std_out.getvalue().split('\n')[5:]
 
             # Test all line values.
             self.assertEqual(std_out_lines[0], '')
-            self.assertEqual(std_out_lines[1], OUTPUT_RESET)
-            self.assertEqual(std_out_lines[2], OUTPUT_RESET)
-            self.assertEqual(std_out_lines[3], OUTPUT_RESET)
-            self.assertEqual(std_out_lines[4], '{0}EXPECTED:{1}'.format(OUTPUT_EXPECTED_MATCH, OUTPUT_RESET))
+            self.assertEqual(std_out_lines[1], ETC_OUTPUT_RESET_COLOR)
+            self.assertEqual(std_out_lines[2], ETC_OUTPUT_RESET_COLOR)
+            self.assertEqual(std_out_lines[3], ETC_OUTPUT_RESET_COLOR)
+            self.assertEqual(std_out_lines[4], '{0}EXPECTED:{1}'.format(ETC_OUTPUT_EXPECTED_MATCH_COLOR, ETC_OUTPUT_RESET_COLOR))
             self.assertEqual(
                 std_out_lines[5],
                 '{0}This is a test {1}VALUE!{2}'.format(
-                    OUTPUT_EXPECTED_MATCH,
-                    OUTPUT_EXPECTED_ERROR,
-                    OUTPUT_RESET,
+                    ETC_OUTPUT_EXPECTED_MATCH_COLOR,
+                    ETC_OUTPUT_EXPECTED_ERROR_COLOR,
+                    ETC_OUTPUT_RESET_COLOR,
                 ),
             )
-            self.assertEqual(std_out_lines[6], OUTPUT_RESET)
-            self.assertEqual(std_out_lines[7], OUTPUT_RESET)
-            self.assertEqual(std_out_lines[8], '{0}ACTUAL:{1}'.format(OUTPUT_ACTUALS_MATCH, OUTPUT_RESET))
+            self.assertEqual(std_out_lines[6], ETC_OUTPUT_RESET_COLOR)
+            self.assertEqual(std_out_lines[7], ETC_OUTPUT_RESET_COLOR)
+            self.assertEqual(std_out_lines[8], '{0}ACTUAL:{1}'.format(ETC_OUTPUT_ACTUALS_MATCH_COLOR, ETC_OUTPUT_RESET_COLOR))
             self.assertEqual(
                 std_out_lines[9],
                 '{0}This is a test {1}value.{2}'.format(
-                    OUTPUT_ACTUALS_MATCH,
-                    OUTPUT_ACTUALS_ERROR,
-                    OUTPUT_RESET,
+                    ETC_OUTPUT_ACTUALS_MATCH_COLOR,
+                    ETC_OUTPUT_ACTUALS_ERROR_COLOR,
+                    ETC_OUTPUT_RESET_COLOR,
                 ),
             )
-            self.assertEqual(std_out_lines[10], OUTPUT_RESET)
-            self.assertEqual(std_out_lines[11], OUTPUT_RESET)
+            self.assertEqual(std_out_lines[10], ETC_OUTPUT_RESET_COLOR)
+            self.assertEqual(std_out_lines[11], ETC_OUTPUT_RESET_COLOR)
             self.assertEqual(std_out_lines[12], '')
 
     # endregion Assertion Tests
 
     # region User Management Function Tests
 
     def test__get_user__with_project_defaults(self):
```

### Comparing `django-expanded-test-cases-0.3.0/tests/test_cases/test_integration_case.py` & `django-expanded-test-cases-0.4.0/tests/test_cases/test_integration_case.py`

 * *Files 0% similar despite different names*

```diff
@@ -13,15 +13,15 @@
 from django.core.exceptions import ValidationError
 from django.http import HttpResponse
 
 # Internal Imports.
 from django_expanded_test_cases import IntegrationTestCase
 
 
-class IntegrationClassTest__Base():
+class IntegrationClassTest__Base(IntegrationTestCase):
     """Tests for IntegrationTestCase class."""
 
     # region Assertion Tests
 
     # region Response Assertion Tests
 
     def test__assertResponse__url(self):
@@ -1180,108 +1180,104 @@
                     'Pretend this',
                     'project landing',
                 ),
                 ignore_ordering=True,  # Ignore because we recheck the same values.
             )
 
         with self.subTest('Standard Response - Set of items on user page - As list'):
-            response = self._get_page_response('django_expanded_test_cases:user-detail', args=(1,))
+            response = self._get_page_response('django_expanded_test_cases:user-detail', args=(1,), user=self.test_user)
 
             # Standard, ordered page match.
             self.assertPageContent(
                 response,
                 [
                     '<h1>User Detail Page Header</h1>',
                     'Username: "test_superuser"',
-                    'First Name: "TestFirst"',
-                    'Last Name: "TestLast"',
+                    'First Name: "SuperUserFirst"',
+                    'Last Name: "SuperUserLast"',
                     'Is Active: "True"',
                     'Is SuperUser: "True"',
                     'Is Staff: "False"',
                 ],
             )
 
             # With repeating values.
             self.assertPageContent(
                 response,
                 [
                     '<h1>User Detail Page Header</h1>',
                     'User Detail',
                     'Username: "test_superuser"',
-                    'First Name: "TestFirst"',
-                    'Last Name: "TestLast"',
+                    'First Name: "SuperUserFirst"',
+                    'Last Name: "SuperUserLast"',
                     'Is Active: "True"',
                     'Is SuperUser: "True"',
                     'Is Staff: "False"',
-                    'TestFirst',
-                    'TestLast',
                 ],
                 ignore_ordering=True,  # Ignore because we recheck the same values.
             )
 
             # Standard page match but values are unordered.
             self.assertPageContent(
                 response,
                 [
                     'Is Active: "True"',
                     'Is SuperUser: "True"',
                     'Is Staff: "False"',
                     'Username: "test_superuser"',
-                    'First Name: "TestFirst"',
-                    'Last Name: "TestLast"',
+                    'First Name: "SuperUserFirst"',
+                    'Last Name: "SuperUserLast"',
                     '<h1>User Detail Page Header</h1>',
                 ],
                 ignore_ordering=True,  # Ignore because unordered.
             )
 
         with self.subTest('Standard Response - Set of items on user page - As Tuple'):
-            response = self._get_page_response('django_expanded_test_cases:user-detail', args=(1,))
+            response = self._get_page_response('django_expanded_test_cases:user-detail', args=(1,), user=self.test_user)
 
             # Standard, ordered page match.
             self.assertPageContent(
                 response,
                 (
                     '<h1>User Detail Page Header</h1>',
                     'Username: "test_superuser"',
-                    'First Name: "TestFirst"',
-                    'Last Name: "TestLast"',
+                    'First Name: "SuperUserFirst"',
+                    'Last Name: "SuperUserLast"',
                     'Is Active: "True"',
                     'Is SuperUser: "True"',
                     'Is Staff: "False"',
                 ),
             )
 
             # With repeating values.
             self.assertPageContent(
                 response,
                 (
                     '<h1>User Detail Page Header</h1>',
                     'User Detail',
                     'Username: "test_superuser"',
-                    'First Name: "TestFirst"',
-                    'Last Name: "TestLast"',
+                    'First Name: "SuperUserFirst"',
+                    'Last Name: "SuperUserLast"',
                     'Is Active: "True"',
                     'Is SuperUser: "True"',
                     'Is Staff: "False"',
-                    'TestFirst',
-                    'TestLast',
                 ),
                 ignore_ordering=True,  # Ignore because we recheck the same values.
             )
 
             # Standard page match but values are unordered.
             self.assertPageContent(
                 response,
                 (
                     'Is Active: "True"',
                     'Is SuperUser: "True"',
                     'Is Staff: "False"',
                     'Username: "test_superuser"',
-                    'First Name: "TestFirst"',
-                    'Last Name: "TestLast"',
+                    'First Name: "SuperUserFirst"',
+                    'Last Name: "SuperUserLast"',
                     '<h1>User Detail Page Header</h1>',
                 ),
                 ignore_ordering=True,  # Ignore because unordered.
             )
 
         with self.subTest('Standard Response - Checking repeated values on page'):
             """
@@ -1517,104 +1513,104 @@
             response = self._get_page_response('django_expanded_test_cases:user-detail', args=(1,))
 
             with self.assertRaises(AssertionError) as err:
                 # Test "first name" string at top.
                 self.assertPageContent(
                     response,
                     [
-                        'First Name: "TestFirst"',
+                        'First Name: "SuperUserFirst"',
                         '<h1>User Detail Page Header</h1>',
                         'Username: "test_superuser"',
-                        'Last Name: "TestLast"',
+                        'Last Name: "SuperUserLast"',
                         'Is Active: "True"',
                         'Is SuperUser: "True"',
                         'Is Staff: "False"',
                     ],
                 )
             self.assertEqual(str(err.exception), exception_msg_bad_order.format('<h1>User Detail Page Header</h1>'))
 
             with self.assertRaises(AssertionError) as err:
                 # Test "first name" string after header.
                 self.assertPageContent(
                     response,
                     [
                         '<h1>User Detail Page Header</h1>',
-                        'First Name: "TestFirst"',
+                        'First Name: "SuperUserFirst"',
                         'Username: "test_superuser"',
-                        'Last Name: "TestLast"',
+                        'Last Name: "SuperUserLast"',
                         'Is Active: "True"',
                         'Is SuperUser: "True"',
                         'Is Staff: "False"',
                     ],
                 )
             self.assertEqual(str(err.exception), exception_msg_bad_order.format('Username: "test_superuser"'))
 
             with self.assertRaises(AssertionError) as err:
                 # Test "first name" string after last name.
                 self.assertPageContent(
                     response,
                     [
                         '<h1>User Detail Page Header</h1>',
                         'Username: "test_superuser"',
-                        'Last Name: "TestLast"',
-                        'First Name: "TestFirst"',
+                        'Last Name: "SuperUserLast"',
+                        'First Name: "SuperUserFirst"',
                         'Is Active: "True"',
                         'Is SuperUser: "True"',
                         'Is Staff: "False"',
                     ],
                 )
-            self.assertEqual(str(err.exception), exception_msg_bad_order.format('First Name: "TestFirst"'))
+            self.assertEqual(str(err.exception), exception_msg_bad_order.format('First Name: "SuperUserFirst"'))
 
             with self.assertRaises(AssertionError) as err:
                 # Test "first name" string after active.
                 self.assertPageContent(
                     response,
                     [
                         '<h1>User Detail Page Header</h1>',
                         'Username: "test_superuser"',
-                        'Last Name: "TestLast"',
+                        'Last Name: "SuperUserLast"',
                         'Is Active: "True"',
-                        'First Name: "TestFirst"',
+                        'First Name: "SuperUserFirst"',
                         'Is SuperUser: "True"',
                         'Is Staff: "False"',
                     ],
                 )
-            self.assertEqual(str(err.exception), exception_msg_bad_order.format('First Name: "TestFirst"'))
+            self.assertEqual(str(err.exception), exception_msg_bad_order.format('First Name: "SuperUserFirst"'))
 
             with self.assertRaises(AssertionError) as err:
                 # Test "first name" string after superuser.
                 self.assertPageContent(
                     response,
                     [
                         '<h1>User Detail Page Header</h1>',
                         'Username: "test_superuser"',
-                        'Last Name: "TestLast"',
+                        'Last Name: "SuperUserLast"',
                         'Is Active: "True"',
                         'Is SuperUser: "True"',
-                        'First Name: "TestFirst"',
+                        'First Name: "SuperUserFirst"',
                         'Is Staff: "False"',
                     ],
                 )
-            self.assertEqual(str(err.exception), exception_msg_bad_order.format('First Name: "TestFirst"'))
+            self.assertEqual(str(err.exception), exception_msg_bad_order.format('First Name: "SuperUserFirst"'))
 
             with self.assertRaises(AssertionError) as err:
                 # Test "first name" string after staff.
                 self.assertPageContent(
                     response,
                     [
                         '<h1>User Detail Page Header</h1>',
                         'Username: "test_superuser"',
-                        'Last Name: "TestLast"',
+                        'Last Name: "SuperUserLast"',
                         'Is Active: "True"',
                         'Is SuperUser: "True"',
                         'Is Staff: "False"',
-                        'First Name: "TestFirst"',
+                        'First Name: "SuperUserFirst"',
                     ],
                 )
-            self.assertEqual(str(err.exception), exception_msg_bad_order.format('First Name: "TestFirst"'))
+            self.assertEqual(str(err.exception), exception_msg_bad_order.format('First Name: "SuperUserFirst"'))
 
     def test__assertPageContent__failure__with_bad_search_space(self):
         exception_msg = 'Could not find "{0}" value in content response. Provided value was:\n{1}'
         response = self._get_page_response('django_expanded_test_cases:index')
 
         # Bad content_starts_after values.
         with self.subTest('With content_starts_after not found'):
```

### Comparing `django-expanded-test-cases-0.3.0/tests/test_cases/test_live_server_case.py` & `django-expanded-test-cases-0.4.0/tests/test_cases/test_live_server_case.py`

 * *Files identical despite different names*

### Comparing `django-expanded-test-cases-0.3.0/tests/views.py` & `django-expanded-test-cases-0.4.0/tests/views.py`

 * *Files identical despite different names*

