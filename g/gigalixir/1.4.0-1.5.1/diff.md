# Comparing `tmp/gigalixir-1.4.0.tar.gz` & `tmp/gigalixir-1.5.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "gigalixir-1.4.0.tar", last modified: Thu Mar 16 02:59:43 2023, max compression
+gzip compressed data, was "gigalixir-1.5.1.tar", last modified: Mon Jun 12 14:23:45 2023, max compression
```

## Comparing `gigalixir-1.4.0.tar` & `gigalixir-1.5.1.tar`

### file list

```diff
@@ -1,51 +1,51 @@
-drwxrwxr-x   0 tim       (1001) tim       (1001)        0 2023-03-16 02:59:43.901723 gigalixir-1.4.0/
--rw-rw-r--   0 tim       (1001) tim       (1001)     1081 2022-12-06 04:22:54.000000 gigalixir-1.4.0/LICENSE
--rw-rw-r--   0 tim       (1001) tim       (1001)      269 2023-03-16 02:59:43.901723 gigalixir-1.4.0/PKG-INFO
--rw-rw-r--   0 tim       (1001) tim       (1001)     1470 2022-12-06 04:22:54.000000 gigalixir-1.4.0/README.md
-drwxrwxr-x   0 tim       (1001) tim       (1001)        0 2023-03-16 02:59:43.901723 gigalixir-1.4.0/gigalixir/
--rw-rw-r--   0 tim       (1001) tim       (1001)    40590 2023-03-16 02:46:36.000000 gigalixir-1.4.0/gigalixir/__init__.py
--rw-rw-r--   0 tim       (1001) tim       (1001)      229 2022-01-04 16:13:56.000000 gigalixir-1.4.0/gigalixir/api_exception.py
--rw-rw-r--   0 tim       (1001) tim       (1001)      858 2022-01-04 16:13:56.000000 gigalixir-1.4.0/gigalixir/api_key.py
--rw-rw-r--   0 tim       (1001) tim       (1001)    10135 2022-09-09 11:05:48.000000 gigalixir-1.4.0/gigalixir/app.py
--rw-rw-r--   0 tim       (1001) tim       (1001)      538 2022-01-04 16:13:56.000000 gigalixir-1.4.0/gigalixir/app_activity.py
--rw-rw-r--   0 tim       (1001) tim       (1001)      391 2022-01-04 16:13:56.000000 gigalixir-1.4.0/gigalixir/auth.py
--rw-rw-r--   0 tim       (1001) tim       (1001)     1560 2022-01-04 16:13:56.000000 gigalixir-1.4.0/gigalixir/canary.py
--rw-rw-r--   0 tim       (1001) tim       (1001)     2385 2022-01-04 16:13:56.000000 gigalixir-1.4.0/gigalixir/config.py
--rw-rw-r--   0 tim       (1001) tim       (1001)     4082 2022-01-04 16:13:56.000000 gigalixir-1.4.0/gigalixir/database.py
--rw-rw-r--   0 tim       (1001) tim       (1001)     1633 2022-01-04 16:13:56.000000 gigalixir-1.4.0/gigalixir/domain.py
--rw-rw-r--   0 tim       (1001) tim       (1001)     1336 2022-01-04 16:13:56.000000 gigalixir-1.4.0/gigalixir/free_database.py
--rw-rw-r--   0 tim       (1001) tim       (1001)      601 2022-01-04 16:13:56.000000 gigalixir-1.4.0/gigalixir/git.py
--rw-rw-r--   0 tim       (1001) tim       (1001)      446 2022-01-04 16:13:56.000000 gigalixir-1.4.0/gigalixir/invoice.py
--rw-rw-r--   0 tim       (1001) tim       (1001)     1262 2022-01-04 16:13:56.000000 gigalixir-1.4.0/gigalixir/log_drain.py
--rw-rw-r--   0 tim       (1001) tim       (1001)     2653 2022-01-04 16:13:56.000000 gigalixir-1.4.0/gigalixir/mfa.py
--rw-rw-r--   0 tim       (1001) tim       (1001)     3084 2022-01-04 16:13:56.000000 gigalixir-1.4.0/gigalixir/netrc.py
--rw-rw-r--   0 tim       (1001) tim       (1001)     7045 2022-01-04 16:13:56.000000 gigalixir-1.4.0/gigalixir/observer.py
-drwxrwxr-x   0 tim       (1001) tim       (1001)        0 2023-03-16 02:59:43.901723 gigalixir-1.4.0/gigalixir/openers/
--rw-rw-r--   0 tim       (1001) tim       (1001)        0 2022-01-04 16:13:56.000000 gigalixir-1.4.0/gigalixir/openers/__init__.py
--rw-rw-r--   0 tim       (1001) tim       (1001)      207 2022-01-04 16:13:56.000000 gigalixir-1.4.0/gigalixir/openers/darwin.py
--rw-rw-r--   0 tim       (1001) tim       (1001)      214 2022-01-04 16:13:56.000000 gigalixir-1.4.0/gigalixir/openers/linux.py
--rw-rw-r--   0 tim       (1001) tim       (1001)      210 2022-01-04 16:13:56.000000 gigalixir-1.4.0/gigalixir/openers/windows.py
--rw-rw-r--   0 tim       (1001) tim       (1001)     1172 2022-01-18 14:21:12.000000 gigalixir-1.4.0/gigalixir/payment_method.py
--rw-rw-r--   0 tim       (1001) tim       (1001)     1274 2022-01-04 16:13:56.000000 gigalixir-1.4.0/gigalixir/permission.py
--rw-rw-r--   0 tim       (1001) tim       (1001)      347 2022-01-04 16:13:56.000000 gigalixir-1.4.0/gigalixir/presenter.py
--rw-rw-r--   0 tim       (1001) tim       (1001)      538 2022-01-04 16:13:56.000000 gigalixir-1.4.0/gigalixir/release.py
-drwxrwxr-x   0 tim       (1001) tim       (1001)        0 2023-03-16 02:59:43.901723 gigalixir-1.4.0/gigalixir/routers/
--rw-rw-r--   0 tim       (1001) tim       (1001)        0 2022-01-04 16:13:56.000000 gigalixir-1.4.0/gigalixir/routers/__init__.py
--rw-rw-r--   0 tim       (1001) tim       (1001)     1551 2022-01-04 16:13:56.000000 gigalixir-1.4.0/gigalixir/routers/darwin.py
--rw-rw-r--   0 tim       (1001) tim       (1001)      902 2022-01-04 16:13:56.000000 gigalixir-1.4.0/gigalixir/routers/linux.py
--rw-rw-r--   0 tim       (1001) tim       (1001)      618 2022-01-04 16:13:56.000000 gigalixir-1.4.0/gigalixir/routers/windows.py
--rw-rw-r--   0 tim       (1001) tim       (1001)     1490 2022-01-04 16:13:56.000000 gigalixir-1.4.0/gigalixir/shell.py
--rw-rw-r--   0 tim       (1001) tim       (1001)     1234 2022-01-04 16:13:56.000000 gigalixir-1.4.0/gigalixir/ssh_key.py
--rw-rw-r--   0 tim       (1001) tim       (1001)      801 2022-08-20 15:11:07.000000 gigalixir-1.4.0/gigalixir/usage.py
--rw-rw-r--   0 tim       (1001) tim       (1001)     7549 2023-03-16 02:46:36.000000 gigalixir-1.4.0/gigalixir/user.py
-drwxrwxr-x   0 tim       (1001) tim       (1001)        0 2023-03-16 02:59:43.901723 gigalixir-1.4.0/gigalixir.egg-info/
--rw-rw-r--   0 tim       (1001) tim       (1001)      269 2023-03-16 02:59:43.000000 gigalixir-1.4.0/gigalixir.egg-info/PKG-INFO
--rw-rw-r--   0 tim       (1001) tim       (1001)     1019 2023-03-16 02:59:43.000000 gigalixir-1.4.0/gigalixir.egg-info/SOURCES.txt
--rw-rw-r--   0 tim       (1001) tim       (1001)        1 2023-03-16 02:59:43.000000 gigalixir-1.4.0/gigalixir.egg-info/dependency_links.txt
--rw-rw-r--   0 tim       (1001) tim       (1001)       63 2023-03-16 02:59:43.000000 gigalixir-1.4.0/gigalixir.egg-info/entry_points.txt
--rw-rw-r--   0 tim       (1001) tim       (1001)      187 2023-03-16 02:59:43.000000 gigalixir-1.4.0/gigalixir.egg-info/requires.txt
--rw-rw-r--   0 tim       (1001) tim       (1001)       10 2023-03-16 02:59:43.000000 gigalixir-1.4.0/gigalixir.egg-info/top_level.txt
--rw-rw-r--   0 tim       (1001) tim       (1001)       63 2023-03-16 02:59:43.901723 gigalixir-1.4.0/setup.cfg
--rw-rw-r--   0 tim       (1001) tim       (1001)      959 2023-03-16 02:46:36.000000 gigalixir-1.4.0/setup.py
-drwxrwxr-x   0 tim       (1001) tim       (1001)        0 2023-03-16 02:59:43.901723 gigalixir-1.4.0/test/
--rw-rw-r--   0 tim       (1001) tim       (1001)    36261 2022-01-27 06:29:24.000000 gigalixir-1.4.0/test/test_gigalixir.py
+drwxrwxr-x   0 tim       (1001) tim       (1001)        0 2023-06-12 14:23:45.311078 gigalixir-1.5.1/
+-rw-rw-r--   0 tim       (1001) tim       (1001)     1081 2022-12-06 04:22:54.000000 gigalixir-1.5.1/LICENSE
+-rw-rw-r--   0 tim       (1001) tim       (1001)      269 2023-06-12 14:23:45.311078 gigalixir-1.5.1/PKG-INFO
+-rw-rw-r--   0 tim       (1001) tim       (1001)     1470 2022-12-06 04:22:54.000000 gigalixir-1.5.1/README.md
+drwxrwxr-x   0 tim       (1001) tim       (1001)        0 2023-06-12 14:23:45.311078 gigalixir-1.5.1/gigalixir/
+-rw-rw-r--   0 tim       (1001) tim       (1001)    40314 2023-06-12 14:17:21.000000 gigalixir-1.5.1/gigalixir/__init__.py
+-rw-rw-r--   0 tim       (1001) tim       (1001)      229 2022-01-04 16:13:56.000000 gigalixir-1.5.1/gigalixir/api_exception.py
+-rw-rw-r--   0 tim       (1001) tim       (1001)      858 2022-01-04 16:13:56.000000 gigalixir-1.5.1/gigalixir/api_key.py
+-rw-rw-r--   0 tim       (1001) tim       (1001)    10135 2022-09-09 11:05:48.000000 gigalixir-1.5.1/gigalixir/app.py
+-rw-rw-r--   0 tim       (1001) tim       (1001)      538 2022-01-04 16:13:56.000000 gigalixir-1.5.1/gigalixir/app_activity.py
+-rw-rw-r--   0 tim       (1001) tim       (1001)      391 2022-01-04 16:13:56.000000 gigalixir-1.5.1/gigalixir/auth.py
+-rw-rw-r--   0 tim       (1001) tim       (1001)     1560 2022-01-04 16:13:56.000000 gigalixir-1.5.1/gigalixir/canary.py
+-rw-rw-r--   0 tim       (1001) tim       (1001)     1966 2023-06-12 13:26:20.000000 gigalixir-1.5.1/gigalixir/config.py
+-rw-rw-r--   0 tim       (1001) tim       (1001)     4082 2022-01-04 16:13:56.000000 gigalixir-1.5.1/gigalixir/database.py
+-rw-rw-r--   0 tim       (1001) tim       (1001)     1633 2022-01-04 16:13:56.000000 gigalixir-1.5.1/gigalixir/domain.py
+-rw-rw-r--   0 tim       (1001) tim       (1001)     1336 2022-01-04 16:13:56.000000 gigalixir-1.5.1/gigalixir/free_database.py
+-rw-rw-r--   0 tim       (1001) tim       (1001)      601 2022-01-04 16:13:56.000000 gigalixir-1.5.1/gigalixir/git.py
+-rw-rw-r--   0 tim       (1001) tim       (1001)      446 2022-01-04 16:13:56.000000 gigalixir-1.5.1/gigalixir/invoice.py
+-rw-rw-r--   0 tim       (1001) tim       (1001)     1262 2022-01-04 16:13:56.000000 gigalixir-1.5.1/gigalixir/log_drain.py
+-rw-rw-r--   0 tim       (1001) tim       (1001)     2653 2022-01-04 16:13:56.000000 gigalixir-1.5.1/gigalixir/mfa.py
+-rw-rw-r--   0 tim       (1001) tim       (1001)     3084 2022-01-04 16:13:56.000000 gigalixir-1.5.1/gigalixir/netrc.py
+-rw-rw-r--   0 tim       (1001) tim       (1001)     7045 2022-01-04 16:13:56.000000 gigalixir-1.5.1/gigalixir/observer.py
+drwxrwxr-x   0 tim       (1001) tim       (1001)        0 2023-06-12 14:23:45.311078 gigalixir-1.5.1/gigalixir/openers/
+-rw-rw-r--   0 tim       (1001) tim       (1001)        0 2022-01-04 16:13:56.000000 gigalixir-1.5.1/gigalixir/openers/__init__.py
+-rw-rw-r--   0 tim       (1001) tim       (1001)      207 2022-01-04 16:13:56.000000 gigalixir-1.5.1/gigalixir/openers/darwin.py
+-rw-rw-r--   0 tim       (1001) tim       (1001)      214 2022-01-04 16:13:56.000000 gigalixir-1.5.1/gigalixir/openers/linux.py
+-rw-rw-r--   0 tim       (1001) tim       (1001)      210 2022-01-04 16:13:56.000000 gigalixir-1.5.1/gigalixir/openers/windows.py
+-rw-rw-r--   0 tim       (1001) tim       (1001)     1172 2022-01-18 14:21:12.000000 gigalixir-1.5.1/gigalixir/payment_method.py
+-rw-rw-r--   0 tim       (1001) tim       (1001)     1274 2022-01-04 16:13:56.000000 gigalixir-1.5.1/gigalixir/permission.py
+-rw-rw-r--   0 tim       (1001) tim       (1001)      347 2022-01-04 16:13:56.000000 gigalixir-1.5.1/gigalixir/presenter.py
+-rw-rw-r--   0 tim       (1001) tim       (1001)      538 2022-01-04 16:13:56.000000 gigalixir-1.5.1/gigalixir/release.py
+drwxrwxr-x   0 tim       (1001) tim       (1001)        0 2023-06-12 14:23:45.311078 gigalixir-1.5.1/gigalixir/routers/
+-rw-rw-r--   0 tim       (1001) tim       (1001)        0 2022-01-04 16:13:56.000000 gigalixir-1.5.1/gigalixir/routers/__init__.py
+-rw-rw-r--   0 tim       (1001) tim       (1001)     1551 2022-01-04 16:13:56.000000 gigalixir-1.5.1/gigalixir/routers/darwin.py
+-rw-rw-r--   0 tim       (1001) tim       (1001)      902 2022-01-04 16:13:56.000000 gigalixir-1.5.1/gigalixir/routers/linux.py
+-rw-rw-r--   0 tim       (1001) tim       (1001)      618 2022-01-04 16:13:56.000000 gigalixir-1.5.1/gigalixir/routers/windows.py
+-rw-rw-r--   0 tim       (1001) tim       (1001)     1490 2022-01-04 16:13:56.000000 gigalixir-1.5.1/gigalixir/shell.py
+-rw-rw-r--   0 tim       (1001) tim       (1001)     1234 2022-01-04 16:13:56.000000 gigalixir-1.5.1/gigalixir/ssh_key.py
+-rw-rw-r--   0 tim       (1001) tim       (1001)      801 2022-08-20 15:11:07.000000 gigalixir-1.5.1/gigalixir/usage.py
+-rw-rw-r--   0 tim       (1001) tim       (1001)     7549 2023-03-16 02:46:36.000000 gigalixir-1.5.1/gigalixir/user.py
+drwxrwxr-x   0 tim       (1001) tim       (1001)        0 2023-06-12 14:23:45.311078 gigalixir-1.5.1/gigalixir.egg-info/
+-rw-rw-r--   0 tim       (1001) tim       (1001)      269 2023-06-12 14:23:45.000000 gigalixir-1.5.1/gigalixir.egg-info/PKG-INFO
+-rw-rw-r--   0 tim       (1001) tim       (1001)     1019 2023-06-12 14:23:45.000000 gigalixir-1.5.1/gigalixir.egg-info/SOURCES.txt
+-rw-rw-r--   0 tim       (1001) tim       (1001)        1 2023-06-12 14:23:45.000000 gigalixir-1.5.1/gigalixir.egg-info/dependency_links.txt
+-rw-rw-r--   0 tim       (1001) tim       (1001)       63 2023-06-12 14:23:45.000000 gigalixir-1.5.1/gigalixir.egg-info/entry_points.txt
+-rw-rw-r--   0 tim       (1001) tim       (1001)      187 2023-06-12 14:23:45.000000 gigalixir-1.5.1/gigalixir.egg-info/requires.txt
+-rw-rw-r--   0 tim       (1001) tim       (1001)       10 2023-06-12 14:23:45.000000 gigalixir-1.5.1/gigalixir.egg-info/top_level.txt
+-rw-rw-r--   0 tim       (1001) tim       (1001)       63 2023-06-12 14:23:45.311078 gigalixir-1.5.1/setup.cfg
+-rw-rw-r--   0 tim       (1001) tim       (1001)      959 2023-06-12 14:17:49.000000 gigalixir-1.5.1/setup.py
+drwxrwxr-x   0 tim       (1001) tim       (1001)        0 2023-06-12 14:23:45.311078 gigalixir-1.5.1/test/
+-rw-rw-r--   0 tim       (1001) tim       (1001)    36261 2022-01-27 06:29:24.000000 gigalixir-1.5.1/test/test_gigalixir.py
```

### Comparing `gigalixir-1.4.0/LICENSE` & `gigalixir-1.5.1/LICENSE`

 * *Files identical despite different names*

### Comparing `gigalixir-1.4.0/README.md` & `gigalixir-1.5.1/README.md`

 * *Files identical despite different names*

### Comparing `gigalixir-1.4.0/gigalixir/__init__.py` & `gigalixir-1.5.1/gigalixir/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -716,28 +716,14 @@
 @detect_app_name
 def add_domain(ctx, app_name, fully_qualified_domain_name):
     """
     Adds a custom domain name to your app.
     """
     gigalixir_domain.create(ctx.obj['host'], app_name, fully_qualified_domain_name)
 
-# @create.command()
-@cli.command(name='deprecated:set_config')
-@click.option('-a', '--app_name', envvar="GIGALIXIR_APP")
-@click.argument('key')
-@click.argument('value')
-@click.pass_context
-@report_errors
-@detect_app_name
-def set_config(ctx, app_name, key, value):
-    """
-    Set an app configuration/environment variable.
-    """
-    gigalixir_config.create(ctx.obj['host'], app_name, key, value)
-
 @cli.command(name="config:copy")
 @click.option('-s', '--src_app_name', required=True)
 @click.option('-d', '--dst_app_name', required=True)
 @click.option('-y', '--yes', is_flag=True)
 @click.pass_context
 @report_errors
 # no detecting app name for this one
@@ -748,19 +734,20 @@
     """
     logging.getLogger("gigalixir-cli").info("WARNING: This will copy all configs from %s to %s. This might overwrite some configs in %s." % (src_app_name, dst_app_name, dst_app_name))
     if yes or click.confirm('Are you sure you want to continue?'):
         gigalixir_config.copy(ctx.obj['host'], src_app_name, dst_app_name)
 
 @cli.command(name="config:set")
 @click.option('-a', '--app_name', envvar="GIGALIXIR_APP")
+@click.option('--no_restart', default=False, help="Do not restart the application.", is_flag=True)
 @click.argument('assignments', nargs=-1)
 @click.pass_context
 @report_errors
 @detect_app_name
-def config_set(ctx, app_name, assignments):
+def config_set(ctx, app_name, no_restart, assignments):
     """
     Set configuration variables and restarts your app.
     ASSIGNMENTS are of the form KEY=VALUE.
     For example,
     gigalixir config:set KEY0=VALUE0 KEY1="VALUE 1"
     """
     colored_keys = []
@@ -769,15 +756,15 @@
         try:
             key, value = assignment.split('=', 1)
             configs[key] = value
         except ValueError:
             print_help(ctx, "config:set")
             raise
 
-    gigalixir_config.create_multiple(ctx.obj['host'], app_name, configs)
+    gigalixir_config.create_multiple(ctx.obj['host'], app_name, configs, no_restart)
 
 # @get.command()
 @cli.command(name='account:confirmation:resend')
 @click.option('-e', '--email', prompt=True)
 @click.pass_context
 @report_errors
 def send_email_confirmation_token(ctx, email):
```

### Comparing `gigalixir-1.4.0/gigalixir/api_key.py` & `gigalixir-1.5.1/gigalixir/api_key.py`

 * *Files identical despite different names*

### Comparing `gigalixir-1.4.0/gigalixir/app.py` & `gigalixir-1.5.1/gigalixir/app.py`

 * *Files identical despite different names*

### Comparing `gigalixir-1.4.0/gigalixir/app_activity.py` & `gigalixir-1.5.1/gigalixir/app_activity.py`

 * *Files identical despite different names*

### Comparing `gigalixir-1.4.0/gigalixir/canary.py` & `gigalixir-1.5.1/gigalixir/canary.py`

 * *Files identical despite different names*

### Comparing `gigalixir-1.4.0/gigalixir/config.py` & `gigalixir-1.5.1/gigalixir/config.py`

 * *Files 7% similar despite different names*

```diff
@@ -14,34 +14,20 @@
         if r.status_code == 401:
             raise auth.AuthException()
         raise Exception(r.text)
     else:
         data = json.loads(r.text)["data"]
         presenter.echo_json(data)
 
-def create(host, app_name, key, value):
+def create_multiple(host, app_name, configs, dont_restart):
     r = requests.post('%s/api/apps/%s/configs' % (host, quote(app_name.encode('utf-8'))), headers = {
         'Content-Type': 'application/json',
     }, json = {
-        "key": key,
-        "value": value
-    })
-    if r.status_code != 201:
-        if r.status_code == 401:
-            raise auth.AuthException()
-        raise Exception(r.text)
-    else:
-        data = json.loads(r.text)["data"]
-        presenter.echo_json(data)
-
-def create_multiple(host, app_name, configs):
-    r = requests.post('%s/api/apps/%s/configs' % (host, quote(app_name.encode('utf-8'))), headers = {
-        'Content-Type': 'application/json',
-    }, json = {
-        "configs": configs
+        "configs": configs,
+        "avoid_restart": dont_restart
     })
     if r.status_code != 201:
         if r.status_code == 401:
             raise auth.AuthException()
         raise Exception(r.text)
     else:
         data = json.loads(r.text)["data"]
```

### Comparing `gigalixir-1.4.0/gigalixir/database.py` & `gigalixir-1.5.1/gigalixir/database.py`

 * *Files identical despite different names*

### Comparing `gigalixir-1.4.0/gigalixir/domain.py` & `gigalixir-1.5.1/gigalixir/domain.py`

 * *Files identical despite different names*

### Comparing `gigalixir-1.4.0/gigalixir/free_database.py` & `gigalixir-1.5.1/gigalixir/free_database.py`

 * *Files identical despite different names*

### Comparing `gigalixir-1.4.0/gigalixir/git.py` & `gigalixir-1.5.1/gigalixir/git.py`

 * *Files identical despite different names*

### Comparing `gigalixir-1.4.0/gigalixir/log_drain.py` & `gigalixir-1.5.1/gigalixir/log_drain.py`

 * *Files identical despite different names*

### Comparing `gigalixir-1.4.0/gigalixir/mfa.py` & `gigalixir-1.5.1/gigalixir/mfa.py`

 * *Files identical despite different names*

### Comparing `gigalixir-1.4.0/gigalixir/netrc.py` & `gigalixir-1.5.1/gigalixir/netrc.py`

 * *Files identical despite different names*

### Comparing `gigalixir-1.4.0/gigalixir/observer.py` & `gigalixir-1.5.1/gigalixir/observer.py`

 * *Files identical despite different names*

### Comparing `gigalixir-1.4.0/gigalixir/payment_method.py` & `gigalixir-1.5.1/gigalixir/payment_method.py`

 * *Files identical despite different names*

### Comparing `gigalixir-1.4.0/gigalixir/permission.py` & `gigalixir-1.5.1/gigalixir/permission.py`

 * *Files identical despite different names*

### Comparing `gigalixir-1.4.0/gigalixir/release.py` & `gigalixir-1.5.1/gigalixir/release.py`

 * *Files identical despite different names*

### Comparing `gigalixir-1.4.0/gigalixir/routers/darwin.py` & `gigalixir-1.5.1/gigalixir/routers/darwin.py`

 * *Files identical despite different names*

### Comparing `gigalixir-1.4.0/gigalixir/routers/linux.py` & `gigalixir-1.5.1/gigalixir/routers/linux.py`

 * *Files identical despite different names*

### Comparing `gigalixir-1.4.0/gigalixir/routers/windows.py` & `gigalixir-1.5.1/gigalixir/routers/windows.py`

 * *Files identical despite different names*

### Comparing `gigalixir-1.4.0/gigalixir/shell.py` & `gigalixir-1.5.1/gigalixir/shell.py`

 * *Files identical despite different names*

### Comparing `gigalixir-1.4.0/gigalixir/ssh_key.py` & `gigalixir-1.5.1/gigalixir/ssh_key.py`

 * *Files identical despite different names*

### Comparing `gigalixir-1.4.0/gigalixir/usage.py` & `gigalixir-1.5.1/gigalixir/usage.py`

 * *Files identical despite different names*

### Comparing `gigalixir-1.4.0/gigalixir/user.py` & `gigalixir-1.5.1/gigalixir/user.py`

 * *Files identical despite different names*

### Comparing `gigalixir-1.4.0/gigalixir.egg-info/SOURCES.txt` & `gigalixir-1.5.1/gigalixir.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `gigalixir-1.4.0/setup.py` & `gigalixir-1.5.1/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 from setuptools import setup, find_packages
 
 setup(
     name='gigalixir',
     url='https://github.com/gigalixir/gigalixir-cli',
     author='Tim Day',
     author_email='tim@gigalixir.com',
-    version='1.4.0',
+    version='1.5.1',
     packages=find_packages(),
     include_package_data=True,
     install_requires=[
         'click>=8.1',
         'requests>=2.28',
         'stripe>=4.1',
         'rollbar>=0.16',
```

### Comparing `gigalixir-1.4.0/test/test_gigalixir.py` & `gigalixir-1.5.1/test/test_gigalixir.py`

 * *Files identical despite different names*

