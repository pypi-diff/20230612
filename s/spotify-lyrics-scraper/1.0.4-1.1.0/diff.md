# Comparing `tmp/spotify_lyrics_scraper-1.0.4.tar.gz` & `tmp/spotify_lyrics_scraper-1.1.0.tar.gz`

## Comparing `spotify_lyrics_scraper-1.0.4.tar` & `spotify_lyrics_scraper-1.1.0.tar`

### file list

```diff
@@ -1,5 +1,5 @@
--rw-r--r--   0        0        0     4654 2020-02-02 00:00:00.000000 spotify_lyrics_scraper-1.0.4/src/spotify_lyrics/__init__.py
--rw-r--r--   0        0        0     1101 2020-02-02 00:00:00.000000 spotify_lyrics_scraper-1.0.4/LICENSE
--rw-r--r--   0        0        0      911 2020-02-02 00:00:00.000000 spotify_lyrics_scraper-1.0.4/README.md
--rw-r--r--   0        0        0      565 2020-02-02 00:00:00.000000 spotify_lyrics_scraper-1.0.4/pyproject.toml
--rw-r--r--   0        0        0     1344 2020-02-02 00:00:00.000000 spotify_lyrics_scraper-1.0.4/PKG-INFO
+-rw-r--r--   0        0        0     4654 2020-02-02 00:00:00.000000 spotify_lyrics_scraper-1.1.0/src/spotify_lyrics/__init__.py
+-rw-r--r--   0        0        0     1101 2020-02-02 00:00:00.000000 spotify_lyrics_scraper-1.1.0/LICENSE
+-rw-r--r--   0        0        0      907 2020-02-02 00:00:00.000000 spotify_lyrics_scraper-1.1.0/README.md
+-rw-r--r--   0        0        0      583 2020-02-02 00:00:00.000000 spotify_lyrics_scraper-1.1.0/pyproject.toml
+-rw-r--r--   0        0        0     1358 2020-02-02 00:00:00.000000 spotify_lyrics_scraper-1.1.0/PKG-INFO
```

### Comparing `spotify_lyrics_scraper-1.0.4/src/spotify_lyrics/__init__.py` & `spotify_lyrics_scraper-1.1.0/src/spotify_lyrics/__init__.py`

 * *Files identical despite different names*

### Comparing `spotify_lyrics_scraper-1.0.4/LICENSE` & `spotify_lyrics_scraper-1.1.0/LICENSE`

 * *Files identical despite different names*

### Comparing `spotify_lyrics_scraper-1.0.4/README.md` & `spotify_lyrics_scraper-1.1.0/README.md`

 * *Files 12% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 # Spotify Lyrics Grabber
 This Spotify Lyrics Grabber is a tool to grab Spotify Lyrics of any song, not just the one you are listening to.
 
 **Table of Contents**
 
-- [Installation](#installation)\n
-- [Examples](#examples)\n
+- [Installation](#installation)
+- [Examples](#examples)
 
 ### Installation
 To install, run `pip install spotify-lyrics-scraper` in your command prompt. To import it, I recommend `import spotify-lyrics-scraper as spotify`
 
 ### Examples
 - Always using: `import spotify-lyrics-scraper as spotify`
 - To obtain the sp_dc, please check out https://github.com/akashrchandran/syrics/wiki/Finding-sp_dc. This is required to have access to the lyrics API.
```

### Comparing `spotify_lyrics_scraper-1.0.4/pyproject.toml` & `spotify_lyrics_scraper-1.1.0/pyproject.toml`

 * *Files 14% similar despite different names*

```diff
@@ -1,18 +1,18 @@
 [build-system]
 requires = ["hatchling", "requests", "requests[socks]"]
 build-backend = "hatchling.build"
 
 [project]
 name = "spotify_lyrics_scraper"
-version = "1.0.4"
+version = "1.1.0"
 authors = [
   { name="PolyAnthi", email="polyanthi_pumicing@aleeas.com" },
 ]
-description = "This allows you to grab Spotify lyrics from their API. You can input song names or track IDs."
+description = "This allows you to grab Spotify lyrics from their API. You can input song names or track IDs. Supports proxies."
 readme = "README.md"
 requires-python = ">=3.7"
 classifiers = [
     "Programming Language :: Python :: 3",
     "License :: OSI Approved :: MIT License",
     "Operating System :: OS Independent",
 ]
```

### Comparing `spotify_lyrics_scraper-1.0.4/PKG-INFO` & `spotify_lyrics_scraper-1.1.0/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,26 +1,26 @@
 Metadata-Version: 2.1
 Name: spotify_lyrics_scraper
-Version: 1.0.4
-Summary: This allows you to grab Spotify lyrics from their API. You can input song names or track IDs.
+Version: 1.1.0
+Summary: This allows you to grab Spotify lyrics from their API. You can input song names or track IDs. Supports proxies.
 Author-email: PolyAnthi <polyanthi_pumicing@aleeas.com>
 License-File: LICENSE
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
 
 # Spotify Lyrics Grabber
 This Spotify Lyrics Grabber is a tool to grab Spotify Lyrics of any song, not just the one you are listening to.
 
 **Table of Contents**
 
-- [Installation](#installation)\n
-- [Examples](#examples)\n
+- [Installation](#installation)
+- [Examples](#examples)
 
 ### Installation
 To install, run `pip install spotify-lyrics-scraper` in your command prompt. To import it, I recommend `import spotify-lyrics-scraper as spotify`
 
 ### Examples
 - Always using: `import spotify-lyrics-scraper as spotify`
 - To obtain the sp_dc, please check out https://github.com/akashrchandran/syrics/wiki/Finding-sp_dc. This is required to have access to the lyrics API.
```

