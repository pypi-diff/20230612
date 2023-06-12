# Comparing `tmp/nonebot-plugin-twitter-0.1.5.tar.gz` & `tmp/nonebot-plugin-twitter-0.1.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "nonebot-plugin-twitter-0.1.5.tar", last modified: Sun Jun 11 07:23:35 2023, max compression
+gzip compressed data, was "nonebot-plugin-twitter-0.1.6.tar", last modified: Mon Jun 12 04:59:44 2023, max compression
```

## Comparing `nonebot-plugin-twitter-0.1.5.tar` & `nonebot-plugin-twitter-0.1.6.tar`

### file list

```diff
@@ -1,7 +1,7 @@
--rw-r--r--   0        0        0     1064 2023-06-11 07:23:27.829079 nonebot-plugin-twitter-0.1.5/LICENSE
--rw-r--r--   0        0        0     3053 2023-06-11 07:23:27.829079 nonebot-plugin-twitter-0.1.5/README.md
--rw-r--r--   0        0        0    14094 2023-06-11 07:23:27.829079 nonebot-plugin-twitter-0.1.5/nonebot_plugin_twitter/__init__.py
--rw-r--r--   0        0        0     4685 2023-06-11 07:23:27.829079 nonebot-plugin-twitter-0.1.5/nonebot_plugin_twitter/api.py
--rw-r--r--   0        0        0     1582 2023-06-11 07:23:27.829079 nonebot-plugin-twitter-0.1.5/nonebot_plugin_twitter/config.py
--rw-r--r--   0        0        0      654 2023-06-11 07:23:27.833079 nonebot-plugin-twitter-0.1.5/pyproject.toml
--rw-r--r--   0        0        0     3421 1970-01-01 00:00:00.000000 nonebot-plugin-twitter-0.1.5/PKG-INFO
+-rw-r--r--   0        0        0     1064 2023-06-12 04:59:36.655169 nonebot-plugin-twitter-0.1.6/LICENSE
+-rw-r--r--   0        0        0     3053 2023-06-12 04:59:36.655169 nonebot-plugin-twitter-0.1.6/README.md
+-rw-r--r--   0        0        0    14094 2023-06-12 04:59:36.655169 nonebot-plugin-twitter-0.1.6/nonebot_plugin_twitter/__init__.py
+-rw-r--r--   0        0        0     4741 2023-06-12 04:59:36.655169 nonebot-plugin-twitter-0.1.6/nonebot_plugin_twitter/api.py
+-rw-r--r--   0        0        0     1582 2023-06-12 04:59:36.655169 nonebot-plugin-twitter-0.1.6/nonebot_plugin_twitter/config.py
+-rw-r--r--   0        0        0      654 2023-06-12 04:59:36.655169 nonebot-plugin-twitter-0.1.6/pyproject.toml
+-rw-r--r--   0        0        0     3421 1970-01-01 00:00:00.000000 nonebot-plugin-twitter-0.1.6/PKG-INFO
```

### Comparing `nonebot-plugin-twitter-0.1.5/LICENSE` & `nonebot-plugin-twitter-0.1.6/LICENSE`

 * *Files identical despite different names*

### Comparing `nonebot-plugin-twitter-0.1.5/README.md` & `nonebot-plugin-twitter-0.1.6/README.md`

 * *Files identical despite different names*

### Comparing `nonebot-plugin-twitter-0.1.5/nonebot_plugin_twitter/__init__.py` & `nonebot-plugin-twitter-0.1.6/nonebot_plugin_twitter/__init__.py`

 * *Files identical despite different names*

### Comparing `nonebot-plugin-twitter-0.1.5/nonebot_plugin_twitter/api.py` & `nonebot-plugin-twitter-0.1.6/nonebot_plugin_twitter/api.py`

 * *Files 2% similar despite different names*

```diff
@@ -16,15 +16,15 @@
     async with httpx.AsyncClient(proxies=config_dev.twitter_proxy) as client:
         res = await client.get(url=f"{config_dev.twitter_url}/{user_name}")
         result ={}
         if res.status_code ==200:
             result["status"] = True
             result["user_name"] = user_name
             soup = BeautifulSoup(res.text,"html.parser")
-            result["screen_name"] = soup.find_all('a', class_='profile-card-fullname')[0].next
+            result["screen_name"] = match[0].text if (match := soup.find_all('a', class_='profile-card-fullname')) else ""
             result["bio"] = match[0].text if (match := soup.find_all('p')) else ""
         else:
             result["status"] = False
 
     return result
 
 async def get_user_newtimeline(user_name:str,since_id: str = "0") -> str:
@@ -69,15 +69,15 @@
     async with httpx.AsyncClient(proxies=config_dev.twitter_proxy) as client:
         res = await client.get(url=f"{config_dev.twitter_url}/{user_name}/status/{tweet_id}",cookies={"hlsPlayback": "on"})
         result = {}
         if res.status_code ==200:
             result["status"] = True
             soup = BeautifulSoup(res.text,"html.parser")
             # text
-            result["text"] = soup.find_all('div', class_='tweet-content media-body')[0].text
+            result["text"] = match[0].text if (match := soup.find_all('div', class_='tweet-content media-body')) else ""
             # pic
             if pic_list := soup.find_all('a', class_='still-image'):
                 result["pic_url_list"] = [x.attrs["href"] for x in pic_list]
             else:
                 result["pic_url_list"] = []
             # video
             if video_list := soup.find_all('video'):
```

### Comparing `nonebot-plugin-twitter-0.1.5/nonebot_plugin_twitter/config.py` & `nonebot-plugin-twitter-0.1.6/nonebot_plugin_twitter/config.py`

 * *Files identical despite different names*

### Comparing `nonebot-plugin-twitter-0.1.5/pyproject.toml` & `nonebot-plugin-twitter-0.1.6/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [project]
 name = "nonebot-plugin-twitter"
-version = "0.1.5"
+version = "0.1.6"
 description = "NoneBot2 plugin for twitter"
 authors = [
     { name = "nek0us", email = "nekouss@gmail.com" },
 ]
 dependencies = [
     "nonebot2>=2.0.0",
     "nonebot-adapter-onebot>=2.1.3",
```

### Comparing `nonebot-plugin-twitter-0.1.5/PKG-INFO` & `nonebot-plugin-twitter-0.1.6/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: nonebot-plugin-twitter
-Version: 0.1.5
+Version: 0.1.6
 Summary: NoneBot2 plugin for twitter
 License: MIT
 Author-email: nek0us <nekouss@gmail.com>
 Requires-Python: >=3.8
 Project-URL: Homepage, https://github.com/nek0us/nonebot-plugin-twitter
 Project-URL: Repository, https://github.com/nek0us/nonebot-plugin-twitter
 Description-Content-Type: text/markdown
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: nonebot-plugin-twitter Version: 0.1.5 Summary:
+Metadata-Version: 2.1 Name: nonebot-plugin-twitter Version: 0.1.6 Summary:
 NoneBot2 plugin for twitter License: MIT Author-email: nek0us
 gmail.com> Requires-Python: >=3.8 Project-URL: Homepage, https://github.com/
 nek0us/nonebot-plugin-twitter Project-URL: Repository, https://github.com/
 nek0us/nonebot-plugin-twitter Description-Content-Type: text/markdown
                              [NoneBotPluginLogo]
                               [NoneBotPluginText]
  # nonebot-plugin-twitter _â¨ æ¨æè®¢éæ¨éæä»¶ â¨_ [license] [pypi]
```

