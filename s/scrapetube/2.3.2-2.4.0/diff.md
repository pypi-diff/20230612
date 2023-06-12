# Comparing `tmp/scrapetube-2.3.2-py3-none-any.whl.zip` & `tmp/scrapetube-2.4.0-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,9 +1,9 @@
-Zip file size: 5240 bytes, number of entries: 7
--rw-r--r--  2.0 unx       85 b- defN 23-Jun-12 19:39 scrapetube/__init__.py
--rw-r--r--  2.0 unx     8473 b- defN 23-Jun-12 19:34 scrapetube/scrapetube.py
--rw-r--r--  2.0 unx     1072 b- defN 23-Jun-12 19:40 scrapetube-2.3.2.dist-info/LICENSE
--rw-r--r--  2.0 unx     1656 b- defN 23-Jun-12 19:40 scrapetube-2.3.2.dist-info/METADATA
--rw-r--r--  2.0 unx       92 b- defN 23-Jun-12 19:40 scrapetube-2.3.2.dist-info/WHEEL
--rw-r--r--  2.0 unx       11 b- defN 23-Jun-12 19:40 scrapetube-2.3.2.dist-info/top_level.txt
-?rw-rw-r--  2.0 unx      559 b- defN 23-Jun-12 19:40 scrapetube-2.3.2.dist-info/RECORD
-7 files, 11948 bytes uncompressed, 4246 bytes compressed:  64.5%
+Zip file size: 5328 bytes, number of entries: 7
+-rw-r--r--  2.0 unx       85 b- defN 23-Jun-12 20:17 scrapetube/__init__.py
+-rw-r--r--  2.0 unx     8970 b- defN 23-Jun-12 20:15 scrapetube/scrapetube.py
+-rw-r--r--  2.0 unx     1072 b- defN 23-Jun-12 20:17 scrapetube-2.4.0.dist-info/LICENSE
+-rw-r--r--  2.0 unx     1656 b- defN 23-Jun-12 20:17 scrapetube-2.4.0.dist-info/METADATA
+-rw-r--r--  2.0 unx       92 b- defN 23-Jun-12 20:17 scrapetube-2.4.0.dist-info/WHEEL
+-rw-r--r--  2.0 unx       11 b- defN 23-Jun-12 20:17 scrapetube-2.4.0.dist-info/top_level.txt
+?rw-rw-r--  2.0 unx      559 b- defN 23-Jun-12 20:17 scrapetube-2.4.0.dist-info/RECORD
+7 files, 12445 bytes uncompressed, 4334 bytes compressed:  65.2%
```

## zipnote {}

```diff
@@ -1,22 +1,22 @@
 Filename: scrapetube/__init__.py
 Comment: 
 
 Filename: scrapetube/scrapetube.py
 Comment: 
 
-Filename: scrapetube-2.3.2.dist-info/LICENSE
+Filename: scrapetube-2.4.0.dist-info/LICENSE
 Comment: 
 
-Filename: scrapetube-2.3.2.dist-info/METADATA
+Filename: scrapetube-2.4.0.dist-info/METADATA
 Comment: 
 
-Filename: scrapetube-2.3.2.dist-info/WHEEL
+Filename: scrapetube-2.4.0.dist-info/WHEEL
 Comment: 
 
-Filename: scrapetube-2.3.2.dist-info/top_level.txt
+Filename: scrapetube-2.4.0.dist-info/top_level.txt
 Comment: 
 
-Filename: scrapetube-2.3.2.dist-info/RECORD
+Filename: scrapetube-2.4.0.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## scrapetube/__init__.py

```diff
@@ -1,3 +1,3 @@
 from .scrapetube import get_channel, get_search, get_playlist
 
-__version__ = "2.3.2"
+__version__ = "2.4.0"
```

## scrapetube/scrapetube.py

```diff
@@ -10,14 +10,15 @@
     "streams": "videoRenderer",
     "shorts": "reelItemRenderer"
 }
 
 def get_channel(
     channel_id: str = None,
     channel_url: str = None,
+    channel_username: str = None,
     limit: int = None,
     sleep: int = 1,
     sort_by: Literal["newest", "oldest", "popular"] = "newest",
     content_type: Literal["videos", "shorts", "streams"] = "videos",
 ) -> Generator[dict, None, None]:
 
     """Get videos for a channel.
@@ -28,14 +29,19 @@
             If you prefer to use the channel url instead, see ``channel_url`` below.
 
         channel_url (``str``, *optional*):
             The url to the channel you want to get the videos for.
             Since there is a few type's of channel url's, you can use the one you want
             by passing it here instead of using ``channel_id``.
 
+        channel_username (``str``, *optional*):
+            The username from the channel you want to get the videos for.
+            Ex. ``LinusTechTips`` (without the @).
+            If you prefer to use the channel url instead, see ``channel_url`` above.
+
         limit (``int``, *optional*):
             Limit the number of videos you want to get.
 
         sleep (``int``, *optional*):
             Seconds to sleep between API calls to youtube, in order to prevent getting blocked.
             Defaults to 1.
 
@@ -48,17 +54,26 @@
         content_type (``str``, *optional*):
             In order to get content type. Pass one of the following values.
             ``"videos"``: Videos
             ``"shorts"``: Shorts
             ``"streams"``: Streams
     """
 
-    sort_by_map = {"newest": "dd", "oldest": "da", "popular": "p"}    
-    url = "{url}/{content_type}?view=0&sort={sort_by}&flow=grid".format(
-        url=channel_url or f"https://www.youtube.com/channel/{channel_id}",
+    sort_by_map = {"newest": "dd", "oldest": "da", "popular": "p"}
+
+    base_url = ""
+    if channel_url:
+        base_url = channel_url
+    elif channel_id:
+        base_url = f"https://www.youtube.com/channel/{channel_id}"
+    elif channel_username:
+        base_url = f"https://www.youtube.com/@{channel_username}"
+
+    url = "{base_url}/{content_type}?view=0&sort={sort_by}&flow=grid".format(
+        base_url=base_url,
         content_type=content_type,
         sort_by=sort_by_map[sort_by],
     )
     api_endpoint = "https://www.youtube.com/youtubei/v1/browse"
     videos = get_videos(url, api_endpoint, type_property_map[content_type], limit, sleep)
     for video in videos:
         yield video
```

## Comparing `scrapetube-2.3.2.dist-info/LICENSE` & `scrapetube-2.4.0.dist-info/LICENSE`

 * *Files identical despite different names*

## Comparing `scrapetube-2.3.2.dist-info/METADATA` & `scrapetube-2.4.0.dist-info/METADATA`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: scrapetube
-Version: 2.3.2
+Version: 2.4.0
 Summary: Scrape youtube without the official youtube api and without selenium.
 Home-page: https://github.com/dermasmid/scrapetube
 Author: Cheskel Twersky
 Author-email: twerskycheskel@gmail.com
 License: MIT
 Project-URL: Documentation, https://scrapetube.readthedocs.io/en/latest/
 Keywords: youtube python channel videos search playlist list get
```

## Comparing `scrapetube-2.3.2.dist-info/RECORD` & `scrapetube-2.4.0.dist-info/RECORD`

 * *Files 16% similar despite different names*

```diff
@@ -1,7 +1,7 @@
-scrapetube/__init__.py,sha256=94ICVkkQGmC85kx2GAOfJcRDbtNmfurX61Em4rrTgoU,85
-scrapetube/scrapetube.py,sha256=mKkaYXP_0RG7Ddc57NGU_rPK8gSDtyrOV9uzyw7ny4g,8473
-scrapetube-2.3.2.dist-info/LICENSE,sha256=BYIZCcJrWOrt4tv4kLtd2B3_x-_W79WA3qOYrqiYQiw,1072
-scrapetube-2.3.2.dist-info/METADATA,sha256=K3O_SObtlyL3F0WSGQY4WZPV7iT7pS9DnFmNoXqSV1M,1656
-scrapetube-2.3.2.dist-info/WHEEL,sha256=ewwEueio1C2XeHTvT17n8dZUJgOvyCWCt0WVNLClP9o,92
-scrapetube-2.3.2.dist-info/top_level.txt,sha256=_bKLdUlmHTUhm4ZHvUqmlr0_kIjW2_H1ncLQuFYeG8k,11
-scrapetube-2.3.2.dist-info/RECORD,,
+scrapetube/__init__.py,sha256=KdnRh-Hj7_2cZX2qTUunqGwPtmLFKGqFXNC_8oMDTmg,85
+scrapetube/scrapetube.py,sha256=AeZjmKZr2esHgXEEm7ocg6lKdJHXGPYIlPcnd_XmiHM,8970
+scrapetube-2.4.0.dist-info/LICENSE,sha256=BYIZCcJrWOrt4tv4kLtd2B3_x-_W79WA3qOYrqiYQiw,1072
+scrapetube-2.4.0.dist-info/METADATA,sha256=PLI2zJeR-ItjOYyoCGQwZnD2IbFndEtL_4ynFFNZHOA,1656
+scrapetube-2.4.0.dist-info/WHEEL,sha256=ewwEueio1C2XeHTvT17n8dZUJgOvyCWCt0WVNLClP9o,92
+scrapetube-2.4.0.dist-info/top_level.txt,sha256=_bKLdUlmHTUhm4ZHvUqmlr0_kIjW2_H1ncLQuFYeG8k,11
+scrapetube-2.4.0.dist-info/RECORD,,
```

