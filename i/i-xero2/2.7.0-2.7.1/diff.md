# Comparing `tmp/i_xero2-2.7.0.tar.gz` & `tmp/i_xero2-2.7.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "i_xero2-2.7.0.tar", max compression
+gzip compressed data, was "i_xero2-2.7.1.tar", max compression
```

## Comparing `i_xero2-2.7.0.tar` & `i_xero2-2.7.1.tar`

### file list

```diff
@@ -1,9 +1,9 @@
--rw-r--r--   0        0        0     1079 2021-10-14 01:56:57.796205 i_xero2-2.7.0/LICENSE
--rw-r--r--   0        0        0     1403 2022-11-30 18:07:38.057869 i_xero2-2.7.0/README.md
--rw-r--r--   0        0        0      229 2023-06-09 20:33:49.252776 i_xero2-2.7.0/i_xero2/__init__.py
--rw-r--r--   0        0        0     2143 2022-11-03 18:19:48.298576 i_xero2-2.7.0/i_xero2/i_flask.py
--rw-r--r--   0        0        0    49162 2023-06-09 20:33:20.776544 i_xero2-2.7.0/i_xero2/i_xero.py
--rw-r--r--   0        0        0     7090 2022-11-03 18:19:48.298576 i_xero2-2.7.0/i_xero2/i_xero_ui.py
--rw-r--r--   0        0        0      829 2023-06-09 20:33:33.640649 i_xero2-2.7.0/pyproject.toml
--rw-r--r--   0        0        0     2260 1970-01-01 00:00:00.000000 i_xero2-2.7.0/setup.py
--rw-r--r--   0        0        0     2235 1970-01-01 00:00:00.000000 i_xero2-2.7.0/PKG-INFO
+-rw-r--r--   0        0        0     1079 2021-10-14 01:56:57.796205 i_xero2-2.7.1/LICENSE
+-rw-r--r--   0        0        0     1403 2022-11-30 18:07:38.057869 i_xero2-2.7.1/README.md
+-rw-r--r--   0        0        0      229 2023-06-12 18:12:22.375635 i_xero2-2.7.1/i_xero2/__init__.py
+-rw-r--r--   0        0        0     2143 2022-11-03 18:19:48.298576 i_xero2-2.7.1/i_xero2/i_flask.py
+-rw-r--r--   0        0        0    49180 2023-06-12 18:11:40.111269 i_xero2-2.7.1/i_xero2/i_xero.py
+-rw-r--r--   0        0        0     7090 2022-11-03 18:19:48.298576 i_xero2-2.7.1/i_xero2/i_xero_ui.py
+-rw-r--r--   0        0        0      829 2023-06-12 18:12:16.511584 i_xero2-2.7.1/pyproject.toml
+-rw-r--r--   0        0        0     2260 1970-01-01 00:00:00.000000 i_xero2-2.7.1/setup.py
+-rw-r--r--   0        0        0     2235 1970-01-01 00:00:00.000000 i_xero2-2.7.1/PKG-INFO
```

### Comparing `i_xero2-2.7.0/LICENSE` & `i_xero2-2.7.1/LICENSE`

 * *Files identical despite different names*

### Comparing `i_xero2-2.7.0/README.md` & `i_xero2-2.7.1/README.md`

 * *Files identical despite different names*

### Comparing `i_xero2-2.7.0/i_xero2/i_flask.py` & `i_xero2-2.7.1/i_xero2/i_flask.py`

 * *Files identical despite different names*

### Comparing `i_xero2-2.7.0/i_xero2/i_xero.py` & `i_xero2-2.7.1/i_xero2/i_xero.py`

 * *Files 0% similar despite different names*

```diff
@@ -99,16 +99,17 @@
         """
         # check for window length
         if len(self.call_window) < self.rate_limit_calls:
             self.call_window.append(datetime.now())
             return
 
         # check for window duration
-        if duration := datetime.now() - self.call_window[0] < self.rate_limit_seconds:
-            time.sleep(self.rate_limit_seconds - duration.total_seconds())
+        duration = (datetime.now() - self.call_window[0]).total_seconds()
+        if duration < self.rate_limit_seconds:
+            time.sleep(self.rate_limit_seconds - duration)
             self.call_window.append(datetime.now())
 
     def set_client(self):
         """Connect to Xero and set the client.
         """
         token = self.get_token()
```

### Comparing `i_xero2-2.7.0/i_xero2/i_xero_ui.py` & `i_xero2-2.7.1/i_xero2/i_xero_ui.py`

 * *Files identical despite different names*

### Comparing `i_xero2-2.7.0/pyproject.toml` & `i_xero2-2.7.1/pyproject.toml`

 * *Files 12% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "i-xero2"
-version = "2.7.0"
+version = "2.7.1"
 description = "Custom connector to Xero"
 authors = ["Jason Romano <aracnid@gmail.com>"]
 license = "MIT"
 readme = "README.md"
 repository = "https://github.com/aracnid/i-xero2"
 keywords = ["python", "xero"]
 packages = [{include = "i_xero2"}]
```

### Comparing `i_xero2-2.7.0/setup.py` & `i_xero2-2.7.1/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -14,15 +14,15 @@
  'flask>=2.1,<3.0',
  'i-mongodb>=2.0,<3.0',
  'pytz>=2022.1,<2023.0',
  'xero-python>=1.16,<2.0']
 
 setup_kwargs = {
     'name': 'i-xero2',
-    'version': '2.7.0',
+    'version': '2.7.1',
     'description': 'Custom connector to Xero',
     'long_description': '# i-Xero2\n\nThis is a standardized and customized connector to Xero.\n\n## Getting Started\n\nThese instructions will get you a copy of the project up and running on your local machine for development and testing purposes.\n\n### Prerequisites\n\nThis package supports the following version of Python. It probably supports older versions, but they have not been tested.\n\n- Python 3.10 or later\n\n### Installing\n\nInstall the latest package using pip.\n\n```bash\n$ pip install i-xero2\n```\n\nEnd with an example of getting some data out of the system or using it for a little demo\n\n## Running the tests\n\nBefore running the tests, you need to authorize the app with Xero and save the tenant ID in the environment.\n\n1. In Xero, switch to the "Demo Company".\n1. Run the app locally.\n\n    ```bash\n    $ python app.py\n    ```\n\n1. In the browser, navigate to `http://localhost:5000/`\n1. Follow the prompts to allow app to access Xero.\n1. Read tenants.\n1. Copy the `tenantId`.\n1. Save the tenant id as an environment variable named `XERO_TENANT_ID`.\n1. Run the tests.\n\n    ```bash\n    $ python -m pytest\n    ```\n\n## Usage\n\nTODO\n\n## Authors\n\n- **Jason Romano** - [Aracnid](https://github.com/aracnid)\n\nSee also the list of [contributors](https://github.com/aracnid/i-xero2/contributors) who participated in this project.\n\n## License\n\nThis project is licensed under the MIT License - see the [LICENSE](LICENSE) file for details\n',
     'author': 'Jason Romano',
     'author_email': 'aracnid@gmail.com',
     'maintainer': 'None',
     'maintainer_email': 'None',
     'url': 'https://github.com/aracnid/i-xero2',
```

### Comparing `i_xero2-2.7.0/PKG-INFO` & `i_xero2-2.7.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: i-xero2
-Version: 2.7.0
+Version: 2.7.1
 Summary: Custom connector to Xero
 Home-page: https://github.com/aracnid/i-xero2
 License: MIT
 Keywords: python,xero
 Author: Jason Romano
 Author-email: aracnid@gmail.com
 Requires-Python: >=3.10,<4.0
```

