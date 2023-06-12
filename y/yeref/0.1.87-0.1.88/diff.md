# Comparing `tmp/yeref-0.1.87.tar.gz` & `tmp/yeref-0.1.88.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "yeref-0.1.87.tar", last modified: Sun Jun 11 16:06:45 2023, max compression
+gzip compressed data, was "yeref-0.1.88.tar", last modified: Mon Jun 12 09:30:17 2023, max compression
```

## Comparing `yeref-0.1.87.tar` & `yeref-0.1.88.tar`

### file list

```diff
@@ -1,13 +1,13 @@
-drwxr-xr-x   0 mark       (501) staff       (20)        0 2023-06-11 16:06:45.474534 yeref-0.1.87/
--rw-r--r--   0 mark       (501) staff       (20)       85 2023-06-11 16:06:45.474773 yeref-0.1.87/PKG-INFO
--rw-r--r--   0 mark       (501) staff       (20)       38 2023-06-11 16:06:45.475723 yeref-0.1.87/setup.cfg
--rw-r--r--   0 mark       (501) staff       (20)     1391 2023-06-11 16:06:23.000000 yeref-0.1.87/setup.py
-drwxr-xr-x   0 mark       (501) staff       (20)        0 2023-06-11 16:06:45.466133 yeref-0.1.87/yeref/
--rw-r--r--   0 mark       (501) staff       (20)       39 2023-04-21 17:52:00.000000 yeref-0.1.87/yeref/__init__.py
--rw-r--r--   0 mark       (501) staff       (20)   553500 2023-06-11 15:47:28.000000 yeref-0.1.87/yeref/l_.py
--rw-r--r--   0 mark       (501) staff       (20)   213622 2023-06-11 16:06:12.000000 yeref-0.1.87/yeref/yeref.py
-drwxr-xr-x   0 mark       (501) staff       (20)        0 2023-06-11 16:06:45.473737 yeref-0.1.87/yeref.egg-info/
--rw-r--r--   0 mark       (501) staff       (20)       85 2023-06-11 16:06:45.000000 yeref-0.1.87/yeref.egg-info/PKG-INFO
--rw-r--r--   0 mark       (501) staff       (20)      179 2023-06-11 16:06:45.000000 yeref-0.1.87/yeref.egg-info/SOURCES.txt
--rw-r--r--   0 mark       (501) staff       (20)        1 2023-06-11 16:06:45.000000 yeref-0.1.87/yeref.egg-info/dependency_links.txt
--rw-r--r--   0 mark       (501) staff       (20)        6 2023-06-11 16:06:45.000000 yeref-0.1.87/yeref.egg-info/top_level.txt
+drwxr-xr-x   0 mark       (501) staff       (20)        0 2023-06-12 09:30:17.522991 yeref-0.1.88/
+-rw-r--r--   0 mark       (501) staff       (20)       85 2023-06-12 09:30:17.523251 yeref-0.1.88/PKG-INFO
+-rw-r--r--   0 mark       (501) staff       (20)       38 2023-06-12 09:30:17.523927 yeref-0.1.88/setup.cfg
+-rw-r--r--   0 mark       (501) staff       (20)     1391 2023-06-12 09:30:05.000000 yeref-0.1.88/setup.py
+drwxr-xr-x   0 mark       (501) staff       (20)        0 2023-06-12 09:30:17.514697 yeref-0.1.88/yeref/
+-rw-r--r--   0 mark       (501) staff       (20)       39 2023-04-21 17:52:00.000000 yeref-0.1.88/yeref/__init__.py
+-rw-r--r--   0 mark       (501) staff       (20)   553500 2023-06-11 15:47:28.000000 yeref-0.1.88/yeref/l_.py
+-rw-r--r--   0 mark       (501) staff       (20)   214041 2023-06-12 09:27:25.000000 yeref-0.1.88/yeref/yeref.py
+drwxr-xr-x   0 mark       (501) staff       (20)        0 2023-06-12 09:30:17.522269 yeref-0.1.88/yeref.egg-info/
+-rw-r--r--   0 mark       (501) staff       (20)       85 2023-06-12 09:30:17.000000 yeref-0.1.88/yeref.egg-info/PKG-INFO
+-rw-r--r--   0 mark       (501) staff       (20)      179 2023-06-12 09:30:17.000000 yeref-0.1.88/yeref.egg-info/SOURCES.txt
+-rw-r--r--   0 mark       (501) staff       (20)        1 2023-06-12 09:30:17.000000 yeref-0.1.88/yeref.egg-info/dependency_links.txt
+-rw-r--r--   0 mark       (501) staff       (20)        6 2023-06-12 09:30:17.000000 yeref-0.1.88/yeref.egg-info/top_level.txt
```

### Comparing `yeref-0.1.87/setup.py` & `yeref-0.1.88/setup.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from setuptools import setup
 
 setup(
       name='yeref',
-      version='0.1.87',
+      version='0.1.88',
       description='desc-f',
       author='john smith',
       packages=['yeref'],
       # install_requires=[
       #       "httplib2>=0.20.4",
       #       "moviepy>=1.0.3",
       #       "Pillow>=9.2.0",
```

### Comparing `yeref-0.1.87/yeref/l_.py` & `yeref-0.1.88/yeref/l_.py`

 * *Files identical despite different names*

### Comparing `yeref-0.1.87/yeref/yeref.py` & `yeref-0.1.88/yeref/yeref.py`

 * *Files 0% similar despite different names*

```diff
@@ -742,14 +742,29 @@
         logger.info(log_ % f"TelegramRetryAfter {e.retry_after}")
         await asyncio.sleep(e.retry_after + 1)
     except Exception as e:
         logger.info(log_ % str(e))
         await asyncio.sleep(round(random.uniform(0, 1), 2))
 
 
+async def in_ban_list(tid, username=None):
+    result = False
+    try:
+        # 68728482 yagupov
+        b_ids = [68728482, ]
+
+        if username and username.startswith('kwprod'):
+            result = True
+        elif tid in b_ids:
+            result = True
+    except Exception as e:
+        logger.info(log_ % str(e))
+        await asyncio.sleep(round(random.uniform(0, 1), 2))
+    finally:
+        return result
 # endregion
 
 
 # region admin
 async def pre_upload(bot, chat_id, media_name, media_type, EXTRA_D, BASE_D):
     result = None
     try:
```

