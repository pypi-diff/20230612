# Comparing `tmp/smartbetsAPI-1.1.1.tar.gz` & `tmp/smartbetsAPI-1.1.3.linux-aarch64.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "smartbetsAPI-1.1.1.tar", last modified: Wed Apr 26 13:33:06 2023, max compression
+gzip compressed data, was "smartbetsAPI-1.1.3.linux-aarch64.tar", last modified: Mon Jun 12 19:50:42 2023, max compression
```

## Comparing `smartbetsAPI-1.1.1.tar` & `smartbetsAPI-1.1.3.linux-aarch64.tar`

### file list

```diff
@@ -1,27 +1,46 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-26 13:33:06.183328 smartbetsAPI-1.1.1/
--rw-r--r--   0 root         (0) root         (0)    35149 2023-02-06 18:42:43.000000 smartbetsAPI-1.1.1/LICENSE
--rw-r--r--   0 root         (0) root         (0)    10984 2023-04-26 13:33:06.183328 smartbetsAPI-1.1.1/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     9441 2023-04-26 13:12:46.000000 smartbetsAPI-1.1.1/README.md
--rw-r--r--   0 root         (0) root         (0)       38 2023-04-26 13:33:06.183328 smartbetsAPI-1.1.1/setup.cfg
--rw-r--r--   0 root         (0) root         (0)     1951 2023-04-26 13:31:03.000000 smartbetsAPI-1.1.1/setup.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-26 13:33:06.179994 smartbetsAPI-1.1.1/smartbetsAPI.egg-info/
--rw-r--r--   0 root         (0) root         (0)    10984 2023-04-26 13:33:06.000000 smartbetsAPI-1.1.1/smartbetsAPI.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      624 2023-04-26 13:33:06.000000 smartbetsAPI-1.1.1/smartbetsAPI.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-04-26 13:33:06.000000 smartbetsAPI-1.1.1/smartbetsAPI.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)       70 2023-04-26 13:33:06.000000 smartbetsAPI-1.1.1/smartbetsAPI.egg-info/entry_points.txt
--rw-r--r--   0 root         (0) root         (0)       86 2023-04-26 13:33:06.000000 smartbetsAPI-1.1.1/smartbetsAPI.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)       14 2023-04-26 13:33:06.000000 smartbetsAPI-1.1.1/smartbetsAPI.egg-info/top_level.txt
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-26 13:33:06.183328 smartbetsAPI-1.1.1/smartbets_API/
--rw-r--r--   0 root         (0) root         (0)      126 2023-04-26 12:51:40.000000 smartbetsAPI-1.1.1/smartbets_API/__init__.py
--rw-r--r--   0 root         (0) root         (0)       50 2023-04-26 12:26:14.000000 smartbetsAPI-1.1.1/smartbets_API/__main__.py
--rw-r--r--   0 root         (0) root         (0)     2050 2023-02-06 18:42:43.000000 smartbetsAPI-1.1.1/smartbets_API/bet_analyzer.py
--rw-r--r--   0 root         (0) root         (0)     3652 2023-04-26 12:39:32.000000 smartbetsAPI-1.1.1/smartbets_API/bet_at_api_level.py
--rw-r--r--   0 root         (0) root         (0)    11304 2023-03-31 20:51:37.000000 smartbetsAPI-1.1.1/smartbets_API/bet_common.py
--rw-r--r--   0 root         (0) root         (0)     4144 2023-03-31 20:48:34.000000 smartbetsAPI-1.1.1/smartbets_API/configuration_handler.py
--rw-r--r--   0 root         (0) root         (0)     6613 2023-02-06 18:42:43.000000 smartbetsAPI-1.1.1/smartbets_API/figure_harvester.py
--rw-r--r--   0 root         (0) root         (0)     3065 2023-02-06 18:42:43.000000 smartbetsAPI-1.1.1/smartbets_API/googler.py
--rw-r--r--   0 root         (0) root         (0)     6379 2023-03-31 20:20:15.000000 smartbetsAPI-1.1.1/smartbets_API/html_fetcher.py
--rw-r--r--   0 root         (0) root         (0)     6611 2023-03-31 20:17:33.000000 smartbetsAPI-1.1.1/smartbets_API/interface.py
--rw-r--r--   0 root         (0) root         (0)     8775 2023-02-06 18:42:43.000000 smartbetsAPI-1.1.1/smartbets_API/predictor.py
--rw-r--r--   0 root         (0) root         (0)     1728 2023-03-26 16:28:20.000000 smartbetsAPI-1.1.1/smartbets_API/proxyh.py
--rw-r--r--   0 root         (0) root         (0)     2201 2023-03-12 10:54:19.000000 smartbetsAPI-1.1.1/smartbets_API/tertiary_bet.py
+drwxrwx---   0 root         (0) everybody  (9997)        0 2023-06-12 19:50:38.693000 ./
+drwxrwx---   0 root         (0) everybody  (9997)        0 2023-06-12 19:50:38.697000 ./data/
+drwxrwx---   0 root         (0) everybody  (9997)        0 2023-06-12 19:50:38.701000 ./data/data/
+drwxrwx---   0 root         (0) everybody  (9997)        0 2023-06-12 19:50:38.701000 ./data/data/com.termux/
+drwxrwx---   0 root         (0) everybody  (9997)        0 2023-06-12 19:50:38.705000 ./data/data/com.termux/files/
+drwxrwx---   0 root         (0) everybody  (9997)        0 2023-06-12 19:50:42.673000 ./data/data/com.termux/files/usr/
+drwxrwx---   0 root         (0) everybody  (9997)        0 2023-06-12 19:50:42.745000 ./data/data/com.termux/files/usr/bin/
+-rw-rw----   0 root         (0) everybody  (9997)     1009 2023-06-12 19:50:42.749000 ./data/data/com.termux/files/usr/bin/smartbetsAPI
+drwxrwx---   0 root         (0) everybody  (9997)        0 2023-06-12 19:50:38.713000 ./data/data/com.termux/files/usr/lib/
+drwxrwx---   0 root         (0) everybody  (9997)        0 2023-06-12 19:50:38.713000 ./data/data/com.termux/files/usr/lib/python3.11/
+drwxrwx---   0 root         (0) everybody  (9997)        0 2023-06-12 19:50:40.929000 ./data/data/com.termux/files/usr/lib/python3.11/site-packages/
+drwxrwx---   0 root         (0) everybody  (9997)        0 2023-06-12 19:50:41.141000 ./data/data/com.termux/files/usr/lib/python3.11/site-packages/smartbetsAPI-1.1.3-py3.11.egg-info/
+-rw-rw----   0 root         (0) everybody  (9997)    10984 2023-06-12 19:50:40.717000 ./data/data/com.termux/files/usr/lib/python3.11/site-packages/smartbetsAPI-1.1.3-py3.11.egg-info/PKG-INFO
+-rw-rw----   0 root         (0) everybody  (9997)      624 2023-06-12 19:50:40.917000 ./data/data/com.termux/files/usr/lib/python3.11/site-packages/smartbetsAPI-1.1.3-py3.11.egg-info/SOURCES.txt
+-rw-rw----   0 root         (0) everybody  (9997)        1 2023-06-12 19:50:40.725000 ./data/data/com.termux/files/usr/lib/python3.11/site-packages/smartbetsAPI-1.1.3-py3.11.egg-info/dependency_links.txt
+-rw-rw----   0 root         (0) everybody  (9997)       70 2023-06-12 19:50:40.733000 ./data/data/com.termux/files/usr/lib/python3.11/site-packages/smartbetsAPI-1.1.3-py3.11.egg-info/entry_points.txt
+-rw-rw----   0 root         (0) everybody  (9997)       86 2023-06-12 19:50:40.737000 ./data/data/com.termux/files/usr/lib/python3.11/site-packages/smartbetsAPI-1.1.3-py3.11.egg-info/requires.txt
+-rw-rw----   0 root         (0) everybody  (9997)       14 2023-06-12 19:50:40.741000 ./data/data/com.termux/files/usr/lib/python3.11/site-packages/smartbetsAPI-1.1.3-py3.11.egg-info/top_level.txt
+drwxrwx---   0 root         (0) everybody  (9997)        0 2023-06-12 19:50:39.253000 ./data/data/com.termux/files/usr/lib/python3.11/site-packages/smartbets_API/
+-rw-rw----   0 root         (0) everybody  (9997)      181 2023-06-12 16:08:11.000000 ./data/data/com.termux/files/usr/lib/python3.11/site-packages/smartbets_API/__init__.py
+-rw-rw----   0 root         (0) everybody  (9997)       50 2023-06-12 15:32:20.000000 ./data/data/com.termux/files/usr/lib/python3.11/site-packages/smartbets_API/__main__.py
+drwxrwx---   0 root         (0) everybody  (9997)        0 2023-06-12 19:50:40.225000 ./data/data/com.termux/files/usr/lib/python3.11/site-packages/smartbets_API/__pycache__/
+-rw-rw----   0 root         (0) everybody  (9997)      404 2023-06-12 19:50:39.389000 ./data/data/com.termux/files/usr/lib/python3.11/site-packages/smartbets_API/__pycache__/__init__.cpython-311.pyc
+-rw-rw----   0 root         (0) everybody  (9997)      284 2023-06-12 19:50:39.437000 ./data/data/com.termux/files/usr/lib/python3.11/site-packages/smartbets_API/__pycache__/__main__.cpython-311.pyc
+-rw-rw----   0 root         (0) everybody  (9997)     3794 2023-06-12 19:50:39.493000 ./data/data/com.termux/files/usr/lib/python3.11/site-packages/smartbets_API/__pycache__/bet_analyzer.cpython-311.pyc
+-rw-rw----   0 root         (0) everybody  (9997)     4726 2023-06-12 19:50:39.585000 ./data/data/com.termux/files/usr/lib/python3.11/site-packages/smartbets_API/__pycache__/bet_at_api_level.cpython-311.pyc
+-rw-rw----   0 root         (0) everybody  (9997)    25451 2023-06-12 19:50:39.653000 ./data/data/com.termux/files/usr/lib/python3.11/site-packages/smartbets_API/__pycache__/bet_common.cpython-311.pyc
+-rw-rw----   0 root         (0) everybody  (9997)     9331 2023-06-12 19:50:39.705000 ./data/data/com.termux/files/usr/lib/python3.11/site-packages/smartbets_API/__pycache__/configuration_handler.cpython-311.pyc
+-rw-rw----   0 root         (0) everybody  (9997)    11185 2023-06-12 19:50:39.801000 ./data/data/com.termux/files/usr/lib/python3.11/site-packages/smartbets_API/__pycache__/figure_harvester.cpython-311.pyc
+-rw-rw----   0 root         (0) everybody  (9997)     5325 2023-06-12 19:50:39.845000 ./data/data/com.termux/files/usr/lib/python3.11/site-packages/smartbets_API/__pycache__/googler.cpython-311.pyc
+-rw-rw----   0 root         (0) everybody  (9997)    11506 2023-06-12 19:50:39.897000 ./data/data/com.termux/files/usr/lib/python3.11/site-packages/smartbets_API/__pycache__/html_fetcher.cpython-311.pyc
+-rw-rw----   0 root         (0) everybody  (9997)    12038 2023-06-12 19:50:40.017000 ./data/data/com.termux/files/usr/lib/python3.11/site-packages/smartbets_API/__pycache__/interface.cpython-311.pyc
+-rw-rw----   0 root         (0) everybody  (9997)    15172 2023-06-12 19:50:40.081000 ./data/data/com.termux/files/usr/lib/python3.11/site-packages/smartbets_API/__pycache__/predictor.cpython-311.pyc
+-rw-rw----   0 root         (0) everybody  (9997)     3354 2023-06-12 19:50:40.169000 ./data/data/com.termux/files/usr/lib/python3.11/site-packages/smartbets_API/__pycache__/proxyh.cpython-311.pyc
+-rw-rw----   0 root         (0) everybody  (9997)     3358 2023-06-12 19:50:40.213000 ./data/data/com.termux/files/usr/lib/python3.11/site-packages/smartbets_API/__pycache__/tertiary_bet.cpython-311.pyc
+-rw-rw----   0 root         (0) everybody  (9997)     2050 2023-06-12 15:32:20.000000 ./data/data/com.termux/files/usr/lib/python3.11/site-packages/smartbets_API/bet_analyzer.py
+-rw-rw----   0 root         (0) everybody  (9997)     3660 2023-06-12 16:08:24.000000 ./data/data/com.termux/files/usr/lib/python3.11/site-packages/smartbets_API/bet_at_api_level.py
+-rw-rw----   0 root         (0) everybody  (9997)    11304 2023-06-12 15:32:20.000000 ./data/data/com.termux/files/usr/lib/python3.11/site-packages/smartbets_API/bet_common.py
+-rw-rw----   0 root         (0) everybody  (9997)     4144 2023-06-12 15:32:20.000000 ./data/data/com.termux/files/usr/lib/python3.11/site-packages/smartbets_API/configuration_handler.py
+-rw-rw----   0 root         (0) everybody  (9997)     6613 2023-06-12 15:32:20.000000 ./data/data/com.termux/files/usr/lib/python3.11/site-packages/smartbets_API/figure_harvester.py
+-rw-rw----   0 root         (0) everybody  (9997)     3065 2023-06-12 15:32:20.000000 ./data/data/com.termux/files/usr/lib/python3.11/site-packages/smartbets_API/googler.py
+-rw-rw----   0 root         (0) everybody  (9997)     6379 2023-06-12 15:32:20.000000 ./data/data/com.termux/files/usr/lib/python3.11/site-packages/smartbets_API/html_fetcher.py
+-rw-rw----   0 root         (0) everybody  (9997)     6612 2023-06-12 15:32:20.000000 ./data/data/com.termux/files/usr/lib/python3.11/site-packages/smartbets_API/interface.py
+-rw-rw----   0 root         (0) everybody  (9997)     8856 2023-06-12 19:21:58.000000 ./data/data/com.termux/files/usr/lib/python3.11/site-packages/smartbets_API/predictor.py
+-rw-rw----   0 root         (0) everybody  (9997)     1728 2023-06-12 15:32:20.000000 ./data/data/com.termux/files/usr/lib/python3.11/site-packages/smartbets_API/proxyh.py
+-rw-rw----   0 root         (0) everybody  (9997)     2201 2023-06-12 15:32:20.000000 ./data/data/com.termux/files/usr/lib/python3.11/site-packages/smartbets_API/tertiary_bet.py
```

### Comparing `smartbetsAPI-1.1.1/PKG-INFO` & `./data/data/com.termux/files/usr/lib/python3.11/site-packages/smartbetsAPI-1.1.3-py3.11.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: smartbetsAPI
-Version: 1.1.1
+Version: 1.1.3
 Summary: Simple football prediction API
 Home-page: https://github.com/Simatwa/smartbetsAPI
 Author: Smartwa Caleb
 Author-email: smartwacaleb@gmail.com
 Maintainer: Smartwa Caleb
 Maintainer-email: smartwacaleb@gmail.com
 License: GPL-3.0
@@ -29,15 +29,15 @@
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 <h1 align="center">smartbetsAPI</h1>
 
 <p align="center">
 
- <a href="https://github.com/Simatwa/smartbetsAPI"><img alt="Github" src="https://img.shields.io/static/v1?logo=github&color=blueviolet&label=Test&message=Passing"/></a> <a href="LICENSE"><img alt="License" src="https://img.shields.io/static/v1?logo=GPL&color=Blue&message=GPL-v3&label=License"/></a> <a href="https://pypi.org/project/smartbetsAPI"><img alt="PyPi" src="https://img.shields.io/static/v1?logo=pypi&label=Pypi&message=v1.1.1&color=green"/></a> <a href="https://github.com/psf/black"><img alt="Black" src="https://img.shields.io/static/v1?logo=Black&label=Code-style&message=Black"/></a> <a href="#"><img alt="Accuracy" src="https://img.shields.io/static/v1?logo=accuracy&label=Accuracy&message=55%&color=critical"/></a> <a href="#"><img alt="Passing" src="https://img.shields.io/static/v1?logo=Docs&label=Docs&message=Passing&color=green"/></a> <a href="#"><img alt="coverage" src="https://img.shields.io/static/v1?logo=Coverage&label=Coverage&message=100%&color=yellowgreen"/></a>  <a href="#" alt="progress"><img alt="Progress" src="https://img.shields.io/static/v1?logo=Progress&label=Progress&message=95%&color=green"/></a>  <a href="https://pepy.tech/project/smartbetsapi"><img src="https://static.pepy.tech/personalized-badge/smartbetsapi?period=total&units=international_system&left_color=grey&right_color=orange&left_text=Downloads" alt="Downloads"></a></p><br>
+ <a href="https://github.com/Simatwa/smartbetsAPI"><img alt="Github" src="https://img.shields.io/static/v1?logo=github&color=blueviolet&label=Test&message=Passing"/></a> <a href="LICENSE"><img alt="License" src="https://img.shields.io/static/v1?logo=GPL&color=Blue&message=GPL-v3&label=License"/></a> <a href="https://pypi.org/project/smartbetsAPI"><img alt="PyPi" src="https://img.shields.io/static/v1?logo=pypi&label=Pypi&message=v1.1.2&color=green"/></a> <a href="https://github.com/psf/black"><img alt="Black" src="https://img.shields.io/static/v1?logo=Black&label=Code-style&message=Black"/></a> <a href="#"><img alt="Accuracy" src="https://img.shields.io/static/v1?logo=accuracy&label=Accuracy&message=55%&color=critical"/></a> <a href="#"><img alt="Passing" src="https://img.shields.io/static/v1?logo=Docs&label=Docs&message=Passing&color=green"/></a> <a href="#"><img alt="coverage" src="https://img.shields.io/static/v1?logo=Coverage&label=Coverage&message=100%&color=yellowgreen"/></a>  <a href="#" alt="progress"><img alt="Progress" src="https://img.shields.io/static/v1?logo=Progress&label=Progress&message=95%&color=green"/></a>  <a href="https://pepy.tech/project/smartbetsapi"><img src="https://static.pepy.tech/personalized-badge/smartbetsapi?period=total&units=international_system&left_color=grey&right_color=orange&left_text=Downloads" alt="Downloads"></a></p><br>
 
  
 
  > "Punter's choice"
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: smartbetsAPI Version: 1.1.1 Summary: Simple
+Metadata-Version: 2.1 Name: smartbetsAPI Version: 1.1.3 Summary: Simple
 football prediction API Home-page: https://github.com/Simatwa/smartbetsAPI
 Author: Smartwa Caleb Author-email: smartwacaleb@gmail.com Maintainer: Smartwa
 Caleb Maintainer-email: smartwacaleb@gmail.com License: GPL-3.0 Keywords:
 Football,Predictions,Betting API,Soccer predictions,Football Predictions
 Classifier: Development Status :: 5 - Production/Stable Classifier: Environment
 :: Console Classifier: Intended Audience :: Developers Classifier: Intended
 Audience :: Customer Service Classifier: Intended Audience :: Other Audience
```

### Comparing `smartbetsAPI-1.1.1/smartbetsAPI.egg-info/SOURCES.txt` & `./data/data/com.termux/files/usr/lib/python3.11/site-packages/smartbetsAPI-1.1.3-py3.11.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `smartbetsAPI-1.1.1/smartbets_API/bet_analyzer.py` & `./data/data/com.termux/files/usr/lib/python3.11/site-packages/smartbets_API/bet_analyzer.py`

 * *Files identical despite different names*

### Comparing `smartbetsAPI-1.1.1/smartbets_API/bet_at_api_level.py` & `./data/data/com.termux/files/usr/lib/python3.11/site-packages/smartbets_API/bet_at_api_level.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,22 +1,22 @@
-from requests import Session
 from json import loads
 from sys import exit
 from os import path
 
 
 class predictor:
     def __init__(self, api_url: str, password: str, username="API"):
         """Connect to the REST API
 
         Args:
             api_url (str): Link to API
             password (str): API's password
             username (str, optional): API's username. Defaults to "API".
         """
+        from requests import Session
         self.url = api_url
         self.username = username
         self.password = password
         self.session = Session()
         # Verifies the login credentials
         __login_trial = self.__api_login()
         if not __login_trial["status_code"] == 200:
```

### Comparing `smartbetsAPI-1.1.1/smartbets_API/bet_common.py` & `./data/data/com.termux/files/usr/lib/python3.11/site-packages/smartbets_API/bet_common.py`

 * *Files identical despite different names*

### Comparing `smartbetsAPI-1.1.1/smartbets_API/configuration_handler.py` & `./data/data/com.termux/files/usr/lib/python3.11/site-packages/smartbets_API/configuration_handler.py`

 * *Files identical despite different names*

### Comparing `smartbetsAPI-1.1.1/smartbets_API/figure_harvester.py` & `./data/data/com.termux/files/usr/lib/python3.11/site-packages/smartbets_API/figure_harvester.py`

 * *Files identical despite different names*

### Comparing `smartbetsAPI-1.1.1/smartbets_API/googler.py` & `./data/data/com.termux/files/usr/lib/python3.11/site-packages/smartbets_API/googler.py`

 * *Files identical despite different names*

### Comparing `smartbetsAPI-1.1.1/smartbets_API/html_fetcher.py` & `./data/data/com.termux/files/usr/lib/python3.11/site-packages/smartbets_API/html_fetcher.py`

 * *Files identical despite different names*

### Comparing `smartbetsAPI-1.1.1/smartbets_API/interface.py` & `./data/data/com.termux/files/usr/lib/python3.11/site-packages/smartbets_API/interface.py`

 * *Files 2% similar despite different names*

```diff
@@ -116,15 +116,15 @@
 def error(msg: str, comment=None):
     logging.debug(f"INVALID {request.remote_addr} : {msg}")
     return jsonify({"message": msg, "comment": comment})
 
 
 def bad_request() -> tuple:
     info = "Kindly pass team names"
-    help = "Params {User:username, paswd:paswword, net:(true/false)}"
+    help = "Params {home:home-team, away:away-team, net:(true/false)}"
     return error(info, help), 400
 
 
 # Home route
 @app.route("/")
 def home():
     return error("Dormant path", "Paths available [/login,/predict]"), 404
```

### Comparing `smartbetsAPI-1.1.1/smartbets_API/predictor.py` & `./data/data/com.termux/files/usr/lib/python3.11/site-packages/smartbets_API/predictor.py`

 * *Files 2% similar despite different names*

```diff
@@ -2,26 +2,28 @@
     def __init__(self, **kwargs):
         v = lambda t: kwargs[t]
         self.log = v("log")
         self.color = v("color")
         self.filename = v("filename")
         self.gui = v("gui")
         self.level = v("level")
+        self.proxy=v("proxy")
 
 
 class predictor:
     def __init__(
         self,
         include_position=False,
         log=False,
         level=0,
         filename=None,
         color=False,
         gui=False,
         api=False,
+        proxy =None,
     ):
         """Initializes the class.
 
         :param include_position: (optional) Include team's league ranking in making predictions.
         :type include_position: bool
         :param log: (optional) Log at api default log's path.
         :type log: bool
@@ -41,14 +43,15 @@
 
             args = {
                 "log": log,
                 "color": color,
                 "filename": filename,
                 "gui": gui,
                 "level": level,
+                "proxy":proxy
             }
             set_config(args_handler(**args)).main()
         from .bet_common import logging
         from .bet_analyzer import analyze
         from .figure_harvester import harvest
 
         self.logging, self.harvest, self.analyze = logging, harvest, analyze
```

### Comparing `smartbetsAPI-1.1.1/smartbets_API/proxyh.py` & `./data/data/com.termux/files/usr/lib/python3.11/site-packages/smartbets_API/proxyh.py`

 * *Files identical despite different names*

### Comparing `smartbetsAPI-1.1.1/smartbets_API/tertiary_bet.py` & `./data/data/com.termux/files/usr/lib/python3.11/site-packages/smartbets_API/tertiary_bet.py`

 * *Files identical despite different names*

