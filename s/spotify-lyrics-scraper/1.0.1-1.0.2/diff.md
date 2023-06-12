# Comparing `tmp/spotify_lyrics_scraper-1.0.1.tar.gz` & `tmp/spotify_lyrics_scraper-1.0.2.tar.gz`

## Comparing `spotify_lyrics_scraper-1.0.1.tar` & `spotify_lyrics_scraper-1.0.2.tar`

### file list

```diff
@@ -1,5 +1,5 @@
--rw-r--r--   0        0        0     4142 2020-02-02 00:00:00.000000 spotify_lyrics_scraper-1.0.1/src/spotify_lyrics/__init__.py
--rw-r--r--   0        0        0     1101 2020-02-02 00:00:00.000000 spotify_lyrics_scraper-1.0.1/LICENSE
--rw-r--r--   0        0        0      545 2020-02-02 00:00:00.000000 spotify_lyrics_scraper-1.0.1/README.md
--rw-r--r--   0        0        0      546 2020-02-02 00:00:00.000000 spotify_lyrics_scraper-1.0.1/pyproject.toml
--rw-r--r--   0        0        0      991 2020-02-02 00:00:00.000000 spotify_lyrics_scraper-1.0.1/PKG-INFO
+-rw-r--r--   0        0        0     4690 2020-02-02 00:00:00.000000 spotify_lyrics_scraper-1.0.2/src/spotify_lyrics/__init__.py
+-rw-r--r--   0        0        0     1101 2020-02-02 00:00:00.000000 spotify_lyrics_scraper-1.0.2/LICENSE
+-rw-r--r--   0        0        0      545 2020-02-02 00:00:00.000000 spotify_lyrics_scraper-1.0.2/README.md
+-rw-r--r--   0        0        0      565 2020-02-02 00:00:00.000000 spotify_lyrics_scraper-1.0.2/pyproject.toml
+-rw-r--r--   0        0        0      991 2020-02-02 00:00:00.000000 spotify_lyrics_scraper-1.0.2/PKG-INFO
```

### Comparing `spotify_lyrics_scraper-1.0.1/src/spotify_lyrics/__init__.py` & `spotify_lyrics_scraper-1.0.2/src/spotify_lyrics/__init__.py`

 * *Files 19% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 ### Spotify Create a Token
-import requests, time
+import requests, time, random
 
 def getToken(sp_dc: str) -> dict:
     """
     Generates a Spotify Auth Token for searching lyrics/track IDs.\n
     To obtain the sp_dc, please check out https://github.com/akashrchandran/syrics/wiki/Finding-sp_dc. This is required to have access to the lyrics API.
 
     Returns:
@@ -29,22 +29,23 @@
 
     Arguments:
         info {dict} - Information (contains token and expiry)\n
     """
     if info["expiry"] > round(time.time()-3*1000): return {"expired": False}
     return {"expired": True}
 
-def getLyrics(info: dict, trackId: str = None, songName: str = None) -> dict:
+def getLyrics(info: dict, trackId: str = None, songName: str = None, proxies: dict = {}) -> dict:
     """
     Search up lyrics of any given song. Uses trackId first over songName.
 
     Arguments:
         info {dict} - Information (contains token and expiry)\n
         trackId {string} - The track ID for the Spotify song to search up.\n
-        songName {string} - The song name to search up.
+        songName {string} - The song name to search up.\n
+        proxies {dict} - Supports Socks5 and HTTP/S, example: {"http": "http://1.1.1.1:80", "https": "https://1.1.1.1:443", "http": "socks5://1.1.1.1:443"}
 
     Returns:
         dict - {"status": False if error, True if success, "message": "Reason why/lyrics"}
     """
 
     if not trackId and not songName: return {"status": False, "message": "No data was provided to search up."}
     
@@ -56,27 +57,30 @@
     if trackId:
         headers = {
             "User-Agent": "Mozilla/5.0 (X11; Linux x86_64) AppleWebKit/537.36 (KHTML, like Gecko) Chrome/101.0.0.0 Safari/537.36",
             "App-Platform": "WebPlayer",
             "Authorization": f"Bearer {info['token']}"
         }
 
-        r = requests.get(f"https://spclient.wg.spotify.com/color-lyrics/v2/track/{trackId}?format=json&market=from_token", headers=headers)
+        try: r = requests.get(f"https://spclient.wg.spotify.com/color-lyrics/v2/track/{trackId}?format=json&market=from_token", headers=headers, proxies=proxies)
+        except Exception as e: return {"status": False, "message": f"Error occured: {e}"}
 
         if '"lines"' in r.text: return {"status": True, "message": r.json()}
         else: return {"status": False, "message": f"Could not find track/{r.text}"}
 
     if songName:
         headers = {
             "User-Agent": "Mozilla/5.0 (X11; Linux x86_64) AppleWebKit/537.36 (KHTML, like Gecko) Chrome/101.0.0.0 Safari/537.36",
             "App-Platform": "WebPlayer",
             "Authorization": f"Bearer {info['token']}"
         }
 
-        r = requests.get(f"https://api-partner.spotify.com/pathfinder/v1/query?operationName=searchDesktop&variables=%7B%22searchTerm%22%3A%22{songName.replace(' ', '+')}%22%2C%22offset%22%3A0%2C%22limit%22%3A10%2C%22numberOfTopResults%22%3A5%2C%22includeAudiobooks%22%3Afalse%7D&extensions=%7B%22persistedQuery%22%3A%7B%22version%22%3A1%2C%22sha256Hash%22%3A%22130115162add6f3499d2f88ead8a37a7cad1d4d2314f3a206377035e7d26b74c%22%7D%7D", headers=headers)
+        try: r = requests.get(f"https://api-partner.spotify.com/pathfinder/v1/query?operationName=searchDesktop&variables=%7B%22searchTerm%22%3A%22{songName.replace(' ', '+')}%22%2C%22offset%22%3A0%2C%22limit%22%3A10%2C%22numberOfTopResults%22%3A5%2C%22includeAudiobooks%22%3Afalse%7D&extensions=%7B%22persistedQuery%22%3A%7B%22version%22%3A1%2C%22sha256Hash%22%3A%22130115162add6f3499d2f88ead8a37a7cad1d4d2314f3a206377035e7d26b74c%22%7D%7D", headers=headers, proxies=proxies)
+        except Exception as e: return {"status": False, "message": f"Error occured: {e}"}
 
         try: trackId = r.json()["data"]["searchV2"]["tracksV2"]["items"][0]["item"]["data"]["id"]
-        except Exception as e: return {"status": False, "message": f"Error occured: {e}"}
+        except Exception as e: return {"status": False, "message": f"Error occured: {e} - song doesn't exist?"}
 
-        r = requests.get(f"https://spclient.wg.spotify.com/color-lyrics/v2/track/{trackId}?format=json&market=from_token", headers=headers)
+        try: r = requests.get(f"https://spclient.wg.spotify.com/color-lyrics/v2/track/{trackId}?format=json&market=from_token", headers=headers, proxies=proxies)
+        except Exception as e: return {"status": False, "message": f"Error occured: {e}"}
         if '"lines"' in r.text: return {"status": True, "message": r.json()}
         else: return {"status": False, "message": f"Could not find track/{r.text}"}
```

### Comparing `spotify_lyrics_scraper-1.0.1/LICENSE` & `spotify_lyrics_scraper-1.0.2/LICENSE`

 * *Files identical despite different names*

### Comparing `spotify_lyrics_scraper-1.0.1/README.md` & `spotify_lyrics_scraper-1.0.2/README.md`

 * *Files identical despite different names*

### Comparing `spotify_lyrics_scraper-1.0.1/pyproject.toml` & `spotify_lyrics_scraper-1.0.2/pyproject.toml`

 * *Files 14% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
-requires = ["hatchling", "requests"]
+requires = ["hatchling", "requests", "requests[socks]"]
 build-backend = "hatchling.build"
 
 [project]
 name = "spotify_lyrics_scraper"
-version = "1.0.1"
+version = "1.0.2"
 authors = [
   { name="PolyAnthi", email="polyanthi_pumicing@aleeas.com" },
 ]
 description = "This allows you to grab Spotify lyrics from their API. You can input song names or track IDs."
 readme = "README.md"
 requires-python = ">=3.7"
 classifiers = [
```

### Comparing `spotify_lyrics_scraper-1.0.1/PKG-INFO` & `spotify_lyrics_scraper-1.0.2/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: spotify_lyrics_scraper
-Version: 1.0.1
+Version: 1.0.2
 Summary: This allows you to grab Spotify lyrics from their API. You can input song names or track IDs.
 Author-email: PolyAnthi <polyanthi_pumicing@aleeas.com>
 License-File: LICENSE
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3
 Requires-Python: >=3.7
```

