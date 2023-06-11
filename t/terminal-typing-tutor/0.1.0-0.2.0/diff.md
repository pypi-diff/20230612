# Comparing `tmp/terminal_typing_tutor-0.1.0.tar.gz` & `tmp/terminal_typing_tutor-0.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "terminal_typing_tutor-0.1.0.tar", max compression
+gzip compressed data, was "terminal_typing_tutor-0.2.0.tar", max compression
```

## Comparing `terminal_typing_tutor-0.1.0.tar` & `terminal_typing_tutor-0.2.0.tar`

### file list

```diff
@@ -1,119 +1,120 @@
--rw-r--r--   0        0        0     1071 2023-06-11 03:21:24.159766 terminal_typing_tutor-0.1.0/LICENSE
--rw-r--r--   0        0        0     1514 2023-06-11 04:37:37.319671 terminal_typing_tutor-0.1.0/README.md
--rw-r--r--   0        0        0      562 2023-06-11 04:13:04.467701 terminal_typing_tutor-0.1.0/pyproject.toml
--rw-r--r--   0        0        0        0 2023-06-11 03:16:41.451772 terminal_typing_tutor-0.1.0/terminal_typing_tutor/__init__.py
--rw-r--r--   0        0        0       31 2023-06-11 04:25:58.607685 terminal_typing_tutor-0.1.0/terminal_typing_tutor/__main__.py
--rw-r--r--   0        0        0     1517 2023-06-11 03:22:35.767764 terminal_typing_tutor-0.1.0/terminal_typing_tutor/constants.py
--rwxr-xr-x   0        0        0      201 2023-06-11 04:11:52.927703 terminal_typing_tutor-0.1.0/terminal_typing_tutor/main.py
--rw-r--r--   0        0        0     3364 2023-06-11 03:21:12.331766 terminal_typing_tutor-0.1.0/terminal_typing_tutor/series/M/1/data.yaml
--rw-r--r--   0        0        0     3377 2023-06-11 03:21:12.331766 terminal_typing_tutor-0.1.0/terminal_typing_tutor/series/M/10/data.yaml
--rw-r--r--   0        0        0     4191 2023-06-11 03:21:12.331766 terminal_typing_tutor-0.1.0/terminal_typing_tutor/series/M/11/data.yaml
--rw-r--r--   0        0        0     2861 2023-06-11 03:21:12.331766 terminal_typing_tutor-0.1.0/terminal_typing_tutor/series/M/2/data.yaml
--rw-r--r--   0        0        0     3201 2023-06-11 03:21:12.331766 terminal_typing_tutor-0.1.0/terminal_typing_tutor/series/M/3/data.yaml
--rw-r--r--   0        0        0     2680 2023-06-11 03:21:12.331766 terminal_typing_tutor-0.1.0/terminal_typing_tutor/series/M/4/data.yaml
--rw-r--r--   0        0        0     3175 2023-06-11 03:21:12.331766 terminal_typing_tutor-0.1.0/terminal_typing_tutor/series/M/5/data.yaml
--rw-r--r--   0        0        0     3017 2023-06-11 03:21:12.331766 terminal_typing_tutor-0.1.0/terminal_typing_tutor/series/M/6/data.yaml
--rw-r--r--   0        0        0     2591 2023-06-11 03:21:12.331766 terminal_typing_tutor-0.1.0/terminal_typing_tutor/series/M/7/data.yaml
--rw-r--r--   0        0        0     3028 2023-06-11 03:21:12.331766 terminal_typing_tutor-0.1.0/terminal_typing_tutor/series/M/8/data.yaml
--rw-r--r--   0        0        0     3861 2023-06-11 03:21:12.331766 terminal_typing_tutor-0.1.0/terminal_typing_tutor/series/M/9/data.yaml
--rw-r--r--   0        0        0        3 2023-06-11 03:21:12.331766 terminal_typing_tutor-0.1.0/terminal_typing_tutor/series/M/lesson_count
--rw-r--r--   0        0        0    36212 2023-06-11 03:21:12.331766 terminal_typing_tutor-0.1.0/terminal_typing_tutor/series/M/m.typ
--rw-r--r--   0        0        0      520 2023-06-11 03:21:12.331766 terminal_typing_tutor-0.1.0/terminal_typing_tutor/series/M/menu.json
--rw-r--r--   0        0        0       14 2023-06-11 03:21:12.331766 terminal_typing_tutor-0.1.0/terminal_typing_tutor/series/M/title
--rw-r--r--   0        0        0     5885 2023-06-11 03:21:12.331766 terminal_typing_tutor-0.1.0/terminal_typing_tutor/series/Q/1/data.yaml
--rw-r--r--   0        0        0     2445 2023-06-11 03:21:12.331766 terminal_typing_tutor-0.1.0/terminal_typing_tutor/series/Q/2/data.yaml
--rw-r--r--   0        0        0     3099 2023-06-11 03:21:12.331766 terminal_typing_tutor-0.1.0/terminal_typing_tutor/series/Q/3/data.yaml
--rw-r--r--   0        0        0     3034 2023-06-11 03:21:12.335766 terminal_typing_tutor-0.1.0/terminal_typing_tutor/series/Q/4/data.yaml
--rw-r--r--   0        0        0     2004 2023-06-11 03:21:12.335766 terminal_typing_tutor-0.1.0/terminal_typing_tutor/series/Q/5/data.yaml
--rw-r--r--   0        0        0        2 2023-06-11 03:21:12.331766 terminal_typing_tutor-0.1.0/terminal_typing_tutor/series/Q/lesson_count
--rw-r--r--   0        0        0      293 2023-06-11 03:21:12.331766 terminal_typing_tutor-0.1.0/terminal_typing_tutor/series/Q/menu.json
--rw-r--r--   0        0        0    16803 2023-06-11 03:21:12.331766 terminal_typing_tutor-0.1.0/terminal_typing_tutor/series/Q/q.typ
--rw-r--r--   0        0        0       20 2023-06-11 03:21:12.331766 terminal_typing_tutor-0.1.0/terminal_typing_tutor/series/Q/title
--rw-r--r--   0        0        0     2650 2023-06-11 03:21:12.335766 terminal_typing_tutor-0.1.0/terminal_typing_tutor/series/R/1/data.yaml
--rw-r--r--   0        0        0     3389 2023-06-11 03:21:12.335766 terminal_typing_tutor-0.1.0/terminal_typing_tutor/series/R/10/data.yaml
--rw-r--r--   0        0        0     2608 2023-06-11 03:21:12.335766 terminal_typing_tutor-0.1.0/terminal_typing_tutor/series/R/11/data.yaml
--rw-r--r--   0        0        0     2975 2023-06-11 03:21:12.335766 terminal_typing_tutor-0.1.0/terminal_typing_tutor/series/R/12/data.yaml
--rw-r--r--   0        0        0     2659 2023-06-11 03:21:12.335766 terminal_typing_tutor-0.1.0/terminal_typing_tutor/series/R/13/data.yaml
--rw-r--r--   0        0        0     3307 2023-06-11 03:21:12.335766 terminal_typing_tutor-0.1.0/terminal_typing_tutor/series/R/14/data.yaml
--rw-r--r--   0        0        0     2721 2023-06-11 03:21:12.335766 terminal_typing_tutor-0.1.0/terminal_typing_tutor/series/R/2/data.yaml
--rw-r--r--   0        0        0     3181 2023-06-11 03:21:12.335766 terminal_typing_tutor-0.1.0/terminal_typing_tutor/series/R/3/data.yaml
--rw-r--r--   0        0        0     2764 2023-06-11 03:21:12.335766 terminal_typing_tutor-0.1.0/terminal_typing_tutor/series/R/4/data.yaml
--rw-r--r--   0        0        0     3166 2023-06-11 03:21:12.335766 terminal_typing_tutor-0.1.0/terminal_typing_tutor/series/R/5/data.yaml
--rw-r--r--   0        0        0     2920 2023-06-11 03:21:12.335766 terminal_typing_tutor-0.1.0/terminal_typing_tutor/series/R/6/data.yaml
--rw-r--r--   0        0        0     2852 2023-06-11 03:21:12.335766 terminal_typing_tutor-0.1.0/terminal_typing_tutor/series/R/7/data.yaml
--rw-r--r--   0        0        0     3119 2023-06-11 03:21:12.335766 terminal_typing_tutor-0.1.0/terminal_typing_tutor/series/R/8/data.yaml
--rw-r--r--   0        0        0     3491 2023-06-11 03:21:12.335766 terminal_typing_tutor-0.1.0/terminal_typing_tutor/series/R/9/data.yaml
--rw-r--r--   0        0        0        3 2023-06-11 03:21:12.335766 terminal_typing_tutor-0.1.0/terminal_typing_tutor/series/R/lesson_count
--rw-r--r--   0        0        0      672 2023-06-11 03:21:12.335766 terminal_typing_tutor-0.1.0/terminal_typing_tutor/series/R/menu.json
--rw-r--r--   0        0        0    41316 2023-06-11 03:21:12.335766 terminal_typing_tutor-0.1.0/terminal_typing_tutor/series/R/r.typ
--rw-r--r--   0        0        0       19 2023-06-11 03:21:12.335766 terminal_typing_tutor-0.1.0/terminal_typing_tutor/series/R/title
--rw-r--r--   0        0        0     2762 2023-06-11 03:21:12.335766 terminal_typing_tutor-0.1.0/terminal_typing_tutor/series/S/1/data.yaml
--rw-r--r--   0        0        0     3364 2023-06-11 03:21:12.335766 terminal_typing_tutor-0.1.0/terminal_typing_tutor/series/S/2/data.yaml
--rw-r--r--   0        0        0     4005 2023-06-11 03:21:12.335766 terminal_typing_tutor-0.1.0/terminal_typing_tutor/series/S/3/data.yaml
--rw-r--r--   0        0        0     6793 2023-06-11 03:21:12.335766 terminal_typing_tutor-0.1.0/terminal_typing_tutor/series/S/4/data.yaml
--rw-r--r--   0        0        0        2 2023-06-11 03:21:12.335766 terminal_typing_tutor-0.1.0/terminal_typing_tutor/series/S/lesson_count
--rw-r--r--   0        0        0      203 2023-06-11 03:21:12.335766 terminal_typing_tutor-0.1.0/terminal_typing_tutor/series/S/menu.json
--rw-r--r--   0        0        0    18263 2023-06-11 03:21:12.335766 terminal_typing_tutor-0.1.0/terminal_typing_tutor/series/S/s.typ
--rw-r--r--   0        0        0       13 2023-06-11 03:21:12.335766 terminal_typing_tutor-0.1.0/terminal_typing_tutor/series/S/title
--rw-r--r--   0        0        0     4694 2023-06-11 03:21:12.335766 terminal_typing_tutor-0.1.0/terminal_typing_tutor/series/T/1/data.yaml
--rw-r--r--   0        0        0     4139 2023-06-11 03:21:12.335766 terminal_typing_tutor-0.1.0/terminal_typing_tutor/series/T/10/data.yaml
--rw-r--r--   0        0        0     3081 2023-06-11 03:21:12.335766 terminal_typing_tutor-0.1.0/terminal_typing_tutor/series/T/11/data.yaml
--rw-r--r--   0        0        0     3842 2023-06-11 03:21:12.335766 terminal_typing_tutor-0.1.0/terminal_typing_tutor/series/T/12/data.yaml
--rw-r--r--   0        0        0      741 2023-06-11 03:21:12.339766 terminal_typing_tutor-0.1.0/terminal_typing_tutor/series/T/13/data.yaml
--rw-r--r--   0        0        0     1669 2023-06-11 03:21:12.339766 terminal_typing_tutor-0.1.0/terminal_typing_tutor/series/T/14/data.yaml
--rw-r--r--   0        0        0     3331 2023-06-11 03:21:12.339766 terminal_typing_tutor-0.1.0/terminal_typing_tutor/series/T/15/data.yaml
--rw-r--r--   0        0        0     3828 2023-06-11 03:21:12.339766 terminal_typing_tutor-0.1.0/terminal_typing_tutor/series/T/16/data.yaml
--rw-r--r--   0        0        0     2344 2023-06-11 03:21:12.335766 terminal_typing_tutor-0.1.0/terminal_typing_tutor/series/T/2/data.yaml
--rw-r--r--   0        0        0     3296 2023-06-11 03:21:12.335766 terminal_typing_tutor-0.1.0/terminal_typing_tutor/series/T/3/data.yaml
--rw-r--r--   0        0        0     2254 2023-06-11 03:21:12.335766 terminal_typing_tutor-0.1.0/terminal_typing_tutor/series/T/4/data.yaml
--rw-r--r--   0        0        0     2633 2023-06-11 03:21:12.335766 terminal_typing_tutor-0.1.0/terminal_typing_tutor/series/T/5/data.yaml
--rw-r--r--   0        0        0     2227 2023-06-11 03:21:12.335766 terminal_typing_tutor-0.1.0/terminal_typing_tutor/series/T/6/data.yaml
--rw-r--r--   0        0        0     3282 2023-06-11 03:21:12.335766 terminal_typing_tutor-0.1.0/terminal_typing_tutor/series/T/7/data.yaml
--rw-r--r--   0        0        0     3137 2023-06-11 03:21:12.335766 terminal_typing_tutor-0.1.0/terminal_typing_tutor/series/T/8/data.yaml
--rw-r--r--   0        0        0     2791 2023-06-11 03:21:12.335766 terminal_typing_tutor-0.1.0/terminal_typing_tutor/series/T/9/data.yaml
--rw-r--r--   0        0        0        3 2023-06-11 03:21:12.335766 terminal_typing_tutor-0.1.0/terminal_typing_tutor/series/T/lesson_count
--rw-r--r--   0        0        0      932 2023-06-11 03:21:12.335766 terminal_typing_tutor-0.1.0/terminal_typing_tutor/series/T/menu.json
--rw-r--r--   0        0        0    40881 2023-06-11 03:21:12.335766 terminal_typing_tutor-0.1.0/terminal_typing_tutor/series/T/t.typ
--rw-r--r--   0        0        0       20 2023-06-11 03:21:12.335766 terminal_typing_tutor-0.1.0/terminal_typing_tutor/series/T/title
--rw-r--r--   0        0        0      416 2023-06-11 03:21:12.339766 terminal_typing_tutor-0.1.0/terminal_typing_tutor/series/U/1/data.yaml
--rw-r--r--   0        0        0     1376 2023-06-11 03:21:12.339766 terminal_typing_tutor-0.1.0/terminal_typing_tutor/series/U/10/data.yaml
--rw-r--r--   0        0        0     1324 2023-06-11 03:21:12.339766 terminal_typing_tutor-0.1.0/terminal_typing_tutor/series/U/11/data.yaml
--rw-r--r--   0        0        0     1400 2023-06-11 03:21:12.339766 terminal_typing_tutor-0.1.0/terminal_typing_tutor/series/U/12/data.yaml
--rw-r--r--   0        0        0     3117 2023-06-11 03:21:12.339766 terminal_typing_tutor-0.1.0/terminal_typing_tutor/series/U/13/data.yaml
--rw-r--r--   0        0        0      996 2023-06-11 03:21:12.339766 terminal_typing_tutor-0.1.0/terminal_typing_tutor/series/U/2/data.yaml
--rw-r--r--   0        0        0     1295 2023-06-11 03:21:12.339766 terminal_typing_tutor-0.1.0/terminal_typing_tutor/series/U/3/data.yaml
--rw-r--r--   0        0        0      631 2023-06-11 03:21:12.339766 terminal_typing_tutor-0.1.0/terminal_typing_tutor/series/U/4/data.yaml
--rw-r--r--   0        0        0     1119 2023-06-11 03:21:12.339766 terminal_typing_tutor-0.1.0/terminal_typing_tutor/series/U/5/data.yaml
--rw-r--r--   0        0        0     1166 2023-06-11 03:21:12.339766 terminal_typing_tutor-0.1.0/terminal_typing_tutor/series/U/6/data.yaml
--rw-r--r--   0        0        0     1189 2023-06-11 03:21:12.339766 terminal_typing_tutor-0.1.0/terminal_typing_tutor/series/U/7/data.yaml
--rw-r--r--   0        0        0     1239 2023-06-11 03:21:12.339766 terminal_typing_tutor-0.1.0/terminal_typing_tutor/series/U/8/data.yaml
--rw-r--r--   0        0        0     1343 2023-06-11 03:21:12.339766 terminal_typing_tutor-0.1.0/terminal_typing_tutor/series/U/9/data.yaml
--rw-r--r--   0        0        0        3 2023-06-11 03:21:12.339766 terminal_typing_tutor-0.1.0/terminal_typing_tutor/series/U/lesson_count
--rw-r--r--   0        0        0     1030 2023-06-11 03:21:12.339766 terminal_typing_tutor-0.1.0/terminal_typing_tutor/series/U/menu.json
--rw-r--r--   0        0        0       15 2023-06-11 03:21:12.339766 terminal_typing_tutor-0.1.0/terminal_typing_tutor/series/U/title
--rw-r--r--   0        0        0    19159 2023-06-11 03:21:12.339766 terminal_typing_tutor-0.1.0/terminal_typing_tutor/series/U/u.typ
--rw-r--r--   0        0        0      581 2023-06-11 03:21:12.339766 terminal_typing_tutor-0.1.0/terminal_typing_tutor/series/V/1/data.yaml
--rw-r--r--   0        0        0     2382 2023-06-11 03:21:12.339766 terminal_typing_tutor-0.1.0/terminal_typing_tutor/series/V/10/data.yaml
--rw-r--r--   0        0        0     2467 2023-06-11 03:21:12.339766 terminal_typing_tutor-0.1.0/terminal_typing_tutor/series/V/11/data.yaml
--rw-r--r--   0        0        0     2535 2023-06-11 03:21:12.339766 terminal_typing_tutor-0.1.0/terminal_typing_tutor/series/V/12/data.yaml
--rw-r--r--   0        0        0     2915 2023-06-11 03:21:12.339766 terminal_typing_tutor-0.1.0/terminal_typing_tutor/series/V/13/data.yaml
--rw-r--r--   0        0        0     3006 2023-06-11 03:21:12.343766 terminal_typing_tutor-0.1.0/terminal_typing_tutor/series/V/14/data.yaml
--rw-r--r--   0        0        0     5525 2023-06-11 03:21:12.339766 terminal_typing_tutor-0.1.0/terminal_typing_tutor/series/V/15/data.yaml
--rw-r--r--   0        0        0     3465 2023-06-11 03:21:12.339766 terminal_typing_tutor-0.1.0/terminal_typing_tutor/series/V/16/data.yaml
--rw-r--r--   0        0        0     3747 2023-06-11 03:21:12.339766 terminal_typing_tutor-0.1.0/terminal_typing_tutor/series/V/17/data.yaml
--rw-r--r--   0        0        0     3711 2023-06-11 03:21:12.339766 terminal_typing_tutor-0.1.0/terminal_typing_tutor/series/V/18/data.yaml
--rw-r--r--   0        0        0     2927 2023-06-11 03:21:12.339766 terminal_typing_tutor-0.1.0/terminal_typing_tutor/series/V/19/data.yaml
--rw-r--r--   0        0        0     1598 2023-06-11 03:21:12.339766 terminal_typing_tutor-0.1.0/terminal_typing_tutor/series/V/2/data.yaml
--rw-r--r--   0        0        0     2077 2023-06-11 03:21:12.339766 terminal_typing_tutor-0.1.0/terminal_typing_tutor/series/V/3/data.yaml
--rw-r--r--   0        0        0     1873 2023-06-11 03:21:12.339766 terminal_typing_tutor-0.1.0/terminal_typing_tutor/series/V/4/data.yaml
--rw-r--r--   0        0        0     2103 2023-06-11 03:21:12.339766 terminal_typing_tutor-0.1.0/terminal_typing_tutor/series/V/5/data.yaml
--rw-r--r--   0        0        0     1831 2023-06-11 03:21:12.339766 terminal_typing_tutor-0.1.0/terminal_typing_tutor/series/V/6/data.yaml
--rw-r--r--   0        0        0     2071 2023-06-11 03:21:12.339766 terminal_typing_tutor-0.1.0/terminal_typing_tutor/series/V/7/data.yaml
--rw-r--r--   0        0        0     1780 2023-06-11 03:21:12.339766 terminal_typing_tutor-0.1.0/terminal_typing_tutor/series/V/8/data.yaml
--rw-r--r--   0        0        0     2053 2023-06-11 03:21:12.339766 terminal_typing_tutor-0.1.0/terminal_typing_tutor/series/V/9/data.yaml
--rw-r--r--   0        0        0        3 2023-06-11 03:21:12.339766 terminal_typing_tutor-0.1.0/terminal_typing_tutor/series/V/lesson_count
--rw-r--r--   0        0        0     1295 2023-06-11 03:21:12.339766 terminal_typing_tutor-0.1.0/terminal_typing_tutor/series/V/menu.json
--rw-r--r--   0        0        0       16 2023-06-11 03:21:12.339766 terminal_typing_tutor-0.1.0/terminal_typing_tutor/series/V/title
--rw-r--r--   0        0        0    47250 2023-06-11 03:21:12.339766 terminal_typing_tutor-0.1.0/terminal_typing_tutor/series/V/v.typ
--rw-r--r--   0        0        0    15860 2023-06-11 04:21:49.699690 terminal_typing_tutor-0.1.0/terminal_typing_tutor/tutor.py
--rw-r--r--   0        0        0     2268 1970-01-01 00:00:00.000000 terminal_typing_tutor-0.1.0/PKG-INFO
+-rw-r--r--   0        0        0    35149 2023-06-11 22:25:13.467755 terminal_typing_tutor-0.2.0/LICENSE
+-rw-r--r--   0        0        0     2927 2023-06-11 22:34:08.347744 terminal_typing_tutor-0.2.0/README.md
+-rw-r--r--   0        0        0      562 2023-06-11 20:19:26.487912 terminal_typing_tutor-0.2.0/pyproject.toml
+-rw-r--r--   0        0        0       69 2023-06-11 21:09:06.071850 terminal_typing_tutor-0.2.0/terminal_typing_tutor/__init__.py
+-rw-r--r--   0        0        0       31 2023-06-11 04:25:58.607685 terminal_typing_tutor-0.2.0/terminal_typing_tutor/__main__.py
+-rw-r--r--   0        0        0     1567 2023-06-11 21:08:32.491851 terminal_typing_tutor-0.2.0/terminal_typing_tutor/constants.py
+-rwxr-xr-x   0        0        0      201 2023-06-11 04:11:52.927703 terminal_typing_tutor-0.2.0/terminal_typing_tutor/main.py
+-rw-r--r--   0        0        0     3364 2023-06-11 03:21:12.331766 terminal_typing_tutor-0.2.0/terminal_typing_tutor/series/M/1/data.yaml
+-rw-r--r--   0        0        0     3377 2023-06-11 03:21:12.331766 terminal_typing_tutor-0.2.0/terminal_typing_tutor/series/M/10/data.yaml
+-rw-r--r--   0        0        0     4191 2023-06-11 03:21:12.331766 terminal_typing_tutor-0.2.0/terminal_typing_tutor/series/M/11/data.yaml
+-rw-r--r--   0        0        0     2861 2023-06-11 03:21:12.331766 terminal_typing_tutor-0.2.0/terminal_typing_tutor/series/M/2/data.yaml
+-rw-r--r--   0        0        0     3201 2023-06-11 03:21:12.331766 terminal_typing_tutor-0.2.0/terminal_typing_tutor/series/M/3/data.yaml
+-rw-r--r--   0        0        0     2680 2023-06-11 03:21:12.331766 terminal_typing_tutor-0.2.0/terminal_typing_tutor/series/M/4/data.yaml
+-rw-r--r--   0        0        0     3175 2023-06-11 03:21:12.331766 terminal_typing_tutor-0.2.0/terminal_typing_tutor/series/M/5/data.yaml
+-rw-r--r--   0        0        0     3017 2023-06-11 03:21:12.331766 terminal_typing_tutor-0.2.0/terminal_typing_tutor/series/M/6/data.yaml
+-rw-r--r--   0        0        0     2591 2023-06-11 03:21:12.331766 terminal_typing_tutor-0.2.0/terminal_typing_tutor/series/M/7/data.yaml
+-rw-r--r--   0        0        0     3028 2023-06-11 03:21:12.331766 terminal_typing_tutor-0.2.0/terminal_typing_tutor/series/M/8/data.yaml
+-rw-r--r--   0        0        0     3861 2023-06-11 03:21:12.331766 terminal_typing_tutor-0.2.0/terminal_typing_tutor/series/M/9/data.yaml
+-rw-r--r--   0        0        0        3 2023-06-11 03:21:12.331766 terminal_typing_tutor-0.2.0/terminal_typing_tutor/series/M/lesson_count
+-rw-r--r--   0        0        0    36212 2023-06-11 03:21:12.331766 terminal_typing_tutor-0.2.0/terminal_typing_tutor/series/M/m.typ
+-rw-r--r--   0        0        0      520 2023-06-11 03:21:12.331766 terminal_typing_tutor-0.2.0/terminal_typing_tutor/series/M/menu.json
+-rw-r--r--   0        0        0       14 2023-06-11 03:21:12.331766 terminal_typing_tutor-0.2.0/terminal_typing_tutor/series/M/title
+-rw-r--r--   0        0        0     5885 2023-06-11 03:21:12.331766 terminal_typing_tutor-0.2.0/terminal_typing_tutor/series/Q/1/data.yaml
+-rw-r--r--   0        0        0     2445 2023-06-11 03:21:12.331766 terminal_typing_tutor-0.2.0/terminal_typing_tutor/series/Q/2/data.yaml
+-rw-r--r--   0        0        0     3099 2023-06-11 03:21:12.331766 terminal_typing_tutor-0.2.0/terminal_typing_tutor/series/Q/3/data.yaml
+-rw-r--r--   0        0        0     3034 2023-06-11 03:21:12.335766 terminal_typing_tutor-0.2.0/terminal_typing_tutor/series/Q/4/data.yaml
+-rw-r--r--   0        0        0     2004 2023-06-11 03:21:12.335766 terminal_typing_tutor-0.2.0/terminal_typing_tutor/series/Q/5/data.yaml
+-rw-r--r--   0        0        0        2 2023-06-11 03:21:12.331766 terminal_typing_tutor-0.2.0/terminal_typing_tutor/series/Q/lesson_count
+-rw-r--r--   0        0        0      293 2023-06-11 03:21:12.331766 terminal_typing_tutor-0.2.0/terminal_typing_tutor/series/Q/menu.json
+-rw-r--r--   0        0        0    16803 2023-06-11 03:21:12.331766 terminal_typing_tutor-0.2.0/terminal_typing_tutor/series/Q/q.typ
+-rw-r--r--   0        0        0       20 2023-06-11 03:21:12.331766 terminal_typing_tutor-0.2.0/terminal_typing_tutor/series/Q/title
+-rw-r--r--   0        0        0     2650 2023-06-11 03:21:12.335766 terminal_typing_tutor-0.2.0/terminal_typing_tutor/series/R/1/data.yaml
+-rw-r--r--   0        0        0     3389 2023-06-11 03:21:12.335766 terminal_typing_tutor-0.2.0/terminal_typing_tutor/series/R/10/data.yaml
+-rw-r--r--   0        0        0     2608 2023-06-11 03:21:12.335766 terminal_typing_tutor-0.2.0/terminal_typing_tutor/series/R/11/data.yaml
+-rw-r--r--   0        0        0     2975 2023-06-11 03:21:12.335766 terminal_typing_tutor-0.2.0/terminal_typing_tutor/series/R/12/data.yaml
+-rw-r--r--   0        0        0     2659 2023-06-11 03:21:12.335766 terminal_typing_tutor-0.2.0/terminal_typing_tutor/series/R/13/data.yaml
+-rw-r--r--   0        0        0     3307 2023-06-11 03:21:12.335766 terminal_typing_tutor-0.2.0/terminal_typing_tutor/series/R/14/data.yaml
+-rw-r--r--   0        0        0     2721 2023-06-11 03:21:12.335766 terminal_typing_tutor-0.2.0/terminal_typing_tutor/series/R/2/data.yaml
+-rw-r--r--   0        0        0     3181 2023-06-11 03:21:12.335766 terminal_typing_tutor-0.2.0/terminal_typing_tutor/series/R/3/data.yaml
+-rw-r--r--   0        0        0     2764 2023-06-11 03:21:12.335766 terminal_typing_tutor-0.2.0/terminal_typing_tutor/series/R/4/data.yaml
+-rw-r--r--   0        0        0     3166 2023-06-11 03:21:12.335766 terminal_typing_tutor-0.2.0/terminal_typing_tutor/series/R/5/data.yaml
+-rw-r--r--   0        0        0     2920 2023-06-11 03:21:12.335766 terminal_typing_tutor-0.2.0/terminal_typing_tutor/series/R/6/data.yaml
+-rw-r--r--   0        0        0     2852 2023-06-11 03:21:12.335766 terminal_typing_tutor-0.2.0/terminal_typing_tutor/series/R/7/data.yaml
+-rw-r--r--   0        0        0     3119 2023-06-11 03:21:12.335766 terminal_typing_tutor-0.2.0/terminal_typing_tutor/series/R/8/data.yaml
+-rw-r--r--   0        0        0     3491 2023-06-11 03:21:12.335766 terminal_typing_tutor-0.2.0/terminal_typing_tutor/series/R/9/data.yaml
+-rw-r--r--   0        0        0        3 2023-06-11 03:21:12.335766 terminal_typing_tutor-0.2.0/terminal_typing_tutor/series/R/lesson_count
+-rw-r--r--   0        0        0      672 2023-06-11 03:21:12.335766 terminal_typing_tutor-0.2.0/terminal_typing_tutor/series/R/menu.json
+-rw-r--r--   0        0        0    41316 2023-06-11 03:21:12.335766 terminal_typing_tutor-0.2.0/terminal_typing_tutor/series/R/r.typ
+-rw-r--r--   0        0        0       19 2023-06-11 03:21:12.335766 terminal_typing_tutor-0.2.0/terminal_typing_tutor/series/R/title
+-rw-r--r--   0        0        0     2762 2023-06-11 03:21:12.335766 terminal_typing_tutor-0.2.0/terminal_typing_tutor/series/S/1/data.yaml
+-rw-r--r--   0        0        0     3364 2023-06-11 03:21:12.335766 terminal_typing_tutor-0.2.0/terminal_typing_tutor/series/S/2/data.yaml
+-rw-r--r--   0        0        0     4005 2023-06-11 03:21:12.335766 terminal_typing_tutor-0.2.0/terminal_typing_tutor/series/S/3/data.yaml
+-rw-r--r--   0        0        0     6793 2023-06-11 03:21:12.335766 terminal_typing_tutor-0.2.0/terminal_typing_tutor/series/S/4/data.yaml
+-rw-r--r--   0        0        0        2 2023-06-11 03:21:12.335766 terminal_typing_tutor-0.2.0/terminal_typing_tutor/series/S/lesson_count
+-rw-r--r--   0        0        0      203 2023-06-11 03:21:12.335766 terminal_typing_tutor-0.2.0/terminal_typing_tutor/series/S/menu.json
+-rw-r--r--   0        0        0    18263 2023-06-11 03:21:12.335766 terminal_typing_tutor-0.2.0/terminal_typing_tutor/series/S/s.typ
+-rw-r--r--   0        0        0       13 2023-06-11 03:21:12.335766 terminal_typing_tutor-0.2.0/terminal_typing_tutor/series/S/title
+-rw-r--r--   0        0        0     4694 2023-06-11 03:21:12.335766 terminal_typing_tutor-0.2.0/terminal_typing_tutor/series/T/1/data.yaml
+-rw-r--r--   0        0        0     4139 2023-06-11 03:21:12.335766 terminal_typing_tutor-0.2.0/terminal_typing_tutor/series/T/10/data.yaml
+-rw-r--r--   0        0        0     3081 2023-06-11 03:21:12.335766 terminal_typing_tutor-0.2.0/terminal_typing_tutor/series/T/11/data.yaml
+-rw-r--r--   0        0        0     3842 2023-06-11 03:21:12.335766 terminal_typing_tutor-0.2.0/terminal_typing_tutor/series/T/12/data.yaml
+-rw-r--r--   0        0        0      741 2023-06-11 03:21:12.339766 terminal_typing_tutor-0.2.0/terminal_typing_tutor/series/T/13/data.yaml
+-rw-r--r--   0        0        0     1669 2023-06-11 03:21:12.339766 terminal_typing_tutor-0.2.0/terminal_typing_tutor/series/T/14/data.yaml
+-rw-r--r--   0        0        0     3331 2023-06-11 03:21:12.339766 terminal_typing_tutor-0.2.0/terminal_typing_tutor/series/T/15/data.yaml
+-rw-r--r--   0        0        0     3828 2023-06-11 03:21:12.339766 terminal_typing_tutor-0.2.0/terminal_typing_tutor/series/T/16/data.yaml
+-rw-r--r--   0        0        0     2344 2023-06-11 03:21:12.335766 terminal_typing_tutor-0.2.0/terminal_typing_tutor/series/T/2/data.yaml
+-rw-r--r--   0        0        0     3296 2023-06-11 03:21:12.335766 terminal_typing_tutor-0.2.0/terminal_typing_tutor/series/T/3/data.yaml
+-rw-r--r--   0        0        0     2254 2023-06-11 03:21:12.335766 terminal_typing_tutor-0.2.0/terminal_typing_tutor/series/T/4/data.yaml
+-rw-r--r--   0        0        0     2633 2023-06-11 03:21:12.335766 terminal_typing_tutor-0.2.0/terminal_typing_tutor/series/T/5/data.yaml
+-rw-r--r--   0        0        0     2227 2023-06-11 03:21:12.335766 terminal_typing_tutor-0.2.0/terminal_typing_tutor/series/T/6/data.yaml
+-rw-r--r--   0        0        0     3282 2023-06-11 03:21:12.335766 terminal_typing_tutor-0.2.0/terminal_typing_tutor/series/T/7/data.yaml
+-rw-r--r--   0        0        0     3137 2023-06-11 03:21:12.335766 terminal_typing_tutor-0.2.0/terminal_typing_tutor/series/T/8/data.yaml
+-rw-r--r--   0        0        0     2791 2023-06-11 03:21:12.335766 terminal_typing_tutor-0.2.0/terminal_typing_tutor/series/T/9/data.yaml
+-rw-r--r--   0        0        0        3 2023-06-11 03:21:12.335766 terminal_typing_tutor-0.2.0/terminal_typing_tutor/series/T/lesson_count
+-rw-r--r--   0        0        0      932 2023-06-11 03:21:12.335766 terminal_typing_tutor-0.2.0/terminal_typing_tutor/series/T/menu.json
+-rw-r--r--   0        0        0    40881 2023-06-11 03:21:12.335766 terminal_typing_tutor-0.2.0/terminal_typing_tutor/series/T/t.typ
+-rw-r--r--   0        0        0       20 2023-06-11 03:21:12.335766 terminal_typing_tutor-0.2.0/terminal_typing_tutor/series/T/title
+-rw-r--r--   0        0        0      416 2023-06-11 03:21:12.339766 terminal_typing_tutor-0.2.0/terminal_typing_tutor/series/U/1/data.yaml
+-rw-r--r--   0        0        0     1376 2023-06-11 03:21:12.339766 terminal_typing_tutor-0.2.0/terminal_typing_tutor/series/U/10/data.yaml
+-rw-r--r--   0        0        0     1324 2023-06-11 03:21:12.339766 terminal_typing_tutor-0.2.0/terminal_typing_tutor/series/U/11/data.yaml
+-rw-r--r--   0        0        0     1400 2023-06-11 03:21:12.339766 terminal_typing_tutor-0.2.0/terminal_typing_tutor/series/U/12/data.yaml
+-rw-r--r--   0        0        0     3117 2023-06-11 03:21:12.339766 terminal_typing_tutor-0.2.0/terminal_typing_tutor/series/U/13/data.yaml
+-rw-r--r--   0        0        0      996 2023-06-11 03:21:12.339766 terminal_typing_tutor-0.2.0/terminal_typing_tutor/series/U/2/data.yaml
+-rw-r--r--   0        0        0     1295 2023-06-11 03:21:12.339766 terminal_typing_tutor-0.2.0/terminal_typing_tutor/series/U/3/data.yaml
+-rw-r--r--   0        0        0      631 2023-06-11 03:21:12.339766 terminal_typing_tutor-0.2.0/terminal_typing_tutor/series/U/4/data.yaml
+-rw-r--r--   0        0        0     1119 2023-06-11 03:21:12.339766 terminal_typing_tutor-0.2.0/terminal_typing_tutor/series/U/5/data.yaml
+-rw-r--r--   0        0        0     1166 2023-06-11 03:21:12.339766 terminal_typing_tutor-0.2.0/terminal_typing_tutor/series/U/6/data.yaml
+-rw-r--r--   0        0        0     1189 2023-06-11 03:21:12.339766 terminal_typing_tutor-0.2.0/terminal_typing_tutor/series/U/7/data.yaml
+-rw-r--r--   0        0        0     1239 2023-06-11 03:21:12.339766 terminal_typing_tutor-0.2.0/terminal_typing_tutor/series/U/8/data.yaml
+-rw-r--r--   0        0        0     1343 2023-06-11 03:21:12.339766 terminal_typing_tutor-0.2.0/terminal_typing_tutor/series/U/9/data.yaml
+-rw-r--r--   0        0        0        3 2023-06-11 03:21:12.339766 terminal_typing_tutor-0.2.0/terminal_typing_tutor/series/U/lesson_count
+-rw-r--r--   0        0        0     1030 2023-06-11 03:21:12.339766 terminal_typing_tutor-0.2.0/terminal_typing_tutor/series/U/menu.json
+-rw-r--r--   0        0        0       15 2023-06-11 03:21:12.339766 terminal_typing_tutor-0.2.0/terminal_typing_tutor/series/U/title
+-rw-r--r--   0        0        0    19159 2023-06-11 03:21:12.339766 terminal_typing_tutor-0.2.0/terminal_typing_tutor/series/U/u.typ
+-rw-r--r--   0        0        0      581 2023-06-11 03:21:12.339766 terminal_typing_tutor-0.2.0/terminal_typing_tutor/series/V/1/data.yaml
+-rw-r--r--   0        0        0     2382 2023-06-11 03:21:12.339766 terminal_typing_tutor-0.2.0/terminal_typing_tutor/series/V/10/data.yaml
+-rw-r--r--   0        0        0     2467 2023-06-11 03:21:12.339766 terminal_typing_tutor-0.2.0/terminal_typing_tutor/series/V/11/data.yaml
+-rw-r--r--   0        0        0     2535 2023-06-11 03:21:12.339766 terminal_typing_tutor-0.2.0/terminal_typing_tutor/series/V/12/data.yaml
+-rw-r--r--   0        0        0     2915 2023-06-11 03:21:12.339766 terminal_typing_tutor-0.2.0/terminal_typing_tutor/series/V/13/data.yaml
+-rw-r--r--   0        0        0     3006 2023-06-11 03:21:12.343766 terminal_typing_tutor-0.2.0/terminal_typing_tutor/series/V/14/data.yaml
+-rw-r--r--   0        0        0     5525 2023-06-11 03:21:12.339766 terminal_typing_tutor-0.2.0/terminal_typing_tutor/series/V/15/data.yaml
+-rw-r--r--   0        0        0     3465 2023-06-11 03:21:12.339766 terminal_typing_tutor-0.2.0/terminal_typing_tutor/series/V/16/data.yaml
+-rw-r--r--   0        0        0     3747 2023-06-11 03:21:12.339766 terminal_typing_tutor-0.2.0/terminal_typing_tutor/series/V/17/data.yaml
+-rw-r--r--   0        0        0     3711 2023-06-11 03:21:12.339766 terminal_typing_tutor-0.2.0/terminal_typing_tutor/series/V/18/data.yaml
+-rw-r--r--   0        0        0     2927 2023-06-11 03:21:12.339766 terminal_typing_tutor-0.2.0/terminal_typing_tutor/series/V/19/data.yaml
+-rw-r--r--   0        0        0     1598 2023-06-11 03:21:12.339766 terminal_typing_tutor-0.2.0/terminal_typing_tutor/series/V/2/data.yaml
+-rw-r--r--   0        0        0     2077 2023-06-11 03:21:12.339766 terminal_typing_tutor-0.2.0/terminal_typing_tutor/series/V/3/data.yaml
+-rw-r--r--   0        0        0     1873 2023-06-11 03:21:12.339766 terminal_typing_tutor-0.2.0/terminal_typing_tutor/series/V/4/data.yaml
+-rw-r--r--   0        0        0     2103 2023-06-11 03:21:12.339766 terminal_typing_tutor-0.2.0/terminal_typing_tutor/series/V/5/data.yaml
+-rw-r--r--   0        0        0     1831 2023-06-11 03:21:12.339766 terminal_typing_tutor-0.2.0/terminal_typing_tutor/series/V/6/data.yaml
+-rw-r--r--   0        0        0     2071 2023-06-11 03:21:12.339766 terminal_typing_tutor-0.2.0/terminal_typing_tutor/series/V/7/data.yaml
+-rw-r--r--   0        0        0     1780 2023-06-11 03:21:12.339766 terminal_typing_tutor-0.2.0/terminal_typing_tutor/series/V/8/data.yaml
+-rw-r--r--   0        0        0     2053 2023-06-11 03:21:12.339766 terminal_typing_tutor-0.2.0/terminal_typing_tutor/series/V/9/data.yaml
+-rw-r--r--   0        0        0        3 2023-06-11 03:21:12.339766 terminal_typing_tutor-0.2.0/terminal_typing_tutor/series/V/lesson_count
+-rw-r--r--   0        0        0     1295 2023-06-11 03:21:12.339766 terminal_typing_tutor-0.2.0/terminal_typing_tutor/series/V/menu.json
+-rw-r--r--   0        0        0       16 2023-06-11 03:21:12.339766 terminal_typing_tutor-0.2.0/terminal_typing_tutor/series/V/title
+-rw-r--r--   0        0        0    47250 2023-06-11 03:21:12.339766 terminal_typing_tutor-0.2.0/terminal_typing_tutor/series/V/v.typ
+-rw-r--r--   0        0        0    18397 2023-06-11 21:40:04.475811 terminal_typing_tutor-0.2.0/terminal_typing_tutor/tutor.py
+-rw-r--r--   0        0        0       80 2023-06-11 22:07:39.227777 terminal_typing_tutor-0.2.0/terminal_typing_tutor/update.json
+-rw-r--r--   0        0        0     3681 1970-01-01 00:00:00.000000 terminal_typing_tutor-0.2.0/PKG-INFO
```

### Comparing `terminal_typing_tutor-0.1.0/pyproject.toml` & `terminal_typing_tutor-0.2.0/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "terminal-typing-tutor"
-version = "0.1.0"
+version = "0.2.0"
 description = "Improve your touch-typing skills in the terminal, based on the GNU Typist program"
 authors = ["Justin Angeles <justinaawd@gmail.com>"]
 readme = "README.md"
 packages = [
 {include = "terminal_typing_tutor"},
 ]
```

### Comparing `terminal_typing_tutor-0.1.0/terminal_typing_tutor/constants.py` & `terminal_typing_tutor-0.2.0/terminal_typing_tutor/constants.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,12 @@
 from blessed import Terminal
 from typing import Literal, TypedDict
 
+CURRENT_VERSION = "0.2.0"
+
 
 
 MAIN_MENU_TITLE = "Series selection menu"
 
 MAIN_MENU = [
     {
         "title": "Series Q    Quick QWERTY course  (Q1 - Q5) ",
@@ -42,15 +44,16 @@
 WIDTH = TERM.width
 CLEAR = TERM.clear
 CENTER = TERM.center
 DOWN = TERM.move_down
 UP = TERM.move_up
 XY = TERM.move_xy
 X = TERM.move_x
-LEFT = TERM.move_right
+LEFT = TERM.move_left
+RIGHT = TERM.move_right
 MIN_PB_CHARS = 200
 
 STATS_DICT = {
 #    "drill": '', not sure of necessary right now, can tell the drill by the file path
     "accuracy": 0.00,
     "wpm": 0,
     "cpm": 0,
```

### Comparing `terminal_typing_tutor-0.1.0/terminal_typing_tutor/series/M/1/data.yaml` & `terminal_typing_tutor-0.2.0/terminal_typing_tutor/series/M/1/data.yaml`

 * *Files identical despite different names*

### Comparing `terminal_typing_tutor-0.1.0/terminal_typing_tutor/series/M/10/data.yaml` & `terminal_typing_tutor-0.2.0/terminal_typing_tutor/series/M/10/data.yaml`

 * *Files identical despite different names*

### Comparing `terminal_typing_tutor-0.1.0/terminal_typing_tutor/series/M/11/data.yaml` & `terminal_typing_tutor-0.2.0/terminal_typing_tutor/series/M/11/data.yaml`

 * *Files identical despite different names*

### Comparing `terminal_typing_tutor-0.1.0/terminal_typing_tutor/series/M/2/data.yaml` & `terminal_typing_tutor-0.2.0/terminal_typing_tutor/series/M/2/data.yaml`

 * *Files identical despite different names*

### Comparing `terminal_typing_tutor-0.1.0/terminal_typing_tutor/series/M/3/data.yaml` & `terminal_typing_tutor-0.2.0/terminal_typing_tutor/series/M/3/data.yaml`

 * *Files identical despite different names*

### Comparing `terminal_typing_tutor-0.1.0/terminal_typing_tutor/series/M/4/data.yaml` & `terminal_typing_tutor-0.2.0/terminal_typing_tutor/series/M/4/data.yaml`

 * *Files identical despite different names*

### Comparing `terminal_typing_tutor-0.1.0/terminal_typing_tutor/series/M/5/data.yaml` & `terminal_typing_tutor-0.2.0/terminal_typing_tutor/series/M/5/data.yaml`

 * *Files identical despite different names*

### Comparing `terminal_typing_tutor-0.1.0/terminal_typing_tutor/series/M/6/data.yaml` & `terminal_typing_tutor-0.2.0/terminal_typing_tutor/series/M/6/data.yaml`

 * *Files identical despite different names*

### Comparing `terminal_typing_tutor-0.1.0/terminal_typing_tutor/series/M/7/data.yaml` & `terminal_typing_tutor-0.2.0/terminal_typing_tutor/series/M/7/data.yaml`

 * *Files identical despite different names*

### Comparing `terminal_typing_tutor-0.1.0/terminal_typing_tutor/series/M/8/data.yaml` & `terminal_typing_tutor-0.2.0/terminal_typing_tutor/series/M/8/data.yaml`

 * *Files identical despite different names*

### Comparing `terminal_typing_tutor-0.1.0/terminal_typing_tutor/series/M/9/data.yaml` & `terminal_typing_tutor-0.2.0/terminal_typing_tutor/series/M/9/data.yaml`

 * *Files identical despite different names*

### Comparing `terminal_typing_tutor-0.1.0/terminal_typing_tutor/series/M/m.typ` & `terminal_typing_tutor-0.2.0/terminal_typing_tutor/series/M/m.typ`

 * *Files identical despite different names*

### Comparing `terminal_typing_tutor-0.1.0/terminal_typing_tutor/series/M/menu.json` & `terminal_typing_tutor-0.2.0/terminal_typing_tutor/series/M/menu.json`

 * *Files identical despite different names*

### Comparing `terminal_typing_tutor-0.1.0/terminal_typing_tutor/series/Q/1/data.yaml` & `terminal_typing_tutor-0.2.0/terminal_typing_tutor/series/Q/1/data.yaml`

 * *Files identical despite different names*

### Comparing `terminal_typing_tutor-0.1.0/terminal_typing_tutor/series/Q/2/data.yaml` & `terminal_typing_tutor-0.2.0/terminal_typing_tutor/series/Q/2/data.yaml`

 * *Files identical despite different names*

### Comparing `terminal_typing_tutor-0.1.0/terminal_typing_tutor/series/Q/3/data.yaml` & `terminal_typing_tutor-0.2.0/terminal_typing_tutor/series/Q/3/data.yaml`

 * *Files identical despite different names*

### Comparing `terminal_typing_tutor-0.1.0/terminal_typing_tutor/series/Q/4/data.yaml` & `terminal_typing_tutor-0.2.0/terminal_typing_tutor/series/Q/4/data.yaml`

 * *Files identical despite different names*

### Comparing `terminal_typing_tutor-0.1.0/terminal_typing_tutor/series/Q/5/data.yaml` & `terminal_typing_tutor-0.2.0/terminal_typing_tutor/series/Q/5/data.yaml`

 * *Files identical despite different names*

### Comparing `terminal_typing_tutor-0.1.0/terminal_typing_tutor/series/Q/q.typ` & `terminal_typing_tutor-0.2.0/terminal_typing_tutor/series/Q/q.typ`

 * *Files identical despite different names*

### Comparing `terminal_typing_tutor-0.1.0/terminal_typing_tutor/series/R/1/data.yaml` & `terminal_typing_tutor-0.2.0/terminal_typing_tutor/series/R/1/data.yaml`

 * *Files identical despite different names*

### Comparing `terminal_typing_tutor-0.1.0/terminal_typing_tutor/series/R/10/data.yaml` & `terminal_typing_tutor-0.2.0/terminal_typing_tutor/series/R/10/data.yaml`

 * *Files identical despite different names*

### Comparing `terminal_typing_tutor-0.1.0/terminal_typing_tutor/series/R/11/data.yaml` & `terminal_typing_tutor-0.2.0/terminal_typing_tutor/series/R/11/data.yaml`

 * *Files identical despite different names*

### Comparing `terminal_typing_tutor-0.1.0/terminal_typing_tutor/series/R/12/data.yaml` & `terminal_typing_tutor-0.2.0/terminal_typing_tutor/series/R/12/data.yaml`

 * *Files identical despite different names*

### Comparing `terminal_typing_tutor-0.1.0/terminal_typing_tutor/series/R/13/data.yaml` & `terminal_typing_tutor-0.2.0/terminal_typing_tutor/series/R/13/data.yaml`

 * *Files identical despite different names*

### Comparing `terminal_typing_tutor-0.1.0/terminal_typing_tutor/series/R/14/data.yaml` & `terminal_typing_tutor-0.2.0/terminal_typing_tutor/series/R/14/data.yaml`

 * *Files identical despite different names*

### Comparing `terminal_typing_tutor-0.1.0/terminal_typing_tutor/series/R/2/data.yaml` & `terminal_typing_tutor-0.2.0/terminal_typing_tutor/series/R/2/data.yaml`

 * *Files identical despite different names*

### Comparing `terminal_typing_tutor-0.1.0/terminal_typing_tutor/series/R/3/data.yaml` & `terminal_typing_tutor-0.2.0/terminal_typing_tutor/series/R/3/data.yaml`

 * *Files identical despite different names*

### Comparing `terminal_typing_tutor-0.1.0/terminal_typing_tutor/series/R/4/data.yaml` & `terminal_typing_tutor-0.2.0/terminal_typing_tutor/series/R/4/data.yaml`

 * *Files identical despite different names*

### Comparing `terminal_typing_tutor-0.1.0/terminal_typing_tutor/series/R/5/data.yaml` & `terminal_typing_tutor-0.2.0/terminal_typing_tutor/series/R/5/data.yaml`

 * *Files identical despite different names*

### Comparing `terminal_typing_tutor-0.1.0/terminal_typing_tutor/series/R/6/data.yaml` & `terminal_typing_tutor-0.2.0/terminal_typing_tutor/series/R/6/data.yaml`

 * *Files identical despite different names*

### Comparing `terminal_typing_tutor-0.1.0/terminal_typing_tutor/series/R/7/data.yaml` & `terminal_typing_tutor-0.2.0/terminal_typing_tutor/series/R/7/data.yaml`

 * *Files identical despite different names*

### Comparing `terminal_typing_tutor-0.1.0/terminal_typing_tutor/series/R/8/data.yaml` & `terminal_typing_tutor-0.2.0/terminal_typing_tutor/series/R/8/data.yaml`

 * *Files identical despite different names*

### Comparing `terminal_typing_tutor-0.1.0/terminal_typing_tutor/series/R/9/data.yaml` & `terminal_typing_tutor-0.2.0/terminal_typing_tutor/series/R/9/data.yaml`

 * *Files identical despite different names*

### Comparing `terminal_typing_tutor-0.1.0/terminal_typing_tutor/series/R/menu.json` & `terminal_typing_tutor-0.2.0/terminal_typing_tutor/series/R/menu.json`

 * *Files identical despite different names*

### Comparing `terminal_typing_tutor-0.1.0/terminal_typing_tutor/series/R/r.typ` & `terminal_typing_tutor-0.2.0/terminal_typing_tutor/series/R/r.typ`

 * *Files identical despite different names*

### Comparing `terminal_typing_tutor-0.1.0/terminal_typing_tutor/series/S/1/data.yaml` & `terminal_typing_tutor-0.2.0/terminal_typing_tutor/series/S/1/data.yaml`

 * *Files identical despite different names*

### Comparing `terminal_typing_tutor-0.1.0/terminal_typing_tutor/series/S/2/data.yaml` & `terminal_typing_tutor-0.2.0/terminal_typing_tutor/series/S/2/data.yaml`

 * *Files identical despite different names*

### Comparing `terminal_typing_tutor-0.1.0/terminal_typing_tutor/series/S/3/data.yaml` & `terminal_typing_tutor-0.2.0/terminal_typing_tutor/series/S/3/data.yaml`

 * *Files identical despite different names*

### Comparing `terminal_typing_tutor-0.1.0/terminal_typing_tutor/series/S/4/data.yaml` & `terminal_typing_tutor-0.2.0/terminal_typing_tutor/series/S/4/data.yaml`

 * *Files identical despite different names*

### Comparing `terminal_typing_tutor-0.1.0/terminal_typing_tutor/series/S/s.typ` & `terminal_typing_tutor-0.2.0/terminal_typing_tutor/series/S/s.typ`

 * *Files identical despite different names*

### Comparing `terminal_typing_tutor-0.1.0/terminal_typing_tutor/series/T/1/data.yaml` & `terminal_typing_tutor-0.2.0/terminal_typing_tutor/series/T/1/data.yaml`

 * *Files identical despite different names*

### Comparing `terminal_typing_tutor-0.1.0/terminal_typing_tutor/series/T/10/data.yaml` & `terminal_typing_tutor-0.2.0/terminal_typing_tutor/series/T/10/data.yaml`

 * *Files identical despite different names*

### Comparing `terminal_typing_tutor-0.1.0/terminal_typing_tutor/series/T/11/data.yaml` & `terminal_typing_tutor-0.2.0/terminal_typing_tutor/series/T/11/data.yaml`

 * *Files identical despite different names*

### Comparing `terminal_typing_tutor-0.1.0/terminal_typing_tutor/series/T/12/data.yaml` & `terminal_typing_tutor-0.2.0/terminal_typing_tutor/series/T/12/data.yaml`

 * *Files identical despite different names*

### Comparing `terminal_typing_tutor-0.1.0/terminal_typing_tutor/series/T/13/data.yaml` & `terminal_typing_tutor-0.2.0/terminal_typing_tutor/series/T/13/data.yaml`

 * *Files identical despite different names*

### Comparing `terminal_typing_tutor-0.1.0/terminal_typing_tutor/series/T/14/data.yaml` & `terminal_typing_tutor-0.2.0/terminal_typing_tutor/series/T/14/data.yaml`

 * *Files identical despite different names*

### Comparing `terminal_typing_tutor-0.1.0/terminal_typing_tutor/series/T/15/data.yaml` & `terminal_typing_tutor-0.2.0/terminal_typing_tutor/series/T/15/data.yaml`

 * *Files identical despite different names*

### Comparing `terminal_typing_tutor-0.1.0/terminal_typing_tutor/series/T/16/data.yaml` & `terminal_typing_tutor-0.2.0/terminal_typing_tutor/series/T/16/data.yaml`

 * *Files identical despite different names*

### Comparing `terminal_typing_tutor-0.1.0/terminal_typing_tutor/series/T/2/data.yaml` & `terminal_typing_tutor-0.2.0/terminal_typing_tutor/series/T/2/data.yaml`

 * *Files identical despite different names*

### Comparing `terminal_typing_tutor-0.1.0/terminal_typing_tutor/series/T/3/data.yaml` & `terminal_typing_tutor-0.2.0/terminal_typing_tutor/series/T/3/data.yaml`

 * *Files identical despite different names*

### Comparing `terminal_typing_tutor-0.1.0/terminal_typing_tutor/series/T/4/data.yaml` & `terminal_typing_tutor-0.2.0/terminal_typing_tutor/series/T/4/data.yaml`

 * *Files identical despite different names*

### Comparing `terminal_typing_tutor-0.1.0/terminal_typing_tutor/series/T/5/data.yaml` & `terminal_typing_tutor-0.2.0/terminal_typing_tutor/series/T/5/data.yaml`

 * *Files identical despite different names*

### Comparing `terminal_typing_tutor-0.1.0/terminal_typing_tutor/series/T/6/data.yaml` & `terminal_typing_tutor-0.2.0/terminal_typing_tutor/series/T/6/data.yaml`

 * *Files identical despite different names*

### Comparing `terminal_typing_tutor-0.1.0/terminal_typing_tutor/series/T/7/data.yaml` & `terminal_typing_tutor-0.2.0/terminal_typing_tutor/series/T/7/data.yaml`

 * *Files identical despite different names*

### Comparing `terminal_typing_tutor-0.1.0/terminal_typing_tutor/series/T/8/data.yaml` & `terminal_typing_tutor-0.2.0/terminal_typing_tutor/series/T/8/data.yaml`

 * *Files identical despite different names*

### Comparing `terminal_typing_tutor-0.1.0/terminal_typing_tutor/series/T/9/data.yaml` & `terminal_typing_tutor-0.2.0/terminal_typing_tutor/series/T/9/data.yaml`

 * *Files identical despite different names*

### Comparing `terminal_typing_tutor-0.1.0/terminal_typing_tutor/series/T/menu.json` & `terminal_typing_tutor-0.2.0/terminal_typing_tutor/series/T/menu.json`

 * *Files identical despite different names*

### Comparing `terminal_typing_tutor-0.1.0/terminal_typing_tutor/series/T/t.typ` & `terminal_typing_tutor-0.2.0/terminal_typing_tutor/series/T/t.typ`

 * *Files identical despite different names*

### Comparing `terminal_typing_tutor-0.1.0/terminal_typing_tutor/series/U/10/data.yaml` & `terminal_typing_tutor-0.2.0/terminal_typing_tutor/series/U/10/data.yaml`

 * *Files identical despite different names*

### Comparing `terminal_typing_tutor-0.1.0/terminal_typing_tutor/series/U/11/data.yaml` & `terminal_typing_tutor-0.2.0/terminal_typing_tutor/series/U/11/data.yaml`

 * *Files identical despite different names*

### Comparing `terminal_typing_tutor-0.1.0/terminal_typing_tutor/series/U/12/data.yaml` & `terminal_typing_tutor-0.2.0/terminal_typing_tutor/series/U/12/data.yaml`

 * *Files identical despite different names*

### Comparing `terminal_typing_tutor-0.1.0/terminal_typing_tutor/series/U/13/data.yaml` & `terminal_typing_tutor-0.2.0/terminal_typing_tutor/series/U/13/data.yaml`

 * *Files identical despite different names*

### Comparing `terminal_typing_tutor-0.1.0/terminal_typing_tutor/series/U/2/data.yaml` & `terminal_typing_tutor-0.2.0/terminal_typing_tutor/series/U/2/data.yaml`

 * *Files identical despite different names*

### Comparing `terminal_typing_tutor-0.1.0/terminal_typing_tutor/series/U/3/data.yaml` & `terminal_typing_tutor-0.2.0/terminal_typing_tutor/series/U/3/data.yaml`

 * *Files identical despite different names*

### Comparing `terminal_typing_tutor-0.1.0/terminal_typing_tutor/series/U/4/data.yaml` & `terminal_typing_tutor-0.2.0/terminal_typing_tutor/series/U/4/data.yaml`

 * *Files identical despite different names*

### Comparing `terminal_typing_tutor-0.1.0/terminal_typing_tutor/series/U/5/data.yaml` & `terminal_typing_tutor-0.2.0/terminal_typing_tutor/series/U/5/data.yaml`

 * *Files identical despite different names*

### Comparing `terminal_typing_tutor-0.1.0/terminal_typing_tutor/series/U/6/data.yaml` & `terminal_typing_tutor-0.2.0/terminal_typing_tutor/series/U/6/data.yaml`

 * *Files identical despite different names*

### Comparing `terminal_typing_tutor-0.1.0/terminal_typing_tutor/series/U/7/data.yaml` & `terminal_typing_tutor-0.2.0/terminal_typing_tutor/series/U/7/data.yaml`

 * *Files identical despite different names*

### Comparing `terminal_typing_tutor-0.1.0/terminal_typing_tutor/series/U/8/data.yaml` & `terminal_typing_tutor-0.2.0/terminal_typing_tutor/series/U/8/data.yaml`

 * *Files identical despite different names*

### Comparing `terminal_typing_tutor-0.1.0/terminal_typing_tutor/series/U/9/data.yaml` & `terminal_typing_tutor-0.2.0/terminal_typing_tutor/series/U/9/data.yaml`

 * *Files identical despite different names*

### Comparing `terminal_typing_tutor-0.1.0/terminal_typing_tutor/series/U/menu.json` & `terminal_typing_tutor-0.2.0/terminal_typing_tutor/series/U/menu.json`

 * *Files identical despite different names*

### Comparing `terminal_typing_tutor-0.1.0/terminal_typing_tutor/series/U/u.typ` & `terminal_typing_tutor-0.2.0/terminal_typing_tutor/series/U/u.typ`

 * *Files identical despite different names*

### Comparing `terminal_typing_tutor-0.1.0/terminal_typing_tutor/series/V/1/data.yaml` & `terminal_typing_tutor-0.2.0/terminal_typing_tutor/series/V/1/data.yaml`

 * *Files identical despite different names*

### Comparing `terminal_typing_tutor-0.1.0/terminal_typing_tutor/series/V/10/data.yaml` & `terminal_typing_tutor-0.2.0/terminal_typing_tutor/series/V/10/data.yaml`

 * *Files identical despite different names*

### Comparing `terminal_typing_tutor-0.1.0/terminal_typing_tutor/series/V/11/data.yaml` & `terminal_typing_tutor-0.2.0/terminal_typing_tutor/series/V/11/data.yaml`

 * *Files identical despite different names*

### Comparing `terminal_typing_tutor-0.1.0/terminal_typing_tutor/series/V/12/data.yaml` & `terminal_typing_tutor-0.2.0/terminal_typing_tutor/series/V/12/data.yaml`

 * *Files identical despite different names*

### Comparing `terminal_typing_tutor-0.1.0/terminal_typing_tutor/series/V/13/data.yaml` & `terminal_typing_tutor-0.2.0/terminal_typing_tutor/series/V/13/data.yaml`

 * *Files identical despite different names*

### Comparing `terminal_typing_tutor-0.1.0/terminal_typing_tutor/series/V/14/data.yaml` & `terminal_typing_tutor-0.2.0/terminal_typing_tutor/series/V/14/data.yaml`

 * *Files identical despite different names*

### Comparing `terminal_typing_tutor-0.1.0/terminal_typing_tutor/series/V/15/data.yaml` & `terminal_typing_tutor-0.2.0/terminal_typing_tutor/series/V/15/data.yaml`

 * *Files identical despite different names*

### Comparing `terminal_typing_tutor-0.1.0/terminal_typing_tutor/series/V/16/data.yaml` & `terminal_typing_tutor-0.2.0/terminal_typing_tutor/series/V/16/data.yaml`

 * *Files identical despite different names*

### Comparing `terminal_typing_tutor-0.1.0/terminal_typing_tutor/series/V/17/data.yaml` & `terminal_typing_tutor-0.2.0/terminal_typing_tutor/series/V/17/data.yaml`

 * *Files identical despite different names*

### Comparing `terminal_typing_tutor-0.1.0/terminal_typing_tutor/series/V/18/data.yaml` & `terminal_typing_tutor-0.2.0/terminal_typing_tutor/series/V/18/data.yaml`

 * *Files identical despite different names*

### Comparing `terminal_typing_tutor-0.1.0/terminal_typing_tutor/series/V/19/data.yaml` & `terminal_typing_tutor-0.2.0/terminal_typing_tutor/series/V/19/data.yaml`

 * *Files identical despite different names*

### Comparing `terminal_typing_tutor-0.1.0/terminal_typing_tutor/series/V/2/data.yaml` & `terminal_typing_tutor-0.2.0/terminal_typing_tutor/series/V/2/data.yaml`

 * *Files identical despite different names*

### Comparing `terminal_typing_tutor-0.1.0/terminal_typing_tutor/series/V/3/data.yaml` & `terminal_typing_tutor-0.2.0/terminal_typing_tutor/series/V/3/data.yaml`

 * *Files identical despite different names*

### Comparing `terminal_typing_tutor-0.1.0/terminal_typing_tutor/series/V/4/data.yaml` & `terminal_typing_tutor-0.2.0/terminal_typing_tutor/series/V/4/data.yaml`

 * *Files identical despite different names*

### Comparing `terminal_typing_tutor-0.1.0/terminal_typing_tutor/series/V/5/data.yaml` & `terminal_typing_tutor-0.2.0/terminal_typing_tutor/series/V/5/data.yaml`

 * *Files identical despite different names*

### Comparing `terminal_typing_tutor-0.1.0/terminal_typing_tutor/series/V/6/data.yaml` & `terminal_typing_tutor-0.2.0/terminal_typing_tutor/series/V/6/data.yaml`

 * *Files identical despite different names*

### Comparing `terminal_typing_tutor-0.1.0/terminal_typing_tutor/series/V/7/data.yaml` & `terminal_typing_tutor-0.2.0/terminal_typing_tutor/series/V/7/data.yaml`

 * *Files identical despite different names*

### Comparing `terminal_typing_tutor-0.1.0/terminal_typing_tutor/series/V/8/data.yaml` & `terminal_typing_tutor-0.2.0/terminal_typing_tutor/series/V/8/data.yaml`

 * *Files identical despite different names*

### Comparing `terminal_typing_tutor-0.1.0/terminal_typing_tutor/series/V/9/data.yaml` & `terminal_typing_tutor-0.2.0/terminal_typing_tutor/series/V/9/data.yaml`

 * *Files identical despite different names*

### Comparing `terminal_typing_tutor-0.1.0/terminal_typing_tutor/series/V/menu.json` & `terminal_typing_tutor-0.2.0/terminal_typing_tutor/series/V/menu.json`

 * *Files identical despite different names*

### Comparing `terminal_typing_tutor-0.1.0/terminal_typing_tutor/series/V/v.typ` & `terminal_typing_tutor-0.2.0/terminal_typing_tutor/series/V/v.typ`

 * *Files identical despite different names*

### Comparing `terminal_typing_tutor-0.1.0/terminal_typing_tutor/tutor.py` & `terminal_typing_tutor-0.2.0/terminal_typing_tutor/tutor.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,16 +1,20 @@
 from typing import List, Literal, cast
+from pathlib import Path
+from datetime import date
 from blessed.keyboard import Keystroke
+from urllib import request
 import yaml
 import json
 import time
 import os
 from terminal_typing_tutor.constants import (
     MAIN_MENU,
     MAIN_MENU_TITLE,
+    RIGHT,
     STATS_DICT,
     TERM,
     HOME,
     HEIGHT,
     WIDTH,
     CLEAR,
     CENTER,
@@ -20,14 +24,15 @@
     X,
     LEFT,
     PB_DICT,
     MIN_PB_CHARS,
     TSeries,
     TStats,
     TStatsFile,
+    CURRENT_VERSION
 )
 
 # global variables, used in many functions, all should point to the same variable
 # only one series, lesson, and segment can be active at any time
 series: TSeries
 lesson: int
 segment = 0
@@ -54,29 +59,31 @@
     with TERM.raw():
         key = TERM.inkey()
         if key == "\x03":
             exit()
         return key
 
 
-def file_content(file: str, parse: Literal["yaml", "json", "text"] = "text") -> str | TStatsFile:
+def file_content(file: Path, parse: Literal["yaml", "json", "text"] = "text") -> str | TStatsFile:
     with open(file, "r") as f:
         if parse == "yaml":
             return yaml.unsafe_load(f)
         if parse == "json":
             return json.load(f)
         return f.read()
 
 
 def get_stats():
     # make sure stats files exist, create them if not
     home_dir = os.path.expanduser("~")
     pb_dir = f"{home_dir}/.config/terminal-typing-tutor/pb/{series}/{lesson}"
-    pb_file = f"{pb_dir}/{segment}.yaml"
-    all_time_file = f"{home_dir}/.config/terminal-typing-tutor/pb.yaml"
+    pb_fp = f"{pb_dir}/{segment}.yaml"
+    all_time_fp = f"{home_dir}/.config/terminal-typing-tutor/pb.yaml"
+    pb_file = Path(pb_fp)
+    all_time_file = Path(all_time_fp)
     if not os.path.exists(pb_dir):
         os.makedirs(pb_dir)
     if not os.path.exists(pb_file):
         with open(pb_file, "w") as file:
             file.write(yaml.safe_dump(STATS_DICT))
     if not os.path.exists(all_time_file):
         with open(all_time_file, "w") as file:
@@ -149,45 +156,41 @@
         current_chars = len(test_string)
         mistyped_characters = len(incorrect_pressed_keys)
         correct_characters = current_chars - mistyped_characters
         current_words = round(current_chars / 5)
         current_cpm = round(current_chars / minutes)
         current_wpm = round(current_words / minutes)
         current_acc = round(correct_characters / current_chars * 100, 2)
-        wpm_string = TERM.cyan_on_black(str(current_wpm)) + TERM.white_on_black( " words per minute")
-        accuracy_string = TERM.cyan_on_black( str(current_acc) + "%") + TERM.white_on_black(" Accuracy")
-        words_string = TERM.cyan_on_black(str(current_words)) + TERM.white_on_black( " words typed")
+        wpm_string = f" {TERM.cyan_on_black(str(current_wpm)) + TERM.white_on_black( ' Words Per Minute ')}"
+        accuracy_string = f" {TERM.cyan_on_black( str(current_acc) + '%') + TERM.white_on_black(' Accuracy ')}"
+        words_string = f" {TERM.cyan_on_black(str(current_words)) + TERM.white_on_black( ' Words Typed ')}"
         if current_acc < 97.00:
             failed_drill = True
             end_msg = " Accuracy not high enough, must hit at least 97% "
         else:
             pbs = track_pb()
             if pbs["new_wpm"]:
-                wpm_string += TERM.red_on_black(" NEW ALL TIME PB")
+                wpm_string += TERM.red_on_black("NEW ALL TIME PB ")
             elif pbs["new_drill_pb"]:
-                wpm_string += TERM.red_on_black(" NEW DRILL PB")
+                wpm_string += TERM.red_on_black("NEW DRILL PB ")
 
         print(XY(0, round(HEIGHT // 3)))
-        print(CENTER(wpm_string))
-        print(CENTER(accuracy_string))
+        print(f"{CENTER(wpm_string)}\n")
+        print(f"{CENTER(accuracy_string)}\n")
         print(CENTER(words_string))
 
     # reset stats after they are tracked and displayed
     current_wpm = 0
     current_cpm = 0
     current_acc = 0
     current_words = 0
     current_chars = 0
 
     print(HOME + XY(0, HEIGHT), end="", flush=True)
-    print(
-        TERM.black_on_white(end_msg),
-        end="",
-        flush=True,
-    )
+    print(TERM.black_on_white(end_msg), end="", flush=True)
 
     while True:
         # exit program if user hits ctrl + c
         key = get_key()
         if failed_drill:
             if key.name in ["KEY_ESCAPE", "KEY_ENTER"] or key == " ":
                 return "repeat"
@@ -204,17 +207,15 @@
                 return "menu"
             if key.lower() == "n" and confirming_exit:
                 print(HOME + XY(0, HEIGHT), end="", flush=True)
                 print( TERM.black_on_white( " Press R to repeat, N for next exercise or E to exit "), end="", flush=True,)
                 confirming_exit = False
 
 
-def pressed_key(key: Keystroke, test_string: str, correct_pressed_keys: List[str]):
-    # exit program if user hits ctrl + c
-    target_character = test_string[len(correct_pressed_keys)]
+def pressed_key(key: Keystroke, target_character: str):
     line_break = target_character == "\n"
     pressed_enter = key.name == "KEY_ENTER"
     pressed_space = key == " "
     if (key == target_character) or (line_break and pressed_enter):
         return {
             "pressed_enter": pressed_enter,
             "pressed_space": pressed_space,
@@ -222,68 +223,82 @@
         }
     return {
         "pressed_enter": pressed_enter,
         "pressed_space": pressed_space,
         "hit_target": False,
     }
 
+def print_lines(test_string: str) -> int:
+    lines = test_string.split("\n")
+    line_count = len(lines)
+    longest_line = lines[0]
+    for line in lines:
+        if len(line) > len(longest_line):
+            longest_line = line
+    extra_width = WIDTH - len(longest_line)
+    left_padding = extra_width // 2
+    for index, line in enumerate(lines):
+        if index == line_count - 1:
+            print(f"{RIGHT(left_padding)}{line}", end="", flush=True)
+        else:
+            print(f"{RIGHT(left_padding)}{line}\n", end="", flush=True)
+    if line_count > 1:
+        print(UP(line_count))
+    print(X(left_padding), end="", flush=True)
+    
+    return left_padding
 
 def run_drill(title: str, intro: str, content: str):
     drill_started = False
     pressed_wrong_key = False
     start_time = 0.0
-    test_string = content
+    test_string = content.rstrip()
     print(HOME + CLEAR, end="", flush=True)
     with TERM.location():
         print(HOME + XY(0, HEIGHT), end="", flush=True)
         info_str = "   Drill   "
-        print(
-            LEFT(WIDTH - (len(info_str))) + TERM.black_on_white(info_str),
-            end="",
-            flush=True,
-        )
+        print(RIGHT(WIDTH - (len(info_str))) + TERM.black_on_white(info_str), end="", flush=True)
     # TODO: fix down/move_up with end=''
     print(TERM.black_on_cyan(CENTER(title)) + DOWN(1))
     print(TERM.white(CENTER(intro)) + DOWN(2))
-    print(test_string + UP(2))
-    for _ in test_string.split("\n"):
-        print(UP(2))
-    print(DOWN(1))
+    left_padding = print_lines(test_string)
     correct_pressed_keys = []
     incorrect_pressed_keys = []
 
     while True:
         # first check to see if all characters typed, end drill
         if len(correct_pressed_keys) == len(test_string):
             action = end_drill(start_time, test_string, incorrect_pressed_keys)
             return action
 
+        target_character = test_string[len(correct_pressed_keys)]
+        print(f"{TERM.black_on_white(target_character)}{LEFT(1)}", end="", flush=True)
         key = get_key()
 
         if key.name == "KEY_ESCAPE":
             # start test over if in middle of test, else confirm exit
             if drill_started:
                 return "repeat"
             else:
                 action = end_drill(0.0, test_string, incorrect_pressed_keys)
                 return action
 
-        _pressed_key = pressed_key(key, test_string, correct_pressed_keys)
+        _pressed_key = pressed_key(key, target_character)
 
         # Set the start time on first key press
         if drill_started == False:
             start_time = time.time()
             drill_started = True
 
         if _pressed_key["hit_target"]:
             if pressed_wrong_key == False:
                 if not _pressed_key["pressed_enter"]:
                     print(TERM.green(key), end="", flush=True)
                 else:
-                    print(TERM.green(key))
+                    print(f"{TERM.green(key)}{RIGHT(left_padding)}", end="", flush=True)
 
             if pressed_wrong_key == True:
                 if _pressed_key["pressed_space"]:
                     print(TERM.red_on_red("x"), end="", flush=True)
                 elif _pressed_key["pressed_enter"]:
                     # may not want down here
                     print(TERM.red_on_red("x"))
@@ -335,17 +350,19 @@
         # needs to redraw menu screen every time selection is changed to highlight new selection
         display_menu_screen(menu_title, selection, menu)
     return selection
 
 
 def run_lesson_menu():
     global lesson
-    dir = f"terminal_typing_tutor/series/{series}"
-    title_file = f"{dir}/title"
-    menu_file = f"{dir}/menu.json"
+    dir = f"series/{series}"
+    title_fp = f"{dir}/title"
+    menu_fp = f"{dir}/menu.json"
+    title_file = Path(__file__).parent.joinpath(title_fp)
+    menu_file = Path(__file__).parent.joinpath(menu_fp)
     menu = file_content(menu_file, "json")
     menu_title = file_content(title_file)
 
     # lessons start at 1 not 0
     lesson = menu_selection(menu_title, menu) + 1
 
 
@@ -370,15 +387,15 @@
             even_line += " "
         print(CENTER(even_line))
     print(HOME + XY(0, HEIGHT), end="", flush=True)
     message = " Press RETURN or SPACE to continue, ESC to return to the menu "
     print(TERM.black_on_white(message) + X(0), end="", flush=True)
     info_str = " Info "
     print(
-        LEFT(WIDTH - len(info_str)) + TERM.black_on_white(info_str), end="", flush=True
+        RIGHT(WIDTH - len(info_str)) + TERM.black_on_white(info_str), end="", flush=True
     )
     while display_info:
         key = get_key()
         if key.name == "KEY_ESCAPE":
             action = "menu"
             display_info = False
         if key.name == "KEY_ENTER" or key == " ":
@@ -396,29 +413,31 @@
         if key.lower() == "y":
             return "next"
         if key.lower() == "n":
             return "menu"
 
 
 def get_lesson_data() -> dict:
-    lesson_dir = f"terminal_typing_tutor/series/{series}/{str(lesson)}"
-    data_file = f"{lesson_dir}/data.yaml"
+    lesson_dir = f"series/{series}/{str(lesson)}"
+    data_fp = f"{lesson_dir}/data.yaml"
+    data_file = Path(__file__).parent.joinpath(data_fp)
     lesson_data = cast(dict, file_content(data_file, "yaml"))
     return lesson_data
 
 
 def run_lesson():
     global lesson
     global segment
     run_lesson_menu()
     if lesson == 0:
         return 0
     show_menu = False
     lesson_data = get_lesson_data()
-    lc_file = f"terminal_typing_tutor/series/{series}/lesson_count"
+    lc_fp = f"series/{series}/lesson_count"
+    lc_file = Path(__file__).parent.joinpath(lc_fp)
     lesson_count = int(cast(str,file_content(lc_file)))
 
     while segment <= lesson_data["total_segments"]:
         is_last_segment = segment == lesson_data["total_segments"]
         if is_last_segment:
             segment = 0
             # check if user is on last lesson, return to menu
@@ -456,19 +475,53 @@
             break
 
     if show_menu == False:
         return 1
 
     return 2
 
+def days_difference(day1,day2):
+    if day1 == day2:
+        return 0
+    else:
+        return int(str(date.fromisoformat(day2)-date.fromisoformat(day1)).split(' ')[0])
+
+def update_check():
+    today=str(date.today())
+    package_name='terminal_typing_tutor'
+    update_data = Path(__file__).parent.joinpath("update.json").read_text()
+    update = json.loads(update_data)
+    latest_version = CURRENT_VERSION
+    if update["check_date"] == "" or (days_difference(update["check_date"],today) > 7 and not update["available"]):
+        try:
+            url = f"https://pypi.org/pypi/{package_name}/json"
+            data = json.load(request.urlopen(url))
+            versions = sorted(list(data["releases"].keys()))
+            latest_version = versions[-1]
+        except Exception as _:
+            print("Failed getting latest version information to check for update")
+
+        if latest_version > CURRENT_VERSION:
+             update["available"] = True
+             update["number"] = latest_version
+        update["check_date"] = today
+    update_data_to_dump = json.dumps(update)
+    Path(__file__).parent.joinpath("update.json").write_text(update_data_to_dump)
+    if update["available"] and (update["last_shown"] == "" or days_difference(update["last_shown"],today) >= 2):
+        update["last_shown"] = today
+        update_data_to_dump = json.dumps(update)
+        Path(__file__).parent.joinpath("update.json").write_text(update_data_to_dump)
+        print(f"Upgrade available! To upgrade run:")
+        print(f"pip install --user --upgrade terminal-typing-tutor")
 
 def tutor():
     """
     runs typing tutor program
     """
+    update_check()
     # with TERM.fullscreen(), TERM.hidden_cursor():
     with TERM.fullscreen(), TERM.cbreak(), TERM.hidden_cursor():  # hidden cursor off during development
         num = 0
         while True:
             if num == 0:
                 run_series_menu()
                 num = run_lesson()
```

