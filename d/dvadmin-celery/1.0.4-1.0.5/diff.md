# Comparing `tmp/dvadmin-celery-1.0.4.tar.gz` & `tmp/dvadmin-celery-1.0.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dvadmin-celery-1.0.4.tar", last modified: Thu Mar  2 04:02:57 2023, max compression
+gzip compressed data, was "dvadmin-celery-1.0.5.tar", last modified: Mon Jun 12 03:28:27 2023, max compression
```

## Comparing `dvadmin-celery-1.0.4.tar` & `dvadmin-celery-1.0.5.tar`

### file list

```diff
@@ -1,31 +1,32 @@
-drwxrwxrwx   0        0        0        0 2023-03-02 04:02:57.736606 dvadmin-celery-1.0.4/
--rw-rw-rw-   0        0        0     1096 2023-02-23 03:00:37.000000 dvadmin-celery-1.0.4/LICENSE
--rw-rw-rw-   0        0        0       33 2023-02-23 03:00:37.000000 dvadmin-celery-1.0.4/MANIFEST.in
--rw-rw-rw-   0        0        0     3762 2023-03-02 04:02:57.736606 dvadmin-celery-1.0.4/PKG-INFO
--rw-rw-rw-   0        0        0     3282 2023-02-23 03:00:37.000000 dvadmin-celery-1.0.4/README.md
-drwxrwxrwx   0        0        0        0 2023-03-02 04:02:57.727607 dvadmin-celery-1.0.4/dvadmin_celery/
--rw-rw-rw-   0        0        0        0 2023-02-23 03:00:37.000000 dvadmin-celery-1.0.4/dvadmin_celery/__init__.py
--rw-rw-rw-   0        0        0       34 2023-02-23 03:00:37.000000 dvadmin-celery-1.0.4/dvadmin_celery/admin.py
--rw-rw-rw-   0        0        0      200 2023-02-23 03:00:37.000000 dvadmin-celery-1.0.4/dvadmin_celery/apps.py
-drwxrwxrwx   0        0        0        0 2023-03-02 04:02:57.732609 dvadmin-celery-1.0.4/dvadmin_celery/fixtures/
--rw-rw-rw-   0        0        0        0 2023-02-23 03:00:37.000000 dvadmin-celery-1.0.4/dvadmin_celery/fixtures/__init__.py
--rw-rw-rw-   0        0        0      609 2023-02-23 03:00:37.000000 dvadmin-celery-1.0.4/dvadmin_celery/fixtures/initialize.py
--rw-rw-rw-   0        0        0     2174 2023-02-23 03:00:37.000000 dvadmin-celery-1.0.4/dvadmin_celery/settings.py
--rw-rw-rw-   0        0        0      360 2023-02-23 03:00:37.000000 dvadmin-celery-1.0.4/dvadmin_celery/tasks.py
--rw-rw-rw-   0        0        0     1171 2023-02-23 03:00:37.000000 dvadmin-celery-1.0.4/dvadmin_celery/urls.py
-drwxrwxrwx   0        0        0        0 2023-03-02 04:02:57.735609 dvadmin-celery-1.0.4/dvadmin_celery/views/
--rw-rw-rw-   0        0        0        0 2023-02-23 03:00:37.000000 dvadmin-celery-1.0.4/dvadmin_celery/views/__init__.py
--rw-rw-rw-   0        0        0      721 2023-02-23 03:00:37.000000 dvadmin-celery-1.0.4/dvadmin_celery/views/crontab_schedule.py
--rw-rw-rw-   0        0        0      639 2023-02-23 03:00:37.000000 dvadmin-celery-1.0.4/dvadmin_celery/views/interval_schedule.py
--rw-rw-rw-   0        0        0     2719 2023-02-23 03:00:37.000000 dvadmin-celery-1.0.4/dvadmin_celery/views/periodic_task.py
--rw-rw-rw-   0        0        0     5342 2023-02-23 03:00:37.000000 dvadmin-celery-1.0.4/dvadmin_celery/views/task.py
--rw-rw-rw-   0        0        0     1019 2023-02-23 03:00:37.000000 dvadmin-celery-1.0.4/dvadmin_celery/views/task_detail.py
-drwxrwxrwx   0        0        0        0 2023-03-02 04:02:57.731609 dvadmin-celery-1.0.4/dvadmin_celery.egg-info/
--rw-rw-rw-   0        0        0     3762 2023-03-02 04:02:57.000000 dvadmin-celery-1.0.4/dvadmin_celery.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      683 2023-03-02 04:02:57.000000 dvadmin-celery-1.0.4/dvadmin_celery.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-03-02 04:02:57.000000 dvadmin-celery-1.0.4/dvadmin_celery.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0      104 2023-03-02 04:02:57.000000 dvadmin-celery-1.0.4/dvadmin_celery.egg-info/requires.txt
--rw-rw-rw-   0        0        0       15 2023-03-02 04:02:57.000000 dvadmin-celery-1.0.4/dvadmin_celery.egg-info/top_level.txt
--rw-rw-rw-   0        0        0      110 2023-02-23 03:00:37.000000 dvadmin-celery-1.0.4/pyproject.toml
--rw-rw-rw-   0        0        0       42 2023-03-02 04:02:57.736606 dvadmin-celery-1.0.4/setup.cfg
--rw-rw-rw-   0        0        0     1142 2023-03-02 04:00:18.000000 dvadmin-celery-1.0.4/setup.py
+drwxr-xr-x   0 liqiang    (501) staff       (20)        0 2023-06-12 03:28:27.709534 dvadmin-celery-1.0.5/
+-rw-r--r--   0 liqiang    (501) staff       (20)     1075 2022-04-09 09:46:23.000000 dvadmin-celery-1.0.5/LICENSE
+-rw-r--r--   0 liqiang    (501) staff       (20)       33 2022-10-17 01:40:02.000000 dvadmin-celery-1.0.5/MANIFEST.in
+-rw-r--r--   0 liqiang    (501) staff       (20)     3621 2023-06-12 03:28:27.709295 dvadmin-celery-1.0.5/PKG-INFO
+-rw-r--r--   0 liqiang    (501) staff       (20)     3155 2022-10-17 01:40:02.000000 dvadmin-celery-1.0.5/README.md
+drwxr-xr-x   0 liqiang    (501) staff       (20)        0 2023-06-12 03:28:27.705475 dvadmin-celery-1.0.5/dvadmin_celery/
+-rw-r--r--   0 liqiang    (501) staff       (20)        0 2022-04-09 09:46:23.000000 dvadmin-celery-1.0.5/dvadmin_celery/__init__.py
+-rw-r--r--   0 liqiang    (501) staff       (20)       33 2022-04-09 09:46:23.000000 dvadmin-celery-1.0.5/dvadmin_celery/admin.py
+-rw-r--r--   0 liqiang    (501) staff       (20)      193 2022-04-09 09:46:23.000000 dvadmin-celery-1.0.5/dvadmin_celery/apps.py
+drwxr-xr-x   0 liqiang    (501) staff       (20)        0 2023-06-12 03:28:27.707376 dvadmin-celery-1.0.5/dvadmin_celery/fixtures/
+-rw-r--r--   0 liqiang    (501) staff       (20)        0 2022-10-17 01:40:02.000000 dvadmin-celery-1.0.5/dvadmin_celery/fixtures/__init__.py
+-rw-r--r--   0 liqiang    (501) staff       (20)     1683 2023-02-23 14:12:37.000000 dvadmin-celery-1.0.5/dvadmin_celery/fixtures/init_menu.json
+-rw-r--r--   0 liqiang    (501) staff       (20)      583 2022-10-17 01:40:02.000000 dvadmin-celery-1.0.5/dvadmin_celery/fixtures/initialize.py
+-rw-r--r--   0 liqiang    (501) staff       (20)     2115 2022-10-17 01:40:02.000000 dvadmin-celery-1.0.5/dvadmin_celery/settings.py
+-rw-r--r--   0 liqiang    (501) staff       (20)      332 2022-10-17 01:40:02.000000 dvadmin-celery-1.0.5/dvadmin_celery/tasks.py
+-rw-r--r--   0 liqiang    (501) staff       (20)     1146 2022-10-17 01:40:02.000000 dvadmin-celery-1.0.5/dvadmin_celery/urls.py
+drwxr-xr-x   0 liqiang    (501) staff       (20)        0 2023-06-12 03:28:27.708992 dvadmin-celery-1.0.5/dvadmin_celery/views/
+-rw-r--r--   0 liqiang    (501) staff       (20)        0 2022-04-09 09:46:23.000000 dvadmin-celery-1.0.5/dvadmin_celery/views/__init__.py
+-rw-r--r--   0 liqiang    (501) staff       (20)      696 2022-04-09 09:46:23.000000 dvadmin-celery-1.0.5/dvadmin_celery/views/crontab_schedule.py
+-rw-r--r--   0 liqiang    (501) staff       (20)      618 2022-04-09 09:46:23.000000 dvadmin-celery-1.0.5/dvadmin_celery/views/interval_schedule.py
+-rw-r--r--   0 liqiang    (501) staff       (20)     2638 2022-04-09 09:46:23.000000 dvadmin-celery-1.0.5/dvadmin_celery/views/periodic_task.py
+-rw-r--r--   0 liqiang    (501) staff       (20)     5185 2022-10-17 01:40:55.000000 dvadmin-celery-1.0.5/dvadmin_celery/views/task.py
+-rw-r--r--   0 liqiang    (501) staff       (20)      976 2022-10-17 01:40:02.000000 dvadmin-celery-1.0.5/dvadmin_celery/views/task_detail.py
+drwxr-xr-x   0 liqiang    (501) staff       (20)        0 2023-06-12 03:28:27.706712 dvadmin-celery-1.0.5/dvadmin_celery.egg-info/
+-rw-r--r--   0 liqiang    (501) staff       (20)     3621 2023-06-12 03:28:27.000000 dvadmin-celery-1.0.5/dvadmin_celery.egg-info/PKG-INFO
+-rw-r--r--   0 liqiang    (501) staff       (20)      724 2023-06-12 03:28:27.000000 dvadmin-celery-1.0.5/dvadmin_celery.egg-info/SOURCES.txt
+-rw-r--r--   0 liqiang    (501) staff       (20)        1 2023-06-12 03:28:27.000000 dvadmin-celery-1.0.5/dvadmin_celery.egg-info/dependency_links.txt
+-rw-r--r--   0 liqiang    (501) staff       (20)      104 2023-06-12 03:28:27.000000 dvadmin-celery-1.0.5/dvadmin_celery.egg-info/requires.txt
+-rw-r--r--   0 liqiang    (501) staff       (20)       15 2023-06-12 03:28:27.000000 dvadmin-celery-1.0.5/dvadmin_celery.egg-info/top_level.txt
+-rw-r--r--   0 liqiang    (501) staff       (20)      104 2022-04-09 09:46:23.000000 dvadmin-celery-1.0.5/pyproject.toml
+-rw-r--r--   0 liqiang    (501) staff       (20)       38 2023-06-12 03:28:27.709609 dvadmin-celery-1.0.5/setup.cfg
+-rw-r--r--   0 liqiang    (501) staff       (20)      988 2023-06-12 03:26:03.000000 dvadmin-celery-1.0.5/setup.py
```

### Comparing `dvadmin-celery-1.0.4/LICENSE` & `dvadmin-celery-1.0.5/LICENSE`

 * *Ordering differences only*

 * *Files 12% similar despite different names*

```diff
@@ -1,21 +1,21 @@
-MIT License
-
-Copyright (c) [2022] [dvadmin-celery]
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
+Copyright (c) [2022] [dvadmin-celery]
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

### Comparing `dvadmin-celery-1.0.4/PKG-INFO` & `dvadmin-celery-1.0.5/PKG-INFO`

 * *Files 17% similar despite different names*

```diff
@@ -1,141 +1,141 @@
-Metadata-Version: 2.1
-Name: dvadmin-celery
-Version: 1.0.4
-Summary: 适用于 django-vue-admin 的celery异步插件
-Home-page: https://gitee.com/huge-dream/dvadmin-celery
-Author: DVAdmin
-Author-email: liqiang@django-vue-admin.com
-Classifier: Programming Language :: Python :: 3
-Classifier: License :: OSI Approved :: MIT License
-Classifier: Operating System :: OS Independent
-Requires-Python: >=3.7, <4
-Description-Content-Type: text/markdown
-License-File: LICENSE
-
-# dvadmin_celery
-
-#### 介绍
-dvadmin-celery 插件是集成 django-celery-beat、tenant-schemas-celery、django-redis、django-celery-results 的一个后端插件，
-安装可快速使用异步任务，包含在线添加任务、启停任务、查看任务记录等功能。<br>
-与之相对应的是 dvadmin-celery-web 前端插件
-
-## 安装包
-
-使用pip安装软件包：
-
-```python
-pip install dvadmin-celery
-```
-
-目录结构：<br>
-```
-dvadmin-celery
-|   dvdadmin_celery
-|   |   fixtures
-|   |   |   __init__.py
-|   |   |   init_menu.json
-|   |   |   initialize.py
-|   |   views
-|   |   |   __init__.py
-|   |   |   crontab_schedule.py
-|   |   |   interval_schedule.py
-|   |   |   periodic_task.py
-|   |   |   task.py
-|   |   |   task_detail.py
-|   |   __init__.py
-|   |   admin.py
-|   |   apps.py
-|   |   settings.py
-|   |   tasks.py
-|   |   urls.py
-|   setup.py
-```
-
-### 方式一: 一键导入注册配置
-在 application / settings.py 插件配置中下导入默认配置
-```python
-...
-from dvadmin_celery.settings import *
-```
-### 方式二: 手动配置
-在INSTALLED_APPS 中注册app（注意先后顺序）
-
-```python
-INSTALLED_APPS = [
-    ...
-    'django_celery_beat',
-    'django_celery_results',
-    'dvadmin_celery',
-]
-```
-
-在 application / urls.py 中注册url地址
-
-```python
-urlpatterns = [
-    ...
-    path(r'api/dvadmin_celery/', include('dvadmin_celery.urls')),
-]
-```
-
-如果没有系统redis，请启动redis并添加配置 (./conf/env.example.py 及 ./conf/env.py中添加如下配置)
-
-```python
-# redis 配置
-REDIS_PASSWORD = '' # 如果没密码就为空
-REDIS_HOST = '127.0.0.1'
-REDIS_URL = f'redis://:{REDIS_PASSWORD or ""}@{REDIS_HOST}:6379'
-
-```
-
-在 application / settings.py 下添加配置
-
-```python
-...
-CACHES = { # 配置缓存
-    "default": {
-        "BACKEND": "django_redis.cache.RedisCache",
-        "LOCATION": f'{REDIS_URL}/1', # 库名可自选1~16
-        "OPTIONS": {
-            "CLIENT_CLASS": "django_redis.client.DefaultClient",
-        }
-    },
-}
-BROKER_URL = f'{REDIS_URL}/2' # 库名可自选1~16
-CELERY_RESULT_BACKEND = 'django-db' # celery结果存储到数据库中
-CELERYBEAT_SCHEDULER = 'django_celery_beat.schedulers.DatabaseScheduler'  # Backend数据库
-```
-
-进行迁移及初始化
-```python
-python3 manage.py makemigrations 
-python3 manage.py migrate 
-# 注意备份初始化信息
-python3 manage.py init -y 
-```
-
-其他配置请参考 django_celery_beat 和 celery 文档
-
-#### 使用说明
-
-``` python
-mac/linux:
-celery -A application.celery worker -B --loglevel=info
-
-win:
-需要安装: pip install eventlet,需要启动两个程序（worker + beat 顺序不分先后）
-celery -A application.celery worker -P eventlet --loglevel=info
-celery -A application.celery beat --loglevel=info
-```
-
-#### 注意
-``` python
-如果 celery worker 报错 KeyError,可尝试在django_vue_admin/application/celery.py文件里将
-app = Celery(f"application")
-改为
-app = Celery(f"application", include=['dvadmin_celery.tasks'])
-再重启尝试
-```
-redis下载地址：<br>
-Mac/Linux下载 http://download.redis.io/releases/ <br>
-Windows下载 https://github.com/tporadowski/redis/releases/ <br>
+Metadata-Version: 2.1
+Name: dvadmin-celery
+Version: 1.0.5
+Summary: 适用于 django-vue-admin 的celery异步插件
+Home-page: https://gitee.com/huge-dream/dvadmin-celery
+Author: DVAdmin
+Author-email: liqiang@django-vue-admin.com
+Classifier: Programming Language :: Python :: 3
+Classifier: License :: OSI Approved :: MIT License
+Classifier: Operating System :: OS Independent
+Requires-Python: >=3.7, <4
+Description-Content-Type: text/markdown
+License-File: LICENSE
+
+# dvadmin_celery
+
+#### 介绍
+dvadmin-celery 插件是集成 django-celery-beat、tenant-schemas-celery、django-redis、django-celery-results 的一个后端插件，
+安装可快速使用异步任务，包含在线添加任务、启停任务、查看任务记录等功能。<br>
+与之相对应的是 dvadmin-celery-web 前端插件
+
+## 安装包
+
+使用pip安装软件包：
+
+```python
+pip install dvadmin-celery
+```
+
+目录结构：<br>
+```
+dvadmin-celery
+|   dvdadmin_celery
+|   |   fixtures
+|   |   |   __init__.py
+|   |   |   init_menu.json
+|   |   |   initialize.py
+|   |   views
+|   |   |   __init__.py
+|   |   |   crontab_schedule.py
+|   |   |   interval_schedule.py
+|   |   |   periodic_task.py
+|   |   |   task.py
+|   |   |   task_detail.py
+|   |   __init__.py
+|   |   admin.py
+|   |   apps.py
+|   |   settings.py
+|   |   tasks.py
+|   |   urls.py
+|   setup.py
+```
+
+### 方式一: 一键导入注册配置
+在 application / settings.py 插件配置中下导入默认配置
+```python
+...
+from dvadmin_celery.settings import *
+```
+### 方式二: 手动配置
+在INSTALLED_APPS 中注册app（注意先后顺序）
+
+```python
+INSTALLED_APPS = [
+    ...
+    'django_celery_beat',
+    'django_celery_results',
+    'dvadmin_celery',
+]
+```
+
+在 application / urls.py 中注册url地址
+
+```python
+urlpatterns = [
+    ...
+    path(r'api/dvadmin_celery/', include('dvadmin_celery.urls')),
+]
+```
+
+如果没有系统redis，请启动redis并添加配置 (./conf/env.example.py 及 ./conf/env.py中添加如下配置)
+
+```python
+# redis 配置
+REDIS_PASSWORD = '' # 如果没密码就为空
+REDIS_HOST = '127.0.0.1'
+REDIS_URL = f'redis://:{REDIS_PASSWORD or ""}@{REDIS_HOST}:6379'
+
+```
+
+在 application / settings.py 下添加配置
+
+```python
+...
+CACHES = { # 配置缓存
+    "default": {
+        "BACKEND": "django_redis.cache.RedisCache",
+        "LOCATION": f'{REDIS_URL}/1', # 库名可自选1~16
+        "OPTIONS": {
+            "CLIENT_CLASS": "django_redis.client.DefaultClient",
+        }
+    },
+}
+BROKER_URL = f'{REDIS_URL}/2' # 库名可自选1~16
+CELERY_RESULT_BACKEND = 'django-db' # celery结果存储到数据库中
+CELERYBEAT_SCHEDULER = 'django_celery_beat.schedulers.DatabaseScheduler'  # Backend数据库
+```
+
+进行迁移及初始化
+```python
+python3 manage.py makemigrations 
+python3 manage.py migrate 
+# 注意备份初始化信息
+python3 manage.py init -y 
+```
+
+其他配置请参考 django_celery_beat 和 celery 文档
+
+#### 使用说明
+
+``` python
+mac/linux:
+celery -A application.celery worker -B --loglevel=info
+
+win:
+需要安装: pip install eventlet,需要启动两个程序（worker + beat 顺序不分先后）
+celery -A application.celery worker -P eventlet --loglevel=info
+celery -A application.celery beat --loglevel=info
+```
+
+#### 注意
+``` python
+如果 celery worker 报错 KeyError,可尝试在django_vue_admin/application/celery.py文件里将
+app = Celery(f"application")
+改为
+app = Celery(f"application", include=['dvadmin_celery.tasks'])
+再重启尝试
+```
+redis下载地址：<br>
+Mac/Linux下载 http://download.redis.io/releases/ <br>
+Windows下载 https://github.com/tporadowski/redis/releases/ <br>
```

### Comparing `dvadmin-celery-1.0.4/README.md` & `dvadmin-celery-1.0.5/README.md`

 * *Ordering differences only*

 * *Files 19% similar despite different names*

```diff
@@ -1,127 +1,127 @@
-# dvadmin_celery
-
-#### 介绍
-dvadmin-celery 插件是集成 django-celery-beat、tenant-schemas-celery、django-redis、django-celery-results 的一个后端插件，
-安装可快速使用异步任务，包含在线添加任务、启停任务、查看任务记录等功能。<br>
-与之相对应的是 dvadmin-celery-web 前端插件
-
-## 安装包
-
-使用pip安装软件包：
-
-```python
-pip install dvadmin-celery
-```
-
-目录结构：<br>
-```
-dvadmin-celery
-|   dvdadmin_celery
-|   |   fixtures
-|   |   |   __init__.py
-|   |   |   init_menu.json
-|   |   |   initialize.py
-|   |   views
-|   |   |   __init__.py
-|   |   |   crontab_schedule.py
-|   |   |   interval_schedule.py
-|   |   |   periodic_task.py
-|   |   |   task.py
-|   |   |   task_detail.py
-|   |   __init__.py
-|   |   admin.py
-|   |   apps.py
-|   |   settings.py
-|   |   tasks.py
-|   |   urls.py
-|   setup.py
-```
-
-### 方式一: 一键导入注册配置
-在 application / settings.py 插件配置中下导入默认配置
-```python
-...
-from dvadmin_celery.settings import *
-```
-### 方式二: 手动配置
-在INSTALLED_APPS 中注册app（注意先后顺序）
-
-```python
-INSTALLED_APPS = [
-    ...
-    'django_celery_beat',
-    'django_celery_results',
-    'dvadmin_celery',
-]
-```
-
-在 application / urls.py 中注册url地址
-
-```python
-urlpatterns = [
-    ...
-    path(r'api/dvadmin_celery/', include('dvadmin_celery.urls')),
-]
-```
-
-如果没有系统redis，请启动redis并添加配置 (./conf/env.example.py 及 ./conf/env.py中添加如下配置)
-
-```python
-# redis 配置
-REDIS_PASSWORD = '' # 如果没密码就为空
-REDIS_HOST = '127.0.0.1'
-REDIS_URL = f'redis://:{REDIS_PASSWORD or ""}@{REDIS_HOST}:6379'
-
-```
-
-在 application / settings.py 下添加配置
-
-```python
-...
-CACHES = { # 配置缓存
-    "default": {
-        "BACKEND": "django_redis.cache.RedisCache",
-        "LOCATION": f'{REDIS_URL}/1', # 库名可自选1~16
-        "OPTIONS": {
-            "CLIENT_CLASS": "django_redis.client.DefaultClient",
-        }
-    },
-}
-BROKER_URL = f'{REDIS_URL}/2' # 库名可自选1~16
-CELERY_RESULT_BACKEND = 'django-db' # celery结果存储到数据库中
-CELERYBEAT_SCHEDULER = 'django_celery_beat.schedulers.DatabaseScheduler'  # Backend数据库
-```
-
-进行迁移及初始化
-```python
-python3 manage.py makemigrations 
-python3 manage.py migrate 
-# 注意备份初始化信息
-python3 manage.py init -y 
-```
-
-其他配置请参考 django_celery_beat 和 celery 文档
-
-#### 使用说明
-
-``` python
-mac/linux:
-celery -A application.celery worker -B --loglevel=info
-
-win:
-需要安装: pip install eventlet,需要启动两个程序（worker + beat 顺序不分先后）
-celery -A application.celery worker -P eventlet --loglevel=info
-celery -A application.celery beat --loglevel=info
-```
-
-#### 注意
-``` python
-如果 celery worker 报错 KeyError,可尝试在django_vue_admin/application/celery.py文件里将
-app = Celery(f"application")
-改为
-app = Celery(f"application", include=['dvadmin_celery.tasks'])
-再重启尝试
-```
-redis下载地址：<br>
-Mac/Linux下载 http://download.redis.io/releases/ <br>
-Windows下载 https://github.com/tporadowski/redis/releases/ <br>
+# dvadmin_celery
+
+#### 介绍
+dvadmin-celery 插件是集成 django-celery-beat、tenant-schemas-celery、django-redis、django-celery-results 的一个后端插件，
+安装可快速使用异步任务，包含在线添加任务、启停任务、查看任务记录等功能。<br>
+与之相对应的是 dvadmin-celery-web 前端插件
+
+## 安装包
+
+使用pip安装软件包：
+
+```python
+pip install dvadmin-celery
+```
+
+目录结构：<br>
+```
+dvadmin-celery
+|   dvdadmin_celery
+|   |   fixtures
+|   |   |   __init__.py
+|   |   |   init_menu.json
+|   |   |   initialize.py
+|   |   views
+|   |   |   __init__.py
+|   |   |   crontab_schedule.py
+|   |   |   interval_schedule.py
+|   |   |   periodic_task.py
+|   |   |   task.py
+|   |   |   task_detail.py
+|   |   __init__.py
+|   |   admin.py
+|   |   apps.py
+|   |   settings.py
+|   |   tasks.py
+|   |   urls.py
+|   setup.py
+```
+
+### 方式一: 一键导入注册配置
+在 application / settings.py 插件配置中下导入默认配置
+```python
+...
+from dvadmin_celery.settings import *
+```
+### 方式二: 手动配置
+在INSTALLED_APPS 中注册app（注意先后顺序）
+
+```python
+INSTALLED_APPS = [
+    ...
+    'django_celery_beat',
+    'django_celery_results',
+    'dvadmin_celery',
+]
+```
+
+在 application / urls.py 中注册url地址
+
+```python
+urlpatterns = [
+    ...
+    path(r'api/dvadmin_celery/', include('dvadmin_celery.urls')),
+]
+```
+
+如果没有系统redis，请启动redis并添加配置 (./conf/env.example.py 及 ./conf/env.py中添加如下配置)
+
+```python
+# redis 配置
+REDIS_PASSWORD = '' # 如果没密码就为空
+REDIS_HOST = '127.0.0.1'
+REDIS_URL = f'redis://:{REDIS_PASSWORD or ""}@{REDIS_HOST}:6379'
+
+```
+
+在 application / settings.py 下添加配置
+
+```python
+...
+CACHES = { # 配置缓存
+    "default": {
+        "BACKEND": "django_redis.cache.RedisCache",
+        "LOCATION": f'{REDIS_URL}/1', # 库名可自选1~16
+        "OPTIONS": {
+            "CLIENT_CLASS": "django_redis.client.DefaultClient",
+        }
+    },
+}
+BROKER_URL = f'{REDIS_URL}/2' # 库名可自选1~16
+CELERY_RESULT_BACKEND = 'django-db' # celery结果存储到数据库中
+CELERYBEAT_SCHEDULER = 'django_celery_beat.schedulers.DatabaseScheduler'  # Backend数据库
+```
+
+进行迁移及初始化
+```python
+python3 manage.py makemigrations 
+python3 manage.py migrate 
+# 注意备份初始化信息
+python3 manage.py init -y 
+```
+
+其他配置请参考 django_celery_beat 和 celery 文档
+
+#### 使用说明
+
+``` python
+mac/linux:
+celery -A application.celery worker -B --loglevel=info
+
+win:
+需要安装: pip install eventlet,需要启动两个程序（worker + beat 顺序不分先后）
+celery -A application.celery worker -P eventlet --loglevel=info
+celery -A application.celery beat --loglevel=info
+```
+
+#### 注意
+``` python
+如果 celery worker 报错 KeyError,可尝试在django_vue_admin/application/celery.py文件里将
+app = Celery(f"application")
+改为
+app = Celery(f"application", include=['dvadmin_celery.tasks'])
+再重启尝试
+```
+redis下载地址：<br>
+Mac/Linux下载 http://download.redis.io/releases/ <br>
+Windows下载 https://github.com/tporadowski/redis/releases/ <br>
```

### Comparing `dvadmin-celery-1.0.4/dvadmin_celery/fixtures/initialize.py` & `dvadmin-celery-1.0.5/dvadmin_celery/fixtures/initialize.py`

 * *Ordering differences only*

 * *Files 20% similar despite different names*

```diff
@@ -1,26 +1,26 @@
-# 初始化
-import os
-
-import django
-
-os.environ.setdefault("DJANGO_SETTINGS_MODULE", "application.settings")
-django.setup()
-
-from dvadmin.system.views.menu import MenuInitSerializer
-from dvadmin.utils.core_initialize import CoreInitialize
-
-
-class Initialize(CoreInitialize):
-
-    def init_menu(self):
-        """
-        初始化菜单信息
-        """
-        self.init_base(MenuInitSerializer, unique_fields=['name', 'web_path', 'component', 'component_name'])
-
-    def run(self):
-        self.init_menu()
-
-
-if __name__ == "__main__":
-    Initialize(app='dvadmin_celery').run()
+# 初始化
+import os
+
+import django
+
+os.environ.setdefault("DJANGO_SETTINGS_MODULE", "application.settings")
+django.setup()
+
+from dvadmin.system.views.menu import MenuInitSerializer
+from dvadmin.utils.core_initialize import CoreInitialize
+
+
+class Initialize(CoreInitialize):
+
+    def init_menu(self):
+        """
+        初始化菜单信息
+        """
+        self.init_base(MenuInitSerializer, unique_fields=['name', 'web_path', 'component', 'component_name'])
+
+    def run(self):
+        self.init_menu()
+
+
+if __name__ == "__main__":
+    Initialize(app='dvadmin_celery').run()
```

### Comparing `dvadmin-celery-1.0.4/dvadmin_celery/settings.py` & `dvadmin-celery-1.0.5/dvadmin_celery/settings.py`

 * *Ordering differences only*

 * *Files 26% similar despite different names*

```diff
@@ -1,60 +1,60 @@
-from application import settings
-
-# ================================================= #
-# ***************** 插件配置区开始 *******************
-# ================================================= #
-# 路由配置
-plugins_url_patterns = [
-    {"re_path": r'api/dvadmin_celery/', "include": "dvadmin_celery.urls"}
-]
-# app 配置
-apps = ['django_celery_beat', 'django_celery_results', 'dvadmin_celery']
-# 租户模式中，public模式共享app配置
-tenant_shared_apps = []
-# ================================================= #
-# ******************* 插件配置区结束 *****************
-# ================================================= #
-
-if not hasattr(settings, 'CACHES'):
-    _DEFAULT_CACHES = {
-        "default": {
-            "BACKEND": "django_redis.cache.RedisCache",
-            "LOCATION": f'{settings.REDIS_URL}/1',
-            "OPTIONS": {
-                "CLIENT_CLASS": "django_redis.client.DefaultClient",
-            }
-        },
-    }
-else:
-    _DEFAULT_CACHES = settings.CACHES
-
-if not hasattr(settings, 'REDIS_URL'):
-    raise Exception("请配置redis地址，否则celery无法使用！")
-
-# ********** 赋值到 settings 中 **********
-settings.CACHES = _DEFAULT_CACHES
-settings.INSTALLED_APPS += [app for app in apps if app not in settings.INSTALLED_APPS]
-settings.TENANT_SHARED_APPS += tenant_shared_apps
-
-# ********** celery 配置 **********
-if not hasattr(settings, 'BROKER_URL'):
-    settings.BROKER_URL = f'{settings.REDIS_URL}/2'
-
-# ********** 执行结果保存位置 **********
-if not hasattr(settings, 'CELERY_RESULT_BACKEND'):
-    settings.CELERY_RESULT_BACKEND = 'django-db'
-
-# ********** Backend数据库 **********
-if not hasattr(settings, 'CELERYBEAT_SCHEDULER'):
-    settings.CELERYBEAT_SCHEDULER = 'django_celery_beat.schedulers.DatabaseScheduler'
-
-# ********** 执行结果扩展 **********
-if not hasattr(settings, 'CELERY_RESULT_EXTENDED'):
-    settings.CELERY_RESULT_EXTENDED = True
-
-# ********** 注册路由 **********
-settings.PLUGINS_URL_PATTERNS += plugins_url_patterns
-
-# 避免时区的问题
-CELERY_ENABLE_UTC = False
+from application import settings
+
+# ================================================= #
+# ***************** 插件配置区开始 *******************
+# ================================================= #
+# 路由配置
+plugins_url_patterns = [
+    {"re_path": r'api/dvadmin_celery/', "include": "dvadmin_celery.urls"}
+]
+# app 配置
+apps = ['django_celery_beat', 'django_celery_results', 'dvadmin_celery']
+# 租户模式中，public模式共享app配置
+tenant_shared_apps = []
+# ================================================= #
+# ******************* 插件配置区结束 *****************
+# ================================================= #
+
+if not hasattr(settings, 'CACHES'):
+    _DEFAULT_CACHES = {
+        "default": {
+            "BACKEND": "django_redis.cache.RedisCache",
+            "LOCATION": f'{settings.REDIS_URL}/1',
+            "OPTIONS": {
+                "CLIENT_CLASS": "django_redis.client.DefaultClient",
+            }
+        },
+    }
+else:
+    _DEFAULT_CACHES = settings.CACHES
+
+if not hasattr(settings, 'REDIS_URL'):
+    raise Exception("请配置redis地址，否则celery无法使用！")
+
+# ********** 赋值到 settings 中 **********
+settings.CACHES = _DEFAULT_CACHES
+settings.INSTALLED_APPS += [app for app in apps if app not in settings.INSTALLED_APPS]
+settings.TENANT_SHARED_APPS += tenant_shared_apps
+
+# ********** celery 配置 **********
+if not hasattr(settings, 'BROKER_URL'):
+    settings.BROKER_URL = f'{settings.REDIS_URL}/2'
+
+# ********** 执行结果保存位置 **********
+if not hasattr(settings, 'CELERY_RESULT_BACKEND'):
+    settings.CELERY_RESULT_BACKEND = 'django-db'
+
+# ********** Backend数据库 **********
+if not hasattr(settings, 'CELERYBEAT_SCHEDULER'):
+    settings.CELERYBEAT_SCHEDULER = 'django_celery_beat.schedulers.DatabaseScheduler'
+
+# ********** 执行结果扩展 **********
+if not hasattr(settings, 'CELERY_RESULT_EXTENDED'):
+    settings.CELERY_RESULT_EXTENDED = True
+
+# ********** 注册路由 **********
+settings.PLUGINS_URL_PATTERNS += plugins_url_patterns
+
+# 避免时区的问题
+CELERY_ENABLE_UTC = False
 DJANGO_CELERY_BEAT_TZ_AWARE = False
```

### Comparing `dvadmin-celery-1.0.4/dvadmin_celery/views/crontab_schedule.py` & `dvadmin-celery-1.0.5/dvadmin_celery/views/crontab_schedule.py`

 * *Ordering differences only*

 * *Files 10% similar despite different names*

```diff
@@ -1,25 +1,25 @@
-from django_celery_beat.models import CrontabSchedule
-
-from dvadmin.utils.serializers import CustomModelSerializer
-from dvadmin.utils.viewset import CustomModelViewSet
-
-
-class CrontabScheduleSerializer(CustomModelSerializer):
-    class Meta:
-        model = CrontabSchedule
-        exclude = ('timezone',)
-
-
-class CrontabScheduleModelViewSet(CustomModelViewSet):
-    """
-    CrontabSchedule crontab调度模型
-    minute 分钟
-    hour 小时
-    day_of_week 每周的周几
-    day_of_month 每月的某一天
-    month_of_year 每年的某一个月
-
-    """
-    queryset = CrontabSchedule.objects.all()
-    serializer_class = CrontabScheduleSerializer
-    ordering = 'minute'  # 默认排序
+from django_celery_beat.models import CrontabSchedule
+
+from dvadmin.utils.serializers import CustomModelSerializer
+from dvadmin.utils.viewset import CustomModelViewSet
+
+
+class CrontabScheduleSerializer(CustomModelSerializer):
+    class Meta:
+        model = CrontabSchedule
+        exclude = ('timezone',)
+
+
+class CrontabScheduleModelViewSet(CustomModelViewSet):
+    """
+    CrontabSchedule crontab调度模型
+    minute 分钟
+    hour 小时
+    day_of_week 每周的周几
+    day_of_month 每月的某一天
+    month_of_year 每年的某一个月
+
+    """
+    queryset = CrontabSchedule.objects.all()
+    serializer_class = CrontabScheduleSerializer
+    ordering = 'minute'  # 默认排序
```

### Comparing `dvadmin-celery-1.0.4/dvadmin_celery/views/interval_schedule.py` & `dvadmin-celery-1.0.5/dvadmin_celery/views/interval_schedule.py`

 * *Ordering differences only*

 * *Files 19% similar despite different names*

```diff
@@ -1,21 +1,21 @@
-from django_celery_beat.models import IntervalSchedule
-
-from dvadmin.utils.serializers import CustomModelSerializer
-from dvadmin.utils.viewset import CustomModelViewSet
-
-
-class IntervalScheduleSerializer(CustomModelSerializer):
-    class Meta:
-        model = IntervalSchedule
-        fields = '__all__'
-
-
-class IntervalScheduleModelViewSet(CustomModelViewSet):
-    """
-    IntervalSchedule 调度间隔模型
-    every 次数
-    period 时间(天,小时,分钟,秒.毫秒)
-    """
-    queryset = IntervalSchedule.objects.all()
-    serializer_class = IntervalScheduleSerializer
-    ordering = 'every'  # 默认排序
+from django_celery_beat.models import IntervalSchedule
+
+from dvadmin.utils.serializers import CustomModelSerializer
+from dvadmin.utils.viewset import CustomModelViewSet
+
+
+class IntervalScheduleSerializer(CustomModelSerializer):
+    class Meta:
+        model = IntervalSchedule
+        fields = '__all__'
+
+
+class IntervalScheduleModelViewSet(CustomModelViewSet):
+    """
+    IntervalSchedule 调度间隔模型
+    every 次数
+    period 时间(天,小时,分钟,秒.毫秒)
+    """
+    queryset = IntervalSchedule.objects.all()
+    serializer_class = IntervalScheduleSerializer
+    ordering = 'every'  # 默认排序
```

### Comparing `dvadmin-celery-1.0.4/dvadmin_celery/views/periodic_task.py` & `dvadmin-celery-1.0.5/dvadmin_celery/views/periodic_task.py`

 * *Ordering differences only*

 * *Files 23% similar despite different names*

```diff
@@ -1,81 +1,81 @@
-from django_celery_beat.models import PeriodicTask
-from rest_framework import serializers
-
-from dvadmin.utils.json_response import SuccessResponse, ErrorResponse
-from dvadmin.utils.serializers import CustomModelSerializer
-from dvadmin.utils.viewset import CustomModelViewSet
-from ..views.crontab_schedule import CrontabScheduleSerializer
-from ..views.interval_schedule import IntervalScheduleSerializer
-
-
-class PeriodicTaskSerializer(CustomModelSerializer):
-    interval_list = serializers.SerializerMethodField(read_only=True)
-    crontab_list = serializers.SerializerMethodField(read_only=True)
-
-    def get_interval_list(self, obj):
-        return IntervalScheduleSerializer(obj.interval).data if obj.interval else {}
-
-    def get_crontab_list(self, obj):
-        return CrontabScheduleSerializer(obj.crontab).data if obj.crontab else {}
-
-    class Meta:
-        model = PeriodicTask
-        fields = '__all__'
-
-
-class PeriodicTaskModelViewSet(CustomModelViewSet):
-    """
-    PeriodicTask celery 任务数据模型
-    name 名称
-    task celery任务名称
-    interval 频率
-    crontab 任务编排
-    args 形式参数
-    kwargs 位置参数
-    queue 队列名称
-    exchange 交换
-    routing_key 路由密钥
-    expires 过期时间
-    enabled 是否开启
-
-    """
-    queryset = PeriodicTask.objects.exclude(name="celery.backend_cleanup")
-    serializer_class = PeriodicTaskSerializer
-    ordering = 'date_changed'  # 默认排序
-
-    def tasks_as_choices(self, request, *args, **kwargs):
-        """
-        获取所有 tasks 名称
-        :param request:
-        :param args:
-        :param kwargs:
-        :return:
-        """
-        lis = []
-
-        def get_data(datas):
-            for item in datas:
-                if isinstance(item, (str, int)) and item:
-                    lis.append(item)
-                else:
-                    get_data(item)
-
-        from celery import current_app
-        tasks = list(sorted(name for name in current_app.tasks
-                            if not name.startswith('celery.')))
-        get_data((('', ''),) + tuple(zip(tasks, tasks)))
-        return SuccessResponse(list(set(lis)))
-
-    def operate_celery(self, request, *args, **kwargs):
-        task_name = request.data.get('celery_name', '')
-        data = {
-            'task': None
-        }
-        test = f"""
-from {'.'.join(task_name.split('.')[:-1])} import {task_name.split('.')[-1]}
-task = {task_name.split('.')[-1]}.delay()
-        """
-        exec(test, data)
-        if not data["task"]:
-            ErrorResponse(msg="执行失败")
-        return SuccessResponse({'task_id': data.get('task', ).id})
+from django_celery_beat.models import PeriodicTask
+from rest_framework import serializers
+
+from dvadmin.utils.json_response import SuccessResponse, ErrorResponse
+from dvadmin.utils.serializers import CustomModelSerializer
+from dvadmin.utils.viewset import CustomModelViewSet
+from ..views.crontab_schedule import CrontabScheduleSerializer
+from ..views.interval_schedule import IntervalScheduleSerializer
+
+
+class PeriodicTaskSerializer(CustomModelSerializer):
+    interval_list = serializers.SerializerMethodField(read_only=True)
+    crontab_list = serializers.SerializerMethodField(read_only=True)
+
+    def get_interval_list(self, obj):
+        return IntervalScheduleSerializer(obj.interval).data if obj.interval else {}
+
+    def get_crontab_list(self, obj):
+        return CrontabScheduleSerializer(obj.crontab).data if obj.crontab else {}
+
+    class Meta:
+        model = PeriodicTask
+        fields = '__all__'
+
+
+class PeriodicTaskModelViewSet(CustomModelViewSet):
+    """
+    PeriodicTask celery 任务数据模型
+    name 名称
+    task celery任务名称
+    interval 频率
+    crontab 任务编排
+    args 形式参数
+    kwargs 位置参数
+    queue 队列名称
+    exchange 交换
+    routing_key 路由密钥
+    expires 过期时间
+    enabled 是否开启
+
+    """
+    queryset = PeriodicTask.objects.exclude(name="celery.backend_cleanup")
+    serializer_class = PeriodicTaskSerializer
+    ordering = 'date_changed'  # 默认排序
+
+    def tasks_as_choices(self, request, *args, **kwargs):
+        """
+        获取所有 tasks 名称
+        :param request:
+        :param args:
+        :param kwargs:
+        :return:
+        """
+        lis = []
+
+        def get_data(datas):
+            for item in datas:
+                if isinstance(item, (str, int)) and item:
+                    lis.append(item)
+                else:
+                    get_data(item)
+
+        from celery import current_app
+        tasks = list(sorted(name for name in current_app.tasks
+                            if not name.startswith('celery.')))
+        get_data((('', ''),) + tuple(zip(tasks, tasks)))
+        return SuccessResponse(list(set(lis)))
+
+    def operate_celery(self, request, *args, **kwargs):
+        task_name = request.data.get('celery_name', '')
+        data = {
+            'task': None
+        }
+        test = f"""
+from {'.'.join(task_name.split('.')[:-1])} import {task_name.split('.')[-1]}
+task = {task_name.split('.')[-1]}.delay()
+        """
+        exec(test, data)
+        if not data["task"]:
+            ErrorResponse(msg="执行失败")
+        return SuccessResponse({'task_id': data.get('task', ).id})
```

### Comparing `dvadmin-celery-1.0.4/dvadmin_celery/views/task.py` & `dvadmin-celery-1.0.5/dvadmin_celery/views/task.py`

 * *Ordering differences only*

 * *Files 14% similar despite different names*

```diff
@@ -1,157 +1,157 @@
-# -*- coding: utf-8 -*-
-
-"""
-@author: 阿辉
-@contact: QQ:2655399832
-@Created on: 2022/9/21 16:30
-@Remark:
-"""
-import uuid
-
-from django_celery_beat.models import PeriodicTask, CrontabSchedule, cronexp
-from rest_framework.exceptions import APIException
-from rest_framework import serializers
-
-from dvadmin.utils.serializers import CustomModelSerializer
-from dvadmin.utils.viewset import CustomModelViewSet
-from dvadmin.utils.json_response import SuccessResponse, ErrorResponse
-
-
-CrontabSchedule.__str__ = lambda self : '{0} {1} {2} {3} {4} {5}'.format(
-            cronexp(self.minute), cronexp(self.hour),
-            cronexp(self.day_of_month), cronexp(self.month_of_year),
-            cronexp(self.day_of_week), str(self.timezone)
-        )
-
-
-
-
-def get_job_list():
-    from application import settings
-    task_list = []
-    task_dict_list = []
-    for app in settings.INSTALLED_APPS:
-        try:
-            exec(f"""
-from {app} import tasks
-for ele in [i for i in dir(tasks) if i.startswith('task__')]:
-    task_dict = dict()
-    task_dict['label'] = '{app}.tasks.' + ele
-    task_dict['value'] = '{app}.tasks.' + ele
-    task_list.append('{app}.tasks.' + ele)
-    task_dict_list.append(task_dict)
-                """)
-        except ImportError :
-            pass
-    return {'task_list': task_list, 'task_dict_list': task_dict_list}
-
-
-#将cron表达式进行解析
-def CronSlpit(cron):
-    cron = cron.split(" ")
-    result = {
-        # "second":cron[0],
-        "minute":cron[0],
-        "hour":cron[1],
-        "day":cron[2],
-        "month":cron[3],
-        "week":cron[4]
-    }
-    return result
-
-
-class CeleryCrontabScheduleSerializer(CustomModelSerializer):
-    class Meta:
-        model = CrontabSchedule
-        exclude = ('timezone',)
-
-
-class PeriodicTasksSerializer(CustomModelSerializer):
-    crontab = serializers.StringRelatedField(read_only=True)
-
-    class Meta:
-        model = PeriodicTask
-        fields = '__all__'
-
-
-class CeleryTaskModelViewSet(CustomModelViewSet):
-    """
-    CeleryTask 添加任务调度
-    """
-
-    queryset = PeriodicTask.objects.exclude(name="celery.backend_cleanup")
-    serializer_class = PeriodicTasksSerializer
-    filter_fields = ['name', 'task', 'enabled']
-    # permission_classes = []
-    # authentication_classes = []
-
-    def list(self, request, *args, **kwargs):
-        queryset = self.filter_queryset(self.get_queryset())
-        page = self.paginate_queryset(queryset)
-        if page is not None:
-            serializer = self.get_serializer(page, many=True, request=request)
-            return self.get_paginated_response(serializer.data)
-        serializer = self.get_serializer(queryset, many=True, request=request)
-        return SuccessResponse(data=serializer.data, msg="获取成功")
-
-    def job_list(self, request, *args, **kwargs):
-        """获取所有任务"""
-        result = get_job_list()
-        task_list = result.get('task_dict_list')
-        return SuccessResponse(msg='获取成功', data=task_list, total=len(task_list))
-
-    def create(self, request, *args, **kwargs):
-        body_data = request.data.copy()
-        cron = body_data.get('crontab')
-        cron_lisr = CronSlpit(cron)
-        minute = cron_lisr["minute"]
-        hour = cron_lisr["hour"]
-        day = cron_lisr["day"]
-        month = cron_lisr["month"]
-        week = cron_lisr["week"]
-        cron_data = {
-            'minute': minute,
-            'hour': hour,
-            'day_of_week': week,
-            'day_of_month': day,
-            'month_of_year': month
-        }
-        task = body_data.get('task')
-        result = None
-        task_list = get_job_list()
-        task_list = task_list.get('task_list')
-        if task in task_list:
-            # job_name = task.split('.')[-1]
-            # path_name = '.'.join(task.split('.')[:-1])
-
-            # 添加crontab
-            serializer = CeleryCrontabScheduleSerializer(data=cron_data, request=request)
-            serializer.is_valid(raise_exception=True)
-            self.perform_create(serializer)
-
-            # 添加任务
-            body_data['crontab'] = serializer.data.get('id')
-            body_data['enabled'] = False
-            serializer = self.get_serializer(data=body_data, request=request)
-            res = serializer.is_valid()
-            if not res:
-                raise APIException({"msg":f"添加失败，已经有一个名为 {body_data['name']} 的任务了"}, code=4000)
-            self.perform_create(serializer)
-            result = serializer.data
-            return SuccessResponse(msg="添加成功", data=result)
-        else:
-            return ErrorResponse(msg="添加失败,没有该任务", data=None)
-
-    def destroy(self, request, *args, **kwargs):
-        """删除定时任务"""
-        instance = self.get_object()
-        self.perform_destroy(instance)
-        return SuccessResponse(data=[], msg="删除成功")
-
-    def update_status(self,request, *args, **kwargs):
-        """开始/暂停任务"""
-        instance = self.get_object()
-        body_data = request.data
-        instance.enabled = body_data.get('enabled')
-        instance.save()
-        return SuccessResponse(msg="修改成功", data=None)
+# -*- coding: utf-8 -*-
+
+"""
+@author: 阿辉
+@contact: QQ:2655399832
+@Created on: 2022/9/21 16:30
+@Remark:
+"""
+import uuid
+
+from django_celery_beat.models import PeriodicTask, CrontabSchedule, cronexp
+from rest_framework.exceptions import APIException
+from rest_framework import serializers
+
+from dvadmin.utils.serializers import CustomModelSerializer
+from dvadmin.utils.viewset import CustomModelViewSet
+from dvadmin.utils.json_response import SuccessResponse, ErrorResponse
+
+
+CrontabSchedule.__str__ = lambda self : '{0} {1} {2} {3} {4} {5}'.format(
+            cronexp(self.minute), cronexp(self.hour),
+            cronexp(self.day_of_month), cronexp(self.month_of_year),
+            cronexp(self.day_of_week), str(self.timezone)
+        )
+
+
+
+
+def get_job_list():
+    from application import settings
+    task_list = []
+    task_dict_list = []
+    for app in settings.INSTALLED_APPS:
+        try:
+            exec(f"""
+from {app} import tasks
+for ele in [i for i in dir(tasks) if i.startswith('task__')]:
+    task_dict = dict()
+    task_dict['label'] = '{app}.tasks.' + ele
+    task_dict['value'] = '{app}.tasks.' + ele
+    task_list.append('{app}.tasks.' + ele)
+    task_dict_list.append(task_dict)
+                """)
+        except ImportError :
+            pass
+    return {'task_list': task_list, 'task_dict_list': task_dict_list}
+
+
+#将cron表达式进行解析
+def CronSlpit(cron):
+    cron = cron.split(" ")
+    result = {
+        # "second":cron[0],
+        "minute":cron[0],
+        "hour":cron[1],
+        "day":cron[2],
+        "month":cron[3],
+        "week":cron[4]
+    }
+    return result
+
+
+class CeleryCrontabScheduleSerializer(CustomModelSerializer):
+    class Meta:
+        model = CrontabSchedule
+        exclude = ('timezone',)
+
+
+class PeriodicTasksSerializer(CustomModelSerializer):
+    crontab = serializers.StringRelatedField(read_only=True)
+
+    class Meta:
+        model = PeriodicTask
+        fields = '__all__'
+
+
+class CeleryTaskModelViewSet(CustomModelViewSet):
+    """
+    CeleryTask 添加任务调度
+    """
+
+    queryset = PeriodicTask.objects.exclude(name="celery.backend_cleanup")
+    serializer_class = PeriodicTasksSerializer
+    filter_fields = ['name', 'task', 'enabled']
+    # permission_classes = []
+    # authentication_classes = []
+
+    def list(self, request, *args, **kwargs):
+        queryset = self.filter_queryset(self.get_queryset())
+        page = self.paginate_queryset(queryset)
+        if page is not None:
+            serializer = self.get_serializer(page, many=True, request=request)
+            return self.get_paginated_response(serializer.data)
+        serializer = self.get_serializer(queryset, many=True, request=request)
+        return SuccessResponse(data=serializer.data, msg="获取成功")
+
+    def job_list(self, request, *args, **kwargs):
+        """获取所有任务"""
+        result = get_job_list()
+        task_list = result.get('task_dict_list')
+        return SuccessResponse(msg='获取成功', data=task_list, total=len(task_list))
+
+    def create(self, request, *args, **kwargs):
+        body_data = request.data.copy()
+        cron = body_data.get('crontab')
+        cron_lisr = CronSlpit(cron)
+        minute = cron_lisr["minute"]
+        hour = cron_lisr["hour"]
+        day = cron_lisr["day"]
+        month = cron_lisr["month"]
+        week = cron_lisr["week"]
+        cron_data = {
+            'minute': minute,
+            'hour': hour,
+            'day_of_week': week,
+            'day_of_month': day,
+            'month_of_year': month
+        }
+        task = body_data.get('task')
+        result = None
+        task_list = get_job_list()
+        task_list = task_list.get('task_list')
+        if task in task_list:
+            # job_name = task.split('.')[-1]
+            # path_name = '.'.join(task.split('.')[:-1])
+
+            # 添加crontab
+            serializer = CeleryCrontabScheduleSerializer(data=cron_data, request=request)
+            serializer.is_valid(raise_exception=True)
+            self.perform_create(serializer)
+
+            # 添加任务
+            body_data['crontab'] = serializer.data.get('id')
+            body_data['enabled'] = False
+            serializer = self.get_serializer(data=body_data, request=request)
+            res = serializer.is_valid()
+            if not res:
+                raise APIException({"msg":f"添加失败，已经有一个名为 {body_data['name']} 的任务了"}, code=4000)
+            self.perform_create(serializer)
+            result = serializer.data
+            return SuccessResponse(msg="添加成功", data=result)
+        else:
+            return ErrorResponse(msg="添加失败,没有该任务", data=None)
+
+    def destroy(self, request, *args, **kwargs):
+        """删除定时任务"""
+        instance = self.get_object()
+        self.perform_destroy(instance)
+        return SuccessResponse(data=[], msg="删除成功")
+
+    def update_status(self,request, *args, **kwargs):
+        """开始/暂停任务"""
+        instance = self.get_object()
+        body_data = request.data
+        instance.enabled = body_data.get('enabled')
+        instance.save()
+        return SuccessResponse(msg="修改成功", data=None)
```

### Comparing `dvadmin-celery-1.0.4/dvadmin_celery/views/task_detail.py` & `dvadmin-celery-1.0.5/dvadmin_celery/views/task_detail.py`

 * *Ordering differences only*

 * *Files 21% similar despite different names*

```diff
@@ -1,43 +1,43 @@
-# -*- coding: utf-8 -*-
-
-"""
-@author: 阿辉
-@contact: QQ:2655399832
-@Created on: 2022/9/21 16:30
-@Remark:
-"""
-
-import time
-
-from django_celery_results.models import TaskResult
-import django_filters
-
-from dvadmin.utils.serializers import CustomModelSerializer
-from dvadmin.utils.viewset import CustomModelViewSet
-
-
-
-
-class CeleryTaskDetailSerializer(CustomModelSerializer):
-    """定时任务详情 序列化器"""
-    class Meta:
-        model = TaskResult
-        fields = '__all__'
-
-
-class CeleryTaskDetailFilterSet(django_filters.FilterSet):
-    date_created = django_filters.BaseRangeFilter(field_name="date_created")
-    class Meta:
-        model = TaskResult
-        fields = ['id', 'status', 'date_done', 'date_created', 'result', 'task_name']
-
-
-
-
-class CeleryTaskDetailViewSet(CustomModelViewSet):
-    """
-    定时任务
-    """
-    queryset = TaskResult.objects.all()
-    serializer_class = CeleryTaskDetailSerializer
-    filter_class = CeleryTaskDetailFilterSet
+# -*- coding: utf-8 -*-
+
+"""
+@author: 阿辉
+@contact: QQ:2655399832
+@Created on: 2022/9/21 16:30
+@Remark:
+"""
+
+import time
+
+from django_celery_results.models import TaskResult
+import django_filters
+
+from dvadmin.utils.serializers import CustomModelSerializer
+from dvadmin.utils.viewset import CustomModelViewSet
+
+
+
+
+class CeleryTaskDetailSerializer(CustomModelSerializer):
+    """定时任务详情 序列化器"""
+    class Meta:
+        model = TaskResult
+        fields = '__all__'
+
+
+class CeleryTaskDetailFilterSet(django_filters.FilterSet):
+    date_created = django_filters.BaseRangeFilter(field_name="date_created")
+    class Meta:
+        model = TaskResult
+        fields = ['id', 'status', 'date_done', 'date_created', 'result', 'task_name']
+
+
+
+
+class CeleryTaskDetailViewSet(CustomModelViewSet):
+    """
+    定时任务
+    """
+    queryset = TaskResult.objects.all()
+    serializer_class = CeleryTaskDetailSerializer
+    filter_class = CeleryTaskDetailFilterSet
```

### Comparing `dvadmin-celery-1.0.4/dvadmin_celery.egg-info/PKG-INFO` & `dvadmin-celery-1.0.5/dvadmin_celery.egg-info/PKG-INFO`

 * *Files 17% similar despite different names*

```diff
@@ -1,141 +1,141 @@
-Metadata-Version: 2.1
-Name: dvadmin-celery
-Version: 1.0.4
-Summary: 适用于 django-vue-admin 的celery异步插件
-Home-page: https://gitee.com/huge-dream/dvadmin-celery
-Author: DVAdmin
-Author-email: liqiang@django-vue-admin.com
-Classifier: Programming Language :: Python :: 3
-Classifier: License :: OSI Approved :: MIT License
-Classifier: Operating System :: OS Independent
-Requires-Python: >=3.7, <4
-Description-Content-Type: text/markdown
-License-File: LICENSE
-
-# dvadmin_celery
-
-#### 介绍
-dvadmin-celery 插件是集成 django-celery-beat、tenant-schemas-celery、django-redis、django-celery-results 的一个后端插件，
-安装可快速使用异步任务，包含在线添加任务、启停任务、查看任务记录等功能。<br>
-与之相对应的是 dvadmin-celery-web 前端插件
-
-## 安装包
-
-使用pip安装软件包：
-
-```python
-pip install dvadmin-celery
-```
-
-目录结构：<br>
-```
-dvadmin-celery
-|   dvdadmin_celery
-|   |   fixtures
-|   |   |   __init__.py
-|   |   |   init_menu.json
-|   |   |   initialize.py
-|   |   views
-|   |   |   __init__.py
-|   |   |   crontab_schedule.py
-|   |   |   interval_schedule.py
-|   |   |   periodic_task.py
-|   |   |   task.py
-|   |   |   task_detail.py
-|   |   __init__.py
-|   |   admin.py
-|   |   apps.py
-|   |   settings.py
-|   |   tasks.py
-|   |   urls.py
-|   setup.py
-```
-
-### 方式一: 一键导入注册配置
-在 application / settings.py 插件配置中下导入默认配置
-```python
-...
-from dvadmin_celery.settings import *
-```
-### 方式二: 手动配置
-在INSTALLED_APPS 中注册app（注意先后顺序）
-
-```python
-INSTALLED_APPS = [
-    ...
-    'django_celery_beat',
-    'django_celery_results',
-    'dvadmin_celery',
-]
-```
-
-在 application / urls.py 中注册url地址
-
-```python
-urlpatterns = [
-    ...
-    path(r'api/dvadmin_celery/', include('dvadmin_celery.urls')),
-]
-```
-
-如果没有系统redis，请启动redis并添加配置 (./conf/env.example.py 及 ./conf/env.py中添加如下配置)
-
-```python
-# redis 配置
-REDIS_PASSWORD = '' # 如果没密码就为空
-REDIS_HOST = '127.0.0.1'
-REDIS_URL = f'redis://:{REDIS_PASSWORD or ""}@{REDIS_HOST}:6379'
-
-```
-
-在 application / settings.py 下添加配置
-
-```python
-...
-CACHES = { # 配置缓存
-    "default": {
-        "BACKEND": "django_redis.cache.RedisCache",
-        "LOCATION": f'{REDIS_URL}/1', # 库名可自选1~16
-        "OPTIONS": {
-            "CLIENT_CLASS": "django_redis.client.DefaultClient",
-        }
-    },
-}
-BROKER_URL = f'{REDIS_URL}/2' # 库名可自选1~16
-CELERY_RESULT_BACKEND = 'django-db' # celery结果存储到数据库中
-CELERYBEAT_SCHEDULER = 'django_celery_beat.schedulers.DatabaseScheduler'  # Backend数据库
-```
-
-进行迁移及初始化
-```python
-python3 manage.py makemigrations 
-python3 manage.py migrate 
-# 注意备份初始化信息
-python3 manage.py init -y 
-```
-
-其他配置请参考 django_celery_beat 和 celery 文档
-
-#### 使用说明
-
-``` python
-mac/linux:
-celery -A application.celery worker -B --loglevel=info
-
-win:
-需要安装: pip install eventlet,需要启动两个程序（worker + beat 顺序不分先后）
-celery -A application.celery worker -P eventlet --loglevel=info
-celery -A application.celery beat --loglevel=info
-```
-
-#### 注意
-``` python
-如果 celery worker 报错 KeyError,可尝试在django_vue_admin/application/celery.py文件里将
-app = Celery(f"application")
-改为
-app = Celery(f"application", include=['dvadmin_celery.tasks'])
-再重启尝试
-```
-redis下载地址：<br>
-Mac/Linux下载 http://download.redis.io/releases/ <br>
-Windows下载 https://github.com/tporadowski/redis/releases/ <br>
+Metadata-Version: 2.1
+Name: dvadmin-celery
+Version: 1.0.5
+Summary: 适用于 django-vue-admin 的celery异步插件
+Home-page: https://gitee.com/huge-dream/dvadmin-celery
+Author: DVAdmin
+Author-email: liqiang@django-vue-admin.com
+Classifier: Programming Language :: Python :: 3
+Classifier: License :: OSI Approved :: MIT License
+Classifier: Operating System :: OS Independent
+Requires-Python: >=3.7, <4
+Description-Content-Type: text/markdown
+License-File: LICENSE
+
+# dvadmin_celery
+
+#### 介绍
+dvadmin-celery 插件是集成 django-celery-beat、tenant-schemas-celery、django-redis、django-celery-results 的一个后端插件，
+安装可快速使用异步任务，包含在线添加任务、启停任务、查看任务记录等功能。<br>
+与之相对应的是 dvadmin-celery-web 前端插件
+
+## 安装包
+
+使用pip安装软件包：
+
+```python
+pip install dvadmin-celery
+```
+
+目录结构：<br>
+```
+dvadmin-celery
+|   dvdadmin_celery
+|   |   fixtures
+|   |   |   __init__.py
+|   |   |   init_menu.json
+|   |   |   initialize.py
+|   |   views
+|   |   |   __init__.py
+|   |   |   crontab_schedule.py
+|   |   |   interval_schedule.py
+|   |   |   periodic_task.py
+|   |   |   task.py
+|   |   |   task_detail.py
+|   |   __init__.py
+|   |   admin.py
+|   |   apps.py
+|   |   settings.py
+|   |   tasks.py
+|   |   urls.py
+|   setup.py
+```
+
+### 方式一: 一键导入注册配置
+在 application / settings.py 插件配置中下导入默认配置
+```python
+...
+from dvadmin_celery.settings import *
+```
+### 方式二: 手动配置
+在INSTALLED_APPS 中注册app（注意先后顺序）
+
+```python
+INSTALLED_APPS = [
+    ...
+    'django_celery_beat',
+    'django_celery_results',
+    'dvadmin_celery',
+]
+```
+
+在 application / urls.py 中注册url地址
+
+```python
+urlpatterns = [
+    ...
+    path(r'api/dvadmin_celery/', include('dvadmin_celery.urls')),
+]
+```
+
+如果没有系统redis，请启动redis并添加配置 (./conf/env.example.py 及 ./conf/env.py中添加如下配置)
+
+```python
+# redis 配置
+REDIS_PASSWORD = '' # 如果没密码就为空
+REDIS_HOST = '127.0.0.1'
+REDIS_URL = f'redis://:{REDIS_PASSWORD or ""}@{REDIS_HOST}:6379'
+
+```
+
+在 application / settings.py 下添加配置
+
+```python
+...
+CACHES = { # 配置缓存
+    "default": {
+        "BACKEND": "django_redis.cache.RedisCache",
+        "LOCATION": f'{REDIS_URL}/1', # 库名可自选1~16
+        "OPTIONS": {
+            "CLIENT_CLASS": "django_redis.client.DefaultClient",
+        }
+    },
+}
+BROKER_URL = f'{REDIS_URL}/2' # 库名可自选1~16
+CELERY_RESULT_BACKEND = 'django-db' # celery结果存储到数据库中
+CELERYBEAT_SCHEDULER = 'django_celery_beat.schedulers.DatabaseScheduler'  # Backend数据库
+```
+
+进行迁移及初始化
+```python
+python3 manage.py makemigrations 
+python3 manage.py migrate 
+# 注意备份初始化信息
+python3 manage.py init -y 
+```
+
+其他配置请参考 django_celery_beat 和 celery 文档
+
+#### 使用说明
+
+``` python
+mac/linux:
+celery -A application.celery worker -B --loglevel=info
+
+win:
+需要安装: pip install eventlet,需要启动两个程序（worker + beat 顺序不分先后）
+celery -A application.celery worker -P eventlet --loglevel=info
+celery -A application.celery beat --loglevel=info
+```
+
+#### 注意
+``` python
+如果 celery worker 报错 KeyError,可尝试在django_vue_admin/application/celery.py文件里将
+app = Celery(f"application")
+改为
+app = Celery(f"application", include=['dvadmin_celery.tasks'])
+再重启尝试
+```
+redis下载地址：<br>
+Mac/Linux下载 http://download.redis.io/releases/ <br>
+Windows下载 https://github.com/tporadowski/redis/releases/ <br>
```

### Comparing `dvadmin-celery-1.0.4/dvadmin_celery.egg-info/SOURCES.txt` & `dvadmin-celery-1.0.5/dvadmin_celery.egg-info/SOURCES.txt`

 * *Files 8% similar despite different names*

```diff
@@ -1,12 +1,13 @@
 LICENSE
 MANIFEST.in
 README.md
 pyproject.toml
 setup.py
+./dvadmin_celery/fixtures/init_menu.json
 dvadmin_celery/__init__.py
 dvadmin_celery/admin.py
 dvadmin_celery/apps.py
 dvadmin_celery/settings.py
 dvadmin_celery/tasks.py
 dvadmin_celery/urls.py
 dvadmin_celery.egg-info/PKG-INFO
```

### Comparing `dvadmin-celery-1.0.4/setup.py` & `dvadmin-celery-1.0.5/setup.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,34 +1,29 @@
-import setuptools
-
-with open("README.md", "r", encoding='utf-8') as fh:
-    long_description = fh.read()
-
-setuptools.setup(
-    name="dvadmin-celery",
-    version="1.0.4",
-    author="DVAdmin",
-    author_email="liqiang@django-vue-admin.com",
-    description="适用于 django-vue-admin 的celery异步插件",
-    long_description=long_description,
-    long_description_content_type="text/markdown",
-    url="https://gitee.com/huge-dream/dvadmin-celery",
-    packages=setuptools.find_packages(),
-    python_requires='>=3.7, <4',
-    install_requires=["django-celery-beat>=2.2.1",
-                      "tenant-schemas-celery>=1.0.1",
-                      "django-redis>=5.0.0",
-                      "django-celery-results>=2.2.0"],
-    classifiers=[
-        "Programming Language :: Python :: 3",
-        "License :: OSI Approved :: MIT License",
-        "Operating System :: OS Independent",
-    ],
-    # data_files=[
-    #     ('', ['./dvadmin_celery/fixtures/init_menu.json']),
-    # ],
-    packace_data={
-        '': ['*.json'],
-        'fixtures': ['*.json'],
-    },
-    include_package_data=True,
-)
+import setuptools
+
+with open("README.md", "r", encoding='utf-8') as fh:
+    long_description = fh.read()
+
+setuptools.setup(
+    name="dvadmin-celery",
+    version="1.0.5",
+    author="DVAdmin",
+    author_email="liqiang@django-vue-admin.com",
+    description="适用于 django-vue-admin 的celery异步插件",
+    long_description=long_description,
+    long_description_content_type="text/markdown",
+    url="https://gitee.com/huge-dream/dvadmin-celery",
+    packages=setuptools.find_packages(),
+    python_requires='>=3.7, <4',
+    install_requires=["django-celery-beat>=2.5.0",
+                      "tenant-schemas-celery>=2.2.0",
+                      "django-redis>=5.2.0",
+                      "django-celery-results>=2.5.1"],
+    classifiers=[
+        "Programming Language :: Python :: 3",
+        "License :: OSI Approved :: MIT License",
+        "Operating System :: OS Independent",
+    ],
+    data_files=[
+        ('', ['./dvadmin_celery/fixtures/init_menu.json']),
+    ]
+)
```

