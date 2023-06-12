# Comparing `tmp/conversion-units-0.0.1.tar.gz` & `tmp/conversion-units-0.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "conversion-units-0.0.1.tar", last modified: Mon Jun 12 01:47:28 2023, max compression
+gzip compressed data, was "conversion-units-0.0.2.tar", last modified: Mon Jun 12 02:54:45 2023, max compression
```

## Comparing `conversion-units-0.0.1.tar` & `conversion-units-0.0.2.tar`

### file list

```diff
@@ -1,11 +1,11 @@
-drwxrwxrwx   0 brice_kengni_zanguim  (1000) brice_kengni_zanguim  (1000)        0 2023-06-12 01:47:28.949528 conversion-units-0.0.1/
--rwxrwxrwx   0 brice_kengni_zanguim  (1000) brice_kengni_zanguim  (1000)     1080 2023-06-11 08:46:24.000000 conversion-units-0.0.1/LICENSE
--rwxrwxrwx   0 brice_kengni_zanguim  (1000) brice_kengni_zanguim  (1000)      981 2023-06-12 01:47:28.949144 conversion-units-0.0.1/PKG-INFO
-drwxrwxrwx   0 brice_kengni_zanguim  (1000) brice_kengni_zanguim  (1000)        0 2023-06-12 01:47:28.942259 conversion-units-0.0.1/conversion_units/
-drwxrwxrwx   0 brice_kengni_zanguim  (1000) brice_kengni_zanguim  (1000)        0 2023-06-12 01:47:28.948052 conversion-units-0.0.1/conversion_units/conversion_units.egg-info/
--rwxrwxrwx   0 brice_kengni_zanguim  (1000) brice_kengni_zanguim  (1000)      981 2023-06-12 01:47:28.000000 conversion-units-0.0.1/conversion_units/conversion_units.egg-info/PKG-INFO
--rwxrwxrwx   0 brice_kengni_zanguim  (1000) brice_kengni_zanguim  (1000)      244 2023-06-12 01:47:28.000000 conversion-units-0.0.1/conversion_units/conversion_units.egg-info/SOURCES.txt
--rwxrwxrwx   0 brice_kengni_zanguim  (1000) brice_kengni_zanguim  (1000)        1 2023-06-12 01:47:28.000000 conversion-units-0.0.1/conversion_units/conversion_units.egg-info/dependency_links.txt
--rwxrwxrwx   0 brice_kengni_zanguim  (1000) brice_kengni_zanguim  (1000)        1 2023-06-12 01:47:28.000000 conversion-units-0.0.1/conversion_units/conversion_units.egg-info/top_level.txt
--rwxrwxrwx   0 brice_kengni_zanguim  (1000) brice_kengni_zanguim  (1000)       38 2023-06-12 01:47:28.949638 conversion-units-0.0.1/setup.cfg
--rwxrwxrwx   0 brice_kengni_zanguim  (1000) brice_kengni_zanguim  (1000)     1038 2023-06-12 01:47:21.000000 conversion-units-0.0.1/setup.py
+drwxrwxrwx   0 brice_kengni_zanguim  (1000) brice_kengni_zanguim  (1000)        0 2023-06-12 02:54:45.357629 conversion-units-0.0.2/
+-rwxrwxrwx   0 brice_kengni_zanguim  (1000) brice_kengni_zanguim  (1000)     1080 2023-06-11 08:46:24.000000 conversion-units-0.0.2/LICENSE
+-rwxrwxrwx   0 brice_kengni_zanguim  (1000) brice_kengni_zanguim  (1000)     1847 2023-06-12 02:54:45.357318 conversion-units-0.0.2/PKG-INFO
+drwxrwxrwx   0 brice_kengni_zanguim  (1000) brice_kengni_zanguim  (1000)        0 2023-06-12 02:54:45.352001 conversion-units-0.0.2/conversion_units/
+drwxrwxrwx   0 brice_kengni_zanguim  (1000) brice_kengni_zanguim  (1000)        0 2023-06-12 02:54:45.356607 conversion-units-0.0.2/conversion_units/conversion_units.egg-info/
+-rwxrwxrwx   0 brice_kengni_zanguim  (1000) brice_kengni_zanguim  (1000)     1847 2023-06-12 02:54:45.000000 conversion-units-0.0.2/conversion_units/conversion_units.egg-info/PKG-INFO
+-rwxrwxrwx   0 brice_kengni_zanguim  (1000) brice_kengni_zanguim  (1000)      244 2023-06-12 02:54:45.000000 conversion-units-0.0.2/conversion_units/conversion_units.egg-info/SOURCES.txt
+-rwxrwxrwx   0 brice_kengni_zanguim  (1000) brice_kengni_zanguim  (1000)        1 2023-06-12 02:54:45.000000 conversion-units-0.0.2/conversion_units/conversion_units.egg-info/dependency_links.txt
+-rwxrwxrwx   0 brice_kengni_zanguim  (1000) brice_kengni_zanguim  (1000)        1 2023-06-12 02:54:45.000000 conversion-units-0.0.2/conversion_units/conversion_units.egg-info/top_level.txt
+-rwxrwxrwx   0 brice_kengni_zanguim  (1000) brice_kengni_zanguim  (1000)       38 2023-06-12 02:54:45.357733 conversion-units-0.0.2/setup.cfg
+-rwxrwxrwx   0 brice_kengni_zanguim  (1000) brice_kengni_zanguim  (1000)     1200 2023-06-12 02:03:13.000000 conversion-units-0.0.2/setup.py
```

### Comparing `conversion-units-0.0.1/LICENSE` & `conversion-units-0.0.2/LICENSE`

 * *Files identical despite different names*

