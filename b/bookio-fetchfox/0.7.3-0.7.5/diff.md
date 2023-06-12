# Comparing `tmp/bookio_fetchfox-0.7.3.tar.gz` & `tmp/bookio_fetchfox-0.7.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "bookio_fetchfox-0.7.3.tar", max compression
+gzip compressed data, was "bookio_fetchfox-0.7.5.tar", max compression
```

## Comparing `bookio_fetchfox-0.7.3.tar` & `bookio_fetchfox-0.7.5.tar`

### file list

```diff
@@ -1,57 +1,57 @@
--rw-r--r--   0        0        0     3723 2023-06-11 00:16:32.317610 bookio_fetchfox-0.7.3/README.md
--rw-r--r--   0        0        0        0 2023-06-11 00:16:32.317610 bookio_fetchfox-0.7.3/fetchfox/__init__.py
--rw-r--r--   0        0        0        0 2023-06-11 00:16:32.321610 bookio_fetchfox-0.7.3/fetchfox/apis/__init__.py
--rw-r--r--   0        0        0        0 2023-06-11 00:16:32.321610 bookio_fetchfox-0.7.3/fetchfox/apis/algorand/__init__.py
--rw-r--r--   0        0        0     2140 2023-06-11 00:16:32.321610 bookio_fetchfox-0.7.3/fetchfox/apis/algorand/algonodecloud.py
--rw-r--r--   0        0        0      596 2023-06-11 00:16:32.321610 bookio_fetchfox-0.7.3/fetchfox/apis/algorand/algoxnftcom.py
--rw-r--r--   0        0        0     1349 2023-06-11 00:16:32.321610 bookio_fetchfox-0.7.3/fetchfox/apis/algorand/nfdomains.py
--rw-r--r--   0        0        0     1764 2023-06-11 00:16:32.321610 bookio_fetchfox-0.7.3/fetchfox/apis/algorand/nftexplorerapp.py
--rw-r--r--   0        0        0      592 2023-06-11 00:16:32.321610 bookio_fetchfox-0.7.3/fetchfox/apis/algorand/randswapcom.py
--rw-r--r--   0        0        0      262 2023-06-11 00:16:32.321610 bookio_fetchfox-0.7.3/fetchfox/apis/bookio.py
--rw-r--r--   0        0        0        0 2023-06-11 00:16:32.321610 bookio_fetchfox-0.7.3/fetchfox/apis/cardano/__init__.py
--rw-r--r--   0        0        0     2658 2023-06-11 00:16:32.321610 bookio_fetchfox-0.7.3/fetchfox/apis/cardano/blockfrostio.py
--rw-r--r--   0        0        0      734 2023-06-11 00:16:32.321610 bookio_fetchfox-0.7.3/fetchfox/apis/cardano/cnfttools.py
--rw-r--r--   0        0        0     1056 2023-06-11 00:16:32.321610 bookio_fetchfox-0.7.3/fetchfox/apis/cardano/handleme.py
--rw-r--r--   0        0        0     1606 2023-06-11 00:16:32.321610 bookio_fetchfox-0.7.3/fetchfox/apis/cardano/jpgstore.py
--rwxr-xr-x   0        0        0      675 2023-06-11 00:16:32.321610 bookio_fetchfox-0.7.3/fetchfox/apis/coingeckocom.py
--rw-r--r--   0        0        0        0 2023-06-11 00:16:32.321610 bookio_fetchfox-0.7.3/fetchfox/apis/evm/__init__.py
--rw-r--r--   0        0        0      963 2023-06-11 00:16:32.321610 bookio_fetchfox-0.7.3/fetchfox/apis/evm/ensideascom.py
--rw-r--r--   0        0        0     4147 2023-06-11 00:16:32.321610 bookio_fetchfox-0.7.3/fetchfox/apis/evm/moralisio.py
--rw-r--r--   0        0        0     2555 2023-06-11 00:16:32.321610 bookio_fetchfox-0.7.3/fetchfox/apis/evm/openseaio.py
--rw-r--r--   0        0        0      120 2023-06-11 00:16:32.321610 bookio_fetchfox-0.7.3/fetchfox/blockchains/__init__.py
--rw-r--r--   0        0        0       33 2023-06-11 00:16:32.321610 bookio_fetchfox-0.7.3/fetchfox/blockchains/algorand/__init__.py
--rw-r--r--   0        0        0     8433 2023-06-11 00:16:32.321610 bookio_fetchfox-0.7.3/fetchfox/blockchains/algorand/blockchain.py
--rw-r--r--   0        0        0      504 2023-06-11 00:16:32.321610 bookio_fetchfox-0.7.3/fetchfox/blockchains/algorand/utils.py
--rw-r--r--   0        0        0     2380 2023-06-11 00:16:32.321610 bookio_fetchfox-0.7.3/fetchfox/blockchains/base.py
--rw-r--r--   0        0        0       32 2023-06-11 00:16:32.321610 bookio_fetchfox-0.7.3/fetchfox/blockchains/cardano/__init__.py
--rw-r--r--   0        0        0    12449 2023-06-11 00:16:32.321610 bookio_fetchfox-0.7.3/fetchfox/blockchains/cardano/blockchain.py
--rw-r--r--   0        0        0     1061 2023-06-11 00:16:32.321610 bookio_fetchfox-0.7.3/fetchfox/blockchains/cardano/utils.py
--rw-r--r--   0        0        0       33 2023-06-11 00:16:32.321610 bookio_fetchfox-0.7.3/fetchfox/blockchains/ethereum/__init__.py
--rw-r--r--   0        0        0      666 2023-06-11 00:16:32.321610 bookio_fetchfox-0.7.3/fetchfox/blockchains/ethereum/blockchain.py
--rw-r--r--   0        0        0       28 2023-06-11 00:16:32.321610 bookio_fetchfox-0.7.3/fetchfox/blockchains/evm/__init__.py
--rw-r--r--   0        0        0     9983 2023-06-11 00:16:32.321610 bookio_fetchfox-0.7.3/fetchfox/blockchains/evm/blockchain.py
--rw-r--r--   0        0        0      619 2023-06-11 00:16:32.321610 bookio_fetchfox-0.7.3/fetchfox/blockchains/evm/utils.py
--rw-r--r--   0        0        0       32 2023-06-11 00:16:32.321610 bookio_fetchfox-0.7.3/fetchfox/blockchains/polygon/__init__.py
--rw-r--r--   0        0        0      670 2023-06-11 00:16:32.321610 bookio_fetchfox-0.7.3/fetchfox/blockchains/polygon/blockchain.py
--rw-r--r--   0        0        0      154 2023-06-11 00:16:32.321610 bookio_fetchfox-0.7.3/fetchfox/blockchains/utils.py
--rw-r--r--   0        0        0      322 2023-06-11 00:16:32.321610 bookio_fetchfox-0.7.3/fetchfox/checks.py
--rw-r--r--   0        0        0        0 2023-06-11 00:16:32.321610 bookio_fetchfox-0.7.3/fetchfox/constants/__init__.py
--rw-r--r--   0        0        0      158 2023-06-11 00:16:32.321610 bookio_fetchfox-0.7.3/fetchfox/constants/blockchains.py
--rw-r--r--   0        0        0      112 2023-06-11 00:16:32.321610 bookio_fetchfox-0.7.3/fetchfox/constants/currencies.py
--rw-r--r--   0        0        0      296 2023-06-11 00:16:32.321610 bookio_fetchfox-0.7.3/fetchfox/constants/marketplaces.py
--rw-r--r--   0        0        0       95 2023-06-11 00:16:32.321610 bookio_fetchfox-0.7.3/fetchfox/constants/sales.py
--rw-r--r--   0        0        0       28 2023-06-11 00:16:32.321610 bookio_fetchfox-0.7.3/fetchfox/constants/specials.py
--rw-r--r--   0        0        0      216 2023-06-11 00:16:32.321610 bookio_fetchfox-0.7.3/fetchfox/dtos/__init__.py
--rw-r--r--   0        0        0     2263 2023-06-11 00:16:32.321610 bookio_fetchfox-0.7.3/fetchfox/dtos/asset.py
--rw-r--r--   0        0        0     3435 2023-06-11 00:16:32.321610 bookio_fetchfox-0.7.3/fetchfox/dtos/campaign.py
--rw-r--r--   0        0        0      285 2023-06-11 00:16:32.321610 bookio_fetchfox-0.7.3/fetchfox/dtos/floor.py
--rw-r--r--   0        0        0      463 2023-06-11 00:16:32.321610 bookio_fetchfox-0.7.3/fetchfox/dtos/holding.py
--rw-r--r--   0        0        0     1586 2023-06-11 00:16:32.321610 bookio_fetchfox-0.7.3/fetchfox/dtos/listing.py
--rw-r--r--   0        0        0      365 2023-06-11 00:16:32.321610 bookio_fetchfox-0.7.3/fetchfox/dtos/rank.py
--rw-r--r--   0        0        0     1969 2023-06-11 00:16:32.321610 bookio_fetchfox-0.7.3/fetchfox/dtos/sale.py
--rw-r--r--   0        0        0        0 2023-06-11 00:16:32.321610 bookio_fetchfox-0.7.3/fetchfox/helpers/__init__.py
--rw-r--r--   0        0        0      150 2023-06-11 00:16:32.321610 bookio_fetchfox-0.7.3/fetchfox/helpers/formatters.py
--rw-r--r--   0        0        0     1895 2023-06-11 00:16:32.321610 bookio_fetchfox-0.7.3/fetchfox/rest.py
--rw-r--r--   0        0        0     1148 2023-06-11 00:16:32.333610 bookio_fetchfox-0.7.3/pyproject.toml
--rw-r--r--   0        0        0     4986 1970-01-01 00:00:00.000000 bookio_fetchfox-0.7.3/setup.py
--rw-r--r--   0        0        0     4938 1970-01-01 00:00:00.000000 bookio_fetchfox-0.7.3/PKG-INFO
+-rw-r--r--   0        0        0     3723 2023-06-12 20:53:50.099279 bookio_fetchfox-0.7.5/README.md
+-rw-r--r--   0        0        0        0 2023-06-12 20:53:50.099279 bookio_fetchfox-0.7.5/fetchfox/__init__.py
+-rw-r--r--   0        0        0        0 2023-06-12 20:53:50.099279 bookio_fetchfox-0.7.5/fetchfox/apis/__init__.py
+-rw-r--r--   0        0        0        0 2023-06-12 20:53:50.099279 bookio_fetchfox-0.7.5/fetchfox/apis/algorand/__init__.py
+-rw-r--r--   0        0        0     2156 2023-06-12 20:53:50.099279 bookio_fetchfox-0.7.5/fetchfox/apis/algorand/algonodecloud.py
+-rw-r--r--   0        0        0      604 2023-06-12 20:53:50.099279 bookio_fetchfox-0.7.5/fetchfox/apis/algorand/algoxnftcom.py
+-rw-r--r--   0        0        0     1357 2023-06-12 20:53:50.099279 bookio_fetchfox-0.7.5/fetchfox/apis/algorand/nfdomains.py
+-rw-r--r--   0        0        0     1780 2023-06-12 20:53:50.099279 bookio_fetchfox-0.7.5/fetchfox/apis/algorand/nftexplorerapp.py
+-rw-r--r--   0        0        0      600 2023-06-12 20:53:50.103280 bookio_fetchfox-0.7.5/fetchfox/apis/algorand/randswapcom.py
+-rw-r--r--   0        0        0      262 2023-06-12 20:53:50.103280 bookio_fetchfox-0.7.5/fetchfox/apis/bookio.py
+-rw-r--r--   0        0        0        0 2023-06-12 20:53:50.103280 bookio_fetchfox-0.7.5/fetchfox/apis/cardano/__init__.py
+-rw-r--r--   0        0        0     2658 2023-06-12 20:53:50.103280 bookio_fetchfox-0.7.5/fetchfox/apis/cardano/blockfrostio.py
+-rw-r--r--   0        0        0      734 2023-06-12 20:53:50.103280 bookio_fetchfox-0.7.5/fetchfox/apis/cardano/cnfttools.py
+-rw-r--r--   0        0        0     1056 2023-06-12 20:53:50.103280 bookio_fetchfox-0.7.5/fetchfox/apis/cardano/handleme.py
+-rw-r--r--   0        0        0     1647 2023-06-12 20:53:50.103280 bookio_fetchfox-0.7.5/fetchfox/apis/cardano/jpgstore.py
+-rwxr-xr-x   0        0        0      683 2023-06-12 20:53:50.103280 bookio_fetchfox-0.7.5/fetchfox/apis/coingeckocom.py
+-rw-r--r--   0        0        0        0 2023-06-12 20:53:50.103280 bookio_fetchfox-0.7.5/fetchfox/apis/evm/__init__.py
+-rw-r--r--   0        0        0      963 2023-06-12 20:53:50.103280 bookio_fetchfox-0.7.5/fetchfox/apis/evm/ensideascom.py
+-rw-r--r--   0        0        0     4277 2023-06-12 20:53:50.103280 bookio_fetchfox-0.7.5/fetchfox/apis/evm/moralisio.py
+-rw-r--r--   0        0        0     2725 2023-06-12 20:53:50.103280 bookio_fetchfox-0.7.5/fetchfox/apis/evm/openseaio.py
+-rw-r--r--   0        0        0      120 2023-06-12 20:53:50.103280 bookio_fetchfox-0.7.5/fetchfox/blockchains/__init__.py
+-rw-r--r--   0        0        0       33 2023-06-12 20:53:50.103280 bookio_fetchfox-0.7.5/fetchfox/blockchains/algorand/__init__.py
+-rw-r--r--   0        0        0     8903 2023-06-12 20:53:50.103280 bookio_fetchfox-0.7.5/fetchfox/blockchains/algorand/blockchain.py
+-rw-r--r--   0        0        0      501 2023-06-12 20:53:50.103280 bookio_fetchfox-0.7.5/fetchfox/blockchains/algorand/utils.py
+-rw-r--r--   0        0        0     2459 2023-06-12 20:53:50.103280 bookio_fetchfox-0.7.5/fetchfox/blockchains/base.py
+-rw-r--r--   0        0        0       32 2023-06-12 20:53:50.103280 bookio_fetchfox-0.7.5/fetchfox/blockchains/cardano/__init__.py
+-rw-r--r--   0        0        0    12945 2023-06-12 20:53:50.103280 bookio_fetchfox-0.7.5/fetchfox/blockchains/cardano/blockchain.py
+-rw-r--r--   0        0        0     1043 2023-06-12 20:53:50.103280 bookio_fetchfox-0.7.5/fetchfox/blockchains/cardano/utils.py
+-rw-r--r--   0        0        0       33 2023-06-12 20:53:50.103280 bookio_fetchfox-0.7.5/fetchfox/blockchains/ethereum/__init__.py
+-rw-r--r--   0        0        0     1394 2023-06-12 20:53:50.103280 bookio_fetchfox-0.7.5/fetchfox/blockchains/ethereum/blockchain.py
+-rw-r--r--   0        0        0       28 2023-06-12 20:53:50.103280 bookio_fetchfox-0.7.5/fetchfox/blockchains/evm/__init__.py
+-rw-r--r--   0        0        0     9864 2023-06-12 20:53:50.103280 bookio_fetchfox-0.7.5/fetchfox/blockchains/evm/blockchain.py
+-rw-r--r--   0        0        0      616 2023-06-12 20:53:50.103280 bookio_fetchfox-0.7.5/fetchfox/blockchains/evm/utils.py
+-rw-r--r--   0        0        0       32 2023-06-12 20:53:50.103280 bookio_fetchfox-0.7.5/fetchfox/blockchains/polygon/__init__.py
+-rw-r--r--   0        0        0     1398 2023-06-12 20:53:50.103280 bookio_fetchfox-0.7.5/fetchfox/blockchains/polygon/blockchain.py
+-rw-r--r--   0        0        0      146 2023-06-12 20:53:50.103280 bookio_fetchfox-0.7.5/fetchfox/blockchains/utils.py
+-rw-r--r--   0        0        0      322 2023-06-12 20:53:50.103280 bookio_fetchfox-0.7.5/fetchfox/checks.py
+-rw-r--r--   0        0        0        0 2023-06-12 20:53:50.103280 bookio_fetchfox-0.7.5/fetchfox/constants/__init__.py
+-rw-r--r--   0        0        0      158 2023-06-12 20:53:50.103280 bookio_fetchfox-0.7.5/fetchfox/constants/blockchains.py
+-rw-r--r--   0        0        0      112 2023-06-12 20:53:50.103280 bookio_fetchfox-0.7.5/fetchfox/constants/currencies.py
+-rw-r--r--   0        0        0      296 2023-06-12 20:53:50.103280 bookio_fetchfox-0.7.5/fetchfox/constants/marketplaces.py
+-rw-r--r--   0        0        0       95 2023-06-12 20:53:50.103280 bookio_fetchfox-0.7.5/fetchfox/constants/sales.py
+-rw-r--r--   0        0        0       28 2023-06-12 20:53:50.103280 bookio_fetchfox-0.7.5/fetchfox/constants/specials.py
+-rw-r--r--   0        0        0      216 2023-06-12 20:53:50.103280 bookio_fetchfox-0.7.5/fetchfox/dtos/__init__.py
+-rw-r--r--   0        0        0     2263 2023-06-12 20:53:50.103280 bookio_fetchfox-0.7.5/fetchfox/dtos/asset.py
+-rw-r--r--   0        0        0     3435 2023-06-12 20:53:50.103280 bookio_fetchfox-0.7.5/fetchfox/dtos/campaign.py
+-rw-r--r--   0        0        0      285 2023-06-12 20:53:50.103280 bookio_fetchfox-0.7.5/fetchfox/dtos/floor.py
+-rw-r--r--   0        0        0      463 2023-06-12 20:53:50.103280 bookio_fetchfox-0.7.5/fetchfox/dtos/holding.py
+-rw-r--r--   0        0        0     1586 2023-06-12 20:53:50.103280 bookio_fetchfox-0.7.5/fetchfox/dtos/listing.py
+-rw-r--r--   0        0        0      365 2023-06-12 20:53:50.103280 bookio_fetchfox-0.7.5/fetchfox/dtos/rank.py
+-rw-r--r--   0        0        0     1969 2023-06-12 20:53:50.103280 bookio_fetchfox-0.7.5/fetchfox/dtos/sale.py
+-rw-r--r--   0        0        0        0 2023-06-12 20:53:50.103280 bookio_fetchfox-0.7.5/fetchfox/helpers/__init__.py
+-rw-r--r--   0        0        0      150 2023-06-12 20:53:50.103280 bookio_fetchfox-0.7.5/fetchfox/helpers/formatters.py
+-rw-r--r--   0        0        0     1895 2023-06-12 20:53:50.103280 bookio_fetchfox-0.7.5/fetchfox/rest.py
+-rw-r--r--   0        0        0     1148 2023-06-12 20:53:50.115280 bookio_fetchfox-0.7.5/pyproject.toml
+-rw-r--r--   0        0        0     4986 1970-01-01 00:00:00.000000 bookio_fetchfox-0.7.5/setup.py
+-rw-r--r--   0        0        0     4938 1970-01-01 00:00:00.000000 bookio_fetchfox-0.7.5/PKG-INFO
```

### Comparing `bookio_fetchfox-0.7.3/README.md` & `bookio_fetchfox-0.7.5/README.md`

 * *Files identical despite different names*

### Comparing `bookio_fetchfox-0.7.3/fetchfox/apis/algorand/algonodecloud.py` & `bookio_fetchfox-0.7.5/fetchfox/apis/algorand/algonodecloud.py`

 * *Files 2% similar despite different names*

```diff
@@ -13,15 +13,15 @@
         url=f"{BASE_URL}/v{version}/{service}",
         params=params or {},
     )
 
 
 def get_assets(creator_address: str) -> Iterable[str]:
     check_str(creator_address, "algonodecloud.creator_address")
-    creator_address = creator_address.upper()
+    creator_address = creator_address.strip().upper()
 
     response, status_code = get(f"accounts/{creator_address}")
 
     assets = sorted(
         response["account"].get("created-assets", []),
         key=lambda a: a["index"],
         reverse=True,
@@ -54,15 +54,15 @@
     response, status_code = get(f"assets/{asset_id}")
 
     return response["asset"]["params"]
 
 
 def get_holdings(address: str) -> Iterable[dict]:
     check_str(address, "algonodecloud.address")
-    address = address.upper()
+    address = address.strip().upper()
 
     response, status_code = get(f"accounts/{address}")
 
     account = response["account"]
 
     for asset in account.get("assets", []):
         yield asset
```

### Comparing `bookio_fetchfox-0.7.3/fetchfox/apis/algorand/algoxnftcom.py` & `bookio_fetchfox-0.7.5/fetchfox/apis/algorand/randswapcom.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,22 +1,22 @@
 from typing import Iterable, Tuple
 
 from fetchfox import rest
 from fetchfox.checks import check_str
 
-BASE_URL = "https://api.algoxnft.com"
+BASE_URL = "https://www.randswap.com"
 
 
 def get(service: str, params: dict = None, version: int = 1) -> Tuple[dict, int]:
     return rest.get(
         url=f"{BASE_URL}/v{version}/{service}",
         params=params or {},
     )
 
 
 def get_listings(creator_address: str) -> Iterable[dict]:
-    check_str(creator_address, "algoxnftcom.creator_address")
-    creator_address = creator_address.upper()
+    check_str(creator_address, "randswapcom.creator_address")
+    creator_address = creator_address.strip().upper()
 
-    response, status_code = get(f"nft-explorer/creator/{creator_address}")
+    response, status_code = get(f"listings/creator/{creator_address}")
 
     yield from response
```

### Comparing `bookio_fetchfox-0.7.3/fetchfox/apis/algorand/nfdomains.py` & `bookio_fetchfox-0.7.5/fetchfox/apis/algorand/nfdomains.py`

 * *Files 4% similar despite different names*

```diff
@@ -37,15 +37,15 @@
 
     return address
 
 
 @lru_cache
 def get_nf_domain(address: str):
     check_str(address, "nfddomains.address")
-    address = address.upper()
+    address = address.strip().upper()
 
     response, status_code = get(
         f"nfd/v2/address",
         params={
             "address": address,
         },
     )
```

### Comparing `bookio_fetchfox-0.7.3/fetchfox/apis/algorand/nftexplorerapp.py` & `bookio_fetchfox-0.7.5/fetchfox/apis/algorand/nftexplorerapp.py`

 * *Files 7% similar despite different names*

```diff
@@ -19,15 +19,15 @@
         sleep=1,
     )
 
 
 @lru_cache
 def get_collection_id(creator_address: str, api_key: str) -> str:
     check_str(creator_address, "randswap.creator_address")
-    creator_address = creator_address.upper()
+    creator_address = creator_address.strip().upper()
 
     response, status_code = get(
         "collections/search",
         params={
             "q": creator_address,
         },
         api_key=api_key,
@@ -44,15 +44,15 @@
         return recognized[0]["collectionId"]
 
     return None
 
 
 def get_sales(creator_address: str, api_key: str) -> Iterable[dict]:
     check_str(creator_address, "randswap.creator_address")
-    creator_address = creator_address.upper()
+    creator_address = creator_address.strip().upper()
 
     collection_id = get_collection_id(creator_address, api_key)
 
     next_token = None
 
     while True:
         response, status_code = get(
```

### Comparing `bookio_fetchfox-0.7.3/fetchfox/apis/algorand/randswapcom.py` & `bookio_fetchfox-0.7.5/fetchfox/apis/algorand/algoxnftcom.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,22 +1,22 @@
 from typing import Iterable, Tuple
 
 from fetchfox import rest
 from fetchfox.checks import check_str
 
-BASE_URL = "https://www.randswap.com"
+BASE_URL = "https://api.algoxnft.com"
 
 
 def get(service: str, params: dict = None, version: int = 1) -> Tuple[dict, int]:
     return rest.get(
         url=f"{BASE_URL}/v{version}/{service}",
         params=params or {},
     )
 
 
 def get_listings(creator_address: str) -> Iterable[dict]:
-    check_str(creator_address, "randswapcom.creator_address")
-    creator_address = creator_address.upper()
+    check_str(creator_address, "algoxnftcom.creator_address")
+    creator_address = creator_address.strip().upper()
 
-    response, status_code = get(f"listings/creator/{creator_address}")
+    response, status_code = get(f"nft-explorer/creator/{creator_address}")
 
     yield from response
```

### Comparing `bookio_fetchfox-0.7.3/fetchfox/apis/cardano/blockfrostio.py` & `bookio_fetchfox-0.7.5/fetchfox/apis/cardano/blockfrostio.py`

 * *Files identical despite different names*

### Comparing `bookio_fetchfox-0.7.3/fetchfox/apis/cardano/cnfttools.py` & `bookio_fetchfox-0.7.5/fetchfox/apis/cardano/cnfttools.py`

 * *Files identical despite different names*

### Comparing `bookio_fetchfox-0.7.3/fetchfox/apis/cardano/handleme.py` & `bookio_fetchfox-0.7.5/fetchfox/apis/cardano/handleme.py`

 * *Files identical despite different names*

### Comparing `bookio_fetchfox-0.7.3/fetchfox/apis/cardano/jpgstore.py` & `bookio_fetchfox-0.7.5/fetchfox/apis/cardano/jpgstore.py`

 * *Files 8% similar despite different names*

```diff
@@ -60,18 +60,20 @@
             f"collection/{policy_id}/transactions",
             params={
                 "page": page,
                 "count": 50,
             },
         )
 
-        if not response:  # pragma: no cover
+        transactions = response["transactions"]
+
+        if not transactions:  # pragma: no cover
             break
 
-        for sale in response["transactions"]:
+        for sale in transactions:
             tx_hash = sale["tx_hash"]
 
             if tx_hash in txs:
                 continue
 
             txs.add(tx_hash)
```

### Comparing `bookio_fetchfox-0.7.3/fetchfox/apis/evm/ensideascom.py` & `bookio_fetchfox-0.7.5/fetchfox/apis/evm/ensideascom.py`

 * *Files identical despite different names*

### Comparing `bookio_fetchfox-0.7.3/fetchfox/apis/evm/moralisio.py` & `bookio_fetchfox-0.7.5/fetchfox/apis/evm/moralisio.py`

 * *Files 12% similar despite different names*

```diff
@@ -49,22 +49,18 @@
 
         if not response.get("cursor"):
             break
 
         cursor = response["cursor"]
 
 
-def resync_metadata(
-    contract_address: str,
-    asset_id: str,
-    blockchain: str,
-    api_key: str,
-):
+def resync_metadata(contract_address: str, asset_id: str, blockchain: str, api_key: str):
     check_str(contract_address, "moralisio.contract_address")
     check_str(asset_id, "moralisio.asset_id")
+    contract_address = contract_address.strip().lower()
 
     response, status_code = get(
         f"nft/{contract_address}/{asset_id}/metadata/resync",
         params={
             "flag": "uri",
             "mode": "sync",
         },
@@ -74,22 +70,18 @@
 
     if status_code == 404:
         raise ValueError(f"{contract_address}/{asset_id} doesn't exist")
 
     return response.get("status")
 
 
-def get_asset_data(
-    contract_address: str,
-    asset_id: str,
-    blockchain: str,
-    api_key: str,
-) -> dict:
+def get_asset_data(contract_address: str, asset_id: str, blockchain: str, api_key: str) -> dict:
     check_str(contract_address, "moralisio.contract_address")
     check_str(asset_id, "moralisio.asset_id")
+    contract_address = contract_address.strip().lower()
 
     response, status_code = get(
         f"nft/{contract_address}/{asset_id}",
         blockchain=blockchain,
         api_key=api_key,
     )
 
@@ -132,14 +124,15 @@
             break
 
         cursor = response["cursor"]
 
 
 def get_owners(contract_address: str, blockchain: str, api_key: str) -> Iterable[dict]:
     check_str(contract_address, "moralisio.contract_address")
+    contract_address = contract_address.strip().lower()
 
     cursor = ""
 
     while True:
         response, status_code = get(
             f"nft/{contract_address}/owners",
             params={
```

### Comparing `bookio_fetchfox-0.7.3/fetchfox/apis/evm/openseaio.py` & `bookio_fetchfox-0.7.5/fetchfox/apis/evm/openseaio.py`

 * *Files 6% similar despite different names*

```diff
@@ -27,14 +27,15 @@
         sleep=1.5,
     )
 
 
 @lru_cache
 def get_slug(contract_address: str, api_key) -> str:
     check_str(contract_address, "openseaio.contract_address")
+    contract_address = contract_address.strip().lower()
 
     logger.info("fetching slug for %s", contract_address)
 
     response, status_code = get(
         "events",
         params={
             "asset_contract_address": contract_address,
@@ -45,14 +46,16 @@
         api_key=api_key,
     )
 
     return response["asset_events"][0]["collection_slug"]
 
 
 def get_events(contract_address: str, event_type: str, api_key: str, slug: str = None) -> Iterable[dict]:
+    contract_address = contract_address.strip().lower()
+
     if not slug:
         slug = get_slug(contract_address, api_key=api_key)
 
     cursor = ""
 
     while True:
         response, status_code = get(
@@ -81,14 +84,16 @@
         event_type="successful",
         api_key=api_key,
         slug=slug,
     )
 
 
 def get_listings(contract_address: str, api_key: str, slug: str = None) -> Iterable[dict]:
+    contract_address = contract_address.strip().lower()
+
     if not slug:
         slug = get_slug(contract_address, api_key=api_key)
 
     cursor = ""
 
     while True:
         response, status_code = get(
```

### Comparing `bookio_fetchfox-0.7.3/fetchfox/blockchains/algorand/blockchain.py` & `bookio_fetchfox-0.7.5/fetchfox/blockchains/algorand/blockchain.py`

 * *Files 6% similar despite different names*

```diff
@@ -44,19 +44,34 @@
         if not utils.is_asset_id(asset_id):
             raise ValueError(f"{asset_id} is not a valid algorand asset id")
 
     def check_wallet(self, wallet: str):
         if not utils.is_wallet(wallet):
             raise ValueError(f"{wallet} is not a valid algorand address or nfdomain")
 
-    def explorer_url(self, collection_id: str) -> str:
-        return f"https://algoexplorer.io/address/{collection_id}"
+    def explorer_url(self, collection_id: str = None, asset_id: str = None, tx_hash: str = None) -> str:
+        if asset_id:
+            return f"https://algoexplorer.io/asset/{asset_id}"
 
-    def marketplace_url(self, collection_id: str) -> str:
-        return f"https://randgallery.com/algo-collection/?address={collection_id}"
+        if collection_id:
+            return f"https://algoexplorer.io/address/{collection_id.upper()}"
+
+        if tx_hash:
+            return f"https://algoexplorer.io/tx/{tx_hash.upper()}"
+
+        return None
+
+    def marketplace_url(self, collection_id: str = None, asset_id: str = None) -> str:
+        if asset_id:
+            return f"https://www.randgallery.com/algo-collection/?address={asset_id}"
+
+        if collection_id:
+            return f"https://randgallery.com/algo-collection/?address={collection_id}"
+
+        return None
 
     def get_assets(self, collection_id: str, fetch_metadata: bool = True, *args, **kwargs) -> Iterable[AssetDTO]:
         self.check_collection_id(collection_id)
 
         for asset_id in algonodecloud.get_assets(collection_id):
             if fetch_metadata:
                 yield self.get_asset(
```

### Comparing `bookio_fetchfox-0.7.3/fetchfox/blockchains/base.py` & `bookio_fetchfox-0.7.5/fetchfox/blockchains/base.py`

 * *Files 24% similar despite different names*

```diff
@@ -31,19 +31,19 @@
         raise NotImplementedError()
 
     @abstractmethod
     def check_wallet(self, wallet: str):
         raise NotImplementedError()
 
     @abstractmethod
-    def explorer_url(self, collection_id: str) -> str:
+    def explorer_url(self, collection_id: str = None, asset_id: str = None, tx_hash: str = None) -> str:
         raise NotImplementedError()
 
     @abstractmethod
-    def marketplace_url(self, collection_id: str) -> str:
+    def marketplace_url(self, collection_id: str = None, asset_id: str = None) -> str:
         raise NotImplementedError()
 
     @abstractmethod
     def get_assets(self, collection_id: str, fetch_metadata: bool = True, *args, **kwargs) -> Iterable[AssetDTO]:
         raise NotImplementedError()
 
     @abstractmethod
```

### Comparing `bookio_fetchfox-0.7.3/fetchfox/blockchains/cardano/blockchain.py` & `bookio_fetchfox-0.7.5/fetchfox/blockchains/cardano/blockchain.py`

 * *Files 3% similar despite different names*

```diff
@@ -47,19 +47,34 @@
         if not utils.is_asset_id(asset_id):
             raise ValueError(f"{asset_id} is not a valid cardano asset id")
 
     def check_wallet(self, wallet: str):
         if not utils.is_wallet(wallet):
             raise ValueError(f"{wallet} is not a valid cardano address, stake key or ada handle")
 
-    def explorer_url(self, collection_id: str) -> str:
-        return f"https://cardanoscan.io/tokenPolicy/{collection_id}"
+    def explorer_url(self, collection_id: str = None, asset_id: str = None, tx_hash: str = None) -> str:
+        if asset_id:
+            return f"https://cardanoscan.io/token/{asset_id.lower()}"
 
-    def marketplace_url(self, collection_id: str) -> str:
-        return f"https://jpg.store/collection/{collection_id}"
+        if collection_id:
+            return f"https://cardanoscan.io/tokenPolicy/{collection_id.lower()}"
+
+        if tx_hash:
+            return f"https://cardanoscan.io/transaction/{collection_id.lower()}"
+
+        return None
+
+    def marketplace_url(self, collection_id: str = None, asset_id: str = None) -> str:
+        if asset_id:
+            return f"https://www.jpg.store/asset/{asset_id.lower()}"
+
+        if collection_id:
+            return f"https://jpg.store/collection/{collection_id.lower()}"
+
+        return None
 
     @lru_cache
     def get_stake_key(self, wallet: str) -> str:
         self.check_wallet(wallet)
 
         if utils.is_stake_key(wallet):
             return wallet
@@ -139,15 +154,15 @@
                 description=campaign["landing"]["opener"],
                 price=landing["price"],
                 supply=campaign["total_deas"],
                 pricing=pricing,
                 limit=campaign["max_quantity"],
                 start_at=formatters.timestamp(start_at["start_at"]),
                 explorer_url=f"https://pool.pm/nfts/{collection_id}",
-                marketplace_url=self.marketplace_url(collection_id),
+                marketplace_url=self.marketplace_url(collection_id=collection_id),
                 rarity_chart_url=landing["rarity_chart_url"],
             )
 
     def get_holdings(self, wallet: str, *args, **kwargs) -> Iterable[HoldingDTO]:
         self.check_wallet(wallet)
 
         stake_address = self.get_stake_key(wallet)
```

### Comparing `bookio_fetchfox-0.7.3/fetchfox/blockchains/cardano/utils.py` & `bookio_fetchfox-0.7.5/fetchfox/blockchains/cardano/utils.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,17 +1,17 @@
 from typing import Tuple
 
 from fetchfox.blockchains.utils import check
 
-ADA_HANDLE_REGEX = r"^\$[a-zA-Z0-9\-_.]{1,15}$"
-SHORT_ADDRESS_REGEX = r"^addr1[0-9a-zA-Z]{53}$"
-LONG_ADDRESS_REGEX = r"^addr1[0-9a-zA-Z]{98}$"
-ASSET_ID_REGEX = r"^[a-fA-F0-9]{56}[a-fA-F0-9]+$"
-POLICY_ID_REGEX = r"^[a-fA-F0-9]{56}$"
-STAKE_KEY_REGEX = r"^stake1[0-9a-zA-Z]{53}$"
+ADA_HANDLE_REGEX = r"^\$[a-z0-9\-_.]{1,15}$"
+SHORT_ADDRESS_REGEX = r"^addr1[0-9a-z]{53}$"
+LONG_ADDRESS_REGEX = r"^addr1[0-9a-z]{98}$"
+ASSET_ID_REGEX = r"^[a-f0-9]{56}[a-fA-F0-9]+$"
+POLICY_ID_REGEX = r"^[a-f0-9]{56}$"
+STAKE_KEY_REGEX = r"^stake1[0-9a-z]{53}$"
 
 
 def is_ada_handle(string: str) -> bool:
     return check(ADA_HANDLE_REGEX, string)
 
 
 def is_address(string) -> bool:
```

### Comparing `bookio_fetchfox-0.7.3/fetchfox/blockchains/evm/blockchain.py` & `bookio_fetchfox-0.7.5/fetchfox/blockchains/evm/blockchain.py`

 * *Files 3% similar despite different names*

```diff
@@ -32,17 +32,14 @@
         if not utils.is_asset_id(asset_id):
             raise ValueError(f"{asset_id} is not a valid {self.name} asset id")
 
     def check_wallet(self, wallet: str):
         if not utils.is_wallet(wallet):
             raise ValueError(f"{wallet} is not a valid {self.name} address or ens domain")
 
-    def marketplace_url(self, collection_id: str) -> str:
-        return f"https://opensea.io/assets?search[query]={collection_id}"
-
     def get_assets(self, collection_id: str, fetch_metadata: bool = True, *args, **kwargs) -> Iterable[AssetDTO]:
         self.check_collection_id(collection_id)
 
         if fetch_metadata:
             asset_id = -1
 
             while True:
@@ -118,15 +115,15 @@
                 description=campaign["landing"]["opener"],
                 price=landing["price"],
                 supply=campaign["total_deas"],
                 pricing=landing["price_description"],
                 limit=campaign["max_quantity"],
                 start_at=formatters.timestamp(start_at["start_at"]),
                 explorer_url=self.explorer_url(collection_id),
-                marketplace_url=self.marketplace_url(collection_id),
+                marketplace_url=self.marketplace_url(collection_id=collection_id),
                 rarity_chart_url=landing["rarity_chart_url"],
             )
 
     def get_holdings(self, wallet: str, *args, **kwargs) -> Iterable[HoldingDTO]:
         self.check_wallet(wallet)
 
         if utils.is_ens_domain(wallet):
```

### Comparing `bookio_fetchfox-0.7.3/fetchfox/blockchains/evm/utils.py` & `bookio_fetchfox-0.7.5/fetchfox/blockchains/evm/utils.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 import re
 
 
-ADDRESS_REGEX = r"^0x[a-fA-F0-9]{40}$"
+ADDRESS_REGEX = r"^0x[a-f0-9]{40}$"
 ASSET_ID_REGEX = r"^[0-9]+$"
 ENS_DOMAIN_REGEX = r"^[a-z0-9]+([\-\.][a-z0-9]+)*\.eth$"
 
 
 def check(pattern, string: str) -> bool:
     if string is None:
         return False
```

### Comparing `bookio_fetchfox-0.7.3/fetchfox/dtos/asset.py` & `bookio_fetchfox-0.7.5/fetchfox/dtos/asset.py`

 * *Files identical despite different names*

### Comparing `bookio_fetchfox-0.7.3/fetchfox/dtos/campaign.py` & `bookio_fetchfox-0.7.5/fetchfox/dtos/campaign.py`

 * *Files identical despite different names*

### Comparing `bookio_fetchfox-0.7.3/fetchfox/dtos/listing.py` & `bookio_fetchfox-0.7.5/fetchfox/dtos/listing.py`

 * *Files identical despite different names*

### Comparing `bookio_fetchfox-0.7.3/fetchfox/dtos/sale.py` & `bookio_fetchfox-0.7.5/fetchfox/dtos/sale.py`

 * *Files identical despite different names*

### Comparing `bookio_fetchfox-0.7.3/fetchfox/rest.py` & `bookio_fetchfox-0.7.5/fetchfox/rest.py`

 * *Files identical despite different names*

### Comparing `bookio_fetchfox-0.7.3/pyproject.toml` & `bookio_fetchfox-0.7.5/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "bookio-fetchfox"
-version = "0.7.3"
+version = "0.7.5"
 description = "Collection of API services to fetch information from several blockchains."
 documentation = "https://github.com/book-io/fetchfox/blob/main/README.md"
 homepage = "https://github.com/book-io/fetchfox"
 license = "MIT"
 readme = "README.md"
 
 authors = [
```

### Comparing `bookio_fetchfox-0.7.3/setup.py` & `bookio_fetchfox-0.7.5/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -25,15 +25,15 @@
  'asyncio>=3.4.3,<4.0.0',
  'backoff>=2.2.1,<3.0.0',
  'cachetools>=5.3.1,<6.0.0',
  'pytz>=2023.3,<2024.0']
 
 setup_kwargs = {
     'name': 'bookio-fetchfox',
-    'version': '0.7.3',
+    'version': '0.7.5',
     'description': 'Collection of API services to fetch information from several blockchains.',
     'long_description': '# book.io / fetchfox\n\n> Collection of API services to fetch information from several blockchains.\n\n![](https://s2.coinmarketcap.com/static/img/coins/64x64/4030.png)\n![](https://s2.coinmarketcap.com/static/img/coins/64x64/2010.png)\n![](https://s2.coinmarketcap.com/static/img/coins/64x64/1027.png)\n![](https://s2.coinmarketcap.com/static/img/coins/64x64/3890.png)\n\n\n## Supported Blockchains\n\n### Algorand\n\n```python\nimport os\nfrom fetchfox.blockchains import Algorand\n\nalgorand = Algorand(\n    nftexplorerapp_api_key=os.getenv("NFTEXPLORER_API_KEY"),\n)\n\n# Brave New World\ncreator_address = "6WII6ES4H6UW7G7T7RJX63CUNPKJEPEGQ3PTYVVU3JHJ652W34GCJV5OVY"\n\nfor asset in algorand.get_assets(creator_address):\n    print(asset)\n```\n\n#### Services\n\n* get_asset ([algonode.cloud](https://algonode.cloud))\n* get_assets ([algonode.cloud](https://algonode.cloud))\n* get_holdings ([algonode.cloud](https://algonode.cloud))\n* get_snapshot ([algonode.cloud](https://algonode.cloud))\n* get_campaigns ([book.io](https://book.io))\n* get_listings ([randgallery.com](https://randgallery.com) / [algoxnft.com](https://algoxnft.com))\n* get_floor ([randgallery.com](https://randgallery.com) / [algoxnft.com](https://algoxnft.com))\n* get_sales ([nftexplorer.app¹](https://nftexplorer.app))\n\n\n### Cardano\n\n```python\nimport os\nfrom fetchfox.blockchains import Cardano\n\ncardano = Cardano(\n    blockfrostio_project_id=os.getenv("BLOCKFROST_PROJECT_ID"),\n)\n\n# Gutenberg Bible\npolicy_id = "477cec772adb1466b301fb8161f505aa66ed1ee8d69d3e7984256a43"\n\nfor asset in cardano.get_assets(policy_id):\n    print(asset)\n```\n\n#### Services\n\n* get_asset ([blockfrost.io²](https://blockfrost.io))\n* get_assets ([blockfrost.io²](https://blockfrost.io))\n* get_holdings ([blockfrost.io²](https://blockfrost.io))\n* get_campaigns ([book.io](https://book.io))\n* get_snapshot ([blockfrost.io²](https://blockfrost.io))\n* get_listings ([jpg.store](https://jpg.store))\n* get_floor ([jpg.store](https://jpg.store))\n* get_sales ([jpg.store](https://jpg.store))\n* get_ranks ([cnft.tools](https://cnft.tools))\n\n\n### EVM (Ethereum and Polygon)\n\n```python\nimport os\nfrom fetchfox.blockchains import Ethereum, Polygon\n\nethereum = Ethereum(\n    geckodriver_path=os.getenv("GECKODRIVER_PATH"),\n    moralisio_api_key=os.getenv("MORALIS_API_KEY"),\n    openseaio_api_key=os.getenv("OPENSEA_API_KEY"),\n)\n\npolygon = Polygon(\n    geckodriver_path=os.getenv("GECKODRIVER_PATH"),\n    moralisio_api_key=os.getenv("MORALIS_API_KEY"),\n    openseaio_api_key=os.getenv("OPENSEA_API_KEY"),\n)\n\n\n# Alice in Wonderland\ncontract_address = "0x919da7fef646226f88f70305201de392ff365059"\n\nfor asset in ethereum.get_assets(contract_address):\n    print(asset)\n\n# Art of War\ncontract_address = "0xb56010e0500e4f163758881603b8083996ae47ec"\n\nfor asset in polygon.get_assets(contract_address):\n    print(asset)\n```\n\n#### Services\n\n* get_asset ([moralis.io³](https://moralis.io))\n* get_assets ([moralis.io³](https://moralis.io))\n* get_holdings ([moralis.io³](https://moralis.io))\n* get_snapshot ([moralis.io³](https://moralis.io))\n* get_campaigns ([book.io](https://book.io))\n* get_listings ([opensea.io⁴](https://opensea.io))\n* get_floor ([opensea.io⁴](https://opensea.io))\n* get_sales ([opensea.io⁴](https://opensea.io))\n\n\n> ¹ **nftexplorer.app** services require an [api key](https://www.nftexplorer.app/nftx-api).\n> \n> ² **blockfrost.io** services require a [project id](https://blockfrost.dev/docs/overview/plans-and-billing).\n> \n> ³ **moralis.io** services require an [api key](https://moralis.io/pricing).\n> \n> ⁴ **opensea.io** some services also require an [api key](https://docs.opensea.io/reference/api-keys). \n\n---\n\n![fetch, the fox](https://i.imgur.com/fm6mqzS.png)\n> fetch, the fox\n\n',
     'author': 'Fede',
     'author_email': 'fede@book.io',
     'maintainer': 'None',
     'maintainer_email': 'None',
     'url': 'https://github.com/book-io/fetchfox',
```

### Comparing `bookio_fetchfox-0.7.3/PKG-INFO` & `bookio_fetchfox-0.7.5/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: bookio-fetchfox
-Version: 0.7.3
+Version: 0.7.5
 Summary: Collection of API services to fetch information from several blockchains.
 Home-page: https://github.com/book-io/fetchfox
 License: MIT
 Keywords: book.io,blockchain,crypto,algorand,cardano,ethereum,polygon
 Author: Fede
 Author-email: fede@book.io
 Requires-Python: >=3.8,<4.0
```

