# Comparing `tmp/ExpoSeq-1.1.3.tar.gz` & `tmp/ExpoSeq-1.1.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ExpoSeq-1.1.3.tar", last modified: Mon Jun 12 12:01:12 2023, max compression
+gzip compressed data, was "ExpoSeq-1.1.4.tar", last modified: Mon Jun 12 12:13:41 2023, max compression
```

## Comparing `ExpoSeq-1.1.3.tar` & `ExpoSeq-1.1.4.tar`

### file list

```diff
@@ -1,90 +1,91 @@
-drwxrwxrwx   0        0        0        0 2023-06-12 12:01:12.344405 ExpoSeq-1.1.3/
--rw-rw-rw-   0        0        0     1090 2023-05-30 20:50:39.000000 ExpoSeq-1.1.3/LICENSE
--rw-rw-rw-   0        0        0       59 2023-05-30 20:50:39.000000 ExpoSeq-1.1.3/MANIFEST.in
--rw-rw-rw-   0        0        0     4091 2023-06-12 12:01:12.343403 ExpoSeq-1.1.3/PKG-INFO
--rw-rw-rw-   0        0        0     3725 2023-05-30 20:50:39.000000 ExpoSeq-1.1.3/README.md
--rw-rw-rw-   0        0        0       42 2023-06-12 12:01:12.344405 ExpoSeq-1.1.3/setup.cfg
--rw-rw-rw-   0        0        0     1320 2023-06-12 12:00:37.000000 ExpoSeq-1.1.3/setup.py
-drwxrwxrwx   0        0        0        0 2023-06-12 12:01:12.034551 ExpoSeq-1.1.3/src/
-drwxrwxrwx   0        0        0        0 2023-06-12 12:01:12.069553 ExpoSeq-1.1.3/src/ExpoSeq/
--rw-rw-rw-   0        0        0        0 2023-06-12 07:39:03.000000 ExpoSeq-1.1.3/src/ExpoSeq/__init__.py
-drwxrwxrwx   0        0        0        0 2023-06-12 12:01:12.134110 ExpoSeq-1.1.3/src/ExpoSeq/augment_data/
--rw-rw-rw-   0        0        0        0 2023-05-30 20:50:39.000000 ExpoSeq-1.1.3/src/ExpoSeq/augment_data/__init__.py
--rw-rw-rw-   0        0        0     1007 2023-05-30 20:50:39.000000 ExpoSeq-1.1.3/src/ExpoSeq/augment_data/binding_data.py
--rw-rw-rw-   0        0        0      858 2023-05-30 20:50:39.000000 ExpoSeq-1.1.3/src/ExpoSeq/augment_data/check_reports.py
--rw-rw-rw-   0        0        0      913 2023-05-30 20:50:39.000000 ExpoSeq-1.1.3/src/ExpoSeq/augment_data/load_data.py
--rw-rw-rw-   0        0        0     4616 2023-06-09 10:59:18.000000 ExpoSeq-1.1.3/src/ExpoSeq/augment_data/loop_collect_reports.py
--rw-rw-rw-   0        0        0     7915 2023-06-09 10:59:18.000000 ExpoSeq-1.1.3/src/ExpoSeq/augment_data/mixcr_cl.py
--rw-rw-rw-   0        0        0    10406 2023-06-12 10:03:32.000000 ExpoSeq-1.1.3/src/ExpoSeq/augment_data/mixcr_nils.py
--rw-rw-rw-   0        0        0     6586 2023-06-09 10:59:18.000000 ExpoSeq-1.1.3/src/ExpoSeq/augment_data/randomizer.py
--rw-rw-rw-   0        0        0      580 2023-05-30 20:50:39.000000 ExpoSeq-1.1.3/src/ExpoSeq/augment_data/read_raw_data.py
--rw-rw-rw-   0        0        0     3646 2023-05-30 20:50:39.000000 ExpoSeq-1.1.3/src/ExpoSeq/augment_data/structure_files.py
--rw-rw-rw-   0        0        0      519 2023-05-30 20:50:39.000000 ExpoSeq-1.1.3/src/ExpoSeq/augment_data/trimming.py
--rw-rw-rw-   0        0        0    17046 2023-06-12 11:43:10.000000 ExpoSeq-1.1.3/src/ExpoSeq/augment_data/uploader.py
--rw-rw-rw-   0        0        0    10265 2023-06-12 11:49:42.000000 ExpoSeq-1.1.3/src/ExpoSeq/full_pipe.py
--rw-rw-rw-   0        0        0    27442 2023-06-12 11:33:17.000000 ExpoSeq-1.1.3/src/ExpoSeq/pipeline.py
-drwxrwxrwx   0        0        0        0 2023-06-12 12:01:12.199463 ExpoSeq-1.1.3/src/ExpoSeq/plots/
--rw-rw-rw-   0        0        0        0 2023-05-30 20:50:39.000000 ExpoSeq-1.1.3/src/ExpoSeq/plots/__init__.py
--rw-rw-rw-   0        0        0     2061 2023-06-12 07:50:14.000000 ExpoSeq-1.1.3/src/ExpoSeq/plots/barplot.py
--rw-rw-rw-   0        0        0     1666 2023-06-12 07:50:14.000000 ExpoSeq-1.1.3/src/ExpoSeq/plots/cluster_embedding.py
--rw-rw-rw-   0        0        0     4363 2023-05-30 20:50:39.000000 ExpoSeq-1.1.3/src/ExpoSeq/plots/embedding_with_binding.py
--rw-rw-rw-   0        0        0     3444 2023-06-09 10:59:18.000000 ExpoSeq-1.1.3/src/ExpoSeq/plots/length_distribution.py
--rw-rw-rw-   0        0        0     7669 2023-06-12 07:50:14.000000 ExpoSeq-1.1.3/src/ExpoSeq/plots/levenshtein_clustering.py
--rw-rw-rw-   0        0        0     4379 2023-06-12 07:50:14.000000 ExpoSeq-1.1.3/src/ExpoSeq/plots/logo_plot.py
--rw-rw-rw-   0        0        0     3352 2023-06-12 07:50:14.000000 ExpoSeq-1.1.3/src/ExpoSeq/plots/plt_heatmap.py
--rw-rw-rw-   0        0        0     2524 2023-05-30 20:50:39.000000 ExpoSeq-1.1.3/src/ExpoSeq/plots/protvec.py
--rw-rw-rw-   0        0        0     1470 2023-06-12 07:50:14.000000 ExpoSeq-1.1.3/src/ExpoSeq/plots/relative_sequence_abundance.py
--rw-rw-rw-   0        0        0     1634 2023-05-30 20:50:39.000000 ExpoSeq-1.1.3/src/ExpoSeq/plots/saveFig.py
--rw-rw-rw-   0        0        0     1064 2023-06-12 07:50:14.000000 ExpoSeq-1.1.3/src/ExpoSeq/plots/stacked_aa_distribution.py
--rw-rw-rw-   0        0        0     2542 2023-06-12 07:50:14.000000 ExpoSeq-1.1.3/src/ExpoSeq/plots/usq_plot.py
--rw-rw-rw-   0        0        0     3019 2023-06-01 12:20:51.000000 ExpoSeq-1.1.3/src/ExpoSeq/reset.py
--rw-rw-rw-   0        0        0      288 2023-06-12 07:47:58.000000 ExpoSeq-1.1.3/src/ExpoSeq/run.py
-drwxrwxrwx   0        0        0        0 2023-06-12 12:01:12.224675 ExpoSeq-1.1.3/src/ExpoSeq/settings/
--rw-rw-rw-   0        0        0        0 2023-05-30 20:50:39.000000 ExpoSeq-1.1.3/src/ExpoSeq/settings/__init__.py
--rw-rw-rw-   0        0        0     2086 2023-05-30 20:50:39.000000 ExpoSeq-1.1.3/src/ExpoSeq/settings/blosum_62.txt
--rw-rw-rw-   0        0        0     1883 2023-06-12 11:49:42.000000 ExpoSeq-1.1.3/src/ExpoSeq/settings/change_save_settings.py
--rw-rw-rw-   0        0        0       94 2023-06-12 11:44:07.000000 ExpoSeq-1.1.3/src/ExpoSeq/settings/colorbar.txt
--rw-rw-rw-   0        0        0       86 2023-06-12 11:44:07.000000 ExpoSeq-1.1.3/src/ExpoSeq/settings/font_settings.txt
--rw-rw-rw-   0        0        0       57 2023-06-12 11:44:07.000000 ExpoSeq-1.1.3/src/ExpoSeq/settings/global_vars.txt
--rw-rw-rw-   0        0        0      179 2023-06-12 11:44:07.000000 ExpoSeq-1.1.3/src/ExpoSeq/settings/legend_settings.txt
--rw-rw-rw-   0        0        0     8133 2023-05-30 20:50:39.000000 ExpoSeq-1.1.3/src/ExpoSeq/settings/plot_styler.py
--rw-rw-rw-   0        0        0       42 2023-06-12 11:44:07.000000 ExpoSeq-1.1.3/src/ExpoSeq/settings/save_settings.txt
-drwxrwxrwx   0        0        0        0 2023-06-12 12:01:12.228695 ExpoSeq-1.1.3/src/ExpoSeq/test_data/
--rw-rw-rw-   0        0        0        0 2023-06-12 07:52:57.000000 ExpoSeq-1.1.3/src/ExpoSeq/test_data/__init__.py
--rw-rw-rw-   0        0        0    20748 2023-06-09 10:59:18.000000 ExpoSeq-1.1.3/src/ExpoSeq/test_data/all_alignment_reports.pickle
-drwxrwxrwx   0        0        0        0 2023-06-12 12:01:12.257677 ExpoSeq-1.1.3/src/ExpoSeq/test_data/test_files/
--rw-rw-rw-   0        0        0     3578 2023-06-09 10:59:18.000000 ExpoSeq-1.1.3/src/ExpoSeq/test_data/test_files/Chris_main_df.csv
--rw-rw-rw-   0        0        0    11571 2023-06-12 11:58:23.000000 ExpoSeq-1.1.3/src/ExpoSeq/test_data/test_files/binding_data.csv
--rw-rw-rw-   0        0        0      566 2023-06-12 11:58:23.000000 ExpoSeq-1.1.3/src/ExpoSeq/test_data/test_files/experiment_names.pickle
--rw-rw-rw-   0        0        0 19607644 2023-06-12 11:58:23.000000 ExpoSeq-1.1.3/src/ExpoSeq/test_data/test_files/sequencing_report.csv
--rw-rw-rw-   0        0        0    87391 2023-06-12 09:06:58.000000 ExpoSeq-1.1.3/src/ExpoSeq/test_data/test_files/test1.fastq
--rw-rw-rw-   0        0        0   210829 2023-06-12 09:06:58.000000 ExpoSeq-1.1.3/src/ExpoSeq/test_data/test_files/test2.fastq
--rw-rw-rw-   0        0        0    94420 2023-06-12 09:06:59.000000 ExpoSeq-1.1.3/src/ExpoSeq/test_data/test_files/test3.fastq
--rw-rw-rw-   0        0        0     2589 2023-06-12 10:02:11.000000 ExpoSeq-1.1.3/src/ExpoSeq/test_uploader.py
-drwxrwxrwx   0        0        0        0 2023-06-12 12:01:12.308222 ExpoSeq-1.1.3/src/ExpoSeq/tidy_data/
--rw-rw-rw-   0        0        0        0 2023-05-30 20:50:39.000000 ExpoSeq-1.1.3/src/ExpoSeq/tidy_data/__init__.py
--rw-rw-rw-   0        0        0     2176 2023-05-30 20:50:39.000000 ExpoSeq-1.1.3/src/ExpoSeq/tidy_data/aminoacid_distribution.py
--rw-rw-rw-   0        0        0     2228 2023-05-30 20:50:39.000000 ExpoSeq-1.1.3/src/ExpoSeq/tidy_data/barplot.py
--rw-rw-rw-   0        0        0     1152 2023-05-30 20:50:39.000000 ExpoSeq-1.1.3/src/ExpoSeq/tidy_data/clustering.py
-drwxrwxrwx   0        0        0        0 2023-06-12 12:01:12.338419 ExpoSeq-1.1.3/src/ExpoSeq/tidy_data/heatmaps/
--rw-rw-rw-   0        0        0        0 2023-05-30 20:50:39.000000 ExpoSeq-1.1.3/src/ExpoSeq/tidy_data/heatmaps/__init__.py
--rw-rw-rw-   0        0        0     1509 2023-05-30 20:50:39.000000 ExpoSeq-1.1.3/src/ExpoSeq/tidy_data/heatmaps/bool_sequences_matrix.py
--rw-rw-rw-   0        0        0     1818 2023-05-30 20:50:39.000000 ExpoSeq-1.1.3/src/ExpoSeq/tidy_data/heatmaps/tidy_heatmap_share.py
--rw-rw-rw-   0        0        0     1673 2023-05-30 20:50:39.000000 ExpoSeq-1.1.3/src/ExpoSeq/tidy_data/heatmaps/tidy_jaccard.py
--rw-rw-rw-   0        0        0     5139 2023-05-30 20:50:39.000000 ExpoSeq-1.1.3/src/ExpoSeq/tidy_data/heatmaps/tidy_morosita_horn.py
--rw-rw-rw-   0        0        0     1597 2023-05-30 20:50:39.000000 ExpoSeq-1.1.3/src/ExpoSeq/tidy_data/heatmaps/tidy_sorensen.py
--rw-rw-rw-   0        0        0      678 2023-05-30 20:50:39.000000 ExpoSeq-1.1.3/src/ExpoSeq/tidy_data/interpret_data.py
--rw-rw-rw-   0        0        0     3907 2023-05-30 20:50:39.000000 ExpoSeq-1.1.3/src/ExpoSeq/tidy_data/read_extract_data.py
--rw-rw-rw-   0        0        0      440 2023-06-12 07:48:51.000000 ExpoSeq-1.1.3/src/ExpoSeq/tidy_data/tidy_USQ_plot_.py
--rw-rw-rw-   0        0        0     1217 2023-06-12 07:48:51.000000 ExpoSeq-1.1.3/src/ExpoSeq/tidy_data/tidy_alignment_reports.py
--rw-rw-rw-   0        0        0     1461 2023-05-30 20:50:39.000000 ExpoSeq-1.1.3/src/ExpoSeq/tidy_data/tidy_cluster_embedding.py
--rw-rw-rw-   0        0        0      391 2023-05-30 20:50:39.000000 ExpoSeq-1.1.3/src/ExpoSeq/tidy_data/tidy_library.py
--rw-rw-rw-   0        0        0     1992 2023-05-30 20:50:39.000000 ExpoSeq-1.1.3/src/ExpoSeq/tidy_data/tidy_rel_sequence_abun.py
--rw-rw-rw-   0        0        0     1599 2023-05-30 20:50:39.000000 ExpoSeq-1.1.3/src/ExpoSeq/tidy_data/tidy_seqlogoPlot.py
--rw-rw-rw-   0        0        0     1299 2023-05-30 20:50:39.000000 ExpoSeq-1.1.3/src/ExpoSeq/tidy_data/tidy_stacked_aa_distr.py
-drwxrwxrwx   0        0        0        0 2023-06-12 12:01:12.080702 ExpoSeq-1.1.3/src/ExpoSeq.egg-info/
--rw-rw-rw-   0        0        0     4091 2023-06-12 12:01:11.000000 ExpoSeq-1.1.3/src/ExpoSeq.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0     2926 2023-06-12 12:01:11.000000 ExpoSeq-1.1.3/src/ExpoSeq.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-06-12 12:01:11.000000 ExpoSeq-1.1.3/src/ExpoSeq.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0      188 2023-06-12 12:01:11.000000 ExpoSeq-1.1.3/src/ExpoSeq.egg-info/requires.txt
--rw-rw-rw-   0        0        0        8 2023-06-12 12:01:11.000000 ExpoSeq-1.1.3/src/ExpoSeq.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-06-12 12:13:41.638835 ExpoSeq-1.1.4/
+-rw-rw-rw-   0        0        0     1090 2023-05-30 20:50:39.000000 ExpoSeq-1.1.4/LICENSE
+-rw-rw-rw-   0        0        0       59 2023-05-30 20:50:39.000000 ExpoSeq-1.1.4/MANIFEST.in
+-rw-rw-rw-   0        0        0     4091 2023-06-12 12:13:41.638835 ExpoSeq-1.1.4/PKG-INFO
+-rw-rw-rw-   0        0        0     3725 2023-05-30 20:50:39.000000 ExpoSeq-1.1.4/README.md
+-rw-rw-rw-   0        0        0       42 2023-06-12 12:13:41.639821 ExpoSeq-1.1.4/setup.cfg
+-rw-rw-rw-   0        0        0     1320 2023-06-12 12:13:33.000000 ExpoSeq-1.1.4/setup.py
+drwxrwxrwx   0        0        0        0 2023-06-12 12:13:41.246049 ExpoSeq-1.1.4/src/
+drwxrwxrwx   0        0        0        0 2023-06-12 12:13:41.292541 ExpoSeq-1.1.4/src/ExpoSeq/
+-rw-rw-rw-   0        0        0        0 2023-06-12 12:03:02.000000 ExpoSeq-1.1.4/src/ExpoSeq/__init__.py
+drwxrwxrwx   0        0        0        0 2023-06-12 12:13:41.374494 ExpoSeq-1.1.4/src/ExpoSeq/augment_data/
+-rw-rw-rw-   0        0        0        0 2023-06-12 12:03:02.000000 ExpoSeq-1.1.4/src/ExpoSeq/augment_data/__init__.py
+-rw-rw-rw-   0        0        0     1007 2023-06-12 12:03:02.000000 ExpoSeq-1.1.4/src/ExpoSeq/augment_data/binding_data.py
+-rw-rw-rw-   0        0        0      858 2023-06-12 12:03:02.000000 ExpoSeq-1.1.4/src/ExpoSeq/augment_data/check_reports.py
+-rw-rw-rw-   0        0        0      913 2023-06-12 12:03:02.000000 ExpoSeq-1.1.4/src/ExpoSeq/augment_data/load_data.py
+-rw-rw-rw-   0        0        0     4616 2023-06-12 12:03:02.000000 ExpoSeq-1.1.4/src/ExpoSeq/augment_data/loop_collect_reports.py
+-rw-rw-rw-   0        0        0     7915 2023-06-12 12:03:02.000000 ExpoSeq-1.1.4/src/ExpoSeq/augment_data/mixcr_cl.py
+-rw-rw-rw-   0        0        0    10406 2023-06-12 12:03:02.000000 ExpoSeq-1.1.4/src/ExpoSeq/augment_data/mixcr_nils.py
+-rw-rw-rw-   0        0        0     6586 2023-06-12 12:03:02.000000 ExpoSeq-1.1.4/src/ExpoSeq/augment_data/randomizer.py
+-rw-rw-rw-   0        0        0      580 2023-06-12 12:03:02.000000 ExpoSeq-1.1.4/src/ExpoSeq/augment_data/read_raw_data.py
+-rw-rw-rw-   0        0        0     3646 2023-06-12 12:03:02.000000 ExpoSeq-1.1.4/src/ExpoSeq/augment_data/structure_files.py
+-rw-rw-rw-   0        0        0      519 2023-06-12 12:03:02.000000 ExpoSeq-1.1.4/src/ExpoSeq/augment_data/trimming.py
+-rw-rw-rw-   0        0        0    17058 2023-06-12 12:09:54.000000 ExpoSeq-1.1.4/src/ExpoSeq/augment_data/uploader.py
+-rw-rw-rw-   0        0        0    10260 2023-06-12 12:11:34.000000 ExpoSeq-1.1.4/src/ExpoSeq/full_pipe.py
+-rw-rw-rw-   0        0        0    27442 2023-06-12 12:03:02.000000 ExpoSeq-1.1.4/src/ExpoSeq/pipeline.py
+drwxrwxrwx   0        0        0        0 2023-06-12 12:13:41.455555 ExpoSeq-1.1.4/src/ExpoSeq/plots/
+-rw-rw-rw-   0        0        0        0 2023-06-12 12:03:02.000000 ExpoSeq-1.1.4/src/ExpoSeq/plots/__init__.py
+-rw-rw-rw-   0        0        0     2061 2023-06-12 12:03:02.000000 ExpoSeq-1.1.4/src/ExpoSeq/plots/barplot.py
+-rw-rw-rw-   0        0        0     1666 2023-06-12 12:03:02.000000 ExpoSeq-1.1.4/src/ExpoSeq/plots/cluster_embedding.py
+-rw-rw-rw-   0        0        0     4363 2023-06-12 12:03:02.000000 ExpoSeq-1.1.4/src/ExpoSeq/plots/embedding_with_binding.py
+-rw-rw-rw-   0        0        0     3444 2023-06-12 12:03:02.000000 ExpoSeq-1.1.4/src/ExpoSeq/plots/length_distribution.py
+-rw-rw-rw-   0        0        0     7669 2023-06-12 12:03:02.000000 ExpoSeq-1.1.4/src/ExpoSeq/plots/levenshtein_clustering.py
+-rw-rw-rw-   0        0        0     4379 2023-06-12 12:03:02.000000 ExpoSeq-1.1.4/src/ExpoSeq/plots/logo_plot.py
+-rw-rw-rw-   0        0        0     3352 2023-06-12 12:03:02.000000 ExpoSeq-1.1.4/src/ExpoSeq/plots/plt_heatmap.py
+-rw-rw-rw-   0        0        0     2524 2023-06-12 12:03:02.000000 ExpoSeq-1.1.4/src/ExpoSeq/plots/protvec.py
+-rw-rw-rw-   0        0        0     1470 2023-06-12 12:03:02.000000 ExpoSeq-1.1.4/src/ExpoSeq/plots/relative_sequence_abundance.py
+-rw-rw-rw-   0        0        0     1634 2023-06-12 12:03:02.000000 ExpoSeq-1.1.4/src/ExpoSeq/plots/saveFig.py
+-rw-rw-rw-   0        0        0     1064 2023-06-12 12:03:02.000000 ExpoSeq-1.1.4/src/ExpoSeq/plots/stacked_aa_distribution.py
+-rw-rw-rw-   0        0        0     2542 2023-06-12 12:03:02.000000 ExpoSeq-1.1.4/src/ExpoSeq/plots/usq_plot.py
+-rw-rw-rw-   0        0        0     3019 2023-06-12 12:03:02.000000 ExpoSeq-1.1.4/src/ExpoSeq/reset.py
+-rw-rw-rw-   0        0        0      288 2023-06-12 12:03:02.000000 ExpoSeq-1.1.4/src/ExpoSeq/run.py
+drwxrwxrwx   0        0        0        0 2023-06-12 12:13:41.481193 ExpoSeq-1.1.4/src/ExpoSeq/settings/
+-rw-rw-rw-   0        0        0        0 2023-06-12 12:03:02.000000 ExpoSeq-1.1.4/src/ExpoSeq/settings/__init__.py
+-rw-rw-rw-   0        0        0     2086 2023-06-12 12:03:02.000000 ExpoSeq-1.1.4/src/ExpoSeq/settings/blosum_62.txt
+-rw-rw-rw-   0        0        0     1883 2023-06-12 12:03:02.000000 ExpoSeq-1.1.4/src/ExpoSeq/settings/change_save_settings.py
+-rw-rw-rw-   0        0        0       94 2023-06-12 12:10:03.000000 ExpoSeq-1.1.4/src/ExpoSeq/settings/colorbar.txt
+-rw-rw-rw-   0        0        0       86 2023-06-12 12:10:03.000000 ExpoSeq-1.1.4/src/ExpoSeq/settings/font_settings.txt
+-rw-rw-rw-   0        0        0       57 2023-06-12 12:10:03.000000 ExpoSeq-1.1.4/src/ExpoSeq/settings/global_vars.txt
+-rw-rw-rw-   0        0        0      179 2023-06-12 12:10:03.000000 ExpoSeq-1.1.4/src/ExpoSeq/settings/legend_settings.txt
+-rw-rw-rw-   0        0        0     8133 2023-06-12 12:03:02.000000 ExpoSeq-1.1.4/src/ExpoSeq/settings/plot_styler.py
+-rw-rw-rw-   0        0        0       42 2023-06-12 12:10:03.000000 ExpoSeq-1.1.4/src/ExpoSeq/settings/save_settings.txt
+drwxrwxrwx   0        0        0        0 2023-06-12 12:13:41.486221 ExpoSeq-1.1.4/src/ExpoSeq/test_data/
+-rw-rw-rw-   0        0        0        0 2023-06-12 12:03:02.000000 ExpoSeq-1.1.4/src/ExpoSeq/test_data/__init__.py
+-rw-rw-rw-   0        0        0    20748 2023-06-12 12:03:02.000000 ExpoSeq-1.1.4/src/ExpoSeq/test_data/all_alignment_reports.pickle
+drwxrwxrwx   0        0        0        0 2023-06-12 12:13:41.518193 ExpoSeq-1.1.4/src/ExpoSeq/test_data/test_files/
+-rw-rw-rw-   0        0        0     3578 2023-06-12 12:03:02.000000 ExpoSeq-1.1.4/src/ExpoSeq/test_data/test_files/Chris_main_df.csv
+-rw-rw-rw-   0        0        0        0 2023-06-12 12:03:02.000000 ExpoSeq-1.1.4/src/ExpoSeq/test_data/test_files/__init__.py
+-rw-rw-rw-   0        0        0    11571 2023-06-12 12:03:02.000000 ExpoSeq-1.1.4/src/ExpoSeq/test_data/test_files/binding_data.csv
+-rw-rw-rw-   0        0        0      566 2023-06-12 12:03:02.000000 ExpoSeq-1.1.4/src/ExpoSeq/test_data/test_files/experiment_names.pickle
+-rw-rw-rw-   0        0        0 19607644 2023-06-12 12:03:02.000000 ExpoSeq-1.1.4/src/ExpoSeq/test_data/test_files/sequencing_report.csv
+-rw-rw-rw-   0        0        0    87391 2023-06-12 12:03:02.000000 ExpoSeq-1.1.4/src/ExpoSeq/test_data/test_files/test1.fastq
+-rw-rw-rw-   0        0        0   210829 2023-06-12 12:03:02.000000 ExpoSeq-1.1.4/src/ExpoSeq/test_data/test_files/test2.fastq
+-rw-rw-rw-   0        0        0    94420 2023-06-12 12:03:02.000000 ExpoSeq-1.1.4/src/ExpoSeq/test_data/test_files/test3.fastq
+-rw-rw-rw-   0        0        0     2632 2023-06-12 12:05:40.000000 ExpoSeq-1.1.4/src/ExpoSeq/test_uploader.py
+drwxrwxrwx   0        0        0        0 2023-06-12 12:13:41.591984 ExpoSeq-1.1.4/src/ExpoSeq/tidy_data/
+-rw-rw-rw-   0        0        0        0 2023-06-12 12:03:02.000000 ExpoSeq-1.1.4/src/ExpoSeq/tidy_data/__init__.py
+-rw-rw-rw-   0        0        0     2176 2023-06-12 12:03:02.000000 ExpoSeq-1.1.4/src/ExpoSeq/tidy_data/aminoacid_distribution.py
+-rw-rw-rw-   0        0        0     2228 2023-06-12 12:03:02.000000 ExpoSeq-1.1.4/src/ExpoSeq/tidy_data/barplot.py
+-rw-rw-rw-   0        0        0     1152 2023-06-12 12:03:02.000000 ExpoSeq-1.1.4/src/ExpoSeq/tidy_data/clustering.py
+drwxrwxrwx   0        0        0        0 2023-06-12 12:13:41.631735 ExpoSeq-1.1.4/src/ExpoSeq/tidy_data/heatmaps/
+-rw-rw-rw-   0        0        0        0 2023-06-12 12:03:02.000000 ExpoSeq-1.1.4/src/ExpoSeq/tidy_data/heatmaps/__init__.py
+-rw-rw-rw-   0        0        0     1509 2023-06-12 12:03:02.000000 ExpoSeq-1.1.4/src/ExpoSeq/tidy_data/heatmaps/bool_sequences_matrix.py
+-rw-rw-rw-   0        0        0     1818 2023-06-12 12:03:02.000000 ExpoSeq-1.1.4/src/ExpoSeq/tidy_data/heatmaps/tidy_heatmap_share.py
+-rw-rw-rw-   0        0        0     1673 2023-06-12 12:03:02.000000 ExpoSeq-1.1.4/src/ExpoSeq/tidy_data/heatmaps/tidy_jaccard.py
+-rw-rw-rw-   0        0        0     5139 2023-06-12 12:03:02.000000 ExpoSeq-1.1.4/src/ExpoSeq/tidy_data/heatmaps/tidy_morosita_horn.py
+-rw-rw-rw-   0        0        0     1597 2023-06-12 12:03:02.000000 ExpoSeq-1.1.4/src/ExpoSeq/tidy_data/heatmaps/tidy_sorensen.py
+-rw-rw-rw-   0        0        0      678 2023-06-12 12:03:02.000000 ExpoSeq-1.1.4/src/ExpoSeq/tidy_data/interpret_data.py
+-rw-rw-rw-   0        0        0     3907 2023-06-12 12:03:02.000000 ExpoSeq-1.1.4/src/ExpoSeq/tidy_data/read_extract_data.py
+-rw-rw-rw-   0        0        0      440 2023-06-12 12:03:02.000000 ExpoSeq-1.1.4/src/ExpoSeq/tidy_data/tidy_USQ_plot_.py
+-rw-rw-rw-   0        0        0     1217 2023-06-12 12:03:02.000000 ExpoSeq-1.1.4/src/ExpoSeq/tidy_data/tidy_alignment_reports.py
+-rw-rw-rw-   0        0        0     1461 2023-06-12 12:03:02.000000 ExpoSeq-1.1.4/src/ExpoSeq/tidy_data/tidy_cluster_embedding.py
+-rw-rw-rw-   0        0        0      391 2023-06-12 12:03:02.000000 ExpoSeq-1.1.4/src/ExpoSeq/tidy_data/tidy_library.py
+-rw-rw-rw-   0        0        0     1992 2023-06-12 12:03:02.000000 ExpoSeq-1.1.4/src/ExpoSeq/tidy_data/tidy_rel_sequence_abun.py
+-rw-rw-rw-   0        0        0     1599 2023-06-12 12:03:02.000000 ExpoSeq-1.1.4/src/ExpoSeq/tidy_data/tidy_seqlogoPlot.py
+-rw-rw-rw-   0        0        0     1299 2023-06-12 12:03:02.000000 ExpoSeq-1.1.4/src/ExpoSeq/tidy_data/tidy_stacked_aa_distr.py
+drwxrwxrwx   0        0        0        0 2023-06-12 12:13:41.300618 ExpoSeq-1.1.4/src/ExpoSeq.egg-info/
+-rw-rw-rw-   0        0        0     4091 2023-06-12 12:13:41.000000 ExpoSeq-1.1.4/src/ExpoSeq.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0     2971 2023-06-12 12:13:41.000000 ExpoSeq-1.1.4/src/ExpoSeq.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-06-12 12:13:41.000000 ExpoSeq-1.1.4/src/ExpoSeq.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0      188 2023-06-12 12:13:41.000000 ExpoSeq-1.1.4/src/ExpoSeq.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        8 2023-06-12 12:13:41.000000 ExpoSeq-1.1.4/src/ExpoSeq.egg-info/top_level.txt
```

### Comparing `ExpoSeq-1.1.3/LICENSE` & `ExpoSeq-1.1.4/LICENSE`

 * *Files identical despite different names*

### Comparing `ExpoSeq-1.1.3/PKG-INFO` & `ExpoSeq-1.1.4/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ExpoSeq
-Version: 1.1.3
+Version: 1.1.4
 Summary: A pacakge which provides various ways to analyze NGS data from phage display campaigns
 Home-page: https://github.com/nilshof01/ExpoSeq
 Author: Nils Hofmann
 Author-email: n.hofmann.99@web.de
 License: MIT
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
```

### Comparing `ExpoSeq-1.1.3/README.md` & `ExpoSeq-1.1.4/README.md`

 * *Files identical despite different names*

### Comparing `ExpoSeq-1.1.3/setup.py` & `ExpoSeq-1.1.4/setup.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 from setuptools import setup, find_packages
 
 with open("README.md", "r") as fh:
     long_description = fh.read()
 
 setup(
     name = "ExpoSeq",
-    version = "1.1.3",
+    version = "1.1.4",
     description = "A pacakge which provides various ways to analyze NGS data from phage display campaigns",
     long_description=long_description,
     long_description_content_type = "text/markdown",
     url = "https://github.com/nilshof01/ExpoSeq",
     author = "Nils Hofmann",
     author_email = "n.hofmann.99@web.de",
     license = "MIT",
```

### Comparing `ExpoSeq-1.1.3/src/ExpoSeq/augment_data/binding_data.py` & `ExpoSeq-1.1.4/src/ExpoSeq/augment_data/binding_data.py`

 * *Files identical despite different names*

### Comparing `ExpoSeq-1.1.3/src/ExpoSeq/augment_data/check_reports.py` & `ExpoSeq-1.1.4/src/ExpoSeq/augment_data/check_reports.py`

 * *Files identical despite different names*

### Comparing `ExpoSeq-1.1.3/src/ExpoSeq/augment_data/load_data.py` & `ExpoSeq-1.1.4/src/ExpoSeq/augment_data/load_data.py`

 * *Files identical despite different names*

### Comparing `ExpoSeq-1.1.3/src/ExpoSeq/augment_data/loop_collect_reports.py` & `ExpoSeq-1.1.4/src/ExpoSeq/augment_data/loop_collect_reports.py`

 * *Files identical despite different names*

### Comparing `ExpoSeq-1.1.3/src/ExpoSeq/augment_data/mixcr_cl.py` & `ExpoSeq-1.1.4/src/ExpoSeq/augment_data/mixcr_cl.py`

 * *Files identical despite different names*

### Comparing `ExpoSeq-1.1.3/src/ExpoSeq/augment_data/mixcr_nils.py` & `ExpoSeq-1.1.4/src/ExpoSeq/augment_data/mixcr_nils.py`

 * *Files identical despite different names*

### Comparing `ExpoSeq-1.1.3/src/ExpoSeq/augment_data/randomizer.py` & `ExpoSeq-1.1.4/src/ExpoSeq/augment_data/randomizer.py`

 * *Files identical despite different names*

### Comparing `ExpoSeq-1.1.3/src/ExpoSeq/augment_data/read_raw_data.py` & `ExpoSeq-1.1.4/src/ExpoSeq/augment_data/read_raw_data.py`

 * *Files identical despite different names*

### Comparing `ExpoSeq-1.1.3/src/ExpoSeq/augment_data/structure_files.py` & `ExpoSeq-1.1.4/src/ExpoSeq/augment_data/structure_files.py`

 * *Files identical despite different names*

### Comparing `ExpoSeq-1.1.3/src/ExpoSeq/augment_data/trimming.py` & `ExpoSeq-1.1.4/src/ExpoSeq/augment_data/trimming.py`

 * *Files identical despite different names*

### Comparing `ExpoSeq-1.1.3/src/ExpoSeq/augment_data/uploader.py` & `ExpoSeq-1.1.4/src/ExpoSeq/augment_data/uploader.py`

 * *Files 0% similar despite different names*

```diff
@@ -342,15 +342,15 @@
         all_alignment_reports = pd.DataFrame([])
         print("No alignment reports could be found in " + experiment + ". You will continue without being able to analyze the Alignment Quality.")
 
     return sequencing_report, all_alignment_reports, experiment
 
 def process_data_with_last_experiment(module_dir, last_experiment, testing):
     experiment = last_experiment
-    sequencing_report, all_alignment_reports = retrieve_reports(module_dir, experiment, testing)
+    sequencing_report, all_alignment_reports, experiment = retrieve_reports(module_dir, experiment, testing)
     return sequencing_report, all_alignment_reports, experiment
 
 def upload(testing=False, continue_analysis = "n", upload_type = "2", choose_exp = '1', paired_end_test = 'n', experiment_column = '1'):
    # module_dir = os.path.abspath("")
     module_dir = os.getcwd()
     pkg_path = pkg_resources.resource_filename("ExpoSeq", "")
     repo_path, last_experiment = check_last_exp(pkg_path, module_dir, testing)
```

### Comparing `ExpoSeq-1.1.3/src/ExpoSeq/full_pipe.py` & `ExpoSeq-1.1.4/src/ExpoSeq/full_pipe.py`

 * *Files 0% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 import os
 import pandas as pd
 import shutil
 import pkg_resources
 
 def run_pipeline(antigens = None, usq_multiple = "n", pass_interrupt = True, test = False):
     pkg_path = pkg_resources.resource_filename("ExpoSeq", "")
-    save_settings_path = os.path.join(self.pkg_path,
+    save_settings_path = os.path.join(pkg_path,
                  "settings",
                  "save_settings.txt")
     with open(save_settings_path, "r") as f:
         save_settings = f.read()
     save_settings = literal_eval(save_settings)
     original_path = save_settings["fname"]
     if antigens == True or antigens == False or antigens == None:
```

### Comparing `ExpoSeq-1.1.3/src/ExpoSeq/pipeline.py` & `ExpoSeq-1.1.4/src/ExpoSeq/pipeline.py`

 * *Files identical despite different names*

### Comparing `ExpoSeq-1.1.3/src/ExpoSeq/plots/barplot.py` & `ExpoSeq-1.1.4/src/ExpoSeq/plots/barplot.py`

 * *Files identical despite different names*

### Comparing `ExpoSeq-1.1.3/src/ExpoSeq/plots/cluster_embedding.py` & `ExpoSeq-1.1.4/src/ExpoSeq/plots/cluster_embedding.py`

 * *Files identical despite different names*

### Comparing `ExpoSeq-1.1.3/src/ExpoSeq/plots/embedding_with_binding.py` & `ExpoSeq-1.1.4/src/ExpoSeq/plots/embedding_with_binding.py`

 * *Files identical despite different names*

### Comparing `ExpoSeq-1.1.3/src/ExpoSeq/plots/length_distribution.py` & `ExpoSeq-1.1.4/src/ExpoSeq/plots/length_distribution.py`

 * *Files identical despite different names*

### Comparing `ExpoSeq-1.1.3/src/ExpoSeq/plots/levenshtein_clustering.py` & `ExpoSeq-1.1.4/src/ExpoSeq/plots/levenshtein_clustering.py`

 * *Files identical despite different names*

### Comparing `ExpoSeq-1.1.3/src/ExpoSeq/plots/logo_plot.py` & `ExpoSeq-1.1.4/src/ExpoSeq/plots/logo_plot.py`

 * *Files identical despite different names*

### Comparing `ExpoSeq-1.1.3/src/ExpoSeq/plots/plt_heatmap.py` & `ExpoSeq-1.1.4/src/ExpoSeq/plots/plt_heatmap.py`

 * *Files identical despite different names*

### Comparing `ExpoSeq-1.1.3/src/ExpoSeq/plots/protvec.py` & `ExpoSeq-1.1.4/src/ExpoSeq/plots/protvec.py`

 * *Files identical despite different names*

### Comparing `ExpoSeq-1.1.3/src/ExpoSeq/plots/relative_sequence_abundance.py` & `ExpoSeq-1.1.4/src/ExpoSeq/plots/relative_sequence_abundance.py`

 * *Files identical despite different names*

### Comparing `ExpoSeq-1.1.3/src/ExpoSeq/plots/saveFig.py` & `ExpoSeq-1.1.4/src/ExpoSeq/plots/saveFig.py`

 * *Files identical despite different names*

### Comparing `ExpoSeq-1.1.3/src/ExpoSeq/plots/stacked_aa_distribution.py` & `ExpoSeq-1.1.4/src/ExpoSeq/plots/stacked_aa_distribution.py`

 * *Files identical despite different names*

### Comparing `ExpoSeq-1.1.3/src/ExpoSeq/plots/usq_plot.py` & `ExpoSeq-1.1.4/src/ExpoSeq/plots/usq_plot.py`

 * *Files identical despite different names*

### Comparing `ExpoSeq-1.1.3/src/ExpoSeq/reset.py` & `ExpoSeq-1.1.4/src/ExpoSeq/reset.py`

 * *Files identical despite different names*

### Comparing `ExpoSeq-1.1.3/src/ExpoSeq/settings/blosum_62.txt` & `ExpoSeq-1.1.4/src/ExpoSeq/settings/blosum_62.txt`

 * *Files identical despite different names*

### Comparing `ExpoSeq-1.1.3/src/ExpoSeq/settings/change_save_settings.py` & `ExpoSeq-1.1.4/src/ExpoSeq/settings/change_save_settings.py`

 * *Files identical despite different names*

### Comparing `ExpoSeq-1.1.3/src/ExpoSeq/settings/plot_styler.py` & `ExpoSeq-1.1.4/src/ExpoSeq/settings/plot_styler.py`

 * *Files identical despite different names*

### Comparing `ExpoSeq-1.1.3/src/ExpoSeq/test_data/all_alignment_reports.pickle` & `ExpoSeq-1.1.4/src/ExpoSeq/test_data/all_alignment_reports.pickle`

 * *Files identical despite different names*

### Comparing `ExpoSeq-1.1.3/src/ExpoSeq/test_data/test_files/Chris_main_df.csv` & `ExpoSeq-1.1.4/src/ExpoSeq/test_data/test_files/Chris_main_df.csv`

 * *Files identical despite different names*

### Comparing `ExpoSeq-1.1.3/src/ExpoSeq/test_data/test_files/binding_data.csv` & `ExpoSeq-1.1.4/src/ExpoSeq/test_data/test_files/binding_data.csv`

 * *Files identical despite different names*

### Comparing `ExpoSeq-1.1.3/src/ExpoSeq/test_data/test_files/experiment_names.pickle` & `ExpoSeq-1.1.4/src/ExpoSeq/test_data/test_files/experiment_names.pickle`

 * *Files identical despite different names*

### Comparing `ExpoSeq-1.1.3/src/ExpoSeq/test_data/test_files/sequencing_report.csv` & `ExpoSeq-1.1.4/src/ExpoSeq/test_data/test_files/sequencing_report.csv`

 * *Files identical despite different names*

### Comparing `ExpoSeq-1.1.3/src/ExpoSeq/test_data/test_files/test1.fastq` & `ExpoSeq-1.1.4/src/ExpoSeq/test_data/test_files/test1.fastq`

 * *Files identical despite different names*

### Comparing `ExpoSeq-1.1.3/src/ExpoSeq/test_data/test_files/test2.fastq` & `ExpoSeq-1.1.4/src/ExpoSeq/test_data/test_files/test2.fastq`

 * *Files identical despite different names*

### Comparing `ExpoSeq-1.1.3/src/ExpoSeq/test_data/test_files/test3.fastq` & `ExpoSeq-1.1.4/src/ExpoSeq/test_data/test_files/test3.fastq`

 * *Files identical despite different names*

### Comparing `ExpoSeq-1.1.3/src/ExpoSeq/test_uploader.py` & `ExpoSeq-1.1.4/src/ExpoSeq/test_uploader.py`

 * *Files 5% similar despite different names*

```diff
@@ -15,15 +15,15 @@
         os.mkdir(os.path.join(module_dir, "temp"))
     if not os.path.isdir(os.path.join(module_dir, "my_experiments", "test_directory")):
         new_dir = os.path.join(module_dir, "my_experiments", "test_directory")
         os.mkdir(new_dir)
         source_seq_report = os.path.join(pkg_dir, "test_data","test_files", "sequencing_report.csv")
      #   source_align_report = os.path.join(pkg_dir, "test_data", "all_alignment_reports.pickle")
         source_experiments = os.path.join(pkg_dir, "test_data","test_files", "experiment_names.pickle")
-        shutil.copy2(source_seq_report, new_dir)
+        assert shutil.copy2(source_seq_report, new_dir), "could not copy sequencing report"
      #   shutil.copy2(source_align_report, new_dir)
         shutil.copy2(source_experiments, new_dir)
     else:
         pass
     
     #upload(testing=True, continue_analysis = "n", upload_type = "2", choose_exp = '1', paired_end_test = 'n', experiment_column = '1')
     assert upload(testing=True, continue_analysis = "n", upload_type = "1", choose_exp = '1', paired_end_test = 'n', experiment_column = '1'), "test 1 with upload_type 1,choose_exp = 1 and negative analysis continuation failed"
```

### Comparing `ExpoSeq-1.1.3/src/ExpoSeq/tidy_data/aminoacid_distribution.py` & `ExpoSeq-1.1.4/src/ExpoSeq/tidy_data/aminoacid_distribution.py`

 * *Files identical despite different names*

### Comparing `ExpoSeq-1.1.3/src/ExpoSeq/tidy_data/barplot.py` & `ExpoSeq-1.1.4/src/ExpoSeq/tidy_data/barplot.py`

 * *Files identical despite different names*

### Comparing `ExpoSeq-1.1.3/src/ExpoSeq/tidy_data/clustering.py` & `ExpoSeq-1.1.4/src/ExpoSeq/tidy_data/clustering.py`

 * *Files identical despite different names*

### Comparing `ExpoSeq-1.1.3/src/ExpoSeq/tidy_data/heatmaps/bool_sequences_matrix.py` & `ExpoSeq-1.1.4/src/ExpoSeq/tidy_data/heatmaps/bool_sequences_matrix.py`

 * *Files identical despite different names*

### Comparing `ExpoSeq-1.1.3/src/ExpoSeq/tidy_data/heatmaps/tidy_heatmap_share.py` & `ExpoSeq-1.1.4/src/ExpoSeq/tidy_data/heatmaps/tidy_heatmap_share.py`

 * *Files identical despite different names*

### Comparing `ExpoSeq-1.1.3/src/ExpoSeq/tidy_data/heatmaps/tidy_jaccard.py` & `ExpoSeq-1.1.4/src/ExpoSeq/tidy_data/heatmaps/tidy_jaccard.py`

 * *Files identical despite different names*

### Comparing `ExpoSeq-1.1.3/src/ExpoSeq/tidy_data/heatmaps/tidy_morosita_horn.py` & `ExpoSeq-1.1.4/src/ExpoSeq/tidy_data/heatmaps/tidy_morosita_horn.py`

 * *Files identical despite different names*

### Comparing `ExpoSeq-1.1.3/src/ExpoSeq/tidy_data/heatmaps/tidy_sorensen.py` & `ExpoSeq-1.1.4/src/ExpoSeq/tidy_data/heatmaps/tidy_sorensen.py`

 * *Files identical despite different names*

### Comparing `ExpoSeq-1.1.3/src/ExpoSeq/tidy_data/interpret_data.py` & `ExpoSeq-1.1.4/src/ExpoSeq/tidy_data/interpret_data.py`

 * *Files identical despite different names*

### Comparing `ExpoSeq-1.1.3/src/ExpoSeq/tidy_data/read_extract_data.py` & `ExpoSeq-1.1.4/src/ExpoSeq/tidy_data/read_extract_data.py`

 * *Files identical despite different names*

### Comparing `ExpoSeq-1.1.3/src/ExpoSeq/tidy_data/tidy_alignment_reports.py` & `ExpoSeq-1.1.4/src/ExpoSeq/tidy_data/tidy_alignment_reports.py`

 * *Files identical despite different names*

### Comparing `ExpoSeq-1.1.3/src/ExpoSeq/tidy_data/tidy_cluster_embedding.py` & `ExpoSeq-1.1.4/src/ExpoSeq/tidy_data/tidy_cluster_embedding.py`

 * *Files identical despite different names*

### Comparing `ExpoSeq-1.1.3/src/ExpoSeq/tidy_data/tidy_rel_sequence_abun.py` & `ExpoSeq-1.1.4/src/ExpoSeq/tidy_data/tidy_rel_sequence_abun.py`

 * *Files identical despite different names*

### Comparing `ExpoSeq-1.1.3/src/ExpoSeq/tidy_data/tidy_seqlogoPlot.py` & `ExpoSeq-1.1.4/src/ExpoSeq/tidy_data/tidy_seqlogoPlot.py`

 * *Files identical despite different names*

### Comparing `ExpoSeq-1.1.3/src/ExpoSeq/tidy_data/tidy_stacked_aa_distr.py` & `ExpoSeq-1.1.4/src/ExpoSeq/tidy_data/tidy_stacked_aa_distr.py`

 * *Files identical despite different names*

### Comparing `ExpoSeq-1.1.3/src/ExpoSeq.egg-info/PKG-INFO` & `ExpoSeq-1.1.4/src/ExpoSeq.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ExpoSeq
-Version: 1.1.3
+Version: 1.1.4
 Summary: A pacakge which provides various ways to analyze NGS data from phage display campaigns
 Home-page: https://github.com/nilshof01/ExpoSeq
 Author: Nils Hofmann
 Author-email: n.hofmann.99@web.de
 License: MIT
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
```

### Comparing `ExpoSeq-1.1.3/src/ExpoSeq.egg-info/SOURCES.txt` & `ExpoSeq-1.1.4/src/ExpoSeq.egg-info/SOURCES.txt`

 * *Files 1% similar despite different names*

```diff
@@ -46,14 +46,15 @@
 src/ExpoSeq/settings/global_vars.txt
 src/ExpoSeq/settings/legend_settings.txt
 src/ExpoSeq/settings/plot_styler.py
 src/ExpoSeq/settings/save_settings.txt
 src/ExpoSeq/test_data/__init__.py
 src/ExpoSeq/test_data/all_alignment_reports.pickle
 src/ExpoSeq/test_data/test_files/Chris_main_df.csv
+src/ExpoSeq/test_data/test_files/__init__.py
 src/ExpoSeq/test_data/test_files/binding_data.csv
 src/ExpoSeq/test_data/test_files/experiment_names.pickle
 src/ExpoSeq/test_data/test_files/sequencing_report.csv
 src/ExpoSeq/test_data/test_files/test1.fastq
 src/ExpoSeq/test_data/test_files/test2.fastq
 src/ExpoSeq/test_data/test_files/test3.fastq
 src/ExpoSeq/tidy_data/__init__.py
```

