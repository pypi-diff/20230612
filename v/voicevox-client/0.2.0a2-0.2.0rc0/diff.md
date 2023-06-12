# Comparing `tmp/voicevox-client-0.2.0a2.tar.gz` & `tmp/voicevox-client-0.2.0rc0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "voicevox-client-0.2.0a2.tar", last modified: Tue May  9 14:20:05 2023, max compression
+gzip compressed data, was "voicevox-client-0.2.0rc0.tar", last modified: Mon May 22 04:26:18 2023, max compression
```

## Comparing `voicevox-client-0.2.0a2.tar` & `voicevox-client-0.2.0rc0.tar`

### file list

```diff
@@ -1,28 +1,28 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-09 14:20:05.866662 voicevox-client-0.2.0a2/
--rw-r--r--   0 runner    (1001) docker     (123)     1065 2023-05-09 14:19:49.000000 voicevox-client-0.2.0a2/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     1402 2023-05-09 14:20:05.866662 voicevox-client-0.2.0a2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      985 2023-05-09 14:19:49.000000 voicevox-client-0.2.0a2/README.rst
--rw-r--r--   0 runner    (1001) docker     (123)       90 2023-05-09 14:19:50.000000 voicevox-client-0.2.0a2/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-09 14:20:05.866662 voicevox-client-0.2.0a2/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1094 2023-05-09 14:19:50.000000 voicevox-client-0.2.0a2/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-09 14:20:05.866662 voicevox-client-0.2.0a2/voicevox/
--rw-r--r--   0 runner    (1001) docker     (123)      357 2023-05-09 14:19:50.000000 voicevox-client-0.2.0a2/voicevox/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5078 2023-05-09 14:19:50.000000 voicevox-client-0.2.0a2/voicevox/audio_query.py
--rw-r--r--   0 runner    (1001) docker     (123)     6774 2023-05-09 14:19:50.000000 voicevox-client-0.2.0a2/voicevox/client.py
--rw-r--r--   0 runner    (1001) docker     (123)      109 2023-05-09 14:19:50.000000 voicevox-client-0.2.0a2/voicevox/errors.py
--rw-r--r--   0 runner    (1001) docker     (123)     3385 2023-05-09 14:19:50.000000 voicevox-client-0.2.0a2/voicevox/http.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-09 14:19:50.000000 voicevox-client-0.2.0a2/voicevox/py.typed
--rw-r--r--   0 runner    (1001) docker     (123)     1339 2023-05-09 14:19:50.000000 voicevox-client-0.2.0a2/voicevox/speaker_info.py
--rw-r--r--   0 runner    (1001) docker     (123)     1554 2023-05-09 14:19:50.000000 voicevox-client-0.2.0a2/voicevox/speakers.py
--rw-r--r--   0 runner    (1001) docker     (123)      597 2023-05-09 14:19:50.000000 voicevox-client-0.2.0a2/voicevox/supported_devices.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-09 14:20:05.866662 voicevox-client-0.2.0a2/voicevox/types/
--rw-r--r--   0 runner    (1001) docker     (123)      280 2023-05-09 14:19:50.000000 voicevox-client-0.2.0a2/voicevox/types/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      640 2023-05-09 14:19:50.000000 voicevox-client-0.2.0a2/voicevox/types/audio_query.py
--rw-r--r--   0 runner    (1001) docker     (123)      282 2023-05-09 14:19:50.000000 voicevox-client-0.2.0a2/voicevox/types/speaker_info.py
--rw-r--r--   0 runner    (1001) docker     (123)      357 2023-05-09 14:19:50.000000 voicevox-client-0.2.0a2/voicevox/types/speakers.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-09 14:20:05.866662 voicevox-client-0.2.0a2/voicevox_client.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     1402 2023-05-09 14:20:05.000000 voicevox-client-0.2.0a2/voicevox_client.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      545 2023-05-09 14:20:05.000000 voicevox-client-0.2.0a2/voicevox_client.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-09 14:20:05.000000 voicevox-client-0.2.0a2/voicevox_client.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       84 2023-05-09 14:20:05.000000 voicevox-client-0.2.0a2/voicevox_client.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        9 2023-05-09 14:20:05.000000 voicevox-client-0.2.0a2/voicevox_client.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 04:26:18.684219 voicevox-client-0.2.0rc0/
+-rw-r--r--   0 runner    (1001) docker     (123)     1065 2023-05-22 04:26:05.000000 voicevox-client-0.2.0rc0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     1412 2023-05-22 04:26:18.684219 voicevox-client-0.2.0rc0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      994 2023-05-22 04:26:05.000000 voicevox-client-0.2.0rc0/README.rst
+-rw-r--r--   0 runner    (1001) docker     (123)       90 2023-05-22 04:26:05.000000 voicevox-client-0.2.0rc0/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-22 04:26:18.688218 voicevox-client-0.2.0rc0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1094 2023-05-22 04:26:05.000000 voicevox-client-0.2.0rc0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 04:26:18.684219 voicevox-client-0.2.0rc0/voicevox/
+-rw-r--r--   0 runner    (1001) docker     (123)      357 2023-05-22 04:26:05.000000 voicevox-client-0.2.0rc0/voicevox/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5136 2023-05-22 04:26:05.000000 voicevox-client-0.2.0rc0/voicevox/audio_query.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6774 2023-05-22 04:26:05.000000 voicevox-client-0.2.0rc0/voicevox/client.py
+-rw-r--r--   0 runner    (1001) docker     (123)      109 2023-05-22 04:26:05.000000 voicevox-client-0.2.0rc0/voicevox/errors.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3385 2023-05-22 04:26:05.000000 voicevox-client-0.2.0rc0/voicevox/http.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-22 04:26:05.000000 voicevox-client-0.2.0rc0/voicevox/py.typed
+-rw-r--r--   0 runner    (1001) docker     (123)     1339 2023-05-22 04:26:05.000000 voicevox-client-0.2.0rc0/voicevox/speaker_info.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1554 2023-05-22 04:26:05.000000 voicevox-client-0.2.0rc0/voicevox/speakers.py
+-rw-r--r--   0 runner    (1001) docker     (123)      597 2023-05-22 04:26:05.000000 voicevox-client-0.2.0rc0/voicevox/supported_devices.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 04:26:18.684219 voicevox-client-0.2.0rc0/voicevox/types/
+-rw-r--r--   0 runner    (1001) docker     (123)      280 2023-05-22 04:26:05.000000 voicevox-client-0.2.0rc0/voicevox/types/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      640 2023-05-22 04:26:05.000000 voicevox-client-0.2.0rc0/voicevox/types/audio_query.py
+-rw-r--r--   0 runner    (1001) docker     (123)      282 2023-05-22 04:26:05.000000 voicevox-client-0.2.0rc0/voicevox/types/speaker_info.py
+-rw-r--r--   0 runner    (1001) docker     (123)      357 2023-05-22 04:26:05.000000 voicevox-client-0.2.0rc0/voicevox/types/speakers.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 04:26:18.684219 voicevox-client-0.2.0rc0/voicevox_client.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     1412 2023-05-22 04:26:18.000000 voicevox-client-0.2.0rc0/voicevox_client.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      545 2023-05-22 04:26:18.000000 voicevox-client-0.2.0rc0/voicevox_client.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-22 04:26:18.000000 voicevox-client-0.2.0rc0/voicevox_client.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       84 2023-05-22 04:26:18.000000 voicevox-client-0.2.0rc0/voicevox_client.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        9 2023-05-22 04:26:18.000000 voicevox-client-0.2.0rc0/voicevox_client.egg-info/top_level.txt
```

### Comparing `voicevox-client-0.2.0a2/LICENSE` & `voicevox-client-0.2.0rc0/LICENSE`

 * *Files identical despite different names*

### Comparing `voicevox-client-0.2.0a2/PKG-INFO` & `voicevox-client-0.2.0rc0/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: voicevox-client
-Version: 0.2.0a2
+Version: 0.2.0rc0
 Summary: Voicevox engine unoffical wrapper
 Home-page: https://github.com/voicevox-client/python
 Author: tuna2134
 License: MIT
 Project-URL: Documentation, https://voicevox-client.tuna2134.jp
 Project-URL: Source, https://github.com/voicevox-client/python
 Description-Content-Type: text/x-rst
@@ -49,12 +49,12 @@
 
    async def main():
        async with Client() as client:
            audio_query = await client.create_audio_query(
                "こんにちは！", speaker=1
            )
            with open("voice.wav", "wb") as f:
-               f.write(await audio_query.synthesis())
+               f.write(await audio_query.synthesis(speaker=4))
 
 
    if __name__ == "__main__":
        asyncio.run(main())
```

### Comparing `voicevox-client-0.2.0a2/README.rst` & `voicevox-client-0.2.0rc0/README.rst`

 * *Files 2% similar despite different names*

```diff
@@ -35,12 +35,12 @@
 
    async def main():
        async with Client() as client:
            audio_query = await client.create_audio_query(
                "こんにちは！", speaker=1
            )
            with open("voice.wav", "wb") as f:
-               f.write(await audio_query.synthesis())
+               f.write(await audio_query.synthesis(speaker=4))
 
 
    if __name__ == "__main__":
        asyncio.run(main())
```

### Comparing `voicevox-client-0.2.0a2/setup.py` & `voicevox-client-0.2.0rc0/setup.py`

 * *Files identical despite different names*

### Comparing `voicevox-client-0.2.0a2/voicevox/audio_query.py` & `voicevox-client-0.2.0rc0/voicevox/audio_query.py`

 * *Files 4% similar despite different names*

```diff
@@ -9,25 +9,25 @@
 
 class Mora:
     """Mora class
 
     Attributes
     ----------
     text: str
-        文字
+        Text to synthesize
     consonant: str
-        子音の音素
+        Start of consonants
     consonant_length: int
-        子音の音長
+        Pronounciation length of consonants
     vowel: str
-        母音の音素
+        Start of vowels
     vowel_length: int
-        母音の音長
+        Length of vowels
     pitch: int
-        ピッチ
+        ピッチ //Pitch of the voice
     """
 
     def __init__(self, payload: MoraType):
         self.text: str = payload["text"]
         self.consonant: str = payload["consonant"]
         self.consonant_length: int = payload["consonant_length"]
         self.vowel: int = payload["vowel"]
```

### Comparing `voicevox-client-0.2.0a2/voicevox/client.py` & `voicevox-client-0.2.0rc0/voicevox/client.py`

 * *Files identical despite different names*

### Comparing `voicevox-client-0.2.0a2/voicevox/http.py` & `voicevox-client-0.2.0rc0/voicevox/http.py`

 * *Files identical despite different names*

### Comparing `voicevox-client-0.2.0a2/voicevox/speaker_info.py` & `voicevox-client-0.2.0rc0/voicevox/speaker_info.py`

 * *Files identical despite different names*

### Comparing `voicevox-client-0.2.0a2/voicevox/speakers.py` & `voicevox-client-0.2.0rc0/voicevox/speakers.py`

 * *Files identical despite different names*

### Comparing `voicevox-client-0.2.0a2/voicevox/supported_devices.py` & `voicevox-client-0.2.0rc0/voicevox/supported_devices.py`

 * *Files identical despite different names*

### Comparing `voicevox-client-0.2.0a2/voicevox/types/audio_query.py` & `voicevox-client-0.2.0rc0/voicevox/types/audio_query.py`

 * *Files identical despite different names*

### Comparing `voicevox-client-0.2.0a2/voicevox_client.egg-info/PKG-INFO` & `voicevox-client-0.2.0rc0/voicevox_client.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: voicevox-client
-Version: 0.2.0a2
+Version: 0.2.0rc0
 Summary: Voicevox engine unoffical wrapper
 Home-page: https://github.com/voicevox-client/python
 Author: tuna2134
 License: MIT
 Project-URL: Documentation, https://voicevox-client.tuna2134.jp
 Project-URL: Source, https://github.com/voicevox-client/python
 Description-Content-Type: text/x-rst
@@ -49,12 +49,12 @@
 
    async def main():
        async with Client() as client:
            audio_query = await client.create_audio_query(
                "こんにちは！", speaker=1
            )
            with open("voice.wav", "wb") as f:
-               f.write(await audio_query.synthesis())
+               f.write(await audio_query.synthesis(speaker=4))
 
 
    if __name__ == "__main__":
        asyncio.run(main())
```

### Comparing `voicevox-client-0.2.0a2/voicevox_client.egg-info/SOURCES.txt` & `voicevox-client-0.2.0rc0/voicevox_client.egg-info/SOURCES.txt`

 * *Files identical despite different names*

