# Comparing `tmp/autodistill-sam-clip-0.0.1.tar.gz` & `tmp/autodistill-sam-clip-0.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "autodistill-sam-clip-0.0.1.tar", last modified: Wed Jun  7 13:17:22 2023, max compression
+gzip compressed data, was "autodistill-sam-clip-0.1.1.tar", last modified: Mon Jun 12 08:32:57 2023, max compression
```

## Comparing `autodistill-sam-clip-0.0.1.tar` & `autodistill-sam-clip-0.1.1.tar`

### file list

```diff
@@ -1,13 +1,16 @@
-drwxr-xr-x   0 james      (501) staff       (20)        0 2023-06-07 13:17:22.103003 autodistill-sam-clip-0.0.1/
--rw-r--r--   0 james      (501) staff       (20)      903 2023-06-07 13:17:22.102870 autodistill-sam-clip-0.0.1/PKG-INFO
--rw-r--r--   0 james      (501) staff       (20)      556 2023-06-07 13:17:20.000000 autodistill-sam-clip-0.0.1/README.md
-drwxr-xr-x   0 james      (501) staff       (20)        0 2023-06-07 13:17:22.101702 autodistill-sam-clip-0.0.1/autodistill_sam_clip/
--rw-r--r--   0 james      (501) staff       (20)       44 2023-06-07 13:17:20.000000 autodistill-sam-clip-0.0.1/autodistill_sam_clip/__init__.py
-drwxr-xr-x   0 james      (501) staff       (20)        0 2023-06-07 13:17:22.102670 autodistill-sam-clip-0.0.1/autodistill_sam_clip.egg-info/
--rw-r--r--   0 james      (501) staff       (20)      903 2023-06-07 13:17:22.000000 autodistill-sam-clip-0.0.1/autodistill_sam_clip.egg-info/PKG-INFO
--rw-r--r--   0 james      (501) staff       (20)      270 2023-06-07 13:17:22.000000 autodistill-sam-clip-0.0.1/autodistill_sam_clip.egg-info/SOURCES.txt
--rw-r--r--   0 james      (501) staff       (20)        1 2023-06-07 13:17:22.000000 autodistill-sam-clip-0.0.1/autodistill_sam_clip.egg-info/dependency_links.txt
--rw-r--r--   0 james      (501) staff       (20)       53 2023-06-07 13:17:22.000000 autodistill-sam-clip-0.0.1/autodistill_sam_clip.egg-info/requires.txt
--rw-r--r--   0 james      (501) staff       (20)       21 2023-06-07 13:17:22.000000 autodistill-sam-clip-0.0.1/autodistill_sam_clip.egg-info/top_level.txt
--rw-r--r--   0 james      (501) staff       (20)       38 2023-06-07 13:17:22.103051 autodistill-sam-clip-0.0.1/setup.cfg
--rw-r--r--   0 james      (501) staff       (20)      985 2023-06-07 13:17:20.000000 autodistill-sam-clip-0.0.1/setup.py
+drwxr-xr-x   0 james      (501) staff       (20)        0 2023-06-12 08:32:57.401580 autodistill-sam-clip-0.1.1/
+-rw-r--r--   0 james      (501) staff       (20)    11356 2023-06-09 18:33:41.000000 autodistill-sam-clip-0.1.1/LICENSE
+-rw-r--r--   0 james      (501) staff       (20)      479 2023-06-12 08:32:57.401338 autodistill-sam-clip-0.1.1/PKG-INFO
+-rw-r--r--   0 james      (501) staff       (20)     1884 2023-06-09 18:57:56.000000 autodistill-sam-clip-0.1.1/README.md
+drwxr-xr-x   0 james      (501) staff       (20)        0 2023-06-12 08:32:57.399587 autodistill-sam-clip-0.1.1/autodistill_sam_clip/
+-rw-r--r--   0 james      (501) staff       (20)       73 2023-06-09 18:45:16.000000 autodistill-sam-clip-0.1.1/autodistill_sam_clip/__init__.py
+-rw-r--r--   0 james      (501) staff       (20)     2798 2023-06-12 08:32:31.000000 autodistill-sam-clip-0.1.1/autodistill_sam_clip/helpers.py
+-rw-r--r--   0 james      (501) staff       (20)     5206 2023-06-12 08:29:22.000000 autodistill-sam-clip-0.1.1/autodistill_sam_clip/sam_clip.py
+drwxr-xr-x   0 james      (501) staff       (20)        0 2023-06-12 08:32:57.401024 autodistill-sam-clip-0.1.1/autodistill_sam_clip.egg-info/
+-rw-r--r--   0 james      (501) staff       (20)      479 2023-06-12 08:32:57.000000 autodistill-sam-clip-0.1.1/autodistill_sam_clip.egg-info/PKG-INFO
+-rw-r--r--   0 james      (501) staff       (20)      343 2023-06-12 08:32:57.000000 autodistill-sam-clip-0.1.1/autodistill_sam_clip.egg-info/SOURCES.txt
+-rw-r--r--   0 james      (501) staff       (20)        1 2023-06-12 08:32:57.000000 autodistill-sam-clip-0.1.1/autodistill_sam_clip.egg-info/dependency_links.txt
+-rw-r--r--   0 james      (501) staff       (20)      138 2023-06-12 08:32:57.000000 autodistill-sam-clip-0.1.1/autodistill_sam_clip.egg-info/requires.txt
+-rw-r--r--   0 james      (501) staff       (20)       21 2023-06-12 08:32:57.000000 autodistill-sam-clip-0.1.1/autodistill_sam_clip.egg-info/top_level.txt
+-rw-r--r--   0 james      (501) staff       (20)       38 2023-06-12 08:32:57.401656 autodistill-sam-clip-0.1.1/setup.cfg
+-rw-r--r--   0 james      (501) staff       (20)     1469 2023-06-12 08:32:01.000000 autodistill-sam-clip-0.1.1/setup.py
```

