# Comparing `tmp/nonebot-plugin-twitter-0.1.6.tar.gz` & `tmp/nonebot-plugin-twitter-0.1.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "nonebot-plugin-twitter-0.1.6.tar", last modified: Mon Jun 12 04:59:44 2023, max compression
+gzip compressed data, was "nonebot-plugin-twitter-0.1.7.tar", last modified: Mon Jun 12 06:32:23 2023, max compression
```

## Comparing `nonebot-plugin-twitter-0.1.6.tar` & `nonebot-plugin-twitter-0.1.7.tar`

### file list

```diff
@@ -1,7 +1,7 @@
--rw-r--r--   0        0        0     1064 2023-06-12 04:59:36.655169 nonebot-plugin-twitter-0.1.6/LICENSE
--rw-r--r--   0        0        0     3053 2023-06-12 04:59:36.655169 nonebot-plugin-twitter-0.1.6/README.md
--rw-r--r--   0        0        0    14094 2023-06-12 04:59:36.655169 nonebot-plugin-twitter-0.1.6/nonebot_plugin_twitter/__init__.py
--rw-r--r--   0        0        0     4741 2023-06-12 04:59:36.655169 nonebot-plugin-twitter-0.1.6/nonebot_plugin_twitter/api.py
--rw-r--r--   0        0        0     1582 2023-06-12 04:59:36.655169 nonebot-plugin-twitter-0.1.6/nonebot_plugin_twitter/config.py
--rw-r--r--   0        0        0      654 2023-06-12 04:59:36.655169 nonebot-plugin-twitter-0.1.6/pyproject.toml
--rw-r--r--   0        0        0     3421 1970-01-01 00:00:00.000000 nonebot-plugin-twitter-0.1.6/PKG-INFO
+-rw-r--r--   0        0        0     1064 2023-06-12 06:32:12.568953 nonebot-plugin-twitter-0.1.7/LICENSE
+-rw-r--r--   0        0        0     3053 2023-06-12 06:32:12.568953 nonebot-plugin-twitter-0.1.7/README.md
+-rw-r--r--   0        0        0    14773 2023-06-12 06:32:12.568953 nonebot-plugin-twitter-0.1.7/nonebot_plugin_twitter/__init__.py
+-rw-r--r--   0        0        0     4741 2023-06-12 06:32:12.568953 nonebot-plugin-twitter-0.1.7/nonebot_plugin_twitter/api.py
+-rw-r--r--   0        0        0     1582 2023-06-12 06:32:12.568953 nonebot-plugin-twitter-0.1.7/nonebot_plugin_twitter/config.py
+-rw-r--r--   0        0        0      654 2023-06-12 06:32:12.568953 nonebot-plugin-twitter-0.1.7/pyproject.toml
+-rw-r--r--   0        0        0     3421 1970-01-01 00:00:00.000000 nonebot-plugin-twitter-0.1.7/PKG-INFO
```

### Comparing `nonebot-plugin-twitter-0.1.6/LICENSE` & `nonebot-plugin-twitter-0.1.7/LICENSE`

 * *Files identical despite different names*

### Comparing `nonebot-plugin-twitter-0.1.6/README.md` & `nonebot-plugin-twitter-0.1.7/README.md`

 * *Files identical despite different names*

### Comparing `nonebot-plugin-twitter-0.1.6/nonebot_plugin_twitter/__init__.py` & `nonebot-plugin-twitter-0.1.7/nonebot_plugin_twitter/__init__.py`

 * *Files 13% similar despite different names*

```diff
@@ -313,20 +313,31 @@
     
 twitter_status = on_command("推文推送",block=True,rule=is_rule,priority=config_dev.command_priority)
 @twitter_status.handle()
 async def twitter_status_handle(bot:Bot,event: MessageEvent,matcher: Matcher,arg: Message = CommandArg()):
     twitter_list = json.loads(dirpath.read_text("utf8"))
     try:
         if isinstance(event,GroupMessageEvent):
-            if arg.extract_plain_text() == "开启":
-                for user_name in twitter_list:
-                    twitter_list[user_name]["group"][str(event.group_id)]["status"] = True
-            elif arg.extract_plain_text() == "关闭":
-                for user_name in twitter_list:
-                    twitter_list[user_name]["group"][str(event.group_id)]["status"] = False
+            for user_name in twitter_list:
+                if str(event.group_id) in twitter_list[user_name]["group"]:
+                    if arg.extract_plain_text() == "开启":
+                        twitter_list[user_name]["group"][str(event.group_id)]["status"] = True
+                    elif arg.extract_plain_text() == "关闭":
+                        twitter_list[user_name]["group"][str(event.group_id)]["status"] = False
+                    else:
+                        await matcher.finish("错误指令")
+        else:
+            for user_name in twitter_list:
+                if str(event.user_id) in twitter_list[user_name]["private"]:
+                    if arg.extract_plain_text() == "开启":
+                        twitter_list[user_name]["private"][str(event.user_id)]["status"] = True
+                    elif arg.extract_plain_text() == "关闭":
+                        twitter_list[user_name]["private"][str(event.user_id)]["status"] = False
+                    else:
+                        await matcher.finish("错误指令")
         dirpath.write_text(json.dumps(twitter_list))
         await matcher.finish(f"推送已{arg.extract_plain_text()}")
     except FinishedException:
         pass
-    except:
-        await matcher.finish("未关注任何推主")
+    except Exception as e:
+        await matcher.finish(f"异常:{e}")
```

### Comparing `nonebot-plugin-twitter-0.1.6/nonebot_plugin_twitter/api.py` & `nonebot-plugin-twitter-0.1.7/nonebot_plugin_twitter/api.py`

 * *Files identical despite different names*

### Comparing `nonebot-plugin-twitter-0.1.6/nonebot_plugin_twitter/config.py` & `nonebot-plugin-twitter-0.1.7/nonebot_plugin_twitter/config.py`

 * *Files identical despite different names*

### Comparing `nonebot-plugin-twitter-0.1.6/pyproject.toml` & `nonebot-plugin-twitter-0.1.7/pyproject.toml`

 * *Files 19% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [project]
 name = "nonebot-plugin-twitter"
-version = "0.1.6"
+version = "0.1.7"
 description = "NoneBot2 plugin for twitter"
 authors = [
     { name = "nek0us", email = "nekouss@gmail.com" },
 ]
 dependencies = [
     "nonebot2>=2.0.0",
     "nonebot-adapter-onebot>=2.1.3",
```

### Comparing `nonebot-plugin-twitter-0.1.6/PKG-INFO` & `nonebot-plugin-twitter-0.1.7/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: nonebot-plugin-twitter
-Version: 0.1.6
+Version: 0.1.7
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
-Metadata-Version: 2.1 Name: nonebot-plugin-twitter Version: 0.1.6 Summary:
+Metadata-Version: 2.1 Name: nonebot-plugin-twitter Version: 0.1.7 Summary:
 NoneBot2 plugin for twitter License: MIT Author-email: nek0us
 gmail.com> Requires-Python: >=3.8 Project-URL: Homepage, https://github.com/
 nek0us/nonebot-plugin-twitter Project-URL: Repository, https://github.com/
 nek0us/nonebot-plugin-twitter Description-Content-Type: text/markdown
                              [NoneBotPluginLogo]
                               [NoneBotPluginText]
  # nonebot-plugin-twitter _â¨ æ¨æè®¢éæ¨éæä»¶ â¨_ [license] [pypi]
```

