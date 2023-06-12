# Comparing `tmp/pxm_liuyi778_stable-1.0.0.tar.gz` & `tmp/pxm_liuyi778_stable-1.0.2.tar.gz`

## Comparing `pxm_liuyi778_stable-1.0.0.tar` & `pxm_liuyi778_stable-1.0.2.tar`

### file list

```diff
@@ -1,27 +1,27 @@
--rw-r--r--   0        0        0     1544 2020-02-02 00:00:00.000000 pxm_liuyi778_stable-1.0.0/DemoRead.py
--rw-r--r--   0        0        0     1336 2020-02-02 00:00:00.000000 pxm_liuyi778_stable-1.0.0/DemoWrite.py
--rw-r--r--   0        0        0     3115 2020-02-02 00:00:00.000000 pxm_liuyi778_stable-1.0.0/UploadToPypi.py
--rw-r--r--   0        0        0       69 2020-02-02 00:00:00.000000 pxm_liuyi778_stable-1.0.0/req.py
--rw-r--r--   0        0        0       35 2020-02-02 00:00:00.000000 pxm_liuyi778_stable-1.0.0/requirements.txt
--rw-r--r--   0        0        0       50 2020-02-02 00:00:00.000000 pxm_liuyi778_stable-1.0.0/.idea/.gitignore
--rw-r--r--   0        0        0      189 2020-02-02 00:00:00.000000 pxm_liuyi778_stable-1.0.0/.idea/misc.xml
--rw-r--r--   0        0        0      265 2020-02-02 00:00:00.000000 pxm_liuyi778_stable-1.0.0/.idea/modules.xml
--rw-r--r--   0        0        0      440 2020-02-02 00:00:00.000000 pxm_liuyi778_stable-1.0.0/.idea/pxm.iml
--rw-r--r--   0        0        0      185 2020-02-02 00:00:00.000000 pxm_liuyi778_stable-1.0.0/.idea/vcs.xml
--rw-r--r--   0        0        0    10941 2020-02-02 00:00:00.000000 pxm_liuyi778_stable-1.0.0/.idea/workspace.xml
--rw-r--r--   0        0        0     8474 2020-02-02 00:00:00.000000 pxm_liuyi778_stable-1.0.0/.idea/inspectionProfiles/Project_Default.xml
--rw-r--r--   0        0        0      179 2020-02-02 00:00:00.000000 pxm_liuyi778_stable-1.0.0/.idea/inspectionProfiles/profiles_settings.xml
--rw-r--r--   0        0        0      386 2020-02-02 00:00:00.000000 pxm_liuyi778_stable-1.0.0/src/pxm_liuyi778_Stable/__init__.py
--rw-r--r--   0        0        0      349 2020-02-02 00:00:00.000000 pxm_liuyi778_stable-1.0.0/src/pxm_liuyi778_Stable/dic.py
--rw-r--r--   0        0        0      702 2020-02-02 00:00:00.000000 pxm_liuyi778_stable-1.0.0/src/pxm_liuyi778_Stable/exists.py
--rw-r--r--   0        0        0      413 2020-02-02 00:00:00.000000 pxm_liuyi778_stable-1.0.0/src/pxm_liuyi778_Stable/pxm.py
--rw-r--r--   0        0        0     7814 2020-02-02 00:00:00.000000 pxm_liuyi778_stable-1.0.0/src/pxm_liuyi778_Stable/read.py
--rw-r--r--   0        0        0     4036 2020-02-02 00:00:00.000000 pxm_liuyi778_stable-1.0.0/src/pxm_liuyi778_Stable/write.py
--rw-r--r--   0        0        0      204 2020-02-02 00:00:00.000000 pxm_liuyi778_stable-1.0.0/src/tests/read.py
--rw-r--r--   0        0        0    10310 2020-02-02 00:00:00.000000 pxm_liuyi778_stable-1.0.0/xls/demo.xlsx
--rw-r--r--   0        0        0     4841 2020-02-02 00:00:00.000000 pxm_liuyi778_stable-1.0.0/xls/demoW.xlsx
--rw-r--r--   0        0        0     2174 2020-02-02 00:00:00.000000 pxm_liuyi778_stable-1.0.0/.gitignore
--rw-r--r--   0        0        0    11558 2020-02-02 00:00:00.000000 pxm_liuyi778_stable-1.0.0/LICENSE
--rw-r--r--   0        0        0     3023 2020-02-02 00:00:00.000000 pxm_liuyi778_stable-1.0.0/README.md
--rw-r--r--   0        0        0      666 2020-02-02 00:00:00.000000 pxm_liuyi778_stable-1.0.0/pyproject.toml
--rw-r--r--   0        0        0     3504 2020-02-02 00:00:00.000000 pxm_liuyi778_stable-1.0.0/PKG-INFO
+-rw-r--r--   0        0        0     1544 2020-02-02 00:00:00.000000 pxm_liuyi778_stable-1.0.2/DemoRead.py
+-rw-r--r--   0        0        0     1336 2020-02-02 00:00:00.000000 pxm_liuyi778_stable-1.0.2/DemoWrite.py
+-rw-r--r--   0        0        0     3115 2020-02-02 00:00:00.000000 pxm_liuyi778_stable-1.0.2/UploadToPypi.py
+-rw-r--r--   0        0        0       69 2020-02-02 00:00:00.000000 pxm_liuyi778_stable-1.0.2/req.py
+-rw-r--r--   0        0        0       35 2020-02-02 00:00:00.000000 pxm_liuyi778_stable-1.0.2/requirements.txt
+-rw-r--r--   0        0        0       50 2020-02-02 00:00:00.000000 pxm_liuyi778_stable-1.0.2/.idea/.gitignore
+-rw-r--r--   0        0        0      189 2020-02-02 00:00:00.000000 pxm_liuyi778_stable-1.0.2/.idea/misc.xml
+-rw-r--r--   0        0        0      265 2020-02-02 00:00:00.000000 pxm_liuyi778_stable-1.0.2/.idea/modules.xml
+-rw-r--r--   0        0        0      440 2020-02-02 00:00:00.000000 pxm_liuyi778_stable-1.0.2/.idea/pxm.iml
+-rw-r--r--   0        0        0      185 2020-02-02 00:00:00.000000 pxm_liuyi778_stable-1.0.2/.idea/vcs.xml
+-rw-r--r--   0        0        0    10643 2020-02-02 00:00:00.000000 pxm_liuyi778_stable-1.0.2/.idea/workspace.xml
+-rw-r--r--   0        0        0     8474 2020-02-02 00:00:00.000000 pxm_liuyi778_stable-1.0.2/.idea/inspectionProfiles/Project_Default.xml
+-rw-r--r--   0        0        0      179 2020-02-02 00:00:00.000000 pxm_liuyi778_stable-1.0.2/.idea/inspectionProfiles/profiles_settings.xml
+-rw-r--r--   0        0        0      340 2020-02-02 00:00:00.000000 pxm_liuyi778_stable-1.0.2/src/pxm_liuyi778_Stable/__init__.py
+-rw-r--r--   0        0        0      349 2020-02-02 00:00:00.000000 pxm_liuyi778_stable-1.0.2/src/pxm_liuyi778_Stable/dic.py
+-rw-r--r--   0        0        0      702 2020-02-02 00:00:00.000000 pxm_liuyi778_stable-1.0.2/src/pxm_liuyi778_Stable/exists.py
+-rw-r--r--   0        0        0      413 2020-02-02 00:00:00.000000 pxm_liuyi778_stable-1.0.2/src/pxm_liuyi778_Stable/pxm.py
+-rw-r--r--   0        0        0     7814 2020-02-02 00:00:00.000000 pxm_liuyi778_stable-1.0.2/src/pxm_liuyi778_Stable/read.py
+-rw-r--r--   0        0        0     4036 2020-02-02 00:00:00.000000 pxm_liuyi778_stable-1.0.2/src/pxm_liuyi778_Stable/write.py
+-rw-r--r--   0        0        0      204 2020-02-02 00:00:00.000000 pxm_liuyi778_stable-1.0.2/src/tests/read.py
+-rw-r--r--   0        0        0    10310 2020-02-02 00:00:00.000000 pxm_liuyi778_stable-1.0.2/xls/demo.xlsx
+-rw-r--r--   0        0        0     4841 2020-02-02 00:00:00.000000 pxm_liuyi778_stable-1.0.2/xls/demoW.xlsx
+-rw-r--r--   0        0        0     2174 2020-02-02 00:00:00.000000 pxm_liuyi778_stable-1.0.2/.gitignore
+-rw-r--r--   0        0        0    11558 2020-02-02 00:00:00.000000 pxm_liuyi778_stable-1.0.2/LICENSE
+-rw-r--r--   0        0        0     3023 2020-02-02 00:00:00.000000 pxm_liuyi778_stable-1.0.2/README.md
+-rw-r--r--   0        0        0      666 2020-02-02 00:00:00.000000 pxm_liuyi778_stable-1.0.2/pyproject.toml
+-rw-r--r--   0        0        0     3504 2020-02-02 00:00:00.000000 pxm_liuyi778_stable-1.0.2/PKG-INFO
```

### Comparing `pxm_liuyi778_stable-1.0.0/DemoRead.py` & `pxm_liuyi778_stable-1.0.2/DemoRead.py`

 * *Files identical despite different names*

### Comparing `pxm_liuyi778_stable-1.0.0/DemoWrite.py` & `pxm_liuyi778_stable-1.0.2/DemoWrite.py`

 * *Files identical despite different names*

### Comparing `pxm_liuyi778_stable-1.0.0/UploadToPypi.py` & `pxm_liuyi778_stable-1.0.2/UploadToPypi.py`

 * *Files identical despite different names*

### Comparing `pxm_liuyi778_stable-1.0.0/.idea/workspace.xml` & `pxm_liuyi778_stable-1.0.2/.idea/workspace.xml`

 * *Files 10% similar despite different names*

#### Comparing `pxm_liuyi778_stable-1.0.0/.idea/workspace.xml` & `pxm_liuyi778_stable-1.0.2/.idea/workspace.xml`

```diff
@@ -1,20 +1,14 @@
 <?xml version="1.0" encoding="utf-8"?>
 <project version="4">
   <component name="AutoImportSettings">
     <option name="autoReloadType" value="SELECTIVE"/>
   </component>
   <component name="ChangeListManager">
-    <list default="true" id="d41c57d7-f66c-4f3e-b27b-fe814c0a247d" name="变更" comment="使用新标准上传">
-      <change beforePath="$PROJECT_DIR$/README.md" beforeDir="false" afterPath="$PROJECT_DIR$/README.md" afterDir="false"/>
-      <change beforePath="$PROJECT_DIR$/UploadToPypi.py" beforeDir="false" afterPath="$PROJECT_DIR$/UploadToPypi.py" afterDir="false"/>
-      <change beforePath="$PROJECT_DIR$/pyproject.toml" beforeDir="false" afterPath="$PROJECT_DIR$/pyproject.toml" afterDir="false"/>
-      <change beforePath="$PROJECT_DIR$/src/pxm_liuyi778_Stable/__init__.py" beforeDir="false" afterPath="$PROJECT_DIR$/src/pxm_liuyi778_Stable/__init__.py" afterDir="false"/>
-      <change beforePath="$PROJECT_DIR$/src/pxm_liuyi778_Stable/exists.py" beforeDir="false" afterPath="$PROJECT_DIR$/src/pxm_liuyi778_Stable/exists.py" afterDir="false"/>
-    </list>
+    <list default="true" id="d41c57d7-f66c-4f3e-b27b-fe814c0a247d" name="变更" comment="完成自动化安装"/>
     <option name="SHOW_DIALOG" value="false"/>
     <option name="HIGHLIGHT_CONFLICTS" value="true"/>
     <option name="HIGHLIGHT_NON_ACTIVE_CHANGELIST" value="false"/>
     <option name="LAST_RESOLUTION" value="IGNORE"/>
   </component>
   <component name="FileTemplateManagerImpl">
     <option name="RECENT_TEMPLATES">
@@ -31,24 +25,24 @@
     <option name="stateVersion" value="1"/>
   </component>
   <component name="ProjectId" id="2MUul9Mh4APeq7WLIx2GqKgGrFb"/>
   <component name="ProjectViewState">
     <option name="hideEmptyMiddlePackages" value="true"/>
     <option name="showLibraryContents" value="true"/>
   </component>
-  <component name="PropertiesComponent"><![CDATA[{
-  "keyToString": {
-    "RunOnceActivity.OpenProjectViewOnStart": "true",
-    "RunOnceActivity.ShowReadmeOnStart": "true",
-    "WebServerToolWindowFactoryState": "false",
-    "last_opened_file_path": "D:/code/gitee/开源/Python/plbm",
-    "nodejs_package_manager_path": "npm",
-    "settings.editor.selected.configurable": "com.jetbrains.python.configuration.PyActiveSdkModuleConfigurable"
+  <component name="PropertiesComponent">{
+  &quot;keyToString&quot;: {
+    &quot;RunOnceActivity.OpenProjectViewOnStart&quot;: &quot;true&quot;,
+    &quot;RunOnceActivity.ShowReadmeOnStart&quot;: &quot;true&quot;,
+    &quot;WebServerToolWindowFactoryState&quot;: &quot;false&quot;,
+    &quot;last_opened_file_path&quot;: &quot;D:/code/Coding/bs/printer&quot;,
+    &quot;nodejs_package_manager_path&quot;: &quot;npm&quot;,
+    &quot;settings.editor.selected.configurable&quot;: &quot;com.jetbrains.python.configuration.PyActiveSdkModuleConfigurable&quot;
   }
-}]]></component>
+}</component>
   <component name="RecentsManager">
     <key name="MoveFile.RECENT_KEYS">
       <recent name="D:\code\gitee\开源\Python\pxm\src"/>
     </key>
   </component>
   <component name="RunManager" selected="Python.UploadToPypi">
     <configuration name="UploadToPypi" type="PythonConfigurationType" factoryName="Python" temporary="true" nameIsGenerated="true">
@@ -139,15 +133,15 @@
     <task active="true" id="Default" summary="默认任务">
       <changelist id="d41c57d7-f66c-4f3e-b27b-fe814c0a247d" name="变更" comment=""/>
       <created>1677834630850</created>
       <option name="number" value="Default"/>
       <option name="presentableId" value="Default"/>
       <updated>1677834630850</updated>
       <workItem from="1686534393051" duration="1884000"/>
-      <workItem from="1686536307862" duration="660000"/>
+      <workItem from="1686536307862" duration="1345000"/>
     </task>
     <task id="LOCAL-00001" summary="更新日志">
       <created>1679642216056</created>
       <option name="number" value="00001"/>
       <option name="presentableId" value="LOCAL-00001"/>
       <option name="project" value="LOCAL"/>
       <updated>1679642216056</updated>
@@ -176,15 +170,22 @@
     <task id="LOCAL-00005" summary="使用新标准上传">
       <created>1686536333391</created>
       <option name="number" value="00005"/>
       <option name="presentableId" value="LOCAL-00005"/>
       <option name="project" value="LOCAL"/>
       <updated>1686536333391</updated>
     </task>
-    <option name="localTasksCounter" value="6"/>
+    <task id="LOCAL-00006" summary="完成自动化安装">
+      <created>1686537085850</created>
+      <option name="number" value="00006"/>
+      <option name="presentableId" value="LOCAL-00006"/>
+      <option name="project" value="LOCAL"/>
+      <updated>1686537085850</updated>
+    </task>
+    <option name="localTasksCounter" value="7"/>
     <servers/>
   </component>
   <component name="TypeScriptGeneratedFilesManager">
     <option name="version" value="3"/>
   </component>
   <component name="Vcs.Log.Tabs.Properties">
     <option name="TAB_STATES">
@@ -196,15 +197,16 @@
         </entry>
       </map>
     </option>
   </component>
   <component name="VcsManagerConfiguration">
     <MESSAGE value="更新日志"/>
     <MESSAGE value="使用新标准上传"/>
-    <option name="LAST_COMMIT_MESSAGE" value="使用新标准上传"/>
+    <MESSAGE value="完成自动化安装"/>
+    <option name="LAST_COMMIT_MESSAGE" value="完成自动化安装"/>
   </component>
   <component name="com.intellij.coverage.CoverageDataManagerImpl">
     <SUITE FILE_PATH="coverage/pxm$req.coverage" NAME="req 覆盖结果" MODIFIED="1686536122567" SOURCE_PROVIDER="com.intellij.coverage.DefaultCoverageFileProvider" RUNNER="coverage.py" COVERAGE_BY_TEST_ENABLED="true" COVERAGE_TRACING_ENABLED="false" WORKING_DIRECTORY="$PROJECT_DIR$"/>
-    <SUITE FILE_PATH="coverage/pxm$UploadToPypi.coverage" NAME="UploadToPypi 覆盖结果" MODIFIED="1686536772145" SOURCE_PROVIDER="com.intellij.coverage.DefaultCoverageFileProvider" RUNNER="coverage.py" COVERAGE_BY_TEST_ENABLED="true" COVERAGE_TRACING_ENABLED="false" WORKING_DIRECTORY="$PROJECT_DIR$"/>
+    <SUITE FILE_PATH="coverage/pxm$UploadToPypi.coverage" NAME="UploadToPypi 覆盖结果" MODIFIED="1686537025387" SOURCE_PROVIDER="com.intellij.coverage.DefaultCoverageFileProvider" RUNNER="coverage.py" COVERAGE_BY_TEST_ENABLED="true" COVERAGE_TRACING_ENABLED="false" WORKING_DIRECTORY="$PROJECT_DIR$"/>
     <SUITE FILE_PATH="coverage/pxm$.coverage" NAME=" 覆盖结果" MODIFIED="1686536236197" SOURCE_PROVIDER="com.intellij.coverage.DefaultCoverageFileProvider" RUNNER="coverage.py" COVERAGE_BY_TEST_ENABLED="true" COVERAGE_TRACING_ENABLED="false" WORKING_DIRECTORY="$PROJECT_DIR$/src/tests"/>
   </component>
 </project>
```

### Comparing `pxm_liuyi778_stable-1.0.0/.idea/inspectionProfiles/Project_Default.xml` & `pxm_liuyi778_stable-1.0.2/.idea/inspectionProfiles/Project_Default.xml`

 * *Files identical despite different names*

### Comparing `pxm_liuyi778_stable-1.0.0/src/pxm_liuyi778_Stable/exists.py` & `pxm_liuyi778_stable-1.0.2/src/pxm_liuyi778_Stable/exists.py`

 * *Files identical despite different names*

### Comparing `pxm_liuyi778_stable-1.0.0/src/pxm_liuyi778_Stable/read.py` & `pxm_liuyi778_stable-1.0.2/src/pxm_liuyi778_Stable/read.py`

 * *Files identical despite different names*

### Comparing `pxm_liuyi778_stable-1.0.0/src/pxm_liuyi778_Stable/write.py` & `pxm_liuyi778_stable-1.0.2/src/pxm_liuyi778_Stable/write.py`

 * *Files identical despite different names*

### Comparing `pxm_liuyi778_stable-1.0.0/xls/demo.xlsx` & `pxm_liuyi778_stable-1.0.2/xls/demo.xlsx`

 * *Files identical despite different names*

### Comparing `pxm_liuyi778_stable-1.0.0/xls/demoW.xlsx` & `pxm_liuyi778_stable-1.0.2/xls/demoW.xlsx`

 * *Files identical despite different names*

### Comparing `pxm_liuyi778_stable-1.0.0/.gitignore` & `pxm_liuyi778_stable-1.0.2/.gitignore`

 * *Files identical despite different names*

### Comparing `pxm_liuyi778_stable-1.0.0/LICENSE` & `pxm_liuyi778_stable-1.0.2/LICENSE`

 * *Files identical despite different names*

### Comparing `pxm_liuyi778_stable-1.0.0/README.md` & `pxm_liuyi778_stable-1.0.2/README.md`

 * *Files identical despite different names*

### Comparing `pxm_liuyi778_stable-1.0.0/pyproject.toml` & `pxm_liuyi778_stable-1.0.2/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [project]
 name = "pxm_liuyi778_Stable"
-version = "1.0.0"
+version = "1.0.2"
 authors = [
   { name="坐公交也用券", email="liumou.site@qq.com" },
 ]
 description = "这是一个Python编写的表格读写常用操作功能基础模块,基于openpyxl封装常用功能"
 readme = "README.md"
 requires-python = ">=3.7"
 classifiers = [
```

### Comparing `pxm_liuyi778_stable-1.0.0/PKG-INFO` & `pxm_liuyi778_stable-1.0.2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pxm_liuyi778_Stable
-Version: 1.0.0
+Version: 1.0.2
 Summary: 这是一个Python编写的表格读写常用操作功能基础模块,基于openpyxl封装常用功能
 Project-URL: Homepage, https://gitee.com/liumou_site/pxm
 Project-URL: Bug Tracker, https://gitee.com/liumou_site/pxm/issues
 Author-email: 坐公交也用券 <liumou.site@qq.com>
 License-File: LICENSE
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

