# Comparing `tmp/python_strategies_breezeconnect-2.0.tar.gz` & `tmp/python_strategies_breezeconnect-3.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "python_strategies_breezeconnect-2.0.tar", last modified: Fri Jun  9 09:43:09 2023, max compression
+gzip compressed data, was "python_strategies_breezeconnect-3.0.tar", last modified: Mon Jun 12 04:09:56 2023, max compression
```

## Comparing `python_strategies_breezeconnect-2.0.tar` & `python_strategies_breezeconnect-3.0.tar`

### file list

```diff
@@ -1,15 +1,15 @@
-drwxrwxrwx   0        0        0        0 2023-06-09 09:43:09.946557 python_strategies_breezeconnect-2.0/
--rw-rw-rw-   0        0        0     1113 2023-06-09 09:29:34.000000 python_strategies_breezeconnect-2.0/LICENSE
--rw-rw-rw-   0        0        0     1274 2023-06-09 09:43:09.941171 python_strategies_breezeconnect-2.0/PKG-INFO
--rw-rw-rw-   0        0        0      749 2023-06-09 09:42:38.000000 python_strategies_breezeconnect-2.0/README.md
-drwxrwxrwx   0        0        0        0 2023-06-09 09:43:09.896136 python_strategies_breezeconnect-2.0/python_strategies/
--rw-rw-rw-   0        0        0       58 2023-06-09 09:24:56.000000 python_strategies_breezeconnect-2.0/python_strategies/__init__.py
--rw-rw-rw-   0        0        0    18215 2023-06-09 09:43:03.000000 python_strategies_breezeconnect-2.0/python_strategies/python_strategies.py
-drwxrwxrwx   0        0        0        0 2023-06-09 09:43:09.937172 python_strategies_breezeconnect-2.0/python_strategies_breezeconnect.egg-info/
--rw-rw-rw-   0        0        0     1274 2023-06-09 09:43:09.000000 python_strategies_breezeconnect-2.0/python_strategies_breezeconnect.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      369 2023-06-09 09:43:09.000000 python_strategies_breezeconnect-2.0/python_strategies_breezeconnect.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-06-09 09:43:09.000000 python_strategies_breezeconnect-2.0/python_strategies_breezeconnect.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       32 2023-06-09 09:43:09.000000 python_strategies_breezeconnect-2.0/python_strategies_breezeconnect.egg-info/requires.txt
--rw-rw-rw-   0        0        0       18 2023-06-09 09:43:09.000000 python_strategies_breezeconnect-2.0/python_strategies_breezeconnect.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-06-09 09:43:09.947927 python_strategies_breezeconnect-2.0/setup.cfg
--rw-rw-rw-   0        0        0      787 2023-06-09 09:41:39.000000 python_strategies_breezeconnect-2.0/setup.py
+drwxrwxrwx   0        0        0        0 2023-06-12 04:09:56.861990 python_strategies_breezeconnect-3.0/
+-rw-rw-rw-   0        0        0     1113 2023-06-09 09:29:34.000000 python_strategies_breezeconnect-3.0/LICENSE
+-rw-rw-rw-   0        0        0     1113 2023-06-12 04:09:56.855931 python_strategies_breezeconnect-3.0/PKG-INFO
+-rw-rw-rw-   0        0        0      588 2023-06-12 04:09:43.000000 python_strategies_breezeconnect-3.0/README.md
+drwxrwxrwx   0        0        0        0 2023-06-12 04:09:56.761624 python_strategies_breezeconnect-3.0/python_strategies/
+-rw-rw-rw-   0        0        0       58 2023-06-09 09:24:56.000000 python_strategies_breezeconnect-3.0/python_strategies/__init__.py
+-rw-rw-rw-   0        0        0    18682 2023-06-09 12:26:53.000000 python_strategies_breezeconnect-3.0/python_strategies/python_strategies.py
+drwxrwxrwx   0        0        0        0 2023-06-12 04:09:56.850774 python_strategies_breezeconnect-3.0/python_strategies_breezeconnect.egg-info/
+-rw-rw-rw-   0        0        0     1113 2023-06-12 04:09:56.000000 python_strategies_breezeconnect-3.0/python_strategies_breezeconnect.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      369 2023-06-12 04:09:56.000000 python_strategies_breezeconnect-3.0/python_strategies_breezeconnect.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-06-12 04:09:56.000000 python_strategies_breezeconnect-3.0/python_strategies_breezeconnect.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       32 2023-06-12 04:09:56.000000 python_strategies_breezeconnect-3.0/python_strategies_breezeconnect.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       18 2023-06-12 04:09:56.000000 python_strategies_breezeconnect-3.0/python_strategies_breezeconnect.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-06-12 04:09:56.863995 python_strategies_breezeconnect-3.0/setup.cfg
+-rw-rw-rw-   0        0        0      787 2023-06-09 12:19:14.000000 python_strategies_breezeconnect-3.0/setup.py
```

### Comparing `python_strategies_breezeconnect-2.0/LICENSE` & `python_strategies_breezeconnect-3.0/LICENSE`

 * *Files identical despite different names*

### Comparing `python_strategies_breezeconnect-2.0/PKG-INFO` & `python_strategies_breezeconnect-3.0/python_strategies_breezeconnect.egg-info/PKG-INFO`

 * *Files 13% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
-Name: python_strategies_breezeconnect
-Version: 2.0
+Name: python-strategies-breezeconnect
+Version: 3.0
 Summary: breeze connect strategies in python
 Home-page: https://github.com/pypa/sampleproject
 Author: UAT python strategy Breeze Connect
 Author-email: test@mail.com
 License: UNKNOWN
 Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3
@@ -17,29 +17,28 @@
 # UAT  python_strategies
 
 ## Steps to install Strategy Library for UAT
 
 
 ```python
 
-pip install python_strategies_breezeconnect==2.0
+pip install python_strategies_breezeconnect==3.0
 
 ```
 
 
 ## code usage
 
 ```python
 
 from python_strategies import Strategies
 
 async def main():
     obj = Strategies(app_key = "your app key",secret_key = "your secret key",api_session = "your api session",max_profit = "your max profit",max_loss = "your max loss")
-    await obj.long_straddle(product_type = "options", stock_code = "NIFTY",strike_price = "18700",qty = "50",expiry_date = "2023-06-15T06:00:00.000Z",order_type = "market",validity = "day",validity_date = 
-    "2023-06-09T06:00:00.000Z",exchange_code = "NFO",stoploss = "",put_price = "0",call_price = "0")
+    await obj.long_straddle(stock_code = "NIFTY",strike_price = "18700",qty = "50",expiry_date = "2023-06-15T06:00:00.000Z",exchange_code = "NFO")
 
 await main()
 
 ```
```

### Comparing `python_strategies_breezeconnect-2.0/python_strategies/python_strategies.py` & `python_strategies_breezeconnect-3.0/python_strategies/python_strategies.py`

 * *Files 2% similar despite different names*

```diff
@@ -2,14 +2,16 @@
 import queue
 import time 
 #import datetime
 import sys
 import asyncio
 import nest_asyncio
 from breeze_connect import BreezeConnect
+from datetime import datetime
+
 nest_asyncio.apply()
 
 class Strategies:
     
     #initialize strategy object
     def __init__(self,app_key,secret_key,api_session,max_profit,max_loss):
         
@@ -154,15 +156,15 @@
         #task1 = asyncio.create_task(perform_operation1())
         #task2 = asyncio.create_task(perform_operation2())
 
         # Wait for all tasks to complete
         await asyncio.gather(p1, p2)
         
         
-    async def long_straddle(self, product_type, stock_code, strike_price, qty, expiry_date, order_type, validity, validity_date, exchange_code, stoploss, put_price, call_price):
+    async def long_straddle(self, product_type = "options", stock_code, strike_price, qty, expiry_date, order_type = "market", validity = "day", validity_date = datetime.utcnow().strftime('%Y-%m-%dT%H:%M:%S.%fZ'), exchange_code, stoploss = "", put_price = "0", call_price = "0"):
         def place_order_method(stock_code,exchange_code,product,action,order_type,stoploss,quantity,price,validity,validity_date,expiry_date,right,strike_price,res_queue):
          
             data =  self.client.place_order(stock_code=stock_code,
                     exchange_code=exchange_code,
                     product="options",
                     action = "buy",
                     order_type=order_type,
@@ -279,21 +281,25 @@
             for entry in details['Success']:
                 if(entry['status'] == "Executed"):
                     put_execution = entry['average_price']
                     break
                     
             if(call_execution == -1 or put_execution == -1):
                 print("Dear User order could not execute within time limit ..cancelling it")
-                if(call_execution == -1):
+                if(call_execution == -1 and put_execution == -1):
+                    pass
+
+                elif(call_execution == -1):
                     #call cancel order api
                     print("call order could not execute due to some reason so cancelling order")
+                    #self.squareoff(self,rightval,exchange_code, stock_code, product_type, expiry_date, right, strike_price, action, order_type, validity, stoploss, quantity, price,validity_date, trade_password, disclosed_quantity)
                     self.client.cancel_order(exchange_code=exchange_code,
                     order_id = orderids[0])
                     
-                if(put_execution == -1):
+                elif(put_execution == -1):
                     #call cancel order api
                     print("put order could not execute due to some reason so cancelling order")
                     status = self.client.cancel_order(exchange_code=exchange_code,
                     order_id = orderids[1])
                     
             else:
                 print("Call order got executed at price :{0} Rs and Put Order got executed at price : {1} Rs".format(call_execution,put_execution))
```

### Comparing `python_strategies_breezeconnect-2.0/setup.py` & `python_strategies_breezeconnect-3.0/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import setuptools
 
 with open("README.md", "r", encoding="utf-8") as fh:
     long_description = fh.read()
 
 setuptools.setup(
     name="python_strategies_breezeconnect",
-    version="2.0",
+    version="3.0",
     author="UAT python strategy Breeze Connect",
     author_email="test@mail.com",
     description="breeze connect strategies in python",
     long_description=long_description,
     long_description_content_type="text/markdown",
     install_requires=['uat-breeze-connect','nest_asyncio'],
     url="https://github.com/pypa/sampleproject",
```

