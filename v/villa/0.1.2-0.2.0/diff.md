# Comparing `tmp/villa-0.1.2.tar.gz` & `tmp/villa-0.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "villa-0.1.2.tar", max compression
+gzip compressed data, was "villa-0.2.0.tar", max compression
```

## Comparing `villa-0.1.2.tar` & `villa-0.2.0.tar`

### file list

```diff
@@ -1,14 +1,14 @@
--rw-r--r--   0        0        0     1062 2023-06-09 04:26:48.597982 villa-0.1.2/LICENSE
--rw-r--r--   0        0        0     2399 2023-06-09 04:26:48.597982 villa-0.1.2/README.md
--rw-r--r--   0        0        0     1034 2023-06-09 04:26:48.597982 villa-0.1.2/pyproject.toml
--rw-r--r--   0        0        0      120 2023-06-09 04:26:48.597982 villa-0.1.2/villa/__init__.py
--rw-r--r--   0        0        0    30542 2023-06-09 04:26:48.597982 villa-0.1.2/villa/bot.py
--rw-r--r--   0        0        0     7799 2023-06-09 04:26:48.597982 villa-0.1.2/villa/event.py
--rw-r--r--   0        0        0      473 2023-06-09 04:26:48.601982 villa-0.1.2/villa/exception.py
--rw-r--r--   0        0        0     1504 2023-06-09 04:26:48.601982 villa-0.1.2/villa/log.py
--rw-r--r--   0        0        0    16613 2023-06-09 04:26:48.601982 villa-0.1.2/villa/message.py
--rw-r--r--   0        0        0     9982 2023-06-09 04:26:48.601982 villa-0.1.2/villa/models.py
--rw-r--r--   0        0        0      113 2023-06-09 04:26:48.601982 villa-0.1.2/villa/store.py
--rw-r--r--   0        0        0      794 2023-06-09 04:26:48.601982 villa-0.1.2/villa/typing.py
--rw-r--r--   0        0        0      995 2023-06-09 04:26:48.601982 villa-0.1.2/villa/utils.py
--rw-r--r--   0        0        0     3351 1970-01-01 00:00:00.000000 villa-0.1.2/PKG-INFO
+-rw-r--r--   0        0        0     1062 2023-06-12 15:23:36.018385 villa-0.2.0/LICENSE
+-rw-r--r--   0        0        0     2844 2023-06-12 15:23:36.018385 villa-0.2.0/README.md
+-rw-r--r--   0        0        0     1034 2023-06-12 15:23:36.018385 villa-0.2.0/pyproject.toml
+-rw-r--r--   0        0        0      285 2023-06-12 15:23:36.018385 villa-0.2.0/villa/__init__.py
+-rw-r--r--   0        0        0    38490 2023-06-12 15:23:36.018385 villa-0.2.0/villa/bot.py
+-rw-r--r--   0        0        0     8160 2023-06-12 15:23:36.018385 villa-0.2.0/villa/event.py
+-rw-r--r--   0        0        0      473 2023-06-12 15:23:36.022385 villa-0.2.0/villa/exception.py
+-rw-r--r--   0        0        0     1504 2023-06-12 15:23:36.022385 villa-0.2.0/villa/log.py
+-rw-r--r--   0        0        0    16316 2023-06-12 15:23:36.022385 villa-0.2.0/villa/message.py
+-rw-r--r--   0        0        0     9982 2023-06-12 15:23:36.022385 villa-0.2.0/villa/models.py
+-rw-r--r--   0        0        0      935 2023-06-12 15:23:36.022385 villa-0.2.0/villa/store.py
+-rw-r--r--   0        0        0      822 2023-06-12 15:23:36.022385 villa-0.2.0/villa/typing.py
+-rw-r--r--   0        0        0      995 2023-06-12 15:23:36.022385 villa-0.2.0/villa/utils.py
+-rw-r--r--   0        0        0     3796 1970-01-01 00:00:00.000000 villa-0.2.0/PKG-INFO
```

### Comparing `villa-0.1.2/LICENSE` & `villa-0.2.0/LICENSE`

 * *Files identical despite different names*

### Comparing `villa-0.1.2/README.md` & `villa-0.2.0/README.md`

 * *Files 16% similar despite different names*

```diff
@@ -1,16 +1,24 @@
 <div align="center">
 
 # Villa
 
 _✨ 米游社大别野Bot Python SDK ✨_
 
-<img src="https://img.shields.io/pypi/v/villa-py" alt="version">
+<a href="https://cdn.jsdelivr.net/gh/CMHopeSunshine/villa-py@master/LICENSE">
+    <img src="https://img.shields.io/github/license/CMHopeSunshine/villa-py" alt="license">
+</a>
+<img src="https://img.shields.io/pypi/v/villa" alt="version">
 <img src="https://img.shields.io/badge/Python-3.8+-yellow" alt="python">
-<a href="https://cdn.jsdelivr.net/gh/CMHopeSunshine/villa-py@master/LICENSE"><img src="https://img.shields.io/github/license/CMHopeSunshine/villa-py" alt="license"></a>
+<a href="https://pypi.python.org/pypi/villa">
+  <img src="https://img.shields.io/pypi/dm/villa" alt="pypi download">
+</a>
+<a href="https://wakatime.com/badge/user/eed3f89c-5d65-46e6-ab19-78dcc4b62b3f/project/d3b88a99-17c2-4c98-bbc2-c1949ce7c078">
+  <img src="https://wakatime.com/badge/user/eed3f89c-5d65-46e6-ab19-78dcc4b62b3f/project/d3b88a99-17c2-4c98-bbc2-c1949ce7c078.svg" alt="wakatime">
+</a>
 
 </div>
 
 ## 特性
 
 - 基于`FastAPI`和`Pydantic`，异步、快速、高性能！
 - 完整的类型注解支持
@@ -22,15 +30,15 @@
 
 - 使用pip: `pip install villa`
 - 使用poetry: `poetry add villa`
 - 使用pdm: `pdm add villa`
 
 ## 快速开始
 
-首先你需要一个[米游社大别野](https://dby.miyoushe.com/chat)的Bot，如果没有请先到机器人开发者社区(别野ID: OpenVilla)申请，取得`bot_id`、`bot_secret`
+首先你需要一个[米游社大别野](https://dby.miyoushe.com/chat)的Bot，如果没有请先到[机器人开发者社区](https://dby.miyoushe.com/chat/463/20020)(别野ID: OpenVilla)申请，取得`bot_id`、`bot_secret`
 
 ```python
 from villa import Bot
 from villa.event import SendMessageEvent
 
 bot = Bot(bot_id="your_bot_id", bot_secret="your_bot_secret", callback_url="your_callback_url")
 # 初始化Bot，填写你的bot_id、密钥以及回调地址
```

### Comparing `villa-0.1.2/pyproject.toml` & `villa-0.2.0/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "villa"
-version = "0.1.2"
+version = "0.2.0"
 description = "米游社大别野Bot Python SDK。MiHoYo Villa Bot Python SDK."
 authors = ["CMHopeSunshine <277073121@qq.com>"]
 license = "MIT"
 readme = "README.md"
 homepage = "https://github.com/CMHopeSunshine/villa-py"
 repository = "https://github.com/CMHopeSunshine/villa-py"
 documentation = "https://github.com/CMHopeSunshine/villa-py"
```

### Comparing `villa-0.1.2/villa/bot.py` & `villa-0.2.0/villa/bot.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,56 +1,109 @@
 import re
 import asyncio
 from itertools import product
 from typing import Any, Set, Dict, List, Type, Union, Literal, Optional
 
 import httpx
 import uvicorn
-from fastapi import FastAPI
 from pydantic import parse_obj_as
 from fastapi.responses import JSONResponse
 
 from .models import *
-from .store import _bots
 from .message import Message
 from .exception import ActionFailed
 from .message import MessageSegment
 from .log import logger, _log_patcher
 from .utils import run_sync, escape_tag
 from .message import Link as LinkSegment
 from .message import Text as TextSegment
 from .message import Image as ImageSegment
-from .typing import T_Handler, EventHandler
+from .store import get_app, get_bot, store_bot
 from .message import RoomLink as RoomLinkSegment
+from .typing import T_Func, T_Handler, EventHandler
 from .message import MentionAll as MentionAllSegment
 from .message import MentionUser as MentionUserSegment
 from .message import MentionRobot as MentionRobotSegment
 from .event import Event, SendMessageEvent, event_classes
 
 
 class Bot:
+    """Villa Bot"""
+
     _event_handlers: List[EventHandler] = []
+    _client: httpx.AsyncClient
+    bot_id: str
+    """机器人 Id"""
+    bot_secret: str
+    """机器人密钥"""
+    callback_url: str
+    """事件回调地址"""
+    bot_info: Optional[Robot] = None
+    """机器人信息"""
 
     def __init__(self, bot_id: str, bot_secret: str, callback_url: str):
+        """初始化一个 Bot 实例
+
+        参数:
+            bot_id: 机器人 ID
+            bot_secret: 机器人密钥
+            callback_url: 事件回调地址
+        """
         self.bot_id: str = bot_id
         self.bot_secret: str = bot_secret
         self.callback_url: str = callback_url
-        self.bot_info: Optional[Robot] = None
-        if bot_id in _bots:
-            raise ValueError(f"Bot {bot_id} already in bots")
-        _bots[bot_id] = self
+        self._client = httpx.AsyncClient(
+            base_url="https://bbs-api.miyoushe.com/vila/api/bot/platform/"
+        )
+        store_bot(self)
+
+    @property
+    def nickname(self) -> str:
+        """Bot 昵称"""
+        if self.bot_info is None:
+            raise ValueError(f"Bot {self.bot_id} not connected")
+        return self.bot_info.template.name
+
+    @property
+    def avatar_icon(self) -> str:
+        """Bot 头像地址"""
+        if self.bot_info is None:
+            raise ValueError(f"Bot {self.bot_id} not connected")
+        return self.bot_info.template.icon
+
+    @property
+    def commands(self) -> Optional[List[RobotCommand]]:
+        """Bot 预设命令列表"""
+        if self.bot_info is None:
+            raise ValueError(f"Bot {self.bot_id} not connected")
+        return self.bot_info.template.commands
+
+    @property
+    def description(self) -> str:
+        """Bot 介绍"""
+        if self.bot_info is None:
+            raise ValueError(f"Bot {self.bot_id} not connected")
+        return self.bot_info.template.desc
+
+    @property
+    def current_villa_id(self) -> str:
+        """Bot 最后收到的事件的大别野 ID"""
+        if self.bot_info is None:
+            raise ValueError(f"Bot {self.bot_id} not connected")
+        return self.bot_info.villa_id
 
     def on_event(
         self, *event_type: Type[Event], block: bool = False, priority: int = 1
     ):
         """注册一个事件处理函数
 
         当事件属于 event_type 中的任意一个时，执行处理函数。
 
         参数:
+            *event_type: 事件类型列表.
             block: 是否阻止更低优先级的处理函数执行. 默认为 False.
             priority: 优先级. 默认为 1.
         """
 
         def _decorator(func: T_Handler) -> T_Handler:
             self._event_handlers.append(
                 EventHandler(
@@ -203,14 +256,24 @@
             return func
 
         return _decorator
 
     async def send(
         self, villa_id: int, room_id: int, message: Union[str, Message, MessageSegment]
     ) -> str:
+        """发送消息
+
+        参数:
+            villa_id: 大别野 ID
+            room_id: 房间 ID
+            message: 消息内容
+
+        返回:
+            str: 消息 ID
+        """
         if isinstance(message, str):
             message = MessageSegment.text(message)
         if isinstance(message, MessageSegment):
             message = Message(message)
         content = await self._parse_message_content(message)
         return await self.send_message(
             villa_id=villa_id,
@@ -218,384 +281,635 @@
             object_name="MHY:Text",
             msg_content=content,
         )
 
     async def check_member_bot_access_token(
         self, token: str, villa_id: Optional[int] = None
     ) -> CheckMemberBotAccessTokenReturn:
+        """校验用户机器人访问凭证，并返回用户信息
+
+        参数:
+            token: 用户机器人访问凭证
+            villa_id: 大别野 ID. 默认为 None.
+
+        返回:
+            CheckMemberBotAccessTokenReturn: 用户信息
+        """
         return CheckMemberBotAccessTokenReturn.parse_obj(
             await self._request(
                 "GET",
-                "vila/api/bot/platform/checkMemberBotAccessToken",
+                "checkMemberBotAccessToken",
                 villa_id,
                 json={"token": token},
             )
         )
 
     async def get_villa(self, villa_id: int) -> Villa:
+        """获取大别野信息
+
+        参数:
+            villa_id: 大别野 ID
+
+        返回:
+            Villa: 大别野信息
+        """
         return Villa.parse_obj(
-            (
-                await self._request(
-                    "GET", "vila/api/bot/platform/getVilla", villa_id, json={}
-                )
-            )["villa"]
+            (await self._request("GET", "getVilla", villa_id, json={}))["villa"]
         )
 
     async def get_member(self, villa_id: int, uid: int) -> Member:
+        """获取用户信息
+
+        参数:
+            villa_id: 大别野
+            uid: 用户 ID
+
+        返回:
+            Member: 用户详情
+        """
         return Member.parse_obj(
             (
                 await self._request(
                     "GET",
-                    "vila/api/bot/platform/getMember",
+                    "getMember",
                     villa_id,
                     json={"uid": uid},
                 )
             )["member"]
         )
 
     async def get_villa_members(
         self, villa_id: int, offset: int, size: int
     ) -> MemberListReturn:
+        """获取大别野成员列表
+
+        参数:
+            villa_id: 大别野 ID
+            offset: 偏移量
+            size: 分页大小
+
+        返回:
+            MemberListReturn: 大别野成员列表信息
+        """
         return MemberListReturn.parse_obj(
             await self._request(
                 "GET",
-                "vila/api/bot/platform/getVillaMembers",
+                "getVillaMembers",
                 villa_id,
                 json={"offset": offset, "size": size},
             )
         )
 
     async def delete_villa_member(self, villa_id: int, uid: int) -> None:
+        """踢出大别野用户
+
+        参数:
+            villa_id: 大别野 ID
+            uid: 用户 ID
+        """
         await self._request(
             "POST",
-            "vila/api/bot/platform/deleteVillaMember",
+            "deleteVillaMember",
             villa_id,
             json={"uid": uid},
         )
 
     async def pin_message(
         self, villa_id: int, msg_uid: str, is_cancel: bool, room_id: int, send_at: int
     ) -> None:
+        """置顶消息
+
+        参数:
+            villa_id: 大别野 ID
+            msg_uid: 消息 ID
+            is_cancel: 是否取消置顶
+            room_id: 房间 ID
+            send_at: 消息发送时间
+        """
         await self._request(
             "POST",
-            "vila/api/bot/platform/pinMessage",
+            "pinMessage",
             villa_id,
             json={
                 "msg_uid": msg_uid,
                 "is_cancel": is_cancel,
                 "room_id": room_id,
                 "send_at": send_at,
             },
         )
 
     async def recall_message(
         self, villa_id: int, msg_uid: str, room_id: int, msg_time: int
     ) -> None:
+        """撤回消息
+
+        参数:
+            villa_id: 大别野 ID
+            msg_uid: 消息 ID
+            room_id: 房间 ID
+            msg_time: 消息发送时间
+        """
         await self._request(
             "POST",
-            "vila/api/bot/platform/recallMessage",
+            "recallMessage",
             villa_id,
             json={"msg_uid": msg_uid, "msg_time": msg_time, "room_id": room_id},
         )
 
     async def send_message(
         self,
         villa_id: int,
         room_id: int,
         object_name: str,
         msg_content: Union[str, MessageContentInfo],
     ) -> str:
+        """发送消息
+
+        参数:
+            villa_id: 大别野 ID
+            room_id: 房间 ID
+            object_name: 消息类型
+            msg_content: 将 MsgContentInfo 结构体序列化后的字符串
+
+        返回:
+            str: 消息 ID
+        """
         if isinstance(msg_content, MessageContentInfo):
             content = msg_content.json(by_alias=True, exclude_none=True)
         else:
             content = msg_content
         return (
             await self._request(
                 "POST",
-                "vila/api/bot/platform/sendMessage",
+                "sendMessage",
                 villa_id,
                 json={
                     "room_id": room_id,
                     "object_name": object_name,
                     "msg_content": content,
                 },
             )
         )["bot_msg_id"]
 
     async def create_group(self, villa_id: int, group_name: str) -> int:
+        """创建分组
+
+        参数:
+            villa_id: 大别野 ID
+            group_name: 分组名称
+
+        返回:
+            int: 分组 ID
+        """
         return (
             await self._request(
                 "POST",
-                "vila/api/bot/platform/createGroup",
+                "createGroup",
                 villa_id,
                 json={
                     "group_name": group_name,
                 },
             )
         )["group_id"]
 
     async def edit_group(self, villa_id: int, group_id: int, group_name: str) -> None:
+        """编辑分组
+
+        参数:
+            villa_id: 大别野 ID
+            group_id: 分组 ID
+            group_name: 分组名称
+        """
         await self._request(
             "POST",
-            "vila/api/bot/platform/editGroup",
+            "editGroup",
             villa_id,
             json={"group_id": group_id, "group_name": group_name},
         )
 
     async def delete_group(self, villa_id: int, group_id: int) -> None:
+        """删除分组
+
+        参数:
+            villa_id: 大别野 ID
+            group_id: 分组 ID
+        """
         await self._request(
             "POST",
-            "vila/api/bot/platform/deleteGroup",
+            "deleteGroup",
             villa_id,
             json={"group_id": group_id},
         )
 
     async def get_group_list(self, villa_id: int) -> List[Group]:
+        """获取分组列表
+
+        参数:
+            villa_id: 大别野 ID
+
+        返回:
+            List[Group]: 分组列表
+        """
         return parse_obj_as(
             List[Group],
-            (
-                await self._request(
-                    "GET", "vila/api/bot/platform/getGroupList", villa_id, json={}
-                )
-            )["list"],
+            (await self._request("GET", "getGroupList", villa_id, json={}))["list"],
         )
 
     async def sort_group_list(self, villa_id: int, group_ids: List[int]) -> None:
+        """分组列表排序
+
+        参数:
+            villa_id: 大别野 ID
+            group_ids: 分组 ID 排序
+        """
         await self._request(
             "POST",
-            "vila/api/bot/platform/sortGroupList",
+            "sortGroupList",
             villa_id,
             json={"villa_id": villa_id, "group_ids": group_ids},
         )
 
     async def create_room(
         self,
         villa_id: int,
         room_name: str,
         room_type: Union[Literal[1, 2, 3], CreateRoomType],
         group_id: int,
         room_default_notify_type: Union[Literal[1, 2], CreateRoomDefaultNotifyType],
         send_msg_auth_range: SendMsgAuthRange,
     ) -> Room:
+        """创建房间
+
+        参数:
+            villa_id: 大别野 ID
+            room_name: 房间名称
+            room_type: 房间类型
+            group_id: 分组 ID
+            room_default_notify_type: 房间默认通知类型
+            send_msg_auth_range: 房间消息发送权限范围设置
+
+        返回:
+            Room: 房间信息
+        """
         return Room.parse_obj(
             (
                 await self._request(
                     "POST",
-                    "vila/api/bot/platform/createRoom",
+                    "createRoom",
                     villa_id,
                     json={
                         "room_name": room_name,
                         "room_type": room_type,
                         "group_id": group_id,
                         "room_default_notify_type": room_default_notify_type,
                         "send_msg_auth_range": send_msg_auth_range.dict(),
                     },
                 )
             )["room"]
         )
 
     async def edit_room(self, villa_id: int, room_id: int, room_name: str) -> None:
+        """编辑房间
+
+        参数:
+            villa_id: 大别野 ID
+            room_id: 房间 ID
+            room_name: 房间名称
+        """
         await self._request(
             "POST",
-            "vila/api/bot/platform/editRoom",
+            "editRoom",
             villa_id,
             json={"room_id": room_id, "room_name": room_name},
         )
 
     async def delete_room(self, villa_id: int, room_id: int) -> None:
+        """删除房间
+
+        参数:
+            villa_id: 大别野 ID
+            room_id: 房间 ID
+        """
         await self._request(
             "POST",
-            "vila/api/bot/platform/deleteRoom",
+            "deleteRoom",
             villa_id,
             json={"room_id": room_id},
         )
 
     async def get_room(self, villa_id: int, room_id: int) -> Room:
+        """获取房间信息
+
+        参数:
+            villa_id: 大别野 ID
+            room_id: 房间 ID
+
+        返回:
+            Room: 房间详情
+        """
         return Room.parse_obj(
             (
                 await self._request(
                     "GET",
-                    "vila/api/bot/platform/getRoom",
+                    "getRoom",
                     villa_id,
                     json={"room_id": room_id},
                 )
             )["room"]
         )
 
     async def get_villa_group_room_list(self, villa_id: int) -> GroupRoom:
+        """获取房间列表信息
+
+        参数:
+            villa_id: 大别野 ID
+
+        返回:
+            GroupRoom: 房间列表
+        """
         return GroupRoom.parse_obj(
             (
                 await self._request(
                     "GET",
-                    "vila/api/bot/platform/getVillaGroupRoomList",
+                    "getVillaGroupRoomList",
                     villa_id,
                     json={},
                 )
             )["list"]
         )
 
     async def sort_room_list(self, villa_id: int, room_list: List[RoomSort]) -> None:
+        """房间列表排序
+
+        参数:
+            villa_id: 大别野 ID
+            room_list: 期望的排序列表
+        """
         await self._request(
             "POST",
-            "vila/api/bot/platform/sortRoomList",
+            "sortRoomList",
             villa_id,
             json={
                 "villa_id": villa_id,
                 "room_list": [room.dict() for room in room_list],
             },
         )
 
     async def operate_member_to_role(
         self, villa_id: int, role_id: int, uid: int, is_add: bool
     ) -> None:
+        """向身份组操作用户
+
+        参数:
+            villa_id: 大别野 ID
+            role_id: 身份组 ID
+            uid: 用户 ID
+            is_add: 是否添加用户
+        """
         await self._request(
             "POST",
-            "vila/api/bot/platform/operateMemberToRole",
+            "operateMemberToRole",
             villa_id,
             json={"role_id": role_id, "uid": uid, "is_add": is_add},
         )
 
     async def create_member_role(
         self, villa_id: int, name: str, color: Color, permissions: List[Permission]
     ) -> int:
+        """创建身份组
+
+        参数:
+            villa_id: 大别野 ID
+            name: 身份组名称
+            color: 身份组颜色
+            permissions: 权限列表
+
+        返回:
+            int: 身份组 ID
+        """
         return (
             await self._request(
                 "POST",
-                "vila/api/bot/platform/createMemberRole",
+                "createMemberRole",
                 villa_id,
                 json={"name": name, "color": str(color), "permissions": permissions},
             )
         )["id"]
 
     async def edit_member_role(
         self,
         villa_id: int,
         role_id: int,
         name: str,
         color: Color,
         permissions: List[Permission],
     ) -> None:
+        """编辑身份组
+
+        参数:
+            villa_id: 大别野 ID
+            role_id: 身份组 ID
+            name: 身份组名称
+            color: 身份组颜色
+            permissions: 权限列表
+        """
         await self._request(
             "POST",
-            "vila/api/bot/platform/editMemberRole",
+            "editMemberRole",
             villa_id,
             json={
                 "id": role_id,
                 "name": name,
                 "color": str(color),
                 "permissions": permissions,
             },
         )
 
     async def delete_member_role(self, villa_id: int, role_id: int) -> None:
+        """删除身份组
+
+        参数:
+            villa_id: 大别野 ID
+            role_id: 身份组 ID
+        """
         await self._request(
             "POST",
-            "vila/api/bot/platform/deleteMemberRole",
+            "deleteMemberRole",
             villa_id,
             json={"id": role_id},
         )
 
     async def get_member_role_info(
         self, villa_id: int, role_id: int
     ) -> MemberRoleDetail:
+        """获取身份组
+
+        参数:
+            villa_id: 大别野 ID
+            role_id: 身份组 ID
+
+        返回:
+            MemberRoleDetail: 身份组详情
+        """
         return MemberRoleDetail.parse_obj(
             (
                 await self._request(
                     "GET",
-                    "vila/api/bot/platform/getMemberRoleInfo",
+                    "getMemberRoleInfo",
                     villa_id,
                     json={"id": role_id},
                 )
             )["role"]
         )
 
     async def get_villa_member_roles(self, villa_id: int) -> List[MemberRoleDetail]:
+        """获取大别野下所有身份组
+
+        参数:
+            villa_id: 大别野 ID
+
+        返回:
+            List[MemberRoleDetail]: 身份组列表
+        """
         return parse_obj_as(
             List[MemberRoleDetail],
             (
                 await self._request(
                     "GET",
-                    "vila/api/bot/platform/getVillaMemberRoles",
+                    "getVillaMemberRoles",
                     villa_id,
                     json={},
                 )
             )["list"],
         )
 
-    async def get_all_emoticons(self, villa_id: int) -> List[Emoticon]:
+    async def get_all_emoticons(self) -> List[Emoticon]:
+        """获取全量表情
+
+        参数:
+            villa_id: 参数说明
+
+        返回:
+            List[Emoticon]: 表情列表
+        """
         return parse_obj_as(
             List[Emoticon],
             (
                 await self._request(
                     "GET",
-                    "vila/api/bot/platform/getAllEmoticons",
-                    villa_id,
+                    "getAllEmoticons",
+                    None,
                     json={},
                 )
             )["list"],
         )
 
     async def audit(
         self,
         villa_id: int,
         audit_content: str,
-        pass_through: str,
-        room_id: int,
-        uid: int,
+        pass_through: Optional[str] = None,
+        room_id: Optional[int] = None,
+        uid: Optional[int] = None,
     ) -> int:
+        """审核
+
+        审核用户配置内容是否合规，调用成功后会返回审核事件id(audit_id)。审核结果会通过回调接口异步通知。
+
+        参数:
+            villa_id: 大别野 ID
+            audit_content: 待审核内容
+            pass_through: 透传信息，该字段会在审核结果回调时携带给开发者，选填
+            room_id: 房间 id，选填
+            uid: 用户 id, 选填明
+
+        返回:
+            int: 审核事件 ID
+        """
         return (
             await self._request(
                 "POST",
-                "vila/api/bot/platform/audit",
+                "audit",
                 villa_id,
                 json={
                     "audit_content": audit_content,
                     "pass_through": pass_through,
                     "room_id": room_id,
                     "uid": uid,
                 },
             )
         )["audit_id"]
 
     def _get_headers(self, villa_id: Optional[int] = None) -> Dict[str, str]:
+        """获取鉴权请求头
+
+        参数:
+            villa_id: 大别野 ID，部分无需
+
+        返回:
+            Dict[str, str]: 请求头
+        """
         return {
             "x-rpc-bot_id": self.bot_id,
             "x-rpc-bot_secret": self.bot_secret,
             "x-rpc-bot_villa_id": str(villa_id) if villa_id else "",
         }
 
     async def _request(
         self,
-        method: str,
+        method: Literal["GET", "POST"],
         api: str,
         villa_id: Optional[int],
         json: Dict[str, Any],
         **kwargs,
     ) -> Any:
+        """请求 API
+
+        参数:
+            method: 请求方法
+            api: API 名称
+            villa_id: 大别野 ID
+            json: JSON请求体
+
+        异常:
+            ActionFailed: 动作失败
+            e: 其他请求异常
+
+        返回:
+            Any: 返回结果
+        """
         logger.opt(colors=True).debug(
-            f"<b><m>{self.bot_id}</m></b> | Calling API <y>{api.split('/')[-1]}</y>"
+            f"<b><m>{self.bot_id}</m></b> | Calling API <y>{api}</y>"
         )
         try:
-            async with httpx.AsyncClient() as client:
-                resp = await client.request(
-                    method=method,
-                    url=f"https://bbs-api.miyoushe.com/{api}",
-                    headers=self._get_headers(villa_id),
-                    json=json,
-                    **kwargs,
-                )
-                resp = ApiResponse.parse_raw(resp.content)
-                if resp.retcode == 0:
-                    return resp.data
-                else:
-                    raise ActionFailed(resp.retcode, resp)
+            resp = await self._client.request(
+                method=method,
+                url=api,
+                headers=self._get_headers(villa_id),
+                json=json,
+                **kwargs,
+            )
+            resp = ApiResponse.parse_raw(resp.content)
+            if resp.retcode == 0:
+                return resp.data
+            else:
+                raise ActionFailed(resp.retcode, resp)
         except Exception as e:
             raise e
 
+    async def _close_client(self) -> None:
+        """关闭 HTTP Client"""
+        await self._client.aclose()
+
     async def _handle_event(self, event: Event):
+        """处理事件
+
+        参数:
+            event: 事件
+        """
         is_handled = False
         for event_handler in self._event_handlers:
             if isinstance(event, event_handler.event_type):
                 if isinstance(event, SendMessageEvent):
                     if (
                         event_handler.startswith is not None
                         and not event.message.startswith(event_handler.startswith)
@@ -638,14 +952,15 @@
                     break
         if is_handled:
             logger.opt(colors=True).success(
                 f"<b><y>[{event.__class__.__name__}]</y></b> handle completed"
             )
 
     async def _parse_message_content(self, message: Message) -> MessageContentInfo:
+        """解析消息内容"""
         if quote := message["quote", 0]:
             quote = QuoteInfo(**quote.dict())
 
         if images_msg := (message["image"] or None):
             images_msg: List[ImageSegment]
             images = [
                 Image(
@@ -760,39 +1075,57 @@
     def run(
         self,
         host: str = "127.0.0.1",
         port: int = 13350,
         log_level: str = "INFO",
         **kwargs,
     ):
+        """启动机器人.
+
+        参数:
+            host: HOST 地址. 默认为 "127.0.0.1".
+            port: 端口号. 默认为 13350.
+            log_level: 日志等级. 默认为 "INFO".
+        """
         run_bots(bots=[self], host=host, port=port, log_level=log_level, **kwargs)
 
 
 def run_bots(
     bots: List[Bot],
     host: str = "127.0.0.1",
     port: int = 13350,
     log_level: str = "INFO",
     **kwargs,
 ):
+    """启动多个机器人.
+
+    参数:
+        bots: 机器人列表.
+        host: HOST 地址. 默认为 "127.0.0.1".
+        port: 端口号. 默认为 13350.
+        log_level: 日志等级. 默认为 "INFO".
+    """
     logger.configure(extra={"villa_log_level": log_level}, patcher=_log_patcher)
     logger.success("Starting Villa...")
     fastapi_kwargs = {
-        k.lstrip("fastapi"): v for k, v in kwargs.items() if k.startswith("fastapi_")
+        k.lstrip("fastapi_"): v for k, v in kwargs.items() if k.startswith("fastapi_")
     }
     uvicorn_kwargs = {
         k.lstrip("uvicorn_"): v for k, v in kwargs.items() if k.startswith("uvicorn_")
     }
-    app = FastAPI(**fastapi_kwargs)
+    app = get_app()
+    for key, value in fastapi_kwargs.items():
+        setattr(app, key, value)
     for bot in bots:
         logger.opt(colors=True).info(f"Initializing Bot <m>{bot.bot_id}</m>...")
         logger.opt(colors=True).debug(
             f"With Secret: <m>{bot.bot_secret}</m> and Callback URL: <m>{bot.callback_url}</m>"
         )
         app.post(bot.callback_url, status_code=200)(handle_event)
+        app.on_event("shutdown")(bot._close_client)
     uvicorn.run(
         app,
         host=host,
         port=port,
         log_config={
             "version": 1,
             "disable_existing_loggers": False,
@@ -810,14 +1143,15 @@
             },
         },
         **uvicorn_kwargs,
     )
 
 
 async def handle_event(data: dict) -> JSONResponse:
+    """处理事件"""
     if not (payload_data := data.get("event", None)):
         logger.warning(f"Received invalid data: {escape_tag(str(data))}")
         return JSONResponse(
             status_code=400, content={"retcode": -1, "msg": "Invalid data"}
         )
     try:
         payload = Payload.parse_obj(payload_data)
@@ -825,15 +1159,15 @@
         logger.opt(exception=e).warning(
             f"Failed to parse payload {escape_tag(str(payload_data))}"
         )
         return JSONResponse(
             status_code=400, content={"retcode": -1, "msg": "Invalid data"}
         )
     logger.trace(f"Received payload {escape_tag(repr(payload))}")
-    if not (bot := _bots.get(payload.robot.template.id, None)):
+    if (bot := get_bot(payload.robot.template.id)) is None:
         raise ValueError(f"Bot {payload.robot.template.id} not found")
     bot.bot_info = payload.robot
     if (event_class := event_classes.get(payload.type, None)) and (
         event_class.__type__.name in payload.extend_data["EventData"]
     ):
         try:
             event = event_class.parse_obj(
@@ -853,16 +1187,35 @@
             f"Unknown event type: {payload.type} data={escape_tag(str(payload.extend_data))}"
         )
 
     return JSONResponse(status_code=200, content={"retcode": 0, "message": "success"})
 
 
 async def run_handler(handler: EventHandler, event: Event):
+    """运行事件处理器"""
     try:
         if asyncio.iscoroutinefunction(handler.func):
             await handler.func(event)
         else:
             await run_sync(handler.func)(event)
     except Exception as e:
         logger.opt(exception=e).error(
             f"Error when running {handler} for {event.__class__.__name__}"
         )
+
+
+def on_startup(func: T_Func):
+    """让函数在 APP 启动时运行
+
+    参数:
+        func: 无参函数
+    """
+    get_app().on_event("startup")(func)
+
+
+def on_shutdown(func: T_Func):
+    """让函数在 APP 终止前运行
+
+    参数:
+        func: 无参函数
+    """
+    get_app().on_event("shutdown")(func)
```

### Comparing `villa-0.1.2/villa/event.py` & `villa-0.2.0/villa/event.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 from enum import IntEnum
 from typing import Dict, Type, Union, Optional
 
 from pydantic import Extra, BaseModel, root_validator
 
-from .store import _bots
+from .store import get_bot
 from .models import MessageContentInfo
 from .message import Message, MessageSegment
 
 
 class EventType(IntEnum):
     """事件类型"""
 
@@ -157,17 +157,29 @@
 
     async def send(
         self,
         message: Union[str, MessageSegment, Message],
         mention_sender: bool = False,
         quote_message: bool = False,
     ) -> str:
-        """回复消息"""
-        if not (bot := _bots.get(self.bot_id)):
-            raise ValueError("bot not found")
+        """对事件进行快速发送消息
+
+        参数:
+            message: 消息内容
+            mention_sender: 是否@发送者. 默认为 False.
+            quote_message: 是否引用事件消息. 默认为 False.
+
+        异常:
+            ValueError: 找不到 Bot 实例
+
+        返回:
+            str: 消息 ID
+        """
+        if (bot := get_bot(self.bot_id)) is None:
+            raise ValueError(f"Bot {self.bot_id} not found. Cannot send message.")
         if isinstance(message, (str, MessageSegment)):
             message = Message(message)
         if mention_sender:
             message.insert(
                 0, MessageSegment.mention_user(self.from_user_id, self.villa_id)
             )
         if quote_message:
```

### Comparing `villa-0.1.2/villa/log.py` & `villa-0.2.0/villa/log.py`

 * *Files identical despite different names*

### Comparing `villa-0.1.2/villa/message.py` & `villa-0.2.0/villa/message.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,21 +1,14 @@
 import re
 from abc import ABC
 from typing_extensions import Self
 from typing import List, Tuple, Union, Literal, Iterable, Iterator, Optional, overload
 
 from pydantic import Field, BaseModel
 
-from .models import Link as LinkInfo
-from .models import MessageContentInfo
-from .models import MentionedAll as MentionedAllInfo
-from .models import MentionedUser as MentionedUserInfo
-from .models import VillaRoomLink as VillaRoomLinkInfo
-from .models import MentionedRobot as MentionedRobotInfo
-
 MessageType = Literal[
     "text",
     "mention_user",
     "mention_all",
     "mention_robot",
     "room_link",
     "link",
```

### Comparing `villa-0.1.2/villa/models.py` & `villa-0.2.0/villa/models.py`

 * *Files identical despite different names*

### Comparing `villa-0.1.2/villa/typing.py` & `villa-0.2.0/villa/typing.py`

 * *Files 21% similar despite different names*

```diff
@@ -5,14 +5,15 @@
 
 from .event import Event
 
 T_Event = TypeVar("T_Event", bound=Event)
 
 
 T_Handler = Union[Callable[[T_Event], Any], Callable[[T_Event], Awaitable[Any]]]
+T_Func = Callable[..., Any]
 
 
 class EventHandler(BaseModel):
     event_type: Tuple[Type[Event], ...]
     func: T_Handler
     priority: int = 1
     block: bool = False
```

### Comparing `villa-0.1.2/villa/utils.py` & `villa-0.2.0/villa/utils.py`

 * *Files identical despite different names*

### Comparing `villa-0.1.2/PKG-INFO` & `villa-0.2.0/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: villa
-Version: 0.1.2
+Version: 0.2.0
 Summary: 米游社大别野Bot Python SDK。MiHoYo Villa Bot Python SDK.
 Home-page: https://github.com/CMHopeSunshine/villa-py
 License: MIT
 Keywords: mihoyo,bot,villa
 Author: CMHopeSunshine
 Author-email: 277073121@qq.com
 Requires-Python: >=3.8,<4.0
@@ -24,17 +24,25 @@
 
 <div align="center">
 
 # Villa
 
 _✨ 米游社大别野Bot Python SDK ✨_
 
-<img src="https://img.shields.io/pypi/v/villa-py" alt="version">
+<a href="https://cdn.jsdelivr.net/gh/CMHopeSunshine/villa-py@master/LICENSE">
+    <img src="https://img.shields.io/github/license/CMHopeSunshine/villa-py" alt="license">
+</a>
+<img src="https://img.shields.io/pypi/v/villa" alt="version">
 <img src="https://img.shields.io/badge/Python-3.8+-yellow" alt="python">
-<a href="https://cdn.jsdelivr.net/gh/CMHopeSunshine/villa-py@master/LICENSE"><img src="https://img.shields.io/github/license/CMHopeSunshine/villa-py" alt="license"></a>
+<a href="https://pypi.python.org/pypi/villa">
+  <img src="https://img.shields.io/pypi/dm/villa" alt="pypi download">
+</a>
+<a href="https://wakatime.com/badge/user/eed3f89c-5d65-46e6-ab19-78dcc4b62b3f/project/d3b88a99-17c2-4c98-bbc2-c1949ce7c078">
+  <img src="https://wakatime.com/badge/user/eed3f89c-5d65-46e6-ab19-78dcc4b62b3f/project/d3b88a99-17c2-4c98-bbc2-c1949ce7c078.svg" alt="wakatime">
+</a>
 
 </div>
 
 ## 特性
 
 - 基于`FastAPI`和`Pydantic`，异步、快速、高性能！
 - 完整的类型注解支持
@@ -46,15 +54,15 @@
 
 - 使用pip: `pip install villa`
 - 使用poetry: `poetry add villa`
 - 使用pdm: `pdm add villa`
 
 ## 快速开始
 
-首先你需要一个[米游社大别野](https://dby.miyoushe.com/chat)的Bot，如果没有请先到机器人开发者社区(别野ID: OpenVilla)申请，取得`bot_id`、`bot_secret`
+首先你需要一个[米游社大别野](https://dby.miyoushe.com/chat)的Bot，如果没有请先到[机器人开发者社区](https://dby.miyoushe.com/chat/463/20020)(别野ID: OpenVilla)申请，取得`bot_id`、`bot_secret`
 
 ```python
 from villa import Bot
 from villa.event import SendMessageEvent
 
 bot = Bot(bot_id="your_bot_id", bot_secret="your_bot_secret", callback_url="your_callback_url")
 # 初始化Bot，填写你的bot_id、密钥以及回调地址
```

