# Comparing `tmp/spotify_lyrics_scraper-1.1.2.tar.gz` & `tmp/spotify_lyrics_scraper-1.1.3.tar.gz`

## Comparing `spotify_lyrics_scraper-1.1.2.tar` & `spotify_lyrics_scraper-1.1.3.tar`

### file list

```diff
@@ -1,6 +1,5 @@
--rw-r--r--   0        0        0       29 2020-02-02 00:00:00.000000 spotify_lyrics_scraper-1.1.2/main.py
--rw-r--r--   0        0        0     5017 2020-02-02 00:00:00.000000 spotify_lyrics_scraper-1.1.2/spotify-lyrics-scraper/__init__.py
--rw-r--r--   0        0        0     1101 2020-02-02 00:00:00.000000 spotify_lyrics_scraper-1.1.2/LICENSE
--rw-r--r--   0        0        0      907 2020-02-02 00:00:00.000000 spotify_lyrics_scraper-1.1.2/README.md
--rw-r--r--   0        0        0      583 2020-02-02 00:00:00.000000 spotify_lyrics_scraper-1.1.2/pyproject.toml
--rw-r--r--   0        0        0     1358 2020-02-02 00:00:00.000000 spotify_lyrics_scraper-1.1.2/PKG-INFO
+-rw-r--r--   0        0        0     4922 2020-02-02 00:00:00.000000 spotify_lyrics_scraper-1.1.3/spotify_lyrics_scraper/__init__.py
+-rw-r--r--   0        0        0     1101 2020-02-02 00:00:00.000000 spotify_lyrics_scraper-1.1.3/LICENSE
+-rw-r--r--   0        0        0      907 2020-02-02 00:00:00.000000 spotify_lyrics_scraper-1.1.3/README.md
+-rw-r--r--   0        0        0      583 2020-02-02 00:00:00.000000 spotify_lyrics_scraper-1.1.3/pyproject.toml
+-rw-r--r--   0        0        0     1358 2020-02-02 00:00:00.000000 spotify_lyrics_scraper-1.1.3/PKG-INFO
```

### Comparing `spotify_lyrics_scraper-1.1.2/spotify-lyrics-scraper/__init__.py` & `spotify_lyrics_scraper-1.1.3/spotify_lyrics_scraper/__init__.py`

 * *Files 14% similar despite different names*

```diff
@@ -28,24 +28,35 @@
 
     Arguments:
         info {dict} - Information (contains token and expiry)\n
     """
     if info["expiry"] > round(time.time()-3*1000): return {"expired": False}
     return {"expired": True}
 
-def formatLyrics(lyrics: dict, mode: int = 0):
+def formatLyrics(lyrics: dict, mode: int = 0) -> dict:
     """
     Format the lyrics to your liking with several modes.
 
     Arguments:
         lyrics {dict} - Takes the direct output from the getLyrics function. Needs the lyrics in the base spotify format.\n
         mode {int} - Choose which mode to format the lyrics in.\n
-            - Just Lyrics
+            - 0: Lyrics Only
     """
 
+    if "message" not in lyrics: return {"status": False, "message": "No lyrics were provided or they were not in the correct format."}
+    if "status" in lyrics:
+        if not lyrics["status"]: return {"status": False, "message": "That JSON data is invalid because the status is set to false."}
+
+    toReturn = []
+    if mode == 0:
+        for element in lyrics["message"]["lyrics"]["lines"]: toReturn.append(str(element["words"]).replace("\\", ""))
+        return {"status": True, "message": toReturn}
+
+    return {"status": False, "message": "That is not a valid format type."}
+
 def getLyrics(info: dict, trackId: str = None, songName: str = None, proxies: dict = {}) -> dict:
     """
     Search up lyrics of any given song. Uses trackId first over songName.
 
     Arguments:
         info {dict} - Information (contains token and expiry)\n
         trackId {string} - The track ID for the Spotify song to search up.\n
@@ -59,37 +70,27 @@
     if not trackId and not songName: return {"status": False, "message": "No data was provided to search up."}
     
     if "expiry" and "token" not in info: return {"status": False, "message": "The key 'expiry' or 'value' was not found in the info dict."}
 
     tempCheck = checkExpiry(info)
     if tempCheck["expired"] == True: return {"status": False, "message": "Cookie has expired."}
 
-    if trackId:
-        headers = {
-            "User-Agent": "Mozilla/5.0 (X11; Linux x86_64) AppleWebKit/537.36 (KHTML, like Gecko) Chrome/101.0.0.0 Safari/537.36",
-            "App-Platform": "WebPlayer",
-            "Authorization": f"Bearer {info['token']}"
-        }
-
-        try: r = requests.get(f"https://spclient.wg.spotify.com/color-lyrics/v2/track/{trackId}?format=json&market=from_token", headers=headers, proxies=proxies)
-        except Exception as e: return {"status": False, "message": f"Error occured: {e}"}
-
-        if '"lines"' in r.text: return {"status": True, "message": r.json()}
-        else: return {"status": False, "message": f"Could not find track/{r.text}"}
+    headers = {
+        "User-Agent": "Mozilla/5.0 (X11; Linux x86_64) AppleWebKit/537.36 (KHTML, like Gecko) Chrome/101.0.0.0 Safari/537.36",
+        "App-Platform": "WebPlayer",
+        "Authorization": f"Bearer {info['token']}"
+    }
 
     if songName:
-        headers = {
-            "User-Agent": "Mozilla/5.0 (X11; Linux x86_64) AppleWebKit/537.36 (KHTML, like Gecko) Chrome/101.0.0.0 Safari/537.36",
-            "App-Platform": "WebPlayer",
-            "Authorization": f"Bearer {info['token']}"
-        }
-
         try: r = requests.get(f"https://api-partner.spotify.com/pathfinder/v1/query?operationName=searchDesktop&variables=%7B%22searchTerm%22%3A%22{songName.replace(' ', '+')}%22%2C%22offset%22%3A0%2C%22limit%22%3A10%2C%22numberOfTopResults%22%3A5%2C%22includeAudiobooks%22%3Afalse%7D&extensions=%7B%22persistedQuery%22%3A%7B%22version%22%3A1%2C%22sha256Hash%22%3A%22130115162add6f3499d2f88ead8a37a7cad1d4d2314f3a206377035e7d26b74c%22%7D%7D", headers=headers, proxies=proxies)
         except Exception as e: return {"status": False, "message": f"Error occured: {e}"}
 
         try: trackId = r.json()["data"]["searchV2"]["tracksV2"]["items"][0]["item"]["data"]["id"]
         except Exception as e: return {"status": False, "message": f"Error occured: {e} - song doesn't exist?"}
 
+    if trackId:
+
         try: r = requests.get(f"https://spclient.wg.spotify.com/color-lyrics/v2/track/{trackId}?format=json&market=from_token", headers=headers, proxies=proxies)
         except Exception as e: return {"status": False, "message": f"Error occured: {e}"}
+
         if '"lines"' in r.text: return {"status": True, "message": r.json()}
-        else: return {"status": False, "message": f"Could not find track/{r.text}"}
+        else: return {"status": False, "message": f"Could not find track/{r.text}"}
```

### Comparing `spotify_lyrics_scraper-1.1.2/LICENSE` & `spotify_lyrics_scraper-1.1.3/LICENSE`

 * *Files identical despite different names*

### Comparing `spotify_lyrics_scraper-1.1.2/README.md` & `spotify_lyrics_scraper-1.1.3/README.md`

 * *Files 3% similar despite different names*

```diff
@@ -3,18 +3,18 @@
 
 **Table of Contents**
 
 - [Installation](#installation)
 - [Examples](#examples)
 
 ### Installation
-To install, run `pip install spotify-lyrics-scraper` in your command prompt. To import it, I recommend `import spotify-lyrics-scraper as spotify`
+To install, run `pip install spotify-lyrics-scraper` in your command prompt. To import it, I recommend `import spotify_lyrics_scraper as spotify`
 
 ### Examples
-- Always using: `import spotify-lyrics-scraper as spotify`
+- Always using: `import spotify_lyrics_scraper as spotify`
 - To obtain the sp_dc, please check out https://github.com/akashrchandran/syrics/wiki/Finding-sp_dc. This is required to have access to the lyrics API.
 ##### Example 1
 ```
 token = spotify.getToken("SP_DC Here")
 print(spotify.getLyrics(token, songName="Song"))
 ```
```

### Comparing `spotify_lyrics_scraper-1.1.2/pyproject.toml` & `spotify_lyrics_scraper-1.1.3/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["hatchling", "requests", "requests[socks]"]
 build-backend = "hatchling.build"
 
 [project]
 name = "spotify_lyrics_scraper"
-version = "1.1.2"
+version = "1.1.3"
 authors = [
   { name="PolyAnthi", email="polyanthi_pumicing@aleeas.com" },
 ]
 description = "This allows you to grab Spotify lyrics from their API. You can input song names or track IDs. Supports proxies."
 readme = "README.md"
 requires-python = ">=3.7"
 classifiers = [
```

### Comparing `spotify_lyrics_scraper-1.1.2/PKG-INFO` & `spotify_lyrics_scraper-1.1.3/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: spotify_lyrics_scraper
-Version: 1.1.2
+Version: 1.1.3
 Summary: This allows you to grab Spotify lyrics from their API. You can input song names or track IDs. Supports proxies.
 Author-email: PolyAnthi <polyanthi_pumicing@aleeas.com>
 License-File: LICENSE
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3
 Requires-Python: >=3.7
@@ -15,18 +15,18 @@
 
 **Table of Contents**
 
 - [Installation](#installation)
 - [Examples](#examples)
 
 ### Installation
-To install, run `pip install spotify-lyrics-scraper` in your command prompt. To import it, I recommend `import spotify-lyrics-scraper as spotify`
+To install, run `pip install spotify-lyrics-scraper` in your command prompt. To import it, I recommend `import spotify_lyrics_scraper as spotify`
 
 ### Examples
-- Always using: `import spotify-lyrics-scraper as spotify`
+- Always using: `import spotify_lyrics_scraper as spotify`
 - To obtain the sp_dc, please check out https://github.com/akashrchandran/syrics/wiki/Finding-sp_dc. This is required to have access to the lyrics API.
 ##### Example 1
 ```
 token = spotify.getToken("SP_DC Here")
 print(spotify.getLyrics(token, songName="Song"))
 ```
```

