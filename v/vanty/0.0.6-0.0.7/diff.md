# Comparing `tmp/vanty-0.0.6.tar.gz` & `tmp/vanty-0.0.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "vanty-0.0.6.tar", max compression
+gzip compressed data, was "vanty-0.0.7.tar", max compression
```

## Comparing `vanty-0.0.6.tar` & `vanty-0.0.7.tar`

### file list

```diff
@@ -1,14 +1,17 @@
--rw-r--r--   0        0        0    11357 2023-05-26 15:47:21.194628 vanty-0.0.6/LICENSE
--rw-r--r--   0        0        0     1246 2023-05-26 17:56:09.814324 vanty-0.0.6/README.md
--rw-r--r--   0        0        0      666 2023-05-28 22:01:28.809277 vanty-0.0.6/pyproject.toml
--rw-r--r--   0        0        0        0 2023-05-26 16:33:35.338956 vanty-0.0.6/vanty/__init__.py
--rw-r--r--   0        0        0      181 2023-05-28 11:37:40.483417 vanty-0.0.6/vanty/__main__.py
--rw-r--r--   0        0        0     2494 2023-05-26 18:06:12.522287 vanty-0.0.6/vanty/_client.py
--rw-r--r--   0        0        0     1194 2023-05-26 18:06:12.531596 vanty-0.0.6/vanty/auth.py
--rw-r--r--   0        0        0      506 2023-05-26 17:53:23.021988 vanty-0.0.6/vanty/cli.py
--rw-r--r--   0        0        0     3737 2023-05-28 22:00:27.024845 vanty-0.0.6/vanty/config.py
--rw-r--r--   0        0        0     3476 2023-05-28 21:57:49.717243 vanty-0.0.6/vanty/dev.py
--rw-r--r--   0        0        0     1842 2023-05-26 16:00:32.579158 vanty-0.0.6/vanty/ops.py
--rw-r--r--   0        0        0      811 2023-05-26 17:53:22.962011 vanty-0.0.6/vanty/project.py
--rw-r--r--   0        0        0      948 2023-05-26 16:00:32.166597 vanty-0.0.6/vanty/schema.py
--rw-r--r--   0        0        0     2100 1970-01-01 00:00:00.000000 vanty-0.0.6/PKG-INFO
+-rw-r--r--   0        0        0    11357 2023-05-26 15:47:21.194628 vanty-0.0.7/LICENSE
+-rw-r--r--   0        0        0     1333 2023-06-12 15:41:08.353566 vanty-0.0.7/README.md
+-rw-r--r--   0        0        0     1924 2023-06-12 15:41:17.061202 vanty-0.0.7/pyproject.toml
+-rw-r--r--   0        0        0        0 2023-05-26 16:33:35.338956 vanty-0.0.7/vanty/__init__.py
+-rw-r--r--   0        0        0      181 2023-05-28 11:37:40.483417 vanty-0.0.7/vanty/__main__.py
+-rw-r--r--   0        0        0     2677 2023-06-12 15:37:15.731208 vanty-0.0.7/vanty/_client.py
+-rw-r--r--   0        0        0     1373 2023-06-12 15:41:08.370865 vanty-0.0.7/vanty/auth.py
+-rw-r--r--   0        0        0      506 2023-05-26 17:53:23.021988 vanty-0.0.7/vanty/cli.py
+-rw-r--r--   0        0        0     3737 2023-05-28 22:00:27.024845 vanty-0.0.7/vanty/config.py
+-rw-r--r--   0        0        0     3483 2023-06-12 15:36:30.548723 vanty-0.0.7/vanty/dev.py
+-rw-r--r--   0        0        0     1566 2023-06-12 15:36:30.449484 vanty-0.0.7/vanty/ops.py
+-rw-r--r--   0        0        0      885 2023-06-12 15:36:30.378656 vanty-0.0.7/vanty/project.py
+-rw-r--r--   0        0        0      951 2023-06-12 15:09:28.698119 vanty-0.0.7/vanty/schema.py
+-rw-r--r--   0        0        0        0 2023-06-12 15:18:24.487437 vanty-0.0.7/vanty/utils/__init__.py
+-rw-r--r--   0        0        0      871 2023-06-12 15:36:30.432585 vanty-0.0.7/vanty/utils/console_printer.py
+-rw-r--r--   0        0        0      221 2023-06-12 15:36:30.363263 vanty-0.0.7/vanty/utils/handlers.py
+-rw-r--r--   0        0        0     2351 1970-01-01 00:00:00.000000 vanty-0.0.7/PKG-INFO
```

### Comparing `vanty-0.0.6/LICENSE` & `vanty-0.0.7/LICENSE`

 * *Files identical despite different names*

### Comparing `vanty-0.0.6/README.md` & `vanty-0.0.7/README.md`

 * *Files 10% similar despite different names*

```diff
@@ -6,32 +6,32 @@
 
    This  Vanty Starter Kit is the fastest way to launch new SaaS & AI products.
 
    Visit https://www.advantch.com/ for documentation and more information
 
 ## Installation
 
-We recommend using pipx to install vanty:
+We recommend using poetry to install vanty:
 
 ```bash
-pipx install vanty
+poetry install vanty
 ```
 
 ## Usage
 
 1. Verify your license:
 
    ```bash
-   vanty verify --license <your-license-id>
+   vanty auth verify <your-license-token>
    ```
 
 2. Download the project to the current directory:
 
    ```bash
-   vanty project download
+   vanty project download --project <project-id>
    ```
 
 3. Get started:
 
    ```bash
    cd <project-name>
    vanty dev init
@@ -45,16 +45,23 @@
 
 ## Issues & Support:
 
 Advantch users can report issues on the slack issue channel.
 
 - https://www.advantch.com/issues/
 
+## Building for pypi
+
+```bash
+poetry build
+poetry publish
+```
+
 ## PRs and Contributions:
 
 Please note that whilst this is open source, it is not intended to be a community project.
 
 Advantch users can submit PRs for extensions etc that maybe helpful to the core project or other users.
 
 Otherwise, please fork and use this as a base for your own projects.
- 
+
 2023 &centerdot; Advantch.
```

### Comparing `vanty-0.0.6/vanty/_client.py` & `vanty-0.0.7/vanty/_client.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,77 +1,82 @@
+from __future__ import annotations
+
 import io
 import zipfile
 
-import httpx
+import requests
 import rich
 
-from vanty.config import config
+from vanty.config import config, logger
 from vanty.schema import DownloadProjectHttpResponse, LicenseVerifiedHttpResponse
 
 
 class Client:
     def _download_zip(self, url: str) -> io.BytesIO:
         """
         Downloads the zip file from the url.
 
         :param url:
         :return:
         """
-        response = httpx.get(url)
+        response = requests.get(url)
         zipped_file = io.BytesIO(response.content)
         return zipped_file
 
-    def verify(self, license_id: str) -> LicenseVerifiedHttpResponse:
+    def verify(self, license_token: str) -> LicenseVerifiedHttpResponse:
         """
         Authenticates the token.
 
         :param token:
         :return:
         """
         server_url = config.get("server_url")
         rich.print(f"Verifying license against [blue]{server_url}[/blue]")
         try:
-            res = httpx.post(
+            res = requests.post(
                 f"{server_url}/projects/authenticate-license/",
-                json={"license_id": license_id},
+                json={"license_token": license_token},
             )
             data = res.json()
-            return LicenseVerifiedHttpResponse(**data)
+            return LicenseVerifiedHttpResponse(**data, license_token=license_token)
         except Exception as e:
-            rich.print(f"[red]Error: {e}[/red]")
+            logger.error(f"Error verifying token: {e}")
             return LicenseVerifiedHttpResponse.error()
 
-    def download(self):
+    def download(self, project_id: str | None = None):
         """
         Gets the project.
         :return:
         """
+
         headers = {"X-API-Token": f"{config.get('token_secret')}"}
         local_folder = config.get("local_folder")
         server_url = config.get("server_url")
 
         rich.print(f"Downloading project from [blue]{server_url}[/blue]")
-        response = httpx.get(f"{server_url}/projects/", headers=headers)
+        response = requests.get(f"{server_url}/projects/download/", headers=headers)
         data = DownloadProjectHttpResponse(**response.json())
 
         if data.is_valid is False or data.profile_status == "inactive":
             rich.print(
-                "[red]Project Download Failed, the link may have expired!\n Please try again.[/red]"
+                "[red]Project Download Failed, the link may have expired!"
+                "\n Please try again.[/red]"
             )
             return
 
         if data.profile_status == "inactive":
             rich.print("[red]Project is no longer active or has expired.[/red]")
             return
 
         # fetch the zip file
-        response = httpx.get(data.url)
+        response = requests.get(data.url)
         if not response.status_code == 200:
             rich.print(
-                "[red]File Download Failed, the link may have expired!\n Please try again.[/red]"
+                "[red]File Download Failed, the link may have expired!\n "
+                "Please try again.[/red]"
             )
             return
 
         # save the zip file
         zipped_file = self._download_zip(data.url)
         with zipfile.ZipFile(zipped_file) as zf:
             zf.extractall(path=local_folder)
```

### Comparing `vanty-0.0.6/vanty/auth.py` & `vanty-0.0.7/vanty/auth.py`

 * *Files 25% similar despite different names*

```diff
@@ -1,37 +1,41 @@
-import getpass
-
 import rich
 import typer
 
 from vanty._client import Client
 from vanty.config import _store_user_config, config, user_config_path
+from vanty.utils.console_printer import vlog
 
 app = typer.Typer(name="auth", help="Manage tokens.", no_args_is_help=True)
 
 
 @app.command(
-    help="Set license id for connecting to advantch.com."
+    help="Set license token for connecting to advantch.com."
     "If not provided with the command, you will be prompted"
     " to enter your credentials."
 )
-def set(
-    license_id: str = typer.Option(prompt=True, help="License id."),
-):
-    if license_id is None:
-        license_id = getpass.getpass("License_id:")
-
+def set(license_token: str):
     server_url = config.get("server_url")
     rich.print(f"Verifying token against [blue]{server_url}[/blue]")
-    data = Client.verify(server_url, license_id)
+    data = Client.verify(server_url, license_token)
     if data.is_valid:
         rich.print("[green]Token verified successfully[/green]")
         _store_user_config(
             {"token_id": data.token_id, "token_secret": data.token_secret}
         )
         rich.print(f"Token written to {user_config_path}")
+        return data.token_id
 
     else:
         rich.print(
-            "[red]Unable to verify invalid[/red]. Please check your license id and try again."
+            "[red]Unable to verify invalid[/red]. "
+            "Please check your license id and try again."
         )
-        rich.print(f"If this problem persists, please contact support@advantch.com")
+        rich.print("If this problem persists, please contact support@advantch.com")
+        return None
+
+
+@app.command(help="Remove the token from the config file.")
+def remove():
+    _store_user_config({"token_id": None, "token_secret": None})
+    vlog.info(f"Token removed from {user_config_path}")
+    return None
```

### Comparing `vanty-0.0.6/vanty/config.py` & `vanty-0.0.7/vanty/config.py`

 * *Files identical despite different names*

### Comparing `vanty-0.0.6/vanty/dev.py` & `vanty-0.0.7/vanty/dev.py`

 * *Files 0% similar despite different names*

```diff
@@ -7,15 +7,16 @@
 from rich import print
 from typer import Typer
 
 from vanty.config import config
 
 app = Typer(
     name="dev",
-    help="Development commands for initializing the project, running the app, run migrations, etc.",
+    help="Development commands for initializing the project,"
+    " running the app, run migrations, etc.",
     no_args_is_help=True,
 )
 
 
 @app.command()
 def docs():
     """Open the docs in browser"""
```

### Comparing `vanty-0.0.6/vanty/project.py` & `vanty-0.0.7/vanty/project.py`

 * *Files 10% similar despite different names*

```diff
@@ -4,27 +4,29 @@
 from vanty._client import Client
 from vanty.config import config
 
 app = typer.Typer(name="project", help="Manage project files", no_args_is_help=True)
 
 
 @app.command(help="Downloads project files from advantch.com.")
-def download():
+def download(project_id=None):
     """
     Download project files from advantch.com.
     :return:
     """
 
     token_id = config.get("token_id")
     if token_id is None:
-        rich.print("[red]Please run `vanty auth set` to set your token.[/red]")
+        rich.print(
+            "[red]Please run `vanty auth set <license-token>` to set your token.[/red]"
+        )
         raise typer.Exit(code=1)
 
     rich.print("[green]Downloading project files...[/green]")
-    Client().download()
+    Client().download(project_id=project_id)
 
 
 @app.command(help="Print current configuration.")
 def print_config():
     """
     Print current configuration.
     :return:
```

### Comparing `vanty-0.0.6/vanty/schema.py` & `vanty-0.0.7/vanty/schema.py`

 * *Files 1% similar despite different names*

```diff
@@ -9,15 +9,15 @@
     ACTIVE = "active"
     INACTIVE = "inactive"
     DELETED = "deleted"
     NOT_FETCHED = "not_fetched"
 
 
 class LicenseVerifiedHttpResponse(BaseModel):
-    license_id: str
+    license_token: str
     token_id: str | None
     token_secret: str | None
     is_valid: bool
 
     @classmethod
     def error(cls):
         return cls(license_id="", token_id="", token_secret="", is_valid=False)
```

### Comparing `vanty-0.0.6/PKG-INFO` & `vanty-0.0.7/PKG-INFO`

 * *Files 9% similar despite different names*

```diff
@@ -1,25 +1,29 @@
 Metadata-Version: 2.1
 Name: vanty
-Version: 0.0.6
+Version: 0.0.7
 Summary: CLI for installing and managing projects & applications from advantch.com
 License: Apache
 Author: Themba
 Author-email: themba@advantch.com
-Requires-Python: >=3.8,<4.0
+Requires-Python: >=3.8.1,<4.0
 Classifier: License :: Other/Proprietary License
 Classifier: Programming Language :: Python :: 3
-Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Requires-Dist: django-environ (>=0.10.0,<0.11.0)
 Requires-Dist: honcho (>=1.1.0,<2.0.0)
 Requires-Dist: httpx (>=0.24.1,<0.25.0)
 Requires-Dist: pydantic (>=1.10.8,<2.0.0)
+Requires-Dist: pytest-mock (>=3.10.0,<4.0.0)
+Requires-Dist: requests (>=2.31.0,<3.0.0)
+Requires-Dist: responses (>=0.23.1,<0.24.0)
+Requires-Dist: respx (>=0.20.1,<0.21.0)
+Requires-Dist: ruff (>=0.0.270,<0.0.271)
 Requires-Dist: sh (>=2.0.4,<3.0.0)
 Requires-Dist: toml (>=0.10.2,<0.11.0)
 Requires-Dist: typer[all] (>=0.9.0,<0.10.0)
 Description-Content-Type: text/markdown
 
 # <img style="margin-right: 2px; margin-top: 10px" alt="logo" height="12" width="12" src="https://cdn.advantch.com/static/images/logo.png"> Vanty CLI
 
@@ -29,32 +33,32 @@
 
    This  Vanty Starter Kit is the fastest way to launch new SaaS & AI products.
 
    Visit https://www.advantch.com/ for documentation and more information
 
 ## Installation
 
-We recommend using pipx to install vanty:
+We recommend using poetry to install vanty:
 
 ```bash
-pipx install vanty
+poetry install vanty
 ```
 
 ## Usage
 
 1. Verify your license:
 
    ```bash
-   vanty verify --license <your-license-id>
+   vanty auth verify <your-license-token>
    ```
 
 2. Download the project to the current directory:
 
    ```bash
-   vanty project download
+   vanty project download --project <project-id>
    ```
 
 3. Get started:
 
    ```bash
    cd <project-name>
    vanty dev init
@@ -68,17 +72,24 @@
 
 ## Issues & Support:
 
 Advantch users can report issues on the slack issue channel.
 
 - https://www.advantch.com/issues/
 
+## Building for pypi
+
+```bash
+poetry build
+poetry publish
+```
+
 ## PRs and Contributions:
 
 Please note that whilst this is open source, it is not intended to be a community project.
 
 Advantch users can submit PRs for extensions etc that maybe helpful to the core project or other users.
 
 Otherwise, please fork and use this as a base for your own projects.
- 
+
 2023 &centerdot; Advantch.
```

