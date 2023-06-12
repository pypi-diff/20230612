# Comparing `tmp/qgis-plugin-manager-1.5.0.tar.gz` & `tmp/qgis-plugin-manager-1.6.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "qgis-plugin-manager-1.5.0.tar", last modified: Tue Jan 24 14:34:06 2023, max compression
+gzip compressed data, was "qgis-plugin-manager-1.6.0.tar", last modified: Mon Jun 12 09:55:21 2023, max compression
```

## Comparing `qgis-plugin-manager-1.5.0.tar` & `qgis-plugin-manager-1.6.0.tar`

### file list

```diff
@@ -1,24 +1,24 @@
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-01-24 14:34:06.256955 qgis-plugin-manager-1.5.0/
--rw-r--r--   0 runner    (1001) docker     (122)    10537 2023-01-24 14:34:06.260956 qgis-plugin-manager-1.5.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (122)     9142 2023-01-24 14:34:00.000000 qgis-plugin-manager-1.5.0/README.md
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-01-24 14:34:06.256955 qgis-plugin-manager-1.5.0/qgis_plugin_manager/
--rw-r--r--   0 runner    (1001) docker     (122)     1203 2023-01-24 14:34:04.000000 qgis-plugin-manager-1.5.0/qgis_plugin_manager/__about__.py
--rw-r--r--   0 runner    (1001) docker     (122)       97 2023-01-24 14:34:00.000000 qgis-plugin-manager-1.5.0/qgis_plugin_manager/__init__.py
--rwxr-xr-x   0 runner    (1001) docker     (122)     6784 2023-01-24 14:34:00.000000 qgis-plugin-manager-1.5.0/qgis_plugin_manager/__main__.py
--rw-r--r--   0 runner    (1001) docker     (122)      970 2023-01-24 14:34:00.000000 qgis-plugin-manager-1.5.0/qgis_plugin_manager/definitions.py
--rw-r--r--   0 runner    (1001) docker     (122)    11958 2023-01-24 14:34:00.000000 qgis-plugin-manager-1.5.0/qgis_plugin_manager/local_directory.py
--rw-r--r--   0 runner    (1001) docker     (122)    16186 2023-01-24 14:34:00.000000 qgis-plugin-manager-1.5.0/qgis_plugin_manager/remote.py
--rw-r--r--   0 runner    (1001) docker     (122)     4055 2023-01-24 14:34:00.000000 qgis-plugin-manager-1.5.0/qgis_plugin_manager/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-01-24 14:34:06.256955 qgis-plugin-manager-1.5.0/qgis_plugin_manager.egg-info/
--rw-r--r--   0 runner    (1001) docker     (122)    10537 2023-01-24 14:34:06.000000 qgis-plugin-manager-1.5.0/qgis_plugin_manager.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (122)      560 2023-01-24 14:34:06.000000 qgis-plugin-manager-1.5.0/qgis_plugin_manager.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (122)        1 2023-01-24 14:34:06.000000 qgis-plugin-manager-1.5.0/qgis_plugin_manager.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (122)       74 2023-01-24 14:34:06.000000 qgis-plugin-manager-1.5.0/qgis_plugin_manager.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (122)       20 2023-01-24 14:34:06.000000 qgis-plugin-manager-1.5.0/qgis_plugin_manager.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (122)      308 2023-01-24 14:34:06.260956 qgis-plugin-manager-1.5.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (122)     2431 2023-01-24 14:34:04.000000 qgis-plugin-manager-1.5.0/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-01-24 14:34:06.256955 qgis-plugin-manager-1.5.0/test/
--rw-r--r--   0 runner    (1001) docker     (122)     3737 2023-01-24 14:34:00.000000 qgis-plugin-manager-1.5.0/test/test_full_install.py
--rw-r--r--   0 runner    (1001) docker     (122)     2025 2023-01-24 14:34:00.000000 qgis-plugin-manager-1.5.0/test/test_local.py
--rw-r--r--   0 runner    (1001) docker     (122)     3117 2023-01-24 14:34:00.000000 qgis-plugin-manager-1.5.0/test/test_remote.py
--rw-r--r--   0 runner    (1001) docker     (122)     1041 2023-01-24 14:34:00.000000 qgis-plugin-manager-1.5.0/test/test_utils.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-12 09:55:21.743742 qgis-plugin-manager-1.6.0/
+-rw-r--r--   0 runner    (1001) docker     (122)    10853 2023-06-12 09:55:21.743742 qgis-plugin-manager-1.6.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (122)     9458 2023-06-12 09:55:13.000000 qgis-plugin-manager-1.6.0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-12 09:55:21.739742 qgis-plugin-manager-1.6.0/qgis_plugin_manager/
+-rw-r--r--   0 runner    (1001) docker     (122)     1203 2023-06-12 09:55:19.000000 qgis-plugin-manager-1.6.0/qgis_plugin_manager/__about__.py
+-rw-r--r--   0 runner    (1001) docker     (122)       97 2023-06-12 09:55:13.000000 qgis-plugin-manager-1.6.0/qgis_plugin_manager/__init__.py
+-rwxr-xr-x   0 runner    (1001) docker     (122)     6784 2023-06-12 09:55:13.000000 qgis-plugin-manager-1.6.0/qgis_plugin_manager/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (122)      970 2023-06-12 09:55:13.000000 qgis-plugin-manager-1.6.0/qgis_plugin_manager/definitions.py
+-rw-r--r--   0 runner    (1001) docker     (122)    11958 2023-06-12 09:55:13.000000 qgis-plugin-manager-1.6.0/qgis_plugin_manager/local_directory.py
+-rw-r--r--   0 runner    (1001) docker     (122)    18787 2023-06-12 09:55:13.000000 qgis-plugin-manager-1.6.0/qgis_plugin_manager/remote.py
+-rw-r--r--   0 runner    (1001) docker     (122)     4055 2023-06-12 09:55:13.000000 qgis-plugin-manager-1.6.0/qgis_plugin_manager/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-12 09:55:21.739742 qgis-plugin-manager-1.6.0/qgis_plugin_manager.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (122)    10853 2023-06-12 09:55:21.000000 qgis-plugin-manager-1.6.0/qgis_plugin_manager.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (122)      560 2023-06-12 09:55:21.000000 qgis-plugin-manager-1.6.0/qgis_plugin_manager.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (122)        1 2023-06-12 09:55:21.000000 qgis-plugin-manager-1.6.0/qgis_plugin_manager.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (122)       74 2023-06-12 09:55:21.000000 qgis-plugin-manager-1.6.0/qgis_plugin_manager.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (122)       20 2023-06-12 09:55:21.000000 qgis-plugin-manager-1.6.0/qgis_plugin_manager.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (122)      308 2023-06-12 09:55:21.743742 qgis-plugin-manager-1.6.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (122)     2431 2023-06-12 09:55:19.000000 qgis-plugin-manager-1.6.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-12 09:55:21.743742 qgis-plugin-manager-1.6.0/test/
+-rw-r--r--   0 runner    (1001) docker     (122)     3737 2023-06-12 09:55:13.000000 qgis-plugin-manager-1.6.0/test/test_full_install.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2025 2023-06-12 09:55:13.000000 qgis-plugin-manager-1.6.0/test/test_local.py
+-rw-r--r--   0 runner    (1001) docker     (122)     4298 2023-06-12 09:55:13.000000 qgis-plugin-manager-1.6.0/test/test_remote.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1041 2023-06-12 09:55:13.000000 qgis-plugin-manager-1.6.0/test/test_utils.py
```

### Comparing `qgis-plugin-manager-1.5.0/PKG-INFO` & `qgis-plugin-manager-1.6.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 Metadata-Version: 2.1
 Name: qgis-plugin-manager
-Version: 1.5.0
+Version: 1.6.0
 Summary: Tool for downloading/managing QGIS plugins from CLI.
 Home-page: https://github.com/3liz/qgis-plugin-manager
-Download-URL: https://github.com/3liz/qgis-plugin-manager/archive/1.5.0.tar.gz
+Download-URL: https://github.com/3liz/qgis-plugin-manager/archive/1.6.0.tar.gz
 Author: Étienne Trimaille
 Author-email: etrimaille@3liz.com
 Project-URL: Docs, https://github.com/3liz/qgis-plugin-manager/blob/master/README.md
 Project-URL: Bug Reports, https://github.com/3liz/qgis-plugin-manager/issues/
 Project-URL: Source, https://github.com/3liz/qgis-plugin-manager
 Keywords: QGIS
 Classifier: Development Status :: 5 - Production/Stable
@@ -157,14 +157,25 @@
 `[VERSION]` is a token in the `sources.list` file to be replaced by the QGIS version, for instance `3.22`.
 If QGIS is upgraded, the XML file will be updated as well.
 
 You don't have to set the TOKEN for all URL : 
 
 `https://docs.3liz.org/plugins.xml` is valid.
 
+#### Basic authentication
+
+It's possible to add a login and password in the remote URL :
+
+```bash
+https://docs.3liz.org/private/repo.xml?username=loginwpd&password=pass
+```
+
+Every URL is parsed, and if some credentials are found, the URL is cleaned and the request is done using the
+basic authentication.
+
 ### Update
 
 To fetch the XML files from each repository :
 
 ```bash
 $ qgis-plugin-manager update
 Downloading https://plugins.qgis.org/plugins/plugins.xml?qgis=3.19...
@@ -250,17 +261,18 @@
 You can use `--force` or `-f` to force the upgrade for all plugins despite their version.
 
 *Note*, like APT, `update` is needed before to refresh the cache.
 
 #### Ignore plugins from the upgrade
 
 Some plugins might be installed by hand, without being installed with a remote. This command will try to upgrade
-**all valid** plugins found. However, the command will fail because the plugin has been installed without a remote.
+**all valid** plugins found in the directory. However, the command will fail because the plugin has been installed 
+without a remote.
 
-It's possible to ignore such plugin by adding a file `ignorePlugins.list`, next to the `sources.list` file,
+It's possible to ignore such plugin by adding a file `ignorePlugins.list`, in your plugins' folder,
 with a list of **plugin name** on each line. The `upgrade` will not try to upgrade them.
 
 ### Remove
 
 It's possible to use `rm -rf folder_dir` but you can also remove by the plugin name.
 It will take care of the `QGIS_PLUGINPATH` environment variable.
```

### Comparing `qgis-plugin-manager-1.5.0/README.md` & `qgis-plugin-manager-1.6.0/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -128,14 +128,25 @@
 `[VERSION]` is a token in the `sources.list` file to be replaced by the QGIS version, for instance `3.22`.
 If QGIS is upgraded, the XML file will be updated as well.
 
 You don't have to set the TOKEN for all URL : 
 
 `https://docs.3liz.org/plugins.xml` is valid.
 
+#### Basic authentication
+
+It's possible to add a login and password in the remote URL :
+
+```bash
+https://docs.3liz.org/private/repo.xml?username=loginwpd&password=pass
+```
+
+Every URL is parsed, and if some credentials are found, the URL is cleaned and the request is done using the
+basic authentication.
+
 ### Update
 
 To fetch the XML files from each repository :
 
 ```bash
 $ qgis-plugin-manager update
 Downloading https://plugins.qgis.org/plugins/plugins.xml?qgis=3.19...
@@ -221,17 +232,18 @@
 You can use `--force` or `-f` to force the upgrade for all plugins despite their version.
 
 *Note*, like APT, `update` is needed before to refresh the cache.
 
 #### Ignore plugins from the upgrade
 
 Some plugins might be installed by hand, without being installed with a remote. This command will try to upgrade
-**all valid** plugins found. However, the command will fail because the plugin has been installed without a remote.
+**all valid** plugins found in the directory. However, the command will fail because the plugin has been installed 
+without a remote.
 
-It's possible to ignore such plugin by adding a file `ignorePlugins.list`, next to the `sources.list` file,
+It's possible to ignore such plugin by adding a file `ignorePlugins.list`, in your plugins' folder,
 with a list of **plugin name** on each line. The `upgrade` will not try to upgrade them.
 
 ### Remove
 
 It's possible to use `rm -rf folder_dir` but you can also remove by the plugin name.
 It will take care of the `QGIS_PLUGINPATH` environment variable.
```

### Comparing `qgis-plugin-manager-1.5.0/qgis_plugin_manager/__about__.py` & `qgis-plugin-manager-1.6.0/qgis_plugin_manager/__about__.py`

 * *Files 0% similar despite different names*

```diff
@@ -24,15 +24,15 @@
 __license__ = "GNU General Public License v3.0"
 __summary__ = "Tool for downloading/managing QGIS plugins from CLI."
 __title__ = "QGIS Plugin Manager"
 __title_clean__ = "".join(e for e in __title__ if e.isalnum())
 __uri__ = "https://github.com/3liz/qgis-plugin-manager"
 
 # This string might be updated on CI on runtime with a proper semantic version name with X.Y.Z
-__version__ = "1.5.0"
+__version__ = "1.6.0"
 
 if "." not in __version__:
     # If __version__ is still not a proper semantic versioning with X.Y.Z
     # let's hardcode 0.0.0
     __version__ = "0.0.0"
 
 __version_info__ = tuple(
```

### Comparing `qgis-plugin-manager-1.5.0/qgis_plugin_manager/__main__.py` & `qgis-plugin-manager-1.6.0/qgis_plugin_manager/__main__.py`

 * *Files identical despite different names*

### Comparing `qgis-plugin-manager-1.5.0/qgis_plugin_manager/definitions.py` & `qgis-plugin-manager-1.6.0/qgis_plugin_manager/definitions.py`

 * *Files identical despite different names*

### Comparing `qgis-plugin-manager-1.5.0/qgis_plugin_manager/local_directory.py` & `qgis-plugin-manager-1.6.0/qgis_plugin_manager/local_directory.py`

 * *Files identical despite different names*

### Comparing `qgis-plugin-manager-1.5.0/qgis_plugin_manager/remote.py` & `qgis-plugin-manager-1.6.0/qgis_plugin_manager/remote.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,21 +1,22 @@
 __copyright__ = 'Copyright 2022, 3Liz'
 __license__ = 'GPL version 3'
 __email__ = 'info@3liz.org'
 
+import base64
 import os
 import re
 import shutil
 import urllib
 import urllib.request
 import zipfile
 
 from pathlib import Path
 from typing import Dict, List, Optional, Tuple, Union
-from urllib.parse import unquote, urlparse
+from urllib.parse import unquote, urlencode, urlparse, urlunparse, parse_qs
 from xml.etree.ElementTree import parse
 
 from qgis_plugin_manager.definitions import Level, Plugin
 from qgis_plugin_manager.utils import (
     current_user,
     restart_qgis_server,
     similar_names,
@@ -140,15 +141,15 @@
     def print_list(self):
         """ Print in the console the list of remotes. """
         if self.list is None:
             self.remote_list()
 
         print("List of remotes :\n")
         if len(self.list):
-            print('\n'.join(self.list))
+            print('\n'.join([self.public_remote_name(s) for s in self.list]))
         else:
             print(f"{Level.Alert}No remote configured{Level.End}")
 
     def update(self) -> bool:
         """ For each remote, it updates the XML file. """
         if self.list is None:
             self.remote_list()
@@ -166,16 +167,23 @@
                 print(f"\t{Level.Critical}{e}{Level.End}")
                 return False
 
         cache.mkdir()
 
         flag = False
         for server in self.list:
-            print(f"Downloading {server}...")
-            request = urllib.request.Request(server, headers={'User-Agent': 'Mozilla/5.0'})
+            print(f"Downloading {self.public_remote_name(server)}…")
+            url, login, password = self.credentials(server)
+            headers = {
+                'User-Agent': 'Mozilla/5.0',
+            }
+            if login:
+                token = base64.b64encode(f"{login}:{password}".encode())
+                headers["Authorization"] = b"Basic %s" % token
+            request = urllib.request.Request(url, headers=headers)
             try:
                 f = urllib.request.urlopen(request)
             except urllib.error.HTTPError as e:
                 print(f"\t{e}")
                 continue
             except urllib.error.URLError as e:
                 print(f"\t{e}")
@@ -401,18 +409,39 @@
     ) -> Tuple[bool, Union[None, Path]]:
         """ Download the ZIP
         """
         if url.startswith('file:'):
             zip_file = Path(unquote(urlparse(url).path))
 
         else:
-            request = urllib.request.Request(url, headers={'User-Agent': 'Mozilla/5.0'})
+            headers = {
+                'User-Agent': 'Mozilla/5.0',
+            }
+            request = urllib.request.Request(url, headers=headers)
+            result = False
             try:
                 f = urllib.request.urlopen(request)
-            except urllib.error.HTTPError:
+                result = True
+            except urllib.error.HTTPError as e:
+                if e.code == 401:
+                    print("Require authentication")
+                    for _, login, password in self.all_credentials():
+                        # Hack to try all logins until we find the one working…
+                        token = base64.b64encode(f"{login}:{password}".encode())
+                        headers["Authorization"] = b"Basic %s" % token
+
+                        request = urllib.request.Request(url, headers=headers)
+                        try:
+                            f = urllib.request.urlopen(request)
+                            result = True
+                            break
+                        except urllib.error.HTTPError:
+                            continue
+
+            if not result:
                 print(f"{Level.Alert}Plugin {plugin_name} {version} not found.{Level.End}")
                 return False, None
 
             # Saving the zip from the URL
             zip_file = Path(self.folder / file_name)
 
             try:
@@ -447,16 +476,55 @@
                 f"{Level.End}"
             )
         return qgis_version
 
     @staticmethod
     def server_cache_filename(cache_folder, server) -> Path:
         """ Return the path for XML file. """
+        server, login, _ = Remote.credentials(server)
         filename = ""
         for x in server:
             if x.isalnum():
                 filename += x
             else:
                 filename += '-'
 
         filename = re.sub(r"\-+", "-", filename)
+        if login:
+            filename += '-protected'
         return Path(cache_folder / f"{filename}.xml")
+
+    @classmethod
+    def credentials(cls, server: str) -> Tuple[str, str, str]:
+        """ Parse for login and password if needed. """
+        u = urlparse(server)
+        query = parse_qs(u.query, keep_blank_values=True)
+        login = query.get('username', '')
+        password = query.get('password', '')
+
+        query.pop('username', None)
+        query.pop('password', None)
+
+        u = u._replace(query=urlencode(query, True))
+        if login and password:
+            return urlunparse(u), login[0], password[0]
+
+        return urlunparse(u), '', ''
+
+    def all_credentials(self):
+        """ Dirty hack to get all credentials for now… """
+        if self.list is None:
+            self.remote_list()
+
+        for server in self.list:
+            url, login, password = self.credentials(server)
+            yield url, login, password
+
+    @classmethod
+    def public_remote_name(cls, server: str) -> str:
+        """ Clean a URL from a password if needed. """
+        u = urlparse(server)
+        query = parse_qs(u.query, keep_blank_values=True)
+        if 'password' in query.keys():
+            query['password'] = 'XXXXX'
+        u = u._replace(query=urlencode(query, True))
+        return urlunparse(u)
```

### Comparing `qgis-plugin-manager-1.5.0/qgis_plugin_manager/utils.py` & `qgis-plugin-manager-1.6.0/qgis_plugin_manager/utils.py`

 * *Files identical despite different names*

### Comparing `qgis-plugin-manager-1.5.0/qgis_plugin_manager.egg-info/PKG-INFO` & `qgis-plugin-manager-1.6.0/qgis_plugin_manager.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 Metadata-Version: 2.1
 Name: qgis-plugin-manager
-Version: 1.5.0
+Version: 1.6.0
 Summary: Tool for downloading/managing QGIS plugins from CLI.
 Home-page: https://github.com/3liz/qgis-plugin-manager
-Download-URL: https://github.com/3liz/qgis-plugin-manager/archive/1.5.0.tar.gz
+Download-URL: https://github.com/3liz/qgis-plugin-manager/archive/1.6.0.tar.gz
 Author: Étienne Trimaille
 Author-email: etrimaille@3liz.com
 Project-URL: Docs, https://github.com/3liz/qgis-plugin-manager/blob/master/README.md
 Project-URL: Bug Reports, https://github.com/3liz/qgis-plugin-manager/issues/
 Project-URL: Source, https://github.com/3liz/qgis-plugin-manager
 Keywords: QGIS
 Classifier: Development Status :: 5 - Production/Stable
@@ -157,14 +157,25 @@
 `[VERSION]` is a token in the `sources.list` file to be replaced by the QGIS version, for instance `3.22`.
 If QGIS is upgraded, the XML file will be updated as well.
 
 You don't have to set the TOKEN for all URL : 
 
 `https://docs.3liz.org/plugins.xml` is valid.
 
+#### Basic authentication
+
+It's possible to add a login and password in the remote URL :
+
+```bash
+https://docs.3liz.org/private/repo.xml?username=loginwpd&password=pass
+```
+
+Every URL is parsed, and if some credentials are found, the URL is cleaned and the request is done using the
+basic authentication.
+
 ### Update
 
 To fetch the XML files from each repository :
 
 ```bash
 $ qgis-plugin-manager update
 Downloading https://plugins.qgis.org/plugins/plugins.xml?qgis=3.19...
@@ -250,17 +261,18 @@
 You can use `--force` or `-f` to force the upgrade for all plugins despite their version.
 
 *Note*, like APT, `update` is needed before to refresh the cache.
 
 #### Ignore plugins from the upgrade
 
 Some plugins might be installed by hand, without being installed with a remote. This command will try to upgrade
-**all valid** plugins found. However, the command will fail because the plugin has been installed without a remote.
+**all valid** plugins found in the directory. However, the command will fail because the plugin has been installed 
+without a remote.
 
-It's possible to ignore such plugin by adding a file `ignorePlugins.list`, next to the `sources.list` file,
+It's possible to ignore such plugin by adding a file `ignorePlugins.list`, in your plugins' folder,
 with a list of **plugin name** on each line. The `upgrade` will not try to upgrade them.
 
 ### Remove
 
 It's possible to use `rm -rf folder_dir` but you can also remove by the plugin name.
 It will take care of the `QGIS_PLUGINPATH` environment variable.
```

### Comparing `qgis-plugin-manager-1.5.0/qgis_plugin_manager.egg-info/SOURCES.txt` & `qgis-plugin-manager-1.6.0/qgis_plugin_manager.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `qgis-plugin-manager-1.5.0/setup.py` & `qgis-plugin-manager-1.6.0/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -16,15 +16,15 @@
     sys.exit(
         "qgis-plugin-manager requires at least Python version "
         f"{python_min_version[0]}.{python_min_version[1]}.\n"
         f"You are currently running this installation with\n\n{sys.version}"
     )
 
 # This string might be updated on CI on runtime with a proper semantic version name with X.Y.Z
-VERSION = "1.5.0"
+VERSION = "1.6.0"
 
 if "." not in VERSION:
     # If VERSION is still not a proper semantic versioning with X.Y.Z
     # let's hardcode 0.0.0
     VERSION = "0.0.0"
 
 read_me = Path(__file__).parent.joinpath("README.md").read_text(encoding='utf8')
```

### Comparing `qgis-plugin-manager-1.5.0/test/test_full_install.py` & `qgis-plugin-manager-1.6.0/test/test_full_install.py`

 * *Files identical despite different names*

### Comparing `qgis-plugin-manager-1.5.0/test/test_local.py` & `qgis-plugin-manager-1.6.0/test/test_local.py`

 * *Files identical despite different names*

### Comparing `qgis-plugin-manager-1.5.0/test/test_utils.py` & `qgis-plugin-manager-1.6.0/test/test_utils.py`

 * *Files identical despite different names*

