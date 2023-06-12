# Comparing `tmp/simple-zarr-server-0.1.0.tar.gz` & `tmp/simple_zarr_server-0.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/simple-zarr-server-0.1.0.tar", last modified: Thu Sep  3 12:22:24 2020, max compression
+gzip compressed data, last modified: Sun Feb  2 00:00:00 2020, max compression
```

## Comparing `simple-zarr-server-0.1.0.tar` & `simple_zarr_server-0.2.0.tar`

### file list

```diff
@@ -1,28 +1,11 @@
-drwxr-xr-x   0 runner    (1001) docker     (116)        0 2020-09-03 12:22:24.285981 simple-zarr-server-0.1.0/
-drwxr-xr-x   0 runner    (1001) docker     (116)        0 2020-09-03 12:22:24.277980 simple-zarr-server-0.1.0/.github/
-drwxr-xr-x   0 runner    (1001) docker     (116)        0 2020-09-03 12:22:24.281981 simple-zarr-server-0.1.0/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (116)     1845 2020-09-03 12:22:15.000000 simple-zarr-server-0.1.0/.github/workflows/test_and_deploy.yml
--rw-r--r--   0 runner    (1001) docker     (116)      978 2020-09-03 12:22:15.000000 simple-zarr-server-0.1.0/.gitignore
--rw-r--r--   0 runner    (1001) docker     (116)     1488 2020-09-03 12:22:15.000000 simple-zarr-server-0.1.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (116)      121 2020-09-03 12:22:15.000000 simple-zarr-server-0.1.0/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (116)     7185 2020-09-03 12:22:24.285981 simple-zarr-server-0.1.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (116)     5011 2020-09-03 12:22:15.000000 simple-zarr-server-0.1.0/README.md
--rw-r--r--   0 runner    (1001) docker     (116)       60 2020-09-03 12:22:15.000000 simple-zarr-server-0.1.0/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (116)       38 2020-09-03 12:22:24.285981 simple-zarr-server-0.1.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (116)     1793 2020-09-03 12:22:15.000000 simple-zarr-server-0.1.0/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (116)        0 2020-09-03 12:22:24.281981 simple-zarr-server-0.1.0/simple_zarr_server/
--rw-r--r--   0 runner    (1001) docker     (116)      148 2020-09-03 12:22:15.000000 simple-zarr-server-0.1.0/simple_zarr_server/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (116)        0 2020-09-03 12:22:24.281981 simple-zarr-server-0.1.0/simple_zarr_server/_tests/
--rw-r--r--   0 runner    (1001) docker     (116)        0 2020-09-03 12:22:15.000000 simple-zarr-server-0.1.0/simple_zarr_server/_tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (116)     2058 2020-09-03 12:22:15.000000 simple-zarr-server-0.1.0/simple_zarr_server/_tests/test_simple_zarr_server.py
--rw-r--r--   0 runner    (1001) docker     (116)      116 2020-09-03 12:22:24.000000 simple-zarr-server-0.1.0/simple_zarr_server/_version.py
--rw-r--r--   0 runner    (1001) docker     (116)     2874 2020-09-03 12:22:15.000000 simple-zarr-server-0.1.0/simple_zarr_server/cli.py
--rw-r--r--   0 runner    (1001) docker     (116)     3386 2020-09-03 12:22:15.000000 simple-zarr-server-0.1.0/simple_zarr_server/server.py
-drwxr-xr-x   0 runner    (1001) docker     (116)        0 2020-09-03 12:22:24.281981 simple-zarr-server-0.1.0/simple_zarr_server.egg-info/
--rw-r--r--   0 runner    (1001) docker     (116)     7185 2020-09-03 12:22:24.000000 simple-zarr-server-0.1.0/simple_zarr_server.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (116)      574 2020-09-03 12:22:24.000000 simple-zarr-server-0.1.0/simple_zarr_server.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (116)        1 2020-09-03 12:22:24.000000 simple-zarr-server-0.1.0/simple_zarr_server.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (116)       68 2020-09-03 12:22:24.000000 simple-zarr-server-0.1.0/simple_zarr_server.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (116)       60 2020-09-03 12:22:24.000000 simple-zarr-server-0.1.0/simple_zarr_server.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (116)       19 2020-09-03 12:22:24.000000 simple-zarr-server-0.1.0/simple_zarr_server.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (116)      507 2020-09-03 12:22:15.000000 simple-zarr-server-0.1.0/tox.ini
+-rw-r--r--   0        0        0      959 2020-02-02 00:00:00.000000 simple_zarr_server-0.2.0/.github/workflows/ci.yml
+-rw-r--r--   0        0        0      808 2020-02-02 00:00:00.000000 simple_zarr_server-0.2.0/.github/workflows/release.yml
+-rw-r--r--   0        0        0      266 2020-02-02 00:00:00.000000 simple_zarr_server-0.2.0/src/simple_zarr_server/__init__.py
+-rw-r--r--   0        0        0     2875 2020-02-02 00:00:00.000000 simple_zarr_server-0.2.0/src/simple_zarr_server/cli.py
+-rw-r--r--   0        0        0     3590 2020-02-02 00:00:00.000000 simple_zarr_server-0.2.0/src/simple_zarr_server/server.py
+-rw-r--r--   0        0        0     2320 2020-02-02 00:00:00.000000 simple_zarr_server-0.2.0/tests/test_simple_zarr_server.py
+-rw-r--r--   0        0        0      978 2020-02-02 00:00:00.000000 simple_zarr_server-0.2.0/.gitignore
+-rw-r--r--   0        0        0     1488 2020-02-02 00:00:00.000000 simple_zarr_server-0.2.0/LICENSE
+-rw-r--r--   0        0        0     5011 2020-02-02 00:00:00.000000 simple_zarr_server-0.2.0/README.md
+-rw-r--r--   0        0        0     2121 2020-02-02 00:00:00.000000 simple_zarr_server-0.2.0/pyproject.toml
+-rw-r--r--   0        0        0     5757 2020-02-02 00:00:00.000000 simple_zarr_server-0.2.0/PKG-INFO
```

### Comparing `simple-zarr-server-0.1.0/.gitignore` & `simple_zarr_server-0.2.0/.gitignore`

 * *Files identical despite different names*

### Comparing `simple-zarr-server-0.1.0/LICENSE` & `simple_zarr_server-0.2.0/LICENSE`

 * *Files identical despite different names*

### Comparing `simple-zarr-server-0.1.0/README.md` & `simple_zarr_server-0.2.0/README.md`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 # simple-zarr-server
 
-[![License](https://img.shields.io/pypi/l/simple-zarr-server.svg)](https://github.com/manzt/simple-zarr-server/raw/master/LICENSE)
+[![License](https://img.shields.io/pypi/l/simple-zarr-server.svg)](https://github.com/manzt/simple-zarr-server/raw/main/LICENSE)
 [![PyPI](https://img.shields.io/pypi/v/simple-zarr-server.svg?color=green)](https://pypi.org/project/simple-zarr-server)
 [![Python Version](https://img.shields.io/pypi/pyversions/simple-zarr-server.svg?color=green)](https://python.org)
 [![tests](https://github.com/manzt/simple-zarr-server/workflows/tests/badge.svg)](https://github.com/manzt/simple-zarr-server/actions)
 
 A minimal server for sharing zarr over HTTP.
 
 ----------------------------------
@@ -53,15 +53,15 @@
 ```
 
 #### Python API:
 
 The python API is more flexible than the CLI, and can serve any [`zarr.Array`](https://zarr.readthedocs.io/en/stable/api/core.html#zarr.core.Array), 
 [`zarr.Group`](https://zarr.readthedocs.io/en/stable/api/hierarchy.html#zarr.hierarchy.Group) or `np.ndarray`. 
 
-##### Server 
+##### Server
 
 ```python
 from simple_zarr_server import serve
 import numpy as np
 arr = np.random.rand(1024, 1024)
 serve(arr) # creates an in-memory store if not zarr.Array or zarr.Group
 ```
@@ -69,15 +69,15 @@
 ##### Client
 
 ##### `zarr-python`
 
 ```python
 import zarr
 from fsspec import get_mapper
-store = get_mapper("http://localhost:8000") 
+store = get_mapper("http://localhost:8000")
 arr = zarr.open(store, mode='r')
 # or 
 import dask.array as da
 arr = da.from_zarr("http://localhost:8000")
 ```
 
 ##### `zarr.js`
@@ -130,23 +130,23 @@
 Some non-standard zarr stores that might be of interest include:
 
 - [`napari_lazy_openslide.OpenSlideStore`](https://github.com/manzt/napari-lazy-openslide) - read multiscale RGB TIFFs as zarr
 - [`HDF5Zarr`](https://github.com/catalystneuro/HDF5Zarr) - read HDF5 with zarr
 
 ## Contributing
 
-Contributions are very welcome. Tests can be run with [tox].
+Contributions are very welcome. Tests can be run with `hatch run cov`.
 
 ## License
 
 Distributed under the terms of the [BSD-3] license,
 "simple-zarr-server" is free and open source software
 
 ## Issues
 
 If you encounter any problems, please [file an issue] along with a detailed description.
 
 [BSD-3]: http://opensource.org/licenses/BSD-3-Clause
 [file an issue]: https://github.com/manzt/simple-zarr-server/issues
-[tox]: https://tox.readthedocs.io/en/latest/
+[hatch]: https://hatch.pypa.io/latest/
 [pip]: https://pypi.org/project/pip/
 [PyPI]: https://pypi.org/
```

### Comparing `simple-zarr-server-0.1.0/simple_zarr_server/_tests/test_simple_zarr_server.py` & `simple_zarr_server-0.2.0/tests/test_simple_zarr_server.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,36 +1,45 @@
-import pytest
 import numpy as np
+import pytest
 import zarr
-from simple_zarr_server.server import create_zarr_route
-from starlette.testclient import TestClient
 from starlette.applications import Starlette
+from starlette.testclient import TestClient
+from zarr.storage import BaseStore
+
+from simple_zarr_server.server import create_zarr_route
 
 
-class HTTPStore:
-    def __init__(self, client):
+class HTTPStore(BaseStore):
+    def __init__(self, client: TestClient):
         self.client = client
 
-    def __getitem__(self, path):
+    def __getitem__(self, path: str):
         r = self.client.get(f"/{path}")
-        if r.ok:
-            return r.content
-        else:
-            raise KeyError
+        if r.is_error:
+            raise KeyError(path)
+        return r.content
 
-    def __contains__(self, path):
+    def __contains__(self, path: str):
         r = self.client.head(f"/{path}")
-        if r.ok:
-            return True
+        return r.is_success
 
-    def __setitem__(self, path, cdata):
-        r = self.client.put(f"/{path}", cdata)
-        if not r.ok:
+    def __setitem__(self, path: str, cdata: bytes):
+        r = self.client.put(f"/{path}", content=cdata)
+        if r.is_error:
             raise ValueError
 
+    def __delitem__(self, path: str):
+        raise NotImplementedError
+
+    def __len__(self):
+        raise NotImplementedError
+
+    def __iter__(self):
+        raise NotImplementedError
+
 
 def test_numpy_read_only():
     # Create data
     original = np.random.rand(1024, 1024)
     z = zarr.array(original, read_only=True)
 
     # Initialize app
```

### Comparing `simple-zarr-server-0.1.0/simple_zarr_server/cli.py` & `simple_zarr_server-0.2.0/src/simple_zarr_server/cli.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,17 +1,18 @@
 import click
-from simple_zarr_server.server import serve
 import zarr
 from uvicorn.config import (
     HTTP_PROTOCOLS,
     LIFESPAN,
     LOOP_SETUPS,
     WS_PROTOCOLS,
 )
 
+from simple_zarr_server.server import serve
+
 HTTP_CHOICES = click.Choice(HTTP_PROTOCOLS.keys())
 WS_CHOICES = click.Choice(WS_PROTOCOLS.keys())
 LIFESPAN_CHOICES = click.Choice(LIFESPAN.keys())
 LOOP_CHOICES = click.Choice([key for key in LOOP_SETUPS.keys() if key != "none"])
 
 
 @click.command()
```

### Comparing `simple-zarr-server-0.1.0/simple_zarr_server/server.py` & `simple_zarr_server-0.2.0/src/simple_zarr_server/server.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,45 +1,46 @@
-import numpy as np
-from starlette.applications import Starlette
-from starlette.responses import Response
-from starlette.routing import Route, Mount
-from starlette.middleware.cors import CORSMiddleware
+from __future__ import annotations
 
+import numpy as np
 import uvicorn
 import zarr
+from starlette.applications import Starlette
+from starlette.middleware.cors import CORSMiddleware
+from starlette.responses import Response
+from starlette.routing import Mount, Route
 
 
-def create_zarr_route(z):
+def create_zarr_route(z: zarr.Array | zarr.Group) -> Route:
     """Creates a Starlette app, mapping HTTP requests on top of a Zarr store.
 
     Parameters
     ----------
     z : zarr.Array or zarr.Group
         Part of zarr hierarchy to expose over HTTP. The `read_only` property is
         checked to determine which HTTP methods are available.
 
     Returns
     -------
-    app : starlette.applications.Starlette
-        Starlette app
+    route : starlette.routing.Route
+        Route object that can be added to a Starlette app.
     """
     # Use read_only property to determine how the underlying store should be protected.
     methods = ["GET", "HEAD", "PUT"] if not z.read_only else ["GET", "HEAD"]
     # If z isn't the root of a hierarchy, need to prepend it's path.
     path_prefix = f"{z.path}/" if z.path else ""
 
     async def map_request(request):
         path = path_prefix + request.path_params["path"]
         if request.method == "PUT":
             # PUT only handled if writeable
             try:
                 blob = await request.body()
                 z.store[path] = blob
                 return Response(status_code=200)
-            except:
+            except Exception:
                 return Response(status_code=404)
         else:
             try:
                 # Return blob if GET, otherwise it's HEAD and should return empty body
                 body = z.store[path]
                 if request.method == "HEAD":
                     body = None
@@ -47,25 +48,31 @@
             except KeyError:
                 # Key not in store, return 404
                 return Response(status_code=404)
 
     return Route("/{path:path}", endpoint=map_request, methods=methods)
 
 
-def serve(source, *, name=None, allowed_origins=None, **kwargs):
+def serve(
+    source: zarr.Array | zarr.Group | np.ndarray,
+    *,
+    name: str | None = None,
+    allowed_origins: list[str] | None = None,
+    **kwargs,
+):
     """Starts an HTTP server, serving a part of a zarr hierarchy or numpy array as zarr.
 
     Parameters
     ----------
     source : zarr.Array, zarr.Group, or np.ndarray
         Source data to serve over HTTP. The underlying store of a zarr.Array,
         or zarr.Group are used to forward requests. If a numpy array is provided,
-        an in-memory zarry array is created, and the underlying store is wrapped.
+        an in-memory zarray array is created, and the underlying store is wrapped.
     name : str
-        Path prefix for underlying store keys (e.g. "data.zarr"). If provided, routes are 
+        Path prefix for underlying store keys (e.g. "data.zarr"). If provided, routes are
         prefixed with name.
     allowed_origins : list of str, optional
         List of allowed origins (as strings). Use wildcard "*" to allow all.
     **kwargs : keyword arguments
         All extra keyword arguments are forwarded to uvicorn.run
     """
```

