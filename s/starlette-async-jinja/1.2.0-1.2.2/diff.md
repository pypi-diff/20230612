# Comparing `tmp/starlette_async_jinja-1.2.0.tar.gz` & `tmp/starlette_async_jinja-1.2.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "starlette_async_jinja-1.2.0.tar", last modified: Fri May 19 14:47:00 2023, max compression
+gzip compressed data, was "starlette_async_jinja-1.2.2.tar", last modified: Sun Jun 11 23:49:39 2023, max compression
```

## Comparing `starlette_async_jinja-1.2.0.tar` & `starlette_async_jinja-1.2.2.tar`

### file list

```diff
@@ -1,5 +1,5 @@
--rw-r--r--   0        0        0      282 2023-04-26 14:31:29.295695 starlette_async_jinja-1.2.0/README.md
--rw-r--r--   0        0        0     1169 2023-05-19 14:47:00.917189 starlette_async_jinja-1.2.0/pyproject.toml
--rw-r--r--   0        0        0       85 2023-05-19 13:51:11.189835 starlette_async_jinja-1.2.0/starlette_async_jinja/__init__.py
--rw-r--r--   0        0        0     5994 2023-05-19 13:43:09.701695 starlette_async_jinja-1.2.0/starlette_async_jinja/responses.py
--rw-r--r--   0        0        0      823 1970-01-01 00:00:00.000000 starlette_async_jinja-1.2.0/PKG-INFO
+-rw-r--r--   0        0        0      592 2023-06-11 12:03:51.211467 starlette_async_jinja-1.2.2/README.md
+-rw-r--r--   0        0        0     1188 2023-06-11 23:49:39.424545 starlette_async_jinja-1.2.2/pyproject.toml
+-rw-r--r--   0        0        0      211 2023-06-11 12:03:37.580220 starlette_async_jinja-1.2.2/starlette_async_jinja/__init__.py
+-rw-r--r--   0        0        0     6035 2023-06-11 23:48:44.601334 starlette_async_jinja-1.2.2/starlette_async_jinja/responses.py
+-rw-r--r--   0        0        0     1133 1970-01-01 00:00:00.000000 starlette_async_jinja-1.2.2/PKG-INFO
```

### Comparing `starlette_async_jinja-1.2.0/pyproject.toml` & `starlette_async_jinja-1.2.2/pyproject.toml`

 * *Files 12% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 [tool.pdm.dev-dependencies]
 dev = [
     "pre-commit>=3.2.2",
-    "Crackerjack @ file:///${PROJECT_ROOT}/../crackerjack",
+    "crackerjack>=0.2.13",
 ]
 
 [tool.ruff]
 line-length = 88
 target-version = "py311"
 fix = true
 show-fixes = true
@@ -21,34 +21,33 @@
 convention = "google"
 
 [tool.black]
 target-version = [
     "py311",
 ]
 
-[tool.mypy]
-strict = true
-pretty = true
-
 [tool.refurb]
 enable_all = true
 
-[tool.pytype]
-inputs = [
-    "package_name",
+[tool.pyright]
+include = [
+    "starlette_async_jinja",
 ]
+reportMissingImports = true
+reportMissingTypeStubs = false
+pythonVersion = "3.11"
 
 [project]
 name = "starlette-async-jinja"
-version = "1.2.0"
+version = "1.2.2"
 description = ""
 dependencies = [
-    "starlette>=0.26.1",
+    "starlette>=0.28.0",
     "jinja2>=3.1.2",
-    "jinja2-async-environment>=0.1.1",
+    "jinja2-async-environment>=0.1.6",
 ]
 requires-python = ">=3.11"
 readme = "README.md"
 authors = [
     { name = "lesleslie", email = "les@wedgwoodwebworks.com" },
 ]
```

### Comparing `starlette_async_jinja-1.2.0/starlette_async_jinja/responses.py` & `starlette_async_jinja-1.2.2/starlette_async_jinja/responses.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,11 +1,11 @@
-import os
 import typing as t
 from functools import partial
 
+from aiopath import AsyncPath
 from jinja2.environment import Template
 from jinja2_async_environment import AsyncEnvironment
 from jinja2_async_environment import FileSystemLoader
 from markupsafe import Markup
 from msgspec import json
 from starlette.background import BackgroundTask
 from starlette.requests import Request
@@ -62,28 +62,46 @@
             )
         await super().__call__(scope, receive, send)
 
 
 class AsyncJinja2Templates(Jinja2Templates):
     def __init__(
         self,
-        directory: str | os.PathLike,
+        directory: AsyncPath,
         context_processors: t.Optional[
             t.List[t.Callable[[Request], t.Dict[str, t.Any]]]
         ] = None,
         **env_options: t.Any,
     ) -> None:
         super().__init__(directory, **env_options)
         self.env_options = env_options
         self.context_processors = context_processors or []
         self.env = self._create_env(directory, **env_options)
 
+    def _create_env(
+        self, directory: AsyncPath, **env_options: dict[str, str] | bool
+    ) -> "AsyncEnvironment":
+        @pass_context
+        def url_for(
+            context: dict[str, t.Any], name: str, **path_params: dict[str, str | bool]
+        ) -> str:
+            request = context["request"]
+            return request.url_for(name, **path_params)
+
+        loader = FileSystemLoader(directory)
+        env_options.setdefault("loader", loader)  # type: ignore
+        env_options.setdefault("autoescape", True)
+        env = AsyncEnvironment(**env_options)
+        env.globals["render_partial"] = self.generate_render_partial(self.renderer)
+        env.globals["url_for"] = url_for
+        return env
+
     # Partials - https://github.com/mikeckennedy/jinja_partials
+    @staticmethod
     async def render_partial(
-        self,
         template_name: str,
         renderer: t.Optional[t.Callable[..., t.Any]] = None,
         **data: t.Any,
     ) -> Markup:
         return Markup(await renderer(template_name, **data))
 
     def generate_render_partial(
@@ -91,15 +109,15 @@
     ) -> t.Callable[..., Markup]:
         return partial(self.render_partial, renderer=renderer)
 
     async def renderer(self, template_name: str, **data: t.Any) -> str:
         return await (await self.get_template(template_name)).render_async(**data)
 
     # Fragments - https://github.com/sponsfreixes/jinja2-fragments
-    async def render_block_async(
+    async def render_block(
         self,
         template: "Template",
         block_name: str,
         *args: t.Any,
         **kwargs: t.Any,
     ) -> str:
         try:
@@ -111,32 +129,14 @@
         try:
             return self.env.concat(  # type: ignore
                 [n async for n in block_render_func(ctx)]  # type: ignore
             )
         except Exception:
             return self.env.handle_exception()
 
-    def _create_env(
-        self, directory: str | os.PathLike, **env_options: dict[str, str] | bool
-    ) -> "AsyncEnvironment":
-        @pass_context
-        def url_for(
-            context: dict[str, t.Any], name: str, **path_params: dict[str, str | bool]
-        ) -> str:
-            request = context["request"]
-            return request.url_for(name, **path_params)
-
-        loader = FileSystemLoader(directory)
-        env_options.setdefault("loader", loader)  # type: ignore
-        env_options.setdefault("autoescape", True)
-        env = AsyncEnvironment(**env_options)
-        env.globals["render_partial"] = self.generate_render_partial(self.renderer)
-        env.globals["url_for"] = url_for
-        return env
-
     async def get_template(self, name: str) -> "Template":
         return await self.env.get_template(name)
 
     async def AsyncTemplateResponse(
         self,
         name: str,
         context: dict[str, str],
@@ -151,15 +151,15 @@
             raise ValueError('context must include a "request" key')
         request = t.cast(Request, context["request"])
         for context_processor in self.context_processors:
             context.update(context_processor(request))
         template = await self.get_template(name)
 
         if block_name:
-            return await self.render_block_async(
+            return await self.render_block(
                 template,
                 block_name,
                 context,
             )
 
         content = await template.render_async(context)
         return _AsyncTemplateResponse(
@@ -167,7 +167,9 @@
             context,
             content,
             status_code=status_code,
             headers=headers,
             media_type=media_type,
             background=background,
         )
+
+    render_template = AsyncTemplateResponse
```

