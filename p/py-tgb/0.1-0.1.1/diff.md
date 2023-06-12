# Comparing `tmp/py-tgb-0.1.tar.gz` & `tmp/py_tgb-0.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "py-tgb-0.1.tar", last modified: Mon Jun 12 18:48:39 2023, max compression
+gzip compressed data, was "py_tgb-0.1.1.tar", max compression
```

## Comparing `py-tgb-0.1.tar` & `py_tgb-0.1.1.tar`

### file list

```diff
@@ -1,10 +1,31 @@
-drwxrwxrwx   0 andy      (1001) andy      (1001)        0 2023-06-12 18:48:39.233975 py-tgb-0.1/
--rwxrwxrwx   0 andy      (1001) andy      (1001)       48 2023-06-12 18:48:39.232976 py-tgb-0.1/PKG-INFO
--rwxrwxrwx   0 andy      (1001) andy      (1001)     1905 2023-05-31 13:03:27.000000 py-tgb-0.1/README.md
-drwxrwxrwx   0 andy      (1001) andy      (1001)        0 2023-06-12 18:48:39.232477 py-tgb-0.1/py_tgb.egg-info/
--rwxrwxrwx   0 andy      (1001) andy      (1001)       48 2023-06-12 18:48:39.000000 py-tgb-0.1/py_tgb.egg-info/PKG-INFO
--rwxrwxrwx   0 andy      (1001) andy      (1001)      138 2023-06-12 18:48:39.000000 py-tgb-0.1/py_tgb.egg-info/SOURCES.txt
--rwxrwxrwx   0 andy      (1001) andy      (1001)        1 2023-06-12 18:48:39.000000 py-tgb-0.1/py_tgb.egg-info/dependency_links.txt
--rwxrwxrwx   0 andy      (1001) andy      (1001)        1 2023-06-12 18:48:39.000000 py-tgb-0.1/py_tgb.egg-info/top_level.txt
--rwxrwxrwx   0 andy      (1001) andy      (1001)       38 2023-06-12 18:48:39.234476 py-tgb-0.1/setup.cfg
--rwxrwxrwx   0 andy      (1001) andy      (1001)      110 2023-06-12 18:48:16.000000 py-tgb-0.1/setup.py
+-rw-r--r--   0        0        0     1905 2023-06-12 18:33:10.179693 py_tgb-0.1.1/README.md
+-rw-r--r--   0        0        0      703 2023-06-12 19:25:39.195693 py_tgb-0.1.1/pyproject.toml
+-rw-r--r--   0        0        0      177 2023-06-12 18:33:10.199693 py_tgb-0.1.1/tgb/datasets/MAG/mag.py
+-rw-r--r--   0        0        0      820 2023-06-12 18:33:10.199693 py_tgb-0.1.1/tgb/datasets/MAG/old/plot_stats.py
+-rw-r--r--   0        0        0     4777 2023-06-12 18:33:10.199693 py_tgb-0.1.1/tgb/datasets/amazonreview/amazonreview.py
+-rw-r--r--   0        0        0     2499 2023-06-12 18:33:10.199693 py_tgb-0.1.1/tgb/datasets/amazonreview/amazonreview_neg_generator.py
+-rw-r--r--   0        0        0     7781 2023-06-12 18:33:10.199693 py_tgb-0.1.1/tgb/datasets/flight_raw/opensky.py
+-rw-r--r--   0        0        0    19780 2023-06-12 18:33:10.203693 py_tgb-0.1.1/tgb/datasets/lastfmGenre/lastfm.py
+-rw-r--r--   0        0        0     2518 2023-06-12 18:33:10.203693 py_tgb-0.1.1/tgb/datasets/opensky/opensky_neg_generator.py
+-rw-r--r--   0        0        0     6912 2023-06-12 18:33:10.203693 py_tgb-0.1.1/tgb/datasets/redditcomments/redditcomments.py
+-rw-r--r--   0        0        0     2501 2023-06-12 18:33:10.203693 py_tgb-0.1.1/tgb/datasets/redditcomments/redditcomments_neg_generator.py
+-rw-r--r--   0        0        0     4740 2023-06-12 18:33:10.203693 py_tgb-0.1.1/tgb/datasets/stablecoin/stablecoin.py
+-rw-r--r--   0        0        0     2497 2023-06-12 18:33:10.203693 py_tgb-0.1.1/tgb/datasets/stablecoin/stablecoin_neg_generator.py
+-rw-r--r--   0        0        0    11859 2023-06-12 18:33:10.203693 py_tgb-0.1.1/tgb/datasets/subreddits/subreddits.py
+-rw-r--r--   0        0        0     5927 2023-06-12 18:33:10.203693 py_tgb-0.1.1/tgb/datasets/un_trade/un_trade.py
+-rw-r--r--   0        0        0    14106 2023-06-12 18:33:10.203693 py_tgb-0.1.1/tgb/edgeregression/dataset.py
+-rw-r--r--   0        0        0     3992 2023-06-12 18:33:10.203693 py_tgb-0.1.1/tgb/edgeregression/dataset_pyg.py
+-rw-r--r--   0        0        0     5087 2023-06-12 18:33:10.203693 py_tgb-0.1.1/tgb/edgeregression/evaluate.py
+-rw-r--r--   0        0        0    13856 2023-06-12 18:33:10.203693 py_tgb-0.1.1/tgb/linkproppred/dataset.py
+-rw-r--r--   0        0        0     7293 2023-06-12 18:33:10.203693 py_tgb-0.1.1/tgb/linkproppred/dataset_pyg.py
+-rw-r--r--   0        0        0     4664 2023-06-12 18:33:10.203693 py_tgb-0.1.1/tgb/linkproppred/evaluate.py
+-rw-r--r--   0        0        0    10770 2023-06-12 18:33:10.207693 py_tgb-0.1.1/tgb/linkproppred/negative_generator.py
+-rw-r--r--   0        0        0     3903 2023-06-12 18:33:10.207693 py_tgb-0.1.1/tgb/linkproppred/negative_sampler.py
+-rw-r--r--   0        0        0    16249 2023-06-12 18:33:10.207693 py_tgb-0.1.1/tgb/nodeproppred/dataset.py
+-rw-r--r--   0        0        0     7205 2023-06-12 18:33:10.207693 py_tgb-0.1.1/tgb/nodeproppred/dataset_pyg.py
+-rw-r--r--   0        0        0     5334 2023-06-12 18:33:10.207693 py_tgb-0.1.1/tgb/nodeproppred/evaluate.py
+-rw-r--r--   0        0        0     1683 2023-06-12 18:33:10.207693 py_tgb-0.1.1/tgb/utils/info.py
+-rw-r--r--   0        0        0    27787 2023-06-12 18:33:10.207693 py_tgb-0.1.1/tgb/utils/pre_process.py
+-rw-r--r--   0        0        0     2905 2023-06-12 18:33:10.207693 py_tgb-0.1.1/tgb/utils/stats.py
+-rw-r--r--   0        0        0     2974 2023-06-12 18:33:10.207693 py_tgb-0.1.1/tgb/utils/utils.py
+-rw-r--r--   0        0        0     2600 1970-01-01 00:00:00.000000 py_tgb-0.1.1/PKG-INFO
```

### Comparing `py-tgb-0.1/README.md` & `py_tgb-0.1.1/README.md`

 * *Files identical despite different names*

