# Comparing `tmp/jinja2_async_environment-0.1.4.tar.gz` & `tmp/jinja2_async_environment-0.1.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "jinja2_async_environment-0.1.4.tar", last modified: Fri May 19 14:38:42 2023, max compression
+gzip compressed data, was "jinja2_async_environment-0.1.5.tar", last modified: Sun Jun 11 22:54:03 2023, max compression
```

## Comparing `jinja2_async_environment-0.1.4.tar` & `jinja2_async_environment-0.1.5.tar`

### file list

```diff
@@ -1,9 +1,9 @@
--rw-r--r--   0        0        0     1518 2023-04-29 16:12:44.541343 jinja2_async_environment-0.1.4/LICENSE
--rw-r--r--   0        0        0     6245 2023-04-29 16:12:44.541545 jinja2_async_environment-0.1.4/README.md
--rw-r--r--   0        0        0      497 2023-05-19 14:34:15.779905 jinja2_async_environment-0.1.4/jinja2_async_environment/__init__.py
--rw-r--r--   0        0        0     1342 2023-04-29 16:58:02.839049 jinja2_async_environment-0.1.4/jinja2_async_environment/bccache.py
--rw-r--r--   0        0        0     5079 2023-04-16 01:42:22.123633 jinja2_async_environment-0.1.4/jinja2_async_environment/compiler.py
--rw-r--r--   0        0        0     1790 2023-04-29 17:13:12.496114 jinja2_async_environment-0.1.4/jinja2_async_environment/environment.py
--rw-r--r--   0        0        0    10606 2023-05-19 14:31:50.584841 jinja2_async_environment-0.1.4/jinja2_async_environment/loaders.py
--rw-r--r--   0        0        0      997 2023-05-19 14:38:42.808681 jinja2_async_environment-0.1.4/pyproject.toml
--rw-r--r--   0        0        0     6539 1970-01-01 00:00:00.000000 jinja2_async_environment-0.1.4/PKG-INFO
+-rw-r--r--   0        0        0     1518 2023-04-29 16:12:44.541343 jinja2_async_environment-0.1.5/LICENSE
+-rw-r--r--   0        0        0      255 2023-06-11 17:54:31.705304 jinja2_async_environment-0.1.5/README.md
+-rw-r--r--   0        0        0      497 2023-06-08 14:36:19.764543 jinja2_async_environment-0.1.5/jinja2_async_environment/__init__.py
+-rw-r--r--   0        0        0     1395 2023-06-11 20:52:38.004790 jinja2_async_environment-0.1.5/jinja2_async_environment/bccache.py
+-rw-r--r--   0        0        0     5079 2023-04-16 01:42:22.123633 jinja2_async_environment-0.1.5/jinja2_async_environment/compiler.py
+-rw-r--r--   0        0        0     1545 2023-06-11 17:38:28.289761 jinja2_async_environment-0.1.5/jinja2_async_environment/environment.py
+-rw-r--r--   0        0        0     9734 2023-06-11 21:49:07.502050 jinja2_async_environment-0.1.5/jinja2_async_environment/loaders.py
+-rw-r--r--   0        0        0      963 2023-06-11 22:54:03.219132 jinja2_async_environment-0.1.5/pyproject.toml
+-rw-r--r--   0        0        0      518 1970-01-01 00:00:00.000000 jinja2_async_environment-0.1.5/PKG-INFO
```

### Comparing `jinja2_async_environment-0.1.4/LICENSE` & `jinja2_async_environment-0.1.5/LICENSE`

 * *Files identical despite different names*

### Comparing `jinja2_async_environment-0.1.4/jinja2_async_environment/bccache.py` & `jinja2_async_environment-0.1.5/jinja2_async_environment/bccache.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,41 +1,42 @@
 import typing as t
 
-from .environment import AsyncEnvironment
+from aiopath import AsyncPath
 from jinja2 import BytecodeCache
 from jinja2.bccache import Bucket
 from redis.asyncio import Redis as AsyncRedis
+from .environment import AsyncEnvironment
 
 
 class AsyncRedisBytecodeCache(AsyncRedis, BytecodeCache):
     def __init__(self, prefix: t.Optional[str] = None, **configs) -> None:
         super().__init__(**configs)
         self.prefix = prefix
 
-    def get_bucket_name(self, key):
+    def get_bucket_name(self, key: str) -> str:
         return ":".join([self.prefix, key]) if self.prefix else key
 
-    async def load_bytecode(self, key_bucket):
+    async def load_bytecode(self, key_bucket: Bucket) -> bytes | None:
         code = await self.get(self.get_bucket_name(key_bucket.key))
-        if code is not None:
+        if code:
             return key_bucket.bytecode_from_string(code)
 
-    async def dump_bytecode(self, key_bucket) -> None:
+    async def dump_bytecode(self, key_bucket: Bucket) -> None:
         await self.set(
             self.get_bucket_name(key_bucket.key), key_bucket.bytecode_to_string()
         )
 
     async def get_bucket(
         self,
         environment: "AsyncEnvironment",
         name: str,
-        filename: t.Optional[str],
+        path: AsyncPath,
         source: str,
     ) -> Bucket:
-        key = self.get_cache_key(name, filename)
+        key = self.get_cache_key(name, path.name)
         checksum = self.get_source_checksum(source)
         bucket = Bucket(environment, key, checksum)
         await self.load_bytecode(bucket)
         return bucket
 
     async def set_bucket(self, bucket: Bucket) -> None:
         await self.dump_bytecode(bucket)
```

### Comparing `jinja2_async_environment-0.1.4/jinja2_async_environment/compiler.py` & `jinja2_async_environment-0.1.5/jinja2_async_environment/compiler.py`

 * *Files identical despite different names*

### Comparing `jinja2_async_environment-0.1.4/jinja2_async_environment/environment.py` & `jinja2_async_environment-0.1.5/jinja2_async_environment/environment.py`

 * *Files 21% similar despite different names*

```diff
@@ -1,30 +1,25 @@
 import typing as t
 from weakref import ref
 
-from .bccache import AsyncRedisBytecodeCache
-from .compiler import AsyncCodeGenerator
 from jinja2 import Environment
 from jinja2.environment import Template
 from jinja2.utils import internalcode
-from .loaders import AsyncBaseLoader
+from .compiler import AsyncCodeGenerator
 
 
 class AsyncEnvironment(Environment):
     code_generator_class = AsyncCodeGenerator
-    loader: AsyncBaseLoader = None
-    bytecode_cache: AsyncRedisBytecodeCache = None
-
-    def __init__(self, **env_options) -> None:
-        super().__init__(**env_options)
+    loader: t.Optional[t.Any] = None
+    bytecode_cache: t.Optional[t.Any] = None
 
     @internalcode
     async def get_template(
         self,
-        name: t.Union[str, "Template"],
+        name: str,
         parent: t.Optional[str] = None,
         env_globals: t.Optional[t.MutableMapping[str, t.Any]] = None,
     ) -> "Template":
         if isinstance(name, Template):
             return name
         if parent is not None:
             name = self.join_path(name, parent)
@@ -35,17 +30,15 @@
         self, name: str, env_globals: t.Optional[t.MutableMapping[str, t.Any]]
     ) -> "Template":
         if self.loader is None:
             raise TypeError("no loader for this environment specified")
         cache_key = (ref(self.loader), name)
         if self.cache is not None:
             template = self.cache.get(cache_key)
-            if template is not None and (
-                not self.auto_reload or (await template.is_up_to_date)
-            ):
+            if template and (not self.auto_reload or template.is_up_to_date):
                 if env_globals:
                     template.globals.update(env_globals)
                 return template
         template = await self.loader.load(self, name, self.make_globals(env_globals))
         if self.cache is not None:
             self.cache[cache_key] = template
         return template
```

### Comparing `jinja2_async_environment-0.1.4/jinja2_async_environment/loaders.py` & `jinja2_async_environment-0.1.5/jinja2_async_environment/loaders.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,17 +1,13 @@
 import importlib.util
 import typing as t
 import zipimport
 from collections import abc
 from contextlib import suppress
 from importlib import import_module
-from os import PathLike
-from typing import Any
-from typing import Callable
-from typing import Coroutine
 
 from aiopath import AsyncPath
 from jinja2.environment import Template
 from jinja2.exceptions import TemplateNotFound
 from jinja2.utils import internalcode
 from .environment import AsyncEnvironment
 
@@ -23,284 +19,257 @@
 class LoaderNotFound(TemplateNotFound):
     """Raised if a loader is not found."""
 
 
 class AsyncBaseLoader:
     has_source_access = True
 
-    def __init__(
-        self, searchpath: str | AsyncPath | t.Sequence[str | PathLike]
-    ) -> None:
+    def __init__(self, searchpath: AsyncPath | t.Sequence[AsyncPath]) -> None:
         self.searchpath = searchpath
-        if not isinstance(searchpath, abc.Iterable) or isinstance(searchpath, str):
+        if not isinstance(searchpath, abc.Iterable):
             self.searchpath = [searchpath]
-        self.searchpath = [AsyncPath(p) for p in searchpath]
 
     async def get_source(
-        self, environment: "AsyncEnvironment", template: str | PathLike
-    ) -> t.Tuple[str, t.Optional[str], t.Optional[t.Callable[[], bool]]]:  # type:ignore
-        template = AsyncPath(template)
+        self, environment: "AsyncEnvironment", template: AsyncPath
+    ) -> t.Tuple[
+        str, t.Optional[AsyncPath], t.Optional[t.Callable[[], bool]]
+    ] | t.NoReturn:
         if not self.has_source_access:
             raise RuntimeError(
                 f"{type(self).__name__} cannot provide access to the source"
             )
         raise TemplateNotFound(template.name)
 
-    async def list_templates(self) -> t.List[str]:
+    async def list_templates(self) -> list[str] | t.NoReturn:
         raise TypeError("this loader cannot iterate over all templates")
 
     @internalcode
     async def load(
         self,
         environment: "AsyncEnvironment",
         name: str,
         env_globals: t.Optional[t.MutableMapping[str, t.Any]] = None,
     ) -> "Template":
-        code = None
         if env_globals is None:
             env_globals = {}
-        source, filename, uptodate = await self.get_source(environment, name)
+        code: t.Any = None
+        bucket: t.Any = None
+        source, path, uptodate = await self.get_source(environment, AsyncPath(name))
         bcc = environment.bytecode_cache
-        bucket = None
-        if bcc is not None:
-            bucket = await bcc.get_bucket(environment, name, filename, source)
+        if bcc:
+            bucket = await bcc.get_bucket(environment, name, path, source)
             code = bucket.code
-        if code is None:
-            code = environment.compile(source, name, filename)
-        if bcc is not None and bucket.code is None:
+        if not code:
+            code = environment.compile(source, name, path.name)  # type: ignore
+        if bcc and not bucket.code:
             bucket.code = code
             await bcc.set_bucket(bucket)
         return environment.template_class.from_code(
             environment, code, env_globals, uptodate
         )
 
 
 class FileSystemLoader(AsyncBaseLoader):
     def __init__(
         self,
-        searchpath,
+        searchpath: AsyncPath | t.Sequence[AsyncPath],
         encoding: str = "utf-8",
         followlinks: bool = False,
     ) -> None:
         super().__init__(searchpath)
         self.encoding = encoding
         self.followlinks = followlinks
 
     async def get_source(
-        self, environment: "AsyncEnvironment", template: str
-    ) -> tuple[Any, Any, Callable[[], Coroutine[Any, Any, bool]]]:
+        self, environment: "AsyncEnvironment", template: AsyncPath
+    ) -> tuple[str, AsyncPath, t.Callable | bool]:
         # split_template_path(template)
-        for searchpath in self.searchpath:
-            filename = searchpath / template
-            if filename.is_file():
+        for searchpath in self.searchpath:  # type: ignore
+            path = searchpath / template
+            if await path.is_file():
                 break
         else:
-            raise TemplateNotFound(template)
+            raise TemplateNotFound(template.name)
         try:
-            resp = await filename.read_text()
+            resp = await path.read_text()
         except FileNotFoundError:
-            raise TemplateNotFound(filename.name)
-        mtime = (await filename.stat()).st_mtime
+            raise TemplateNotFound(path.name)
+        mtime = (await path.stat()).st_mtime
 
         async def uptodate() -> bool:
             try:
-                return (await filename.stat()).st_mtime == mtime
+                return (await path.stat()).st_mtime == mtime
             except OSError:
                 return False
 
-        return resp, filename.name, uptodate
+        return resp, path, uptodate
 
     async def list_templates(self) -> list[str]:
         found = set()
-        for searchpath in self.searchpath:
-            found.update(
-                [p.name async for p in searchpath.iterdir() if p.suffix == ".html"]
-            )
+        for searchpath in self.searchpath:  # type: ignore
+            found.update([path.name async for path in searchpath.rglob("*.html")])
         return sorted(found)
 
 
 class PackageLoader(AsyncBaseLoader):
     def __init__(
         self,
         package_name: str,
-        searchpath: AsyncPath,
-        package_path: str | AsyncPath = "templates",
+        searchpath: AsyncPath | t.Sequence[AsyncPath],
+        package_path: AsyncPath = AsyncPath("templates"),
         encoding: str = "utf-8",
     ) -> None:
         super().__init__(searchpath)
-        package_path = AsyncPath(package_path)
         self.package_path = package_path
         self.package_name = package_name
         self.encoding = encoding
         # Make sure the package exists. This also makes namespace
         # packages work, otherwise get_loader returns None.
         import_module(package_name)
         spec = importlib.util.find_spec(package_name)
         if not spec:
-            raise PackageSpecNotFound("An import spec was not found for the package.")
+            raise PackageSpecNotFound("An import spec was not found for the package")
         loader = spec.loader
         if not loader:
-            raise LoaderNotFound("A loader was not found for the package.")
+            raise LoaderNotFound("A loader was not found for the package")
         self._loader = loader
         self._archive = None
         template_root = None
         if isinstance(loader, zipimport.zipimporter):
             self._archive = loader.archive
             pkgdir = next(iter(spec.submodule_search_locations))  # type: ignore
             template_root = AsyncPath(pkgdir) / package_path
         else:
-            roots: t.List[AsyncPath] = []
+            roots = []
             # One element for regular packages, multiple for namespace
             # packages, or None for single module file.
             if spec.submodule_search_locations:
                 roots.extend([AsyncPath(s) for s in spec.submodule_search_locations])
             # A single module file, use the parent directory instead.
             elif spec.origin is not None:
                 roots.append(AsyncPath(spec.origin))
             for root in roots:
-                root = root / package_path
-                if root.is_dir():
+                path = root / package_path
+                if path.is_dir():
                     template_root = root
                     break
 
-        if template_root is None:
+        if not template_root:
             raise ValueError(
                 f"The {package_name!r} package was not installed in a"
-                " way that PackageLoader understands."
+                " way that PackageLoader understands"
             )
 
         self._template_root = template_root
 
     async def get_source(
-        self, environment: "AsyncEnvironment", template: str | AsyncPath
-    ) -> t.Tuple[str, str, t.Optional[t.Callable[[], bool]]]:
-        p = self._template_root / template
-        up_to_date: t.Optional[t.Callable[[], bool]]
-        if self._archive is None:
-            if not p.is_file():
-                raise TemplateNotFound(template)
-            source = await p.read_text()
-            mtime = (await p.stat()).st_mtime
+        self, environment: "AsyncEnvironment", template: AsyncPath
+    ) -> t.Tuple[str, AsyncPath, t.Optional[t.Coroutine[t.Any, t.Any, bool]]]:
+        path = self._template_root / template
+        # up_to_date: t.Optional[t.Callable[[], bool]] | None
+        if self._archive:
+            if not path.is_file():
+                raise TemplateNotFound(path.name)
+            source = await path.read_bytes()
+            mtime = (await path.stat()).st_mtime
 
             async def up_to_date() -> bool:
-                return p.is_file() and (await p.stat()).st_mtime == mtime
+                return await path.is_file() and (await path.stat()).st_mtime == mtime
 
         else:
             # Package is a zip file.
             try:
-                source = self._loader.get_data(p)  # type: ignore
+                source = self._loader.get_data(str(path))  # type: ignore
             except OSError as e:
-                raise TemplateNotFound(template) from e
-            up_to_date = None
-        return source.decode(self.encoding), p, up_to_date
+                raise TemplateNotFound(path.name) from e
+            up_to_date = None  # type: ignore
+        return source.decode(self.encoding), path, up_to_date  # type: ignore
 
-    async def list_templates(self) -> t.List[AsyncPath]:
-        results: t.List[AsyncPath] = []
+    async def list_templates(self) -> list[AsyncPath]:
+        results: list[AsyncPath] = []
 
         if self._archive is None:
             # Package is a directory.
             paths = self._template_root.rglob("*.html")
             results.extend([p async for p in paths])
         else:
             if not hasattr(self._loader, "_files"):
                 raise TypeError(
                     "This zip import does not have the required"
-                    " metadata to list templates."
+                    " metadata to list templates"
                 )
             # Package is a zip file.
             prefix = self._template_root.name
-            for name in self._loader._files.keys():
+            for name in self._loader._files.keys():  # type: ignore
                 # Find names under the templates directory that aren't directories.
-                if name.startswith(prefix) and await AsyncPath(name).is_file():
+                if name.startswith(prefix) and (await AsyncPath(name).is_file()):
                     results.append(name)
         results.sort()
         return results
 
 
 class DictLoader(AsyncBaseLoader):
     def __init__(
         self,
         mapping: t.Mapping[str, str],
-        searchpath: str | AsyncPath | t.Sequence[str | AsyncPath] = None,
+        searchpath: AsyncPath | t.Sequence[AsyncPath],
     ) -> None:
         super().__init__(searchpath)
         self.mapping = mapping
 
     async def get_source(
         self, environment: "AsyncEnvironment", template: str
     ) -> t.Tuple[str, None, t.Callable[[], bool]]:
         if template in self.mapping:
             source = self.mapping[template]
             return source, None, lambda: source == self.mapping.get(template)
         raise TemplateNotFound(template)
 
-    async def list_templates(self) -> t.List[str]:
+    async def list_templates(self) -> list[str]:
         return sorted(self.mapping)
 
 
 class FunctionLoader(AsyncBaseLoader):
     def __init__(
         self,
-        load_func: t.Callable[
-            [t.Coroutine],
-            t.Optional[
-                str
-                | AsyncPath
-                | t.Tuple[str, t.Optional[str]]
-                | t.Optional[t.Callable[[], bool]],
-            ],
-        ],
-        searchpath: str | AsyncPath | t.Sequence[str | AsyncPath] = None,
+        load_func: t.Callable,
+        searchpath: AsyncPath | t.Sequence[AsyncPath],
     ) -> None:
         super().__init__(searchpath)
         self.load_func = load_func
 
     async def get_source(
         self, environment: "AsyncEnvironment", template: str | AsyncPath
-    ) -> t.Tuple[str, t.Optional[str], t.Optional[t.Callable[[], bool]]]:
-        template = AsyncPath(template)
-        rv = await self.load_func(template)
-        if rv is None:
-            raise TemplateNotFound(template.name)
-        if isinstance(rv, str):
-            return rv, None, None
-        return rv
+    ) -> t.Tuple[str, AsyncPath | None, t.Callable | bool | None]:
+        path = AsyncPath(template)
+        source = self.load_func(path)
+        if source is None:
+            raise TemplateNotFound(path.name)
+        if isinstance(source, str):
+            return source, path, True
+        return source
 
 
 class ChoiceLoader(AsyncBaseLoader):
-    loaders: list = []
+    loaders: list[AsyncBaseLoader] = []
 
     def __init__(
         self,
         loaders: list[AsyncBaseLoader],
-        searchpath: str | AsyncPath | t.Sequence[str | AsyncPath] = None,
+        searchpath: AsyncPath | t.Sequence[AsyncPath],
     ) -> None:
         super().__init__(searchpath)
         self.loaders = loaders
 
     async def get_source(
-        self, environment: "AsyncEnvironment", template: str
-    ) -> t.Tuple[str, t.Optional[str], t.Optional[t.Callable[[], bool]]]:
+        self, environment: "AsyncEnvironment", template: AsyncPath
+    ) -> t.Tuple[str, t.Optional[AsyncPath], t.Optional[t.Callable | bool]]:
         for loader in self.loaders:
             with suppress(TemplateNotFound):
                 return await loader.get_source(environment, template)
-        raise TemplateNotFound(template)
+        raise TemplateNotFound(template.name)
 
     async def list_templates(self) -> list[str]:
         found = set()
         for loader in self.loaders:
-            found.update(loader.list_templates())
+            found.update(await loader.list_templates())
         return sorted(found)
-
-    # @internalcode
-    # def load(
-    #     self,
-    #     environment: "AsyncEnvironment",
-    #     name: str,
-    #     globals: t.Optional[t.MutableMapping[str, t.Any]] = None,
-    # ) -> "Template":
-    #     for loader in self.loaders:
-    #         try:
-    #             return loader.load(environment, name, globals)
-    #         except TemplateNotFound:
-    #             pass
-    #     raise TemplateNotFound(name)
```

