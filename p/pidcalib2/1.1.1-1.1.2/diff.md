# Comparing `tmp/pidcalib2-1.1.1.tar.gz` & `tmp/pidcalib2-1.1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "/builds/lhcb-rta/pidcalib2/dist/.tmp-mevam7bq/pidcalib2-1.1.1.tar", last modified: Tue Apr 11 12:06:01 2023, max compression
+gzip compressed data, was "/builds/lhcb-rta/pidcalib2/dist/.tmp-g8myio6a/pidcalib2-1.1.2.tar", last modified: Mon Jun 12 12:13:21 2023, max compression
```

## Comparing `pidcalib2-1.1.1.tar` & `pidcalib2-1.1.2.tar`

### file list

```diff
@@ -1,72 +1,72 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-11 12:06:01.000000 pidcalib2-1.1.1/
--rw-r--r--   0 root         (0) root         (0)       69 2023-04-11 12:05:45.000000 pidcalib2-1.1.1/.coveragerc
--rw-r--r--   0 root         (0) root         (0)       30 2023-04-11 12:05:45.000000 pidcalib2-1.1.1/.flake8
--rw-r--r--   0 root         (0) root         (0)     2267 2023-04-11 12:05:45.000000 pidcalib2-1.1.1/.gitignore
--rw-r--r--   0 root         (0) root         (0)     2364 2023-04-11 12:05:45.000000 pidcalib2-1.1.1/.gitlab-ci.yml
--rw-r--r--   0 root         (0) root         (0)       37 2023-04-11 12:05:45.000000 pidcalib2-1.1.1/.mypy.ini
--rw-r--r--   0 root         (0) root         (0)      690 2023-04-11 12:05:45.000000 pidcalib2-1.1.1/.pre-commit-config.yaml
--rw-r--r--   0 root         (0) root         (0)    18151 2023-04-11 12:05:45.000000 pidcalib2-1.1.1/.pylintrc
--rw-r--r--   0 root         (0) root         (0)      138 2023-04-11 12:05:45.000000 pidcalib2-1.1.1/.sourcery.yaml
--rw-r--r--   0 root         (0) root         (0)    35065 2023-04-11 12:05:45.000000 pidcalib2-1.1.1/LICENSE
--rw-r--r--   0 root         (0) root         (0)    15428 2023-04-11 12:06:01.000000 pidcalib2-1.1.1/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)    14817 2023-04-11 12:05:45.000000 pidcalib2-1.1.1/README.md
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-11 12:06:01.000000 pidcalib2-1.1.1/notebooks/
--rw-r--r--   0 root         (0) root         (0)    15142 2023-04-11 12:05:45.000000 pidcalib2-1.1.1/notebooks/plots.ipynb
--rw-r--r--   0 root         (0) root         (0)      654 2023-04-11 12:05:45.000000 pidcalib2-1.1.1/pyproject.toml
--rw-r--r--   0 root         (0) root         (0)      371 2023-04-11 12:05:45.000000 pidcalib2-1.1.1/requirements-ci.txt
--rw-r--r--   0 root         (0) root         (0)      796 2023-04-11 12:05:45.000000 pidcalib2-1.1.1/requirements-dev.txt
--rw-r--r--   0 root         (0) root         (0)     1304 2023-04-11 12:06:01.000000 pidcalib2-1.1.1/setup.cfg
--rw-r--r--   0 root         (0) root         (0)      894 2023-04-11 12:05:45.000000 pidcalib2-1.1.1/setup.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-11 12:06:01.000000 pidcalib2-1.1.1/src/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-11 12:06:01.000000 pidcalib2-1.1.1/src/pidcalib2/
--rw-r--r--   0 root         (0) root         (0)      577 2023-04-11 12:05:45.000000 pidcalib2-1.1.1/src/pidcalib2/__init__.py
--rw-r--r--   0 root         (0) root         (0)     1173 2023-04-11 12:05:45.000000 pidcalib2-1.1.1/src/pidcalib2/__main__.py
--rw-r--r--   0 root         (0) root         (0)     5212 2023-04-11 12:05:45.000000 pidcalib2-1.1.1/src/pidcalib2/aliases.py
--rw-r--r--   0 root         (0) root         (0)     2709 2023-04-11 12:05:45.000000 pidcalib2-1.1.1/src/pidcalib2/argparse_tools.py
--rw-r--r--   0 root         (0) root         (0)     9884 2023-04-11 12:05:45.000000 pidcalib2-1.1.1/src/pidcalib2/binning.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-11 12:06:01.000000 pidcalib2-1.1.1/src/pidcalib2/data/
--rw-r--r--   0 root         (0) root         (0)   819948 2023-04-11 12:05:45.000000 pidcalib2-1.1.1/src/pidcalib2/data/samples.json
--rw-r--r--   0 root         (0) root         (0)     8179 2023-04-11 12:05:45.000000 pidcalib2-1.1.1/src/pidcalib2/make_eff_hists.py
--rw-r--r--   0 root         (0) root         (0)     3996 2023-04-11 12:05:45.000000 pidcalib2-1.1.1/src/pidcalib2/markdown_table.py
--rw-r--r--   0 root         (0) root         (0)     3496 2023-04-11 12:05:45.000000 pidcalib2-1.1.1/src/pidcalib2/merge_trees.py
--rw-r--r--   0 root         (0) root         (0)    16282 2023-04-11 12:05:45.000000 pidcalib2-1.1.1/src/pidcalib2/pid_data.py
--rw-r--r--   0 root         (0) root         (0)     6754 2023-04-11 12:05:45.000000 pidcalib2-1.1.1/src/pidcalib2/pklhisto2root.py
--rw-r--r--   0 root         (0) root         (0)    13557 2023-04-11 12:05:45.000000 pidcalib2-1.1.1/src/pidcalib2/plot_calib_distributions.py
--rw-r--r--   0 root         (0) root         (0)     9937 2023-04-11 12:05:45.000000 pidcalib2-1.1.1/src/pidcalib2/ref_calib.py
--rw-r--r--   0 root         (0) root         (0)     2593 2023-04-11 12:05:45.000000 pidcalib2-1.1.1/src/pidcalib2/samples.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-11 12:06:01.000000 pidcalib2-1.1.1/src/pidcalib2/tests/
--rw-r--r--   0 root         (0) root         (0)       57 2023-04-11 12:05:45.000000 pidcalib2-1.1.1/src/pidcalib2/tests/__init__.py
--rw-r--r--   0 root         (0) root         (0)     2320 2023-04-11 12:05:45.000000 pidcalib2-1.1.1/src/pidcalib2/tests/test_binning.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-11 12:06:01.000000 pidcalib2-1.1.1/src/pidcalib2/tests/test_data/
--rw-r--r--   0 root         (0) root         (0)     9898 2023-04-11 12:05:45.000000 pidcalib2-1.1.1/src/pidcalib2/tests/test_data/cal_test_data.csv
--rw-r--r--   0 root         (0) root         (0)     5653 2023-04-11 12:05:45.000000 pidcalib2-1.1.1/src/pidcalib2/tests/test_data/cal_test_data.pkl
--rw-r--r--   0 root         (0) root         (0)      103 2023-04-11 12:05:45.000000 pidcalib2-1.1.1/src/pidcalib2/tests/test_data/custom_binning.json
--rw-r--r--   0 root         (0) root         (0)     2556 2023-04-11 12:05:45.000000 pidcalib2-1.1.1/src/pidcalib2/tests/test_data/effhists-Turbo18-up-K-DLLK>0-P-pre1.1.0.pkl
--rw-r--r--   0 root         (0) root         (0)     2507 2023-04-11 12:05:45.000000 pidcalib2-1.1.1/src/pidcalib2/tests/test_data/effhists-Turbo18-up-K-DLLK>0-P.pkl
--rw-r--r--   0 root         (0) root         (0)    36807 2023-04-11 12:05:45.000000 pidcalib2-1.1.1/src/pidcalib2/tests/test_data/effhists-Turbo18-up-K-DLLK>4-P.ETA.nTracks.pkl
--rw-r--r--   0 root         (0) root         (0)     2556 2023-04-11 12:05:45.000000 pidcalib2-1.1.1/src/pidcalib2/tests/test_data/effhists-Turbo18-up-Pi-DLLK<0-P.pkl
--rw-r--r--   0 root         (0) root         (0)      865 2023-04-11 12:05:45.000000 pidcalib2-1.1.1/src/pidcalib2/tests/test_data/effhists-Turbo18-up-pi-DLLK<4-P.pkl
--rw-r--r--   0 root         (0) root         (0)    20907 2023-04-11 12:05:45.000000 pidcalib2-1.1.1/src/pidcalib2/tests/test_data/ref_PID_eff.root
--rw-r--r--   0 root         (0) root         (0)     8045 2023-04-11 12:05:45.000000 pidcalib2-1.1.1/src/pidcalib2/tests/test_data/ref_test_data.csv
--rw-r--r--   0 root         (0) root         (0)     9244 2023-04-11 12:05:45.000000 pidcalib2-1.1.1/src/pidcalib2/tests/test_data/ref_test_data.root
--rw-r--r--   0 root         (0) root         (0)     9817 2023-04-11 12:05:45.000000 pidcalib2-1.1.1/src/pidcalib2/tests/test_data/ref_test_data_subdir.root
--rw-r--r--   0 root         (0) root         (0)      127 2023-04-11 12:05:45.000000 pidcalib2-1.1.1/src/pidcalib2/tests/test_data/test_file_list
--rw-r--r--   0 root         (0) root         (0)      206 2023-04-11 12:05:45.000000 pidcalib2-1.1.1/src/pidcalib2/tests/test_data/test_samples.json
--rw-r--r--   0 root         (0) root         (0)     9950 2023-04-11 12:05:45.000000 pidcalib2-1.1.1/src/pidcalib2/tests/test_make_eff_hist.py
--rw-r--r--   0 root         (0) root         (0)     4109 2023-04-11 12:05:45.000000 pidcalib2-1.1.1/src/pidcalib2/tests/test_merge_trees.py
--rw-r--r--   0 root         (0) root         (0)     8095 2023-04-11 12:05:45.000000 pidcalib2-1.1.1/src/pidcalib2/tests/test_pid_data.py
--rw-r--r--   0 root         (0) root         (0)     2549 2023-04-11 12:05:45.000000 pidcalib2-1.1.1/src/pidcalib2/tests/test_pklhisto2root.py
--rw-r--r--   0 root         (0) root         (0)     4297 2023-04-11 12:05:45.000000 pidcalib2-1.1.1/src/pidcalib2/tests/test_plot_calib_distributions.py
--rw-r--r--   0 root         (0) root         (0)     4097 2023-04-11 12:05:45.000000 pidcalib2-1.1.1/src/pidcalib2/tests/test_ref_calib.py
--rw-r--r--   0 root         (0) root         (0)     4597 2023-04-11 12:05:45.000000 pidcalib2-1.1.1/src/pidcalib2/tests/test_utils.py
--rw-r--r--   0 root         (0) root         (0)    25950 2023-04-11 12:05:45.000000 pidcalib2-1.1.1/src/pidcalib2/utils.py
--rw-r--r--   0 root         (0) root         (0)      160 2023-04-11 12:06:01.000000 pidcalib2-1.1.1/src/pidcalib2/version.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-11 12:06:01.000000 pidcalib2-1.1.1/src/pidcalib2.egg-info/
--rw-r--r--   0 root         (0) root         (0)    15428 2023-04-11 12:06:01.000000 pidcalib2-1.1.1/src/pidcalib2.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     2059 2023-04-11 12:06:01.000000 pidcalib2-1.1.1/src/pidcalib2.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-04-11 12:06:01.000000 pidcalib2-1.1.1/src/pidcalib2.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)      305 2023-04-11 12:06:01.000000 pidcalib2-1.1.1/src/pidcalib2.egg-info/entry_points.txt
--rw-r--r--   0 root         (0) root         (0)       86 2023-04-11 12:06:01.000000 pidcalib2-1.1.1/src/pidcalib2.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)       10 2023-04-11 12:06:01.000000 pidcalib2-1.1.1/src/pidcalib2.egg-info/top_level.txt
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-11 12:06:01.000000 pidcalib2-1.1.1/typings/
--rw-r--r--   0 root         (0) root         (0)       53 2023-04-11 12:05:45.000000 pidcalib2-1.1.1/typings/ROOT.pyi
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-12 12:13:21.000000 pidcalib2-1.1.2/
+-rw-r--r--   0 root         (0) root         (0)       69 2023-06-12 12:13:11.000000 pidcalib2-1.1.2/.coveragerc
+-rw-r--r--   0 root         (0) root         (0)       30 2023-06-12 12:13:11.000000 pidcalib2-1.1.2/.flake8
+-rw-r--r--   0 root         (0) root         (0)     2267 2023-06-12 12:13:11.000000 pidcalib2-1.1.2/.gitignore
+-rw-r--r--   0 root         (0) root         (0)     2364 2023-06-12 12:13:11.000000 pidcalib2-1.1.2/.gitlab-ci.yml
+-rw-r--r--   0 root         (0) root         (0)       37 2023-06-12 12:13:11.000000 pidcalib2-1.1.2/.mypy.ini
+-rw-r--r--   0 root         (0) root         (0)      690 2023-06-12 12:13:11.000000 pidcalib2-1.1.2/.pre-commit-config.yaml
+-rw-r--r--   0 root         (0) root         (0)    18151 2023-06-12 12:13:11.000000 pidcalib2-1.1.2/.pylintrc
+-rw-r--r--   0 root         (0) root         (0)      138 2023-06-12 12:13:11.000000 pidcalib2-1.1.2/.sourcery.yaml
+-rw-r--r--   0 root         (0) root         (0)    35065 2023-06-12 12:13:11.000000 pidcalib2-1.1.2/LICENSE
+-rw-r--r--   0 root         (0) root         (0)    15428 2023-06-12 12:13:21.000000 pidcalib2-1.1.2/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)    14817 2023-06-12 12:13:11.000000 pidcalib2-1.1.2/README.md
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-12 12:13:21.000000 pidcalib2-1.1.2/notebooks/
+-rw-r--r--   0 root         (0) root         (0)    15142 2023-06-12 12:13:11.000000 pidcalib2-1.1.2/notebooks/plots.ipynb
+-rw-r--r--   0 root         (0) root         (0)      654 2023-06-12 12:13:11.000000 pidcalib2-1.1.2/pyproject.toml
+-rw-r--r--   0 root         (0) root         (0)      371 2023-06-12 12:13:11.000000 pidcalib2-1.1.2/requirements-ci.txt
+-rw-r--r--   0 root         (0) root         (0)      796 2023-06-12 12:13:11.000000 pidcalib2-1.1.2/requirements-dev.txt
+-rw-r--r--   0 root         (0) root         (0)     1304 2023-06-12 12:13:21.000000 pidcalib2-1.1.2/setup.cfg
+-rw-r--r--   0 root         (0) root         (0)      894 2023-06-12 12:13:11.000000 pidcalib2-1.1.2/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-12 12:13:21.000000 pidcalib2-1.1.2/src/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-12 12:13:21.000000 pidcalib2-1.1.2/src/pidcalib2/
+-rw-r--r--   0 root         (0) root         (0)      577 2023-06-12 12:13:11.000000 pidcalib2-1.1.2/src/pidcalib2/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     1173 2023-06-12 12:13:11.000000 pidcalib2-1.1.2/src/pidcalib2/__main__.py
+-rw-r--r--   0 root         (0) root         (0)     5212 2023-06-12 12:13:11.000000 pidcalib2-1.1.2/src/pidcalib2/aliases.py
+-rw-r--r--   0 root         (0) root         (0)     2709 2023-06-12 12:13:11.000000 pidcalib2-1.1.2/src/pidcalib2/argparse_tools.py
+-rw-r--r--   0 root         (0) root         (0)     9884 2023-06-12 12:13:11.000000 pidcalib2-1.1.2/src/pidcalib2/binning.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-12 12:13:21.000000 pidcalib2-1.1.2/src/pidcalib2/data/
+-rw-r--r--   0 root         (0) root         (0)   819948 2023-06-12 12:13:11.000000 pidcalib2-1.1.2/src/pidcalib2/data/samples.json
+-rw-r--r--   0 root         (0) root         (0)     8179 2023-06-12 12:13:11.000000 pidcalib2-1.1.2/src/pidcalib2/make_eff_hists.py
+-rw-r--r--   0 root         (0) root         (0)     3996 2023-06-12 12:13:11.000000 pidcalib2-1.1.2/src/pidcalib2/markdown_table.py
+-rw-r--r--   0 root         (0) root         (0)     3496 2023-06-12 12:13:11.000000 pidcalib2-1.1.2/src/pidcalib2/merge_trees.py
+-rw-r--r--   0 root         (0) root         (0)    16282 2023-06-12 12:13:11.000000 pidcalib2-1.1.2/src/pidcalib2/pid_data.py
+-rw-r--r--   0 root         (0) root         (0)     6754 2023-06-12 12:13:11.000000 pidcalib2-1.1.2/src/pidcalib2/pklhisto2root.py
+-rw-r--r--   0 root         (0) root         (0)    13557 2023-06-12 12:13:11.000000 pidcalib2-1.1.2/src/pidcalib2/plot_calib_distributions.py
+-rw-r--r--   0 root         (0) root         (0)     9937 2023-06-12 12:13:11.000000 pidcalib2-1.1.2/src/pidcalib2/ref_calib.py
+-rw-r--r--   0 root         (0) root         (0)     2593 2023-06-12 12:13:11.000000 pidcalib2-1.1.2/src/pidcalib2/samples.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-12 12:13:21.000000 pidcalib2-1.1.2/src/pidcalib2/tests/
+-rw-r--r--   0 root         (0) root         (0)       57 2023-06-12 12:13:11.000000 pidcalib2-1.1.2/src/pidcalib2/tests/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     2320 2023-06-12 12:13:11.000000 pidcalib2-1.1.2/src/pidcalib2/tests/test_binning.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-12 12:13:21.000000 pidcalib2-1.1.2/src/pidcalib2/tests/test_data/
+-rw-r--r--   0 root         (0) root         (0)     9898 2023-06-12 12:13:11.000000 pidcalib2-1.1.2/src/pidcalib2/tests/test_data/cal_test_data.csv
+-rw-r--r--   0 root         (0) root         (0)     5653 2023-06-12 12:13:11.000000 pidcalib2-1.1.2/src/pidcalib2/tests/test_data/cal_test_data.pkl
+-rw-r--r--   0 root         (0) root         (0)      103 2023-06-12 12:13:11.000000 pidcalib2-1.1.2/src/pidcalib2/tests/test_data/custom_binning.json
+-rw-r--r--   0 root         (0) root         (0)     2556 2023-06-12 12:13:11.000000 pidcalib2-1.1.2/src/pidcalib2/tests/test_data/effhists-Turbo18-up-K-DLLK>0-P-pre1.1.0.pkl
+-rw-r--r--   0 root         (0) root         (0)     2507 2023-06-12 12:13:11.000000 pidcalib2-1.1.2/src/pidcalib2/tests/test_data/effhists-Turbo18-up-K-DLLK>0-P.pkl
+-rw-r--r--   0 root         (0) root         (0)    36807 2023-06-12 12:13:11.000000 pidcalib2-1.1.2/src/pidcalib2/tests/test_data/effhists-Turbo18-up-K-DLLK>4-P.ETA.nTracks.pkl
+-rw-r--r--   0 root         (0) root         (0)     2556 2023-06-12 12:13:11.000000 pidcalib2-1.1.2/src/pidcalib2/tests/test_data/effhists-Turbo18-up-Pi-DLLK<0-P.pkl
+-rw-r--r--   0 root         (0) root         (0)      865 2023-06-12 12:13:11.000000 pidcalib2-1.1.2/src/pidcalib2/tests/test_data/effhists-Turbo18-up-pi-DLLK<4-P.pkl
+-rw-r--r--   0 root         (0) root         (0)    20907 2023-06-12 12:13:11.000000 pidcalib2-1.1.2/src/pidcalib2/tests/test_data/ref_PID_eff.root
+-rw-r--r--   0 root         (0) root         (0)     8045 2023-06-12 12:13:11.000000 pidcalib2-1.1.2/src/pidcalib2/tests/test_data/ref_test_data.csv
+-rw-r--r--   0 root         (0) root         (0)     9244 2023-06-12 12:13:11.000000 pidcalib2-1.1.2/src/pidcalib2/tests/test_data/ref_test_data.root
+-rw-r--r--   0 root         (0) root         (0)     9817 2023-06-12 12:13:11.000000 pidcalib2-1.1.2/src/pidcalib2/tests/test_data/ref_test_data_subdir.root
+-rw-r--r--   0 root         (0) root         (0)      127 2023-06-12 12:13:11.000000 pidcalib2-1.1.2/src/pidcalib2/tests/test_data/test_file_list
+-rw-r--r--   0 root         (0) root         (0)      206 2023-06-12 12:13:11.000000 pidcalib2-1.1.2/src/pidcalib2/tests/test_data/test_samples.json
+-rw-r--r--   0 root         (0) root         (0)     9950 2023-06-12 12:13:11.000000 pidcalib2-1.1.2/src/pidcalib2/tests/test_make_eff_hist.py
+-rw-r--r--   0 root         (0) root         (0)     4109 2023-06-12 12:13:11.000000 pidcalib2-1.1.2/src/pidcalib2/tests/test_merge_trees.py
+-rw-r--r--   0 root         (0) root         (0)     8095 2023-06-12 12:13:11.000000 pidcalib2-1.1.2/src/pidcalib2/tests/test_pid_data.py
+-rw-r--r--   0 root         (0) root         (0)     2549 2023-06-12 12:13:11.000000 pidcalib2-1.1.2/src/pidcalib2/tests/test_pklhisto2root.py
+-rw-r--r--   0 root         (0) root         (0)     4297 2023-06-12 12:13:11.000000 pidcalib2-1.1.2/src/pidcalib2/tests/test_plot_calib_distributions.py
+-rw-r--r--   0 root         (0) root         (0)     4097 2023-06-12 12:13:11.000000 pidcalib2-1.1.2/src/pidcalib2/tests/test_ref_calib.py
+-rw-r--r--   0 root         (0) root         (0)     4597 2023-06-12 12:13:11.000000 pidcalib2-1.1.2/src/pidcalib2/tests/test_utils.py
+-rw-r--r--   0 root         (0) root         (0)    26220 2023-06-12 12:13:11.000000 pidcalib2-1.1.2/src/pidcalib2/utils.py
+-rw-r--r--   0 root         (0) root         (0)      160 2023-06-12 12:13:21.000000 pidcalib2-1.1.2/src/pidcalib2/version.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-12 12:13:21.000000 pidcalib2-1.1.2/src/pidcalib2.egg-info/
+-rw-r--r--   0 root         (0) root         (0)    15428 2023-06-12 12:13:21.000000 pidcalib2-1.1.2/src/pidcalib2.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     2059 2023-06-12 12:13:21.000000 pidcalib2-1.1.2/src/pidcalib2.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-06-12 12:13:21.000000 pidcalib2-1.1.2/src/pidcalib2.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)      305 2023-06-12 12:13:21.000000 pidcalib2-1.1.2/src/pidcalib2.egg-info/entry_points.txt
+-rw-r--r--   0 root         (0) root         (0)       86 2023-06-12 12:13:21.000000 pidcalib2-1.1.2/src/pidcalib2.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)       10 2023-06-12 12:13:21.000000 pidcalib2-1.1.2/src/pidcalib2.egg-info/top_level.txt
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-12 12:13:21.000000 pidcalib2-1.1.2/typings/
+-rw-r--r--   0 root         (0) root         (0)       53 2023-06-12 12:13:11.000000 pidcalib2-1.1.2/typings/ROOT.pyi
```

### Comparing `pidcalib2-1.1.1/.gitignore` & `pidcalib2-1.1.2/.gitignore`

 * *Files identical despite different names*

### Comparing `pidcalib2-1.1.1/.gitlab-ci.yml` & `pidcalib2-1.1.2/.gitlab-ci.yml`

 * *Files identical despite different names*

### Comparing `pidcalib2-1.1.1/.pre-commit-config.yaml` & `pidcalib2-1.1.2/.pre-commit-config.yaml`

 * *Files identical despite different names*

### Comparing `pidcalib2-1.1.1/.pylintrc` & `pidcalib2-1.1.2/.pylintrc`

 * *Files identical despite different names*

### Comparing `pidcalib2-1.1.1/LICENSE` & `pidcalib2-1.1.2/LICENSE`

 * *Files identical despite different names*

### Comparing `pidcalib2-1.1.1/PKG-INFO` & `pidcalib2-1.1.2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pidcalib2
-Version: 1.1.1
+Version: 1.1.2
 Summary: A set of tools for estimating LHCb PID efficiencies
 Home-page: https://gitlab.cern.ch/lhcb-rta/pidcalib2
 Author: Daniel Cervenkov
 Author-email: daniel.cervenkov@cern.ch
 License: GNU General Public License v3 (GPLv3)
 Project-URL: Bug Tracker, https://gitlab.cern.ch/lhcb-rta/pidcalib2/issues
 Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
```

### Comparing `pidcalib2-1.1.1/README.md` & `pidcalib2-1.1.2/README.md`

 * *Files identical despite different names*

### Comparing `pidcalib2-1.1.1/notebooks/plots.ipynb` & `pidcalib2-1.1.2/notebooks/plots.ipynb`

 * *Files identical despite different names*

### Comparing `pidcalib2-1.1.1/pyproject.toml` & `pidcalib2-1.1.2/pyproject.toml`

 * *Files identical despite different names*

### Comparing `pidcalib2-1.1.1/requirements-dev.txt` & `pidcalib2-1.1.2/requirements-dev.txt`

 * *Files identical despite different names*

### Comparing `pidcalib2-1.1.1/setup.cfg` & `pidcalib2-1.1.2/setup.cfg`

 * *Files identical despite different names*

### Comparing `pidcalib2-1.1.1/setup.py` & `pidcalib2-1.1.2/setup.py`

 * *Files identical despite different names*

### Comparing `pidcalib2-1.1.1/src/pidcalib2/__init__.py` & `pidcalib2-1.1.2/src/pidcalib2/__init__.py`

 * *Files identical despite different names*

### Comparing `pidcalib2-1.1.1/src/pidcalib2/__main__.py` & `pidcalib2-1.1.2/src/pidcalib2/__main__.py`

 * *Files identical despite different names*

### Comparing `pidcalib2-1.1.1/src/pidcalib2/aliases.py` & `pidcalib2-1.1.2/src/pidcalib2/aliases.py`

 * *Files identical despite different names*

### Comparing `pidcalib2-1.1.1/src/pidcalib2/argparse_tools.py` & `pidcalib2-1.1.2/src/pidcalib2/argparse_tools.py`

 * *Files identical despite different names*

### Comparing `pidcalib2-1.1.1/src/pidcalib2/binning.py` & `pidcalib2-1.1.2/src/pidcalib2/binning.py`

 * *Files identical despite different names*

### Comparing `pidcalib2-1.1.1/src/pidcalib2/data/samples.json` & `pidcalib2-1.1.2/src/pidcalib2/data/samples.json`

 * *Files identical despite different names*

### Comparing `pidcalib2-1.1.1/src/pidcalib2/make_eff_hists.py` & `pidcalib2-1.1.2/src/pidcalib2/make_eff_hists.py`

 * *Files identical despite different names*

### Comparing `pidcalib2-1.1.1/src/pidcalib2/markdown_table.py` & `pidcalib2-1.1.2/src/pidcalib2/markdown_table.py`

 * *Files identical despite different names*

### Comparing `pidcalib2-1.1.1/src/pidcalib2/merge_trees.py` & `pidcalib2-1.1.2/src/pidcalib2/merge_trees.py`

 * *Files identical despite different names*

### Comparing `pidcalib2-1.1.1/src/pidcalib2/pid_data.py` & `pidcalib2-1.1.2/src/pidcalib2/pid_data.py`

 * *Files identical despite different names*

### Comparing `pidcalib2-1.1.1/src/pidcalib2/pklhisto2root.py` & `pidcalib2-1.1.2/src/pidcalib2/pklhisto2root.py`

 * *Files identical despite different names*

### Comparing `pidcalib2-1.1.1/src/pidcalib2/plot_calib_distributions.py` & `pidcalib2-1.1.2/src/pidcalib2/plot_calib_distributions.py`

 * *Files identical despite different names*

### Comparing `pidcalib2-1.1.1/src/pidcalib2/ref_calib.py` & `pidcalib2-1.1.2/src/pidcalib2/ref_calib.py`

 * *Files identical despite different names*

### Comparing `pidcalib2-1.1.1/src/pidcalib2/samples.py` & `pidcalib2-1.1.2/src/pidcalib2/samples.py`

 * *Files identical despite different names*

### Comparing `pidcalib2-1.1.1/src/pidcalib2/tests/test_binning.py` & `pidcalib2-1.1.2/src/pidcalib2/tests/test_binning.py`

 * *Files identical despite different names*

### Comparing `pidcalib2-1.1.1/src/pidcalib2/tests/test_data/cal_test_data.csv` & `pidcalib2-1.1.2/src/pidcalib2/tests/test_data/cal_test_data.csv`

 * *Files identical despite different names*

### Comparing `pidcalib2-1.1.1/src/pidcalib2/tests/test_data/cal_test_data.pkl` & `pidcalib2-1.1.2/src/pidcalib2/tests/test_data/cal_test_data.pkl`

 * *Files identical despite different names*

### Comparing `pidcalib2-1.1.1/src/pidcalib2/tests/test_data/effhists-Turbo18-up-K-DLLK>0-P-pre1.1.0.pkl` & `pidcalib2-1.1.2/src/pidcalib2/tests/test_data/effhists-Turbo18-up-K-DLLK>0-P-pre1.1.0.pkl`

 * *Files identical despite different names*

### Comparing `pidcalib2-1.1.1/src/pidcalib2/tests/test_data/effhists-Turbo18-up-K-DLLK>0-P.pkl` & `pidcalib2-1.1.2/src/pidcalib2/tests/test_data/effhists-Turbo18-up-K-DLLK>0-P.pkl`

 * *Files identical despite different names*

### Comparing `pidcalib2-1.1.1/src/pidcalib2/tests/test_data/effhists-Turbo18-up-K-DLLK>4-P.ETA.nTracks.pkl` & `pidcalib2-1.1.2/src/pidcalib2/tests/test_data/effhists-Turbo18-up-K-DLLK>4-P.ETA.nTracks.pkl`

 * *Files identical despite different names*

### Comparing `pidcalib2-1.1.1/src/pidcalib2/tests/test_data/effhists-Turbo18-up-Pi-DLLK<0-P.pkl` & `pidcalib2-1.1.2/src/pidcalib2/tests/test_data/effhists-Turbo18-up-Pi-DLLK<0-P.pkl`

 * *Files identical despite different names*

### Comparing `pidcalib2-1.1.1/src/pidcalib2/tests/test_data/effhists-Turbo18-up-pi-DLLK<4-P.pkl` & `pidcalib2-1.1.2/src/pidcalib2/tests/test_data/effhists-Turbo18-up-pi-DLLK<4-P.pkl`

 * *Files identical despite different names*

### Comparing `pidcalib2-1.1.1/src/pidcalib2/tests/test_data/ref_PID_eff.root` & `pidcalib2-1.1.2/src/pidcalib2/tests/test_data/ref_PID_eff.root`

 * *Files identical despite different names*

### Comparing `pidcalib2-1.1.1/src/pidcalib2/tests/test_data/ref_test_data.csv` & `pidcalib2-1.1.2/src/pidcalib2/tests/test_data/ref_test_data.csv`

 * *Files identical despite different names*

### Comparing `pidcalib2-1.1.1/src/pidcalib2/tests/test_data/ref_test_data.root` & `pidcalib2-1.1.2/src/pidcalib2/tests/test_data/ref_test_data.root`

 * *Files identical despite different names*

### Comparing `pidcalib2-1.1.1/src/pidcalib2/tests/test_data/ref_test_data_subdir.root` & `pidcalib2-1.1.2/src/pidcalib2/tests/test_data/ref_test_data_subdir.root`

 * *Files identical despite different names*

### Comparing `pidcalib2-1.1.1/src/pidcalib2/tests/test_make_eff_hist.py` & `pidcalib2-1.1.2/src/pidcalib2/tests/test_make_eff_hist.py`

 * *Files identical despite different names*

### Comparing `pidcalib2-1.1.1/src/pidcalib2/tests/test_merge_trees.py` & `pidcalib2-1.1.2/src/pidcalib2/tests/test_merge_trees.py`

 * *Files identical despite different names*

### Comparing `pidcalib2-1.1.1/src/pidcalib2/tests/test_pid_data.py` & `pidcalib2-1.1.2/src/pidcalib2/tests/test_pid_data.py`

 * *Files identical despite different names*

### Comparing `pidcalib2-1.1.1/src/pidcalib2/tests/test_pklhisto2root.py` & `pidcalib2-1.1.2/src/pidcalib2/tests/test_pklhisto2root.py`

 * *Files identical despite different names*

### Comparing `pidcalib2-1.1.1/src/pidcalib2/tests/test_plot_calib_distributions.py` & `pidcalib2-1.1.2/src/pidcalib2/tests/test_plot_calib_distributions.py`

 * *Files identical despite different names*

### Comparing `pidcalib2-1.1.1/src/pidcalib2/tests/test_ref_calib.py` & `pidcalib2-1.1.2/src/pidcalib2/tests/test_ref_calib.py`

 * *Files identical despite different names*

### Comparing `pidcalib2-1.1.1/src/pidcalib2/tests/test_utils.py` & `pidcalib2-1.1.2/src/pidcalib2/tests/test_utils.py`

 * *Files identical despite different names*

### Comparing `pidcalib2-1.1.1/src/pidcalib2/utils.py` & `pidcalib2-1.1.2/src/pidcalib2/utils.py`

 * *Files 2% similar despite different names*

```diff
@@ -15,14 +15,15 @@
 - Creating histograms from dataframes
 - Calculating binomic uncertainties
 - Applying cuts to dataframes
 - Printing configs and cut summaries
 """
 
 import difflib
+import hashlib
 import re
 import sys
 from typing import Any, Dict, List, Tuple, Union
 
 import boost_histogram as bh
 import numpy as np
 import pandas as pd
@@ -305,25 +306,32 @@
 
 
 def create_hist_filename(
     sample: str, magnet: str, particle: str, pid_cut: str, bin_vars: List[str]
 ) -> str:
     """Return effhists filename corresponding to parameters.
 
+    If the name would be longer than 255 characters, the name is truncated and a
+    hash is appended instead.
+
     Args:
         sample: Data sample name (Turbo18, etc.).
         magnet: Magnet polarity (up, down).
         particle: Particle type (K, Pi, etc.).
         pid_cut: Simplified user-level cut, e.g., "DLLK < 4".
         bin_vars: Variables used for binning.
     """
     whitespace = re.compile(r"\s+")
     cut = re.sub(whitespace, "", pid_cut)
+    name = f"effhists-{sample}-{magnet}-{particle}-{cut}-{'.'.join(bin_vars)}.pkl"
+    if len(name) > 255:
+        hash = hashlib.md5(name.encode('utf-8')).hexdigest()
+        return f"{name[:200]}:{hash}.pkl"
 
-    return f"effhists-{sample}-{magnet}-{particle}-{cut}-{'.'.join(bin_vars)}.pkl"
+    return name
 
 
 def binomial_uncertainty(
     num_pass: Union[float, np.ndarray],
     num_total: Union[float, np.ndarray],
     err_pass_sq: Union[float, np.ndarray, None] = None,
     err_tot_sq: Union[float, np.ndarray, None] = None,
```

### Comparing `pidcalib2-1.1.1/src/pidcalib2.egg-info/PKG-INFO` & `pidcalib2-1.1.2/src/pidcalib2.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pidcalib2
-Version: 1.1.1
+Version: 1.1.2
 Summary: A set of tools for estimating LHCb PID efficiencies
 Home-page: https://gitlab.cern.ch/lhcb-rta/pidcalib2
 Author: Daniel Cervenkov
 Author-email: daniel.cervenkov@cern.ch
 License: GNU General Public License v3 (GPLv3)
 Project-URL: Bug Tracker, https://gitlab.cern.ch/lhcb-rta/pidcalib2/issues
 Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
```

### Comparing `pidcalib2-1.1.1/src/pidcalib2.egg-info/SOURCES.txt` & `pidcalib2-1.1.2/src/pidcalib2.egg-info/SOURCES.txt`

 * *Files identical despite different names*

