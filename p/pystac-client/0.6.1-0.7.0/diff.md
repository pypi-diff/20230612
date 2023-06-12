# Comparing `tmp/pystac-client-0.6.1.tar.gz` & `tmp/pystac-client-0.7.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pystac-client-0.6.1.tar", last modified: Tue Mar 14 12:41:32 2023, max compression
+gzip compressed data, was "pystac-client-0.7.0.tar", last modified: Mon Jun 12 21:16:01 2023, max compression
```

## Comparing `pystac-client-0.6.1.tar` & `pystac-client-0.7.0.tar`

### file list

```diff
@@ -1,28 +1,35 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-14 12:41:32.122802 pystac-client-0.6.1/
--rw-r--r--   0 runner    (1001) docker     (123)      553 2023-03-14 12:41:19.000000 pystac-client-0.6.1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)       23 2023-03-14 12:41:19.000000 pystac-client-0.6.1/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     7785 2023-03-14 12:41:32.122802 pystac-client-0.6.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     6598 2023-03-14 12:41:19.000000 pystac-client-0.6.1/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-14 12:41:32.122802 pystac-client-0.6.1/pystac_client/
--rw-r--r--   0 runner    (1001) docker     (123)      384 2023-03-14 12:41:19.000000 pystac-client-0.6.1/pystac_client/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      806 2023-03-14 12:41:19.000000 pystac-client-0.6.1/pystac_client/_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     8032 2023-03-14 12:41:19.000000 pystac-client-0.6.1/pystac_client/cli.py
--rw-r--r--   0 runner    (1001) docker     (123)    21927 2023-03-14 12:41:19.000000 pystac-client-0.6.1/pystac_client/client.py
--rw-r--r--   0 runner    (1001) docker     (123)     6396 2023-03-14 12:41:19.000000 pystac-client-0.6.1/pystac_client/collection_client.py
--rw-r--r--   0 runner    (1001) docker     (123)     1024 2023-03-14 12:41:19.000000 pystac-client-0.6.1/pystac_client/conformance.py
--rw-r--r--   0 runner    (1001) docker     (123)      246 2023-03-14 12:41:19.000000 pystac-client-0.6.1/pystac_client/errors.py
--rw-r--r--   0 runner    (1001) docker     (123)      449 2023-03-14 12:41:19.000000 pystac-client-0.6.1/pystac_client/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (123)    32144 2023-03-14 12:41:19.000000 pystac-client-0.6.1/pystac_client/item_search.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-03-14 12:41:19.000000 pystac-client-0.6.1/pystac_client/py.typed
--rw-r--r--   0 runner    (1001) docker     (123)    12756 2023-03-14 12:41:19.000000 pystac-client-0.6.1/pystac_client/stac_api_io.py
--rw-r--r--   0 runner    (1001) docker     (123)       22 2023-03-14 12:41:19.000000 pystac-client-0.6.1/pystac_client/version.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-14 12:41:32.122802 pystac-client-0.6.1/pystac_client.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     7785 2023-03-14 12:41:32.000000 pystac-client-0.6.1/pystac_client.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      625 2023-03-14 12:41:32.000000 pystac-client-0.6.1/pystac_client.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-03-14 12:41:32.000000 pystac-client-0.6.1/pystac_client.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       54 2023-03-14 12:41:32.000000 pystac-client-0.6.1/pystac_client.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-03-14 12:41:32.000000 pystac-client-0.6.1/pystac_client.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)       86 2023-03-14 12:41:32.000000 pystac-client-0.6.1/pystac_client.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)      121 2023-03-14 12:41:32.000000 pystac-client-0.6.1/pystac_client.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)      581 2023-03-14 12:41:32.126802 pystac-client-0.6.1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     2158 2023-03-14 12:41:19.000000 pystac-client-0.6.1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-12 21:16:01.587874 pystac-client-0.7.0/
+-rw-r--r--   0 runner    (1001) docker     (123)      553 2023-06-12 21:15:37.000000 pystac-client-0.7.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)       23 2023-06-12 21:15:37.000000 pystac-client-0.7.0/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     3175 2023-06-12 21:16:01.587874 pystac-client-0.7.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1592 2023-06-12 21:15:37.000000 pystac-client-0.7.0/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)     3483 2023-06-12 21:15:37.000000 pystac-client-0.7.0/pyproject.toml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-12 21:16:01.587874 pystac-client-0.7.0/pystac_client/
+-rw-r--r--   0 runner    (1001) docker     (123)      431 2023-06-12 21:15:37.000000 pystac-client-0.7.0/pystac_client/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      806 2023-06-12 21:15:37.000000 pystac-client-0.7.0/pystac_client/_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11237 2023-06-12 21:15:37.000000 pystac-client-0.7.0/pystac_client/cli.py
+-rw-r--r--   0 runner    (1001) docker     (123)    26027 2023-06-12 21:15:37.000000 pystac-client-0.7.0/pystac_client/client.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7170 2023-06-12 21:15:37.000000 pystac-client-0.7.0/pystac_client/collection_client.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1324 2023-06-12 21:15:37.000000 pystac-client-0.7.0/pystac_client/conformance.py
+-rw-r--r--   0 runner    (1001) docker     (123)      246 2023-06-12 21:15:37.000000 pystac-client-0.7.0/pystac_client/errors.py
+-rw-r--r--   0 runner    (1001) docker     (123)      449 2023-06-12 21:15:37.000000 pystac-client-0.7.0/pystac_client/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (123)    32409 2023-06-12 21:15:37.000000 pystac-client-0.7.0/pystac_client/item_search.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2217 2023-06-12 21:15:37.000000 pystac-client-0.7.0/pystac_client/mixins.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-12 21:15:37.000000 pystac-client-0.7.0/pystac_client/py.typed
+-rw-r--r--   0 runner    (1001) docker     (123)    12401 2023-06-12 21:15:37.000000 pystac-client-0.7.0/pystac_client/stac_api_io.py
+-rw-r--r--   0 runner    (1001) docker     (123)       22 2023-06-12 21:15:37.000000 pystac-client-0.7.0/pystac_client/version.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2767 2023-06-12 21:15:37.000000 pystac-client-0.7.0/pystac_client/warnings.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-12 21:16:01.587874 pystac-client-0.7.0/pystac_client.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     3175 2023-06-12 21:16:01.000000 pystac-client-0.7.0/pystac_client.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      758 2023-06-12 21:16:01.000000 pystac-client-0.7.0/pystac_client.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-12 21:16:01.000000 pystac-client-0.7.0/pystac_client.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       54 2023-06-12 21:16:01.000000 pystac-client-0.7.0/pystac_client.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      743 2023-06-12 21:16:01.000000 pystac-client-0.7.0/pystac_client.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       14 2023-06-12 21:16:01.000000 pystac-client-0.7.0/pystac_client.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-12 21:16:01.587874 pystac-client-0.7.0/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-12 21:16:01.587874 pystac-client-0.7.0/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)     2679 2023-06-12 21:15:37.000000 pystac-client-0.7.0/tests/test_cli.py
+-rw-r--r--   0 runner    (1001) docker     (123)    25263 2023-06-12 21:15:37.000000 pystac-client-0.7.0/tests/test_client.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2810 2023-06-12 21:15:37.000000 pystac-client-0.7.0/tests/test_collection_client.py
+-rw-r--r--   0 runner    (1001) docker     (123)    29284 2023-06-12 21:15:37.000000 pystac-client-0.7.0/tests/test_item_search.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9118 2023-06-12 21:15:37.000000 pystac-client-0.7.0/tests/test_stac_api_io.py
```

### Comparing `pystac-client-0.6.1/LICENSE` & `pystac-client-0.7.0/LICENSE`

 * *Files identical despite different names*

### Comparing `pystac-client-0.6.1/pystac_client/_utils.py` & `pystac-client-0.7.0/pystac_client/_utils.py`

 * *Files identical despite different names*

### Comparing `pystac-client-0.6.1/pystac_client/cli.py` & `pystac-client-0.7.0/pystac_client/cli.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,18 +1,29 @@
 import argparse
 import json
 import logging
 import os
 import re
 import sys
+import warnings
 from typing import Any, Dict, List, Optional
 
+from pystac import STACTypeError
+
 from .client import Client
+from .conformance import ConformanceClasses
 from .item_search import OPS
 from .version import __version__
+from .warnings import (
+    DoesNotConformTo,
+    FallbackToPystac,
+    MissingLink,
+    NoConformsTo,
+    PystacClientWarning,
+)
 
 logger = logging.getLogger(__name__)
 
 
 def search(
     client: Client,
     method: str = "GET",
@@ -37,33 +48,102 @@
                 with open(save, "w") as f:
                     f.write(json.dumps(feature_collection))
             else:
                 print(json.dumps(feature_collection))
         return 0
 
     except Exception as e:
-        print(e)
+        print(f"ERROR: {e}")
         return 1
 
 
 def collections(client: Client, save: Optional[str] = None) -> int:
     """Fetch collections from collections endpoint"""
     try:
         collections_dicts = [c.to_dict() for c in client.get_all_collections()]
         if save:
             with open(save, "w") as f:
                 f.write(json.dumps(collections_dicts))
         else:
             print(json.dumps(collections_dicts))
         return 0
+    except STACTypeError as e:
+        print(f"ERROR: {e}")
+        print(
+            f"The client at {client.self_href} is OK, but one or more of the "
+            "collections is invalid."
+        )
+        return 1
     except Exception as e:
-        print(e)
+        print(f"ERROR: {e}")
         return 1
 
 
+def add_warnings_behavior(parser: argparse.ArgumentParser) -> None:
+    warnings_group = parser.add_argument_group("warnings behavior")
+    warnings_group.add_argument(
+        "--error",
+        nargs="*",
+        choices=[
+            "no-conforms-to",
+            "does-not-conform-to",
+            "missing-link",
+            "fallback-to-pystac",
+        ],
+        help="Error on all stac-client warnings or specific warnings.",
+    )
+    warnings_group.add_argument(
+        "--ignore",
+        nargs="*",
+        choices=[
+            "no-conforms-to",
+            "does-not-conform-to",
+            "missing-link",
+            "fallback-to-pystac",
+        ],
+        help="Ignore all stac-client warnings or specific warnings.",
+    )
+
+
+def set_warnings(error: Optional[List[str]], ignore: Optional[List[str]]) -> None:
+    # First set filters on the base class
+    if ignore is not None and len(ignore) == 0:
+        warnings.filterwarnings("ignore", category=PystacClientWarning)
+    if error is not None and len(error) == 0:
+        warnings.filterwarnings("ignore", category=PystacClientWarning)
+
+    # Then set filters on any specific classes
+    category_options = {
+        "no-conforms-to": NoConformsTo,
+        "does-not-conform-to": DoesNotConformTo,
+        "missing-link": MissingLink,
+        "fallback-to-pystac": FallbackToPystac,
+    }
+    if ignore is not None:
+        for w in ignore:
+            warnings.filterwarnings("ignore", category=category_options[w])
+    if error is not None:
+        for w in error:
+            warnings.filterwarnings("error", category=category_options[w])
+
+
+def set_conforms_to(
+    client: Client, clear: bool, remove: Optional[List[str]], add: Optional[List[str]]
+) -> None:
+    """Alters conforms_to settings on client in-place"""
+    if clear:
+        client.clear_conforms_to()
+    if remove is not None:
+        for conformance_class in remove:
+            client.remove_conforms_to(conformance_class)
+    if add is not None:
+        for conformance_class in add:
+            client.add_conforms_to(conformance_class)
+
+
 def parse_args(args: List[str]) -> Dict[str, Any]:
     desc = "STAC Client"
     dhf = argparse.ArgumentDefaultsHelpFormatter
     parser0 = argparse.ArgumentParser(description=desc)
     parser0.add_argument(
         "--version",
         help="Print version and exit",
@@ -79,29 +159,42 @@
     parent.add_argument(
         "--headers",
         nargs="*",
         help="Additional request headers (KEY=VALUE pairs)",
         default=None,
     )
     parent.add_argument(
-        "--ignore-conformance",
-        dest="ignore_conformance",
+        "--add-conforms-to",
+        choices=[c.name for c in ConformanceClasses],
+        nargs="*",
+        help="Specify conformance classes to add to client",
+    )
+    parent.add_argument(
+        "--remove-conforms-to",
+        choices=[c.name for c in ConformanceClasses],
+        nargs="*",
+        help="Specify conformance classes to remove from client",
+    )
+    parent.add_argument(
+        "--clear-conforms-to",
         default=False,
         action="store_true",
     )
 
     subparsers = parser0.add_subparsers(dest="command")
 
     # collections command
     parser = subparsers.add_parser(
         "collections",
         help="Get all collections in this Catalog",
         parents=[parent],
         formatter_class=dhf,
     )
+    add_warnings_behavior(parser)
+
     output_group = parser.add_argument_group("output options")
     output_group.add_argument(
         "--save", help="Filename to save collections to", default=None
     )
 
     # search command
     parser = subparsers.add_parser(
@@ -157,14 +250,15 @@
     search_group.add_argument(
         "--max-items",
         dest="max_items",
         help="Max items to retrieve from search",
         type=int,
     )
     search_group.add_argument("--method", help="GET or POST", default="POST")
+    add_warnings_behavior(parser)
 
     output_group = parser.add_argument_group("output options")
     output_group.add_argument(
         "--matched", help="Print number matched", default=False, action="store_true"
     )
     output_group.add_argument(
         "--save", help="Filename to save Item collection to", default=None
@@ -228,29 +322,38 @@
         logging.getLogger("urllib3").propagate = False
 
     cmd = args.pop("command")
 
     try:
         url = args.pop("url")
         headers = args.pop("headers", {})
-        ignore_conformance = args.pop("ignore_conformance")
-        client = Client.open(
-            url, headers=headers, ignore_conformance=ignore_conformance
+
+        set_warnings(args.pop("error", None), args.pop("ignore", None))
+
+        client = Client.open(url, headers=headers)
+        set_conforms_to(
+            client,
+            args.pop("clear_conforms_to"),
+            args.pop("remove_conforms_to", None),
+            args.pop("add_conforms_to", None),
         )
+
     except Exception as e:
-        print(e)
+        print(f"ERROR: {e}", file=sys.stderr)
         return 1
 
     if cmd == "search":
         return search(client, **args)
     elif cmd == "collections":
         return collections(client, **args)
     else:
         print(
-            f"Command '{cmd}' is not a valid command, must be 'search' or 'collections'"
+            f"Command '{cmd}' is not a valid command. "
+            "must be 'search' or 'collections'",
+            file=sys.stderr,
         )
         return 1
 
 
 if __name__ == "__main__":
     return_code = cli()
     if return_code and return_code != 0:
```

### Comparing `pystac-client-0.6.1/pystac_client/client.py` & `pystac-client-0.7.0/pystac_client/client.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,9 +1,21 @@
+import re
+import warnings
 from functools import lru_cache
-from typing import TYPE_CHECKING, Any, Callable, Dict, Iterator, List, Optional, Union
+from typing import (
+    TYPE_CHECKING,
+    Any,
+    Callable,
+    Dict,
+    Iterator,
+    List,
+    Optional,
+    Union,
+    cast,
+)
 
 import pystac
 import pystac.utils
 import pystac.validation
 from pystac import CatalogType, Collection
 from requests import Request
 
@@ -22,21 +34,23 @@
     FilterLike,
     IDsLike,
     IntersectsLike,
     ItemSearch,
     QueryLike,
     SortbyLike,
 )
-from pystac_client.stac_api_io import StacApiIO
+from pystac_client.mixins import QUERYABLES_ENDPOINT, QueryablesMixin
+from pystac_client.stac_api_io import StacApiIO, Timeout
+from pystac_client.warnings import DoesNotConformTo, FallbackToPystac, NoConformsTo
 
 if TYPE_CHECKING:
     from pystac.item import Item as Item_Type
 
 
-class Client(pystac.Catalog):
+class Client(pystac.Catalog, QueryablesMixin):
     """A Client for interacting with the root of a STAC Catalog or API
 
     Instances of the ``Client`` class inherit from :class:`pystac.Catalog`
     and provide a convenient way of interacting
     with STAC Catalogs OR STAC APIs that conform to the `STAC API spec
     <https://github.com/radiantearth/stac-api-spec>`_.
     In addition to being a valid
@@ -79,33 +93,39 @@
 
     @classmethod
     def open(
         cls,
         url: str,
         headers: Optional[Dict[str, str]] = None,
         parameters: Optional[Dict[str, Any]] = None,
-        ignore_conformance: bool = False,
+        ignore_conformance: Optional[bool] = None,
         modifier: Optional[Callable[[Modifiable], None]] = None,
         request_modifier: Optional[Callable[[Request], Union[Request, None]]] = None,
         stac_io: Optional[StacApiIO] = None,
+        timeout: Optional[Timeout] = None,
     ) -> "Client":
         """Opens a STAC Catalog or API
         This function will read the root catalog of a STAC Catalog or API
 
         Args:
             url : The URL of a STAC Catalog.
             headers : A dictionary of additional headers to use in all requests
                 made to any part of this Catalog/API.
             parameters: Optional dictionary of query string parameters to
                 include in all requests.
-            ignore_conformance : Ignore any advertised Conformance Classes in this
-                Catalog/API. This means that
+            ignore_conformance (DEPRECATED) : Ignore any advertised Conformance Classes
+                in this Catalog/API. This means that
                 functions will skip checking conformance, and may throw an unknown
                 error if that feature is
                 not supported, rather than a :class:`NotImplementedError`.
+
+                .. deprecated:: 0.7.0
+                    Conformance can be altered rather than ignored using methods like
+                    :meth:`clear_conforms_to` and :meth:`add_conforms_to`
+
             modifier : A callable that modifies the children collection and items
                 returned by this Client. This can be useful for injecting
                 authentication parameters into child assets to access data
                 from non-public sources.
 
                 The callable should expect a single argument, which will be one
                 of the following types:
@@ -132,88 +152,158 @@
 
                 If the callable returns a `requests.Request`, that will be used.
                 Alternately, the callable may simply modify the provided request object
                 and return `None`.
             stac_io: A `StacApiIO` object to use for I/O requests. Generally, leave
                 this to the default. However in cases where customized I/O processing
                 is required, a custom instance can be provided here.
+            timeout: Optional float or (float, float) tuple following the semantics
+              defined by `Requests
+              <https://requests.readthedocs.io/en/latest/api/#main-interface>`__.
 
         Return:
             catalog : A :class:`Client` instance for this Catalog/API
         """
         client: Client = cls.from_file(
             url,
             headers=headers,
             parameters=parameters,
             modifier=modifier,
             request_modifier=request_modifier,
             stac_io=stac_io,
+            timeout=timeout,
         )
-        search_link = client.get_search_link()
-        # if there is a search link, but no conformsTo advertised, ignore
-        # conformance entirely
-        # NOTE: this behavior to be deprecated as implementations become conformant
-        if client._stac_io and (
-            ignore_conformance
-            or (
-                client
-                and "conformsTo" not in client.extra_fields.keys()
-                and search_link
-                and search_link.href
-                and len(search_link.href) > 0
+
+        if ignore_conformance is not None:
+            warnings.warn(
+                (
+                    "The `ignore_conformance` option is deprecated and will be "
+                    "removed in the next major release. Instead use `set_conforms_to` "
+                    "or `add_conforms_to` to control behavior."
+                ),
+                FutureWarning,
             )
-        ):
-            client._stac_io.set_conformance(None)
+
+        if not client.has_conforms_to():
+            warnings.warn(NoConformsTo())
 
         return client
 
     @classmethod
     def from_file(  # type: ignore
         cls,
         href: str,
         stac_io: Optional[StacApiIO] = None,
         headers: Optional[Dict[str, str]] = None,
         parameters: Optional[Dict[str, Any]] = None,
         modifier: Optional[Callable[[Modifiable], None]] = None,
         request_modifier: Optional[Callable[[Request], Union[Request, None]]] = None,
+        timeout: Optional[Timeout] = None,
     ) -> "Client":
         """Open a STAC Catalog/API
 
         Returns:
             Client: A Client (PySTAC Catalog) of the root Catalog for this Catalog/API
         """
         if stac_io is None:
             stac_io = StacApiIO(
                 headers=headers,
                 parameters=parameters,
                 request_modifier=request_modifier,
+                timeout=timeout,
             )
         else:
             stac_io.update(
                 headers=headers,
                 parameters=parameters,
                 request_modifier=request_modifier,
+                timeout=timeout,
             )
 
         client: Client = super().from_file(href, stac_io)
-
-        client._stac_io._conformance = client.extra_fields.get(  # type: ignore
-            "conformsTo", []
-        )
         client.modifier = modifier
 
         return client
 
-    def _supports_collections(self) -> bool:
-        return self._conforms_to(ConformanceClasses.COLLECTIONS) or self._conforms_to(
-            ConformanceClasses.FEATURES
+    def has_conforms_to(self) -> bool:
+        """Whether server contains list of ``"conformsTo"`` URIs"""
+        return "conformsTo" in self.extra_fields
+
+    def get_conforms_to(self) -> List[str]:
+        """List of ``"conformsTo"`` URIs
+
+        Return:
+            List[str]: List of  URIs that the server conforms to
+        """
+        return cast(List[str], self.extra_fields.get("conformsTo", []).copy())
+
+    def set_conforms_to(self, conformance_uris: List[str]) -> None:
+        """Set list of ``"conformsTo"`` URIs
+
+        Args:
+            conformance_uris : URIs indicating what the server conforms to
+        """
+        self.extra_fields["conformsTo"] = conformance_uris
+
+    def clear_conforms_to(self) -> None:
+        """Clear list of ``"conformsTo"`` urls
+
+        Removes the entire list, so :py:meth:`has_conforms_to` will
+        return False after using this method.
+        """
+        self.extra_fields.pop("conformsTo", None)
+
+    def add_conforms_to(self, name: str) -> None:
+        """Add ``"conformsTo"`` by name.
+
+        Args:
+            name : name of :py:class:`ConformanceClasses` keys to add.
+        """
+        conformance_class = ConformanceClasses.get_by_name(name)
+
+        if not self.conforms_to(conformance_class):
+            self.set_conforms_to([*self.get_conforms_to(), conformance_class.valid_uri])
+
+    def remove_conforms_to(self, name: str) -> None:
+        """Remove ``"conformsTo"`` by name.
+
+        Args:
+            name : name of :py:class:`ConformanceClasses` keys to remove.
+        """
+        conformance_class = ConformanceClasses.get_by_name(name)
+
+        self.set_conforms_to(
+            [
+                uri
+                for uri in self.get_conforms_to()
+                if not re.match(conformance_class.pattern, uri)
+            ]
         )
 
-    def _conforms_to(self, conformance_class: ConformanceClasses) -> bool:
-        return self._stac_io.conforms_to(conformance_class)  # type: ignore
+    def conforms_to(self, conformance_class: Union[ConformanceClasses, str]) -> bool:
+        """Checks whether the API conforms to the given standard.
+
+        This method only checks
+        against the ``"conformsTo"`` property from the API landing page and does not
+        make any additional calls to a ``/conformance`` endpoint even if the API
+        provides such an endpoint.
+
+        Args:
+            name : name of :py:class:`ConformanceClasses` keys to check
+                conformance against.
+
+        Return:
+            bool: Indicates if the API conforms to the given spec or URI.
+        """
+        if isinstance(conformance_class, str):
+            conformance_class = ConformanceClasses.get_by_name(conformance_class)
+
+        return any(
+            re.match(conformance_class.pattern, uri) for uri in self.get_conforms_to()
+        )
 
     @classmethod
     def from_dict(
         cls,
         d: Dict[str, Any],
         href: Optional[str] = None,
         root: Optional[pystac.Catalog] = None,
@@ -231,99 +321,154 @@
                 f"Could not open Client (href={href}), "
                 f"expected type=Catalog, found type={d.get('type', None)}"
             )
 
         result.modifier = modifier
         return result
 
+    def _supports_collections(self) -> bool:
+        return self.conforms_to(ConformanceClasses.COLLECTIONS) or self.conforms_to(
+            ConformanceClasses.FEATURES
+        )
+
+    def _warn_about_fallback(self, *args: str) -> None:
+        if self.has_conforms_to():
+            warnings.warn(DoesNotConformTo(*args), stacklevel=2)
+        warnings.warn(FallbackToPystac(), stacklevel=2)
+
+    def get_merged_queryables(self, collections: List[str]) -> Dict[str, Any]:
+        """Return the set of queryables in common to the specified collections.
+
+        Queryables from multiple collections are unioned together, except in the case
+        when the same queryable key has a different definition, in which case that key
+        is dropped.
+
+        Output is a dictionary that can be used in ``jsonshema.validate``
+
+        Args:
+            collections List[str]: The IDs of the collections to inspect.
+
+        Return:
+            Dict[str, Any]: Dictionary containing queryable fields
+        """
+        if not collections:
+            raise ValueError("cannot get_merged_queryables from empty Iterable")
+
+        if not self.conforms_to(ConformanceClasses.FILTER):
+            raise DoesNotConformTo(ConformanceClasses.FILTER.name)
+        response = self.get_queryables_from(
+            self._get_collection_queryables_href(collections[0])
+        )
+        response.pop("$id")
+        addl_props = response.get("additionalProperties", False)
+        for collection in collections[1:]:
+            resp = self.get_queryables_from(
+                self._get_collection_queryables_href(collection)
+            )
+
+            # additionalProperties is false if any collection doesn't support additional
+            # properties
+            addl_props &= resp.get("additionalProperties", False)
+
+            # drop queryables if their keys match, but the descriptions differ
+            for k in set(resp["properties"]).intersection(response["properties"]):
+                if resp["properties"][k] != response["properties"][k]:
+                    resp["properties"].pop(k)
+                    response["properties"].pop(k)
+            response["properties"].update(resp["properties"])
+        return response
+
     @lru_cache()
-    def get_collection(self, collection_id: str) -> Optional[Collection]:
+    def get_collection(self, collection_id: str) -> Union[Collection, CollectionClient]:
         """Get a single collection from this Catalog/API
 
         Args:
             collection_id: The Collection ID to get
 
         Returns:
-            CollectionClient: A STAC Collection
+            Union[Collection, CollectionClient]: A STAC Collection
+
+        Raises:
+            NotFoundError if collection_id does not exist.
         """
-        if self._supports_collections() and self._stac_io:
-            url = self._get_collections_href(collection_id)
+        collection: Union[Collection, CollectionClient]
+
+        if self._supports_collections():
+            assert self._stac_io is not None
+
+            url = self._collections_href(collection_id)
             collection = CollectionClient.from_dict(
                 self._stac_io.read_json(url),
                 root=self,
                 modifier=self.modifier,
             )
             call_modifier(self.modifier, collection)
-            return collection
         else:
-            for col in self.get_collections():
-                if col.id == collection_id:
-                    call_modifier(self.modifier, col)
-                    return col
-
-        return None
+            self._warn_about_fallback("COLLECTIONS", "FEATURES")
+            for collection in super().get_collections():
+                if collection.id == collection_id:
+                    call_modifier(self.modifier, collection)
+        return collection
 
     def get_collections(self) -> Iterator[Collection]:
         """Get Collections in this Catalog
 
             Gets the collections from the /collections endpoint if supported,
             otherwise fall back to Catalog behavior of following child links
 
         Return:
-            Iterator[Collection]: Iterator over Collections in Catalog/API
+            Iterator[Union[Collection, CollectionClient]]: Collections in Catalog/API
         """
         collection: Union[Collection, CollectionClient]
 
-        if self._supports_collections() and self._stac_io:
-            url = self._get_collections_href()
+        if self._supports_collections():
+            assert self._stac_io is not None
+
+            url = self._collections_href()
             for page in self._stac_io.get_pages(url):
                 if "collections" not in page:
                     raise APIError("Invalid response from /collections")
                 for col in page["collections"]:
                     collection = CollectionClient.from_dict(
                         col, root=self, modifier=self.modifier
                     )
                     call_modifier(self.modifier, collection)
                     yield collection
         else:
+            self._warn_about_fallback("COLLECTIONS", "FEATURES")
             for collection in super().get_collections():
                 call_modifier(self.modifier, collection)
                 yield collection
 
     def get_items(self) -> Iterator["Item_Type"]:
         """Return all items of this catalog.
 
         Return:
             Iterator[Item]:: Iterator of items whose parent is this
                 catalog.
         """
-        if self._conforms_to(ConformanceClasses.ITEM_SEARCH):
+        if self.conforms_to(ConformanceClasses.ITEM_SEARCH):
             search = self.search()
             yield from search.items()
         else:
+            self._warn_about_fallback("ITEM_SEARCH")
             for item in super().get_items():
                 call_modifier(self.modifier, item)
                 yield item
 
     def get_all_items(self) -> Iterator["Item_Type"]:
         """Get all items from this catalog and all subcatalogs. Will traverse
         any subcatalogs recursively, or use the /search endpoint if supported
 
         Returns:
             Iterator[Item]:: All items that belong to this catalog, and all
                 catalogs or collections connected to this catalog through
                 child links.
         """
-        if self._conforms_to(ConformanceClasses.ITEM_SEARCH):
-            # these are already modified
-            yield from self.get_items()
-        else:
-            for item in super().get_items():
-                call_modifier(self.modifier, item)
-                yield item
+        yield from self.get_items()
 
     def search(
         self,
         *,
         method: Optional[str] = "POST",
         max_items: Optional[int] = None,
         limit: Optional[int] = DEFAULT_LIMIT_AND_MAX_ITEMS,
@@ -434,37 +579,24 @@
 
         Raises:
             NotImplementedError: If the API does not conform to the `Item Search spec
                 <https://github.com/radiantearth/stac-api-spec/tree/master/item-search>`__
                 or does not have a link with
                 a ``"rel"`` type of ``"search"``.
         """
-        if not self._conforms_to(ConformanceClasses.ITEM_SEARCH):
-            raise NotImplementedError(
-                "This catalog does not support search because it "
-                f'does not conform to "{ConformanceClasses.ITEM_SEARCH}"'
-            )
-        search_link = self.get_search_link()
-        if search_link:
-            if isinstance(search_link.target, str):
-                search_href = search_link.target
-            else:
-                raise NotImplementedError(
-                    "Link with rel=search was an object rather than a URI"
-                )
-        else:
-            raise NotImplementedError(
-                "No link with rel=search could be found in this catalog"
+
+        if not self.conforms_to(ConformanceClasses.ITEM_SEARCH):
+            raise DoesNotConformTo(
+                "ITEM_SEARCH", "There is not fallback option available for search."
             )
 
         return ItemSearch(
-            url=search_href,
+            url=self._search_href(),
             method=method,
             max_items=max_items,
-            stac_io=self._stac_io,
             client=self,
             limit=limit,
             ids=ids,
             collections=collections,
             bbox=bbox,
             intersects=intersects,
             datetime=datetime,
@@ -493,39 +625,24 @@
                     link.media_type == pystac.MediaType.GEOJSON
                     or link.media_type == pystac.MediaType.JSON
                 )
             ),
             None,
         )
 
-    def _get_collections_href(self, collection_id: Optional[str] = None) -> str:
-        self_href = self.get_self_href()
-        if self_href is None:
-            data_link = self.get_single_link("data")
-            if data_link is None:
-                raise ValueError(
-                    "cannot build a collections href without a self href or a data link"
-                )
-            else:
-                collections_href = data_link.href
-        else:
-            collections_href = f"{self_href.rstrip('/')}/collections"
-
-        if not pystac.utils.is_absolute_href(collections_href):
-            collections_href = self._make_absolute_href(collections_href)
-
-        if collection_id is None:
-            return collections_href
-        else:
-            return f"{collections_href.rstrip('/')}/{collection_id}"
+    def _search_href(self) -> str:
+        search_link = self.get_search_link()
+        href = self._get_href("search", search_link, "search")
+        return href
 
-    def _make_absolute_href(self, href: str) -> str:
-        self_link = self.get_single_link("self")
-        if self_link is None:
-            raise ValueError("cannot build an absolute href without a self link")
-        elif not pystac.utils.is_absolute_href(self_link.href):
-            raise ValueError(
-                "cannot build an absolute href from "
-                f"a relative self link: {self_link.href}"
-            )
-        else:
-            return pystac.utils.make_absolute_href(href, self_link.href)
+    def _collections_href(self, collection_id: Optional[str] = None) -> str:
+        data_link = self.get_single_link("data")
+        href = self._get_href("data", data_link, "collections")
+        if collection_id is not None:
+            return f"{href.rstrip('/')}/{collection_id}"
+        return href
+
+    def _get_collection_queryables_href(
+        self, collection_id: Optional[str] = None
+    ) -> str:
+        href = self._collections_href(collection_id)
+        return f"{href.rstrip('/')}/{QUERYABLES_ENDPOINT}"
```

### Comparing `pystac-client-0.6.1/pystac_client/collection_client.py` & `pystac-client-0.7.0/pystac_client/collection_client.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,24 +1,41 @@
-from typing import TYPE_CHECKING, Any, Callable, Dict, Iterator, List, Optional, cast
+from __future__ import annotations
+
+import warnings
+from typing import (
+    TYPE_CHECKING,
+    Any,
+    Callable,
+    Dict,
+    Iterator,
+    List,
+    Optional,
+    Union,
+    cast,
+)
 
 import pystac
 
 from pystac_client._utils import Modifiable, call_modifier
 from pystac_client.conformance import ConformanceClasses
 from pystac_client.exceptions import APIError
 from pystac_client.item_search import ItemSearch
+from pystac_client.mixins import QueryablesMixin
 from pystac_client.stac_api_io import StacApiIO
+from pystac_client.warnings import FallbackToPystac
 
 if TYPE_CHECKING:
     from pystac.item import Item as Item_Type
 
+    from pystac_client import Client
+
 
-class CollectionClient(pystac.Collection):
+class CollectionClient(pystac.Collection, QueryablesMixin):
     modifier: Callable[[Modifiable], None]
-    _stac_io: Optional[StacApiIO]
+    _stac_io: StacApiIO
 
     def __init__(
         self,
         id: str,
         description: str,
         extent: pystac.Extent,
         title: Optional[str] = None,
@@ -55,57 +72,74 @@
         setattr(self, "modifier", modifier)
 
     @classmethod
     def from_dict(
         cls,
         d: Dict[str, Any],
         href: Optional[str] = None,
-        root: Optional[pystac.Catalog] = None,
+        root: Optional[Union[pystac.Catalog, Client]] = None,
         migrate: bool = False,
         preserve_dict: bool = True,
         modifier: Optional[Callable[[Modifiable], None]] = None,
     ) -> "CollectionClient":
         result = super().from_dict(d, href, root, migrate, preserve_dict)
         # error: Cannot assign to a method  [assignment]
         # https://github.com/python/mypy/issues/2427
         setattr(result, "modifier", modifier)
         return result
 
     def __repr__(self) -> str:
         return "<CollectionClient id={}>".format(self.id)
 
+    def set_root(self, root: Optional[Union[pystac.Catalog, Client]]) -> None:
+        # hook in to set_root and use it for setting _stac_io
+        super().set_root(root=root)
+        if root is None:
+            raise ValueError("`CollectionClient.root` must be set")
+        elif root._stac_io is not None and isinstance(root._stac_io, StacApiIO):
+            self._stac_io = root._stac_io
+        else:
+            raise ValueError("`CollectionClient.root` must be a valid `Client` object")
+
+    def get_root(self) -> Client:
+        from pystac_client.client import Client
+
+        root = super().get_root()
+        if root is None or not isinstance(root, Client):
+            raise ValueError(
+                "`CollectionClient.root` is not have a valid `Client` object."
+            )
+        return root
+
+    def conforms_to(self, conformance_class: Union[ConformanceClasses, str]) -> bool:
+        root = self.get_root()
+        return root.conforms_to(conformance_class)
+
     def get_items(self) -> Iterator["Item_Type"]:
         """Return all items in this Collection.
 
         If the Collection contains a link of with a `rel` value of `items`,
         that link will be used to iterate through items. Otherwise, the default
         PySTAC behavior is assumed.
 
         Return:
             Iterator[Item]: Iterator of items whose parent is this catalog.
         """
-
-        link = self.get_single_link("items")
         root = self.get_root()
-        if link is not None and root is not None:
-            # error: Argument "stac_io" to "ItemSearch" has incompatible type
-            # "Optional[StacIO]"; expected "Optional[StacApiIO]"  [arg-type]
-            # so we add these asserts
-            stac_io = root._stac_io
-            assert stac_io
-            assert isinstance(stac_io, StacApiIO)
-
+        if root.conforms_to(ConformanceClasses.ITEM_SEARCH):
             search = ItemSearch(
-                url=link.href,
+                url=self._items_href(),
                 method="GET",
-                stac_io=stac_io,
+                client=root,
+                collections=[self.id],
                 modifier=self.modifier,
             )
             yield from search.items()
         else:
+            root._warn_about_fallback("ITEM_SEARCH")
             for item in super().get_items():
                 call_modifier(self.modifier, item)
                 yield item
 
     def get_item(self, id: str, recursive: bool = False) -> Optional["Item_Type"]:
         """Returns an item with a given ID.
 
@@ -124,53 +158,43 @@
                 to False.
 
         Return:
             Item or None: The item with the given ID, or None if not found.
         """
         if not recursive:
             root = self.get_root()
-            assert root
-            stac_io = root._stac_io
-            assert stac_io
-            assert isinstance(stac_io, StacApiIO)
-            items_link = self.get_single_link("items")
-            if root:
-                search_link = root.get_single_link("search")
-            else:
-                search_link = None
-            if (
-                stac_io.conforms_to(ConformanceClasses.FEATURES)
-                and items_link is not None
-            ):
-                url = f"{items_link.href}/{id}"
+            if root.conforms_to(ConformanceClasses.FEATURES) and self._stac_io:
+                url = f"{self._items_href().rstrip('/')}/{id}"
                 try:
-                    obj = stac_io.read_stac_object(url, root=self)
+                    obj = self._stac_io.read_stac_object(url, root=self)
                     item = cast(Optional[pystac.Item], obj)
                 except APIError as err:
-                    if err.status_code and err.status_code == 404:
+                    if getattr(err, "status_code", None) and err.status_code == 404:
                         return None
                     else:
                         raise err
-                assert isinstance(item, pystac.Item)
-            elif (
-                stac_io.conforms_to(ConformanceClasses.ITEM_SEARCH)
-                and search_link
-                and search_link.href
-            ):
+            elif root.conforms_to(ConformanceClasses.ITEM_SEARCH) and self._stac_io:
                 item_search = ItemSearch(
-                    url=search_link.href,
+                    url=root._search_href(),
                     method="GET",
-                    stac_io=self._stac_io,
+                    client=root,
                     ids=[id],
                     collections=[self.id],
                     modifier=self.modifier,
                 )
                 item = next(item_search.items(), None)
             else:
+                root._warn_about_fallback("FEATURES", "ITEM_SEARCH")
                 item = super().get_item(id, recursive=False)
         else:
+            warnings.warn(FallbackToPystac())
             item = super().get_item(id, recursive=True)
 
         if item:
             call_modifier(self.modifier, item)
 
         return item
+
+    def _items_href(self) -> str:
+        link = self.get_single_link("items")
+        href = self._get_href("items", link, "items")
+        return href
```

### Comparing `pystac-client-0.6.1/pystac_client/item_search.py` & `pystac-client-0.7.0/pystac_client/item_search.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,9 @@
 import json
 import re
-import urllib.parse
 import warnings
 from collections.abc import Iterable, Mapping
 from copy import deepcopy
 from datetime import datetime as datetime_
 from datetime import timezone
 from functools import lru_cache
 from itertools import chain
@@ -25,14 +24,15 @@
 from dateutil.tz import tzutc
 from pystac import Collection, Item, ItemCollection
 from requests import Request
 
 from pystac_client._utils import Modifiable, call_modifier
 from pystac_client.conformance import ConformanceClasses
 from pystac_client.stac_api_io import StacApiIO
+from pystac_client.warnings import DoesNotConformTo
 
 if TYPE_CHECKING:
     from pystac_client import client as _client
 
 DATETIME_REGEX = re.compile(
     r"^(?P<year>\d{4})(-(?P<month>\d{2})(-(?P<day>\d{2})"
     r"(?P<remainder>([Tt])\d{2}:\d{2}:\d{2}(\.\d+)?"
@@ -137,24 +137,23 @@
     `STAC API - Item Search spec
     <https://github.com/radiantearth/stac-api-spec/tree/master/item-search>`__.
 
     No request is sent to the API until a method is called to iterate
     through the resulting STAC Items, either :meth:`ItemSearch.item_collections`,
     :meth:`ItemSearch.items`, or :meth:`ItemSearch.items_as_dicts`.
 
-    All parameters except `url``, ``method``, ``max_items``, ``stac_io``, and ``client``
+    All parameters except `url``, ``method``, ``max_items``, and ``client``
     correspond to query parameters
     described in the `STAC API - Item Search: Query Parameters Table
     <https://github.com/radiantearth/stac-api-spec/tree/master/item-search#query-parameter-table>`__
     docs. Please refer
     to those docs for details on how these parameters filter search results.
 
     Args:
-        url: The URL to the root / landing page of the STAC API
-            implementing the Item Search endpoint.
+        url: The URL to the search page of the STAC API.
         method : The HTTP method to use when making a request to the service.
             This must be either ``"GET"``, ``"POST"``, or
             ``None``. If ``None``, this will default to ``"POST"``.
             If a ``"POST"`` request receives a ``405`` status for
             the response, it will automatically retry with
             ``"GET"`` for all subsequent requests.
         max_items : The maximum number of items to return from the search, even
@@ -245,14 +244,16 @@
 
             ``modifier`` propagates recursively to children of this Client.
             After getting a child collection with, e.g.
             :meth:`Client.get_collection`, the child items of that collection
             will still be signed with ``modifier``.
     """
 
+    _stac_io: StacApiIO
+
     def __init__(
         self,
         url: str,
         *,
         method: Optional[str] = "POST",
         max_items: Optional[int] = None,
         stac_io: Optional[StacApiIO] = None,
@@ -269,20 +270,20 @@
         sortby: Optional[SortbyLike] = None,
         fields: Optional[FieldsLike] = None,
         modifier: Optional[Callable[[Modifiable], None]] = None,
     ):
         self.url = url
         self.client = client
 
-        if stac_io:
-            self._stac_io = stac_io
+        if client and client._stac_io is not None and stac_io is None:
+            self._stac_io = client._stac_io
+            if not client.conforms_to(ConformanceClasses.ITEM_SEARCH):
+                warnings.warn(DoesNotConformTo("ITEM_SEARCH"))
         else:
-            self._stac_io = StacApiIO()
-
-        self._assert_conforms_to(ConformanceClasses.ITEM_SEARCH)
+            self._stac_io = stac_io or StacApiIO()
 
         self._max_items = max_items
         if self._max_items is not None and limit is not None:
             limit = min(limit, self._max_items)
 
         if limit is not None and (limit < 1 or limit > 10000):
             raise Exception(f"Invalid limit of {limit}, must be between 1 and 10,000")
@@ -304,17 +305,14 @@
             "fields": self._format_fields(fields),
         }
 
         self._parameters: Dict[str, Any] = {
             k: v for k, v in params.items() if v is not None
         }
 
-    def _assert_conforms_to(self, conformance_class: ConformanceClasses) -> None:
-        self._stac_io.assert_conforms_to(conformance_class)
-
     def get_parameters(self) -> Dict[str, Any]:
         if self.method == "POST":
             return self._parameters
         elif self.method == "GET":
             return self._clean_params_for_get_request()
         else:
             raise Exception(f"Unsupported method {self.method}")
@@ -324,15 +322,19 @@
         if "bbox" in params:
             params["bbox"] = ",".join(map(str, params["bbox"]))
         if "ids" in params:
             params["ids"] = ",".join(params["ids"])
         if "collections" in params:
             params["collections"] = ",".join(params["collections"])
         if "intersects" in params:
-            params["intersects"] = json.dumps(params["intersects"])
+            params["intersects"] = json.dumps(
+                params["intersects"], separators=(",", ":")
+            )
+        if "query" in params:
+            params["query"] = json.dumps(params["query"], separators=(",", ":"))
         if "sortby" in params:
             params["sortby"] = self._sortby_dict_to_str(params["sortby"])
         if "fields" in params:
             params["fields"] = self._fields_dict_to_str(params["fields"])
         return params
 
     def url_with_parameters(self) -> str:
@@ -355,21 +357,22 @@
             str: The search url with parameters.
         """
         params = self._clean_params_for_get_request()
         request = Request("GET", self.url, params=params)
         url = request.prepare().url
         if url is None:
             raise ValueError("Could not construct a full url")
-        return urllib.parse.unquote(url)
+        return url
 
     def _format_query(self, value: Optional[QueryLike]) -> Optional[Dict[str, Any]]:
         if value is None:
             return None
 
-        self._assert_conforms_to(ConformanceClasses.QUERY)
+        if self.client and not self.client.conforms_to(ConformanceClasses.QUERY):
+            warnings.warn(DoesNotConformTo("QUERY"))
 
         if isinstance(value, dict):
             return value
         elif isinstance(value, list):
             query: Dict[str, Any] = {}
             for q in value:
                 if isinstance(q, str):
@@ -410,15 +413,16 @@
 
         return None
 
     def _format_filter(self, value: Optional[FilterLike]) -> Optional[FilterLike]:
         if value is None:
             return None
 
-        self._assert_conforms_to(ConformanceClasses.FILTER)
+        if self.client and not self.client.conforms_to(ConformanceClasses.FILTER):
+            warnings.warn(DoesNotConformTo("FILTER"))
 
         return value
 
     @staticmethod
     def _format_bbox(value: Optional[BBoxLike]) -> Optional[BBox]:
         if value is None:
             return None
@@ -554,15 +558,16 @@
 
         return tuple(value)
 
     def _format_sortby(self, value: Optional[SortbyLike]) -> Optional[Sortby]:
         if value is None:
             return None
 
-        self._assert_conforms_to(ConformanceClasses.SORT)
+        if self.client and not self.client.conforms_to(ConformanceClasses.SORT):
+            warnings.warn(DoesNotConformTo("SORT"))
 
         if isinstance(value, str):
             return [self._sortby_part_to_dict(part) for part in value.split(",")]
 
         if isinstance(value, list):
             if value and isinstance(value[0], str):
                 return [self._sortby_part_to_dict(str(v)) for v in value]
@@ -591,15 +596,16 @@
             ]
         )
 
     def _format_fields(self, value: Optional[FieldsLike]) -> Optional[Fields]:
         if value is None:
             return None
 
-        self._assert_conforms_to(ConformanceClasses.FIELDS)
+        if self.client and not self.client.conforms_to(ConformanceClasses.FIELDS):
+            warnings.warn(DoesNotConformTo("FIELDS"))
 
         if isinstance(value, str):
             return self._fields_to_dict(value.split(","))
         if isinstance(value, list):
             return self._fields_to_dict(value)
         if isinstance(value, dict):
             return value
@@ -682,24 +688,18 @@
     def items_as_dicts(self) -> Iterator[Dict[str, Any]]:
         """Iterator that yields :class:`dict` instances for each item matching
         the given search parameters.
 
         Yields:
             Item : each Item matching the search criteria
         """
-        nitems = 0
-        for page in self._stac_io.get_pages(
-            self.url, self.method, self.get_parameters()
-        ):
+        for page in self.pages_as_dicts():
             for item in page.get("features", []):
-                call_modifier(self.modifier, item)
+                # already signed in pages_as_dicts
                 yield item
-                nitems += 1
-                if self._max_items and nitems >= self._max_items:
-                    return
 
     # ------------------------------------------------------------------------
     # By Page
     def pages(self) -> Iterator[ItemCollection]:
         """Iterator that yields ItemCollection objects.  Each ItemCollection is
         a page of results from the search.
 
@@ -719,19 +719,30 @@
         of results from the search.
 
         Yields:
             Dict : a group of items matching the search
             criteria as a feature-collection-like dictionary.
         """
         if isinstance(self._stac_io, StacApiIO):
+            num_items = 0
             for page in self._stac_io.get_pages(
                 self.url, self.method, self.get_parameters()
             ):
                 call_modifier(self.modifier, page)
-                yield page
+                features = page.get("features", [])
+                if features:
+                    num_items += len(features)
+                    if self._max_items and num_items > self._max_items:
+                        # Slice the features down to make sure we hit max_items
+                        page["features"] = features[0 : -(num_items - self._max_items)]
+                    yield page
+                    if self._max_items and num_items >= self._max_items:
+                        return
+                else:
+                    return
 
     # ------------------------------------------------------------------------
     # Everything
 
     @lru_cache(1)
     def item_collection(self) -> ItemCollection:
         """
@@ -759,28 +770,18 @@
         2. ``'features'`` with the value being a list of dictionaries
             for the matching items.
 
         Return:
             Dict : A GeoJSON FeatureCollection
         """
         features = []
-        for page in self._stac_io.get_pages(
-            self.url, self.method, self.get_parameters()
-        ):
+        for page in self.pages_as_dicts():
             for feature in page["features"]:
                 features.append(feature)
-                if self._max_items and len(features) >= self._max_items:
-                    feature_collection = {
-                        "type": "FeatureCollection",
-                        "features": features,
-                    }
-                    call_modifier(self.modifier, feature_collection)
-                    return feature_collection
         feature_collection = {"type": "FeatureCollection", "features": features}
-        call_modifier(self.modifier, feature_collection)
         return feature_collection
 
     # Deprecated methods
     # not caching these, since they're cached in the implementation
 
     def get_item_collections(self) -> Iterator[ItemCollection]:
         """DEPRECATED
@@ -789,15 +790,15 @@
             Use :meth:`ItemSearch.pages` instead.
 
         Yields:
             ItemCollection : a group of Items matching the search criteria.
         """
         warnings.warn(
             "get_item_collections() is deprecated, use pages() instead",
-            DeprecationWarning,
+            FutureWarning,
         )
         return self.pages()
 
     def item_collections(self) -> Iterator[ItemCollection]:
         """DEPRECATED
 
         .. deprecated:: 0.5.0
@@ -805,45 +806,45 @@
 
         Yields:
             ItemCollection : a group of Items matching the search criteria within an
             ItemCollection
         """
         warnings.warn(
             "item_collections() is deprecated, use pages() instead",
-            DeprecationWarning,
+            FutureWarning,
         )
         return self.pages()
 
     def get_items(self) -> Iterator[Item]:
         """DEPRECATED.
 
         .. deprecated:: 0.4.0
             Use :meth:`ItemSearch.items` instead.
 
         Yields:
             Item : each Item matching the search criteria
         """
         warnings.warn(
             "get_items() is deprecated, use items() instead",
-            DeprecationWarning,
+            FutureWarning,
         )
         return self.items()
 
     def get_all_items(self) -> ItemCollection:
         """DEPRECATED
 
         .. deprecated:: 0.4.0
            Use :meth:`ItemSearch.item_collection` instead.
 
         Return:
             item_collection : ItemCollection
         """
         warnings.warn(
             "get_all_items() is deprecated, use item_collection() instead.",
-            DeprecationWarning,
+            FutureWarning,
         )
         return self.item_collection()
 
     def get_all_items_as_dict(self) -> Dict[str, Any]:
         """DEPRECATED
 
         .. deprecated:: 0.4.0
@@ -851,10 +852,10 @@
 
         Return:
             Dict : A GeoJSON FeatureCollection
         """
         warnings.warn(
             "get_all_items_as_dict() is deprecated, use item_collection_as_dict() "
             "instead.",
-            DeprecationWarning,
+            FutureWarning,
         )
         return self.item_collection_as_dict()
```

### Comparing `pystac-client-0.6.1/pystac_client/stac_api_io.py` & `pystac-client-0.7.0/pystac_client/stac_api_io.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,88 +1,133 @@
 import json
 import logging
-import re
+import warnings
 from copy import deepcopy
-from typing import TYPE_CHECKING, Any, Callable, Dict, Iterator, List, Optional, Union
+from typing import (
+    TYPE_CHECKING,
+    Any,
+    Callable,
+    Dict,
+    Iterator,
+    List,
+    Optional,
+    Tuple,
+    Union,
+)
 from urllib.parse import urlparse
 
 import pystac
 from pystac.link import Link
 from pystac.serialization import (
     identify_stac_object,
     identify_stac_object_type,
     merge_common_properties,
     migrate_to_latest,
 )
 from pystac.stac_io import DefaultStacIO
 from requests import Request, Session
+from requests.adapters import HTTPAdapter
+from typing_extensions import TypeAlias
 
 import pystac_client
 
-from .conformance import CONFORMANCE_URIS, ConformanceClasses
 from .exceptions import APIError
 
 if TYPE_CHECKING:
     from pystac.catalog import Catalog as Catalog_Type
     from pystac.stac_object import STACObject as STACObject_Type
 
 logger = logging.getLogger(__name__)
 
 
+Timeout: TypeAlias = Union[float, Tuple[float, float], Tuple[float, None]]
+
+
 class StacApiIO(DefaultStacIO):
     def __init__(
         self,
         headers: Optional[Dict[str, str]] = None,
         conformance: Optional[List[str]] = None,
         parameters: Optional[Dict[str, Any]] = None,
         request_modifier: Optional[Callable[[Request], Union[Request, None]]] = None,
+        timeout: Optional[Timeout] = None,
+        max_retries: Optional[int] = 5,
     ):
         """Initialize class for API IO
 
         Args:
             headers : Optional dictionary of headers to include in all requests
-            conformance : Optional list of `Conformance Classes
+            conformance (DEPRECATED) : Optional list of `Conformance Classes
                 <https://github.com/radiantearth/stac-api-spec/blob/master/overview.md#conformance-classes>`__.
+
+                .. deprecated:: 0.7.0
+                    Conformance can be altered on the client class directly
+
             parameters: Optional dictionary of query string parameters to
               include in all requests.
             request_modifier: Optional callable that can be used to modify Request
               objects before they are sent. If provided, the callable receives a
               `request.Request` and must either modify the object directly or return
               a new / modified request instance.
+            timeout: Optional float or (float, float) tuple following the semantics
+              defined by `Requests
+              <https://requests.readthedocs.io/en/latest/api/#main-interface>`__.
+            max_retries: The number of times to retry requests. Set to ``None`` to
+              disable retries.
 
         Return:
             StacApiIO : StacApiIO instance
         """
         # TODO - this should super() to parent class
+
+        if conformance is not None:
+            warnings.warn(
+                (
+                    "The `conformance` option is deprecated and will be "
+                    "removed in the next major release. Instead use "
+                    "`Client.set_conforms_to` or `Client.add_conforms_to` to control "
+                    "behavior."
+                ),
+                category=FutureWarning,
+            )
+
         self.session = Session()
-        self._conformance = conformance
+        if max_retries:
+            self.session.mount("http://", HTTPAdapter(max_retries=max_retries))
+            self.session.mount("https://", HTTPAdapter(max_retries=max_retries))
+        self.timeout = timeout
         self.update(
             headers=headers, parameters=parameters, request_modifier=request_modifier
         )
 
     def update(
         self,
         headers: Optional[Dict[str, str]] = None,
         parameters: Optional[Dict[str, Any]] = None,
         request_modifier: Optional[Callable[[Request], Union[Request, None]]] = None,
+        timeout: Optional[Timeout] = None,
     ) -> None:
         """Updates this StacApi's headers, parameters, and/or request_modifer.
 
         Args:
             headers : Optional dictionary of headers to include in all requests
             parameters: Optional dictionary of query string parameters to
               include in all requests.
             request_modifier: Optional callable that can be used to modify Request
               objects before they are sent. If provided, the callable receives a
               `request.Request` and must either modify the object directly or return
               a new / modified request instance.
+            timeout: Optional float or (float, float) tuple following the semantics
+              defined by `Requests
+              <https://requests.readthedocs.io/en/latest/api/#main-interface>`__.
         """
         self.session.headers.update(headers or {})
         self.session.params.update(parameters or {})  # type: ignore
         self._req_modifier = request_modifier
+        self.timeout = timeout
 
     def read_text(self, source: pystac.link.HREF, *args: Any, **kwargs: Any) -> str:
         """Read text from the given URI.
 
         Overwrites the default method for reading text from a URL or file to allow
         :class:`urllib.request.Request` instances as input. This method also raises
         any :exc:`urllib.error.HTTPError` exceptions rather than catching
@@ -150,26 +195,27 @@
         Return:
             str: The decoded response from the endpoint
         """
         if method == "POST":
             request = Request(method=method, url=href, headers=headers, json=parameters)
         else:
             params = deepcopy(parameters) or {}
-            if "intersects" in params:
-                params["intersects"] = json.dumps(params["intersects"])
             request = Request(method="GET", url=href, headers=headers, params=params)
         try:
             modified = self._req_modifier(request) if self._req_modifier else None
             prepped = self.session.prepare_request(modified or request)
             msg = f"{prepped.method} {prepped.url} Headers: {prepped.headers}"
             if method == "POST":
                 msg += f" Payload: {json.dumps(request.json)}"
+            if self.timeout is not None:
+                msg += f" Timeout: {self.timeout}"
             logger.debug(msg)
-            resp = self.session.send(prepped)
+            resp = self.session.send(prepped, timeout=self.timeout)
         except Exception as err:
+            logger.debug(err)
             raise APIError(str(err))
         if resp.status_code != 200:
             raise APIError.from_response(resp)
         try:
             return resp.content.decode("utf-8")
         except Exception as err:
             raise APIError(str(err))
@@ -218,14 +264,15 @@
             result = pystac_client.client.Client.from_dict(
                 d, href=str(href), root=root, migrate=False, preserve_dict=preserve_dict
             )
             result._stac_io = self
             return result
 
         if info.object_type == pystac.STACObjectType.COLLECTION:
+            assert isinstance(root, pystac_client.client.Client)
             return pystac_client.collection_client.CollectionClient.from_dict(
                 d, href=str(href), root=root, migrate=False, preserve_dict=preserve_dict
             )
 
         if info.object_type == pystac.STACObjectType.ITEM:
             return pystac.Item.from_dict(
                 d, href=str(href), root=root, migrate=False, preserve_dict=preserve_dict
@@ -261,59 +308,11 @@
             yield page
 
             # get the next link and make the next request
             next_link = next(
                 (link for link in page.get("links", []) if link["rel"] == "next"), None
             )
 
-    def assert_conforms_to(self, conformance_class: ConformanceClasses) -> None:
-        """Raises a :exc:`NotImplementedError` if the API does not publish the given
-        conformance class. This method only checks against the ``"conformsTo"``
-        property from the API landing page and does not make any additional
-        calls to a ``/conformance`` endpoint even if the API provides such an endpoint.
-
-        Args:
-            conformance_class: The ``ConformanceClasses`` key to check conformance
-            against.
-        """
-        if not self.conforms_to(conformance_class):
-            raise NotImplementedError(f"{conformance_class} not supported")
-
-    def conforms_to(self, conformance_class: ConformanceClasses) -> bool:
-        """Whether the API conforms to the given standard. This method only checks
-        against the ``"conformsTo"`` property from the API landing page and does not
-        make any additional calls to a ``/conformance`` endpoint even if the API
-        provides such an endpoint.
-
-        Args:
-            conformance_class : The ``ConformanceClasses`` key to check conformance
-                against.
-
-        Return:
-            bool: Indicates if the API conforms to the given spec or URI.
-        """
-
-        # Conformance of None means ignore all conformance as opposed to an
-        #  empty array which would indicate the API conforms to nothing
-        if self._conformance is None:
-            return True
-
-        class_regex = CONFORMANCE_URIS.get(conformance_class.name, None)
-
-        if class_regex is None:
-            raise Exception(f"Invalid conformance class {conformance_class}")
-
-        pattern = re.compile(class_regex)
-
-        if not any(re.match(pattern, uri) for uri in self._conformance):
-            return False
-
-        return True
-
-    def set_conformance(self, conformance: Optional[List[str]]) -> None:
-        """Sets (or clears) the conformance classes for this StacIO."""
-        self._conformance = conformance
-
 
 def _is_url(href: str) -> bool:
     url = urlparse(href)
     return bool(url.scheme) and bool(url.netloc)
```

### Comparing `pystac-client-0.6.1/pystac_client.egg-info/SOURCES.txt` & `pystac-client-0.7.0/pystac_client.egg-info/SOURCES.txt`

 * *Files 14% similar despite different names*

```diff
@@ -1,24 +1,29 @@
 LICENSE
 MANIFEST.in
 README.md
-setup.cfg
-setup.py
+pyproject.toml
 pystac_client/__init__.py
 pystac_client/_utils.py
 pystac_client/cli.py
 pystac_client/client.py
 pystac_client/collection_client.py
 pystac_client/conformance.py
 pystac_client/errors.py
 pystac_client/exceptions.py
 pystac_client/item_search.py
+pystac_client/mixins.py
 pystac_client/py.typed
 pystac_client/stac_api_io.py
 pystac_client/version.py
+pystac_client/warnings.py
 pystac_client.egg-info/PKG-INFO
 pystac_client.egg-info/SOURCES.txt
 pystac_client.egg-info/dependency_links.txt
 pystac_client.egg-info/entry_points.txt
-pystac_client.egg-info/not-zip-safe
 pystac_client.egg-info/requires.txt
-pystac_client.egg-info/top_level.txt
+pystac_client.egg-info/top_level.txt
+tests/test_cli.py
+tests/test_client.py
+tests/test_collection_client.py
+tests/test_item_search.py
+tests/test_stac_api_io.py
```

