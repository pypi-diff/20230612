# Comparing `tmp/gh_subdir-1.0.1.tar.gz` & `tmp/gh_subdir-1.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "gh_subdir-1.0.1.tar", last modified: Mon Jun 12 07:41:10 2023, max compression
+gzip compressed data, was "gh_subdir-1.0.2.tar", last modified: Mon Jun 12 19:33:58 2023, max compression
```

## Comparing `gh_subdir-1.0.1.tar` & `gh_subdir-1.0.2.tar`

### file list

```diff
@@ -1,18 +1,18 @@
-drwxrwxrwx   0 rlvela    (1000) rlvela    (1000)        0 2023-06-12 07:41:10.962072 gh_subdir-1.0.1/
--rwxrwxrwx   0 rlvela    (1000) rlvela    (1000)    35823 2023-06-12 04:39:33.000000 gh_subdir-1.0.1/LICENSE
--rwxrwxrwx   0 rlvela    (1000) rlvela    (1000)     1815 2023-06-12 07:41:10.963072 gh_subdir-1.0.1/PKG-INFO
--rwxrwxrwx   0 rlvela    (1000) rlvela    (1000)     1003 2023-06-12 07:40:36.000000 gh_subdir-1.0.1/README.md
--rwxrwxrwx   0 rlvela    (1000) rlvela    (1000)       74 2023-06-12 07:41:10.971096 gh_subdir-1.0.1/setup.cfg
--rwxrwxrwx   0 rlvela    (1000) rlvela    (1000)      831 2023-06-12 07:41:06.000000 gh_subdir-1.0.1/setup.py
-drwxrwxrwx   0 rlvela    (1000) rlvela    (1000)        0 2023-06-12 07:41:10.915398 gh_subdir-1.0.1/src/
-drwxrwxrwx   0 rlvela    (1000) rlvela    (1000)        0 2023-06-12 07:41:10.938827 gh_subdir-1.0.1/src/gh_subdir/
--rwxrwxrwx   0 rlvela    (1000) rlvela    (1000)       38 2023-06-12 07:25:25.000000 gh_subdir-1.0.1/src/gh_subdir/__init__.py
-drwxrwxrwx   0 rlvela    (1000) rlvela    (1000)        0 2023-06-12 07:41:10.960075 gh_subdir-1.0.1/src/gh_subdir/tools/
--rwxrwxrwx   0 rlvela    (1000) rlvela    (1000)        0 2023-06-12 07:14:16.000000 gh_subdir-1.0.1/src/gh_subdir/tools/__init__.py
--rwxrwxrwx   0 rlvela    (1000) rlvela    (1000)     1968 2023-06-12 07:19:43.000000 gh_subdir-1.0.1/src/gh_subdir/tools/gh_subdir.py
-drwxrwxrwx   0 rlvela    (1000) rlvela    (1000)        0 2023-06-12 07:41:10.954073 gh_subdir-1.0.1/src/gh_subdir.egg-info/
--rwxrwxrwx   0 rlvela    (1000) rlvela    (1000)     1815 2023-06-12 07:41:10.000000 gh_subdir-1.0.1/src/gh_subdir.egg-info/PKG-INFO
--rwxrwxrwx   0 rlvela    (1000) rlvela    (1000)      311 2023-06-12 07:41:10.000000 gh_subdir-1.0.1/src/gh_subdir.egg-info/SOURCES.txt
--rwxrwxrwx   0 rlvela    (1000) rlvela    (1000)        1 2023-06-12 07:41:10.000000 gh_subdir-1.0.1/src/gh_subdir.egg-info/dependency_links.txt
--rwxrwxrwx   0 rlvela    (1000) rlvela    (1000)        9 2023-06-12 07:41:10.000000 gh_subdir-1.0.1/src/gh_subdir.egg-info/requires.txt
--rwxrwxrwx   0 rlvela    (1000) rlvela    (1000)       10 2023-06-12 07:41:10.000000 gh_subdir-1.0.1/src/gh_subdir.egg-info/top_level.txt
+drwxrwxrwx   0 rlvela    (1000) rlvela    (1000)        0 2023-06-12 19:33:58.624716 gh_subdir-1.0.2/
+-rwxrwxrwx   0 rlvela    (1000) rlvela    (1000)    35823 2023-06-12 04:39:33.000000 gh_subdir-1.0.2/LICENSE
+-rwxrwxrwx   0 rlvela    (1000) rlvela    (1000)     1815 2023-06-12 19:33:58.625711 gh_subdir-1.0.2/PKG-INFO
+-rwxrwxrwx   0 rlvela    (1000) rlvela    (1000)     1003 2023-06-12 07:40:36.000000 gh_subdir-1.0.2/README.md
+-rwxrwxrwx   0 rlvela    (1000) rlvela    (1000)       74 2023-06-12 19:33:58.634286 gh_subdir-1.0.2/setup.cfg
+-rwxrwxrwx   0 rlvela    (1000) rlvela    (1000)      831 2023-06-12 19:33:53.000000 gh_subdir-1.0.2/setup.py
+drwxrwxrwx   0 rlvela    (1000) rlvela    (1000)        0 2023-06-12 19:33:58.569278 gh_subdir-1.0.2/src/
+drwxrwxrwx   0 rlvela    (1000) rlvela    (1000)        0 2023-06-12 19:33:58.597505 gh_subdir-1.0.2/src/gh_subdir/
+-rwxrwxrwx   0 rlvela    (1000) rlvela    (1000)       38 2023-06-12 07:25:25.000000 gh_subdir-1.0.2/src/gh_subdir/__init__.py
+drwxrwxrwx   0 rlvela    (1000) rlvela    (1000)        0 2023-06-12 19:33:58.621711 gh_subdir-1.0.2/src/gh_subdir/tools/
+-rwxrwxrwx   0 rlvela    (1000) rlvela    (1000)        0 2023-06-12 07:14:16.000000 gh_subdir-1.0.2/src/gh_subdir/tools/__init__.py
+-rwxrwxrwx   0 rlvela    (1000) rlvela    (1000)     2107 2023-06-12 19:32:20.000000 gh_subdir-1.0.2/src/gh_subdir/tools/gh_subdir.py
+drwxrwxrwx   0 rlvela    (1000) rlvela    (1000)        0 2023-06-12 19:33:58.616711 gh_subdir-1.0.2/src/gh_subdir.egg-info/
+-rwxrwxrwx   0 rlvela    (1000) rlvela    (1000)     1815 2023-06-12 19:33:58.000000 gh_subdir-1.0.2/src/gh_subdir.egg-info/PKG-INFO
+-rwxrwxrwx   0 rlvela    (1000) rlvela    (1000)      311 2023-06-12 19:33:58.000000 gh_subdir-1.0.2/src/gh_subdir.egg-info/SOURCES.txt
+-rwxrwxrwx   0 rlvela    (1000) rlvela    (1000)        1 2023-06-12 19:33:58.000000 gh_subdir-1.0.2/src/gh_subdir.egg-info/dependency_links.txt
+-rwxrwxrwx   0 rlvela    (1000) rlvela    (1000)        9 2023-06-12 19:33:58.000000 gh_subdir-1.0.2/src/gh_subdir.egg-info/requires.txt
+-rwxrwxrwx   0 rlvela    (1000) rlvela    (1000)       10 2023-06-12 19:33:58.000000 gh_subdir-1.0.2/src/gh_subdir.egg-info/top_level.txt
```

### Comparing `gh_subdir-1.0.1/LICENSE` & `gh_subdir-1.0.2/LICENSE`

 * *Files identical despite different names*

### Comparing `gh_subdir-1.0.1/PKG-INFO` & `gh_subdir-1.0.2/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: gh_subdir
-Version: 1.0.1
+Version: 1.0.2
 Summary: A Python module for installing GitHub subdirectories.
 Home-page: https://github.com/reecevela/gh-subdir-py
 Author: Reece Vela
 Author-email: reecevela@outlook.com
 License: GPLv3
 Description: # gh_subdir
         Python module to install a subfolder of a github repo instead of the entire repo.
```

### Comparing `gh_subdir-1.0.1/README.md` & `gh_subdir-1.0.2/README.md`

 * *Files identical despite different names*

### Comparing `gh_subdir-1.0.1/setup.py` & `gh_subdir-1.0.2/setup.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from setuptools import setup, find_packages
 
 setup(
     name='gh_subdir',
-    version='1.0.1',
+    version='1.0.2',
     description='A Python module for installing GitHub subdirectories.',
     long_description=open('README.md').read(),
     long_description_content_type='text/markdown',
     author='Reece Vela',
     author_email='reecevela@outlook.com',
     url='https://github.com/reecevela/gh-subdir-py',
     packages=find_packages('src'),
```

### Comparing `gh_subdir-1.0.1/src/gh_subdir/tools/gh_subdir.py` & `gh_subdir-1.0.2/src/gh_subdir/tools/gh_subdir.py`

 * *Files 16% similar despite different names*

```diff
@@ -31,14 +31,17 @@
             if response.headers['Content-Type'].startswith('text'):
                 write_mode = 'w'
                 content = response.text
             else:
                 write_mode = 'wb'
                 content = response.content
 
-            if self.create_subfolder:
-                os.makedirs(base_path + '/' + relative_path, exist_ok=True)
-                with open(base_path + '/' + relative_path + '/' + url.split('/')[-1], write_mode, encoding=self.encoding) as file:
-                    file.write(content)
-            else:
-                with open(url.split('/')[-1], write_mode, encoding=self.encoding) as file:
-                    file.write(content)
+            try:
+                if self.create_subfolder:
+                    os.makedirs(base_path + '/' + relative_path, exist_ok=True)
+                    with open(base_path + '/' + relative_path + '/' + url.split('/')[-1], write_mode, encoding=self.encoding) as file:
+                        file.write(content)
+                else:
+                    with open(url.split('/')[-1], write_mode, encoding=self.encoding) as file:
+                        file.write(content)
+            except Exception as e:
+                print(f"Failed to download {url}: {e}")
```

### Comparing `gh_subdir-1.0.1/src/gh_subdir.egg-info/PKG-INFO` & `gh_subdir-1.0.2/src/gh_subdir.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: gh-subdir
-Version: 1.0.1
+Version: 1.0.2
 Summary: A Python module for installing GitHub subdirectories.
 Home-page: https://github.com/reecevela/gh-subdir-py
 Author: Reece Vela
 Author-email: reecevela@outlook.com
 License: GPLv3
 Description: # gh_subdir
         Python module to install a subfolder of a github repo instead of the entire repo.
```

