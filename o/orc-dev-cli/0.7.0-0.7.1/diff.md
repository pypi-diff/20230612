# Comparing `tmp/orc-dev-cli-0.7.0.tar.gz` & `tmp/orc_dev_cli-0.7.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "orc-dev-cli-0.7.0.tar", max compression
+gzip compressed data, was "orc_dev_cli-0.7.1.tar", max compression
```

## Comparing `orc-dev-cli-0.7.0.tar` & `orc_dev_cli-0.7.1.tar`

### file list

```diff
@@ -1,24 +1,23 @@
--rw-r--r--   0        0        0      917 2023-02-18 14:16:18.860429 orc-dev-cli-0.7.0/README.md
--rw-r--r--   0        0        0       22 2023-02-18 14:19:07.336879 orc-dev-cli-0.7.0/orc_dev_cli/__init__.py
--rw-r--r--   0        0        0     6849 2023-02-18 14:16:18.861429 orc-dev-cli-0.7.0/orc_dev_cli/addon_state.py
--rw-r--r--   0        0        0      656 2023-02-18 14:16:18.861429 orc-dev-cli-0.7.0/orc_dev_cli/cli.py
--rw-r--r--   0        0        0     1505 2023-02-18 14:16:18.861429 orc-dev-cli-0.7.0/orc_dev_cli/cluster/__init__.py
--rw-r--r--   0        0        0     3157 2023-02-18 14:16:18.861429 orc-dev-cli-0.7.0/orc_dev_cli/cluster/cli.py
--rw-r--r--   0        0        0      217 2023-02-18 14:16:18.861429 orc-dev-cli-0.7.0/orc_dev_cli/cluster/defaults.py
--rw-r--r--   0        0        0      356 2023-02-18 14:16:18.861429 orc-dev-cli-0.7.0/orc_dev_cli/cluster/delete.py
--rw-r--r--   0        0        0     4754 2023-02-18 14:16:18.861429 orc-dev-cli-0.7.0/orc_dev_cli/cluster/list.py
--rw-r--r--   0        0        0     1566 2023-02-18 14:16:18.861429 orc-dev-cli-0.7.0/orc_dev_cli/cluster/login.py
--rw-r--r--   0        0        0     1350 2023-02-18 14:16:18.861429 orc-dev-cli-0.7.0/orc_dev_cli/cluster/status.py
--rw-r--r--   0        0        0      729 2023-02-18 14:16:18.862429 orc-dev-cli-0.7.0/orc_dev_cli/code.py
--rw-r--r--   0        0        0     2073 2023-02-18 14:16:18.862429 orc-dev-cli-0.7.0/orc_dev_cli/config.py
--rw-r--r--   0        0        0     7010 2023-02-18 14:01:37.799281 orc-dev-cli-0.7.0/orc_dev_cli/data/index_build.toml
--rw-r--r--   0        0        0      216 2023-02-18 14:16:18.862429 orc-dev-cli-0.7.0/orc_dev_cli/helper.py
--rw-r--r--   0        0        0        0 2023-02-18 14:16:18.862429 orc-dev-cli-0.7.0/orc_dev_cli/rhoam/__init__.py
--rw-r--r--   0        0        0     2891 2023-02-18 14:16:18.862429 orc-dev-cli-0.7.0/orc_dev_cli/rhoam/cli.py
--rw-r--r--   0        0        0      751 2023-02-18 14:16:18.862429 orc-dev-cli-0.7.0/orc_dev_cli/rhoam/delete.py
--rw-r--r--   0        0        0    17153 2023-02-18 14:16:18.862429 orc-dev-cli-0.7.0/orc_dev_cli/rhoam/index/__init__.py
--rw-r--r--   0        0        0      911 2023-02-18 14:16:18.862429 orc-dev-cli-0.7.0/orc_dev_cli/rhoam/index/default.py
--rw-r--r--   0        0        0      789 2023-02-18 14:16:18.862429 orc-dev-cli-0.7.0/orc_dev_cli/rhoam/status.py
--rw-r--r--   0        0        0     1577 2023-02-18 14:19:07.336879 orc-dev-cli-0.7.0/pyproject.toml
--rw-r--r--   0        0        0     2172 2023-02-18 14:22:37.223758 orc-dev-cli-0.7.0/setup.py
--rw-r--r--   0        0        0     2052 2023-02-18 14:22:37.224074 orc-dev-cli-0.7.0/PKG-INFO
+-rw-r--r--   0        0        0      917 2023-02-18 14:28:03.267048 orc_dev_cli-0.7.1/README.md
+-rw-r--r--   0        0        0       22 2023-06-12 18:00:00.228050 orc_dev_cli-0.7.1/orc_dev_cli/__init__.py
+-rw-r--r--   0        0        0     6869 2023-06-12 18:00:00.229050 orc_dev_cli-0.7.1/orc_dev_cli/addon_state.py
+-rw-r--r--   0        0        0      656 2023-02-18 14:16:18.861429 orc_dev_cli-0.7.1/orc_dev_cli/cli.py
+-rw-r--r--   0        0        0     1504 2023-06-12 18:00:00.229050 orc_dev_cli-0.7.1/orc_dev_cli/cluster/__init__.py
+-rw-r--r--   0        0        0     3157 2023-02-18 14:16:18.861429 orc_dev_cli-0.7.1/orc_dev_cli/cluster/cli.py
+-rw-r--r--   0        0        0      217 2023-02-18 14:16:18.861429 orc_dev_cli-0.7.1/orc_dev_cli/cluster/defaults.py
+-rw-r--r--   0        0        0      356 2023-02-18 14:16:18.861429 orc_dev_cli-0.7.1/orc_dev_cli/cluster/delete.py
+-rw-r--r--   0        0        0     4754 2023-02-18 14:16:18.861429 orc_dev_cli-0.7.1/orc_dev_cli/cluster/list.py
+-rw-r--r--   0        0        0     1566 2023-02-18 14:16:18.861429 orc_dev_cli-0.7.1/orc_dev_cli/cluster/login.py
+-rw-r--r--   0        0        0     1350 2023-02-18 14:16:18.861429 orc_dev_cli-0.7.1/orc_dev_cli/cluster/status.py
+-rw-r--r--   0        0        0      728 2023-06-12 18:00:00.229050 orc_dev_cli-0.7.1/orc_dev_cli/code.py
+-rw-r--r--   0        0        0     2071 2023-06-12 18:00:00.229050 orc_dev_cli-0.7.1/orc_dev_cli/config.py
+-rw-r--r--   0        0        0     7010 2023-02-18 14:01:37.799281 orc_dev_cli-0.7.1/orc_dev_cli/data/index_build.toml
+-rw-r--r--   0        0        0      216 2023-02-18 14:16:18.862429 orc_dev_cli-0.7.1/orc_dev_cli/helper.py
+-rw-r--r--   0        0        0        0 2023-02-18 14:16:18.862429 orc_dev_cli-0.7.1/orc_dev_cli/rhoam/__init__.py
+-rw-r--r--   0        0        0     2942 2023-03-04 12:14:08.959799 orc_dev_cli-0.7.1/orc_dev_cli/rhoam/cli.py
+-rw-r--r--   0        0        0      751 2023-02-18 14:28:03.268048 orc_dev_cli-0.7.1/orc_dev_cli/rhoam/delete.py
+-rw-r--r--   0        0        0    17160 2023-06-12 18:00:00.229050 orc_dev_cli-0.7.1/orc_dev_cli/rhoam/index/__init__.py
+-rw-r--r--   0        0        0      911 2023-02-18 14:16:18.862429 orc_dev_cli-0.7.1/orc_dev_cli/rhoam/index/default.py
+-rw-r--r--   0        0        0      789 2023-02-18 14:16:18.862429 orc_dev_cli-0.7.1/orc_dev_cli/rhoam/status.py
+-rw-r--r--   0        0        0     1577 2023-06-12 18:00:00.230050 orc_dev_cli-0.7.1/pyproject.toml
+-rw-r--r--   0        0        0     2104 1970-01-01 00:00:00.000000 orc_dev_cli-0.7.1/PKG-INFO
```

### Comparing `orc-dev-cli-0.7.0/README.md` & `orc_dev_cli-0.7.1/README.md`

 * *Files identical despite different names*

### Comparing `orc-dev-cli-0.7.0/orc_dev_cli/addon_state.py` & `orc_dev_cli-0.7.1/orc_dev_cli/addon_state.py`

 * *Files 1% similar despite different names*

```diff
@@ -152,14 +152,15 @@
 
 def get_addon_alerts(route, bearer_token):
     resq = requests.get(
         f"https://{route}/api/v1/alerts",
         headers={"Authorization": f"Bearer {bearer_token}"},
         cookies={},
         auth=(),
+        timeout=30,
     )
 
     if resq.status_code == 200:
         return resq.json()["data"]["alerts"]
     else:
         return None
```

### Comparing `orc-dev-cli-0.7.0/orc_dev_cli/cli.py` & `orc_dev_cli-0.7.1/orc_dev_cli/cli.py`

 * *Files identical despite different names*

### Comparing `orc-dev-cli-0.7.0/orc_dev_cli/cluster/__init__.py` & `orc_dev_cli-0.7.1/orc_dev_cli/cluster/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -11,15 +11,14 @@
     found_cluster = get_cluster_data(cluster_name)
 
     cluster_id: str = found_cluster["id"]
     return cluster_id
 
 
 def get_cluster_data(cluster_name):
-
     n = safe_string(cluster_name)
     s = f"search=\"name='{n}'\""
 
     output = subprocess.run(
         [f"ocm get clusters -p {s}"], shell=True, capture_output=True  # nosec
     )
```

### Comparing `orc-dev-cli-0.7.0/orc_dev_cli/cluster/cli.py` & `orc_dev_cli-0.7.1/orc_dev_cli/cluster/cli.py`

 * *Files identical despite different names*

### Comparing `orc-dev-cli-0.7.0/orc_dev_cli/cluster/list.py` & `orc_dev_cli-0.7.1/orc_dev_cli/cluster/list.py`

 * *Files identical despite different names*

### Comparing `orc-dev-cli-0.7.0/orc_dev_cli/cluster/login.py` & `orc_dev_cli-0.7.1/orc_dev_cli/cluster/login.py`

 * *Files identical despite different names*

### Comparing `orc-dev-cli-0.7.0/orc_dev_cli/cluster/status.py` & `orc_dev_cli-0.7.1/orc_dev_cli/cluster/status.py`

 * *Files identical despite different names*

### Comparing `orc-dev-cli-0.7.0/orc_dev_cli/code.py` & `orc_dev_cli-0.7.1/orc_dev_cli/code.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,13 @@
 import sys
 
 import click
 
 
 def state_exit_condition(state, message):
-
     if state is None:
         return
 
     state = state.lower()
     data = message.split("\n")
 
     if len(data) > 2:
```

### Comparing `orc-dev-cli-0.7.0/orc_dev_cli/config.py` & `orc_dev_cli-0.7.1/orc_dev_cli/config.py`

 * *Files 0% similar despite different names*

```diff
@@ -14,15 +14,14 @@
 
 HOST = pathlib.Path.home()
 CONFIG_PATH = pathlib.Path(HOST, ".config", "orc")
 CONFIG_FILE = pathlib.Path(CONFIG_PATH, "config.toml")
 
 
 def configuration_file():
-
     if not CONFIG_FILE.is_file():
         CONFIG_PATH.mkdir(parents=True, exist_ok=True)
         data = textwrap.dedent(
             """\
         [default]
         cluster = ""
         delay = 10
@@ -44,15 +43,14 @@
         click.echo("Auto opening of configuration file failed unsupported platform")
         exit(1)
 
     subprocess.call([cmd, CONFIG_FILE])  # nosec
 
 
 def merge(a: dict, b: dict):
-
     for key in a:
         if key in b:
             if isinstance(a[key], dict) and isinstance(b[key], dict):
                 a[key].update(merge(a[key], b[key]))
             else:
                 a[key] = b[key]
```

### Comparing `orc-dev-cli-0.7.0/orc_dev_cli/data/index_build.toml` & `orc_dev_cli-0.7.1/orc_dev_cli/data/index_build.toml`

 * *Files identical despite different names*

### Comparing `orc-dev-cli-0.7.0/orc_dev_cli/rhoam/cli.py` & `orc_dev_cli-0.7.1/orc_dev_cli/rhoam/cli.py`

 * *Files 2% similar despite different names*

```diff
@@ -111,8 +111,9 @@
     prompt="Are you sure you want to delete this RHOAM?",
     help="Confirm deletion on command execution.",
 )
 def delete(cluster_, prefix):
     """
     Delete the RHOAM rhmi CR from a cluster
     """
+    click.echo("This action may take sometime...")
     _delete.action(cluster_, prefix)
```

### Comparing `orc-dev-cli-0.7.0/orc_dev_cli/rhoam/delete.py` & `orc_dev_cli-0.7.1/orc_dev_cli/rhoam/delete.py`

 * *Files identical despite different names*

### Comparing `orc-dev-cli-0.7.0/orc_dev_cli/rhoam/index/__init__.py` & `orc_dev_cli-0.7.1/orc_dev_cli/rhoam/index/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -63,15 +63,14 @@
         version = get_semver(release, prefix)
         versions[version] = release
 
     return versions
 
 
 def sort_releases(releases):
-
     keys = list(releases.keys())
     keys = sorted(keys)
 
     versions = []
     prerelease = []
     prerelease_rc = {}
     for key in keys:
@@ -123,15 +122,14 @@
         if key in config and config[key]["include"]:
             result.append(key)
 
     return result
 
 
 def get_working_release(chain_start, data):
-
     match chain_start:
         case None:
             return {"tags": [], "other": []}
         case "new":
             return {"tags": [], "other": ["new"]}
         case "latest":
             return {"tags": [], "other": ["latest", "new"]}
@@ -185,15 +183,15 @@
             fg="red",
             bold=True,
         )
         return False
 
     click.echo(f"Searching for tag {tag} in repository {repo}")
     url = f"https://{image_site}/api/v1/repository/{org}/{repo}/tag"
-    resq = requests.get(url)
+    resq = requests.get(url, timeout=30)
     data = resq.json()
     data = data["tags"]
     for t in data:
         if t["name"] == tag:
             return True
     return False
 
@@ -340,28 +338,26 @@
     if label != "new":
         repo.git.restore("*")
 
     return data
 
 
 def is_service_affecting(csv, state):
-
     match state:
         case "existing":
             if csv.exists():
                 service_affecting = get_service_affecting(csv)
             else:
                 service_affecting = True
             return service_affecting
         case _:
             return state
 
 
 def get_config_value(setting, config, tag=None, label=None):
-
     if tag is not None:
         tag = str(tag)
         if tag in config and setting in config[tag]:
             return config[tag][setting]
 
     if label is not None:
         if label in config and setting in config[label]:
@@ -444,15 +440,14 @@
         if tag == data["tags"][-1]:
             label = "current"
         chain_data = work_on_tag(repo, tag, config, bundles, first, label=label)
         chain[tag] = chain_data
         last_tag = tag
 
     if "latest" in data["other"]:
-
         click.echo(f"Working on: latest ({config['latest']['branch']})")
 
         if last_tag is None:
             first = True
         else:
             first = False
```

### Comparing `orc-dev-cli-0.7.0/orc_dev_cli/rhoam/index/default.py` & `orc_dev_cli-0.7.1/orc_dev_cli/rhoam/index/default.py`

 * *Files identical despite different names*

### Comparing `orc-dev-cli-0.7.0/orc_dev_cli/rhoam/status.py` & `orc_dev_cli-0.7.1/orc_dev_cli/rhoam/status.py`

 * *Files identical despite different names*

### Comparing `orc-dev-cli-0.7.0/pyproject.toml` & `orc_dev_cli-0.7.1/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "orc-dev-cli"
-version = "0.7.0"
+version = "0.7.1"
 description = "CLI dev tool for interacting with openshift clusters and RHOAM addons."
 authors = ["Jim Fitzpatrick <jimfity@gmail.com>"]
 readme="README.md"
 homepage = "https://github.com/Boomatang/orc-dev-cli"
 repository = "https://github.com/Boomatang/orc-dev-cli"
 documentation = "https://github.com/Boomatang/orc-dev-cli/tree/main/doc"
 keywords = ['OpenShift', 'addon', 'operator', 'index', 'bundle']
```

### Comparing `orc-dev-cli-0.7.0/PKG-INFO` & `orc_dev_cli-0.7.1/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,30 +1,31 @@
 Metadata-Version: 2.1
 Name: orc-dev-cli
-Version: 0.7.0
+Version: 0.7.1
 Summary: CLI dev tool for interacting with openshift clusters and RHOAM addons.
 Home-page: https://github.com/Boomatang/orc-dev-cli
 Keywords: OpenShift,addon,operator,index,bundle
 Author: Jim Fitzpatrick
 Author-email: jimfity@gmail.com
 Requires-Python: >=3.10,<4.0
 Classifier: Intended Audience :: Developers
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
 Classifier: Topic :: Software Development :: Build Tools
 Requires-Dist: GitPython (>=3.1.28,<4.0.0)
 Requires-Dist: PyYAML (>=6.0,<7.0)
 Requires-Dist: click (>=8.1.2,<9.0.0)
 Requires-Dist: podman (>=4.2.0,<5.0.0)
 Requires-Dist: pydantic (>=1.10.4,<2.0.0)
 Requires-Dist: pyperclip (>=1.8.2,<2.0.0)
 Requires-Dist: requests (>=2.28.1,<3.0.0)
 Requires-Dist: rich (>=13.2.0,<14.0.0)
 Requires-Dist: semver (>=2.13.0,<3.0.0)
-Requires-Dist: toml (>=0.10.2,<0.11.0); python_version < "3.11"
+Requires-Dist: toml (>=0.10.2,<0.11.0) ; python_version < "3.11"
 Project-URL: Documentation, https://github.com/Boomatang/orc-dev-cli/tree/main/doc
 Project-URL: Repository, https://github.com/Boomatang/orc-dev-cli
 Description-Content-Type: text/markdown
 
 # Welcome to orc-dev-cli
 
 Orc-dev-cli gives developers a CLI tool called orc.
```

