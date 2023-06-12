# Comparing `tmp/spotify_lyrics_scraper-1.1.1.tar.gz` & `tmp/spotify_lyrics_scraper-1.1.2.tar.gz`

## Comparing `spotify_lyrics_scraper-1.1.1.tar` & `spotify_lyrics_scraper-1.1.2.tar`

### file list

```diff
@@ -1,6 +1,6 @@
--rw-r--r--   0        0        0     5017 2020-02-02 00:00:00.000000 spotify_lyrics_scraper-1.1.1/__init__.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 spotify_lyrics_scraper-1.1.1/main.py
--rw-r--r--   0        0        0     1101 2020-02-02 00:00:00.000000 spotify_lyrics_scraper-1.1.1/LICENSE
--rw-r--r--   0        0        0      907 2020-02-02 00:00:00.000000 spotify_lyrics_scraper-1.1.1/README.md
--rw-r--r--   0        0        0      583 2020-02-02 00:00:00.000000 spotify_lyrics_scraper-1.1.1/pyproject.toml
--rw-r--r--   0        0        0     1358 2020-02-02 00:00:00.000000 spotify_lyrics_scraper-1.1.1/PKG-INFO
+-rw-r--r--   0        0        0       29 2020-02-02 00:00:00.000000 spotify_lyrics_scraper-1.1.2/main.py
+-rw-r--r--   0        0        0     5017 2020-02-02 00:00:00.000000 spotify_lyrics_scraper-1.1.2/spotify-lyrics-scraper/__init__.py
+-rw-r--r--   0        0        0     1101 2020-02-02 00:00:00.000000 spotify_lyrics_scraper-1.1.2/LICENSE
+-rw-r--r--   0        0        0      907 2020-02-02 00:00:00.000000 spotify_lyrics_scraper-1.1.2/README.md
+-rw-r--r--   0        0        0      583 2020-02-02 00:00:00.000000 spotify_lyrics_scraper-1.1.2/pyproject.toml
+-rw-r--r--   0        0        0     1358 2020-02-02 00:00:00.000000 spotify_lyrics_scraper-1.1.2/PKG-INFO
```

### Comparing `spotify_lyrics_scraper-1.1.1/__init__.py` & `spotify_lyrics_scraper-1.1.2/spotify-lyrics-scraper/__init__.py`

 * *Files identical despite different names*

### Comparing `spotify_lyrics_scraper-1.1.1/LICENSE` & `spotify_lyrics_scraper-1.1.2/LICENSE`

 * *Files identical despite different names*

### Comparing `spotify_lyrics_scraper-1.1.1/README.md` & `spotify_lyrics_scraper-1.1.2/README.md`

 * *Files identical despite different names*

### Comparing `spotify_lyrics_scraper-1.1.1/pyproject.toml` & `spotify_lyrics_scraper-1.1.2/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["hatchling", "requests", "requests[socks]"]
 build-backend = "hatchling.build"
 
 [project]
 name = "spotify_lyrics_scraper"
-version = "1.1.1"
+version = "1.1.2"
 authors = [
   { name="PolyAnthi", email="polyanthi_pumicing@aleeas.com" },
 ]
 description = "This allows you to grab Spotify lyrics from their API. You can input song names or track IDs. Supports proxies."
 readme = "README.md"
 requires-python = ">=3.7"
 classifiers = [
```

### Comparing `spotify_lyrics_scraper-1.1.1/PKG-INFO` & `spotify_lyrics_scraper-1.1.2/PKG-INFO`

 * *Files 11% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: spotify_lyrics_scraper
-Version: 1.1.1
+Version: 1.1.2
 Summary: This allows you to grab Spotify lyrics from their API. You can input song names or track IDs. Supports proxies.
 Author-email: PolyAnthi <polyanthi_pumicing@aleeas.com>
 License-File: LICENSE
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3
 Requires-Python: >=3.7
```

