# Comparing `tmp/yeref-0.1.89.tar.gz` & `tmp/yeref-0.1.90.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "yeref-0.1.89.tar", last modified: Mon Jun 12 10:46:35 2023, max compression
+gzip compressed data, was "yeref-0.1.90.tar", last modified: Mon Jun 12 11:55:24 2023, max compression
```

## Comparing `yeref-0.1.89.tar` & `yeref-0.1.90.tar`

### file list

```diff
@@ -1,13 +1,13 @@
-drwxr-xr-x   0 mark       (501) staff       (20)        0 2023-06-12 10:46:35.786374 yeref-0.1.89/
--rw-r--r--   0 mark       (501) staff       (20)       85 2023-06-12 10:46:35.786525 yeref-0.1.89/PKG-INFO
--rw-r--r--   0 mark       (501) staff       (20)       38 2023-06-12 10:46:35.787134 yeref-0.1.89/setup.cfg
--rw-r--r--   0 mark       (501) staff       (20)     1391 2023-06-12 10:46:23.000000 yeref-0.1.89/setup.py
-drwxr-xr-x   0 mark       (501) staff       (20)        0 2023-06-12 10:46:35.782143 yeref-0.1.89/yeref/
--rw-r--r--   0 mark       (501) staff       (20)       39 2023-04-21 17:52:00.000000 yeref-0.1.89/yeref/__init__.py
--rw-r--r--   0 mark       (501) staff       (20)   553500 2023-06-11 15:47:28.000000 yeref-0.1.89/yeref/l_.py
--rw-r--r--   0 mark       (501) staff       (20)   213847 2023-06-12 10:46:23.000000 yeref-0.1.89/yeref/yeref.py
-drwxr-xr-x   0 mark       (501) staff       (20)        0 2023-06-12 10:46:35.785973 yeref-0.1.89/yeref.egg-info/
--rw-r--r--   0 mark       (501) staff       (20)       85 2023-06-12 10:46:35.000000 yeref-0.1.89/yeref.egg-info/PKG-INFO
--rw-r--r--   0 mark       (501) staff       (20)      179 2023-06-12 10:46:35.000000 yeref-0.1.89/yeref.egg-info/SOURCES.txt
--rw-r--r--   0 mark       (501) staff       (20)        1 2023-06-12 10:46:35.000000 yeref-0.1.89/yeref.egg-info/dependency_links.txt
--rw-r--r--   0 mark       (501) staff       (20)        6 2023-06-12 10:46:35.000000 yeref-0.1.89/yeref.egg-info/top_level.txt
+drwxr-xr-x   0 mark       (501) staff       (20)        0 2023-06-12 11:55:24.148914 yeref-0.1.90/
+-rw-r--r--   0 mark       (501) staff       (20)       85 2023-06-12 11:55:24.149176 yeref-0.1.90/PKG-INFO
+-rw-r--r--   0 mark       (501) staff       (20)       38 2023-06-12 11:55:24.150263 yeref-0.1.90/setup.cfg
+-rw-r--r--   0 mark       (501) staff       (20)     1391 2023-06-12 11:55:02.000000 yeref-0.1.90/setup.py
+drwxr-xr-x   0 mark       (501) staff       (20)        0 2023-06-12 11:55:24.145353 yeref-0.1.90/yeref/
+-rw-r--r--   0 mark       (501) staff       (20)       39 2023-04-21 17:52:00.000000 yeref-0.1.90/yeref/__init__.py
+-rw-r--r--   0 mark       (501) staff       (20)   553500 2023-06-11 15:47:28.000000 yeref-0.1.90/yeref/l_.py
+-rw-r--r--   0 mark       (501) staff       (20)   213869 2023-06-12 11:47:33.000000 yeref-0.1.90/yeref/yeref.py
+drwxr-xr-x   0 mark       (501) staff       (20)        0 2023-06-12 11:55:24.148488 yeref-0.1.90/yeref.egg-info/
+-rw-r--r--   0 mark       (501) staff       (20)       85 2023-06-12 11:55:24.000000 yeref-0.1.90/yeref.egg-info/PKG-INFO
+-rw-r--r--   0 mark       (501) staff       (20)      179 2023-06-12 11:55:24.000000 yeref-0.1.90/yeref.egg-info/SOURCES.txt
+-rw-r--r--   0 mark       (501) staff       (20)        1 2023-06-12 11:55:24.000000 yeref-0.1.90/yeref.egg-info/dependency_links.txt
+-rw-r--r--   0 mark       (501) staff       (20)        6 2023-06-12 11:55:24.000000 yeref-0.1.90/yeref.egg-info/top_level.txt
```

### Comparing `yeref-0.1.89/setup.py` & `yeref-0.1.90/setup.py`

 * *Files 17% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from setuptools import setup
 
 setup(
       name='yeref',
-      version='0.1.89',
+      version='0.1.90',
       description='desc-f',
       author='john smith',
       packages=['yeref'],
       # install_requires=[
       #       "httplib2>=0.20.4",
       #       "moviepy>=1.0.3",
       #       "Pillow>=9.2.0",
```

### Comparing `yeref-0.1.89/yeref/l_.py` & `yeref-0.1.90/yeref/l_.py`

 * *Files identical despite different names*

### Comparing `yeref-0.1.89/yeref/yeref.py` & `yeref-0.1.90/yeref/yeref.py`

 * *Files 0% similar despite different names*

```diff
@@ -4819,34 +4819,34 @@
 
 
 # region payment
 async def update_subscribe(bot, BASE_D):
     try:
         dt_ = datetime.datetime.utcnow()
         if not (dt_.hour % 2 == 0 and dt_.minute % 2 == 0 and dt_.second % 2 == 0): return
-        sql = "SELECT USER_TID, USER_LZ, USER_PAYDT FROM USER WHERE USER_ISPAID=1"
+        sql = "SELECT USER_TID, USER_LZ, USER_DTPAID FROM USER WHERE USER_ISPAID=1"
         data = await db_select(sql, (), BASE_D)
 
         for item in data:
             try:
                 await asyncio.sleep(round(random.uniform(0, 1), 2))
-                USER_TID, USER_LZ, USER_PAYDT = item
+                USER_TID, USER_LZ, USER_DTPAID = item
                 get_ = await bot.get_chat(chat_id=USER_TID)
 
-                if (dt_ - datetime.datetime.strptime(USER_PAYDT, '%d-%m-%Y_%H-%M-%S')).days > 32:
+                if USER_DTPAID and (dt_ - datetime.datetime.strptime(USER_DTPAID, '%d-%m-%Y_%H-%M-%S')).days > 31:
                     chan_private_donate = channel_library_ru if USER_LZ == 'ru' else channel_library_en
                     extra_bot = Bot(token=BOT_TOKEN_E18B)
                     get_chat_member_ = await extra_bot.get_chat_member(chat_id=chan_private_donate, user_id=USER_TID)
                     await extra_bot.session.close()
 
                     if get_chat_member_.status in ['member', 'administrator', 'creator']:
-                        USER_PAYDT = datetime.datetime.utcnow().strftime('%d-%m-%Y_%H-%M-%S')
-                        sql = "UPDATE USER SET USER_ISPAID=1, USER_USERNAME=?, USER_FULLNAME=?, USER_PAYDT=? " \
+                        USER_DTPAID = datetime.datetime.utcnow().strftime('%d-%m-%Y_%H-%M-%S')
+                        sql = "UPDATE USER SET USER_ISPAID=1, USER_USERNAME=?, USER_FULLNAME=?, USER_DTPAID=? " \
                               "WHERE USER_TID=?"
-                        await db_change(sql, (get_.username, get_.full_name, USER_PAYDT, USER_TID,), BASE_D)
+                        await db_change(sql, (get_.username, get_.full_name, USER_DTPAID, USER_TID,), BASE_D)
                     else:
                         sql = "UPDATE USER SET USER_ISPAID=0, USER_USERNAME=?, USER_FULLNAME=? WHERE USER_TID=?"
                         await db_change(sql, (get_.username, get_.full_name, USER_TID, ), BASE_D)
                 else:
                     sql = "UPDATE USER SET USER_USERNAME=?, USER_FULLNAME=? WHERE USER_TID=?"
                     await db_change(sql, (get_.username, get_.full_name, USER_TID,), BASE_D)
             except TelegramRetryAfter as e:
```

