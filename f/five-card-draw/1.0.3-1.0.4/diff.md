# Comparing `tmp/five_card_draw-1.0.3.tar.gz` & `tmp/five_card_draw-1.0.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "five_card_draw-1.0.3.tar", last modified: Sun Jun 11 21:23:12 2023, max compression
+gzip compressed data, was "five_card_draw-1.0.4.tar", last modified: Mon Jun 12 14:17:57 2023, max compression
```

## Comparing `five_card_draw-1.0.3.tar` & `five_card_draw-1.0.4.tar`

### file list

```diff
@@ -1,18 +1,77 @@
-drwxrwxrwx   0        0        0        0 2023-06-11 21:23:12.696927 five_card_draw-1.0.3/
--rw-rw-rw-   0        0        0     1085 2023-05-07 02:37:12.000000 five_card_draw-1.0.3/LICENSE.txt
--rw-rw-rw-   0        0        0      653 2023-06-11 21:23:12.697924 five_card_draw-1.0.3/PKG-INFO
--rw-rw-rw-   0        0        0     6556 2023-06-09 00:30:17.000000 five_card_draw-1.0.3/README.md
--rw-rw-rw-   0        0        0      308 2023-06-11 21:23:12.698922 five_card_draw-1.0.3/setup.cfg
--rw-rw-rw-   0        0        0     1861 2023-06-11 21:23:04.000000 five_card_draw-1.0.3/setup.py
-drwxrwxrwx   0        0        0        0 2023-06-11 21:23:12.681994 five_card_draw-1.0.3/src/
-drwxrwxrwx   0        0        0        0 2023-06-11 21:23:12.689946 five_card_draw-1.0.3/src/5_card_draw/
--rw-rw-rw-   0        0        0       89 2023-06-11 21:18:27.000000 five_card_draw-1.0.3/src/5_card_draw/__init__.py
--rw-rw-rw-   0        0        0     9460 2023-06-09 00:26:20.000000 five_card_draw-1.0.3/src/5_card_draw/fcd_functions.py
--rw-rw-rw-   0        0        0    15610 2023-06-10 22:08:20.000000 five_card_draw-1.0.3/src/5_card_draw/fcd_pagegui.py
--rw-rw-rw-   0        0        0      466 2023-06-09 00:21:15.000000 five_card_draw-1.0.3/src/5_card_draw/five_card_draw.py
-drwxrwxrwx   0        0        0        0 2023-06-11 21:23:12.696927 five_card_draw-1.0.3/src/five_card_draw.egg-info/
--rw-rw-rw-   0        0        0      653 2023-06-11 21:23:12.000000 five_card_draw-1.0.3/src/five_card_draw.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      375 2023-06-11 21:23:12.000000 five_card_draw-1.0.3/src/five_card_draw.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-06-11 21:23:12.000000 five_card_draw-1.0.3/src/five_card_draw.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       11 2023-06-11 21:23:12.000000 five_card_draw-1.0.3/src/five_card_draw.egg-info/requires.txt
--rw-rw-rw-   0        0        0       12 2023-06-11 21:23:12.000000 five_card_draw-1.0.3/src/five_card_draw.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-06-12 14:17:57.580869 five_card_draw-1.0.4/
+-rw-rw-rw-   0        0        0     1085 2023-05-07 02:37:12.000000 five_card_draw-1.0.4/LICENSE.txt
+-rw-rw-rw-   0        0        0       55 2023-06-12 13:48:00.000000 five_card_draw-1.0.4/MANIFEST.in
+-rw-rw-rw-   0        0        0     6860 2023-06-12 14:17:57.580869 five_card_draw-1.0.4/PKG-INFO
+-rw-rw-rw-   0        0        0     6556 2023-06-09 00:30:17.000000 five_card_draw-1.0.4/README.md
+drwxrwxrwx   0        0        0        0 2023-06-12 14:17:57.525416 five_card_draw-1.0.4/five_card_draw.egg-info/
+-rw-rw-rw-   0        0        0     6860 2023-06-12 14:17:57.000000 five_card_draw-1.0.4/five_card_draw.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0     2203 2023-06-12 14:17:57.000000 five_card_draw-1.0.4/five_card_draw.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-06-12 14:17:57.000000 five_card_draw-1.0.4/five_card_draw.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       11 2023-06-12 14:17:57.000000 five_card_draw-1.0.4/five_card_draw.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       15 2023-06-12 14:17:57.000000 five_card_draw-1.0.4/five_card_draw.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0      308 2023-06-12 14:17:57.581869 five_card_draw-1.0.4/setup.cfg
+-rw-rw-rw-   0        0        0     1690 2023-06-12 14:17:04.000000 five_card_draw-1.0.4/setup.py
+drwxrwxrwx   0        0        0        0 2023-06-12 14:17:57.514446 five_card_draw-1.0.4/src/
+drwxrwxrwx   0        0        0        0 2023-06-12 14:17:57.528408 five_card_draw-1.0.4/src/five_card_draw/
+-rw-rw-rw-   0        0        0       89 2023-06-11 21:18:27.000000 five_card_draw-1.0.4/src/five_card_draw/__init__.py
+drwxrwxrwx   0        0        0        0 2023-06-12 14:17:57.578969 five_card_draw-1.0.4/src/five_card_draw/data/
+-rw-rw-rw-   0        0        0    56484 2021-10-31 00:37:11.000000 five_card_draw-1.0.4/src/five_card_draw/data/C10.png
+-rw-rw-rw-   0        0        0   187958 2021-10-31 00:37:11.000000 five_card_draw-1.0.4/src/five_card_draw/data/C11.png
+-rw-rw-rw-   0        0        0   205820 2021-10-31 00:37:11.000000 five_card_draw-1.0.4/src/five_card_draw/data/C12.png
+-rw-rw-rw-   0        0        0   189382 2021-10-31 00:37:12.000000 five_card_draw-1.0.4/src/five_card_draw/data/C13.png
+-rw-rw-rw-   0        0        0    37544 2021-10-31 00:37:12.000000 five_card_draw-1.0.4/src/five_card_draw/data/C14.png
+-rw-rw-rw-   0        0        0    23382 2021-10-31 00:37:12.000000 five_card_draw-1.0.4/src/five_card_draw/data/C2.png
+-rw-rw-rw-   0        0        0    29340 2021-10-31 00:37:12.000000 five_card_draw-1.0.4/src/five_card_draw/data/C3.png
+-rw-rw-rw-   0        0        0    29132 2021-10-31 00:37:12.000000 five_card_draw-1.0.4/src/five_card_draw/data/C4.png
+-rw-rw-rw-   0        0        0    35845 2021-10-31 00:37:12.000000 five_card_draw-1.0.4/src/five_card_draw/data/C5.png
+-rw-rw-rw-   0        0        0    40916 2021-10-31 00:37:12.000000 five_card_draw-1.0.4/src/five_card_draw/data/C6.png
+-rw-rw-rw-   0        0        0    41816 2021-10-31 00:37:12.000000 five_card_draw-1.0.4/src/five_card_draw/data/C7.png
+-rw-rw-rw-   0        0        0    48567 2021-10-31 00:37:12.000000 five_card_draw-1.0.4/src/five_card_draw/data/C8.png
+-rw-rw-rw-   0        0        0    52318 2021-10-31 00:37:12.000000 five_card_draw-1.0.4/src/five_card_draw/data/C9.png
+-rw-rw-rw-   0        0        0   432659 2021-11-02 01:23:17.000000 five_card_draw-1.0.4/src/five_card_draw/data/CardBack.png
+-rw-rw-rw-   0        0        0    46699 2021-10-31 00:37:11.000000 five_card_draw-1.0.4/src/five_card_draw/data/D10.png
+-rw-rw-rw-   0        0        0   197802 2021-10-31 00:37:11.000000 five_card_draw-1.0.4/src/five_card_draw/data/D11.png
+-rw-rw-rw-   0        0        0   180712 2021-10-31 00:37:11.000000 five_card_draw-1.0.4/src/five_card_draw/data/D12.png
+-rw-rw-rw-   0        0        0   198565 2021-10-31 00:37:12.000000 five_card_draw-1.0.4/src/five_card_draw/data/D13.png
+-rw-rw-rw-   0        0        0    30901 2021-10-31 00:37:12.000000 five_card_draw-1.0.4/src/five_card_draw/data/D14.png
+-rw-rw-rw-   0        0        0    19170 2021-10-31 00:37:12.000000 five_card_draw-1.0.4/src/five_card_draw/data/D2.png
+-rw-rw-rw-   0        0        0    23815 2021-10-31 00:37:12.000000 five_card_draw-1.0.4/src/five_card_draw/data/D3.png
+-rw-rw-rw-   0        0        0    24296 2021-10-31 00:37:12.000000 five_card_draw-1.0.4/src/five_card_draw/data/D4.png
+-rw-rw-rw-   0        0        0    29806 2021-10-31 00:37:12.000000 five_card_draw-1.0.4/src/five_card_draw/data/D5.png
+-rw-rw-rw-   0        0        0    33800 2021-10-31 00:37:12.000000 five_card_draw-1.0.4/src/five_card_draw/data/D6.png
+-rw-rw-rw-   0        0        0    34176 2021-10-31 00:37:12.000000 five_card_draw-1.0.4/src/five_card_draw/data/D7.png
+-rw-rw-rw-   0        0        0    40724 2021-10-31 00:37:12.000000 five_card_draw-1.0.4/src/five_card_draw/data/D8.png
+-rw-rw-rw-   0        0        0    43365 2021-10-31 00:37:13.000000 five_card_draw-1.0.4/src/five_card_draw/data/D9.png
+-rw-rw-rw-   0        0        0    49317 2021-10-31 00:37:11.000000 five_card_draw-1.0.4/src/five_card_draw/data/H10.png
+-rw-rw-rw-   0        0        0   203728 2021-10-31 00:37:11.000000 five_card_draw-1.0.4/src/five_card_draw/data/H11.png
+-rw-rw-rw-   0        0        0   197792 2021-10-31 00:37:11.000000 five_card_draw-1.0.4/src/five_card_draw/data/H12.png
+-rw-rw-rw-   0        0        0   207052 2021-10-31 00:37:12.000000 five_card_draw-1.0.4/src/five_card_draw/data/H13.png
+-rw-rw-rw-   0        0        0    36444 2021-10-31 00:37:12.000000 five_card_draw-1.0.4/src/five_card_draw/data/H14.png
+-rw-rw-rw-   0        0        0    20058 2021-10-31 00:37:12.000000 five_card_draw-1.0.4/src/five_card_draw/data/H2.png
+-rw-rw-rw-   0        0        0    24919 2021-10-31 00:37:12.000000 five_card_draw-1.0.4/src/five_card_draw/data/H3.png
+-rw-rw-rw-   0        0        0    25320 2021-10-31 00:37:12.000000 five_card_draw-1.0.4/src/five_card_draw/data/H4.png
+-rw-rw-rw-   0        0        0    31082 2021-10-31 00:37:12.000000 five_card_draw-1.0.4/src/five_card_draw/data/H5.png
+-rw-rw-rw-   0        0        0    35239 2021-10-31 00:37:12.000000 five_card_draw-1.0.4/src/five_card_draw/data/H6.png
+-rw-rw-rw-   0        0        0    35904 2021-10-31 00:37:12.000000 five_card_draw-1.0.4/src/five_card_draw/data/H7.png
+-rw-rw-rw-   0        0        0    42890 2021-10-31 00:37:12.000000 five_card_draw-1.0.4/src/five_card_draw/data/H8.png
+-rw-rw-rw-   0        0        0    45669 2021-10-31 00:37:13.000000 five_card_draw-1.0.4/src/five_card_draw/data/H9.png
+-rw-rw-rw-   0        0        0    50853 2021-10-31 00:37:11.000000 five_card_draw-1.0.4/src/five_card_draw/data/S10.png
+-rw-rw-rw-   0        0        0   190953 2021-10-31 00:37:11.000000 five_card_draw-1.0.4/src/five_card_draw/data/S11.png
+-rw-rw-rw-   0        0        0   186480 2021-10-31 00:37:12.000000 five_card_draw-1.0.4/src/five_card_draw/data/S12.png
+-rw-rw-rw-   0        0        0   183329 2021-10-31 00:37:12.000000 five_card_draw-1.0.4/src/five_card_draw/data/S13.png
+-rw-rw-rw-   0        0        0    56051 2021-10-31 00:37:12.000000 five_card_draw-1.0.4/src/five_card_draw/data/S14.png
+-rw-rw-rw-   0        0        0    21104 2021-10-31 00:37:12.000000 five_card_draw-1.0.4/src/five_card_draw/data/S2.png
+-rw-rw-rw-   0        0        0    26211 2021-10-31 00:37:12.000000 five_card_draw-1.0.4/src/five_card_draw/data/S3.png
+-rw-rw-rw-   0        0        0    26311 2021-10-31 00:37:12.000000 five_card_draw-1.0.4/src/five_card_draw/data/S4.png
+-rw-rw-rw-   0        0        0    32110 2021-10-31 00:37:12.000000 five_card_draw-1.0.4/src/five_card_draw/data/S5.png
+-rw-rw-rw-   0        0        0    36726 2021-10-31 00:37:12.000000 five_card_draw-1.0.4/src/five_card_draw/data/S6.png
+-rw-rw-rw-   0        0        0    37510 2021-10-31 00:37:12.000000 five_card_draw-1.0.4/src/five_card_draw/data/S7.png
+-rw-rw-rw-   0        0        0    43823 2021-10-31 00:37:12.000000 five_card_draw-1.0.4/src/five_card_draw/data/S8.png
+-rw-rw-rw-   0        0        0    46996 2021-10-31 00:37:13.000000 five_card_draw-1.0.4/src/five_card_draw/data/S9.png
+-rw-rw-rw-   0        0        0   560393 2023-06-08 17:03:00.000000 five_card_draw-1.0.4/src/five_card_draw/data/ScoringImage.png
+-rw-rw-rw-   0        0        0       89 2023-06-11 21:18:27.000000 five_card_draw-1.0.4/src/five_card_draw/data/__init__.py
+-rw-rw-rw-   0        0        0    43719 2021-10-31 00:37:13.000000 five_card_draw-1.0.4/src/five_card_draw/data/black_joker.png
+-rw-rw-rw-   0        0        0    44079 2021-10-31 00:37:13.000000 five_card_draw-1.0.4/src/five_card_draw/data/red_joker.png
+-rw-rw-rw-   0        0        0     9460 2023-06-09 00:26:20.000000 five_card_draw-1.0.4/src/five_card_draw/fcd_functions.py
+-rw-rw-rw-   0        0        0    15610 2023-06-10 22:08:20.000000 five_card_draw-1.0.4/src/five_card_draw/fcd_pagegui.py
+-rw-rw-rw-   0        0        0      466 2023-06-09 00:21:15.000000 five_card_draw-1.0.4/src/five_card_draw/five_card_draw.py
```

### Comparing `five_card_draw-1.0.3/LICENSE.txt` & `five_card_draw-1.0.4/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `five_card_draw-1.0.3/README.md` & `five_card_draw-1.0.4/README.md`

 * *Files identical despite different names*

### Comparing `five_card_draw-1.0.3/src/5_card_draw/fcd_functions.py` & `five_card_draw-1.0.4/src/five_card_draw/fcd_functions.py`

 * *Files identical despite different names*

### Comparing `five_card_draw-1.0.3/src/5_card_draw/fcd_pagegui.py` & `five_card_draw-1.0.4/src/five_card_draw/fcd_pagegui.py`

 * *Files identical despite different names*

