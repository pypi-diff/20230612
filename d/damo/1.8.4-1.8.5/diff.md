# Comparing `tmp/damo-1.8.4.tar.gz` & `tmp/damo-1.8.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "damo-1.8.4.tar", last modified: Mon Jun  5 19:42:27 2023, max compression
+gzip compressed data, was "damo-1.8.5.tar", last modified: Mon Jun 12 17:22:53 2023, max compression
```

## Comparing `damo-1.8.4.tar` & `damo-1.8.5.tar`

### file list

```diff
@@ -1,52 +1,57 @@
-drwxrwxr-x   0 sjpark    (1000) sjpark    (1000)        0 2023-06-05 19:42:27.117919 damo-1.8.4/
--rw-rw-r--   0 sjpark    (1000) sjpark    (1000)     8162 2023-06-05 19:42:27.117919 damo-1.8.4/PKG-INFO
--rw-rw-r--   0 sjpark    (1000) sjpark    (1000)     7641 2023-06-05 19:42:23.000000 damo-1.8.4/README.md
--rw-rw-r--   0 sjpark    (1000) sjpark    (1000)      104 2023-06-05 19:42:23.000000 damo-1.8.4/pyproject.toml
--rw-rw-r--   0 sjpark    (1000) sjpark    (1000)       38 2023-06-05 19:42:27.117919 damo-1.8.4/setup.cfg
--rw-rw-r--   0 sjpark    (1000) sjpark    (1000)     1104 2023-06-05 19:42:23.000000 damo-1.8.4/setup.py
-drwxrwxr-x   0 sjpark    (1000) sjpark    (1000)        0 2023-06-05 19:42:27.101920 damo-1.8.4/src/
-drwxrwxr-x   0 sjpark    (1000) sjpark    (1000)        0 2023-06-05 19:42:27.113920 damo-1.8.4/src/damo/
--rw-rw-r--   0 sjpark    (1000) sjpark    (1000)        0 2023-06-05 19:42:23.000000 damo-1.8.4/src/damo/__init__.py
--rw-rw-r--   0 sjpark    (1000) sjpark    (1000)     7358 2023-06-05 19:42:23.000000 damo-1.8.4/src/damo/_damo_deprecated.py
--rw-rw-r--   0 sjpark    (1000) sjpark    (1000)      963 2023-06-05 19:42:23.000000 damo-1.8.4/src/damo/_damo_deprecation_notice.py
--rw-rw-r--   0 sjpark    (1000) sjpark    (1000)      620 2023-06-05 19:42:23.000000 damo-1.8.4/src/damo/_damo_dist.py
--rw-rw-r--   0 sjpark    (1000) sjpark    (1000)     9673 2023-06-05 19:42:23.000000 damo-1.8.4/src/damo/_damo_fmt_str.py
--rw-rw-r--   0 sjpark    (1000) sjpark    (1000)     2995 2023-06-05 19:42:23.000000 damo-1.8.4/src/damo/_damo_fs.py
--rw-rw-r--   0 sjpark    (1000) sjpark    (1000)     5345 2023-06-05 19:42:23.000000 damo-1.8.4/src/damo/_damo_paddr_layout.py
--rw-rw-r--   0 sjpark    (1000) sjpark    (1000)      739 2023-06-05 19:42:23.000000 damo-1.8.4/src/damo/_damo_subcmds.py
--rw-rw-r--   0 sjpark    (1000) sjpark    (1000)    34675 2023-06-05 19:42:23.000000 damo-1.8.4/src/damo/_damon.py
--rw-rw-r--   0 sjpark    (1000) sjpark    (1000)    11111 2023-06-05 19:42:23.000000 damo-1.8.4/src/damo/_damon_args.py
--rw-rw-r--   0 sjpark    (1000) sjpark    (1000)    17097 2023-06-05 19:42:23.000000 damo-1.8.4/src/damo/_damon_dbgfs.py
--rw-rw-r--   0 sjpark    (1000) sjpark    (1000)    22589 2023-06-05 19:42:23.000000 damo-1.8.4/src/damo/_damon_result.py
--rw-rw-r--   0 sjpark    (1000) sjpark    (1000)    19134 2023-06-05 19:42:23.000000 damo-1.8.4/src/damo/_damon_sysfs.py
--rwxrwxr-x   0 sjpark    (1000) sjpark    (1000)     3723 2023-06-05 19:42:23.000000 damo-1.8.4/src/damo/damo.py
--rw-rw-r--   0 sjpark    (1000) sjpark    (1000)     2002 2023-06-05 19:42:23.000000 damo-1.8.4/src/damo/damo_adjust.py
--rw-rw-r--   0 sjpark    (1000) sjpark    (1000)      891 2023-06-05 19:42:23.000000 damo-1.8.4/src/damo/damo_convert_record_format.py
--rw-rw-r--   0 sjpark    (1000) sjpark    (1000)     1147 2023-06-05 19:42:23.000000 damo-1.8.4/src/damo/damo_features.py
--rw-rw-r--   0 sjpark    (1000) sjpark    (1000)      746 2023-06-05 19:42:23.000000 damo-1.8.4/src/damo/damo_fmt_json.py
--rw-rw-r--   0 sjpark    (1000) sjpark    (1000)    13295 2023-06-05 19:42:23.000000 damo-1.8.4/src/damo/damo_heats.py
--rw-rw-r--   0 sjpark    (1000) sjpark    (1000)     4668 2023-06-05 19:42:23.000000 damo-1.8.4/src/damo/damo_lru_sort.py
--rw-rw-r--   0 sjpark    (1000) sjpark    (1000)     3029 2023-06-05 19:42:23.000000 damo-1.8.4/src/damo/damo_monitor.py
--rw-rw-r--   0 sjpark    (1000) sjpark    (1000)     2749 2023-06-05 19:42:23.000000 damo-1.8.4/src/damo/damo_nr_regions.py
--rw-rw-r--   0 sjpark    (1000) sjpark    (1000)     4458 2023-06-05 19:42:23.000000 damo-1.8.4/src/damo/damo_reclaim.py
--rw-rw-r--   0 sjpark    (1000) sjpark    (1000)     5615 2023-06-05 19:42:23.000000 damo-1.8.4/src/damo/damo_record.py
--rw-rw-r--   0 sjpark    (1000) sjpark    (1000)     1173 2023-06-05 19:42:23.000000 damo-1.8.4/src/damo/damo_report.py
--rw-rw-r--   0 sjpark    (1000) sjpark    (1000)     3195 2023-06-05 19:42:23.000000 damo-1.8.4/src/damo/damo_report_raw.py
--rw-rw-r--   0 sjpark    (1000) sjpark    (1000)     1582 2023-06-05 19:42:23.000000 damo-1.8.4/src/damo/damo_schemes.py
--rw-rw-r--   0 sjpark    (1000) sjpark    (1000)      542 2023-06-05 19:42:23.000000 damo-1.8.4/src/damo/damo_start.py
--rw-rw-r--   0 sjpark    (1000) sjpark    (1000)     2383 2023-06-05 19:42:23.000000 damo-1.8.4/src/damo/damo_stat.py
--rw-rw-r--   0 sjpark    (1000) sjpark    (1000)     1490 2023-06-05 19:42:23.000000 damo-1.8.4/src/damo/damo_stat_kdamonds.py
--rw-rw-r--   0 sjpark    (1000) sjpark    (1000)     3056 2023-06-05 19:42:23.000000 damo-1.8.4/src/damo/damo_stat_regions.py
--rw-rw-r--   0 sjpark    (1000) sjpark    (1000)     2786 2023-06-05 19:42:23.000000 damo-1.8.4/src/damo/damo_stat_schemes.py
--rw-rw-r--   0 sjpark    (1000) sjpark    (1000)      654 2023-06-05 19:42:23.000000 damo-1.8.4/src/damo/damo_stop.py
--rw-rw-r--   0 sjpark    (1000) sjpark    (1000)      865 2023-06-05 19:42:23.000000 damo-1.8.4/src/damo/damo_translate_damos.py
--rw-rw-r--   0 sjpark    (1000) sjpark    (1000)      627 2023-06-05 19:42:23.000000 damo-1.8.4/src/damo/damo_tune.py
--rw-rw-r--   0 sjpark    (1000) sjpark    (1000)     3943 2023-06-05 19:42:23.000000 damo-1.8.4/src/damo/damo_validate.py
--rw-rw-r--   0 sjpark    (1000) sjpark    (1000)       22 2023-06-05 19:42:23.000000 damo-1.8.4/src/damo/damo_version.py
--rw-rw-r--   0 sjpark    (1000) sjpark    (1000)     5553 2023-06-05 19:42:23.000000 damo-1.8.4/src/damo/damo_wss.py
-drwxrwxr-x   0 sjpark    (1000) sjpark    (1000)        0 2023-06-05 19:42:27.117919 damo-1.8.4/src/damo.egg-info/
--rw-rw-r--   0 sjpark    (1000) sjpark    (1000)     8162 2023-06-05 19:42:27.000000 damo-1.8.4/src/damo.egg-info/PKG-INFO
--rw-rw-r--   0 sjpark    (1000) sjpark    (1000)     1174 2023-06-05 19:42:27.000000 damo-1.8.4/src/damo.egg-info/SOURCES.txt
--rw-rw-r--   0 sjpark    (1000) sjpark    (1000)        1 2023-06-05 19:42:27.000000 damo-1.8.4/src/damo.egg-info/dependency_links.txt
--rw-rw-r--   0 sjpark    (1000) sjpark    (1000)       40 2023-06-05 19:42:27.000000 damo-1.8.4/src/damo.egg-info/entry_points.txt
--rw-rw-r--   0 sjpark    (1000) sjpark    (1000)        5 2023-06-05 19:42:27.000000 damo-1.8.4/src/damo.egg-info/top_level.txt
+drwxrwxr-x   0 sjpark    (1000) sjpark    (1000)        0 2023-06-12 17:22:53.175708 damo-1.8.5/
+-rw-rw-r--   0 sjpark    (1000) sjpark    (1000)     8162 2023-06-12 17:22:53.175708 damo-1.8.5/PKG-INFO
+-rw-rw-r--   0 sjpark    (1000) sjpark    (1000)     7641 2023-06-12 17:22:49.000000 damo-1.8.5/README.md
+-rw-rw-r--   0 sjpark    (1000) sjpark    (1000)      104 2022-04-22 09:53:30.000000 damo-1.8.5/pyproject.toml
+-rw-rw-r--   0 sjpark    (1000) sjpark    (1000)       38 2023-06-12 17:22:53.175708 damo-1.8.5/setup.cfg
+-rw-rw-r--   0 sjpark    (1000) sjpark    (1000)     1104 2023-05-13 14:44:13.000000 damo-1.8.5/setup.py
+drwxrwxr-x   0 sjpark    (1000) sjpark    (1000)        0 2023-06-12 17:22:53.159708 damo-1.8.5/src/
+drwxrwxr-x   0 sjpark    (1000) sjpark    (1000)        0 2023-06-12 17:22:53.171708 damo-1.8.5/src/damo/
+-rw-rw-r--   0 sjpark    (1000) sjpark    (1000)        0 2023-06-12 17:22:49.000000 damo-1.8.5/src/damo/__init__.py
+-rw-rw-r--   0 sjpark    (1000) sjpark    (1000)     7358 2023-06-04 17:35:27.000000 damo-1.8.5/src/damo/_damo_deprecated.py
+-rw-rw-r--   0 sjpark    (1000) sjpark    (1000)      963 2023-05-21 19:11:52.000000 damo-1.8.5/src/damo/_damo_deprecation_notice.py
+-rw-rw-r--   0 sjpark    (1000) sjpark    (1000)      620 2023-05-20 19:08:28.000000 damo-1.8.5/src/damo/_damo_dist.py
+-rw-rw-r--   0 sjpark    (1000) sjpark    (1000)     9673 2023-05-20 19:08:28.000000 damo-1.8.5/src/damo/_damo_fmt_str.py
+-rw-rw-r--   0 sjpark    (1000) sjpark    (1000)     2995 2023-05-20 19:08:28.000000 damo-1.8.5/src/damo/_damo_fs.py
+-rw-rw-r--   0 sjpark    (1000) sjpark    (1000)     5345 2023-05-20 19:08:28.000000 damo-1.8.5/src/damo/_damo_paddr_layout.py
+-rw-rw-r--   0 sjpark    (1000) sjpark    (1000)      739 2023-05-20 19:08:28.000000 damo-1.8.5/src/damo/_damo_subcmds.py
+-rw-rw-r--   0 sjpark    (1000) sjpark    (1000)    34675 2023-06-04 19:34:22.000000 damo-1.8.5/src/damo/_damon.py
+-rw-rw-r--   0 sjpark    (1000) sjpark    (1000)    11111 2023-05-29 19:08:47.000000 damo-1.8.5/src/damo/_damon_args.py
+-rw-rw-r--   0 sjpark    (1000) sjpark    (1000)    17097 2023-06-04 19:28:36.000000 damo-1.8.5/src/damo/_damon_dbgfs.py
+-rw-rw-r--   0 sjpark    (1000) sjpark    (1000)    22589 2023-06-04 19:06:02.000000 damo-1.8.5/src/damo/_damon_result.py
+-rw-rw-r--   0 sjpark    (1000) sjpark    (1000)    19134 2023-06-04 19:28:46.000000 damo-1.8.5/src/damo/_damon_sysfs.py
+-rwxrwxr-x   0 sjpark    (1000) sjpark    (1000)     3880 2023-06-10 21:05:04.000000 damo-1.8.5/src/damo/damo.py
+-rw-rw-r--   0 sjpark    (1000) sjpark    (1000)     2002 2023-06-03 19:10:51.000000 damo-1.8.5/src/damo/damo_adjust.py
+-rw-rw-r--   0 sjpark    (1000) sjpark    (1000)      891 2023-06-03 18:38:32.000000 damo-1.8.5/src/damo/damo_convert_record_format.py
+-rw-rw-r--   0 sjpark    (1000) sjpark    (1000)     1147 2023-05-20 19:08:28.000000 damo-1.8.5/src/damo/damo_features.py
+-rw-rw-r--   0 sjpark    (1000) sjpark    (1000)      746 2023-05-20 19:08:28.000000 damo-1.8.5/src/damo/damo_fmt_json.py
+-rw-rw-r--   0 sjpark    (1000) sjpark    (1000)    13295 2023-06-03 19:10:58.000000 damo-1.8.5/src/damo/damo_heats.py
+-rw-rw-r--   0 sjpark    (1000) sjpark    (1000)     4668 2023-05-20 19:08:28.000000 damo-1.8.5/src/damo/damo_lru_sort.py
+-rw-rw-r--   0 sjpark    (1000) sjpark    (1000)     3029 2023-05-20 19:08:28.000000 damo-1.8.5/src/damo/damo_monitor.py
+-rw-rw-r--   0 sjpark    (1000) sjpark    (1000)     2749 2023-06-03 19:10:58.000000 damo-1.8.5/src/damo/damo_nr_regions.py
+-rw-rw-r--   0 sjpark    (1000) sjpark    (1000)     4458 2023-05-20 19:08:28.000000 damo-1.8.5/src/damo/damo_reclaim.py
+-rw-rw-r--   0 sjpark    (1000) sjpark    (1000)     5615 2023-06-04 19:26:26.000000 damo-1.8.5/src/damo/damo_record.py
+-rw-rw-r--   0 sjpark    (1000) sjpark    (1000)     4132 2023-06-11 18:10:19.000000 damo-1.8.5/src/damo/damo_record_info.py
+-rw-rw-r--   0 sjpark    (1000) sjpark    (1000)     1173 2023-06-04 19:50:04.000000 damo-1.8.5/src/damo/damo_report.py
+-rw-rw-r--   0 sjpark    (1000) sjpark    (1000)     3195 2023-06-11 19:00:48.000000 damo-1.8.5/src/damo/damo_report_raw.py
+-rw-rw-r--   0 sjpark    (1000) sjpark    (1000)     1582 2023-06-04 19:26:37.000000 damo-1.8.5/src/damo/damo_schemes.py
+-rw-rw-r--   0 sjpark    (1000) sjpark    (1000)      974 2023-06-11 18:40:28.000000 damo-1.8.5/src/damo/damo_show.py
+-rw-rw-r--   0 sjpark    (1000) sjpark    (1000)     1653 2023-06-11 19:01:29.000000 damo-1.8.5/src/damo/damo_show_accesses.py
+-rw-rw-r--   0 sjpark    (1000) sjpark    (1000)      837 2023-06-11 18:26:23.000000 damo-1.8.5/src/damo/damo_show_snapshot.py
+-rw-rw-r--   0 sjpark    (1000) sjpark    (1000)     3354 2023-06-11 17:45:41.000000 damo-1.8.5/src/damo/damo_show_status.py
+-rw-rw-r--   0 sjpark    (1000) sjpark    (1000)      542 2023-05-20 19:08:28.000000 damo-1.8.5/src/damo/damo_start.py
+-rw-rw-r--   0 sjpark    (1000) sjpark    (1000)     2383 2023-06-10 19:35:18.000000 damo-1.8.5/src/damo/damo_stat.py
+-rw-rw-r--   0 sjpark    (1000) sjpark    (1000)     1073 2023-06-10 21:05:04.000000 damo-1.8.5/src/damo/damo_stat_kdamonds.py
+-rw-rw-r--   0 sjpark    (1000) sjpark    (1000)     3056 2023-05-20 19:08:28.000000 damo-1.8.5/src/damo/damo_stat_regions.py
+-rw-rw-r--   0 sjpark    (1000) sjpark    (1000)     1016 2023-06-10 21:05:04.000000 damo-1.8.5/src/damo/damo_stat_schemes.py
+-rw-rw-r--   0 sjpark    (1000) sjpark    (1000)      654 2023-05-20 19:08:28.000000 damo-1.8.5/src/damo/damo_stop.py
+-rw-rw-r--   0 sjpark    (1000) sjpark    (1000)      865 2023-05-29 19:12:16.000000 damo-1.8.5/src/damo/damo_translate_damos.py
+-rw-rw-r--   0 sjpark    (1000) sjpark    (1000)      627 2023-05-20 19:08:28.000000 damo-1.8.5/src/damo/damo_tune.py
+-rw-rw-r--   0 sjpark    (1000) sjpark    (1000)     3943 2023-05-20 19:08:28.000000 damo-1.8.5/src/damo/damo_validate.py
+-rw-rw-r--   0 sjpark    (1000) sjpark    (1000)       22 2023-06-12 17:21:48.000000 damo-1.8.5/src/damo/damo_version.py
+-rw-rw-r--   0 sjpark    (1000) sjpark    (1000)     5553 2023-05-20 19:08:28.000000 damo-1.8.5/src/damo/damo_wss.py
+drwxrwxr-x   0 sjpark    (1000) sjpark    (1000)        0 2023-06-12 17:22:53.171708 damo-1.8.5/src/damo.egg-info/
+-rw-rw-r--   0 sjpark    (1000) sjpark    (1000)     8162 2023-06-12 17:22:53.000000 damo-1.8.5/src/damo.egg-info/PKG-INFO
+-rw-rw-r--   0 sjpark    (1000) sjpark    (1000)     1316 2023-06-12 17:22:53.000000 damo-1.8.5/src/damo.egg-info/SOURCES.txt
+-rw-rw-r--   0 sjpark    (1000) sjpark    (1000)        1 2023-06-12 17:22:53.000000 damo-1.8.5/src/damo.egg-info/dependency_links.txt
+-rw-rw-r--   0 sjpark    (1000) sjpark    (1000)       40 2023-06-12 17:22:53.000000 damo-1.8.5/src/damo.egg-info/entry_points.txt
+-rw-rw-r--   0 sjpark    (1000) sjpark    (1000)        5 2023-06-12 17:22:53.000000 damo-1.8.5/src/damo.egg-info/top_level.txt
```

### Comparing `damo-1.8.4/PKG-INFO` & `damo-1.8.5/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: damo
-Version: 1.8.4
+Version: 1.8.5
 Summary: DAMON user-space tool
 Home-page: https://github.com/awslabs/damo
 Author: SeongJae Park
 Author-email: sj@kernel.org
 Project-URL: Bug Tracker, https://github.com/awslabs/damo/issues
 Project-URL: DAMON, https://damonitor.github.io
 Classifier: Programming Language :: Python :: 3
@@ -42,16 +42,16 @@
     $ # ensure your kernel is built with CONFIG_DAMON_*=y
     $ sudo pip3 install damo
     $ sudo damo record $(pidof <your workload>)
     $ damo report heats --heatmap stdout --stdout_heatmap_color emotion
 
 The last command will show the access pattern of your workload, like below:
 
-![masim zigzag heatmap in ascii](https://raw.githubusercontent.com/awslabs/damo/v1.8.4/images/masim_zigzag_heatmap_ascii.png)
-![masim stairs heatmap in ascii](https://raw.githubusercontent.com/awslabs/damo/v1.8.4/images/masim_stairs_heatmap_ascii.png)
+![masim zigzag heatmap in ascii](https://raw.githubusercontent.com/awslabs/damo/v1.8.5/images/masim_zigzag_heatmap_ascii.png)
+![masim stairs heatmap in ascii](https://raw.githubusercontent.com/awslabs/damo/v1.8.5/images/masim_stairs_heatmap_ascii.png)
 
 
 FAQs
 ====
 
 How can I install a kernel that is built with `CONFIG_DAMON_*=y`?
 -----------------------------------------------------------------
@@ -59,15 +59,15 @@
 Please refer to 'Install'
 [section](https://sjp38.github.io/post/damon/#install) of the project webpage.
 
 Where can I get more detailed usage?
 ------------------------------------
 
 The below sections provide quick introductions for `damo`'s major features.
-For more detailed usage, please refer to [USAGE.md](https://github.com/awslabs/damo/blob/v1.8.4/USAGE.md) file.
+For more detailed usage, please refer to [USAGE.md](https://github.com/awslabs/damo/blob/v1.8.5/USAGE.md) file.
 
 
 What does the version number mean?
 ----------------------------------
 
 Nothing at all but indicate which version is more fresh.  A higher version
 number means it is more recently released.
@@ -87,19 +87,19 @@
 How can I participate in the development of `damo`?
 ---------------------------------------------------
 
 Please refer to
 [CONTRIBUTING](https://github.com/awslabs/damo/blob/next/CONTRIBUTING) file.
 
 
-Why some subcommands are not documented on [USAGE.md](https://github.com/awslabs/damo/blob/v1.8.4/USAGE.md) file?
+Why some subcommands are not documented on [USAGE.md](https://github.com/awslabs/damo/blob/v1.8.5/USAGE.md) file?
 ---------------------------------------------------------------------
 
 Only sufficiently stabilized features are documented there.  In other words,
-any feature that not documented on [USAGE.md](https://github.com/awslabs/damo/blob/v1.8.4/USAGE.md) are in experimental
+any feature that not documented on [USAGE.md](https://github.com/awslabs/damo/blob/v1.8.5/USAGE.md) are in experimental
 stage.  Such experimental features could be deprecated and removed without any
 notice and grace priods.  The documented features could also be deprecated, but
 those will provide some notification and grace periods.
 
 
 Recording Data Access Patterns
 ==============================
```

### Comparing `damo-1.8.4/README.md` & `damo-1.8.5/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -27,16 +27,16 @@
     $ # ensure your kernel is built with CONFIG_DAMON_*=y
     $ sudo pip3 install damo
     $ sudo damo record $(pidof <your workload>)
     $ damo report heats --heatmap stdout --stdout_heatmap_color emotion
 
 The last command will show the access pattern of your workload, like below:
 
-![masim zigzag heatmap in ascii](https://raw.githubusercontent.com/awslabs/damo/v1.8.4/images/masim_zigzag_heatmap_ascii.png)
-![masim stairs heatmap in ascii](https://raw.githubusercontent.com/awslabs/damo/v1.8.4/images/masim_stairs_heatmap_ascii.png)
+![masim zigzag heatmap in ascii](https://raw.githubusercontent.com/awslabs/damo/v1.8.5/images/masim_zigzag_heatmap_ascii.png)
+![masim stairs heatmap in ascii](https://raw.githubusercontent.com/awslabs/damo/v1.8.5/images/masim_stairs_heatmap_ascii.png)
 
 
 FAQs
 ====
 
 How can I install a kernel that is built with `CONFIG_DAMON_*=y`?
 -----------------------------------------------------------------
@@ -44,15 +44,15 @@
 Please refer to 'Install'
 [section](https://sjp38.github.io/post/damon/#install) of the project webpage.
 
 Where can I get more detailed usage?
 ------------------------------------
 
 The below sections provide quick introductions for `damo`'s major features.
-For more detailed usage, please refer to [USAGE.md](https://github.com/awslabs/damo/blob/v1.8.4/USAGE.md) file.
+For more detailed usage, please refer to [USAGE.md](https://github.com/awslabs/damo/blob/v1.8.5/USAGE.md) file.
 
 
 What does the version number mean?
 ----------------------------------
 
 Nothing at all but indicate which version is more fresh.  A higher version
 number means it is more recently released.
@@ -72,19 +72,19 @@
 How can I participate in the development of `damo`?
 ---------------------------------------------------
 
 Please refer to
 [CONTRIBUTING](https://github.com/awslabs/damo/blob/next/CONTRIBUTING) file.
 
 
-Why some subcommands are not documented on [USAGE.md](https://github.com/awslabs/damo/blob/v1.8.4/USAGE.md) file?
+Why some subcommands are not documented on [USAGE.md](https://github.com/awslabs/damo/blob/v1.8.5/USAGE.md) file?
 ---------------------------------------------------------------------
 
 Only sufficiently stabilized features are documented there.  In other words,
-any feature that not documented on [USAGE.md](https://github.com/awslabs/damo/blob/v1.8.4/USAGE.md) are in experimental
+any feature that not documented on [USAGE.md](https://github.com/awslabs/damo/blob/v1.8.5/USAGE.md) are in experimental
 stage.  Such experimental features could be deprecated and removed without any
 notice and grace priods.  The documented features could also be deprecated, but
 those will provide some notification and grace periods.
 
 
 Recording Data Access Patterns
 ==============================
```

### Comparing `damo-1.8.4/setup.py` & `damo-1.8.5/setup.py`

 * *Files identical despite different names*

### Comparing `damo-1.8.4/src/damo/_damo_deprecated.py` & `damo-1.8.5/src/damo/_damo_deprecated.py`

 * *Files identical despite different names*

### Comparing `damo-1.8.4/src/damo/_damo_deprecation_notice.py` & `damo-1.8.5/src/damo/_damo_deprecation_notice.py`

 * *Files identical despite different names*

### Comparing `damo-1.8.4/src/damo/_damo_dist.py` & `damo-1.8.5/src/damo/_damo_dist.py`

 * *Files identical despite different names*

### Comparing `damo-1.8.4/src/damo/_damo_fmt_str.py` & `damo-1.8.5/src/damo/_damo_fmt_str.py`

 * *Files identical despite different names*

### Comparing `damo-1.8.4/src/damo/_damo_fs.py` & `damo-1.8.5/src/damo/_damo_fs.py`

 * *Files identical despite different names*

### Comparing `damo-1.8.4/src/damo/_damo_paddr_layout.py` & `damo-1.8.5/src/damo/_damo_paddr_layout.py`

 * *Files identical despite different names*

### Comparing `damo-1.8.4/src/damo/_damo_subcmds.py` & `damo-1.8.5/src/damo/_damo_subcmds.py`

 * *Files identical despite different names*

### Comparing `damo-1.8.4/src/damo/_damon.py` & `damo-1.8.5/src/damo/_damon.py`

 * *Files identical despite different names*

### Comparing `damo-1.8.4/src/damo/_damon_args.py` & `damo-1.8.5/src/damo/_damon_args.py`

 * *Files identical despite different names*

### Comparing `damo-1.8.4/src/damo/_damon_dbgfs.py` & `damo-1.8.5/src/damo/_damon_dbgfs.py`

 * *Files identical despite different names*

### Comparing `damo-1.8.4/src/damo/_damon_result.py` & `damo-1.8.5/src/damo/_damon_result.py`

 * *Files identical despite different names*

### Comparing `damo-1.8.4/src/damo/_damon_sysfs.py` & `damo-1.8.5/src/damo/_damon_sysfs.py`

 * *Files identical despite different names*

### Comparing `damo-1.8.4/src/damo/damo.py` & `damo-1.8.5/src/damo/damo.py`

 * *Files 4% similar despite different names*

```diff
@@ -13,14 +13,15 @@
 import damo_fmt_json
 import damo_lru_sort
 import damo_monitor
 import damo_reclaim
 import damo_record
 import damo_report
 import damo_schemes
+import damo_show
 import damo_start
 import damo_stat
 import damo_stop
 import damo_translate_damos
 import damo_tune
 import damo_validate
 import damo_version
@@ -63,15 +64,18 @@
             module=_damo_subcmds.DamoSubCmdModule(None, pr_damo_version),
             msg='print the version number'),
         _damo_subcmds.DamoSubCmd(name='translate_damos',
             module=damo_translate_damos,
             msg='translate old .damos to the new json format'),
         _damo_subcmds.DamoSubCmd(name='convert_record_format',
             module=damo_convert_record_format,
-            msg='convert DAMON result record file\'s format')
+            msg='convert DAMON result record file\'s format'),
+        _damo_subcmds.DamoSubCmd(name='show',
+            module=damo_show,
+            msg='show status or results of damon operations'),
         ]
 
 class SubCmdHelpFormatter(argparse.RawDescriptionHelpFormatter):
     def _format_action(self, action):
         parts = super(argparse.RawDescriptionHelpFormatter,
                 self)._format_action(action)
         # skip sub parsers help
```

### Comparing `damo-1.8.4/src/damo/damo_adjust.py` & `damo-1.8.5/src/damo/damo_adjust.py`

 * *Files identical despite different names*

### Comparing `damo-1.8.4/src/damo/damo_convert_record_format.py` & `damo-1.8.5/src/damo/damo_convert_record_format.py`

 * *Files identical despite different names*

### Comparing `damo-1.8.4/src/damo/damo_features.py` & `damo-1.8.5/src/damo/damo_features.py`

 * *Files identical despite different names*

### Comparing `damo-1.8.4/src/damo/damo_fmt_json.py` & `damo-1.8.5/src/damo/damo_fmt_json.py`

 * *Files identical despite different names*

### Comparing `damo-1.8.4/src/damo/damo_heats.py` & `damo-1.8.5/src/damo/damo_heats.py`

 * *Files identical despite different names*

### Comparing `damo-1.8.4/src/damo/damo_lru_sort.py` & `damo-1.8.5/src/damo/damo_lru_sort.py`

 * *Files identical despite different names*

### Comparing `damo-1.8.4/src/damo/damo_monitor.py` & `damo-1.8.5/src/damo/damo_monitor.py`

 * *Files identical despite different names*

### Comparing `damo-1.8.4/src/damo/damo_nr_regions.py` & `damo-1.8.5/src/damo/damo_nr_regions.py`

 * *Files identical despite different names*

### Comparing `damo-1.8.4/src/damo/damo_reclaim.py` & `damo-1.8.5/src/damo/damo_reclaim.py`

 * *Files identical despite different names*

### Comparing `damo-1.8.4/src/damo/damo_record.py` & `damo-1.8.5/src/damo/damo_record.py`

 * *Files identical despite different names*

### Comparing `damo-1.8.4/src/damo/damo_report.py` & `damo-1.8.5/src/damo/damo_report.py`

 * *Files identical despite different names*

### Comparing `damo-1.8.4/src/damo/damo_report_raw.py` & `damo-1.8.5/src/damo/damo_report_raw.py`

 * *Files identical despite different names*

### Comparing `damo-1.8.4/src/damo/damo_schemes.py` & `damo-1.8.5/src/damo/damo_schemes.py`

 * *Files identical despite different names*

### Comparing `damo-1.8.4/src/damo/damo_start.py` & `damo-1.8.5/src/damo/damo_start.py`

 * *Files identical despite different names*

### Comparing `damo-1.8.4/src/damo/damo_stat.py` & `damo-1.8.5/src/damo/damo_stat.py`

 * *Files identical despite different names*

### Comparing `damo-1.8.4/src/damo/damo_stat_regions.py` & `damo-1.8.5/src/damo/damo_stat_regions.py`

 * *Files identical despite different names*

### Comparing `damo-1.8.4/src/damo/damo_stat_schemes.py` & `damo-1.8.5/src/damo/damo_show_status.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,16 +1,18 @@
 # SPDX-License-Identifier: GPL-2.0
 
-import argparse
+"""
+Show status of DAMON.
+"""
 
-import damo_stat
+import json
 
 import _damo_fmt_str
-import _damo_subcmds
 import _damon
+import _damon_args
 
 def pr_schemes_tried_regions(kdamonds, raw_nr):
     print('# <kdamond> <context> <scheme>')
     print('# <regions>')
     print('# ...')
     for kd_idx, kdamond in enumerate(kdamonds):
         for ctx_idx, ctx in enumerate(kdamond.contexts):
@@ -49,32 +51,47 @@
                 print('%s %s %s %s %s' % (kd_idx, ctx_idx, scheme_idx,
                     'sz_applied', _damo_fmt_str.format_sz(
                         scheme.stats.sz_applied, raw_nr)))
                 print('%s %s %s %s %s' % (kd_idx, ctx_idx, scheme_idx,
                     'qt_exceeds', _damo_fmt_str.format_nr(
                         scheme.stats.qt_exceeds, raw_nr)))
 
-def set_argparser(parser):
-    damo_stat.set_common_argparser(parser)
+def update_pr_kdamonds_summary(json_format, raw_nr):
+    kdamonds = _damon.current_kdamonds()
+    summary = [k.summary_str() for k in kdamonds]
+    if json_format:
+        print(json.dumps(summary, indent=4))
+        return
+    print('\n'.join(summary))
+
+def update_pr_kdamonds(json_format, raw_nr):
+    kdamonds, err = _damon.update_read_kdamonds()
+    if err:
+        print(err)
+        return
+    if json_format:
+        print(json.dumps([k.to_kvpairs(raw_nr) for k in kdamonds], indent=4))
+    else:
+        for idx, k in enumerate(kdamonds):
+            print('kdamond %d' % idx)
+            print(_damo_fmt_str.indent_lines( k.to_str(raw_nr), 4))
 
-def __main(args):
-    if args.stat_type == 'schemes_stats':
-        update_pr_schemes_stats(args.raw)
-    elif args.stat_type == 'schemes_tried_regions':
-        update_pr_schemes_tried_regions(args.raw)
+
+def set_argparser(parser):
+    parser.add_argument('--json', action='store_true', default=False,
+            help='print output in json format')
+    parser.add_argument('--raw', action='store_true', default=False,
+            help='print raw numbers')
+    _damon_args.set_common_argparser(parser)
+    return parser
 
 def main(args=None):
     if not args:
-        parser = argparse.ArgumentParser()
-        set_argparser(parser)
+        parser = set_argparser(parser)
         args = parser.parse_args()
 
     _damon.ensure_root_and_initialized(args)
 
-    damo_stat.run_count_delay(__main, args)
-
-    for i in range(args.count):
-        if i != args.count - 1:
-            time.sleep(args.delay)
+    update_pr_kdamonds(args.json, args.raw)
 
 if __name__ == '__main__':
     main()
```

### Comparing `damo-1.8.4/src/damo/damo_stop.py` & `damo-1.8.5/src/damo/damo_stop.py`

 * *Files identical despite different names*

### Comparing `damo-1.8.4/src/damo/damo_translate_damos.py` & `damo-1.8.5/src/damo/damo_translate_damos.py`

 * *Files identical despite different names*

### Comparing `damo-1.8.4/src/damo/damo_tune.py` & `damo-1.8.5/src/damo/damo_tune.py`

 * *Files identical despite different names*

### Comparing `damo-1.8.4/src/damo/damo_validate.py` & `damo-1.8.5/src/damo/damo_validate.py`

 * *Files identical despite different names*

### Comparing `damo-1.8.4/src/damo/damo_wss.py` & `damo-1.8.5/src/damo/damo_wss.py`

 * *Files identical despite different names*

### Comparing `damo-1.8.4/src/damo.egg-info/PKG-INFO` & `damo-1.8.5/src/damo.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: damo
-Version: 1.8.4
+Version: 1.8.5
 Summary: DAMON user-space tool
 Home-page: https://github.com/awslabs/damo
 Author: SeongJae Park
 Author-email: sj@kernel.org
 Project-URL: Bug Tracker, https://github.com/awslabs/damo/issues
 Project-URL: DAMON, https://damonitor.github.io
 Classifier: Programming Language :: Python :: 3
@@ -42,16 +42,16 @@
     $ # ensure your kernel is built with CONFIG_DAMON_*=y
     $ sudo pip3 install damo
     $ sudo damo record $(pidof <your workload>)
     $ damo report heats --heatmap stdout --stdout_heatmap_color emotion
 
 The last command will show the access pattern of your workload, like below:
 
-![masim zigzag heatmap in ascii](https://raw.githubusercontent.com/awslabs/damo/v1.8.4/images/masim_zigzag_heatmap_ascii.png)
-![masim stairs heatmap in ascii](https://raw.githubusercontent.com/awslabs/damo/v1.8.4/images/masim_stairs_heatmap_ascii.png)
+![masim zigzag heatmap in ascii](https://raw.githubusercontent.com/awslabs/damo/v1.8.5/images/masim_zigzag_heatmap_ascii.png)
+![masim stairs heatmap in ascii](https://raw.githubusercontent.com/awslabs/damo/v1.8.5/images/masim_stairs_heatmap_ascii.png)
 
 
 FAQs
 ====
 
 How can I install a kernel that is built with `CONFIG_DAMON_*=y`?
 -----------------------------------------------------------------
@@ -59,15 +59,15 @@
 Please refer to 'Install'
 [section](https://sjp38.github.io/post/damon/#install) of the project webpage.
 
 Where can I get more detailed usage?
 ------------------------------------
 
 The below sections provide quick introductions for `damo`'s major features.
-For more detailed usage, please refer to [USAGE.md](https://github.com/awslabs/damo/blob/v1.8.4/USAGE.md) file.
+For more detailed usage, please refer to [USAGE.md](https://github.com/awslabs/damo/blob/v1.8.5/USAGE.md) file.
 
 
 What does the version number mean?
 ----------------------------------
 
 Nothing at all but indicate which version is more fresh.  A higher version
 number means it is more recently released.
@@ -87,19 +87,19 @@
 How can I participate in the development of `damo`?
 ---------------------------------------------------
 
 Please refer to
 [CONTRIBUTING](https://github.com/awslabs/damo/blob/next/CONTRIBUTING) file.
 
 
-Why some subcommands are not documented on [USAGE.md](https://github.com/awslabs/damo/blob/v1.8.4/USAGE.md) file?
+Why some subcommands are not documented on [USAGE.md](https://github.com/awslabs/damo/blob/v1.8.5/USAGE.md) file?
 ---------------------------------------------------------------------
 
 Only sufficiently stabilized features are documented there.  In other words,
-any feature that not documented on [USAGE.md](https://github.com/awslabs/damo/blob/v1.8.4/USAGE.md) are in experimental
+any feature that not documented on [USAGE.md](https://github.com/awslabs/damo/blob/v1.8.5/USAGE.md) are in experimental
 stage.  Such experimental features could be deprecated and removed without any
 notice and grace priods.  The documented features could also be deprecated, but
 those will provide some notification and grace periods.
 
 
 Recording Data Access Patterns
 ==============================
```

### Comparing `damo-1.8.4/src/damo.egg-info/SOURCES.txt` & `damo-1.8.5/src/damo.egg-info/SOURCES.txt`

 * *Files 6% similar despite different names*

```diff
@@ -21,17 +21,22 @@
 src/damo/damo_fmt_json.py
 src/damo/damo_heats.py
 src/damo/damo_lru_sort.py
 src/damo/damo_monitor.py
 src/damo/damo_nr_regions.py
 src/damo/damo_reclaim.py
 src/damo/damo_record.py
+src/damo/damo_record_info.py
 src/damo/damo_report.py
 src/damo/damo_report_raw.py
 src/damo/damo_schemes.py
+src/damo/damo_show.py
+src/damo/damo_show_accesses.py
+src/damo/damo_show_snapshot.py
+src/damo/damo_show_status.py
 src/damo/damo_start.py
 src/damo/damo_stat.py
 src/damo/damo_stat_kdamonds.py
 src/damo/damo_stat_regions.py
 src/damo/damo_stat_schemes.py
 src/damo/damo_stop.py
 src/damo/damo_translate_damos.py
```

