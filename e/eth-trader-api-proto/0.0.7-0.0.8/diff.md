# Comparing `tmp/eth-trader-api-proto-0.0.7.tar.gz` & `tmp/eth-trader-api-proto-0.0.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "eth-trader-api-proto-0.0.7.tar", last modified: Thu Jun  1 13:57:36 2023, max compression
+gzip compressed data, was "eth-trader-api-proto-0.0.8.tar", last modified: Mon Jun 12 19:51:54 2023, max compression
```

## Comparing `eth-trader-api-proto-0.0.7.tar` & `eth-trader-api-proto-0.0.8.tar`

### file list

```diff
@@ -1,15 +1,15 @@
-drwxr-xr-x   0 atulsrivastava   (501) staff       (20)        0 2023-06-01 13:57:36.855386 eth-trader-api-proto-0.0.7/
--rw-r--r--   0 atulsrivastava   (501) staff       (20)      114 2023-06-01 13:57:36.855220 eth-trader-api-proto-0.0.7/PKG-INFO
--rw-r--r--   0 atulsrivastava   (501) staff       (20)     1111 2023-06-01 13:57:23.000000 eth-trader-api-proto-0.0.7/README.md
--rw-r--r--   0 atulsrivastava   (501) staff       (20)      357 2023-06-01 13:57:11.000000 eth-trader-api-proto-0.0.7/pyproject.toml
--rw-r--r--   0 atulsrivastava   (501) staff       (20)       38 2023-06-01 13:57:36.855441 eth-trader-api-proto-0.0.7/setup.cfg
-drwxr-xr-x   0 atulsrivastava   (501) staff       (20)        0 2023-06-01 13:57:36.853211 eth-trader-api-proto-0.0.7/src/
-drwxr-xr-x   0 atulsrivastava   (501) staff       (20)        0 2023-06-01 13:57:36.854176 eth-trader-api-proto-0.0.7/src/eth_trader_api/
--rw-r--r--   0 atulsrivastava   (501) staff       (20)       20 2023-06-01 13:56:19.000000 eth-trader-api-proto-0.0.7/src/eth_trader_api/__init__.py
--rw-r--r--   0 atulsrivastava   (501) staff       (20)     5089 2023-06-01 13:56:12.000000 eth-trader-api-proto-0.0.7/src/eth_trader_api/proto.py
-drwxr-xr-x   0 atulsrivastava   (501) staff       (20)        0 2023-06-01 13:57:36.855031 eth-trader-api-proto-0.0.7/src/eth_trader_api_proto.egg-info/
--rw-r--r--   0 atulsrivastava   (501) staff       (20)      114 2023-06-01 13:57:36.000000 eth-trader-api-proto-0.0.7/src/eth_trader_api_proto.egg-info/PKG-INFO
--rw-r--r--   0 atulsrivastava   (501) staff       (20)      322 2023-06-01 13:57:36.000000 eth-trader-api-proto-0.0.7/src/eth_trader_api_proto.egg-info/SOURCES.txt
--rw-r--r--   0 atulsrivastava   (501) staff       (20)        1 2023-06-01 13:57:36.000000 eth-trader-api-proto-0.0.7/src/eth_trader_api_proto.egg-info/dependency_links.txt
--rw-r--r--   0 atulsrivastava   (501) staff       (20)       22 2023-06-01 13:57:36.000000 eth-trader-api-proto-0.0.7/src/eth_trader_api_proto.egg-info/requires.txt
--rw-r--r--   0 atulsrivastava   (501) staff       (20)       15 2023-06-01 13:57:36.000000 eth-trader-api-proto-0.0.7/src/eth_trader_api_proto.egg-info/top_level.txt
+drwxr-xr-x   0 atulsrivastava   (501) staff       (20)        0 2023-06-12 19:51:54.693728 eth-trader-api-proto-0.0.8/
+-rw-r--r--   0 atulsrivastava   (501) staff       (20)      114 2023-06-12 19:51:54.693546 eth-trader-api-proto-0.0.8/PKG-INFO
+-rw-r--r--   0 atulsrivastava   (501) staff       (20)     1111 2023-06-07 22:30:30.000000 eth-trader-api-proto-0.0.8/README.md
+-rw-r--r--   0 atulsrivastava   (501) staff       (20)      357 2023-06-07 22:30:12.000000 eth-trader-api-proto-0.0.8/pyproject.toml
+-rw-r--r--   0 atulsrivastava   (501) staff       (20)       38 2023-06-12 19:51:54.693776 eth-trader-api-proto-0.0.8/setup.cfg
+drwxr-xr-x   0 atulsrivastava   (501) staff       (20)        0 2023-06-12 19:51:54.691436 eth-trader-api-proto-0.0.8/src/
+drwxr-xr-x   0 atulsrivastava   (501) staff       (20)        0 2023-06-12 19:51:54.692512 eth-trader-api-proto-0.0.8/src/eth_trader_api/
+-rw-r--r--   0 atulsrivastava   (501) staff       (20)       20 2023-06-07 23:22:36.000000 eth-trader-api-proto-0.0.8/src/eth_trader_api/__init__.py
+-rw-r--r--   0 atulsrivastava   (501) staff       (20)     5384 2023-06-12 19:37:54.000000 eth-trader-api-proto-0.0.8/src/eth_trader_api/proto.py
+drwxr-xr-x   0 atulsrivastava   (501) staff       (20)        0 2023-06-12 19:51:54.693374 eth-trader-api-proto-0.0.8/src/eth_trader_api_proto.egg-info/
+-rw-r--r--   0 atulsrivastava   (501) staff       (20)      114 2023-06-12 19:51:54.000000 eth-trader-api-proto-0.0.8/src/eth_trader_api_proto.egg-info/PKG-INFO
+-rw-r--r--   0 atulsrivastava   (501) staff       (20)      322 2023-06-12 19:51:54.000000 eth-trader-api-proto-0.0.8/src/eth_trader_api_proto.egg-info/SOURCES.txt
+-rw-r--r--   0 atulsrivastava   (501) staff       (20)        1 2023-06-12 19:51:54.000000 eth-trader-api-proto-0.0.8/src/eth_trader_api_proto.egg-info/dependency_links.txt
+-rw-r--r--   0 atulsrivastava   (501) staff       (20)       22 2023-06-12 19:51:54.000000 eth-trader-api-proto-0.0.8/src/eth_trader_api_proto.egg-info/requires.txt
+-rw-r--r--   0 atulsrivastava   (501) staff       (20)       15 2023-06-12 19:51:54.000000 eth-trader-api-proto-0.0.8/src/eth_trader_api_proto.egg-info/top_level.txt
```

### Comparing `eth-trader-api-proto-0.0.7/README.md` & `eth-trader-api-proto-0.0.8/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -24,15 +24,15 @@
     cd python
     rm -rf dist/ && python3 -m build 
 ```
 
 you can install package locally before uploading it to the pypi
 
 ```shell
-    pip install dist/eth-trader-api-proto-0.0.7.tar.gz
+    pip install dist/eth-trader-api-proto-0.0.8.tar.gz
 ```
 
     (Don't forget to fix the proto compilation issues before releasing)
     To upload this library officially to pypi, use this command
 
 ```shell
     python3 -m twine upload --repository pypi dist/*
```

### Comparing `eth-trader-api-proto-0.0.7/src/eth_trader_api/proto.py` & `eth-trader-api-proto-0.0.8/src/eth_trader_api/proto.py`

 * *Files 10% similar despite different names*

```diff
@@ -16,15 +16,14 @@
 
 
 class OrderType(betterproto.Enum):
     OT_UNKNOWN = 0
     OT_NEW = 1
     OT_CANCEL = 2
 
-
 class SwapType(betterproto.Enum):
     ST_UNKNOWN = 0
     ST_LONG_TERM = 1
     ST_PARTNER_SWAP = 2
 
 
 @dataclass
@@ -40,22 +39,24 @@
 
 @dataclass
 class VirtualPool(betterproto.Message):
     pool_i_d: str = betterproto.string_field(1)
     token0_symbol: str = betterproto.string_field(2)
     token0_address: str = betterproto.string_field(3)
     virtual_token0_reserve: int = betterproto.uint64_field(4)
-    sales_rate_token0: int = betterproto.uint64_field(5)
-    token1_symbol: str = betterproto.string_field(6)
-    token1_address: str = betterproto.string_field(7)
-    virtual_token1_reserve: int = betterproto.uint64_field(8)
-    sales_rate_token1: int = betterproto.uint64_field(9)
-    sales_price: float = betterproto.double_field(10)
-    adjusted_sales_price: float = betterproto.double_field(11)
-    orders: List["VirtualOrder"] = betterproto.message_field(12)
+    sales_price_token0: float = betterproto.double_field(5)
+    sales_price_token0_predicted: float = betterproto.double_field(6)
+    sales_rate_token0: int = betterproto.uint64_field(7)
+    token1_symbol: str = betterproto.string_field(8)
+    token1_address: str = betterproto.string_field(9)
+    virtual_token1_reserve: int = betterproto.uint64_field(10)
+    sales_price_token1: float = betterproto.double_field(11)
+    sales_price_token1_predicted: float = betterproto.double_field(12)
+    sales_rate_token1: int = betterproto.uint64_field(13)
+    orders: List["VirtualOrder"] = betterproto.message_field(14)
 
 
 @dataclass
 class VirtualOrder(betterproto.Message):
     order_i_d: int = betterproto.uint64_field(1)
     sender: str = betterproto.string_field(2)
     token_in: str = betterproto.string_field(3)
@@ -80,18 +81,20 @@
     pool_i_d: str = betterproto.string_field(1)
     token0_symbol: str = betterproto.string_field(2)
     token0_address: str = betterproto.string_field(3)
     virtual_token0_reserve: int = betterproto.uint64_field(4)
     token1_symbol: str = betterproto.string_field(5)
     token1_address: str = betterproto.string_field(6)
     virtual_token1_reserve: int = betterproto.uint64_field(7)
-    sales_rate_token0: int = betterproto.uint64_field(8)
-    sales_rate_token1: int = betterproto.uint64_field(9)
-    sales_price: float = betterproto.float_field(10)
-    adjusted_sales_price: float = betterproto.float_field(11)
+    sales_price_token0: float = betterproto.double_field(8)
+    sales_price_token1: float = betterproto.double_field(9)
+    sales_rate_token0: int = betterproto.uint64_field(10)
+    sales_rate_token1: int = betterproto.uint64_field(11)
+    sales_price_token0_predicted: float = betterproto.double_field(12)
+    sales_price_token1_predicted: float = betterproto.double_field(13)
 
 
 @dataclass
 class OrderStreamRequest(betterproto.Message):
     pool_i_ds: List[str] = betterproto.string_field(1)
```

