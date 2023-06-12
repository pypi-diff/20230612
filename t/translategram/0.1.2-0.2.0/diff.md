# Comparing `tmp/translategram-0.1.2.tar.gz` & `tmp/translategram-0.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "translategram-0.1.2.tar", last modified: Sun Jun  4 16:06:14 2023, max compression
+gzip compressed data, was "translategram-0.2.0.tar", last modified: Mon Jun 12 15:54:32 2023, max compression
```

## Comparing `translategram-0.1.2.tar` & `translategram-0.2.0.tar`

### file list

```diff
@@ -1,23 +1,24 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-04 16:06:14.294062 translategram-0.1.2/
--rw-r--r--   0 runner    (1001) docker     (123)     1069 2023-06-04 16:06:04.000000 translategram-0.1.2/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)       26 2023-06-04 16:06:04.000000 translategram-0.1.2/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     4158 2023-06-04 16:06:14.290062 translategram-0.1.2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     3351 2023-06-04 16:06:04.000000 translategram-0.1.2/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-04 16:06:14.290062 translategram-0.1.2/auto_translategram/
--rw-r--r--   0 runner    (1001) docker     (123)      188 2023-06-04 16:06:04.000000 translategram-0.1.2/auto_translategram/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-04 16:06:14.290062 translategram-0.1.2/auto_translategram/auto_translategram/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-04 16:06:04.000000 translategram-0.1.2/auto_translategram/auto_translategram/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)       69 2023-06-04 16:06:04.000000 translategram-0.1.2/auto_translategram/auto_translategram/service_libs.py
--rw-r--r--   0 runner    (1001) docker     (123)     1220 2023-06-04 16:06:04.000000 translategram-0.1.2/auto_translategram/auto_translategram/translator.py
--rw-r--r--   0 runner    (1001) docker     (123)     1283 2023-06-04 16:06:04.000000 translategram-0.1.2/auto_translategram/auto_translategram/translator_services.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-04 16:06:14.290062 translategram-0.1.2/auto_translategram/python_telegram_bot_translator/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-04 16:06:04.000000 translategram-0.1.2/auto_translategram/python_telegram_bot_translator/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2973 2023-06-04 16:06:04.000000 translategram-0.1.2/auto_translategram/python_telegram_bot_translator/adapter.py
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-04 16:06:14.294062 translategram-0.1.2/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1170 2023-06-04 16:06:04.000000 translategram-0.1.2/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-04 16:06:14.290062 translategram-0.1.2/translategram.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     4158 2023-06-04 16:06:14.000000 translategram-0.1.2/translategram.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      593 2023-06-04 16:06:14.000000 translategram-0.1.2/translategram.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-04 16:06:14.000000 translategram-0.1.2/translategram.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       11 2023-06-04 16:06:14.000000 translategram-0.1.2/translategram.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       19 2023-06-04 16:06:14.000000 translategram-0.1.2/translategram.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-12 15:54:32.959290 translategram-0.2.0/
+-rw-r--r--   0 runner    (1001) docker     (123)     1069 2023-06-12 15:54:23.000000 translategram-0.2.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)       26 2023-06-12 15:54:23.000000 translategram-0.2.0/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     4129 2023-06-12 15:54:32.959290 translategram-0.2.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     3299 2023-06-12 15:54:23.000000 translategram-0.2.0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-12 15:54:32.959290 translategram-0.2.0/auto_translategram/
+-rw-r--r--   0 runner    (1001) docker     (123)      292 2023-06-12 15:54:23.000000 translategram-0.2.0/auto_translategram/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-12 15:54:32.959290 translategram-0.2.0/auto_translategram/auto_translategram/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-12 15:54:23.000000 translategram-0.2.0/auto_translategram/auto_translategram/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      943 2023-06-12 15:54:23.000000 translategram-0.2.0/auto_translategram/auto_translategram/cache.py
+-rw-r--r--   0 runner    (1001) docker     (123)       69 2023-06-12 15:54:23.000000 translategram-0.2.0/auto_translategram/auto_translategram/service_libs.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1380 2023-06-12 15:54:23.000000 translategram-0.2.0/auto_translategram/auto_translategram/translator.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1320 2023-06-12 15:54:23.000000 translategram-0.2.0/auto_translategram/auto_translategram/translator_services.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-12 15:54:32.959290 translategram-0.2.0/auto_translategram/python_telegram_bot_translator/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-12 15:54:23.000000 translategram-0.2.0/auto_translategram/python_telegram_bot_translator/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4080 2023-06-12 15:54:23.000000 translategram-0.2.0/auto_translategram/python_telegram_bot_translator/adapter.py
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-12 15:54:32.959290 translategram-0.2.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1194 2023-06-12 15:54:23.000000 translategram-0.2.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-12 15:54:32.959290 translategram-0.2.0/translategram.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     4129 2023-06-12 15:54:32.000000 translategram-0.2.0/translategram.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      640 2023-06-12 15:54:32.000000 translategram-0.2.0/translategram.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-12 15:54:32.000000 translategram-0.2.0/translategram.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       11 2023-06-12 15:54:32.000000 translategram-0.2.0/translategram.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       19 2023-06-12 15:54:32.000000 translategram-0.2.0/translategram.egg-info/top_level.txt
```

### Comparing `translategram-0.1.2/LICENSE` & `translategram-0.2.0/LICENSE`

 * *Files identical despite different names*

### Comparing `translategram-0.1.2/PKG-INFO` & `translategram-0.2.0/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: translategram
-Version: 0.1.2
-Summary: Python library for translating messages are sent by Bot in Telegram
+Version: 0.2.0
+Summary: Translategram is a Python library for translating messages are sent by your Bot in Telegram
 Home-page: https://github.com/EkberHasanov/translategram
 Author: Akbar
 Author-email: hasanvakbar@gmail.com
 License: MIT
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
@@ -31,24 +31,25 @@
 pip install translategram
 ```
 
 ## Usage
 
 ### First you need to add a parameter to your handler called whatever you want *(in this example we called it ```message```)* and its type should be the ```string```.
 ```python
+@translator.handler_translator(message="Welcome to out community!")
 async def login(update: Update, context: ContextTypes.DEFAULT_TYPE, message: str) -> None:
     await context.bot.send_message(
             chat_id=update.effective_chat.id if update.effective_chat else 0,
             text=message
             )
 ```
 
-### And then you need to call ```handler_translator``` method when you register your handler in handler class.
+### And then just register your handler in handler class.
 ```python
-login_handler = CommandHandler('login', translator.handler_translator(login, message="Welcome to our community!"))
+login_handler = CommandHandler('login', login)
 ```
 
 ### As well as you should create translator instance based on the framework you are using *(in this case python-telegram-bot)*.
 
 ```python
 from auto_translategram import PythonTelegramBotTranslator, MtranslateTranslatorService
 
@@ -69,32 +70,34 @@
     format='%(asctime)s - %(name)s - %(levelname)s - %(message)s',
     level=logging.INFO
 )
 
 logger = logging.getLogger(__name__)
 
 
+@translator.handler_translator(message="Welcome to out community!")
 async def login(update: Update, context: ContextTypes.DEFAULT_TYPE, message: str) -> None:
     await context.bot.send_message(
             chat_id=update.effective_chat.id if update.effective_chat else 0,
             text=message
             )
 
 
+@translator.handler_translator(message="This bot is very simple. You can just login with the /login command and that is it!")
 async def start(update: Update, context: ContextTypes.DEFAULT_TYPE, message: str) -> None:
     await context.bot.send_message(
             chat_id=update.effective_chat.id if update.effective_chat else 0,
             text=message
             )
 
 if __name__ == '__main__':
     application = ApplicationBuilder().token(TOKEN).build()
 
-    login_handler = CommandHandler('login', translator.handler_translator(login, message="Welcome to our community!"))
-    start_handler = CommandHandler('start', translator.handler_translator(start, message="This bot is very simple. You can just login with the /login command and that is it!"))
+    login_handler = CommandHandler('login', login)
+    start_handler = CommandHandler('start', start)
     application.add_handler(login_handler)
     application.add_handler(start_handler)
 
     application.run_polling()
 
 ```
```

### Comparing `translategram-0.1.2/README.md` & `translategram-0.2.0/README.md`

 * *Files 12% similar despite different names*

```diff
@@ -10,24 +10,25 @@
 pip install translategram
 ```
 
 ## Usage
 
 ### First you need to add a parameter to your handler called whatever you want *(in this example we called it ```message```)* and its type should be the ```string```.
 ```python
+@translator.handler_translator(message="Welcome to out community!")
 async def login(update: Update, context: ContextTypes.DEFAULT_TYPE, message: str) -> None:
     await context.bot.send_message(
             chat_id=update.effective_chat.id if update.effective_chat else 0,
             text=message
             )
 ```
 
-### And then you need to call ```handler_translator``` method when you register your handler in handler class.
+### And then just register your handler in handler class.
 ```python
-login_handler = CommandHandler('login', translator.handler_translator(login, message="Welcome to our community!"))
+login_handler = CommandHandler('login', login)
 ```
 
 ### As well as you should create translator instance based on the framework you are using *(in this case python-telegram-bot)*.
 
 ```python
 from auto_translategram import PythonTelegramBotTranslator, MtranslateTranslatorService
 
@@ -48,32 +49,34 @@
     format='%(asctime)s - %(name)s - %(levelname)s - %(message)s',
     level=logging.INFO
 )
 
 logger = logging.getLogger(__name__)
 
 
+@translator.handler_translator(message="Welcome to out community!")
 async def login(update: Update, context: ContextTypes.DEFAULT_TYPE, message: str) -> None:
     await context.bot.send_message(
             chat_id=update.effective_chat.id if update.effective_chat else 0,
             text=message
             )
 
 
+@translator.handler_translator(message="This bot is very simple. You can just login with the /login command and that is it!")
 async def start(update: Update, context: ContextTypes.DEFAULT_TYPE, message: str) -> None:
     await context.bot.send_message(
             chat_id=update.effective_chat.id if update.effective_chat else 0,
             text=message
             )
 
 if __name__ == '__main__':
     application = ApplicationBuilder().token(TOKEN).build()
 
-    login_handler = CommandHandler('login', translator.handler_translator(login, message="Welcome to our community!"))
-    start_handler = CommandHandler('start', translator.handler_translator(start, message="This bot is very simple. You can just login with the /login command and that is it!"))
+    login_handler = CommandHandler('login', login)
+    start_handler = CommandHandler('start', start)
     application.add_handler(login_handler)
     application.add_handler(start_handler)
 
     application.run_polling()
 
 ```
 
@@ -88,8 +91,8 @@
 * Add aiogram framework adapter.
 * Add pyTelegramBotApi framework adapter.
 * Add support for more translation services.
 
 
 ## License
 
-This project is licensed under the terms of the MIT license.
+This project is licensed under the terms of the MIT license.
```

### Comparing `translategram-0.1.2/auto_translategram/auto_translategram/translator.py` & `translategram-0.2.0/auto_translategram/auto_translategram/translator.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,21 +1,23 @@
 from abc import ABC, abstractmethod
-from typing import Any, Callable, Coroutine, TypeVar
-from .translator_services import TranslatorService
+from typing import Any, Callable, Coroutine, Type, TypeVar, Union
+
+from auto_translategram.auto_translategram.cache import Cache
+from auto_translategram.auto_translategram.translator_services import TranslatorService
 
 T = TypeVar('T')
 
 
 class Translator(ABC):
     """
     Abstract base class for implementing translation functionality in various frameworks.
     This class provides a uniform interface for translation, allowing adapters to be written for different frameworks.
     This class is meant to be subclassed, and the `handler_translator` method should be implemented in the subclass.
     """
-    def __init__(self, translator_service: TranslatorService) -> None:
+    def __init__(self, translator_service: TranslatorService, cache_system: Union[Type[Cache], None] = None) -> None:
         """
         Initializes a new Translator instance using the specified `translator_service`.
 
         :param translator_service: The `BaseTranslatorService` to use for translations.
         """
         ...
```

### Comparing `translategram-0.1.2/auto_translategram/auto_translategram/translator_services.py` & `translategram-0.2.0/auto_translategram/auto_translategram/translator_services.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 from typing import Protocol
-from .service_libs import mtranslate
+from auto_translategram.auto_translategram.service_libs import mtranslate
 
 
 class TranslatorService(Protocol):
     """
     Defines the interface for the translator services
     """
     async def translate_str(self, text: str, target_language: str = 'auto', source_language: str = 'auto') -> str:
```

### Comparing `translategram-0.1.2/setup.py` & `translategram-0.2.0/setup.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,16 +1,16 @@
 from setuptools import setup, find_packages
 
 with open("README.md", "r", encoding='utf-8') as f:
     long_description = f.read()
 
 setup(
     name='translategram',
-    version='0.1.2',
-    description='Python library for translating messages are sent by Bot in Telegram',
+    version='0.2.0',
+    description='Translategram is a Python library for translating messages are sent by your Bot in Telegram',
     url='https://github.com/EkberHasanov/translategram',
     author='Akbar',
     author_email='hasanvakbar@gmail.com',
     license='MIT',
     install_requires=[
         'mtranslate',
     ],
```

### Comparing `translategram-0.1.2/translategram.egg-info/PKG-INFO` & `translategram-0.2.0/translategram.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: translategram
-Version: 0.1.2
-Summary: Python library for translating messages are sent by Bot in Telegram
+Version: 0.2.0
+Summary: Translategram is a Python library for translating messages are sent by your Bot in Telegram
 Home-page: https://github.com/EkberHasanov/translategram
 Author: Akbar
 Author-email: hasanvakbar@gmail.com
 License: MIT
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
@@ -31,24 +31,25 @@
 pip install translategram
 ```
 
 ## Usage
 
 ### First you need to add a parameter to your handler called whatever you want *(in this example we called it ```message```)* and its type should be the ```string```.
 ```python
+@translator.handler_translator(message="Welcome to out community!")
 async def login(update: Update, context: ContextTypes.DEFAULT_TYPE, message: str) -> None:
     await context.bot.send_message(
             chat_id=update.effective_chat.id if update.effective_chat else 0,
             text=message
             )
 ```
 
-### And then you need to call ```handler_translator``` method when you register your handler in handler class.
+### And then just register your handler in handler class.
 ```python
-login_handler = CommandHandler('login', translator.handler_translator(login, message="Welcome to our community!"))
+login_handler = CommandHandler('login', login)
 ```
 
 ### As well as you should create translator instance based on the framework you are using *(in this case python-telegram-bot)*.
 
 ```python
 from auto_translategram import PythonTelegramBotTranslator, MtranslateTranslatorService
 
@@ -69,32 +70,34 @@
     format='%(asctime)s - %(name)s - %(levelname)s - %(message)s',
     level=logging.INFO
 )
 
 logger = logging.getLogger(__name__)
 
 
+@translator.handler_translator(message="Welcome to out community!")
 async def login(update: Update, context: ContextTypes.DEFAULT_TYPE, message: str) -> None:
     await context.bot.send_message(
             chat_id=update.effective_chat.id if update.effective_chat else 0,
             text=message
             )
 
 
+@translator.handler_translator(message="This bot is very simple. You can just login with the /login command and that is it!")
 async def start(update: Update, context: ContextTypes.DEFAULT_TYPE, message: str) -> None:
     await context.bot.send_message(
             chat_id=update.effective_chat.id if update.effective_chat else 0,
             text=message
             )
 
 if __name__ == '__main__':
     application = ApplicationBuilder().token(TOKEN).build()
 
-    login_handler = CommandHandler('login', translator.handler_translator(login, message="Welcome to our community!"))
-    start_handler = CommandHandler('start', translator.handler_translator(start, message="This bot is very simple. You can just login with the /login command and that is it!"))
+    login_handler = CommandHandler('login', login)
+    start_handler = CommandHandler('start', start)
     application.add_handler(login_handler)
     application.add_handler(start_handler)
 
     application.run_polling()
 
 ```
```

### Comparing `translategram-0.1.2/translategram.egg-info/SOURCES.txt` & `translategram-0.2.0/translategram.egg-info/SOURCES.txt`

 * *Files 12% similar despite different names*

```diff
@@ -1,13 +1,14 @@
 LICENSE
 MANIFEST.in
 README.md
 setup.py
 auto_translategram/__init__.py
 auto_translategram/auto_translategram/__init__.py
+auto_translategram/auto_translategram/cache.py
 auto_translategram/auto_translategram/service_libs.py
 auto_translategram/auto_translategram/translator.py
 auto_translategram/auto_translategram/translator_services.py
 auto_translategram/python_telegram_bot_translator/__init__.py
 auto_translategram/python_telegram_bot_translator/adapter.py
 translategram.egg-info/PKG-INFO
 translategram.egg-info/SOURCES.txt
```

