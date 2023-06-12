# Comparing `tmp/philbot_voice-1.9.5.tar.gz` & `tmp/philbot_voice-1.9.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "philbot_voice-1.9.5.tar", max compression
+gzip compressed data, was "philbot_voice-1.9.6.tar", max compression
```

## Comparing `philbot_voice-1.9.5.tar` & `philbot_voice-1.9.6.tar`

### file list

```diff
@@ -1,5 +1,5 @@
--rw-r--r--   0        0        0       19 2023-06-12 09:20:33.675229 philbot_voice-1.9.5/philbot-voice/__init__.py
--rw-r--r--   0        0        0       26 2023-06-12 09:20:33.675229 philbot_voice-1.9.5/philbot-voice/__main__.py
--rw-r--r--   0        0        0    43605 2023-06-12 09:20:33.675229 philbot_voice-1.9.5/philbot-voice/voice.py
--rw-r--r--   0        0        0      625 2023-06-12 09:20:33.675229 philbot_voice-1.9.5/pyproject.toml
--rw-r--r--   0        0        0      766 1970-01-01 00:00:00.000000 philbot_voice-1.9.5/PKG-INFO
+-rw-r--r--   0        0        0       19 2023-06-12 11:34:00.995492 philbot_voice-1.9.6/philbot-voice/__init__.py
+-rw-r--r--   0        0        0       26 2023-06-12 11:34:00.995492 philbot_voice-1.9.6/philbot-voice/__main__.py
+-rw-r--r--   0        0        0    43610 2023-06-12 11:34:00.995492 philbot_voice-1.9.6/philbot-voice/voice.py
+-rw-r--r--   0        0        0      625 2023-06-12 11:34:00.995492 philbot_voice-1.9.6/pyproject.toml
+-rw-r--r--   0        0        0      766 1970-01-01 00:00:00.000000 philbot_voice-1.9.6/PKG-INFO
```

### Comparing `philbot_voice-1.9.5/philbot-voice/voice.py` & `philbot_voice-1.9.6/philbot-voice/voice.py`

 * *Files 0% similar despite different names*

```diff
@@ -282,15 +282,15 @@
         # flush if necessary
         if do_flush:
             self.file.close()
             self.file = None
             from_filename = generate_audio_file_path(self.guild_id, self.channel_id, self.user_id, self.nonce, 'wav');
             to_filename = generate_audio_file_path(self.guild_id, self.channel_id, self.user_id, self.nonce, 'mp3');
             subprocess.run(['ffmpeg', '-i', from_filename, to_filename]).check_returncode()
-            os.remove(filename)
+            os.remove(from_filename)
         return do_flush
 
     def flush(self):
         return self.try_flush(0)
 
     def reset(self):
         if self.file:
```

### Comparing `philbot_voice-1.9.5/pyproject.toml` & `philbot_voice-1.9.6/pyproject.toml`

 * *Files 20% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "philbot-voice"
-version = "1.9.5"
+version = "1.9.6"
 description = ""
 authors = ["philipp.lengauer <p.lengauer@gmail.com>"]
 packages = [{include = "philbot-voice"}]
 
 [tool.poetry.dependencies]
 python = "^3.10"
 Flask = "^2.2.2"
```

### Comparing `philbot_voice-1.9.5/PKG-INFO` & `philbot_voice-1.9.6/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: philbot-voice
-Version: 1.9.5
+Version: 1.9.6
 Summary: 
 Author: philipp.lengauer
 Author-email: p.lengauer@gmail.com
 Requires-Python: >=3.10,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
```

