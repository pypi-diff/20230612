# Comparing `tmp/pymino-1.1.9.2.tar.gz` & `tmp/pymino-1.1.9.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "C:\Users\12095\Desktop\New folder (4)\dist\.tmp-vaxzuj92\pymino-1.1.9.2.tar", last modified: Sun Jun 11 21:53:28 2023, max compression
+gzip compressed data, was "C:\Users\12095\Desktop\New folder (4)\dist\.tmp-ctik5qfd\pymino-1.1.9.3.tar", last modified: Sun Jun 11 22:23:04 2023, max compression
```

## Comparing `pymino-1.1.9.2.tar` & `pymino-1.1.9.3.tar`

### file list

```diff
@@ -1,54 +1,54 @@
-drwxrwxrwx   0        0        0        0 2023-06-11 21:53:28.492042 pymino-1.1.9.2/
--rw-rw-rw-   0        0        0     1085 2023-02-11 18:40:37.000000 pymino-1.1.9.2/LICENSE
--rw-rw-rw-   0        0        0     6082 2023-06-11 21:53:28.492538 pymino-1.1.9.2/PKG-INFO
--rw-rw-rw-   0        0        0     5364 2023-03-09 02:27:22.000000 pymino-1.1.9.2/README.md
-drwxrwxrwx   0        0        0        0 2023-06-11 21:53:28.427067 pymino-1.1.9.2/pymino/
--rw-rw-rw-   0        0        0      721 2023-06-11 21:52:23.000000 pymino-1.1.9.2/pymino/__init__.py
--rw-rw-rw-   0        0        0     7986 2023-06-11 13:46:02.000000 pymino-1.1.9.2/pymino/async_bot.py
--rw-rw-rw-   0        0        0    30128 2023-06-11 20:06:18.000000 pymino-1.1.9.2/pymino/bot.py
--rw-rw-rw-   0        0        0    52021 2023-06-08 12:36:59.000000 pymino-1.1.9.2/pymino/client.py
-drwxrwxrwx   0        0        0        0 2023-06-11 21:53:28.461292 pymino-1.1.9.2/pymino/ext/
--rw-rw-rw-   0        0        0      498 2023-06-11 16:50:39.000000 pymino-1.1.9.2/pymino/ext/__init__.py
--rw-rw-rw-   0        0        0    13871 2023-06-08 12:06:58.000000 pymino-1.1.9.2/pymino/ext/account.py
--rw-rw-rw-   0        0        0   287511 2023-06-08 12:33:03.000000 pymino-1.1.9.2/pymino/ext/async_community.py
--rw-rw-rw-   0        0        0    18079 2023-06-10 00:59:39.000000 pymino-1.1.9.2/pymino/ext/async_context.py
--rw-rw-rw-   0        0        0    23958 2023-06-11 13:57:44.000000 pymino-1.1.9.2/pymino/ext/async_event_handler.py
--rw-rw-rw-   0        0        0     7238 2023-06-11 14:03:00.000000 pymino-1.1.9.2/pymino/ext/async_socket.py
--rw-rw-rw-   0        0        0   292004 2023-06-11 18:06:25.000000 pymino-1.1.9.2/pymino/ext/community.py
--rw-rw-rw-   0        0        0     2428 2023-06-11 21:49:55.000000 pymino-1.1.9.2/pymino/ext/console.py
--rw-rw-rw-   0        0        0    41963 2023-06-11 20:52:12.000000 pymino-1.1.9.2/pymino/ext/context.py
--rw-rw-rw-   0        0        0     1758 2023-05-28 22:00:16.000000 pymino-1.1.9.2/pymino/ext/dispatcher.py
-drwxrwxrwx   0        0        0        0 2023-06-11 21:53:28.479642 pymino-1.1.9.2/pymino/ext/entities/
--rw-rw-rw-   0        0        0      312 2023-06-08 07:25:34.000000 pymino-1.1.9.2/pymino/ext/entities/__init__.py
--rw-rw-rw-   0        0        0     1670 2023-06-08 12:22:47.000000 pymino-1.1.9.2/pymino/ext/entities/api_response.py
--rw-rw-rw-   0        0        0    20323 2023-06-08 12:02:08.000000 pymino-1.1.9.2/pymino/ext/entities/chat_threads.py
--rw-rw-rw-   0        0        0    13223 2023-06-08 11:59:16.000000 pymino-1.1.9.2/pymino/ext/entities/comments.py
--rw-rw-rw-   0        0        0      765 2023-03-05 16:56:17.000000 pymino-1.1.9.2/pymino/ext/entities/enums.py
--rw-rw-rw-   0        0        0    16021 2023-06-10 00:36:20.000000 pymino-1.1.9.2/pymino/ext/entities/exceptions.py
--rw-rw-rw-   0        0        0    43596 2023-06-08 08:03:53.000000 pymino-1.1.9.2/pymino/ext/entities/general.py
--rw-rw-rw-   0        0        0     4802 2023-06-11 21:21:53.000000 pymino-1.1.9.2/pymino/ext/entities/handlers.py
--rw-rw-rw-   0        0        0     5127 2023-06-08 08:11:36.000000 pymino-1.1.9.2/pymino/ext/entities/link_info.py
--rw-rw-rw-   0        0        0    42516 2023-06-08 07:28:10.000000 pymino-1.1.9.2/pymino/ext/entities/messages.py
--rw-rw-rw-   0        0        0     1847 2023-06-08 07:26:04.000000 pymino-1.1.9.2/pymino/ext/entities/notification.py
--rw-rw-rw-   0        0        0    31609 2023-02-13 01:22:30.000000 pymino-1.1.9.2/pymino/ext/entities/userprofile.py
--rw-rw-rw-   0        0        0     2451 2023-05-17 03:04:06.000000 pymino-1.1.9.2/pymino/ext/entities/wsevents.py
--rw-rw-rw-   0        0        0      543 2023-05-28 22:01:44.000000 pymino-1.1.9.2/pymino/ext/handle_queue.py
--rw-rw-rw-   0        0        0     6729 2023-06-11 14:02:47.000000 pymino-1.1.9.2/pymino/ext/socket.py
-drwxrwxrwx   0        0        0        0 2023-06-11 21:53:28.491050 pymino-1.1.9.2/pymino/ext/utilities/
--rw-rw-rw-   0        0        0      234 2023-06-11 17:31:29.000000 pymino-1.1.9.2/pymino/ext/utilities/__init__.py
--rw-rw-rw-   0        0        0    11320 2023-05-29 04:02:19.000000 pymino-1.1.9.2/pymino/ext/utilities/async_request_handler.py
--rw-rw-rw-   0        0        0     9324 2023-06-11 21:49:21.000000 pymino-1.1.9.2/pymino/ext/utilities/chat_console.py
--rw-rw-rw-   0        0        0     6396 2023-03-02 00:41:30.000000 pymino-1.1.9.2/pymino/ext/utilities/commands.py
--rw-rw-rw-   0        0        0     1917 2023-06-11 21:48:00.000000 pymino-1.1.9.2/pymino/ext/utilities/community_console.py
--rw-rw-rw-   0        0        0     1110 2023-02-28 16:10:43.000000 pymino-1.1.9.2/pymino/ext/utilities/generate.py
--rw-rw-rw-   0        0        0     2911 2023-06-11 21:47:35.000000 pymino-1.1.9.2/pymino/ext/utilities/menu.py
--rw-rw-rw-   0        0        0     1969 2023-06-11 21:49:47.000000 pymino-1.1.9.2/pymino/ext/utilities/profile_console.py
--rw-rw-rw-   0        0        0    10274 2023-06-08 12:27:04.000000 pymino-1.1.9.2/pymino/ext/utilities/request_handler.py
-drwxrwxrwx   0        0        0        0 2023-06-11 21:53:28.441450 pymino-1.1.9.2/pymino.egg-info/
--rw-rw-rw-   0        0        0     6082 2023-06-11 21:53:28.000000 pymino-1.1.9.2/pymino.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0     1323 2023-06-11 21:53:28.000000 pymino-1.1.9.2/pymino.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-06-11 21:53:28.000000 pymino-1.1.9.2/pymino.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0      102 2023-06-11 21:53:28.000000 pymino-1.1.9.2/pymino.egg-info/requires.txt
--rw-rw-rw-   0        0        0        7 2023-06-11 21:53:28.000000 pymino-1.1.9.2/pymino.egg-info/top_level.txt
--rw-rw-rw-   0        0        0      873 2023-06-11 21:53:28.499977 pymino-1.1.9.2/setup.cfg
--rw-rw-rw-   0        0        0     1367 2023-05-29 00:20:50.000000 pymino-1.1.9.2/setup.py
+drwxrwxrwx   0        0        0        0 2023-06-11 22:23:04.685539 pymino-1.1.9.3/
+-rw-rw-rw-   0        0        0     1085 2023-02-11 18:40:37.000000 pymino-1.1.9.3/LICENSE
+-rw-rw-rw-   0        0        0     6082 2023-06-11 22:23:04.686034 pymino-1.1.9.3/PKG-INFO
+-rw-rw-rw-   0        0        0     5364 2023-03-09 02:27:22.000000 pymino-1.1.9.3/README.md
+drwxrwxrwx   0        0        0        0 2023-06-11 22:23:04.622051 pymino-1.1.9.3/pymino/
+-rw-rw-rw-   0        0        0      721 2023-06-11 22:22:36.000000 pymino-1.1.9.3/pymino/__init__.py
+-rw-rw-rw-   0        0        0     7986 2023-06-11 13:46:02.000000 pymino-1.1.9.3/pymino/async_bot.py
+-rw-rw-rw-   0        0        0    30128 2023-06-11 20:06:18.000000 pymino-1.1.9.3/pymino/bot.py
+-rw-rw-rw-   0        0        0    52021 2023-06-08 12:36:59.000000 pymino-1.1.9.3/pymino/client.py
+drwxrwxrwx   0        0        0        0 2023-06-11 22:23:04.654291 pymino-1.1.9.3/pymino/ext/
+-rw-rw-rw-   0        0        0      498 2023-06-11 16:50:39.000000 pymino-1.1.9.3/pymino/ext/__init__.py
+-rw-rw-rw-   0        0        0    13871 2023-06-08 12:06:58.000000 pymino-1.1.9.3/pymino/ext/account.py
+-rw-rw-rw-   0        0        0   287511 2023-06-08 12:33:03.000000 pymino-1.1.9.3/pymino/ext/async_community.py
+-rw-rw-rw-   0        0        0    18079 2023-06-10 00:59:39.000000 pymino-1.1.9.3/pymino/ext/async_context.py
+-rw-rw-rw-   0        0        0    23958 2023-06-11 13:57:44.000000 pymino-1.1.9.3/pymino/ext/async_event_handler.py
+-rw-rw-rw-   0        0        0     7238 2023-06-11 14:03:00.000000 pymino-1.1.9.3/pymino/ext/async_socket.py
+-rw-rw-rw-   0        0        0   292004 2023-06-11 18:06:25.000000 pymino-1.1.9.3/pymino/ext/community.py
+-rw-rw-rw-   0        0        0     3040 2023-06-11 22:20:09.000000 pymino-1.1.9.3/pymino/ext/console.py
+-rw-rw-rw-   0        0        0    41963 2023-06-11 20:52:12.000000 pymino-1.1.9.3/pymino/ext/context.py
+-rw-rw-rw-   0        0        0     1758 2023-05-28 22:00:16.000000 pymino-1.1.9.3/pymino/ext/dispatcher.py
+drwxrwxrwx   0        0        0        0 2023-06-11 22:23:04.673635 pymino-1.1.9.3/pymino/ext/entities/
+-rw-rw-rw-   0        0        0      312 2023-06-08 07:25:34.000000 pymino-1.1.9.3/pymino/ext/entities/__init__.py
+-rw-rw-rw-   0        0        0     1670 2023-06-08 12:22:47.000000 pymino-1.1.9.3/pymino/ext/entities/api_response.py
+-rw-rw-rw-   0        0        0    20323 2023-06-08 12:02:08.000000 pymino-1.1.9.3/pymino/ext/entities/chat_threads.py
+-rw-rw-rw-   0        0        0    13223 2023-06-08 11:59:16.000000 pymino-1.1.9.3/pymino/ext/entities/comments.py
+-rw-rw-rw-   0        0        0      765 2023-03-05 16:56:17.000000 pymino-1.1.9.3/pymino/ext/entities/enums.py
+-rw-rw-rw-   0        0        0    16021 2023-06-10 00:36:20.000000 pymino-1.1.9.3/pymino/ext/entities/exceptions.py
+-rw-rw-rw-   0        0        0    43596 2023-06-08 08:03:53.000000 pymino-1.1.9.3/pymino/ext/entities/general.py
+-rw-rw-rw-   0        0        0     4802 2023-06-11 21:21:53.000000 pymino-1.1.9.3/pymino/ext/entities/handlers.py
+-rw-rw-rw-   0        0        0     5127 2023-06-08 08:11:36.000000 pymino-1.1.9.3/pymino/ext/entities/link_info.py
+-rw-rw-rw-   0        0        0    42516 2023-06-08 07:28:10.000000 pymino-1.1.9.3/pymino/ext/entities/messages.py
+-rw-rw-rw-   0        0        0     1847 2023-06-08 07:26:04.000000 pymino-1.1.9.3/pymino/ext/entities/notification.py
+-rw-rw-rw-   0        0        0    31609 2023-02-13 01:22:30.000000 pymino-1.1.9.3/pymino/ext/entities/userprofile.py
+-rw-rw-rw-   0        0        0     2451 2023-05-17 03:04:06.000000 pymino-1.1.9.3/pymino/ext/entities/wsevents.py
+-rw-rw-rw-   0        0        0      543 2023-05-28 22:01:44.000000 pymino-1.1.9.3/pymino/ext/handle_queue.py
+-rw-rw-rw-   0        0        0     6729 2023-06-11 14:02:47.000000 pymino-1.1.9.3/pymino/ext/socket.py
+drwxrwxrwx   0        0        0        0 2023-06-11 22:23:04.684547 pymino-1.1.9.3/pymino/ext/utilities/
+-rw-rw-rw-   0        0        0      234 2023-06-11 17:31:29.000000 pymino-1.1.9.3/pymino/ext/utilities/__init__.py
+-rw-rw-rw-   0        0        0    11320 2023-05-29 04:02:19.000000 pymino-1.1.9.3/pymino/ext/utilities/async_request_handler.py
+-rw-rw-rw-   0        0        0     9580 2023-06-11 22:17:23.000000 pymino-1.1.9.3/pymino/ext/utilities/chat_console.py
+-rw-rw-rw-   0        0        0     6396 2023-03-02 00:41:30.000000 pymino-1.1.9.3/pymino/ext/utilities/commands.py
+-rw-rw-rw-   0        0        0     2078 2023-06-11 22:22:27.000000 pymino-1.1.9.3/pymino/ext/utilities/community_console.py
+-rw-rw-rw-   0        0        0     1110 2023-02-28 16:10:43.000000 pymino-1.1.9.3/pymino/ext/utilities/generate.py
+-rw-rw-rw-   0        0        0     2911 2023-06-11 21:47:35.000000 pymino-1.1.9.3/pymino/ext/utilities/menu.py
+-rw-rw-rw-   0        0        0     2106 2023-06-11 22:17:45.000000 pymino-1.1.9.3/pymino/ext/utilities/profile_console.py
+-rw-rw-rw-   0        0        0    10274 2023-06-08 12:27:04.000000 pymino-1.1.9.3/pymino/ext/utilities/request_handler.py
+drwxrwxrwx   0        0        0        0 2023-06-11 22:23:04.637922 pymino-1.1.9.3/pymino.egg-info/
+-rw-rw-rw-   0        0        0     6082 2023-06-11 22:23:04.000000 pymino-1.1.9.3/pymino.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0     1323 2023-06-11 22:23:04.000000 pymino-1.1.9.3/pymino.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-06-11 22:23:04.000000 pymino-1.1.9.3/pymino.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0      102 2023-06-11 22:23:04.000000 pymino-1.1.9.3/pymino.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        7 2023-06-11 22:23:04.000000 pymino-1.1.9.3/pymino.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0      873 2023-06-11 22:23:04.691987 pymino-1.1.9.3/setup.cfg
+-rw-rw-rw-   0        0        0     1367 2023-05-29 00:20:50.000000 pymino-1.1.9.3/setup.py
```

### Comparing `pymino-1.1.9.2/LICENSE` & `pymino-1.1.9.3/LICENSE`

 * *Files identical despite different names*

### Comparing `pymino-1.1.9.2/PKG-INFO` & `pymino-1.1.9.3/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pymino
-Version: 1.1.9.2
+Version: 1.1.9.3
 Summary: Easily create a bot for Amino Apps using a modern easy to use synchronous library.
 Home-page: https://github.com/forevercynical/pymino
 Author: forevercynical
 Author-email: me@cynical.gg
 License: MIT
 Keywords: amino,pymino,narvii,amino-api,narvii-bots,aminoapps,amino-bot,amino-bots
 Classifier: Programming Language :: Python :: 3
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: pymino Version: 1.1.9.2 Summary: Easily create a
+Metadata-Version: 2.1 Name: pymino Version: 1.1.9.3 Summary: Easily create a
 bot for Amino Apps using a modern easy to use synchronous library. Home-page:
 https://github.com/forevercynical/pymino Author: forevercynical Author-email:
 me@cynical.gg License: MIT Keywords: amino,pymino,narvii,amino-api,narvii-
 bots,aminoapps,amino-bot,amino-bots Classifier: Programming Language :: Python
 :: 3 Classifier: Programming Language :: Python :: 3.7 Classifier: Programming
 Language :: Python :: 3.8 Classifier: Programming Language :: Python :: 3.9
 Classifier: Topic :: Software Development :: Libraries :: Python Modules
```

### Comparing `pymino-1.1.9.2/README.md` & `pymino-1.1.9.3/README.md`

 * *Files identical despite different names*

### Comparing `pymino-1.1.9.2/pymino/__init__.py` & `pymino-1.1.9.3/pymino/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 __title__ = 'pymino'
 __author__ = 'cynical'
 __license__ = 'MIT'
 __copyright__ = 'Copyright 2023 Cynical'
-__version__ = '1.1.9.2'
+__version__ = '1.1.9.3'
 __description__ = 'A Python wrapper for the aminoapps.com API'
 
 from .bot import Bot as Bot
 from .async_bot import AsyncBot as AsyncBot
 from .client import Client as Client
 
 from requests import get
```

### Comparing `pymino-1.1.9.2/pymino/async_bot.py` & `pymino-1.1.9.3/pymino/async_bot.py`

 * *Files identical despite different names*

### Comparing `pymino-1.1.9.2/pymino/bot.py` & `pymino-1.1.9.3/pymino/bot.py`

 * *Files identical despite different names*

### Comparing `pymino-1.1.9.2/pymino/client.py` & `pymino-1.1.9.3/pymino/client.py`

 * *Files identical despite different names*

### Comparing `pymino-1.1.9.2/pymino/ext/account.py` & `pymino-1.1.9.3/pymino/ext/account.py`

 * *Files identical despite different names*

### Comparing `pymino-1.1.9.2/pymino/ext/async_community.py` & `pymino-1.1.9.3/pymino/ext/async_community.py`

 * *Files identical despite different names*

### Comparing `pymino-1.1.9.2/pymino/ext/async_context.py` & `pymino-1.1.9.3/pymino/ext/async_context.py`

 * *Files identical despite different names*

### Comparing `pymino-1.1.9.2/pymino/ext/async_event_handler.py` & `pymino-1.1.9.3/pymino/ext/async_event_handler.py`

 * *Files identical despite different names*

### Comparing `pymino-1.1.9.2/pymino/ext/async_socket.py` & `pymino-1.1.9.3/pymino/ext/async_socket.py`

 * *Files identical despite different names*

### Comparing `pymino-1.1.9.2/pymino/ext/community.py` & `pymino-1.1.9.3/pymino/ext/community.py`

 * *Files identical despite different names*

### Comparing `pymino-1.1.9.2/pymino/ext/console.py` & `pymino-1.1.9.3/pymino/ext/console.py`

 * *Files 13% similar despite different names*

```diff
@@ -39,14 +39,31 @@
         :param text: The string to be printed.
         :type text: str
         :param amount: The number of spaces to indent.
         :type amount: int
         """
         print(textwrap.indent(text, ' ' * self.indent_size))
 
+    def error_print(self, text=""):
+        """
+        Prints a string with a specified indentation and a red color.
+
+        :param text: The string to be printed.
+        :type text: str
+        """
+        print(Fore.RED + textwrap.indent(text, ' ' * self.indent_size) + Style.RESET_ALL)
+
+    def on_error(self, error):
+        """
+        Displays an error message to the user and prompts them to press enter to return to the main menu.
+        """
+        self.error_print(error)
+        input(f"{' ' * self.indent_size}Press enter to return to the main menu.")
+        self.fetch_menu()
+
     def sleep(self, seconds):
         """
         Sleeps for a specified number of seconds.
 
         :param seconds: The number of seconds to sleep.
         :type seconds: int
         """
```

### Comparing `pymino-1.1.9.2/pymino/ext/context.py` & `pymino-1.1.9.3/pymino/ext/context.py`

 * *Files identical despite different names*

### Comparing `pymino-1.1.9.2/pymino/ext/dispatcher.py` & `pymino-1.1.9.3/pymino/ext/dispatcher.py`

 * *Files identical despite different names*

### Comparing `pymino-1.1.9.2/pymino/ext/entities/api_response.py` & `pymino-1.1.9.3/pymino/ext/entities/api_response.py`

 * *Files identical despite different names*

### Comparing `pymino-1.1.9.2/pymino/ext/entities/chat_threads.py` & `pymino-1.1.9.3/pymino/ext/entities/chat_threads.py`

 * *Files identical despite different names*

### Comparing `pymino-1.1.9.2/pymino/ext/entities/comments.py` & `pymino-1.1.9.3/pymino/ext/entities/comments.py`

 * *Files identical despite different names*

### Comparing `pymino-1.1.9.2/pymino/ext/entities/enums.py` & `pymino-1.1.9.3/pymino/ext/entities/enums.py`

 * *Files identical despite different names*

### Comparing `pymino-1.1.9.2/pymino/ext/entities/exceptions.py` & `pymino-1.1.9.3/pymino/ext/entities/exceptions.py`

 * *Files identical despite different names*

### Comparing `pymino-1.1.9.2/pymino/ext/entities/general.py` & `pymino-1.1.9.3/pymino/ext/entities/general.py`

 * *Files identical despite different names*

### Comparing `pymino-1.1.9.2/pymino/ext/entities/handlers.py` & `pymino-1.1.9.3/pymino/ext/entities/handlers.py`

 * *Files identical despite different names*

### Comparing `pymino-1.1.9.2/pymino/ext/entities/link_info.py` & `pymino-1.1.9.3/pymino/ext/entities/link_info.py`

 * *Files identical despite different names*

### Comparing `pymino-1.1.9.2/pymino/ext/entities/messages.py` & `pymino-1.1.9.3/pymino/ext/entities/messages.py`

 * *Files identical despite different names*

### Comparing `pymino-1.1.9.2/pymino/ext/entities/notification.py` & `pymino-1.1.9.3/pymino/ext/entities/notification.py`

 * *Files identical despite different names*

### Comparing `pymino-1.1.9.2/pymino/ext/entities/userprofile.py` & `pymino-1.1.9.3/pymino/ext/entities/userprofile.py`

 * *Files identical despite different names*

### Comparing `pymino-1.1.9.2/pymino/ext/entities/wsevents.py` & `pymino-1.1.9.3/pymino/ext/entities/wsevents.py`

 * *Files identical despite different names*

### Comparing `pymino-1.1.9.2/pymino/ext/handle_queue.py` & `pymino-1.1.9.3/pymino/ext/handle_queue.py`

 * *Files identical despite different names*

### Comparing `pymino-1.1.9.2/pymino/ext/socket.py` & `pymino-1.1.9.3/pymino/ext/socket.py`

 * *Files identical despite different names*

### Comparing `pymino-1.1.9.2/pymino/ext/utilities/async_request_handler.py` & `pymino-1.1.9.3/pymino/ext/utilities/async_request_handler.py`

 * *Files identical despite different names*

### Comparing `pymino-1.1.9.2/pymino/ext/utilities/chat_console.py` & `pymino-1.1.9.3/pymino/ext/utilities/chat_console.py`

 * *Files 2% similar despite different names*

```diff
@@ -20,14 +20,17 @@
     - Type 'clear' to clear the chat.
 """
 
     def join_public_chat(self):
         """
         Handles joining of a public chat.
         """
+        if not self.console.bot.community_id:
+            return self.console.on_error("You must select a community first.")
+
         self.console.print("Join Public Chat")
         self.console.print("""
     1. Join by Chat ID
     2. Join by Link
     3. Find Public Chats To Join
     4. Back
     """)
@@ -78,14 +81,16 @@
 
         return self.console.menu.display()
 
     def my_chats(self):
         """
         Lists the user's chats and allows them to interact with selected chat.
         """
+        if not self.console.bot.community_id:
+            return self.console.on_error("You must select a community first.")
         self.print_chats()
         chat_id, chat_title = self.select_chat()
         if chat_id and chat_title:
             self.interact_with_chat(chat_id, chat_title)
         else:
             return self.console.menu.display()
```

### Comparing `pymino-1.1.9.2/pymino/ext/utilities/commands.py` & `pymino-1.1.9.3/pymino/ext/utilities/commands.py`

 * *Files identical despite different names*

### Comparing `pymino-1.1.9.2/pymino/ext/utilities/community_console.py` & `pymino-1.1.9.3/pymino/ext/utilities/community_console.py`

 * *Files 8% similar despite different names*

```diff
@@ -32,18 +32,21 @@
     def select_community(self):
         """
         Prompts the user to select a community and sets the bot's community accordingly.
         """
         communities = self.console.bot.community.joined_communities()
         self.console.print("\nSelect a community:\n")
         self.print_communities(communities)
-        print()
+        self.console.print(f"{len(communities.comId)+1}. Back\n")
         choice = self.console.input(">>> ")
         print()
 
+        if choice == str(len(communities.comId)+1):
+            return self.console.menu.display()
+        
         try:
             choice = int(choice)
             if not (1 <= choice <= len(communities.comId)):
                 raise ValueError
         except ValueError:
             self.console.print("Invalid option. Please try again.")
             return self.select_community()
```

### Comparing `pymino-1.1.9.2/pymino/ext/utilities/generate.py` & `pymino-1.1.9.3/pymino/ext/utilities/generate.py`

 * *Files identical despite different names*

### Comparing `pymino-1.1.9.2/pymino/ext/utilities/menu.py` & `pymino-1.1.9.3/pymino/ext/utilities/menu.py`

 * *Files identical despite different names*

### Comparing `pymino-1.1.9.2/pymino/ext/utilities/profile_console.py` & `pymino-1.1.9.3/pymino/ext/utilities/profile_console.py`

 * *Files 4% similar despite different names*

```diff
@@ -8,26 +8,29 @@
         """
         self.console = console
 
     def edit_profile(self):
         """
         Handles editing of user profile.
         """
+        if not self.console.bot.community_id:
+            return self.console.on_error("You must select a community first.")
+        
         self.console.print("Edit Profile")
         self.console.print("""
     1. Change Username
     2. Change Bio
     3. Change Profile Picture
     4. Change Background Picture
     5. Back
     """)
         choice = self.console.input(">>> ")
 
         try:
-            if choice == "6":
+            if choice == "5":
                 return self.console.menu.display()
 
             field_name = None
             new_value = None
 
             if choice == "1":
                 field_name = "nickname"
```

### Comparing `pymino-1.1.9.2/pymino/ext/utilities/request_handler.py` & `pymino-1.1.9.3/pymino/ext/utilities/request_handler.py`

 * *Files identical despite different names*

### Comparing `pymino-1.1.9.2/pymino.egg-info/PKG-INFO` & `pymino-1.1.9.3/pymino.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pymino
-Version: 1.1.9.2
+Version: 1.1.9.3
 Summary: Easily create a bot for Amino Apps using a modern easy to use synchronous library.
 Home-page: https://github.com/forevercynical/pymino
 Author: forevercynical
 Author-email: me@cynical.gg
 License: MIT
 Keywords: amino,pymino,narvii,amino-api,narvii-bots,aminoapps,amino-bot,amino-bots
 Classifier: Programming Language :: Python :: 3
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: pymino Version: 1.1.9.2 Summary: Easily create a
+Metadata-Version: 2.1 Name: pymino Version: 1.1.9.3 Summary: Easily create a
 bot for Amino Apps using a modern easy to use synchronous library. Home-page:
 https://github.com/forevercynical/pymino Author: forevercynical Author-email:
 me@cynical.gg License: MIT Keywords: amino,pymino,narvii,amino-api,narvii-
 bots,aminoapps,amino-bot,amino-bots Classifier: Programming Language :: Python
 :: 3 Classifier: Programming Language :: Python :: 3.7 Classifier: Programming
 Language :: Python :: 3.8 Classifier: Programming Language :: Python :: 3.9
 Classifier: Topic :: Software Development :: Libraries :: Python Modules
```

### Comparing `pymino-1.1.9.2/pymino.egg-info/SOURCES.txt` & `pymino-1.1.9.3/pymino.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `pymino-1.1.9.2/setup.cfg` & `pymino-1.1.9.3/setup.cfg`

 * *Files 10% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 00000000: 5b6d 6574 6164 6174 615d 0d0a 6e61 6d65  [metadata]..name
 00000010: 203d 2070 796d 696e 6f0d 0a76 6572 7369   = pymino..versi
-00000020: 6f6e 203d 2031 2e31 2e39 2e32 0d0a 6175  on = 1.1.9.2..au
+00000020: 6f6e 203d 2031 2e31 2e39 2e33 0d0a 6175  on = 1.1.9.3..au
 00000030: 7468 6f72 203d 2066 6f72 6576 6572 6379  thor = forevercy
 00000040: 6e69 6361 6c0d 0a61 7574 686f 725f 656d  nical..author_em
 00000050: 6169 6c20 3d20 6d65 4063 796e 6963 616c  ail = me@cynical
 00000060: 2e67 670d 0a64 6573 6372 6970 7469 6f6e  .gg..description
 00000070: 203d 2045 6173 696c 7920 6372 6561 7465   = Easily create
 00000080: 2061 2062 6f74 2066 6f72 2041 6d69 6e6f   a bot for Amino
 00000090: 2041 7070 7320 7573 696e 6720 6120 6d6f   Apps using a mo
```

### Comparing `pymino-1.1.9.2/setup.py` & `pymino-1.1.9.3/setup.py`

 * *Files identical despite different names*

