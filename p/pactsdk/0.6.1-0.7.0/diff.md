# Comparing `tmp/pactsdk-0.6.1.tar.gz` & `tmp/pactsdk-0.7.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pactsdk-0.6.1.tar", max compression
+gzip compressed data, was "pactsdk-0.7.0.tar", max compression
```

## Comparing `pactsdk-0.6.1.tar` & `pactsdk-0.7.0.tar`

### file list

```diff
@@ -1,33 +1,33 @@
--rw-r--r--   0        0        0     1063 2022-07-14 08:55:23.297528 pactsdk-0.6.1/LICENSE
--rw-r--r--   0        0        0     5482 2023-03-30 10:07:17.918258 pactsdk-0.6.1/README.md
--rw-r--r--   0        0        0      538 2023-04-11 09:21:24.923112 pactsdk-0.6.1/pactsdk/__init__.py
--rw-r--r--   0        0        0     4504 2023-01-03 15:45:49.490178 pactsdk-0.6.1/pactsdk/add_liquidity.py
--rw-r--r--   0        0        0     2174 2022-07-14 08:55:23.297528 pactsdk-0.6.1/pactsdk/api.py
--rw-r--r--   0        0        0     8096 2023-03-30 09:06:45.857841 pactsdk-0.6.1/pactsdk/asset.py
--rw-r--r--   0        0        0     5263 2023-03-30 10:07:12.264922 pactsdk-0.6.1/pactsdk/client.py
--rw-r--r--   0        0        0     1725 2023-04-11 09:21:34.039780 pactsdk-0.6.1/pactsdk/config.py
--rw-r--r--   0        0        0     2353 2022-07-14 08:55:23.297528 pactsdk-0.6.1/pactsdk/constant_product_calculator.py
--rw-r--r--   0        0        0      852 2023-03-09 15:26:59.934347 pactsdk-0.6.1/pactsdk/encoding.py
--rw-r--r--   0        0        0      143 2022-07-14 08:55:23.297528 pactsdk-0.6.1/pactsdk/exceptions.py
--rw-r--r--   0        0        0      191 2023-03-30 09:06:45.871175 pactsdk-0.6.1/pactsdk/factories/__init__.py
--rw-r--r--   0        0        0     6986 2023-03-30 09:06:45.874508 pactsdk-0.6.1/pactsdk/factories/base_factory.py
--rw-r--r--   0        0        0     1950 2023-03-30 09:06:45.874508 pactsdk-0.6.1/pactsdk/factories/constant_product.py
--rw-r--r--   0        0        0     1000 2023-03-30 09:06:45.874508 pactsdk-0.6.1/pactsdk/factories/get_pool_factory.py
--rw-r--r--   0        0        0     4637 2023-03-30 09:06:45.847841 pactsdk-0.6.1/pactsdk/farming/README.md
--rw-r--r--   0        0        0      565 2023-03-30 09:06:45.847841 pactsdk-0.6.1/pactsdk/farming/__init__.py
--rw-r--r--   0        0        0     7907 2023-04-11 09:21:34.039780 pactsdk-0.6.1/pactsdk/farming/escrow.py
--rw-r--r--   0        0        0    16770 2023-04-11 09:21:34.039780 pactsdk-0.6.1/pactsdk/farming/farm.py
--rw-r--r--   0        0        0     5785 2023-03-30 09:06:45.851175 pactsdk-0.6.1/pactsdk/farming/farm_state.py
--rw-r--r--   0        0        0      786 2023-03-30 09:06:45.861175 pactsdk-0.6.1/pactsdk/farming/farming_client.py
--rw-r--r--   0        0        0     1484 2023-03-30 09:06:45.854508 pactsdk-0.6.1/pactsdk/gas_station.py
--rw-r--r--   0        0        0    24155 2023-03-30 10:07:05.564919 pactsdk-0.6.1/pactsdk/pool.py
--rw-r--r--   0        0        0    11887 2023-03-30 09:06:45.871175 pactsdk-0.6.1/pactsdk/pool_calculator.py
--rw-r--r--   0        0        0     2863 2023-03-30 09:06:45.871175 pactsdk-0.6.1/pactsdk/pool_state.py
--rw-r--r--   0        0        0    12291 2023-01-03 15:45:34.790183 pactsdk-0.6.1/pactsdk/stableswap_calculator.py
--rw-r--r--   0        0        0     5592 2022-07-14 08:55:23.300861 pactsdk-0.6.1/pactsdk/swap.py
--rw-r--r--   0        0        0     1905 2023-03-30 09:06:45.854508 pactsdk-0.6.1/pactsdk/transaction_group.py
--rw-r--r--   0        0        0     2166 2023-03-30 09:06:45.861175 pactsdk-0.6.1/pactsdk/utils.py
--rw-r--r--   0        0        0     5535 2022-08-18 13:32:35.849222 pactsdk-0.6.1/pactsdk/zap.py
--rw-r--r--   0        0        0     1022 2023-04-11 09:21:14.509777 pactsdk-0.6.1/pyproject.toml
--rw-r--r--   0        0        0     6416 1970-01-01 00:00:00.000000 pactsdk-0.6.1/setup.py
--rw-r--r--   0        0        0     6176 1970-01-01 00:00:00.000000 pactsdk-0.6.1/PKG-INFO
+-rw-r--r--   0        0        0     1063 2022-07-14 08:55:23.297528 pactsdk-0.7.0/LICENSE
+-rw-r--r--   0        0        0     5482 2023-03-30 10:07:17.918258 pactsdk-0.7.0/README.md
+-rw-r--r--   0        0        0      680 2023-06-12 13:14:44.907642 pactsdk-0.7.0/pactsdk/__init__.py
+-rw-r--r--   0        0        0     4504 2023-01-03 15:45:49.490178 pactsdk-0.7.0/pactsdk/add_liquidity.py
+-rw-r--r--   0        0        0     2174 2022-07-14 08:55:23.297528 pactsdk-0.7.0/pactsdk/api.py
+-rw-r--r--   0        0        0     8096 2023-03-30 09:06:45.857841 pactsdk-0.7.0/pactsdk/asset.py
+-rw-r--r--   0        0        0     6971 2023-06-12 13:14:34.580973 pactsdk-0.7.0/pactsdk/client.py
+-rw-r--r--   0        0        0     2085 2023-06-12 13:14:34.580973 pactsdk-0.7.0/pactsdk/config.py
+-rw-r--r--   0        0        0     2353 2023-06-05 09:02:08.789645 pactsdk-0.7.0/pactsdk/constant_product_calculator.py
+-rw-r--r--   0        0        0      962 2023-06-12 13:14:34.580973 pactsdk-0.7.0/pactsdk/encoding.py
+-rw-r--r--   0        0        0      143 2022-07-14 08:55:23.297528 pactsdk-0.7.0/pactsdk/exceptions.py
+-rw-r--r--   0        0        0      191 2023-03-30 09:06:45.871175 pactsdk-0.7.0/pactsdk/factories/__init__.py
+-rw-r--r--   0        0        0     6986 2023-03-30 09:06:45.874508 pactsdk-0.7.0/pactsdk/factories/base_factory.py
+-rw-r--r--   0        0        0     1950 2023-03-30 09:06:45.874508 pactsdk-0.7.0/pactsdk/factories/constant_product.py
+-rw-r--r--   0        0        0     1000 2023-03-30 09:06:45.874508 pactsdk-0.7.0/pactsdk/factories/get_pool_factory.py
+-rw-r--r--   0        0        0     4637 2023-03-30 09:06:45.847841 pactsdk-0.7.0/pactsdk/farming/README.md
+-rw-r--r--   0        0        0      565 2023-03-30 09:06:45.847841 pactsdk-0.7.0/pactsdk/farming/__init__.py
+-rw-r--r--   0        0        0     7907 2023-04-11 09:21:34.039780 pactsdk-0.7.0/pactsdk/farming/escrow.py
+-rw-r--r--   0        0        0    16770 2023-04-11 09:21:34.039780 pactsdk-0.7.0/pactsdk/farming/farm.py
+-rw-r--r--   0        0        0     5785 2023-03-30 09:06:45.851175 pactsdk-0.7.0/pactsdk/farming/farm_state.py
+-rw-r--r--   0        0        0      786 2023-03-30 09:06:45.861175 pactsdk-0.7.0/pactsdk/farming/farming_client.py
+-rw-r--r--   0        0        0    20492 2023-06-12 13:14:34.580973 pactsdk-0.7.0/pactsdk/folks_lending_pool.py
+-rw-r--r--   0        0        0     1484 2023-03-30 09:06:45.854508 pactsdk-0.7.0/pactsdk/gas_station.py
+-rw-r--r--   0        0        0    24155 2023-03-30 10:07:05.564919 pactsdk-0.7.0/pactsdk/pool.py
+-rw-r--r--   0        0        0    11887 2023-03-30 09:06:45.871175 pactsdk-0.7.0/pactsdk/pool_calculator.py
+-rw-r--r--   0        0        0     2863 2023-03-30 09:06:45.871175 pactsdk-0.7.0/pactsdk/pool_state.py
+-rw-r--r--   0        0        0    12291 2023-01-03 15:45:34.790183 pactsdk-0.7.0/pactsdk/stableswap_calculator.py
+-rw-r--r--   0        0        0     5592 2022-07-14 08:55:23.300861 pactsdk-0.7.0/pactsdk/swap.py
+-rw-r--r--   0        0        0     1905 2023-03-30 09:06:45.854508 pactsdk-0.7.0/pactsdk/transaction_group.py
+-rw-r--r--   0        0        0     2166 2023-06-01 12:21:01.694131 pactsdk-0.7.0/pactsdk/utils.py
+-rw-r--r--   0        0        0     5535 2022-08-18 13:32:35.849222 pactsdk-0.7.0/pactsdk/zap.py
+-rw-r--r--   0        0        0     1064 2023-06-12 13:14:49.660976 pactsdk-0.7.0/pyproject.toml
+-rw-r--r--   0        0        0     6214 1970-01-01 00:00:00.000000 pactsdk-0.7.0/PKG-INFO
```

### Comparing `pactsdk-0.6.1/LICENSE` & `pactsdk-0.7.0/LICENSE`

 * *Files identical despite different names*

### Comparing `pactsdk-0.6.1/README.md` & `pactsdk-0.7.0/README.md`

 * *Files identical despite different names*

### Comparing `pactsdk-0.6.1/pactsdk/__init__.py` & `pactsdk-0.7.0/pactsdk/__init__.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,13 +1,19 @@
-__version__ = "0.6.1"
+__version__ = "0.7.0"
 
 from .add_liquidity import LiquidityAddition  # noqa
 from .asset import Asset, fetch_asset_by_index  # noqa
 from .client import PactClient  # noqa
 from .exceptions import PactSdkError  # noqa
 from .factories import *  # noqa
 from .farming import *  # noqa
+from .folks_lending_pool import (  # noqa
+    FolksLendingPool,
+    FolksLendingPoolAdapter,
+    LendingLiquidityAddition,
+    LendingSwap,
+)
 from .gas_station import GasStation, get_gas_station, set_gas_station  # noqa
 from .pool import Pool, PoolState  # noqa
 from .swap import Swap, SwapEffect  # noqa
 from .transaction_group import TransactionGroup  # noqa
 from .zap import Zap, ZapParams  # noqa
```

### Comparing `pactsdk-0.6.1/pactsdk/add_liquidity.py` & `pactsdk-0.7.0/pactsdk/add_liquidity.py`

 * *Files identical despite different names*

### Comparing `pactsdk-0.6.1/pactsdk/api.py` & `pactsdk-0.7.0/pactsdk/api.py`

 * *Files identical despite different names*

### Comparing `pactsdk-0.6.1/pactsdk/asset.py` & `pactsdk-0.7.0/pactsdk/asset.py`

 * *Files identical despite different names*

### Comparing `pactsdk-0.6.1/pactsdk/client.py` & `pactsdk-0.7.0/pactsdk/client.py`

 * *Files 25% similar despite different names*

```diff
@@ -21,14 +21,19 @@
 
 from pactsdk.api import ApiListPoolsResponse
 from pactsdk.farming.farming_client import PactFarmingClient
 
 from .asset import Asset, fetch_asset_by_index
 from .config import Config, Network, get_config
 from .factories import ConstantProductFactory, get_pool_factory
+from .folks_lending_pool import (
+    FolksLendingPool,
+    FolksLendingPoolAdapter,
+    fetch_folks_lending_pool,
+)
 from .gas_station import get_gas_station, set_gas_station
 from .pool import (
     ListPoolsParams,
     Pool,
     fetch_pool_by_id,
     fetch_pools_by_assets,
     list_pools,
@@ -129,14 +134,51 @@
             algosdk.error.AlgodHTTPError: If the pool does not exist.
 
         Returns:
             The pool for the application id.
         """
         return fetch_pool_by_id(algod=self.algod, app_id=app_id)
 
+    def fetch_folks_lending_pool(self, app_id: int) -> FolksLendingPool:
+        """Fetches Folks Finance lending pool that can be used in FolksLendingPoolAdapter which allows higher APR than a normal pool.
+        See :py:mod:`pactsdk.folks_lending_pool` for details.
+
+        Args:
+            app_id: The application id of the Folks Finance pool. You can find the ids here - https://docs.folks.finance/developer/contracts
+
+        Returns:
+            The Folks Finance lending pool for the given application id.
+        """
+        return fetch_folks_lending_pool(self.algod, app_id)
+
+    def get_folks_lending_pool_adapter(
+        self,
+        pact_pool: Pool,
+        primary_lending_pool: FolksLendingPool,
+        secondary_lending_pool: FolksLendingPool,
+    ) -> FolksLendingPoolAdapter:
+        """Creates the adapter object that allows composing Folks Finance lending pools with Pact pool, resulting in a higher APR.
+        See :py:mod:`pactsdk.folks_lending_pool` for details.
+
+        Args:
+            pact_pool: The Pact pool between two fAssets tokens.
+            primary_lending_pool: The Folks Finance pool for the primary fAsset.
+            secondary_lending_pool: The Folks Finance pool for the secondary fAsset.
+
+        Returns:
+            The adapter object.
+        """
+        return FolksLendingPoolAdapter(
+            algod=self.algod,
+            app_id=self.config.folks_lending_pool_adapter_id,
+            pact_pool=pact_pool,
+            primary_lending_pool=primary_lending_pool,
+            secondary_lending_pool=secondary_lending_pool,
+        )
+
     def get_constant_product_pool_factory(self) -> ConstantProductFactory:
         """Gets the constant product pool factory according to the client's configuration."""
         factory = get_pool_factory(
             algod=self.algod, pool_type="CONSTANT_PRODUCT", config=self.config
         )
         return cast(ConstantProductFactory, factory)
```

### Comparing `pactsdk-0.6.1/pactsdk/config.py` & `pactsdk-0.7.0/pactsdk/config.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,52 +1,58 @@
 import dataclasses
 from typing import Literal
 
 MAINNET_API_URL = "https://api.pact.fi"
 MAINNET_GAS_STATION_ID = 1027956681
+MAINNET_FOLKS_LENDING_POOL_ADAPTER_ID = 1123472996
 MAINNET_FACTORY_CONSTANT_PRODUCT_ID = 1072843805
 MAINNET_FACTORY_NFT_CONSTANT_PRODUCT_ID = 1076423760
 
 TESTNET_API_URL = "https://api.testnet.pact.fi"
 TESTNET_GAS_STATION_ID = 156575978
+TESTNET_FOLKS_LENDING_POOL_ADAPTER_ID = 228284187
 TESTNET_FACTORY_CONSTANT_PRODUCT_ID = 166540424
-TESTNET_FACTORY_NFT_CONSTANT_PRODUCT_ID = 166540708
+TESTNET_FACTORY_NFT_CONSTANT_PRODUCT_ID = 190269485
 
 Network = Literal["mainnet", "testnet", "dev"]
 
 
 @dataclasses.dataclass
 class Config:
     api_url: str = ""
     gas_station_id: int = 0
+    folks_lending_pool_adapter_id: int = 0
     factory_constant_product_id: int = 0
     factory_nft_constant_product_id: int = 0
 
 
 def get_config(network: Network, **kwargs) -> Config:
     if network == "mainnet":
         params: dict = {
             "api_url": MAINNET_API_URL,
             "gas_station_id": MAINNET_GAS_STATION_ID,
+            "folks_lending_pool_adapter_id": MAINNET_FOLKS_LENDING_POOL_ADAPTER_ID,
             "factory_constant_product_id": MAINNET_FACTORY_CONSTANT_PRODUCT_ID,
             "factory_nft_constant_product_id": MAINNET_FACTORY_NFT_CONSTANT_PRODUCT_ID,
             **kwargs,
         }
     elif network == "testnet":
         params = {
             "api_url": TESTNET_API_URL,
             "gas_station_id": TESTNET_GAS_STATION_ID,
+            "folks_lending_pool_adapter_id": TESTNET_FOLKS_LENDING_POOL_ADAPTER_ID,
             "factory_constant_product_id": TESTNET_FACTORY_CONSTANT_PRODUCT_ID,
             "factory_nft_constant_product_id": TESTNET_FACTORY_NFT_CONSTANT_PRODUCT_ID,
             **kwargs,
         }
     elif network == "dev":
         params = {
             "api_url": "",
             "gas_station_id": 0,
+            "folks_lending_pool_adapter_id": 0,
             "factory_constant_product_id": 0,
             "factory_nft_constant_product_id": 0,
             **kwargs,
         }
     else:
         raise ValueError(f"No predefined config for network {network}")
```

### Comparing `pactsdk-0.6.1/pactsdk/constant_product_calculator.py` & `pactsdk-0.7.0/pactsdk/constant_product_calculator.py`

 * *Files identical despite different names*

### Comparing `pactsdk-0.6.1/pactsdk/encoding.py` & `pactsdk-0.7.0/pactsdk/encoding.py`

 * *Files 24% similar despite different names*

```diff
@@ -12,18 +12,20 @@
         for x in int.to_bytes(i, length=8, byteorder="big", signed=False)
     )
     return base64.b64encode(_bytes).decode("ascii")
 
 
 def deserialize_uint64(data: str) -> list[int]:
     decoded = base64.b64decode(data)
-    return [
-        int.from_bytes(decoded[offset : offset + 8], byteorder="big", signed=False)
-        for offset in range(0, len(decoded), 8)
-    ]
+    return [extract_uint64(decoded, offset) for offset in range(0, len(decoded), 8)]
+
+
+def extract_uint64(byte_str: bytes, index: int) -> int:
+    """Extract a uint64 from a byte string"""
+    return int.from_bytes(byte_str[index : index + 8], byteorder="big")
 
 
 def decode_string_from_global_state(encoded: str) -> str:
     return base64.b64decode(encoded).decode()
 
 
 def decode_address_from_global_state(encoded: str) -> str:
```

### Comparing `pactsdk-0.6.1/pactsdk/factories/base_factory.py` & `pactsdk-0.7.0/pactsdk/factories/base_factory.py`

 * *Files identical despite different names*

### Comparing `pactsdk-0.6.1/pactsdk/factories/constant_product.py` & `pactsdk-0.7.0/pactsdk/factories/constant_product.py`

 * *Files identical despite different names*

### Comparing `pactsdk-0.6.1/pactsdk/factories/get_pool_factory.py` & `pactsdk-0.7.0/pactsdk/factories/get_pool_factory.py`

 * *Files identical despite different names*

### Comparing `pactsdk-0.6.1/pactsdk/farming/README.md` & `pactsdk-0.7.0/pactsdk/farming/README.md`

 * *Files identical despite different names*

### Comparing `pactsdk-0.6.1/pactsdk/farming/__init__.py` & `pactsdk-0.7.0/pactsdk/farming/__init__.py`

 * *Files identical despite different names*

### Comparing `pactsdk-0.6.1/pactsdk/farming/escrow.py` & `pactsdk-0.7.0/pactsdk/farming/escrow.py`

 * *Files identical despite different names*

### Comparing `pactsdk-0.6.1/pactsdk/farming/farm.py` & `pactsdk-0.7.0/pactsdk/farming/farm.py`

 * *Files identical despite different names*

### Comparing `pactsdk-0.6.1/pactsdk/farming/farm_state.py` & `pactsdk-0.7.0/pactsdk/farming/farm_state.py`

 * *Files identical despite different names*

### Comparing `pactsdk-0.6.1/pactsdk/farming/farming_client.py` & `pactsdk-0.7.0/pactsdk/farming/farming_client.py`

 * *Files identical despite different names*

### Comparing `pactsdk-0.6.1/pactsdk/gas_station.py` & `pactsdk-0.7.0/pactsdk/gas_station.py`

 * *Files identical despite different names*

### Comparing `pactsdk-0.6.1/pactsdk/pool.py` & `pactsdk-0.7.0/pactsdk/pool.py`

 * *Files identical despite different names*

### Comparing `pactsdk-0.6.1/pactsdk/pool_calculator.py` & `pactsdk-0.7.0/pactsdk/pool_calculator.py`

 * *Files identical despite different names*

### Comparing `pactsdk-0.6.1/pactsdk/pool_state.py` & `pactsdk-0.7.0/pactsdk/pool_state.py`

 * *Files identical despite different names*

### Comparing `pactsdk-0.6.1/pactsdk/stableswap_calculator.py` & `pactsdk-0.7.0/pactsdk/stableswap_calculator.py`

 * *Files identical despite different names*

### Comparing `pactsdk-0.6.1/pactsdk/swap.py` & `pactsdk-0.7.0/pactsdk/swap.py`

 * *Files identical despite different names*

### Comparing `pactsdk-0.6.1/pactsdk/transaction_group.py` & `pactsdk-0.7.0/pactsdk/transaction_group.py`

 * *Files identical despite different names*

### Comparing `pactsdk-0.6.1/pactsdk/utils.py` & `pactsdk-0.7.0/pactsdk/utils.py`

 * *Files identical despite different names*

### Comparing `pactsdk-0.6.1/pactsdk/zap.py` & `pactsdk-0.7.0/pactsdk/zap.py`

 * *Files identical despite different names*

### Comparing `pactsdk-0.6.1/pyproject.toml` & `pactsdk-0.7.0/pyproject.toml`

 * *Files 11% similar despite different names*

```diff
@@ -1,35 +1,37 @@
 [tool.poetry]
 name = "pactsdk"
-version = "0.6.1"
+version = "0.7.0"
 description = "Python SDK for Pact smart contracts"
 authors = ["Mateusz Tomczyk <mateusz.tomczyk@ulam.io>"]
 homepage = "https://github.com/pactfi/pact-py-sdk"
 repository = "https://github.com/pactfi/pact-py-sdk"
 readme = "README.md"
 license = "MIT"
 
 [tool.poetry.dependencies]
 python = "^3.9"
 py-algorand-sdk = "^2.0.0"
 requests = "^2.27.1"
+cffi = "^1.15.1"
 
-[tool.poetry.dev-dependencies]
+[tool.poetry.group.dev.dependencies]
 pytest = "^7.0.0"
 black = "^22.1.0"
 mypy = "^1.1.1"
 flake8 = "^4.0.1"
 isort = "^5.10.1"
 types-requests = "^2.27.8"
 responses = "^0.18.0"
 freezegun = "^1.2.1"
 Sphinx = "^4.5.0"
 sphinx-rtd-theme = "^1.0.0"
 sphinx_mdinclude = "^0.5.1"
 sphinx-autodoc-typehints = "^1.18.1"
+tealish = "^0.0.2"
 
 [build-system]
 requires = ["poetry-core>=1.0.0"]
 build-backend = "poetry.core.masonry.api"
 
 [tool.black]
 exclude = ".venv"
```

### Comparing `pactsdk-0.6.1/setup.py` & `pactsdk-0.7.0/PKG-INFO`

 * *Files 16% similar despite different names*

```diff
@@ -1,30 +1,212 @@
-# -*- coding: utf-8 -*-
-from setuptools import setup
+Metadata-Version: 2.1
+Name: pactsdk
+Version: 0.7.0
+Summary: Python SDK for Pact smart contracts
+Home-page: https://github.com/pactfi/pact-py-sdk
+License: MIT
+Author: Mateusz Tomczyk
+Author-email: mateusz.tomczyk@ulam.io
+Requires-Python: >=3.9,<4.0
+Classifier: License :: OSI Approved :: MIT License
+Classifier: Programming Language :: Python :: 3
+Classifier: Programming Language :: Python :: 3.9
+Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
+Requires-Dist: cffi (>=1.15.1,<2.0.0)
+Requires-Dist: py-algorand-sdk (>=2.0.0,<3.0.0)
+Requires-Dist: requests (>=2.27.1,<3.0.0)
+Project-URL: Repository, https://github.com/pactfi/pact-py-sdk
+Description-Content-Type: text/markdown
 
-packages = \
-['pactsdk', 'pactsdk.factories', 'pactsdk.farming']
+# Pact Python SDK
 
-package_data = \
-{'': ['*']}
+**pactsdk** is a software development kit for interfacing to [Pact](https://pact.fi), a decentralized automated market maker on the Algorand protocol.
 
-install_requires = \
-['py-algorand-sdk>=2.0.0,<3.0.0', 'requests>=2.27.1,<3.0.0']
-
-setup_kwargs = {
-    'name': 'pactsdk',
-    'version': '0.6.1',
-    'description': 'Python SDK for Pact smart contracts',
-    'long_description': '# Pact Python SDK\n\n**pactsdk** is a software development kit for interfacing to [Pact](https://pact.fi), a decentralized automated market maker on the Algorand protocol.\n\nThe full documentation for this module can be found here:\n\n[https://pactfi.github.io/pact-py-sdk/latest/](https://pactfi.github.io/pact-py-sdk/latest/)\n\nThe Python SDK provides a set of modules on top of the Algorand Python SDK for interacting with liquidity pools and making swaps.\nClients can use the Python SDK to enhance their trading experience with Pact.\n\nWhat is covered by the library:\n\n- Creating pools\n- Managing liquidity\n- Making swaps\n- Farming\n\nSigning and sending transactions is not covered by the library. The provided examples use algosdk directly to send the transactions.\n\n# Installation\n\n`pip install pactsdk`\n\n# Basic usage\n\n**CAUTION** - The library uses integers for asset amounts e.g. microalgos instead of algos so if you want to send 1 algo, you need to specify it as 1_000_000.\n\nCreate a Pact client.\n\n```py\nfrom algosdk.v2client.algod import AlgodClient\nimport pactsdk\n\nalgod = AlgodClient(token, url)\npact = pactsdk.PactClient(algod)\n```\n\nBy default, the client is configured to work with mainnet. You can easily change it by providing `network` argument. The `network` argument changes the default values in `pact.config` object. It contains things like API URL or global contract ids.\n\n```py\npact = pactsdk.PactClient(algod, network="testnet")\n```\n\nFetching pools by assets pair. It uses Pact API to retrieve the pool. Can return multiple pools with differing fee_bps.\n\n```py\nalgo = pact.fetch_asset(0)\nother_coin = pact.fetch_asset(8949213)\n\npools = pact.fetch_pools_by_assets(algo, other_coin) # The pool will be fetched regardless of assets order.\n```\n\nYou can fetch a pool by providing assets ids instead of Asset objects.\n\n```py\npools = pact.fetch_pools_by_assets(0, 8949213)\n```\n\nYou can also fetch a pool by providing app id. This way the pool is retrieved directly from the chain.\n\n```py\npool = pact.fetch_pool_by_id(456321)\n```\n\nBefore making the transactions you need to opt-in for the assets. There\'s no need to opt-in for algo.\n\n```py\nimport algosdk\n\nprivate_key = algosdk.mnemonic.to_private_key(\'<mnemonic>\')\naddress = algosdk.account.address_from_private_key(private_key)\n\ndef opt_in(asset):\n    is_opted_in = asset.is_opted_in(address)\n    if not is_opted_in:\n        opt_in_tx = asset.prepare_opt_in_tx(address)\n        signed_tx = opt_in_tx.sign(private_key)\n        algod.send_transaction(signed_tx)\n\nopt_in(pool.primary_asset)\nopt_in(pool.secondary_asset)\nopt_in(pool.liquidity_asset) # Needed if you want to manage the liquidity.\n```\n\nCheck the current pool state.\n\n```py\nprint(pool.state)\n# PoolState(\n#   total_liquidity=900000,\n#   total_primary=956659,\n#   total_secondary=849972,\n#   primary_asset_price=0.8884795940873393,\n#   secondary_asset_price=1.1255182523659604,\n# )\n```\n\nExplicit pool state update is necessary periodically and after each pool operation.\n\n```py\npool.update_state()\npool.state  # Now holds fresh values.\n```\n\nManaging the liquidity.\n\n```py\n# Add liquidity.\nliquidity_addition = pool.prepare_add_liquidity(\n  primary_asset_amount=100_000,\n  secondary_asset_amount=50_000,\n);\nadd_liq_tx_group = liquidity_addition.prepare_tx_group(address)\nsigned_add_liq_tx_group = add_liq_tx_group.sign(private_key)\nalgod.send_transactions(signed_add_liq_tx_group)\n\n# Remove liquidity.\nremove_liq_tx_group = pool.prepare_remove_liquidity_tx_group(\n  address=address,\n  amount=100_000,\n)\nsigned_remove_liq_tx_group = remove_liq_tx_group.sign(private_key)\nalgod.send_transactions(signed_remove_liq_tx_group)\n```\n\nMaking a swap.\n\n```py\nswap = pool.prepare_swap(\n  asset=algo,\n  amount=200_000,\n  slippage_pct=2,\n)\n\n# You can inspect swap effect before submitting the transaction.\nprint(swap.effect)\n# SwapEffect(\n#     amount_deposited=200000,\n#     amount_received=146529,\n#     minimum_amount_received=143598,\n#     fee=441,\n#     price=0.73485,\n#     primary_asset_price_after_swap=0.6081680080300244,\n#     secondary_asset_price_after_swap=1.6442824791774173,\n#     primary_asset_price_change_pct=-31.549580645715963,\n#     secondary_asset_price_change_pct=46.091142966447585,\n# )\n\n# Let\'s submit the swap.\nswap_tx_group = swap.prepare_tx_group(address)\nsigned_tx_group = swap_tx_group.sign_txn(private_key)\nalgod.send_transactions(signed_tx_group)\n```\n\n## Composability of transactions.\n\nThe SDK has two sets of methods for creating transactions:\n\n1. `prepare_..._tx_group` e.g. `pool.prepare_swap_tx_group`\n\n   Those methods are convenience methods which ask algod for suggested transaction parameters, build transactions and create a transaction group. You can\'t add you own transactions to the group using those methods.\n\n2. `build_..._txs` e.g. `pool.build_swap_txs`\n\n   Those methods return a list of transactions. You can extend that list with your own transactions and create a `TransactionGroup` manually from this list.\n\n# Development\n\n- `poetry install`\n\nDevelopment requires [Pact contracts V1](https://github.com/pactfi/algorand-testbed) to be checked out.\n\n- `git clone git@github.com:pactfi/algorand-testbed.git`\n- `cd algorand-testbed`\n- `poetry install`\n- `docker compose up -d`\n- `cd ..`\n\n## Building\n\n- `poetry build`\n\nYou can install the package locally with\n`pip install dist/pactsdk-<version>.whl`\n\nValidate the installation `python -c "import pactsdk; print(pactsdk.__version__)"`\n\n## Running tests\n\n- `poetry run pytest`\n',
-    'author': 'Mateusz Tomczyk',
-    'author_email': 'mateusz.tomczyk@ulam.io',
-    'maintainer': 'None',
-    'maintainer_email': 'None',
-    'url': 'https://github.com/pactfi/pact-py-sdk',
-    'packages': packages,
-    'package_data': package_data,
-    'install_requires': install_requires,
-    'python_requires': '>=3.9,<4.0',
-}
+The full documentation for this module can be found here:
 
+[https://pactfi.github.io/pact-py-sdk/latest/](https://pactfi.github.io/pact-py-sdk/latest/)
+
+The Python SDK provides a set of modules on top of the Algorand Python SDK for interacting with liquidity pools and making swaps.
+Clients can use the Python SDK to enhance their trading experience with Pact.
+
+What is covered by the library:
+
+- Creating pools
+- Managing liquidity
+- Making swaps
+- Farming
+
+Signing and sending transactions is not covered by the library. The provided examples use algosdk directly to send the transactions.
+
+# Installation
+
+`pip install pactsdk`
+
+# Basic usage
+
+**CAUTION** - The library uses integers for asset amounts e.g. microalgos instead of algos so if you want to send 1 algo, you need to specify it as 1_000_000.
+
+Create a Pact client.
+
+```py
+from algosdk.v2client.algod import AlgodClient
+import pactsdk
+
+algod = AlgodClient(token, url)
+pact = pactsdk.PactClient(algod)
+```
+
+By default, the client is configured to work with mainnet. You can easily change it by providing `network` argument. The `network` argument changes the default values in `pact.config` object. It contains things like API URL or global contract ids.
+
+```py
+pact = pactsdk.PactClient(algod, network="testnet")
+```
+
+Fetching pools by assets pair. It uses Pact API to retrieve the pool. Can return multiple pools with differing fee_bps.
+
+```py
+algo = pact.fetch_asset(0)
+other_coin = pact.fetch_asset(8949213)
+
+pools = pact.fetch_pools_by_assets(algo, other_coin) # The pool will be fetched regardless of assets order.
+```
+
+You can fetch a pool by providing assets ids instead of Asset objects.
+
+```py
+pools = pact.fetch_pools_by_assets(0, 8949213)
+```
+
+You can also fetch a pool by providing app id. This way the pool is retrieved directly from the chain.
+
+```py
+pool = pact.fetch_pool_by_id(456321)
+```
+
+Before making the transactions you need to opt-in for the assets. There's no need to opt-in for algo.
+
+```py
+import algosdk
+
+private_key = algosdk.mnemonic.to_private_key('<mnemonic>')
+address = algosdk.account.address_from_private_key(private_key)
+
+def opt_in(asset):
+    is_opted_in = asset.is_opted_in(address)
+    if not is_opted_in:
+        opt_in_tx = asset.prepare_opt_in_tx(address)
+        signed_tx = opt_in_tx.sign(private_key)
+        algod.send_transaction(signed_tx)
+
+opt_in(pool.primary_asset)
+opt_in(pool.secondary_asset)
+opt_in(pool.liquidity_asset) # Needed if you want to manage the liquidity.
+```
+
+Check the current pool state.
+
+```py
+print(pool.state)
+# PoolState(
+#   total_liquidity=900000,
+#   total_primary=956659,
+#   total_secondary=849972,
+#   primary_asset_price=0.8884795940873393,
+#   secondary_asset_price=1.1255182523659604,
+# )
+```
+
+Explicit pool state update is necessary periodically and after each pool operation.
+
+```py
+pool.update_state()
+pool.state  # Now holds fresh values.
+```
+
+Managing the liquidity.
+
+```py
+# Add liquidity.
+liquidity_addition = pool.prepare_add_liquidity(
+  primary_asset_amount=100_000,
+  secondary_asset_amount=50_000,
+);
+add_liq_tx_group = liquidity_addition.prepare_tx_group(address)
+signed_add_liq_tx_group = add_liq_tx_group.sign(private_key)
+algod.send_transactions(signed_add_liq_tx_group)
+
+# Remove liquidity.
+remove_liq_tx_group = pool.prepare_remove_liquidity_tx_group(
+  address=address,
+  amount=100_000,
+)
+signed_remove_liq_tx_group = remove_liq_tx_group.sign(private_key)
+algod.send_transactions(signed_remove_liq_tx_group)
+```
+
+Making a swap.
+
+```py
+swap = pool.prepare_swap(
+  asset=algo,
+  amount=200_000,
+  slippage_pct=2,
+)
+
+# You can inspect swap effect before submitting the transaction.
+print(swap.effect)
+# SwapEffect(
+#     amount_deposited=200000,
+#     amount_received=146529,
+#     minimum_amount_received=143598,
+#     fee=441,
+#     price=0.73485,
+#     primary_asset_price_after_swap=0.6081680080300244,
+#     secondary_asset_price_after_swap=1.6442824791774173,
+#     primary_asset_price_change_pct=-31.549580645715963,
+#     secondary_asset_price_change_pct=46.091142966447585,
+# )
+
+# Let's submit the swap.
+swap_tx_group = swap.prepare_tx_group(address)
+signed_tx_group = swap_tx_group.sign_txn(private_key)
+algod.send_transactions(signed_tx_group)
+```
+
+## Composability of transactions.
+
+The SDK has two sets of methods for creating transactions:
+
+1. `prepare_..._tx_group` e.g. `pool.prepare_swap_tx_group`
+
+   Those methods are convenience methods which ask algod for suggested transaction parameters, build transactions and create a transaction group. You can't add you own transactions to the group using those methods.
+
+2. `build_..._txs` e.g. `pool.build_swap_txs`
+
+   Those methods return a list of transactions. You can extend that list with your own transactions and create a `TransactionGroup` manually from this list.
+
+# Development
+
+- `poetry install`
+
+Development requires [Pact contracts V1](https://github.com/pactfi/algorand-testbed) to be checked out.
+
+- `git clone git@github.com:pactfi/algorand-testbed.git`
+- `cd algorand-testbed`
+- `poetry install`
+- `docker compose up -d`
+- `cd ..`
+
+## Building
+
+- `poetry build`
+
+You can install the package locally with
+`pip install dist/pactsdk-<version>.whl`
+
+Validate the installation `python -c "import pactsdk; print(pactsdk.__version__)"`
+
+## Running tests
+
+- `poetry run pytest`
 
-setup(**setup_kwargs)
```

