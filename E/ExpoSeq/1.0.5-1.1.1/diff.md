# Comparing `tmp/ExpoSeq-1.0.5.tar.gz` & `tmp/ExpoSeq-1.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ExpoSeq-1.0.5.tar", last modified: Wed May  3 10:37:44 2023, max compression
+gzip compressed data, was "ExpoSeq-1.1.1.tar", last modified: Mon Jun 12 11:52:42 2023, max compression
```

## Comparing `ExpoSeq-1.0.5.tar` & `ExpoSeq-1.1.1.tar`

### file list

```diff
@@ -1,77 +1,81 @@
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
+drwxrwxrwx   0        0        0        0 2023-06-12 11:52:42.196009 ExpoSeq-1.1.1/
+-rw-rw-rw-   0        0        0     1090 2023-05-30 20:50:39.000000 ExpoSeq-1.1.1/LICENSE
+-rw-rw-rw-   0        0        0       59 2023-05-30 20:50:39.000000 ExpoSeq-1.1.1/MANIFEST.in
+-rw-rw-rw-   0        0        0     4091 2023-06-12 11:52:42.194987 ExpoSeq-1.1.1/PKG-INFO
+-rw-rw-rw-   0        0        0     3725 2023-05-30 20:50:39.000000 ExpoSeq-1.1.1/README.md
+-rw-rw-rw-   0        0        0       42 2023-06-12 11:52:42.196009 ExpoSeq-1.1.1/setup.cfg
+-rw-rw-rw-   0        0        0     1279 2023-06-12 11:52:31.000000 ExpoSeq-1.1.1/setup.py
+drwxrwxrwx   0        0        0        0 2023-06-12 11:52:41.914875 ExpoSeq-1.1.1/src/
+drwxrwxrwx   0        0        0        0 2023-06-12 11:52:41.948566 ExpoSeq-1.1.1/src/ExpoSeq/
+-rw-rw-rw-   0        0        0        0 2023-06-12 07:39:03.000000 ExpoSeq-1.1.1/src/ExpoSeq/__init__.py
+drwxrwxrwx   0        0        0        0 2023-06-12 11:52:42.010014 ExpoSeq-1.1.1/src/ExpoSeq/augment_data/
+-rw-rw-rw-   0        0        0        0 2023-05-30 20:50:39.000000 ExpoSeq-1.1.1/src/ExpoSeq/augment_data/__init__.py
+-rw-rw-rw-   0        0        0     1007 2023-05-30 20:50:39.000000 ExpoSeq-1.1.1/src/ExpoSeq/augment_data/binding_data.py
+-rw-rw-rw-   0        0        0      858 2023-05-30 20:50:39.000000 ExpoSeq-1.1.1/src/ExpoSeq/augment_data/check_reports.py
+-rw-rw-rw-   0        0        0      913 2023-05-30 20:50:39.000000 ExpoSeq-1.1.1/src/ExpoSeq/augment_data/load_data.py
+-rw-rw-rw-   0        0        0     4616 2023-06-09 10:59:18.000000 ExpoSeq-1.1.1/src/ExpoSeq/augment_data/loop_collect_reports.py
+-rw-rw-rw-   0        0        0     7915 2023-06-09 10:59:18.000000 ExpoSeq-1.1.1/src/ExpoSeq/augment_data/mixcr_cl.py
+-rw-rw-rw-   0        0        0    10406 2023-06-12 10:03:32.000000 ExpoSeq-1.1.1/src/ExpoSeq/augment_data/mixcr_nils.py
+-rw-rw-rw-   0        0        0     6586 2023-06-09 10:59:18.000000 ExpoSeq-1.1.1/src/ExpoSeq/augment_data/randomizer.py
+-rw-rw-rw-   0        0        0      580 2023-05-30 20:50:39.000000 ExpoSeq-1.1.1/src/ExpoSeq/augment_data/read_raw_data.py
+-rw-rw-rw-   0        0        0     3646 2023-05-30 20:50:39.000000 ExpoSeq-1.1.1/src/ExpoSeq/augment_data/structure_files.py
+-rw-rw-rw-   0        0        0      519 2023-05-30 20:50:39.000000 ExpoSeq-1.1.1/src/ExpoSeq/augment_data/trimming.py
+-rw-rw-rw-   0        0        0    17046 2023-06-12 11:43:10.000000 ExpoSeq-1.1.1/src/ExpoSeq/augment_data/uploader.py
+-rw-rw-rw-   0        0        0    10265 2023-06-12 11:49:42.000000 ExpoSeq-1.1.1/src/ExpoSeq/full_pipe.py
+-rw-rw-rw-   0        0        0    27442 2023-06-12 11:33:17.000000 ExpoSeq-1.1.1/src/ExpoSeq/pipeline.py
+drwxrwxrwx   0        0        0        0 2023-06-12 11:52:42.071976 ExpoSeq-1.1.1/src/ExpoSeq/plots/
+-rw-rw-rw-   0        0        0        0 2023-05-30 20:50:39.000000 ExpoSeq-1.1.1/src/ExpoSeq/plots/__init__.py
+-rw-rw-rw-   0        0        0     2061 2023-06-12 07:50:14.000000 ExpoSeq-1.1.1/src/ExpoSeq/plots/barplot.py
+-rw-rw-rw-   0        0        0     1666 2023-06-12 07:50:14.000000 ExpoSeq-1.1.1/src/ExpoSeq/plots/cluster_embedding.py
+-rw-rw-rw-   0        0        0     4363 2023-05-30 20:50:39.000000 ExpoSeq-1.1.1/src/ExpoSeq/plots/embedding_with_binding.py
+-rw-rw-rw-   0        0        0     3444 2023-06-09 10:59:18.000000 ExpoSeq-1.1.1/src/ExpoSeq/plots/length_distribution.py
+-rw-rw-rw-   0        0        0     7669 2023-06-12 07:50:14.000000 ExpoSeq-1.1.1/src/ExpoSeq/plots/levenshtein_clustering.py
+-rw-rw-rw-   0        0        0     4379 2023-06-12 07:50:14.000000 ExpoSeq-1.1.1/src/ExpoSeq/plots/logo_plot.py
+-rw-rw-rw-   0        0        0     3352 2023-06-12 07:50:14.000000 ExpoSeq-1.1.1/src/ExpoSeq/plots/plt_heatmap.py
+-rw-rw-rw-   0        0        0     2524 2023-05-30 20:50:39.000000 ExpoSeq-1.1.1/src/ExpoSeq/plots/protvec.py
+-rw-rw-rw-   0        0        0     1470 2023-06-12 07:50:14.000000 ExpoSeq-1.1.1/src/ExpoSeq/plots/relative_sequence_abundance.py
+-rw-rw-rw-   0        0        0     1634 2023-05-30 20:50:39.000000 ExpoSeq-1.1.1/src/ExpoSeq/plots/saveFig.py
+-rw-rw-rw-   0        0        0     1064 2023-06-12 07:50:14.000000 ExpoSeq-1.1.1/src/ExpoSeq/plots/stacked_aa_distribution.py
+-rw-rw-rw-   0        0        0     2542 2023-06-12 07:50:14.000000 ExpoSeq-1.1.1/src/ExpoSeq/plots/usq_plot.py
+-rw-rw-rw-   0        0        0     3019 2023-06-01 12:20:51.000000 ExpoSeq-1.1.1/src/ExpoSeq/reset.py
+-rw-rw-rw-   0        0        0      288 2023-06-12 07:47:58.000000 ExpoSeq-1.1.1/src/ExpoSeq/run.py
+drwxrwxrwx   0        0        0        0 2023-06-12 11:52:42.095794 ExpoSeq-1.1.1/src/ExpoSeq/settings/
+-rw-rw-rw-   0        0        0        0 2023-05-30 20:50:39.000000 ExpoSeq-1.1.1/src/ExpoSeq/settings/__init__.py
+-rw-rw-rw-   0        0        0     2086 2023-05-30 20:50:39.000000 ExpoSeq-1.1.1/src/ExpoSeq/settings/blosum_62.txt
+-rw-rw-rw-   0        0        0     1883 2023-06-12 11:49:42.000000 ExpoSeq-1.1.1/src/ExpoSeq/settings/change_save_settings.py
+-rw-rw-rw-   0        0        0       94 2023-06-12 11:44:07.000000 ExpoSeq-1.1.1/src/ExpoSeq/settings/colorbar.txt
+-rw-rw-rw-   0        0        0       86 2023-06-12 11:44:07.000000 ExpoSeq-1.1.1/src/ExpoSeq/settings/font_settings.txt
+-rw-rw-rw-   0        0        0       57 2023-06-12 11:44:07.000000 ExpoSeq-1.1.1/src/ExpoSeq/settings/global_vars.txt
+-rw-rw-rw-   0        0        0      179 2023-06-12 11:44:07.000000 ExpoSeq-1.1.1/src/ExpoSeq/settings/legend_settings.txt
+-rw-rw-rw-   0        0        0     8133 2023-05-30 20:50:39.000000 ExpoSeq-1.1.1/src/ExpoSeq/settings/plot_styler.py
+-rw-rw-rw-   0        0        0       42 2023-06-12 11:44:07.000000 ExpoSeq-1.1.1/src/ExpoSeq/settings/save_settings.txt
+drwxrwxrwx   0        0        0        0 2023-06-12 11:52:42.097896 ExpoSeq-1.1.1/src/ExpoSeq/test_data/
+-rw-rw-rw-   0        0        0        0 2023-06-12 07:52:57.000000 ExpoSeq-1.1.1/src/ExpoSeq/test_data/__init__.py
+-rw-rw-rw-   0        0        0     2589 2023-06-12 10:02:11.000000 ExpoSeq-1.1.1/src/ExpoSeq/test_uploader.py
+drwxrwxrwx   0        0        0        0 2023-06-12 11:52:42.160922 ExpoSeq-1.1.1/src/ExpoSeq/tidy_data/
+-rw-rw-rw-   0        0        0        0 2023-05-30 20:50:39.000000 ExpoSeq-1.1.1/src/ExpoSeq/tidy_data/__init__.py
+-rw-rw-rw-   0        0        0     2176 2023-05-30 20:50:39.000000 ExpoSeq-1.1.1/src/ExpoSeq/tidy_data/aminoacid_distribution.py
+-rw-rw-rw-   0        0        0     2228 2023-05-30 20:50:39.000000 ExpoSeq-1.1.1/src/ExpoSeq/tidy_data/barplot.py
+-rw-rw-rw-   0        0        0     1152 2023-05-30 20:50:39.000000 ExpoSeq-1.1.1/src/ExpoSeq/tidy_data/clustering.py
+drwxrwxrwx   0        0        0        0 2023-06-12 11:52:42.190953 ExpoSeq-1.1.1/src/ExpoSeq/tidy_data/heatmaps/
+-rw-rw-rw-   0        0        0        0 2023-05-30 20:50:39.000000 ExpoSeq-1.1.1/src/ExpoSeq/tidy_data/heatmaps/__init__.py
+-rw-rw-rw-   0        0        0     1509 2023-05-30 20:50:39.000000 ExpoSeq-1.1.1/src/ExpoSeq/tidy_data/heatmaps/bool_sequences_matrix.py
+-rw-rw-rw-   0        0        0     1818 2023-05-30 20:50:39.000000 ExpoSeq-1.1.1/src/ExpoSeq/tidy_data/heatmaps/tidy_heatmap_share.py
+-rw-rw-rw-   0        0        0     1673 2023-05-30 20:50:39.000000 ExpoSeq-1.1.1/src/ExpoSeq/tidy_data/heatmaps/tidy_jaccard.py
+-rw-rw-rw-   0        0        0     5139 2023-05-30 20:50:39.000000 ExpoSeq-1.1.1/src/ExpoSeq/tidy_data/heatmaps/tidy_morosita_horn.py
+-rw-rw-rw-   0        0        0     1597 2023-05-30 20:50:39.000000 ExpoSeq-1.1.1/src/ExpoSeq/tidy_data/heatmaps/tidy_sorensen.py
+-rw-rw-rw-   0        0        0      678 2023-05-30 20:50:39.000000 ExpoSeq-1.1.1/src/ExpoSeq/tidy_data/interpret_data.py
+-rw-rw-rw-   0        0        0     3907 2023-05-30 20:50:39.000000 ExpoSeq-1.1.1/src/ExpoSeq/tidy_data/read_extract_data.py
+-rw-rw-rw-   0        0        0      440 2023-06-12 07:48:51.000000 ExpoSeq-1.1.1/src/ExpoSeq/tidy_data/tidy_USQ_plot_.py
+-rw-rw-rw-   0        0        0     1217 2023-06-12 07:48:51.000000 ExpoSeq-1.1.1/src/ExpoSeq/tidy_data/tidy_alignment_reports.py
+-rw-rw-rw-   0        0        0     1461 2023-05-30 20:50:39.000000 ExpoSeq-1.1.1/src/ExpoSeq/tidy_data/tidy_cluster_embedding.py
+-rw-rw-rw-   0        0        0      391 2023-05-30 20:50:39.000000 ExpoSeq-1.1.1/src/ExpoSeq/tidy_data/tidy_library.py
+-rw-rw-rw-   0        0        0     1992 2023-05-30 20:50:39.000000 ExpoSeq-1.1.1/src/ExpoSeq/tidy_data/tidy_rel_sequence_abun.py
+-rw-rw-rw-   0        0        0     1599 2023-05-30 20:50:39.000000 ExpoSeq-1.1.1/src/ExpoSeq/tidy_data/tidy_seqlogoPlot.py
+-rw-rw-rw-   0        0        0     1299 2023-05-30 20:50:39.000000 ExpoSeq-1.1.1/src/ExpoSeq/tidy_data/tidy_stacked_aa_distr.py
+drwxrwxrwx   0        0        0        0 2023-06-12 11:52:41.958495 ExpoSeq-1.1.1/src/ExpoSeq.egg-info/
+-rw-rw-rw-   0        0        0     4091 2023-06-12 11:52:41.000000 ExpoSeq-1.1.1/src/ExpoSeq.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0     2527 2023-06-12 11:52:41.000000 ExpoSeq-1.1.1/src/ExpoSeq.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-06-12 11:52:41.000000 ExpoSeq-1.1.1/src/ExpoSeq.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0      188 2023-06-12 11:52:41.000000 ExpoSeq-1.1.1/src/ExpoSeq.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        8 2023-06-12 11:52:41.000000 ExpoSeq-1.1.1/src/ExpoSeq.egg-info/top_level.txt
```

### Comparing `ExpoSeq-1.0.5/LICENSE` & `ExpoSeq-1.1.1/LICENSE`

 * *Files identical despite different names*

### Comparing `ExpoSeq-1.0.5/PKG-INFO` & `ExpoSeq-1.1.1/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 Metadata-Version: 2.1
 Name: ExpoSeq
-Version: 1.0.5
+Version: 1.1.1
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

### Comparing `ExpoSeq-1.0.5/README.md` & `ExpoSeq-1.1.1/README.md`

 * *Files identical despite different names*

### Comparing `ExpoSeq-1.0.5/setup.py` & `ExpoSeq-1.1.1/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,21 +1,21 @@
 from setuptools import setup, find_packages
 
 with open("README.md", "r") as fh:
     long_description = fh.read()
 
 setup(
     name = "ExpoSeq",
-    version = "1.0.5",
+    version = "1.1.1",
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
@@ -30,8 +30,8 @@
                         "biopython==1.80",
                         "sgt>=2.0.3",
                         ],
     python_requires=">=3.8",
     package_dir = {"": "src"},
     packages = find_packages(where="src"),
 
-)
+)
```

### Comparing `ExpoSeq-1.0.5/src/ExpoSeq/augment_data/binding_data.py` & `ExpoSeq-1.1.1/src/ExpoSeq/augment_data/binding_data.py`

 * *Files identical despite different names*

### Comparing `ExpoSeq-1.0.5/src/ExpoSeq/augment_data/check_reports.py` & `ExpoSeq-1.1.1/src/ExpoSeq/augment_data/check_reports.py`

 * *Files identical despite different names*

### Comparing `ExpoSeq-1.0.5/src/ExpoSeq/augment_data/load_data.py` & `ExpoSeq-1.1.1/src/ExpoSeq/augment_data/load_data.py`

 * *Files identical despite different names*

### Comparing `ExpoSeq-1.0.5/src/ExpoSeq/augment_data/mixcr_cl.py` & `ExpoSeq-1.1.1/src/ExpoSeq/augment_data/mixcr_cl.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 import pandas as pd
 import os
 import subprocess
 import pickle
 from glob import glob
 import shutil
-from src.ExpoSeq.augment_data.trimming import trimming
+from ExpoSeq.augment_data.trimming import trimming
 #from .trimming import trimming
 
 #
 def remove_directories(directory_path):
     # Iterate over all items in the directory
     for item in os.listdir(directory_path):
         shutil.rmtree(os.path.join(directory_path, item))
@@ -26,16 +26,19 @@
         print("These are the files you chose:")
         for i in filenames:
             print(os.path.basename(i))
 
     return filenames
 
 
-def mixcr_(fastq_directory, path_to_mixcr, save_dir, paired_end_sequencing, threads, method, trim_div_by, trim_min_count):
-    filenames = collect_fastq_files(fastq_directory)
+def mixcr_(fastq_directory, path_to_mixcr, save_dir, paired_end_sequencing, threads, method, trim_div_by, trim_min_count, testing = False):
+    if not testing:
+        filenames = collect_fastq_files(fastq_directory)
+    else:
+        filenames = glob(os.path.join(r"C:\Users\nilsh\my_projects\ExpoSeq\tests", "*.fastq"))
     if len(filenames) == 0:
         print("You have not added any fastq files.")
         return
     print("Test Mixcr")
     subprocess.run(["java",
                     "-jar",
                     path_to_mixcr,
```

### Comparing `ExpoSeq-1.0.5/src/ExpoSeq/augment_data/mixcr_nils.py` & `ExpoSeq-1.1.1/src/ExpoSeq/augment_data/mixcr_nils.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,80 +1,102 @@
 import os
 import sys
 from glob import glob
 import subprocess
 from ast import literal_eval
 import pickle
 import pandas as pd
-from ..augment_data.trimming import trimming
+from ExpoSeq.augment_data.trimming import trimming
 import pkg_resources
 try:
     import tkinter as tk
     from tkinter import filedialog
 except:
     pass
 def add_fastq_files():
     filenames = []
     while True:
         try:
-            path_to_files = filedialog.askdirectory()
+            while True:
+                path_to_files = filedialog.askdirectory()
+                if os.path.isdir(path_to_files) == True:
+                    break
+                else:
+                    pass
+            
         except:
             while True:
                 path_to_files = input("copy and paste the path to your directory")
                 if os.path.isdir(os.path.abspath(path_to_files)) == True:
                     break
                 else:
-                    print("Please enter a valid directory")
+                    print("Please enter a valid directory. Dont add a \ to the end of the directory path")
         path_to_files = os.path.abspath(path_to_files)
         filenames.extend(glob(os.path.join(path_to_files, "*.fastq")))
         if len(filenames) == 0:
             user_choice = input("You have not chosen a directory with fastq files. If you want to try again press 1. If you want to cancel the analysis press 2")
             if user_choice == str(1):
                 read_more_files = "Y"
             else:
                 read_more_files = "N"
         else:
             print("These are the files you chose:")
             for i in filenames:
                 print(os.path.basename(i))
-            read_more_files = input("do you want to add another folder? (Y/n)")
-
+            while True:
+                read_more_files = input("do you want to add another folder? (Y/n)")
+                if read_more_files in ["Y" "y", "n", "N"]:
+                    break
+                else:
+                    pass
         if read_more_files == "Y" or read_more_files == "y":
             continue
         else:
             break
     sorted(filenames)
 
     return filenames
 
 
-def process_mixcr(experiment,method, paired_end_sequencing = False):
-    print("Choose the directory where you store your fastq files")
-    filenames = add_fastq_files()
-    if len(filenames) == 0:
-        print("You have not added any fastq files the preprocessing is cancelled now.")
-        return
+def process_mixcr(experiment, method, testing, paired_end_sequencing):
     pkg_path = pkg_resources.resource_filename("ExpoSeq", "")
     module_dir = os.path.abspath("")
+    if not testing:
+        print("Choose the directory where you store your fastq files")
+        while True:
+            filenames = add_fastq_files()
+            if len(filenames) == 0:
+                print("You have not added any fastq files the preprocessing is cancelled now.")
+            else:
+                break
+
+    else:
+
+        filenames = glob(os.path.join(pkg_path,"test_data","test_files", "*.fastq"))
+        print(filenames)
+        experiment = "test_directory"
     settings_dir = os.path.join(pkg_path,
                                 "settings",
                                 "global_vars.txt")
     with open(settings_dir) as f:
         data = f.read()
     data = literal_eval(data)
     path_to_mixcr = data["mixcr_path"]
     if path_to_mixcr == "":
         while True:
             print("choose the mixcr java file with the file chooser")
             try:
                 path_to_mixcr = filedialog.askopenfilename()
             except:
                 path_to_mixcr = input("copy and paste the path to the mixcr jar file here.")
-                if os.path.isdir(os.path.abspath(path_to_mixcr)) == True:
-                    break
+                path_to_mixcr = os.path.normpath(path_to_mixcr)
+            if testing == True:
+                break
+
+            
             try:
                 print("Test Mixcr")
                 subprocess.run(["java",
                                     "-jar",
                                     path_to_mixcr,
                                     "--version"
                                     ])
@@ -89,22 +111,15 @@
                     f.write(str(data))
                 break
     else:
         pass
     #kAligner2_4.0
     #nebnext-human-bcr-cdr3
     #milab-human-tcr-dna-multiplex-cdr3
-    while True:
-        if not os.path.isdir("my_experiments/" + experiment):
 
-            os.mkdir(os.path.join(module_dir, "my_experiments", experiment))
-            os.mkdir(os.path.join(module_dir, "my_experiments", experiment, "alignment_reports"))  # raise error if already exists
-            break
-        else:
-            experiment = input("The given experiment name already exists. Please type another one.")
 
     sequencing_report = pd.DataFrame([])
     if paired_end_sequencing == True:
         filenames_unique_reverse = [unique for unique in filenames if "2.fastq" in unique]
         filenames_unique_forward = [unique for unique in filenames if "1.fastq" in unique]
         combined_filenames = []
         for i in filenames_unique_reverse:
@@ -203,26 +218,28 @@
                                  new_fraction = "clonesFraction")
         sequencing_report = pd.concat([sequencing_report, clones_sample])
         files_to_remove = os.listdir(os.path.join(module_dir, "temp"))
         for file in files_to_remove:
             os.remove(os.path.join(module_dir,
                                    "temp",
                                    file))
-    report_dir = os.path.join(module_dir,
-                              "my_experiments",
-                              experiment,
-                              "sequencing_report.txt")
-    sequencing_report.to_csv(report_dir)
-    data["last_experiment"] = experiment
-    glob_vars_dir = os.path.join(pkg_path,
-                                 "settings",
-                                 "global_vars.txt")
-    with open(glob_vars_dir, "w") as f:
-        f.write(str(data))
-    unique_experiments = sequencing_report["Experiment"].unique()
-    experiment_dic = {item: item for item in list(unique_experiments)}
-    exp_names_dir = os.path.join(module_dir,
-                                 "my_experiments",
-                                 experiment,
-                                 "experiment_names.pickle")
-    with open(exp_names_dir, "wb") as f:
-        pickle.dump(experiment_dic, f)
+    if not testing:
+        report_dir = os.path.join(module_dir,
+                                  "my_experiments",
+                                  experiment,
+                                  "sequencing_report.csv")
+        sequencing_report.to_csv(report_dir)
+        data["last_experiment"] = experiment
+        glob_vars_dir = os.path.join(pkg_path,
+                                     "settings",
+                                     "global_vars.txt")
+        with open(glob_vars_dir, "w") as f:
+            f.write(str(data))
+        unique_experiments = sequencing_report["Experiment"].unique()
+        experiment_dic = {item: item for item in list(unique_experiments)}
+        exp_names_dir = os.path.join(module_dir,
+                                     "my_experiments",
+                                     experiment,
+                                     "experiment_names.pickle")
+        with open(exp_names_dir, "wb") as f:
+            pickle.dump(experiment_dic, f)
+
```

### Comparing `ExpoSeq-1.0.5/src/ExpoSeq/augment_data/randomizer.py` & `ExpoSeq-1.1.1/src/ExpoSeq/augment_data/randomizer.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 import numpy as np
 import random
 import string
-
+import os
 import pandas as pd
 from Bio.Seq import Seq
-
+import pickle
 
 import math
 def create_fractions(num_fractions, top_fraction):
     total_sum = 1
     decrement_factor = math.pow(top_fraction, 1/(num_fractions-1))
 
     # Create a list of fractions that decrease geometrically
@@ -90,35 +90,45 @@
 
 def create_binding_report(sequencing_report, num_antigen):
     threshold_aa_seq = 5
     sampled_df = sequencing_report[~sequencing_report.duplicated(subset='aaSeqCDR3', keep=False)]
     sampled_df = sampled_df.groupby("Experiment").sample(frac = 0.01)
     sampled_df
     sampled_df = sampled_df[sampled_df['aaSeqCDR3'].apply(len) >= threshold_aa_seq]
-    aaSeq = sampled_df.aaSeqCDR3.to_list()
+    aaSeq = sampled_df["aaSeqCDR3"].to_list()
     fractions = sampled_df.clonesFraction
     binding_values = []
     for i in fractions:
         random_binding = random.randint(1000000, 10000000000)
         binding_value = i * random_binding
         binding_values.append(binding_value)
     num_splits = num_antigen
     # generate random indices where the splits should occur
-    split_indices = np.sort(np.random.choice(range(1, len(binding_values)), num_splits-1, replace=False))
+    split_indices = np.sort(np.random.choice(range(1, len(binding_values)), num_splits, replace=False))
     # split the list into random parts
     split_lists = [(binding_values[i:j], aaSeq[i:j]) for i, j in zip([0]+split_indices, split_indices+[len(binding_values)])]
     for i in range(len(split_lists)):
         part_binding = split_lists[i][0]
         part_aaSeq = split_lists[i][1]
         data = {"aaSeqCDR3": part_aaSeq, "Antibody " + str(i): part_binding}
         intermediate_binding = pd.DataFrame(data)
         if i == 0:
             binding_data = intermediate_binding
         else:
             binding_data = pd.merge(binding_data, intermediate_binding,how = "left",on = "aaSeqCDR3")
-
+    
     return binding_data
 
 
-
-
-
+def create_test_dataset():
+    sequencing_report = create_sequencing_report()
+    binding_data = create_binding_report(sequencing_report, 5)
+    binding_data.to_csv(os.path.join(r"C:\Users\nilsh\my_projects\ExpoSeq\src\ExpoSeq\test_data\test_files", "binding_data.csv"))
+    sequencing_report.to_csv(os.path.join(r"C:\Users\nilsh\my_projects\ExpoSeq\src\ExpoSeq\test_data\test_files",  "sequencing_report.csv"))
+    unique_experiments = sequencing_report["Experiment"].unique()
+    experiment_dic = {item: item for item in list(unique_experiments)}
+    exp_names_dir = os.path.join(r"C:\Users\nilsh\my_projects\ExpoSeq\src\ExpoSeq\test_data\test_files",
+                                "experiment_names.pickle")
+    with open(exp_names_dir, "wb") as f:
+        pickle.dump(experiment_dic, f)
+        
+create_test_dataset()
```

### Comparing `ExpoSeq-1.0.5/src/ExpoSeq/augment_data/read_raw_data.py` & `ExpoSeq-1.1.1/src/ExpoSeq/augment_data/read_raw_data.py`

 * *Files identical despite different names*

### Comparing `ExpoSeq-1.0.5/src/ExpoSeq/augment_data/structure_files.py` & `ExpoSeq-1.1.1/src/ExpoSeq/augment_data/structure_files.py`

 * *Files identical despite different names*

### Comparing `ExpoSeq-1.0.5/src/ExpoSeq/augment_data/trimming.py` & `ExpoSeq-1.1.1/src/ExpoSeq/augment_data/trimming.py`

 * *Files identical despite different names*

### Comparing `ExpoSeq-1.0.5/src/ExpoSeq/augment_data/uploader.py` & `ExpoSeq-1.1.1/src/ExpoSeq/augment_data/uploader.py`

 * *Files 17% similar despite different names*

```diff
@@ -1,79 +1,116 @@
+
 from .mixcr_nils import process_mixcr
 from ast import literal_eval
 import os
-from .load_data import collectFiles
 from .loop_collect_reports import load_mixed_files, load_alignment_reports
 import pandas as pd
 from glob import glob
-from .check_reports import check_completeness
+from ExpoSeq.augment_data.check_reports import check_completeness
 import sys
 import pickle
 import pkg_resources
-from .trimming import trimming
+from ExpoSeq.augment_data.trimming import trimming
 try:
     import tkinter as tk
     from tkinter import filedialog
 except:
     pass
+import random
+import string
+import shutil
+
+def get_random_string(length):
+    letters = string.ascii_letters  # this will get all the uppercase and lowercase letters
+    result_str = ''.join(random.choice(letters) for i in range(length))
+    return result_str
 
-def pull_seq_align_repo():
-    try:
-        print("choose the directory where you store your alignment reports and your sequencing report")
-        filenames_dir = filedialog.askdirectory()
+def pull_seq_align_repo(testing, testing_value):
+    if not testing:
+        try:
+            print("choose the directory where you store your alignment reports and your sequencing report")
+            filenames_dir = filedialog.askdirectory()
+            assert os.path.isdir(filenames_dir), "Please enter a valid directory."
+            filenames = glob(filenames_dir + "//*")
+            
+        except:
+            filenames_dir = input(
+                "Enter the directory where you store the alignment reports and your sequencing report manually. You should have one file for the sequencing report and multiple files for the alignment reports.")
+            while True:
+                if os.path.isdir(filenames_dir):
+                    break
+                else:
+                    print("Please enter a valid directory.")
+                    filenames_dir = input(
+                        "Enter the directory where you store the alignment reports and your sequencing report manually. You should have one file for the sequencing report and multiple files for the alignment reports.")
+            filenames_dir = os.path.abspath(filenames_dir + "//*")
+            filenames = glob(filenames_dir)
+    else:
+        module_dir = os.path.abspath("")
+        filenames_dir = os.path.join(module_dir,
+                                    "tests",
+                                    "test_files")
         filenames = glob(filenames_dir + "//*")
-        for i in filenames:
-            if os.path.isdir(i):
-                if "alignment_reports" in i:
-                    alignment_repos = glob(i)
-                    filenames.extend(alignment_repos)
-    except:
-        filenames_dir = input(
-            "Enter the directory where you store the alignment reports and your sequencing report manually.")
-        filenames_dir = os.path.abspath(filenames_dir)
-        filenames = glob(filenames_dir)
-        for i in filenames:
-            if os.path.isdir(i):
-                if "alignment_reports" in i:
-                    alignment_repos = glob(i)
-                    filenames.extend(alignment_repos)
-    sequencing_report, all_alignment_reports = load_mixed_files(filenames)
+    for i in filenames:
+        if os.path.isdir(i):
+            if "alignment_reports" in i:
+                alignment_repos = glob(i)
+                filenames.extend(alignment_repos)
+        sequencing_report, all_alignment_reports = load_mixed_files(filenames, testing, testing_value)
     return sequencing_report, all_alignment_reports
 
-def check_experiment(module_dir):
-    while True:
-        experiment = input("How do you want to call your new experiment?")
-        if os.path.isdir(os.path.join(module_dir, "my_experiments", experiment)) == True:
-            replace = input("The given directory already exists. Do you want to replace it? (Y/n)")
-            if replace in ["Y", "y", "n", "N"]:
-                break
+def check_experiment(module_dir, testing):
+    if not testing:
+        while True:
+            experiment = input("How do you want to call your new experiment?")
+            if os.path.isdir(os.path.join(module_dir, "my_experiments", experiment)) == True:
+                replace = input("The given directory already exists. Do you want to replace it? (Y/n)")
+                if replace in ["Y", "y", "n", "N"]:
+                    break
+                else:
+                    print("Please enter another name.")
             else:
-                print("Please enter another name.")
-        else:
-
-            os.mkdir(os.path.join(module_dir,
-                                       "my_experiments",
-                                       experiment))
-            break
+                break
+    else: 
+        experiment = get_random_string(10)
+    
+    os.mkdir(os.path.join(module_dir,
+                    "my_experiments",
+                    experiment))
     return experiment
 
-def method_one(experiment, repo_path, module_dir):
-    use_method = input(
-        "Per default you will align your data with the following method: milab-human-tcr-dna-multiplex-cdr3 . Press enter if you want to continue. Otherwise type in the method of your choice which. It has to be the exact same string which is given on the Mixcr documentation.")
+def method_one(experiment, repo_path, module_dir, testing, paired_end_test = "n"):
+    if not testing:
+        use_method = input(
+            "Per default you will align your data with the following method: milab-human-tcr-dna-multiplex-cdr3 . Press enter if you want to continue. Otherwise type in the method of your choice which. It has to be the exact same string which is given on the Mixcr documentation.")
+    else:
+        use_method = ""
     if use_method == "":
         method = "milab-human-tcr-dna-multiplex-cdr3"
     else:
         method = use_method
-    paired_end = input("Do you want to analyze paired_end_sequencing data? (Y/n)")
+    if not testing:
+        paired_end = input("Do you want to analyze paired_end_sequencing data? (Y/n)")
+        
+    else: 
+        paired_end = 'n'
+    while True:
+        if paired_end in ["Y", "y", "n", "N"]:
+            break
+        else:
+            print("Please enter a correct value.")
+            paired_end = input("Do you want to analyze paired_end_sequencing data? (Y/n)")
     if paired_end.lower() in ["Y", "y"]:
         paired_end = True
     else:
         paired_end = False
+
     process_mixcr(experiment,
                   method=method,
+                  testing = testing,
                   paired_end_sequencing=paired_end)
 
     with open(repo_path, "rb") as f:
         sequencing_report = pd.read_table(f, sep=",")
     try:
         align_repo_path = os.path.join(module_dir,
                                        "my_experiemnts",
@@ -83,34 +120,36 @@
         alignment_reports = glob(align_repo_path)
         all_alignment_reports = load_alignment_reports(alignment_reports)
     except:
         all_alignment_reports = pd.DataFrame([])
         print(
             "No alignment reports could be found in " + experiment + ". You will continue without being able to analyze the Alignment Quality.")
     return sequencing_report, all_alignment_reports
-def method_two(module_dir, experiment):
+def method_two(module_dir, experiment, testing = False, testing_value = None):
 
     print("Choose the folder which contains the sequencing_report and the alignment reports.")
 
-    sequencing_report, all_alignment_reports = pull_seq_align_repo()
+    sequencing_report, all_alignment_reports = pull_seq_align_repo(testing, testing_value)
 
     while True:
         if sequencing_report.shape[0] == 0:
             print(
-                "Something went wrong. Unfortunately you could not collect the data in the sequencing report. Please make sure that you have chosen the right directory and that you have tsv files as output from mixcr in that directory.")
-            sequencing_report, all_alignment_reports = pull_seq_align_repo()
+                "Something went wrong. Unfortunately you could not collect the data in the sequencing report.")
+            sequencing_report, all_alignment_reports = pull_seq_align_repo(testing, testing_value)
         else:
             break
         #  sys.exit()
-    while True:
-        trim_data = input("Do you need to trim your data? (Y/n)")
-        if trim_data in ["Y", "y", "n", "N"]:
-            break
-        else:
-            print("Please enter a correct value.")
+    if not testing:
+        while True:
+            trim_data = input("Do you need to trim your data? (Y/n)")
+            if trim_data in ["Y", "y", "n", "N"]:
+                break
+            else:
+                print("Please enter a correct value.")
+    else: trim_data = "Y"
     if trim_data.lower() in ["Y", "y"]:
         sequencing_report = trimming(sequencing_report,
                                      divisible_by=3,  # might be possible that columns are different
                                      min_count=1,
                                      new_fraction="cloneFraction")
     else:
         pass
@@ -144,129 +183,193 @@
     unique_experiments = sequencing_report["Experiment"].unique()
     experiment_dic = {item: item for item in list(unique_experiments)}
 
     with open(exp_name_path, "wb") as f:
         pickle.dump(experiment_dic, f)
     return sequencing_report, all_alignment_reports
 
-def method_three():
-    try:
-        print("choose the file where you store your sequencing report")
-        f = filedialog.askopenfilename()
-        sequencing_report = pd.read_table(f, sep=",")
-    except:
-        while True:
+def method_three(module_dir, experiment, testing ):
+    if not testing:
+        try:
+            print("choose the file where you store your sequencing report")
+            while True:
+                f = filedialog.askopenfilename()
+                if os.path.isfile(f):
+                    break
+                else:
+                    print("Please enter a valid file path")
+        except:
             f = input("give the path to your file which is the sequencing report")
             f = os.path.abspath(f)
-            if os.path.isfile(f):
-                sequencing_report = pd.read_table(f, sep=",")
+            while True:
+                if os.path.isfile(f):
+                    break
+                else:
+                    print("Please enter a valid file path")
+    else:
+
+        f = os.path.join(module_dir,
+                        "my_experiments",
+                        "test_directory",
+                        "sequencing_report.csv")
+        experiment = "test_directory"
+    while True:
+        sequencing_report = pd.read_table(f, sep=",")
+        if os.path.isfile(f) :
+            sequencing_report = pd.read_table(f, sep=",")
+            if "Experiment" in sequencing_report:
+                exp_name_path = os.path.join(module_dir,
+                                            "my_experiments",
+                                            experiment,
+                                            "experiment_names.pickle")
+
+                unique_experiments = sequencing_report["Experiment"].unique()
+                experiment_dic = {item: item for item in list(unique_experiments)}
+                with open(exp_name_path, "wb") as f:
+                    pickle.dump(experiment_dic, f)
                 break
             else:
-                print("Sorry, but the filepath you entered is invalid.")
+                print("Sorry, but we could not find the column Experiment in your sequencing report. Please check if you have this")
+        else:
+            print("Sorry, but the filepath you entered is invalid.")
     all_alignment_reports = None
-    return sequencing_report,all_alignment_reports
 
-def check_last_exp(pkg_path, module_dir):
-    glob_vars = os.path.join(pkg_path,
-                             "settings",
-                             "global_vars.txt")
-    with open(glob_vars, "r") as f:
-        data = f.read()
-    data = literal_eval(data)
-
-    last_experiment = data["last_experiment"]
-    repo_path = os.path.join(module_dir,
-                             "my_experiments",
-                             "last_experiment",
-                             "sequencing_report.txt")
+    return sequencing_report,all_alignment_reports, experiment
+
+def check_last_exp(pkg_path, module_dir, testing):
+    if not testing:
+        glob_vars = os.path.join(pkg_path,
+                                "settings",
+                                "global_vars.txt")
+        with open(glob_vars, "r") as f:
+            data = f.read()
+        data = literal_eval(data)
+
+        last_experiment = data["last_experiment"]
+        if last_experiment == "":
+            print("You have no experiments in your folder.")
+            repo_path = ""
+        else:
+            repo_path = os.path.join(module_dir,
+                                    "my_experiments",
+                                    last_experiment,
+                                    "sequencing_report.csv")
+    else:
+        repo_path = os.path.join(module_dir,
+                                "my_experiments",
+                                "test_directory",
+                                "sequencing_report.csv")
+        last_experiment = "test_directory"
     return repo_path, last_experiment
-def upload():
-    module_dir = os.path.abspath("")
-    pkg_path = pkg_resources.resource_filename("ExpoSeq", "")
-    repo_path, last_experiment = check_last_exp(pkg_path, module_dir)
+def get_continue_analysis_input(last_experiment, testing=False, testing_value = None):
+    if not testing:
+        continue_input = input("Do you want to continue to analyze with " + last_experiment + "? Y/n")
+    else:
+        continue_input = testing_value
+    return continue_input
 
-    if os.path.isfile(repo_path):
-        continue_analysis = input("Do you want to continue to analyze with " + last_experiment + "? Y/n")
-        if continue_analysis.lower() in ["n", "N"]:
-            next_step = input("If you want to upload a new experiment press 1. If you want to choose another experiment press 2")
-            if next_step == "1":
-                experiment = check_experiment(module_dir)
+def get_next_step_input(testing=False, testing_value = None):
+    if not testing:
+        next_step = input("If you want to upload a new experiment press 1. If you want to choose another experiment press 2. ")
+    else:
+        next_step = testing_value
+    return next_step
 
-                choose_method = input("If you want to process your data with mixcr press 1. If you want to upload already processed txt files with unique clones, press 2")
-                if choose_method == "1":
-                    sequencing_report, all_alignment_reports = method_one(experiment, repo_path, module_dir)
-                if choose_method == "2":
-                    sequencing_report, all_alignment_reports = method_two(module_dir, experiment)
-
-
-                if choose_method == "3":
-                    sequencing_report, all_alignment_reports = method_three()
-
-            if next_step == "2":
-                while True:
-                    user_input = input("Enter the name of the experiment you want to analyze")
-
-                    user_input = user_input  # Try to convert the input to an integer
-                    spec_exp_name_path = os.path.join(module_dir,
-                                                      "my_experiments",
-                                                      user_input)
-                    if os.path.isdir(spec_exp_name_path):  # Check if the input is in the correct range
-                        break  # If the input is valid, break out of the loop
-                    else:
-                        print("The experiment name does not exist in my_experiments. Please enter the correct name")
-                experiment = user_input
-                seq_report_path = os.path.join(module_dir,
-                                               "my_experiments",
-                                               experiment,
-                                               "sequencing_report.txt")
-                with open(seq_report_path, "rb") as f:
-                    sequencing_report = pd.read_table(f, sep=",")
-                try:
-                    align_repo_path = os.path.join(module_dir,
-                                                   "my_experiments",
-                                                   experiment,
-                                                   "alignment_reports",
-                                                   "*")
-                    alignment_reports = glob(align_repo_path)
-                    all_alignment_reports = load_alignment_reports(alignment_reports)
-                except:
-                    all_alignment_reports = pd.DataFrame([])
-                    print(
-                        "No alignment reports could be found in " + experiment + ". You will continue without being able to analyze the Alignment Quality.")
+def get_choose_method_input(testing, testing_value = None):
+    if not testing:
+        processing = input("If you want to process your fastq files with mixcr press 1. If you want to upload already processed txt files with unique clones, press 2. If you want to upload an already processed sequencing report in table format, press 3.")
+    else:
+        processing = testing_value
+    return processing
 
+def get_experiment_name_input(testing = False):
+    if not testing:
+        experiment_name = input("Enter the name of the experiment you want to analyze")
+    else:
+        experiment_name = get_random_string(10)
+    return experiment_name  
+
+def upload_new_experiment(module_dir, repo_path, testing, testing_value, paired_end_test, experiment_column):
+    experiment = check_experiment(module_dir, testing)
+    choose_method = get_choose_method_input(testing, testing_value)
+    
+    if choose_method == "1":
+        
+        sequencing_report, all_alignment_reports = method_one(experiment, repo_path,module_dir,testing, paired_end_test )
+    elif choose_method == "2":
+        sequencing_report, all_alignment_reports = method_two(module_dir, experiment,testing, experiment_column)
+    elif choose_method == "3":
+        sequencing_report, all_alignment_reports, experiment = method_three(module_dir, experiment, testing)
+    else:
+        raise ValueError("Invalid option")
+
+    return sequencing_report, all_alignment_reports, experiment
+
+def choose_existing_experiment(module_dir, testing):
+    if not testing:
+        while True:
+            user_input = get_experiment_name_input()
+            spec_exp_name_path = os.path.join(module_dir, "my_experiments", user_input)
+            if os.path.isdir(spec_exp_name_path): 
+                break
             else:
-                pass
-        else:
-            experiment = last_experiment
-            seq_report_path = os.path.join(module_dir,
-                                           "my_experiments",
-                                           experiment,
-                                           "sequencing_report.txt")
-            with open(seq_report_path, "rb") as f:
-                sequencing_report = pd.read_table(f, sep=",")
-            try:
-                align_repo_path = os.path.join(module_dir,
-                                               "my_experiments",
-                                               experiment,
-                                               "alignment_reports",
-                                               "*")
-                alignment_reports = glob(align_repo_path)
-                all_alignment_reports = load_alignment_reports(alignment_reports)
-            except:
-                all_alignment_reports = pd.DataFrame([])
-                print(
-                    "No alignment reports could be found in " + experiment + ". You will continue without being able to analyze the Alignment Quality.")
+                print("The experiment name does not exist in my_experiments. Please enter the correct name")
+    else:
+        user_input = "test_directory"
+    return user_input  # experiment
+
 
+
+def retrieve_reports(module_dir, experiment, testing):
+    if not testing:
+        seq_report_path = os.path.join(module_dir, "my_experiments", experiment, "sequencing_report.csv")
+        align_repo_path = os.path.join(module_dir,
+                            "my_experiments",
+                            experiment,
+                            "alignment_reports", "*")
     else:
+        seq_report_path = os.path.join(module_dir, "my_experiments", "test_directory", "sequencing_report.csv")
+        align_repo_path = os.path.join(module_dir, "tests", "test_directory", "all_alignment_reports.pickle")
+    with open(seq_report_path, "rb") as f:
+        sequencing_report = pd.read_table(f, sep=",")
+    try:
+        align_repo_path = os.path.join(module_dir,
+                                    "my_experiments",
+                                    experiment,
+                                    "alignment_reports", "*")
+        alignment_reports = glob(align_repo_path)
+        all_alignment_reports = load_alignment_reports(alignment_reports)
+    except:
+        all_alignment_reports = pd.DataFrame([])
+        print("No alignment reports could be found in " + experiment + ". You will continue without being able to analyze the Alignment Quality.")
 
-        choose_method = input("Welcome to ExpoSeq. If you want to start by processing your fastq files with mixcr press 1. If you want to upload already processed files press 2. If you want to upload a sequencing report press 3.")
-        experiment = check_experiment(module_dir)
-        if choose_method == "1":
-            sequencing_report, all_alignment_reports = method_one(experiment, repo_path, module_dir)
-        else:
-            pass
-        if choose_method == "2":
-            sequencing_report, all_alignment_reports = method_two(module_dir, experiment)
-        if choose_method == "3":
-            sequencing_report, all_alignment_reports = method_three()
+    return sequencing_report, all_alignment_reports, experiment
 
-    return sequencing_report, all_alignment_reports, experiment
+def process_data_with_last_experiment(module_dir, last_experiment, testing):
+    experiment = last_experiment
+    sequencing_report, all_alignment_reports = retrieve_reports(module_dir, experiment, testing)
+    return sequencing_report, all_alignment_reports, experiment
+
+def upload(testing=False, continue_analysis = "n", upload_type = "2", choose_exp = '1', paired_end_test = 'n', experiment_column = '1'):
+   # module_dir = os.path.abspath("")
+    module_dir = os.getcwd()
+    pkg_path = pkg_resources.resource_filename("ExpoSeq", "")
+    repo_path, last_experiment = check_last_exp(pkg_path, module_dir, testing)
+
+    if os.path.isfile(repo_path):
+        continue_analysis = get_continue_analysis_input(last_experiment, testing,continue_analysis)
+        if continue_analysis.lower() in ["n", "no"]:
+            next_step = get_next_step_input(testing, choose_exp)
+            if next_step == "1":
+                sequencing_report, all_alignment_reports, experiment = upload_new_experiment(module_dir,repo_path, testing, upload_type, paired_end_test, experiment_column)
+            elif next_step == "2":
+                experiment = choose_existing_experiment(module_dir, testing)
+                sequencing_report, all_alignment_reports, experiment = retrieve_reports(module_dir, experiment, testing)
+            else:
+                raise ValueError("Invalid option")
+        else:
+            sequencing_report, all_alignment_reports, experiment = process_data_with_last_experiment(module_dir, last_experiment, testing)
+    else:
+        sequencing_report, all_alignment_reports, experiment = upload_new_experiment(module_dir, repo_path, testing, upload_type, paired_end_test, experiment_column)
+    if testing and experiment != "test_directory":
+        shutil.rmtree(os.path.join(module_dir, "my_experiments", experiment))
+    return sequencing_report, all_alignment_reports, experiment
```

### Comparing `ExpoSeq-1.0.5/src/ExpoSeq/pipeline.py` & `ExpoSeq-1.1.1/src/ExpoSeq/pipeline.py`

 * *Files 4% similar despite different names*

```diff
@@ -14,83 +14,70 @@
 from .augment_data.uploader import upload
 from ast import literal_eval
 from .settings.plot_styler import PlotStyle
 import pandas as pd
 import pickle
 import pkg_resources
 import os
-from .settings.change_save_settings import Change_save_settings
-from .augment_data.randomizer import create_sequencing_report, create_binding_report
-
+from ExpoSeq.settings.change_save_settings import Change_save_settings
+from ExpoSeq.augment_data.randomizer import create_sequencing_report, create_binding_report
+from ExpoSeq.reset import original_settings
+import shutil
 
 class PlotManager:
     def __init__(self, test_version = False):
+        self.is_test = test_version
         self.module_dir = os.path.abspath("")
         self.pkg_path = pkg_resources.resource_filename("ExpoSeq", "")
-        if os.path.isdir(os.path.join(self.module_dir, "my_experiments")):
-            pass
-        else:
-            os.mkdir(os.path.join(self.module_dir, "my_experiments"))
-        if os.path.isdir(os.path.join(self.module_dir, "temp")):
-            pass
+        #self.module_dir = r"C:\Users\nilsh\my_projects\ExpoSeq\src\ExpoSeq" ## has to be changed
+        #self.pkg_path = r"C:\Users\nilsh\my_projects\ExpoSeq\src\ExpoSeq"
+        common_vars_path = os.path.join(self.pkg_path,
+                                        "settings",
+                                        "global_vars.txt")
+        with open(common_vars_path, "r") as f:
+            self.global_params = f.read()
+        self.global_params = literal_eval(self.global_params)
+        print(self.global_params)
+        if test_version == True:
+            if os.path.isdir(os.path.join(self.module_dir, "my_experiments")):
+                pass
+            else:
+                os.mkdir(os.path.join(self.module_dir, "my_experiments"))
+            if os.path.isdir(os.path.join(self.module_dir, "temp")):
+                pass
+            else:
+                os.mkdir(os.path.join(self.module_dir, "temp"))
+                
+            self.experiment = "Test"
+            self.sequencing_report = create_sequencing_report(num_experiments = 3,
+                                                              panning_rounds = 1,
+                                                              )
+            self.unique_experiments = self.sequencing_report["Experiment"].unique().tolist()
+            self.unique_experiments = dict(zip(self.unique_experiments, self.unique_experiments))
+            self.alignment_report = None
+            self.sequencing_report["Experiment"] = self.sequencing_report["Experiment"].map(self.unique_experiments)
+            self.binding_data = create_binding_report(self.sequencing_report,
+                                                      num_antigen = 1)
+            
         else:
-            os.mkdir(os.path.join(self.module_dir, "temp"))
-        if test_version == False:
-
             self.sequencing_report, self.alignment_report, self.experiment = upload()
             experiment_path = os.path.join(self.module_dir,
-                                           "my_experiments",
-                                           self.experiment,
-                                           "experiment_names.pickle")
+                                            "my_experiments",
+                                            self.experiment,
+                                            "experiment_names.pickle")
             with open(experiment_path, "rb") as f:
                 self.unique_experiments = pickle.load(f)
             self.sequencing_report["Experiment"] = self.sequencing_report["Experiment"].map(self.unique_experiments)
             self.add_binding = input("Do you have binding Data? Y/n")
             if self.add_binding.lower() in ["Y", "y"]:
                 self.binding_data = collect_binding_data()
             else:
                 self.binding_data = None
-        else:
-            self.experiment = "Test"
-            self.sequencing_report = create_sequencing_report()
-          #  report_path = os.path.join(self.pkg_path,
-         #                              "test_data",
-           #                            "sequencing_report.csv")
-           # with open(report_path, "rb") as f:
-            #    self.sequencing_report = pd.read_csv(f, sep=",")
-           # with open("test_data/sequencing_report.csv", "rb") as f:
-            #    self.sequencing_report = pd.read_csv(f, sep = ",")
-            common_vars_path = os.path.join(self.pkg_path,
-                                            "settings",
-                                            "global_vars.txt")
-            with open(common_vars_path, "r") as f:
-                self.global_params = f.read()
-            self.global_params = literal_eval(self.global_params)
-      #      experiment_names_path = os.path.join(self.pkg_path,
-       #                                          "test_data"
-        #                                         , "experiment_names.pickle")
-            self.unique_experiments = self.sequencing_report["Experiment"].unique().tolist()
-            self.unique_experiments = dict(zip(self.unique_experiments, self.unique_experiments))
-            #with open(experiment_names_path, "rb") as f:
-             #   self.unique_experiments = pickle.load(f)
-           # alignments_repos_path = os.path.join(self.pkg_path,
-            #                                     "test_data",
-             #                                    "all_alignment_reports.pickle")
-         #   with open(alignments_repos_path, "rb") as f:
-          #      self.alignment_report = pickle.load(f)
-            self.alignment_report = None
-            self.sequencing_report["Experiment"] = self.sequencing_report["Experiment"].map(self.unique_experiments)
-            self.binding_data = create_binding_report(self.sequencing_report,
-                                                      num_antigen = 5)
-     #       binding_data_path = os.path.join(self.pkg_path,
-      #                                       "/test_data",
-       #                                      "binding_data.txt")
-        #    self.binding_data = pd.read_table(binding_data_path, sep=",")
-         #   self.binding_data.drop(self.binding_data.columns[0], axis=1, inplace=True)
-
+                
+                
         font_settings_path = os.path.join(self.pkg_path,
                                           "settings",
                                           "font_settings.txt")
         with open(font_settings_path, "r") as f:
             font_settings = f.read()
         self.font_settings = literal_eval(font_settings)
         legend_settings_path = os.path.join(self.pkg_path,
@@ -136,15 +123,15 @@
     def add_binding_data(self):
         self.binding_data = collect_binding_data(binding_data = self.binding_data)
     def print_antigens(self):
         """
         :return: prints the antigens (columns) of your binding data
         """
         try:
-            print(self.binding_data.columns.to_list()[1:-1])
+            print(self.binding_data.columns.to_list()[1:])
         except:
             print("You have not given binding data.")
     def print_samples(self):
         """
         :return: prints the names of your samples, so you can insert them in lists or similar for the analysis with some plots
         """
         print(list(self.unique_experiments.values()))
@@ -271,26 +258,28 @@
         self.style = PlotStyle(self.ax, self.plot_type)
         figManager = plt.get_current_fig_manager()
         figManager.window.showMaximized()
 
 
     def logoPlot_multi(self,
                  samples = "all",
-                 chosen_seq_length = 16):
+                 chosen_seq_length = 16,
+                    ):
         """
         :param samples: You analyze ExpoSeq samples per default. If you want to analyze specific samples it has to be a list with the corresponding sample names
         :param chosen_seq_length: 16 per default. You always analyze online one sequence length! You can change it if you would like
         :return: Gives you in one figure one logoPlot per sample.
         """
         self.fig.clear()
         plot_logo_multi(self.fig,
                   self.sequencing_report,
                   samples,
                   self.font_settings,
-                  chosen_seq_length
+                  chosen_seq_length,
+                    test_version = self.is_test
                   )
 
         self.plot_type = "multi"
         self.ax= self.fig.gca()
         self.style = PlotStyle(self.ax, self.plot_type)
         figManager = plt.get_current_fig_manager()
         figManager.window.showMaximized()
@@ -320,15 +309,16 @@
         :param samples: You analyze ExpoSeq samples per default. If you want to analyze specific samples it has to be a list with the corresponding sample names
         :return: Outputs one figurewith one subplot per sample which shows you the distribution of sequence length
         """
         self.fig.clear()
         length_distribution_multi(self.fig,
                             self.sequencing_report,
                             samples,
-                            font_settings=self.font_settings)
+                            font_settings=self.font_settings,
+                                test_version = self.is_test)
         self.plot_type = "multi"
         self.ax = self.fig.gca()
         self.style = PlotStyle(self.ax, self.plot_type)
         figManager = plt.get_current_fig_manager()
         figManager.window.showMaximized()
         plt.tight_layout()
 
@@ -560,14 +550,21 @@
                      specific_experiments = specific_samples,
                      )
         self.plot_type = "single"
         self.ax = self.fig.gca()
         self.style = PlotStyle(self.ax, self.plot_type)
         figManager = plt.get_current_fig_manager()
         figManager.window.showMaximized()
+        
+
+
+
+
+
+
```

### Comparing `ExpoSeq-1.0.5/src/ExpoSeq/plots/barplot.py` & `ExpoSeq-1.1.1/src/ExpoSeq/plots/barplot.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 import matplotlib.pyplot as plt
-from ..tidy_data.barplot import cleaning_data
+from ExpoSeq.tidy_data.barplot import cleaning_data
 import numpy as np
 import matplotlib
 
 def barplot(ax, all_alignment_reports, sequencing_report_all,font_settings, legend_settings, apply_log):
     matplotlib.use("Qt5Agg")
     boxplot_data_frame = cleaning_data(all_alignment_reports,
                                        sequencing_report_all)
```

### Comparing `ExpoSeq-1.0.5/src/ExpoSeq/plots/cluster_embedding.py` & `ExpoSeq-1.1.1/src/ExpoSeq/plots/cluster_embedding.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 import pandas as pd
-from ..tidy_data.tidy_cluster_embedding import tidy_embed
+from ExpoSeq.tidy_data.tidy_cluster_embedding import tidy_embed
 
 def show_difference(sequencing_report, list_experiments,strands, batch_size, pca_components, perplexity, iterations_tsne, ax, legend_settings, font_settings):
     tsne_results, aminoacids, experiments_batch = tidy_embed(sequencing_report,
                                                               batch_size,
                                                               list_experiments,
                                                               pca_components,
                                                               perplexity,
```

### Comparing `ExpoSeq-1.0.5/src/ExpoSeq/plots/embedding_with_binding.py` & `ExpoSeq-1.1.1/src/ExpoSeq/plots/embedding_with_binding.py`

 * *Files identical despite different names*

### Comparing `ExpoSeq-1.0.5/src/ExpoSeq/plots/length_distribution.py` & `ExpoSeq-1.1.1/src/ExpoSeq/plots/length_distribution.py`

 * *Files 8% similar despite different names*

```diff
@@ -20,27 +20,30 @@
     original_fontsize = font_settings["fontsize"]
     font_settings["fontsize"] = 22
     plt.title("Length Distribution of " + sample, pad=12, **font_settings)
     font_settings["fontsize"] = original_fontsize
 
 
 
-def length_distribution_multi(fig, sequencing_report, samples, font_settings):
+def length_distribution_multi(fig, sequencing_report, samples, font_settings, test_version = False):
     if samples == "all":
         unique_experiments = sequencing_report["Experiment"].unique()
         unique_experiments = np.sort(unique_experiments)
     else:
         sequencing_report = sequencing_report[sequencing_report['Experiment'].isin(samples)]
         unique_experiments = sequencing_report["Experiment"].unique()
         unique_experiments = np.sort(unique_experiments)
 
     # Subplots are organized in a Rows x Cols Grid
     # Tot and Cols are known
     Tot = unique_experiments.shape[0]
-    Cols = int(input("How many Rows for the Plots do you want?"))
+    if not test_version:
+        Cols = int(input("How many Rows for the Plots do you want?"))
+    else:
+        Cols = 6
     # Compute Rows required
     Rows = Tot // Cols
     #     EDIT for correct number of rows:
     #     If one additional row is necessary -> add one:
     if Tot % Cols != 0:
         Rows += 1
     # Create a Position index
```

### Comparing `ExpoSeq-1.0.5/src/ExpoSeq/plots/levenshtein_clustering.py` & `ExpoSeq-1.1.1/src/ExpoSeq/plots/levenshtein_clustering.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 import matplotlib.pyplot as plt
 from numpy import unique
 import networkx
 import math
 import pandas as pd
-from ..tidy_data.clustering import cleaning
+from ExpoSeq.tidy_data.clustering import cleaning
 
 
 def clusterSeq(ax, sequencing_report, sample,max_ld, min_ld, batch_size, font_settings, second_figure):
     sample_report = sequencing_report[sequencing_report["Experiment"] == sample] ## insert test if sample not found
     sample_report = sample_report.head(batch_size)
     G, degree_sequence = cleaning(sample_report, max_ld, min_ld)
     # Create a gridspec for adding subplots of different sizes
```

### Comparing `ExpoSeq-1.0.5/src/ExpoSeq/plots/logo_plot.py` & `ExpoSeq-1.1.1/src/ExpoSeq/plots/logo_plot.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 import matplotlib.pyplot as plt
 import logomaker
-from ..tidy_data.tidy_seqlogoPlot import cleaning
+from ExpoSeq.tidy_data.tidy_seqlogoPlot import cleaning
 import numpy as np
 
 def plot_logo_single(ax, sequencing_report, sample, font_settings, highlight_specific_pos, highlight_pos_range, chosen_seq_length = 16):
     aa_distribution, sequence_length, length_filtered_seqs = cleaning(sample,
                                                                       sequencing_report,
                                                                       chosen_seq_length)
     logo_plot = logomaker.Logo(aa_distribution,
@@ -26,24 +26,27 @@
                                      alpha=.5)
     if highlight_pos_range != False:
         logo_plot.ax.highlight_position_range(pmin=3,
                                               pmax=5,
                                               color="lightcyan")
 
 
-def plot_logo_multi(fig, sequencing_report, samples,font_settings, chosen_seq_length = 16):
+def plot_logo_multi(fig, sequencing_report, samples,font_settings, chosen_seq_length = 16, test_version = False):
     if samples == "all":
         unique_experiments = sequencing_report["Experiment"].unique()
         unique_experiments = np.sort(unique_experiments)
     else:
         unique_experiments = sequencing_report["Experiment"].unique()
         unique_experiments = np.array([i for i in unique_experiments if i in samples])
         unique_experiments = np.sort(unique_experiments)
     Tot = unique_experiments.shape[0]
-    Cols = int(input("How many Columns for the Plots do you want?"))
+    if not test_version:
+        Cols = int(input("How many Columns for the Plots do you want?"))
+    else: 
+        Cols = 6
     # Compute Rows required
     Rows = Tot // Cols
     if Tot % Cols != 0:
         Rows += 1
     # Create a Position index
     Position = range(1, Tot + 1)
     n = 0
```

### Comparing `ExpoSeq-1.0.5/src/ExpoSeq/plots/plt_heatmap.py` & `ExpoSeq-1.1.1/src/ExpoSeq/plots/plt_heatmap.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 import matplotlib
 import matplotlib.pyplot as plt
 import seaborn as sns
-from ..tidy_data.heatmaps import tidy_jaccard, tidy_sorensen, tidy_morosita_horn, tidy_heatmap_share
+from ExpoSeq.tidy_data.heatmaps import tidy_jaccard, tidy_sorensen, tidy_morosita_horn, tidy_heatmap_share
 
 import numpy as np
 
 def plot_heatmap(sequencing_report, protein, heatmap, ax, colorbar_settings, font_settings, specific_experiments = False):
 
     if heatmap == "morosita_horn":
         unique_sequences, unique_experiments = tidy_morosita_horn.cleaning_data(sequencing_report,
```

### Comparing `ExpoSeq-1.0.5/src/ExpoSeq/plots/protvec.py` & `ExpoSeq-1.1.1/src/ExpoSeq/plots/protvec.py`

 * *Files identical despite different names*

### Comparing `ExpoSeq-1.0.5/src/ExpoSeq/plots/relative_sequence_abundance.py` & `ExpoSeq-1.1.1/src/ExpoSeq/plots/relative_sequence_abundance.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-from ..tidy_data.tidy_rel_sequence_abun import cleaning
+from ExpoSeq.tidy_data.tidy_rel_sequence_abun import cleaning
 def relative_sequence_abundance(ax, sequencing_report, samples,max_levenshtein_distance,length_filter,batch, font_settings, legend_settings):
     all_samples = cleaning(sequencing_report,
                             max_levenshtein_distance,
                             samples,
                             length_filter,
                             batch)
     x_vals = all_samples.index.to_list()
```

### Comparing `ExpoSeq-1.0.5/src/ExpoSeq/plots/saveFig.py` & `ExpoSeq-1.1.1/src/ExpoSeq/plots/saveFig.py`

 * *Files identical despite different names*

### Comparing `ExpoSeq-1.0.5/src/ExpoSeq/plots/stacked_aa_distribution.py` & `ExpoSeq-1.1.1/src/ExpoSeq/plots/stacked_aa_distribution.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-from ..tidy_data.tidy_stacked_aa_distr import cleaning
+from ExpoSeq.tidy_data.tidy_stacked_aa_distr import cleaning
 import matplotlib.pyplot as plt
 
 def stacked_aa_distr(ax, sequencing_report, sample, region, protein, font_settings, legend_settings):
     aa_distribution = cleaning(sequencing_report, sample, region, protein)
     aa_distribution.plot(kind='bar', stacked=True, ax = ax)
     ax.set_xlabel('Position on amino acid sequence', **font_settings)
     if protein == True:
```

### Comparing `ExpoSeq-1.0.5/src/ExpoSeq/plots/usq_plot.py` & `ExpoSeq-1.1.1/src/ExpoSeq/plots/usq_plot.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-from ..tidy_data.tidy_USQ_plot_ import cleaning_data
+from ExpoSeq.tidy_data.tidy_USQ_plot_ import cleaning_data
 import matplotlib.pyplot as plt
 import random
 from collections import Counter
 import warnings
 import matplotlib
 matplotlib.use('Qt5Agg')
 def plot_USQ(fig, sequencing_report, samples, font_settings, legend_settings):
```

### Comparing `ExpoSeq-1.0.5/src/ExpoSeq/reset.py` & `ExpoSeq-1.1.1/src/ExpoSeq/reset.py`

 * *Files identical despite different names*

### Comparing `ExpoSeq-1.0.5/src/ExpoSeq/settings/blosum_62.txt` & `ExpoSeq-1.1.1/src/ExpoSeq/settings/blosum_62.txt`

 * *Files identical despite different names*

### Comparing `ExpoSeq-1.0.5/src/ExpoSeq/settings/change_save_settings.py` & `ExpoSeq-1.1.1/src/ExpoSeq/settings/change_save_settings.py`

 * *Files 7% similar despite different names*

```diff
@@ -18,26 +18,32 @@
             save_settings = f.read()
         self.save_settings = literal_eval(save_settings)
     def change_dpi(self, dpi):
         self.save_settings["dpi"] = dpi
         with open(self.save_settings_path, "w") as f:
             f.write(str(self.save_settings))
     def change_save_path(self, path = None):
-        if path == True:
+        if path == None:
             try:
                 self.save_settings["fname"] = filedialog.askopenfilename()
             except:
                 while True:
                     save_dir = input("copy and paste the path to the directory where you want to save your plots")
                     if os.path.isdir(os.path.abspath(save_dir)):
                         self.save_settings["fname"] = save_dir
                         break
                     else:
                         print("Try again and input a valid directory")
         else:
             self.save_settings["fname"] = path
+            print("The new path you safe your results in is: " + path)
         with open(self.save_settings_path, "w") as f:
             f.write(str(self.save_settings))
+
     def change_format(self, format):
         self.save_settings["format"] = format
         with open(self.save_settings_path, "w") as f:
-            f.write(str(self.save_settings))
+            f.write(str(self.save_settings))
+
+    def print_save_path(self):
+        print(self.save_settings["fname"])
+
```

### Comparing `ExpoSeq-1.0.5/src/ExpoSeq/settings/plot_styler.py` & `ExpoSeq-1.1.1/src/ExpoSeq/settings/plot_styler.py`

 * *Files identical despite different names*

### Comparing `ExpoSeq-1.0.5/src/ExpoSeq/tidy_data/aminoacid_distribution.py` & `ExpoSeq-1.1.1/src/ExpoSeq/tidy_data/aminoacid_distribution.py`

 * *Files identical despite different names*

### Comparing `ExpoSeq-1.0.5/src/ExpoSeq/tidy_data/barplot.py` & `ExpoSeq-1.1.1/src/ExpoSeq/tidy_data/barplot.py`

 * *Files identical despite different names*

### Comparing `ExpoSeq-1.0.5/src/ExpoSeq/tidy_data/clustering.py` & `ExpoSeq-1.1.1/src/ExpoSeq/tidy_data/clustering.py`

 * *Files identical despite different names*

### Comparing `ExpoSeq-1.0.5/src/ExpoSeq/tidy_data/heatmaps/bool_sequences_matrix.py` & `ExpoSeq-1.1.1/src/ExpoSeq/tidy_data/heatmaps/bool_sequences_matrix.py`

 * *Files identical despite different names*

### Comparing `ExpoSeq-1.0.5/src/ExpoSeq/tidy_data/heatmaps/tidy_heatmap_share.py` & `ExpoSeq-1.1.1/src/ExpoSeq/tidy_data/heatmaps/tidy_heatmap_share.py`

 * *Files identical despite different names*

### Comparing `ExpoSeq-1.0.5/src/ExpoSeq/tidy_data/heatmaps/tidy_jaccard.py` & `ExpoSeq-1.1.1/src/ExpoSeq/tidy_data/heatmaps/tidy_jaccard.py`

 * *Files identical despite different names*

### Comparing `ExpoSeq-1.0.5/src/ExpoSeq/tidy_data/heatmaps/tidy_morosita_horn.py` & `ExpoSeq-1.1.1/src/ExpoSeq/tidy_data/heatmaps/tidy_morosita_horn.py`

 * *Files identical despite different names*

### Comparing `ExpoSeq-1.0.5/src/ExpoSeq/tidy_data/heatmaps/tidy_sorensen.py` & `ExpoSeq-1.1.1/src/ExpoSeq/tidy_data/heatmaps/tidy_sorensen.py`

 * *Files identical despite different names*

### Comparing `ExpoSeq-1.0.5/src/ExpoSeq/tidy_data/interpret_data.py` & `ExpoSeq-1.1.1/src/ExpoSeq/tidy_data/interpret_data.py`

 * *Files identical despite different names*

### Comparing `ExpoSeq-1.0.5/src/ExpoSeq/tidy_data/read_extract_data.py` & `ExpoSeq-1.1.1/src/ExpoSeq/tidy_data/read_extract_data.py`

 * *Files identical despite different names*

### Comparing `ExpoSeq-1.0.5/src/ExpoSeq/tidy_data/tidy_alignment_reports.py` & `ExpoSeq-1.1.1/src/ExpoSeq/tidy_data/tidy_alignment_reports.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 import pandas as pd
-from .read_extract_data import read_alignment_report
+from ExpoSeq.tidy_data.read_extract_data import read_alignment_report
 
 
 
 def collect_boxplot_data(report_filename, local_pattern):
     with open(report_filename) as f:
         alignment_report = f.readlines()
     data_extractor = read_alignment_report(alignment_report)
```

### Comparing `ExpoSeq-1.0.5/src/ExpoSeq/tidy_data/tidy_cluster_embedding.py` & `ExpoSeq-1.1.1/src/ExpoSeq/tidy_data/tidy_cluster_embedding.py`

 * *Files identical despite different names*

### Comparing `ExpoSeq-1.0.5/src/ExpoSeq/tidy_data/tidy_rel_sequence_abun.py` & `ExpoSeq-1.1.1/src/ExpoSeq/tidy_data/tidy_rel_sequence_abun.py`

 * *Files identical despite different names*

### Comparing `ExpoSeq-1.0.5/src/ExpoSeq/tidy_data/tidy_seqlogoPlot.py` & `ExpoSeq-1.1.1/src/ExpoSeq/tidy_data/tidy_seqlogoPlot.py`

 * *Files identical despite different names*

### Comparing `ExpoSeq-1.0.5/src/ExpoSeq/tidy_data/tidy_stacked_aa_distr.py` & `ExpoSeq-1.1.1/src/ExpoSeq/tidy_data/tidy_stacked_aa_distr.py`

 * *Files identical despite different names*

### Comparing `ExpoSeq-1.0.5/src/ExpoSeq.egg-info/PKG-INFO` & `ExpoSeq-1.1.1/src/ExpoSeq.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 Metadata-Version: 2.1
 Name: ExpoSeq
-Version: 1.0.5
+Version: 1.1.1
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

### Comparing `ExpoSeq-1.0.5/src/ExpoSeq.egg-info/SOURCES.txt` & `ExpoSeq-1.1.1/src/ExpoSeq.egg-info/SOURCES.txt`

 * *Files 5% similar despite different names*

```diff
@@ -1,15 +1,17 @@
 LICENSE
 MANIFEST.in
 README.md
 setup.py
 src/ExpoSeq/__init__.py
+src/ExpoSeq/full_pipe.py
 src/ExpoSeq/pipeline.py
 src/ExpoSeq/reset.py
 src/ExpoSeq/run.py
+src/ExpoSeq/test_uploader.py
 src/ExpoSeq.egg-info/PKG-INFO
 src/ExpoSeq.egg-info/SOURCES.txt
 src/ExpoSeq.egg-info/dependency_links.txt
 src/ExpoSeq.egg-info/requires.txt
 src/ExpoSeq.egg-info/top_level.txt
 src/ExpoSeq/augment_data/__init__.py
 src/ExpoSeq/augment_data/binding_data.py
@@ -41,14 +43,15 @@
 src/ExpoSeq/settings/change_save_settings.py
 src/ExpoSeq/settings/colorbar.txt
 src/ExpoSeq/settings/font_settings.txt
 src/ExpoSeq/settings/global_vars.txt
 src/ExpoSeq/settings/legend_settings.txt
 src/ExpoSeq/settings/plot_styler.py
 src/ExpoSeq/settings/save_settings.txt
+src/ExpoSeq/test_data/__init__.py
 src/ExpoSeq/tidy_data/__init__.py
 src/ExpoSeq/tidy_data/aminoacid_distribution.py
 src/ExpoSeq/tidy_data/barplot.py
 src/ExpoSeq/tidy_data/clustering.py
 src/ExpoSeq/tidy_data/interpret_data.py
 src/ExpoSeq/tidy_data/read_extract_data.py
 src/ExpoSeq/tidy_data/tidy_USQ_plot_.py
```

