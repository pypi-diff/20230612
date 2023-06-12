# Comparing `tmp/ibasis-0.0.1a0.tar.gz` & `tmp/ibasis-0.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ibasis-0.0.1a0.tar", last modified: Thu May 25 06:58:50 2023, max compression
+gzip compressed data, was "ibasis-0.0.2.tar", last modified: Mon Jun  5 07:39:50 2023, max compression
```

## Comparing `ibasis-0.0.1a0.tar` & `ibasis-0.0.2.tar`

### file list

```diff
@@ -1,58 +1,69 @@
-drwxrwxr-x   0 user      (1000) user      (1000)        0 2023-05-25 06:58:50.477696 ibasis-0.0.1a0/
--rw-rw-r--   0 user      (1000) user      (1000)    35149 2023-05-25 06:20:31.000000 ibasis-0.0.1a0/LICENSE
--rw-rw-r--   0 user      (1000) user      (1000)      873 2023-05-25 06:58:50.477696 ibasis-0.0.1a0/PKG-INFO
--rw-rw-r--   0 user      (1000) user      (1000)      221 2023-05-25 06:21:55.000000 ibasis-0.0.1a0/README.md
-drwxrwxr-x   0 user      (1000) user      (1000)        0 2023-05-25 06:58:50.473696 ibasis-0.0.1a0/ibasis/
--rw-rw-r--   0 user      (1000) user      (1000)        0 2023-05-25 06:21:55.000000 ibasis-0.0.1a0/ibasis/__init__.py
--rw-rw-r--   0 user      (1000) user      (1000)     2020 2023-05-25 06:21:55.000000 ibasis-0.0.1a0/ibasis/ibasic.py
-drwxrwxr-x   0 user      (1000) user      (1000)        0 2023-05-25 06:58:50.477696 ibasis-0.0.1a0/ibasis/ibasisF/
--rw-rw-r--   0 user      (1000) user      (1000)      450 2023-05-25 06:58:49.000000 ibasis-0.0.1a0/ibasis/ibasisF/__init__.py
--rw-rw-r--   0 user      (1000) user      (1000)     2020 2023-05-25 06:21:55.000000 ibasis-0.0.1a0/ibasis/ibasisF/ibasic.py
--rw-rw-r--   0 user      (1000) user      (1000)     2360 2023-05-25 06:21:55.000000 ibasis-0.0.1a0/ibasis/ibasisF/icolor.py
--rw-rw-r--   0 user      (1000) user      (1000)     3794 2023-05-25 06:21:55.000000 ibasis-0.0.1a0/ibasis/ibasisF/idraw.py
--rw-rw-r--   0 user      (1000) user      (1000)     5472 2023-05-25 06:21:55.000000 ibasis-0.0.1a0/ibasis/ibasisF/idtbs.py
--rw-rw-r--   0 user      (1000) user      (1000)     1137 2023-05-25 06:21:55.000000 ibasis-0.0.1a0/ibasis/ibasisF/ifile.py
--rw-rw-r--   0 user      (1000) user      (1000)      378 2023-05-25 06:21:55.000000 ibasis-0.0.1a0/ibasis/ibasisF/iformat.py
--rw-rw-r--   0 user      (1000) user      (1000)     1904 2023-05-25 06:21:55.000000 ibasis-0.0.1a0/ibasis/ibasisF/iimg.py
--rw-rw-r--   0 user      (1000) user      (1000)     4660 2023-05-25 06:21:55.000000 ibasis-0.0.1a0/ibasis/ibasisF/ilmdb.py
--rw-rw-r--   0 user      (1000) user      (1000)     2749 2023-05-25 06:21:55.000000 ibasis-0.0.1a0/ibasis/ibasisF/ilog.py
--rw-rw-r--   0 user      (1000) user      (1000)     2942 2023-05-25 06:21:55.000000 ibasis-0.0.1a0/ibasis/ibasisF/imath.py
--rw-rw-r--   0 user      (1000) user      (1000)     2745 2023-05-25 06:21:55.000000 ibasis-0.0.1a0/ibasis/ibasisF/imetric.py
--rw-rw-r--   0 user      (1000) user      (1000)     4764 2023-05-25 06:21:55.000000 ibasis-0.0.1a0/ibasis/ibasisF/imgalg.py
--rw-rw-r--   0 user      (1000) user      (1000)      439 2023-05-25 06:21:55.000000 ibasis-0.0.1a0/ibasis/ibasisF/imultiproc.py
--rw-rw-r--   0 user      (1000) user      (1000)    12283 2023-05-25 06:21:55.000000 ibasis-0.0.1a0/ibasis/ibasisF/ipath.py
--rw-rw-r--   0 user      (1000) user      (1000)      469 2023-05-25 06:21:55.000000 ibasis-0.0.1a0/ibasis/ibasisF/ipoint.py
--rw-rw-r--   0 user      (1000) user      (1000)      879 2023-05-25 06:21:55.000000 ibasis-0.0.1a0/ibasis/ibasisF/iprofile.py
--rw-rw-r--   0 user      (1000) user      (1000)      196 2023-05-25 06:21:55.000000 ibasis-0.0.1a0/ibasis/ibasisF/iserialization.py
--rw-rw-r--   0 user      (1000) user      (1000)      574 2023-05-25 06:21:55.000000 ibasis-0.0.1a0/ibasis/ibasisF/ishell.py
--rw-rw-r--   0 user      (1000) user      (1000)     1729 2023-05-25 06:21:55.000000 ibasis-0.0.1a0/ibasis/ibasisF/itimeutils.py
--rw-rw-r--   0 user      (1000) user      (1000)     3001 2023-05-25 06:21:55.000000 ibasis-0.0.1a0/ibasis/ibasisF/itorch.py
--rw-rw-r--   0 user      (1000) user      (1000)     2360 2023-05-25 06:21:55.000000 ibasis-0.0.1a0/ibasis/icolor.py
--rw-rw-r--   0 user      (1000) user      (1000)     3794 2023-05-25 06:21:55.000000 ibasis-0.0.1a0/ibasis/idraw.py
--rw-rw-r--   0 user      (1000) user      (1000)     5472 2023-05-25 06:21:55.000000 ibasis-0.0.1a0/ibasis/idtbs.py
--rw-rw-r--   0 user      (1000) user      (1000)     1137 2023-05-25 06:21:55.000000 ibasis-0.0.1a0/ibasis/ifile.py
--rw-rw-r--   0 user      (1000) user      (1000)      378 2023-05-25 06:21:55.000000 ibasis-0.0.1a0/ibasis/iformat.py
--rw-rw-r--   0 user      (1000) user      (1000)     1904 2023-05-25 06:21:55.000000 ibasis-0.0.1a0/ibasis/iimg.py
--rw-rw-r--   0 user      (1000) user      (1000)     4660 2023-05-25 06:21:55.000000 ibasis-0.0.1a0/ibasis/ilmdb.py
--rw-rw-r--   0 user      (1000) user      (1000)     2749 2023-05-25 06:21:55.000000 ibasis-0.0.1a0/ibasis/ilog.py
--rw-rw-r--   0 user      (1000) user      (1000)     2942 2023-05-25 06:21:55.000000 ibasis-0.0.1a0/ibasis/imath.py
--rw-rw-r--   0 user      (1000) user      (1000)     2745 2023-05-25 06:21:55.000000 ibasis-0.0.1a0/ibasis/imetric.py
--rw-rw-r--   0 user      (1000) user      (1000)     4764 2023-05-25 06:21:55.000000 ibasis-0.0.1a0/ibasis/imgalg.py
--rw-rw-r--   0 user      (1000) user      (1000)      439 2023-05-25 06:21:55.000000 ibasis-0.0.1a0/ibasis/imultiproc.py
--rw-rw-r--   0 user      (1000) user      (1000)    12283 2023-05-25 06:21:55.000000 ibasis-0.0.1a0/ibasis/ipath.py
--rw-rw-r--   0 user      (1000) user      (1000)      469 2023-05-25 06:21:55.000000 ibasis-0.0.1a0/ibasis/ipoint.py
--rw-rw-r--   0 user      (1000) user      (1000)      879 2023-05-25 06:21:55.000000 ibasis-0.0.1a0/ibasis/iprofile.py
--rw-rw-r--   0 user      (1000) user      (1000)      196 2023-05-25 06:21:55.000000 ibasis-0.0.1a0/ibasis/iserialization.py
--rw-rw-r--   0 user      (1000) user      (1000)      574 2023-05-25 06:21:55.000000 ibasis-0.0.1a0/ibasis/ishell.py
--rw-rw-r--   0 user      (1000) user      (1000)     1729 2023-05-25 06:21:55.000000 ibasis-0.0.1a0/ibasis/itimeutils.py
--rw-rw-r--   0 user      (1000) user      (1000)     3001 2023-05-25 06:21:55.000000 ibasis-0.0.1a0/ibasis/itorch.py
-drwxrwxr-x   0 user      (1000) user      (1000)        0 2023-05-25 06:58:50.473696 ibasis-0.0.1a0/ibasis.egg-info/
--rw-rw-r--   0 user      (1000) user      (1000)      873 2023-05-25 06:58:50.000000 ibasis-0.0.1a0/ibasis.egg-info/PKG-INFO
--rw-rw-r--   0 user      (1000) user      (1000)     1101 2023-05-25 06:58:50.000000 ibasis-0.0.1a0/ibasis.egg-info/SOURCES.txt
--rw-rw-r--   0 user      (1000) user      (1000)        1 2023-05-25 06:58:50.000000 ibasis-0.0.1a0/ibasis.egg-info/dependency_links.txt
--rw-rw-r--   0 user      (1000) user      (1000)        1 2023-05-25 06:58:50.000000 ibasis-0.0.1a0/ibasis.egg-info/not-zip-safe
--rw-rw-r--   0 user      (1000) user      (1000)        7 2023-05-25 06:58:50.000000 ibasis-0.0.1a0/ibasis.egg-info/top_level.txt
--rw-rw-r--   0 user      (1000) user      (1000)       38 2023-05-25 06:58:50.477696 ibasis-0.0.1a0/setup.cfg
--rw-rw-r--   0 user      (1000) user      (1000)     1042 2023-05-25 06:57:53.000000 ibasis-0.0.1a0/setup.py
-drwxrwxr-x   0 user      (1000) user      (1000)        0 2023-05-25 06:58:50.477696 ibasis-0.0.1a0/test/
--rw-rw-r--   0 user      (1000) user      (1000)       19 2023-05-25 06:21:55.000000 ibasis-0.0.1a0/test/test_import.py
+drwxrwxr-x   0 user      (1000) user      (1000)        0 2023-06-05 07:39:50.830736 ibasis-0.0.2/
+-rw-rw-r--   0 user      (1000) user      (1000)    35149 2023-05-25 06:20:31.000000 ibasis-0.0.2/LICENSE
+-rw-rw-r--   0 user      (1000) user      (1000)      871 2023-06-05 07:39:50.830736 ibasis-0.0.2/PKG-INFO
+-rw-rw-r--   0 user      (1000) user      (1000)      221 2023-05-25 06:21:55.000000 ibasis-0.0.2/README.md
+drwxrwxr-x   0 user      (1000) user      (1000)        0 2023-06-05 07:39:50.822736 ibasis-0.0.2/busi/
+-rw-rw-r--   0 user      (1000) user      (1000)      123 2023-05-26 03:09:41.000000 ibasis-0.0.2/busi/__init__.py
+-rw-rw-r--   0 user      (1000) user      (1000)     2849 2023-05-26 03:09:41.000000 ibasis-0.0.2/busi/dtbs.py
+-rw-rw-r--   0 user      (1000) user      (1000)    10148 2023-05-26 03:09:41.000000 ibasis-0.0.2/busi/fio.py
+-rw-rw-r--   0 user      (1000) user      (1000)     5600 2023-05-26 03:09:41.000000 ibasis-0.0.2/busi/idraw.py
+-rw-rw-r--   0 user      (1000) user      (1000)     9060 2023-05-26 03:09:41.000000 ibasis-0.0.2/busi/idtbs.py
+-rw-rw-r--   0 user      (1000) user      (1000)    10169 2023-05-26 03:09:41.000000 ibasis-0.0.2/busi/parser.py
+-rw-rw-r--   0 user      (1000) user      (1000)     1233 2023-05-26 03:09:41.000000 ibasis-0.0.2/busi/test.py
+-rw-rw-r--   0 user      (1000) user      (1000)     7458 2023-05-26 03:09:41.000000 ibasis-0.0.2/busi/utils.py
+drwxrwxr-x   0 user      (1000) user      (1000)        0 2023-06-05 07:39:50.826736 ibasis-0.0.2/ibasis/
+-rw-rw-r--   0 user      (1000) user      (1000)        0 2023-05-25 06:21:55.000000 ibasis-0.0.2/ibasis/__init__.py
+-rw-rw-r--   0 user      (1000) user      (1000)     4252 2023-05-31 14:16:44.000000 ibasis-0.0.2/ibasis/iaffine.py
+-rw-rw-r--   0 user      (1000) user      (1000)     2020 2023-05-25 06:21:55.000000 ibasis-0.0.2/ibasis/ibasic.py
+drwxrwxr-x   0 user      (1000) user      (1000)        0 2023-06-05 07:39:50.830736 ibasis-0.0.2/ibasis/ibasisF/
+-rw-rw-r--   0 user      (1000) user      (1000)      473 2023-06-05 07:39:50.000000 ibasis-0.0.2/ibasis/ibasisF/__init__.py
+-rw-rw-r--   0 user      (1000) user      (1000)     4252 2023-05-31 14:16:44.000000 ibasis-0.0.2/ibasis/ibasisF/iaffine.py
+-rw-rw-r--   0 user      (1000) user      (1000)     2020 2023-05-25 06:21:55.000000 ibasis-0.0.2/ibasis/ibasisF/ibasic.py
+-rw-rw-r--   0 user      (1000) user      (1000)     2360 2023-05-25 06:21:55.000000 ibasis-0.0.2/ibasis/ibasisF/icolor.py
+-rw-rw-r--   0 user      (1000) user      (1000)     3794 2023-05-25 06:21:55.000000 ibasis-0.0.2/ibasis/ibasisF/idraw.py
+-rw-rw-r--   0 user      (1000) user      (1000)     5472 2023-05-25 06:21:55.000000 ibasis-0.0.2/ibasis/ibasisF/idtbs.py
+-rw-rw-r--   0 user      (1000) user      (1000)     1137 2023-05-25 06:21:55.000000 ibasis-0.0.2/ibasis/ibasisF/ifile.py
+-rw-rw-r--   0 user      (1000) user      (1000)      378 2023-05-25 06:21:55.000000 ibasis-0.0.2/ibasis/ibasisF/iformat.py
+-rw-rw-r--   0 user      (1000) user      (1000)     1904 2023-05-25 06:21:55.000000 ibasis-0.0.2/ibasis/ibasisF/iimg.py
+-rw-rw-r--   0 user      (1000) user      (1000)     4660 2023-05-25 06:21:55.000000 ibasis-0.0.2/ibasis/ibasisF/ilmdb.py
+-rw-rw-r--   0 user      (1000) user      (1000)     2939 2023-05-25 08:21:23.000000 ibasis-0.0.2/ibasis/ibasisF/ilog.py
+-rw-rw-r--   0 user      (1000) user      (1000)     2942 2023-05-25 06:21:55.000000 ibasis-0.0.2/ibasis/ibasisF/imath.py
+-rw-rw-r--   0 user      (1000) user      (1000)     2745 2023-05-25 06:21:55.000000 ibasis-0.0.2/ibasis/ibasisF/imetric.py
+-rw-rw-r--   0 user      (1000) user      (1000)     6122 2023-06-02 08:06:29.000000 ibasis-0.0.2/ibasis/ibasisF/imgalg.py
+-rw-rw-r--   0 user      (1000) user      (1000)      439 2023-05-25 06:21:55.000000 ibasis-0.0.2/ibasis/ibasisF/imultiproc.py
+-rw-rw-r--   0 user      (1000) user      (1000)    12284 2023-06-05 07:39:45.000000 ibasis-0.0.2/ibasis/ibasisF/ipath.py
+-rw-rw-r--   0 user      (1000) user      (1000)      469 2023-05-25 06:21:55.000000 ibasis-0.0.2/ibasis/ibasisF/ipoint.py
+-rw-rw-r--   0 user      (1000) user      (1000)      879 2023-05-25 06:21:55.000000 ibasis-0.0.2/ibasis/ibasisF/iprofile.py
+-rw-rw-r--   0 user      (1000) user      (1000)      196 2023-05-25 06:21:55.000000 ibasis-0.0.2/ibasis/ibasisF/iserialization.py
+-rw-rw-r--   0 user      (1000) user      (1000)      574 2023-05-25 06:21:55.000000 ibasis-0.0.2/ibasis/ibasisF/ishell.py
+-rw-rw-r--   0 user      (1000) user      (1000)     1729 2023-05-25 06:21:55.000000 ibasis-0.0.2/ibasis/ibasisF/itimeutils.py
+-rw-rw-r--   0 user      (1000) user      (1000)     3001 2023-05-25 06:21:55.000000 ibasis-0.0.2/ibasis/ibasisF/itorch.py
+-rw-rw-r--   0 user      (1000) user      (1000)     2360 2023-05-25 06:21:55.000000 ibasis-0.0.2/ibasis/icolor.py
+-rw-rw-r--   0 user      (1000) user      (1000)     3794 2023-05-25 06:21:55.000000 ibasis-0.0.2/ibasis/idraw.py
+-rw-rw-r--   0 user      (1000) user      (1000)     5472 2023-05-25 06:21:55.000000 ibasis-0.0.2/ibasis/idtbs.py
+-rw-rw-r--   0 user      (1000) user      (1000)     1137 2023-05-25 06:21:55.000000 ibasis-0.0.2/ibasis/ifile.py
+-rw-rw-r--   0 user      (1000) user      (1000)      378 2023-05-25 06:21:55.000000 ibasis-0.0.2/ibasis/iformat.py
+-rw-rw-r--   0 user      (1000) user      (1000)     1904 2023-05-25 06:21:55.000000 ibasis-0.0.2/ibasis/iimg.py
+-rw-rw-r--   0 user      (1000) user      (1000)     4660 2023-05-25 06:21:55.000000 ibasis-0.0.2/ibasis/ilmdb.py
+-rw-rw-r--   0 user      (1000) user      (1000)     2939 2023-05-25 08:21:23.000000 ibasis-0.0.2/ibasis/ilog.py
+-rw-rw-r--   0 user      (1000) user      (1000)     2942 2023-05-25 06:21:55.000000 ibasis-0.0.2/ibasis/imath.py
+-rw-rw-r--   0 user      (1000) user      (1000)     2745 2023-05-25 06:21:55.000000 ibasis-0.0.2/ibasis/imetric.py
+-rw-rw-r--   0 user      (1000) user      (1000)     6122 2023-06-02 08:06:29.000000 ibasis-0.0.2/ibasis/imgalg.py
+-rw-rw-r--   0 user      (1000) user      (1000)      439 2023-05-25 06:21:55.000000 ibasis-0.0.2/ibasis/imultiproc.py
+-rw-rw-r--   0 user      (1000) user      (1000)    12284 2023-06-05 07:39:45.000000 ibasis-0.0.2/ibasis/ipath.py
+-rw-rw-r--   0 user      (1000) user      (1000)      469 2023-05-25 06:21:55.000000 ibasis-0.0.2/ibasis/ipoint.py
+-rw-rw-r--   0 user      (1000) user      (1000)      879 2023-05-25 06:21:55.000000 ibasis-0.0.2/ibasis/iprofile.py
+-rw-rw-r--   0 user      (1000) user      (1000)      196 2023-05-25 06:21:55.000000 ibasis-0.0.2/ibasis/iserialization.py
+-rw-rw-r--   0 user      (1000) user      (1000)      574 2023-05-25 06:21:55.000000 ibasis-0.0.2/ibasis/ishell.py
+-rw-rw-r--   0 user      (1000) user      (1000)     1729 2023-05-25 06:21:55.000000 ibasis-0.0.2/ibasis/itimeutils.py
+-rw-rw-r--   0 user      (1000) user      (1000)     3001 2023-05-25 06:21:55.000000 ibasis-0.0.2/ibasis/itorch.py
+drwxrwxr-x   0 user      (1000) user      (1000)        0 2023-06-05 07:39:50.826736 ibasis-0.0.2/ibasis.egg-info/
+-rw-rw-r--   0 user      (1000) user      (1000)      871 2023-06-05 07:39:50.000000 ibasis-0.0.2/ibasis.egg-info/PKG-INFO
+-rw-rw-r--   0 user      (1000) user      (1000)     1257 2023-06-05 07:39:50.000000 ibasis-0.0.2/ibasis.egg-info/SOURCES.txt
+-rw-rw-r--   0 user      (1000) user      (1000)        1 2023-06-05 07:39:50.000000 ibasis-0.0.2/ibasis.egg-info/dependency_links.txt
+-rw-rw-r--   0 user      (1000) user      (1000)        1 2023-06-05 07:39:50.000000 ibasis-0.0.2/ibasis.egg-info/not-zip-safe
+-rw-rw-r--   0 user      (1000) user      (1000)       12 2023-06-05 07:39:50.000000 ibasis-0.0.2/ibasis.egg-info/top_level.txt
+-rw-rw-r--   0 user      (1000) user      (1000)       38 2023-06-05 07:39:50.830736 ibasis-0.0.2/setup.cfg
+-rw-rw-r--   0 user      (1000) user      (1000)     1040 2023-06-05 06:45:55.000000 ibasis-0.0.2/setup.py
+drwxrwxr-x   0 user      (1000) user      (1000)        0 2023-06-05 07:39:50.830736 ibasis-0.0.2/test/
+-rw-rw-r--   0 user      (1000) user      (1000)       19 2023-05-25 06:21:55.000000 ibasis-0.0.2/test/test_import.py
```

### Comparing `ibasis-0.0.1a0/LICENSE` & `ibasis-0.0.2/LICENSE`

 * *Files identical despite different names*

### Comparing `ibasis-0.0.1a0/PKG-INFO` & `ibasis-0.0.2/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ibasis
-Version: 0.0.1a0
+Version: 0.0.2
 Summary: basic functions in coding, include fio, image processing, profile, etc.
 Home-page: https://github.com/AvinsWang/ibasis
 Download-URL: http://pypi.python.org/pypi/ibasis/
 Author: Avins Wang
 Author-email: avinswang@gmail.com
 License: LGPL-3.0
 Keywords: py-itime,python time
```

### Comparing `ibasis-0.0.1a0/ibasis/ibasic.py` & `ibasis-0.0.2/ibasis/ibasic.py`

 * *Files identical despite different names*

### Comparing `ibasis-0.0.1a0/ibasis/ibasisF/ibasic.py` & `ibasis-0.0.2/ibasis/ibasisF/ibasic.py`

 * *Files identical despite different names*

### Comparing `ibasis-0.0.1a0/ibasis/ibasisF/icolor.py` & `ibasis-0.0.2/ibasis/ibasisF/icolor.py`

 * *Files identical despite different names*

### Comparing `ibasis-0.0.1a0/ibasis/ibasisF/idraw.py` & `ibasis-0.0.2/ibasis/ibasisF/idraw.py`

 * *Files identical despite different names*

### Comparing `ibasis-0.0.1a0/ibasis/ibasisF/idtbs.py` & `ibasis-0.0.2/ibasis/ibasisF/idtbs.py`

 * *Files identical despite different names*

### Comparing `ibasis-0.0.1a0/ibasis/ibasisF/ifile.py` & `ibasis-0.0.2/ibasis/ibasisF/ifile.py`

 * *Files identical despite different names*

### Comparing `ibasis-0.0.1a0/ibasis/ibasisF/iimg.py` & `ibasis-0.0.2/ibasis/ibasisF/iimg.py`

 * *Files identical despite different names*

### Comparing `ibasis-0.0.1a0/ibasis/ibasisF/ilmdb.py` & `ibasis-0.0.2/ibasis/ibasisF/ilmdb.py`

 * *Files identical despite different names*

### Comparing `ibasis-0.0.1a0/ibasis/ibasisF/ilog.py` & `ibasis-0.0.2/ibasis/ibasisF/ilog.py`

 * *Files 2% similar despite different names*

```diff
@@ -49,14 +49,20 @@
             self.print(msg, level='INFO')
 
     def warning(self, msg, is_print=False):
         if self._logger is not None:
             self._logger.warning(msg)
         if is_print:
             self.print(msg, level='WARNING')
+    
+    def debug(self, msg, is_print=False):
+        if self._logger is not None:
+            self._logger.debug(msg)
+        if is_print:
+            self.print(msg, level='DEBUG')
 
     def exception(self, e, is_print=False):
         if self._logger is not None:
             self._logger.exception(e)
         if is_print:
             self.print(traceback.format_exc(), level='EXCEPTION')
```

### Comparing `ibasis-0.0.1a0/ibasis/ibasisF/imath.py` & `ibasis-0.0.2/ibasis/ibasisF/imath.py`

 * *Files identical despite different names*

### Comparing `ibasis-0.0.1a0/ibasis/ibasisF/imetric.py` & `ibasis-0.0.2/ibasis/ibasisF/imetric.py`

 * *Files identical despite different names*

### Comparing `ibasis-0.0.1a0/ibasis/ibasisF/imgalg.py` & `ibasis-0.0.2/ibasis/ibasisF/imgalg.py`

 * *Files 25% similar despite different names*

```diff
@@ -1,13 +1,15 @@
 import cv2
 import math
 import traceback
 import numpy as np
 from scipy.spatial import ConvexHull
-from .imath import (to_norm_vec, is_vec_eq, calc_eula_dis, cos2x)
+
+from . import imath
+from . import ipoint
 
 
 def calc_polygon_main_direction(polygon):
     """计算polygon的主方向
 
     Args:
         polygon (list): [[x,y], ...]
@@ -63,28 +65,28 @@
         
     matched = []
     for l, r in search_idxs:
         l1_pt = x_left_lis[l]
         r1_pt = x_right_lis[r]
         l2_pt = x_left_lis[1-l]
         r2_pt = x_right_lis[1-r]
-        v1 = to_norm_vec(r2_pt - l1_pt)
-        v2 = to_norm_vec(r1_pt - l2_pt)
+        v1 = imath.to_norm_vec(r2_pt - l1_pt)
+        v2 = imath.to_norm_vec(r1_pt - l2_pt)
         # 四边形需要修改此处
-        if is_vec_eq(v1, v2, error):
+        if imath.is_vec_eq(v1, v2, error):
             matched = [[l, r], [1-l, 1-r]]
             break
     # 找出lb点
     ld = x_left_lis[0]
     if x_left_lis[1][1] > x_left_lis[0][1]:
         ld = x_left_lis[1]
     # 确定所有点的顺序
     sorted_pts = list()
     for l, r in matched:
-        if is_vec_eq(x_left_lis[l], ld):
+        if imath.is_vec_eq(x_left_lis[l], ld):
             sorted_pts = [
                 x_left_lis[1-l],
                 x_right_lis[r],
                 x_right_lis[1-r],
                 x_left_lis[l]
             ]
             break
@@ -141,10 +143,50 @@
 
 def get_rotate_rect_info(rotate_rect):
     """[lt, rt, rb, lb] 获取(lb-rb) 与x轴夹角, 宽Len(lt, rt), 高Len(lt, rb)"""
     lt, rt, rb, lb = np.array(rotate_rect)
     v_lbrb = rb-lb
     deg = math.degrees(math.acos(cos2x(v_lbrb)))   # 与y轴正方向夹角
     # deg = 90 - deg
-    W = calc_eula_dis(rb, lb)
-    H = calc_eula_dis(lb, lt)
-    return W, H, deg
+    W = imath.calc_eula_dis(rb, lb)
+    H = imath.calc_eula_dis(lb, lt)
+    return W, H, deg
+
+
+def rotate_2D_pts(pts, M):
+    """二维坐标点右乘旋转矩阵->得到变换后的点
+
+    Args:
+        pts (np.array): [[x, y], ...]
+        M (np.array, 2x3): 旋转矩阵, cv2.getRotationMatrix2D()得到
+
+    Returns:
+        np.array: 旋转后的点
+    """
+    homo_pts = np.concatenate([pts, np.ones([pts.shape[0], 1])], -1)
+    return (M[:2] @ homo_pts.T).T
+
+
+def sort_rrect_with_deg(rrect, deg):
+    """将旋转矩形的四个点根据旋转角进行排序
+
+    Args:
+        rrect (np.array): 旋转矩形的四个点
+        deg (float): [0, 360), 注: cv2中是逆时针旋转
+
+    Returns:
+        np.array: 排序后的旋转矩形的四个点, [lt, rt, rb, lb]
+    """
+    rrect = np.array(rrect, dtype=np.float32)
+    center = rrect.mean(axis=0)
+    
+    M = cv2.getRotationMatrix2D(center, deg, 1.0)
+    
+    r_rrect = rotate_2D_pts(rrect, M).astype(np.int32)
+    r_rrect_dic = {pt: i for i, pt in enumerate(ipoint.fmt_2d_pts(r_rrect, is_tuple=True, is_int=True))}
+    order_r_rrect = sort_rotate_rect(r_rrect, error=1)
+    ordered_rrect = np.array([rrect[r_rrect_dic[p]] for p in order_r_rrect], dtype=np.int32)
+    
+    wh = np.array([imath.calc_eula_dis(ordered_rrect[0], ordered_rrect[1]), 
+                    imath.calc_eula_dis(ordered_rrect[1], ordered_rrect[2])])
+
+    return ordered_rrect, wh.astype(np.int32)
```

### Comparing `ibasis-0.0.1a0/ibasis/ibasisF/ipath.py` & `ibasis-0.0.2/ibasis/ibasisF/ipath.py`

 * *Files 0% similar despite different names*

```diff
@@ -306,15 +306,15 @@
 def get_dataset_pair(dir1, dir2, file_type1=None, file_type2=None, key_mode1=0, key_mode2=0,
                      stem_append1=None, stem_append2=None, is_sort=True, is_lis=False):
     print('获取路径下配对文件:')
     print('dir1:', dir1)
     print('dir2:', dir2)
     img_path_dic = get_paths(dir1, file_type=file_type1, key_mode=key_mode1, stem_append=stem_append1)
     lbl_path_dic = get_paths(dir2, file_type=file_type2, key_mode=key_mode2, stem_append=stem_append2)
-    inter_keys = basic.get_intersection_keys(img_path_dic, lbl_path_dic, is_sort=is_sort)
+    inter_keys = ibasic.get_intersection_keys(img_path_dic, lbl_path_dic, is_sort=is_sort)
     if is_lis:
         return [[k, img_path_dic[k], lbl_path_dic[k]] for k in inter_keys]
     else:
         for key in inter_keys:
             yield [key, img_path_dic.get(key), lbl_path_dic.get(key)]
```

### Comparing `ibasis-0.0.1a0/ibasis/ibasisF/iprofile.py` & `ibasis-0.0.2/ibasis/ibasisF/iprofile.py`

 * *Files identical despite different names*

### Comparing `ibasis-0.0.1a0/ibasis/ibasisF/ishell.py` & `ibasis-0.0.2/ibasis/ibasisF/ishell.py`

 * *Files identical despite different names*

### Comparing `ibasis-0.0.1a0/ibasis/ibasisF/itimeutils.py` & `ibasis-0.0.2/ibasis/ibasisF/itimeutils.py`

 * *Files identical despite different names*

### Comparing `ibasis-0.0.1a0/ibasis/ibasisF/itorch.py` & `ibasis-0.0.2/ibasis/ibasisF/itorch.py`

 * *Files identical despite different names*

### Comparing `ibasis-0.0.1a0/ibasis/icolor.py` & `ibasis-0.0.2/ibasis/icolor.py`

 * *Files identical despite different names*

### Comparing `ibasis-0.0.1a0/ibasis/idraw.py` & `ibasis-0.0.2/ibasis/idraw.py`

 * *Files identical despite different names*

### Comparing `ibasis-0.0.1a0/ibasis/idtbs.py` & `ibasis-0.0.2/ibasis/idtbs.py`

 * *Files identical despite different names*

### Comparing `ibasis-0.0.1a0/ibasis/ifile.py` & `ibasis-0.0.2/ibasis/ifile.py`

 * *Files identical despite different names*

### Comparing `ibasis-0.0.1a0/ibasis/iimg.py` & `ibasis-0.0.2/ibasis/iimg.py`

 * *Files identical despite different names*

### Comparing `ibasis-0.0.1a0/ibasis/ilmdb.py` & `ibasis-0.0.2/ibasis/ilmdb.py`

 * *Files identical despite different names*

### Comparing `ibasis-0.0.1a0/ibasis/ilog.py` & `ibasis-0.0.2/ibasis/ilog.py`

 * *Files 2% similar despite different names*

```diff
@@ -49,14 +49,20 @@
             self.print(msg, level='INFO')
 
     def warning(self, msg, is_print=False):
         if self._logger is not None:
             self._logger.warning(msg)
         if is_print:
             self.print(msg, level='WARNING')
+    
+    def debug(self, msg, is_print=False):
+        if self._logger is not None:
+            self._logger.debug(msg)
+        if is_print:
+            self.print(msg, level='DEBUG')
 
     def exception(self, e, is_print=False):
         if self._logger is not None:
             self._logger.exception(e)
         if is_print:
             self.print(traceback.format_exc(), level='EXCEPTION')
```

### Comparing `ibasis-0.0.1a0/ibasis/imath.py` & `ibasis-0.0.2/ibasis/imath.py`

 * *Files identical despite different names*

### Comparing `ibasis-0.0.1a0/ibasis/imetric.py` & `ibasis-0.0.2/ibasis/imetric.py`

 * *Files identical despite different names*

### Comparing `ibasis-0.0.1a0/ibasis/imgalg.py` & `ibasis-0.0.2/ibasis/imgalg.py`

 * *Files 25% similar despite different names*

```diff
@@ -1,13 +1,15 @@
 import cv2
 import math
 import traceback
 import numpy as np
 from scipy.spatial import ConvexHull
-from .imath import (to_norm_vec, is_vec_eq, calc_eula_dis, cos2x)
+
+from . import imath
+from . import ipoint
 
 
 def calc_polygon_main_direction(polygon):
     """计算polygon的主方向
 
     Args:
         polygon (list): [[x,y], ...]
@@ -63,28 +65,28 @@
         
     matched = []
     for l, r in search_idxs:
         l1_pt = x_left_lis[l]
         r1_pt = x_right_lis[r]
         l2_pt = x_left_lis[1-l]
         r2_pt = x_right_lis[1-r]
-        v1 = to_norm_vec(r2_pt - l1_pt)
-        v2 = to_norm_vec(r1_pt - l2_pt)
+        v1 = imath.to_norm_vec(r2_pt - l1_pt)
+        v2 = imath.to_norm_vec(r1_pt - l2_pt)
         # 四边形需要修改此处
-        if is_vec_eq(v1, v2, error):
+        if imath.is_vec_eq(v1, v2, error):
             matched = [[l, r], [1-l, 1-r]]
             break
     # 找出lb点
     ld = x_left_lis[0]
     if x_left_lis[1][1] > x_left_lis[0][1]:
         ld = x_left_lis[1]
     # 确定所有点的顺序
     sorted_pts = list()
     for l, r in matched:
-        if is_vec_eq(x_left_lis[l], ld):
+        if imath.is_vec_eq(x_left_lis[l], ld):
             sorted_pts = [
                 x_left_lis[1-l],
                 x_right_lis[r],
                 x_right_lis[1-r],
                 x_left_lis[l]
             ]
             break
@@ -141,10 +143,50 @@
 
 def get_rotate_rect_info(rotate_rect):
     """[lt, rt, rb, lb] 获取(lb-rb) 与x轴夹角, 宽Len(lt, rt), 高Len(lt, rb)"""
     lt, rt, rb, lb = np.array(rotate_rect)
     v_lbrb = rb-lb
     deg = math.degrees(math.acos(cos2x(v_lbrb)))   # 与y轴正方向夹角
     # deg = 90 - deg
-    W = calc_eula_dis(rb, lb)
-    H = calc_eula_dis(lb, lt)
-    return W, H, deg
+    W = imath.calc_eula_dis(rb, lb)
+    H = imath.calc_eula_dis(lb, lt)
+    return W, H, deg
+
+
+def rotate_2D_pts(pts, M):
+    """二维坐标点右乘旋转矩阵->得到变换后的点
+
+    Args:
+        pts (np.array): [[x, y], ...]
+        M (np.array, 2x3): 旋转矩阵, cv2.getRotationMatrix2D()得到
+
+    Returns:
+        np.array: 旋转后的点
+    """
+    homo_pts = np.concatenate([pts, np.ones([pts.shape[0], 1])], -1)
+    return (M[:2] @ homo_pts.T).T
+
+
+def sort_rrect_with_deg(rrect, deg):
+    """将旋转矩形的四个点根据旋转角进行排序
+
+    Args:
+        rrect (np.array): 旋转矩形的四个点
+        deg (float): [0, 360), 注: cv2中是逆时针旋转
+
+    Returns:
+        np.array: 排序后的旋转矩形的四个点, [lt, rt, rb, lb]
+    """
+    rrect = np.array(rrect, dtype=np.float32)
+    center = rrect.mean(axis=0)
+    
+    M = cv2.getRotationMatrix2D(center, deg, 1.0)
+    
+    r_rrect = rotate_2D_pts(rrect, M).astype(np.int32)
+    r_rrect_dic = {pt: i for i, pt in enumerate(ipoint.fmt_2d_pts(r_rrect, is_tuple=True, is_int=True))}
+    order_r_rrect = sort_rotate_rect(r_rrect, error=1)
+    ordered_rrect = np.array([rrect[r_rrect_dic[p]] for p in order_r_rrect], dtype=np.int32)
+    
+    wh = np.array([imath.calc_eula_dis(ordered_rrect[0], ordered_rrect[1]), 
+                    imath.calc_eula_dis(ordered_rrect[1], ordered_rrect[2])])
+
+    return ordered_rrect, wh.astype(np.int32)
```

### Comparing `ibasis-0.0.1a0/ibasis/ipath.py` & `ibasis-0.0.2/ibasis/ipath.py`

 * *Files 0% similar despite different names*

```diff
@@ -306,15 +306,15 @@
 def get_dataset_pair(dir1, dir2, file_type1=None, file_type2=None, key_mode1=0, key_mode2=0,
                      stem_append1=None, stem_append2=None, is_sort=True, is_lis=False):
     print('获取路径下配对文件:')
     print('dir1:', dir1)
     print('dir2:', dir2)
     img_path_dic = get_paths(dir1, file_type=file_type1, key_mode=key_mode1, stem_append=stem_append1)
     lbl_path_dic = get_paths(dir2, file_type=file_type2, key_mode=key_mode2, stem_append=stem_append2)
-    inter_keys = basic.get_intersection_keys(img_path_dic, lbl_path_dic, is_sort=is_sort)
+    inter_keys = ibasic.get_intersection_keys(img_path_dic, lbl_path_dic, is_sort=is_sort)
     if is_lis:
         return [[k, img_path_dic[k], lbl_path_dic[k]] for k in inter_keys]
     else:
         for key in inter_keys:
             yield [key, img_path_dic.get(key), lbl_path_dic.get(key)]
```

### Comparing `ibasis-0.0.1a0/ibasis/iprofile.py` & `ibasis-0.0.2/ibasis/iprofile.py`

 * *Files identical despite different names*

### Comparing `ibasis-0.0.1a0/ibasis/ishell.py` & `ibasis-0.0.2/ibasis/ishell.py`

 * *Files identical despite different names*

### Comparing `ibasis-0.0.1a0/ibasis/itimeutils.py` & `ibasis-0.0.2/ibasis/itimeutils.py`

 * *Files identical despite different names*

### Comparing `ibasis-0.0.1a0/ibasis/itorch.py` & `ibasis-0.0.2/ibasis/itorch.py`

 * *Files identical despite different names*

### Comparing `ibasis-0.0.1a0/ibasis.egg-info/PKG-INFO` & `ibasis-0.0.2/ibasis.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ibasis
-Version: 0.0.1a0
+Version: 0.0.2
 Summary: basic functions in coding, include fio, image processing, profile, etc.
 Home-page: https://github.com/AvinsWang/ibasis
 Download-URL: http://pypi.python.org/pypi/ibasis/
 Author: Avins Wang
 Author-email: avinswang@gmail.com
 License: LGPL-3.0
 Keywords: py-itime,python time
```

### Comparing `ibasis-0.0.1a0/setup.py` & `ibasis-0.0.2/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 import os
 from setuptools import setup, find_packages
 
 here = os.path.abspath(os.path.dirname(__file__))
 
 setup(
     name='ibasis',
-    version='0.0.1a0',
+    version='0.0.2',
     author='Avins Wang',
     author_email='avinswang@gmail.com',
     url='https://github.com/AvinsWang/ibasis',
     download_url="http://pypi.python.org/pypi/ibasis/",
     description="basic functions in coding, include fio, image processing, profile, etc.",
     long_description=open(os.path.join(here, 'README.md')).read(),
     license='LGPL-3.0',
```

