# Comparing `tmp/discord-2.2.3.tar.gz` & `tmp/discord-2.3.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "discord-2.2.3.tar", last modified: Mon May  1 22:44:53 2023, max compression
+gzip compressed data, was "discord-2.3.0.tar", last modified: Mon Jun 12 18:08:14 2023, max compression
```

## Comparing `discord-2.2.3.tar` & `discord-2.3.0.tar`

### file list

```diff
@@ -1,11 +1,11 @@
-drwxrwxrwx   0        0        0        0 2023-05-01 22:44:53.302195 discord-2.2.3/
--rw-rw-rw-   0        0        0      360 2023-05-01 22:44:53.302195 discord-2.2.3/PKG-INFO
--rw-rw-rw-   0        0        0       82 2021-06-10 01:32:34.000000 discord-2.2.3/README.md
-drwxrwxrwx   0        0        0        0 2023-05-01 22:44:53.301194 discord-2.2.3/discord.egg-info/
--rw-rw-rw-   0        0        0      360 2023-05-01 22:44:53.000000 discord-2.2.3/discord.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      172 2023-05-01 22:44:53.000000 discord-2.2.3/discord.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-05-01 22:44:53.000000 discord-2.2.3/discord.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       18 2023-05-01 22:44:53.000000 discord-2.2.3/discord.egg-info/requires.txt
--rw-rw-rw-   0        0        0        1 2023-05-01 22:44:53.000000 discord-2.2.3/discord.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-05-01 22:44:53.303196 discord-2.2.3/setup.cfg
--rw-rw-rw-   0        0        0      562 2023-05-01 22:44:41.000000 discord-2.2.3/setup.py
+drwxrwxrwx   0        0        0        0 2023-06-12 18:08:14.352134 discord-2.3.0/
+-rw-rw-rw-   0        0        0      360 2023-06-12 18:08:14.351133 discord-2.3.0/PKG-INFO
+-rw-rw-rw-   0        0        0       82 2021-06-10 01:32:34.000000 discord-2.3.0/README.md
+drwxrwxrwx   0        0        0        0 2023-06-12 18:08:14.350132 discord-2.3.0/discord.egg-info/
+-rw-rw-rw-   0        0        0      360 2023-06-12 18:08:14.000000 discord-2.3.0/discord.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      172 2023-06-12 18:08:14.000000 discord-2.3.0/discord.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-06-12 18:08:14.000000 discord-2.3.0/discord.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       18 2023-06-12 18:08:14.000000 discord-2.3.0/discord.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        1 2023-06-12 18:08:14.000000 discord-2.3.0/discord.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-06-12 18:08:14.352134 discord-2.3.0/setup.cfg
+-rw-rw-rw-   0        0        0      562 2023-06-12 18:01:57.000000 discord-2.3.0/setup.py
```

### Comparing `discord-2.2.3/setup.py` & `discord-2.3.0/setup.py`

 * *Files 3% similar despite different names*

```diff
@@ -3,16 +3,16 @@
 from os import path
 this_directory = path.abspath(path.dirname(__file__))
 with open(path.join(this_directory, 'README.md'), encoding='utf-8') as f:
     long_description = f.read()
 
 setup(
     name='discord',
-    version='2.2.3',
+    version='2.3.0',
     url='https://github.com/Rapptz/discord.py',
     author='Rapptz',
     description='A mirror package for discord.py. Please install that instead.',
     long_description=long_description,
     long_description_content_type='text/markdown',
     packages=[],
-    install_requires=['discord.py>=2.2.3'],
+    install_requires=['discord.py>=2.3.0'],
 )
```

