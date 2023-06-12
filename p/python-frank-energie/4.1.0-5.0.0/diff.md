# Comparing `tmp/python_frank_energie-4.1.0.tar.gz` & `tmp/python_frank_energie-5.0.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "python_frank_energie-4.1.0.tar", max compression
+gzip compressed data, was "python_frank_energie-5.0.0.tar", max compression
```

## Comparing `python_frank_energie-4.1.0.tar` & `python_frank_energie-5.0.0.tar`

### file list

```diff
@@ -1,8 +1,8 @@
--rw-r--r--   0        0        0    11346 2023-05-22 09:34:41.962801 python_frank_energie-4.1.0/LICENSE
--rw-r--r--   0        0        0      325 2023-05-22 09:34:41.962801 python_frank_energie-4.1.0/README.md
--rw-r--r--   0        0        0     2353 2023-05-22 09:35:02.079432 python_frank_energie-4.1.0/pyproject.toml
--rw-r--r--   0        0        0      175 2023-05-22 09:34:41.962801 python_frank_energie-4.1.0/python_frank_energie/__init__.py
--rw-r--r--   0        0        0      378 2023-05-22 09:34:41.962801 python_frank_energie-4.1.0/python_frank_energie/exceptions.py
--rw-r--r--   0        0        0     8256 2023-05-22 09:34:41.962801 python_frank_energie-4.1.0/python_frank_energie/frank_energie.py
--rw-r--r--   0        0        0    11198 2023-05-22 09:34:41.962801 python_frank_energie-4.1.0/python_frank_energie/models.py
--rw-r--r--   0        0        0     1217 1970-01-01 00:00:00.000000 python_frank_energie-4.1.0/PKG-INFO
+-rw-r--r--   0        0        0    11346 2023-06-12 21:41:16.326471 python_frank_energie-5.0.0/LICENSE
+-rw-r--r--   0        0        0     1442 2023-06-12 21:41:16.326471 python_frank_energie-5.0.0/README.md
+-rw-r--r--   0        0        0     2352 2023-06-12 21:41:45.992268 python_frank_energie-5.0.0/pyproject.toml
+-rw-r--r--   0        0        0      175 2023-06-12 21:41:16.330471 python_frank_energie-5.0.0/python_frank_energie/__init__.py
+-rw-r--r--   0        0        0      378 2023-06-12 21:41:16.330471 python_frank_energie-5.0.0/python_frank_energie/exceptions.py
+-rw-r--r--   0        0        0     9007 2023-06-12 21:41:16.330471 python_frank_energie-5.0.0/python_frank_energie/frank_energie.py
+-rw-r--r--   0        0        0    11198 2023-06-12 21:41:16.330471 python_frank_energie-5.0.0/python_frank_energie/models.py
+-rw-r--r--   0        0        0     2334 1970-01-01 00:00:00.000000 python_frank_energie-5.0.0/PKG-INFO
```

### Comparing `python_frank_energie-4.1.0/LICENSE` & `python_frank_energie-5.0.0/LICENSE`

 * *Files identical despite different names*

### Comparing `python_frank_energie-4.1.0/pyproject.toml` & `python_frank_energie-5.0.0/pyproject.toml`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "python-frank-energie"
-version = "4.1.0"
+version = "5.0.0"
 description = "Asynchronous Python client for the Frank Energie"
 authors = ["DCSBL"]
 maintainers = ["DCSBL"]
 license = "Apache License 2.0"
 readme = "README.md"
 homepage = "https://github.com/dcsbl/python-frank-energie"
 repository = "https://github.com/dcsbl/python-frank-energie"
@@ -23,23 +23,23 @@
 [tool.poetry.dev-dependencies]
 aresponses = "^2.1.6"
 black = "^22.12"
 blacken-docs = "^1.13.0"
 flake8 = "^4.0.1"
 flake8-docstrings = "^1.5.0"
 isort = "^5.11.4"
-pre-commit = "^3.1.1"
+pre-commit = "^3.3.2"
 pre-commit-hooks = "^4.4.0"
-pylint = "^2.15.10"
+pylint = "^2.17.4"
 pytest = "^7.2.1"
 pytest-asyncio = "^0.21.0"
-pytest-cov = "^4.0.0"
+pytest-cov = "^4.1.0"
 yamllint = "^1.29.0"
-pyupgrade = "^3.3.1"
-flake8-simplify = "^0.19.3"
+pyupgrade = "^3.6.0"
+flake8-simplify = "^0.20.0"
 vulture = "^2.7"
 flake8-bandit = "^3.0.0"
 flake8-bugbear = "^23.3.12"
 flake8-builtins = "^2.1.0"
 flake8-comprehensions = "^3.10.0"
 flake8-eradicate = "^1.2.1"
 flake8-markdown = "^0.3.0"
```

### Comparing `python_frank_energie-4.1.0/python_frank_energie/frank_energie.py` & `python_frank_energie-5.0.0/python_frank_energie/frank_energie.py`

 * *Files 16% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 
 import asyncio
 from datetime import date
 from typing import Any
 
 from aiohttp.client import ClientError, ClientSession
 
-from .exceptions import AuthRequiredException
+from .exceptions import AuthException, AuthRequiredException
 from .models import Authentication, Invoices, MarketPrices, MonthSummary, User
 
 
 class FrankEnergie:
     """FrankEnergie API."""
 
     DATA_URL = "https://frank-graphql-prod.graphcdn.app/"
@@ -41,19 +41,27 @@
                 self.DATA_URL,
                 json=query,
                 headers={"Authorization": f"Bearer {self._auth.authToken}"}
                 if self._auth is not None
                 else None,
             )
 
-            return await resp.json()
+            response = await resp.json()
 
         except (asyncio.TimeoutError, ClientError, KeyError) as error:
             raise ValueError(f"Request failed: {error}") from error
 
+        # Catch common error messages and raise a more specific exception
+        if errors := response.get("errors"):
+            for error in errors:
+                if error["message"] == "user-error:auth-not-authorised":
+                    raise AuthException
+
+        return response
+
     async def login(self, username: str, password: str) -> Authentication:
         """Login and get the authentication token."""
         query = {
             "query": """
                 mutation Login($email: String!, $password: String!) {
                     login(email: $email, password: $password) {
                         authToken
@@ -64,36 +72,39 @@
             "operationName": "Login",
             "variables": {"email": username, "password": password},
         }
 
         self._auth = Authentication.from_dict(await self._query(query))
         return self._auth
 
-    async def renewToken(self, authToken: str, refreshToken: str) -> Authentication:
+    async def renew_token(self) -> Authentication:
         """Renew the authentication token."""
+        if self._auth is None:
+            raise AuthRequiredException
+
         query = {
             "query": """
                 mutation RenewToken($authToken: String!, $refreshToken: String!) {
                     renewToken(authToken: $authToken, refreshToken: $refreshToken) {
                         authToken
                         refreshToken
                     }
                 }
             """,
             "operationName": "RenewToken",
-            "variables": {"authToken": authToken, "refreshToken": refreshToken},
+            "variables": {
+                "authToken": self._auth.authToken,
+                "refreshToken": self._auth.refreshToken,
+            },
         }
 
-        json = await self._query(query)
-        print(json)
-
-        self._auth = Authentication.from_dict(json)
+        self._auth = Authentication.from_dict(await self._query(query))
         return self._auth
 
-    async def monthSummary(self) -> MonthSummary:
+    async def month_summary(self) -> MonthSummary:
         """Get month summary data."""
         if self._auth is None:
             raise AuthRequiredException
 
         query = {
             "query": """
                 query MonthSummary {
@@ -178,56 +189,70 @@
         self, start_date: date, end_date: date | None = None
     ) -> MarketPrices:
         """Get market prices."""
         query_data = {
             "query": """
                 query MarketPrices($startDate: Date!, $endDate: Date!) {
                     marketPricesElectricity(startDate: $startDate, endDate: $endDate) {
-                       from till marketPrice marketPriceTax sourcingMarkupPrice energyTaxPrice
+                       from
+                       till
+                       marketPrice
+                       marketPriceTax
+                       sourcingMarkupPrice
+                       energyTaxPrice
                     }
                     marketPricesGas(startDate: $startDate, endDate: $endDate) {
-                       from till marketPrice marketPriceTax sourcingMarkupPrice energyTaxPrice
+                       from
+                       till
+                       marketPrice
+                       marketPriceTax
+                       sourcingMarkupPrice
+                       energyTaxPrice
                     }
                 }
             """,
             "variables": {"startDate": str(start_date), "endDate": str(end_date)},
             "operationName": "MarketPrices",
         }
 
         return MarketPrices.from_dict(await self._query(query_data))
 
-    async def userPrices(self, start_date: date) -> MarketPrices:
+    async def user_prices(self, start_date: date) -> MarketPrices:
         """Get customer market prices."""
         if self._auth is None:
             raise AuthRequiredException
 
         query_data = {
             "query": """
                 query CustomerMarketPrices($date: String!) {
                     customerMarketPrices(date: $date) {
                         electricityPrices {
-                            from till marketPrice marketPriceTax
+                            from
+                            till
+                            marketPrice
+                            marketPriceTax
                             sourcingMarkupPrice: consumptionSourcingMarkupPrice
                             energyTaxPrice: energyTax
                         }
                         gasPrices {
-                            from till marketPrice marketPriceTax
+                            from
+                            till
+                            marketPrice
+                            marketPriceTax
                             sourcingMarkupPrice: consumptionSourcingMarkupPrice
                             energyTaxPrice: energyTax
                         }
                     }
                 }
             """,
             "variables": {"date": str(start_date)},
             "operationName": "CustomerMarketPrices",
         }
 
-        result = await self._query(query_data)
-
-        return MarketPrices.from_userprices_dict(result)
+        return MarketPrices.from_userprices_dict(await self._query(query_data))
 
     @property
     def is_authenticated(self) -> bool:
         """Return if client is authenticated.
 
         Does not actually check if the token is valid.
         """
```

### Comparing `python_frank_energie-4.1.0/python_frank_energie/models.py` & `python_frank_energie-5.0.0/python_frank_energie/models.py`

 * *Files identical despite different names*

