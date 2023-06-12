# Comparing `tmp/eveparse-0.0.1.tar.gz` & `tmp/eveparse-1.0.0.tar.gz`

## Comparing `eveparse-0.0.1.tar` & `eveparse-1.0.0.tar`

### file list

```diff
@@ -1,62 +1,69 @@
--rw-r--r--   0        0        0       60 2020-02-02 00:00:00.000000 eveparse-0.0.1/hash.md5
--rw-r--r--   0        0        0       10 2020-02-02 00:00:00.000000 eveparse-0.0.1/requirements.txt
--rw-r--r--   0        0        0        3 2020-02-02 00:00:00.000000 eveparse-0.0.1/.local/.gitignore
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 eveparse-0.0.1/.local/DISTRIBUTE.md
--rw-r--r--   0        0        0     1223 2020-02-02 00:00:00.000000 eveparse-0.0.1/.local/TODO.md
--rw-r--r--   0        0        0      952 2020-02-02 00:00:00.000000 eveparse-0.0.1/.local/app.py
--rw-r--r--   0        0        0   116756 2020-02-02 00:00:00.000000 eveparse-0.0.1/.local/evepraisal.txt
--rw-r--r--   0        0        0      252 2020-02-02 00:00:00.000000 eveparse-0.0.1/.local/pastes/buy_orders.txt
--rw-r--r--   0        0        0      200 2020-02-02 00:00:00.000000 eveparse-0.0.1/.local/pastes/cargo_scanner.txt
--rw-r--r--   0        0        0      183 2020-02-02 00:00:00.000000 eveparse-0.0.1/.local/pastes/drone.txt
--rw-r--r--   0        0        0     6557 2020-02-02 00:00:00.000000 eveparse-0.0.1/.local/pastes/dscan.txt
--rw-r--r--   0        0        0      929 2020-02-02 00:00:00.000000 eveparse-0.0.1/.local/pastes/fitting.txt
--rw-r--r--   0        0        0      897 2020-02-02 00:00:00.000000 eveparse-0.0.1/.local/pastes/market_orders.txt
--rw-r--r--   0        0        0      139 2020-02-02 00:00:00.000000 eveparse-0.0.1/.local/pastes/multibuy.txt
--rw-r--r--   0        0        0      479 2020-02-02 00:00:00.000000 eveparse-0.0.1/.local/pastes/orders_history.txt
--rw-r--r--   0        0        0       53 2020-02-02 00:00:00.000000 eveparse-0.0.1/.local/pastes/quickbar.txt
--rw-r--r--   0        0        0      219 2020-02-02 00:00:00.000000 eveparse-0.0.1/.local/pastes/sell_orders.txt
--rw-r--r--   0        0        0     3586 2020-02-02 00:00:00.000000 eveparse-0.0.1/.local/pastes/survey_scan.txt
--rw-r--r--   0        0        0     1202 2020-02-02 00:00:00.000000 eveparse-0.0.1/.local/pastes/view_contents.txt
--rw-r--r--   0        0        0     2238 2020-02-02 00:00:00.000000 eveparse-0.0.1/eveparse/__init__.py
--rw-r--r--   0        0        0      263 2020-02-02 00:00:00.000000 eveparse-0.0.1/eveparse/constants.py
--rw-r--r--   0        0        0      732 2020-02-02 00:00:00.000000 eveparse-0.0.1/eveparse/converters.py
--rw-r--r--   0        0        0      149 2020-02-02 00:00:00.000000 eveparse-0.0.1/eveparse/errors.py
--rw-r--r--   0        0        0     1129 2020-02-02 00:00:00.000000 eveparse-0.0.1/eveparse/validators.py
--rw-r--r--   0        0        0  2294022 2020-02-02 00:00:00.000000 eveparse-0.0.1/eveparse/data/invTypes.json
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 eveparse-0.0.1/eveparse/parsers/__init__.py
--rw-r--r--   0        0        0      612 2020-02-02 00:00:00.000000 eveparse-0.0.1/eveparse/parsers/base.py
--rw-r--r--   0        0        0      721 2020-02-02 00:00:00.000000 eveparse-0.0.1/eveparse/parsers/contract.py
--rw-r--r--   0        0        0      730 2020-02-02 00:00:00.000000 eveparse-0.0.1/eveparse/parsers/contractnodetails.py
--rw-r--r--   0        0        0      215 2020-02-02 00:00:00.000000 eveparse-0.0.1/eveparse/parsers/nameonly.py
--rw-r--r--   0        0        0      705 2020-02-02 00:00:00.000000 eveparse-0.0.1/eveparse/parsers/namespacequantity.py
--rw-r--r--   0        0        0      712 2020-02-02 00:00:00.000000 eveparse-0.0.1/eveparse/parsers/namespacexquantity.py
--rw-r--r--   0        0        0      680 2020-02-02 00:00:00.000000 eveparse-0.0.1/eveparse/parsers/nametabquantity.py
--rw-r--r--   0        0        0      703 2020-02-02 00:00:00.000000 eveparse-0.0.1/eveparse/parsers/quantityspacename.py
--rw-r--r--   0        0        0      725 2020-02-02 00:00:00.000000 eveparse-0.0.1/eveparse/parsers/quantityspacexspacename.py
--rw-r--r--   0        0        0      710 2020-02-02 00:00:00.000000 eveparse-0.0.1/eveparse/parsers/quantityxspacename.py
--rw-r--r--   0        0        0      674 2020-02-02 00:00:00.000000 eveparse-0.0.1/eveparse/parsers/shipfitname.py
--rwxr-xr-x   0        0        0      348 2020-02-02 00:00:00.000000 eveparse-0.0.1/scripts/build.bat
--rwxr-xr-x   0        0        0      342 2020-02-02 00:00:00.000000 eveparse-0.0.1/scripts/dist.bat
--rw-r--r--   0        0        0     2761 2020-02-02 00:00:00.000000 eveparse-0.0.1/scripts/sde.py
--rwxr-xr-x   0        0        0      244 2020-02-02 00:00:00.000000 eveparse-0.0.1/scripts/test.bat
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 eveparse-0.0.1/tests/__init__.py
--rw-r--r--   0        0        0      801 2020-02-02 00:00:00.000000 eveparse-0.0.1/tests/test_converters.py
--rw-r--r--   0        0        0     1636 2020-02-02 00:00:00.000000 eveparse-0.0.1/tests/test_parse.py
--rw-r--r--   0        0        0     1088 2020-02-02 00:00:00.000000 eveparse-0.0.1/tests/test_validators.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 eveparse-0.0.1/tests/test_parsers/__init__.py
--rw-r--r--   0        0        0      652 2020-02-02 00:00:00.000000 eveparse-0.0.1/tests/test_parsers/test_base.py
--rw-r--r--   0        0        0      636 2020-02-02 00:00:00.000000 eveparse-0.0.1/tests/test_parsers/test_contract.py
--rw-r--r--   0        0        0      685 2020-02-02 00:00:00.000000 eveparse-0.0.1/tests/test_parsers/test_contractnodetails.py
--rw-r--r--   0        0        0      354 2020-02-02 00:00:00.000000 eveparse-0.0.1/tests/test_parsers/test_nameonly.py
--rw-r--r--   0        0        0      541 2020-02-02 00:00:00.000000 eveparse-0.0.1/tests/test_parsers/test_namespacequantity.py
--rw-r--r--   0        0        0      548 2020-02-02 00:00:00.000000 eveparse-0.0.1/tests/test_parsers/test_namespacexquantity.py
--rw-r--r--   0        0        0      529 2020-02-02 00:00:00.000000 eveparse-0.0.1/tests/test_parsers/test_nametabquantity.py
--rw-r--r--   0        0        0      541 2020-02-02 00:00:00.000000 eveparse-0.0.1/tests/test_parsers/test_quantityspacename.py
--rw-r--r--   0        0        0      598 2020-02-02 00:00:00.000000 eveparse-0.0.1/tests/test_parsers/test_quantityspacexspacename.py
--rw-r--r--   0        0        0      707 2020-02-02 00:00:00.000000 eveparse-0.0.1/tests/test_parsers/test_quantityxspacename.py
--rw-r--r--   0        0        0      837 2020-02-02 00:00:00.000000 eveparse-0.0.1/tests/test_parsers/test_shipfitname.py
--rw-r--r--   0        0        0       37 2020-02-02 00:00:00.000000 eveparse-0.0.1/.gitignore
--rw-r--r--   0        0        0     1065 2020-02-02 00:00:00.000000 eveparse-0.0.1/LICENSE
--rw-r--r--   0        0        0      550 2020-02-02 00:00:00.000000 eveparse-0.0.1/README.md
--rw-r--r--   0        0        0      684 2020-02-02 00:00:00.000000 eveparse-0.0.1/pyproject.toml
--rw-r--r--   0        0        0     2214 2020-02-02 00:00:00.000000 eveparse-0.0.1/PKG-INFO
+-rw-r--r--   0        0        0      439 2020-02-02 00:00:00.000000 eveparse-1.0.0/.editorconfig
+-rw-r--r--   0        0        0      153 2020-02-02 00:00:00.000000 eveparse-1.0.0/.flake8
+-rw-r--r--   0        0        0      781 2020-02-02 00:00:00.000000 eveparse-1.0.0/CHANGELOG.md
+-rw-r--r--   0        0        0       60 2020-02-02 00:00:00.000000 eveparse-1.0.0/hash.md5
+-rw-r--r--   0        0        0       32 2020-02-02 00:00:00.000000 eveparse-1.0.0/requirements.txt
+-rw-r--r--   0        0        0     1121 2020-02-02 00:00:00.000000 eveparse-1.0.0/.github/workflows/ci.yaml
+-rw-r--r--   0        0        0        3 2020-02-02 00:00:00.000000 eveparse-1.0.0/.local/.gitignore
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 eveparse-1.0.0/.local/DISTRIBUTE.md
+-rw-r--r--   0        0        0     1223 2020-02-02 00:00:00.000000 eveparse-1.0.0/.local/TODO.md
+-rw-r--r--   0        0        0      952 2020-02-02 00:00:00.000000 eveparse-1.0.0/.local/app.py
+-rw-r--r--   0        0        0   116756 2020-02-02 00:00:00.000000 eveparse-1.0.0/.local/evepraisal.txt
+-rw-r--r--   0        0        0      252 2020-02-02 00:00:00.000000 eveparse-1.0.0/.local/pastes/buy_orders.txt
+-rw-r--r--   0        0        0      200 2020-02-02 00:00:00.000000 eveparse-1.0.0/.local/pastes/cargo_scanner.txt
+-rw-r--r--   0        0        0      183 2020-02-02 00:00:00.000000 eveparse-1.0.0/.local/pastes/drone.txt
+-rw-r--r--   0        0        0     6557 2020-02-02 00:00:00.000000 eveparse-1.0.0/.local/pastes/dscan.txt
+-rw-r--r--   0        0        0      929 2020-02-02 00:00:00.000000 eveparse-1.0.0/.local/pastes/fitting.txt
+-rw-r--r--   0        0        0      897 2020-02-02 00:00:00.000000 eveparse-1.0.0/.local/pastes/market_orders.txt
+-rw-r--r--   0        0        0      139 2020-02-02 00:00:00.000000 eveparse-1.0.0/.local/pastes/multibuy.txt
+-rw-r--r--   0        0        0      479 2020-02-02 00:00:00.000000 eveparse-1.0.0/.local/pastes/orders_history.txt
+-rw-r--r--   0        0        0       53 2020-02-02 00:00:00.000000 eveparse-1.0.0/.local/pastes/quickbar.txt
+-rw-r--r--   0        0        0      219 2020-02-02 00:00:00.000000 eveparse-1.0.0/.local/pastes/sell_orders.txt
+-rw-r--r--   0        0        0     3586 2020-02-02 00:00:00.000000 eveparse-1.0.0/.local/pastes/survey_scan.txt
+-rw-r--r--   0        0        0     1202 2020-02-02 00:00:00.000000 eveparse-1.0.0/.local/pastes/view_contents.txt
+-rw-r--r--   0        0        0     2295 2020-02-02 00:00:00.000000 eveparse-1.0.0/eveparse/__init__.py
+-rw-r--r--   0        0        0      263 2020-02-02 00:00:00.000000 eveparse-1.0.0/eveparse/constants.py
+-rw-r--r--   0        0        0      732 2020-02-02 00:00:00.000000 eveparse-1.0.0/eveparse/converters.py
+-rw-r--r--   0        0        0      149 2020-02-02 00:00:00.000000 eveparse-1.0.0/eveparse/errors.py
+-rw-r--r--   0        0        0     1129 2020-02-02 00:00:00.000000 eveparse-1.0.0/eveparse/validators.py
+-rw-r--r--   0        0        0  2294022 2020-02-02 00:00:00.000000 eveparse-1.0.0/eveparse/data/invTypes.json
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 eveparse-1.0.0/eveparse/parsers/__init__.py
+-rw-r--r--   0        0        0      612 2020-02-02 00:00:00.000000 eveparse-1.0.0/eveparse/parsers/base.py
+-rw-r--r--   0        0        0      721 2020-02-02 00:00:00.000000 eveparse-1.0.0/eveparse/parsers/contract.py
+-rw-r--r--   0        0        0      743 2020-02-02 00:00:00.000000 eveparse-1.0.0/eveparse/parsers/contractnodetails.py
+-rw-r--r--   0        0        0      215 2020-02-02 00:00:00.000000 eveparse-1.0.0/eveparse/parsers/nameonly.py
+-rw-r--r--   0        0        0      705 2020-02-02 00:00:00.000000 eveparse-1.0.0/eveparse/parsers/namespacequantity.py
+-rw-r--r--   0        0        0      712 2020-02-02 00:00:00.000000 eveparse-1.0.0/eveparse/parsers/namespacexquantity.py
+-rw-r--r--   0        0        0      680 2020-02-02 00:00:00.000000 eveparse-1.0.0/eveparse/parsers/nametabquantity.py
+-rw-r--r--   0        0        0      703 2020-02-02 00:00:00.000000 eveparse-1.0.0/eveparse/parsers/quantityspacename.py
+-rw-r--r--   0        0        0      725 2020-02-02 00:00:00.000000 eveparse-1.0.0/eveparse/parsers/quantityspacexspacename.py
+-rw-r--r--   0        0        0      710 2020-02-02 00:00:00.000000 eveparse-1.0.0/eveparse/parsers/quantityxspacename.py
+-rw-r--r--   0        0        0      674 2020-02-02 00:00:00.000000 eveparse-1.0.0/eveparse/parsers/shipfitname.py
+-rw-r--r--   0        0        0      721 2020-02-02 00:00:00.000000 eveparse-1.0.0/eveparse/parsers/viewcontents.py
+-rwxr-xr-x   0        0        0      348 2020-02-02 00:00:00.000000 eveparse-1.0.0/scripts/build.bat
+-rwxr-xr-x   0        0        0      423 2020-02-02 00:00:00.000000 eveparse-1.0.0/scripts/dist.bat
+-rwxr-xr-x   0        0        0      241 2020-02-02 00:00:00.000000 eveparse-1.0.0/scripts/lint.bat
+-rw-r--r--   0        0        0     2559 2020-02-02 00:00:00.000000 eveparse-1.0.0/scripts/sde.py
+-rwxr-xr-x   0        0        0      244 2020-02-02 00:00:00.000000 eveparse-1.0.0/scripts/test.bat
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 eveparse-1.0.0/tests/__init__.py
+-rw-r--r--   0        0        0      801 2020-02-02 00:00:00.000000 eveparse-1.0.0/tests/test_converters.py
+-rw-r--r--   0        0        0     1799 2020-02-02 00:00:00.000000 eveparse-1.0.0/tests/test_parse.py
+-rw-r--r--   0        0        0     1088 2020-02-02 00:00:00.000000 eveparse-1.0.0/tests/test_validators.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 eveparse-1.0.0/tests/test_parsers/__init__.py
+-rw-r--r--   0        0        0      652 2020-02-02 00:00:00.000000 eveparse-1.0.0/tests/test_parsers/test_base.py
+-rw-r--r--   0        0        0      636 2020-02-02 00:00:00.000000 eveparse-1.0.0/tests/test_parsers/test_contract.py
+-rw-r--r--   0        0        0      685 2020-02-02 00:00:00.000000 eveparse-1.0.0/tests/test_parsers/test_contractnodetails.py
+-rw-r--r--   0        0        0      354 2020-02-02 00:00:00.000000 eveparse-1.0.0/tests/test_parsers/test_nameonly.py
+-rw-r--r--   0        0        0      541 2020-02-02 00:00:00.000000 eveparse-1.0.0/tests/test_parsers/test_namespacequantity.py
+-rw-r--r--   0        0        0      548 2020-02-02 00:00:00.000000 eveparse-1.0.0/tests/test_parsers/test_namespacexquantity.py
+-rw-r--r--   0        0        0      529 2020-02-02 00:00:00.000000 eveparse-1.0.0/tests/test_parsers/test_nametabquantity.py
+-rw-r--r--   0        0        0      541 2020-02-02 00:00:00.000000 eveparse-1.0.0/tests/test_parsers/test_quantityspacename.py
+-rw-r--r--   0        0        0      598 2020-02-02 00:00:00.000000 eveparse-1.0.0/tests/test_parsers/test_quantityspacexspacename.py
+-rw-r--r--   0        0        0      707 2020-02-02 00:00:00.000000 eveparse-1.0.0/tests/test_parsers/test_quantityxspacename.py
+-rw-r--r--   0        0        0      837 2020-02-02 00:00:00.000000 eveparse-1.0.0/tests/test_parsers/test_shipfitname.py
+-rw-r--r--   0        0        0      638 2020-02-02 00:00:00.000000 eveparse-1.0.0/tests/test_parsers/test_viewcontents.py
+-rw-r--r--   0        0        0       37 2020-02-02 00:00:00.000000 eveparse-1.0.0/.gitignore
+-rw-r--r--   0        0        0     1065 2020-02-02 00:00:00.000000 eveparse-1.0.0/LICENSE
+-rw-r--r--   0        0        0      550 2020-02-02 00:00:00.000000 eveparse-1.0.0/README.md
+-rw-r--r--   0        0        0      684 2020-02-02 00:00:00.000000 eveparse-1.0.0/pyproject.toml
+-rw-r--r--   0        0        0     2214 2020-02-02 00:00:00.000000 eveparse-1.0.0/PKG-INFO
```

### Comparing `eveparse-0.0.1/.local/TODO.md` & `eveparse-1.0.0/.local/TODO.md`

 * *Files identical despite different names*

### Comparing `eveparse-0.0.1/.local/app.py` & `eveparse-1.0.0/.local/app.py`

 * *Files identical despite different names*

### Comparing `eveparse-0.0.1/.local/evepraisal.txt` & `eveparse-1.0.0/.local/evepraisal.txt`

 * *Files identical despite different names*

### Comparing `eveparse-0.0.1/.local/pastes/dscan.txt` & `eveparse-1.0.0/.local/pastes/dscan.txt`

 * *Files identical despite different names*

### Comparing `eveparse-0.0.1/.local/pastes/fitting.txt` & `eveparse-1.0.0/.local/pastes/fitting.txt`

 * *Files identical despite different names*

### Comparing `eveparse-0.0.1/.local/pastes/market_orders.txt` & `eveparse-1.0.0/.local/pastes/market_orders.txt`

 * *Files identical despite different names*

### Comparing `eveparse-0.0.1/.local/pastes/survey_scan.txt` & `eveparse-1.0.0/.local/pastes/survey_scan.txt`

 * *Files identical despite different names*

### Comparing `eveparse-0.0.1/.local/pastes/view_contents.txt` & `eveparse-1.0.0/.local/pastes/view_contents.txt`

 * *Files identical despite different names*

### Comparing `eveparse-0.0.1/eveparse/__init__.py` & `eveparse-1.0.0/eveparse/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,36 +1,37 @@
 import functools
 
 from .constants import TYPES
 from .converters import normalize_string
 from .errors import ConverterError, ParserError, ValidatorError
-from .validators import is_int, is_legal_string, is_valid_name
-
 from .parsers.contract import Contract
 from .parsers.contractnodetails import ContractNoDetails
 from .parsers.nameonly import NameOnly
 from .parsers.namespacequantity import NameSpaceQuantity
 from .parsers.namespacexquantity import NameSpaceXQuantity
 from .parsers.nametabquantity import NameTabQuantity
 from .parsers.quantityspacename import QuantitySpaceName
 from .parsers.quantityspacexspacename import QuantitySpaceXSpaceName
 from .parsers.quantityxspacename import QuantityXSpaceName
 from .parsers.shipfitname import ShipFitName
+from .parsers.viewcontents import ViewContents
+from .validators import is_legal_string, is_valid_name
 
 PARSERS = [
     NameOnly,
     Contract,
     ContractNoDetails,
     NameSpaceQuantity,
     NameSpaceXQuantity,
     NameTabQuantity,
     QuantitySpaceName,
     QuantitySpaceXSpaceName,
     QuantityXSpaceName,
     ShipFitName,
+    ViewContents,
 ]
 
 
 @functools.cache
 def parse(string: str) -> tuple[int, str, int]:
     """Attempt to extract a valid item name and quantity from a string.
     Tries all parsers and returns first non-failing parser.
```

### Comparing `eveparse-0.0.1/eveparse/converters.py` & `eveparse-1.0.0/eveparse/converters.py`

 * *Files identical despite different names*

### Comparing `eveparse-0.0.1/eveparse/validators.py` & `eveparse-1.0.0/eveparse/validators.py`

 * *Files 2% similar despite different names*

```diff
@@ -30,10 +30,11 @@
 
 def is_legal_string(string: str) -> bool:
     if string in ILLEGAL_STRINGS:
         return False
     return True
 
 
-@functools.lru_cache(maxsize=25000)  # slightly more than number of currently published invTypes at 23623
+# slightly more than number of currently published invTypes at 23623
+@functools.lru_cache(maxsize=25000)
 def is_valid_name(string: str) -> bool:
     return string in TYPE_NAMES
```

### Comparing `eveparse-0.0.1/eveparse/data/invTypes.json` & `eveparse-1.0.0/eveparse/data/invTypes.json`

 * *Files identical despite different names*

### Comparing `eveparse-0.0.1/eveparse/parsers/base.py` & `eveparse-1.0.0/eveparse/parsers/base.py`

 * *Files identical despite different names*

### Comparing `eveparse-0.0.1/eveparse/parsers/contract.py` & `eveparse-1.0.0/eveparse/parsers/contract.py`

 * *Files identical despite different names*

### Comparing `eveparse-0.0.1/eveparse/parsers/contractnodetails.py` & `eveparse-1.0.0/eveparse/parsers/contractnodetails.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 from eveparse.converters import to_int
 from eveparse.errors import ParserError
 from eveparse.parsers.base import TabbedParser
 from eveparse.validators import is_int
 
 
 class ContractNoDetails(TabbedParser):
-    """Cybernetic Subprocessor - Basic	1	Cyber Learning	Implant	"""
+    """Cybernetic Subprocessor - Basic	1	Cyber Learning	Implant	"""  # fmt: skip
 
     @classmethod
     def parse(cls, string: str) -> tuple[str, int]:
         super().parse(string)
         if string.count("\t") != 3:
             raise ParserError("Not 3 tabs")
         parts = string.split("\t")
```

### Comparing `eveparse-0.0.1/eveparse/parsers/namespacequantity.py` & `eveparse-1.0.0/eveparse/parsers/namespacequantity.py`

 * *Ordering differences only*

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
-from eveparse.parsers.base import UnTabbedParser
 from eveparse.converters import to_int
 from eveparse.errors import ParserError
+from eveparse.parsers.base import UnTabbedParser
 from eveparse.validators import is_int
 
 
 class NameSpaceQuantity(UnTabbedParser):
     """Ragnarok 2"""
 
     @classmethod
```

### Comparing `eveparse-0.0.1/eveparse/parsers/namespacexquantity.py` & `eveparse-1.0.0/eveparse/parsers/namespacexquantity.py`

 * *Ordering differences only*

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
-from eveparse.parsers.base import UnTabbedParser
 from eveparse.converters import to_int
 from eveparse.errors import ParserError
+from eveparse.parsers.base import UnTabbedParser
 from eveparse.validators import is_int
 
 
 class NameSpaceXQuantity(UnTabbedParser):
     """Ragnarok x2"""
 
     @classmethod
```

### Comparing `eveparse-0.0.1/eveparse/parsers/nametabquantity.py` & `eveparse-1.0.0/eveparse/parsers/nametabquantity.py`

 * *Ordering differences only*

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
-from eveparse.parsers.base import TabbedParser
 from eveparse.converters import to_int
 from eveparse.errors import ParserError
+from eveparse.parsers.base import TabbedParser
 from eveparse.validators import is_int
 
 
 class NameTabQuantity(TabbedParser):
     """Ragnarok	2"""
 
     @classmethod
```

### Comparing `eveparse-0.0.1/eveparse/parsers/quantityspacename.py` & `eveparse-1.0.0/eveparse/parsers/quantityspacename.py`

 * *Ordering differences only*

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
-from eveparse.parsers.base import UnTabbedParser
 from eveparse.converters import to_int
 from eveparse.errors import ParserError
+from eveparse.parsers.base import UnTabbedParser
 from eveparse.validators import is_int
 
 
 class QuantitySpaceName(UnTabbedParser):
     """1 Ragnarok"""
 
     @classmethod
```

### Comparing `eveparse-0.0.1/eveparse/parsers/quantityspacexspacename.py` & `eveparse-1.0.0/eveparse/parsers/quantityspacexspacename.py`

 * *Ordering differences only*

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
-from eveparse.parsers.base import UnTabbedParser
 from eveparse.converters import to_int
 from eveparse.errors import ParserError
+from eveparse.parsers.base import UnTabbedParser
 from eveparse.validators import is_int
 
 
 class QuantitySpaceXSpaceName(UnTabbedParser):
     """1 x Ragnarok"""
 
     @classmethod
```

### Comparing `eveparse-0.0.1/eveparse/parsers/quantityxspacename.py` & `eveparse-1.0.0/eveparse/parsers/quantityxspacename.py`

 * *Ordering differences only*

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
-from eveparse.parsers.base import UnTabbedParser
 from eveparse.converters import to_int
 from eveparse.errors import ParserError
+from eveparse.parsers.base import UnTabbedParser
 from eveparse.validators import is_int
 
 
 class QuantityXSpaceName(UnTabbedParser):
     """1x Ragnarok"""
 
     @classmethod
```

### Comparing `eveparse-0.0.1/eveparse/parsers/shipfitname.py` & `eveparse-1.0.0/eveparse/parsers/shipfitname.py`

 * *Ordering differences only*

 * *Files 14% similar despite different names*

```diff
@@ -1,9 +1,9 @@
-from eveparse.parsers.base import UnTabbedParser
 from eveparse.errors import ParserError
+from eveparse.parsers.base import UnTabbedParser
 
 
 class ShipFitName(UnTabbedParser):
     """[Ragnarok, Bob's Ragnarok]"""
 
     @classmethod
     def parse(cls, string: str) -> tuple[str, int]:
```

### Comparing `eveparse-0.0.1/scripts/sde.py` & `eveparse-1.0.0/scripts/sde.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,25 +1,25 @@
 import csv
+import io
 import json
 import os
 import pathlib
 import requests
 import sys
 
 MD5_HASH_FILE_PATH: str = str(pathlib.Path(__file__).parent.parent / "hash.md5")
-INV_TYPES_CSV_FILE_PATH: str = str(pathlib.Path(__file__).parent.parent / "eveparse/data/invTypes.csv")
 INV_TYPES_JSON_FILE_PATH: str = str(pathlib.Path(__file__).parent.parent / "eveparse/data/invTypes.json")
 
 MD5_HASH_URL: str = "https://www.fuzzwork.co.uk/dump/sqlite-latest.sqlite.bz2.md5"
 INV_TYPES_CSV_URL: str = "https://www.fuzzwork.co.uk/dump/latest/invTypes-nodescription.csv"
 
 
-def convert_csv_to_dict(csv_file_path: str) -> dict:
+def convert_csv_to_dict(csv_file_content: str) -> dict:
     inv_types = {}
-    with open(csv_file_path, "r", encoding="utf-8") as csv_file:
+    with io.StringIO(csv_file_content) as csv_file:
         csv_content = csv.reader(csv_file)
         for row in csv_content:
             # CSV column names are:
             # type_id, group_id, name, mass, volume, capacity, portion_size, race_id,
             # base_price, published, market_group_id, icon_id, sound_id, graphic_id
 
             type_id = row[0]
@@ -69,20 +69,18 @@
     latest_md5_hash_string = request_url_text(MD5_HASH_URL)
     current_md5_hash_string = read_file_text(MD5_HASH_FILE_PATH)
     if latest_md5_hash_string == current_md5_hash_string:
         sys.exit(0)
 
     # Download updated SDE
     csv_file = request_url_text(INV_TYPES_CSV_URL)
-    write_file_text(INV_TYPES_CSV_FILE_PATH, csv_file)
 
-    # Convert CSV SDE to JSON
-    inv_types = convert_csv_to_dict(INV_TYPES_CSV_FILE_PATH)
+    # Convert CSV SDE to JSON and write to file
+    inv_types = convert_csv_to_dict(csv_file)
     write_file_json(INV_TYPES_JSON_FILE_PATH, inv_types)
 
-    # Clean up files
-    delete_file(INV_TYPES_CSV_FILE_PATH)
+    # Update hash
     write_file_text(MD5_HASH_FILE_PATH, latest_md5_hash_string)
 
 
 if __name__ == '__main__':
     main()
```

### Comparing `eveparse-0.0.1/tests/test_converters.py` & `eveparse-1.0.0/tests/test_converters.py`

 * *Files identical despite different names*

### Comparing `eveparse-0.0.1/tests/test_parse.py` & `eveparse-1.0.0/tests/test_parse.py`

 * *Files 4% similar despite different names*

```diff
@@ -35,7 +35,10 @@
         self.assertEqual(parse("4 x Ragnarok"), (23773, "Ragnarok", 4))
 
     def test_quantityxspacename(self):
         self.assertEqual(parse("3x Ragnarok"), (23773, "Ragnarok", 3))
 
     def test_shipfitname(self):
         self.assertEqual(parse("[Ragnarok, Bob's Ragnarok]"), (23773, "Ragnarok", 1))
+
+    def test_viewcontents(self):
+        self.assertEqual(parse("Burned Logic Circuit	Salvaged Materials	Cargo Hold	26"), (25600, "Burned Logic Circuit", 26))
```

### Comparing `eveparse-0.0.1/tests/test_validators.py` & `eveparse-1.0.0/tests/test_validators.py`

 * *Files identical despite different names*

### Comparing `eveparse-0.0.1/tests/test_parsers/test_base.py` & `eveparse-1.0.0/tests/test_parsers/test_base.py`

 * *Files identical despite different names*

### Comparing `eveparse-0.0.1/tests/test_parsers/test_contract.py` & `eveparse-1.0.0/tests/test_parsers/test_contract.py`

 * *Files identical despite different names*

### Comparing `eveparse-0.0.1/tests/test_parsers/test_contractnodetails.py` & `eveparse-1.0.0/tests/test_parsers/test_contractnodetails.py`

 * *Files identical despite different names*

### Comparing `eveparse-0.0.1/tests/test_parsers/test_namespacequantity.py` & `eveparse-1.0.0/tests/test_parsers/test_namespacequantity.py`

 * *Files identical despite different names*

### Comparing `eveparse-0.0.1/tests/test_parsers/test_namespacexquantity.py` & `eveparse-1.0.0/tests/test_parsers/test_namespacexquantity.py`

 * *Files identical despite different names*

### Comparing `eveparse-0.0.1/tests/test_parsers/test_nametabquantity.py` & `eveparse-1.0.0/tests/test_parsers/test_nametabquantity.py`

 * *Files identical despite different names*

### Comparing `eveparse-0.0.1/tests/test_parsers/test_quantityspacename.py` & `eveparse-1.0.0/tests/test_parsers/test_quantityspacename.py`

 * *Files identical despite different names*

### Comparing `eveparse-0.0.1/tests/test_parsers/test_quantityspacexspacename.py` & `eveparse-1.0.0/tests/test_parsers/test_quantityspacexspacename.py`

 * *Files identical despite different names*

### Comparing `eveparse-0.0.1/tests/test_parsers/test_quantityxspacename.py` & `eveparse-1.0.0/tests/test_parsers/test_quantityxspacename.py`

 * *Files identical despite different names*

### Comparing `eveparse-0.0.1/tests/test_parsers/test_shipfitname.py` & `eveparse-1.0.0/tests/test_parsers/test_shipfitname.py`

 * *Files identical despite different names*

### Comparing `eveparse-0.0.1/LICENSE` & `eveparse-1.0.0/LICENSE`

 * *Files identical despite different names*

### Comparing `eveparse-0.0.1/README.md` & `eveparse-1.0.0/README.md`

 * *Files identical despite different names*

### Comparing `eveparse-0.0.1/pyproject.toml` & `eveparse-1.0.0/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,21 +1,21 @@
 [build-system]
 requires = ["hatchling"]
 build-backend = "hatchling.build"
 
 [project]
 name = "eveparse"
-version = "0.0.1"
+version = "1.0.0"
 authors = [
   {name="Chris Harrel", email="24297899+harrelchris@users.noreply.github.com"},
 ]
 description = "Parser for Eve Online - extract item name and quantity from a string"
 readme = "README.md"
 license = {file = "LICENSE"}
-requires-python = ">=3.7"
+requires-python = ">=3.9"
 classifiers = [
     "Programming Language :: Python :: 3",
     "License :: OSI Approved :: MIT License",
     "Operating System :: OS Independent",
 ]
 
 [project.urls]
```

### Comparing `eveparse-0.0.1/PKG-INFO` & `eveparse-1.0.0/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: eveparse
-Version: 0.0.1
+Version: 1.0.0
 Summary: Parser for Eve Online - extract item name and quantity from a string
 Project-URL: Homepage, https://github.com/harrelchris/eveparse
 Project-URL: Bug Tracker, https://github.com/harrelchris/eveparse/issues
 Author-email: Chris Harrel <24297899+harrelchris@users.noreply.github.com>
 License: Copyright 2023 Chris Harrel
         
         Permission is hereby granted, free of charge, to any person obtaining a copy of this software and associated documentation files (the “Software”), to deal in the Software without restriction, including without limitation the rights to use, copy, modify, merge, publish, distribute, sublicense, and/or sell copies of the Software, and to permit persons to whom the Software is furnished to do so, subject to the following conditions:
@@ -12,15 +12,15 @@
         The above copyright notice and this permission notice shall be included in all copies or substantial portions of the Software.
         
         THE SOFTWARE IS PROVIDED “AS IS”, WITHOUT WARRANTY OF ANY KIND, EXPRESS OR IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY, FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM, OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE SOFTWARE.
 License-File: LICENSE
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3
-Requires-Python: >=3.7
+Requires-Python: >=3.9
 Description-Content-Type: text/markdown
 
 # Eve Parse
 
 Parser for Eve Online - extract item name and quantity from a string, and return values with type_id
 
 ## Install
```

