# Comparing `tmp/cron-validator-1.0.6.tar.gz` & `tmp/cron-validator-1.0.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "cron-validator-1.0.6.tar", last modified: Mon Apr  4 02:40:52 2022, max compression
+gzip compressed data, was "cron-validator-1.0.7.tar", last modified: Mon Jun 12 16:54:07 2023, max compression
```

## Comparing `cron-validator-1.0.6.tar` & `cron-validator-1.0.7.tar`

### file list

```diff
@@ -1,24 +1,24 @@
-drwxr-xr-x   0 baodoan    (503) staff       (20)        0 2022-04-04 02:40:52.291208 cron-validator-1.0.6/
--rw-r--r--   0 baodoan    (503) staff       (20)     1068 2021-10-24 03:55:01.000000 cron-validator-1.0.6/LICENSE.txt
--rw-r--r--   0 baodoan    (503) staff       (20)     4047 2022-04-04 02:40:52.291323 cron-validator-1.0.6/PKG-INFO
--rw-r--r--   0 baodoan    (503) staff       (20)     3573 2022-04-04 02:40:10.000000 cron-validator-1.0.6/README.md
-drwxr-xr-x   0 baodoan    (503) staff       (20)        0 2022-04-04 02:40:52.285429 cron-validator-1.0.6/cron_validator/
--rw-r--r--   0 baodoan    (503) staff       (20)      103 2022-04-04 02:37:41.000000 cron-validator-1.0.6/cron_validator/__init__.py
--rw-r--r--   0 baodoan    (503) staff       (20)     9180 2022-04-04 02:37:41.000000 cron-validator-1.0.6/cron_validator/regexes.py
--rw-r--r--   0 baodoan    (503) staff       (20)      799 2022-02-22 01:59:03.000000 cron-validator-1.0.6/cron_validator/scheduler.py
--rw-r--r--   0 baodoan    (503) staff       (20)      720 2022-02-22 01:59:03.000000 cron-validator-1.0.6/cron_validator/util.py
--rw-r--r--   0 baodoan    (503) staff       (20)     2151 2022-04-04 02:37:41.000000 cron-validator-1.0.6/cron_validator/validator.py
-drwxr-xr-x   0 baodoan    (503) staff       (20)        0 2022-04-04 02:40:52.287571 cron-validator-1.0.6/cron_validator.egg-info/
--rw-r--r--   0 baodoan    (503) staff       (20)     4047 2022-04-04 02:40:52.000000 cron-validator-1.0.6/cron_validator.egg-info/PKG-INFO
--rw-r--r--   0 baodoan    (503) staff       (20)      478 2022-04-04 02:40:52.000000 cron-validator-1.0.6/cron_validator.egg-info/SOURCES.txt
--rw-r--r--   0 baodoan    (503) staff       (20)        1 2022-04-04 02:40:52.000000 cron-validator-1.0.6/cron_validator.egg-info/dependency_links.txt
--rw-r--r--   0 baodoan    (503) staff       (20)       21 2022-04-04 02:40:52.000000 cron-validator-1.0.6/cron_validator.egg-info/requires.txt
--rw-r--r--   0 baodoan    (503) staff       (20)       15 2022-04-04 02:40:52.000000 cron-validator-1.0.6/cron_validator.egg-info/top_level.txt
--rw-r--r--   0 baodoan    (503) staff       (20)       79 2022-04-04 02:40:52.291976 cron-validator-1.0.6/setup.cfg
--rw-r--r--   0 baodoan    (503) staff       (20)      864 2022-04-04 02:37:55.000000 cron-validator-1.0.6/setup.py
-drwxr-xr-x   0 baodoan    (503) staff       (20)        0 2022-04-04 02:40:52.290717 cron-validator-1.0.6/test/
--rw-r--r--   0 baodoan    (503) staff       (20)     3875 2022-02-22 01:59:03.000000 cron-validator-1.0.6/test/test_CronScheduler.py
--rw-r--r--   0 baodoan    (503) staff       (20)     6319 2022-02-22 01:59:03.000000 cron-validator-1.0.6/test/test_execution_time.py
--rw-r--r--   0 baodoan    (503) staff       (20)     4537 2022-04-04 02:37:41.000000 cron-validator-1.0.6/test/test_match.py
--rw-r--r--   0 baodoan    (503) staff       (20)      992 2022-02-22 01:59:03.000000 cron-validator-1.0.6/test/test_util.py
--rw-r--r--   0 baodoan    (503) staff       (20)     4020 2022-02-22 01:59:03.000000 cron-validator-1.0.6/test/test_valid_regex.py
+drwxr-xr-x   0 baodoan    (503) staff       (20)        0 2023-06-12 16:54:07.949175 cron-validator-1.0.7/
+-rw-r--r--   0 baodoan    (503) staff       (20)     1068 2021-10-24 03:55:01.000000 cron-validator-1.0.7/LICENSE.txt
+-rw-r--r--   0 baodoan    (503) staff       (20)     4047 2023-06-12 16:54:07.949437 cron-validator-1.0.7/PKG-INFO
+-rw-r--r--   0 baodoan    (503) staff       (20)     3573 2022-04-04 02:40:10.000000 cron-validator-1.0.7/README.md
+drwxr-xr-x   0 baodoan    (503) staff       (20)        0 2023-06-12 16:54:07.942344 cron-validator-1.0.7/cron_validator/
+-rw-r--r--   0 baodoan    (503) staff       (20)      103 2022-04-04 02:37:41.000000 cron-validator-1.0.7/cron_validator/__init__.py
+-rw-r--r--   0 baodoan    (503) staff       (20)     9180 2022-04-04 02:37:41.000000 cron-validator-1.0.7/cron_validator/regexes.py
+-rw-r--r--   0 baodoan    (503) staff       (20)      799 2022-02-22 01:59:03.000000 cron-validator-1.0.7/cron_validator/scheduler.py
+-rw-r--r--   0 baodoan    (503) staff       (20)     1537 2023-06-12 16:48:02.000000 cron-validator-1.0.7/cron_validator/util.py
+-rw-r--r--   0 baodoan    (503) staff       (20)     2213 2023-06-12 16:48:02.000000 cron-validator-1.0.7/cron_validator/validator.py
+drwxr-xr-x   0 baodoan    (503) staff       (20)        0 2023-06-12 16:54:07.944826 cron-validator-1.0.7/cron_validator.egg-info/
+-rw-r--r--   0 baodoan    (503) staff       (20)     4047 2023-06-12 16:54:07.000000 cron-validator-1.0.7/cron_validator.egg-info/PKG-INFO
+-rw-r--r--   0 baodoan    (503) staff       (20)      478 2023-06-12 16:54:07.000000 cron-validator-1.0.7/cron_validator.egg-info/SOURCES.txt
+-rw-r--r--   0 baodoan    (503) staff       (20)        1 2023-06-12 16:54:07.000000 cron-validator-1.0.7/cron_validator.egg-info/dependency_links.txt
+-rw-r--r--   0 baodoan    (503) staff       (20)       21 2023-06-12 16:54:07.000000 cron-validator-1.0.7/cron_validator.egg-info/requires.txt
+-rw-r--r--   0 baodoan    (503) staff       (20)       15 2023-06-12 16:54:07.000000 cron-validator-1.0.7/cron_validator.egg-info/top_level.txt
+-rw-r--r--   0 baodoan    (503) staff       (20)       79 2023-06-12 16:54:07.950207 cron-validator-1.0.7/setup.cfg
+-rw-r--r--   0 baodoan    (503) staff       (20)      864 2023-06-12 16:49:49.000000 cron-validator-1.0.7/setup.py
+drwxr-xr-x   0 baodoan    (503) staff       (20)        0 2023-06-12 16:54:07.948469 cron-validator-1.0.7/test/
+-rw-r--r--   0 baodoan    (503) staff       (20)     3875 2022-02-22 01:59:03.000000 cron-validator-1.0.7/test/test_CronScheduler.py
+-rw-r--r--   0 baodoan    (503) staff       (20)     6319 2022-02-22 01:59:03.000000 cron-validator-1.0.7/test/test_execution_time.py
+-rw-r--r--   0 baodoan    (503) staff       (20)     4537 2022-04-04 02:37:41.000000 cron-validator-1.0.7/test/test_match.py
+-rw-r--r--   0 baodoan    (503) staff       (20)     1458 2023-06-12 16:48:02.000000 cron-validator-1.0.7/test/test_util.py
+-rw-r--r--   0 baodoan    (503) staff       (20)     5128 2023-06-12 16:48:02.000000 cron-validator-1.0.7/test/test_valid_regex.py
```

### Comparing `cron-validator-1.0.6/LICENSE.txt` & `cron-validator-1.0.7/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `cron-validator-1.0.6/PKG-INFO` & `cron-validator-1.0.7/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,16 +1,16 @@
 Metadata-Version: 2.1
 Name: cron-validator
-Version: 1.0.6
+Version: 1.0.7
 Summary: Unix cron implementation by Python
 Home-page: https://github.com/vcoder4c/cron-validator
 Author: vcoder
 Author-email: doanngocbao@gmail.com
 License: MIT
-Download-URL: https://github.com/vcoder4c/cron-validator/archive/v1.0.6.tar.gz
+Download-URL: https://github.com/vcoder4c/cron-validator/archive/v1.0.7.tar.gz
 Keywords: cron,python,cron expression validator,cron expression iterator,cron scheduler
 Platform: UNKNOWN
 Description-Content-Type: text/markdown
 License-File: LICENSE.txt
 
 # Cron Validator
```

### Comparing `cron-validator-1.0.6/README.md` & `cron-validator-1.0.7/README.md`

 * *Files identical despite different names*

### Comparing `cron-validator-1.0.6/cron_validator/regexes.py` & `cron-validator-1.0.7/cron_validator/regexes.py`

 * *Files identical despite different names*

### Comparing `cron-validator-1.0.6/cron_validator/scheduler.py` & `cron-validator-1.0.7/cron_validator/scheduler.py`

 * *Files identical despite different names*

### Comparing `cron-validator-1.0.6/cron_validator/validator.py` & `cron-validator-1.0.7/cron_validator/validator.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,21 +1,22 @@
 from dateutil import rrule
 
 from .regexes import ElementPart, Version, element_kind_map, regex_dict
-from .util import ts_to_datetime
+from .util import replace_names, ts_to_datetime
 
 
 class CronValidator:
     @classmethod
     def parse(cls, expression, version=Version.UNIX):
         """
 
         :param str expression:
         :return:
         """
+        expression = replace_names(expression)
         parts = expression.split(" ")
         if len(parts) != 5:
             raise ValueError("Invalid expression")
         elements = []
         for i in range(0, 5):
             m = regex_dict[version][i].fullmatch(parts[i])
             if not m:
```

### Comparing `cron-validator-1.0.6/cron_validator.egg-info/PKG-INFO` & `cron-validator-1.0.7/cron_validator.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,16 +1,16 @@
 Metadata-Version: 2.1
 Name: cron-validator
-Version: 1.0.6
+Version: 1.0.7
 Summary: Unix cron implementation by Python
 Home-page: https://github.com/vcoder4c/cron-validator
 Author: vcoder
 Author-email: doanngocbao@gmail.com
 License: MIT
-Download-URL: https://github.com/vcoder4c/cron-validator/archive/v1.0.6.tar.gz
+Download-URL: https://github.com/vcoder4c/cron-validator/archive/v1.0.7.tar.gz
 Keywords: cron,python,cron expression validator,cron expression iterator,cron scheduler
 Platform: UNKNOWN
 Description-Content-Type: text/markdown
 License-File: LICENSE.txt
 
 # Cron Validator
```

### Comparing `cron-validator-1.0.6/setup.py` & `cron-validator-1.0.7/setup.py`

 * *Files 14% similar despite different names*

```diff
@@ -8,19 +8,19 @@
 else:
     with open("README.md", encoding="utf-8") as f:
         long_description = f.read()
 
 setup(
     name="cron-validator",
     packages=["cron_validator"],
-    version="1.0.6",
+    version="1.0.7",
     license="MIT",
     description="Unix cron implementation by Python",
     long_description=long_description,
     long_description_content_type="text/markdown",
     author="vcoder",
     author_email="doanngocbao@gmail.com",
     url="https://github.com/vcoder4c/cron-validator",
     keywords=["cron", "python", "cron expression validator", "cron expression iterator", "cron scheduler"],
-    download_url="https://github.com/vcoder4c/cron-validator/archive/v1.0.6.tar.gz",
+    download_url="https://github.com/vcoder4c/cron-validator/archive/v1.0.7.tar.gz",
     install_requires=["python_dateutil", "pytz"],
 )
```

### Comparing `cron-validator-1.0.6/test/test_CronScheduler.py` & `cron-validator-1.0.7/test/test_CronScheduler.py`

 * *Files identical despite different names*

### Comparing `cron-validator-1.0.6/test/test_execution_time.py` & `cron-validator-1.0.7/test/test_execution_time.py`

 * *Files identical despite different names*

### Comparing `cron-validator-1.0.6/test/test_match.py` & `cron-validator-1.0.7/test/test_match.py`

 * *Files identical despite different names*

### Comparing `cron-validator-1.0.6/test/test_valid_regex.py` & `cron-validator-1.0.7/test/test_valid_regex.py`

 * *Files 12% similar despite different names*

```diff
@@ -103,7 +103,36 @@
     assert_validate_fail("* * * * 1,7")
     assert_validate_fail("* * * * 1/0")
     assert_validate_successfully("* * * * 1/1")
     assert_validate_successfully("* * * * */1")
     assert_validate_successfully("* * * * */6")
     assert_validate_fail("* * * * */0")
     assert_validate_fail("* * * * */7")
+
+
+def test_validator_month_names():
+    assert_validate_successfully("* * * jan *")
+    assert_validate_successfully("* * * FEB,mar,Apr *")
+    assert_validate_successfully("* * * MAY-JUL *")
+    assert_validate_successfully("* * * jun-Aug *")
+    assert_validate_successfully("* * * Sep,Oct *")
+    assert_validate_successfully("* * * dec/3 *")
+    assert_validate_fail("* * * January *")
+    assert_validate_fail("* * * jan1 *")
+    assert_validate_fail("* * * 1jan *")
+    assert_validate_fail("* * * 2/feb *")
+    assert_validate_fail("* * * */feb *")
+    assert_validate_fail("* * * NOV/0 *")
+
+
+def test_validator_day_of_week_names():
+    assert_validate_successfully("* * * * sun")
+    assert_validate_successfully("* * * * mon,TUE,Wed")
+    assert_validate_successfully("* * * * FRI-SAT")
+    assert_validate_successfully("* * * * wed/2")
+    assert_validate_fail("* * * * Sunday")
+    assert_validate_fail("* * * * sun,mon-fri")
+    assert_validate_fail("* * * * tue/0")
+    assert_validate_fail("* * * * */mon")
+    assert_validate_fail("* * * * 1/wed")
+    assert_validate_fail("* * * * mon/mon")
+
```

