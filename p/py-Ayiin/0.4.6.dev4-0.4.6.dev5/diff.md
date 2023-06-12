# Comparing `tmp/py-Ayiin-0.4.6.dev4.tar.gz` & `tmp/py-Ayiin-0.4.6.dev5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "py-Ayiin-0.4.6.dev4.tar", last modified: Sun Jun 11 15:08:51 2023, max compression
+gzip compressed data, was "py-Ayiin-0.4.6.dev5.tar", last modified: Mon Jun 12 16:36:09 2023, max compression
```

## Comparing `py-Ayiin-0.4.6.dev4.tar` & `py-Ayiin-0.4.6.dev5.tar`

### file list

```diff
@@ -1,88 +1,88 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-11 15:08:51.381365 py-Ayiin-0.4.6.dev4/
--rw-r--r--   0 runner    (1001) docker     (123)    35149 2023-06-11 15:08:42.000000 py-Ayiin-0.4.6.dev4/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)      147 2023-06-11 15:08:42.000000 py-Ayiin-0.4.6.dev4/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)      775 2023-06-11 15:08:42.000000 py-Ayiin-0.4.6.dev4/NOTICE
--rw-r--r--   0 runner    (1001) docker     (123)     2572 2023-06-11 15:08:51.381365 py-Ayiin-0.4.6.dev4/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1642 2023-06-11 15:08:42.000000 py-Ayiin-0.4.6.dev4/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-11 15:08:51.373365 py-Ayiin-0.4.6.dev4/pyAyiin/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-11 15:08:51.373365 py-Ayiin-0.4.6.dev4/pyAyiin/Clients/
--rw-r--r--   0 runner    (1001) docker     (123)      639 2023-06-11 15:08:42.000000 py-Ayiin-0.4.6.dev4/pyAyiin/Clients/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    12525 2023-06-11 15:08:42.000000 py-Ayiin-0.4.6.dev4/pyAyiin/Clients/client.py
--rw-r--r--   0 runner    (1001) docker     (123)     6165 2023-06-11 15:08:42.000000 py-Ayiin-0.4.6.dev4/pyAyiin/Clients/pytgcalls.py
--rw-r--r--   0 runner    (1001) docker     (123)    38778 2023-06-11 15:08:42.000000 py-Ayiin-0.4.6.dev4/pyAyiin/Clients/startup.py
--rw-r--r--   0 runner    (1001) docker     (123)     4570 2023-06-11 15:08:42.000000 py-Ayiin-0.4.6.dev4/pyAyiin/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1494 2023-06-11 15:08:42.000000 py-Ayiin-0.4.6.dev4/pyAyiin/__main__.py
--rw-r--r--   0 runner    (1001) docker     (123)     6704 2023-06-11 15:08:42.000000 py-Ayiin-0.4.6.dev4/pyAyiin/assistant.py
--rw-r--r--   0 runner    (1001) docker     (123)     5126 2023-06-11 15:08:42.000000 py-Ayiin-0.4.6.dev4/pyAyiin/config.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-11 15:08:51.373365 py-Ayiin-0.4.6.dev4/pyAyiin/dB/
--rw-r--r--   0 runner    (1001) docker     (123)     1388 2023-06-11 15:08:42.000000 py-Ayiin-0.4.6.dev4/pyAyiin/dB/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      170 2023-06-11 15:08:42.000000 py-Ayiin-0.4.6.dev4/pyAyiin/dB/_core.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-11 15:08:42.000000 py-Ayiin-0.4.6.dev4/pyAyiin/dB/_session.py
--rw-r--r--   0 runner    (1001) docker     (123)     1330 2023-06-11 15:08:42.000000 py-Ayiin-0.4.6.dev4/pyAyiin/dB/absen.py
--rw-r--r--   0 runner    (1001) docker     (123)      816 2023-06-11 15:08:42.000000 py-Ayiin-0.4.6.dev4/pyAyiin/dB/admins.py
--rw-r--r--   0 runner    (1001) docker     (123)     2255 2023-06-11 15:08:42.000000 py-Ayiin-0.4.6.dev4/pyAyiin/dB/auth.py
--rw-r--r--   0 runner    (1001) docker     (123)     1406 2023-06-11 15:08:42.000000 py-Ayiin-0.4.6.dev4/pyAyiin/dB/blacklistfilter.py
--rw-r--r--   0 runner    (1001) docker     (123)     1164 2023-06-11 15:08:42.000000 py-Ayiin-0.4.6.dev4/pyAyiin/dB/blacklistgcast.py
--rw-r--r--   0 runner    (1001) docker     (123)      783 2023-06-11 15:08:42.000000 py-Ayiin-0.4.6.dev4/pyAyiin/dB/blacklistuser.py
--rw-r--r--   0 runner    (1001) docker     (123)      706 2023-06-11 15:08:42.000000 py-Ayiin-0.4.6.dev4/pyAyiin/dB/gban.py
--rw-r--r--   0 runner    (1001) docker     (123)     1271 2023-06-11 15:08:42.000000 py-Ayiin-0.4.6.dev4/pyAyiin/dB/langs.py
--rw-r--r--   0 runner    (1001) docker     (123)     1049 2023-06-11 15:08:42.000000 py-Ayiin-0.4.6.dev4/pyAyiin/dB/logdb.py
--rw-r--r--   0 runner    (1001) docker     (123)     4755 2023-06-11 15:08:42.000000 py-Ayiin-0.4.6.dev4/pyAyiin/dB/pmpermit.py
--rw-r--r--   0 runner    (1001) docker     (123)     1331 2023-06-11 15:08:42.000000 py-Ayiin-0.4.6.dev4/pyAyiin/dB/premium.py
--rw-r--r--   0 runner    (1001) docker     (123)      914 2023-06-11 15:08:42.000000 py-Ayiin-0.4.6.dev4/pyAyiin/dB/start.py
--rw-r--r--   0 runner    (1001) docker     (123)     1006 2023-06-11 15:08:42.000000 py-Ayiin-0.4.6.dev4/pyAyiin/dB/sudo.py
--rw-r--r--   0 runner    (1001) docker     (123)      746 2023-06-11 15:08:42.000000 py-Ayiin-0.4.6.dev4/pyAyiin/dB/variable.py
--rw-r--r--   0 runner    (1001) docker     (123)     1251 2023-06-11 15:08:42.000000 py-Ayiin-0.4.6.dev4/pyAyiin/dB/videocalls.py
--rw-r--r--   0 runner    (1001) docker     (123)     2012 2023-06-11 15:08:42.000000 py-Ayiin-0.4.6.dev4/pyAyiin/dB/welcome.py
--rw-r--r--   0 runner    (1001) docker     (123)    33973 2023-06-11 15:08:42.000000 py-Ayiin-0.4.6.dev4/pyAyiin/decorator.py
--rw-r--r--   0 runner    (1001) docker     (123)      959 2023-06-11 15:08:42.000000 py-Ayiin-0.4.6.dev4/pyAyiin/exceptions.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-11 15:08:51.377364 py-Ayiin-0.4.6.dev4/pyAyiin/methods/
--rw-r--r--   0 runner    (1001) docker     (123)      954 2023-06-11 15:08:42.000000 py-Ayiin-0.4.6.dev4/pyAyiin/methods/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    10094 2023-06-11 15:08:42.000000 py-Ayiin-0.4.6.dev4/pyAyiin/methods/_database.py
--rw-r--r--   0 runner    (1001) docker     (123)     3939 2023-06-11 15:08:42.000000 py-Ayiin-0.4.6.dev4/pyAyiin/methods/_misc.py
--rw-r--r--   0 runner    (1001) docker     (123)     1897 2023-06-11 15:08:42.000000 py-Ayiin-0.4.6.dev4/pyAyiin/methods/changer.py
--rw-r--r--   0 runner    (1001) docker     (123)      853 2023-06-11 15:08:42.000000 py-Ayiin-0.4.6.dev4/pyAyiin/methods/converter.py
--rw-r--r--   0 runner    (1001) docker     (123)     6909 2023-06-11 15:08:42.000000 py-Ayiin-0.4.6.dev4/pyAyiin/methods/func.py
--rw-r--r--   0 runner    (1001) docker     (123)     6135 2023-06-11 15:08:42.000000 py-Ayiin-0.4.6.dev4/pyAyiin/methods/funcb.py
--rw-r--r--   0 runner    (1001) docker     (123)     8828 2023-06-11 15:08:42.000000 py-Ayiin-0.4.6.dev4/pyAyiin/methods/helpers.py
--rw-r--r--   0 runner    (1001) docker     (123)     1213 2023-06-11 15:08:42.000000 py-Ayiin-0.4.6.dev4/pyAyiin/methods/hosting.py
--rw-r--r--   0 runner    (1001) docker     (123)     7650 2023-06-11 15:08:42.000000 py-Ayiin-0.4.6.dev4/pyAyiin/methods/inlinebot.py
--rw-r--r--   0 runner    (1001) docker     (123)     2879 2023-06-11 15:08:42.000000 py-Ayiin-0.4.6.dev4/pyAyiin/methods/queue.py
--rw-r--r--   0 runner    (1001) docker     (123)     6067 2023-06-11 15:08:42.000000 py-Ayiin-0.4.6.dev4/pyAyiin/methods/thumbnail.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-11 15:08:51.377364 py-Ayiin-0.4.6.dev4/pyAyiin/pyrogram/
--rw-r--r--   0 runner    (1001) docker     (123)      612 2023-06-11 15:08:42.000000 py-Ayiin-0.4.6.dev4/pyAyiin/pyrogram/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2446 2023-06-11 15:08:42.000000 py-Ayiin-0.4.6.dev4/pyAyiin/pyrogram/_wrappers.py
--rw-r--r--   0 runner    (1001) docker     (123)    13157 2023-06-11 15:08:42.000000 py-Ayiin-0.4.6.dev4/pyAyiin/pyrogram/func.py
--rw-r--r--   0 runner    (1001) docker     (123)     3559 2023-06-11 15:08:42.000000 py-Ayiin-0.4.6.dev4/pyAyiin/pyrogram/misc.py
--rw-r--r--   0 runner    (1001) docker     (123)     1936 2023-06-11 15:08:42.000000 py-Ayiin-0.4.6.dev4/pyAyiin/pyrogram/pastebin.py
--rw-r--r--   0 runner    (1001) docker     (123)      832 2023-06-11 15:08:42.000000 py-Ayiin-0.4.6.dev4/pyAyiin/pyrogram/sections.py
--rw-r--r--   0 runner    (1001) docker     (123)     2138 2023-06-11 15:08:42.000000 py-Ayiin-0.4.6.dev4/pyAyiin/pyrogram/toolbot.py
--rw-r--r--   0 runner    (1001) docker     (123)     8684 2023-06-11 15:08:42.000000 py-Ayiin-0.4.6.dev4/pyAyiin/pyrogram/tools.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-11 15:08:51.381365 py-Ayiin-0.4.6.dev4/pyAyiin/resources/
--rw-r--r--   0 runner    (1001) docker     (123)   281001 2023-06-11 15:08:42.000000 py-Ayiin-0.4.6.dev4/pyAyiin/resources/Logo Ayiin.jpg
--rw-r--r--   0 runner    (1001) docker     (123)    31343 2023-06-11 15:08:42.000000 py-Ayiin-0.4.6.dev4/pyAyiin/resources/Youtube.jpeg
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-11 15:08:42.000000 py-Ayiin-0.4.6.dev4/pyAyiin/resources/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    39497 2023-06-11 15:08:42.000000 py-Ayiin-0.4.6.dev4/pyAyiin/resources/ayiin_music.jpg
--rw-r--r--   0 runner    (1001) docker     (123)  1808670 2023-06-11 15:08:42.000000 py-Ayiin-0.4.6.dev4/pyAyiin/resources/ayiin_ubot.jpg
--rw-r--r--   0 runner    (1001) docker     (123)    60539 2023-06-11 15:08:42.000000 py-Ayiin-0.4.6.dev4/pyAyiin/resources/ayiin_userbot.jpg
--rw-r--r--   0 runner    (1001) docker     (123)      889 2023-06-11 15:08:42.000000 py-Ayiin-0.4.6.dev4/pyAyiin/resources/blank.png
--rw-r--r--   0 runner    (1001) docker     (123)    56364 2023-06-11 15:08:42.000000 py-Ayiin-0.4.6.dev4/pyAyiin/resources/default.ttf
--rw-r--r--   0 runner    (1001) docker     (123)   141612 2023-06-11 15:08:42.000000 py-Ayiin-0.4.6.dev4/pyAyiin/resources/font.ttf
--rw-r--r--   0 runner    (1001) docker     (123)   128248 2023-06-11 15:08:42.000000 py-Ayiin-0.4.6.dev4/pyAyiin/resources/font2.ttf
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-11 15:08:51.381365 py-Ayiin-0.4.6.dev4/pyAyiin/telethon/
--rw-r--r--   0 runner    (1001) docker     (123)       31 2023-06-11 15:08:42.000000 py-Ayiin-0.4.6.dev4/pyAyiin/telethon/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-11 15:08:51.381365 py-Ayiin-0.4.6.dev4/pyAyiin/telethon/ayiin/
--rw-r--r--   0 runner    (1001) docker     (123)      152 2023-06-11 15:08:42.000000 py-Ayiin-0.4.6.dev4/pyAyiin/telethon/ayiin/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1803 2023-06-11 15:08:42.000000 py-Ayiin-0.4.6.dev4/pyAyiin/telethon/ayiin/_wrappers.py
--rw-r--r--   0 runner    (1001) docker     (123)     3848 2023-06-11 15:08:42.000000 py-Ayiin-0.4.6.dev4/pyAyiin/telethon/ayiin/events.py
--rw-r--r--   0 runner    (1001) docker     (123)     6803 2023-06-11 15:08:42.000000 py-Ayiin-0.4.6.dev4/pyAyiin/telethon/ayiin/misc.py
--rw-r--r--   0 runner    (1001) docker     (123)    17263 2023-06-11 15:08:42.000000 py-Ayiin-0.4.6.dev4/pyAyiin/xd.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-11 15:08:51.381365 py-Ayiin-0.4.6.dev4/py_Ayiin.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     2572 2023-06-11 15:08:51.000000 py-Ayiin-0.4.6.dev4/py_Ayiin.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1912 2023-06-11 15:08:51.000000 py-Ayiin-0.4.6.dev4/py_Ayiin.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-11 15:08:51.000000 py-Ayiin-0.4.6.dev4/py_Ayiin.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      149 2023-06-11 15:08:51.000000 py-Ayiin-0.4.6.dev4/py_Ayiin.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        8 2023-06-11 15:08:51.000000 py-Ayiin-0.4.6.dev4/py_Ayiin.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)      149 2023-06-11 15:08:42.000000 py-Ayiin-0.4.6.dev4/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-11 15:08:51.381365 py-Ayiin-0.4.6.dev4/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1641 2023-06-11 15:08:42.000000 py-Ayiin-0.4.6.dev4/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-12 16:36:09.986822 py-Ayiin-0.4.6.dev5/
+-rw-r--r--   0 runner    (1001) docker     (123)    35149 2023-06-12 16:36:00.000000 py-Ayiin-0.4.6.dev5/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)      147 2023-06-12 16:36:00.000000 py-Ayiin-0.4.6.dev5/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)      775 2023-06-12 16:36:00.000000 py-Ayiin-0.4.6.dev5/NOTICE
+-rw-r--r--   0 runner    (1001) docker     (123)     2572 2023-06-12 16:36:09.986822 py-Ayiin-0.4.6.dev5/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1642 2023-06-12 16:36:00.000000 py-Ayiin-0.4.6.dev5/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-12 16:36:09.978822 py-Ayiin-0.4.6.dev5/pyAyiin/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-12 16:36:09.978822 py-Ayiin-0.4.6.dev5/pyAyiin/Clients/
+-rw-r--r--   0 runner    (1001) docker     (123)      639 2023-06-12 16:36:00.000000 py-Ayiin-0.4.6.dev5/pyAyiin/Clients/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12525 2023-06-12 16:36:00.000000 py-Ayiin-0.4.6.dev5/pyAyiin/Clients/client.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6295 2023-06-12 16:36:00.000000 py-Ayiin-0.4.6.dev5/pyAyiin/Clients/pytgcalls.py
+-rw-r--r--   0 runner    (1001) docker     (123)    38781 2023-06-12 16:36:00.000000 py-Ayiin-0.4.6.dev5/pyAyiin/Clients/startup.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4570 2023-06-12 16:36:00.000000 py-Ayiin-0.4.6.dev5/pyAyiin/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1505 2023-06-12 16:36:00.000000 py-Ayiin-0.4.6.dev5/pyAyiin/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6704 2023-06-12 16:36:00.000000 py-Ayiin-0.4.6.dev5/pyAyiin/assistant.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5126 2023-06-12 16:36:00.000000 py-Ayiin-0.4.6.dev5/pyAyiin/config.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-12 16:36:09.982822 py-Ayiin-0.4.6.dev5/pyAyiin/dB/
+-rw-r--r--   0 runner    (1001) docker     (123)     1388 2023-06-12 16:36:00.000000 py-Ayiin-0.4.6.dev5/pyAyiin/dB/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      170 2023-06-12 16:36:00.000000 py-Ayiin-0.4.6.dev5/pyAyiin/dB/_core.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-12 16:36:00.000000 py-Ayiin-0.4.6.dev5/pyAyiin/dB/_session.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1330 2023-06-12 16:36:00.000000 py-Ayiin-0.4.6.dev5/pyAyiin/dB/absen.py
+-rw-r--r--   0 runner    (1001) docker     (123)      816 2023-06-12 16:36:00.000000 py-Ayiin-0.4.6.dev5/pyAyiin/dB/admins.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2255 2023-06-12 16:36:00.000000 py-Ayiin-0.4.6.dev5/pyAyiin/dB/auth.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1406 2023-06-12 16:36:00.000000 py-Ayiin-0.4.6.dev5/pyAyiin/dB/blacklistfilter.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1164 2023-06-12 16:36:00.000000 py-Ayiin-0.4.6.dev5/pyAyiin/dB/blacklistgcast.py
+-rw-r--r--   0 runner    (1001) docker     (123)      783 2023-06-12 16:36:00.000000 py-Ayiin-0.4.6.dev5/pyAyiin/dB/blacklistuser.py
+-rw-r--r--   0 runner    (1001) docker     (123)      706 2023-06-12 16:36:00.000000 py-Ayiin-0.4.6.dev5/pyAyiin/dB/gban.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1271 2023-06-12 16:36:00.000000 py-Ayiin-0.4.6.dev5/pyAyiin/dB/langs.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1049 2023-06-12 16:36:00.000000 py-Ayiin-0.4.6.dev5/pyAyiin/dB/logdb.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4755 2023-06-12 16:36:00.000000 py-Ayiin-0.4.6.dev5/pyAyiin/dB/pmpermit.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1331 2023-06-12 16:36:00.000000 py-Ayiin-0.4.6.dev5/pyAyiin/dB/premium.py
+-rw-r--r--   0 runner    (1001) docker     (123)      914 2023-06-12 16:36:00.000000 py-Ayiin-0.4.6.dev5/pyAyiin/dB/start.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1006 2023-06-12 16:36:00.000000 py-Ayiin-0.4.6.dev5/pyAyiin/dB/sudo.py
+-rw-r--r--   0 runner    (1001) docker     (123)      746 2023-06-12 16:36:00.000000 py-Ayiin-0.4.6.dev5/pyAyiin/dB/variable.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1251 2023-06-12 16:36:00.000000 py-Ayiin-0.4.6.dev5/pyAyiin/dB/videocalls.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2012 2023-06-12 16:36:00.000000 py-Ayiin-0.4.6.dev5/pyAyiin/dB/welcome.py
+-rw-r--r--   0 runner    (1001) docker     (123)    33973 2023-06-12 16:36:00.000000 py-Ayiin-0.4.6.dev5/pyAyiin/decorator.py
+-rw-r--r--   0 runner    (1001) docker     (123)      959 2023-06-12 16:36:00.000000 py-Ayiin-0.4.6.dev5/pyAyiin/exceptions.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-12 16:36:09.982822 py-Ayiin-0.4.6.dev5/pyAyiin/methods/
+-rw-r--r--   0 runner    (1001) docker     (123)      954 2023-06-12 16:36:00.000000 py-Ayiin-0.4.6.dev5/pyAyiin/methods/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10094 2023-06-12 16:36:00.000000 py-Ayiin-0.4.6.dev5/pyAyiin/methods/_database.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3939 2023-06-12 16:36:00.000000 py-Ayiin-0.4.6.dev5/pyAyiin/methods/_misc.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1897 2023-06-12 16:36:00.000000 py-Ayiin-0.4.6.dev5/pyAyiin/methods/changer.py
+-rw-r--r--   0 runner    (1001) docker     (123)      853 2023-06-12 16:36:00.000000 py-Ayiin-0.4.6.dev5/pyAyiin/methods/converter.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6909 2023-06-12 16:36:00.000000 py-Ayiin-0.4.6.dev5/pyAyiin/methods/func.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10022 2023-06-12 16:36:00.000000 py-Ayiin-0.4.6.dev5/pyAyiin/methods/funcb.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8828 2023-06-12 16:36:00.000000 py-Ayiin-0.4.6.dev5/pyAyiin/methods/helpers.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1213 2023-06-12 16:36:00.000000 py-Ayiin-0.4.6.dev5/pyAyiin/methods/hosting.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7703 2023-06-12 16:36:00.000000 py-Ayiin-0.4.6.dev5/pyAyiin/methods/inlinebot.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2879 2023-06-12 16:36:00.000000 py-Ayiin-0.4.6.dev5/pyAyiin/methods/queue.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6067 2023-06-12 16:36:00.000000 py-Ayiin-0.4.6.dev5/pyAyiin/methods/thumbnail.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-12 16:36:09.982822 py-Ayiin-0.4.6.dev5/pyAyiin/pyrogram/
+-rw-r--r--   0 runner    (1001) docker     (123)      612 2023-06-12 16:36:00.000000 py-Ayiin-0.4.6.dev5/pyAyiin/pyrogram/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2446 2023-06-12 16:36:00.000000 py-Ayiin-0.4.6.dev5/pyAyiin/pyrogram/_wrappers.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13157 2023-06-12 16:36:00.000000 py-Ayiin-0.4.6.dev5/pyAyiin/pyrogram/func.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3559 2023-06-12 16:36:00.000000 py-Ayiin-0.4.6.dev5/pyAyiin/pyrogram/misc.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1936 2023-06-12 16:36:00.000000 py-Ayiin-0.4.6.dev5/pyAyiin/pyrogram/pastebin.py
+-rw-r--r--   0 runner    (1001) docker     (123)      832 2023-06-12 16:36:00.000000 py-Ayiin-0.4.6.dev5/pyAyiin/pyrogram/sections.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2138 2023-06-12 16:36:00.000000 py-Ayiin-0.4.6.dev5/pyAyiin/pyrogram/toolbot.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8684 2023-06-12 16:36:00.000000 py-Ayiin-0.4.6.dev5/pyAyiin/pyrogram/tools.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-12 16:36:09.986822 py-Ayiin-0.4.6.dev5/pyAyiin/resources/
+-rw-r--r--   0 runner    (1001) docker     (123)   281001 2023-06-12 16:36:00.000000 py-Ayiin-0.4.6.dev5/pyAyiin/resources/Logo Ayiin.jpg
+-rw-r--r--   0 runner    (1001) docker     (123)    31343 2023-06-12 16:36:00.000000 py-Ayiin-0.4.6.dev5/pyAyiin/resources/Youtube.jpeg
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-12 16:36:00.000000 py-Ayiin-0.4.6.dev5/pyAyiin/resources/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    39497 2023-06-12 16:36:00.000000 py-Ayiin-0.4.6.dev5/pyAyiin/resources/ayiin_music.jpg
+-rw-r--r--   0 runner    (1001) docker     (123)  1808670 2023-06-12 16:36:00.000000 py-Ayiin-0.4.6.dev5/pyAyiin/resources/ayiin_ubot.jpg
+-rw-r--r--   0 runner    (1001) docker     (123)    60539 2023-06-12 16:36:00.000000 py-Ayiin-0.4.6.dev5/pyAyiin/resources/ayiin_userbot.jpg
+-rw-r--r--   0 runner    (1001) docker     (123)      889 2023-06-12 16:36:00.000000 py-Ayiin-0.4.6.dev5/pyAyiin/resources/blank.png
+-rw-r--r--   0 runner    (1001) docker     (123)    56364 2023-06-12 16:36:00.000000 py-Ayiin-0.4.6.dev5/pyAyiin/resources/default.ttf
+-rw-r--r--   0 runner    (1001) docker     (123)   141612 2023-06-12 16:36:00.000000 py-Ayiin-0.4.6.dev5/pyAyiin/resources/font.ttf
+-rw-r--r--   0 runner    (1001) docker     (123)   128248 2023-06-12 16:36:00.000000 py-Ayiin-0.4.6.dev5/pyAyiin/resources/font2.ttf
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-12 16:36:09.986822 py-Ayiin-0.4.6.dev5/pyAyiin/telethon/
+-rw-r--r--   0 runner    (1001) docker     (123)       31 2023-06-12 16:36:00.000000 py-Ayiin-0.4.6.dev5/pyAyiin/telethon/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-12 16:36:09.986822 py-Ayiin-0.4.6.dev5/pyAyiin/telethon/ayiin/
+-rw-r--r--   0 runner    (1001) docker     (123)      152 2023-06-12 16:36:00.000000 py-Ayiin-0.4.6.dev5/pyAyiin/telethon/ayiin/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1803 2023-06-12 16:36:00.000000 py-Ayiin-0.4.6.dev5/pyAyiin/telethon/ayiin/_wrappers.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3848 2023-06-12 16:36:00.000000 py-Ayiin-0.4.6.dev5/pyAyiin/telethon/ayiin/events.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6803 2023-06-12 16:36:00.000000 py-Ayiin-0.4.6.dev5/pyAyiin/telethon/ayiin/misc.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17263 2023-06-12 16:36:00.000000 py-Ayiin-0.4.6.dev5/pyAyiin/xd.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-12 16:36:09.986822 py-Ayiin-0.4.6.dev5/py_Ayiin.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     2572 2023-06-12 16:36:09.000000 py-Ayiin-0.4.6.dev5/py_Ayiin.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1912 2023-06-12 16:36:09.000000 py-Ayiin-0.4.6.dev5/py_Ayiin.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-12 16:36:09.000000 py-Ayiin-0.4.6.dev5/py_Ayiin.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      149 2023-06-12 16:36:09.000000 py-Ayiin-0.4.6.dev5/py_Ayiin.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        8 2023-06-12 16:36:09.000000 py-Ayiin-0.4.6.dev5/py_Ayiin.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      149 2023-06-12 16:36:00.000000 py-Ayiin-0.4.6.dev5/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-12 16:36:09.986822 py-Ayiin-0.4.6.dev5/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1641 2023-06-12 16:36:00.000000 py-Ayiin-0.4.6.dev5/setup.py
```

### Comparing `py-Ayiin-0.4.6.dev4/LICENSE` & `py-Ayiin-0.4.6.dev5/LICENSE`

 * *Files identical despite different names*

### Comparing `py-Ayiin-0.4.6.dev4/NOTICE` & `py-Ayiin-0.4.6.dev5/NOTICE`

 * *Files identical despite different names*

### Comparing `py-Ayiin-0.4.6.dev4/PKG-INFO` & `py-Ayiin-0.4.6.dev5/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: py-Ayiin
-Version: 0.4.6.dev4
+Version: 0.4.6.dev5
 Summary: A Secure and Powerful Python-Telethon Based and Python-Pyrogram Based Library For Your Userbot Module.
 Home-page: https://github.com/AyiinXd/AyiinXd
 Author: AyiinXd
 Author-email: ayingaming98@gmail.com
 License: GNU General Public License v3.0 (GPL-3.0)
 Project-URL: Bug Tracker, https://github.com/AyiinXd/AyiinXd/issues
 Project-URL: Source Code, https://github.com/AyiinXd/AyiinXd
```

### Comparing `py-Ayiin-0.4.6.dev4/README.md` & `py-Ayiin-0.4.6.dev5/README.md`

 * *Files identical despite different names*

### Comparing `py-Ayiin-0.4.6.dev4/pyAyiin/Clients/__init__.py` & `py-Ayiin-0.4.6.dev5/pyAyiin/Clients/__init__.py`

 * *Files identical despite different names*

### Comparing `py-Ayiin-0.4.6.dev4/pyAyiin/Clients/client.py` & `py-Ayiin-0.4.6.dev5/pyAyiin/Clients/client.py`

 * *Files identical despite different names*

### Comparing `py-Ayiin-0.4.6.dev4/pyAyiin/Clients/pytgcalls.py` & `py-Ayiin-0.4.6.dev5/pyAyiin/Clients/pytgcalls.py`

 * *Files 7% similar despite different names*

```diff
@@ -93,25 +93,29 @@
     ):
         group_call = await self.get_group_call(client, message, err_msg="group call already ended")
         if not group_call:
             return
         await client.invoke(DiscardGroupCall(call=group_call))
 
 
-class VcMusic(GroupCalls, Queues):
+class VcMusic(Queues):
     def __init__(self, client: Client, message: Message):
         self.m = message
         self.chat_id = []
         self.clients = {}
         self.client = client
         self.active_calls = []
         self.msgid_cache = {}
         self.play_on = {}
 
     async def startCall(self):
+        from pyAyiin.dB.langs import get_lang, get_string
+        
+        lang = await get_lang(self.client.me.id)
+        _ = get_string(lang)
         if PLAY_ON:
             for chats in PLAY_ON:
                 await PLAY_ON[chats].stop()
             PLAY_ON.clear()
             await asyncio.sleep(3)
         if self.m.video:
             for chats in list(CLIENTS):
@@ -122,20 +126,18 @@
         if self.m.chat.id not in ACTIVE_CALLS:
             try:
                 self.client.group_call.on_network_status_changed(
                     self.on_network_changed)
                 self.client.group_call.on_playout_ended(self.playout_ended_handler)
                 await self.client.group_call.join(self.m.chat.id)
             except GroupCallNotFoundError as er:
-                await self.m.reply(er)
-                dn, err = await self.StartVc()
-                if err:
-                    return False, err
+                await self.m.reply(_["err"].format(er))
+                return False, er
             except Exception as e:
-                await self.m.reply(e)
+                await self.m.reply(_["err"].format(e))
                 return False, e
         return True, None
 
     async def on_network_changed(self, call, is_connected):
         chat = self.m.chat.id
         if is_connected:
             if chat not in ACTIVE_CALLS:
@@ -145,31 +147,35 @@
 
     async def playout_ended_handler(self, call, source, mtype):
         if os.path.exists(source):
             os.remove(source)
         await self.play_from_queue()
 
     async def play_from_queue(self):
+        from pyAyiin.dB.langs import get_lang, get_string
+        
+        lang = await get_lang(self.client.me.id)
+        _ = get_string(lang)
         chat_id = self.m.chat.id
         if chat_id in PLAY_ON:
             await self.client.group_call.stop_video()
             PLAY_ON.pop(chat_id)
         try:
             ppk = await self.skip_song(self.client, chat_id)
             if ppk == 0:
                 await self.client.group_call.leave()
             elif ppk == 1:
-                await self.m.reply("<b>Antrian Udah Kosong Tod, Gua Cabut Dari OS</b>")
+                await self.m.reply(_["play_9"])
             else:
                 await self.m.reply(
-                    f"<b>• Memutar</b> - <a href='{ppk[1]}'>{ppk[0]}</a> | <code>{ppk[2]}</code>\n• <b>Pengguna:</b> {self.client.me.mention}",
+                    _["play_12"].format(ppk[1], ppk[0], ppk[2]),
                     disable_web_page_preview=True,
                 )
         except Exception as e:
-            await self.m.reply(e)
+            await self.m.reply(_["err"].format(e))
 
 
     async def JoinVc(self):
         chat_id = self.m.chat.id
         done, err = await self.startCall()
 
         if done:
```

### Comparing `py-Ayiin-0.4.6.dev4/pyAyiin/Clients/startup.py` & `py-Ayiin-0.4.6.dev5/pyAyiin/Clients/startup.py`

 * *Files 0% similar despite different names*

```diff
@@ -55,15 +55,15 @@
         plugins = Xd.import_module(
             "AyiinXd/",
             display_module=False,
             exclude=Var.NO_LOAD,
         )
         logs.info(f"{plugins} Total Plugins User")
         lang = await import_lang("languages/")
-        logs.info(f'Berhasil Mengambil Bahasa User')
+        logs.info('Berhasil Mengambil Bahasa Pengguna')
     except BaseException as e:
         logs.info(e)
         sys.exit()
     if Var.TELEBOT == "True":
         logs.info('Starting Telethon Bot...')
         await TeleBot.start(bot_token=Var.BOT_TOKEN)
         me = await TeleBot.get_me()
```

### Comparing `py-Ayiin-0.4.6.dev4/pyAyiin/__init__.py` & `py-Ayiin-0.4.6.dev5/pyAyiin/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -48,15 +48,15 @@
 
 
 logs = logging.getLogger(__name__)
 
 
 __copyright__ = "Copyright (C) 2022-present AyiinXd <https://github.com/AyiinXd>"
 __license__ = "GNU General Public License v3.0 (GPL-3.0)"
-__version__ = "0.4.6.dev04"
+__version__ = "0.4.6.dev05"
 ayiin_ver = "0.1.1"
 prem_version = "0.1"
 
 
 DEVS = [
     607067484, # Ayiin
     997461844, #Ayang_Ayiin
```

### Comparing `py-Ayiin-0.4.6.dev4/pyAyiin/__main__.py` & `py-Ayiin-0.4.6.dev5/pyAyiin/__main__.py`

 * *Files 4% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 
 from pyAyiin import __version__
 
 from . import *
 
 from .config import Var
 from .Clients.client import Bots
-from .Clients.startup import StartPyrogram
+from .Clients.startup import StartPyrogram, client_id
 
 yinsxd = Var()
 xd = PyrogramXd()
 
 
 try:
     from uvloop import install
```

### Comparing `py-Ayiin-0.4.6.dev4/pyAyiin/assistant.py` & `py-Ayiin-0.4.6.dev5/pyAyiin/assistant.py`

 * *Files identical despite different names*

### Comparing `py-Ayiin-0.4.6.dev4/pyAyiin/config.py` & `py-Ayiin-0.4.6.dev5/pyAyiin/config.py`

 * *Files identical despite different names*

### Comparing `py-Ayiin-0.4.6.dev4/pyAyiin/dB/__init__.py` & `py-Ayiin-0.4.6.dev5/pyAyiin/dB/__init__.py`

 * *Files identical despite different names*

### Comparing `py-Ayiin-0.4.6.dev4/pyAyiin/dB/absen.py` & `py-Ayiin-0.4.6.dev5/pyAyiin/dB/absen.py`

 * *Files identical despite different names*

### Comparing `py-Ayiin-0.4.6.dev4/pyAyiin/dB/admins.py` & `py-Ayiin-0.4.6.dev5/pyAyiin/dB/admins.py`

 * *Files identical despite different names*

### Comparing `py-Ayiin-0.4.6.dev4/pyAyiin/dB/auth.py` & `py-Ayiin-0.4.6.dev5/pyAyiin/dB/auth.py`

 * *Files identical despite different names*

### Comparing `py-Ayiin-0.4.6.dev4/pyAyiin/dB/blacklistfilter.py` & `py-Ayiin-0.4.6.dev5/pyAyiin/dB/blacklistfilter.py`

 * *Files identical despite different names*

### Comparing `py-Ayiin-0.4.6.dev4/pyAyiin/dB/blacklistgcast.py` & `py-Ayiin-0.4.6.dev5/pyAyiin/dB/blacklistgcast.py`

 * *Files identical despite different names*

### Comparing `py-Ayiin-0.4.6.dev4/pyAyiin/dB/blacklistuser.py` & `py-Ayiin-0.4.6.dev5/pyAyiin/dB/blacklistuser.py`

 * *Files identical despite different names*

### Comparing `py-Ayiin-0.4.6.dev4/pyAyiin/dB/gban.py` & `py-Ayiin-0.4.6.dev5/pyAyiin/dB/gban.py`

 * *Files identical despite different names*

### Comparing `py-Ayiin-0.4.6.dev4/pyAyiin/dB/langs.py` & `py-Ayiin-0.4.6.dev5/pyAyiin/dB/langs.py`

 * *Files identical despite different names*

### Comparing `py-Ayiin-0.4.6.dev4/pyAyiin/dB/logdb.py` & `py-Ayiin-0.4.6.dev5/pyAyiin/dB/logdb.py`

 * *Files identical despite different names*

### Comparing `py-Ayiin-0.4.6.dev4/pyAyiin/dB/pmpermit.py` & `py-Ayiin-0.4.6.dev5/pyAyiin/dB/pmpermit.py`

 * *Files identical despite different names*

### Comparing `py-Ayiin-0.4.6.dev4/pyAyiin/dB/premium.py` & `py-Ayiin-0.4.6.dev5/pyAyiin/dB/premium.py`

 * *Files identical despite different names*

### Comparing `py-Ayiin-0.4.6.dev4/pyAyiin/dB/start.py` & `py-Ayiin-0.4.6.dev5/pyAyiin/dB/start.py`

 * *Files identical despite different names*

### Comparing `py-Ayiin-0.4.6.dev4/pyAyiin/dB/sudo.py` & `py-Ayiin-0.4.6.dev5/pyAyiin/dB/sudo.py`

 * *Files identical despite different names*

### Comparing `py-Ayiin-0.4.6.dev4/pyAyiin/dB/variable.py` & `py-Ayiin-0.4.6.dev5/pyAyiin/dB/variable.py`

 * *Files identical despite different names*

### Comparing `py-Ayiin-0.4.6.dev4/pyAyiin/dB/videocalls.py` & `py-Ayiin-0.4.6.dev5/pyAyiin/dB/videocalls.py`

 * *Files identical despite different names*

### Comparing `py-Ayiin-0.4.6.dev4/pyAyiin/dB/welcome.py` & `py-Ayiin-0.4.6.dev5/pyAyiin/dB/welcome.py`

 * *Files identical despite different names*

### Comparing `py-Ayiin-0.4.6.dev4/pyAyiin/decorator.py` & `py-Ayiin-0.4.6.dev5/pyAyiin/decorator.py`

 * *Files identical despite different names*

### Comparing `py-Ayiin-0.4.6.dev4/pyAyiin/exceptions.py` & `py-Ayiin-0.4.6.dev5/pyAyiin/exceptions.py`

 * *Files identical despite different names*

### Comparing `py-Ayiin-0.4.6.dev4/pyAyiin/methods/__init__.py` & `py-Ayiin-0.4.6.dev5/pyAyiin/methods/__init__.py`

 * *Files identical despite different names*

### Comparing `py-Ayiin-0.4.6.dev4/pyAyiin/methods/_database.py` & `py-Ayiin-0.4.6.dev5/pyAyiin/methods/_database.py`

 * *Files identical despite different names*

### Comparing `py-Ayiin-0.4.6.dev4/pyAyiin/methods/_misc.py` & `py-Ayiin-0.4.6.dev5/pyAyiin/methods/_misc.py`

 * *Files identical despite different names*

### Comparing `py-Ayiin-0.4.6.dev4/pyAyiin/methods/changer.py` & `py-Ayiin-0.4.6.dev5/pyAyiin/methods/changer.py`

 * *Files identical despite different names*

### Comparing `py-Ayiin-0.4.6.dev4/pyAyiin/methods/converter.py` & `py-Ayiin-0.4.6.dev5/pyAyiin/methods/converter.py`

 * *Files identical despite different names*

### Comparing `py-Ayiin-0.4.6.dev4/pyAyiin/methods/func.py` & `py-Ayiin-0.4.6.dev5/pyAyiin/methods/func.py`

 * *Files identical despite different names*

### Comparing `py-Ayiin-0.4.6.dev4/pyAyiin/methods/helpers.py` & `py-Ayiin-0.4.6.dev5/pyAyiin/methods/helpers.py`

 * *Files identical despite different names*

### Comparing `py-Ayiin-0.4.6.dev4/pyAyiin/methods/hosting.py` & `py-Ayiin-0.4.6.dev5/pyAyiin/methods/hosting.py`

 * *Files identical despite different names*

### Comparing `py-Ayiin-0.4.6.dev4/pyAyiin/methods/inlinebot.py` & `py-Ayiin-0.4.6.dev5/pyAyiin/methods/inlinebot.py`

 * *Files 2% similar despite different names*

```diff
@@ -186,17 +186,18 @@
                         input_message_content=InputTextMessageContent(output),
                     )
                 )
             ]
         return results
     
     async def inline_languages(self, _):
-        from pyAyiin.dB.langs import get_languages
+        from pyAyiin.dB.langs import get_lang, get_languages
         
-        text = _["lang"]
+        lang = await get_lang
+        text = _["lang"].format(lang)
         languages = get_languages()
         tutud = [
             InlineKeyboardButton(
                 f"{languages[yins]['nama']}",
                 callback_data=f"set_{yins}",
             )
             for yins in languages
```

### Comparing `py-Ayiin-0.4.6.dev4/pyAyiin/methods/queue.py` & `py-Ayiin-0.4.6.dev5/pyAyiin/methods/queue.py`

 * *Files identical despite different names*

### Comparing `py-Ayiin-0.4.6.dev4/pyAyiin/methods/thumbnail.py` & `py-Ayiin-0.4.6.dev5/pyAyiin/methods/thumbnail.py`

 * *Files identical despite different names*

### Comparing `py-Ayiin-0.4.6.dev4/pyAyiin/pyrogram/__init__.py` & `py-Ayiin-0.4.6.dev5/pyAyiin/pyrogram/__init__.py`

 * *Files identical despite different names*

### Comparing `py-Ayiin-0.4.6.dev4/pyAyiin/pyrogram/_wrappers.py` & `py-Ayiin-0.4.6.dev5/pyAyiin/pyrogram/_wrappers.py`

 * *Files identical despite different names*

### Comparing `py-Ayiin-0.4.6.dev4/pyAyiin/pyrogram/func.py` & `py-Ayiin-0.4.6.dev5/pyAyiin/pyrogram/func.py`

 * *Files identical despite different names*

### Comparing `py-Ayiin-0.4.6.dev4/pyAyiin/pyrogram/misc.py` & `py-Ayiin-0.4.6.dev5/pyAyiin/pyrogram/misc.py`

 * *Files identical despite different names*

### Comparing `py-Ayiin-0.4.6.dev4/pyAyiin/pyrogram/pastebin.py` & `py-Ayiin-0.4.6.dev5/pyAyiin/pyrogram/pastebin.py`

 * *Files identical despite different names*

### Comparing `py-Ayiin-0.4.6.dev4/pyAyiin/pyrogram/sections.py` & `py-Ayiin-0.4.6.dev5/pyAyiin/pyrogram/sections.py`

 * *Files identical despite different names*

### Comparing `py-Ayiin-0.4.6.dev4/pyAyiin/pyrogram/toolbot.py` & `py-Ayiin-0.4.6.dev5/pyAyiin/pyrogram/toolbot.py`

 * *Files identical despite different names*

### Comparing `py-Ayiin-0.4.6.dev4/pyAyiin/pyrogram/tools.py` & `py-Ayiin-0.4.6.dev5/pyAyiin/pyrogram/tools.py`

 * *Files identical despite different names*

### Comparing `py-Ayiin-0.4.6.dev4/pyAyiin/resources/Logo Ayiin.jpg` & `py-Ayiin-0.4.6.dev5/pyAyiin/resources/Logo Ayiin.jpg`

 * *Files identical despite different names*

### Comparing `py-Ayiin-0.4.6.dev4/pyAyiin/resources/Youtube.jpeg` & `py-Ayiin-0.4.6.dev5/pyAyiin/resources/Youtube.jpeg`

 * *Files identical despite different names*

### Comparing `py-Ayiin-0.4.6.dev4/pyAyiin/resources/ayiin_music.jpg` & `py-Ayiin-0.4.6.dev5/pyAyiin/resources/ayiin_music.jpg`

 * *Files identical despite different names*

### Comparing `py-Ayiin-0.4.6.dev4/pyAyiin/resources/ayiin_ubot.jpg` & `py-Ayiin-0.4.6.dev5/pyAyiin/resources/ayiin_ubot.jpg`

 * *Files identical despite different names*

### Comparing `py-Ayiin-0.4.6.dev4/pyAyiin/resources/ayiin_userbot.jpg` & `py-Ayiin-0.4.6.dev5/pyAyiin/resources/ayiin_userbot.jpg`

 * *Files identical despite different names*

### Comparing `py-Ayiin-0.4.6.dev4/pyAyiin/resources/blank.png` & `py-Ayiin-0.4.6.dev5/pyAyiin/resources/blank.png`

 * *Files identical despite different names*

### Comparing `py-Ayiin-0.4.6.dev4/pyAyiin/resources/default.ttf` & `py-Ayiin-0.4.6.dev5/pyAyiin/resources/default.ttf`

 * *Files identical despite different names*

### Comparing `py-Ayiin-0.4.6.dev4/pyAyiin/resources/font.ttf` & `py-Ayiin-0.4.6.dev5/pyAyiin/resources/font.ttf`

 * *Files identical despite different names*

### Comparing `py-Ayiin-0.4.6.dev4/pyAyiin/resources/font2.ttf` & `py-Ayiin-0.4.6.dev5/pyAyiin/resources/font2.ttf`

 * *Files identical despite different names*

### Comparing `py-Ayiin-0.4.6.dev4/pyAyiin/telethon/ayiin/_wrappers.py` & `py-Ayiin-0.4.6.dev5/pyAyiin/telethon/ayiin/_wrappers.py`

 * *Files identical despite different names*

### Comparing `py-Ayiin-0.4.6.dev4/pyAyiin/telethon/ayiin/events.py` & `py-Ayiin-0.4.6.dev5/pyAyiin/telethon/ayiin/events.py`

 * *Files identical despite different names*

### Comparing `py-Ayiin-0.4.6.dev4/pyAyiin/telethon/ayiin/misc.py` & `py-Ayiin-0.4.6.dev5/pyAyiin/telethon/ayiin/misc.py`

 * *Files identical despite different names*

### Comparing `py-Ayiin-0.4.6.dev4/pyAyiin/xd.py` & `py-Ayiin-0.4.6.dev5/pyAyiin/xd.py`

 * *Files identical despite different names*

### Comparing `py-Ayiin-0.4.6.dev4/py_Ayiin.egg-info/PKG-INFO` & `py-Ayiin-0.4.6.dev5/py_Ayiin.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: py-Ayiin
-Version: 0.4.6.dev4
+Version: 0.4.6.dev5
 Summary: A Secure and Powerful Python-Telethon Based and Python-Pyrogram Based Library For Your Userbot Module.
 Home-page: https://github.com/AyiinXd/AyiinXd
 Author: AyiinXd
 Author-email: ayingaming98@gmail.com
 License: GNU General Public License v3.0 (GPL-3.0)
 Project-URL: Bug Tracker, https://github.com/AyiinXd/AyiinXd/issues
 Project-URL: Source Code, https://github.com/AyiinXd/AyiinXd
```

### Comparing `py-Ayiin-0.4.6.dev4/py_Ayiin.egg-info/SOURCES.txt` & `py-Ayiin-0.4.6.dev5/py_Ayiin.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `py-Ayiin-0.4.6.dev4/setup.py` & `py-Ayiin-0.4.6.dev5/setup.py`

 * *Files identical despite different names*

