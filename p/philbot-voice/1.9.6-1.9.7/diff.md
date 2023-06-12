# Comparing `tmp/philbot_voice-1.9.6.tar.gz` & `tmp/philbot_voice-1.9.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "philbot_voice-1.9.6.tar", max compression
+gzip compressed data, was "philbot_voice-1.9.7.tar", max compression
```

## Comparing `philbot_voice-1.9.6.tar` & `philbot_voice-1.9.7.tar`

### file list

```diff
@@ -1,5 +1,5 @@
--rw-r--r--   0        0        0       19 2023-06-12 11:34:00.995492 philbot_voice-1.9.6/philbot-voice/__init__.py
--rw-r--r--   0        0        0       26 2023-06-12 11:34:00.995492 philbot_voice-1.9.6/philbot-voice/__main__.py
--rw-r--r--   0        0        0    43610 2023-06-12 11:34:00.995492 philbot_voice-1.9.6/philbot-voice/voice.py
--rw-r--r--   0        0        0      625 2023-06-12 11:34:00.995492 philbot_voice-1.9.6/pyproject.toml
--rw-r--r--   0        0        0      766 1970-01-01 00:00:00.000000 philbot_voice-1.9.6/PKG-INFO
+-rw-r--r--   0        0        0       19 2023-06-12 21:08:36.028691 philbot_voice-1.9.7/philbot-voice/__init__.py
+-rw-r--r--   0        0        0       26 2023-06-12 21:08:36.028691 philbot_voice-1.9.7/philbot-voice/__main__.py
+-rw-r--r--   0        0        0    43475 2023-06-12 21:08:36.028691 philbot_voice-1.9.7/philbot-voice/voice.py
+-rw-r--r--   0        0        0      625 2023-06-12 21:08:36.028691 philbot_voice-1.9.7/pyproject.toml
+-rw-r--r--   0        0        0      766 1970-01-01 00:00:00.000000 philbot_voice-1.9.7/PKG-INFO
```

### Comparing `philbot_voice-1.9.6/philbot-voice/voice.py` & `philbot_voice-1.9.7/philbot-voice/voice.py`

 * *Files 1% similar despite different names*

```diff
@@ -952,36 +952,36 @@
             return 'true'
         time.sleep(tryy / 1000.0)
         tryy = tryy * 2
     return 'false'
 
 @app.route('/audio/guild/<guild_id>/channel/<channel_id>/user/<user_id>/nonce/<nonce>', methods=['GET'])
 def audio(guild_id, channel_id, user_id, nonce):
-    # authenticate? attacker would need to know all the right IDs in real time before they are cleared and would then "just" get a random audio chunk
+    # authenticate?
     # attacker would have to know guild_id, channel_id (needs to be in the server), user_id (needs to be in the server or friend), and guess the right nonce, and access it in real-time
     # they would get a small random audio chunk
     for extension in ['wav', 'mp3']:
         filename = generate_audio_file_path(guild_id, channel_id, user_id, nonce, extension)
         if os.path.exists(filename):
             with open(filename, 'rb') as bites:
                 return send_file(io.BytesIO(bites.read()), mimetype='audio/' + extension)
     return Response('Not Found', status=404)
 
 def cleanup():
     for file in os.listdir(STORAGE_DIRECTORY):
-        if os.path.getmtime(STORAGE_DIRECTORY + '/' + file) + 60 * 60 < time_seconds():
+        if os.path.getmtime(STORAGE_DIRECTORY + '/' + file) + 60 * 15 < time_seconds():
             try:
                 os.remove(STORAGE_DIRECTORY + '/' + file)
             except:
                 pass
 
 def cleanup_loop():
     while True:
         cleanup()
-        time.sleep(60 * 60)
+        time.sleep(60)
 
 def main():
     for file in os.listdir('.'):
         if file.startswith('.state.') and file.endswith('.json'):
             get_context(file[len('.state.'):len(file) - len('.json')])
     threading.Thread(target=cleanup_loop).start()
     print('VOICE ready')
```

### Comparing `philbot_voice-1.9.6/pyproject.toml` & `philbot_voice-1.9.7/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "philbot-voice"
-version = "1.9.6"
+version = "1.9.7"
 description = ""
 authors = ["philipp.lengauer <p.lengauer@gmail.com>"]
 packages = [{include = "philbot-voice"}]
 
 [tool.poetry.dependencies]
 python = "^3.10"
 Flask = "^2.2.2"
```

### Comparing `philbot_voice-1.9.6/PKG-INFO` & `philbot_voice-1.9.7/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: philbot-voice
-Version: 1.9.6
+Version: 1.9.7
 Summary: 
 Author: philipp.lengauer
 Author-email: p.lengauer@gmail.com
 Requires-Python: >=3.10,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
```

