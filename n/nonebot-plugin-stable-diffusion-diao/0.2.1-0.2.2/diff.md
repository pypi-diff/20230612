# Comparing `tmp/nonebot_plugin_stable_diffusion_diao-0.2.1.tar.gz` & `tmp/nonebot_plugin_stable_diffusion_diao-0.2.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "nonebot_plugin_stable_diffusion_diao-0.2.1.tar", last modified: Tue May 30 17:07:19 2023, max compression
+gzip compressed data, was "nonebot_plugin_stable_diffusion_diao-0.2.2.tar", last modified: Mon Jun 12 05:16:58 2023, max compression
```

## Comparing `nonebot_plugin_stable_diffusion_diao-0.2.1.tar` & `nonebot_plugin_stable_diffusion_diao-0.2.2.tar`

### file list

```diff
@@ -1,39 +1,39 @@
--rw-r--r--   0        0        0     1082 2023-05-28 09:58:15.375966 nonebot_plugin_stable_diffusion_diao-0.2.1/LICENSE
--rw-r--r--   0        0        0      686 2023-05-28 09:58:15.400842 nonebot_plugin_stable_diffusion_diao-0.2.1/nonebot_plugin_stable_diffusion_diao/__init__.py
--rw-r--r--   0        0        0    18642 2023-05-30 17:04:49.624751 nonebot_plugin_stable_diffusion_diao-0.2.1/nonebot_plugin_stable_diffusion_diao/aidraw.py
--rw-r--r--   0        0        0     6213 2023-05-30 17:03:22.535709 nonebot_plugin_stable_diffusion_diao-0.2.1/nonebot_plugin_stable_diffusion_diao/amusement/chatgpt_tagger.py
--rw-r--r--   0        0        0        0 2023-05-28 09:58:15.402430 nonebot_plugin_stable_diffusion_diao-0.2.1/nonebot_plugin_stable_diffusion_diao/amusement/ramdomgirl.py
--rw-r--r--   0        0        0    65703 2023-05-30 17:03:23.970846 nonebot_plugin_stable_diffusion_diao-0.2.1/nonebot_plugin_stable_diffusion_diao/amusement/today_girl.py
--rw-r--r--   0        0        0     2528 2023-05-30 15:35:38.313378 nonebot_plugin_stable_diffusion_diao-0.2.1/nonebot_plugin_stable_diffusion_diao/amusement/vits.py
--rw-r--r--   0        0        0        0 2023-05-28 09:58:15.402952 nonebot_plugin_stable_diffusion_diao-0.2.1/nonebot_plugin_stable_diffusion_diao/amusement/wordbank.py
--rw-r--r--   0        0        0      699 2023-05-28 09:58:15.404033 nonebot_plugin_stable_diffusion_diao-0.2.1/nonebot_plugin_stable_diffusion_diao/backend/__init__.py
--rw-r--r--   0        0        0    15349 2023-05-30 14:20:07.688799 nonebot_plugin_stable_diffusion_diao-0.2.1/nonebot_plugin_stable_diffusion_diao/backend/base.py
--rw-r--r--   0        0        0     1279 2023-05-28 09:58:15.404557 nonebot_plugin_stable_diffusion_diao-0.2.1/nonebot_plugin_stable_diffusion_diao/backend/naifu.py
--rw-r--r--   0        0        0     1659 2023-05-28 09:58:15.405158 nonebot_plugin_stable_diffusion_diao-0.2.1/nonebot_plugin_stable_diffusion_diao/backend/novelai.py
--rw-r--r--   0        0        0     6300 2023-05-30 15:28:12.457021 nonebot_plugin_stable_diffusion_diao-0.2.1/nonebot_plugin_stable_diffusion_diao/backend/sd.py
--rw-r--r--   0        0        0    13640 2023-05-30 17:06:09.122349 nonebot_plugin_stable_diffusion_diao-0.2.1/nonebot_plugin_stable_diffusion_diao/config.py
--rw-r--r--   0        0        0     9282 2023-05-28 09:58:15.406675 nonebot_plugin_stable_diffusion_diao-0.2.1/nonebot_plugin_stable_diffusion_diao/extension/aidraw_help.py
--rw-r--r--   0        0        0     3340 2023-05-28 09:58:15.406675 nonebot_plugin_stable_diffusion_diao-0.2.1/nonebot_plugin_stable_diffusion_diao/extension/anlas.py
--rw-r--r--   0        0        0     1935 2023-05-28 09:58:15.406675 nonebot_plugin_stable_diffusion_diao-0.2.1/nonebot_plugin_stable_diffusion_diao/extension/control_net.py
--rw-r--r--   0        0        0     1102 2023-05-30 17:05:34.472127 nonebot_plugin_stable_diffusion_diao-0.2.1/nonebot_plugin_stable_diffusion_diao/extension/daylimit.py
--rw-r--r--   0        0        0     3751 2023-05-28 09:58:15.407673 nonebot_plugin_stable_diffusion_diao-0.2.1/nonebot_plugin_stable_diffusion_diao/extension/deepdanbooru.py
--rw-r--r--   0        0        0    11882 2023-05-30 15:32:52.299649 nonebot_plugin_stable_diffusion_diao-0.2.1/nonebot_plugin_stable_diffusion_diao/extension/explicit_api.py
--rw-r--r--   0        0        0     3668 2023-05-28 12:10:58.511567 nonebot_plugin_stable_diffusion_diao-0.2.1/nonebot_plugin_stable_diffusion_diao/extension/safe_method.py
--rw-r--r--   0        0        0    28782 2023-05-30 17:03:26.416767 nonebot_plugin_stable_diffusion_diao-0.2.1/nonebot_plugin_stable_diffusion_diao/extension/sd_extra_api_func.py
--rw-r--r--   0        0        0     5964 2023-05-28 09:58:15.408672 nonebot_plugin_stable_diffusion_diao-0.2.1/nonebot_plugin_stable_diffusion_diao/extension/translation.py
--rw-r--r--   0        0        0      400 2023-05-28 09:58:15.409671 nonebot_plugin_stable_diffusion_diao-0.2.1/nonebot_plugin_stable_diffusion_diao/fifo.py
--rw-r--r--   0        0        0        0 2023-05-28 09:58:15.410176 nonebot_plugin_stable_diffusion_diao-0.2.1/nonebot_plugin_stable_diffusion_diao/locales/__init__.py
--rw-r--r--   0        0        0        0 2023-05-28 09:58:15.410176 nonebot_plugin_stable_diffusion_diao-0.2.1/nonebot_plugin_stable_diffusion_diao/locales/en.py
--rw-r--r--   0        0        0        0 2023-05-28 09:58:15.410176 nonebot_plugin_stable_diffusion_diao-0.2.1/nonebot_plugin_stable_diffusion_diao/locales/jp.py
--rw-r--r--   0        0        0        0 2023-05-28 09:58:15.410176 nonebot_plugin_stable_diffusion_diao-0.2.1/nonebot_plugin_stable_diffusion_diao/locales/moe_jp.py
--rw-r--r--   0        0        0        0 2023-05-28 09:58:15.411183 nonebot_plugin_stable_diffusion_diao-0.2.1/nonebot_plugin_stable_diffusion_diao/locales/moe_zh.py
--rw-r--r--   0        0        0        0 2023-05-28 09:58:15.411183 nonebot_plugin_stable_diffusion_diao-0.2.1/nonebot_plugin_stable_diffusion_diao/locales/zh.py
--rw-r--r--   0        0        0     1905 2023-05-28 09:58:15.411183 nonebot_plugin_stable_diffusion_diao-0.2.1/nonebot_plugin_stable_diffusion_diao/manage.py
--rw-r--r--   0        0        0     1479 2023-05-28 09:58:15.412189 nonebot_plugin_stable_diffusion_diao-0.2.1/nonebot_plugin_stable_diffusion_diao/utils/__init__.py
--rw-r--r--   0        0        0     2314 2023-05-28 09:58:15.412189 nonebot_plugin_stable_diffusion_diao-0.2.1/nonebot_plugin_stable_diffusion_diao/utils/data.py
--rw-r--r--   0        0        0     7499 2023-05-30 15:27:52.695256 nonebot_plugin_stable_diffusion_diao-0.2.1/nonebot_plugin_stable_diffusion_diao/utils/load_balance.py
--rw-r--r--   0        0        0      647 2023-05-28 09:58:15.413187 nonebot_plugin_stable_diffusion_diao-0.2.1/nonebot_plugin_stable_diffusion_diao/utils/prepocess.py
--rw-r--r--   0        0        0      727 2023-05-28 09:58:15.413187 nonebot_plugin_stable_diffusion_diao-0.2.1/nonebot_plugin_stable_diffusion_diao/utils/save.py
--rw-r--r--   0        0        0     1994 2023-05-28 09:58:15.414188 nonebot_plugin_stable_diffusion_diao-0.2.1/nonebot_plugin_stable_diffusion_diao/version.py
--rw-r--r--   0        0        0      701 2023-05-30 17:07:19.612767 nonebot_plugin_stable_diffusion_diao-0.2.1/pyproject.toml
--rw-r--r--   0        0        0      442 1970-01-01 00:00:00.000000 nonebot_plugin_stable_diffusion_diao-0.2.1/PKG-INFO
+-rw-r--r--   0        0        0     1082 2023-05-28 09:58:15.375966 nonebot_plugin_stable_diffusion_diao-0.2.2/LICENSE
+-rw-r--r--   0        0        0      692 2023-05-31 13:01:37.260789 nonebot_plugin_stable_diffusion_diao-0.2.2/nonebot_plugin_stable_diffusion_diao/__init__.py
+-rw-r--r--   0        0        0    18642 2023-06-12 05:11:59.033569 nonebot_plugin_stable_diffusion_diao-0.2.2/nonebot_plugin_stable_diffusion_diao/aidraw.py
+-rw-r--r--   0        0        0     6213 2023-05-30 17:03:22.535709 nonebot_plugin_stable_diffusion_diao-0.2.2/nonebot_plugin_stable_diffusion_diao/amusement/chatgpt_tagger.py
+-rw-r--r--   0        0        0        0 2023-05-28 09:58:15.402430 nonebot_plugin_stable_diffusion_diao-0.2.2/nonebot_plugin_stable_diffusion_diao/amusement/ramdomgirl.py
+-rw-r--r--   0        0        0    65703 2023-05-30 17:03:23.970846 nonebot_plugin_stable_diffusion_diao-0.2.2/nonebot_plugin_stable_diffusion_diao/amusement/today_girl.py
+-rw-r--r--   0        0        0     3894 2023-06-12 05:12:59.000048 nonebot_plugin_stable_diffusion_diao-0.2.2/nonebot_plugin_stable_diffusion_diao/amusement/vits.py
+-rw-r--r--   0        0        0        0 2023-05-28 09:58:15.402952 nonebot_plugin_stable_diffusion_diao-0.2.2/nonebot_plugin_stable_diffusion_diao/amusement/wordbank.py
+-rw-r--r--   0        0        0      699 2023-05-28 09:58:15.404033 nonebot_plugin_stable_diffusion_diao-0.2.2/nonebot_plugin_stable_diffusion_diao/backend/__init__.py
+-rw-r--r--   0        0        0    15349 2023-05-30 14:20:07.688799 nonebot_plugin_stable_diffusion_diao-0.2.2/nonebot_plugin_stable_diffusion_diao/backend/base.py
+-rw-r--r--   0        0        0     1279 2023-05-28 09:58:15.404557 nonebot_plugin_stable_diffusion_diao-0.2.2/nonebot_plugin_stable_diffusion_diao/backend/naifu.py
+-rw-r--r--   0        0        0     1659 2023-05-28 09:58:15.405158 nonebot_plugin_stable_diffusion_diao-0.2.2/nonebot_plugin_stable_diffusion_diao/backend/novelai.py
+-rw-r--r--   0        0        0     5947 2023-06-10 12:00:09.717111 nonebot_plugin_stable_diffusion_diao-0.2.2/nonebot_plugin_stable_diffusion_diao/backend/sd.py
+-rw-r--r--   0        0        0    13640 2023-06-12 05:12:09.613233 nonebot_plugin_stable_diffusion_diao-0.2.2/nonebot_plugin_stable_diffusion_diao/config.py
+-rw-r--r--   0        0        0     9282 2023-05-28 09:58:15.406675 nonebot_plugin_stable_diffusion_diao-0.2.2/nonebot_plugin_stable_diffusion_diao/extension/aidraw_help.py
+-rw-r--r--   0        0        0     3340 2023-05-28 09:58:15.406675 nonebot_plugin_stable_diffusion_diao-0.2.2/nonebot_plugin_stable_diffusion_diao/extension/anlas.py
+-rw-r--r--   0        0        0     1935 2023-05-28 09:58:15.406675 nonebot_plugin_stable_diffusion_diao-0.2.2/nonebot_plugin_stable_diffusion_diao/extension/control_net.py
+-rw-r--r--   0        0        0     1102 2023-05-30 17:05:34.472127 nonebot_plugin_stable_diffusion_diao-0.2.2/nonebot_plugin_stable_diffusion_diao/extension/daylimit.py
+-rw-r--r--   0        0        0     3751 2023-05-28 09:58:15.407673 nonebot_plugin_stable_diffusion_diao-0.2.2/nonebot_plugin_stable_diffusion_diao/extension/deepdanbooru.py
+-rw-r--r--   0        0        0    11882 2023-05-30 15:32:52.299649 nonebot_plugin_stable_diffusion_diao-0.2.2/nonebot_plugin_stable_diffusion_diao/extension/explicit_api.py
+-rw-r--r--   0        0        0     3673 2023-05-31 13:33:47.513170 nonebot_plugin_stable_diffusion_diao-0.2.2/nonebot_plugin_stable_diffusion_diao/extension/safe_method.py
+-rw-r--r--   0        0        0    28782 2023-05-31 04:29:04.237402 nonebot_plugin_stable_diffusion_diao-0.2.2/nonebot_plugin_stable_diffusion_diao/extension/sd_extra_api_func.py
+-rw-r--r--   0        0        0     5964 2023-05-28 09:58:15.408672 nonebot_plugin_stable_diffusion_diao-0.2.2/nonebot_plugin_stable_diffusion_diao/extension/translation.py
+-rw-r--r--   0        0        0      400 2023-05-28 09:58:15.409671 nonebot_plugin_stable_diffusion_diao-0.2.2/nonebot_plugin_stable_diffusion_diao/fifo.py
+-rw-r--r--   0        0        0        0 2023-05-28 09:58:15.410176 nonebot_plugin_stable_diffusion_diao-0.2.2/nonebot_plugin_stable_diffusion_diao/locales/__init__.py
+-rw-r--r--   0        0        0        0 2023-05-28 09:58:15.410176 nonebot_plugin_stable_diffusion_diao-0.2.2/nonebot_plugin_stable_diffusion_diao/locales/en.py
+-rw-r--r--   0        0        0        0 2023-05-28 09:58:15.410176 nonebot_plugin_stable_diffusion_diao-0.2.2/nonebot_plugin_stable_diffusion_diao/locales/jp.py
+-rw-r--r--   0        0        0        0 2023-05-28 09:58:15.410176 nonebot_plugin_stable_diffusion_diao-0.2.2/nonebot_plugin_stable_diffusion_diao/locales/moe_jp.py
+-rw-r--r--   0        0        0        0 2023-05-28 09:58:15.411183 nonebot_plugin_stable_diffusion_diao-0.2.2/nonebot_plugin_stable_diffusion_diao/locales/moe_zh.py
+-rw-r--r--   0        0        0        0 2023-05-28 09:58:15.411183 nonebot_plugin_stable_diffusion_diao-0.2.2/nonebot_plugin_stable_diffusion_diao/locales/zh.py
+-rw-r--r--   0        0        0     1905 2023-05-28 09:58:15.411183 nonebot_plugin_stable_diffusion_diao-0.2.2/nonebot_plugin_stable_diffusion_diao/manage.py
+-rw-r--r--   0        0        0     1479 2023-05-28 09:58:15.412189 nonebot_plugin_stable_diffusion_diao-0.2.2/nonebot_plugin_stable_diffusion_diao/utils/__init__.py
+-rw-r--r--   0        0        0     2314 2023-05-28 09:58:15.412189 nonebot_plugin_stable_diffusion_diao-0.2.2/nonebot_plugin_stable_diffusion_diao/utils/data.py
+-rw-r--r--   0        0        0     7499 2023-05-30 15:27:52.695256 nonebot_plugin_stable_diffusion_diao-0.2.2/nonebot_plugin_stable_diffusion_diao/utils/load_balance.py
+-rw-r--r--   0        0        0      647 2023-05-28 09:58:15.413187 nonebot_plugin_stable_diffusion_diao-0.2.2/nonebot_plugin_stable_diffusion_diao/utils/prepocess.py
+-rw-r--r--   0        0        0      727 2023-05-28 09:58:15.413187 nonebot_plugin_stable_diffusion_diao-0.2.2/nonebot_plugin_stable_diffusion_diao/utils/save.py
+-rw-r--r--   0        0        0     1994 2023-05-28 09:58:15.414188 nonebot_plugin_stable_diffusion_diao-0.2.2/nonebot_plugin_stable_diffusion_diao/version.py
+-rw-r--r--   0        0        0      701 2023-06-12 05:16:58.457184 nonebot_plugin_stable_diffusion_diao-0.2.2/pyproject.toml
+-rw-r--r--   0        0        0      442 1970-01-01 00:00:00.000000 nonebot_plugin_stable_diffusion_diao-0.2.2/PKG-INFO
```

### Comparing `nonebot_plugin_stable_diffusion_diao-0.2.1/LICENSE` & `nonebot_plugin_stable_diffusion_diao-0.2.2/LICENSE`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_stable_diffusion_diao-0.2.1/nonebot_plugin_stable_diffusion_diao/__init__.py` & `nonebot_plugin_stable_diffusion_diao-0.2.2/nonebot_plugin_stable_diffusion_diao/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from . import config, manage
 from .aidraw import AIDRAW
 from nonebot.plugin import PluginMetadata
 from .extension.deepdanbooru import deepdanbooru
-from .amusement import today_girl, chatgpt_tagger
+from .amusement import today_girl, chatgpt_tagger, vits
 from .extension import sd_extra_api_func, aidraw_help
 
 __plugin_meta__ = PluginMetadata(
     name="AI绘图",
     description="调用novelai进行二次元AI绘图",
     usage=f"发送 绘画帮助 获取更多帮助\n基础用法:\n.aidraw[指令] [空格] loli,[参数]\n示例:.aidraw loli,cute,kawaii,\n项目地址:https://github.com/Mutsukibot/tree/nonebot-plugin-novelai\n说明书：https://sena-nana.github.io/MutsukiDocs/",
 )
```

### Comparing `nonebot_plugin_stable_diffusion_diao-0.2.1/nonebot_plugin_stable_diffusion_diao/aidraw.py` & `nonebot_plugin_stable_diffusion_diao-0.2.2/nonebot_plugin_stable_diffusion_diao/aidraw.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_stable_diffusion_diao-0.2.1/nonebot_plugin_stable_diffusion_diao/amusement/chatgpt_tagger.py` & `nonebot_plugin_stable_diffusion_diao-0.2.2/nonebot_plugin_stable_diffusion_diao/amusement/chatgpt_tagger.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_stable_diffusion_diao-0.2.1/nonebot_plugin_stable_diffusion_diao/amusement/today_girl.py` & `nonebot_plugin_stable_diffusion_diao-0.2.2/nonebot_plugin_stable_diffusion_diao/amusement/today_girl.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_stable_diffusion_diao-0.2.1/nonebot_plugin_stable_diffusion_diao/backend/__init__.py` & `nonebot_plugin_stable_diffusion_diao-0.2.2/nonebot_plugin_stable_diffusion_diao/backend/__init__.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_stable_diffusion_diao-0.2.1/nonebot_plugin_stable_diffusion_diao/backend/base.py` & `nonebot_plugin_stable_diffusion_diao-0.2.2/nonebot_plugin_stable_diffusion_diao/backend/base.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_stable_diffusion_diao-0.2.1/nonebot_plugin_stable_diffusion_diao/backend/naifu.py` & `nonebot_plugin_stable_diffusion_diao-0.2.2/nonebot_plugin_stable_diffusion_diao/backend/naifu.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_stable_diffusion_diao-0.2.1/nonebot_plugin_stable_diffusion_diao/backend/novelai.py` & `nonebot_plugin_stable_diffusion_diao-0.2.2/nonebot_plugin_stable_diffusion_diao/backend/novelai.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_stable_diffusion_diao-0.2.1/nonebot_plugin_stable_diffusion_diao/backend/sd.py` & `nonebot_plugin_stable_diffusion_diao-0.2.2/nonebot_plugin_stable_diffusion_diao/backend/sd.py`

 * *Files 4% similar despite different names*

```diff
@@ -38,30 +38,25 @@
         return resp_tuple
 
     async def post_parameters(self):
         '''
         获取post参数
         '''
         global site
+        if self.backend_index is not None and isinstance(self.backend_index, int):
+            self.backend_site = list(config.novelai_backend_url_dict.values())[self.backend_index]
         if self.backend_site:
             site = self.backend_site
         else:
             if config.novelai_load_balance:
-                if self.backend_index is not None and isinstance(self.backend_index, int):
-                    site = list(config.novelai_backend_url_dict.values())[self.backend_index]
-                    self.backend_site = site
-                else:
-                    await self.load_balance_init()
-                    site = self.backend_site or defult_site 
+                await self.load_balance_init()
+                site = self.backend_site or defult_site 
             else:
-                if self.backend_index is not None and isinstance(self.backend_index, int):
-                    site = defult_site or list(config.novelai_backend_url_dict.values())[self.backend_index]
-                    self.backend_site = site
-                else:
-                    site = defult_site or await config.get_value(self.group_id, "site") or config.novelai_site or "127.0.0.1:7860"
+                site = defult_site or await config.get_value(self.group_id, "site") or config.novelai_site or "127.0.0.1:7860"
+
         post_api = f"http://{site}/sdapi/v1/img2img" if self.img2img else f"http://{site}/sdapi/v1/txt2img"
         
         parameters = {
             "prompt": self.tags,
             "seed": self.seed,
             "steps": self.steps,
             "cfg_scale": self.scale,
```

### Comparing `nonebot_plugin_stable_diffusion_diao-0.2.1/nonebot_plugin_stable_diffusion_diao/config.py` & `nonebot_plugin_stable_diffusion_diao-0.2.2/nonebot_plugin_stable_diffusion_diao/config.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_stable_diffusion_diao-0.2.1/nonebot_plugin_stable_diffusion_diao/extension/aidraw_help.py` & `nonebot_plugin_stable_diffusion_diao-0.2.2/nonebot_plugin_stable_diffusion_diao/extension/aidraw_help.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_stable_diffusion_diao-0.2.1/nonebot_plugin_stable_diffusion_diao/extension/anlas.py` & `nonebot_plugin_stable_diffusion_diao-0.2.2/nonebot_plugin_stable_diffusion_diao/extension/anlas.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_stable_diffusion_diao-0.2.1/nonebot_plugin_stable_diffusion_diao/extension/control_net.py` & `nonebot_plugin_stable_diffusion_diao-0.2.2/nonebot_plugin_stable_diffusion_diao/extension/control_net.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_stable_diffusion_diao-0.2.1/nonebot_plugin_stable_diffusion_diao/extension/daylimit.py` & `nonebot_plugin_stable_diffusion_diao-0.2.2/nonebot_plugin_stable_diffusion_diao/extension/daylimit.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_stable_diffusion_diao-0.2.1/nonebot_plugin_stable_diffusion_diao/extension/deepdanbooru.py` & `nonebot_plugin_stable_diffusion_diao-0.2.2/nonebot_plugin_stable_diffusion_diao/extension/deepdanbooru.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_stable_diffusion_diao-0.2.1/nonebot_plugin_stable_diffusion_diao/extension/explicit_api.py` & `nonebot_plugin_stable_diffusion_diao-0.2.2/nonebot_plugin_stable_diffusion_diao/extension/explicit_api.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_stable_diffusion_diao-0.2.1/nonebot_plugin_stable_diffusion_diao/extension/safe_method.py` & `nonebot_plugin_stable_diffusion_diao-0.2.2/nonebot_plugin_stable_diffusion_diao/extension/safe_method.py`

 * *Files 1% similar despite different names*

```diff
@@ -59,15 +59,15 @@
     else:
         if isinstance(message, str):
             new_list.append(message)
         else:
             new_list.append(message)
     if md_temple:
         for img in new_list:
-            msg_list = "".join(img)
+            msg_list = "".join(str(img))
             markdown = await markdown_temple(bot, msg_list)
             img = await md_to_pic(md=markdown, width=width)
             await bot.send(event=event, message=MessageSegment.image(img))
     if isinstance(message, list):
         if is_forward:
             msg_list = ["".join(message[i:i+10]) for i in range(0, len(message), 10)]
             try:
```

### Comparing `nonebot_plugin_stable_diffusion_diao-0.2.1/nonebot_plugin_stable_diffusion_diao/extension/sd_extra_api_func.py` & `nonebot_plugin_stable_diffusion_diao-0.2.2/nonebot_plugin_stable_diffusion_diao/extension/sd_extra_api_func.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_stable_diffusion_diao-0.2.1/nonebot_plugin_stable_diffusion_diao/extension/translation.py` & `nonebot_plugin_stable_diffusion_diao-0.2.2/nonebot_plugin_stable_diffusion_diao/extension/translation.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_stable_diffusion_diao-0.2.1/nonebot_plugin_stable_diffusion_diao/manage.py` & `nonebot_plugin_stable_diffusion_diao-0.2.2/nonebot_plugin_stable_diffusion_diao/manage.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_stable_diffusion_diao-0.2.1/nonebot_plugin_stable_diffusion_diao/utils/__init__.py` & `nonebot_plugin_stable_diffusion_diao-0.2.2/nonebot_plugin_stable_diffusion_diao/utils/__init__.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_stable_diffusion_diao-0.2.1/nonebot_plugin_stable_diffusion_diao/utils/data.py` & `nonebot_plugin_stable_diffusion_diao-0.2.2/nonebot_plugin_stable_diffusion_diao/utils/data.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_stable_diffusion_diao-0.2.1/nonebot_plugin_stable_diffusion_diao/utils/load_balance.py` & `nonebot_plugin_stable_diffusion_diao-0.2.2/nonebot_plugin_stable_diffusion_diao/utils/load_balance.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_stable_diffusion_diao-0.2.1/nonebot_plugin_stable_diffusion_diao/utils/prepocess.py` & `nonebot_plugin_stable_diffusion_diao-0.2.2/nonebot_plugin_stable_diffusion_diao/utils/prepocess.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_stable_diffusion_diao-0.2.1/nonebot_plugin_stable_diffusion_diao/utils/save.py` & `nonebot_plugin_stable_diffusion_diao-0.2.2/nonebot_plugin_stable_diffusion_diao/utils/save.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_stable_diffusion_diao-0.2.1/nonebot_plugin_stable_diffusion_diao/version.py` & `nonebot_plugin_stable_diffusion_diao-0.2.2/nonebot_plugin_stable_diffusion_diao/version.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_stable_diffusion_diao-0.2.1/pyproject.toml` & `nonebot_plugin_stable_diffusion_diao-0.2.2/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [project]
 name = "nonebot-plugin-stable-diffusion-diao"
-version = "0.2.1"
+version = "0.2.2"
 description = "主要面对stable-diffusion-webui-api的nonebot2插件"
 authors = [
     { name = "DiaoDaiaChan", email = "diaodaiachan@qq.com" },
 ]
 dependencies = [
     "aiofiles>=23.1.0",
     "aiohttp>=3.8.4",
```

