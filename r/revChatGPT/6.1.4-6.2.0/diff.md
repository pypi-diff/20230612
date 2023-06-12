# Comparing `tmp/revChatGPT-6.1.4.tar.gz` & `tmp/revChatGPT-6.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "revChatGPT-6.1.4.tar", last modified: Fri Jun  9 15:30:07 2023, max compression
+gzip compressed data, was "revChatGPT-6.2.0.tar", last modified: Mon Jun 12 10:29:06 2023, max compression
```

## Comparing `revChatGPT-6.1.4.tar` & `revChatGPT-6.2.0.tar`

### file list

```diff
@@ -1,24 +1,24 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-09 15:30:07.622983 revChatGPT-6.1.4/
--rw-r--r--   0 runner    (1001) docker     (123)    18092 2023-06-09 15:29:32.000000 revChatGPT-6.1.4/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     7961 2023-06-09 15:30:07.622983 revChatGPT-6.1.4/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     6818 2023-06-09 15:30:07.000000 revChatGPT-6.1.4/README.md
--rw-r--r--   0 runner    (1001) docker     (123)      103 2023-06-09 15:30:07.622983 revChatGPT-6.1.4/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1966 2023-06-09 15:29:32.000000 revChatGPT-6.1.4/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-09 15:30:07.618983 revChatGPT-6.1.4/src/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-09 15:30:07.622983 revChatGPT-6.1.4/src/revChatGPT/
--rw-r--r--   0 runner    (1001) docker     (123)    54195 2023-06-09 15:29:32.000000 revChatGPT-6.1.4/src/revChatGPT/V1.py
--rw-r--r--   0 runner    (1001) docker     (123)    23208 2023-06-09 15:29:32.000000 revChatGPT-6.1.4/src/revChatGPT/V3.py
--rw-r--r--   0 runner    (1001) docker     (123)     1009 2023-06-09 15:29:32.000000 revChatGPT-6.1.4/src/revChatGPT/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1716 2023-06-09 15:29:32.000000 revChatGPT-6.1.4/src/revChatGPT/__main__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-09 15:30:07.622983 revChatGPT-6.1.4/src/revChatGPT/config/
--rw-r--r--   0 runner    (1001) docker     (123)     1838 2023-06-09 15:29:32.000000 revChatGPT-6.1.4/src/revChatGPT/config/enable_internet.json
--rw-r--r--   0 runner    (1001) docker     (123)     4817 2023-06-09 15:29:32.000000 revChatGPT-6.1.4/src/revChatGPT/typings.py
--rw-r--r--   0 runner    (1001) docker     (123)     2667 2023-06-09 15:29:32.000000 revChatGPT-6.1.4/src/revChatGPT/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-09 15:30:07.622983 revChatGPT-6.1.4/src/revChatGPT.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     7961 2023-06-09 15:30:07.000000 revChatGPT-6.1.4/src/revChatGPT.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      438 2023-06-09 15:30:07.000000 revChatGPT-6.1.4/src/revChatGPT.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-09 15:30:07.000000 revChatGPT-6.1.4/src/revChatGPT.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      105 2023-06-09 15:30:07.000000 revChatGPT-6.1.4/src/revChatGPT.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       11 2023-06-09 15:30:07.000000 revChatGPT-6.1.4/src/revChatGPT.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-09 15:30:07.622983 revChatGPT-6.1.4/tests/
--rw-r--r--   0 runner    (1001) docker     (123)      508 2023-06-09 15:29:32.000000 revChatGPT-6.1.4/tests/test_recipient.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-12 10:29:06.357603 revChatGPT-6.2.0/
+-rw-r--r--   0 runner    (1001) docker     (123)    18092 2023-06-12 10:28:38.000000 revChatGPT-6.2.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     8055 2023-06-12 10:29:06.357603 revChatGPT-6.2.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     6912 2023-06-12 10:29:06.000000 revChatGPT-6.2.0/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)      103 2023-06-12 10:29:06.361603 revChatGPT-6.2.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1966 2023-06-12 10:28:38.000000 revChatGPT-6.2.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-12 10:29:06.357603 revChatGPT-6.2.0/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-12 10:29:06.357603 revChatGPT-6.2.0/src/revChatGPT/
+-rw-r--r--   0 runner    (1001) docker     (123)    54299 2023-06-12 10:28:38.000000 revChatGPT-6.2.0/src/revChatGPT/V1.py
+-rw-r--r--   0 runner    (1001) docker     (123)    23208 2023-06-12 10:28:38.000000 revChatGPT-6.2.0/src/revChatGPT/V3.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1009 2023-06-12 10:28:38.000000 revChatGPT-6.2.0/src/revChatGPT/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1716 2023-06-12 10:28:38.000000 revChatGPT-6.2.0/src/revChatGPT/__main__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-12 10:29:06.357603 revChatGPT-6.2.0/src/revChatGPT/config/
+-rw-r--r--   0 runner    (1001) docker     (123)     1838 2023-06-12 10:28:38.000000 revChatGPT-6.2.0/src/revChatGPT/config/enable_internet.json
+-rw-r--r--   0 runner    (1001) docker     (123)     4817 2023-06-12 10:28:38.000000 revChatGPT-6.2.0/src/revChatGPT/typings.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2667 2023-06-12 10:28:38.000000 revChatGPT-6.2.0/src/revChatGPT/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-12 10:29:06.357603 revChatGPT-6.2.0/src/revChatGPT.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     8055 2023-06-12 10:29:06.000000 revChatGPT-6.2.0/src/revChatGPT.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      438 2023-06-12 10:29:06.000000 revChatGPT-6.2.0/src/revChatGPT.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-12 10:29:06.000000 revChatGPT-6.2.0/src/revChatGPT.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      105 2023-06-12 10:29:06.000000 revChatGPT-6.2.0/src/revChatGPT.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       11 2023-06-12 10:29:06.000000 revChatGPT-6.2.0/src/revChatGPT.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-12 10:29:06.357603 revChatGPT-6.2.0/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)      508 2023-06-12 10:28:38.000000 revChatGPT-6.2.0/tests/test_recipient.py
```

### Comparing `revChatGPT-6.1.4/LICENSE` & `revChatGPT-6.2.0/LICENSE`

 * *Files identical despite different names*

### Comparing `revChatGPT-6.1.4/PKG-INFO` & `revChatGPT-6.2.0/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: revChatGPT
-Version: 6.1.4
+Version: 6.2.0
 Summary: ChatGPT is a reverse engineering of OpenAI's ChatGPT API
 Home-page: https://github.com/acheong08/ChatGPT
 Author: Antonio Cheong
 Author-email: acheong@student.dalat.org
 License: GNU General Public License v2.0
 Project-URL: Bug Report, https://github.com/acheong08/ChatGPT/issues/new?assignees=&labels=bug-report&template=bug_report.yml&title=%5BBug%5D%3A+
 Project-URL: Feature request, https://github.com/acheong08/ChatGPT/issues/new?assignees=&labels=enhancement&template=feature_request.yml&title=%5BFeature+Request%5D%3A+
@@ -91,14 +91,15 @@
 {
   "conversation_id": "UUID...",
   "parent_id": "UUID...",
   "proxy": "...",
   "model": "gpt-4", // gpt-4-browsing, text-davinci-002-render-sha, gpt-4, gpt-4-plugins
   "plugin_ids" : ["plugin-d1d6eb04-3375-40aa-940a-c2fc57ce0f51"], // Wolfram Alpha example
   "disable_history": true,
+  "PUID": "<_puid cookie for plus accounts>" // Only if you have a plus account and use GPT-4
 }
 ```
 
 1. Save this as `$HOME/.config/revChatGPT/config.json`
 2. If you are using Windows, you will need to create an environment variable named `HOME` and set it to your home profile for the script to be able to locate the config.json file.
 
 Plugin IDs can be found [here](./plugins.json). Remember to set model to `gpt-4-plugins` if plugins are enabled. Plugins may or may not work if you haven't installed them from the web interface. You can call `chatbot.install_plugin(plugin_id=plugin_id)` to install any one of them from code. Call `chatbot.get_plugins()` to get a list of all plugins available.
```

### Comparing `revChatGPT-6.1.4/README.md` & `revChatGPT-6.2.0/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -69,14 +69,15 @@
 {
   "conversation_id": "UUID...",
   "parent_id": "UUID...",
   "proxy": "...",
   "model": "gpt-4", // gpt-4-browsing, text-davinci-002-render-sha, gpt-4, gpt-4-plugins
   "plugin_ids" : ["plugin-d1d6eb04-3375-40aa-940a-c2fc57ce0f51"], // Wolfram Alpha example
   "disable_history": true,
+  "PUID": "<_puid cookie for plus accounts>" // Only if you have a plus account and use GPT-4
 }
 ```
 
 1. Save this as `$HOME/.config/revChatGPT/config.json`
 2. If you are using Windows, you will need to create an environment variable named `HOME` and set it to your home profile for the script to be able to locate the config.json file.
 
 Plugin IDs can be found [here](./plugins.json). Remember to set model to `gpt-4-plugins` if plugins are enabled. Plugins may or may not work if you haven't installed them from the web interface. You can call `chatbot.install_plugin(plugin_id=plugin_id)` to install any one of them from code. Call `chatbot.get_plugins()` to get a list of all plugins available.
```

### Comparing `revChatGPT-6.1.4/setup.py` & `revChatGPT-6.2.0/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -8,15 +8,15 @@
 if not PATH.exists():
     with open(DOCS_PATH, encoding="utf-8") as f1:
         with open(PATH, "w+", encoding="utf-8") as f2:
             f2.write(f1.read())
 
 setup(
     name="revChatGPT",
-    version="6.1.4",
+    version="6.2.0",
     description="ChatGPT is a reverse engineering of OpenAI's ChatGPT API",
     long_description=open(PATH, encoding="utf-8").read(),
     long_description_content_type="text/markdown",
     url="https://github.com/acheong08/ChatGPT",
     project_urls={
         "Bug Report": "https://github.com/acheong08/ChatGPT/issues/new?assignees=&labels=bug-report&template=bug_report.yml&title=%5BBug%5D%3A+",
         "Feature request": "https://github.com/acheong08/ChatGPT/issues/new?assignees=&labels=enhancement&template=feature_request.yml&title=%5BFeature+Request%5D%3A+",
```

### Comparing `revChatGPT-6.1.4/src/revChatGPT/V1.py` & `revChatGPT-6.2.0/src/revChatGPT/V1.py`

 * *Files 0% similar despite different names*

```diff
@@ -163,14 +163,17 @@
         self.parent_id_prev_queue = []
         self.lazy_loading = lazy_loading
         self.base_url = base_url or BASE_URL
         self.disable_history = config.get("disable_history", False)
 
         self.__check_credentials()
 
+        if self.config.get("PUID"):
+            self.session.cookies.set("_puid", self.config["PUID"])
+
     @logger(is_timed=True)
     def __check_credentials(self) -> None:
         """Check login info and perform login
 
         Any one of the following is sufficient for login. Multiple login info can be provided at the same time and they will be used in the order listed below.
             - access_token
             - email + password
```

### Comparing `revChatGPT-6.1.4/src/revChatGPT/V3.py` & `revChatGPT-6.2.0/src/revChatGPT/V3.py`

 * *Files identical despite different names*

### Comparing `revChatGPT-6.1.4/src/revChatGPT/__init__.py` & `revChatGPT-6.2.0/src/revChatGPT/__init__.py`

 * *Files identical despite different names*

### Comparing `revChatGPT-6.1.4/src/revChatGPT/__main__.py` & `revChatGPT-6.2.0/src/revChatGPT/__main__.py`

 * *Files identical despite different names*

### Comparing `revChatGPT-6.1.4/src/revChatGPT/config/enable_internet.json` & `revChatGPT-6.2.0/src/revChatGPT/config/enable_internet.json`

 * *Files identical despite different names*

### Comparing `revChatGPT-6.1.4/src/revChatGPT/typings.py` & `revChatGPT-6.2.0/src/revChatGPT/typings.py`

 * *Files identical despite different names*

### Comparing `revChatGPT-6.1.4/src/revChatGPT/utils.py` & `revChatGPT-6.2.0/src/revChatGPT/utils.py`

 * *Files identical despite different names*

### Comparing `revChatGPT-6.1.4/src/revChatGPT.egg-info/PKG-INFO` & `revChatGPT-6.2.0/src/revChatGPT.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: revChatGPT
-Version: 6.1.4
+Version: 6.2.0
 Summary: ChatGPT is a reverse engineering of OpenAI's ChatGPT API
 Home-page: https://github.com/acheong08/ChatGPT
 Author: Antonio Cheong
 Author-email: acheong@student.dalat.org
 License: GNU General Public License v2.0
 Project-URL: Bug Report, https://github.com/acheong08/ChatGPT/issues/new?assignees=&labels=bug-report&template=bug_report.yml&title=%5BBug%5D%3A+
 Project-URL: Feature request, https://github.com/acheong08/ChatGPT/issues/new?assignees=&labels=enhancement&template=feature_request.yml&title=%5BFeature+Request%5D%3A+
@@ -91,14 +91,15 @@
 {
   "conversation_id": "UUID...",
   "parent_id": "UUID...",
   "proxy": "...",
   "model": "gpt-4", // gpt-4-browsing, text-davinci-002-render-sha, gpt-4, gpt-4-plugins
   "plugin_ids" : ["plugin-d1d6eb04-3375-40aa-940a-c2fc57ce0f51"], // Wolfram Alpha example
   "disable_history": true,
+  "PUID": "<_puid cookie for plus accounts>" // Only if you have a plus account and use GPT-4
 }
 ```
 
 1. Save this as `$HOME/.config/revChatGPT/config.json`
 2. If you are using Windows, you will need to create an environment variable named `HOME` and set it to your home profile for the script to be able to locate the config.json file.
 
 Plugin IDs can be found [here](./plugins.json). Remember to set model to `gpt-4-plugins` if plugins are enabled. Plugins may or may not work if you haven't installed them from the web interface. You can call `chatbot.install_plugin(plugin_id=plugin_id)` to install any one of them from code. Call `chatbot.get_plugins()` to get a list of all plugins available.
```

