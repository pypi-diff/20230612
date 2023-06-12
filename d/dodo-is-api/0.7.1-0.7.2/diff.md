# Comparing `tmp/dodo_is_api-0.7.1.tar.gz` & `tmp/dodo_is_api-0.7.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dodo_is_api-0.7.1.tar", max compression
+gzip compressed data, was "dodo_is_api-0.7.2.tar", max compression
```

## Comparing `dodo_is_api-0.7.1.tar` & `dodo_is_api-0.7.2.tar`

### file list

```diff
@@ -1,25 +1,25 @@
--rw-r--r--   0        0        0     1075 2023-03-22 13:32:15.868970 dodo_is_api-0.7.1/LICENSE
--rw-r--r--   0        0        0     2689 2023-06-11 19:00:32.393182 dodo_is_api-0.7.1/README.md
--rw-r--r--   0        0        0        0 2023-03-18 06:06:54.111388 dodo_is_api-0.7.1/dodo_is_api/__init__.py
--rw-r--r--   0        0        0       55 2023-05-10 05:26:32.091241 dodo_is_api-0.7.1/dodo_is_api/connection/__init__.py
--rw-r--r--   0        0        0    16088 2023-06-11 18:35:09.363455 dodo_is_api-0.7.1/dodo_is_api/connection/asynchronous.py
--rw-r--r--   0        0        0     3055 2023-06-11 18:22:28.674699 dodo_is_api-0.7.1/dodo_is_api/connection/base.py
--rw-r--r--   0        0        0    15937 2023-06-11 18:35:09.368594 dodo_is_api-0.7.1/dodo_is_api/connection/synchronous.py
--rw-r--r--   0        0        0      248 2023-03-18 06:06:54.113625 dodo_is_api-0.7.1/dodo_is_api/exceptions.py
--rw-r--r--   0        0        0      583 2023-06-11 08:10:22.290413 dodo_is_api-0.7.1/dodo_is_api/logger.py
--rw-r--r--   0        0        0      419 2023-06-11 13:11:06.903175 dodo_is_api-0.7.1/dodo_is_api/models/__init__.py
--rw-r--r--   0        0        0      149 2023-06-11 08:39:51.057307 dodo_is_api-0.7.1/dodo_is_api/models/channel_stop_types.py
--rw-r--r--   0        0        0      349 2023-06-11 08:21:43.504521 dodo_is_api-0.7.1/dodo_is_api/models/country_codes.py
--rw-r--r--   0        0        0     1551 2023-06-11 20:17:46.220836 dodo_is_api-0.7.1/dodo_is_api/models/courier_orders.py
--rw-r--r--   0        0        0     1068 2023-06-11 20:17:46.212257 dodo_is_api-0.7.1/dodo_is_api/models/delivery_statistics.py
--rw-r--r--   0        0        0      174 2023-06-11 08:41:14.500495 dodo_is_api-0.7.1/dodo_is_api/models/delivery_transport_names.py
--rw-r--r--   0        0        0      860 2023-06-11 20:17:46.224929 dodo_is_api-0.7.1/dodo_is_api/models/late_delivery_vouchers.py
--rw-r--r--   0        0        0      308 2023-06-11 13:11:06.905522 dodo_is_api-0.7.1/dodo_is_api/models/order_sources.py
--rw-r--r--   0        0        0      647 2023-06-11 20:19:11.590789 dodo_is_api-0.7.1/dodo_is_api/models/orders_handover_statistics.py
--rw-r--r--   0        0        0      869 2023-06-11 20:19:11.594036 dodo_is_api-0.7.1/dodo_is_api/models/orders_handover_time.py
--rw-r--r--   0        0        0      781 2023-06-11 20:19:11.596459 dodo_is_api-0.7.1/dodo_is_api/models/production_productivity_statistics.py
--rw-r--r--   0        0        0      161 2023-06-11 08:37:28.682394 dodo_is_api-0.7.1/dodo_is_api/models/sales_channels.py
--rw-r--r--   0        0        0     1115 2023-06-11 20:19:11.598966 dodo_is_api-0.7.1/dodo_is_api/models/stop_sales.py
--rw-r--r--   0        0        0      582 2023-06-11 20:19:59.428652 dodo_is_api-0.7.1/pyproject.toml
--rw-r--r--   0        0        0     3521 1970-01-01 00:00:00.000000 dodo_is_api-0.7.1/setup.py
--rw-r--r--   0        0        0     3105 1970-01-01 00:00:00.000000 dodo_is_api-0.7.1/PKG-INFO
+-rw-r--r--   0        0        0     1075 2023-03-22 13:32:15.868970 dodo_is_api-0.7.2/LICENSE
+-rw-r--r--   0        0        0     2689 2023-06-11 19:00:32.393182 dodo_is_api-0.7.2/README.md
+-rw-r--r--   0        0        0        0 2023-03-18 06:06:54.111388 dodo_is_api-0.7.2/dodo_is_api/__init__.py
+-rw-r--r--   0        0        0       55 2023-05-10 05:26:32.091241 dodo_is_api-0.7.2/dodo_is_api/connection/__init__.py
+-rw-r--r--   0        0        0    16088 2023-06-11 18:35:09.363455 dodo_is_api-0.7.2/dodo_is_api/connection/asynchronous.py
+-rw-r--r--   0        0        0     3160 2023-06-12 05:17:25.385543 dodo_is_api-0.7.2/dodo_is_api/connection/base.py
+-rw-r--r--   0        0        0    15937 2023-06-11 18:35:09.368594 dodo_is_api-0.7.2/dodo_is_api/connection/synchronous.py
+-rw-r--r--   0        0        0      248 2023-03-18 06:06:54.113625 dodo_is_api-0.7.2/dodo_is_api/exceptions.py
+-rw-r--r--   0        0        0      583 2023-06-11 08:10:22.290413 dodo_is_api-0.7.2/dodo_is_api/logger.py
+-rw-r--r--   0        0        0      419 2023-06-11 13:11:06.903175 dodo_is_api-0.7.2/dodo_is_api/models/__init__.py
+-rw-r--r--   0        0        0      149 2023-06-11 08:39:51.057307 dodo_is_api-0.7.2/dodo_is_api/models/channel_stop_types.py
+-rw-r--r--   0        0        0      349 2023-06-11 08:21:43.504521 dodo_is_api-0.7.2/dodo_is_api/models/country_codes.py
+-rw-r--r--   0        0        0     1551 2023-06-11 20:17:46.220836 dodo_is_api-0.7.2/dodo_is_api/models/courier_orders.py
+-rw-r--r--   0        0        0     1068 2023-06-11 20:17:46.212257 dodo_is_api-0.7.2/dodo_is_api/models/delivery_statistics.py
+-rw-r--r--   0        0        0      174 2023-06-11 08:41:14.500495 dodo_is_api-0.7.2/dodo_is_api/models/delivery_transport_names.py
+-rw-r--r--   0        0        0      860 2023-06-11 20:17:46.224929 dodo_is_api-0.7.2/dodo_is_api/models/late_delivery_vouchers.py
+-rw-r--r--   0        0        0      308 2023-06-11 13:11:06.905522 dodo_is_api-0.7.2/dodo_is_api/models/order_sources.py
+-rw-r--r--   0        0        0      647 2023-06-11 20:19:11.590789 dodo_is_api-0.7.2/dodo_is_api/models/orders_handover_statistics.py
+-rw-r--r--   0        0        0      869 2023-06-11 20:19:11.594036 dodo_is_api-0.7.2/dodo_is_api/models/orders_handover_time.py
+-rw-r--r--   0        0        0      781 2023-06-11 20:19:11.596459 dodo_is_api-0.7.2/dodo_is_api/models/production_productivity_statistics.py
+-rw-r--r--   0        0        0      161 2023-06-11 08:37:28.682394 dodo_is_api-0.7.2/dodo_is_api/models/sales_channels.py
+-rw-r--r--   0        0        0     1115 2023-06-11 20:19:11.598966 dodo_is_api-0.7.2/dodo_is_api/models/stop_sales.py
+-rw-r--r--   0        0        0      582 2023-06-12 05:23:52.281457 dodo_is_api-0.7.2/pyproject.toml
+-rw-r--r--   0        0        0     3521 1970-01-01 00:00:00.000000 dodo_is_api-0.7.2/setup.py
+-rw-r--r--   0        0        0     3105 1970-01-01 00:00:00.000000 dodo_is_api-0.7.2/PKG-INFO
```

### Comparing `dodo_is_api-0.7.1/LICENSE` & `dodo_is_api-0.7.2/LICENSE`

 * *Files identical despite different names*

### Comparing `dodo_is_api-0.7.1/README.md` & `dodo_is_api-0.7.2/README.md`

 * *Files identical despite different names*

### Comparing `dodo_is_api-0.7.1/dodo_is_api/connection/asynchronous.py` & `dodo_is_api-0.7.2/dodo_is_api/connection/asynchronous.py`

 * *Files identical despite different names*

### Comparing `dodo_is_api-0.7.1/dodo_is_api/connection/base.py` & `dodo_is_api-0.7.2/dodo_is_api/connection/base.py`

 * *Files 9% similar despite different names*

```diff
@@ -11,18 +11,14 @@
     'build_request_query_params',
     'concatenate_uuids',
     'raise_for_status',
     'BaseDodoISAPIConnection',
 )
 
 
-def kebab_case_to_pascal_case(text: str) -> str:
-    return ''.join(word.capitalize() for word in text.split('-'))
-
-
 def concatenate_uuids(uuids: Iterable[UUID], join_symbol: str = ',') -> str:
     """Convert UUIDs collection to UUIDs string suitable for Dodo IS API.
 
     Examples:
          >>> concatenate_uuids([UUID('6ff7d64d-1457-47f2-a396-1174994c1e20'), UUID('e27b64cf-346f-4f69-817c-c8ccd4814826')])
          '6ff7d64d145747f2a3961174994c1e20,e27b64cf346f4f69817cc8ccd4814826'
 
@@ -56,18 +52,25 @@
 
     if take is not None:
         query_params['take'] = take
     if skip is not None:
         query_params['skip'] = skip
 
     if sales_channels is not None:
-        query_params['salesChannels'] = ','.join(
-            kebab_case_to_pascal_case(sales_channel)
-            for sales_channel in sales_channels
-        )
+        sales_channel_to_request_query_param = {
+            models.SalesChannel.DINE_IN: 'DineIn',
+            models.SalesChannel.TAKEAWAY: 'TakeAway',
+        }
+
+        query_params['salesChannels'] = [
+            sales_channel_to_request_query_param.get(
+                sales_channel,
+                sales_channel,
+            ) for sales_channel in sales_channels
+        ]
 
     return query_params
 
 
 def raise_for_status(response: httpx.Response) -> None:
     if response.is_success:
         return
```

### Comparing `dodo_is_api-0.7.1/dodo_is_api/connection/synchronous.py` & `dodo_is_api-0.7.2/dodo_is_api/connection/synchronous.py`

 * *Files identical despite different names*

### Comparing `dodo_is_api-0.7.1/dodo_is_api/logger.py` & `dodo_is_api-0.7.2/dodo_is_api/logger.py`

 * *Files identical despite different names*

### Comparing `dodo_is_api-0.7.1/dodo_is_api/models/courier_orders.py` & `dodo_is_api-0.7.2/dodo_is_api/models/courier_orders.py`

 * *Files identical despite different names*

### Comparing `dodo_is_api-0.7.1/dodo_is_api/models/delivery_statistics.py` & `dodo_is_api-0.7.2/dodo_is_api/models/delivery_statistics.py`

 * *Files identical despite different names*

### Comparing `dodo_is_api-0.7.1/dodo_is_api/models/late_delivery_vouchers.py` & `dodo_is_api-0.7.2/dodo_is_api/models/late_delivery_vouchers.py`

 * *Files identical despite different names*

### Comparing `dodo_is_api-0.7.1/dodo_is_api/models/orders_handover_statistics.py` & `dodo_is_api-0.7.2/dodo_is_api/models/orders_handover_statistics.py`

 * *Files identical despite different names*

### Comparing `dodo_is_api-0.7.1/dodo_is_api/models/orders_handover_time.py` & `dodo_is_api-0.7.2/dodo_is_api/models/orders_handover_time.py`

 * *Files identical despite different names*

### Comparing `dodo_is_api-0.7.1/dodo_is_api/models/production_productivity_statistics.py` & `dodo_is_api-0.7.2/dodo_is_api/models/production_productivity_statistics.py`

 * *Files identical despite different names*

### Comparing `dodo_is_api-0.7.1/dodo_is_api/models/stop_sales.py` & `dodo_is_api-0.7.2/dodo_is_api/models/stop_sales.py`

 * *Files identical despite different names*

### Comparing `dodo_is_api-0.7.1/pyproject.toml` & `dodo_is_api-0.7.2/pyproject.toml`

 * *Files 24% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "dodo-is-api"
-version = "0.7.1"
+version = "0.7.2"
 description = ""
 authors = ["Eldos <eldos.baktybekov@gmail.com>"]
 readme = "README.md"
 packages = [{include = "dodo_is_api"}]
 
 [tool.poetry.dependencies]
 python = "^3.11"
```

### Comparing `dodo_is_api-0.7.1/setup.py` & `dodo_is_api-0.7.2/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -10,15 +10,15 @@
 install_requires = \
 ['httpx>=0.23.3,<0.24.0',
  'pydantic>=1.10.9,<2.0.0',
  'structlog>=23.1.0,<24.0.0']
 
 setup_kwargs = {
     'name': 'dodo-is-api',
-    'version': '0.7.1',
+    'version': '0.7.2',
     'description': '',
     'long_description': '<h1 align="center">\n🍕 Dodo IS API Wrapper\n</h1>\n\n<p align="center">\n<a href="https://github.com/goretsky-integration/dodo-is-api-python-wrapper/actions/workflows/unittest.yaml">\n<img src="https://github.com/goretsky-integration/dodo-is-api-python-wrapper/actions/workflows/unittest.yaml/badge.svg" alt="Test badge">\n</a>\n<a href="https://codecov.io/gh/goretsky-integration/dodo-is-api-python-wrapper">\n<img src="https://codecov.io/gh/goretsky-integration/dodo-is-api-python-wrapper/branch/main/graph/badge.svg?token=unzlMmAjsD"/>\n</a>\n<img src="https://img.shields.io/badge/python-3.11-brightgreen" alt="python">\n</p>\n\n---\n\n### Installation\n\nVia pip:\n\n```shell\npip install dodo-is-api\n```\n\nVia poetry:\n\n```shell\npoetry add dodo-is-api\n```\n\n---\n\n#### 📝 [Changelog](https://github.com/goretsky-integration/dodo-is-api-python-wrapper/blob/main/CHANGELOG.md) is here.\n\n---\n\n### 🧪 Usage:\n\n🌩️ Synchronous version:\n\n```python\nfrom datetime import datetime\nfrom uuid import UUID\n\nimport httpx\n\nfrom dodo_is_api import models\nfrom dodo_is_api.connection.synchronous import DodoISAPIConnection\n\n\ndef main():\n    access_token = \'your access token\'\n    country_code = models.CountryCode.RU\n\n    from_date = datetime(2004, 10, 7)\n    to_date = datetime(2004, 10, 7, 23)\n    units = [UUID(\'ec81831c-b8a7-4ba8-a6aa-7ae7d0c4e0bb\')]\n\n    with httpx.Client() as http_client:\n        connection = DodoISAPIConnection(\n            http_client=http_client,\n            access_token=access_token,\n            country_code=country_code,\n        )\n\n        stop_sales = connection.get_stop_sales_by_products(\n            from_date=from_date,\n            to_date=to_date,\n            units=units,\n        )\n\n    print(stop_sales)\n\n\nif __name__ == \'__main__\':\n    main()\n```\n\n⚡️ Asynchronous version:\n\n```python\nimport asyncio\nfrom datetime import datetime\nfrom uuid import UUID\n\nimport httpx\n\nfrom dodo_is_api import models\nfrom dodo_is_api.connection.asynchronous import AsyncDodoISAPIConnection\n\n\nasync def main():\n    access_token = \'your access token\'\n    country_code = models.CountryCode.RU\n\n    from_date = datetime(2004, 10, 7)\n    to_date = datetime(2004, 10, 7, 23)\n    units = [UUID(\'ec81831c-b8a7-4ba8-a6aa-7ae7d0c4e0bb\')]\n\n    with httpx.AsyncClient() as http_client:\n        connection = AsyncDodoISAPIConnection(\n            http_client=http_client,\n            access_token=access_token,\n            country_code=country_code,\n        )\n\n        stop_sales = await connection.get_stop_sales_by_products(\n            from_date=from_date,\n            to_date=to_date,\n            units=units,\n        )\n\n    print(stop_sales)\n\n\nif __name__ == \'__main__\':\n    asyncio.run(main())\n```',
     'author': 'Eldos',
     'author_email': 'eldos.baktybekov@gmail.com',
     'maintainer': 'None',
     'maintainer_email': 'None',
     'url': 'None',
```

#### html2text {}

```diff
@@ -1,12 +1,12 @@
 # -*- coding: utf-8 -*- from setuptools import setup packages = \
 ['dodo_is_api', 'dodo_is_api.connection', 'dodo_is_api.models'] package_data =
 \ {'': ['*']} install_requires = \ ['httpx>=0.23.3,<0.24.0',
 'pydantic>=1.10.9,<2.0.0', 'structlog>=23.1.0,<24.0.0'] setup_kwargs =
-{ 'name': 'dodo-is-api', 'version': '0.7.1', 'description': '',
+{ 'name': 'dodo-is-api', 'version': '0.7.2', 'description': '',
 'long_description': '
                   ****** \nð Dodo IS API Wrapper\n ******
 \n\n
 \n\n[Test_badge]\n\n\n[https://codecov.io/gh/goretsky-integration/dodo-is-api-
   python-wrapper/branch/main/graph/badge.svg?token=unzlMmAjsD]\n\n[python]\n
 \n\n---\n\n### Installation\n\nVia pip:\n\n```shell\npip install dodo-is-
 api\n```\n\nVia poetry:\n\n```shell\npoetry add dodo-is-api\n```\n\n---\n\n####
```

### Comparing `dodo_is_api-0.7.1/PKG-INFO` & `dodo_is_api-0.7.2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dodo-is-api
-Version: 0.7.1
+Version: 0.7.2
 Summary: 
 Author: Eldos
 Author-email: eldos.baktybekov@gmail.com
 Requires-Python: >=3.11,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.11
 Requires-Dist: httpx (>=0.23.3,<0.24.0)
```

