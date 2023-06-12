# Comparing `tmp/stripe_api_client-0.1.2.tar.gz` & `tmp/stripe_api_client-0.1.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "stripe_api_client-0.1.2.tar", max compression
+gzip compressed data, was "stripe_api_client-0.1.3.tar", max compression
```

## Comparing `stripe_api_client-0.1.2.tar` & `stripe_api_client-0.1.3.tar`

### file list

```diff
@@ -1,15 +1,15 @@
--rw-r--r--   0        0        0        0 2023-06-07 10:16:48.295067 stripe_api_client-0.1.2/README.md
--rw-r--r--   0        0        0      343 2023-06-11 12:25:38.121181 stripe_api_client-0.1.2/pyproject.toml
--rw-r--r--   0        0        0       26 2023-06-07 10:30:36.351871 stripe_api_client-0.1.2/stripe_api_client/__init__.py
--rw-r--r--   0        0        0     2054 2023-06-09 12:54:09.952976 stripe_api_client-0.1.2/stripe_api_client/client.py
--rw-r--r--   0        0        0      266 2023-06-09 12:12:59.578367 stripe_api_client-0.1.2/stripe_api_client/resources/__init__.py
--rw-r--r--   0        0        0     1412 2023-06-07 10:39:02.667985 stripe_api_client-0.1.2/stripe_api_client/resources/base.py
--rw-r--r--   0        0        0      538 2023-06-07 10:43:23.129565 stripe_api_client-0.1.2/stripe_api_client/resources/charges.py
--rw-r--r--   0        0        0     1093 2023-06-07 10:52:35.422836 stripe_api_client-0.1.2/stripe_api_client/resources/customers.py
--rw-r--r--   0        0        0     1728 2023-06-09 12:10:34.150731 stripe_api_client-0.1.2/stripe_api_client/resources/invoices.py
--rw-r--r--   0        0        0     1158 2023-06-09 11:55:29.570309 stripe_api_client-0.1.2/stripe_api_client/resources/payment_intents.py
--rw-r--r--   0        0        0      589 2023-06-07 10:50:26.654229 stripe_api_client-0.1.2/stripe_api_client/resources/payment_methods.py
--rw-r--r--   0        0        0      570 2023-06-09 12:12:50.834821 stripe_api_client-0.1.2/stripe_api_client/resources/subscriptions.py
--rw-r--r--   0        0        0      255 2023-06-07 10:20:06.632274 stripe_api_client-0.1.2/stripe_api_client/utils.py
--rw-r--r--   0        0        0      642 1970-01-01 00:00:00.000000 stripe_api_client-0.1.2/setup.py
--rw-r--r--   0        0        0      439 1970-01-01 00:00:00.000000 stripe_api_client-0.1.2/PKG-INFO
+-rw-r--r--   0        0        0        0 2023-06-07 10:16:48.295067 stripe_api_client-0.1.3/README.md
+-rw-r--r--   0        0        0      343 2023-06-12 12:42:17.142817 stripe_api_client-0.1.3/pyproject.toml
+-rw-r--r--   0        0        0       26 2023-06-07 10:30:36.351871 stripe_api_client-0.1.3/stripe_api_client/__init__.py
+-rw-r--r--   0        0        0     2054 2023-06-09 12:54:09.952976 stripe_api_client-0.1.3/stripe_api_client/client.py
+-rw-r--r--   0        0        0      266 2023-06-09 12:12:59.578367 stripe_api_client-0.1.3/stripe_api_client/resources/__init__.py
+-rw-r--r--   0        0        0     1412 2023-06-07 10:39:02.667985 stripe_api_client-0.1.3/stripe_api_client/resources/base.py
+-rw-r--r--   0        0        0      538 2023-06-07 10:43:23.129565 stripe_api_client-0.1.3/stripe_api_client/resources/charges.py
+-rw-r--r--   0        0        0     1093 2023-06-07 10:52:35.422836 stripe_api_client-0.1.3/stripe_api_client/resources/customers.py
+-rw-r--r--   0        0        0     1728 2023-06-09 12:10:34.150731 stripe_api_client-0.1.3/stripe_api_client/resources/invoices.py
+-rw-r--r--   0        0        0     1387 2023-06-12 12:41:42.832049 stripe_api_client-0.1.3/stripe_api_client/resources/payment_intents.py
+-rw-r--r--   0        0        0      589 2023-06-07 10:50:26.654229 stripe_api_client-0.1.3/stripe_api_client/resources/payment_methods.py
+-rw-r--r--   0        0        0      570 2023-06-09 12:12:50.834821 stripe_api_client-0.1.3/stripe_api_client/resources/subscriptions.py
+-rw-r--r--   0        0        0      255 2023-06-07 10:20:06.632274 stripe_api_client-0.1.3/stripe_api_client/utils.py
+-rw-r--r--   0        0        0      642 1970-01-01 00:00:00.000000 stripe_api_client-0.1.3/setup.py
+-rw-r--r--   0        0        0      439 1970-01-01 00:00:00.000000 stripe_api_client-0.1.3/PKG-INFO
```

### Comparing `stripe_api_client-0.1.2/stripe_api_client/client.py` & `stripe_api_client-0.1.3/stripe_api_client/client.py`

 * *Files identical despite different names*

### Comparing `stripe_api_client-0.1.2/stripe_api_client/resources/base.py` & `stripe_api_client-0.1.3/stripe_api_client/resources/base.py`

 * *Files identical despite different names*

### Comparing `stripe_api_client-0.1.2/stripe_api_client/resources/charges.py` & `stripe_api_client-0.1.3/stripe_api_client/resources/charges.py`

 * *Files identical despite different names*

### Comparing `stripe_api_client-0.1.2/stripe_api_client/resources/customers.py` & `stripe_api_client-0.1.3/stripe_api_client/resources/customers.py`

 * *Files identical despite different names*

### Comparing `stripe_api_client-0.1.2/stripe_api_client/resources/invoices.py` & `stripe_api_client-0.1.3/stripe_api_client/resources/invoices.py`

 * *Files identical despite different names*

### Comparing `stripe_api_client-0.1.2/stripe_api_client/resources/payment_intents.py` & `stripe_api_client-0.1.3/stripe_api_client/resources/payment_intents.py`

 * *Files 24% similar despite different names*

```diff
@@ -7,37 +7,43 @@
     base.ResourcePool,
     base.CreatableResource,
     base.GettableResource,
     base.ListableResource,
     base.UpdatableResource
 ):
     
+    @property
+    def search(self):
+        return base.QueryPool(
+            urljoin(self._endpoint, 'search'), self._session
+        )
+
     def confirm(self, pi_id):
         return base.ActionPool(
-            urljoin(self._endpoint, pi_id, 'confirm')
+            urljoin(self._endpoint, pi_id, 'confirm'), self._session
         )
     
     def capture(self, pi_id):
         return base.ActionPool(
-            urljoin(self._endpoint, pi_id, 'capture')
+            urljoin(self._endpoint, pi_id, 'capture'), self._session
         )
 
     def cancel(self, pi_id):
         return base.ActionPool(
-            urljoin(self._endpoint, pi_id, 'cancel')
+            urljoin(self._endpoint, pi_id, 'cancel'), self._session
         )        
     
     def increment_authorization(self, pi_id):
         return base.ActionPool(
-            urljoin(self._endpoint, pi_id, 'increment_authorization')
+            urljoin(self._endpoint, pi_id, 'increment_authorization'), self._session
         )        
 
     def verify_microdeposits(self, pi_id):
         return base.ActionPool(
-            urljoin(self._endpoint, pi_id, 'verify_microdeposits')
+            urljoin(self._endpoint, pi_id, 'verify_microdeposits'), self._session
         )        
 
     def apply_customer_balance(self, pi_id):
         return base.ActionPool(
-            urljoin(self._endpoint, pi_id, 'apply_customer_balance')
+            urljoin(self._endpoint, pi_id, 'apply_customer_balance'), self._session
         )
```

### Comparing `stripe_api_client-0.1.2/stripe_api_client/resources/payment_methods.py` & `stripe_api_client-0.1.3/stripe_api_client/resources/payment_methods.py`

 * *Files identical despite different names*

### Comparing `stripe_api_client-0.1.2/stripe_api_client/resources/subscriptions.py` & `stripe_api_client-0.1.3/stripe_api_client/resources/subscriptions.py`

 * *Files identical despite different names*

### Comparing `stripe_api_client-0.1.2/setup.py` & `stripe_api_client-0.1.3/setup.py`

 * *Files 14% similar despite different names*

```diff
@@ -8,15 +8,15 @@
 {'': ['*']}
 
 install_requires = \
 ['requests>=2.31.0,<3.0.0']
 
 setup_kwargs = {
     'name': 'stripe-api-client',
-    'version': '0.1.2',
+    'version': '0.1.3',
     'description': '',
     'long_description': '',
     'author': 'Steven Athouel',
     'author_email': 'sathouel@gmail.com',
     'maintainer': 'None',
     'maintainer_email': 'None',
     'url': 'None',
```

