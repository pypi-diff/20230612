# Comparing `tmp/yeref-0.1.88.tar.gz` & `tmp/yeref-0.1.89.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "yeref-0.1.88.tar", last modified: Mon Jun 12 09:30:17 2023, max compression
+gzip compressed data, was "yeref-0.1.89.tar", last modified: Mon Jun 12 10:46:35 2023, max compression
```

## Comparing `yeref-0.1.88.tar` & `yeref-0.1.89.tar`

### file list

```diff
@@ -1,13 +1,13 @@
-drwxr-xr-x   0 mark       (501) staff       (20)        0 2023-06-12 09:30:17.522991 yeref-0.1.88/
--rw-r--r--   0 mark       (501) staff       (20)       85 2023-06-12 09:30:17.523251 yeref-0.1.88/PKG-INFO
--rw-r--r--   0 mark       (501) staff       (20)       38 2023-06-12 09:30:17.523927 yeref-0.1.88/setup.cfg
--rw-r--r--   0 mark       (501) staff       (20)     1391 2023-06-12 09:30:05.000000 yeref-0.1.88/setup.py
-drwxr-xr-x   0 mark       (501) staff       (20)        0 2023-06-12 09:30:17.514697 yeref-0.1.88/yeref/
--rw-r--r--   0 mark       (501) staff       (20)       39 2023-04-21 17:52:00.000000 yeref-0.1.88/yeref/__init__.py
--rw-r--r--   0 mark       (501) staff       (20)   553500 2023-06-11 15:47:28.000000 yeref-0.1.88/yeref/l_.py
--rw-r--r--   0 mark       (501) staff       (20)   214041 2023-06-12 09:27:25.000000 yeref-0.1.88/yeref/yeref.py
-drwxr-xr-x   0 mark       (501) staff       (20)        0 2023-06-12 09:30:17.522269 yeref-0.1.88/yeref.egg-info/
--rw-r--r--   0 mark       (501) staff       (20)       85 2023-06-12 09:30:17.000000 yeref-0.1.88/yeref.egg-info/PKG-INFO
--rw-r--r--   0 mark       (501) staff       (20)      179 2023-06-12 09:30:17.000000 yeref-0.1.88/yeref.egg-info/SOURCES.txt
--rw-r--r--   0 mark       (501) staff       (20)        1 2023-06-12 09:30:17.000000 yeref-0.1.88/yeref.egg-info/dependency_links.txt
--rw-r--r--   0 mark       (501) staff       (20)        6 2023-06-12 09:30:17.000000 yeref-0.1.88/yeref.egg-info/top_level.txt
+drwxr-xr-x   0 mark       (501) staff       (20)        0 2023-06-12 10:46:35.786374 yeref-0.1.89/
+-rw-r--r--   0 mark       (501) staff       (20)       85 2023-06-12 10:46:35.786525 yeref-0.1.89/PKG-INFO
+-rw-r--r--   0 mark       (501) staff       (20)       38 2023-06-12 10:46:35.787134 yeref-0.1.89/setup.cfg
+-rw-r--r--   0 mark       (501) staff       (20)     1391 2023-06-12 10:46:23.000000 yeref-0.1.89/setup.py
+drwxr-xr-x   0 mark       (501) staff       (20)        0 2023-06-12 10:46:35.782143 yeref-0.1.89/yeref/
+-rw-r--r--   0 mark       (501) staff       (20)       39 2023-04-21 17:52:00.000000 yeref-0.1.89/yeref/__init__.py
+-rw-r--r--   0 mark       (501) staff       (20)   553500 2023-06-11 15:47:28.000000 yeref-0.1.89/yeref/l_.py
+-rw-r--r--   0 mark       (501) staff       (20)   213847 2023-06-12 10:46:23.000000 yeref-0.1.89/yeref/yeref.py
+drwxr-xr-x   0 mark       (501) staff       (20)        0 2023-06-12 10:46:35.785973 yeref-0.1.89/yeref.egg-info/
+-rw-r--r--   0 mark       (501) staff       (20)       85 2023-06-12 10:46:35.000000 yeref-0.1.89/yeref.egg-info/PKG-INFO
+-rw-r--r--   0 mark       (501) staff       (20)      179 2023-06-12 10:46:35.000000 yeref-0.1.89/yeref.egg-info/SOURCES.txt
+-rw-r--r--   0 mark       (501) staff       (20)        1 2023-06-12 10:46:35.000000 yeref-0.1.89/yeref.egg-info/dependency_links.txt
+-rw-r--r--   0 mark       (501) staff       (20)        6 2023-06-12 10:46:35.000000 yeref-0.1.89/yeref.egg-info/top_level.txt
```

### Comparing `yeref-0.1.88/setup.py` & `yeref-0.1.89/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from setuptools import setup
 
 setup(
       name='yeref',
-      version='0.1.88',
+      version='0.1.89',
       description='desc-f',
       author='john smith',
       packages=['yeref'],
       # install_requires=[
       #       "httplib2>=0.20.4",
       #       "moviepy>=1.0.3",
       #       "Pillow>=9.2.0",
```

### Comparing `yeref-0.1.88/yeref/l_.py` & `yeref-0.1.89/yeref/l_.py`

 * *Files identical despite different names*

### Comparing `yeref-0.1.88/yeref/yeref.py` & `yeref-0.1.89/yeref/yeref.py`

 * *Files 0% similar despite different names*

```diff
@@ -159,17 +159,14 @@
     [types.KeyboardButton(text='⬅️ Prev'), types.KeyboardButton(text='↩️ Menu'),
      types.KeyboardButton(text='➡️️ Next')]], resize_keyboard=True, selective=True, row_width=3)
 
 BOT_VARS_ = '{"BOT_PROMO": "#911", "BOT_CHANNEL": 0, "BOT_CHANNELTID": 0, "BOT_GROUP": 0, "BOT_GROUPTID": 0, "BOT_TZ": 0, "BOT_TZ": 0, "BOT_LZ": "en", "BOT_LC": "en"}'
 BOT_LSTS_ = '{"BOT_ADMINS": []}'
 USER_VARS_ = '{"USER_TEXT": "", "USER_EMAIL": "", "USER_PROMO": "", "USER_PHONE": "", "USER_GEO": "", "USER_UTM": "", "USER_ID": 0, "USER_DT": "", "USER_TZ": 0, "USER_LC": "en", "USER_ISADMIN": 0, "USER_ISPREMIUM": 0, "USER_BALL": 0, "USER_RAND": 0, "USER_QUIZ": 0, "USER_DICE": 0, "USER_PAY": 0, "DATE_TIME": 0}'
 USER_LSTS_ = '{"USER_UTMREF": []}'
-
-logger.add('debug.log', format="{time:DD-MM-YYYY HH:mm:ss} | {name}({line}): {message}", level="INFO",
-           colorize=True, enqueue=True, backtrace=True, diagnose=True, rotation="1 week")
 # endregion
 
 
 # region db
 def sqlite_lower(value_):
     return value_.lower() if value_ else None
```

