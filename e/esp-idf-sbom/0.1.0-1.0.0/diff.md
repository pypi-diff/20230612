# Comparing `tmp/esp-idf-sbom-0.1.0.tar.gz` & `tmp/esp-idf-sbom-1.0.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "/home/runner/work/esp-idf-sbom/esp-idf-sbom/dist/.tmp-8lkel82v/esp-idf-sbom-0.1.0.tar", last modified: Mon Jun 12 14:24:59 2023, max compression
+gzip compressed data, was "/home/runner/work/esp-idf-sbom/esp-idf-sbom/dist/.tmp-chtgb59k/esp-idf-sbom-1.0.0.tar", last modified: Fri Jun  2 11:45:29 2023, max compression
```

## Comparing `esp-idf-sbom-0.1.0.tar` & `esp-idf-sbom-1.0.0.tar`

### file list

```diff
@@ -1,26 +1,13 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-12 14:24:59.000000 esp-idf-sbom-0.1.0/
--rw-r--r--   0 runner    (1001) docker     (123)    11365 2023-06-12 14:24:40.000000 esp-idf-sbom-0.1.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     8469 2023-06-12 14:24:59.000000 esp-idf-sbom-0.1.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     7461 2023-06-12 14:24:40.000000 esp-idf-sbom-0.1.0/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-12 14:24:59.000000 esp-idf-sbom-0.1.0/esp-idf-sbom/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-12 14:24:40.000000 esp-idf-sbom-0.1.0/esp-idf-sbom/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-12 14:24:59.000000 esp-idf-sbom-0.1.0/esp_idf_sbom/
--rw-r--r--   0 runner    (1001) docker     (123)      127 2023-06-12 14:24:40.000000 esp-idf-sbom-0.1.0/esp_idf_sbom/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      180 2023-06-12 14:24:40.000000 esp-idf-sbom-0.1.0/esp_idf_sbom/__main__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-12 14:24:59.000000 esp-idf-sbom-0.1.0/esp_idf_sbom/libsbom/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-12 14:24:40.000000 esp-idf-sbom-0.1.0/esp_idf_sbom/libsbom/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4543 2023-06-12 14:24:40.000000 esp-idf-sbom-0.1.0/esp_idf_sbom/libsbom/git.py
--rw-r--r--   0 runner    (1001) docker     (123)     4272 2023-06-12 14:24:40.000000 esp-idf-sbom-0.1.0/esp_idf_sbom/libsbom/log.py
--rw-r--r--   0 runner    (1001) docker     (123)     2289 2023-06-12 14:24:40.000000 esp-idf-sbom-0.1.0/esp_idf_sbom/libsbom/nvd.py
--rw-r--r--   0 runner    (1001) docker     (123)    37759 2023-06-12 14:24:40.000000 esp-idf-sbom-0.1.0/esp_idf_sbom/libsbom/spdx.py
--rw-r--r--   0 runner    (1001) docker     (123)     1962 2023-06-12 14:24:40.000000 esp-idf-sbom-0.1.0/esp_idf_sbom/libsbom/utils.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     9797 2023-06-12 14:24:40.000000 esp-idf-sbom-0.1.0/esp_idf_sbom/sbom.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-12 14:24:59.000000 esp-idf-sbom-0.1.0/esp_idf_sbom.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     8469 2023-06-12 14:24:59.000000 esp-idf-sbom-0.1.0/esp_idf_sbom.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      516 2023-06-12 14:24:59.000000 esp-idf-sbom-0.1.0/esp_idf_sbom.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-12 14:24:59.000000 esp-idf-sbom-0.1.0/esp_idf_sbom.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       56 2023-06-12 14:24:59.000000 esp-idf-sbom-0.1.0/esp_idf_sbom.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)        7 2023-06-12 14:24:59.000000 esp-idf-sbom-0.1.0/esp_idf_sbom.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       26 2023-06-12 14:24:59.000000 esp-idf-sbom-0.1.0/esp_idf_sbom.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-12 14:24:59.000000 esp-idf-sbom-0.1.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     2196 2023-06-12 14:24:40.000000 esp-idf-sbom-0.1.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-02 11:45:29.000000 esp-idf-sbom-1.0.0/
+-rw-r--r--   0 runner    (1001) docker     (123)    11365 2023-06-02 11:45:08.000000 esp-idf-sbom-1.0.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     1001 2023-06-02 11:45:29.000000 esp-idf-sbom-1.0.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)       14 2023-06-02 11:45:08.000000 esp-idf-sbom-1.0.0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-02 11:45:29.000000 esp-idf-sbom-1.0.0/esp-idf-sbom/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-02 11:45:08.000000 esp-idf-sbom-1.0.0/esp-idf-sbom/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-02 11:45:29.000000 esp-idf-sbom-1.0.0/esp_idf_sbom.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     1001 2023-06-02 11:45:29.000000 esp-idf-sbom-1.0.0/esp_idf_sbom.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      195 2023-06-02 11:45:29.000000 esp-idf-sbom-1.0.0/esp_idf_sbom.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-02 11:45:29.000000 esp-idf-sbom-1.0.0/esp_idf_sbom.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       13 2023-06-02 11:45:29.000000 esp-idf-sbom-1.0.0/esp_idf_sbom.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-02 11:45:29.000000 esp-idf-sbom-1.0.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1266 2023-06-02 11:45:08.000000 esp-idf-sbom-1.0.0/setup.py
```

### Comparing `esp-idf-sbom-0.1.0/LICENSE` & `esp-idf-sbom-1.0.0/LICENSE`

 * *Files identical despite different names*

