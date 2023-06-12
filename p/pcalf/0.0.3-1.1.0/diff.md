# Comparing `tmp/pcalf-0.0.3.tar.gz` & `tmp/pcalf-1.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pcalf-0.0.3.tar", last modified: Thu Apr 13 12:58:46 2023, max compression
+gzip compressed data, was "pcalf-1.1.0.tar", last modified: Mon Jun 12 06:28:11 2023, max compression
```

## Comparing `pcalf-0.0.3.tar` & `pcalf-1.1.0.tar`

### file list

```diff
@@ -1,41 +1,149 @@
-drwxr-xr-x   0 mmillet    (501) staff       (20)        0 2023-04-13 12:58:46.000000 pcalf-0.0.3/
--rw-r--r--   0 mmillet    (501) staff       (20)     1069 2023-04-13 11:29:34.000000 pcalf-0.0.3/LICENSE.txt
--rw-r--r--   0 mmillet    (501) staff       (20)       42 2023-04-13 08:49:42.000000 pcalf-0.0.3/MANIFEST.in
--rw-r--r--   0 mmillet    (501) staff       (20)     2340 2023-04-13 12:58:46.000000 pcalf-0.0.3/PKG-INFO
--rw-r--r--   0 mmillet    (501) staff       (20)     1854 2023-04-13 08:49:42.000000 pcalf-0.0.3/README.md
--rw-r--r--   0 mmillet    (501) staff       (20)       84 2023-04-13 11:28:33.000000 pcalf-0.0.3/pyproject.toml
-drwxr-xr-x   0 mmillet    (501) staff       (20)        0 2023-04-13 12:58:46.000000 pcalf-0.0.3/scripts/
--rw-r--r--   0 mmillet    (501) staff       (20)    13197 2023-04-13 12:45:06.000000 pcalf-0.0.3/scripts/pcalf
--rw-r--r--   0 mmillet    (501) staff       (20)       38 2023-04-13 12:58:46.000000 pcalf-0.0.3/setup.cfg
--rw-r--r--   0 mmillet    (501) staff       (20)     1181 2023-04-13 12:55:04.000000 pcalf-0.0.3/setup.py
-drwxr-xr-x   0 mmillet    (501) staff       (20)        0 2023-04-13 12:58:46.000000 pcalf-0.0.3/src/
-drwxr-xr-x   0 mmillet    (501) staff       (20)        0 2023-04-13 12:58:46.000000 pcalf-0.0.3/src/pcalf/
--rw-r--r--   0 mmillet    (501) staff       (20)        0 2023-04-13 12:43:28.000000 pcalf-0.0.3/src/pcalf/__init__.py
-drwxr-xr-x   0 mmillet    (501) staff       (20)        0 2023-04-13 12:58:46.000000 pcalf-0.0.3/src/pcalf/core/
--rw-r--r--   0 mmillet    (501) staff       (20)        0 2023-04-13 12:01:24.000000 pcalf-0.0.3/src/pcalf/core/__init__.py
--rw-r--r--   0 mmillet    (501) staff       (20)     7841 2023-04-13 08:49:42.000000 pcalf-0.0.3/src/pcalf/core/biohmm.py
--rw-r--r--   0 mmillet    (501) staff       (20)    17748 2023-04-13 08:49:42.000000 pcalf-0.0.3/src/pcalf/core/bioseq.py
--rw-r--r--   0 mmillet    (501) staff       (20)     1662 2023-04-13 08:49:42.000000 pcalf-0.0.3/src/pcalf/core/log.py
--rw-r--r--   0 mmillet    (501) staff       (20)    22688 2023-04-13 08:49:42.000000 pcalf-0.0.3/src/pcalf/core/search.py
-drwxr-xr-x   0 mmillet    (501) staff       (20)        0 2023-04-13 12:58:46.000000 pcalf-0.0.3/src/pcalf/datas/
--rw-r--r--   0 mmillet    (501) staff       (20)    29491 2023-04-13 08:49:42.000000 pcalf-0.0.3/src/pcalf/datas/Gly1.hmm
--rw-r--r--   0 mmillet    (501) staff       (20)     3440 2023-04-13 08:49:42.000000 pcalf-0.0.3/src/pcalf/datas/Gly1.msa.fa
--rw-r--r--   0 mmillet    (501) staff       (20)    28897 2023-04-13 08:49:42.000000 pcalf-0.0.3/src/pcalf/datas/Gly2.hmm
--rw-r--r--   0 mmillet    (501) staff       (20)     2819 2023-04-13 08:49:42.000000 pcalf-0.0.3/src/pcalf/datas/Gly2.msa.fa
--rw-r--r--   0 mmillet    (501) staff       (20)    27603 2023-04-13 08:49:42.000000 pcalf-0.0.3/src/pcalf/datas/Gly3.hmm
--rw-r--r--   0 mmillet    (501) staff       (20)     3674 2023-04-13 08:49:42.000000 pcalf-0.0.3/src/pcalf/datas/Gly3.msa.fa
--rw-r--r--   0 mmillet    (501) staff       (20)   106797 2023-04-13 08:49:42.000000 pcalf-0.0.3/src/pcalf/datas/GlyX3.hmm
--rw-r--r--   0 mmillet    (501) staff       (20)    11209 2023-04-13 08:49:42.000000 pcalf-0.0.3/src/pcalf/datas/GlyX3.msa.fa
--rw-r--r--   0 mmillet    (501) staff       (20)        0 2023-04-13 08:49:42.000000 pcalf-0.0.3/src/pcalf/datas/__init__.py
--rw-r--r--   0 mmillet    (501) staff       (20)      496 2023-04-13 08:49:42.000000 pcalf-0.0.3/src/pcalf/datas/accession.txt
--rw-r--r--   0 mmillet    (501) staff       (20)   192788 2023-04-13 08:49:42.000000 pcalf-0.0.3/src/pcalf/datas/all.hmm
--rw-r--r--   0 mmillet    (501) staff       (20)    12236 2023-04-13 08:49:42.000000 pcalf-0.0.3/src/pcalf/datas/nterdb.fasta
--rw-r--r--   0 mmillet    (501) staff       (20)     6003 2023-04-13 08:49:42.000000 pcalf-0.0.3/src/pcalf/datas/nterdb.ref.tsv
--rw-r--r--   0 mmillet    (501) staff       (20)     3188 2023-04-13 08:49:42.000000 pcalf-0.0.3/src/pcalf/datas/nterdb.tsv
-drwxr-xr-x   0 mmillet    (501) staff       (20)        0 2023-04-13 12:58:46.000000 pcalf-0.0.3/src/pcalf.egg-info/
--rw-r--r--   0 mmillet    (501) staff       (20)     2340 2023-04-13 12:58:45.000000 pcalf-0.0.3/src/pcalf.egg-info/PKG-INFO
--rw-r--r--   0 mmillet    (501) staff       (20)      796 2023-04-13 12:58:46.000000 pcalf-0.0.3/src/pcalf.egg-info/SOURCES.txt
--rw-r--r--   0 mmillet    (501) staff       (20)        1 2023-04-13 12:58:45.000000 pcalf-0.0.3/src/pcalf.egg-info/dependency_links.txt
--rw-r--r--   0 mmillet    (501) staff       (20)        1 2023-04-13 12:39:50.000000 pcalf-0.0.3/src/pcalf.egg-info/not-zip-safe
--rw-r--r--   0 mmillet    (501) staff       (20)       96 2023-04-13 12:58:46.000000 pcalf-0.0.3/src/pcalf.egg-info/requires.txt
--rw-r--r--   0 mmillet    (501) staff       (20)       10 2023-04-13 12:58:46.000000 pcalf-0.0.3/src/pcalf.egg-info/top_level.txt
+drwxr-xr-x   0 mmillet    (501) staff       (20)        0 2023-06-12 06:28:11.000000 pcalf-1.1.0/
+-rw-r--r--   0 mmillet    (501) staff       (20)     1069 2023-04-13 11:29:34.000000 pcalf-1.1.0/LICENSE.txt
+-rw-r--r--   0 mmillet    (501) staff       (20)       70 2023-04-28 08:11:35.000000 pcalf-1.1.0/MANIFEST.in
+-rw-r--r--   0 mmillet    (501) staff       (20)     8021 2023-06-12 06:28:11.000000 pcalf-1.1.0/PKG-INFO
+-rw-r--r--   0 mmillet    (501) staff       (20)     7555 2023-06-12 06:04:06.000000 pcalf-1.1.0/README.md
+-rw-r--r--   0 mmillet    (501) staff       (20)       84 2023-04-22 07:07:20.000000 pcalf-1.1.0/pyproject.toml
+drwxr-xr-x   0 mmillet    (501) staff       (20)        0 2023-06-12 06:28:10.000000 pcalf-1.1.0/scripts/
+-rw-r--r--   0 mmillet    (501) staff       (20)    12193 2023-06-08 07:19:44.000000 pcalf-1.1.0/scripts/pcalf
+-rw-r--r--   0 mmillet    (501) staff       (20)     8613 2023-06-08 07:19:44.000000 pcalf-1.1.0/scripts/pcalf-annotate-workflow
+-rw-r--r--   0 mmillet    (501) staff       (20)     4197 2023-06-08 07:19:44.000000 pcalf-1.1.0/scripts/pcalf-datasets-workflow
+-rw-r--r--   0 mmillet    (501) staff       (20)     1330 2023-06-12 06:17:48.000000 pcalf-1.1.0/scripts/pcalf-report
+-rw-r--r--   0 mmillet    (501) staff       (20)       38 2023-06-12 06:28:11.000000 pcalf-1.1.0/setup.cfg
+-rw-r--r--   0 mmillet    (501) staff       (20)     1238 2023-06-12 06:20:27.000000 pcalf-1.1.0/setup.py
+drwxr-xr-x   0 mmillet    (501) staff       (20)        0 2023-06-12 06:28:10.000000 pcalf-1.1.0/src/
+-rw-r--r--   0 mmillet    (501) staff       (20)     6148 2023-06-09 08:04:56.000000 pcalf-1.1.0/src/.DS_Store
+drwxr-xr-x   0 mmillet    (501) staff       (20)        0 2023-06-12 06:28:10.000000 pcalf-1.1.0/src/pcalf/
+-rw-r--r--   0 mmillet    (501) staff       (20)     8196 2023-06-09 09:07:00.000000 pcalf-1.1.0/src/pcalf/.DS_Store
+-rw-r--r--   0 mmillet    (501) staff       (20)        0 2023-04-13 12:43:28.000000 pcalf-1.1.0/src/pcalf/__init__.py
+drwxr-xr-x   0 mmillet    (501) staff       (20)        0 2023-06-12 06:28:10.000000 pcalf-1.1.0/src/pcalf/__pycache__/
+-rw-r--r--   0 mmillet    (501) staff       (20)      161 2023-04-13 14:59:36.000000 pcalf-1.1.0/src/pcalf/__pycache__/__init__.cpython-39.pyc
+drwxr-xr-x   0 mmillet    (501) staff       (20)        0 2023-06-12 06:28:10.000000 pcalf-1.1.0/src/pcalf/core/
+-rw-r--r--   0 mmillet    (501) staff       (20)     8938 2023-06-06 08:39:02.000000 pcalf-1.1.0/src/pcalf/core/PcalfDB.py
+-rw-r--r--   0 mmillet    (501) staff       (20)     2226 2023-04-21 21:26:25.000000 pcalf-1.1.0/src/pcalf/core/PcalfSnake.py
+-rw-r--r--   0 mmillet    (501) staff       (20)    23546 2023-03-23 08:39:39.000000 pcalf-1.1.0/src/pcalf/core/_HarleyReport.py
+-rw-r--r--   0 mmillet    (501) staff       (20)     1589 2023-03-25 07:55:52.000000 pcalf-1.1.0/src/pcalf/core/_PcalfIO.py
+-rw-r--r--   0 mmillet    (501) staff       (20)        0 2023-04-13 12:01:24.000000 pcalf-1.1.0/src/pcalf/core/__init__.py
+drwxr-xr-x   0 mmillet    (501) staff       (20)        0 2023-06-12 06:28:10.000000 pcalf-1.1.0/src/pcalf/core/__pycache__/
+-rw-r--r--   0 mmillet    (501) staff       (20)     9597 2023-06-05 15:00:06.000000 pcalf-1.1.0/src/pcalf/core/__pycache__/HarleyDB.cpython-39.pyc
+-rw-r--r--   0 mmillet    (501) staff       (20)     2246 2023-06-05 14:44:11.000000 pcalf-1.1.0/src/pcalf/core/__pycache__/HarleySnake.cpython-39.pyc
+-rw-r--r--   0 mmillet    (501) staff       (20)     9578 2023-06-12 06:07:26.000000 pcalf-1.1.0/src/pcalf/core/__pycache__/PcalfDB.cpython-39.pyc
+-rw-r--r--   0 mmillet    (501) staff       (20)     2245 2023-06-12 06:07:26.000000 pcalf-1.1.0/src/pcalf/core/__pycache__/PcalfSnake.cpython-39.pyc
+-rw-r--r--   0 mmillet    (501) staff       (20)      166 2023-06-12 06:07:21.000000 pcalf-1.1.0/src/pcalf/core/__pycache__/__init__.cpython-39.pyc
+-rw-r--r--   0 mmillet    (501) staff       (20)     7198 2023-06-12 06:07:21.000000 pcalf-1.1.0/src/pcalf/core/__pycache__/biohmm.cpython-39.pyc
+-rw-r--r--   0 mmillet    (501) staff       (20)    15516 2023-06-12 06:07:21.000000 pcalf-1.1.0/src/pcalf/core/__pycache__/bioseq.cpython-39.pyc
+-rw-r--r--   0 mmillet    (501) staff       (20)     1075 2023-06-12 06:07:22.000000 pcalf-1.1.0/src/pcalf/core/__pycache__/log.cpython-39.pyc
+-rw-r--r--   0 mmillet    (501) staff       (20)    15093 2023-06-05 07:19:44.000000 pcalf-1.1.0/src/pcalf/core/__pycache__/pcalf.cpython-39.pyc
+-rw-r--r--   0 mmillet    (501) staff       (20)    15102 2023-06-12 06:07:21.000000 pcalf-1.1.0/src/pcalf/core/__pycache__/search.cpython-39.pyc
+-rw-r--r--   0 mmillet    (501) staff       (20)    15095 2023-06-02 08:53:48.000000 pcalf-1.1.0/src/pcalf/core/__pycache__/search2.cpython-39.pyc
+-rw-r--r--   0 mmillet    (501) staff       (20)    24097 2023-05-30 14:42:58.000000 pcalf-1.1.0/src/pcalf/core/_bkpsearch.py
+-rw-r--r--   0 mmillet    (501) staff       (20)     8282 2023-04-25 13:41:20.000000 pcalf-1.1.0/src/pcalf/core/biohmm.py
+-rw-r--r--   0 mmillet    (501) staff       (20)    17320 2023-06-06 12:18:32.000000 pcalf-1.1.0/src/pcalf/core/bioseq.py
+-rw-r--r--   0 mmillet    (501) staff       (20)      993 2023-04-25 13:43:01.000000 pcalf-1.1.0/src/pcalf/core/log.py
+-rw-r--r--   0 mmillet    (501) staff       (20)     5153 2023-06-12 06:17:59.000000 pcalf-1.1.0/src/pcalf/core/pcalf_db_scheme.sql
+-rw-r--r--   0 mmillet    (501) staff       (20)    22642 2023-06-06 12:54:33.000000 pcalf-1.1.0/src/pcalf/core/search.py
+drwxr-xr-x   0 mmillet    (501) staff       (20)        0 2023-06-12 06:28:10.000000 pcalf-1.1.0/src/pcalf/datas/
+-rw-r--r--   0 mmillet    (501) staff       (20)    29491 2023-04-13 08:49:42.000000 pcalf-1.1.0/src/pcalf/datas/Gly1.hmm
+-rw-r--r--   0 mmillet    (501) staff       (20)     3440 2023-04-13 08:49:42.000000 pcalf-1.1.0/src/pcalf/datas/Gly1.msa.fa
+-rw-r--r--   0 mmillet    (501) staff       (20)    28897 2023-04-13 08:49:42.000000 pcalf-1.1.0/src/pcalf/datas/Gly2.hmm
+-rw-r--r--   0 mmillet    (501) staff       (20)     2819 2023-04-13 08:49:42.000000 pcalf-1.1.0/src/pcalf/datas/Gly2.msa.fa
+-rw-r--r--   0 mmillet    (501) staff       (20)    27603 2023-04-13 08:49:42.000000 pcalf-1.1.0/src/pcalf/datas/Gly3.hmm
+-rw-r--r--   0 mmillet    (501) staff       (20)     3674 2023-04-13 08:49:42.000000 pcalf-1.1.0/src/pcalf/datas/Gly3.msa.fa
+-rw-r--r--   0 mmillet    (501) staff       (20)   106797 2023-04-13 08:49:42.000000 pcalf-1.1.0/src/pcalf/datas/GlyX3.hmm
+-rw-r--r--   0 mmillet    (501) staff       (20)    11209 2023-04-13 08:49:42.000000 pcalf-1.1.0/src/pcalf/datas/GlyX3.msa.fa
+-rw-r--r--   0 mmillet    (501) staff       (20)        0 2023-04-13 08:49:42.000000 pcalf-1.1.0/src/pcalf/datas/__init__.py
+drwxr-xr-x   0 mmillet    (501) staff       (20)        0 2023-06-12 06:28:10.000000 pcalf-1.1.0/src/pcalf/datas/__pycache__/
+-rw-r--r--   0 mmillet    (501) staff       (20)      167 2023-04-17 05:28:29.000000 pcalf-1.1.0/src/pcalf/datas/__pycache__/__init__.cpython-39.pyc
+-rw-r--r--   0 mmillet    (501) staff       (20)      496 2023-04-13 08:49:42.000000 pcalf-1.1.0/src/pcalf/datas/accession.txt
+-rw-r--r--   0 mmillet    (501) staff       (20)   192788 2023-04-13 08:49:42.000000 pcalf-1.1.0/src/pcalf/datas/all.hmm
+-rw-r--r--   0 mmillet    (501) staff       (20)    12236 2023-04-13 08:49:42.000000 pcalf-1.1.0/src/pcalf/datas/nterdb.fasta
+-rw-r--r--   0 mmillet    (501) staff       (20)     6003 2023-04-13 08:49:42.000000 pcalf-1.1.0/src/pcalf/datas/nterdb.ref.tsv
+-rw-r--r--   0 mmillet    (501) staff       (20)     3188 2023-04-13 08:49:42.000000 pcalf-1.1.0/src/pcalf/datas/nterdb.tsv
+drwxr-xr-x   0 mmillet    (501) staff       (20)        0 2023-06-12 06:28:10.000000 pcalf-1.1.0/src/pcalf/report/
+drwxr-xr-x   0 mmillet    (501) staff       (20)        0 2023-06-12 06:28:11.000000 pcalf-1.1.0/src/pcalf/report/.ipynb_checkpoints/
+-rw-r--r--   0 mmillet    (501) staff       (20)  1158450 2023-06-08 13:25:54.000000 pcalf-1.1.0/src/pcalf/report/.ipynb_checkpoints/Report-checkpoint.ipynb
+-rw-r--r--   0 mmillet    (501) staff       (20)  1182597 2023-06-09 08:06:06.000000 pcalf-1.1.0/src/pcalf/report/Report.ipynb
+-rw-r--r--   0 mmillet    (501) staff       (20)        0 2023-05-02 06:26:00.000000 pcalf-1.1.0/src/pcalf/report/__init__.py
+drwxr-xr-x   0 mmillet    (501) staff       (20)        0 2023-06-12 06:28:11.000000 pcalf-1.1.0/src/pcalf/report/__pycache__/
+-rw-r--r--   0 mmillet    (501) staff       (20)      168 2023-06-12 06:13:04.000000 pcalf-1.1.0/src/pcalf/report/__pycache__/__init__.cpython-39.pyc
+-rw-r--r--   0 mmillet    (501) staff       (20)    17744 2023-06-12 06:13:04.000000 pcalf-1.1.0/src/pcalf/report/__pycache__/render.cpython-39.pyc
+-rw-r--r--   0 mmillet    (501) staff       (20)    79976 2023-06-12 06:04:06.000000 pcalf-1.1.0/src/pcalf/report/pcalf.svg
+-rw-r--r--   0 mmillet    (501) staff       (20)    25860 2023-06-12 06:04:06.000000 pcalf-1.1.0/src/pcalf/report/render.py
+-rw-r--r--   0 mmillet    (501) staff       (20)    71713 2023-06-09 08:00:16.000000 pcalf-1.1.0/src/pcalf/report/template.css
+-rw-r--r--   0 mmillet    (501) staff       (20)    19121 2023-06-09 08:04:40.000000 pcalf-1.1.0/src/pcalf/report/template.html
+-rw-r--r--   0 mmillet    (501) staff       (20)    23654 2023-06-09 08:01:24.000000 pcalf-1.1.0/src/pcalf/report/template.js
+-rw-r--r--   0 mmillet    (501) staff       (20) 25809227 2023-06-09 08:04:56.000000 pcalf-1.1.0/src/pcalf/report/test.html
+drwxr-xr-x   0 mmillet    (501) staff       (20)        0 2023-06-12 06:28:11.000000 pcalf-1.1.0/src/pcalf/workflow/
+-rw-r--r--   0 mmillet    (501) staff       (20)    10244 2023-04-22 07:44:56.000000 pcalf-1.1.0/src/pcalf/workflow/.DS_Store
+drwxr-xr-x   0 mmillet    (501) staff       (20)        0 2023-06-12 06:28:11.000000 pcalf-1.1.0/src/pcalf/workflow/.ipynb_checkpoints/
+-rw-r--r--   0 mmillet    (501) staff       (20)    34112 2023-04-28 09:41:00.000000 pcalf-1.1.0/src/pcalf/workflow/.ipynb_checkpoints/Report-checkpoint.ipynb
+drwxr-xr-x   0 mmillet    (501) staff       (20)        0 2023-06-12 06:28:11.000000 pcalf-1.1.0/src/pcalf/workflow/__pycache__/
+-rw-r--r--   0 mmillet    (501) staff       (20)     9601 2023-04-25 18:01:24.000000 pcalf-1.1.0/src/pcalf/workflow/__pycache__/HarleyDB.cpython-39.pyc
+-rw-r--r--   0 mmillet    (501) staff       (20)     1894 2023-04-13 15:00:02.000000 pcalf-1.1.0/src/pcalf/workflow/__pycache__/HarleyIO.cpython-39.pyc
+-rw-r--r--   0 mmillet    (501) staff       (20)     2250 2023-04-21 22:17:26.000000 pcalf-1.1.0/src/pcalf/workflow/__pycache__/HarleySnake.cpython-39.pyc
+drwxr-xr-x   0 mmillet    (501) staff       (20)        0 2023-06-12 06:28:11.000000 pcalf-1.1.0/src/pcalf/workflow/annotate/
+-rw-r--r--   0 mmillet    (501) staff       (20)     8196 2023-04-12 05:29:59.000000 pcalf-1.1.0/src/pcalf/workflow/annotate/.DS_Store
+-rw-r--r--   0 mmillet    (501) staff       (20)     1712 2023-04-25 09:05:13.000000 pcalf-1.1.0/src/pcalf/workflow/annotate/Snakefile
+-rw-r--r--   0 mmillet    (501) staff       (20)        0 2023-03-22 07:27:01.000000 pcalf-1.1.0/src/pcalf/workflow/annotate/__init__.py
+drwxr-xr-x   0 mmillet    (501) staff       (20)        0 2023-06-12 06:28:11.000000 pcalf-1.1.0/src/pcalf/workflow/annotate/__pycache__/
+-rw-r--r--   0 mmillet    (501) staff       (20)      179 2023-06-12 06:07:26.000000 pcalf-1.1.0/src/pcalf/workflow/annotate/__pycache__/__init__.cpython-39.pyc
+drwxr-xr-x   0 mmillet    (501) staff       (20)        0 2023-06-12 06:28:11.000000 pcalf-1.1.0/src/pcalf/workflow/annotate/config/
+-rw-r--r--   0 mmillet    (501) staff       (20)     6148 2023-03-14 14:02:53.000000 pcalf-1.1.0/src/pcalf/workflow/annotate/config/.DS_Store
+-rw-r--r--   0 mmillet    (501) staff       (20)      553 2023-04-26 04:06:18.000000 pcalf-1.1.0/src/pcalf/workflow/annotate/config/config.yaml
+drwxr-xr-x   0 mmillet    (501) staff       (20)        0 2023-06-12 06:28:11.000000 pcalf-1.1.0/src/pcalf/workflow/annotate/envs/
+-rw-r--r--   0 mmillet    (501) staff       (20)     6148 2023-04-12 05:29:53.000000 pcalf-1.1.0/src/pcalf/workflow/annotate/envs/.DS_Store
+-rw-r--r--   0 mmillet    (501) staff       (20)      129 2023-02-08 20:05:34.000000 pcalf-1.1.0/src/pcalf/workflow/annotate/envs/biopython_1.79.yaml
+-rw-r--r--   0 mmillet    (501) staff       (20)      135 2023-03-14 10:20:07.000000 pcalf-1.1.0/src/pcalf/workflow/annotate/envs/checkm.yaml
+-rw-r--r--   0 mmillet    (501) staff       (20)      230 2023-02-09 17:17:11.000000 pcalf-1.1.0/src/pcalf/workflow/annotate/envs/gtdbtk_2.1.yaml
+-rw-r--r--   0 mmillet    (501) staff       (20)      252 2023-04-21 15:22:02.000000 pcalf-1.1.0/src/pcalf/workflow/annotate/envs/ncbi_dataset_14.14.0.yaml
+drwxr-xr-x   0 mmillet    (501) staff       (20)        0 2023-06-12 06:28:11.000000 pcalf-1.1.0/src/pcalf/workflow/annotate/rules/
+-rw-r--r--   0 mmillet    (501) staff       (20)     6148 2023-04-12 11:13:52.000000 pcalf-1.1.0/src/pcalf/workflow/annotate/rules/.DS_Store
+-rw-r--r--   0 mmillet    (501) staff       (20)     7958 2023-04-22 06:50:08.000000 pcalf-1.1.0/src/pcalf/workflow/annotate/rules/checkm.smk
+-rw-r--r--   0 mmillet    (501) staff       (20)     3802 2023-04-22 06:50:53.000000 pcalf-1.1.0/src/pcalf/workflow/annotate/rules/gtdbtk.smk
+-rw-r--r--   0 mmillet    (501) staff       (20)    14816 2023-03-25 09:42:50.000000 pcalf-1.1.0/src/pcalf/workflow/annotate/rules/gtdbtk_by_batch.smk
+-rw-r--r--   0 mmillet    (501) staff       (20)      981 2023-04-24 07:21:03.000000 pcalf-1.1.0/src/pcalf/workflow/annotate/rules/ncbi_metadatas.smk
+-rw-r--r--   0 mmillet    (501) staff       (20)     8423 2023-06-08 11:11:38.000000 pcalf-1.1.0/src/pcalf/workflow/annotate/rules/pcalf.smk
+drwxr-xr-x   0 mmillet    (501) staff       (20)        0 2023-06-12 06:28:11.000000 pcalf-1.1.0/src/pcalf/workflow/annotate/scripts/
+-rw-r--r--   0 mmillet    (501) staff       (20)     6148 2023-03-14 14:02:13.000000 pcalf-1.1.0/src/pcalf/workflow/annotate/scripts/.DS_Store
+-rw-r--r--   0 mmillet    (501) staff       (20)     8201 2023-06-06 15:04:17.000000 pcalf-1.1.0/src/pcalf/workflow/annotate/scripts/ncbi_metadatas.py
+drwxr-xr-x   0 mmillet    (501) staff       (20)        0 2023-06-12 06:28:11.000000 pcalf-1.1.0/src/pcalf/workflow/datasets/
+-rw-r--r--   0 mmillet    (501) staff       (20)     8196 2023-04-12 05:29:03.000000 pcalf-1.1.0/src/pcalf/workflow/datasets/.DS_Store
+-rw-r--r--   0 mmillet    (501) staff       (20)      741 2023-06-05 12:37:32.000000 pcalf-1.1.0/src/pcalf/workflow/datasets/Snakefile
+-rw-r--r--   0 mmillet    (501) staff       (20)        0 2023-03-22 07:27:01.000000 pcalf-1.1.0/src/pcalf/workflow/datasets/__init__.py
+drwxr-xr-x   0 mmillet    (501) staff       (20)        0 2023-06-12 06:28:11.000000 pcalf-1.1.0/src/pcalf/workflow/datasets/__pycache__/
+-rw-r--r--   0 mmillet    (501) staff       (20)      165 2023-06-12 06:04:06.000000 pcalf-1.1.0/src/pcalf/workflow/datasets/__pycache__/__init__.cpython-39.pyc
+drwxr-xr-x   0 mmillet    (501) staff       (20)        0 2023-06-12 06:28:11.000000 pcalf-1.1.0/src/pcalf/workflow/datasets/config/
+-rw-r--r--   0 mmillet    (501) staff       (20)     6148 2023-03-14 14:02:53.000000 pcalf-1.1.0/src/pcalf/workflow/datasets/config/.DS_Store
+-rw-r--r--   0 mmillet    (501) staff       (20)      169 2023-04-12 10:10:19.000000 pcalf-1.1.0/src/pcalf/workflow/datasets/config/config.yaml
+drwxr-xr-x   0 mmillet    (501) staff       (20)        0 2023-06-12 06:28:11.000000 pcalf-1.1.0/src/pcalf/workflow/datasets/envs/
+-rw-r--r--   0 mmillet    (501) staff       (20)     6148 2023-04-12 05:28:48.000000 pcalf-1.1.0/src/pcalf/workflow/datasets/envs/.DS_Store
+-rw-r--r--   0 mmillet    (501) staff       (20)      129 2023-02-08 20:05:34.000000 pcalf-1.1.0/src/pcalf/workflow/datasets/envs/biopython_1.79.yaml
+-rw-r--r--   0 mmillet    (501) staff       (20)      174 2023-03-14 10:20:07.000000 pcalf-1.1.0/src/pcalf/workflow/datasets/envs/ncbi_dataset_14.14.0.yaml
+-rw-r--r--   0 mmillet    (501) staff       (20)      199 2023-03-14 15:33:00.000000 pcalf-1.1.0/src/pcalf/workflow/datasets/envs/ngd.yaml
+-rw-r--r--   0 mmillet    (501) staff       (20)      141 2023-02-08 20:05:34.000000 pcalf-1.1.0/src/pcalf/workflow/datasets/envs/prodigal-2.6.yaml
+-rw-r--r--   0 mmillet    (501) staff       (20)      154 2023-03-14 10:20:07.000000 pcalf-1.1.0/src/pcalf/workflow/datasets/envs/seqkit.yaml
+drwxr-xr-x   0 mmillet    (501) staff       (20)        0 2023-06-12 06:28:11.000000 pcalf-1.1.0/src/pcalf/workflow/datasets/rules/
+-rw-r--r--   0 mmillet    (501) staff       (20)     6148 2023-04-12 05:29:03.000000 pcalf-1.1.0/src/pcalf/workflow/datasets/rules/.DS_Store
+-rw-r--r--   0 mmillet    (501) staff       (20)     4356 2023-06-05 12:54:47.000000 pcalf-1.1.0/src/pcalf/workflow/datasets/rules/download.smk
+-rw-r--r--   0 mmillet    (501) staff       (20)     5331 2023-06-05 12:55:21.000000 pcalf-1.1.0/src/pcalf/workflow/datasets/rules/fetch.smk
+-rw-r--r--   0 mmillet    (501) staff       (20)     3557 2023-06-05 12:18:45.000000 pcalf-1.1.0/src/pcalf/workflow/datasets/rules/translate.smk
+drwxr-xr-x   0 mmillet    (501) staff       (20)        0 2023-06-12 06:28:11.000000 pcalf-1.1.0/src/pcalf/workflow/datasets/scripts/
+-rw-r--r--   0 mmillet    (501) staff       (20)     6148 2023-04-12 05:29:03.000000 pcalf-1.1.0/src/pcalf/workflow/datasets/scripts/.DS_Store
+drwxr-xr-x   0 mmillet    (501) staff       (20)        0 2023-06-12 06:28:11.000000 pcalf-1.1.0/src/pcalf/workflow/datasets/scripts/__pycache__/
+-rw-r--r--   0 mmillet    (501) staff       (20)     5644 2023-03-15 07:56:31.000000 pcalf-1.1.0/src/pcalf/workflow/datasets/scripts/__pycache__/gimme_taxa.cpython-39.pyc
+-rw-r--r--   0 mmillet    (501) staff       (20)     1840 2023-03-14 19:35:29.000000 pcalf-1.1.0/src/pcalf/workflow/datasets/scripts/__pycache__/utils.cpython-39.pyc
+-rw-r--r--   0 mmillet    (501) staff       (20)     3085 2023-03-16 20:52:40.000000 pcalf-1.1.0/src/pcalf/workflow/datasets/scripts/datas.py
+-rw-r--r--   0 mmillet    (501) staff       (20)     4227 2023-03-25 10:16:37.000000 pcalf-1.1.0/src/pcalf/workflow/datasets/scripts/fallback.py
+-rw-r--r--   0 mmillet    (501) staff       (20)     2233 2023-03-16 12:37:36.000000 pcalf-1.1.0/src/pcalf/workflow/datasets/scripts/get_assemblies.py
+-rw-r--r--   0 mmillet    (501) staff       (20)     4629 2023-03-15 20:10:28.000000 pcalf-1.1.0/src/pcalf/workflow/datasets/scripts/get_ncbi_reports.py
+-rwxr-xr-x   0 mmillet    (501) staff       (20)     6473 2023-02-08 20:05:34.000000 pcalf-1.1.0/src/pcalf/workflow/datasets/scripts/gimme_taxa.py
+-rwxr-xr-x   0 mmillet    (501) staff       (20)     1464 2023-02-09 17:17:11.000000 pcalf-1.1.0/src/pcalf/workflow/datasets/scripts/log.py
+-rw-r--r--   0 mmillet    (501) staff       (20)     1241 2023-03-14 15:27:24.000000 pcalf-1.1.0/src/pcalf/workflow/datasets/scripts/taxid_children.py
+-rw-r--r--   0 mmillet    (501) staff       (20)     1515 2023-02-09 21:49:17.000000 pcalf-1.1.0/src/pcalf/workflow/datasets/scripts/utils.py
+drwxr-xr-x   0 mmillet    (501) staff       (20)        0 2023-06-12 06:28:10.000000 pcalf-1.1.0/src/pcalf.egg-info/
+-rw-r--r--   0 mmillet    (501) staff       (20)     8021 2023-06-12 06:28:10.000000 pcalf-1.1.0/src/pcalf.egg-info/PKG-INFO
+-rw-r--r--   0 mmillet    (501) staff       (20)     4632 2023-06-12 06:28:10.000000 pcalf-1.1.0/src/pcalf.egg-info/SOURCES.txt
+-rw-r--r--   0 mmillet    (501) staff       (20)        1 2023-06-12 06:28:10.000000 pcalf-1.1.0/src/pcalf.egg-info/dependency_links.txt
+-rw-r--r--   0 mmillet    (501) staff       (20)        1 2023-04-13 12:39:50.000000 pcalf-1.1.0/src/pcalf.egg-info/not-zip-safe
+-rw-r--r--   0 mmillet    (501) staff       (20)      133 2023-06-12 06:28:10.000000 pcalf-1.1.0/src/pcalf.egg-info/requires.txt
+-rw-r--r--   0 mmillet    (501) staff       (20)       10 2023-06-12 06:28:10.000000 pcalf-1.1.0/src/pcalf.egg-info/top_level.txt
```

### Comparing `pcalf-0.0.3/LICENSE.txt` & `pcalf-1.1.0/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `pcalf-0.0.3/scripts/pcalf` & `pcalf-1.1.0/scripts/pcalf`

 * *Files 13% similar despite different names*

```diff
@@ -1,88 +1,66 @@
 #!/usr/bin/env python3
 # -*- coding: utf-8 -*-
-"""
-        
-               _ (.".) _    
-              '-'/. .\'-'   
-    pcalf      ( o o )     
-                 `"-"`  jgs    
-
-
-        pcalf stand for python CALcyanin Finder
-        The calcyanin protein will be search and annotated within your input file(s) following three steps:
-            1) the glycine triplication specific of calcyanin will be searched using a specific HMM profile.
-            2) glycine zipper will be annotated individually using specifics HMM models for sequences with a glycine triplication.
-            3) the N-ter extremity of sequences with a glyX3 will be annotated using blastp and known n-ter as subject database.
-"""
 
 
 import argparse
 import gzip
 import os
 import sys
 import shutil
 import logging
 import multiprocessing
 from importlib import resources
 import pandas as pd
 
 
-import pcalf.datas
+import pcalf.datas as datas
 from pcalf.core import search,bioseq,biohmm,log
 
 
-logging.basicConfig(
-    format="%(asctime)s [%(threadName)-12.12s] [%(levelname)-5.5s]  %(message)s",
-    level=logging.INFO,
-    handlers=[]
-)
-
-DATASDIR = os.path.join(resources.files(pcalf.datas))
+DATASDIR = os.path.join(resources.files(datas))
 
 def get_args():
     parser = argparse.ArgumentParser(
-        description="""pcalf
-                        
-    pcalf stand for Python CALcyanin Finder
-
-    The input fasta file(s) will be scanned following three steps:
-    - First a specific HMM profile of the glycine triplication is searched using HMMSEARCH and only sequence with a hit above coverage and E-value threshold are retained.
-    - Secondly, those sequences are more precisely annotated using specifics HMM profiles for each glycine zipper in order to define their modular organization for their C-ter extremity.
-    - Finally, a set of known N-ter is blasted against them and the nearest neighbor is retained as (potential) N-ter type.
-    
+        description="""                        
+    pcalf 
+    Search calcyanin protein in one or multiple files containing CDS.
     """,
         formatter_class= argparse.RawTextHelpFormatter
     )
     parser.add_argument('-i','--input', dest='input', 
                         type = str, default=None,
                         help="Either a fasta file [gzip supported] or a tabular file with one file \"designation\tfile path\" per line.")
                                   
     parser.add_argument('-o', dest='res_dir', type=str, required=True,
                         help='Output directory. pcalf will ouput several files including updated HMMs and MSAs, a feature table and a summary.')   
 
-    parser.add_argument('--max-iteration', type=int, default = 1,
-                        help="Number of iteration.")
-
     parser.add_argument('--iterative-update', action="store_true",
                         help="If set, HMM profiles will be updated by aligning one sequence by one sequence. ")
 
     parser.add_argument('--glyx3-msa', dest = 'glyx3_msa', 
                         default = DATASDIR + "/GlyX3.msa.fa", 
                         help='Path to GlyX3 msa (default: %(default)s). A weighted HMM will be built from it.')                                     
 
-    parser.add_argument('--domz', dest='domz', type=int, default=10000,
-                        help='Sequence space size for hmmsearch (default: %(default)s).')     
+    parser.add_argument('-Z', dest='Z', type=int, default=None,
+                        help='The effective number of comparisons done, for E-value calculation.\
+                            Leave as None to auto-detect by counting the number of sequences queried.\
+                            (default: %(default)s).') 
+
+    parser.add_argument('--domZ', dest='domZ', type=int, default=None,
+                        help='The number of significant sequences found, for domain E-value calculation.\
+                            Leave as None to auto-detect by counting the number of sequences reported. \
+                            (default: %(default)s).')     
 
     parser.add_argument('--glyx3-coverage', dest='glyx3_coverage_threshold', 
                         type=float,default=0.6,
                         help="Minimal coverage (default: %(default)s)." )
     
     parser.add_argument('--glyx3-evalue', dest='glyx3_evalue_threshold', 
-                        type=float,default=1e-21,
+                        type=float,default=1e-20,
                         help="Glyx3 E-value when considering Glyx3 Hits (default: %(default)s).")
                         
     parser.add_argument('--gly1-msa', dest = 'gly1_msa', 
                         default = DATASDIR + "/Gly1.msa.fa", 
                         help='Path to GlyZip1 msa (default: %(default)s). A weighted HMM will be built from it.' )
 
     parser.add_argument('--gly2-msa', dest = 'gly2_msa', 
@@ -90,15 +68,15 @@
                         help='path to GlyZip2 msa (default: %(default)s). A weighted HMM will be built from it.')
 
     parser.add_argument('--gly3-msa', dest = 'gly3_msa', 
                         default = DATASDIR + "/Gly3.msa.fa", 
                         help='path to GlyZip3 msa (default: %(default)s). A weighted HMM will be built from it.')                        
 
     parser.add_argument('--glyzip-E-value', dest='glyzip_e_evalue', 
-                        type=float,default=3.6e-4,
+                        type=float,default=1e-10,
                         help = "Glyzip E-evalue when considering Gly(1|2|3) Hits (default: %(default)s)." )
     parser.add_argument('--glyzip-coverage', dest='glyzip_coverage', 
                         type=float,default=0.7,
                         help = "Glyzip coverage threshold when considering Gly(1|2|3) Hits (default: %(default)s)." )
     
     parser.add_argument('--nterdb', dest='nterdb', 
                         default = DATASDIR + "/nterdb.ref.tsv", 
@@ -126,56 +104,55 @@
     args = parser.parse_args()
     
     return args
 
 
 def main():
     args = get_args()
-
+    logger = logging.getLogger()
     # Setup Logger and Handlers
     level = logging.INFO
     if args.debug:
         level = logging.DEBUG
+    logger.setLevel(level)
     if not args.quiet:
-        console = logging.StreamHandler()
-        console.setLevel(level)
+        console = logging.StreamHandler()        
         console.setFormatter(log.CustomFormatter())
-        logging.getLogger('').addHandler(
+        console.setLevel(level)
+        logger.addHandler(
             console
         )
     if args.log:
         os.makedirs(os.path.dirname(os.path.abspath(args.log)),exist_ok=True)
         fhandler = logging.FileHandler(args.log)
         fhandler.setLevel(level)
         fhandler.setFormatter(log.CustomFormatter())
-        logging.getLogger('').addHandler(
+        logger.addHandler(
             fhandler
         )
     
+    logger.info("PCALF")
+    logger.debug("DEBUG")
+
     if not shutil.which("blastp"):
-        logging.error("blast not found, please, considere installing it using conda install -c bioconda blast.")
+        logger.error("blast not found, please, considere installing it using conda install -c bioconda blast.")
         exit(-1)
     else:
-        logging.debug("blastp found : {}".format(shutil.which("blastp")))
-
+        logger.debug("blastp found : {}".format(shutil.which("blastp")))
+    
+    
     res_dir = os.path.abspath(args.res_dir)
-
     if os.path.exists(res_dir):
         if args.force:
-            logging.debug("{} directory have been removed because of the --force flag.".format(res_dir))
+            logger.debug("{} directory have been removed because of the --force flag.".format(res_dir))
             shutil.rmtree(res_dir)            
         else:
-            logging.error("Output directory already exist , Bye !")
+            logger.error("Output directory already exist , Bye !")
             exit(-1)
     
-
-    # if (args.fasta and args.input) or (not args.fasta and not args.input) :
-    #     logging.error("Please choose one between --fasta and --input-file...")
-    #     exit(-1)
-
     fastas = []
     names = []
     if not args.input.endswith(".gz"): 
         with open(args.input,'r') as stream:   
             for line in stream.readlines():
                 # Check if not a fasta file
                 if not line.startswith(">"):
@@ -186,99 +163,103 @@
                     fastas.append(args.input)
                     names.append(os.path.basename(args.input))
                     break
     else: 
         with gzip.open(args.input ,'rt') as stream:
             for line in stream.readlines():                
                 if not line.startswith(">"): # Not a fasta file
-                    logging.error("{} is not a fasta file.".format(args.input))
+                    logger.error("{} is not a fasta file.".format(args.input))
                 else: # fasta file 
                     fastas.append(args.input)
                     names.append(os.path.basename(args.input))
                     break
 
 
-    logging.info("Init HMMs from MSAs.")    
+    logger.info("Init HMMs from MSAs.")    
     glyx3 = biohmm.Hmm("Glyx3",args.glyx3_msa)
     gly1 = biohmm.Hmm("Gly1",args.gly1_msa)
     gly2 = biohmm.Hmm("Gly2",args.gly2_msa)
     gly3 = biohmm.Hmm("Gly3",args.gly3_msa)
     
-    logging.info("Increase Glycine weight.")
+    logger.info("Increase Glycine weight.")
     glyx3.hmm = search.increase_glycine_weight( glyx3,0.2 )
     gly1.hmm  = search.increase_glycine_weight( gly1,0.2 )
     gly2.hmm  = search.increase_glycine_weight( gly2,0.2 )
     gly3.hmm  = search.increase_glycine_weight( gly3,0.2 )
 
-
-    logging.info("Init N-Ter DB.")
+    logger.info("Init N-Ter DB.")
     nterdb = search.parse_nterdb(args.nterdb)
     
     # Initital number of sequences.
     _glyx3_nseq = glyx3.hmm.nseq
     _gly1_nseq = gly1.hmm.nseq
     _gly2_nseq = gly2.hmm.nseq
     _gly3_nseq = gly3.hmm.nseq
 
-    logging.info("Start search.")
-    calseq , u_glyx3 , u_gly1, u_gly2 , u_gly3 , u_nter , seq_per_iteration = search.search(
-        res_dir,
+    logger.info("Start search.")
+    calseq , u_glyx3 , u_gly1, u_gly2 , u_gly3 , u_nter = search.pcalf(
+        #res_dir,
         fastas,
         names,
         glyx3,
         gly1,
         gly2,
         gly3,
-        nterdb,        
-        domz = args.domz,
+        nterdb, 
+        Z = args.Z,       
+        domZ = args.domZ,
         glyx3_evalue_threshold=args.glyx3_evalue_threshold,  
         glyx3_coverage_threshold=args.glyx3_coverage_threshold,  
         glyzip_evalue_threshold= args.glyzip_e_evalue,
         glyzip_coverage_threshold = args.glyzip_coverage,
         nter_coverage_threshold = args.nter_coverage, 
         nter_evalue_threshold  =  args.nter_evalue,
-        max_iteration=args.max_iteration, 
         is_update_iterative=args.iterative_update,
     )
    
-    logging.info("The search is over.")
+    logger.info("The search is over.")
 
-    logging.info("# Number of calcyanin detected : {}".format(len(calseq.sequences)))
-    logging.info("# N_seqs within Glyx3 HMM : {} [+{}]".format(u_glyx3.hmm.nseq, u_glyx3.hmm.nseq -  _glyx3_nseq))
-    logging.info("# N_seqs within Gly1 HMM : {} [+{}]".format(u_gly1.hmm.nseq, u_gly1.hmm.nseq - _gly1_nseq))
-    logging.info("# N_seqs within Gly2 HMM : {} [+{}]".format(u_gly2.hmm.nseq, u_gly2.hmm.nseq - _gly2_nseq))
-    logging.info("# N_seqs within Gly3 HMM : {} [+{}]".format(u_gly3.hmm.nseq, u_gly3.hmm.nseq - _gly3_nseq))
+    logger.info("# N_seqs within Glyx3 HMM : {} [+{}]".format(
+        u_glyx3.hmm.nseq, u_glyx3.hmm.nseq -  _glyx3_nseq))
+    logger.info("# N_seqs within Gly1 HMM : {} [+{}]".format(
+        u_gly1.hmm.nseq, u_gly1.hmm.nseq - _gly1_nseq))
+    logger.info("# N_seqs within Gly2 HMM : {} [+{}]".format(
+        u_gly2.hmm.nseq, u_gly2.hmm.nseq - _gly2_nseq))
+    logger.info("# N_seqs within Gly3 HMM : {} [+{}]".format(
+        u_gly3.hmm.nseq, u_gly3.hmm.nseq - _gly3_nseq))
     
-    logging.info("Dumping HMMs.") 
+    logger.info("Dumping HMMs.") 
     hmmdir = os.path.join(res_dir,"HMM")
     os.makedirs(hmmdir,exist_ok=True)
     u_glyx3.hmm.write(open(hmmdir + "/Glyx3.hmm","wb"))
     u_gly1.hmm.write(open(hmmdir + "/Gly1.hmm","wb"))
     u_gly2.hmm.write(open(hmmdir + "/Gly2.hmm","wb"))
     u_gly3.hmm.write(open(hmmdir + "/Gly3.hmm","wb"))
 
-    logging.info("Dumping MSAs.")
-    msadir = os.path.join(res_dir,"MSA")
+    logger.info("Dumping MSAs.")
+    msadir = os.path.join(res_dir,"MSA")    
     os.makedirs(msadir,exist_ok=True)
     u_glyx3.msa.write(open(msadir+"/Glyx3.msa.fa","wb"),format="afa")
     u_gly1.msa.write(open(msadir+"/Gly1.msa.fa","wb"),format="afa")
     u_gly2.msa.write(open(msadir+"/Gly2.msa.fa","wb"),format="afa")
     u_gly3.msa.write(open(msadir+"/Gly3.msa.fa","wb"),format="afa")
     
-    logging.info("Dumping N-ter table.")
+    logger.info("Dumping N-ter table.")
     with open(res_dir+"/N-ter-DB.tsv","w") as nterout:
         for nterid, n in u_nter.items():
             nterout.write("{}\t{}\t{}\n".format(n[0],nterid,n[1]))
 
-    logging.info("Dumping feature table.")
+    logger.info("Write feature table.")
     features = calseq.to_feature_table()
     features.to_csv(res_dir + "/pcalf.features.tsv",sep="\t",header=True,index=True)
-    
+    logger.info("Write hits table")
+    hits = calseq.to_hits_table()
+    hits.to_csv(res_dir + "/pcalf.hits.tsv",sep="\t",header=True,index=True)
 
-    logging.info("Make summary.")
+    logger.info("Make summary.")
     summary_datas = []
     for sequence, seq_features_df in features.groupby("sequence_id"):
         cterom = ",".join(
                         list(
                             seq_features_df[seq_features_df.feature_id.isin(["Gly1","Gly2","Gly3"]) ].sort_values("feature_start").feature_id
                             )
                 )
@@ -295,17 +276,18 @@
                 "sequence_accession":sequence,
                 "sequence_src": "".join(set(seq_features_df.sequence_src.unique())),
                 "flag":search.decision_tree(nter_type,cterom),
                 "nter":nter_type,
                 "nter_neighbor": nter_neighbor,
                 "cter":cterom,
                 "sequence":str(calseq.get_seq_by_id(sequence).seq),
-                "iteration":seq_per_iteration[sequence]
+                # "iteration":seq_per_iteration[sequence]
             }
         )
     if summary_datas:
         df = pd.DataFrame(summary_datas).set_index("sequence_accession")
     else:
         df = pd.DataFrame(columns=["sequence_accession","sequence_src","flag","nter","nter_neighbor","cter","sequence","iteration"]).set_index("sequence_accession")
     df.to_csv(res_dir + "/pcalf.summary.tsv",sep="\t",index=True,header=True)
+
 if __name__ == "__main__":
     sys.exit(main())
```

### Comparing `pcalf-0.0.3/setup.py` & `pcalf-1.1.0/setup.py`

 * *Files 19% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 from setuptools import setup, find_packages
 
 with open("README.md", "r", encoding = "utf-8") as fh:
     long_description = fh.read()
 
 setup(
     name='pcalf',
-    version='0.0.3',
+    version='1.1.0',
     description='Search calcyanin in a set of amino acid sequences',
     long_description = long_description,
     long_description_content_type = "text/markdown",
     url='https://github.com/K2SOHIGH/pcalf',
     author='Maxime Millet',
     author_email='maxime.luc.millet@gmail.com',
     license='MIT',
@@ -24,15 +24,17 @@
          "pyhmmer==0.7.1",
          "biopython==1.81",
          "numpy>=1.21",
          "pyyaml>=6",
          "snakemake==7.22",
          "pandas==1.5.3",
          "tqdm==4.64.1",
-    ],    
+         "plotly==5.11.0",
+         "python-igraph==0.10.4",
+    ],
     python_requires = ">=3.9",
     packages = find_packages(where="src"),
     package_dir = {"": "src"},
     include_package_data=True,
     scripts = [script for script in glob.glob("scripts/*") if not os.path.basename(script).startswith("_") ],
     py_modules = ["bin"],
     zip_safe=False
```

### Comparing `pcalf-0.0.3/src/pcalf/core/biohmm.py` & `pcalf-1.1.0/src/pcalf/core/biohmm.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,26 +1,28 @@
 import os
 import tqdm
 import pyhmmer
+import logging
 
+#logger = logging.getLogger()
 
 class HmmIO:
     """Class to handle IO operation for Hmm object"""
     
     def load_msa(self,msafile:str,msa_name:str,alphabet=pyhmmer.easel.Alphabet.amino(),format=None):
         """Load a fasta file as pyhmmmer.easel.MSA object.
 
         Args:
             msafile (str): Path to fasta file
             msa_name (str): Name of your MSA
             alphabet (pyhmmer.easel.Alphabet): Kind of alphabet to use
             format (str): pyhmmer.easel.MSAFile format, default is None for auto detection. \
                 See pyhmmer.easel.MSAFile documentation for a complete list of format.
 
-        Returns:
+        Returns: 
         pyhmmmer.easel.MSA
 
         Raises:
         ValueError: When format is not a valid MSA format.
         FileNotFound: If msafile doesn't exist.
         """
         if os.path.exists(msafile):
@@ -45,15 +47,15 @@
         """Initializes the instance.
 
         Args:
             msa_name (str): Name of the msa/hmm object - required
             msafile (str): Path to the alignment file - optional
         """
         self._msa = self.load_msa(msafile,msa_name) if msafile else None        
-        self._hmm = self.hmmbuild(self.msa, **kwargs) if msafile else None #self.load_hmm(hmmfile,**kwargs)
+        self._hmm = self.hmmbuild(self.msa, **kwargs) if msafile else None
     
     @property
     def msa(self):
         return self._msa
 
     @property
     def hmm(self):
@@ -69,55 +71,142 @@
     @hmm.setter
     def hmm(self, value):        
         if isinstance(value,pyhmmer.plan7.HMM):                 
             self._hmm = value
         else:
             raise TypeError("value must be pyhmmer.plan7.HMM")        
 
+    def _align(self,
+                sequences:list,
+                hmm:pyhmmer.plan7.HMM,
+                trim:bool=True,
+                alphabet:pyhmmer.easel.Alphabet=pyhmmer.easel.Alphabet.amino()):
+        """Helper function to align sequences against temporary hmm 
+
+        Args:
+            sequences (list): List of  pyhmmer.easel.DigitalSequences - required.
+            hmm (pyhmmer.plan7.HMM): Hmm profile.
+            trim (bool): N-ter/C-ter trimming, see pyhmmer.hmmalign documentation for details
+            alphabet: Kind of alphabet to use.  
+        
+        Raises:
+            TypeError: If one sequence is not an instance of pyhmmer.easel.DigitalSequence.
+
+        Return:
+            Tuple of pyhmmer.easel.MSA and pyhmmer.plan7.HMM
+        """
+        for seq in sequences:
+            if not isinstance(seq,pyhmmer.easel.DigitalSequence):
+                raise TypeError("TypeError, get {} while pyhmmer.easel.DigitalSequence was expected".format(
+                    type(seq)
+                ))
+        msa = pyhmmer.hmmalign(hmm, 
+                               sequences, 
+                               digitize=True,
+                               trim=trim)     
+        msa.name = hmm.name
+        hmm = self.hmmbuild( msa )
+        return msa,hmm
 
-    def hmmalign(self,sequences:list,self_include=True,trim=True,alphabet=pyhmmer.easel.Alphabet.amino()):
+    def _count_kmers(self,sequence, k_size=5):
+        data = {}
+        kmers = []
+        size = len(sequence)
+        for i in range(size - k_size + 1):
+            kmer = sequence[i: i + k_size]
+            kmers.append(kmer)
+            if kmer not in data:
+                data[kmer] = 1
+                continue        
+            data[kmer] += 1 
+
+        return data , kmers 
+
+    def _jaccard_similarity(self, a, b):
+        a = set(a)
+        b = set(b)
+        intersection = len(a.intersection(b))
+        union = len(a.union(b))
+        return intersection / union
+
+
+    def hmmalign(self,sequences:list,
+                 self_include=True,
+                 iterative = False,
+                 trim=True,
+                 alphabet=pyhmmer.easel.Alphabet.amino()):
         """Align sequences to the hmm 
 
         Args:
           sequence (list): List of pyhmmer.easel.DigitalSequence - required
           self_include (bool): If set, sequences already present within the hmm will be added to the new hmm produced
           trim (bool): N-ter/C-ter trimming, see pyhmmer.hmmalign documentation for details
           alphabet (pyhmmer.easel.Alphabet): Kind of alphabet to use.
 
         Raises:
             TypeError: If one sequence is not an instance of pyhmmer.easel.DigitalSequence.
 
         Return:
             Hmm -> A new Hmm object including the hmm profile and the multiple sequence alignment.
-        """
-        if self_include:
-            sequences += self.msa.sequences
+        """    
 
+        accs = {} # keep sequence name in a list 
         for seq in sequences:            
-            if not isinstance(seq,pyhmmer.easel.DigitalSequence): 
-                raise TypeError("TypeError, get {} while pyhmmer.easel.DigitalSequence was expected".format(
-                    type(seq)
-                ))
+            if isinstance(seq,pyhmmer.easel.DigitalSequence): 
+                accs[seq.name] = seq.textize().sequence
+                continue
+            raise TypeError("TypeError, get {} while pyhmmer.easel.DigitalSequence was expected".format(
+                type(seq)
+            ))            
+                
+        if self_include: # Current MSA is kept.
+            for seq in self.msa.sequences:
+                if seq.name not in accs:
+                    sequences.append(seq)
+                else: # Duplicates      
+                    k_size = 5              
+                    _ , kmer_A = self._count_kmers(seq.textize().sequence,k_size= k_size)
+                    _ , kmer_B = self._count_kmers(accs[seq.name],k_size= k_size)
+                    jaccard = self._jaccard_similarity(kmer_A,kmer_B)
+                    logging.warning("""Duplicate identifier : {}\nHMM seqlength: {};\nNEW seqlength: {};\n Jaccard similarity: {} [kmer length: {}]""".format(
+                        seq.name,
+                        len(accs[seq.name]),
+                        len(seq.textize().sequence),
+                        jaccard,
+                        k_size
+                    ))
         
-        msa = pyhmmer.hmmalign( self.hmm, sequences, digitize=True , trim=trim )         
-        if not msa.name:
-            msa.name=self.hmm.name 
+        hmm = self.hmm
+        msa = self.msa
+        no_seqs = len(sequences)
+        logging.debug("Current No nodes within hmm : {} ".format(hmm.nseq) )
+        logging.debug("# Sequences to align : {} ".format(no_seqs) )
+        query = []
+        while sequences:        
+            if not iterative:
+                query = [sequences.pop() for _ in range(no_seqs)]
+            else:                
+                query.append(sequences.pop())
+                                     
+            msa, hmm = self._align(
+                        query,
+                        hmm,
+                        trim=trim,
+                        alphabet=alphabet)
             
-        hmm = self.hmmbuild(msa)
-        
-        assert isinstance(hmm,pyhmmer.plan7.HMM)
-        assert isinstance(msa,pyhmmer.easel.MSA)
+            assert isinstance(hmm,pyhmmer.plan7.HMM)
+            assert isinstance(msa,pyhmmer.easel.MSA)
         
         new_hmm = Hmm(hmm.name)
         new_hmm.hmm = hmm
-        new_hmm.msa = msa
-
+        new_hmm.msa = msa     
+        logging.debug("No of sequence in updated hmm/msa : {}/{}".format(
+            hmm.nseq,len(msa.sequences)))
         return new_hmm
-
-    
+        
 
     def hmmbuild(self,
                 msa,
                 alphabet=pyhmmer.easel.Alphabet.amino(),
                 matrix = "BLOSUM90",
                 **kwargs):    
         """Build HMM from MSA 
@@ -132,93 +221,11 @@
             None
 
         Return:
             pyhmmer.plan7.HMM object
         """
 
         builder = pyhmmer.plan7.Builder(alphabet,**kwargs)
-        builder.score_matrix = "BLOSUM90"
+        builder.score_matrix = matrix
         background = pyhmmer.plan7.Background(alphabet)        
         hmm, _ , __ = builder.build_msa(msa, background)
         return hmm
-
-    def _align(self,
-                sequences:list,
-                hmm:pyhmmer.plan7.HMM,
-                trim:bool=True,
-                alphabet:pyhmmer.easel.Alphabet=pyhmmer.easel.Alphabet.amino()):
-        """Helper function to align sequences against temporary hmm 
-
-        Args:
-            sequences (list): List of  pyhmmer.easel.DigitalSequences - required.
-            hmm (pyhmmer.plan7.HMM): Hmm profile.
-            trim (bool): N-ter/C-ter trimming, see pyhmmer.hmmalign documentation for details
-            alphabet: Kind of alphabet to use.  
-        
-        Raises:
-            TypeError: If one sequence is not an instance of pyhmmer.easel.DigitalSequence.
-
-        Return:
-            Tuple of pyhmmer.easel.MSA and pyhmmer.plan7.HMM
-        """
-        for seq in sequences:
-            if not isinstance(seq,pyhmmer.easel.DigitalSequence):
-                raise TypeError("TypeError, get {} while pyhmmer.easel.DigitalSequence was expected".format(
-                    type(seq)
-                ))
-        msa = pyhmmer.hmmalign(hmm, sequences , digitize=True ,trim=trim)     
-        msa.name = hmm.name
-        hmm = self.hmmbuild( msa )
-        return msa,hmm
-
-    def iterative_align(self,
-                sequences:list,
-                self_include=True,
-                trim=True,
-                alphabet=pyhmmer.easel.Alphabet.amino()):                        
-
-        """Align sequence to HMM iteratively
-
-        Args:
-            sequences (list): List of pyhmmer.easel.DigitalSequences - required.
-            self_include (bool): If set, sequences already present within the hmm will be added to the new hmm produced
-            trim (bool): N-ter/C-ter trimming, see pyhmmer.hmmalign documentation for details
-            alphabet (pyhmmer.easel.Alphabet): Kind of alphabet to use.  
-        
-        Raises:
-            TypeError: If one sequence is not an instance of pyhmmer.easel.DigitalSequence.
-
-        Return:
-            Tuple of pyhmmer.easel.MSA and pyhmmer.plan7.HMM
-        """
-
-                
-        
-        hmm = self.hmm
-        msa = None
-        if self_include:
-            msa = self.msa
-        #seq_iterator = iter(sequences)
-        #while (seq := next(seq_iterator, None)) is not None:                                                
-        for seq in tqdm.tqdm(sequences,colour="yellow"):
-            if not isinstance(seq,pyhmmer.easel.DigitalSequence):
-                raise TypeError("Wrong type - {} , expected pyhmmer.easel.DigitalSequence".format(type(seq)))            
-            
-            lseq = [seq] 
-            if msa:
-                lseq += msa.sequences
-            
-            
-            msa, hmm = self._align(
-                        lseq,
-                        hmm,
-                        trim=trim,
-                        alphabet=alphabet)
-                        
-        assert isinstance(hmm,pyhmmer.plan7.HMM)
-        assert isinstance(msa,pyhmmer.easel.MSA)
-        
-        new_hmm = Hmm(hmm.name)
-        new_hmm.hmm = hmm
-        new_hmm.msa = msa
-
-        return new_hmm
```

### Comparing `pcalf-0.0.3/src/pcalf/core/bioseq.py` & `pcalf-1.1.0/src/pcalf/core/bioseq.py`

 * *Files 3% similar despite different names*

```diff
@@ -62,16 +62,18 @@
                 fhl = self._openfile(fasta)
         else:
             fhl = fasta
         
         assert isinstance(fhl,io.TextIOWrapper)
 
         sequences = []
+        #'ACDEFGHIKLMNPQRSTVWY-BJZOUX*~'
         for record in SeqIO.parse(fhl,format="fasta"):
             if len(record.seq) < 10000:
+                record.seq = record.seq.strip()
                 sequences.append(Seq(record,src=src))
             else:                
                 logging.warning("Sequence {} seems very long and can't be scan through hmmer".format(record.id))
         return sequences
 
     def to_fasta(self , filehandle ):
         """Dump fasta records.
@@ -116,15 +118,15 @@
         src:str="",
         ):
         
         self.hid = hid
         self.target_len=target_len
         self.start_location = start_location
         self.stop_location = stop_location
-        self.score = float('{:0.3e}'.format(score).strip("'")) if score else score #'{:0.3e}'.format(score) if score else score
+        self.score = float('{:0.3e}'.format(score).strip("'")) if score else score
         self.identity= round(identity,3) if identity else identity
         self.coverage = round(coverage,2) if coverage else coverage
         self.method = method
         self.src = src
 
 
 class Seq(SeqRecord):  
@@ -195,17 +197,16 @@
         fseq = []
         for f in self.features:
             keep = True            
             if feature_id:                
                 keep = feature_id == f.id
             if keep:
                 fseq.append(
-                    Seq(SeqRecord(seq=f.extract(self.seq),id=self.id,description=f.id, features = [f] )    )
+                    Seq(SeqRecord(seq=f.extract(self.seq),id=self.id, description="", features = [f] )    )
                 )
-
         return fseq
         
     def per_residue_annotation(self):
         """Put annotation hits under the residues (self.res) they cover [sorted by score].
         
         Args:
             None
@@ -220,33 +221,15 @@
         self.hits.sort(key=lambda x: x.score, reverse=False)
 
         for hit in self.hits:
             for aa in range(hit.start_location,hit.stop_location):
                 if not self.res[aa]:
                     self.res[aa] = []#                
                 self.res[aa].append(hit)
-                #self.res[aa].evalue.append(hit.score)   
-    
-    # def _keep_best_annotation(self):
-    #     """helper function to keep only the best hit
-        
-    #     Args:
-    #         None
-    #     Raises:
-    #         None
-    #     Return:
-    #         None
-    #     """
-    #     b = []
-    #     for _ , residue in self.res.items():
-    #         if residue:
-    #             b.append(residue.keep_best())
-    #         else:
-    #             b.append("-")
-    #     return b 
+
 
     def addhit(self,hit):
         """Add Hit object to Seq.
         
         Args:
             hit (Hit): Hit object.
         Raises:
@@ -360,15 +343,15 @@
             Sequences object -> a new Sequences object containing sequence (Seq) with at least one hit against one or more profiles.
         """                    
         assert isinstance(hmms,list)
         for hmm in hmms:            
             if not isinstance(hmm, pyhmmer.plan7.HMM):
                 raise TypeError("Except pyhmmer.plan7.HMM but received".format(type(hmm)))
 
-        hits = pyhmmer.hmmsearch(hmms,self.digitize(alphabet),cpus=cpus)
+        hits = pyhmmer.hmmsearch(hmms,self.digitize(alphabet),cpus=cpus,**kwargs)
         hmm_datas = [(h.name.decode("UTF-8"),h.M)  for h in hmms]
         seq_with_hit = []
         for hmm_datas , hit_by_hmm in zip(hmm_datas,hits):
             hmm_id,hmm_len=hmm_datas
             for hit in hit_by_hmm:
                 sequence_identifier = hit.name.decode("UTF-8")
                 if sequence_identifier not in seq_with_hit:
@@ -386,18 +369,16 @@
                             coverage=(dom.alignment.target_to-dom.alignment.target_from)/hmm_len,#len(seq.seq),
                             src = hmm_id,
                             identity = round(
                                 self.hamming_distance(dom.alignment.target_sequence.lower(),dom.alignment.hmm_sequence.lower()),2)                            
                         )
                     seq.addhit(dh)
 
+        return self
 
-        sequences_with_hit = Sequences()
-        sequences_with_hit.sequences = [self.get_seq_by_id(sid) for sid in seq_with_hit]
-        return sequences_with_hit
 
 
     def blastp(self,blast_subject_fasta,evalue=1e-4,outfmt="10 std slen"):   
         """Perform a sequence vs sequence blastp search and append \ 
         resulting hits to the hits attribute of their respective sequence.
         
         Args:
@@ -424,15 +405,15 @@
                     "-subject", blast_subject_fasta,
                     "-evalue" , str(evalue),
                     "-outfmt" , '"10 std slen"'                    
                 ]
 
         o = subprocess.run(" ".join(command) , capture_output=True , shell=True)         
         res = o.stdout.decode('ascii').strip()
-
+        sequences = Sequences() # create a new sequence object that will store sequences with at least one hit
         if res:
             df = pd.read_table( StringIO(res)  , sep=","  , header=None )          
             df.columns = "qacc sacc pident length mismatch gapopen qstart qend sstart send evalue bitscore slen".split(" ")
             df.sort_values("pident",inplace=True,ascending=False)    
             df.set_index("qacc",inplace=True)
             df["coverage"] = df.apply(lambda x: (x.send-x.sstart) / x.slen * 100, axis=1 )
             for _ , blastp_hit in df.iterrows():
@@ -444,16 +425,15 @@
                         score = blastp_hit.evalue,
                         method="blastp",
                         coverage=(blastp_hit.send-blastp_hit.sstart)/blastp_hit.slen ,
                         src = blastp_hit.sacc,
                         identity = blastp_hit.pident
                     )
                 self.get_seq_by_id(_).addhit(dh)
-            return df
-        return None
+        return self        
 
     def to_feature_table(self,add_sequence=True,feature_id=""):
         """Generate a feature table.
         
         Args:
             add_sequence (bool): If set, the feature sequence (str) will be append to the table.
             feature_id (str): If set, only feature with the same identifier will be considered.            
@@ -474,26 +454,27 @@
                         seq.id,
                         seq.src,
                         feature.type,
                         feature.location.start,
                         feature.location.end,
                         feature.id,
                         feature.qualifiers["identity"],
+                        feature.qualifiers["coverage"],
                         feature.qualifiers["score"],
                         feature.qualifiers["src"],
                         feature.qualifiers["src_len"]
                     ]
                     if add_sequence:                    
                         f.append(
                             str(feature.extract(seq.seq))
                         )
                     features.append(f)
         return pd.DataFrame(features,columns=[
             "sequence_id","sequence_src","feature_type","feature_start","feature_end",
-            "feature_id","pident","e-value","feature_src","feature_target_len","feature_seq"
+            "feature_id","pident","coverage","e-value","feature_src","feature_target_len","feature_seq"
         ]).set_index("sequence_id")
 
     def to_hits_table(self):
         """Generate a hits table.
         
         Args:
             self
```

### Comparing `pcalf-0.0.3/src/pcalf/core/log.py` & `pcalf-1.1.0/src/pcalf/workflow/datasets/scripts/log.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,61 +1,53 @@
 import os
 import logging
-import inspect 
 
-
-class CustomFormatter(logging.Formatter):
+class CustomFormatter(logging.Formatter):    
     grey = "\x1b[38;20m"
     yellow = "\x1b[33;20m"
     red = "\x1b[31;20m"
     bold_red = "\x1b[31;1m"
     reset = "\x1b[0m"
-    black = "\u001b[30m"
+    black = "\u001b[30m"    
     green = "\u001b[32m"
     blue = "\u001b[34m"
     magenta = "\u001b[35m"
     cyan = "\u001b[36m"
     white = "\u001b[37m"
-    lightpurple = "\x1b[38;5;69m" #[38;5;141m" #"\x1b[38;5;84m"
-    pink90 = "\x1b[38;5;162m" #"\x1b[38;5;214m"
-    
-    format = "PCALF | %(message)s"
-    
+
+
+    format = "%(asctime)s - %(name)s - %(levelname)s - %(message)s (%(filename)s:%(lineno)d)"
+
     FORMATS = {
         logging.DEBUG: reset + format + reset,
-        logging.INFO: lightpurple + format + reset,
-        logging.WARNING: pink90 + format + reset,
-        logging.ERROR: bold_red + format + reset,
+        logging.INFO: magenta + format + reset,
+        logging.WARNING: cyan + format + reset,
+        logging.ERROR: red + format + reset,
         logging.CRITICAL: bold_red + format + reset
     }
 
     def format(self, record):
-        log_fmt = self.FORMATS.get(record.levelno)                
+        log_fmt = self.FORMATS.get(record.levelno)
         formatter = logging.Formatter(log_fmt)
         return formatter.format(record)
 
 
 
-# def setlogger(name="__main__",level="INFO"):
-#     logger = logging.Logger(name)    
-#     logger.setLevel(level)
-#     logger.addHandler(
-#         stream_handler(level)
-#     )
-
-#     return logger
-
-# def file_handler(logfile,level):
-#     dirname = os.path.abspath(
-#         os.path.dirname(logfile)
-#     )
-#     os.makedirs(dirname,exist_ok=True)
-#     handler = logging.FileHandler( logfile , mode = 'a' )
-#     handler.setFormatter( CustomFormatter() )
-#     handler.setLevel(level)
-#     return handler
-
-# def stream_handler(level):
-#     handler = logging.StreamHandler( )
-#     handler.setFormatter( CustomFormatter() )
-#     handler.setLevel(level)
-#     return handler
+def setlogger(name="__main__"):    
+    logger = logging.Logger(name)          
+    return logger 
+
+def file_handler(logfile,level):    
+    dirname = os.path.abspath(
+        os.path.dirname(logfile)
+    )
+    os.makedirs(dirname,exist_ok=True)
+    handler = logging.FileHandler( logfile , mode = 'a' )    
+    handler.setFormatter( CustomFormatter() )    
+    handler.setLevel(level)
+    return handler
+    
+def stream_handler(level):    
+    handler = logging.StreamHandler( )    
+    handler.setFormatter( CustomFormatter() )    
+    handler.setLevel(level)
+    return handler
```

### Comparing `pcalf-0.0.3/src/pcalf/core/search.py` & `pcalf-1.1.0/src/pcalf/core/_bkpsearch.py`

 * *Files 6% similar despite different names*

```diff
@@ -16,37 +16,33 @@
 
 # from utils import log
 from .biohmm import Hmm
 from .bioseq  import Sequences , Hit
 
 from Bio.SeqRecord import SeqRecord
 
-logging.basicConfig(
-    format="%(asctime)s [%(threadName)-12.12s] [%(levelname)-5.5s]  %(message)s",
-    level=logging.INFO,
-    handlers=[]
-)
-
-def _search_calcyanin(fasta:str, 
-                    src:str,
-                    glyx3_hmm:pyhmmer.plan7.HMM, 
-                    gly1_hmm:pyhmmer.plan7.HMM, 
-                    gly2_hmm:pyhmmer.plan7.HMM, 
-                    gly3_hmm:pyhmmer.plan7.HMM,
-                    nter_fa:str, 
-                    domz:int=10000,
-                    glyx3_evalue_threshold:float=1e-30,
-                    glyx3_coverage_threshold:float=0.5,
-                    glyzip_evalue_threshold:float=3.6e-4,
-                    glyzip_coverage_threshold:float=0.7,
-                    nter_coverage_threshold:float = 0.80, 
-                    nter_evalue_threshold:float = 1e-07,
-                    tmp_dir = None,
-                    ):
-    """Find calcyanin within a fasta file using several HMM profiles and 'database' of known N-ter.
+def search_calcyanin(fasta:str, 
+            src:str,
+            glyx3_hmm:pyhmmer.plan7.HMM, 
+            gly1_hmm:pyhmmer.plan7.HMM, 
+            gly2_hmm:pyhmmer.plan7.HMM, 
+            gly3_hmm:pyhmmer.plan7.HMM,
+            nter_fa:str, 
+            Z:int=10000,
+            domZ:int=10000,
+            glyx3_evalue_threshold:float=1e-30,
+            glyx3_coverage_threshold:float=0.5,
+            glyzip_evalue_threshold:float=1e-5,
+            glyzip_coverage_threshold:float=0.7,
+            nter_coverage_threshold:float = 0.80, 
+            nter_evalue_threshold:float = 1e-07,
+            tmp_dir = None,
+            ):
+    """Find calcyanin within a fasta file using several HMM 
+    profiles and 'database' of known N-ter.
     
     Args:
         fasta (str): Path to a fasta file - required.
         src (str): will be attached to calcyanin. Useful when searching across multiple files.  
         glyx3_hmm (pyhmmer.plan7.HMM):  Glyx3 HMM profile - required
         gly1_hmm (pyhmmer.plan7.HMM): Gly1 HMM profile - required
         gly2_hmm (pyhmmer.plan7.HMM): Gly2 HMM profile - required
@@ -69,33 +65,33 @@
     if tmp_dir:
         tmp_dir = os.path.join(tmp_dir, src )
         os.makedirs(tmp_dir, exist_ok=True)
 
     # Setup sequences - Parse fasta into Sequences object 
     sequences = Sequences(fasta,src=src)
     
-        
-    # Search sequences against GlyX3 profile
-    glyx3_sequences = sequences.hmmsearch([glyx3_hmm])
+    # 1) Search sequences against GlyX3 profile
+    logging.debug("1) Search {} against GlyX3".format(fasta))
+    glyx3_sequences = sequences.hmmsearch([glyx3_hmm],Z=Z, domZ=domZ )
     glyx3_sequences.to_hits_table().to_csv(os.path.join(tmp_dir,"glyx3.hits.tsv"),sep="\t",header=True,index=True)
+    
     for seq in glyx3_sequences.sequences:
         # We filter hits based on their e-value and the total coverage against the GlyX3 HMM profile.
-
         hit_below_evalue_threshold = [ h for h in seq.hits if h.score < glyx3_evalue_threshold]     
         if hit_below_evalue_threshold:          
             start_glyx3 = min([h.start_location for h in hit_below_evalue_threshold])
             end_glyx3 = max([h.stop_location for h in hit_below_evalue_threshold])
+
             scores = [h.score for h in hit_below_evalue_threshold]
             hmm_profile_len = [h.target_len for h in hit_below_evalue_threshold][0]
             coverage_on_glyx3 = (end_glyx3-start_glyx3)/hmm_profile_len #glyx3_easel_hmm[0].M
             mean_identity = sum([h.identity for h in hit_below_evalue_threshold])/len(hit_below_evalue_threshold)
 
             # COVERAGE THESHOLD 
             if coverage_on_glyx3 > glyx3_coverage_threshold:
-
                 f = SeqFeature(
                     FeatureLocation(
                         start_glyx3, 
                         end_glyx3
                         ),
                     id="GlyX3",
                     type="domain", 
@@ -110,30 +106,37 @@
                 seq.hits=[]
                 seq.features.append( f )
 
     # we free some memory.
     del sequences 
     # keep only sequence with a hit against the glyx3 profile with a E-value below and a coverage above E-value and coverage thresholds respectively.
     glyx3_sequences.sequences = [s for s in glyx3_sequences.sequences if s.features] 
-    # We can then use those sequences for the next steps aka Glycine zipper annotation and N-ter comparison.
-    
-    # Search GlyZip profiles
+    # We can then use those sequences for the next steps 
+    # i.e, Glycine zipper annotation and N-ter comparison.
+
+    # 2) Search GlyZip profiles
+    logging.debug("2) Search {} sequences against Glyzip HMM profiles".format(len(glyx3_sequences.sequences)))
     glzips_easel_hmm = [gly1_hmm,gly2_hmm,gly3_hmm]
-    glyx3_sequences = glyx3_sequences.hmmsearch(glzips_easel_hmm)
+    glyx3_sequences = glyx3_sequences.hmmsearch(glzips_easel_hmm ) #,Z=Z ,domZ=domZ )
     glyx3_sequences.to_hits_table().to_csv(os.path.join(tmp_dir,"glyzips.hits.tsv"),sep="\t",header=True,index=True)
+    
     for seq in glyx3_sequences.sequences:
         # Hit filtering and features creation.
         seq.per_residue_annotation()
         current = Hit()
         features = []
         features_len = []
         fraglen = 0
+        
         for res,hit in seq.res.items():   
             if hit:
-                # E-VALUE THRESHOLD
+                # E-VALUE THRESHOLD   
+                if seq.id == "lcl|JAJTDD010000010.1_cds_MCE2661253.1_93":
+                    logging.debug("- {}  {}  {}".format(
+                        hit[0].hid , hit[0].score, glyzip_evalue_threshold))
                 if hit[0].score < glyzip_evalue_threshold:        
                     if current.hid == hit[0].hid:
                         fraglen += 1
                         continue    
                     else:
                         if current.hid:                            
                             features.append(current)
@@ -145,15 +148,15 @@
                 if current.hid:
                     features.append(current)
                     features_len.append(fraglen)
                 current = Hit()
                 fraglen=0
         
         # COVERAGE THRESHOLD 
-        feat = [ f for f,fl in zip(features,features_len)  if fl/f.target_len > glyzip_coverage_threshold ]
+        feat = [ f for f,fl in zip(features,features_len)  if fl/f.target_len > glyzip_coverage_threshold and f.score < glyzip_evalue_threshold ]
         # We can then remove all hits that do not respect the coverage threshold.
         seq.hits = feat
         # For each hit we create a feature 
         for valid_glyzip_hit in seq.hits:
             f = SeqFeature(
                 FeatureLocation(
                     valid_glyzip_hit.start_location, 
@@ -164,70 +167,92 @@
                 qualifiers={
                     "n_hits":1,
                     "score":valid_glyzip_hit.score,
                     "src":"{}_HMM_Profile".format(valid_glyzip_hit.hid),
                     "src_len":valid_glyzip_hit.target_len,
                     "identity":valid_glyzip_hit.identity
                 })
+            if seq.id == "lcl|JAJTDD010000010.1_cds_MCE2661253.1_93":
+                logging.debug("- {}".format(f.__dict__))
+                        
 
             seq.features.append( f )
         # Again, we clean the hits attributes for the next step.
         seq.hits = []
 
-    # Search N-ter
+    # 3) Compare sequence with known N-ter.
+    logging.debug("3) blast {} sequences against known N-ters".format(len(glyx3_sequences.sequences)))
     blastp_raw_results = glyx3_sequences.blastp(nter_fa)
     if  blastp_raw_results is not None:
         if not blastp_raw_results.empty:
             glyx3_sequences.to_hits_table().to_csv(os.path.join(tmp_dir,"nter.hits.tsv"),sep="\t",header=True,index=True)
 
+    
     for seq in glyx3_sequences.sequences:
-        for valid_nter_hit in seq.hits:
+        self_match = None
+        valid_match = []
+        for nter_hit in seq.hits:
             # E-value and coverage filtering.
-            if valid_nter_hit.score < nter_evalue_threshold and \
-                valid_nter_hit.coverage >= nter_coverage_threshold and \
-                valid_nter_hit.hid.split("||")[-1] != seq.id:
+            if nter_hit.score < nter_evalue_threshold and \
+                nter_hit.coverage >= nter_coverage_threshold:
+                if seq.id == "Cyanothece_sp_PCC_7425":
+                    print(seq.id, nter_hit.hid)
+                    print(nter_hit.score , nter_evalue_threshold )
+                    print(nter_hit.coverage, nter_coverage_threshold)
+
                 f = SeqFeature(
                     FeatureLocation(
-                        valid_nter_hit.start_location, 
-                        valid_nter_hit.stop_location
+                        nter_hit.start_location, 
+                        nter_hit.stop_location
                         ),
                     id="N-ter",
                     type="domain", 
                     qualifiers={
                         "n_hits":len(seq.hits),
-                        "score":valid_nter_hit.score,
-                        "src":valid_nter_hit.hid,
-                        "src_len":valid_nter_hit.target_len,
-                        "identity":valid_nter_hit.identity
-                    })                
-                seq.features.append( f )
-
+                        "score":nter_hit.score,
+                        "src":nter_hit.hid,
+                        "src_len":nter_hit.target_len,
+                        "identity":nter_hit.identity
+                    })     
+                if nter_hit.hid.split("||")[-1] == seq.id:
+                    self_match = f
+                else:
+                    valid_match.append(f)
+                #seq.features.append( f )
                 # we break the loop because we keep only the best hit - aka the nearest neighboor.
-                break
+                # break
+        if valid_match:
+            seq.features.append(valid_match[0]) # because we keep only the best hit - aka the nearest neighboor.
+        elif self_match:
+            seq.features.append(self_match) # because there is no nearest neighboor but a self match exist.
+        else:
+            pass # because there is not hit at all.
+
         seq.hits = []
     # we return the calcyanin as a Sequences object with all their features.
     return glyx3_sequences
 
 def _search_calcyanin_mt(args):    
     """helper function to run search_calcyanin() from concurrent futures."""    
     # mem = (psutil.Process().memory_info().rss / (1024 * 1024))/1000
     # logging.debug("memory usage : {}".format(mem))
-    return _search_calcyanin(*args)
+    return search_calcyanin(*args) # return a Sequences object # bioseq.py
 
 def _search_calcyanin_concurrent(fastas:list,  
                     srcs:list,                                
                     glyx3_hmm:Hmm, 
                     gly1_hmm:Hmm, 
                     gly2_hmm:Hmm, 
                     gly3_hmm:Hmm,
                     nter_fa:str, 
-                    domz:int=10000,
+                    Z:int=10000,
+                    domZ:int=10000,
                     glyx3_evalue_threshold:float=1e-30,
                     glyx3_coverage_threshold:float=0.5,
-                    glyzip_evalue_threshold:float=3.6e-4,
+                    glyzip_evalue_threshold:float=1e-5,
                     glyzip_coverage_threshold:float=0.7,
                     nter_coverage_threshold:float = 0.80, 
                     nter_evalue_threshold:float = 1e-07,
                     tmp_dir = None):
     """Wrapper to run multiple file at once with the function _search_calcyanin.
     
     Args:
@@ -262,33 +287,35 @@
             (fasta_file,
             src,
             glyx3_hmm.hmm,
             gly1_hmm.hmm,
             gly2_hmm.hmm,
             gly3_hmm.hmm,
             nter_fa,
-            domz,
+            Z,
+            domZ,
             glyx3_evalue_threshold,
             glyx3_coverage_threshold,
             glyzip_evalue_threshold,
             glyzip_coverage_threshold,
             nter_coverage_threshold, 
             nter_evalue_threshold,
             tmp_dir
             )
         )
     
     with concurrent.futures.ThreadPoolExecutor(max_workers=multiprocessing.cpu_count()-1) as executor:
         
-        l+=list(tqdm.tqdm(executor.map(_search_calcyanin_mt, pools), total=len(pools) , colour="yellow") )
-        
-    calcyanin_sequences = Sequences()
+        l+=list(tqdm.tqdm(executor.map(_search_calcyanin_mt, pools), total=len(pools) , colour="CYAN") )
+    
+    # concatenate Sequences objects
+    sequences = Sequences()
     for e in l:
-        calcyanin_sequences.sequences += e.sequences
-    return calcyanin_sequences
+        sequences.sequences += e.sequences
+    return sequences
 
 def __modifyline__(string,val):
     """Modify the weight of Glycine residue"""
     liste = string.split()
     if len(liste) >= 21:
         liste[6] = str(val*float(liste[6]))
     elif len(liste) == 20:
@@ -346,21 +373,24 @@
         hmm (Hmm): Hmm object.
     Raises:
         None
     Return:
         Updated Hmm object.
     """    
 
-    l_digital_seq = [ s.digitize() for s in l_seq ]
-    if is_update_iterative:
-        new_hmm = hmm.iterative_align(l_digital_seq)
-    else:        
-        new_hmm = hmm.hmmalign( l_digital_seq )
+    l_digital_seq = [ s.digitize() for s in l_seq]# if s.id not in sequences_in_msa]
     
-    new_hmm.hmm = increase_glycine_weight( new_hmm,0.2 )
+    logging.debug("Number of sequence provided to update_hmm() : {} ".format(
+        len(l_digital_seq)))
+    
+    new_hmm = hmm.hmmalign(l_digital_seq , iterative = is_update_iterative)
+    new_hmm.hmm = increase_glycine_weight( new_hmm , 0.2 )
+    logging.debug("length of updated hmm :  {} ".format(
+        new_hmm.hmm.nseq
+    ))
     return new_hmm
 
 def parse_nterdb(nterdb):   
     """parse the nterdb file to dictionnary"""
     nter_dict={} 
     with open(nterdb) as db:
         for line in db.readlines():
@@ -374,18 +404,19 @@
         fastas:list, 
         srcs:list,
         glyx3:Hmm, 
         gly1:Hmm, 
         gly2:Hmm, 
         gly3:Hmm,
         nterdb:str, 
-        domz:int=10000,
+        Z:int=10000,
+        domZ:int=10000,
         glyx3_evalue_threshold:float=1e-30,  
         glyx3_coverage_threshold:float=0.60,  
-        glyzip_evalue_threshold:float=3.6e-4,
+        glyzip_evalue_threshold:float=1e-5,
         glyzip_coverage_threshold:float=0.7,
         nter_coverage_threshold:float = 0.80, 
         nter_evalue_threshold:float = 1e-07,
         max_iteration:int=1,
         is_update_iterative:bool=False): 
     """Search for calcyanin within one or more fasta files using several HMM profiles and 'database' of known N-ter.
 
@@ -425,36 +456,38 @@
         tmp_dir = os.path.join(out,"tmp","iteration_{}".format(ite))
         logging.info("Dump Nter DB as fasta.")
         nterfa = tempfile.NamedTemporaryFile(mode="w+")
         for sid, nter in nterdb.items():
             nterfa.write(">{}||{}\n{}\n".format(nter[0],sid,nter[1]))
         nterfa.flush()
         # search calcyanin        
-        logging.info("[iteration {}] |  Search calcyanin".format(ite))
+        logging.info("[iteration {}] |  Iteratively search of calcyanin".format(ite))
+        
         calcyanin_sequences = _search_calcyanin_concurrent(fastas, 
                 srcs,
                 glyx3,
                 gly1,
                 gly2,
                 gly3,
                 nterfa.name,
-                domz,
+                Z,
+                domZ,
                 glyx3_evalue_threshold,
                 glyx3_coverage_threshold,
                 glyzip_evalue_threshold,
                 glyzip_coverage_threshold,
                 nter_coverage_threshold, 
                 nter_evalue_threshold,
                 tmp_dir
             )
+        
         not_converged=False       
         new_calc = 0
         new_seq = 0
         valid_calcyanin = Sequences() 
-        
         if calcyanin_sequences.sequences:            
             for seq in calcyanin_sequences.sequences:     
                 if seq.id not in seq_per_iteration:                                              
                     seq_per_iteration[seq.id] = ite
                     new_seq+=1                    
                     nter = ",".join([f.features[0].qualifiers["src"].split("|")[0] for f in  seq.get_feature("N-ter")])
                     cter = ",".join([f.features[0].id for f in seq.get_feature("Gly1" )+
@@ -474,15 +507,15 @@
             glyx3features = valid_calcyanin.get_feature("GlyX3")
             if glyx3features:  
                 logging.info("[iteration {}] |  Updating GlyX3".format(ite))
                 glyx3 = update_hmm(glyx3features,glyx3,is_update_iterative)
 
             
             gly1features = valid_calcyanin.get_feature("Gly1")        
-            if gly1features:
+            if gly1features:    
                 logging.info("[iteration {}] |  Updating Gly1".format(ite))
                 gly1 = update_hmm(gly1features,gly1,is_update_iterative)
   
             
             gly2features = valid_calcyanin.get_feature("Gly2")        
             if gly2features:
                 logging.info("[iteration {}] |  Updating Gly2".format(ite))
@@ -490,37 +523,37 @@
 
             
             gly3features = valid_calcyanin.get_feature("Gly3")        
             if gly3features:
                 logging.info("[iteration {}] |  Updating Gly3".format(ite))
                 gly3 = update_hmm(gly1features,gly3,is_update_iterative)
 
-            
-            
             nterfeatures = valid_calcyanin.get_feature("N-ter")
             if nterfeatures:                
                 logging.info("[iteration {}] |  Updating N-ter".format(ite))
-                for nf in tqdm.tqdm(nterfeatures,colour="yellow"):
+                for nf in nterfeatures:
                     ntype,src = nf.features[0].qualifiers["src"].split("||")
                     idt = nf.features[0].qualifiers["identity"]                    
                     if idt<100:                        
                         nterdb.update(
                             {nf.id:( ntype , str(nf.seq) )}
                         )
                     else:
-                        logging.warning("Sequence already in DB ...")                     
+                        logging.warning("Already in DB ... {} has 100% identity with {} which is already in the N-ter DB.".format(                            
+                            nf.id,
+                            src,
+                        ))                     
             logging.info("Number of sequences in the N-ter database after update : {}".format(len(nterdb)))                    
             ite += 1
             if ite == max_iteration:
                 logging.warning("Max iteration reached.")
                 not_converged=False
         else:
             logging.info("[iteration {}] | No new calcyanin detected.".format(ite))
             logging.info("[iteration {}] | Stop.".format(ite))
-    
     return calcyanin_sequences, glyx3 , gly1, gly2, gly3 , nterdb , seq_per_iteration
 
             
 def decision_tree(nter , cter):
     """give a flag to a calcyanin based on its C-ter modular organization and its N-ter."""
     if re.search("Gly1,Gly2,Gly3",cter):
         if nter in ["CoBaHMA-type","Y-type","X-type","Z-type"]:
@@ -534,26 +567,14 @@
             flag = "Atypical Gly region with known N-ter"
         else:
             flag = "Atypical Gly region with new N-ter"
     else:
         flag="Ancestral gly containing protein"
     return flag
 
-def valid_calcyanin(sequences):
-    """Subset 
-    
-    Args:
-        l_seq (list): List of Seq object.
-        hmm (Hmm): Hmm object.
-    Raises:
-        None
-    Return:
-        Updated Hmm object.
-    """    
-
 
 def parse_nterdb(nterdb):   
     """parse the nterdb file to dictionnary"""
     nter_dict={} 
     with open(nterdb) as db:
         for line in db.readlines():
             nter, strain, seq = line.strip().split()
```

### Comparing `pcalf-0.0.3/src/pcalf/datas/Gly1.hmm` & `pcalf-1.1.0/src/pcalf/datas/Gly1.hmm`

 * *Files identical despite different names*

### Comparing `pcalf-0.0.3/src/pcalf/datas/Gly1.msa.fa` & `pcalf-1.1.0/src/pcalf/datas/Gly1.msa.fa`

 * *Files identical despite different names*

### Comparing `pcalf-0.0.3/src/pcalf/datas/Gly2.hmm` & `pcalf-1.1.0/src/pcalf/datas/Gly2.hmm`

 * *Files identical despite different names*

### Comparing `pcalf-0.0.3/src/pcalf/datas/Gly2.msa.fa` & `pcalf-1.1.0/src/pcalf/datas/Gly2.msa.fa`

 * *Files identical despite different names*

### Comparing `pcalf-0.0.3/src/pcalf/datas/Gly3.hmm` & `pcalf-1.1.0/src/pcalf/datas/Gly3.hmm`

 * *Files identical despite different names*

### Comparing `pcalf-0.0.3/src/pcalf/datas/Gly3.msa.fa` & `pcalf-1.1.0/src/pcalf/datas/Gly3.msa.fa`

 * *Files identical despite different names*

### Comparing `pcalf-0.0.3/src/pcalf/datas/GlyX3.hmm` & `pcalf-1.1.0/src/pcalf/datas/GlyX3.hmm`

 * *Files identical despite different names*

### Comparing `pcalf-0.0.3/src/pcalf/datas/GlyX3.msa.fa` & `pcalf-1.1.0/src/pcalf/datas/GlyX3.msa.fa`

 * *Files identical despite different names*

### Comparing `pcalf-0.0.3/src/pcalf/datas/all.hmm` & `pcalf-1.1.0/src/pcalf/datas/all.hmm`

 * *Files identical despite different names*

### Comparing `pcalf-0.0.3/src/pcalf/datas/nterdb.fasta` & `pcalf-1.1.0/src/pcalf/datas/nterdb.fasta`

 * *Files identical despite different names*

### Comparing `pcalf-0.0.3/src/pcalf/datas/nterdb.ref.tsv` & `pcalf-1.1.0/src/pcalf/datas/nterdb.ref.tsv`

 * *Files identical despite different names*

### Comparing `pcalf-0.0.3/src/pcalf/datas/nterdb.tsv` & `pcalf-1.1.0/src/pcalf/datas/nterdb.tsv`

 * *Files identical despite different names*

