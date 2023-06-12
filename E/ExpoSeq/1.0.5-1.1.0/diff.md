# Comparing `tmp/ExpoSeq-1.0.5.tar.gz` & `tmp/ExpoSeq-1.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ExpoSeq-1.0.5.tar", last modified: Wed May  3 10:37:44 2023, max compression
+gzip compressed data, was "ExpoSeq-1.1.0.tar", last modified: Mon Jun 12 07:21:39 2023, max compression
```

## Comparing `ExpoSeq-1.0.5.tar` & `ExpoSeq-1.1.0.tar`

### file list

```diff
@@ -1,77 +1,14 @@
-drwxrwxrwx   0        0        0        0 2023-05-03 10:37:44.973711 ExpoSeq-1.0.5/
--rw-rw-rw-   0        0        0     1090 2023-05-02 17:31:18.000000 ExpoSeq-1.0.5/LICENSE
--rw-rw-rw-   0        0        0       59 2023-03-08 13:53:44.000000 ExpoSeq-1.0.5/MANIFEST.in
--rw-rw-rw-   0        0        0     4086 2023-05-03 10:37:44.973711 ExpoSeq-1.0.5/PKG-INFO
--rw-rw-rw-   0        0        0     3725 2023-03-11 12:17:37.000000 ExpoSeq-1.0.5/README.md
--rw-rw-rw-   0        0        0       42 2023-05-03 10:37:44.973711 ExpoSeq-1.0.5/setup.cfg
--rw-rw-rw-   0        0        0     1272 2023-05-03 10:37:24.000000 ExpoSeq-1.0.5/setup.py
-drwxrwxrwx   0        0        0        0 2023-05-03 10:37:44.895585 ExpoSeq-1.0.5/src/
-drwxrwxrwx   0        0        0        0 2023-05-03 10:37:44.895585 ExpoSeq-1.0.5/src/ExpoSeq/
--rw-rw-rw-   0        0        0        0 2023-03-08 13:17:42.000000 ExpoSeq-1.0.5/src/ExpoSeq/__init__.py
-drwxrwxrwx   0        0        0        0 2023-05-03 10:37:44.926840 ExpoSeq-1.0.5/src/ExpoSeq/augment_data/
--rw-rw-rw-   0        0        0        0 2023-03-08 13:17:42.000000 ExpoSeq-1.0.5/src/ExpoSeq/augment_data/__init__.py
--rw-rw-rw-   0        0        0     1007 2023-03-11 12:06:04.000000 ExpoSeq-1.0.5/src/ExpoSeq/augment_data/binding_data.py
--rw-rw-rw-   0        0        0      858 2023-03-08 13:17:42.000000 ExpoSeq-1.0.5/src/ExpoSeq/augment_data/check_reports.py
--rw-rw-rw-   0        0        0      913 2023-05-01 13:26:21.000000 ExpoSeq-1.0.5/src/ExpoSeq/augment_data/load_data.py
--rw-rw-rw-   0        0        0     3114 2023-05-01 13:32:58.000000 ExpoSeq-1.0.5/src/ExpoSeq/augment_data/loop_collect_reports.py
--rw-rw-rw-   0        0        0     7770 2023-03-13 10:18:22.000000 ExpoSeq-1.0.5/src/ExpoSeq/augment_data/mixcr_cl.py
--rw-rw-rw-   0        0        0    10041 2023-03-11 10:14:21.000000 ExpoSeq-1.0.5/src/ExpoSeq/augment_data/mixcr_nils.py
--rw-rw-rw-   0        0        0     5730 2023-03-10 12:50:00.000000 ExpoSeq-1.0.5/src/ExpoSeq/augment_data/randomizer.py
--rw-rw-rw-   0        0        0      580 2023-03-09 15:09:25.000000 ExpoSeq-1.0.5/src/ExpoSeq/augment_data/read_raw_data.py
--rw-rw-rw-   0        0        0     3646 2023-03-08 13:17:42.000000 ExpoSeq-1.0.5/src/ExpoSeq/augment_data/structure_files.py
--rw-rw-rw-   0        0        0      519 2023-03-08 13:17:42.000000 ExpoSeq-1.0.5/src/ExpoSeq/augment_data/trimming.py
--rw-rw-rw-   0        0        0    12835 2023-05-02 17:41:45.000000 ExpoSeq-1.0.5/src/ExpoSeq/augment_data/uploader.py
--rw-rw-rw-   0        0        0    28170 2023-03-11 12:06:04.000000 ExpoSeq-1.0.5/src/ExpoSeq/pipeline.py
-drwxrwxrwx   0        0        0        0 2023-05-03 10:37:44.942461 ExpoSeq-1.0.5/src/ExpoSeq/plots/
--rw-rw-rw-   0        0        0        0 2023-03-08 13:17:42.000000 ExpoSeq-1.0.5/src/ExpoSeq/plots/__init__.py
--rw-rw-rw-   0        0        0     2055 2023-03-08 13:17:42.000000 ExpoSeq-1.0.5/src/ExpoSeq/plots/barplot.py
--rw-rw-rw-   0        0        0     1660 2023-03-08 13:17:42.000000 ExpoSeq-1.0.5/src/ExpoSeq/plots/cluster_embedding.py
--rw-rw-rw-   0        0        0     4363 2023-03-10 14:44:08.000000 ExpoSeq-1.0.5/src/ExpoSeq/plots/embedding_with_binding.py
--rw-rw-rw-   0        0        0     3363 2023-03-10 12:31:37.000000 ExpoSeq-1.0.5/src/ExpoSeq/plots/length_distribution.py
--rw-rw-rw-   0        0        0     7663 2023-03-10 14:40:44.000000 ExpoSeq-1.0.5/src/ExpoSeq/plots/levenshtein_clustering.py
--rw-rw-rw-   0        0        0     4291 2023-03-10 12:31:37.000000 ExpoSeq-1.0.5/src/ExpoSeq/plots/logo_plot.py
--rw-rw-rw-   0        0        0     3346 2023-03-08 13:17:42.000000 ExpoSeq-1.0.5/src/ExpoSeq/plots/plt_heatmap.py
--rw-rw-rw-   0        0        0     2524 2023-03-08 13:17:42.000000 ExpoSeq-1.0.5/src/ExpoSeq/plots/protvec.py
--rw-rw-rw-   0        0        0     1464 2023-03-08 13:17:42.000000 ExpoSeq-1.0.5/src/ExpoSeq/plots/relative_sequence_abundance.py
--rw-rw-rw-   0        0        0     1634 2023-03-10 10:47:32.000000 ExpoSeq-1.0.5/src/ExpoSeq/plots/saveFig.py
--rw-rw-rw-   0        0        0     1058 2023-03-08 13:17:42.000000 ExpoSeq-1.0.5/src/ExpoSeq/plots/stacked_aa_distribution.py
--rw-rw-rw-   0        0        0     2536 2023-03-09 13:38:51.000000 ExpoSeq-1.0.5/src/ExpoSeq/plots/usq_plot.py
--rw-rw-rw-   0        0        0     3019 2023-03-11 11:48:16.000000 ExpoSeq-1.0.5/src/ExpoSeq/reset.py
--rw-rw-rw-   0        0        0     7139 2023-03-13 09:53:10.000000 ExpoSeq-1.0.5/src/ExpoSeq/run.py
-drwxrwxrwx   0        0        0        0 2023-05-03 10:37:44.942461 ExpoSeq-1.0.5/src/ExpoSeq/settings/
--rw-rw-rw-   0        0        0        0 2023-03-08 13:17:42.000000 ExpoSeq-1.0.5/src/ExpoSeq/settings/__init__.py
--rw-rw-rw-   0        0        0     2086 2023-03-08 13:17:42.000000 ExpoSeq-1.0.5/src/ExpoSeq/settings/blosum_62.txt
--rw-rw-rw-   0        0        0     1727 2023-03-10 12:14:15.000000 ExpoSeq-1.0.5/src/ExpoSeq/settings/change_save_settings.py
--rw-rw-rw-   0        0        0       94 2023-03-08 13:17:42.000000 ExpoSeq-1.0.5/src/ExpoSeq/settings/colorbar.txt
--rw-rw-rw-   0        0        0       86 2023-03-08 13:17:42.000000 ExpoSeq-1.0.5/src/ExpoSeq/settings/font_settings.txt
--rw-rw-rw-   0        0        0       57 2023-03-08 13:17:42.000000 ExpoSeq-1.0.5/src/ExpoSeq/settings/global_vars.txt
--rw-rw-rw-   0        0        0      179 2023-03-08 13:17:42.000000 ExpoSeq-1.0.5/src/ExpoSeq/settings/legend_settings.txt
--rw-rw-rw-   0        0        0     8133 2023-03-08 14:12:47.000000 ExpoSeq-1.0.5/src/ExpoSeq/settings/plot_styler.py
--rw-rw-rw-   0        0        0       42 2023-03-11 11:49:10.000000 ExpoSeq-1.0.5/src/ExpoSeq/settings/save_settings.txt
-drwxrwxrwx   0        0        0        0 2023-05-03 10:37:44.958087 ExpoSeq-1.0.5/src/ExpoSeq/tidy_data/
--rw-rw-rw-   0        0        0        0 2023-03-08 13:17:42.000000 ExpoSeq-1.0.5/src/ExpoSeq/tidy_data/__init__.py
--rw-rw-rw-   0        0        0     2176 2023-03-08 13:17:42.000000 ExpoSeq-1.0.5/src/ExpoSeq/tidy_data/aminoacid_distribution.py
--rw-rw-rw-   0        0        0     2228 2023-03-08 13:17:42.000000 ExpoSeq-1.0.5/src/ExpoSeq/tidy_data/barplot.py
--rw-rw-rw-   0        0        0     1152 2023-03-08 13:17:42.000000 ExpoSeq-1.0.5/src/ExpoSeq/tidy_data/clustering.py
-drwxrwxrwx   0        0        0        0 2023-05-03 10:37:44.958087 ExpoSeq-1.0.5/src/ExpoSeq/tidy_data/heatmaps/
--rw-rw-rw-   0        0        0        0 2023-03-08 13:17:42.000000 ExpoSeq-1.0.5/src/ExpoSeq/tidy_data/heatmaps/__init__.py
--rw-rw-rw-   0        0        0     1509 2023-03-08 13:17:42.000000 ExpoSeq-1.0.5/src/ExpoSeq/tidy_data/heatmaps/bool_sequences_matrix.py
--rw-rw-rw-   0        0        0     1818 2023-03-08 13:17:42.000000 ExpoSeq-1.0.5/src/ExpoSeq/tidy_data/heatmaps/tidy_heatmap_share.py
--rw-rw-rw-   0        0        0     1673 2023-03-08 13:17:42.000000 ExpoSeq-1.0.5/src/ExpoSeq/tidy_data/heatmaps/tidy_jaccard.py
--rw-rw-rw-   0        0        0     5139 2023-03-09 13:29:06.000000 ExpoSeq-1.0.5/src/ExpoSeq/tidy_data/heatmaps/tidy_morosita_horn.py
--rw-rw-rw-   0        0        0     1597 2023-03-08 13:17:42.000000 ExpoSeq-1.0.5/src/ExpoSeq/tidy_data/heatmaps/tidy_sorensen.py
--rw-rw-rw-   0        0        0      678 2023-03-08 13:17:42.000000 ExpoSeq-1.0.5/src/ExpoSeq/tidy_data/interpret_data.py
--rw-rw-rw-   0        0        0     3907 2023-03-08 13:17:42.000000 ExpoSeq-1.0.5/src/ExpoSeq/tidy_data/read_extract_data.py
--rw-rw-rw-   0        0        0      423 2023-03-08 13:17:42.000000 ExpoSeq-1.0.5/src/ExpoSeq/tidy_data/tidy_USQ_plot_.py
--rw-rw-rw-   0        0        0     1200 2023-03-08 13:17:42.000000 ExpoSeq-1.0.5/src/ExpoSeq/tidy_data/tidy_alignment_reports.py
--rw-rw-rw-   0        0        0     1461 2023-03-08 13:17:42.000000 ExpoSeq-1.0.5/src/ExpoSeq/tidy_data/tidy_cluster_embedding.py
--rw-rw-rw-   0        0        0      391 2023-03-08 13:17:42.000000 ExpoSeq-1.0.5/src/ExpoSeq/tidy_data/tidy_library.py
--rw-rw-rw-   0        0        0     1992 2023-03-08 13:17:42.000000 ExpoSeq-1.0.5/src/ExpoSeq/tidy_data/tidy_rel_sequence_abun.py
--rw-rw-rw-   0        0        0     1599 2023-03-08 13:17:42.000000 ExpoSeq-1.0.5/src/ExpoSeq/tidy_data/tidy_seqlogoPlot.py
--rw-rw-rw-   0        0        0     1299 2023-03-08 13:17:42.000000 ExpoSeq-1.0.5/src/ExpoSeq/tidy_data/tidy_stacked_aa_distr.py
-drwxrwxrwx   0        0        0        0 2023-05-03 10:37:44.911212 ExpoSeq-1.0.5/src/ExpoSeq.egg-info/
--rw-rw-rw-   0        0        0     4086 2023-05-03 10:37:44.000000 ExpoSeq-1.0.5/src/ExpoSeq.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0     2439 2023-05-03 10:37:44.000000 ExpoSeq-1.0.5/src/ExpoSeq.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-05-03 10:37:44.000000 ExpoSeq-1.0.5/src/ExpoSeq.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0      188 2023-05-03 10:37:44.000000 ExpoSeq-1.0.5/src/ExpoSeq.egg-info/requires.txt
--rw-rw-rw-   0        0        0        8 2023-05-03 10:37:44.000000 ExpoSeq-1.0.5/src/ExpoSeq.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-06-12 07:21:39.508294 ExpoSeq-1.1.0/
+-rw-rw-rw-   0        0        0     1090 2023-05-30 20:50:39.000000 ExpoSeq-1.1.0/LICENSE
+-rw-rw-rw-   0        0        0       59 2023-05-30 20:50:39.000000 ExpoSeq-1.1.0/MANIFEST.in
+-rw-rw-rw-   0        0        0     4091 2023-06-12 07:21:39.505781 ExpoSeq-1.1.0/PKG-INFO
+-rw-rw-rw-   0        0        0     3725 2023-05-30 20:50:39.000000 ExpoSeq-1.1.0/README.md
+-rw-rw-rw-   0        0        0       42 2023-06-12 07:21:39.508294 ExpoSeq-1.1.0/setup.cfg
+-rw-rw-rw-   0        0        0     1277 2023-06-09 10:59:18.000000 ExpoSeq-1.1.0/setup.py
+drwxrwxrwx   0        0        0        0 2023-06-12 07:21:39.483948 ExpoSeq-1.1.0/src/
+drwxrwxrwx   0        0        0        0 2023-06-12 07:21:39.505781 ExpoSeq-1.1.0/src/ExpoSeq.egg-info/
+-rw-rw-rw-   0        0        0     4091 2023-06-12 07:21:39.000000 ExpoSeq-1.1.0/src/ExpoSeq.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      212 2023-06-12 07:21:39.000000 ExpoSeq-1.1.0/src/ExpoSeq.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-06-12 07:21:39.000000 ExpoSeq-1.1.0/src/ExpoSeq.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0      188 2023-06-12 07:21:39.000000 ExpoSeq-1.1.0/src/ExpoSeq.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        1 2023-06-12 07:21:39.000000 ExpoSeq-1.1.0/src/ExpoSeq.egg-info/top_level.txt
```

### Comparing `ExpoSeq-1.0.5/LICENSE` & `ExpoSeq-1.1.0/LICENSE`

 * *Files identical despite different names*

### Comparing `ExpoSeq-1.0.5/PKG-INFO` & `ExpoSeq-1.1.0/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 Metadata-Version: 2.1
 Name: ExpoSeq
-Version: 1.0.5
+Version: 1.1.0
 Summary: A pacakge which provides various ways to analyze NGS data from phage display campaigns
 Home-page: https://github.com/nilshof01/ExpoSeq
 Author: Nils Hofmann
-Author-email: s220672@dtu.dk
+Author-email: n.hofmann.99@web.de
 License: MIT
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 # Welcome to ExpoSeq
```

### Comparing `ExpoSeq-1.0.5/README.md` & `ExpoSeq-1.1.0/README.md`

 * *Files identical despite different names*

### Comparing `ExpoSeq-1.0.5/setup.py` & `ExpoSeq-1.1.0/setup.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,21 +1,21 @@
 from setuptools import setup, find_packages
 
 with open("README.md", "r") as fh:
     long_description = fh.read()
 
 setup(
     name = "ExpoSeq",
-    version = "1.0.5",
+    version = "1.1.0",
     description = "A pacakge which provides various ways to analyze NGS data from phage display campaigns",
     long_description=long_description,
     long_description_content_type = "text/markdown",
     url = "https://github.com/nilshof01/ExpoSeq",
     author = "Nils Hofmann",
-    author_email = "s220672@dtu.dk",
+    author_email = "n.hofmann.99@web.de",
     license = "MIT",
     package_data={
         "ExpoSeq": ["settings/*.txt"]
     },
     install_requires = [
                         "numpy>=1.23.5",
                         "pandas>=1.5.3",
```

### Comparing `ExpoSeq-1.0.5/src/ExpoSeq.egg-info/PKG-INFO` & `ExpoSeq-1.1.0/src/ExpoSeq.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 Metadata-Version: 2.1
 Name: ExpoSeq
-Version: 1.0.5
+Version: 1.1.0
 Summary: A pacakge which provides various ways to analyze NGS data from phage display campaigns
 Home-page: https://github.com/nilshof01/ExpoSeq
 Author: Nils Hofmann
-Author-email: s220672@dtu.dk
+Author-email: n.hofmann.99@web.de
 License: MIT
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 # Welcome to ExpoSeq
```

