# Comparing `tmp/py-Ayiin-0.4.6.dev6.tar.gz` & `tmp/py-Ayiin-0.4.6.dev7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "py-Ayiin-0.4.6.dev6.tar", last modified: Mon Jun 12 16:42:01 2023, max compression
+gzip compressed data, was "py-Ayiin-0.4.6.dev7.tar", last modified: Mon Jun 12 17:22:51 2023, max compression
```

## Comparing `py-Ayiin-0.4.6.dev6.tar` & `py-Ayiin-0.4.6.dev7.tar`

### file list

```diff
@@ -1,88 +1,88 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-12 16:42:01.509876 py-Ayiin-0.4.6.dev6/
--rw-r--r--   0 runner    (1001) docker     (123)    35149 2023-06-12 16:41:52.000000 py-Ayiin-0.4.6.dev6/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)      147 2023-06-12 16:41:52.000000 py-Ayiin-0.4.6.dev6/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)      775 2023-06-12 16:41:52.000000 py-Ayiin-0.4.6.dev6/NOTICE
--rw-r--r--   0 runner    (1001) docker     (123)     2572 2023-06-12 16:42:01.505876 py-Ayiin-0.4.6.dev6/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1642 2023-06-12 16:41:52.000000 py-Ayiin-0.4.6.dev6/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-12 16:42:01.497876 py-Ayiin-0.4.6.dev6/pyAyiin/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-12 16:42:01.497876 py-Ayiin-0.4.6.dev6/pyAyiin/Clients/
--rw-r--r--   0 runner    (1001) docker     (123)      639 2023-06-12 16:41:52.000000 py-Ayiin-0.4.6.dev6/pyAyiin/Clients/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    12525 2023-06-12 16:41:52.000000 py-Ayiin-0.4.6.dev6/pyAyiin/Clients/client.py
--rw-r--r--   0 runner    (1001) docker     (123)     6295 2023-06-12 16:41:52.000000 py-Ayiin-0.4.6.dev6/pyAyiin/Clients/pytgcalls.py
--rw-r--r--   0 runner    (1001) docker     (123)    38781 2023-06-12 16:41:52.000000 py-Ayiin-0.4.6.dev6/pyAyiin/Clients/startup.py
--rw-r--r--   0 runner    (1001) docker     (123)     4570 2023-06-12 16:41:52.000000 py-Ayiin-0.4.6.dev6/pyAyiin/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1505 2023-06-12 16:41:52.000000 py-Ayiin-0.4.6.dev6/pyAyiin/__main__.py
--rw-r--r--   0 runner    (1001) docker     (123)     6704 2023-06-12 16:41:52.000000 py-Ayiin-0.4.6.dev6/pyAyiin/assistant.py
--rw-r--r--   0 runner    (1001) docker     (123)     5126 2023-06-12 16:41:52.000000 py-Ayiin-0.4.6.dev6/pyAyiin/config.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-12 16:42:01.501875 py-Ayiin-0.4.6.dev6/pyAyiin/dB/
--rw-r--r--   0 runner    (1001) docker     (123)     1388 2023-06-12 16:41:52.000000 py-Ayiin-0.4.6.dev6/pyAyiin/dB/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      170 2023-06-12 16:41:52.000000 py-Ayiin-0.4.6.dev6/pyAyiin/dB/_core.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-12 16:41:52.000000 py-Ayiin-0.4.6.dev6/pyAyiin/dB/_session.py
--rw-r--r--   0 runner    (1001) docker     (123)     1330 2023-06-12 16:41:52.000000 py-Ayiin-0.4.6.dev6/pyAyiin/dB/absen.py
--rw-r--r--   0 runner    (1001) docker     (123)      816 2023-06-12 16:41:52.000000 py-Ayiin-0.4.6.dev6/pyAyiin/dB/admins.py
--rw-r--r--   0 runner    (1001) docker     (123)     2255 2023-06-12 16:41:52.000000 py-Ayiin-0.4.6.dev6/pyAyiin/dB/auth.py
--rw-r--r--   0 runner    (1001) docker     (123)     1406 2023-06-12 16:41:52.000000 py-Ayiin-0.4.6.dev6/pyAyiin/dB/blacklistfilter.py
--rw-r--r--   0 runner    (1001) docker     (123)     1164 2023-06-12 16:41:52.000000 py-Ayiin-0.4.6.dev6/pyAyiin/dB/blacklistgcast.py
--rw-r--r--   0 runner    (1001) docker     (123)      783 2023-06-12 16:41:52.000000 py-Ayiin-0.4.6.dev6/pyAyiin/dB/blacklistuser.py
--rw-r--r--   0 runner    (1001) docker     (123)      706 2023-06-12 16:41:52.000000 py-Ayiin-0.4.6.dev6/pyAyiin/dB/gban.py
--rw-r--r--   0 runner    (1001) docker     (123)     1271 2023-06-12 16:41:52.000000 py-Ayiin-0.4.6.dev6/pyAyiin/dB/langs.py
--rw-r--r--   0 runner    (1001) docker     (123)     1049 2023-06-12 16:41:52.000000 py-Ayiin-0.4.6.dev6/pyAyiin/dB/logdb.py
--rw-r--r--   0 runner    (1001) docker     (123)     4755 2023-06-12 16:41:52.000000 py-Ayiin-0.4.6.dev6/pyAyiin/dB/pmpermit.py
--rw-r--r--   0 runner    (1001) docker     (123)     1331 2023-06-12 16:41:52.000000 py-Ayiin-0.4.6.dev6/pyAyiin/dB/premium.py
--rw-r--r--   0 runner    (1001) docker     (123)      914 2023-06-12 16:41:52.000000 py-Ayiin-0.4.6.dev6/pyAyiin/dB/start.py
--rw-r--r--   0 runner    (1001) docker     (123)     1006 2023-06-12 16:41:52.000000 py-Ayiin-0.4.6.dev6/pyAyiin/dB/sudo.py
--rw-r--r--   0 runner    (1001) docker     (123)      746 2023-06-12 16:41:52.000000 py-Ayiin-0.4.6.dev6/pyAyiin/dB/variable.py
--rw-r--r--   0 runner    (1001) docker     (123)     1251 2023-06-12 16:41:52.000000 py-Ayiin-0.4.6.dev6/pyAyiin/dB/videocalls.py
--rw-r--r--   0 runner    (1001) docker     (123)     2012 2023-06-12 16:41:52.000000 py-Ayiin-0.4.6.dev6/pyAyiin/dB/welcome.py
--rw-r--r--   0 runner    (1001) docker     (123)    33973 2023-06-12 16:41:52.000000 py-Ayiin-0.4.6.dev6/pyAyiin/decorator.py
--rw-r--r--   0 runner    (1001) docker     (123)      959 2023-06-12 16:41:52.000000 py-Ayiin-0.4.6.dev6/pyAyiin/exceptions.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-12 16:42:01.501875 py-Ayiin-0.4.6.dev6/pyAyiin/methods/
--rw-r--r--   0 runner    (1001) docker     (123)      954 2023-06-12 16:41:52.000000 py-Ayiin-0.4.6.dev6/pyAyiin/methods/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    10094 2023-06-12 16:41:52.000000 py-Ayiin-0.4.6.dev6/pyAyiin/methods/_database.py
--rw-r--r--   0 runner    (1001) docker     (123)     3939 2023-06-12 16:41:52.000000 py-Ayiin-0.4.6.dev6/pyAyiin/methods/_misc.py
--rw-r--r--   0 runner    (1001) docker     (123)     1897 2023-06-12 16:41:52.000000 py-Ayiin-0.4.6.dev6/pyAyiin/methods/changer.py
--rw-r--r--   0 runner    (1001) docker     (123)      853 2023-06-12 16:41:52.000000 py-Ayiin-0.4.6.dev6/pyAyiin/methods/converter.py
--rw-r--r--   0 runner    (1001) docker     (123)     6909 2023-06-12 16:41:52.000000 py-Ayiin-0.4.6.dev6/pyAyiin/methods/func.py
--rw-r--r--   0 runner    (1001) docker     (123)    10022 2023-06-12 16:41:52.000000 py-Ayiin-0.4.6.dev6/pyAyiin/methods/funcb.py
--rw-r--r--   0 runner    (1001) docker     (123)     8828 2023-06-12 16:41:52.000000 py-Ayiin-0.4.6.dev6/pyAyiin/methods/helpers.py
--rw-r--r--   0 runner    (1001) docker     (123)     1213 2023-06-12 16:41:52.000000 py-Ayiin-0.4.6.dev6/pyAyiin/methods/hosting.py
--rw-r--r--   0 runner    (1001) docker     (123)     7713 2023-06-12 16:41:52.000000 py-Ayiin-0.4.6.dev6/pyAyiin/methods/inlinebot.py
--rw-r--r--   0 runner    (1001) docker     (123)     2879 2023-06-12 16:41:52.000000 py-Ayiin-0.4.6.dev6/pyAyiin/methods/queue.py
--rw-r--r--   0 runner    (1001) docker     (123)     6067 2023-06-12 16:41:52.000000 py-Ayiin-0.4.6.dev6/pyAyiin/methods/thumbnail.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-12 16:42:01.501875 py-Ayiin-0.4.6.dev6/pyAyiin/pyrogram/
--rw-r--r--   0 runner    (1001) docker     (123)      612 2023-06-12 16:41:52.000000 py-Ayiin-0.4.6.dev6/pyAyiin/pyrogram/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2446 2023-06-12 16:41:52.000000 py-Ayiin-0.4.6.dev6/pyAyiin/pyrogram/_wrappers.py
--rw-r--r--   0 runner    (1001) docker     (123)    13157 2023-06-12 16:41:52.000000 py-Ayiin-0.4.6.dev6/pyAyiin/pyrogram/func.py
--rw-r--r--   0 runner    (1001) docker     (123)     3559 2023-06-12 16:41:52.000000 py-Ayiin-0.4.6.dev6/pyAyiin/pyrogram/misc.py
--rw-r--r--   0 runner    (1001) docker     (123)     1936 2023-06-12 16:41:52.000000 py-Ayiin-0.4.6.dev6/pyAyiin/pyrogram/pastebin.py
--rw-r--r--   0 runner    (1001) docker     (123)      832 2023-06-12 16:41:52.000000 py-Ayiin-0.4.6.dev6/pyAyiin/pyrogram/sections.py
--rw-r--r--   0 runner    (1001) docker     (123)     2138 2023-06-12 16:41:52.000000 py-Ayiin-0.4.6.dev6/pyAyiin/pyrogram/toolbot.py
--rw-r--r--   0 runner    (1001) docker     (123)     8684 2023-06-12 16:41:52.000000 py-Ayiin-0.4.6.dev6/pyAyiin/pyrogram/tools.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-12 16:42:01.505876 py-Ayiin-0.4.6.dev6/pyAyiin/resources/
--rw-r--r--   0 runner    (1001) docker     (123)   281001 2023-06-12 16:41:52.000000 py-Ayiin-0.4.6.dev6/pyAyiin/resources/Logo Ayiin.jpg
--rw-r--r--   0 runner    (1001) docker     (123)    31343 2023-06-12 16:41:52.000000 py-Ayiin-0.4.6.dev6/pyAyiin/resources/Youtube.jpeg
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-12 16:41:52.000000 py-Ayiin-0.4.6.dev6/pyAyiin/resources/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    39497 2023-06-12 16:41:52.000000 py-Ayiin-0.4.6.dev6/pyAyiin/resources/ayiin_music.jpg
--rw-r--r--   0 runner    (1001) docker     (123)  1808670 2023-06-12 16:41:52.000000 py-Ayiin-0.4.6.dev6/pyAyiin/resources/ayiin_ubot.jpg
--rw-r--r--   0 runner    (1001) docker     (123)    60539 2023-06-12 16:41:52.000000 py-Ayiin-0.4.6.dev6/pyAyiin/resources/ayiin_userbot.jpg
--rw-r--r--   0 runner    (1001) docker     (123)      889 2023-06-12 16:41:52.000000 py-Ayiin-0.4.6.dev6/pyAyiin/resources/blank.png
--rw-r--r--   0 runner    (1001) docker     (123)    56364 2023-06-12 16:41:52.000000 py-Ayiin-0.4.6.dev6/pyAyiin/resources/default.ttf
--rw-r--r--   0 runner    (1001) docker     (123)   141612 2023-06-12 16:41:52.000000 py-Ayiin-0.4.6.dev6/pyAyiin/resources/font.ttf
--rw-r--r--   0 runner    (1001) docker     (123)   128248 2023-06-12 16:41:52.000000 py-Ayiin-0.4.6.dev6/pyAyiin/resources/font2.ttf
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-12 16:42:01.505876 py-Ayiin-0.4.6.dev6/pyAyiin/telethon/
--rw-r--r--   0 runner    (1001) docker     (123)       31 2023-06-12 16:41:52.000000 py-Ayiin-0.4.6.dev6/pyAyiin/telethon/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-12 16:42:01.505876 py-Ayiin-0.4.6.dev6/pyAyiin/telethon/ayiin/
--rw-r--r--   0 runner    (1001) docker     (123)      152 2023-06-12 16:41:52.000000 py-Ayiin-0.4.6.dev6/pyAyiin/telethon/ayiin/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1803 2023-06-12 16:41:52.000000 py-Ayiin-0.4.6.dev6/pyAyiin/telethon/ayiin/_wrappers.py
--rw-r--r--   0 runner    (1001) docker     (123)     3848 2023-06-12 16:41:52.000000 py-Ayiin-0.4.6.dev6/pyAyiin/telethon/ayiin/events.py
--rw-r--r--   0 runner    (1001) docker     (123)     6803 2023-06-12 16:41:52.000000 py-Ayiin-0.4.6.dev6/pyAyiin/telethon/ayiin/misc.py
--rw-r--r--   0 runner    (1001) docker     (123)    17263 2023-06-12 16:41:52.000000 py-Ayiin-0.4.6.dev6/pyAyiin/xd.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-12 16:42:01.505876 py-Ayiin-0.4.6.dev6/py_Ayiin.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     2572 2023-06-12 16:42:01.000000 py-Ayiin-0.4.6.dev6/py_Ayiin.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1912 2023-06-12 16:42:01.000000 py-Ayiin-0.4.6.dev6/py_Ayiin.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-12 16:42:01.000000 py-Ayiin-0.4.6.dev6/py_Ayiin.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      149 2023-06-12 16:42:01.000000 py-Ayiin-0.4.6.dev6/py_Ayiin.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        8 2023-06-12 16:42:01.000000 py-Ayiin-0.4.6.dev6/py_Ayiin.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)      149 2023-06-12 16:41:52.000000 py-Ayiin-0.4.6.dev6/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-12 16:42:01.509876 py-Ayiin-0.4.6.dev6/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1641 2023-06-12 16:41:52.000000 py-Ayiin-0.4.6.dev6/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-12 17:22:51.128386 py-Ayiin-0.4.6.dev7/
+-rw-r--r--   0 runner    (1001) docker     (123)    35149 2023-06-12 17:22:37.000000 py-Ayiin-0.4.6.dev7/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)      147 2023-06-12 17:22:37.000000 py-Ayiin-0.4.6.dev7/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)      775 2023-06-12 17:22:37.000000 py-Ayiin-0.4.6.dev7/NOTICE
+-rw-r--r--   0 runner    (1001) docker     (123)     2572 2023-06-12 17:22:51.128386 py-Ayiin-0.4.6.dev7/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1642 2023-06-12 17:22:37.000000 py-Ayiin-0.4.6.dev7/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-12 17:22:51.120386 py-Ayiin-0.4.6.dev7/pyAyiin/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-12 17:22:51.120386 py-Ayiin-0.4.6.dev7/pyAyiin/Clients/
+-rw-r--r--   0 runner    (1001) docker     (123)      639 2023-06-12 17:22:37.000000 py-Ayiin-0.4.6.dev7/pyAyiin/Clients/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12525 2023-06-12 17:22:37.000000 py-Ayiin-0.4.6.dev7/pyAyiin/Clients/client.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6313 2023-06-12 17:22:37.000000 py-Ayiin-0.4.6.dev7/pyAyiin/Clients/pytgcalls.py
+-rw-r--r--   0 runner    (1001) docker     (123)    38781 2023-06-12 17:22:37.000000 py-Ayiin-0.4.6.dev7/pyAyiin/Clients/startup.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4570 2023-06-12 17:22:37.000000 py-Ayiin-0.4.6.dev7/pyAyiin/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1505 2023-06-12 17:22:37.000000 py-Ayiin-0.4.6.dev7/pyAyiin/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6704 2023-06-12 17:22:37.000000 py-Ayiin-0.4.6.dev7/pyAyiin/assistant.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5126 2023-06-12 17:22:37.000000 py-Ayiin-0.4.6.dev7/pyAyiin/config.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-12 17:22:51.124386 py-Ayiin-0.4.6.dev7/pyAyiin/dB/
+-rw-r--r--   0 runner    (1001) docker     (123)     1388 2023-06-12 17:22:37.000000 py-Ayiin-0.4.6.dev7/pyAyiin/dB/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      170 2023-06-12 17:22:37.000000 py-Ayiin-0.4.6.dev7/pyAyiin/dB/_core.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-12 17:22:37.000000 py-Ayiin-0.4.6.dev7/pyAyiin/dB/_session.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1330 2023-06-12 17:22:37.000000 py-Ayiin-0.4.6.dev7/pyAyiin/dB/absen.py
+-rw-r--r--   0 runner    (1001) docker     (123)      816 2023-06-12 17:22:37.000000 py-Ayiin-0.4.6.dev7/pyAyiin/dB/admins.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2255 2023-06-12 17:22:37.000000 py-Ayiin-0.4.6.dev7/pyAyiin/dB/auth.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1406 2023-06-12 17:22:37.000000 py-Ayiin-0.4.6.dev7/pyAyiin/dB/blacklistfilter.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1164 2023-06-12 17:22:37.000000 py-Ayiin-0.4.6.dev7/pyAyiin/dB/blacklistgcast.py
+-rw-r--r--   0 runner    (1001) docker     (123)      783 2023-06-12 17:22:37.000000 py-Ayiin-0.4.6.dev7/pyAyiin/dB/blacklistuser.py
+-rw-r--r--   0 runner    (1001) docker     (123)      706 2023-06-12 17:22:37.000000 py-Ayiin-0.4.6.dev7/pyAyiin/dB/gban.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1271 2023-06-12 17:22:37.000000 py-Ayiin-0.4.6.dev7/pyAyiin/dB/langs.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1049 2023-06-12 17:22:37.000000 py-Ayiin-0.4.6.dev7/pyAyiin/dB/logdb.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4755 2023-06-12 17:22:37.000000 py-Ayiin-0.4.6.dev7/pyAyiin/dB/pmpermit.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1331 2023-06-12 17:22:37.000000 py-Ayiin-0.4.6.dev7/pyAyiin/dB/premium.py
+-rw-r--r--   0 runner    (1001) docker     (123)      914 2023-06-12 17:22:37.000000 py-Ayiin-0.4.6.dev7/pyAyiin/dB/start.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1006 2023-06-12 17:22:37.000000 py-Ayiin-0.4.6.dev7/pyAyiin/dB/sudo.py
+-rw-r--r--   0 runner    (1001) docker     (123)      746 2023-06-12 17:22:37.000000 py-Ayiin-0.4.6.dev7/pyAyiin/dB/variable.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1251 2023-06-12 17:22:37.000000 py-Ayiin-0.4.6.dev7/pyAyiin/dB/videocalls.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2012 2023-06-12 17:22:37.000000 py-Ayiin-0.4.6.dev7/pyAyiin/dB/welcome.py
+-rw-r--r--   0 runner    (1001) docker     (123)    33973 2023-06-12 17:22:37.000000 py-Ayiin-0.4.6.dev7/pyAyiin/decorator.py
+-rw-r--r--   0 runner    (1001) docker     (123)      959 2023-06-12 17:22:37.000000 py-Ayiin-0.4.6.dev7/pyAyiin/exceptions.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-12 17:22:51.124386 py-Ayiin-0.4.6.dev7/pyAyiin/methods/
+-rw-r--r--   0 runner    (1001) docker     (123)      954 2023-06-12 17:22:37.000000 py-Ayiin-0.4.6.dev7/pyAyiin/methods/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10094 2023-06-12 17:22:37.000000 py-Ayiin-0.4.6.dev7/pyAyiin/methods/_database.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3939 2023-06-12 17:22:37.000000 py-Ayiin-0.4.6.dev7/pyAyiin/methods/_misc.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1897 2023-06-12 17:22:37.000000 py-Ayiin-0.4.6.dev7/pyAyiin/methods/changer.py
+-rw-r--r--   0 runner    (1001) docker     (123)      853 2023-06-12 17:22:37.000000 py-Ayiin-0.4.6.dev7/pyAyiin/methods/converter.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6909 2023-06-12 17:22:37.000000 py-Ayiin-0.4.6.dev7/pyAyiin/methods/func.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12691 2023-06-12 17:22:37.000000 py-Ayiin-0.4.6.dev7/pyAyiin/methods/funcb.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8828 2023-06-12 17:22:37.000000 py-Ayiin-0.4.6.dev7/pyAyiin/methods/helpers.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1213 2023-06-12 17:22:37.000000 py-Ayiin-0.4.6.dev7/pyAyiin/methods/hosting.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7650 2023-06-12 17:22:37.000000 py-Ayiin-0.4.6.dev7/pyAyiin/methods/inlinebot.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2879 2023-06-12 17:22:37.000000 py-Ayiin-0.4.6.dev7/pyAyiin/methods/queue.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6067 2023-06-12 17:22:37.000000 py-Ayiin-0.4.6.dev7/pyAyiin/methods/thumbnail.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-12 17:22:51.124386 py-Ayiin-0.4.6.dev7/pyAyiin/pyrogram/
+-rw-r--r--   0 runner    (1001) docker     (123)      612 2023-06-12 17:22:37.000000 py-Ayiin-0.4.6.dev7/pyAyiin/pyrogram/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2446 2023-06-12 17:22:37.000000 py-Ayiin-0.4.6.dev7/pyAyiin/pyrogram/_wrappers.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13157 2023-06-12 17:22:37.000000 py-Ayiin-0.4.6.dev7/pyAyiin/pyrogram/func.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3559 2023-06-12 17:22:37.000000 py-Ayiin-0.4.6.dev7/pyAyiin/pyrogram/misc.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1936 2023-06-12 17:22:37.000000 py-Ayiin-0.4.6.dev7/pyAyiin/pyrogram/pastebin.py
+-rw-r--r--   0 runner    (1001) docker     (123)      832 2023-06-12 17:22:37.000000 py-Ayiin-0.4.6.dev7/pyAyiin/pyrogram/sections.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2138 2023-06-12 17:22:37.000000 py-Ayiin-0.4.6.dev7/pyAyiin/pyrogram/toolbot.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8684 2023-06-12 17:22:37.000000 py-Ayiin-0.4.6.dev7/pyAyiin/pyrogram/tools.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-12 17:22:51.128386 py-Ayiin-0.4.6.dev7/pyAyiin/resources/
+-rw-r--r--   0 runner    (1001) docker     (123)   281001 2023-06-12 17:22:37.000000 py-Ayiin-0.4.6.dev7/pyAyiin/resources/Logo Ayiin.jpg
+-rw-r--r--   0 runner    (1001) docker     (123)    31343 2023-06-12 17:22:37.000000 py-Ayiin-0.4.6.dev7/pyAyiin/resources/Youtube.jpeg
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-12 17:22:37.000000 py-Ayiin-0.4.6.dev7/pyAyiin/resources/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    39497 2023-06-12 17:22:37.000000 py-Ayiin-0.4.6.dev7/pyAyiin/resources/ayiin_music.jpg
+-rw-r--r--   0 runner    (1001) docker     (123)  1808670 2023-06-12 17:22:37.000000 py-Ayiin-0.4.6.dev7/pyAyiin/resources/ayiin_ubot.jpg
+-rw-r--r--   0 runner    (1001) docker     (123)    60539 2023-06-12 17:22:37.000000 py-Ayiin-0.4.6.dev7/pyAyiin/resources/ayiin_userbot.jpg
+-rw-r--r--   0 runner    (1001) docker     (123)      889 2023-06-12 17:22:37.000000 py-Ayiin-0.4.6.dev7/pyAyiin/resources/blank.png
+-rw-r--r--   0 runner    (1001) docker     (123)    56364 2023-06-12 17:22:37.000000 py-Ayiin-0.4.6.dev7/pyAyiin/resources/default.ttf
+-rw-r--r--   0 runner    (1001) docker     (123)   141612 2023-06-12 17:22:37.000000 py-Ayiin-0.4.6.dev7/pyAyiin/resources/font.ttf
+-rw-r--r--   0 runner    (1001) docker     (123)   128248 2023-06-12 17:22:37.000000 py-Ayiin-0.4.6.dev7/pyAyiin/resources/font2.ttf
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-12 17:22:51.128386 py-Ayiin-0.4.6.dev7/pyAyiin/telethon/
+-rw-r--r--   0 runner    (1001) docker     (123)       31 2023-06-12 17:22:37.000000 py-Ayiin-0.4.6.dev7/pyAyiin/telethon/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-12 17:22:51.128386 py-Ayiin-0.4.6.dev7/pyAyiin/telethon/ayiin/
+-rw-r--r--   0 runner    (1001) docker     (123)      152 2023-06-12 17:22:37.000000 py-Ayiin-0.4.6.dev7/pyAyiin/telethon/ayiin/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1803 2023-06-12 17:22:37.000000 py-Ayiin-0.4.6.dev7/pyAyiin/telethon/ayiin/_wrappers.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3848 2023-06-12 17:22:37.000000 py-Ayiin-0.4.6.dev7/pyAyiin/telethon/ayiin/events.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6803 2023-06-12 17:22:37.000000 py-Ayiin-0.4.6.dev7/pyAyiin/telethon/ayiin/misc.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17263 2023-06-12 17:22:37.000000 py-Ayiin-0.4.6.dev7/pyAyiin/xd.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-12 17:22:51.128386 py-Ayiin-0.4.6.dev7/py_Ayiin.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     2572 2023-06-12 17:22:51.000000 py-Ayiin-0.4.6.dev7/py_Ayiin.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1912 2023-06-12 17:22:51.000000 py-Ayiin-0.4.6.dev7/py_Ayiin.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-12 17:22:51.000000 py-Ayiin-0.4.6.dev7/py_Ayiin.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      149 2023-06-12 17:22:51.000000 py-Ayiin-0.4.6.dev7/py_Ayiin.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        8 2023-06-12 17:22:51.000000 py-Ayiin-0.4.6.dev7/py_Ayiin.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      149 2023-06-12 17:22:37.000000 py-Ayiin-0.4.6.dev7/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-12 17:22:51.128386 py-Ayiin-0.4.6.dev7/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1641 2023-06-12 17:22:37.000000 py-Ayiin-0.4.6.dev7/setup.py
```

### Comparing `py-Ayiin-0.4.6.dev6/LICENSE` & `py-Ayiin-0.4.6.dev7/LICENSE`

 * *Files identical despite different names*

### Comparing `py-Ayiin-0.4.6.dev6/NOTICE` & `py-Ayiin-0.4.6.dev7/NOTICE`

 * *Files identical despite different names*

### Comparing `py-Ayiin-0.4.6.dev6/PKG-INFO` & `py-Ayiin-0.4.6.dev7/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: py-Ayiin
-Version: 0.4.6.dev6
+Version: 0.4.6.dev7
 Summary: A Secure and Powerful Python-Telethon Based and Python-Pyrogram Based Library For Your Userbot Module.
 Home-page: https://github.com/AyiinXd/AyiinXd
 Author: AyiinXd
 Author-email: ayingaming98@gmail.com
 License: GNU General Public License v3.0 (GPL-3.0)
 Project-URL: Bug Tracker, https://github.com/AyiinXd/AyiinXd/issues
 Project-URL: Source Code, https://github.com/AyiinXd/AyiinXd
```

### Comparing `py-Ayiin-0.4.6.dev6/README.md` & `py-Ayiin-0.4.6.dev7/README.md`

 * *Files identical despite different names*

### Comparing `py-Ayiin-0.4.6.dev6/pyAyiin/Clients/__init__.py` & `py-Ayiin-0.4.6.dev7/pyAyiin/Clients/__init__.py`

 * *Files identical despite different names*

### Comparing `py-Ayiin-0.4.6.dev6/pyAyiin/Clients/client.py` & `py-Ayiin-0.4.6.dev7/pyAyiin/Clients/client.py`

 * *Files identical despite different names*

### Comparing `py-Ayiin-0.4.6.dev6/pyAyiin/Clients/pytgcalls.py` & `py-Ayiin-0.4.6.dev7/pyAyiin/Clients/pytgcalls.py`

 * *Files 2% similar despite different names*

```diff
@@ -93,14 +93,17 @@
     ):
         group_call = await self.get_group_call(client, message, err_msg="group call already ended")
         if not group_call:
             return
         await client.invoke(DiscardGroupCall(call=group_call))
 
 
+xx = GroupCalls()
+
+
 class VcMusic(Queues):
     def __init__(self, client: Client, message: Message):
         self.m = message
         self.chat_id = []
         self.clients = {}
         self.client = client
         self.active_calls = []
@@ -126,15 +129,15 @@
         if self.m.chat.id not in ACTIVE_CALLS:
             try:
                 self.client.group_call.on_network_status_changed(
                     self.on_network_changed)
                 self.client.group_call.on_playout_ended(self.playout_ended_handler)
                 await self.client.group_call.join(self.m.chat.id)
             except GroupCallNotFoundError as er:
-                await self.m.reply(_["err"].format(er))
+                await xx.StartVc(self.client, self.m)
                 return False, er
             except Exception as e:
                 await self.m.reply(_["err"].format(e))
                 return False, e
         return True, None
 
     async def on_network_changed(self, call, is_connected):
```

### Comparing `py-Ayiin-0.4.6.dev6/pyAyiin/Clients/startup.py` & `py-Ayiin-0.4.6.dev7/pyAyiin/Clients/startup.py`

 * *Files identical despite different names*

### Comparing `py-Ayiin-0.4.6.dev6/pyAyiin/__init__.py` & `py-Ayiin-0.4.6.dev7/pyAyiin/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -48,15 +48,15 @@
 
 
 logs = logging.getLogger(__name__)
 
 
 __copyright__ = "Copyright (C) 2022-present AyiinXd <https://github.com/AyiinXd>"
 __license__ = "GNU General Public License v3.0 (GPL-3.0)"
-__version__ = "0.4.6.dev06"
+__version__ = "0.4.6.dev07"
 ayiin_ver = "0.1.1"
 prem_version = "0.1"
 
 
 DEVS = [
     607067484, # Ayiin
     997461844, #Ayang_Ayiin
```

### Comparing `py-Ayiin-0.4.6.dev6/pyAyiin/__main__.py` & `py-Ayiin-0.4.6.dev7/pyAyiin/__main__.py`

 * *Files identical despite different names*

### Comparing `py-Ayiin-0.4.6.dev6/pyAyiin/assistant.py` & `py-Ayiin-0.4.6.dev7/pyAyiin/assistant.py`

 * *Files identical despite different names*

### Comparing `py-Ayiin-0.4.6.dev6/pyAyiin/config.py` & `py-Ayiin-0.4.6.dev7/pyAyiin/config.py`

 * *Files identical despite different names*

### Comparing `py-Ayiin-0.4.6.dev6/pyAyiin/dB/__init__.py` & `py-Ayiin-0.4.6.dev7/pyAyiin/dB/__init__.py`

 * *Files identical despite different names*

### Comparing `py-Ayiin-0.4.6.dev6/pyAyiin/dB/absen.py` & `py-Ayiin-0.4.6.dev7/pyAyiin/dB/absen.py`

 * *Files identical despite different names*

### Comparing `py-Ayiin-0.4.6.dev6/pyAyiin/dB/admins.py` & `py-Ayiin-0.4.6.dev7/pyAyiin/dB/admins.py`

 * *Files identical despite different names*

### Comparing `py-Ayiin-0.4.6.dev6/pyAyiin/dB/auth.py` & `py-Ayiin-0.4.6.dev7/pyAyiin/dB/auth.py`

 * *Files identical despite different names*

### Comparing `py-Ayiin-0.4.6.dev6/pyAyiin/dB/blacklistfilter.py` & `py-Ayiin-0.4.6.dev7/pyAyiin/dB/blacklistfilter.py`

 * *Files identical despite different names*

### Comparing `py-Ayiin-0.4.6.dev6/pyAyiin/dB/blacklistgcast.py` & `py-Ayiin-0.4.6.dev7/pyAyiin/dB/blacklistgcast.py`

 * *Files identical despite different names*

### Comparing `py-Ayiin-0.4.6.dev6/pyAyiin/dB/blacklistuser.py` & `py-Ayiin-0.4.6.dev7/pyAyiin/dB/blacklistuser.py`

 * *Files identical despite different names*

### Comparing `py-Ayiin-0.4.6.dev6/pyAyiin/dB/gban.py` & `py-Ayiin-0.4.6.dev7/pyAyiin/dB/gban.py`

 * *Files identical despite different names*

### Comparing `py-Ayiin-0.4.6.dev6/pyAyiin/dB/langs.py` & `py-Ayiin-0.4.6.dev7/pyAyiin/dB/langs.py`

 * *Files identical despite different names*

### Comparing `py-Ayiin-0.4.6.dev6/pyAyiin/dB/logdb.py` & `py-Ayiin-0.4.6.dev7/pyAyiin/dB/logdb.py`

 * *Files identical despite different names*

### Comparing `py-Ayiin-0.4.6.dev6/pyAyiin/dB/pmpermit.py` & `py-Ayiin-0.4.6.dev7/pyAyiin/dB/pmpermit.py`

 * *Files identical despite different names*

### Comparing `py-Ayiin-0.4.6.dev6/pyAyiin/dB/premium.py` & `py-Ayiin-0.4.6.dev7/pyAyiin/dB/premium.py`

 * *Files identical despite different names*

### Comparing `py-Ayiin-0.4.6.dev6/pyAyiin/dB/start.py` & `py-Ayiin-0.4.6.dev7/pyAyiin/dB/start.py`

 * *Files identical despite different names*

### Comparing `py-Ayiin-0.4.6.dev6/pyAyiin/dB/sudo.py` & `py-Ayiin-0.4.6.dev7/pyAyiin/dB/sudo.py`

 * *Files identical despite different names*

### Comparing `py-Ayiin-0.4.6.dev6/pyAyiin/dB/variable.py` & `py-Ayiin-0.4.6.dev7/pyAyiin/dB/variable.py`

 * *Files identical despite different names*

### Comparing `py-Ayiin-0.4.6.dev6/pyAyiin/dB/videocalls.py` & `py-Ayiin-0.4.6.dev7/pyAyiin/dB/videocalls.py`

 * *Files identical despite different names*

### Comparing `py-Ayiin-0.4.6.dev6/pyAyiin/dB/welcome.py` & `py-Ayiin-0.4.6.dev7/pyAyiin/dB/welcome.py`

 * *Files identical despite different names*

### Comparing `py-Ayiin-0.4.6.dev6/pyAyiin/decorator.py` & `py-Ayiin-0.4.6.dev7/pyAyiin/decorator.py`

 * *Files identical despite different names*

### Comparing `py-Ayiin-0.4.6.dev6/pyAyiin/exceptions.py` & `py-Ayiin-0.4.6.dev7/pyAyiin/exceptions.py`

 * *Files identical despite different names*

### Comparing `py-Ayiin-0.4.6.dev6/pyAyiin/methods/__init__.py` & `py-Ayiin-0.4.6.dev7/pyAyiin/methods/__init__.py`

 * *Files identical despite different names*

### Comparing `py-Ayiin-0.4.6.dev6/pyAyiin/methods/_database.py` & `py-Ayiin-0.4.6.dev7/pyAyiin/methods/_database.py`

 * *Files identical despite different names*

### Comparing `py-Ayiin-0.4.6.dev6/pyAyiin/methods/_misc.py` & `py-Ayiin-0.4.6.dev7/pyAyiin/methods/_misc.py`

 * *Files identical despite different names*

### Comparing `py-Ayiin-0.4.6.dev6/pyAyiin/methods/changer.py` & `py-Ayiin-0.4.6.dev7/pyAyiin/methods/changer.py`

 * *Files identical despite different names*

### Comparing `py-Ayiin-0.4.6.dev6/pyAyiin/methods/converter.py` & `py-Ayiin-0.4.6.dev7/pyAyiin/methods/converter.py`

 * *Files identical despite different names*

### Comparing `py-Ayiin-0.4.6.dev6/pyAyiin/methods/func.py` & `py-Ayiin-0.4.6.dev7/pyAyiin/methods/func.py`

 * *Files identical despite different names*

### Comparing `py-Ayiin-0.4.6.dev6/pyAyiin/methods/funcb.py` & `py-Ayiin-0.4.6.dev7/pyAyiin/methods/funcb.py`

 * *Files 11% similar despite different names*

```diff
@@ -77,184 +77,228 @@
         succ = await client.send_message(tgbot.me.username, "/start")
         return succ
 
 
     async def logger_bot(
         self,
         client,
-        pepek,
+        pepek: None,
+        group: bool = None,
     ):
         from pyAyiin.Clients.client import tgbot
 
-        if pepek.text:
+        if group:
+            from_user = f"{pepek.from_user.first_name}" if pepek.from_user.first_name else None
             try:
-                return await tgbot.send_message(
+                await tgbot.send_message(
                     client.me.id,
-                    f"Logs: {client.me.first_name}\nPesan Dari: {pepek.from_user.first_name}\nPesan:\n{pepek.text}",
+                    f"""📨 #TAGS #MESSAGE
+• <b>Logs:</b> <code>{client.me.first_name}</code>
+• <b>Group:</b> <code>{pepek.chat.title}</code>
+• <b>Dari :</b> <code>{from_user}</code>
+• <b>Pesan:</b> ↓↓↓↓\n\n<code>{pepek.text}</code>
+""",
                     reply_markup=InlineKeyboardMarkup(
                         [
+                            [InlineKeyboardButton("👀 Pesan 👀", url=f"{pepek.link}")],
                             [InlineKeyboardButton("💌 Pengirim 💌", url=f"tg://openmessage?user_id={pepek.from_user.id}")],
                         ]
                     ),
                     disable_web_page_preview=True,
-                )
+                    )
             except PeerIdInvalid:
-                x = await self.start_bot(client)
-                if x:
-                    return await tgbot.send_message(
+                xd = await self.start_bot(client)
+                if xd:
+                    await tgbot.send_message(
                         client.me.id,
-                        f"Logs: {client.me.first_name}\nPesan Dari: {pepek.from_user.first_name}\nPesan:\n{pepek.text}",
+                        f"""📨 #TAGS #MESSAGE
+• <b>Logs:</b> <code>{client.me.first_name}</code>
+• <b>Group:</b> <code>{pepek.chat.title}</code>
+• <b>Dari :</b> <code>{from_user}</code>
+• <b>Pesan:</b> ↓↓↓↓\n\n<code>{pepek.text}</code>
+""",
                         reply_markup=InlineKeyboardMarkup(
                             [
+                                [InlineKeyboardButton("👀 Pesan 👀", url=f"{pepek.link}")],
                                 [InlineKeyboardButton("💌 Pengirim 💌", url=f"tg://openmessage?user_id={pepek.from_user.id}")],
                             ]
                         ),
                         disable_web_page_preview=True,
-                    )
-                else:
-                    pass
+                        )
             except FloodWait as e:
                 await asyncio.sleep(e.value)
             except BaseException:
                 pass
-        if pepek.photo:
-            file = await client.download_media(pepek.photo)
-            try:
-                await tgbot.send_photo(
-                    client.me.id,
-                    photo=file,
-                    caption=f"Logs: {client.me.first_name}\nPesan Dari: {pepek.from_user.first_name}",
-                    reply_markup=InlineKeyboardMarkup(
-                        [
-                            [InlineKeyboardButton("💌 Pengirim 💌", url=f"tg://openmessage?user_id={pepek.from_user.id}")],
-                        ]
-                    ),
-                )
-                os.remove(file)
-                return
-            except PeerIdInvalid:
-                x = await self.start_bot(client)
-                if x:
+        if pepek:
+            if pepek.text:
+                try:
+                    return await tgbot.send_message(
+                        client.me.id,
+                        f"Logs: {client.me.first_name}\nPesan Dari: {pepek.from_user.first_name}\nPesan:\n{pepek.text}",
+                        reply_markup=InlineKeyboardMarkup(
+                            [
+                                [InlineKeyboardButton("💌 Pengirim 💌", url=f"tg://openmessage?user_id={pepek.from_user.id}")],
+                            ]
+                        ),
+                        disable_web_page_preview=True,
+                    )
+                except PeerIdInvalid:
+                    x = await self.start_bot(client)
+                    if x:
+                        return await tgbot.send_message(
+                            client.me.id,
+                            f"Logs: {client.me.first_name}\nPesan Dari: {pepek.from_user.first_name}\nPesan:\n{pepek.text}",
+                            reply_markup=InlineKeyboardMarkup(
+                                [
+                                    [InlineKeyboardButton("💌 Pengirim 💌", url=f"tg://openmessage?user_id={pepek.from_user.id}")],
+                                ]
+                            ),
+                            disable_web_page_preview=True,
+                        )
+                    else:
+                        pass
+                except FloodWait as e:
+                    await asyncio.sleep(e.value)
+                except BaseException:
+                    pass
+            if pepek.photo:
+                file = await client.download_media(pepek.photo)
+                try:
                     await tgbot.send_photo(
                         client.me.id,
                         photo=file,
                         caption=f"Logs: {client.me.first_name}\nPesan Dari: {pepek.from_user.first_name}",
                         reply_markup=InlineKeyboardMarkup(
                             [
                                 [InlineKeyboardButton("💌 Pengirim 💌", url=f"tg://openmessage?user_id={pepek.from_user.id}")],
                             ]
                         ),
                     )
                     os.remove(file)
                     return
-                else:
+                except PeerIdInvalid:
+                    x = await self.start_bot(client)
+                    if x:
+                        await tgbot.send_photo(
+                            client.me.id,
+                            photo=file,
+                            caption=f"Logs: {client.me.first_name}\nPesan Dari: {pepek.from_user.first_name}",
+                            reply_markup=InlineKeyboardMarkup(
+                                [
+                                    [InlineKeyboardButton("💌 Pengirim 💌", url=f"tg://openmessage?user_id={pepek.from_user.id}")],
+                                ]
+                            ),
+                        )
+                        os.remove(file)
+                        return
+                    else:
+                        pass
+                except FloodWait as e:
+                    await asyncio.sleep(e.value)
+                except BaseException:
                     pass
-            except FloodWait as e:
-                await asyncio.sleep(e.value)
-            except BaseException:
-                pass
-        if pepek.video:
-            file = await client.download_media(pepek.video)
-            try:
-                await tgbot.send_video(
-                    client.me.id,
-                    video=file,
-                    caption=f"Logs: {client.me.first_name}\nPesan Dari: {pepek.from_user.first_name}",
-                    reply_markup=InlineKeyboardMarkup(
-                        [
-                            [InlineKeyboardButton("💌 Pengirim 💌", url=f"tg://openmessage?user_id={pepek.from_user.id}")],
-                        ]
-                    ),
-                )
-                os.remove(file)
-                return
-            except PeerIdInvalid:
-                x = await self.start_bot(client)
-                if x:
+            if pepek.video:
+                file = await client.download_media(pepek.video)
+                try:
                     await tgbot.send_video(
                         client.me.id,
                         video=file,
                         caption=f"Logs: {client.me.first_name}\nPesan Dari: {pepek.from_user.first_name}",
                         reply_markup=InlineKeyboardMarkup(
                             [
                                 [InlineKeyboardButton("💌 Pengirim 💌", url=f"tg://openmessage?user_id={pepek.from_user.id}")],
                             ]
                         ),
                     )
                     os.remove(file)
                     return
-                else:
+                except PeerIdInvalid:
+                    x = await self.start_bot(client)
+                    if x:
+                        await tgbot.send_video(
+                            client.me.id,
+                            video=file,
+                            caption=f"Logs: {client.me.first_name}\nPesan Dari: {pepek.from_user.first_name}",
+                            reply_markup=InlineKeyboardMarkup(
+                                [
+                                    [InlineKeyboardButton("💌 Pengirim 💌", url=f"tg://openmessage?user_id={pepek.from_user.id}")],
+                                ]
+                            ),
+                        )
+                        os.remove(file)
+                        return
+                    else:
+                        pass
+                except FloodWait as e:
+                    await asyncio.sleep(e.value)
+                except BaseException:
                     pass
-            except FloodWait as e:
-                await asyncio.sleep(e.value)
-            except BaseException:
-                pass
-        if pepek.voice:
-            file = await client.download_media(pepek.voice)
-            try:
-                await tgbot.send_voice(
-                    client.me.id,
-                    voice=file,
-                    caption=f"Logs: {client.me.first_name}\nPesan Dari: {pepek.from_user.first_name}",
-                    reply_markup=InlineKeyboardMarkup(
-                        [
-                            [InlineKeyboardButton("💌 Pengirim 💌", url=f"tg://openmessage?user_id={pepek.from_user.id}")],
-                        ]
-                    ),
-                )
-                os.remove(file)
-                return
-            except PeerIdInvalid:
-                x = await self.start_bot(client)
-                if x:
+            if pepek.voice:
+                file = await client.download_media(pepek.voice)
+                try:
                     await tgbot.send_voice(
                         client.me.id,
                         voice=file,
                         caption=f"Logs: {client.me.first_name}\nPesan Dari: {pepek.from_user.first_name}",
                         reply_markup=InlineKeyboardMarkup(
                             [
                                 [InlineKeyboardButton("💌 Pengirim 💌", url=f"tg://openmessage?user_id={pepek.from_user.id}")],
                             ]
                         ),
                     )
                     os.remove(file)
                     return
-                else:
+                except PeerIdInvalid:
+                    x = await self.start_bot(client)
+                    if x:
+                        await tgbot.send_voice(
+                            client.me.id,
+                            voice=file,
+                            caption=f"Logs: {client.me.first_name}\nPesan Dari: {pepek.from_user.first_name}",
+                            reply_markup=InlineKeyboardMarkup(
+                                [
+                                    [InlineKeyboardButton("💌 Pengirim 💌", url=f"tg://openmessage?user_id={pepek.from_user.id}")],
+                                ]
+                            ),
+                        )
+                        os.remove(file)
+                        return
+                    else:
+                        pass
+                except FloodWait as e:
+                    await asyncio.sleep(e.value)
+                except BaseException:
                     pass
-            except FloodWait as e:
-                await asyncio.sleep(e.value)
-            except BaseException:
-                pass
-        if pepek.sticker:
-            file = await client.download_media(pepek.sticker)
-            try:
-                await tgbot.send_sticker(
-                    client.me.id,
-                    sticker=file,
-                    reply_markup=InlineKeyboardMarkup(
-                        [
-                            [InlineKeyboardButton("💌 Pengirim 💌", url=f"tg://openmessage?user_id={pepek.from_user.id}")],
-                        ]
-                    ),
-                )
-                os.remove(file)
-                return
-            except PeerIdInvalid:
-                x = await self.start_bot(client)
-                if x:
+            if pepek.sticker:
+                file = await client.download_media(pepek.sticker)
+                try:
                     await tgbot.send_sticker(
                         client.me.id,
                         sticker=file,
                         reply_markup=InlineKeyboardMarkup(
                             [
                                 [InlineKeyboardButton("💌 Pengirim 💌", url=f"tg://openmessage?user_id={pepek.from_user.id}")],
                             ]
                         ),
                     )
                     os.remove(file)
                     return
-                else:
+                except PeerIdInvalid:
+                    x = await self.start_bot(client)
+                    if x:
+                        await tgbot.send_sticker(
+                            client.me.id,
+                            sticker=file,
+                            reply_markup=InlineKeyboardMarkup(
+                                [
+                                    [InlineKeyboardButton("💌 Pengirim 💌", url=f"tg://openmessage?user_id={pepek.from_user.id}")],
+                                ]
+                            ),
+                        )
+                        os.remove(file)
+                        return
+                    else:
+                        pass
+                except FloodWait as e:
+                    await asyncio.sleep(e.value)
+                except BaseException:
                     pass
-            except FloodWait as e:
-                await asyncio.sleep(e.value)
-            except BaseException:
-                pass
```

### Comparing `py-Ayiin-0.4.6.dev6/pyAyiin/methods/helpers.py` & `py-Ayiin-0.4.6.dev7/pyAyiin/methods/helpers.py`

 * *Files identical despite different names*

### Comparing `py-Ayiin-0.4.6.dev6/pyAyiin/methods/hosting.py` & `py-Ayiin-0.4.6.dev7/pyAyiin/methods/hosting.py`

 * *Files identical despite different names*

### Comparing `py-Ayiin-0.4.6.dev6/pyAyiin/methods/inlinebot.py` & `py-Ayiin-0.4.6.dev7/pyAyiin/methods/inlinebot.py`

 * *Files 2% similar despite different names*

```diff
@@ -185,19 +185,18 @@
                         reply_markup=InlineKeyboardMarkup(buttons),
                         input_message_content=InputTextMessageContent(output),
                     )
                 )
             ]
         return results
     
-    async def inline_languages(self, ids, _):
-        from pyAyiin.dB.langs import get_lang, get_languages
+    async def inline_languages(self, _):
+        from pyAyiin.dB.langs import get_languages
         
-        lang = await get_lang(ids)
-        text = _["lang"].format(lang)
+        text = _["lang"]
         languages = get_languages()
         tutud = [
             InlineKeyboardButton(
                 f"{languages[yins]['nama']}",
                 callback_data=f"set_{yins}",
             )
             for yins in languages
```

### Comparing `py-Ayiin-0.4.6.dev6/pyAyiin/methods/queue.py` & `py-Ayiin-0.4.6.dev7/pyAyiin/methods/queue.py`

 * *Files identical despite different names*

### Comparing `py-Ayiin-0.4.6.dev6/pyAyiin/methods/thumbnail.py` & `py-Ayiin-0.4.6.dev7/pyAyiin/methods/thumbnail.py`

 * *Files identical despite different names*

### Comparing `py-Ayiin-0.4.6.dev6/pyAyiin/pyrogram/__init__.py` & `py-Ayiin-0.4.6.dev7/pyAyiin/pyrogram/__init__.py`

 * *Files identical despite different names*

### Comparing `py-Ayiin-0.4.6.dev6/pyAyiin/pyrogram/_wrappers.py` & `py-Ayiin-0.4.6.dev7/pyAyiin/pyrogram/_wrappers.py`

 * *Files identical despite different names*

### Comparing `py-Ayiin-0.4.6.dev6/pyAyiin/pyrogram/func.py` & `py-Ayiin-0.4.6.dev7/pyAyiin/pyrogram/func.py`

 * *Files identical despite different names*

### Comparing `py-Ayiin-0.4.6.dev6/pyAyiin/pyrogram/misc.py` & `py-Ayiin-0.4.6.dev7/pyAyiin/pyrogram/misc.py`

 * *Files identical despite different names*

### Comparing `py-Ayiin-0.4.6.dev6/pyAyiin/pyrogram/pastebin.py` & `py-Ayiin-0.4.6.dev7/pyAyiin/pyrogram/pastebin.py`

 * *Files identical despite different names*

### Comparing `py-Ayiin-0.4.6.dev6/pyAyiin/pyrogram/sections.py` & `py-Ayiin-0.4.6.dev7/pyAyiin/pyrogram/sections.py`

 * *Files identical despite different names*

### Comparing `py-Ayiin-0.4.6.dev6/pyAyiin/pyrogram/toolbot.py` & `py-Ayiin-0.4.6.dev7/pyAyiin/pyrogram/toolbot.py`

 * *Files identical despite different names*

### Comparing `py-Ayiin-0.4.6.dev6/pyAyiin/pyrogram/tools.py` & `py-Ayiin-0.4.6.dev7/pyAyiin/pyrogram/tools.py`

 * *Files identical despite different names*

### Comparing `py-Ayiin-0.4.6.dev6/pyAyiin/resources/Logo Ayiin.jpg` & `py-Ayiin-0.4.6.dev7/pyAyiin/resources/Logo Ayiin.jpg`

 * *Files identical despite different names*

### Comparing `py-Ayiin-0.4.6.dev6/pyAyiin/resources/Youtube.jpeg` & `py-Ayiin-0.4.6.dev7/pyAyiin/resources/Youtube.jpeg`

 * *Files identical despite different names*

### Comparing `py-Ayiin-0.4.6.dev6/pyAyiin/resources/ayiin_music.jpg` & `py-Ayiin-0.4.6.dev7/pyAyiin/resources/ayiin_music.jpg`

 * *Files identical despite different names*

### Comparing `py-Ayiin-0.4.6.dev6/pyAyiin/resources/ayiin_ubot.jpg` & `py-Ayiin-0.4.6.dev7/pyAyiin/resources/ayiin_ubot.jpg`

 * *Files identical despite different names*

### Comparing `py-Ayiin-0.4.6.dev6/pyAyiin/resources/ayiin_userbot.jpg` & `py-Ayiin-0.4.6.dev7/pyAyiin/resources/ayiin_userbot.jpg`

 * *Files identical despite different names*

### Comparing `py-Ayiin-0.4.6.dev6/pyAyiin/resources/blank.png` & `py-Ayiin-0.4.6.dev7/pyAyiin/resources/blank.png`

 * *Files identical despite different names*

### Comparing `py-Ayiin-0.4.6.dev6/pyAyiin/resources/default.ttf` & `py-Ayiin-0.4.6.dev7/pyAyiin/resources/default.ttf`

 * *Files identical despite different names*

### Comparing `py-Ayiin-0.4.6.dev6/pyAyiin/resources/font.ttf` & `py-Ayiin-0.4.6.dev7/pyAyiin/resources/font.ttf`

 * *Files identical despite different names*

### Comparing `py-Ayiin-0.4.6.dev6/pyAyiin/resources/font2.ttf` & `py-Ayiin-0.4.6.dev7/pyAyiin/resources/font2.ttf`

 * *Files identical despite different names*

### Comparing `py-Ayiin-0.4.6.dev6/pyAyiin/telethon/ayiin/_wrappers.py` & `py-Ayiin-0.4.6.dev7/pyAyiin/telethon/ayiin/_wrappers.py`

 * *Files identical despite different names*

### Comparing `py-Ayiin-0.4.6.dev6/pyAyiin/telethon/ayiin/events.py` & `py-Ayiin-0.4.6.dev7/pyAyiin/telethon/ayiin/events.py`

 * *Files identical despite different names*

### Comparing `py-Ayiin-0.4.6.dev6/pyAyiin/telethon/ayiin/misc.py` & `py-Ayiin-0.4.6.dev7/pyAyiin/telethon/ayiin/misc.py`

 * *Files identical despite different names*

### Comparing `py-Ayiin-0.4.6.dev6/pyAyiin/xd.py` & `py-Ayiin-0.4.6.dev7/pyAyiin/xd.py`

 * *Files identical despite different names*

### Comparing `py-Ayiin-0.4.6.dev6/py_Ayiin.egg-info/PKG-INFO` & `py-Ayiin-0.4.6.dev7/py_Ayiin.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: py-Ayiin
-Version: 0.4.6.dev6
+Version: 0.4.6.dev7
 Summary: A Secure and Powerful Python-Telethon Based and Python-Pyrogram Based Library For Your Userbot Module.
 Home-page: https://github.com/AyiinXd/AyiinXd
 Author: AyiinXd
 Author-email: ayingaming98@gmail.com
 License: GNU General Public License v3.0 (GPL-3.0)
 Project-URL: Bug Tracker, https://github.com/AyiinXd/AyiinXd/issues
 Project-URL: Source Code, https://github.com/AyiinXd/AyiinXd
```

### Comparing `py-Ayiin-0.4.6.dev6/py_Ayiin.egg-info/SOURCES.txt` & `py-Ayiin-0.4.6.dev7/py_Ayiin.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `py-Ayiin-0.4.6.dev6/setup.py` & `py-Ayiin-0.4.6.dev7/setup.py`

 * *Files identical despite different names*

