# Comparing `tmp/wwpdb.utils.dp-0.45.tar.gz` & `tmp/wwpdb.utils.dp-0.46.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "wwpdb.utils.dp-0.45.tar", last modified: Sat Apr 15 23:48:07 2023, max compression
+gzip compressed data, was "wwpdb.utils.dp-0.46.tar", last modified: Sun Jun 11 23:57:20 2023, max compression
```

## Comparing `wwpdb.utils.dp-0.45.tar` & `wwpdb.utils.dp-0.46.tar`

### file list

```diff
@@ -1,37 +1,37 @@
-drwxr-xr-x   0 vsts      (1001) docker     (123)        0 2023-04-15 23:48:07.176215 wwpdb.utils.dp-0.45/
--rw-r--r--   0 vsts      (1001) docker     (123)       96 2023-04-15 23:47:02.000000 wwpdb.utils.dp-0.45/HISTORY.txt
--rw-r--r--   0 vsts      (1001) docker     (123)      552 2023-04-15 23:47:02.000000 wwpdb.utils.dp-0.45/LICENSE
--rw-r--r--   0 vsts      (1001) docker     (123)      104 2023-04-15 23:47:02.000000 wwpdb.utils.dp-0.45/MANIFEST.in
--rw-r--r--   0 vsts      (1001) docker     (123)      755 2023-04-15 23:48:07.176215 wwpdb.utils.dp-0.45/PKG-INFO
--rw-r--r--   0 vsts      (1001) docker     (123)      180 2023-04-15 23:47:02.000000 wwpdb.utils.dp-0.45/README.md
--rwxr-xr-x   0 vsts      (1001) docker     (123)      108 2023-04-15 23:48:07.176215 wwpdb.utils.dp-0.45/setup.cfg
--rwxr-xr-x   0 vsts      (1001) docker     (123)     2125 2023-04-15 23:47:02.000000 wwpdb.utils.dp-0.45/setup.py
-drwxr-xr-x   0 vsts      (1001) docker     (123)        0 2023-04-15 23:48:07.168214 wwpdb.utils.dp-0.45/wwpdb/
--rw-r--r--   0 vsts      (1001) docker     (123)       65 2023-04-15 23:47:02.000000 wwpdb.utils.dp-0.45/wwpdb/__init__.py
-drwxr-xr-x   0 vsts      (1001) docker     (123)        0 2023-04-15 23:48:07.172215 wwpdb.utils.dp-0.45/wwpdb/utils/
--rw-r--r--   0 vsts      (1001) docker     (123)       65 2023-04-15 23:47:02.000000 wwpdb.utils.dp-0.45/wwpdb/utils/__init__.py
-drwxr-xr-x   0 vsts      (1001) docker     (123)        0 2023-04-15 23:48:07.176215 wwpdb.utils.dp-0.45/wwpdb/utils/dp/
--rw-r--r--   0 vsts      (1001) docker     (123)     5332 2023-04-15 23:47:02.000000 wwpdb.utils.dp-0.45/wwpdb/utils/dp/CentreOfMass.py
--rw-r--r--   0 vsts      (1001) docker     (123)    11569 2023-04-15 23:47:02.000000 wwpdb.utils.dp-0.45/wwpdb/utils/dp/DataFileAdapter.py
--rw-r--r--   0 vsts      (1001) docker     (123)     2358 2023-04-15 23:47:02.000000 wwpdb.utils.dp-0.45/wwpdb/utils/dp/DensityWrapper.py
--rw-r--r--   0 vsts      (1001) docker     (123)     1782 2023-04-15 23:47:02.000000 wwpdb.utils.dp-0.45/wwpdb/utils/dp/DepositorSyncUtil.py
--rw-r--r--   0 vsts      (1001) docker     (123)     1918 2023-04-15 23:47:02.000000 wwpdb.utils.dp-0.45/wwpdb/utils/dp/PdbxChemShiftReport.py
--rw-r--r--   0 vsts      (1001) docker     (123)     2694 2023-04-15 23:47:02.000000 wwpdb.utils.dp-0.45/wwpdb/utils/dp/PdbxMergeCategory.py
--rw-r--r--   0 vsts      (1001) docker     (123)     5231 2023-04-15 23:47:02.000000 wwpdb.utils.dp-0.45/wwpdb/utils/dp/PdbxSFMapCoefficients.py
--rw-r--r--   0 vsts      (1001) docker     (123)     2368 2023-04-15 23:47:02.000000 wwpdb.utils.dp-0.45/wwpdb/utils/dp/PdbxStripCategory.py
--rw-r--r--   0 vsts      (1001) docker     (123)   206750 2023-04-15 23:47:02.000000 wwpdb.utils.dp-0.45/wwpdb/utils/dp/RcsbDpUtility.py
--rw-r--r--   0 vsts      (1001) docker     (123)    17219 2023-04-15 23:47:02.000000 wwpdb.utils.dp-0.45/wwpdb/utils/dp/RunRemote.py
--rw-r--r--   0 vsts      (1001) docker     (123)     4429 2023-04-15 23:47:02.000000 wwpdb.utils.dp-0.45/wwpdb/utils/dp/ValidationWrapper.py
--rw-r--r--   0 vsts      (1001) docker     (123)      154 2023-04-15 23:47:02.000000 wwpdb.utils.dp-0.45/wwpdb/utils/dp/__init__.py
-drwxr-xr-x   0 vsts      (1001) docker     (123)        0 2023-04-15 23:48:07.176215 wwpdb.utils.dp-0.45/wwpdb/utils/dp/electron_density/
--rw-r--r--   0 vsts      (1001) docker     (123)        0 2023-04-15 23:47:02.000000 wwpdb.utils.dp-0.45/wwpdb/utils/dp/electron_density/__init__.py
--rw-r--r--   0 vsts      (1001) docker     (123)     3930 2023-04-15 23:47:02.000000 wwpdb.utils.dp-0.45/wwpdb/utils/dp/electron_density/common_functions.py
--rw-r--r--   0 vsts      (1001) docker     (123)     3801 2023-04-15 23:47:02.000000 wwpdb.utils.dp-0.45/wwpdb/utils/dp/electron_density/em_density_map.py
--rw-r--r--   0 vsts      (1001) docker     (123)    10279 2023-04-15 23:47:02.000000 wwpdb.utils.dp-0.45/wwpdb/utils/dp/electron_density/x_ray_density_map.py
-drwxr-xr-x   0 vsts      (1001) docker     (123)        0 2023-04-15 23:48:07.172215 wwpdb.utils.dp-0.45/wwpdb.utils.dp.egg-info/
--rw-r--r--   0 vsts      (1001) docker     (123)      755 2023-04-15 23:48:07.000000 wwpdb.utils.dp-0.45/wwpdb.utils.dp.egg-info/PKG-INFO
--rw-r--r--   0 vsts      (1001) docker     (123)      934 2023-04-15 23:48:07.000000 wwpdb.utils.dp-0.45/wwpdb.utils.dp.egg-info/SOURCES.txt
--rw-r--r--   0 vsts      (1001) docker     (123)        1 2023-04-15 23:48:07.000000 wwpdb.utils.dp-0.45/wwpdb.utils.dp.egg-info/dependency_links.txt
--rw-r--r--   0 vsts      (1001) docker     (123)        1 2023-04-15 23:47:53.000000 wwpdb.utils.dp-0.45/wwpdb.utils.dp.egg-info/not-zip-safe
--rw-r--r--   0 vsts      (1001) docker     (123)      103 2023-04-15 23:48:07.000000 wwpdb.utils.dp-0.45/wwpdb.utils.dp.egg-info/requires.txt
--rw-r--r--   0 vsts      (1001) docker     (123)        6 2023-04-15 23:48:07.000000 wwpdb.utils.dp-0.45/wwpdb.utils.dp.egg-info/top_level.txt
+drwxr-xr-x   0 vsts      (1001) docker     (123)        0 2023-06-11 23:57:20.783711 wwpdb.utils.dp-0.46/
+-rw-r--r--   0 vsts      (1001) docker     (123)       96 2023-06-11 23:56:32.000000 wwpdb.utils.dp-0.46/HISTORY.txt
+-rw-r--r--   0 vsts      (1001) docker     (123)      552 2023-06-11 23:56:32.000000 wwpdb.utils.dp-0.46/LICENSE
+-rw-r--r--   0 vsts      (1001) docker     (123)      104 2023-06-11 23:56:32.000000 wwpdb.utils.dp-0.46/MANIFEST.in
+-rw-r--r--   0 vsts      (1001) docker     (123)      755 2023-06-11 23:57:20.783711 wwpdb.utils.dp-0.46/PKG-INFO
+-rw-r--r--   0 vsts      (1001) docker     (123)      180 2023-06-11 23:56:32.000000 wwpdb.utils.dp-0.46/README.md
+-rwxr-xr-x   0 vsts      (1001) docker     (123)      108 2023-06-11 23:57:20.783711 wwpdb.utils.dp-0.46/setup.cfg
+-rwxr-xr-x   0 vsts      (1001) docker     (123)     2125 2023-06-11 23:56:32.000000 wwpdb.utils.dp-0.46/setup.py
+drwxr-xr-x   0 vsts      (1001) docker     (123)        0 2023-06-11 23:57:20.783711 wwpdb.utils.dp-0.46/wwpdb/
+-rw-r--r--   0 vsts      (1001) docker     (123)       65 2023-06-11 23:56:32.000000 wwpdb.utils.dp-0.46/wwpdb/__init__.py
+drwxr-xr-x   0 vsts      (1001) docker     (123)        0 2023-06-11 23:57:20.783711 wwpdb.utils.dp-0.46/wwpdb/utils/
+-rw-r--r--   0 vsts      (1001) docker     (123)       65 2023-06-11 23:56:32.000000 wwpdb.utils.dp-0.46/wwpdb/utils/__init__.py
+drwxr-xr-x   0 vsts      (1001) docker     (123)        0 2023-06-11 23:57:20.783711 wwpdb.utils.dp-0.46/wwpdb/utils/dp/
+-rw-r--r--   0 vsts      (1001) docker     (123)     5332 2023-06-11 23:56:32.000000 wwpdb.utils.dp-0.46/wwpdb/utils/dp/CentreOfMass.py
+-rw-r--r--   0 vsts      (1001) docker     (123)    11569 2023-06-11 23:56:32.000000 wwpdb.utils.dp-0.46/wwpdb/utils/dp/DataFileAdapter.py
+-rw-r--r--   0 vsts      (1001) docker     (123)     2358 2023-06-11 23:56:32.000000 wwpdb.utils.dp-0.46/wwpdb/utils/dp/DensityWrapper.py
+-rw-r--r--   0 vsts      (1001) docker     (123)     1782 2023-06-11 23:56:32.000000 wwpdb.utils.dp-0.46/wwpdb/utils/dp/DepositorSyncUtil.py
+-rw-r--r--   0 vsts      (1001) docker     (123)     1918 2023-06-11 23:56:32.000000 wwpdb.utils.dp-0.46/wwpdb/utils/dp/PdbxChemShiftReport.py
+-rw-r--r--   0 vsts      (1001) docker     (123)     2694 2023-06-11 23:56:32.000000 wwpdb.utils.dp-0.46/wwpdb/utils/dp/PdbxMergeCategory.py
+-rw-r--r--   0 vsts      (1001) docker     (123)     5231 2023-06-11 23:56:32.000000 wwpdb.utils.dp-0.46/wwpdb/utils/dp/PdbxSFMapCoefficients.py
+-rw-r--r--   0 vsts      (1001) docker     (123)     2368 2023-06-11 23:56:32.000000 wwpdb.utils.dp-0.46/wwpdb/utils/dp/PdbxStripCategory.py
+-rw-r--r--   0 vsts      (1001) docker     (123)   207589 2023-06-11 23:56:32.000000 wwpdb.utils.dp-0.46/wwpdb/utils/dp/RcsbDpUtility.py
+-rw-r--r--   0 vsts      (1001) docker     (123)    17219 2023-06-11 23:56:32.000000 wwpdb.utils.dp-0.46/wwpdb/utils/dp/RunRemote.py
+-rw-r--r--   0 vsts      (1001) docker     (123)     4429 2023-06-11 23:56:32.000000 wwpdb.utils.dp-0.46/wwpdb/utils/dp/ValidationWrapper.py
+-rw-r--r--   0 vsts      (1001) docker     (123)      154 2023-06-11 23:56:32.000000 wwpdb.utils.dp-0.46/wwpdb/utils/dp/__init__.py
+drwxr-xr-x   0 vsts      (1001) docker     (123)        0 2023-06-11 23:57:20.783711 wwpdb.utils.dp-0.46/wwpdb/utils/dp/electron_density/
+-rw-r--r--   0 vsts      (1001) docker     (123)        0 2023-06-11 23:56:32.000000 wwpdb.utils.dp-0.46/wwpdb/utils/dp/electron_density/__init__.py
+-rw-r--r--   0 vsts      (1001) docker     (123)     3930 2023-06-11 23:56:32.000000 wwpdb.utils.dp-0.46/wwpdb/utils/dp/electron_density/common_functions.py
+-rw-r--r--   0 vsts      (1001) docker     (123)     3801 2023-06-11 23:56:32.000000 wwpdb.utils.dp-0.46/wwpdb/utils/dp/electron_density/em_density_map.py
+-rw-r--r--   0 vsts      (1001) docker     (123)    10279 2023-06-11 23:56:32.000000 wwpdb.utils.dp-0.46/wwpdb/utils/dp/electron_density/x_ray_density_map.py
+drwxr-xr-x   0 vsts      (1001) docker     (123)        0 2023-06-11 23:57:20.783711 wwpdb.utils.dp-0.46/wwpdb.utils.dp.egg-info/
+-rw-r--r--   0 vsts      (1001) docker     (123)      755 2023-06-11 23:57:20.000000 wwpdb.utils.dp-0.46/wwpdb.utils.dp.egg-info/PKG-INFO
+-rw-r--r--   0 vsts      (1001) docker     (123)      934 2023-06-11 23:57:20.000000 wwpdb.utils.dp-0.46/wwpdb.utils.dp.egg-info/SOURCES.txt
+-rw-r--r--   0 vsts      (1001) docker     (123)        1 2023-06-11 23:57:20.000000 wwpdb.utils.dp-0.46/wwpdb.utils.dp.egg-info/dependency_links.txt
+-rw-r--r--   0 vsts      (1001) docker     (123)        1 2023-06-11 23:57:10.000000 wwpdb.utils.dp-0.46/wwpdb.utils.dp.egg-info/not-zip-safe
+-rw-r--r--   0 vsts      (1001) docker     (123)      103 2023-06-11 23:57:20.000000 wwpdb.utils.dp-0.46/wwpdb.utils.dp.egg-info/requires.txt
+-rw-r--r--   0 vsts      (1001) docker     (123)        6 2023-06-11 23:57:20.000000 wwpdb.utils.dp-0.46/wwpdb.utils.dp.egg-info/top_level.txt
```

### Comparing `wwpdb.utils.dp-0.45/LICENSE` & `wwpdb.utils.dp-0.46/LICENSE`

 * *Files identical despite different names*

### Comparing `wwpdb.utils.dp-0.45/PKG-INFO` & `wwpdb.utils.dp-0.46/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: wwpdb.utils.dp
-Version: 0.45
+Version: 0.46
 Summary: API for Common Data Processing Operations
 Home-page: https://github.com/wwpdb/py-wwpdb_utils_dp
 Author: John Westbrook
 Author-email: john.westbrook@rcsb.org
 License: Apache 2.0
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
```

### Comparing `wwpdb.utils.dp-0.45/setup.py` & `wwpdb.utils.dp-0.46/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -37,15 +37,15 @@
         "Programming Language :: Python :: 2.7",
         "Programming Language :: Python :: 3",
         "Programming Language :: Python :: 3.6",
         "Programming Language :: Python :: 3.7",
     ],
     entry_points={"console_scripts": []},
     #
-    install_requires=["future", "mmcif ~= 0.18", "wwpdb.utils.config >= 0.32", "wwpdb.io", "gemmi >= 0.4"],
+    install_requires=["future", "mmcif ~= 0.18", "wwpdb.utils.config >= 0.34", "wwpdb.io", "gemmi >= 0.4"],
     packages=find_packages(exclude=["wwpdb.mock-data", "wwpdb.utils.tests-dp", "tests.*"]),
     package_data={
         # If any package contains *.md or *.rst ...  files, include them:
         "": ["*.md", "*.rst", "*.txt", "*.cfg"],
     },
     #
     # These basic tests require no database services -
```

### Comparing `wwpdb.utils.dp-0.45/wwpdb/utils/dp/CentreOfMass.py` & `wwpdb.utils.dp-0.46/wwpdb/utils/dp/CentreOfMass.py`

 * *Files identical despite different names*

### Comparing `wwpdb.utils.dp-0.45/wwpdb/utils/dp/DataFileAdapter.py` & `wwpdb.utils.dp-0.46/wwpdb/utils/dp/DataFileAdapter.py`

 * *Files identical despite different names*

### Comparing `wwpdb.utils.dp-0.45/wwpdb/utils/dp/DensityWrapper.py` & `wwpdb.utils.dp-0.46/wwpdb/utils/dp/DensityWrapper.py`

 * *Files identical despite different names*

### Comparing `wwpdb.utils.dp-0.45/wwpdb/utils/dp/DepositorSyncUtil.py` & `wwpdb.utils.dp-0.46/wwpdb/utils/dp/DepositorSyncUtil.py`

 * *Files identical despite different names*

### Comparing `wwpdb.utils.dp-0.45/wwpdb/utils/dp/PdbxChemShiftReport.py` & `wwpdb.utils.dp-0.46/wwpdb/utils/dp/PdbxChemShiftReport.py`

 * *Files identical despite different names*

### Comparing `wwpdb.utils.dp-0.45/wwpdb/utils/dp/PdbxMergeCategory.py` & `wwpdb.utils.dp-0.46/wwpdb/utils/dp/PdbxMergeCategory.py`

 * *Files identical despite different names*

### Comparing `wwpdb.utils.dp-0.45/wwpdb/utils/dp/PdbxSFMapCoefficients.py` & `wwpdb.utils.dp-0.46/wwpdb/utils/dp/PdbxSFMapCoefficients.py`

 * *Files identical despite different names*

### Comparing `wwpdb.utils.dp-0.45/wwpdb/utils/dp/PdbxStripCategory.py` & `wwpdb.utils.dp-0.46/wwpdb/utils/dp/PdbxStripCategory.py`

 * *Files identical despite different names*

### Comparing `wwpdb.utils.dp-0.45/wwpdb/utils/dp/RcsbDpUtility.py` & `wwpdb.utils.dp-0.46/wwpdb/utils/dp/RcsbDpUtility.py`

 * *Files 0% similar despite different names*

```diff
@@ -152,15 +152,15 @@
 try:
     from itertools import zip_longest
 except ImportError:
     from itertools import izip_longest as zip_longest
 
 from wwpdb.io.file.DataFile import DataFile
 from wwpdb.utils.config.ConfigInfo import ConfigInfo
-from wwpdb.utils.config.ConfigInfoApp import ConfigInfoAppEm, ConfigInfoAppCommon, ConfigInfoAppValidation
+from wwpdb.utils.config.ConfigInfoApp import ConfigInfoAppEm, ConfigInfoAppCommon, ConfigInfoAppValidation, ConfigInfoAppCc
 from wwpdb.utils.dp.PdbxStripCategory import PdbxStripCategory
 from wwpdb.utils.dp.RunRemote import RunRemote
 
 logger = logging.getLogger(__name__)
 
 
 class RcsbDpUtility(object):
@@ -362,14 +362,15 @@
             "em2em-spider",
             "fsc_check",
             "img-convert",
             "annot-read-map-header",
             "annot-read-map-header-in-place",
             "annot-update-map-header-in-place",
             "deposit-update-map-header-in-place",
+            "em-map-model-upload-check"
         ]
 
         #
 
         # Source, destination and logfile path details
         #
         self.__srcPath = None
@@ -384,14 +385,15 @@
         self.__numThreads = 1  # this is used by RunRemote to set the number of cores requested
         self.__startingMemory = 0  # this is used by RunRemote to set the starting RAM to be requested
 
         self.__run_remote = False
 
         self.__cI = ConfigInfo(self.__siteId)
         self.__cICommon = ConfigInfoAppCommon(self.__siteId)
+        self.__cIAppCc = ConfigInfoAppCc(self.__siteId)
         self.__cIVal = ConfigInfoAppValidation(self.__siteId)
         self.__initPath()
         self.__getRunRemote()
 
     def __getConfigPath(self, ky):
         try:
             pth = os.path.abspath(self.__cI.get(ky))
@@ -777,25 +779,27 @@
         #
         self.__annotAppsPath = self.__cICommon.get_site_annot_tools_path()
         self.__localAppsPath = self.__cICommon.get_site_local_apps_path()
         self.__packagePath = self.__cICommon.get_site_packages_path()
         self.__deployPath = self.__getConfigPath("SITE_DEPLOY_PATH")
         self.__sfvalidPath = self.__cICommon.get_sf_valid()
         self.__siteLoc = self.__cI.get("WWPDB_SITE_LOC")
+
         # self.__ccDictPath = self.__cICommon.get_site_cc_dict_path()
-        self.__ccCvsPath = self.__cICommon.get_site_cc_cvs_path()
-        self.__prdccCvsPath = self.__cICommon.get_site_prdcc_cvs_path()
-        self.__prdDictPath = self.__cICommon.get_site_prd_dict_path()
-        self.__prdSummarySerial = self.__cICommon.get_prd_summary_sdb()
+        self.__ccCvsPath = self.__cIAppCc.get_site_cc_cvs_path()
+        self.__prdccCvsPath = self.__cIAppCc.get_site_prdcc_cvs_path()
+        self.__prdDictPath = self.__cIAppCc.get_site_prd_dict_path()
+        self.__prdSummarySerial = self.__cIAppCc.get_prd_summary_sdb()
+        self.__ccDictPathIdx = self.__cIAppCc.get_cc_dict_idx()
+
         self.__oeDirPath = self.__cICommon.get_site_cc_oe_dir()
         self.__oeLicensePath = self.__cICommon.get_site_cc_oe_licence()
         self.__siteWebAppsSessionsPath = self.__cICommon.get_site_web_apps_sessions_path()
         self.__validScrPath = self.__cI.get("VALID_SCR_PATH")
         self.__siteConfigDir = self.__getConfigPath("TOP_WWPDB_SITE_CONFIG_DIR")
-        self.__ccDictPathIdx = self.__cICommon.get_cc_dict_idx()
         self.__pathPdbxDictSdb = self.__cICommon.get_mmcif_next_dictionary_sdb_file_path()
         self.__site_config_command = ". %s/init/env.sh -s %s -l %s" % (self.__siteConfigDir, self.__siteId, self.__siteLoc)
 
         # JDW 2013-02-26
         self.__rcsbAppsPath = self.__cICommon.get_site_annot_tools_path()
         #
         #
@@ -2885,17 +2889,17 @@
         #
         # Set application specific path details here -
         #
         self.__localAppsPath = self.__cICommon.get_site_local_apps_path()
         self.__packagePath = self.__cICommon.get_site_packages_path()
         self.__deployPath = self.__getConfigPath("SITE_DEPLOY_PATH")
         # self.__ccDictPath = self.__cICommon.get_site_cc_dict_path()
-        self.__ccCvsPath = self.__cICommon.get_site_cc_cvs_path()
-        self.__prdccCvsPath = self.__cICommon.get_site_prdcc_cvs_path()
-        self.__prdDictPath = self.__cICommon.get_site_prd_dict_path()
+        self.__ccCvsPath = self.__cIAppCc.get_site_cc_cvs_path()
+        self.__prdccCvsPath = self.__cIAppCc.get_site_prdcc_cvs_path()
+        self.__prdDictPath = self.__cIAppCc.get_site_prd_dict_path()
 
         self.__rcsbAppsPath = self.__cICommon.get_site_annot_tools_path()
         self.__pathPdbxDictSdb = self.__cICommon.get_mmcif_next_dictionary_sdb_file_path()
         #
         #
         iPath = self.__getSourceWrkFile(self.__stepNo)
         # iPathList = self.__getSourceWrkFileList(self.__stepNo)
@@ -3323,26 +3327,39 @@
             # any options ---
             if "options" in self.__inputParamDict:
                 argVal = str(self.__inputParamDict["options"]).strip()
                 cmd += " " + argVal
 
             cmd += " ; } 2> " + ePath + " 1> " + oPath
             cmd += " ; cat " + ePath + " > " + lPath
+        elif op == "em-map-model-upload-check":
+            inpMapFilePath = None
+            inpModelFilePath = None
+            outFilePath = None
+            if "input_map_file_path" in self.__inputParamDict:
+                inpMapFilePath = self.__inputParamDict["input_map_file_path"]
+            if "input_model_file_path" in self.__inputParamDict:
+                inpModelFilePath = self.__inputParamDict["input_model_file_path"]
+            if "output_file_path" in self.__inputParamDict:
+                outFilePath = self.__inputParamDict["output_file_path"]
+
+            cmd = f"python -m wwpdb.utils.emdb.atomcheck.atomcheck -m {inpMapFilePath} -d {inpModelFilePath} -o {outFilePath}"
         else:
             pass
 
         if op not in (
             "em2em-spider",
             "mapfix-big",
             "fsc_check",
             "img-convert",
             "annot-read-map-header",
             "annot-read-map-header-in-place",
             "annot-update-map-header-in-place",
             "deposit-update-map-header-in-place",
+            "em-map-model-upload-check"
         ):
             return -1
         #
 
         if self.__debug:
             logger.info("+RcsbDpUtility._emStep()  - Application string:\n%s\n", cmd)
 
@@ -3364,15 +3381,15 @@
     def __maxitStep(self, op, progName="maxit"):
         """Internal method that performs a single maxit operation."""
         # Set application specific path details --
         #
         # If this has not been initialized take if from the configuration class.
         if self.__rcsbAppsPath is None:
             self.__rcsbAppsPath = self.__cICommon.get_site_annot_tools_path()
-        self.__ccCvsPath = self.__cICommon.get_site_cc_cvs_path()
+        self.__ccCvsPath = self.__cIAppCc.get_site_cc_cvs_path()
         self.__pathPdbxDictSdb = self.__cICommon.get_mmcif_next_dictionary_sdb_file_path()
         #
         iPath = self.__getSourceWrkFile(self.__stepNo)
         # iPathList = self.__getSourceWrkFileList(self.__stepNo)
         oPath = self.__getResultWrkFile(self.__stepNo)
         lPath = self.__getLogWrkFile(self.__stepNo)
         ePath = self.__getErrWrkFile(self.__stepNo)
@@ -3502,20 +3519,20 @@
 
         #
         self.__ccAppsPath = self.__cICommon.get_site_cc_apps_path()
         self.__pdbxDictPath = self.__cICommon.get_mmcif_dict_path()
         self.__pdbxV4DictName = self.__cI.get("SITE_PDBX_V4_DICT_NAME", "missing")
 
         # self.__ccDictPath = self.__cICommon.get_site_cc_dict_path()
-        self.__ccCvsPath = self.__cICommon.get_site_cc_cvs_path()
+        self.__ccCvsPath = self.__cIAppCc.get_site_cc_cvs_path()
 
-        self.__patternPath = self.__cICommon.get_cc_fp_patterns()
+        self.__patternPath = self.__cIAppCc.get_cc_fp_patterns()
         # self.__ccDictPathCif = self.__cICommon.get_cc_dict()
-        self.__ccDictPathSdb = self.__cICommon.get_cc_dict_serial()
-        self.__ccDictPathIdx = self.__cICommon.get_cc_dict_idx()
+        self.__ccDictPathSdb = self.__cIAppCc.get_cc_dict_serial()
+        self.__ccDictPathIdx = self.__cIAppCc.get_cc_dict_idx()
         #
         self.__pathDdlSdb = os.path.join(self.__pdbxDictPath, "mmcif_ddl.sdb")
         # self.__pathDdl = os.path.join(self.__pdbxDictPath, "mmcif_ddl.dic")
         self.__pathPdbxDictSdb = self.__cICommon.get_mmcif_next_dictionary_sdb_file_path()
         self.__pathPdbxV4DictSdb = os.path.join(self.__pdbxDictPath, self.__pdbxV4DictName + ".sdb")
         self.__pathPdbxDictOdb = self.__cICommon.get_mmcif_next_dictionary_odb_file_path()
         #
```

### Comparing `wwpdb.utils.dp-0.45/wwpdb/utils/dp/RunRemote.py` & `wwpdb.utils.dp-0.46/wwpdb/utils/dp/RunRemote.py`

 * *Files identical despite different names*

### Comparing `wwpdb.utils.dp-0.45/wwpdb/utils/dp/ValidationWrapper.py` & `wwpdb.utils.dp-0.46/wwpdb/utils/dp/ValidationWrapper.py`

 * *Files identical despite different names*

### Comparing `wwpdb.utils.dp-0.45/wwpdb/utils/dp/electron_density/common_functions.py` & `wwpdb.utils.dp-0.46/wwpdb/utils/dp/electron_density/common_functions.py`

 * *Files identical despite different names*

### Comparing `wwpdb.utils.dp-0.45/wwpdb/utils/dp/electron_density/em_density_map.py` & `wwpdb.utils.dp-0.46/wwpdb/utils/dp/electron_density/em_density_map.py`

 * *Files identical despite different names*

### Comparing `wwpdb.utils.dp-0.45/wwpdb/utils/dp/electron_density/x_ray_density_map.py` & `wwpdb.utils.dp-0.46/wwpdb/utils/dp/electron_density/x_ray_density_map.py`

 * *Files identical despite different names*

### Comparing `wwpdb.utils.dp-0.45/wwpdb.utils.dp.egg-info/PKG-INFO` & `wwpdb.utils.dp-0.46/wwpdb.utils.dp.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: wwpdb.utils.dp
-Version: 0.45
+Version: 0.46
 Summary: API for Common Data Processing Operations
 Home-page: https://github.com/wwpdb/py-wwpdb_utils_dp
 Author: John Westbrook
 Author-email: john.westbrook@rcsb.org
 License: Apache 2.0
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
```

### Comparing `wwpdb.utils.dp-0.45/wwpdb.utils.dp.egg-info/SOURCES.txt` & `wwpdb.utils.dp-0.46/wwpdb.utils.dp.egg-info/SOURCES.txt`

 * *Files identical despite different names*

