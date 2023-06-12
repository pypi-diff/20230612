# Comparing `tmp/mly-0.3.4.4.tar.gz` & `tmp/mly-0.3.4.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mly-0.3.4.4.tar", last modified: Tue May 23 11:51:07 2023, max compression
+gzip compressed data, was "mly-0.3.4.5.tar", last modified: Mon Jun 12 16:22:40 2023, max compression
```

## Comparing `mly-0.3.4.4.tar` & `mly-0.3.4.5.tar`

### file list

```diff
@@ -1,41 +1,41 @@
-drwxrwxr-x   0 vasileios.skliris (44659) vasileios.skliris (44659)        0 2023-05-23 11:51:07.617215 mly-0.3.4.4/
--rw-rw-r--   0 vasileios.skliris (44659) vasileios.skliris (44659)    35148 2023-05-10 08:55:19.000000 mly-0.3.4.4/LICENSE
--rw-rw-r--   0 vasileios.skliris (44659) vasileios.skliris (44659)      499 2023-05-23 11:51:07.617215 mly-0.3.4.4/PKG-INFO
--rw-rw-r--   0 vasileios.skliris (44659) vasileios.skliris (44659)        0 2021-01-11 16:48:33.000000 mly-0.3.4.4/README.md
-drwxrwxr-x   0 vasileios.skliris (44659) vasileios.skliris (44659)        0 2023-05-23 11:51:07.596215 mly-0.3.4.4/mly/
--rw-rw-r--   0 vasileios.skliris (44659) vasileios.skliris (44659)  1433718 2021-05-11 10:43:11.000000 mly-0.3.4.4/mly/SRD.py
--rw-rw-r--   0 vasileios.skliris (44659) vasileios.skliris (44659)       24 2023-05-09 14:15:39.000000 mly-0.3.4.4/mly/__init__.py
--rw-rw-r--   0 vasileios.skliris (44659) vasileios.skliris (44659)    10219 2023-05-16 10:32:51.000000 mly-0.3.4.4/mly/createFileSystem.py
-drwxrwxr-x   0 vasileios.skliris (44659) vasileios.skliris (44659)        0 2023-05-23 11:51:07.605215 mly-0.3.4.4/mly/datatools/
--rw-rw-r--   0 vasileios.skliris (44659) vasileios.skliris (44659)      140 2023-05-09 14:56:02.000000 mly-0.3.4.4/mly/datatools/__init__.py
--rw-rw-r--   0 vasileios.skliris (44659) vasileios.skliris (44659)    22280 2023-05-09 14:56:02.000000 mly-0.3.4.4/mly/datatools/core.py
--rw-rw-r--   0 vasileios.skliris (44659) vasileios.skliris (44659)    29339 2023-05-23 11:49:52.000000 mly-0.3.4.4/mly/datatools/datatools.py
--rw-rw-r--   0 vasileios.skliris (44659) vasileios.skliris (44659)    90481 2023-05-09 14:56:02.000000 mly-0.3.4.4/mly/datatools/generator.py
-drwxrwxr-x   0 vasileios.skliris (44659) vasileios.skliris (44659)        0 2023-05-23 11:51:07.611215 mly-0.3.4.4/mly/datatools/tests/
--rw-rw-r--   0 vasileios.skliris (44659) vasileios.skliris (44659)       24 2023-05-09 14:56:02.000000 mly-0.3.4.4/mly/datatools/tests/__init__.py
--rw-rw-r--   0 vasileios.skliris (44659) vasileios.skliris (44659)     3438 2023-05-09 14:56:02.000000 mly-0.3.4.4/mly/datatools/tests/test_core.py
--rw-rw-r--   0 vasileios.skliris (44659) vasileios.skliris (44659)      441 2023-05-09 14:56:02.000000 mly-0.3.4.4/mly/datatools/tests/test_datatools.py
--rw-rw-r--   0 vasileios.skliris (44659) vasileios.skliris (44659)     4570 2023-05-09 14:56:02.000000 mly-0.3.4.4/mly/datatools/tests/test_generator.py
--rw-rw-r--   0 vasileios.skliris (44659) vasileios.skliris (44659)    18459 2023-05-09 14:56:02.000000 mly-0.3.4.4/mly/exceptions.py
--rw-rw-r--   0 vasileios.skliris (44659) vasileios.skliris (44659)     7770 2022-08-17 15:08:03.000000 mly-0.3.4.4/mly/mlTools.py
--rw-rw-r--   0 vasileios.skliris (44659) vasileios.skliris (44659)     6996 2021-01-11 16:48:33.000000 mly-0.3.4.4/mly/models.py
--rw-rw-r--   0 vasileios.skliris (44659) vasileios.skliris (44659)    12353 2023-05-04 12:56:19.000000 mly-0.3.4.4/mly/null_energy_map.py
--rw-rw-r--   0 vasileios.skliris (44659) vasileios.skliris (44659)     7255 2023-05-23 11:33:19.000000 mly-0.3.4.4/mly/offlinefar.py
--rw-rw-r--   0 vasileios.skliris (44659) vasileios.skliris (44659)     7797 2023-05-04 12:56:19.000000 mly-0.3.4.4/mly/plugins.py
--rw-rw-r--   0 vasileios.skliris (44659) vasileios.skliris (44659)    10134 2023-05-04 12:56:19.000000 mly-0.3.4.4/mly/projectwave.py
--rw-rw-r--   0 vasileios.skliris (44659) vasileios.skliris (44659)     8913 2022-03-15 16:16:40.000000 mly-0.3.4.4/mly/simulateddetectornoise.py
-drwxrwxr-x   0 vasileios.skliris (44659) vasileios.skliris (44659)        0 2023-05-23 11:51:07.616215 mly-0.3.4.4/mly/tests/
--rw-rw-r--   0 vasileios.skliris (44659) vasileios.skliris (44659)      728 2021-10-07 09:34:45.000000 mly-0.3.4.4/mly/tests/__init__.py
--rw-rw-r--   0 vasileios.skliris (44659) vasileios.skliris (44659)     1601 2021-10-08 08:22:16.000000 mly-0.3.4.4/mly/tests/test_init.py
--rw-rw-r--   0 vasileios.skliris (44659) vasileios.skliris (44659)     5258 2022-03-02 09:58:19.000000 mly-0.3.4.4/mly/tests/test_tools.py
--rw-rw-r--   0 vasileios.skliris (44659) vasileios.skliris (44659)    13014 2023-05-04 12:56:19.000000 mly-0.3.4.4/mly/tools.py
--rw-rw-r--   0 vasileios.skliris (44659) vasileios.skliris (44659)   126771 2023-05-23 11:32:17.000000 mly-0.3.4.4/mly/validators.py
--rw-rw-r--   0 vasileios.skliris (44659) vasileios.skliris (44659)    34282 2023-05-09 14:56:02.000000 mly-0.3.4.4/mly/waveforms.py
-drwxrwxr-x   0 vasileios.skliris (44659) vasileios.skliris (44659)        0 2023-05-23 11:51:07.601215 mly-0.3.4.4/mly.egg-info/
--rw-rw-r--   0 vasileios.skliris (44659) vasileios.skliris (44659)      499 2023-05-23 11:51:07.000000 mly-0.3.4.4/mly.egg-info/PKG-INFO
--rw-rw-r--   0 vasileios.skliris (44659) vasileios.skliris (44659)      733 2023-05-23 11:51:07.000000 mly-0.3.4.4/mly.egg-info/SOURCES.txt
--rw-rw-r--   0 vasileios.skliris (44659) vasileios.skliris (44659)        1 2023-05-23 11:51:07.000000 mly-0.3.4.4/mly.egg-info/dependency_links.txt
--rw-rw-r--   0 vasileios.skliris (44659) vasileios.skliris (44659)       96 2023-05-23 11:51:07.000000 mly-0.3.4.4/mly.egg-info/requires.txt
--rw-rw-r--   0 vasileios.skliris (44659) vasileios.skliris (44659)        4 2023-05-23 11:51:07.000000 mly-0.3.4.4/mly.egg-info/top_level.txt
--rw-rw-r--   0 vasileios.skliris (44659) vasileios.skliris (44659)       79 2023-05-23 11:51:07.618215 mly-0.3.4.4/setup.cfg
--rw-rw-r--   0 vasileios.skliris (44659) vasileios.skliris (44659)      956 2023-05-23 11:50:56.000000 mly-0.3.4.4/setup.py
+drwxrwxr-x   0 vasileios.skliris (44659) vasileios.skliris (44659)        0 2023-06-12 16:22:40.146598 mly-0.3.4.5/
+-rw-rw-r--   0 vasileios.skliris (44659) vasileios.skliris (44659)    35148 2023-05-10 08:55:19.000000 mly-0.3.4.5/LICENSE
+-rw-rw-r--   0 vasileios.skliris (44659) vasileios.skliris (44659)      499 2023-06-12 16:22:40.146598 mly-0.3.4.5/PKG-INFO
+-rw-rw-r--   0 vasileios.skliris (44659) vasileios.skliris (44659)        0 2021-01-11 16:48:33.000000 mly-0.3.4.5/README.md
+drwxrwxr-x   0 vasileios.skliris (44659) vasileios.skliris (44659)        0 2023-06-12 16:22:40.130598 mly-0.3.4.5/mly/
+-rw-rw-r--   0 vasileios.skliris (44659) vasileios.skliris (44659)  1433718 2021-05-11 10:43:11.000000 mly-0.3.4.5/mly/SRD.py
+-rw-rw-r--   0 vasileios.skliris (44659) vasileios.skliris (44659)       24 2023-05-09 14:15:39.000000 mly-0.3.4.5/mly/__init__.py
+-rw-rw-r--   0 vasileios.skliris (44659) vasileios.skliris (44659)    10219 2023-05-16 10:32:51.000000 mly-0.3.4.5/mly/createFileSystem.py
+drwxrwxr-x   0 vasileios.skliris (44659) vasileios.skliris (44659)        0 2023-06-12 16:22:40.138598 mly-0.3.4.5/mly/datatools/
+-rw-rw-r--   0 vasileios.skliris (44659) vasileios.skliris (44659)      155 2023-06-09 13:56:57.000000 mly-0.3.4.5/mly/datatools/__init__.py
+-rw-rw-r--   0 vasileios.skliris (44659) vasileios.skliris (44659)    22280 2023-05-09 14:56:02.000000 mly-0.3.4.5/mly/datatools/core.py
+-rw-rw-r--   0 vasileios.skliris (44659) vasileios.skliris (44659)    28108 2023-06-09 10:58:15.000000 mly-0.3.4.5/mly/datatools/datatools.py
+-rw-rw-r--   0 vasileios.skliris (44659) vasileios.skliris (44659)    91676 2023-06-09 11:06:25.000000 mly-0.3.4.5/mly/datatools/generator.py
+drwxrwxr-x   0 vasileios.skliris (44659) vasileios.skliris (44659)        0 2023-06-12 16:22:40.142598 mly-0.3.4.5/mly/datatools/tests/
+-rw-rw-r--   0 vasileios.skliris (44659) vasileios.skliris (44659)       24 2023-05-09 14:56:02.000000 mly-0.3.4.5/mly/datatools/tests/__init__.py
+-rw-rw-r--   0 vasileios.skliris (44659) vasileios.skliris (44659)     3438 2023-05-09 14:56:02.000000 mly-0.3.4.5/mly/datatools/tests/test_core.py
+-rw-rw-r--   0 vasileios.skliris (44659) vasileios.skliris (44659)      441 2023-05-09 14:56:02.000000 mly-0.3.4.5/mly/datatools/tests/test_datatools.py
+-rw-rw-r--   0 vasileios.skliris (44659) vasileios.skliris (44659)     4975 2023-06-09 11:10:13.000000 mly-0.3.4.5/mly/datatools/tests/test_generator.py
+-rw-rw-r--   0 vasileios.skliris (44659) vasileios.skliris (44659)    18459 2023-05-09 14:56:02.000000 mly-0.3.4.5/mly/exceptions.py
+-rw-rw-r--   0 vasileios.skliris (44659) vasileios.skliris (44659)     7770 2022-08-17 15:08:03.000000 mly-0.3.4.5/mly/mlTools.py
+-rw-rw-r--   0 vasileios.skliris (44659) vasileios.skliris (44659)     6996 2021-01-11 16:48:33.000000 mly-0.3.4.5/mly/models.py
+-rw-rw-r--   0 vasileios.skliris (44659) vasileios.skliris (44659)    12353 2023-05-04 12:56:19.000000 mly-0.3.4.5/mly/null_energy_map.py
+-rw-rw-r--   0 vasileios.skliris (44659) vasileios.skliris (44659)     7316 2023-06-09 11:13:40.000000 mly-0.3.4.5/mly/offlinefar.py
+-rw-rw-r--   0 vasileios.skliris (44659) vasileios.skliris (44659)     7797 2023-05-04 12:56:19.000000 mly-0.3.4.5/mly/plugins.py
+-rw-rw-r--   0 vasileios.skliris (44659) vasileios.skliris (44659)    10134 2023-05-04 12:56:19.000000 mly-0.3.4.5/mly/projectwave.py
+-rw-rw-r--   0 vasileios.skliris (44659) vasileios.skliris (44659)     8913 2022-03-15 16:16:40.000000 mly-0.3.4.5/mly/simulateddetectornoise.py
+drwxrwxr-x   0 vasileios.skliris (44659) vasileios.skliris (44659)        0 2023-06-12 16:22:40.145598 mly-0.3.4.5/mly/tests/
+-rw-rw-r--   0 vasileios.skliris (44659) vasileios.skliris (44659)      728 2021-10-07 09:34:45.000000 mly-0.3.4.5/mly/tests/__init__.py
+-rw-rw-r--   0 vasileios.skliris (44659) vasileios.skliris (44659)     1601 2021-10-08 08:22:16.000000 mly-0.3.4.5/mly/tests/test_init.py
+-rw-rw-r--   0 vasileios.skliris (44659) vasileios.skliris (44659)     5258 2022-03-02 09:58:19.000000 mly-0.3.4.5/mly/tests/test_tools.py
+-rw-rw-r--   0 vasileios.skliris (44659) vasileios.skliris (44659)    13014 2023-05-04 12:56:19.000000 mly-0.3.4.5/mly/tools.py
+-rw-rw-r--   0 vasileios.skliris (44659) vasileios.skliris (44659)   126803 2023-06-09 13:52:48.000000 mly-0.3.4.5/mly/validators.py
+-rw-rw-r--   0 vasileios.skliris (44659) vasileios.skliris (44659)    34282 2023-05-09 14:56:02.000000 mly-0.3.4.5/mly/waveforms.py
+drwxrwxr-x   0 vasileios.skliris (44659) vasileios.skliris (44659)        0 2023-06-12 16:22:40.135598 mly-0.3.4.5/mly.egg-info/
+-rw-rw-r--   0 vasileios.skliris (44659) vasileios.skliris (44659)      499 2023-06-12 16:22:40.000000 mly-0.3.4.5/mly.egg-info/PKG-INFO
+-rw-rw-r--   0 vasileios.skliris (44659) vasileios.skliris (44659)      733 2023-06-12 16:22:40.000000 mly-0.3.4.5/mly.egg-info/SOURCES.txt
+-rw-rw-r--   0 vasileios.skliris (44659) vasileios.skliris (44659)        1 2023-06-12 16:22:40.000000 mly-0.3.4.5/mly.egg-info/dependency_links.txt
+-rw-rw-r--   0 vasileios.skliris (44659) vasileios.skliris (44659)       96 2023-06-12 16:22:40.000000 mly-0.3.4.5/mly.egg-info/requires.txt
+-rw-rw-r--   0 vasileios.skliris (44659) vasileios.skliris (44659)        4 2023-06-12 16:22:40.000000 mly-0.3.4.5/mly.egg-info/top_level.txt
+-rw-rw-r--   0 vasileios.skliris (44659) vasileios.skliris (44659)       79 2023-06-12 16:22:40.147598 mly-0.3.4.5/setup.cfg
+-rw-rw-r--   0 vasileios.skliris (44659) vasileios.skliris (44659)      956 2023-06-12 16:21:50.000000 mly-0.3.4.5/setup.py
```

### Comparing `mly-0.3.4.4/LICENSE` & `mly-0.3.4.5/LICENSE`

 * *Files identical despite different names*

### Comparing `mly-0.3.4.4/mly/SRD.py` & `mly-0.3.4.5/mly/SRD.py`

 * *Files identical despite different names*

### Comparing `mly-0.3.4.4/mly/createFileSystem.py` & `mly-0.3.4.5/mly/createFileSystem.py`

 * *Files identical despite different names*

### Comparing `mly-0.3.4.4/mly/datatools/core.py` & `mly-0.3.4.5/mly/datatools/core.py`

 * *Files identical despite different names*

### Comparing `mly-0.3.4.4/mly/datatools/datatools.py` & `mly-0.3.4.5/mly/datatools/datatools.py`

 * *Files 6% similar despite different names*

```diff
@@ -716,33 +716,9 @@
     def exportGPS(self):
         goods =[]
         for pod in self.dataPods:
             goods.append(pod.gps)
         return goods
         
  
-    def stackDetector(self,**kwargs):
-        kwargs['size']=len(self)
-        if 'duration' not in kwargs: kwargs['duration']=self[0].duration
-        if 'fs' not in kwargs: kwargs['fs']=self[0].fs   
-        if 'detectors' not in kwargs: 
-            raise ValueError("You need to at least specify a detector")
 
-        if 'plugins' not in kwargs: kwargs['plugins']=[]
-        if 'psd' in self[0].pluginDict and 'psd' not in kwargs['plugins']: kwargs['plugins'].append('psd')
-        # if 'snr'+self[0].detectors[0] in self[0].pluginDict and 'snr' not in kwargs['plugins']: 
-        #     kwargs['plugins'].append('snr')
-        
-
-        newSet=generator(**kwargs)
-
-        for i in range(len(self)):
-            self[i].strain=np.vstack((self[i].strain,newSet[i].strain))
-            self[i].detectors+=newSet[i].detectors
-            self[i].gps+=newSet[i].gps
-            if 'psd' in kwargs['plugins']: self[i].psd+=newSet[i].psd
-            # if 'snr' in kwargs['plugins']:
-            #     for d in newSet[i].detectors:
-            #         self[i].addPlugIn(newSet[i].pluginDict['snr'+d])        
-            if 'correlation' in self[i].pluginDict:
-                self[i].addPlugIn(self[i].pluginDict['correlation'])
```

### Comparing `mly-0.3.4.4/mly/datatools/generator.py` & `mly-0.3.4.5/mly/datatools/generator.py`

 * *Files 2% similar despite different names*

```diff
@@ -254,15 +254,14 @@
     and it returns None.
 
 
 
     """
     # Integration limits for the calculation of analytical SNR
     # These values are very important for the calculation
-    print(injection_initialization)
     fl, fm=20, int(fs/2)#
 
     profile = {'H' :'aligo','L':'aligo','V':'avirgo','K':'KAGRA_Early','I':'aligo'}
 
     # Labels used in saving file
     #lab={10:'X', 100:'C', 1000:'M', 10000:'XM',100000:'CM'}  
 
@@ -2070,7 +2069,38 @@
             _=DataSet.fusion(fusionNames, sizes = sizes, save = path+finalName+str(sum(sizes)))
 
         # Deleting unnescesary file in the folder
         for file in dirlist(path):
             if (('.out' in file) or ('.py' in file)
                 or ('part_of' in file) or ('.sh' in file)):
                 os.system('rm '+path+file)
+
+
+
+
+def stackDetector(dataset,**kwargs):
+    kwargs['size']=len(dataset)
+    if 'duration' not in kwargs: kwargs['duration']=dataset[0].duration
+    if 'fs' not in kwargs: kwargs['fs']=dataset[0].fs   
+    if 'detectors' not in kwargs: 
+        raise ValueError("You need to at least specify a detector")
+
+    if 'plugins' not in kwargs: kwargs['plugins']=[]
+    if 'psd' in dataset[0].pluginDict and 'psd' not in kwargs['plugins']: kwargs['plugins'].append('psd')
+    # if 'snr'+dataset[0].detectors[0] in dataset[0].pluginDict and 'snr' not in kwargs['plugins']: 
+    #     kwargs['plugins'].append('snr')
+    
+
+    newSet=generator(**kwargs)
+
+    for i in range(len(dataset)):
+        dataset[i].strain=np.vstack((dataset[i].strain,newSet[i].strain))
+        dataset[i].detectors+=newSet[i].detectors
+        dataset[i].gps+=newSet[i].gps
+        if 'psd' in kwargs['plugins']: dataset[i].psd+=newSet[i].psd
+        # if 'snr' in kwargs['plugins']:
+        #     for d in newSet[i].detectors:
+        #         dataset[i].addPlugIn(newSet[i].pluginDict['snr'+d])        
+        if 'correlation' in dataset[i].pluginDict:
+            dataset[i].addPlugIn(dataset[i].pluginDict['correlation'])   
+            
+    return(dataset)
```

### Comparing `mly-0.3.4.4/mly/datatools/tests/test_core.py` & `mly-0.3.4.5/mly/datatools/tests/test_core.py`

 * *Files identical despite different names*

### Comparing `mly-0.3.4.4/mly/datatools/tests/test_generator.py` & `mly-0.3.4.5/mly/datatools/tests/test_generator.py`

 * *Files 4% similar despite different names*

```diff
@@ -177,9 +177,27 @@
     p = d / "hello.txt"
     p.write_text("lalalala")
     assert p.read_text() == "lalalala"
     assert len(list(tmp_path.iterdir())) == 1
 
 
 
+def test_stackDetector():
 
-# def test_injection_initialization_DataPod() 
+    keys = { 
+                "duration": 1,
+                "fs": 1024,
+                "detectors" : "V",
+                "backgroundType" :"optimal",
+                "PSDm":{"V": 32}}
+
+    podlist= []
+    for i in range(10):
+
+        pod = DataPod(np.random.randn(2,1024),fs =1024,detectors = 'HL')
+        podlist.append(pod)
+
+    S = DataSet(podlist)
+
+    S = stackDetector(S,**keys)
+
+    assert(S[0].shape == (3,1024))
```

### Comparing `mly-0.3.4.4/mly/exceptions.py` & `mly-0.3.4.5/mly/exceptions.py`

 * *Files identical despite different names*

### Comparing `mly-0.3.4.4/mly/mlTools.py` & `mly-0.3.4.5/mly/mlTools.py`

 * *Files identical despite different names*

### Comparing `mly-0.3.4.4/mly/models.py` & `mly-0.3.4.5/mly/models.py`

 * *Files identical despite different names*

### Comparing `mly-0.3.4.4/mly/null_energy_map.py` & `mly-0.3.4.5/mly/null_energy_map.py`

 * *Files identical despite different names*

### Comparing `mly-0.3.4.4/mly/offlinefar.py` & `mly-0.3.4.5/mly/offlinefar.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,13 +1,14 @@
 import tensorflow as tf
 import pandas as pd
 # Path sourcing and access to the ligo real data
 import sys
 import os
 from mly.datatools import DataPod, DataSet
+from mly.datatools.generator import stackDetector
 from mly.validators import *
 from mly.exceptions import *
 from mly.waveforms import cbc
 
 from mly.plugins import *
 # Python packages that we will need
 import numpy as np
@@ -118,15 +119,15 @@
         pod.addPlugIn(knownPlugIns('correlation_30'))
 
         podList.append(pod)
 
     dataSet = DataSet(podList)
 
     if 'V' not in detectors:
-        dataSet.stackDetector(**{ 'duration':duration
+        dataSet = stackDetector(dataSet, **{ 'duration':duration
                                         ,'fs':fs
                                         ,'detectors' : 'V'
                                         ,'windowSize':windowSize
                                         ,'backgroundType' :'optimal'
                                         ,'PSDm':{'V':32}})
 
     return dataSet
```

### Comparing `mly-0.3.4.4/mly/plugins.py` & `mly-0.3.4.5/mly/plugins.py`

 * *Files identical despite different names*

### Comparing `mly-0.3.4.4/mly/projectwave.py` & `mly-0.3.4.5/mly/projectwave.py`

 * *Files identical despite different names*

### Comparing `mly-0.3.4.4/mly/simulateddetectornoise.py` & `mly-0.3.4.5/mly/simulateddetectornoise.py`

 * *Files identical despite different names*

### Comparing `mly-0.3.4.4/mly/tests/__init__.py` & `mly-0.3.4.5/mly/tests/__init__.py`

 * *Files identical despite different names*

### Comparing `mly-0.3.4.4/mly/tests/test_init.py` & `mly-0.3.4.5/mly/tests/test_init.py`

 * *Files identical despite different names*

### Comparing `mly-0.3.4.4/mly/tests/test_tools.py` & `mly-0.3.4.5/mly/tests/test_tools.py`

 * *Files identical despite different names*

### Comparing `mly-0.3.4.4/mly/tools.py` & `mly-0.3.4.5/mly/tools.py`

 * *Files identical despite different names*

### Comparing `mly-0.3.4.4/mly/validators.py` & `mly-0.3.4.5/mly/validators.py`

 * *Files 0% similar despite different names*

```diff
@@ -8,15 +8,15 @@
 import copy
 from math import ceil
 from dqsegdb2.query import query_segments
 from gwpy.io.kerberos import kinit
 
 from .simulateddetectornoise import *
 from .tools import dirlist,  fromCategorical, correlate,internalLags,circularTimeSlides
-from .datatools import DataPod, DataSet, generator
+from .datatools import DataPod, DataSet , generator, stackDetector
 from gwpy.time import to_gps,from_gps
 from gwpy.segments import DataQualityFlag
 from gwpy.segments import Segment,SegmentList
 
 from gwpy.io.kerberos import kinit
 
 from gwpy.timeseries import TimeSeries
@@ -183,15 +183,15 @@
                                    ,maxDuration = maxDuration
                                    ,differentSignals = differentSignals
                                    ,plugins=plugins
                                    ,**kwargs)
 
             
             if 'stackDetectorDict' in kwargs:
-                DATA.stackDetector(**kwargs['stackDetectorDict'])
+                DATA = stackDetector(DATA, **kwargs['stackDetectorDict'])
                 
             #random.shuffle(DATA.dataPods)
 
 
             result[loopname].append(val)
 
             
@@ -357,15 +357,15 @@
                        ,plugins=plugins
                        ,**kwargs)
             
             DATA.add(DATA_)
         
 
         if 'stackDetectorDict' in kwargs:
-            DATA.stackDetector(**kwargs['stackDetectorDict'])
+            DATA = stackDetector(DATA, **kwargs['stackDetectorDict'])
         
         generationtime=time.time()
         print("GENERATION TIME:", generationtime-preptime)
 
         result_list=[]
         scores_collection=[]
```

### Comparing `mly-0.3.4.4/mly/waveforms.py` & `mly-0.3.4.5/mly/waveforms.py`

 * *Files identical despite different names*

### Comparing `mly-0.3.4.4/mly.egg-info/SOURCES.txt` & `mly-0.3.4.5/mly.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `mly-0.3.4.4/setup.py` & `mly-0.3.4.5/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import setuptools
 
 with open("README.md", "r") as fh:
     long_description = fh.read()
 
 setuptools.setup(
     name="mly",
-    version="0.3.4.4",
+    version="0.3.4.5",
     author="Vasileios Skliris",
     author_email='vas.skliris@gmail.com',
     description='This tool helps you create training and testing data for ML to use for gravitational wave detection.',
     long_description=long_description,
     long_description_content_type="text/markdown",
     url='http://pypi.python.org/pypi/mly/',
     packages=setuptools.find_packages(),
```

