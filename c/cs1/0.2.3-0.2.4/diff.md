# Comparing `tmp/cs1-0.2.3.tar.gz` & `tmp/cs1-0.2.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "cs1-0.2.3.tar", last modified: Sat Jun  3 05:05:21 2023, max compression
+gzip compressed data, was "cs1-0.2.4.tar", last modified: Mon Jun 12 03:07:02 2023, max compression
```

## Comparing `cs1-0.2.3.tar` & `cs1-0.2.4.tar`

### file list

```diff
@@ -1,80 +1,80 @@
-drwxrwxrwx   0        0        0        0 2023-06-03 05:05:21.716906 cs1-0.2.3/
--rw-rw-rw-   0        0        0      214 2022-03-26 07:50:46.000000 cs1-0.2.3/LICENCE
--rw-rw-rw-   0        0        0     4998 2023-06-03 05:05:21.716906 cs1-0.2.3/PKG-INFO
--rw-rw-rw-   0        0        0     4359 2023-06-03 02:56:39.000000 cs1-0.2.3/README.md
--rw-rw-rw-   0        0        0      108 2022-01-07 07:21:30.000000 cs1-0.2.3/pyproject.toml
--rw-rw-rw-   0        0        0     1015 2023-06-03 05:05:21.724934 cs1-0.2.3/setup.cfg
-drwxrwxrwx   0        0        0        0 2023-06-03 05:05:21.591519 cs1-0.2.3/src/
-drwxrwxrwx   0        0        0        0 2023-06-03 05:05:21.605640 cs1-0.2.3/src/cs1/
--rw-rw-rw-   0        0        0    38783 2023-02-24 08:13:59.000000 cs1-0.2.3/src/cs1/__init__.py
-drwxrwxrwx   0        0        0        0 2023-06-03 05:05:21.628652 cs1-0.2.3/src/cs1/basis/
--rw-rw-rw-   0        0        0        0 2022-10-07 10:23:54.000000 cs1-0.2.3/src/cs1/basis/__init__.py
-drwxrwxrwx   0        0        0        0 2023-06-03 05:05:21.631649 cs1-0.2.3/src/cs1/basis/adaptive/
--rw-rw-rw-   0        0        0     5124 2023-02-21 12:23:56.000000 cs1-0.2.3/src/cs1/basis/adaptive/__init__.py
--rw-rw-rw-   0        0        0    18165 2023-04-04 07:11:28.000000 cs1-0.2.3/src/cs1/basis/adaptive/vae.py
--rw-rw-rw-   0        0        0     7148 2023-01-15 10:21:44.000000 cs1-0.2.3/src/cs1/basis/common.py
--rw-rw-rw-   0        0        0    24696 2023-06-03 03:57:26.000000 cs1-0.2.3/src/cs1/cs.py
-drwxrwxrwx   0        0        0        0 2023-06-03 05:05:21.635648 cs1-0.2.3/src/cs1/domain/
--rw-rw-rw-   0        0        0      693 2022-10-08 07:15:14.000000 cs1-0.2.3/src/cs1/domain/__init__.py
--rw-rw-rw-   0        0        0     9862 2023-01-08 15:31:23.000000 cs1-0.2.3/src/cs1/domain/audio.py
--rw-rw-rw-   0        0        0    11912 2023-01-15 13:30:15.000000 cs1-0.2.3/src/cs1/domain/image.py
-drwxrwxrwx   0        0        0        0 2023-06-03 05:05:21.638653 cs1-0.2.3/src/cs1/gui/
--rw-rw-rw-   0        0        0        0 2022-10-07 10:23:54.000000 cs1-0.2.3/src/cs1/gui/__init__.py
--rw-rw-rw-   0        0        0     4433 2023-03-16 02:40:31.000000 cs1-0.2.3/src/cs1/gui/run.py
-drwxrwxrwx   0        0        0        0 2023-06-03 05:05:21.658898 cs1-0.2.3/src/cs1/gui/static/
--rw-rw-rw-   0        0        0        0 2022-01-07 02:28:31.000000 cs1-0.2.3/src/cs1/gui/static/__init__.py
--rw-rw-rw-   0        0        0     2518 2022-07-20 15:27:40.000000 cs1-0.2.3/src/cs1/gui/static/bootstrap-dialog.css
--rw-rw-rw-   0        0        0   192352 2020-09-09 05:39:36.000000 cs1-0.2.3/src/cs1/gui/static/bootstrap.css
--rw-rw-rw-   0        0        0   131637 2020-02-15 01:34:39.000000 cs1-0.2.3/src/cs1/gui/static/bootstrap.js
--rw-rw-rw-   0        0        0    37444 2022-11-12 14:05:28.000000 cs1-0.2.3/src/cs1/gui/static/font-awesome.css
-drwxrwxrwx   0        0        0        0 2023-06-03 05:05:21.681901 cs1-0.2.3/src/cs1/gui/static/fonts/
--rw-rw-rw-   0        0        0   134808 2022-07-20 15:27:41.000000 cs1-0.2.3/src/cs1/gui/static/fonts/FontAwesome.otf
--rw-rw-rw-   0        0        0        0 2022-01-07 02:28:31.000000 cs1-0.2.3/src/cs1/gui/static/fonts/__init__.py
--rw-rw-rw-   0        0        0   165742 2022-07-20 15:27:41.000000 cs1-0.2.3/src/cs1/gui/static/fonts/fontawesome-webfont.eot
--rw-rw-rw-   0        0        0   447050 2022-07-20 15:27:41.000000 cs1-0.2.3/src/cs1/gui/static/fonts/fontawesome-webfont.svg
--rw-rw-rw-   0        0        0   165548 2022-07-20 15:27:41.000000 cs1-0.2.3/src/cs1/gui/static/fonts/fontawesome-webfont.ttf
--rw-rw-rw-   0        0        0    98024 2022-07-20 15:27:41.000000 cs1-0.2.3/src/cs1/gui/static/fonts/fontawesome-webfont.woff
--rw-rw-rw-   0        0        0    77160 2022-07-20 15:27:41.000000 cs1-0.2.3/src/cs1/gui/static/fonts/fontawesome-webfont.woff2
--rw-rw-rw-   0        0        0    20127 2022-07-20 15:27:41.000000 cs1-0.2.3/src/cs1/gui/static/fonts/glyphicons-halflings-regular.eot
--rw-rw-rw-   0        0        0   108738 2022-07-20 15:27:41.000000 cs1-0.2.3/src/cs1/gui/static/fonts/glyphicons-halflings-regular.svg
--rw-rw-rw-   0        0        0    45404 2022-07-20 15:27:41.000000 cs1-0.2.3/src/cs1/gui/static/fonts/glyphicons-halflings-regular.ttf
--rw-rw-rw-   0        0        0    23424 2022-07-20 15:27:41.000000 cs1-0.2.3/src/cs1/gui/static/fonts/glyphicons-halflings-regular.woff
--rw-rw-rw-   0        0        0    18028 2022-07-20 15:27:41.000000 cs1-0.2.3/src/cs1/gui/static/fonts/glyphicons-halflings-regular.woff2
-drwxrwxrwx   0        0        0        0 2023-06-03 05:05:21.706900 cs1-0.2.3/src/cs1/gui/static/images/
--rw-rw-rw-   0        0        0    51449 2022-07-20 15:47:00.000000 cs1-0.2.3/src/cs1/gui/static/images/BCoT.png
--rw-rw-rw-   0        0        0   111921 2022-07-20 15:47:00.000000 cs1-0.2.3/src/cs1/gui/static/images/DCT.png
--rw-rw-rw-   0        0        0    74145 2022-07-20 15:47:00.000000 cs1-0.2.3/src/cs1/gui/static/images/DFT.png
--rw-rw-rw-   0        0        0     8052 2022-07-20 15:47:00.000000 cs1-0.2.3/src/cs1/gui/static/images/DFT_A.png
--rw-rw-rw-   0        0        0   108584 2022-07-20 15:47:00.000000 cs1-0.2.3/src/cs1/gui/static/images/DFT_P.png
--rw-rw-rw-   0        0        0    13354 2022-07-20 15:47:00.000000 cs1-0.2.3/src/cs1/gui/static/images/HWT.png
--rw-rw-rw-   0        0        0     1511 2022-07-20 15:47:00.000000 cs1-0.2.3/src/cs1/gui/static/images/IDM.png
--rw-rw-rw-   0        0        0    86935 2022-07-20 15:47:00.000000 cs1-0.2.3/src/cs1/gui/static/images/SECS.png
--rw-rw-rw-   0        0        0    71199 2022-07-20 15:47:00.000000 cs1-0.2.3/src/cs1/gui/static/images/Sensing - clean.png
--rw-rw-rw-   0        0        0        0 2022-01-07 02:28:31.000000 cs1-0.2.3/src/cs1/gui/static/images/__init__.py
--rw-rw-rw-   0        0        0    80565 2022-07-20 15:47:00.000000 cs1-0.2.3/src/cs1/gui/static/images/reconstruction - clean.png
--rw-rw-rw-   0        0        0   264308 2022-07-20 15:47:00.000000 cs1-0.2.3/src/cs1/gui/static/images/reconstruction.png
--rw-rw-rw-   0        0        0   152714 2022-07-20 15:47:00.000000 cs1-0.2.3/src/cs1/gui/static/images/sensing matrix - clean.png
--rw-rw-rw-   0        0        0   804558 2022-07-20 15:47:00.000000 cs1-0.2.3/src/cs1/gui/static/images/sensing matrix.jpeg
--rw-rw-rw-   0        0        0   160937 2022-07-20 15:47:00.000000 cs1-0.2.3/src/cs1/gui/static/images/sensing.png
--rw-rw-rw-   0        0        0    86927 2020-02-15 01:36:15.000000 cs1-0.2.3/src/cs1/gui/static/jquery-3.3.1.min.js
--rw-rw-rw-   0        0        0   520714 2022-07-20 15:28:09.000000 cs1-0.2.3/src/cs1/gui/static/jquery-ui-1.12.1.js
--rw-rw-rw-   0        0        0    64017 2022-07-20 15:27:42.000000 cs1-0.2.3/src/cs1/gui/static/jquery-ui.css
--rw-rw-rw-   0        0        0    24228 2020-02-15 04:11:19.000000 cs1-0.2.3/src/cs1/gui/static/jquery.blockUI.js
--rw-rw-rw-   0        0        0    17108 2020-02-15 04:11:19.000000 cs1-0.2.3/src/cs1/gui/static/jquery.form.min.js
--rw-rw-rw-   0        0        0     8602 2022-07-20 15:28:18.000000 cs1-0.2.3/src/cs1/gui/static/seedrandom.js
--rw-rw-rw-   0        0        0     4727 2022-11-12 02:00:29.000000 cs1-0.2.3/src/cs1/gui/static/utility.chart.js
-drwxrwxrwx   0        0        0        0 2023-06-03 05:05:21.712924 cs1-0.2.3/src/cs1/gui/templates/
--rw-rw-rw-   0        0        0        0 2022-11-03 12:58:21.000000 cs1-0.2.3/src/cs1/gui/templates/__init__.py
--rw-rw-rw-   0        0        0    95318 2022-11-18 14:09:58.000000 cs1-0.2.3/src/cs1/gui/templates/home.html
--rw-rw-rw-   0        0        0    23043 2022-11-18 14:32:23.000000 cs1-0.2.3/src/cs1/gui/templates/receiver.html
--rw-rw-rw-   0        0        0     8549 2022-11-19 14:14:31.000000 cs1-0.2.3/src/cs1/gui/templates/tutorial.html
--rw-rw-rw-   0        0        0     7753 2023-01-15 08:44:54.000000 cs1-0.2.3/src/cs1/metrics.py
-drwxrwxrwx   0        0        0        0 2023-06-03 05:05:21.715901 cs1-0.2.3/src/cs1/security/
--rw-rw-rw-   0        0        0        0 2022-10-07 10:23:54.000000 cs1-0.2.3/src/cs1/security/__init__.py
--rw-rw-rw-   0        0        0     4237 2022-10-08 09:28:26.000000 cs1-0.2.3/src/cs1/security/tvsm.py
-drwxrwxrwx   0        0        0        0 2023-06-03 05:05:21.626648 cs1-0.2.3/src/cs1.egg-info/
--rw-rw-rw-   0        0        0     4998 2023-06-03 05:05:21.000000 cs1-0.2.3/src/cs1.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0     2317 2023-06-03 05:05:21.000000 cs1-0.2.3/src/cs1.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-06-03 05:05:21.000000 cs1-0.2.3/src/cs1.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       91 2023-06-03 05:05:21.000000 cs1-0.2.3/src/cs1.egg-info/requires.txt
--rw-rw-rw-   0        0        0        4 2023-06-03 05:05:21.000000 cs1-0.2.3/src/cs1.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-06-12 03:07:02.242056 cs1-0.2.4/
+-rw-rw-rw-   0        0        0      214 2022-03-26 07:50:46.000000 cs1-0.2.4/LICENCE
+-rw-rw-rw-   0        0        0     4998 2023-06-12 03:07:02.243057 cs1-0.2.4/PKG-INFO
+-rw-rw-rw-   0        0        0     4359 2023-06-03 02:56:39.000000 cs1-0.2.4/README.md
+-rw-rw-rw-   0        0        0      108 2022-01-07 07:21:30.000000 cs1-0.2.4/pyproject.toml
+-rw-rw-rw-   0        0        0     1023 2023-06-12 03:07:02.246055 cs1-0.2.4/setup.cfg
+drwxrwxrwx   0        0        0        0 2023-06-12 03:07:02.104721 cs1-0.2.4/src/
+drwxrwxrwx   0        0        0        0 2023-06-12 03:07:02.123535 cs1-0.2.4/src/cs1/
+-rw-rw-rw-   0        0        0    38783 2023-02-24 08:13:59.000000 cs1-0.2.4/src/cs1/__init__.py
+drwxrwxrwx   0        0        0        0 2023-06-12 03:07:02.147523 cs1-0.2.4/src/cs1/basis/
+-rw-rw-rw-   0        0        0        0 2022-10-07 10:23:54.000000 cs1-0.2.4/src/cs1/basis/__init__.py
+drwxrwxrwx   0        0        0        0 2023-06-12 03:07:02.150529 cs1-0.2.4/src/cs1/basis/adaptive/
+-rw-rw-rw-   0        0        0     5124 2023-06-05 05:01:27.000000 cs1-0.2.4/src/cs1/basis/adaptive/__init__.py
+-rw-rw-rw-   0        0        0    18165 2023-04-04 07:11:28.000000 cs1-0.2.4/src/cs1/basis/adaptive/vae.py
+-rw-rw-rw-   0        0        0     7148 2023-01-15 10:21:44.000000 cs1-0.2.4/src/cs1/basis/common.py
+-rw-rw-rw-   0        0        0    31223 2023-06-12 03:05:17.000000 cs1-0.2.4/src/cs1/cs.py
+drwxrwxrwx   0        0        0        0 2023-06-12 03:07:02.153533 cs1-0.2.4/src/cs1/domain/
+-rw-rw-rw-   0        0        0      693 2022-10-08 07:15:14.000000 cs1-0.2.4/src/cs1/domain/__init__.py
+-rw-rw-rw-   0        0        0     9862 2023-01-08 15:31:23.000000 cs1-0.2.4/src/cs1/domain/audio.py
+-rw-rw-rw-   0        0        0    11912 2023-01-15 13:30:15.000000 cs1-0.2.4/src/cs1/domain/image.py
+drwxrwxrwx   0        0        0        0 2023-06-12 03:07:02.155530 cs1-0.2.4/src/cs1/gui/
+-rw-rw-rw-   0        0        0        0 2022-10-07 10:23:54.000000 cs1-0.2.4/src/cs1/gui/__init__.py
+-rw-rw-rw-   0        0        0     4433 2023-03-16 02:40:31.000000 cs1-0.2.4/src/cs1/gui/run.py
+drwxrwxrwx   0        0        0        0 2023-06-12 03:07:02.177054 cs1-0.2.4/src/cs1/gui/static/
+-rw-rw-rw-   0        0        0        0 2022-01-07 02:28:31.000000 cs1-0.2.4/src/cs1/gui/static/__init__.py
+-rw-rw-rw-   0        0        0     2518 2022-07-20 15:27:40.000000 cs1-0.2.4/src/cs1/gui/static/bootstrap-dialog.css
+-rw-rw-rw-   0        0        0   192352 2020-09-09 05:39:36.000000 cs1-0.2.4/src/cs1/gui/static/bootstrap.css
+-rw-rw-rw-   0        0        0   131637 2020-02-15 01:34:39.000000 cs1-0.2.4/src/cs1/gui/static/bootstrap.js
+-rw-rw-rw-   0        0        0    37444 2022-11-12 14:05:28.000000 cs1-0.2.4/src/cs1/gui/static/font-awesome.css
+drwxrwxrwx   0        0        0        0 2023-06-12 03:07:02.198078 cs1-0.2.4/src/cs1/gui/static/fonts/
+-rw-rw-rw-   0        0        0   134808 2022-07-20 15:27:41.000000 cs1-0.2.4/src/cs1/gui/static/fonts/FontAwesome.otf
+-rw-rw-rw-   0        0        0        0 2022-01-07 02:28:31.000000 cs1-0.2.4/src/cs1/gui/static/fonts/__init__.py
+-rw-rw-rw-   0        0        0   165742 2022-07-20 15:27:41.000000 cs1-0.2.4/src/cs1/gui/static/fonts/fontawesome-webfont.eot
+-rw-rw-rw-   0        0        0   447050 2022-07-20 15:27:41.000000 cs1-0.2.4/src/cs1/gui/static/fonts/fontawesome-webfont.svg
+-rw-rw-rw-   0        0        0   165548 2022-07-20 15:27:41.000000 cs1-0.2.4/src/cs1/gui/static/fonts/fontawesome-webfont.ttf
+-rw-rw-rw-   0        0        0    98024 2022-07-20 15:27:41.000000 cs1-0.2.4/src/cs1/gui/static/fonts/fontawesome-webfont.woff
+-rw-rw-rw-   0        0        0    77160 2022-07-20 15:27:41.000000 cs1-0.2.4/src/cs1/gui/static/fonts/fontawesome-webfont.woff2
+-rw-rw-rw-   0        0        0    20127 2022-07-20 15:27:41.000000 cs1-0.2.4/src/cs1/gui/static/fonts/glyphicons-halflings-regular.eot
+-rw-rw-rw-   0        0        0   108738 2022-07-20 15:27:41.000000 cs1-0.2.4/src/cs1/gui/static/fonts/glyphicons-halflings-regular.svg
+-rw-rw-rw-   0        0        0    45404 2022-07-20 15:27:41.000000 cs1-0.2.4/src/cs1/gui/static/fonts/glyphicons-halflings-regular.ttf
+-rw-rw-rw-   0        0        0    23424 2022-07-20 15:27:41.000000 cs1-0.2.4/src/cs1/gui/static/fonts/glyphicons-halflings-regular.woff
+-rw-rw-rw-   0        0        0    18028 2022-07-20 15:27:41.000000 cs1-0.2.4/src/cs1/gui/static/fonts/glyphicons-halflings-regular.woff2
+drwxrwxrwx   0        0        0        0 2023-06-12 03:07:02.230052 cs1-0.2.4/src/cs1/gui/static/images/
+-rw-rw-rw-   0        0        0    51449 2022-07-20 15:47:00.000000 cs1-0.2.4/src/cs1/gui/static/images/BCoT.png
+-rw-rw-rw-   0        0        0   111921 2022-07-20 15:47:00.000000 cs1-0.2.4/src/cs1/gui/static/images/DCT.png
+-rw-rw-rw-   0        0        0    74145 2022-07-20 15:47:00.000000 cs1-0.2.4/src/cs1/gui/static/images/DFT.png
+-rw-rw-rw-   0        0        0     8052 2022-07-20 15:47:00.000000 cs1-0.2.4/src/cs1/gui/static/images/DFT_A.png
+-rw-rw-rw-   0        0        0   108584 2022-07-20 15:47:00.000000 cs1-0.2.4/src/cs1/gui/static/images/DFT_P.png
+-rw-rw-rw-   0        0        0    13354 2022-07-20 15:47:00.000000 cs1-0.2.4/src/cs1/gui/static/images/HWT.png
+-rw-rw-rw-   0        0        0     1511 2022-07-20 15:47:00.000000 cs1-0.2.4/src/cs1/gui/static/images/IDM.png
+-rw-rw-rw-   0        0        0    86935 2022-07-20 15:47:00.000000 cs1-0.2.4/src/cs1/gui/static/images/SECS.png
+-rw-rw-rw-   0        0        0    71199 2022-07-20 15:47:00.000000 cs1-0.2.4/src/cs1/gui/static/images/Sensing - clean.png
+-rw-rw-rw-   0        0        0        0 2022-01-07 02:28:31.000000 cs1-0.2.4/src/cs1/gui/static/images/__init__.py
+-rw-rw-rw-   0        0        0    80565 2022-07-20 15:47:00.000000 cs1-0.2.4/src/cs1/gui/static/images/reconstruction - clean.png
+-rw-rw-rw-   0        0        0   264308 2022-07-20 15:47:00.000000 cs1-0.2.4/src/cs1/gui/static/images/reconstruction.png
+-rw-rw-rw-   0        0        0   152714 2022-07-20 15:47:00.000000 cs1-0.2.4/src/cs1/gui/static/images/sensing matrix - clean.png
+-rw-rw-rw-   0        0        0   804558 2022-07-20 15:47:00.000000 cs1-0.2.4/src/cs1/gui/static/images/sensing matrix.jpeg
+-rw-rw-rw-   0        0        0   160937 2022-07-20 15:47:00.000000 cs1-0.2.4/src/cs1/gui/static/images/sensing.png
+-rw-rw-rw-   0        0        0    86927 2020-02-15 01:36:15.000000 cs1-0.2.4/src/cs1/gui/static/jquery-3.3.1.min.js
+-rw-rw-rw-   0        0        0   520714 2022-07-20 15:28:09.000000 cs1-0.2.4/src/cs1/gui/static/jquery-ui-1.12.1.js
+-rw-rw-rw-   0        0        0    64017 2022-07-20 15:27:42.000000 cs1-0.2.4/src/cs1/gui/static/jquery-ui.css
+-rw-rw-rw-   0        0        0    24228 2020-02-15 04:11:19.000000 cs1-0.2.4/src/cs1/gui/static/jquery.blockUI.js
+-rw-rw-rw-   0        0        0    17108 2020-02-15 04:11:19.000000 cs1-0.2.4/src/cs1/gui/static/jquery.form.min.js
+-rw-rw-rw-   0        0        0     8602 2022-07-20 15:28:18.000000 cs1-0.2.4/src/cs1/gui/static/seedrandom.js
+-rw-rw-rw-   0        0        0     4727 2022-11-12 02:00:29.000000 cs1-0.2.4/src/cs1/gui/static/utility.chart.js
+drwxrwxrwx   0        0        0        0 2023-06-12 03:07:02.238058 cs1-0.2.4/src/cs1/gui/templates/
+-rw-rw-rw-   0        0        0        0 2022-11-03 12:58:21.000000 cs1-0.2.4/src/cs1/gui/templates/__init__.py
+-rw-rw-rw-   0        0        0    95318 2022-11-18 14:09:58.000000 cs1-0.2.4/src/cs1/gui/templates/home.html
+-rw-rw-rw-   0        0        0    23043 2022-11-18 14:32:23.000000 cs1-0.2.4/src/cs1/gui/templates/receiver.html
+-rw-rw-rw-   0        0        0     8549 2022-11-19 14:14:31.000000 cs1-0.2.4/src/cs1/gui/templates/tutorial.html
+-rw-rw-rw-   0        0        0     7753 2023-01-15 08:44:54.000000 cs1-0.2.4/src/cs1/metrics.py
+drwxrwxrwx   0        0        0        0 2023-06-12 03:07:02.240052 cs1-0.2.4/src/cs1/security/
+-rw-rw-rw-   0        0        0        0 2022-10-07 10:23:54.000000 cs1-0.2.4/src/cs1/security/__init__.py
+-rw-rw-rw-   0        0        0     4237 2022-10-08 09:28:26.000000 cs1-0.2.4/src/cs1/security/tvsm.py
+drwxrwxrwx   0        0        0        0 2023-06-12 03:07:02.145525 cs1-0.2.4/src/cs1.egg-info/
+-rw-rw-rw-   0        0        0     4998 2023-06-12 03:07:02.000000 cs1-0.2.4/src/cs1.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0     2317 2023-06-12 03:07:02.000000 cs1-0.2.4/src/cs1.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-06-12 03:07:02.000000 cs1-0.2.4/src/cs1.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       97 2023-06-12 03:07:02.000000 cs1-0.2.4/src/cs1.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        4 2023-06-12 03:07:02.000000 cs1-0.2.4/src/cs1.egg-info/top_level.txt
```

### Comparing `cs1-0.2.3/PKG-INFO` & `cs1-0.2.4/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cs1
-Version: 0.2.3
+Version: 0.2.4
 Summary: Compressed Sensing library for 1D Spectroscopic Profiling Data
 Home-page: https://github.com/zhangys11/cs1
 Author: Yinsheng Zhang (Ph.D.)
 Author-email: oo@zju.edu.cn
 Project-URL: Bug Tracker, https://github.com/zhangys11/cs1/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: GNU Lesser General Public License v3 or later (LGPLv3+)
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: cs1 Version: 0.2.3 Summary: Compressed Sensing
+Metadata-Version: 2.1 Name: cs1 Version: 0.2.4 Summary: Compressed Sensing
 library for 1D Spectroscopic Profiling Data Home-page: https://github.com/
 zhangys11/cs1 Author: Yinsheng Zhang (Ph.D.) Author-email: oo@zju.edu.cn
 Project-URL: Bug Tracker, https://github.com/zhangys11/cs1/issues Classifier:
 Programming Language :: Python :: 3 Classifier: License :: OSI Approved :: GNU
 Lesser General Public License v3 or later (LGPLv3+) Classifier: Operating
 System :: OS Independent Classifier: Topic :: Scientific/Engineering ::
 Mathematics Requires-Python: >=3.6 Description-Content-Type: text/markdown
```

### Comparing `cs1-0.2.3/README.md` & `cs1-0.2.4/README.md`

 * *Files identical despite different names*

### Comparing `cs1-0.2.3/setup.cfg` & `cs1-0.2.4/setup.cfg`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 00000000: 5b6d 6574 6164 6174 615d 0d0a 6e61 6d65  [metadata]..name
 00000010: 203d 2063 7331 0d0a 7665 7273 696f 6e20   = cs1..version 
-00000020: 3d20 302e 322e 330d 0a61 7574 686f 7220  = 0.2.3..author 
+00000020: 3d20 302e 322e 340d 0a61 7574 686f 7220  = 0.2.4..author 
 00000030: 3d20 5969 6e73 6865 6e67 205a 6861 6e67  = Yinsheng Zhang
 00000040: 2028 5068 2e44 2e29 0d0a 6175 7468 6f72   (Ph.D.)..author
 00000050: 5f65 6d61 696c 203d 206f 6f40 7a6a 752e  _email = oo@zju.
 00000060: 6564 752e 636e 0d0a 6465 7363 7269 7074  edu.cn..descript
 00000070: 696f 6e20 3d20 436f 6d70 7265 7373 6564  ion = Compressed
 00000080: 2053 656e 7369 6e67 206c 6962 7261 7279   Sensing library
 00000090: 2066 6f72 2031 4420 5370 6563 7472 6f73   for 1D Spectros
@@ -44,21 +44,21 @@
 000002b0: 6c6c 5f72 6571 7569 7265 7320 3d20 0d0a  ll_requires = ..
 000002c0: 0973 6369 6b69 742d 6c65 6172 6e0d 0a09  .scikit-learn...
 000002d0: 6d61 7470 6c6f 746c 6962 0d0a 096e 756d  matplotlib...num
 000002e0: 7079 0d0a 0950 7957 6176 656c 6574 730d  py...PyWavelets.
 000002f0: 0a09 7374 6174 736d 6f64 656c 730d 0a09  ..statsmodels...
 00000300: 7079 6475 620d 0a09 6f70 656e 6376 2d70  pydub...opencv-p
 00000310: 7974 686f 6e0d 0a09 746f 7263 680d 0a09  ython...torch...
-00000320: 746f 7263 6876 6973 696f 6e0d 0a0d 0a5b  torchvision....[
-00000330: 6f70 7469 6f6e 732e 7061 636b 6167 6573  options.packages
-00000340: 2e66 696e 645d 0d0a 7768 6572 6520 3d20  .find]..where = 
-00000350: 7372 630d 0a0d 0a5b 6f70 7469 6f6e 732e  src....[options.
-00000360: 7061 636b 6167 655f 6461 7461 5d0d 0a2a  package_data]..*
-00000370: 203d 202a 2e68 746d 6c2c 202a 2e6a 732c   = *.html, *.js,
-00000380: 202a 2e63 7373 2c20 2a2e 776f 6666 2c20   *.css, *.woff, 
-00000390: 2a2e 776f 6666 322c 202a 2e74 7466 2c20  *.woff2, *.ttf, 
-000003a0: 2a2e 7376 672c 202a 2e65 6f74 2c20 2a2e  *.svg, *.eot, *.
-000003b0: 6f74 662c 202a 2e70 6e67 2c20 2a2e 6a70  otf, *.png, *.jp
-000003c0: 6567 2c20 2a2e 6a70 670d 0a0d 0a5b 6567  eg, *.jpg....[eg
-000003d0: 675f 696e 666f 5d0d 0a74 6167 5f62 7569  g_info]..tag_bui
-000003e0: 6c64 203d 200d 0a74 6167 5f64 6174 6520  ld = ..tag_date 
-000003f0: 3d20 300d 0a0d 0a                        = 0....
+00000320: 746f 7263 6876 6973 696f 6e0d 0a09 7363  torchvision...sc
+00000330: 6970 790d 0a0d 0a5b 6f70 7469 6f6e 732e  ipy....[options.
+00000340: 7061 636b 6167 6573 2e66 696e 645d 0d0a  packages.find]..
+00000350: 7768 6572 6520 3d20 7372 630d 0a0d 0a5b  where = src....[
+00000360: 6f70 7469 6f6e 732e 7061 636b 6167 655f  options.package_
+00000370: 6461 7461 5d0d 0a2a 203d 202a 2e68 746d  data]..* = *.htm
+00000380: 6c2c 202a 2e6a 732c 202a 2e63 7373 2c20  l, *.js, *.css, 
+00000390: 2a2e 776f 6666 2c20 2a2e 776f 6666 322c  *.woff, *.woff2,
+000003a0: 202a 2e74 7466 2c20 2a2e 7376 672c 202a   *.ttf, *.svg, *
+000003b0: 2e65 6f74 2c20 2a2e 6f74 662c 202a 2e70  .eot, *.otf, *.p
+000003c0: 6e67 2c20 2a2e 6a70 6567 2c20 2a2e 6a70  ng, *.jpeg, *.jp
+000003d0: 670d 0a0d 0a5b 6567 675f 696e 666f 5d0d  g....[egg_info].
+000003e0: 0a74 6167 5f62 7569 6c64 203d 200d 0a74  .tag_build = ..t
+000003f0: 6167 5f64 6174 6520 3d20 300d 0a0d 0a    ag_date = 0....
```

### Comparing `cs1-0.2.3/src/cs1/__init__.py` & `cs1-0.2.4/src/cs1/__init__.py`

 * *Files identical despite different names*

### Comparing `cs1-0.2.3/src/cs1/basis/adaptive/__init__.py` & `cs1-0.2.4/src/cs1/basis/adaptive/__init__.py`

 * *Files identical despite different names*

### Comparing `cs1-0.2.3/src/cs1/basis/adaptive/vae.py` & `cs1-0.2.4/src/cs1/basis/adaptive/vae.py`

 * *Files identical despite different names*

### Comparing `cs1-0.2.3/src/cs1/basis/common.py` & `cs1-0.2.4/src/cs1/basis/common.py`

 * *Files identical despite different names*

### Comparing `cs1-0.2.3/src/cs1/cs.py` & `cs1-0.2.4/src/cs1/cs.py`

 * *Files 14% similar despite different names*

```diff
@@ -13,16 +13,17 @@
 import matplotlib.pyplot as plt
 from matplotlib import cm
 import pylab
 
 from sklearn.preprocessing import StandardScaler
 from sklearn.decomposition import PCA
 from sklearn.discriminant_analysis import LinearDiscriminantAnalysis
-from sklearn.linear_model import Lasso, LassoCV, LogisticRegressionCV, OrthogonalMatchingPursuit
+from sklearn.linear_model import LinearRegression, Lasso, LassoCV, LogisticRegressionCV, OrthogonalMatchingPursuit
 from statsmodels.multivariate.manova import MANOVA
+from scipy.signal import savgol_filter
 
 if __package__:
     from . import GetSensingMatrix, SensingWithPHI, PSI_LONGNAMES, PSI_NAMES
     from .basis.common import Generate_PSI
     from .metrics import Univariate_KLD, Multivarate_KLD, calculate_recon_error
 else:
     DIR = os.path.dirname(__file__)  # cs1 dir
@@ -611,14 +612,203 @@
             Xc2 = Xr_lda[y == c]
 
         ukld = Univariate_KLD( (Xc1.mean(), Xc1.std()),  (Xc2.mean(), Xc2.std()) )
         print('KLD between the orignal and reconstructed signals ( y = ' + str(c) +  '): ', round(ukld,3))
     
     return Z, Xr
 
+def preprocessed_singal_sensing_n_recovery(x, X, PSIs, ks = [0.01, 0.05,0.1,0.3,0.5,1]):
+    
+    '''
+    This function demonstrates the performance of CS recovery on different preprocessed signals, i.e., 1st derivative, 2nd derivative, scatter correction, and savagol smooth filter.
+    
+    Parameters
+    ----------
+    x : target signal 
+    X : the entire training set. Used only for scatter correction.
+    PSIs : a list of PSIs for comparison
+    ks : a list of sampling ratios for comparison
+
+    Examples:
+    ---------
+    selected_PSIs = {}
+    for key in ['DFT','DCT']: 
+        selected_PSIs[key] = PSIs[key]
+    _ = preprocessed_singal_sensing_n_recovery(X[0], X, selected_PSIs , ks = [0.01, 0.05,0.1,0.3,0.5,1])
+    '''
+    def D1(x):
+        return np.array([0] + list(np.diff(x)))
+    
+    # Second derivatives
+    def D2(x):        
+        return D1(D1(x))
+
+
+    # Scatter correction
+    def MSC(X):
+        '''
+        X : a batch of samples for training, not a single sample.
+        
+        Sample
+        ------
+        plt.plot(MSC(X)[0]) # display the 1st sample after MSC
+        '''
+        n, p = X.shape
+        Xmsc = np.ones((n, p))
+
+        # mu = x.mean()
+
+        for j in range(n):
+            mu = np.mean(X, axis=0)
+
+        for i in range(n):
+            y = X[i, :]
+            l = LinearRegression()
+            l.fit(mu.reshape(-1, 1), y.reshape(-1, 1))
+            k = l.coef_
+            b = l.intercept_
+            Xmsc[i, :] = (y - b) / k
+
+        return Xmsc
+    
+    
+    x1=D1(x)
+    x2=D2(x)
+    x3=savgol_filter(x, window_length=5, polyorder=3)    
+    x4=MSC(X)[0]
+        
+    for x, method in zip([x1,x2,x3,x4],['1st derivative','2nd derivative','smooth filtering','scatter correction']):
+        
+        # print(method)        
+    
+        plt.figure(figsize=(15 + len(ks)*5, len(PSIs)*7))
+        rows = len(PSIs) + 1
+        matplotlib.rcParams.update({'font.size': 24})    
+        COLS = 3 + len(ks)
+        MSES = []
+        RMSES = []
+
+        for idx, key in enumerate(PSIs):
+
+            PSI = PSIs[key]
+        
+            # padded version
+            xe = np.copy(x)
+        
+            # pad x with zero if necessary
+            if (len(x) < len(PSI)): # the HWT case
+                xe = np.zeros(len(PSI))
+                xe[:len(x)] = x     
+            if len(xe) % 2 == 1:
+                xe = xe[:-1] # xe = np.append(xe, 0) # make even length, as required by some transform, e.g., DCT
+                PSI = PSI[:-1,:-1] # align with xe
+        
+            psi_name = key
+        
+            z = PSI @ xe
+            
+            MAX = np.max(np.abs(z)) # abs(max(z, key=abs))
+            thresholds = np.array(range(100)) / 50000
+        
+            rs =[]
+            for threshold in thresholds:
+                rs.append((np.abs(np.array(z)) <= threshold * MAX).sum() / len(z))
+            
+            auc = 0
+            for i in range(1000):
+                auc += (np.abs(np.array(z)) <= (i+1)/1000 * MAX).sum() / len(z)        
+            auc = auc/1000
+        
+            r = (np.abs(np.array(z)) <= 0.001 * MAX).sum() / len(z)  #   # use 0.001 MAX ABS as threshold # sys.float_info.epsilon
+        
+        
+            ########## plot ###########    
+    
+            plt.subplot(rows,COLS,COLS*idx+1)  
+            plt.title(method)
+            plt.plot(x)
+            plt.xticks([])
+            plt.yticks([])  
+            
+            
+            plt.subplot(rows,COLS,COLS*idx+2)    
+            if PSI.dtype == 'complex': # DFT
+                plt.title('\n'+psi_name + ' basis(phase)')
+                plt.imshow(np.angle(PSI), interpolation='nearest', cmap=cm.Greys_r)
+            else:
+                plt.title('\n'+psi_name + ' basis')
+                plt.imshow(PSI, interpolation='nearest', cmap=cm.Greys_r)
+            plt.axis('off')
+            
+            
+            plt.subplot(rows,COLS,COLS*idx+3)
+
+            if np.any(np.iscomplex(z)):
+                plt.plot(np.abs(z), color='gray')
+            else:
+                plt.plot(z, color = 'gray')
+                
+            if idx == 0:
+                plt.title('z (latent space)') # '\n'+psi_name + 
+
+            plt.xticks([])
+            plt.yticks([])
+            # plt.axis('off')
+        
+            mses = []
+            rmses = []
+        
+            for kidx, k in enumerate(ks):
+        
+                ########## sensing #############
+
+                # either works fine
+                if True:
+                    PHI, OMEGA = GetSensingMatrix(len(xe), k)            
+                    xs = PHI @ xe
+                    pidx = np.argmax(PHI, axis = 1)
+                else:
+                    xs, pidx = Sensing(xe, k)
+                    PHI = np.zeros((len(pidx), len(xe)))
+                    for i,j in enumerate(pidx):
+                        PHI[i, j] = 1
+
+                ####### reconstruction ##########
+            
+                A = MeasurementMatrix(len(xe), pidx, psi_name)
+                W = None
+                if (psi_name == 'HWT' or psi_name == 'DWT' or psi_name == 'ROM' or \
+                    psi_name == 'EBP' or psi_name == 'LDA'):
+                    W = PSI
+                    A = PHI @ W  
+
+                else:
+                    A = MeasurementMatrix(len(xe), pidx, psi_name)
+                    W = None
+
+                z, xr = Recovery (A, xs, psi_name, display = False, PSI = W, ) # lower k needs bigger L1. k 0.1 - L1 0.1, k 0.01, L1 - 10
+            
+                mse, _, rmse = calculate_recon_error(xe.reshape(1, -1), xr.reshape(1, -1)) #(np.matrix(xe), np.matrix(xr))        
+                mses.append(mse)
+                rmses.append(rmse)
+            
+                plt.subplot(rows,COLS,COLS*idx+3+1+kidx)
+                plt.plot(xr[:len(x)]) #, label = 'RMSE ' + str( round(rmse, 3) ), color='gray') # cut the first n points, as in HWT, xr is padded.
+                if idx == 0:
+                    plt.title('$x_r$ ($k$=' + str(round(k, 2)) + ', $n_s$=' + str(len(xs)) + ')')
+                plt.xticks([])
+                plt.yticks([])                
+                # plt.legend()
+            
+            MSES.append(mses)
+            RMSES.append(rmses)
+            
+        plt.show()
+        
+    return MSES, RMSES
 
 def plot_reconstructed(z, xr):
     '''
     Plot the reconstructed latent representation z and the reconstructed signal xr
     '''
     matplotlib.rcParams.update({'font.size': 20})
```

### Comparing `cs1-0.2.3/src/cs1/domain/__init__.py` & `cs1-0.2.4/src/cs1/domain/__init__.py`

 * *Files identical despite different names*

### Comparing `cs1-0.2.3/src/cs1/domain/audio.py` & `cs1-0.2.4/src/cs1/domain/audio.py`

 * *Files identical despite different names*

### Comparing `cs1-0.2.3/src/cs1/domain/image.py` & `cs1-0.2.4/src/cs1/domain/image.py`

 * *Files identical despite different names*

### Comparing `cs1-0.2.3/src/cs1/gui/run.py` & `cs1-0.2.4/src/cs1/gui/run.py`

 * *Files identical despite different names*

### Comparing `cs1-0.2.3/src/cs1/gui/static/bootstrap-dialog.css` & `cs1-0.2.4/src/cs1/gui/static/bootstrap-dialog.css`

 * *Files identical despite different names*

### Comparing `cs1-0.2.3/src/cs1/gui/static/bootstrap.css` & `cs1-0.2.4/src/cs1/gui/static/bootstrap.css`

 * *Files identical despite different names*

### Comparing `cs1-0.2.3/src/cs1/gui/static/bootstrap.js` & `cs1-0.2.4/src/cs1/gui/static/bootstrap.js`

 * *Files identical despite different names*

### Comparing `cs1-0.2.3/src/cs1/gui/static/font-awesome.css` & `cs1-0.2.4/src/cs1/gui/static/font-awesome.css`

 * *Files identical despite different names*

### Comparing `cs1-0.2.3/src/cs1/gui/static/fonts/FontAwesome.otf` & `cs1-0.2.4/src/cs1/gui/static/fonts/FontAwesome.otf`

 * *Files identical despite different names*

### Comparing `cs1-0.2.3/src/cs1/gui/static/fonts/fontawesome-webfont.eot` & `cs1-0.2.4/src/cs1/gui/static/fonts/fontawesome-webfont.eot`

 * *Files identical despite different names*

### Comparing `cs1-0.2.3/src/cs1/gui/static/fonts/fontawesome-webfont.svg` & `cs1-0.2.4/src/cs1/gui/static/fonts/fontawesome-webfont.svg`

 * *Files identical despite different names*

### Comparing `cs1-0.2.3/src/cs1/gui/static/fonts/fontawesome-webfont.ttf` & `cs1-0.2.4/src/cs1/gui/static/fonts/fontawesome-webfont.ttf`

 * *Files identical despite different names*

### Comparing `cs1-0.2.3/src/cs1/gui/static/fonts/fontawesome-webfont.woff` & `cs1-0.2.4/src/cs1/gui/static/fonts/fontawesome-webfont.woff`

 * *Files identical despite different names*

### Comparing `cs1-0.2.3/src/cs1/gui/static/fonts/fontawesome-webfont.woff2` & `cs1-0.2.4/src/cs1/gui/static/fonts/fontawesome-webfont.woff2`

 * *Files identical despite different names*

### Comparing `cs1-0.2.3/src/cs1/gui/static/fonts/glyphicons-halflings-regular.eot` & `cs1-0.2.4/src/cs1/gui/static/fonts/glyphicons-halflings-regular.eot`

 * *Files identical despite different names*

### Comparing `cs1-0.2.3/src/cs1/gui/static/fonts/glyphicons-halflings-regular.svg` & `cs1-0.2.4/src/cs1/gui/static/fonts/glyphicons-halflings-regular.svg`

 * *Files identical despite different names*

### Comparing `cs1-0.2.3/src/cs1/gui/static/fonts/glyphicons-halflings-regular.ttf` & `cs1-0.2.4/src/cs1/gui/static/fonts/glyphicons-halflings-regular.ttf`

 * *Files identical despite different names*

### Comparing `cs1-0.2.3/src/cs1/gui/static/fonts/glyphicons-halflings-regular.woff` & `cs1-0.2.4/src/cs1/gui/static/fonts/glyphicons-halflings-regular.woff`

 * *Files identical despite different names*

### Comparing `cs1-0.2.3/src/cs1/gui/static/fonts/glyphicons-halflings-regular.woff2` & `cs1-0.2.4/src/cs1/gui/static/fonts/glyphicons-halflings-regular.woff2`

 * *Files identical despite different names*

### Comparing `cs1-0.2.3/src/cs1/gui/static/images/BCoT.png` & `cs1-0.2.4/src/cs1/gui/static/images/BCoT.png`

 * *Files identical despite different names*

### Comparing `cs1-0.2.3/src/cs1/gui/static/images/DCT.png` & `cs1-0.2.4/src/cs1/gui/static/images/DCT.png`

 * *Files identical despite different names*

### Comparing `cs1-0.2.3/src/cs1/gui/static/images/DFT.png` & `cs1-0.2.4/src/cs1/gui/static/images/DFT.png`

 * *Files identical despite different names*

### Comparing `cs1-0.2.3/src/cs1/gui/static/images/DFT_A.png` & `cs1-0.2.4/src/cs1/gui/static/images/DFT_A.png`

 * *Files identical despite different names*

### Comparing `cs1-0.2.3/src/cs1/gui/static/images/DFT_P.png` & `cs1-0.2.4/src/cs1/gui/static/images/DFT_P.png`

 * *Files identical despite different names*

### Comparing `cs1-0.2.3/src/cs1/gui/static/images/HWT.png` & `cs1-0.2.4/src/cs1/gui/static/images/HWT.png`

 * *Files identical despite different names*

### Comparing `cs1-0.2.3/src/cs1/gui/static/images/IDM.png` & `cs1-0.2.4/src/cs1/gui/static/images/IDM.png`

 * *Files identical despite different names*

### Comparing `cs1-0.2.3/src/cs1/gui/static/images/SECS.png` & `cs1-0.2.4/src/cs1/gui/static/images/SECS.png`

 * *Files identical despite different names*

### Comparing `cs1-0.2.3/src/cs1/gui/static/images/Sensing - clean.png` & `cs1-0.2.4/src/cs1/gui/static/images/Sensing - clean.png`

 * *Files identical despite different names*

### Comparing `cs1-0.2.3/src/cs1/gui/static/images/reconstruction - clean.png` & `cs1-0.2.4/src/cs1/gui/static/images/reconstruction - clean.png`

 * *Files identical despite different names*

### Comparing `cs1-0.2.3/src/cs1/gui/static/images/reconstruction.png` & `cs1-0.2.4/src/cs1/gui/static/images/reconstruction.png`

 * *Files identical despite different names*

### Comparing `cs1-0.2.3/src/cs1/gui/static/images/sensing matrix - clean.png` & `cs1-0.2.4/src/cs1/gui/static/images/sensing matrix - clean.png`

 * *Files identical despite different names*

### Comparing `cs1-0.2.3/src/cs1/gui/static/images/sensing matrix.jpeg` & `cs1-0.2.4/src/cs1/gui/static/images/sensing matrix.jpeg`

 * *Files identical despite different names*

### Comparing `cs1-0.2.3/src/cs1/gui/static/images/sensing.png` & `cs1-0.2.4/src/cs1/gui/static/images/sensing.png`

 * *Files identical despite different names*

### Comparing `cs1-0.2.3/src/cs1/gui/static/jquery-3.3.1.min.js` & `cs1-0.2.4/src/cs1/gui/static/jquery-3.3.1.min.js`

 * *Files identical despite different names*

### Comparing `cs1-0.2.3/src/cs1/gui/static/jquery-ui-1.12.1.js` & `cs1-0.2.4/src/cs1/gui/static/jquery-ui-1.12.1.js`

 * *Files identical despite different names*

### Comparing `cs1-0.2.3/src/cs1/gui/static/jquery-ui.css` & `cs1-0.2.4/src/cs1/gui/static/jquery-ui.css`

 * *Files identical despite different names*

### Comparing `cs1-0.2.3/src/cs1/gui/static/jquery.blockUI.js` & `cs1-0.2.4/src/cs1/gui/static/jquery.blockUI.js`

 * *Files identical despite different names*

### Comparing `cs1-0.2.3/src/cs1/gui/static/jquery.form.min.js` & `cs1-0.2.4/src/cs1/gui/static/jquery.form.min.js`

 * *Files identical despite different names*

### Comparing `cs1-0.2.3/src/cs1/gui/static/seedrandom.js` & `cs1-0.2.4/src/cs1/gui/static/seedrandom.js`

 * *Files identical despite different names*

### Comparing `cs1-0.2.3/src/cs1/gui/static/utility.chart.js` & `cs1-0.2.4/src/cs1/gui/static/utility.chart.js`

 * *Files identical despite different names*

### Comparing `cs1-0.2.3/src/cs1/gui/templates/home.html` & `cs1-0.2.4/src/cs1/gui/templates/home.html`

 * *Files identical despite different names*

### Comparing `cs1-0.2.3/src/cs1/gui/templates/receiver.html` & `cs1-0.2.4/src/cs1/gui/templates/receiver.html`

 * *Files identical despite different names*

### Comparing `cs1-0.2.3/src/cs1/gui/templates/tutorial.html` & `cs1-0.2.4/src/cs1/gui/templates/tutorial.html`

 * *Files identical despite different names*

### Comparing `cs1-0.2.3/src/cs1/metrics.py` & `cs1-0.2.4/src/cs1/metrics.py`

 * *Files identical despite different names*

### Comparing `cs1-0.2.3/src/cs1/security/tvsm.py` & `cs1-0.2.4/src/cs1/security/tvsm.py`

 * *Files identical despite different names*

### Comparing `cs1-0.2.3/src/cs1.egg-info/PKG-INFO` & `cs1-0.2.4/src/cs1.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cs1
-Version: 0.2.3
+Version: 0.2.4
 Summary: Compressed Sensing library for 1D Spectroscopic Profiling Data
 Home-page: https://github.com/zhangys11/cs1
 Author: Yinsheng Zhang (Ph.D.)
 Author-email: oo@zju.edu.cn
 Project-URL: Bug Tracker, https://github.com/zhangys11/cs1/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: GNU Lesser General Public License v3 or later (LGPLv3+)
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: cs1 Version: 0.2.3 Summary: Compressed Sensing
+Metadata-Version: 2.1 Name: cs1 Version: 0.2.4 Summary: Compressed Sensing
 library for 1D Spectroscopic Profiling Data Home-page: https://github.com/
 zhangys11/cs1 Author: Yinsheng Zhang (Ph.D.) Author-email: oo@zju.edu.cn
 Project-URL: Bug Tracker, https://github.com/zhangys11/cs1/issues Classifier:
 Programming Language :: Python :: 3 Classifier: License :: OSI Approved :: GNU
 Lesser General Public License v3 or later (LGPLv3+) Classifier: Operating
 System :: OS Independent Classifier: Topic :: Scientific/Engineering ::
 Mathematics Requires-Python: >=3.6 Description-Content-Type: text/markdown
```

### Comparing `cs1-0.2.3/src/cs1.egg-info/SOURCES.txt` & `cs1-0.2.4/src/cs1.egg-info/SOURCES.txt`

 * *Files identical despite different names*

