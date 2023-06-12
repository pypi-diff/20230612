# Comparing `tmp/getmodelspec-1.0.363.tar.gz` & `tmp/getmodelspec-1.0.369.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist\getmodelspec-1.0.363.tar", last modified: Mon Jun 12 13:28:51 2023, max compression
+gzip compressed data, was "dist\getmodelspec-1.0.369.tar", last modified: Mon Jun 12 13:48:55 2023, max compression
```

## Comparing `getmodelspec-1.0.363.tar` & `getmodelspec-1.0.369.tar`

### file list

```diff
@@ -1,24 +1,24 @@
-drwxrwxrwx   0        0        0        0 2023-06-12 13:28:51.000000 getmodelspec-1.0.363/
--rw-rw-rw-   0        0        0      351 2023-06-12 13:28:51.000000 getmodelspec-1.0.363/PKG-INFO
--rw-rw-rw-   0        0        0     3896 2023-06-12 12:43:13.000000 getmodelspec-1.0.363/README.md
-drwxrwxrwx   0        0        0        0 2023-06-12 13:28:50.000000 getmodelspec-1.0.363/getmodelspec/
--rw-rw-rw-   0        0        0      253 2023-06-12 12:36:25.000000 getmodelspec-1.0.363/getmodelspec/__init__.py
--rw-rw-rw-   0        0        0      531 2023-06-11 16:18:57.000000 getmodelspec-1.0.363/getmodelspec/lineup.py
-drwxrwxrwx   0        0        0        0 2023-06-12 13:28:50.000000 getmodelspec-1.0.363/getmodelspec/src/
--rw-rw-rw-   0        0        0        0 2023-06-05 07:20:11.000000 getmodelspec-1.0.363/getmodelspec/src/__init__.py
--rw-rw-rw-   0        0        0    22455 2023-06-12 13:28:45.000000 getmodelspec-1.0.363/getmodelspec/src/sony.py
--rw-rw-rw-   0        0        0     1817 2023-06-12 11:30:21.000000 getmodelspec-1.0.363/getmodelspec/src/tv_score.py
--rw-rw-rw-   0        0        0     4277 2023-06-10 11:21:39.000000 getmodelspec-1.0.363/getmodelspec/src/tv_spepcifications.py
-drwxrwxrwx   0        0        0        0 2023-06-12 13:28:50.000000 getmodelspec-1.0.363/getmodelspec/tools/
--rw-rw-rw-   0        0        0        0 2023-06-05 07:20:04.000000 getmodelspec-1.0.363/getmodelspec/tools/__init__.py
--rw-rw-rw-   0        0        0     2042 2023-06-12 12:32:15.000000 getmodelspec-1.0.363/getmodelspec/tools/functions.py
--rw-rw-rw-   0        0        0     5038 2023-06-10 06:31:05.000000 getmodelspec-1.0.363/getmodelspec/tools/webdriver.py
-drwxrwxrwx   0        0        0        0 2023-06-12 13:28:50.000000 getmodelspec-1.0.363/getmodelspec.egg-info/
--rw-rw-rw-   0        0        0      351 2023-06-12 13:28:50.000000 getmodelspec-1.0.363/getmodelspec.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      501 2023-06-12 13:28:50.000000 getmodelspec-1.0.363/getmodelspec.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-06-12 13:28:50.000000 getmodelspec-1.0.363/getmodelspec.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       52 2023-06-12 13:28:50.000000 getmodelspec-1.0.363/getmodelspec.egg-info/entry_points.txt
--rw-rw-rw-   0        0        0       26 2023-06-12 13:28:50.000000 getmodelspec-1.0.363/getmodelspec.egg-info/requires.txt
--rw-rw-rw-   0        0        0       13 2023-06-12 13:28:50.000000 getmodelspec-1.0.363/getmodelspec.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-06-12 13:28:51.000000 getmodelspec-1.0.363/setup.cfg
--rw-rw-rw-   0        0        0      811 2023-06-12 13:28:45.000000 getmodelspec-1.0.363/setup.py
+drwxrwxrwx   0        0        0        0 2023-06-12 13:48:55.000000 getmodelspec-1.0.369/
+-rw-rw-rw-   0        0        0      351 2023-06-12 13:48:55.000000 getmodelspec-1.0.369/PKG-INFO
+-rw-rw-rw-   0        0        0     3796 2023-06-12 13:29:40.000000 getmodelspec-1.0.369/README.md
+drwxrwxrwx   0        0        0        0 2023-06-12 13:48:55.000000 getmodelspec-1.0.369/getmodelspec/
+-rw-rw-rw-   0        0        0      253 2023-06-12 12:36:25.000000 getmodelspec-1.0.369/getmodelspec/__init__.py
+-rw-rw-rw-   0        0        0      531 2023-06-11 16:18:57.000000 getmodelspec-1.0.369/getmodelspec/lineup.py
+drwxrwxrwx   0        0        0        0 2023-06-12 13:48:55.000000 getmodelspec-1.0.369/getmodelspec/src/
+-rw-rw-rw-   0        0        0        0 2023-06-05 07:20:11.000000 getmodelspec-1.0.369/getmodelspec/src/__init__.py
+-rw-rw-rw-   0        0        0    22421 2023-06-12 13:48:35.000000 getmodelspec-1.0.369/getmodelspec/src/sony.py
+-rw-rw-rw-   0        0        0     1817 2023-06-12 11:30:21.000000 getmodelspec-1.0.369/getmodelspec/src/tv_score.py
+-rw-rw-rw-   0        0        0     4277 2023-06-10 11:21:39.000000 getmodelspec-1.0.369/getmodelspec/src/tv_spepcifications.py
+drwxrwxrwx   0        0        0        0 2023-06-12 13:48:55.000000 getmodelspec-1.0.369/getmodelspec/tools/
+-rw-rw-rw-   0        0        0        0 2023-06-05 07:20:04.000000 getmodelspec-1.0.369/getmodelspec/tools/__init__.py
+-rw-rw-rw-   0        0        0     2042 2023-06-12 13:38:19.000000 getmodelspec-1.0.369/getmodelspec/tools/functions.py
+-rw-rw-rw-   0        0        0     5038 2023-06-10 06:31:05.000000 getmodelspec-1.0.369/getmodelspec/tools/webdriver.py
+drwxrwxrwx   0        0        0        0 2023-06-12 13:48:55.000000 getmodelspec-1.0.369/getmodelspec.egg-info/
+-rw-rw-rw-   0        0        0      351 2023-06-12 13:48:55.000000 getmodelspec-1.0.369/getmodelspec.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      501 2023-06-12 13:48:55.000000 getmodelspec-1.0.369/getmodelspec.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-06-12 13:48:55.000000 getmodelspec-1.0.369/getmodelspec.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       52 2023-06-12 13:48:55.000000 getmodelspec-1.0.369/getmodelspec.egg-info/entry_points.txt
+-rw-rw-rw-   0        0        0       26 2023-06-12 13:48:55.000000 getmodelspec-1.0.369/getmodelspec.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       13 2023-06-12 13:48:55.000000 getmodelspec-1.0.369/getmodelspec.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-06-12 13:48:55.000000 getmodelspec-1.0.369/setup.cfg
+-rw-rw-rw-   0        0        0      811 2023-06-12 13:48:48.000000 getmodelspec-1.0.369/setup.py
```

### Comparing `getmodelspec-1.0.363/README.md` & `getmodelspec-1.0.369/README.md`

 * *Files 7% similar despite different names*

```diff
@@ -1,8 +1,14 @@
 이 프로젝트는 웹사이트에서 제품 모델 사양을 가져오는 기능을 제공합니다.
+## 노트북 파일
+이 프로젝트는 다음과 같은 노트북 파일을 제공합니다:
+각 노트북 파일을 열어 자세한 사용법을 확인하세요
+- [제품 라인업 가져오기에 대한 Quick Guide](https://githubtocolab.com/xikest/Research-on-the-TV-market/blob/main/quick_guide_lineup.ipynb)
+- [제품 스코어 가져오기에 대한 Quick Guide](https://githubtocolab.com/xikest/Research-on-the-TV-market/blob/main/quick_guide_score.ipynb)
+- [제품 사양 가져오기에 대한 Quick Guide](https://githubtocolab.com/xikest/Research-on-the-TV-market/blob/main/quick_guide_specifications.ipynb)
 
 ## 설명
 이 프로젝트는 Selenium 라이브러리를 사용하여 웹사이트에서 제품 정보를 수집합니다. 
 디렉토리 생성, 페이지 로딩 대기, 데이터 백업 등과 같은 작업을 위한 여러 유틸리티 함수를 포함하고 있습니다. 
 또한, 웹 드라이버와 상호작용하기 위한 WebDriver 클래스와 웹사이트에서 제품 정보를 가져오는 LineUp 클래스가 포함되어 있습니다.
 
 ## 설치
@@ -52,21 +58,13 @@
 - src: 가져올 Sony 웹사이트의 소스를 지정합니다. "jp"를 선택하면 Sony 일본 사이트에서 제품 정보를 가져옵니다.
 - toExcel: 가져온 제품 정보를 Excel 파일로 저장할지 여부를 지정합니다. True로 설정하면 Excel 파일로 저장됩니다.
 
 ## 주의사항
 이 도구는 Selenium을 사용하여 웹 스크래핑을 수행하므로 Chrome 웹 드라이버가 필요합니다. Chrome 웹 드라이버를 설치하고 경로를 올바르게 설정해야 합니다.
 빠른 모드를 사용할 경우 일부 정보가 생략되므로 결과의 완전성을 확인하기 위해 정확성을 검토해야 합니다.
 
-## 노트북 파일
-프로젝트는 다음과 같은 노트북 파일을 제공합니다:
-각 노트북 파일을 열어 자세한 사용법을 확인하세요
-
-- [quick_guide_lineup.ipynb](https://githubtocolab.com/xikest/Research-on-the-TV-market/blob/main/quick_guide_lineup.ipynb): 제품 라인업 가져오기에 대한 빠른 가이드
-- [quick_guide_score.ipynb](https://githubtocolab.com/xikest/Research-on-the-TV-market/blob/main/quick_guide_score.ipynb): 제품 스코어 가져오기에 대한 빠른 가이드
-- [quick_guide_specifications.ipynb](https://githubtocolab.com/xikest/Research-on-the-TV-market/blob/main/quick_guide_specifications.ipynb): 제품 사양 가져오기에 대한 빠른 가이드
-
 ## 라이선스
 이 프로젝트는 MIT 라이선스를 따릅니다.
 
 ## 후원
 만약 이 프로젝트가 도움이 되었다면, 커피 한 잔의 후원은 큰 격려가 됩니다. ☕️
```

### Comparing `getmodelspec-1.0.363/getmodelspec/lineup.py` & `getmodelspec-1.0.369/getmodelspec/lineup.py`

 * *Files identical despite different names*

### Comparing `getmodelspec-1.0.363/getmodelspec/src/sony.py` & `getmodelspec-1.0.369/getmodelspec/src/sony.py`

 * *Files 1% similar despite different names*

```diff
@@ -78,15 +78,15 @@
                 print(f"fail to get info from {key}")
                 print(e)
                 pass
 
     # ======export====================================================================
         if self.toExcel == True:
             fileName = f"sony_LineUpGlobal_{date.today().strftime('%Y-%m-%d')}"
-            dictToexcel(dictModels, fileName=fileName,sheetName="Global", orient_col=False)  # 엑셀 파일로 저장
+            dictToexcel(dictModels, fileName=fileName,sheetName="Global")  # 엑셀 파일로 저장
 
         return dictModels
 
     ###=====================get info main page====================================##
     def __getUrlSeries__(self)-> set:
         """
         스크롤 다운이 되어야 전체 웹페이지가 로딩되어, 스크롤은 selenium, page parcing은 BS4로 진행
@@ -302,22 +302,22 @@
 
         ## 웹페이지의 모든 모델 url을 추출
         dictModels = {}
         for model, url in tqdm(setUrlSeries.items()):
             print(model,":", url)
             modelspec = self.__getSpec__(url=url)
             dictModels.update(modelspec)
-            backUp(dictModels, "dictModels_b")
+            # backUp(dictModels, "dictModels_b")
         print("Number of all Series:", len(dictModels))
         print(dictModels)
         # backUp(dictModels, "dictModels")
     # ======export====================================================================
         if self.toExcel == True:
             fileName = f"sonyJp_LineUp_{date.today().strftime('%Y-%m-%d')}"
-            dictToexcel(dictModels, fileName=fileName,sheetName="Jp", orient_col=False)  # 엑셀 파일로 저장
+            dictToexcel(dictModels, fileName=fileName,sheetName="Jp")  # 엑셀 파일로 저장
 
         return dictModels
 
 
     ###=====================get info main page====================================##
     def __getSpecSeries__(self, url: str = "https://www.sony.jp/bravia/gallery/") -> dict:
         """
```

### Comparing `getmodelspec-1.0.363/getmodelspec/src/tv_score.py` & `getmodelspec-1.0.369/getmodelspec/src/tv_score.py`

 * *Files identical despite different names*

### Comparing `getmodelspec-1.0.363/getmodelspec/src/tv_spepcifications.py` & `getmodelspec-1.0.369/getmodelspec/src/tv_spepcifications.py`

 * *Files identical despite different names*

### Comparing `getmodelspec-1.0.363/getmodelspec/tools/functions.py` & `getmodelspec-1.0.369/getmodelspec/tools/functions.py`

 * *Files 5% similar despite different names*

```diff
@@ -54,15 +54,15 @@
     """
     마지막 / 이후 문자만 가져 옴
     """
     return url.rsplit('/', 1)[-1]
 
 
 
-def dictToexcel(dictData, fileName="dictToExcel", sheetName="sheet1", orient_col=True):
-    if orient_col == True: orient = 'columns'
-    else: orient = 'index'
+def dictToexcel(dictData, fileName="dictToExcel", sheetName="sheet1", orient_idx=True):
+    if orient_idx == True: orient = 'index'
+    else: orient = 'columns'
     df = pd.DataFrame.from_dict(dictData, orient=orient)
     # Create a Pandas Excel writer
     df.to_excel(f"{fileName}"+".xlsx", sheet_name=sheetName, index=True)
     return None
```

### Comparing `getmodelspec-1.0.363/getmodelspec/tools/webdriver.py` & `getmodelspec-1.0.369/getmodelspec/tools/webdriver.py`

 * *Files identical despite different names*

### Comparing `getmodelspec-1.0.363/setup.py` & `getmodelspec-1.0.369/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from setuptools import setup, find_packages
 
 setup(
     name='getmodelspec',
-    version='1.0.363',
+    version='1.0.369',
     author='xikest',
     description='get model spec,',
     packages=find_packages(),
     python_requires='>=3.7',
     install_requires=[
         'numpy',
         'pandas',
```

