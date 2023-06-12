# Comparing `tmp/pytranscoder-ffmpeg-2.2.6.tar.gz` & `tmp/pytranscoder-ffmpeg-2.2.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pytranscoder-ffmpeg-2.2.6.tar", last modified: Sun Apr  9 17:36:30 2023, max compression
+gzip compressed data, was "pytranscoder-ffmpeg-2.2.7.tar", last modified: Mon Jun 12 19:46:22 2023, max compression
```

## Comparing `pytranscoder-ffmpeg-2.2.6.tar` & `pytranscoder-ffmpeg-2.2.7.tar`

### file list

```diff
@@ -1,33 +1,33 @@
-drwxr-xr-x   0 mark      (1026) users      (100)        0 2023-04-09 17:36:30.765936 pytranscoder-ffmpeg-2.2.6/
--rw-r--r--   0 mark      (1026) users      (100)    14467 2023-02-02 00:59:46.000000 pytranscoder-ffmpeg-2.2.6/Cluster.md
--rw-r--r--   0 mark      (1026) users      (100)    35149 2019-03-25 22:56:14.000000 pytranscoder-ffmpeg-2.2.6/LICENSE
--rw-r--r--   0 mark      (1026) users      (100)    28729 2023-04-09 17:36:30.765936 pytranscoder-ffmpeg-2.2.6/PKG-INFO
--rw-r--r--   0 mark      (1026) users      (100)    27861 2023-02-02 00:59:46.000000 pytranscoder-ffmpeg-2.2.6/README.md
-drwxr-xr-x   0 mark      (1026) users      (100)        0 2023-04-09 17:36:30.765936 pytranscoder-ffmpeg-2.2.6/config-samples/
--rwxr-xr-x   0 mark      (1026) users      (100)     5239 2023-02-02 00:59:46.000000 pytranscoder-ffmpeg-2.2.6/config-samples/cluster-sample.yml
--rw-r--r--   0 mark      (1026) users      (100)     2392 2023-02-02 00:59:46.000000 pytranscoder-ffmpeg-2.2.6/config-samples/simple.yml
--rwxr-xr-x   0 mark      (1026) users      (100)     9941 2023-02-02 00:59:46.000000 pytranscoder-ffmpeg-2.2.6/config-samples/transcode-sample2.yml
--rw-r--r--   0 mark      (1026) users      (100)     9013 2023-02-02 00:59:46.000000 pytranscoder-ffmpeg-2.2.6/config-samples/transcode.yml
-drwxr-xr-x   0 mark      (1026) users      (100)        0 2023-04-09 17:36:30.765936 pytranscoder-ffmpeg-2.2.6/pytranscoder/
--rw-r--r--   0 mark      (1026) users      (100)      240 2023-04-09 17:00:24.000000 pytranscoder-ffmpeg-2.2.6/pytranscoder/__init__.py
--rw-r--r--   0 mark      (1026) users      (100)       59 2019-03-05 22:29:59.000000 pytranscoder-ffmpeg-2.2.6/pytranscoder/__main__.py
--rw-r--r--   0 mark      (1026) users      (100)     5251 2023-02-02 00:59:46.000000 pytranscoder-ffmpeg-2.2.6/pytranscoder/agent.py
--rw-r--r--   0 mark      (1026) users      (100)    41615 2023-04-09 17:14:18.000000 pytranscoder-ffmpeg-2.2.6/pytranscoder/cluster.py
--rw-r--r--   0 mark      (1026) users      (100)     3945 2023-04-09 17:14:18.000000 pytranscoder-ffmpeg-2.2.6/pytranscoder/config.py
--rw-r--r--   0 mark      (1026) users      (100)     5077 2023-04-09 17:14:18.000000 pytranscoder-ffmpeg-2.2.6/pytranscoder/ffmpeg.py
--rw-r--r--   0 mark      (1026) users      (100)    13121 2023-04-09 17:14:18.000000 pytranscoder-ffmpeg-2.2.6/pytranscoder/media.py
--rw-r--r--   0 mark      (1026) users      (100)     2623 2023-02-02 00:59:46.000000 pytranscoder-ffmpeg-2.2.6/pytranscoder/processor.py
--rw-r--r--   0 mark      (1026) users      (100)    10176 2023-04-09 17:14:18.000000 pytranscoder-ffmpeg-2.2.6/pytranscoder/profile.py
--rw-r--r--   0 mark      (1026) users      (100)     2736 2023-02-02 00:59:46.000000 pytranscoder-ffmpeg-2.2.6/pytranscoder/rule.py
--rw-r--r--   0 mark      (1026) users      (100)     3741 2023-04-09 17:14:18.000000 pytranscoder-ffmpeg-2.2.6/pytranscoder/template.py
--rwxr-xr-x   0 mark      (1026) users      (100)    19074 2023-04-09 17:14:18.000000 pytranscoder-ffmpeg-2.2.6/pytranscoder/transcode.py
--rw-r--r--   0 mark      (1026) users      (100)     2218 2023-04-09 17:14:18.000000 pytranscoder-ffmpeg-2.2.6/pytranscoder/utils.py
-drwxr-xr-x   0 mark      (1026) users      (100)        0 2023-04-09 17:36:30.765936 pytranscoder-ffmpeg-2.2.6/pytranscoder_ffmpeg.egg-info/
--rw-r--r--   0 mark      (1026) users      (100)    28729 2023-04-09 17:36:30.000000 pytranscoder-ffmpeg-2.2.6/pytranscoder_ffmpeg.egg-info/PKG-INFO
--rw-r--r--   0 mark      (1026) users      (100)      731 2023-04-09 17:36:30.000000 pytranscoder-ffmpeg-2.2.6/pytranscoder_ffmpeg.egg-info/SOURCES.txt
--rw-r--r--   0 mark      (1026) users      (100)        1 2023-04-09 17:36:30.000000 pytranscoder-ffmpeg-2.2.6/pytranscoder_ffmpeg.egg-info/dependency_links.txt
--rw-r--r--   0 mark      (1026) users      (100)       62 2023-04-09 17:36:30.000000 pytranscoder-ffmpeg-2.2.6/pytranscoder_ffmpeg.egg-info/entry_points.txt
--rw-r--r--   0 mark      (1026) users      (100)       20 2023-04-09 17:36:30.000000 pytranscoder-ffmpeg-2.2.6/pytranscoder_ffmpeg.egg-info/requires.txt
--rw-r--r--   0 mark      (1026) users      (100)       13 2023-04-09 17:36:30.000000 pytranscoder-ffmpeg-2.2.6/pytranscoder_ffmpeg.egg-info/top_level.txt
--rw-r--r--   0 mark      (1026) users      (100)       38 2023-04-09 17:36:30.765936 pytranscoder-ffmpeg-2.2.6/setup.cfg
--rw-r--r--   0 mark      (1026) users      (100)     1739 2023-02-02 00:59:46.000000 pytranscoder-ffmpeg-2.2.6/setup.py
+drwxr-xr-x   0 mark      (1026) users      (100)        0 2023-06-12 19:46:22.415629 pytranscoder-ffmpeg-2.2.7/
+-rw-r--r--   0 mark      (1026) users      (100)    14467 2023-02-02 00:59:46.000000 pytranscoder-ffmpeg-2.2.7/Cluster.md
+-rw-r--r--   0 mark      (1026) users      (100)    35149 2019-03-25 22:56:14.000000 pytranscoder-ffmpeg-2.2.7/LICENSE
+-rw-r--r--   0 mark      (1026) users      (100)    28729 2023-06-12 19:46:22.415629 pytranscoder-ffmpeg-2.2.7/PKG-INFO
+-rw-r--r--   0 mark      (1026) users      (100)    27861 2023-02-02 00:59:46.000000 pytranscoder-ffmpeg-2.2.7/README.md
+drwxr-xr-x   0 mark      (1026) users      (100)        0 2023-06-12 19:46:22.411628 pytranscoder-ffmpeg-2.2.7/config-samples/
+-rwxr-xr-x   0 mark      (1026) users      (100)     5239 2023-02-02 00:59:46.000000 pytranscoder-ffmpeg-2.2.7/config-samples/cluster-sample.yml
+-rw-r--r--   0 mark      (1026) users      (100)     2392 2023-02-02 00:59:46.000000 pytranscoder-ffmpeg-2.2.7/config-samples/simple.yml
+-rwxr-xr-x   0 mark      (1026) users      (100)     9941 2023-02-02 00:59:46.000000 pytranscoder-ffmpeg-2.2.7/config-samples/transcode-sample2.yml
+-rw-r--r--   0 mark      (1026) users      (100)     9013 2023-02-02 00:59:46.000000 pytranscoder-ffmpeg-2.2.7/config-samples/transcode.yml
+drwxr-xr-x   0 mark      (1026) users      (100)        0 2023-06-12 19:46:22.415629 pytranscoder-ffmpeg-2.2.7/pytranscoder/
+-rw-r--r--   0 mark      (1026) users      (100)      240 2023-06-12 19:45:28.000000 pytranscoder-ffmpeg-2.2.7/pytranscoder/__init__.py
+-rw-r--r--   0 mark      (1026) users      (100)       59 2019-03-05 22:29:59.000000 pytranscoder-ffmpeg-2.2.7/pytranscoder/__main__.py
+-rw-r--r--   0 mark      (1026) users      (100)     5251 2023-02-02 00:59:46.000000 pytranscoder-ffmpeg-2.2.7/pytranscoder/agent.py
+-rw-r--r--   0 mark      (1026) users      (100)    41462 2023-06-12 03:04:35.000000 pytranscoder-ffmpeg-2.2.7/pytranscoder/cluster.py
+-rw-r--r--   0 mark      (1026) users      (100)     3945 2023-04-09 17:14:18.000000 pytranscoder-ffmpeg-2.2.7/pytranscoder/config.py
+-rw-r--r--   0 mark      (1026) users      (100)     5077 2023-04-09 17:14:18.000000 pytranscoder-ffmpeg-2.2.7/pytranscoder/ffmpeg.py
+-rw-r--r--   0 mark      (1026) users      (100)    13121 2023-04-09 17:14:18.000000 pytranscoder-ffmpeg-2.2.7/pytranscoder/media.py
+-rw-r--r--   0 mark      (1026) users      (100)     2623 2023-02-02 00:59:46.000000 pytranscoder-ffmpeg-2.2.7/pytranscoder/processor.py
+-rw-r--r--   0 mark      (1026) users      (100)    10176 2023-04-09 17:14:18.000000 pytranscoder-ffmpeg-2.2.7/pytranscoder/profile.py
+-rw-r--r--   0 mark      (1026) users      (100)     2736 2023-02-02 00:59:46.000000 pytranscoder-ffmpeg-2.2.7/pytranscoder/rule.py
+-rw-r--r--   0 mark      (1026) users      (100)     3900 2023-06-12 00:26:58.000000 pytranscoder-ffmpeg-2.2.7/pytranscoder/template.py
+-rwxr-xr-x   0 mark      (1026) users      (100)    19074 2023-04-11 02:35:50.000000 pytranscoder-ffmpeg-2.2.7/pytranscoder/transcode.py
+-rw-r--r--   0 mark      (1026) users      (100)     2200 2023-04-11 02:38:10.000000 pytranscoder-ffmpeg-2.2.7/pytranscoder/utils.py
+drwxr-xr-x   0 mark      (1026) users      (100)        0 2023-06-12 19:46:22.415629 pytranscoder-ffmpeg-2.2.7/pytranscoder_ffmpeg.egg-info/
+-rw-r--r--   0 mark      (1026) users      (100)    28729 2023-06-12 19:46:22.000000 pytranscoder-ffmpeg-2.2.7/pytranscoder_ffmpeg.egg-info/PKG-INFO
+-rw-r--r--   0 mark      (1026) users      (100)      731 2023-06-12 19:46:22.000000 pytranscoder-ffmpeg-2.2.7/pytranscoder_ffmpeg.egg-info/SOURCES.txt
+-rw-r--r--   0 mark      (1026) users      (100)        1 2023-06-12 19:46:22.000000 pytranscoder-ffmpeg-2.2.7/pytranscoder_ffmpeg.egg-info/dependency_links.txt
+-rw-r--r--   0 mark      (1026) users      (100)       62 2023-06-12 19:46:22.000000 pytranscoder-ffmpeg-2.2.7/pytranscoder_ffmpeg.egg-info/entry_points.txt
+-rw-r--r--   0 mark      (1026) users      (100)       20 2023-06-12 19:46:22.000000 pytranscoder-ffmpeg-2.2.7/pytranscoder_ffmpeg.egg-info/requires.txt
+-rw-r--r--   0 mark      (1026) users      (100)       13 2023-06-12 19:46:22.000000 pytranscoder-ffmpeg-2.2.7/pytranscoder_ffmpeg.egg-info/top_level.txt
+-rw-r--r--   0 mark      (1026) users      (100)       38 2023-06-12 19:46:22.415629 pytranscoder-ffmpeg-2.2.7/setup.cfg
+-rw-r--r--   0 mark      (1026) users      (100)     1739 2023-02-02 00:59:46.000000 pytranscoder-ffmpeg-2.2.7/setup.py
```

### Comparing `pytranscoder-ffmpeg-2.2.6/Cluster.md` & `pytranscoder-ffmpeg-2.2.7/Cluster.md`

 * *Files identical despite different names*

### Comparing `pytranscoder-ffmpeg-2.2.6/LICENSE` & `pytranscoder-ffmpeg-2.2.7/LICENSE`

 * *Files identical despite different names*

### Comparing `pytranscoder-ffmpeg-2.2.6/PKG-INFO` & `pytranscoder-ffmpeg-2.2.7/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pytranscoder-ffmpeg
-Version: 2.2.6
+Version: 2.2.7
 Summary: A ffmpeg workflow manager for transcoding
 Home-page: https://github.com/mlsmithjr/transcoder
 Author: Marshall L Smith Jr
 Author-email: marshallsmithjr@gmail.com
 License: UNKNOWN
 Keywords: ffmpeg qsv cuda encode transcode
 Platform: UNKNOWN
```

### Comparing `pytranscoder-ffmpeg-2.2.6/README.md` & `pytranscoder-ffmpeg-2.2.7/README.md`

 * *Files identical despite different names*

### Comparing `pytranscoder-ffmpeg-2.2.6/config-samples/cluster-sample.yml` & `pytranscoder-ffmpeg-2.2.7/config-samples/cluster-sample.yml`

 * *Files identical despite different names*

### Comparing `pytranscoder-ffmpeg-2.2.6/config-samples/simple.yml` & `pytranscoder-ffmpeg-2.2.7/config-samples/simple.yml`

 * *Files identical despite different names*

### Comparing `pytranscoder-ffmpeg-2.2.6/config-samples/transcode-sample2.yml` & `pytranscoder-ffmpeg-2.2.7/config-samples/transcode-sample2.yml`

 * *Files identical despite different names*

### Comparing `pytranscoder-ffmpeg-2.2.6/config-samples/transcode.yml` & `pytranscoder-ffmpeg-2.2.7/config-samples/transcode.yml`

 * *Files identical despite different names*

### Comparing `pytranscoder-ffmpeg-2.2.6/pytranscoder/agent.py` & `pytranscoder-ffmpeg-2.2.7/pytranscoder/agent.py`

 * *Files identical despite different names*

### Comparing `pytranscoder-ffmpeg-2.2.6/pytranscoder/cluster.py` & `pytranscoder-ffmpeg-2.2.7/pytranscoder/cluster.py`

 * *Files 1% similar despite different names*

```diff
@@ -43,15 +43,15 @@
         return self.props['ip']
 
     @property
     def os(self):
         return self.props['os']
 
     @property
-    def profiles(self) -> [str]:
+    def profiles(self) -> List[str]:
         return self.props.get('profiles', None)
 
     @property
     def working_dir(self):
         return self.props.get('working_dir', None)
 
     @property
@@ -70,15 +70,15 @@
     def has_path_subst(self):
         return 'path-substitutions' in self.props
 
     @property
     def queues(self) -> Dict:
         return self.props.get('queues', {'_default': 1})
 
-    def substitute_paths(self, in_path, out_path) -> (str, str):
+    def substitute_paths(self, in_path, out_path):
         lst = self.props['path-substitutions']
         for item in lst:
             src, dest = item.split(' ')
             if src in in_path:
                 in_path = in_path.replace(src, dest)
                 out_path = out_path.replace(src, dest)
                 break
@@ -195,14 +195,15 @@
             self.lock.release()
 
     def testrun(self):
         pass
 
     def converted_path(self, path):
         if self.props.is_windows():
+            path = '"' + path + '"'
             return str(PureWindowsPath(path))
         else:
             return str(PosixPath(path))
 
     def ssh_cmd(self):
         return [self._manager.ssh, self.props.user + '@' + self.props.ip]
 
@@ -574,18 +575,16 @@
                     #                    remote_inpath = self.converted_path(remote_inpath)
                     remote_outpath = remote_outpath.replace("/", "\\")
                     remote_inpath = remote_inpath.replace("/", "\\")
                     if get_local_os_type() == "linux":
                         remote_outpath = remote_outpath.replace(r"\\", "\\")
                         remote_inpath = remote_inpath.replace(r"\\", "\\")
                     self.run_process([*ssh_cmd, f'del "{remote_outpath}"'])
-                    self.run_process([*ssh_cmd, f'del "{remote_inpath}"'])
                 else:
                     self.run_process([*ssh_cmd, f'"rm {remote_outpath}"'])
-                    self.run_process([*ssh_cmd, f'"rm {remote_inpath}"'])
 
             finally:
                 self.queue.task_done()
 
 
 class MountedManagedHost(ManagedHost):
     """Implementation of a mounted host worker thread"""
@@ -925,15 +924,15 @@
                         if not _h.validate_settings():
                             sys.exit(1)
                         self.hosts.append(_h)
 
             else:
                 print(crayons.red(f'Unknown cluster host type "{hosttype}" - skipping'))
 
-    def enqueue(self, file, forced_directive: Optional[str]) -> (str, Optional[EncodeJob]):
+    def enqueue(self, file, forced_directive: Optional[str]):
         """Add a media file to this cluster queue.
            This is different than in local mode in that we only care about handling skips here.
            The profile will be selected once a host is assigned to the work
         """
 
         path = os.path.abspath(file)  # convert to full path so that rule filtering can work
         if pytranscoder.verbose:
```

### Comparing `pytranscoder-ffmpeg-2.2.6/pytranscoder/config.py` & `pytranscoder-ffmpeg-2.2.7/pytranscoder/config.py`

 * *Files identical despite different names*

### Comparing `pytranscoder-ffmpeg-2.2.6/pytranscoder/ffmpeg.py` & `pytranscoder-ffmpeg-2.2.7/pytranscoder/ffmpeg.py`

 * *Files identical despite different names*

### Comparing `pytranscoder-ffmpeg-2.2.6/pytranscoder/media.py` & `pytranscoder-ffmpeg-2.2.7/pytranscoder/media.py`

 * *Files identical despite different names*

### Comparing `pytranscoder-ffmpeg-2.2.6/pytranscoder/processor.py` & `pytranscoder-ffmpeg-2.2.7/pytranscoder/processor.py`

 * *Files identical despite different names*

### Comparing `pytranscoder-ffmpeg-2.2.6/pytranscoder/profile.py` & `pytranscoder-ffmpeg-2.2.7/pytranscoder/profile.py`

 * *Files identical despite different names*

### Comparing `pytranscoder-ffmpeg-2.2.6/pytranscoder/rule.py` & `pytranscoder-ffmpeg-2.2.7/pytranscoder/rule.py`

 * *Files identical despite different names*

### Comparing `pytranscoder-ffmpeg-2.2.6/pytranscoder/template.py` & `pytranscoder-ffmpeg-2.2.7/pytranscoder/template.py`

 * *Files 2% similar despite different names*

```diff
@@ -19,30 +19,34 @@
 
         self.cli = template["cli"]
 
     def input_options_list(self) -> List[str]:
         opt = self.cli.get("input-options", None)
         return opt or []
 
-    def output_options_list(self, config, mixins: Optional = None) -> List[str]:
+    def output_options_list(self, config, mixins: Optional[List] = None) -> List[str]:
         opts = []
         vopt = self.cli.get("video-codec", None) or ""
         opts.extend(vopt.split(" "))
         aopt = self.cli.get("audio-codec", None) or ""
         opts.extend(aopt.split(" "))
         sopt = self.cli.get("subtitles", None) or ""
         opts.extend(sopt.split(" "))
 
         return opts
 
     def get(self, key: str):
         return self.template.get(key, None)
 
     def extension(self) -> str:
-        return self.template['extension']
+        ext = self.template.get('extension', None)
+        if not ext:
+            print(f"Required value for 'extension' missing in template {self.name}")
+            exit(1)
+        return ext
 
     def name(self) -> str:
         return self._name
 
     def queue_name(self) -> str:
         return self.template.get('queue', None)
```

### Comparing `pytranscoder-ffmpeg-2.2.6/pytranscoder/transcode.py` & `pytranscoder-ffmpeg-2.2.7/pytranscoder/transcode.py`

 * *Files identical despite different names*

### Comparing `pytranscoder-ffmpeg-2.2.6/pytranscoder/utils.py` & `pytranscoder-ffmpeg-2.2.7/pytranscoder/utils.py`

 * *Files 9% similar despite different names*

```diff
@@ -23,15 +23,15 @@
     if pct_savings < pct_threshold:
         return False
     return True
 
 
 def files_from_file(queuepath) -> list:
     if not os.path.exists(queuepath):
-        print(f'Queue file {queuepath} not found')
+        print(f'Nothing to do.')
         return []
     with open(queuepath, 'r') as qf:
         _files = [fn.rstrip() for fn in qf.readlines()]
         return _files
 
 
 def get_local_os_type():
```

### Comparing `pytranscoder-ffmpeg-2.2.6/pytranscoder_ffmpeg.egg-info/PKG-INFO` & `pytranscoder-ffmpeg-2.2.7/pytranscoder_ffmpeg.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pytranscoder-ffmpeg
-Version: 2.2.6
+Version: 2.2.7
 Summary: A ffmpeg workflow manager for transcoding
 Home-page: https://github.com/mlsmithjr/transcoder
 Author: Marshall L Smith Jr
 Author-email: marshallsmithjr@gmail.com
 License: UNKNOWN
 Keywords: ffmpeg qsv cuda encode transcode
 Platform: UNKNOWN
```

### Comparing `pytranscoder-ffmpeg-2.2.6/pytranscoder_ffmpeg.egg-info/SOURCES.txt` & `pytranscoder-ffmpeg-2.2.7/pytranscoder_ffmpeg.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `pytranscoder-ffmpeg-2.2.6/setup.py` & `pytranscoder-ffmpeg-2.2.7/setup.py`

 * *Files identical despite different names*

