# Comparing `tmp/zyppnotify-0.5.0rc2.tar.gz` & `tmp/zyppnotify-0.5.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "zyppnotify-0.5.0rc2.tar", last modified: Wed Dec 14 08:33:32 2022, max compression
+gzip compressed data, was "zyppnotify-0.5.1.tar", last modified: Mon Jun 12 08:15:02 2023, max compression
```

## Comparing `zyppnotify-0.5.0rc2.tar` & `zyppnotify-0.5.1.tar`

### file list

```diff
@@ -1,23 +1,23 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-14 08:33:32.937411 zyppnotify-0.5.0rc2/
--rw-r--r--   0 runner    (1001) docker     (123)     1061 2022-12-14 08:33:11.000000 zyppnotify-0.5.0rc2/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)       54 2022-12-14 08:33:11.000000 zyppnotify-0.5.0rc2/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     2764 2022-12-14 08:33:32.937411 zyppnotify-0.5.0rc2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     2151 2022-12-14 08:33:11.000000 zyppnotify-0.5.0rc2/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-14 08:33:32.937411 zyppnotify-0.5.0rc2/notify/
--rw-r--r--   0 runner    (1001) docker     (123)      377 2022-12-14 08:33:11.000000 zyppnotify-0.5.0rc2/notify/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      109 2022-12-14 08:33:11.000000 zyppnotify-0.5.0rc2/notify/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (123)     4074 2022-12-14 08:33:11.000000 zyppnotify-0.5.0rc2/notify/mail.py
--rw-r--r--   0 runner    (1001) docker     (123)      780 2022-12-14 08:33:11.000000 zyppnotify-0.5.0rc2/notify/msgraph.py
--rw-r--r--   0 runner    (1001) docker     (123)     3599 2022-12-14 08:33:11.000000 zyppnotify-0.5.0rc2/notify/teams.py
--rw-r--r--   0 runner    (1001) docker     (123)       94 2022-12-14 08:33:11.000000 zyppnotify-0.5.0rc2/notify/types.py
--rw-r--r--   0 runner    (1001) docker     (123)     3885 2022-12-14 08:33:11.000000 zyppnotify-0.5.0rc2/notify/utils.py
--rw-r--r--   0 runner    (1001) docker     (123)      104 2022-12-14 08:33:11.000000 zyppnotify-0.5.0rc2/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       27 2022-12-14 08:33:11.000000 zyppnotify-0.5.0rc2/requirements-dev.txt
--rw-r--r--   0 runner    (1001) docker     (123)      104 2022-12-14 08:33:11.000000 zyppnotify-0.5.0rc2/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (123)      805 2022-12-14 08:33:32.937411 zyppnotify-0.5.0rc2/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-14 08:33:32.937411 zyppnotify-0.5.0rc2/zyppnotify.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     2764 2022-12-14 08:33:32.000000 zyppnotify-0.5.0rc2/zyppnotify.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      382 2022-12-14 08:33:32.000000 zyppnotify-0.5.0rc2/zyppnotify.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2022-12-14 08:33:32.000000 zyppnotify-0.5.0rc2/zyppnotify.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      104 2022-12-14 08:33:32.000000 zyppnotify-0.5.0rc2/zyppnotify.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        7 2022-12-14 08:33:32.000000 zyppnotify-0.5.0rc2/zyppnotify.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-12 08:15:02.886470 zyppnotify-0.5.1/
+-rw-r--r--   0 runner    (1001) docker     (123)     1061 2023-06-12 08:14:48.000000 zyppnotify-0.5.1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)       54 2023-06-12 08:14:48.000000 zyppnotify-0.5.1/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     2953 2023-06-12 08:15:02.886470 zyppnotify-0.5.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2343 2023-06-12 08:14:48.000000 zyppnotify-0.5.1/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-12 08:15:02.882470 zyppnotify-0.5.1/notify/
+-rw-r--r--   0 runner    (1001) docker     (123)      372 2023-06-12 08:14:48.000000 zyppnotify-0.5.1/notify/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      109 2023-06-12 08:14:48.000000 zyppnotify-0.5.1/notify/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4074 2023-06-12 08:14:48.000000 zyppnotify-0.5.1/notify/mail.py
+-rw-r--r--   0 runner    (1001) docker     (123)      780 2023-06-12 08:14:48.000000 zyppnotify-0.5.1/notify/msgraph.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3599 2023-06-12 08:14:48.000000 zyppnotify-0.5.1/notify/teams.py
+-rw-r--r--   0 runner    (1001) docker     (123)       94 2023-06-12 08:14:48.000000 zyppnotify-0.5.1/notify/types.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3885 2023-06-12 08:14:48.000000 zyppnotify-0.5.1/notify/utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)      104 2023-06-12 08:14:48.000000 zyppnotify-0.5.1/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       46 2023-06-12 08:14:48.000000 zyppnotify-0.5.1/requirements-dev.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      104 2023-06-12 08:14:48.000000 zyppnotify-0.5.1/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      800 2023-06-12 08:15:02.886470 zyppnotify-0.5.1/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-12 08:15:02.886470 zyppnotify-0.5.1/zyppnotify.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     2953 2023-06-12 08:15:02.000000 zyppnotify-0.5.1/zyppnotify.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      382 2023-06-12 08:15:02.000000 zyppnotify-0.5.1/zyppnotify.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-12 08:15:02.000000 zyppnotify-0.5.1/zyppnotify.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      104 2023-06-12 08:15:02.000000 zyppnotify-0.5.1/zyppnotify.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        7 2023-06-12 08:15:02.000000 zyppnotify-0.5.1/zyppnotify.egg-info/top_level.txt
```

### Comparing `zyppnotify-0.5.0rc2/LICENSE` & `zyppnotify-0.5.1/LICENSE`

 * *Files identical despite different names*

### Comparing `zyppnotify-0.5.0rc2/PKG-INFO` & `zyppnotify-0.5.1/README.md`

 * *Files 11% similar despite different names*

```diff
@@ -1,24 +1,7 @@
-Metadata-Version: 2.1
-Name: zyppnotify
-Version: 0.5.0rc2
-Summary: Send users notifications through various platforms
-Home-page: https://github.com/zypp-io/zyppnotify
-Author: Zypp
-Author-email: hello@zypp.io
-Project-URL: Bug Tracker, https://github.com/zypp-io/zyppnotify/issues
-Project-URL: Source, https://github.com/zypp-io/zyppnotify
-Keywords: python,notifications,teams,e-mail
-Classifier: Programming Language :: Python :: 3
-Classifier: License :: OSI Approved :: MIT License
-Classifier: Operating System :: OS Independent
-Requires-Python: >=3.6
-Description-Content-Type: text/markdown
-License-File: LICENSE
-
 <div style="text-align:center"><img alt="logo" src="https://www.zypp.io/static/assets/img/logos/zypp/white/500px.png" width="200"></div>
 <br>
 
 [![Downloads](https://pepy.tech/badge/zyppnotify)](https://pepy.tech/project/zyppnotify)
 [![PyPI version](https://badge.fury.io/py/zyppnotify.svg)](https://badge.fury.io/py/zyppnotify)
 [![Open Source](https://badges.frapsoft.com/os/v1/open-source.svg?v=103)](https://opensource.org/)
 
@@ -31,15 +14,15 @@
 ---
 
 ```commandline
 pip install zyppnotify
 ```
 
 ## Notify Mail
-When using the `NotifyMail` class, the environment variables `EMAIL_USER` and `EMAIL_PW` need to be set.
+When using the `NotifyMail` class, the environment variables `EMAIL_USER` (mailadress you want to mail with), `MAIL_TENANT_ID`, `MAIL_CLIENT_ID` and `MAIL_CLIENT_SECRET` (3x App registration credentials with User.Read.All permission with admin consent to authenticate to MS Graph) need to be set.
 The initialization of this class will return an error if one of thes variables is not set.
 
 ```python
 from notify import NotifyMail, NotifyTeams
 
 # versturen van een basis bericht met onderwerp en tekst
 mail = NotifyMail(to="reveiver@domain.com",
```

### Comparing `zyppnotify-0.5.0rc2/notify/mail.py` & `zyppnotify-0.5.1/notify/mail.py`

 * *Files identical despite different names*

### Comparing `zyppnotify-0.5.0rc2/notify/msgraph.py` & `zyppnotify-0.5.1/notify/msgraph.py`

 * *Files identical despite different names*

### Comparing `zyppnotify-0.5.0rc2/notify/teams.py` & `zyppnotify-0.5.1/notify/teams.py`

 * *Files identical despite different names*

### Comparing `zyppnotify-0.5.0rc2/notify/utils.py` & `zyppnotify-0.5.1/notify/utils.py`

 * *Files identical despite different names*

### Comparing `zyppnotify-0.5.0rc2/setup.cfg` & `zyppnotify-0.5.1/setup.cfg`

 * *Files 18% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [metadata]
 name = zyppnotify
-version = 0.5.0-rc.2
+version = 0.5.1
 author = Zypp
 author_email = hello@zypp.io
 description = Send users notifications through various platforms
 long_description = file: README.md
 long_description_content_type = text/markdown
 keywords = python, notifications, teams, e-mail
 url = https://github.com/zypp-io/zyppnotify
@@ -16,18 +16,18 @@
 	License :: OSI Approved :: MIT License
 	Operating System :: OS Independent
 
 [options]
 packages = notify
 python_requires = >=3.6
 install_requires = 
-	Babel~=2.10.3
-	pymsteams~=0.2.1
-	pandas~=1.4.4
-	tabulate~=0.8.10
+	Babel>=2.10.3
+	pymsteams>=0.2.1
+	pandas>=1.4.4
+	tabulate>=0.8.10
 	msgraph-core==0.2.2
 	azure-identity==1.7.1
 
 [egg_info]
 tag_build = 
 tag_date = 0
```

### Comparing `zyppnotify-0.5.0rc2/zyppnotify.egg-info/PKG-INFO` & `zyppnotify-0.5.1/PKG-INFO`

 * *Files 20% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: zyppnotify
-Version: 0.5.0rc2
+Version: 0.5.1
 Summary: Send users notifications through various platforms
 Home-page: https://github.com/zypp-io/zyppnotify
 Author: Zypp
 Author-email: hello@zypp.io
 Project-URL: Bug Tracker, https://github.com/zypp-io/zyppnotify/issues
 Project-URL: Source, https://github.com/zypp-io/zyppnotify
 Keywords: python,notifications,teams,e-mail
@@ -31,15 +31,15 @@
 ---
 
 ```commandline
 pip install zyppnotify
 ```
 
 ## Notify Mail
-When using the `NotifyMail` class, the environment variables `EMAIL_USER` and `EMAIL_PW` need to be set.
+When using the `NotifyMail` class, the environment variables `EMAIL_USER` (mailadress you want to mail with), `MAIL_TENANT_ID`, `MAIL_CLIENT_ID` and `MAIL_CLIENT_SECRET` (3x App registration credentials with User.Read.All permission with admin consent to authenticate to MS Graph) need to be set.
 The initialization of this class will return an error if one of thes variables is not set.
 
 ```python
 from notify import NotifyMail, NotifyTeams
 
 # versturen van een basis bericht met onderwerp en tekst
 mail = NotifyMail(to="reveiver@domain.com",
```

