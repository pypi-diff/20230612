# Comparing `tmp/getmodelspec-1.0.351.tar.gz` & `tmp/getmodelspec-1.0.36.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist\getmodelspec-1.0.351.tar", last modified: Mon Jun 12 11:33:48 2023, max compression
+gzip compressed data, was "dist\getmodelspec-1.0.36.tar", last modified: Mon Jun 12 12:26:04 2023, max compression
```

## Comparing `getmodelspec-1.0.351.tar` & `getmodelspec-1.0.36.tar`

### file list

```diff
@@ -1,25 +1,25 @@
-drwxrwxrwx   0        0        0        0 2023-06-12 11:33:48.000000 getmodelspec-1.0.351/
--rw-rw-rw-   0        0        0      351 2023-06-12 11:33:48.000000 getmodelspec-1.0.351/PKG-INFO
--rw-rw-rw-   0        0        0     1253 2023-06-11 16:27:14.000000 getmodelspec-1.0.351/README.md
-drwxrwxrwx   0        0        0        0 2023-06-12 11:33:48.000000 getmodelspec-1.0.351/getmodelspec/
--rw-rw-rw-   0        0        0      199 2023-06-11 12:04:13.000000 getmodelspec-1.0.351/getmodelspec/__init__.py
--rw-rw-rw-   0        0        0      531 2023-06-11 16:18:57.000000 getmodelspec-1.0.351/getmodelspec/lineup.py
-drwxrwxrwx   0        0        0        0 2023-06-12 11:33:48.000000 getmodelspec-1.0.351/getmodelspec/src/
--rw-rw-rw-   0        0        0        0 2023-06-05 07:20:11.000000 getmodelspec-1.0.351/getmodelspec/src/__init__.py
--rw-rw-rw-   0        0        0    22547 2023-06-12 11:33:32.000000 getmodelspec-1.0.351/getmodelspec/src/sony.py
--rw-rw-rw-   0        0        0     1817 2023-06-12 11:30:21.000000 getmodelspec-1.0.351/getmodelspec/src/tv_score.py
--rw-rw-rw-   0        0        0     4277 2023-06-10 11:21:39.000000 getmodelspec-1.0.351/getmodelspec/src/tv_spepcifications.py
-drwxrwxrwx   0        0        0        0 2023-06-12 11:33:48.000000 getmodelspec-1.0.351/getmodelspec/tools/
--rw-rw-rw-   0        0        0        0 2023-06-05 07:20:04.000000 getmodelspec-1.0.351/getmodelspec/tools/__init__.py
--rw-rw-rw-   0        0        0     2000 2023-06-11 15:37:20.000000 getmodelspec-1.0.351/getmodelspec/tools/functions.py
--rw-rw-rw-   0        0        0     2823 2023-06-12 10:09:49.000000 getmodelspec-1.0.351/getmodelspec/tools/translate.py
--rw-rw-rw-   0        0        0     5038 2023-06-10 06:31:05.000000 getmodelspec-1.0.351/getmodelspec/tools/webdriver.py
-drwxrwxrwx   0        0        0        0 2023-06-12 11:33:48.000000 getmodelspec-1.0.351/getmodelspec.egg-info/
--rw-rw-rw-   0        0        0      351 2023-06-12 11:33:47.000000 getmodelspec-1.0.351/getmodelspec.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      533 2023-06-12 11:33:48.000000 getmodelspec-1.0.351/getmodelspec.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-06-12 11:33:47.000000 getmodelspec-1.0.351/getmodelspec.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       52 2023-06-12 11:33:47.000000 getmodelspec-1.0.351/getmodelspec.egg-info/entry_points.txt
--rw-rw-rw-   0        0        0       26 2023-06-12 11:33:47.000000 getmodelspec-1.0.351/getmodelspec.egg-info/requires.txt
--rw-rw-rw-   0        0        0       13 2023-06-12 11:33:47.000000 getmodelspec-1.0.351/getmodelspec.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-06-12 11:33:48.000000 getmodelspec-1.0.351/setup.cfg
--rw-rw-rw-   0        0        0      811 2023-06-12 11:33:38.000000 getmodelspec-1.0.351/setup.py
+drwxrwxrwx   0        0        0        0 2023-06-12 12:26:04.000000 getmodelspec-1.0.36/
+-rw-rw-rw-   0        0        0      350 2023-06-12 12:26:04.000000 getmodelspec-1.0.36/PKG-INFO
+-rw-rw-rw-   0        0        0     1253 2023-06-11 16:27:14.000000 getmodelspec-1.0.36/README.md
+drwxrwxrwx   0        0        0        0 2023-06-12 12:26:04.000000 getmodelspec-1.0.36/getmodelspec/
+-rw-rw-rw-   0        0        0      199 2023-06-11 12:04:13.000000 getmodelspec-1.0.36/getmodelspec/__init__.py
+-rw-rw-rw-   0        0        0      531 2023-06-11 16:18:57.000000 getmodelspec-1.0.36/getmodelspec/lineup.py
+drwxrwxrwx   0        0        0        0 2023-06-12 12:26:04.000000 getmodelspec-1.0.36/getmodelspec/src/
+-rw-rw-rw-   0        0        0        0 2023-06-05 07:20:11.000000 getmodelspec-1.0.36/getmodelspec/src/__init__.py
+-rw-rw-rw-   0        0        0    22408 2023-06-12 12:25:33.000000 getmodelspec-1.0.36/getmodelspec/src/sony.py
+-rw-rw-rw-   0        0        0     1817 2023-06-12 11:30:21.000000 getmodelspec-1.0.36/getmodelspec/src/tv_score.py
+-rw-rw-rw-   0        0        0     4277 2023-06-10 11:21:39.000000 getmodelspec-1.0.36/getmodelspec/src/tv_spepcifications.py
+drwxrwxrwx   0        0        0        0 2023-06-12 12:26:04.000000 getmodelspec-1.0.36/getmodelspec/tools/
+-rw-rw-rw-   0        0        0        0 2023-06-05 07:20:04.000000 getmodelspec-1.0.36/getmodelspec/tools/__init__.py
+-rw-rw-rw-   0        0        0     2000 2023-06-11 15:37:20.000000 getmodelspec-1.0.36/getmodelspec/tools/functions.py
+-rw-rw-rw-   0        0        0     2823 2023-06-12 10:09:49.000000 getmodelspec-1.0.36/getmodelspec/tools/translate.py
+-rw-rw-rw-   0        0        0     5038 2023-06-10 06:31:05.000000 getmodelspec-1.0.36/getmodelspec/tools/webdriver.py
+drwxrwxrwx   0        0        0        0 2023-06-12 12:26:04.000000 getmodelspec-1.0.36/getmodelspec.egg-info/
+-rw-rw-rw-   0        0        0      350 2023-06-12 12:26:03.000000 getmodelspec-1.0.36/getmodelspec.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      533 2023-06-12 12:26:03.000000 getmodelspec-1.0.36/getmodelspec.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-06-12 12:26:03.000000 getmodelspec-1.0.36/getmodelspec.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       52 2023-06-12 12:26:03.000000 getmodelspec-1.0.36/getmodelspec.egg-info/entry_points.txt
+-rw-rw-rw-   0        0        0       26 2023-06-12 12:26:03.000000 getmodelspec-1.0.36/getmodelspec.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       13 2023-06-12 12:26:03.000000 getmodelspec-1.0.36/getmodelspec.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-06-12 12:26:04.000000 getmodelspec-1.0.36/setup.cfg
+-rw-rw-rw-   0        0        0      810 2023-06-12 12:25:53.000000 getmodelspec-1.0.36/setup.py
```

### Comparing `getmodelspec-1.0.351/README.md` & `getmodelspec-1.0.36/README.md`

 * *Files identical despite different names*

### Comparing `getmodelspec-1.0.351/getmodelspec/lineup.py` & `getmodelspec-1.0.36/getmodelspec/lineup.py`

 * *Files identical despite different names*

### Comparing `getmodelspec-1.0.351/getmodelspec/src/sony.py` & `getmodelspec-1.0.36/getmodelspec/src/sony.py`

 * *Files 2% similar despite different names*

```diff
@@ -14,24 +14,24 @@
 from getmodelspec.src.tv_score import Score
 from getmodelspec.tools.functions import *
 from getmodelspec.tools.webdriver import WebDriver
 
 
 
 class GetSONY:
-    def __init__(self, fastMode=True, srcfromOfficial=True, toExcel=True):
+    def __init__(self, fastMode=True, srcfromGlobal=True, toExcel=True):
         self.waitTime = 10
         self.fastMode = fastMode
-        self.srcfromOfficial = srcfromOfficial
+        self.srcfromGlobal = srcfromGlobal
         self.toExcel = toExcel
         self.dir_3rd = "sony/log/models"
         makeDir(self.dir_3rd)
         pass
 
-    def getModels(self, toExcel:bool = True) -> pd.DataFrame:
+    def getModels(self, toExcel:bool = True) -> dict:
         # 메인 페이지에서 시리즈를 추출
         setUrlSeries = self.__getUrlSeries__()
         print(setUrlSeries)
         ==========================================================================
         # backUp(setUrlSeries, "setUrlSeries")
         # with open(f"setUrlSeries.pickle", "rb") as file:
         #     setUrlSeries = pickle.load(file)
@@ -57,15 +57,15 @@
             try:
                 dictInfo = self.__getModelInfo__(urlModel)
                 time.sleep(1)
                 dictModels[key] = dictInfo
                 model = dictInfo.get('model')
 
                 if self.fastMode == False:
-                    if self.srcfromOfficial == True:
+                    if self.srcfromGlobal == True:
                         dictSpec = self.__getSpecGlobal__(url=urlModel)
                         dictModels[key].update(dictSpec)
                     else:
                         print("global")
                         dictSpec = self.__getSpec__(maker="sony", model=model)
                         dictModels[key].update(dictSpec)
 
@@ -76,23 +76,19 @@
                 dictModels[key].update(dictScore)
             except Exception as e:
                 print(f"fail to get info from {key}")
                 print(e)
                 pass
 
     # ======export====================================================================
-        dfModels = pd.DataFrame.from_dict(dictModels, orient="index")
-        # dfModels = dfModels.rename_axis('model').reset_index()
-
-
         if self.toExcel == True:
-            fileName = f"sony_TV_series_{date.today().strftime('%Y-%m-%d')}"
-            dfModels.to_excel(fileName, index=False)  # 엑셀 파일로 저장
+            fileName = f"sony_LineUpGlobal_{date.today().strftime('%Y-%m-%d')}"
+            dictToexcel(dictModels, fileName=fileName, orient_col=False)  # 엑셀 파일로 저장
 
-        return dfModels
+        return dictModels
 
     ###=====================get info main page====================================##
     def __getUrlSeries__(self)-> set:
         """
         스크롤 다운이 되어야 전체 웹페이지가 로딩되어, 스크롤은 selenium, page parcing은 BS4로 진행
         """
         url: str = "https://electronics.sony.com/tv-video/televisions/c/all-tvs/"
@@ -289,15 +285,15 @@
 class GetSONYjp:
     def __init__(self, fastMode=True,  toExcel=True):
         self.waitTime = 10
         self.fastMode = fastMode
         self.toExcel = toExcel
         pass
 
-    def getModels(self, toExcel:bool = True) -> pd.DataFrame:
+    def getModels(self, toExcel:bool = True) -> dict:
         self.toExcel=toExcel
         # 메인 페이지에서 시리즈를 추출
         setUrlSeries = self.__getSpecSeries__()
         print(setUrlSeries)
         # ==========================================================================
         # backUp(setUrlSeries, "setUrlSeries")
         # with open(f"setUrlSeries.pickle", "rb") as file:
@@ -312,19 +308,20 @@
             dictModels.update(modelspec)
             backUp(dictModels, "dictModels_b")
         print("Number of all Series:", len(dictModels))
         print(dictModels)
         # backUp(dictModels, "dictModels")
     # ======export====================================================================
         if self.toExcel == True:
-            fileName = f"sony_TV_series_{date.today().strftime('%Y-%m-%d')}"
+            fileName = f"sonyJp_LineUp_{date.today().strftime('%Y-%m-%d')}"
             dictToexcel(dictModels, fileName=fileName, orient_col=False)  # 엑셀 파일로 저장
 
         return dictModels
 
+
     ###=====================get info main page====================================##
     def __getSpecSeries__(self, url: str = "https://www.sony.jp/bravia/gallery/") -> dict:
         """
         스크롤 다운이 되어야 전체 웹페이지가 로딩되어, 스크롤은 selenium, page parcing은 BS4로 진행
         """
         step: int = 200
         dictSeries = {}
```

### Comparing `getmodelspec-1.0.351/getmodelspec/src/tv_score.py` & `getmodelspec-1.0.36/getmodelspec/src/tv_score.py`

 * *Files identical despite different names*

### Comparing `getmodelspec-1.0.351/getmodelspec/src/tv_spepcifications.py` & `getmodelspec-1.0.36/getmodelspec/src/tv_spepcifications.py`

 * *Files identical despite different names*

### Comparing `getmodelspec-1.0.351/getmodelspec/tools/functions.py` & `getmodelspec-1.0.36/getmodelspec/tools/functions.py`

 * *Files identical despite different names*

### Comparing `getmodelspec-1.0.351/getmodelspec/tools/translate.py` & `getmodelspec-1.0.36/getmodelspec/tools/translate.py`

 * *Files identical despite different names*

### Comparing `getmodelspec-1.0.351/getmodelspec/tools/webdriver.py` & `getmodelspec-1.0.36/getmodelspec/tools/webdriver.py`

 * *Files identical despite different names*

### Comparing `getmodelspec-1.0.351/getmodelspec.egg-info/SOURCES.txt` & `getmodelspec-1.0.36/getmodelspec.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `getmodelspec-1.0.351/setup.py` & `getmodelspec-1.0.36/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from setuptools import setup, find_packages
 
 setup(
     name='getmodelspec',
-    version='1.0.351',
+    version='1.0.36',
     author='xikest',
     description='get model spec,',
     packages=find_packages(),
     python_requires='>=3.7',
     install_requires=[
         'numpy',
         'pandas',
```

