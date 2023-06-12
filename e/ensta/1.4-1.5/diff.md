# Comparing `tmp/ensta-1.4.tar.gz` & `tmp/ensta-1.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ensta-1.4.tar", last modified: Fri Jun  9 09:29:00 2023, max compression
+gzip compressed data, was "ensta-1.5.tar", last modified: Mon Jun 12 16:04:13 2023, max compression
```

## Comparing `ensta-1.4.tar` & `ensta-1.5.tar`

### file list

```diff
@@ -1,26 +1,27 @@
-drwxrwxrwx   0        0        0        0 2023-06-09 09:29:00.500176 ensta-1.4/
--rw-rw-rw-   0        0        0     1081 2023-06-06 15:38:39.000000 ensta-1.4/LICENSE.txt
--rw-rw-rw-   0        0        0     3368 2023-06-09 09:29:00.500176 ensta-1.4/PKG-INFO
--rw-rw-rw-   0        0        0     2646 2023-06-08 05:38:39.000000 ensta-1.4/README.md
-drwxrwxrwx   0        0        0        0 2023-06-09 09:29:00.453258 ensta-1.4/ensta/
--rw-rw-rw-   0        0        0    11420 2023-06-09 09:07:44.000000 ensta-1.4/ensta/Guest.py
--rw-rw-rw-   0        0        0    19816 2023-06-09 09:23:24.000000 ensta-1.4/ensta/Host.py
--rw-rw-rw-   0        0        0       60 2023-06-09 05:22:01.000000 ensta-1.4/ensta/__init__.py
-drwxrwxrwx   0        0        0        0 2023-06-09 09:29:00.500176 ensta-1.4/ensta/containers/
--rw-rw-rw-   0        0        0      347 2023-06-09 08:53:51.000000 ensta-1.4/ensta/containers/FollowPerson.py
--rw-rw-rw-   0        0        0      222 2023-06-09 08:46:48.000000 ensta-1.4/ensta/containers/FollowedStatus.py
--rw-rw-rw-   0        0        0      584 2023-06-09 07:33:57.000000 ensta-1.4/ensta/containers/Profile.py
--rw-rw-rw-   0        0        0      153 2023-06-09 08:28:13.000000 ensta-1.4/ensta/containers/UnfollowedStatus.py
--rw-rw-rw-   0        0        0      162 2023-06-09 08:48:05.000000 ensta-1.4/ensta/containers/__init__.py
-drwxrwxrwx   0        0        0        0 2023-06-09 09:29:00.500176 ensta-1.4/ensta/lib/
--rw-rw-rw-   0        0        0     1424 2023-06-09 09:01:13.000000 ensta-1.4/ensta/lib/Commons.py
--rw-rw-rw-   0        0        0      616 2023-06-09 09:10:35.000000 ensta-1.4/ensta/lib/Exceptions.py
--rw-rw-rw-   0        0        0      298 2023-06-09 09:10:42.000000 ensta-1.4/ensta/lib/__init__.py
-drwxrwxrwx   0        0        0        0 2023-06-09 09:29:00.468789 ensta-1.4/ensta.egg-info/
--rw-rw-rw-   0        0        0     3368 2023-06-09 09:29:00.000000 ensta-1.4/ensta.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      460 2023-06-09 09:29:00.000000 ensta-1.4/ensta.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-06-09 09:29:00.000000 ensta-1.4/ensta.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        9 2023-06-09 09:29:00.000000 ensta-1.4/ensta.egg-info/requires.txt
--rw-rw-rw-   0        0        0        6 2023-06-09 09:29:00.000000 ensta-1.4/ensta.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       86 2023-06-09 09:29:00.500176 ensta-1.4/setup.cfg
--rw-rw-rw-   0        0        0     1052 2023-06-09 09:28:43.000000 ensta-1.4/setup.py
+drwxrwxrwx   0        0        0        0 2023-06-12 16:04:13.225485 ensta-1.5/
+-rw-rw-rw-   0        0        0     1081 2023-06-06 15:38:39.000000 ensta-1.5/LICENSE.txt
+-rw-rw-rw-   0        0        0     6100 2023-06-12 16:04:13.225485 ensta-1.5/PKG-INFO
+-rw-rw-rw-   0        0        0     5365 2023-06-12 15:53:10.000000 ensta-1.5/README.md
+drwxrwxrwx   0        0        0        0 2023-06-12 16:04:13.162726 ensta-1.5/ensta/
+-rw-rw-rw-   0        0        0    11201 2023-06-12 15:22:13.000000 ensta-1.5/ensta/Guest.py
+-rw-rw-rw-   0        0        0    12446 2023-06-12 15:23:46.000000 ensta-1.5/ensta/Host.py
+-rw-rw-rw-   0        0        0    14411 2023-06-12 15:13:54.000000 ensta-1.5/ensta/Stream.py
+-rw-rw-rw-   0        0        0       93 2023-06-12 14:44:37.000000 ensta-1.5/ensta/__init__.py
+drwxrwxrwx   0        0        0        0 2023-06-12 16:04:13.209656 ensta-1.5/ensta/containers/
+-rw-rw-rw-   0        0        0      347 2023-06-09 08:53:51.000000 ensta-1.5/ensta/containers/FollowPerson.py
+-rw-rw-rw-   0        0        0      222 2023-06-09 08:46:48.000000 ensta-1.5/ensta/containers/FollowedStatus.py
+-rw-rw-rw-   0        0        0      584 2023-06-09 07:33:57.000000 ensta-1.5/ensta/containers/Profile.py
+-rw-rw-rw-   0        0        0      153 2023-06-09 08:28:13.000000 ensta-1.5/ensta/containers/UnfollowedStatus.py
+-rw-rw-rw-   0        0        0      162 2023-06-09 08:48:05.000000 ensta-1.5/ensta/containers/__init__.py
+drwxrwxrwx   0        0        0        0 2023-06-12 16:04:13.225485 ensta-1.5/ensta/lib/
+-rw-rw-rw-   0        0        0     1424 2023-06-09 09:01:13.000000 ensta-1.5/ensta/lib/Commons.py
+-rw-rw-rw-   0        0        0      597 2023-06-09 15:54:08.000000 ensta-1.5/ensta/lib/Exceptions.py
+-rw-rw-rw-   0        0        0      298 2023-06-09 09:10:42.000000 ensta-1.5/ensta/lib/__init__.py
+drwxrwxrwx   0        0        0        0 2023-06-12 16:04:13.192954 ensta-1.5/ensta.egg-info/
+-rw-rw-rw-   0        0        0     6100 2023-06-12 16:04:13.000000 ensta-1.5/ensta.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      476 2023-06-12 16:04:13.000000 ensta-1.5/ensta.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-06-12 16:04:13.000000 ensta-1.5/ensta.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        9 2023-06-12 16:04:13.000000 ensta-1.5/ensta.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        6 2023-06-12 16:04:13.000000 ensta-1.5/ensta.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       86 2023-06-12 16:04:13.240008 ensta-1.5/setup.cfg
+-rw-rw-rw-   0        0        0     1081 2023-06-12 16:04:02.000000 ensta-1.5/setup.py
```

### Comparing `ensta-1.4/LICENSE.txt` & `ensta-1.5/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `ensta-1.4/ensta/Guest.py` & `ensta-1.5/ensta/Guest.py`

 * *Files 3% similar despite different names*

```diff
@@ -69,18 +69,16 @@
             response_json = http_response.json()
 
             if "errors" in response_json:
                 return "username" not in response_json["errors"]
         except JSONDecodeError:
             return None
 
-    def profile(self, username: str) -> Profile:
+    def profile(self, username: str, __session__: requests.Session = None) -> Profile | None:
         username = format_username(username)
-        failure_response = Profile()
-
         refresh_csrf_token(self)
         request_headers = {
             "accept": "*/*",
             "accept-language": "en-US,en;q=0.9",
             "sec-ch-prefers-color-scheme": random.choice(["light", "dark"]),
             "sec-ch-ua": "\"Not.A/Brand\";v=\"8\", \"Chromium\";v=\"114\", \"Google Chrome\";v=\"114\"",
             "sec-ch-ua-full-version-list": "\"Not.A/Brand\";v=\"8.0.0.0\", \"Chromium\";v=\"114.0.5735.91\", \"Google Chrome\";v=\"114.0.5735.91\"",
@@ -97,15 +95,18 @@
             "x-ig-www-claim": "0",
             "x-requested-with": "XMLHttpRequest",
             "Referer": f"https://www.instagram.com/{username}/",
             "Referrer-Policy": "strict-origin-when-cross-origin"
         }
 
         try:
-            http_response = self.request_session.get(
+            session = __session__
+            if __session__ is None: session = self.request_session
+
+            http_response = session.get(
                 f"https://www.instagram.com/api/v1/users/web_profile_info/?username={username}",
                 headers=request_headers
             )
             response_json = http_response.json()
 
             if "status" in response_json:
                 if response_json["status"] == "ok" and "data" in response_json:
@@ -174,38 +175,33 @@
 
                         if "pronouns" in response_json["data"]["user"]:
                             user_pronouns = []
                             for pronoun in response_json["data"]["user"]["pronouns"]:
                                 user_pronouns.append(pronoun)
                             profile_object_pronouns = user_pronouns
 
-                        return Profile(biography=profile_object_biography,
-                                       country_block=profile_object_country_block,
-                                       full_name=profile_object_full_name,
-                                       follower_count=profile_object_follower_count,
-                                       following_count=profile_object_following_count,
-                                       user_id=profile_object_user_id,
-                                       is_business_account=profile_object_is_business_account,
-                                       is_professional_account=profile_object_is_professional_account,
-                                       is_supervision_enabled=profile_object_is_supervision_enabled,
-                                       is_joined_recently=profile_object_is_joined_recently,
-                                       is_private=profile_object_is_private,
-                                       is_verified=profile_object_is_verified,
-                                       profile_picture_url=profile_object_profile_picture_url,
-                                       profile_picture_url_hd=profile_object_profile_picture_url_hd,
-                                       pronouns=profile_object_pronouns)
-
-                    else:
-                        return failure_response
-                else:
-                    return failure_response
-            else:
-                return failure_response
+                        return Profile(
+                            biography=profile_object_biography,
+                            country_block=profile_object_country_block,
+                            full_name=profile_object_full_name,
+                            follower_count=profile_object_follower_count,
+                            following_count=profile_object_following_count,
+                            user_id=profile_object_user_id,
+                            is_business_account=profile_object_is_business_account,
+                            is_professional_account=profile_object_is_professional_account,
+                            is_supervision_enabled=profile_object_is_supervision_enabled,
+                            is_joined_recently=profile_object_is_joined_recently,
+                            is_private=profile_object_is_private,
+                            is_verified=profile_object_is_verified,
+                            profile_picture_url=profile_object_profile_picture_url,
+                            profile_picture_url_hd=profile_object_profile_picture_url_hd,
+                            pronouns=profile_object_pronouns
+                        )
         except JSONDecodeError:
-            return failure_response
+            return None
 
     def get_uid(self, username: str) -> str | None:
         username = username.strip().lower().replace(" ", "")
         response = self.profile(username)
 
         if response.user_id is not None:
             return format_uid(response.user_id)
```

### Comparing `ensta-1.4/ensta/Host.py` & `ensta-1.5/ensta/Stream.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,11 +1,12 @@
 import requests
 from json import JSONDecodeError
 import random
 import string
+from collections.abc import Generator
 from .Guest import Guest
 from .lib.Commons import (
     refresh_csrf_token,
     update_app_id,
     update_homepage_source,
     update_session,
     format_identifier
@@ -13,21 +14,20 @@
 from .lib import (
     AuthenticationError,
     NetworkError,
     IdentifierError,
     CodeError
 )
 from .containers import FollowPerson
-from .containers import (FollowedStatus, UnfollowedStatus)
 
 USERNAME = 0
 UID = 1
 
 
-class Host:
+class Stream:
     request_session: requests.Session = None
     homepage_source: str = None
     insta_app_id: str = None
     preferred_color_scheme: str = "dark"
     x_ig_www_claim: str = None
     csrf_token: str = None
     guest: Guest = None
@@ -40,26 +40,26 @@
         self.guest = Guest(
             homepage_source=self.homepage_source,
             insta_app_id=self.insta_app_id
         )
 
         self.request_session.cookies.set("sessionid", session_id)
 
-        if not self.is_authenticated():
+        if not self.authenticated():
             raise AuthenticationError("Either User ID or Session ID is not valid.")
 
     def update_homepage_source(self) -> None:
         temp_homepage_source = requests.get("https://www.instagram.com/").text.strip()
 
         if temp_homepage_source == "":
             raise NetworkError("Couldn't load instagram homepage.")
 
         self.homepage_source = temp_homepage_source
 
-    def is_authenticated(self) -> bool:
+    def authenticated(self) -> bool:
         refresh_csrf_token(self)
         request_headers = {
             "accept": "*/*",
             "accept-language": "en-US,en;q=0.9",
             "sec-ch-prefers-color-scheme": self.preferred_color_scheme,
             "sec-ch-ua": "\"Not.A/Brand\";v=\"8\", \"Chromium\";v=\"114\", \"Google Chrome\";v=\"114\"",
             "sec-ch-ua-full-version-list": "\"Not.A/Brand\";v=\"8.0.0.0\", \"Chromium\";v=\"114.0.5735.91\", \"Google Chrome\";v=\"114.0.5735.91\"",
@@ -82,123 +82,20 @@
 
         try:
             http_response.json()
             return True
         except JSONDecodeError:
             return False
 
-    def follow(self, identifier: str | int) -> FollowedStatus | None:
-        conversion_success, identifier = self.identifier_conversion(identifier, UID)
-        if not conversion_success: return None
-
-        # Actual Request
-        refresh_csrf_token(self)
-        body_json = {
-            "container_module": "profile",
-            "nav_chain": f"PolarisProfileRoot:profilePage:1:via_cold_start",
-            "user_id": identifier
-        }
-        request_headers = {
-            "accept": "*/*",
-            "accept-language": "en-US,en;q=0.9",
-            "content-type": "application/x-www-form-urlencoded",
-            "sec-ch-prefers-color-scheme": self.preferred_color_scheme,
-            "sec-ch-ua": "\"Not.A/Brand\";v=\"8\", \"Chromium\";v=\"114\", \"Google Chrome\";v=\"114\"",
-            "sec-ch-ua-full-version-list": "\"Not.A/Brand\";v=\"8.0.0.0\", \"Chromium\";v=\"114.0.5735.91\", \"Google Chrome\";v=\"114.0.5735.91\"",
-            "sec-ch-ua-mobile": "?0",
-            "sec-ch-ua-platform": "\"Windows\"",
-            "sec-ch-ua-platform-version": "\"15.0.0\"",
-            "sec-fetch-dest": "empty",
-            "sec-fetch-mode": "cors",
-            "sec-fetch-site": "same-origin",
-            "viewport-width": "1475",
-            "x-asbd-id": "198387",
-            "x-csrftoken": self.csrf_token,
-            "x-ig-app-id": self.insta_app_id,
-            "x-ig-www-claim": self.x_ig_www_claim,
-            "x-instagram-ajax": "1007616494",
-            "x-requested-with": "XMLHttpRequest",
-            "Referer": f"https://www.instagram.com/{''.join(random.choices(string.ascii_lowercase, k=5))}/",
-            "Referrer-Policy": "strict-origin-when-cross-origin"
-        }
-
-        try:
-            http_response = self.request_session.post(f"https://www.instagram.com/api/v1/friendships/create/{identifier}/", headers=request_headers, data=body_json)
-            response_json = http_response.json()
-
-            if "status" in response_json:
-                if response_json["status"] == "ok" and "friendship_status" in response_json:
-                    if "following" in response_json["friendship_status"] \
-                            and "outgoing_request" in response_json["friendship_status"] \
-                            and "followed_by" in response_json["friendship_status"] \
-                            and "previous_following" in response_json:
-                        return FollowedStatus(
-                            following=response_json["friendship_status"]["following"],
-                            follow_requested=response_json["friendship_status"]["outgoing_request"],
-                            is_my_follower=response_json["friendship_status"]["followed_by"],
-                            previous_following=response_json["previous_following"]
-                        )
-        except JSONDecodeError:
-            return None
-
-    def unfollow(self, identifier: str | int) -> UnfollowedStatus | None:
-        conversion_success, identifier = self.identifier_conversion(identifier, UID)
-        if not conversion_success: return None
-
-        # Actual Request
-        refresh_csrf_token(self)
-        body_json = {
-            "container_module": "profile",
-            "nav_chain": f"PolarisProfileRoot:profilePage:1:via_cold_start",
-            "user_id": identifier
-        }
-        request_headers = {
-            "accept": "*/*",
-            "accept-language": "en-US,en;q=0.9",
-            "content-type": "application/x-www-form-urlencoded",
-            "sec-ch-prefers-color-scheme": self.preferred_color_scheme,
-            "sec-ch-ua": "\"Not.A/Brand\";v=\"8\", \"Chromium\";v=\"114\", \"Google Chrome\";v=\"114\"",
-            "sec-ch-ua-full-version-list": "\"Not.A/Brand\";v=\"8.0.0.0\", \"Chromium\";v=\"114.0.5735.91\", \"Google Chrome\";v=\"114.0.5735.91\"",
-            "sec-ch-ua-mobile": "?0",
-            "sec-ch-ua-platform": "\"Windows\"",
-            "sec-ch-ua-platform-version": "\"15.0.0\"",
-            "sec-fetch-dest": "empty",
-            "sec-fetch-mode": "cors",
-            "sec-fetch-site": "same-origin",
-            "viewport-width": "1475",
-            "x-asbd-id": "198387",
-            "x-csrftoken": self.csrf_token,
-            "x-ig-app-id": self.insta_app_id,
-            "x-ig-www-claim": self.x_ig_www_claim,
-            "x-instagram-ajax": "1007616494",
-            "x-requested-with": "XMLHttpRequest",
-            "Referer": f"https://www.instagram.com/{''.join(random.choices(string.ascii_lowercase, k=6))}/",
-            "Referrer-Policy": "strict-origin-when-cross-origin"
-        }
-
-        try:
-            http_response = self.request_session.post(f"https://www.instagram.com/api/v1/friendships/destroy/{identifier}/", headers=request_headers, data=body_json)
-            response_json = http_response.json()
-
-            if "status" in response_json:
-                if response_json["status"] == "ok" and "friendship_status" in response_json:
-                    if "following" in response_json["friendship_status"] \
-                            and "outgoing_request" in response_json["friendship_status"] \
-                            and "followed_by" in response_json["friendship_status"]:
-                        return UnfollowedStatus(
-                            unfollowed=not response_json["friendship_status"]["following"] and not response_json["friendship_status"]["outgoing_request"],
-                            is_my_follower=response_json["friendship_status"]["followed_by"]
-                        )
-        except JSONDecodeError:
+    def followers(self, identifier: str | int, count: int = 0) -> Generator[FollowPerson, None, None]:
+        conversion_success, identifier = self._identifier(identifier, UID)
+        if not conversion_success:
+            yield None
             return None
 
-    def follower_list(self, identifier: str | int, count: int = 0) -> list[FollowPerson] | None:
-        conversion_success, identifier = self.identifier_conversion(identifier, UID)
-        if not conversion_success: return None
-
         # Actual Request
         refresh_csrf_token(self)
         request_headers = {
             "accept": "*/*",
             "accept-language": "en-US,en;q=0.9",
             "sec-ch-prefers-color-scheme": self.preferred_color_scheme,
             "sec-ch-ua": "\"Not.A/Brand\";v=\"8\", \"Chromium\";v=\"114\", \"Google Chrome\";v=\"114\"",
@@ -216,15 +113,15 @@
             "x-ig-www-claim": self.x_ig_www_claim,
             "x-requested-with": "XMLHttpRequest",
             "Referer": f"https://www.instagram.com/{''.join(random.choices(string.ascii_lowercase, k=6))}/followers/",
             "Referrer-Policy": "strict-origin-when-cross-origin"
         }
 
         current_max_id = ""
-        generated_list = []
+        generated_count = 0
 
         while True:
             current_max_id_text = ""
 
             if current_max_id != "":
                 current_max_id_text = f"&max_id={current_max_id}"
 
@@ -234,21 +131,23 @@
                 if count < 35:
                     count_text = count
 
                 http_response = self.request_session.get(f"https://www.instagram.com/api/v1/friendships/{identifier}/followers/?count={str(count_text)}{current_max_id_text}&search_surface=follow_list_page", headers=request_headers)
                 response_json = http_response.json()
 
                 if "status" not in response_json or "users" not in response_json:
+                    yield None
                     return None
 
                 if response_json["status"] != "ok":
+                    yield None
                     return None
 
                 for each_item in response_json["users"]:
-                    if len(generated_list) < count or count == 0:
+                    if generated_count < count or count == 0:
 
                         prop_has_anonymous_profile_picture = None
                         prop_user_id = None
                         prop_username = None
                         prop_full_name = None
                         prop_is_private = None
                         prop_is_verified = None
@@ -275,35 +174,40 @@
 
                         if "profile_pic_url" in each_item:
                             prop_profile_picture_url = each_item["profile_pic_url"]
 
                         if "is_possible_scammer" in each_item:
                             prop_is_possible_scammer = each_item["is_possible_scammer"]
 
-                        generated_list.append(FollowPerson(
+                        yield FollowPerson(
                             has_anonymous_profile_picture=prop_has_anonymous_profile_picture,
                             user_id=prop_user_id,
                             username=prop_username,
                             full_name=prop_full_name,
                             is_private=prop_is_private,
                             is_verified=prop_is_verified,
                             profile_picture_url=prop_profile_picture_url,
                             is_possible_scammer=prop_is_possible_scammer
-                        ))
+                        )
 
-                if (len(generated_list) < count or count == 0) and "next_max_id" in response_json:
+                        generated_count += 1
+
+                if (generated_count < count or count == 0) and "next_max_id" in response_json:
                     current_max_id = response_json["next_max_id"]
                 else:
-                    return generated_list
+                    return None
             except JSONDecodeError:
+                yield None
                 return None
 
-    def following_list(self, identifier: str | int, count: int = 0) -> list[FollowPerson] | None:
-        conversion_success, identifier = self.identifier_conversion(identifier, UID)
-        if not conversion_success: return None
+    def followings(self, identifier: str | int, count: int = 0) -> Generator[FollowPerson, None, None]:
+        conversion_success, identifier = self._identifier(identifier, UID)
+        if not conversion_success:
+            yield None
+            return None
 
         # Actual Request
         refresh_csrf_token(self)
         request_headers = {
             "accept": "*/*",
             "accept-language": "en-US,en;q=0.9",
             "sec-ch-prefers-color-scheme": self.preferred_color_scheme,
@@ -322,48 +226,52 @@
             "x-ig-www-claim": self.x_ig_www_claim,
             "x-requested-with": "XMLHttpRequest",
             "Referer": f"https://www.instagram.com/{''.join(random.choices(string.ascii_lowercase, k=6))}/following/",
             "Referrer-Policy": "strict-origin-when-cross-origin"
         }
 
         current_max_id = ""
-        generated_list = []
+        generated_count = 0
 
         while True:
             current_max_id_text = ""
 
             if current_max_id != "":
                 current_max_id_text = f"&max_id={current_max_id}"
 
             try:
                 count_text = 35
 
                 if count < 35:
                     count_text = count
 
-                http_response = self.request_session.get(f"https://www.instagram.com/api/v1/friendships/{identifier}/following/?count={str(count_text)}{current_max_id_text}", headers=request_headers)
+                http_response = self.request_session.get(
+                    f"https://www.instagram.com/api/v1/friendships/{identifier}/following/?count={str(count_text)}{current_max_id_text}",
+                    headers=request_headers)
                 response_json = http_response.json()
 
                 if "status" not in response_json or "users" not in response_json:
+                    yield None
                     return None
 
                 if response_json["status"] != "ok":
+                    yield None
                     return None
 
                 for each_item in response_json["users"]:
-                    if len(generated_list) < count or count == 0:
+                    if generated_count < count or count == 0:
 
-                        prop_has_anonymous_profile_picture = False
-                        prop_user_id = ""
-                        prop_username = ""
-                        prop_full_name = ""
-                        prop_is_private = False
-                        prop_is_verified = False
-                        prop_profile_picture_url = ""
-                        prop_is_possible_scammer = False
+                        prop_has_anonymous_profile_picture = None
+                        prop_user_id = None
+                        prop_username = None
+                        prop_full_name = None
+                        prop_is_private = None
+                        prop_is_verified = None
+                        prop_profile_picture_url = None
+                        prop_is_possible_scammer = None
 
                         if "has_anonymous_profile_picture" in each_item:
                             prop_has_anonymous_profile_picture = each_item["has_anonymous_profile_picture"]
 
                         if "pk" in each_item:
                             prop_user_id = each_item["pk"]
 
@@ -381,33 +289,36 @@
 
                         if "profile_pic_url" in each_item:
                             prop_profile_picture_url = each_item["profile_pic_url"]
 
                         if "is_possible_scammer" in each_item:
                             prop_is_possible_scammer = each_item["is_possible_scammer"]
 
-                        generated_list.append(FollowPerson(
+                        yield FollowPerson(
                             has_anonymous_profile_picture=prop_has_anonymous_profile_picture,
                             user_id=prop_user_id,
                             username=prop_username,
                             full_name=prop_full_name,
                             is_private=prop_is_private,
                             is_verified=prop_is_verified,
                             profile_picture_url=prop_profile_picture_url,
                             is_possible_scammer=prop_is_possible_scammer
-                        ))
+                        )
 
-                if (len(generated_list) < count or count == 0) and "next_max_id" in response_json:
+                        generated_count += 1
+
+                if (generated_count < count or count == 0) and "next_max_id" in response_json:
                     current_max_id = response_json["next_max_id"]
                 else:
-                    return generated_list
+                    return None
             except JSONDecodeError:
+                yield None
                 return None
 
-    def identifier_conversion(self, identifier: str | int, required: str | int):
+    def _identifier(self, identifier: str | int, required: str | int):
         identifier = format_identifier(identifier)
 
         if len(identifier) <= 0:
             raise IdentifierError("No identifier was given. Please pass either UserId or Username as an argument.")
 
         # Identifier: Username or UID?
         is_username = False
```

### Comparing `ensta-1.4/ensta/containers/Profile.py` & `ensta-1.5/ensta/containers/Profile.py`

 * *Files identical despite different names*

### Comparing `ensta-1.4/ensta/lib/Commons.py` & `ensta-1.5/ensta/lib/Commons.py`

 * *Files identical despite different names*

### Comparing `ensta-1.4/ensta/lib/Exceptions.py` & `ensta-1.5/ensta/lib/Exceptions.py`

 * *Files 19% similar despite different names*

```diff
@@ -15,8 +15,8 @@
     def __init__(self, message):
         super().__init__(message)
 
 
 class CodeError(Exception):
 
     def __init__(self, location: str = "Unknown"):
-        super().__init__(f"There was some problem when executing this method. This was caused due to a bug in the code. Please contact the developer of submit this as an issue.\nFound in: {location}")
+        super().__init__(f"There was an error while executing this function, maybe caused due to a bug in the code. Please submit this as an issue on GitHub.\nFound in: {location}")
```

### Comparing `ensta-1.4/setup.py` & `ensta-1.5/setup.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,28 +1,28 @@
 from distutils.core import setup
 from pathlib import Path
 
-long_description = (Path(__file__).parent / "README.md").read_text()
+long_description = (Path(__file__).parent / "README.md").read_text(encoding="utf-8")
 
 setup(
     name="ensta",
     packages=["ensta", "ensta.lib", "ensta.containers"],
-    version="1.4",
+    version="1.5",
     license="MIT",
     description="Simple & Up-to-date Instagram API",
     long_description=long_description,
     long_description_content_type="text/markdown",
     author="Deepak Soni",
     author_email="lonelycube@proton.me",
     url="https://github.com/diezo/ensta",
-    download_url="https://github.com/diezo/ensta/archive/refs/tags/v1.4.tar.gz",
+    download_url="https://github.com/diezo/ensta/archive/refs/tags/v1.5.tar.gz",
     keywords=["instagram", "web", "private", "api", "scraper", "easy", "download", "upload"],
     install_requires=["requests"],
     classifiers=[
-        "Development Status :: 4 - Beta",
+        "Development Status :: 5 - Production/Stable",
         "Intended Audience :: Developers",
         "Topic :: Software Development :: Build Tools",
         "License :: OSI Approved :: MIT License",
         "Programming Language :: Python :: 3",
         "Programming Language :: Python :: 3.10"
     ]
 )
```

