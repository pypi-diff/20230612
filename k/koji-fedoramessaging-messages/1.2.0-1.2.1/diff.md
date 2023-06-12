# Comparing `tmp/koji-fedoramessaging-messages-1.2.0.tar.gz` & `tmp/koji-fedoramessaging-messages-1.2.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "koji-fedoramessaging-messages-1.2.0.tar", max compression
+gzip compressed data, was "koji-fedoramessaging-messages-1.2.1.tar", max compression
```

## Comparing `koji-fedoramessaging-messages-1.2.0.tar` & `koji-fedoramessaging-messages-1.2.1.tar`

### file list

```diff
@@ -1,26 +1,26 @@
--rw-r--r--   0        0        0    18092 2023-01-24 15:38:49.840028 koji-fedoramessaging-messages-1.2.0/LICENSE
--rw-r--r--   0        0        0      257 2023-01-24 15:38:49.840028 koji-fedoramessaging-messages-1.2.0/README.md
--rw-r--r--   0        0        0      676 2023-01-30 14:55:09.035636 koji-fedoramessaging-messages-1.2.0/koji_fedoramessaging_messages/__init__.py
--rw-r--r--   0        0        0     4969 2023-06-12 09:08:17.321402 koji-fedoramessaging-messages-1.2.0/koji_fedoramessaging_messages/base.py
--rw-r--r--   0        0        0     6977 2023-06-12 09:21:47.340321 koji-fedoramessaging-messages-1.2.0/koji_fedoramessaging_messages/build.py
--rw-r--r--   0        0        0     3468 2023-06-12 09:08:17.320402 koji-fedoramessaging-messages-1.2.0/koji_fedoramessaging_messages/package.py
--rw-r--r--   0        0        0     2470 2023-06-12 09:08:17.320402 koji-fedoramessaging-messages-1.2.0/koji_fedoramessaging_messages/repo.py
--rw-r--r--   0        0        0     9699 2023-06-12 09:08:17.321402 koji-fedoramessaging-messages-1.2.0/koji_fedoramessaging_messages/rpm.py
--rw-r--r--   0        0        0     4686 2023-06-12 09:07:06.617144 koji-fedoramessaging-messages-1.2.0/koji_fedoramessaging_messages/tag.py
--rw-r--r--   0        0        0     4155 2023-06-12 09:08:17.320402 koji-fedoramessaging-messages-1.2.0/koji_fedoramessaging_messages/task.py
--rw-r--r--   0        0        0     1534 2023-06-12 09:08:17.320402 koji-fedoramessaging-messages-1.2.0/koji_fedoramessaging_messages/utilities.py
--rwxr-xr-x   0        0        0      333 2023-05-03 11:22:25.710843 koji-fedoramessaging-messages-1.2.0/make-spec.sh
--rw-r--r--   0        0        0     2108 2023-06-12 10:28:52.708142 koji-fedoramessaging-messages-1.2.0/pyproject.toml
--rw-r--r--   0        0        0     1315 2023-05-05 14:55:46.956888 koji-fedoramessaging-messages-1.2.0/python-koji-fedoramessaging-messages.spec.in
--rw-r--r--   0        0        0        0 2023-01-24 15:38:49.841028 koji-fedoramessaging-messages-1.2.0/tests/__init__.py
--rw-r--r--   0        0        0     1061 2023-06-12 08:59:04.745385 koji-fedoramessaging-messages-1.2.0/tests/test_base.py
--rw-r--r--   0        0        0     4681 2023-06-12 09:22:34.937492 koji-fedoramessaging-messages-1.2.0/tests/test_build.py
--rw-r--r--   0        0        0     1541 2023-04-03 08:49:37.134775 koji-fedoramessaging-messages-1.2.0/tests/test_package.py
--rw-r--r--   0        0        0     1036 2023-04-03 08:49:37.134775 koji-fedoramessaging-messages-1.2.0/tests/test_repo.py
--rw-r--r--   0        0        0     3510 2023-04-03 08:49:37.135775 koji-fedoramessaging-messages-1.2.0/tests/test_rpm.py
--rw-r--r--   0        0        0     2283 2023-06-12 08:59:04.820385 koji-fedoramessaging-messages-1.2.0/tests/test_tag.py
--rw-r--r--   0        0        0    14967 2023-06-12 09:17:58.576499 koji-fedoramessaging-messages-1.2.0/tests/test_task.py
--rw-r--r--   0        0        0      322 2023-06-12 08:56:09.866746 koji-fedoramessaging-messages-1.2.0/tests/test_utilities.py
--rw-r--r--   0        0        0      512 2023-06-12 09:23:28.867686 koji-fedoramessaging-messages-1.2.0/tox.ini
--rw-r--r--   0        0        0     2165 2023-06-12 10:34:00.099405 koji-fedoramessaging-messages-1.2.0/setup.py
--rw-r--r--   0        0        0      999 2023-06-12 10:34:00.099705 koji-fedoramessaging-messages-1.2.0/PKG-INFO
+-rw-r--r--   0        0        0    18092 2023-01-24 15:38:49.840028 koji-fedoramessaging-messages-1.2.1/LICENSE
+-rw-r--r--   0        0        0      257 2023-01-24 15:38:49.840028 koji-fedoramessaging-messages-1.2.1/README.md
+-rw-r--r--   0        0        0      676 2023-01-30 14:55:09.035636 koji-fedoramessaging-messages-1.2.1/koji_fedoramessaging_messages/__init__.py
+-rw-r--r--   0        0        0     4969 2023-06-12 09:08:17.321402 koji-fedoramessaging-messages-1.2.1/koji_fedoramessaging_messages/base.py
+-rw-r--r--   0        0        0     6977 2023-06-12 09:21:47.340321 koji-fedoramessaging-messages-1.2.1/koji_fedoramessaging_messages/build.py
+-rw-r--r--   0        0        0     3468 2023-06-12 09:08:17.320402 koji-fedoramessaging-messages-1.2.1/koji_fedoramessaging_messages/package.py
+-rw-r--r--   0        0        0     2470 2023-06-12 09:08:17.320402 koji-fedoramessaging-messages-1.2.1/koji_fedoramessaging_messages/repo.py
+-rw-r--r--   0        0        0     9699 2023-06-12 09:08:17.321402 koji-fedoramessaging-messages-1.2.1/koji_fedoramessaging_messages/rpm.py
+-rw-r--r--   0        0        0     4686 2023-06-12 09:07:06.617144 koji-fedoramessaging-messages-1.2.1/koji_fedoramessaging_messages/tag.py
+-rw-r--r--   0        0        0     4155 2023-06-12 09:08:17.320402 koji-fedoramessaging-messages-1.2.1/koji_fedoramessaging_messages/task.py
+-rw-r--r--   0        0        0     1534 2023-06-12 09:08:17.320402 koji-fedoramessaging-messages-1.2.1/koji_fedoramessaging_messages/utilities.py
+-rwxr-xr-x   0        0        0      333 2023-05-03 11:22:25.710843 koji-fedoramessaging-messages-1.2.1/make-spec.sh
+-rw-r--r--   0        0        0     2108 2023-06-12 10:57:04.772263 koji-fedoramessaging-messages-1.2.1/pyproject.toml
+-rw-r--r--   0        0        0     1302 2023-06-12 10:54:15.813652 koji-fedoramessaging-messages-1.2.1/python-koji-fedoramessaging-messages.spec.in
+-rw-r--r--   0        0        0        0 2023-01-24 15:38:49.841028 koji-fedoramessaging-messages-1.2.1/tests/__init__.py
+-rw-r--r--   0        0        0     1061 2023-06-12 08:59:04.745385 koji-fedoramessaging-messages-1.2.1/tests/test_base.py
+-rw-r--r--   0        0        0     4681 2023-06-12 09:22:34.937492 koji-fedoramessaging-messages-1.2.1/tests/test_build.py
+-rw-r--r--   0        0        0     1541 2023-04-03 08:49:37.134775 koji-fedoramessaging-messages-1.2.1/tests/test_package.py
+-rw-r--r--   0        0        0     1036 2023-04-03 08:49:37.134775 koji-fedoramessaging-messages-1.2.1/tests/test_repo.py
+-rw-r--r--   0        0        0     3510 2023-04-03 08:49:37.135775 koji-fedoramessaging-messages-1.2.1/tests/test_rpm.py
+-rw-r--r--   0        0        0     2283 2023-06-12 08:59:04.820385 koji-fedoramessaging-messages-1.2.1/tests/test_tag.py
+-rw-r--r--   0        0        0    14967 2023-06-12 09:17:58.576499 koji-fedoramessaging-messages-1.2.1/tests/test_task.py
+-rw-r--r--   0        0        0      322 2023-06-12 08:56:09.866746 koji-fedoramessaging-messages-1.2.1/tests/test_utilities.py
+-rw-r--r--   0        0        0      512 2023-06-12 09:23:28.867686 koji-fedoramessaging-messages-1.2.1/tox.ini
+-rw-r--r--   0        0        0     2165 2023-06-12 10:58:08.051550 koji-fedoramessaging-messages-1.2.1/setup.py
+-rw-r--r--   0        0        0      999 2023-06-12 10:58:08.051818 koji-fedoramessaging-messages-1.2.1/PKG-INFO
```

### Comparing `koji-fedoramessaging-messages-1.2.0/LICENSE` & `koji-fedoramessaging-messages-1.2.1/LICENSE`

 * *Files identical despite different names*

### Comparing `koji-fedoramessaging-messages-1.2.0/koji_fedoramessaging_messages/__init__.py` & `koji-fedoramessaging-messages-1.2.1/koji_fedoramessaging_messages/__init__.py`

 * *Files identical despite different names*

### Comparing `koji-fedoramessaging-messages-1.2.0/koji_fedoramessaging_messages/base.py` & `koji-fedoramessaging-messages-1.2.1/koji_fedoramessaging_messages/base.py`

 * *Files identical despite different names*

### Comparing `koji-fedoramessaging-messages-1.2.0/koji_fedoramessaging_messages/build.py` & `koji-fedoramessaging-messages-1.2.1/koji_fedoramessaging_messages/build.py`

 * *Files identical despite different names*

### Comparing `koji-fedoramessaging-messages-1.2.0/koji_fedoramessaging_messages/package.py` & `koji-fedoramessaging-messages-1.2.1/koji_fedoramessaging_messages/package.py`

 * *Files identical despite different names*

### Comparing `koji-fedoramessaging-messages-1.2.0/koji_fedoramessaging_messages/repo.py` & `koji-fedoramessaging-messages-1.2.1/koji_fedoramessaging_messages/repo.py`

 * *Files identical despite different names*

### Comparing `koji-fedoramessaging-messages-1.2.0/koji_fedoramessaging_messages/rpm.py` & `koji-fedoramessaging-messages-1.2.1/koji_fedoramessaging_messages/rpm.py`

 * *Files identical despite different names*

### Comparing `koji-fedoramessaging-messages-1.2.0/koji_fedoramessaging_messages/tag.py` & `koji-fedoramessaging-messages-1.2.1/koji_fedoramessaging_messages/tag.py`

 * *Files identical despite different names*

### Comparing `koji-fedoramessaging-messages-1.2.0/koji_fedoramessaging_messages/task.py` & `koji-fedoramessaging-messages-1.2.1/koji_fedoramessaging_messages/task.py`

 * *Files identical despite different names*

### Comparing `koji-fedoramessaging-messages-1.2.0/koji_fedoramessaging_messages/utilities.py` & `koji-fedoramessaging-messages-1.2.1/koji_fedoramessaging_messages/utilities.py`

 * *Files identical despite different names*

### Comparing `koji-fedoramessaging-messages-1.2.0/pyproject.toml` & `koji-fedoramessaging-messages-1.2.1/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "koji-fedoramessaging-messages"
-version = "1.2.0"
+version = "1.2.1"
 description = "A schema package for messages sent by the koji-fedoramessaging plugin"
 
 license = "GPL-3.0-or-later"
 
 authors = [
   "Fedora Infrastructure Team <infrastructure@lists.fedoraproject.org>"
 ]
```

### Comparing `koji-fedoramessaging-messages-1.2.0/python-koji-fedoramessaging-messages.spec.in` & `koji-fedoramessaging-messages-1.2.1/python-koji-fedoramessaging-messages.spec.in`

 * *Files 3% similar despite different names*

```diff
@@ -36,15 +36,15 @@
 %build
 %py3_build
 
 %install
 %py3_install
 
 %check
-%{__python3} -m pytest -v %{pypi_name}/tests/
+%{__python3} -m pytest -v tests/
 
 %files -n python3-%{rpm_name}
 %license LICENSE
 %doc README.md
 %{python3_sitelib}/%{pypi_name}
 %{python3_sitelib}/%{pypi_name}-%{pypi_version}-py%{python3_version}.egg-info
```

### Comparing `koji-fedoramessaging-messages-1.2.0/tests/test_base.py` & `koji-fedoramessaging-messages-1.2.1/tests/test_base.py`

 * *Files identical despite different names*

### Comparing `koji-fedoramessaging-messages-1.2.0/tests/test_build.py` & `koji-fedoramessaging-messages-1.2.1/tests/test_build.py`

 * *Files identical despite different names*

### Comparing `koji-fedoramessaging-messages-1.2.0/tests/test_package.py` & `koji-fedoramessaging-messages-1.2.1/tests/test_package.py`

 * *Files identical despite different names*

### Comparing `koji-fedoramessaging-messages-1.2.0/tests/test_repo.py` & `koji-fedoramessaging-messages-1.2.1/tests/test_repo.py`

 * *Files identical despite different names*

### Comparing `koji-fedoramessaging-messages-1.2.0/tests/test_rpm.py` & `koji-fedoramessaging-messages-1.2.1/tests/test_rpm.py`

 * *Files identical despite different names*

### Comparing `koji-fedoramessaging-messages-1.2.0/tests/test_tag.py` & `koji-fedoramessaging-messages-1.2.1/tests/test_tag.py`

 * *Files identical despite different names*

### Comparing `koji-fedoramessaging-messages-1.2.0/tests/test_task.py` & `koji-fedoramessaging-messages-1.2.1/tests/test_task.py`

 * *Files identical despite different names*

### Comparing `koji-fedoramessaging-messages-1.2.0/tox.ini` & `koji-fedoramessaging-messages-1.2.1/tox.ini`

 * *Files identical despite different names*

### Comparing `koji-fedoramessaging-messages-1.2.0/setup.py` & `koji-fedoramessaging-messages-1.2.1/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -26,15 +26,15 @@
                      'koji_fedoramessaging.tag.UntagV1 = '
                      'koji_fedoramessaging_messages.tag:UntagV1',
                      'koji_fedoramessaging.task.TaskStateChangeV1 = '
                      'koji_fedoramessaging_messages.task:TaskStateChangeV1']}
 
 setup_kwargs = {
     'name': 'koji-fedoramessaging-messages',
-    'version': '1.2.0',
+    'version': '1.2.1',
     'description': 'A schema package for messages sent by the koji-fedoramessaging plugin',
     'long_description': '# koji-fedoramessaging messages\n\nA schema package for [koji-fedoramessaging](http://github.com/fedora-infra/koji-fedoramessaging).\n\nSee the [detailed documentation](https://fedora-messaging.readthedocs.io/en/latest/messages.html) on packaging your schemas.\n',
     'author': 'Fedora Infrastructure Team',
     'author_email': 'infrastructure@lists.fedoraproject.org',
     'maintainer': None,
     'maintainer_email': None,
     'url': 'https://github.com/fedora-infra/koji-fedoramessaging-messages',
```

### Comparing `koji-fedoramessaging-messages-1.2.0/PKG-INFO` & `koji-fedoramessaging-messages-1.2.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: koji-fedoramessaging-messages
-Version: 1.2.0
+Version: 1.2.1
 Summary: A schema package for messages sent by the koji-fedoramessaging plugin
 Home-page: https://github.com/fedora-infra/koji-fedoramessaging-messages
 License: GPL-3.0-or-later
 Keywords: fedora
 Author: Fedora Infrastructure Team
 Author-email: infrastructure@lists.fedoraproject.org
 Requires-Python: >=3.10,<4.0
```

