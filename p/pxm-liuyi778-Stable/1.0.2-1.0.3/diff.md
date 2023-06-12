# Comparing `tmp/pxm_liuyi778_stable-1.0.2.tar.gz` & `tmp/pxm_liuyi778_stable-1.0.3.tar.gz`

## Comparing `pxm_liuyi778_stable-1.0.2.tar` & `pxm_liuyi778_stable-1.0.3.tar`

### file list

```diff
@@ -1,27 +1,27 @@
--rw-r--r--   0        0        0     1544 2020-02-02 00:00:00.000000 pxm_liuyi778_stable-1.0.2/DemoRead.py
--rw-r--r--   0        0        0     1336 2020-02-02 00:00:00.000000 pxm_liuyi778_stable-1.0.2/DemoWrite.py
--rw-r--r--   0        0        0     3115 2020-02-02 00:00:00.000000 pxm_liuyi778_stable-1.0.2/UploadToPypi.py
--rw-r--r--   0        0        0       69 2020-02-02 00:00:00.000000 pxm_liuyi778_stable-1.0.2/req.py
--rw-r--r--   0        0        0       35 2020-02-02 00:00:00.000000 pxm_liuyi778_stable-1.0.2/requirements.txt
--rw-r--r--   0        0        0       50 2020-02-02 00:00:00.000000 pxm_liuyi778_stable-1.0.2/.idea/.gitignore
--rw-r--r--   0        0        0      189 2020-02-02 00:00:00.000000 pxm_liuyi778_stable-1.0.2/.idea/misc.xml
--rw-r--r--   0        0        0      265 2020-02-02 00:00:00.000000 pxm_liuyi778_stable-1.0.2/.idea/modules.xml
--rw-r--r--   0        0        0      440 2020-02-02 00:00:00.000000 pxm_liuyi778_stable-1.0.2/.idea/pxm.iml
--rw-r--r--   0        0        0      185 2020-02-02 00:00:00.000000 pxm_liuyi778_stable-1.0.2/.idea/vcs.xml
--rw-r--r--   0        0        0    10643 2020-02-02 00:00:00.000000 pxm_liuyi778_stable-1.0.2/.idea/workspace.xml
--rw-r--r--   0        0        0     8474 2020-02-02 00:00:00.000000 pxm_liuyi778_stable-1.0.2/.idea/inspectionProfiles/Project_Default.xml
--rw-r--r--   0        0        0      179 2020-02-02 00:00:00.000000 pxm_liuyi778_stable-1.0.2/.idea/inspectionProfiles/profiles_settings.xml
--rw-r--r--   0        0        0      340 2020-02-02 00:00:00.000000 pxm_liuyi778_stable-1.0.2/src/pxm_liuyi778_Stable/__init__.py
--rw-r--r--   0        0        0      349 2020-02-02 00:00:00.000000 pxm_liuyi778_stable-1.0.2/src/pxm_liuyi778_Stable/dic.py
--rw-r--r--   0        0        0      702 2020-02-02 00:00:00.000000 pxm_liuyi778_stable-1.0.2/src/pxm_liuyi778_Stable/exists.py
--rw-r--r--   0        0        0      413 2020-02-02 00:00:00.000000 pxm_liuyi778_stable-1.0.2/src/pxm_liuyi778_Stable/pxm.py
--rw-r--r--   0        0        0     7814 2020-02-02 00:00:00.000000 pxm_liuyi778_stable-1.0.2/src/pxm_liuyi778_Stable/read.py
--rw-r--r--   0        0        0     4036 2020-02-02 00:00:00.000000 pxm_liuyi778_stable-1.0.2/src/pxm_liuyi778_Stable/write.py
--rw-r--r--   0        0        0      204 2020-02-02 00:00:00.000000 pxm_liuyi778_stable-1.0.2/src/tests/read.py
--rw-r--r--   0        0        0    10310 2020-02-02 00:00:00.000000 pxm_liuyi778_stable-1.0.2/xls/demo.xlsx
--rw-r--r--   0        0        0     4841 2020-02-02 00:00:00.000000 pxm_liuyi778_stable-1.0.2/xls/demoW.xlsx
--rw-r--r--   0        0        0     2174 2020-02-02 00:00:00.000000 pxm_liuyi778_stable-1.0.2/.gitignore
--rw-r--r--   0        0        0    11558 2020-02-02 00:00:00.000000 pxm_liuyi778_stable-1.0.2/LICENSE
--rw-r--r--   0        0        0     3023 2020-02-02 00:00:00.000000 pxm_liuyi778_stable-1.0.2/README.md
--rw-r--r--   0        0        0      666 2020-02-02 00:00:00.000000 pxm_liuyi778_stable-1.0.2/pyproject.toml
--rw-r--r--   0        0        0     3504 2020-02-02 00:00:00.000000 pxm_liuyi778_stable-1.0.2/PKG-INFO
+-rw-r--r--   0        0        0     1544 2020-02-02 00:00:00.000000 pxm_liuyi778_stable-1.0.3/DemoRead.py
+-rw-r--r--   0        0        0     1336 2020-02-02 00:00:00.000000 pxm_liuyi778_stable-1.0.3/DemoWrite.py
+-rw-r--r--   0        0        0     3115 2020-02-02 00:00:00.000000 pxm_liuyi778_stable-1.0.3/UploadToPypi.py
+-rw-r--r--   0        0        0       69 2020-02-02 00:00:00.000000 pxm_liuyi778_stable-1.0.3/req.py
+-rw-r--r--   0        0        0       35 2020-02-02 00:00:00.000000 pxm_liuyi778_stable-1.0.3/requirements.txt
+-rw-r--r--   0        0        0       50 2020-02-02 00:00:00.000000 pxm_liuyi778_stable-1.0.3/.idea/.gitignore
+-rw-r--r--   0        0        0      189 2020-02-02 00:00:00.000000 pxm_liuyi778_stable-1.0.3/.idea/misc.xml
+-rw-r--r--   0        0        0      265 2020-02-02 00:00:00.000000 pxm_liuyi778_stable-1.0.3/.idea/modules.xml
+-rw-r--r--   0        0        0      440 2020-02-02 00:00:00.000000 pxm_liuyi778_stable-1.0.3/.idea/pxm.iml
+-rw-r--r--   0        0        0      185 2020-02-02 00:00:00.000000 pxm_liuyi778_stable-1.0.3/.idea/vcs.xml
+-rw-r--r--   0        0        0    11008 2020-02-02 00:00:00.000000 pxm_liuyi778_stable-1.0.3/.idea/workspace.xml
+-rw-r--r--   0        0        0     8474 2020-02-02 00:00:00.000000 pxm_liuyi778_stable-1.0.3/.idea/inspectionProfiles/Project_Default.xml
+-rw-r--r--   0        0        0      179 2020-02-02 00:00:00.000000 pxm_liuyi778_stable-1.0.3/.idea/inspectionProfiles/profiles_settings.xml
+-rw-r--r--   0        0        0      340 2020-02-02 00:00:00.000000 pxm_liuyi778_stable-1.0.3/src/pxm_liuyi778_Stable/__init__.py
+-rw-r--r--   0        0        0      349 2020-02-02 00:00:00.000000 pxm_liuyi778_stable-1.0.3/src/pxm_liuyi778_Stable/dic.py
+-rw-r--r--   0        0        0      702 2020-02-02 00:00:00.000000 pxm_liuyi778_stable-1.0.3/src/pxm_liuyi778_Stable/exists.py
+-rw-r--r--   0        0        0      367 2020-02-02 00:00:00.000000 pxm_liuyi778_stable-1.0.3/src/pxm_liuyi778_Stable/pxm.py
+-rw-r--r--   0        0        0     7768 2020-02-02 00:00:00.000000 pxm_liuyi778_stable-1.0.3/src/pxm_liuyi778_Stable/read.py
+-rw-r--r--   0        0        0     4013 2020-02-02 00:00:00.000000 pxm_liuyi778_stable-1.0.3/src/pxm_liuyi778_Stable/write.py
+-rw-r--r--   0        0        0      204 2020-02-02 00:00:00.000000 pxm_liuyi778_stable-1.0.3/src/tests/read.py
+-rw-r--r--   0        0        0    10310 2020-02-02 00:00:00.000000 pxm_liuyi778_stable-1.0.3/xls/demo.xlsx
+-rw-r--r--   0        0        0     4841 2020-02-02 00:00:00.000000 pxm_liuyi778_stable-1.0.3/xls/demoW.xlsx
+-rw-r--r--   0        0        0     2174 2020-02-02 00:00:00.000000 pxm_liuyi778_stable-1.0.3/.gitignore
+-rw-r--r--   0        0        0    11558 2020-02-02 00:00:00.000000 pxm_liuyi778_stable-1.0.3/LICENSE
+-rw-r--r--   0        0        0     3023 2020-02-02 00:00:00.000000 pxm_liuyi778_stable-1.0.3/README.md
+-rw-r--r--   0        0        0      666 2020-02-02 00:00:00.000000 pxm_liuyi778_stable-1.0.3/pyproject.toml
+-rw-r--r--   0        0        0     3504 2020-02-02 00:00:00.000000 pxm_liuyi778_stable-1.0.3/PKG-INFO
```

### Comparing `pxm_liuyi778_stable-1.0.2/DemoRead.py` & `pxm_liuyi778_stable-1.0.3/DemoRead.py`

 * *Files identical despite different names*

### Comparing `pxm_liuyi778_stable-1.0.2/DemoWrite.py` & `pxm_liuyi778_stable-1.0.3/DemoWrite.py`

 * *Files identical despite different names*

### Comparing `pxm_liuyi778_stable-1.0.2/UploadToPypi.py` & `pxm_liuyi778_stable-1.0.3/UploadToPypi.py`

 * *Files identical despite different names*

### Comparing `pxm_liuyi778_stable-1.0.2/.idea/workspace.xml` & `pxm_liuyi778_stable-1.0.3/.idea/workspace.xml`

 * *Files 2% similar despite different names*

#### Comparing `pxm_liuyi778_stable-1.0.2/.idea/workspace.xml` & `pxm_liuyi778_stable-1.0.3/.idea/workspace.xml`

```diff
@@ -134,14 +134,15 @@
       <changelist id="d41c57d7-f66c-4f3e-b27b-fe814c0a247d" name="变更" comment=""/>
       <created>1677834630850</created>
       <option name="number" value="Default"/>
       <option name="presentableId" value="Default"/>
       <updated>1677834630850</updated>
       <workItem from="1686534393051" duration="1884000"/>
       <workItem from="1686536307862" duration="1345000"/>
+      <workItem from="1686537768322" duration="371000"/>
     </task>
     <task id="LOCAL-00001" summary="更新日志">
       <created>1679642216056</created>
       <option name="number" value="00001"/>
       <option name="presentableId" value="LOCAL-00001"/>
       <option name="project" value="LOCAL"/>
       <updated>1679642216056</updated>
@@ -177,15 +178,22 @@
     <task id="LOCAL-00006" summary="完成自动化安装">
       <created>1686537085850</created>
       <option name="number" value="00006"/>
       <option name="presentableId" value="LOCAL-00006"/>
       <option name="project" value="LOCAL"/>
       <updated>1686537085850</updated>
     </task>
-    <option name="localTasksCounter" value="7"/>
+    <task id="LOCAL-00007" summary="完成自动化安装">
+      <created>1686537866526</created>
+      <option name="number" value="00007"/>
+      <option name="presentableId" value="LOCAL-00007"/>
+      <option name="project" value="LOCAL"/>
+      <updated>1686537866526</updated>
+    </task>
+    <option name="localTasksCounter" value="8"/>
     <servers/>
   </component>
   <component name="TypeScriptGeneratedFilesManager">
     <option name="version" value="3"/>
   </component>
   <component name="Vcs.Log.Tabs.Properties">
     <option name="TAB_STATES">
@@ -202,11 +210,11 @@
     <MESSAGE value="更新日志"/>
     <MESSAGE value="使用新标准上传"/>
     <MESSAGE value="完成自动化安装"/>
     <option name="LAST_COMMIT_MESSAGE" value="完成自动化安装"/>
   </component>
   <component name="com.intellij.coverage.CoverageDataManagerImpl">
     <SUITE FILE_PATH="coverage/pxm$req.coverage" NAME="req 覆盖结果" MODIFIED="1686536122567" SOURCE_PROVIDER="com.intellij.coverage.DefaultCoverageFileProvider" RUNNER="coverage.py" COVERAGE_BY_TEST_ENABLED="true" COVERAGE_TRACING_ENABLED="false" WORKING_DIRECTORY="$PROJECT_DIR$"/>
-    <SUITE FILE_PATH="coverage/pxm$UploadToPypi.coverage" NAME="UploadToPypi 覆盖结果" MODIFIED="1686537025387" SOURCE_PROVIDER="com.intellij.coverage.DefaultCoverageFileProvider" RUNNER="coverage.py" COVERAGE_BY_TEST_ENABLED="true" COVERAGE_TRACING_ENABLED="false" WORKING_DIRECTORY="$PROJECT_DIR$"/>
+    <SUITE FILE_PATH="coverage/pxm$UploadToPypi.coverage" NAME="UploadToPypi 覆盖结果" MODIFIED="1686537827673" SOURCE_PROVIDER="com.intellij.coverage.DefaultCoverageFileProvider" RUNNER="coverage.py" COVERAGE_BY_TEST_ENABLED="true" COVERAGE_TRACING_ENABLED="false" WORKING_DIRECTORY="$PROJECT_DIR$"/>
     <SUITE FILE_PATH="coverage/pxm$.coverage" NAME=" 覆盖结果" MODIFIED="1686536236197" SOURCE_PROVIDER="com.intellij.coverage.DefaultCoverageFileProvider" RUNNER="coverage.py" COVERAGE_BY_TEST_ENABLED="true" COVERAGE_TRACING_ENABLED="false" WORKING_DIRECTORY="$PROJECT_DIR$/src/tests"/>
   </component>
 </project>
```

### Comparing `pxm_liuyi778_stable-1.0.2/.idea/inspectionProfiles/Project_Default.xml` & `pxm_liuyi778_stable-1.0.3/.idea/inspectionProfiles/Project_Default.xml`

 * *Files identical despite different names*

### Comparing `pxm_liuyi778_stable-1.0.2/src/pxm_liuyi778_Stable/exists.py` & `pxm_liuyi778_stable-1.0.3/src/pxm_liuyi778_Stable/exists.py`

 * *Files identical despite different names*

### Comparing `pxm_liuyi778_stable-1.0.2/src/pxm_liuyi778_Stable/read.py` & `pxm_liuyi778_stable-1.0.3/src/pxm_liuyi778_Stable/read.py`

 * *Files 2% similar despite different names*

```diff
@@ -7,16 +7,16 @@
 @Contact :   faith01238@hotmail.com
 @Homepage : https://liumou.site
 @Desc    :   使用Openpyxl模块实现的读取功能
 """
 from openpyxl import load_workbook
 from ColorInfo import ColorLogger
 from sys import exit
-from src.pxm_liuyi778_Stable.exists import _exists
-from src.pxm_liuyi778_Stable.dic import GetDic
+from .exists import _exists
+from .dic import GetDic
 
 
 class Read:
 	def __init__(self, filename):
 		"""
 		读取表格数据
 		:param filename: 需要读取的表格文件
```

### Comparing `pxm_liuyi778_stable-1.0.2/src/pxm_liuyi778_Stable/write.py` & `pxm_liuyi778_stable-1.0.3/src/pxm_liuyi778_Stable/write.py`

 * *Files 1% similar despite different names*

```diff
@@ -7,15 +7,15 @@
 @Contact :   faith01238@hotmail.com
 @Homepage : https://liumou.site
 @Desc    :   使用Openpyxl模块实现的写入功能
 """
 from ColorInfo import ColorLogger
 from openpyxl import Workbook, load_workbook
 
-from src.pxm_liuyi778_Stable.exists import _exists
+from .exists import _exists
 
 
 class Write:
 	def __init__(self, filename):
 		"""
 		写入表格数据
 		:param filename: 需要写入的表格文件
```

### Comparing `pxm_liuyi778_stable-1.0.2/xls/demo.xlsx` & `pxm_liuyi778_stable-1.0.3/xls/demo.xlsx`

 * *Files identical despite different names*

### Comparing `pxm_liuyi778_stable-1.0.2/xls/demoW.xlsx` & `pxm_liuyi778_stable-1.0.3/xls/demoW.xlsx`

 * *Files identical despite different names*

### Comparing `pxm_liuyi778_stable-1.0.2/.gitignore` & `pxm_liuyi778_stable-1.0.3/.gitignore`

 * *Files identical despite different names*

### Comparing `pxm_liuyi778_stable-1.0.2/LICENSE` & `pxm_liuyi778_stable-1.0.3/LICENSE`

 * *Files identical despite different names*

### Comparing `pxm_liuyi778_stable-1.0.2/README.md` & `pxm_liuyi778_stable-1.0.3/README.md`

 * *Files identical despite different names*

### Comparing `pxm_liuyi778_stable-1.0.2/pyproject.toml` & `pxm_liuyi778_stable-1.0.3/pyproject.toml`

 * *Files 14% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [project]
 name = "pxm_liuyi778_Stable"
-version = "1.0.2"
+version = "1.0.3"
 authors = [
   { name="坐公交也用券", email="liumou.site@qq.com" },
 ]
 description = "这是一个Python编写的表格读写常用操作功能基础模块,基于openpyxl封装常用功能"
 readme = "README.md"
 requires-python = ">=3.7"
 classifiers = [
```

### Comparing `pxm_liuyi778_stable-1.0.2/PKG-INFO` & `pxm_liuyi778_stable-1.0.3/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pxm_liuyi778_Stable
-Version: 1.0.2
+Version: 1.0.3
 Summary: 这是一个Python编写的表格读写常用操作功能基础模块,基于openpyxl封装常用功能
 Project-URL: Homepage, https://gitee.com/liumou_site/pxm
 Project-URL: Bug Tracker, https://gitee.com/liumou_site/pxm/issues
 Author-email: 坐公交也用券 <liumou.site@qq.com>
 License-File: LICENSE
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

