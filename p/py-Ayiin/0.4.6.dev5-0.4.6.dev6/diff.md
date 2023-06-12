# Comparing `tmp/py-Ayiin-0.4.6.dev5.tar.gz` & `tmp/py-Ayiin-0.4.6.dev6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "py-Ayiin-0.4.6.dev5.tar", last modified: Mon Jun 12 16:36:09 2023, max compression
+gzip compressed data, was "py-Ayiin-0.4.6.dev6.tar", last modified: Mon Jun 12 16:42:01 2023, max compression
```

## Comparing `py-Ayiin-0.4.6.dev5.tar` & `py-Ayiin-0.4.6.dev6.tar`

### file list

```diff
@@ -1,88 +1,88 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-12 16:36:09.986822 py-Ayiin-0.4.6.dev5/
--rw-r--r--   0 runner    (1001) docker     (123)    35149 2023-06-12 16:36:00.000000 py-Ayiin-0.4.6.dev5/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)      147 2023-06-12 16:36:00.000000 py-Ayiin-0.4.6.dev5/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)      775 2023-06-12 16:36:00.000000 py-Ayiin-0.4.6.dev5/NOTICE
--rw-r--r--   0 runner    (1001) docker     (123)     2572 2023-06-12 16:36:09.986822 py-Ayiin-0.4.6.dev5/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1642 2023-06-12 16:36:00.000000 py-Ayiin-0.4.6.dev5/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-12 16:36:09.978822 py-Ayiin-0.4.6.dev5/pyAyiin/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-12 16:36:09.978822 py-Ayiin-0.4.6.dev5/pyAyiin/Clients/
--rw-r--r--   0 runner    (1001) docker     (123)      639 2023-06-12 16:36:00.000000 py-Ayiin-0.4.6.dev5/pyAyiin/Clients/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    12525 2023-06-12 16:36:00.000000 py-Ayiin-0.4.6.dev5/pyAyiin/Clients/client.py
--rw-r--r--   0 runner    (1001) docker     (123)     6295 2023-06-12 16:36:00.000000 py-Ayiin-0.4.6.dev5/pyAyiin/Clients/pytgcalls.py
--rw-r--r--   0 runner    (1001) docker     (123)    38781 2023-06-12 16:36:00.000000 py-Ayiin-0.4.6.dev5/pyAyiin/Clients/startup.py
--rw-r--r--   0 runner    (1001) docker     (123)     4570 2023-06-12 16:36:00.000000 py-Ayiin-0.4.6.dev5/pyAyiin/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1505 2023-06-12 16:36:00.000000 py-Ayiin-0.4.6.dev5/pyAyiin/__main__.py
--rw-r--r--   0 runner    (1001) docker     (123)     6704 2023-06-12 16:36:00.000000 py-Ayiin-0.4.6.dev5/pyAyiin/assistant.py
--rw-r--r--   0 runner    (1001) docker     (123)     5126 2023-06-12 16:36:00.000000 py-Ayiin-0.4.6.dev5/pyAyiin/config.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-12 16:36:09.982822 py-Ayiin-0.4.6.dev5/pyAyiin/dB/
--rw-r--r--   0 runner    (1001) docker     (123)     1388 2023-06-12 16:36:00.000000 py-Ayiin-0.4.6.dev5/pyAyiin/dB/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      170 2023-06-12 16:36:00.000000 py-Ayiin-0.4.6.dev5/pyAyiin/dB/_core.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-12 16:36:00.000000 py-Ayiin-0.4.6.dev5/pyAyiin/dB/_session.py
--rw-r--r--   0 runner    (1001) docker     (123)     1330 2023-06-12 16:36:00.000000 py-Ayiin-0.4.6.dev5/pyAyiin/dB/absen.py
--rw-r--r--   0 runner    (1001) docker     (123)      816 2023-06-12 16:36:00.000000 py-Ayiin-0.4.6.dev5/pyAyiin/dB/admins.py
--rw-r--r--   0 runner    (1001) docker     (123)     2255 2023-06-12 16:36:00.000000 py-Ayiin-0.4.6.dev5/pyAyiin/dB/auth.py
--rw-r--r--   0 runner    (1001) docker     (123)     1406 2023-06-12 16:36:00.000000 py-Ayiin-0.4.6.dev5/pyAyiin/dB/blacklistfilter.py
--rw-r--r--   0 runner    (1001) docker     (123)     1164 2023-06-12 16:36:00.000000 py-Ayiin-0.4.6.dev5/pyAyiin/dB/blacklistgcast.py
--rw-r--r--   0 runner    (1001) docker     (123)      783 2023-06-12 16:36:00.000000 py-Ayiin-0.4.6.dev5/pyAyiin/dB/blacklistuser.py
--rw-r--r--   0 runner    (1001) docker     (123)      706 2023-06-12 16:36:00.000000 py-Ayiin-0.4.6.dev5/pyAyiin/dB/gban.py
--rw-r--r--   0 runner    (1001) docker     (123)     1271 2023-06-12 16:36:00.000000 py-Ayiin-0.4.6.dev5/pyAyiin/dB/langs.py
--rw-r--r--   0 runner    (1001) docker     (123)     1049 2023-06-12 16:36:00.000000 py-Ayiin-0.4.6.dev5/pyAyiin/dB/logdb.py
--rw-r--r--   0 runner    (1001) docker     (123)     4755 2023-06-12 16:36:00.000000 py-Ayiin-0.4.6.dev5/pyAyiin/dB/pmpermit.py
--rw-r--r--   0 runner    (1001) docker     (123)     1331 2023-06-12 16:36:00.000000 py-Ayiin-0.4.6.dev5/pyAyiin/dB/premium.py
--rw-r--r--   0 runner    (1001) docker     (123)      914 2023-06-12 16:36:00.000000 py-Ayiin-0.4.6.dev5/pyAyiin/dB/start.py
--rw-r--r--   0 runner    (1001) docker     (123)     1006 2023-06-12 16:36:00.000000 py-Ayiin-0.4.6.dev5/pyAyiin/dB/sudo.py
--rw-r--r--   0 runner    (1001) docker     (123)      746 2023-06-12 16:36:00.000000 py-Ayiin-0.4.6.dev5/pyAyiin/dB/variable.py
--rw-r--r--   0 runner    (1001) docker     (123)     1251 2023-06-12 16:36:00.000000 py-Ayiin-0.4.6.dev5/pyAyiin/dB/videocalls.py
--rw-r--r--   0 runner    (1001) docker     (123)     2012 2023-06-12 16:36:00.000000 py-Ayiin-0.4.6.dev5/pyAyiin/dB/welcome.py
--rw-r--r--   0 runner    (1001) docker     (123)    33973 2023-06-12 16:36:00.000000 py-Ayiin-0.4.6.dev5/pyAyiin/decorator.py
--rw-r--r--   0 runner    (1001) docker     (123)      959 2023-06-12 16:36:00.000000 py-Ayiin-0.4.6.dev5/pyAyiin/exceptions.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-12 16:36:09.982822 py-Ayiin-0.4.6.dev5/pyAyiin/methods/
--rw-r--r--   0 runner    (1001) docker     (123)      954 2023-06-12 16:36:00.000000 py-Ayiin-0.4.6.dev5/pyAyiin/methods/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    10094 2023-06-12 16:36:00.000000 py-Ayiin-0.4.6.dev5/pyAyiin/methods/_database.py
--rw-r--r--   0 runner    (1001) docker     (123)     3939 2023-06-12 16:36:00.000000 py-Ayiin-0.4.6.dev5/pyAyiin/methods/_misc.py
--rw-r--r--   0 runner    (1001) docker     (123)     1897 2023-06-12 16:36:00.000000 py-Ayiin-0.4.6.dev5/pyAyiin/methods/changer.py
--rw-r--r--   0 runner    (1001) docker     (123)      853 2023-06-12 16:36:00.000000 py-Ayiin-0.4.6.dev5/pyAyiin/methods/converter.py
--rw-r--r--   0 runner    (1001) docker     (123)     6909 2023-06-12 16:36:00.000000 py-Ayiin-0.4.6.dev5/pyAyiin/methods/func.py
--rw-r--r--   0 runner    (1001) docker     (123)    10022 2023-06-12 16:36:00.000000 py-Ayiin-0.4.6.dev5/pyAyiin/methods/funcb.py
--rw-r--r--   0 runner    (1001) docker     (123)     8828 2023-06-12 16:36:00.000000 py-Ayiin-0.4.6.dev5/pyAyiin/methods/helpers.py
--rw-r--r--   0 runner    (1001) docker     (123)     1213 2023-06-12 16:36:00.000000 py-Ayiin-0.4.6.dev5/pyAyiin/methods/hosting.py
--rw-r--r--   0 runner    (1001) docker     (123)     7703 2023-06-12 16:36:00.000000 py-Ayiin-0.4.6.dev5/pyAyiin/methods/inlinebot.py
--rw-r--r--   0 runner    (1001) docker     (123)     2879 2023-06-12 16:36:00.000000 py-Ayiin-0.4.6.dev5/pyAyiin/methods/queue.py
--rw-r--r--   0 runner    (1001) docker     (123)     6067 2023-06-12 16:36:00.000000 py-Ayiin-0.4.6.dev5/pyAyiin/methods/thumbnail.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-12 16:36:09.982822 py-Ayiin-0.4.6.dev5/pyAyiin/pyrogram/
--rw-r--r--   0 runner    (1001) docker     (123)      612 2023-06-12 16:36:00.000000 py-Ayiin-0.4.6.dev5/pyAyiin/pyrogram/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2446 2023-06-12 16:36:00.000000 py-Ayiin-0.4.6.dev5/pyAyiin/pyrogram/_wrappers.py
--rw-r--r--   0 runner    (1001) docker     (123)    13157 2023-06-12 16:36:00.000000 py-Ayiin-0.4.6.dev5/pyAyiin/pyrogram/func.py
--rw-r--r--   0 runner    (1001) docker     (123)     3559 2023-06-12 16:36:00.000000 py-Ayiin-0.4.6.dev5/pyAyiin/pyrogram/misc.py
--rw-r--r--   0 runner    (1001) docker     (123)     1936 2023-06-12 16:36:00.000000 py-Ayiin-0.4.6.dev5/pyAyiin/pyrogram/pastebin.py
--rw-r--r--   0 runner    (1001) docker     (123)      832 2023-06-12 16:36:00.000000 py-Ayiin-0.4.6.dev5/pyAyiin/pyrogram/sections.py
--rw-r--r--   0 runner    (1001) docker     (123)     2138 2023-06-12 16:36:00.000000 py-Ayiin-0.4.6.dev5/pyAyiin/pyrogram/toolbot.py
--rw-r--r--   0 runner    (1001) docker     (123)     8684 2023-06-12 16:36:00.000000 py-Ayiin-0.4.6.dev5/pyAyiin/pyrogram/tools.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-12 16:36:09.986822 py-Ayiin-0.4.6.dev5/pyAyiin/resources/
--rw-r--r--   0 runner    (1001) docker     (123)   281001 2023-06-12 16:36:00.000000 py-Ayiin-0.4.6.dev5/pyAyiin/resources/Logo Ayiin.jpg
--rw-r--r--   0 runner    (1001) docker     (123)    31343 2023-06-12 16:36:00.000000 py-Ayiin-0.4.6.dev5/pyAyiin/resources/Youtube.jpeg
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-12 16:36:00.000000 py-Ayiin-0.4.6.dev5/pyAyiin/resources/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    39497 2023-06-12 16:36:00.000000 py-Ayiin-0.4.6.dev5/pyAyiin/resources/ayiin_music.jpg
--rw-r--r--   0 runner    (1001) docker     (123)  1808670 2023-06-12 16:36:00.000000 py-Ayiin-0.4.6.dev5/pyAyiin/resources/ayiin_ubot.jpg
--rw-r--r--   0 runner    (1001) docker     (123)    60539 2023-06-12 16:36:00.000000 py-Ayiin-0.4.6.dev5/pyAyiin/resources/ayiin_userbot.jpg
--rw-r--r--   0 runner    (1001) docker     (123)      889 2023-06-12 16:36:00.000000 py-Ayiin-0.4.6.dev5/pyAyiin/resources/blank.png
--rw-r--r--   0 runner    (1001) docker     (123)    56364 2023-06-12 16:36:00.000000 py-Ayiin-0.4.6.dev5/pyAyiin/resources/default.ttf
--rw-r--r--   0 runner    (1001) docker     (123)   141612 2023-06-12 16:36:00.000000 py-Ayiin-0.4.6.dev5/pyAyiin/resources/font.ttf
--rw-r--r--   0 runner    (1001) docker     (123)   128248 2023-06-12 16:36:00.000000 py-Ayiin-0.4.6.dev5/pyAyiin/resources/font2.ttf
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-12 16:36:09.986822 py-Ayiin-0.4.6.dev5/pyAyiin/telethon/
--rw-r--r--   0 runner    (1001) docker     (123)       31 2023-06-12 16:36:00.000000 py-Ayiin-0.4.6.dev5/pyAyiin/telethon/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-12 16:36:09.986822 py-Ayiin-0.4.6.dev5/pyAyiin/telethon/ayiin/
--rw-r--r--   0 runner    (1001) docker     (123)      152 2023-06-12 16:36:00.000000 py-Ayiin-0.4.6.dev5/pyAyiin/telethon/ayiin/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1803 2023-06-12 16:36:00.000000 py-Ayiin-0.4.6.dev5/pyAyiin/telethon/ayiin/_wrappers.py
--rw-r--r--   0 runner    (1001) docker     (123)     3848 2023-06-12 16:36:00.000000 py-Ayiin-0.4.6.dev5/pyAyiin/telethon/ayiin/events.py
--rw-r--r--   0 runner    (1001) docker     (123)     6803 2023-06-12 16:36:00.000000 py-Ayiin-0.4.6.dev5/pyAyiin/telethon/ayiin/misc.py
--rw-r--r--   0 runner    (1001) docker     (123)    17263 2023-06-12 16:36:00.000000 py-Ayiin-0.4.6.dev5/pyAyiin/xd.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-12 16:36:09.986822 py-Ayiin-0.4.6.dev5/py_Ayiin.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     2572 2023-06-12 16:36:09.000000 py-Ayiin-0.4.6.dev5/py_Ayiin.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1912 2023-06-12 16:36:09.000000 py-Ayiin-0.4.6.dev5/py_Ayiin.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-12 16:36:09.000000 py-Ayiin-0.4.6.dev5/py_Ayiin.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      149 2023-06-12 16:36:09.000000 py-Ayiin-0.4.6.dev5/py_Ayiin.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        8 2023-06-12 16:36:09.000000 py-Ayiin-0.4.6.dev5/py_Ayiin.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)      149 2023-06-12 16:36:00.000000 py-Ayiin-0.4.6.dev5/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-12 16:36:09.986822 py-Ayiin-0.4.6.dev5/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1641 2023-06-12 16:36:00.000000 py-Ayiin-0.4.6.dev5/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-12 16:42:01.509876 py-Ayiin-0.4.6.dev6/
+-rw-r--r--   0 runner    (1001) docker     (123)    35149 2023-06-12 16:41:52.000000 py-Ayiin-0.4.6.dev6/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)      147 2023-06-12 16:41:52.000000 py-Ayiin-0.4.6.dev6/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)      775 2023-06-12 16:41:52.000000 py-Ayiin-0.4.6.dev6/NOTICE
+-rw-r--r--   0 runner    (1001) docker     (123)     2572 2023-06-12 16:42:01.505876 py-Ayiin-0.4.6.dev6/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1642 2023-06-12 16:41:52.000000 py-Ayiin-0.4.6.dev6/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-12 16:42:01.497876 py-Ayiin-0.4.6.dev6/pyAyiin/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-12 16:42:01.497876 py-Ayiin-0.4.6.dev6/pyAyiin/Clients/
+-rw-r--r--   0 runner    (1001) docker     (123)      639 2023-06-12 16:41:52.000000 py-Ayiin-0.4.6.dev6/pyAyiin/Clients/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12525 2023-06-12 16:41:52.000000 py-Ayiin-0.4.6.dev6/pyAyiin/Clients/client.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6295 2023-06-12 16:41:52.000000 py-Ayiin-0.4.6.dev6/pyAyiin/Clients/pytgcalls.py
+-rw-r--r--   0 runner    (1001) docker     (123)    38781 2023-06-12 16:41:52.000000 py-Ayiin-0.4.6.dev6/pyAyiin/Clients/startup.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4570 2023-06-12 16:41:52.000000 py-Ayiin-0.4.6.dev6/pyAyiin/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1505 2023-06-12 16:41:52.000000 py-Ayiin-0.4.6.dev6/pyAyiin/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6704 2023-06-12 16:41:52.000000 py-Ayiin-0.4.6.dev6/pyAyiin/assistant.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5126 2023-06-12 16:41:52.000000 py-Ayiin-0.4.6.dev6/pyAyiin/config.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-12 16:42:01.501875 py-Ayiin-0.4.6.dev6/pyAyiin/dB/
+-rw-r--r--   0 runner    (1001) docker     (123)     1388 2023-06-12 16:41:52.000000 py-Ayiin-0.4.6.dev6/pyAyiin/dB/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      170 2023-06-12 16:41:52.000000 py-Ayiin-0.4.6.dev6/pyAyiin/dB/_core.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-12 16:41:52.000000 py-Ayiin-0.4.6.dev6/pyAyiin/dB/_session.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1330 2023-06-12 16:41:52.000000 py-Ayiin-0.4.6.dev6/pyAyiin/dB/absen.py
+-rw-r--r--   0 runner    (1001) docker     (123)      816 2023-06-12 16:41:52.000000 py-Ayiin-0.4.6.dev6/pyAyiin/dB/admins.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2255 2023-06-12 16:41:52.000000 py-Ayiin-0.4.6.dev6/pyAyiin/dB/auth.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1406 2023-06-12 16:41:52.000000 py-Ayiin-0.4.6.dev6/pyAyiin/dB/blacklistfilter.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1164 2023-06-12 16:41:52.000000 py-Ayiin-0.4.6.dev6/pyAyiin/dB/blacklistgcast.py
+-rw-r--r--   0 runner    (1001) docker     (123)      783 2023-06-12 16:41:52.000000 py-Ayiin-0.4.6.dev6/pyAyiin/dB/blacklistuser.py
+-rw-r--r--   0 runner    (1001) docker     (123)      706 2023-06-12 16:41:52.000000 py-Ayiin-0.4.6.dev6/pyAyiin/dB/gban.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1271 2023-06-12 16:41:52.000000 py-Ayiin-0.4.6.dev6/pyAyiin/dB/langs.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1049 2023-06-12 16:41:52.000000 py-Ayiin-0.4.6.dev6/pyAyiin/dB/logdb.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4755 2023-06-12 16:41:52.000000 py-Ayiin-0.4.6.dev6/pyAyiin/dB/pmpermit.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1331 2023-06-12 16:41:52.000000 py-Ayiin-0.4.6.dev6/pyAyiin/dB/premium.py
+-rw-r--r--   0 runner    (1001) docker     (123)      914 2023-06-12 16:41:52.000000 py-Ayiin-0.4.6.dev6/pyAyiin/dB/start.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1006 2023-06-12 16:41:52.000000 py-Ayiin-0.4.6.dev6/pyAyiin/dB/sudo.py
+-rw-r--r--   0 runner    (1001) docker     (123)      746 2023-06-12 16:41:52.000000 py-Ayiin-0.4.6.dev6/pyAyiin/dB/variable.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1251 2023-06-12 16:41:52.000000 py-Ayiin-0.4.6.dev6/pyAyiin/dB/videocalls.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2012 2023-06-12 16:41:52.000000 py-Ayiin-0.4.6.dev6/pyAyiin/dB/welcome.py
+-rw-r--r--   0 runner    (1001) docker     (123)    33973 2023-06-12 16:41:52.000000 py-Ayiin-0.4.6.dev6/pyAyiin/decorator.py
+-rw-r--r--   0 runner    (1001) docker     (123)      959 2023-06-12 16:41:52.000000 py-Ayiin-0.4.6.dev6/pyAyiin/exceptions.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-12 16:42:01.501875 py-Ayiin-0.4.6.dev6/pyAyiin/methods/
+-rw-r--r--   0 runner    (1001) docker     (123)      954 2023-06-12 16:41:52.000000 py-Ayiin-0.4.6.dev6/pyAyiin/methods/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10094 2023-06-12 16:41:52.000000 py-Ayiin-0.4.6.dev6/pyAyiin/methods/_database.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3939 2023-06-12 16:41:52.000000 py-Ayiin-0.4.6.dev6/pyAyiin/methods/_misc.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1897 2023-06-12 16:41:52.000000 py-Ayiin-0.4.6.dev6/pyAyiin/methods/changer.py
+-rw-r--r--   0 runner    (1001) docker     (123)      853 2023-06-12 16:41:52.000000 py-Ayiin-0.4.6.dev6/pyAyiin/methods/converter.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6909 2023-06-12 16:41:52.000000 py-Ayiin-0.4.6.dev6/pyAyiin/methods/func.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10022 2023-06-12 16:41:52.000000 py-Ayiin-0.4.6.dev6/pyAyiin/methods/funcb.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8828 2023-06-12 16:41:52.000000 py-Ayiin-0.4.6.dev6/pyAyiin/methods/helpers.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1213 2023-06-12 16:41:52.000000 py-Ayiin-0.4.6.dev6/pyAyiin/methods/hosting.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7713 2023-06-12 16:41:52.000000 py-Ayiin-0.4.6.dev6/pyAyiin/methods/inlinebot.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2879 2023-06-12 16:41:52.000000 py-Ayiin-0.4.6.dev6/pyAyiin/methods/queue.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6067 2023-06-12 16:41:52.000000 py-Ayiin-0.4.6.dev6/pyAyiin/methods/thumbnail.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-12 16:42:01.501875 py-Ayiin-0.4.6.dev6/pyAyiin/pyrogram/
+-rw-r--r--   0 runner    (1001) docker     (123)      612 2023-06-12 16:41:52.000000 py-Ayiin-0.4.6.dev6/pyAyiin/pyrogram/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2446 2023-06-12 16:41:52.000000 py-Ayiin-0.4.6.dev6/pyAyiin/pyrogram/_wrappers.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13157 2023-06-12 16:41:52.000000 py-Ayiin-0.4.6.dev6/pyAyiin/pyrogram/func.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3559 2023-06-12 16:41:52.000000 py-Ayiin-0.4.6.dev6/pyAyiin/pyrogram/misc.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1936 2023-06-12 16:41:52.000000 py-Ayiin-0.4.6.dev6/pyAyiin/pyrogram/pastebin.py
+-rw-r--r--   0 runner    (1001) docker     (123)      832 2023-06-12 16:41:52.000000 py-Ayiin-0.4.6.dev6/pyAyiin/pyrogram/sections.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2138 2023-06-12 16:41:52.000000 py-Ayiin-0.4.6.dev6/pyAyiin/pyrogram/toolbot.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8684 2023-06-12 16:41:52.000000 py-Ayiin-0.4.6.dev6/pyAyiin/pyrogram/tools.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-12 16:42:01.505876 py-Ayiin-0.4.6.dev6/pyAyiin/resources/
+-rw-r--r--   0 runner    (1001) docker     (123)   281001 2023-06-12 16:41:52.000000 py-Ayiin-0.4.6.dev6/pyAyiin/resources/Logo Ayiin.jpg
+-rw-r--r--   0 runner    (1001) docker     (123)    31343 2023-06-12 16:41:52.000000 py-Ayiin-0.4.6.dev6/pyAyiin/resources/Youtube.jpeg
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-12 16:41:52.000000 py-Ayiin-0.4.6.dev6/pyAyiin/resources/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    39497 2023-06-12 16:41:52.000000 py-Ayiin-0.4.6.dev6/pyAyiin/resources/ayiin_music.jpg
+-rw-r--r--   0 runner    (1001) docker     (123)  1808670 2023-06-12 16:41:52.000000 py-Ayiin-0.4.6.dev6/pyAyiin/resources/ayiin_ubot.jpg
+-rw-r--r--   0 runner    (1001) docker     (123)    60539 2023-06-12 16:41:52.000000 py-Ayiin-0.4.6.dev6/pyAyiin/resources/ayiin_userbot.jpg
+-rw-r--r--   0 runner    (1001) docker     (123)      889 2023-06-12 16:41:52.000000 py-Ayiin-0.4.6.dev6/pyAyiin/resources/blank.png
+-rw-r--r--   0 runner    (1001) docker     (123)    56364 2023-06-12 16:41:52.000000 py-Ayiin-0.4.6.dev6/pyAyiin/resources/default.ttf
+-rw-r--r--   0 runner    (1001) docker     (123)   141612 2023-06-12 16:41:52.000000 py-Ayiin-0.4.6.dev6/pyAyiin/resources/font.ttf
+-rw-r--r--   0 runner    (1001) docker     (123)   128248 2023-06-12 16:41:52.000000 py-Ayiin-0.4.6.dev6/pyAyiin/resources/font2.ttf
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-12 16:42:01.505876 py-Ayiin-0.4.6.dev6/pyAyiin/telethon/
+-rw-r--r--   0 runner    (1001) docker     (123)       31 2023-06-12 16:41:52.000000 py-Ayiin-0.4.6.dev6/pyAyiin/telethon/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-12 16:42:01.505876 py-Ayiin-0.4.6.dev6/pyAyiin/telethon/ayiin/
+-rw-r--r--   0 runner    (1001) docker     (123)      152 2023-06-12 16:41:52.000000 py-Ayiin-0.4.6.dev6/pyAyiin/telethon/ayiin/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1803 2023-06-12 16:41:52.000000 py-Ayiin-0.4.6.dev6/pyAyiin/telethon/ayiin/_wrappers.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3848 2023-06-12 16:41:52.000000 py-Ayiin-0.4.6.dev6/pyAyiin/telethon/ayiin/events.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6803 2023-06-12 16:41:52.000000 py-Ayiin-0.4.6.dev6/pyAyiin/telethon/ayiin/misc.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17263 2023-06-12 16:41:52.000000 py-Ayiin-0.4.6.dev6/pyAyiin/xd.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-12 16:42:01.505876 py-Ayiin-0.4.6.dev6/py_Ayiin.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     2572 2023-06-12 16:42:01.000000 py-Ayiin-0.4.6.dev6/py_Ayiin.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1912 2023-06-12 16:42:01.000000 py-Ayiin-0.4.6.dev6/py_Ayiin.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-12 16:42:01.000000 py-Ayiin-0.4.6.dev6/py_Ayiin.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      149 2023-06-12 16:42:01.000000 py-Ayiin-0.4.6.dev6/py_Ayiin.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        8 2023-06-12 16:42:01.000000 py-Ayiin-0.4.6.dev6/py_Ayiin.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      149 2023-06-12 16:41:52.000000 py-Ayiin-0.4.6.dev6/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-12 16:42:01.509876 py-Ayiin-0.4.6.dev6/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1641 2023-06-12 16:41:52.000000 py-Ayiin-0.4.6.dev6/setup.py
```

### Comparing `py-Ayiin-0.4.6.dev5/LICENSE` & `py-Ayiin-0.4.6.dev6/LICENSE`

 * *Files identical despite different names*

### Comparing `py-Ayiin-0.4.6.dev5/NOTICE` & `py-Ayiin-0.4.6.dev6/NOTICE`

 * *Files identical despite different names*

### Comparing `py-Ayiin-0.4.6.dev5/PKG-INFO` & `py-Ayiin-0.4.6.dev6/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: py-Ayiin
-Version: 0.4.6.dev5
+Version: 0.4.6.dev6
 Summary: A Secure and Powerful Python-Telethon Based and Python-Pyrogram Based Library For Your Userbot Module.
 Home-page: https://github.com/AyiinXd/AyiinXd
 Author: AyiinXd
 Author-email: ayingaming98@gmail.com
 License: GNU General Public License v3.0 (GPL-3.0)
 Project-URL: Bug Tracker, https://github.com/AyiinXd/AyiinXd/issues
 Project-URL: Source Code, https://github.com/AyiinXd/AyiinXd
```

### Comparing `py-Ayiin-0.4.6.dev5/README.md` & `py-Ayiin-0.4.6.dev6/README.md`

 * *Files identical despite different names*

### Comparing `py-Ayiin-0.4.6.dev5/pyAyiin/Clients/__init__.py` & `py-Ayiin-0.4.6.dev6/pyAyiin/Clients/__init__.py`

 * *Files identical despite different names*

### Comparing `py-Ayiin-0.4.6.dev5/pyAyiin/Clients/client.py` & `py-Ayiin-0.4.6.dev6/pyAyiin/Clients/client.py`

 * *Files identical despite different names*

### Comparing `py-Ayiin-0.4.6.dev5/pyAyiin/Clients/pytgcalls.py` & `py-Ayiin-0.4.6.dev6/pyAyiin/Clients/pytgcalls.py`

 * *Files identical despite different names*

### Comparing `py-Ayiin-0.4.6.dev5/pyAyiin/Clients/startup.py` & `py-Ayiin-0.4.6.dev6/pyAyiin/Clients/startup.py`

 * *Files identical despite different names*

### Comparing `py-Ayiin-0.4.6.dev5/pyAyiin/__init__.py` & `py-Ayiin-0.4.6.dev6/pyAyiin/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -48,15 +48,15 @@
 
 
 logs = logging.getLogger(__name__)
 
 
 __copyright__ = "Copyright (C) 2022-present AyiinXd <https://github.com/AyiinXd>"
 __license__ = "GNU General Public License v3.0 (GPL-3.0)"
-__version__ = "0.4.6.dev05"
+__version__ = "0.4.6.dev06"
 ayiin_ver = "0.1.1"
 prem_version = "0.1"
 
 
 DEVS = [
     607067484, # Ayiin
     997461844, #Ayang_Ayiin
```

### Comparing `py-Ayiin-0.4.6.dev5/pyAyiin/__main__.py` & `py-Ayiin-0.4.6.dev6/pyAyiin/__main__.py`

 * *Files identical despite different names*

### Comparing `py-Ayiin-0.4.6.dev5/pyAyiin/assistant.py` & `py-Ayiin-0.4.6.dev6/pyAyiin/assistant.py`

 * *Files identical despite different names*

### Comparing `py-Ayiin-0.4.6.dev5/pyAyiin/config.py` & `py-Ayiin-0.4.6.dev6/pyAyiin/config.py`

 * *Files identical despite different names*

### Comparing `py-Ayiin-0.4.6.dev5/pyAyiin/dB/__init__.py` & `py-Ayiin-0.4.6.dev6/pyAyiin/dB/__init__.py`

 * *Files identical despite different names*

### Comparing `py-Ayiin-0.4.6.dev5/pyAyiin/dB/absen.py` & `py-Ayiin-0.4.6.dev6/pyAyiin/dB/absen.py`

 * *Files identical despite different names*

### Comparing `py-Ayiin-0.4.6.dev5/pyAyiin/dB/admins.py` & `py-Ayiin-0.4.6.dev6/pyAyiin/dB/admins.py`

 * *Files identical despite different names*

### Comparing `py-Ayiin-0.4.6.dev5/pyAyiin/dB/auth.py` & `py-Ayiin-0.4.6.dev6/pyAyiin/dB/auth.py`

 * *Files identical despite different names*

### Comparing `py-Ayiin-0.4.6.dev5/pyAyiin/dB/blacklistfilter.py` & `py-Ayiin-0.4.6.dev6/pyAyiin/dB/blacklistfilter.py`

 * *Files identical despite different names*

### Comparing `py-Ayiin-0.4.6.dev5/pyAyiin/dB/blacklistgcast.py` & `py-Ayiin-0.4.6.dev6/pyAyiin/dB/blacklistgcast.py`

 * *Files identical despite different names*

### Comparing `py-Ayiin-0.4.6.dev5/pyAyiin/dB/blacklistuser.py` & `py-Ayiin-0.4.6.dev6/pyAyiin/dB/blacklistuser.py`

 * *Files identical despite different names*

### Comparing `py-Ayiin-0.4.6.dev5/pyAyiin/dB/gban.py` & `py-Ayiin-0.4.6.dev6/pyAyiin/dB/gban.py`

 * *Files identical despite different names*

### Comparing `py-Ayiin-0.4.6.dev5/pyAyiin/dB/langs.py` & `py-Ayiin-0.4.6.dev6/pyAyiin/dB/langs.py`

 * *Files identical despite different names*

### Comparing `py-Ayiin-0.4.6.dev5/pyAyiin/dB/logdb.py` & `py-Ayiin-0.4.6.dev6/pyAyiin/dB/logdb.py`

 * *Files identical despite different names*

### Comparing `py-Ayiin-0.4.6.dev5/pyAyiin/dB/pmpermit.py` & `py-Ayiin-0.4.6.dev6/pyAyiin/dB/pmpermit.py`

 * *Files identical despite different names*

### Comparing `py-Ayiin-0.4.6.dev5/pyAyiin/dB/premium.py` & `py-Ayiin-0.4.6.dev6/pyAyiin/dB/premium.py`

 * *Files identical despite different names*

### Comparing `py-Ayiin-0.4.6.dev5/pyAyiin/dB/start.py` & `py-Ayiin-0.4.6.dev6/pyAyiin/dB/start.py`

 * *Files identical despite different names*

### Comparing `py-Ayiin-0.4.6.dev5/pyAyiin/dB/sudo.py` & `py-Ayiin-0.4.6.dev6/pyAyiin/dB/sudo.py`

 * *Files identical despite different names*

### Comparing `py-Ayiin-0.4.6.dev5/pyAyiin/dB/variable.py` & `py-Ayiin-0.4.6.dev6/pyAyiin/dB/variable.py`

 * *Files identical despite different names*

### Comparing `py-Ayiin-0.4.6.dev5/pyAyiin/dB/videocalls.py` & `py-Ayiin-0.4.6.dev6/pyAyiin/dB/videocalls.py`

 * *Files identical despite different names*

### Comparing `py-Ayiin-0.4.6.dev5/pyAyiin/dB/welcome.py` & `py-Ayiin-0.4.6.dev6/pyAyiin/dB/welcome.py`

 * *Files identical despite different names*

### Comparing `py-Ayiin-0.4.6.dev5/pyAyiin/decorator.py` & `py-Ayiin-0.4.6.dev6/pyAyiin/decorator.py`

 * *Files identical despite different names*

### Comparing `py-Ayiin-0.4.6.dev5/pyAyiin/exceptions.py` & `py-Ayiin-0.4.6.dev6/pyAyiin/exceptions.py`

 * *Files identical despite different names*

### Comparing `py-Ayiin-0.4.6.dev5/pyAyiin/methods/__init__.py` & `py-Ayiin-0.4.6.dev6/pyAyiin/methods/__init__.py`

 * *Files identical despite different names*

### Comparing `py-Ayiin-0.4.6.dev5/pyAyiin/methods/_database.py` & `py-Ayiin-0.4.6.dev6/pyAyiin/methods/_database.py`

 * *Files identical despite different names*

### Comparing `py-Ayiin-0.4.6.dev5/pyAyiin/methods/_misc.py` & `py-Ayiin-0.4.6.dev6/pyAyiin/methods/_misc.py`

 * *Files identical despite different names*

### Comparing `py-Ayiin-0.4.6.dev5/pyAyiin/methods/changer.py` & `py-Ayiin-0.4.6.dev6/pyAyiin/methods/changer.py`

 * *Files identical despite different names*

### Comparing `py-Ayiin-0.4.6.dev5/pyAyiin/methods/converter.py` & `py-Ayiin-0.4.6.dev6/pyAyiin/methods/converter.py`

 * *Files identical despite different names*

### Comparing `py-Ayiin-0.4.6.dev5/pyAyiin/methods/func.py` & `py-Ayiin-0.4.6.dev6/pyAyiin/methods/func.py`

 * *Files identical despite different names*

### Comparing `py-Ayiin-0.4.6.dev5/pyAyiin/methods/funcb.py` & `py-Ayiin-0.4.6.dev6/pyAyiin/methods/funcb.py`

 * *Files identical despite different names*

### Comparing `py-Ayiin-0.4.6.dev5/pyAyiin/methods/helpers.py` & `py-Ayiin-0.4.6.dev6/pyAyiin/methods/helpers.py`

 * *Files identical despite different names*

### Comparing `py-Ayiin-0.4.6.dev5/pyAyiin/methods/hosting.py` & `py-Ayiin-0.4.6.dev6/pyAyiin/methods/hosting.py`

 * *Files identical despite different names*

### Comparing `py-Ayiin-0.4.6.dev5/pyAyiin/methods/inlinebot.py` & `py-Ayiin-0.4.6.dev6/pyAyiin/methods/inlinebot.py`

 * *Files 1% similar despite different names*

```diff
@@ -185,18 +185,18 @@
                         reply_markup=InlineKeyboardMarkup(buttons),
                         input_message_content=InputTextMessageContent(output),
                     )
                 )
             ]
         return results
     
-    async def inline_languages(self, _):
+    async def inline_languages(self, ids, _):
         from pyAyiin.dB.langs import get_lang, get_languages
         
-        lang = await get_lang
+        lang = await get_lang(ids)
         text = _["lang"].format(lang)
         languages = get_languages()
         tutud = [
             InlineKeyboardButton(
                 f"{languages[yins]['nama']}",
                 callback_data=f"set_{yins}",
             )
```

### Comparing `py-Ayiin-0.4.6.dev5/pyAyiin/methods/queue.py` & `py-Ayiin-0.4.6.dev6/pyAyiin/methods/queue.py`

 * *Files identical despite different names*

### Comparing `py-Ayiin-0.4.6.dev5/pyAyiin/methods/thumbnail.py` & `py-Ayiin-0.4.6.dev6/pyAyiin/methods/thumbnail.py`

 * *Files identical despite different names*

### Comparing `py-Ayiin-0.4.6.dev5/pyAyiin/pyrogram/__init__.py` & `py-Ayiin-0.4.6.dev6/pyAyiin/pyrogram/__init__.py`

 * *Files identical despite different names*

### Comparing `py-Ayiin-0.4.6.dev5/pyAyiin/pyrogram/_wrappers.py` & `py-Ayiin-0.4.6.dev6/pyAyiin/pyrogram/_wrappers.py`

 * *Files identical despite different names*

### Comparing `py-Ayiin-0.4.6.dev5/pyAyiin/pyrogram/func.py` & `py-Ayiin-0.4.6.dev6/pyAyiin/pyrogram/func.py`

 * *Files identical despite different names*

### Comparing `py-Ayiin-0.4.6.dev5/pyAyiin/pyrogram/misc.py` & `py-Ayiin-0.4.6.dev6/pyAyiin/pyrogram/misc.py`

 * *Files identical despite different names*

### Comparing `py-Ayiin-0.4.6.dev5/pyAyiin/pyrogram/pastebin.py` & `py-Ayiin-0.4.6.dev6/pyAyiin/pyrogram/pastebin.py`

 * *Files identical despite different names*

### Comparing `py-Ayiin-0.4.6.dev5/pyAyiin/pyrogram/sections.py` & `py-Ayiin-0.4.6.dev6/pyAyiin/pyrogram/sections.py`

 * *Files identical despite different names*

### Comparing `py-Ayiin-0.4.6.dev5/pyAyiin/pyrogram/toolbot.py` & `py-Ayiin-0.4.6.dev6/pyAyiin/pyrogram/toolbot.py`

 * *Files identical despite different names*

### Comparing `py-Ayiin-0.4.6.dev5/pyAyiin/pyrogram/tools.py` & `py-Ayiin-0.4.6.dev6/pyAyiin/pyrogram/tools.py`

 * *Files identical despite different names*

### Comparing `py-Ayiin-0.4.6.dev5/pyAyiin/resources/Logo Ayiin.jpg` & `py-Ayiin-0.4.6.dev6/pyAyiin/resources/Logo Ayiin.jpg`

 * *Files identical despite different names*

### Comparing `py-Ayiin-0.4.6.dev5/pyAyiin/resources/Youtube.jpeg` & `py-Ayiin-0.4.6.dev6/pyAyiin/resources/Youtube.jpeg`

 * *Files identical despite different names*

### Comparing `py-Ayiin-0.4.6.dev5/pyAyiin/resources/ayiin_music.jpg` & `py-Ayiin-0.4.6.dev6/pyAyiin/resources/ayiin_music.jpg`

 * *Files identical despite different names*

### Comparing `py-Ayiin-0.4.6.dev5/pyAyiin/resources/ayiin_ubot.jpg` & `py-Ayiin-0.4.6.dev6/pyAyiin/resources/ayiin_ubot.jpg`

 * *Files identical despite different names*

### Comparing `py-Ayiin-0.4.6.dev5/pyAyiin/resources/ayiin_userbot.jpg` & `py-Ayiin-0.4.6.dev6/pyAyiin/resources/ayiin_userbot.jpg`

 * *Files identical despite different names*

### Comparing `py-Ayiin-0.4.6.dev5/pyAyiin/resources/blank.png` & `py-Ayiin-0.4.6.dev6/pyAyiin/resources/blank.png`

 * *Files identical despite different names*

### Comparing `py-Ayiin-0.4.6.dev5/pyAyiin/resources/default.ttf` & `py-Ayiin-0.4.6.dev6/pyAyiin/resources/default.ttf`

 * *Files identical despite different names*

### Comparing `py-Ayiin-0.4.6.dev5/pyAyiin/resources/font.ttf` & `py-Ayiin-0.4.6.dev6/pyAyiin/resources/font.ttf`

 * *Files identical despite different names*

### Comparing `py-Ayiin-0.4.6.dev5/pyAyiin/resources/font2.ttf` & `py-Ayiin-0.4.6.dev6/pyAyiin/resources/font2.ttf`

 * *Files identical despite different names*

### Comparing `py-Ayiin-0.4.6.dev5/pyAyiin/telethon/ayiin/_wrappers.py` & `py-Ayiin-0.4.6.dev6/pyAyiin/telethon/ayiin/_wrappers.py`

 * *Files identical despite different names*

### Comparing `py-Ayiin-0.4.6.dev5/pyAyiin/telethon/ayiin/events.py` & `py-Ayiin-0.4.6.dev6/pyAyiin/telethon/ayiin/events.py`

 * *Files identical despite different names*

### Comparing `py-Ayiin-0.4.6.dev5/pyAyiin/telethon/ayiin/misc.py` & `py-Ayiin-0.4.6.dev6/pyAyiin/telethon/ayiin/misc.py`

 * *Files identical despite different names*

### Comparing `py-Ayiin-0.4.6.dev5/pyAyiin/xd.py` & `py-Ayiin-0.4.6.dev6/pyAyiin/xd.py`

 * *Files identical despite different names*

### Comparing `py-Ayiin-0.4.6.dev5/py_Ayiin.egg-info/PKG-INFO` & `py-Ayiin-0.4.6.dev6/py_Ayiin.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: py-Ayiin
-Version: 0.4.6.dev5
+Version: 0.4.6.dev6
 Summary: A Secure and Powerful Python-Telethon Based and Python-Pyrogram Based Library For Your Userbot Module.
 Home-page: https://github.com/AyiinXd/AyiinXd
 Author: AyiinXd
 Author-email: ayingaming98@gmail.com
 License: GNU General Public License v3.0 (GPL-3.0)
 Project-URL: Bug Tracker, https://github.com/AyiinXd/AyiinXd/issues
 Project-URL: Source Code, https://github.com/AyiinXd/AyiinXd
```

### Comparing `py-Ayiin-0.4.6.dev5/py_Ayiin.egg-info/SOURCES.txt` & `py-Ayiin-0.4.6.dev6/py_Ayiin.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `py-Ayiin-0.4.6.dev5/setup.py` & `py-Ayiin-0.4.6.dev6/setup.py`

 * *Files identical despite different names*

