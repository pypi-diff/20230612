# Comparing `tmp/pm20_3-0.3.tar.gz` & `tmp/pm20_3-0.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pm20_3-0.3.tar", last modified: Mon Jun 12 18:39:12 2023, max compression
+gzip compressed data, was "pm20_3-0.4.tar", last modified: Mon Jun 12 18:43:24 2023, max compression
```

## Comparing `pm20_3-0.3.tar` & `pm20_3-0.4.tar`

### file list

```diff
@@ -1,7 +1,130 @@
-drwxrwxrwx   0        0        0        0 2023-06-12 18:39:12.623762 pm20_3-0.3/
--rw-rw-rw-   0        0        0      993 2023-06-12 18:39:12.624735 pm20_3-0.3/PKG-INFO
-drwxrwxrwx   0        0        0        0 2023-06-12 18:39:12.623762 pm20_3-0.3/pm20_3/
--rw-rw-rw-   0        0        0       37 2023-06-12 16:30:23.669995 pm20_3-0.3/pm20_3/__init__.py
--rw-rw-rw-   0        0        0     1647 2023-06-12 18:30:45.253599 pm20_3-0.3/pm20_3/questions.py
--rw-rw-rw-   0        0        0       63 2023-06-12 17:51:03.693651 pm20_3-0.3/setup.cfg
--rw-rw-rw-   0        0        0     1914 2023-06-12 18:38:19.837998 pm20_3-0.3/setup.py
+drwxrwxrwx   0        0        0        0 2023-06-12 18:43:24.231475 pm20_3-0.4/
+-rw-rw-rw-   0        0        0      993 2023-06-12 18:43:24.232473 pm20_3-0.4/PKG-INFO
+drwxrwxrwx   0        0        0        0 2023-06-12 18:43:24.110980 pm20_3-0.4/pm20_3/
+-rw-rw-rw-   0        0        0       37 2023-06-12 16:30:23.669995 pm20_3-0.4/pm20_3/__init__.py
+drwxrwxrwx   0        0        0        0 2023-06-12 18:43:24.113009 pm20_3-0.4/pm20_3/__pycache__/
+-rw-rw-rw-   0        0        0      174 2023-06-12 16:52:57.741706 pm20_3-0.4/pm20_3/__pycache__/__init__.cpython-39.pyc
+-rw-rw-rw-   0        0        0      989 2023-06-12 16:52:56.543340 pm20_3-0.4/pm20_3/__pycache__/questions.cpython-39.pyc
+drwxrwxrwx   0        0        0        0 2023-06-12 18:43:24.231475 pm20_3-0.4/pm20_3/q/
+-rw-rw-rw-   0        0        0    22332 2023-06-11 23:36:53.000000 pm20_3-0.4/pm20_3/q/1.png
+-rw-rw-rw-   0        0        0    13076 2023-06-12 14:12:00.000000 pm20_3-0.4/pm20_3/q/100_1.png
+-rw-rw-rw-   0        0        0    19820 2023-06-12 14:12:00.000000 pm20_3-0.4/pm20_3/q/100_2.png
+-rw-rw-rw-   0        0        0    35413 2023-06-12 17:24:14.000000 pm20_3-0.4/pm20_3/q/101.png
+-rw-rw-rw-   0        0        0    31641 2023-06-12 17:24:14.000000 pm20_3-0.4/pm20_3/q/102_1.png
+-rw-rw-rw-   0        0        0    43027 2023-06-12 17:24:14.000000 pm20_3-0.4/pm20_3/q/102_2.png
+-rw-rw-rw-   0        0        0    22381 2023-06-12 17:24:15.000000 pm20_3-0.4/pm20_3/q/103.png
+-rw-rw-rw-   0        0        0    18175 2023-06-12 17:24:15.000000 pm20_3-0.4/pm20_3/q/104.png
+-rw-rw-rw-   0        0        0    17204 2023-06-12 17:24:15.000000 pm20_3-0.4/pm20_3/q/105.png
+-rw-rw-rw-   0        0        0    21939 2023-06-12 17:24:15.000000 pm20_3-0.4/pm20_3/q/106.png
+-rw-rw-rw-   0        0        0    22657 2023-06-12 17:24:15.000000 pm20_3-0.4/pm20_3/q/107.png
+-rw-rw-rw-   0        0        0    20422 2023-06-12 17:24:15.000000 pm20_3-0.4/pm20_3/q/108.png
+-rw-rw-rw-   0        0        0    19033 2023-06-12 17:24:15.000000 pm20_3-0.4/pm20_3/q/109_1.png
+-rw-rw-rw-   0        0        0    10710 2023-06-12 17:24:15.000000 pm20_3-0.4/pm20_3/q/109_2.png
+-rw-rw-rw-   0        0        0    24896 2023-06-12 10:14:10.000000 pm20_3-0.4/pm20_3/q/10_1.png
+-rw-rw-rw-   0        0        0    11980 2023-06-12 10:14:10.000000 pm20_3-0.4/pm20_3/q/10_2.png
+-rw-rw-rw-   0        0        0    25238 2023-06-12 10:14:10.000000 pm20_3-0.4/pm20_3/q/11_1.png
+-rw-rw-rw-   0        0        0    11242 2023-06-12 10:14:10.000000 pm20_3-0.4/pm20_3/q/11_2.png
+-rw-rw-rw-   0        0        0    25827 2023-06-12 10:14:10.000000 pm20_3-0.4/pm20_3/q/12_1.png
+-rw-rw-rw-   0        0        0    15607 2023-06-12 10:14:10.000000 pm20_3-0.4/pm20_3/q/12_2.png
+-rw-rw-rw-   0        0        0    23559 2023-06-12 10:14:10.000000 pm20_3-0.4/pm20_3/q/13_1.png
+-rw-rw-rw-   0        0        0    12135 2023-06-12 10:14:10.000000 pm20_3-0.4/pm20_3/q/13_2.png
+-rw-rw-rw-   0        0        0    17871 2023-06-12 10:32:37.000000 pm20_3-0.4/pm20_3/q/14.png
+-rw-rw-rw-   0        0        0    47983 2023-06-12 10:32:37.000000 pm20_3-0.4/pm20_3/q/15.png
+-rw-rw-rw-   0        0        0    14560 2023-06-12 10:32:37.000000 pm20_3-0.4/pm20_3/q/16.png
+-rw-rw-rw-   0        0        0    30806 2023-06-12 10:32:37.000000 pm20_3-0.4/pm20_3/q/17.png
+-rw-rw-rw-   0        0        0    25570 2023-06-12 10:32:37.000000 pm20_3-0.4/pm20_3/q/18.png
+-rw-rw-rw-   0        0        0    18952 2023-06-12 10:32:37.000000 pm20_3-0.4/pm20_3/q/19.png
+-rw-rw-rw-   0        0        0    36031 2023-06-11 23:36:53.000000 pm20_3-0.4/pm20_3/q/2.png
+-rw-rw-rw-   0        0        0    18386 2023-06-12 10:32:38.000000 pm20_3-0.4/pm20_3/q/20.png
+-rw-rw-rw-   0        0        0    13506 2023-06-12 10:32:38.000000 pm20_3-0.4/pm20_3/q/21.png
+-rw-rw-rw-   0        0        0    17480 2023-06-12 10:32:38.000000 pm20_3-0.4/pm20_3/q/22.png
+-rw-rw-rw-   0        0        0    20865 2023-06-12 10:32:38.000000 pm20_3-0.4/pm20_3/q/23.png
+-rw-rw-rw-   0        0        0    16150 2023-06-12 16:24:49.000000 pm20_3-0.4/pm20_3/q/24.png
+-rw-rw-rw-   0        0        0    17873 2023-06-12 16:24:49.000000 pm20_3-0.4/pm20_3/q/25.png
+-rw-rw-rw-   0        0        0    17632 2023-06-12 16:24:49.000000 pm20_3-0.4/pm20_3/q/26.png
+-rw-rw-rw-   0        0        0    24749 2023-06-12 16:24:49.000000 pm20_3-0.4/pm20_3/q/27.png
+-rw-rw-rw-   0        0        0    30463 2023-06-12 16:24:49.000000 pm20_3-0.4/pm20_3/q/28_1.png
+-rw-rw-rw-   0        0        0    26196 2023-06-12 16:24:49.000000 pm20_3-0.4/pm20_3/q/28_2.png
+-rw-rw-rw-   0        0        0     7463 2023-06-12 16:24:49.000000 pm20_3-0.4/pm20_3/q/28_3.png
+-rw-rw-rw-   0        0        0    24175 2023-06-12 16:24:50.000000 pm20_3-0.4/pm20_3/q/29.png
+-rw-rw-rw-   0        0        0    14997 2023-06-12 16:24:50.000000 pm20_3-0.4/pm20_3/q/30.png
+-rw-rw-rw-   0        0        0    32838 2023-06-12 16:24:50.000000 pm20_3-0.4/pm20_3/q/31.png
+-rw-rw-rw-   0        0        0    31497 2023-06-12 17:07:45.000000 pm20_3-0.4/pm20_3/q/32.png
+-rw-rw-rw-   0        0        0    36121 2023-06-12 17:07:45.000000 pm20_3-0.4/pm20_3/q/33.png
+-rw-rw-rw-   0        0        0    24766 2023-06-12 17:07:45.000000 pm20_3-0.4/pm20_3/q/34.png
+-rw-rw-rw-   0        0        0    24693 2023-06-12 17:07:45.000000 pm20_3-0.4/pm20_3/q/35.png
+-rw-rw-rw-   0        0        0    17212 2023-06-12 17:07:45.000000 pm20_3-0.4/pm20_3/q/36.png
+-rw-rw-rw-   0        0        0    14414 2023-06-12 17:07:45.000000 pm20_3-0.4/pm20_3/q/37.png
+-rw-rw-rw-   0        0        0    28049 2023-06-12 17:07:45.000000 pm20_3-0.4/pm20_3/q/38.png
+-rw-rw-rw-   0        0        0    22897 2023-06-12 17:07:45.000000 pm20_3-0.4/pm20_3/q/39.png
+-rw-rw-rw-   0        0        0    22808 2023-06-11 23:36:53.000000 pm20_3-0.4/pm20_3/q/3_1.png
+-rw-rw-rw-   0        0        0    18430 2023-06-11 23:36:53.000000 pm20_3-0.4/pm20_3/q/3_2.png
+-rw-rw-rw-   0        0        0    17794 2023-06-12 17:07:45.000000 pm20_3-0.4/pm20_3/q/40.png
+-rw-rw-rw-   0        0        0    22946 2023-06-12 14:09:12.000000 pm20_3-0.4/pm20_3/q/41.png
+-rw-rw-rw-   0        0        0     5229 2023-06-12 14:09:13.000000 pm20_3-0.4/pm20_3/q/42.png
+-rw-rw-rw-   0        0        0    14311 2023-06-12 14:09:13.000000 pm20_3-0.4/pm20_3/q/44.png
+-rw-rw-rw-   0        0        0    17569 2023-06-12 14:09:13.000000 pm20_3-0.4/pm20_3/q/45_1.png
+-rw-rw-rw-   0        0        0    11219 2023-06-12 14:09:13.000000 pm20_3-0.4/pm20_3/q/45_2.png
+-rw-rw-rw-   0        0        0    13042 2023-06-12 14:09:13.000000 pm20_3-0.4/pm20_3/q/47.png
+-rw-rw-rw-   0        0        0    23492 2023-06-12 14:09:13.000000 pm20_3-0.4/pm20_3/q/48.png
+-rw-rw-rw-   0        0        0    14396 2023-06-12 14:09:13.000000 pm20_3-0.4/pm20_3/q/49.png
+-rw-rw-rw-   0        0        0    22250 2023-06-11 23:36:53.000000 pm20_3-0.4/pm20_3/q/4_1.png
+-rw-rw-rw-   0        0        0     9394 2023-06-11 23:36:53.000000 pm20_3-0.4/pm20_3/q/4_2.png
+-rw-rw-rw-   0        0        0     9631 2023-06-12 14:09:13.000000 pm20_3-0.4/pm20_3/q/50.png
+-rw-rw-rw-   0        0        0    21267 2023-06-12 14:09:13.000000 pm20_3-0.4/pm20_3/q/51.png
+-rw-rw-rw-   0        0        0    24781 2023-06-12 14:10:27.000000 pm20_3-0.4/pm20_3/q/52.png
+-rw-rw-rw-   0        0        0    15292 2023-06-12 14:10:27.000000 pm20_3-0.4/pm20_3/q/53.png
+-rw-rw-rw-   0        0        0    15971 2023-06-12 14:10:27.000000 pm20_3-0.4/pm20_3/q/54.png
+-rw-rw-rw-   0        0        0    12039 2023-06-12 14:10:27.000000 pm20_3-0.4/pm20_3/q/55.png
+-rw-rw-rw-   0        0        0     6877 2023-06-12 14:10:27.000000 pm20_3-0.4/pm20_3/q/56.png
+-rw-rw-rw-   0        0        0     8127 2023-06-12 14:10:27.000000 pm20_3-0.4/pm20_3/q/57.png
+-rw-rw-rw-   0        0        0    16492 2023-06-12 14:10:27.000000 pm20_3-0.4/pm20_3/q/58.png
+-rw-rw-rw-   0        0        0    15539 2023-06-12 14:10:27.000000 pm20_3-0.4/pm20_3/q/59.png
+-rw-rw-rw-   0        0        0    39623 2023-06-11 23:36:53.000000 pm20_3-0.4/pm20_3/q/5_1.png
+-rw-rw-rw-   0        0        0    21741 2023-06-11 23:36:53.000000 pm20_3-0.4/pm20_3/q/5_2.png
+-rw-rw-rw-   0        0        0    35512 2023-06-11 23:36:53.000000 pm20_3-0.4/pm20_3/q/6.png
+-rw-rw-rw-   0        0        0    16512 2023-06-12 14:10:27.000000 pm20_3-0.4/pm20_3/q/60.png
+-rw-rw-rw-   0        0        0    24946 2023-06-12 09:47:25.000000 pm20_3-0.4/pm20_3/q/61.png
+-rw-rw-rw-   0        0        0    12308 2023-06-12 09:47:25.000000 pm20_3-0.4/pm20_3/q/62.png
+-rw-rw-rw-   0        0        0    14477 2023-06-12 09:47:25.000000 pm20_3-0.4/pm20_3/q/63.png
+-rw-rw-rw-   0        0        0    29479 2023-06-12 09:47:25.000000 pm20_3-0.4/pm20_3/q/64_1.png
+-rw-rw-rw-   0        0        0     7143 2023-06-12 09:47:25.000000 pm20_3-0.4/pm20_3/q/64_2.png
+-rw-rw-rw-   0        0        0    20260 2023-06-12 09:47:26.000000 pm20_3-0.4/pm20_3/q/65.png
+-rw-rw-rw-   0        0        0    24172 2023-06-12 09:47:26.000000 pm20_3-0.4/pm20_3/q/66.png
+-rw-rw-rw-   0        0        0    25316 2023-06-12 09:47:26.000000 pm20_3-0.4/pm20_3/q/67.png
+-rw-rw-rw-   0        0        0    24259 2023-06-12 09:47:26.000000 pm20_3-0.4/pm20_3/q/68.png
+-rw-rw-rw-   0        0        0    24844 2023-06-12 09:47:26.000000 pm20_3-0.4/pm20_3/q/69.png
+-rw-rw-rw-   0        0        0    29634 2023-06-11 23:36:53.000000 pm20_3-0.4/pm20_3/q/7.png
+-rw-rw-rw-   0        0        0    22730 2023-06-12 09:58:57.000000 pm20_3-0.4/pm20_3/q/70.png
+-rw-rw-rw-   0        0        0    20214 2023-06-12 09:58:57.000000 pm20_3-0.4/pm20_3/q/71.png
+-rw-rw-rw-   0        0        0    20354 2023-06-12 09:58:57.000000 pm20_3-0.4/pm20_3/q/72.png
+-rw-rw-rw-   0        0        0    20613 2023-06-12 09:58:57.000000 pm20_3-0.4/pm20_3/q/73.png
+-rw-rw-rw-   0        0        0    19630 2023-06-12 09:58:57.000000 pm20_3-0.4/pm20_3/q/74.png
+-rw-rw-rw-   0        0        0    19406 2023-06-12 09:58:57.000000 pm20_3-0.4/pm20_3/q/75.png
+-rw-rw-rw-   0        0        0    19924 2023-06-12 09:58:57.000000 pm20_3-0.4/pm20_3/q/76.png
+-rw-rw-rw-   0        0        0    22668 2023-06-12 09:58:57.000000 pm20_3-0.4/pm20_3/q/77.png
+-rw-rw-rw-   0        0        0    27086 2023-06-12 09:58:57.000000 pm20_3-0.4/pm20_3/q/78_1.png
+-rw-rw-rw-   0        0        0    20610 2023-06-12 09:58:57.000000 pm20_3-0.4/pm20_3/q/78_2.png
+-rw-rw-rw-   0        0        0    41510 2023-06-12 10:14:10.000000 pm20_3-0.4/pm20_3/q/8.png
+-rw-rw-rw-   0        0        0    24624 2023-06-12 10:14:10.000000 pm20_3-0.4/pm20_3/q/9.png
+-rw-rw-rw-   0        0        0    22857 2023-06-12 14:11:23.000000 pm20_3-0.4/pm20_3/q/91_1.png
+-rw-rw-rw-   0        0        0    14390 2023-06-12 14:11:23.000000 pm20_3-0.4/pm20_3/q/91_2.png
+-rw-rw-rw-   0        0        0    39595 2023-06-12 14:11:23.000000 pm20_3-0.4/pm20_3/q/92.png
+-rw-rw-rw-   0        0        0    12829 2023-06-12 14:11:23.000000 pm20_3-0.4/pm20_3/q/93.png
+-rw-rw-rw-   0        0        0    17694 2023-06-12 14:11:23.000000 pm20_3-0.4/pm20_3/q/94.png
+-rw-rw-rw-   0        0        0    25458 2023-06-12 14:11:23.000000 pm20_3-0.4/pm20_3/q/95.png
+-rw-rw-rw-   0        0        0    19844 2023-06-12 14:11:23.000000 pm20_3-0.4/pm20_3/q/96_1.png
+-rw-rw-rw-   0        0        0    11215 2023-06-12 14:11:23.000000 pm20_3-0.4/pm20_3/q/96_2.png
+-rw-rw-rw-   0        0        0    15567 2023-06-12 14:11:23.000000 pm20_3-0.4/pm20_3/q/97.png
+-rw-rw-rw-   0        0        0    16770 2023-06-12 14:11:23.000000 pm20_3-0.4/pm20_3/q/98.png
+-rw-rw-rw-   0        0        0    15343 2023-06-12 14:12:00.000000 pm20_3-0.4/pm20_3/q/99.png
+-rw-rw-rw-   0        0        0        0 2023-06-12 16:59:25.432042 pm20_3-0.4/pm20_3/q/__init__.py
+-rw-rw-rw-   0        0        0    24796 2023-06-11 23:13:18.000000 pm20_3-0.4/pm20_3/q/task_1.png
+-rw-rw-rw-   0        0        0    26421 2023-06-11 23:13:18.000000 pm20_3-0.4/pm20_3/q/task_2.png
+-rw-rw-rw-   0        0        0    25932 2023-06-11 23:13:18.000000 pm20_3-0.4/pm20_3/q/task_3.png
+-rw-rw-rw-   0        0        0    25398 2023-06-11 23:13:18.000000 pm20_3-0.4/pm20_3/q/task_4.png
+-rw-rw-rw-   0        0        0    26943 2023-06-11 23:13:18.000000 pm20_3-0.4/pm20_3/q/task_5.png
+-rw-rw-rw-   0        0        0    10322 2023-06-11 23:13:18.000000 pm20_3-0.4/pm20_3/q/task_6.png
+-rw-rw-rw-   0        0        0     1651 2023-06-12 18:40:37.675172 pm20_3-0.4/pm20_3/questions.py
+-rw-rw-rw-   0        0        0       63 2023-06-12 17:51:03.693651 pm20_3-0.4/setup.cfg
+-rw-rw-rw-   0        0        0     1914 2023-06-12 18:43:23.902943 pm20_3-0.4/setup.py
```

### Comparing `pm20_3-0.3/PKG-INFO` & `pm20_3-0.4/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.1
 Name: pm20_3
-Version: 0.3
+Version: 0.4
 Summary: For cheating again..
 Home-page: http://www.fa.ru/Pages/Home.aspx
 Author: Anatoliy Nesterov
 Author-email: your.email@domain.com
 License: MIT
 Download-URL: https://github.com/user/reponame/archive/v_01.tar.gz
 Description: UNKNOWN
```

### Comparing `pm20_3-0.3/pm20_3/questions.py` & `pm20_3-0.4/pm20_3/questions.py`

 * *Files 0% similar despite different names*

```diff
@@ -62,7 +62,9 @@
             with path(
                     'pm20_3.q',
                     elem
             ) as pt:
                 img = Image(filename=pt)
                 display(img)
 
+
+
```

### Comparing `pm20_3-0.3/setup.py` & `pm20_3-0.4/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 from distutils.core import setup
 
 setup(
     name='pm20_3',  # How you named your package folder (MyLib)
     packages=['pm20_3'],  # Chose the same as "name"
-    version='0.3',  # Start with a small number and increase it with every change you make
+    version='0.4',  # Start with a small number and increase it with every change you make
     license='MIT',  # Chose a license from here: https://help.github.com/articles/licensing-a-repository
     description='For cheating again..',  # Give a short description about your library
     author='Anatoliy Nesterov',  # Type in your name
     author_email='your.email@domain.com',  # Type in your E-Mail
     url='http://www.fa.ru/Pages/Home.aspx',  # Provide either the link to your github or to your website
     download_url='https://github.com/user/reponame/archive/v_01.tar.gz',  # I explain this later on
     keywords=['CHEATING'],  # Keywords that define your package best
```

