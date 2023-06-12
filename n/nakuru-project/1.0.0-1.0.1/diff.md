# Comparing `tmp/nakuru_project-1.0.0.tar.gz` & `tmp/nakuru_project-1.0.1.tar.gz`

## Comparing `nakuru_project-1.0.0.tar` & `nakuru_project-1.0.1.tar`

### file list

```diff
@@ -1,28 +1,28 @@
--rw-r--r--   0        0        0   280258 2020-02-02 00:00:00.000000 nakuru_project-1.0.0/logo.png
--rw-r--r--   0        0        0      523 2020-02-02 00:00:00.000000 nakuru_project-1.0.0/setup.py
--rw-r--r--   0        0        0     1084 2020-02-02 00:00:00.000000 nakuru_project-1.0.0/.github/workflows/python-publish.yml
--rw-r--r--   0        0        0       59 2020-02-02 00:00:00.000000 nakuru_project-1.0.0/nakuru/__init__.py
--rw-r--r--   0        0        0    13700 2020-02-02 00:00:00.000000 nakuru_project-1.0.0/nakuru/application.py
--rw-r--r--   0        0        0       52 2020-02-02 00:00:00.000000 nakuru_project-1.0.0/nakuru/logger.py
--rw-r--r--   0        0        0     3826 2020-02-02 00:00:00.000000 nakuru_project-1.0.0/nakuru/misc.py
--rw-r--r--   0        0        0     1404 2020-02-02 00:00:00.000000 nakuru_project-1.0.0/nakuru/network.py
--rw-r--r--   0        0        0    28618 2020-02-02 00:00:00.000000 nakuru_project-1.0.0/nakuru/protocol.py
--rw-r--r--   0        0        0      127 2020-02-02 00:00:00.000000 nakuru_project-1.0.0/nakuru/entities/__init__.py
--rw-r--r--   0        0        0    10705 2020-02-02 00:00:00.000000 nakuru_project-1.0.0/nakuru/entities/components.py
--rw-r--r--   0        0        0      114 2020-02-02 00:00:00.000000 nakuru_project-1.0.0/nakuru/entities/device.py
--rw-r--r--   0        0        0      868 2020-02-02 00:00:00.000000 nakuru_project-1.0.0/nakuru/entities/file.py
--rw-r--r--   0        0        0      188 2020-02-02 00:00:00.000000 nakuru_project-1.0.0/nakuru/entities/friend.py
--rw-r--r--   0        0        0     1430 2020-02-02 00:00:00.000000 nakuru_project-1.0.0/nakuru/entities/group.py
--rw-r--r--   0        0        0     2315 2020-02-02 00:00:00.000000 nakuru_project-1.0.0/nakuru/entities/guild.py
--rw-r--r--   0        0        0     2142 2020-02-02 00:00:00.000000 nakuru_project-1.0.0/nakuru/entities/others.py
--rw-r--r--   0        0        0      221 2020-02-02 00:00:00.000000 nakuru_project-1.0.0/nakuru/event/__init__.py
--rw-r--r--   0        0        0      592 2020-02-02 00:00:00.000000 nakuru_project-1.0.0/nakuru/event/builtins.py
--rw-r--r--   0        0        0     1802 2020-02-02 00:00:00.000000 nakuru_project-1.0.0/nakuru/event/enums.py
--rw-r--r--   0        0        0     7901 2020-02-02 00:00:00.000000 nakuru_project-1.0.0/nakuru/event/models.py
--rw-r--r--   0        0        0     1802 2020-02-02 00:00:00.000000 nakuru_project-1.0.0/nakuru/examples/forward_message.py
--rw-r--r--   0        0        0    51695 2020-02-02 00:00:00.000000 nakuru_project-1.0.0/nakuru/examples/src/1.jpg
--rw-r--r--   0        0        0       27 2020-02-02 00:00:00.000000 nakuru_project-1.0.0/.gitignore
--rw-r--r--   0        0        0     1068 2020-02-02 00:00:00.000000 nakuru_project-1.0.0/LICENSE
--rw-r--r--   0        0        0     2071 2020-02-02 00:00:00.000000 nakuru_project-1.0.0/README.md
--rw-r--r--   0        0        0      750 2020-02-02 00:00:00.000000 nakuru_project-1.0.0/pyproject.toml
--rw-r--r--   0        0        0     2775 2020-02-02 00:00:00.000000 nakuru_project-1.0.0/PKG-INFO
+-rw-r--r--   0        0        0   280258 2020-02-02 00:00:00.000000 nakuru_project-1.0.1/logo.png
+-rw-r--r--   0        0        0      524 2020-02-02 00:00:00.000000 nakuru_project-1.0.1/setup.py
+-rw-r--r--   0        0        0     1084 2020-02-02 00:00:00.000000 nakuru_project-1.0.1/.github/workflows/python-publish.yml
+-rw-r--r--   0        0        0       59 2020-02-02 00:00:00.000000 nakuru_project-1.0.1/nakuru/__init__.py
+-rw-r--r--   0        0        0    13854 2020-02-02 00:00:00.000000 nakuru_project-1.0.1/nakuru/application.py
+-rw-r--r--   0        0        0       52 2020-02-02 00:00:00.000000 nakuru_project-1.0.1/nakuru/logger.py
+-rw-r--r--   0        0        0     3826 2020-02-02 00:00:00.000000 nakuru_project-1.0.1/nakuru/misc.py
+-rw-r--r--   0        0        0     1404 2020-02-02 00:00:00.000000 nakuru_project-1.0.1/nakuru/network.py
+-rw-r--r--   0        0        0    29284 2020-02-02 00:00:00.000000 nakuru_project-1.0.1/nakuru/protocol.py
+-rw-r--r--   0        0        0      127 2020-02-02 00:00:00.000000 nakuru_project-1.0.1/nakuru/entities/__init__.py
+-rw-r--r--   0        0        0    10705 2020-02-02 00:00:00.000000 nakuru_project-1.0.1/nakuru/entities/components.py
+-rw-r--r--   0        0        0      114 2020-02-02 00:00:00.000000 nakuru_project-1.0.1/nakuru/entities/device.py
+-rw-r--r--   0        0        0      868 2020-02-02 00:00:00.000000 nakuru_project-1.0.1/nakuru/entities/file.py
+-rw-r--r--   0        0        0      188 2020-02-02 00:00:00.000000 nakuru_project-1.0.1/nakuru/entities/friend.py
+-rw-r--r--   0        0        0     1430 2020-02-02 00:00:00.000000 nakuru_project-1.0.1/nakuru/entities/group.py
+-rw-r--r--   0        0        0     2315 2020-02-02 00:00:00.000000 nakuru_project-1.0.1/nakuru/entities/guild.py
+-rw-r--r--   0        0        0     2142 2020-02-02 00:00:00.000000 nakuru_project-1.0.1/nakuru/entities/others.py
+-rw-r--r--   0        0        0      221 2020-02-02 00:00:00.000000 nakuru_project-1.0.1/nakuru/event/__init__.py
+-rw-r--r--   0        0        0      592 2020-02-02 00:00:00.000000 nakuru_project-1.0.1/nakuru/event/builtins.py
+-rw-r--r--   0        0        0     1802 2020-02-02 00:00:00.000000 nakuru_project-1.0.1/nakuru/event/enums.py
+-rw-r--r--   0        0        0     7901 2020-02-02 00:00:00.000000 nakuru_project-1.0.1/nakuru/event/models.py
+-rw-r--r--   0        0        0     1802 2020-02-02 00:00:00.000000 nakuru_project-1.0.1/nakuru/examples/forward_message.py
+-rw-r--r--   0        0        0    51695 2020-02-02 00:00:00.000000 nakuru_project-1.0.1/nakuru/examples/src/1.jpg
+-rw-r--r--   0        0        0       27 2020-02-02 00:00:00.000000 nakuru_project-1.0.1/.gitignore
+-rw-r--r--   0        0        0     1068 2020-02-02 00:00:00.000000 nakuru_project-1.0.1/LICENSE
+-rw-r--r--   0        0        0     2031 2020-02-02 00:00:00.000000 nakuru_project-1.0.1/README.md
+-rw-r--r--   0        0        0      751 2020-02-02 00:00:00.000000 nakuru_project-1.0.1/pyproject.toml
+-rw-r--r--   0        0        0     2735 2020-02-02 00:00:00.000000 nakuru_project-1.0.1/PKG-INFO
```

### Comparing `nakuru_project-1.0.0/logo.png` & `nakuru_project-1.0.1/logo.png`

 * *Files identical despite different names*

### Comparing `nakuru_project-1.0.0/setup.py` & `nakuru_project-1.0.1/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,17 +1,17 @@
 from setuptools import setup, find_packages
 
 setup(
     name="nakuru-project",
-    version="1.0.0",
+    version="1.0.1",
     author="Lxns-Network",
     author_email="joinchang1206@gmail.com",
     description="一款为 go-cqhttp 的正向 WebSocket 设计的 Python SDK，支持纯 CQ 码与消息链的转换处理",
     url="https://github.com/Lxns-Network/nakuru-project",
     packages=find_packages(include=("nakuru", "nakuru.*")),
     install_requires=[
         "aiohttp",
         "pydantic",
         "Logbook",
         "async_lru"
     ]
-)
+)
```

### Comparing `nakuru_project-1.0.0/.github/workflows/python-publish.yml` & `nakuru_project-1.0.1/.github/workflows/python-publish.yml`

 * *Files identical despite different names*

### Comparing `nakuru_project-1.0.0/nakuru/application.py` & `nakuru_project-1.0.1/nakuru/application.py`

 * *Files 1% similar despite different names*

```diff
@@ -49,19 +49,26 @@
             self.headers["Authorization"] = f"Bearer {token}"
             self.protocol_params = {
                 "access_token": token
             }
         self.baseurl = f"http://{host}:{port}"
         self.baseurl_http = f"http://{host}:{http_port}"
 
+        self.closed = False
+
+    def close(self):
+        self.closed = True
+
     async def ws_event(self):
         async with aiohttp.ClientSession() as session:
             async with session.ws_connect(f"{self.baseurl}", headers=self.headers) as ws_connection:
                 logger.info("Protocol: connected")
                 while True:
+                    if self.closed:
+                        break
                     try:
                         received_data = await ws_connection.receive_json()
                     except TypeError:
                         continue
                     if received_data:
                         post_type = received_data["post_type"]
                         try:
@@ -70,18 +77,18 @@
                             elif post_type == "notice":
                                 received_data = NoticeTypes[received_data["notice_type"]].parse_obj(received_data)
                             elif post_type == "request":
                                 received_data = RequestTypes[received_data["request_type"]].parse_obj(received_data)
                             else:
                                 continue
                         except KeyError:
-                            logger.error("Protocol: data parse error: " + received_data)
+                            logger.error("Protocol: data parse error: " + str(received_data))
                             continue
                         except pydantic.error_wrappers.ValidationError:
-                            logger.error("Protocol: data parse error: " + received_data)
+                            logger.error("Protocol: data parse error: " + str(received_data))
                             continue
                         await self.queue.put(InternalEvent(
                             name=self.getEventCurrentName(type(received_data)),
                             body=received_data
                         ))
 
     async def event_runner(self):
```

### Comparing `nakuru_project-1.0.0/nakuru/misc.py` & `nakuru_project-1.0.1/nakuru/misc.py`

 * *Files identical despite different names*

### Comparing `nakuru_project-1.0.0/nakuru/network.py` & `nakuru_project-1.0.1/nakuru/network.py`

 * *Files identical despite different names*

### Comparing `nakuru_project-1.0.0/nakuru/protocol.py` & `nakuru_project-1.0.1/nakuru/protocol.py`

 * *Files 1% similar despite different names*

```diff
@@ -59,14 +59,29 @@
         result = await fetch.http_post(f"{self.baseurl_http}/send_group_forward_msg", {
             "group_id": group_id,
             "messages": messages
         }, params=self.protocol_params)
         if result["status"] == "ok":
             return BotMessage.parse_obj(result["data"])
         return False
+    
+    async def sendPrivateForwardMessage(self,
+                                        user_id: int,
+                                        messages: list) -> T.Union[BotMessage, bool]:
+        for i in range(len(messages)):
+            if isinstance(messages[i], Node):
+                messages[i] = messages[i].toDict()
+
+        result = await fetch.http_post(f"{self.baseurl_http}/send_private_forward_msg", {
+            "user_id": user_id,
+            "messages": messages
+        }, params=self.protocol_params)
+        if result["status"] == "ok":
+            return BotMessage.parse_obj(result["data"])
+        return False
 
     async def recall(self, message_id: int) -> bool:
         result = await fetch.http_post(f"{self.baseurl_http}/delete_msg", {
             "message_id": message_id
         }, params=self.protocol_params)
         if result["status"] == "ok":
             return True
@@ -251,15 +266,15 @@
             "reason": reason
         }, params=self.protocol_params)
         if result["status"] == "ok":
             return True
         return False
 
     async def getLoginInfo(self) -> T.Union[Bot, bool]:
-        result = await fetch.http_post(f"{self.baseurl_http}/get_login_info")
+        result = await fetch.http_post(f"{self.baseurl_http}/get_login_info", params=self.protocol_params)
         if result["status"] == "ok":
             return Bot.parse_obj(result["data"])
         return False
 
     async def getQiDianAccountInfo(self) -> T.Union[QiDianAccount, bool]:
         result = await fetch.http_post(f"{self.baseurl_http}/qidian_get_account_info")
         if result["status"] == "ok":
```

### Comparing `nakuru_project-1.0.0/nakuru/entities/components.py` & `nakuru_project-1.0.1/nakuru/entities/components.py`

 * *Files identical despite different names*

### Comparing `nakuru_project-1.0.0/nakuru/entities/file.py` & `nakuru_project-1.0.1/nakuru/entities/file.py`

 * *Files identical despite different names*

### Comparing `nakuru_project-1.0.0/nakuru/entities/group.py` & `nakuru_project-1.0.1/nakuru/entities/group.py`

 * *Files identical despite different names*

### Comparing `nakuru_project-1.0.0/nakuru/entities/guild.py` & `nakuru_project-1.0.1/nakuru/entities/guild.py`

 * *Files identical despite different names*

### Comparing `nakuru_project-1.0.0/nakuru/entities/others.py` & `nakuru_project-1.0.1/nakuru/entities/others.py`

 * *Files identical despite different names*

### Comparing `nakuru_project-1.0.0/nakuru/event/builtins.py` & `nakuru_project-1.0.1/nakuru/event/builtins.py`

 * *Files identical despite different names*

### Comparing `nakuru_project-1.0.0/nakuru/event/enums.py` & `nakuru_project-1.0.1/nakuru/event/enums.py`

 * *Files identical despite different names*

### Comparing `nakuru_project-1.0.0/nakuru/event/models.py` & `nakuru_project-1.0.1/nakuru/event/models.py`

 * *Files identical despite different names*

### Comparing `nakuru_project-1.0.0/nakuru/examples/forward_message.py` & `nakuru_project-1.0.1/nakuru/examples/forward_message.py`

 * *Files identical despite different names*

### Comparing `nakuru_project-1.0.0/nakuru/examples/src/1.jpg` & `nakuru_project-1.0.1/nakuru/examples/src/1.jpg`

 * *Files identical despite different names*

### Comparing `nakuru_project-1.0.0/LICENSE` & `nakuru_project-1.0.1/LICENSE`

 * *Files identical despite different names*

### Comparing `nakuru_project-1.0.0/README.md` & `nakuru_project-1.0.1/README.md`

 * *Files 6% similar despite different names*

```diff
@@ -6,15 +6,15 @@
 
 在 [kuriyama](https://github.com/Lxns-Network/mirai-python-sdk) 的基础上改动
 
 项目名来源于藍月なくる，图标由[せら](https://www.pixiv.net/users/577968)绘制
 </div>
 
 ## 食用方法
-使用 `pip install git+https://github.com/Lxns-Network/nakuru-project.git` 安装。
+使用 `pip install nakuru-project` 安装。
 
 需要将 go-cqhttp 的正向 WebSocket 与 HTTP 配置项开启。
 
 ## 示例
 没有文档，源码就是文档。
 
 ```python
```

### Comparing `nakuru_project-1.0.0/pyproject.toml` & `nakuru_project-1.0.1/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["hatchling"]
 build-backend = "hatchling.build"
 
 [project]
 name = "nakuru-project"
-version = "1.0.0"
+version = "1.0.1"
 authors = [
   { name="Lxns-Network", email="joinchang1206@gmail.com" },
 ]
 description = "一款为 go-cqhttp 的正向 WebSocket 设计的 Python SDK，支持纯 CQ 码与消息链的转换处理"
 readme = "README.md"
 requires-python = ">=3.7"
 classifiers = [
@@ -21,8 +21,8 @@
     "pydantic",
     "Logbook",
     "async_lru"
 ]
 
 [project.urls]
 "Homepage" = "https://github.com/Lxns-Network/nakuru-project"
-"Bug Tracker" = "https://github.com/Lxns-Network/nakuru-project/issues"
+"Bug Tracker" = "https://github.com/Lxns-Network/nakuru-project/issues"
```

### Comparing `nakuru_project-1.0.0/PKG-INFO` & `nakuru_project-1.0.1/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: nakuru-project
-Version: 1.0.0
+Version: 1.0.1
 Summary: 一款为 go-cqhttp 的正向 WebSocket 设计的 Python SDK，支持纯 CQ 码与消息链的转换处理
 Project-URL: Homepage, https://github.com/Lxns-Network/nakuru-project
 Project-URL: Bug Tracker, https://github.com/Lxns-Network/nakuru-project/issues
 Author-email: Lxns-Network <joinchang1206@gmail.com>
 License-File: LICENSE
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
@@ -24,15 +24,15 @@
 
 在 [kuriyama](https://github.com/Lxns-Network/mirai-python-sdk) 的基础上改动
 
 项目名来源于藍月なくる，图标由[せら](https://www.pixiv.net/users/577968)绘制
 </div>
 
 ## 食用方法
-使用 `pip install git+https://github.com/Lxns-Network/nakuru-project.git` 安装。
+使用 `pip install nakuru-project` 安装。
 
 需要将 go-cqhttp 的正向 WebSocket 与 HTTP 配置项开启。
 
 ## 示例
 没有文档，源码就是文档。
 
 ```python
```

