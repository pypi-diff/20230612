# Comparing `tmp/nonebot-plugin-mcversion-0.1.1.tar.gz` & `tmp/nonebot-plugin-mcversion-0.1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "nonebot-plugin-mcversion-0.1.1.tar", last modified: Sun May  7 12:15:47 2023, max compression
+gzip compressed data, was "nonebot-plugin-mcversion-0.1.2.tar", last modified: Mon Jun 12 14:44:59 2023, max compression
```

## Comparing `nonebot-plugin-mcversion-0.1.1.tar` & `nonebot-plugin-mcversion-0.1.2.tar`

### file list

```diff
@@ -1,5 +1,5 @@
--rw-r--r--   0        0        0     1065 2023-05-07 12:15:37.356691 nonebot-plugin-mcversion-0.1.1/LICENSE
--rw-r--r--   0        0        0     1931 2023-05-07 12:15:37.356691 nonebot-plugin-mcversion-0.1.1/README.md
--rw-r--r--   0        0        0     4114 2023-05-07 12:15:37.356691 nonebot-plugin-mcversion-0.1.1/nonebot_plugin_mcversion/__init__.py
--rw-r--r--   0        0        0      621 2023-05-07 12:15:37.356691 nonebot-plugin-mcversion-0.1.1/pyproject.toml
--rw-r--r--   0        0        0     2314 1970-01-01 00:00:00.000000 nonebot-plugin-mcversion-0.1.1/PKG-INFO
+-rw-r--r--   0        0        0     1065 2023-06-12 14:44:48.571203 nonebot-plugin-mcversion-0.1.2/LICENSE
+-rw-r--r--   0        0        0     1931 2023-06-12 14:44:48.571203 nonebot-plugin-mcversion-0.1.2/README.md
+-rw-r--r--   0        0        0     4199 2023-06-12 14:44:48.571203 nonebot-plugin-mcversion-0.1.2/nonebot_plugin_mcversion/__init__.py
+-rw-r--r--   0        0        0      621 2023-06-12 14:44:48.571203 nonebot-plugin-mcversion-0.1.2/pyproject.toml
+-rw-r--r--   0        0        0     2314 1970-01-01 00:00:00.000000 nonebot-plugin-mcversion-0.1.2/PKG-INFO
```

### Comparing `nonebot-plugin-mcversion-0.1.1/LICENSE` & `nonebot-plugin-mcversion-0.1.2/LICENSE`

 * *Files identical despite different names*

### Comparing `nonebot-plugin-mcversion-0.1.1/README.md` & `nonebot-plugin-mcversion-0.1.2/README.md`

 * *Files identical despite different names*

### Comparing `nonebot-plugin-mcversion-0.1.1/nonebot_plugin_mcversion/__init__.py` & `nonebot-plugin-mcversion-0.1.2/nonebot_plugin_mcversion/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -6,15 +6,15 @@
 from nonebot.adapters.onebot.v11 import Bot
 from nonebot.adapters.onebot.v11.message import Message
 
 env_config = Config(**get_driver().config.dict())
 mcver_group_id = list(env_config.mcver_group_id)
 
 # 定义命令“mcver”
-mcver = on_command('mcver', aliases={'mcversion', 'MC版本'}, priority=50)
+mcver = on_command('mcver',priority=50)
 
 # 处理命令“mcver”
 @mcver.handle()
 async def mcver_handle():
     # 获取Minecraft版本信息
     url = 'https://launchermeta.mojang.com/mc/game/version_manifest.json'
     response = requests.get(url)
@@ -66,33 +66,34 @@
         for i in mcver_group_id:
             int (i)
             await bot.send_group_msg(
                 group_id=i,
                 message=Message(f'发现MC更新：{latest_release} (Release)\n时间：{release_time}')
             )
     if latest_snapshot != old_snapshot:
-        # 更新版本信息
-        with open('data/latest_snapshot.txt', 'w') as f:
-            f.write(latest_snapshot)
-        # 获取版本发布时间
-        snapshot_time = ''
-        for version in data['versions']:
-            if version['id'] == latest_snapshot:
-                snapshot_time = version['releaseTime']
-                break
-        snapshot_time = datetime.strptime(snapshot_time, '%Y-%m-%dT%H:%M:%S%z')
-        snapshot_time = snapshot_time.replace(hour=snapshot_time.hour+8)
-        snapshot_time = snapshot_time.strftime('%Y-%m-%dT%H:%M:%S+08')
-        # 发送群消息
-        for i in mcver_group_id:
-            int (i)
-            await bot.send_group_msg(
-                group_id=i,
-                message=Message(f'发现MC更新：{latest_snapshot} (Snapshot)\n时间：{snapshot_time}')
-            )
+        if latest_snapshot != latest_release:
+            # 更新版本信息
+            with open('data/latest_snapshot.txt', 'w') as f:
+                f.write(latest_snapshot)
+            # 获取版本发布时间
+            snapshot_time = ''
+            for version in data['versions']:
+                if version['id'] == latest_snapshot:
+                    snapshot_time = version['releaseTime']
+                    break
+            snapshot_time = datetime.strptime(snapshot_time, '%Y-%m-%dT%H:%M:%S%z')
+            snapshot_time = snapshot_time.replace(hour=snapshot_time.hour+8)
+            snapshot_time = snapshot_time.strftime('%Y-%m-%dT%H:%M:%S+08')
+            # 发送群消息
+            for i in mcver_group_id:
+                int(i)
+                await bot.send_group_msg(
+                    group_id=i,
+                    message=Message(f'发现MC更新：{latest_snapshot} (Snapshot)\n时间：{snapshot_time}')
+                )
 # 获取nonebot的机器人实例
 from nonebot import get_bots
 # 定义定时任务，每分钟检查一次Minecraft更新
 @scheduler.scheduled_job('interval', minutes=1)
 async def mc_update_check():
     (bot, ) = get_bots().values()
     await check_mc_update(bot)
```

### Comparing `nonebot-plugin-mcversion-0.1.1/pyproject.toml` & `nonebot-plugin-mcversion-0.1.2/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [project]
 name = "nonebot-plugin-mcversion"
-version = "0.1.1"
+version = "0.1.2"
 description = "NoneBot2 plugin for CheckMCupdate"
 authors = [
     { name = "CN171-1", email = "3428166361@qq.com" },
 ]
 dependencies = [
     "nonebot2>=2.0.0rc2",
     "nonebot-adapter-onebot>=2.1.5",
```

### Comparing `nonebot-plugin-mcversion-0.1.1/PKG-INFO` & `nonebot-plugin-mcversion-0.1.2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: nonebot-plugin-mcversion
-Version: 0.1.1
+Version: 0.1.2
 Summary: NoneBot2 plugin for CheckMCupdate
 License: MIT
 Author-email: CN171-1 <3428166361@qq.com>
 Requires-Python: >=3.8
 Project-URL: Homepage, https://github.com/CN171-1/nonebot-plugin-mcversion
 Project-URL: Repository, https://github.com/CN171-1/nonebot-plugin-mcversion
 Description-Content-Type: text/markdown
```

