# Comparing `tmp/python_substack-0.1.8.tar.gz` & `tmp/python_substack-0.1.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "python_substack-0.1.8.tar", max compression
+gzip compressed data, was "python_substack-0.1.9.tar", max compression
```

## Comparing `python_substack-0.1.8.tar` & `python_substack-0.1.9.tar`

### file list

```diff
@@ -1,8 +1,8 @@
--rw-r--r--   0        0        0     1063 2023-05-24 14:01:21.167468 python_substack-0.1.8/LICENSE
--rw-r--r--   0        0        0      745 2023-05-24 14:01:21.167468 python_substack-0.1.8/README.md
--rw-r--r--   0        0        0      619 2023-05-24 14:01:21.171468 python_substack-0.1.8/pyproject.toml
--rw-r--r--   0        0        0      388 2023-05-24 14:01:21.171468 python_substack-0.1.8/substack/__init__.py
--rw-r--r--   0        0        0     8472 2023-05-24 14:01:21.171468 python_substack-0.1.8/substack/api.py
--rw-r--r--   0        0        0      841 2023-05-24 14:01:21.171468 python_substack-0.1.8/substack/exceptions.py
--rw-r--r--   0        0        0     7104 2023-05-24 14:01:21.171468 python_substack-0.1.8/substack/post.py
--rw-r--r--   0        0        0     1610 1970-01-01 00:00:00.000000 python_substack-0.1.8/PKG-INFO
+-rw-r--r--   0        0        0     1062 2023-06-12 02:56:25.239141 python_substack-0.1.9/LICENSE
+-rw-r--r--   0        0        0     1641 2023-06-12 02:56:25.239141 python_substack-0.1.9/README.md
+-rw-r--r--   0        0        0      619 2023-06-12 02:56:25.243141 python_substack-0.1.9/pyproject.toml
+-rw-r--r--   0        0        0      387 2023-06-12 02:56:25.243141 python_substack-0.1.9/substack/__init__.py
+-rw-r--r--   0        0        0     8838 2023-06-12 02:56:25.243141 python_substack-0.1.9/substack/api.py
+-rw-r--r--   0        0        0      841 2023-06-12 02:56:25.243141 python_substack-0.1.9/substack/exceptions.py
+-rw-r--r--   0        0        0     7426 2023-06-12 02:56:25.243141 python_substack-0.1.9/substack/post.py
+-rw-r--r--   0        0        0     2506 1970-01-01 00:00:00.000000 python_substack-0.1.9/PKG-INFO
```

### Comparing `python_substack-0.1.8/LICENSE` & `python_substack-0.1.9/LICENSE`

 * *Files 22% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 MIT License
 
-Copyright (c) 2022 hogier
+Copyright (c) 2022 ma2za
 
 Permission is hereby granted, free of charge, to any person obtaining a copy
 of this software and associated documentation files (the "Software"), to deal
 in the Software without restriction, including without limitation the rights
 to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
 copies of the Software, and to permit persons to whom the Software is
 furnished to do so, subject to the following conditions:
```

### Comparing `python_substack-0.1.8/pyproject.toml` & `python_substack-0.1.9/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "python-substack"
-version = "0.1.8"
+version = "0.1.9"
 description = "A Python wrapper around the Substack API."
 authors = ["Paolo Mazza <mazzapaolo2019@gmail.com>"]
 license = "MIT"
 packages = [
     { include = "substack" }
 ]
 
@@ -14,15 +14,15 @@
 homepage = "https://github.com/ma2za/python-substack"
 
 keywords = ["substack"]
 
 [tool.poetry.dependencies]
 python = "^3.7"
 
-requests = "^2.28.1"
+requests = "^2.31.0"
 python-dotenv = "^0.21.0"
 PyYAML = "^6.0"
 
 
 [tool.poetry.dev-dependencies]
```

### Comparing `python_substack-0.1.8/substack/api.py` & `python_substack-0.1.9/substack/api.py`

 * *Files 4% similar despite different names*

```diff
@@ -6,14 +6,16 @@
 
 import requests
 
 from substack.exceptions import SubstackAPIException, SubstackRequestException
 
 logger = logging.getLogger(__name__)
 
+__all__ = ["Api"]
+
 
 class Api:
     """
 
     A python interface into the Substack API
 
     """
@@ -88,41 +90,60 @@
         try:
             return response.json()
         except ValueError:
             raise SubstackRequestException("Invalid Response: %s" % response.text)
 
     def get_publication_users(self):
         """
+        Get list of users.
+
+        Returns:
 
-        :return:
         """
         response = self._session.get(f"{self.publication_url}/publication/users")
 
         return Api._handle_response(response=response)
 
     def get_posts(self) -> dict:
         """
 
-        :return:
+        Returns:
+
         """
         response = self._session.get(f"{self.base_url}/reader/posts")
 
         return Api._handle_response(response=response)
 
     def get_drafts(self, filter=None, offset=None, limit=None):
+        """
+
+        Args:
+            filter:
+            offset:
+            limit:
+
+        Returns:
+
+        """
         response = self._session.get(
             f"{self.publication_url}/drafts",
             params={"filter": filter, "offset": offset, "limit": limit},
         )
         return Api._handle_response(response=response)
 
     def delete_draft(self, draft_id):
-        response = self._session.delete(
-            f"{self.publication_url}/drafts/{draft_id}"
-        )
+        """
+
+        Args:
+            draft_id:
+
+        Returns:
+
+        """
+        response = self._session.delete(f"{self.publication_url}/drafts/{draft_id}")
         return Api._handle_response(response=response)
 
     def post_draft(self, body) -> dict:
         """
 
         Args:
           body:
@@ -207,30 +228,29 @@
             draft_datetime: datetime to schedule the draft
 
         Returns:
 
         """
         response = self._session.post(
             f"{self.publication_url}/drafts/{draft}/schedule",
-            json={"post_date": draft_datetime.isoformat()}
+            json={"post_date": draft_datetime.isoformat()},
         )
         return Api._handle_response(response=response)
 
     def unschedule_draft(self, draft) -> dict:
         """
 
         Args:
             draft: draft id
 
         Returns:
 
         """
         response = self._session.post(
-            f"{self.publication_url}/drafts/{draft}/schedule",
-            json={"post_date": None}
+            f"{self.publication_url}/drafts/{draft}/schedule", json={"post_date": None}
         )
         return Api._handle_response(response=response)
 
     def get_image(self, image: str):
         """
 
         This method generates a new substack link that contains the image.
@@ -243,17 +263,15 @@
         """
         if os.path.exists(image):
             with open(image, "rb") as file:
                 image = b"data:image/jpeg;base64," + base64.b64encode(file.read())
 
         response = self._session.post(
             f"{self.publication_url}/image",
-            data={
-                "image": image
-            },
+            data={"image": image},
         )
         return Api._handle_response(response=response)
 
     def get_categories(self):
         """
 
         Retrieve list of all available categories.
@@ -261,20 +279,31 @@
         Returns:
 
         """
         response = self._session.get(f"{self.base_url}/categories")
         return Api._handle_response(response=response)
 
     def get_category(self, category_id, category_type, page):
-        response = self._session.get(f"{self.base_url}/category/public/{category_id}/{category_type}",
-                                     params={"page": page})
+        """
+
+        Args:
+            category_id:
+            category_type:
+            page:
+
+        Returns:
+
+        """
+        response = self._session.get(
+            f"{self.base_url}/category/public/{category_id}/{category_type}",
+            params={"page": page},
+        )
         return Api._handle_response(response=response)
 
-    def get_single_category(self, category_id, category_type, page=None,
-                            limit=None):
+    def get_single_category(self, category_id, category_type, page=None, limit=None):
         """
 
         Args:
             category_id:
             category_type: paid or all
             page: by default substack retrieves only the first 25 publications in the category. If this is left None,
                   then all pages will be retrieved. The page size is 25 publications.
@@ -286,25 +315,32 @@
             output = self.get_category(category_id, category_type, page)
         else:
             publications = []
             page = 0
             while True:
                 page_output = self.get_category(category_id, category_type, page)
                 publications.extend(page_output.get("publications", []))
-                if (limit is not None and limit <= len(publications)) or not page_output.get("more", False):
+                if (
+                        limit is not None and limit <= len(publications)
+                ) or not page_output.get("more", False):
                     publications = publications[:limit]
                     break
                 page += 1
             output = {
                 "publications": publications,
-                "more": page_output.get("more", False)
+                "more": page_output.get("more", False),
             }
         return output
 
     def delete_all_drafts(self):
+        """
+
+        Returns:
+
+        """
         response = None
         while True:
             drafts = self.get_drafts(filter="draft", limit=10, offset=0)
             if len(drafts) == 0:
                 break
             for draft in drafts:
                 response = self.delete_draft(draft.get("id"))
```

### Comparing `python_substack-0.1.8/substack/exceptions.py` & `python_substack-0.1.9/substack/exceptions.py`

 * *Files identical despite different names*

### Comparing `python_substack-0.1.8/substack/post.py` & `python_substack-0.1.9/substack/post.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,16 +1,22 @@
 import json
 from typing import Dict
 
+__all__ = ["Post"]
 
-class Post:
 
-    def __init__(self, title: str, subtitle: str, user_id,
-                 audience: str = None,
-                 write_comment_permissions: str = None):
+class Post:
+    def __init__(
+            self,
+            title: str,
+            subtitle: str,
+            user_id,
+            audience: str = None,
+            write_comment_permissions: str = None,
+    ):
         """
 
         Args:
             title:
             subtitle:
             user_id:
             audience: possible values: everyone, only_paid, founding, only_free
@@ -36,15 +42,17 @@
         Args:
             item:
 
         Returns:
 
         """
 
-        self.draft_body["content"] = self.draft_body.get("content", []) + [{"type": item.get("type")}]
+        self.draft_body["content"] = self.draft_body.get("content", []) + [
+            {"type": item.get("type")}
+        ]
         content = item.get("content")
         if item.get("type") == "captionedImage":
             self.captioned_image(**item)
         elif item.get("type") == "youtube2":
             self.youtube(item.get("src"))
         else:
             if content is not None:
@@ -108,29 +116,30 @@
 
         """
         content_attrs = self.draft_body["content"][-1].get("attrs", {})
         content_attrs.update({"level": level})
         self.draft_body["content"][-1]["attrs"] = content_attrs
         return self
 
-    def captioned_image(self,
-                        src: str,
-                        fullscreen: bool = False,
-                        imageSize: str = "normal",
-                        height: int = 819,
-                        width: int = 1456,
-                        resizeWidth: int = 728,
-                        bytes: str = None,
-                        alt: str = None,
-                        title: str = None,
-                        type: str = None,
-                        href: str = None,
-                        belowTheFold: bool = False,
-                        internalRedirect: str = None
-                        ):
+    def captioned_image(
+            self,
+            src: str,
+            fullscreen: bool = False,
+            imageSize: str = "normal",
+            height: int = 819,
+            width: int = 1456,
+            resizeWidth: int = 728,
+            bytes: str = None,
+            alt: str = None,
+            title: str = None,
+            type: str = None,
+            href: str = None,
+            belowTheFold: bool = False,
+            internalRedirect: str = None,
+    ):
         """
 
         Add image to body.
 
         Args:
             bytes:
             alt:
@@ -144,30 +153,34 @@
             imageSize:
             height:
             width:
             resizeWidth:
         """
 
         content = self.draft_body["content"][-1].get("content", [])
-        content += [{"type": "image2", "attrs": {
-            "src": src,
-            "fullscreen": fullscreen,
-            "imageSize": imageSize,
-            "height": height,
-            "width": width,
-            "resizeWidth": resizeWidth,
-            "bytes": bytes,
-            "alt": alt,
-            "title": title,
-            "type": type,
-            "href": href,
-            "belowTheFold": belowTheFold,
-            "internalRedirect": internalRedirect
-
-        }}]
+        content += [
+            {
+                "type": "image2",
+                "attrs": {
+                    "src": src,
+                    "fullscreen": fullscreen,
+                    "imageSize": imageSize,
+                    "height": height,
+                    "width": width,
+                    "resizeWidth": resizeWidth,
+                    "bytes": bytes,
+                    "alt": alt,
+                    "title": title,
+                    "type": type,
+                    "href": href,
+                    "belowTheFold": belowTheFold,
+                    "internalRedirect": internalRedirect,
+                },
+            }
+        ]
         self.draft_body["content"][-1]["content"] = content
         return self
 
     def text(self, value: str):
         """
 
         Add text to the last paragraph.
@@ -207,65 +220,77 @@
         """
         content = self.draft_body["content"][-1].get("content", [])[-1]
         content_marks = content.get("marks", [])
         for mark in marks:
             new_mark = {"type": mark.get("type")}
             if mark.get("type") == "link":
                 href = mark.get("href")
-                new_mark.update({"attrs": {
-                    "href": href
-                }})
+                new_mark.update({"attrs": {"href": href}})
             content_marks.append(new_mark)
         content["marks"] = content_marks
         return self
 
     def remove_last_paragraph(self):
-        """
-
-        """
+        """ """
         del self.draft_body.get("content")[-1]
 
     def get_draft(self):
         """
 
         Returns:
 
         """
         out = vars(self)
         out["draft_body"] = json.dumps(out["draft_body"])
         return out
 
-    def subscribe_with_caption(self, value: str):
+    def subscribe_with_caption(self, message: str = None):
         """
 
+        Add subscribe widget with caption
+
         Args:
-            value:
+            message:
 
         Returns:
 
         """
+
+        if message is None:
+            message = """Thanks for reading this newsletter!
+            Subscribe for free to receive new posts and support my work."""
+
         content = self.draft_body["content"][-1].get("content", [])
-        content += [{"type": "subscribeWidget",
-                     "attrs": {"url": "%%checkout_url%%", "text": "Subscribe"},
-                     "content": [
-                         {
-                             "type": "ctaCaption",
-                             "content": [{"type": "text",
-                                          "text": f"""Thanks for reading {value}! 
-                                          Subscribe for free to receive new posts and support my work."""}]
-                         }
-                     ]}]
+        content += [
+            {
+                "type": "subscribeWidget",
+                "attrs": {"url": "%%checkout_url%%", "text": "Subscribe"},
+                "content": [
+                    {
+                        "type": "ctaCaption",
+                        "content": [
+                            {
+                                "type": "text",
+                                "text": message,
+                            }
+                        ],
+                    }
+                ],
+            }
+        ]
         self.draft_body["content"][-1]["content"] = content
         return self
 
     def youtube(self, value: str):
         """
 
+        Add youtube video to post.
+
         Args:
-            value:
+            value: youtube url
 
         Returns:
 
         """
         content_attrs = self.draft_body["content"][-1].get("attrs", {})
         content_attrs.update({"videoId": value})
         self.draft_body["content"][-1]["attrs"] = content_attrs
```

