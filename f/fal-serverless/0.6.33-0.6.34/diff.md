# Comparing `tmp/fal_serverless-0.6.33.tar.gz` & `tmp/fal_serverless-0.6.34.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "fal_serverless-0.6.33.tar", max compression
+gzip compressed data, was "fal_serverless-0.6.34.tar", max compression
```

## Comparing `fal_serverless-0.6.33.tar` & `fal_serverless-0.6.34.tar`

### file list

```diff
@@ -1,27 +1,27 @@
--rw-r--r--   0        0        0      213 2023-06-01 14:31:42.566849 fal_serverless-0.6.33/README.md
--rw-r--r--   0        0        0      998 2023-06-01 14:32:00.095054 fal_serverless-0.6.33/pyproject.toml
--rw-r--r--   0        0        0      335 2023-06-01 14:31:42.570849 fal_serverless-0.6.33/src/fal_serverless/__init__.py
--rw-r--r--   0        0        0    17363 2023-06-01 14:31:42.570849 fal_serverless-0.6.33/src/fal_serverless/api.py
--rw-r--r--   0        0        0     2593 2023-06-01 14:31:42.570849 fal_serverless-0.6.33/src/fal_serverless/auth/__init__.py
--rw-r--r--   0        0        0     5426 2023-06-01 14:31:42.570849 fal_serverless-0.6.33/src/fal_serverless/auth/auth0.py
--rw-r--r--   0        0        0     1786 2023-06-01 14:31:42.570849 fal_serverless-0.6.33/src/fal_serverless/auth/local.py
--rw-r--r--   0        0        0    15759 2023-06-01 14:31:42.570849 fal_serverless-0.6.33/src/fal_serverless/cli.py
--rw-r--r--   0        0        0      132 2023-06-01 14:31:42.570849 fal_serverless-0.6.33/src/fal_serverless/console/__init__.py
--rw-r--r--   0        0        0      108 2023-06-01 14:31:42.570849 fal_serverless-0.6.33/src/fal_serverless/console/icons.py
--rw-r--r--   0        0        0      485 2023-06-01 14:31:42.570849 fal_serverless-0.6.33/src/fal_serverless/console/ux.py
--rw-r--r--   0        0        0      172 2023-06-01 14:31:53.702972 fal_serverless-0.6.33/src/fal_serverless/env.py
--rw-r--r--   0        0        0      938 2023-06-01 14:31:42.570849 fal_serverless-0.6.33/src/fal_serverless/exceptions/__init__.py
--rw-r--r--   0        0        0      412 2023-06-01 14:31:42.570849 fal_serverless-0.6.33/src/fal_serverless/exceptions/_base.py
--rw-r--r--   0        0        0      353 2023-06-01 14:31:42.570849 fal_serverless-0.6.33/src/fal_serverless/exceptions/auth.py
--rw-r--r--   0        0        0     1435 2023-06-01 14:31:42.570849 fal_serverless-0.6.33/src/fal_serverless/exceptions/handlers.py
--rw-r--r--   0        0        0      326 2023-06-01 14:31:42.570849 fal_serverless-0.6.33/src/fal_serverless/flags.py
--rw-r--r--   0        0        0     1649 2023-06-01 14:31:42.570849 fal_serverless-0.6.33/src/fal_serverless/logging/__init__.py
--rw-r--r--   0        0        0     2574 2023-06-01 14:31:42.570849 fal_serverless-0.6.33/src/fal_serverless/logging/datadog.py
--rw-r--r--   0        0        0     2122 2023-06-01 14:31:42.570849 fal_serverless-0.6.33/src/fal_serverless/logging/isolate.py
--rw-r--r--   0        0        0      386 2023-06-01 14:31:42.570849 fal_serverless-0.6.33/src/fal_serverless/logging/style.py
--rw-r--r--   0        0        0     1785 2023-06-01 14:31:42.570849 fal_serverless-0.6.33/src/fal_serverless/logging/trace.py
--rw-r--r--   0        0        0      643 2023-06-01 14:31:42.570849 fal_serverless-0.6.33/src/fal_serverless/logging/user.py
--rw-r--r--   0        0        0    15875 2023-06-01 14:31:42.570849 fal_serverless-0.6.33/src/fal_serverless/sdk.py
--rw-r--r--   0        0        0     5335 2023-06-01 14:31:42.570849 fal_serverless-0.6.33/src/fal_serverless/sync.py
--rw-r--r--   0        0        0     1773 1970-01-01 00:00:00.000000 fal_serverless-0.6.33/setup.py
--rw-r--r--   0        0        0     1603 1970-01-01 00:00:00.000000 fal_serverless-0.6.33/PKG-INFO
+-rw-r--r--   0        0        0      213 2023-06-12 16:47:30.829636 fal_serverless-0.6.34/README.md
+-rw-r--r--   0        0        0     1006 2023-06-12 16:47:53.626225 fal_serverless-0.6.34/pyproject.toml
+-rw-r--r--   0        0        0      335 2023-06-12 16:47:30.829636 fal_serverless-0.6.34/src/fal_serverless/__init__.py
+-rw-r--r--   0        0        0    17568 2023-06-12 16:47:30.829636 fal_serverless-0.6.34/src/fal_serverless/api.py
+-rw-r--r--   0        0        0     2593 2023-06-12 16:47:30.829636 fal_serverless-0.6.34/src/fal_serverless/auth/__init__.py
+-rw-r--r--   0        0        0     5426 2023-06-12 16:47:30.829636 fal_serverless-0.6.34/src/fal_serverless/auth/auth0.py
+-rw-r--r--   0        0        0     1786 2023-06-12 16:47:30.829636 fal_serverless-0.6.34/src/fal_serverless/auth/local.py
+-rw-r--r--   0        0        0    15633 2023-06-12 16:47:30.829636 fal_serverless-0.6.34/src/fal_serverless/cli.py
+-rw-r--r--   0        0        0      132 2023-06-12 16:47:30.829636 fal_serverless-0.6.34/src/fal_serverless/console/__init__.py
+-rw-r--r--   0        0        0      108 2023-06-12 16:47:30.829636 fal_serverless-0.6.34/src/fal_serverless/console/icons.py
+-rw-r--r--   0        0        0      485 2023-06-12 16:47:30.829636 fal_serverless-0.6.34/src/fal_serverless/console/ux.py
+-rw-r--r--   0        0        0      172 2023-06-12 16:47:45.242028 fal_serverless-0.6.34/src/fal_serverless/env.py
+-rw-r--r--   0        0        0      938 2023-06-12 16:47:30.829636 fal_serverless-0.6.34/src/fal_serverless/exceptions/__init__.py
+-rw-r--r--   0        0        0      412 2023-06-12 16:47:30.829636 fal_serverless-0.6.34/src/fal_serverless/exceptions/_base.py
+-rw-r--r--   0        0        0      353 2023-06-12 16:47:30.829636 fal_serverless-0.6.34/src/fal_serverless/exceptions/auth.py
+-rw-r--r--   0        0        0     1435 2023-06-12 16:47:30.829636 fal_serverless-0.6.34/src/fal_serverless/exceptions/handlers.py
+-rw-r--r--   0        0        0      326 2023-06-12 16:47:30.829636 fal_serverless-0.6.34/src/fal_serverless/flags.py
+-rw-r--r--   0        0        0     1649 2023-06-12 16:47:30.829636 fal_serverless-0.6.34/src/fal_serverless/logging/__init__.py
+-rw-r--r--   0        0        0     2574 2023-06-12 16:47:30.829636 fal_serverless-0.6.34/src/fal_serverless/logging/datadog.py
+-rw-r--r--   0        0        0     2122 2023-06-12 16:47:30.829636 fal_serverless-0.6.34/src/fal_serverless/logging/isolate.py
+-rw-r--r--   0        0        0      386 2023-06-12 16:47:30.829636 fal_serverless-0.6.34/src/fal_serverless/logging/style.py
+-rw-r--r--   0        0        0     1785 2023-06-12 16:47:30.829636 fal_serverless-0.6.34/src/fal_serverless/logging/trace.py
+-rw-r--r--   0        0        0      643 2023-06-12 16:47:30.829636 fal_serverless-0.6.34/src/fal_serverless/logging/user.py
+-rw-r--r--   0        0        0    16029 2023-06-12 16:47:30.829636 fal_serverless-0.6.34/src/fal_serverless/sdk.py
+-rw-r--r--   0        0        0     6533 2023-06-12 16:47:30.829636 fal_serverless-0.6.34/src/fal_serverless/sync.py
+-rw-r--r--   0        0        0     1778 1970-01-01 00:00:00.000000 fal_serverless-0.6.34/setup.py
+-rw-r--r--   0        0        0     1608 1970-01-01 00:00:00.000000 fal_serverless-0.6.34/PKG-INFO
```

### Comparing `fal_serverless-0.6.33/pyproject.toml` & `fal_serverless-0.6.34/pyproject.toml`

 * *Files 10% similar despite different names*

```diff
@@ -1,22 +1,22 @@
 [tool.poetry]
 name = "fal_serverless"
-version = "0.6.33"
+version = "0.6.34"
 description = "fal Serverless is an easy-to-use Serverless Python Framework"
 authors = ["Features & Labels <hello@fal.ai>"]
 readme = "README.md"
 
 [tool.poetry.dependencies]
 python = "^3.7"
 auth0-python = "^4.1.0"
 requests = "^2.28.1"
-isolate = {version = "0.12.0", extras = ["build"]}
+isolate = {version = ">=0.12.2, <1.0", extras = ["build"]}
 grpcio = "^1.50.0"
 dill = "0.3.5.1"
-isolate-proto = "^0.0.28"
+isolate-proto = "^0.0.30"
 typing-extensions = "4.4"
 click = "^8.1.3"
 structlog = "^22.3.0"
 datadog-api-client = "2.12.0"
 opentelemetry-api = "^1.15.0"
 opentelemetry-sdk = "^1.15.0"
 grpc-interceptor = "^0.15.0"
```

### Comparing `fal_serverless-0.6.33/src/fal_serverless/api.py` & `fal_serverless-0.6.34/src/fal_serverless/api.py`

 * *Files 3% similar despite different names*

```diff
@@ -204,15 +204,15 @@
                         "This is likely due to resource overflow. "
                         "You can try again by setting a bigger `machine_type`"
                     )
 
                 elif e.code() == grpc.StatusCode.INVALID_ARGUMENT and (
                     "The function function could not be deserialized" in e.details()
                 ):
-                    raise FalMissingDependencyError(e.details())
+                    raise FalMissingDependencyError(e.details()) from None
                 else:
                     raise FalServerlessError(e.details())
 
         return handler
 
     return decorator
 
@@ -251,15 +251,17 @@
             continue
         yield module_name, used_names
 
 
 # TODO: Should we build all these in fal/dbt-fal packages instead?
 @dataclass
 class FalServerlessHost(Host):
-    _SUPPORTED_KEYS = frozenset({"machine_type", "keep_alive", "setup_function"})
+    _SUPPORTED_KEYS = frozenset(
+        {"machine_type", "keep_alive", "setup_function", "_base_image"}
+    )
 
     url: str = FAL_SERVERLESS_DEFAULT_URL
     credentials: Credentials = field(default_factory=get_default_credentials)
     _lock: threading.Lock = field(default_factory=threading.Lock)
 
     _log_printer = IsolateLogPrinter(debug=bool_envvar("DEBUG"))
 
@@ -285,17 +287,20 @@
         environment_options.setdefault("python_version", active_python())
         environments = [self._connection.define_environment(**environment_options)]
 
         machine_type = options.host.get(
             "machine_type", FAL_SERVERLESS_DEFAULT_MACHINE_TYPE
         )
         keep_alive = options.host.get("keep_alive", FAL_SERVERLESS_DEFAULT_KEEP_ALIVE)
+        base_image = options.host.get("_base_image", None)
 
         machine_requirements = MachineRequirements(
-            machine_type=machine_type, keep_alive=keep_alive
+            machine_type=machine_type,
+            keep_alive=keep_alive,
+            base_image=base_image,
         )
 
         partial_func = _execution_controller(func, tuple(), {})
 
         for partial_result in self._connection.register(
             partial_func,
             environments,
@@ -329,18 +334,21 @@
         environment_options.setdefault("python_version", active_python())
         environments = [self._connection.define_environment(**environment_options)]
 
         machine_type = options.host.get(
             "machine_type", FAL_SERVERLESS_DEFAULT_MACHINE_TYPE
         )
         keep_alive = options.host.get("keep_alive", FAL_SERVERLESS_DEFAULT_KEEP_ALIVE)
+        base_image = options.host.get("_base_image", None)
         setup_function = options.host.get("setup_function", None)
 
         machine_requirements = MachineRequirements(
-            machine_type=machine_type, keep_alive=keep_alive
+            machine_type=machine_type,
+            keep_alive=keep_alive,
+            base_image=base_image,
         )
 
         return_value = _UNSET
         # Allow isolate provided arguments (such as setup function) to take
         # precedence over the ones provided by the user.
         partial_func = _execution_controller(func, args, kwargs)
         for partial_result in self._connection.run(
@@ -488,24 +496,23 @@
             pairs = list(find_missing_dependencies(self.func, self.options.environment))
             if not pairs:
                 raise e
             else:
                 lines = []
                 for used_modules, references in pairs:
                     lines.append(
-                        f"    - {used_modules} (as referred by {', '.join(references)})"
+                        f"\t- {used_modules!r} (accessed through {', '.join(map(repr, references))})"
                     )
 
+                function_name = self.func.__name__
                 raise FalServerlessError(
-                    "A deserialization error regarding your function has occurred. \nHint: This might be "
-                    " because the following modules are referenced but not required as part of your environment "
-                    "declaration:\n"
+                    f"Couldn't deserialize your function on the remote server. \n\n[Hint] {function_name!r} "
+                    f"function uses the following modules which weren't present in the environment definition:\n"
                     + "\n".join(lines)
-                    + "\ntry adding them to the requirements of your isolated function"
-                )
+                ) from None
 
     def on(self, host: Host | None = None, **config: Any) -> IsolatedFunction[ReturnT]:
         host = host or self.host
         if isinstance(host, type(self.host)):
             previous_host_options = self.options.host
         else:
             previous_host_options = {}
```

### Comparing `fal_serverless-0.6.33/src/fal_serverless/auth/__init__.py` & `fal_serverless-0.6.34/src/fal_serverless/auth/__init__.py`

 * *Files identical despite different names*

### Comparing `fal_serverless-0.6.33/src/fal_serverless/auth/auth0.py` & `fal_serverless-0.6.34/src/fal_serverless/auth/auth0.py`

 * *Files identical despite different names*

### Comparing `fal_serverless-0.6.33/src/fal_serverless/auth/local.py` & `fal_serverless-0.6.34/src/fal_serverless/auth/local.py`

 * *Files identical despite different names*

### Comparing `fal_serverless-0.6.33/src/fal_serverless/cli.py` & `fal_serverless-0.6.34/src/fal_serverless/cli.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,25 +1,23 @@
 from __future__ import annotations
 
-import datetime
-import operator
 from sys import argv
 from typing import Literal
 from uuid import uuid4
 
 import click
 import fal_serverless.auth as auth
 import grpc
 from fal_serverless import api, sdk
 from fal_serverless.console import console
 from fal_serverless.exceptions import ApplicationExceptionHandler
 from fal_serverless.logging import get_logger, set_debug_logging
 from fal_serverless.logging.isolate import IsolateLogPrinter
 from fal_serverless.logging.trace import get_tracer
-from fal_serverless.sync import list_children, parse_logs
+from fal_serverless.sync import get_latest_logs
 from rich.table import Table
 
 DEFAULT_HOST = "api.alpha.fal.ai"
 HOST_ENVVAR = "FAL_HOST"
 
 DEFAULT_PORT = "443"
 PORT_ENVVAR = "FAL_PORT"
@@ -297,14 +295,15 @@
         options=isolated_function.options,
         application_name=alias,
         application_is_public=auth_mode == "public",
     )
     if id:
         # TODO: should we centralize this URL format?
         gateway_host = host.url.replace("api.", "gateway.")
+        gateway_host = remove_http_and_port_from_url(gateway_host)
 
         # Encode since user_id can contain special characters
         user_id = auth.USER.info["sub"].split("|")[1]
         if alias:
             console.print(
                 f"Registered a new revision for function '{alias}' (revision='{id}')."
             )
@@ -331,38 +330,27 @@
         func=isolated_function.func, cron=cron_string, options=isolated_function.options
     )
     if cron_id:
         console.print(cron_id)
 
 
 @function_cli.command("logs")
-@click.argument("url", required=True)
-@click.argument("call_id", required=True)
+@click.option("--lines", default=100)
+@click.option("--url", default=None)
 @click.pass_obj
-def get_logs(host: api.FalServerlessHost, url: str, call_id: str):
-    logs = parse_logs(f"/data/logs/gateway/{url}/{call_id}")
+def get_logs(host: api.FalServerlessHost, lines: int | None, url: str | None):
+    if url:
+        url = remove_http_and_port_from_url(url)
+    latest_logs = get_latest_logs(lines, url)
+    latest_logs.reverse()
     log_printer = IsolateLogPrinter(debug=True)
-    for log in logs:
+    for log in latest_logs:
         log_printer.print_dict(log)
 
 
-@function_cli.command("calls")
-@click.argument("url", required=True)
-@click.pass_obj
-def get_function_call_ids(host: api.FalServerlessHost, url: str):
-    # This will only return a list calls that we have logs for.
-    calls = list_children(f"/data/logs/gateway/{url}")
-    calls.sort(key=operator.itemgetter("updated_time"))
-    for call in calls:
-        name = call["name"].split(".")[0]
-        timestamp = datetime.datetime.fromtimestamp(call["updated_time"])
-        timestamp_str = timestamp.strftime("%Y-%m-%d %H:%M:%S.%f")[:-3]
-        console.print(f"{timestamp_str}: {name}")
-
-
 ##### Alias group #####
 @click.group
 @click.option("--host", default=DEFAULT_HOST, envvar=HOST_ENVVAR)
 @click.option("--port", default=DEFAULT_PORT, envvar=PORT_ENVVAR, hidden=True)
 @click.pass_context
 def alias_cli(ctx, host: str, port: str):
     ctx.obj = api.FalServerlessClient(f"{host}:{port}")
@@ -499,9 +487,26 @@
 cli.add_command(function_cli, name="function", aliases=["fn"])
 cli.add_command(alias_cli, name="alias")
 cli.add_command(crons_cli, name="cron", aliases=["crons"])
 cli.add_command(usage_cli, name="usage")
 cli.add_command(secrets_cli, name="secret", aliases=["secrets"])
 
 
+def remove_http_and_port_from_url(url):
+    # Remove http://
+    if "http://" in url:
+        url = url.replace("http://", "")
+
+    # Remove https://
+    if "https://" in url:
+        url = url.replace("https://", "")
+
+    # Remove port information
+    url_parts = url.split(":")
+    if len(url_parts) > 1:
+        url = url_parts[0]
+
+    return url
+
+
 if __name__ == "__main__":
     cli()
```

### Comparing `fal_serverless-0.6.33/src/fal_serverless/exceptions/__init__.py` & `fal_serverless-0.6.34/src/fal_serverless/exceptions/__init__.py`

 * *Files identical despite different names*

### Comparing `fal_serverless-0.6.33/src/fal_serverless/exceptions/handlers.py` & `fal_serverless-0.6.34/src/fal_serverless/exceptions/handlers.py`

 * *Files identical despite different names*

### Comparing `fal_serverless-0.6.33/src/fal_serverless/logging/__init__.py` & `fal_serverless-0.6.34/src/fal_serverless/logging/__init__.py`

 * *Files identical despite different names*

### Comparing `fal_serverless-0.6.33/src/fal_serverless/logging/datadog.py` & `fal_serverless-0.6.34/src/fal_serverless/logging/datadog.py`

 * *Files identical despite different names*

### Comparing `fal_serverless-0.6.33/src/fal_serverless/logging/isolate.py` & `fal_serverless-0.6.34/src/fal_serverless/logging/isolate.py`

 * *Files identical despite different names*

### Comparing `fal_serverless-0.6.33/src/fal_serverless/logging/trace.py` & `fal_serverless-0.6.34/src/fal_serverless/logging/trace.py`

 * *Files identical despite different names*

### Comparing `fal_serverless-0.6.33/src/fal_serverless/logging/user.py` & `fal_serverless-0.6.34/src/fal_serverless/logging/user.py`

 * *Files identical despite different names*

### Comparing `fal_serverless-0.6.33/src/fal_serverless/sdk.py` & `fal_serverless-0.6.34/src/fal_serverless/sdk.py`

 * *Files 2% similar despite different names*

```diff
@@ -301,14 +301,15 @@
         return run
 
 
 @dataclass
 class MachineRequirements:
     machine_type: str
     keep_alive: int = FAL_SERVERLESS_DEFAULT_KEEP_ALIVE
+    base_image: str | None = None
 
 
 @dataclass
 class FalServerlessConnection:
     hostname: str
     credentials: Credentials
 
@@ -394,14 +395,15 @@
         machine_requirements: MachineRequirements | None = None,
     ) -> Iterator[isolate_proto.RegisterApplicationResult]:
         wrapped_function = to_serialized_object(function, serialization_method)
         if machine_requirements:
             wrapped_requirements = isolate_proto.MachineRequirements(
                 machine_type=machine_requirements.machine_type,
                 keep_alive=machine_requirements.keep_alive,
+                base_image=machine_requirements.base_image,
             )
         else:
             wrapped_requirements = None
 
         request = isolate_proto.RegisterApplicationRequest(
             function=wrapped_function,
             environments=environments,
@@ -422,14 +424,15 @@
         setup_function: Callable[[], InputT] | None = None,
     ) -> Iterator[HostedRunResult[ResultT]]:
         wrapped_function = to_serialized_object(function, serialization_method)
         if machine_requirements:
             wrapped_requirements = isolate_proto.MachineRequirements(
                 machine_type=machine_requirements.machine_type,
                 keep_alive=machine_requirements.keep_alive,
+                base_image=machine_requirements.base_image,
             )
         else:
             wrapped_requirements = None
 
         request = isolate_proto.HostedRun(
             function=wrapped_function,
             environments=environments,
```

### Comparing `fal_serverless-0.6.33/src/fal_serverless/sync.py` & `fal_serverless-0.6.34/src/fal_serverless/sync.py`

 * *Files 12% similar despite different names*

```diff
@@ -46,48 +46,82 @@
 def _clear_destination_file(destination_path):
     os.makedirs("/data/sync", exist_ok=True)
     with open(destination_path, "wb") as f:
         f.truncate(0)
 
 
 @isolated()
-def list_children(parent_directory: str) -> list[dict]:
-    items: list[dict] = []
+def get_latest_logs(n: int = 100, endpoint_url: str | None = None) -> Any:
+    import os
+
+    def list_children(parent_directory: str) -> list[dict]:
+        items: list[dict] = []
+
+        if not os.path.exists(parent_directory):
+            return items
+
+        for file_name in os.listdir(parent_directory):
+            file_path = os.path.join(parent_directory, file_name)
+
+            created_time = os.path.getctime(file_path)
+            updated_time = os.path.getmtime(file_path)
+
+            items.append(
+                {
+                    "name": file_name,
+                    "created_time": created_time,
+                    "updated_time": updated_time,
+                    "is_file": os.path.isfile(file_path),
+                }
+            )
 
-    if not os.path.exists(parent_directory):
         return items
 
-    for file_name in os.listdir(parent_directory):
-        file_path = os.path.join(parent_directory, file_name)
+    def parse_logs(file_path: str) -> Any:
+        import json
 
-        created_time = os.path.getctime(file_path)
-        updated_time = os.path.getmtime(file_path)
+        if os.path.exists(file_path):
+            with open(file_path) as f:
+                lines = f.readlines()
+                parsed = [json.loads(line) for line in lines]
+                return [log for sub in parsed for log in sub]
+        return []
 
-        items.append(
-            {
-                "name": file_name,
-                "created_time": created_time,
-                "updated_time": updated_time,
-                "is_file": os.path.isfile(file_path),
-            }
-        )
+    # Get all the URLs as directory names inside /data/logs/gateway/
+    urls = list_children("/data/logs/gateway/")
 
-    return items
+    all_logs = []
 
+    for url in urls:
+        url_name = url["name"]
+        if endpoint_url and url_name != endpoint_url:
+            continue
 
-@isolated()
-def parse_logs(file_path: str) -> Any:
-    import json
+        # Get all function call_ids for each URL
+        calls = list_children(f"/data/logs/gateway/{url_name}")
+
+        for call in calls:
+            call_id = call["name"].split(".")[0]
+
+            # Get logs associated with each call_id
+            logs = parse_logs(f"/data/logs/gateway/{url_name}/{call_id}")
+
+            # Add timestamp and URL name to logs for formatting
+            for log in logs:
+                log["message"] = f"[{url_name}] {log['message']}"
+
+            all_logs.extend(logs)
+
+    # Sort logs based on timestamp
+    sorted_logs = sorted(all_logs, key=lambda x: x["timestamp"], reverse=True)
+
+    # Limit the logs by the specified number of lines (default: 100)
+    latest_logs = sorted_logs[:n]
 
-    if os.path.exists(file_path):
-        with open(file_path) as f:
-            lines = f.readlines()
-            parsed = [json.loads(line) for line in lines]
-            return [log for sub in parsed for log in sub]
-    return []
+    return latest_logs
 
 
 def _upload_file(source_path: str, destination_path: str) -> None:
     file_size = os.path.getsize(source_path)
     total_chunks = (file_size // CHUNK_SIZE) + (1 if file_size % CHUNK_SIZE else 0)
 
     # Clear the destination file
```

### Comparing `fal_serverless-0.6.33/setup.py` & `fal_serverless-0.6.34/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -18,16 +18,16 @@
 ['auth0-python>=4.1.0,<5.0.0',
  'click>=8.1.3,<9.0.0',
  'colorama>=0.4.6,<0.5.0',
  'datadog-api-client==2.12.0',
  'dill==0.3.5.1',
  'grpc-interceptor>=0.15.0,<0.16.0',
  'grpcio>=1.50.0,<2.0.0',
- 'isolate-proto>=0.0.28,<0.0.29',
- 'isolate[build]==0.12.0',
+ 'isolate-proto>=0.0.30,<0.0.31',
+ 'isolate[build]>=0.12.2,<1.0',
  'opentelemetry-api>=1.15.0,<2.0.0',
  'opentelemetry-sdk>=1.15.0,<2.0.0',
  'packaging>=21.3',
  'pathspec>=0.11.1,<0.12.0',
  'portalocker>=2.7.0,<3.0.0',
  'requests>=2.28.1,<3.0.0',
  'rich>=13.3.2,<14.0.0',
@@ -38,15 +38,15 @@
 {':python_version < "3.10"': ['importlib-metadata>=4.4']}
 
 entry_points = \
 {'console_scripts': ['fal-serverless = fal_serverless.cli:cli']}
 
 setup_kwargs = {
     'name': 'fal-serverless',
-    'version': '0.6.33',
+    'version': '0.6.34',
     'description': 'fal Serverless is an easy-to-use Serverless Python Framework',
     'long_description': '# fal-serverless\n\nLibrary to run, serve or schedule your Python functions in the cloud with any machine type you may need.\n\nCheck out to the [docs](https://docs.fal.ai/fal-serverless/quickstart) for more details.\n',
     'author': 'Features & Labels',
     'author_email': 'hello@fal.ai',
     'maintainer': 'None',
     'maintainer_email': 'None',
     'url': 'None',
```

### Comparing `fal_serverless-0.6.33/PKG-INFO` & `fal_serverless-0.6.34/PKG-INFO`

 * *Files 9% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: fal-serverless
-Version: 0.6.33
+Version: 0.6.34
 Summary: fal Serverless is an easy-to-use Serverless Python Framework
 Author: Features & Labels
 Author-email: hello@fal.ai
 Requires-Python: >=3.7,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
@@ -15,16 +15,16 @@
 Requires-Dist: click (>=8.1.3,<9.0.0)
 Requires-Dist: colorama (>=0.4.6,<0.5.0)
 Requires-Dist: datadog-api-client (==2.12.0)
 Requires-Dist: dill (==0.3.5.1)
 Requires-Dist: grpc-interceptor (>=0.15.0,<0.16.0)
 Requires-Dist: grpcio (>=1.50.0,<2.0.0)
 Requires-Dist: importlib-metadata (>=4.4) ; python_version < "3.10"
-Requires-Dist: isolate-proto (>=0.0.28,<0.0.29)
-Requires-Dist: isolate[build] (==0.12.0)
+Requires-Dist: isolate-proto (>=0.0.30,<0.0.31)
+Requires-Dist: isolate[build] (>=0.12.2,<1.0)
 Requires-Dist: opentelemetry-api (>=1.15.0,<2.0.0)
 Requires-Dist: opentelemetry-sdk (>=1.15.0,<2.0.0)
 Requires-Dist: packaging (>=21.3)
 Requires-Dist: pathspec (>=0.11.1,<0.12.0)
 Requires-Dist: portalocker (>=2.7.0,<3.0.0)
 Requires-Dist: requests (>=2.28.1,<3.0.0)
 Requires-Dist: rich (>=13.3.2,<14.0.0)
```

