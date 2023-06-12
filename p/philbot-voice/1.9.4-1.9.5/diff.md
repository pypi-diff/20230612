# Comparing `tmp/philbot_voice-1.9.4.tar.gz` & `tmp/philbot_voice-1.9.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "philbot_voice-1.9.4.tar", max compression
+gzip compressed data, was "philbot_voice-1.9.5.tar", max compression
```

## Comparing `philbot_voice-1.9.4.tar` & `philbot_voice-1.9.5.tar`

### file list

```diff
@@ -1,5 +1,5 @@
--rw-r--r--   0        0        0       19 2023-06-11 15:14:36.519749 philbot_voice-1.9.4/philbot-voice/__init__.py
--rw-r--r--   0        0        0       26 2023-06-11 15:14:36.519749 philbot_voice-1.9.4/philbot-voice/__main__.py
--rw-r--r--   0        0        0    42898 2023-06-11 15:14:36.519749 philbot_voice-1.9.4/philbot-voice/voice.py
--rw-r--r--   0        0        0      625 2023-06-11 15:14:36.519749 philbot_voice-1.9.4/pyproject.toml
--rw-r--r--   0        0        0      766 1970-01-01 00:00:00.000000 philbot_voice-1.9.4/PKG-INFO
+-rw-r--r--   0        0        0       19 2023-06-12 09:20:33.675229 philbot_voice-1.9.5/philbot-voice/__init__.py
+-rw-r--r--   0        0        0       26 2023-06-12 09:20:33.675229 philbot_voice-1.9.5/philbot-voice/__main__.py
+-rw-r--r--   0        0        0    43605 2023-06-12 09:20:33.675229 philbot_voice-1.9.5/philbot-voice/voice.py
+-rw-r--r--   0        0        0      625 2023-06-12 09:20:33.675229 philbot_voice-1.9.5/pyproject.toml
+-rw-r--r--   0        0        0      766 1970-01-01 00:00:00.000000 philbot_voice-1.9.5/PKG-INFO
```

### Comparing `philbot_voice-1.9.4/philbot-voice/voice.py` & `philbot_voice-1.9.5/philbot-voice/voice.py`

 * *Files 3% similar despite different names*

```diff
@@ -101,16 +101,16 @@
     sequence, timestamp, ssrc = unwrap_voice_package_header(header)
     voice_chunk = secret_box.decrypt(package[12:], bytes(nonce))
     if voice_chunk[0] == 0xbe and voice_chunk[1] == 0xde: # RTP header extensions ...
         extension_length = int.from_bytes(voice_chunk[2:2+2], byteorder='big')
         voice_chunk = voice_chunk[2 + 2 + 4 * extension_length:]
     return sequence, timestamp, ssrc, voice_chunk
 
-def generate_audio_file_path(guild_id, channel_id, user_id, nonce):
-    return STORAGE_DIRECTORY + '/audio.' + guild_id + '.' + channel_id + '.' + user_id + '.' + str(nonce) + '.wav' 
+def generate_audio_file_path(guild_id, channel_id, user_id, nonce, extension = 'wav'):
+    return STORAGE_DIRECTORY + '/audio.' + guild_id + '.' + channel_id + '.' + user_id + '.' + str(nonce) + '.' + extension
 
 download_lock = threading.Lock()
 downloads = {}
 
 def download_from_youtube(guild_id, url):
     codec = 'wav'
     filename = url[url.index('v=') + 2:]
@@ -229,27 +229,26 @@
     
     def get_duration_secs(self):
         return self.packages * frame_duration / 1000
 
     def write(self, sequence, timestamp, pcm, nonce):
         if not self.file:
             self.nonce = nonce
-            self.file = wave.open(generate_audio_file_path(self.guild_id, self.channel_id, self.user_id, nonce), 'wb')
+            self.file = wave.open(generate_audio_file_path(self.guild_id, self.channel_id, self.user_id, nonce, 'wav'), 'wb')
             self.file.setsampwidth(sample_width)
             self.file.setnchannels(channels)
             self.file.setframerate(frame_rate)
             self.packages = 0
             self.last_sequence = None
             self.last_timestamp = None
             self.buffer = {}
             self.buffer_revision = None
         self.buffer[sequence] = Packet(sequence, timestamp, pcm)
         self.buffer_revision = time_millis()
     
-    # create_voice_package(sequence, sequence * desired_frame_size, self.ssrc, secret_box, opus_frame)
     def try_flush(self, limit = 1000):
         if not self.file:
             return False
         # some basic threasholds
         too_young_packages = max(0, limit - ((time_millis() - self.buffer_revision) if self.buffer_revision else 0)) // frame_duration
         min_pause_duration = 1000
         # find first earliest sequence in case we are just starting
@@ -280,14 +279,18 @@
         # check whether we ran out completely
         if len(self.buffer) == 0 and too_young_packages == 0:
             do_flush = True
         # flush if necessary
         if do_flush:
             self.file.close()
             self.file = None
+            from_filename = generate_audio_file_path(self.guild_id, self.channel_id, self.user_id, self.nonce, 'wav');
+            to_filename = generate_audio_file_path(self.guild_id, self.channel_id, self.user_id, self.nonce, 'mp3');
+            subprocess.run(['ffmpeg', '-i', from_filename, to_filename]).check_returncode()
+            os.remove(filename)
         return do_flush
 
     def flush(self):
         return self.try_flush(0)
 
     def reset(self):
         if self.file:
@@ -950,16 +953,22 @@
         time.sleep(tryy / 1000.0)
         tryy = tryy * 2
     return 'false'
 
 @app.route('/audio/guild/<guild_id>/channel/<channel_id>/user/<user_id>/nonce/<nonce>', methods=['GET'])
 def audio(guild_id, channel_id, user_id, nonce):
     # authenticate? attacker would need to know all the right IDs in real time before they are cleared and would then "just" get a random audio chunk
-    with open(generate_audio_file_path(guild_id, channel_id, user_id, nonce), 'rb') as bites:
-        return send_file(io.BytesIO(bites.read()), mimetype='audio/wav')
+    # attacker would have to know guild_id, channel_id (needs to be in the server), user_id (needs to be in the server or friend), and guess the right nonce, and access it in real-time
+    # they would get a small random audio chunk
+    for extension in ['wav', 'mp3']:
+        filename = generate_audio_file_path(guild_id, channel_id, user_id, nonce, extension)
+        if os.path.exists(filename):
+            with open(filename, 'rb') as bites:
+                return send_file(io.BytesIO(bites.read()), mimetype='audio/' + extension)
+    return Response('Not Found', status=404)
 
 def cleanup():
     for file in os.listdir(STORAGE_DIRECTORY):
         if os.path.getmtime(STORAGE_DIRECTORY + '/' + file) + 60 * 60 < time_seconds():
             try:
                 os.remove(STORAGE_DIRECTORY + '/' + file)
             except:
```

### Comparing `philbot_voice-1.9.4/pyproject.toml` & `philbot_voice-1.9.5/pyproject.toml`

 * *Files 20% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "philbot-voice"
-version = "1.9.4"
+version = "1.9.5"
 description = ""
 authors = ["philipp.lengauer <p.lengauer@gmail.com>"]
 packages = [{include = "philbot-voice"}]
 
 [tool.poetry.dependencies]
 python = "^3.10"
 Flask = "^2.2.2"
```

### Comparing `philbot_voice-1.9.4/PKG-INFO` & `philbot_voice-1.9.5/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: philbot-voice
-Version: 1.9.4
+Version: 1.9.5
 Summary: 
 Author: philipp.lengauer
 Author-email: p.lengauer@gmail.com
 Requires-Python: >=3.10,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
```

