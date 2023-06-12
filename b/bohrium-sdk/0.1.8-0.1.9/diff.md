# Comparing `tmp/bohrium-sdk-0.1.8.tar.gz` & `tmp/bohrium-sdk-0.1.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "bohrium-sdk-0.1.8.tar", last modified: Fri Jun  2 07:39:44 2023, max compression
+gzip compressed data, was "bohrium-sdk-0.1.9.tar", last modified: Fri Jun  2 08:11:57 2023, max compression
```

## Comparing `bohrium-sdk-0.1.8.tar` & `bohrium-sdk-0.1.9.tar`

### file list

```diff
@@ -1,25 +1,25 @@
-drwxr-xr-x   0 dingzhaohan   (501) staff       (20)        0 2023-06-02 07:39:44.107296 bohrium-sdk-0.1.8/
--rw-r--r--   0 dingzhaohan   (501) staff       (20)      205 2023-06-02 07:39:44.106062 bohrium-sdk-0.1.8/PKG-INFO
--rw-r--r--   0 dingzhaohan   (501) staff       (20)       56 2023-05-16 07:10:39.000000 bohrium-sdk-0.1.8/README.md
-drwxr-xr-x   0 dingzhaohan   (501) staff       (20)        0 2023-06-02 07:39:44.089518 bohrium-sdk-0.1.8/bohrium_sdk.egg-info/
--rw-r--r--   0 dingzhaohan   (501) staff       (20)      205 2023-06-02 07:39:44.000000 bohrium-sdk-0.1.8/bohrium_sdk.egg-info/PKG-INFO
--rw-r--r--   0 dingzhaohan   (501) staff       (20)      459 2023-06-02 07:39:44.000000 bohrium-sdk-0.1.8/bohrium_sdk.egg-info/SOURCES.txt
--rw-r--r--   0 dingzhaohan   (501) staff       (20)        1 2023-06-02 07:39:44.000000 bohrium-sdk-0.1.8/bohrium_sdk.egg-info/dependency_links.txt
--rw-r--r--   0 dingzhaohan   (501) staff       (20)       84 2023-06-02 07:39:44.000000 bohrium-sdk-0.1.8/bohrium_sdk.egg-info/entry_points.txt
--rw-r--r--   0 dingzhaohan   (501) staff       (20)       11 2023-06-02 07:39:44.000000 bohrium-sdk-0.1.8/bohrium_sdk.egg-info/top_level.txt
-drwxr-xr-x   0 dingzhaohan   (501) staff       (20)        0 2023-06-02 07:39:44.103219 bohrium-sdk-0.1.8/bohriumsdk/
--rw-r--r--   0 dingzhaohan   (501) staff       (20)      123 2023-05-16 07:22:01.000000 bohrium-sdk-0.1.8/bohriumsdk/__init__.py
--rw-r--r--   0 dingzhaohan   (501) staff       (20)        0 2023-05-29 08:11:22.000000 bohrium-sdk-0.1.8/bohriumsdk/__main__.py
--rw-r--r--   0 dingzhaohan   (501) staff       (20)     6147 2023-06-02 07:37:14.000000 bohrium-sdk-0.1.8/bohriumsdk/client.py
--rw-r--r--   0 dingzhaohan   (501) staff       (20)     1970 2023-05-30 07:06:19.000000 bohrium-sdk-0.1.8/bohriumsdk/image.py
--rw-r--r--   0 dingzhaohan   (501) staff       (20)     3766 2023-05-30 07:06:03.000000 bohrium-sdk-0.1.8/bohriumsdk/job.py
--rw-r--r--   0 dingzhaohan   (501) staff       (20)     2159 2023-05-30 07:06:38.000000 bohrium-sdk-0.1.8/bohriumsdk/node.py
--rw-r--r--   0 dingzhaohan   (501) staff       (20)     2223 2023-05-30 07:25:30.000000 bohrium-sdk-0.1.8/bohriumsdk/project.py
--rw-r--r--   0 dingzhaohan   (501) staff       (20)     2835 2023-05-30 07:06:55.000000 bohrium-sdk-0.1.8/bohriumsdk/storage.py
-drwxr-xr-x   0 dingzhaohan   (501) staff       (20)        0 2023-06-02 07:39:44.105307 bohrium-sdk-0.1.8/bohriumsdk/test/
--rw-r--r--   0 dingzhaohan   (501) staff       (20)        0 2023-05-29 08:09:08.000000 bohrium-sdk-0.1.8/bohriumsdk/test/__init__.py
--rw-r--r--   0 dingzhaohan   (501) staff       (20)       80 2023-05-29 08:13:02.000000 bohrium-sdk-0.1.8/bohriumsdk/test/test_node.py
--rw-r--r--   0 dingzhaohan   (501) staff       (20)     2369 2023-05-30 01:45:00.000000 bohrium-sdk-0.1.8/bohriumsdk/test.py
--rw-r--r--   0 dingzhaohan   (501) staff       (20)     4730 2023-06-02 07:31:47.000000 bohrium-sdk-0.1.8/bohriumsdk/util.py
--rw-r--r--   0 dingzhaohan   (501) staff       (20)       38 2023-06-02 07:39:44.107375 bohrium-sdk-0.1.8/setup.cfg
--rw-r--r--   0 dingzhaohan   (501) staff       (20)      501 2023-06-02 07:39:33.000000 bohrium-sdk-0.1.8/setup.py
+drwxr-xr-x   0 dingzhaohan   (501) staff       (20)        0 2023-06-02 08:11:57.332857 bohrium-sdk-0.1.9/
+-rw-r--r--   0 dingzhaohan   (501) staff       (20)      205 2023-06-02 08:11:57.332654 bohrium-sdk-0.1.9/PKG-INFO
+-rw-r--r--   0 dingzhaohan   (501) staff       (20)       56 2023-05-16 07:10:39.000000 bohrium-sdk-0.1.9/README.md
+drwxr-xr-x   0 dingzhaohan   (501) staff       (20)        0 2023-06-02 08:11:57.327827 bohrium-sdk-0.1.9/bohrium_sdk.egg-info/
+-rw-r--r--   0 dingzhaohan   (501) staff       (20)      205 2023-06-02 08:11:57.000000 bohrium-sdk-0.1.9/bohrium_sdk.egg-info/PKG-INFO
+-rw-r--r--   0 dingzhaohan   (501) staff       (20)      459 2023-06-02 08:11:57.000000 bohrium-sdk-0.1.9/bohrium_sdk.egg-info/SOURCES.txt
+-rw-r--r--   0 dingzhaohan   (501) staff       (20)        1 2023-06-02 08:11:57.000000 bohrium-sdk-0.1.9/bohrium_sdk.egg-info/dependency_links.txt
+-rw-r--r--   0 dingzhaohan   (501) staff       (20)       84 2023-06-02 08:11:57.000000 bohrium-sdk-0.1.9/bohrium_sdk.egg-info/entry_points.txt
+-rw-r--r--   0 dingzhaohan   (501) staff       (20)       11 2023-06-02 08:11:57.000000 bohrium-sdk-0.1.9/bohrium_sdk.egg-info/top_level.txt
+drwxr-xr-x   0 dingzhaohan   (501) staff       (20)        0 2023-06-02 08:11:57.331425 bohrium-sdk-0.1.9/bohriumsdk/
+-rw-r--r--   0 dingzhaohan   (501) staff       (20)      123 2023-05-16 07:22:01.000000 bohrium-sdk-0.1.9/bohriumsdk/__init__.py
+-rw-r--r--   0 dingzhaohan   (501) staff       (20)        0 2023-05-29 08:11:22.000000 bohrium-sdk-0.1.9/bohriumsdk/__main__.py
+-rw-r--r--   0 dingzhaohan   (501) staff       (20)     6137 2023-06-02 08:11:36.000000 bohrium-sdk-0.1.9/bohriumsdk/client.py
+-rw-r--r--   0 dingzhaohan   (501) staff       (20)     1970 2023-05-30 07:06:19.000000 bohrium-sdk-0.1.9/bohriumsdk/image.py
+-rw-r--r--   0 dingzhaohan   (501) staff       (20)     3766 2023-05-30 07:06:03.000000 bohrium-sdk-0.1.9/bohriumsdk/job.py
+-rw-r--r--   0 dingzhaohan   (501) staff       (20)     2159 2023-05-30 07:06:38.000000 bohrium-sdk-0.1.9/bohriumsdk/node.py
+-rw-r--r--   0 dingzhaohan   (501) staff       (20)     2223 2023-05-30 07:25:30.000000 bohrium-sdk-0.1.9/bohriumsdk/project.py
+-rw-r--r--   0 dingzhaohan   (501) staff       (20)     2835 2023-05-30 07:06:55.000000 bohrium-sdk-0.1.9/bohriumsdk/storage.py
+drwxr-xr-x   0 dingzhaohan   (501) staff       (20)        0 2023-06-02 08:11:57.332215 bohrium-sdk-0.1.9/bohriumsdk/test/
+-rw-r--r--   0 dingzhaohan   (501) staff       (20)        0 2023-05-29 08:09:08.000000 bohrium-sdk-0.1.9/bohriumsdk/test/__init__.py
+-rw-r--r--   0 dingzhaohan   (501) staff       (20)       80 2023-05-29 08:13:02.000000 bohrium-sdk-0.1.9/bohriumsdk/test/test_node.py
+-rw-r--r--   0 dingzhaohan   (501) staff       (20)     2369 2023-05-30 01:45:00.000000 bohrium-sdk-0.1.9/bohriumsdk/test.py
+-rw-r--r--   0 dingzhaohan   (501) staff       (20)     4730 2023-06-02 07:31:47.000000 bohrium-sdk-0.1.9/bohriumsdk/util.py
+-rw-r--r--   0 dingzhaohan   (501) staff       (20)       38 2023-06-02 08:11:57.333020 bohrium-sdk-0.1.9/setup.cfg
+-rw-r--r--   0 dingzhaohan   (501) staff       (20)      501 2023-06-02 08:11:41.000000 bohrium-sdk-0.1.9/setup.py
```

### Comparing `bohrium-sdk-0.1.8/bohriumsdk/client.py` & `bohrium-sdk-0.1.9/bohriumsdk/client.py`

 * *Files 1% similar despite different names*

```diff
@@ -117,23 +117,23 @@
     def login(self):
         email = input("Please enter Bohrium Account Email: ")
         password = getpass.getpass(prompt="Please enter password: ")
         post_data = {
             'username': email,
             'password': password
         }
-        resp = requests.post('https://bohrium.test.dp.tech/account_gw/login', json=post_data).json().get("data", {})
+        resp = requests.post('https://bohrium.dp.tech/account_gw/login', json=post_data).json().get("data", {})
         self.token = resp.get('token', '')
         if self.token: print("Login successfully!")
         else: print("Login failed!")
 
     def generate_access_key(self, name="default"):
         post_data = { "name": name }
         headers = { 'Authorization': f'Bearer {self.token}' }
-        resp = requests.post(url="https://bohrium-api.test.dp.tech/bohrapi/v1/ak/add", json=post_data, headers=headers)
+        resp = requests.post(url="https://bohrium-api.dp.tech/bohrapi/v1/ak/add", json=post_data, headers=headers)
         print(resp)
         resp = resp.json().get("data", {})
         self.access_key = resp.get("accessKey", "")
         data = f"[Credentials]\nbaseUrl=https://openapi.dp.tech\naccessKey={self.access_key}"
         with open(self.config_file_location_expand, 'w') as f:
             f.write(data)
         return resp
```

### Comparing `bohrium-sdk-0.1.8/bohriumsdk/image.py` & `bohrium-sdk-0.1.9/bohriumsdk/image.py`

 * *Files identical despite different names*

### Comparing `bohrium-sdk-0.1.8/bohriumsdk/job.py` & `bohrium-sdk-0.1.9/bohriumsdk/job.py`

 * *Files identical despite different names*

### Comparing `bohrium-sdk-0.1.8/bohriumsdk/node.py` & `bohrium-sdk-0.1.9/bohriumsdk/node.py`

 * *Files identical despite different names*

### Comparing `bohrium-sdk-0.1.8/bohriumsdk/project.py` & `bohrium-sdk-0.1.9/bohriumsdk/project.py`

 * *Files identical despite different names*

### Comparing `bohrium-sdk-0.1.8/bohriumsdk/storage.py` & `bohrium-sdk-0.1.9/bohriumsdk/storage.py`

 * *Files identical despite different names*

### Comparing `bohrium-sdk-0.1.8/bohriumsdk/test.py` & `bohrium-sdk-0.1.9/bohriumsdk/test.py`

 * *Files identical despite different names*

### Comparing `bohrium-sdk-0.1.8/bohriumsdk/util.py` & `bohrium-sdk-0.1.9/bohriumsdk/util.py`

 * *Files identical despite different names*

