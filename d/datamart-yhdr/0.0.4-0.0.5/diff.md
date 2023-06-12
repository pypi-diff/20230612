# Comparing `tmp/datamart_yhdr-0.0.4.tar.gz` & `tmp/datamart_yhdr-0.0.5.tar.gz`

## Comparing `datamart_yhdr-0.0.4.tar` & `datamart_yhdr-0.0.5.tar`

### file list

```diff
@@ -1,14 +1,16 @@
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 datamart_yhdr-0.0.4/src/datamart_yhdr/__init__.py
--rw-r--r--   0        0        0      493 2020-02-02 00:00:00.000000 datamart_yhdr-0.0.4/src/datamart_yhdr/const.py
--rw-r--r--   0        0        0     3885 2020-02-02 00:00:00.000000 datamart_yhdr-0.0.4/src/datamart_yhdr/interface.py
--rw-r--r--   0        0        0      460 2020-02-02 00:00:00.000000 datamart_yhdr-0.0.4/src/datamart_yhdr/settings.py
--rw-r--r--   0        0        0     4047 2020-02-02 00:00:00.000000 datamart_yhdr-0.0.4/tests/datamart_yhdr-0.0.1-py3-none-any.whl
--rw-r--r--   0        0        0    12909 2020-02-02 00:00:00.000000 datamart_yhdr-0.0.4/tests/datamart_yhdr-0.0.1.tar.gz
--rw-r--r--   0        0        0     4413 2020-02-02 00:00:00.000000 datamart_yhdr-0.0.4/tests/datamart_yhdr-0.0.2-py3-none-any.whl
--rw-r--r--   0        0        0    13273 2020-02-02 00:00:00.000000 datamart_yhdr-0.0.4/tests/datamart_yhdr-0.0.2.tar.gz
--rw-r--r--   0        0        0     4402 2020-02-02 00:00:00.000000 datamart_yhdr-0.0.4/tests/datamart_yhdr-0.0.3-py3-none-any.whl
--rw-r--r--   0        0        0    40616 2020-02-02 00:00:00.000000 datamart_yhdr-0.0.4/tests/datamart_yhdr-0.0.3.tar.gz
--rw-r--r--   0        0        0     1090 2020-02-02 00:00:00.000000 datamart_yhdr-0.0.4/LICENSE
--rw-r--r--   0        0        0      197 2020-02-02 00:00:00.000000 datamart_yhdr-0.0.4/README.md
--rw-r--r--   0        0        0      711 2020-02-02 00:00:00.000000 datamart_yhdr-0.0.4/pyproject.toml
--rw-r--r--   0        0        0      812 2020-02-02 00:00:00.000000 datamart_yhdr-0.0.4/PKG-INFO
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 datamart_yhdr-0.0.5/src/datamart_yhdr/__init__.py
+-rw-r--r--   0        0        0      493 2020-02-02 00:00:00.000000 datamart_yhdr-0.0.5/src/datamart_yhdr/const.py
+-rw-r--r--   0        0        0     3641 2020-02-02 00:00:00.000000 datamart_yhdr-0.0.5/src/datamart_yhdr/interface.py
+-rw-r--r--   0        0        0      460 2020-02-02 00:00:00.000000 datamart_yhdr-0.0.5/src/datamart_yhdr/settings.py
+-rw-r--r--   0        0        0     4047 2020-02-02 00:00:00.000000 datamart_yhdr-0.0.5/tests/datamart_yhdr-0.0.1-py3-none-any.whl
+-rw-r--r--   0        0        0    12909 2020-02-02 00:00:00.000000 datamart_yhdr-0.0.5/tests/datamart_yhdr-0.0.1.tar.gz
+-rw-r--r--   0        0        0     4413 2020-02-02 00:00:00.000000 datamart_yhdr-0.0.5/tests/datamart_yhdr-0.0.2-py3-none-any.whl
+-rw-r--r--   0        0        0    13273 2020-02-02 00:00:00.000000 datamart_yhdr-0.0.5/tests/datamart_yhdr-0.0.2.tar.gz
+-rw-r--r--   0        0        0     4402 2020-02-02 00:00:00.000000 datamart_yhdr-0.0.5/tests/datamart_yhdr-0.0.3-py3-none-any.whl
+-rw-r--r--   0        0        0    40616 2020-02-02 00:00:00.000000 datamart_yhdr-0.0.5/tests/datamart_yhdr-0.0.3.tar.gz
+-rw-r--r--   0        0        0     4571 2020-02-02 00:00:00.000000 datamart_yhdr-0.0.5/tests/datamart_yhdr-0.0.4-py3-none-any.whl
+-rw-r--r--   0        0        0    79181 2020-02-02 00:00:00.000000 datamart_yhdr-0.0.5/tests/datamart_yhdr-0.0.4.tar.gz
+-rw-r--r--   0        0        0     1090 2020-02-02 00:00:00.000000 datamart_yhdr-0.0.5/LICENSE
+-rw-r--r--   0        0        0      197 2020-02-02 00:00:00.000000 datamart_yhdr-0.0.5/README.md
+-rw-r--r--   0        0        0      711 2020-02-02 00:00:00.000000 datamart_yhdr-0.0.5/pyproject.toml
+-rw-r--r--   0        0        0      812 2020-02-02 00:00:00.000000 datamart_yhdr-0.0.5/PKG-INFO
```

### Comparing `datamart_yhdr-0.0.4/src/datamart_yhdr/interface.py` & `datamart_yhdr-0.0.5/src/datamart_yhdr/interface.py`

 * *Files 12% similar despite different names*

```diff
@@ -62,39 +62,33 @@
         if "data" in get_query:
             data.extend(get_query["data"])
             return data
         if "value" in get_query:
             data.extend(get_query["value"])
         return data
 
-    def submit_command(self, command: str, data: list):
+    def submit_command(self, command: str, data: list, silent_mode=False):
         """
 
-        :param data:
-        :param command:
+        :param silent_mode: 无通报模式
+        :param data: 发送数据
+        :param command: 触发指令
         :return:
         """
         command_params = {"code": command}
         for item in data:
             command_params.update({"args": item})
             sub = requests.post(self.command_url, headers={'Authorization': self.token}, json=command_params).json()
 
             if "success" in sub:
                 if not sub["success"]:
                     raise ConnectionAbortedError(f"请求失败，请检查操作入参。\n失败条目：{item}\n备注：{sub.get('remarks')}")
                 else:
-                    print(f"请求成功。\n入参：{item}\n请求结果：{sub.get('remarks')}")
+                    if not silent_mode:
+                        print(f"请求成功。\n入参：{item}\n请求结果：{sub.get('remarks')}")
             else:
                 raise ConnectionError("请求失败，未知原因。")
         return True
 
 
 if __name__ == '__main__':
-    dr = DMInterface("admin", "YHDR@20221206")
-    trade_date = "2023-02-13"
-    dm_GetPos = dr.get_query("dm_GetPos", limit=-1,
-                             args={"StartDate": trade_date, "EndDate": trade_date, 'FrontSource': "EXCSpot"})
-    count_53378 = 0
-    for item in dm_GetPos:
-        if item["ExternalAccountNumber"] == "53378":
-            count_53378 += 1
-    print(count_53378)
+    print("Hello!")
```

### Comparing `datamart_yhdr-0.0.4/tests/datamart_yhdr-0.0.1-py3-none-any.whl` & `datamart_yhdr-0.0.5/tests/datamart_yhdr-0.0.1-py3-none-any.whl`

 * *Files identical despite different names*

### Comparing `datamart_yhdr-0.0.4/tests/datamart_yhdr-0.0.1.tar.gz` & `datamart_yhdr-0.0.5/tests/datamart_yhdr-0.0.1.tar.gz`

 * *Files identical despite different names*

### Comparing `datamart_yhdr-0.0.4/tests/datamart_yhdr-0.0.2-py3-none-any.whl` & `datamart_yhdr-0.0.5/tests/datamart_yhdr-0.0.2-py3-none-any.whl`

 * *Files identical despite different names*

### Comparing `datamart_yhdr-0.0.4/tests/datamart_yhdr-0.0.2.tar.gz` & `datamart_yhdr-0.0.5/tests/datamart_yhdr-0.0.2.tar.gz`

 * *Files identical despite different names*

### Comparing `datamart_yhdr-0.0.4/tests/datamart_yhdr-0.0.3-py3-none-any.whl` & `datamart_yhdr-0.0.5/tests/datamart_yhdr-0.0.3-py3-none-any.whl`

 * *Files identical despite different names*

### Comparing `datamart_yhdr-0.0.4/tests/datamart_yhdr-0.0.3.tar.gz` & `datamart_yhdr-0.0.5/tests/datamart_yhdr-0.0.3.tar.gz`

 * *Files identical despite different names*

### Comparing `datamart_yhdr-0.0.4/LICENSE` & `datamart_yhdr-0.0.5/LICENSE`

 * *Files identical despite different names*

### Comparing `datamart_yhdr-0.0.4/pyproject.toml` & `datamart_yhdr-0.0.5/pyproject.toml`

 * *Files 16% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["hatchling", "requests"]
 build-backend = "hatchling.build"
 
 [project]
 name = "datamart_yhdr"
-version = "0.0.4"
+version = "0.0.5"
 authors = [
   { name="Shihua Huang", email="huangshihua@galaxyderivatives.com" },
 ]
 description = "A data interface package developed for Galaxy Derivatives Data Mart"
 readme = "README.md"
 requires-python = ">=3.6"
 classifiers = [
```

### Comparing `datamart_yhdr-0.0.4/PKG-INFO` & `datamart_yhdr-0.0.5/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: datamart_yhdr
-Version: 0.0.4
+Version: 0.0.5
 Summary: A data interface package developed for Galaxy Derivatives Data Mart
 Project-URL: Homepage, https://galaxyderivatives.feishu.cn/wiki/wikcn6BhNvlpE8yOCmkjmJHTWHe
 Project-URL: Documentation, https://galaxyderivatives.feishu.cn/wiki/wikcnjOa3s7OQ06v82CzXHBDqUd
 Author-email: Shihua Huang <huangshihua@galaxyderivatives.com>
 License-File: LICENSE
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

