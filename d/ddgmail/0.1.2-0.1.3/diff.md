# Comparing `tmp/ddgmail-0.1.2.tar.gz` & `tmp/ddgmail-0.1.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ddgmail-0.1.2.tar", last modified: Mon Jun 12 16:35:12 2023, max compression
+gzip compressed data, was "ddgmail-0.1.3.tar", last modified: Mon Jun 12 18:43:00 2023, max compression
```

## Comparing `ddgmail-0.1.2.tar` & `ddgmail-0.1.3.tar`

### file list

```diff
@@ -1,16 +1,17 @@
-drwxrwxr-x   0 user      (1000) user      (1000)        0 2023-06-12 16:35:12.514848 ddgmail-0.1.2/
--rw-rw-r--   0 user      (1000) user      (1000)     3078 2023-06-12 15:21:01.000000 ddgmail-0.1.2/.gitignore
--rw-------   0 user      (1000) user      (1000)    35149 2023-06-12 11:39:18.000000 ddgmail-0.1.2/LICENSE
--rw-rw-r--   0 user      (1000) user      (1000)      220 2023-06-12 12:07:16.000000 ddgmail-0.1.2/Makefile
--rw-rw-r--   0 user      (1000) user      (1000)      454 2023-06-12 16:35:12.514848 ddgmail-0.1.2/PKG-INFO
--rwx------   0 user      (1000) user      (1000)      136 2023-06-12 15:37:51.000000 ddgmail-0.1.2/build_and_publish.sh
-drwxrwxr-x   0 user      (1000) user      (1000)        0 2023-06-12 16:35:12.514848 ddgmail-0.1.2/ddgmail.egg-info/
--rw-rw-r--   0 user      (1000) user      (1000)      454 2023-06-12 16:35:12.000000 ddgmail-0.1.2/ddgmail.egg-info/PKG-INFO
--rw-rw-r--   0 user      (1000) user      (1000)      256 2023-06-12 16:35:12.000000 ddgmail-0.1.2/ddgmail.egg-info/SOURCES.txt
--rw-rw-r--   0 user      (1000) user      (1000)        1 2023-06-12 16:35:12.000000 ddgmail-0.1.2/ddgmail.egg-info/dependency_links.txt
--rw-rw-r--   0 user      (1000) user      (1000)       41 2023-06-12 16:35:12.000000 ddgmail-0.1.2/ddgmail.egg-info/entry_points.txt
--rw-rw-r--   0 user      (1000) user      (1000)       25 2023-06-12 16:35:12.000000 ddgmail-0.1.2/ddgmail.egg-info/requires.txt
--rw-rw-r--   0 user      (1000) user      (1000)        8 2023-06-12 16:35:12.000000 ddgmail-0.1.2/ddgmail.egg-info/top_level.txt
--rw-rw-r--   0 user      (1000) user      (1000)     4174 2023-06-12 16:32:33.000000 ddgmail-0.1.2/ddgmail.py
--rw-rw-r--   0 user      (1000) user      (1000)       38 2023-06-12 16:35:12.514848 ddgmail-0.1.2/setup.cfg
--rw-rw-r--   0 user      (1000) user      (1000)     1126 2023-06-12 16:32:43.000000 ddgmail-0.1.2/setup.py
+drwxrwxr-x   0 user      (1000) user      (1000)        0 2023-06-12 18:43:00.698792 ddgmail-0.1.3/
+-rw-rw-r--   0 user      (1000) user      (1000)     3078 2023-06-12 15:21:01.000000 ddgmail-0.1.3/.gitignore
+-rw-rw-r--   0 user      (1000) user      (1000)    20623 2023-06-12 17:51:04.000000 ddgmail-0.1.3/.pylintrc
+-rw-------   0 user      (1000) user      (1000)    35149 2023-06-12 11:39:18.000000 ddgmail-0.1.3/LICENSE
+-rw-rw-r--   0 user      (1000) user      (1000)      220 2023-06-12 12:07:16.000000 ddgmail-0.1.3/Makefile
+-rw-rw-r--   0 user      (1000) user      (1000)      454 2023-06-12 18:43:00.698792 ddgmail-0.1.3/PKG-INFO
+-rwx------   0 user      (1000) user      (1000)      136 2023-06-12 15:37:51.000000 ddgmail-0.1.3/build_and_publish.sh
+drwxrwxr-x   0 user      (1000) user      (1000)        0 2023-06-12 18:43:00.698792 ddgmail-0.1.3/ddgmail.egg-info/
+-rw-rw-r--   0 user      (1000) user      (1000)      454 2023-06-12 18:43:00.000000 ddgmail-0.1.3/ddgmail.egg-info/PKG-INFO
+-rw-rw-r--   0 user      (1000) user      (1000)      266 2023-06-12 18:43:00.000000 ddgmail-0.1.3/ddgmail.egg-info/SOURCES.txt
+-rw-rw-r--   0 user      (1000) user      (1000)        1 2023-06-12 18:43:00.000000 ddgmail-0.1.3/ddgmail.egg-info/dependency_links.txt
+-rw-rw-r--   0 user      (1000) user      (1000)       41 2023-06-12 18:43:00.000000 ddgmail-0.1.3/ddgmail.egg-info/entry_points.txt
+-rw-rw-r--   0 user      (1000) user      (1000)       25 2023-06-12 18:43:00.000000 ddgmail-0.1.3/ddgmail.egg-info/requires.txt
+-rw-rw-r--   0 user      (1000) user      (1000)        8 2023-06-12 18:43:00.000000 ddgmail-0.1.3/ddgmail.egg-info/top_level.txt
+-rw-rw-r--   0 user      (1000) user      (1000)     5407 2023-06-12 18:41:00.000000 ddgmail-0.1.3/ddgmail.py
+-rw-rw-r--   0 user      (1000) user      (1000)       38 2023-06-12 18:43:00.698792 ddgmail-0.1.3/setup.cfg
+-rw-rw-r--   0 user      (1000) user      (1000)     1126 2023-06-12 18:41:38.000000 ddgmail-0.1.3/setup.py
```

### Comparing `ddgmail-0.1.2/.gitignore` & `ddgmail-0.1.3/.gitignore`

 * *Files identical despite different names*

### Comparing `ddgmail-0.1.2/LICENSE` & `ddgmail-0.1.3/LICENSE`

 * *Files identical despite different names*

### Comparing `ddgmail-0.1.2/ddgmail.py` & `ddgmail-0.1.3/ddgmail.py`

 * *Files 18% similar despite different names*

```diff
@@ -32,31 +32,31 @@
 config_file = os.path.join(config_dir, "config.json")
 
 
 def load_config():
     config = None
 
     if os.path.exists(config_file):
-        with open(config_file) as f:
-            config = json.load(f)
+        with open(config_file, encoding='utf-8') as fobj:
+            config = json.load(fobj)
 
     if (
         not config
         or not config.get("user")
         or not config.get("token")
         or not config.get("access_token")
     ):
         raise click.ClickException("Login first")
 
     return config
 
 
 def save_config(config):
-    with open(config_file, "w") as f:
-        json.dump(config, f)
+    with open(config_file, "w", encoding='utf-8') as fobj:
+        json.dump(config, fobj)
 
 
 @click.group()
 def cli():
     pass
 
 
@@ -67,24 +67,34 @@
     response = session.get(BASE_URL + "auth/loginlink", params={"user": username})
     response.raise_for_status()
     click.echo("Please check your inbox for the magic password!")
 
 
 @cli.command()
 @click.argument("username")
-def login(username, otp=None):
+@click.pass_context
+def login(ctx: click.Context, username, otp=None, tries=0):
     """Login to the account with OTP"""
     while not otp:
         otp = click.prompt("Enter the magic password", type=str)
 
     config = {}
     response = session.get(
         BASE_URL + "auth/login", params={"user": username, "otp": otp}
     )
-    response.raise_for_status()
+    try:
+        response.raise_for_status()
+    except requests.exceptions.HTTPError as e:
+        if e.response.status_code == 401:
+            if tries < 3:
+                click.echo("Invalid magic password", err=True)
+                ctx.invoke(login, username=username, otp=None, tries=tries + 1)
+                return
+            raise click.ClickException("Retry threshold exceeded")
+        raise e
     data = response.json()
     if data["status"] != "authenticated":
         raise click.ClickException("Login failed")
     config["user"] = username
     config["token"] = data["token"]
     response = session.get(
         BASE_URL + "email/dashboard",
@@ -95,21 +105,29 @@
     config["access_token"] = data["user"]["access_token"]
     # write to config
     save_config(config)
     click.echo("Login successful")
 
 
 @cli.command()
-def dashboard():
+@click.pass_context
+def dashboard(ctx: click.Context, tries=0):
     """Show dashboard information"""
     config = load_config()
     response = session.get(
         BASE_URL + "email/dashboard",
         headers={"Authorization": f"Bearer {config['token']}"},
     )
+    if response.status_code == 401:
+        if tries < 3:
+            ctx.invoke(request_otp, username=config["user"])
+            ctx.invoke(login, username=config["user"], otp=None)
+            ctx.invoke(dashboard, tries=tries + 1)
+            return
+        raise click.ClickException("Retry threshold exceeded")
     response.raise_for_status()
     data = response.json()
     mapping = {
         "stats": {
             "addresses_generated": "Addresses Generated",
         },
         "user": {
@@ -121,23 +139,31 @@
             for key, value in section_data.items():
                 if key in mapping[section]:
                     click.echo(f"{mapping[section][key]}: {value}")
 
 
 @cli.command()
 @click.argument("email")
-def change_forwarding_email(email):
+@click.pass_context
+def change_forwarding_email(ctx: click.Context, email, tries = 0):
     """Change forwarding email"""
     config = load_config()
     data = {"email": email, "disable_secure_reply": 0}
     response = session.post(
         BASE_URL + "email/change-email-address",
         headers={"Authorization": f"Bearer {config['token']}"},
         data=data,
     )
+    if response.status_code == 401:
+        if tries < 3:
+            ctx.invoke(request_otp, username=config["user"])
+            ctx.invoke(login, username=config["user"], otp=None)
+            ctx.invoke(change_forwarding_email, email=email, tries=tries + 1)
+            return
+        raise click.ClickException("Retry threshold exceeded")
     response.raise_for_status()
     click.echo("Forwarding email changed")
 
 
 @cli.command()
 def generate_new_alias():
     """Generates a new E-Mail alias"""
```

### Comparing `ddgmail-0.1.2/setup.py` & `ddgmail-0.1.3/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -6,15 +6,15 @@
 # This conditional isn't necessary, but it provides better error messages to
 # people who try to install this package with older versions of setuptools.
 if parse_version(setuptools_version) < parse_version(min_setuptools_version):
     raise RuntimeError(f"setuptools {min_setuptools_version}+ is required")
 
 setup(
     name="ddgmail",
-    version="0.1.2",
+    version="0.1.3",
     py_modules=["ddgmail"],
     author='rany',
     author_email='ranygh@riseup.net',
     url='https://github.com/rany2/ddgmail',
     description="A command line tool to use DuckDuckGo's E-mail forwarding service",
     install_requires=[
         "Click",
```

