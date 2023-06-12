# Comparing `tmp/boosty-0.0.7.tar.gz` & `tmp/boosty-0.0.8.tar.gz`

## Comparing `boosty-0.0.7.tar` & `boosty-0.0.8.tar`

### file list

```diff
@@ -1,28 +1,29 @@
--rw-r--r--   0        0        0    24409 2020-02-02 00:00:00.000000 boosty-0.0.7/logo.png
--rw-r--r--   0        0        0       23 2020-02-02 00:00:00.000000 boosty-0.0.7/boosty/__init__.py
--rw-r--r--   0        0        0       22 2020-02-02 00:00:00.000000 boosty-0.0.7/boosty/api/__init__.py
--rw-r--r--   0        0        0     3659 2020-02-02 00:00:00.000000 boosty-0.0.7/boosty/api/api.py
--rw-r--r--   0        0        0     3673 2020-02-02 00:00:00.000000 boosty-0.0.7/boosty/api/auth.py
--rw-r--r--   0        0        0       21 2020-02-02 00:00:00.000000 boosty-0.0.7/boosty/types/__init__.py
--rw-r--r--   0        0        0      216 2020-02-02 00:00:00.000000 boosty-0.0.7/boosty/types/base.py
--rw-r--r--   0        0        0      968 2020-02-02 00:00:00.000000 boosty-0.0.7/boosty/types/comment.py
--rw-r--r--   0        0        0      262 2020-02-02 00:00:00.000000 boosty-0.0.7/boosty/types/content.py
--rw-r--r--   0        0        0      464 2020-02-02 00:00:00.000000 boosty-0.0.7/boosty/types/donator.py
--rw-r--r--   0        0        0     2427 2020-02-02 00:00:00.000000 boosty-0.0.7/boosty/types/media_types.py
--rw-r--r--   0        0        0     2598 2020-02-02 00:00:00.000000 boosty-0.0.7/boosty/types/post.py
--rw-r--r--   0        0        0      428 2020-02-02 00:00:00.000000 boosty-0.0.7/boosty/types/reactions.py
--rw-r--r--   0        0        0      781 2020-02-02 00:00:00.000000 boosty-0.0.7/boosty/types/reply.py
--rw-r--r--   0        0        0      178 2020-02-02 00:00:00.000000 boosty-0.0.7/boosty/types/teaser.py
--rw-r--r--   0        0        0      680 2020-02-02 00:00:00.000000 boosty-0.0.7/boosty/types/users.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 boosty-0.0.7/boosty/utils/__init__.py
--rw-r--r--   0        0        0     5163 2020-02-02 00:00:00.000000 boosty-0.0.7/boosty/utils/client.py
--rw-r--r--   0        0        0      486 2020-02-02 00:00:00.000000 boosty-0.0.7/boosty/utils/json.py
--rw-r--r--   0        0        0      389 2020-02-02 00:00:00.000000 boosty-0.0.7/boosty/utils/logging.py
--rw-r--r--   0        0        0     5089 2020-02-02 00:00:00.000000 boosty-0.0.7/boosty/utils/post.py
--rw-r--r--   0        0        0     3325 2020-02-02 00:00:00.000000 boosty-0.0.7/boosty/utils/video.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 boosty-0.0.7/tests/__init__.py
--rw-r--r--   0        0        0     2307 2020-02-02 00:00:00.000000 boosty-0.0.7/.gitignore
--rw-r--r--   0        0        0     1085 2020-02-02 00:00:00.000000 boosty-0.0.7/LICENSE
--rw-r--r--   0        0        0     1727 2020-02-02 00:00:00.000000 boosty-0.0.7/README.md
--rw-r--r--   0        0        0     1665 2020-02-02 00:00:00.000000 boosty-0.0.7/pyproject.toml
--rw-r--r--   0        0        0     2881 2020-02-02 00:00:00.000000 boosty-0.0.7/PKG-INFO
+-rw-r--r--   0        0        0    24409 2020-02-02 00:00:00.000000 boosty-0.0.8/logo.png
+-rw-r--r--   0        0        0       23 2020-02-02 00:00:00.000000 boosty-0.0.8/boosty/__init__.py
+-rw-r--r--   0        0        0       22 2020-02-02 00:00:00.000000 boosty-0.0.8/boosty/api/__init__.py
+-rw-r--r--   0        0        0     3765 2020-02-02 00:00:00.000000 boosty-0.0.8/boosty/api/api.py
+-rw-r--r--   0        0        0     3331 2020-02-02 00:00:00.000000 boosty-0.0.8/boosty/api/auth.py
+-rw-r--r--   0        0        0       21 2020-02-02 00:00:00.000000 boosty-0.0.8/boosty/types/__init__.py
+-rw-r--r--   0        0        0      216 2020-02-02 00:00:00.000000 boosty-0.0.8/boosty/types/base.py
+-rw-r--r--   0        0        0     1216 2020-02-02 00:00:00.000000 boosty-0.0.8/boosty/types/comment.py
+-rw-r--r--   0        0        0      262 2020-02-02 00:00:00.000000 boosty-0.0.8/boosty/types/content.py
+-rw-r--r--   0        0        0      464 2020-02-02 00:00:00.000000 boosty-0.0.8/boosty/types/donator.py
+-rw-r--r--   0        0        0     3058 2020-02-02 00:00:00.000000 boosty-0.0.8/boosty/types/media_types.py
+-rw-r--r--   0        0        0      666 2020-02-02 00:00:00.000000 boosty-0.0.8/boosty/types/poll.py
+-rw-r--r--   0        0        0     2951 2020-02-02 00:00:00.000000 boosty-0.0.8/boosty/types/post.py
+-rw-r--r--   0        0        0      428 2020-02-02 00:00:00.000000 boosty-0.0.8/boosty/types/reactions.py
+-rw-r--r--   0        0        0      781 2020-02-02 00:00:00.000000 boosty-0.0.8/boosty/types/reply.py
+-rw-r--r--   0        0        0      178 2020-02-02 00:00:00.000000 boosty-0.0.8/boosty/types/teaser.py
+-rw-r--r--   0        0        0      755 2020-02-02 00:00:00.000000 boosty-0.0.8/boosty/types/users.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 boosty-0.0.8/boosty/utils/__init__.py
+-rw-r--r--   0        0        0     5163 2020-02-02 00:00:00.000000 boosty-0.0.8/boosty/utils/client.py
+-rw-r--r--   0        0        0      486 2020-02-02 00:00:00.000000 boosty-0.0.8/boosty/utils/json.py
+-rw-r--r--   0        0        0      403 2020-02-02 00:00:00.000000 boosty-0.0.8/boosty/utils/logging.py
+-rw-r--r--   0        0        0     5312 2020-02-02 00:00:00.000000 boosty-0.0.8/boosty/utils/post.py
+-rw-r--r--   0        0        0     3483 2020-02-02 00:00:00.000000 boosty-0.0.8/boosty/utils/video.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 boosty-0.0.8/tests/__init__.py
+-rw-r--r--   0        0        0     2307 2020-02-02 00:00:00.000000 boosty-0.0.8/.gitignore
+-rw-r--r--   0        0        0     1085 2020-02-02 00:00:00.000000 boosty-0.0.8/LICENSE
+-rw-r--r--   0        0        0     1974 2020-02-02 00:00:00.000000 boosty-0.0.8/README.md
+-rw-r--r--   0        0        0     1665 2020-02-02 00:00:00.000000 boosty-0.0.8/pyproject.toml
+-rw-r--r--   0        0        0     3118 2020-02-02 00:00:00.000000 boosty-0.0.8/PKG-INFO
```

### Comparing `boosty-0.0.7/logo.png` & `boosty-0.0.8/logo.png`

 * *Files identical despite different names*

### Comparing `boosty-0.0.7/boosty/api/api.py` & `boosty-0.0.8/boosty/api/api.py`

 * *Files 4% similar despite different names*

```diff
@@ -3,19 +3,20 @@
 from boosty.api.auth import Auth
 from boosty.types import PostsResponse, Post, CommentsResponse
 from boosty.utils.client import AiohttpClient, ABCHTTPClient
 from boosty.utils.logging import logger
 
 
 class Error(BaseModel):
+    status_code: int
     error: str
-    error_description: str
+    error_description: str | None
 
 
-class BoostyError(ValueError):
+class BoostyError(Exception):
     pass
 
 
 class API:
     API_URL = "https://api.boosty.to"
 
     def __init__(
@@ -37,35 +38,41 @@
             f"{self.API_URL}{method}",
             method="GET",
             params=params,
             data=data,
             headers=self.auth.headers,
         )
 
-        if response.status // 100 == 5:
-            raise BoostyError(Error(error_description=str(response.status), error="Server error"))
-
-        response_json = await response.json(
-            encoding="utf-8", content_type=None
-        )
-
-        if response.status // 100 == 4:
-            if response.status == 401:
-                logger.warning("AUTH EXPIRED, REFRESHING VIA REFRESH_TOKEN...")
-                await self.auth.refresh_auth_data(self.http_client, self.API_URL)
-                return await self.request(method, params, data)
-            raise BoostyError(Error(**response_json))
+        if response.status == 401:
+            logger.warning("AUTH EXPIRED, REFRESHING VIA REFRESH_TOKEN...")
+            await self.auth.refresh_auth_data(self.http_client, self.API_URL)
+            return await self.request(method, params, data)
+
+        try:
+            response_json = await response.json(
+                encoding="utf-8", content_type=None
+            )
+        except ValueError:
+            response_json = {}
+
+        if response.status // 100 != 2:
+            raise BoostyError(
+                Error(
+                    status_code=response.status,
+                    **response_json or {"error": "Unknown error"}
+                )
+            )
 
         return response_json
 
     async def get_posts(
             self,
             name: str,
             *,
-            limit: conint(ge=1, le=100) = None,  # limit is based on data amount
+            limit: conint(ge=1) = None,  # limit is based on data amount ~300
             offset: str = None,  # "1654884900:923396"
             comments_limit: conint(ge=0) = None,
             reply_limit: int = None,  # idk ~1
     ) -> PostsResponse:
         resp_json = await self.request(
             f"/v1/blog/{name}/post/", params={
                 "limit": limit,
```

### Comparing `boosty-0.0.7/boosty/api/auth.py` & `boosty-0.0.8/boosty/api/auth.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,11 +1,10 @@
-import asyncio
 from time import time
 
-from boosty.utils.client import ABCHTTPClient, AiohttpClient
+from boosty.utils.client import ABCHTTPClient
 from boosty.utils.json import dict_to_file, file_to_dict
 from boosty.utils.logging import logger
 
 
 class Auth:  # TODO vk auth
     access_token, refresh_token, expires_at, device_id, headers = None, None, None, None, None
     DEFAULT_USER_AGENT = "Mozilla/5.0 (Windows NT 10.0; Win64; x64) AppleWebKit/537.36 (KHTML, like Gecko) Chrome/110.0.0.0 Safari/537.36"  # noqa
@@ -56,15 +55,14 @@
         dotenv.set_key(dotenv_file, "REFRESH_TOKEN", self.refresh_token, "auto")
         dotenv.set_key(dotenv_file, "EXPIRES_AT", self.expires_at, "auto")
         dotenv.set_key(dotenv_file, "DEVICE_ID", self.device_id, "auto")
 
     async def refresh_auth_data(self, session: ABCHTTPClient, api_url: str = ""):
         self.load_auth_data()
         if not self.refresh_token:
-            logger.error("No refresh token was found to refresh auth data")
             raise ValueError("No refresh token was found to refresh auth data")
 
         response_data = await session.request_json(
             f"{api_url}/oauth/token/",
             method="POST",
             data={
                 "device_id": self.device_id,
@@ -74,23 +72,12 @@
             },
             headers=self.headers)
 
         try:
             self.refresh_token = response_data["refresh_token"]
             self.access_token = response_data["access_token"]
             self.expires_at = int(time()) + response_data["expires_in"]
-        except KeyError:
-            logger.error(f"Failed to refresh auth data: {response_data}")
-            raise
+        except KeyError as e:
+            raise ValueError(f"Failed to refresh auth data: {response_data}") from e
 
         self.save_auth_data()
         self.load_auth_data()
-
-
-async def main():
-    auth = Auth()
-    await auth.refresh_auth_data(AiohttpClient())
-    logger.info(f"{auth.access_token, auth.refresh_token, auth.expires_at = }")
-
-
-if __name__ == "__main__":
-    asyncio.run(main())
```

### Comparing `boosty-0.0.7/boosty/types/comment.py` & `boosty-0.0.8/boosty/types/comment.py`

 * *Files 20% similar despite different names*

```diff
@@ -4,16 +4,18 @@
 from pydantic import UUID4, Field
 
 from .base import BaseObject
 from .reply import RepliesResponse
 from .users import Commentator
 from .reactions import Reactions, Reacted
 from .media_types import Text, Smile, Link, Image
+from ..utils.post import render_text, Entity
 
-CommentData = Annotated[
+
+CommentContent = Annotated[
     Text | Smile | Image | Link,
     Field(discriminator="type")]
 
 
 class Comment(BaseObject):
     id: UUID4
     intId: int
@@ -24,15 +26,24 @@
     isDeleted: bool
     author: Commentator
     reactions: Reactions
     reacted: Reacted | None
     replyCount: int
     replies: RepliesResponse
     post: dict[Literal["id"], UUID4]
-    data: list[CommentData]
+    data: list[CommentContent]
+
+    @property
+    def query(self) -> str:
+        return f"?comment={self.intId}"
+
+    @property
+    def text(self) -> tuple[str, list[Entity]]:
+        return render_text(self.data)
+
 
 
 class CommentsResponseExtra(BaseObject):
     isLast: bool
     isFirst: bool | None
```

### Comparing `boosty-0.0.7/boosty/types/media_types.py` & `boosty-0.0.8/boosty/types/media_types.py`

 * *Files 15% similar despite different names*

```diff
@@ -10,26 +10,36 @@
     "quad_hd",   # 1440
     "full_hd",   # 1080
     "high",      # 720
     "medium",    # 480
     "low",       # 360
     "lowest",    # 144
     "tiny",      # 144
+    "dash",                # TODO idk
+    "dash_uni",            # TODO idk
+    "hls",                 # TODO idk
+    "tiny",                # TODO idk
+    "live_hls",            # TODO idk
+    "live_dash",           # TODO idk
+    "live_playback_hls",   # TODO idk
+    "live_playback_dash",  # TODO idk
 ]
 
 
 class PlayerUrl(BaseObject):
     type: player_urls_size_names
     url: HttpUrl | Literal[""]
 
 
 class Text(BaseObject):
     type: Literal["text"]
     content: str
+    """JSON string with list of text with entities or '' if modificator is 'BLOCK_END'"""
     modificator: str
+    """One of ['', 'BLOCK_END']"""
 
 
 class Smile(BaseObject):
     type: Literal["smile"]
     smallUrl: HttpUrl
     mediumUrl: HttpUrl
     largeUrl: HttpUrl
@@ -73,29 +83,31 @@
     album: str
     artist: str
     track: str
 
 
 class Video(FileBase):
     type: Literal["ok_video"]
+    url: HttpUrl | Literal[""]
+    """Could be '' due to boosty moment"""
     complete: bool
     """Unknown, probably True if video completely processed (could be False if Post.isRecord)"""
     title: str
     """Video title"""
     duration: int
     """Video duration in seconds"""
     width: int
     """Video max width in pixels"""
     height: int
     """Video max height in pixels"""
     playerUrls: list[PlayerUrl]
     """List of video urls for different resolutions"""
-    defaultPreview: HttpUrl
+    defaultPreview: HttpUrl | Literal[""]  # TODO SOMETIMES SERVER SENDS EMPTY STRING
     """random frame from video as thumbnail"""
-    preview: HttpUrl
+    preview: HttpUrl | Literal[""]  # TODO SOMETIMES SERVER SENDS EMPTY STRING
     """author thumbnail or defaultPreview"""
     previewId: UUID4 | None
     """author thumbnail image id or None"""
     vid: int
     """Unknown, probably ok.ru video id"""
     failoverHost: str
     """Unknown, probably interchangeable host for playerUrls"""
```

### Comparing `boosty-0.0.7/boosty/types/reply.py` & `boosty-0.0.8/boosty/types/reply.py`

 * *Files identical despite different names*

### Comparing `boosty-0.0.7/boosty/types/users.py` & `boosty-0.0.8/boosty/types/users.py`

 * *Files 9% similar despite different names*

```diff
@@ -7,27 +7,31 @@
 
 class BaseUser(BaseObject):
     id: int
     name: str
     nick: str
     hasAvatar: bool
     avatarUrl: HttpUrl | Literal[""]
+    isVerifiedStreamer: bool | None
+    """None for BlogUser"""
 
 
 class BlogUser(BaseUser):
     blogUrl: str
 
 
-class DonatorUser(BaseUser):
+class Voter(BaseUser):
     nickColor: conint(ge=0, le=15)
     """color id from 0 to 15"""
     displayName: str
     vkplayProfileLink: HttpUrl | None
-    email: EmailStr
-    isVerifiedStreamer: bool
+
+
+class DonatorUser(Voter):
+    email: EmailStr | Literal[""]
 
 
 class Commentator(BaseUser):
     nickColor: conint(ge=0, le=15)
     """color id from 0 to 15"""
     displayName: str
     vkplayProfileLink: HttpUrl | Literal[""]
```

### Comparing `boosty-0.0.7/boosty/utils/client.py` & `boosty-0.0.8/boosty/utils/client.py`

 * *Files identical despite different names*

### Comparing `boosty-0.0.7/boosty/utils/post.py` & `boosty-0.0.8/boosty/utils/post.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,16 +1,21 @@
 import re
 from struct import unpack
+from typing import TYPE_CHECKING
 
-from boosty.types import Post, Content
 from boosty.types.base import schema_strict
+from boosty.types.comment import Comment
 from boosty.types.media_types import Text, Link
 from boosty.utils.json import json
 from pydantic import BaseModel, HttpUrl
 
+if TYPE_CHECKING:
+    from boosty.types import Post, Content
+
+
 # pyrogram/parser/utils.py:19@626a1bd
 # SMP = Supplementary Multilingual Plane: https://en.wikipedia.org/wiki/Plane_(Unicode)#Overview
 SMP_RE = re.compile(r"[\U00010000-\U0010FFFF]")
 
 
 def add_surrogates(text):
     # Replace each SMP code point with a surrogate pair
@@ -18,29 +23,25 @@
         lambda match:  # Split SMP in two surrogates
         "".join(chr(i) for i in unpack("<HH", match.group().encode("utf-16le"))),
         text
     )
 # pyrogram/parser/utils.py:41@626a1bd
 
 
-def get_post_url(post: Post) -> HttpUrl:
-    """Get post url"""
-    return HttpUrl(f"https://boosty.to/{post.user.blogUrl}/posts/{post.id}", scheme="https")
-
-
 class Entity(BaseModel):
     """Telegram-like entity"""
     type: str
     offset: int
     length: int
     url: str = None
 
 
 def render_text(
-        post_data: list[Content], *,
+        post_data: list["Content"],
+        *,
         header="", placeholder="\n\n",
         fix_long_newlines=True, fix_end_newlines=True,
 ) -> tuple[str, list[Entity]]:
     """
     :param post_data: any of boosty.types.media_types (types other than Text and Link will create placeholder)
     :param header: header for output text (for correct offsets)
     :param placeholder: placeholder for non-text content
@@ -92,14 +93,16 @@
                     format_type, offset, length = format_list
                     if format_type == 0:
                         entity_type = "bold"
                     elif format_type == 2:
                         entity_type = "italic"
                     elif format_type == 4:
                         entity_type = "underline"
+                    elif format_type is None:
+                        continue  # TODO unknown format in comments [None, 64, 0]
                     else:
                         if schema_strict:
                             raise ValueError(
                                 f"TEXT PARSER ERROR\n"
                                 f"Unknown style\n"
                                 f"{raw_text, raw_unstyled, raw_entities =}")
                         continue
@@ -113,7 +116,11 @@
         elif text:
             text.strip()
             text += placeholder
 
     while fix_end_newlines and text.endswith("\n"):
         text = text[:-1]
     return text, entities
+
+
+def get_comment_url(post: "Post", comment: "Comment") -> HttpUrl:
+    return HttpUrl(f"{post.url.query}{comment.query}", scheme="https")
```

### Comparing `boosty-0.0.7/boosty/utils/video.py` & `boosty-0.0.8/boosty/utils/video.py`

 * *Files 13% similar despite different names*

```diff
@@ -33,15 +33,22 @@
     "ultra_hd": 7,
     "quad_hd": 6,
     "full_hd": 5,
     "high": 3,
     "medium": 2,
     "low": 1,
     "lowest": 0,
-    "tiny": -1,  # 4
+    "dash": -1,
+    "dash_uni": -2,
+    "hls": -3,  # 4
+    "tiny": -4,
+    "live_playback_dash": -6,
+    "live_playback_hls": -7,
+    "live_dash": -8,
+    "live_hls": -9,
 }
 player_size_by_number: dict[int, player_urls_size_names] = {v: k for k, v in player_size_dict.items()}  # type: ignore
 
 
 class VideoSize(BaseObject):
     name: size_names
     url: HttpUrl
```

### Comparing `boosty-0.0.7/.gitignore` & `boosty-0.0.8/.gitignore`

 * *Files identical despite different names*

### Comparing `boosty-0.0.7/LICENSE` & `boosty-0.0.8/LICENSE`

 * *Files identical despite different names*

### Comparing `boosty-0.0.7/README.md` & `boosty-0.0.8/README.md`

 * *Files 15% similar despite different names*

```diff
@@ -51,13 +51,23 @@
 from boosty.api import API
 
 api = API()
 response = await api.get_post("boosty", post_id="c9fb8a19-c45e-4602-9942-087c3af28c1b")
 print(response.title)
 # 'Добро пожаловать на борт!'
 ```
+More examples in [examples/](examples/) folder
 
 ### TODO for stable release
 - api schema
   - add access levels logic for requests
 - minimal docs
-- tests
+- useful properties for models
+- merge reply comment with comment model 
+- add examples
+  - render text
+  - get video url
+  - get comment url
+- add tests
+  - boosty profile
+  - comments
+  - replies
```

#### html2text {}

```diff
@@ -13,10 +13,13 @@
 with authentication data: ```json { "access_token":
 "ffffffffffffffffffffffffffffffffffffffffffffffffffffffffffffffff",
 "device_id": "ffffffff-ffff-ffff-ffff-ffffffffffff", "expires_at": 12345678900,
 "refresh_token":
 "ffffffffffffffffffffffffffffffffffffffffffffffffffffffffffffffff" } ```
 Example: ```python from boosty.api import API api = API() response = await
 api.get_post("boosty", post_id="c9fb8a19-c45e-4602-9942-087c3af28c1b") print
-(response.title) # 'ÐÐ¾Ð±ÑÐ¾ Ð¿Ð¾Ð¶Ð°Ð»Ð¾Ð²Ð°ÑÑ Ð½Ð° Ð±Ð¾ÑÑ!' ``` ###
-TODO for stable release - api schema - add access levels logic for requests -
-minimal docs - tests
+(response.title) # 'ÐÐ¾Ð±ÑÐ¾ Ð¿Ð¾Ð¶Ð°Ð»Ð¾Ð²Ð°ÑÑ Ð½Ð° Ð±Ð¾ÑÑ!' ``` More
+examples in [examples/](examples/) folder ### TODO for stable release - api
+schema - add access levels logic for requests - minimal docs - useful
+properties for models - merge reply comment with comment model - add examples -
+render text - get video url - get comment url - add tests - boosty profile -
+comments - replies
```

### Comparing `boosty-0.0.7/pyproject.toml` & `boosty-0.0.8/pyproject.toml`

 * *Files identical despite different names*

### Comparing `boosty-0.0.7/PKG-INFO` & `boosty-0.0.8/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: boosty
-Version: 0.0.7
+Version: 0.0.8
 Summary: Asynchronous boosty wrapper with some utils
 Project-URL: Documentation, https://github.com/barsikus007/boosty#readme
 Project-URL: Issues, https://github.com/barsikus007/boosty/issues
 Project-URL: Source, https://github.com/barsikus007/boosty
 Author: barsikus007
 License-Expression: MIT
 License-File: LICENSE
@@ -82,13 +82,23 @@
 from boosty.api import API
 
 api = API()
 response = await api.get_post("boosty", post_id="c9fb8a19-c45e-4602-9942-087c3af28c1b")
 print(response.title)
 # 'Добро пожаловать на борт!'
 ```
+More examples in [examples/](examples/) folder
 
 ### TODO for stable release
 - api schema
   - add access levels logic for requests
 - minimal docs
-- tests
+- useful properties for models
+- merge reply comment with comment model 
+- add examples
+  - render text
+  - get video url
+  - get comment url
+- add tests
+  - boosty profile
+  - comments
+  - replies
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: boosty Version: 0.0.7 Summary: Asynchronous boosty
+Metadata-Version: 2.1 Name: boosty Version: 0.0.8 Summary: Asynchronous boosty
 wrapper with some utils Project-URL: Documentation, https://github.com/
 barsikus007/boosty#readme Project-URL: Issues, https://github.com/barsikus007/
 boosty/issues Project-URL: Source, https://github.com/barsikus007/boosty
 Author: barsikus007 License-Expression: MIT License-File: LICENSE Keywords:
 asyncio,boosty,wrapper Classifier: Development Status :: 4 - Beta Classifier:
 Programming Language :: Python Classifier: Programming Language :: Python ::
 3.10 Classifier: Programming Language :: Python :: 3.11 Classifier: Programming
@@ -29,10 +29,13 @@
 with authentication data: ```json { "access_token":
 "ffffffffffffffffffffffffffffffffffffffffffffffffffffffffffffffff",
 "device_id": "ffffffff-ffff-ffff-ffff-ffffffffffff", "expires_at": 12345678900,
 "refresh_token":
 "ffffffffffffffffffffffffffffffffffffffffffffffffffffffffffffffff" } ```
 Example: ```python from boosty.api import API api = API() response = await
 api.get_post("boosty", post_id="c9fb8a19-c45e-4602-9942-087c3af28c1b") print
-(response.title) # 'ÐÐ¾Ð±ÑÐ¾ Ð¿Ð¾Ð¶Ð°Ð»Ð¾Ð²Ð°ÑÑ Ð½Ð° Ð±Ð¾ÑÑ!' ``` ###
-TODO for stable release - api schema - add access levels logic for requests -
-minimal docs - tests
+(response.title) # 'ÐÐ¾Ð±ÑÐ¾ Ð¿Ð¾Ð¶Ð°Ð»Ð¾Ð²Ð°ÑÑ Ð½Ð° Ð±Ð¾ÑÑ!' ``` More
+examples in [examples/](examples/) folder ### TODO for stable release - api
+schema - add access levels logic for requests - minimal docs - useful
+properties for models - merge reply comment with comment model - add examples -
+render text - get video url - get comment url - add tests - boosty profile -
+comments - replies
```

