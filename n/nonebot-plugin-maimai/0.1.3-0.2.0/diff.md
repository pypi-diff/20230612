# Comparing `tmp/nonebot_plugin_maimai-0.1.3.tar.gz` & `tmp/nonebot_plugin_maimai-0.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "nonebot_plugin_maimai-0.1.3.tar", max compression
+gzip compressed data, was "nonebot_plugin_maimai-0.2.0.tar", max compression
```

## Comparing `nonebot_plugin_maimai-0.1.3.tar` & `nonebot_plugin_maimai-0.2.0.tar`

### file list

```diff
@@ -1,13 +1,12 @@
--rw-r--r--   0        0        0     1089 2023-02-08 00:46:07.674998 nonebot_plugin_maimai-0.1.3/LICENSE
--rw-r--r--   0        0        0    13115 2023-04-18 11:07:27.814657 nonebot_plugin_maimai-0.1.3/nonebot_plugin_maimai/__init__.py
--rw-r--r--   0        0        0        0 2023-02-08 03:30:51.719115 nonebot_plugin_maimai-0.1.3/nonebot_plugin_maimai/libraries/__init__.py
--rw-r--r--   0        0        0     1605 2023-02-08 01:36:17.843087 nonebot_plugin_maimai-0.1.3/nonebot_plugin_maimai/libraries/image.py
--rw-r--r--   0        0        0    17833 2023-02-13 15:25:45.342461 nonebot_plugin_maimai-0.1.3/nonebot_plugin_maimai/libraries/maimai_best_40.py
--rw-r--r--   0        0        0    17924 2023-02-08 01:57:57.403213 nonebot_plugin_maimai-0.1.3/nonebot_plugin_maimai/libraries/maimai_best_50.py
--rw-r--r--   0        0        0     5218 2023-02-08 06:25:11.968762 nonebot_plugin_maimai-0.1.3/nonebot_plugin_maimai/libraries/maimaidx_music.py
--rw-r--r--   0        0        0      397 2023-03-02 02:30:46.242798 nonebot_plugin_maimai-0.1.3/nonebot_plugin_maimai/libraries/tool.py
--rw-r--r--   0        0        0     7266 2023-04-18 16:25:08.291032 nonebot_plugin_maimai-0.1.3/nonebot_plugin_maimai/public.py
--rw-r--r--   0        0        0     1085 2023-04-18 16:27:16.980558 nonebot_plugin_maimai-0.1.3/pyproject.toml
--rw-r--r--   0        0        0     3481 2023-04-18 16:29:53.751976 nonebot_plugin_maimai-0.1.3/README.md
--rw-r--r--   0        0        0     4383 1970-01-01 00:00:00.000000 nonebot_plugin_maimai-0.1.3/setup.py
--rw-r--r--   0        0        0     4665 1970-01-01 00:00:00.000000 nonebot_plugin_maimai-0.1.3/PKG-INFO
+-rw-r--r--   0        0        0     1089 2023-02-08 00:46:07.674998 nonebot_plugin_maimai-0.2.0/LICENSE
+-rw-r--r--   0        0        0    13245 2023-06-12 14:56:52.704104 nonebot_plugin_maimai-0.2.0/nonebot_plugin_maimai/__init__.py
+-rw-r--r--   0        0        0        0 2023-02-08 03:30:51.719115 nonebot_plugin_maimai-0.2.0/nonebot_plugin_maimai/libraries/__init__.py
+-rw-r--r--   0        0        0     1605 2023-02-08 01:36:17.843087 nonebot_plugin_maimai-0.2.0/nonebot_plugin_maimai/libraries/image.py
+-rw-r--r--   0        0        0    17837 2023-06-12 14:49:23.491131 nonebot_plugin_maimai-0.2.0/nonebot_plugin_maimai/libraries/maimai_best_40.py
+-rw-r--r--   0        0        0    17928 2023-06-12 14:49:22.832470 nonebot_plugin_maimai-0.2.0/nonebot_plugin_maimai/libraries/maimai_best_50.py
+-rw-r--r--   0        0        0     5522 2023-06-12 14:49:03.118975 nonebot_plugin_maimai-0.2.0/nonebot_plugin_maimai/libraries/maimaidx_music.py
+-rw-r--r--   0        0        0      397 2023-03-02 02:30:46.242798 nonebot_plugin_maimai-0.2.0/nonebot_plugin_maimai/libraries/tool.py
+-rw-r--r--   0        0        0     7497 2023-05-20 16:28:12.333709 nonebot_plugin_maimai-0.2.0/nonebot_plugin_maimai/public.py
+-rw-r--r--   0        0        0     1062 2023-06-12 14:55:04.696808 nonebot_plugin_maimai-0.2.0/pyproject.toml
+-rw-r--r--   0        0        0     3478 2023-06-12 14:54:59.661881 nonebot_plugin_maimai-0.2.0/README.md
+-rw-r--r--   0        0        0     4428 1970-01-01 00:00:00.000000 nonebot_plugin_maimai-0.2.0/PKG-INFO
```

### Comparing `nonebot_plugin_maimai-0.1.3/LICENSE` & `nonebot_plugin_maimai-0.2.0/LICENSE`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_maimai-0.1.3/nonebot_plugin_maimai/__init__.py` & `nonebot_plugin_maimai-0.2.0/nonebot_plugin_maimai/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -23,28 +23,30 @@
     nickname = "宁宁"
 
 __version__ = "0.1.0"
 __plugin_meta__ = PluginMetadata(
     name="舞萌maimai",
     description='指令：舞萌帮助',
     usage='指令：舞萌帮助',
+    type="application",
+    homepage="https://github.com/Agnes4m/nonebot_plugin_maimai",
+    supported_adapters={"~onebot.v11"},
     extra={
         "version": __version__,
         "author": "Umamusume-Agnes-Digital <Z735803792@163.com>",
     },
 )
 
-
 def song_txt(music: Music):
     return Message([
         MessageSegment("text", {
             "text": f"{music.id}. {music.title}\n"
         }),
         MessageSegment("image", {
-            "file": f"https://www.diving-fish.com/covers/{get_cover_len4_id(music.id)}.png"
+            "file": f"https://www.diving-fish.com/covers/{get_cover_len5_id(music.id)}.png"
         }),
         MessageSegment("text", {
             "text": f"\n{'/'.join(music.level)}"
         })
     ])
 
 
@@ -158,15 +160,15 @@
             level_index = level_labels.index(groups[0])
             level_name = ['Basic', 'Advanced', 'Expert', 'Master', 'Re: MASTER']
             name = groups[1]
             music = total_list.by_id(name)
             chart = music['charts'][level_index]
             ds = music['ds'][level_index]
             level = music['level'][level_index]
-            file = f"https://www.diving-fish.com/covers/{get_cover_len4_id(music['id'])}.png"
+            file = f"https://www.diving-fish.com/covers/{get_cover_len5_id(music['id'])}.png"
             if len(chart['notes']) == 4:
                 msg = f'''{level_name[level_index]} {level}({ds})
 TAP: {chart['notes'][0]}
 HOLD: {chart['notes'][1]}
 SLIDE: {chart['notes'][2]}
 BREAK: {chart['notes'][3]}
 谱师: {chart['charter']}'''
@@ -191,15 +193,15 @@
             ]))
         except Exception:
             await query_chart.send("未找到该谱面")
     else:
         name = groups[1]
         music = total_list.by_id(name)
         try:
-            file =f"https://www.diving-fish.com/covers/{get_cover_len4_id(music['id'])}.png"
+            file =f"https://www.diving-fish.com/covers/{get_cover_len5_id(music['id'])}.png"
             await query_chart.send(Message([
                 MessageSegment("text", {
                     "text": f"{music['id']}. {music['title']}\n"
                 }),
                 MessageSegment("image", {
                     "file": f"{file}"
                 }),
```

### Comparing `nonebot_plugin_maimai-0.1.3/nonebot_plugin_maimai/libraries/image.py` & `nonebot_plugin_maimai-0.2.0/nonebot_plugin_maimai/libraries/image.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_maimai-0.1.3/nonebot_plugin_maimai/libraries/maimai_best_40.py` & `nonebot_plugin_maimai-0.2.0/nonebot_plugin_maimai/libraries/maimai_best_40.py`

 * *Files 1% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 
 import os
 import math
 from typing import Optional, Dict, List,Tuple
 from .tool import STATIC
 import aiohttp
 from PIL import Image, ImageDraw, ImageFont, ImageFilter
-from .maimaidx_music import get_cover_len4_id, total_list
+from .maimaidx_music import get_cover_len5_id, total_list
 
 
 scoreRank = 'D C B BB BBB A AA AAA S S+ SS SS+ SSS SSS+'.split(' ')
 combo = ' FC FC+ AP AP+'.split(' ')
 diffs = 'Basic Advanced Expert Master Re:Master'.split(' ')
 
 
@@ -200,17 +200,17 @@
         comboPic = ' FC FCp AP APp'.split(' ')
         imgDraw = ImageDraw.Draw(img)
         titleFontName = STATIC + '/adobe_simhei.otf'
         for num in range(0, len(sdBest)):
             i = num // 5
             j = num % 5
             chartInfo = sdBest[num]
-            pngPath = self.cover_dir + f'{get_cover_len4_id(chartInfo.idNum)}.png'
+            pngPath = self.cover_dir + f'{get_cover_len5_id(chartInfo.idNum)}.png'
             if not os.path.exists(pngPath):
-                pngPath = self.cover_dir + '1000.png'
+                pngPath = self.cover_dir + '01000.png'
             temp = Image.open(pngPath).convert('RGB')
             temp = self._resizePic(temp, itemW / temp.size[0])
             temp = temp.crop((0, (temp.size[1] - itemH) / 2, itemW, (temp.size[1] + itemH) / 2))
             temp = temp.filter(ImageFilter.GaussianBlur(3))
             temp = temp.point(lambda p: int(p * 0.72))
 
             tempDraw = ImageDraw.Draw(temp)
@@ -238,26 +238,26 @@
             recBase = Image.new('RGBA', (itemW, itemH), 'black')
             recBase = recBase.point(lambda p: int(p * 0.8))
             img.paste(recBase, (self.COLOUMS_IMG[j] + 5, self.ROWS_IMG[i + 1] + 5))
             img.paste(temp, (self.COLOUMS_IMG[j] + 4, self.ROWS_IMG[i + 1] + 4))
         for num in range(len(sdBest), sdBest.size):
             i = num // 5
             j = num % 5
-            temp = Image.open(self.cover_dir + f'1000.png').convert('RGB')
+            temp = Image.open(self.cover_dir + f'01000.png').convert('RGB')
             temp = self._resizePic(temp, itemW / temp.size[0])
             temp = temp.crop((0, (temp.size[1] - itemH) / 2, itemW, (temp.size[1] + itemH) / 2))
             temp = temp.filter(ImageFilter.GaussianBlur(1))
             img.paste(temp, (self.COLOUMS_IMG[j] + 4, self.ROWS_IMG[i + 1] + 4))
         for num in range(0, len(dxBest)):
             i = num // 3
             j = num % 3
             chartInfo = dxBest[num]
-            pngPath = self.cover_dir + f'{get_cover_len4_id(chartInfo.idNum)}.png'
+            pngPath = self.cover_dir + f'{get_cover_len5_id(chartInfo.idNum)}.png'
             if not os.path.exists(pngPath):
-                pngPath = self.cover_dir + '1000.png'
+                pngPath = self.cover_dir + '01000.png'
             temp = Image.open(pngPath).convert('RGB')
             temp = self._resizePic(temp, itemW / temp.size[0])
             temp = temp.crop((0, (temp.size[1] - itemH) / 2, itemW, (temp.size[1] + itemH) / 2))
             temp = temp.filter(ImageFilter.GaussianBlur(3))
             temp = temp.point(lambda p: int(p * 0.72))
 
             tempDraw = ImageDraw.Draw(temp)
@@ -286,15 +286,15 @@
             recBase = Image.new('RGBA', (itemW, itemH), 'black')
             recBase = recBase.point(lambda p: int(p * 0.8))
             img.paste(recBase, (self.COLOUMS_IMG[j + 6] + 5, self.ROWS_IMG[i + 1] + 5))
             img.paste(temp, (self.COLOUMS_IMG[j + 6] + 4, self.ROWS_IMG[i + 1] + 4))
         for num in range(len(dxBest), dxBest.size):
             i = num // 3
             j = num % 3
-            temp = Image.open(self.cover_dir + f'1000.png').convert('RGB')
+            temp = Image.open(self.cover_dir + f'01000.png').convert('RGB')
             temp = self._resizePic(temp, itemW / temp.size[0])
             temp = temp.crop((0, (temp.size[1] - itemH) / 2, itemW, (temp.size[1] + itemH) / 2))
             temp = temp.filter(ImageFilter.GaussianBlur(1))
             img.paste(temp, (self.COLOUMS_IMG[j + 6] + 4, self.ROWS_IMG[i + 1] + 4))
 
     def draw(self):
         splashLogo = Image.open(self.pic_dir + 'UI_CMN_TabTitle_MaimaiTitle_Ver214.png').convert('RGBA')
```

### Comparing `nonebot_plugin_maimai-0.1.3/nonebot_plugin_maimai/libraries/maimai_best_50.py` & `nonebot_plugin_maimai-0.2.0/nonebot_plugin_maimai/libraries/maimai_best_50.py`

 * *Files 0% similar despite different names*

```diff
@@ -8,15 +8,15 @@
 00000070: 7470 0d0a 6672 6f6d 2050 494c 2069 6d70  tp..from PIL imp
 00000080: 6f72 7420 496d 6167 652c 2049 6d61 6765  ort Image, Image
 00000090: 4472 6177 2c20 496d 6167 6546 6f6e 742c  Draw, ImageFont,
 000000a0: 2049 6d61 6765 4669 6c74 6572 0d0a 6672   ImageFilter..fr
 000000b0: 6f6d 202e 6d61 696d 6169 6478 5f6d 7573  om .maimaidx_mus
 000000c0: 6963 2069 6d70 6f72 7420 746f 7461 6c5f  ic import total_
 000000d0: 6c69 7374 2c20 6765 745f 636f 7665 725f  list, get_cover_
-000000e0: 6c65 6e34 5f69 640d 0a0d 0a0d 0a73 636f  len4_id......sco
+000000e0: 6c65 6e35 5f69 640d 0a0d 0a0d 0a73 636f  len5_id......sco
 000000f0: 7265 5261 6e6b 203d 2027 4420 4320 4220  reRank = 'D C B 
 00000100: 4242 2042 4242 2041 2041 4120 4141 4120  BB BBB A AA AAA 
 00000110: 5320 532b 2053 5320 5353 2b20 5353 5320  S S+ SS SS+ SSS 
 00000120: 5353 532b 272e 7370 6c69 7428 2720 2729  SSS+'.split(' ')
 00000130: 0d0a 636f 6d62 6f20 3d20 2720 4643 2046  ..combo = ' FC F
 00000140: 432b 2041 5020 4150 2b27 2e73 706c 6974  C+ AP AP+'.split
 00000150: 2827 2027 290d 0a64 6966 6673 203d 2027  (' ')..diffs = '
@@ -445,677 +445,677 @@
 00001bc0: 2020 2020 2020 2020 2020 2020 6a20 3d20              j = 
 00001bd0: 6e75 6d20 2520 370d 0a20 2020 2020 2020  num % 7..       
 00001be0: 2020 2020 2063 6861 7274 496e 666f 203d       chartInfo =
 00001bf0: 2073 6442 6573 745b 6e75 6d5d 0d0a 2020   sdBest[num]..  
 00001c00: 2020 2020 2020 2020 2020 706e 6750 6174            pngPat
 00001c10: 6820 3d20 7365 6c66 2e63 6f76 6572 5f64  h = self.cover_d
 00001c20: 6972 202b 2066 277b 6765 745f 636f 7665  ir + f'{get_cove
-00001c30: 725f 6c65 6e34 5f69 6428 6368 6172 7449  r_len4_id(chartI
+00001c30: 725f 6c65 6e35 5f69 6428 6368 6172 7449  r_len5_id(chartI
 00001c40: 6e66 6f2e 6964 4e75 6d29 7d2e 706e 6727  nfo.idNum)}.png'
 00001c50: 0d0a 2020 2020 2020 2020 2020 2020 6966  ..            if
 00001c60: 206e 6f74 206f 732e 7061 7468 2e65 7869   not os.path.exi
 00001c70: 7374 7328 706e 6750 6174 6829 3a0d 0a20  sts(pngPath):.. 
 00001c80: 2020 2020 2020 2020 2020 2020 2020 2070                 p
 00001c90: 6e67 5061 7468 203d 2073 656c 662e 636f  ngPath = self.co
-00001ca0: 7665 725f 6469 7220 2b20 2731 3030 302e  ver_dir + '1000.
-00001cb0: 706e 6727 0d0a 2020 2020 2020 2020 2020  png'..          
-00001cc0: 2020 7465 6d70 203d 2049 6d61 6765 2e6f    temp = Image.o
-00001cd0: 7065 6e28 706e 6750 6174 6829 2e63 6f6e  pen(pngPath).con
-00001ce0: 7665 7274 2827 5247 4227 290d 0a20 2020  vert('RGB')..   
-00001cf0: 2020 2020 2020 2020 2074 656d 7020 3d20           temp = 
-00001d00: 7365 6c66 2e5f 7265 7369 7a65 5069 6328  self._resizePic(
-00001d10: 7465 6d70 2c20 6974 656d 5720 2f20 7465  temp, itemW / te
-00001d20: 6d70 2e73 697a 655b 305d 290d 0a20 2020  mp.size[0])..   
-00001d30: 2020 2020 2020 2020 2074 656d 7020 3d20           temp = 
-00001d40: 7465 6d70 2e63 726f 7028 2830 2c20 2874  temp.crop((0, (t
-00001d50: 656d 702e 7369 7a65 5b31 5d20 2d20 6974  emp.size[1] - it
-00001d60: 656d 4829 202f 2032 2c20 6974 656d 572c  emH) / 2, itemW,
-00001d70: 2028 7465 6d70 2e73 697a 655b 315d 202b   (temp.size[1] +
-00001d80: 2069 7465 6d48 2920 2f20 3229 290d 0a20   itemH) / 2)).. 
-00001d90: 2020 2020 2020 2020 2020 2074 656d 7020             temp 
-00001da0: 3d20 7465 6d70 2e66 696c 7465 7228 496d  = temp.filter(Im
-00001db0: 6167 6546 696c 7465 722e 4761 7573 7369  ageFilter.Gaussi
-00001dc0: 616e 426c 7572 2833 2929 0d0a 2020 2020  anBlur(3))..    
-00001dd0: 2020 2020 2020 2020 7465 6d70 203d 2074          temp = t
-00001de0: 656d 702e 706f 696e 7428 6c61 6d62 6461  emp.point(lambda
-00001df0: 2070 3a20 696e 7428 7020 2a20 302e 3732   p: int(p * 0.72
-00001e00: 2929 0d0a 0d0a 2020 2020 2020 2020 2020  ))....          
-00001e10: 2020 7465 6d70 4472 6177 203d 2049 6d61    tempDraw = Ima
-00001e20: 6765 4472 6177 2e44 7261 7728 7465 6d70  geDraw.Draw(temp
-00001e30: 290d 0a20 2020 2020 2020 2020 2020 2074  )..            t
-00001e40: 656d 7044 7261 772e 706f 6c79 676f 6e28  empDraw.polygon(
-00001e50: 6c65 7665 6c54 7269 6167 6c65 2c20 436f  levelTriagle, Co
-00001e60: 6c6f 725b 6368 6172 7449 6e66 6f2e 6469  lor[chartInfo.di
-00001e70: 6666 5d29 0d0a 2020 2020 2020 2020 2020  ff])..          
-00001e80: 2020 666f 6e74 203d 2049 6d61 6765 466f    font = ImageFo
-00001e90: 6e74 2e74 7275 6574 7970 6528 7469 746c  nt.truetype(titl
-00001ea0: 6546 6f6e 744e 616d 652c 2031 362c 2065  eFontName, 16, e
-00001eb0: 6e63 6f64 696e 673d 2775 7466 2d38 2729  ncoding='utf-8')
-00001ec0: 0d0a 2020 2020 2020 2020 2020 2020 7469  ..            ti
-00001ed0: 746c 6520 3d20 6368 6172 7449 6e66 6f2e  tle = chartInfo.
-00001ee0: 7469 746c 650d 0a20 2020 2020 2020 2020  title..         
-00001ef0: 2020 2069 6620 7365 6c66 2e5f 636f 6c6f     if self._colo
-00001f00: 756d 5769 6474 6828 7469 746c 6529 203e  umWidth(title) >
-00001f10: 2031 353a 0d0a 2020 2020 2020 2020 2020   15:..          
-00001f20: 2020 2020 2020 7469 746c 6520 3d20 7365        title = se
-00001f30: 6c66 2e5f 6368 616e 6765 436f 6c75 6d6e  lf._changeColumn
-00001f40: 5769 6474 6828 7469 746c 652c 2031 3229  Width(title, 12)
-00001f50: 202b 2027 2e2e 2e27 0d0a 2020 2020 2020   + '...'..      
-00001f60: 2020 2020 2020 7465 6d70 4472 6177 2e74        tempDraw.t
-00001f70: 6578 7428 2838 2c20 3829 2c20 7469 746c  ext((8, 8), titl
-00001f80: 652c 2027 7768 6974 6527 2c20 666f 6e74  e, 'white', font
-00001f90: 290d 0a20 2020 2020 2020 2020 2020 2066  )..            f
-00001fa0: 6f6e 7420 3d20 496d 6167 6546 6f6e 742e  ont = ImageFont.
-00001fb0: 7472 7565 7479 7065 2874 6974 6c65 466f  truetype(titleFo
-00001fc0: 6e74 4e61 6d65 2c20 3132 2c20 656e 636f  ntName, 12, enco
-00001fd0: 6469 6e67 3d27 7574 662d 3827 290d 0a0d  ding='utf-8')...
-00001fe0: 0a20 2020 2020 2020 2020 2020 2074 656d  .            tem
-00001ff0: 7044 7261 772e 7465 7874 2828 372c 2032  pDraw.text((7, 2
-00002000: 3829 2c20 6627 7b22 252e 3466 2220 2520  8), f'{"%.4f" % 
-00002010: 6368 6172 7449 6e66 6f2e 6163 6869 6576  chartInfo.achiev
-00002020: 656d 656e 747d 2527 2c20 2777 6869 7465  ement}%', 'white
-00002030: 272c 2066 6f6e 7429 0d0a 2020 2020 2020  ', font)..      
-00002040: 2020 2020 2020 7261 6e6b 496d 6720 3d20        rankImg = 
-00002050: 496d 6167 652e 6f70 656e 2873 656c 662e  Image.open(self.
-00002060: 7069 635f 6469 7220 2b20 6627 5549 5f47  pic_dir + f'UI_G
-00002070: 414d 5f52 616e 6b5f 7b72 616e 6b50 6963  AM_Rank_{rankPic
-00002080: 5b63 6861 7274 496e 666f 2e73 636f 7265  [chartInfo.score
-00002090: 4964 5d7d 2e70 6e67 2729 2e63 6f6e 7665  Id]}.png').conve
-000020a0: 7274 2827 5247 4241 2729 0d0a 2020 2020  rt('RGBA')..    
-000020b0: 2020 2020 2020 2020 7261 6e6b 496d 6720          rankImg 
-000020c0: 3d20 7365 6c66 2e5f 7265 7369 7a65 5069  = self._resizePi
-000020d0: 6328 7261 6e6b 496d 672c 2030 2e33 290d  c(rankImg, 0.3).
-000020e0: 0a20 2020 2020 2020 2020 2020 2074 656d  .            tem
-000020f0: 702e 7061 7374 6528 7261 6e6b 496d 672c  p.paste(rankImg,
-00002100: 2028 3732 2c20 3238 292c 2072 616e 6b49   (72, 28), rankI
-00002110: 6d67 2e73 706c 6974 2829 5b33 5d29 0d0a  mg.split()[3])..
-00002120: 2020 2020 2020 2020 2020 2020 6966 2063              if c
-00002130: 6861 7274 496e 666f 2e63 6f6d 626f 4964  hartInfo.comboId
-00002140: 3a0d 0a20 2020 2020 2020 2020 2020 2020  :..             
-00002150: 2020 2063 6f6d 626f 496d 6720 3d20 496d     comboImg = Im
-00002160: 6167 652e 6f70 656e 2873 656c 662e 7069  age.open(self.pi
-00002170: 635f 6469 7220 2b20 6627 5549 5f4d 5353  c_dir + f'UI_MSS
-00002180: 5f4d 4261 7365 5f49 636f 6e5f 7b63 6f6d  _MBase_Icon_{com
-00002190: 626f 5069 635b 6368 6172 7449 6e66 6f2e  boPic[chartInfo.
-000021a0: 636f 6d62 6f49 645d 7d5f 532e 706e 6727  comboId]}_S.png'
-000021b0: 292e 636f 6e76 6572 7428 2752 4742 4127  ).convert('RGBA'
-000021c0: 290d 0a20 2020 2020 2020 2020 2020 2020  )..             
-000021d0: 2020 2063 6f6d 626f 496d 6720 3d20 7365     comboImg = se
-000021e0: 6c66 2e5f 7265 7369 7a65 5069 6328 636f  lf._resizePic(co
-000021f0: 6d62 6f49 6d67 2c20 302e 3435 290d 0a20  mboImg, 0.45).. 
-00002200: 2020 2020 2020 2020 2020 2020 2020 2074                 t
-00002210: 656d 702e 7061 7374 6528 636f 6d62 6f49  emp.paste(comboI
-00002220: 6d67 2c20 2831 3033 2c20 3237 292c 2063  mg, (103, 27), c
-00002230: 6f6d 626f 496d 672e 7370 6c69 7428 295b  omboImg.split()[
-00002240: 335d 290d 0a20 2020 2020 2020 2020 2020  3])..           
-00002250: 2066 6f6e 7420 3d20 496d 6167 6546 6f6e   font = ImageFon
-00002260: 742e 7472 7565 7479 7065 2853 5441 5449  t.truetype(STATI
-00002270: 4320 2b20 272f 6164 6f62 655f 7369 6d68  C + '/adobe_simh
-00002280: 6569 2e6f 7466 272c 2031 322c 2065 6e63  ei.otf', 12, enc
-00002290: 6f64 696e 673d 2775 7466 2d38 2729 0d0a  oding='utf-8')..
-000022a0: 2020 2020 2020 2020 2020 2020 7465 6d70              temp
-000022b0: 4472 6177 2e74 6578 7428 2838 2c20 3434  Draw.text((8, 44
-000022c0: 292c 2066 2742 6173 653a 207b 6368 6172  ), f'Base: {char
-000022d0: 7449 6e66 6f2e 6473 7d20 2d3e 207b 636f  tInfo.ds} -> {co
-000022e0: 6d70 7574 6552 6128 6368 6172 7449 6e66  mputeRa(chartInf
-000022f0: 6f2e 6473 2c20 6368 6172 7449 6e66 6f2e  o.ds, chartInfo.
-00002300: 6163 6869 6576 656d 656e 7429 7d27 2c20  achievement)}', 
-00002310: 2777 6869 7465 272c 2066 6f6e 7429 0d0a  'white', font)..
-00002320: 2020 2020 2020 2020 2020 2020 666f 6e74              font
-00002330: 203d 2049 6d61 6765 466f 6e74 2e74 7275   = ImageFont.tru
-00002340: 6574 7970 6528 5354 4154 4943 202b 2027  etype(STATIC + '
-00002350: 2f61 646f 6265 5f73 696d 6865 692e 6f74  /adobe_simhei.ot
-00002360: 6627 2c20 3138 2c20 656e 636f 6469 6e67  f', 18, encoding
-00002370: 3d27 7574 662d 3827 290d 0a20 2020 2020  ='utf-8')..     
-00002380: 2020 2020 2020 2074 656d 7044 7261 772e         tempDraw.
-00002390: 7465 7874 2828 382c 2036 3029 2c20 6627  text((8, 60), f'
-000023a0: 237b 6e75 6d20 2b20 317d 272c 2027 7768  #{num + 1}', 'wh
-000023b0: 6974 6527 2c20 666f 6e74 290d 0a0d 0a20  ite', font).... 
-000023c0: 2020 2020 2020 2020 2020 2072 6563 4261             recBa
-000023d0: 7365 203d 2049 6d61 6765 2e6e 6577 2827  se = Image.new('
-000023e0: 5247 4241 272c 2028 6974 656d 572c 2069  RGBA', (itemW, i
-000023f0: 7465 6d48 292c 2027 626c 6163 6b27 290d  temH), 'black').
-00002400: 0a20 2020 2020 2020 2020 2020 2072 6563  .            rec
-00002410: 4261 7365 203d 2072 6563 4261 7365 2e70  Base = recBase.p
-00002420: 6f69 6e74 286c 616d 6264 6120 703a 2069  oint(lambda p: i
-00002430: 6e74 2870 202a 2030 2e38 2929 0d0a 2020  nt(p * 0.8))..  
-00002440: 2020 2020 2020 2020 2020 696d 672e 7061            img.pa
-00002450: 7374 6528 7265 6342 6173 652c 2028 7365  ste(recBase, (se
-00002460: 6c66 2e43 4f4c 4f55 4d53 5f49 4d47 5b6a  lf.COLOUMS_IMG[j
-00002470: 5d20 2b20 352c 2073 656c 662e 524f 5753  ] + 5, self.ROWS
-00002480: 5f49 4d47 5b69 202b 2031 5d20 2b20 3529  _IMG[i + 1] + 5)
-00002490: 290d 0a20 2020 2020 2020 2020 2020 2069  )..            i
-000024a0: 6d67 2e70 6173 7465 2874 656d 702c 2028  mg.paste(temp, (
-000024b0: 7365 6c66 2e43 4f4c 4f55 4d53 5f49 4d47  self.COLOUMS_IMG
-000024c0: 5b6a 5d20 2b20 342c 2073 656c 662e 524f  [j] + 4, self.RO
-000024d0: 5753 5f49 4d47 5b69 202b 2031 5d20 2b20  WS_IMG[i + 1] + 
-000024e0: 3429 290d 0a20 2020 2020 2020 2066 6f72  4))..        for
-000024f0: 206e 756d 2069 6e20 7261 6e67 6528 6c65   num in range(le
-00002500: 6e28 7364 4265 7374 292c 2073 6442 6573  n(sdBest), sdBes
-00002510: 742e 7369 7a65 293a 0d0a 2020 2020 2020  t.size):..      
-00002520: 2020 2020 2020 6920 3d20 6e75 6d20 2f2f        i = num //
-00002530: 2037 0d0a 2020 2020 2020 2020 2020 2020   7..            
-00002540: 6a20 3d20 6e75 6d20 2520 370d 0a20 2020  j = num % 7..   
-00002550: 2020 2020 2020 2020 2074 656d 7020 3d20           temp = 
-00002560: 496d 6167 652e 6f70 656e 2873 656c 662e  Image.open(self.
-00002570: 636f 7665 725f 6469 7220 2b20 6627 3130  cover_dir + f'10
-00002580: 3030 2e70 6e67 2729 2e63 6f6e 7665 7274  00.png').convert
-00002590: 2827 5247 4227 290d 0a20 2020 2020 2020  ('RGB')..       
-000025a0: 2020 2020 2074 656d 7020 3d20 7365 6c66       temp = self
-000025b0: 2e5f 7265 7369 7a65 5069 6328 7465 6d70  ._resizePic(temp
-000025c0: 2c20 6974 656d 5720 2f20 7465 6d70 2e73  , itemW / temp.s
-000025d0: 697a 655b 305d 290d 0a20 2020 2020 2020  ize[0])..       
-000025e0: 2020 2020 2074 656d 7020 3d20 7465 6d70       temp = temp
-000025f0: 2e63 726f 7028 2830 2c20 2874 656d 702e  .crop((0, (temp.
-00002600: 7369 7a65 5b31 5d20 2d20 6974 656d 4829  size[1] - itemH)
-00002610: 202f 2032 2c20 6974 656d 572c 2028 7465   / 2, itemW, (te
-00002620: 6d70 2e73 697a 655b 315d 202b 2069 7465  mp.size[1] + ite
-00002630: 6d48 2920 2f20 3229 290d 0a20 2020 2020  mH) / 2))..     
-00002640: 2020 2020 2020 2074 656d 7020 3d20 7465         temp = te
-00002650: 6d70 2e66 696c 7465 7228 496d 6167 6546  mp.filter(ImageF
-00002660: 696c 7465 722e 4761 7573 7369 616e 426c  ilter.GaussianBl
-00002670: 7572 2831 2929 0d0a 2020 2020 2020 2020  ur(1))..        
-00002680: 2020 2020 696d 672e 7061 7374 6528 7465      img.paste(te
-00002690: 6d70 2c20 2873 656c 662e 434f 4c4f 554d  mp, (self.COLOUM
-000026a0: 535f 494d 475b 6a5d 202b 2034 2c20 7365  S_IMG[j] + 4, se
-000026b0: 6c66 2e52 4f57 535f 494d 475b 6920 2b20  lf.ROWS_IMG[i + 
-000026c0: 315d 202b 2034 2929 0d0a 2020 2020 2020  1] + 4))..      
-000026d0: 2020 666f 7220 6e75 6d20 696e 2072 616e    for num in ran
-000026e0: 6765 2830 2c20 6c65 6e28 6478 4265 7374  ge(0, len(dxBest
-000026f0: 2929 3a0d 0a20 2020 2020 2020 2020 2020  )):..           
-00002700: 2069 203d 206e 756d 202f 2f20 330d 0a20   i = num // 3.. 
-00002710: 2020 2020 2020 2020 2020 206a 203d 206e             j = n
-00002720: 756d 2025 2033 0d0a 2020 2020 2020 2020  um % 3..        
-00002730: 2020 2020 6368 6172 7449 6e66 6f20 3d20      chartInfo = 
-00002740: 6478 4265 7374 5b6e 756d 5d0d 0a20 2020  dxBest[num]..   
-00002750: 2020 2020 2020 2020 2070 6e67 5061 7468           pngPath
-00002760: 203d 2073 656c 662e 636f 7665 725f 6469   = self.cover_di
-00002770: 7220 2b20 6627 7b67 6574 5f63 6f76 6572  r + f'{get_cover
-00002780: 5f6c 656e 345f 6964 2863 6861 7274 496e  _len4_id(chartIn
-00002790: 666f 2e69 644e 756d 297d 2e70 6e67 270d  fo.idNum)}.png'.
-000027a0: 0a20 2020 2020 2020 2020 2020 2069 6620  .            if 
-000027b0: 6e6f 7420 6f73 2e70 6174 682e 6578 6973  not os.path.exis
-000027c0: 7473 2870 6e67 5061 7468 293a 0d0a 2020  ts(pngPath):..  
-000027d0: 2020 2020 2020 2020 2020 2020 2020 706e                pn
-000027e0: 6750 6174 6820 3d20 7365 6c66 2e63 6f76  gPath = self.cov
-000027f0: 6572 5f64 6972 202b 2027 3130 3030 2e70  er_dir + '1000.p
-00002800: 6e67 270d 0a20 2020 2020 2020 2020 2020  ng'..           
-00002810: 2074 656d 7020 3d20 496d 6167 652e 6f70   temp = Image.op
-00002820: 656e 2870 6e67 5061 7468 292e 636f 6e76  en(pngPath).conv
-00002830: 6572 7428 2752 4742 2729 0d0a 2020 2020  ert('RGB')..    
-00002840: 2020 2020 2020 2020 7465 6d70 203d 2073          temp = s
-00002850: 656c 662e 5f72 6573 697a 6550 6963 2874  elf._resizePic(t
-00002860: 656d 702c 2069 7465 6d57 202f 2074 656d  emp, itemW / tem
-00002870: 702e 7369 7a65 5b30 5d29 0d0a 2020 2020  p.size[0])..    
-00002880: 2020 2020 2020 2020 7465 6d70 203d 2074          temp = t
-00002890: 656d 702e 6372 6f70 2828 302c 2028 7465  emp.crop((0, (te
-000028a0: 6d70 2e73 697a 655b 315d 202d 2069 7465  mp.size[1] - ite
-000028b0: 6d48 2920 2f20 322c 2069 7465 6d57 2c20  mH) / 2, itemW, 
-000028c0: 2874 656d 702e 7369 7a65 5b31 5d20 2b20  (temp.size[1] + 
-000028d0: 6974 656d 4829 202f 2032 2929 0d0a 2020  itemH) / 2))..  
-000028e0: 2020 2020 2020 2020 2020 7465 6d70 203d            temp =
-000028f0: 2074 656d 702e 6669 6c74 6572 2849 6d61   temp.filter(Ima
-00002900: 6765 4669 6c74 6572 2e47 6175 7373 6961  geFilter.Gaussia
-00002910: 6e42 6c75 7228 3329 290d 0a20 2020 2020  nBlur(3))..     
-00002920: 2020 2020 2020 2074 656d 7020 3d20 7465         temp = te
-00002930: 6d70 2e70 6f69 6e74 286c 616d 6264 6120  mp.point(lambda 
-00002940: 703a 2069 6e74 2870 202a 2030 2e37 3229  p: int(p * 0.72)
-00002950: 290d 0a0d 0a20 2020 2020 2020 2020 2020  )....           
-00002960: 2074 656d 7044 7261 7720 3d20 496d 6167   tempDraw = Imag
-00002970: 6544 7261 772e 4472 6177 2874 656d 7029  eDraw.Draw(temp)
-00002980: 0d0a 2020 2020 2020 2020 2020 2020 7465  ..            te
-00002990: 6d70 4472 6177 2e70 6f6c 7967 6f6e 286c  mpDraw.polygon(l
-000029a0: 6576 656c 5472 6961 676c 652c 2043 6f6c  evelTriagle, Col
-000029b0: 6f72 5b63 6861 7274 496e 666f 2e64 6966  or[chartInfo.dif
-000029c0: 665d 290d 0a20 2020 2020 2020 2020 2020  f])..           
-000029d0: 2066 6f6e 7420 3d20 496d 6167 6546 6f6e   font = ImageFon
-000029e0: 742e 7472 7565 7479 7065 2874 6974 6c65  t.truetype(title
-000029f0: 466f 6e74 4e61 6d65 2c20 3134 2c20 656e  FontName, 14, en
-00002a00: 636f 6469 6e67 3d27 7574 662d 3827 290d  coding='utf-8').
-00002a10: 0a20 2020 2020 2020 2020 2020 2074 6974  .            tit
-00002a20: 6c65 203d 2063 6861 7274 496e 666f 2e74  le = chartInfo.t
-00002a30: 6974 6c65 0d0a 2020 2020 2020 2020 2020  itle..          
-00002a40: 2020 6966 2073 656c 662e 5f63 6f6c 6f75    if self._colou
-00002a50: 6d57 6964 7468 2874 6974 6c65 2920 3e20  mWidth(title) > 
-00002a60: 3133 3a0d 0a20 2020 2020 2020 2020 2020  13:..           
-00002a70: 2020 2020 2074 6974 6c65 203d 2073 656c       title = sel
-00002a80: 662e 5f63 6861 6e67 6543 6f6c 756d 6e57  f._changeColumnW
-00002a90: 6964 7468 2874 6974 6c65 2c20 3132 2920  idth(title, 12) 
-00002aa0: 2b20 272e 2e2e 270d 0a20 2020 2020 2020  + '...'..       
-00002ab0: 2020 2020 2074 656d 7044 7261 772e 7465       tempDraw.te
-00002ac0: 7874 2828 382c 2038 292c 2074 6974 6c65  xt((8, 8), title
-00002ad0: 2c20 2777 6869 7465 272c 2066 6f6e 7429  , 'white', font)
-00002ae0: 0d0a 2020 2020 2020 2020 2020 2020 666f  ..            fo
-00002af0: 6e74 203d 2049 6d61 6765 466f 6e74 2e74  nt = ImageFont.t
-00002b00: 7275 6574 7970 6528 7469 746c 6546 6f6e  ruetype(titleFon
-00002b10: 744e 616d 652c 2031 322c 2065 6e63 6f64  tName, 12, encod
-00002b20: 696e 673d 2775 7466 2d38 2729 0d0a 0d0a  ing='utf-8')....
-00002b30: 2020 2020 2020 2020 2020 2020 7465 6d70              temp
-00002b40: 4472 6177 2e74 6578 7428 2837 2c20 3238  Draw.text((7, 28
-00002b50: 292c 2066 277b 2225 2e34 6622 2025 2063  ), f'{"%.4f" % c
-00002b60: 6861 7274 496e 666f 2e61 6368 6965 7665  hartInfo.achieve
-00002b70: 6d65 6e74 7d25 272c 2027 7768 6974 6527  ment}%', 'white'
-00002b80: 2c20 666f 6e74 290d 0a20 2020 2020 2020  , font)..       
-00002b90: 2020 2020 2072 616e 6b49 6d67 203d 2049       rankImg = I
-00002ba0: 6d61 6765 2e6f 7065 6e28 7365 6c66 2e70  mage.open(self.p
-00002bb0: 6963 5f64 6972 202b 2066 2755 495f 4741  ic_dir + f'UI_GA
-00002bc0: 4d5f 5261 6e6b 5f7b 7261 6e6b 5069 635b  M_Rank_{rankPic[
-00002bd0: 6368 6172 7449 6e66 6f2e 7363 6f72 6549  chartInfo.scoreI
-00002be0: 645d 7d2e 706e 6727 292e 636f 6e76 6572  d]}.png').conver
-00002bf0: 7428 2752 4742 4127 290d 0a20 2020 2020  t('RGBA')..     
-00002c00: 2020 2020 2020 2072 616e 6b49 6d67 203d         rankImg =
-00002c10: 2073 656c 662e 5f72 6573 697a 6550 6963   self._resizePic
-00002c20: 2872 616e 6b49 6d67 2c20 302e 3329 0d0a  (rankImg, 0.3)..
-00002c30: 2020 2020 2020 2020 2020 2020 7465 6d70              temp
-00002c40: 2e70 6173 7465 2872 616e 6b49 6d67 2c20  .paste(rankImg, 
-00002c50: 2837 322c 2032 3829 2c20 7261 6e6b 496d  (72, 28), rankIm
-00002c60: 672e 7370 6c69 7428 295b 335d 290d 0a20  g.split()[3]).. 
-00002c70: 2020 2020 2020 2020 2020 2069 6620 6368             if ch
-00002c80: 6172 7449 6e66 6f2e 636f 6d62 6f49 643a  artInfo.comboId:
-00002c90: 0d0a 2020 2020 2020 2020 2020 2020 2020  ..              
-00002ca0: 2020 636f 6d62 6f49 6d67 203d 2049 6d61    comboImg = Ima
-00002cb0: 6765 2e6f 7065 6e28 7365 6c66 2e70 6963  ge.open(self.pic
-00002cc0: 5f64 6972 202b 2066 2755 495f 4d53 535f  _dir + f'UI_MSS_
-00002cd0: 4d42 6173 655f 4963 6f6e 5f7b 636f 6d62  MBase_Icon_{comb
-00002ce0: 6f50 6963 5b63 6861 7274 496e 666f 2e63  oPic[chartInfo.c
-00002cf0: 6f6d 626f 4964 5d7d 5f53 2e70 6e67 2729  omboId]}_S.png')
-00002d00: 2e63 6f6e 7665 7274 280d 0a20 2020 2020  .convert(..     
-00002d10: 2020 2020 2020 2020 2020 2020 2020 2027                 '
-00002d20: 5247 4241 2729 0d0a 2020 2020 2020 2020  RGBA')..        
-00002d30: 2020 2020 2020 2020 636f 6d62 6f49 6d67          comboImg
-00002d40: 203d 2073 656c 662e 5f72 6573 697a 6550   = self._resizeP
-00002d50: 6963 2863 6f6d 626f 496d 672c 2030 2e34  ic(comboImg, 0.4
-00002d60: 3529 0d0a 2020 2020 2020 2020 2020 2020  5)..            
-00002d70: 2020 2020 7465 6d70 2e70 6173 7465 2863      temp.paste(c
-00002d80: 6f6d 626f 496d 672c 2028 3130 332c 2032  omboImg, (103, 2
-00002d90: 3729 2c20 636f 6d62 6f49 6d67 2e73 706c  7), comboImg.spl
-00002da0: 6974 2829 5b33 5d29 0d0a 2020 2020 2020  it()[3])..      
-00002db0: 2020 2020 2020 666f 6e74 203d 2049 6d61        font = Ima
-00002dc0: 6765 466f 6e74 2e74 7275 6574 7970 6528  geFont.truetype(
-00002dd0: 5354 4154 4943 202b 2027 2f61 646f 6265  STATIC + '/adobe
-00002de0: 5f73 696d 6865 692e 6f74 6627 2c20 3132  _simhei.otf', 12
-00002df0: 2c20 656e 636f 6469 6e67 3d27 7574 662d  , encoding='utf-
-00002e00: 3827 290d 0a20 2020 2020 2020 2020 2020  8')..           
-00002e10: 2074 656d 7044 7261 772e 7465 7874 2828   tempDraw.text((
-00002e20: 382c 2034 3429 2c20 6627 4261 7365 3a20  8, 44), f'Base: 
-00002e30: 7b63 6861 7274 496e 666f 2e64 737d 202d  {chartInfo.ds} -
-00002e40: 3e20 7b63 6861 7274 496e 666f 2e72 617d  > {chartInfo.ra}
-00002e50: 272c 2027 7768 6974 6527 2c20 666f 6e74  ', 'white', font
-00002e60: 290d 0a20 2020 2020 2020 2020 2020 2066  )..            f
-00002e70: 6f6e 7420 3d20 496d 6167 6546 6f6e 742e  ont = ImageFont.
-00002e80: 7472 7565 7479 7065 2853 5441 5449 4320  truetype(STATIC 
-00002e90: 2b20 272f 6164 6f62 655f 7369 6d68 6569  + '/adobe_simhei
-00002ea0: 2e6f 7466 272c 2031 382c 2065 6e63 6f64  .otf', 18, encod
-00002eb0: 696e 673d 2775 7466 2d38 2729 0d0a 2020  ing='utf-8')..  
-00002ec0: 2020 2020 2020 2020 2020 7465 6d70 4472            tempDr
-00002ed0: 6177 2e74 6578 7428 2838 2c20 3630 292c  aw.text((8, 60),
-00002ee0: 2066 2723 7b6e 756d 202b 2031 7d27 2c20   f'#{num + 1}', 
-00002ef0: 2777 6869 7465 272c 2066 6f6e 7429 0d0a  'white', font)..
-00002f00: 0d0a 2020 2020 2020 2020 2020 2020 7265  ..            re
-00002f10: 6342 6173 6520 3d20 496d 6167 652e 6e65  cBase = Image.ne
-00002f20: 7728 2752 4742 4127 2c20 2869 7465 6d57  w('RGBA', (itemW
-00002f30: 2c20 6974 656d 4829 2c20 2762 6c61 636b  , itemH), 'black
-00002f40: 2729 0d0a 2020 2020 2020 2020 2020 2020  ')..            
-00002f50: 7265 6342 6173 6520 3d20 7265 6342 6173  recBase = recBas
-00002f60: 652e 706f 696e 7428 6c61 6d62 6461 2070  e.point(lambda p
-00002f70: 3a20 696e 7428 7020 2a20 302e 3829 290d  : int(p * 0.8)).
-00002f80: 0a20 2020 2020 2020 2020 2020 2069 6d67  .            img
-00002f90: 2e70 6173 7465 2872 6563 4261 7365 2c20  .paste(recBase, 
-00002fa0: 2873 656c 662e 434f 4c4f 554d 535f 494d  (self.COLOUMS_IM
-00002fb0: 475b 6a20 2b20 385d 202b 2035 2c20 7365  G[j + 8] + 5, se
-00002fc0: 6c66 2e52 4f57 535f 494d 475b 6920 2b20  lf.ROWS_IMG[i + 
-00002fd0: 315d 202b 2035 2929 0d0a 2020 2020 2020  1] + 5))..      
-00002fe0: 2020 2020 2020 696d 672e 7061 7374 6528        img.paste(
-00002ff0: 7465 6d70 2c20 2873 656c 662e 434f 4c4f  temp, (self.COLO
-00003000: 554d 535f 494d 475b 6a20 2b20 385d 202b  UMS_IMG[j + 8] +
-00003010: 2034 2c20 7365 6c66 2e52 4f57 535f 494d   4, self.ROWS_IM
-00003020: 475b 6920 2b20 315d 202b 2034 2929 0d0a  G[i + 1] + 4))..
-00003030: 2020 2020 2020 2020 666f 7220 6e75 6d20          for num 
-00003040: 696e 2072 616e 6765 286c 656e 2864 7842  in range(len(dxB
-00003050: 6573 7429 2c20 6478 4265 7374 2e73 697a  est), dxBest.siz
-00003060: 6529 3a0d 0a20 2020 2020 2020 2020 2020  e):..           
-00003070: 2069 203d 206e 756d 202f 2f20 330d 0a20   i = num // 3.. 
-00003080: 2020 2020 2020 2020 2020 206a 203d 206e             j = n
-00003090: 756d 2025 2033 0d0a 2020 2020 2020 2020  um % 3..        
-000030a0: 2020 2020 7465 6d70 203d 2049 6d61 6765      temp = Image
-000030b0: 2e6f 7065 6e28 7365 6c66 2e63 6f76 6572  .open(self.cover
-000030c0: 5f64 6972 202b 2066 2731 3030 302e 706e  _dir + f'1000.pn
-000030d0: 6727 292e 636f 6e76 6572 7428 2752 4742  g').convert('RGB
-000030e0: 2729 0d0a 2020 2020 2020 2020 2020 2020  ')..            
-000030f0: 7465 6d70 203d 2073 656c 662e 5f72 6573  temp = self._res
-00003100: 697a 6550 6963 2874 656d 702c 2069 7465  izePic(temp, ite
-00003110: 6d57 202f 2074 656d 702e 7369 7a65 5b30  mW / temp.size[0
-00003120: 5d29 0d0a 2020 2020 2020 2020 2020 2020  ])..            
-00003130: 7465 6d70 203d 2074 656d 702e 6372 6f70  temp = temp.crop
-00003140: 2828 302c 2028 7465 6d70 2e73 697a 655b  ((0, (temp.size[
-00003150: 315d 202d 2069 7465 6d48 2920 2f20 322c  1] - itemH) / 2,
-00003160: 2069 7465 6d57 2c20 2874 656d 702e 7369   itemW, (temp.si
-00003170: 7a65 5b31 5d20 2b20 6974 656d 4829 202f  ze[1] + itemH) /
-00003180: 2032 2929 0d0a 2020 2020 2020 2020 2020   2))..          
-00003190: 2020 7465 6d70 203d 2074 656d 702e 6669    temp = temp.fi
-000031a0: 6c74 6572 2849 6d61 6765 4669 6c74 6572  lter(ImageFilter
-000031b0: 2e47 6175 7373 6961 6e42 6c75 7228 3129  .GaussianBlur(1)
-000031c0: 290d 0a20 2020 2020 2020 2020 2020 2069  )..            i
-000031d0: 6d67 2e70 6173 7465 2874 656d 702c 2028  mg.paste(temp, (
-000031e0: 7365 6c66 2e43 4f4c 4f55 4d53 5f49 4d47  self.COLOUMS_IMG
-000031f0: 5b6a 202b 2038 5d20 2b20 342c 2073 656c  [j + 8] + 4, sel
-00003200: 662e 524f 5753 5f49 4d47 5b69 202b 2031  f.ROWS_IMG[i + 1
-00003210: 5d20 2b20 3429 290d 0a0d 0a20 2020 2064  ] + 4))....    d
-00003220: 6566 2064 7261 7728 7365 6c66 293a 0d0a  ef draw(self):..
-00003230: 2020 2020 2020 2020 7370 6c61 7368 4c6f          splashLo
-00003240: 676f 203d 2049 6d61 6765 2e6f 7065 6e28  go = Image.open(
-00003250: 7365 6c66 2e70 6963 5f64 6972 202b 2027  self.pic_dir + '
-00003260: 5549 5f43 4d4e 5f54 6162 5469 746c 655f  UI_CMN_TabTitle_
-00003270: 4d61 696d 6169 5469 746c 655f 5665 7232  MaimaiTitle_Ver2
-00003280: 3134 2e70 6e67 2729 2e63 6f6e 7665 7274  14.png').convert
-00003290: 2827 5247 4241 2729 0d0a 2020 2020 2020  ('RGBA')..      
-000032a0: 2020 7370 6c61 7368 4c6f 676f 203d 2073    splashLogo = s
-000032b0: 656c 662e 5f72 6573 697a 6550 6963 2873  elf._resizePic(s
-000032c0: 706c 6173 684c 6f67 6f2c 2030 2e36 3529  plashLogo, 0.65)
-000032d0: 0d0a 2020 2020 2020 2020 7365 6c66 2e69  ..        self.i
-000032e0: 6d67 2e70 6173 7465 2873 706c 6173 684c  mg.paste(splashL
-000032f0: 6f67 6f2c 2028 3130 2c20 3130 292c 206d  ogo, (10, 10), m
-00003300: 6173 6b3d 7370 6c61 7368 4c6f 676f 2e73  ask=splashLogo.s
-00003310: 706c 6974 2829 5b33 5d29 0d0a 0d0a 2020  plit()[3])....  
-00003320: 2020 2020 2020 7261 7469 6e67 4261 7365        ratingBase
-00003330: 496d 6720 3d20 496d 6167 652e 6f70 656e  Img = Image.open
-00003340: 2873 656c 662e 7069 635f 6469 7220 2b20  (self.pic_dir + 
-00003350: 7365 6c66 2e5f 6669 6e64 5261 5069 6328  self._findRaPic(
-00003360: 2929 2e63 6f6e 7665 7274 2827 5247 4241  )).convert('RGBA
-00003370: 2729 0d0a 2020 2020 2020 2020 7261 7469  ')..        rati
-00003380: 6e67 4261 7365 496d 6720 3d20 7365 6c66  ngBaseImg = self
-00003390: 2e5f 6472 6177 5261 7469 6e67 2872 6174  ._drawRating(rat
-000033a0: 696e 6742 6173 6549 6d67 290d 0a20 2020  ingBaseImg)..   
-000033b0: 2020 2020 2072 6174 696e 6742 6173 6549       ratingBaseI
-000033c0: 6d67 203d 2073 656c 662e 5f72 6573 697a  mg = self._resiz
-000033d0: 6550 6963 2872 6174 696e 6742 6173 6549  ePic(ratingBaseI
-000033e0: 6d67 2c20 302e 3835 290d 0a20 2020 2020  mg, 0.85)..     
-000033f0: 2020 2073 656c 662e 696d 672e 7061 7374     self.img.past
-00003400: 6528 7261 7469 6e67 4261 7365 496d 672c  e(ratingBaseImg,
-00003410: 2028 3234 302c 2038 292c 206d 6173 6b3d   (240, 8), mask=
-00003420: 7261 7469 6e67 4261 7365 496d 672e 7370  ratingBaseImg.sp
-00003430: 6c69 7428 295b 335d 290d 0a0d 0a20 2020  lit()[3])....   
-00003440: 2020 2020 206e 616d 6550 6c61 7465 496d       namePlateIm
-00003450: 6720 3d20 496d 6167 652e 6f70 656e 2873  g = Image.open(s
-00003460: 656c 662e 7069 635f 6469 7220 2b20 2755  elf.pic_dir + 'U
-00003470: 495f 5453 545f 506c 6174 654d 6173 6b2e  I_TST_PlateMask.
-00003480: 706e 6727 292e 636f 6e76 6572 7428 2752  png').convert('R
-00003490: 4742 4127 290d 0a20 2020 2020 2020 206e  GBA')..        n
-000034a0: 616d 6550 6c61 7465 496d 6720 3d20 6e61  amePlateImg = na
-000034b0: 6d65 506c 6174 6549 6d67 2e72 6573 697a  mePlateImg.resiz
-000034c0: 6528 2832 3835 2c20 3430 2929 0d0a 2020  e((285, 40))..  
-000034d0: 2020 2020 2020 6e61 6d65 506c 6174 6544        namePlateD
-000034e0: 7261 7720 3d20 496d 6167 6544 7261 772e  raw = ImageDraw.
-000034f0: 4472 6177 286e 616d 6550 6c61 7465 496d  Draw(namePlateIm
-00003500: 6729 0d0a 2020 2020 2020 2020 666f 6e74  g)..        font
-00003510: 3120 3d20 496d 6167 6546 6f6e 742e 7472  1 = ImageFont.tr
-00003520: 7565 7479 7065 2853 5441 5449 4320 2b20  uetype(STATIC + 
-00003530: 272f 6d73 7968 2e74 7463 272c 2032 382c  '/msyh.ttc', 28,
-00003540: 2065 6e63 6f64 696e 673d 2775 6e69 6327   encoding='unic'
-00003550: 290d 0a20 2020 2020 2020 206e 616d 6550  )..        nameP
-00003560: 6c61 7465 4472 6177 2e74 6578 7428 2831  lateDraw.text((1
-00003570: 322c 2034 292c 2027 2027 2e6a 6f69 6e28  2, 4), ' '.join(
-00003580: 6c69 7374 2873 656c 662e 7573 6572 4e61  list(self.userNa
-00003590: 6d65 2929 2c20 2762 6c61 636b 272c 2066  me)), 'black', f
-000035a0: 6f6e 7431 290d 0a20 2020 2020 2020 206e  ont1)..        n
-000035b0: 616d 6544 7849 6d67 203d 2049 6d61 6765  ameDxImg = Image
-000035c0: 2e6f 7065 6e28 7365 6c66 2e70 6963 5f64  .open(self.pic_d
-000035d0: 6972 202b 2027 5549 5f43 4d4e 5f4e 616d  ir + 'UI_CMN_Nam
-000035e0: 655f 4458 2e70 6e67 2729 2e63 6f6e 7665  e_DX.png').conve
-000035f0: 7274 2827 5247 4241 2729 0d0a 2020 2020  rt('RGBA')..    
-00003600: 2020 2020 6e61 6d65 4478 496d 6720 3d20      nameDxImg = 
-00003610: 7365 6c66 2e5f 7265 7369 7a65 5069 6328  self._resizePic(
-00003620: 6e61 6d65 4478 496d 672c 2030 2e39 290d  nameDxImg, 0.9).
-00003630: 0a20 2020 2020 2020 206e 616d 6550 6c61  .        namePla
-00003640: 7465 496d 672e 7061 7374 6528 6e61 6d65  teImg.paste(name
-00003650: 4478 496d 672c 2028 3233 302c 2034 292c  DxImg, (230, 4),
-00003660: 206d 6173 6b3d 6e61 6d65 4478 496d 672e   mask=nameDxImg.
-00003670: 7370 6c69 7428 295b 335d 290d 0a20 2020  split()[3])..   
-00003680: 2020 2020 2073 656c 662e 696d 672e 7061       self.img.pa
-00003690: 7374 6528 6e61 6d65 506c 6174 6549 6d67  ste(namePlateImg
-000036a0: 2c20 2832 3430 2c20 3430 292c 206d 6173  , (240, 40), mas
-000036b0: 6b3d 6e61 6d65 506c 6174 6549 6d67 2e73  k=namePlateImg.s
-000036c0: 706c 6974 2829 5b33 5d29 0d0a 0d0a 2020  plit()[3])....  
-000036d0: 2020 2020 2020 7368 6f75 676f 7549 6d67        shougouImg
-000036e0: 203d 2049 6d61 6765 2e6f 7065 6e28 7365   = Image.open(se
-000036f0: 6c66 2e70 6963 5f64 6972 202b 2027 5549  lf.pic_dir + 'UI
-00003700: 5f43 4d4e 5f53 686f 7567 6f75 5f52 6169  _CMN_Shougou_Rai
-00003710: 6e62 6f77 2e70 6e67 2729 2e63 6f6e 7665  nbow.png').conve
-00003720: 7274 2827 5247 4241 2729 0d0a 2020 2020  rt('RGBA')..    
-00003730: 2020 2020 7368 6f75 676f 7544 7261 7720      shougouDraw 
-00003740: 3d20 496d 6167 6544 7261 772e 4472 6177  = ImageDraw.Draw
-00003750: 2873 686f 7567 6f75 496d 6729 0d0a 2020  (shougouImg)..  
-00003760: 2020 2020 2020 666f 6e74 3220 3d20 496d        font2 = Im
-00003770: 6167 6546 6f6e 742e 7472 7565 7479 7065  ageFont.truetype
-00003780: 2853 5441 5449 4320 2b20 272f 6164 6f62  (STATIC + '/adob
-00003790: 655f 7369 6d68 6569 2e6f 7466 272c 2031  e_simhei.otf', 1
-000037a0: 342c 2065 6e63 6f64 696e 673d 2775 7466  4, encoding='utf
-000037b0: 2d38 2729 0d0a 2020 2020 2020 2020 706c  -8')..        pl
-000037c0: 6179 436f 756e 7449 6e66 6f20 3d20 6627  ayCountInfo = f'
-000037d0: 5344 3a20 7b73 656c 662e 7364 5261 7469  SD: {self.sdRati
-000037e0: 6e67 7d20 2b20 4458 3a20 7b73 656c 662e  ng} + DX: {self.
-000037f0: 6478 5261 7469 6e67 7d20 3d20 7b73 656c  dxRating} = {sel
-00003800: 662e 706c 6179 6572 5261 7469 6e67 7d27  f.playerRating}'
-00003810: 0d0a 2020 2020 2020 2020 7368 6f75 676f  ..        shougo
-00003820: 7549 6d67 572c 2073 686f 7567 6f75 496d  uImgW, shougouIm
-00003830: 6748 203d 2073 686f 7567 6f75 496d 672e  gH = shougouImg.
-00003840: 7369 7a65 0d0a 2020 2020 2020 2020 706c  size..        pl
-00003850: 6179 436f 756e 7449 6e66 6f57 2c20 706c  ayCountInfoW, pl
-00003860: 6179 436f 756e 7449 6e66 6f48 203d 2073  ayCountInfoH = s
-00003870: 686f 7567 6f75 4472 6177 2e74 6578 7473  hougouDraw.texts
-00003880: 697a 6528 706c 6179 436f 756e 7449 6e66  ize(playCountInf
-00003890: 6f2c 2066 6f6e 7432 290d 0a20 2020 2020  o, font2)..     
-000038a0: 2020 2074 6578 7450 6f73 203d 2028 2873     textPos = ((s
-000038b0: 686f 7567 6f75 496d 6757 202d 2070 6c61  hougouImgW - pla
-000038c0: 7943 6f75 6e74 496e 666f 5720 2d20 666f  yCountInfoW - fo
-000038d0: 6e74 322e 6765 746f 6666 7365 7428 706c  nt2.getoffset(pl
-000038e0: 6179 436f 756e 7449 6e66 6f29 5b30 5d29  ayCountInfo)[0])
-000038f0: 202f 2032 2c20 3529 0d0a 2020 2020 2020   / 2, 5)..      
-00003900: 2020 7368 6f75 676f 7544 7261 772e 7465    shougouDraw.te
-00003910: 7874 2828 7465 7874 506f 735b 305d 202d  xt((textPos[0] -
-00003920: 2031 2c20 7465 7874 506f 735b 315d 292c   1, textPos[1]),
-00003930: 2070 6c61 7943 6f75 6e74 496e 666f 2c20   playCountInfo, 
-00003940: 2762 6c61 636b 272c 2066 6f6e 7432 290d  'black', font2).
-00003950: 0a20 2020 2020 2020 2073 686f 7567 6f75  .        shougou
-00003960: 4472 6177 2e74 6578 7428 2874 6578 7450  Draw.text((textP
-00003970: 6f73 5b30 5d20 2b20 312c 2074 6578 7450  os[0] + 1, textP
-00003980: 6f73 5b31 5d29 2c20 706c 6179 436f 756e  os[1]), playCoun
-00003990: 7449 6e66 6f2c 2027 626c 6163 6b27 2c20  tInfo, 'black', 
-000039a0: 666f 6e74 3229 0d0a 2020 2020 2020 2020  font2)..        
-000039b0: 7368 6f75 676f 7544 7261 772e 7465 7874  shougouDraw.text
-000039c0: 2828 7465 7874 506f 735b 305d 2c20 7465  ((textPos[0], te
-000039d0: 7874 506f 735b 315d 202d 2031 292c 2070  xtPos[1] - 1), p
-000039e0: 6c61 7943 6f75 6e74 496e 666f 2c20 2762  layCountInfo, 'b
-000039f0: 6c61 636b 272c 2066 6f6e 7432 290d 0a20  lack', font2).. 
-00003a00: 2020 2020 2020 2073 686f 7567 6f75 4472         shougouDr
-00003a10: 6177 2e74 6578 7428 2874 6578 7450 6f73  aw.text((textPos
-00003a20: 5b30 5d2c 2074 6578 7450 6f73 5b31 5d20  [0], textPos[1] 
-00003a30: 2b20 3129 2c20 706c 6179 436f 756e 7449  + 1), playCountI
-00003a40: 6e66 6f2c 2027 626c 6163 6b27 2c20 666f  nfo, 'black', fo
-00003a50: 6e74 3229 0d0a 2020 2020 2020 2020 7368  nt2)..        sh
-00003a60: 6f75 676f 7544 7261 772e 7465 7874 2828  ougouDraw.text((
-00003a70: 7465 7874 506f 735b 305d 202d 2031 2c20  textPos[0] - 1, 
-00003a80: 7465 7874 506f 735b 315d 202d 2031 292c  textPos[1] - 1),
-00003a90: 2070 6c61 7943 6f75 6e74 496e 666f 2c20   playCountInfo, 
-00003aa0: 2762 6c61 636b 272c 2066 6f6e 7432 290d  'black', font2).
-00003ab0: 0a20 2020 2020 2020 2073 686f 7567 6f75  .        shougou
-00003ac0: 4472 6177 2e74 6578 7428 2874 6578 7450  Draw.text((textP
-00003ad0: 6f73 5b30 5d20 2b20 312c 2074 6578 7450  os[0] + 1, textP
-00003ae0: 6f73 5b31 5d20 2d20 3129 2c20 706c 6179  os[1] - 1), play
-00003af0: 436f 756e 7449 6e66 6f2c 2027 626c 6163  CountInfo, 'blac
-00003b00: 6b27 2c20 666f 6e74 3229 0d0a 2020 2020  k', font2)..    
-00003b10: 2020 2020 7368 6f75 676f 7544 7261 772e      shougouDraw.
-00003b20: 7465 7874 2828 7465 7874 506f 735b 305d  text((textPos[0]
-00003b30: 202d 2031 2c20 7465 7874 506f 735b 315d   - 1, textPos[1]
-00003b40: 202b 2031 292c 2070 6c61 7943 6f75 6e74   + 1), playCount
-00003b50: 496e 666f 2c20 2762 6c61 636b 272c 2066  Info, 'black', f
-00003b60: 6f6e 7432 290d 0a20 2020 2020 2020 2073  ont2)..        s
-00003b70: 686f 7567 6f75 4472 6177 2e74 6578 7428  hougouDraw.text(
-00003b80: 2874 6578 7450 6f73 5b30 5d20 2b20 312c  (textPos[0] + 1,
-00003b90: 2074 6578 7450 6f73 5b31 5d20 2b20 3129   textPos[1] + 1)
-00003ba0: 2c20 706c 6179 436f 756e 7449 6e66 6f2c  , playCountInfo,
-00003bb0: 2027 626c 6163 6b27 2c20 666f 6e74 3229   'black', font2)
-00003bc0: 0d0a 2020 2020 2020 2020 7368 6f75 676f  ..        shougo
-00003bd0: 7544 7261 772e 7465 7874 2874 6578 7450  uDraw.text(textP
-00003be0: 6f73 2c20 706c 6179 436f 756e 7449 6e66  os, playCountInf
-00003bf0: 6f2c 2027 7768 6974 6527 2c20 666f 6e74  o, 'white', font
-00003c00: 3229 0d0a 2020 2020 2020 2020 7368 6f75  2)..        shou
-00003c10: 676f 7549 6d67 203d 2073 656c 662e 5f72  gouImg = self._r
-00003c20: 6573 697a 6550 6963 2873 686f 7567 6f75  esizePic(shougou
-00003c30: 496d 672c 2031 2e30 3529 0d0a 2020 2020  Img, 1.05)..    
-00003c40: 2020 2020 7365 6c66 2e69 6d67 2e70 6173      self.img.pas
-00003c50: 7465 2873 686f 7567 6f75 496d 672c 2028  te(shougouImg, (
-00003c60: 3234 302c 2038 3329 2c20 6d61 736b 3d73  240, 83), mask=s
-00003c70: 686f 7567 6f75 496d 672e 7370 6c69 7428  hougouImg.split(
-00003c80: 295b 335d 290d 0a0d 0a20 2020 2020 2020  )[3])....       
-00003c90: 2073 656c 662e 5f64 7261 7742 6573 744c   self._drawBestL
-00003ca0: 6973 7428 7365 6c66 2e69 6d67 2c20 7365  ist(self.img, se
-00003cb0: 6c66 2e73 6442 6573 742c 2073 656c 662e  lf.sdBest, self.
-00003cc0: 6478 4265 7374 290d 0a0d 0a20 2020 2020  dxBest)....     
-00003cd0: 2020 2061 7574 686f 7242 6f61 7264 496d     authorBoardIm
-00003ce0: 6720 3d20 496d 6167 652e 6f70 656e 2873  g = Image.open(s
-00003cf0: 656c 662e 7069 635f 6469 7220 2b20 2755  elf.pic_dir + 'U
-00003d00: 495f 434d 4e5f 4d69 6e69 4469 616c 6f67  I_CMN_MiniDialog
-00003d10: 5f30 312e 706e 6727 292e 636f 6e76 6572  _01.png').conver
-00003d20: 7428 2752 4742 4127 290d 0a20 2020 2020  t('RGBA')..     
-00003d30: 2020 2061 7574 686f 7242 6f61 7264 496d     authorBoardIm
-00003d40: 6720 3d20 7365 6c66 2e5f 7265 7369 7a65  g = self._resize
-00003d50: 5069 6328 6175 7468 6f72 426f 6172 6449  Pic(authorBoardI
-00003d60: 6d67 2c20 302e 3335 290d 0a20 2020 2020  mg, 0.35)..     
-00003d70: 2020 2061 7574 686f 7242 6f61 7264 4472     authorBoardDr
-00003d80: 6177 203d 2049 6d61 6765 4472 6177 2e44  aw = ImageDraw.D
-00003d90: 7261 7728 6175 7468 6f72 426f 6172 6449  raw(authorBoardI
-00003da0: 6d67 290d 0a20 2020 2020 2020 2061 7574  mg)..        aut
-00003db0: 686f 7242 6f61 7264 4472 6177 2e74 6578  horBoardDraw.tex
-00003dc0: 7428 2833 312c 2032 3829 2c20 2720 2020  t((31, 28), '   
-00003dd0: 4765 6e65 7261 7465 6420 4279 5c6e 5879  Generated By\nXy
-00003de0: 6242 6f74 2026 2043 6869 7975 6b69 272c  bBot & Chiyuki',
-00003df0: 2027 626c 6163 6b27 2c20 666f 6e74 3229   'black', font2)
-00003e00: 0d0a 2020 2020 2020 2020 7365 6c66 2e69  ..        self.i
-00003e10: 6d67 2e70 6173 7465 2861 7574 686f 7242  mg.paste(authorB
-00003e20: 6f61 7264 496d 672c 2028 3132 3234 2c20  oardImg, (1224, 
-00003e30: 3139 292c 206d 6173 6b3d 6175 7468 6f72  19), mask=author
-00003e40: 426f 6172 6449 6d67 2e73 706c 6974 2829  BoardImg.split()
-00003e50: 5b33 5d29 0d0a 0d0a 2020 2020 2020 2020  [3])....        
-00003e60: 6478 496d 6720 3d20 496d 6167 652e 6f70  dxImg = Image.op
-00003e70: 656e 2873 656c 662e 7069 635f 6469 7220  en(self.pic_dir 
-00003e80: 2b20 2755 495f 5253 4c5f 4d42 6173 655f  + 'UI_RSL_MBase_
-00003e90: 5061 7274 735f 3031 2e70 6e67 2729 2e63  Parts_01.png').c
-00003ea0: 6f6e 7665 7274 2827 5247 4241 2729 0d0a  onvert('RGBA')..
-00003eb0: 2020 2020 2020 2020 7365 6c66 2e69 6d67          self.img
-00003ec0: 2e70 6173 7465 2864 7849 6d67 2c20 2839  .paste(dxImg, (9
-00003ed0: 3838 2c20 3635 292c 206d 6173 6b3d 6478  88, 65), mask=dx
-00003ee0: 496d 672e 7370 6c69 7428 295b 335d 290d  Img.split()[3]).
-00003ef0: 0a20 2020 2020 2020 2073 6449 6d67 203d  .        sdImg =
-00003f00: 2049 6d61 6765 2e6f 7065 6e28 7365 6c66   Image.open(self
-00003f10: 2e70 6963 5f64 6972 202b 2027 5549 5f52  .pic_dir + 'UI_R
-00003f20: 534c 5f4d 4261 7365 5f50 6172 7473 5f30  SL_MBase_Parts_0
-00003f30: 322e 706e 6727 292e 636f 6e76 6572 7428  2.png').convert(
-00003f40: 2752 4742 4127 290d 0a20 2020 2020 2020  'RGBA')..       
-00003f50: 2073 656c 662e 696d 672e 7061 7374 6528   self.img.paste(
-00003f60: 7364 496d 672c 2028 3836 352c 2036 3529  sdImg, (865, 65)
-00003f70: 2c20 6d61 736b 3d73 6449 6d67 2e73 706c  , mask=sdImg.spl
-00003f80: 6974 2829 5b33 5d29 0d0a 0d0a 2020 2020  it()[3])....    
-00003f90: 2020 2020 2320 7365 6c66 2e69 6d67 2e73      # self.img.s
-00003fa0: 686f 7728 290d 0a0d 0a20 2020 2064 6566  how()....    def
-00003fb0: 2067 6574 4469 7228 7365 6c66 293a 0d0a   getDir(self):..
-00003fc0: 2020 2020 2020 2020 7265 7475 726e 2073          return s
-00003fd0: 656c 662e 696d 670d 0a0d 0a0d 0a64 6566  elf.img......def
-00003fe0: 2063 6f6d 7075 7465 5261 2864 733a 2066   computeRa(ds: f
-00003ff0: 6c6f 6174 2c20 6163 6869 6576 656d 656e  loat, achievemen
-00004000: 743a 2066 6c6f 6174 2920 2d3e 2069 6e74  t: float) -> int
-00004010: 3a0d 0a20 2020 2062 6173 6552 6120 3d20  :..    baseRa = 
-00004020: 3232 2e34 200d 0a20 2020 2069 6620 6163  22.4 ..    if ac
-00004030: 6869 6576 656d 656e 7420 3c20 3530 3a0d  hievement < 50:.
-00004040: 0a20 2020 2020 2020 2062 6173 6552 6120  .        baseRa 
-00004050: 3d20 372e 300d 0a20 2020 2065 6c69 6620  = 7.0..    elif 
-00004060: 6163 6869 6576 656d 656e 7420 3c20 3630  achievement < 60
-00004070: 3a0d 0a20 2020 2020 2020 2062 6173 6552  :..        baseR
-00004080: 6120 3d20 382e 3020 0d0a 2020 2020 656c  a = 8.0 ..    el
-00004090: 6966 2061 6368 6965 7665 6d65 6e74 203c  if achievement <
-000040a0: 2037 303a 0d0a 2020 2020 2020 2020 6261   70:..        ba
-000040b0: 7365 5261 203d 2039 2e36 200d 0a20 2020  seRa = 9.6 ..   
-000040c0: 2065 6c69 6620 6163 6869 6576 656d 656e   elif achievemen
-000040d0: 7420 3c20 3735 3a0d 0a20 2020 2020 2020  t < 75:..       
-000040e0: 2062 6173 6552 6120 3d20 3131 2e32 200d   baseRa = 11.2 .
-000040f0: 0a20 2020 2065 6c69 6620 6163 6869 6576  .    elif achiev
-00004100: 656d 656e 7420 3c20 3830 3a0d 0a20 2020  ement < 80:..   
-00004110: 2020 2020 2062 6173 6552 6120 3d20 3132       baseRa = 12
-00004120: 2e30 200d 0a20 2020 2065 6c69 6620 6163  .0 ..    elif ac
-00004130: 6869 6576 656d 656e 7420 3c20 3930 3a0d  hievement < 90:.
-00004140: 0a20 2020 2020 2020 2062 6173 6552 6120  .        baseRa 
-00004150: 3d20 3133 2e36 200d 0a20 2020 2065 6c69  = 13.6 ..    eli
-00004160: 6620 6163 6869 6576 656d 656e 7420 3c20  f achievement < 
-00004170: 3934 3a0d 0a20 2020 2020 2020 2062 6173  94:..        bas
-00004180: 6552 6120 3d20 3135 2e32 200d 0a20 2020  eRa = 15.2 ..   
-00004190: 2065 6c69 6620 6163 6869 6576 656d 656e   elif achievemen
-000041a0: 7420 3c20 3937 3a0d 0a20 2020 2020 2020  t < 97:..       
-000041b0: 2062 6173 6552 6120 3d20 3136 2e38 200d   baseRa = 16.8 .
-000041c0: 0a20 2020 2065 6c69 6620 6163 6869 6576  .    elif achiev
-000041d0: 656d 656e 7420 3c20 3938 3a0d 0a20 2020  ement < 98:..   
-000041e0: 2020 2020 2062 6173 6552 6120 3d20 3230       baseRa = 20
-000041f0: 2e30 200d 0a20 2020 2065 6c69 6620 6163  .0 ..    elif ac
-00004200: 6869 6576 656d 656e 7420 3c20 3939 3a0d  hievement < 99:.
-00004210: 0a20 2020 2020 2020 2062 6173 6552 6120  .        baseRa 
-00004220: 3d20 3230 2e33 0d0a 2020 2020 656c 6966  = 20.3..    elif
-00004230: 2061 6368 6965 7665 6d65 6e74 203c 2039   achievement < 9
-00004240: 392e 353a 0d0a 2020 2020 2020 2020 6261  9.5:..        ba
-00004250: 7365 5261 203d 2032 302e 3820 0d0a 2020  seRa = 20.8 ..  
-00004260: 2020 656c 6966 2061 6368 6965 7665 6d65    elif achieveme
-00004270: 6e74 203c 2031 3030 3a0d 0a20 2020 2020  nt < 100:..     
-00004280: 2020 2062 6173 6552 6120 3d20 3231 2e31     baseRa = 21.1
-00004290: 200d 0a20 2020 2065 6c69 6620 6163 6869   ..    elif achi
-000042a0: 6576 656d 656e 7420 3c20 3130 302e 353a  evement < 100.5:
-000042b0: 0d0a 2020 2020 2020 2020 6261 7365 5261  ..        baseRa
-000042c0: 203d 2032 312e 3620 0d0a 0d0a 2020 2020   = 21.6 ....    
-000042d0: 7265 7475 726e 206d 6174 682e 666c 6f6f  return math.floo
-000042e0: 7228 6473 202a 2028 6d69 6e28 3130 302e  r(ds * (min(100.
-000042f0: 352c 2061 6368 6965 7665 6d65 6e74 2920  5, achievement) 
-00004300: 2f20 3130 3029 202a 2062 6173 6552 6129  / 100) * baseRa)
-00004310: 0d0a 0d0a 0d0a 6173 796e 6320 6465 6620  ......async def 
-00004320: 6765 6e65 7261 7465 3530 2870 6179 6c6f  generate50(paylo
-00004330: 6164 3a20 4469 6374 2920 2d3e 2054 7570  ad: Dict) -> Tup
-00004340: 6c65 5b4f 7074 696f 6e61 6c5b 496d 6167  le[Optional[Imag
-00004350: 652e 496d 6167 655d 2c20 626f 6f6c 5d3a  e.Image], bool]:
-00004360: 0d0a 2020 2020 6173 796e 6320 7769 7468  ..    async with
-00004370: 2061 696f 6874 7470 2e72 6571 7565 7374   aiohttp.request
-00004380: 2822 504f 5354 222c 2022 6874 7470 733a  ("POST", "https:
-00004390: 2f2f 7777 772e 6469 7669 6e67 2d66 6973  //www.diving-fis
-000043a0: 682e 636f 6d2f 6170 692f 6d61 696d 6169  h.com/api/maimai
-000043b0: 6478 7072 6f62 6572 2f71 7565 7279 2f70  dxprober/query/p
-000043c0: 6c61 7965 7222 2c20 6a73 6f6e 3d70 6179  layer", json=pay
-000043d0: 6c6f 6164 2920 6173 2072 6573 703a 0d0a  load) as resp:..
-000043e0: 2020 2020 2020 2020 6966 2072 6573 702e          if resp.
-000043f0: 7374 6174 7573 203d 3d20 3430 303a 0d0a  status == 400:..
-00004400: 2020 2020 2020 2020 2020 2020 7265 7475              retu
-00004410: 726e 204e 6f6e 652c 2034 3030 0d0a 2020  rn None, 400..  
-00004420: 2020 2020 2020 6966 2072 6573 702e 7374        if resp.st
-00004430: 6174 7573 203d 3d20 3430 333a 0d0a 2020  atus == 403:..  
-00004440: 2020 2020 2020 2020 2020 7265 7475 726e            return
-00004450: 204e 6f6e 652c 2034 3033 0d0a 2020 2020   None, 403..    
-00004460: 2020 2020 7364 5f62 6573 7420 3d20 4265      sd_best = Be
-00004470: 7374 4c69 7374 2833 3529 0d0a 2020 2020  stList(35)..    
-00004480: 2020 2020 6478 5f62 6573 7420 3d20 4265      dx_best = Be
-00004490: 7374 4c69 7374 2831 3529 0d0a 2020 2020  stList(15)..    
-000044a0: 2020 2020 6f62 6a20 3d20 6177 6169 7420      obj = await 
-000044b0: 7265 7370 2e6a 736f 6e28 290d 0a20 2020  resp.json()..   
-000044c0: 2020 2020 2064 783a 204c 6973 745b 4469       dx: List[Di
-000044d0: 6374 5d20 3d20 6f62 6a5b 2263 6861 7274  ct] = obj["chart
-000044e0: 7322 5d5b 2264 7822 5d0d 0a20 2020 2020  s"]["dx"]..     
-000044f0: 2020 2073 643a 204c 6973 745b 4469 6374     sd: List[Dict
-00004500: 5d20 3d20 6f62 6a5b 2263 6861 7274 7322  ] = obj["charts"
-00004510: 5d5b 2273 6422 5d0d 0a20 2020 2020 2020  ]["sd"]..       
-00004520: 2066 6f72 2063 2069 6e20 7364 3a0d 0a20   for c in sd:.. 
-00004530: 2020 2020 2020 2020 2020 2073 645f 6265             sd_be
-00004540: 7374 2e70 7573 6828 4368 6172 7449 6e66  st.push(ChartInf
-00004550: 6f2e 6672 6f6d 5f6a 736f 6e28 6329 290d  o.from_json(c)).
-00004560: 0a20 2020 2020 2020 2066 6f72 2063 2069  .        for c i
-00004570: 6e20 6478 3a0d 0a20 2020 2020 2020 2020  n dx:..         
-00004580: 2020 2064 785f 6265 7374 2e70 7573 6828     dx_best.push(
-00004590: 4368 6172 7449 6e66 6f2e 6672 6f6d 5f6a  ChartInfo.from_j
-000045a0: 736f 6e28 6329 290d 0a20 2020 2020 2020  son(c))..       
-000045b0: 2070 6963 203d 2044 7261 7742 6573 7428   pic = DrawBest(
-000045c0: 7364 5f62 6573 742c 2064 785f 6265 7374  sd_best, dx_best
-000045d0: 2c20 6f62 6a5b 226e 6963 6b6e 616d 6522  , obj["nickname"
-000045e0: 5d29 2e67 6574 4469 7228 290d 0a20 2020  ]).getDir()..   
-000045f0: 2020 2020 2072 6574 7572 6e20 7069 632c       return pic,
-00004600: 2030 0d0a                                 0..
+00001ca0: 7665 725f 6469 7220 2b20 2730 3130 3030  ver_dir + '01000
+00001cb0: 2e70 6e67 270d 0a20 2020 2020 2020 2020  .png'..         
+00001cc0: 2020 2074 656d 7020 3d20 496d 6167 652e     temp = Image.
+00001cd0: 6f70 656e 2870 6e67 5061 7468 292e 636f  open(pngPath).co
+00001ce0: 6e76 6572 7428 2752 4742 2729 0d0a 2020  nvert('RGB')..  
+00001cf0: 2020 2020 2020 2020 2020 7465 6d70 203d            temp =
+00001d00: 2073 656c 662e 5f72 6573 697a 6550 6963   self._resizePic
+00001d10: 2874 656d 702c 2069 7465 6d57 202f 2074  (temp, itemW / t
+00001d20: 656d 702e 7369 7a65 5b30 5d29 0d0a 2020  emp.size[0])..  
+00001d30: 2020 2020 2020 2020 2020 7465 6d70 203d            temp =
+00001d40: 2074 656d 702e 6372 6f70 2828 302c 2028   temp.crop((0, (
+00001d50: 7465 6d70 2e73 697a 655b 315d 202d 2069  temp.size[1] - i
+00001d60: 7465 6d48 2920 2f20 322c 2069 7465 6d57  temH) / 2, itemW
+00001d70: 2c20 2874 656d 702e 7369 7a65 5b31 5d20  , (temp.size[1] 
+00001d80: 2b20 6974 656d 4829 202f 2032 2929 0d0a  + itemH) / 2))..
+00001d90: 2020 2020 2020 2020 2020 2020 7465 6d70              temp
+00001da0: 203d 2074 656d 702e 6669 6c74 6572 2849   = temp.filter(I
+00001db0: 6d61 6765 4669 6c74 6572 2e47 6175 7373  mageFilter.Gauss
+00001dc0: 6961 6e42 6c75 7228 3329 290d 0a20 2020  ianBlur(3))..   
+00001dd0: 2020 2020 2020 2020 2074 656d 7020 3d20           temp = 
+00001de0: 7465 6d70 2e70 6f69 6e74 286c 616d 6264  temp.point(lambd
+00001df0: 6120 703a 2069 6e74 2870 202a 2030 2e37  a p: int(p * 0.7
+00001e00: 3229 290d 0a0d 0a20 2020 2020 2020 2020  2))....         
+00001e10: 2020 2074 656d 7044 7261 7720 3d20 496d     tempDraw = Im
+00001e20: 6167 6544 7261 772e 4472 6177 2874 656d  ageDraw.Draw(tem
+00001e30: 7029 0d0a 2020 2020 2020 2020 2020 2020  p)..            
+00001e40: 7465 6d70 4472 6177 2e70 6f6c 7967 6f6e  tempDraw.polygon
+00001e50: 286c 6576 656c 5472 6961 676c 652c 2043  (levelTriagle, C
+00001e60: 6f6c 6f72 5b63 6861 7274 496e 666f 2e64  olor[chartInfo.d
+00001e70: 6966 665d 290d 0a20 2020 2020 2020 2020  iff])..         
+00001e80: 2020 2066 6f6e 7420 3d20 496d 6167 6546     font = ImageF
+00001e90: 6f6e 742e 7472 7565 7479 7065 2874 6974  ont.truetype(tit
+00001ea0: 6c65 466f 6e74 4e61 6d65 2c20 3136 2c20  leFontName, 16, 
+00001eb0: 656e 636f 6469 6e67 3d27 7574 662d 3827  encoding='utf-8'
+00001ec0: 290d 0a20 2020 2020 2020 2020 2020 2074  )..            t
+00001ed0: 6974 6c65 203d 2063 6861 7274 496e 666f  itle = chartInfo
+00001ee0: 2e74 6974 6c65 0d0a 2020 2020 2020 2020  .title..        
+00001ef0: 2020 2020 6966 2073 656c 662e 5f63 6f6c      if self._col
+00001f00: 6f75 6d57 6964 7468 2874 6974 6c65 2920  oumWidth(title) 
+00001f10: 3e20 3135 3a0d 0a20 2020 2020 2020 2020  > 15:..         
+00001f20: 2020 2020 2020 2074 6974 6c65 203d 2073         title = s
+00001f30: 656c 662e 5f63 6861 6e67 6543 6f6c 756d  elf._changeColum
+00001f40: 6e57 6964 7468 2874 6974 6c65 2c20 3132  nWidth(title, 12
+00001f50: 2920 2b20 272e 2e2e 270d 0a20 2020 2020  ) + '...'..     
+00001f60: 2020 2020 2020 2074 656d 7044 7261 772e         tempDraw.
+00001f70: 7465 7874 2828 382c 2038 292c 2074 6974  text((8, 8), tit
+00001f80: 6c65 2c20 2777 6869 7465 272c 2066 6f6e  le, 'white', fon
+00001f90: 7429 0d0a 2020 2020 2020 2020 2020 2020  t)..            
+00001fa0: 666f 6e74 203d 2049 6d61 6765 466f 6e74  font = ImageFont
+00001fb0: 2e74 7275 6574 7970 6528 7469 746c 6546  .truetype(titleF
+00001fc0: 6f6e 744e 616d 652c 2031 322c 2065 6e63  ontName, 12, enc
+00001fd0: 6f64 696e 673d 2775 7466 2d38 2729 0d0a  oding='utf-8')..
+00001fe0: 0d0a 2020 2020 2020 2020 2020 2020 7465  ..            te
+00001ff0: 6d70 4472 6177 2e74 6578 7428 2837 2c20  mpDraw.text((7, 
+00002000: 3238 292c 2066 277b 2225 2e34 6622 2025  28), f'{"%.4f" %
+00002010: 2063 6861 7274 496e 666f 2e61 6368 6965   chartInfo.achie
+00002020: 7665 6d65 6e74 7d25 272c 2027 7768 6974  vement}%', 'whit
+00002030: 6527 2c20 666f 6e74 290d 0a20 2020 2020  e', font)..     
+00002040: 2020 2020 2020 2072 616e 6b49 6d67 203d         rankImg =
+00002050: 2049 6d61 6765 2e6f 7065 6e28 7365 6c66   Image.open(self
+00002060: 2e70 6963 5f64 6972 202b 2066 2755 495f  .pic_dir + f'UI_
+00002070: 4741 4d5f 5261 6e6b 5f7b 7261 6e6b 5069  GAM_Rank_{rankPi
+00002080: 635b 6368 6172 7449 6e66 6f2e 7363 6f72  c[chartInfo.scor
+00002090: 6549 645d 7d2e 706e 6727 292e 636f 6e76  eId]}.png').conv
+000020a0: 6572 7428 2752 4742 4127 290d 0a20 2020  ert('RGBA')..   
+000020b0: 2020 2020 2020 2020 2072 616e 6b49 6d67           rankImg
+000020c0: 203d 2073 656c 662e 5f72 6573 697a 6550   = self._resizeP
+000020d0: 6963 2872 616e 6b49 6d67 2c20 302e 3329  ic(rankImg, 0.3)
+000020e0: 0d0a 2020 2020 2020 2020 2020 2020 7465  ..            te
+000020f0: 6d70 2e70 6173 7465 2872 616e 6b49 6d67  mp.paste(rankImg
+00002100: 2c20 2837 322c 2032 3829 2c20 7261 6e6b  , (72, 28), rank
+00002110: 496d 672e 7370 6c69 7428 295b 335d 290d  Img.split()[3]).
+00002120: 0a20 2020 2020 2020 2020 2020 2069 6620  .            if 
+00002130: 6368 6172 7449 6e66 6f2e 636f 6d62 6f49  chartInfo.comboI
+00002140: 643a 0d0a 2020 2020 2020 2020 2020 2020  d:..            
+00002150: 2020 2020 636f 6d62 6f49 6d67 203d 2049      comboImg = I
+00002160: 6d61 6765 2e6f 7065 6e28 7365 6c66 2e70  mage.open(self.p
+00002170: 6963 5f64 6972 202b 2066 2755 495f 4d53  ic_dir + f'UI_MS
+00002180: 535f 4d42 6173 655f 4963 6f6e 5f7b 636f  S_MBase_Icon_{co
+00002190: 6d62 6f50 6963 5b63 6861 7274 496e 666f  mboPic[chartInfo
+000021a0: 2e63 6f6d 626f 4964 5d7d 5f53 2e70 6e67  .comboId]}_S.png
+000021b0: 2729 2e63 6f6e 7665 7274 2827 5247 4241  ').convert('RGBA
+000021c0: 2729 0d0a 2020 2020 2020 2020 2020 2020  ')..            
+000021d0: 2020 2020 636f 6d62 6f49 6d67 203d 2073      comboImg = s
+000021e0: 656c 662e 5f72 6573 697a 6550 6963 2863  elf._resizePic(c
+000021f0: 6f6d 626f 496d 672c 2030 2e34 3529 0d0a  omboImg, 0.45)..
+00002200: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00002210: 7465 6d70 2e70 6173 7465 2863 6f6d 626f  temp.paste(combo
+00002220: 496d 672c 2028 3130 332c 2032 3729 2c20  Img, (103, 27), 
+00002230: 636f 6d62 6f49 6d67 2e73 706c 6974 2829  comboImg.split()
+00002240: 5b33 5d29 0d0a 2020 2020 2020 2020 2020  [3])..          
+00002250: 2020 666f 6e74 203d 2049 6d61 6765 466f    font = ImageFo
+00002260: 6e74 2e74 7275 6574 7970 6528 5354 4154  nt.truetype(STAT
+00002270: 4943 202b 2027 2f61 646f 6265 5f73 696d  IC + '/adobe_sim
+00002280: 6865 692e 6f74 6627 2c20 3132 2c20 656e  hei.otf', 12, en
+00002290: 636f 6469 6e67 3d27 7574 662d 3827 290d  coding='utf-8').
+000022a0: 0a20 2020 2020 2020 2020 2020 2074 656d  .            tem
+000022b0: 7044 7261 772e 7465 7874 2828 382c 2034  pDraw.text((8, 4
+000022c0: 3429 2c20 6627 4261 7365 3a20 7b63 6861  4), f'Base: {cha
+000022d0: 7274 496e 666f 2e64 737d 202d 3e20 7b63  rtInfo.ds} -> {c
+000022e0: 6f6d 7075 7465 5261 2863 6861 7274 496e  omputeRa(chartIn
+000022f0: 666f 2e64 732c 2063 6861 7274 496e 666f  fo.ds, chartInfo
+00002300: 2e61 6368 6965 7665 6d65 6e74 297d 272c  .achievement)}',
+00002310: 2027 7768 6974 6527 2c20 666f 6e74 290d   'white', font).
+00002320: 0a20 2020 2020 2020 2020 2020 2066 6f6e  .            fon
+00002330: 7420 3d20 496d 6167 6546 6f6e 742e 7472  t = ImageFont.tr
+00002340: 7565 7479 7065 2853 5441 5449 4320 2b20  uetype(STATIC + 
+00002350: 272f 6164 6f62 655f 7369 6d68 6569 2e6f  '/adobe_simhei.o
+00002360: 7466 272c 2031 382c 2065 6e63 6f64 696e  tf', 18, encodin
+00002370: 673d 2775 7466 2d38 2729 0d0a 2020 2020  g='utf-8')..    
+00002380: 2020 2020 2020 2020 7465 6d70 4472 6177          tempDraw
+00002390: 2e74 6578 7428 2838 2c20 3630 292c 2066  .text((8, 60), f
+000023a0: 2723 7b6e 756d 202b 2031 7d27 2c20 2777  '#{num + 1}', 'w
+000023b0: 6869 7465 272c 2066 6f6e 7429 0d0a 0d0a  hite', font)....
+000023c0: 2020 2020 2020 2020 2020 2020 7265 6342              recB
+000023d0: 6173 6520 3d20 496d 6167 652e 6e65 7728  ase = Image.new(
+000023e0: 2752 4742 4127 2c20 2869 7465 6d57 2c20  'RGBA', (itemW, 
+000023f0: 6974 656d 4829 2c20 2762 6c61 636b 2729  itemH), 'black')
+00002400: 0d0a 2020 2020 2020 2020 2020 2020 7265  ..            re
+00002410: 6342 6173 6520 3d20 7265 6342 6173 652e  cBase = recBase.
+00002420: 706f 696e 7428 6c61 6d62 6461 2070 3a20  point(lambda p: 
+00002430: 696e 7428 7020 2a20 302e 3829 290d 0a20  int(p * 0.8)).. 
+00002440: 2020 2020 2020 2020 2020 2069 6d67 2e70             img.p
+00002450: 6173 7465 2872 6563 4261 7365 2c20 2873  aste(recBase, (s
+00002460: 656c 662e 434f 4c4f 554d 535f 494d 475b  elf.COLOUMS_IMG[
+00002470: 6a5d 202b 2035 2c20 7365 6c66 2e52 4f57  j] + 5, self.ROW
+00002480: 535f 494d 475b 6920 2b20 315d 202b 2035  S_IMG[i + 1] + 5
+00002490: 2929 0d0a 2020 2020 2020 2020 2020 2020  ))..            
+000024a0: 696d 672e 7061 7374 6528 7465 6d70 2c20  img.paste(temp, 
+000024b0: 2873 656c 662e 434f 4c4f 554d 535f 494d  (self.COLOUMS_IM
+000024c0: 475b 6a5d 202b 2034 2c20 7365 6c66 2e52  G[j] + 4, self.R
+000024d0: 4f57 535f 494d 475b 6920 2b20 315d 202b  OWS_IMG[i + 1] +
+000024e0: 2034 2929 0d0a 2020 2020 2020 2020 666f   4))..        fo
+000024f0: 7220 6e75 6d20 696e 2072 616e 6765 286c  r num in range(l
+00002500: 656e 2873 6442 6573 7429 2c20 7364 4265  en(sdBest), sdBe
+00002510: 7374 2e73 697a 6529 3a0d 0a20 2020 2020  st.size):..     
+00002520: 2020 2020 2020 2069 203d 206e 756d 202f         i = num /
+00002530: 2f20 370d 0a20 2020 2020 2020 2020 2020  / 7..           
+00002540: 206a 203d 206e 756d 2025 2037 0d0a 2020   j = num % 7..  
+00002550: 2020 2020 2020 2020 2020 7465 6d70 203d            temp =
+00002560: 2049 6d61 6765 2e6f 7065 6e28 7365 6c66   Image.open(self
+00002570: 2e63 6f76 6572 5f64 6972 202b 2066 2730  .cover_dir + f'0
+00002580: 3130 3030 2e70 6e67 2729 2e63 6f6e 7665  1000.png').conve
+00002590: 7274 2827 5247 4227 290d 0a20 2020 2020  rt('RGB')..     
+000025a0: 2020 2020 2020 2074 656d 7020 3d20 7365         temp = se
+000025b0: 6c66 2e5f 7265 7369 7a65 5069 6328 7465  lf._resizePic(te
+000025c0: 6d70 2c20 6974 656d 5720 2f20 7465 6d70  mp, itemW / temp
+000025d0: 2e73 697a 655b 305d 290d 0a20 2020 2020  .size[0])..     
+000025e0: 2020 2020 2020 2074 656d 7020 3d20 7465         temp = te
+000025f0: 6d70 2e63 726f 7028 2830 2c20 2874 656d  mp.crop((0, (tem
+00002600: 702e 7369 7a65 5b31 5d20 2d20 6974 656d  p.size[1] - item
+00002610: 4829 202f 2032 2c20 6974 656d 572c 2028  H) / 2, itemW, (
+00002620: 7465 6d70 2e73 697a 655b 315d 202b 2069  temp.size[1] + i
+00002630: 7465 6d48 2920 2f20 3229 290d 0a20 2020  temH) / 2))..   
+00002640: 2020 2020 2020 2020 2074 656d 7020 3d20           temp = 
+00002650: 7465 6d70 2e66 696c 7465 7228 496d 6167  temp.filter(Imag
+00002660: 6546 696c 7465 722e 4761 7573 7369 616e  eFilter.Gaussian
+00002670: 426c 7572 2831 2929 0d0a 2020 2020 2020  Blur(1))..      
+00002680: 2020 2020 2020 696d 672e 7061 7374 6528        img.paste(
+00002690: 7465 6d70 2c20 2873 656c 662e 434f 4c4f  temp, (self.COLO
+000026a0: 554d 535f 494d 475b 6a5d 202b 2034 2c20  UMS_IMG[j] + 4, 
+000026b0: 7365 6c66 2e52 4f57 535f 494d 475b 6920  self.ROWS_IMG[i 
+000026c0: 2b20 315d 202b 2034 2929 0d0a 2020 2020  + 1] + 4))..    
+000026d0: 2020 2020 666f 7220 6e75 6d20 696e 2072      for num in r
+000026e0: 616e 6765 2830 2c20 6c65 6e28 6478 4265  ange(0, len(dxBe
+000026f0: 7374 2929 3a0d 0a20 2020 2020 2020 2020  st)):..         
+00002700: 2020 2069 203d 206e 756d 202f 2f20 330d     i = num // 3.
+00002710: 0a20 2020 2020 2020 2020 2020 206a 203d  .            j =
+00002720: 206e 756d 2025 2033 0d0a 2020 2020 2020   num % 3..      
+00002730: 2020 2020 2020 6368 6172 7449 6e66 6f20        chartInfo 
+00002740: 3d20 6478 4265 7374 5b6e 756d 5d0d 0a20  = dxBest[num].. 
+00002750: 2020 2020 2020 2020 2020 2070 6e67 5061             pngPa
+00002760: 7468 203d 2073 656c 662e 636f 7665 725f  th = self.cover_
+00002770: 6469 7220 2b20 6627 7b67 6574 5f63 6f76  dir + f'{get_cov
+00002780: 6572 5f6c 656e 355f 6964 2863 6861 7274  er_len5_id(chart
+00002790: 496e 666f 2e69 644e 756d 297d 2e70 6e67  Info.idNum)}.png
+000027a0: 270d 0a20 2020 2020 2020 2020 2020 2069  '..            i
+000027b0: 6620 6e6f 7420 6f73 2e70 6174 682e 6578  f not os.path.ex
+000027c0: 6973 7473 2870 6e67 5061 7468 293a 0d0a  ists(pngPath):..
+000027d0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000027e0: 706e 6750 6174 6820 3d20 7365 6c66 2e63  pngPath = self.c
+000027f0: 6f76 6572 5f64 6972 202b 2027 3031 3030  over_dir + '0100
+00002800: 302e 706e 6727 0d0a 2020 2020 2020 2020  0.png'..        
+00002810: 2020 2020 7465 6d70 203d 2049 6d61 6765      temp = Image
+00002820: 2e6f 7065 6e28 706e 6750 6174 6829 2e63  .open(pngPath).c
+00002830: 6f6e 7665 7274 2827 5247 4227 290d 0a20  onvert('RGB').. 
+00002840: 2020 2020 2020 2020 2020 2074 656d 7020             temp 
+00002850: 3d20 7365 6c66 2e5f 7265 7369 7a65 5069  = self._resizePi
+00002860: 6328 7465 6d70 2c20 6974 656d 5720 2f20  c(temp, itemW / 
+00002870: 7465 6d70 2e73 697a 655b 305d 290d 0a20  temp.size[0]).. 
+00002880: 2020 2020 2020 2020 2020 2074 656d 7020             temp 
+00002890: 3d20 7465 6d70 2e63 726f 7028 2830 2c20  = temp.crop((0, 
+000028a0: 2874 656d 702e 7369 7a65 5b31 5d20 2d20  (temp.size[1] - 
+000028b0: 6974 656d 4829 202f 2032 2c20 6974 656d  itemH) / 2, item
+000028c0: 572c 2028 7465 6d70 2e73 697a 655b 315d  W, (temp.size[1]
+000028d0: 202b 2069 7465 6d48 2920 2f20 3229 290d   + itemH) / 2)).
+000028e0: 0a20 2020 2020 2020 2020 2020 2074 656d  .            tem
+000028f0: 7020 3d20 7465 6d70 2e66 696c 7465 7228  p = temp.filter(
+00002900: 496d 6167 6546 696c 7465 722e 4761 7573  ImageFilter.Gaus
+00002910: 7369 616e 426c 7572 2833 2929 0d0a 2020  sianBlur(3))..  
+00002920: 2020 2020 2020 2020 2020 7465 6d70 203d            temp =
+00002930: 2074 656d 702e 706f 696e 7428 6c61 6d62   temp.point(lamb
+00002940: 6461 2070 3a20 696e 7428 7020 2a20 302e  da p: int(p * 0.
+00002950: 3732 2929 0d0a 0d0a 2020 2020 2020 2020  72))....        
+00002960: 2020 2020 7465 6d70 4472 6177 203d 2049      tempDraw = I
+00002970: 6d61 6765 4472 6177 2e44 7261 7728 7465  mageDraw.Draw(te
+00002980: 6d70 290d 0a20 2020 2020 2020 2020 2020  mp)..           
+00002990: 2074 656d 7044 7261 772e 706f 6c79 676f   tempDraw.polygo
+000029a0: 6e28 6c65 7665 6c54 7269 6167 6c65 2c20  n(levelTriagle, 
+000029b0: 436f 6c6f 725b 6368 6172 7449 6e66 6f2e  Color[chartInfo.
+000029c0: 6469 6666 5d29 0d0a 2020 2020 2020 2020  diff])..        
+000029d0: 2020 2020 666f 6e74 203d 2049 6d61 6765      font = Image
+000029e0: 466f 6e74 2e74 7275 6574 7970 6528 7469  Font.truetype(ti
+000029f0: 746c 6546 6f6e 744e 616d 652c 2031 342c  tleFontName, 14,
+00002a00: 2065 6e63 6f64 696e 673d 2775 7466 2d38   encoding='utf-8
+00002a10: 2729 0d0a 2020 2020 2020 2020 2020 2020  ')..            
+00002a20: 7469 746c 6520 3d20 6368 6172 7449 6e66  title = chartInf
+00002a30: 6f2e 7469 746c 650d 0a20 2020 2020 2020  o.title..       
+00002a40: 2020 2020 2069 6620 7365 6c66 2e5f 636f       if self._co
+00002a50: 6c6f 756d 5769 6474 6828 7469 746c 6529  loumWidth(title)
+00002a60: 203e 2031 333a 0d0a 2020 2020 2020 2020   > 13:..        
+00002a70: 2020 2020 2020 2020 7469 746c 6520 3d20          title = 
+00002a80: 7365 6c66 2e5f 6368 616e 6765 436f 6c75  self._changeColu
+00002a90: 6d6e 5769 6474 6828 7469 746c 652c 2031  mnWidth(title, 1
+00002aa0: 3229 202b 2027 2e2e 2e27 0d0a 2020 2020  2) + '...'..    
+00002ab0: 2020 2020 2020 2020 7465 6d70 4472 6177          tempDraw
+00002ac0: 2e74 6578 7428 2838 2c20 3829 2c20 7469  .text((8, 8), ti
+00002ad0: 746c 652c 2027 7768 6974 6527 2c20 666f  tle, 'white', fo
+00002ae0: 6e74 290d 0a20 2020 2020 2020 2020 2020  nt)..           
+00002af0: 2066 6f6e 7420 3d20 496d 6167 6546 6f6e   font = ImageFon
+00002b00: 742e 7472 7565 7479 7065 2874 6974 6c65  t.truetype(title
+00002b10: 466f 6e74 4e61 6d65 2c20 3132 2c20 656e  FontName, 12, en
+00002b20: 636f 6469 6e67 3d27 7574 662d 3827 290d  coding='utf-8').
+00002b30: 0a0d 0a20 2020 2020 2020 2020 2020 2074  ...            t
+00002b40: 656d 7044 7261 772e 7465 7874 2828 372c  empDraw.text((7,
+00002b50: 2032 3829 2c20 6627 7b22 252e 3466 2220   28), f'{"%.4f" 
+00002b60: 2520 6368 6172 7449 6e66 6f2e 6163 6869  % chartInfo.achi
+00002b70: 6576 656d 656e 747d 2527 2c20 2777 6869  evement}%', 'whi
+00002b80: 7465 272c 2066 6f6e 7429 0d0a 2020 2020  te', font)..    
+00002b90: 2020 2020 2020 2020 7261 6e6b 496d 6720          rankImg 
+00002ba0: 3d20 496d 6167 652e 6f70 656e 2873 656c  = Image.open(sel
+00002bb0: 662e 7069 635f 6469 7220 2b20 6627 5549  f.pic_dir + f'UI
+00002bc0: 5f47 414d 5f52 616e 6b5f 7b72 616e 6b50  _GAM_Rank_{rankP
+00002bd0: 6963 5b63 6861 7274 496e 666f 2e73 636f  ic[chartInfo.sco
+00002be0: 7265 4964 5d7d 2e70 6e67 2729 2e63 6f6e  reId]}.png').con
+00002bf0: 7665 7274 2827 5247 4241 2729 0d0a 2020  vert('RGBA')..  
+00002c00: 2020 2020 2020 2020 2020 7261 6e6b 496d            rankIm
+00002c10: 6720 3d20 7365 6c66 2e5f 7265 7369 7a65  g = self._resize
+00002c20: 5069 6328 7261 6e6b 496d 672c 2030 2e33  Pic(rankImg, 0.3
+00002c30: 290d 0a20 2020 2020 2020 2020 2020 2074  )..            t
+00002c40: 656d 702e 7061 7374 6528 7261 6e6b 496d  emp.paste(rankIm
+00002c50: 672c 2028 3732 2c20 3238 292c 2072 616e  g, (72, 28), ran
+00002c60: 6b49 6d67 2e73 706c 6974 2829 5b33 5d29  kImg.split()[3])
+00002c70: 0d0a 2020 2020 2020 2020 2020 2020 6966  ..            if
+00002c80: 2063 6861 7274 496e 666f 2e63 6f6d 626f   chartInfo.combo
+00002c90: 4964 3a0d 0a20 2020 2020 2020 2020 2020  Id:..           
+00002ca0: 2020 2020 2063 6f6d 626f 496d 6720 3d20       comboImg = 
+00002cb0: 496d 6167 652e 6f70 656e 2873 656c 662e  Image.open(self.
+00002cc0: 7069 635f 6469 7220 2b20 6627 5549 5f4d  pic_dir + f'UI_M
+00002cd0: 5353 5f4d 4261 7365 5f49 636f 6e5f 7b63  SS_MBase_Icon_{c
+00002ce0: 6f6d 626f 5069 635b 6368 6172 7449 6e66  omboPic[chartInf
+00002cf0: 6f2e 636f 6d62 6f49 645d 7d5f 532e 706e  o.comboId]}_S.pn
+00002d00: 6727 292e 636f 6e76 6572 7428 0d0a 2020  g').convert(..  
+00002d10: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00002d20: 2020 2752 4742 4127 290d 0a20 2020 2020    'RGBA')..     
+00002d30: 2020 2020 2020 2020 2020 2063 6f6d 626f             combo
+00002d40: 496d 6720 3d20 7365 6c66 2e5f 7265 7369  Img = self._resi
+00002d50: 7a65 5069 6328 636f 6d62 6f49 6d67 2c20  zePic(comboImg, 
+00002d60: 302e 3435 290d 0a20 2020 2020 2020 2020  0.45)..         
+00002d70: 2020 2020 2020 2074 656d 702e 7061 7374         temp.past
+00002d80: 6528 636f 6d62 6f49 6d67 2c20 2831 3033  e(comboImg, (103
+00002d90: 2c20 3237 292c 2063 6f6d 626f 496d 672e  , 27), comboImg.
+00002da0: 7370 6c69 7428 295b 335d 290d 0a20 2020  split()[3])..   
+00002db0: 2020 2020 2020 2020 2066 6f6e 7420 3d20           font = 
+00002dc0: 496d 6167 6546 6f6e 742e 7472 7565 7479  ImageFont.truety
+00002dd0: 7065 2853 5441 5449 4320 2b20 272f 6164  pe(STATIC + '/ad
+00002de0: 6f62 655f 7369 6d68 6569 2e6f 7466 272c  obe_simhei.otf',
+00002df0: 2031 322c 2065 6e63 6f64 696e 673d 2775   12, encoding='u
+00002e00: 7466 2d38 2729 0d0a 2020 2020 2020 2020  tf-8')..        
+00002e10: 2020 2020 7465 6d70 4472 6177 2e74 6578      tempDraw.tex
+00002e20: 7428 2838 2c20 3434 292c 2066 2742 6173  t((8, 44), f'Bas
+00002e30: 653a 207b 6368 6172 7449 6e66 6f2e 6473  e: {chartInfo.ds
+00002e40: 7d20 2d3e 207b 6368 6172 7449 6e66 6f2e  } -> {chartInfo.
+00002e50: 7261 7d27 2c20 2777 6869 7465 272c 2066  ra}', 'white', f
+00002e60: 6f6e 7429 0d0a 2020 2020 2020 2020 2020  ont)..          
+00002e70: 2020 666f 6e74 203d 2049 6d61 6765 466f    font = ImageFo
+00002e80: 6e74 2e74 7275 6574 7970 6528 5354 4154  nt.truetype(STAT
+00002e90: 4943 202b 2027 2f61 646f 6265 5f73 696d  IC + '/adobe_sim
+00002ea0: 6865 692e 6f74 6627 2c20 3138 2c20 656e  hei.otf', 18, en
+00002eb0: 636f 6469 6e67 3d27 7574 662d 3827 290d  coding='utf-8').
+00002ec0: 0a20 2020 2020 2020 2020 2020 2074 656d  .            tem
+00002ed0: 7044 7261 772e 7465 7874 2828 382c 2036  pDraw.text((8, 6
+00002ee0: 3029 2c20 6627 237b 6e75 6d20 2b20 317d  0), f'#{num + 1}
+00002ef0: 272c 2027 7768 6974 6527 2c20 666f 6e74  ', 'white', font
+00002f00: 290d 0a0d 0a20 2020 2020 2020 2020 2020  )....           
+00002f10: 2072 6563 4261 7365 203d 2049 6d61 6765   recBase = Image
+00002f20: 2e6e 6577 2827 5247 4241 272c 2028 6974  .new('RGBA', (it
+00002f30: 656d 572c 2069 7465 6d48 292c 2027 626c  emW, itemH), 'bl
+00002f40: 6163 6b27 290d 0a20 2020 2020 2020 2020  ack')..         
+00002f50: 2020 2072 6563 4261 7365 203d 2072 6563     recBase = rec
+00002f60: 4261 7365 2e70 6f69 6e74 286c 616d 6264  Base.point(lambd
+00002f70: 6120 703a 2069 6e74 2870 202a 2030 2e38  a p: int(p * 0.8
+00002f80: 2929 0d0a 2020 2020 2020 2020 2020 2020  ))..            
+00002f90: 696d 672e 7061 7374 6528 7265 6342 6173  img.paste(recBas
+00002fa0: 652c 2028 7365 6c66 2e43 4f4c 4f55 4d53  e, (self.COLOUMS
+00002fb0: 5f49 4d47 5b6a 202b 2038 5d20 2b20 352c  _IMG[j + 8] + 5,
+00002fc0: 2073 656c 662e 524f 5753 5f49 4d47 5b69   self.ROWS_IMG[i
+00002fd0: 202b 2031 5d20 2b20 3529 290d 0a20 2020   + 1] + 5))..   
+00002fe0: 2020 2020 2020 2020 2069 6d67 2e70 6173           img.pas
+00002ff0: 7465 2874 656d 702c 2028 7365 6c66 2e43  te(temp, (self.C
+00003000: 4f4c 4f55 4d53 5f49 4d47 5b6a 202b 2038  OLOUMS_IMG[j + 8
+00003010: 5d20 2b20 342c 2073 656c 662e 524f 5753  ] + 4, self.ROWS
+00003020: 5f49 4d47 5b69 202b 2031 5d20 2b20 3429  _IMG[i + 1] + 4)
+00003030: 290d 0a20 2020 2020 2020 2066 6f72 206e  )..        for n
+00003040: 756d 2069 6e20 7261 6e67 6528 6c65 6e28  um in range(len(
+00003050: 6478 4265 7374 292c 2064 7842 6573 742e  dxBest), dxBest.
+00003060: 7369 7a65 293a 0d0a 2020 2020 2020 2020  size):..        
+00003070: 2020 2020 6920 3d20 6e75 6d20 2f2f 2033      i = num // 3
+00003080: 0d0a 2020 2020 2020 2020 2020 2020 6a20  ..            j 
+00003090: 3d20 6e75 6d20 2520 330d 0a20 2020 2020  = num % 3..     
+000030a0: 2020 2020 2020 2074 656d 7020 3d20 496d         temp = Im
+000030b0: 6167 652e 6f70 656e 2873 656c 662e 636f  age.open(self.co
+000030c0: 7665 725f 6469 7220 2b20 6627 3031 3030  ver_dir + f'0100
+000030d0: 302e 706e 6727 292e 636f 6e76 6572 7428  0.png').convert(
+000030e0: 2752 4742 2729 0d0a 2020 2020 2020 2020  'RGB')..        
+000030f0: 2020 2020 7465 6d70 203d 2073 656c 662e      temp = self.
+00003100: 5f72 6573 697a 6550 6963 2874 656d 702c  _resizePic(temp,
+00003110: 2069 7465 6d57 202f 2074 656d 702e 7369   itemW / temp.si
+00003120: 7a65 5b30 5d29 0d0a 2020 2020 2020 2020  ze[0])..        
+00003130: 2020 2020 7465 6d70 203d 2074 656d 702e      temp = temp.
+00003140: 6372 6f70 2828 302c 2028 7465 6d70 2e73  crop((0, (temp.s
+00003150: 697a 655b 315d 202d 2069 7465 6d48 2920  ize[1] - itemH) 
+00003160: 2f20 322c 2069 7465 6d57 2c20 2874 656d  / 2, itemW, (tem
+00003170: 702e 7369 7a65 5b31 5d20 2b20 6974 656d  p.size[1] + item
+00003180: 4829 202f 2032 2929 0d0a 2020 2020 2020  H) / 2))..      
+00003190: 2020 2020 2020 7465 6d70 203d 2074 656d        temp = tem
+000031a0: 702e 6669 6c74 6572 2849 6d61 6765 4669  p.filter(ImageFi
+000031b0: 6c74 6572 2e47 6175 7373 6961 6e42 6c75  lter.GaussianBlu
+000031c0: 7228 3129 290d 0a20 2020 2020 2020 2020  r(1))..         
+000031d0: 2020 2069 6d67 2e70 6173 7465 2874 656d     img.paste(tem
+000031e0: 702c 2028 7365 6c66 2e43 4f4c 4f55 4d53  p, (self.COLOUMS
+000031f0: 5f49 4d47 5b6a 202b 2038 5d20 2b20 342c  _IMG[j + 8] + 4,
+00003200: 2073 656c 662e 524f 5753 5f49 4d47 5b69   self.ROWS_IMG[i
+00003210: 202b 2031 5d20 2b20 3429 290d 0a0d 0a20   + 1] + 4)).... 
+00003220: 2020 2064 6566 2064 7261 7728 7365 6c66     def draw(self
+00003230: 293a 0d0a 2020 2020 2020 2020 7370 6c61  ):..        spla
+00003240: 7368 4c6f 676f 203d 2049 6d61 6765 2e6f  shLogo = Image.o
+00003250: 7065 6e28 7365 6c66 2e70 6963 5f64 6972  pen(self.pic_dir
+00003260: 202b 2027 5549 5f43 4d4e 5f54 6162 5469   + 'UI_CMN_TabTi
+00003270: 746c 655f 4d61 696d 6169 5469 746c 655f  tle_MaimaiTitle_
+00003280: 5665 7232 3134 2e70 6e67 2729 2e63 6f6e  Ver214.png').con
+00003290: 7665 7274 2827 5247 4241 2729 0d0a 2020  vert('RGBA')..  
+000032a0: 2020 2020 2020 7370 6c61 7368 4c6f 676f        splashLogo
+000032b0: 203d 2073 656c 662e 5f72 6573 697a 6550   = self._resizeP
+000032c0: 6963 2873 706c 6173 684c 6f67 6f2c 2030  ic(splashLogo, 0
+000032d0: 2e36 3529 0d0a 2020 2020 2020 2020 7365  .65)..        se
+000032e0: 6c66 2e69 6d67 2e70 6173 7465 2873 706c  lf.img.paste(spl
+000032f0: 6173 684c 6f67 6f2c 2028 3130 2c20 3130  ashLogo, (10, 10
+00003300: 292c 206d 6173 6b3d 7370 6c61 7368 4c6f  ), mask=splashLo
+00003310: 676f 2e73 706c 6974 2829 5b33 5d29 0d0a  go.split()[3])..
+00003320: 0d0a 2020 2020 2020 2020 7261 7469 6e67  ..        rating
+00003330: 4261 7365 496d 6720 3d20 496d 6167 652e  BaseImg = Image.
+00003340: 6f70 656e 2873 656c 662e 7069 635f 6469  open(self.pic_di
+00003350: 7220 2b20 7365 6c66 2e5f 6669 6e64 5261  r + self._findRa
+00003360: 5069 6328 2929 2e63 6f6e 7665 7274 2827  Pic()).convert('
+00003370: 5247 4241 2729 0d0a 2020 2020 2020 2020  RGBA')..        
+00003380: 7261 7469 6e67 4261 7365 496d 6720 3d20  ratingBaseImg = 
+00003390: 7365 6c66 2e5f 6472 6177 5261 7469 6e67  self._drawRating
+000033a0: 2872 6174 696e 6742 6173 6549 6d67 290d  (ratingBaseImg).
+000033b0: 0a20 2020 2020 2020 2072 6174 696e 6742  .        ratingB
+000033c0: 6173 6549 6d67 203d 2073 656c 662e 5f72  aseImg = self._r
+000033d0: 6573 697a 6550 6963 2872 6174 696e 6742  esizePic(ratingB
+000033e0: 6173 6549 6d67 2c20 302e 3835 290d 0a20  aseImg, 0.85).. 
+000033f0: 2020 2020 2020 2073 656c 662e 696d 672e         self.img.
+00003400: 7061 7374 6528 7261 7469 6e67 4261 7365  paste(ratingBase
+00003410: 496d 672c 2028 3234 302c 2038 292c 206d  Img, (240, 8), m
+00003420: 6173 6b3d 7261 7469 6e67 4261 7365 496d  ask=ratingBaseIm
+00003430: 672e 7370 6c69 7428 295b 335d 290d 0a0d  g.split()[3])...
+00003440: 0a20 2020 2020 2020 206e 616d 6550 6c61  .        namePla
+00003450: 7465 496d 6720 3d20 496d 6167 652e 6f70  teImg = Image.op
+00003460: 656e 2873 656c 662e 7069 635f 6469 7220  en(self.pic_dir 
+00003470: 2b20 2755 495f 5453 545f 506c 6174 654d  + 'UI_TST_PlateM
+00003480: 6173 6b2e 706e 6727 292e 636f 6e76 6572  ask.png').conver
+00003490: 7428 2752 4742 4127 290d 0a20 2020 2020  t('RGBA')..     
+000034a0: 2020 206e 616d 6550 6c61 7465 496d 6720     namePlateImg 
+000034b0: 3d20 6e61 6d65 506c 6174 6549 6d67 2e72  = namePlateImg.r
+000034c0: 6573 697a 6528 2832 3835 2c20 3430 2929  esize((285, 40))
+000034d0: 0d0a 2020 2020 2020 2020 6e61 6d65 506c  ..        namePl
+000034e0: 6174 6544 7261 7720 3d20 496d 6167 6544  ateDraw = ImageD
+000034f0: 7261 772e 4472 6177 286e 616d 6550 6c61  raw.Draw(namePla
+00003500: 7465 496d 6729 0d0a 2020 2020 2020 2020  teImg)..        
+00003510: 666f 6e74 3120 3d20 496d 6167 6546 6f6e  font1 = ImageFon
+00003520: 742e 7472 7565 7479 7065 2853 5441 5449  t.truetype(STATI
+00003530: 4320 2b20 272f 6d73 7968 2e74 7463 272c  C + '/msyh.ttc',
+00003540: 2032 382c 2065 6e63 6f64 696e 673d 2775   28, encoding='u
+00003550: 6e69 6327 290d 0a20 2020 2020 2020 206e  nic')..        n
+00003560: 616d 6550 6c61 7465 4472 6177 2e74 6578  amePlateDraw.tex
+00003570: 7428 2831 322c 2034 292c 2027 2027 2e6a  t((12, 4), ' '.j
+00003580: 6f69 6e28 6c69 7374 2873 656c 662e 7573  oin(list(self.us
+00003590: 6572 4e61 6d65 2929 2c20 2762 6c61 636b  erName)), 'black
+000035a0: 272c 2066 6f6e 7431 290d 0a20 2020 2020  ', font1)..     
+000035b0: 2020 206e 616d 6544 7849 6d67 203d 2049     nameDxImg = I
+000035c0: 6d61 6765 2e6f 7065 6e28 7365 6c66 2e70  mage.open(self.p
+000035d0: 6963 5f64 6972 202b 2027 5549 5f43 4d4e  ic_dir + 'UI_CMN
+000035e0: 5f4e 616d 655f 4458 2e70 6e67 2729 2e63  _Name_DX.png').c
+000035f0: 6f6e 7665 7274 2827 5247 4241 2729 0d0a  onvert('RGBA')..
+00003600: 2020 2020 2020 2020 6e61 6d65 4478 496d          nameDxIm
+00003610: 6720 3d20 7365 6c66 2e5f 7265 7369 7a65  g = self._resize
+00003620: 5069 6328 6e61 6d65 4478 496d 672c 2030  Pic(nameDxImg, 0
+00003630: 2e39 290d 0a20 2020 2020 2020 206e 616d  .9)..        nam
+00003640: 6550 6c61 7465 496d 672e 7061 7374 6528  ePlateImg.paste(
+00003650: 6e61 6d65 4478 496d 672c 2028 3233 302c  nameDxImg, (230,
+00003660: 2034 292c 206d 6173 6b3d 6e61 6d65 4478   4), mask=nameDx
+00003670: 496d 672e 7370 6c69 7428 295b 335d 290d  Img.split()[3]).
+00003680: 0a20 2020 2020 2020 2073 656c 662e 696d  .        self.im
+00003690: 672e 7061 7374 6528 6e61 6d65 506c 6174  g.paste(namePlat
+000036a0: 6549 6d67 2c20 2832 3430 2c20 3430 292c  eImg, (240, 40),
+000036b0: 206d 6173 6b3d 6e61 6d65 506c 6174 6549   mask=namePlateI
+000036c0: 6d67 2e73 706c 6974 2829 5b33 5d29 0d0a  mg.split()[3])..
+000036d0: 0d0a 2020 2020 2020 2020 7368 6f75 676f  ..        shougo
+000036e0: 7549 6d67 203d 2049 6d61 6765 2e6f 7065  uImg = Image.ope
+000036f0: 6e28 7365 6c66 2e70 6963 5f64 6972 202b  n(self.pic_dir +
+00003700: 2027 5549 5f43 4d4e 5f53 686f 7567 6f75   'UI_CMN_Shougou
+00003710: 5f52 6169 6e62 6f77 2e70 6e67 2729 2e63  _Rainbow.png').c
+00003720: 6f6e 7665 7274 2827 5247 4241 2729 0d0a  onvert('RGBA')..
+00003730: 2020 2020 2020 2020 7368 6f75 676f 7544          shougouD
+00003740: 7261 7720 3d20 496d 6167 6544 7261 772e  raw = ImageDraw.
+00003750: 4472 6177 2873 686f 7567 6f75 496d 6729  Draw(shougouImg)
+00003760: 0d0a 2020 2020 2020 2020 666f 6e74 3220  ..        font2 
+00003770: 3d20 496d 6167 6546 6f6e 742e 7472 7565  = ImageFont.true
+00003780: 7479 7065 2853 5441 5449 4320 2b20 272f  type(STATIC + '/
+00003790: 6164 6f62 655f 7369 6d68 6569 2e6f 7466  adobe_simhei.otf
+000037a0: 272c 2031 342c 2065 6e63 6f64 696e 673d  ', 14, encoding=
+000037b0: 2775 7466 2d38 2729 0d0a 2020 2020 2020  'utf-8')..      
+000037c0: 2020 706c 6179 436f 756e 7449 6e66 6f20    playCountInfo 
+000037d0: 3d20 6627 5344 3a20 7b73 656c 662e 7364  = f'SD: {self.sd
+000037e0: 5261 7469 6e67 7d20 2b20 4458 3a20 7b73  Rating} + DX: {s
+000037f0: 656c 662e 6478 5261 7469 6e67 7d20 3d20  elf.dxRating} = 
+00003800: 7b73 656c 662e 706c 6179 6572 5261 7469  {self.playerRati
+00003810: 6e67 7d27 0d0a 2020 2020 2020 2020 7368  ng}'..        sh
+00003820: 6f75 676f 7549 6d67 572c 2073 686f 7567  ougouImgW, shoug
+00003830: 6f75 496d 6748 203d 2073 686f 7567 6f75  ouImgH = shougou
+00003840: 496d 672e 7369 7a65 0d0a 2020 2020 2020  Img.size..      
+00003850: 2020 706c 6179 436f 756e 7449 6e66 6f57    playCountInfoW
+00003860: 2c20 706c 6179 436f 756e 7449 6e66 6f48  , playCountInfoH
+00003870: 203d 2073 686f 7567 6f75 4472 6177 2e74   = shougouDraw.t
+00003880: 6578 7473 697a 6528 706c 6179 436f 756e  extsize(playCoun
+00003890: 7449 6e66 6f2c 2066 6f6e 7432 290d 0a20  tInfo, font2).. 
+000038a0: 2020 2020 2020 2074 6578 7450 6f73 203d         textPos =
+000038b0: 2028 2873 686f 7567 6f75 496d 6757 202d   ((shougouImgW -
+000038c0: 2070 6c61 7943 6f75 6e74 496e 666f 5720   playCountInfoW 
+000038d0: 2d20 666f 6e74 322e 6765 746f 6666 7365  - font2.getoffse
+000038e0: 7428 706c 6179 436f 756e 7449 6e66 6f29  t(playCountInfo)
+000038f0: 5b30 5d29 202f 2032 2c20 3529 0d0a 2020  [0]) / 2, 5)..  
+00003900: 2020 2020 2020 7368 6f75 676f 7544 7261        shougouDra
+00003910: 772e 7465 7874 2828 7465 7874 506f 735b  w.text((textPos[
+00003920: 305d 202d 2031 2c20 7465 7874 506f 735b  0] - 1, textPos[
+00003930: 315d 292c 2070 6c61 7943 6f75 6e74 496e  1]), playCountIn
+00003940: 666f 2c20 2762 6c61 636b 272c 2066 6f6e  fo, 'black', fon
+00003950: 7432 290d 0a20 2020 2020 2020 2073 686f  t2)..        sho
+00003960: 7567 6f75 4472 6177 2e74 6578 7428 2874  ugouDraw.text((t
+00003970: 6578 7450 6f73 5b30 5d20 2b20 312c 2074  extPos[0] + 1, t
+00003980: 6578 7450 6f73 5b31 5d29 2c20 706c 6179  extPos[1]), play
+00003990: 436f 756e 7449 6e66 6f2c 2027 626c 6163  CountInfo, 'blac
+000039a0: 6b27 2c20 666f 6e74 3229 0d0a 2020 2020  k', font2)..    
+000039b0: 2020 2020 7368 6f75 676f 7544 7261 772e      shougouDraw.
+000039c0: 7465 7874 2828 7465 7874 506f 735b 305d  text((textPos[0]
+000039d0: 2c20 7465 7874 506f 735b 315d 202d 2031  , textPos[1] - 1
+000039e0: 292c 2070 6c61 7943 6f75 6e74 496e 666f  ), playCountInfo
+000039f0: 2c20 2762 6c61 636b 272c 2066 6f6e 7432  , 'black', font2
+00003a00: 290d 0a20 2020 2020 2020 2073 686f 7567  )..        shoug
+00003a10: 6f75 4472 6177 2e74 6578 7428 2874 6578  ouDraw.text((tex
+00003a20: 7450 6f73 5b30 5d2c 2074 6578 7450 6f73  tPos[0], textPos
+00003a30: 5b31 5d20 2b20 3129 2c20 706c 6179 436f  [1] + 1), playCo
+00003a40: 756e 7449 6e66 6f2c 2027 626c 6163 6b27  untInfo, 'black'
+00003a50: 2c20 666f 6e74 3229 0d0a 2020 2020 2020  , font2)..      
+00003a60: 2020 7368 6f75 676f 7544 7261 772e 7465    shougouDraw.te
+00003a70: 7874 2828 7465 7874 506f 735b 305d 202d  xt((textPos[0] -
+00003a80: 2031 2c20 7465 7874 506f 735b 315d 202d   1, textPos[1] -
+00003a90: 2031 292c 2070 6c61 7943 6f75 6e74 496e   1), playCountIn
+00003aa0: 666f 2c20 2762 6c61 636b 272c 2066 6f6e  fo, 'black', fon
+00003ab0: 7432 290d 0a20 2020 2020 2020 2073 686f  t2)..        sho
+00003ac0: 7567 6f75 4472 6177 2e74 6578 7428 2874  ugouDraw.text((t
+00003ad0: 6578 7450 6f73 5b30 5d20 2b20 312c 2074  extPos[0] + 1, t
+00003ae0: 6578 7450 6f73 5b31 5d20 2d20 3129 2c20  extPos[1] - 1), 
+00003af0: 706c 6179 436f 756e 7449 6e66 6f2c 2027  playCountInfo, '
+00003b00: 626c 6163 6b27 2c20 666f 6e74 3229 0d0a  black', font2)..
+00003b10: 2020 2020 2020 2020 7368 6f75 676f 7544          shougouD
+00003b20: 7261 772e 7465 7874 2828 7465 7874 506f  raw.text((textPo
+00003b30: 735b 305d 202d 2031 2c20 7465 7874 506f  s[0] - 1, textPo
+00003b40: 735b 315d 202b 2031 292c 2070 6c61 7943  s[1] + 1), playC
+00003b50: 6f75 6e74 496e 666f 2c20 2762 6c61 636b  ountInfo, 'black
+00003b60: 272c 2066 6f6e 7432 290d 0a20 2020 2020  ', font2)..     
+00003b70: 2020 2073 686f 7567 6f75 4472 6177 2e74     shougouDraw.t
+00003b80: 6578 7428 2874 6578 7450 6f73 5b30 5d20  ext((textPos[0] 
+00003b90: 2b20 312c 2074 6578 7450 6f73 5b31 5d20  + 1, textPos[1] 
+00003ba0: 2b20 3129 2c20 706c 6179 436f 756e 7449  + 1), playCountI
+00003bb0: 6e66 6f2c 2027 626c 6163 6b27 2c20 666f  nfo, 'black', fo
+00003bc0: 6e74 3229 0d0a 2020 2020 2020 2020 7368  nt2)..        sh
+00003bd0: 6f75 676f 7544 7261 772e 7465 7874 2874  ougouDraw.text(t
+00003be0: 6578 7450 6f73 2c20 706c 6179 436f 756e  extPos, playCoun
+00003bf0: 7449 6e66 6f2c 2027 7768 6974 6527 2c20  tInfo, 'white', 
+00003c00: 666f 6e74 3229 0d0a 2020 2020 2020 2020  font2)..        
+00003c10: 7368 6f75 676f 7549 6d67 203d 2073 656c  shougouImg = sel
+00003c20: 662e 5f72 6573 697a 6550 6963 2873 686f  f._resizePic(sho
+00003c30: 7567 6f75 496d 672c 2031 2e30 3529 0d0a  ugouImg, 1.05)..
+00003c40: 2020 2020 2020 2020 7365 6c66 2e69 6d67          self.img
+00003c50: 2e70 6173 7465 2873 686f 7567 6f75 496d  .paste(shougouIm
+00003c60: 672c 2028 3234 302c 2038 3329 2c20 6d61  g, (240, 83), ma
+00003c70: 736b 3d73 686f 7567 6f75 496d 672e 7370  sk=shougouImg.sp
+00003c80: 6c69 7428 295b 335d 290d 0a0d 0a20 2020  lit()[3])....   
+00003c90: 2020 2020 2073 656c 662e 5f64 7261 7742       self._drawB
+00003ca0: 6573 744c 6973 7428 7365 6c66 2e69 6d67  estList(self.img
+00003cb0: 2c20 7365 6c66 2e73 6442 6573 742c 2073  , self.sdBest, s
+00003cc0: 656c 662e 6478 4265 7374 290d 0a0d 0a20  elf.dxBest).... 
+00003cd0: 2020 2020 2020 2061 7574 686f 7242 6f61         authorBoa
+00003ce0: 7264 496d 6720 3d20 496d 6167 652e 6f70  rdImg = Image.op
+00003cf0: 656e 2873 656c 662e 7069 635f 6469 7220  en(self.pic_dir 
+00003d00: 2b20 2755 495f 434d 4e5f 4d69 6e69 4469  + 'UI_CMN_MiniDi
+00003d10: 616c 6f67 5f30 312e 706e 6727 292e 636f  alog_01.png').co
+00003d20: 6e76 6572 7428 2752 4742 4127 290d 0a20  nvert('RGBA').. 
+00003d30: 2020 2020 2020 2061 7574 686f 7242 6f61         authorBoa
+00003d40: 7264 496d 6720 3d20 7365 6c66 2e5f 7265  rdImg = self._re
+00003d50: 7369 7a65 5069 6328 6175 7468 6f72 426f  sizePic(authorBo
+00003d60: 6172 6449 6d67 2c20 302e 3335 290d 0a20  ardImg, 0.35).. 
+00003d70: 2020 2020 2020 2061 7574 686f 7242 6f61         authorBoa
+00003d80: 7264 4472 6177 203d 2049 6d61 6765 4472  rdDraw = ImageDr
+00003d90: 6177 2e44 7261 7728 6175 7468 6f72 426f  aw.Draw(authorBo
+00003da0: 6172 6449 6d67 290d 0a20 2020 2020 2020  ardImg)..       
+00003db0: 2061 7574 686f 7242 6f61 7264 4472 6177   authorBoardDraw
+00003dc0: 2e74 6578 7428 2833 312c 2032 3829 2c20  .text((31, 28), 
+00003dd0: 2720 2020 4765 6e65 7261 7465 6420 4279  '   Generated By
+00003de0: 5c6e 5879 6242 6f74 2026 2043 6869 7975  \nXybBot & Chiyu
+00003df0: 6b69 272c 2027 626c 6163 6b27 2c20 666f  ki', 'black', fo
+00003e00: 6e74 3229 0d0a 2020 2020 2020 2020 7365  nt2)..        se
+00003e10: 6c66 2e69 6d67 2e70 6173 7465 2861 7574  lf.img.paste(aut
+00003e20: 686f 7242 6f61 7264 496d 672c 2028 3132  horBoardImg, (12
+00003e30: 3234 2c20 3139 292c 206d 6173 6b3d 6175  24, 19), mask=au
+00003e40: 7468 6f72 426f 6172 6449 6d67 2e73 706c  thorBoardImg.spl
+00003e50: 6974 2829 5b33 5d29 0d0a 0d0a 2020 2020  it()[3])....    
+00003e60: 2020 2020 6478 496d 6720 3d20 496d 6167      dxImg = Imag
+00003e70: 652e 6f70 656e 2873 656c 662e 7069 635f  e.open(self.pic_
+00003e80: 6469 7220 2b20 2755 495f 5253 4c5f 4d42  dir + 'UI_RSL_MB
+00003e90: 6173 655f 5061 7274 735f 3031 2e70 6e67  ase_Parts_01.png
+00003ea0: 2729 2e63 6f6e 7665 7274 2827 5247 4241  ').convert('RGBA
+00003eb0: 2729 0d0a 2020 2020 2020 2020 7365 6c66  ')..        self
+00003ec0: 2e69 6d67 2e70 6173 7465 2864 7849 6d67  .img.paste(dxImg
+00003ed0: 2c20 2839 3838 2c20 3635 292c 206d 6173  , (988, 65), mas
+00003ee0: 6b3d 6478 496d 672e 7370 6c69 7428 295b  k=dxImg.split()[
+00003ef0: 335d 290d 0a20 2020 2020 2020 2073 6449  3])..        sdI
+00003f00: 6d67 203d 2049 6d61 6765 2e6f 7065 6e28  mg = Image.open(
+00003f10: 7365 6c66 2e70 6963 5f64 6972 202b 2027  self.pic_dir + '
+00003f20: 5549 5f52 534c 5f4d 4261 7365 5f50 6172  UI_RSL_MBase_Par
+00003f30: 7473 5f30 322e 706e 6727 292e 636f 6e76  ts_02.png').conv
+00003f40: 6572 7428 2752 4742 4127 290d 0a20 2020  ert('RGBA')..   
+00003f50: 2020 2020 2073 656c 662e 696d 672e 7061       self.img.pa
+00003f60: 7374 6528 7364 496d 672c 2028 3836 352c  ste(sdImg, (865,
+00003f70: 2036 3529 2c20 6d61 736b 3d73 6449 6d67   65), mask=sdImg
+00003f80: 2e73 706c 6974 2829 5b33 5d29 0d0a 0d0a  .split()[3])....
+00003f90: 2020 2020 2020 2020 2320 7365 6c66 2e69          # self.i
+00003fa0: 6d67 2e73 686f 7728 290d 0a0d 0a20 2020  mg.show()....   
+00003fb0: 2064 6566 2067 6574 4469 7228 7365 6c66   def getDir(self
+00003fc0: 293a 0d0a 2020 2020 2020 2020 7265 7475  ):..        retu
+00003fd0: 726e 2073 656c 662e 696d 670d 0a0d 0a0d  rn self.img.....
+00003fe0: 0a64 6566 2063 6f6d 7075 7465 5261 2864  .def computeRa(d
+00003ff0: 733a 2066 6c6f 6174 2c20 6163 6869 6576  s: float, achiev
+00004000: 656d 656e 743a 2066 6c6f 6174 2920 2d3e  ement: float) ->
+00004010: 2069 6e74 3a0d 0a20 2020 2062 6173 6552   int:..    baseR
+00004020: 6120 3d20 3232 2e34 200d 0a20 2020 2069  a = 22.4 ..    i
+00004030: 6620 6163 6869 6576 656d 656e 7420 3c20  f achievement < 
+00004040: 3530 3a0d 0a20 2020 2020 2020 2062 6173  50:..        bas
+00004050: 6552 6120 3d20 372e 300d 0a20 2020 2065  eRa = 7.0..    e
+00004060: 6c69 6620 6163 6869 6576 656d 656e 7420  lif achievement 
+00004070: 3c20 3630 3a0d 0a20 2020 2020 2020 2062  < 60:..        b
+00004080: 6173 6552 6120 3d20 382e 3020 0d0a 2020  aseRa = 8.0 ..  
+00004090: 2020 656c 6966 2061 6368 6965 7665 6d65    elif achieveme
+000040a0: 6e74 203c 2037 303a 0d0a 2020 2020 2020  nt < 70:..      
+000040b0: 2020 6261 7365 5261 203d 2039 2e36 200d    baseRa = 9.6 .
+000040c0: 0a20 2020 2065 6c69 6620 6163 6869 6576  .    elif achiev
+000040d0: 656d 656e 7420 3c20 3735 3a0d 0a20 2020  ement < 75:..   
+000040e0: 2020 2020 2062 6173 6552 6120 3d20 3131       baseRa = 11
+000040f0: 2e32 200d 0a20 2020 2065 6c69 6620 6163  .2 ..    elif ac
+00004100: 6869 6576 656d 656e 7420 3c20 3830 3a0d  hievement < 80:.
+00004110: 0a20 2020 2020 2020 2062 6173 6552 6120  .        baseRa 
+00004120: 3d20 3132 2e30 200d 0a20 2020 2065 6c69  = 12.0 ..    eli
+00004130: 6620 6163 6869 6576 656d 656e 7420 3c20  f achievement < 
+00004140: 3930 3a0d 0a20 2020 2020 2020 2062 6173  90:..        bas
+00004150: 6552 6120 3d20 3133 2e36 200d 0a20 2020  eRa = 13.6 ..   
+00004160: 2065 6c69 6620 6163 6869 6576 656d 656e   elif achievemen
+00004170: 7420 3c20 3934 3a0d 0a20 2020 2020 2020  t < 94:..       
+00004180: 2062 6173 6552 6120 3d20 3135 2e32 200d   baseRa = 15.2 .
+00004190: 0a20 2020 2065 6c69 6620 6163 6869 6576  .    elif achiev
+000041a0: 656d 656e 7420 3c20 3937 3a0d 0a20 2020  ement < 97:..   
+000041b0: 2020 2020 2062 6173 6552 6120 3d20 3136       baseRa = 16
+000041c0: 2e38 200d 0a20 2020 2065 6c69 6620 6163  .8 ..    elif ac
+000041d0: 6869 6576 656d 656e 7420 3c20 3938 3a0d  hievement < 98:.
+000041e0: 0a20 2020 2020 2020 2062 6173 6552 6120  .        baseRa 
+000041f0: 3d20 3230 2e30 200d 0a20 2020 2065 6c69  = 20.0 ..    eli
+00004200: 6620 6163 6869 6576 656d 656e 7420 3c20  f achievement < 
+00004210: 3939 3a0d 0a20 2020 2020 2020 2062 6173  99:..        bas
+00004220: 6552 6120 3d20 3230 2e33 0d0a 2020 2020  eRa = 20.3..    
+00004230: 656c 6966 2061 6368 6965 7665 6d65 6e74  elif achievement
+00004240: 203c 2039 392e 353a 0d0a 2020 2020 2020   < 99.5:..      
+00004250: 2020 6261 7365 5261 203d 2032 302e 3820    baseRa = 20.8 
+00004260: 0d0a 2020 2020 656c 6966 2061 6368 6965  ..    elif achie
+00004270: 7665 6d65 6e74 203c 2031 3030 3a0d 0a20  vement < 100:.. 
+00004280: 2020 2020 2020 2062 6173 6552 6120 3d20         baseRa = 
+00004290: 3231 2e31 200d 0a20 2020 2065 6c69 6620  21.1 ..    elif 
+000042a0: 6163 6869 6576 656d 656e 7420 3c20 3130  achievement < 10
+000042b0: 302e 353a 0d0a 2020 2020 2020 2020 6261  0.5:..        ba
+000042c0: 7365 5261 203d 2032 312e 3620 0d0a 0d0a  seRa = 21.6 ....
+000042d0: 2020 2020 7265 7475 726e 206d 6174 682e      return math.
+000042e0: 666c 6f6f 7228 6473 202a 2028 6d69 6e28  floor(ds * (min(
+000042f0: 3130 302e 352c 2061 6368 6965 7665 6d65  100.5, achieveme
+00004300: 6e74 2920 2f20 3130 3029 202a 2062 6173  nt) / 100) * bas
+00004310: 6552 6129 0d0a 0d0a 0d0a 6173 796e 6320  eRa)......async 
+00004320: 6465 6620 6765 6e65 7261 7465 3530 2870  def generate50(p
+00004330: 6179 6c6f 6164 3a20 4469 6374 2920 2d3e  ayload: Dict) ->
+00004340: 2054 7570 6c65 5b4f 7074 696f 6e61 6c5b   Tuple[Optional[
+00004350: 496d 6167 652e 496d 6167 655d 2c20 626f  Image.Image], bo
+00004360: 6f6c 5d3a 0d0a 2020 2020 6173 796e 6320  ol]:..    async 
+00004370: 7769 7468 2061 696f 6874 7470 2e72 6571  with aiohttp.req
+00004380: 7565 7374 2822 504f 5354 222c 2022 6874  uest("POST", "ht
+00004390: 7470 733a 2f2f 7777 772e 6469 7669 6e67  tps://www.diving
+000043a0: 2d66 6973 682e 636f 6d2f 6170 692f 6d61  -fish.com/api/ma
+000043b0: 696d 6169 6478 7072 6f62 6572 2f71 7565  imaidxprober/que
+000043c0: 7279 2f70 6c61 7965 7222 2c20 6a73 6f6e  ry/player", json
+000043d0: 3d70 6179 6c6f 6164 2920 6173 2072 6573  =payload) as res
+000043e0: 703a 0d0a 2020 2020 2020 2020 6966 2072  p:..        if r
+000043f0: 6573 702e 7374 6174 7573 203d 3d20 3430  esp.status == 40
+00004400: 303a 0d0a 2020 2020 2020 2020 2020 2020  0:..            
+00004410: 7265 7475 726e 204e 6f6e 652c 2034 3030  return None, 400
+00004420: 0d0a 2020 2020 2020 2020 6966 2072 6573  ..        if res
+00004430: 702e 7374 6174 7573 203d 3d20 3430 333a  p.status == 403:
+00004440: 0d0a 2020 2020 2020 2020 2020 2020 7265  ..            re
+00004450: 7475 726e 204e 6f6e 652c 2034 3033 0d0a  turn None, 403..
+00004460: 2020 2020 2020 2020 7364 5f62 6573 7420          sd_best 
+00004470: 3d20 4265 7374 4c69 7374 2833 3529 0d0a  = BestList(35)..
+00004480: 2020 2020 2020 2020 6478 5f62 6573 7420          dx_best 
+00004490: 3d20 4265 7374 4c69 7374 2831 3529 0d0a  = BestList(15)..
+000044a0: 2020 2020 2020 2020 6f62 6a20 3d20 6177          obj = aw
+000044b0: 6169 7420 7265 7370 2e6a 736f 6e28 290d  ait resp.json().
+000044c0: 0a20 2020 2020 2020 2064 783a 204c 6973  .        dx: Lis
+000044d0: 745b 4469 6374 5d20 3d20 6f62 6a5b 2263  t[Dict] = obj["c
+000044e0: 6861 7274 7322 5d5b 2264 7822 5d0d 0a20  harts"]["dx"].. 
+000044f0: 2020 2020 2020 2073 643a 204c 6973 745b         sd: List[
+00004500: 4469 6374 5d20 3d20 6f62 6a5b 2263 6861  Dict] = obj["cha
+00004510: 7274 7322 5d5b 2273 6422 5d0d 0a20 2020  rts"]["sd"]..   
+00004520: 2020 2020 2066 6f72 2063 2069 6e20 7364       for c in sd
+00004530: 3a0d 0a20 2020 2020 2020 2020 2020 2073  :..            s
+00004540: 645f 6265 7374 2e70 7573 6828 4368 6172  d_best.push(Char
+00004550: 7449 6e66 6f2e 6672 6f6d 5f6a 736f 6e28  tInfo.from_json(
+00004560: 6329 290d 0a20 2020 2020 2020 2066 6f72  c))..        for
+00004570: 2063 2069 6e20 6478 3a0d 0a20 2020 2020   c in dx:..     
+00004580: 2020 2020 2020 2064 785f 6265 7374 2e70         dx_best.p
+00004590: 7573 6828 4368 6172 7449 6e66 6f2e 6672  ush(ChartInfo.fr
+000045a0: 6f6d 5f6a 736f 6e28 6329 290d 0a20 2020  om_json(c))..   
+000045b0: 2020 2020 2070 6963 203d 2044 7261 7742       pic = DrawB
+000045c0: 6573 7428 7364 5f62 6573 742c 2064 785f  est(sd_best, dx_
+000045d0: 6265 7374 2c20 6f62 6a5b 226e 6963 6b6e  best, obj["nickn
+000045e0: 616d 6522 5d29 2e67 6574 4469 7228 290d  ame"]).getDir().
+000045f0: 0a20 2020 2020 2020 2072 6574 7572 6e20  .        return 
+00004600: 7069 632c 2030 0d0a                      pic, 0..
```

### Comparing `nonebot_plugin_maimai-0.1.3/nonebot_plugin_maimai/libraries/maimaidx_music.py` & `nonebot_plugin_maimai-0.2.0/nonebot_plugin_maimai/libraries/maimaidx_music.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,19 +1,19 @@
 
 import random
 from typing import Dict, List, Optional, Union, Tuple, Any
 from copy import deepcopy
 
-import httpx
+import aiohttp,asyncio
 
-def get_cover_len4_id(mid) -> str:
+def get_cover_len5_id(mid) -> str:
     mid = int(mid)
-    if 10001 <= mid:
+    if mid > 10000 and mid <= 11000:
         mid -= 10000
-    return f'{mid:04d}'
+    return f'{mid:05d}'
 
 def cross(checker: List[Any], elem: Optional[Union[Any, List[Any]]], diff):
     ret = False
     diff_ret = []
     if not elem or elem is Ellipsis:
         return True, diff
     if isinstance(elem, List):
@@ -147,13 +147,23 @@
             if title_search is not Ellipsis and title_search.lower() not in music.title.lower():
                 continue
             music.diff = diff2
             new_list.append(music)
         return new_list
 
 
-obj = httpx.get('https://www.diving-fish.com/api/maimaidxprober/music_data').json()
-total_list: MusicList = MusicList(obj)
-for __i in range(len(total_list)):
-    total_list[__i] = Music(total_list[__i])
-    for __j in range(len(total_list[__i].charts)):
-        total_list[__i].charts[__j] = Chart(total_list[__i].charts[__j])
+async def main():
+    global obj,total_list
+    async def fetch_json(url):
+        async with aiohttp.ClientSession() as session:
+            async with session.get(url) as response:
+                return await response.json()
+
+    obj = await fetch_json('https://www.diving-fish.com/api/maimaidxprober/music_data')
+    total_list = MusicList(obj)
+    for __i in range(len(total_list)):
+        total_list[__i] = Music(total_list[__i])
+        for __j in range(len(total_list[__i].charts)):
+            total_list[__i].charts[__j] = Chart(total_list[__i].charts[__j])
+    
+asyncio.run(main())
+
```

### Comparing `nonebot_plugin_maimai-0.1.3/nonebot_plugin_maimai/public.py` & `nonebot_plugin_maimai-0.2.0/nonebot_plugin_maimai/public.py`

 * *Files 4% similar despite different names*

```diff
@@ -7,15 +7,15 @@
 from nonebot import get_driver
 from nonebot.params import CommandArg
 from nonebot.matcher import Matcher
 from .libraries.image import *
 
 from bs4 import BeautifulSoup
 from typing import Dict,List
-import httpx
+import aiohttp
 from io import BytesIO
 import json
 
 try:
     maimai_font: str = get_driver().config.maimai_font
 except:
     maimai_font: str = 'simsun.ttc'
@@ -79,24 +79,29 @@
     tag = tag.extract_plain_text()
     if tag.isdigit() and int(tag) in range(1, 10):
         msg:List[Dict[str,Dict[str,str]]] = state['msg']
         Url = msg[int(tag)-1]['url']['视频链接:']
         print(msg[int(tag)-1])
         await matcher.finish(Url)
     
+async def fetch_page(url, headers):
+    async with aiohttp.ClientSession(headers=headers) as session:
+        async with session.get(url) as response:
+            return await response.text()    
     
 async def get_target(keyword:str):
     headers = {
     'User-Agent':
         'Mozilla/5.0 (Windows NT 10.0; Win64; x64) AppleWebKit/537.36 (KHTML, like Gecko) Chrome/111.0.0.0 Safari/537.36 Edg/111.0.1661.62',
     'cookie': b_cookie
     }
 
     mainUrl='https://search.bilibili.com/all?keyword='+keyword
-    mainSoup = BeautifulSoup(httpx.get(url = mainUrl, headers= headers).text, "html.parser")
+    content = await fetch_page(mainUrl, headers)
+    mainSoup = BeautifulSoup(content, "html.parser")
     viedoNum = 1
     msg_list = []
     for item in mainSoup.find_all('div',class_="bili-video-card"):
         item:BeautifulSoup
         msg = {'data':{},'url':{}}
         # try:
         msg['data']['序号:'] = '第'+ viedoNum.__str__() + '个视频:'
@@ -151,19 +156,19 @@
     for msg in msg_list:
         data = msg['data']
         url = msg['url']
         data_list.append((url, data))
 
     for i, (url, data) in enumerate(data_list):
         # 将图片缩放并插入到格子中
-        response = httpx.get(url = url['封面:'],headers= {
-        'User-Agent':
-        'Mozilla/5.0 (Windows NT 10.0; Win64; x64) AppleWebKit/537.36 (KHTML, like Gecko) Chrome/111.0.0.0 Safari/537.36 Edg/111.0.1661.62',
-    })
-        image = Image.open(BytesIO(response.content))
+        image_content = await fetch_page(url['封面:'], headers={
+            'User-Agent':
+                'Mozilla/5.0 (Windows NT 10.0; Win64; x64) AppleWebKit/537.36 (KHTML, like Gecko) Chrome/111.0.0.0 Safari/537.36 Edg/111.0.1661.62',
+        })
+        image = Image.open(BytesIO(image_content))
         img_width, img_height = image.size
         ratio = min(cell_width/img_width, cell_height/img_height)
         new_width = int(img_width*ratio)
         new_height = int(img_height*ratio)
         image = image.resize((new_width, new_height), Image.ANTIALIAS)
         img_x = ((i % cols) * cell_width) + ((cell_width - new_width) // 2)
         img_y = ((i // cols) * cell_height) + ((cell_height - new_height-200) // 2)
```

### Comparing `nonebot_plugin_maimai-0.1.3/pyproject.toml` & `nonebot_plugin_maimai-0.2.0/pyproject.toml`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "nonebot_plugin_maimai"
-version = "0.1.3"
+version = "0.2.0"
 description= "Maimai DX plugin for NoneBot"
 authors = ["Agnes_Digital <Z735803792@163.com>"]
 license = "MIT"
 readme = "README.md"
 homepage = "https://github.com/Umamusume-Agnes-Digital/nonebot_plugin_maimai"
 repository = "https://github.com/Umamusume-Agnes-Digital/nonebot_plugin_maimai"
 keywords = ["maimai", "nonebot2", "plugin"]
@@ -18,20 +18,19 @@
 
 ]
 include = [
     "LICENSE","README.md"
 ]
  
 [tool.poetry.dependencies]
-python = "^3.8"
-aiohttp = "^3.8.1"
-nonebot2 = "^2.0.0rc4"
+python = "^3.9"
+aiohttp = "^3.8.3"
+nonebot2 = "^2.0.0"
 nonebot-adapter-onebot = ">=2.1.3"
 pillow = ">=9.3.0"
-httpx = ">=0.23.0"
 nonebot-plugin-txt2img = "^0.3.0"
 bs4 = "^0.0.1"
  
 [tool.poetry.dev-dependencies]
  
 [build-system]
 requires = ["poetry-core>=1.0.0"]
```

### Comparing `nonebot_plugin_maimai-0.1.3/README.md` & `nonebot_plugin_maimai-0.2.0/README.md`

 * *Files 0% similar despite different names*

```diff
@@ -20,15 +20,15 @@
 </a>
     <img src="https://img.shields.io/badge/python-3.7+-blue.svg" alt="python">
     <img src="https://img.shields.io/badge/nonebot-2.0.0rc1+-red.svg" alt="NoneBot">
 </div>
 
 ## 说明
 
-从[mai-bot](https://github.com/Diving-Fish/mai-bot)适配nonebot2插件，测试环境nonebot2.0.0rc1
+从[mai-bot](https://github.com/Diving-Fish/mai-bot)适配nonebot2插件，测试环境nonebot2.0.0
 
 修改部分：
  - b40/b50可以艾特人查询
  - static文件可以放maimai插件文件夹中，或机器人路径下/data/maimai/static
  - env设置 `maimai_font`和`b_cookie`,分别是str对象的`字体`和`cookie`
  - 新增指令`b站搜索[text]`
```

#### html2text {}

```diff
@@ -1,13 +1,13 @@
                              [NoneBotPluginLogo]
                               [NoneBotPluginText]
 # nonebot_plugin_maimai _â¨maimaiDXï¼nonebot2æä»¶çæ¬â¨_ [GitHub_stars]
               [GitHub_issues] [QQ_Chat_Group] [python] [NoneBot]
 ## è¯´æ ä»[mai-bot](https://github.com/Diving-Fish/mai-
-bot)éénonebot2æä»¶ï¼æµè¯ç¯å¢nonebot2.0.0rc1 ä¿®æ¹é¨åï¼ - b40/
+bot)éénonebot2æä»¶ï¼æµè¯ç¯å¢nonebot2.0.0 ä¿®æ¹é¨åï¼ - b40/
 b50å¯ä»¥è¾ç¹äººæ¥è¯¢ -
 staticæä»¶å¯ä»¥æ¾maimaiæä»¶æä»¶å¤¹ä¸­ï¼ææºå¨äººè·¯å¾ä¸/data/
 maimai/static - envè®¾ç½®
 `maimai_font`å`b_cookie`,åå«æ¯strå¯¹è±¡ç`å­ä½`å`cookie` -
 æ°å¢æä»¤`bç«æç´¢[text]`
 æåçééæé®é¢è¯·å²ææ¥ä¸è¦ææ°åä½èæï¼å¯ä»¥æissæè
 [å ç¾¤qq](https://jq.qq.com/?_wv=1027&k=l82tMuPG)åé¦, ##
```

### Comparing `nonebot_plugin_maimai-0.1.3/setup.py` & `nonebot_plugin_maimai-0.2.0/PKG-INFO`

 * *Files 15% similar despite different names*

```diff
@@ -1,36 +1,110 @@
-# -*- coding: utf-8 -*-
-from setuptools import setup
+Metadata-Version: 2.1
+Name: nonebot-plugin-maimai
+Version: 0.2.0
+Summary: Maimai DX plugin for NoneBot
+Home-page: https://github.com/Umamusume-Agnes-Digital/nonebot_plugin_maimai
+License: MIT
+Keywords: maimai,nonebot2,plugin
+Author: Agnes_Digital
+Author-email: Z735803792@163.com
+Requires-Python: >=3.9,<4.0
+Classifier: License :: OSI Approved :: MIT License
+Classifier: Operating System :: OS Independent
+Classifier: Programming Language :: Python
+Classifier: Programming Language :: Python :: 3
+Classifier: Programming Language :: Python :: 3.9
+Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
+Requires-Dist: aiohttp (>=3.8.3,<4.0.0)
+Requires-Dist: bs4 (>=0.0.1,<0.0.2)
+Requires-Dist: nonebot-adapter-onebot (>=2.1.3)
+Requires-Dist: nonebot-plugin-txt2img (>=0.3.0,<0.4.0)
+Requires-Dist: nonebot2 (>=2.0.0,<3.0.0)
+Requires-Dist: pillow (>=9.3.0)
+Project-URL: Repository, https://github.com/Umamusume-Agnes-Digital/nonebot_plugin_maimai
+Description-Content-Type: text/markdown
+
+<div align="center">
+  <img src="https://s2.loli.net/2022/06/16/opBDE8Swad5rU3n.png" width="180" height="180" alt="NoneBotPluginLogo">
+  <br>
+  <p><img src="https://s2.loli.net/2022/06/16/xsVUGRrkbn1ljTD.png" width="240" alt="NoneBotPluginText"></p>
+</div>
+
+<div align="center">
+
+# nonebot_plugin_maimai
+_✨maimaiDX，nonebot2插件版本✨_
+
+<a href="https://github.com/Umamusume-Agnes-Digital/nonebot_plugin_maimai/stargazers">
+        <img alt="GitHub stars" src="https://img.shields.io/github/stars/Umamusume-Agnes-Digital/nonebot_plugin_maimai" alt="stars">
+</a>
+<a href="https://github.com/Umamusume-Agnes-Digital/nonebot_plugin_maimai/issues">
+        <img alt="GitHub issues" src="https://img.shields.io/github/issues/Umamusume-Agnes-Digital/nonebot_plugin_maimai" alt="issues">
+</a>
+<a href="https://jq.qq.com/?_wv=1027&k=l82tMuPG">
+        <img src="https://img.shields.io/badge/QQ%E7%BE%A4-424506063-orange?style=flat-square" alt="QQ Chat Group">
+</a>
+    <img src="https://img.shields.io/badge/python-3.7+-blue.svg" alt="python">
+    <img src="https://img.shields.io/badge/nonebot-2.0.0rc1+-red.svg" alt="NoneBot">
+</div>
+
+## 说明
+
+从[mai-bot](https://github.com/Diving-Fish/mai-bot)适配nonebot2插件，测试环境nonebot2.0.0
+
+修改部分：
+ - b40/b50可以艾特人查询
+ - static文件可以放maimai插件文件夹中，或机器人路径下/data/maimai/static
+ - env设置 `maimai_font`和`b_cookie`,分别是str对象的`字体`和`cookie`
+ - 新增指令`b站搜索[text]`
+
+我做的适配有问题请冲我来不要打扰原作者捏，可以提iss或者[加群qq](https://jq.qq.com/?_wv=1027&k=l82tMuPG)反馈,
+
+## 前置步骤（和原项目一样）
+
+安装:
+
+    pip3 install nonebot_plugin_maimai
+    nb plugin install nonebot_plugin_maimai
+    # git clone 那我建议你还是用原作者的罢
+
+您需要从[此链接](https://www.diving-fish.com/maibot/static.zip)下载资源文件并，并将其static文件解压到:(以下方法2选1)
+
+ - pypi`nonebot_plugin_maimai`文件夹中 - 最终路径类似是/path/to/nonebot_plugin_maimai/static
+ - 机器人目录下 - 最终路径类似是/path/to/data/maimai/static中。其中bot.py文件在/path/to位置
+
+> 资源文件仅供学习交流使用，请自觉在下载 24 小时内删除资源文件。
+
+## FAQ
+
+配置 nonebot 或 cq-http 过程中出错？
+> 请查阅 https://github.com/nonebot/nonebot2 以及 https://github.com/Mrs4s/go-cqhttp 中的文档。
+
+部分消息发不出来？
+> 被风控了。解决方式：换号或者让这个号保持登陆状态和一定的聊天频率，持续一段时间。
+
+## 说明
+
+本 bot 提供了如下功能：
+
+命令 | 功能
+--- | ---
+help | 查看帮助文档
+今日舞萌 | 查看今天的舞萌运势
+XXXmaimaiXXX什么 | 随机一首歌
+随个[dx/标准][绿黄红紫白]<难度> | 随机一首指定条件的乐曲
+查歌<乐曲标题的一部分> | 查询符合条件的乐曲
+[绿黄红紫白]id<歌曲编号> | 查询乐曲信息或谱面信息
+定数查歌 <定数> <br> 定数查歌 <定数下限> <定数上限> |  查询定数对应的乐曲
+分数线 <难度+歌曲id> <分数线> | 展示歌曲的分数线
+
+## 原作者
 
-packages = \
-['nonebot_plugin_maimai', 'nonebot_plugin_maimai.libraries']
+[Diving-Fish](https://github.com/Diving-Fish),感谢大佬为音游人的无私奉献
 
-package_data = \
-{'': ['*']}
+## License
 
-install_requires = \
-['aiohttp>=3.8.1,<4.0.0',
- 'bs4>=0.0.1,<0.0.2',
- 'httpx>=0.23.0',
- 'nonebot-adapter-onebot>=2.1.3',
- 'nonebot-plugin-txt2img>=0.3.0,<0.4.0',
- 'nonebot2>=2.0.0rc4,<3.0.0',
- 'pillow>=9.3.0']
-
-setup_kwargs = {
-    'name': 'nonebot-plugin-maimai',
-    'version': '0.1.3',
-    'description': 'Maimai DX plugin for NoneBot',
-    'long_description': '<div align="center">\n  <img src="https://s2.loli.net/2022/06/16/opBDE8Swad5rU3n.png" width="180" height="180" alt="NoneBotPluginLogo">\n  <br>\n  <p><img src="https://s2.loli.net/2022/06/16/xsVUGRrkbn1ljTD.png" width="240" alt="NoneBotPluginText"></p>\n</div>\n\n<div align="center">\n\n# nonebot_plugin_maimai\n_✨maimaiDX，nonebot2插件版本✨_\n\n<a href="https://github.com/Umamusume-Agnes-Digital/nonebot_plugin_maimai/stargazers">\n        <img alt="GitHub stars" src="https://img.shields.io/github/stars/Umamusume-Agnes-Digital/nonebot_plugin_maimai" alt="stars">\n</a>\n<a href="https://github.com/Umamusume-Agnes-Digital/nonebot_plugin_maimai/issues">\n        <img alt="GitHub issues" src="https://img.shields.io/github/issues/Umamusume-Agnes-Digital/nonebot_plugin_maimai" alt="issues">\n</a>\n<a href="https://jq.qq.com/?_wv=1027&k=l82tMuPG">\n        <img src="https://img.shields.io/badge/QQ%E7%BE%A4-424506063-orange?style=flat-square" alt="QQ Chat Group">\n</a>\n    <img src="https://img.shields.io/badge/python-3.7+-blue.svg" alt="python">\n    <img src="https://img.shields.io/badge/nonebot-2.0.0rc1+-red.svg" alt="NoneBot">\n</div>\n\n## 说明\n\n从[mai-bot](https://github.com/Diving-Fish/mai-bot)适配nonebot2插件，测试环境nonebot2.0.0rc1\n\n修改部分：\n - b40/b50可以艾特人查询\n - static文件可以放maimai插件文件夹中，或机器人路径下/data/maimai/static\n - env设置 `maimai_font`和`b_cookie`,分别是str对象的`字体`和`cookie`\n - 新增指令`b站搜索[text]`\n\n我做的适配有问题请冲我来不要打扰原作者捏，可以提iss或者[加群qq](https://jq.qq.com/?_wv=1027&k=l82tMuPG)反馈,\n\n## 前置步骤（和原项目一样）\n\n安装:\n\n    pip3 install nonebot_plugin_maimai\n    nb plugin install nonebot_plugin_maimai\n    # git clone 那我建议你还是用原作者的罢\n\n您需要从[此链接](https://www.diving-fish.com/maibot/static.zip)下载资源文件并，并将其static文件解压到:(以下方法2选1)\n\n - pypi`nonebot_plugin_maimai`文件夹中 - 最终路径类似是/path/to/nonebot_plugin_maimai/static\n - 机器人目录下 - 最终路径类似是/path/to/data/maimai/static中。其中bot.py文件在/path/to位置\n\n> 资源文件仅供学习交流使用，请自觉在下载 24 小时内删除资源文件。\n\n## FAQ\n\n配置 nonebot 或 cq-http 过程中出错？\n> 请查阅 https://github.com/nonebot/nonebot2 以及 https://github.com/Mrs4s/go-cqhttp 中的文档。\n\n部分消息发不出来？\n> 被风控了。解决方式：换号或者让这个号保持登陆状态和一定的聊天频率，持续一段时间。\n\n## 说明\n\n本 bot 提供了如下功能：\n\n命令 | 功能\n--- | ---\nhelp | 查看帮助文档\n今日舞萌 | 查看今天的舞萌运势\nXXXmaimaiXXX什么 | 随机一首歌\n随个[dx/标准][绿黄红紫白]<难度> | 随机一首指定条件的乐曲\n查歌<乐曲标题的一部分> | 查询符合条件的乐曲\n[绿黄红紫白]id<歌曲编号> | 查询乐曲信息或谱面信息\n定数查歌 <定数> <br> 定数查歌 <定数下限> <定数上限> |  查询定数对应的乐曲\n分数线 <难度+歌曲id> <分数线> | 展示歌曲的分数线\n\n## 原作者\n\n[Diving-Fish](https://github.com/Diving-Fish),感谢大佬为音游人的无私奉献\n\n## License\n\nMIT\n\n您可以自由使用本项目的代码用于商业或非商业的用途，但必须附带 MIT 授权协议。\n',
-    'author': 'Agnes_Digital',
-    'author_email': 'Z735803792@163.com',
-    'maintainer': 'None',
-    'maintainer_email': 'None',
-    'url': 'https://github.com/Umamusume-Agnes-Digital/nonebot_plugin_maimai',
-    'packages': packages,
-    'package_data': package_data,
-    'install_requires': install_requires,
-    'python_requires': '>=3.8,<4.0',
-}
+MIT
 
+您可以自由使用本项目的代码用于商业或非商业的用途，但必须附带 MIT 授权协议。
 
-setup(**setup_kwargs)
```

#### html2text {}

```diff
@@ -1,56 +1,53 @@
-# -*- coding: utf-8 -*- from setuptools import setup packages = \
-['nonebot_plugin_maimai', 'nonebot_plugin_maimai.libraries'] package_data = \
-{'': ['*']} install_requires = \ ['aiohttp>=3.8.1,<4.0.0', 'bs4>=0.0.1,<0.0.2',
-'httpx>=0.23.0', 'nonebot-adapter-onebot>=2.1.3', 'nonebot-plugin-
-txt2img>=0.3.0,<0.4.0', 'nonebot2>=2.0.0rc4,<3.0.0', 'pillow>=9.3.0']
-setup_kwargs = { 'name': 'nonebot-plugin-maimai', 'version': '0.1.3',
-'description': 'Maimai DX plugin for NoneBot', 'long_description': '
-                           \n [NoneBotPluginLogo]\n
-                                      \n
+Metadata-Version: 2.1 Name: nonebot-plugin-maimai Version: 0.2.0 Summary:
+Maimai DX plugin for NoneBot Home-page: https://github.com/Umamusume-Agnes-
+Digital/nonebot_plugin_maimai License: MIT Keywords: maimai,nonebot2,plugin
+Author: Agnes_Digital Author-email: Z735803792@163.com Requires-Python:
+>=3.9,<4.0 Classifier: License :: OSI Approved :: MIT License Classifier:
+Operating System :: OS Independent Classifier: Programming Language :: Python
+Classifier: Programming Language :: Python :: 3 Classifier: Programming
+Language :: Python :: 3.9 Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11 Requires-Dist: aiohttp
+(>=3.8.3,<4.0.0) Requires-Dist: bs4 (>=0.0.1,<0.0.2) Requires-Dist: nonebot-
+adapter-onebot (>=2.1.3) Requires-Dist: nonebot-plugin-txt2img (>=0.3.0,<0.4.0)
+Requires-Dist: nonebot2 (>=2.0.0,<3.0.0) Requires-Dist: pillow (>=9.3.0)
+Project-URL: Repository, https://github.com/Umamusume-Agnes-Digital/
+nonebot_plugin_maimai Description-Content-Type: text/markdown
+                             [NoneBotPluginLogo]
                               [NoneBotPluginText]
-                                      \n
-\n\n
-  \n\n# nonebot_plugin_maimai\n_â¨maimaiDXï¼nonebot2æä»¶çæ¬â¨_\n\n\n_
-  [GitHub_stars]\n\n\n_[GitHub_issues]\n\n\n_[QQ_Chat_Group]\n\n [python]\n
-                                  [NoneBot]\n
-\n\n## è¯´æ\n\nä»[mai-bot](https://github.com/Diving-Fish/mai-
-bot)éénonebot2æä»¶ï¼æµè¯ç¯å¢nonebot2.0.0rc1\n\nä¿®æ¹é¨åï¼\n -
-b40/b50å¯ä»¥è¾ç¹äººæ¥è¯¢\n -
+# nonebot_plugin_maimai _â¨maimaiDXï¼nonebot2æä»¶çæ¬â¨_ [GitHub_stars]
+              [GitHub_issues] [QQ_Chat_Group] [python] [NoneBot]
+## è¯´æ ä»[mai-bot](https://github.com/Diving-Fish/mai-
+bot)éénonebot2æä»¶ï¼æµè¯ç¯å¢nonebot2.0.0 ä¿®æ¹é¨åï¼ - b40/
+b50å¯ä»¥è¾ç¹äººæ¥è¯¢ -
 staticæä»¶å¯ä»¥æ¾maimaiæä»¶æä»¶å¤¹ä¸­ï¼ææºå¨äººè·¯å¾ä¸/data/
-maimai/static\n - envè®¾ç½®
-`maimai_font`å`b_cookie`,åå«æ¯strå¯¹è±¡ç`å­ä½`å`cookie`\n -
-æ°å¢æä»¤`bç«æç´¢
-[text]`\n\næåçééæé®é¢è¯·å²ææ¥ä¸è¦ææ°åä½èæï¼å¯ä»¥æissæè
-[å ç¾¤qq](https://jq.qq.com/?_wv=1027&k=l82tMuPG)åé¦,\n\n##
-åç½®æ­¥éª¤ï¼ååé¡¹ç®ä¸æ ·ï¼\n\nå®è£:\n\n pip3 install
-nonebot_plugin_maimai\n nb plugin install nonebot_plugin_maimai\n # git clone
-é£æå»ºè®®ä½ è¿æ¯ç¨åä½èçç½¢\n\næ¨éè¦ä»[æ­¤é¾æ¥](https://
+maimai/static - envè®¾ç½®
+`maimai_font`å`b_cookie`,åå«æ¯strå¯¹è±¡ç`å­ä½`å`cookie` -
+æ°å¢æä»¤`bç«æç´¢[text]`
+æåçééæé®é¢è¯·å²ææ¥ä¸è¦ææ°åä½èæï¼å¯ä»¥æissæè
+[å ç¾¤qq](https://jq.qq.com/?_wv=1027&k=l82tMuPG)åé¦, ##
+åç½®æ­¥éª¤ï¼ååé¡¹ç®ä¸æ ·ï¼ å®è£: pip3 install nonebot_plugin_maimai
+nb plugin install nonebot_plugin_maimai # git clone
+é£æå»ºè®®ä½ è¿æ¯ç¨åä½èçç½¢ æ¨éè¦ä»[æ­¤é¾æ¥](https://
 www.diving-fish.com/maibot/
 static.zip)ä¸è½½èµæºæä»¶å¹¶ï¼å¹¶å°å¶staticæä»¶è§£åå°:
-(ä»¥ä¸æ¹æ³2é1)\n\n - pypi`nonebot_plugin_maimai`æä»¶å¤¹ä¸­ -
-æç»è·¯å¾ç±»ä¼¼æ¯/path/to/nonebot_plugin_maimai/static\n -
-æºå¨äººç®å½ä¸ - æç»è·¯å¾ç±»ä¼¼æ¯/path/to/data/maimai/
-staticä¸­ãå¶ä¸­bot.pyæä»¶å¨/path/toä½ç½®\n\n>
-èµæºæä»¶ä»ä¾å­¦ä¹ äº¤æµä½¿ç¨ï¼è¯·èªè§å¨ä¸è½½ 24
-å°æ¶åå é¤èµæºæä»¶ã\n\n## FAQ\n\néç½® nonebot æ cq-http
-è¿ç¨ä¸­åºéï¼\n> è¯·æ¥é https://github.com/nonebot/nonebot2 ä»¥å
-https://github.com/Mrs4s/go-cqhttp
-ä¸­çææ¡£ã\n\né¨åæ¶æ¯åä¸åºæ¥ï¼\n>
-è¢«é£æ§äºãè§£å³æ¹å¼ï¼æ¢å·æèè®©è¿ä¸ªå·ä¿æç»éç¶æåä¸å®çèå¤©é¢çï¼æç»­ä¸æ®µæ¶é´ã\n\n##
-è¯´æ\n\næ¬ bot æä¾äºå¦ä¸åè½ï¼\n\nå½ä»¤ | åè½\n--- | ---\nhelp
-| æ¥çå¸®å©ææ¡£\nä»æ¥èè |
-æ¥çä»å¤©çèèè¿å¿\nXXXmaimaiXXXä»ä¹ | éæºä¸é¦æ­\néä¸ª[dx/
-æ å][ç»¿é»çº¢ç´«ç½]<é¾åº¦> |
-éæºä¸é¦æå®æ¡ä»¶çä¹æ²\næ¥æ­<ä¹æ²æ é¢çä¸é¨å> |
-æ¥è¯¢ç¬¦åæ¡ä»¶çä¹æ²\n[ç»¿é»çº¢ç´«ç½]id<æ­æ²ç¼å·> |
-æ¥è¯¢ä¹æ²ä¿¡æ¯æè°±é¢ä¿¡æ¯\nå®æ°æ¥æ­ <å®æ°>
-å®æ°æ¥æ­ <å®æ°ä¸é> <å®æ°ä¸é> |
-æ¥è¯¢å®æ°å¯¹åºçä¹æ²\nåæ°çº¿ <é¾åº¦+æ­æ²id> <åæ°çº¿> |
-å±ç¤ºæ­æ²çåæ°çº¿\n\n## åä½è\n\n[Diving-Fish](https://github.com/
-Diving-Fish),æè°¢å¤§ä½¬ä¸ºé³æ¸¸äººçæ ç§å¥ç®\n\n##
-License\n\nMIT\n\næ¨å¯ä»¥èªç±ä½¿ç¨æ¬é¡¹ç®çä»£ç ç¨äºåä¸æéåä¸çç¨éï¼ä½å¿é¡»éå¸¦
-MIT ææåè®®ã\n', 'author': 'Agnes_Digital', 'author_email':
-'Z735803792@163.com', 'maintainer': 'None', 'maintainer_email': 'None', 'url':
-'https://github.com/Umamusume-Agnes-Digital/nonebot_plugin_maimai', 'packages':
-packages, 'package_data': package_data, 'install_requires': install_requires,
-'python_requires': '>=3.8,<4.0', } setup(**setup_kwargs)
+(ä»¥ä¸æ¹æ³2é1) - pypi`nonebot_plugin_maimai`æä»¶å¤¹ä¸­ -
+æç»è·¯å¾ç±»ä¼¼æ¯/path/to/nonebot_plugin_maimai/static - æºå¨äººç®å½ä¸
+- æç»è·¯å¾ç±»ä¼¼æ¯/path/to/data/maimai/staticä¸­ãå¶ä¸­bot.pyæä»¶å¨/
+path/toä½ç½® > èµæºæä»¶ä»ä¾å­¦ä¹ äº¤æµä½¿ç¨ï¼è¯·èªè§å¨ä¸è½½ 24
+å°æ¶åå é¤èµæºæä»¶ã ## FAQ éç½® nonebot æ cq-http
+è¿ç¨ä¸­åºéï¼ > è¯·æ¥é https://github.com/nonebot/nonebot2 ä»¥å
+https://github.com/Mrs4s/go-cqhttp ä¸­çææ¡£ã é¨åæ¶æ¯åä¸åºæ¥ï¼
+>
+è¢«é£æ§äºãè§£å³æ¹å¼ï¼æ¢å·æèè®©è¿ä¸ªå·ä¿æç»éç¶æåä¸å®çèå¤©é¢çï¼æç»­ä¸æ®µæ¶é´ã
+## è¯´æ æ¬ bot æä¾äºå¦ä¸åè½ï¼ å½ä»¤ | åè½ --- | --- help |
+æ¥çå¸®å©ææ¡£ ä»æ¥èè | æ¥çä»å¤©çèèè¿å¿
+XXXmaimaiXXXä»ä¹ | éæºä¸é¦æ­ éä¸ª[dx/æ å][ç»¿é»çº¢ç´«ç½]<é¾åº¦>
+| éæºä¸é¦æå®æ¡ä»¶çä¹æ² æ¥æ­<ä¹æ²æ é¢çä¸é¨å> |
+æ¥è¯¢ç¬¦åæ¡ä»¶çä¹æ² [ç»¿é»çº¢ç´«ç½]id<æ­æ²ç¼å·> |
+æ¥è¯¢ä¹æ²ä¿¡æ¯æè°±é¢ä¿¡æ¯ å®æ°æ¥æ­ <å®æ°>
+å®æ°æ¥æ­ <å®æ°ä¸é> <å®æ°ä¸é> | æ¥è¯¢å®æ°å¯¹åºçä¹æ²
+åæ°çº¿ <é¾åº¦+æ­æ²id> <åæ°çº¿> | å±ç¤ºæ­æ²çåæ°çº¿ ## åä½è
+[Diving-Fish](https://github.com/Diving-
+Fish),æè°¢å¤§ä½¬ä¸ºé³æ¸¸äººçæ ç§å¥ç® ## License MIT
+æ¨å¯ä»¥èªç±ä½¿ç¨æ¬é¡¹ç®çä»£ç ç¨äºåä¸æéåä¸çç¨éï¼ä½å¿é¡»éå¸¦
+MIT ææåè®®ã
```

