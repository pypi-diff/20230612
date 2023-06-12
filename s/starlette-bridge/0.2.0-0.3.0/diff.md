# Comparing `tmp/starlette_bridge-0.2.0.tar.gz` & `tmp/starlette_bridge-0.3.0.tar.gz`

## Comparing `starlette_bridge-0.2.0.tar` & `starlette_bridge-0.3.0.tar`

### file list

```diff
@@ -1,10 +1,10 @@
--rw-r--r--   0        0        0       78 2020-02-02 00:00:00.000000 starlette_bridge-0.2.0/starlette_bridge/__init__.py
--rw-r--r--   0        0        0     2274 2020-02-02 00:00:00.000000 starlette_bridge-0.2.0/starlette_bridge/bridge.py
--rw-r--r--   0        0        0     1205 2020-02-02 00:00:00.000000 starlette_bridge-0.2.0/starlette_bridge/context_managers.py
--rw-r--r--   0        0        0        1 2020-02-02 00:00:00.000000 starlette_bridge-0.2.0/starlette_bridge/py.typed
--rw-r--r--   0        0        0     2679 2020-02-02 00:00:00.000000 starlette_bridge-0.2.0/starlette_bridge/routing.py
--rw-r--r--   0        0        0      277 2020-02-02 00:00:00.000000 starlette_bridge-0.2.0/.gitignore
--rw-r--r--   0        0        0     1078 2020-02-02 00:00:00.000000 starlette_bridge-0.2.0/LICENSE
--rw-r--r--   0        0        0     5050 2020-02-02 00:00:00.000000 starlette_bridge-0.2.0/README.md
--rw-r--r--   0        0        0     3717 2020-02-02 00:00:00.000000 starlette_bridge-0.2.0/pyproject.toml
--rw-r--r--   0        0        0     8130 2020-02-02 00:00:00.000000 starlette_bridge-0.2.0/PKG-INFO
+-rw-r--r--   0        0        0       78 2020-02-02 00:00:00.000000 starlette_bridge-0.3.0/starlette_bridge/__init__.py
+-rw-r--r--   0        0        0     2274 2020-02-02 00:00:00.000000 starlette_bridge-0.3.0/starlette_bridge/bridge.py
+-rw-r--r--   0        0        0     1205 2020-02-02 00:00:00.000000 starlette_bridge-0.3.0/starlette_bridge/context_managers.py
+-rw-r--r--   0        0        0        1 2020-02-02 00:00:00.000000 starlette_bridge-0.3.0/starlette_bridge/py.typed
+-rw-r--r--   0        0        0     2679 2020-02-02 00:00:00.000000 starlette_bridge-0.3.0/starlette_bridge/routing.py
+-rw-r--r--   0        0        0      277 2020-02-02 00:00:00.000000 starlette_bridge-0.3.0/.gitignore
+-rw-r--r--   0        0        0     1078 2020-02-02 00:00:00.000000 starlette_bridge-0.3.0/LICENSE
+-rw-r--r--   0        0        0     5050 2020-02-02 00:00:00.000000 starlette_bridge-0.3.0/README.md
+-rw-r--r--   0        0        0     3715 2020-02-02 00:00:00.000000 starlette_bridge-0.3.0/pyproject.toml
+-rw-r--r--   0        0        0     8128 2020-02-02 00:00:00.000000 starlette_bridge-0.3.0/PKG-INFO
```

### Comparing `starlette_bridge-0.2.0/starlette_bridge/bridge.py` & `starlette_bridge-0.3.0/starlette_bridge/bridge.py`

 * *Files identical despite different names*

### Comparing `starlette_bridge-0.2.0/starlette_bridge/context_managers.py` & `starlette_bridge-0.3.0/starlette_bridge/context_managers.py`

 * *Files identical despite different names*

### Comparing `starlette_bridge-0.2.0/starlette_bridge/routing.py` & `starlette_bridge-0.3.0/starlette_bridge/routing.py`

 * *Files identical despite different names*

### Comparing `starlette_bridge-0.2.0/LICENSE` & `starlette_bridge-0.3.0/LICENSE`

 * *Files identical despite different names*

### Comparing `starlette_bridge-0.2.0/README.md` & `starlette_bridge-0.3.0/README.md`

 * *Files identical despite different names*

### Comparing `starlette_bridge-0.2.0/pyproject.toml` & `starlette_bridge-0.3.0/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -33,15 +33,15 @@
     "Programming Language :: Python :: 3.8",
     "Programming Language :: Python :: 3.9",
     "Programming Language :: Python :: 3.10",
     "Programming Language :: Python :: 3.11",
     "Topic :: Internet :: WWW/HTTP :: HTTP Servers",
     "Topic :: Internet :: WWW/HTTP",
 ]
-dependencies = ["starlette>=0.27.0,<0.30.0"]
+dependencies = ["starlette>=0.28.0,<1.0"]
 keywords = [
     "api",
     "rest",
     "http",
     "asgi",
     "pydantic",
     "starlette",
@@ -66,30 +66,30 @@
     "anyio>=3.0.0,<4",
     "anyio[trio]>=3.2.1,<4.0.0",
     "asyncio[trio]>=3.4.3,<4.0.0",
     "black== 23.3.0",
     "flake8>=5.0.4",
     "httpx>=0.22.0",
     "isort>=5.0.6,<6.0.0",
-    "mypy==1.1.1",
+    "mypy==1.3.0",
     "mock==5.0.1",
     "pytest>=7.1.3,<8.0.0",
     "pytest-cov>=2.12.0,<5.0.0",
     "pytest-asyncio >=0.19.0",
     "ruff>=0.0.256,<1.0.0",
     "types-orjson==3.6.2",
 ]
 
 doc = [
     "mkautodoc>=0.2.0,<0.3.0",
     "mkdocs>=1.4.2,<2.0.0",
-    "mkdocs-material==9.1.5",
+    "mkdocs-material==9.1.15",
     "mdx-include>=1.4.1,<2.0.0",
     "mkdocs-markdownextradata-plugin>=0.1.7,<0.3.0",
-    "mkdocstrings>=0.19.0,<0.21.0",
+    "mkdocstrings>=0.19.0,<0.23.0",
     "pyyaml>=5.3.1,<7.0.0",
 ]
 
 [tool.hatch.version]
 path = "starlette_bridge/__init__.py"
 
 [tool.isort]
```

### Comparing `starlette_bridge-0.2.0/PKG-INFO` & `starlette_bridge-0.3.0/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: starlette_bridge
-Version: 0.2.0
+Version: 0.3.0
 Summary: The Starlette events bridge that you need.
 Project-URL: Homepage, https://github.com/tarsil/starlette-bridge
 Project-URL: Documentation, https://starlette-bridge.tarsild.io/
 Project-URL: Changelog, https://starlette-bridge.tarsild.io/release-notes/
 Project-URL: Funding, https://github.com/sponsors/tarsil
 Project-URL: Source, https://github.com/tarsil/starlette-bridge
 Author-email: Tiago Silva <tiago.arasilva@gmail.com>
@@ -32,33 +32,33 @@
 Classifier: Topic :: Internet :: WWW/HTTP :: HTTP Servers
 Classifier: Topic :: Software Development
 Classifier: Topic :: Software Development :: Libraries
 Classifier: Topic :: Software Development :: Libraries :: Application Frameworks
 Classifier: Topic :: Software Development :: Libraries :: Python Modules
 Classifier: Typing :: Typed
 Requires-Python: >=3.8
-Requires-Dist: starlette<0.30.0,>=0.27.0
+Requires-Dist: starlette<1.0,>=0.28.0
 Provides-Extra: doc
 Requires-Dist: mdx-include<2.0.0,>=1.4.1; extra == 'doc'
 Requires-Dist: mkautodoc<0.3.0,>=0.2.0; extra == 'doc'
 Requires-Dist: mkdocs-markdownextradata-plugin<0.3.0,>=0.1.7; extra == 'doc'
-Requires-Dist: mkdocs-material==9.1.5; extra == 'doc'
+Requires-Dist: mkdocs-material==9.1.15; extra == 'doc'
 Requires-Dist: mkdocs<2.0.0,>=1.4.2; extra == 'doc'
-Requires-Dist: mkdocstrings<0.21.0,>=0.19.0; extra == 'doc'
+Requires-Dist: mkdocstrings<0.23.0,>=0.19.0; extra == 'doc'
 Requires-Dist: pyyaml<7.0.0,>=5.3.1; extra == 'doc'
 Provides-Extra: test
 Requires-Dist: anyio<4,>=3.0.0; extra == 'test'
 Requires-Dist: anyio[trio]<4.0.0,>=3.2.1; extra == 'test'
 Requires-Dist: asyncio[trio]<4.0.0,>=3.4.3; extra == 'test'
 Requires-Dist: black==23.3.0; extra == 'test'
 Requires-Dist: flake8>=5.0.4; extra == 'test'
 Requires-Dist: httpx>=0.22.0; extra == 'test'
 Requires-Dist: isort<6.0.0,>=5.0.6; extra == 'test'
 Requires-Dist: mock==5.0.1; extra == 'test'
-Requires-Dist: mypy==1.1.1; extra == 'test'
+Requires-Dist: mypy==1.3.0; extra == 'test'
 Requires-Dist: pytest-asyncio>=0.19.0; extra == 'test'
 Requires-Dist: pytest-cov<5.0.0,>=2.12.0; extra == 'test'
 Requires-Dist: pytest<8.0.0,>=7.1.3; extra == 'test'
 Requires-Dist: ruff<1.0.0,>=0.0.256; extra == 'test'
 Requires-Dist: types-orjson==3.6.2; extra == 'test'
 Description-Content-Type: text/markdown
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: starlette_bridge Version: 0.2.0 Summary: The
+Metadata-Version: 2.1 Name: starlette_bridge Version: 0.3.0 Summary: The
 Starlette events bridge that you need. Project-URL: Homepage, https://
 github.com/tarsil/starlette-bridge Project-URL: Documentation, https://
 starlette-bridge.tarsild.io/ Project-URL: Changelog, https://starlette-
 bridge.tarsild.io/release-notes/ Project-URL: Funding, https://github.com/
 sponsors/tarsil Project-URL: Source, https://github.com/tarsil/starlette-bridge
 Author-email: Tiago Silva
 arasilva@gmail.com> License-Expression: MIT License-File: LICENSE Keywords:
@@ -19,27 +19,27 @@
 Python :: 3.9 Classifier: Programming Language :: Python :: 3.10 Classifier:
 Programming Language :: Python :: 3.11 Classifier: Topic :: Internet
 Classifier: Topic :: Internet :: WWW/HTTP Classifier: Topic :: Internet :: WWW/
 HTTP :: HTTP Servers Classifier: Topic :: Software Development Classifier:
 Topic :: Software Development :: Libraries Classifier: Topic :: Software
 Development :: Libraries :: Application Frameworks Classifier: Topic ::
 Software Development :: Libraries :: Python Modules Classifier: Typing :: Typed
-Requires-Python: >=3.8 Requires-Dist: starlette<0.30.0,>=0.27.0 Provides-Extra:
+Requires-Python: >=3.8 Requires-Dist: starlette<1.0,>=0.28.0 Provides-Extra:
 doc Requires-Dist: mdx-include<2.0.0,>=1.4.1; extra == 'doc' Requires-Dist:
 mkautodoc<0.3.0,>=0.2.0; extra == 'doc' Requires-Dist: mkdocs-
 markdownextradata-plugin<0.3.0,>=0.1.7; extra == 'doc' Requires-Dist: mkdocs-
-material==9.1.5; extra == 'doc' Requires-Dist: mkdocs<2.0.0,>=1.4.2; extra ==
-'doc' Requires-Dist: mkdocstrings<0.21.0,>=0.19.0; extra == 'doc' Requires-
+material==9.1.15; extra == 'doc' Requires-Dist: mkdocs<2.0.0,>=1.4.2; extra ==
+'doc' Requires-Dist: mkdocstrings<0.23.0,>=0.19.0; extra == 'doc' Requires-
 Dist: pyyaml<7.0.0,>=5.3.1; extra == 'doc' Provides-Extra: test Requires-Dist:
 anyio<4,>=3.0.0; extra == 'test' Requires-Dist: anyio[trio]<4.0.0,>=3.2.1;
 extra == 'test' Requires-Dist: asyncio[trio]<4.0.0,>=3.4.3; extra == 'test'
 Requires-Dist: black==23.3.0; extra == 'test' Requires-Dist: flake8>=5.0.4;
 extra == 'test' Requires-Dist: httpx>=0.22.0; extra == 'test' Requires-Dist:
 isort<6.0.0,>=5.0.6; extra == 'test' Requires-Dist: mock==5.0.1; extra ==
-'test' Requires-Dist: mypy==1.1.1; extra == 'test' Requires-Dist: pytest-
+'test' Requires-Dist: mypy==1.3.0; extra == 'test' Requires-Dist: pytest-
 asyncio>=0.19.0; extra == 'test' Requires-Dist: pytest-cov<5.0.0,>=2.12.0;
 extra == 'test' Requires-Dist: pytest<8.0.0,>=7.1.3; extra == 'test' Requires-
 Dist: ruff<1.0.0,>=0.0.256; extra == 'test' Requires-Dist: types-orjson==3.6.2;
 extra == 'test' Description-Content-Type: text/markdown # Starlette Bridge
                               [Starlette_Bridge]
              ð The Starlette events bridge that you need. ð
           [Test_Suite] [Package_version] [Supported_Python_versions]
```

