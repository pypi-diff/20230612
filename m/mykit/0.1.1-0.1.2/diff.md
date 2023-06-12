# Comparing `tmp/mykit-0.1.1.tar.gz` & `tmp/mykit-0.1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mykit-0.1.1.tar", last modified: Mon Jun 12 10:55:28 2023, max compression
+gzip compressed data, was "mykit-0.1.2.tar", last modified: Mon Jun 12 12:16:32 2023, max compression
```

## Comparing `mykit-0.1.1.tar` & `mykit-0.1.2.tar`

### file list

```diff
@@ -1,60 +1,47 @@
-drwxrwxrwx   0        0        0        0 2023-06-12 10:55:28.651495 mykit-0.1.1/
--rw-rw-rw-   0        0        0     1097 2023-04-10 22:01:23.000000 mykit-0.1.1/LICENSE
--rw-rw-rw-   0        0        0     3848 2023-06-12 10:55:28.601485 mykit-0.1.1/PKG-INFO
--rw-rw-rw-   0        0        0     3344 2023-06-12 09:13:41.000000 mykit-0.1.1/README.md
-drwxrwxrwx   0        0        0        0 2023-06-12 10:55:28.171458 mykit-0.1.1/mykit.egg-info/
--rw-rw-rw-   0        0        0     3848 2023-06-12 10:55:27.000000 mykit-0.1.1/mykit.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      969 2023-06-12 10:55:27.000000 mykit-0.1.1/mykit.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-06-12 10:55:27.000000 mykit-0.1.1/mykit.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        7 2023-06-12 10:55:27.000000 mykit-0.1.1/mykit.egg-info/top_level.txt
-drwxrwxrwx   0        0        0        0 2023-06-12 10:55:28.181461 mykit-0.1.1/mykitx/
--rw-rw-rw-   0        0        0      564 2023-06-12 08:43:01.000000 mykit-0.1.1/mykitx/__init__.py
--rw-rw-rw-   0        0        0      326 2023-05-27 14:47:02.000000 mykit-0.1.1/mykitx/__main__.py
-drwxrwxrwx   0        0        0        0 2023-06-12 10:55:27.992421 mykit-0.1.1/mykitx/kit/
-drwxrwxrwx   0        0        0        0 2023-06-12 10:55:28.194463 mykit-0.1.1/mykitx/kit/color/
--rw-rw-rw-   0        0        0     3655 2023-06-11 17:23:45.000000 mykit-0.1.1/mykitx/kit/color/__init__.py
--rw-rw-rw-   0        0        0     5245 2023-06-11 17:48:09.000000 mykit-0.1.1/mykitx/kit/color/test_color.py
-drwxrwxrwx   0        0        0        0 2023-06-12 10:55:28.203469 mykit-0.1.1/mykitx/kit/ffmpeg/
--rw-rw-rw-   0        0        0     5787 2023-05-07 02:46:01.000000 mykit-0.1.1/mykitx/kit/ffmpeg/__init__.py
-drwxrwxrwx   0        0        0        0 2023-06-12 10:55:28.210467 mykit-0.1.1/mykitx/kit/graph/
--rw-rw-rw-   0        0        0        0 2023-05-04 08:26:58.000000 mykit-0.1.1/mykitx/kit/graph/__init__.py
-drwxrwxrwx   0        0        0        0 2023-06-12 10:55:28.227480 mykit-0.1.1/mykitx/kit/graph/graph2d/
--rw-rw-rw-   0        0        0     6021 2023-05-06 16:31:01.000000 mykit-0.1.1/mykitx/kit/graph/graph2d/__init__.py
--rw-rw-rw-   0        0        0    16620 2023-05-15 09:41:37.000000 mykit-0.1.1/mykitx/kit/graph/graph2d/v2.py
-drwxrwxrwx   0        0        0        0 2023-06-12 10:55:27.937407 mykit-0.1.1/mykitx/kit/gui/
-drwxrwxrwx   0        0        0        0 2023-06-12 10:55:28.278004 mykit-0.1.1/mykitx/kit/gui/button/
--rw-rw-rw-   0        0        0     7403 2023-05-13 04:57:02.000000 mykit-0.1.1/mykitx/kit/gui/button/__init__.py
--rw-rw-rw-   0        0        0    11489 2023-05-20 15:47:14.000000 mykit-0.1.1/mykitx/kit/gui/button/v2.py
--rw-rw-rw-   0        0        0    13441 2023-05-27 15:38:04.000000 mykit-0.1.1/mykitx/kit/gui/button/v3.py
-drwxrwxrwx   0        0        0        0 2023-06-12 10:55:28.299007 mykit-0.1.1/mykitx/kit/gui/label/
--rw-rw-rw-   0        0        0     6076 2023-05-12 14:09:30.000000 mykit-0.1.1/mykitx/kit/gui/label/__init__.py
--rw-rw-rw-   0        0        0     9542 2023-05-27 15:38:15.000000 mykit-0.1.1/mykitx/kit/gui/label/v2.py
-drwxrwxrwx   0        0        0        0 2023-06-12 10:55:28.304010 mykit-0.1.1/mykitx/kit/gui/shape/
--rw-rw-rw-   0        0        0     4224 2023-05-13 04:59:18.000000 mykit-0.1.1/mykitx/kit/gui/shape/__init__.py
-drwxrwxrwx   0        0        0        0 2023-06-12 10:55:28.342126 mykit-0.1.1/mykitx/kit/gui/slider/
--rw-rw-rw-   0        0        0    20347 2023-05-18 07:01:02.000000 mykit-0.1.1/mykitx/kit/gui/slider/__init__.py
--rw-rw-rw-   0        0        0    28699 2023-05-27 18:19:56.000000 mykit-0.1.1/mykitx/kit/gui/slider/v2.py
-drwxrwxrwx   0        0        0        0 2023-06-12 10:55:28.362229 mykit-0.1.1/mykitx/kit/keycrate/
--rw-rw-rw-   0        0        0     6467 2023-05-18 13:56:54.000000 mykit-0.1.1/mykitx/kit/keycrate/__init__.py
-drwxrwxrwx   0        0        0        0 2023-06-12 10:55:28.429441 mykit-0.1.1/mykitx/kit/maths/
--rw-rw-rw-   0        0        0     2802 2023-06-11 17:45:01.000000 mykit-0.1.1/mykitx/kit/maths/__init__.py
--rw-rw-rw-   0        0        0     3544 2023-06-11 18:25:53.000000 mykit-0.1.1/mykitx/kit/maths/test_maths.py
-drwxrwxrwx   0        0        0        0 2023-06-12 10:55:27.952401 mykit-0.1.1/mykitx/kit/neuralnet/
-drwxrwxrwx   0        0        0        0 2023-06-12 10:55:28.443452 mykit-0.1.1/mykitx/kit/neuralnet/dense/
--rw-rw-rw-   0        0        0     7317 2023-05-15 21:04:54.000000 mykit-0.1.1/mykitx/kit/neuralnet/dense/__init__.py
-drwxrwxrwx   0        0        0        0 2023-06-12 10:55:28.450449 mykit-0.1.1/mykitx/kit/neuralnet/genetic/
--rw-rw-rw-   0        0        0    15106 2023-05-27 08:37:35.000000 mykit-0.1.1/mykitx/kit/neuralnet/genetic/__init__.py
-drwxrwxrwx   0        0        0        0 2023-06-12 10:55:28.478459 mykit-0.1.1/mykitx/kit/noise/
--rw-rw-rw-   0        0        0     3039 2023-05-06 18:30:49.000000 mykit-0.1.1/mykitx/kit/noise/__init__.py
-drwxrwxrwx   0        0        0        0 2023-06-12 10:55:28.492459 mykit-0.1.1/mykitx/kit/path/
--rw-rw-rw-   0        0        0     4253 2023-05-18 13:55:09.000000 mykit-0.1.1/mykitx/kit/path/__init__.py
-drwxrwxrwx   0        0        0        0 2023-06-12 10:55:28.548471 mykit-0.1.1/mykitx/kit/quick_visual/
--rw-rw-rw-   0        0        0      838 2023-05-06 12:20:28.000000 mykit-0.1.1/mykitx/kit/quick_visual/plot2d.py
-drwxrwxrwx   0        0        0        0 2023-06-12 10:55:28.560475 mykit-0.1.1/mykitx/kit/text/
--rw-rw-rw-   0        0        0      403 2023-06-11 18:43:02.000000 mykit-0.1.1/mykitx/kit/text/__init__.py
-drwxrwxrwx   0        0        0        0 2023-06-12 10:55:28.570479 mykit-0.1.1/mykitx/kit/timelib/
--rw-rw-rw-   0        0        0     2582 2023-06-12 08:42:32.000000 mykit-0.1.1/mykitx/kit/timelib/__init__.py
-drwxrwxrwx   0        0        0        0 2023-06-12 10:55:28.574478 mykit-0.1.1/mykitx/kit/utils/
--rw-rw-rw-   0        0        0     3156 2023-05-18 13:20:09.000000 mykit-0.1.1/mykitx/kit/utils/__init__.py
--rw-rw-rw-   0        0        0      582 2023-06-12 10:54:42.000000 mykit-0.1.1/pyproject.toml
--rw-rw-rw-   0        0        0       42 2023-06-12 10:55:28.652498 mykit-0.1.1/setup.cfg
+drwxrwxrwx   0        0        0        0 2023-06-12 12:16:32.890277 mykit-0.1.2/
+-rw-rw-rw-   0        0        0     1097 2023-04-10 22:01:23.000000 mykit-0.1.2/LICENSE
+-rw-rw-rw-   0        0        0     4701 2023-06-12 12:16:32.886274 mykit-0.1.2/PKG-INFO
+-rw-rw-rw-   0        0        0     4197 2023-06-12 12:12:50.000000 mykit-0.1.2/README.md
+drwxrwxrwx   0        0        0        0 2023-06-12 12:16:32.648218 mykit-0.1.2/mykit/
+-rw-rw-rw-   0        0        0      134 2023-06-12 12:04:04.000000 mykit-0.1.2/mykit/__init__.py
+-rw-rw-rw-   0        0        0      326 2023-05-27 14:47:02.000000 mykit-0.1.2/mykit/__main__.py
+drwxrwxrwx   0        0        0        0 2023-06-12 12:16:32.793257 mykit-0.1.2/mykit/kit/
+-rw-rw-rw-   0        0        0     3655 2023-06-11 17:23:45.000000 mykit-0.1.2/mykit/kit/color.py
+-rw-rw-rw-   0        0        0     5809 2023-06-12 11:57:08.000000 mykit-0.1.2/mykit/kit/ffmpeg.py
+drwxrwxrwx   0        0        0        0 2023-06-12 12:16:32.804262 mykit-0.1.2/mykit/kit/graph/
+-rw-rw-rw-   0        0        0    16521 2023-06-12 12:03:05.000000 mykit-0.1.2/mykit/kit/graph/graph2d.py
+drwxrwxrwx   0        0        0        0 2023-06-12 12:16:32.487175 mykit-0.1.2/mykit/kit/gui/
+drwxrwxrwx   0        0        0        0 2023-06-12 12:16:32.827263 mykit-0.1.2/mykit/kit/gui/button/
+-rw-rw-rw-   0        0        0     7403 2023-05-13 04:57:02.000000 mykit-0.1.2/mykit/kit/gui/button/__init__.py
+-rw-rw-rw-   0        0        0    11489 2023-05-20 15:47:14.000000 mykit-0.1.2/mykit/kit/gui/button/v2.py
+-rw-rw-rw-   0        0        0    13441 2023-05-27 15:38:04.000000 mykit-0.1.2/mykit/kit/gui/button/v3.py
+drwxrwxrwx   0        0        0        0 2023-06-12 12:16:32.840271 mykit-0.1.2/mykit/kit/gui/label/
+-rw-rw-rw-   0        0        0     6076 2023-05-12 14:09:30.000000 mykit-0.1.2/mykit/kit/gui/label/__init__.py
+-rw-rw-rw-   0        0        0     9542 2023-05-27 15:38:15.000000 mykit-0.1.2/mykit/kit/gui/label/v2.py
+drwxrwxrwx   0        0        0        0 2023-06-12 12:16:32.846276 mykit-0.1.2/mykit/kit/gui/shape/
+-rw-rw-rw-   0        0        0     4224 2023-05-13 04:59:18.000000 mykit-0.1.2/mykit/kit/gui/shape/__init__.py
+drwxrwxrwx   0        0        0        0 2023-06-12 12:16:32.861268 mykit-0.1.2/mykit/kit/gui/slider/
+-rw-rw-rw-   0        0        0    20347 2023-05-18 07:01:02.000000 mykit-0.1.2/mykit/kit/gui/slider/__init__.py
+-rw-rw-rw-   0        0        0    28699 2023-05-27 18:19:56.000000 mykit-0.1.2/mykit/kit/gui/slider/v2.py
+drwxrwxrwx   0        0        0        0 2023-06-12 12:16:32.867270 mykit-0.1.2/mykit/kit/keycrate/
+-rw-rw-rw-   0        0        0     6467 2023-05-18 13:56:54.000000 mykit-0.1.2/mykit/kit/keycrate/__init__.py
+-rw-rw-rw-   0        0        0     2741 2023-06-12 12:12:05.000000 mykit-0.1.2/mykit/kit/math.py
+drwxrwxrwx   0        0        0        0 2023-06-12 12:16:32.502184 mykit-0.1.2/mykit/kit/neuralnet/
+drwxrwxrwx   0        0        0        0 2023-06-12 12:16:32.875275 mykit-0.1.2/mykit/kit/neuralnet/dense/
+-rw-rw-rw-   0        0        0     7317 2023-05-15 21:04:54.000000 mykit-0.1.2/mykit/kit/neuralnet/dense/__init__.py
+drwxrwxrwx   0        0        0        0 2023-06-12 12:16:32.878272 mykit-0.1.2/mykit/kit/neuralnet/genetic/
+-rw-rw-rw-   0        0        0    15106 2023-05-27 08:37:35.000000 mykit-0.1.2/mykit/kit/neuralnet/genetic/__init__.py
+-rw-rw-rw-   0        0        0     3039 2023-05-06 18:30:49.000000 mykit-0.1.2/mykit/kit/noise.py
+-rw-rw-rw-   0        0        0     4253 2023-05-18 13:55:09.000000 mykit-0.1.2/mykit/kit/path.py
+drwxrwxrwx   0        0        0        0 2023-06-12 12:16:32.882273 mykit-0.1.2/mykit/kit/quick_visual/
+-rw-rw-rw-   0        0        0      838 2023-05-06 12:20:28.000000 mykit-0.1.2/mykit/kit/quick_visual/plot2d.py
+-rw-rw-rw-   0        0        0      403 2023-06-11 18:43:02.000000 mykit-0.1.2/mykit/kit/text.py
+-rw-rw-rw-   0        0        0     2453 2023-06-12 11:34:47.000000 mykit-0.1.2/mykit/kit/time.py
+-rw-rw-rw-   0        0        0     3156 2023-05-18 13:20:09.000000 mykit-0.1.2/mykit/kit/utils.py
+drwxrwxrwx   0        0        0        0 2023-06-12 12:16:32.727238 mykit-0.1.2/mykit.egg-info/
+-rw-rw-rw-   0        0        0     4701 2023-06-12 12:16:32.000000 mykit-0.1.2/mykit.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      739 2023-06-12 12:16:32.000000 mykit-0.1.2/mykit.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-06-12 12:16:32.000000 mykit-0.1.2/mykit.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        6 2023-06-12 12:16:32.000000 mykit-0.1.2/mykit.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0      582 2023-06-12 12:03:36.000000 mykit-0.1.2/pyproject.toml
+-rw-rw-rw-   0        0        0       42 2023-06-12 12:16:32.891279 mykit-0.1.2/setup.cfg
```

### Comparing `mykit-0.1.1/LICENSE` & `mykit-0.1.2/LICENSE`

 * *Files identical despite different names*

### Comparing `mykit-0.1.1/mykit.egg-info/SOURCES.txt` & `mykit-0.1.2/mykit.egg-info/SOURCES.txt`

 * *Files 25% similar despite different names*

```diff
@@ -1,34 +1,30 @@
 LICENSE
 README.md
 pyproject.toml
+mykit/__init__.py
+mykit/__main__.py
 mykit.egg-info/PKG-INFO
 mykit.egg-info/SOURCES.txt
 mykit.egg-info/dependency_links.txt
 mykit.egg-info/top_level.txt
-mykitx/__init__.py
-mykitx/__main__.py
-mykitx/kit/color/__init__.py
-mykitx/kit/color/test_color.py
-mykitx/kit/ffmpeg/__init__.py
-mykitx/kit/graph/__init__.py
-mykitx/kit/graph/graph2d/__init__.py
-mykitx/kit/graph/graph2d/v2.py
-mykitx/kit/gui/button/__init__.py
-mykitx/kit/gui/button/v2.py
-mykitx/kit/gui/button/v3.py
-mykitx/kit/gui/label/__init__.py
-mykitx/kit/gui/label/v2.py
-mykitx/kit/gui/shape/__init__.py
-mykitx/kit/gui/slider/__init__.py
-mykitx/kit/gui/slider/v2.py
-mykitx/kit/keycrate/__init__.py
-mykitx/kit/maths/__init__.py
-mykitx/kit/maths/test_maths.py
-mykitx/kit/neuralnet/dense/__init__.py
-mykitx/kit/neuralnet/genetic/__init__.py
-mykitx/kit/noise/__init__.py
-mykitx/kit/path/__init__.py
-mykitx/kit/quick_visual/plot2d.py
-mykitx/kit/text/__init__.py
-mykitx/kit/timelib/__init__.py
-mykitx/kit/utils/__init__.py
+mykit/kit/color.py
+mykit/kit/ffmpeg.py
+mykit/kit/math.py
+mykit/kit/noise.py
+mykit/kit/path.py
+mykit/kit/text.py
+mykit/kit/time.py
+mykit/kit/utils.py
+mykit/kit/graph/graph2d.py
+mykit/kit/gui/button/__init__.py
+mykit/kit/gui/button/v2.py
+mykit/kit/gui/button/v3.py
+mykit/kit/gui/label/__init__.py
+mykit/kit/gui/label/v2.py
+mykit/kit/gui/shape/__init__.py
+mykit/kit/gui/slider/__init__.py
+mykit/kit/gui/slider/v2.py
+mykit/kit/keycrate/__init__.py
+mykit/kit/neuralnet/dense/__init__.py
+mykit/kit/neuralnet/genetic/__init__.py
+mykit/kit/quick_visual/plot2d.py
```

### Comparing `mykit-0.1.1/mykitx/kit/color/__init__.py` & `mykit-0.1.2/mykit/kit/color.py`

 * *Files identical despite different names*

### Comparing `mykit-0.1.1/mykitx/kit/ffmpeg/__init__.py` & `mykit-0.1.2/mykit/kit/ffmpeg.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,9 +1,9 @@
-import re
-import subprocess as sp
+import re as _re
+import subprocess as _sp
 
 
 def get_resolution(input_path: str, ffprobe_path: str) -> tuple[int, int]:
     """
     image/video resolution.
 
     `input_path`: absolute path to the input file
@@ -15,95 +15,95 @@
         ffprobe_path,
         '-v', 'error',
         '-select_streams', 'v',
         '-of', 'csv=p=0',
         '-show_entries', 'stream=width,height',
         input_path
     ]
-    res = sp.run(cmd, capture_output=True, text=True)
-    match = re.search(r'^(\d+),(\d+)$', res.stdout.strip())
+    res = _sp.run(cmd, capture_output=True, text=True)
+    match = _re.search(r'^(\d+),(\d+)$', res.stdout.strip())
     width, height = int(match.group(1)), int(match.group(2))
     return width, height
 
 
 def get_audio_sample_rate(input_path: str, ffprobe_path: str) -> float:
-    res = sp.check_output(
+    res = _sp.check_output(
         [
             ffprobe_path, '-v', 'error',
             '-select_streams', 'a',
             '-of', 'csv=p=0',
             '-show_entries', 'stream=sample_rate',
             input_path
         ],
-        stderr=sp.STDOUT, text=True
+        stderr=_sp.STDOUT, text=True
     )
-    reg = re.match(r'^(?P<v>\d+(?:\.\d+)?)', res)
+    reg = _re.match(r'^(?P<v>\d+(?:\.\d+)?)', res)
     return float(reg.group('v'))
 
 
 def get_vid_dur(file: str, ffprobe: str, /) -> float:
     """
     Get video duration in secs.
     Note, video and audio might be different.
     `file`: full path to the input file
     `ffprobe`: ffprobe.exe full path
     """
-    stdout = sp.check_output(
+    stdout = _sp.check_output(
         [
             ffprobe, '-v', 'error',
             '-select_streams', 'v',
             '-of', 'csv=p=0',
             '-show_entries', 'stream=duration',
             file
         ],
-        stderr=sp.STDOUT, text=True
+        stderr=_sp.STDOUT, text=True
     )
-    res = re.match(r'^(?P<dur>\d+(?:\.\d+)?)', stdout)
+    res = _re.match(r'^(?P<dur>\d+(?:\.\d+)?)', stdout)
     return float(res.group('dur'))
 
 def get_audio_dur(file: str, ffprobe: str, /) -> float:
     """
     Get audio duration in secs.
     Note, video and audio might be different.
     `file`: full path to the input file
     `ffprobe`: ffprobe.exe full path
     """
-    stdout = sp.check_output(
+    stdout = _sp.check_output(
         [
             ffprobe, '-v', 'error',
             '-select_streams', 'a',
             '-of', 'csv=p=0',
             '-show_entries', 'stream=duration',
             file
         ],
-        stderr=sp.STDOUT, text=True
+        stderr=_sp.STDOUT, text=True
     )
-    res = re.match(r'^(?P<dur>\d+(?:\.\d+)?)', stdout)
+    res = _re.match(r'^(?P<dur>\d+(?:\.\d+)?)', stdout)
     return float(res.group('dur'))
 
 
 def get_vid_fps(file: str, ffprobe: str, /, *, do_round: bool = False) -> int | float:
     """
     Video fps (average frame rate).
 
     `file`: full path to the input file
     `ffprobe`: ffprobe.exe full path
     `do_round`: round the fps to the nearest integer
     """
-    stdout = sp.check_output(
+    stdout = _sp.check_output(
         [
             ffprobe, '-v', 'error',
             '-select_streams', 'v',
             '-of', 'csv=p=0',
             '-show_entries', 'stream=avg_frame_rate',
             file
         ],
-        stderr=sp.STDOUT, text=True
+        stderr=_sp.STDOUT, text=True
     )
-    res = re.match(r'^(?P<fps>\d+/\d+)', stdout)
+    res = _re.match(r'^(?P<fps>\d+/\d+)', stdout)
     fps = eval(res.group('fps'), {})
     if do_round:
         return round(fps)
     else:
         return fps
```

### Comparing `mykit-0.1.1/mykitx/kit/graph/graph2d/v2.py` & `mykit-0.1.2/mykit/kit/graph/graph2d.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,11 @@
 import random as _random
 import tkinter as _tk
 import typing as _typing
 
-from carbon.gui.shape import Arrow  # not suitable as axes due to complicated removal mechanism
-
 
 class Graph2D:
 
     page: _tk.Canvas = None
     @staticmethod
     def set_page(page: _tk.Canvas, /):
         Graph2D.page = page
```

### Comparing `mykit-0.1.1/mykitx/kit/gui/button/__init__.py` & `mykit-0.1.2/mykit/kit/gui/button/__init__.py`

 * *Files identical despite different names*

### Comparing `mykit-0.1.1/mykitx/kit/gui/button/v2.py` & `mykit-0.1.2/mykit/kit/gui/button/v2.py`

 * *Files identical despite different names*

### Comparing `mykit-0.1.1/mykitx/kit/gui/button/v3.py` & `mykit-0.1.2/mykit/kit/gui/button/v3.py`

 * *Files identical despite different names*

### Comparing `mykit-0.1.1/mykitx/kit/gui/label/__init__.py` & `mykit-0.1.2/mykit/kit/gui/label/__init__.py`

 * *Files identical despite different names*

### Comparing `mykit-0.1.1/mykitx/kit/gui/label/v2.py` & `mykit-0.1.2/mykit/kit/gui/label/v2.py`

 * *Files identical despite different names*

### Comparing `mykit-0.1.1/mykitx/kit/gui/shape/__init__.py` & `mykit-0.1.2/mykit/kit/gui/shape/__init__.py`

 * *Files identical despite different names*

### Comparing `mykit-0.1.1/mykitx/kit/gui/slider/__init__.py` & `mykit-0.1.2/mykit/kit/gui/slider/__init__.py`

 * *Files identical despite different names*

### Comparing `mykit-0.1.1/mykitx/kit/gui/slider/v2.py` & `mykit-0.1.2/mykit/kit/gui/slider/v2.py`

 * *Files identical despite different names*

### Comparing `mykit-0.1.1/mykitx/kit/keycrate/__init__.py` & `mykit-0.1.2/mykit/kit/keycrate/__init__.py`

 * *Files identical despite different names*

### Comparing `mykit-0.1.1/mykitx/kit/maths/__init__.py` & `mykit-0.1.2/mykit/kit/math.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,10 +1,7 @@
-"""
-This module is the next generation of carbon.math
-"""
 import numpy as _np
 
 
 def tanh(x: float | _np.ndarray, /, derivative: bool = False) -> float | _np.ndarray:
 
     z = _np.tanh(x)
```

### Comparing `mykit-0.1.1/mykitx/kit/neuralnet/dense/__init__.py` & `mykit-0.1.2/mykit/kit/neuralnet/dense/__init__.py`

 * *Files identical despite different names*

### Comparing `mykit-0.1.1/mykitx/kit/neuralnet/genetic/__init__.py` & `mykit-0.1.2/mykit/kit/neuralnet/genetic/__init__.py`

 * *Files identical despite different names*

### Comparing `mykit-0.1.1/mykitx/kit/noise/__init__.py` & `mykit-0.1.2/mykit/kit/noise.py`

 * *Files identical despite different names*

### Comparing `mykit-0.1.1/mykitx/kit/path/__init__.py` & `mykit-0.1.2/mykit/kit/path.py`

 * *Files identical despite different names*

### Comparing `mykit-0.1.1/mykitx/kit/quick_visual/plot2d.py` & `mykit-0.1.2/mykit/kit/quick_visual/plot2d.py`

 * *Files identical despite different names*

### Comparing `mykit-0.1.1/mykitx/kit/timelib/__init__.py` & `mykit-0.1.2/mykit/kit/time.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,12 +1,7 @@
-"""
-
-Reminder: This module has been renamed to "timelib" to prevent confusion with the built-in Python library "time".
-
-"""
 import re as _re
 
 
 def get_sexagecimal(secs: float, /, include_ms: bool = False) -> str:
     """
     Converts seconds to sexagesimal format.
```

### Comparing `mykit-0.1.1/mykitx/kit/utils/__init__.py` & `mykit-0.1.2/mykit/kit/utils.py`

 * *Files identical despite different names*

### Comparing `mykit-0.1.1/pyproject.toml` & `mykit-0.1.2/pyproject.toml`

 * *Files 24% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools>=61.0"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "mykit"
-version = "0.1.1"
+version = "0.1.2"
 authors = [
   { name="Nicholas Valentinus", email="nvfastplease@gmail.com" },
 ]
 description = "Python utility library"
 readme = "README.md"
 requires-python = ">=3.7"
 classifiers = [
```

