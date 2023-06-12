# Comparing `tmp/TeenStudy-0.1.9.tar.gz` & `tmp/teenstudy-0.2.0rc1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "TeenStudy-0.1.9.tar", max compression
+gzip compressed data, was "teenstudy-0.2.0rc1.tar", max compression
```

## Comparing `TeenStudy-0.1.9.tar` & `teenstudy-0.2.0rc1.tar`

### file list

```diff
@@ -1,38 +1,39 @@
--rw-r--r--   0        0        0     1084 2023-05-20 16:35:19.074377 TeenStudy-0.1.9/LICENSE
--rw-r--r--   0        0        0     1002 2023-05-20 16:36:15.517840 TeenStudy-0.1.9/pyproject.toml
--rw-r--r--   0        0        0    10598 2023-05-20 17:11:32.317080 TeenStudy-0.1.9/README.md
--rw-r--r--   0        0        0      666 2023-05-20 16:35:19.076378 TeenStudy-0.1.9/TeenStudy/__init__.py
--rw-r--r--   0        0        0       28 2023-05-20 16:35:19.076378 TeenStudy-0.1.9/TeenStudy/models/__init__.py
--rw-r--r--   0        0        0     3547 2023-05-20 16:35:19.076378 TeenStudy-0.1.9/TeenStudy/models/accuont.py
--rw-r--r--   0        0        0     3621 2023-05-20 16:35:19.077425 TeenStudy-0.1.9/TeenStudy/models/dxx.py
--rw-r--r--   0        0        0   881164 2023-05-20 16:35:19.134720 TeenStudy-0.1.9/TeenStudy/resource/answer.png
--rw-r--r--   0        0        0    52240 2023-05-20 16:35:19.135720 TeenStudy-0.1.9/TeenStudy/resource/backgroud1.jpg
--rw-r--r--   0        0        0    52119 2023-05-20 16:35:19.136721 TeenStudy-0.1.9/TeenStudy/resource/backgroud2.jpg
--rw-r--r--   0        0        0    52136 2023-05-20 16:35:19.136721 TeenStudy-0.1.9/TeenStudy/resource/backgroud3.jpg
--rw-r--r--   0        0        0    51874 2023-05-20 16:35:19.137721 TeenStudy-0.1.9/TeenStudy/resource/backgroud4.jpg
--rw-r--r--   0        0        0    51634 2023-05-20 16:35:19.137721 TeenStudy-0.1.9/TeenStudy/resource/backgroud5.jpg
--rw-r--r--   0        0        0 10424793 2023-05-20 16:35:19.169356 TeenStudy-0.1.9/TeenStudy/resource/dxx_jx.json
--rw-r--r--   0        0        0  7977480 2023-05-20 16:35:19.131719 TeenStudy-0.1.9/TeenStudy/resource/MiSans-Light.ttf
--rw-r--r--   0        0        0      121 2023-05-20 16:35:19.170651 TeenStudy-0.1.9/TeenStudy/utils/__init__.py
--rw-r--r--   0        0        0    54138 2023-05-20 16:55:34.498100 TeenStudy-0.1.9/TeenStudy/utils/dxx.py
--rw-r--r--   0        0        0    18819 2023-05-20 16:35:19.171671 TeenStudy-0.1.9/TeenStudy/utils/handle.py
--rw-r--r--   0        0        0     4331 2023-05-20 16:35:19.171671 TeenStudy-0.1.9/TeenStudy/utils/path.py
--rw-r--r--   0        0        0     2026 2023-05-20 16:35:19.172718 TeenStudy-0.1.9/TeenStudy/utils/rule.py
--rw-r--r--   0        0        0    10411 2023-05-20 16:35:19.172718 TeenStudy-0.1.9/TeenStudy/utils/update.py
--rw-r--r--   0        0        0    24243 2023-05-20 16:57:33.116329 TeenStudy-0.1.9/TeenStudy/utils/utils.py
--rw-r--r--   0        0        0     2185 2023-05-20 16:35:19.174802 TeenStudy-0.1.9/TeenStudy/web/__init__.py
--rw-r--r--   0        0        0      396 2023-05-20 16:35:19.174802 TeenStudy-0.1.9/TeenStudy/web/api/__init__.py
--rw-r--r--   0        0        0    46020 2023-05-20 17:00:14.593604 TeenStudy-0.1.9/TeenStudy/web/api/add.py
--rw-r--r--   0        0        0    11925 2023-05-20 16:35:19.175806 TeenStudy-0.1.9/TeenStudy/web/api/admin.py
--rw-r--r--   0        0        0     4706 2023-05-20 16:35:19.175806 TeenStudy-0.1.9/TeenStudy/web/api/home.py
--rw-r--r--   0        0        0     6317 2023-05-20 16:35:19.176809 TeenStudy-0.1.9/TeenStudy/web/api/login.py
--rw-r--r--   0        0        0       78 2023-05-20 16:35:19.176809 TeenStudy-0.1.9/TeenStudy/web/pages/__init__.py
--rw-r--r--   0        0        0    38893 2023-05-20 16:59:29.116308 TeenStudy-0.1.9/TeenStudy/web/pages/add.py
--rw-r--r--   0        0        0    73709 2023-05-20 17:01:52.359960 TeenStudy-0.1.9/TeenStudy/web/pages/admin.py
--rw-r--r--   0        0        0    17385 2023-05-20 16:35:19.177813 TeenStudy-0.1.9/TeenStudy/web/pages/home.py
--rw-r--r--   0        0        0     1731 2023-05-20 16:35:19.177813 TeenStudy-0.1.9/TeenStudy/web/pages/login.py
--rw-r--r--   0        0        0       24 2023-05-20 16:35:19.179316 TeenStudy-0.1.9/TeenStudy/web/utils/__init__.py
--rw-r--r--   0        0        0     1902 2023-05-20 16:35:19.179316 TeenStudy-0.1.9/TeenStudy/web/utils/add.py
--rw-r--r--   0        0        0     2240 2023-05-20 16:35:19.180340 TeenStudy-0.1.9/TeenStudy/web/utils/status.py
--rw-r--r--   0        0        0    12060 1970-01-01 00:00:00.000000 TeenStudy-0.1.9/setup.py
--rw-r--r--   0        0        0    11811 1970-01-01 00:00:00.000000 TeenStudy-0.1.9/PKG-INFO
+-rw-r--r--   0        0        0     1063 2023-06-12 02:32:00.308969 teenstudy-0.2.0rc1/LICENSE
+-rw-r--r--   0        0        0    11355 2023-06-12 02:32:00.308969 teenstudy-0.2.0rc1/README.md
+-rw-r--r--   0        0        0      766 2023-06-12 02:32:00.308969 teenstudy-0.2.0rc1/TeenStudy/__init__.py
+-rw-r--r--   0        0        0       27 2023-06-12 02:32:00.308969 teenstudy-0.2.0rc1/TeenStudy/models/__init__.py
+-rw-r--r--   0        0        0     3438 2023-06-12 02:32:00.308969 teenstudy-0.2.0rc1/TeenStudy/models/accuont.py
+-rw-r--r--   0        0        0     2770 2023-06-12 02:32:00.308969 teenstudy-0.2.0rc1/TeenStudy/models/dxx.py
+-rw-r--r--   0        0        0  7977480 2023-06-12 02:32:00.368970 teenstudy-0.2.0rc1/TeenStudy/resource/MiSans-Light.ttf
+-rw-r--r--   0        0        0   881164 2023-06-12 02:32:00.372970 teenstudy-0.2.0rc1/TeenStudy/resource/answer.png
+-rw-r--r--   0        0        0    52240 2023-06-12 02:32:00.372970 teenstudy-0.2.0rc1/TeenStudy/resource/backgroud1.jpg
+-rw-r--r--   0        0        0    52119 2023-06-12 02:32:00.372970 teenstudy-0.2.0rc1/TeenStudy/resource/backgroud2.jpg
+-rw-r--r--   0        0        0    52136 2023-06-12 02:32:00.372970 teenstudy-0.2.0rc1/TeenStudy/resource/backgroud3.jpg
+-rw-r--r--   0        0        0    51874 2023-06-12 02:32:00.372970 teenstudy-0.2.0rc1/TeenStudy/resource/backgroud4.jpg
+-rw-r--r--   0        0        0    51634 2023-06-12 02:32:00.372970 teenstudy-0.2.0rc1/TeenStudy/resource/backgroud5.jpg
+-rw-r--r--   0        0        0      116 2023-06-12 02:32:00.372970 teenstudy-0.2.0rc1/TeenStudy/utils/__init__.py
+-rw-r--r--   0        0        0    56096 2023-06-12 02:32:00.372970 teenstudy-0.2.0rc1/TeenStudy/utils/dxx.py
+-rw-r--r--   0        0        0    18464 2023-06-12 02:32:00.372970 teenstudy-0.2.0rc1/TeenStudy/utils/handle.py
+-rw-r--r--   0        0        0     4195 2023-06-12 02:32:00.372970 teenstudy-0.2.0rc1/TeenStudy/utils/path.py
+-rw-r--r--   0        0        0     2354 2023-06-12 02:32:00.372970 teenstudy-0.2.0rc1/TeenStudy/utils/rule.py
+-rw-r--r--   0        0        0    10171 2023-06-12 02:32:00.372970 teenstudy-0.2.0rc1/TeenStudy/utils/update.py
+-rw-r--r--   0        0        0    20971 2023-06-12 02:32:00.372970 teenstudy-0.2.0rc1/TeenStudy/utils/utils.py
+-rw-r--r--   0        0        0     2209 2023-06-12 02:32:00.372970 teenstudy-0.2.0rc1/TeenStudy/web/__init__.py
+-rw-r--r--   0        0        0      456 2023-06-12 02:32:00.372970 teenstudy-0.2.0rc1/TeenStudy/web/api/__init__.py
+-rw-r--r--   0        0        0    38486 2023-06-12 02:32:00.372970 teenstudy-0.2.0rc1/TeenStudy/web/api/add.py
+-rw-r--r--   0        0        0    11593 2023-06-12 02:32:00.372970 teenstudy-0.2.0rc1/TeenStudy/web/api/admin.py
+-rw-r--r--   0        0        0     4927 2023-06-12 02:32:00.372970 teenstudy-0.2.0rc1/TeenStudy/web/api/home.py
+-rw-r--r--   0        0        0     1403 2023-06-12 02:32:00.372970 teenstudy-0.2.0rc1/TeenStudy/web/api/log.py
+-rw-r--r--   0        0        0     5192 2023-06-12 02:32:00.372970 teenstudy-0.2.0rc1/TeenStudy/web/api/login.py
+-rw-r--r--   0        0        0      111 2023-06-12 02:32:00.372970 teenstudy-0.2.0rc1/TeenStudy/web/pages/__init__.py
+-rw-r--r--   0        0        0    29300 2023-06-12 02:32:00.372970 teenstudy-0.2.0rc1/TeenStudy/web/pages/add.py
+-rw-r--r--   0        0        0    44883 2023-06-12 02:32:00.372970 teenstudy-0.2.0rc1/TeenStudy/web/pages/addArea.py
+-rw-r--r--   0        0        0    23125 2023-06-12 02:32:00.372970 teenstudy-0.2.0rc1/TeenStudy/web/pages/admin.py
+-rw-r--r--   0        0        0    18037 2023-06-12 02:32:00.372970 teenstudy-0.2.0rc1/TeenStudy/web/pages/home.py
+-rw-r--r--   0        0        0     2038 2023-06-12 02:32:00.372970 teenstudy-0.2.0rc1/TeenStudy/web/pages/log.py
+-rw-r--r--   0        0        0     1982 2023-06-12 02:32:00.372970 teenstudy-0.2.0rc1/TeenStudy/web/pages/login.py
+-rw-r--r--   0        0        0       24 2023-06-12 02:32:00.372970 teenstudy-0.2.0rc1/TeenStudy/web/utils/__init__.py
+-rw-r--r--   0        0        0     2158 2023-06-12 02:32:00.372970 teenstudy-0.2.0rc1/TeenStudy/web/utils/add.py
+-rw-r--r--   0        0        0     2175 2023-06-12 02:32:00.372970 teenstudy-0.2.0rc1/TeenStudy/web/utils/status.py
+-rw-r--r--   0        0        0      988 2023-06-12 02:32:00.376970 teenstudy-0.2.0rc1/pyproject.toml
+-rw-r--r--   0        0        0    12903 1970-01-01 00:00:00.000000 teenstudy-0.2.0rc1/PKG-INFO
```

### Comparing `TeenStudy-0.1.9/LICENSE` & `teenstudy-0.2.0rc1/LICENSE`

 * *Ordering differences only*

 * *Files 19% similar despite different names*

```diff
@@ -1,21 +1,21 @@
-MIT License
-
-Copyright (c) 2023 ZM25XC
-
-Permission is hereby granted, free of charge, to any person obtaining a copy
-of this software and associated documentation files (the "Software"), to deal
-in the Software without restriction, including without limitation the rights
-to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
-copies of the Software, and to permit persons to whom the Software is
-furnished to do so, subject to the following conditions:
-
-The above copyright notice and this permission notice shall be included in all
-copies or substantial portions of the Software.
-
-THE SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF ANY KIND, EXPRESS OR
-IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY,
-FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE
-AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER
-LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,
-OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE
-SOFTWARE.
+MIT License
+
+Copyright (c) 2023 ZM25XC
+
+Permission is hereby granted, free of charge, to any person obtaining a copy
+of this software and associated documentation files (the "Software"), to deal
+in the Software without restriction, including without limitation the rights
+to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
+copies of the Software, and to permit persons to whom the Software is
+furnished to do so, subject to the following conditions:
+
+The above copyright notice and this permission notice shall be included in all
+copies or substantial portions of the Software.
+
+THE SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF ANY KIND, EXPRESS OR
+IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY,
+FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE
+AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER
+LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,
+OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE
+SOFTWARE.
```

### Comparing `TeenStudy-0.1.9/README.md` & `teenstudy-0.2.0rc1/README.md`

 * *Files 13% similar despite different names*

```diff
@@ -1,242 +1,263 @@
-<div align="center">
-    <img src="https://i.328888.xyz/2023/02/28/z23ho.png" alt="TeenStudy.png" border="0" width="500px" height="500px"/>
-    <h1>TeenStudy</h1>
-    <b>基于nonebot2和go-cqhttp的青年大学习自动提交插件，用于自动完成大学习，在后台留下记录，返回完成截图</b>
-    <br/>
-    <a href="https://github.com/ZM25XC/TeenStudy/issues"><img alt="GitHub issues" src="https://img.shields.io/github/issues/ZM25XC/TeenStudy?style=flat-square"></a>
-    <a href="https://github.com/ZM25XC/TeenStudy/network"><img alt="GitHub forks" src="https://img.shields.io/github/forks/ZM25XC/TeenStudy?style=flat-square"></a>
-    <a href="https://github.com/ZM25XC/TeenStudy/stargazers"><img alt="GitHub stars" src="https://img.shields.io/github/stars/ZM25XC/TeenStudy?style=flat-square"></a>
-    <a href="https://pypi.python.org/pypi/TeenStudy"><img src="https://img.shields.io/pypi/v/TeenStudy?color=yellow" alt="pypi"></a>
-  	<a href="https://pypi.python.org/pypi/TeenStudy">
-    <img src="https://img.shields.io/pypi/dm/TeenStudy" alt="pypi download"></a>
-	  <a href="https://github.com/ZM25XC/TeenStudy/blob/main/LICENSE"><img alt="GitHub license" src="https://img.shields.io/github/license/ZM25XC/TeenStudy?style=flat-square"></a>
-    <a href="https://jq.qq.com/?_wv=1027&k=NGFEwXyS">
-    <img src="https://img.shields.io/badge/QQ%E7%BE%A4-511173803-orange?style=flat-square" alt="QQ Chat Group">
-  </a>
-  </div>
-
-## 说明
-
-- 本项目为[青年大学习提交](https://github.com/ZM25XC/nonebot_plugin_auto_teenstudy) `Web UI`版
-- 本项目基于[nonebot2](https://github.com/nonebot/nonebot2)和[go-cqhttp](https://github.com/Mrs4s/go-cqhttp)，使用本插件前请先阅读以上两个项目的使用文档
--  **启动插件之后，一定要登录后台在推送列表中添加需要开启大学习功能的群聊**
--  **本项目无法在国外IP环境下使用，如有开启代理，请关闭或添加代理规则**
-- 需要抓包的地区，绑定后尽量别进官方公众号，避免token或cookie刷新导致无法提交
-- 本项目需要部署在公网可访问的容器中，并开放端口（nonebot2配置的port），否则大部分功能将出现异常
-- 欢迎加入[QQ群](https://jq.qq.com/?_wv=1027&k=NGFEwXyS)，交流讨论。
-- 时间精力有限，目前只维护湖北和江西两个地区，其他地区出问题请提交Issues,我找个时间修，需要增加地区请进群帮忙测试，个别地区没账号无法测试
-
-- 觉得项目不错，不妨点个stars.
-
-## 地区状态
-
-<details>
-
-| 共青团名称 | 开发状态 | 备注 |
-|:-----:|:----:|:----:|
-|青春湖北|支持|无需抓包|
-|江西共青团|支持|无需抓包|
-|安徽共青团|支持|无需抓包|
-|广东共青团|支持|无需抓包|
-|青春上海|支持|微信扫码绑定|
-|青春浙江|支持|微信扫码绑定|
-|江苏共青团|支持|需要自行抓包|
-|青春山东|支持|需要自行抓包|
-|重庆共青团|支持|需要自行抓包|
-|吉青飞扬|支持|需要自行抓包|
-|黑龙江共青团|支持|需要自行抓包，该地区上线测试中|
-|天府新青年|支持|不进入公众号token时效大于1周|
-|河南共青团|不支持|cookie时效小于1周|
-|广西青年圈|待开发||
-|青春湖南|待开发||
-|甘肃青年|待开发||
-|山西青年|待开发||
-|河北共青团|待开发||
-|福建共青团|待开发||
-|内蒙古青年|待开发||
-|云南共青团|待开发||
-|三秦青年|待开发||
-|青春北京|待开发||
-|海南共青团|待开发||
-|津彩青春|待开发||
-|青春黔言|待开发||
-|青春柳州|待开发||
-|辽宁共青团|待开发||
-|宁夏共青团|待开发||
-|新疆共青团|待开发||
-|西藏共青团|待开发||
-</details>
-
-
-##  安装及更新
-
-<details>
-<summary>第一种方式(不推荐)</summary>
-
-- 使用`git clone https://github.com/ZM25XC/TeenStudy.git`指令克隆本仓库或下载压缩包文件
-
-</details>
-
-<details>
-<summary>第二种方式(二选一)</summary>
-
-- 使用`pip install TeenStudy`来进行安装,使用`pip install TeenStudy -U`进行更新
-- 使用`nb plugin install TeenStudy`来进行安装,使用`nb plugin install TeenStudy -U`进行更新
-
-</details>
-
-
-## 导入插件
-
-<details>
-<summary>使用第一种方式安装看此方法</summary>
-
-- 将`TeenStudy`放在nb的`plugins`目录下，运行nb机器人即可
-
-- 文件结构如下
-
-    ```py
-    📦 AweSome-Bot
-    ├── 📂 awesome_bot
-    │   └── 📂 plugins
-    |       └── 📂 TeenStudy
-    |           └── 📜 __init__.py
-    ├── 📜 .env.prod
-    ├── 📜 .gitignore
-    ├── 📜 pyproject.toml
-    └── 📜 README.md
-    ```
-
-    
-
-</details>
-
-<details>
-<summary>使用第二种方式安装看此方法</summary>
-
-- 在`pyproject.toml`里的`[tool.nonebot]`中添加`plugins = ["TeenStudy"]`
-
-</details>
-
-## 机器人配置
-
-- 在nonebot的`.env` 或 `.env.prod`配置文件中修改nonebot2的`HOST`为`0.0.0.0`、设置好超管账号和公网IP
-
-  ```py
-  HOST = "0.0.0.0"  #nonebot2监听的IP
-  SUPERUSERS = [""] # 超级用户
-  COMMAND_START=[""] # 命令前缀,根据需要自行修改
-  DXX_IP = ""
-  ```
-
-## 使用方式
-
-- 启动nb,等待插件加载数据，加载完毕后登录后台，账号默认为`nonebot配置文件中的超管账号`，密码默认为：`admin`,开放端口（默认为.env中配置的port）
-- 在管理后台的推送列表中添加需要开启大学习使用的群聊
-
-## 功能列表
-|    指令    |               指令格式               |                               说明                               |
-| :--------: | :----------------------------------: | :--------------------------------------------------------------: |
-| 添加大学习 |           添加大学习`地区`           |                    添加大学习湖北 添加大学习                     |
-| 我的大学习 |              我的大学习              |                           查询个人信息                           |
-| 提交大学习 |         提交大学习 戳一戳Bot         |                        提交最新一期大学习                        |
-|   大学习   |     大学习答案、大学习、答案截图     |                    获取最新一期青年大学习答案                    |
-|  完成截图  | 完成截图、大学习截图、大学习完成截图 |            获取最新一期青年大学习完成截图（带状态栏）            |
-| 完成大学习 |        完成大学习、全员大学习        | 团支书可用，需要成员填写团支书ID，填写后团支书可发指令提交大学习 |
-|  重置配置  |          重置配置、刷新配置          |                   超管可用，刷新Web UI默认配置                   |
-|  重置密码  |               重置密码               |                   重置登录Web UI的密码为用户ID                   |
-|删除大学习|删除大学习|用户申请清除数据库的信息|
-|导出用户数据|导出用户数据、导出数据|将数据导出至TeenStudy目录下|
-|更新用户数据|更新用户数据、刷新用户数据|将用户数据导入到数据库|
-|更新资源数据|更新资源数据、刷新资源数据|更新数据库中的资源数据（江西共青团团支部数据）|
-
-
-## ToDo
-
-
-- [ ] 增加更多地区支持
-- [ ] 优化 Bot
-
-
-## 更新日志
-
-### 2023/05/21
-
-- 增加黑龙江地区，需要自行抓包，该地区上线测试中，请积极提issue反馈
-- 下版本为大版本更新，将添加新功能，优化功能，请积极提issue反馈或加交流群反馈
-
-<details>
-<summary>2023/05/11</summary> 
-
-- 增加广东地区，无需抓包[#13](https://github.com/ZM25XC/TeenStudy/issues/13)，感谢[@neal240](https://github.com/neal240)提供账号测试
-
-</details>
-
-<details>
-<summary>2023/05/06</summary> 
-
-- 增加吉林地区，需要自行抓包
-- 修复超管更改登录密码后用原密码能继续登录问题
-- 添加二维码转链接开关，需要自行在后台配置页面打开
-- 调整部分依赖
-
-</details>
-
-<details>
-<summary> 2023/04/12</summary> 
-
-- 因河南地区cookie时效小于1周，移除河南地区
-- 添加`删除大学习`功能，用户可自行删除数据
-- 添加`导出用户数据`功能
-- 添加`更新用户数据`功能
-- 添加`更新资源数据`功能，江西地区更新后请使用下此功能刷新团支部数据
-- 添加戳一戳提交大学习开关，默认开启，请在Web UI后台配置页面进行修改
-- 添加大学习提醒开关，默认开启，支持修改时间，请在Web UI后台配置页面进行修改
-- 添加自动提交大学习开关，默认开启，支持修改时间，请在Web UI后台进行修改
-- 调整安徽地区添加方式[#9](https://github.com/ZM25XC/TeenStudy/issues/9)，无需抓包，感谢[@yhzcake](https://github.com/yhzcake)测试提供方法
-- 修复Web UI 首页公网IP显示异常
-- 修复浙江地区用户重复显示
-- 更新江西共青团团支部数据
-  
-</details>
-
-
-<details>
-<summary>2023/03/18</summary>
-
-- 适配河南地区，需要自行抓包
-- 适配四川地区，需要自行抓包
-- 适配山东地区，需要自行抓包
-- 适配重庆地区，需要自行抓包
-- 添加自动获取公网IP功能，别再问如何配置公网IP啦
-- 添加重置密码功能，指令`重置密码`
-- 添加重置配置功能，指令`重置配置`，`刷新配置`
-- 添加完成大学习功能，团支书可一次性提交全班的大学习，指令`完成大学习`，`全员大学习`
-- 管理后台开放添加用户权限（浙江，上海地区无法添加）
-- 优化用户信息页
-- 优化登录界面提示
-- 将添加链接，登录链接转化成二维码，减少公网IP暴露，没啥用，样式好看一些
-- 修复Ubuntu系统导入资源失败BUG
-  
-</details>
-
-<details>
-
-<summary>2023/03/05</summary>
-
-- 适配浙江地区，使用微信扫码进行绑定
-- 适配上海地区，使用微信扫码进行绑定
-- 适配江苏地区，需要自行抓包
-- 适配安徽地区，需要自行抓包
-
-</details>
-
-<details>
-<summary>2023/03/01</summary>
-
-- 将代码上传至pypi，可使用`pip install TeenStudy`指令安装本插件
-- 上传基础代码
-- 适配湖北地区，无需抓包，安装即用
-- 适配江西地区，无需抓包，安装即用
-
-</details>
+<div align="center">
+    <img src="https://img1.imgtp.com/2023/06/11/sG4KdlpL.png" alt="TeenStudy.png" border="0" width="500px" height="500px"/>
+    <h1>TeenStudy</h1>
+    <b>基于nonebot2和go-cqhttp的青年大学习自动提交插件，用于自动完成大学习，在后台留下记录，返回完成截图</b>
+    <br/>
+    <a href="https://github.com/ZM25XC/TeenStudy/issues"><img alt="GitHub issues" src="https://img.shields.io/github/issues/ZM25XC/TeenStudy?style=flat-square"></a>
+    <a href="https://github.com/ZM25XC/TeenStudy/network"><img alt="GitHub forks" src="https://img.shields.io/github/forks/ZM25XC/TeenStudy?style=flat-square"></a>
+    <a href="https://github.com/ZM25XC/TeenStudy/stargazers"><img alt="GitHub stars" src="https://img.shields.io/github/stars/ZM25XC/TeenStudy?style=flat-square"></a>
+    <a href="https://pypi.python.org/pypi/TeenStudy"><img src="https://img.shields.io/pypi/v/TeenStudy?color=yellow" alt="pypi"></a>
+  	<a href="https://pypi.python.org/pypi/TeenStudy">
+    <img src="https://img.shields.io/pypi/dm/TeenStudy" alt="pypi download"></a>
+	  <a href="https://github.com/ZM25XC/TeenStudy/blob/main/LICENSE"><img alt="GitHub license" src="https://img.shields.io/github/license/ZM25XC/TeenStudy?style=flat-square"></a>
+    <a href="https://jq.qq.com/?_wv=1027&k=NGFEwXyS">
+    <img src="https://img.shields.io/badge/QQ反馈群-511173803-orange?style=flat-square" alt="QQ Chat Group">
+  </a>
+	<a href="http://qm.qq.com/cgi-bin/qm/qr?_wv=1027&k=2PQucjirnkHyPjoS1Pkr-ai2aPGToBKm">
+    <img src="https://img.shields.io/badge/QQ体验群-821280615-orange?style=flat-square" alt="QQ Chat Group">
+  </a>
+  </div>
+
+## 说明
+
+- 本项目为[青年大学习提交](https://github.com/ZM25XC/nonebot_plugin_auto_teenstudy) `Web UI`版
+- 本项目基于[nonebot2](https://github.com/nonebot/nonebot2)和[go-cqhttp](https://github.com/Mrs4s/go-cqhttp)，使用本插件前请先阅读以上两个项目的使用文档
+-  **启动插件之后，一定要登录后台在推送列表中添加需要开启大学习功能的群聊**
+-  **本项目无法在国外IP环境下使用，如有开启代理，请关闭或添加代理规则**
+- 需要抓包的地区，绑定后尽量别进官方公众号，避免token或cookie刷新导致无法提交
+- 本项目需要部署在公网可访问的容器中，并开放端口（nonebot2配置的port），否则大部分功能将出现异常
+- 欢迎加入[QQ反馈群](https://jq.qq.com/?_wv=1027&k=NGFEwXyS)，交流讨论，如您不会搭建又想每周自动提交，可加入[QQ体验群](http://qm.qq.com/cgi-bin/qm/qr?_wv=1027&k=2PQucjirnkHyPjoS1Pkr-ai2aPGToBKm)。
+- 时间精力有限，目前只维护湖北和江西两个地区，其他地区出问题请提交Issues,我找个时间修，需要增加地区请进群帮忙测试，个别地区没账号无法测试
+
+- 觉得项目不错，不妨点个stars.
+
+## 地区状态
+
+<details>
+
+| 共青团名称 | 开发状态 | 备注 |
+|:-----:|:----:|:----:|
+|青春湖北|支持|无需抓包|
+|江西共青团|支持|无需抓包|
+|安徽共青团|支持|无需抓包|
+|广东共青团|支持|无需抓包|
+|青春北京|支持|无需抓包|
+|青春上海|支持|微信扫码绑定|
+|青春浙江|支持|微信扫码绑定|
+|津彩青春|支持|需要自行抓包|
+|青春山东|支持|需要自行抓包|
+|重庆共青团|支持|需要自行抓包|
+|吉青飞扬|支持|需要自行抓包|
+|天府新青年|支持|不进入公众号token时效大于1周|
+|河南共青团|不支持|cookie时效小于1周|
+|江苏共青团|不支持|cookie失效小于1周|
+|黑龙江共青团|不支持|cookie失效小于1周|
+|广西青年圈|待开发||
+|青春湖南|待开发||
+|甘肃青年|待开发||
+|山西青年|待开发||
+|河北共青团|待开发||
+|福建共青团|待开发||
+|内蒙古青年|待开发||
+|云南共青团|待开发||
+|三秦青年|待开发||
+|海南共青团|待开发||
+|青春黔言|待开发||
+|青春柳州|待开发||
+|辽宁共青团|待开发||
+|宁夏共青团|待开发||
+|新疆共青团|待开发||
+|西藏共青团|待开发||
+</details>
+
+
+##  安装及更新
+
+<details>
+<summary>第一种方式(不推荐)</summary>
+
+- 使用`git clone https://github.com/ZM25XC/TeenStudy.git`指令克隆本仓库或下载压缩包文件
+
+</details>
+
+<details>
+<summary>第二种方式(二选一)</summary>
+
+- 使用`pip install TeenStudy`来进行安装,使用`pip install TeenStudy -U`进行更新
+- 使用`nb plugin install TeenStudy`来进行安装,使用`nb plugin install TeenStudy -U`进行更新
+
+</details>
+
+
+## 导入插件
+
+<details>
+<summary>使用第一种方式安装看此方法</summary>
+
+- 将`TeenStudy`放在nb的`plugins`目录下，运行nb机器人即可
+
+- 文件结构如下
+
+    ```py
+    📦 AweSome-Bot
+    ├── 📂 awesome_bot
+    │   └── 📂 plugins
+    |       └── 📂 TeenStudy
+    |           └── 📜 __init__.py
+    ├── 📜 .env.prod
+    ├── 📜 .gitignore
+    ├── 📜 pyproject.toml
+    └── 📜 README.md
+    ```
+
+    
+
+</details>
+
+<details>
+<summary>使用第二种方式安装看此方法</summary>
+
+- 在`pyproject.toml`里的`[tool.nonebot]`中添加`plugins = ["TeenStudy"]`
+
+</details>
+
+## 机器人配置
+
+- 在nonebot的`.env` 或 `.env.prod`配置文件中修改nonebot2的`HOST`为`0.0.0.0`、设置好超管账号和公网IP
+
+  ```py
+  HOST = "0.0.0.0"  #nonebot2监听的IP
+  SUPERUSERS = [""] # 超级用户
+  COMMAND_START=[""] # 命令前缀,根据需要自行修改
+  DXX_IP = ""
+  ```
+
+## 使用方式
+
+- 启动nb,等待插件加载数据，加载完毕后登录后台，账号默认为`nonebot配置文件中的超管账号`，密码默认为：`admin`,开放端口（默认为.env中配置的port）
+- 在管理后台的推送列表中添加需要开启大学习使用的群聊
+
+## 功能列表
+|    指令    |               指令格式               |                               说明                               |
+| :--------: | :----------------------------------: | :--------------------------------------------------------------: |
+| 添加大学习 |           添加大学习`地区`           |                    添加大学习湖北 添加大学习                     |
+| 我的大学习 |              我的大学习              |                           查询个人信息                           |
+| 提交大学习 |         提交大学习 戳一戳Bot         |                        提交最新一期大学习                        |
+|   大学习   |     大学习答案、大学习、答案截图     |                    获取最新一期青年大学习答案                    |
+|  完成截图  | 完成截图、大学习截图、大学习完成截图 |            获取最新一期青年大学习完成截图（带状态栏）            |
+| 完成大学习 |        完成大学习、全员大学习        | 团支书可用，需要成员填写团支书ID，填写后团支书可发指令提交大学习 |
+|  重置配置  |          重置配置、刷新配置          |                   超管可用，刷新Web UI默认配置                   |
+|  重置密码  |               重置密码               |                   重置登录Web UI的密码为用户ID                   |
+|删除大学习|删除大学习|用户申请清除数据库的信息|
+|导出用户数据|导出用户数据、导出数据|将数据导出至TeenStudy目录下|
+|更新用户数据|更新用户数据、刷新用户数据|将用户数据导入到数据库|
+|更新资源数据|更新资源数据、刷新资源数据|更新数据库中的资源数据（江西共青团团支部数据）|
+
+
+## ToDo
+
+
+- [ ] 增加更多地区支持
+- [ ] 优化 Bot
+
+
+## 更新日志
+
+### 2023/06/12
+
+- 适配北京地区，无需抓包
+- 增加天津地区，需要自行抓包
+- 因江苏和黑龙江地区Cookie时效小于1周，移除江苏和黑龙江地区
+- Web UI添加日志和主动退出功能
+- 更新江西地区拉取团支部数据方式，移除缓存团支部数据，包体积减小50%
+- 修复大学习公网检测失败问题
+- 更新Nonebot2强制meta字段
+- 同步UI依赖AMIS版本到最新版本
+- 开放体验群，不会搭建又想使用的可加[QQ体验群](http://qm.qq.com/cgi-bin/qm/qr?_wv=1027&k=2PQucjirnkHyPjoS1Pkr-ai2aPGToBKm)
+  
+
+<details>
+
+<summary>2023/05/21</summary>
+
+- 增加黑龙江地区，需要自行抓包，该地区上线测试中，请积极提issue反馈
+- 下版本为大版本更新，将添加新功能，优化功能，请积极提issue反馈或加交流群反馈
+- 
+</details>
+
+
+<details>
+<summary>2023/05/11</summary> 
+
+- 增加广东地区，无需抓包[#13](https://github.com/ZM25XC/TeenStudy/issues/13)，感谢[@neal240](https://github.com/neal240)提供账号测试
+
+</details>
+
+<details>
+<summary>2023/05/06</summary> 
+
+- 增加吉林地区，需要自行抓包
+- 修复超管更改登录密码后用原密码能继续登录问题
+- 添加二维码转链接开关，需要自行在后台配置页面打开
+- 调整部分依赖
+
+</details>
+
+<details>
+<summary> 2023/04/12</summary> 
+
+- 因河南地区cookie时效小于1周，移除河南地区
+- 添加`删除大学习`功能，用户可自行删除数据
+- 添加`导出用户数据`功能
+- 添加`更新用户数据`功能
+- 添加`更新资源数据`功能，江西地区更新后请使用下此功能刷新团支部数据
+- 添加戳一戳提交大学习开关，默认开启，请在Web UI后台配置页面进行修改
+- 添加大学习提醒开关，默认开启，支持修改时间，请在Web UI后台配置页面进行修改
+- 添加自动提交大学习开关，默认开启，支持修改时间，请在Web UI后台进行修改
+- 调整安徽地区添加方式[#9](https://github.com/ZM25XC/TeenStudy/issues/9)，无需抓包，感谢[@yhzcake](https://github.com/yhzcake)测试提供方法
+- 修复Web UI 首页公网IP显示异常
+- 修复浙江地区用户重复显示
+- 更新江西共青团团支部数据
+  
+</details>
+
+
+<details>
+<summary>2023/03/18</summary>
+
+- 适配河南地区，需要自行抓包
+- 适配四川地区，需要自行抓包
+- 适配山东地区，需要自行抓包
+- 适配重庆地区，需要自行抓包
+- 添加自动获取公网IP功能，别再问如何配置公网IP啦
+- 添加重置密码功能，指令`重置密码`
+- 添加重置配置功能，指令`重置配置`，`刷新配置`
+- 添加完成大学习功能，团支书可一次性提交全班的大学习，指令`完成大学习`，`全员大学习`
+- 管理后台开放添加用户权限（浙江，上海地区无法添加）
+- 优化用户信息页
+- 优化登录界面提示
+- 将添加链接，登录链接转化成二维码，减少公网IP暴露，没啥用，样式好看一些
+- 修复Ubuntu系统导入资源失败BUG
+  
+</details>
+
+<details>
+
+<summary>2023/03/05</summary>
+
+- 适配浙江地区，使用微信扫码进行绑定
+- 适配上海地区，使用微信扫码进行绑定
+- 适配江苏地区，需要自行抓包
+- 适配安徽地区，需要自行抓包
+
+</details>
+
+<details>
+<summary>2023/03/01</summary>
+
+- 将代码上传至pypi，可使用`pip install TeenStudy`指令安装本插件
+- 上传基础代码
+- 适配湖北地区，无需抓包，安装即用
+- 适配江西地区，无需抓包，安装即用
+
+</details>
```

#### html2text {}

```diff
@@ -1,46 +1,49 @@
                                 [TeenStudy.png]
                             ****** TeenStudy ******
                              åºäºnonebot2ågo-
 cqhttpçéå¹´å¤§å­¦ä¹ èªå¨æäº¤æä»¶ï¼ç¨äºèªå¨å®æå¤§å­¦ä¹ ï¼å¨åå°çä¸è®°å½ï¼è¿åå®ææªå¾
 
  [GitHub_issues] [GitHub_forks] [GitHub_stars] [pypi] [pypi_download] [GitHub
-                           license] [QQ_Chat_Group]
+                   license] [QQ_Chat_Group] [QQ_Chat_Group]
 ## è¯´æ - æ¬é¡¹ç®ä¸º[éå¹´å¤§å­¦ä¹ æäº¤](https://github.com/ZM25XC/
 nonebot_plugin_auto_teenstudy) `Web UI`ç - æ¬é¡¹ç®åºäº[nonebot2](https://
 github.com/nonebot/nonebot2)å[go-cqhttp](https://github.com/Mrs4s/go-
 cqhttp)ï¼ä½¿ç¨æ¬æä»¶åè¯·åéè¯»ä»¥ä¸ä¸¤ä¸ªé¡¹ç®çä½¿ç¨ææ¡£ -
 **å¯å¨æä»¶ä¹åï¼ä¸å®è¦ç»å½åå°å¨æ¨éåè¡¨ä¸­æ·»å éè¦å¼å¯å¤§å­¦ä¹ åè½çç¾¤è**
 -
 **æ¬é¡¹ç®æ æ³å¨å½å¤IPç¯å¢ä¸ä½¿ç¨ï¼å¦æå¼å¯ä»£çï¼è¯·å³é­ææ·»å ä»£çè§å**
 -
 éè¦æåçå°åºï¼ç»å®åå°½éå«è¿å®æ¹å¬ä¼å·ï¼é¿åtokenæcookieå·æ°å¯¼è´æ æ³æäº¤
 -
 æ¬é¡¹ç®éè¦é¨ç½²å¨å¬ç½å¯è®¿é®çå®¹å¨ä¸­ï¼å¹¶å¼æ¾ç«¯å£ï¼nonebot2éç½®çportï¼ï¼å¦åå¤§é¨ååè½å°åºç°å¼å¸¸
-- æ¬¢è¿å å¥[QQç¾¤](https://jq.qq.com/?_wv=1027&k=NGFEwXyS)ï¼äº¤æµè®¨è®ºã
--
+- æ¬¢è¿å å¥[QQåé¦ç¾¤](https://jq.qq.com/
+?_wv=1027&k=NGFEwXyS)ï¼äº¤æµè®¨è®ºï¼å¦æ¨ä¸ä¼æ­å»ºåæ³æ¯å¨èªå¨æäº¤ï¼å¯å å¥
+[QQä½éªç¾¤](http://qm.qq.com/cgi-bin/qm/qr?_wv=1027&k=2PQucjirnkHyPjoS1Pkr-
+ai2aPGToBKm)ã -
 æ¶é´ç²¾åæéï¼ç®ååªç»´æ¤æ¹ååæ±è¥¿ä¸¤ä¸ªå°åºï¼å¶ä»å°åºåºé®é¢è¯·æäº¤Issues,ææ¾ä¸ªæ¶é´ä¿®ï¼éè¦å¢å å°åºè¯·è¿ç¾¤å¸®å¿æµè¯ï¼ä¸ªå«å°åºæ²¡è´¦å·æ æ³æµè¯
 - è§å¾é¡¹ç®ä¸éï¼ä¸å¦¨ç¹ä¸ªstars. ## å°åºç¶æ  | å±éå¢åç§° |
 å¼åç¶æ | å¤æ³¨ | |:-----:|:----:|:----:
 | |éæ¥æ¹å|æ¯æ|æ éæå| |æ±è¥¿å±éå¢|æ¯æ|æ éæå|
 |å®å¾½å±éå¢|æ¯æ|æ éæå| |å¹¿ä¸å±éå¢|æ¯æ|æ éæå|
-|éæ¥ä¸æµ·|æ¯æ|å¾®ä¿¡æ«ç ç»å®|
+|éæ¥åäº¬|æ¯æ|æ éæå| |éæ¥ä¸æµ·|æ¯æ|å¾®ä¿¡æ«ç ç»å®|
 |éæ¥æµæ±|æ¯æ|å¾®ä¿¡æ«ç ç»å®|
-|æ±èå±éå¢|æ¯æ|éè¦èªè¡æå|
+|æ´¥å½©éæ¥|æ¯æ|éè¦èªè¡æå|
 |éæ¥å±±ä¸|æ¯æ|éè¦èªè¡æå|
 |éåºå±éå¢|æ¯æ|éè¦èªè¡æå|
 |åéé£æ¬|æ¯æ|éè¦èªè¡æå|
-|é»é¾æ±å±éå¢|æ¯æ|éè¦èªè¡æåï¼è¯¥å°åºä¸çº¿æµè¯ä¸­|
 |å¤©åºæ°éå¹´|æ¯æ|ä¸è¿å¥å¬ä¼å·tokenæ¶æå¤§äº1å¨|
-|æ²³åå±éå¢|ä¸æ¯æ|cookieæ¶æå°äº1å¨| |å¹¿è¥¿éå¹´å|å¾å¼å||
-|éæ¥æ¹å|å¾å¼å|| |çèéå¹´|å¾å¼å|| |å±±è¥¿éå¹´|å¾å¼å||
+|æ²³åå±éå¢|ä¸æ¯æ|cookieæ¶æå°äº1å¨|
+|æ±èå±éå¢|ä¸æ¯æ|cookieå¤±æå°äº1å¨|
+|é»é¾æ±å±éå¢|ä¸æ¯æ|cookieå¤±æå°äº1å¨|
+|å¹¿è¥¿éå¹´å|å¾å¼å|| |éæ¥æ¹å|å¾å¼å||
+|çèéå¹´|å¾å¼å|| |å±±è¥¿éå¹´|å¾å¼å||
 |æ²³åå±éå¢|å¾å¼å|| |ç¦å»ºå±éå¢|å¾å¼å||
 |åèå¤éå¹´|å¾å¼å|| |äºåå±éå¢|å¾å¼å||
-|ä¸ç§¦éå¹´|å¾å¼å|| |éæ¥åäº¬|å¾å¼å||
-|æµ·åå±éå¢|å¾å¼å|| |æ´¥å½©éæ¥|å¾å¼å||
+|ä¸ç§¦éå¹´|å¾å¼å|| |æµ·åå±éå¢|å¾å¼å||
 |éæ¥é»è¨|å¾å¼å|| |éæ¥æ³å·|å¾å¼å||
 |è¾½å®å±éå¢|å¾å¼å|| |å®å¤å±éå¢|å¾å¼å||
 |æ°çå±éå¢|å¾å¼å|| |è¥¿èå±éå¢|å¾å¼å||  ## å®è£åæ´æ°
 ç¬¬ä¸ç§æ¹å¼(ä¸æ¨è) - ä½¿ç¨`git clone https://github.com/ZM25XC/
 TeenStudy.git`æä»¤åéæ¬ä»åºæä¸è½½åç¼©åæä»¶   ç¬¬äºç§æ¹å¼
 (äºéä¸) - ä½¿ç¨`pip install TeenStudy`æ¥è¿è¡å®è£,ä½¿ç¨`pip install
 TeenStudy -U`è¿è¡æ´æ° - ä½¿ç¨`nb plugin install
@@ -76,20 +79,29 @@
 UIé»è®¤éç½® | | éç½®å¯ç  | éç½®å¯ç  | éç½®ç»å½Web
 UIçå¯ç ä¸ºç¨æ·ID |
 |å é¤å¤§å­¦ä¹ |å é¤å¤§å­¦ä¹ |ç¨æ·ç³è¯·æ¸é¤æ°æ®åºçä¿¡æ¯|
 |å¯¼åºç¨æ·æ°æ®|å¯¼åºç¨æ·æ°æ®ãå¯¼åºæ°æ®|å°æ°æ®å¯¼åºè³TeenStudyç®å½ä¸|
 |æ´æ°ç¨æ·æ°æ®|æ´æ°ç¨æ·æ°æ®ãå·æ°ç¨æ·æ°æ®|å°ç¨æ·æ°æ®å¯¼å¥å°æ°æ®åº|
 |æ´æ°èµæºæ°æ®|æ´æ°èµæºæ°æ®ãå·æ°èµæºæ°æ®|æ´æ°æ°æ®åºä¸­çèµæºæ°æ®ï¼æ±è¥¿å±éå¢å¢æ¯é¨æ°æ®ï¼|
 ## ToDo - [ ] å¢å æ´å¤å°åºæ¯æ - [ ] ä¼å Bot ## æ´æ°æ¥å¿ ###
-2023/05/21 -
+2023/06/12 - ééåäº¬å°åºï¼æ éæå -
+å¢å å¤©æ´¥å°åºï¼éè¦èªè¡æå -
+å æ±èåé»é¾æ±å°åºCookieæ¶æå°äº1å¨ï¼ç§»é¤æ±èåé»é¾æ±å°åº
+- Web UIæ·»å æ¥å¿åä¸»å¨éåºåè½ -
+æ´æ°æ±è¥¿å°åºæåå¢æ¯é¨æ°æ®æ¹å¼ï¼ç§»é¤ç¼å­å¢æ¯é¨æ°æ®ï¼åä½ç§¯åå°50%
+- ä¿®å¤å¤§å­¦ä¹ å¬ç½æ£æµå¤±è´¥é®é¢ - æ´æ°Nonebot2å¼ºå¶metaå­æ®µ -
+åæ­¥UIä¾èµAMISçæ¬å°ææ°çæ¬ -
+å¼æ¾ä½éªç¾¤ï¼ä¸ä¼æ­å»ºåæ³ä½¿ç¨çå¯å [QQä½éªç¾¤](http://
+qm.qq.com/cgi-bin/qm/qr?_wv=1027&k=2PQucjirnkHyPjoS1Pkr-ai2aPGToBKm)  2023/05/
+21 -
 å¢å é»é¾æ±å°åºï¼éè¦èªè¡æåï¼è¯¥å°åºä¸çº¿æµè¯ä¸­ï¼è¯·ç§¯ææissueåé¦
 -
 ä¸çæ¬ä¸ºå¤§çæ¬æ´æ°ï¼å°æ·»å æ°åè½ï¼ä¼ååè½ï¼è¯·ç§¯ææissueåé¦æå äº¤æµç¾¤åé¦
-2023/05/11 - å¢å å¹¿ä¸å°åºï¼æ éæå[#13](https://github.com/ZM25XC/
-TeenStudy/issues/13)ï¼æè°¢[@neal240](https://github.com/
+-   2023/05/11 - å¢å å¹¿ä¸å°åºï¼æ éæå[#13](https://github.com/
+ZM25XC/TeenStudy/issues/13)ï¼æè°¢[@neal240](https://github.com/
 neal240)æä¾è´¦å·æµè¯   2023/05/06 -
 å¢å åæå°åºï¼éè¦èªè¡æå -
 ä¿®å¤è¶ç®¡æ´æ¹ç»å½å¯ç åç¨åå¯ç è½ç»§ç»­ç»å½é®é¢ -
 æ·»å äºç»´ç è½¬é¾æ¥å¼å³ï¼éè¦èªè¡å¨åå°éç½®é¡µé¢æå¼ -
 è°æ´é¨åä¾èµ    2023/04/12 -
 å æ²³åå°åºcookieæ¶æå°äº1å¨ï¼ç§»é¤æ²³åå°åº -
 æ·»å `å é¤å¤§å­¦ä¹ `åè½ï¼ç¨æ·å¯èªè¡å é¤æ°æ® -
```

### Comparing `TeenStudy-0.1.9/TeenStudy/models/dxx.py` & `teenstudy-0.2.0rc1/TeenStudy/models/dxx.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,118 +1,94 @@
-from tortoise import fields
-from tortoise.models import Model
-
-
-class Answer(Model):
-    id: int = fields.IntField(pk=True, generated=True, auto_increment=True)
-    """自增主键，数据库ID"""
-    code: str = fields.TextField()
-    """大学习期数标识"""
-    catalogue: str = fields.TextField()
-    """大学习期数名称"""
-    time: int = fields.IntField()
-    """更新时间戳"""
-    url: str = fields.TextField()
-    """大学习网址"""
-    end_url: str = fields.TextField()
-    """完成截图网址"""
-    answer: str = fields.TextField()
-    """答案"""
-    cover: bytes = fields.BinaryField()
-    """大学习完成截图"""
-
-    class Meta:
-        table = 'Answer'
-        table_description = '大学习答案'
-        indexes = ('time',)
-
-
-class Area(Model):
-    id: int = fields.IntField(pk=True, generated=True, auto_increment=True)
-    """自增主键，数据库ID"""
-    time: int = fields.IntField(null=True)
-    """更新时间戳"""
-    area: str = fields.TextField()
-    """地区"""
-    host: str = fields.TextField()
-    """请求host"""
-    referer: str = fields.TextField(null=True)
-    """请求Referer"""
-    origin: str = fields.TextField(null=True)
-    """请求Origin"""
-    url: str = fields.TextField()
-    """检查更新url"""
-    status: bool = fields.BooleanField(default=True, null=True)
-    """是否为最新一期"""
-    catalogue: str = fields.TextField(null=True)
-    """大学习期数名称"""
-
-    class Meta:
-        table = 'Area'
-        table_description = '地区列表'
-        indexes = ('time',)
-
-
-class Resource(Model):
-    id: int = fields.IntField(pk=True, generated=True, auto_increment=True)
-    """自增主键，数据库ID"""
-    time: int = fields.IntField()
-    """创建时间"""
-    name: str = fields.TextField()
-    """资源名称"""
-    type: str = fields.TextField()
-    """资源类型"""
-    url: str = fields.TextField()
-    """文件下载链接"""
-    file: bytes = fields.BinaryField(null=True)
-    """资源内容"""
-    size: str = fields.TextField(null=True)
-    """文件大小"""
-
-    class Meta:
-        table = 'Resource'
-        table_description = '大学习插件资源'
-        indexes = ('time',)
-
-
-class JiangXi(Model):
-    id: int = fields.IntField(pk=True, generated=True, auto_increment=True)
-    """自增主键，数据库ID"""
-    time: int = fields.IntField()
-    """创建时间"""
-    university_id: str = fields.TextField(null=True)
-    """学校id"""
-    university: str = fields.TextField()
-    """学校名称"""
-    college_id: str = fields.TextField(null=True)
-    """学院id"""
-    college: str = fields.TextField()
-    """学院名称"""
-    organization = fields.TextField(null=True)
-    """团支部"""
-    organization_id: str = fields.TextField(null=True)
-    """团支部id"""
-
-    class Meta:
-        table = 'JiangXi'
-        table_description = '江西地区团支部数据'
-        indexes = ('time',)
-
-
-class PushList(Model):
-    id: int = fields.IntField(pk=True, generated=True, auto_increment=True)
-    """自增主键，数据库ID"""
-    time: int = fields.IntField()
-    """创建时间"""
-    self_id: int = fields.IntField()
-    """机器人Id"""
-    user_id: int = fields.IntField()
-    """添加人员"""
-    group_id: int = fields.IntField()
-    """通知群聊"""
-    status: bool = fields.BooleanField(default=True)
-    """通知状态"""
-
-    class Meta:
-        table = 'PushList'
-        table_description = '通知群列表'
-        indexes = ('time',)
+from tortoise import fields
+from tortoise.models import Model
+
+
+class Answer(Model):
+    id: int = fields.IntField(pk=True, generated=True, auto_increment=True)
+    """自增主键，数据库ID"""
+    code: str = fields.TextField()
+    """大学习期数标识"""
+    catalogue: str = fields.TextField()
+    """大学习期数名称"""
+    time: int = fields.IntField()
+    """更新时间戳"""
+    url: str = fields.TextField()
+    """大学习网址"""
+    end_url: str = fields.TextField()
+    """完成截图网址"""
+    answer: str = fields.TextField()
+    """答案"""
+    cover: bytes = fields.BinaryField()
+    """大学习完成截图"""
+
+    class Meta:
+        table = 'Answer'
+        table_description = '大学习答案'
+        indexes = ('time',)
+
+
+class Area(Model):
+    id: int = fields.IntField(pk=True, generated=True, auto_increment=True)
+    """自增主键，数据库ID"""
+    time: int = fields.IntField(null=True)
+    """更新时间戳"""
+    area: str = fields.TextField()
+    """地区"""
+    host: str = fields.TextField()
+    """请求host"""
+    referer: str = fields.TextField(null=True)
+    """请求Referer"""
+    origin: str = fields.TextField(null=True)
+    """请求Origin"""
+    url: str = fields.TextField()
+    """检查更新url"""
+    status: bool = fields.BooleanField(default=True, null=True)
+    """是否为最新一期"""
+    catalogue: str = fields.TextField(null=True)
+    """大学习期数名称"""
+
+    class Meta:
+        table = 'Area'
+        table_description = '地区列表'
+        indexes = ('time',)
+
+
+class Resource(Model):
+    id: int = fields.IntField(pk=True, generated=True, auto_increment=True)
+    """自增主键，数据库ID"""
+    time: int = fields.IntField()
+    """创建时间"""
+    name: str = fields.TextField()
+    """资源名称"""
+    type: str = fields.TextField()
+    """资源类型"""
+    url: str = fields.TextField()
+    """文件下载链接"""
+    file: bytes = fields.BinaryField(null=True)
+    """资源内容"""
+    size: str = fields.TextField(null=True)
+    """文件大小"""
+
+    class Meta:
+        table = 'Resource'
+        table_description = '大学习插件资源'
+        indexes = ('time',)
+
+
+class PushList(Model):
+    id: int = fields.IntField(pk=True, generated=True, auto_increment=True)
+    """自增主键，数据库ID"""
+    time: int = fields.IntField()
+    """创建时间"""
+    self_id: int = fields.IntField()
+    """机器人Id"""
+    user_id: int = fields.IntField()
+    """添加人员"""
+    group_id: int = fields.IntField()
+    """通知群聊"""
+    status: bool = fields.BooleanField(default=True)
+    """通知状态"""
+
+    class Meta:
+        table = 'PushList'
+        table_description = '通知群列表'
+        indexes = ('time',)
```

### Comparing `TeenStudy-0.1.9/TeenStudy/resource/answer.png` & `teenstudy-0.2.0rc1/TeenStudy/resource/answer.png`

 * *Files identical despite different names*

### Comparing `TeenStudy-0.1.9/TeenStudy/resource/backgroud1.jpg` & `teenstudy-0.2.0rc1/TeenStudy/resource/backgroud1.jpg`

 * *Files identical despite different names*

### Comparing `TeenStudy-0.1.9/TeenStudy/resource/backgroud2.jpg` & `teenstudy-0.2.0rc1/TeenStudy/resource/backgroud2.jpg`

 * *Files identical despite different names*

### Comparing `TeenStudy-0.1.9/TeenStudy/resource/backgroud3.jpg` & `teenstudy-0.2.0rc1/TeenStudy/resource/backgroud3.jpg`

 * *Files identical despite different names*

### Comparing `TeenStudy-0.1.9/TeenStudy/resource/backgroud4.jpg` & `teenstudy-0.2.0rc1/TeenStudy/resource/backgroud4.jpg`

 * *Files identical despite different names*

### Comparing `TeenStudy-0.1.9/TeenStudy/resource/backgroud5.jpg` & `teenstudy-0.2.0rc1/TeenStudy/resource/backgroud5.jpg`

 * *Files identical despite different names*

### Comparing `TeenStudy-0.1.9/TeenStudy/resource/MiSans-Light.ttf` & `teenstudy-0.2.0rc1/TeenStudy/resource/MiSans-Light.ttf`

 * *Files identical despite different names*

### Comparing `TeenStudy-0.1.9/TeenStudy/utils/dxx.py` & `teenstudy-0.2.0rc1/TeenStudy/utils/dxx.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,1145 +1,1178 @@
-import json
-import random
-import re
-import secrets
-import time
-import urllib.parse
-
-from anti_useragent import UserAgent
-from httpx import AsyncClient
-from nonebot import logger
-
-from ..models.accuont import User, Commit
-from ..models.dxx import Answer
-
-headers = {
-    'Accept': 'application/json, text/plain, */*',
-    'Accept-Encoding': 'gzip, deflate',
-    'Accept-Language': 'zh-CN,zh;q=0.9,en-US;q=0.8,en;q=0.7',
-    'Connection': 'keep-alive',
-    'Content-Type': 'application/json;charset=UTF-8',
-    'User-Agent': UserAgent(platform="iphone", min_version=1, max_version=5).wechat,
-    'X-Requested-With': 'XMLHttpRequest'
-}
-
-
-async def commit(user_id: int, catalogue: str, status: bool = False) -> None:
-    """
-    记录提交状态
-    :param catalogue: 提交期数
-    :param user_id: 用户ID
-    :param status:提交状态，默认为False
-    :return:
-    """
-    result = await User.filter(user_id=user_id).values()
-    await Commit.create(
-        time=time.time(),
-        user_id=user_id,
-        area=result[0]["area"],
-        status=status,
-        name=result[0]["name"],
-        university=result[0]["university"],
-        college=result[0]["college"],
-        organization=result[0]["organization"],
-        catalogue=catalogue
-    )
-
-
-async def hubei(user_id: int) -> dict:
-    """
-    青春湖北
-    :param user_id:用户ID
-    :return:
-    """
-    result = await User.filter(user_id=user_id).values()
-    if not result:
-        return {
-            "status": 500,
-            "msg": "用户数据不存在！"
-        }
-    else:
-        name = result[0]["name"]
-        openid = result[0]["openid"]
-        university = result[0]["university"]
-        college = result[0]["college"]
-        organization = result[0]["organization"]
-        answer = await Answer.all().order_by("time").values()
-        headers.update({
-            "Host": "cp.fjg360.cn",
-            "X-Requested-With": "XMLHttpRequest",
-            "Sec-Fetch-Site": "same-origin",
-            "Sec-Fetch-Mode": "cors",
-            "Sec-Fetch-Dest": "empty",
-            "Accept-Encoding": "gzip, deflate",
-            "Accept-Language": "zh-CN,zh;q=0.9,en-US;q=0.8,en;q=0.7",
-        })
-        url = "https://cp.fjg360.cn/index.php?m=vote&c=index&a=save_door&sessionId=&imgTextId=&ip="
-        url += "&username=" + name
-        url += "&phone=" + "未知"
-        url += "&city=" + university
-        url += "&danwei2=" + organization
-        url += "&danwei=" + college
-        url += "&openid=" + openid
-        url += "&num=10"
-        url += "&lesson_name=" + answer[-1]["catalogue"]
-        try:
-            async with AsyncClient(headers=headers) as client:
-                response = await client.get(url)
-            response_json = json.loads(response.text)
-            if response_json.get('code') == 1:
-                await User.filter(user_id=user_id).update(
-                    commit_time=time.time(),
-                    catalogue=answer[-1]["catalogue"]
-                )
-                await commit(user_id=user_id, catalogue=answer[-1]["catalogue"], status=True)
-                return {
-                    "status": 0,
-                    "catalogue": answer[-1]["catalogue"],
-                    "msg": "提交成功！"
-                }
-            else:
-                await commit(user_id=user_id, catalogue=answer[-1]["catalogue"], status=False)
-                return {
-                    "status": 500,
-                    "msg": "提交失败！"
-                }
-        except Exception as e:
-            logger.error(e)
-            await commit(user_id=user_id, catalogue=answer[-1]["catalogue"], status=False)
-            return {
-                "status": 500,
-                "msg": "提交失败！"
-            }
-
-
-async def jiangxi(user_id: int) -> dict:
-    """
-    江西共青团
-    :param user_id:用户ID
-    :return:
-    """
-    result = await User.filter(user_id=user_id).values()
-    if not result:
-        return {
-            "status": 500,
-            "msg": "用户数据不存在！"
-        }
-    else:
-        name = result[0]["name"]
-        nid = result[0]["dxx_id"]
-        openid = result[0]["openid"]
-        if result[0]["mobile"]:
-            suborg = result[0]["mobile"]
-        else:
-            suborg = ''
-        answer = await Answer.all().order_by("time").values()
-        try:
-            url = f"http://www.jxqingtuan.cn/pub/vol/volClass/index?userId={random.randint(4363000, 4364000)}"
-            headers.update({
-                'Cookie': 'JSESSIONID=' + secrets.token_urlsafe(40),
-                'Host': 'www.jxqingtuan.cn',
-                'Origin': 'http://www.jxqingtuan.cn',
-                'Referer': 'http://www.jxqingtuan.cn/html/h5_index.html?&accessToken=' + openid,
-            })
-            async with AsyncClient(headers=headers) as client:
-                course = await client.get(url=url)
-            course.encoding = course.charset_encoding
-            if json.loads(course.text).get('code') == 0:
-                title = json.loads(course.text).get("list")[0].get("title")
-                course = json.loads(course.text).get('list')[0].get('id')
-                resp_url = 'http://www.jxqingtuan.cn/pub/vol/volClass/join?accessToken='
-                data = {"course": course, "nid": nid, "cardNo": name, "subOrg": suborg}
-                async with AsyncClient(headers=headers) as client:
-                    res = await client.post(url=resp_url, json=data)
-                    res.encoding = res.charset_encoding
-                resp = json.loads(res.text)
-                if resp.get("status") == 200:
-                    await User.filter(user_id=user_id).update(
-                        commit_time=time.time(),
-                        catalogue=title
-                    )
-                    await commit(user_id=user_id, catalogue=title, status=True)
-                    return {
-                        "status": 0,
-                        "catalogue": title,
-                        "msg": "提交成功！"
-                    }
-                else:
-                    await commit(user_id=user_id, catalogue=title, status=False)
-                    return {
-                        "status": 500,
-                        "msg": "提交失败！"
-                    }
-        except Exception as e:
-            logger.error(e)
-            await commit(user_id=user_id, catalogue=answer[-1]["catalogue"], status=False)
-            return {
-                "status": 500,
-                "msg": "提交失败！"
-            }
-
-
-async def zhejiang(user_id: int) -> dict:
-    """
-    青春浙江
-    :param user_id:
-    :return:
-    """
-    result = await User.filter(user_id=user_id).values()
-    if not result:
-        return {
-            "status": 500,
-            "msg": "用户数据不存在！"
-        }
-    else:
-        nickname = result[0]["token"]
-        name = result[0]["name"]
-        nid = result[0]["dxx_id"]
-        openid = result[0]["openid"]
-        cookie = result[0]["cookie"]
-        if result[0]["mobile"]:
-            suborg = result[0]["mobile"]
-        else:
-            suborg = None
-        answer = await Answer.all().order_by("time").values()
-        try:
-            headers = {
-                "Host": "qczj.h5yunban.com",
-                "Connection": "keep-alive",
-                "Accept": "application/json, text/javascript, */*; q=0.01",
-                "X-Requested-With": "XMLHttpRequest",
-                "User-Agent": "Mozilla/5.0 (Linux; Android 12; M2007J3SC Build/SKQ1.220303.001; wv) AppleWebKit/537.36 (KHTML, like Gecko) Version/4.0 Chrome/86.0.4240.99 XWEB/3262 MMWEBSDK/20220204 Mobile Safari/537.36 MMWEBID/6170 MicroMessenger/8.0.20.2100(0x28001438) Process/toolsmp WeChat/arm32 Weixin NetType/WIFI Language/zh_CN ABI/arm64",
-                "Content-Type": "application/json;charset=UTF-8",
-                "Sec-Fetch-Site": "same-origin",
-                "Sec-Fetch-Mode": "cors",
-                "Sec-Fetch-Dest": "empty",
-                "Accept-Encoding": "gzip, deflate",
-                "Accept-Language": "zh-CN,zh;q=0.9,en-US;q=0.8,en;q=0.7",
-            }
-            url = f"https://qczj.h5yunban.com/qczj-youth-learning/cgi-bin/login/we-chat/callback?callback=https%3A%2F%2Fqczj.h5yunban.com%2Fqczj-youth-learning%2Findex.php&scope=snsapi_userinfo&appid=wx56b888a1409a2920&openid={openid}&nickname={nickname}&headimg={cookie}&time={int(time.time())}&source=common&sign=&t={int(time.time())}"
-            async with AsyncClient(headers=headers) as client:
-                response = await client.get(url)
-            response.encoding = response.charset_encoding
-            accessToken = re.findall(r"\(\'accessToken\'\,\s+\'(.+?)\'\)", response.text)[0]
-            study_url = f"https://qczj.h5yunban.com/qczj-youth-learning/cgi-bin/common-api/course/current?accessToken={accessToken}"
-            async with AsyncClient(headers=headers, max_redirects=5, timeout=10) as client:
-                response = await client.get(url=study_url)
-            response.encoding = response.charset_encoding
-            if response.json()['status'] == 200:
-                title = response.json()["result"]['title']
-                course = response.json()['result']['id']
-                commit_url = f"https://qczj.h5yunban.com/qczj-youth-learning/cgi-bin/user-api/course/join?accessToken={accessToken}"
-                params = {
-                    "course": course,
-                    "subOrg": suborg,
-                    "nid": nid,
-                    "cardNo": name
-                }
-                async with AsyncClient(headers=headers, timeout=10, max_redirects=5) as client:
-                    response = await client.post(url=commit_url, json=params)
-                response.encoding = response.charset_encoding
-                if response.json()['status'] == 200:
-                    await User.filter(user_id=user_id).update(
-                        commit_time=time.time(),
-                        catalogue=title
-                    )
-                    await commit(user_id=user_id, catalogue=title, status=True)
-                    return {
-                        "status": 0,
-                        "catalogue": title,
-                        "msg": "提交成功！"
-                    }
-                else:
-                    await commit(user_id=user_id, catalogue=title, status=False)
-                    return {
-                        "status": 500,
-                        "msg": "提交失败！"
-                    }
-        except Exception as e:
-            logger.error(e)
-            await commit(user_id=user_id, catalogue=answer[-1]["catalogue"], status=False)
-            return {
-                "status": 500,
-                "msg": "提交失败！"
-            }
-
-
-async def shanghai(user_id: int) -> dict:
-    """
-    青春上海
-    :param user_id:
-    :return:
-    """
-    result = await User.filter(user_id=user_id).values()
-    if not result:
-        return {
-            "status": 500,
-            "msg": "用户数据不存在！"
-        }
-    else:
-        nickname = result[0]["token"]
-        name = result[0]["name"]
-        nid = result[0]["dxx_id"]
-        openid = result[0]["openid"]
-        cookie = result[0]["cookie"]
-        if result[0]["mobile"]:
-            suborg = result[0]["mobile"]
-        else:
-            suborg = None
-        answer = await Answer.all().order_by("time").values()
-        try:
-            headers = {
-                "Host": "qcsh.h5yunban.com",
-                "Connection": "keep-alive",
-                "Accept": "application/json, text/javascript, */*; q=0.01",
-                "X-Requested-With": "XMLHttpRequest",
-                "User-Agent": "Mozilla/5.0 (Linux; Android 12; M2007J3SC Build/SKQ1.220303.001; wv) AppleWebKit/537.36 (KHTML, like Gecko) Version/4.0 Chrome/86.0.4240.99 XWEB/3262 MMWEBSDK/20220204 Mobile Safari/537.36 MMWEBID/6170 MicroMessenger/8.0.20.2100(0x28001438) Process/toolsmp WeChat/arm32 Weixin NetType/WIFI Language/zh_CN ABI/arm64",
-                "Content-Type": "application/json;charset=UTF-8",
-                "Sec-Fetch-Site": "same-origin",
-                "Sec-Fetch-Mode": "cors",
-                "Sec-Fetch-Dest": "empty",
-                "Referer": "https://qcsh.h5yunban.com/youth-learning/signUp.php?rv=2020",
-                "Accept-Encoding": "gzip, deflate",
-                "Accept-Language": "zh-CN,zh;q=0.9,en-US;q=0.8,en;q=0.7",
-            }
-            url = f"https://qcsh.h5yunban.com/youth-learning/cgi-bin/login/we-chat/callback?appid=wxa693f4127cc93fad&openid={openid}&nickname={nickname}&headimg={cookie}&callback=https://qcsh.h5yunban.com/youth-learning/&scope=snsapi_userinfo"
-            async with AsyncClient(headers=headers) as client:
-                response = await client.get(url)
-            response.encoding = response.charset_encoding
-            accessToken = re.findall(r"\(\'accessToken\'\,\s+\'(.+?)\'\)", response.text)[0]
-            study_url = f"https://qcsh.h5yunban.com/youth-learning/cgi-bin/common-api/course/current?accessToken={accessToken}"
-            async with AsyncClient(headers=headers, max_redirects=5, timeout=10) as client:
-                response = await client.get(url=study_url)
-            response.encoding = response.charset_encoding
-            if response.json()['status'] == 200:
-                title = response.json()["result"]['title']
-                course = response.json()['result']['id']
-                commit_url = f"https://qcsh.h5yunban.com/youth-learning/cgi-bin/user-api/course/join?accessToken={accessToken}"
-                params = {
-                    "course": course,
-                    "subOrg": suborg,
-                    "nid": nid,
-                    "cardNo": name
-                }
-                async with AsyncClient(headers=headers, timeout=10, max_redirects=5) as client:
-                    response = await client.post(url=commit_url, json=params)
-                response.encoding = response.charset_encoding
-                if response.json()['status'] == 200:
-                    await User.filter(user_id=user_id).update(
-                        commit_time=time.time(),
-                        catalogue=title
-                    )
-                    await commit(user_id=user_id, catalogue=title, status=True)
-                    return {
-                        "status": 0,
-                        "catalogue": title,
-                        "msg": "提交成功！"
-                    }
-                else:
-                    await commit(user_id=user_id, catalogue=title, status=False)
-                    return {
-                        "status": 500,
-                        "msg": "提交失败！"
-                    }
-        except Exception as e:
-            logger.error(e)
-            await commit(user_id=user_id, catalogue=answer[-1]["catalogue"], status=False)
-            return {
-                "status": 500,
-                "msg": "提交失败！"
-            }
-
-
-async def jiangsu(user_id: int) -> dict:
-    """
-    江苏共青团
-    :param user_id:用户ID
-    :return:
-    """
-    result = await User.filter(user_id=user_id).values()
-    if not result:
-        return {
-            "status": 500,
-            "msg": "用户数据不存在！"
-        }
-    else:
-        cookie = result[0]["cookie"]
-        answer = await Answer.all().order_by("time").values()
-        headers = {
-            "Host": "service.jiangsugqt.org",
-            "Connection": "keep-alive",
-            "Upgrade-Insecure-Requests": '1',
-            "User-Agent": "Mozilla/5.0 (Linux; Android 12; M2007J3SC Build/SKQ1.220303.001; wv) AppleWebKit/537.36 (KHTML, like Gecko) Version/4.0 Chrome/86.0.4240.99 XWEB/3262 MMWEBSDK/20220204 Mobile Safari/537.36 MMWEBID/6170 MicroMessenger/8.0.20.2100(0x28001438) Process/toolsmp WeChat/arm32 Weixin NetType/WIFI Language/zh_CN ABI/arm64",
-            "Accept": "text/html,application/xhtml+xml,application/xml;q=0.9,image/avif,image/wxpic,image/tpg,image/webp,image/apng,*/*;q=0.8,application/signed-exchange;v=b3;q=0.9",
-            "X-Requested-With": "com.tencent.mm",
-            "Sec-Fetch-Site": "none",
-            "Sec-Fetch-Mode": "navigate",
-            "Sec-Fetch-User": "?1",
-            "Sec-Fetch-Dest": "document",
-            "Accept-Encoding": "gzip, deflate",
-            "Accept-Language": "zh-CN,zh;q=0.9,en-US;q=0.8,en;q=0.7",
-            "Cookie": cookie
-        }
-        try:
-            url = "https://service.jiangsugqt.org/api/lessons"
-            params = {"pages": 1, "limit": 5}
-            async with AsyncClient(headers=headers) as client:
-                response = await client.post(url=url, json=params)
-            response.encoding = response.charset_encoding
-            result = response.json()
-            if result["status"] == 1:
-                params = {
-                    "lesson_id": result["data"][0]["id"]
-                }
-                title = result["data"][0]["title"]
-                commit_url = "https://service.jiangsugqt.org/api/doLesson"
-                async with AsyncClient(headers=headers) as client:
-                    response = await client.post(url=commit_url, json=params)
-                response.encoding = response.charset_encoding
-                result = response.json()
-                if result["status"] == 1:
-                    await User.filter(user_id=user_id).update(
-                        commit_time=time.time(),
-                        catalogue=result["data"]["title"]
-                    )
-                    await commit(user_id=user_id, catalogue=result["data"]["title"], status=True)
-                    return {
-                        "status": 0,
-                        "catalogue": result["data"]["title"],
-                        "msg": "提交成功！"
-                    }
-                else:
-                    await commit(user_id=user_id, catalogue=title, status=False)
-                    return {
-                        "status": 500,
-                        "msg": "提交失败！"
-                    }
-            else:
-                await commit(user_id=user_id, catalogue=answer[-1]["catalogue"], status=False)
-                return {
-                    "status": 500,
-                    "msg": "提交失败！"
-                }
-        except Exception as e:
-            logger.error(e)
-            await commit(user_id=user_id, catalogue=answer[-1]["catalogue"], status=False)
-            return {
-                "status": 500,
-                "msg": "提交失败！"
-            }
-
-
-async def anhui(user_id: int) -> dict:
-    """
-    安徽共青团
-    :param user_id:用户ID
-    :return:
-    """
-    result = await User.filter(user_id=user_id).values()
-    if not result:
-        return {
-            "status": 500,
-            "msg": "用户数据不存在！"
-        }
-    else:
-        username = result[0]['name']
-        gender = result[0]['gender']
-        mobile = result[0]['mobile']
-        level1 = result[0]['university_type']
-        level2 = result[0]['university']
-        level3 = result[0]['college']
-        level4 = result[0]['organization']
-        level5 = result[0]['organization_id']
-        token = result[0]["token"]
-        answer = await Answer.all().order_by("time").values()
-        try:
-            headers.update({
-                "Host": "dxx.ahyouth.org.cn",
-                "Accept": "application/json, text/plain, */*",
-                "Accept-Language": "zh-CN,zh;q=0.9,en-US;q=0.8,en;q=0.7",
-                "Referer": "http://dxx.ahyouth.org.cn/",
-                "Accept-Encoding": "gzip, deflate",
-                "Connection": "keep-alive",
-                'Content-Type': 'application/x-www-form-urlencoded',
-                "X-Requested-With": 'com.tencent.mm',
-                "Origin": 'http://dxx.ahyouth.org.cn',
-                "token": token
-            })
-            data = {
-                'username': username,
-                'gender': gender,
-                'mobile': mobile,
-                'level1': level1,
-                'level2': level2,
-                'level3': level3,
-                'level4': level4,
-                'level5': level5
-            }
-            get_infor_url = 'http://dxx.ahyouth.org.cn/api/saveUserInfo'
-            async with AsyncClient(headers=headers, timeout=30, max_redirects=5) as client:
-                infor_response = await client.post(url=get_infor_url, params=data)
-            infor_response.encoding = infor_response.charset_encoding
-            infor_response_json = infor_response.json()
-            if infor_response_json['code'] == 200:
-                username = infor_response_json['content']['username']
-                token = infor_response_json['content']['token']
-                gender = infor_response_json['content']['gender']
-                mobile = infor_response_json['content']['mobile']
-                level1 = infor_response_json['content']['level1']
-                level2 = infor_response_json['content']['level2']
-                level3 = infor_response_json['content']['level3']
-                level4 = infor_response_json['content']['level4']
-                level5 = infor_response_json['content']['level5']
-                headers.update({
-                    "Host": "dxx.ahyouth.org.cn",
-                    "Accept": "application/json, text/plain, */*",
-                    "Accept-Language": "zh-CN,zh;q=0.9,en-US;q=0.8,en;q=0.7",
-                    "Referer": "http://dxx.ahyouth.org.cn/",
-                    "Accept-Encoding": "gzip, deflate",
-                    "Connection": "keep-alive",
-                    'Content-Type': 'application/x-www-form-urlencoded',
-                    "X-Requested-With": 'com.tencent.mm',
-                    "Origin": 'http://dxx.ahyouth.org.cn',
-                    "token": token
-                })
-                data = {
-                    'username': username,
-                    'gender': gender,
-                    'mobile': mobile,
-                    'level1': level1,
-                    'level2': level2,
-                    'level3': level3,
-                    'level4': level4,
-                    'level5': level5
-                }
-                commit_url = 'http://dxx.ahyouth.org.cn/api/newLearn'
-                async with AsyncClient(headers=headers, timeout=30, max_redirects=5) as client:
-                    commit_response = await client.post(url=commit_url, params=data)
-                commit_response.encoding = commit_response.charset_encoding
-                commit_response_json = commit_response.json()
-                if commit_response_json['code'] == 200:
-                    await User.filter(user_id=user_id).update(
-                        token=token,
-                        commit_time=time.time(),
-                        catalogue=answer[-1]["catalogue"]
-                    )
-                    await commit(user_id=user_id, catalogue=answer[-1]["catalogue"], status=True)
-                    return {
-                        "status": 0,
-                        "catalogue": answer[-1]["catalogue"],
-                        "msg": "提交成功！"
-                    }
-                else:
-                    await commit(user_id=user_id, catalogue=answer[-1]["catalogue"], status=False)
-                    return {
-                        "status": 500,
-                        "msg": "提交失败！"
-                    }
-            else:
-                await commit(user_id=user_id, catalogue=answer[-1]["catalogue"], status=False)
-                return {
-                    "status": 500,
-                    "msg": "提交失败！"
-                }
-        except Exception as e:
-            logger.error(e)
-            await commit(user_id=user_id, catalogue=answer[-1]["catalogue"], status=False)
-            return {
-                "status": 500,
-                "msg": "提交失败！"
-            }
-
-
-async def sichuan(user_id: int) -> dict:
-    """
-    天府新青年
-    :param user_id:
-    :return:
-    """
-    result = await User.filter(user_id=user_id).values()
-    if not result:
-        return {
-            "status": 500,
-            "msg": "用户数据不存在！"
-        }
-    else:
-        token = result[0]["token"]
-        university_type = result[0]["university_type"]
-        university_id = result[0]["university_id"]
-        university = result[0]["university"]
-        name = result[0]["name"]
-        mobile = result[0]["mobile"]
-        college_id = result[0]["college_id"]
-        college = result[0]["college"]
-        organization_id = result[0]["organization_id"]
-        organization = result[0]["organization"]
-        dxx_id = result[0]["dxx_id"]
-        data_json = {
-            "name": name,
-            "tel": mobile,
-            "org": f"#{dxx_id}#{university_id}#{college_id}#{organization_id}#",
-            "lastOrg": organization_id,
-            "orgName": organization,
-            "allOrgName": f"#{university_type}#{university}#{college}#{organization}#"
-        }
-        headers.update({
-            "Referer": 'http://scyol.com/v_prod6.02/',
-            "Host": "dxx.scyol.com",
-            "Connection": "keep-alive",
-            "Content_Length": '9',
-            "Content_Type": "application/json",
-            "Accept": "*/*",
-            "User-Agent": "Mozilla/5.0 (Linux; Android 11; M2007J3SC Build/SKQ1.220213.001; wv) AppleWebKit/537.36 (KHTML, like Gecko) Version/4.0 Chrome/86.0.4240.99 XWEB/3224 MMWEBSDK/20210902 Mobile Safari/537.36 MMWEBID/6170 MicroMessenger/8.0.15.2020(0x28000F30) Process/toolsmp WeChat/arm32 Weixin NetType/WIFI Language/zh_CN ABI/arm64",
-            "Origin": "http://scyol.com",
-            "X-Requested-With": "com.tencent.mm",
-            "Sec-Fetch-Site": "same-origin",
-            "Sec-Fetch-Mode": "cors",
-            "Sec-Fetch-Dest": "empty",
-            "token": token,
-            "Accept-Encoding": "gzip, deflate",
-            "Accept-Language": "zh-CN,zh;q=0.9,en-US;q=0.8,en;q=0.7",
-        })
-        answer = await Answer.all().order_by("time").values()
-        title = answer[-1]["catalogue"]
-        url = 'https://dxx.scyol.com/api/student/commit'
-        try:
-            async with AsyncClient(headers=headers) as client:
-                response = await client.post(url=url, json=data_json)
-            if response.status_code == 200:
-                response.encoding = response.charset_encoding
-                if response.json()["code"] == 2:
-                    await User.filter(user_id=user_id).update(
-                        commit_time=time.time(),
-                        catalogue=title
-                    )
-                    await commit(user_id=user_id, catalogue=title, status=True)
-                    return {
-                        "status": 0,
-                        "catalogue": title,
-                        "msg": "你已经提交了，请勿重复提交哦"
-                    }
-                elif response.json()["code"] == 200:
-                    await User.filter(user_id=user_id).update(
-                        commit_time=time.time(),
-                        catalogue=title
-                    )
-                    await commit(user_id=user_id, catalogue=title, status=True)
-                    return {
-                        "status": 0,
-                        "catalogue": title,
-                        "msg": "提交成功！"
-                    }
-                else:
-                    await commit(user_id=user_id, catalogue=answer[-1]["catalogue"], status=False)
-                    return {
-                        "status": 500,
-                        "msg": "提交失败！"
-                    }
-            else:
-                return {
-                    "status": 500,
-                    "msg": "提交失败,cookie失效！"
-                }
-        except Exception as e:
-            return {
-                "status": 500,
-                "msg": f"提交失败,{e}"
-            }
-
-
-async def shandong(user_id: int) -> dict:
-    """
-    青春山东
-    :param user_id: 用户ID
-    :return:
-    """
-    result = await User.filter(user_id=user_id).values()
-    if not result:
-        return {
-            "status": 500,
-            "msg": "用户数据不存在！"
-        }
-    else:
-        openid = result[0]["openid"]
-        cookie = result[0]["cookie"]
-        answer = await Answer.all().order_by("time").values()
-        title = answer[-1]["catalogue"]
-        headers.update({
-            "Host": "qndxx.youth54.cn",
-            "Connection": "keep-alive",
-            "Accept": "*/*",
-            "User-Agent": "Mozilla/5.0 (Linux; Android 12; M2007J3SC Build/SKQ1.220213.001; wv) AppleWebKit/537.36 (KHTML, like Gecko) Version/4.0 Chrome/86.0.4240.99 XWEB/3234 MMWEBSDK/20210902 Mobile Safari/537.36 MMWEBID/6170 MicroMessenger/8.0.15.2020(0x28000F30) Process/toolsmp WeChat/arm32 Weixin NetType/WIFI Language/zh_CN ABI/arm64",
-            "X-Requested-With": "XMLHttpRequest",
-            "Content-Type": "application/x-www-form-urlencoded; charset=UTF-8",
-            "Origin": "http://qndxx.youth54.cn",
-            "Referer": "http://qndxx.youth54.cn/SmartLA/dxx.w?method=pageSdtwdt",
-            "Accept-Encoding": "gzip, deflate",
-            "Accept-Language": "zh-CN,zh;q=0.9,en-US;q=0.8,en;q=0.7",
-            "Cookie": cookie
-        })
-        try:
-            version_url = f'http://qndxx.youth54.cn/SmartLA/dxxjfgl.w?method=getNewestVersionInfo&openid={openid}'
-            async with AsyncClient(headers=headers) as client:
-                version_response = await client.post(url=version_url)
-            if version_response.status_code == 200:
-                version_response.encoding = version_response.charset_encoding
-                content = version_response.json()
-                if content["errcode"] == "0":
-                    versionname = content['versionname']
-                    version = content['version']
-                    headers.update({
-                        "Host": "qndxx.youth54.cn",
-                        "Connection": "keep-alive",
-                        "Accept": "*/*",
-                        "User-Agent": "Mozilla/5.0 (Linux; Android 12; M2007J3SC Build/SKQ1.220213.001; wv) AppleWebKit/537.36 (KHTML, like Gecko) Version/4.0 Chrome/86.0.4240.99 XWEB/3234 MMWEBSDK/20210902 Mobile Safari/537.36 MMWEBID/6170 MicroMessenger/8.0.15.2020(0x28000F30) Process/toolsmp WeChat/arm32 Weixin NetType/WIFI Language/zh_CN ABI/arm64",
-                        "X-Requested-With": "XMLHttpRequest",
-                        "Content-Type": "application/x-www-form-urlencoded; charset=UTF-8",
-                        "Origin": "http://qndxx.youth54.cn",
-                        "Referer": "http://qndxx.youth54.cn/SmartLA/dxx.w?method=pageSdtwdt",
-                        "Accept-Encoding": "gzip, deflate",
-                        "Accept-Language": "zh-CN,zh;q=0.9,en-US;q=0.8,en;q=0.7",
-                        "Cookie": cookie
-                    })
-                    data = {
-                        'openid': openid,
-                        'version': version
-                    }
-                    commit_url = 'http://qndxx.youth54.cn/SmartLA/dxxjfgl.w?method=studyLatest'
-                    async with AsyncClient(headers=headers) as client:
-                        response = await client.post(url=commit_url, params=data)
-                    if response.status_code == 200:
-                        response.encoding = response.charset_encoding
-                        if response.json()["errcode"] == "0":
-                            await User.filter(user_id=user_id).update(
-                                commit_time=time.time(),
-                                catalogue=versionname
-                            )
-                            await commit(user_id=user_id, catalogue=versionname, status=True)
-                            return {
-                                "status": 0,
-                                "catalogue": versionname,
-                                "msg": "提交成功！"
-                            }
-                        else:
-                            await commit(user_id=user_id, catalogue=versionname, status=False)
-                            return {
-                                "status": 500,
-                                "msg": "提交失败！"
-                            }
-                    else:
-                        await commit(user_id=user_id, catalogue=versionname, status=False)
-                        return {
-                            "status": 500,
-                            "msg": "提交失败！"
-                        }
-                else:
-                    await commit(user_id=user_id, catalogue=title, status=False)
-                    return {
-                        "status": 500,
-                        "msg": "提交失败！"
-                    }
-            else:
-                await commit(user_id=user_id, catalogue=title, status=False)
-                return {
-                    "status": 500,
-                    "msg": "提交失败！"
-                }
-        except Exception as e:
-            await commit(user_id=user_id, catalogue=title, status=False)
-            return {
-                "status": 500,
-                "msg": f"提交失败,{e}"
-            }
-
-
-async def chongqing(user_id: int) -> dict:
-    """
-    重庆共青团
-    :param user_id:
-    :return:
-    """
-    result = await User.filter(user_id=user_id).values()
-    if not result:
-        return {
-            "status": 500,
-            "msg": "用户数据不存在！"
-        }
-    else:
-        openid = result[0]["openid"]
-        answer = await Answer.all().order_by("time").values()
-        title = answer[-1]["catalogue"]
-        headers.update(
-            {
-                "Host": "qndxx.cqyouths.com",
-                "Connection": "keep-alive",
-                "Accept": "application/json, text/plain, */*",
-                "User-Agent": "Mozilla/5.0 (Linux; Android 12; M2007J3SC Build/SKQ1.220303.001; wv) AppleWebKit/537.36 (KHTML, like Gecko) Version/4.0 Chrome/86.0.4240.99 XWEB/3262 MMWEBSDK/20220204 Mobile Safari/537.36 MMWEBID/6170 MicroMessenger/8.0.20.2100(0x28001438) Process/toolsmp WeChat/arm32 Weixin NetType/WIFI Language/zh_CN ABI/arm64",
-                "X-Requested-With": "com.tencent.mm",
-                "Accept-Encoding": "gzip, deflate",
-                "Accept-Language": "zh-CN,zh;q=0.9,en-US;q=0.8,en;q=0.7"
-            }
-        )
-        try:
-            new_url = f"http://qndxx.cqyouths.com/new_course.json?time={int(time.time())}"
-            async with AsyncClient(headers=headers) as client:
-                new_response = await client.get(url=new_url)
-            if new_response.status_code == 200:
-                new_response.encoding = new_response.charset_encoding
-                course_id = new_response.json()['data'][0]['id']
-                commit_url = f"http://qndxx.cqyouths.com/api/course/studyCourse?openid={openid}&id={course_id}"
-                async with AsyncClient(headers=headers) as client:
-                    response = await client.get(url=commit_url)
-                if response.status_code == 200:
-                    response.encoding = response.charset_encoding
-                    if response.json()["status"] == 200:
-                        await User.filter(user_id=user_id).update(
-                            commit_time=time.time(),
-                            catalogue=title
-                        )
-                        await commit(user_id=user_id, catalogue=title, status=True)
-                        return {
-                            "status": 0,
-                            "catalogue": title,
-                            "msg": "提交成功！"
-                        }
-                    elif response.json()["status"] == 201:
-                        await User.filter(user_id=user_id).update(
-                            commit_time=time.time(),
-                            catalogue=title
-                        )
-                        await commit(user_id=user_id, catalogue=title, status=True)
-                        return {
-                            "status": 0,
-                            "catalogue": title,
-                            "msg": "提交成功！"
-                        }
-                    else:
-                        await commit(user_id=user_id, catalogue=title, status=False)
-                        return {
-                            "status": 500,
-                            "msg": "提交失败！"
-                        }
-                else:
-                    await commit(user_id=user_id, catalogue=title, status=False)
-                    return {
-                        "status": 500,
-                        "msg": "提交失败！"
-                    }
-            else:
-                await commit(user_id=user_id, catalogue=title, status=False)
-                return {
-                    "status": 500,
-                    "msg": "提交失败！"
-                }
-        except Exception as e:
-            logger.error(e)
-            return {
-                "status": 500,
-                "msg": f"提交失败,{e}"
-            }
-
-
-async def jilin(user_id: int) -> dict:
-    """
-    吉青飞扬
-    :param user_id:
-    :return:
-    """
-    result = await User.filter(user_id=user_id).values()
-    if not result:
-        return {
-            "status": 500,
-            "msg": "用户数据不存在！"
-        }
-    else:
-        openid = result[0]["openid"]
-        dxx_id = result[0]["dxx_id"]
-        answer = await Answer.all().order_by("time").values()
-        title = answer[-1]["catalogue"]
-        headers.update(
-            {
-                "Host": "jqfy.jl54.org",
-                "Connection": "keep-alive",
-                "Upgrade-Insecure-Requests": "1",
-                "User-Agent": "Mozilla/5.0 (Linux; Android 12; M2007J3SC Build/SKQ1.220303.001; wv) AppleWebKit/537.36 (KHTML, like Gecko) Version/4.0 Chrome/86.0.4240.99 XWEB/3262 MMWEBSDK/20220204 Mobile Safari/537.36 MMWEBID/6170 MicroMessenger/8.0.20.2100(0x28001438) Process/toolsmp WeChat/arm32 Weixin NetType/WIFI Language/zh_CN ABI/arm64",
-                "Accept": "text/html,application/xhtml+xml,application/xml;q=0.9,image/avif,image/wxpic,image/tpg,image/webp,image/apng,*/*;q=0.8,application/signed-exchange;v=b3;q=0.9",
-                "X-Requested-With": "com.tencent.mm",
-                "Accept-Encoding": "gzip, deflate",
-                "Accept-Language": "zh-CN,zh;q=0.9,en-US;q=0.8,en;q=0.7"
-            }
-        )
-        try:
-            commit_url = f"http://jqfy.jl54.org/jltw/wechat/editStudyRecord/{dxx_id}"
-            data = {
-                "openid": openid
-            }
-            async with AsyncClient(headers=headers) as client:
-                response = await client.post(url=commit_url, params=data)
-            if response.status_code == 200:
-                response.encoding = response.charset_encoding
-                if response.json()["code"] == '0001':
-                    await User.filter(user_id=user_id).update(
-                        commit_time=time.time(),
-                        catalogue=title
-                    )
-                    await commit(user_id=user_id, catalogue=title, status=True)
-                    return {
-                        "status": 0,
-                        "catalogue": title,
-                        "msg": "提交成功！"
-                    }
-                else:
-                    await commit(user_id=user_id, catalogue=title, status=False)
-                    return {
-                        "status": 500,
-                        "msg": f"提交失败!"
-                    }
-            else:
-                await commit(user_id=user_id, catalogue=title, status=False)
-                return {
-                    "status": 500,
-                    "msg": "提交失败！"
-                }
-        except Exception as e:
-            logger.error(e)
-            return {
-                "status": 500,
-                "msg": f"提交失败,{e}"
-            }
-
-
-async def guangdong(user_id: int) -> dict:
-    """
-    广东共青团
-    :param user_id:用户ID
-    :return:
-    """
-    result = await User.filter(user_id=user_id).values()
-    if not result:
-        return {
-            "status": 500,
-            "msg": "用户数据不存在！"
-        }
-    else:
-        dxx_id = result[0]['dxx_id']
-        token = result[0]["token"]
-        answer = await Answer.all().order_by("time").values()
-        try:
-            study_headers = {
-                'Host': 'youthstudy.12355.net',
-                'Connection': 'keep-alive',
-                'X-Litemall-Token': token,
-                'X-Litemall-IdentiFication': 'young',
-                'User-Agent': 'MicroMessenger',
-                'Accept': '*/*',
-                'Origin': 'https://youthstudy.12355.net',
-                'X-Requested-With': 'com.tencent.mm',
-                'Sec-Fetch-Site': 'same-origin',
-                'Sec-Fetch-Mode': 'cors',
-                'Sec-Fetch-Dest': 'empty',
-                'Referer': 'https://youthstudy.12355.net/h5/',
-                'Accept-Language': 'zh-CN,zh;q=0.9,en-US;q=0.8,en;q=0.7',
-            }
-            new_study_url = "https://youthstudy.12355.net/saomah5/api/young/chapter/new"
-            async with AsyncClient(headers=study_headers, timeout=30, max_redirects=5) as client:
-                study_response = await client.get(url=new_study_url)
-            study_response.encoding=study_response.charset_encoding
-            if study_response.json()["errno"] == 0:
-                chapterId = study_response.json().get('data').get('entity').get('id')
-                title = study_response.json().get('data').get('entity').get('name').replace('“青年大学习”', "").strip()
-                commit_url = "https://youthstudy.12355.net/saomah5/api/young/course/chapter/saveHistory"
-                async with AsyncClient(headers=study_headers, timeout=30, max_redirects=5) as client:
-                    commit_response = await client.post(url=commit_url, data={
-                        "chapterId": chapterId
-                    })
-                if commit_response.json()["errno"] == 0:
-                    await User.filter(user_id=user_id).update(
-                        token=token,
-                        commit_time=time.time(),
-                        catalogue=title
-                    )
-                    await commit(user_id=user_id, catalogue=title, status=True)
-                    return {
-                        "status": 0,
-                        "catalogue": title,
-                        "msg": "提交成功！"
-                    }
-                else:
-                    await commit(user_id=user_id, catalogue=answer[-1]["catalogue"], status=False)
-                    return {
-                        "status": 500,
-                        "msg": "提交失败！"
-                    }
-            else:
-                token_headers = {
-                    'Host': 'tuanapi.12355.net',
-                    'Connection': 'keep-alive',
-                    'Accept': 'application/json, text/javascript, */*; q=0.01',
-                    'Origin': 'https://tuan.12355.net',
-                    'User-Agent': 'MicroMessenger',
-                    'X-Requested-With': 'com.tencent.mm',
-                    'Sec-Fetch-Site': 'same-site',
-                    'Sec-Fetch-Mode': 'cors',
-                    'Referer': 'https://tuan.12355.net/wechat/view/YouthLearning/page.html',
-                    'Accept-Encoding': 'gzip, deflate',
-                    'Accept-Language': 'zh-CN,zh;q=0.9,en-US;q=0.8,en;q=0.7',
-                }
-                ger_param_url = f"https://tuanapi.12355.net/questionnaire/getYouthLearningUrl?mid={dxx_id}"
-                async with AsyncClient(headers=token_headers, timeout=30, max_redirects=5) as client:
-                    param_response = await client.get(url=ger_param_url)
-                    if param_response.json()["status"] == 200:
-                        content = param_response.json()["youthLearningUrl"].split("=")[-1]
-                        token_url = "https://youthstudy.12355.net/apih5/api/user/get"
-                        token_headers = {
-                            'Host': 'youthstudy.12355.net',
-                            'Connection': 'keep-alive',
-                            'Content-Length': '134',
-                            'Origin': 'https://youthstudy.12355.net',
-                            'X-Litemall-Token': '',
-                            'X-Litemall-IdentiFication': 'young',
-                            'User-Agent': 'MicroMessenger',
-                            'Content-Type': 'application/x-www-form-urlencoded',
-                            'Accept': '*/*',
-                            'X-Requested-With': 'com.tencent.mm',
-                            'Sec-Fetch-Site': 'same-origin',
-                            'Sec-Fetch-Mode': 'cors',
-                            'Referer': 'https://youthstudy.12355.net/h5/',
-                            'Accept-Encoding': 'gzip, deflate',
-                            'Accept-Language': 'zh-CN,zh;q=0.9,en-US;q=0.8,en;q=0.7'
-                        }
-                        async with AsyncClient(headers=token_headers, timeout=30, max_redirects=5) as client:
-                            token_response = await client.post(url=token_url, data="sign="+urllib.parse.quote(content))
-                        if token_response.json()["errno"] == 0:
-                            token = token_response.json()['data']['entity']['token']
-                            study_headers = {
-                                'Host': 'youthstudy.12355.net',
-                                'Connection': 'keep-alive',
-                                'X-Litemall-Token': token,
-                                'X-Litemall-IdentiFication': 'young',
-                                'User-Agent': 'MicroMessenger',
-                                'Accept': '*/*',
-                                'Origin': 'https://youthstudy.12355.net',
-                                'X-Requested-With': 'com.tencent.mm',
-                                'Sec-Fetch-Site': 'same-origin',
-                                'Sec-Fetch-Mode': 'cors',
-                                'Sec-Fetch-Dest': 'empty',
-                                'Referer': 'https://youthstudy.12355.net/h5/',
-                                'Accept-Language': 'zh-CN,zh;q=0.9,en-US;q=0.8,en;q=0.7',
-                            }
-                            new_study_url = "https://youthstudy.12355.net/saomah5/api/young/chapter/new"
-                            async with AsyncClient(headers=study_headers, timeout=30, max_redirects=5) as client:
-                                study_response = await client.get(url=new_study_url)
-                            if study_response.json()["errno"] == 0:
-                                chapterId = study_response.json().get('data').get('entity').get('id')
-                                title = study_response.json().get('data').get('entity').get('name').replace(
-                                    '"青年大学习”', "").strip()
-                                commit_url = "https://youthstudy.12355.net/saomah5/api/young/course/chapter/saveHistory"
-                                async with AsyncClient(headers=study_headers, timeout=30, max_redirects=5) as client:
-                                    commit_response = await client.post(url=commit_url, data={
-                                        "chapterId": chapterId
-                                    })
-                                if commit_response.json()["errno"] == 0:
-                                    await User.filter(user_id=user_id).update(
-                                        token=token,
-                                        commit_time=time.time(),
-                                        catalogue=title
-                                    )
-                                    await commit(user_id=user_id, catalogue=title, status=True)
-                                    return {
-                                        "status": 0,
-                                        "catalogue": title,
-                                        "msg": "提交成功！"
-                                    }
-                                else:
-                                    await commit(user_id=user_id, catalogue=answer[-1]["catalogue"], status=False)
-                                    return {
-                                        "status": 500,
-                                        "msg": "提交失败！"
-                                    }
-                        else:
-                            await commit(user_id=user_id, catalogue=answer[-1]["catalogue"], status=False)
-                            return {
-                                "status": 500,
-                                "msg": "提交失败，token获取失效！"
-                            }
-                    else:
-                        await commit(user_id=user_id, catalogue=answer[-1]["catalogue"], status=False)
-                        return {
-                            "status": 500,
-                            "msg": "提交失败，token获取失效！"
-                        }
-        except Exception as e:
-            logger.error(e)
-            await commit(user_id=user_id, catalogue=answer[-1]["catalogue"], status=False)
-            return {
-                "status": 500,
-                "msg": "提交失败！"
-            }
-
-async def heilongjiang(user_id: int) -> dict:
-    """
-    黑龙江共青团
-    :param user_id:用户ID
-    :return:
-    """
-    result = await User.filter(user_id=user_id).values()
-    if not result:
-        return {
-            "status": 500,
-            "msg": "用户数据不存在！"
-        }
-    else:
-        cookie = result[0]["cookie"]
-        answer = await Answer.all().order_by("time").values()
-        headers = {
-            "Host": "tsw.ithyxy.com",
-            "Connection": "keep-alive",
-            "Accept": "application/json, text/plain, */*",
-            "User-Agent": "Mozilla/5.0 (Linux; Android 12; M2007J3SC Build/SKQ1.220303.001; wv) AppleWebKit/537.36 (KHTML, like Gecko) Version/4.0 Chrome/86.0.4240.99 XWEB/3262 MMWEBSDK/20220204 Mobile Safari/537.36 MMWEBID/6170 MicroMessenger/8.0.20.2100(0x28001438) Process/toolsmp WeChat/arm32 Weixin NetType/WIFI Language/zh_CN ABI/arm64",
-            "X-Requested-With": "com.tencent.mm",
-            "Referer": "http://tsw.ithyxy.com/login",
-            "Accept-Encoding": "gzip, deflate",
-            "Accept-Language": "zh-CN,zh;q=0.9,en-US;q=0.8,en;q=0.7",
-            "Cookie": cookie
-        }
-        try:
-            learn_url = "http://tsw.ithyxy.com/h5/learn/home"
-            async with AsyncClient(headers=headers, timeout=5, max_redirects=5) as client:
-                response = await client.get(url=learn_url)
-            response.encoding = response.charset_encoding
-            if response.status_code == 200 and response.json()["code"] == 200:
-                learn_id = response.json()["data"]["id"]
-                commit_url = f"http://tsw.ithyxy.com/h5/learn/enter?id={learn_id}"
-                async with AsyncClient(headers=headers, timeout=5, max_redirects=5) as client:
-                    response = await client.get(url=commit_url)
-                response.encoding = response.charset_encoding
-                if response.status_code == 200 and response.json()["code"] == 200:
-                    await User.filter(user_id=user_id).update(
-                        commit_time=time.time(),
-                        catalogue=answer[-1]["catalogue"]
-                    )
-                    await commit(user_id=user_id, catalogue=answer[-1]["catalogue"], status=True)
-                    return {
-                        "status": 0,
-                        "catalogue": answer[-1]["catalogue"],
-                        "msg": "提交成功！"
-                    }
-                else:
-                    await commit(user_id=user_id, catalogue=answer[-1]["catalogue"], status=False)
-                    return {
-                        "status": 500,
-                        "msg": "提交失败，cookie失效！"
-                    }
-            else:
-                await commit(user_id=user_id, catalogue=answer[-1]["catalogue"], status=False)
-                return {
-                    "status": 500,
-                    "msg": "提交失败，cookie失效！"
-                }
-        except Exception as e:
-            logger.error(e)
-            await commit(user_id=user_id, catalogue=answer[-1]["catalogue"], status=False)
-            return {
-                "status": 500,
-                "msg": "提交失败！"
-            }
+import json
+import random
+import re
+import secrets
+import time
+import urllib.parse
+
+from anti_useragent import UserAgent
+from bs4 import BeautifulSoup
+from ddddocr import DdddOcr
+from httpx import AsyncClient
+from nonebot import logger
+
+from .utils import encrypt
+from ..models.accuont import User, Commit
+from ..models.dxx import Answer
+
+headers = {
+    'Accept': 'application/json, text/plain, */*',
+    'Accept-Encoding': 'gzip, deflate',
+    'Accept-Language': 'zh-CN,zh;q=0.9,en-US;q=0.8,en;q=0.7',
+    'Connection': 'keep-alive',
+    'Content-Type': 'application/json;charset=UTF-8',
+    'User-Agent': UserAgent(platform="iphone", min_version=1, max_version=5).wechat,
+    'X-Requested-With': 'XMLHttpRequest'
+}
+
+
+async def commit(user_id: int, catalogue: str, status: bool = False) -> None:
+    """
+    记录提交状态
+    :param catalogue: 提交期数
+    :param user_id: 用户ID
+    :param status:提交状态，默认为False
+    :return:
+    """
+    result = await User.filter(user_id=user_id).values()
+    await Commit.create(
+        time=time.time(),
+        user_id=user_id,
+        area=result[0]["area"],
+        status=status,
+        name=result[0]["name"],
+        university=result[0]["university"],
+        college=result[0]["college"],
+        organization=result[0]["organization"],
+        catalogue=catalogue
+    )
+
+
+async def hubei(user_id: int) -> dict:
+    """
+    青春湖北
+    :param user_id:用户ID
+    :return:
+    """
+    result = await User.filter(user_id=user_id).values()
+    if not result:
+        return {
+            "status": 500,
+            "msg": "用户数据不存在！"
+        }
+    else:
+        name = result[0]["name"]
+        openid = result[0]["openid"]
+        university = result[0]["university"]
+        college = result[0]["college"]
+        organization = result[0]["organization"]
+        answer = await Answer.all().order_by("time").values()
+        headers.update({
+            "Host": "cp.fjg360.cn",
+            "X-Requested-With": "XMLHttpRequest",
+            "Sec-Fetch-Site": "same-origin",
+            "Sec-Fetch-Mode": "cors",
+            "Sec-Fetch-Dest": "empty",
+            "Accept-Encoding": "gzip, deflate",
+            "Accept-Language": "zh-CN,zh;q=0.9,en-US;q=0.8,en;q=0.7",
+        })
+        url = "https://cp.fjg360.cn/index.php?m=vote&c=index&a=save_door&sessionId=&imgTextId=&ip="
+        url += "&username=" + name
+        url += "&phone=" + "未知"
+        url += "&city=" + university
+        url += "&danwei2=" + organization
+        url += "&danwei=" + college
+        url += "&openid=" + openid
+        url += "&num=10"
+        url += "&lesson_name=" + answer[-1]["catalogue"]
+        try:
+            async with AsyncClient(headers=headers) as client:
+                response = await client.get(url)
+            response_json = json.loads(response.text)
+            if response_json.get('code') == 1:
+                await User.filter(user_id=user_id).update(
+                    commit_time=time.time(),
+                    catalogue=answer[-1]["catalogue"]
+                )
+                await commit(user_id=user_id, catalogue=answer[-1]["catalogue"], status=True)
+                return {
+                    "status": 0,
+                    "catalogue": answer[-1]["catalogue"],
+                    "msg": "提交成功！"
+                }
+            else:
+                await commit(user_id=user_id, catalogue=answer[-1]["catalogue"], status=False)
+                return {
+                    "status": 500,
+                    "msg": "提交失败！"
+                }
+        except Exception as e:
+            logger.error(e)
+            await commit(user_id=user_id, catalogue=answer[-1]["catalogue"], status=False)
+            return {
+                "status": 500,
+                "msg": "提交失败！"
+            }
+
+
+async def jiangxi(user_id: int) -> dict:
+    """
+    江西共青团
+    :param user_id:用户ID
+    :return:
+    """
+    result = await User.filter(user_id=user_id).values()
+    if not result:
+        return {
+            "status": 500,
+            "msg": "用户数据不存在！"
+        }
+    else:
+        name = result[0]["name"]
+        nid = result[0]["dxx_id"]
+        openid = result[0]["openid"]
+        if result[0]["mobile"]:
+            suborg = result[0]["mobile"]
+        else:
+            suborg = ''
+        answer = await Answer.all().order_by("time").values()
+        try:
+            url = f"http://www.jxqingtuan.cn/pub/vol/volClass/index?userId={random.randint(4363000, 4364000)}"
+            headers.update({
+                'Cookie': 'JSESSIONID=' + secrets.token_urlsafe(40),
+                'Host': 'www.jxqingtuan.cn',
+                'Origin': 'http://www.jxqingtuan.cn',
+                'Referer': 'http://www.jxqingtuan.cn/html/h5_index.html?&accessToken=' + openid,
+            })
+            async with AsyncClient(headers=headers) as client:
+                course = await client.get(url=url)
+                course.encoding = course.charset_encoding
+                if json.loads(course.text).get('code') == 0:
+                    title = json.loads(course.text).get("list")[0].get("title")
+                    course = json.loads(course.text).get('list')[0].get('id')
+                    resp_url = 'http://www.jxqingtuan.cn/pub/vol/volClass/join?accessToken='
+                    data = {"course": course, "nid": nid, "cardNo": name, "subOrg": suborg}
+                    res = await client.post(url=resp_url, json=data)
+                    res.encoding = res.charset_encoding
+                    resp = json.loads(res.text)
+                    if resp.get("status") == 200:
+                        await User.filter(user_id=user_id).update(
+                            commit_time=time.time(),
+                            catalogue=title
+                        )
+                        await commit(user_id=user_id, catalogue=title, status=True)
+                        return {
+                            "status": 0,
+                            "catalogue": title,
+                            "msg": "提交成功！"
+                        }
+                    else:
+                        await commit(user_id=user_id, catalogue=title, status=False)
+                        return {
+                            "status": 500,
+                            "msg": "提交失败,信息错误！"
+                        }
+                else:
+                    await commit(user_id=user_id, catalogue=answer[-1]["catalogue"], status=False)
+                    return {
+                        "status": 500,
+                        "msg": "提交失败,江西共青团访问错误！"
+                    }
+        except Exception as e:
+            logger.error(e)
+            await commit(user_id=user_id, catalogue=answer[-1]["catalogue"], status=False)
+            return {
+                "status": 500,
+                "msg": f"提交失败,{e}"
+            }
+
+
+async def zhejiang(user_id: int) -> dict:
+    """
+    青春浙江
+    :param user_id:
+    :return:
+    """
+    result = await User.filter(user_id=user_id).values()
+    if not result:
+        return {
+            "status": 500,
+            "msg": "用户数据不存在！"
+        }
+    else:
+        nickname = result[0]["token"]
+        name = result[0]["name"]
+        nid = result[0]["dxx_id"]
+        openid = result[0]["openid"]
+        cookie = result[0]["cookie"]
+        if result[0]["mobile"]:
+            suborg = result[0]["mobile"]
+        else:
+            suborg = None
+        answer = await Answer.all().order_by("time").values()
+        try:
+            headers = {
+                "Host": "qczj.h5yunban.com",
+                "Connection": "keep-alive",
+                "Accept": "application/json, text/javascript, */*; q=0.01",
+                "X-Requested-With": "XMLHttpRequest",
+                "User-Agent": "Mozilla/5.0 (Linux; Android 12; M2007J3SC Build/SKQ1.220303.001; wv) AppleWebKit/537.36 (KHTML, like Gecko) Version/4.0 Chrome/86.0.4240.99 XWEB/3262 MMWEBSDK/20220204 Mobile Safari/537.36 MMWEBID/6170 MicroMessenger/8.0.20.2100(0x28001438) Process/toolsmp WeChat/arm32 Weixin NetType/WIFI Language/zh_CN ABI/arm64",
+                "Content-Type": "application/json;charset=UTF-8",
+                "Sec-Fetch-Site": "same-origin",
+                "Sec-Fetch-Mode": "cors",
+                "Sec-Fetch-Dest": "empty",
+                "Accept-Encoding": "gzip, deflate",
+                "Accept-Language": "zh-CN,zh;q=0.9,en-US;q=0.8,en;q=0.7",
+            }
+            url = f"https://qczj.h5yunban.com/qczj-youth-learning/cgi-bin/login/we-chat/callback?callback=https%3A%2F%2Fqczj.h5yunban.com%2Fqczj-youth-learning%2Findex.php&scope=snsapi_userinfo&appid=wx56b888a1409a2920&openid={openid}&nickname={nickname}&headimg={cookie}&time={int(time.time())}&source=common&sign=&t={int(time.time())}"
+            async with AsyncClient(headers=headers) as client:
+                response = await client.get(url)
+                response.encoding = response.charset_encoding
+                accessToken = re.findall(r"\(\'accessToken\'\,\s+\'(.+?)\'\)", response.text)[0]
+                study_url = f"https://qczj.h5yunban.com/qczj-youth-learning/cgi-bin/common-api/course/current?accessToken={accessToken}"
+                response = await client.get(url=study_url)
+                response.encoding = response.charset_encoding
+                if response.json()['status'] == 200:
+                    title = response.json()["result"]['title']
+                    course = response.json()['result']['id']
+                    commit_url = f"https://qczj.h5yunban.com/qczj-youth-learning/cgi-bin/user-api/course/join?accessToken={accessToken}"
+                    params = {
+                        "course": course,
+                        "subOrg": suborg,
+                        "nid": nid,
+                        "cardNo": name
+                    }
+                    response = await client.post(url=commit_url, json=params)
+                    response.encoding = response.charset_encoding
+                    if response.json()['status'] == 200:
+                        await User.filter(user_id=user_id).update(
+                            commit_time=time.time(),
+                            catalogue=title
+                        )
+                        await commit(user_id=user_id, catalogue=title, status=True)
+                        return {
+                            "status": 0,
+                            "catalogue": title,
+                            "msg": "提交成功！"
+                        }
+                    else:
+                        await commit(user_id=user_id, catalogue=title, status=False)
+                        return {
+                            "status": 500,
+                            "msg": "提交失败，信息错误！"
+                        }
+                else:
+                    await commit(user_id=user_id, catalogue=answer[-1]["catalogue"], status=False)
+                    return {
+                        "status": 500,
+                        "msg": "提交失败，青春浙江访问失败！"
+                    }
+        except Exception as e:
+            logger.error(e)
+            await commit(user_id=user_id, catalogue=answer[-1]["catalogue"], status=False)
+            return {
+                "status": 500,
+                "msg": f"提交失败,{e}"
+            }
+
+
+async def shanghai(user_id: int) -> dict:
+    """
+    青春上海
+    :param user_id:
+    :return:
+    """
+    result = await User.filter(user_id=user_id).values()
+    if not result:
+        return {
+            "status": 500,
+            "msg": "用户数据不存在！"
+        }
+    else:
+        nickname = result[0]["token"]
+        name = result[0]["name"]
+        nid = result[0]["dxx_id"]
+        openid = result[0]["openid"]
+        cookie = result[0]["cookie"]
+        if result[0]["mobile"]:
+            suborg = result[0]["mobile"]
+        else:
+            suborg = None
+        answer = await Answer.all().order_by("time").values()
+        try:
+            headers = {
+                "Host": "qcsh.h5yunban.com",
+                "Connection": "keep-alive",
+                "Accept": "application/json, text/javascript, */*; q=0.01",
+                "X-Requested-With": "XMLHttpRequest",
+                "User-Agent": "Mozilla/5.0 (Linux; Android 12; M2007J3SC Build/SKQ1.220303.001; wv) AppleWebKit/537.36 (KHTML, like Gecko) Version/4.0 Chrome/86.0.4240.99 XWEB/3262 MMWEBSDK/20220204 Mobile Safari/537.36 MMWEBID/6170 MicroMessenger/8.0.20.2100(0x28001438) Process/toolsmp WeChat/arm32 Weixin NetType/WIFI Language/zh_CN ABI/arm64",
+                "Content-Type": "application/json;charset=UTF-8",
+                "Sec-Fetch-Site": "same-origin",
+                "Sec-Fetch-Mode": "cors",
+                "Sec-Fetch-Dest": "empty",
+                "Referer": "https://qcsh.h5yunban.com/youth-learning/signUp.php?rv=2020",
+                "Accept-Encoding": "gzip, deflate",
+                "Accept-Language": "zh-CN,zh;q=0.9,en-US;q=0.8,en;q=0.7",
+            }
+            url = f"https://qcsh.h5yunban.com/youth-learning/cgi-bin/login/we-chat/callback?appid=wxa693f4127cc93fad&openid={openid}&nickname={nickname}&headimg={cookie}&callback=https://qcsh.h5yunban.com/youth-learning/&scope=snsapi_userinfo"
+            async with AsyncClient(headers=headers) as client:
+                response = await client.get(url)
+                response.encoding = response.charset_encoding
+                accessToken = re.findall(r"\(\'accessToken\'\,\s+\'(.+?)\'\)", response.text)[0]
+                study_url = f"https://qcsh.h5yunban.com/youth-learning/cgi-bin/common-api/course/current?accessToken={accessToken}"
+                response = await client.get(url=study_url)
+                response.encoding = response.charset_encoding
+                if response.json()['status'] == 200:
+                    title = response.json()["result"]['title']
+                    course = response.json()['result']['id']
+                    commit_url = f"https://qcsh.h5yunban.com/youth-learning/cgi-bin/user-api/course/join?accessToken={accessToken}"
+                    params = {
+                        "course": course,
+                        "subOrg": suborg,
+                        "nid": nid,
+                        "cardNo": name
+                    }
+                    response = await client.post(url=commit_url, json=params)
+                    response.encoding = response.charset_encoding
+                    if response.json()['status'] == 200:
+                        await User.filter(user_id=user_id).update(
+                            commit_time=time.time(),
+                            catalogue=title
+                        )
+                        await commit(user_id=user_id, catalogue=title, status=True)
+                        return {
+                            "status": 0,
+                            "catalogue": title,
+                            "msg": "提交成功！"
+                        }
+                    else:
+                        await commit(user_id=user_id, catalogue=title, status=False)
+                        return {
+                            "status": 500,
+                            "msg": "提交失败,信息错误！"
+                        }
+                else:
+                    await commit(user_id=user_id, catalogue=answer[-1]["catalogue"], status=False)
+                    return {
+                        "status": 500,
+                        "msg": "提交失败，青春上海访问失败！"
+                    }
+        except Exception as e:
+            logger.error(e)
+            await commit(user_id=user_id, catalogue=answer[-1]["catalogue"], status=False)
+            return {
+                "status": 500,
+                "msg": "提交失败！"
+            }
+
+
+async def anhui(user_id: int) -> dict:
+    """
+    安徽共青团
+    :param user_id:用户ID
+    :return:
+    """
+    result = await User.filter(user_id=user_id).values()
+    if not result:
+        return {
+            "status": 500,
+            "msg": "用户数据不存在！"
+        }
+    else:
+        username = result[0]['name']
+        gender = result[0]['gender']
+        mobile = result[0]['mobile']
+        level1 = result[0]['university_type']
+        level2 = result[0]['university']
+        level3 = result[0]['college']
+        level4 = result[0]['organization']
+        level5 = result[0]['organization_id']
+        token = result[0]["token"]
+        answer = await Answer.all().order_by("time").values()
+        try:
+            headers = {
+                "Host": "dxx.ahyouth.org.cn",
+                "Accept": "application/json, text/plain, */*",
+                "Accept-Language": "zh-CN,zh;q=0.9,en-US;q=0.8,en;q=0.7",
+                "Referer": "http://dxx.ahyouth.org.cn/",
+                "Accept-Encoding": "gzip, deflate",
+                "Connection": "keep-alive",
+                'Content-Type': 'application/x-www-form-urlencoded',
+                "X-Requested-With": 'com.tencent.mm',
+                "Origin": 'http://dxx.ahyouth.org.cn',
+                "token": token
+            }
+            data = {
+                'username': username,
+                'gender': gender,
+                'mobile': mobile,
+                'level1': level1,
+                'level2': level2,
+                'level3': level3,
+                'level4': level4,
+                'level5': level5
+            }
+            get_infor_url = 'http://dxx.ahyouth.org.cn/api/saveUserInfo'
+            async with AsyncClient(headers=headers, timeout=30, max_redirects=5) as client:
+                infor_response = await client.post(url=get_infor_url, params=data)
+                infor_response.encoding = infor_response.charset_encoding
+                infor_response_json = infor_response.json()
+                if infor_response_json['code'] == 200:
+                    username = infor_response_json['content']['username']
+                    token = infor_response_json['content']['token']
+                    gender = infor_response_json['content']['gender']
+                    mobile = infor_response_json['content']['mobile']
+                    level1 = infor_response_json['content']['level1']
+                    level2 = infor_response_json['content']['level2']
+                    level3 = infor_response_json['content']['level3']
+                    level4 = infor_response_json['content']['level4']
+                    level5 = infor_response_json['content']['level5']
+                    data = {
+                        'username': username,
+                        'gender': gender,
+                        'mobile': mobile,
+                        'level1': level1,
+                        'level2': level2,
+                        'level3': level3,
+                        'level4': level4,
+                        'level5': level5
+                    }
+                    commit_url = 'http://dxx.ahyouth.org.cn/api/newLearn'
+                    commit_response = await client.post(url=commit_url, params=data)
+                    commit_response.encoding = commit_response.charset_encoding
+                    commit_response_json = commit_response.json()
+                    if commit_response_json['code'] == 200:
+                        await User.filter(user_id=user_id).update(
+                            token=token,
+                            commit_time=time.time(),
+                            catalogue=answer[-1]["catalogue"]
+                        )
+                        await commit(user_id=user_id, catalogue=answer[-1]["catalogue"], status=True)
+                        return {
+                            "status": 0,
+                            "catalogue": answer[-1]["catalogue"],
+                            "msg": "提交成功！"
+                        }
+                    else:
+                        await commit(user_id=user_id, catalogue=answer[-1]["catalogue"], status=False)
+                        return {
+                            "status": 500,
+                            "msg": "提交失败，token失效！"
+                        }
+                else:
+                    await commit(user_id=user_id, catalogue=answer[-1]["catalogue"], status=False)
+                    return {
+                        "status": 500,
+                        "msg": "提交失败,token获取失败！"
+                    }
+        except Exception as e:
+            logger.error(e)
+            await commit(user_id=user_id, catalogue=answer[-1]["catalogue"], status=False)
+            return {
+                "status": 500,
+                "msg": f"提交失败,{e}"
+            }
+
+
+async def sichuan(user_id: int) -> dict:
+    """
+    天府新青年
+    :param user_id:
+    :return:
+    """
+    result = await User.filter(user_id=user_id).values()
+    if not result:
+        return {
+            "status": 500,
+            "msg": "用户数据不存在！"
+        }
+    else:
+        token = result[0]["token"]
+        university_type = result[0]["university_type"]
+        university_id = result[0]["university_id"]
+        university = result[0]["university"]
+        name = result[0]["name"]
+        mobile = result[0]["mobile"]
+        college_id = result[0]["college_id"]
+        college = result[0]["college"]
+        organization_id = result[0]["organization_id"]
+        organization = result[0]["organization"]
+        dxx_id = result[0]["dxx_id"]
+        data_json = {
+            "name": name,
+            "tel": mobile,
+            "org": f"#{dxx_id}#{university_id}#{college_id}#{organization_id}#",
+            "lastOrg": organization_id,
+            "orgName": organization,
+            "allOrgName": f"#{university_type}#{university}#{college}#{organization}#"
+        }
+        headers.update({
+            "Referer": 'http://scyol.com/v_prod6.02/',
+            "Host": "dxx.scyol.com",
+            "Connection": "keep-alive",
+            "Content_Length": '9',
+            "Content_Type": "application/json",
+            "Accept": "*/*",
+            "User-Agent": "Mozilla/5.0 (Linux; Android 11; M2007J3SC Build/SKQ1.220213.001; wv) AppleWebKit/537.36 (KHTML, like Gecko) Version/4.0 Chrome/86.0.4240.99 XWEB/3224 MMWEBSDK/20210902 Mobile Safari/537.36 MMWEBID/6170 MicroMessenger/8.0.15.2020(0x28000F30) Process/toolsmp WeChat/arm32 Weixin NetType/WIFI Language/zh_CN ABI/arm64",
+            "Origin": "http://scyol.com",
+            "X-Requested-With": "com.tencent.mm",
+            "Sec-Fetch-Site": "same-origin",
+            "Sec-Fetch-Mode": "cors",
+            "Sec-Fetch-Dest": "empty",
+            "token": token,
+            "Accept-Encoding": "gzip, deflate",
+            "Accept-Language": "zh-CN,zh;q=0.9,en-US;q=0.8,en;q=0.7",
+        })
+        answer = await Answer.all().order_by("time").values()
+        title = answer[-1]["catalogue"]
+        url = 'https://dxx.scyol.com/api/student/commit'
+        try:
+            async with AsyncClient(headers=headers) as client:
+                response = await client.post(url=url, json=data_json)
+                if response.status_code == 200:
+                    response.encoding = response.charset_encoding
+                    if response.json()["code"] == 2:
+                        await User.filter(user_id=user_id).update(
+                            commit_time=time.time(),
+                            catalogue=title
+                        )
+                        await commit(user_id=user_id, catalogue=title, status=True)
+                        return {
+                            "status": 0,
+                            "catalogue": title,
+                            "msg": "你已经提交了，请勿重复提交哦"
+                        }
+                    elif response.json()["code"] == 200:
+                        await User.filter(user_id=user_id).update(
+                            commit_time=time.time(),
+                            catalogue=title
+                        )
+                        await commit(user_id=user_id, catalogue=title, status=True)
+                        return {
+                            "status": 0,
+                            "catalogue": title,
+                            "msg": "提交成功！"
+                        }
+                    else:
+                        await commit(user_id=user_id, catalogue=answer[-1]["catalogue"], status=False)
+                        return {
+                            "status": 500,
+                            "msg": "提交失败！"
+                        }
+                else:
+                    return {
+                        "status": 500,
+                        "msg": "提交失败,cookie失效！"
+                    }
+        except Exception as e:
+            return {
+                "status": 500,
+                "msg": f"提交失败,{e}"
+            }
+
+
+async def shandong(user_id: int) -> dict:
+    """
+    青春山东
+    :param user_id: 用户ID
+    :return:
+    """
+    result = await User.filter(user_id=user_id).values()
+    if not result:
+        return {
+            "status": 500,
+            "msg": "用户数据不存在！"
+        }
+    else:
+        openid = result[0]["openid"]
+        cookie = result[0]["cookie"]
+        answer = await Answer.all().order_by("time").values()
+        title = answer[-1]["catalogue"]
+        headers.update({
+            "Host": "qndxx.youth54.cn",
+            "Connection": "keep-alive",
+            "Accept": "*/*",
+            "User-Agent": "Mozilla/5.0 (Linux; Android 12; M2007J3SC Build/SKQ1.220213.001; wv) AppleWebKit/537.36 (KHTML, like Gecko) Version/4.0 Chrome/86.0.4240.99 XWEB/3234 MMWEBSDK/20210902 Mobile Safari/537.36 MMWEBID/6170 MicroMessenger/8.0.15.2020(0x28000F30) Process/toolsmp WeChat/arm32 Weixin NetType/WIFI Language/zh_CN ABI/arm64",
+            "X-Requested-With": "XMLHttpRequest",
+            "Content-Type": "application/x-www-form-urlencoded; charset=UTF-8",
+            "Origin": "http://qndxx.youth54.cn",
+            "Referer": "http://qndxx.youth54.cn/SmartLA/dxx.w?method=pageSdtwdt",
+            "Accept-Encoding": "gzip, deflate",
+            "Accept-Language": "zh-CN,zh;q=0.9,en-US;q=0.8,en;q=0.7",
+            "Cookie": cookie
+        })
+        try:
+            version_url = f'http://qndxx.youth54.cn/SmartLA/dxxjfgl.w?method=getNewestVersionInfo&openid={openid}'
+            async with AsyncClient(headers=headers) as client:
+                version_response = await client.post(url=version_url)
+                if version_response.status_code == 200:
+                    version_response.encoding = version_response.charset_encoding
+                    content = version_response.json()
+                    if content["errcode"] == "0":
+                        versionname = content['versionname']
+                        version = content['version']
+                        headers.update({
+                            "Host": "qndxx.youth54.cn",
+                            "Connection": "keep-alive",
+                            "Accept": "*/*",
+                            "User-Agent": "Mozilla/5.0 (Linux; Android 12; M2007J3SC Build/SKQ1.220213.001; wv) AppleWebKit/537.36 (KHTML, like Gecko) Version/4.0 Chrome/86.0.4240.99 XWEB/3234 MMWEBSDK/20210902 Mobile Safari/537.36 MMWEBID/6170 MicroMessenger/8.0.15.2020(0x28000F30) Process/toolsmp WeChat/arm32 Weixin NetType/WIFI Language/zh_CN ABI/arm64",
+                            "X-Requested-With": "XMLHttpRequest",
+                            "Content-Type": "application/x-www-form-urlencoded; charset=UTF-8",
+                            "Origin": "http://qndxx.youth54.cn",
+                            "Referer": "http://qndxx.youth54.cn/SmartLA/dxx.w?method=pageSdtwdt",
+                            "Accept-Encoding": "gzip, deflate",
+                            "Accept-Language": "zh-CN,zh;q=0.9,en-US;q=0.8,en;q=0.7",
+                            "Cookie": cookie
+                        })
+                        data = {
+                            'openid': openid,
+                            'version': version
+                        }
+                        commit_url = 'http://qndxx.youth54.cn/SmartLA/dxxjfgl.w?method=studyLatest'
+                        response = await client.post(url=commit_url, params=data, headers=headers)
+                        if response.status_code == 200:
+                            response.encoding = response.charset_encoding
+                            if response.json()["errcode"] == "0":
+                                await User.filter(user_id=user_id).update(
+                                    commit_time=time.time(),
+                                    catalogue=versionname
+                                )
+                                await commit(user_id=user_id, catalogue=versionname, status=True)
+                                return {
+                                    "status": 0,
+                                    "catalogue": versionname,
+                                    "msg": "提交成功！"
+                                }
+                            else:
+                                await commit(user_id=user_id, catalogue=versionname, status=False)
+                                return {
+                                    "status": 500,
+                                    "msg": "提交失败,cookie失效！"
+                                }
+                        else:
+                            await commit(user_id=user_id, catalogue=versionname, status=False)
+                            return {
+                                "status": 500,
+                                "msg": "提交失败，cookie失效！"
+                            }
+                    else:
+                        await commit(user_id=user_id, catalogue=title, status=False)
+                        return {
+                            "status": 500,
+                            "msg": "提交失败，cookie失效！"
+                        }
+                else:
+                    await commit(user_id=user_id, catalogue=title, status=False)
+                    return {
+                        "status": 500,
+                        "msg": "提交失败，青春山东访问失败！"
+                    }
+        except Exception as e:
+            await commit(user_id=user_id, catalogue=title, status=False)
+            return {
+                "status": 500,
+                "msg": f"提交失败,{e}"
+            }
+
+
+async def chongqing(user_id: int) -> dict:
+    """
+    重庆共青团
+    :param user_id:
+    :return:
+    """
+    result = await User.filter(user_id=user_id).values()
+    if not result:
+        return {
+            "status": 500,
+            "msg": "用户数据不存在！"
+        }
+    else:
+        openid = result[0]["openid"]
+        answer = await Answer.all().order_by("time").values()
+        title = answer[-1]["catalogue"]
+        headers.update(
+            {
+                "Host": "qndxx.cqyouths.com",
+                "Connection": "keep-alive",
+                "Accept": "application/json, text/plain, */*",
+                "User-Agent": "Mozilla/5.0 (Linux; Android 12; M2007J3SC Build/SKQ1.220303.001; wv) AppleWebKit/537.36 (KHTML, like Gecko) Version/4.0 Chrome/86.0.4240.99 XWEB/3262 MMWEBSDK/20220204 Mobile Safari/537.36 MMWEBID/6170 MicroMessenger/8.0.20.2100(0x28001438) Process/toolsmp WeChat/arm32 Weixin NetType/WIFI Language/zh_CN ABI/arm64",
+                "X-Requested-With": "com.tencent.mm",
+                "Accept-Encoding": "gzip, deflate",
+                "Accept-Language": "zh-CN,zh;q=0.9,en-US;q=0.8,en;q=0.7"
+            }
+        )
+        try:
+            new_url = f"http://qndxx.cqyouths.com/new_course.json?time={int(time.time())}"
+            async with AsyncClient(headers=headers) as client:
+                new_response = await client.get(url=new_url)
+                if new_response.status_code == 200:
+                    new_response.encoding = new_response.charset_encoding
+                    course_id = new_response.json()['data'][0]['id']
+                    commit_url = f"http://qndxx.cqyouths.com/api/course/studyCourse?openid={openid}&id={course_id}"
+                    response = await client.get(url=commit_url)
+                    if response.status_code == 200:
+                        response.encoding = response.charset_encoding
+                        if response.json()["status"] == 200:
+                            await User.filter(user_id=user_id).update(
+                                commit_time=time.time(),
+                                catalogue=title
+                            )
+                            await commit(user_id=user_id, catalogue=title, status=True)
+                            return {
+                                "status": 0,
+                                "catalogue": title,
+                                "msg": "提交成功！"
+                            }
+                        elif response.json()["status"] == 201:
+                            await User.filter(user_id=user_id).update(
+                                commit_time=time.time(),
+                                catalogue=title
+                            )
+                            await commit(user_id=user_id, catalogue=title, status=True)
+                            return {
+                                "status": 0,
+                                "catalogue": title,
+                                "msg": "提交成功！"
+                            }
+                        else:
+                            await commit(user_id=user_id, catalogue=title, status=False)
+                            return {
+                                "status": 500,
+                                "msg": "提交失败，openid错误！"
+                            }
+                    else:
+                        await commit(user_id=user_id, catalogue=title, status=False)
+                        return {
+                            "status": 500,
+                            "msg": "提交失败，openid错误！"
+                        }
+                else:
+                    await commit(user_id=user_id, catalogue=title, status=False)
+                    return {
+                        "status": 500,
+                        "msg": "提交失败，重庆共青团访问失败！"
+                    }
+        except Exception as e:
+            logger.error(e)
+            return {
+                "status": 500,
+                "msg": f"提交失败,{e}"
+            }
+
+
+async def jilin(user_id: int) -> dict:
+    """
+    吉青飞扬
+    :param user_id:
+    :return:
+    """
+    result = await User.filter(user_id=user_id).values()
+    if not result:
+        return {
+            "status": 500,
+            "msg": "用户数据不存在！"
+        }
+    else:
+        openid = result[0]["openid"]
+        dxx_id = result[0]["dxx_id"]
+        answer = await Answer.all().order_by("time").values()
+        title = answer[-1]["catalogue"]
+        headers.update(
+            {
+                "Host": "jqfy.jl54.org",
+                "Connection": "keep-alive",
+                "Upgrade-Insecure-Requests": "1",
+                "User-Agent": "Mozilla/5.0 (Linux; Android 12; M2007J3SC Build/SKQ1.220303.001; wv) AppleWebKit/537.36 (KHTML, like Gecko) Version/4.0 Chrome/86.0.4240.99 XWEB/3262 MMWEBSDK/20220204 Mobile Safari/537.36 MMWEBID/6170 MicroMessenger/8.0.20.2100(0x28001438) Process/toolsmp WeChat/arm32 Weixin NetType/WIFI Language/zh_CN ABI/arm64",
+                "Accept": "text/html,application/xhtml+xml,application/xml;q=0.9,image/avif,image/wxpic,image/tpg,image/webp,image/apng,*/*;q=0.8,application/signed-exchange;v=b3;q=0.9",
+                "X-Requested-With": "com.tencent.mm",
+                "Accept-Encoding": "gzip, deflate",
+                "Accept-Language": "zh-CN,zh;q=0.9,en-US;q=0.8,en;q=0.7"
+            }
+        )
+        try:
+            commit_url = f"http://jqfy.jl54.org/jltw/wechat/editStudyRecord/{dxx_id}"
+            data = {
+                "openid": openid
+            }
+            async with AsyncClient(headers=headers) as client:
+                response = await client.post(url=commit_url, params=data)
+            if response.status_code == 200:
+                response.encoding = response.charset_encoding
+                if response.json()["code"] == '0001':
+                    await User.filter(user_id=user_id).update(
+                        commit_time=time.time(),
+                        catalogue=title
+                    )
+                    await commit(user_id=user_id, catalogue=title, status=True)
+                    return {
+                        "status": 0,
+                        "catalogue": title,
+                        "msg": "提交成功！"
+                    }
+                else:
+                    await commit(user_id=user_id, catalogue=title, status=False)
+                    return {
+                        "status": 500,
+                        "msg": f"提交失败，openid错误！"
+                    }
+            else:
+                await commit(user_id=user_id, catalogue=title, status=False)
+                return {
+                    "status": 500,
+                    "msg": "提交失败，吉青飞扬访问失败！"
+                }
+        except Exception as e:
+            logger.error(e)
+            return {
+                "status": 500,
+                "msg": f"提交失败,{e}"
+            }
+
+
+async def guangdong(user_id: int) -> dict:
+    """
+    广东共青团
+    :param user_id:用户ID
+    :return:
+    """
+    result = await User.filter(user_id=user_id).values()
+    if not result:
+        return {
+            "status": 500,
+            "msg": "用户数据不存在！"
+        }
+    else:
+        dxx_id = result[0]['dxx_id']
+        token = result[0]["token"]
+        answer = await Answer.all().order_by("time").values()
+        try:
+            study_headers = {
+                'Host': 'youthstudy.12355.net',
+                'Connection': 'keep-alive',
+                'X-Litemall-Token': token,
+                'X-Litemall-IdentiFication': 'young',
+                'User-Agent': 'MicroMessenger',
+                'Accept': '*/*',
+                'Origin': 'https://youthstudy.12355.net',
+                'X-Requested-With': 'com.tencent.mm',
+                'Sec-Fetch-Site': 'same-origin',
+                'Sec-Fetch-Mode': 'cors',
+                'Sec-Fetch-Dest': 'empty',
+                'Referer': 'https://youthstudy.12355.net/h5/',
+                'Accept-Language': 'zh-CN,zh;q=0.9,en-US;q=0.8,en;q=0.7',
+            }
+            new_study_url = "https://youthstudy.12355.net/saomah5/api/young/chapter/new"
+            async with AsyncClient(headers=study_headers, timeout=30, max_redirects=5) as client:
+                study_response = await client.get(url=new_study_url)
+            study_response.encoding = study_response.charset_encoding
+            if study_response.json()["errno"] == 0:
+                chapterId = study_response.json().get('data').get('entity').get('id')
+                title = study_response.json().get('data').get('entity').get('name').replace('“青年大学习”', "").strip()
+                commit_url = "https://youthstudy.12355.net/saomah5/api/young/course/chapter/saveHistory"
+                async with AsyncClient(headers=study_headers, timeout=30, max_redirects=5) as client:
+                    commit_response = await client.post(url=commit_url, data={
+                        "chapterId": chapterId
+                    })
+                if commit_response.json()["errno"] == 0:
+                    await User.filter(user_id=user_id).update(
+                        token=token,
+                        commit_time=time.time(),
+                        catalogue=title
+                    )
+                    await commit(user_id=user_id, catalogue=title, status=True)
+                    return {
+                        "status": 0,
+                        "catalogue": title,
+                        "msg": "提交成功！"
+                    }
+                else:
+                    await commit(user_id=user_id, catalogue=answer[-1]["catalogue"], status=False)
+                    return {
+                        "status": 500,
+                        "msg": "提交失败！"
+                    }
+            else:
+                token_headers = {
+                    'Host': 'tuanapi.12355.net',
+                    'Connection': 'keep-alive',
+                    'Accept': 'application/json, text/javascript, */*; q=0.01',
+                    'Origin': 'https://tuan.12355.net',
+                    'User-Agent': 'MicroMessenger',
+                    'X-Requested-With': 'com.tencent.mm',
+                    'Sec-Fetch-Site': 'same-site',
+                    'Sec-Fetch-Mode': 'cors',
+                    'Referer': 'https://tuan.12355.net/wechat/view/YouthLearning/page.html',
+                    'Accept-Encoding': 'gzip, deflate',
+                    'Accept-Language': 'zh-CN,zh;q=0.9,en-US;q=0.8,en;q=0.7',
+                }
+                ger_param_url = f"https://tuanapi.12355.net/questionnaire/getYouthLearningUrl?mid={dxx_id}"
+                async with AsyncClient(headers=token_headers, timeout=30, max_redirects=5) as client:
+                    param_response = await client.get(url=ger_param_url)
+                    if param_response.json()["status"] == 200:
+                        content = param_response.json()["youthLearningUrl"].split("=")[-1]
+                        token_url = "https://youthstudy.12355.net/apih5/api/user/get"
+                        token_headers = {
+                            'Host': 'youthstudy.12355.net',
+                            'Connection': 'keep-alive',
+                            'Content-Length': '134',
+                            'Origin': 'https://youthstudy.12355.net',
+                            'X-Litemall-Token': '',
+                            'X-Litemall-IdentiFication': 'young',
+                            'User-Agent': 'MicroMessenger',
+                            'Content-Type': 'application/x-www-form-urlencoded',
+                            'Accept': '*/*',
+                            'X-Requested-With': 'com.tencent.mm',
+                            'Sec-Fetch-Site': 'same-origin',
+                            'Sec-Fetch-Mode': 'cors',
+                            'Referer': 'https://youthstudy.12355.net/h5/',
+                            'Accept-Encoding': 'gzip, deflate',
+                            'Accept-Language': 'zh-CN,zh;q=0.9,en-US;q=0.8,en;q=0.7'
+                        }
+                        async with AsyncClient(headers=token_headers, timeout=30, max_redirects=5) as client:
+                            token_response = await client.post(url=token_url,
+                                                               data="sign=" + urllib.parse.quote(content))
+                        if token_response.json()["errno"] == 0:
+                            token = token_response.json()['data']['entity']['token']
+                            study_headers = {
+                                'Host': 'youthstudy.12355.net',
+                                'Connection': 'keep-alive',
+                                'X-Litemall-Token': token,
+                                'X-Litemall-IdentiFication': 'young',
+                                'User-Agent': 'MicroMessenger',
+                                'Accept': '*/*',
+                                'Origin': 'https://youthstudy.12355.net',
+                                'X-Requested-With': 'com.tencent.mm',
+                                'Sec-Fetch-Site': 'same-origin',
+                                'Sec-Fetch-Mode': 'cors',
+                                'Sec-Fetch-Dest': 'empty',
+                                'Referer': 'https://youthstudy.12355.net/h5/',
+                                'Accept-Language': 'zh-CN,zh;q=0.9,en-US;q=0.8,en;q=0.7',
+                            }
+                            new_study_url = "https://youthstudy.12355.net/saomah5/api/young/chapter/new"
+                            async with AsyncClient(headers=study_headers, timeout=30, max_redirects=5) as client:
+                                study_response = await client.get(url=new_study_url)
+                            if study_response.json()["errno"] == 0:
+                                chapterId = study_response.json().get('data').get('entity').get('id')
+                                title = study_response.json().get('data').get('entity').get('name').replace(
+                                    '"青年大学习”', "").strip()
+                                commit_url = "https://youthstudy.12355.net/saomah5/api/young/course/chapter/saveHistory"
+                                async with AsyncClient(headers=study_headers, timeout=30, max_redirects=5) as client:
+                                    commit_response = await client.post(url=commit_url, data={
+                                        "chapterId": chapterId
+                                    })
+                                if commit_response.json()["errno"] == 0:
+                                    await User.filter(user_id=user_id).update(
+                                        token=token,
+                                        commit_time=time.time(),
+                                        catalogue=title
+                                    )
+                                    await commit(user_id=user_id, catalogue=title, status=True)
+                                    return {
+                                        "status": 0,
+                                        "catalogue": title,
+                                        "msg": "提交成功！"
+                                    }
+                                else:
+                                    await commit(user_id=user_id, catalogue=answer[-1]["catalogue"], status=False)
+                                    return {
+                                        "status": 500,
+                                        "msg": "提交失败！"
+                                    }
+                        else:
+                            await commit(user_id=user_id, catalogue=answer[-1]["catalogue"], status=False)
+                            return {
+                                "status": 500,
+                                "msg": "提交失败，token获取失效！"
+                            }
+                    else:
+                        await commit(user_id=user_id, catalogue=answer[-1]["catalogue"], status=False)
+                        return {
+                            "status": 500,
+                            "msg": "提交失败，token获取失效！"
+                        }
+        except Exception as e:
+            logger.error(e)
+            await commit(user_id=user_id, catalogue=answer[-1]["catalogue"], status=False)
+            return {
+                "status": 500,
+                "msg": "提交失败！"
+            }
+
+
+async def beijing(user_id: int) -> dict:
+    """
+    青春北京
+    :param user_id:用户ID
+    :return:
+    """
+    result = await User.filter(user_id=user_id).values()
+    if not result:
+        return {
+            "status": 500,
+            "msg": "用户数据不存在！"
+        }
+    else:
+        cookie = result[0]['cookie']
+        token = result[0]["token"]
+        answer = await Answer.all().order_by("time").values()
+        headers = {
+            "User-Agent": "Mozilla/5.0 (iPhone; CPU iPhone OS 13_2_3 like Mac OS X) AppleWebKit/605.1.15 (KHTML, like Gecko) Version/13.0.3 Mobile/15E148 Safari/604.1 Edg/113.0.0.0", }
+        login_url = "https://m.bjyouth.net/site/login"
+        try:
+            async with AsyncClient(headers=headers) as client:
+                login_rsp = await client.get(login_url)
+                if login_rsp.status_code == 200:
+                    login_rsp.encoding = login_rsp.charset_encoding
+                    soup = BeautifulSoup(login_rsp.text, "lxml")
+                    code_url = "https://m.bjyouth.net" + soup.select("#verifyCode-image")[0].get("src")
+                    code_rsp = await client.get(code_url)
+                    code_text = DdddOcr(show_ad=False).classification(code_rsp.content)
+                    login_response = await client.post(
+                        url=login_url,
+                        data={
+                            '_csrf_mobile': client.cookies['_csrf_mobile'],
+                            'Login[password]': await encrypt(token),
+                            'Login[username]': await encrypt(cookie),
+                            'Login[verifyCode]': code_text
+                        }
+                    )
+                    if login_response.status_code == 200:
+                        login_response.encoding = login_response.charset_encoding
+                        if login_response.text == '8':
+                            await commit(user_id=user_id, catalogue=answer[-1]["catalogue"], status=False)
+                            return {
+                                "status": 500,
+                                "msg": "提交失败，验证码识别失败！"
+                            }
+                        if 'fail' in login_response.text:
+                            await commit(user_id=user_id, catalogue=answer[-1]["catalogue"], status=False)
+                            return {
+                                "status": 500,
+                                "msg": "提交失败，账号或密码错误！"
+                            }
+                        course_url = "https://m.bjyouth.net/dxx/index"
+                        course_rsp = await client.get(course_url)
+                        if course_rsp.json()["code"] == 200:
+                            title = course_rsp.json()['newCourse']['title']
+                            courseId = course_rsp.json()['newCourse']['id']
+                            organization_rsp = await client.get('https://m.bjyouth.net/dxx/is-league')
+                            organization_id = int(organization_rsp.text)
+                            study_url = "https://m.bjyouth.net/dxx/check"
+                            study_response = await client.post(url=study_url, json={
+                                "id": str(courseId),
+                                "org_id": organization_id
+                            })
+                            if study_response.status_code == 200:
+                                learnedInfo_url = 'https://m.bjyouth.net/dxx/my-study?page=1&limit=15&year=' + time.strftime(
+                                    "%Y",
+                                    time.localtime())
+                                haveLearned = await client.get(learnedInfo_url)
+                                if haveLearned.json()["code"] == 200:
+                                    if f"学习课程：《{title}》" in list(
+                                            map(lambda x: x['text'], haveLearned.json()['data'])):
+                                        await User.filter(user_id=user_id).update(
+                                            token=token,
+                                            commit_time=time.time(),
+                                            catalogue=answer[-1]["catalogue"]
+                                        )
+                                        await commit(user_id=user_id, catalogue=answer[-1]["catalogue"], status=True)
+                                        return {
+                                            "status": 0,
+                                            "catalogue": answer[-1]["catalogue"],
+                                            "msg": "提交成功！"
+                                        }
+                                    else:
+                                        await commit(user_id=user_id, catalogue=answer[-1]["catalogue"], status=False)
+                                        return {
+                                            "status": 500,
+                                            "msg": "提交失败！"
+                                        }
+                                else:
+                                    await commit(user_id=user_id, catalogue=answer[-1]["catalogue"], status=False)
+                                    return {
+                                        "status": 500,
+                                        "msg": "提交失败,获取历史提交信息失败！"
+                                    }
+                            else:
+                                await commit(user_id=user_id, catalogue=answer[-1]["catalogue"], status=False)
+                                return {
+                                    "status": 500,
+                                    "msg": "提交失败！"
+                                }
+                    else:
+                        await commit(user_id=user_id, catalogue=answer[-1]["catalogue"], status=False)
+                        return {
+                            "status": 500,
+                            "msg": "提交失败，登录失败！"
+                        }
+                else:
+                    await commit(user_id=user_id, catalogue=answer[-1]["catalogue"], status=False)
+                    return {
+                        "status": 500,
+                        "msg": "提交失败，北京共青团官网异常"
+                    }
+        except Exception as e:
+            logger.error(e)
+            await commit(user_id=user_id, catalogue=answer[-1]["catalogue"], status=False)
+            return {
+                "status": 500,
+                "msg": f"提交失败,{e}"
+            }
+
+
+async def tianjin(user_id: int) -> dict:
+    """
+    津彩青春
+    :param user_id:用户ID
+    :return:
+    """
+    result = await User.filter(user_id=user_id).values()
+    if not result:
+        return {
+            "status": 500,
+            "msg": "用户数据不存在！"
+        }
+    else:
+        cookie = result[0]["cookie"]
+        answer = await Answer.all().order_by("time").values()
+        title = answer[-1]["catalogue"]
+        headers = {
+            "User-Agent": "Mozilla/5.0 (iPhone; CPU iPhone OS 13_2_3 like Mac OS X) AppleWebKit/605.1.15 (KHTML, like Gecko) Version/13.0.3 Mobile/15E148 Safari/604.1 Edg/113.0.0.0",
+            "Cookie": cookie,
+        }
+        try:
+            commit_url = "http://admin.ddy.tjyun.com/zm/jump/1"
+            async with AsyncClient(headers=headers) as client:
+                response = await client.get(url=commit_url)
+            if response.status_code == 302:
+                response.encoding = response.charset_encoding
+                if "weui_text_area" not in response.text:
+                    await User.filter(user_id=user_id).update(
+                        commit_time=time.time(),
+                        catalogue=title
+                    )
+                    await commit(user_id=user_id, catalogue=title, status=True)
+                    return {
+                        "status": 0,
+                        "catalogue": title,
+                        "msg": "提交成功！"
+                    }
+                else:
+                    await commit(user_id=user_id, catalogue=title, status=False)
+                    return {
+                        "status": 500,
+                        "msg": f"提交失败，Cookie失效！"
+                    }
+            else:
+                await commit(user_id=user_id, catalogue=title, status=False)
+                return {
+                    "status": 500,
+                    "msg": "提交失败，地址请求失败！"
+                }
+        except Exception as e:
+            logger.error(e)
+            return {
+                "status": 500,
+                "msg": f"提交失败,{e}"
+            }
```

### Comparing `TeenStudy-0.1.9/TeenStudy/utils/handle.py` & `teenstudy-0.2.0rc1/TeenStudy/utils/handle.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,372 +1,372 @@
-import asyncio
-import datetime
-import random
-import socket
-import time
-
-from nonebot import get_driver, on_notice, require, get_bot
-from nonebot import on_command, logger
-from nonebot.adapters.onebot.v11 import GroupMessageEvent, MessageSegment, Bot, GROUP, Message, MessageEvent, \
-    PokeNotifyEvent
-from nonebot.params import ArgStr, T_State, CommandArg
-from nonebot.permission import SUPERUSER
-from nonebot.rule import Rule
-
-from .path import getConfig, saveConfig
-from .rule import must_command, check_poke, check_time, must_group, must_leader
-from .utils import get_end_pic, distribute_area, distribute_area_url, get_answer_pic, get_qrcode, get_login_qrcode, \
-    to_hash
-from ..models.accuont import User, AddUser
-from ..models.dxx import Area, Answer, PushList
-
-scheduler = require('nonebot_plugin_apscheduler').scheduler
-SUPERS = get_driver().config.superusers
-CONFIG = getConfig()
-
-end_pic = on_command("end_pic", aliases={"完成截图", "大学习截图"}, permission=SUPERUSER | GROUP,
-                     rule=Rule(must_command, must_group),
-                     priority=50)
-
-submit = on_command("submit", aliases={"提交大学习"}, permission=SUPERUSER | GROUP, rule=Rule(must_command, must_group),
-                    priority=50)
-add = on_command("add_dxx", aliases={"添加大学习"}, permission=GROUP, rule=must_group, priority=50)
-my_info = on_command("my_info", aliases={"我的大学习"}, permission=SUPERUSER | GROUP,
-                     rule=Rule(must_command, must_group), priority=50)
-poke_notify = on_notice(priority=60, rule=check_poke)
-answer_pic = on_command("answer_pic", aliases={"答案截图", "大学习"}, rule=Rule(must_command, must_group),
-                        permission=SUPERUSER | GROUP,
-                        priority=50)
-finish_dxx = on_command("finish_dxx", aliases={"完成大学习", "全员大学习"},
-                        rule=Rule(must_command, must_group, must_leader), permission=GROUP | SUPERUSER, priority=50)
-reset_config = on_command("reset_config", aliases={"重置配置", "刷新配置"}, permission=SUPERUSER, rule=must_command,
-                          priority=50)
-reset_password = on_command("reset_password", aliases={"重置密码"}, permission=GROUP,
-                            rule=Rule(must_command, must_group), priority=50)
-delete_dxx = on_command("delete_dxx", aliases={"删除大学习"}, priority=50, rule=Rule(must_command, must_group))
-
-
-@end_pic.handle()
-async def test_() -> None:
-    await end_pic.finish(
-        message=MessageSegment.text("青年大学习最新一期完成截图") + MessageSegment.image(await get_end_pic()),
-        at_sender=True, reply_message=True)
-
-
-@submit.handle()
-async def submit_(event: GroupMessageEvent) -> None:
-    user_id = event.user_id
-    result = await User.filter(user_id=user_id).values()
-    if result:
-        if not await check_time():
-            await submit.finish(
-                message=MessageSegment.text("当前时间段禁止提交青年大学习，请在周一11:00之后再提交哦(｡･ω･｡)"),
-                at_sender=True, reply_message=True)
-        area = result[0]['area']
-        data = await distribute_area(user_id=user_id, area=area)
-        if data['status'] == 0:
-            message = f'青年大学习{data["catalogue"]}提交成功( ･´ω`･ )'
-            config = getConfig()
-            content = await get_login_qrcode()
-            if config["URL_STATUS"]:
-                await submit.send(message=MessageSegment.text(message) + MessageSegment.text(
-                    f"\n请点击链接登录查看,如QQ点击无法打开，请复制链接到浏览器打开\n{content['url']}"),
-                                  at_sender=True, reply_message=True)
-            else:
-                await submit.send(message=MessageSegment.text(message) + MessageSegment.image(content['content']),
-                                  at_sender=True, reply_message=True)
-            await asyncio.sleep(1)
-            await submit.finish(
-                message=MessageSegment.text("青年大学习最新一期完成截图") + MessageSegment.image(await get_end_pic()),
-                at_sender=True, reply_message=True)
-        await submit.finish(message=MessageSegment.text(data['msg']), at_sender=True, reply_message=True)
-    else:
-        await submit.finish(message=MessageSegment.text("用户数据不存在！请使用 添加大学习 指令添加(｡･ω･｡)"),
-                            at_sender=True, reply_message=True)
-
-
-@add.handle()
-async def add_(state: T_State, event: GroupMessageEvent, msg: Message = CommandArg()) -> None:
-    user_id = event.user_id
-    if await User.filter(user_id=user_id).count():
-        await add.finish(message=MessageSegment.text("你已经添加过了，不要重复添加哦( • ̀ω•́ )✧"), at_sender=True,
-                         reply_message=True)
-    if str(msg):
-        state['province'] = str(msg)
-
-
-@add.got(key="province", prompt="请输入需要添加的省份或回复 取消 停止操作！")
-async def add_(event: GroupMessageEvent, province: str = ArgStr("province")) -> None:
-    group_id = event.group_id
-    user_id = event.user_id
-    config = getConfig()
-    if province in ["取消", "No", "停止", "NO"]:
-        await add.finish(message=MessageSegment.text("操作取消！φ(>ω<*) "), at_sender=True, reply_message=True)
-    if await Area.filter(area=province).count():
-        url = await distribute_area_url(province=province, user_id=user_id, group_id=group_id)
-        if province in ["上海", "浙江"]:
-            content = await get_qrcode(user_id=user_id, group_id=group_id, area=province)
-            if config["URL_STATUS"]:
-                result = await add.send(
-                    message=MessageSegment.text(f"请复制链接到微信点击打开进行绑定( ･´ω`･ )\n{content['url']}"),
-                    at_sender=True,
-                    reply_message=True)
-            else:
-                result = await add.send(
-                    message=MessageSegment.text("请使用微信扫码进行绑定( ･´ω`･ )") + MessageSegment.image(
-                        content["content"]), at_sender=True,
-                    reply_message=True)
-        else:
-            if config["URL_STATUS"]:
-                result = await add.send(
-                    message=MessageSegment.text(
-                        f"请点击链接进入网页添加绑定，如QQ无法打开链接，请复制链接到浏览器( ･´ω`･ )\n{url['url']}"),
-                    at_sender=True,
-                    reply_message=True)
-            else:
-                result = await add.send(
-                    message=MessageSegment.text(f"请扫码进入网页添加绑定( ･´ω`･ )") + MessageSegment.image(
-                        url['content']),
-                    at_sender=True,
-                    reply_message=True)
-        await AddUser.create(
-            time=time.time(),
-            user_id=user_id,
-            group_id=group_id,
-            area=province,
-            message_id=result["message_id"],
-            status="未通过"
-        )
-    else:
-        await add.reject(
-            prompt=MessageSegment.text(
-                "该省份暂不支持或输入省份名称（名称不要带省字）错误，请重新输入或回复 取消 停止操作( ･´ω`･ )"),
-            at_sender=True,
-            reply_message=True)
-
-
-@my_info.handle()
-async def my_info_(event: MessageEvent) -> None:
-    user_id = event.user_id
-    config = getConfig()
-    if await User.filter(user_id=user_id).count():
-        content = await get_login_qrcode()
-        if config["URL_STATUS"]:
-            await my_info.finish(
-                message=MessageSegment.text(
-                    f'请点击链接登录查看哦，如QQ打不开链接，请复制链接到浏览器(｡･ω･｡)\n{content["url"]}'),
-                at_sender=True, reply_message=True)
-        else:
-            await my_info.finish(
-                message=MessageSegment.text('请扫码登录查看哦(｡･ω･｡)') + MessageSegment.image(content['content']),
-                at_sender=True, reply_message=True)
-    else:
-        await my_info.finish(
-            message=MessageSegment.text("你还没有绑定大学习哦ヾ(ｏ･ω･)ﾉ，使用 添加大学习 指令进行绑定信息吧( • ̀ω•́ )✧"),
-            at_sender=True, reply_message=True)
-
-
-@poke_notify.handle()
-async def poke_notify_(bot: Bot, event: PokeNotifyEvent):
-    config = getConfig()
-    if not config["POKE_SUBMIT"]:
-        return
-    try:
-        group_id = event.group_id
-    except AttributeError:
-        group_id = None
-    user_id = event.user_id
-    target_id = event.target_id
-    if target_id != int(bot.self_id):
-        return
-    if group_id:
-        result = await User.filter(user_id=user_id).values()
-        if result:
-            if not await check_time():
-                await submit.finish(
-                    message=MessageSegment.text("当前时间段禁止提交青年大学习，请在周一11:00之后再提交哦(｡･ω･｡)"),
-                    at_sender=True)
-            area = result[0]['area']
-            data = await distribute_area(user_id=user_id, area=area)
-            if data['status'] == 0:
-                message = f'青年大学习{data["catalogue"]}提交成功( ･´ω`･ )'
-                content = await get_login_qrcode()
-                if config["URL_STATUS"]:
-                    await poke_notify.send(
-                        message=MessageSegment.text(message) + MessageSegment.text(
-                            f"\n请点击链接登录查看,如QQ点击无法打开，请复制链接到浏览器打开\n{content['url']}"),
-                        at_sender=True)
-                else:
-                    await poke_notify.send(
-                        message=MessageSegment.text(message + "\n个人信息请扫码登录查看") + MessageSegment.image(
-                            content["content"]), at_sender=True)
-                await asyncio.sleep(1)
-                await poke_notify.finish(
-                    message=MessageSegment.text("青年大学习最新一期完成截图") + MessageSegment.image(
-                        await get_end_pic()), at_sender=True,
-                    reply_message=True)
-            await poke_notify.finish(message=MessageSegment.text(data['msg']), at_sender=True, reply_message=True)
-        else:
-            await poke_notify.finish(
-                message=MessageSegment.text("用户数据不存在！请使用 添加大学习 指令进行绑定(*^▽^*)"), at_sender=True,
-                reply_message=True)
-    else:
-        await bot.send_private_msg(user_id=user_id,
-                                   message=MessageSegment.at(user_id) + MessageSegment.text("别戳啦(~￣△￣)~"))
-
-
-@answer_pic.handle()
-async def answer_pic_() -> None:
-    await answer_pic.finish(message=MessageSegment.image(await get_answer_pic()), at_sender=True, reply_message=True)
-
-
-@finish_dxx.handle()
-async def finish() -> None:
-    if not await check_time():
-        await submit.finish(
-            message=MessageSegment.text("当前时间段禁止提交青年大学习，请在周一11:00之后再发指令哦(｡･ω･｡)"),
-            at_sender=True, reply_message=True)
-
-
-@finish_dxx.got(key="msg", prompt="是否提交团支部全体成员最新一期青年大学习？（是|否）")
-async def finish(event: GroupMessageEvent, msg: str = ArgStr("msg")) -> None:
-    if msg not in ["是", "yes", "Y", "y", "YES", "true"]:
-        await finish_dxx.finish(message=MessageSegment.text("操作取消(*^▽^*)"), at_sender=True, reply_message=True)
-    else:
-        await finish_dxx.send(message=MessageSegment.text("开始提交(*￣︶￣)"), at_sender=True, reply_message=True)
-
-    group_id = event.group_id
-    user_id = event.user_id
-    result = await User.filter(leader=user_id, group_id=group_id).values()
-    if result:
-        answer_result = await Answer.all().order_by('time').values()
-        catalogue = answer_result[-1]["catalogue"]
-        for item in result:
-            if item["catalogue"] == catalogue:
-                continue
-            else:
-                await distribute_area(user_id=item["user_id"], area=item["area"])
-                await asyncio.sleep(random.randint(10, 15))
-    await finish_dxx.finish(message=MessageSegment.text("提交完成！"), at_sender=True, reply_message=True)
-
-
-@reset_config.got(key="msg", prompt="是否重置大学习配置为默认配置？（是|否）")
-async def reset_config_(event: MessageEvent, msg: str = ArgStr("msg")) -> None:
-    user_id = event.user_id
-    if msg not in ["是", "yes", "Y", "y", "YES", "true"]:
-        await reset_config.finish(message=MessageSegment.text("操作取消(*^▽^*)"), at_sender=True, reply_message=True)
-    else:
-        try:
-            ip = get_driver().config.dxx_ip
-        except AttributeError:
-            s = socket.socket(socket.AF_INET, socket.SOCK_DGRAM)
-            s.connect(('114.114.114.114', 12345))
-            ip = s.getsockname()[0]
-        data = {
-            "TOKEN_TIME": 30,
-            "SUPERUSER": user_id,
-            "KEY": "d82ffad91168fb324ab6ebc2bed8dacd43f5af8e34ad0d1b75d83a0aff966a06",
-            "ALGORITHM": "HS256",
-            "PASSWORD": await to_hash("admin"),
-            "DXX_IP": ip
-        }
-        status = saveConfig(data=data)
-        if status:
-            await reset_config.finish(message=MessageSegment.text("重置成功(oﾟ▽ﾟ)o  "), at_sender=True,
-                                      reply_message=True)
-        else:
-            await reset_config.finish(message=MessageSegment.text("重置失败╮(╯﹏╰）╭ "), at_sender=True,
-                                      reply_message=True)
-
-
-@reset_password.handle()
-async def reset_password_(event: MessageEvent) -> None:
-    user_id = event.user_id
-    result = await User.filter(user_id=user_id).count()
-    if not result:
-        await reset_password.finish(message=MessageSegment.text("重置失败，用户数据不存在！( ･´ω`･ )"), at_sender=True,
-                                    reply_message=True)
-
-
-@reset_password.got(key="msg", prompt="是否重置大学习登录密码？（是|否）")
-async def reset_password_(event: MessageEvent, msg: str = ArgStr("msg")) -> None:
-    user_id = event.user_id
-    if msg not in ["是", "yes", "Y", "y", "YES", "true"]:
-        await reset_password.finish(message=MessageSegment.text("操作取消(*^▽^*)"), at_sender=True, reply_message=True)
-    else:
-        await User.filter(user_id=user_id).update(
-            password=await to_hash(str(user_id))
-        )
-        await reset_password.finish(message=MessageSegment.text("登录密码重置成功，默认为用户QQ(๑*◡*๑)"),
-                                    at_sender=True, reply_message=True)
-
-
-@delete_dxx.handle()
-async def delete_dxx_(event: GroupMessageEvent, state: T_State) -> None:
-    user_id = event.user_id
-    result = await User.filter(user_id=user_id).values("id")
-    if result:
-        state["id"] = result[0]["id"]
-    else:
-        await delete_dxx.finish(message=MessageSegment.text("操作失败，用户数据不存在(*^▽^*)"), at_sender=True,
-                                reply_message=True)
-
-
-@delete_dxx.got(key="msg", prompt="是否删除大学习数据？（是|否）")
-async def delete_dxx_(state: T_State, msg: str = ArgStr("msg")) -> None:
-    if msg not in ["是", "yes", "Y", "y", "YES", "true"]:
-        await delete_dxx.finish(message=MessageSegment.text("操作取消(*^▽^*)"), at_sender=True, reply_message=True)
-    else:
-        await User.filter(id=state["id"]).delete()
-        await delete_dxx.finish(message=MessageSegment.text("删除成功(*^▽^*)"), at_sender=True, reply_message=True)
-
-
-@scheduler.scheduled_job('cron', day_of_week='0', hour=CONFIG["DXX_REMIND_HOUR"], minute=CONFIG["DXX_REMIND_MINUTE"],
-                         id='push_dxx', timezone="Asia/Shanghai")
-async def push_dxx() -> None:
-    config = getConfig()
-    if not config["DXX_REMIND"]:
-        return
-    try:
-        bot: Bot = get_bot()
-    except ValueError as e:
-        logger.error(e)
-        return None
-    answer_result = await Answer.all().order_by('time').values()
-    if (int(time.time()) - answer_result[-1]["time"]) > 259200:
-        return None
-    else:
-        catalogue = answer_result[-1]["catalogue"]
-        now_time = datetime.datetime.fromtimestamp(answer_result[-1]["time"]).strftime("%Y年%m月%d日 %H:%M:%S")
-        message = f'\n本周的大学习开始喽!\n{catalogue}\n更新时间：{now_time}\n答案见图一\n完成截图见图二\nPs:当11:00:00以后，可使用 提交大学习 指令或戳一戳Bot完成大学习!'
-        push_list = await PushList.filter(status=True).values()
-        for item in push_list:
-            try:
-                await bot.send_group_msg(group_id=item["group_id"],
-                                         message=MessageSegment.at("all") + MessageSegment.text(
-                                             message) + MessageSegment.image(
-                                             await get_answer_pic()) + MessageSegment.image(await get_end_pic()))
-                await asyncio.sleep(random.randint(15, 30))
-            except Exception as e:
-                logger.error(e)
-                continue
-
-
-@scheduler.scheduled_job('cron', day_of_week='0', hour=CONFIG["AUTO_SUBMIT_HOUR"], minute=CONFIG["AUTO_SUBMIT_MINUTE"],
-                         id='auto_dxx', timezone="Asia/Shanghai")
-async def auto_dxx() -> None:
-    config = getConfig()
-    if not config["AUTO_SUBMIT"]:
-        return
-    answer_result = await Answer.all().order_by('time').values()
-    if (int(time.time()) - answer_result[-1]["time"]) > 259200:
-        return None
-    else:
-        user_list = await User.all().values("id", "area", "catalogue", "user_id")
-        catalogue = answer_result[-1]["catalogue"]
-        for item in user_list:
-            result = await User.filter(id=item["id"]).values("id", "area", "catalogue", "user_id", "auto_submit")
-            if result[0]["catalogue"] == catalogue or not result[0]["auto_submit"]:
-                continue
-            else:
-                await distribute_area(user_id=item["user_id"], area=item["area"])
-                await asyncio.sleep(random.randint(15, 45))
+import asyncio
+import datetime
+import random
+import socket
+import time
+
+from nonebot import get_driver, on_notice, require, get_bot
+from nonebot import on_command, logger
+from nonebot.adapters.onebot.v11 import GroupMessageEvent, MessageSegment, Bot, GROUP, Message, MessageEvent, \
+    PokeNotifyEvent
+from nonebot.params import ArgStr, T_State, CommandArg
+from nonebot.permission import SUPERUSER
+from nonebot.rule import Rule
+
+from .path import getConfig, saveConfig
+from .rule import must_command, check_poke, check_time, must_group, must_leader
+from .utils import get_end_pic, distribute_area, distribute_area_url, get_answer_pic, get_qrcode, get_login_qrcode, \
+    to_hash
+from ..models.accuont import User, AddUser
+from ..models.dxx import Area, Answer, PushList
+
+scheduler = require('nonebot_plugin_apscheduler').scheduler
+SUPERS = get_driver().config.superusers
+CONFIG = getConfig()
+
+end_pic = on_command("end_pic", aliases={"完成截图", "大学习截图"}, permission=SUPERUSER | GROUP,
+                     rule=Rule(must_command, must_group),
+                     priority=50)
+
+submit = on_command("submit", aliases={"提交大学习"}, permission=SUPERUSER | GROUP, rule=Rule(must_command, must_group),
+                    priority=50)
+add = on_command("add_dxx", aliases={"添加大学习"}, permission=GROUP, rule=must_group, priority=50)
+my_info = on_command("my_info", aliases={"我的大学习"}, permission=SUPERUSER | GROUP,
+                     rule=Rule(must_command, must_group), priority=50)
+poke_notify = on_notice(priority=60, rule=Rule(check_poke,must_group))
+answer_pic = on_command("answer_pic", aliases={"答案截图", "大学习"}, rule=Rule(must_command, must_group),
+                        permission=SUPERUSER | GROUP,
+                        priority=50)
+finish_dxx = on_command("finish_dxx", aliases={"完成大学习", "全员大学习"},
+                        rule=Rule(must_command, must_group, must_leader), permission=GROUP | SUPERUSER, priority=50)
+reset_config = on_command("reset_config", aliases={"重置配置", "刷新配置"}, permission=SUPERUSER, rule=must_command,
+                          priority=50)
+reset_password = on_command("reset_password", aliases={"重置密码"}, permission=GROUP,
+                            rule=Rule(must_command, must_group), priority=50)
+delete_dxx = on_command("delete_dxx", aliases={"删除大学习"}, priority=50, rule=Rule(must_command, must_group))
+
+
+@end_pic.handle()
+async def test_() -> None:
+    await end_pic.finish(
+        message=MessageSegment.text("青年大学习最新一期完成截图") + MessageSegment.image(await get_end_pic()),
+        at_sender=True, reply_message=True)
+
+
+@submit.handle()
+async def submit_(event: GroupMessageEvent) -> None:
+    user_id = event.user_id
+    result = await User.filter(user_id=user_id).values()
+    if result:
+        if not await check_time():
+            await submit.finish(
+                message=MessageSegment.text("当前时间段禁止提交青年大学习，请在周一11:00之后再提交哦(｡･ω･｡)"),
+                at_sender=True, reply_message=True)
+        area = result[0]['area']
+        data = await distribute_area(user_id=user_id, area=area)
+        if data['status'] == 0:
+            message = f'青年大学习{data["catalogue"]}提交成功( ･´ω`･ )'
+            config = getConfig()
+            content = await get_login_qrcode()
+            if config["URL_STATUS"]:
+                await submit.send(message=MessageSegment.text(message) + MessageSegment.text(
+                    f"\n请点击链接登录查看,如QQ点击无法打开，请复制链接到浏览器打开\n{content['url']}"),
+                                  at_sender=True, reply_message=True)
+            else:
+                await submit.send(message=MessageSegment.text(message) + MessageSegment.image(content['content']),
+                                  at_sender=True, reply_message=True)
+            await asyncio.sleep(1)
+            await submit.finish(
+                message=MessageSegment.text("青年大学习最新一期完成截图") + MessageSegment.image(await get_end_pic()),
+                at_sender=True, reply_message=True)
+        await submit.finish(message=MessageSegment.text(data['msg']), at_sender=True, reply_message=True)
+    else:
+        await submit.finish(message=MessageSegment.text("用户数据不存在！请使用 添加大学习 指令添加(｡･ω･｡)"),
+                            at_sender=True, reply_message=True)
+
+
+@add.handle()
+async def add_(state: T_State, event: GroupMessageEvent, msg: Message = CommandArg()) -> None:
+    user_id = event.user_id
+    if await User.filter(user_id=user_id).count():
+        await add.finish(message=MessageSegment.text("你已经添加过了，不要重复添加哦( • ̀ω•́ )✧"), at_sender=True,
+                         reply_message=True)
+    if str(msg):
+        state['province'] = str(msg)
+
+
+@add.got(key="province", prompt="请输入需要添加的省份或回复 取消 停止操作！")
+async def add_(event: GroupMessageEvent, province: str = ArgStr("province")) -> None:
+    group_id = event.group_id
+    user_id = event.user_id
+    config = getConfig()
+    if province in ["取消", "No", "停止", "NO"]:
+        await add.finish(message=MessageSegment.text("操作取消！φ(>ω<*) "), at_sender=True, reply_message=True)
+    if await Area.filter(area=province).count():
+        url = await distribute_area_url(province=province, user_id=user_id, group_id=group_id)
+        if province in ["上海", "浙江"]:
+            content = await get_qrcode(user_id=user_id, group_id=group_id, area=province)
+            if config["URL_STATUS"]:
+                result = await add.send(
+                    message=MessageSegment.text(f"请复制链接到微信点击打开进行绑定( ･´ω`･ )\n{content['url']}"),
+                    at_sender=True,
+                    reply_message=True)
+            else:
+                result = await add.send(
+                    message=MessageSegment.text("请使用微信扫码进行绑定( ･´ω`･ )") + MessageSegment.image(
+                        content["content"]), at_sender=True,
+                    reply_message=True)
+        else:
+            if config["URL_STATUS"]:
+                result = await add.send(
+                    message=MessageSegment.text(
+                        f"请点击链接进入网页添加绑定，如QQ无法打开链接，请复制链接到浏览器( ･´ω`･ )\n{url['url']}"),
+                    at_sender=True,
+                    reply_message=True)
+            else:
+                result = await add.send(
+                    message=MessageSegment.text(f"请扫码进入网页添加绑定( ･´ω`･ )") + MessageSegment.image(
+                        url['content']),
+                    at_sender=True,
+                    reply_message=True)
+        await AddUser.create(
+            time=time.time(),
+            user_id=user_id,
+            group_id=group_id,
+            area=province,
+            message_id=result["message_id"],
+            status="未通过"
+        )
+    else:
+        await add.reject(
+            prompt=MessageSegment.text(
+                "该省份暂不支持或输入省份名称（名称不要带省字）错误，请重新输入或回复 取消 停止操作( ･´ω`･ )"),
+            at_sender=True,
+            reply_message=True)
+
+
+@my_info.handle()
+async def my_info_(event: MessageEvent) -> None:
+    user_id = event.user_id
+    config = getConfig()
+    if await User.filter(user_id=user_id).count():
+        content = await get_login_qrcode()
+        if config["URL_STATUS"]:
+            await my_info.finish(
+                message=MessageSegment.text(
+                    f'请点击链接登录查看哦，如QQ打不开链接，请复制链接到浏览器(｡･ω･｡)\n{content["url"]}'),
+                at_sender=True, reply_message=True)
+        else:
+            await my_info.finish(
+                message=MessageSegment.text('请扫码登录查看哦(｡･ω･｡)') + MessageSegment.image(content['content']),
+                at_sender=True, reply_message=True)
+    else:
+        await my_info.finish(
+            message=MessageSegment.text("你还没有绑定大学习哦ヾ(ｏ･ω･)ﾉ，使用 添加大学习 指令进行绑定信息吧( • ̀ω•́ )✧"),
+            at_sender=True, reply_message=True)
+
+
+@poke_notify.handle()
+async def poke_notify_(bot: Bot, event: PokeNotifyEvent):
+    config = getConfig()
+    if not config["POKE_SUBMIT"]:
+        return
+    try:
+        group_id = event.group_id
+    except AttributeError:
+        group_id = None
+    user_id = event.user_id
+    target_id = event.target_id
+    if target_id != int(bot.self_id):
+        return
+    if group_id:
+        result = await User.filter(user_id=user_id).values()
+        if result:
+            if not await check_time():
+                await submit.finish(
+                    message=MessageSegment.text("当前时间段禁止提交青年大学习，请在周一11:00之后再提交哦(｡･ω･｡)"),
+                    at_sender=True)
+            area = result[0]['area']
+            data = await distribute_area(user_id=user_id, area=area)
+            if data['status'] == 0:
+                message = f'青年大学习{data["catalogue"]}提交成功( ･´ω`･ )'
+                content = await get_login_qrcode()
+                if config["URL_STATUS"]:
+                    await poke_notify.send(
+                        message=MessageSegment.text(message) + MessageSegment.text(
+                            f"\n请点击链接登录查看,如QQ点击无法打开，请复制链接到浏览器打开\n{content['url']}"),
+                        at_sender=True)
+                else:
+                    await poke_notify.send(
+                        message=MessageSegment.text(message + "\n个人信息请扫码登录查看") + MessageSegment.image(
+                            content["content"]), at_sender=True)
+                await asyncio.sleep(1)
+                await poke_notify.finish(
+                    message=MessageSegment.text("青年大学习最新一期完成截图") + MessageSegment.image(
+                        await get_end_pic()), at_sender=True,
+                    reply_message=True)
+            await poke_notify.finish(message=MessageSegment.text(data['msg']), at_sender=True, reply_message=True)
+        else:
+            await poke_notify.finish(
+                message=MessageSegment.text("用户数据不存在！请使用 添加大学习 指令进行绑定(*^▽^*)"), at_sender=True,
+                reply_message=True)
+    else:
+        await bot.send_private_msg(user_id=user_id,
+                                   message=MessageSegment.at(user_id) + MessageSegment.text("别戳啦(~￣△￣)~"))
+
+
+@answer_pic.handle()
+async def answer_pic_() -> None:
+    await answer_pic.finish(message=MessageSegment.image(await get_answer_pic()), at_sender=True, reply_message=True)
+
+
+@finish_dxx.handle()
+async def finish() -> None:
+    if not await check_time():
+        await submit.finish(
+            message=MessageSegment.text("当前时间段禁止提交青年大学习，请在周一11:00之后再发指令哦(｡･ω･｡)"),
+            at_sender=True, reply_message=True)
+
+
+@finish_dxx.got(key="msg", prompt="是否提交团支部全体成员最新一期青年大学习？（是|否）")
+async def finish(event: GroupMessageEvent, msg: str = ArgStr("msg")) -> None:
+    if msg not in ["是", "yes", "Y", "y", "YES", "true"]:
+        await finish_dxx.finish(message=MessageSegment.text("操作取消(*^▽^*)"), at_sender=True, reply_message=True)
+    else:
+        await finish_dxx.send(message=MessageSegment.text("开始提交(*￣︶￣)"), at_sender=True, reply_message=True)
+
+    group_id = event.group_id
+    user_id = event.user_id
+    result = await User.filter(leader=user_id, group_id=group_id).values()
+    if result:
+        answer_result = await Answer.all().order_by('time').values()
+        catalogue = answer_result[-1]["catalogue"]
+        for item in result:
+            if item["catalogue"] == catalogue:
+                continue
+            else:
+                await distribute_area(user_id=item["user_id"], area=item["area"])
+                await asyncio.sleep(random.randint(10, 15))
+    await finish_dxx.finish(message=MessageSegment.text("提交完成！"), at_sender=True, reply_message=True)
+
+
+@reset_config.got(key="msg", prompt="是否重置大学习配置为默认配置？（是|否）")
+async def reset_config_(event: MessageEvent, msg: str = ArgStr("msg")) -> None:
+    user_id = event.user_id
+    if msg not in ["是", "yes", "Y", "y", "YES", "true"]:
+        await reset_config.finish(message=MessageSegment.text("操作取消(*^▽^*)"), at_sender=True, reply_message=True)
+    else:
+        try:
+            ip = get_driver().config.dxx_ip
+        except AttributeError:
+            s = socket.socket(socket.AF_INET, socket.SOCK_DGRAM)
+            s.connect(('114.114.114.114', 12345))
+            ip = s.getsockname()[0]
+        data = {
+            "TOKEN_TIME": 30,
+            "SUPERUSER": user_id,
+            "KEY": "d82ffad91168fb324ab6ebc2bed8dacd43f5af8e34ad0d1b75d83a0aff966a06",
+            "ALGORITHM": "HS256",
+            "PASSWORD": await to_hash("admin"),
+            "DXX_IP": ip
+        }
+        status = saveConfig(data=data)
+        if status:
+            await reset_config.finish(message=MessageSegment.text("重置成功(oﾟ▽ﾟ)o  "), at_sender=True,
+                                      reply_message=True)
+        else:
+            await reset_config.finish(message=MessageSegment.text("重置失败╮(╯﹏╰）╭ "), at_sender=True,
+                                      reply_message=True)
+
+
+@reset_password.handle()
+async def reset_password_(event: MessageEvent) -> None:
+    user_id = event.user_id
+    result = await User.filter(user_id=user_id).count()
+    if not result:
+        await reset_password.finish(message=MessageSegment.text("重置失败，用户数据不存在！( ･´ω`･ )"), at_sender=True,
+                                    reply_message=True)
+
+
+@reset_password.got(key="msg", prompt="是否重置大学习登录密码？（是|否）")
+async def reset_password_(event: MessageEvent, msg: str = ArgStr("msg")) -> None:
+    user_id = event.user_id
+    if msg not in ["是", "yes", "Y", "y", "YES", "true"]:
+        await reset_password.finish(message=MessageSegment.text("操作取消(*^▽^*)"), at_sender=True, reply_message=True)
+    else:
+        await User.filter(user_id=user_id).update(
+            password=await to_hash(str(user_id))
+        )
+        await reset_password.finish(message=MessageSegment.text("登录密码重置成功，默认为用户QQ(๑*◡*๑)"),
+                                    at_sender=True, reply_message=True)
+
+
+@delete_dxx.handle()
+async def delete_dxx_(event: GroupMessageEvent, state: T_State) -> None:
+    user_id = event.user_id
+    result = await User.filter(user_id=user_id).values("id")
+    if result:
+        state["id"] = result[0]["id"]
+    else:
+        await delete_dxx.finish(message=MessageSegment.text("操作失败，用户数据不存在(*^▽^*)"), at_sender=True,
+                                reply_message=True)
+
+
+@delete_dxx.got(key="msg", prompt="是否删除大学习数据？（是|否）")
+async def delete_dxx_(state: T_State, msg: str = ArgStr("msg")) -> None:
+    if msg not in ["是", "yes", "Y", "y", "YES", "true"]:
+        await delete_dxx.finish(message=MessageSegment.text("操作取消(*^▽^*)"), at_sender=True, reply_message=True)
+    else:
+        await User.filter(id=state["id"]).delete()
+        await delete_dxx.finish(message=MessageSegment.text("删除成功(*^▽^*)"), at_sender=True, reply_message=True)
+
+
+@scheduler.scheduled_job('cron', day_of_week='0', hour=CONFIG["DXX_REMIND_HOUR"], minute=CONFIG["DXX_REMIND_MINUTE"],
+                         id='push_dxx', timezone="Asia/Shanghai")
+async def push_dxx() -> None:
+    config = getConfig()
+    if not config["DXX_REMIND"]:
+        return
+    try:
+        bot: Bot = get_bot()
+    except ValueError as e:
+        logger.error(e)
+        return None
+    answer_result = await Answer.all().order_by('time').values()
+    if (int(time.time()) - answer_result[-1]["time"]) > 259200:
+        return None
+    else:
+        catalogue = answer_result[-1]["catalogue"]
+        now_time = datetime.datetime.fromtimestamp(answer_result[-1]["time"]).strftime("%Y年%m月%d日 %H:%M:%S")
+        message = f'\n本周的大学习开始喽!\n{catalogue}\n更新时间：{now_time}\n答案见图一\n完成截图见图二\nPs:当11:00:00以后，可使用 提交大学习 指令或戳一戳Bot完成大学习!'
+        push_list = await PushList.filter(status=True).values()
+        for item in push_list:
+            try:
+                await bot.send_group_msg(group_id=item["group_id"],
+                                         message=MessageSegment.at("all") + MessageSegment.text(
+                                             message) + MessageSegment.image(
+                                             await get_answer_pic()) + MessageSegment.image(await get_end_pic()))
+                await asyncio.sleep(random.randint(15, 30))
+            except Exception as e:
+                logger.error(e)
+                continue
+
+
+@scheduler.scheduled_job('cron', day_of_week='0', hour=CONFIG["AUTO_SUBMIT_HOUR"], minute=CONFIG["AUTO_SUBMIT_MINUTE"],
+                         id='auto_dxx', timezone="Asia/Shanghai")
+async def auto_dxx() -> None:
+    config = getConfig()
+    if not config["AUTO_SUBMIT"]:
+        return
+    answer_result = await Answer.all().order_by('time').values()
+    if (int(time.time()) - answer_result[-1]["time"]) > 259200:
+        return None
+    else:
+        user_list = await User.all().values("id", "area", "catalogue", "user_id")
+        catalogue = answer_result[-1]["catalogue"]
+        for item in user_list:
+            result = await User.filter(id=item["id"]).values("id", "area", "catalogue", "user_id", "auto_submit")
+            if result[0]["catalogue"] == catalogue or not result[0]["auto_submit"]:
+                continue
+            else:
+                await distribute_area(user_id=item["user_id"], area=item["area"])
+                await asyncio.sleep(random.randint(15, 45))
```

### Comparing `TeenStudy-0.1.9/TeenStudy/utils/path.py` & `teenstudy-0.2.0rc1/TeenStudy/utils/path.py`

 * *Ordering differences only*

 * *Files 17% similar despite different names*

```diff
@@ -1,136 +1,136 @@
-import json
-from pathlib import Path
-from typing import Optional, Union
-
-from nonebot import logger
-from pydantic import BaseModel
-from tortoise import Tortoise
-
-from ..models import accuont, dxx
-
-# 插件基础数据
-DATABASE_PATH = Path().cwd() / 'data' / 'TeenStudy'
-
-DATABASE_PATH.mkdir(parents=True, exist_ok=True)
-PATH = DATABASE_PATH / "database.db"
-CONFIG_PATH = DATABASE_PATH / "config.json"
-DATABASE = {
-    'connections': {
-        'TeenStudy_database': {
-            'engine': 'tortoise.backends.sqlite',
-            'credentials': {'file_path': PATH},
-        }
-    },
-    "apps": {
-        'TeenStudy_database': {
-            'models': [accuont.__name__,
-                       dxx.__name__],
-            'default_connection': 'TeenStudy_database',
-        }
-    },
-    'use_tz': False,
-    'timezone': 'Asia/Shanghai'
-}
-
-
-class Config(BaseModel):
-    DXX_IP: str = "127.0.0.1"
-    """大学习访问IP"""
-    DXX_PORT: int = None
-    """大学习访问端口"""
-    SUPERUSER: int = None
-    """超管账号"""
-    KEY: str = "d82ffad91168fb324ab6ebc2bed8dacd43f5af8e34ad0d1b75d83a0aff966a06"
-    """大学习秘钥，为64位哈希散列值，用于生成token"""
-    ALGORITHM: str = "HS256"
-    """加密算法"""
-    TOKEN_TIME: int = 30
-    """token时效"""
-    PASSWORD: str = None
-    """后台登录算法"""
-    DXX_REMIND: bool = True
-    """周一检测更新提醒"""
-    DXX_REMIND_HOUR: int = 9
-    """大学习更新提醒时间-小时，可填范围：0-23"""
-    DXX_REMIND_MINUTE: int = 0
-    """大学习更新提醒时间-分钟，可选范围：0-59"""
-    POKE_SUBMIT: bool = True
-    """戳一戳提交大学习状态"""
-    AUTO_SUBMIT: bool = True
-    """周一11:30自动提交状态"""
-    AUTO_SUBMIT_HOUR: int = 11
-    """大学习自动提交时间-小时，可选范围：0-23"""
-    AUTO_SUBMIT_MINUTE: int = 30
-    """大学习自动提交时间-分钟，可选范围：0-59"""
-    URL_STATUS: bool = False
-    """是否将二维码转链接发送，默认为False"""
-
-
-def saveConfig(data: dict) -> bool:
-    try:
-        config = Config().dict()
-        config.update(**data)
-        with open(CONFIG_PATH, "w", encoding="utf-8") as w:
-            json.dump(config, w, ensure_ascii=False, indent=4)
-        return True
-    except Exception as e:
-        logger.error(e)
-        return False
-
-
-def getConfig() -> dict:
-    if not Path(CONFIG_PATH).exists():
-        status = saveConfig({
-        })
-        if status:
-            return Config().dict()
-    else:
-        with open(CONFIG_PATH, "r", encoding="utf-8") as f:
-            obj = json.load(f)
-        if "URL_STATUS" not in obj.keys():
-            obj["URL_STATUS"] = False
-            with open(CONFIG_PATH, "w", encoding="utf-8") as w:
-                json.dump(obj, w, indent=4, ensure_ascii=False)
-        return obj
-
-
-def register_database(db_name: str, models: str, db_path: Optional[Union[str, Path]]):
-    """
-    注册数据库
-    :param db_name: 数据库名称
-    :param models: 数据存储模型
-    :param db_path: 数据存储路径
-    :return:
-    """
-    if db_name in DATABASE['connections'] and db_name in DATABASE['apps']:
-        DATABASE['apps'][db_name]['models'].append(models)
-    else:
-        DATABASE['connections'][db_name] = {
-            'engine': 'tortoise.backends.sqlite',
-            'credentials': {'file_path': db_path},
-        }
-        DATABASE['apps'][db_name] = {
-            'models': [models],
-            'default_connection': db_name,
-        }
-
-
-async def connect():
-    """
-    建立数据库连接
-    """
-    try:
-        await Tortoise.init(DATABASE)
-        await Tortoise.generate_schemas()
-        logger.opt(colors=True).success('<u><y>[大学习数据库]</y></u><g>➤➤➤➤➤连接成功✔✔✔✔✔</g>')
-    except Exception as e:
-        logger.opt(colors=True).warning(f'<u><y>[大学习数据库]</y></u><r>➤➤➤➤➤连接失败✘✘✘✘✘:{e}</r>')
-        raise e
-
-
-async def disconnect():
-    """
-    断开数据库连接
-    """
-    await Tortoise.close_connections()
-    logger.opt(colors=True).success('<u><y>[大学习数据库]</y></u><r>◄◄◄◄◄连接已断开✘✘✘✘✘</r>')
+import json
+from pathlib import Path
+from typing import Optional, Union
+
+from nonebot import logger
+from pydantic import BaseModel
+from tortoise import Tortoise
+
+from ..models import accuont, dxx
+
+# 插件基础数据
+DATABASE_PATH = Path().cwd() / 'data' / 'TeenStudy'
+
+DATABASE_PATH.mkdir(parents=True, exist_ok=True)
+PATH = DATABASE_PATH / "database.db"
+CONFIG_PATH = DATABASE_PATH / "config.json"
+DATABASE = {
+    'connections': {
+        'TeenStudy_database': {
+            'engine': 'tortoise.backends.sqlite',
+            'credentials': {'file_path': PATH},
+        }
+    },
+    "apps": {
+        'TeenStudy_database': {
+            'models': [accuont.__name__,
+                       dxx.__name__],
+            'default_connection': 'TeenStudy_database',
+        }
+    },
+    'use_tz': False,
+    'timezone': 'Asia/Shanghai'
+}
+
+
+class Config(BaseModel):
+    DXX_IP: str = "127.0.0.1"
+    """大学习访问IP"""
+    DXX_PORT: int = None
+    """大学习访问端口"""
+    SUPERUSER: int = None
+    """超管账号"""
+    KEY: str = "d82ffad91168fb324ab6ebc2bed8dacd43f5af8e34ad0d1b75d83a0aff966a06"
+    """大学习秘钥，为64位哈希散列值，用于生成token"""
+    ALGORITHM: str = "HS256"
+    """加密算法"""
+    TOKEN_TIME: int = 30
+    """token时效"""
+    PASSWORD: str = None
+    """后台登录算法"""
+    DXX_REMIND: bool = True
+    """周一检测更新提醒"""
+    DXX_REMIND_HOUR: int = 9
+    """大学习更新提醒时间-小时，可填范围：0-23"""
+    DXX_REMIND_MINUTE: int = 0
+    """大学习更新提醒时间-分钟，可选范围：0-59"""
+    POKE_SUBMIT: bool = True
+    """戳一戳提交大学习状态"""
+    AUTO_SUBMIT: bool = True
+    """周一11:30自动提交状态"""
+    AUTO_SUBMIT_HOUR: int = 11
+    """大学习自动提交时间-小时，可选范围：0-23"""
+    AUTO_SUBMIT_MINUTE: int = 30
+    """大学习自动提交时间-分钟，可选范围：0-59"""
+    URL_STATUS: bool = False
+    """是否将二维码转链接发送，默认为False"""
+
+
+def saveConfig(data: dict) -> bool:
+    try:
+        config = Config().dict()
+        config.update(**data)
+        with open(CONFIG_PATH, "w", encoding="utf-8") as w:
+            json.dump(config, w, ensure_ascii=False, indent=4)
+        return True
+    except Exception as e:
+        logger.error(e)
+        return False
+
+
+def getConfig() -> dict:
+    if not Path(CONFIG_PATH).exists():
+        status = saveConfig({
+        })
+        if status:
+            return Config().dict()
+    else:
+        with open(CONFIG_PATH, "r", encoding="utf-8") as f:
+            obj = json.load(f)
+        if "URL_STATUS" not in obj.keys():
+            obj["URL_STATUS"] = False
+            with open(CONFIG_PATH, "w", encoding="utf-8") as w:
+                json.dump(obj, w, indent=4, ensure_ascii=False)
+        return obj
+
+
+def register_database(db_name: str, models: str, db_path: Optional[Union[str, Path]]):
+    """
+    注册数据库
+    :param db_name: 数据库名称
+    :param models: 数据存储模型
+    :param db_path: 数据存储路径
+    :return:
+    """
+    if db_name in DATABASE['connections'] and db_name in DATABASE['apps']:
+        DATABASE['apps'][db_name]['models'].append(models)
+    else:
+        DATABASE['connections'][db_name] = {
+            'engine': 'tortoise.backends.sqlite',
+            'credentials': {'file_path': db_path},
+        }
+        DATABASE['apps'][db_name] = {
+            'models': [models],
+            'default_connection': db_name,
+        }
+
+
+async def connect():
+    """
+    建立数据库连接
+    """
+    try:
+        await Tortoise.init(DATABASE)
+        await Tortoise.generate_schemas()
+        logger.opt(colors=True).success('<u><y>[大学习数据库]</y></u><g>➤➤➤➤➤连接成功✔✔✔✔✔</g>')
+    except Exception as e:
+        logger.opt(colors=True).warning(f'<u><y>[大学习数据库]</y></u><r>➤➤➤➤➤连接失败✘✘✘✘✘:{e}</r>')
+        raise e
+
+
+async def disconnect():
+    """
+    断开数据库连接
+    """
+    await Tortoise.close_connections()
+    logger.opt(colors=True).success('<u><y>[大学习数据库]</y></u><r>◄◄◄◄◄连接已断开✘✘✘✘✘</r>')
```

### Comparing `TeenStudy-0.1.9/TeenStudy/utils/rule.py` & `teenstudy-0.2.0rc1/TeenStudy/utils/rule.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,76 +1,88 @@
-import datetime
-
-from nonebot.adapters.onebot.v11 import Bot, Message, MessageEvent, NotifyEvent
-from nonebot.params import CommandArg
-
-from ..models.dxx import PushList
-from ..models.accuont import User
-
-
-async def must_group(bot: Bot, event: MessageEvent) -> bool:
-    """
-    必须是群消息才响应
-    :param bot: 机器人
-    :param event: 事件
-    :return: 返回True或False
-    """
-    if event.message_type == "group":
-        self_id = int(bot.self_id)
-        group_id = event.group_id
-        if await PushList.filter(group_id=group_id, status=True, self_id=self_id).count():
-            return True
-    else:
-        return False
-
-
-async def must_command(order: Message = CommandArg()) -> bool:
-    """
-    限制指令后面不能加内容才生效
-    :param order: 指令后面的内容
-    :return: 返回True或False
-    """
-    if order:
-        return False
-    else:
-        return True
-
-
-async def must_leader(bot: Bot, event: MessageEvent) -> bool:
-    """
-    只有团支书发送才生效
-    :param bot: 机器人id
-    :param event: 消息事件
-    :return:
-    """
-    if event.message_type == "group":
-        self_id = int(bot.self_id)
-        group_id = event.group_id
-        user_id = event.user_id
-        if await User.filter(leader=user_id, group_id=group_id).count():
-            return True
-    else:
-        return False
-
-
-async def check_poke(event: NotifyEvent) -> bool:
-    """
-    判断是否为戳一戳消息通知
-    :param event: 通知事件
-    :return: 返回True或False
-    """
-    if event.sub_type in ["poke"]:
-        return True
-    else:
-        return False
-
-
-async def check_time():
-    now_day = datetime.datetime.now().weekday()
-    now_hour = datetime.datetime.now().hour
-    if now_day in [0,  6]:
-        if now_day in [5, 6]:
-            return False
-        else:
-            if now_hour in [0, 1, 2, 3, 4, 5, 6, 7, 8, 9, 10]:
-                return False
-    return True
+import datetime
+from typing import Union
+
+from nonebot.adapters.onebot.v11 import Bot, Message, MessageEvent, NotifyEvent
+from nonebot.params import CommandArg
+
+from ..models.accuont import User
+from ..models.dxx import PushList
+
+
+async def must_group(bot: Bot, event: Union[MessageEvent, NotifyEvent]) -> bool:
+    """
+    必须是群消息才响应
+    :param bot: 机器人
+    :param event: 事件
+    :return: 返回True或False
+    """
+    if isinstance(event, MessageEvent):
+        if event.message_type == "group":
+            self_id = int(bot.self_id)
+            group_id = event.group_id
+            if await PushList.filter(group_id=group_id, status=True, self_id=self_id).count():
+                return True
+
+        else:
+            return False
+    else:
+        try:
+            group_id = event.group_id
+        except AttributeError:
+            return False
+        self_id = int(bot.self_id)
+        if await PushList.filter(group_id=group_id, status=True, self_id=self_id).count():
+            return True
+        return False
+
+
+async def must_command(order: Message = CommandArg()) -> bool:
+    """
+    限制指令后面不能加内容才生效
+    :param order: 指令后面的内容
+    :return: 返回True或False
+    """
+    if order:
+        return False
+    else:
+        return True
+
+
+async def must_leader(bot: Bot, event: MessageEvent) -> bool:
+    """
+    只有团支书发送才生效
+    :param bot: 机器人id
+    :param event: 消息事件
+    :return:
+    """
+    if event.message_type == "group":
+        self_id = int(bot.self_id)
+        group_id = event.group_id
+        user_id = event.user_id
+        if await User.filter(leader=user_id, group_id=group_id).count():
+            return True
+    else:
+        return False
+
+
+async def check_poke(event: NotifyEvent) -> bool:
+    """
+    判断是否为戳一戳消息通知
+    :param event: 通知事件
+    :return: 返回True或False
+    """
+    if event.sub_type in ["poke"]:
+        return True
+    else:
+        return False
+
+
+async def check_time():
+    now_day = datetime.datetime.now().weekday()
+    now_hour = datetime.datetime.now().hour
+    if now_day in [0, 5, 6]:
+        if now_day in [5, 6]:
+            return False
+        else:
+            if now_hour in [0, 1, 2, 3, 4, 5, 6, 7, 8, 9, 10]:
+                return False
+    return True
```

### Comparing `TeenStudy-0.1.9/TeenStudy/utils/update.py` & `teenstudy-0.2.0rc1/TeenStudy/utils/update.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,651 +1,636 @@
-00000000: 696d 706f 7274 2061 7379 6e63 696f 0d0a  import asyncio..
-00000010: 696d 706f 7274 206a 736f 6e0d 0a69 6d70  import json..imp
-00000020: 6f72 7420 7469 6d65 0d0a 0d0a 6672 6f6d  ort time....from
-00000030: 2062 7334 2069 6d70 6f72 7420 4265 6175   bs4 import Beau
-00000040: 7469 6675 6c53 6f75 700d 0a66 726f 6d20  tifulSoup..from 
-00000050: 6874 7470 7820 696d 706f 7274 2041 7379  httpx import Asy
-00000060: 6e63 436c 6965 6e74 0d0a 6672 6f6d 206e  ncClient..from n
-00000070: 6f6e 6562 6f74 2069 6d70 6f72 7420 6c6f  onebot import lo
-00000080: 6767 6572 2c20 7265 7175 6972 652c 2067  gger, require, g
-00000090: 6574 5f62 6f74 2c20 6765 745f 6472 6976  et_bot, get_driv
-000000a0: 6572 0d0a 6672 6f6d 206e 6f6e 6562 6f74  er..from nonebot
-000000b0: 2e61 6461 7074 6572 732e 6f6e 6562 6f74  .adapters.onebot
-000000c0: 2e76 3131 2069 6d70 6f72 7420 426f 742c  .v11 import Bot,
-000000d0: 204d 6573 7361 6765 5365 676d 656e 740d   MessageSegment.
-000000e0: 0a0d 0a66 726f 6d20 2e70 6174 6820 696d  ...from .path im
-000000f0: 706f 7274 2067 6574 436f 6e66 6967 0d0a  port getConfig..
-00000100: 6672 6f6d 202e 7574 696c 7320 696d 706f  from .utils impo
-00000110: 7274 2067 6574 5f6c 6f67 696e 5f71 7263  rt get_login_qrc
-00000120: 6f64 650d 0a66 726f 6d20 2e2e 6d6f 6465  ode..from ..mode
-00000130: 6c73 2e61 6363 756f 6e74 2069 6d70 6f72  ls.accuont impor
-00000140: 7420 4164 6455 7365 722c 2055 7365 720d  t AddUser, User.
-00000150: 0a66 726f 6d20 2e2e 6d6f 6465 6c73 2e64  .from ..models.d
-00000160: 7878 2069 6d70 6f72 7420 416e 7377 6572  xx import Answer
-00000170: 2c20 4172 6561 0d0a 0d0a 7363 6865 6475  , Area....schedu
-00000180: 6c65 7220 3d20 7265 7175 6972 6528 276e  ler = require('n
-00000190: 6f6e 6562 6f74 5f70 6c75 6769 6e5f 6170  onebot_plugin_ap
-000001a0: 7363 6865 6475 6c65 7227 292e 7363 6865  scheduler').sche
-000001b0: 6475 6c65 720d 0a73 7570 6572 5f69 6420  duler..super_id 
-000001c0: 3d20 6765 745f 6472 6976 6572 2829 2e63  = get_driver().c
-000001d0: 6f6e 6669 672e 7375 7065 7275 7365 7273  onfig.superusers
-000001e0: 2020 2320 e8b6 85e7 aea1 6964 0d0a 6865    # ......id..he
-000001f0: 6164 6572 7320 3d20 7b0d 0a20 2020 2022  aders = {..    "
-00000200: 486f 7374 223a 2022 6835 2e63 796f 6c2e  Host": "h5.cyol.
-00000210: 636f 6d22 2c0d 0a20 2020 2022 436f 6e6e  com",..    "Conn
-00000220: 6563 7469 6f6e 223a 2022 6b65 6570 2d61  ection": "keep-a
-00000230: 6c69 7665 222c 0d0a 2020 2020 2241 6363  live",..    "Acc
-00000240: 6570 7422 3a20 2261 7070 6c69 6361 7469  ept": "applicati
-00000250: 6f6e 2f6a 736f 6e2c 2074 6578 742f 6a61  on/json, text/ja
-00000260: 7661 7363 7269 7074 2c20 2a2f 2a3b 2071  vascript, */*; q
-00000270: 3d30 2e30 3122 2c0d 0a20 2020 2022 5573  =0.01",..    "Us
-00000280: 6572 2d41 6765 6e74 223a 2022 4d6f 7a69  er-Agent": "Mozi
-00000290: 6c6c 612f 352e 3020 284c 696e 7578 3b20  lla/5.0 (Linux; 
-000002a0: 416e 6472 6f69 6420 3130 3b20 5041 434d  Android 10; PACM
-000002b0: 3030 2042 7569 6c64 2f51 5031 412e 3139  00 Build/QP1A.19
-000002c0: 3037 3131 2e30 3230 3b20 7776 2920 4170  0711.020; wv) Ap
-000002d0: 706c 6557 6562 4b69 742f 3533 372e 3336  pleWebKit/537.36
-000002e0: 2028 4b48 544d 4c2c 206c 696b 6520 4765   (KHTML, like Ge
-000002f0: 636b 6f29 2056 6572 7369 6f6e 2f34 2e30  cko) Version/4.0
-00000300: 2043 6872 6f6d 652f 3836 2e30 2e34 3234   Chrome/86.0.424
-00000310: 302e 3939 2058 5745 422f 3331 3634 204d  0.99 XWEB/3164 M
-00000320: 4d57 4542 5344 4b2f 3230 3231 3130 3031  MWEBSDK/20211001
-00000330: 204d 6f62 696c 6520 5361 6661 7269 2f35   Mobile Safari/5
-00000340: 3337 2e33 3620 4d4d 5745 4249 442f 3535  37.36 MMWEBID/55
-00000350: 3620 4d69 6372 6f4d 6573 7365 6e67 6572  6 MicroMessenger
-00000360: 2f38 2e30 2e31 362e 3230 3430 2830 7832  /8.0.16.2040(0x2
-00000370: 3830 3031 3035 3629 2050 726f 6365 7373  8001056) Process
-00000380: 2f74 6f6f 6c73 6d70 2057 6543 6861 742f  /toolsmp WeChat/
-00000390: 6172 6d33 3220 5765 6978 696e 204e 6574  arm32 Weixin Net
-000003a0: 5479 7065 2f57 4946 4920 4c61 6e67 7561  Type/WIFI Langua
-000003b0: 6765 2f7a 685f 434e 2041 4249 2f61 726d  ge/zh_CN ABI/arm
-000003c0: 3634 222c 0d0a 2020 2020 224f 7269 6769  64",..    "Origi
-000003d0: 6e22 3a20 2268 7474 703a 2f2f 6835 2e63  n": "http://h5.c
-000003e0: 796f 6c2e 636f 6d22 2c0d 0a20 2020 2022  yol.com",..    "
-000003f0: 582d 5265 7175 6573 7465 642d 5769 7468  X-Requested-With
-00000400: 223a 2022 636f 6d2e 7465 6e63 656e 742e  ": "com.tencent.
-00000410: 6d6d 222c 0d0a 2020 2020 2253 6563 2d46  mm",..    "Sec-F
-00000420: 6574 6368 2d53 6974 6522 3a20 2263 726f  etch-Site": "cro
-00000430: 7373 2d73 6974 6522 2c0d 0a20 2020 2022  ss-site",..    "
-00000440: 5365 632d 4665 7463 682d 4d6f 6465 223a  Sec-Fetch-Mode":
-00000450: 2022 636f 7273 222c 0d0a 2020 2020 2253   "cors",..    "S
-00000460: 6563 2d46 6574 6368 2d44 6573 7422 3a20  ec-Fetch-Dest": 
-00000470: 2265 6d70 7479 222c 0d0a 2020 2020 2241  "empty",..    "A
-00000480: 6363 6570 742d 456e 636f 6469 6e67 223a  ccept-Encoding":
-00000490: 2022 677a 6970 2c20 6465 666c 6174 6522   "gzip, deflate"
-000004a0: 2c0d 0a20 2020 2022 4163 6365 7074 2d4c  ,..    "Accept-L
-000004b0: 616e 6775 6167 6522 3a20 227a 682d 434e  anguage": "zh-CN
-000004c0: 2c7a 683b 713d 302e 392c 656e 2d55 533b  ,zh;q=0.9,en-US;
-000004d0: 713d 302e 382c 656e 3b71 3d30 2e37 222c  q=0.8,en;q=0.7",
-000004e0: 0d0a 7d0d 0a0d 0a0d 0a61 7379 6e63 2064  ..}......async d
-000004f0: 6566 2063 7261 776c 5f61 6e73 7765 7228  ef crawl_answer(
-00000500: 7572 6c3a 2073 7472 2920 2d3e 2064 6963  url: str) -> dic
-00000510: 743a 0d0a 2020 2020 2222 220d 0a20 2020  t:..    """..   
-00000520: 20e8 8eb7 e58f 96e9 9d92 e5b9 b4e5 a4a7   ...............
-00000530: e5ad a6e4 b9a0 e79a 84e6 9c9f e695 b0ef  ................
-00000540: bc8c e7ad 94e6 a188 e592 8ce5 ae8c e688  ................
-00000550: 90e6 88aa e59b bee9 93be e68e a50d 0a20  ............... 
-00000560: 2020 203a 7061 7261 6d20 7572 6c3a 20e6     :param url: .
-00000570: 9c80 e696 b0e4 b880 e69c 9fe5 a4a7 e5ad  ................
-00000580: a6e4 b9a0 e79a 84e5 9cb0 e59d 800d 0a20  ............... 
-00000590: 2020 203a 7265 7475 726e 3a0d 0a20 2020     :return:..   
-000005a0: 2022 2222 0d0a 2020 2020 6173 796e 6320   """..    async 
-000005b0: 7769 7468 2041 7379 6e63 436c 6965 6e74  with AsyncClient
-000005c0: 2868 6561 6465 7273 3d68 6561 6465 7273  (headers=headers
-000005d0: 2c20 6d61 785f 7265 6469 7265 6374 733d  , max_redirects=
-000005e0: 3529 2061 7320 636c 6965 6e74 3a0d 0a20  5) as client:.. 
-000005f0: 2020 2020 2020 2072 6573 7020 3d20 6177         resp = aw
-00000600: 6169 7420 636c 6965 6e74 2e67 6574 2875  ait client.get(u
-00000610: 726c 3d75 726c 2c20 7469 6d65 6f75 743d  rl=url, timeout=
-00000620: 3130 290d 0a20 2020 2072 6573 702e 656e  10)..    resp.en
-00000630: 636f 6469 6e67 203d 2027 7574 662d 3827  coding = 'utf-8'
-00000640: 0d0a 2020 2020 736f 7570 203d 2042 6561  ..    soup = Bea
-00000650: 7574 6966 756c 536f 7570 2872 6573 702e  utifulSoup(resp.
-00000660: 7465 7874 2c20 276c 786d 6c27 290d 0a20  text, 'lxml').. 
-00000670: 2020 2074 6974 6c65 203d 2073 6f75 702e     title = soup.
-00000680: 6669 6e64 2827 7469 746c 6527 292e 7465  find('title').te
-00000690: 7874 5b37 3a5d 2e73 7472 6970 2829 0d0a  xt[7:].strip()..
-000006a0: 2020 2020 7374 6172 745f 6469 7620 3d20      start_div = 
-000006b0: 7265 7370 2e74 6578 742e 6669 6e64 2827  resp.text.find('
-000006c0: 3c64 6976 2063 6c61 7373 3d22 7365 6374  <div class="sect
-000006d0: 696f 6e30 2074 6f70 696e 6465 7822 3e27  ion0 topindex">'
-000006e0: 290d 0a20 2020 2065 6e64 5f64 6976 203d  )..    end_div =
-000006f0: 2072 6573 702e 7465 7874 2e66 696e 6428   resp.text.find(
-00000700: 273c 7363 7269 7074 2074 7970 653d 2274  '<script type="t
-00000710: 6578 742f 6a61 7661 7363 7269 7074 2220  ext/javascript" 
-00000720: 7372 633d 226a 732f 696e 6465 782e 6a73  src="js/index.js
-00000730: 2729 0d0a 2020 2020 736f 7570 203d 2042  ')..    soup = B
-00000740: 6561 7574 6966 756c 536f 7570 2872 6573  eautifulSoup(res
-00000750: 702e 7465 7874 5b73 7461 7274 5f64 6976  p.text[start_div
-00000760: 3a65 6e64 5f64 6976 5d2c 2027 6c78 6d6c  :end_div], 'lxml
-00000770: 2729 0d0a 2020 2020 746d 7020 3d20 5b5d  ')..    tmp = []
-00000780: 0d0a 2020 2020 616e 7377 6572 5f61 7474  ..    answer_att
-00000790: 7273 203d 207b 2272 6571 7569 7265 6422  rs = {"required"
-000007a0: 3a20 5b5d 2c20 226f 7074 696f 6e61 6c22  : [], "optional"
-000007b0: 3a20 5b5d 7d0d 0a20 2020 206f 7074 696f  : []}..    optio
-000007c0: 6e20 3d20 2241 4243 4445 4622 0d0a 2020  n = "ABCDEF"..  
-000007d0: 2020 7465 6d70 6c61 7465 203d 2022 7b6e    template = "{n
-000007e0: 756d 7d2e 207b 6368 6563 6b7d 220d 0a20  um}. {check}".. 
-000007f0: 2020 2066 6f72 2064 6976 2069 6e20 736f     for div in so
-00000800: 7570 2e66 696e 6428 2262 6f64 7922 293a  up.find("body"):
-00000810: 0d0a 2020 2020 2020 2020 6966 2064 6976  ..        if div
-00000820: 203d 3d20 225c 6e22 3a0d 0a20 2020 2020   == "\n":..     
-00000830: 2020 2020 2020 2063 6f6e 7469 6e75 650d         continue.
-00000840: 0a20 2020 2020 2020 2061 6e73 7765 7220  .        answer 
-00000850: 3d20 5b5d 0d0a 2020 2020 2020 2020 6966  = []..        if
-00000860: 2064 6976 2e6e 616d 6520 3d3d 2022 6469   div.name == "di
-00000870: 7622 3a0d 0a20 2020 2020 2020 2020 2020  v":..           
-00000880: 2066 6f72 2069 2069 6e20 6469 762e 6669   for i in div.fi
-00000890: 6e64 5f61 6c6c 2822 6469 7622 293a 0d0a  nd_all("div"):..
-000008a0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000008b0: 6368 6563 6b20 3d20 692e 6765 7428 2264  check = i.get("d
-000008c0: 6174 612d 6122 290d 0a20 2020 2020 2020  ata-a")..       
-000008d0: 2020 2020 2020 2020 2069 6620 6368 6563           if chec
-000008e0: 6b20 6973 206e 6f74 204e 6f6e 653a 0d0a  k is not None:..
-000008f0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00000900: 2020 2020 616e 7377 6572 2e61 7070 656e      answer.appen
-00000910: 6428 6368 6563 6b29 0d0a 2020 2020 2020  d(check)..      
-00000920: 2020 2020 2020 6966 206c 656e 2861 6e73        if len(ans
-00000930: 7765 7229 203e 2034 3a0d 0a20 2020 2020  wer) > 4:..     
-00000940: 2020 2020 2020 2020 2020 2061 6e73 7765             answe
-00000950: 7220 3d20 616e 7377 6572 5b3a 696e 7428  r = answer[:int(
-00000960: 6c65 6e28 616e 7377 6572 2920 2f20 3229  len(answer) / 2)
-00000970: 5d0d 0a20 2020 2020 2020 2020 2020 2074  ]..            t
-00000980: 6d70 2e61 7070 656e 6428 616e 7377 6572  mp.append(answer
-00000990: 290d 0a20 2020 2072 6571 5f65 6e64 203d  )..    req_end =
-000009a0: 2030 0d0a 2020 2020 666c 6167 203d 207b   0..    flag = {
-000009b0: 226c 6f63 6174 696f 6e22 3a20 302c 2022  "location": 0, "
-000009c0: 7265 7375 6c74 223a 2054 7275 657d 0d0a  result": True}..
-000009d0: 2020 2020 666f 7220 692c 2076 2069 6e20      for i, v in 
-000009e0: 656e 756d 6572 6174 6528 746d 7029 3a0d  enumerate(tmp):.
-000009f0: 0a20 2020 2020 2020 2069 6620 6c65 6e28  .        if len(
-00000a00: 7629 203d 3d20 303a 0d0a 2020 2020 2020  v) == 0:..      
-00000a10: 2020 2020 2020 7265 715f 656e 6420 3d20        req_end = 
-00000a20: 6920 2b20 310d 0a20 2020 2020 2020 2065  i + 1..        e
-00000a30: 6c69 6620 666c 6167 5b22 7265 7375 6c74  lif flag["result
-00000a40: 225d 3a0d 0a20 2020 2020 2020 2020 2020  "]:..           
-00000a50: 2066 6c61 675b 2272 6573 756c 7422 5d20   flag["result"] 
-00000a60: 3d20 4661 6c73 650d 0a20 2020 2020 2020  = False..       
-00000a70: 2020 2020 2066 6c61 675b 226c 6f63 6174       flag["locat
-00000a80: 696f 6e22 5d20 3d20 690d 0a20 2020 2066  ion"] = i..    f
-00000a90: 6f72 2069 2c20 7620 696e 2065 6e75 6d65  or i, v in enume
-00000aa0: 7261 7465 2874 6d70 293a 0d0a 2020 2020  rate(tmp):..    
-00000ab0: 2020 2020 6966 2066 6c61 675b 226c 6f63      if flag["loc
-00000ac0: 6174 696f 6e22 5d20 3c20 7265 715f 656e  ation"] < req_en
-00000ad0: 6420 616e 6420 7265 715f 656e 6420 2d20  d and req_end - 
-00000ae0: 3120 3e20 6920 3e3d 2066 6c61 675b 226c  1 > i >= flag["l
-00000af0: 6f63 6174 696f 6e22 5d3a 0d0a 2020 2020  ocation"]:..    
-00000b00: 2020 2020 2020 2020 6669 656c 6420 3d20          field = 
-00000b10: 2272 6571 7569 7265 6422 0d0a 2020 2020  "required"..    
-00000b20: 2020 2020 2020 2020 616e 7377 6572 5f61          answer_a
-00000b30: 7474 7273 5b66 6965 6c64 5d2e 6170 7065  ttrs[field].appe
-00000b40: 6e64 2876 290d 0a20 2020 2020 2020 2065  nd(v)..        e
-00000b50: 6c69 6620 666c 6167 5b22 6c6f 6361 7469  lif flag["locati
-00000b60: 6f6e 225d 203d 3d20 7265 715f 656e 6420  on"] == req_end 
-00000b70: 616e 6420 6920 3e3d 2072 6571 5f65 6e64  and i >= req_end
-00000b80: 3a0d 0a20 2020 2020 2020 2020 2020 2066  :..            f
-00000b90: 6965 6c64 203d 2022 6f70 7469 6f6e 616c  ield = "optional
-00000ba0: 220d 0a20 2020 2020 2020 2020 2020 2061  "..            a
-00000bb0: 6e73 7765 725f 6174 7472 735b 6669 656c  nswer_attrs[fiel
-00000bc0: 645d 2e61 7070 656e 6428 7629 0d0a 2020  d].append(v)..  
-00000bd0: 2020 2020 2020 656c 6966 2066 6c61 675b        elif flag[
-00000be0: 226c 6f63 6174 696f 6e22 5d20 3c20 7265  "location"] < re
-00000bf0: 715f 656e 6420 3c3d 2069 3a0d 0a20 2020  q_end <= i:..   
-00000c00: 2020 2020 2020 2020 2066 6965 6c64 203d           field =
-00000c10: 2022 6f70 7469 6f6e 616c 220d 0a20 2020   "optional"..   
-00000c20: 2020 2020 2020 2020 2061 6e73 7765 725f           answer_
-00000c30: 6174 7472 735b 6669 656c 645d 2e61 7070  attrs[field].app
-00000c40: 656e 6428 7629 0d0a 2020 2020 6f75 7470  end(v)..    outp
-00000c50: 7574 203d 205b 5d0d 0a20 2020 2069 6620  ut = []..    if 
-00000c60: 6c65 6e28 616e 7377 6572 5f61 7474 7273  len(answer_attrs
-00000c70: 5b22 7265 7175 6972 6564 225d 2920 3e20  ["required"]) > 
-00000c80: 303a 0d0a 2020 2020 2020 2020 6f75 7470  0:..        outp
-00000c90: 7574 2e61 7070 656e 6428 22e6 9cac e69c  ut.append(".....
-00000ca0: 9fe7 ad94 e6a1 885c 6e22 290d 0a20 2020  .......\n")..   
-00000cb0: 2020 2020 2066 6f72 2069 2c20 7620 696e       for i, v in
-00000cc0: 2065 6e75 6d65 7261 7465 2861 6e73 7765   enumerate(answe
-00000cd0: 725f 6174 7472 735b 2272 6571 7569 7265  r_attrs["require
-00000ce0: 6422 5d29 3a0d 0a20 2020 2020 2020 2020  d"]):..         
-00000cf0: 2020 2063 6865 636b 7320 3d20 2222 0d0a     checks = ""..
-00000d00: 2020 2020 2020 2020 2020 2020 666f 7220              for 
-00000d10: 6a2c 2076 3220 696e 2065 6e75 6d65 7261  j, v2 in enumera
-00000d20: 7465 2876 293a 0d0a 2020 2020 2020 2020  te(v):..        
-00000d30: 2020 2020 2020 2020 7472 793a 0d0a 2020          try:..  
-00000d40: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00000d50: 2020 6966 2076 3220 3d3d 2022 3122 3a0d    if v2 == "1":.
-00000d60: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-00000d70: 2020 2020 2020 2020 2063 6865 636b 7320           checks 
-00000d80: 2b3d 206f 7074 696f 6e5b 6a5d 0d0a 2020  += option[j]..  
-00000d90: 2020 2020 2020 2020 2020 2020 2020 6578                ex
-00000da0: 6365 7074 3a0d 0a20 2020 2020 2020 2020  cept:..         
-00000db0: 2020 2020 2020 2020 2020 2070 6173 730d             pass.
-00000dc0: 0a20 2020 2020 2020 2020 2020 206f 7574  .            out
-00000dd0: 7075 742e 6170 7065 6e64 2874 656d 706c  put.append(templ
-00000de0: 6174 652e 666f 726d 6174 286e 756d 3d69  ate.format(num=i
-00000df0: 202b 2031 2c20 6368 6563 6b3d 6368 6563   + 1, check=chec
-00000e00: 6b73 2920 2b20 225c 6e22 290d 0a20 2020  ks) + "\n")..   
-00000e10: 2069 6620 6c65 6e28 616e 7377 6572 5f61   if len(answer_a
-00000e20: 7474 7273 5b22 6f70 7469 6f6e 616c 225d  ttrs["optional"]
-00000e30: 2920 213d 2030 3a0d 0a20 2020 2020 2020  ) != 0:..       
-00000e40: 206f 7574 7075 742e 6170 7065 6e64 2822   output.append("
-00000e50: e8af bee5 a496 e4b9 a0e9 a298 5c6e 2229  ............\n")
-00000e60: 0d0a 2020 2020 2020 2020 666f 7220 692c  ..        for i,
-00000e70: 2076 2069 6e20 656e 756d 6572 6174 6528   v in enumerate(
-00000e80: 616e 7377 6572 5f61 7474 7273 5b22 6f70  answer_attrs["op
-00000e90: 7469 6f6e 616c 225d 293a 0d0a 2020 2020  tional"]):..    
-00000ea0: 2020 2020 2020 2020 6368 6563 6b73 203d          checks =
-00000eb0: 2022 220d 0a20 2020 2020 2020 2020 2020   ""..           
-00000ec0: 2066 6f72 206a 2c20 7632 2069 6e20 656e   for j, v2 in en
-00000ed0: 756d 6572 6174 6528 7629 3a0d 0a20 2020  umerate(v):..   
-00000ee0: 2020 2020 2020 2020 2020 2020 2069 6620               if 
-00000ef0: 7632 203d 3d20 2231 223a 0d0a 2020 2020  v2 == "1":..    
-00000f00: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00000f10: 6368 6563 6b73 202b 3d20 6f70 7469 6f6e  checks += option
-00000f20: 5b6a 5d0d 0a20 2020 2020 2020 2020 2020  [j]..           
-00000f30: 206f 7574 7075 742e 6170 7065 6e64 2874   output.append(t
-00000f40: 656d 706c 6174 652e 666f 726d 6174 286e  emplate.format(n
-00000f50: 756d 3d69 202b 2031 2c20 6368 6563 6b3d  um=i + 1, check=
-00000f60: 6368 6563 6b73 2920 2b20 225c 6e22 290d  checks) + "\n").
-00000f70: 0a20 2020 2072 6573 756c 7420 3d20 5b6f  .    result = [o
-00000f80: 7574 7075 745b 305d 5d0d 0a20 2020 2066  utput[0]]..    f
-00000f90: 6f72 2069 2c20 7620 696e 2065 6e75 6d65  or i, v in enume
-00000fa0: 7261 7465 286f 7574 7075 7429 3a0d 0a20  rate(output):.. 
-00000fb0: 2020 2020 2020 2069 6620 6920 2520 3133         if i % 13
-00000fc0: 2021 3d20 3020 616e 6420 6920 213d 2030   != 0 and i != 0
-00000fd0: 3a0d 0a20 2020 2020 2020 2020 2020 2072  :..            r
-00000fe0: 6573 756c 745b 696e 7428 6920 2f20 3133  esult[int(i / 13
-00000ff0: 295d 202b 3d20 760d 0a20 2020 2020 2020  )] += v..       
-00001000: 2065 6c69 6620 6920 2520 3133 203d 3d20   elif i % 13 == 
-00001010: 3020 616e 6420 6920 213d 2030 3a0d 0a20  0 and i != 0:.. 
-00001020: 2020 2020 2020 2020 2020 2072 6573 756c             resul
-00001030: 742e 6170 7065 6e64 2876 290d 0a20 2020  t.append(v)..   
-00001040: 2074 7279 3a0d 0a20 2020 2020 2020 2065   try:..        e
-00001050: 6e64 5f75 726c 203d 2075 726c 2e72 6570  nd_url = url.rep
-00001060: 6c61 6365 2827 6d2e 6874 6d6c 272c 2027  lace('m.html', '
-00001070: 696d 6167 6573 2f65 6e64 2e6a 7067 2729  images/end.jpg')
-00001080: 0d0a 2020 2020 6578 6365 7074 3a0d 0a20  ..    except:.. 
-00001090: 2020 2020 2020 2065 6e64 5f75 726c 203d         end_url =
-000010a0: 2075 726c 5b3a 2d36 5d20 2b20 2769 6d61   url[:-6] + 'ima
-000010b0: 6765 732f 656e 642e 6a70 6727 0d0a 2020  ges/end.jpg'..  
-000010c0: 2020 7265 7475 726e 207b 0d0a 2020 2020    return {..    
-000010d0: 2020 2020 2265 6e64 5f75 726c 223a 2065      "end_url": e
-000010e0: 6e64 5f75 726c 2c0d 0a20 2020 2020 2020  nd_url,..       
-000010f0: 2022 6361 7461 6c6f 6775 6522 3a20 7469   "catalogue": ti
-00001100: 746c 652c 0d0a 2020 2020 2020 2020 2261  tle,..        "a
-00001110: 6e73 7765 7222 3a20 7265 7375 6c74 5b30  nswer": result[0
-00001120: 5d0d 0a20 2020 207d 0d0a 0d0a 0d0a 6173  ]..    }......as
-00001130: 796e 6320 6465 6620 7570 6461 7465 5f61  ync def update_a
-00001140: 6e73 7765 7228 293a 0d0a 2020 2020 6c6f  nswer():..    lo
-00001150: 6767 6572 2e6f 7074 2863 6f6c 6f72 733d  gger.opt(colors=
-00001160: 5472 7565 292e 696e 666f 2822 3c75 3e3c  True).info("<u><
-00001170: 793e 5be5 a4a7 e5ad a6e4 b9a0 e695 b0e6  y>[.............
-00001180: 8dae e5ba 935d 3c2f 793e 3c2f 753e 3c67  .....]</y></u><g
-00001190: 3ee2 9ea4 e29e a4e2 9ea4 e29e a4e2 9ea4  >...............
-000011a0: e6a3 80e6 9fa5 e7ad 94e6 a188 e695 b0e6  ................
-000011b0: 8dae e29c 94e2 9c94 e29c 94e2 9c94 e29c  ................
-000011c0: 943c 2f67 3e22 290d 0a20 2020 2072 6573  .</g>")..    res
-000011d0: 705f 7572 6c20 3d20 2768 7474 7073 3a2f  p_url = 'https:/
-000011e0: 2f68 352e 6379 6f6c 2e63 6f6d 2f73 7065  /h5.cyol.com/spe
-000011f0: 6369 616c 2f77 6569 7869 6e2f 7369 676e  cial/weixin/sign
-00001200: 2e6a 736f 6e27 0d0a 2020 2020 6173 796e  .json'..    asyn
-00001210: 6320 7769 7468 2041 7379 6e63 436c 6965  c with AsyncClie
-00001220: 6e74 2868 6561 6465 7273 3d68 6561 6465  nt(headers=heade
-00001230: 7273 2920 6173 2063 6c69 656e 743a 0d0a  rs) as client:..
-00001240: 2020 2020 2020 2020 7265 7370 6f6e 7365          response
-00001250: 203d 2061 7761 6974 2063 6c69 656e 742e   = await client.
-00001260: 6765 7428 7572 6c3d 7265 7370 5f75 726c  get(url=resp_url
-00001270: 2c20 7469 6d65 6f75 743d 3130 290d 0a20  , timeout=10).. 
-00001280: 2020 2072 6573 706f 6e73 652e 656e 636f     response.enco
-00001290: 6469 6e67 203d 2072 6573 706f 6e73 652e  ding = response.
-000012a0: 6368 6172 7365 745f 656e 636f 6469 6e67  charset_encoding
-000012b0: 0d0a 2020 2020 7265 7375 6c74 203d 206a  ..    result = j
-000012c0: 736f 6e2e 6c6f 6164 7328 7265 7370 6f6e  son.loads(respon
-000012d0: 7365 2e74 6578 7429 0d0a 2020 2020 636f  se.text)..    co
-000012e0: 6465 5f72 6573 756c 7420 3d20 6c69 7374  de_result = list
-000012f0: 2872 6573 756c 7429 5b2d 3130 3a5d 0d0a  (result)[-10:]..
-00001300: 2020 2020 666f 7220 636f 6465 2069 6e20      for code in 
-00001310: 636f 6465 5f72 6573 756c 743a 0d0a 2020  code_result:..  
-00001320: 2020 2020 2020 6966 2061 7761 6974 2041        if await A
-00001330: 6e73 7765 722e 6669 6c74 6572 2863 6f64  nswer.filter(cod
-00001340: 653d 636f 6465 292e 636f 756e 7428 293a  e=code).count():
-00001350: 0d0a 2020 2020 2020 2020 2020 2020 636f  ..            co
-00001360: 6e74 696e 7565 0d0a 2020 2020 2020 2020  ntinue..        
-00001370: 656c 7365 3a0d 0a20 2020 2020 2020 2020  else:..         
-00001380: 2020 2074 7279 3a0d 0a20 2020 2020 2020     try:..       
-00001390: 2020 2020 2020 2020 2075 726c 203d 2072           url = r
-000013a0: 6573 756c 745b 636f 6465 5d5b 2275 726c  esult[code]["url
-000013b0: 225d 0d0a 2020 2020 2020 2020 2020 2020  "]..            
-000013c0: 2020 2020 6461 7461 203d 2061 7761 6974      data = await
-000013d0: 2063 7261 776c 5f61 6e73 7765 7228 7572   crawl_answer(ur
-000013e0: 6c3d 7572 6c29 0d0a 2020 2020 2020 2020  l=url)..        
-000013f0: 2020 2020 2020 2020 656e 645f 7572 6c20          end_url 
-00001400: 3d20 6461 7461 5b22 656e 645f 7572 6c22  = data["end_url"
-00001410: 5d0d 0a20 2020 2020 2020 2020 2020 2020  ]..             
-00001420: 2020 2061 6e73 7765 7220 3d20 6461 7461     answer = data
-00001430: 5b22 616e 7377 6572 225d 0d0a 2020 2020  ["answer"]..    
-00001440: 2020 2020 2020 2020 2020 2020 6361 7461              cata
-00001450: 6c6f 6775 6520 3d20 6461 7461 5b22 6361  logue = data["ca
-00001460: 7461 6c6f 6775 6522 5d0d 0a20 2020 2020  talogue"]..     
-00001470: 2020 2020 2020 2020 2020 2061 7379 6e63             async
-00001480: 2077 6974 6820 4173 796e 6343 6c69 656e   with AsyncClien
-00001490: 7428 6865 6164 6572 733d 6865 6164 6572  t(headers=header
-000014a0: 7329 2061 7320 636c 6965 6e74 3a0d 0a20  s) as client:.. 
-000014b0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000014c0: 2020 2065 6e64 5f6a 7067 203d 2061 7761     end_jpg = awa
-000014d0: 6974 2063 6c69 656e 742e 6765 7428 656e  it client.get(en
-000014e0: 645f 7572 6c2c 2074 696d 656f 7574 3d31  d_url, timeout=1
-000014f0: 3029 0d0a 2020 2020 2020 2020 2020 2020  0)..            
-00001500: 2020 2020 636f 7665 7220 3d20 656e 645f      cover = end_
-00001510: 6a70 672e 636f 6e74 656e 740d 0a20 2020  jpg.content..   
-00001520: 2020 2020 2020 2020 2020 2020 2061 7761               awa
-00001530: 6974 2041 6e73 7765 722e 6372 6561 7465  it Answer.create
-00001540: 280d 0a20 2020 2020 2020 2020 2020 2020  (..             
-00001550: 2020 2020 2020 2074 696d 653d 7469 6d65         time=time
-00001560: 2e74 696d 6528 292c 0d0a 2020 2020 2020  .time(),..      
-00001570: 2020 2020 2020 2020 2020 2020 2020 636f                co
-00001580: 6465 3d63 6f64 652c 0d0a 2020 2020 2020  de=code,..      
-00001590: 2020 2020 2020 2020 2020 2020 2020 6361                ca
-000015a0: 7461 6c6f 6775 653d 6361 7461 6c6f 6775  talogue=catalogu
-000015b0: 652c 0d0a 2020 2020 2020 2020 2020 2020  e,..            
-000015c0: 2020 2020 2020 2020 7572 6c3d 7572 6c2c          url=url,
-000015d0: 0d0a 2020 2020 2020 2020 2020 2020 2020  ..              
-000015e0: 2020 2020 2020 656e 645f 7572 6c3d 656e        end_url=en
-000015f0: 645f 7572 6c2c 0d0a 2020 2020 2020 2020  d_url,..        
-00001600: 2020 2020 2020 2020 2020 2020 616e 7377              answ
-00001610: 6572 3d61 6e73 7765 722c 0d0a 2020 2020  er=answer,..    
-00001620: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00001630: 636f 7665 723d 636f 7665 720d 0a20 2020  cover=cover..   
-00001640: 2020 2020 2020 2020 2020 2020 2029 0d0a               )..
-00001650: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00001660: 6c6f 6767 6572 2e6f 7074 2863 6f6c 6f72  logger.opt(color
-00001670: 733d 5472 7565 292e 7375 6363 6573 7328  s=True).success(
-00001680: 6622 3c75 3e3c 793e e99d 92e5 b9b4 e5a4  f"<u><y>........
-00001690: a7e5 ada6 e4b9 a03c 2f79 3e3c 2f75 3e20  .......</y></u> 
-000016a0: 3c6d 3e7b 6361 7461 6c6f 6775 657d 3c2f  <m>{catalogue}</
-000016b0: 6d3e 203c 673e e69b b4e6 96b0 e688 90e5  m> <g>..........
-000016c0: 8a9f 213c 2f67 3e22 290d 0a20 2020 2020  ..!</g>")..     
-000016d0: 2020 2020 2020 2065 7863 6570 7420 4578         except Ex
-000016e0: 6365 7074 696f 6e20 6173 2065 3a0d 0a20  ception as e:.. 
-000016f0: 2020 2020 2020 2020 2020 2020 2020 206c                 l
-00001700: 6f67 6765 722e 6572 726f 7228 6529 0d0a  ogger.error(e)..
-00001710: 2020 2020 6c6f 6767 6572 2e6f 7074 2863      logger.opt(c
-00001720: 6f6c 6f72 733d 5472 7565 292e 7375 6363  olors=True).succ
-00001730: 6573 7328 223c 753e 3c79 3e5b e5a4 a7e5  ess("<u><y>[....
-00001740: ada6 e4b9 a0e6 95b0 e68d aee5 ba93 5d3c  ..............]<
-00001750: 2f79 3e3c 2f75 3e3c 673e e29e a4e2 9ea4  /y></u><g>......
-00001760: e29e a4e2 9ea4 e29e a4e7 ad94 e6a1 88e6  ................
-00001770: 95b0 e68d aee6 9bb4 e696 b0e5 ae8c e688  ................
-00001780: 90e2 9c94 e29c 94e2 9c94 e29c 94e2 9c94  ................
-00001790: 3c2f 673e 2229 0d0a 0d0a 0d0a 4073 6368  </g>")......@sch
-000017a0: 6564 756c 6572 2e73 6368 6564 756c 6564  eduler.scheduled
-000017b0: 5f6a 6f62 2827 6372 6f6e 272c 2064 6179  _job('cron', day
-000017c0: 5f6f 665f 7765 656b 3d27 3627 2c20 686f  _of_week='6', ho
-000017d0: 7572 3d22 3231 2d32 3322 2c20 6d69 6e75  ur="21-23", minu
-000017e0: 7465 3d22 2a2f 3135 222c 2069 643d 2775  te="*/15", id='u
-000017f0: 7064 6174 655f 6461 7461 272c 0d0a 2020  pdate_data',..  
-00001800: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00001810: 2020 2020 2020 2074 696d 657a 6f6e 653d         timezone=
-00001820: 2241 7369 612f 5368 616e 6768 6169 2229  "Asia/Shanghai")
-00001830: 0d0a 6173 796e 6320 6465 6620 7570 6461  ..async def upda
-00001840: 7465 5f64 6174 6128 293a 0d0a 2020 2020  te_data():..    
-00001850: 7472 793a 0d0a 2020 2020 2020 2020 626f  try:..        bo
-00001860: 743a 2042 6f74 203d 2067 6574 5f62 6f74  t: Bot = get_bot
-00001870: 2829 0d0a 2020 2020 6578 6365 7074 2056  ()..    except V
-00001880: 616c 7565 4572 726f 7220 6173 2065 3a0d  alueError as e:.
-00001890: 0a20 2020 2020 2020 2072 6574 7572 6e0d  .        return.
-000018a0: 0a20 2020 2072 6573 705f 7572 6c20 3d20  .    resp_url = 
-000018b0: 2768 7474 7073 3a2f 2f68 352e 6379 6f6c  'https://h5.cyol
-000018c0: 2e63 6f6d 2f73 7065 6369 616c 2f77 6569  .com/special/wei
-000018d0: 7869 6e2f 7369 676e 2e6a 736f 6e27 0d0a  xin/sign.json'..
-000018e0: 2020 2020 6173 796e 6320 7769 7468 2041      async with A
-000018f0: 7379 6e63 436c 6965 6e74 2868 6561 6465  syncClient(heade
-00001900: 7273 3d68 6561 6465 7273 2920 6173 2063  rs=headers) as c
-00001910: 6c69 656e 743a 0d0a 2020 2020 2020 2020  lient:..        
-00001920: 7265 7370 6f6e 7365 203d 2061 7761 6974  response = await
-00001930: 2063 6c69 656e 742e 6765 7428 7572 6c3d   client.get(url=
-00001940: 7265 7370 5f75 726c 2c20 7469 6d65 6f75  resp_url, timeou
-00001950: 743d 3130 290d 0a20 2020 2072 6573 706f  t=10)..    respo
-00001960: 6e73 652e 656e 636f 6469 6e67 203d 2072  nse.encoding = r
-00001970: 6573 706f 6e73 652e 6368 6172 7365 745f  esponse.charset_
-00001980: 656e 636f 6469 6e67 0d0a 2020 2020 7265  encoding..    re
-00001990: 7375 6c74 203d 206a 736f 6e2e 6c6f 6164  sult = json.load
-000019a0: 7328 7265 7370 6f6e 7365 2e74 6578 7429  s(response.text)
-000019b0: 0d0a 2020 2020 636f 6465 5f72 6573 756c  ..    code_resul
-000019c0: 7420 3d20 6c69 7374 2872 6573 756c 7429  t = list(result)
-000019d0: 5b2d 3130 3a5d 0d0a 2020 2020 666f 7220  [-10:]..    for 
-000019e0: 636f 6465 2069 6e20 636f 6465 5f72 6573  code in code_res
-000019f0: 756c 743a 0d0a 2020 2020 2020 2020 6966  ult:..        if
-00001a00: 2061 7761 6974 2041 6e73 7765 722e 6669   await Answer.fi
-00001a10: 6c74 6572 2863 6f64 653d 636f 6465 292e  lter(code=code).
-00001a20: 636f 756e 7428 293a 0d0a 2020 2020 2020  count():..      
-00001a30: 2020 2020 2020 636f 6e74 696e 7565 0d0a        continue..
-00001a40: 2020 2020 2020 2020 656c 7365 3a0d 0a20          else:.. 
-00001a50: 2020 2020 2020 2020 2020 2074 7279 3a0d             try:.
-00001a60: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-00001a70: 2075 726c 203d 2072 6573 756c 745b 636f   url = result[co
-00001a80: 6465 5d5b 2275 726c 225d 0d0a 2020 2020  de]["url"]..    
-00001a90: 2020 2020 2020 2020 2020 2020 6461 7461              data
-00001aa0: 203d 2061 7761 6974 2063 7261 776c 5f61   = await crawl_a
-00001ab0: 6e73 7765 7228 7572 6c3d 7572 6c29 0d0a  nswer(url=url)..
-00001ac0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00001ad0: 656e 645f 7572 6c20 3d20 6461 7461 5b22  end_url = data["
-00001ae0: 656e 645f 7572 6c22 5d0d 0a20 2020 2020  end_url"]..     
-00001af0: 2020 2020 2020 2020 2020 2061 6e73 7765             answe
-00001b00: 7220 3d20 6461 7461 5b22 616e 7377 6572  r = data["answer
-00001b10: 225d 0d0a 2020 2020 2020 2020 2020 2020  "]..            
-00001b20: 2020 2020 6361 7461 6c6f 6775 6520 3d20      catalogue = 
-00001b30: 6461 7461 5b22 6361 7461 6c6f 6775 6522  data["catalogue"
-00001b40: 5d0d 0a20 2020 2020 2020 2020 2020 2020  ]..             
-00001b50: 2020 2061 7379 6e63 2077 6974 6820 4173     async with As
-00001b60: 796e 6343 6c69 656e 7428 6865 6164 6572  yncClient(header
-00001b70: 733d 6865 6164 6572 7329 2061 7320 636c  s=headers) as cl
-00001b80: 6965 6e74 3a0d 0a20 2020 2020 2020 2020  ient:..         
-00001b90: 2020 2020 2020 2020 2020 2065 6e64 5f6a             end_j
-00001ba0: 7067 203d 2061 7761 6974 2063 6c69 656e  pg = await clien
-00001bb0: 742e 6765 7428 656e 645f 7572 6c2c 2074  t.get(end_url, t
-00001bc0: 696d 656f 7574 3d31 3029 0d0a 2020 2020  imeout=10)..    
-00001bd0: 2020 2020 2020 2020 2020 2020 636f 7665              cove
-00001be0: 7220 3d20 656e 645f 6a70 672e 636f 6e74  r = end_jpg.cont
-00001bf0: 656e 740d 0a20 2020 2020 2020 2020 2020  ent..           
-00001c00: 2020 2020 2061 7761 6974 2041 6e73 7765       await Answe
-00001c10: 722e 6372 6561 7465 280d 0a20 2020 2020  r.create(..     
-00001c20: 2020 2020 2020 2020 2020 2020 2020 2074                 t
-00001c30: 696d 653d 7469 6d65 2e74 696d 6528 292c  ime=time.time(),
-00001c40: 0d0a 2020 2020 2020 2020 2020 2020 2020  ..              
-00001c50: 2020 2020 2020 636f 6465 3d63 6f64 652c        code=code,
-00001c60: 0d0a 2020 2020 2020 2020 2020 2020 2020  ..              
-00001c70: 2020 2020 2020 6361 7461 6c6f 6775 653d        catalogue=
-00001c80: 6361 7461 6c6f 6775 652c 0d0a 2020 2020  catalogue,..    
-00001c90: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00001ca0: 7572 6c3d 7572 6c2c 0d0a 2020 2020 2020  url=url,..      
-00001cb0: 2020 2020 2020 2020 2020 2020 2020 656e                en
-00001cc0: 645f 7572 6c3d 656e 645f 7572 6c2c 0d0a  d_url=end_url,..
-00001cd0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00001ce0: 2020 2020 616e 7377 6572 3d61 6e73 7765      answer=answe
-00001cf0: 722c 0d0a 2020 2020 2020 2020 2020 2020  r,..            
-00001d00: 2020 2020 2020 2020 636f 7665 723d 636f          cover=co
-00001d10: 7665 720d 0a20 2020 2020 2020 2020 2020  ver..           
-00001d20: 2020 2020 2029 0d0a 2020 2020 2020 2020       )..        
-00001d30: 2020 2020 2020 2020 6c6f 6767 6572 2e6f          logger.o
-00001d40: 7074 2863 6f6c 6f72 733d 5472 7565 292e  pt(colors=True).
-00001d50: 7375 6363 6573 7328 6622 3c75 3e3c 793e  success(f"<u><y>
-00001d60: e99d 92e5 b9b4 e5a4 a7e5 ada6 e4b9 a03c  ...............<
-00001d70: 2f79 3e3c 2f75 3e20 3c6d 3e7b 6361 7461  /y></u> <m>{cata
-00001d80: 6c6f 6775 657d 3c2f 6d3e 203c 673e e69b  logue}</m> <g>..
-00001d90: b4e6 96b0 e688 90e5 8a9f 213c 2f67 3e22  ..........!</g>"
-00001da0: 290d 0a20 2020 2020 2020 2020 2020 2020  )..             
-00001db0: 2020 2061 646d 696e 203d 2067 6574 436f     admin = getCo
-00001dc0: 6e66 6967 2829 0d0a 2020 2020 2020 2020  nfig()..        
-00001dd0: 2020 2020 2020 2020 636f 6e74 656e 7420          content 
-00001de0: 3d20 6177 6169 7420 6765 745f 6c6f 6769  = await get_logi
-00001df0: 6e5f 7172 636f 6465 2829 0d0a 2020 2020  n_qrcode()..    
-00001e00: 2020 2020 2020 2020 2020 2020 6966 2061              if a
-00001e10: 646d 696e 5b22 5552 4c5f 5354 4154 5553  dmin["URL_STATUS
-00001e20: 225d 3a0d 0a20 2020 2020 2020 2020 2020  "]:..           
-00001e30: 2020 2020 2020 2020 2061 7761 6974 2062           await b
-00001e40: 6f74 2e73 656e 645f 7072 6976 6174 655f  ot.send_private_
-00001e50: 6d73 6728 7573 6572 5f69 643d 6164 6d69  msg(user_id=admi
-00001e60: 6e5b 2253 5550 4552 5553 4552 225d 2c20  n["SUPERUSER"], 
-00001e70: 6d65 7373 6167 653d 4d65 7373 6167 6553  message=MessageS
-00001e80: 6567 6d65 6e74 2e74 6578 7428 0d0a 2020  egment.text(..  
-00001e90: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00001ea0: 2020 2020 2020 6622 e6a3 80e6 b58b e588        f"........
-00001eb0: b0e9 9d92 e5b9 b4e5 a4a7 e5ad a6e4 b9a0  ................
-00001ec0: e69c 89e6 9bb4 e696 b0ef bc8c e4b8 8be5  ................
-00001ed0: 91a8 e4b8 80e4 b8ba 7b63 6174 616c 6f67  ........{catalog
-00001ee0: 7565 7d2c e8af a6e7 bb86 e4bf a1e6 81af  ue},............
-00001ef0: e8af b7e7 82b9 e587 bbe9 93be e68e a5e7  ................
-00001f00: 99bb e5bd 95e5 908e e58f b0e6 9fa5 e79c  ................
-00001f10: 8bef bc8c e5a6 82e6 8993 e4b8 8de5 bc80  ................
-00001f20: e993 bee6 8ea5 efbc 8ce8 afb7 e5a4 8de5  ................
-00001f30: 88b6 e993 bee6 8ea5 e588 b0e6 b58f e8a7  ................
-00001f40: 88e5 99a8 6428 c2b4 cf89 efbd 802a 295c  ....d(.......*)\
-00001f50: 6e22 2920 2b20 4d65 7373 6167 6553 6567  n") + MessageSeg
-00001f60: 6d65 6e74 2e74 6578 7428 0d0a 2020 2020  ment.text(..    
-00001f70: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00001f80: 2020 2020 636f 6e74 656e 745b 2275 726c      content["url
-00001f90: 225d 2929 0d0a 2020 2020 2020 2020 2020  "]))..          
-00001fa0: 2020 2020 2020 6177 6169 7420 626f 742e        await bot.
-00001fb0: 7365 6e64 5f70 7269 7661 7465 5f6d 7367  send_private_msg
-00001fc0: 2875 7365 725f 6964 3d61 646d 696e 5b22  (user_id=admin["
-00001fd0: 5355 5045 5255 5345 5222 5d2c 206d 6573  SUPERUSER"], mes
-00001fe0: 7361 6765 3d4d 6573 7361 6765 5365 676d  sage=MessageSegm
-00001ff0: 656e 742e 7465 7874 280d 0a20 2020 2020  ent.text(..     
-00002000: 2020 2020 2020 2020 2020 2020 2020 2066                 f
-00002010: 22e6 a380 e6b5 8be5 88b0 e99d 92e5 b9b4  "...............
-00002020: e5a4 a7e5 ada6 e4b9 a0e6 9c89 e69b b4e6  ................
-00002030: 96b0 efbc 8ce4 b88b e591 a8e4 b880 e4b8  ................
-00002040: ba7b 6361 7461 6c6f 6775 657d 2ce8 afa6  .{catalogue},...
-00002050: e7bb 86e4 bfa1 e681 afe8 afb7 e689 abe7  ................
-00002060: a081 e799 bbe5 bd95 e590 8ee5 8fb0 e69f  ................
-00002070: a5e7 9c8b 6428 c2b4 cf89 efbd 802a 2922  ....d(.......*)"
-00002080: 2920 2b20 4d65 7373 6167 6553 6567 6d65  ) + MessageSegme
-00002090: 6e74 2e69 6d61 6765 280d 0a20 2020 2020  nt.image(..     
-000020a0: 2020 2020 2020 2020 2020 2020 2020 2063                 c
-000020b0: 6f6e 7465 6e74 5b22 636f 6e74 656e 7422  ontent["content"
-000020c0: 5d29 290d 0a20 2020 2020 2020 2020 2020  ]))..           
-000020d0: 2065 7863 6570 7420 4578 6365 7074 696f   except Exceptio
-000020e0: 6e20 6173 2065 3a0d 0a20 2020 2020 2020  n as e:..       
-000020f0: 2020 2020 2020 2020 206c 6f67 6765 722e           logger.
-00002100: 6572 726f 7228 6529 0d0a 0d0a 0d0a 4073  error(e)......@s
-00002110: 6368 6564 756c 6572 2e73 6368 6564 756c  cheduler.schedul
-00002120: 6564 5f6a 6f62 2827 6372 6f6e 272c 2073  ed_job('cron', s
-00002130: 6563 6f6e 643d 272a 2f31 3527 2c20 6d69  econd='*/15', mi
-00002140: 7366 6972 655f 6772 6163 655f 7469 6d65  sfire_grace_time
-00002150: 3d31 3029 0d0a 6173 796e 6320 6465 6620  =10)..async def 
-00002160: 6368 6563 6b5f 6170 706c 7928 293a 0d0a  check_apply():..
-00002170: 2020 2020 7472 793a 0d0a 2020 2020 2020      try:..      
-00002180: 2020 626f 743a 2042 6f74 203d 2067 6574    bot: Bot = get
-00002190: 5f62 6f74 2829 0d0a 2020 2020 6578 6365  _bot()..    exce
-000021a0: 7074 2056 616c 7565 4572 726f 7220 6173  pt ValueError as
-000021b0: 2065 3a0d 0a20 2020 2020 2020 2072 6574   e:..        ret
-000021c0: 7572 6e0d 0a20 2020 2061 7070 6c79 5f6c  urn..    apply_l
-000021d0: 6973 7420 3d20 6177 6169 7420 4164 6455  ist = await AddU
-000021e0: 7365 722e 6669 6c74 6572 2873 7461 7475  ser.filter(statu
-000021f0: 733d 22e6 9caa e980 9ae8 bf87 2229 2e76  s=".........").v
-00002200: 616c 7565 7328 290d 0a0d 0a20 2020 2066  alues()....    f
-00002210: 6f72 2069 7465 6d20 696e 2061 7070 6c79  or item in apply
-00002220: 5f6c 6973 743a 0d0a 2020 2020 2020 2020  _list:..        
-00002230: 7265 7375 6c74 203d 2061 7761 6974 2055  result = await U
-00002240: 7365 722e 6669 6c74 6572 2875 7365 725f  ser.filter(user_
-00002250: 6964 3d69 7465 6d5b 2275 7365 725f 6964  id=item["user_id
-00002260: 225d 2c20 6772 6f75 705f 6964 3d69 7465  "], group_id=ite
-00002270: 6d5b 2267 726f 7570 5f69 6422 5d29 2e63  m["group_id"]).c
-00002280: 6f75 6e74 2829 0d0a 2020 2020 2020 2020  ount()..        
-00002290: 6966 2072 6573 756c 743a 0d0a 2020 2020  if result:..    
-000022a0: 2020 2020 2020 2020 6177 6169 7420 4164          await Ad
-000022b0: 6455 7365 722e 6669 6c74 6572 2869 643d  dUser.filter(id=
-000022c0: 6974 656d 5b22 6964 225d 292e 7570 6461  item["id"]).upda
-000022d0: 7465 2873 7461 7475 733d 22e5 b7b2 e980  te(status=".....
-000022e0: 9ae8 bf87 2229 0d0a 2020 2020 2020 2020  ....")..        
-000022f0: 2020 2020 6177 6169 7420 626f 742e 7365      await bot.se
-00002300: 6e64 5f67 726f 7570 5f6d 7367 2867 726f  nd_group_msg(gro
-00002310: 7570 5f69 643d 6974 656d 5b22 6772 6f75  up_id=item["grou
-00002320: 705f 6964 225d 2c0d 0a20 2020 2020 2020  p_id"],..       
-00002330: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00002340: 2020 2020 2020 2020 2020 2020 2020 6d65                me
-00002350: 7373 6167 653d 4d65 7373 6167 6553 6567  ssage=MessageSeg
-00002360: 6d65 6e74 2e61 7428 7573 6572 5f69 643d  ment.at(user_id=
-00002370: 6974 656d 5b22 7573 6572 5f69 6422 5d29  item["user_id"])
-00002380: 202b 204d 6573 7361 6765 5365 676d 656e   + MessageSegmen
-00002390: 742e 7465 7874 280d 0a20 2020 2020 2020  t.text(..       
-000023a0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000023b0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000023c0: 2020 22e4 bfa1 e681 afe7 bb91 e5ae 9ae6    ".............
-000023d0: 8890 e58a 9f28 20e2 80a2 20cc 80cf 89e2  .....( ... .....
-000023e0: 80a2 cc81 2029 e29c a722 2929 0d0a 2020  .... )..."))..  
-000023f0: 2020 2020 2020 2020 2020 6177 6169 7420            await 
-00002400: 6173 796e 6369 6f2e 736c 6565 7028 3229  asyncio.sleep(2)
-00002410: 0d0a 2020 2020 2020 2020 2020 2020 636f  ..            co
-00002420: 6e74 696e 7565 0d0a 2020 2020 2020 2020  ntinue..        
-00002430: 6e6f 775f 7469 6d65 203d 2069 6e74 2874  now_time = int(t
-00002440: 696d 652e 7469 6d65 2829 290d 0a20 2020  ime.time())..   
-00002450: 2020 2020 2069 6620 286e 6f77 5f74 696d       if (now_tim
-00002460: 6520 2d20 6974 656d 5b22 7469 6d65 225d  e - item["time"]
-00002470: 2920 3e20 3138 303a 0d0a 2020 2020 2020  ) > 180:..      
-00002480: 2020 2020 2020 6177 6169 7420 4164 6455        await AddU
-00002490: 7365 722e 6669 6c74 6572 2869 643d 6974  ser.filter(id=it
-000024a0: 656d 5b22 6964 225d 292e 7570 6461 7465  em["id"]).update
-000024b0: 2873 7461 7475 733d 22e5 b7b2 e8bf 87e6  (status=".......
-000024c0: 9c9f 2229 0d0a 2020 2020 2020 2020 2020  ..")..          
-000024d0: 2020 6177 6169 7420 626f 742e 7365 6e64    await bot.send
-000024e0: 5f67 726f 7570 5f6d 7367 2867 726f 7570  _group_msg(group
-000024f0: 5f69 643d 6974 656d 5b22 6772 6f75 705f  _id=item["group_
-00002500: 6964 225d 2c0d 0a20 2020 2020 2020 2020  id"],..         
-00002510: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00002520: 2020 2020 2020 2020 2020 2020 6d65 7373              mess
-00002530: 6167 653d 4d65 7373 6167 6553 6567 6d65  age=MessageSegme
-00002540: 6e74 2e61 7428 7573 6572 5f69 643d 6974  nt.at(user_id=it
-00002550: 656d 5b22 7573 6572 5f69 6422 5d29 202b  em["user_id"]) +
-00002560: 204d 6573 7361 6765 5365 676d 656e 742e   MessageSegment.
-00002570: 7465 7874 280d 0a20 2020 2020 2020 2020  text(..         
-00002580: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00002590: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000025a0: 22e6 b7bb e58a a0e7 94b3 e8af b7e5 b7b2  "...............
-000025b0: e8bf 87e6 9c9f efbc 8ce8 afb7 e987 8de6  ................
-000025c0: 96b0 e58f 9120 e6b7 bbe5 8aa0 e5a4 a7e5  ..... ..........
-000025d0: ada6 e4b9 a020 e68c 87e4 bba4 e8bf 9be8  ..... ..........
-000025e0: a18c e794 b3e8 afb7 2820 e280 a220 cc80  ........( ... ..
-000025f0: cf89 e280 a2cc 8120 29e2 9ca7 2229 290d  ....... )...")).
-00002600: 0a20 2020 2020 2020 2020 2020 2061 7761  .            awa
-00002610: 6974 2061 7379 6e63 696f 2e73 6c65 6570  it asyncio.sleep
-00002620: 2832 290d 0a20 2020 2020 2020 2065 6c73  (2)..        els
-00002630: 653a 0d0a 2020 2020 2020 2020 2020 2020  e:..            
-00002640: 636f 6e74 696e 7565 0d0a 0d0a 0d0a 4073  continue......@s
-00002650: 6368 6564 756c 6572 2e73 6368 6564 756c  cheduler.schedul
-00002660: 6564 5f6a 6f62 2827 6372 6f6e 272c 2064  ed_job('cron', d
-00002670: 6179 5f6f 665f 7765 656b 3d27 3027 2c20  ay_of_week='0', 
-00002680: 686f 7572 3d27 3027 2c20 6d69 6e75 7465  hour='0', minute
-00002690: 3d27 3027 2c20 6964 3d27 636c 6561 7227  ='0', id='clear'
-000026a0: 2c20 7469 6d65 7a6f 6e65 3d22 4173 6961  , timezone="Asia
-000026b0: 2f53 6861 6e67 6861 6922 290d 0a61 7379  /Shanghai")..asy
-000026c0: 6e63 2064 6566 2063 6c65 6172 2829 3a0d  nc def clear():.
-000026d0: 0a20 2020 2074 7279 3a0d 0a20 2020 2020  .    try:..     
-000026e0: 2020 2072 6573 756c 7420 3d20 6177 6169     result = awai
-000026f0: 7420 4172 6561 2e61 6c6c 2829 2e76 616c  t Area.all().val
-00002700: 7565 7328 290d 0a20 2020 2020 2020 2066  ues()..        f
-00002710: 6f72 2069 7465 6d20 696e 2072 6573 756c  or item in resul
-00002720: 743a 0d0a 2020 2020 2020 2020 2020 2020  t:..            
-00002730: 6177 6169 7420 4172 6561 2e66 696c 7465  await Area.filte
-00002740: 7228 6964 3d69 7465 6d5b 2269 6422 5d29  r(id=item["id"])
-00002750: 2e75 7064 6174 6528 7374 6174 7573 3d46  .update(status=F
-00002760: 616c 7365 290d 0a20 2020 2020 2020 206c  alse)..        l
-00002770: 6f67 6765 722e 6f70 7428 636f 6c6f 7273  ogger.opt(colors
-00002780: 3d54 7275 6529 2e73 7563 6365 7373 280d  =True).success(.
-00002790: 0a20 2020 2020 2020 2020 2020 2066 223c  .            f"<
-000027a0: 753e 3c79 3e5b e5a4 a7e5 ada6 e4b9 a0e6  u><y>[..........
-000027b0: 95b0 e68d aee5 ba93 5d3c 2f79 3e3c 2f75  ........]</y></u
-000027c0: 3e20 3c6d 3ee5 9cb0 e58c bae6 9c80 e696  > <m>...........
-000027d0: b0e4 b880 e69c 9fe7 8ab6 e680 813c 2f6d  .............</m
-000027e0: 3e20 3c67 3ee9 878d e7bd aee6 8890 e58a  > <g>...........
-000027f0: 9f21 3c2f 673e 2229 0d0a 2020 2020 6578  .!</g>")..    ex
-00002800: 6365 7074 2045 7863 6570 7469 6f6e 2061  cept Exception a
-00002810: 7320 653a 0d0a 2020 2020 2020 2020 6c6f  s e:..        lo
-00002820: 6767 6572 2e6f 7074 2863 6f6c 6f72 733d  gger.opt(colors=
-00002830: 5472 7565 292e 6572 726f 7228 0d0a 2020  True).error(..  
-00002840: 2020 2020 2020 2020 2020 6622 3c75 3e3c            f"<u><
-00002850: 793e 5be5 a4a7 e5ad a6e4 b9a0 e695 b0e6  y>[.............
-00002860: 8dae e5ba 935d 3c2f 793e 3c2f 753e 203c  .....]</y></u> <
-00002870: 6d3e e59c b0e5 8cba e69c 80e6 96b0 e4b8  m>..............
-00002880: 80e6 9c9f e78a b6e6 8081 3c2f 6d3e 203c  ..........</m> <
-00002890: 72e9 878d e7bd aee5 a4b1 e8b4 a5ef bc9a  r...............
-000028a0: 7b65 7d3c 2f72 3e22 290d 0a              {e}</r>")..
+00000000: 696d 706f 7274 2061 7379 6e63 696f 0a69  import asyncio.i
+00000010: 6d70 6f72 7420 6a73 6f6e 0a69 6d70 6f72  mport json.impor
+00000020: 7420 7469 6d65 0a0a 6672 6f6d 2062 7334  t time..from bs4
+00000030: 2069 6d70 6f72 7420 4265 6175 7469 6675   import Beautifu
+00000040: 6c53 6f75 700a 6672 6f6d 2068 7474 7078  lSoup.from httpx
+00000050: 2069 6d70 6f72 7420 4173 796e 6343 6c69   import AsyncCli
+00000060: 656e 740a 6672 6f6d 206e 6f6e 6562 6f74  ent.from nonebot
+00000070: 2069 6d70 6f72 7420 6c6f 6767 6572 2c20   import logger, 
+00000080: 7265 7175 6972 652c 2067 6574 5f62 6f74  require, get_bot
+00000090: 2c20 6765 745f 6472 6976 6572 0a66 726f  , get_driver.fro
+000000a0: 6d20 6e6f 6e65 626f 742e 6164 6170 7465  m nonebot.adapte
+000000b0: 7273 2e6f 6e65 626f 742e 7631 3120 696d  rs.onebot.v11 im
+000000c0: 706f 7274 2042 6f74 2c20 4d65 7373 6167  port Bot, Messag
+000000d0: 6553 6567 6d65 6e74 0a0a 6672 6f6d 202e  eSegment..from .
+000000e0: 7061 7468 2069 6d70 6f72 7420 6765 7443  path import getC
+000000f0: 6f6e 6669 670a 6672 6f6d 202e 7574 696c  onfig.from .util
+00000100: 7320 696d 706f 7274 2067 6574 5f6c 6f67  s import get_log
+00000110: 696e 5f71 7263 6f64 650a 6672 6f6d 202e  in_qrcode.from .
+00000120: 2e6d 6f64 656c 732e 6163 6375 6f6e 7420  .models.accuont 
+00000130: 696d 706f 7274 2041 6464 5573 6572 2c20  import AddUser, 
+00000140: 5573 6572 0a66 726f 6d20 2e2e 6d6f 6465  User.from ..mode
+00000150: 6c73 2e64 7878 2069 6d70 6f72 7420 416e  ls.dxx import An
+00000160: 7377 6572 2c20 4172 6561 0a0a 7363 6865  swer, Area..sche
+00000170: 6475 6c65 7220 3d20 7265 7175 6972 6528  duler = require(
+00000180: 276e 6f6e 6562 6f74 5f70 6c75 6769 6e5f  'nonebot_plugin_
+00000190: 6170 7363 6865 6475 6c65 7227 292e 7363  apscheduler').sc
+000001a0: 6865 6475 6c65 720a 7375 7065 725f 6964  heduler.super_id
+000001b0: 203d 2067 6574 5f64 7269 7665 7228 292e   = get_driver().
+000001c0: 636f 6e66 6967 2e73 7570 6572 7573 6572  config.superuser
+000001d0: 7320 2023 20e8 b685 e7ae a169 640a 6865  s  # ......id.he
+000001e0: 6164 6572 7320 3d20 7b0a 2020 2020 2248  aders = {.    "H
+000001f0: 6f73 7422 3a20 2268 352e 6379 6f6c 2e63  ost": "h5.cyol.c
+00000200: 6f6d 222c 0a20 2020 2022 436f 6e6e 6563  om",.    "Connec
+00000210: 7469 6f6e 223a 2022 6b65 6570 2d61 6c69  tion": "keep-ali
+00000220: 7665 222c 0a20 2020 2022 4163 6365 7074  ve",.    "Accept
+00000230: 223a 2022 6170 706c 6963 6174 696f 6e2f  ": "application/
+00000240: 6a73 6f6e 2c20 7465 7874 2f6a 6176 6173  json, text/javas
+00000250: 6372 6970 742c 202a 2f2a 3b20 713d 302e  cript, */*; q=0.
+00000260: 3031 222c 0a20 2020 2022 5573 6572 2d41  01",.    "User-A
+00000270: 6765 6e74 223a 2022 4d6f 7a69 6c6c 612f  gent": "Mozilla/
+00000280: 352e 3020 284c 696e 7578 3b20 416e 6472  5.0 (Linux; Andr
+00000290: 6f69 6420 3130 3b20 5041 434d 3030 2042  oid 10; PACM00 B
+000002a0: 7569 6c64 2f51 5031 412e 3139 3037 3131  uild/QP1A.190711
+000002b0: 2e30 3230 3b20 7776 2920 4170 706c 6557  .020; wv) AppleW
+000002c0: 6562 4b69 742f 3533 372e 3336 2028 4b48  ebKit/537.36 (KH
+000002d0: 544d 4c2c 206c 696b 6520 4765 636b 6f29  TML, like Gecko)
+000002e0: 2056 6572 7369 6f6e 2f34 2e30 2043 6872   Version/4.0 Chr
+000002f0: 6f6d 652f 3836 2e30 2e34 3234 302e 3939  ome/86.0.4240.99
+00000300: 2058 5745 422f 3331 3634 204d 4d57 4542   XWEB/3164 MMWEB
+00000310: 5344 4b2f 3230 3231 3130 3031 204d 6f62  SDK/20211001 Mob
+00000320: 696c 6520 5361 6661 7269 2f35 3337 2e33  ile Safari/537.3
+00000330: 3620 4d4d 5745 4249 442f 3535 3620 4d69  6 MMWEBID/556 Mi
+00000340: 6372 6f4d 6573 7365 6e67 6572 2f38 2e30  croMessenger/8.0
+00000350: 2e31 362e 3230 3430 2830 7832 3830 3031  .16.2040(0x28001
+00000360: 3035 3629 2050 726f 6365 7373 2f74 6f6f  056) Process/too
+00000370: 6c73 6d70 2057 6543 6861 742f 6172 6d33  lsmp WeChat/arm3
+00000380: 3220 5765 6978 696e 204e 6574 5479 7065  2 Weixin NetType
+00000390: 2f57 4946 4920 4c61 6e67 7561 6765 2f7a  /WIFI Language/z
+000003a0: 685f 434e 2041 4249 2f61 726d 3634 222c  h_CN ABI/arm64",
+000003b0: 0a20 2020 2022 4f72 6967 696e 223a 2022  .    "Origin": "
+000003c0: 6874 7470 3a2f 2f68 352e 6379 6f6c 2e63  http://h5.cyol.c
+000003d0: 6f6d 222c 0a20 2020 2022 582d 5265 7175  om",.    "X-Requ
+000003e0: 6573 7465 642d 5769 7468 223a 2022 636f  ested-With": "co
+000003f0: 6d2e 7465 6e63 656e 742e 6d6d 222c 0a20  m.tencent.mm",. 
+00000400: 2020 2022 5365 632d 4665 7463 682d 5369     "Sec-Fetch-Si
+00000410: 7465 223a 2022 6372 6f73 732d 7369 7465  te": "cross-site
+00000420: 222c 0a20 2020 2022 5365 632d 4665 7463  ",.    "Sec-Fetc
+00000430: 682d 4d6f 6465 223a 2022 636f 7273 222c  h-Mode": "cors",
+00000440: 0a20 2020 2022 5365 632d 4665 7463 682d  .    "Sec-Fetch-
+00000450: 4465 7374 223a 2022 656d 7074 7922 2c0a  Dest": "empty",.
+00000460: 2020 2020 2241 6363 6570 742d 456e 636f      "Accept-Enco
+00000470: 6469 6e67 223a 2022 677a 6970 2c20 6465  ding": "gzip, de
+00000480: 666c 6174 6522 2c0a 2020 2020 2241 6363  flate",.    "Acc
+00000490: 6570 742d 4c61 6e67 7561 6765 223a 2022  ept-Language": "
+000004a0: 7a68 2d43 4e2c 7a68 3b71 3d30 2e39 2c65  zh-CN,zh;q=0.9,e
+000004b0: 6e2d 5553 3b71 3d30 2e38 2c65 6e3b 713d  n-US;q=0.8,en;q=
+000004c0: 302e 3722 2c0a 7d0a 0a0a 6173 796e 6320  0.7",.}...async 
+000004d0: 6465 6620 6372 6177 6c5f 616e 7377 6572  def crawl_answer
+000004e0: 2875 726c 3a20 7374 7229 202d 3e20 6469  (url: str) -> di
+000004f0: 6374 3a0a 2020 2020 2222 220a 2020 2020  ct:.    """.    
+00000500: e88e b7e5 8f96 e99d 92e5 b9b4 e5a4 a7e5  ................
+00000510: ada6 e4b9 a0e7 9a84 e69c 9fe6 95b0 efbc  ................
+00000520: 8ce7 ad94 e6a1 88e5 928c e5ae 8ce6 8890  ................
+00000530: e688 aae5 9bbe e993 bee6 8ea5 0a20 2020  .............   
+00000540: 203a 7061 7261 6d20 7572 6c3a 20e6 9c80   :param url: ...
+00000550: e696 b0e4 b880 e69c 9fe5 a4a7 e5ad a6e4  ................
+00000560: b9a0 e79a 84e5 9cb0 e59d 800a 2020 2020  ............    
+00000570: 3a72 6574 7572 6e3a 0a20 2020 2022 2222  :return:.    """
+00000580: 0a20 2020 2061 7379 6e63 2077 6974 6820  .    async with 
+00000590: 4173 796e 6343 6c69 656e 7428 6865 6164  AsyncClient(head
+000005a0: 6572 733d 6865 6164 6572 732c 206d 6178  ers=headers, max
+000005b0: 5f72 6564 6972 6563 7473 3d35 2920 6173  _redirects=5) as
+000005c0: 2063 6c69 656e 743a 0a20 2020 2020 2020   client:.       
+000005d0: 2072 6573 7020 3d20 6177 6169 7420 636c   resp = await cl
+000005e0: 6965 6e74 2e67 6574 2875 726c 3d75 726c  ient.get(url=url
+000005f0: 2c20 7469 6d65 6f75 743d 3130 290a 2020  , timeout=10).  
+00000600: 2020 7265 7370 2e65 6e63 6f64 696e 6720    resp.encoding 
+00000610: 3d20 2775 7466 2d38 270a 2020 2020 736f  = 'utf-8'.    so
+00000620: 7570 203d 2042 6561 7574 6966 756c 536f  up = BeautifulSo
+00000630: 7570 2872 6573 702e 7465 7874 2c20 276c  up(resp.text, 'l
+00000640: 786d 6c27 290a 2020 2020 7469 746c 6520  xml').    title 
+00000650: 3d20 736f 7570 2e66 696e 6428 2774 6974  = soup.find('tit
+00000660: 6c65 2729 2e74 6578 745b 373a 5d2e 7374  le').text[7:].st
+00000670: 7269 7028 290a 2020 2020 7374 6172 745f  rip().    start_
+00000680: 6469 7620 3d20 7265 7370 2e74 6578 742e  div = resp.text.
+00000690: 6669 6e64 2827 3c64 6976 2063 6c61 7373  find('<div class
+000006a0: 3d22 7365 6374 696f 6e30 2074 6f70 696e  ="section0 topin
+000006b0: 6465 7822 3e27 290a 2020 2020 656e 645f  dex">').    end_
+000006c0: 6469 7620 3d20 7265 7370 2e74 6578 742e  div = resp.text.
+000006d0: 6669 6e64 2827 3c73 6372 6970 7420 7479  find('<script ty
+000006e0: 7065 3d22 7465 7874 2f6a 6176 6173 6372  pe="text/javascr
+000006f0: 6970 7422 2073 7263 3d22 6a73 2f69 6e64  ipt" src="js/ind
+00000700: 6578 2e6a 7327 290a 2020 2020 736f 7570  ex.js').    soup
+00000710: 203d 2042 6561 7574 6966 756c 536f 7570   = BeautifulSoup
+00000720: 2872 6573 702e 7465 7874 5b73 7461 7274  (resp.text[start
+00000730: 5f64 6976 3a65 6e64 5f64 6976 5d2c 2027  _div:end_div], '
+00000740: 6c78 6d6c 2729 0a20 2020 2074 6d70 203d  lxml').    tmp =
+00000750: 205b 5d0a 2020 2020 616e 7377 6572 5f61   [].    answer_a
+00000760: 7474 7273 203d 207b 2272 6571 7569 7265  ttrs = {"require
+00000770: 6422 3a20 5b5d 2c20 226f 7074 696f 6e61  d": [], "optiona
+00000780: 6c22 3a20 5b5d 7d0a 2020 2020 6f70 7469  l": []}.    opti
+00000790: 6f6e 203d 2022 4142 4344 4546 220a 2020  on = "ABCDEF".  
+000007a0: 2020 7465 6d70 6c61 7465 203d 2022 7b6e    template = "{n
+000007b0: 756d 7d2e 207b 6368 6563 6b7d 220a 2020  um}. {check}".  
+000007c0: 2020 666f 7220 6469 7620 696e 2073 6f75    for div in sou
+000007d0: 702e 6669 6e64 2822 626f 6479 2229 3a0a  p.find("body"):.
+000007e0: 2020 2020 2020 2020 6966 2064 6976 203d          if div =
+000007f0: 3d20 225c 6e22 3a0a 2020 2020 2020 2020  = "\n":.        
+00000800: 2020 2020 636f 6e74 696e 7565 0a20 2020      continue.   
+00000810: 2020 2020 2061 6e73 7765 7220 3d20 5b5d       answer = []
+00000820: 0a20 2020 2020 2020 2069 6620 6469 762e  .        if div.
+00000830: 6e61 6d65 203d 3d20 2264 6976 223a 0a20  name == "div":. 
+00000840: 2020 2020 2020 2020 2020 2066 6f72 2069             for i
+00000850: 2069 6e20 6469 762e 6669 6e64 5f61 6c6c   in div.find_all
+00000860: 2822 6469 7622 293a 0a20 2020 2020 2020  ("div"):.       
+00000870: 2020 2020 2020 2020 2063 6865 636b 203d           check =
+00000880: 2069 2e67 6574 2822 6461 7461 2d61 2229   i.get("data-a")
+00000890: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+000008a0: 2069 6620 6368 6563 6b20 6973 206e 6f74   if check is not
+000008b0: 204e 6f6e 653a 0a20 2020 2020 2020 2020   None:.         
+000008c0: 2020 2020 2020 2020 2020 2061 6e73 7765             answe
+000008d0: 722e 6170 7065 6e64 2863 6865 636b 290a  r.append(check).
+000008e0: 2020 2020 2020 2020 2020 2020 6966 206c              if l
+000008f0: 656e 2861 6e73 7765 7229 203e 2034 3a0a  en(answer) > 4:.
+00000900: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00000910: 616e 7377 6572 203d 2061 6e73 7765 725b  answer = answer[
+00000920: 3a69 6e74 286c 656e 2861 6e73 7765 7229  :int(len(answer)
+00000930: 202f 2032 295d 0a20 2020 2020 2020 2020   / 2)].         
+00000940: 2020 2074 6d70 2e61 7070 656e 6428 616e     tmp.append(an
+00000950: 7377 6572 290a 2020 2020 7265 715f 656e  swer).    req_en
+00000960: 6420 3d20 300a 2020 2020 666c 6167 203d  d = 0.    flag =
+00000970: 207b 226c 6f63 6174 696f 6e22 3a20 302c   {"location": 0,
+00000980: 2022 7265 7375 6c74 223a 2054 7275 657d   "result": True}
+00000990: 0a20 2020 2066 6f72 2069 2c20 7620 696e  .    for i, v in
+000009a0: 2065 6e75 6d65 7261 7465 2874 6d70 293a   enumerate(tmp):
+000009b0: 0a20 2020 2020 2020 2069 6620 6c65 6e28  .        if len(
+000009c0: 7629 203d 3d20 303a 0a20 2020 2020 2020  v) == 0:.       
+000009d0: 2020 2020 2072 6571 5f65 6e64 203d 2069       req_end = i
+000009e0: 202b 2031 0a20 2020 2020 2020 2065 6c69   + 1.        eli
+000009f0: 6620 666c 6167 5b22 7265 7375 6c74 225d  f flag["result"]
+00000a00: 3a0a 2020 2020 2020 2020 2020 2020 666c  :.            fl
+00000a10: 6167 5b22 7265 7375 6c74 225d 203d 2046  ag["result"] = F
+00000a20: 616c 7365 0a20 2020 2020 2020 2020 2020  alse.           
+00000a30: 2066 6c61 675b 226c 6f63 6174 696f 6e22   flag["location"
+00000a40: 5d20 3d20 690a 2020 2020 666f 7220 692c  ] = i.    for i,
+00000a50: 2076 2069 6e20 656e 756d 6572 6174 6528   v in enumerate(
+00000a60: 746d 7029 3a0a 2020 2020 2020 2020 6966  tmp):.        if
+00000a70: 2066 6c61 675b 226c 6f63 6174 696f 6e22   flag["location"
+00000a80: 5d20 3c20 7265 715f 656e 6420 616e 6420  ] < req_end and 
+00000a90: 7265 715f 656e 6420 2d20 3120 3e20 6920  req_end - 1 > i 
+00000aa0: 3e3d 2066 6c61 675b 226c 6f63 6174 696f  >= flag["locatio
+00000ab0: 6e22 5d3a 0a20 2020 2020 2020 2020 2020  n"]:.           
+00000ac0: 2066 6965 6c64 203d 2022 7265 7175 6972   field = "requir
+00000ad0: 6564 220a 2020 2020 2020 2020 2020 2020  ed".            
+00000ae0: 616e 7377 6572 5f61 7474 7273 5b66 6965  answer_attrs[fie
+00000af0: 6c64 5d2e 6170 7065 6e64 2876 290a 2020  ld].append(v).  
+00000b00: 2020 2020 2020 656c 6966 2066 6c61 675b        elif flag[
+00000b10: 226c 6f63 6174 696f 6e22 5d20 3d3d 2072  "location"] == r
+00000b20: 6571 5f65 6e64 2061 6e64 2069 203e 3d20  eq_end and i >= 
+00000b30: 7265 715f 656e 643a 0a20 2020 2020 2020  req_end:.       
+00000b40: 2020 2020 2066 6965 6c64 203d 2022 6f70       field = "op
+00000b50: 7469 6f6e 616c 220a 2020 2020 2020 2020  tional".        
+00000b60: 2020 2020 616e 7377 6572 5f61 7474 7273      answer_attrs
+00000b70: 5b66 6965 6c64 5d2e 6170 7065 6e64 2876  [field].append(v
+00000b80: 290a 2020 2020 2020 2020 656c 6966 2066  ).        elif f
+00000b90: 6c61 675b 226c 6f63 6174 696f 6e22 5d20  lag["location"] 
+00000ba0: 3c20 7265 715f 656e 6420 3c3d 2069 3a0a  < req_end <= i:.
+00000bb0: 2020 2020 2020 2020 2020 2020 6669 656c              fiel
+00000bc0: 6420 3d20 226f 7074 696f 6e61 6c22 0a20  d = "optional". 
+00000bd0: 2020 2020 2020 2020 2020 2061 6e73 7765             answe
+00000be0: 725f 6174 7472 735b 6669 656c 645d 2e61  r_attrs[field].a
+00000bf0: 7070 656e 6428 7629 0a20 2020 206f 7574  ppend(v).    out
+00000c00: 7075 7420 3d20 5b5d 0a20 2020 2069 6620  put = [].    if 
+00000c10: 6c65 6e28 616e 7377 6572 5f61 7474 7273  len(answer_attrs
+00000c20: 5b22 7265 7175 6972 6564 225d 2920 3e20  ["required"]) > 
+00000c30: 303a 0a20 2020 2020 2020 206f 7574 7075  0:.        outpu
+00000c40: 742e 6170 7065 6e64 2822 e69c ace6 9c9f  t.append("......
+00000c50: e7ad 94e6 a188 5c6e 2229 0a20 2020 2020  ......\n").     
+00000c60: 2020 2066 6f72 2069 2c20 7620 696e 2065     for i, v in e
+00000c70: 6e75 6d65 7261 7465 2861 6e73 7765 725f  numerate(answer_
+00000c80: 6174 7472 735b 2272 6571 7569 7265 6422  attrs["required"
+00000c90: 5d29 3a0a 2020 2020 2020 2020 2020 2020  ]):.            
+00000ca0: 6368 6563 6b73 203d 2022 220a 2020 2020  checks = "".    
+00000cb0: 2020 2020 2020 2020 666f 7220 6a2c 2076          for j, v
+00000cc0: 3220 696e 2065 6e75 6d65 7261 7465 2876  2 in enumerate(v
+00000cd0: 293a 0a20 2020 2020 2020 2020 2020 2020  ):.             
+00000ce0: 2020 2074 7279 3a0a 2020 2020 2020 2020     try:.        
+00000cf0: 2020 2020 2020 2020 2020 2020 6966 2076              if v
+00000d00: 3220 3d3d 2022 3122 3a0a 2020 2020 2020  2 == "1":.      
+00000d10: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00000d20: 2020 6368 6563 6b73 202b 3d20 6f70 7469    checks += opti
+00000d30: 6f6e 5b6a 5d0a 2020 2020 2020 2020 2020  on[j].          
+00000d40: 2020 2020 2020 6578 6365 7074 3a0a 2020        except:.  
+00000d50: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00000d60: 2020 7061 7373 0a20 2020 2020 2020 2020    pass.         
+00000d70: 2020 206f 7574 7075 742e 6170 7065 6e64     output.append
+00000d80: 2874 656d 706c 6174 652e 666f 726d 6174  (template.format
+00000d90: 286e 756d 3d69 202b 2031 2c20 6368 6563  (num=i + 1, chec
+00000da0: 6b3d 6368 6563 6b73 2920 2b20 225c 6e22  k=checks) + "\n"
+00000db0: 290a 2020 2020 6966 206c 656e 2861 6e73  ).    if len(ans
+00000dc0: 7765 725f 6174 7472 735b 226f 7074 696f  wer_attrs["optio
+00000dd0: 6e61 6c22 5d29 2021 3d20 303a 0a20 2020  nal"]) != 0:.   
+00000de0: 2020 2020 206f 7574 7075 742e 6170 7065       output.appe
+00000df0: 6e64 2822 e8af bee5 a496 e4b9 a0e9 a298  nd("............
+00000e00: 5c6e 2229 0a20 2020 2020 2020 2066 6f72  \n").        for
+00000e10: 2069 2c20 7620 696e 2065 6e75 6d65 7261   i, v in enumera
+00000e20: 7465 2861 6e73 7765 725f 6174 7472 735b  te(answer_attrs[
+00000e30: 226f 7074 696f 6e61 6c22 5d29 3a0a 2020  "optional"]):.  
+00000e40: 2020 2020 2020 2020 2020 6368 6563 6b73            checks
+00000e50: 203d 2022 220a 2020 2020 2020 2020 2020   = "".          
+00000e60: 2020 666f 7220 6a2c 2076 3220 696e 2065    for j, v2 in e
+00000e70: 6e75 6d65 7261 7465 2876 293a 0a20 2020  numerate(v):.   
+00000e80: 2020 2020 2020 2020 2020 2020 2069 6620               if 
+00000e90: 7632 203d 3d20 2231 223a 0a20 2020 2020  v2 == "1":.     
+00000ea0: 2020 2020 2020 2020 2020 2020 2020 2063                 c
+00000eb0: 6865 636b 7320 2b3d 206f 7074 696f 6e5b  hecks += option[
+00000ec0: 6a5d 0a20 2020 2020 2020 2020 2020 206f  j].            o
+00000ed0: 7574 7075 742e 6170 7065 6e64 2874 656d  utput.append(tem
+00000ee0: 706c 6174 652e 666f 726d 6174 286e 756d  plate.format(num
+00000ef0: 3d69 202b 2031 2c20 6368 6563 6b3d 6368  =i + 1, check=ch
+00000f00: 6563 6b73 2920 2b20 225c 6e22 290a 2020  ecks) + "\n").  
+00000f10: 2020 7265 7375 6c74 203d 205b 6f75 7470    result = [outp
+00000f20: 7574 5b30 5d5d 0a20 2020 2066 6f72 2069  ut[0]].    for i
+00000f30: 2c20 7620 696e 2065 6e75 6d65 7261 7465  , v in enumerate
+00000f40: 286f 7574 7075 7429 3a0a 2020 2020 2020  (output):.      
+00000f50: 2020 6966 2069 2025 2031 3320 213d 2030    if i % 13 != 0
+00000f60: 2061 6e64 2069 2021 3d20 303a 0a20 2020   and i != 0:.   
+00000f70: 2020 2020 2020 2020 2072 6573 756c 745b           result[
+00000f80: 696e 7428 6920 2f20 3133 295d 202b 3d20  int(i / 13)] += 
+00000f90: 760a 2020 2020 2020 2020 656c 6966 2069  v.        elif i
+00000fa0: 2025 2031 3320 3d3d 2030 2061 6e64 2069   % 13 == 0 and i
+00000fb0: 2021 3d20 303a 0a20 2020 2020 2020 2020   != 0:.         
+00000fc0: 2020 2072 6573 756c 742e 6170 7065 6e64     result.append
+00000fd0: 2876 290a 2020 2020 7472 793a 0a20 2020  (v).    try:.   
+00000fe0: 2020 2020 2065 6e64 5f75 726c 203d 2075       end_url = u
+00000ff0: 726c 2e72 6570 6c61 6365 2827 6d2e 6874  rl.replace('m.ht
+00001000: 6d6c 272c 2027 696d 6167 6573 2f65 6e64  ml', 'images/end
+00001010: 2e6a 7067 2729 0a20 2020 2065 7863 6570  .jpg').    excep
+00001020: 743a 0a20 2020 2020 2020 2065 6e64 5f75  t:.        end_u
+00001030: 726c 203d 2075 726c 5b3a 2d36 5d20 2b20  rl = url[:-6] + 
+00001040: 2769 6d61 6765 732f 656e 642e 6a70 6727  'images/end.jpg'
+00001050: 0a20 2020 2072 6574 7572 6e20 7b0a 2020  .    return {.  
+00001060: 2020 2020 2020 2265 6e64 5f75 726c 223a        "end_url":
+00001070: 2065 6e64 5f75 726c 2c0a 2020 2020 2020   end_url,.      
+00001080: 2020 2263 6174 616c 6f67 7565 223a 2074    "catalogue": t
+00001090: 6974 6c65 2c0a 2020 2020 2020 2020 2261  itle,.        "a
+000010a0: 6e73 7765 7222 3a20 7265 7375 6c74 5b30  nswer": result[0
+000010b0: 5d0a 2020 2020 7d0a 0a0a 6173 796e 6320  ].    }...async 
+000010c0: 6465 6620 7570 6461 7465 5f61 6e73 7765  def update_answe
+000010d0: 7228 293a 0a20 2020 206c 6f67 6765 722e  r():.    logger.
+000010e0: 6f70 7428 636f 6c6f 7273 3d54 7275 6529  opt(colors=True)
+000010f0: 2e69 6e66 6f28 223c 753e 3c79 3e5b e5a4  .info("<u><y>[..
+00001100: a7e5 ada6 e4b9 a0e6 95b0 e68d aee5 ba93  ................
+00001110: 5d3c 2f79 3e3c 2f75 3e3c 673e e29e a4e2  ]</y></u><g>....
+00001120: 9ea4 e29e a4e2 9ea4 e29e a4e6 a380 e69f  ................
+00001130: a5e7 ad94 e6a1 88e6 95b0 e68d aee2 9c94  ................
+00001140: e29c 94e2 9c94 e29c 94e2 9c94 3c2f 673e  ............</g>
+00001150: 2229 0a20 2020 2072 6573 705f 7572 6c20  ").    resp_url 
+00001160: 3d20 2768 7474 7073 3a2f 2f68 352e 6379  = 'https://h5.cy
+00001170: 6f6c 2e63 6f6d 2f73 7065 6369 616c 2f77  ol.com/special/w
+00001180: 6569 7869 6e2f 7369 676e 2e6a 736f 6e27  eixin/sign.json'
+00001190: 0a20 2020 2061 7379 6e63 2077 6974 6820  .    async with 
+000011a0: 4173 796e 6343 6c69 656e 7428 6865 6164  AsyncClient(head
+000011b0: 6572 733d 6865 6164 6572 7329 2061 7320  ers=headers) as 
+000011c0: 636c 6965 6e74 3a0a 2020 2020 2020 2020  client:.        
+000011d0: 7265 7370 6f6e 7365 203d 2061 7761 6974  response = await
+000011e0: 2063 6c69 656e 742e 6765 7428 7572 6c3d   client.get(url=
+000011f0: 7265 7370 5f75 726c 2c20 7469 6d65 6f75  resp_url, timeou
+00001200: 743d 3130 290a 2020 2020 7265 7370 6f6e  t=10).    respon
+00001210: 7365 2e65 6e63 6f64 696e 6720 3d20 7265  se.encoding = re
+00001220: 7370 6f6e 7365 2e63 6861 7273 6574 5f65  sponse.charset_e
+00001230: 6e63 6f64 696e 670a 2020 2020 7265 7375  ncoding.    resu
+00001240: 6c74 203d 206a 736f 6e2e 6c6f 6164 7328  lt = json.loads(
+00001250: 7265 7370 6f6e 7365 2e74 6578 7429 0a20  response.text). 
+00001260: 2020 2063 6f64 655f 7265 7375 6c74 203d     code_result =
+00001270: 206c 6973 7428 7265 7375 6c74 295b 2d31   list(result)[-1
+00001280: 303a 5d0a 2020 2020 666f 7220 636f 6465  0:].    for code
+00001290: 2069 6e20 636f 6465 5f72 6573 756c 743a   in code_result:
+000012a0: 0a20 2020 2020 2020 2069 6620 6177 6169  .        if awai
+000012b0: 7420 416e 7377 6572 2e66 696c 7465 7228  t Answer.filter(
+000012c0: 636f 6465 3d63 6f64 6529 2e63 6f75 6e74  code=code).count
+000012d0: 2829 3a0a 2020 2020 2020 2020 2020 2020  ():.            
+000012e0: 636f 6e74 696e 7565 0a20 2020 2020 2020  continue.       
+000012f0: 2065 6c73 653a 0a20 2020 2020 2020 2020   else:.         
+00001300: 2020 2074 7279 3a0a 2020 2020 2020 2020     try:.        
+00001310: 2020 2020 2020 2020 7572 6c20 3d20 7265          url = re
+00001320: 7375 6c74 5b63 6f64 655d 5b22 7572 6c22  sult[code]["url"
+00001330: 5d0a 2020 2020 2020 2020 2020 2020 2020  ].              
+00001340: 2020 6461 7461 203d 2061 7761 6974 2063    data = await c
+00001350: 7261 776c 5f61 6e73 7765 7228 7572 6c3d  rawl_answer(url=
+00001360: 7572 6c29 0a20 2020 2020 2020 2020 2020  url).           
+00001370: 2020 2020 2065 6e64 5f75 726c 203d 2064       end_url = d
+00001380: 6174 615b 2265 6e64 5f75 726c 225d 0a20  ata["end_url"]. 
+00001390: 2020 2020 2020 2020 2020 2020 2020 2061                 a
+000013a0: 6e73 7765 7220 3d20 6461 7461 5b22 616e  nswer = data["an
+000013b0: 7377 6572 225d 0a20 2020 2020 2020 2020  swer"].         
+000013c0: 2020 2020 2020 2063 6174 616c 6f67 7565         catalogue
+000013d0: 203d 2064 6174 615b 2263 6174 616c 6f67   = data["catalog
+000013e0: 7565 225d 0a20 2020 2020 2020 2020 2020  ue"].           
+000013f0: 2020 2020 2061 7379 6e63 2077 6974 6820       async with 
+00001400: 4173 796e 6343 6c69 656e 7428 6865 6164  AsyncClient(head
+00001410: 6572 733d 6865 6164 6572 7329 2061 7320  ers=headers) as 
+00001420: 636c 6965 6e74 3a0a 2020 2020 2020 2020  client:.        
+00001430: 2020 2020 2020 2020 2020 2020 656e 645f              end_
+00001440: 6a70 6720 3d20 6177 6169 7420 636c 6965  jpg = await clie
+00001450: 6e74 2e67 6574 2865 6e64 5f75 726c 2c20  nt.get(end_url, 
+00001460: 7469 6d65 6f75 743d 3130 290a 2020 2020  timeout=10).    
+00001470: 2020 2020 2020 2020 2020 2020 636f 7665              cove
+00001480: 7220 3d20 656e 645f 6a70 672e 636f 6e74  r = end_jpg.cont
+00001490: 656e 740a 2020 2020 2020 2020 2020 2020  ent.            
+000014a0: 2020 2020 6177 6169 7420 416e 7377 6572      await Answer
+000014b0: 2e63 7265 6174 6528 0a20 2020 2020 2020  .create(.       
+000014c0: 2020 2020 2020 2020 2020 2020 2074 696d               tim
+000014d0: 653d 7469 6d65 2e74 696d 6528 292c 0a20  e=time.time(),. 
+000014e0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000014f0: 2020 2063 6f64 653d 636f 6465 2c0a 2020     code=code,.  
+00001500: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00001510: 2020 6361 7461 6c6f 6775 653d 6361 7461    catalogue=cata
+00001520: 6c6f 6775 652c 0a20 2020 2020 2020 2020  logue,.         
+00001530: 2020 2020 2020 2020 2020 2075 726c 3d75             url=u
+00001540: 726c 2c0a 2020 2020 2020 2020 2020 2020  rl,.            
+00001550: 2020 2020 2020 2020 656e 645f 7572 6c3d          end_url=
+00001560: 656e 645f 7572 6c2c 0a20 2020 2020 2020  end_url,.       
+00001570: 2020 2020 2020 2020 2020 2020 2061 6e73               ans
+00001580: 7765 723d 616e 7377 6572 2c0a 2020 2020  wer=answer,.    
+00001590: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000015a0: 636f 7665 723d 636f 7665 720a 2020 2020  cover=cover.    
+000015b0: 2020 2020 2020 2020 2020 2020 290a 2020              ).  
+000015c0: 2020 2020 2020 2020 2020 2020 2020 6c6f                lo
+000015d0: 6767 6572 2e6f 7074 2863 6f6c 6f72 733d  gger.opt(colors=
+000015e0: 5472 7565 292e 7375 6363 6573 7328 6622  True).success(f"
+000015f0: 3c75 3e3c 793e e99d 92e5 b9b4 e5a4 a7e5  <u><y>..........
+00001600: ada6 e4b9 a03c 2f79 3e3c 2f75 3e20 3c6d  .....</y></u> <m
+00001610: 3e7b 6361 7461 6c6f 6775 657d 3c2f 6d3e  >{catalogue}</m>
+00001620: 203c 673e e69b b4e6 96b0 e688 90e5 8a9f   <g>............
+00001630: 213c 2f67 3e22 290a 2020 2020 2020 2020  !</g>").        
+00001640: 2020 2020 6578 6365 7074 2045 7863 6570      except Excep
+00001650: 7469 6f6e 2061 7320 653a 0a20 2020 2020  tion as e:.     
+00001660: 2020 2020 2020 2020 2020 206c 6f67 6765             logge
+00001670: 722e 6572 726f 7228 6529 0a20 2020 206c  r.error(e).    l
+00001680: 6f67 6765 722e 6f70 7428 636f 6c6f 7273  ogger.opt(colors
+00001690: 3d54 7275 6529 2e73 7563 6365 7373 2822  =True).success("
+000016a0: 3c75 3e3c 793e 5be5 a4a7 e5ad a6e4 b9a0  <u><y>[.........
+000016b0: e695 b0e6 8dae e5ba 935d 3c2f 793e 3c2f  .........]</y></
+000016c0: 753e 3c67 3ee2 9ea4 e29e a4e2 9ea4 e29e  u><g>...........
+000016d0: a4e2 9ea4 e7ad 94e6 a188 e695 b0e6 8dae  ................
+000016e0: e69b b4e6 96b0 e5ae 8ce6 8890 e29c 94e2  ................
+000016f0: 9c94 e29c 94e2 9c94 e29c 943c 2f67 3e22  ...........</g>"
+00001700: 290a 0a0a 4073 6368 6564 756c 6572 2e73  )...@scheduler.s
+00001710: 6368 6564 756c 6564 5f6a 6f62 2827 6372  cheduled_job('cr
+00001720: 6f6e 272c 2064 6179 5f6f 665f 7765 656b  on', day_of_week
+00001730: 3d27 3627 2c20 686f 7572 3d22 3231 2d32  ='6', hour="21-2
+00001740: 3322 2c20 6d69 6e75 7465 3d22 2a2f 3135  3", minute="*/15
+00001750: 222c 2069 643d 2775 7064 6174 655f 6461  ", id='update_da
+00001760: 7461 272c 0a20 2020 2020 2020 2020 2020  ta',.           
+00001770: 2020 2020 2020 2020 2020 2020 2020 7469                ti
+00001780: 6d65 7a6f 6e65 3d22 4173 6961 2f53 6861  mezone="Asia/Sha
+00001790: 6e67 6861 6922 290a 6173 796e 6320 6465  nghai").async de
+000017a0: 6620 7570 6461 7465 5f64 6174 6128 293a  f update_data():
+000017b0: 0a20 2020 2074 7279 3a0a 2020 2020 2020  .    try:.      
+000017c0: 2020 626f 743a 2042 6f74 203d 2067 6574    bot: Bot = get
+000017d0: 5f62 6f74 2829 0a20 2020 2065 7863 6570  _bot().    excep
+000017e0: 7420 5661 6c75 6545 7272 6f72 2061 7320  t ValueError as 
+000017f0: 653a 0a20 2020 2020 2020 2072 6574 7572  e:.        retur
+00001800: 6e0a 2020 2020 7265 7370 5f75 726c 203d  n.    resp_url =
+00001810: 2027 6874 7470 733a 2f2f 6835 2e63 796f   'https://h5.cyo
+00001820: 6c2e 636f 6d2f 7370 6563 6961 6c2f 7765  l.com/special/we
+00001830: 6978 696e 2f73 6967 6e2e 6a73 6f6e 270a  ixin/sign.json'.
+00001840: 2020 2020 6173 796e 6320 7769 7468 2041      async with A
+00001850: 7379 6e63 436c 6965 6e74 2868 6561 6465  syncClient(heade
+00001860: 7273 3d68 6561 6465 7273 2920 6173 2063  rs=headers) as c
+00001870: 6c69 656e 743a 0a20 2020 2020 2020 2072  lient:.        r
+00001880: 6573 706f 6e73 6520 3d20 6177 6169 7420  esponse = await 
+00001890: 636c 6965 6e74 2e67 6574 2875 726c 3d72  client.get(url=r
+000018a0: 6573 705f 7572 6c2c 2074 696d 656f 7574  esp_url, timeout
+000018b0: 3d31 3029 0a20 2020 2072 6573 706f 6e73  =10).    respons
+000018c0: 652e 656e 636f 6469 6e67 203d 2072 6573  e.encoding = res
+000018d0: 706f 6e73 652e 6368 6172 7365 745f 656e  ponse.charset_en
+000018e0: 636f 6469 6e67 0a20 2020 2072 6573 756c  coding.    resul
+000018f0: 7420 3d20 6a73 6f6e 2e6c 6f61 6473 2872  t = json.loads(r
+00001900: 6573 706f 6e73 652e 7465 7874 290a 2020  esponse.text).  
+00001910: 2020 636f 6465 5f72 6573 756c 7420 3d20    code_result = 
+00001920: 6c69 7374 2872 6573 756c 7429 5b2d 3130  list(result)[-10
+00001930: 3a5d 0a20 2020 2066 6f72 2063 6f64 6520  :].    for code 
+00001940: 696e 2063 6f64 655f 7265 7375 6c74 3a0a  in code_result:.
+00001950: 2020 2020 2020 2020 6966 2061 7761 6974          if await
+00001960: 2041 6e73 7765 722e 6669 6c74 6572 2863   Answer.filter(c
+00001970: 6f64 653d 636f 6465 292e 636f 756e 7428  ode=code).count(
+00001980: 293a 0a20 2020 2020 2020 2020 2020 2063  ):.            c
+00001990: 6f6e 7469 6e75 650a 2020 2020 2020 2020  ontinue.        
+000019a0: 656c 7365 3a0a 2020 2020 2020 2020 2020  else:.          
+000019b0: 2020 7472 793a 0a20 2020 2020 2020 2020    try:.         
+000019c0: 2020 2020 2020 2075 726c 203d 2072 6573         url = res
+000019d0: 756c 745b 636f 6465 5d5b 2275 726c 225d  ult[code]["url"]
+000019e0: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+000019f0: 2064 6174 6120 3d20 6177 6169 7420 6372   data = await cr
+00001a00: 6177 6c5f 616e 7377 6572 2875 726c 3d75  awl_answer(url=u
+00001a10: 726c 290a 2020 2020 2020 2020 2020 2020  rl).            
+00001a20: 2020 2020 656e 645f 7572 6c20 3d20 6461      end_url = da
+00001a30: 7461 5b22 656e 645f 7572 6c22 5d0a 2020  ta["end_url"].  
+00001a40: 2020 2020 2020 2020 2020 2020 2020 616e                an
+00001a50: 7377 6572 203d 2064 6174 615b 2261 6e73  swer = data["ans
+00001a60: 7765 7222 5d0a 2020 2020 2020 2020 2020  wer"].          
+00001a70: 2020 2020 2020 6361 7461 6c6f 6775 6520        catalogue 
+00001a80: 3d20 6461 7461 5b22 6361 7461 6c6f 6775  = data["catalogu
+00001a90: 6522 5d0a 2020 2020 2020 2020 2020 2020  e"].            
+00001aa0: 2020 2020 6173 796e 6320 7769 7468 2041      async with A
+00001ab0: 7379 6e63 436c 6965 6e74 2868 6561 6465  syncClient(heade
+00001ac0: 7273 3d68 6561 6465 7273 2920 6173 2063  rs=headers) as c
+00001ad0: 6c69 656e 743a 0a20 2020 2020 2020 2020  lient:.         
+00001ae0: 2020 2020 2020 2020 2020 2065 6e64 5f6a             end_j
+00001af0: 7067 203d 2061 7761 6974 2063 6c69 656e  pg = await clien
+00001b00: 742e 6765 7428 656e 645f 7572 6c2c 2074  t.get(end_url, t
+00001b10: 696d 656f 7574 3d31 3029 0a20 2020 2020  imeout=10).     
+00001b20: 2020 2020 2020 2020 2020 2063 6f76 6572             cover
+00001b30: 203d 2065 6e64 5f6a 7067 2e63 6f6e 7465   = end_jpg.conte
+00001b40: 6e74 0a20 2020 2020 2020 2020 2020 2020  nt.             
+00001b50: 2020 2061 7761 6974 2041 6e73 7765 722e     await Answer.
+00001b60: 6372 6561 7465 280a 2020 2020 2020 2020  create(.        
+00001b70: 2020 2020 2020 2020 2020 2020 7469 6d65              time
+00001b80: 3d74 696d 652e 7469 6d65 2829 2c0a 2020  =time.time(),.  
+00001b90: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00001ba0: 2020 636f 6465 3d63 6f64 652c 0a20 2020    code=code,.   
+00001bb0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00001bc0: 2063 6174 616c 6f67 7565 3d63 6174 616c   catalogue=catal
+00001bd0: 6f67 7565 2c0a 2020 2020 2020 2020 2020  ogue,.          
+00001be0: 2020 2020 2020 2020 2020 7572 6c3d 7572            url=ur
+00001bf0: 6c2c 0a20 2020 2020 2020 2020 2020 2020  l,.             
+00001c00: 2020 2020 2020 2065 6e64 5f75 726c 3d65         end_url=e
+00001c10: 6e64 5f75 726c 2c0a 2020 2020 2020 2020  nd_url,.        
+00001c20: 2020 2020 2020 2020 2020 2020 616e 7377              answ
+00001c30: 6572 3d61 6e73 7765 722c 0a20 2020 2020  er=answer,.     
+00001c40: 2020 2020 2020 2020 2020 2020 2020 2063                 c
+00001c50: 6f76 6572 3d63 6f76 6572 0a20 2020 2020  over=cover.     
+00001c60: 2020 2020 2020 2020 2020 2029 0a20 2020             ).   
+00001c70: 2020 2020 2020 2020 2020 2020 206c 6f67               log
+00001c80: 6765 722e 6f70 7428 636f 6c6f 7273 3d54  ger.opt(colors=T
+00001c90: 7275 6529 2e73 7563 6365 7373 2866 223c  rue).success(f"<
+00001ca0: 753e 3c79 3ee9 9d92 e5b9 b4e5 a4a7 e5ad  u><y>...........
+00001cb0: a6e4 b9a0 3c2f 793e 3c2f 753e 203c 6d3e  ....</y></u> <m>
+00001cc0: 7b63 6174 616c 6f67 7565 7d3c 2f6d 3e20  {catalogue}</m> 
+00001cd0: 3c67 3ee6 9bb4 e696 b0e6 8890 e58a 9f21  <g>............!
+00001ce0: 3c2f 673e 2229 0a20 2020 2020 2020 2020  </g>").         
+00001cf0: 2020 2020 2020 2061 646d 696e 203d 2067         admin = g
+00001d00: 6574 436f 6e66 6967 2829 0a20 2020 2020  etConfig().     
+00001d10: 2020 2020 2020 2020 2020 2063 6f6e 7465             conte
+00001d20: 6e74 203d 2061 7761 6974 2067 6574 5f6c  nt = await get_l
+00001d30: 6f67 696e 5f71 7263 6f64 6528 290a 2020  ogin_qrcode().  
+00001d40: 2020 2020 2020 2020 2020 2020 2020 6966                if
+00001d50: 2061 646d 696e 5b22 5552 4c5f 5354 4154   admin["URL_STAT
+00001d60: 5553 225d 3a0a 2020 2020 2020 2020 2020  US"]:.          
+00001d70: 2020 2020 2020 2020 2020 6177 6169 7420            await 
+00001d80: 626f 742e 7365 6e64 5f70 7269 7661 7465  bot.send_private
+00001d90: 5f6d 7367 2875 7365 725f 6964 3d61 646d  _msg(user_id=adm
+00001da0: 696e 5b22 5355 5045 5255 5345 5222 5d2c  in["SUPERUSER"],
+00001db0: 206d 6573 7361 6765 3d4d 6573 7361 6765   message=Message
+00001dc0: 5365 676d 656e 742e 7465 7874 280a 2020  Segment.text(.  
+00001dd0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00001de0: 2020 2020 2020 6622 e6a3 80e6 b58b e588        f"........
+00001df0: b0e9 9d92 e5b9 b4e5 a4a7 e5ad a6e4 b9a0  ................
+00001e00: e69c 89e6 9bb4 e696 b0ef bc8c e4b8 8be5  ................
+00001e10: 91a8 e4b8 80e4 b8ba 7b63 6174 616c 6f67  ........{catalog
+00001e20: 7565 7d2c e8af a6e7 bb86 e4bf a1e6 81af  ue},............
+00001e30: e8af b7e7 82b9 e587 bbe9 93be e68e a5e7  ................
+00001e40: 99bb e5bd 95e5 908e e58f b0e6 9fa5 e79c  ................
+00001e50: 8bef bc8c e5a6 82e6 8993 e4b8 8de5 bc80  ................
+00001e60: e993 bee6 8ea5 efbc 8ce8 afb7 e5a4 8de5  ................
+00001e70: 88b6 e993 bee6 8ea5 e588 b0e6 b58f e8a7  ................
+00001e80: 88e5 99a8 6428 c2b4 cf89 efbd 802a 295c  ....d(.......*)\
+00001e90: 6e22 2920 2b20 4d65 7373 6167 6553 6567  n") + MessageSeg
+00001ea0: 6d65 6e74 2e74 6578 7428 0a20 2020 2020  ment.text(.     
+00001eb0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00001ec0: 2020 2063 6f6e 7465 6e74 5b22 7572 6c22     content["url"
+00001ed0: 5d29 290a 2020 2020 2020 2020 2020 2020  ])).            
+00001ee0: 2020 2020 6177 6169 7420 626f 742e 7365      await bot.se
+00001ef0: 6e64 5f70 7269 7661 7465 5f6d 7367 2875  nd_private_msg(u
+00001f00: 7365 725f 6964 3d61 646d 696e 5b22 5355  ser_id=admin["SU
+00001f10: 5045 5255 5345 5222 5d2c 206d 6573 7361  PERUSER"], messa
+00001f20: 6765 3d4d 6573 7361 6765 5365 676d 656e  ge=MessageSegmen
+00001f30: 742e 7465 7874 280a 2020 2020 2020 2020  t.text(.        
+00001f40: 2020 2020 2020 2020 2020 2020 6622 e6a3              f"..
+00001f50: 80e6 b58b e588 b0e9 9d92 e5b9 b4e5 a4a7  ................
+00001f60: e5ad a6e4 b9a0 e69c 89e6 9bb4 e696 b0ef  ................
+00001f70: bc8c e4b8 8be5 91a8 e4b8 80e4 b8ba 7b63  ..............{c
+00001f80: 6174 616c 6f67 7565 7d2c e8af a6e7 bb86  atalogue},......
+00001f90: e4bf a1e6 81af e8af b7e6 89ab e7a0 81e7  ................
+00001fa0: 99bb e5bd 95e5 908e e58f b0e6 9fa5 e79c  ................
+00001fb0: 8b64 28c2 b4cf 89ef bd80 2a29 2229 202b  .d(.......*)") +
+00001fc0: 204d 6573 7361 6765 5365 676d 656e 742e   MessageSegment.
+00001fd0: 696d 6167 6528 0a20 2020 2020 2020 2020  image(.         
+00001fe0: 2020 2020 2020 2020 2020 2063 6f6e 7465             conte
+00001ff0: 6e74 5b22 636f 6e74 656e 7422 5d29 290a  nt["content"])).
+00002000: 2020 2020 2020 2020 2020 2020 6578 6365              exce
+00002010: 7074 2045 7863 6570 7469 6f6e 2061 7320  pt Exception as 
+00002020: 653a 0a20 2020 2020 2020 2020 2020 2020  e:.             
+00002030: 2020 206c 6f67 6765 722e 6572 726f 7228     logger.error(
+00002040: 6529 0a0a 0a40 7363 6865 6475 6c65 722e  e)...@scheduler.
+00002050: 7363 6865 6475 6c65 645f 6a6f 6228 2763  scheduled_job('c
+00002060: 726f 6e27 2c20 7365 636f 6e64 3d27 2a2f  ron', second='*/
+00002070: 3130 272c 206d 6973 6669 7265 5f67 7261  10', misfire_gra
+00002080: 6365 5f74 696d 653d 3130 290a 6173 796e  ce_time=10).asyn
+00002090: 6320 6465 6620 6368 6563 6b5f 6170 706c  c def check_appl
+000020a0: 7928 293a 0a20 2020 2074 7279 3a0a 2020  y():.    try:.  
+000020b0: 2020 2020 2020 626f 743a 2042 6f74 203d        bot: Bot =
+000020c0: 2067 6574 5f62 6f74 2829 0a20 2020 2065   get_bot().    e
+000020d0: 7863 6570 7420 5661 6c75 6545 7272 6f72  xcept ValueError
+000020e0: 2061 7320 653a 0a20 2020 2020 2020 2072   as e:.        r
+000020f0: 6574 7572 6e0a 2020 2020 6170 706c 795f  eturn.    apply_
+00002100: 6c69 7374 203d 2061 7761 6974 2041 6464  list = await Add
+00002110: 5573 6572 2e66 696c 7465 7228 7374 6174  User.filter(stat
+00002120: 7573 3d22 e69c aae9 809a e8bf 8722 292e  us=".........").
+00002130: 7661 6c75 6573 2829 0a0a 2020 2020 666f  values()..    fo
+00002140: 7220 6974 656d 2069 6e20 6170 706c 795f  r item in apply_
+00002150: 6c69 7374 3a0a 2020 2020 2020 2020 7265  list:.        re
+00002160: 7375 6c74 203d 2061 7761 6974 2055 7365  sult = await Use
+00002170: 722e 6669 6c74 6572 2875 7365 725f 6964  r.filter(user_id
+00002180: 3d69 7465 6d5b 2275 7365 725f 6964 225d  =item["user_id"]
+00002190: 2c20 6772 6f75 705f 6964 3d69 7465 6d5b  , group_id=item[
+000021a0: 2267 726f 7570 5f69 6422 5d29 2e63 6f75  "group_id"]).cou
+000021b0: 6e74 2829 0a20 2020 2020 2020 2069 6620  nt().        if 
+000021c0: 7265 7375 6c74 3a0a 2020 2020 2020 2020  result:.        
+000021d0: 2020 2020 6177 6169 7420 4164 6455 7365      await AddUse
+000021e0: 722e 6669 6c74 6572 2869 643d 6974 656d  r.filter(id=item
+000021f0: 5b22 6964 225d 292e 7570 6461 7465 2873  ["id"]).update(s
+00002200: 7461 7475 733d 22e5 b7b2 e980 9ae8 bf87  tatus=".........
+00002210: 2229 0a20 2020 2020 2020 2020 2020 2061  ").            a
+00002220: 7761 6974 2062 6f74 2e73 656e 645f 6772  wait bot.send_gr
+00002230: 6f75 705f 6d73 6728 6772 6f75 705f 6964  oup_msg(group_id
+00002240: 3d69 7465 6d5b 2267 726f 7570 5f69 6422  =item["group_id"
+00002250: 5d2c 0a20 2020 2020 2020 2020 2020 2020  ],.             
+00002260: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00002270: 2020 2020 2020 2020 6d65 7373 6167 653d          message=
+00002280: 4d65 7373 6167 6553 6567 6d65 6e74 2e61  MessageSegment.a
+00002290: 7428 7573 6572 5f69 643d 6974 656d 5b22  t(user_id=item["
+000022a0: 7573 6572 5f69 6422 5d29 202b 204d 6573  user_id"]) + Mes
+000022b0: 7361 6765 5365 676d 656e 742e 7465 7874  sageSegment.text
+000022c0: 280a 2020 2020 2020 2020 2020 2020 2020  (.              
+000022d0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000022e0: 2020 2020 2020 2020 2020 2022 e4bf a1e6             "....
+000022f0: 81af e7bb 91e5 ae9a e688 90e5 8a9f 2820  ..............( 
+00002300: e280 a220 cc80 cf89 e280 a2cc 8120 29e2  ... ......... ).
+00002310: 9ca7 2229 290a 2020 2020 2020 2020 2020  ..")).          
+00002320: 2020 6177 6169 7420 6173 796e 6369 6f2e    await asyncio.
+00002330: 736c 6565 7028 3229 0a20 2020 2020 2020  sleep(2).       
+00002340: 2020 2020 2063 6f6e 7469 6e75 650a 2020       continue.  
+00002350: 2020 2020 2020 6e6f 775f 7469 6d65 203d        now_time =
+00002360: 2069 6e74 2874 696d 652e 7469 6d65 2829   int(time.time()
+00002370: 290a 2020 2020 2020 2020 6966 2028 6e6f  ).        if (no
+00002380: 775f 7469 6d65 202d 2069 7465 6d5b 2274  w_time - item["t
+00002390: 696d 6522 5d29 203e 2031 3830 3a0a 2020  ime"]) > 180:.  
+000023a0: 2020 2020 2020 2020 2020 6177 6169 7420            await 
+000023b0: 4164 6455 7365 722e 6669 6c74 6572 2869  AddUser.filter(i
+000023c0: 643d 6974 656d 5b22 6964 225d 292e 7570  d=item["id"]).up
+000023d0: 6461 7465 2873 7461 7475 733d 22e5 b7b2  date(status="...
+000023e0: e8bf 87e6 9c9f 2229 0a20 2020 2020 2020  ......").       
+000023f0: 2020 2020 2061 7761 6974 2062 6f74 2e73       await bot.s
+00002400: 656e 645f 6772 6f75 705f 6d73 6728 6772  end_group_msg(gr
+00002410: 6f75 705f 6964 3d69 7465 6d5b 2267 726f  oup_id=item["gro
+00002420: 7570 5f69 6422 5d2c 0a20 2020 2020 2020  up_id"],.       
+00002430: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00002440: 2020 2020 2020 2020 2020 2020 2020 6d65                me
+00002450: 7373 6167 653d 4d65 7373 6167 6553 6567  ssage=MessageSeg
+00002460: 6d65 6e74 2e61 7428 7573 6572 5f69 643d  ment.at(user_id=
+00002470: 6974 656d 5b22 7573 6572 5f69 6422 5d29  item["user_id"])
+00002480: 202b 204d 6573 7361 6765 5365 676d 656e   + MessageSegmen
+00002490: 742e 7465 7874 280a 2020 2020 2020 2020  t.text(.        
+000024a0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000024b0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000024c0: 2022 e6b7 bbe5 8aa0 e794 b3e8 afb7 e5b7   "..............
+000024d0: b2e8 bf87 e69c 9fef bc8c e8af b7e9 878d  ................
+000024e0: e696 b0e5 8f91 20e6 b7bb e58a a0e5 a4a7  ...... .........
+000024f0: e5ad a6e4 b9a0 20e6 8c87 e4bb a4e8 bf9b  ...... .........
+00002500: e8a1 8ce7 94b3 e8af b728 20e2 80a2 20cc  .........( ... .
+00002510: 80cf 89e2 80a2 cc81 2029 e29c a722 2929  ........ )..."))
+00002520: 0a20 2020 2020 2020 2020 2020 2061 7761  .            awa
+00002530: 6974 2061 7379 6e63 696f 2e73 6c65 6570  it asyncio.sleep
+00002540: 2832 290a 2020 2020 2020 2020 656c 7365  (2).        else
+00002550: 3a0a 2020 2020 2020 2020 2020 2020 636f  :.            co
+00002560: 6e74 696e 7565 0a0a 0a40 7363 6865 6475  ntinue...@schedu
+00002570: 6c65 722e 7363 6865 6475 6c65 645f 6a6f  ler.scheduled_jo
+00002580: 6228 2763 726f 6e27 2c20 6461 795f 6f66  b('cron', day_of
+00002590: 5f77 6565 6b3d 2730 272c 2068 6f75 723d  _week='0', hour=
+000025a0: 2730 272c 206d 696e 7574 653d 2730 272c  '0', minute='0',
+000025b0: 2069 643d 2763 6c65 6172 272c 2074 696d   id='clear', tim
+000025c0: 657a 6f6e 653d 2241 7369 612f 5368 616e  ezone="Asia/Shan
+000025d0: 6768 6169 2229 0a61 7379 6e63 2064 6566  ghai").async def
+000025e0: 2063 6c65 6172 2829 3a0a 2020 2020 7472   clear():.    tr
+000025f0: 793a 0a20 2020 2020 2020 2072 6573 756c  y:.        resul
+00002600: 7420 3d20 6177 6169 7420 4172 6561 2e61  t = await Area.a
+00002610: 6c6c 2829 2e76 616c 7565 7328 290a 2020  ll().values().  
+00002620: 2020 2020 2020 666f 7220 6974 656d 2069        for item i
+00002630: 6e20 7265 7375 6c74 3a0a 2020 2020 2020  n result:.      
+00002640: 2020 2020 2020 6177 6169 7420 4172 6561        await Area
+00002650: 2e66 696c 7465 7228 6964 3d69 7465 6d5b  .filter(id=item[
+00002660: 2269 6422 5d29 2e75 7064 6174 6528 7374  "id"]).update(st
+00002670: 6174 7573 3d46 616c 7365 290a 2020 2020  atus=False).    
+00002680: 2020 2020 6c6f 6767 6572 2e6f 7074 2863      logger.opt(c
+00002690: 6f6c 6f72 733d 5472 7565 292e 7375 6363  olors=True).succ
+000026a0: 6573 7328 0a20 2020 2020 2020 2020 2020  ess(.           
+000026b0: 2066 223c 753e 3c79 3e5b e5a4 a7e5 ada6   f"<u><y>[......
+000026c0: e4b9 a0e6 95b0 e68d aee5 ba93 5d3c 2f79  ............]</y
+000026d0: 3e3c 2f75 3e20 3c6d 3ee5 9cb0 e58c bae6  ></u> <m>.......
+000026e0: 9c80 e696 b0e4 b880 e69c 9fe7 8ab6 e680  ................
+000026f0: 813c 2f6d 3e20 3c67 3ee9 878d e7bd aee6  .</m> <g>.......
+00002700: 8890 e58a 9f21 3c2f 673e 2229 0a20 2020  .....!</g>").   
+00002710: 2065 7863 6570 7420 4578 6365 7074 696f   except Exceptio
+00002720: 6e20 6173 2065 3a0a 2020 2020 2020 2020  n as e:.        
+00002730: 6c6f 6767 6572 2e6f 7074 2863 6f6c 6f72  logger.opt(color
+00002740: 733d 5472 7565 292e 6572 726f 7228 0a20  s=True).error(. 
+00002750: 2020 2020 2020 2020 2020 2066 223c 753e             f"<u>
+00002760: 3c79 3e5b e5a4 a7e5 ada6 e4b9 a0e6 95b0  <y>[............
+00002770: e68d aee5 ba93 5d3c 2f79 3e3c 2f75 3e20  ......]</y></u> 
+00002780: 3c6d 3ee5 9cb0 e58c bae6 9c80 e696 b0e4  <m>.............
+00002790: b880 e69c 9fe7 8ab6 e680 813c 2f6d 3e20  ...........</m> 
+000027a0: 3c72 e987 8de7 bdae e5a4 b1e8 b4a5 efbc  <r..............
+000027b0: 9a7b 657d 3c2f 723e 2229 0a              .{e}</r>").
```

### Comparing `TeenStudy-0.1.9/TeenStudy/utils/utils.py` & `teenstudy-0.2.0rc1/TeenStudy/utils/utils.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,600 +1,566 @@
-import base64
-import datetime
-import hashlib
-import json
-import os
-import random
-import socket
-import time
-from io import BytesIO
-from pathlib import Path
-
-import qrcode
-from PIL import Image, ImageDraw, ImageFont
-from httpx import AsyncClient
-from nonebot import logger, get_driver, on_command
-from nonebot.adapters.onebot.v11 import MessageEvent
-from nonebot.params import ArgStr
-from nonebot.permission import SUPERUSER
-from pydantic import BaseModel
-
-from . import dxx, path, rule
-from ..models.accuont import User
-from ..models.dxx import Area, Answer, Resource, JiangXi
-
-USERDATA = path.DATABASE_PATH / "users.json"
-
-
-class UserModel(BaseModel):
-    id: int = None
-    """用户ID"""
-    time: int = None
-    """添加时间戳"""
-    self_id: int = None
-    """BOT ID"""
-    user_id: int = None
-    """用户ID"""
-    password: str = None
-    """登录密码，用于登录web端"""
-    group_id: int = None
-    """通知群号"""
-    name: str = None
-    """姓名"""
-    gender: str = None
-    """性别"""
-    mobile: str = None
-    """手机号"""
-    area: str = None
-    """地区"""
-    leader: int = None
-    """团支书ID"""
-    openid: str = None
-    """微信认证ID"""
-    dxx_id: str = None
-    """大学习用户id,nid或uid"""
-    university_type: str = None
-    """学校类型"""
-    university_id: str = None
-    """学校id"""
-    university: str = None
-    """学校名称"""
-    college_id: str = None
-    """学院id"""
-    college: str = None
-    """学院名称"""
-    organization_id: str = None
-    """团支部id"""
-    organization: str = None
-    """团支部名称"""
-    token: str = None
-    """提交需要的token"""
-    cookie: str = None
-    """提交要用的cookie"""
-    catalogue: str = None
-    """提交期数"""
-    auto_submit: bool = True
-    """自动提交状态"""
-    commit_time: int = None
-    """提交时间"""
-
-
-SUPERS = get_driver().config.superusers
-AREA = [
-    {
-        "area": "湖北",
-        "host": "cp.fjg360.cn",
-        "referer": None,
-        "origin": None,
-        "url": "https://h5.cyol.com/special/weixin/sign.json",
-        "status": True,
-        "catalogue": None
-    },
-    {
-        "area": "江西",
-        "host": "www.jxqingtuan.cn",
-        "referer": "http://www.jxqingtuan.cn/html/h5_index.html?&accessToken=",
-        "origin": "http://www.jxqingtuan.cn",
-        "url": "http://www.jxqingtuan.cn/pub/vol/volClass/index?userId=4363431",
-        "status": True,
-        "catalogue": None
-    },
-    {
-        "area": "浙江",
-        "host": "qczj.h5yunban.com",
-        "referer": None,
-        "origin": None,
-        "url": "https://qczj.h5yunban.com/qczj-youth-learning/cgi-bin/common-api/course/current?accessToken=",
-        "status": True,
-        "catalogue": None
-    },
-    {
-        "area": "上海",
-        "host": "qcsh.h5yunban.com",
-        "referer": None,
-        "origin": None,
-        "url": "https://qcsh.h5yunban.com/youth-learning/cgi-bin/user-api/course/join?accessToken=",
-        "status": True,
-        "catalogue": None
-    },
-    {
-        "area": "江苏",
-        "host": "service.jiangsugqt.org",
-        "referer": None,
-        "origin": None,
-        "url": "https://service.jiangsugqt.org/youth/lesson/confirm",
-        "status": True,
-        "catalogue": None
-    },
-    {
-        "area": "安徽",
-        "host": "dxx.ahyouth.org.cn",
-        "referer": "http://dxx.ahyouth.org.cn/",
-        "origin": "http://dxx.ahyouth.org.cn",
-        "url": "http://dxx.ahyouth.org.cn/api/hidtoryList",
-        "status": True,
-        "catalogue": None
-    },
-    {
-        "area": "四川",
-        "host": "dxx.scyol.com",
-        "referer": "http://scyol.com/v_prod6.02/",
-        "origin": "http://scyol.com",
-        "url": "https://dxx.scyol.com/api/student/commit",
-        "status": True,
-        "catalogue": None
-    },
-    {
-        "area": "山东",
-        "host": "qndxx.youth54.cn",
-        "referer": "http://qndxx.youth54.cn/SmartLA/dxx.w?method=pageSdtwdt",
-        "origin": "http://qndxx.youth54.cn",
-        "url": "http://qndxx.youth54.cn/SmartLA/dxxjfgl.w?method=getNewestVersionInfo&openid=",
-        "status": True,
-        "catalogue": None
-    },
-    {
-        "area": "重庆",
-        "host": "qndxx.cqyouths.com",
-        "referer": None,
-        "origin": "http://qndxx.cqyouths.com",
-        "url": "http://qndxx.cqyouths.com/new_course.json?time=",
-        "status": True,
-        "catalogue": None
-    },
-    {
-        "area": "吉林",
-        "host": "jqfy.jl54.org",
-        "referer": None,
-        "origin": "http://jqfy.jl54.org/jltw/wechat",
-        "url": "http://jqfy.jl54.org/jltw/wechat",
-        "status": True,
-        "catalogue": None
-    },
-    {
-        "area": "广东",
-        "host": "tuanapi.12355.net",
-        "referer": None,
-        "origin": "https://tuan.12355.net",
-        "url": "https://youthstudy.12355.net/saomah5/api/young/chapter/new",
-        "status": True,
-        "catalogue": None
-    },
-    {
-        "area": "黑龙江",
-        "host": "tsw.ithyxy.com",
-        "referer": None,
-        "origin": "http://tsw.ithyxy.com/login",
-        "url": "http://tsw.ithyxy.com/h5/learn/home",
-        "status": True,
-        "catalogue": None
-    },
-]
-RESOURCE = [
-    {
-        "name": "MiSans-Light.ttf",
-        "url": "",
-        "type": "字体",
-        "size": "7.6 M"
-    }, {
-        "name": "answer.png",
-        "url": "",
-        "type": "答案背景",
-        "size": "860.5 K"
-    },
-    {
-        "name": "backgroud1.jpg",
-        "url": "",
-        "type": "完成截图背景",
-        "size": "51.0 K"
-    }, {
-        "name": "backgroud2.jpg",
-        "url": "",
-        "type": "完成截图背景",
-        "size": "50.9 K"
-    }, {
-        "name": "backgroud3.jpg",
-        "url": "",
-        "type": "完成截图背景",
-        "size": "50.9 K"
-    }, {
-        "name": "backgroud4.jpg",
-        "url": "",
-        "type": "完成截图背景",
-        "size": "50.7 K"
-    }, {
-        "name": "backgroud5.jpg",
-        "url": "",
-        "type": "完成截图背景",
-        "size": "50.4 K"
-    }
-]
-
-export_data = on_command("export_data", aliases={"导出用户数据", "导出数据"}, priority=50, permission=SUPERUSER,
-                         rule=rule.must_command)
-update_users = on_command("update_user", aliases={"更新用户数据", "刷新用户数据"}, priority=50, permission=SUPERUSER,
-                          rule=rule.must_command)
-update_resource = on_command("update_resource", aliases={"更新资源数据", "刷新资源数据"}, priority=50,
-                             permission=SUPERUSER, rule=rule.must_command)
-
-
-@update_resource.got(key="msg", prompt="是否刷新资源数据库信息？（是|否）")
-async def update_resource_(msg: str = ArgStr("msg")) -> None:
-    if msg not in ["是", "yes", "Y", "y", "YES", "true"]:
-        await update_resource.finish(message="操作取消(*^▽^*)", at_sender=True, reply_message=True)
-    else:
-        await update_resource.send("资源重新载入中（请等待1分钟左右）······", at_sender=True, reply_message=True)
-        await JiangXi.all().delete()
-        await Resource.all().delete()
-        await resource_init()
-        await update_resource.finish(message="资源数据载入成功(^_−)☆", at_sender=True, reply_message=True)
-
-
-@export_data.got(key="msg", prompt="是否导出用户数据至TeenStudy目录？（是|否）")
-async def export_user(event: MessageEvent, msg: str = ArgStr("msg")) -> None:
-    self_id = event.self_id
-    if msg not in ["是", "yes", "Y", "y", "YES", "true"]:
-        await export_data.finish(message="操作取消(*^▽^*)", at_sender=True, reply_message=True)
-    else:
-        result = await User.all().values()
-        user_list = []
-        for item in result:
-            data = UserModel().dict()
-            item["self_id"] = self_id
-            data.update(**item)
-            user_list.append(data)
-        with open(USERDATA, "w", encoding="utf-8") as w:
-            json.dump(user_list, w, indent=4, ensure_ascii=False)
-        await export_data.finish(message="用户数据成功导出至TeenStudy目录(*^▽^*)", at_sender=True,
-                                 reply_message=True)
-
-
-@update_users.handle()
-async def update_user() -> None:
-    if not Path(USERDATA).exists():
-        await update_users.finish(
-            message="更新失败，没有找到可导入用户数据文件，请确保TeeStudy数据目录下存有用户数据文件╮(╯﹏╰）╭",
-            at_sender=True, reply_message=True)
-
-
-@update_users.got(key="msg", prompt="是否覆盖更新用户数据?（是|否）")
-async def update_user() -> None:
-    with open(USERDATA, "r", encoding="utf-8") as f:
-        data_obj = json.load(f)
-    await User.all().delete()
-    for item in data_obj:
-        data = UserModel().dict()
-        data.update(**item)
-        await User.create(**data)
-    await update_users.finish(message="用户数据更新完成(*^▽^*)", at_sender=True, reply_message=True)
-
-
-async def plugin_init():
-    for item in AREA:
-        if await Area.filter(area=item['area']).count():
-            continue
-        else:
-            await Area.create(
-                time=time.time(),
-                area=item['area'],
-                host=item['host'],
-                referer=item['referer'],
-                origin=item['origin'],
-                url=item['url'],
-                status=item['status'],
-                catalogue=item['catalogue']
-            )
-
-
-async def admin_init():
-    try:
-        superuser = int(list(get_driver().config.superusers)[0])
-    except AttributeError:
-        superuser = -1
-        logger.error("请配置好超管账号，之后重启nonebot2")
-    try:
-        ip = get_driver().config.dxx_ip
-    except AttributeError:
-        s = socket.socket(socket.AF_INET, socket.SOCK_DGRAM)
-        s.connect(('114.114.114.114', 12345))
-        ip = s.getsockname()[0]
-    result = path.getConfig()
-    if result["DXX_IP"] == ip and result["SUPERUSER"] == superuser:
-        return
-    else:
-        headers = {
-            "User-Agent": "Mozilla/5.0 (Windows NT 10.0; Win64; x64) AppleWebKit/537.36 (KHTML, like Gecko) Chrome/110.0.0.0 Safari/537.36 Edg/110.0.1587.41"
-        }
-        try:
-            logger.opt(colors=True).info(
-                f'<u><y>[大学习数据库]</y></u><g>加载配置公网IP</g>')
-            ip = get_driver().config.dxx_ip
-            logger.opt(colors=True).info(
-                f'<u><y>[大学习数据库]</y></u><g>加载配置公网IP成功，启动检测公网IP访问状态</g>ip:<m>{ip}</m>')
-            url = f"http://{ip}:{get_driver().config.port}/TeenStudy/login"
-            logger.info(url)
-            try:
-                async with AsyncClient(headers=headers) as client:
-                    response = await client.get(url=url)
-                logger.debug(f"公网请求状态：{response.status_code}")
-                if response.status_code != 200:
-                    ip = ""
-                    logger.opt(colors=True).info(
-                        f'<u><y>[大学习数据库]</y></u><g>检测到配置公网ip地址无法通过外网访问，将自动获取公网IP</g>')
-                logger.opt(colors=True).success(
-                    f'<u><y>[大学习提交 Web UI]</y></u><g>配置外网IP设置成功</g>，外网访问地址为:<m>http://{ip}:{get_driver().config.port}/TeenStudy/login</m>')
-            except Exception as e:
-                logger.error(e)
-                ip = ""
-                logger.opt(colors=True).info(
-                    f'<u><y>[大学习数据库]</y></u><g>检测到配置公网ip地址无法通过外网访问，将自动配置局域网IP</g>')
-        except AttributeError:
-            ip = ''
-            logger.opt(colors=True).info(
-                f'<u><y>[大学习数据库]</y></u><g>加载配置IP失败，未检测到配置ip，启动自动获取公网IP</g>')
-        if not ip:
-            async with AsyncClient(headers=headers) as client:
-                response = await client.get("http://ip.42.pl/raw")
-            if response.status_code == 200:
-                ip = response.text.strip()
-                logger.opt(colors=True).info(
-                    f'<u><y>[大学习数据库]</y></u><g>自动获取公网IP成功，启动检测公网IP访问状态</g>ip:<m>{ip}</m>')
-                url = f"http://{ip}:{get_driver().config.port}/TeenStudy/login"
-                logger.info(url)
-                try:
-                    async with AsyncClient(headers=headers, timeout=5) as client:
-                        response = await client.get(url=url)
-                    logger.debug(f"公网请求状态:{response.status_code}")
-                    if response.status_code != 200:
-                        ip = ""
-                        logger.opt(colors=True).warning(
-                            f'<u><y>[大学习数据库]</y></u><g>检测到ip地址无法通过外网访问，将自动配置局域网IP，请手动在.env.prod文件中配置公网IP，配置格式：DXX_IP="您的公网IP"</g>')
-                    else:
-                        logger.opt(colors=True).success(
-                            f'<u><y>[大学习提交 Web UI]</y></u><g>自动获取外网IP成功</g>，外网访问地址为:<m>http://{ip}:{get_driver().config.port}/TeenStudy/login</m>')
-                except Exception as e:
-                    ip = ""
-                    logger.debug(e)
-                    logger.opt(colors=True).warning(
-                        f'<u><y>[大学习数据库]</y></u><g>检测到ip地址无法通过外网访问，将自动配置局域网IP，请手动在.env.prod文件中配置公网IP，配置格式：DXX_IP="您的公网IP"</g>')
-            else:
-                ip = ""
-                logger.opt(colors=True).warning(
-                    f'<u><y>[大学习数据库]</y></u><g>自动获取公网IP失败，将自动配置局域网IP，请手动在.env.prod文件中配置公网IP，配置格式：DXX_IP="您的公网IP"</g>')
-        if not ip:
-            s = socket.socket(socket.AF_INET, socket.SOCK_DGRAM)
-            s.connect(('114.114.114.114', 12345))
-            ip = s.getsockname()[0]
-            logger.opt(colors=True).success(
-                f'<u><y>[大学习提交 Web UI]</y></u><g>配置局域网IP成功</g>，局域网访问地址为:<m>http://{ip}:{get_driver().config.port}/TeenStudy/login</m>')
-        data = {
-            "TOKEN_TIME": 30,
-            "SUPERUSER": int(list(SUPERS)[0]),
-            "KEY": "d82ffad91168fb324ab6ebc2bed8dacd43f5af8e34ad0d1b75d83a0aff966a06",
-            "ALGORITHM": "HS256",
-            "PASSWORD": await to_hash("admin"),
-            "DXX_IP": ip,
-            "DXX_PORT": get_driver().config.port
-        }
-        path.saveConfig(data=data)
-
-
-async def resource_init():
-    base_file_path = os.path.dirname(__file__)[:-5] + "resource/"
-    logger.opt(colors=True).info("<u><y>[大学习数据库]</y></u><g>➤➤➤➤➤检查资源数据✔✔✔✔✔</g>")
-    for item in RESOURCE:
-        if not await Resource.filter(name=item['name']).count():
-            try:
-                with open(base_file_path + item['name'], 'rb') as r:
-                    content = r.read()
-                await Resource.create(
-                    time=time.time(),
-                    name=item['name'],
-                    type=item['type'],
-                    url=item['url'],
-                    size=item['size'],
-                    file=content
-                )
-                logger.opt(colors=True).success(
-                    f"<u><y>[大学习数据库]</y></u> <m>{item['type']}-{item['name']}</m> <g>更新成功!</g>")
-            except Exception as e:
-                logger.success(e)
-                continue
-    try:
-        if not await JiangXi.all().count():
-            with open(base_file_path + "dxx_jx.json", 'r', encoding='utf-8') as r:
-                obj = json.load(r)
-            for item in obj:
-                await JiangXi.create(
-                    time=time.time(),
-                    university_id=item['university_id'],
-                    university=item['university'],
-                    college_id=item['college_id'],
-                    college=item['college'],
-                    organization=item['organization'],
-                    organization_id=item['organization_id']
-                )
-            logger.opt(colors=True).success(
-                f"<u><y>[大学习数据库]</y></u> <m>江西共青团团支部数据</m> <g>更新成功!</g>")
-    except Exception as e:
-        logger.error(e)
-    logger.opt(colors=True).success("<u><y>[大学习数据库]</y></u><g>➤➤➤➤➤资源数据更新完成✔✔✔✔✔</g>")
-
-
-async def get_end_pic():
-    font_data = await Resource.filter(type="字体").values()
-    answer = await Answer.all().order_by('time').values()
-    title = '"青年大学习"' + answer[-1]["catalogue"]
-    backgrouds = await Resource.filter(type="完成截图背景").values()
-    bg_img = Image.open(BytesIO(backgrouds[random.randint(0, 4)]['file']))
-    end_img = Image.open(BytesIO(answer[-1]['cover']))
-    end_img = end_img.resize((1080, 2200), Image.BILINEAR)
-    font = ImageFont.truetype(BytesIO(font_data[0]['file']), 45)
-    img = Image.new('RGB', (end_img.width, bg_img.height), (255, 255, 255))
-    draw = ImageDraw.Draw(img)
-    img.paste(bg_img)
-    time = (datetime.datetime.now() + datetime.timedelta(minutes=random.randint(5, 10))).strftime('%H:%M')
-    draw.text((120, 30), text=time, font=font, fill='black')
-    draw.text((1080 / 2 - (len(title) / 2) * 30, 130), text=title, font=font, fill='black')
-    img.paste(end_img, (0, 200))
-    buf = BytesIO()
-    img.save(buf, format="PNG")
-    base64_str = base64.b64encode(buf.getbuffer()).decode()
-    content = "base64://" + base64_str
-    return content
-
-
-async def get_answer_pic():
-    font_data = await Resource.filter(type="字体").values()
-    answer_result = await Answer.all().order_by('time').values()
-    backgrouds = await Resource.filter(type="答案背景").values()
-    title = answer_result[-1]["catalogue"]
-    answer = answer_result[-1]["answer"]
-    start_time = datetime.datetime.fromtimestamp(answer_result[-1]['time']).strftime(
-        "%Y年%m月%d日 %H:%M:%S")
-    end_day = (datetime.datetime.fromtimestamp(answer_result[-1]["time"]) + datetime.timedelta(
-        days=7)).strftime("%Y年%m月%d日")
-    end_time = f'{end_day} 22:00:00'
-    answer_bg = Image.open(BytesIO(backgrouds[0]['file']))
-    img = Image.new('RGB', (902, 987), (255, 255, 255))
-    img.paste(answer_bg)
-    draw = ImageDraw.Draw(img)
-    font = ImageFont.truetype(BytesIO(font_data[0]['file']), 55)
-    draw.text((20, 20), text='青年大学习主题团课', fill='gold', font=font)
-    font = ImageFont.truetype(BytesIO(font_data[0]['file']), 48)
-    draw.text((20, 100), text=title, fill='gold', font=font)
-    font = ImageFont.truetype(BytesIO(font_data[0]['file']), 40)
-    draw.text((20, 180), fill='gold', font=font, text=answer)
-    font = ImageFont.truetype(BytesIO(font_data[0]['file']), 40)
-    draw.text((410, 550), fill='gold', font=font, text=start_time)
-    font = ImageFont.truetype(BytesIO(font_data[0]['file']), 40)
-    draw.text((410, 650), fill='gold', font=font, text=end_time)
-    font = ImageFont.truetype(BytesIO(font_data[0]['file']), 40)
-    draw.text((550, 500), text='开始时间', fill='gold', font=font)
-    font = ImageFont.truetype(BytesIO(font_data[0]['file']), 40)
-    draw.text((550, 600), text='结束时间', fill='gold', font=font)
-    buf = BytesIO()
-    img.save(buf, format="PNG")
-    base64_str = base64.b64encode(buf.getbuffer()).decode()
-    content = "base64://" + base64_str
-    return content
-
-
-async def to_hash(text: str) -> str:
-    return hashlib.sha256(text.encode("utf-8")).hexdigest()
-
-
-async def distribute_area(user_id: int, area: str) -> dict:
-    if area == "湖北":
-        return await dxx.hubei(user_id=user_id)
-    elif area == "江西":
-        return await dxx.jiangxi(user_id=user_id)
-    elif area == "浙江":
-        return await dxx.zhejiang(user_id=user_id)
-    elif area == "上海":
-        return await dxx.shanghai(user_id=user_id)
-    elif area == "江苏":
-        return await dxx.jiangsu(user_id=user_id)
-    elif area == "安徽":
-        return await dxx.anhui(user_id=user_id)
-    elif area == "四川":
-        return await dxx.sichuan(user_id=user_id)
-    elif area == "山东":
-        return await dxx.shandong(user_id=user_id)
-    elif area == "重庆":
-        return await dxx.chongqing(user_id=user_id)
-    elif area == "吉林":
-        return await dxx.jilin(user_id=user_id)
-    elif area == "广东":
-        return await dxx.guangdong(user_id=user_id)
-    elif area == "黑龙江":
-        return await dxx.heilongjiang(user_id=user_id)
-    else:
-        return {
-            "status": 404,
-            "msg": "该地区暂未支持！"
-        }
-
-
-async def distribute_area_url(province: str, user_id: int, group_id: int) -> dict:
-    config = path.getConfig()
-    if province == "湖北":
-        province = "hubei"
-    elif province == "江西":
-        province = "jiangxi"
-    elif province == "江苏":
-        province = "jiangsu"
-    elif province == "安徽":
-        province = "anhui"
-    elif province == "四川":
-        province = "sichuan"
-    elif province == "山东":
-        province = "shandong"
-    elif province == "重庆":
-        province = "chongqing"
-    elif province == "吉林":
-        province = "jilin"
-    elif province == "广东":
-        province="guangdong"
-    elif province == "黑龙江":
-        province = "heilongjiang"
-    data = f"http://{config['DXX_IP']}:{config['DXX_PORT']}/TeenStudy/api/{province}?user_id={user_id}&group_id={group_id}"
-    img = qrcode.make(data=data)
-    buf = BytesIO()
-    img.save(buf, format="PNG")
-    base64_str = base64.b64encode(buf.getbuffer()).decode()
-    content = "base64://" + base64_str
-    return {
-        "url": data,
-        "content": content
-    }
-
-
-async def get_login_qrcode() -> dict:
-    config = path.getConfig()
-    data = f'http://{config["DXX_IP"]}:{config["DXX_PORT"]}/TeenStudy/login'
-    img = qrcode.make(data=data)
-    buf = BytesIO()
-    img.save(buf, format="PNG")
-    base64_str = base64.b64encode(buf.getbuffer()).decode()
-    content = "base64://" + base64_str
-    return {
-        "url": data,
-        "content": content
-    }
-
-
-async def get_qrcode(user_id: int, group_id: int, area: str) -> dict:
-    config = path.getConfig()
-    if area == "浙江":
-        data = f"https://open.weixin.qq.com/connect/oauth2/authorize?appid=wx56b888a1409a2920&redirect_uri=https://wx.yunban.cn/wx/oauthInfoCallback?r_uri=http://{config['DXX_IP']}:{config['DXX_PORT']}/TeenStudy/api/zhejiang/{user_id}/{group_id}&source=common&response_type=code&scope=snsapi_userinfo&state=STATE&component_appid=wx0f0063354bfd3d19&connect_redirect=1"
-    else:
-        data = f"https://open.weixin.qq.com/connect/oauth2/authorize?appid=wxa693f4127cc93fad&redirect_uri=https://wx.yunban.cn/wx/oauthInfoCallback?r_uri=http://{config['DXX_IP']}:{config['DXX_PORT']}/TeenStudy/api/shanghai/{user_id}/{group_id}&source=common&response_type=code&scope=snsapi_userinfo&state=STATE&component_appid=wx0f0063354bfd3d19&connect_redirect=1"
-    img = qrcode.make(data=data)
-    buf = BytesIO()
-    img.save(buf, format="PNG")
-    base64_str = base64.b64encode(buf.getbuffer()).decode()
-    content = "base64://" + base64_str
-    return {
-        "url": data,
-        "content": content
-    }
+import base64
+import datetime
+import hashlib
+import json
+import os
+import random
+import socket
+import time
+from io import BytesIO
+from pathlib import Path
+
+import qrcode
+from Crypto.Cipher import PKCS1_v1_5
+from Crypto.PublicKey import RSA
+from PIL import Image, ImageDraw, ImageFont
+from httpx import AsyncClient
+from nonebot import logger, get_driver, on_command
+from nonebot.adapters.onebot.v11 import MessageEvent
+from nonebot.params import ArgStr
+from nonebot.permission import SUPERUSER
+from pydantic import BaseModel
+
+from . import dxx, path, rule
+from ..models.accuont import User
+from ..models.dxx import Area, Answer, Resource
+
+USERDATA = path.DATABASE_PATH / "users.json"
+
+
+class UserModel(BaseModel):
+    id: int = None
+    """用户ID"""
+    time: int = None
+    """添加时间戳"""
+    self_id: int = None
+    """BOT ID"""
+    user_id: int = None
+    """用户ID"""
+    password: str = None
+    """登录密码，用于登录web端"""
+    group_id: int = None
+    """通知群号"""
+    name: str = None
+    """姓名"""
+    gender: str = None
+    """性别"""
+    mobile: str = None
+    """手机号"""
+    area: str = None
+    """地区"""
+    leader: int = None
+    """团支书ID"""
+    openid: str = None
+    """微信认证ID"""
+    dxx_id: str = None
+    """大学习用户id,nid或uid"""
+    university_type: str = None
+    """学校类型"""
+    university_id: str = None
+    """学校id"""
+    university: str = None
+    """学校名称"""
+    college_id: str = None
+    """学院id"""
+    college: str = None
+    """学院名称"""
+    organization_id: str = None
+    """团支部id"""
+    organization: str = None
+    """团支部名称"""
+    token: str = None
+    """提交需要的token"""
+    cookie: str = None
+    """提交要用的cookie"""
+    catalogue: str = None
+    """提交期数"""
+    auto_submit: bool = True
+    """自动提交状态"""
+    commit_time: int = None
+    """提交时间"""
+
+
+SUPERS = get_driver().config.superusers
+AREA = [
+    {
+        "area": "湖北",
+        "host": "cp.fjg360.cn",
+        "referer": None,
+        "origin": None,
+        "url": "https://h5.cyol.com/special/weixin/sign.json",
+        "status": True,
+        "catalogue": None
+    },
+    {
+        "area": "江西",
+        "host": "www.jxqingtuan.cn",
+        "referer": "http://www.jxqingtuan.cn/html/h5_index.html?&accessToken=",
+        "origin": "http://www.jxqingtuan.cn",
+        "url": "http://www.jxqingtuan.cn/pub/vol/volClass/index?userId=4363431",
+        "status": True,
+        "catalogue": None
+    },
+    {
+        "area": "浙江",
+        "host": "qczj.h5yunban.com",
+        "referer": None,
+        "origin": None,
+        "url": "https://qczj.h5yunban.com/qczj-youth-learning/cgi-bin/common-api/course/current?accessToken=",
+        "status": True,
+        "catalogue": None
+    },
+    {
+        "area": "上海",
+        "host": "qcsh.h5yunban.com",
+        "referer": None,
+        "origin": None,
+        "url": "https://qcsh.h5yunban.com/youth-learning/cgi-bin/user-api/course/join?accessToken=",
+        "status": True,
+        "catalogue": None
+    },
+    {
+        "area": "安徽",
+        "host": "dxx.ahyouth.org.cn",
+        "referer": "http://dxx.ahyouth.org.cn/",
+        "origin": "http://dxx.ahyouth.org.cn",
+        "url": "http://dxx.ahyouth.org.cn/api/hidtoryList",
+        "status": True,
+        "catalogue": None
+    },
+    {
+        "area": "四川",
+        "host": "dxx.scyol.com",
+        "referer": "http://scyol.com/v_prod6.02/",
+        "origin": "http://scyol.com",
+        "url": "https://dxx.scyol.com/api/student/commit",
+        "status": True,
+        "catalogue": None
+    },
+    {
+        "area": "山东",
+        "host": "qndxx.youth54.cn",
+        "referer": "http://qndxx.youth54.cn/SmartLA/dxx.w?method=pageSdtwdt",
+        "origin": "http://qndxx.youth54.cn",
+        "url": "http://qndxx.youth54.cn/SmartLA/dxxjfgl.w?method=getNewestVersionInfo&openid=",
+        "status": True,
+        "catalogue": None
+    },
+    {
+        "area": "重庆",
+        "host": "qndxx.cqyouths.com",
+        "referer": None,
+        "origin": "http://qndxx.cqyouths.com",
+        "url": "http://qndxx.cqyouths.com/new_course.json?time=",
+        "status": True,
+        "catalogue": None
+    },
+    {
+        "area": "吉林",
+        "host": "jqfy.jl54.org",
+        "referer": None,
+        "origin": "http://jqfy.jl54.org/jltw/wechat",
+        "url": "http://jqfy.jl54.org/jltw/wechat",
+        "status": True,
+        "catalogue": None
+    },
+    {
+        "area": "广东",
+        "host": "tuanapi.12355.net",
+        "referer": None,
+        "origin": "https://tuan.12355.net",
+        "url": "https://youthstudy.12355.net/saomah5/api/young/chapter/new",
+        "status": True,
+        "catalogue": None
+    },
+    {
+        "area": "北京",
+        "host": "m.bjyouth.net",
+        "referer": None,
+        "origin": "https://m.bjyouth.net",
+        "url": "https://m.bjyouth.net/dxx/index",
+        "status": True,
+        "catalogue": None
+    },
+    {
+        "area": "天津",
+        "host": "admin.ddy.tjyun.com",
+        "referer": None,
+        "origin": "https://admin.ddy.tjyun.com",
+        "url": "http://admin.ddy.tjyun.com/zm/jump/1",
+        "status": True,
+        "catalogue": None
+    },
+]
+RESOURCE = [
+    {
+        "name": "MiSans-Light.ttf",
+        "url": "",
+        "type": "字体",
+        "size": "7.6 M"
+    }, {
+        "name": "answer.png",
+        "url": "",
+        "type": "答案背景",
+        "size": "860.5 K"
+    },
+    {
+        "name": "backgroud1.jpg",
+        "url": "",
+        "type": "完成截图背景",
+        "size": "51.0 K"
+    }, {
+        "name": "backgroud2.jpg",
+        "url": "",
+        "type": "完成截图背景",
+        "size": "50.9 K"
+    }, {
+        "name": "backgroud3.jpg",
+        "url": "",
+        "type": "完成截图背景",
+        "size": "50.9 K"
+    }, {
+        "name": "backgroud4.jpg",
+        "url": "",
+        "type": "完成截图背景",
+        "size": "50.7 K"
+    }, {
+        "name": "backgroud5.jpg",
+        "url": "",
+        "type": "完成截图背景",
+        "size": "50.4 K"
+    }
+]
+
+export_data = on_command("export_data", aliases={"导出用户数据", "导出数据"}, priority=50, permission=SUPERUSER,
+                         rule=rule.must_command)
+update_users = on_command("update_user", aliases={"更新用户数据", "刷新用户数据"}, priority=50, permission=SUPERUSER,
+                          rule=rule.must_command)
+update_resource = on_command("update_resource", aliases={"更新资源数据", "刷新资源数据"}, priority=50,
+                             permission=SUPERUSER, rule=rule.must_command)
+
+
+@update_resource.got(key="msg", prompt="是否刷新资源数据库信息？（是|否）")
+async def update_resource_(msg: str = ArgStr("msg")) -> None:
+    if msg not in ["是", "yes", "Y", "y", "YES", "true"]:
+        await update_resource.finish(message="操作取消(*^▽^*)", at_sender=True, reply_message=True)
+    else:
+        await update_resource.send("资源重新载入中（请等待1分钟左右）······", at_sender=True, reply_message=True)
+        await Resource.all().delete()
+        await resource_init()
+        await update_resource.finish(message="资源数据载入成功(^_−)☆", at_sender=True, reply_message=True)
+
+
+@export_data.got(key="msg", prompt="是否导出用户数据至TeenStudy目录？（是|否）")
+async def export_user(event: MessageEvent, msg: str = ArgStr("msg")) -> None:
+    self_id = event.self_id
+    if msg not in ["是", "yes", "Y", "y", "YES", "true"]:
+        await export_data.finish(message="操作取消(*^▽^*)", at_sender=True, reply_message=True)
+    else:
+        result = await User.all().values()
+        user_list = []
+        for item in result:
+            data = UserModel().dict()
+            item["self_id"] = self_id
+            data.update(**item)
+            user_list.append(data)
+        with open(USERDATA, "w", encoding="utf-8") as w:
+            json.dump(user_list, w, indent=4, ensure_ascii=False)
+        await export_data.finish(message="用户数据成功导出至TeenStudy目录(*^▽^*)", at_sender=True,
+                                 reply_message=True)
+
+
+@update_users.handle()
+async def update_user() -> None:
+    if not Path(USERDATA).exists():
+        await update_users.finish(
+            message="更新失败，没有找到可导入用户数据文件，请确保TeeStudy数据目录下存有用户数据文件╮(╯﹏╰）╭",
+            at_sender=True, reply_message=True)
+
+
+@update_users.got(key="msg", prompt="是否覆盖更新用户数据?（是|否）")
+async def update_user() -> None:
+    with open(USERDATA, "r", encoding="utf-8") as f:
+        data_obj = json.load(f)
+    await User.all().delete()
+    for item in data_obj:
+        data = UserModel().dict()
+        data.update(**item)
+        await User.create(**data)
+    await update_users.finish(message="用户数据更新完成(*^▽^*)", at_sender=True, reply_message=True)
+
+
+async def plugin_init():
+    for item in AREA:
+        if await Area.filter(area=item['area']).count():
+            continue
+        else:
+            await Area.create(
+                time=time.time(),
+                area=item['area'],
+                host=item['host'],
+                referer=item['referer'],
+                origin=item['origin'],
+                url=item['url'],
+                status=item['status'],
+                catalogue=item['catalogue']
+            )
+
+
+async def admin_init():
+    try:
+        superuser = int(list(get_driver().config.superusers)[0])
+    except AttributeError:
+        superuser = -1
+        logger.error("请配置好超管账号，之后重启nonebot2")
+    try:
+        ip = get_driver().config.dxx_ip
+    except AttributeError:
+        s = socket.socket(socket.AF_INET, socket.SOCK_DGRAM)
+        s.connect(('114.114.114.114', 12345))
+        ip = s.getsockname()[0]
+    result = path.getConfig()
+    if result["DXX_IP"] == ip and result["SUPERUSER"] == superuser:
+        return
+    else:
+        headers = {
+            "User-Agent": "Mozilla/5.0 (Windows NT 10.0; Win64; x64) AppleWebKit/537.36 (KHTML, like Gecko) Chrome/110.0.0.0 Safari/537.36 Edg/110.0.1587.41"
+        }
+        try:
+            logger.opt(colors=True).info(
+                f'<u><y>[大学习数据库]</y></u><g>加载配置公网IP</g>')
+            ip = get_driver().config.dxx_ip
+            logger.opt(colors=True).info(
+                f'<u><y>[大学习数据库]</y></u><g>加载配置公网IP成功，启动检测公网IP访问状态</g>ip:<m>{ip}</m>')
+        except AttributeError:
+            ip = ''
+            logger.opt(colors=True).info(
+                f'<u><y>[大学习数据库]</y></u><g>加载配置IP失败，未检测到配置ip，启动自动获取公网IP</g>')
+        if not ip:
+            async with AsyncClient(headers=headers) as client:
+                response = await client.get("http://ip.42.pl/raw")
+            if response.status_code == 200:
+                ip = response.text.strip()
+                logger.opt(colors=True).info(
+                    f'<u><y>[大学习数据库]</y></u><g>自动获取公网IP成功</g>ip:<m>{ip}</m>')
+            else:
+                ip = ""
+                logger.opt(colors=True).warning(
+                    f'<u><y>[大学习数据库]</y></u><g>自动获取公网IP失败，将自动配置局域网IP，请手动在.env.prod文件中配置公网IP，配置格式：DXX_IP="您的公网IP"</g>')
+        if not ip:
+            s = socket.socket(socket.AF_INET, socket.SOCK_DGRAM)
+            s.connect(('114.114.114.114', 12345))
+            ip = s.getsockname()[0]
+            logger.opt(colors=True).success(
+                f'<u><y>[大学习提交 Web UI]</y></u><g>配置局域网IP成功</g>，局域网访问地址为:<m>http://{ip}:{get_driver().config.port}/TeenStudy/login</m>')
+        data = {
+            "TOKEN_TIME": 30,
+            "SUPERUSER": int(list(SUPERS)[0]),
+            "KEY": "d82ffad91168fb324ab6ebc2bed8dacd43f5af8e34ad0d1b75d83a0aff966a06",
+            "ALGORITHM": "HS256",
+            "PASSWORD": await to_hash("admin"),
+            "DXX_IP": ip,
+            "DXX_PORT": get_driver().config.port
+        }
+        path.saveConfig(data=data)
+
+
+async def resource_init():
+    base_file_path = os.path.dirname(__file__)[:-5] + "resource/"
+    logger.opt(colors=True).info("<u><y>[大学习数据库]</y></u><g>➤➤➤➤➤检查资源数据✔✔✔✔✔</g>")
+    for item in RESOURCE:
+        if not await Resource.filter(name=item['name']).count():
+            try:
+                with open(base_file_path + item['name'], 'rb') as r:
+                    content = r.read()
+                await Resource.create(
+                    time=time.time(),
+                    name=item['name'],
+                    type=item['type'],
+                    url=item['url'],
+                    size=item['size'],
+                    file=content
+                )
+                logger.opt(colors=True).success(
+                    f"<u><y>[大学习数据库]</y></u> <m>{item['type']}-{item['name']}</m> <g>更新成功!</g>")
+            except Exception as e:
+                logger.success(e)
+                continue
+    logger.opt(colors=True).success("<u><y>[大学习数据库]</y></u><g>➤➤➤➤➤资源数据更新完成✔✔✔✔✔</g>")
+
+
+async def get_end_pic():
+    font_data = await Resource.filter(type="字体").values()
+    answer = await Answer.all().order_by('time').values()
+    title = '"青年大学习"' + answer[-1]["catalogue"]
+    backgrouds = await Resource.filter(type="完成截图背景").values()
+    bg_img = Image.open(BytesIO(backgrouds[random.randint(0, 4)]['file']))
+    end_img = Image.open(BytesIO(answer[-1]['cover']))
+    end_img = end_img.resize((1080, 2200), Image.BILINEAR)
+    font = ImageFont.truetype(BytesIO(font_data[0]['file']), 45)
+    img = Image.new('RGB', (end_img.width, bg_img.height), (255, 255, 255))
+    draw = ImageDraw.Draw(img)
+    img.paste(bg_img)
+    time = (datetime.datetime.now() + datetime.timedelta(minutes=random.randint(5, 10))).strftime('%H:%M')
+    draw.text((120, 30), text=time, font=font, fill='black')
+    draw.text((1080 / 2 - (len(title) / 2) * 30, 130), text=title, font=font, fill='black')
+    img.paste(end_img, (0, 200))
+    buf = BytesIO()
+    img.save(buf, format="PNG")
+    base64_str = base64.b64encode(buf.getbuffer()).decode()
+    content = "base64://" + base64_str
+    return content
+
+
+async def get_answer_pic():
+    font_data = await Resource.filter(type="字体").values()
+    answer_result = await Answer.all().order_by('time').values()
+    backgrouds = await Resource.filter(type="答案背景").values()
+    title = answer_result[-1]["catalogue"]
+    answer = answer_result[-1]["answer"]
+    start_time = datetime.datetime.fromtimestamp(answer_result[-1]['time']).strftime(
+        "%Y年%m月%d日 %H:%M:%S")
+    end_day = (datetime.datetime.fromtimestamp(answer_result[-1]["time"]) + datetime.timedelta(
+        days=7)).strftime("%Y年%m月%d日")
+    end_time = f'{end_day} 22:00:00'
+    answer_bg = Image.open(BytesIO(backgrouds[0]['file']))
+    img = Image.new('RGB', (902, 987), (255, 255, 255))
+    img.paste(answer_bg)
+    draw = ImageDraw.Draw(img)
+    font = ImageFont.truetype(BytesIO(font_data[0]['file']), 55)
+    draw.text((20, 20), text='青年大学习主题团课', fill='gold', font=font)
+    font = ImageFont.truetype(BytesIO(font_data[0]['file']), 48)
+    draw.text((20, 100), text=title, fill='gold', font=font)
+    font = ImageFont.truetype(BytesIO(font_data[0]['file']), 40)
+    draw.text((20, 180), fill='gold', font=font, text=answer)
+    font = ImageFont.truetype(BytesIO(font_data[0]['file']), 40)
+    draw.text((410, 550), fill='gold', font=font, text=start_time)
+    font = ImageFont.truetype(BytesIO(font_data[0]['file']), 40)
+    draw.text((410, 650), fill='gold', font=font, text=end_time)
+    font = ImageFont.truetype(BytesIO(font_data[0]['file']), 40)
+    draw.text((550, 500), text='开始时间', fill='gold', font=font)
+    font = ImageFont.truetype(BytesIO(font_data[0]['file']), 40)
+    draw.text((550, 600), text='结束时间', fill='gold', font=font)
+    buf = BytesIO()
+    img.save(buf, format="PNG")
+    base64_str = base64.b64encode(buf.getbuffer()).decode()
+    content = "base64://" + base64_str
+    return content
+
+
+async def to_hash(text: str) -> str:
+    """
+    哈希散列加密
+    :param text:待加密文本
+    :return: 加密文本
+    """
+    return hashlib.sha256(text.encode("utf-8")).hexdigest()
+
+
+async def encrypt(text: str):
+    """
+    RSA加密
+    :param text: 待加密文本
+    :return: 加密文本
+    """
+    public_key = "-----BEGIN PUBLIC KEY-----\nMIGfMA0GCSqGSIb3DQEBAQUAA4GNADCBiQKBgQD5uIDebA2qU746e/NVPiQSBA0Q3J8/G23zfrwMz4qoip1vuKaVZykuMtsAkCJFZhEcmuaOVl8nAor7cz/KZe8ZCNInbXp2kUQNjJiOPwEhkGiVvxvU5V5vCK4mzGZhhawF5cI/pw2GJDSKbXK05YHXVtOAmg17zB1iJf+ie28TbwIDAQAB\n-----END PUBLIC KEY-----"
+    rsa_key = RSA.importKey(public_key)
+    cipher = PKCS1_v1_5.new(rsa_key)
+    cipher_text = base64.b64encode(cipher.encrypt(text.encode()))
+    return cipher_text.decode()
+
+
+async def distribute_area(user_id: int, area: str) -> dict:
+    if area == "湖北":
+        return await dxx.hubei(user_id=user_id)
+    elif area == "江西":
+        return await dxx.jiangxi(user_id=user_id)
+    elif area == "浙江":
+        return await dxx.zhejiang(user_id=user_id)
+    elif area == "上海":
+        return await dxx.shanghai(user_id=user_id)
+    elif area == "安徽":
+        return await dxx.anhui(user_id=user_id)
+    elif area == "四川":
+        return await dxx.sichuan(user_id=user_id)
+    elif area == "山东":
+        return await dxx.shandong(user_id=user_id)
+    elif area == "重庆":
+        return await dxx.chongqing(user_id=user_id)
+    elif area == "吉林":
+        return await dxx.jilin(user_id=user_id)
+    elif area == "广东":
+        return await dxx.guangdong(user_id=user_id)
+    elif area == "北京":
+        return await dxx.beijing(user_id=user_id)
+    elif area == "天津":
+        return await dxx.tianjin(user_id=user_id)
+    else:
+        return {
+            "status": 404,
+            "msg": "该地区暂未支持！"
+        }
+
+
+async def distribute_area_url(province: str, user_id: int, group_id: int) -> dict:
+    config = path.getConfig()
+    if province == "湖北":
+        province = "hubei"
+    elif province == "江西":
+        province = "jiangxi"
+    elif province == "安徽":
+        province = "anhui"
+    elif province == "四川":
+        province = "sichuan"
+    elif province == "山东":
+        province = "shandong"
+    elif province == "重庆":
+        province = "chongqing"
+    elif province == "吉林":
+        province = "jilin"
+    elif province == "广东":
+        province = "guangdong"
+    elif province == "北京":
+        province = "beijing"
+    elif province == "天津":
+        province = "tianjin"
+    data = f"http://{config['DXX_IP']}:{config['DXX_PORT']}/TeenStudy/api/{province}?user_id={user_id}&group_id={group_id}"
+    img = qrcode.make(data=data)
+    buf = BytesIO()
+    img.save(buf, format="PNG")
+    base64_str = base64.b64encode(buf.getbuffer()).decode()
+    content = "base64://" + base64_str
+    return {
+        "url": data,
+        "content": content
+    }
+
+
+async def get_login_qrcode() -> dict:
+    config = path.getConfig()
+    data = f'http://{config["DXX_IP"]}:{config["DXX_PORT"]}/TeenStudy/login'
+    img = qrcode.make(data=data)
+    buf = BytesIO()
+    img.save(buf, format="PNG")
+    base64_str = base64.b64encode(buf.getbuffer()).decode()
+    content = "base64://" + base64_str
+    return {
+        "url": data,
+        "content": content
+    }
+
+
+async def get_qrcode(user_id: int, group_id: int, area: str) -> dict:
+    config = path.getConfig()
+    if area == "浙江":
+        data = f"https://open.weixin.qq.com/connect/oauth2/authorize?appid=wx56b888a1409a2920&redirect_uri=https://wx.yunban.cn/wx/oauthInfoCallback?r_uri=http://{config['DXX_IP']}:{config['DXX_PORT']}/TeenStudy/api/zhejiang/{user_id}/{group_id}&source=common&response_type=code&scope=snsapi_userinfo&state=STATE&component_appid=wx0f0063354bfd3d19&connect_redirect=1"
+    else:
+        data = f"https://open.weixin.qq.com/connect/oauth2/authorize?appid=wxa693f4127cc93fad&redirect_uri=https://wx.yunban.cn/wx/oauthInfoCallback?r_uri=http://{config['DXX_IP']}:{config['DXX_PORT']}/TeenStudy/api/shanghai/{user_id}/{group_id}&source=common&response_type=code&scope=snsapi_userinfo&state=STATE&component_appid=wx0f0063354bfd3d19&connect_redirect=1"
+    img = qrcode.make(data=data)
+    buf = BytesIO()
+    img.save(buf, format="PNG")
+    base64_str = base64.b64encode(buf.getbuffer()).decode()
+    content = "base64://" + base64_str
+    return {
+        "url": data,
+        "content": content
+    }
```

### Comparing `TeenStudy-0.1.9/TeenStudy/web/__init__.py` & `teenstudy-0.2.0rc1/TeenStudy/web/__init__.py`

 * *Files 17% similar despite different names*

```diff
@@ -1,65 +1,67 @@
-import nonebot
-from fastapi import FastAPI
-from fastapi.responses import HTMLResponse
-from nonebot import get_driver
-from nonebot.log import logger
-
-from . import api, pages, utils
-from .pages.admin import admin_app
-from .pages.home import home_app
-from .pages.login import login_page
-
-requestAdaptor = '''
-requestAdaptor(api) {
-    api.headers["token"] = localStorage.getItem("token");
-    api.headers["role"] = localStorage.getItem("role");
-    api.headers["user_id"] = localStorage.getItem("user_id");
-    return api;
-},
-'''
-responseAdaptor = '''
-responseAdaptor(api, payload, query, request, response) {
-    if (response.data.detail == '登录验证失败或已失效，请重新登录') {
-        window.location.href = '/TeenStudy/login'
-        window.localStorage.clear()
-        window.sessionStorage.clear()
-        window.alert('登录验证失败或已失效，请重新登录')
-    }
-    return payload
-},
-'''
-DRIVER = get_driver()
-icon_path = 'https://i.328888.xyz/2023/02/23/xIh5k.png'
-
-
-@DRIVER.on_startup
-async def init_web():
-    app: FastAPI = nonebot.get_app()
-    logger.opt(colors=True).info(
-        f'<u><y>[大学习提交 Web UI]</y></u><g>启用成功</g>，本机访问地址为:<m>http://127.0.0.1:{DRIVER.config.port}/TeenStudy/login</m>')
-    app.include_router(api.BaseApiRouter)
-
-    @app.get("/TeenStudy/login", response_class=HTMLResponse)
-    async def login():
-        return login_page.render(
-            site_title='TeenStudy | 登录',
-            site_icon=icon_path
-        )
-
-    @app.get('/TeenStudy/home', response_class=HTMLResponse)
-    async def home(user_id: int):
-        return home_app.render(
-            site_title='TeenStudy 首页',
-            site_icon=icon_path,
-            requestAdaptor=requestAdaptor,
-            responseAdaptor=responseAdaptor
-        )
-
-    @app.get("/TeenStudy/admin", response_class=HTMLResponse)
-    async def admin():
-        return admin_app.render(
-            site_title='TeenStudy | 管理后台',
-            site_icon=icon_path,
-            requestAdaptor=requestAdaptor,
-            responseAdaptor=responseAdaptor
-        )
+import nonebot
+from fastapi import FastAPI
+from fastapi.responses import HTMLResponse
+from nonebot import get_driver
+from nonebot.log import logger
+
+from . import api, pages, utils
+from .pages.admin import admin_app
+from .pages.home import home_app
+from .pages.login import login_page
+
+requestAdaptor = '''
+requestAdaptor(api) {
+    api.headers["token"] = localStorage.getItem("token");
+    api.headers["role"] = localStorage.getItem("role");
+    api.headers["user_id"] = localStorage.getItem("user_id");
+    return api;
+},
+'''
+responseAdaptor = '''
+responseAdaptor(api, payload, query, request, response) {
+    if (response.data.detail == '登录验证失败或已失效，请重新登录') {
+        window.location.href = '/TeenStudy/login'
+        window.localStorage.clear()
+        window.sessionStorage.clear()
+        window.alert('登录验证失败或已失效，请重新登录')
+    }
+    return payload
+},
+'''
+DRIVER = get_driver()
+icon_path = 'https://img1.imgtp.com/2023/06/11/sG4KdlpL.png'
+
+
+@DRIVER.on_startup
+async def init_web():
+    app: FastAPI = nonebot.get_app()
+    logger.opt(colors=True).info(
+        f'<u><y>[大学习提交 Web UI]</y></u><g>启用成功</g>，本机访问地址为:<m>http://127.0.0.1:{DRIVER.config.port}/TeenStudy/login</m>')
+    app.include_router(api.BaseApiRouter)
+
+    @app.get("/TeenStudy/login", response_class=HTMLResponse)
+    async def login():
+        return login_page.render(
+            site_title='TeenStudy | 登录',
+            site_icon=icon_path
+        )
+
+    @app.get('/TeenStudy/home', response_class=HTMLResponse)
+    async def home():
+        return home_app.render(
+            site_title='TeenStudy 首页',
+            site_icon=icon_path,
+            routerModel="createBrowserHistory",
+            requestAdaptor=requestAdaptor,
+            responseAdaptor=responseAdaptor
+        )
+
+    @app.get("/TeenStudy/admin", response_class=HTMLResponse)
+    async def admin():
+        return admin_app.render(
+            site_title='TeenStudy | 管理后台',
+            site_icon=icon_path,
+            routerModel="createBrowserHistory",
+            requestAdaptor=requestAdaptor,
+            responseAdaptor=responseAdaptor
+        )
```

### Comparing `TeenStudy-0.1.9/TeenStudy/web/api/admin.py` & `teenstudy-0.2.0rc1/TeenStudy/web/api/admin.py`

 * *Ordering differences only*

 * *Files 20% similar despite different names*

```diff
@@ -1,332 +1,332 @@
-import time
-from typing import Optional
-import datetime
-from fastapi import APIRouter
-from fastapi.responses import JSONResponse
-from nonebot import logger, get_bot
-from nonebot.adapters.onebot.v11.bot import Bot
-
-from .login import admin_authentication
-from ..utils.status import get_status
-from ...models.accuont import Commit, AddUser, User
-from ...models.dxx import Answer, PushList
-from ...utils.utils import to_hash
-from ...utils.path import getConfig, saveConfig
-
-route = APIRouter()
-
-
-@route.get('/status', response_class=JSONResponse, dependencies=[admin_authentication()])
-async def status():
-    return await get_status()
-
-
-@route.delete("/delete_all", response_class=JSONResponse, dependencies=[admin_authentication()])
-async def delete_all(type: str) -> JSONResponse:
-    if type == "records":
-        await Commit.all().delete()
-    elif type == "answers":
-        await Answer.all().delete()
-    elif type == "requests":
-        await AddUser.all().delete()
-    else:
-        return JSONResponse({"status": 500, "msg": "删除失败！"})
-    return JSONResponse({"status": 0, "msg": "删除成功！"})
-
-
-@route.delete("/delete_record", response_class=JSONResponse, dependencies=[admin_authentication()])
-async def delete_record(id: int) -> JSONResponse:
-    try:
-        await Commit.filter(id=id).delete()
-        return JSONResponse({
-            "status": 0,
-            "msg": "删除成功！"
-        })
-    except Exception as e:
-        logger.error(e)
-        return JSONResponse({
-            "status": 500,
-            "msg": "删除失败！"
-        })
-
-
-@route.delete("/delete_records", response_class=JSONResponse, dependencies=[admin_authentication()])
-async def delete_records(ids: str) -> JSONResponse:
-    for id in ids.split(","):
-        await Commit.filter(id=id).delete()
-    return JSONResponse({
-        "status": 0, "msg": "删除成功！"
-    })
-
-
-@route.delete("/delete_answer", response_class=JSONResponse, dependencies=[admin_authentication()])
-async def delete_answer(id: int) -> JSONResponse:
-    try:
-        await Answer.filter(id=id).delete()
-        return JSONResponse({
-            "status": 0,
-            "msg": "删除成功！"
-        })
-    except Exception as e:
-        logger.error(e)
-        return JSONResponse({
-            "status": 500,
-            "msg": "删除失败！"
-        })
-
-
-@route.delete("/delete_answers", response_class=JSONResponse, dependencies=[admin_authentication()])
-async def delete_answers(ids: str) -> JSONResponse:
-    for id in ids.split(","):
-        await Answer.filter(id=id).delete()
-    return JSONResponse({"status": 0, "msg": "删除成功！"})
-
-
-@route.get("/get_settings", response_class=JSONResponse, dependencies=[admin_authentication()])
-async def get_answers() -> JSONResponse:
-    result = getConfig()
-    result["auto"] = time.mktime(datetime.datetime(year=2023, month=1, day=1, hour=result["AUTO_SUBMIT_HOUR"],
-                                                   minute=result["AUTO_SUBMIT_MINUTE"], second=0).timetuple())
-    result["remind"] = time.mktime(datetime.datetime(year=2023, month=1, day=1, hour=result["DXX_REMIND_HOUR"],
-                                                     minute=result["DXX_REMIND_MINUTE"], second=0).timetuple())
-    return JSONResponse({"status": 0, "msg": "数据加载成功！", "data": result
-                         })
-
-
-@route.put("/change_settings", response_class=JSONResponse, dependencies=[admin_authentication()])
-async def change_settings(data: dict) -> JSONResponse:
-    try:
-        if data["password"]:
-            data["PASSWORD"] = await to_hash(data["password"])
-        data["DXX_REMIND_HOUR"] = datetime.datetime.fromtimestamp(float(data["remind"])).hour
-        data["DXX_REMIND_MINUTE"] = datetime.datetime.fromtimestamp(float(data["remind"])).minute
-        data["AUTO_SUBMIT_HOUR"] = datetime.datetime.fromtimestamp(float(data["auto"])).hour
-        data["AUTO_SUBMIT_MINUTE"] = datetime.datetime.fromtimestamp(float(data["auto"])).minute
-        data.pop("password")
-        data.pop("auto")
-        data.pop("remind")
-        saveConfig(data=data)
-        return JSONResponse({
-            "status": 0,
-            "msg": "修改成功！"
-        })
-    except Exception as e:
-        logger.error(e)
-        return JSONResponse({
-            "status": 500,
-            "msg": f"修改失败{e}"
-        })
-
-
-@route.delete("/delete_request", response_class=JSONResponse, dependencies=[admin_authentication()])
-async def delete_request(id: int) -> JSONResponse:
-    try:
-        await AddUser.filter(id=id).delete()
-        return JSONResponse({
-            "status": 0,
-            "msg": "删除成功！"
-        })
-    except Exception as e:
-        logger.error(e)
-        return JSONResponse({
-            "status": 500,
-            "msg": "删除失败！"
-        })
-
-
-@route.delete("/delete_requests", response_class=JSONResponse, dependencies=[admin_authentication()])
-async def delete_requests(ids: str) -> JSONResponse:
-    for id in ids.split(","):
-        await AddUser.filter(id=id).delete()
-    return JSONResponse({
-        "status": 0, "msg": "删除成功！"
-    })
-
-
-@route.delete("/delete_answer", response_class=JSONResponse, dependencies=[admin_authentication()])
-async def delete_answer(id: int) -> JSONResponse:
-    try:
-        await Answer.filter(id=id).delete()
-        return JSONResponse({
-            "status": 0,
-            "msg": "删除成功！"
-        })
-    except Exception as e:
-        logger.error(e)
-        return JSONResponse({
-            "status": 500,
-            "msg": "删除失败！"
-        })
-
-
-@route.get("/get_requests", response_class=JSONResponse, dependencies=[admin_authentication()])
-async def get_requests(
-        page: int = 1,
-        perPage: int = 10,
-        orderBy: str = 'time',
-        orderDir: str = 'desc',
-        group_id: Optional[str] = None,
-        user_id: Optional[str] = None,
-        area: Optional[str] = None,
-        status: Optional[str] = None) -> JSONResponse:
-    orderBy = (orderBy or 'time') if (orderDir or 'desc') == 'asc' else f'-{orderBy or "time"}'
-    filter_args = {f'{k}__contains': v for k, v in
-                   {'group_id': group_id, 'user_id': user_id, "area": area, "status": status}.items() if v}
-    return JSONResponse({
-        'status': 0,
-        'msg': 'ok',
-        'data': {
-            'items': await AddUser.filter(**filter_args).order_by(orderBy).offset((page - 1) * perPage).limit(
-                perPage).values(),
-            'total': await AddUser.filter(**filter_args).count()
-        }
-    })
-
-
-@route.get("/get_members", response_class=JSONResponse, dependencies=[admin_authentication()])
-async def get_members() -> JSONResponse:
-    result = await User.all().values()
-    return JSONResponse({
-        'status': 0,
-        'msg': 'ok',
-        'data': {
-            'rows': result,
-            'total': len(result)
-        }
-    })
-
-
-@route.delete('/delete_member', response_class=JSONResponse, dependencies=[admin_authentication()])
-async def delete_member(user_id: int) -> JSONResponse:
-    try:
-        await User.filter(user_id=user_id).delete()
-        return JSONResponse({
-            "status": 0,
-            "msg": "删除成功！"
-        })
-    except Exception as e:
-        logger.error(e)
-        return JSONResponse({
-            "status": 500,
-            "msg": f"删除失败!{e}"
-        })
-
-
-@route.get("/get_push_list", response_class=JSONResponse, dependencies=[admin_authentication()])
-async def get_push_list(
-        page: int = 1,
-        perPage: int = 10,
-        orderBy: str = 'time',
-        orderDir: str = 'desc',
-        group_id: Optional[str] = None,
-        self_id: Optional[str] = None,
-        user_id: Optional[str] = None,
-        status: Optional[str] = None) -> JSONResponse:
-    orderBy = (orderBy or 'time') if (orderDir or 'desc') == 'asc' else f'-{orderBy or "time"}'
-    filter_args = {f'{k}__contains': v for k, v in
-                   {'group_id': group_id, "user_id": user_id, "self_id": self_id, "status": status}.items() if v}
-    return JSONResponse({
-        'status': 0,
-        'msg': 'ok',
-        'data': {
-            'items': await PushList.filter(**filter_args).order_by(orderBy).offset((page - 1) * perPage).limit(
-                perPage).values(),
-            'total': await PushList.filter(**filter_args).count()
-        }
-    })
-
-
-@route.get('/get_group_list', response_class=JSONResponse, dependencies=[admin_authentication()])
-async def get_group_list() -> JSONResponse:
-    try:
-        group_list = await get_bot().get_group_list()
-        group_list = [{'label': f'{group["group_name"]}({group["group_id"]})', 'value': group['group_id']} for group in
-                      group_list]
-        return JSONResponse({
-            'status': 0,
-            'msg': 'ok',
-            'data': {"options": group_list}
-        })
-    except ValueError:
-        return JSONResponse({
-            'status': 500,
-            'msg': '获取群和好友列表失败，请确认已连接go-cqhttp'
-        })
-
-
-@route.get('/get_member_list', response_class=JSONResponse, dependencies=[admin_authentication()])
-async def get_member_list(group_id: Optional[str] = None) -> JSONResponse:
-    if not group_id:
-        return JSONResponse({
-            'status': 0,
-            'msg': 'ok',
-            'data': {"options": []}
-        })
-    try:
-        member_list = await get_bot().get_group_member_list(group_id=int(group_id))
-        member_list = [{'label': f'{member["nickname"]}-{member["user_id"]}', 'value': member['user_id']} for member in
-                       member_list]
-        return JSONResponse({
-            'status': 0,
-            'msg': 'ok',
-            'data': {"options": member_list}
-        })
-    except ValueError:
-        return JSONResponse({
-            'status': 500,
-            'msg': '获取群和好友列表失败，请确认已连接go-cqhttp'
-        })
-
-
-@route.post("/add_push", response_class=JSONResponse, dependencies=[admin_authentication()])
-async def add_push(data: dict) -> JSONResponse:
-    bot: Bot = get_bot()
-    self_id = int(bot.self_id)
-    user_id = self_id
-    group_ids = data["groups"]
-    for group_id in group_ids:
-        try:
-            if await PushList.filter(group_id=group_id).count():
-                continue
-            await PushList.create(
-                time=time.time(),
-                self_id=self_id,
-                user_id=user_id,
-                group_id=group_id,
-                status=True
-            )
-        except Exception as e:
-            logger.error(e)
-            return JSONResponse({
-                "status": 500,
-                "msg": f"添加失败！{e}"
-            })
-    return JSONResponse({
-        "status": 0,
-        "msg": "添加成功！"
-    })
-
-
-@route.delete("/delete_push", response_class=JSONResponse, dependencies=[admin_authentication()])
-async def delete_push(id: int) -> JSONResponse:
-    try:
-        await PushList.filter(id=id).delete()
-        return JSONResponse({
-            "status": 0,
-            "msg": "删除成功！"
-        })
-    except Exception as e:
-        logger.error(e)
-        return JSONResponse({
-            "status": 500,
-            "msg": "删除失败！"
-        })
-
-
-@route.delete("/delete_pushs", response_class=JSONResponse, dependencies=[admin_authentication()])
-async def delete_pushs(ids: str) -> JSONResponse:
-    for id in ids.split(","):
-        await PushList.filter(id=id).delete()
-    return JSONResponse({
-        "status": 0, "msg": "删除成功！"
-    })
+import time
+from typing import Optional
+import datetime
+from fastapi import APIRouter
+from fastapi.responses import JSONResponse
+from nonebot import logger, get_bot
+from nonebot.adapters.onebot.v11.bot import Bot
+
+from .login import admin_authentication
+from ..utils.status import get_status
+from ...models.accuont import Commit, AddUser, User
+from ...models.dxx import Answer, PushList
+from ...utils.utils import to_hash
+from ...utils.path import getConfig, saveConfig
+
+route = APIRouter()
+
+
+@route.get('/status', response_class=JSONResponse, dependencies=[admin_authentication()])
+async def status():
+    return await get_status()
+
+
+@route.delete("/delete_all", response_class=JSONResponse, dependencies=[admin_authentication()])
+async def delete_all(type: str) -> JSONResponse:
+    if type == "records":
+        await Commit.all().delete()
+    elif type == "answers":
+        await Answer.all().delete()
+    elif type == "requests":
+        await AddUser.all().delete()
+    else:
+        return JSONResponse({"status": 500, "msg": "删除失败！"})
+    return JSONResponse({"status": 0, "msg": "删除成功！"})
+
+
+@route.delete("/delete_record", response_class=JSONResponse, dependencies=[admin_authentication()])
+async def delete_record(id: int) -> JSONResponse:
+    try:
+        await Commit.filter(id=id).delete()
+        return JSONResponse({
+            "status": 0,
+            "msg": "删除成功！"
+        })
+    except Exception as e:
+        logger.error(e)
+        return JSONResponse({
+            "status": 500,
+            "msg": "删除失败！"
+        })
+
+
+@route.delete("/delete_records", response_class=JSONResponse, dependencies=[admin_authentication()])
+async def delete_records(ids: str) -> JSONResponse:
+    for id in ids.split(","):
+        await Commit.filter(id=id).delete()
+    return JSONResponse({
+        "status": 0, "msg": "删除成功！"
+    })
+
+
+@route.delete("/delete_answer", response_class=JSONResponse, dependencies=[admin_authentication()])
+async def delete_answer(id: int) -> JSONResponse:
+    try:
+        await Answer.filter(id=id).delete()
+        return JSONResponse({
+            "status": 0,
+            "msg": "删除成功！"
+        })
+    except Exception as e:
+        logger.error(e)
+        return JSONResponse({
+            "status": 500,
+            "msg": "删除失败！"
+        })
+
+
+@route.delete("/delete_answers", response_class=JSONResponse, dependencies=[admin_authentication()])
+async def delete_answers(ids: str) -> JSONResponse:
+    for id in ids.split(","):
+        await Answer.filter(id=id).delete()
+    return JSONResponse({"status": 0, "msg": "删除成功！"})
+
+
+@route.get("/get_settings", response_class=JSONResponse, dependencies=[admin_authentication()])
+async def get_answers() -> JSONResponse:
+    result = getConfig()
+    result["auto"] = time.mktime(datetime.datetime(year=2023, month=1, day=1, hour=result["AUTO_SUBMIT_HOUR"],
+                                                   minute=result["AUTO_SUBMIT_MINUTE"], second=0).timetuple())
+    result["remind"] = time.mktime(datetime.datetime(year=2023, month=1, day=1, hour=result["DXX_REMIND_HOUR"],
+                                                     minute=result["DXX_REMIND_MINUTE"], second=0).timetuple())
+    return JSONResponse({"status": 0, "msg": "数据加载成功！", "data": result
+                         })
+
+
+@route.put("/change_settings", response_class=JSONResponse, dependencies=[admin_authentication()])
+async def change_settings(data: dict) -> JSONResponse:
+    try:
+        if data["password"]:
+            data["PASSWORD"] = await to_hash(data["password"])
+        data["DXX_REMIND_HOUR"] = datetime.datetime.fromtimestamp(float(data["remind"])).hour
+        data["DXX_REMIND_MINUTE"] = datetime.datetime.fromtimestamp(float(data["remind"])).minute
+        data["AUTO_SUBMIT_HOUR"] = datetime.datetime.fromtimestamp(float(data["auto"])).hour
+        data["AUTO_SUBMIT_MINUTE"] = datetime.datetime.fromtimestamp(float(data["auto"])).minute
+        data.pop("password")
+        data.pop("auto")
+        data.pop("remind")
+        saveConfig(data=data)
+        return JSONResponse({
+            "status": 0,
+            "msg": "修改成功！"
+        })
+    except Exception as e:
+        logger.error(e)
+        return JSONResponse({
+            "status": 500,
+            "msg": f"修改失败{e}"
+        })
+
+
+@route.delete("/delete_request", response_class=JSONResponse, dependencies=[admin_authentication()])
+async def delete_request(id: int) -> JSONResponse:
+    try:
+        await AddUser.filter(id=id).delete()
+        return JSONResponse({
+            "status": 0,
+            "msg": "删除成功！"
+        })
+    except Exception as e:
+        logger.error(e)
+        return JSONResponse({
+            "status": 500,
+            "msg": "删除失败！"
+        })
+
+
+@route.delete("/delete_requests", response_class=JSONResponse, dependencies=[admin_authentication()])
+async def delete_requests(ids: str) -> JSONResponse:
+    for id in ids.split(","):
+        await AddUser.filter(id=id).delete()
+    return JSONResponse({
+        "status": 0, "msg": "删除成功！"
+    })
+
+
+@route.delete("/delete_answer", response_class=JSONResponse, dependencies=[admin_authentication()])
+async def delete_answer(id: int) -> JSONResponse:
+    try:
+        await Answer.filter(id=id).delete()
+        return JSONResponse({
+            "status": 0,
+            "msg": "删除成功！"
+        })
+    except Exception as e:
+        logger.error(e)
+        return JSONResponse({
+            "status": 500,
+            "msg": "删除失败！"
+        })
+
+
+@route.get("/get_requests", response_class=JSONResponse, dependencies=[admin_authentication()])
+async def get_requests(
+        page: int = 1,
+        perPage: int = 10,
+        orderBy: str = 'time',
+        orderDir: str = 'desc',
+        group_id: Optional[str] = None,
+        user_id: Optional[str] = None,
+        area: Optional[str] = None,
+        status: Optional[str] = None) -> JSONResponse:
+    orderBy = (orderBy or 'time') if (orderDir or 'desc') == 'asc' else f'-{orderBy or "time"}'
+    filter_args = {f'{k}__contains': v for k, v in
+                   {'group_id': group_id, 'user_id': user_id, "area": area, "status": status}.items() if v}
+    return JSONResponse({
+        'status': 0,
+        'msg': 'ok',
+        'data': {
+            'items': await AddUser.filter(**filter_args).order_by(orderBy).offset((page - 1) * perPage).limit(
+                perPage).values(),
+            'total': await AddUser.filter(**filter_args).count()
+        }
+    })
+
+
+@route.get("/get_members", response_class=JSONResponse, dependencies=[admin_authentication()])
+async def get_members() -> JSONResponse:
+    result = await User.all().values()
+    return JSONResponse({
+        'status': 0,
+        'msg': 'ok',
+        'data': {
+            'rows': result,
+            'total': len(result)
+        }
+    })
+
+
+@route.delete('/delete_member', response_class=JSONResponse, dependencies=[admin_authentication()])
+async def delete_member(user_id: int) -> JSONResponse:
+    try:
+        await User.filter(user_id=user_id).delete()
+        return JSONResponse({
+            "status": 0,
+            "msg": "删除成功！"
+        })
+    except Exception as e:
+        logger.error(e)
+        return JSONResponse({
+            "status": 500,
+            "msg": f"删除失败!{e}"
+        })
+
+
+@route.get("/get_push_list", response_class=JSONResponse, dependencies=[admin_authentication()])
+async def get_push_list(
+        page: int = 1,
+        perPage: int = 10,
+        orderBy: str = 'time',
+        orderDir: str = 'desc',
+        group_id: Optional[str] = None,
+        self_id: Optional[str] = None,
+        user_id: Optional[str] = None,
+        status: Optional[str] = None) -> JSONResponse:
+    orderBy = (orderBy or 'time') if (orderDir or 'desc') == 'asc' else f'-{orderBy or "time"}'
+    filter_args = {f'{k}__contains': v for k, v in
+                   {'group_id': group_id, "user_id": user_id, "self_id": self_id, "status": status}.items() if v}
+    return JSONResponse({
+        'status': 0,
+        'msg': 'ok',
+        'data': {
+            'items': await PushList.filter(**filter_args).order_by(orderBy).offset((page - 1) * perPage).limit(
+                perPage).values(),
+            'total': await PushList.filter(**filter_args).count()
+        }
+    })
+
+
+@route.get('/get_group_list', response_class=JSONResponse, dependencies=[admin_authentication()])
+async def get_group_list() -> JSONResponse:
+    try:
+        group_list = await get_bot().get_group_list()
+        group_list = [{'label': f'{group["group_name"]}({group["group_id"]})', 'value': group['group_id']} for group in
+                      group_list]
+        return JSONResponse({
+            'status': 0,
+            'msg': 'ok',
+            'data': {"options": group_list}
+        })
+    except ValueError:
+        return JSONResponse({
+            'status': 500,
+            'msg': '获取群和好友列表失败，请确认已连接go-cqhttp'
+        })
+
+
+@route.get('/get_member_list', response_class=JSONResponse, dependencies=[admin_authentication()])
+async def get_member_list(group_id: Optional[str] = None) -> JSONResponse:
+    if not group_id:
+        return JSONResponse({
+            'status': 0,
+            'msg': 'ok',
+            'data': {"options": []}
+        })
+    try:
+        member_list = await get_bot().get_group_member_list(group_id=int(group_id))
+        member_list = [{'label': f'{member["nickname"]}-{member["user_id"]}', 'value': member['user_id']} for member in
+                       member_list]
+        return JSONResponse({
+            'status': 0,
+            'msg': 'ok',
+            'data': {"options": member_list}
+        })
+    except ValueError:
+        return JSONResponse({
+            'status': 500,
+            'msg': '获取群和好友列表失败，请确认已连接go-cqhttp'
+        })
+
+
+@route.post("/add_push", response_class=JSONResponse, dependencies=[admin_authentication()])
+async def add_push(data: dict) -> JSONResponse:
+    bot: Bot = get_bot()
+    self_id = int(bot.self_id)
+    user_id = self_id
+    group_ids = data["groups"]
+    for group_id in group_ids:
+        try:
+            if await PushList.filter(group_id=group_id).count():
+                continue
+            await PushList.create(
+                time=time.time(),
+                self_id=self_id,
+                user_id=user_id,
+                group_id=group_id,
+                status=True
+            )
+        except Exception as e:
+            logger.error(e)
+            return JSONResponse({
+                "status": 500,
+                "msg": f"添加失败！{e}"
+            })
+    return JSONResponse({
+        "status": 0,
+        "msg": "添加成功！"
+    })
+
+
+@route.delete("/delete_push", response_class=JSONResponse, dependencies=[admin_authentication()])
+async def delete_push(id: int) -> JSONResponse:
+    try:
+        await PushList.filter(id=id).delete()
+        return JSONResponse({
+            "status": 0,
+            "msg": "删除成功！"
+        })
+    except Exception as e:
+        logger.error(e)
+        return JSONResponse({
+            "status": 500,
+            "msg": "删除失败！"
+        })
+
+
+@route.delete("/delete_pushs", response_class=JSONResponse, dependencies=[admin_authentication()])
+async def delete_pushs(ids: str) -> JSONResponse:
+    for id in ids.split(","):
+        await PushList.filter(id=id).delete()
+    return JSONResponse({
+        "status": 0, "msg": "删除成功！"
+    })
```

### Comparing `TeenStudy-0.1.9/TeenStudy/web/api/home.py` & `teenstudy-0.2.0rc1/TeenStudy/web/api/home.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,125 +1,134 @@
-import datetime
-from typing import Optional
-
-from fastapi import APIRouter
-from fastapi.responses import JSONResponse
-
-from .login import authentication
-from ...models.accuont import User, Commit
-from ...models.dxx import Answer
-from ...utils.rule import check_time
-from ...utils.utils import distribute_area
-from ...utils.utils import to_hash
-
-route = APIRouter()
-
-
-@route.get("/get_user", response_class=JSONResponse, dependencies=[authentication()])
-async def get_user(user_id: int) -> JSONResponse:
-    result = await User.filter(user_id=user_id).values()
-    if result:
-        data = result[0]
-        try:
-            data["commit_time"] = datetime.datetime.fromtimestamp(data['commit_time']).strftime(
-                "%Y-%m-%d %H:%M:%S")
-        except TypeError:
-            data["commit_time"] = "暂未提交"
-        if data["catalogue"] is None:
-            data["catalogue"] = "暂未提交"
-        return JSONResponse(
-            data)
-
-
-@route.put("/change", response_class=JSONResponse, dependencies=[authentication()])
-async def change(user_id: int, data: dict) -> JSONResponse:
-    if await User.filter(user_id=user_id).values():
-        password = data["Password"]
-        if password:
-            data["password"] = await to_hash(password)
-        data.pop("Password")
-        if data["leader"] == "":
-            data["leader"] = None
-        await User.filter(user_id=user_id).update(**data)
-        return JSONResponse({
-            "status": 0,
-            "msg": "修改成功！"
-        })
-    else:
-        return JSONResponse({
-            "status": 422,
-            "msg": "用户不存在！"
-        })
-
-
-@route.get("/get_records", response_class=JSONResponse, dependencies=[authentication()])
-async def get_records(
-        page: int = 1,
-        perPage: int = 10,
-        orderBy: str = 'time',
-        orderDir: str = 'desc',
-        group_id: Optional[str] = None,
-        user_id: Optional[str] = None,
-        name: Optional[str] = None,
-        college: Optional[str] = None,
-        organization: Optional[str] = None,
-        catalogue: Optional[str] = None,
-        status: Optional[str] = None,
-        area: Optional[str] = None
-) -> JSONResponse:
-    orderBy = (orderBy or 'time') if (orderDir or 'desc') == 'asc' else f'-{orderBy or "time"}'
-    filter_args = {f'{k}__contains': v for k, v in
-                   {'group_id': group_id, 'user_id': user_id, "area": area, "name": name, "college": college,
-                    "organization": organization, "catalogue": catalogue, "status": status}.items() if v}
-    return JSONResponse({
-        'status': 0,
-        'msg': 'ok',
-        'data': {
-            'items': await Commit.filter(**filter_args).order_by(orderBy).offset((page - 1) * perPage).limit(
-                perPage).values(),
-            'total': await Commit.filter(**filter_args).count()
-        }
-    })
-
-
-@route.get('/get_answers', response_class=JSONResponse, dependencies=[authentication()])
-async def get_answers(page: int = 1,
-                      perPage: int = 10,
-                      orderBy: str = 'time',
-                      orderDir: str = 'desc',
-                      catalogue: Optional[str] = None
-                      ) -> JSONResponse:
-    orderBy = (orderBy or 'time') if (orderDir or 'desc') == 'asc' else f'-{orderBy or "time"}'
-    filter_args = {f'{k}__contains': v for k, v in
-                   {'catalogue': catalogue}.items() if v}
-    items = await Answer.filter(**filter_args).order_by(orderBy).offset((page - 1) * perPage).limit(
-        perPage).values()
-    for item in items:
-        item.pop("cover")
-    return JSONResponse({
-        'status': 0,
-        'msg': 'ok',
-        'data': {
-            'items': items,
-            'total': await Answer.filter(**filter_args).count()
-        }
-    })
-
-
-@route.get('/commit', response_class=JSONResponse, dependencies=[authentication()])
-async def commit(user_id: int, area: str) -> JSONResponse:
-    if not await check_time():
-        return JSONResponse({
-            "status": 500,
-            "msg": "当前时间段禁止提交青年大学习，请在周一11:00之后再提交哦(｡･ω･｡)"
-        })
-    data = await distribute_area(user_id=user_id, area=area)
-    return JSONResponse({
-        "status": data["status"],
-        "msg": data["msg"]
-    })
-
-
-@route.put("/set_auto_submit", response_class=JSONResponse, dependencies=[authentication()])
-async def set_auto_submit(data: dict) -> JSONResponse:
-    await User.filter(id=data["id"]).update(auto_submit=data["status"])
-    return JSONResponse({"status": 0})
+import datetime
+from typing import Optional
+
+from fastapi import APIRouter, Header
+from fastapi.responses import JSONResponse
+
+from .login import authentication, get_userInfo
+from ...models.accuont import User, Commit
+from ...models.dxx import Answer
+from ...utils.rule import check_time
+from ...utils.utils import distribute_area
+from ...utils.utils import to_hash
+
+route = APIRouter()
+
+
+@route.get("/get_user", response_class=JSONResponse, dependencies=[authentication()])
+async def get_user(token: Optional[str] = Header(...)) -> JSONResponse:
+    userinfo = await get_userInfo(token=token)
+    user_id = userinfo["user_id"]
+    result = await User.filter(user_id=user_id).values()
+    if result:
+        data = result[0]
+        try:
+            data["commit_time"] = datetime.datetime.fromtimestamp(data['commit_time']).strftime(
+                "%Y-%m-%d %H:%M:%S")
+        except TypeError:
+            data["commit_time"] = "暂未提交"
+        if data["catalogue"] is None:
+            data["catalogue"] = "暂未提交"
+        return JSONResponse(
+            data)
+
+
+@route.put("/change", response_class=JSONResponse, dependencies=[authentication()])
+async def change(user_id: int, data: dict) -> JSONResponse:
+    if await User.filter(user_id=user_id).values():
+        password = data["Password"]
+        if password:
+            data["password"] = await to_hash(password)
+        data.pop("Password")
+        if data["leader"] == "":
+            data["leader"] = None
+        await User.filter(user_id=user_id).update(**data)
+        return JSONResponse({
+            "status": 0,
+            "msg": "修改成功！"
+        })
+    else:
+        return JSONResponse({
+            "status": 422,
+            "msg": "用户不存在！"
+        })
+
+
+@route.get("/get_records", response_class=JSONResponse, dependencies=[authentication()])
+async def get_records(
+        token: Optional[str] = Header(...),
+        page: int = 1,
+        perPage: int = 10,
+        orderBy: str = 'time',
+        orderDir: str = 'desc',
+        group_id: Optional[str] = None,
+        user_id: Optional[str] = None,
+        name: Optional[str] = None,
+        college: Optional[str] = None,
+        organization: Optional[str] = None,
+        catalogue: Optional[str] = None,
+        status: Optional[str] = None,
+        area: Optional[str] = None
+) -> JSONResponse:
+    userinfo = await get_userInfo(token=token)
+    if not user_id:
+        if userinfo["role"]:
+            user_id = ""
+        else:
+            user_id = userinfo["user_id"]
+    orderBy = (orderBy or 'time') if (orderDir or 'desc') == 'asc' else f'-{orderBy or "time"}'
+    filter_args = {f'{k}__contains': v for k, v in
+                   {'group_id': group_id, 'user_id': user_id, "area": area, "name": name, "college": college,
+                    "organization": organization, "catalogue": catalogue, "status": status}.items() if v}
+    return JSONResponse({
+        'status': 0,
+        'msg': 'ok',
+        'data': {
+            'items': await Commit.filter(**filter_args).order_by(orderBy).offset((page - 1) * perPage).limit(
+                perPage).values(),
+            'total': await Commit.filter(**filter_args).count()
+        }
+    })
+
+
+@route.get('/get_answers', response_class=JSONResponse, dependencies=[authentication()])
+async def get_answers(page: int = 1,
+                      perPage: int = 10,
+                      orderBy: str = 'time',
+                      orderDir: str = 'desc',
+                      catalogue: Optional[str] = None
+                      ) -> JSONResponse:
+    orderBy = (orderBy or 'time') if (orderDir or 'desc') == 'asc' else f'-{orderBy or "time"}'
+    filter_args = {f'{k}__contains': v for k, v in
+                   {'catalogue': catalogue}.items() if v}
+    items = await Answer.filter(**filter_args).order_by(orderBy).offset((page - 1) * perPage).limit(
+        perPage).values()
+    for item in items:
+        item.pop("cover")
+    return JSONResponse({
+        'status': 0,
+        'msg': 'ok',
+        'data': {
+            'items': items,
+            'total': await Answer.filter(**filter_args).count()
+        }
+    })
+
+
+@route.get('/commit', response_class=JSONResponse, dependencies=[authentication()])
+async def commit(user_id: int, area: str) -> JSONResponse:
+    if not await check_time():
+        return JSONResponse({
+            "status": 500,
+            "msg": "当前时间段禁止提交青年大学习，请在周一11:00之后再提交哦(｡･ω･｡)"
+        })
+    data = await distribute_area(user_id=user_id, area=area)
+    return JSONResponse({
+        "status": data["status"],
+        "msg": data["msg"]
+    })
+
+
+@route.put("/set_auto_submit", response_class=JSONResponse, dependencies=[authentication()])
+async def set_auto_submit(data: dict) -> JSONResponse:
+    await User.filter(id=data["id"]).update(auto_submit=data["status"])
+    return JSONResponse({"status": 0})
```

### Comparing `TeenStudy-0.1.9/TeenStudy/web/api/login.py` & `teenstudy-0.2.0rc1/TeenStudy/web/api/login.py`

 * *Files 27% similar despite different names*

```diff
@@ -1,155 +1,145 @@
-import datetime
-from typing import Optional
-
-from fastapi import APIRouter
-from fastapi import Header, HTTPException, Depends
-from fastapi.responses import JSONResponse
-from jose import jwt
-from pydantic import BaseModel
-
-from ...models.accuont import User
-from ...utils.utils import to_hash
-from ...utils.path import getConfig
-
-
-class UserModel(BaseModel):
-    user_id: int
-    password: str
-    role: bool
-
-
-route = APIRouter()
-
-
-@route.post('/login', response_class=JSONResponse)
-async def login(user: UserModel):
-    user_id = user.user_id
-    password = await to_hash(user.password)
-    role = user.role
-    if role:
-        result = getConfig()
-        if result["SUPERUSER"] != user_id or result["PASSWORD"] != password:
-            result = False
-    else:
-        result = await User.filter(user_id=user_id, password=password).count()
-    if not result:
-        return {
-            'status': -100,
-            'msg': '登录失败，请确认用户ID和密码无误'
-        }
-    token = await create_token(user_id=user.user_id, role=role)
-    if role:
-        return {
-            'status': 0,
-            'msg': '登录成功',
-            'data': {
-                'url': "admin",
-                'role': role,
-                'user_id': user_id,
-                'token': token
-            }
-        }
-    else:
-        return {
-            'status': 0,
-            'msg': '登录成功',
-            'data': {
-                'url': f"home?user_id={user_id}",
-                'role': role,
-                'user_id': user_id,
-                'token': token
-            }
-        }
-
-
-def user_authentication():
-    async def inner(token: Optional[str] = Header(...)):
-        result = getConfig()
-        key = result["KEY"]
-        algorithm = result["ALGORITHM"]
-        try:
-            payload = jwt.decode(token, key, algorithms=algorithm)
-            if not (user_id := payload.get('user_id')):
-                raise HTTPException(status_code=400, detail='登录验证失败或已失效，请重新登录')
-            else:
-                try:
-                    role = payload.get('role')
-                    if role:
-                        raise HTTPException(status_code=400, detail='登录验证失败或已失效，请重新登录')
-                    else:
-                        result = await User.filter(user_id=user_id).count()
-                        if not result:
-                            raise HTTPException(status_code=400, detail='登录验证失败或已失效，请重新登录')
-                except (jwt.JWTError, jwt.ExpiredSignatureError, AttributeError):
-                    raise HTTPException(status_code=400, detail='登录验证失败或已失效，请重新登录')
-        except (jwt.JWTError, jwt.ExpiredSignatureError, AttributeError):
-            raise HTTPException(status_code=400, detail='登录验证失败或已失效，请重新登录')
-
-    return Depends(inner)
-
-
-def admin_authentication():
-    async def inner(token: Optional[str] = Header(...)):
-        result = getConfig()
-        key = result["KEY"]
-        algorithm = result["ALGORITHM"]
-        try:
-            payload = jwt.decode(token, key, algorithms=algorithm)
-            if not (user_id := payload.get('user_id')):
-                raise HTTPException(status_code=400, detail='登录验证失败或已失效，请重新登录')
-            else:
-                try:
-                    role = payload.get('role')
-                    if role:
-                        result = getConfig()
-                        if result["SUPERUSER"] != user_id:
-                            result = False
-                        if not result:
-                            raise HTTPException(status_code=400, detail='登录验证失败或已失效，请重新登录')
-                    else:
-                        raise HTTPException(status_code=400, detail='登录验证失败或已失效，请重新登录')
-                except (jwt.JWTError, jwt.ExpiredSignatureError, AttributeError):
-                    raise HTTPException(status_code=400, detail='登录验证失败或已失效，请重新登录')
-        except (jwt.JWTError, jwt.ExpiredSignatureError, AttributeError):
-            raise HTTPException(status_code=400, detail='登录验证失败或已失效，请重新登录')
-
-    return Depends(inner)
-
-
-def authentication():
-    async def inner(token: Optional[str] = Header(...)):
-        result = getConfig()
-        key = result["KEY"]
-        algorithm = result["ALGORITHM"]
-        try:
-            payload = jwt.decode(token, key, algorithms=algorithm)
-            if not (user_id := payload.get('user_id')):
-                raise HTTPException(status_code=400, detail='登录验证失败或已失效，请重新登录')
-            try:
-                role = payload.get('role')
-                if role:
-                    result = getConfig()
-                    if result['SUPERUSER'] != user_id:
-                        result = False
-                    if not result:
-                        raise HTTPException(status_code=400, detail='登录验证失败或已失效，请重新登录')
-                else:
-                    result = await User.filter(user_id=user_id).count()
-                    if not result:
-                        raise HTTPException(status_code=400, detail='登录验证失败或已失效，请重新登录')
-            except (jwt.JWTError, jwt.ExpiredSignatureError, AttributeError):
-                raise HTTPException(status_code=400, detail='登录验证失败或已失效，请重新登录')
-        except (jwt.JWTError, jwt.ExpiredSignatureError, AttributeError):
-            raise HTTPException(status_code=400, detail='登录验证失败或已失效，请重新登录')
-
-    return Depends(inner)
-
-
-async def create_token(user_id: int, role: bool):
-    result = getConfig()
-    key = result["KEY"]
-    time = result["TOKEN_TIME"]
-    algorithm = result["ALGORITHM"]
-    data = {'user_id': user_id, 'role': role,
-            'exp': datetime.datetime.now(datetime.timezone.utc) + datetime.timedelta(minutes=time)}
-    return jwt.encode(data, key, algorithm=algorithm)
+import datetime
+from typing import Optional
+
+from fastapi import APIRouter
+from fastapi import Header, HTTPException, Depends
+from fastapi.responses import JSONResponse
+from jose import jwt
+from pydantic import BaseModel
+
+from ...models.accuont import User
+from ...utils.path import getConfig
+from ...utils.utils import to_hash
+
+
+class UserModel(BaseModel):
+    user_id: int
+    password: str
+    role: bool
+
+
+route = APIRouter()
+
+
+@route.post('/login', response_class=JSONResponse)
+async def login(user: UserModel):
+    user_id = user.user_id
+    password = await to_hash(user.password)
+    role = user.role
+    if role:
+        result = getConfig()
+        if result["SUPERUSER"] != user_id or result["PASSWORD"] != password:
+            result = False
+    else:
+        result = await User.filter(user_id=user_id, password=password).count()
+    if not result:
+        return {
+            'status': -100,
+            'msg': '登录失败，请确认用户ID和密码无误'
+        }
+    token = await create_token(user_id=user.user_id, role=role)
+    if role:
+        return {
+            'status': 0,
+            'msg': '登录成功',
+            'data': {
+                'url': "admin",
+                'role': role,
+                'user_id': user_id,
+                'token': token
+            }
+        }
+    else:
+        return {
+            'status': 0,
+            'msg': '登录成功',
+            'data': {
+                'url': f"/home?user_id={user_id}",
+                'role': role,
+                'user_id': user_id,
+                'token': token
+            }
+        }
+
+
+async def get_userInfo(token: str) -> dict:
+    """
+    返回用户信息
+    :param token: token值
+    :return:
+    """
+    result = getConfig()
+    key = result["KEY"]
+    algorithm = result["ALGORITHM"]
+    payload = jwt.decode(token, key, algorithms=algorithm)
+    return {
+        "user_id": payload.get("user_id"),
+        "role": payload.get("role")
+    }
+
+
+def admin_authentication():
+    async def inner(token: Optional[str] = Header(...)):
+        result = getConfig()
+        key = result["KEY"]
+        algorithm = result["ALGORITHM"]
+        try:
+            payload = jwt.decode(token, key, algorithms=algorithm)
+            if not (user_id := payload.get('user_id')):
+                raise HTTPException(status_code=400, detail='登录验证失败或已失效，请重新登录')
+            else:
+                try:
+                    role = payload.get('role')
+                    if role:
+                        result = getConfig()
+                        if result["SUPERUSER"] != user_id:
+                            result = False
+                        if not result:
+                            raise HTTPException(status_code=400, detail='登录验证失败或已失效，请重新登录')
+                    else:
+                        raise HTTPException(status_code=400, detail='登录验证失败或已失效，请重新登录')
+                except (jwt.JWTError, jwt.ExpiredSignatureError, AttributeError):
+                    raise HTTPException(status_code=400, detail='登录验证失败或已失效，请重新登录')
+        except (jwt.JWTError, jwt.ExpiredSignatureError, AttributeError):
+            raise HTTPException(status_code=400, detail='登录验证失败或已失效，请重新登录')
+
+    return Depends(inner)
+
+
+def authentication():
+    async def inner(token: Optional[str] = Header(...)):
+        result = getConfig()
+        key = result["KEY"]
+        algorithm = result["ALGORITHM"]
+        try:
+            payload = jwt.decode(token, key, algorithms=algorithm)
+            if not (user_id := payload.get('user_id')):
+                raise HTTPException(status_code=400, detail='登录验证失败或已失效，请重新登录')
+            try:
+                role = payload.get('role')
+                if role:
+                    result = getConfig()
+                    if result['SUPERUSER'] != user_id:
+                        result = False
+                    if not result:
+                        raise HTTPException(status_code=400, detail='登录验证失败或已失效，请重新登录')
+                else:
+                    result = await User.filter(user_id=user_id).count()
+                    if not result:
+                        raise HTTPException(status_code=400, detail='登录验证失败或已失效，请重新登录')
+            except (jwt.JWTError, jwt.ExpiredSignatureError, AttributeError):
+                raise HTTPException(status_code=400, detail='登录验证失败或已失效，请重新登录')
+        except (jwt.JWTError, jwt.ExpiredSignatureError, AttributeError):
+            raise HTTPException(status_code=400, detail='登录验证失败或已失效，请重新登录')
+
+    return Depends(inner)
+
+
+async def create_token(user_id: int, role: bool):
+    result = getConfig()
+    key = result["KEY"]
+    time = result["TOKEN_TIME"]
+    algorithm = result["ALGORITHM"]
+    data = {'user_id': user_id, 'role': role,
+            'exp': datetime.datetime.now(datetime.timezone.utc) + datetime.timedelta(minutes=time)}
+    return jwt.encode(data, key, algorithm=algorithm)
```

### Comparing `TeenStudy-0.1.9/TeenStudy/web/pages/home.py` & `teenstudy-0.2.0rc1/TeenStudy/web/pages/home.py`

 * *Files 23% similar despite different names*

```diff
@@ -1,307 +1,335 @@
-from amis import App, PageSchema, Flex, ActionType, LevelEnum, Dialog, Form, DisplayModeEnum, InputText, TableColumn, \
-    CRUD, Tpl, Switch
-from amis import Html, Page, Property, Service, Divider
-
-logo = Html(html=f'''
-<p align="center">
-    <a href="https://github.com/ZM25XC/TeenStudy/">
-        <img src="https://i.328888.xyz/2023/02/23/xIh5k.png"
-         width="256" height="256" alt="TeenStudy">
-    </a>
-</p>
-<h2 align="center">大学习自动提交</h2>
-<div align="center">
-    <a href="https://github.com/ZM25XC/TeenStudy/" target="_blank">
-    Github仓库</a>
-    <a href="https://jq.qq.com/?_wv=1027&k=NGFEwXyS" target="_blank">交流群</a>
-</div>
-<br>
-''')
-github_logo = Tpl(className='w-full',
-                  tpl='<div class="flex justify-between"><div></div><div><a href="https://github.com/ZM25XC/TeenStudy" target="_blank" title="Github 仓库"><i class="fa fa-github fa-2x"></i></a></div></div>')
-header = Flex(className='w-full', justify='flex-end', alignItems='flex-end', items=[github_logo])
-operation_button = Flex(justify='center', items=[
-    ActionType.Dialog(
-        label='修改信息',
-        className='m-l',
-        level=LevelEnum.primary,
-        dialog=Dialog(title='修改信息',
-                      size='lg',
-                      body=[
-                          Form(
-                              title='',
-                              api='put:/TeenStudy/api/change?user_id=${user_id}',
-                              submitText='保存修改',
-                              mode=DisplayModeEnum.horizontal,
-                              labelAlign='right',
-                              body=[
-                                  InputText(label='性别', name='gender', value='${gender}', required=True,
-                                            trimContents=True, clearable=True,
-                                            showCounter=True, maxLength=3, visibleOn="${gender==null?false:true}",
-                                            description='性别'),
-                                  InputText(label='uid|nid', name='dxx_id', value='${dxx_id}', required=True,
-                                            trimContents=True, clearable=True,
-                                            showCounter=True, maxLength=24, visibleOn="${dxx_id==null?false:true}",
-                                            description='大学习认证ID，不清楚请勿改动'),
-                                  InputText(label='手机号', name='mobile', value='${mobile}', required=True,
-                                            trimContents=True, clearable=True,
-                                            showCounter=True, maxLength=24, visibleOn="${mobile==null?false:true}",
-                                            description='手机号'),
-                                  InputText(label='团支书ID', name='leader', value='${leader}',
-                                            showCounter=True, maxLength=10, hiddenOn=True, trimContents=True,
-                                            clearable=True,
-                                            description='团支书ID，填写后团支书可操作提交功能，不清楚请勿改动'),
-                                  InputText(label='openid', name='openid', value='${openid}', required=True,
-                                            trimContents=True, clearable=True,
-                                            showCounter=True, maxLength=64, visibleOn="${openid==null?false:true}",
-                                            description='微信认证ID，不清楚请勿改动'),
-                                  InputText(label='登录密码', name='Password', value='', type="input-password",
-                                            trimContents=True, clearable=True,
-                                            showCounter=True, maxLength=16, visibleOn="${password==null?false:true}",
-                                            description='登录Web UI的密码'),
-                                  InputText(label='学校类型', name='university_type', value='${university_type}',
-                                            showCounter=True, maxLength=16, required=True, trimContents=True,
-                                            clearable=True,
-                                            visibleOn="${university_type==null?false:true}",
-                                            description='学校类型，不清楚清无改动'),
-                                  InputText(label='学校ID', name='university_id', value='${university_id}',
-                                            required=True, trimContents=True, clearable=True,
-                                            showCounter=True, maxLength=24,
-                                            visibleOn="${university_id==null?false:true}",
-                                            description='学校ID，不清楚请勿改动'),
-                                  InputText(label='学校名称', name='university', value='${university}', required=True,
-                                            trimContents=True, clearable=True,
-                                            showCounter=True, maxLength=20, visibleOn="${university==null?false:true}",
-                                            description='学校名称'),
-                                  InputText(label='学院ID', name='college_id', value='${college_id}', required=True,
-                                            trimContents=True, clearable=True,
-                                            showCounter=True, maxLength=24, visibleOn="${college_id==null?false:true}",
-                                            description='学院ID'),
-                                  InputText(label='学院名称', name='college', value='${college}',
-                                            trimContents=True, clearable=True,
-                                            showCounter=True, maxLength=24, visibleOn="${college==null?false:true}",
-                                            description='学院名称'),
-                                  InputText(label='团支部ID', name='organization_id', value='${organization_id}',
-                                            required=True, trimContents=True, clearable=True,
-                                            showCounter=True, maxLength=24,
-                                            visibleOn="${organization_id==null?false:true}",
-                                            description='团支部ID'),
-                                  InputText(label='团支部名称', name='organization', value='${organization}',
-                                            required=False, trimContents=True, clearable=True,
-                                            showCounter=True, maxLength=36,
-                                            visibleOn="${organization==null?false:true}",
-                                            description='团支部名称'),
-                                  InputText(label='token', name='token', value='${token}', required=True,
-                                            trimContents=True, clearable=True,
-                                            showCounter=True, visibleOn="${token==null?false:true}",
-                                            description='提交大学习需要的token'),
-                                  InputText(label='cookie', name='cookie', value='${cookie}', required=True,
-                                            trimContents=True, clearable=True,
-                                            showCounter=True, visibleOn="${cookie==null?false:true}",
-                                            description='提交大学习需要的cookie')
-                              ])
-                      ])
-    ),
-    ActionType.Ajax(
-        label="提交大学习",
-        className='m-l',
-        level=LevelEnum.primary,
-        confirmText='是否提交最新一期青年大学习？',
-        api='get:/TeenStudy/api/commit?user_id=${user_id}&area=${area}'
-    ),
-    Switch(name='auto_submit',
-           value='${auto_submit}',
-           tooltip='自动提交大学习开关',
-           onText='自动提交大学习开',
-           offText='自动提交大学习关',
-           onEvent={
-               'change': {
-                   'actions': {
-                       'actionType': 'ajax',
-                       'args': {
-                           'api': {
-                               'url': '/TeenStudy/api/set_auto_submit',
-                               'method': 'put'
-                           },
-                           'messages': {
-                               'success': '自动提交已设置为${event.data.value==true?"开启":"关闭"}',
-                               'failed': '修改失败！'
-                           },
-                           'status': '${event.data.value}',
-                           'id': '${id}'
-                       }
-                   }
-               }
-           })
-])
-
-from_table = Service(
-    title="",
-    api="/TeenStudy/api/get_user?user_id=${user_id}",
-    interval=12000,
-    body=[
-        Property(
-            title='用户详细信息',
-            column=2,
-            items=[
-                Property.Item(
-                    label='用户ID',
-                    content='${user_id}'
-                ),
-                Property.Item(
-                    label='姓名',
-                    content='${name}'
-                ),
-                Property.Item(
-                    label='地区',
-                    content='${area}'
-                ),
-                Property.Item(
-                    label='学校',
-                    content='${university}'
-                ),
-                Property.Item(
-                    label='学院',
-                    content='${college}'
-                ),
-                Property.Item(
-                    label='团支部',
-                    content='${organization}'
-                ),
-                Property.Item(
-                    label='最新提交期数',
-                    content='${catalogue}'
-                ),
-                Property.Item(
-                    label='最新提交时间',
-                    content='${commit_time}'
-                ),
-                Property.Item(
-                    label='性别',
-                    content='${gender}',
-                    visibleOn="${gender==null?false:true}"
-                ),
-                Property.Item(
-                    label='手机号|学号',
-                    content='${mobile}',
-                    visibleOn="${mobile==null?false:true}"
-                ),
-                Property.Item(
-                    label='团支书ID',
-                    content='${leader}',
-                    visibleOn="${leader==null?false:true}"
-                ),
-                Property.Item(
-                    label='Uid|Nid',
-                    content='${dxx_id}',
-                    visibleOn="${dxx_id==null?false:true}"
-                ),
-                Property.Item(
-                    label='学校类型',
-                    content='${university_type}',
-                    visibleOn="${university_type==null?false:true}"
-                ),
-                Property.Item(
-                    label='学校ID',
-                    content='${university_id}',
-                    visibleOn="${university_id==null?false:true}"
-                ),
-                Property.Item(
-                    label='学院ID',
-                    content='${college_id}',
-                    visibleOn="${college_id==null?false:true}"
-                ),
-                Property.Item(
-                    label='团支部ID',
-                    content='${organization_id}',
-                    visibleOn="${organization_id==null?false:true}"
-                ), Property.Item(
-                    label='openid',
-                    content='${openid}',
-                    visibleOn="${openid==null?false:true}"
-                ), Property.Item(
-                    label='token',
-                    content='${token}',
-                    visibleOn="${token==null?false:true}",
-                    span=2
-                ), Property.Item(
-                    label='cookie',
-                    content='${cookie}',
-                    visibleOn="${cookie==null?false:true}",
-                    span=2
-                )
-            ]
-        )
-    ]
-)
-"""提交记录模板"""
-record_table = CRUD(mode='table',
-                    title='',
-                    syncLocation=False,
-                    api='/TeenStudy/api/get_records?user_id=${user_id}',
-                    type='crud',
-                    headerToolbar=[],
-                    itemActions=[],
-                    footable=True,
-                    columns=[
-                        TableColumn(label='用户ID', name='user_id'),
-                        TableColumn(label='姓名', name='name'),
-                        TableColumn(label='提交地区', name='area'),
-                        TableColumn(label='学校名称', name='university'),
-                        TableColumn(label='学院名称', name='college'),
-                        TableColumn(label='团支部', name='organization'),
-                        TableColumn(label='提交期数', name='catalogue', searchable=True),
-                        TableColumn(label='提交状态', name='${status==true?"成功":"失败"}'),
-                        TableColumn(type='tpl', tpl='${time|date:YYYY-MM-DD HH\\:mm\\:ss}',
-                                    label='提交时间',
-                                    name='time', sortable=True)
-                    ])
-answer_table = CRUD(mode='table',
-                    title='',
-                    syncLocation=False,
-                    api='/TeenStudy/api/get_answers',
-                    type='crud',
-                    headerToolbar=[],
-                    itemActions=[],
-                    footable=True,
-                    columns=[
-                        TableColumn(label='数据库ID', name='id'),
-                        TableColumn(label='大学习ID', name='code'),
-                        TableColumn(label='大学习期数', name='catalogue', searchable=True),
-                        TableColumn(type='tpl', tpl='${url|truncate:20}', label='官方网址',
-                                    name='url',
-                                    popOver={'mode': 'dialog', 'title': '完整网址',
-                                             'className': 'break-all',
-                                             'body': {'type': 'tpl',
-                                                      'tpl': '${url}'}}, copyable=True),
-                        TableColumn(type='tpl', tpl='${end_url|truncate:20}', label='完成截图网址',
-                                    name='end_url',
-                                    popOver={'mode': 'dialog', 'title': '完整网址',
-                                             'className': 'break-all',
-                                             'body': {'type': 'tpl',
-                                                      'tpl': '${end_url}'}}, copyable=True),
-                        TableColumn(type='tpl', tpl='${answer|truncate:20}', label='答案',
-                                    name='answer',
-                                    popOver={'mode': 'dialog', 'title': '完整答案',
-                                             'className': 'break-all',
-                                             'body': {'type': 'tpl',
-                                                      'tpl': '${answer}'}}),
-                        TableColumn(type='tpl', tpl='${time|date:YYYY-MM-DD HH\\:mm\\:ss}',
-                                    label='更新时间',
-                                    name='time', sortable=True)
-                    ])
-page_detail = Page(title='', body=[logo, operation_button, Divider(), from_table])
-home_page = PageSchema(url='/home', label='首页', icon='fa fa-home', isDefaultPage=True, schema=page_detail)
-home_app = App(brandName='TeenStudy',
-               logo='https://i.328888.xyz/2023/02/23/xIh5k.png',
-               header=header,
-               pages=[{
-                   'children': [
-                       home_page,
-                       PageSchema(url="answer", label='大学习列表', icon='fa fa-book-open',
-                                  schema=Page(title='', body=[answer_table])),
-                       PageSchema(url="/records", label='提交记录', icon='fa fa-code-commit',
-                                  schema=Page(title='', body=[record_table]))
-                   ]}],
-               footer=Html(
-                   html=f'<div class="p-2 text-center bg-blue-100">Copyright © 2022 - 2023 <a href="https://github.com/ZM25XC/TeenStudy" target="_blank" class="link-secondary">TeenStudy</a> X<a target="_blank" href="https://github.com/baidu/amis" class="link-secondary" rel="noopener"> amis v2.2.0</a></div>'))
+from amis import App, PageSchema, Flex, ActionType, LevelEnum, Dialog, Form, DisplayModeEnum, InputText, TableColumn, \
+    CRUD, Tpl, Switch
+from amis import Html, Page, Property, Service, Divider
+
+logo = Html(html=f'''
+<p align="center">
+    <a href="https://github.com/ZM25XC/TeenStudy/">
+        <img src="https://i.imgloc.com/2023/05/20/VyRjTV.png"
+         width="256" height="256" alt="TeenStudy">
+    </a>
+</p>
+<h2 align="center">大学习自动提交</h2>
+<div align="center">
+    <a href="https://github.com/ZM25XC/TeenStudy/" target="_blank">
+    Github仓库</a>
+    <a href="https://jq.qq.com/?_wv=1027&k=NGFEwXyS" target="_blank">交流群</a>
+    <a href="http://qm.qq.com/cgi-bin/qm/qr?_wv=1027&k=2PQucjirnkHyPjoS1Pkr-ai2aPGToBKm" target="_blank">QQ体验群</a>
+</div>
+<br>
+''')
+github_logo = Tpl(className='w-full',
+                  tpl='<div class="flex justify-between"><div></div><div><a href="https://github.com/ZM25XC/TeenStudy" target="_blank" title="Github 仓库"><i class="fa fa-github fa-2x"></i></a></div></div>')
+header = Flex(className='w-full', justify='flex-end', alignItems='flex-end', items=[github_logo, {
+    "type": "button",
+    "label": "退出",
+    "onEvent": {
+        "click": {
+            "actions": [
+                {
+                    "actionType": "confirmDialog",
+                    "args": {
+                        "title": "操作确认",
+                        "msg": "是否退出系统？"
+                    }},
+
+                {
+                    "actionType": "custom",
+                    "script": "window.location.href = '/TeenStudy/login';window.localStorage.clear();window.sessionStorage.clear();\n //event.stopPropagation();"
+                }
+
+            ]
+        },
+    }}])
+operation_button = Flex(justify='center', items=[
+    ActionType.Dialog(
+        label='修改信息',
+        className='m-l',
+        level=LevelEnum.primary,
+        dialog=Dialog(title='修改信息',
+                      size='lg',
+                      body=[
+                          Form(
+                              title='',
+                              api='put:/TeenStudy/api/change?user_id=${user_id}',
+                              submitText='保存修改',
+                              mode=DisplayModeEnum.horizontal,
+                              labelAlign='right',
+                              body=[
+                                  InputText(label='性别', name='gender', value='${gender}', required=True,
+                                            trimContents=True, clearable=True,
+                                            showCounter=True, maxLength=3, visibleOn="${gender==null?false:true}",
+                                            description='性别'),
+                                  InputText(label='uid|nid', name='dxx_id', value='${dxx_id}', required=True,
+                                            trimContents=True, clearable=True,
+                                            showCounter=True, maxLength=24, visibleOn="${dxx_id==null?false:true}",
+                                            description='大学习认证ID，不清楚请勿改动'),
+                                  InputText(label='手机号', name='mobile', value='${mobile}', required=True,
+                                            trimContents=True, clearable=True,
+                                            showCounter=True, maxLength=24, visibleOn="${mobile==null?false:true}",
+                                            description='手机号'),
+                                  InputText(label='团支书ID', name='leader', value='${leader}',
+                                            showCounter=True, maxLength=10, hiddenOn=True, trimContents=True,
+                                            clearable=True,
+                                            description='团支书ID，填写后团支书可操作提交功能，不清楚请勿改动'),
+                                  InputText(label='openid', name='openid', value='${openid}', required=True,
+                                            trimContents=True, clearable=True,
+                                            showCounter=True, maxLength=64, visibleOn="${openid==null?false:true}",
+                                            description='微信认证ID，不清楚请勿改动'),
+                                  InputText(label='登录密码', name='Password', value='', type="input-password",
+                                            trimContents=True, clearable=True,
+                                            showCounter=True, maxLength=16, visibleOn="${password==null?false:true}",
+                                            description='登录Web UI的密码'),
+                                  InputText(label='学校类型', name='university_type', value='${university_type}',
+                                            showCounter=True, maxLength=16, required=True, trimContents=True,
+                                            clearable=True,
+                                            visibleOn="${university_type==null?false:true}",
+                                            description='学校类型，不清楚请勿改动'),
+                                  InputText(label='学校ID', name='university_id', value='${university_id}',
+                                            required=True, trimContents=True, clearable=True,
+                                            showCounter=True, maxLength=24,
+                                            visibleOn="${university_id==null?false:true}",
+                                            description='学校ID，不清楚请勿改动'),
+                                  InputText(label='学校名称', name='university', value='${university}', required=True,
+                                            trimContents=True, clearable=True,
+                                            showCounter=True, maxLength=20, visibleOn="${university==null?false:true}",
+                                            description='学校名称'),
+                                  InputText(label='学院ID', name='college_id', value='${college_id}', required=True,
+                                            trimContents=True, clearable=True,
+                                            showCounter=True, maxLength=24, visibleOn="${college_id==null?false:true}",
+                                            description='学院ID'),
+                                  InputText(label='学院名称', name='college', value='${college}',
+                                            trimContents=True, clearable=True,
+                                            showCounter=True, maxLength=24, visibleOn="${college==null?false:true}",
+                                            description='学院名称'),
+                                  InputText(label='团支部ID', name='organization_id', value='${organization_id}',
+                                            required=True, trimContents=True, clearable=True,
+                                            showCounter=True, maxLength=24,
+                                            visibleOn="${organization_id==null?false:true}",
+                                            description='团支部ID'),
+                                  InputText(label='团支部名称', name='organization', value='${organization}',
+                                            required=False, trimContents=True, clearable=True,
+                                            showCounter=True, maxLength=36,
+                                            visibleOn="${organization==null?false:true}",
+                                            description='团支部名称'),
+                                  InputText(label='token', name='token', value='${token}', required=True,
+                                            trimContents=True, clearable=True,
+                                            showCounter=True, visibleOn="${token==null?false:true}",
+                                            description='提交大学习需要的token'),
+                                  InputText(label='cookie', name='cookie', value='${cookie}', required=True,
+                                            trimContents=True, clearable=True,
+                                            showCounter=True, visibleOn="${cookie==null?false:true}",
+                                            description='提交大学习需要的cookie')
+                              ])
+                      ])
+    ),
+    ActionType.Ajax(
+        label="提交大学习",
+        className='m-l',
+        level=LevelEnum.primary,
+        confirmText='是否提交最新一期青年大学习？',
+        api='get:/TeenStudy/api/commit?user_id=${user_id}&area=${area}'
+    ),
+    Switch(name='auto_submit',
+           value='${auto_submit}',
+           tooltip='自动提交大学习开关',
+           onText='自动开',
+           offText='自动关',
+           onEvent={
+               'change': {
+                   'actions': {
+                       'actionType': 'ajax',
+                       'args': {
+                           'api': {
+                               'url': '/TeenStudy/api/set_auto_submit',
+                               'method': 'put'
+                           },
+                           'messages': {
+                               'success': '自动提交已设置为${event.data.value==true?"开启":"关闭"}',
+                               'failed': '修改失败！'
+                           },
+                           'status': '${event.data.value}',
+                           'id': '${id}'
+                       }
+                   }
+               }
+           })
+])
+
+from_table = Service(
+    title="",
+    api={
+        "method": "get",
+        "url": "/TeenStudy/api/get_user",
+        "headers": {
+            "token": """${window.localStorage.getItem("token")}""",
+        }
+    },
+    interval=12000,
+    body=[
+        Property(
+            title='用户详细信息',
+            column=2,
+            items=[
+                Property.Item(
+                    label='用户ID',
+                    content='${user_id}'
+                ),
+                Property.Item(
+                    label='姓名',
+                    content='${name}'
+                ),
+                Property.Item(
+                    label='地区',
+                    content='${area}'
+                ),
+                Property.Item(
+                    label='学校',
+                    content='${university}'
+                ),
+                Property.Item(
+                    label='学院',
+                    content='${college}'
+                ),
+                Property.Item(
+                    label='团支部',
+                    content='${organization}'
+                ),
+                Property.Item(
+                    label='最新提交期数',
+                    content='${catalogue}'
+                ),
+                Property.Item(
+                    label='最新提交时间',
+                    content='${commit_time}'
+                ),
+                Property.Item(
+                    label='性别',
+                    content='${gender}',
+                    visibleOn="${gender==null?false:true}"
+                ),
+                Property.Item(
+                    label='手机号|学号',
+                    content='${mobile}',
+                    visibleOn="${mobile==null?false:true}"
+                ),
+                Property.Item(
+                    label='团支书ID',
+                    content='${leader}',
+                    visibleOn="${leader==null?false:true}"
+                ),
+                Property.Item(
+                    label='Uid|Nid',
+                    content='${dxx_id}',
+                    visibleOn="${dxx_id==null?false:true}"
+                ),
+                Property.Item(
+                    label='学校类型',
+                    content='${university_type}',
+                    visibleOn="${university_type==null?false:true}"
+                ),
+                Property.Item(
+                    label='学校ID',
+                    content='${university_id}',
+                    visibleOn="${university_id==null?false:true}"
+                ),
+                Property.Item(
+                    label='学院ID',
+                    content='${college_id}',
+                    visibleOn="${college_id==null?false:true}"
+                ),
+                Property.Item(
+                    label='团支部ID',
+                    content='${organization_id}',
+                    visibleOn="${organization_id==null?false:true}"
+                ), Property.Item(
+                    label='openid',
+                    content='${openid}',
+                    visibleOn="${openid==null?false:true}"
+                ), Property.Item(
+                    label='token',
+                    content='${token}',
+                    visibleOn="${token==null?false:true}",
+                    span=2
+                ), Property.Item(
+                    label='cookie',
+                    content='${cookie}',
+                    visibleOn="${cookie==null?false:true}",
+                    span=2
+                )
+            ]
+        )
+    ]
+)
+"""提交记录模板"""
+record_table = CRUD(mode='table',
+                    title='',
+                    syncLocation=False,
+                    api='/TeenStudy/api/get_records?user_id=${user_id}',
+                    type='crud',
+                    headerToolbar=[],
+                    itemActions=[],
+                    footable=True,
+                    columns=[
+                        TableColumn(label='用户ID', name='user_id'),
+                        TableColumn(label='姓名', name='name'),
+                        TableColumn(label='提交地区', name='area'),
+                        TableColumn(label='学校名称', name='university'),
+                        TableColumn(label='学院名称', name='college'),
+                        TableColumn(label='团支部', name='organization'),
+                        TableColumn(label='提交期数', name='catalogue', searchable=True),
+                        TableColumn(tppe="tpl", label='提交状态', tpl='${status===true?"成功":"失败"}', name="status",
+                                    searchable=True),
+                        TableColumn(type='tpl', tpl='${time|date:YYYY-MM-DD HH\\:mm\\:ss}',
+                                    label='提交时间',
+                                    name='time', sortable=True)
+                    ])
+answer_table = CRUD(mode='table',
+                    title='',
+                    syncLocation=False,
+                    api='/TeenStudy/api/get_answers',
+                    type='crud',
+                    headerToolbar=[],
+                    itemActions=[],
+                    footable=True,
+                    columns=[
+                        TableColumn(label='数据库ID', name='id'),
+                        TableColumn(label='大学习ID', name='code'),
+                        TableColumn(label='大学习期数', name='catalogue', searchable=True),
+                        TableColumn(type='tpl', tpl='${url|truncate:20}', label='官方网址',
+                                    name='url',
+                                    popOver={'mode': 'dialog', 'title': '完整网址',
+                                             'className': 'break-all',
+                                             'body': {'type': 'tpl',
+                                                      'tpl': '${url}'}}, copyable=True),
+                        TableColumn(type='tpl', tpl='${end_url|truncate:20}', label='完成截图网址',
+                                    name='end_url',
+                                    popOver={'mode': 'dialog', 'title': '完整网址',
+                                             'className': 'break-all',
+                                             'body': {'type': 'tpl',
+                                                      'tpl': '${end_url}'}}, copyable=True),
+                        TableColumn(type='tpl', tpl='${answer|truncate:20}', label='答案',
+                                    name='answer',
+                                    popOver={'mode': 'dialog', 'title': '完整答案',
+                                             'className': 'break-all',
+                                             'body': {'type': 'tpl',
+                                                      'tpl': '${answer}'}}),
+                        TableColumn(type='tpl', tpl='${time|date:YYYY-MM-DD HH\\:mm\\:ss}',
+                                    label='更新时间',
+                                    name='time', sortable=True)
+                    ])
+page_detail = Page(title='', body=[logo, operation_button, Divider(), from_table])
+home_page = PageSchema(url='/TeenStudy/home', label='首页', icon='fa fa-home', isDefaultPage=True, schema=page_detail)
+home_app = App(brandName='TeenStudy',
+               logo='https://img1.imgtp.com/2023/06/11/sG4KdlpL.png',
+               header=header,
+               pages=[{
+                   'children': [
+                       home_page,
+                       PageSchema(url="/TeenStudy/answer", label='大学习列表', icon='fa fa-book-open',
+                                  schema=Page(title='', body=[answer_table])),
+                       PageSchema(url="/TeenStudy/records", label='提交记录', icon='fa fa-code-commit',
+                                  schema=Page(title='', body=[record_table]))
+                   ]}],
+               footer=Html(
+                   html=f'<div class="p-2 text-center bg-blue-100">Copyright © 2022 - 2023 <a href="https://github.com/ZM25XC/TeenStudy" target="_blank" class="link-secondary">TeenStudy v0.2.0rc1</a> X<a target="_blank" href="https://github.com/baidu/amis" class="link-secondary" rel="noopener"> amis v3.1.1</a></div>'))
```

#### html2text {}

```diff
@@ -1,26 +1,31 @@
 from amis import App, PageSchema, Flex, ActionType, LevelEnum, Dialog, Form,
 DisplayModeEnum, InputText, TableColumn, \ CRUD, Tpl, Switch from amis import
 Html, Page, Property, Service, Divider logo = Html(html=f'''
                                   [TeenStudy]
                        ***** å¤§å­¦ä¹ èªå¨æäº¤ *****
-                            Githubä»åº äº¤æµç¾¤
+                      Githubä»åº äº¤æµç¾¤ QQä½éªç¾¤
 
 ''') github_logo = Tpl(className='w-full', tpl='
 ') header = Flex(className='w-full', justify='flex-end', alignItems='flex-end',
-items=[github_logo]) operation_button = Flex(justify='center', items=
-[ ActionType.Dialog( label='ä¿®æ¹ä¿¡æ¯', className='m-l',
-level=LevelEnum.primary, dialog=Dialog(title='ä¿®æ¹ä¿¡æ¯', size='lg', body=
-[ Form( title='', api='put:/TeenStudy/api/change?user_id=${user_id}',
-submitText='ä¿å­ä¿®æ¹', mode=DisplayModeEnum.horizontal, labelAlign='right',
-body=[ InputText(label='æ§å«', name='gender', value='${gender}',
-required=True, trimContents=True, clearable=True, showCounter=True,
-maxLength=3, visibleOn="${gender==null?false:true}", description='æ§å«'),
-InputText(label='uid|nid', name='dxx_id', value='${dxx_id}', required=True,
-trimContents=True, clearable=True, showCounter=True, maxLength=24, visibleOn="$
+items=[github_logo, { "type": "button", "label": "éåº", "onEvent":
+{ "click": { "actions": [ { "actionType": "confirmDialog", "args": { "title":
+"æä½ç¡®è®¤", "msg": "æ¯å¦éåºç³»ç»ï¼" }}, { "actionType": "custom",
+"script": "window.location.href = '/TeenStudy/login';window.localStorage.clear
+();window.sessionStorage.clear();\n //event.stopPropagation();" } ] }, }}])
+operation_button = Flex(justify='center', items=[ ActionType.Dialog
+( label='ä¿®æ¹ä¿¡æ¯', className='m-l', level=LevelEnum.primary, dialog=Dialog
+(title='ä¿®æ¹ä¿¡æ¯', size='lg', body=[ Form( title='', api='put:/TeenStudy/
+api/change?user_id=${user_id}', submitText='ä¿å­ä¿®æ¹',
+mode=DisplayModeEnum.horizontal, labelAlign='right', body=[ InputText
+(label='æ§å«', name='gender', value='${gender}', required=True,
+trimContents=True, clearable=True, showCounter=True, maxLength=3, visibleOn="$
+{gender==null?false:true}", description='æ§å«'), InputText(label='uid|nid',
+name='dxx_id', value='${dxx_id}', required=True, trimContents=True,
+clearable=True, showCounter=True, maxLength=24, visibleOn="$
 {dxx_id==null?false:true}",
 description='å¤§å­¦ä¹ è®¤è¯IDï¼ä¸æ¸æ¥è¯·å¿æ¹å¨'), InputText
 (label='ææºå·', name='mobile', value='${mobile}', required=True,
 trimContents=True, clearable=True, showCounter=True, maxLength=24, visibleOn="$
 {mobile==null?false:true}", description='ææºå·'), InputText
 (label='å¢æ¯ä¹¦ID', name='leader', value='${leader}', showCounter=True,
 maxLength=10, hiddenOn=True, trimContents=True, clearable=True,
@@ -31,15 +36,15 @@
 description='å¾®ä¿¡è®¤è¯IDï¼ä¸æ¸æ¥è¯·å¿æ¹å¨'), InputText
 (label='ç»å½å¯ç ', name='Password', value='', type="input-password",
 trimContents=True, clearable=True, showCounter=True, maxLength=16, visibleOn="$
 {password==null?false:true}", description='ç»å½Web UIçå¯ç '), InputText
 (label='å­¦æ ¡ç±»å', name='university_type', value='${university_type}',
 showCounter=True, maxLength=16, required=True, trimContents=True,
 clearable=True, visibleOn="${university_type==null?false:true}",
-description='å­¦æ ¡ç±»åï¼ä¸æ¸æ¥æ¸æ æ¹å¨'), InputText
+description='å­¦æ ¡ç±»åï¼ä¸æ¸æ¥è¯·å¿æ¹å¨'), InputText
 (label='å­¦æ ¡ID', name='university_id', value='${university_id}',
 required=True, trimContents=True, clearable=True, showCounter=True,
 maxLength=24, visibleOn="${university_id==null?false:true}",
 description='å­¦æ ¡IDï¼ä¸æ¸æ¥è¯·å¿æ¹å¨'), InputText
 (label='å­¦æ ¡åç§°', name='university', value='${university}', required=True,
 trimContents=True, clearable=True, showCounter=True, maxLength=20, visibleOn="$
 {university==null?false:true}", description='å­¦æ ¡åç§°'), InputText
@@ -63,21 +68,22 @@
 trimContents=True, clearable=True, showCounter=True, visibleOn="$
 {cookie==null?false:true}", description='æäº¤å¤§å­¦ä¹ éè¦çcookie') ]) ])
 ), ActionType.Ajax( label="æäº¤å¤§å­¦ä¹ ", className='m-l',
 level=LevelEnum.primary,
 confirmText='æ¯å¦æäº¤ææ°ä¸æéå¹´å¤§å­¦ä¹ ï¼', api='get:/TeenStudy/
 api/commit?user_id=${user_id}&area=${area}' ), Switch(name='auto_submit',
 value='${auto_submit}', tooltip='èªå¨æäº¤å¤§å­¦ä¹ å¼å³',
-onText='èªå¨æäº¤å¤§å­¦ä¹ å¼', offText='èªå¨æäº¤å¤§å­¦ä¹ å³', onEvent=
-{ 'change': { 'actions': { 'actionType': 'ajax', 'args': { 'api': { 'url': '/
-TeenStudy/api/set_auto_submit', 'method': 'put' }, 'messages': { 'success':
+onText='èªå¨å¼', offText='èªå¨å³', onEvent={ 'change': { 'actions':
+{ 'actionType': 'ajax', 'args': { 'api': { 'url': '/TeenStudy/api/
+set_auto_submit', 'method': 'put' }, 'messages': { 'success':
 'èªå¨æäº¤å·²è®¾ç½®ä¸º${event.data.value==true?"å¼å¯":"å³é­"}',
 'failed': 'ä¿®æ¹å¤±è´¥ï¼' }, 'status': '${event.data.value}', 'id': '${id}' }
-} } }) ]) from_table = Service( title="", api="/TeenStudy/api/
-get_user?user_id=${user_id}", interval=12000, body=[ Property
+} } }) ]) from_table = Service( title="", api={ "method": "get", "url": "/
+TeenStudy/api/get_user", "headers": { "token": """${window.localStorage.getItem
+("token")}""", } }, interval=12000, body=[ Property
 ( title='ç¨æ·è¯¦ç»ä¿¡æ¯', column=2, items=[ Property.Item
 ( label='ç¨æ·ID', content='${user_id}' ), Property.Item( label='å§å',
 content='${name}' ), Property.Item( label='å°åº', content='${area}' ),
 Property.Item( label='å­¦æ ¡', content='${university}' ), Property.Item
 ( label='å­¦é¢', content='${college}' ), Property.Item( label='å¢æ¯é¨',
 content='${organization}' ), Property.Item( label='ææ°æäº¤ææ°',
 content='${catalogue}' ), Property.Item( label='ææ°æäº¤æ¶é´', content='$
@@ -102,35 +108,37 @@
 TeenStudy/api/get_records?user_id=${user_id}', type='crud', headerToolbar=[],
 itemActions=[], footable=True, columns=[ TableColumn(label='ç¨æ·ID',
 name='user_id'), TableColumn(label='å§å', name='name'), TableColumn
 (label='æäº¤å°åº', name='area'), TableColumn(label='å­¦æ ¡åç§°',
 name='university'), TableColumn(label='å­¦é¢åç§°', name='college'),
 TableColumn(label='å¢æ¯é¨', name='organization'), TableColumn
 (label='æäº¤ææ°', name='catalogue', searchable=True), TableColumn
-(label='æäº¤ç¶æ', name='${status==true?"æå":"å¤±è´¥"}'), TableColumn
-(type='tpl', tpl='${time|date:YYYY-MM-DD HH\\:mm\\:ss}', label='æäº¤æ¶é´',
-name='time', sortable=True) ]) answer_table = CRUD(mode='table', title='',
-syncLocation=False, api='/TeenStudy/api/get_answers', type='crud',
-headerToolbar=[], itemActions=[], footable=True, columns=[ TableColumn
-(label='æ°æ®åºID', name='id'), TableColumn(label='å¤§å­¦ä¹ ID',
-name='code'), TableColumn(label='å¤§å­¦ä¹ ææ°', name='catalogue',
-searchable=True), TableColumn(type='tpl', tpl='${url|truncate:20}',
-label='å®æ¹ç½å', name='url', popOver={'mode': 'dialog', 'title':
-'å®æ´ç½å', 'className': 'break-all', 'body': {'type': 'tpl', 'tpl': '$
-{url}'}}, copyable=True), TableColumn(type='tpl', tpl='${end_url|truncate:20}',
-label='å®ææªå¾ç½å', name='end_url', popOver={'mode': 'dialog', 'title':
-'å®æ´ç½å', 'className': 'break-all', 'body': {'type': 'tpl', 'tpl': '$
-{end_url}'}}, copyable=True), TableColumn(type='tpl', tpl='${answer|truncate:
-20}', label='ç­æ¡', name='answer', popOver={'mode': 'dialog', 'title':
+(tppe="tpl", label='æäº¤ç¶æ', tpl='${status===true?"æå":"å¤±è´¥"}',
+name="status", searchable=True), TableColumn(type='tpl', tpl='${time|date:YYYY-
+MM-DD HH\\:mm\\:ss}', label='æäº¤æ¶é´', name='time', sortable=True) ])
+answer_table = CRUD(mode='table', title='', syncLocation=False, api='/
+TeenStudy/api/get_answers', type='crud', headerToolbar=[], itemActions=[],
+footable=True, columns=[ TableColumn(label='æ°æ®åºID', name='id'),
+TableColumn(label='å¤§å­¦ä¹ ID', name='code'), TableColumn
+(label='å¤§å­¦ä¹ ææ°', name='catalogue', searchable=True), TableColumn
+(type='tpl', tpl='${url|truncate:20}', label='å®æ¹ç½å', name='url',
+popOver={'mode': 'dialog', 'title': 'å®æ´ç½å', 'className': 'break-all',
+'body': {'type': 'tpl', 'tpl': '${url}'}}, copyable=True), TableColumn
+(type='tpl', tpl='${end_url|truncate:20}', label='å®ææªå¾ç½å',
+name='end_url', popOver={'mode': 'dialog', 'title': 'å®æ´ç½å',
+'className': 'break-all', 'body': {'type': 'tpl', 'tpl': '${end_url}'}},
+copyable=True), TableColumn(type='tpl', tpl='${answer|truncate:20}',
+label='ç­æ¡', name='answer', popOver={'mode': 'dialog', 'title':
 'å®æ´ç­æ¡', 'className': 'break-all', 'body': {'type': 'tpl', 'tpl': '$
 {answer}'}}), TableColumn(type='tpl', tpl='${time|date:YYYY-MM-DD HH\\:mm\\:
 ss}', label='æ´æ°æ¶é´', name='time', sortable=True) ]) page_detail = Page
 (title='', body=[logo, operation_button, Divider(), from_table]) home_page =
-PageSchema(url='/home', label='é¦é¡µ', icon='fa fa-home', isDefaultPage=True,
-schema=page_detail) home_app = App(brandName='TeenStudy', logo='https://
-i.328888.xyz/2023/02/23/xIh5k.png', header=header, pages=[{ 'children':
-[ home_page, PageSchema(url="answer", label='å¤§å­¦ä¹ åè¡¨', icon='fa fa-
-book-open', schema=Page(title='', body=[answer_table])), PageSchema(url="/
-records", label='æäº¤è®°å½', icon='fa fa-code-commit', schema=Page(title='',
-body=[record_table])) ]}], footer=Html( html=f'
-Copyright Â© 2022 - 2023 TeenStudy Xamis_v2.2.0
+PageSchema(url='/TeenStudy/home', label='é¦é¡µ', icon='fa fa-home',
+isDefaultPage=True, schema=page_detail) home_app = App(brandName='TeenStudy',
+logo='https://img1.imgtp.com/2023/06/11/sG4KdlpL.png', header=header, pages=[
+{ 'children': [ home_page, PageSchema(url="/TeenStudy/answer",
+label='å¤§å­¦ä¹ åè¡¨', icon='fa fa-book-open', schema=Page(title='', body=
+[answer_table])), PageSchema(url="/TeenStudy/records", label='æäº¤è®°å½',
+icon='fa fa-code-commit', schema=Page(title='', body=[record_table])) ]}],
+footer=Html( html=f'
+Copyright Â© 2022 - 2023 TeenStudy_v0.2.0rc1 Xamis_v3.1.1
 '))
```

### Comparing `TeenStudy-0.1.9/TeenStudy/web/pages/login.py` & `teenstudy-0.2.0rc1/TeenStudy/web/pages/login.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,42 +1,47 @@
-from amis import Form, InputText, InputPassword, DisplayModeEnum, Horizontal, Remark, Html, Page, AmisAPI, Wrapper, \
-    Switch
-
-logo = Html(html=f'''
-<p align="center">
-    <a href="https://github.com/ZM25XC/TeenStudy/">
-        <img src="https://i.328888.xyz/2023/02/23/xIh5k.png"
-         width="256" height="256" alt="TeenStudy">
-    </a>
-</p>
-<h2 align="center">大学习自动提交</h2>
-<div align="center">
-    <a href="https://github.com/ZM25XC/TeenStudy/" target="_blank">
-    Github仓库</a>
-    <a href="https://jq.qq.com/?_wv=1027&k=NGFEwXyS" target="_blank">交流群</a>
-</div>
-<br>
-<br>
-''')
-login_api = AmisAPI(
-    url='/TeenStudy/api/login',
-    method='post',
-    adaptor='''
-        if (payload.status == 0) {
-            localStorage.setItem("token", payload.data.token);
-            localStorage.setItem("user_id", payload.data.user_id);
-            localStorage.setItem("role", payload.data.role);
-        }
-        return payload;
-    '''
-)
-
-login_form = Form(api=login_api, title='', body=[
-    InputText(name='user_id', label='用户ID', description='默认为用户QQ号'),
-    InputPassword(name='password', label='密码',
-                  description='管理员默认为admin，普通用户默认为QQ号'),
-    Switch(name='role', label='身份组', onText='管理员', offText='用户', value=False,
-           labelRemark=Remark(shape='circle', content='是否以管理员身份登录'))
-], mode=DisplayModeEnum.horizontal, horizontal=Horizontal(left=3, right=9, offset=5),
-                  redirect='${url}', submitText="登录")
-body = Wrapper(className='w-2/5 mx-auto my-0 m:w-full', body=login_form)
-login_page = Page(title='', body=[logo, body])
+from amis import Form, InputText, InputPassword, DisplayModeEnum, Horizontal, Remark, Html, Page, AmisAPI, Wrapper, \
+    Switch
+
+logo = Html(html=f'''
+<p align="center">
+    <a href="https://github.com/ZM25XC/TeenStudy/">
+        <img src="https://i.imgloc.com/2023/05/20/VyRjTV.png"
+         width="256" height="256" alt="TeenStudy">
+    </a>
+</p>
+<h2 align="center">大学习自动提交</h2>
+<div align="center">
+    <a href="https://github.com/ZM25XC/TeenStudy/" target="_blank">
+    Github仓库</a>
+    <a href="https://jq.qq.com/?_wv=1027&k=NGFEwXyS" target="_blank">QQ反馈群</a>
+    <a href="http://qm.qq.com/cgi-bin/qm/qr?_wv=1027&k=2PQucjirnkHyPjoS1Pkr-ai2aPGToBKm" target="_blank">QQ体验群</a>
+</div>
+<br>
+<br>
+''')
+login_api = AmisAPI(
+    url='/TeenStudy/api/login',
+    method='post',
+    adaptor='''
+        if (payload.status == 0) {
+            localStorage.setItem("token", payload.data.token);
+            localStorage.setItem("user_id", payload.data.user_id);
+            localStorage.setItem("role", payload.data.role);
+            if(payload.data.role){
+            window.location.href = '/TeenStudy/admin'
+            }
+            else{
+            window.location.href = '/TeenStudy/home?user_id='+payload.data.user_id;}
+        }
+        return payload;
+    '''
+)
+
+login_form = Form(api=login_api, title='', body=[
+    InputText(name='user_id', label='用户ID', description='默认为用户QQ号'),
+    InputPassword(name='password', label='密码',
+                  description='管理员默认为admin，普通用户默认为QQ号'),
+    Switch(name='role', label='身份组', onText='管理员', offText='用户', value=False,
+           labelRemark=Remark(shape='circle', content='是否以管理员身份登录'))
+], mode=DisplayModeEnum.horizontal, horizontal=Horizontal(left=3, right=9, offset=5), submitText="登录")
+body = Wrapper(className='w-2/5 mx-auto my-0 m:w-full', body=login_form)
+login_page = Page(title='', body=[logo, body])
```

#### html2text {}

```diff
@@ -1,21 +1,23 @@
 from amis import Form, InputText, InputPassword, DisplayModeEnum, Horizontal,
 Remark, Html, Page, AmisAPI, Wrapper, \ Switch logo = Html(html=f'''
                                   [TeenStudy]
                        ***** å¤§å­¦ä¹ èªå¨æäº¤ *****
-                            Githubä»åº äº¤æµç¾¤
+                     Githubä»åº QQåé¦ç¾¤ QQä½éªç¾¤
 
 
 ''') login_api = AmisAPI( url='/TeenStudy/api/login', method='post',
 adaptor=''' if (payload.status == 0) { localStorage.setItem("token",
 payload.data.token); localStorage.setItem("user_id", payload.data.user_id);
-localStorage.setItem("role", payload.data.role); } return payload; ''' )
+localStorage.setItem("role", payload.data.role); if(payload.data.role)
+{ window.location.href = '/TeenStudy/admin' } else{ window.location.href = '/
+TeenStudy/home?user_id='+payload.data.user_id;} } return payload; ''' )
 login_form = Form(api=login_api, title='', body=[ InputText(name='user_id',
 label='ç¨æ·ID', description='é»è®¤ä¸ºç¨æ·QQå·'), InputPassword
 (name='password', label='å¯ç ',
 description='ç®¡çåé»è®¤ä¸ºadminï¼æ®éç¨æ·é»è®¤ä¸ºQQå·'), Switch
 (name='role', label='èº«ä»½ç»', onText='ç®¡çå', offText='ç¨æ·',
 value=False, labelRemark=Remark(shape='circle',
 content='æ¯å¦ä»¥ç®¡çåèº«ä»½ç»å½')) ], mode=DisplayModeEnum.horizontal,
-horizontal=Horizontal(left=3, right=9, offset=5), redirect='${url}',
-submitText="ç»å½") body = Wrapper(className='w-2/5 mx-auto my-0 m:w-full',
-body=login_form) login_page = Page(title='', body=[logo, body])
+horizontal=Horizontal(left=3, right=9, offset=5), submitText="ç»å½") body =
+Wrapper(className='w-2/5 mx-auto my-0 m:w-full', body=login_form) login_page =
+Page(title='', body=[logo, body])
```

### Comparing `TeenStudy-0.1.9/TeenStudy/web/utils/status.py` & `teenstudy-0.2.0rc1/TeenStudy/web/utils/status.py`

 * *Ordering differences only*

 * *Files 14% similar despite different names*

```diff
@@ -1,65 +1,65 @@
-import asyncio
-import datetime
-
-import psutil
-from nonebot import get_bot, get_driver
-
-from ...models.accuont import User
-from ...models.dxx import PushList, Answer, Area
-from ...utils.path import getConfig
-
-DRIVER = get_driver()
-start_time: str = ""
-
-
-async def get_status():
-    status_result = {
-    }
-    try:
-        status_result['start_time'] = start_time
-    except Exception:
-        status_result['start_time'] = '未知'
-    try:
-        bot = get_bot()
-        bot_info = await bot.get_login_info()
-        status_result['bot_id'] = bot_info['user_id']
-        status_result['nickname'] = bot_info['nickname']
-        bot_friends = await bot.get_friend_list()
-        bot_groups = await bot.get_group_list()
-        status_result['friend_count'] = len(bot_friends)
-        status_result['group_count'] = len(bot_groups)
-        status_result['user_count'] = await User.all().count()
-        status_result['area_count'] = await Area.all().count()
-        answer = await Answer.all().order_by("time").values()
-        title = answer[-1]["catalogue"]
-        setting = getConfig()
-        status_result["ip"] = setting["DXX_IP"]
-        status_result['catalogue'] = title
-        status_result['notice_count'] = await PushList.all().count()
-    except Exception:
-        status_result['bot_id'] = '未知'
-        status_result['msg_received'] = '未知'
-        status_result['msg_sent'] = '未知'
-
-    status_result['system_start_time'] = datetime.datetime.fromtimestamp(psutil.boot_time()).strftime(
-        "%Y-%m-%d %H:%M:%S")
-
-    psutil.cpu_percent()
-    await asyncio.sleep(0.1)
-    cpu_percent = psutil.cpu_percent()
-    # cpu_count = psutil.cpu_count(logical=False)
-    # cpu_count_logical = psutil.cpu_count()
-    # cpu_freq = psutil.cpu_freq()
-    ram_stat = psutil.virtual_memory()
-    swap_stat = psutil.swap_memory()
-    status_result['cpu_percent'] = f'{cpu_percent}%'
-    status_result['ram_percent'] = f'{ram_stat.percent}%'
-    status_result['swap_percent'] = f'{swap_stat.percent}%'
-
-    return status_result
-
-
-@DRIVER.on_startup
-async def start_up():
-    global start_time
-    start_time = datetime.datetime.now().strftime('%Y-%m-%d %H:%M:%S')
+import asyncio
+import datetime
+
+import psutil
+from nonebot import get_bot, get_driver
+
+from ...models.accuont import User
+from ...models.dxx import PushList, Answer, Area
+from ...utils.path import getConfig
+
+DRIVER = get_driver()
+start_time: str = ""
+
+
+async def get_status():
+    status_result = {
+    }
+    try:
+        status_result['start_time'] = start_time
+    except Exception:
+        status_result['start_time'] = '未知'
+    try:
+        bot = get_bot()
+        bot_info = await bot.get_login_info()
+        status_result['bot_id'] = bot_info['user_id']
+        status_result['nickname'] = bot_info['nickname']
+        bot_friends = await bot.get_friend_list()
+        bot_groups = await bot.get_group_list()
+        status_result['friend_count'] = len(bot_friends)
+        status_result['group_count'] = len(bot_groups)
+        status_result['user_count'] = await User.all().count()
+        status_result['area_count'] = await Area.all().count()
+        answer = await Answer.all().order_by("time").values()
+        title = answer[-1]["catalogue"]
+        setting = getConfig()
+        status_result["ip"] = setting["DXX_IP"]
+        status_result['catalogue'] = title
+        status_result['notice_count'] = await PushList.all().count()
+    except Exception:
+        status_result['bot_id'] = '未知'
+        status_result['msg_received'] = '未知'
+        status_result['msg_sent'] = '未知'
+
+    status_result['system_start_time'] = datetime.datetime.fromtimestamp(psutil.boot_time()).strftime(
+        "%Y-%m-%d %H:%M:%S")
+
+    psutil.cpu_percent()
+    await asyncio.sleep(0.1)
+    cpu_percent = psutil.cpu_percent()
+    # cpu_count = psutil.cpu_count(logical=False)
+    # cpu_count_logical = psutil.cpu_count()
+    # cpu_freq = psutil.cpu_freq()
+    ram_stat = psutil.virtual_memory()
+    swap_stat = psutil.swap_memory()
+    status_result['cpu_percent'] = f'{cpu_percent}%'
+    status_result['ram_percent'] = f'{ram_stat.percent}%'
+    status_result['swap_percent'] = f'{swap_stat.percent}%'
+
+    return status_result
+
+
+@DRIVER.on_startup
+async def start_up():
+    global start_time
+    start_time = datetime.datetime.now().strftime('%Y-%m-%d %H:%M:%S')
```

### Comparing `TeenStudy-0.1.9/setup.py` & `teenstudy-0.2.0rc1/PKG-INFO`

 * *Files 14% similar despite different names*

```diff
@@ -1,53 +1,300 @@
-# -*- coding: utf-8 -*-
-from setuptools import setup
+Metadata-Version: 2.1
+Name: teenstudy
+Version: 0.2.0rc1
+Summary: 基于nonebot2异步框架的青年大学自动提交插件基于nonebot2的青年大学习自动提交插件，用于自动完成大学习，在后台留下记录，返回完成截图
+Home-page: https://github.com/ZM25XC/TeenStudy
+License: MIT
+Author: ZM25XC
+Author-email: xingling25@qq.com
+Requires-Python: >=3.8,<4.0
+Classifier: License :: OSI Approved :: MIT License
+Classifier: Programming Language :: Python :: 3
+Classifier: Programming Language :: Python :: 3.8
+Classifier: Programming Language :: Python :: 3.9
+Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
+Requires-Dist: Jinja2 (>=3.1.2,<4.0.0)
+Requires-Dist: amis-python (>=1.0.8,<2.0.0)
+Requires-Dist: anti-useragent (>=1.0.10,<2.0.0)
+Requires-Dist: beautifulsoup4 (>=4.11.2,<5.0.0)
+Requires-Dist: bs4 (>=0.0.1,<0.0.2)
+Requires-Dist: ddddocr (>=1.4.7,<2.0.0)
+Requires-Dist: fastapi (>=0.95.0,<0.96.0)
+Requires-Dist: httpx (>=0.24.0,<0.25.0)
+Requires-Dist: lxml (>=4.9.2,<5.0.0)
+Requires-Dist: nonebot-adapter-onebot (>=2.2.3,<3.0.0)
+Requires-Dist: nonebot-plugin-apscheduler (>=0.3.0,<0.4.0)
+Requires-Dist: nonebot2 (>=2.0.0,<3.0.0)
+Requires-Dist: psutil (>=5.9.4,<6.0.0)
+Requires-Dist: pycryptodome (>=3.17,<4.0)
+Requires-Dist: python-jose (>=3.3.0,<4.0.0)
+Requires-Dist: qrcode (>=7.4.2,<8.0.0)
+Requires-Dist: tortoise-orm (>=0.19.3,<0.20.0)
+Requires-Dist: ujson (>=5.7.0,<6.0.0)
+Requires-Dist: uvicorn (>=0.21.0,<0.22.0)
+Description-Content-Type: text/markdown
 
-packages = \
-['teenstudy',
- 'teenstudy.models',
- 'teenstudy.utils',
- 'teenstudy.web',
- 'teenstudy.web.api',
- 'teenstudy.web.pages',
- 'teenstudy.web.utils']
-
-package_data = \
-{'': ['*'], 'teenstudy': ['resource/*']}
-
-install_requires = \
-['Jinja2>=3.1.2,<4.0.0',
- 'Pillow>=9.4.0,<10.0.0',
- 'amis-python>=1.0.7,<2.0.0',
- 'anti-useragent>=1.0.10,<2.0.0',
- 'beautifulsoup4>=4.11.2,<5.0.0',
- 'bs4>=0.0.1,<0.0.2',
- 'fastapi>=0.95.0,<0.96.0',
- 'httpx>=0.23.3,<0.24.0',
- 'lxml>=4.9.2,<5.0.0',
- 'nonebot-adapter-onebot>=2.2.1,<3.0.0',
- 'nonebot-plugin-apscheduler>=0.2.0,<0.3.0',
- 'nonebot2>=2.0.0rc2,<3.0.0',
- 'psutil>=5.9.4,<6.0.0',
- 'python-jose>=3.3.0,<4.0.0',
- 'qrcode>=7.4.2,<8.0.0',
- 'tortoise-orm>=0.19.3,<0.20.0',
- 'ujson>=5.7.0,<6.0.0',
- 'uvicorn>=0.21.0,<0.22.0']
-
-setup_kwargs = {
-    'name': 'teenstudy',
-    'version': '0.1.9',
-    'description': '基于nonebot2异步框架的青年大学自动提交插件基于nonebot2的青年大学习自动提交插件，用于自动完成大学习，在后台留下记录，返回完成截图',
-    'long_description': '<div align="center">\n    <img src="https://i.328888.xyz/2023/02/28/z23ho.png" alt="TeenStudy.png" border="0" width="500px" height="500px"/>\n    <h1>TeenStudy</h1>\n    <b>基于nonebot2和go-cqhttp的青年大学习自动提交插件，用于自动完成大学习，在后台留下记录，返回完成截图</b>\n    <br/>\n    <a href="https://github.com/ZM25XC/TeenStudy/issues"><img alt="GitHub issues" src="https://img.shields.io/github/issues/ZM25XC/TeenStudy?style=flat-square"></a>\n    <a href="https://github.com/ZM25XC/TeenStudy/network"><img alt="GitHub forks" src="https://img.shields.io/github/forks/ZM25XC/TeenStudy?style=flat-square"></a>\n    <a href="https://github.com/ZM25XC/TeenStudy/stargazers"><img alt="GitHub stars" src="https://img.shields.io/github/stars/ZM25XC/TeenStudy?style=flat-square"></a>\n    <a href="https://pypi.python.org/pypi/TeenStudy"><img src="https://img.shields.io/pypi/v/TeenStudy?color=yellow" alt="pypi"></a>\n  \t<a href="https://pypi.python.org/pypi/TeenStudy">\n    <img src="https://img.shields.io/pypi/dm/TeenStudy" alt="pypi download"></a>\n\t  <a href="https://github.com/ZM25XC/TeenStudy/blob/main/LICENSE"><img alt="GitHub license" src="https://img.shields.io/github/license/ZM25XC/TeenStudy?style=flat-square"></a>\n    <a href="https://jq.qq.com/?_wv=1027&k=NGFEwXyS">\n    <img src="https://img.shields.io/badge/QQ%E7%BE%A4-511173803-orange?style=flat-square" alt="QQ Chat Group">\n  </a>\n  </div>\n\n## 说明\n\n- 本项目为[青年大学习提交](https://github.com/ZM25XC/nonebot_plugin_auto_teenstudy) `Web UI`版\n- 本项目基于[nonebot2](https://github.com/nonebot/nonebot2)和[go-cqhttp](https://github.com/Mrs4s/go-cqhttp)，使用本插件前请先阅读以上两个项目的使用文档\n-  **启动插件之后，一定要登录后台在推送列表中添加需要开启大学习功能的群聊**\n-  **本项目无法在国外IP环境下使用，如有开启代理，请关闭或添加代理规则**\n- 需要抓包的地区，绑定后尽量别进官方公众号，避免token或cookie刷新导致无法提交\n- 本项目需要部署在公网可访问的容器中，并开放端口（nonebot2配置的port），否则大部分功能将出现异常\n- 欢迎加入[QQ群](https://jq.qq.com/?_wv=1027&k=NGFEwXyS)，交流讨论。\n- 时间精力有限，目前只维护湖北和江西两个地区，其他地区出问题请提交Issues,我找个时间修，需要增加地区请进群帮忙测试，个别地区没账号无法测试\n\n- 觉得项目不错，不妨点个stars.\n\n## 地区状态\n\n<details>\n\n| 共青团名称 | 开发状态 | 备注 |\n|:-----:|:----:|:----:|\n|青春湖北|支持|无需抓包|\n|江西共青团|支持|无需抓包|\n|安徽共青团|支持|无需抓包|\n|广东共青团|支持|无需抓包|\n|青春上海|支持|微信扫码绑定|\n|青春浙江|支持|微信扫码绑定|\n|江苏共青团|支持|需要自行抓包|\n|青春山东|支持|需要自行抓包|\n|重庆共青团|支持|需要自行抓包|\n|吉青飞扬|支持|需要自行抓包|\n|黑龙江共青团|支持|需要自行抓包，该地区上线测试中|\n|天府新青年|支持|不进入公众号token时效大于1周|\n|河南共青团|不支持|cookie时效小于1周|\n|广西青年圈|待开发||\n|青春湖南|待开发||\n|甘肃青年|待开发||\n|山西青年|待开发||\n|河北共青团|待开发||\n|福建共青团|待开发||\n|内蒙古青年|待开发||\n|云南共青团|待开发||\n|三秦青年|待开发||\n|青春北京|待开发||\n|海南共青团|待开发||\n|津彩青春|待开发||\n|青春黔言|待开发||\n|青春柳州|待开发||\n|辽宁共青团|待开发||\n|宁夏共青团|待开发||\n|新疆共青团|待开发||\n|西藏共青团|待开发||\n</details>\n\n\n##  安装及更新\n\n<details>\n<summary>第一种方式(不推荐)</summary>\n\n- 使用`git clone https://github.com/ZM25XC/TeenStudy.git`指令克隆本仓库或下载压缩包文件\n\n</details>\n\n<details>\n<summary>第二种方式(二选一)</summary>\n\n- 使用`pip install TeenStudy`来进行安装,使用`pip install TeenStudy -U`进行更新\n- 使用`nb plugin install TeenStudy`来进行安装,使用`nb plugin install TeenStudy -U`进行更新\n\n</details>\n\n\n## 导入插件\n\n<details>\n<summary>使用第一种方式安装看此方法</summary>\n\n- 将`TeenStudy`放在nb的`plugins`目录下，运行nb机器人即可\n\n- 文件结构如下\n\n    ```py\n    📦 AweSome-Bot\n    ├── 📂 awesome_bot\n    │   └── 📂 plugins\n    |       └── 📂 TeenStudy\n    |           └── 📜 __init__.py\n    ├── 📜 .env.prod\n    ├── 📜 .gitignore\n    ├── 📜 pyproject.toml\n    └── 📜 README.md\n    ```\n\n    \n\n</details>\n\n<details>\n<summary>使用第二种方式安装看此方法</summary>\n\n- 在`pyproject.toml`里的`[tool.nonebot]`中添加`plugins = ["TeenStudy"]`\n\n</details>\n\n## 机器人配置\n\n- 在nonebot的`.env` 或 `.env.prod`配置文件中修改nonebot2的`HOST`为`0.0.0.0`、设置好超管账号和公网IP\n\n  ```py\n  HOST = "0.0.0.0"  #nonebot2监听的IP\n  SUPERUSERS = [""] # 超级用户\n  COMMAND_START=[""] # 命令前缀,根据需要自行修改\n  DXX_IP = ""\n  ```\n\n## 使用方式\n\n- 启动nb,等待插件加载数据，加载完毕后登录后台，账号默认为`nonebot配置文件中的超管账号`，密码默认为：`admin`,开放端口（默认为.env中配置的port）\n- 在管理后台的推送列表中添加需要开启大学习使用的群聊\n\n## 功能列表\n|    指令    |               指令格式               |                               说明                               |\n| :--------: | :----------------------------------: | :--------------------------------------------------------------: |\n| 添加大学习 |           添加大学习`地区`           |                    添加大学习湖北 添加大学习                     |\n| 我的大学习 |              我的大学习              |                           查询个人信息                           |\n| 提交大学习 |         提交大学习 戳一戳Bot         |                        提交最新一期大学习                        |\n|   大学习   |     大学习答案、大学习、答案截图     |                    获取最新一期青年大学习答案                    |\n|  完成截图  | 完成截图、大学习截图、大学习完成截图 |            获取最新一期青年大学习完成截图（带状态栏）            |\n| 完成大学习 |        完成大学习、全员大学习        | 团支书可用，需要成员填写团支书ID，填写后团支书可发指令提交大学习 |\n|  重置配置  |          重置配置、刷新配置          |                   超管可用，刷新Web UI默认配置                   |\n|  重置密码  |               重置密码               |                   重置登录Web UI的密码为用户ID                   |\n|删除大学习|删除大学习|用户申请清除数据库的信息|\n|导出用户数据|导出用户数据、导出数据|将数据导出至TeenStudy目录下|\n|更新用户数据|更新用户数据、刷新用户数据|将用户数据导入到数据库|\n|更新资源数据|更新资源数据、刷新资源数据|更新数据库中的资源数据（江西共青团团支部数据）|\n\n\n## ToDo\n\n\n- [ ] 增加更多地区支持\n- [ ] 优化 Bot\n\n\n## 更新日志\n\n### 2023/05/21\n\n- 增加黑龙江地区，需要自行抓包，该地区上线测试中，请积极提issue反馈\n- 下版本为大版本更新，将添加新功能，优化功能，请积极提issue反馈或加交流群反馈\n\n<details>\n<summary>2023/05/11</summary> \n\n- 增加广东地区，无需抓包[#13](https://github.com/ZM25XC/TeenStudy/issues/13)，感谢[@neal240](https://github.com/neal240)提供账号测试\n\n</details>\n\n<details>\n<summary>2023/05/06</summary> \n\n- 增加吉林地区，需要自行抓包\n- 修复超管更改登录密码后用原密码能继续登录问题\n- 添加二维码转链接开关，需要自行在后台配置页面打开\n- 调整部分依赖\n\n</details>\n\n<details>\n<summary> 2023/04/12</summary> \n\n- 因河南地区cookie时效小于1周，移除河南地区\n- 添加`删除大学习`功能，用户可自行删除数据\n- 添加`导出用户数据`功能\n- 添加`更新用户数据`功能\n- 添加`更新资源数据`功能，江西地区更新后请使用下此功能刷新团支部数据\n- 添加戳一戳提交大学习开关，默认开启，请在Web UI后台配置页面进行修改\n- 添加大学习提醒开关，默认开启，支持修改时间，请在Web UI后台配置页面进行修改\n- 添加自动提交大学习开关，默认开启，支持修改时间，请在Web UI后台进行修改\n- 调整安徽地区添加方式[#9](https://github.com/ZM25XC/TeenStudy/issues/9)，无需抓包，感谢[@yhzcake](https://github.com/yhzcake)测试提供方法\n- 修复Web UI 首页公网IP显示异常\n- 修复浙江地区用户重复显示\n- 更新江西共青团团支部数据\n  \n</details>\n\n\n<details>\n<summary>2023/03/18</summary>\n\n- 适配河南地区，需要自行抓包\n- 适配四川地区，需要自行抓包\n- 适配山东地区，需要自行抓包\n- 适配重庆地区，需要自行抓包\n- 添加自动获取公网IP功能，别再问如何配置公网IP啦\n- 添加重置密码功能，指令`重置密码`\n- 添加重置配置功能，指令`重置配置`，`刷新配置`\n- 添加完成大学习功能，团支书可一次性提交全班的大学习，指令`完成大学习`，`全员大学习`\n- 管理后台开放添加用户权限（浙江，上海地区无法添加）\n- 优化用户信息页\n- 优化登录界面提示\n- 将添加链接，登录链接转化成二维码，减少公网IP暴露，没啥用，样式好看一些\n- 修复Ubuntu系统导入资源失败BUG\n  \n</details>\n\n<details>\n\n<summary>2023/03/05</summary>\n\n- 适配浙江地区，使用微信扫码进行绑定\n- 适配上海地区，使用微信扫码进行绑定\n- 适配江苏地区，需要自行抓包\n- 适配安徽地区，需要自行抓包\n\n</details>\n\n<details>\n<summary>2023/03/01</summary>\n\n- 将代码上传至pypi，可使用`pip install TeenStudy`指令安装本插件\n- 上传基础代码\n- 适配湖北地区，无需抓包，安装即用\n- 适配江西地区，无需抓包，安装即用\n\n</details>\n',
-    'author': 'ZM25XC',
-    'author_email': 'xingling25@qq.com',
-    'maintainer': 'None',
-    'maintainer_email': 'None',
-    'url': 'https://github.com/ZM25XC/TeenStudy',
-    'packages': packages,
-    'package_data': package_data,
-    'install_requires': install_requires,
-    'python_requires': '>=3.8,<4.0',
-}
+<div align="center">
+    <img src="https://img1.imgtp.com/2023/06/11/sG4KdlpL.png" alt="TeenStudy.png" border="0" width="500px" height="500px"/>
+    <h1>TeenStudy</h1>
+    <b>基于nonebot2和go-cqhttp的青年大学习自动提交插件，用于自动完成大学习，在后台留下记录，返回完成截图</b>
+    <br/>
+    <a href="https://github.com/ZM25XC/TeenStudy/issues"><img alt="GitHub issues" src="https://img.shields.io/github/issues/ZM25XC/TeenStudy?style=flat-square"></a>
+    <a href="https://github.com/ZM25XC/TeenStudy/network"><img alt="GitHub forks" src="https://img.shields.io/github/forks/ZM25XC/TeenStudy?style=flat-square"></a>
+    <a href="https://github.com/ZM25XC/TeenStudy/stargazers"><img alt="GitHub stars" src="https://img.shields.io/github/stars/ZM25XC/TeenStudy?style=flat-square"></a>
+    <a href="https://pypi.python.org/pypi/TeenStudy"><img src="https://img.shields.io/pypi/v/TeenStudy?color=yellow" alt="pypi"></a>
+  	<a href="https://pypi.python.org/pypi/TeenStudy">
+    <img src="https://img.shields.io/pypi/dm/TeenStudy" alt="pypi download"></a>
+	  <a href="https://github.com/ZM25XC/TeenStudy/blob/main/LICENSE"><img alt="GitHub license" src="https://img.shields.io/github/license/ZM25XC/TeenStudy?style=flat-square"></a>
+    <a href="https://jq.qq.com/?_wv=1027&k=NGFEwXyS">
+    <img src="https://img.shields.io/badge/QQ反馈群-511173803-orange?style=flat-square" alt="QQ Chat Group">
+  </a>
+	<a href="http://qm.qq.com/cgi-bin/qm/qr?_wv=1027&k=2PQucjirnkHyPjoS1Pkr-ai2aPGToBKm">
+    <img src="https://img.shields.io/badge/QQ体验群-821280615-orange?style=flat-square" alt="QQ Chat Group">
+  </a>
+  </div>
 
+## 说明
+
+- 本项目为[青年大学习提交](https://github.com/ZM25XC/nonebot_plugin_auto_teenstudy) `Web UI`版
+- 本项目基于[nonebot2](https://github.com/nonebot/nonebot2)和[go-cqhttp](https://github.com/Mrs4s/go-cqhttp)，使用本插件前请先阅读以上两个项目的使用文档
+-  **启动插件之后，一定要登录后台在推送列表中添加需要开启大学习功能的群聊**
+-  **本项目无法在国外IP环境下使用，如有开启代理，请关闭或添加代理规则**
+- 需要抓包的地区，绑定后尽量别进官方公众号，避免token或cookie刷新导致无法提交
+- 本项目需要部署在公网可访问的容器中，并开放端口（nonebot2配置的port），否则大部分功能将出现异常
+- 欢迎加入[QQ反馈群](https://jq.qq.com/?_wv=1027&k=NGFEwXyS)，交流讨论，如您不会搭建又想每周自动提交，可加入[QQ体验群](http://qm.qq.com/cgi-bin/qm/qr?_wv=1027&k=2PQucjirnkHyPjoS1Pkr-ai2aPGToBKm)。
+- 时间精力有限，目前只维护湖北和江西两个地区，其他地区出问题请提交Issues,我找个时间修，需要增加地区请进群帮忙测试，个别地区没账号无法测试
+
+- 觉得项目不错，不妨点个stars.
+
+## 地区状态
+
+<details>
+
+| 共青团名称 | 开发状态 | 备注 |
+|:-----:|:----:|:----:|
+|青春湖北|支持|无需抓包|
+|江西共青团|支持|无需抓包|
+|安徽共青团|支持|无需抓包|
+|广东共青团|支持|无需抓包|
+|青春北京|支持|无需抓包|
+|青春上海|支持|微信扫码绑定|
+|青春浙江|支持|微信扫码绑定|
+|津彩青春|支持|需要自行抓包|
+|青春山东|支持|需要自行抓包|
+|重庆共青团|支持|需要自行抓包|
+|吉青飞扬|支持|需要自行抓包|
+|天府新青年|支持|不进入公众号token时效大于1周|
+|河南共青团|不支持|cookie时效小于1周|
+|江苏共青团|不支持|cookie失效小于1周|
+|黑龙江共青团|不支持|cookie失效小于1周|
+|广西青年圈|待开发||
+|青春湖南|待开发||
+|甘肃青年|待开发||
+|山西青年|待开发||
+|河北共青团|待开发||
+|福建共青团|待开发||
+|内蒙古青年|待开发||
+|云南共青团|待开发||
+|三秦青年|待开发||
+|海南共青团|待开发||
+|青春黔言|待开发||
+|青春柳州|待开发||
+|辽宁共青团|待开发||
+|宁夏共青团|待开发||
+|新疆共青团|待开发||
+|西藏共青团|待开发||
+</details>
+
+
+##  安装及更新
+
+<details>
+<summary>第一种方式(不推荐)</summary>
+
+- 使用`git clone https://github.com/ZM25XC/TeenStudy.git`指令克隆本仓库或下载压缩包文件
+
+</details>
+
+<details>
+<summary>第二种方式(二选一)</summary>
+
+- 使用`pip install TeenStudy`来进行安装,使用`pip install TeenStudy -U`进行更新
+- 使用`nb plugin install TeenStudy`来进行安装,使用`nb plugin install TeenStudy -U`进行更新
+
+</details>
+
+
+## 导入插件
+
+<details>
+<summary>使用第一种方式安装看此方法</summary>
+
+- 将`TeenStudy`放在nb的`plugins`目录下，运行nb机器人即可
+
+- 文件结构如下
+
+    ```py
+    📦 AweSome-Bot
+    ├── 📂 awesome_bot
+    │   └── 📂 plugins
+    |       └── 📂 TeenStudy
+    |           └── 📜 __init__.py
+    ├── 📜 .env.prod
+    ├── 📜 .gitignore
+    ├── 📜 pyproject.toml
+    └── 📜 README.md
+    ```
+
+    
+
+</details>
+
+<details>
+<summary>使用第二种方式安装看此方法</summary>
+
+- 在`pyproject.toml`里的`[tool.nonebot]`中添加`plugins = ["TeenStudy"]`
+
+</details>
+
+## 机器人配置
+
+- 在nonebot的`.env` 或 `.env.prod`配置文件中修改nonebot2的`HOST`为`0.0.0.0`、设置好超管账号和公网IP
+
+  ```py
+  HOST = "0.0.0.0"  #nonebot2监听的IP
+  SUPERUSERS = [""] # 超级用户
+  COMMAND_START=[""] # 命令前缀,根据需要自行修改
+  DXX_IP = ""
+  ```
+
+## 使用方式
+
+- 启动nb,等待插件加载数据，加载完毕后登录后台，账号默认为`nonebot配置文件中的超管账号`，密码默认为：`admin`,开放端口（默认为.env中配置的port）
+- 在管理后台的推送列表中添加需要开启大学习使用的群聊
+
+## 功能列表
+|    指令    |               指令格式               |                               说明                               |
+| :--------: | :----------------------------------: | :--------------------------------------------------------------: |
+| 添加大学习 |           添加大学习`地区`           |                    添加大学习湖北 添加大学习                     |
+| 我的大学习 |              我的大学习              |                           查询个人信息                           |
+| 提交大学习 |         提交大学习 戳一戳Bot         |                        提交最新一期大学习                        |
+|   大学习   |     大学习答案、大学习、答案截图     |                    获取最新一期青年大学习答案                    |
+|  完成截图  | 完成截图、大学习截图、大学习完成截图 |            获取最新一期青年大学习完成截图（带状态栏）            |
+| 完成大学习 |        完成大学习、全员大学习        | 团支书可用，需要成员填写团支书ID，填写后团支书可发指令提交大学习 |
+|  重置配置  |          重置配置、刷新配置          |                   超管可用，刷新Web UI默认配置                   |
+|  重置密码  |               重置密码               |                   重置登录Web UI的密码为用户ID                   |
+|删除大学习|删除大学习|用户申请清除数据库的信息|
+|导出用户数据|导出用户数据、导出数据|将数据导出至TeenStudy目录下|
+|更新用户数据|更新用户数据、刷新用户数据|将用户数据导入到数据库|
+|更新资源数据|更新资源数据、刷新资源数据|更新数据库中的资源数据（江西共青团团支部数据）|
+
+
+## ToDo
+
+
+- [ ] 增加更多地区支持
+- [ ] 优化 Bot
+
+
+## 更新日志
+
+### 2023/06/12
+
+- 适配北京地区，无需抓包
+- 增加天津地区，需要自行抓包
+- 因江苏和黑龙江地区Cookie时效小于1周，移除江苏和黑龙江地区
+- Web UI添加日志和主动退出功能
+- 更新江西地区拉取团支部数据方式，移除缓存团支部数据，包体积减小50%
+- 修复大学习公网检测失败问题
+- 更新Nonebot2强制meta字段
+- 同步UI依赖AMIS版本到最新版本
+- 开放体验群，不会搭建又想使用的可加[QQ体验群](http://qm.qq.com/cgi-bin/qm/qr?_wv=1027&k=2PQucjirnkHyPjoS1Pkr-ai2aPGToBKm)
+  
+
+<details>
+
+<summary>2023/05/21</summary>
+
+- 增加黑龙江地区，需要自行抓包，该地区上线测试中，请积极提issue反馈
+- 下版本为大版本更新，将添加新功能，优化功能，请积极提issue反馈或加交流群反馈
+- 
+</details>
+
+
+<details>
+<summary>2023/05/11</summary> 
+
+- 增加广东地区，无需抓包[#13](https://github.com/ZM25XC/TeenStudy/issues/13)，感谢[@neal240](https://github.com/neal240)提供账号测试
+
+</details>
+
+<details>
+<summary>2023/05/06</summary> 
+
+- 增加吉林地区，需要自行抓包
+- 修复超管更改登录密码后用原密码能继续登录问题
+- 添加二维码转链接开关，需要自行在后台配置页面打开
+- 调整部分依赖
+
+</details>
+
+<details>
+<summary> 2023/04/12</summary> 
+
+- 因河南地区cookie时效小于1周，移除河南地区
+- 添加`删除大学习`功能，用户可自行删除数据
+- 添加`导出用户数据`功能
+- 添加`更新用户数据`功能
+- 添加`更新资源数据`功能，江西地区更新后请使用下此功能刷新团支部数据
+- 添加戳一戳提交大学习开关，默认开启，请在Web UI后台配置页面进行修改
+- 添加大学习提醒开关，默认开启，支持修改时间，请在Web UI后台配置页面进行修改
+- 添加自动提交大学习开关，默认开启，支持修改时间，请在Web UI后台进行修改
+- 调整安徽地区添加方式[#9](https://github.com/ZM25XC/TeenStudy/issues/9)，无需抓包，感谢[@yhzcake](https://github.com/yhzcake)测试提供方法
+- 修复Web UI 首页公网IP显示异常
+- 修复浙江地区用户重复显示
+- 更新江西共青团团支部数据
+  
+</details>
+
+
+<details>
+<summary>2023/03/18</summary>
+
+- 适配河南地区，需要自行抓包
+- 适配四川地区，需要自行抓包
+- 适配山东地区，需要自行抓包
+- 适配重庆地区，需要自行抓包
+- 添加自动获取公网IP功能，别再问如何配置公网IP啦
+- 添加重置密码功能，指令`重置密码`
+- 添加重置配置功能，指令`重置配置`，`刷新配置`
+- 添加完成大学习功能，团支书可一次性提交全班的大学习，指令`完成大学习`，`全员大学习`
+- 管理后台开放添加用户权限（浙江，上海地区无法添加）
+- 优化用户信息页
+- 优化登录界面提示
+- 将添加链接，登录链接转化成二维码，减少公网IP暴露，没啥用，样式好看一些
+- 修复Ubuntu系统导入资源失败BUG
+  
+</details>
+
+<details>
+
+<summary>2023/03/05</summary>
+
+- 适配浙江地区，使用微信扫码进行绑定
+- 适配上海地区，使用微信扫码进行绑定
+- 适配江苏地区，需要自行抓包
+- 适配安徽地区，需要自行抓包
+
+</details>
+
+<details>
+<summary>2023/03/01</summary>
+
+- 将代码上传至pypi，可使用`pip install TeenStudy`指令安装本插件
+- 上传基础代码
+- 适配湖北地区，无需抓包，安装即用
+- 适配江西地区，无需抓包，安装即用
+
+</details>
 
-setup(**setup_kwargs)
```

#### html2text {}

```diff
@@ -1,123 +1,157 @@
-# -*- coding: utf-8 -*- from setuptools import setup packages = \ ['teenstudy',
-'teenstudy.models', 'teenstudy.utils', 'teenstudy.web', 'teenstudy.web.api',
-'teenstudy.web.pages', 'teenstudy.web.utils'] package_data = \ {'': ['*'],
-'teenstudy': ['resource/*']} install_requires = \ ['Jinja2>=3.1.2,<4.0.0',
-'Pillow>=9.4.0,<10.0.0', 'amis-python>=1.0.7,<2.0.0', 'anti-
-useragent>=1.0.10,<2.0.0', 'beautifulsoup4>=4.11.2,<5.0.0',
-'bs4>=0.0.1,<0.0.2', 'fastapi>=0.95.0,<0.96.0', 'httpx>=0.23.3,<0.24.0',
-'lxml>=4.9.2,<5.0.0', 'nonebot-adapter-onebot>=2.2.1,<3.0.0', 'nonebot-plugin-
-apscheduler>=0.2.0,<0.3.0', 'nonebot2>=2.0.0rc2,<3.0.0',
-'psutil>=5.9.4,<6.0.0', 'python-jose>=3.3.0,<4.0.0', 'qrcode>=7.4.2,<8.0.0',
-'tortoise-orm>=0.19.3,<0.20.0', 'ujson>=5.7.0,<6.0.0',
-'uvicorn>=0.21.0,<0.22.0'] setup_kwargs = { 'name': 'teenstudy', 'version':
-'0.1.9', 'description':
-'åºäºnonebot2å¼æ­¥æ¡æ¶çéå¹´å¤§å­¦èªå¨æäº¤æä»¶åºäºnonebot2çéå¹´å¤§å­¦ä¹ èªå¨æäº¤æä»¶ï¼ç¨äºèªå¨å®æå¤§å­¦ä¹ ï¼å¨åå°çä¸è®°å½ï¼è¿åå®ææªå¾',
-'long_description': '
-                             \n [TeenStudy.png]\n
+Metadata-Version: 2.1 Name: teenstudy Version: 0.2.0rc1 Summary:
+åºäºnonebot2å¼æ­¥æ¡æ¶çéå¹´å¤§å­¦èªå¨æäº¤æä»¶åºäºnonebot2çéå¹´å¤§å­¦ä¹ èªå¨æäº¤æä»¶ï¼ç¨äºèªå¨å®æå¤§å­¦ä¹ ï¼å¨åå°çä¸è®°å½ï¼è¿åå®ææªå¾
+Home-page: https://github.com/ZM25XC/TeenStudy License: MIT Author: ZM25XC
+Author-email: xingling25@qq.com Requires-Python: >=3.8,<4.0 Classifier: License
+:: OSI Approved :: MIT License Classifier: Programming Language :: Python :: 3
+Classifier: Programming Language :: Python :: 3.8 Classifier: Programming
+Language :: Python :: 3.9 Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11 Requires-Dist: Jinja2
+(>=3.1.2,<4.0.0) Requires-Dist: amis-python (>=1.0.8,<2.0.0) Requires-Dist:
+anti-useragent (>=1.0.10,<2.0.0) Requires-Dist: beautifulsoup4
+(>=4.11.2,<5.0.0) Requires-Dist: bs4 (>=0.0.1,<0.0.2) Requires-Dist: ddddocr
+(>=1.4.7,<2.0.0) Requires-Dist: fastapi (>=0.95.0,<0.96.0) Requires-Dist: httpx
+(>=0.24.0,<0.25.0) Requires-Dist: lxml (>=4.9.2,<5.0.0) Requires-Dist: nonebot-
+adapter-onebot (>=2.2.3,<3.0.0) Requires-Dist: nonebot-plugin-apscheduler
+(>=0.3.0,<0.4.0) Requires-Dist: nonebot2 (>=2.0.0,<3.0.0) Requires-Dist: psutil
+(>=5.9.4,<6.0.0) Requires-Dist: pycryptodome (>=3.17,<4.0) Requires-Dist:
+python-jose (>=3.3.0,<4.0.0) Requires-Dist: qrcode (>=7.4.2,<8.0.0) Requires-
+Dist: tortoise-orm (>=0.19.3,<0.20.0) Requires-Dist: ujson (>=5.7.0,<6.0.0)
+Requires-Dist: uvicorn (>=0.21.0,<0.22.0) Description-Content-Type: text/
+markdown
+                                [TeenStudy.png]
                             ****** TeenStudy ******
-                            \n åºäºnonebot2ågo-
-cqhttpçéå¹´å¤§å­¦ä¹ èªå¨æäº¤æä»¶ï¼ç¨äºèªå¨å®æå¤§å­¦ä¹ ï¼å¨åå°çä¸è®°å½ï¼è¿åå®ææªå¾\n
+                             åºäºnonebot2ågo-
+cqhttpçéå¹´å¤§å­¦ä¹ èªå¨æäº¤æä»¶ï¼ç¨äºèªå¨å®æå¤§å­¦ä¹ ï¼å¨åå°çä¸è®°å½ï¼è¿åå®ææªå¾
 
-  \n [GitHub_issues]\n [GitHub_forks]\n [GitHub_stars]\n [pypi]\n \t\n_[pypi
-            download]\n\t [GitHub_license]\n \n_[QQ_Chat_Group]\n\n
-\n\n## è¯´æ\n\n- æ¬é¡¹ç®ä¸º[éå¹´å¤§å­¦ä¹ æäº¤](https://github.com/
-ZM25XC/nonebot_plugin_auto_teenstudy) `Web UI`ç\n- æ¬é¡¹ç®åºäº[nonebot2]
-(https://github.com/nonebot/nonebot2)å[go-cqhttp](https://github.com/Mrs4s/
-go-cqhttp)ï¼ä½¿ç¨æ¬æä»¶åè¯·åéè¯»ä»¥ä¸ä¸¤ä¸ªé¡¹ç®çä½¿ç¨ææ¡£\n-
-**å¯å¨æä»¶ä¹åï¼ä¸å®è¦ç»å½åå°å¨æ¨éåè¡¨ä¸­æ·»å éè¦å¼å¯å¤§å­¦ä¹ åè½çç¾¤è**\n-
-**æ¬é¡¹ç®æ æ³å¨å½å¤IPç¯å¢ä¸ä½¿ç¨ï¼å¦æå¼å¯ä»£çï¼è¯·å³é­ææ·»å ä»£çè§å**\n-
-éè¦æåçå°åºï¼ç»å®åå°½éå«è¿å®æ¹å¬ä¼å·ï¼é¿åtokenæcookieå·æ°å¯¼è´æ æ³æäº¤\n-
-æ¬é¡¹ç®éè¦é¨ç½²å¨å¬ç½å¯è®¿é®çå®¹å¨ä¸­ï¼å¹¶å¼æ¾ç«¯å£ï¼nonebot2éç½®çportï¼ï¼å¦åå¤§é¨ååè½å°åºç°å¼å¸¸\n-
-æ¬¢è¿å å¥[QQç¾¤](https://jq.qq.com/
-?_wv=1027&k=NGFEwXyS)ï¼äº¤æµè®¨è®ºã\n-
-æ¶é´ç²¾åæéï¼ç®ååªç»´æ¤æ¹ååæ±è¥¿ä¸¤ä¸ªå°åºï¼å¶ä»å°åºåºé®é¢è¯·æäº¤Issues,ææ¾ä¸ªæ¶é´ä¿®ï¼éè¦å¢å å°åºè¯·è¿ç¾¤å¸®å¿æµè¯ï¼ä¸ªå«å°åºæ²¡è´¦å·æ æ³æµè¯\n\n-
-è§å¾é¡¹ç®ä¸éï¼ä¸å¦¨ç¹ä¸ªstars.\n\n## å°åºç¶æ\n\n\n\n|
-å±éå¢åç§° | å¼åç¶æ | å¤æ³¨ |\n|:-----:|:----:|:----:
-|\n|éæ¥æ¹å|æ¯æ|æ éæå|\n|æ±è¥¿å±éå¢|æ¯æ|æ éæå|\n|å®å¾½å±éå¢|æ¯æ|æ éæå|\n|å¹¿ä¸å±éå¢|æ¯æ|æ éæå|\n|éæ¥ä¸æµ·|æ¯æ|å¾®ä¿¡æ«ç ç»å®|\n|éæ¥æµæ±|æ¯æ|å¾®ä¿¡æ«ç ç»å®|\n|æ±èå±éå¢|æ¯æ|éè¦èªè¡æå|\n|éæ¥å±±ä¸|æ¯æ|éè¦èªè¡æå|\n|éåºå±éå¢|æ¯æ|éè¦èªè¡æå|\n|åéé£æ¬|æ¯æ|éè¦èªè¡æå|\n|é»é¾æ±å±éå¢|æ¯æ|éè¦èªè¡æåï¼è¯¥å°åºä¸çº¿æµè¯ä¸­|\n|å¤©åºæ°éå¹´|æ¯æ|ä¸è¿å¥å¬ä¼å·tokenæ¶æå¤§äº1å¨|\n|æ²³åå±éå¢|ä¸æ¯æ|cookieæ¶æå°äº1å¨|\n|å¹¿è¥¿éå¹´å|å¾å¼å||\n|éæ¥æ¹å|å¾å¼å||\n|çèéå¹´|å¾å¼å||\n|å±±è¥¿éå¹´|å¾å¼å||\n|æ²³åå±éå¢|å¾å¼å||\n|ç¦å»ºå±éå¢|å¾å¼å||\n|åèå¤éå¹´|å¾å¼å||\n|äºåå±éå¢|å¾å¼å||\n|ä¸ç§¦éå¹´|å¾å¼å||\n|éæ¥åäº¬|å¾å¼å||\n|æµ·åå±éå¢|å¾å¼å||\n|æ´¥å½©éæ¥|å¾å¼å||\n|éæ¥é»è¨|å¾å¼å||\n|éæ¥æ³å·|å¾å¼å||\n|è¾½å®å±éå¢|å¾å¼å||\n|å®å¤å±éå¢|å¾å¼å||\n|æ°çå±éå¢|å¾å¼å||\n|è¥¿èå±éå¢|å¾å¼å||\n\n\n\n##
-å®è£åæ´æ°\n\n\nç¬¬ä¸ç§æ¹å¼(ä¸æ¨è)\n\n- ä½¿ç¨`git clone https://
-github.com/ZM25XC/
-TeenStudy.git`æä»¤åéæ¬ä»åºæä¸è½½åç¼©åæä»¶\n\n\n\n\nç¬¬äºç§æ¹å¼
-(äºéä¸)\n\n- ä½¿ç¨`pip install TeenStudy`æ¥è¿è¡å®è£,ä½¿ç¨`pip
-install TeenStudy -U`è¿è¡æ´æ°\n- ä½¿ç¨`nb plugin install
-TeenStudy`æ¥è¿è¡å®è£,ä½¿ç¨`nb plugin install TeenStudy -
-U`è¿è¡æ´æ°\n\n\n\n\n##
-å¯¼å¥æä»¶\n\n\nä½¿ç¨ç¬¬ä¸ç§æ¹å¼å®è£çæ­¤æ¹æ³\n\n-
-å°`TeenStudy`æ¾å¨nbç`plugins`ç®å½ä¸ï¼è¿è¡nbæºå¨äººå³å¯\n\n-
-æä»¶ç»æå¦ä¸\n\n ```py\n ð¦ AweSome-Bot\n âââ ð awesome_bot\n
-â âââ ð plugins\n | âââ ð TeenStudy\n | âââ ð
-__init__.py\n âââ ð .env.prod\n âââ ð .gitignore\n âââ
-ð pyproject.toml\n âââ ð README.md\n ```\n\n
-\n\n\n\n\nä½¿ç¨ç¬¬äºç§æ¹å¼å®è£çæ­¤æ¹æ³\n\n-
-å¨`pyproject.toml`éç`[tool.nonebot]`ä¸­æ·»å `plugins =
-["TeenStudy"]`\n\n\n\n## æºå¨äººéç½®\n\n- å¨nonebotç`.env` æ
-`.env.prod`éç½®æä»¶ä¸­ä¿®æ¹nonebot2ç`HOST`ä¸º`0.0.0.0`ãè®¾ç½®å¥½è¶ç®¡è´¦å·åå¬ç½IP\n\n
-```py\n HOST = "0.0.0.0" #nonebot2çå¬çIP\n SUPERUSERS = [""] #
-è¶çº§ç¨æ·\n COMMAND_START=[""] # å½ä»¤åç¼,æ ¹æ®éè¦èªè¡ä¿®æ¹\n
-DXX_IP = ""\n ```\n\n## ä½¿ç¨æ¹å¼\n\n-
-å¯å¨nb,ç­å¾æä»¶å è½½æ°æ®ï¼å è½½å®æ¯åç»å½åå°ï¼è´¦å·é»è®¤ä¸º`nonebotéç½®æä»¶ä¸­çè¶ç®¡è´¦å·`ï¼å¯ç é»è®¤ä¸ºï¼`admin`,å¼æ¾ç«¯å£ï¼é»è®¤ä¸º.envä¸­éç½®çportï¼\n-
-å¨ç®¡çåå°çæ¨éåè¡¨ä¸­æ·»å éè¦å¼å¯å¤§å­¦ä¹ ä½¿ç¨çç¾¤è\n\n##
-åè½åè¡¨\n| æä»¤ | æä»¤æ ¼å¼ | è¯´æ |\n| :--------: | :-------------
----------------------: | :-----------------------------------------------------
----------: |\n| æ·»å å¤§å­¦ä¹  | æ·»å å¤§å­¦ä¹ `å°åº` |
-æ·»å å¤§å­¦ä¹ æ¹å æ·»å å¤§å­¦ä¹  |\n| æçå¤§å­¦ä¹  | æçå¤§å­¦ä¹  |
-æ¥è¯¢ä¸ªäººä¿¡æ¯ |\n| æäº¤å¤§å­¦ä¹  | æäº¤å¤§å­¦ä¹  æ³ä¸æ³Bot |
-æäº¤ææ°ä¸æå¤§å­¦ä¹  |\n| å¤§å­¦ä¹  |
+ [GitHub_issues] [GitHub_forks] [GitHub_stars] [pypi] [pypi_download] [GitHub
+                   license] [QQ_Chat_Group] [QQ_Chat_Group]
+## è¯´æ - æ¬é¡¹ç®ä¸º[éå¹´å¤§å­¦ä¹ æäº¤](https://github.com/ZM25XC/
+nonebot_plugin_auto_teenstudy) `Web UI`ç - æ¬é¡¹ç®åºäº[nonebot2](https://
+github.com/nonebot/nonebot2)å[go-cqhttp](https://github.com/Mrs4s/go-
+cqhttp)ï¼ä½¿ç¨æ¬æä»¶åè¯·åéè¯»ä»¥ä¸ä¸¤ä¸ªé¡¹ç®çä½¿ç¨ææ¡£ -
+**å¯å¨æä»¶ä¹åï¼ä¸å®è¦ç»å½åå°å¨æ¨éåè¡¨ä¸­æ·»å éè¦å¼å¯å¤§å­¦ä¹ åè½çç¾¤è**
+-
+**æ¬é¡¹ç®æ æ³å¨å½å¤IPç¯å¢ä¸ä½¿ç¨ï¼å¦æå¼å¯ä»£çï¼è¯·å³é­ææ·»å ä»£çè§å**
+-
+éè¦æåçå°åºï¼ç»å®åå°½éå«è¿å®æ¹å¬ä¼å·ï¼é¿åtokenæcookieå·æ°å¯¼è´æ æ³æäº¤
+-
+æ¬é¡¹ç®éè¦é¨ç½²å¨å¬ç½å¯è®¿é®çå®¹å¨ä¸­ï¼å¹¶å¼æ¾ç«¯å£ï¼nonebot2éç½®çportï¼ï¼å¦åå¤§é¨ååè½å°åºç°å¼å¸¸
+- æ¬¢è¿å å¥[QQåé¦ç¾¤](https://jq.qq.com/
+?_wv=1027&k=NGFEwXyS)ï¼äº¤æµè®¨è®ºï¼å¦æ¨ä¸ä¼æ­å»ºåæ³æ¯å¨èªå¨æäº¤ï¼å¯å å¥
+[QQä½éªç¾¤](http://qm.qq.com/cgi-bin/qm/qr?_wv=1027&k=2PQucjirnkHyPjoS1Pkr-
+ai2aPGToBKm)ã -
+æ¶é´ç²¾åæéï¼ç®ååªç»´æ¤æ¹ååæ±è¥¿ä¸¤ä¸ªå°åºï¼å¶ä»å°åºåºé®é¢è¯·æäº¤Issues,ææ¾ä¸ªæ¶é´ä¿®ï¼éè¦å¢å å°åºè¯·è¿ç¾¤å¸®å¿æµè¯ï¼ä¸ªå«å°åºæ²¡è´¦å·æ æ³æµè¯
+- è§å¾é¡¹ç®ä¸éï¼ä¸å¦¨ç¹ä¸ªstars. ## å°åºç¶æ  | å±éå¢åç§° |
+å¼åç¶æ | å¤æ³¨ | |:-----:|:----:|:----:
+| |éæ¥æ¹å|æ¯æ|æ éæå| |æ±è¥¿å±éå¢|æ¯æ|æ éæå|
+|å®å¾½å±éå¢|æ¯æ|æ éæå| |å¹¿ä¸å±éå¢|æ¯æ|æ éæå|
+|éæ¥åäº¬|æ¯æ|æ éæå| |éæ¥ä¸æµ·|æ¯æ|å¾®ä¿¡æ«ç ç»å®|
+|éæ¥æµæ±|æ¯æ|å¾®ä¿¡æ«ç ç»å®|
+|æ´¥å½©éæ¥|æ¯æ|éè¦èªè¡æå|
+|éæ¥å±±ä¸|æ¯æ|éè¦èªè¡æå|
+|éåºå±éå¢|æ¯æ|éè¦èªè¡æå|
+|åéé£æ¬|æ¯æ|éè¦èªè¡æå|
+|å¤©åºæ°éå¹´|æ¯æ|ä¸è¿å¥å¬ä¼å·tokenæ¶æå¤§äº1å¨|
+|æ²³åå±éå¢|ä¸æ¯æ|cookieæ¶æå°äº1å¨|
+|æ±èå±éå¢|ä¸æ¯æ|cookieå¤±æå°äº1å¨|
+|é»é¾æ±å±éå¢|ä¸æ¯æ|cookieå¤±æå°äº1å¨|
+|å¹¿è¥¿éå¹´å|å¾å¼å|| |éæ¥æ¹å|å¾å¼å||
+|çèéå¹´|å¾å¼å|| |å±±è¥¿éå¹´|å¾å¼å||
+|æ²³åå±éå¢|å¾å¼å|| |ç¦å»ºå±éå¢|å¾å¼å||
+|åèå¤éå¹´|å¾å¼å|| |äºåå±éå¢|å¾å¼å||
+|ä¸ç§¦éå¹´|å¾å¼å|| |æµ·åå±éå¢|å¾å¼å||
+|éæ¥é»è¨|å¾å¼å|| |éæ¥æ³å·|å¾å¼å||
+|è¾½å®å±éå¢|å¾å¼å|| |å®å¤å±éå¢|å¾å¼å||
+|æ°çå±éå¢|å¾å¼å|| |è¥¿èå±éå¢|å¾å¼å||  ## å®è£åæ´æ°
+ç¬¬ä¸ç§æ¹å¼(ä¸æ¨è) - ä½¿ç¨`git clone https://github.com/ZM25XC/
+TeenStudy.git`æä»¤åéæ¬ä»åºæä¸è½½åç¼©åæä»¶   ç¬¬äºç§æ¹å¼
+(äºéä¸) - ä½¿ç¨`pip install TeenStudy`æ¥è¿è¡å®è£,ä½¿ç¨`pip install
+TeenStudy -U`è¿è¡æ´æ° - ä½¿ç¨`nb plugin install
+TeenStudy`æ¥è¿è¡å®è£,ä½¿ç¨`nb plugin install TeenStudy -U`è¿è¡æ´æ°
+## å¯¼å¥æä»¶  ä½¿ç¨ç¬¬ä¸ç§æ¹å¼å®è£çæ­¤æ¹æ³ -
+å°`TeenStudy`æ¾å¨nbç`plugins`ç®å½ä¸ï¼è¿è¡nbæºå¨äººå³å¯ -
+æä»¶ç»æå¦ä¸ ```py ð¦ AweSome-Bot âââ ð awesome_bot â
+âââ ð plugins | âââ ð TeenStudy | âââ ð __init__.py
+âââ ð .env.prod âââ ð .gitignore âââ ð
+pyproject.toml âââ ð README.md ```
+ä½¿ç¨ç¬¬äºç§æ¹å¼å®è£çæ­¤æ¹æ³ - å¨`pyproject.toml`éç`
+[tool.nonebot]`ä¸­æ·»å `plugins = ["TeenStudy"]`  ## æºå¨äººéç½® -
+å¨nonebotç`.env` æ
+`.env.prod`éç½®æä»¶ä¸­ä¿®æ¹nonebot2ç`HOST`ä¸º`0.0.0.0`ãè®¾ç½®å¥½è¶ç®¡è´¦å·åå¬ç½IP
+```py HOST = "0.0.0.0" #nonebot2çå¬çIP SUPERUSERS = [""] # è¶çº§ç¨æ·
+COMMAND_START=[""] # å½ä»¤åç¼,æ ¹æ®éè¦èªè¡ä¿®æ¹ DXX_IP = "" ``` ##
+ä½¿ç¨æ¹å¼ -
+å¯å¨nb,ç­å¾æä»¶å è½½æ°æ®ï¼å è½½å®æ¯åç»å½åå°ï¼è´¦å·é»è®¤ä¸º`nonebotéç½®æä»¶ä¸­çè¶ç®¡è´¦å·`ï¼å¯ç é»è®¤ä¸ºï¼`admin`,å¼æ¾ç«¯å£ï¼é»è®¤ä¸º.envä¸­éç½®çportï¼
+- å¨ç®¡çåå°çæ¨éåè¡¨ä¸­æ·»å éè¦å¼å¯å¤§å­¦ä¹ ä½¿ç¨çç¾¤è
+## åè½åè¡¨ | æä»¤ | æä»¤æ ¼å¼ | è¯´æ | | :--------: | :------------
+----------------------: | :----------------------------------------------------
+----------: | | æ·»å å¤§å­¦ä¹  | æ·»å å¤§å­¦ä¹ `å°åº` |
+æ·»å å¤§å­¦ä¹ æ¹å æ·»å å¤§å­¦ä¹  | | æçå¤§å­¦ä¹  | æçå¤§å­¦ä¹  |
+æ¥è¯¢ä¸ªäººä¿¡æ¯ | | æäº¤å¤§å­¦ä¹  | æäº¤å¤§å­¦ä¹  æ³ä¸æ³Bot |
+æäº¤ææ°ä¸æå¤§å­¦ä¹  | | å¤§å­¦ä¹  |
 å¤§å­¦ä¹ ç­æ¡ãå¤§å­¦ä¹ ãç­æ¡æªå¾ |
-è·åææ°ä¸æéå¹´å¤§å­¦ä¹ ç­æ¡ |\n| å®ææªå¾ |
+è·åææ°ä¸æéå¹´å¤§å­¦ä¹ ç­æ¡ | | å®ææªå¾ |
 å®ææªå¾ãå¤§å­¦ä¹ æªå¾ãå¤§å­¦ä¹ å®ææªå¾ |
-è·åææ°ä¸æéå¹´å¤§å­¦ä¹ å®ææªå¾ï¼å¸¦ç¶ææ ï¼ |\n|
+è·åææ°ä¸æéå¹´å¤§å­¦ä¹ å®ææªå¾ï¼å¸¦ç¶ææ ï¼ | |
 å®æå¤§å­¦ä¹  | å®æå¤§å­¦ä¹ ãå¨åå¤§å­¦ä¹  |
 å¢æ¯ä¹¦å¯ç¨ï¼éè¦æåå¡«åå¢æ¯ä¹¦IDï¼å¡«ååå¢æ¯ä¹¦å¯åæä»¤æäº¤å¤§å­¦ä¹ 
-|\n| éç½®éç½® | éç½®éç½®ãå·æ°éç½® | è¶ç®¡å¯ç¨ï¼å·æ°Web
-UIé»è®¤éç½® |\n| éç½®å¯ç  | éç½®å¯ç  | éç½®ç»å½Web
-UIçå¯ç ä¸ºç¨æ·ID
-|\n|å é¤å¤§å­¦ä¹ |å é¤å¤§å­¦ä¹ |ç¨æ·ç³è¯·æ¸é¤æ°æ®åºçä¿¡æ¯|\n|å¯¼åºç¨æ·æ°æ®|å¯¼åºç¨æ·æ°æ®ãå¯¼åºæ°æ®|å°æ°æ®å¯¼åºè³TeenStudyç®å½ä¸|\n|æ´æ°ç¨æ·æ°æ®|æ´æ°ç¨æ·æ°æ®ãå·æ°ç¨æ·æ°æ®|å°ç¨æ·æ°æ®å¯¼å¥å°æ°æ®åº|\n|æ´æ°èµæºæ°æ®|æ´æ°èµæºæ°æ®ãå·æ°èµæºæ°æ®|æ´æ°æ°æ®åºä¸­çèµæºæ°æ®ï¼æ±è¥¿å±éå¢å¢æ¯é¨æ°æ®ï¼|\n\n\n##
-ToDo\n\n\n- [ ] å¢å æ´å¤å°åºæ¯æ\n- [ ] ä¼å Bot\n\n\n##
-æ´æ°æ¥å¿\n\n### 2023/05/21\n\n-
-å¢å é»é¾æ±å°åºï¼éè¦èªè¡æåï¼è¯¥å°åºä¸çº¿æµè¯ä¸­ï¼è¯·ç§¯ææissueåé¦\n-
-ä¸çæ¬ä¸ºå¤§çæ¬æ´æ°ï¼å°æ·»å æ°åè½ï¼ä¼ååè½ï¼è¯·ç§¯ææissueåé¦æå äº¤æµç¾¤åé¦\n\n\n2023/
-05/11 \n\n- å¢å å¹¿ä¸å°åºï¼æ éæå[#13](https://github.com/ZM25XC/
-TeenStudy/issues/13)ï¼æè°¢[@neal240](https://github.com/
-neal240)æä¾è´¦å·æµè¯\n\n\n\n\n2023/05/06 \n\n-
-å¢å åæå°åºï¼éè¦èªè¡æå\n-
-ä¿®å¤è¶ç®¡æ´æ¹ç»å½å¯ç åç¨åå¯ç è½ç»§ç»­ç»å½é®é¢\n-
-æ·»å äºç»´ç è½¬é¾æ¥å¼å³ï¼éè¦èªè¡å¨åå°éç½®é¡µé¢æå¼\n-
-è°æ´é¨åä¾èµ\n\n\n\n\n 2023/04/12 \n\n-
-å æ²³åå°åºcookieæ¶æå°äº1å¨ï¼ç§»é¤æ²³åå°åº\n-
-æ·»å `å é¤å¤§å­¦ä¹ `åè½ï¼ç¨æ·å¯èªè¡å é¤æ°æ®\n-
-æ·»å `å¯¼åºç¨æ·æ°æ®`åè½\n- æ·»å `æ´æ°ç¨æ·æ°æ®`åè½\n-
-æ·»å `æ´æ°èµæºæ°æ®`åè½ï¼æ±è¥¿å°åºæ´æ°åè¯·ä½¿ç¨ä¸æ­¤åè½å·æ°å¢æ¯é¨æ°æ®\n-
-æ·»å æ³ä¸æ³æäº¤å¤§å­¦ä¹ å¼å³ï¼é»è®¤å¼å¯ï¼è¯·å¨Web
-UIåå°éç½®é¡µé¢è¿è¡ä¿®æ¹\n-
+| | éç½®éç½® | éç½®éç½®ãå·æ°éç½® | è¶ç®¡å¯ç¨ï¼å·æ°Web
+UIé»è®¤éç½® | | éç½®å¯ç  | éç½®å¯ç  | éç½®ç»å½Web
+UIçå¯ç ä¸ºç¨æ·ID |
+|å é¤å¤§å­¦ä¹ |å é¤å¤§å­¦ä¹ |ç¨æ·ç³è¯·æ¸é¤æ°æ®åºçä¿¡æ¯|
+|å¯¼åºç¨æ·æ°æ®|å¯¼åºç¨æ·æ°æ®ãå¯¼åºæ°æ®|å°æ°æ®å¯¼åºè³TeenStudyç®å½ä¸|
+|æ´æ°ç¨æ·æ°æ®|æ´æ°ç¨æ·æ°æ®ãå·æ°ç¨æ·æ°æ®|å°ç¨æ·æ°æ®å¯¼å¥å°æ°æ®åº|
+|æ´æ°èµæºæ°æ®|æ´æ°èµæºæ°æ®ãå·æ°èµæºæ°æ®|æ´æ°æ°æ®åºä¸­çèµæºæ°æ®ï¼æ±è¥¿å±éå¢å¢æ¯é¨æ°æ®ï¼|
+## ToDo - [ ] å¢å æ´å¤å°åºæ¯æ - [ ] ä¼å Bot ## æ´æ°æ¥å¿ ###
+2023/06/12 - ééåäº¬å°åºï¼æ éæå -
+å¢å å¤©æ´¥å°åºï¼éè¦èªè¡æå -
+å æ±èåé»é¾æ±å°åºCookieæ¶æå°äº1å¨ï¼ç§»é¤æ±èåé»é¾æ±å°åº
+- Web UIæ·»å æ¥å¿åä¸»å¨éåºåè½ -
+æ´æ°æ±è¥¿å°åºæåå¢æ¯é¨æ°æ®æ¹å¼ï¼ç§»é¤ç¼å­å¢æ¯é¨æ°æ®ï¼åä½ç§¯åå°50%
+- ä¿®å¤å¤§å­¦ä¹ å¬ç½æ£æµå¤±è´¥é®é¢ - æ´æ°Nonebot2å¼ºå¶metaå­æ®µ -
+åæ­¥UIä¾èµAMISçæ¬å°ææ°çæ¬ -
+å¼æ¾ä½éªç¾¤ï¼ä¸ä¼æ­å»ºåæ³ä½¿ç¨çå¯å [QQä½éªç¾¤](http://
+qm.qq.com/cgi-bin/qm/qr?_wv=1027&k=2PQucjirnkHyPjoS1Pkr-ai2aPGToBKm)  2023/05/
+21 -
+å¢å é»é¾æ±å°åºï¼éè¦èªè¡æåï¼è¯¥å°åºä¸çº¿æµè¯ä¸­ï¼è¯·ç§¯ææissueåé¦
+-
+ä¸çæ¬ä¸ºå¤§çæ¬æ´æ°ï¼å°æ·»å æ°åè½ï¼ä¼ååè½ï¼è¯·ç§¯ææissueåé¦æå äº¤æµç¾¤åé¦
+-   2023/05/11 - å¢å å¹¿ä¸å°åºï¼æ éæå[#13](https://github.com/
+ZM25XC/TeenStudy/issues/13)ï¼æè°¢[@neal240](https://github.com/
+neal240)æä¾è´¦å·æµè¯   2023/05/06 -
+å¢å åæå°åºï¼éè¦èªè¡æå -
+ä¿®å¤è¶ç®¡æ´æ¹ç»å½å¯ç åç¨åå¯ç è½ç»§ç»­ç»å½é®é¢ -
+æ·»å äºç»´ç è½¬é¾æ¥å¼å³ï¼éè¦èªè¡å¨åå°éç½®é¡µé¢æå¼ -
+è°æ´é¨åä¾èµ    2023/04/12 -
+å æ²³åå°åºcookieæ¶æå°äº1å¨ï¼ç§»é¤æ²³åå°åº -
+æ·»å `å é¤å¤§å­¦ä¹ `åè½ï¼ç¨æ·å¯èªè¡å é¤æ°æ® -
+æ·»å `å¯¼åºç¨æ·æ°æ®`åè½ - æ·»å `æ´æ°ç¨æ·æ°æ®`åè½ -
+æ·»å `æ´æ°èµæºæ°æ®`åè½ï¼æ±è¥¿å°åºæ´æ°åè¯·ä½¿ç¨ä¸æ­¤åè½å·æ°å¢æ¯é¨æ°æ®
+- æ·»å æ³ä¸æ³æäº¤å¤§å­¦ä¹ å¼å³ï¼é»è®¤å¼å¯ï¼è¯·å¨Web
+UIåå°éç½®é¡µé¢è¿è¡ä¿®æ¹ -
 æ·»å å¤§å­¦ä¹ æéå¼å³ï¼é»è®¤å¼å¯ï¼æ¯æä¿®æ¹æ¶é´ï¼è¯·å¨Web
-UIåå°éç½®é¡µé¢è¿è¡ä¿®æ¹\n-
+UIåå°éç½®é¡µé¢è¿è¡ä¿®æ¹ -
 æ·»å èªå¨æäº¤å¤§å­¦ä¹ å¼å³ï¼é»è®¤å¼å¯ï¼æ¯æä¿®æ¹æ¶é´ï¼è¯·å¨Web
-UIåå°è¿è¡ä¿®æ¹\n- è°æ´å®å¾½å°åºæ·»å æ¹å¼[#9](https://github.com/
+UIåå°è¿è¡ä¿®æ¹ - è°æ´å®å¾½å°åºæ·»å æ¹å¼[#9](https://github.com/
 ZM25XC/TeenStudy/issues/9)ï¼æ éæåï¼æè°¢[@yhzcake](https://
-github.com/yhzcake)æµè¯æä¾æ¹æ³\n- ä¿®å¤Web UI
-é¦é¡µå¬ç½IPæ¾ç¤ºå¼å¸¸\n- ä¿®å¤æµæ±å°åºç¨æ·éå¤æ¾ç¤º\n-
-æ´æ°æ±è¥¿å±éå¢å¢æ¯é¨æ°æ®\n \n\n\n\n\n2023/03/18\n\n-
-ééæ²³åå°åºï¼éè¦èªè¡æå\n-
-ééåå·å°åºï¼éè¦èªè¡æå\n-
-ééå±±ä¸å°åºï¼éè¦èªè¡æå\n-
-éééåºå°åºï¼éè¦èªè¡æå\n-
-æ·»å èªå¨è·åå¬ç½IPåè½ï¼å«åé®å¦ä½éç½®å¬ç½IPå¦\n-
-æ·»å éç½®å¯ç åè½ï¼æä»¤`éç½®å¯ç `\n-
-æ·»å éç½®éç½®åè½ï¼æä»¤`éç½®éç½®`ï¼`å·æ°éç½®`\n-
-æ·»å å®æå¤§å­¦ä¹ åè½ï¼å¢æ¯ä¹¦å¯ä¸æ¬¡æ§æäº¤å¨ç­çå¤§å­¦ä¹ ï¼æä»¤`å®æå¤§å­¦ä¹ `ï¼`å¨åå¤§å­¦ä¹ `\n-
-ç®¡çåå°å¼æ¾æ·»å ç¨æ·æéï¼æµæ±ï¼ä¸æµ·å°åºæ æ³æ·»å ï¼\n-
-ä¼åç¨æ·ä¿¡æ¯é¡µ\n- ä¼åç»å½çé¢æç¤º\n-
-å°æ·»å é¾æ¥ï¼ç»å½é¾æ¥è½¬åæäºç»´ç ï¼åå°å¬ç½IPæ´é²ï¼æ²¡å¥ç¨ï¼æ ·å¼å¥½çä¸äº\n-
-ä¿®å¤Ubuntuç³»ç»å¯¼å¥èµæºå¤±è´¥BUG\n \n\n\n\n\n2023/03/05\n\n-
-ééæµæ±å°åºï¼ä½¿ç¨å¾®ä¿¡æ«ç è¿è¡ç»å®\n-
-ééä¸æµ·å°åºï¼ä½¿ç¨å¾®ä¿¡æ«ç è¿è¡ç»å®\n-
-ééæ±èå°åºï¼éè¦èªè¡æå\n-
-ééå®å¾½å°åºï¼éè¦èªè¡æå\n\n\n\n\n2023/03/01\n\n-
-å°ä»£ç ä¸ä¼ è³pypiï¼å¯ä½¿ç¨`pip install
-TeenStudy`æä»¤å®è£æ¬æä»¶\n- ä¸ä¼ åºç¡ä»£ç \n-
-ééæ¹åå°åºï¼æ éæåï¼å®è£å³ç¨\n-
-ééæ±è¥¿å°åºï¼æ éæåï¼å®è£å³ç¨\n\n\n', 'author': 'ZM25XC',
-'author_email': 'xingling25@qq.com', 'maintainer': 'None', 'maintainer_email':
-'None', 'url': 'https://github.com/ZM25XC/TeenStudy', 'packages': packages,
-'package_data': package_data, 'install_requires': install_requires,
-'python_requires': '>=3.8,<4.0', } setup(**setup_kwargs)
+github.com/yhzcake)æµè¯æä¾æ¹æ³ - ä¿®å¤Web UI é¦é¡µå¬ç½IPæ¾ç¤ºå¼å¸¸
+- ä¿®å¤æµæ±å°åºç¨æ·éå¤æ¾ç¤º - æ´æ°æ±è¥¿å±éå¢å¢æ¯é¨æ°æ®
+2023/03/18 - ééæ²³åå°åºï¼éè¦èªè¡æå -
+ééåå·å°åºï¼éè¦èªè¡æå -
+ééå±±ä¸å°åºï¼éè¦èªè¡æå -
+éééåºå°åºï¼éè¦èªè¡æå -
+æ·»å èªå¨è·åå¬ç½IPåè½ï¼å«åé®å¦ä½éç½®å¬ç½IPå¦ -
+æ·»å éç½®å¯ç åè½ï¼æä»¤`éç½®å¯ç ` -
+æ·»å éç½®éç½®åè½ï¼æä»¤`éç½®éç½®`ï¼`å·æ°éç½®` -
+æ·»å å®æå¤§å­¦ä¹ åè½ï¼å¢æ¯ä¹¦å¯ä¸æ¬¡æ§æäº¤å¨ç­çå¤§å­¦ä¹ ï¼æä»¤`å®æå¤§å­¦ä¹ `ï¼`å¨åå¤§å­¦ä¹ `
+- ç®¡çåå°å¼æ¾æ·»å ç¨æ·æéï¼æµæ±ï¼ä¸æµ·å°åºæ æ³æ·»å ï¼ -
+ä¼åç¨æ·ä¿¡æ¯é¡µ - ä¼åç»å½çé¢æç¤º -
+å°æ·»å é¾æ¥ï¼ç»å½é¾æ¥è½¬åæäºç»´ç ï¼åå°å¬ç½IPæ´é²ï¼æ²¡å¥ç¨ï¼æ ·å¼å¥½çä¸äº
+- ä¿®å¤Ubuntuç³»ç»å¯¼å¥èµæºå¤±è´¥BUG   2023/03/05 -
+ééæµæ±å°åºï¼ä½¿ç¨å¾®ä¿¡æ«ç è¿è¡ç»å® -
+ééä¸æµ·å°åºï¼ä½¿ç¨å¾®ä¿¡æ«ç è¿è¡ç»å® -
+ééæ±èå°åºï¼éè¦èªè¡æå -
+ééå®å¾½å°åºï¼éè¦èªè¡æå   2023/03/01 -
+å°ä»£ç ä¸ä¼ è³pypiï¼å¯ä½¿ç¨`pip install TeenStudy`æä»¤å®è£æ¬æä»¶
+- ä¸ä¼ åºç¡ä»£ç  - ééæ¹åå°åºï¼æ éæåï¼å®è£å³ç¨ -
+ééæ±è¥¿å°åºï¼æ éæåï¼å®è£å³ç¨
```

