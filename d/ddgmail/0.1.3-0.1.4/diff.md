# Comparing `tmp/ddgmail-0.1.3.tar.gz` & `tmp/ddgmail-0.1.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ddgmail-0.1.3.tar", last modified: Mon Jun 12 18:43:00 2023, max compression
+gzip compressed data, was "ddgmail-0.1.4.tar", last modified: Mon Jun 12 19:02:19 2023, max compression
```

## Comparing `ddgmail-0.1.3.tar` & `ddgmail-0.1.4.tar`

### file list

```diff
@@ -1,17 +1,17 @@
-drwxrwxr-x   0 user      (1000) user      (1000)        0 2023-06-12 18:43:00.698792 ddgmail-0.1.3/
--rw-rw-r--   0 user      (1000) user      (1000)     3078 2023-06-12 15:21:01.000000 ddgmail-0.1.3/.gitignore
--rw-rw-r--   0 user      (1000) user      (1000)    20623 2023-06-12 17:51:04.000000 ddgmail-0.1.3/.pylintrc
--rw-------   0 user      (1000) user      (1000)    35149 2023-06-12 11:39:18.000000 ddgmail-0.1.3/LICENSE
--rw-rw-r--   0 user      (1000) user      (1000)      220 2023-06-12 12:07:16.000000 ddgmail-0.1.3/Makefile
--rw-rw-r--   0 user      (1000) user      (1000)      454 2023-06-12 18:43:00.698792 ddgmail-0.1.3/PKG-INFO
--rwx------   0 user      (1000) user      (1000)      136 2023-06-12 15:37:51.000000 ddgmail-0.1.3/build_and_publish.sh
-drwxrwxr-x   0 user      (1000) user      (1000)        0 2023-06-12 18:43:00.698792 ddgmail-0.1.3/ddgmail.egg-info/
--rw-rw-r--   0 user      (1000) user      (1000)      454 2023-06-12 18:43:00.000000 ddgmail-0.1.3/ddgmail.egg-info/PKG-INFO
--rw-rw-r--   0 user      (1000) user      (1000)      266 2023-06-12 18:43:00.000000 ddgmail-0.1.3/ddgmail.egg-info/SOURCES.txt
--rw-rw-r--   0 user      (1000) user      (1000)        1 2023-06-12 18:43:00.000000 ddgmail-0.1.3/ddgmail.egg-info/dependency_links.txt
--rw-rw-r--   0 user      (1000) user      (1000)       41 2023-06-12 18:43:00.000000 ddgmail-0.1.3/ddgmail.egg-info/entry_points.txt
--rw-rw-r--   0 user      (1000) user      (1000)       25 2023-06-12 18:43:00.000000 ddgmail-0.1.3/ddgmail.egg-info/requires.txt
--rw-rw-r--   0 user      (1000) user      (1000)        8 2023-06-12 18:43:00.000000 ddgmail-0.1.3/ddgmail.egg-info/top_level.txt
--rw-rw-r--   0 user      (1000) user      (1000)     5407 2023-06-12 18:41:00.000000 ddgmail-0.1.3/ddgmail.py
--rw-rw-r--   0 user      (1000) user      (1000)       38 2023-06-12 18:43:00.698792 ddgmail-0.1.3/setup.cfg
--rw-rw-r--   0 user      (1000) user      (1000)     1126 2023-06-12 18:41:38.000000 ddgmail-0.1.3/setup.py
+drwxrwxr-x   0 user      (1000) user      (1000)        0 2023-06-12 19:02:19.721877 ddgmail-0.1.4/
+-rw-rw-r--   0 user      (1000) user      (1000)     3078 2023-06-12 15:21:01.000000 ddgmail-0.1.4/.gitignore
+-rw-rw-r--   0 user      (1000) user      (1000)    20623 2023-06-12 17:51:04.000000 ddgmail-0.1.4/.pylintrc
+-rw-------   0 user      (1000) user      (1000)    35149 2023-06-12 11:39:18.000000 ddgmail-0.1.4/LICENSE
+-rw-rw-r--   0 user      (1000) user      (1000)      220 2023-06-12 12:07:16.000000 ddgmail-0.1.4/Makefile
+-rw-rw-r--   0 user      (1000) user      (1000)      454 2023-06-12 19:02:19.721877 ddgmail-0.1.4/PKG-INFO
+-rwx------   0 user      (1000) user      (1000)      136 2023-06-12 15:37:51.000000 ddgmail-0.1.4/build_and_publish.sh
+drwxrwxr-x   0 user      (1000) user      (1000)        0 2023-06-12 19:02:19.721877 ddgmail-0.1.4/ddgmail.egg-info/
+-rw-rw-r--   0 user      (1000) user      (1000)      454 2023-06-12 19:02:19.000000 ddgmail-0.1.4/ddgmail.egg-info/PKG-INFO
+-rw-rw-r--   0 user      (1000) user      (1000)      266 2023-06-12 19:02:19.000000 ddgmail-0.1.4/ddgmail.egg-info/SOURCES.txt
+-rw-rw-r--   0 user      (1000) user      (1000)        1 2023-06-12 19:02:19.000000 ddgmail-0.1.4/ddgmail.egg-info/dependency_links.txt
+-rw-rw-r--   0 user      (1000) user      (1000)       41 2023-06-12 19:02:19.000000 ddgmail-0.1.4/ddgmail.egg-info/entry_points.txt
+-rw-rw-r--   0 user      (1000) user      (1000)       25 2023-06-12 19:02:19.000000 ddgmail-0.1.4/ddgmail.egg-info/requires.txt
+-rw-rw-r--   0 user      (1000) user      (1000)        8 2023-06-12 19:02:19.000000 ddgmail-0.1.4/ddgmail.egg-info/top_level.txt
+-rwxrwxr-x   0 user      (1000) user      (1000)     5356 2023-06-12 19:01:31.000000 ddgmail-0.1.4/ddgmail.py
+-rw-rw-r--   0 user      (1000) user      (1000)       38 2023-06-12 19:02:19.721877 ddgmail-0.1.4/setup.cfg
+-rw-rw-r--   0 user      (1000) user      (1000)     1126 2023-06-12 19:02:14.000000 ddgmail-0.1.4/setup.py
```

### Comparing `ddgmail-0.1.3/.gitignore` & `ddgmail-0.1.4/.gitignore`

 * *Files identical despite different names*

### Comparing `ddgmail-0.1.3/.pylintrc` & `ddgmail-0.1.4/.pylintrc`

 * *Files identical despite different names*

### Comparing `ddgmail-0.1.3/LICENSE` & `ddgmail-0.1.4/LICENSE`

 * *Files identical despite different names*

### Comparing `ddgmail-0.1.3/ddgmail.py` & `ddgmail-0.1.4/ddgmail.py`

 * *Files 6% similar despite different names*

```diff
@@ -8,15 +8,15 @@
 import requests
 
 BASE_URL = "https://quack.duckduckgo.com/api/"
 BASE_HEADERS = {
     "User-Agent": "Mozilla/5.0 (X11; Linux x86_64; rv:109.0) Gecko/20100101 Firefox/114.0",
     "Accept": "*/*",
     "Accept-Language": "en-US,en;q=0.5",
-#    "Accept-Encoding": "gzip, deflate, br",
+    # "Accept-Encoding": "gzip, deflate, br",
     "Referer": "https://duckduckgo.com/",
     "DNT": "1",
     "Connection": "keep-alive",
     "Sec-Fetch-Dest": "empty",
     "Sec-Fetch-Site": "same-site",
     "Sec-Fetch-Mode": "cors",
     "Sec-GPC": "1",
@@ -32,30 +32,30 @@
 config_file = os.path.join(config_dir, "config.json")
 
 
 def load_config():
     config = None
 
     if os.path.exists(config_file):
-        with open(config_file, encoding='utf-8') as fobj:
+        with open(config_file, encoding="utf-8") as fobj:
             config = json.load(fobj)
 
     if (
         not config
         or not config.get("user")
         or not config.get("token")
         or not config.get("access_token")
     ):
         raise click.ClickException("Login first")
 
     return config
 
 
 def save_config(config):
-    with open(config_file, "w", encoding='utf-8') as fobj:
+    with open(config_file, "w", encoding="utf-8") as fobj:
         json.dump(config, fobj)
 
 
 @click.group()
 def cli():
     pass
 
@@ -104,14 +104,18 @@
     data = response.json()
     config["access_token"] = data["user"]["access_token"]
     # write to config
     save_config(config)
     click.echo("Login successful")
 
 
+def row_string_fmt(row1: str, row2: str, size: int):
+    return f"{row1:>{size}} | {row2:<{size}}"
+
+
 @cli.command()
 @click.pass_context
 def dashboard(ctx: click.Context, tries=0):
     """Show dashboard information"""
     config = load_config()
     response = session.get(
         BASE_URL + "email/dashboard",
@@ -122,33 +126,25 @@
             ctx.invoke(request_otp, username=config["user"])
             ctx.invoke(login, username=config["user"], otp=None)
             ctx.invoke(dashboard, tries=tries + 1)
             return
         raise click.ClickException("Retry threshold exceeded")
     response.raise_for_status()
     data = response.json()
-    mapping = {
-        "stats": {
-            "addresses_generated": "Addresses Generated",
-        },
-        "user": {
-            "email": "Forwarding Email",
-        },
-    }
-    for section, section_data in data.items():
-        if section in mapping:
-            for key, value in section_data.items():
-                if key in mapping[section]:
-                    click.echo(f"{mapping[section][key]}: {value}")
+    click.echo(row_string_fmt("Duck Address", f"{config['user']}@duck.com", 20))
+    click.echo(row_string_fmt("Forwarding Address", data["user"]["email"], 20))
+    click.echo(
+        row_string_fmt("Addresses Generated", data["stats"]["addresses_generated"], 20)
+    )
 
 
 @cli.command()
 @click.argument("email")
 @click.pass_context
-def change_forwarding_email(ctx: click.Context, email, tries = 0):
+def change_forwarding_email(ctx: click.Context, email, tries=0):
     """Change forwarding email"""
     config = load_config()
     data = {"email": email, "disable_secure_reply": 0}
     response = session.post(
         BASE_URL + "email/change-email-address",
         headers={"Authorization": f"Bearer {config['token']}"},
         data=data,
```

### Comparing `ddgmail-0.1.3/setup.py` & `ddgmail-0.1.4/setup.py`

 * *Files 10% similar despite different names*

```diff
@@ -6,19 +6,19 @@
 # This conditional isn't necessary, but it provides better error messages to
 # people who try to install this package with older versions of setuptools.
 if parse_version(setuptools_version) < parse_version(min_setuptools_version):
     raise RuntimeError(f"setuptools {min_setuptools_version}+ is required")
 
 setup(
     name="ddgmail",
-    version="0.1.3",
+    version="0.1.4",
     py_modules=["ddgmail"],
-    author='rany',
-    author_email='ranygh@riseup.net',
-    url='https://github.com/rany2/ddgmail',
+    author="rany",
+    author_email="ranygh@riseup.net",
+    url="https://github.com/rany2/ddgmail",
     description="A command line tool to use DuckDuckGo's E-mail forwarding service",
     install_requires=[
         "Click",
         f"setuptools>={min_setuptools_version}",
     ],
     entry_points={
         "console_scripts": [
```

