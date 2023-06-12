# Comparing `tmp/zhousf-lib-0.6.7.tar.gz` & `tmp/zhousf-lib-0.6.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "zhousf-lib-0.6.7.tar", last modified: Mon Jun 12 03:00:40 2023, max compression
+gzip compressed data, was "zhousf-lib-0.6.8.tar", last modified: Mon Jun 12 03:16:25 2023, max compression
```

## Comparing `zhousf-lib-0.6.7.tar` & `zhousf-lib-0.6.8.tar`

### file list

```diff
@@ -1,78 +1,77 @@
-drwxrwxrwx   0        0        0        0 2023-06-12 03:00:40.446520 zhousf-lib-0.6.7/
--rw-rw-rw-   0        0        0     1086 2023-06-06 02:24:10.000000 zhousf-lib-0.6.7/LICENSE
--rw-rw-rw-   0        0        0     2073 2023-06-12 03:00:40.446520 zhousf-lib-0.6.7/PKG-INFO
--rw-rw-rw-   0        0        0     1179 2023-06-09 06:54:16.000000 zhousf-lib-0.6.7/README.md
--rw-rw-rw-   0        0        0       42 2023-06-12 03:00:40.447519 zhousf-lib-0.6.7/setup.cfg
--rw-rw-rw-   0        0        0     4289 2023-06-12 03:00:36.000000 zhousf-lib-0.6.7/setup.py
-drwxrwxrwx   0        0        0        0 2023-06-12 03:00:40.378520 zhousf-lib-0.6.7/zhousf_lib.egg-info/
--rw-rw-rw-   0        0        0     2073 2023-06-12 03:00:40.000000 zhousf-lib-0.6.7/zhousf_lib.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0     1962 2023-06-12 03:00:40.000000 zhousf-lib-0.6.7/zhousf_lib.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-06-12 03:00:40.000000 zhousf-lib-0.6.7/zhousf_lib.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       14 2023-06-12 03:00:40.000000 zhousf-lib-0.6.7/zhousf_lib.egg-info/requires.txt
--rw-rw-rw-   0        0        0       10 2023-06-12 03:00:40.000000 zhousf-lib-0.6.7/zhousf_lib.egg-info/top_level.txt
-drwxrwxrwx   0        0        0        0 2023-06-12 03:00:40.379518 zhousf-lib-0.6.7/zhousflib/
--rw-rw-rw-   0        0        0       60 2023-06-07 01:49:13.000000 zhousf-lib-0.6.7/zhousflib/__init__.py
-drwxrwxrwx   0        0        0        0 2023-06-12 03:00:40.380519 zhousf-lib-0.6.7/zhousflib/datasets/
--rw-rw-rw-   0        0        0       84 2023-06-06 02:39:10.000000 zhousf-lib-0.6.7/zhousflib/datasets/__init__.py
-drwxrwxrwx   0        0        0        0 2023-06-12 03:00:40.382519 zhousf-lib-0.6.7/zhousflib/datasets/classification/
--rw-rw-rw-   0        0        0       73 2023-06-07 01:45:12.000000 zhousf-lib-0.6.7/zhousflib/datasets/classification/__init__.py
--rw-rw-rw-   0        0        0     2937 2023-06-09 06:13:45.000000 zhousf-lib-0.6.7/zhousflib/datasets/classification/classification_dataset_split.py
-drwxrwxrwx   0        0        0        0 2023-06-12 03:00:40.387519 zhousf-lib-0.6.7/zhousflib/datasets/coco/
--rw-rw-rw-   0        0        0       60 2023-06-07 01:45:12.000000 zhousf-lib-0.6.7/zhousflib/datasets/coco/__init__.py
--rw-rw-rw-   0        0        0     8251 2023-06-07 07:58:31.000000 zhousf-lib-0.6.7/zhousflib/datasets/coco/coco_bbox_extract.py
--rw-rw-rw-   0        0        0     5464 2023-06-07 07:56:06.000000 zhousf-lib-0.6.7/zhousflib/datasets/coco/coco_bbox_update.py
--rw-rw-rw-   0        0        0     6637 2023-06-08 02:33:01.000000 zhousf-lib-0.6.7/zhousflib/datasets/coco/coco_bbox_vis.py
--rw-rw-rw-   0        0        0     2896 2023-06-07 07:55:47.000000 zhousf-lib-0.6.7/zhousflib/datasets/coco/coco_dataset_merge.py
--rw-rw-rw-   0        0        0     6278 2023-06-09 06:13:45.000000 zhousf-lib-0.6.7/zhousflib/datasets/coco/coco_dataset_split.py
-drwxrwxrwx   0        0        0        0 2023-06-12 03:00:40.393518 zhousf-lib-0.6.7/zhousflib/datasets/labelme/
--rw-rw-rw-   0        0        0       60 2023-06-07 01:45:12.000000 zhousf-lib-0.6.7/zhousflib/datasets/labelme/__init__.py
--rw-rw-rw-   0        0        0     3825 2023-06-07 01:45:12.000000 zhousf-lib-0.6.7/zhousflib/datasets/labelme/labelme_clip.py
--rw-rw-rw-   0        0        0     8090 2023-06-07 01:45:12.000000 zhousf-lib-0.6.7/zhousflib/datasets/labelme/labelme_convert_coco.py
--rw-rw-rw-   0        0        0     9622 2023-06-06 09:07:37.000000 zhousf-lib-0.6.7/zhousflib/datasets/labelme/labelme_convert_seg.py
--rw-rw-rw-   0        0        0     3827 2023-06-07 01:45:12.000000 zhousf-lib-0.6.7/zhousflib/datasets/labelme/labelme_dataset_clip.py
-drwxrwxrwx   0        0        0        0 2023-06-12 03:00:40.396551 zhousf-lib-0.6.7/zhousflib/datasets/segmentation/
--rw-rw-rw-   0        0        0       60 2023-06-07 01:45:12.000000 zhousf-lib-0.6.7/zhousflib/datasets/segmentation/__init__.py
--rw-rw-rw-   0        0        0     2871 2023-06-06 09:07:37.000000 zhousf-lib-0.6.7/zhousflib/datasets/segmentation/seg_dataset_split.py
-drwxrwxrwx   0        0        0        0 2023-06-12 03:00:40.398548 zhousf-lib-0.6.7/zhousflib/db/
--rw-rw-rw-   0        0        0       62 2023-06-08 02:33:01.000000 zhousf-lib-0.6.7/zhousflib/db/__init__.py
--rw-rw-rw-   0        0        0     2345 2023-06-09 06:00:56.000000 zhousf-lib-0.6.7/zhousflib/db/lmdb_master.py
-drwxrwxrwx   0        0        0        0 2023-06-12 03:00:40.401520 zhousf-lib-0.6.7/zhousflib/decorator/
--rw-rw-rw-   0        0        0       60 2023-06-07 01:45:12.000000 zhousf-lib-0.6.7/zhousflib/decorator/__init__.py
--rw-rw-rw-   0        0        0      466 2023-06-07 01:49:12.000000 zhousf-lib-0.6.7/zhousflib/decorator/except_util.py
--rw-rw-rw-   0        0        0     1094 2023-06-07 01:49:12.000000 zhousf-lib-0.6.7/zhousflib/decorator/interceptor_util.py
-drwxrwxrwx   0        0        0        0 2023-06-12 03:00:40.416561 zhousf-lib-0.6.7/zhousflib/font/
--rw-rw-rw-   0        0        0 15320040 2023-03-31 01:19:09.000000 zhousf-lib-0.6.7/zhousflib/font/SimSun.ttf
--rw-rw-rw-   0        0        0  2152796 2023-03-31 01:19:09.000000 zhousf-lib-0.6.7/zhousflib/font/Symbola.ttf
--rw-rw-rw-   0        0        0      763 2023-06-09 05:53:49.000000 zhousf-lib-0.6.7/zhousflib/font/__init__.py
-drwxrwxrwx   0        0        0        0 2023-06-12 03:00:40.418520 zhousf-lib-0.6.7/zhousflib/locust/
--rw-rw-rw-   0        0        0       60 2023-06-07 01:49:12.000000 zhousf-lib-0.6.7/zhousflib/locust/__init__.py
--rw-rw-rw-   0        0        0     1544 2023-06-09 06:20:55.000000 zhousf-lib-0.6.7/zhousflib/locust/locust_demo.py
-drwxrwxrwx   0        0        0        0 2023-06-12 03:00:40.421520 zhousf-lib-0.6.7/zhousflib/pandas/
--rw-rw-rw-   0        0        0       60 2023-06-07 01:49:13.000000 zhousf-lib-0.6.7/zhousflib/pandas/__init__.py
--rw-rw-rw-   0        0        0     3143 2023-06-12 02:53:40.000000 zhousf-lib-0.6.7/zhousflib/pandas/openpyxl_util.py
--rw-rw-rw-   0        0        0     5598 2023-06-12 02:57:59.000000 zhousf-lib-0.6.7/zhousflib/pandas/pandas_util.py
-drwxrwxrwx   0        0        0        0 2023-06-12 03:00:40.424518 zhousf-lib-0.6.7/zhousflib/pdf/
--rw-rw-rw-   0        0        0       60 2023-06-07 01:49:12.000000 zhousf-lib-0.6.7/zhousflib/pdf/__init__.py
--rw-rw-rw-   0        0        0     1845 2023-06-07 01:49:12.000000 zhousf-lib-0.6.7/zhousflib/pdf/export_image.py
--rw-rw-rw-   0        0        0     1467 2023-06-08 02:34:30.000000 zhousf-lib-0.6.7/zhousflib/pdf/pdfplumber_util.py
-drwxrwxrwx   0        0        0        0 2023-06-12 03:00:40.439520 zhousf-lib-0.6.7/zhousflib/util/
--rw-rw-rw-   0        0        0       60 2023-06-07 01:49:12.000000 zhousf-lib-0.6.7/zhousflib/util/__init__.py
--rw-rw-rw-   0        0        0     2770 2023-06-07 01:49:13.000000 zhousf-lib-0.6.7/zhousflib/util/calculater_util.py
--rw-rw-rw-   0        0        0      635 2023-06-07 01:49:12.000000 zhousf-lib-0.6.7/zhousflib/util/cv_util.py
--rw-rw-rw-   0        0        0     2193 2023-06-07 01:49:13.000000 zhousf-lib-0.6.7/zhousflib/util/encrypt_util.py
--rw-rw-rw-   0        0        0     1336 2023-06-07 01:49:12.000000 zhousf-lib-0.6.7/zhousflib/util/img_util.py
--rw-rw-rw-   0        0        0    12930 2023-06-07 01:49:12.000000 zhousf-lib-0.6.7/zhousflib/util/iou_util.py
--rw-rw-rw-   0        0        0     3373 2023-06-07 01:49:12.000000 zhousf-lib-0.6.7/zhousflib/util/json_util.py
--rw-rw-rw-   0        0        0      472 2023-06-07 01:49:13.000000 zhousf-lib-0.6.7/zhousflib/util/list_util.py
--rw-rw-rw-   0        0        0     1358 2023-06-07 01:49:12.000000 zhousf-lib-0.6.7/zhousflib/util/permission_util.py
--rw-rw-rw-   0        0        0     3524 2023-06-07 01:49:11.000000 zhousf-lib-0.6.7/zhousflib/util/poly_util.py
--rw-rw-rw-   0        0        0      633 2023-06-07 01:49:12.000000 zhousf-lib-0.6.7/zhousflib/util/re_util.py
--rw-rw-rw-   0        0        0      520 2023-06-07 01:49:12.000000 zhousf-lib-0.6.7/zhousflib/util/singleton.py
--rw-rw-rw-   0        0        0     4246 2023-06-09 06:46:55.000000 zhousf-lib-0.6.7/zhousflib/util/string_util.py
--rw-rw-rw-   0        0        0     4663 2023-06-07 01:49:11.000000 zhousf-lib-0.6.7/zhousflib/util/time_util.py
-drwxrwxrwx   0        0        0        0 2023-06-12 03:00:40.445519 zhousf-lib-0.6.7/zhousflib/web/
--rw-rw-rw-   0        0        0       60 2023-06-07 01:49:12.000000 zhousf-lib-0.6.7/zhousflib/web/__init__.py
--rw-rw-rw-   0        0        0     4355 2023-06-07 01:49:13.000000 zhousf-lib-0.6.7/zhousflib/web/config.py
--rw-rw-rw-   0        0        0     3105 2023-06-07 01:49:12.000000 zhousf-lib-0.6.7/zhousflib/web/log_util.py
--rw-rw-rw-   0        0        0     2860 2023-06-07 01:49:13.000000 zhousf-lib-0.6.7/zhousflib/web/logger.py
--rw-rw-rw-   0        0        0     1340 2023-06-07 01:49:13.000000 zhousf-lib-0.6.7/zhousflib/web/response.py
+drwxrwxrwx   0        0        0        0 2023-06-12 03:16:25.366842 zhousf-lib-0.6.8/
+-rw-rw-rw-   0        0        0     1086 2023-06-06 02:24:10.000000 zhousf-lib-0.6.8/LICENSE
+-rw-rw-rw-   0        0        0     2073 2023-06-12 03:16:25.366842 zhousf-lib-0.6.8/PKG-INFO
+-rw-rw-rw-   0        0        0     1179 2023-06-09 06:54:16.000000 zhousf-lib-0.6.8/README.md
+-rw-rw-rw-   0        0        0       42 2023-06-12 03:16:25.366842 zhousf-lib-0.6.8/setup.cfg
+-rw-rw-rw-   0        0        0     4289 2023-06-12 03:16:19.000000 zhousf-lib-0.6.8/setup.py
+drwxrwxrwx   0        0        0        0 2023-06-12 03:16:25.297239 zhousf-lib-0.6.8/zhousf_lib.egg-info/
+-rw-rw-rw-   0        0        0     2073 2023-06-12 03:16:25.000000 zhousf-lib-0.6.8/zhousf_lib.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0     1929 2023-06-12 03:16:25.000000 zhousf-lib-0.6.8/zhousf_lib.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-06-12 03:16:25.000000 zhousf-lib-0.6.8/zhousf_lib.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       10 2023-06-12 03:16:25.000000 zhousf-lib-0.6.8/zhousf_lib.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-06-12 03:16:25.298834 zhousf-lib-0.6.8/zhousflib/
+-rw-rw-rw-   0        0        0       60 2023-06-07 01:49:13.000000 zhousf-lib-0.6.8/zhousflib/__init__.py
+drwxrwxrwx   0        0        0        0 2023-06-12 03:16:25.299840 zhousf-lib-0.6.8/zhousflib/datasets/
+-rw-rw-rw-   0        0        0       84 2023-06-06 02:39:10.000000 zhousf-lib-0.6.8/zhousflib/datasets/__init__.py
+drwxrwxrwx   0        0        0        0 2023-06-12 03:16:25.301840 zhousf-lib-0.6.8/zhousflib/datasets/classification/
+-rw-rw-rw-   0        0        0       73 2023-06-07 01:45:12.000000 zhousf-lib-0.6.8/zhousflib/datasets/classification/__init__.py
+-rw-rw-rw-   0        0        0     2937 2023-06-09 06:13:45.000000 zhousf-lib-0.6.8/zhousflib/datasets/classification/classification_dataset_split.py
+drwxrwxrwx   0        0        0        0 2023-06-12 03:16:25.308840 zhousf-lib-0.6.8/zhousflib/datasets/coco/
+-rw-rw-rw-   0        0        0       60 2023-06-07 01:45:12.000000 zhousf-lib-0.6.8/zhousflib/datasets/coco/__init__.py
+-rw-rw-rw-   0        0        0     8251 2023-06-07 07:58:31.000000 zhousf-lib-0.6.8/zhousflib/datasets/coco/coco_bbox_extract.py
+-rw-rw-rw-   0        0        0     5464 2023-06-07 07:56:06.000000 zhousf-lib-0.6.8/zhousflib/datasets/coco/coco_bbox_update.py
+-rw-rw-rw-   0        0        0     6637 2023-06-08 02:33:01.000000 zhousf-lib-0.6.8/zhousflib/datasets/coco/coco_bbox_vis.py
+-rw-rw-rw-   0        0        0     2896 2023-06-07 07:55:47.000000 zhousf-lib-0.6.8/zhousflib/datasets/coco/coco_dataset_merge.py
+-rw-rw-rw-   0        0        0     6278 2023-06-09 06:13:45.000000 zhousf-lib-0.6.8/zhousflib/datasets/coco/coco_dataset_split.py
+drwxrwxrwx   0        0        0        0 2023-06-12 03:16:25.314841 zhousf-lib-0.6.8/zhousflib/datasets/labelme/
+-rw-rw-rw-   0        0        0       60 2023-06-07 01:45:12.000000 zhousf-lib-0.6.8/zhousflib/datasets/labelme/__init__.py
+-rw-rw-rw-   0        0        0     3825 2023-06-07 01:45:12.000000 zhousf-lib-0.6.8/zhousflib/datasets/labelme/labelme_clip.py
+-rw-rw-rw-   0        0        0     8090 2023-06-07 01:45:12.000000 zhousf-lib-0.6.8/zhousflib/datasets/labelme/labelme_convert_coco.py
+-rw-rw-rw-   0        0        0     9622 2023-06-06 09:07:37.000000 zhousf-lib-0.6.8/zhousflib/datasets/labelme/labelme_convert_seg.py
+-rw-rw-rw-   0        0        0     3827 2023-06-07 01:45:12.000000 zhousf-lib-0.6.8/zhousflib/datasets/labelme/labelme_dataset_clip.py
+drwxrwxrwx   0        0        0        0 2023-06-12 03:16:25.316840 zhousf-lib-0.6.8/zhousflib/datasets/segmentation/
+-rw-rw-rw-   0        0        0       60 2023-06-07 01:45:12.000000 zhousf-lib-0.6.8/zhousflib/datasets/segmentation/__init__.py
+-rw-rw-rw-   0        0        0     2871 2023-06-06 09:07:37.000000 zhousf-lib-0.6.8/zhousflib/datasets/segmentation/seg_dataset_split.py
+drwxrwxrwx   0        0        0        0 2023-06-12 03:16:25.318842 zhousf-lib-0.6.8/zhousflib/db/
+-rw-rw-rw-   0        0        0       62 2023-06-08 02:33:01.000000 zhousf-lib-0.6.8/zhousflib/db/__init__.py
+-rw-rw-rw-   0        0        0     2345 2023-06-09 06:00:56.000000 zhousf-lib-0.6.8/zhousflib/db/lmdb_master.py
+drwxrwxrwx   0        0        0        0 2023-06-12 03:16:25.321841 zhousf-lib-0.6.8/zhousflib/decorator/
+-rw-rw-rw-   0        0        0       60 2023-06-07 01:45:12.000000 zhousf-lib-0.6.8/zhousflib/decorator/__init__.py
+-rw-rw-rw-   0        0        0      466 2023-06-07 01:49:12.000000 zhousf-lib-0.6.8/zhousflib/decorator/except_util.py
+-rw-rw-rw-   0        0        0     1094 2023-06-07 01:49:12.000000 zhousf-lib-0.6.8/zhousflib/decorator/interceptor_util.py
+drwxrwxrwx   0        0        0        0 2023-06-12 03:16:25.337840 zhousf-lib-0.6.8/zhousflib/font/
+-rw-rw-rw-   0        0        0 15320040 2023-03-31 01:19:09.000000 zhousf-lib-0.6.8/zhousflib/font/SimSun.ttf
+-rw-rw-rw-   0        0        0  2152796 2023-03-31 01:19:09.000000 zhousf-lib-0.6.8/zhousflib/font/Symbola.ttf
+-rw-rw-rw-   0        0        0      763 2023-06-09 05:53:49.000000 zhousf-lib-0.6.8/zhousflib/font/__init__.py
+drwxrwxrwx   0        0        0        0 2023-06-12 03:16:25.339841 zhousf-lib-0.6.8/zhousflib/locust/
+-rw-rw-rw-   0        0        0       60 2023-06-07 01:49:12.000000 zhousf-lib-0.6.8/zhousflib/locust/__init__.py
+-rw-rw-rw-   0        0        0     1544 2023-06-09 06:20:55.000000 zhousf-lib-0.6.8/zhousflib/locust/locust_demo.py
+drwxrwxrwx   0        0        0        0 2023-06-12 03:16:25.342841 zhousf-lib-0.6.8/zhousflib/pandas/
+-rw-rw-rw-   0        0        0       60 2023-06-07 01:49:13.000000 zhousf-lib-0.6.8/zhousflib/pandas/__init__.py
+-rw-rw-rw-   0        0        0     3143 2023-06-12 02:53:40.000000 zhousf-lib-0.6.8/zhousflib/pandas/openpyxl_util.py
+-rw-rw-rw-   0        0        0     5598 2023-06-12 02:57:59.000000 zhousf-lib-0.6.8/zhousflib/pandas/pandas_util.py
+drwxrwxrwx   0        0        0        0 2023-06-12 03:16:25.344841 zhousf-lib-0.6.8/zhousflib/pdf/
+-rw-rw-rw-   0        0        0       60 2023-06-07 01:49:12.000000 zhousf-lib-0.6.8/zhousflib/pdf/__init__.py
+-rw-rw-rw-   0        0        0     1845 2023-06-07 01:49:12.000000 zhousf-lib-0.6.8/zhousflib/pdf/export_image.py
+-rw-rw-rw-   0        0        0     1467 2023-06-08 02:34:30.000000 zhousf-lib-0.6.8/zhousflib/pdf/pdfplumber_util.py
+drwxrwxrwx   0        0        0        0 2023-06-12 03:16:25.359842 zhousf-lib-0.6.8/zhousflib/util/
+-rw-rw-rw-   0        0        0       60 2023-06-07 01:49:12.000000 zhousf-lib-0.6.8/zhousflib/util/__init__.py
+-rw-rw-rw-   0        0        0     2770 2023-06-07 01:49:13.000000 zhousf-lib-0.6.8/zhousflib/util/calculater_util.py
+-rw-rw-rw-   0        0        0      635 2023-06-07 01:49:12.000000 zhousf-lib-0.6.8/zhousflib/util/cv_util.py
+-rw-rw-rw-   0        0        0     2193 2023-06-07 01:49:13.000000 zhousf-lib-0.6.8/zhousflib/util/encrypt_util.py
+-rw-rw-rw-   0        0        0     1336 2023-06-07 01:49:12.000000 zhousf-lib-0.6.8/zhousflib/util/img_util.py
+-rw-rw-rw-   0        0        0    12930 2023-06-07 01:49:12.000000 zhousf-lib-0.6.8/zhousflib/util/iou_util.py
+-rw-rw-rw-   0        0        0     3373 2023-06-07 01:49:12.000000 zhousf-lib-0.6.8/zhousflib/util/json_util.py
+-rw-rw-rw-   0        0        0      472 2023-06-07 01:49:13.000000 zhousf-lib-0.6.8/zhousflib/util/list_util.py
+-rw-rw-rw-   0        0        0     1358 2023-06-07 01:49:12.000000 zhousf-lib-0.6.8/zhousflib/util/permission_util.py
+-rw-rw-rw-   0        0        0     3524 2023-06-07 01:49:11.000000 zhousf-lib-0.6.8/zhousflib/util/poly_util.py
+-rw-rw-rw-   0        0        0      633 2023-06-07 01:49:12.000000 zhousf-lib-0.6.8/zhousflib/util/re_util.py
+-rw-rw-rw-   0        0        0      520 2023-06-07 01:49:12.000000 zhousf-lib-0.6.8/zhousflib/util/singleton.py
+-rw-rw-rw-   0        0        0     4246 2023-06-09 06:46:55.000000 zhousf-lib-0.6.8/zhousflib/util/string_util.py
+-rw-rw-rw-   0        0        0     4663 2023-06-07 01:49:11.000000 zhousf-lib-0.6.8/zhousflib/util/time_util.py
+drwxrwxrwx   0        0        0        0 2023-06-12 03:16:25.365841 zhousf-lib-0.6.8/zhousflib/web/
+-rw-rw-rw-   0        0        0       60 2023-06-07 01:49:12.000000 zhousf-lib-0.6.8/zhousflib/web/__init__.py
+-rw-rw-rw-   0        0        0     4355 2023-06-07 01:49:13.000000 zhousf-lib-0.6.8/zhousflib/web/config.py
+-rw-rw-rw-   0        0        0     3105 2023-06-07 01:49:12.000000 zhousf-lib-0.6.8/zhousflib/web/log_util.py
+-rw-rw-rw-   0        0        0     2860 2023-06-07 01:49:13.000000 zhousf-lib-0.6.8/zhousflib/web/logger.py
+-rw-rw-rw-   0        0        0     1340 2023-06-07 01:49:13.000000 zhousf-lib-0.6.8/zhousflib/web/response.py
```

### Comparing `zhousf-lib-0.6.7/LICENSE` & `zhousf-lib-0.6.8/LICENSE`

 * *Files identical despite different names*

### Comparing `zhousf-lib-0.6.7/PKG-INFO` & `zhousf-lib-0.6.8/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: zhousf-lib
-Version: 0.6.7
+Version: 0.6.8
 Summary: a python library of zhousf
 Home-page: https://github.com/MrZhousf/ZhousfLib
 Author: zhousf
 Author-email: 442553199@qq.com
 License: MIT
 Classifier: Intended Audience :: Developers
 Classifier: Topic :: Software Development :: Build Tools
```

### Comparing `zhousf-lib-0.6.7/README.md` & `zhousf-lib-0.6.8/README.md`

 * *Files identical despite different names*

### Comparing `zhousf-lib-0.6.7/setup.py` & `zhousf-lib-0.6.8/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -16,15 +16,15 @@
 # 打包：python setup.py upload
 NAME = 'zhousf-lib'
 DESCRIPTION = 'a python library of zhousf'
 URL = 'https://github.com/MrZhousf/ZhousfLib'
 EMAIL = '442553199@qq.com'
 AUTHOR = 'zhousf'
 REQUIRES_PYTHON = '>=3.6.13'
-VERSION = '0.6.7'
+VERSION = '0.6.8'
 PACKAGE_DATA = {'': ['*.yaml', '*.ttf', '*.txt', '*.md']}
 
 
 with open('README.md', 'r', encoding='utf-8') as fh:
     long_description = fh.read()
 
 # What packages are required for this module to be executed?
```

### Comparing `zhousf-lib-0.6.7/zhousf_lib.egg-info/PKG-INFO` & `zhousf-lib-0.6.8/zhousf_lib.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: zhousf-lib
-Version: 0.6.7
+Version: 0.6.8
 Summary: a python library of zhousf
 Home-page: https://github.com/MrZhousf/ZhousfLib
 Author: zhousf
 Author-email: 442553199@qq.com
 License: MIT
 Classifier: Intended Audience :: Developers
 Classifier: Topic :: Software Development :: Build Tools
```

### Comparing `zhousf-lib-0.6.7/zhousf_lib.egg-info/SOURCES.txt` & `zhousf-lib-0.6.8/zhousf_lib.egg-info/SOURCES.txt`

 * *Files 2% similar despite different names*

```diff
@@ -1,14 +1,13 @@
 LICENSE
 README.md
 setup.py
 zhousf_lib.egg-info/PKG-INFO
 zhousf_lib.egg-info/SOURCES.txt
 zhousf_lib.egg-info/dependency_links.txt
-zhousf_lib.egg-info/requires.txt
 zhousf_lib.egg-info/top_level.txt
 zhousflib/__init__.py
 zhousflib/datasets/__init__.py
 zhousflib/datasets/classification/__init__.py
 zhousflib/datasets/classification/classification_dataset_split.py
 zhousflib/datasets/coco/__init__.py
 zhousflib/datasets/coco/coco_bbox_extract.py
```

### Comparing `zhousf-lib-0.6.7/zhousflib/datasets/classification/classification_dataset_split.py` & `zhousf-lib-0.6.8/zhousflib/datasets/classification/classification_dataset_split.py`

 * *Files identical despite different names*

### Comparing `zhousf-lib-0.6.7/zhousflib/datasets/coco/coco_bbox_extract.py` & `zhousf-lib-0.6.8/zhousflib/datasets/coco/coco_bbox_extract.py`

 * *Files identical despite different names*

### Comparing `zhousf-lib-0.6.7/zhousflib/datasets/coco/coco_bbox_update.py` & `zhousf-lib-0.6.8/zhousflib/datasets/coco/coco_bbox_update.py`

 * *Files identical despite different names*

### Comparing `zhousf-lib-0.6.7/zhousflib/datasets/coco/coco_bbox_vis.py` & `zhousf-lib-0.6.8/zhousflib/datasets/coco/coco_bbox_vis.py`

 * *Files identical despite different names*

### Comparing `zhousf-lib-0.6.7/zhousflib/datasets/coco/coco_dataset_merge.py` & `zhousf-lib-0.6.8/zhousflib/datasets/coco/coco_dataset_merge.py`

 * *Files identical despite different names*

### Comparing `zhousf-lib-0.6.7/zhousflib/datasets/coco/coco_dataset_split.py` & `zhousf-lib-0.6.8/zhousflib/datasets/coco/coco_dataset_split.py`

 * *Files identical despite different names*

### Comparing `zhousf-lib-0.6.7/zhousflib/datasets/labelme/labelme_clip.py` & `zhousf-lib-0.6.8/zhousflib/datasets/labelme/labelme_clip.py`

 * *Files identical despite different names*

### Comparing `zhousf-lib-0.6.7/zhousflib/datasets/labelme/labelme_convert_coco.py` & `zhousf-lib-0.6.8/zhousflib/datasets/labelme/labelme_convert_coco.py`

 * *Files identical despite different names*

### Comparing `zhousf-lib-0.6.7/zhousflib/datasets/labelme/labelme_convert_seg.py` & `zhousf-lib-0.6.8/zhousflib/datasets/labelme/labelme_convert_seg.py`

 * *Files identical despite different names*

### Comparing `zhousf-lib-0.6.7/zhousflib/datasets/labelme/labelme_dataset_clip.py` & `zhousf-lib-0.6.8/zhousflib/datasets/labelme/labelme_dataset_clip.py`

 * *Files identical despite different names*

### Comparing `zhousf-lib-0.6.7/zhousflib/datasets/segmentation/seg_dataset_split.py` & `zhousf-lib-0.6.8/zhousflib/datasets/segmentation/seg_dataset_split.py`

 * *Files identical despite different names*

### Comparing `zhousf-lib-0.6.7/zhousflib/db/lmdb_master.py` & `zhousf-lib-0.6.8/zhousflib/db/lmdb_master.py`

 * *Files identical despite different names*

### Comparing `zhousf-lib-0.6.7/zhousflib/decorator/interceptor_util.py` & `zhousf-lib-0.6.8/zhousflib/decorator/interceptor_util.py`

 * *Files identical despite different names*

### Comparing `zhousf-lib-0.6.7/zhousflib/font/SimSun.ttf` & `zhousf-lib-0.6.8/zhousflib/font/SimSun.ttf`

 * *Files identical despite different names*

### Comparing `zhousf-lib-0.6.7/zhousflib/font/Symbola.ttf` & `zhousf-lib-0.6.8/zhousflib/font/Symbola.ttf`

 * *Files identical despite different names*

### Comparing `zhousf-lib-0.6.7/zhousflib/font/__init__.py` & `zhousf-lib-0.6.8/zhousflib/font/__init__.py`

 * *Files identical despite different names*

### Comparing `zhousf-lib-0.6.7/zhousflib/locust/locust_demo.py` & `zhousf-lib-0.6.8/zhousflib/locust/locust_demo.py`

 * *Files identical despite different names*

### Comparing `zhousf-lib-0.6.7/zhousflib/pandas/openpyxl_util.py` & `zhousf-lib-0.6.8/zhousflib/pandas/openpyxl_util.py`

 * *Files identical despite different names*

### Comparing `zhousf-lib-0.6.7/zhousflib/pandas/pandas_util.py` & `zhousf-lib-0.6.8/zhousflib/pandas/pandas_util.py`

 * *Files identical despite different names*

### Comparing `zhousf-lib-0.6.7/zhousflib/pdf/export_image.py` & `zhousf-lib-0.6.8/zhousflib/pdf/export_image.py`

 * *Files identical despite different names*

### Comparing `zhousf-lib-0.6.7/zhousflib/pdf/pdfplumber_util.py` & `zhousf-lib-0.6.8/zhousflib/pdf/pdfplumber_util.py`

 * *Files identical despite different names*

### Comparing `zhousf-lib-0.6.7/zhousflib/util/calculater_util.py` & `zhousf-lib-0.6.8/zhousflib/util/calculater_util.py`

 * *Files identical despite different names*

### Comparing `zhousf-lib-0.6.7/zhousflib/util/cv_util.py` & `zhousf-lib-0.6.8/zhousflib/util/cv_util.py`

 * *Files identical despite different names*

### Comparing `zhousf-lib-0.6.7/zhousflib/util/encrypt_util.py` & `zhousf-lib-0.6.8/zhousflib/util/encrypt_util.py`

 * *Files identical despite different names*

### Comparing `zhousf-lib-0.6.7/zhousflib/util/img_util.py` & `zhousf-lib-0.6.8/zhousflib/util/img_util.py`

 * *Files identical despite different names*

### Comparing `zhousf-lib-0.6.7/zhousflib/util/iou_util.py` & `zhousf-lib-0.6.8/zhousflib/util/iou_util.py`

 * *Files identical despite different names*

### Comparing `zhousf-lib-0.6.7/zhousflib/util/json_util.py` & `zhousf-lib-0.6.8/zhousflib/util/json_util.py`

 * *Files identical despite different names*

### Comparing `zhousf-lib-0.6.7/zhousflib/util/permission_util.py` & `zhousf-lib-0.6.8/zhousflib/util/permission_util.py`

 * *Files identical despite different names*

### Comparing `zhousf-lib-0.6.7/zhousflib/util/poly_util.py` & `zhousf-lib-0.6.8/zhousflib/util/poly_util.py`

 * *Files identical despite different names*

### Comparing `zhousf-lib-0.6.7/zhousflib/util/re_util.py` & `zhousf-lib-0.6.8/zhousflib/util/re_util.py`

 * *Files identical despite different names*

### Comparing `zhousf-lib-0.6.7/zhousflib/util/singleton.py` & `zhousf-lib-0.6.8/zhousflib/util/singleton.py`

 * *Files identical despite different names*

### Comparing `zhousf-lib-0.6.7/zhousflib/util/string_util.py` & `zhousf-lib-0.6.8/zhousflib/util/string_util.py`

 * *Files identical despite different names*

### Comparing `zhousf-lib-0.6.7/zhousflib/util/time_util.py` & `zhousf-lib-0.6.8/zhousflib/util/time_util.py`

 * *Files identical despite different names*

### Comparing `zhousf-lib-0.6.7/zhousflib/web/config.py` & `zhousf-lib-0.6.8/zhousflib/web/config.py`

 * *Files identical despite different names*

### Comparing `zhousf-lib-0.6.7/zhousflib/web/log_util.py` & `zhousf-lib-0.6.8/zhousflib/web/log_util.py`

 * *Files identical despite different names*

### Comparing `zhousf-lib-0.6.7/zhousflib/web/logger.py` & `zhousf-lib-0.6.8/zhousflib/web/logger.py`

 * *Files identical despite different names*

### Comparing `zhousf-lib-0.6.7/zhousflib/web/response.py` & `zhousf-lib-0.6.8/zhousflib/web/response.py`

 * *Files identical despite different names*

