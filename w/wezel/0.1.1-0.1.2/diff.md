# Comparing `tmp/wezel-0.1.1.tar.gz` & `tmp/wezel-0.1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "C:\Users\steve\Dropbox\Software\QIB-Sheffield\wezel\dist\.tmp-9gbqtj64\wezel-0.1.1.tar", last modified: Tue Jan 10 00:32:23 2023, max compression
+gzip compressed data, was "wezel-0.1.2.tar", last modified: Mon Jun 12 14:32:24 2023, max compression
```

## Comparing `wezel-0.1.1.tar` & `wezel-0.1.2.tar`

### file list

```diff
@@ -1,130 +1,153 @@
-drwxrwxrwx   0        0        0        0 2023-01-10 00:32:23.000000 wezel-0.1.1/
--rw-rw-rw-   0        0        0    11525 2022-09-23 18:20:24.000000 wezel-0.1.1/LICENSE
--rw-rw-rw-   0        0        0      159 2022-11-14 23:16:05.000000 wezel-0.1.1/MANIFEST.in
--rw-rw-rw-   0        0        0    14205 2023-01-10 00:32:23.000000 wezel-0.1.1/PKG-INFO
--rw-rw-rw-   0        0        0      110 2022-11-14 22:06:20.000000 wezel-0.1.1/README.md
--rw-rw-rw-   0        0        0     2230 2023-01-10 00:08:32.000000 wezel-0.1.1/pyproject.toml
--rw-rw-rw-   0        0        0       42 2023-01-10 00:32:23.000000 wezel-0.1.1/setup.cfg
--rw-rw-rw-   0        0        0      215 2022-09-23 18:20:24.000000 wezel-0.1.1/setup.py
-drwxrwxrwx   0        0        0        0 2023-01-10 00:32:22.000000 wezel-0.1.1/src/
-drwxrwxrwx   0        0        0        0 2023-01-10 00:32:22.000000 wezel-0.1.1/src/wezel/
--rw-rw-rw-   0        0        0      157 2023-01-03 22:08:36.000000 wezel-0.1.1/src/wezel/__init__.py
-drwxrwxrwx   0        0        0        0 2023-01-10 00:32:23.000000 wezel-0.1.1/src/wezel/actions/
--rw-rw-rw-   0        0        0      136 2023-01-03 22:31:56.000000 wezel-0.1.1/src/wezel/actions/__init__.py
--rw-rw-rw-   0        0        0      228 2022-10-22 16:04:00.000000 wezel-0.1.1/src/wezel/actions/about.py
--rw-rw-rw-   0        0        0      236 2022-11-29 17:02:50.000000 wezel-0.1.1/src/wezel/actions/demo.py
--rw-rw-rw-   0        0        0    14317 2023-01-04 00:20:23.000000 wezel-0.1.1/src/wezel/actions/edit.py
--rw-rw-rw-   0        0        0    23178 2023-01-09 22:41:13.000000 wezel-0.1.1/src/wezel/actions/filter.py
--rw-rw-rw-   0        0        0     5699 2022-12-11 17:28:27.000000 wezel-0.1.1/src/wezel/actions/folder.py
--rw-rw-rw-   0        0        0    12352 2023-01-09 22:17:32.000000 wezel-0.1.1/src/wezel/actions/segment.py
--rw-rw-rw-   0        0        0     5199 2022-11-30 09:34:50.000000 wezel-0.1.1/src/wezel/actions/test.py
--rw-rw-rw-   0        0        0     9277 2023-01-09 22:49:49.000000 wezel-0.1.1/src/wezel/actions/transform.py
--rw-rw-rw-   0        0        0     2208 2022-12-30 13:44:55.000000 wezel-0.1.1/src/wezel/actions/view.py
-drwxrwxrwx   0        0        0        0 2023-01-10 00:32:23.000000 wezel-0.1.1/src/wezel/canvas/
--rw-rw-rw-   0        0        0      884 2022-12-22 09:22:41.000000 wezel-0.1.1/src/wezel/canvas/__init__.py
--rw-rw-rw-   0        0        0    16824 2023-01-02 23:37:11.000000 wezel-0.1.1/src/wezel/canvas/canvas.py
--rw-rw-rw-   0        0        0     3825 2022-12-29 11:15:46.000000 wezel-0.1.1/src/wezel/canvas/image_filter.py
--rw-rw-rw-   0        0        0    37208 2023-01-03 02:51:46.000000 wezel-0.1.1/src/wezel/canvas/mask_filter.py
--rw-rw-rw-   0        0        0     2796 2022-12-27 21:21:40.000000 wezel-0.1.1/src/wezel/canvas/scene_filter.py
--rw-rw-rw-   0        0        0    10275 2023-01-05 22:35:46.000000 wezel-0.1.1/src/wezel/canvas/series_canvas.py
--rw-rw-rw-   0        0        0    15301 2022-12-30 16:16:27.000000 wezel-0.1.1/src/wezel/canvas/toolbar.py
--rw-rw-rw-   0        0        0     8602 2023-01-03 00:20:57.000000 wezel-0.1.1/src/wezel/canvas/utils.py
--rw-rw-rw-   0        0        0    11504 2023-01-05 18:17:19.000000 wezel-0.1.1/src/wezel/core.py
-drwxrwxrwx   0        0        0        0 2023-01-10 00:32:23.000000 wezel-0.1.1/src/wezel/icons/
--rw-rw-rw-   0        0        0      112 2022-10-05 13:08:53.000000 wezel-0.1.1/src/wezel/icons/__init__.py
-drwxrwxrwx   0        0        0        0 2023-01-10 00:32:23.000000 wezel-0.1.1/src/wezel/icons/fugue_icons/
--rw-rw-rw-   0        0        0        0 2022-09-23 18:20:24.000000 wezel-0.1.1/src/wezel/icons/fugue_icons/__init__.py
--rw-rw-rw-   0        0        0      524 2022-09-23 18:20:24.000000 wezel-0.1.1/src/wezel/icons/fugue_icons/application-import.png
--rw-rw-rw-   0        0        0      631 2022-09-23 18:20:24.000000 wezel-0.1.1/src/wezel/icons/fugue_icons/arrow-curve-180-left.png
--rw-rw-rw-   0        0        0      613 2021-11-07 15:47:08.000000 wezel-0.1.1/src/wezel/icons/fugue_icons/arrow-curve.png
--rw-rw-rw-   0        0        0      771 2022-09-23 18:20:24.000000 wezel-0.1.1/src/wezel/icons/fugue_icons/arrow-in.png
--rw-rw-rw-   0        0        0      740 2022-09-23 18:20:24.000000 wezel-0.1.1/src/wezel/icons/fugue_icons/arrow-move.png
--rw-rw-rw-   0        0        0      813 2022-09-23 18:20:24.000000 wezel-0.1.1/src/wezel/icons/fugue_icons/arrow-out.png
--rw-rw-rw-   0        0        0      455 2021-11-07 15:47:09.000000 wezel-0.1.1/src/wezel/icons/fugue_icons/arrow-resize-090.png
--rw-rw-rw-   0        0        0      595 2022-09-23 18:20:24.000000 wezel-0.1.1/src/wezel/icons/fugue_icons/bin-metal.png
--rw-rw-rw-   0        0        0      697 2022-09-23 18:20:24.000000 wezel-0.1.1/src/wezel/icons/fugue_icons/blue-document-export.png
--rw-rw-rw-   0        0        0      743 2022-09-23 18:20:24.000000 wezel-0.1.1/src/wezel/icons/fugue_icons/brightness.png
--rw-rw-rw-   0        0        0      858 2021-11-07 15:47:31.000000 wezel-0.1.1/src/wezel/icons/fugue_icons/color--arrow.png
--rw-rw-rw-   0        0        0      811 2021-11-07 15:47:32.000000 wezel-0.1.1/src/wezel/icons/fugue_icons/color.png
--rw-rw-rw-   0        0        0      676 2021-11-07 15:47:32.000000 wezel-0.1.1/src/wezel/icons/fugue_icons/contrast-low.png
--rw-rw-rw-   0        0        0      678 2022-09-23 18:20:24.000000 wezel-0.1.1/src/wezel/icons/fugue_icons/contrast.png
--rw-rw-rw-   0        0        0      529 2021-11-07 15:47:34.000000 wezel-0.1.1/src/wezel/icons/fugue_icons/controller-d-pad.png
--rw-rw-rw-   0        0        0      663 2021-11-07 15:47:35.000000 wezel-0.1.1/src/wezel/icons/fugue_icons/cross-script.png
--rw-rw-rw-   0        0        0      544 2022-09-23 18:20:24.000000 wezel-0.1.1/src/wezel/icons/fugue_icons/cursor.png
--rw-rw-rw-   0        0        0      548 2022-09-23 18:20:24.000000 wezel-0.1.1/src/wezel/icons/fugue_icons/cutter.png
--rw-rw-rw-   0        0        0      507 2022-09-23 18:20:24.000000 wezel-0.1.1/src/wezel/icons/fugue_icons/disk.png
--rw-rw-rw-   0        0        0      762 2021-11-07 15:47:47.000000 wezel-0.1.1/src/wezel/icons/fugue_icons/eraser--arrow.png
--rw-rw-rw-   0        0        0      754 2021-11-07 15:47:47.000000 wezel-0.1.1/src/wezel/icons/fugue_icons/eraser--plus.png
--rw-rw-rw-   0        0        0      656 2022-09-23 18:20:24.000000 wezel-0.1.1/src/wezel/icons/fugue_icons/eraser.png
--rw-rw-rw-   0        0        0     1558 2022-09-23 18:20:24.000000 wezel-0.1.1/src/wezel/icons/fugue_icons/hand-finger.png
--rw-rw-rw-   0        0        0      687 2022-09-23 18:20:24.000000 wezel-0.1.1/src/wezel/icons/fugue_icons/hand-point-090.png
--rw-rw-rw-   0        0        0      672 2022-09-23 18:20:24.000000 wezel-0.1.1/src/wezel/icons/fugue_icons/hand.png
--rw-rw-rw-   0        0        0      536 2021-11-07 15:47:59.000000 wezel-0.1.1/src/wezel/icons/fugue_icons/layer-select.png
--rw-rw-rw-   0        0        0      536 2022-09-23 18:20:24.000000 wezel-0.1.1/src/wezel/icons/fugue_icons/layer-shape-curve.png
--rw-rw-rw-   0        0        0      761 2022-09-23 18:20:24.000000 wezel-0.1.1/src/wezel/icons/fugue_icons/layer-shape-ellipse.png
--rw-rw-rw-   0        0        0      643 2022-09-23 18:20:24.000000 wezel-0.1.1/src/wezel/icons/fugue_icons/layer-shape-polygon.png
--rw-rw-rw-   0        0        0      646 2021-11-07 15:47:59.000000 wezel-0.1.1/src/wezel/icons/fugue_icons/layer-shape-round.png
--rw-rw-rw-   0        0        0      498 2022-09-23 18:20:24.000000 wezel-0.1.1/src/wezel/icons/fugue_icons/layer-shape.png
--rw-rw-rw-   0        0        0      599 2021-11-07 15:47:59.000000 wezel-0.1.1/src/wezel/icons/fugue_icons/layer-transparent.png
--rw-rw-rw-   0        0        0      498 2022-09-23 18:20:24.000000 wezel-0.1.1/src/wezel/icons/fugue_icons/layer.png
--rw-rw-rw-   0        0        0      902 2021-11-07 15:48:00.000000 wezel-0.1.1/src/wezel/icons/fugue_icons/lifebuoy.png
--rw-rw-rw-   0        0        0      640 2022-09-23 18:20:24.000000 wezel-0.1.1/src/wezel/icons/fugue_icons/lock-unlock.png
--rw-rw-rw-   0        0        0     1535 2022-09-23 18:20:24.000000 wezel-0.1.1/src/wezel/icons/fugue_icons/lock.png
--rw-rw-rw-   0        0        0      775 2021-11-07 15:48:02.000000 wezel-0.1.1/src/wezel/icons/fugue_icons/magnifier-zoom-actual.png
--rw-rw-rw-   0        0        0      756 2021-11-07 15:48:02.000000 wezel-0.1.1/src/wezel/icons/fugue_icons/magnifier-zoom-fit.png
--rw-rw-rw-   0        0        0      758 2021-11-07 15:48:02.000000 wezel-0.1.1/src/wezel/icons/fugue_icons/magnifier-zoom-in.png
--rw-rw-rw-   0        0        0      736 2021-11-07 15:48:02.000000 wezel-0.1.1/src/wezel/icons/fugue_icons/magnifier-zoom-out.png
--rw-rw-rw-   0        0        0      700 2022-09-23 18:20:24.000000 wezel-0.1.1/src/wezel/icons/fugue_icons/magnifier.png
--rw-rw-rw-   0        0        0      259 2022-09-23 18:20:24.000000 wezel-0.1.1/src/wezel/icons/fugue_icons/minus.png
--rw-rw-rw-   0        0        0      721 2021-11-07 15:48:10.000000 wezel-0.1.1/src/wezel/icons/fugue_icons/paint-brush--arrow.png
--rw-rw-rw-   0        0        0      655 2022-09-23 18:20:24.000000 wezel-0.1.1/src/wezel/icons/fugue_icons/paint-brush--minus.png
--rw-rw-rw-   0        0        0      723 2021-11-07 15:48:11.000000 wezel-0.1.1/src/wezel/icons/fugue_icons/paint-brush--plus.png
--rw-rw-rw-   0        0        0      589 2022-09-23 18:20:24.000000 wezel-0.1.1/src/wezel/icons/fugue_icons/paint-brush.png
--rw-rw-rw-   0        0        0      776 2022-09-23 18:20:24.000000 wezel-0.1.1/src/wezel/icons/fugue_icons/paint-can--minus.png
--rw-rw-rw-   0        0        0      811 2021-11-07 15:48:11.000000 wezel-0.1.1/src/wezel/icons/fugue_icons/paint-can--plus.png
--rw-rw-rw-   0        0        0      721 2022-09-23 18:20:24.000000 wezel-0.1.1/src/wezel/icons/fugue_icons/paint.png
--rw-rw-rw-   0        0        0     1548 2022-09-23 18:20:24.000000 wezel-0.1.1/src/wezel/icons/fugue_icons/pencil.png
--rw-rw-rw-   0        0        0      521 2022-09-23 18:20:24.000000 wezel-0.1.1/src/wezel/icons/fugue_icons/plus.png
--rw-rw-rw-   0        0        0     1568 2022-09-23 18:20:24.000000 wezel-0.1.1/src/wezel/icons/fugue_icons/spectrum.png
--rw-rw-rw-   0        0        0      605 2021-11-07 15:48:34.000000 wezel-0.1.1/src/wezel/icons/fugue_icons/tick-button.png
--rw-rw-rw-   0        0        0      355 2021-11-07 15:48:37.000000 wezel-0.1.1/src/wezel/icons/fugue_icons/ui-check-box-uncheck.png
--rw-rw-rw-   0        0        0      435 2021-11-07 15:48:37.000000 wezel-0.1.1/src/wezel/icons/fugue_icons/ui-check-box.png
--rw-rw-rw-   0        0        0      725 2022-09-23 18:20:24.000000 wezel-0.1.1/src/wezel/icons/fugue_icons/wand-hat.png
--rw-rw-rw-   0        0        0      610 2022-09-23 18:20:24.000000 wezel-0.1.1/src/wezel/icons/fugue_icons/wand.png
-drwxrwxrwx   0        0        0        0 2023-01-10 00:32:23.000000 wezel-0.1.1/src/wezel/icons/images/
--rw-rw-rw-   0        0        0        0 2022-09-23 18:20:24.000000 wezel-0.1.1/src/wezel/icons/images/__init__.py
--rw-rw-rw-   0        0        0   407459 2022-09-23 18:20:24.000000 wezel-0.1.1/src/wezel/icons/images/wezel.jpg
--rw-rw-rw-   0        0        0     4773 2023-01-03 00:52:03.000000 wezel-0.1.1/src/wezel/icons/inventory.py
-drwxrwxrwx   0        0        0        0 2023-01-10 00:32:23.000000 wezel-0.1.1/src/wezel/icons/my_icons/
--rw-rw-rw-   0        0        0        0 2022-09-23 18:20:24.000000 wezel-0.1.1/src/wezel/icons/my_icons/__init__.py
--rw-rw-rw-   0        0        0     1406 2022-09-23 18:20:24.000000 wezel-0.1.1/src/wezel/icons/my_icons/favicon.ico
--rw-rw-rw-   0        0        0    76029 2022-09-23 18:20:24.000000 wezel-0.1.1/src/wezel/icons/my_icons/question-mark.png
--rw-rw-rw-   0        0        0      701 2022-09-23 18:20:24.000000 wezel-0.1.1/src/wezel/icons/my_icons/slider_icon.png
--rw-rw-rw-   0        0        0     5904 2022-11-30 09:47:57.000000 wezel-0.1.1/src/wezel/main.py
--rw-rw-rw-   0        0        0     2444 2023-01-03 22:28:19.000000 wezel-0.1.1/src/wezel/menus.py
-drwxrwxrwx   0        0        0        0 2023-01-10 00:32:23.000000 wezel-0.1.1/src/wezel/utils/
--rw-rw-rw-   0        0        0        0 2023-01-03 22:11:49.000000 wezel-0.1.1/src/wezel/utils/__init__.py
--rw-rw-rw-   0        0        0     1533 2023-01-09 22:50:10.000000 wezel-0.1.1/src/wezel/utils/dbimage.py
--rw-rw-rw-   0        0        0    26926 2023-01-09 22:48:24.000000 wezel-0.1.1/src/wezel/utils/scipy.py
--rw-rw-rw-   0        0        0    12305 2023-01-09 22:11:19.000000 wezel-0.1.1/src/wezel/utils/skimage.py
-drwxrwxrwx   0        0        0        0 2023-01-10 00:32:23.000000 wezel-0.1.1/src/wezel/widgets/
--rw-rw-rw-   0        0        0      890 2022-12-28 11:52:51.000000 wezel-0.1.1/src/wezel/widgets/__init__.py
--rw-rw-rw-   0        0        0     6495 2022-11-30 09:44:50.000000 wezel-0.1.1/src/wezel/widgets/dbdatabase.py
--rw-rw-rw-   0        0        0    10164 2022-12-15 22:41:33.000000 wezel-0.1.1/src/wezel/widgets/dbimage.py
--rw-rw-rw-   0        0        0    13162 2023-01-05 18:17:44.000000 wezel-0.1.1/src/wezel/widgets/dicom_header.py
--rw-rw-rw-   0        0        0      395 2022-11-25 11:51:45.000000 wezel-0.1.1/src/wezel/widgets/file_display.py
--rw-rw-rw-   0        0        0     5388 2022-09-23 18:20:24.000000 wezel-0.1.1/src/wezel/widgets/log_to_GUI.py
--rw-rw-rw-   0        0        0     2553 2022-12-22 00:00:29.000000 wezel-0.1.1/src/wezel/widgets/main_mdi.py
--rw-rw-rw-   0        0        0    19608 2023-01-09 11:37:22.000000 wezel-0.1.1/src/wezel/widgets/message.py
--rw-rw-rw-   0        0        0     1800 2022-12-27 21:03:59.000000 wezel-0.1.1/src/wezel/widgets/plot_curve.py
--rw-rw-rw-   0        0        0    10255 2022-12-28 11:52:10.000000 wezel-0.1.1/src/wezel/widgets/qrangeslider.py
--rw-rw-rw-   0        0        0     4053 2022-12-21 13:35:20.000000 wezel-0.1.1/src/wezel/widgets/region_list.py
--rw-rw-rw-   0        0        0    10606 2023-01-05 18:24:33.000000 wezel-0.1.1/src/wezel/widgets/series_display.py
--rw-rw-rw-   0        0        0    10919 2022-12-18 22:11:04.000000 wezel-0.1.1/src/wezel/widgets/series_sliders.py
--rw-rw-rw-   0        0        0     6948 2022-12-27 16:39:36.000000 wezel-0.1.1/src/wezel/widgets/sliders.py
-drwxrwxrwx   0        0        0        0 2023-01-10 00:32:23.000000 wezel-0.1.1/src/wezel.egg-info/
--rw-rw-rw-   0        0        0    14205 2023-01-10 00:32:22.000000 wezel-0.1.1/src/wezel.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0     4247 2023-01-10 00:32:22.000000 wezel-0.1.1/src/wezel.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-01-10 00:32:22.000000 wezel-0.1.1/src/wezel.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0      227 2023-01-10 00:32:22.000000 wezel-0.1.1/src/wezel.egg-info/requires.txt
--rw-rw-rw-   0        0        0        6 2023-01-10 00:32:22.000000 wezel-0.1.1/src/wezel.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-06-12 14:32:24.494999 wezel-0.1.2/
+-rw-rw-rw-   0        0        0    11525 2023-01-23 13:32:16.000000 wezel-0.1.2/LICENSE
+-rw-rw-rw-   0        0        0      159 2023-01-23 13:32:16.000000 wezel-0.1.2/MANIFEST.in
+-rw-rw-rw-   0        0        0    14208 2023-06-12 14:32:24.494999 wezel-0.1.2/PKG-INFO
+-rw-rw-rw-   0        0        0      110 2023-01-23 13:32:16.000000 wezel-0.1.2/README.md
+-rw-rw-rw-   0        0        0     3266 2023-06-12 14:11:59.000000 wezel-0.1.2/pyproject.toml
+-rw-rw-rw-   0        0        0       42 2023-06-12 14:32:24.494999 wezel-0.1.2/setup.cfg
+-rw-rw-rw-   0        0        0      215 2023-01-23 13:32:16.000000 wezel-0.1.2/setup.py
+drwxrwxrwx   0        0        0        0 2023-06-12 14:32:22.620568 wezel-0.1.2/src/
+drwxrwxrwx   0        0        0        0 2023-06-12 14:32:22.772629 wezel-0.1.2/src/wezel/
+-rw-rw-rw-   0        0        0      136 2023-03-17 15:55:48.000000 wezel-0.1.2/src/wezel/__init__.py
+-rw-rw-rw-   0        0        0     3795 2023-06-01 11:35:10.000000 wezel-0.1.2/src/wezel/api.py
+drwxrwxrwx   0        0        0        0 2023-06-12 14:32:22.977589 wezel-0.1.2/src/wezel/canvas/
+-rw-rw-rw-   0        0        0      945 2023-03-06 17:41:19.000000 wezel-0.1.2/src/wezel/canvas/__init__.py
+-rw-rw-rw-   0        0        0    17363 2023-03-13 11:30:34.000000 wezel-0.1.2/src/wezel/canvas/canvas.py
+-rw-rw-rw-   0        0        0     4084 2023-03-12 00:28:19.000000 wezel-0.1.2/src/wezel/canvas/image_filter.py
+-rw-rw-rw-   0        0        0    49633 2023-03-13 10:23:24.000000 wezel-0.1.2/src/wezel/canvas/mask_filter.py
+-rw-rw-rw-   0        0        0     2802 2023-03-12 00:27:43.000000 wezel-0.1.2/src/wezel/canvas/scene_filter.py
+-rw-rw-rw-   0        0        0    11020 2023-03-08 09:34:40.000000 wezel-0.1.2/src/wezel/canvas/series_canvas.py
+-rw-rw-rw-   0        0        0    16152 2023-03-12 00:27:43.000000 wezel-0.1.2/src/wezel/canvas/toolbar.py
+-rw-rw-rw-   0        0        0    13913 2023-02-17 21:33:54.000000 wezel-0.1.2/src/wezel/canvas/utils.py
+drwxrwxrwx   0        0        0        0 2023-06-12 14:32:23.078285 wezel-0.1.2/src/wezel/displays/
+-rw-rw-rw-   0        0        0      387 2023-03-17 15:55:48.000000 wezel-0.1.2/src/wezel/displays/__init__.py
+-rw-rw-rw-   0        0        0    13257 2023-03-13 10:26:35.000000 wezel-0.1.2/src/wezel/displays/dicom_header.py
+-rw-rw-rw-   0        0        0     1197 2023-03-12 00:27:43.000000 wezel-0.1.2/src/wezel/displays/plot_display.py
+-rw-rw-rw-   0        0        0     3445 2023-03-12 00:27:43.000000 wezel-0.1.2/src/wezel/displays/series_display.py
+-rw-rw-rw-   0        0        0     8271 2023-03-12 00:27:43.000000 wezel-0.1.2/src/wezel/displays/series_display_4d.py
+-rw-rw-rw-   0        0        0     5641 2023-03-12 00:27:43.000000 wezel-0.1.2/src/wezel/displays/table_display.py
+-rw-rw-rw-   0        0        0    19290 2023-05-25 22:21:13.000000 wezel-0.1.2/src/wezel/gui.py
+drwxrwxrwx   0        0        0        0 2023-06-12 14:32:23.084881 wezel-0.1.2/src/wezel/icons/
+-rw-rw-rw-   0        0        0      112 2023-01-23 13:32:16.000000 wezel-0.1.2/src/wezel/icons/__init__.py
+drwxrwxrwx   0        0        0        0 2023-06-12 14:32:24.052014 wezel-0.1.2/src/wezel/icons/fugue_icons/
+-rw-rw-rw-   0        0        0        0 2023-01-23 13:32:16.000000 wezel-0.1.2/src/wezel/icons/fugue_icons/__init__.py
+-rw-rw-rw-   0        0        0     1701 2021-11-07 15:47:02.000000 wezel-0.1.2/src/wezel/icons/fugue_icons/animal-dog.png
+-rw-rw-rw-   0        0        0      524 2023-01-23 13:32:16.000000 wezel-0.1.2/src/wezel/icons/fugue_icons/application-import.png
+-rw-rw-rw-   0        0        0      631 2023-01-23 13:32:16.000000 wezel-0.1.2/src/wezel/icons/fugue_icons/arrow-curve-180-left.png
+-rw-rw-rw-   0        0        0      613 2023-01-23 13:32:16.000000 wezel-0.1.2/src/wezel/icons/fugue_icons/arrow-curve.png
+-rw-rw-rw-   0        0        0      771 2023-01-23 13:32:16.000000 wezel-0.1.2/src/wezel/icons/fugue_icons/arrow-in.png
+-rw-rw-rw-   0        0        0      740 2023-01-23 13:32:16.000000 wezel-0.1.2/src/wezel/icons/fugue_icons/arrow-move.png
+-rw-rw-rw-   0        0        0      813 2023-01-23 13:32:16.000000 wezel-0.1.2/src/wezel/icons/fugue_icons/arrow-out.png
+-rw-rw-rw-   0        0        0      455 2023-01-23 13:32:16.000000 wezel-0.1.2/src/wezel/icons/fugue_icons/arrow-resize-090.png
+-rw-rw-rw-   0        0        0      628 2021-11-07 15:47:10.000000 wezel-0.1.2/src/wezel/icons/fugue_icons/arrow-stop-090.png
+-rw-rw-rw-   0        0        0      667 2021-11-07 15:47:10.000000 wezel-0.1.2/src/wezel/icons/fugue_icons/arrow-stop-270.png
+-rw-rw-rw-   0        0        0      595 2023-01-23 13:32:16.000000 wezel-0.1.2/src/wezel/icons/fugue_icons/bin-metal.png
+-rw-rw-rw-   0        0        0      697 2023-01-23 13:32:16.000000 wezel-0.1.2/src/wezel/icons/fugue_icons/blue-document-export.png
+-rw-rw-rw-   0        0        0      743 2023-01-23 13:32:16.000000 wezel-0.1.2/src/wezel/icons/fugue_icons/brightness.png
+-rw-rw-rw-   0        0        0      704 2021-11-07 15:47:24.000000 wezel-0.1.2/src/wezel/icons/fugue_icons/bug.png
+-rw-rw-rw-   0        0        0      622 2021-11-07 15:47:30.000000 wezel-0.1.2/src/wezel/icons/fugue_icons/clipboard--plus.png
+-rw-rw-rw-   0        0        0      858 2023-01-23 13:32:16.000000 wezel-0.1.2/src/wezel/icons/fugue_icons/color--arrow.png
+-rw-rw-rw-   0        0        0      811 2023-01-23 13:32:16.000000 wezel-0.1.2/src/wezel/icons/fugue_icons/color.png
+-rw-rw-rw-   0        0        0      676 2023-01-23 13:32:16.000000 wezel-0.1.2/src/wezel/icons/fugue_icons/contrast-low.png
+-rw-rw-rw-   0        0        0      678 2023-01-23 13:32:16.000000 wezel-0.1.2/src/wezel/icons/fugue_icons/contrast.png
+-rw-rw-rw-   0        0        0      529 2023-01-23 13:32:16.000000 wezel-0.1.2/src/wezel/icons/fugue_icons/controller-d-pad.png
+-rw-rw-rw-   0        0        0      663 2023-01-23 13:32:16.000000 wezel-0.1.2/src/wezel/icons/fugue_icons/cross-script.png
+-rw-rw-rw-   0        0        0      544 2023-01-23 13:32:16.000000 wezel-0.1.2/src/wezel/icons/fugue_icons/cursor.png
+-rw-rw-rw-   0        0        0      548 2023-01-23 13:32:16.000000 wezel-0.1.2/src/wezel/icons/fugue_icons/cutter.png
+-rw-rw-rw-   0        0        0      507 2023-01-23 13:32:16.000000 wezel-0.1.2/src/wezel/icons/fugue_icons/disk.png
+-rw-rw-rw-   0        0        0      702 2021-11-07 15:47:40.000000 wezel-0.1.2/src/wezel/icons/fugue_icons/document-excel-csv.png
+-rw-rw-rw-   0        0        0      672 2021-11-07 15:47:40.000000 wezel-0.1.2/src/wezel/icons/fugue_icons/document-excel.png
+-rw-rw-rw-   0        0        0      762 2023-01-23 13:32:16.000000 wezel-0.1.2/src/wezel/icons/fugue_icons/eraser--arrow.png
+-rw-rw-rw-   0        0        0      754 2023-01-23 13:32:16.000000 wezel-0.1.2/src/wezel/icons/fugue_icons/eraser--plus.png
+-rw-rw-rw-   0        0        0      656 2023-01-23 13:32:16.000000 wezel-0.1.2/src/wezel/icons/fugue_icons/eraser.png
+-rw-rw-rw-   0        0        0     1558 2023-01-23 13:32:16.000000 wezel-0.1.2/src/wezel/icons/fugue_icons/hand-finger.png
+-rw-rw-rw-   0        0        0      687 2023-01-23 13:32:16.000000 wezel-0.1.2/src/wezel/icons/fugue_icons/hand-point-090.png
+-rw-rw-rw-   0        0        0      672 2023-01-23 13:32:16.000000 wezel-0.1.2/src/wezel/icons/fugue_icons/hand.png
+-rw-rw-rw-   0        0        0      536 2023-01-23 13:32:16.000000 wezel-0.1.2/src/wezel/icons/fugue_icons/layer-select.png
+-rw-rw-rw-   0        0        0      536 2023-01-23 13:32:16.000000 wezel-0.1.2/src/wezel/icons/fugue_icons/layer-shape-curve.png
+-rw-rw-rw-   0        0        0      761 2023-01-23 13:32:16.000000 wezel-0.1.2/src/wezel/icons/fugue_icons/layer-shape-ellipse.png
+-rw-rw-rw-   0        0        0      643 2023-01-23 13:32:16.000000 wezel-0.1.2/src/wezel/icons/fugue_icons/layer-shape-polygon.png
+-rw-rw-rw-   0        0        0      646 2023-01-23 13:32:16.000000 wezel-0.1.2/src/wezel/icons/fugue_icons/layer-shape-round.png
+-rw-rw-rw-   0        0        0      498 2023-01-23 13:32:16.000000 wezel-0.1.2/src/wezel/icons/fugue_icons/layer-shape.png
+-rw-rw-rw-   0        0        0      599 2023-01-23 13:32:16.000000 wezel-0.1.2/src/wezel/icons/fugue_icons/layer-transparent.png
+-rw-rw-rw-   0        0        0      498 2023-01-23 13:32:16.000000 wezel-0.1.2/src/wezel/icons/fugue_icons/layer.png
+-rw-rw-rw-   0        0        0      902 2023-01-23 13:32:16.000000 wezel-0.1.2/src/wezel/icons/fugue_icons/lifebuoy.png
+-rw-rw-rw-   0        0        0      640 2023-01-23 13:32:16.000000 wezel-0.1.2/src/wezel/icons/fugue_icons/lock-unlock.png
+-rw-rw-rw-   0        0        0     1535 2023-01-23 13:32:16.000000 wezel-0.1.2/src/wezel/icons/fugue_icons/lock.png
+-rw-rw-rw-   0        0        0      775 2023-01-23 13:32:16.000000 wezel-0.1.2/src/wezel/icons/fugue_icons/magnifier-zoom-actual.png
+-rw-rw-rw-   0        0        0      756 2023-01-23 13:32:16.000000 wezel-0.1.2/src/wezel/icons/fugue_icons/magnifier-zoom-fit.png
+-rw-rw-rw-   0        0        0      758 2023-01-23 13:32:16.000000 wezel-0.1.2/src/wezel/icons/fugue_icons/magnifier-zoom-in.png
+-rw-rw-rw-   0        0        0      736 2023-01-23 13:32:16.000000 wezel-0.1.2/src/wezel/icons/fugue_icons/magnifier-zoom-out.png
+-rw-rw-rw-   0        0        0      700 2023-01-23 13:32:16.000000 wezel-0.1.2/src/wezel/icons/fugue_icons/magnifier.png
+-rw-rw-rw-   0        0        0      358 2021-11-07 15:48:06.000000 wezel-0.1.2/src/wezel/icons/fugue_icons/minus-small-circle.png
+-rw-rw-rw-   0        0        0      454 2021-11-07 15:48:06.000000 wezel-0.1.2/src/wezel/icons/fugue_icons/minus-small-white.png
+-rw-rw-rw-   0        0        0      259 2023-01-23 13:32:16.000000 wezel-0.1.2/src/wezel/icons/fugue_icons/minus.png
+-rw-rw-rw-   0        0        0      721 2023-01-23 13:32:16.000000 wezel-0.1.2/src/wezel/icons/fugue_icons/paint-brush--arrow.png
+-rw-rw-rw-   0        0        0      655 2023-01-23 13:32:16.000000 wezel-0.1.2/src/wezel/icons/fugue_icons/paint-brush--minus.png
+-rw-rw-rw-   0        0        0      723 2023-01-23 13:32:16.000000 wezel-0.1.2/src/wezel/icons/fugue_icons/paint-brush--plus.png
+-rw-rw-rw-   0        0        0      589 2023-01-23 13:32:16.000000 wezel-0.1.2/src/wezel/icons/fugue_icons/paint-brush.png
+-rw-rw-rw-   0        0        0      776 2023-01-23 13:32:16.000000 wezel-0.1.2/src/wezel/icons/fugue_icons/paint-can--minus.png
+-rw-rw-rw-   0        0        0      811 2023-01-23 13:32:16.000000 wezel-0.1.2/src/wezel/icons/fugue_icons/paint-can--plus.png
+-rw-rw-rw-   0        0        0      721 2023-01-23 13:32:16.000000 wezel-0.1.2/src/wezel/icons/fugue_icons/paint.png
+-rw-rw-rw-   0        0        0     1548 2023-01-23 13:32:16.000000 wezel-0.1.2/src/wezel/icons/fugue_icons/pencil.png
+-rw-rw-rw-   0        0        0      457 2021-11-07 15:48:15.000000 wezel-0.1.2/src/wezel/icons/fugue_icons/plus-small-white.png
+-rw-rw-rw-   0        0        0      521 2023-01-23 13:32:16.000000 wezel-0.1.2/src/wezel/icons/fugue_icons/plus.png
+-rw-rw-rw-   0        0        0     1568 2023-01-23 13:32:16.000000 wezel-0.1.2/src/wezel/icons/fugue_icons/spectrum.png
+-rw-rw-rw-   0        0        0      605 2023-01-23 13:32:16.000000 wezel-0.1.2/src/wezel/icons/fugue_icons/tick-button.png
+-rw-rw-rw-   0        0        0      355 2023-01-23 13:32:16.000000 wezel-0.1.2/src/wezel/icons/fugue_icons/ui-check-box-uncheck.png
+-rw-rw-rw-   0        0        0      435 2023-01-23 13:32:16.000000 wezel-0.1.2/src/wezel/icons/fugue_icons/ui-check-box.png
+-rw-rw-rw-   0        0        0      725 2023-01-23 13:32:16.000000 wezel-0.1.2/src/wezel/icons/fugue_icons/wand-hat.png
+-rw-rw-rw-   0        0        0      610 2023-01-23 13:32:16.000000 wezel-0.1.2/src/wezel/icons/fugue_icons/wand.png
+drwxrwxrwx   0        0        0        0 2023-06-12 14:32:24.060113 wezel-0.1.2/src/wezel/icons/images/
+-rw-rw-rw-   0        0        0        0 2023-01-23 13:32:16.000000 wezel-0.1.2/src/wezel/icons/images/__init__.py
+-rw-rw-rw-   0        0        0   407459 2023-01-23 13:32:16.000000 wezel-0.1.2/src/wezel/icons/images/wezel.jpg
+-rw-rw-rw-   0        0        0     5730 2023-06-01 11:35:03.000000 wezel-0.1.2/src/wezel/icons/inventory.py
+drwxrwxrwx   0        0        0        0 2023-06-12 14:32:24.149379 wezel-0.1.2/src/wezel/icons/my_icons/
+-rw-rw-rw-   0        0        0        0 2023-01-23 13:32:16.000000 wezel-0.1.2/src/wezel/icons/my_icons/__init__.py
+-rw-rw-rw-   0        0        0     1406 2023-01-23 13:32:16.000000 wezel-0.1.2/src/wezel/icons/my_icons/favicon.ico
+-rw-rw-rw-   0        0        0    76029 2023-01-23 13:32:16.000000 wezel-0.1.2/src/wezel/icons/my_icons/question-mark.png
+-rw-rw-rw-   0        0        0      701 2023-01-23 13:32:16.000000 wezel-0.1.2/src/wezel/icons/my_icons/slider_icon.png
+-rw-rw-rw-   0        0        0  2170388 2023-06-01 11:34:16.000000 wezel-0.1.2/src/wezel/icons/my_icons/wezel-icon-transparent.png
+-rw-rw-rw-   0        0        0  1228073 2023-03-06 22:56:29.000000 wezel-0.1.2/src/wezel/icons/my_icons/wezel-icon.png
+drwxrwxrwx   0        0        0        0 2023-06-12 14:32:24.217941 wezel-0.1.2/src/wezel/menubar/
+-rw-rw-rw-   0        0        0       71 2023-03-17 15:55:49.000000 wezel-0.1.2/src/wezel/menubar/__init__.py
+-rw-rw-rw-   0        0        0      508 2023-06-12 14:10:17.000000 wezel-0.1.2/src/wezel/menubar/about.py
+-rw-rw-rw-   0        0        0    14348 2023-04-11 20:20:21.000000 wezel-0.1.2/src/wezel/menubar/edit.py
+-rw-rw-rw-   0        0        0     9671 2023-04-11 08:37:32.000000 wezel-0.1.2/src/wezel/menubar/folder.py
+-rw-rw-rw-   0        0        0     2464 2023-03-17 15:55:49.000000 wezel-0.1.2/src/wezel/menubar/view.py
+drwxrwxrwx   0        0        0        0 2023-06-12 14:32:24.327463 wezel-0.1.2/src/wezel/plugins/
+-rw-rw-rw-   0        0        0      309 2023-05-25 21:52:32.000000 wezel-0.1.2/src/wezel/plugins/align.py
+-rw-rw-rw-   0        0        0     9176 2023-04-13 16:49:07.000000 wezel-0.1.2/src/wezel/plugins/dipy.py
+-rw-rw-rw-   0        0        0     7379 2023-03-27 18:32:39.000000 wezel-0.1.2/src/wezel/plugins/elastix.py
+-rw-rw-rw-   0        0        0     2456 2023-03-17 15:55:49.000000 wezel-0.1.2/src/wezel/plugins/hello_world.py
+-rw-rw-rw-   0        0        0      245 2023-03-17 15:55:49.000000 wezel-0.1.2/src/wezel/plugins/measure.py
+-rw-rw-rw-   0        0        0     3592 2023-03-22 16:32:15.000000 wezel-0.1.2/src/wezel/plugins/numpy.py
+-rw-rw-rw-   0        0        0     9215 2023-05-31 08:42:50.000000 wezel-0.1.2/src/wezel/plugins/pyvista.py
+-rw-rw-rw-   0        0        0    35199 2023-03-29 21:46:01.000000 wezel-0.1.2/src/wezel/plugins/scipy.py
+-rw-rw-rw-   0        0        0     1048 2023-03-28 08:12:39.000000 wezel-0.1.2/src/wezel/plugins/segment.py
+-rw-rw-rw-   0        0        0    22528 2023-03-28 08:09:08.000000 wezel-0.1.2/src/wezel/plugins/skimage.py
+-rw-rw-rw-   0        0        0     3399 2023-03-28 08:00:21.000000 wezel-0.1.2/src/wezel/plugins/sklearn.py
+-rw-rw-rw-   0        0        0     1773 2023-04-11 20:49:36.000000 wezel-0.1.2/src/wezel/plugins/transform.py
+-rw-rw-rw-   0        0        0     4735 2023-05-30 16:06:21.000000 wezel-0.1.2/src/wezel/plugins/vreg.py
+drwxrwxrwx   0        0        0        0 2023-06-12 14:32:24.488400 wezel-0.1.2/src/wezel/widgets/
+-rw-rw-rw-   0        0        0      742 2023-03-13 10:39:12.000000 wezel-0.1.2/src/wezel/widgets/__init__.py
+-rw-rw-rw-   0        0        0     6622 2023-03-12 00:28:19.000000 wezel-0.1.2/src/wezel/widgets/dbdatabase.py
+-rw-rw-rw-   0        0        0    15974 2023-03-12 00:28:19.000000 wezel-0.1.2/src/wezel/widgets/dbimage.py
+-rw-rw-rw-   0        0        0      399 2023-03-12 00:27:43.000000 wezel-0.1.2/src/wezel/widgets/file_display.py
+-rw-rw-rw-   0        0        0     8756 2023-03-17 15:55:49.000000 wezel-0.1.2/src/wezel/widgets/log_to_GUI.py
+-rw-rw-rw-   0        0        0     2551 2023-03-12 00:28:19.000000 wezel-0.1.2/src/wezel/widgets/main_mdi.py
+-rw-rw-rw-   0        0        0     6698 2023-03-12 00:27:43.000000 wezel-0.1.2/src/wezel/widgets/message.py
+-rw-rw-rw-   0        0        0     2096 2023-03-12 00:27:43.000000 wezel-0.1.2/src/wezel/widgets/plot_curve.py
+-rw-rw-rw-   0        0        0    10227 2023-03-12 00:28:19.000000 wezel-0.1.2/src/wezel/widgets/qrangeslider.py
+-rw-rw-rw-   0        0        0     4029 2023-03-13 10:37:11.000000 wezel-0.1.2/src/wezel/widgets/region_list.py
+-rw-rw-rw-   0        0        0    11285 2023-03-12 00:28:19.000000 wezel-0.1.2/src/wezel/widgets/series_sliders.py
+-rw-rw-rw-   0        0        0     6936 2023-03-12 00:28:19.000000 wezel-0.1.2/src/wezel/widgets/sliders.py
+-rw-rw-rw-   0        0        0    11389 2023-03-24 11:11:20.000000 wezel-0.1.2/src/wezel/widgets/user_input.py
+drwxrwxrwx   0        0        0        0 2023-06-12 14:32:22.898397 wezel-0.1.2/src/wezel.egg-info/
+-rw-rw-rw-   0        0        0    14208 2023-06-12 14:32:22.000000 wezel-0.1.2/src/wezel.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0     5107 2023-06-12 14:32:22.000000 wezel-0.1.2/src/wezel.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-06-12 14:32:22.000000 wezel-0.1.2/src/wezel.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0      283 2023-06-12 14:32:22.000000 wezel-0.1.2/src/wezel.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        6 2023-06-12 14:32:22.000000 wezel-0.1.2/src/wezel.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-06-12 14:32:24.491432 wezel-0.1.2/tests/
+-rw-rw-rw-   0        0        0     8245 2023-03-12 00:27:43.000000 wezel-0.1.2/tests/test_wezel.py
```

### filetype from file(1)

```diff
@@ -1 +1 @@
-POSIX tar archive (GNU)
+POSIX tar archive
```

### Comparing `wezel-0.1.1/LICENSE` & `wezel-0.1.2/LICENSE`

 * *Files identical despite different names*

### Comparing `wezel-0.1.1/PKG-INFO` & `wezel-0.1.2/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 Metadata-Version: 2.1
 Name: wezel
-Version: 0.1.1
+Version: 0.1.2
 Summary: Prototyping medical imaging applications
-Author-email: Steve Shillitoe <s.shillitoe@sheffield.ac.uk>, Joao Almeida e Sousa <j.g.sousa@sheffield.ac.uk>, Steven Sourbron <s.sourbron@sheffield.ac.uk>
+Author-email: Steven Sourbron <s.sourbron@sheffield.ac.uk>, Steve Shillitoe <s.shillitoe@sheffield.ac.uk>, Joao Almeida e Sousa <j.g.sousa@sheffield.ac.uk>
 License: Apache License
                                    Version 2.0, January 2004
                                 http://www.apache.org/licenses/
         
            TERMS AND CONDITIONS FOR USE, REPRODUCTION, AND DISTRIBUTION
         
            1. Definitions.
@@ -212,16 +212,16 @@
 Classifier: Intended Audience :: Science/Research
 Classifier: Topic :: Scientific/Engineering
 Classifier: Environment :: Console
 Classifier: Operating System :: OS Independent
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
-Requires-Python: >=3.6
+Requires-Python: <3.11,>=3.7
 Description-Content-Type: text/markdown
 Provides-Extra: docs
-Provides-Extra: executable
+Provides-Extra: plugins
 License-File: LICENSE
 
 `wezel` is a Python toolbox for prototyping medical imaging applications. 
 
 ***wezel is work in progress.***
```

### Comparing `wezel-0.1.1/pyproject.toml` & `wezel-0.1.2/pyproject.toml`

 * *Files 25% similar despite different names*

```diff
@@ -4,137 +4,202 @@
 00000030: 2d62 6163 6b65 6e64 203d 2022 7365 7475  -backend = "setu
 00000040: 7074 6f6f 6c73 2e62 7569 6c64 5f6d 6574  ptools.build_met
 00000050: 6122 0d0a 0d0a 2320 6d69 6e69 6d61 6c20  a"....# minimal 
 00000060: 7265 7175 6972 6564 2069 6e66 6f72 6d61  required informa
 00000070: 7469 6f6e 0d0a 0d0a 5b70 726f 6a65 6374  tion....[project
 00000080: 5d0d 0a6e 616d 6520 3d20 2277 657a 656c  ]..name = "wezel
 00000090: 220d 0a76 6572 7369 6f6e 203d 2022 302e  "..version = "0.
-000000a0: 312e 3122 0d0a 6465 7065 6e64 656e 6369  1.1"..dependenci
-000000b0: 6573 203d 205b 0d0a 2020 2250 7951 7435  es = [..  "PyQt5
-000000c0: 3c3d 352e 3133 2e31 222c 2020 2320 666f  <=5.13.1",  # fo
-000000d0: 756e 6420 736f 6d65 2072 6573 6f6c 7574  und some resolut
-000000e0: 696f 6e20 6973 7375 6573 2077 6974 6820  ion issues with 
-000000f0: 6c61 7465 7220 7665 7273 696f 6e73 0d0a  later versions..
-00000100: 2020 2264 6264 6963 6f6d 222c 0d0a 2020    "dbdicom",..  
-00000110: 226d 6174 706c 6f74 6c69 6222 2c0d 0a20  "matplotlib",.. 
-00000120: 2022 6e75 6d70 7922 2c0d 0a20 2022 7061   "numpy",..  "pa
-00000130: 6e64 6173 222c 0d0a 2020 2269 6d70 6f72  ndas",..  "impor
-00000140: 746c 6962 2d72 6573 6f75 7263 6573 3e3d  tlib-resources>=
-00000150: 312e 312e 3022 2c0d 0a20 2022 6f70 656e  1.1.0",..  "open
-00000160: 6376 2d70 7974 686f 6e3c 3d34 2e35 2e33  cv-python<=4.5.3
-00000170: 2e35 3622 2c20 2320 6861 636b 2074 6f20  .56", # hack to 
-00000180: 6669 7820 6120 6275 6720 696e 2062 7569  fix a bug in bui
-00000190: 6c64 696e 6720 6578 6563 7574 6162 6c65  lding executable
-000001a0: 0d0a 2020 2320 436f 6e73 6964 6572 2072  ..  # Consider r
-000001b0: 656d 6f76 696e 6720 6c69 6d69 7420 6f6e  emoving limit on
-000001c0: 206f 7065 6e2d 6376 7665 7273 696f 6e20   open-cvversion 
-000001d0: 6e75 6d62 6572 200d 0a20 2023 202d 3e20  number ..  # -> 
-000001e0: 6372 6561 7465 7320 696e 7374 616c 6c61  creates installa
-000001f0: 7469 6f6e 2069 7373 7565 7320 2877 6865  tion issues (whe
-00000200: 656c 206e 6f20 6c6f 6e67 6572 2075 7020  el no longer up 
-00000210: 746f 2064 6174 6529 0d0a 2020 2320 4f72  to date)..  # Or
-00000220: 2063 6f6e 7369 6465 7220 7265 6d6f 7669   consider removi
-00000230: 6e67 206f 7065 6e63 7620 6173 2064 6570  ng opencv as dep
-00000240: 656e 6465 6e63 792e 2049 7320 7363 696b  endency. Is scik
-00000250: 6974 206e 6f74 2065 6e6f 7567 683f 0d0a  it not enough?..
-00000260: 2020 2273 6369 6b69 742d 696d 6167 6522    "scikit-image"
-00000270: 2c0d 0a20 2022 7363 6970 7922 2c0d 0a5d  ,..  "scipy",..]
-00000280: 0d0a 0d0a 2320 6f70 7469 6f6e 616c 2069  ....# optional i
-00000290: 6e66 6f72 6d61 7469 6f6e 0d0a 0d0a 6465  nformation....de
-000002a0: 7363 7269 7074 696f 6e20 3d20 2250 726f  scription = "Pro
-000002b0: 746f 7479 7069 6e67 206d 6564 6963 616c  totyping medical
-000002c0: 2069 6d61 6769 6e67 2061 7070 6c69 6361   imaging applica
-000002d0: 7469 6f6e 7322 0d0a 7265 6164 6d65 203d  tions"..readme =
-000002e0: 2022 5245 4144 4d45 2e6d 6422 0d0a 6175   "README.md"..au
-000002f0: 7468 6f72 7320 3d20 5b0d 0a20 207b 206e  thors = [..  { n
-00000300: 616d 6520 3d20 2253 7465 7665 2053 6869  ame = "Steve Shi
-00000310: 6c6c 6974 6f65 222c 2065 6d61 696c 203d  llitoe", email =
-00000320: 2022 732e 7368 696c 6c69 746f 6540 7368   "s.shillitoe@sh
-00000330: 6566 6669 656c 642e 6163 2e75 6b22 207d  effield.ac.uk" }
-00000340: 2c0d 0a20 207b 206e 616d 6520 3d20 224a  ,..  { name = "J
-00000350: 6f61 6f20 416c 6d65 6964 6120 6520 536f  oao Almeida e So
-00000360: 7573 6122 2c20 656d 6169 6c20 3d20 226a  usa", email = "j
-00000370: 2e67 2e73 6f75 7361 4073 6865 6666 6965  .g.sousa@sheffie
-00000380: 6c64 2e61 632e 756b 2220 7d2c 200d 0a20  ld.ac.uk" }, .. 
-00000390: 207b 206e 616d 6520 3d20 2253 7465 7665   { name = "Steve
-000003a0: 6e20 536f 7572 6272 6f6e 222c 2065 6d61  n Sourbron", ema
-000003b0: 696c 203d 2022 732e 736f 7572 6272 6f6e  il = "s.sourbron
-000003c0: 4073 6865 6666 6965 6c64 2e61 632e 756b  @sheffield.ac.uk
-000003d0: 2220 7d0d 0a20 205d 0d0a 6c69 6365 6e73  " }..  ]..licens
-000003e0: 6520 3d20 7b20 6669 6c65 203d 2022 4c49  e = { file = "LI
-000003f0: 4345 4e53 4522 207d 0d0a 636c 6173 7369  CENSE" }..classi
-00000400: 6669 6572 7320 3d20 5b0d 0a20 2023 2048  fiers = [..  # H
-00000410: 6f77 206d 6174 7572 6520 6973 2074 6869  ow mature is thi
-00000420: 7320 7072 6f6a 6563 743f 2043 6f6d 6d6f  s project? Commo
-00000430: 6e20 7661 6c75 6573 2061 7265 0d0a 2020  n values are..  
-00000440: 2320 2020 3320 2d20 416c 7068 610d 0a20  #   3 - Alpha.. 
-00000450: 2023 2020 2034 202d 2042 6574 610d 0a20   #   4 - Beta.. 
-00000460: 2023 2020 2035 202d 2050 726f 6475 6374   #   5 - Product
-00000470: 696f 6e2f 5374 6162 6c65 0d0a 2020 2744  ion/Stable..  'D
-00000480: 6576 656c 6f70 6d65 6e74 2053 7461 7475  evelopment Statu
-00000490: 7320 3a3a 2033 202d 2041 6c70 6861 272c  s :: 3 - Alpha',
-000004a0: 0d0a 0d0a 2020 2320 496e 6469 6361 7465  ....  # Indicate
-000004b0: 2077 686f 2079 6f75 7220 7072 6f6a 6563   who your projec
-000004c0: 7420 6973 2069 6e74 656e 6465 6420 666f  t is intended fo
-000004d0: 720d 0a20 2027 496e 7465 6e64 6564 2041  r..  'Intended A
-000004e0: 7564 6965 6e63 6520 3a3a 2044 6576 656c  udience :: Devel
-000004f0: 6f70 6572 7327 2c0d 0a20 2027 496e 7465  opers',..  'Inte
-00000500: 6e64 6564 2041 7564 6965 6e63 6520 3a3a  nded Audience ::
-00000510: 2053 6369 656e 6365 2f52 6573 6561 7263   Science/Researc
-00000520: 6827 2c0d 0a20 2027 546f 7069 6320 3a3a  h',..  'Topic ::
-00000530: 2053 6369 656e 7469 6669 632f 456e 6769   Scientific/Engi
-00000540: 6e65 6572 696e 6727 2c0d 0a20 2027 456e  neering',..  'En
-00000550: 7669 726f 6e6d 656e 7420 3a3a 2043 6f6e  vironment :: Con
-00000560: 736f 6c65 272c 0d0a 2020 274f 7065 7261  sole',..  'Opera
-00000570: 7469 6e67 2053 7973 7465 6d20 3a3a 204f  ting System :: O
-00000580: 5320 496e 6465 7065 6e64 656e 7427 2c0d  S Independent',.
-00000590: 0a0d 0a20 2027 4c69 6365 6e73 6520 3a3a  ...  'License ::
-000005a0: 204f 5349 2041 7070 726f 7665 6420 3a3a   OSI Approved ::
-000005b0: 2041 7061 6368 6520 536f 6674 7761 7265   Apache Software
-000005c0: 204c 6963 656e 7365 272c 0d0a 2020 2250   License',..  "P
-000005d0: 726f 6772 616d 6d69 6e67 204c 616e 6775  rogramming Langu
-000005e0: 6167 6520 3a3a 2050 7974 686f 6e22 2c0d  age :: Python",.
-000005f0: 0a20 2022 5072 6f67 7261 6d6d 696e 6720  .  "Programming 
-00000600: 4c61 6e67 7561 6765 203a 3a20 5079 7468  Language :: Pyth
-00000610: 6f6e 203a 3a20 3322 0d0a 5d0d 0a6b 6579  on :: 3"..]..key
-00000620: 776f 7264 7320 3d20 5b27 7079 7468 6f6e  words = ['python
-00000630: 272c 2022 6d65 6469 6361 6c20 696d 6167  ', "medical imag
-00000640: 696e 6722 2c20 2247 7261 7068 6963 616c  ing", "Graphical
-00000650: 2055 7365 7220 496e 7465 7266 6163 6522   User Interface"
-00000660: 5d0d 0a0d 0a72 6571 7569 7265 732d 7079  ]....requires-py
-00000670: 7468 6f6e 203d 2022 3e3d 332e 3622 0d0a  thon = ">=3.6"..
-00000680: 0d0a 5b70 726f 6a65 6374 2e75 726c 735d  ..[project.urls]
-00000690: 0d0a 2248 6f6d 6570 6167 6522 203d 2022  .."Homepage" = "
-000006a0: 6874 7470 733a 2f2f 6769 7468 7562 2e63  https://github.c
-000006b0: 6f6d 2f51 4942 2d53 6865 6666 6965 6c64  om/QIB-Sheffield
-000006c0: 2f77 657a 656c 220d 0a0d 0a0d 0a5b 746f  /wezel"......[to
-000006d0: 6f6c 2e73 6574 7570 746f 6f6c 735d 0d0a  ol.setuptools]..
-000006e0: 2320 2e2e 2e0d 0a23 2042 7920 6465 6661  # .....# By defa
-000006f0: 756c 742c 2069 6e63 6c75 6465 2d70 6163  ult, include-pac
-00000700: 6b61 6765 2d64 6174 6120 6973 2074 7275  kage-data is tru
-00000710: 6520 696e 2070 7970 726f 6a65 6374 2e74  e in pyproject.t
-00000720: 6f6d 6c2c 2073 6f20 796f 7520 646f 0d0a  oml, so you do..
-00000730: 2320 4e4f 5420 6861 7665 2074 6f20 7370  # NOT have to sp
-00000740: 6563 6966 7920 7468 6973 206c 696e 652e  ecify this line.
-00000750: 0d0a 696e 636c 7564 652d 7061 636b 6167  ..include-packag
-00000760: 652d 6461 7461 203d 2074 7275 650d 0a0d  e-data = true...
-00000770: 0a0d 0a5b 746f 6f6c 2e73 6574 7570 746f  ...[tool.setupto
-00000780: 6f6c 732e 7061 636b 6167 6573 2e66 696e  ols.packages.fin
-00000790: 645d 0d0a 7768 6572 6520 3d20 5b22 7372  d]..where = ["sr
-000007a0: 6322 5d0d 0a0d 0a5b 7072 6f6a 6563 742e  c"]....[project.
-000007b0: 6f70 7469 6f6e 616c 2d64 6570 656e 6465  optional-depende
-000007c0: 6e63 6965 735d 0d0a 2320 696d 706f 7274  ncies]..# import
-000007d0: 6c69 622d 7265 736f 7572 6365 7320 2320  lib-resources # 
-000007e0: 7265 6d6f 7665 6420 2d20 6e65 6365 7373  removed - necess
-000007f0: 6172 793f 2077 6865 7265 3f0d 0a64 6f63  ary? where?..doc
-00000800: 7320 3d20 5b0d 0a20 2020 2022 7370 6869  s = [..    "sphi
-00000810: 6e78 222c 0d0a 2020 2020 2273 7068 696e  nx",..    "sphin
-00000820: 785f 7274 645f 7468 656d 6522 2c0d 0a20  x_rtd_theme",.. 
-00000830: 2020 2022 6d79 7374 2d70 6172 7365 7222     "myst-parser"
-00000840: 2c20 0d0a 2020 2020 2273 7068 696e 782d  , ..    "sphinx-
-00000850: 636f 7079 6275 7474 6f6e 222c 0d0a 2020  copybutton",..  
-00000860: 2020 2273 7068 696e 782d 7265 6d6f 7665    "sphinx-remove
-00000870: 2d74 6f63 7472 6565 7322 2c0d 0a5d 0d0a  -toctrees",..]..
-00000880: 6578 6563 7574 6162 6c65 203d 205b 200d  executable = [ .
-00000890: 0a20 2027 7079 696e 7374 616c 6c65 7227  .  'pyinstaller'
-000008a0: 2c0d 0a5d 0d0a 0d0a 0d0a 0d0a 0d0a 0d0a  ,..]............
-000008b0: 0d0a 0d0a 0d0a                           ......
+000000a0: 312e 3222 0d0a 6465 7065 6e64 656e 6369  1.2"..dependenci
+000000b0: 6573 203d 205b 0d0a 2020 2250 7953 6964  es = [..  "PySid
+000000c0: 6532 222c 0d0a 2020 2264 6264 6963 6f6d  e2",..  "dbdicom
+000000d0: 222c 0d0a 2020 226d 6174 706c 6f74 6c69  ",..  "matplotli
+000000e0: 6222 2c20 2320 666f 7220 706c 6f74 7469  b", # for plotti
+000000f0: 6e67 2063 7572 7665 7320 616e 6420 6372  ng curves and cr
+00000100: 6561 7469 6e67 2063 6f6c 6f72 6d61 7073  eating colormaps
+00000110: 0d0a 2020 226e 756d 7079 222c 0d0a 2020  ..  "numpy",..  
+00000120: 2270 616e 6461 7322 2c0d 0a20 2022 6f70  "pandas",..  "op
+00000130: 656e 7079 786c 222c 2023 2072 6571 7569  enpyxl", # requi
+00000140: 7265 6420 666f 7220 7061 6e64 6173 2065  red for pandas e
+00000150: 7870 6f72 7420 746f 2065 7863 656c 0d0a  xport to excel..
+00000160: 2020 2269 6d70 6f72 746c 6962 2d72 6573    "importlib-res
+00000170: 6f75 7263 6573 3e3d 312e 312e 3022 2c20  ources>=1.1.0", 
+00000180: 2320 666f 7220 6963 6f6e 2069 6e76 656e  # for icon inven
+00000190: 746f 7279 0d0a 0d0a 2020 2320 5573 696e  tory....  # Usin
+000001a0: 6720 6f6e 6c79 2064 696c 6174 6520 616e  g only dilate an
+000001b0: 6420 6572 6f64 6520 6675 6e63 7469 6f6e  d erode function
+000001c0: 7320 2d20 7265 706c 6163 6520 6279 2073  s - replace by s
+000001d0: 6b69 6d61 6765 0d0a 2020 2320 226f 7065  kimage..  # "ope
+000001e0: 6e63 762d 7079 7468 6f6e 3c3d 342e 352e  ncv-python<=4.5.
+000001f0: 332e 3536 222c 2023 2070 7265 7669 6f75  3.56", # previou
+00000200: 7320 6861 636b 2074 6f20 6669 7820 6120  s hack to fix a 
+00000210: 6275 6720 696e 2062 7569 6c64 696e 6720  bug in building 
+00000220: 6578 6563 7574 6162 6c65 0d0a 2020 2320  executable..  # 
+00000230: 436f 6e73 6964 6572 2072 656d 6f76 696e  Consider removin
+00000240: 6720 6c69 6d69 7420 6f6e 206f 7065 6e2d  g limit on open-
+00000250: 6376 7665 7273 696f 6e20 6e75 6d62 6572  cvversion number
+00000260: 200d 0a20 2023 202d 3e20 6372 6561 7465   ..  # -> create
+00000270: 7320 696e 7374 616c 6c61 7469 6f6e 2069  s installation i
+00000280: 7373 7565 7320 2877 6865 656c 206e 6f20  ssues (wheel no 
+00000290: 6c6f 6e67 6572 2075 7020 746f 2064 6174  longer up to dat
+000002a0: 6529 0d0a 2020 226f 7065 6e63 762d 7079  e)..  "opencv-py
+000002b0: 7468 6f6e 222c 0d0a 0d0a 2020 2320 7265  thon",....  # re
+000002c0: 7374 7269 6374 696e 6720 746f 2074 6865  stricting to the
+000002d0: 206c 6174 6573 7420 7374 6162 6c65 2072   latest stable r
+000002e0: 656c 6561 7365 2066 6f72 206e 6f77 2064  elease for now d
+000002f0: 7565 2074 6f20 6120 6275 670d 0a20 2023  ue to a bug..  #
+00000300: 2069 6e74 726f 6475 6365 6420 696e 2030   introduced in 0
+00000310: 2e32 302e 3020 7468 6174 2063 6175 7365  .20.0 that cause
+00000320: 7320 6578 6563 7574 6162 6c65 7320 746f  s executables to
+00000330: 2063 7261 7368 2e20 5468 6520 6275 6720   crash. The bug 
+00000340: 6973 206b 6e6f 776e 0d0a 2020 2320 616e  is known..  # an
+00000350: 6420 6120 6669 7820 7769 6c6c 2070 7265  d a fix will pre
+00000360: 7375 6d61 626c 7920 6265 2069 6e63 6c75  sumably be inclu
+00000370: 6465 6420 696e 2075 7063 6f6d 696e 6720  ded in upcoming 
+00000380: 7265 6c65 6173 6573 0d0a 2020 2320 696e  releases..  # in
+00000390: 2077 6869 6368 2063 6173 6520 7468 6973   which case this
+000003a0: 2072 6573 7472 6963 7469 6f6e 2063 616e   restriction can
+000003b0: 2062 6520 7265 6d6f 7665 642e 0d0a 2020   be removed...  
+000003c0: 2320 6874 7470 733a 2f2f 6769 7468 7562  # https://github
+000003d0: 2e63 6f6d 2f73 6369 6b69 742d 696d 6167  .com/scikit-imag
+000003e0: 652f 7363 696b 6974 2d69 6d61 6765 2f69  e/scikit-image/i
+000003f0: 7373 7565 732f 3637 3834 0d0a 2020 2320  ssues/6784..  # 
+00000400: 6874 7470 733a 2f2f 6769 7468 7562 2e63  https://github.c
+00000410: 6f6d 2f73 6369 656e 7469 6669 632d 7079  om/scientific-py
+00000420: 7468 6f6e 2f6c 617a 795f 6c6f 6164 6572  thon/lazy_loader
+00000430: 2f70 756c 6c2f 3339 0d0a 2020 2320 4e6f  /pull/39..  # No
+00000440: 7465 206f 6e20 7079 746f 6e20 332e 3131  te on pyton 3.11
+00000450: 2073 6369 6b69 7420 696d 6167 6520 6d75   scikit image mu
+00000460: 7374 2062 6520 696e 7374 616c 6c65 6420  st be installed 
+00000470: 6173 0d0a 2020 2320 7069 7020 696e 7374  as..  # pip inst
+00000480: 616c 6c20 2d2d 7072 6520 7363 696b 6974  all --pre scikit
+00000490: 2d69 6d61 6765 3c3d 302e 3139 2e30 200d  -image<=0.19.0 .
+000004a0: 0a20 2023 2075 6e74 696c 2061 206e 6577  .  # until a new
+000004b0: 2076 6572 7369 6f6e 2069 7320 7265 6c65   version is rele
+000004c0: 6173 6564 2028 302e 3231 2e30 290d 0a20  ased (0.21.0).. 
+000004d0: 2022 7363 696b 6974 2d69 6d61 6765 3c3d   "scikit-image<=
+000004e0: 302e 3139 2e30 222c 0d0a 2020 0d0a 2020  0.19.0",..  ..  
+000004f0: 2320 5468 6973 2068 6173 2062 6563 6f6d  # This has becom
+00000500: 6520 7061 7274 206f 6620 7765 7a65 6c20  e part of wezel 
+00000510: 2d20 7061 636b 6167 6520 696e 636c 7564  - package includ
+00000520: 6573 2061 7069 2773 2074 6f20 6372 6561  es api's to crea
+00000530: 7465 2065 7865 6375 7461 626c 6573 0d0a  te executables..
+00000540: 2020 2320 7061 636b 6167 6520 6d61 6e61    # package mana
+00000550: 6765 7220 6d6f 6475 6c65 206e 6565 6473  ger module needs
+00000560: 2065 7874 656e 6469 6e67 2074 686f 7567   extending thoug
+00000570: 680d 0a20 2027 7079 696e 7374 616c 6c65  h..  'pyinstalle
+00000580: 7227 2c20 0d0a 0d0a 2020 2273 6369 7079  r', ....  "scipy
+00000590: 222c 2023 2063 7572 7265 6e74 6c79 206f  ", # currently o
+000005a0: 6e6c 7920 7573 6564 2069 6e20 7375 7266  nly used in surf
+000005b0: 6163 6520 6469 7370 6c61 7920 616e 6420  ace display and 
+000005c0: 7468 6520 7368 6966 7420 6675 6e63 7469  the shift functi
+000005d0: 6f6e 2069 6e20 6d61 736b 5f66 696c 7465  on in mask_filte
+000005e0: 7220 2863 616e 2062 6520 7265 706c 6163  r (can be replac
+000005f0: 6564 290d 0a5d 0d0a 0d0a 2320 6f70 7469  ed)..]....# opti
+00000600: 6f6e 616c 2069 6e66 6f72 6d61 7469 6f6e  onal information
+00000610: 0d0a 0d0a 6465 7363 7269 7074 696f 6e20  ....description 
+00000620: 3d20 2250 726f 746f 7479 7069 6e67 206d  = "Prototyping m
+00000630: 6564 6963 616c 2069 6d61 6769 6e67 2061  edical imaging a
+00000640: 7070 6c69 6361 7469 6f6e 7322 0d0a 7265  pplications"..re
+00000650: 6164 6d65 203d 2022 5245 4144 4d45 2e6d  adme = "README.m
+00000660: 6422 0d0a 6175 7468 6f72 7320 3d20 5b0d  d"..authors = [.
+00000670: 0a20 207b 206e 616d 6520 3d20 2253 7465  .  { name = "Ste
+00000680: 7665 6e20 536f 7572 6272 6f6e 222c 2065  ven Sourbron", e
+00000690: 6d61 696c 203d 2022 732e 736f 7572 6272  mail = "s.sourbr
+000006a0: 6f6e 4073 6865 6666 6965 6c64 2e61 632e  on@sheffield.ac.
+000006b0: 756b 2220 7d2c 0d0a 2020 7b20 6e61 6d65  uk" },..  { name
+000006c0: 203d 2022 5374 6576 6520 5368 696c 6c69   = "Steve Shilli
+000006d0: 746f 6522 2c20 656d 6169 6c20 3d20 2273  toe", email = "s
+000006e0: 2e73 6869 6c6c 6974 6f65 4073 6865 6666  .shillitoe@sheff
+000006f0: 6965 6c64 2e61 632e 756b 2220 7d2c 0d0a  ield.ac.uk" },..
+00000700: 2020 7b20 6e61 6d65 203d 2022 4a6f 616f    { name = "Joao
+00000710: 2041 6c6d 6569 6461 2065 2053 6f75 7361   Almeida e Sousa
+00000720: 222c 2065 6d61 696c 203d 2022 6a2e 672e  ", email = "j.g.
+00000730: 736f 7573 6140 7368 6566 6669 656c 642e  sousa@sheffield.
+00000740: 6163 2e75 6b22 207d 2c20 0d0a 2020 5d0d  ac.uk" }, ..  ].
+00000750: 0a6c 6963 656e 7365 203d 207b 2066 696c  .license = { fil
+00000760: 6520 3d20 224c 4943 454e 5345 2220 7d0d  e = "LICENSE" }.
+00000770: 0a63 6c61 7373 6966 6965 7273 203d 205b  .classifiers = [
+00000780: 0d0a 2020 2320 486f 7720 6d61 7475 7265  ..  # How mature
+00000790: 2069 7320 7468 6973 2070 726f 6a65 6374   is this project
+000007a0: 3f20 436f 6d6d 6f6e 2076 616c 7565 7320  ? Common values 
+000007b0: 6172 650d 0a20 2023 2020 2033 202d 2041  are..  #   3 - A
+000007c0: 6c70 6861 0d0a 2020 2320 2020 3420 2d20  lpha..  #   4 - 
+000007d0: 4265 7461 0d0a 2020 2320 2020 3520 2d20  Beta..  #   5 - 
+000007e0: 5072 6f64 7563 7469 6f6e 2f53 7461 626c  Production/Stabl
+000007f0: 650d 0a20 2027 4465 7665 6c6f 706d 656e  e..  'Developmen
+00000800: 7420 5374 6174 7573 203a 3a20 3320 2d20  t Status :: 3 - 
+00000810: 416c 7068 6127 2c0d 0a0d 0a20 2023 2049  Alpha',....  # I
+00000820: 6e64 6963 6174 6520 7768 6f20 796f 7572  ndicate who your
+00000830: 2070 726f 6a65 6374 2069 7320 696e 7465   project is inte
+00000840: 6e64 6564 2066 6f72 0d0a 2020 2749 6e74  nded for..  'Int
+00000850: 656e 6465 6420 4175 6469 656e 6365 203a  ended Audience :
+00000860: 3a20 4465 7665 6c6f 7065 7273 272c 0d0a  : Developers',..
+00000870: 2020 2749 6e74 656e 6465 6420 4175 6469    'Intended Audi
+00000880: 656e 6365 203a 3a20 5363 6965 6e63 652f  ence :: Science/
+00000890: 5265 7365 6172 6368 272c 0d0a 2020 2754  Research',..  'T
+000008a0: 6f70 6963 203a 3a20 5363 6965 6e74 6966  opic :: Scientif
+000008b0: 6963 2f45 6e67 696e 6565 7269 6e67 272c  ic/Engineering',
+000008c0: 0d0a 2020 2745 6e76 6972 6f6e 6d65 6e74  ..  'Environment
+000008d0: 203a 3a20 436f 6e73 6f6c 6527 2c0d 0a20   :: Console',.. 
+000008e0: 2027 4f70 6572 6174 696e 6720 5379 7374   'Operating Syst
+000008f0: 656d 203a 3a20 4f53 2049 6e64 6570 656e  em :: OS Indepen
+00000900: 6465 6e74 272c 0d0a 0d0a 2020 274c 6963  dent',....  'Lic
+00000910: 656e 7365 203a 3a20 4f53 4920 4170 7072  ense :: OSI Appr
+00000920: 6f76 6564 203a 3a20 4170 6163 6865 2053  oved :: Apache S
+00000930: 6f66 7477 6172 6520 4c69 6365 6e73 6527  oftware License'
+00000940: 2c0d 0a20 2022 5072 6f67 7261 6d6d 696e  ,..  "Programmin
+00000950: 6720 4c61 6e67 7561 6765 203a 3a20 5079  g Language :: Py
+00000960: 7468 6f6e 222c 0d0a 2020 2250 726f 6772  thon",..  "Progr
+00000970: 616d 6d69 6e67 204c 616e 6775 6167 6520  amming Language 
+00000980: 3a3a 2050 7974 686f 6e20 3a3a 2033 220d  :: Python :: 3".
+00000990: 0a5d 0d0a 6b65 7977 6f72 6473 203d 205b  .]..keywords = [
+000009a0: 2770 7974 686f 6e27 2c20 226d 6564 6963  'python', "medic
+000009b0: 616c 2069 6d61 6769 6e67 222c 2022 4772  al imaging", "Gr
+000009c0: 6170 6869 6361 6c20 5573 6572 2049 6e74  aphical User Int
+000009d0: 6572 6661 6365 225d 0d0a 0d0a 2320 4578  erface"]....# Ex
+000009e0: 636c 7564 696e 6720 332e 3131 2066 6f72  cluding 3.11 for
+000009f0: 206e 6f77 2061 7320 736f 6d65 2070 6163   now as some pac
+00000a00: 6b61 6765 7320 646f 6e27 7420 6861 7665  kages don't have
+00000a10: 2077 6865 656c 7320 7965 740d 0a23 2045   wheels yet..# E
+00000a20: 7861 6d70 6c65 2073 6369 6b69 742d 696d  xample scikit-im
+00000a30: 6167 6520 2863 6f6d 696e 6720 696e 2074  age (coming in t
+00000a40: 6865 206e 6578 7420 7665 7273 696f 6e29  he next version)
+00000a50: 0d0a 7265 7175 6972 6573 2d70 7974 686f  ..requires-pytho
+00000a60: 6e20 3d20 223e 3d33 2e37 2c20 3c33 2e31  n = ">=3.7, <3.1
+00000a70: 3122 200d 0a0d 0a5b 7072 6f6a 6563 742e  1" ....[project.
+00000a80: 7572 6c73 5d0d 0a22 486f 6d65 7061 6765  urls].."Homepage
+00000a90: 2220 3d20 2268 7474 7073 3a2f 2f67 6974  " = "https://git
+00000aa0: 6875 622e 636f 6d2f 5149 422d 5368 6566  hub.com/QIB-Shef
+00000ab0: 6669 656c 642f 7765 7a65 6c22 0d0a 0d0a  field/wezel"....
+00000ac0: 0d0a 5b74 6f6f 6c2e 7365 7475 7074 6f6f  ..[tool.setuptoo
+00000ad0: 6c73 5d0d 0a23 202e 2e2e 0d0a 2320 4279  ls]..# .....# By
+00000ae0: 2064 6566 6175 6c74 2c20 696e 636c 7564   default, includ
+00000af0: 652d 7061 636b 6167 652d 6461 7461 2069  e-package-data i
+00000b00: 7320 7472 7565 2069 6e20 7079 7072 6f6a  s true in pyproj
+00000b10: 6563 742e 746f 6d6c 2c20 736f 2079 6f75  ect.toml, so you
+00000b20: 2064 6f0d 0a23 204e 4f54 2068 6176 6520   do..# NOT have 
+00000b30: 746f 2073 7065 6369 6679 2074 6869 7320  to specify this 
+00000b40: 6c69 6e65 2e0d 0a69 6e63 6c75 6465 2d70  line...include-p
+00000b50: 6163 6b61 6765 2d64 6174 6120 3d20 7472  ackage-data = tr
+00000b60: 7565 0d0a 0d0a 0d0a 5b74 6f6f 6c2e 7365  ue......[tool.se
+00000b70: 7475 7074 6f6f 6c73 2e70 6163 6b61 6765  tuptools.package
+00000b80: 732e 6669 6e64 5d0d 0a77 6865 7265 203d  s.find]..where =
+00000b90: 205b 2273 7263 225d 0d0a 0d0a 5b70 726f   ["src"]....[pro
+00000ba0: 6a65 6374 2e6f 7074 696f 6e61 6c2d 6465  ject.optional-de
+00000bb0: 7065 6e64 656e 6369 6573 5d0d 0a0d 0a64  pendencies]....d
+00000bc0: 6f63 7320 3d20 5b0d 0a20 2020 2022 7370  ocs = [..    "sp
+00000bd0: 6869 6e78 222c 0d0a 2020 2020 2273 7068  hinx",..    "sph
+00000be0: 696e 785f 7274 645f 7468 656d 6522 2c0d  inx_rtd_theme",.
+00000bf0: 0a20 2020 2022 6d79 7374 2d70 6172 7365  .    "myst-parse
+00000c00: 7222 2c20 0d0a 2020 2020 2273 7068 696e  r", ..    "sphin
+00000c10: 782d 636f 7079 6275 7474 6f6e 222c 0d0a  x-copybutton",..
+00000c20: 2020 2020 2273 7068 696e 782d 7265 6d6f      "sphinx-remo
+00000c30: 7665 2d74 6f63 7472 6565 7322 2c0d 0a5d  ve-toctrees",..]
+00000c40: 0d0a 706c 7567 696e 7320 3d20 5b0d 0a20  ..plugins = [.. 
+00000c50: 2022 6469 7079 222c 0d0a 2020 2253 696d   "dipy",..  "Sim
+00000c60: 706c 6549 544b 222c 0d0a 2020 2269 746b  pleITK",..  "itk
+00000c70: 2d65 6c61 7374 6978 222c 0d0a 2020 2273  -elastix",..  "s
+00000c80: 6369 6b69 742d 6c65 6172 6e22 2c0d 0a20  cikit-learn",.. 
+00000c90: 2022 7079 7669 7374 6122 2c20 0d0a 2020   "pyvista", ..  
+00000ca0: 2270 7976 6973 7461 7174 222c 200d 0a5d  "pyvistaqt", ..]
+00000cb0: 0d0a 0d0a 0d0a 0d0a 0d0a 0d0a 0d0a 0d0a  ................
+00000cc0: 0d0a                                     ..
```

### Comparing `wezel-0.1.1/src/wezel/actions/edit.py` & `wezel-0.1.2/src/wezel/menubar/edit.py`

 * *Files 17% similar despite different names*

```diff
@@ -1,416 +1,375 @@
-import numpy as np
 import dbdicom as db
-import wezel
+from wezel.gui import Menu, Action
 
 
-def all(parent):
-
-    parent.action(DeleteSeries, text='Series > Delete')
-    parent.action(Copy, text='Series > Copy', generation=3)
-    parent.action(CopySeries, text='Series > Copy to..')
-    parent.action(MoveSeries, text='Series > Move to..')
-    parent.action(MergeSeries, text='Series > Merge')
-    parent.action(GroupSeries, text='Series > Group')
-    parent.action(SeriesRename, text='Series > Rename')
-    parent.action(SeriesExtractByIndex, text='Series > Extract subseries (by index)')
-    parent.action(SeriesExtractByValue, text='Series > Extract subseries (by value)')
-    parent.separator()
-    parent.action(DeleteStudies, text='Studies > Delete')
-    parent.action(Copy, text='Studies > Copy', generation=2)
-    parent.action(CopyStudies, text='Studies > Copy to..')
-    parent.action(MoveStudies, text='Studies > Move to..')
-    parent.action(MergeStudies, text='Studies > Merge')
-    parent.action(GroupStudies, text='Studies > Group')
-    parent.action(StudiesRename, text='Studies > Rename')
-    parent.action(NewSeries, text='Studies > New series')
-    parent.separator()
-    parent.action(Delete, text='Patients > Delete', generation=1)
-    parent.action(Copy, text='Patients > Copy', generation=1)
-    parent.action(MergePatients, text='Patients > Merge')
-    parent.action(PatientsRename, text='Patients > Rename')
-    parent.action(NewStudy, text='Patients > New study')
-    parent.separator()
-    parent.action(NewPatient, text='Database > New patient')
-    
-
-class Copy(wezel.Action):
-
-    def enable(self, app):
-        return app.nr_selected(self.generation) != 0
-
-    def run(self, app):
-
-        app.status.message("Copying..")
-        records = app.get_selected(self.generation)   
-        # This can be faster - copy all in one go     
-        for j, record in enumerate(records):
-            #app.status.progress(j, len(records), 'Copying..')
-            record.copy()               
-        app.refresh()
-
-
-class Delete(wezel.Action):
-
-    def enable(self, app):
-        return app.nr_selected(self.generation) != 0
-
-    def run(self, app):
-        app.status.message("Deleting..")
-        records = app.get_selected(self.generation)        
-        for j, record in enumerate(records):
-            app.status.progress(j, len(records), 'Deleting..')
-            record.remove()
-        app.refresh()
-
-
-class DeleteSeries(wezel.Action):
-
-    def enable(self, app):
-        return app.nr_selected('Series') != 0
-
-    def run(self, app):
-        series = app.selected('Series')        
-        for j, sery in enumerate(series):
-            app.status.progress(j, len(series), 'Deleting..')
-            sery.remove()
-        app.refresh()
-
-class DeleteStudies(wezel.Action):
-
-    def enable(self, app):
-        return app.nr_selected('Studies') != 0
-
-    def run(self, app):
-        studies = app.selected('Studies')        
-        for j, study in enumerate(studies):
-            app.status.progress(j, len(studies), 'Deleting..')
-            study.remove()
-        app.refresh()
-
-class CopySeries(wezel.Action):
-
-    def enable(self, app):
-        return app.nr_selected('Series') != 0
-
-    def run(self, app):
-        studies = app.folder.studies()
-        labels = [s.label() for s in studies]
+#
+# is_clickable functions
+#
+
+
+def is_database_open(app): 
+    if app.database() is None:
+        return False
+    return app.database().manager.is_open()
+
+def is_series_selected(app):
+    return app.nr_selected('Series') != 0  
+
+def is_study_selected(app):
+    return app.nr_selected('Studies') != 0 
+
+def is_patient_selected(app):
+    return app.nr_selected('Patients') != 0
+
+
+#
+# on_clicked functions
+#
+ 
+ 
+def delete(app, generation):
+    records = app.selected(generation)        
+    for j, record in enumerate(records):
+        app.status.progress(j, len(records), 'Deleting..')
+        record.remove()
+    app.refresh()
+
+
+def copy(app, generation):
+
+    app.status.message("Copying..")
+    records = app.selected(generation)   
+    # This can be faster - copy all in one go     
+    for j, record in enumerate(records):
+        #app.status.progress(j, len(records), 'Copying..')
+        record.copy()               
+    app.refresh()
+
+
+def copy_series(app):
+    studies = app.database().studies()
+    labels = [s.label() for s in studies]
+    cancel, f = app.dialog.input(
+        {'type':'dropdownlist', 'label':'Copy to study: ', 'list': labels, 'value': 0},
+        title = 'Copy to which study?')
+    if cancel:
+        return
+    study = studies[f[0]['value']]
+    series = app.selected('Series')        
+    for j, sery in enumerate(series):
+        app.status.progress(j, len(series), 'Moving..')
+        sery.copy_to(study)               
+    app.refresh()
+
+
+def copy_studies(app):
+    patients = app.database().patients()
+    labels = [p.label() for p in patients]
+    cancel, f = app.dialog.input(
+        {'type':'dropdownlist', 'label':'Copy to patient: ', 'list': labels, 'value': 0},
+        title = 'Copy to which patient?')
+    if cancel:
+        return
+    patient = patients[f[0]['value']]
+    studies = app.selected('Studies')
+    for j, study in enumerate(studies):
+        app.status.progress(j, len(studies), 'Copying..')
+        study.copy_to(patient)
+    app.refresh()
+
+
+def move_series(app):
+    studies = app.database().studies()
+    labels = [s.label() for s in studies]
+    cancel, f = app.dialog.input(
+        {'type':'dropdownlist', 'label':'Move to study: ', 'list': labels, 'value': 0},
+        title = 'Move to which study?')
+    if cancel:
+        return
+    study = studies[f[0]['value']]
+    series = app.selected('Series')        
+    for j, sery in enumerate(series):
+        app.status.progress(j, len(series), 'Moving..')
+        sery.move_to(study)               
+    app.refresh()
+
+
+def move_studies(app):
+    patients = app.database().patients()
+    labels = [p.label() for p in patients]
+    cancel, f = app.dialog.input(
+        {'type':'dropdownlist', 'label':'Move to patient: ', 'list': labels, 'value': 0},
+        title = 'Move to which patient?')
+    if cancel:
+        return
+    patient = patients[f[0]['value']]
+    studies = app.selected('Studies')        
+    for j, study in enumerate(studies):
+        app.status.progress(j, len(studies), 'Moving..')
+        study.move_to(patient)               
+    app.refresh()
+
+
+def new_series(app): 
+    app.status.message('Creating new series..')
+    studies = app.selected('Studies')
+    for study in studies:
+        study.new_series(SeriesDescription='New series')
+    app.refresh()
+
+
+def new_study(app): 
+    app.status.message('Creating new study..')
+    patients = app.selected('Patients')
+    for patient in patients:
+        patient.new_study(StudyDescription='New study')
+    app.refresh()
+
+
+def new_patient(app): 
+    app.status.message('Creating new patient..')
+    app.database().new_patient(PatientName='New patient')
+    app.refresh()
+
+
+def split_series(app): 
+    series = app.database().series()
+    sel = app.selected('Series')  
+    sel = series[0] if sel==[] else sel[0]      
+    cancel, f = app.dialog.input(
+        {"label":"Split series..", "type":"select record", "options": series, 'default': sel},
+        {"label":"Split by which DICOM keyword?", "type":"string", "value": "ImageType"},
+        title = "Input for series splitting")
+    if cancel:
+        return
+    try:
+        split = f[0].split_by(f[1]['value'])
+    except Exception as e:
+        app.dialog.information(e)
+    else:
+        for s in split:
+            app.display(s)
+        app.refresh()
+
+
+def merge_series(app): 
+    app.status.message('Merging..')
+    records = app.selected('Series')
+    study = records[0].parent()
+    series = study.new_series(SeriesDescription='Merged series')
+    db.merge(records, series)
+    app.refresh()
+
+
+def merge_studies(app): 
+    app.status.message('Merging..')
+    studies = app.selected('Studies')
+    patient = studies[0].new_pibling(PatientName='Merger')
+    db.merge(studies, patient.new_study(StudyDescription='Merged studies'))
+    app.refresh()
+
+
+def merge_patients(app): 
+    app.status.message('Merging..')
+    records = app.selected('Patients')
+    patient = records[0].new_sibling(PatientName='Merged Patients')
+    db.merge(records, patient)
+    app.refresh()
+
+
+def group_series(app): 
+    app.status.message('Grouping..')
+    records = app.selected('Series')
+    study = records[0].new_pibling(StudyDescription='Grouped')
+    db.group(records, study)
+    app.status.hide()
+    app.refresh()
+
+
+def group_studies(app): 
+    app.status.message('Grouping..')
+    records = app.selected('Studies')
+    patient = records[0].new_pibling(PatientName='Grouped')
+    db.group(records, patient)
+    app.status.hide()
+    app.refresh()
+
+
+def rename_series(app): 
+    series_list = app.selected('Series')
+    for s in series_list:
         cancel, f = app.dialog.input(
-            {'type':'dropdownlist', 'label':'Copy to study: ', 'list': labels, 'value': 0},
-            title = 'Copy to which study?')
+            {"type":"string", "label":"New series name:", "value": s.SeriesDescription},
+            title = 'Enter new series name')
         if cancel:
             return
-        study = studies[f[0]['value']]
-        series = app.selected('Series')        
-        for j, sery in enumerate(series):
-            app.status.progress(j, len(series), 'Moving..')
-            sery.copy_to(study)               
-        app.refresh()
-
-
-class MoveSeries(wezel.Action):
+        s.SeriesDescription = f[0]['value']
+    app.refresh()
 
-    def enable(self, app):
-        return app.nr_selected('Series') != 0
 
-    def run(self, app):
-        studies = app.folder.studies()
-        labels = [s.label() for s in studies]
+def rename_studies(app): 
+    for s in app.selected('Studies'):
         cancel, f = app.dialog.input(
-            {'type':'dropdownlist', 'label':'Move to study: ', 'list': labels, 'value': 0},
-            title = 'Move to which study?')
+            {"type":"string", "label":"New study name:", "value": s.StudyDescription},
+            title = 'Enter new study name')
         if cancel:
             return
-        study = studies[f[0]['value']]
-        series = app.selected('Series')        
-        for j, sery in enumerate(series):
-            app.status.progress(j, len(series), 'Moving..')
-            sery.move_to(study)               
-        app.refresh()
-
-
-class MoveStudies(wezel.Action):
+        s.StudyDescription = f[0]['value']
+    app.refresh()
 
-    def enable(self, app):
-        return app.nr_selected('Studies') != 0
 
-    def run(self, app):
-        patients = app.folder.patients()
-        labels = [p.label() for p in patients]
+def rename_patients(app): 
+    for patient in app.selected('Patients'):
         cancel, f = app.dialog.input(
-            {'type':'dropdownlist', 'label':'Move to patient: ', 'list': labels, 'value': 0},
-            title = 'Move to which patient?')
+            {"type":"string", "label":"New patient name:", "value": patient.PatientName},
+            title = 'Enter new patient name')
         if cancel:
             return
-        patient = patients[f[0]['value']]
-        studies = app.selected('Studies')        
-        for j, study in enumerate(studies):
-            app.status.progress(j, len(studies), 'Moving..')
-            study.move_to(patient)               
-        app.refresh()
-
+        patient.PatientName = f[0]['value']
+    app.refresh()
 
-class CopyStudies(wezel.Action):
 
-    def enable(self, app):
-        return app.nr_selected('Studies') != 0
+def series_extract_by_index(app):
 
-    def run(self, app):
-        patients = app.folder.patients()
-        labels = [p.label() for p in patients]
+    # Get source data
+    series = app.selected('Series')[0]
+    _, slices = series.get_pixel_array(['SliceLocation', 'AcquisitionTime'])
+    series.status.hide()
+    nz, nt = slices.shape[0], slices.shape[1]
+    x0, x1, t0, t1 = 0, nz, 0, nt
+
+    # Get user input
+    invalid = True
+    while invalid:
         cancel, f = app.dialog.input(
-            {'type':'dropdownlist', 'label':'Copy to patient: ', 'list': labels, 'value': 0},
-            title = 'Copy to which patient?')
-        if cancel:
-            return
-        patient = patients[f[0]['value']]
-        studies = app.selected('Studies')
-        for j, study in enumerate(studies):
-            app.status.progress(j, len(studies), 'Copying..')
-            study.copy_to(patient)
-        app.refresh()
-
-
-class NewSeries(wezel.Action):
-
-    def enable(self, app):
-        return app.nr_selected('Studies') != 0
-
-    def run(self, app): 
-        app.status.message('Creating new series..')
-        studies = app.selected('Studies')
-        for study in studies:
-            study.new_series(SeriesDescription='New series')
-        app.refresh()
-
-
-class NewStudy(wezel.Action):
-
-    def enable(self, app):
-        return app.nr_selected('Patients') != 0
-
-    def run(self, app): 
-        app.status.message('Creating new study..')
-        patients = app.selected('Patients')
-        for patient in patients:
-            patient.new_study(StudyDescription='New study')
-        app.refresh()
-
-
-class NewPatient(wezel.Action):
-
-    def enable(self, app):
-        return True
-
-    def run(self, app): 
-        app.status.message('Creating new patient..')
-        app.folder.new_patient(PatientName='New patient')
-        app.refresh()
-
-
-class MergeSeries(wezel.Action):
-
-    def enable(self, app):
-        return app.nr_selected('Series') != 0
-
-    def run(self, app): 
-
-        app.status.message('Merging..')
-        records = app.selected('Series')
-        #study = records[0].new_pibling(StudyDescription='Merger')
-        study = records[0].parent()
-        series = study.new_series(SeriesDescription='Merged series')
-        db.merge(records, series)
-        app.refresh()
-
-
-class MergeStudies(wezel.Action):
-
-    def enable(self, app):
-        return app.nr_selected('Studies') != 0
-
-    def run(self, app): 
-        app.status.message('Merging..')
-        studies = app.selected('Studies')
-        patient = studies[0].new_pibling(PatientName='Merger')
-        db.merge(studies, patient.new_study(StudyDescription='Merged studies'))
-        app.refresh()
-
-class MergePatients(wezel.Action):
-
-    def enable(self, app):
-        return app.nr_selected('Patients') != 0
-
-    def run(self, app): 
-        app.status.message('Merging..')
-        records = app.selected('Patients')
-        patient = records[0].new_sibling(PatientName='Merged Patients')
-        db.merge(records, patient)
-        app.refresh()
-
-
-class GroupSeries(wezel.Action):
-
-    def enable(self, app):
-        return app.nr_selected('Series') != 0
-
-    def run(self, app): 
-        app.status.message('Grouping..')
-        records = app.selected('Series')
-        study = records[0].new_pibling(StudyDescription='Grouped')
-        db.group(records, study)
-        app.status.hide()
-        app.refresh()
-
-class GroupStudies(wezel.Action):
-
-    def enable(self, app):
-        return app.nr_selected('Studies') != 0
-
-    def run(self, app): 
-        app.status.message('Grouping..')
-        records = app.selected('Studies')
-        patient = records[0].new_pibling(PatientName='Grouped')
-        db.group(records, patient)
-        app.status.hide()
-        app.refresh()
-
-
-class SeriesRename(wezel.Action):
-
-    def enable(self, app):
-        return app.nr_selected('Series') != 0
-
-    def run(self, app): 
-        series_list = app.get_selected(3)
-        for s in series_list:
-            cancel, f = app.dialog.input(
-                {"type":"string", "label":"New series name:", "value": s.SeriesDescription},
-                title = 'Enter new series name')
-            if cancel:
-                return
-            s.SeriesDescription = f[0]['value']
-        app.refresh()
-
-
-class StudiesRename(wezel.Action):
-
-    def enable(self, app):
-        return app.nr_selected('Studies') != 0
-
-    def run(self, app): 
-        for s in app.selected('Studies'):
-            cancel, f = app.dialog.input(
-                {"type":"string", "label":"New study name:", "value": s.StudyDescription},
-                title = 'Enter new study name')
-            if cancel:
-                return
-            s.StudyDescription = f[0]['value']
-        app.refresh()
-
-
-class PatientsRename(wezel.Action):
-
-    def enable(self, app):
-        return app.nr_selected('Patients') != 0
-
-    def run(self, app): 
-        for patient in app.selected('Patients'):
-            cancel, f = app.dialog.input(
-                {"type":"string", "label":"New patient name:", "value": patient.PatientName},
-                title = 'Enter new patient name')
-            if cancel:
-                return
-            patient.PatientName = f[0]['value']
-        app.refresh()
-
-
-class SeriesExtractByIndex(wezel.Action):
-
-    def enable(self, app):
-        return app.nr_selected(3) != 0
-
-    def run(self, app):
-
-        # Get source data
-        series = app.get_selected(3)[0]
-        _, slices = series.get_pixel_array(['SliceLocation', 'AcquisitionTime'])
-        series.status.hide()
-        nz, nt = slices.shape[0], slices.shape[1]
-        x0, x1, t0, t1 = 0, nz, 0, nt
-
-        # Get user input
-        invalid = True
-        while invalid:
-            cancel, f = app.dialog.input(
-                {"type":"integer", "label":"Slice location from index..", "value":x0, "minimum": 0, "maximum": nz},
-                {"type":"integer", "label":"Slice location to index..", "value":x1, "minimum": 0, "maximum": nz},
-                {"type":"integer", "label":"Acquisition time from index..", "value":t0, "minimum": 0, "maximum": nt},
-                {"type":"integer", "label":"Acquisition time to index..", "value":t1, "minimum": 0, "maximum": nt},
-                title='Select parameter ranges')
-            if cancel: 
-                return
-            x0, x1, t0, t1 = f[0]['value'], f[1]['value'], f[2]['value'], f[3]['value']
-            invalid = (x0 >= x1) or (t0 >= t1)
-            if invalid:
-                app.dialog.information("Invalid selection - first index must be lower than second")
-
-        # Extract series and save
-        #study = series.parent().new_sibling(StudyDescription='Extracted Series')
-        indices = ' [' + str(x0) + ':' + str(x1) 
-        indices += ', ' + str(t0) + ':' + str(t1) + ']'
-        #new_series = study.new_child(SeriesDescription = series.SeriesDescription + indices)
-        new_series = series.new_sibling(SeriesDescription = slices[0,0,0].SeriesDescription + indices)
-        #db.copy_to(slices[x0:x1,t0:t1,:], new_series)
-        new_series.adopt(np.ravel(slices[x0:x1,t0:t1,:]).tolist())
-        app.refresh()
-
-
-class SeriesExtractByValue(wezel.Action):
-
-    def enable(self, app):
-        return app.nr_selected(3) != 0
-
-    def run(self, app):
-
-        # Get source data
-        series = app.get_selected(3)[0]
-        slice_locations = series.SliceLocation
-        if not isinstance(slice_locations, list):
-            slice_locations = [slice_locations]
-        acquisition_times = series.AcquisitionTime
-        if not isinstance(acquisition_times, list):
-            acquisition_times = [acquisition_times]
-        series.status.hide()
-
-        # Get user input
-        cancel, f = app.dialog.input(
-            {"type":"listview", "label":"Slice locations..", 'list': slice_locations},
-            {"type":"listview", "label":"Acquisition times..", 'list': acquisition_times},
+            {"type":"integer", "label":"Slice location from index..", "value":x0, "minimum": 0, "maximum": nz},
+            {"type":"integer", "label":"Slice location to index..", "value":x1, "minimum": 0, "maximum": nz},
+            {"type":"integer", "label":"Acquisition time from index..", "value":t0, "minimum": 0, "maximum": nt},
+            {"type":"integer", "label":"Acquisition time to index..", "value":t1, "minimum": 0, "maximum": nt},
             title='Select parameter ranges')
         if cancel: 
             return
-        if f[0]['value'] != []:
-            slice_locations = [slice_locations[i] for i in f[0]['value']]
-        if f[1]['value'] != []:
-            acquisition_times = [acquisition_times[i] for i in f[1]['value']]
-
-        # Find matching instances
-        all = series.instances()
-        instances = []
-        for i, instance in enumerate(all):
-            series.status.progress(i, len(all), 'Finding instances..')
-            v = instance[['SliceLocation', 'AcquisitionTime']]
-            if (v[0] in slice_locations) and (v[1] in acquisition_times):
-                instances.append(instance)
-        series.status.hide()
-        if instances == []:
-            return
+        x0, x1, t0, t1 = f[0]['value'], f[1]['value'], f[2]['value'], f[3]['value']
+        invalid = (x0 >= x1) or (t0 >= t1)
+        if invalid:
+            app.dialog.information("Invalid selection - first index must be lower than second")
+
+    # Extract series and save
+    #study = series.parent().new_sibling(StudyDescription='Extracted Series')
+    indices = ' [' + str(x0) + ':' + str(x1) 
+    indices += ', ' + str(t0) + ':' + str(t1) + ']'
+    #new_series = study.new_child(SeriesDescription = series.SeriesDescription + indices)
+    new_series = series.new_sibling(SeriesDescription = slices[0,0,0].SeriesDescription + indices)
+    #db.copy_to(slices[x0:x1,t0:t1,:], new_series)
+    #new_series.adopt(np.ravel(slices[x0:x1,t0:t1,:]).tolist())
+    new_series.adopt(slices[x0:x1,t0:t1,:].flatten().tolist())
+    app.display(new_series)
+    app.refresh()
+
+
+def series_extract_by_value(app):
+
+    # Get source data
+    series = app.selected('Series')[0]
+    slice_locations = series.SliceLocation
+    if not isinstance(slice_locations, list):
+        slice_locations = [slice_locations]
+    acquisition_times = series.AcquisitionTime
+    if not isinstance(acquisition_times, list):
+        acquisition_times = [acquisition_times]
+    series.status.hide()
+
+    # Get user input
+    cancel, f = app.dialog.input(
+        {"type":"listview", "label":"Slice locations..", 'list': slice_locations},
+        {"type":"listview", "label":"Acquisition times..", 'list': acquisition_times},
+        title='Select parameter ranges')
+    if cancel: 
+        return
+    if f[0]['value'] != []:
+        slice_locations = [slice_locations[i] for i in f[0]['value']]
+    if f[1]['value'] != []:
+        acquisition_times = [acquisition_times[i] for i in f[1]['value']]
+
+    # Find matching instances
+    all = series.instances()
+    instances = []
+    for i, instance in enumerate(all):
+        series.status.progress(i, len(all), 'Finding instances..')
+        v = instance[['SliceLocation', 'AcquisitionTime']]
+        if (v[0] in slice_locations) and (v[1] in acquisition_times):
+            instances.append(instance)
+    series.status.hide()
+    if instances == []:
+        return
+
+    # Copy matching instances into new series
+    series.status.message('Çopying to series..')
+    desc = instances[0].SeriesDescription + ' [subseries]'
+    new_series = series.new_sibling(SeriesDescription = desc)
+    new_series.adopt(instances)
+    series.status.hide()
+    app.display(new_series)
+    app.refresh()
+
+
+
+
+action_series_delete = Action('Series > Delete', on_clicked=lambda app: delete(app, 'Series'), is_clickable=is_series_selected)
+action_series_copy = Action('Series > Copy', on_clicked=lambda app: copy(app, 'Series'), is_clickable=is_series_selected)
+action_series_copy_to = Action('Series > Copy to..', on_clicked=copy_series, is_clickable=is_series_selected)
+action_series_move_to = Action('Series > Move to..', on_clicked=move_series, is_clickable=is_series_selected)
+action_series_merge = Action('Series > Merge', on_clicked=merge_series, is_clickable=is_series_selected)
+action_series_group = Action('Series > Group', on_clicked=group_series, is_clickable=is_series_selected)
+action_series_split = Action('Series > Split by..', on_clicked=split_series, is_clickable=is_series_selected)
+action_series_rename = Action('Series > Rename', on_clicked=rename_series, is_clickable=is_series_selected)
+action_series_extract_by_index = Action('Series > Extract subseries (by index)', on_clicked=series_extract_by_index, is_clickable=is_series_selected)
+action_series_extract_by_value = Action('Series > Extract subseries (by value)', on_clicked=series_extract_by_value, is_clickable=is_series_selected)
+action_studies_delete = Action('Studies > Delete', on_clicked=lambda app: delete(app, 'Studies'), is_clickable=is_study_selected)
+action_studies_copy = Action('Studies > Copy', on_clicked=lambda app: copy(app, 'Studies'), is_clickable=is_study_selected)
+action_studies_copy_to = Action('Studies > Copy to..', on_clicked=copy_studies, is_clickable=is_study_selected)
+action_studies_move_to = Action('Studies > Move to..', on_clicked=move_studies, is_clickable=is_study_selected)
+action_studies_merge = Action('Studies > Merge', on_clicked=merge_studies, is_clickable=is_study_selected)
+action_studies_group = Action('Studies > Group', on_clicked=group_studies, is_clickable=is_study_selected)
+action_studies_rename = Action('Studies > Rename', on_clicked=rename_studies, is_clickable=is_study_selected)
+action_studies_new_series = Action('Studies > New series', on_clicked=new_series, is_clickable=is_study_selected)
+action_patients_delete = Action('Patients > Delete', on_clicked=lambda app: delete(app, 'Patients'), is_clickable=is_patient_selected)
+action_patients_copy = Action('Patients > Copy', on_clicked=lambda app: copy(app, 'Patients'), is_clickable=is_patient_selected)
+action_patients_merge = Action('Patients > Merge', on_clicked=merge_patients, is_clickable=is_patient_selected)
+action_patients_rename = Action('Patients > Rename', on_clicked=rename_patients, is_clickable=is_patient_selected)
+action_patients_new_study = Action('Patients > New study', on_clicked=new_study, is_clickable=is_patient_selected)
+action_database_new_patient = Action('Database > New patient', on_clicked=new_patient, is_clickable=is_database_open)
+
+
+
+menu = Menu('Edit')
+menu_series = menu.add_menu('Series')
+menu_series.add(action_series_delete)
+menu_series.add(action_series_copy)
+menu_series.add(action_series_copy_to)
+menu_series.add(action_series_move_to)
+menu_series.add(action_series_merge)
+menu_series.add(action_series_group)
+menu_series.add(action_series_split)
+menu_series.add(action_series_rename)
+menu_series.add(action_series_extract_by_index)
+menu_series.add(action_series_extract_by_value)
+menu_study = menu.add_menu('Studies')
+menu_study.add(action_studies_delete)
+menu_study.add(action_studies_copy)
+menu_study.add(action_studies_copy_to)
+menu_study.add(action_studies_move_to)
+menu_study.add(action_studies_merge)
+menu_study.add(action_studies_group)
+menu_study.add(action_studies_rename)
+menu_study.add(action_studies_new_series)
+menu_patient = menu.add_menu('Patient')
+menu_patient.add(action_patients_delete)
+menu_patient.add(action_patients_copy)
+menu_patient.add(action_patients_merge)
+menu_patient.add(action_patients_rename)
+menu_patient.add(action_patients_new_study)
+menu_database = menu.add_menu('Database')
+menu_database.add(action_database_new_patient)
+
 
-        # Copy matching instances into new series
-        series.status.message('Çopying to series..')
-        desc = instances[0].SeriesDescription + ' [subseries]'
-        new_series = series.new_sibling(SeriesDescription = desc)
-        new_series.adopt(instances)
-        series.status.hide()
-        app.refresh()
```

### Comparing `wezel-0.1.1/src/wezel/canvas/__init__.py` & `wezel-0.1.2/src/wezel/canvas/__init__.py`

 * *Files 7% similar despite different names*

```diff
@@ -35,12 +35,16 @@
     MaskPenRectangle,
     MaskPenCircle, 
     MaskThreshold,
     MaskPaintByNumbers,
     MaskRegionGrowing,
     MaskDilate,
     MaskShrink,
+    MaskOpen,
+    MaskClose,
+    MaskWand,
+    MaskMove,
     MaskKidneyEdgeDetection,
 )
 from wezel.canvas.series_canvas import (
     SeriesCanvas,
 )
```

### Comparing `wezel-0.1.1/src/wezel/canvas/canvas.py` & `wezel-0.1.2/src/wezel/canvas/canvas.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,28 +1,28 @@
 import random
 import numpy as np
 import copy
 
 
-from PyQt5.QtCore import Qt, pyqtSignal, QRectF
-from PyQt5.QtWidgets import (QGraphicsObject, QGraphicsItem,
+from PySide2.QtCore import Qt, Signal, QRectF
+from PySide2.QtWidgets import (QGraphicsObject, QGraphicsItem,
     QAction, QMenu, QGraphicsView, QGraphicsScene, QActionGroup)
-from PyQt5.QtGui import QPixmap, QBrush, QIcon, QTransform, QCursor, QImage
+from PySide2.QtGui import QPixmap, QBrush, QIcon, QTransform, QCursor, QImage
 
 from wezel import canvas, icons
 from wezel.canvas.utils import colormap_to_LUT
 
 class Canvas(QGraphicsView):
     """Wrapper for ImageItem displaying it in a scrollable Widget"""
 
-    #imageUpdated = pyqtSignal(object)
-    newMaskSeries = pyqtSignal(object)
-    mousePositionMoved = pyqtSignal(int, int)
-    arrowKeyPress = pyqtSignal(str)
-    #maskChanged = pyqtSignal()
+    #imageUpdated = Signal(object)
+    newMaskSeries = Signal(object)
+    mousePositionMoved = Signal(int, int)
+    arrowKeyPress = Signal(str)
+    #maskChanged = Signal()
 
     def __init__(self, parent=None): 
         super().__init__(parent)
         self.setScene(QGraphicsScene(self))
         self.setBackgroundBrush(QBrush(Qt.black))
         self.setTransformationAnchor(QGraphicsView.AnchorUnderMouse)
         self.setResizeAnchor(QGraphicsView.AnchorUnderMouse)
@@ -48,30 +48,31 @@
     @property
     def maskItem(self):
         return self.item(1)
         
     @property
     def filterItem(self):
         return self.item(2)
-
-    # def mask(self):
-    #     return self.maskItem.bin
+    
+    def setBlank(self):
+        self.removeItem(self.imageItem)
+        self.removeItem(self.maskItem)
 
     def setImage(self, array, center, width, cmap, lut=None):
         if lut is None:
             lut = colormap_to_LUT(cmap)
         self.removeItem(self.imageItem)
         item = ImageItem(array, center, width, lut)
         item._cmap = cmap
         self.scene().addItem(item)
         item.setZValue(0)
         filter = self.filterItem
         if filter is not None:
             filter.prepareGeometryChange()
-            filter.boundingRectangle = self.scene().sceneRect()
+            filter.boundingRectangle = item.boundingRectangle
             filter.initialize()
         self.setMask(None)
         return item
 
     def setMask(self, mask, color=0, opacity=0.5):
         self.removeItem(self.maskItem)
         if self.toolBar is not None:
@@ -92,57 +93,74 @@
             return
         if filter == 'Default':
             filter = canvas.PanFilter()
         self.scene().addItem(filter)
         self.scene().setFocusItem(filter)
         filter.setZValue(2)
         filter.prepareGeometryChange()
-        filter.boundingRectangle = self.scene().sceneRect()
+        if self.imageItem is None:
+            filter.boundingRectangle = self.scene().sceneRect()
+        else:
+            filter.boundingRectangle = self.imageItem.boundingRectangle
         filter.initialize()
 
     def fitItem(self):
         item = self.imageItem
         if item is None:
             item = self.maskItem
         if item is not None:
             self.fitInView(item, Qt.KeepAspectRatio)
 
     def setColormap(self, cmap=None):
+        if self.imageItem is None:
+            return
         if cmap is None:
             cmap = 'Greyscale'
         RGB = colormap_to_LUT(cmap)
         self.imageItem._cmap = cmap
         self.imageItem.setLUT(RGB)
         self.imageItem.setDisplay()
 
     def setWindow(self, center=None, width=None):
+        if self.imageItem is None:
+            return
         if (center is None) or (width is None):
             array = self.imageItem._array
             min = np.min(array)
             max = np.max(array)
         if center is None:
             center = (max+min)/2
         if width is None:
             width = 0.9*(max-min)       
         self.imageItem.setWindow(center, width)
         self.imageItem.setDisplay()
 
     def array(self):
+        if self.imageItem is None:
+            return
         return self.imageItem._array
 
     def lut(self):
+        if self.imageItem is None:
+            return
         return self.imageItem._lut
 
     def colormap(self):
+        if self.imageItem is None:
+            return
         return self.imageItem._cmap
 
     def center(self):
+        if self.imageItem is None:
+            return
         return self.imageItem._center
         
     def width(self):
+        if self.imageItem is None:
+            return
         return self.imageItem._width
 
 
 class AnyItem(QGraphicsObject):
     """Displays an image.
     """
 
@@ -246,15 +264,15 @@
     def array(self):
         return self._array    
 
 
 class MaskItem(AnyItem):
     """Displays a mask as an overlay on an image.
     """
-    maskChanged = pyqtSignal()
+    maskChanged = Signal()
 
     def __init__(self, imageItem, mask, opacity=0.75, color=0): 
         super().__init__(imageItem)
         self._bin = []
         self._current = None
         self._BGRA = None
         self._qImage = None
@@ -487,30 +505,30 @@
 
     def contextMenuEvent(self, event):
         menu = self.contextMenu()
         menu.exec_(event.screenPos())
 
     def pick(self):
         self.actionPick.setChecked(True)
-        self.actionPick.triggered.emit(True)
+        self.actionPick.triggered.emit()
         self.update()
 
 
 class FilterSet():
     def __init__(self):
         self.filters = None
         self.icon = None
         self.text = None
         self.current = None
 
     def pick(self, filter):
         self.current = filter
         self.actionPick.filter = filter
         self.actionPick.setChecked(True)
-        self.actionPick.triggered.emit(True)
+        self.actionPick.triggered.emit()
         #self.update()
 
     def setActionPick(self):
         self.actionPick = QAction(self.icon, self.text)
         self.actionPick.setCheckable(True)
         #self.actionPick.setEnabled(False)
         self.actionPick.filter = self.current
```

### Comparing `wezel-0.1.1/src/wezel/canvas/image_filter.py` & `wezel-0.1.2/src/wezel/canvas/image_filter.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,18 +1,18 @@
 import numpy as np
 
-from PyQt5.QtCore import Qt, pyqtSignal
-from PyQt5.QtWidgets import QAction, QMenu, QActionGroup
-from PyQt5.QtGui import QPixmap, QCursor, QIcon
+from PySide2.QtCore import Qt, Signal
+from PySide2.QtWidgets import QAction, QMenu, QActionGroup
+from PySide2.QtGui import QPixmap, QCursor, QIcon
 
 from wezel import canvas, icons
 
 
 class ImageWindow(canvas.FilterItem):
-    windowChanged = pyqtSignal(object, float, float, bool)
+    windowChanged = Signal(object, float, float, bool)
 
     """Change contrast
     """
     def __init__(self): 
         super().__init__()
         pixMap = QPixmap(icons.color)
         self.cursor = QCursor(pixMap, hotX=4, hotY=0)
@@ -24,33 +24,42 @@
         self.setActionPick()
 
     def window(self, dx, dy):
         """Change intensity and contrast"""
 
         cnvs = self.scene().parent()
         item = cnvs.imageItem
+        if item is None:
+            return
         if self._min is None:
             self._min = np.amin(item._array)
             self._max = np.amax(item._array)
+            #self._min = np.percentile(item._array, 25)
+            #self._max = np.percentile(item._array, 75)
        
         # Move 1024 to change the center over the full range
         # Speed is faster further away from the center of the range
         center = item._center 
+        array_center = (self._min + self._max)/2.0
         v0 = (self._max-self._min)/1024
         a0 = 1.0/256
-        vy = v0 + a0*abs((center - (self._min+(self._max-self._min)/2.0)))
+        #a0 = v0/256
+        #a0=0
+        vy = v0 + a0*abs((center - array_center))
         center = center + vy * dy
 
         # Changing the width is faster at larger widths
         width = item._width
         v0 = (self._max-self._min)/512
         a0 = 1.0/64
+        #a0 = v0/64
+        #a0=0
         vx = v0 + a0*width
         width = width - vx * dx
-        width = width if width>1 else 1
+        #width = width if width>1 else 1
 
         cnvs.setWindow(center, width)
         self.windowChanged.emit(item._array, center, width, True)
 
     def mouseMoveEvent(self, event):
         self.x = int(event.pos().x())
         self.y = int(event.pos().y())
```

### Comparing `wezel-0.1.1/src/wezel/canvas/mask_filter.py` & `wezel-0.1.2/src/wezel/canvas/mask_filter.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,20 +1,76 @@
 import math
 import numpy as np
-from matplotlib.path import Path as MplPath
 import cv2 as cv2
 import skimage
+from scipy import ndimage as ndi
 
-from PyQt5.QtCore import Qt, QRectF, QPointF
-from PyQt5.QtWidgets import QAction, QMenu, QActionGroup
-from PyQt5.QtGui import QPixmap, QCursor, QIcon, QColor, QPen
+from PySide2.QtCore import Qt, QRectF, QPointF
+from PySide2.QtWidgets import QAction, QMenu, QActionGroup
+from PySide2.QtGui import QPixmap, QCursor, QIcon, QColor, QPen
 
 from wezel import canvas, icons
 
 
+class MaskMove(canvas.FilterItem):
+    """Painting or erasing tool.
+    """
+    def __init__(self):
+        super().__init__()
+        pixMap = QPixmap(icons.arrow_move)
+        self.cursor = QCursor(pixMap, hotX=8, hotY=8)
+        self.icon = QIcon(pixMap)
+        self.toolTip = 'Move mask'
+        self.text = 'Move mask'
+        self.setActionPick()
+
+    def hoverMoveEvent(self, event):
+        self.x = int(event.pos().x())
+        self.y = int(event.pos().y())
+        self.update() 
+        cnvs = self.scene().parent()
+        cnvs.mousePositionMoved.emit(self.x, self.y)   
+
+    def mousePressEvent(self, event):
+        self.x = int(event.pos().x())
+        self.y = int(event.pos().y())
+        button = event.button()
+        if button == Qt.LeftButton:
+            item = self.scene().parent().maskItem
+            if item is None:
+                return
+            item.extend()
+            self.x0 = self.x
+            self.y0 = self.y
+            self.bin0 = item.bin()
+
+    def mouseReleaseEvent(self, event):
+        self.x = int(event.pos().x())
+        self.y = int(event.pos().y())
+        self.update()
+
+    def mouseMoveEvent(self, event):
+        self.x = int(event.pos().x())
+        self.y = int(event.pos().y())
+        buttons = event.buttons()
+        if buttons == Qt.LeftButton:
+            self.moveMask() 
+        cnvs = self.scene().parent() 
+        cnvs.mousePositionMoved.emit(self.x, self.y)
+ 
+    def moveMask(self):
+        cnvs = self.scene().parent() 
+        item = cnvs.maskItem
+        if item is None:
+            return
+        bin = ndi.shift(self.bin0, [self.x-self.x0, self.y-self.y0], order=0, mode='grid-wrap')
+        item.setBin(bin)
+        item.setDisplay()
+
+
 class MaskBrush(canvas.FilterItem):
     """Painting or erasing tool.
     """
     def __init__(self, brushSize=3, mode="paint"):
         super().__init__()
         self.brushSize = brushSize
         self.setMode(mode)
@@ -58,14 +114,16 @@
 
     def mousePressEvent(self, event):
         self.x = int(event.pos().x())
         self.y = int(event.pos().y())
         button = event.button()
         if button == Qt.LeftButton:
             item = self.scene().parent().maskItem
+            if item is None:
+                return
             item.extend()
             self.paintPixels()
 
     def mouseReleaseEvent(self, event):
         self.x = int(event.pos().x())
         self.y = int(event.pos().y())
         self.update()
@@ -78,14 +136,16 @@
             self.paintPixels() 
         cnvs = self.scene().parent() 
         cnvs.mousePositionMoved.emit(self.x, self.y)
  
     def paintPixels(self):
         cnvs = self.scene().parent() 
         item = cnvs.maskItem
+        if item is None:
+            return
         w = int((self.brushSize - 1)/2)
         for x in range(self.x-w, self.x+w+1, 1):
             if 0 <= x < item.bin().shape[0]:
                 for y in range(self.y-w, self.y+w+1, 1):
                     if 0 <= y < item.bin().shape[1]:
                         item.setPixel(x, y, self.mode=="paint")
         item.update()
@@ -177,29 +237,14 @@
     def __init__(self, mode="draw"):
         super().__init__(mode)
         self.iconInSet = QIcon(icons.layer_shape_curve)
         self.textInSet = 'Freehand'
         self.path = None
         # self.xc = None
         # self.yc = None
-
-    # def initialize(self):
-    #     # Called by the canvas after the filter is set to a scene
-    #     # And when a new image is set to the scene
-    #     item = self.scene().parent().imageItem
-    #     set_attributes = False
-    #     if self.xc is None:
-    #         set_attributes = True
-    #     elif self.xc.shape != item._array.shape:
-    #         set_attributes = True
-    #     if set_attributes:
-    #         nx, ny = item._array.shape[0], item._array.shape[1]
-    #         x, y = np.arange(0.5, 0.5+nx), np.arange(0.5, 0.5+ny)
-    #         self.xc, self.yc = np.meshgrid(x, y, indexing='ij')
-    #         self.locations = list(zip(self.xc.flatten(), self.yc.flatten()))
         
     def paint(self, painter, option, widget):
         if self.path is None: 
             return
         pen = QPen()
         pen.setColor(QColor(Qt.white))
         pen.setWidth(0)
@@ -215,14 +260,16 @@
         painter.drawLine(p1, p2)
 
     def mousePressEvent(self, event):
         self.x = int(event.pos().x())
         self.y = int(event.pos().y())
         if event.button() == Qt.LeftButton:
             item = self.scene().parent().maskItem
+            if item is None:
+                return
             item.extend()
             position = [event.pos().x(), event.pos().y()]
             self.path = [position]
 
     def mouseReleaseEvent(self, event):
         self.x = int(event.pos().x())
         self.y = int(event.pos().y())
@@ -234,22 +281,25 @@
 
     def mouseMoveEvent(self, event):
         self.x = int(event.pos().x())
         self.y = int(event.pos().y())
         buttons = event.buttons()
         if buttons == Qt.LeftButton:
             position = [event.pos().x(), event.pos().y()]
-            if position != self.path[-1]:
-                self.path.append(position)
-                self.update()
+            if self.path is not None:
+                if position != self.path[-1]:
+                    self.path.append(position)
+                    self.update()
 
     def fillPath(self):
         if len(self.path) == 0: 
             return
         item = self.scene().parent().maskItem
+        if item is None:
+            return
         bin = np.zeros(item.bin().shape, dtype=bool)
         rr, cc = skimage.draw.polygon([p[0]-0.5 for p in self.path], [p[1]-0.5 for p in self.path], item.bin().shape)
         bin[rr, cc] = True
         if self.mode == "draw":
             item.setBin(np.logical_or(item.bin(), bin))
         elif self.mode == "cut":
             item.setBin(np.logical_and(item.bin(), np.logical_not(bin)))
@@ -272,14 +322,16 @@
         self.iconInSet = QIcon(icons.layer_shape_polygon)
         self.textInSet = 'Polygon'
 
     def hoverMoveEvent(self, event):
         if self.path is not None:
             self.path[-1] = [event.pos().x(), event.pos().y()]
             item = self.scene().parent().maskItem
+            if item is None:
+                return
             item.update()
         super().hoverMoveEvent(event) 
 
     def mousePressEvent(self, event):
         self.x = int(event.pos().x())
         self.y = int(event.pos().y())
         if event.button() == Qt.LeftButton:
@@ -295,27 +347,31 @@
 
     def mouseMoveEvent(self, event):
         self.x = int(event.pos().x())
         self.y = int(event.pos().y())
         if self.path is not None:
             self.path[-1] = [event.pos().x(), event.pos().y()]
             item = self.scene().parent().maskItem
+            if item is None:
+                return
             item.update()
     
     def mouseDoubleClickEvent(self, event):
         self.x = int(event.pos().x())
         self.y = int(event.pos().y())
         button = event.button()
         if button == Qt.LeftButton:
             if self.path is not None:
                 item = self.scene().parent().maskItem
+                if item is None:
+                    return
                 item.extend()
                 self.path[-1] = [event.pos().x(), event.pos().y()]
                 self.fillPath()
-                item = self.scene().parent().maskItem
+                #item = self.scene().parent().maskItem
                 item.update()
                 self.path = None
 
 
 class MaskPenRectangle(MaskPenFreehand):
     """Rectangle region drawing tool.
     """
@@ -329,14 +385,16 @@
         self.xc = None
         self.yc = None
 
     def initialize(self):
         # Called by the canvas after the filter is set to a scene
         # And when a new image is set to the scene
         item = self.scene().parent().imageItem
+        if item is None:
+            return
         set_attributes = False
         if self.xc is None:
             set_attributes = True
         elif self.xc.shape != item._array.shape:
             set_attributes = True
         if set_attributes:
             nx, ny = item._array.shape[0], item._array.shape[1]
@@ -356,38 +414,44 @@
         painter.drawRect(rect)
 
     def mousePressEvent(self, event):
         self.x = int(event.pos().x())
         self.y = int(event.pos().y())
         if event.button() == Qt.LeftButton:
             item = self.scene().parent().maskItem
+            if item is None:
+                return
             item.extend()
             self.corner1 = [event.pos().x(), event.pos().y()]
 
     def mouseMoveEvent(self, event):
         self.x = int(event.pos().x())
         self.y = int(event.pos().y())
         buttons = event.buttons()
         if buttons == Qt.LeftButton:
             self.corner2 = [event.pos().x(), event.pos().y()]
             item = self.scene().parent().maskItem
+            if item is None:
+                return
             item.update()
 
     def mouseReleaseEvent(self, event):
         self.x = int(event.pos().x())
         self.y = int(event.pos().y())
         button = event.button()
         if button == Qt.LeftButton:
             if self.corner2 is not None:
                 self.fillRect()
                 self.corner1 = None
                 self.corner2 = None
 
     def fillRect(self):
         item = self.scene().parent().maskItem
+        if item is None:
+            return
         x = [self.corner1[0], self.corner2[0]]
         y = [self.corner1[1], self.corner2[1]]
         rectx = np.logical_and(min(x) <= self.xc, self.xc <= max(x))
         recty = np.logical_and(min(y) <= self.yc, self.yc <= max(y))
         rect = np.logical_and(rectx, recty)
         if self.mode == "draw":
             item.setBin(np.logical_or(item.bin(), rect))
@@ -416,14 +480,16 @@
         self.xc = None
         self.yc = None
 
     def initialize(self):
         # Called by the canvas after the filter is set to a scene
         # And when a new image is set to the scene
         item = self.scene().parent().imageItem
+        if item is None:
+            return
         set_attributes = False
         if self.xc is None:
             set_attributes = True
         elif self.xc.shape != item._array.shape:
             set_attributes = True
         if set_attributes:
             nx, ny = item._array.shape[0], item._array.shape[1]
@@ -441,40 +507,46 @@
         painter.drawEllipse(center, self.radius, self.radius)
 
     def mousePressEvent(self, event):
         self.x = int(event.pos().x())
         self.y = int(event.pos().y())
         if event.button() == Qt.LeftButton:
             item = self.scene().parent().maskItem
+            if item is None:
+                return
             item.extend()
             self.center = [event.pos().x(), event.pos().y()]
             self.radius = 0
 
     def mouseMoveEvent(self, event):
         self.x = int(event.pos().x())
         self.y = int(event.pos().y())
         buttons = event.buttons()
         if buttons == Qt.LeftButton:
+            item = self.scene().parent().maskItem
+            if item is None:
+                return
             dx = event.pos().x() - self.center[0]
             dy = event.pos().y() - self.center[1]
             self.radius = math.sqrt(dx**2 + dy**2)
-            item = self.scene().parent().maskItem
             item.update()
 
     def mouseReleaseEvent(self, event):
         self.x = int(event.pos().x())
         self.y = int(event.pos().y())
         button = event.button()
         if button == Qt.LeftButton:
             if self.center is not None:
                 self.fillCircle()
                 self.center = None
 
     def fillCircle(self):
         item = self.scene().parent().maskItem
+        if item is None:
+            return
         d_sq = (self.xc-self.center[0])**2 + (self.yc-self.center[1])**2
         if self.mode == "draw":
             item.setBin(np.logical_or(item.bin(), d_sq <= self.radius**2))
         elif self.mode == "cut":
             item.setBin(np.logical_and(item.bin(), d_sq > self.radius**2))
         elif self.mode == "catch":
             item.setBin(np.logical_and(item.bin(), d_sq <= self.radius**2))
@@ -517,51 +589,60 @@
 
     def mousePressEvent(self, event):
         self.x = int(event.pos().x())
         self.y = int(event.pos().y())
         if event.button() == Qt.LeftButton:
             self.contour = self.findContour()
             item = self.scene().parent().maskItem
+            if item is None:
+                return
             item.extend()
             item.update()
 
     def mouseMoveEvent(self, event):
         self.x = int(event.pos().x())
         self.y = int(event.pos().y())
         buttons = event.buttons()
         if buttons == Qt.LeftButton:
             self.contour = self.findContour()
             item = self.scene().parent().maskItem
+            if item is None:
+                return
             item.update()
 
     def mouseReleaseEvent(self, event):
         self.x = int(event.pos().x())
         self.y = int(event.pos().y())
         button = event.button()
         if button == Qt.LeftButton:
             if self.contour is not None:
                 self.fillContour()
                 self.contour = None
 
     def findContour(self):
-        array = self.scene().parent().imageItem._array
+        item = self.scene().parent().imageItem
+        if item is None:
+            return
+        array = item._array
         nx, ny = array.shape
         if (self.x < 0) or (self.y < 0) or (self.x > nx-1) or (self.y > ny-1):
             return
         contours = skimage.measure.find_contours(array, level=array[self.x, self.y])
         # Extract only the contour that goes through the current position
         for contour in contours:
             n = contour.shape[0]
             for i in range(n):
                 p = contour[i,:]
                 if (p[0] == self.x) and (p[1] == self.y):
                     return contour
 
     def fillContour(self):
         item = self.scene().parent().maskItem
+        if item is None:
+            return
         bin = np.zeros(item.bin().shape, dtype=bool)
         rr, cc = skimage.draw.polygon(self.contour[:, 0], self.contour[:, 1], item.bin().shape)
         bin[rr, cc] = True
         if self.mode == "draw":
             item.setBin(np.logical_or(item.bin(), bin))
         elif self.mode == "cut":
             item.setBin(np.logical_and(item.bin(), np.logical_not(bin)))
@@ -607,90 +688,103 @@
 
     def mousePressEvent(self, event):
         self.x = int(event.pos().x())
         self.y = int(event.pos().y())
         if event.button() == Qt.LeftButton:
             self.contours = self.findContours()
             item = self.scene().parent().maskItem
+            if item is None:
+                return
             item.extend()
             item.update()
 
     def mouseMoveEvent(self, event):
         self.x = int(event.pos().x())
         self.y = int(event.pos().y())
         buttons = event.buttons()
         if buttons == Qt.LeftButton:
             self.contours = self.findContours()
             item = self.scene().parent().maskItem
+            if item is None:
+                return
             item.update()
 
     def mouseReleaseEvent(self, event):
         self.x = int(event.pos().x())
         self.y = int(event.pos().y())
         button = event.button()
         if button == Qt.LeftButton:
             if self.contours is not None:
                 self.fillContours()
                 self.contours = None
 
     def findContours(self):
-        array = self.scene().parent().imageItem._array
+        item = self.scene().parent().imageItem
+        if item is None:
+            return
+        array = item._array
         nx, ny = array.shape
         if (self.x < 0) or (self.y < 0) or (self.x > nx-1) or (self.y > ny-1):
             return
         item = self.scene().parent().maskItem
+        if item is None:
+            return
         if item.bin() is None:
             return skimage.measure.find_contours(array, level=array[self.x, self.y])
         elif item.bin().any():
             return skimage.measure.find_contours(array, level=array[self.x, self.y], mask=item.bin())
         else:
             return skimage.measure.find_contours(array, level=array[self.x, self.y])
 
     def fillContours(self):
         item = self.scene().parent().maskItem
+        if item is None:
+            return
         bin = np.zeros(item.bin().shape, dtype=bool)
         for contour in self.contours:
             rr, cc = skimage.draw.polygon(contour[:, 0], contour[:, 1], item.bin().shape)
             bin[rr, cc] = True
         if self.mode == "draw":
             item.setBin(np.logical_or(item.bin(), bin))
         elif self.mode == "cut":
             item.setBin(np.logical_and(item.bin(), np.logical_not(bin)))
         elif self.mode == "catch":
             item.setBin(np.logical_and(item.bin(), bin))
         item.setDisplay()
 
 
-
-
 class MaskThreshold(canvas.FilterItem):
     """Create mask by thresholding an image"""
     def __init__(self):
         super().__init__()
         pixMap = QPixmap(icons.controller_d_pad)
         self.cursor = QCursor(pixMap, hotX=8, hotY=8)
         self.toolTip = 'Threshold'
         self.text = 'Threshold'
         self.icon = QIcon(pixMap)
         self.setActionPick()
 
     def initialize(self):
         item = self.scene().parent().imageItem
+        if item is None:
+            return
         self.center, self.width = item._center, item._width
         self.array = item._array
         self.min = np.amin(self.array)
         self.max = np.amax(self.array)
         self.range = self.max-self.min
         #self.setData()
 
     def mousePressEvent(self, event):
         self.x = int(event.pos().x())
         self.y = int(event.pos().y())
         if event.button() == Qt.LeftButton:
             item = self.scene().parent().maskItem
+            if item is None:
+                return
             item.extend()
 
     def mouseMoveEvent(self, event):
         self.x = int(event.pos().x())
         self.y = int(event.pos().y())
         button = event.buttons()
         if button == Qt.LeftButton:
@@ -700,14 +794,18 @@
     def mouseReleaseEvent(self, event):
         self.x = int(event.pos().x())
         self.y = int(event.pos().y())
         self.update()
 
     def window(self, dx, dy):
         """Change intensity and contrast"""
+
+        item = self.scene().parent().maskItem
+        if item is None:
+            return
        
         # Move 1024 to change the center over the full range
         # Speed is faster further away from the center of the range
         center = self.center 
         v0 = self.range/512
         a0 = 1.0/64
         vy = v0 + a0*abs((center - (self.min+self.range/2.0)))
@@ -721,15 +819,14 @@
         vx = v0 + a0*width
         width = width + vx * dx
         self.width = width if width>1 else 1
 
         # Update display
         min, max = self.center-self.width/2, self.center+self.width/2
         threshold = np.logical_and(min<=self.array, self.array<=max)
-        item = self.scene().parent().maskItem
         item.setBin(threshold)
         item.setDisplay()
 
 
 class MaskPaintByNumbers(MaskBrush):
 
     def setMode(self, mode):
@@ -742,22 +839,18 @@
         elif mode == "erase":
             pixMap = QPixmap(icons.eraser__plus)
             self.cursor = QCursor(pixMap, hotX=0, hotY=16)
             self.toolTip = 'Erase by numbers'
             self.text = 'Erase by numbers'
         self.icon = QIcon(pixMap)
 
-    # def initialize(self):
-    #     #cnvs = self.scene().parent()
-    #     #self.array = cnvs.image.get_pixel_array()
-    #     item = self.scene().parent().imageItem
-    #     self.array = item._array
-
     def paintPixels(self):
         item = self.scene().parent().maskItem
+        if item is None:
+            return
         array = self.scene().parent().imageItem._array
         min = max = None 
         w = int((self.brushSize - 1)/2)
         for x in range(self.x-w, self.x+w+1, 1):
             if 0 <= x < item.bin().shape[0]:
                 for y in range(self.y-w, self.y+w+1, 1):
                     if 0 <= y < item.bin().shape[1]:
@@ -799,23 +892,19 @@
         elif mode == "erase":
             pixMap = QPixmap(icons.eraser__arrow)
             self.cursor = QCursor(pixMap, hotX=0, hotY=16)
             self.toolTip = 'Erase by growing..'
             self.text = 'Erase by growing..'
         self.icon = QIcon(pixMap)
 
-    # def initialize(self):
-    #     #cnvs = self.scene().parent()
-    #     #self.array = cnvs.image.get_pixel_array()
-    #     item = self.scene().parent().imageItem
-    #     self.array = item._array
-
     def paintPixels(self):
         # Get range of values under brush
         item = self.scene().parent().maskItem
+        if item is None:
+            return
         array = self.scene().parent().imageItem._array
         # Build a seed list of all pixels under the brush
         # and find minimum and maximum value over the seeds
         seed = []
         min = max = None 
         w = int((self.brushSize - 1)/2)
         for x in range(self.x-w, self.x+w+1, 1):
@@ -836,28 +925,28 @@
             return
         # Find the range of values with the given tolerance
         center = (max+min)/2
         width = self.tolerance*(max-min)/2
         max, min = center+width, center-width
         # Grow region to include all pixels in the same range
         if self.mode == 'paint':
-            #canvas.utils.region_grow_add(self.array, item.bin(), seed, min, max)
             canvas.utils.region_grow_add(array, item.bin(), seed, min, max)
         else:
-            #canvas.utils.region_grow_remove(self.array, item.bin(), seed, min, max)
             canvas.utils.region_grow_remove(array, item.bin(), seed, min, max)
         item.setDisplay()
 
+
     def setOptions(self, option):
         if 'tolerance' in option:
             self.tolerance = option['tolerance']
-        if 'size' in option:
+        elif 'size' in option:
             self.brushSize = option['size']
         self.pick()
 
+
     def menuOptions(self):
         menu = QMenu()
         menu.triggered.connect(lambda action: self.setOptions(action.option))
 
         actionGroup = QActionGroup(menu)
         options = {
             'Seed size: 1 pixel': 1,
@@ -905,14 +994,15 @@
 
 class MaskDilate(canvas.FilterItem):
     """Dilate mask
     """
     def __init__(self, kernelSize=3):
         super().__init__()
         self.setKernel(kernelSize)
+        self.mode = 'draw'
         pixMap = QPixmap(icons.arrow_out)
         self.icon = QIcon(pixMap)
         self.cursor = QCursor(pixMap, hotX=8, hotY=8)
         self.toolTip = 'Dilate'
         self.text = 'Dilate'
         self.setActionPick()
         
@@ -920,58 +1010,84 @@
         self.kernelSize = kernelSize
         self.kernel = cv2.getStructuringElement(cv2.MORPH_ELLIPSE, (self.kernelSize, self.kernelSize))
 
     def mousePressEvent(self, event):
         self.x = int(event.pos().x())
         self.y = int(event.pos().y())
         item = self.scene().parent().maskItem
+        if item is None:
+            return
         if event.button() == Qt.LeftButton:
-            item.extend()
+            bin = item.bin()
+            if bin is None:
+                return
             p = [self.x, self.y]
-            mask = item.bin().astype(np.uint8)
-            if item.bin()[p[0],p[1]]:
-                cluster = np.zeros(mask.shape, dtype=np.bool8)
-                cluster = canvas.utils.region_grow_add(mask, cluster, [p], 0.5, 1.5)
-                cluster = cv2.dilate(cluster.astype(np.uint8), self.kernel)
-                item.setBin(np.logical_or(item.bin(), cluster.astype(np.bool8)))
-            else:
-                mask = cv2.dilate(mask, self.kernel)
-                item.setBin(mask.astype(np.bool8))
-            item.setDisplay()
+            if bin[p[0],p[1]]:
+                bin = canvas.utils.dilate_cluster(bin, p, self.kernel, mode=self.mode)
+                item.extend()
+                item.setBin(bin)
+                item.setDisplay()
         
     def mouseMoveEvent(self, event):
         self.x = int(event.pos().x())
         self.y = int(event.pos().y())
 
-    def setOptions(self, kernelSize):
-        self.setKernel(kernelSize)
+    def setOptions(self, option):
+        if 'size' in option:
+            self.setKernel(option['size'])
+        if 'mode' in option:
+            self.mode = option['mode']
         self.pick()
 
     def menuOptions(self):
         menu = QMenu()
         menu.triggered.connect(lambda action: self.setOptions(action.option))
+
         actionGroup = QActionGroup(menu)
         options = {
-            '1 pixel': 1,
             '3 pixels': 3,
             '5 pixels': 5,
             '7 pixels': 7,
             '9 pixels': 9,
             '11 pixels': 11,
             '21 pixels': 21,
             '31 pixels': 31,
         }
         for text, value in options.items():
             action = QAction(text)
-            action.option = value
+            action.option = {'size': value}
             action.setCheckable(True)
             action.setChecked(value == self.kernelSize)
             actionGroup.addAction(action)
             menu.addAction(action)
 
+        self.addSeparator(menu)
+
+        actionGroup = QActionGroup(menu)
+        options = {
+            'Draw': 'draw',
+            'Cut': 'cut',
+            'Rescue': 'rescue',
+        }
+        icon = [
+            QIcon(icons.pencil), 
+            QIcon(icons.cutter), 
+            QIcon(icons.lifebuoy),
+        ]
+        i=0
+        for text, value in options.items():
+            action = QAction(text)
+            action.option = {'mode': value}
+            action.setCheckable(True)
+            action.setChecked(value == self.mode)
+            action.setIcon(icon[i])
+            i+=1
+            actionGroup.addAction(action)
+            menu.addAction(action)
+
         return menu
 
     def contextMenu(self):
         return self.actionPick.menu()
 
 
 class MaskShrink(MaskDilate):
@@ -986,53 +1102,330 @@
         self.text = 'Shrink'
         self.setActionPick()
 
     def mousePressEvent(self, event):
         self.x = int(event.pos().x())
         self.y = int(event.pos().y())
         item = self.scene().parent().maskItem
+        if item is None:
+            return
         if event.button() == Qt.LeftButton:
+            bin = item.bin()
+            if bin is None:
+                return
             p = [self.x, self.y]
+            if bin[p[0],p[1]]:
+                bin = canvas.utils.erode_cluster(bin, p, self.kernel, mode=self.mode)
+                item.extend()
+                item.setBin(bin)
+                item.setDisplay()
+
+
+class MaskOpen(MaskDilate):
+    """
+    Open Button (remove bright spots)
+    """
+    def __init__(self, kernelSize=3):
+        super().__init__(kernelSize=kernelSize)
+        pixMap = QPixmap(icons.minus_small_circle)
+        self.icon = QIcon(pixMap)
+        self.cursor = QCursor(pixMap, hotX=8, hotY=8)
+        self.toolTip = 'Remove bright spots'
+        self.text = 'Remove bright spots'
+        self.setActionPick()
+
+    def mousePressEvent(self, event):
+        self.x = int(event.pos().x())
+        self.y = int(event.pos().y())
+        item = self.scene().parent().maskItem
+        if item is None:
+            return
+        if event.button() == Qt.LeftButton:
+            bin = item.bin()
+            p = [self.x, self.y]
+            if bin is None:
+                if self.mode == 'draw':
+                    bin = self._grow_from(p)
+                    self._open(p, bin)
+            else:
+                if bin[p[0],p[1]]:
+                    self._open(p, bin, split=True)
+                elif self.mode == 'draw':
+                    cluster = self._grow_from(p)
+                    cluster = canvas.utils.open_cluster(cluster, p, self.kernel, mode=self.mode)
+                    bin = np.logical_or(bin, cluster.astype(np.bool8))
+                    item = self.scene().parent().maskItem
+                    if item is None:
+                        return
+                    item.extend()
+                    item.setBin(bin)
+                    item.setDisplay()
+
+    def _grow_from(self, p):
+        item = self.scene().parent().imageItem
+        if item is None:
+            return
+        array = item._array
+        return canvas.utils.pick_cluster(array, p)
+
+    def _open(self, p, bin, split=False):
+        if np.count_nonzero(bin) > 0:
+            bin = canvas.utils.open_cluster(bin, p, self.kernel, mode=self.mode, split=split)
+            item = self.scene().parent().maskItem
+            if item is None:
+                return
             item.extend()
-            mask = item.bin().astype(np.uint8)
-            if item.bin()[p[0],p[1]]:
-                # Find the selected cluster, take it out, erode it and put it back in
-                cluster = np.zeros(mask.shape, dtype=np.bool8)
-                cluster = canvas.utils.region_grow_add(mask, cluster, [p], 0.5, 1.5)
-                item.setBin(np.logical_and(item.bin(), np.logical_not(cluster)))
-                cluster = cv2.erode(cluster.astype(np.uint8), self.kernel)
-                item.setBin(np.logical_or(item.bin(), cluster.astype(np.bool8)))
+            item.setBin(bin)
+            item.setDisplay()
+            
+
+class MaskClose(MaskDilate):
+    """
+    Close Button (remove dark spots)
+    """
+    def __init__(self, kernelSize=3):
+        super().__init__(kernelSize=kernelSize)
+        pixMap = QPixmap(icons.plus_small_white)
+        self.icon = QIcon(pixMap)
+        self.cursor = QCursor(pixMap, hotX=8, hotY=8)
+        self.toolTip = 'Remove dark spots'
+        self.text = 'Remove dark spots'
+        self.setActionPick()
+
+    def mousePressEvent(self, event):
+        self.x = int(event.pos().x())
+        self.y = int(event.pos().y())
+        item = self.scene().parent().maskItem
+        if item is None:
+            return
+        if event.button() == Qt.LeftButton:
+            bin = item.bin()
+            p = [self.x, self.y]
+            if bin is None:
+                if self.mode == 'draw':
+                    bin = self._grow_from(p)
+                    self._close(p, bin)
             else:
-                mask = cv2.erode(mask, self.kernel)
-                item.setBin(mask.astype(np.bool8))
+                if bin[p[0],p[1]]:
+                    self._close(p, bin)
+                elif self.mode == 'draw':
+                    cluster = self._grow_from(p)
+                    cluster = canvas.utils.close_cluster(cluster, p, self.kernel, mode=self.mode)
+                    bin = np.logical_or(bin, cluster.astype(np.bool8))
+                    item = self.scene().parent().maskItem
+                    if item is None:
+                        return
+                    item.extend()
+                    item.setBin(bin)
+                    item.setDisplay()
+
+    def _grow_from(self, p):
+        item = self.scene().parent().imageItem
+        if item is None:
+            return
+        array = item._array
+        return canvas.utils.pick_cluster(array, p)
+
+    def _close(self, p, bin):
+        if np.count_nonzero(bin) > 0:
+            item = self.scene().parent().maskItem
+            if item is None:
+                return
+            bin = canvas.utils.close_cluster(bin, p, self.kernel, mode=self.mode)
+            item.extend()
+            item.setBin(bin)
             item.setDisplay()
 
 
+class MaskWand(canvas.FilterItem):
+    """
+    Close then open
+    """
+    def __init__(self, brightKernelSize=1, darkKernelSize=1):
+        super().__init__()
+        self.setBrightKernel(brightKernelSize)
+        self.setDarkKernel(darkKernelSize)
+        self.mode = 'draw'
+        pixMap = QPixmap(icons.wand)
+        self.icon = QIcon(pixMap)
+        self.cursor = QCursor(pixMap, hotX=0, hotY=16)
+        self.toolTip = 'Remove spots'
+        self.text = 'Remove spots'
+        self.setActionPick()
+
+    def setDarkKernel(self, kernelSize):
+        self.darkKernelSize = kernelSize
+        if kernelSize == 1:
+            self.darkKernel = None
+        else:
+            self.darkKernel = cv2.getStructuringElement(cv2.MORPH_ELLIPSE, (kernelSize, kernelSize))
+
+    def setBrightKernel(self, kernelSize):
+        self.brightKernelSize = kernelSize
+        if kernelSize == 1:
+            self.brightKernel = None
+        else:
+            self.brightKernel = cv2.getStructuringElement(cv2.MORPH_ELLIPSE, (kernelSize, kernelSize))
+
+    def setOptions(self, option):
+        if 'dark size' in option:
+            self.setDarkKernel(option['dark size'])
+        elif 'bright size' in option:
+            self.setBrightKernel(option['bright size'])
+        elif 'mode' in option:
+            self.mode = option['mode']
+        self.pick()
+
+    def menuOptions(self):
+        menu = QMenu()
+        menu.triggered.connect(lambda action: self.setOptions(action.option))
+
+        actionGroup = QActionGroup(menu)
+        options = {
+            'Do not remove dark spots': 1,
+            'Remove dark spots less than 3 pixels': 3,
+            'Remove dark spots less than 5 pixels': 5,
+            'Remove dark spots less than 7 pixels': 7,
+            'Remove dark spots less than 9 pixels': 9,
+            'Remove dark spots less than 11 pixels': 11,
+            'Remove dark spots less than 21 pixels': 21,
+            'Remove dark spots less than 31 pixels': 31,
+        }
+        for text, value in options.items():
+            action = QAction(text)
+            action.option = {'dark size': value}
+            action.setCheckable(True)
+            action.setChecked(value == self.darkKernelSize)
+            actionGroup.addAction(action)
+            menu.addAction(action)
+
+        self.addSeparator(menu)
+
+        actionGroup = QActionGroup(menu)
+        options = {
+            'Do not remove bright spots': 1,
+            'Remove bright spots less than 3 pixels': 3,
+            'Remove bright spots less than 5 pixels': 5,
+            'Remove bright spots less than 7 pixels': 7,
+            'Remove bright spots less than 9 pixels': 9,
+            'Remove bright spots less than 11 pixels': 11,
+            'Remove bright spots less than 21 pixels': 21,
+            'Remove bright spots less than 31 pixels': 31,
+        }
+        for text, value in options.items():
+            action = QAction(text)
+            action.option = {'bright size': value}
+            action.setCheckable(True)
+            action.setChecked(value == self.brightKernelSize)
+            actionGroup.addAction(action)
+            menu.addAction(action)
+
+        self.addSeparator(menu)
+
+        actionGroup = QActionGroup(menu)
+        options = {
+            'Draw': 'draw',
+            'Cut': 'cut',
+            'Rescue': 'rescue',
+        }
+        icon = [
+            QIcon(icons.pencil), 
+            QIcon(icons.cutter), 
+            QIcon(icons.lifebuoy),
+        ]
+        i=0
+        for text, value in options.items():
+            action = QAction(text)
+            action.option = {'mode': value}
+            action.setCheckable(True)
+            action.setChecked(value == self.mode)
+            action.setIcon(icon[i])
+            i+=1
+            actionGroup.addAction(action)
+            menu.addAction(action)
+
+        return menu
+
+    def contextMenu(self):
+        return self.actionPick.menu()
+
+    def mouseMoveEvent(self, event):
+        self.x = int(event.pos().x())
+        self.y = int(event.pos().y())
+
+    def mousePressEvent(self, event):
+        self.x = int(event.pos().x())
+        self.y = int(event.pos().y())
+        item = self.scene().parent().maskItem
+        if item is None:
+            return
+        if event.button() == Qt.LeftButton:
+            bin = item.bin()
+            p = [self.x, self.y]
+            if bin is None:
+                if self.mode == 'draw':
+                    bin = self._grow_from(p)
+                    self._close_open(p, bin)
+            else:
+                if bin[p[0],p[1]]:
+                    self._close_open(p, bin, split=True)
+                elif self.mode == 'draw':
+                    cluster = self._grow_from(p)
+                    cluster = canvas.utils.open_cluster(cluster, p, self.brightKernel, mode=self.mode)
+                    cluster = canvas.utils.close_cluster(cluster, p, self.darkKernel, mode=self.mode)
+                    bin = np.logical_or(bin, cluster.astype(np.bool8))
+                    item = self.scene().parent().maskItem
+                    if item is None:
+                        return
+                    item.extend()
+                    item.setBin(bin)
+                    item.setDisplay()
+
+    def _grow_from(self, p):
+        item = self.scene().parent().imageItem
+        if item is None:
+            return
+        array = item._array
+        return canvas.utils.pick_cluster(array, p)
+
+    def _close_open(self, p, bin, split=False):
+        if np.count_nonzero(bin) > 0:
+            bin = canvas.utils.open_cluster(bin, p, self.brightKernel, mode=self.mode, split=split)
+            bin = canvas.utils.close_cluster(bin, p, self.darkKernel, mode=self.mode)
+            item = self.scene().parent().maskItem
+            if item is None:
+                return
+            item.extend()
+            item.setBin(bin)
+            item.setDisplay()         
+
+
 class MaskKidneyEdgeDetection(canvas.FilterItem):
 
     def __init__(self):
         super().__init__()
         pixMap = QPixmap(icons.wand)
         self.icon = QIcon(pixMap)
         self.cursor = QCursor(pixMap, hotX=0, hotY=16)
         self.toolTip = 'Pick a kidney'
         self.text = 'Kidney picker'
         self.setActionPick()
 
-    # def initialize(self):
-    #     item = self.scene().parent().imageItem
-    #     self.array = item._array
 
     def mousePressEvent(self, event):
         self.x = int(event.pos().x())
         self.y = int(event.pos().y())
         if event.button() == Qt.LeftButton:
             cnvs = self.scene().parent()
+            if cnvs.imageItem is None:
+                return
             array = cnvs.imageItem._array
             item = cnvs.maskItem
+            if item is None:
+                return
             pixelSize = cnvs.parent().sliders.image.PixelSpacing # Hack!!! Some filters need access to geometry!
             pixels = canvas.utils.kidneySegmentation(array, self.y, self.x, pixelSize)
             if pixels is not None:
                 item.extend()
                 item.setBin(np.logical_or(item.bin(), pixels.astype(np.bool8)))
                 item.setDisplay()
```

### Comparing `wezel-0.1.1/src/wezel/canvas/scene_filter.py` & `wezel-0.1.2/src/wezel/canvas/scene_filter.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,10 +1,10 @@
-from PyQt5.QtCore import Qt, QRectF
-from PyQt5.QtWidgets import QGraphicsObject, QGraphicsItem, QAction, QMenu, QPushButton
-from PyQt5.QtGui import QPixmap, QCursor, QIcon, QColor, QPen, QTransform
+from PySide2.QtCore import Qt, QRectF
+from PySide2.QtWidgets import QGraphicsObject, QGraphicsItem, QAction, QMenu, QPushButton
+from PySide2.QtGui import QPixmap, QCursor, QIcon, QColor, QPen, QTransform
 
 from wezel import canvas, icons
 
 class PanFilter(canvas.FilterItem):
     """Panning the scene
     """
     def __init__(self):
```

### Comparing `wezel-0.1.1/src/wezel/canvas/series_canvas.py` & `wezel-0.1.2/src/wezel/canvas/series_canvas.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,11 +1,12 @@
 import timeit
 import random
 import numpy as np
-from PyQt5.QtCore import pyqtSignal
+
+from dbdicom.wrappers import scipy
 
 from wezel import widgets, canvas
 from wezel.canvas.utils import colormap_to_LUT
 
 class SeriesCanvas(canvas.Canvas):
 
     def __init__(self, parent=None):
@@ -34,42 +35,41 @@
         super().setImage(
             array, 
             self._model.center(), 
             self._model.width(), 
             self._model.colormap(),
         )
 
+    def setBlank(self):
+        self._model.setArray()
+        super().setBlank()
+
     def changeArray(self, array, uid, center, width, colormap):
 
         # Save current mask
-        bin = self.maskItem.bin()
-        if bin is not None:
-            if self._model._regions == []:
-                self.addRegion()
-                if self.toolBar is not None:
-                    self.toolBar.newRegion()
-        self._model.setMask(bin)
+        if self.maskItem is not None:
+            bin = self.maskItem.bin()
+            if bin is not None:
+                if self._model._regions == []:
+                    self.addRegion()
+                    if self.toolBar is not None:
+                        self.toolBar.newRegion()
+            self._model.setMask(bin)
 
         # update toolbar and display
-        self._model.setArray(
-            uid,
-            center,
-            width,
-            colormap)
+        self._model.setArray(uid, center, width, colormap)
+        super().setImage(array, 
+            self._model.center(), 
+            self._model.width(), 
+            self._model.colormap())
         if self.toolBar is not None:
-            self.toolBar.setArray(
-                array,
+            self.toolBar.setArray(array,
                 self._model.center(), 
                 self._model.width(), 
                 self._model.colormap())
-        super().setImage(
-            array, 
-            self._model.center(), 
-            self._model.width(), 
-            self._model.colormap())
 
         # get new mask
         mask = self._model.mask()
         self.setMask(mask, color=self._model.color())
 
 
     def removeCurrentRegion(self):
@@ -118,14 +118,16 @@
 
     def loadRegion(self):
         self._model.loadRegion()
         self.setMask(self._model.mask(), color=self._model.color())
 
     def setColormap(self, cmap=None):
         super().setColormap(cmap)
+        if self.imageItem is None:
+            return
         self._model._cmap[self._model._currentImage] = cmap
         self._model._lut[self._model._currentImage] = self.imageItem._lut
 
     def setWindow(self, center=None, width=None):
         super().setWindow(center, width)
         self._model.setWindow(self.center(), self.width())
 
@@ -146,31 +148,43 @@
         self._lut = {}
         self._cmap = {}
         self._regions = []
         self._currentRegion = None # dict
         self._currentImage = None # uid
 
     def center(self):
+        if self._currentImage is None:
+            return
         return self._center[self._currentImage]
 
     def width(self):
+        if self._currentImage is None:
+            return
         return self._width[self._currentImage]
 
     def lut(self):
+        if self._currentImage is None:
+            return
         return self._lut[self._currentImage]
 
     def colormap(self):
+        if self._currentImage is None:
+            return
         return self._cmap[self._currentImage]
 
     def setWindow(self, center, width):
+        if self._currentImage is None:
+            return
         self._center[self._currentImage] = center
         self._width[self._currentImage] = width
 
-    def setArray(self, uid, center, width, colormap):
+    def setArray(self, uid=None, center=None, width=None, colormap=None):
         self._currentImage = uid
+        if uid is None:
+            return
         if uid in self._center.keys():
             return
         self._center[uid] = center
         self._width[uid] = width
         self._lut[uid] = colormap_to_LUT(colormap)
         self._cmap[uid] = colormap
 
@@ -178,22 +192,26 @@
         if self._currentRegion is None:
             return 0
         return self._currentRegion['color']
 
     def mask(self):
         if self._currentRegion is None:
             return
+        if self._currentImage is None:
+            return
         if self._currentImage in self._currentRegion:
             return self._currentRegion[self._currentImage]
 
     def setMask(self, bin):
         if bin is None:
             return
         if self._currentRegion is None:
             return
+        if self._currentImage is None:
+            return
         self._currentRegion[self._currentImage] = bin
         
     def setColor(self, RGB):
         if self._currentRegion is None:
             return
         self._currentRegion['color'] = RGB
 
@@ -250,57 +268,70 @@
             random.randint(0,255), 
             random.randint(0,255), 
             random.randint(0,255)]
 
 
     def saveRegions(self):
         #start = timeit.default_timer()
+        databaseUpdated = False
         series = self._series
         if not series.exists():
-            return
+            return databaseUpdated
         images = series.instances()
         for region in self._regions:
             if len(region.keys()) > 2:
+                databaseUpdated = True
                 roi_series = series.new_sibling(SeriesDescription=region['name'])
                 for cnt, image in enumerate(images):
                     series.status.progress(cnt+1, len(images), 'Saving region '+ region['name'])
                     uid = image.SOPInstanceUID
                     if uid in region:
                         array = region[uid].astype(np.float32)
                         mask = image.copy_to(roi_series)
                         mask.set_array(array)
                         mask.WindowCenter = 0.5
                         mask.WindowWidth = 1.0
         series.status.hide()
         #print(timeit.default_timer()-start)
+        return databaseUpdated
 
 
     def loadRegion(self):
         # Build list of series for all series in the same study
         seriesList = self._series.parent().children()
-        seriesLabels = [series.instance().SeriesDescription for series in seriesList]
         # Ask the user to select series to import as regions
         input = widgets.UserInput(
-            {"label":"Series:", "type":"listview", "list": seriesLabels}, 
+            {"label":"Import as mask:", "type":"select records", "options": seriesList}, 
             title = "Please select regions to load")
         if input.cancel:
             return
-        seriesList = [seriesList[i] for i in input.values[0]["value"]]
-        seriesLabels = [seriesLabels[i] for i in input.values[0]["value"]]
-        suffix = ' mapped to ' + self._series.instance().SeriesDescription
         # Overlay each of the selected series on the displayed series
-        for s, series in enumerate(seriesList):
-            # Create overlay
-            region, images = series.map_mask_to(self._series)
-            # Add new region
-            newRegion = {'name': seriesLabels[s] + suffix, 'color': self.newColor()}
-            if isinstance(region, list): # If self._series has multiple slice groups
-                for r, reg in enumerate(region):
-                    for i, image in np.ndenumerate(images[r]):
-                        if image is not None:
-                            newRegion[image.SOPInstanceUID] = reg[:,:,i[0]] != 0
+        for series in input.values[0]:
+            try:
+                # Add new region
+                newRegion = {
+                    'name': series.instance().SeriesDescription, 
+                    'color': self.newColor()}
+                # Create overlay
+                region, images = scipy.mask_array(series, on=self._series)
+                _add_slice_groups_to(newRegion, region, images)
+            except:
+                self._series.dialog.error()
             else:
-                for i, image in np.ndenumerate(images):
-                    if image is not None:
-                        newRegion[image.SOPInstanceUID] = region[:,:,i[0]] != 0
-            self._regions.append(newRegion)
-            self._currentRegion = newRegion
+                self._regions.append(newRegion)
+                self._currentRegion = newRegion
+
+def _add_slice_groups_to(newRegion, region, images):
+    if isinstance(region, list): 
+        # If self._series has multiple slice groups
+        for r, reg in enumerate(region):
+            _add_to(newRegion, reg, images[r])
+    else:
+        # Single slice group only
+        _add_to(newRegion, region, images)
+
+def _add_to(newRegion, region, images):
+    for i, image in np.ndenumerate(images):
+        if image is not None:
+            mask = region[:,:,i[0],i[1]] 
+            if np.count_nonzero(mask) > 0:
+                newRegion[image.SOPInstanceUID] = mask != 0
```

### Comparing `wezel-0.1.1/src/wezel/canvas/toolbar.py` & `wezel-0.1.2/src/wezel/canvas/toolbar.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 import numpy as np
 
-from PyQt5.QtWidgets import (
+from PySide2.QtWidgets import (
     QWidget, QGridLayout, 
     QToolBar, QAction, QMenu,
     QActionGroup, QFrame)
-from PyQt5.QtGui import QIcon
+from PySide2.QtGui import QIcon
 
 from wezel import canvas, icons, widgets
 
 
 def defaultFilters():
     return [
         canvas.PanFilter(),
@@ -22,15 +22,17 @@
         canvas.MaskPaintByNumbers(mode='erase'),
         canvas.MaskRegionGrowing(mode='erase'),
         canvas.MaskPenSet(mode='draw'),
         canvas.MaskPenSet(mode='cut'),
         canvas.MaskPenSet(mode='catch'),
         canvas.MaskDilate(),
         canvas.MaskShrink(),
-        canvas.MaskKidneyEdgeDetection(),
+        canvas.MaskWand(),
+        canvas.MaskMove(),
+        #canvas.MaskKidneyEdgeDetection(),
     ]
 
 
 class ToolBar(QWidget):
 
     def __init__(self, parent=None, filters=None):
         super().__init__(parent)
@@ -39,15 +41,15 @@
         if filters is not None:
             self.filters = filters
         else:
             self.filters = defaultFilters()
 
         # Define UI elements
         self.regionList = widgets.RegionList(layout=None)
-        self.window = widgets.ImageWindow(layout=False)
+        self.window = widgets.ImageWindow()
         self.actionFitItem = QAction(QIcon(icons.magnifier_zoom_fit), 'Fit in view', self)
         self.menuZoomToScale = self.menuZoomTo()
         self.actionZoomTo = QAction(QIcon(icons.magnifier_zoom_actual), 'Zoom to..', self)
         self.actionZoomTo.setMenu(self.menuZoomToScale)
         self.actionFitItemAndZoom = QAction(QIcon(icons.magnifier_zoom_fit), 'Fit in view', self)
         self.actionFitItemAndZoom.setMenu(self.menuZoomToScale)
         self.actionZoomIn = QAction(QIcon(icons.magnifier_zoom_in), 'Zoom in..', self)
@@ -123,55 +125,72 @@
         self.setEditMaskEnabled()
     
     def newRegion(self):
         self.setEditMaskEnabled()
         self.regionList.setView()
 
     def setArray(self, array, center, width, colormap):
+        self.setEnabled(array is not None)
+        if array is None:
+            return
         self.setEditMaskEnabled()
-        if self.window.mode.isLocked:
+        if self.window.isLocked():
             v = self.window.getValue()
             cmap = self.filters[2].getColorMap()
             self.canvas.setWindow(v[0], v[1])
             self.canvas.setColormap(cmap)
         else:
             self.window.setData(array, center, width)
             self.filters[2].setChecked(colormap)
 
     def setEditMaskEnabled(self, enable=None):
         if enable is None:
             item = self.canvas.maskItem
-            undoEnable = item._current!=0 and item._current is not None
-            redoEnable = item._current!=len(item._bin)-1 and item._current is not None
-            if item.bin() is None:
+            if item is None:
+                undoEnable = False
+                redoEnable = False
                 eraseEnable = False
             else:
-                eraseEnable = item.bin().any()
+                undoEnable = item._current!=0 and item._current is not None
+                redoEnable = item._current!=len(item._bin)-1 and item._current is not None
+                # Small bug here - does not reset properly when slices
+                # are changed. Skipping for now..
+                # if item.bin() is None:
+                #     eraseEnable = False
+                # else:
+                #     eraseEnable = item.bin().any()
+                eraseEnable = True
         else:
             undoEnable = enable
             redoEnable = enable
             eraseEnable = enable
         self.actionUndo.setEnabled(undoEnable)
         self.actionRedo.setEnabled(redoEnable)
         self.actionErase.setEnabled(eraseEnable)
 
     def undo(self):
         item = self.canvas.maskItem
+        if item is None:
+            return
         item.undo()
         self.canvas.saveMask()
         self.setEditMaskEnabled()
 
     def redo(self):
         item = self.canvas.maskItem
+        if item is None:
+            return
         item.redo()
         self.canvas.saveMask()
         self.setEditMaskEnabled()
 
     def erase(self):
         item = self.canvas.maskItem
+        if item is None:
+            return
         item.erase()
         self.canvas.saveMask()
         self.setEditMaskEnabled()
 
     def setDefaultColor(self):
         self.canvas.setWindow()
         self.canvas.setColormap()
@@ -274,16 +293,18 @@
         framegrid.addWidget(w,0,0)
         w = QToolBar()
         w.addAction(toolBar.actionSetDefaultColor)
         framegrid.addWidget(w,0,1)
         w = QToolBar()
         w.addAction(toolBar.filters[2].actionPick)
         framegrid.addWidget(w,0,2)
-        framegrid.addWidget(toolBar.window.brightness.spinBox, 1, 0, 1, 3)
-        framegrid.addWidget(toolBar.window.contrast.spinBox, 2, 0, 1, 3)
+        #framegrid.addWidget(toolBar.window.spinBox(1), 1, 0, 1, 3)
+        #framegrid.addWidget(toolBar.window.spinBox(0), 2, 0, 1, 3)
+        framegrid.addWidget(toolBar.window.upper, 1, 0, 1, 3)
+        framegrid.addWidget(toolBar.window.lower, 2, 0, 1, 3)
         frame.setLayout(framegrid)
         return frame
     
     def _getWidgetRegion(self, toolBar):
         frame = QFrame()
         frame.setFrameStyle(QFrame.Panel | QFrame.Raised)
         framegrid = QGridLayout()
@@ -352,14 +373,17 @@
         framegrid.addWidget(w,4,1)
         w = QToolBar()
         w.addAction(toolBar.filters[14].actionPick)
         framegrid.addWidget(w,4,2)
         w = QToolBar()
         w.addAction(toolBar.filters[15].actionPick)
         framegrid.addWidget(w,5,0)
+        w = QToolBar()
+        w.addAction(toolBar.filters[16].actionPick)
+        framegrid.addWidget(w,5,1)
         frame.setLayout(framegrid)
         return frame
 
 
 class ActionOpacity(QAction):
     def __init__(self):
         super().__init__()
```

### Comparing `wezel-0.1.1/src/wezel/core.py` & `wezel-0.1.2/src/wezel/widgets/qrangeslider.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,400 +1,313 @@
+# https://stackoverflow.com/questions/47342158/porting-range-slider-widget-to-PySide2
 
+import sys, os
+from PySide2 import QtCore, QtGui, QtWidgets
 
-import sys
-import logging
+__all__ = ['QRangeSlider']
 
-#from PyQt5.QtCore import *
-from PyQt5.QtCore import Qt
-from PyQt5.QtWidgets import (
-    QWidget, 
-    QApplication, 
-    QMainWindow, 
-    QAction, 
-    QMenu, 
-    QMenuBar, 
-    QDockWidget, 
-    QMessageBox) 
-from PyQt5.QtGui import QIcon
-
-import dbdicom as db
-import wezel
-
-QApplication.setAttribute(Qt.AA_EnableHighDpiScaling, True)
-QApplication.setAttribute(Qt.AA_UseHighDpiPixmaps, True)
-
-
-# Examples of style sheets
-# https://doc.qt.io/qtforpython/overviews/stylesheet-examples.html
-# 
-
-STYLESHEET = """ 
-    QMdiArea {
-        background-color: rgb(32, 32, 32);
-    }
-    QDockWidget {
-        border: 0px;
-    }
-    QScrollBar:vertical {
-        border: 0px ;
-        background: black;
-        width: 10px;
-    }
-    QScrollBar::handle:vertical {
-        background: rgb(32, 32, 32);
-        min-height: 20px;
-    }
-    QMainWindow {
-        background: rgb(128, 128, 128);
-    }
-    QMainWindow::separator {
-        width: 2px; /* when vertical */
-        height: 2px; /* when horizontal */
-    }
-    QMenuBar {
-        background-color: rgb(128, 128, 128); 
-    }
-    QTreeView {
-        background: rgb(32, 32, 32);
-    }
-    QTreeView::item { 
-        color: rgb(128, 128, 128);
-    }
-    QTreeView::item:selected { 
-        background-color: rgb(32, 32, 64);
-    }
-    """
-
-
-class Wezel:
-
-    def __init__(self):
-        self.log = logger()
-        self.QApp = QApplication(sys.argv)
-        self.QApp.setWindowIcon(QIcon(wezel.icons.favicon))
-        self.main = Main(self)
-
-    def open(self, path):
-        self.main.open(path)
-
-    def show(self):    
-        self.log.info('Launching Wezel!')
-        try:
-            self.main.show()
-            self.QApp.exec()
-            #sys.exit(self.QApp.exec())
-        except Exception as e:
-            print('Error: ' + str(e))
-            self.log.exception('Error: ' + str(e))
-
-
-class Main(QMainWindow):
-
-    def __init__(self, wzl): 
-        super().__init__()
-        self.wezel = wzl
-        #self.setStyleSheet(STYLESHEET)
-        self.setWindowTitle("Wezel")
-        #self.setWindowIcon(QIcon(wezel.icons.favicon))
-
-        self.dialog = wezel.widgets.Dialog(self)
-        self.status = wezel.widgets.StatusBar()
-        self.setStatusBar(self.status)
-
-        self.toolBar = {}
-        self.toolBarDockWidget = QDockWidget()
-        self.addDockWidget(Qt.RightDockWidgetArea, self.toolBarDockWidget)
-        self.toolBarDockWidget.hide()
-
-        self.treeView = None
-        self.treeViewDockWidget = QDockWidget()
-        self.addDockWidget(Qt.LeftDockWidgetArea, self.treeViewDockWidget)
-        self.treeViewDockWidget.hide()
-
-        self.folder = None # should be in TreeView
-        self.central = wezel.widgets.MainMultipleDocumentInterface()
-        self.central.subWindowActivated.connect(lambda subWindow: self.activateSubWindow(subWindow))
-        self.setCentralWidget(self.central)
-
-        self.set_menu(wezel.menus.dicom)
-
-    def closeEvent(self, event): #main
-        accept = self.close()
-        if accept:
-            event.accept()
-        else:
-            event.ignore()
-
-    def set_menu(self, menu):
-        self.menubar = MenuBar(self, menu)
-        self.setMenuBar(self.menubar)
-
-    def open(self, path):
-        self.folder = db.database(path=path, 
-            status = self.status, 
-            dialog = self.dialog)
-        self.display(self.folder)
-        self.status.hide()
-
-    def close(self):
-        """Closes the application."""
-        if self.folder is None:
-            return True
-        accept = self.folder.close()
-        if accept:
-            self.folder = None
-            self.toolBarDockWidget.hide()
-            self.treeViewDockWidget.hide()
-            for subWindow in self.central.subWindowList():
-                self.central.removeSubWindow(subWindow)
-            self.menuBar().enable()
-        return accept
-
-    def refresh(self):
-        """
-        Refreshes the Wezel display.
-        """
-        self.status.message('Refreshing display..')
-        self.treeView.setFolder()
-        self.menuBar().enable()
-        self.status.hide()
-        
-    def display(self, object):
-        if object.type() == 'Database':
-            self.treeView = wezel.widgets.DICOMFolderTree(object)
-            self.treeView.itemSelectionChanged.connect(self.menuBar().enable)
-            self.treeViewDockWidget.setWidget(self.treeView)
-            self.treeViewDockWidget.show()
-            self.menuBar().enable()
-        elif object.type() == 'Patient': # No Patient Viewer yet
-            pass
-        elif object.type() == 'Study': # No Study Viewer yet
-            pass
-        elif object.type() == 'Series':
-            seriesDisplay = wezel.widgets.SeriesDisplay()
-            seriesDisplay.setSeries(object)
-            self.addWidget(seriesDisplay, title=object.label())
-        elif object.type() == 'Instance':
-            pass
-
-    def addWidget(self, widget, title):
-        # rename to addMainWidget()
-        # widget needs to be subclassed from MainWidget
-        if widget.error:
-            return
-        subWindow = self.central.addWidget(widget, title)
-        subWindow.closed.connect(lambda: self.closeSubWindow(subWindow))
-        self.central.tileSubWindows()
-        if widget.toolBarClass is not None:
-            toolBarName =  widget.toolBarClass.__name__
-            if toolBarName in self.toolBar:
-                toolBar = self.toolBar[toolBarName]
-                widget.setToolBar(toolBar)
-            else:
-                toolBar =  widget.toolBarClass()
-                self.toolBar[toolBarName] = toolBar
-                self.toolBarDockWidget.setWidget(toolBar)
-                widget.setToolBar(toolBar)
-                self.toolBarDockWidget.show()
-
-    def closeSubWindow(self, subWindow):
-        self.central.removeSubWindow(subWindow)
-        self.central.tileSubWindows()
-        widget = subWindow.widget().__class__.__name__
-        if 0 == self.central.countSubWindow(widget):
-            self.toolBarDockWidget.hide()
-        self.refresh()
-
-    def activateSubWindow(self, subWindow):
-        if self.central.activeWindow == subWindow:
-            return
-        activeWindow = self.central.activeWindow
-        if activeWindow is not None:
-            activeWindow.widget().setActive(False)
-        self.central.activeWindow = subWindow
-        if subWindow is not None:
-            subWindow.widget().setActive(True)
-
-    def get_selected(self, generation):   
-        if self.treeView is None: 
-            return []
-        return self.treeView.get_selected(generation)
-
-    def selected(self, generation):
-        if self.treeView is None: 
-            return []
-        return self.treeView.selected(generation)
- 
-    def nr_selected(self, generation):
-        if self.treeView is None: 
-            return 0
-        return self.treeView.nr_selected(generation)
-
-
-class MainWidget(QWidget):
-    """Base class for widgets that are set as subWindow widgets"""
-
-    def __init__(self):
-        super().__init__()
-        self.toolBarClass = None
-        self.toolBar = None
-        self.error = False
-
-    def setError(self, message='Error displaying data!!'):
-        self.error = True
-        QMessageBox.information(self, 'Information', message)
-
-    def setToolBar(self, toolBar):
-        self.toolBar = toolBar
-        self.setToolBarState()
-
-    def setToolBarState(self):
-        self.toolBar.setWidget(self)
-        
-    def setActive(self, active):
-        if active:
-            if self.toolBar is not None:
-                self.setToolBarState()
-                subWindow = self.parentWidget()
-                mdiArea = subWindow.mdiArea()
-                mainWindow = mdiArea.parentWidget()
-                mainWindow.toolBarDockWidget.setWidget(self.toolBar)
-                
-    def closeEvent(self, event):
-        pass
-
-
-
-class MenuBar(QMenuBar):
-    """
-    Programming interfaces for the Wezel menus. 
-    """
-
-    def __init__(self, main, menu):
-        super().__init__()
-
-        self._menus = []
+DEFAULT_CSS = """
+QRangeSlider * {
+    border: 0px;
+    padding: 0px;
+}
+QRangeSlider #Head {
+    background: #222;
+}
+QRangeSlider #Span {
+    background: #393;
+}
+QRangeSlider #Span:active {
+    background: #282;
+}
+QRangeSlider #Tail {
+    background: #222;
+}
+QRangeSlider > QSplitter::handle {
+    background: #393;
+}
+QRangeSlider > QSplitter::handle:vertical {
+    height: 4px;
+}
+QRangeSlider > QSplitter::handle:pressed {
+    background: #ca5;
+}
+"""
+
+def scale(val, src, dst):
+    return int(((val - src[0]) / float(src[1]-src[0])) * (dst[1]-dst[0]) + dst[0])
+
+
+class Ui_Form(object):
+    def setupUi(self, Form):
+        Form.setObjectName("QRangeSlider")
+        Form.resize(300, 30)
+        Form.setStyleSheet(DEFAULT_CSS)
+        self.gridLayout = QtWidgets.QGridLayout(Form)
+        self.gridLayout.setContentsMargins(0, 0, 0, 0)
+        self.gridLayout.setSpacing(0)
+        self.gridLayout.setObjectName("gridLayout")
+        self._splitter = QtWidgets.QSplitter(Form)
+        self._splitter.setMinimumSize(QtCore.QSize(0, 0))
+        self._splitter.setMaximumSize(QtCore.QSize(16777215, 16777215))
+        self._splitter.setOrientation(QtCore.Qt.Horizontal)
+        self._splitter.setObjectName("splitter")
+        self._head = QtWidgets.QGroupBox(self._splitter)
+        self._head.setTitle("")
+        self._head.setObjectName("Head")
+        self._handle = QtWidgets.QGroupBox(self._splitter)
+        self._handle.setTitle("")
+        self._handle.setObjectName("Span")
+        self._tail = QtWidgets.QGroupBox(self._splitter)
+        self._tail.setTitle("")
+        self._tail.setObjectName("Tail")
+        self.gridLayout.addWidget(self._splitter, 0, 0, 1, 1)
+        self.retranslateUi(Form)
+        QtCore.QMetaObject.connectSlotsByName(Form)
+
+    def retranslateUi(self, Form):
+        _translate = QtCore.QCoreApplication.translate
+        Form.setWindowTitle(_translate("QRangeSlider", "QRangeSlider"))
+
+
+class Element(QtWidgets.QGroupBox):
+    def __init__(self, parent, main):
+        super(Element, self).__init__(parent)
         self.main = main
-        menu(self)
-        self.enable()
-
-    def addMenu(self, menu):
-        super().addMenu(menu)
-        self._menus.append(menu)
-        
-    def menu(self, label = "Menu"):
-        """
-        Creates a top level menu in the menuBar.
-        """
-        return Menu(self, label)
-
-    def enable(self):
-        """
-        Refreshes the enabled status of each menu item.
-        """
-        for menu in self._menus:
-            menu.enable()
-
-
-class Menu(QMenu):
-
-    def __init__(self, parent, title='Menu'):
-        super().__init__()
-
-        self._actions = []
-        self._menus = []
-        self.setTitle(title)
-        self.main = parent.main
-        if parent is not None:
-            parent.addMenu(self)
-
-    def addMenu(self, menu):
-        super().addMenu(menu)
-        self._menus.append(menu)
-
-    def menu(self, title='Submenu'):
-        return Menu(self, title)
-
-    def action(self, action, **kwargs):
-        #return action(self, **kwargs)
-        action = action(self, **kwargs)
-        self.addAction(action)
-        self._actions.append(action)
-        return action
-        
-    def separator(self):
-        self.addSeparator() 
-
-    def enable(self):
-        """
-        Refreshes the enabled status of each menu item.
-        """
-        for submenu in self._menus:
-            submenu.enable()
-        for action in self._actions:
-            enable = action.enable(action.main)
-            action.setEnabled(enable)
-
-
-class Action(QAction):
-    """Base class for all wezel actions"""
-
-    def __init__(self, parent,
-        text = None,
-        shortcut = None,
-        tooltip = None, 
-        icon = None,  
-        **kwargs):
-        """parent: App, Menu or MenuBar"""
-        super().__init__()
-
-        self.main = parent.main
-        # parent.addAction(self)
-        # parent._actions.append(self)
-
-        # if hasattr(parent, 'main'):
-        #     self.main = parent.main
-        #     parent.addAction(self)
-        #     parent._actions.append(self)
-        # else:
-        #     self.main = parent
-        if text is None:
-            text = self.__class__.__name__
-        self.setText(text)
-        self.triggered.connect(lambda: self.run(self.main))
-    
-        if icon is not None: 
-            self.setIcon(QIcon(icon))
-        if shortcut is not None: 
-            self.setShortcut(shortcut)
-        if tooltip is not None: 
-            self.setToolTip(tooltip)
-
-        # Dictionary with optional settings
-        for option in kwargs:
-            self.__dict__[option] = kwargs[option]
-
-    def enable(self, app):
-        return True
-
-    def run(self, app):
-        pass
-
 
+    def setStyleSheet(self, style):
+        self.parent().setStyleSheet(style)
 
+    def textColor(self):
+        return getattr(self, '__textColor', QtGui.QColor(125, 125, 125))
 
-
-
-def logger():
-    
-    LOG_FILE_NAME = "wezel_log.log"
-    # creates some sort of conflict with mdreg - commenting out for now
-#    if os.path.exists(LOG_FILE_NAME):
-#        os.remove(LOG_FILE_NAME)
-    LOG_FORMAT = "%(levelname)s %(asctime)s - %(message)s"
-    logging.basicConfig(
-        filename = LOG_FILE_NAME, 
-        level = logging.INFO, 
-        format = LOG_FORMAT)
-    return logging.getLogger(__name__)
-
-
+    def setTextColor(self, color):
+        if type(color) == tuple and len(color) == 3:
+            color = QtGui.QColor(color[0], color[1], color[2])
+        elif type(color) == int:
+            color = QtGui.QColor(color, color, color)
+        setattr(self, '__textColor', color)
+
+    def paintEvent(self, event):
+        qp = QtGui.QPainter()
+        qp.begin(self)
+        if self.main.drawValues():
+            self.drawText(event, qp)
+        qp.end()
+
+
+class Head(Element):
+    def __init__(self, parent, main):
+        super(Head, self).__init__(parent, main)
+
+    def drawText(self, event, qp):
+        qp.setPen(self.textColor())
+        qp.setFont(QtGui.QFont('Arial', 10))
+        qp.drawText(event.rect(), QtCore.Qt.AlignLeft, str(self.main.min()))
+
+
+class Tail(Element):
+    def __init__(self, parent, main):
+        super(Tail, self).__init__(parent, main)
+
+    def drawText(self, event, qp):
+        qp.setPen(self.textColor())
+        qp.setFont(QtGui.QFont('Arial', 10))
+        qp.drawText(event.rect(), QtCore.Qt.AlignRight, str(self.main.max()))
+
+
+class Handle(Element):
+    def __init__(self, parent, main):
+        super(Handle, self).__init__(parent, main)
+
+    def drawText(self, event, qp):
+        qp.setPen(self.textColor())
+        qp.setFont(QtGui.QFont('Arial', 10))
+        qp.drawText(event.rect(), QtCore.Qt.AlignLeft, str(self.main.start()))
+        qp.drawText(event.rect(), QtCore.Qt.AlignRight, str(self.main.end()))
+
+    def mouseMoveEvent(self, event):
+        event.accept()
+        mx = event.globalX()
+        _mx = getattr(self, '__mx', None)
+        if not _mx:
+            setattr(self, '__mx', mx)
+            dx = 0
+        else:
+            dx = mx - _mx
+        setattr(self, '__mx', mx)
+        if dx == 0:
+            event.ignore()
+            return
+        elif dx > 0:
+            dx = 1
+        elif dx < 0:
+            dx = -1
+        s = self.main.start() + dx
+        e = self.main.end() + dx
+        if s >= self.main.min() and e <= self.main.max():
+            self.main.setRange(s, e)
+
+
+class QRangeSlider(QtWidgets.QWidget, Ui_Form):
+    endValueChanged = QtCore.Signal(int)
+    maxValueChanged = QtCore.Signal(int)
+    minValueChanged = QtCore.Signal(int)
+    startValueChanged = QtCore.Signal(int)
+    minValueChanged = QtCore.Signal(int)
+    maxValueChanged = QtCore.Signal(int)
+    startValueChanged = QtCore.Signal(int)
+    endValueChanged = QtCore.Signal(int)
+
+    _SPLIT_START = 1
+    _SPLIT_END = 2
+
+    def __init__(self, parent=None):
+        super(QRangeSlider, self).__init__(parent)
+        self.setupUi(self)
+        self.setMouseTracking(False)
+        self._splitter.splitterMoved.connect(self._handleMoveSplitter)
+        self._head_layout = QtWidgets.QHBoxLayout()
+        self._head_layout.setSpacing(0)
+        self._head_layout.setContentsMargins(0, 0, 0, 0)
+        self._head.setLayout(self._head_layout)
+        self.head = Head(self._head, main=self)
+        self._head_layout.addWidget(self.head)
+        self._handle_layout = QtWidgets.QHBoxLayout()
+        self._handle_layout.setSpacing(0)
+        self._handle_layout.setContentsMargins(0, 0, 0, 0)
+        self._handle.setLayout(self._handle_layout)
+        self.handle = Handle(self._handle, main=self)
+        self.handle.setTextColor((150, 255, 150))
+        self._handle_layout.addWidget(self.handle)
+        self._tail_layout = QtWidgets.QHBoxLayout()
+        self._tail_layout.setSpacing(0)
+        self._tail_layout.setContentsMargins(0, 0, 0, 0)
+        self._tail.setLayout(self._tail_layout)
+        self.tail = Tail(self._tail, main=self)
+        self._tail_layout.addWidget(self.tail)
+        self.setMin(0)
+        self.setMax(99)
+        self.setStart(0)
+        self.setEnd(99)
+        self.setDrawValues(True)
+
+    def min(self):
+        return getattr(self, '__min', None)
+
+    def max(self):
+        return getattr(self, '__max', None)
+
+    def setMin(self, value):
+        setattr(self, '__min', value)
+        self.minValueChanged.emit(value)
+
+    def setMax(self, value):
+        setattr(self, '__max', value)
+        self.maxValueChanged.emit(value)
+
+    def start(self):
+        return getattr(self, '__start', None)
+
+    def end(self):
+        return getattr(self, '__end', None)
+
+    def _setStart(self, value):
+        setattr(self, '__start', value)
+        self.startValueChanged.emit(value)
+
+    def setStart(self, value):
+        v = self._valueToPos(value)
+        self._splitter.splitterMoved.disconnect()
+        self._splitter.moveSplitter(v, self._SPLIT_START)
+        self._splitter.splitterMoved.connect(self._handleMoveSplitter)
+        self._setStart(value)
+
+    def _setEnd(self, value):
+        setattr(self, '__end', value)
+        self.endValueChanged.emit(value)
+
+    def setEnd(self, value):
+        v = self._valueToPos(value)
+        self._splitter.splitterMoved.disconnect()
+        self._splitter.moveSplitter(v, self._SPLIT_END)
+        self._splitter.splitterMoved.connect(self._handleMoveSplitter)
+        self._setEnd(value)
+
+    def drawValues(self):
+        return getattr(self, '__drawValues', None)
+
+    def setDrawValues(self, draw):
+        setattr(self, '__drawValues', draw)
+
+    def getRange(self):
+        return (self.start(), self.end())
+
+    def setRange(self, start, end):
+        self.setStart(start)
+        self.setEnd(end)
+
+    def keyPressEvent(self, event):
+        key = event.key()
+        if key == QtCore.Qt.Key_Left:
+            s = self.start()-1
+            e = self.end()-1
+        elif key == QtCore.Qt.Key_Right:
+            s = self.start()+1
+            e = self.end()+1
+        else:
+            event.ignore()
+            return
+        event.accept()
+        if s >= self.min() and e <= self.max():
+            self.setRange(s, e)
+
+    def setBackgroundStyle(self, style):
+        self._tail.setStyleSheet(style)
+        self._head.setStyleSheet(style)
+
+    def setSpanStyle(self, style):
+        self._handle.setStyleSheet(style)
+
+    def _valueToPos(self, value):
+        return scale(value, (self.min(), self.max()), (0, self.width()))
+
+    def _posToValue(self, xpos):
+        return scale(xpos, (0, self.width()), (self.min(), self.max()))
+
+    def _handleMoveSplitter(self, xpos, index):
+        hw = self._splitter.handleWidth()
+        def _lockWidth(widget):
+            width = widget.size().width()
+            widget.setMinimumWidth(width)
+            widget.setMaximumWidth(width)
+        def _unlockWidth(widget):
+            widget.setMinimumWidth(0)
+            widget.setMaximumWidth(16777215)
+        v = self._posToValue(xpos)
+        if index == self._SPLIT_START:
+            _lockWidth(self._tail)
+            if v >= self.end():
+                return
+            offset = -20
+            w = xpos + offset
+            self._setStart(v)
+        elif index == self._SPLIT_END:
+            _lockWidth(self._head)
+            if v <= self.start():
+                return
+            offset = -40
+            w = self.width() - xpos + offset
+            self._setEnd(v)
+        _unlockWidth(self._tail)
+        _unlockWidth(self._head)
+        _unlockWidth(self._handle)
+
+if __name__ == '__main__':
+
+    app = QtWidgets.QApplication(sys.argv)
+    rs = QRangeSlider()
+    rs.show()
+    rs.setRange(15, 35)
+    rs.setBackgroundStyle('background: qlineargradient(x1:0, y1:0, x2:0, y2:1, stop:0 #222, stop:1 #333);')
+    rs.handle.setStyleSheet('background: qlineargradient(x1:0, y1:0, x2:0, y2:1, stop:0 #282, stop:1 #393);')
+    app.exec_()
```

### Comparing `wezel-0.1.1/src/wezel/icons/fugue_icons/application-import.png` & `wezel-0.1.2/src/wezel/icons/fugue_icons/application-import.png`

 * *Files identical despite different names*

### Comparing `wezel-0.1.1/src/wezel/icons/fugue_icons/arrow-curve-180-left.png` & `wezel-0.1.2/src/wezel/icons/fugue_icons/arrow-curve-180-left.png`

 * *Files identical despite different names*

### Comparing `wezel-0.1.1/src/wezel/icons/fugue_icons/arrow-curve.png` & `wezel-0.1.2/src/wezel/icons/fugue_icons/arrow-curve.png`

 * *Files identical despite different names*

### Comparing `wezel-0.1.1/src/wezel/icons/fugue_icons/arrow-in.png` & `wezel-0.1.2/src/wezel/icons/fugue_icons/arrow-in.png`

 * *Files identical despite different names*

### Comparing `wezel-0.1.1/src/wezel/icons/fugue_icons/arrow-move.png` & `wezel-0.1.2/src/wezel/icons/fugue_icons/arrow-move.png`

 * *Files identical despite different names*

### Comparing `wezel-0.1.1/src/wezel/icons/fugue_icons/arrow-out.png` & `wezel-0.1.2/src/wezel/icons/fugue_icons/arrow-out.png`

 * *Files identical despite different names*

### Comparing `wezel-0.1.1/src/wezel/icons/fugue_icons/bin-metal.png` & `wezel-0.1.2/src/wezel/icons/fugue_icons/bin-metal.png`

 * *Files identical despite different names*

### Comparing `wezel-0.1.1/src/wezel/icons/fugue_icons/blue-document-export.png` & `wezel-0.1.2/src/wezel/icons/fugue_icons/blue-document-export.png`

 * *Files identical despite different names*

### Comparing `wezel-0.1.1/src/wezel/icons/fugue_icons/brightness.png` & `wezel-0.1.2/src/wezel/icons/fugue_icons/brightness.png`

 * *Files identical despite different names*

### Comparing `wezel-0.1.1/src/wezel/icons/fugue_icons/color--arrow.png` & `wezel-0.1.2/src/wezel/icons/fugue_icons/color--arrow.png`

 * *Files identical despite different names*

### Comparing `wezel-0.1.1/src/wezel/icons/fugue_icons/color.png` & `wezel-0.1.2/src/wezel/icons/fugue_icons/color.png`

 * *Files identical despite different names*

### Comparing `wezel-0.1.1/src/wezel/icons/fugue_icons/contrast-low.png` & `wezel-0.1.2/src/wezel/icons/fugue_icons/contrast-low.png`

 * *Files identical despite different names*

### Comparing `wezel-0.1.1/src/wezel/icons/fugue_icons/contrast.png` & `wezel-0.1.2/src/wezel/icons/fugue_icons/contrast.png`

 * *Files identical despite different names*

### Comparing `wezel-0.1.1/src/wezel/icons/fugue_icons/controller-d-pad.png` & `wezel-0.1.2/src/wezel/icons/fugue_icons/controller-d-pad.png`

 * *Files identical despite different names*

### Comparing `wezel-0.1.1/src/wezel/icons/fugue_icons/cross-script.png` & `wezel-0.1.2/src/wezel/icons/fugue_icons/cross-script.png`

 * *Files identical despite different names*

### Comparing `wezel-0.1.1/src/wezel/icons/fugue_icons/cursor.png` & `wezel-0.1.2/src/wezel/icons/fugue_icons/cursor.png`

 * *Files identical despite different names*

### Comparing `wezel-0.1.1/src/wezel/icons/fugue_icons/cutter.png` & `wezel-0.1.2/src/wezel/icons/fugue_icons/cutter.png`

 * *Files identical despite different names*

### Comparing `wezel-0.1.1/src/wezel/icons/fugue_icons/eraser--arrow.png` & `wezel-0.1.2/src/wezel/icons/fugue_icons/eraser--arrow.png`

 * *Files identical despite different names*

### Comparing `wezel-0.1.1/src/wezel/icons/fugue_icons/eraser--plus.png` & `wezel-0.1.2/src/wezel/icons/fugue_icons/eraser--plus.png`

 * *Files identical despite different names*

### Comparing `wezel-0.1.1/src/wezel/icons/fugue_icons/eraser.png` & `wezel-0.1.2/src/wezel/icons/fugue_icons/eraser.png`

 * *Files identical despite different names*

### Comparing `wezel-0.1.1/src/wezel/icons/fugue_icons/hand-finger.png` & `wezel-0.1.2/src/wezel/icons/fugue_icons/hand-finger.png`

 * *Files identical despite different names*

### Comparing `wezel-0.1.1/src/wezel/icons/fugue_icons/hand-point-090.png` & `wezel-0.1.2/src/wezel/icons/fugue_icons/hand-point-090.png`

 * *Files identical despite different names*

### Comparing `wezel-0.1.1/src/wezel/icons/fugue_icons/hand.png` & `wezel-0.1.2/src/wezel/icons/fugue_icons/hand.png`

 * *Files identical despite different names*

### Comparing `wezel-0.1.1/src/wezel/icons/fugue_icons/layer-select.png` & `wezel-0.1.2/src/wezel/icons/fugue_icons/layer-select.png`

 * *Files identical despite different names*

### Comparing `wezel-0.1.1/src/wezel/icons/fugue_icons/layer-shape-curve.png` & `wezel-0.1.2/src/wezel/icons/fugue_icons/layer-shape-curve.png`

 * *Files identical despite different names*

### Comparing `wezel-0.1.1/src/wezel/icons/fugue_icons/layer-shape-ellipse.png` & `wezel-0.1.2/src/wezel/icons/fugue_icons/layer-shape-ellipse.png`

 * *Files identical despite different names*

### Comparing `wezel-0.1.1/src/wezel/icons/fugue_icons/layer-shape-polygon.png` & `wezel-0.1.2/src/wezel/icons/fugue_icons/layer-shape-polygon.png`

 * *Files identical despite different names*

### Comparing `wezel-0.1.1/src/wezel/icons/fugue_icons/layer-shape-round.png` & `wezel-0.1.2/src/wezel/icons/fugue_icons/layer-shape-round.png`

 * *Files identical despite different names*

### Comparing `wezel-0.1.1/src/wezel/icons/fugue_icons/layer-transparent.png` & `wezel-0.1.2/src/wezel/icons/fugue_icons/layer-transparent.png`

 * *Files identical despite different names*

### Comparing `wezel-0.1.1/src/wezel/icons/fugue_icons/lifebuoy.png` & `wezel-0.1.2/src/wezel/icons/fugue_icons/lifebuoy.png`

 * *Files identical despite different names*

### Comparing `wezel-0.1.1/src/wezel/icons/fugue_icons/lock-unlock.png` & `wezel-0.1.2/src/wezel/icons/fugue_icons/lock-unlock.png`

 * *Files identical despite different names*

### Comparing `wezel-0.1.1/src/wezel/icons/fugue_icons/lock.png` & `wezel-0.1.2/src/wezel/icons/fugue_icons/lock.png`

 * *Files identical despite different names*

### Comparing `wezel-0.1.1/src/wezel/icons/fugue_icons/magnifier-zoom-actual.png` & `wezel-0.1.2/src/wezel/icons/fugue_icons/magnifier-zoom-actual.png`

 * *Files identical despite different names*

### Comparing `wezel-0.1.1/src/wezel/icons/fugue_icons/magnifier-zoom-fit.png` & `wezel-0.1.2/src/wezel/icons/fugue_icons/magnifier-zoom-fit.png`

 * *Files identical despite different names*

### Comparing `wezel-0.1.1/src/wezel/icons/fugue_icons/magnifier-zoom-in.png` & `wezel-0.1.2/src/wezel/icons/fugue_icons/magnifier-zoom-in.png`

 * *Files identical despite different names*

### Comparing `wezel-0.1.1/src/wezel/icons/fugue_icons/magnifier-zoom-out.png` & `wezel-0.1.2/src/wezel/icons/fugue_icons/magnifier-zoom-out.png`

 * *Files identical despite different names*

### Comparing `wezel-0.1.1/src/wezel/icons/fugue_icons/magnifier.png` & `wezel-0.1.2/src/wezel/icons/fugue_icons/magnifier.png`

 * *Files identical despite different names*

### Comparing `wezel-0.1.1/src/wezel/icons/fugue_icons/paint-brush--arrow.png` & `wezel-0.1.2/src/wezel/icons/fugue_icons/paint-brush--arrow.png`

 * *Files identical despite different names*

### Comparing `wezel-0.1.1/src/wezel/icons/fugue_icons/paint-brush--minus.png` & `wezel-0.1.2/src/wezel/icons/fugue_icons/paint-brush--minus.png`

 * *Files identical despite different names*

### Comparing `wezel-0.1.1/src/wezel/icons/fugue_icons/paint-brush--plus.png` & `wezel-0.1.2/src/wezel/icons/fugue_icons/paint-brush--plus.png`

 * *Files identical despite different names*

### Comparing `wezel-0.1.1/src/wezel/icons/fugue_icons/paint-brush.png` & `wezel-0.1.2/src/wezel/icons/fugue_icons/paint-brush.png`

 * *Files identical despite different names*

### Comparing `wezel-0.1.1/src/wezel/icons/fugue_icons/paint-can--minus.png` & `wezel-0.1.2/src/wezel/icons/fugue_icons/paint-can--minus.png`

 * *Files identical despite different names*

### Comparing `wezel-0.1.1/src/wezel/icons/fugue_icons/paint-can--plus.png` & `wezel-0.1.2/src/wezel/icons/fugue_icons/paint-can--plus.png`

 * *Files identical despite different names*

### Comparing `wezel-0.1.1/src/wezel/icons/fugue_icons/paint.png` & `wezel-0.1.2/src/wezel/icons/fugue_icons/paint.png`

 * *Files identical despite different names*

### Comparing `wezel-0.1.1/src/wezel/icons/fugue_icons/pencil.png` & `wezel-0.1.2/src/wezel/icons/fugue_icons/pencil.png`

 * *Files identical despite different names*

### Comparing `wezel-0.1.1/src/wezel/icons/fugue_icons/plus.png` & `wezel-0.1.2/src/wezel/icons/fugue_icons/plus.png`

 * *Files identical despite different names*

### Comparing `wezel-0.1.1/src/wezel/icons/fugue_icons/spectrum.png` & `wezel-0.1.2/src/wezel/icons/fugue_icons/spectrum.png`

 * *Files identical despite different names*

### Comparing `wezel-0.1.1/src/wezel/icons/fugue_icons/tick-button.png` & `wezel-0.1.2/src/wezel/icons/fugue_icons/tick-button.png`

 * *Files identical despite different names*

### Comparing `wezel-0.1.1/src/wezel/icons/fugue_icons/wand-hat.png` & `wezel-0.1.2/src/wezel/icons/fugue_icons/wand-hat.png`

 * *Files identical despite different names*

### Comparing `wezel-0.1.1/src/wezel/icons/fugue_icons/wand.png` & `wezel-0.1.2/src/wezel/icons/fugue_icons/wand.png`

 * *Files identical despite different names*

### Comparing `wezel-0.1.1/src/wezel/icons/images/wezel.jpg` & `wezel-0.1.2/src/wezel/icons/images/wezel.jpg`

 * *Files identical despite different names*

### Comparing `wezel-0.1.1/src/wezel/icons/inventory.py` & `wezel-0.1.2/src/wezel/icons/inventory.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,29 +1,36 @@
 __all__ = [
     'favicon',
     'slider_icon', 
+    'animal_dog',
+    'bug',
     'application_import',
     'arrow_curve_180_left',
     'arrow_curve',
     'arrow_in',
     'arrow_move',
     'arrow_out',
     'arrow_resize_090',
+    'arrow_stop_090',
+    'arrow_stop_270',
     'bin_metal',
     'blue_document_export',
     'brightness',
+    'clipboard__plus',
     'color',
     'color__arrow',
     'contrast',
     'contrast_low',
     'controller_d_pad',
     'cross_script',
     'cursor',
     'cutter',
     'disk',
+    'document_excel',
+    'document_excel_csv',
     'eraser',
     'eraser__arrow',
     'eraser__plus',
     'hand',
     'hand_finger',
     'hand_point_090',
     'layer_select', 
@@ -38,28 +45,33 @@
     'lock_unlock',
     'magnifier',
     'magnifier_zoom_actual',
     'magnifier_zoom_fit',
     'magnifier_zoom_in',
     'magnifier_zoom_out',
     'minus',
+    'minus_small_circle',
+    'minus_small_white',
     'paint',
     'paint_brush',
     'paint_brush__arrow',
     'paint_brush__minus',
     'paint_brush__plus',
     'paint_can__minus',
     'paint_can__plus',
     'pencil',
     'plus',
+    'plus_small_white',
     'question_mark',
     'spectrum',
     'wand',
     'wand_hat',
     'wezel', 
+    'wezel_icon',
+    'wezel_icon_transparent',
 ]
 
 # filepaths need to be identified with importlib_resources
 # rather than __file__ as the latter does not work at runtime 
 # when the package is installed via pip install
 
 import sys
@@ -78,36 +90,45 @@
 wezel = str(f.joinpath('wezel.jpg'))
 
 f = importlib_resources.files('wezel.icons.my_icons')
 
 favicon = str(f.joinpath('favicon.ico'))
 slider_icon = str(f.joinpath('slider_icon.png'))
 question_mark = str(f.joinpath('question-mark.png'))
+wezel_icon = str(f.joinpath('wezel-icon.png'))
+wezel_icon_transparent = str(f.joinpath('wezel-icon-transparent.png'))
 
 f = importlib_resources.files('wezel.icons.fugue_icons')
 
+animal_dog = str(f.joinpath('animal-dog.png'))
+bug = str(f.joinpath('bug.png'))
 application_import = str(f.joinpath('application-import.png'))
 arrow_curve = str(f.joinpath('arrow-curve.png'))
 arrow_curve_180_left = str(f.joinpath('arrow-curve-180-left.png'))
 arrow_in = str(f.joinpath('arrow-in.png'))
 arrow_move = str(f.joinpath('arrow-move.png'))
 arrow_out = str(f.joinpath('arrow-out.png'))
 arrow_resize_090 = str(f.joinpath('arrow-resize-090.png'))
+arrow_stop_090 = str(f.joinpath('arrow-stop-090.png'))
+arrow_stop_270 = str(f.joinpath('arrow-stop-270.png'))
 bin_metal = str(f.joinpath('bin-metal.png'))
 blue_document_export = str(f.joinpath('blue-document-export.png'))
 brightness = str(f.joinpath('brightness.png'))
+clipboard__plus = str(f.joinpath('clipboard--plus.png'))
 color = str(f.joinpath('color.png'))
 color__arrow = str(f.joinpath('color--arrow.png'))
 contrast = str(f.joinpath('contrast.png'))
 contrast_low = str(f.joinpath('contrast-low.png'))
 controller_d_pad = str(f.joinpath('controller-d-pad.png'))
 cross_script = str(f.joinpath('cross-script.png'))
 cursor = str(f.joinpath('cursor.png'))
 cutter = str(f.joinpath('cutter.png'))
 disk = str(f.joinpath('disk.png'))
+document_excel = str(f.joinpath('document-excel.png'))
+document_excel_csv = str(f.joinpath('document-excel-csv.png'))
 eraser = str(f.joinpath('eraser.png'))
 eraser__plus = str(f.joinpath('eraser--plus.png'))
 eraser__arrow = str(f.joinpath('eraser--arrow.png'))
 hand = str(f.joinpath('hand.png'))
 hand_finger = str(f.joinpath('hand-finger.png'))
 hand_point_090 = str(f.joinpath('hand-point-090.png'))
 layer_select = str(f.joinpath('layer-select.png'))
@@ -122,19 +143,22 @@
 lock_unlock = str(f.joinpath('lock-unlock.png'))
 magnifier = str(f.joinpath('magnifier.png'))
 magnifier_zoom_actual = str(f.joinpath('magnifier-zoom-actual.png'))
 magnifier_zoom_in = str(f.joinpath('magnifier-zoom-in.png'))
 magnifier_zoom_out = str(f.joinpath('magnifier-zoom-out.png'))
 magnifier_zoom_fit = str(f.joinpath('magnifier-zoom-fit.png'))
 minus = str(f.joinpath('minus.png'))
+minus_small_circle = str(f.joinpath('minus-small-circle.png'))
+minus_small_white = str(f.joinpath('minus-small-white.png'))
 paint = str(f.joinpath('paint.png'))
 paint_can__minus = str(f.joinpath('paint-can--minus.png'))
 paint_can__plus = str(f.joinpath('paint-can--plus.png'))
 paint_brush = str(f.joinpath('paint-brush.png'))
 paint_brush__arrow = str(f.joinpath('paint-brush--arrow.png'))
 paint_brush__minus = str(f.joinpath('paint-brush--minus.png'))
 paint_brush__plus = str(f.joinpath('paint-brush--plus.png'))
 pencil = str(f.joinpath('pencil.png'))
 plus = str(f.joinpath('plus.png'))
+plus_small_white = str(f.joinpath('plus-small-white.png'))
 spectrum = str(f.joinpath('spectrum.png'))
 wand = str(f.joinpath('wand.png'))
 wand_hat = str(f.joinpath('wand-hat.png'))
```

### Comparing `wezel-0.1.1/src/wezel/icons/my_icons/favicon.ico` & `wezel-0.1.2/src/wezel/icons/my_icons/favicon.ico`

 * *Files identical despite different names*

### Comparing `wezel-0.1.1/src/wezel/icons/my_icons/question-mark.png` & `wezel-0.1.2/src/wezel/icons/my_icons/question-mark.png`

 * *Files identical despite different names*

### Comparing `wezel-0.1.1/src/wezel/icons/my_icons/slider_icon.png` & `wezel-0.1.2/src/wezel/icons/my_icons/slider_icon.png`

 * *Files identical despite different names*

### Comparing `wezel-0.1.1/src/wezel/widgets/__init__.py` & `wezel-0.1.2/src/wezel/widgets/__init__.py`

 * *Files 24% similar despite different names*

```diff
@@ -4,24 +4,18 @@
 
 """
 
 #from .log_to_GUI import *
 
 from .dbimage import (
     ImageWindow,
-    ImageBrightness, 
-    ImageContrast,
 )
 from .series_sliders import (
     SeriesSliders,
 )
-from .series_display import (
-    SeriesDisplay,
-    SeriesDisplay4D,
-)
 from .plot_curve import (
     PlotCurve,
 )
 from .qrangeslider import (
     QRangeSlider,
 )
 from .sliders import (
@@ -31,21 +25,20 @@
 )
 from .main_mdi import (
     MainMultipleDocumentInterface, 
 )
 from .message import (
     Dialog, 
     StatusBar,
+)
+from .user_input import (
     UserInput,
 )
 from .dbdatabase import (
     DICOMFolderTree,
 )
 from .region_list import (
     RegionList,
 )
 from .file_display import (
     ImageLabel,
-)
-from .dicom_header import (
-    SeriesViewerMetaData,
 )
```

### Comparing `wezel-0.1.1/src/wezel/widgets/dbdatabase.py` & `wezel-0.1.2/src/wezel/widgets/dbdatabase.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,43 +1,47 @@
-from PyQt5.QtCore import  Qt, pyqtSignal
-from PyQt5.QtWidgets import (
+from PySide2.QtCore import  Qt, Signal
+from PySide2.QtWidgets import (
     QAbstractItemView,
     QTreeWidget, QTreeWidgetItem, QFileSystemModel, QTreeView,
 )
 
 class DICOMFolderTree(QTreeWidget):
     """Displays a DICOM folder as a Tree."""
 
-    itemSelectionChanged = pyqtSignal(dict)
-    itemDoubleClicked = pyqtSignal(dict)
-    databaseSet = pyqtSignal()
+    itemSelectionChanged = Signal(dict)
+    itemDoubleClicked = Signal(dict)
+    databaseSet = Signal()
 
     def __init__(self, folder):
         super().__init__()
 
         self.setSelectionMode(QAbstractItemView.ExtendedSelection)
         self.itemDoubleClicked.connect(lambda item, col: self._itemDoubleClickedEvent(item, col))
         self.itemClicked.connect(lambda item, col: self._itemClickedEvent(item, col))
         # self.setModel(QFileSystemModel()) #This only works for QTreeView
-        self.setFolder(folder)
+        self._database = None
+        self.setDatabase(folder)
 
-    def setFolder(self, folder=None):
+    def database(self):
+        return self._database
+
+    def setDatabase(self, folder=None):
         if folder is not None: 
-            self.database=folder
+            self._database=folder
         self.dict = {
-            'label': self.database.manager.path,
+            'label': self._database.manager.path,
             'level': 'Database',
             'uid': 'Database',
             'key': None,
         }
         self.setUpdatesEnabled(False)
         self.clear()
-        self.setHeaderLabels([self.database.manager.path])
+        self.setHeaderLabels([self._database.manager.path])
         # This does not show empty patients or studies
-        database = self.database.manager.tree()
+        database = self._database.manager.tree()
         for patient in database['patients']:
             patientWidget = self._treeWidgetItem('Patient', patient, self)
             for study in patient['studies']:
                 studyWidget = self._treeWidgetItem('Study', study, patientWidget)
                 for sery in study['series']:
                     seriesWidget = self._treeWidgetItem('Series', sery, studyWidget)
         self.setUpdatesEnabled(True)
@@ -47,15 +51,15 @@
     def _treeWidgetItem(self, level, record, parent, expanded=True):
         """Build an item in the Tree"""
 
         item = QTreeWidgetItem(parent)
         # Custom attributes
         item.checked = False
         item.dict = {
-            'label': self.database.manager.label(key=record['key'], type=level),
+            'label': self._database.manager.label(key=record['key'], type=level),
             'level': level,
             'uid': record['uid'],
             'key': record['key'],
         }
         # Built-in attributes
         item.setText(0, item.dict['label'])
         item.setFlags(Qt.ItemIsEnabled | Qt.ItemIsSelectable | Qt.ItemIsUserCheckable)
@@ -124,15 +128,18 @@
             for gen in [1,2,3]:
                 records += self.get_selected(gen)
             return records
         items = _children([root])
         while generation > 1:
             items = _children(items)
             generation -= 1
-        return [self.database.record(i.dict['level'], i.dict['uid']) for i in items if i.checkState(0)==Qt.Checked]
+        return [
+            self._database.record(i.dict['level'], i.dict['uid']) 
+            for i in items if i.checkState(0) == Qt.Checked
+        ]
 
     def selected(self, generation):
         if isinstance(generation, str):
             if generation == 'Patients':
                 generation=1
             elif generation == 'Studies':
                 generation=2
```

### Comparing `wezel-0.1.1/src/wezel/widgets/dbimage.py` & `wezel-0.1.2/src/wezel/displays/series_display_4d.py`

 * *Files 27% similar despite different names*

```diff
@@ -1,325 +1,250 @@
-import timeit
 import numpy as np
-from PyQt5.QtCore import pyqtSignal, Qt
-from PyQt5.QtWidgets import (QToolBar,
-    QAction, QComboBox, QPushButton, QLabel, 
-    QWidget, QDoubleSpinBox, QHBoxLayout, QVBoxLayout)
-from PyQt5.QtGui import QIcon, QPixmap
-
-from wezel import widgets, icons
-
-listColors =  ['gray', 'cividis',  'magma', 'plasma', 'viridis', 
-    'Greys', 'Purples', 'Blues', 'Greens', 'Oranges', 'Reds',
-    'YlOrBr', 'YlOrRd', 'OrRd', 'PuRd', 'RdPu', 'BuPu',
-    'GnBu', 'PuBu', 'YlGnBu', 'PuBuGn', 'BuGn', 'YlGn',
-    'binary', 'gist_yarg', 'gist_gray', 'bone', 'pink',
-    'spring', 'summer', 'autumn', 'winter', 'cool', 'Wistia',
-    'hot', 'afmhot', 'gist_heat', 'copper',
-    'PiYG', 'PRGn', 'BrBG', 'PuOr', 'RdGy', 'RdBu',
-    'RdYlBu', 'RdYlGn', 'Spectral', 'coolwarm', 'bwr', 'seismic',
-    'twilight', 'twilight_shifted', 'hsv',
-    'flag', 'prism', 'ocean', 'gist_earth', 'terrain', 'gist_stern',
-    'gnuplot', 'gnuplot2', 'CMRmap', 'cubehelix', 'brg', 'turbo',
-    'gist_rainbow', 'rainbow', 'jet', 'nipy_spectral', 'gist_ncar']
-
-QComboBoxStyleSheet = """
-
-QComboBox::drop-down 
-{
-    border: 0px; /* This seems to replace the whole arrow of the combo box */
-}
-QComboBox:down-arrow 
-{
-    image: url("icons/fugue_icons/spectrum.png");
-    width: 14px;
-    height: 14px;
-}
-"""
 
-
-class ImageWindow(QWidget):
-    """Widget to set and manage color and window settings of a Series"""
-
-    valueChanged = pyqtSignal(list)  # emitted when the color settings are changed by the widget
-
-    def __init__(self, layout=True):
-        super().__init__()
-        self._setWidgets(layout)
-        self._setConnections()
-        if layout:
-            self._setLayout()
-
-    def _setWidgets(self, layout):
-        self.mode = LockUnlockWidget(toolTip = 'Lock image settings')
-        self.brightness = ImageBrightness(layout=layout)
-        self.contrast = ImageContrast(layout=layout)
-
-    def _setConnections(self):
-        self.brightness.valueChanged.connect(self._valueChanged)
-        self.contrast.valueChanged.connect(self._valueChanged)
-
-    def _setLayout(self):
-        layout = QVBoxLayout()
-        layout.setContentsMargins(0,0,0,0)
-        layout.setSpacing(0)
-        #layout.addWidget(self.mode)
-        layout.addWidget(self.brightness)
-        layout.addWidget(self.contrast)
-        #self.setStyleSheet("background-color: white")
-        self.setLayout(layout)
-
-    def _valueChanged(self):
-        self.valueChanged.emit(self.getValue())
-
-    def setData(self, array, center, width, set=None):
-        min = np.amin(array)
-        max = np.amax(array)
-        if set is None:
-            set = not self.mode.isLocked
-        self.brightness.setData(min, max, center, set)
-        self.contrast.setData(min, max, width, set)
-
-    def getValue(self):
-        return [
-            self.brightness.getValue(),
-            self.contrast.getValue(),
-        ]
-
-    def setValue(self, WindowCenter=None, WindowWidth=None):
-        self.brightness.setValue(WindowCenter)
-        self.contrast.setValue(WindowWidth)
-
-
-class ImageContrast(QWidget):
-
-    valueChanged = pyqtSignal(float)
-
-    def __init__(self, layout=True):
-        super().__init__()
-
-        self.label = QLabel()
-        self.label.setPixmap(QPixmap(icons.contrast))
-        #self.label.setFixedSize(24, 24)
-        self.spinBox = QDoubleSpinBox()
-        self.spinBox.valueChanged.connect(self.spinBoxValueChanged)
-        self.spinBox.setToolTip("Adjust Contrast")
-        self.spinBox.setMinimum(0)
-        self.spinBox.setMaximum(1000000000.00)
-        self.spinBox.setWrapping(False)
-        self.spinBox.setFixedWidth(115)
-        if layout:
-            self.layout = QHBoxLayout()
-            self.layout.setAlignment(Qt.AlignLeft | Qt.AlignVCenter)
-            self.layout.setContentsMargins(0,0,0,0)
-            self.layout.setSpacing(2)
-            self.layout.addWidget(self.spinBox)
-            self.layout.addWidget(self.label)
-            #self.setMaximumWidth(120)
-            self.setLayout(self.layout)
-
-    def setData(self, min, max, width, set=True):
-        self.spinBox.blockSignals(True)
-        if width is None: 
-            self.spinBox.setValue(1)  
-            self.spinBox.setSingleStep(0.1)
+from PySide2.QtWidgets import (
+    QWidget, 
+    QSplitter,
+    QVBoxLayout,
+)
+
+import wezel
+from wezel import widgets, canvas
+
+
+class SeriesDisplay4D(wezel.gui.MainWidget):
+    """
+    GUI for displaying a 4D numpy array
+    """
+
+    def __init__(self): 
+        super().__init__()
+
+        self.x = None
+        self.y = None
+
+        # Toolbar
+        #self.toolBarClass = canvas.ToolBar
+        self.toolBarClass = SeriesDisplay4DToolBar
+
+        # Widgets
+        self.canvas = canvas.SeriesCanvas(self)
+        self.viewSlider = widgets.IndexSlider()
+        self.plot = widgets.PlotCurve()
+        self.plotSlider = widgets.IndexSlider()
+
+        # Connections
+        self.canvas.arrowKeyPress.connect(lambda arrow: self.arrowKeyPress(arrow))
+        self.canvas.mousePositionMoved.connect(lambda x, y: self.mouseMoved(x,y))
+        self.viewSlider.valueChanged.connect(self.imageChanged)
+        self.plotSlider.valueChanged.connect(self.plotChanged)
+
+        # Display
+        self._view = SeriesDisplay4DView(self)
+
+    def setToolBar(self, toolBar):
+        super().setToolBar(toolBar)
+        self.canvas.fitItem()
+
+    def setActive(self, active):
+        #super().setActive(active)
+        if not active:
+            self.canvas.saveMask()
+
+    def closeEvent(self, event):
+        newSeries = self.canvas._model.saveRegions()
+        if newSeries:
+            self.databaseUpdated.emit()
+
+    def imageChanged(self):
+        z = self.viewSlider.value()
+        t = self.plotSlider.value()
+        self.canvas.changeArray(
+            np.squeeze(self.array[:,:,z,t]),
+            self.uid[z,t], 
+            self.center[z,t], 
+            self.width[z,t], 
+            # self.lut[z,t], 
+            self.colormap[z,t],
+        )
+        self.setStatus()
+        self.setPlot() 
+
+    def plotChanged(self):
+        self.setStatus()
+        self.setPlot()        
+
+    def arrowKeyPress(self, arrow):
+        if arrow == 'left':
+            self.plotSlider.move('down')
+        elif arrow == 'right':
+            self.plotSlider.move('up')
+        elif arrow == 'up':
+            self.viewSlider.move('up')
+        elif arrow == 'down':
+            self.viewSlider.move('down')
+        self.imageChanged()
+
+    def mouseMoved(self, x, y):
+        self.x = x
+        self.y = y
+        self.setStatus()
+        self.setPlot()
+
+    def series(self):
+        return self.canvas._model._series
+
+    def setSeries(self, series, sortby=['SliceLocation', 'AcquisitionTime'], xoffset=True):
+        if series.instances() == []:
+            self.setError('Series ' + series.label() + ' is empty. \n\n Nothing to show here..')
+            return
+        self.canvas._model._series = series
+        array, header = series.array(sortby, pixels_first=True)
+
+        if array is None:
+            self.setError('Series ' + series.label() + ' does not have images. \n\n Nothing to show here..')
+            return
+        series.status.hide()
+        #self.series = series
+        self.array = array[...,0].reshape(array.shape[:4])
+        self.zlabel = sortby[0]
+        self.tlabel = sortby[1]
+        # create index arrays
+        # Unnecessary read of all files
+        d = self.array.shape
+        self.zcoords = np.empty((d[2],d[3]), dtype=np.float32)
+        self.tcoords = np.empty((d[2],d[3]), dtype=np.float32)
+        self.uid = np.empty((d[2],d[3]), dtype=object)
+        self.center = np.empty((d[2],d[3]))
+        self.width = np.empty((d[2],d[3]))
+        self.colormap = np.empty((d[2],d[3]), dtype=object)
+
+        variables = sortby + ['SOPInstanceUID', 'WindowCenter', 'WindowWidth', 'colormap']
+        cnt = 0
+        total = d[2]*d[3]
+        for z in range(d[2]):
+            for t in range(d[3]):
+                cnt += 1
+                series.status.progress(cnt, total, 'Reading image properties..')
+                values = header[z,t,0][variables]
+                self.zcoords[z,t] = values[0]
+                self.tcoords[z,t] = values[1]
+                self.uid[z,t] = values[2]
+                self.center[z,t] = values[3]
+                self.width[z,t] = values[4]
+                self.colormap[z,t] = values[5]
+        series.status.hide()
+        if xoffset:
+            self.tcoords -= np.amin(self.tcoords)
+        self.viewSlider.setMaximum(array.shape[2]-1)
+        self.plotSlider.setMaximum(array.shape[3]-1)
+        self.plot.setXlabel(self.tlabel)
+        self.plot.setYlabel(series.SeriesDescription)
+        self.plot.setXlim([np.amin(self.tcoords), np.amax(self.tcoords)])
+        self.plot.setYlim([np.amin(self.center-self.width/2), np.amax(self.center+self.width/2)])
+
+        self.refresh()
+
+    def refresh(self):
+        self.setStatus()
+        self.setCanvas()
+        self.setPlot()
+
+    def setStatus(self):
+        if self.x is None:
+            return
+        x = self.x
+        y = self.y
+        z = self.viewSlider.value()
+        t = self.plotSlider.value()
+        if (not (0 <= x < self.array.shape[0]) or
+            not (0 <= y < self.array.shape[1])):
+            msg = self.zlabel + ' = ' + str(self.zcoords[z,t])
+            msg += ', ' + self.tlabel + ' = ' + str(self.tcoords[z,t])
         else:
-            if set:  # adjust spinbox value to image contrast
-                self.spinBox.setValue(width)
-        self.setSpinBoxStepSize(min, max)
-        self.spinBox.blockSignals(False)
-
-    def getValue(self):
-        return self.spinBox.value()
-
-    def setValue(self, value):
-        self.spinBox.blockSignals(True)
-        self.spinBox.setValue(value)
-        self.spinBox.blockSignals(False)
-
-    def setSpinBoxStepSize(self, min, max):
-        if min is None:
-            return
-        width = max-min
-        spinBoxStep = float(width / 10)
-        self.spinBox.setSingleStep(spinBoxStep)
-
-    def spinBoxValueChanged(self):
-        """Update Window Width of the image."""
-        width = self.spinBox.value()   
-        self.valueChanged.emit(width)
-
-
-class ImageBrightness(QWidget):
-
-    valueChanged = pyqtSignal(float)
-
-    def __init__(self, layout=True):
-        super().__init__() 
-        self.label = QLabel()
-        self.label.setPixmap(QPixmap(icons.brightness))
-        #self.label.setFixedSize(24, 24)
-        self.spinBox = QDoubleSpinBox()
-        self.spinBox.valueChanged.connect(self.spinBoxValueChanged)
-        self.spinBox.setToolTip("Adjust Brightness")
-        self.spinBox.setMinimum(-1000000000.00)
-        self.spinBox.setMaximum(+1000000000.00)
-        self.spinBox.setWrapping(False)
-        self.spinBox.setFixedWidth(115)
-        if layout:
-            self.layout = QHBoxLayout()
-            self.layout.setAlignment(Qt.AlignLeft  | Qt.AlignVCenter)
-            self.layout.setContentsMargins(0,0,0,0)
-            self.layout.setSpacing(2)
-            self.layout.addWidget(self.spinBox)
-            self.layout.addWidget(self.label)
-            #self.setMaximumWidth(120)
-            self.setLayout(self.layout)
-
-    def setData(self, min, max, center, set=True):
-        self.spinBox.blockSignals(True)
-        if min is None: 
-            self.spinBox.setValue(1)  
-            self.spinBox.setSingleStep(0.1)
+            v = self.array[x,y,z,t]
+            msg = 'x = ' + str(x)
+            msg += ', y = ' + str(y)
+            msg += ', ' + self.zlabel + ' = ' + str(self.zcoords[z,t])
+            msg += ', ' + self.tlabel + ' = ' + str(self.tcoords[z,t])
+            msg += ', signal = ' + str(v)
+        self.series().status.message(msg)
+
+    def setCanvas(self):
+        z = self.viewSlider.value()
+        t = self.plotSlider.value()
+        self.canvas.setArray(
+            np.squeeze(self.array[:,:,z,t]),
+            self.uid[z,t], 
+            self.center[z,t], 
+            self.width[z,t], 
+            self.colormap[z,t],
+        )
+
+    def setPlot(self):
+        if self.x is None:
+            return
+        x = self.x
+        y = self.y
+        if (not (0 <= x < self.array.shape[0]) or
+            not (0 <= y < self.array.shape[1])):
+            self.plot.clear()
         else:
-            if set:  # adjust spinbox value to image contrast
-                self.spinBox.setValue(center)
-        self.setSpinBoxStepSize(min, max)
-        self.spinBox.blockSignals(False)
-
-    def getValue(self):
-        return self.spinBox.value()
-
-    def setValue(self, center):
-        self.spinBox.blockSignals(True)
-        self.spinBox.setValue(center)
-        self.spinBox.blockSignals(False)
-
-    def setSpinBoxStepSize(self, min, max):
-        if min is None:
-            return
-        center = (max+min)/2
-        spinBoxStep = float(center / 10)
-        self.spinBox.setSingleStep(spinBoxStep)
-
-    def spinBoxValueChanged(self):
-        center = self.spinBox.value()
-        self.valueChanged.emit(center)
-
-
-
-class LockUnlockWidget(QToolBar):
-
-    toggled = pyqtSignal()
-
-    def __init__(self, toolTip = 'Lock state'):
-        super().__init__()
-        self.isLocked = True
-        self.icon_lock = QIcon(icons.lock) 
-        self.icon_lock_unlock = QIcon(icons.lock_unlock) 
-        self.mode = QAction()
-        self.mode.setIcon(self.icon_lock)
-        self.mode.setToolTip(toolTip)
-        self.mode.triggered.connect(self.toggle) 
-        self.addAction(self.mode)
-
-    def toggle(self):
-        if self.isLocked == True:
-            self.mode.setIcon(self.icon_lock_unlock)
-            self.isLocked = False
-        elif self.isLocked == False:
-            self.mode.setIcon(self.icon_lock)
-            self.isLocked = True  
-        self.toggled.emit()
-
-
+            z = self.viewSlider.value()
+            t = self.plotSlider.value()
+            self.plot.setData(self.tcoords[z,:], self.array[x,y,z,:], index=t)
 
-class DeleteImageButton(QPushButton):
 
-    buttonClicked = pyqtSignal()
 
-    def __init__(self, image=None):
-        super().__init__()
-        self.setFixedSize(24, 24)
-        self.setIcon(QIcon(icons.bin_metal))
-        self.setToolTip('Delete image')
-        self.clicked.connect(self.delete) 
-        self.setData(image)
-
-    def delete(self):
-        if self.image is None:
-            return
-        self.image.remove()
-        self.buttonClicked.emit()
-
-    def setData(self, image):
-        self.image = image
-
-
-class ExportImageButton(QPushButton):
-
-    def __init__(self, image=None):
-        super().__init__()
- 
-        self.setFixedSize(24, 24)
-        self.setIcon(QIcon(icons.blue_document_export))
-        self.setToolTip('Export as .png')
-        self.clicked.connect(self.export)
-        self.setData(image)
-
-    def setData(self, image):
-        self.image = image
-
-    def export(self):
-        """Export as png."""
-        if self.image is None: 
-            return
-        path = self.image.dialog.directory("Where do you want to export the data?")
-        self.image.export_as_png(path)
-
-
-class RestoreImageButton(QPushButton):
-
-    buttonClicked = pyqtSignal()
-
-    def __init__(self, image=None):
-        super().__init__()
-        self.setFixedSize(24, 24)
-        self.setIcon(QIcon(icons.arrow_curve_180_left))
-        self.setToolTip('Undo changes')
-        self.clicked.connect(self.restore) 
-        self.setData(image)
-
-    def setData(self, image):
-        self.image = image
+class SeriesDisplay4DView():
 
-    def restore(self):
-        if self.image is None: 
-            return
-        self.image.restore()
-        self.buttonClicked.emit()
+    def __init__(self, controller):
 
+        # Create left panel for viewing images
+        layout = QVBoxLayout()
+        layout.setContentsMargins(0, 0, 0, 0)
+        layout.setSpacing(0)
+        layout.addWidget(controller.canvas) 
+        layout.addWidget(controller.viewSlider) 
+        leftPanel = QWidget() 
+        leftPanel.setLayout(layout)
+        
+        # Create right panel for viewing curve plots
+        layout = QVBoxLayout()
+        layout.setContentsMargins(0, 0, 0, 0)
+        layout.setSpacing(0)
+        layout.addWidget(controller.plot) 
+        layout.addWidget(controller.plotSlider) 
+        rightPanel = QWidget() 
+        rightPanel.setLayout(layout)
+        
+        # Add left and right panel to splitter
+        splitter = QSplitter()
+        splitter.addWidget(leftPanel)
+        splitter.addWidget(rightPanel)
+        splitter.setSizes(2*[controller.geometry().width()/2])
+        layout = QVBoxLayout()
+        layout.setContentsMargins(0, 0, 0, 0)
+        layout.setSpacing(0)
+        layout.addWidget(splitter)
+        controller.setLayout(layout)
 
-class SaveImageButton(QPushButton):
 
-    buttonClicked = pyqtSignal()
+class SeriesDisplay4DToolBar(canvas.ToolBar):
 
-    def __init__(self, image=None):
+    def __init__(self):
         super().__init__()
-
-        self.setFixedSize(24, 24)
-        self.setIcon(QIcon(icons.disk))
-        self.setToolTip('Save changes')
-        self.clicked.connect(self.save) 
-
-        self.setData(image)
-
-    def save(self):
- 
-        if self.image is None:
-            return
-        self.image.save()
-        self.buttonClicked.emit()
-
-    def setData(self, image):
-        self.image = image
-
+        self.window.valueChanged.connect(self.setPlotRange)
+        self.actionSetDefaultColor.triggered.connect(self.setPlotRange)
+        self.filters[2].windowChanged.connect(self.setPlotRange)
+
+    def setWidget(self, widget):
+        super().setWidget(widget.canvas)
+        self.plot = widget.plot
+        self.widget = widget
+
+    def setPlotRange(self):
+        center = self.canvas.center()
+        width = self.canvas.width()
+        xmin = center - width/2
+        xmax = center + width/2
+        self.plot.setYlim([xmin, xmax])
+        self.widget.setPlot()
```

### Comparing `wezel-0.1.1/src/wezel/widgets/dicom_header.py` & `wezel-0.1.2/src/wezel/displays/dicom_header.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,18 +1,18 @@
 """This module contains custom widgets for the display DICOM Series Metadata in a table."""
 
 
-from PyQt5.QtCore import Qt
-from PyQt5.QtWidgets import (QFileDialog, QLineEdit, QApplication,                           
-        QMessageBox, QWidget, QVBoxLayout, QHBoxLayout, QTableWidgetItem,
+from PySide2.QtCore import Qt
+from PySide2.QtWidgets import (QFileDialog, QLineEdit, QApplication,                           
+        QWidget, QVBoxLayout, QHBoxLayout, QTableWidgetItem,
         QPushButton, QLabel,  QHeaderView,  QTableWidget,  QAbstractItemView, QScrollArea)
 
 import pydicom
 import pandas as pd
-from wezel import MainWidget
+import wezel
 
 
 localStyleSheet = """
     QTableWidget {
     alternate-background-color: #dce2f2;background-color: #b6bdd1;
     } 
     """
@@ -80,15 +80,15 @@
         verticalLayout.addWidget(self.label)
 
    
     def setText(self, text):
         self.label.setText(text)
 
 
-class SeriesViewerMetaData(MainWidget):
+class SeriesViewerMetaData(wezel.gui.MainWidget):
     """Display DICOM Series Metadata in a table."""
 
     rowHeight = 4
 
     def __init__(self, series):  
         """
         Constructs the composite widget for displaying a table of DICOM series metadata
@@ -97,15 +97,15 @@
         #Get the DICOM object for the first image in the series
         #The DICOM object for an image contains the metadata for the whole series
         instances = series.children()
         if instances == []:
             self.setError('Series ' + series.label() + ' is empty. \n\n Nothing to show here..')
             return 
         self._objectDICOM = instances[0].get_dataset()
-        self.series = series
+        self._series = series
 
         layout = QVBoxLayout()
         layout.setContentsMargins(0, 0, 0, 0)
         layout.setSpacing(0)
 
         self.setLayout(layout)
         self.setAttribute(Qt.WA_DeleteOnClose)
@@ -133,29 +133,33 @@
         self.horizontalBox.setContentsMargins(0, 0, 0, 0)
         self.horizontalBox.setSpacing(0)
         self.horizontalBox.addWidget(self.searchField)
         self.horizontalBox.addWidget(self.export_csv_button)
 
         self.layout().addLayout(self.horizontalBox)
         self.layout().addWidget(self.tableWidget) 
+
+    def series(self): # requried attribute
+        return self._series
         
     
     def resizeColumnsToContents(self):
         header = self.tableWidget.horizontalHeader()
         header.setSectionResizeMode(0, QHeaderView.ResizeToContents)
         header.setSectionResizeMode(1, QHeaderView.ResizeToContents)
         header.setSectionResizeMode(2, QHeaderView.ResizeToContents)
         header.setSectionResizeMode(3, QHeaderView.ResizeMode(QHeaderView.AdjustToContentsOnFirstShow))
 
 
-    def createScrollableLabel(self, rowPosition, valueMetadata):
-        scrollableLabel = ScrollLabel()
-        scrollableLabel.setText(valueMetadata)
-        self.tableWidget.setCellWidget(rowPosition, 3, scrollableLabel)
-        self.tableWidget.resizeRowToContents(rowPosition)
+    # Too slow
+    # def createScrollableLabel(self, rowPosition, valueMetadata):
+    #     scrollableLabel = ScrollLabel()
+    #     scrollableLabel.setText(valueMetadata)
+    #     self.tableWidget.setCellWidget(rowPosition, 3, scrollableLabel)
+    #     self.tableWidget.resizeRowToContents(rowPosition)
 
 
     def populateTable(self):
         """Builds a Table View displaying DICOM image metadata
         as Tag, name, VR & Value"""
     
         QApplication.setOverrideCursor(Qt.WaitCursor)
@@ -178,17 +182,17 @@
                     try:
                         valueMetadata = str(list(meta_element))
                     except:
                         valueMetadata = str(meta_element.value)
                 else:
                     valueMetadata = str(meta_element.value)
 
-                if meta_element.VR == "OB" or meta_element.VR == "OW":
-                    self.createScrollableLabel(rowPosition, valueMetadata)
-                elif meta_element.VR == "SQ":
+                # if meta_element.VR == "OB" or meta_element.VR == "OW":
+                #     self.createScrollableLabel(rowPosition, valueMetadata)
+                if meta_element.VR == "SQ":
                     self.iterateSequenceTag(self.tableWidget, meta_element)
                 else:
                     self.tableWidget.setItem(rowPosition , 3, QTableWidgetItem(valueMetadata))
             
             for data_element in self._objectDICOM:
                 # Exclude pixel data from metadata listing
                 if data_element.name == 'Pixel Data':
@@ -210,17 +214,17 @@
                         try:
                             valueMetadata = str(data_element.value.decode('utf-8'))
                         except:
                             valueMetadata = str(data_element.value)
                 else:
                     valueMetadata = str(data_element.value)
 
-                if data_element.VR == "OB" or data_element.VR == "OW":
-                    self.createScrollableLabel(rowPosition, valueMetadata)
-                elif data_element.VR == "SQ":
+                # if data_element.VR == "OB" or data_element.VR == "OW":
+                #     self.createScrollableLabel(rowPosition, valueMetadata)
+                if data_element.VR == "SQ":
                     self.iterateSequenceTag(self.tableWidget, data_element)
                 else:
                     self.tableWidget.setItem(rowPosition , 3, QTableWidgetItem(valueMetadata))
         self.resizeColumnsToContents()
         QApplication.restoreOverrideCursor()
 
 
@@ -247,23 +251,24 @@
                 self.iterateSequenceTag(table, data_element, level='    ')
             else:
                 rowPosition = table.rowCount()
                 table.insertRow(rowPosition)
                 table.setItem(rowPosition , 0, QTableWidgetItem(level + ' ' + str(data_element.tag)))
                 table.setItem(rowPosition , 1, QTableWidgetItem(data_element.name))
                 table.setItem(rowPosition , 2, QTableWidgetItem(data_element.VR))
+
                 if data_element.VR == "OW" or data_element.VR == "OB":
                     try:
                         valueMetadata = str(data_element.value.decode('utf-8'))
                     except:
                         try:
                             valueMetadata = str(list(data_element))
                         except:
                             valueMetadata = str(data_element.value)
-                    self.createScrollableLabel(rowPosition, valueMetadata)
+                    #self.createScrollableLabel(rowPosition, valueMetadata)
                 else:
                     valueMetadata =  str(data_element.value)
                 
                 if data_element.VR == "SQ":
                     level+=' > '
                     self.iterateSequenceTag(table, data_element, level)
                 else:
@@ -282,15 +287,15 @@
                 item = self.tableWidget.item(row, col)
                 if item is None:
                     #item = self.tableWidget.cellWidget(row, col) 
                     pass # THIS NEEDS FIXING
                 else:
                     text = item.text()
                 df.at[row, columHeaders[col]] = text
-        filename, _ = QFileDialog.getSaveFileName(parent, 'Save CSV file as ...', self.series.label()+'.csv', "CSV files (*.csv)") 
+        filename, _ = QFileDialog.getSaveFileName(parent, 'Save CSV file as ...', self._series.label()+'.csv', "CSV files (*.csv)") 
         if filename != '':
             df.to_csv(filename, index=False)
 
 
 
     def searchTable(self, expression):
```

### Comparing `wezel-0.1.1/src/wezel/widgets/main_mdi.py` & `wezel-0.1.2/src/wezel/widgets/main_mdi.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,10 +1,10 @@
-from PyQt5.QtCore import Qt, pyqtSignal
-from PyQt5.QtGui import QIcon, QBrush
-from PyQt5.QtWidgets import (                         
+from PySide2.QtCore import Qt, Signal
+from PySide2.QtGui import QIcon, QBrush
+from PySide2.QtWidgets import (                         
     QMdiArea, QWidget, QVBoxLayout, 
     QMdiSubWindow, QLabel,
 )
 
 class MainMultipleDocumentInterface(QMdiArea):
 
     def __init__(self):
@@ -62,15 +62,15 @@
         self.addSubWindow(subWindow)
         self.activeWindow = subWindow
         return subWindow
 
 
 class MainMdiSubWindow(QMdiSubWindow):
 
-    closed = pyqtSignal()
+    closed = Signal()
 
     def __init__(self, parent=None):
         super().__init__(parent)
 
     def closeEvent(self, event):
         self.widget().close()
         #self.deleteLater()
```

### Comparing `wezel-0.1.1/src/wezel/widgets/plot_curve.py` & `wezel-0.1.2/src/wezel/displays/plot_display.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,64 +1,63 @@
+from PySide2.QtWidgets import (
+    QVBoxLayout,
+)
+
+import wezel
+from wezel import widgets
+
+class PlotDisplay(wezel.gui.MainWidget):
+    """
+    GUI for displaying a 4D numpy array
+    """
 
-import matplotlib.pyplot as plt
-from matplotlib.backends.backend_qt5agg import FigureCanvasQTAgg
-
-from PyQt5.QtWidgets import QWidget, QVBoxLayout
-
-class PlotCurve(QWidget):
-
-    def __init__(self):
+    def __init__(self, *args, **kwargs): 
         super().__init__()
+        self.initUI()
+        self.setPlot(*args, **kwargs)
 
-        self.figure = plt.figure()
-        self.figure.set_visible(True)
-        self.canvas = FigureCanvasQTAgg(self.figure)
-        self.xLabel = 'x-label'
-        self.yLabel = 'y-label'
-        self.xLim = None
-        self.yLim = None
-       
-        self.subPlot = self.figure.add_subplot(111)
+    def initUI(self):
 
+        # Widgets
+        self.plot = widgets.PlotCurve()
+
+        # Layout
         layout = QVBoxLayout()
         layout.setContentsMargins(0, 0, 0, 0)
         layout.setSpacing(0)
-        layout.addWidget(self.canvas)
+        layout.addWidget(self.plot)
         self.setLayout(layout)
 
-    def setXlim(self, xLim):
-        self.xLim = xLim
+    def setPlot(self, x, y, 
+            xlabel='x-axis', ylabel='y-axis',
+            xlim=None, ylim=None,
+        ):
+        self.x = x
+        self.y = y
+        self.plot.setXlabel(xlabel)
+        self.plot.setYlabel(ylabel)
+        self.plot.setXlim(xlim)
+        self.plot.setYlim(ylim)
+        self.plot.setData(x, y)
+
+    def set_xlabel(self, label):
+        self.plot.setXlabel(label)
+
+    def set_ylabel(self, label):
+        self.plot.setYlabel(label)
+
+    def draw(self):
+        self.plot.setData(self.x, self.y)
+
+
+
+
+
+
+
+
+
+
+
 
-    def setYlim(self, yLim):
-        self.yLim = yLim
 
-    def setXlabel(self, label):
-        self.xLabel = label
 
-    def setYlabel(self, label):
-        self.yLabel = label
-
-    def clear(self):
-        self.subPlot.clear()
-        self.canvas.draw()
-
-    def setData(self, x, y, index=None):
-        self.subPlot.clear()
-        self.subPlot.tick_params(
-            axis='both', 
-            which='major', 
-            labelsize=10)
-        if self.xLim is not None:
-            self.subPlot.set_xlim(self.xLim)
-        if self.yLim is not None:
-            self.subPlot.set_ylim(self.yLim)
-        self.subPlot.set_xlabel(
-            self.xLabel, loc='center', 
-            va='top', fontsize=10)
-        self.subPlot.set_ylabel(
-            self.yLabel, loc='center', 
-            fontsize=10)
-        self.subPlot.grid()
-        self.subPlot.plot(x, y)
-        if index is not None:
-            self.subPlot.plot(x[index], y[index], 'bo')
-        self.canvas.draw()
```

### Comparing `wezel-0.1.1/src/wezel/widgets/region_list.py` & `wezel-0.1.2/src/wezel/widgets/region_list.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,14 @@
-from PyQt5.QtGui import QIcon
-from PyQt5.QtCore import Qt, pyqtSignal
-from PyQt5.QtWidgets import (
+from PySide2.QtGui import QIcon
+from PySide2.QtCore import Qt
+from PySide2.QtWidgets import (
     QAction,
     QWidget, 
     QComboBox, QToolBar, 
-    QHBoxLayout, QVBoxLayout,
-    QPushButton)
+    QHBoxLayout, QVBoxLayout)
 
 from wezel import icons
 
 class RegionList(QWidget):
     """Manages a list of regions on the same underlay series"""
 
     def __init__(self, layout='Horizontal'):
```

### Comparing `wezel-0.1.1/src/wezel/widgets/series_sliders.py` & `wezel-0.1.2/src/wezel/widgets/series_sliders.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,22 +1,22 @@
 import pandas as pd
 
-from PyQt5.QtCore import Qt, pyqtSignal
-from PyQt5.QtWidgets import (
+from PySide2.QtCore import Qt, Signal
+from PySide2.QtWidgets import (
     QWidget, QHBoxLayout, QPushButton,
     )
-from PyQt5.QtGui import QIcon
+from PySide2.QtGui import QIcon
 
 from wezel import widgets, icons
 
 
 class SeriesSliders(QWidget):
     """Widget with sliders to navigate through a DICOM series."""
 
-    valueChanged = pyqtSignal(object)
+    valueChanged = Signal(object)
 
     def __init__(self, series=None, image=None, dimensions=[]):  
         super().__init__()
         self._blockSignals = False
         if dimensions == []:
             self.sliderTags = ["SliceLocation","AcquisitionTime"]
         else: 
@@ -91,15 +91,15 @@
         tags = self.sliderTags.copy()  
         if self.series is None:
             self.dataFrame = pd.DataFrame([], index=[], columns=tags)
             return
         # If all required tags are in the register,
         # then just extract the register for the series;
         # else read the data from disk.
-        columns = list(self.series.manager.columns)
+        columns = list(self.series.manager.columns) # Do we need all of these?
         tags = list(set(tags + columns))
         # if set(tags) == set(columns): # integrated in dbdicom read_dataframe
         #     self.dataFrame = self.series.register()
         # else: 
         #     self.dataFrame = self.series.read_dataframe(tags)  
         self.dataFrame = self.series.read_dataframe(tags)  
         self.dataFrame.sort_values("InstanceNumber", inplace=True)
@@ -144,93 +144,31 @@
         else: 
             # Delete CheckBox sliders
             for slider in self.sliders[1:]:
                 slider.deleteLater()
             self.sliders = self.sliders[:1]
             self.sliders[0].show()
 
+
     def _sliderStateChanged(self):
 
         if self.image is None:
             self._sliderValueChanged()
         else:
             self._setActiveSliderValues()
             self._setMainSliderValue()
 
+
     def _setSliderValues(self):
         
         if self.image is None: 
             return
         self._setActiveSliderValues()
         self._setMainSliderValue()
 
-    def move(self, slider='first', direction=1, key='up'):
-        """
-        Move the sliders by one step forwards or backwards.
-
-        Arguments
-        ---------
-        Specify either slider + direction, or key.
-
-        slider : either first or second slider
-        direction : either +1 (forwards) or -1 (backwards)
-        key: arrow (left, right, up or down)
-        """
-        # Translate keyboard arrow hits to slider movement
-        self._blockSignals = True
-        if key is not None:
-            if key == 'left':
-                slider = 'first'
-                direction = -1
-            elif key == 'right':
-                slider = 'first'
-                direction = 1
-            elif key == 'up':
-                slider = 'second'
-                direction = 1
-            elif key == 'down':
-                slider = 'second'
-                direction = -1
-        active = self._activeSliders
-        if self.sliders[0].isHidden():
-            if slider == 'first':
-                sldr = active[0]
-                index = sldr.index() + direction
-                if sldr.setIndex(index):
-                    self._sliderValueChanged()
-            else:
-                if len(active) > 1:
-                    sldr = active[1]
-                else:
-                    sldr = active[0]
-                index = sldr.index() + direction
-                if sldr.setIndex(index):
-                    self._sliderValueChanged()
-
-        else: # main slider is visible
-
-            if slider == 'first':
-                sldr = self.sliders[0]
-                index = sldr.index() + direction
-                if sldr.setIndex(index):
-                    self._mainSliderValueChanged()
-            else: 
-                if len(active) > 0:
-                    sldr = active[0]
-                    index = sldr.index() + direction
-                    if sldr.setIndex(index):
-                        self._sliderValueChanged()
-                else:
-                    sldr = self.sliders[0]
-                    index = sldr.index() + direction
-                    if sldr.setIndex(index):
-                        self._mainSliderValueChanged()
-        self._blockSignals = False
-
-
     def _setActiveSliderValues(self):
 
         if self.image is None: 
             return
         find = self.dataFrame.SOPInstanceUID == self.image.uid
         row = self.dataFrame.loc[find]
         for slider in self._activeSliders:
@@ -242,14 +180,15 @@
         if self.image is None: 
             return
         imageUIDs = self._getAllSelectedImages()
         if len(imageUIDs) <= 1:
             self.sliders[0].hide()
         else:
             index = imageUIDs.index(self.image.uid)
+            self.sliders[0].setValues(range(len(imageUIDs))) # bug fix 02/03/2023
             self.sliders[0].setValue(index)
             self.sliders[0].show()
 
     def _mainSliderValueChanged(self):  
         """Change the selected image"""
 
         imageUIDs = self._getAllSelectedImages()
@@ -306,7 +245,77 @@
         activeSliders = []
         for slider in self.sliders[1:]:
             if slider.checkBox.isChecked():
                 activeSliders.append(slider)
         return activeSliders
     
 
+    def move(self, slider='first', direction=1, key='up'):
+        """
+        Move the sliders by one step forwards or backwards.
+
+        Arguments
+        ---------
+        Specify either slider + direction, or key.
+
+        slider : either first or second slider
+        direction : either +1 (forwards) or -1 (backwards)
+        key: arrow (left, right, up or down)
+        """
+        # Translate keyboard arrow hits to slider movement
+        self._blockSignals = True
+        if key is not None:
+            if key == 'left':
+                slider = 'first'
+                direction = -1
+            elif key == 'right':
+                slider = 'first'
+                direction = 1
+            elif key == 'up':
+                slider = 'second'
+                direction = 1
+            elif key == 'down':
+                slider = 'second'
+                direction = -1
+        active = self._activeSliders
+        if self.sliders[0].isHidden():
+            if slider == 'first':
+                sldr = active[0]
+                index = sldr.index() + direction
+                if sldr.setIndex(index):
+                    self._blockSignals = False
+                    self._sliderValueChanged()
+            else:
+                if len(active) > 1:
+                    sldr = active[1]
+                else:
+                    sldr = active[0]
+                index = sldr.index() + direction
+                if sldr.setIndex(index):
+                    self._blockSignals = False
+                    self._sliderValueChanged()
+
+        else: # main slider is visible
+
+            if slider == 'first':
+                sldr = self.sliders[0]
+                index = sldr.index() + direction
+                if sldr.setIndex(index):
+                    self._blockSignals = False
+                    self._mainSliderValueChanged()
+            else: 
+                if len(active) > 0:
+                    sldr = active[0]
+                    index = sldr.index() + direction
+                    if sldr.setIndex(index):
+                        self._blockSignals = False
+                        self._sliderValueChanged()
+                else:
+                    sldr = self.sliders[0]
+                    index = sldr.index() + direction
+                    if sldr.setIndex(index):
+                        self._blockSignals = False
+                        self._mainSliderValueChanged()
+        self._blockSignals = False
+
+    
+
```

### Comparing `wezel-0.1.1/src/wezel/widgets/sliders.py` & `wezel-0.1.2/src/wezel/widgets/sliders.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,9 +1,9 @@
-from PyQt5.QtCore import  Qt, pyqtSignal
-from PyQt5.QtWidgets import (
+from PySide2.QtCore import  Qt, Signal
+from PySide2.QtWidgets import (
     QLabel, 
     QGroupBox, 
     QHBoxLayout,  
     QSlider, 
     QCheckBox, 
 )
 
@@ -44,15 +44,15 @@
         self.blockSignals(False)
 
 
 class LabelSlider(QGroupBox):
     """A slider with a label to show the slider value.
     """
 
-    valueChanged = pyqtSignal()
+    valueChanged = Signal()
 
     def __init__(self,  label, values): 
         super().__init__()
 
         self.label = label # E.g. KeyWord or (group, element) pair of the DICOM tag
         self.values = values # E.g. List of unique values for the DICOM tag
 
@@ -137,16 +137,16 @@
     The checkbox carries a label that describes the values 
     navigated by the slider.  
 
     The application is the case where the label is a DICOM tag
     and the label Values are the unique values of that tag.
     """
 
-    stateChanged = pyqtSignal()
-    valueChanged = pyqtSignal()
+    stateChanged = Signal()
+    valueChanged = Signal()
 
     def __init__(self,  label, values): 
         super().__init__()
 
         self.label = label # E.g. KeyWord or (group, element) pair of the DICOM tag
         self.values = values # E.g. List of unique values for the DICOM tag
```

### Comparing `wezel-0.1.1/src/wezel.egg-info/PKG-INFO` & `wezel-0.1.2/src/wezel.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 Metadata-Version: 2.1
 Name: wezel
-Version: 0.1.1
+Version: 0.1.2
 Summary: Prototyping medical imaging applications
-Author-email: Steve Shillitoe <s.shillitoe@sheffield.ac.uk>, Joao Almeida e Sousa <j.g.sousa@sheffield.ac.uk>, Steven Sourbron <s.sourbron@sheffield.ac.uk>
+Author-email: Steven Sourbron <s.sourbron@sheffield.ac.uk>, Steve Shillitoe <s.shillitoe@sheffield.ac.uk>, Joao Almeida e Sousa <j.g.sousa@sheffield.ac.uk>
 License: Apache License
                                    Version 2.0, January 2004
                                 http://www.apache.org/licenses/
         
            TERMS AND CONDITIONS FOR USE, REPRODUCTION, AND DISTRIBUTION
         
            1. Definitions.
@@ -212,16 +212,16 @@
 Classifier: Intended Audience :: Science/Research
 Classifier: Topic :: Scientific/Engineering
 Classifier: Environment :: Console
 Classifier: Operating System :: OS Independent
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
-Requires-Python: >=3.6
+Requires-Python: <3.11,>=3.7
 Description-Content-Type: text/markdown
 Provides-Extra: docs
-Provides-Extra: executable
+Provides-Extra: plugins
 License-File: LICENSE
 
 `wezel` is a Python toolbox for prototyping medical imaging applications. 
 
 ***wezel is work in progress.***
```

### Comparing `wezel-0.1.1/src/wezel.egg-info/SOURCES.txt` & `wezel-0.1.2/src/wezel.egg-info/SOURCES.txt`

 * *Files 13% similar despite different names*

```diff
@@ -1,61 +1,63 @@
 LICENSE
 MANIFEST.in
 README.md
 pyproject.toml
 setup.py
 src/wezel/__init__.py
-src/wezel/core.py
-src/wezel/main.py
-src/wezel/menus.py
+src/wezel/api.py
+src/wezel/gui.py
 src/wezel.egg-info/PKG-INFO
 src/wezel.egg-info/SOURCES.txt
 src/wezel.egg-info/dependency_links.txt
 src/wezel.egg-info/requires.txt
 src/wezel.egg-info/top_level.txt
-src/wezel/actions/__init__.py
-src/wezel/actions/about.py
-src/wezel/actions/demo.py
-src/wezel/actions/edit.py
-src/wezel/actions/filter.py
-src/wezel/actions/folder.py
-src/wezel/actions/segment.py
-src/wezel/actions/test.py
-src/wezel/actions/transform.py
-src/wezel/actions/view.py
 src/wezel/canvas/__init__.py
 src/wezel/canvas/canvas.py
 src/wezel/canvas/image_filter.py
 src/wezel/canvas/mask_filter.py
 src/wezel/canvas/scene_filter.py
 src/wezel/canvas/series_canvas.py
 src/wezel/canvas/toolbar.py
 src/wezel/canvas/utils.py
+src/wezel/displays/__init__.py
+src/wezel/displays/dicom_header.py
+src/wezel/displays/plot_display.py
+src/wezel/displays/series_display.py
+src/wezel/displays/series_display_4d.py
+src/wezel/displays/table_display.py
 src/wezel/icons/__init__.py
 src/wezel/icons/inventory.py
 src/wezel/icons/fugue_icons/__init__.py
+src/wezel/icons/fugue_icons/animal-dog.png
 src/wezel/icons/fugue_icons/application-import.png
 src/wezel/icons/fugue_icons/arrow-curve-180-left.png
 src/wezel/icons/fugue_icons/arrow-curve.png
 src/wezel/icons/fugue_icons/arrow-in.png
 src/wezel/icons/fugue_icons/arrow-move.png
 src/wezel/icons/fugue_icons/arrow-out.png
 src/wezel/icons/fugue_icons/arrow-resize-090.png
+src/wezel/icons/fugue_icons/arrow-stop-090.png
+src/wezel/icons/fugue_icons/arrow-stop-270.png
 src/wezel/icons/fugue_icons/bin-metal.png
 src/wezel/icons/fugue_icons/blue-document-export.png
 src/wezel/icons/fugue_icons/brightness.png
+src/wezel/icons/fugue_icons/bug.png
+src/wezel/icons/fugue_icons/clipboard--plus.png
 src/wezel/icons/fugue_icons/color--arrow.png
 src/wezel/icons/fugue_icons/color.png
 src/wezel/icons/fugue_icons/contrast-low.png
 src/wezel/icons/fugue_icons/contrast.png
 src/wezel/icons/fugue_icons/controller-d-pad.png
 src/wezel/icons/fugue_icons/cross-script.png
 src/wezel/icons/fugue_icons/cursor.png
 src/wezel/icons/fugue_icons/cutter.png
 src/wezel/icons/fugue_icons/disk.png
+src/wezel/icons/fugue_icons/document-excel-csv.png
+src/wezel/icons/fugue_icons/document-excel.png
 src/wezel/icons/fugue_icons/eraser--arrow.png
 src/wezel/icons/fugue_icons/eraser--plus.png
 src/wezel/icons/fugue_icons/eraser.png
 src/wezel/icons/fugue_icons/hand-finger.png
 src/wezel/icons/fugue_icons/hand-point-090.png
 src/wezel/icons/fugue_icons/hand.png
 src/wezel/icons/fugue_icons/layer-select.png
@@ -70,47 +72,66 @@
 src/wezel/icons/fugue_icons/lock-unlock.png
 src/wezel/icons/fugue_icons/lock.png
 src/wezel/icons/fugue_icons/magnifier-zoom-actual.png
 src/wezel/icons/fugue_icons/magnifier-zoom-fit.png
 src/wezel/icons/fugue_icons/magnifier-zoom-in.png
 src/wezel/icons/fugue_icons/magnifier-zoom-out.png
 src/wezel/icons/fugue_icons/magnifier.png
+src/wezel/icons/fugue_icons/minus-small-circle.png
+src/wezel/icons/fugue_icons/minus-small-white.png
 src/wezel/icons/fugue_icons/minus.png
 src/wezel/icons/fugue_icons/paint-brush--arrow.png
 src/wezel/icons/fugue_icons/paint-brush--minus.png
 src/wezel/icons/fugue_icons/paint-brush--plus.png
 src/wezel/icons/fugue_icons/paint-brush.png
 src/wezel/icons/fugue_icons/paint-can--minus.png
 src/wezel/icons/fugue_icons/paint-can--plus.png
 src/wezel/icons/fugue_icons/paint.png
 src/wezel/icons/fugue_icons/pencil.png
+src/wezel/icons/fugue_icons/plus-small-white.png
 src/wezel/icons/fugue_icons/plus.png
 src/wezel/icons/fugue_icons/spectrum.png
 src/wezel/icons/fugue_icons/tick-button.png
 src/wezel/icons/fugue_icons/ui-check-box-uncheck.png
 src/wezel/icons/fugue_icons/ui-check-box.png
 src/wezel/icons/fugue_icons/wand-hat.png
 src/wezel/icons/fugue_icons/wand.png
 src/wezel/icons/images/__init__.py
 src/wezel/icons/images/wezel.jpg
 src/wezel/icons/my_icons/__init__.py
 src/wezel/icons/my_icons/favicon.ico
 src/wezel/icons/my_icons/question-mark.png
 src/wezel/icons/my_icons/slider_icon.png
-src/wezel/utils/__init__.py
-src/wezel/utils/dbimage.py
-src/wezel/utils/scipy.py
-src/wezel/utils/skimage.py
+src/wezel/icons/my_icons/wezel-icon-transparent.png
+src/wezel/icons/my_icons/wezel-icon.png
+src/wezel/menubar/__init__.py
+src/wezel/menubar/about.py
+src/wezel/menubar/edit.py
+src/wezel/menubar/folder.py
+src/wezel/menubar/view.py
+src/wezel/plugins/align.py
+src/wezel/plugins/dipy.py
+src/wezel/plugins/elastix.py
+src/wezel/plugins/hello_world.py
+src/wezel/plugins/measure.py
+src/wezel/plugins/numpy.py
+src/wezel/plugins/pyvista.py
+src/wezel/plugins/scipy.py
+src/wezel/plugins/segment.py
+src/wezel/plugins/skimage.py
+src/wezel/plugins/sklearn.py
+src/wezel/plugins/transform.py
+src/wezel/plugins/vreg.py
 src/wezel/widgets/__init__.py
 src/wezel/widgets/dbdatabase.py
 src/wezel/widgets/dbimage.py
-src/wezel/widgets/dicom_header.py
 src/wezel/widgets/file_display.py
 src/wezel/widgets/log_to_GUI.py
 src/wezel/widgets/main_mdi.py
 src/wezel/widgets/message.py
 src/wezel/widgets/plot_curve.py
 src/wezel/widgets/qrangeslider.py
 src/wezel/widgets/region_list.py
-src/wezel/widgets/series_display.py
 src/wezel/widgets/series_sliders.py
-src/wezel/widgets/sliders.py
+src/wezel/widgets/sliders.py
+src/wezel/widgets/user_input.py
+tests/test_wezel.py
```

