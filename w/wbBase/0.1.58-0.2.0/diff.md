# Comparing `tmp/wbBase-0.1.58.tar.gz` & `tmp/wbBase-0.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "wbBase-0.1.58.tar", last modified: Thu May  4 10:12:29 2023, max compression
+gzip compressed data, was "wbBase-0.2.0.tar", last modified: Mon Jun 12 09:36:34 2023, max compression
```

## Comparing `wbBase-0.1.58.tar` & `wbBase-0.2.0.tar`

### file list

```diff
@@ -1,43 +1,43 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-04 10:12:29.182245 wbBase-0.1.58/
--rw-rw-rw-   0 root         (0) root         (0)     1079 2023-05-04 10:12:27.000000 wbBase-0.1.58/LICENSE
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-04 10:12:29.170244 wbBase-0.1.58/Lib/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-04 10:12:29.176245 wbBase-0.1.58/Lib/wbBase/
--rw-rw-rw-   0 root         (0) root         (0)      153 2023-05-04 10:12:27.000000 wbBase-0.1.58/Lib/wbBase/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)    23569 2023-05-04 10:12:27.000000 wbBase-0.1.58/Lib/wbBase/application.py
--rw-rw-rw-   0 root         (0) root         (0)     2165 2023-05-04 10:12:27.000000 wbBase-0.1.58/Lib/wbBase/applicationInfo.py
--rw-rw-rw-   0 root         (0) root         (0)    20622 2023-05-04 10:12:27.000000 wbBase-0.1.58/Lib/wbBase/applicationWindow.py
--rw-rw-rw-   0 root         (0) root         (0)   309800 2023-05-04 10:12:27.000000 wbBase-0.1.58/Lib/wbBase/artprovider.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-04 10:12:29.179245 wbBase-0.1.58/Lib/wbBase/control/
--rw-rw-rw-   0 root         (0) root         (0)     1118 2023-05-04 10:12:27.000000 wbBase-0.1.58/Lib/wbBase/control/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     4414 2023-05-04 10:12:27.000000 wbBase-0.1.58/Lib/wbBase/control/externalToolConfig.py
--rw-rw-rw-   0 root         (0) root         (0)     5891 2023-05-04 10:12:27.000000 wbBase-0.1.58/Lib/wbBase/control/externalToolConfigUI.py
--rw-rw-rw-   0 root         (0) root         (0)     2666 2023-05-04 10:12:27.000000 wbBase-0.1.58/Lib/wbBase/control/filling.py
--rw-rw-rw-   0 root         (0) root         (0)     1670 2023-05-04 10:12:27.000000 wbBase-0.1.58/Lib/wbBase/control/iePanel.py
--rw-rw-rw-   0 root         (0) root         (0)     8569 2023-05-04 10:12:27.000000 wbBase-0.1.58/Lib/wbBase/control/propgrid.py
--rw-rw-rw-   0 root         (0) root         (0)    47198 2023-05-04 10:12:27.000000 wbBase-0.1.58/Lib/wbBase/control/textEditControl.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-04 10:12:29.180245 wbBase-0.1.58/Lib/wbBase/dialog/
--rw-rw-rw-   0 root         (0) root         (0)       68 2023-05-04 10:12:27.000000 wbBase-0.1.58/Lib/wbBase/dialog/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     2342 2023-05-04 10:12:27.000000 wbBase-0.1.58/Lib/wbBase/dialog/multiSaveModifiedDialog.py
--rw-rw-rw-   0 root         (0) root         (0)     3293 2023-05-04 10:12:27.000000 wbBase-0.1.58/Lib/wbBase/dialog/multiSaveModifiedDialogUI.py
--rw-rw-rw-   0 root         (0) root         (0)    20381 2023-05-04 10:12:27.000000 wbBase-0.1.58/Lib/wbBase/dialog/preferences.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-04 10:12:29.182245 wbBase-0.1.58/Lib/wbBase/document/
--rw-rw-rw-   0 root         (0) root         (0)    23492 2023-05-04 10:12:27.000000 wbBase-0.1.58/Lib/wbBase/document/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)    36912 2023-05-04 10:12:27.000000 wbBase-0.1.58/Lib/wbBase/document/manager.py
--rw-rw-rw-   0 root         (0) root         (0)     4743 2023-05-04 10:12:27.000000 wbBase-0.1.58/Lib/wbBase/document/notebook.py
--rw-rw-rw-   0 root         (0) root         (0)     8016 2023-05-04 10:12:27.000000 wbBase-0.1.58/Lib/wbBase/document/template.py
--rw-rw-rw-   0 root         (0) root         (0)     9208 2023-05-04 10:12:27.000000 wbBase-0.1.58/Lib/wbBase/document/view.py
--rw-rw-rw-   0 root         (0) root         (0)    21455 2023-05-04 10:12:27.000000 wbBase-0.1.58/Lib/wbBase/panelManager.py
--rw-rw-rw-   0 root         (0) root         (0)     3366 2023-05-04 10:12:27.000000 wbBase-0.1.58/Lib/wbBase/pluginManager.py
--rw-rw-rw-   0 root         (0) root         (0)     2942 2023-05-04 10:12:27.000000 wbBase-0.1.58/Lib/wbBase/pluginManager_old.py
--rw-rw-rw-   0 root         (0) root         (0)     8814 2023-05-04 10:12:27.000000 wbBase-0.1.58/Lib/wbBase/scripting.py
--rw-rw-rw-   0 root         (0) root         (0)      922 2023-05-04 10:12:27.000000 wbBase-0.1.58/Lib/wbBase/tools.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-04 10:12:29.177245 wbBase-0.1.58/Lib/wbBase.egg-info/
--rw-r--r--   0 root         (0) root         (0)     2708 2023-05-04 10:12:29.000000 wbBase-0.1.58/Lib/wbBase.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     1027 2023-05-04 10:12:29.000000 wbBase-0.1.58/Lib/wbBase.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-05-04 10:12:29.000000 wbBase-0.1.58/Lib/wbBase.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)       90 2023-05-04 10:12:29.000000 wbBase-0.1.58/Lib/wbBase.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)        7 2023-05-04 10:12:29.000000 wbBase-0.1.58/Lib/wbBase.egg-info/top_level.txt
--rw-r--r--   0 root         (0) root         (0)     2708 2023-05-04 10:12:29.182245 wbBase-0.1.58/PKG-INFO
--rw-rw-rw-   0 root         (0) root         (0)     1347 2023-05-04 10:12:27.000000 wbBase-0.1.58/README.md
--rw-rw-rw-   0 root         (0) root         (0)     1992 2023-05-04 10:12:29.183245 wbBase-0.1.58/setup.cfg
--rw-rw-rw-   0 root         (0) root         (0)       39 2023-05-04 10:12:27.000000 wbBase-0.1.58/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-12 09:36:34.919423 wbBase-0.2.0/
+-rw-rw-rw-   0 root         (0) root         (0)     1079 2023-06-12 09:36:33.000000 wbBase-0.2.0/LICENSE
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-12 09:36:34.912423 wbBase-0.2.0/Lib/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-12 09:36:34.915423 wbBase-0.2.0/Lib/wbBase/
+-rw-rw-rw-   0 root         (0) root         (0)      152 2023-06-12 09:36:33.000000 wbBase-0.2.0/Lib/wbBase/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)    23696 2023-06-12 09:36:33.000000 wbBase-0.2.0/Lib/wbBase/application.py
+-rw-rw-rw-   0 root         (0) root         (0)     2165 2023-06-12 09:36:33.000000 wbBase-0.2.0/Lib/wbBase/applicationInfo.py
+-rw-rw-rw-   0 root         (0) root         (0)    20622 2023-06-12 09:36:33.000000 wbBase-0.2.0/Lib/wbBase/applicationWindow.py
+-rw-rw-rw-   0 root         (0) root         (0)   309800 2023-06-12 09:36:33.000000 wbBase-0.2.0/Lib/wbBase/artprovider.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-12 09:36:34.917423 wbBase-0.2.0/Lib/wbBase/control/
+-rw-rw-rw-   0 root         (0) root         (0)     1118 2023-06-12 09:36:33.000000 wbBase-0.2.0/Lib/wbBase/control/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     4414 2023-06-12 09:36:33.000000 wbBase-0.2.0/Lib/wbBase/control/externalToolConfig.py
+-rw-rw-rw-   0 root         (0) root         (0)     5891 2023-06-12 09:36:33.000000 wbBase-0.2.0/Lib/wbBase/control/externalToolConfigUI.py
+-rw-rw-rw-   0 root         (0) root         (0)     2666 2023-06-12 09:36:33.000000 wbBase-0.2.0/Lib/wbBase/control/filling.py
+-rw-rw-rw-   0 root         (0) root         (0)     1670 2023-06-12 09:36:33.000000 wbBase-0.2.0/Lib/wbBase/control/iePanel.py
+-rw-rw-rw-   0 root         (0) root         (0)     8569 2023-06-12 09:36:33.000000 wbBase-0.2.0/Lib/wbBase/control/propgrid.py
+-rw-rw-rw-   0 root         (0) root         (0)    47198 2023-06-12 09:36:33.000000 wbBase-0.2.0/Lib/wbBase/control/textEditControl.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-12 09:36:34.918423 wbBase-0.2.0/Lib/wbBase/dialog/
+-rw-rw-rw-   0 root         (0) root         (0)       68 2023-06-12 09:36:33.000000 wbBase-0.2.0/Lib/wbBase/dialog/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     2342 2023-06-12 09:36:33.000000 wbBase-0.2.0/Lib/wbBase/dialog/multiSaveModifiedDialog.py
+-rw-rw-rw-   0 root         (0) root         (0)     3293 2023-06-12 09:36:33.000000 wbBase-0.2.0/Lib/wbBase/dialog/multiSaveModifiedDialogUI.py
+-rw-rw-rw-   0 root         (0) root         (0)    20381 2023-06-12 09:36:33.000000 wbBase-0.2.0/Lib/wbBase/dialog/preferences.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-12 09:36:34.919423 wbBase-0.2.0/Lib/wbBase/document/
+-rw-rw-rw-   0 root         (0) root         (0)    23492 2023-06-12 09:36:33.000000 wbBase-0.2.0/Lib/wbBase/document/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)    36912 2023-06-12 09:36:33.000000 wbBase-0.2.0/Lib/wbBase/document/manager.py
+-rw-rw-rw-   0 root         (0) root         (0)     4743 2023-06-12 09:36:33.000000 wbBase-0.2.0/Lib/wbBase/document/notebook.py
+-rw-rw-rw-   0 root         (0) root         (0)     8016 2023-06-12 09:36:33.000000 wbBase-0.2.0/Lib/wbBase/document/template.py
+-rw-rw-rw-   0 root         (0) root         (0)     9208 2023-06-12 09:36:33.000000 wbBase-0.2.0/Lib/wbBase/document/view.py
+-rw-rw-rw-   0 root         (0) root         (0)    21455 2023-06-12 09:36:33.000000 wbBase-0.2.0/Lib/wbBase/panelManager.py
+-rw-rw-rw-   0 root         (0) root         (0)     3366 2023-06-12 09:36:33.000000 wbBase-0.2.0/Lib/wbBase/pluginManager.py
+-rw-rw-rw-   0 root         (0) root         (0)     2942 2023-06-12 09:36:33.000000 wbBase-0.2.0/Lib/wbBase/pluginManager_old.py
+-rw-rw-rw-   0 root         (0) root         (0)     8814 2023-06-12 09:36:33.000000 wbBase-0.2.0/Lib/wbBase/scripting.py
+-rw-rw-rw-   0 root         (0) root         (0)      929 2023-06-12 09:36:33.000000 wbBase-0.2.0/Lib/wbBase/tools.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-12 09:36:34.916423 wbBase-0.2.0/Lib/wbBase.egg-info/
+-rw-r--r--   0 root         (0) root         (0)     2751 2023-06-12 09:36:34.000000 wbBase-0.2.0/Lib/wbBase.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     1027 2023-06-12 09:36:34.000000 wbBase-0.2.0/Lib/wbBase.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-06-12 09:36:34.000000 wbBase-0.2.0/Lib/wbBase.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)       90 2023-06-12 09:36:34.000000 wbBase-0.2.0/Lib/wbBase.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)        7 2023-06-12 09:36:34.000000 wbBase-0.2.0/Lib/wbBase.egg-info/top_level.txt
+-rw-r--r--   0 root         (0) root         (0)     2751 2023-06-12 09:36:34.919423 wbBase-0.2.0/PKG-INFO
+-rw-rw-rw-   0 root         (0) root         (0)     1347 2023-06-12 09:36:33.000000 wbBase-0.2.0/README.md
+-rw-rw-rw-   0 root         (0) root         (0)     2032 2023-06-12 09:36:34.920423 wbBase-0.2.0/setup.cfg
+-rw-rw-rw-   0 root         (0) root         (0)       39 2023-06-12 09:36:33.000000 wbBase-0.2.0/setup.py
```

### Comparing `wbBase-0.1.58/LICENSE` & `wbBase-0.2.0/LICENSE`

 * *Files identical despite different names*

### Comparing `wbBase-0.1.58/Lib/wbBase/application.py` & `wbBase-0.2.0/Lib/wbBase/application.py`

 * *Files 2% similar despite different names*

```diff
@@ -44,14 +44,15 @@
 
 log = logging.getLogger(__name__)
 
 AppInfo_None = 0
 AppInfo_AppName = 1
 AppInfo_VendorName = 2
 
+
 class ExtChangeTestTimer(wx.Timer):
     """
     Timer for test of external changes
     """
 
     @property
     def app(self) -> App:
@@ -99,22 +100,22 @@
             topWin.RequestUserAttention()
         self.Start(200)
 
 
 class AppSplashScreen(SplashScreen):
     def __init__(
         self,
-        bitmap,
-        splashStyle,
-        milliseconds,
-        parent,
-        id=wx.ID_ANY,
-        pos=wx.DefaultPosition,
-        size=wx.DefaultSize,
-        style=wx.BORDER_SIMPLE | wx.FRAME_NO_TASKBAR | wx.STAY_ON_TOP,
+        bitmap: wx.Bitmap,
+        splashStyle: int,
+        milliseconds: int,
+        parent: wx.Frame,
+        id: int = wx.ID_ANY,
+        pos: wx.Point = wx.DefaultPosition,
+        size: wx.Size = wx.DefaultSize,
+        style: int = wx.BORDER_SIMPLE | wx.FRAME_NO_TASKBAR | wx.STAY_ON_TOP,
     ):
         super().__init__(
             bitmap, splashStyle, milliseconds, parent, id, pos, size, style
         )
         position = wx.Point(0, bitmap.Height - 20)
         size = wx.Size(bitmap.Width, 20)
         self.message = wx.StaticText(
@@ -122,15 +123,15 @@
             wx.ID_ANY,
             "Loading App ...",
             position,
             size,
             wx.ALIGN_CENTER_HORIZONTAL | wx.ST_ELLIPSIZE_MIDDLE | wx.TRANSPARENT_WINDOW,
         )
 
-    def setMessage(self, text):
+    def setMessage(self, text:str) -> None:
         self.message.SetLabel(text)
 
 
 class App(wx.App):
     """
     Implements the main application object
     """
@@ -329,15 +330,15 @@
             "__file__",
             "__name__",
             "app",
             "wx",
         ]
         for attr in ("AppName", "AppDisplayName", "VendorName", "VendorDisplayName"):
             setattr(self, attr, getattr(self.info, attr))
-        self.Traits.StandardPaths.UseAppInfo(AppInfo_VendorName|AppInfo_AppName)
+        self.Traits.StandardPaths.UseAppInfo(AppInfo_VendorName | AppInfo_AppName)
         if self.test:
             self.config = wx.FileConfig()
         else:
             self.config = self.Traits.CreateConfig()
         self.instanceChecker = wx.SingleInstanceChecker(
             f"{self.AppName}-{wx.GetUserId()}"
         )
@@ -554,15 +555,17 @@
             sys.exit(0)
         else:
             self.listenAndLoadTimer.Start(250)
 
     def prepareSharedDataFolder(self) -> None:
         self.splashMessage("Preparing shared data folder")
         cfg = self.config
-        defaultFolder = os.path.join(self.Traits.StandardPaths.UserLocalDataDir, "shared")
+        defaultFolder = os.path.join(
+            self.Traits.StandardPaths.UserLocalDataDir, "shared"
+        )
         with wx.ConfigPathChanger(cfg, "/Application/SharedData/"):
             folder = cfg.Read("Dir", defaultFolder)
             url = cfg.Read("URL", "")
             pull_on_start = cfg.ReadBool("PullOnStart", False)
             if folder:
                 if not os.path.isdir(folder) and not self.test:
                     try:
@@ -614,15 +617,17 @@
                     wx.LogError(f"{e}")
         else:
             wx.LogWarning(" GIT not available\n\nShared Data will not be pulled!")
 
     def preparePrivateDataFolder(self) -> None:
         self.splashMessage("Preparing private data folder")
         cfg = self.config
-        defaultFolder = os.path.join(self.Traits.StandardPaths.UserLocalDataDir, "private")
+        defaultFolder = os.path.join(
+            self.Traits.StandardPaths.UserLocalDataDir, "private"
+        )
         with wx.ConfigPathChanger(cfg, "/Application/PrivateData/"):
             folder = cfg.Read("Dir", defaultFolder)
             if not os.path.isdir(folder) and not self.test:
                 os.makedirs(folder)
             self.privateDataDir = folder
 
     def MacOpenFiles(self, fileNames) -> None:
```

### Comparing `wbBase-0.1.58/Lib/wbBase/applicationInfo.py` & `wbBase-0.2.0/Lib/wbBase/applicationInfo.py`

 * *Files identical despite different names*

### Comparing `wbBase-0.1.58/Lib/wbBase/applicationWindow.py` & `wbBase-0.2.0/Lib/wbBase/applicationWindow.py`

 * *Files identical despite different names*

### Comparing `wbBase-0.1.58/Lib/wbBase/artprovider.py` & `wbBase-0.2.0/Lib/wbBase/artprovider.py`

 * *Files identical despite different names*

### Comparing `wbBase-0.1.58/Lib/wbBase/control/__init__.py` & `wbBase-0.2.0/Lib/wbBase/control/__init__.py`

 * *Files identical despite different names*

### Comparing `wbBase-0.1.58/Lib/wbBase/control/externalToolConfig.py` & `wbBase-0.2.0/Lib/wbBase/control/externalToolConfig.py`

 * *Files identical despite different names*

### Comparing `wbBase-0.1.58/Lib/wbBase/control/externalToolConfigUI.py` & `wbBase-0.2.0/Lib/wbBase/control/externalToolConfigUI.py`

 * *Files identical despite different names*

### Comparing `wbBase-0.1.58/Lib/wbBase/control/filling.py` & `wbBase-0.2.0/Lib/wbBase/control/filling.py`

 * *Files identical despite different names*

### Comparing `wbBase-0.1.58/Lib/wbBase/control/iePanel.py` & `wbBase-0.2.0/Lib/wbBase/control/iePanel.py`

 * *Files identical despite different names*

### Comparing `wbBase-0.1.58/Lib/wbBase/control/propgrid.py` & `wbBase-0.2.0/Lib/wbBase/control/propgrid.py`

 * *Files identical despite different names*

### Comparing `wbBase-0.1.58/Lib/wbBase/control/textEditControl.py` & `wbBase-0.2.0/Lib/wbBase/control/textEditControl.py`

 * *Files identical despite different names*

### Comparing `wbBase-0.1.58/Lib/wbBase/dialog/multiSaveModifiedDialog.py` & `wbBase-0.2.0/Lib/wbBase/dialog/multiSaveModifiedDialog.py`

 * *Files identical despite different names*

### Comparing `wbBase-0.1.58/Lib/wbBase/dialog/multiSaveModifiedDialogUI.py` & `wbBase-0.2.0/Lib/wbBase/dialog/multiSaveModifiedDialogUI.py`

 * *Files identical despite different names*

### Comparing `wbBase-0.1.58/Lib/wbBase/dialog/preferences.py` & `wbBase-0.2.0/Lib/wbBase/dialog/preferences.py`

 * *Files identical despite different names*

### Comparing `wbBase-0.1.58/Lib/wbBase/document/__init__.py` & `wbBase-0.2.0/Lib/wbBase/document/__init__.py`

 * *Files identical despite different names*

### Comparing `wbBase-0.1.58/Lib/wbBase/document/manager.py` & `wbBase-0.2.0/Lib/wbBase/document/manager.py`

 * *Files identical despite different names*

### Comparing `wbBase-0.1.58/Lib/wbBase/document/notebook.py` & `wbBase-0.2.0/Lib/wbBase/document/notebook.py`

 * *Files identical despite different names*

### Comparing `wbBase-0.1.58/Lib/wbBase/document/template.py` & `wbBase-0.2.0/Lib/wbBase/document/template.py`

 * *Files identical despite different names*

### Comparing `wbBase-0.1.58/Lib/wbBase/document/view.py` & `wbBase-0.2.0/Lib/wbBase/document/view.py`

 * *Files identical despite different names*

### Comparing `wbBase-0.1.58/Lib/wbBase/panelManager.py` & `wbBase-0.2.0/Lib/wbBase/panelManager.py`

 * *Files identical despite different names*

### Comparing `wbBase-0.1.58/Lib/wbBase/pluginManager.py` & `wbBase-0.2.0/Lib/wbBase/pluginManager.py`

 * *Files identical despite different names*

### Comparing `wbBase-0.1.58/Lib/wbBase/pluginManager_old.py` & `wbBase-0.2.0/Lib/wbBase/pluginManager_old.py`

 * *Files identical despite different names*

### Comparing `wbBase-0.1.58/Lib/wbBase/scripting.py` & `wbBase-0.2.0/Lib/wbBase/scripting.py`

 * *Files identical despite different names*

### Comparing `wbBase-0.1.58/Lib/wbBase/tools.py` & `wbBase-0.2.0/Lib/wbBase/tools.py`

 * *Files 11% similar despite different names*

```diff
@@ -29,9 +29,9 @@
     style=wx.FONTSTYLE_NORMAL,
     weight=wx.FONTWEIGHT_NORMAL,
     underline=False,
     faceName="",
     encoding=wx.FONTENCODING_DEFAULT,
 ) -> wx.Font:
     return wx.TheFontList.FindOrCreateFont(
-        pointSize, family, style, weight, underline, faceName, encoding
+        round(pointSize), family, style, weight, underline, faceName, encoding
     )
```

### Comparing `wbBase-0.1.58/Lib/wbBase.egg-info/PKG-INFO` & `wbBase-0.2.0/Lib/wbBase.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,39 +1,40 @@
 Metadata-Version: 2.1
 Name: wbBase
-Version: 0.1.58
+Version: 0.2.0
 Summary: Base package for WorkBench applications.
 Home-page: https://gitlab.com/workbench2/wbbase
 Author: Andreas Eigendorf
 License: MIT
 Project-URL: Source, https://gitlab.com/workbench2/wbbase
 Project-URL: Documentation, https://workbench2.gitlab.io/wbbase
 Project-URL: Tracker, https://gitlab.com/workbench2/wbbase/-/issues
 Keywords: workbench,wxPython,GUI
 Platform: WIN32
 Platform: WIN64
 Platform: OSX
 Platform: POSIX
-Classifier: Development Status :: 3 - Alpha
+Classifier: Development Status :: 4 - Beta
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: MacOS
 Classifier: Operating System :: Microsoft :: Windows
 Classifier: Operating System :: POSIX
 Classifier: Environment :: MacOS X :: Cocoa
 Classifier: Environment :: Win32 (MS Windows)
 Classifier: Environment :: X11 Applications :: GTK
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: Implementation :: CPython
 Classifier: Intended Audience :: Developers
 Classifier: Topic :: Software Development :: Libraries
 Classifier: Topic :: Software Development :: User Interfaces
-Requires-Python: <3.11,>=3.8
+Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 # wbBase
 
 This is the base package for WorkBench applications.
 Workbench is a plugin based RAD framework for platform independent GUI applications
```

### Comparing `wbBase-0.1.58/Lib/wbBase.egg-info/SOURCES.txt` & `wbBase-0.2.0/Lib/wbBase.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `wbBase-0.1.58/PKG-INFO` & `wbBase-0.2.0/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,39 +1,40 @@
 Metadata-Version: 2.1
 Name: wbBase
-Version: 0.1.58
+Version: 0.2.0
 Summary: Base package for WorkBench applications.
 Home-page: https://gitlab.com/workbench2/wbbase
 Author: Andreas Eigendorf
 License: MIT
 Project-URL: Source, https://gitlab.com/workbench2/wbbase
 Project-URL: Documentation, https://workbench2.gitlab.io/wbbase
 Project-URL: Tracker, https://gitlab.com/workbench2/wbbase/-/issues
 Keywords: workbench,wxPython,GUI
 Platform: WIN32
 Platform: WIN64
 Platform: OSX
 Platform: POSIX
-Classifier: Development Status :: 3 - Alpha
+Classifier: Development Status :: 4 - Beta
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: MacOS
 Classifier: Operating System :: Microsoft :: Windows
 Classifier: Operating System :: POSIX
 Classifier: Environment :: MacOS X :: Cocoa
 Classifier: Environment :: Win32 (MS Windows)
 Classifier: Environment :: X11 Applications :: GTK
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: Implementation :: CPython
 Classifier: Intended Audience :: Developers
 Classifier: Topic :: Software Development :: Libraries
 Classifier: Topic :: Software Development :: User Interfaces
-Requires-Python: <3.11,>=3.8
+Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 # wbBase
 
 This is the base package for WorkBench applications.
 Workbench is a plugin based RAD framework for platform independent GUI applications
```

### Comparing `wbBase-0.1.58/README.md` & `wbBase-0.2.0/README.md`

 * *Files identical despite different names*

### Comparing `wbBase-0.1.58/setup.cfg` & `wbBase-0.2.0/setup.cfg`

 * *Files 6% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 [bumpversion]
-current_version = 0.1.58
+current_version = 0.2.0
 commit = True
 tag = True
 tag_name = {new_version}
 parse = (?P<major>\d+)\.(?P<minor>\d+)\.(?P<patch>\d+)?
 serialize = 
 	{major}.{minor}.{patch}
 
@@ -27,55 +27,57 @@
 	OSX
 	POSIX
 keywords = 
 	workbench
 	wxPython
 	GUI
 classifiers = 
-	Development Status :: 3 - Alpha
+	Development Status :: 4 - Beta
 	License :: OSI Approved :: MIT License
 	Operating System :: MacOS
 	Operating System :: Microsoft :: Windows
 	Operating System :: POSIX
 	Environment :: MacOS X :: Cocoa
 	Environment :: Win32 (MS Windows)
 	Environment :: X11 Applications :: GTK
 	Programming Language :: Python :: 3
 	Programming Language :: Python :: 3.8
 	Programming Language :: Python :: 3.9
 	Programming Language :: Python :: 3.10
+	Programming Language :: Python :: 3.11
 	Programming Language :: Python :: Implementation :: CPython
 	Intended Audience :: Developers
 	Topic :: Software Development :: Libraries
 	Topic :: Software Development :: User Interfaces
 
 [options]
 package_dir = 
 	=Lib
 packages = find:
-python_requires = >=3.8,<3.11
+python_requires = >=3.8
 install_requires = 
-	wxpython>=4.2.0
+	wxpython>=4.2.1
 	GitPython>=3.1
 	PyYAML>=6.0
 	importlib_metadata;python_version<'3.10'
 
 [options.packages.find]
 where = Lib
 
 [bumpversion:file:Lib/wbBase/__init__.py]
 search = __version__ = "{current_version}"
 replace = __version__ = "{new_version}"
 
 [tox:tox]
-min_version = 4.5
+min_version = 4.6
 env_list = 
 	py38
 	py39
-	py10
+	py310
+	py311
 
 [testenv]
 deps = 
 	pytest
 	pytest-cov
 	coverage
 commands =
```

