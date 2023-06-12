# Comparing `tmp/scrapetube-2.3.1-py3-none-any.whl.zip` & `tmp/scrapetube-2.3.2-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,10 +1,9 @@
-Zip file size: 5365 bytes, number of entries: 8
--rw-r--r--  2.0 unx       85 b- defN 22-Nov-03 06:24 scrapetube/__init__.py
--rw-r--r--  2.0 unx     7999 b- defN 22-Nov-03 06:17 scrapetube/scrapetube.py
--rw-r--r--  2.0 unx      129 b- defN 22-Aug-24 06:48 scrapetube/test.py
--rw-r--r--  2.0 unx     1072 b- defN 22-Nov-03 06:24 scrapetube-2.3.1.dist-info/LICENSE
--rw-r--r--  2.0 unx     1636 b- defN 22-Nov-03 06:24 scrapetube-2.3.1.dist-info/METADATA
--rw-r--r--  2.0 unx       92 b- defN 22-Nov-03 06:24 scrapetube-2.3.1.dist-info/WHEEL
--rw-r--r--  2.0 unx       11 b- defN 22-Nov-03 06:24 scrapetube-2.3.1.dist-info/top_level.txt
-?rw-rw-r--  2.0 unx      633 b- defN 22-Nov-03 06:24 scrapetube-2.3.1.dist-info/RECORD
-8 files, 11657 bytes uncompressed, 4259 bytes compressed:  63.5%
+Zip file size: 5240 bytes, number of entries: 7
+-rw-r--r--  2.0 unx       85 b- defN 23-Jun-12 19:39 scrapetube/__init__.py
+-rw-r--r--  2.0 unx     8473 b- defN 23-Jun-12 19:34 scrapetube/scrapetube.py
+-rw-r--r--  2.0 unx     1072 b- defN 23-Jun-12 19:40 scrapetube-2.3.2.dist-info/LICENSE
+-rw-r--r--  2.0 unx     1656 b- defN 23-Jun-12 19:40 scrapetube-2.3.2.dist-info/METADATA
+-rw-r--r--  2.0 unx       92 b- defN 23-Jun-12 19:40 scrapetube-2.3.2.dist-info/WHEEL
+-rw-r--r--  2.0 unx       11 b- defN 23-Jun-12 19:40 scrapetube-2.3.2.dist-info/top_level.txt
+?rw-rw-r--  2.0 unx      559 b- defN 23-Jun-12 19:40 scrapetube-2.3.2.dist-info/RECORD
+7 files, 11948 bytes uncompressed, 4246 bytes compressed:  64.5%
```

## zipnote {}

```diff
@@ -1,25 +1,22 @@
 Filename: scrapetube/__init__.py
 Comment: 
 
 Filename: scrapetube/scrapetube.py
 Comment: 
 
-Filename: scrapetube/test.py
+Filename: scrapetube-2.3.2.dist-info/LICENSE
 Comment: 
 
-Filename: scrapetube-2.3.1.dist-info/LICENSE
+Filename: scrapetube-2.3.2.dist-info/METADATA
 Comment: 
 
-Filename: scrapetube-2.3.1.dist-info/METADATA
+Filename: scrapetube-2.3.2.dist-info/WHEEL
 Comment: 
 
-Filename: scrapetube-2.3.1.dist-info/WHEEL
+Filename: scrapetube-2.3.2.dist-info/top_level.txt
 Comment: 
 
-Filename: scrapetube-2.3.1.dist-info/top_level.txt
-Comment: 
-
-Filename: scrapetube-2.3.1.dist-info/RECORD
+Filename: scrapetube-2.3.2.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## scrapetube/__init__.py

```diff
@@ -1,3 +1,3 @@
 from .scrapetube import get_channel, get_search, get_playlist
 
-__version__ = "2.3.1"
+__version__ = "2.3.2"
```

## scrapetube/scrapetube.py

```diff
@@ -1,21 +1,27 @@
 import json
 import time
 from typing import Generator
 
 import requests
 from typing_extensions import Literal
 
+type_property_map = {
+    "videos": "videoRenderer",
+    "streams": "videoRenderer",
+    "shorts": "reelItemRenderer"
+}
 
 def get_channel(
     channel_id: str = None,
     channel_url: str = None,
     limit: int = None,
     sleep: int = 1,
     sort_by: Literal["newest", "oldest", "popular"] = "newest",
+    content_type: Literal["videos", "shorts", "streams"] = "videos",
 ) -> Generator[dict, None, None]:
 
     """Get videos for a channel.
 
     Parameters:
         channel_id (``str``, *optional*):
             The channel id from the channel you want to get the videos for.
@@ -34,23 +40,30 @@
             Defaults to 1.
 
         sort_by (``str``, *optional*):
             In what order to retrieve to videos. Pass one of the following values.
             ``"newest"``: Get the new videos first.
             ``"oldest"``: Get the old videos first.
             ``"popular"``: Get the popular videos first. Defaults to "newest".
+
+        content_type (``str``, *optional*):
+            In order to get content type. Pass one of the following values.
+            ``"videos"``: Videos
+            ``"shorts"``: Shorts
+            ``"streams"``: Streams
     """
 
-    sort_by_map = {"newest": "dd", "oldest": "da", "popular": "p"}
-    url = "{url}/videos?view=0&sort={sort_by}&flow=grid".format(
+    sort_by_map = {"newest": "dd", "oldest": "da", "popular": "p"}    
+    url = "{url}/{content_type}?view=0&sort={sort_by}&flow=grid".format(
         url=channel_url or f"https://www.youtube.com/channel/{channel_id}",
+        content_type=content_type,
         sort_by=sort_by_map[sort_by],
     )
     api_endpoint = "https://www.youtube.com/youtubei/v1/browse"
-    videos = get_videos(url, api_endpoint, "videoRenderer", limit, sleep)
+    videos = get_videos(url, api_endpoint, type_property_map[content_type], limit, sleep)
     for video in videos:
         yield video
 
 
 def get_playlist(
     playlist_id: str, limit: int = None, sleep: int = 1
 ) -> Generator[dict, None, None]:
```

## Comparing `scrapetube-2.3.1.dist-info/LICENSE` & `scrapetube-2.3.2.dist-info/LICENSE`

 * *Files identical despite different names*

## Comparing `scrapetube-2.3.1.dist-info/METADATA` & `scrapetube-2.3.2.dist-info/METADATA`

 * *Files 10% similar despite different names*

```diff
@@ -1,17 +1,18 @@
 Metadata-Version: 2.1
 Name: scrapetube
-Version: 2.3.1
+Version: 2.3.2
 Summary: Scrape youtube without the official youtube api and without selenium.
 Home-page: https://github.com/dermasmid/scrapetube
 Author: Cheskel Twersky
 Author-email: twerskycheskel@gmail.com
 License: MIT
 Project-URL: Documentation, https://scrapetube.readthedocs.io/en/latest/
 Keywords: youtube python channel videos search playlist list get
+Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.6
 Description-Content-Type: text/markdown
 License-File: LICENSE
 Requires-Dist: requests
@@ -65,7 +66,9 @@
 for video in videos:
     print(video['videoId'])
 ```
 
 # Full Documentation
 
 [https://scrapetube.readthedocs.io/en/latest/](https://scrapetube.readthedocs.io/en/latest/)
+
+
```

