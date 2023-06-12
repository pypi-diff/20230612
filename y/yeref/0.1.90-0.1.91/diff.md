# Comparing `tmp/yeref-0.1.90.tar.gz` & `tmp/yeref-0.1.91.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "yeref-0.1.90.tar", last modified: Mon Jun 12 11:55:24 2023, max compression
+gzip compressed data, was "yeref-0.1.91.tar", last modified: Mon Jun 12 16:04:32 2023, max compression
```

## Comparing `yeref-0.1.90.tar` & `yeref-0.1.91.tar`

### file list

```diff
@@ -1,13 +1,13 @@
-drwxr-xr-x   0 mark       (501) staff       (20)        0 2023-06-12 11:55:24.148914 yeref-0.1.90/
--rw-r--r--   0 mark       (501) staff       (20)       85 2023-06-12 11:55:24.149176 yeref-0.1.90/PKG-INFO
--rw-r--r--   0 mark       (501) staff       (20)       38 2023-06-12 11:55:24.150263 yeref-0.1.90/setup.cfg
--rw-r--r--   0 mark       (501) staff       (20)     1391 2023-06-12 11:55:02.000000 yeref-0.1.90/setup.py
-drwxr-xr-x   0 mark       (501) staff       (20)        0 2023-06-12 11:55:24.145353 yeref-0.1.90/yeref/
--rw-r--r--   0 mark       (501) staff       (20)       39 2023-04-21 17:52:00.000000 yeref-0.1.90/yeref/__init__.py
--rw-r--r--   0 mark       (501) staff       (20)   553500 2023-06-11 15:47:28.000000 yeref-0.1.90/yeref/l_.py
--rw-r--r--   0 mark       (501) staff       (20)   213869 2023-06-12 11:47:33.000000 yeref-0.1.90/yeref/yeref.py
-drwxr-xr-x   0 mark       (501) staff       (20)        0 2023-06-12 11:55:24.148488 yeref-0.1.90/yeref.egg-info/
--rw-r--r--   0 mark       (501) staff       (20)       85 2023-06-12 11:55:24.000000 yeref-0.1.90/yeref.egg-info/PKG-INFO
--rw-r--r--   0 mark       (501) staff       (20)      179 2023-06-12 11:55:24.000000 yeref-0.1.90/yeref.egg-info/SOURCES.txt
--rw-r--r--   0 mark       (501) staff       (20)        1 2023-06-12 11:55:24.000000 yeref-0.1.90/yeref.egg-info/dependency_links.txt
--rw-r--r--   0 mark       (501) staff       (20)        6 2023-06-12 11:55:24.000000 yeref-0.1.90/yeref.egg-info/top_level.txt
+drwxr-xr-x   0 mark       (501) staff       (20)        0 2023-06-12 16:04:32.294782 yeref-0.1.91/
+-rw-r--r--   0 mark       (501) staff       (20)       85 2023-06-12 16:04:32.294961 yeref-0.1.91/PKG-INFO
+-rw-r--r--   0 mark       (501) staff       (20)       38 2023-06-12 16:04:32.297278 yeref-0.1.91/setup.cfg
+-rw-r--r--   0 mark       (501) staff       (20)     1391 2023-06-12 16:04:17.000000 yeref-0.1.91/setup.py
+drwxr-xr-x   0 mark       (501) staff       (20)        0 2023-06-12 16:04:32.286559 yeref-0.1.91/yeref/
+-rw-r--r--   0 mark       (501) staff       (20)       39 2023-04-21 17:52:00.000000 yeref-0.1.91/yeref/__init__.py
+-rw-r--r--   0 mark       (501) staff       (20)   554470 2023-06-12 16:04:06.000000 yeref-0.1.91/yeref/l_.py
+-rw-r--r--   0 mark       (501) staff       (20)   213869 2023-06-12 11:47:33.000000 yeref-0.1.91/yeref/yeref.py
+drwxr-xr-x   0 mark       (501) staff       (20)        0 2023-06-12 16:04:32.294177 yeref-0.1.91/yeref.egg-info/
+-rw-r--r--   0 mark       (501) staff       (20)       85 2023-06-12 16:04:32.000000 yeref-0.1.91/yeref.egg-info/PKG-INFO
+-rw-r--r--   0 mark       (501) staff       (20)      179 2023-06-12 16:04:32.000000 yeref-0.1.91/yeref.egg-info/SOURCES.txt
+-rw-r--r--   0 mark       (501) staff       (20)        1 2023-06-12 16:04:32.000000 yeref-0.1.91/yeref.egg-info/dependency_links.txt
+-rw-r--r--   0 mark       (501) staff       (20)        6 2023-06-12 16:04:32.000000 yeref-0.1.91/yeref.egg-info/top_level.txt
```

### Comparing `yeref-0.1.90/setup.py` & `yeref-0.1.91/setup.py`

 * *Files 17% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from setuptools import setup
 
 setup(
       name='yeref',
-      version='0.1.90',
+      version='0.1.91',
       description='desc-f',
       author='john smith',
       packages=['yeref'],
       # install_requires=[
       #       "httplib2>=0.20.4",
       #       "moviepy>=1.0.3",
       #       "Pillow>=9.2.0",
```

### Comparing `yeref-0.1.90/yeref/l_.py` & `yeref-0.1.91/yeref/l_.py`

 * *Files 0% similar despite different names*

```diff
@@ -198,14 +198,23 @@
     'ru': "👩🏽‍💻 Текущий /balance {0}{1}",
     'en': "👩🏽‍💻 Current /balance {0}{1}",
     'es': "¹ All bots & projects",
     'fr': "¹ All bots & projects",
     'zh': "¹ All bots & projects",
     'ar': "¹ All bots & projects",
 }
+l_subscribe_deposit = {
+    'ru': "² Донат на баланс",
+    'en': "² Donate to balance",
+    'es': "👩🏽‍💻 <b>Regístrese para obtener</b> una\n\n¹ <i>suscripción</i> mensual a @{0}-bot [{1} ₽]\n▪️ sin anuncios\n▪️ tareas creativas\n² Suscríbase a <u>todos</u> los bots [{2} ₽]",
+    'fr': "👩🏽‍💻 <b>Inscrivez-vous pour</b> un <i>abonnement</i>\n\n¹ mensuel à @{0}-bot [{1} ₽]\n▪️ pas de publicité\n▪️ tâches créatives\n² Abonnez-vous à <u>tous</u> les bots [{2} ₽]",
+    'zh': "👩🏽‍💻<b>注册</b>每月\n\n¹<i>订阅</i>@{0}-bot [{1} ₽]\n▪️ 无广告\n▪️ 创意任务\n² 订阅<u>所有</u>机器人 [{2} ₽]",
+    'ar': "👩🏽‍💻 <b>اشترك للحصول على</b> <i>اشتراك</i> شهري\n\n¹ في @ {0} -bot [{1} ₽]\n▪️ بلا إعلانات\n▪️ مهام إبداعية\n² اشترك في <u>جميع</u> برامج التتبُّع [{2} ₽]",
+}
+
 l_language_get = {
     'ru': "🌏 <b>Выбери</b> один из доступных языков",
     'en': "🌏 <b>Choose</b> one of the available languages",
     'es': "🌏 <b>Elige</b> uno de los idiomas disponibles",
     'fr': "🌏 <b>Choisissez</b> l'une des langues disponibles",
     'zh': "🌏<b>选择</b>一种可用的语言",
     'ar': "🌏 <b>اختر</b> إحدى اللغات المتاحة",
```

### Comparing `yeref-0.1.90/yeref/yeref.py` & `yeref-0.1.91/yeref/yeref.py`

 * *Files identical despite different names*

