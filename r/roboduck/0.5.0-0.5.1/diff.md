# Comparing `tmp/roboduck-0.5.0.tar.gz` & `tmp/roboduck-0.5.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "roboduck-0.5.0.tar", last modified: Mon Jun  5 00:25:22 2023, max compression
+gzip compressed data, was "roboduck-0.5.1.tar", last modified: Sun Jun 11 22:36:07 2023, max compression
```

## Comparing `roboduck-0.5.0.tar` & `roboduck-0.5.1.tar`

### file list

```diff
@@ -1,41 +1,41 @@
-drwxr-xr-x   0 hmamin     (501) staff       (20)        0 2023-06-05 00:25:22.981409 roboduck-0.5.0/
--rw-r--r--   0 hmamin     (501) staff       (20)      110 2023-03-29 04:32:37.000000 roboduck-0.5.0/MANIFEST.in
--rw-r--r--   0 hmamin     (501) staff       (20)    12999 2023-06-05 00:25:22.981059 roboduck-0.5.0/PKG-INFO
--rw-r--r--   0 hmamin     (501) staff       (20)    12531 2023-06-05 00:24:46.000000 roboduck-0.5.0/README.md
--rw-r--r--   0 hmamin     (501) staff       (20)      100 2023-04-30 05:54:13.000000 roboduck-0.5.0/requirements.txt
-drwxr-xr-x   0 hmamin     (501) staff       (20)        0 2023-06-05 00:25:22.972094 roboduck-0.5.0/roboduck/
--rw-r--r--   0 hmamin     (501) staff       (20)      548 2023-06-05 00:21:58.000000 roboduck-0.5.0/roboduck/__init__.py
-drwxr-xr-x   0 hmamin     (501) staff       (20)        0 2023-06-05 00:25:22.975451 roboduck-0.5.0/roboduck/cli/
--rw-r--r--   0 hmamin     (501) staff       (20)        0 2023-05-17 05:19:25.000000 roboduck-0.5.0/roboduck/cli/__init__.py
--rw-r--r--   0 hmamin     (501) staff       (20)     3412 2023-05-28 04:07:25.000000 roboduck-0.5.0/roboduck/cli/cli.py
--rw-r--r--   0 hmamin     (501) staff       (20)     7410 2023-05-24 05:02:54.000000 roboduck-0.5.0/roboduck/config.py
--rw-r--r--   0 hmamin     (501) staff       (20)    22975 2023-05-31 07:15:56.000000 roboduck-0.5.0/roboduck/debug.py
--rw-r--r--   0 hmamin     (501) staff       (20)    10858 2023-05-29 22:16:38.000000 roboduck-0.5.0/roboduck/decorators.py
--rw-r--r--   0 hmamin     (501) staff       (20)    11439 2023-05-29 23:13:09.000000 roboduck-0.5.0/roboduck/errors.py
--rw-r--r--   0 hmamin     (501) staff       (20)     5700 2023-05-25 04:02:32.000000 roboduck-0.5.0/roboduck/ipy_utils.py
-drwxr-xr-x   0 hmamin     (501) staff       (20)        0 2023-06-05 00:25:22.977151 roboduck-0.5.0/roboduck/langchain/
--rw-r--r--   0 hmamin     (501) staff       (20)        0 2023-05-13 04:59:30.000000 roboduck-0.5.0/roboduck/langchain/__init__.py
--rw-r--r--   0 hmamin     (501) staff       (20)     1512 2023-05-15 05:01:22.000000 roboduck-0.5.0/roboduck/langchain/callbacks.py
--rw-r--r--   0 hmamin     (501) staff       (20)    14589 2023-05-23 05:07:18.000000 roboduck-0.5.0/roboduck/langchain/chat.py
--rw-r--r--   0 hmamin     (501) staff       (20)     1136 2023-05-15 05:02:58.000000 roboduck-0.5.0/roboduck/langchain/utils.py
--rw-r--r--   0 hmamin     (501) staff       (20)     6333 2023-05-29 23:12:35.000000 roboduck-0.5.0/roboduck/logging.py
--rw-r--r--   0 hmamin     (501) staff       (20)     5183 2023-05-31 05:27:53.000000 roboduck-0.5.0/roboduck/magic.py
-drwxr-xr-x   0 hmamin     (501) staff       (20)        0 2023-06-05 00:25:22.978175 roboduck-0.5.0/roboduck/prompts/
--rw-r--r--   0 hmamin     (501) staff       (20)       36 2023-03-29 04:32:37.000000 roboduck-0.5.0/roboduck/prompts/__init__.py
-drwxr-xr-x   0 hmamin     (501) staff       (20)        0 2023-06-05 00:25:22.980599 roboduck-0.5.0/roboduck/prompts/chat/
--rw-r--r--   0 hmamin     (501) staff       (20)      650 2023-04-20 04:16:32.000000 roboduck-0.5.0/roboduck/prompts/chat/__template__.yaml
--rw-r--r--   0 hmamin     (501) staff       (20)     2123 2023-05-25 03:31:37.000000 roboduck-0.5.0/roboduck/prompts/chat/debug.yaml
--rw-r--r--   0 hmamin     (501) staff       (20)     2170 2023-05-25 03:31:43.000000 roboduck-0.5.0/roboduck/prompts/chat/debug_full.yaml
--rw-r--r--   0 hmamin     (501) staff       (20)     2098 2023-05-25 03:31:49.000000 roboduck-0.5.0/roboduck/prompts/chat/debug_full_stack_trace.yaml
--rw-r--r--   0 hmamin     (501) staff       (20)     2067 2023-05-25 03:31:54.000000 roboduck-0.5.0/roboduck/prompts/chat/debug_stack_trace.yaml
--rw-r--r--   0 hmamin     (501) staff       (20)     3887 2023-05-28 03:58:55.000000 roboduck-0.5.0/roboduck/prompts/utils.py
--rw-r--r--   0 hmamin     (501) staff       (20)    15138 2023-05-28 04:07:13.000000 roboduck-0.5.0/roboduck/utils.py
-drwxr-xr-x   0 hmamin     (501) staff       (20)        0 2023-06-05 00:25:22.974708 roboduck-0.5.0/roboduck.egg-info/
--rw-r--r--   0 hmamin     (501) staff       (20)    12999 2023-06-05 00:25:22.000000 roboduck-0.5.0/roboduck.egg-info/PKG-INFO
--rw-r--r--   0 hmamin     (501) staff       (20)      843 2023-06-05 00:25:22.000000 roboduck-0.5.0/roboduck.egg-info/SOURCES.txt
--rw-r--r--   0 hmamin     (501) staff       (20)        1 2023-06-05 00:25:22.000000 roboduck-0.5.0/roboduck.egg-info/dependency_links.txt
--rw-r--r--   0 hmamin     (501) staff       (20)       46 2023-06-05 00:25:22.000000 roboduck-0.5.0/roboduck.egg-info/entry_points.txt
--rw-r--r--   0 hmamin     (501) staff       (20)      100 2023-06-05 00:25:22.000000 roboduck-0.5.0/roboduck.egg-info/requires.txt
--rw-r--r--   0 hmamin     (501) staff       (20)        9 2023-06-05 00:25:22.000000 roboduck-0.5.0/roboduck.egg-info/top_level.txt
--rw-r--r--   0 hmamin     (501) staff       (20)       38 2023-06-05 00:25:22.981500 roboduck-0.5.0/setup.cfg
--rw-r--r--   0 hmamin     (501) staff       (20)     1685 2023-06-05 00:21:18.000000 roboduck-0.5.0/setup.py
+drwxr-xr-x   0 hmamin     (501) staff       (20)        0 2023-06-11 22:36:07.301744 roboduck-0.5.1/
+-rw-r--r--   0 hmamin     (501) staff       (20)      110 2023-03-29 04:32:37.000000 roboduck-0.5.1/MANIFEST.in
+-rw-r--r--   0 hmamin     (501) staff       (20)    13000 2023-06-11 22:36:07.300916 roboduck-0.5.1/PKG-INFO
+-rw-r--r--   0 hmamin     (501) staff       (20)    12532 2023-06-11 22:35:01.000000 roboduck-0.5.1/README.md
+-rw-r--r--   0 hmamin     (501) staff       (20)      100 2023-04-30 05:54:13.000000 roboduck-0.5.1/requirements.txt
+drwxr-xr-x   0 hmamin     (501) staff       (20)        0 2023-06-11 22:36:07.290075 roboduck-0.5.1/roboduck/
+-rw-r--r--   0 hmamin     (501) staff       (20)      548 2023-06-11 22:35:22.000000 roboduck-0.5.1/roboduck/__init__.py
+drwxr-xr-x   0 hmamin     (501) staff       (20)        0 2023-06-11 22:36:07.293494 roboduck-0.5.1/roboduck/cli/
+-rw-r--r--   0 hmamin     (501) staff       (20)        0 2023-05-17 05:19:25.000000 roboduck-0.5.1/roboduck/cli/__init__.py
+-rw-r--r--   0 hmamin     (501) staff       (20)     3412 2023-05-28 04:07:25.000000 roboduck-0.5.1/roboduck/cli/cli.py
+-rw-r--r--   0 hmamin     (501) staff       (20)     7410 2023-05-24 05:02:54.000000 roboduck-0.5.1/roboduck/config.py
+-rw-r--r--   0 hmamin     (501) staff       (20)    22975 2023-05-31 07:15:56.000000 roboduck-0.5.1/roboduck/debug.py
+-rw-r--r--   0 hmamin     (501) staff       (20)    10858 2023-05-29 22:16:38.000000 roboduck-0.5.1/roboduck/decorators.py
+-rw-r--r--   0 hmamin     (501) staff       (20)    11439 2023-05-29 23:13:09.000000 roboduck-0.5.1/roboduck/errors.py
+-rw-r--r--   0 hmamin     (501) staff       (20)     5700 2023-05-25 04:02:32.000000 roboduck-0.5.1/roboduck/ipy_utils.py
+drwxr-xr-x   0 hmamin     (501) staff       (20)        0 2023-06-11 22:36:07.295197 roboduck-0.5.1/roboduck/langchain/
+-rw-r--r--   0 hmamin     (501) staff       (20)        0 2023-05-13 04:59:30.000000 roboduck-0.5.1/roboduck/langchain/__init__.py
+-rw-r--r--   0 hmamin     (501) staff       (20)     1512 2023-05-15 05:01:22.000000 roboduck-0.5.1/roboduck/langchain/callbacks.py
+-rw-r--r--   0 hmamin     (501) staff       (20)    14589 2023-05-23 05:07:18.000000 roboduck-0.5.1/roboduck/langchain/chat.py
+-rw-r--r--   0 hmamin     (501) staff       (20)     1136 2023-05-15 05:02:58.000000 roboduck-0.5.1/roboduck/langchain/utils.py
+-rw-r--r--   0 hmamin     (501) staff       (20)     6333 2023-05-29 23:12:35.000000 roboduck-0.5.1/roboduck/logging.py
+-rw-r--r--   0 hmamin     (501) staff       (20)     5183 2023-05-31 05:27:53.000000 roboduck-0.5.1/roboduck/magic.py
+drwxr-xr-x   0 hmamin     (501) staff       (20)        0 2023-06-11 22:36:07.296255 roboduck-0.5.1/roboduck/prompts/
+-rw-r--r--   0 hmamin     (501) staff       (20)       36 2023-03-29 04:32:37.000000 roboduck-0.5.1/roboduck/prompts/__init__.py
+drwxr-xr-x   0 hmamin     (501) staff       (20)        0 2023-06-11 22:36:07.299902 roboduck-0.5.1/roboduck/prompts/chat/
+-rw-r--r--   0 hmamin     (501) staff       (20)      650 2023-04-20 04:16:32.000000 roboduck-0.5.1/roboduck/prompts/chat/__template__.yaml
+-rw-r--r--   0 hmamin     (501) staff       (20)     2123 2023-05-25 03:31:37.000000 roboduck-0.5.1/roboduck/prompts/chat/debug.yaml
+-rw-r--r--   0 hmamin     (501) staff       (20)     2170 2023-05-25 03:31:43.000000 roboduck-0.5.1/roboduck/prompts/chat/debug_full.yaml
+-rw-r--r--   0 hmamin     (501) staff       (20)     2098 2023-05-25 03:31:49.000000 roboduck-0.5.1/roboduck/prompts/chat/debug_full_stack_trace.yaml
+-rw-r--r--   0 hmamin     (501) staff       (20)     2067 2023-05-25 03:31:54.000000 roboduck-0.5.1/roboduck/prompts/chat/debug_stack_trace.yaml
+-rw-r--r--   0 hmamin     (501) staff       (20)     3887 2023-05-28 03:58:55.000000 roboduck-0.5.1/roboduck/prompts/utils.py
+-rw-r--r--   0 hmamin     (501) staff       (20)    15138 2023-05-28 04:07:13.000000 roboduck-0.5.1/roboduck/utils.py
+drwxr-xr-x   0 hmamin     (501) staff       (20)        0 2023-06-11 22:36:07.292694 roboduck-0.5.1/roboduck.egg-info/
+-rw-r--r--   0 hmamin     (501) staff       (20)    13000 2023-06-11 22:36:06.000000 roboduck-0.5.1/roboduck.egg-info/PKG-INFO
+-rw-r--r--   0 hmamin     (501) staff       (20)      843 2023-06-11 22:36:07.000000 roboduck-0.5.1/roboduck.egg-info/SOURCES.txt
+-rw-r--r--   0 hmamin     (501) staff       (20)        1 2023-06-11 22:36:06.000000 roboduck-0.5.1/roboduck.egg-info/dependency_links.txt
+-rw-r--r--   0 hmamin     (501) staff       (20)       46 2023-06-11 22:36:06.000000 roboduck-0.5.1/roboduck.egg-info/entry_points.txt
+-rw-r--r--   0 hmamin     (501) staff       (20)      100 2023-06-11 22:36:07.000000 roboduck-0.5.1/roboduck.egg-info/requires.txt
+-rw-r--r--   0 hmamin     (501) staff       (20)        9 2023-06-11 22:36:07.000000 roboduck-0.5.1/roboduck.egg-info/top_level.txt
+-rw-r--r--   0 hmamin     (501) staff       (20)       38 2023-06-11 22:36:07.301923 roboduck-0.5.1/setup.cfg
+-rw-r--r--   0 hmamin     (501) staff       (20)     1685 2023-06-05 00:21:18.000000 roboduck-0.5.1/setup.py
```

### Comparing `roboduck-0.5.0/PKG-INFO` & `roboduck-0.5.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: roboduck
-Version: 0.5.0
+Version: 0.5.1
 Summary: A natural language debugger.
 Author: Harrison Mamin
 Author-email: harrisonmamin@gmail.com
 License: UNKNOWN
 Project-URL: Documentation, https://hdmamin.github.io/roboduck/
 Project-URL: Repository, https://github.com/hdmamin/roboduck
 Keywords: debugging,llm,language model,dev tools,errors,jupyter magic,gpt,openai,langchain
@@ -42,15 +42,15 @@
 
 ```
 pip install roboduck
 ```
 
 ### API Key Setup
 
-You need an openai API key to begin using roboduck. Once you have an account ([sign up here](https://platform.openai.com/signup)), you can visit https://platform.openai.com/account/api-keys to retrieve your key. Your simplest option is then to call `roboduck.set_openai_api_key(api_key, update_config=True)` which essentially does the following: 
+You need an openai API key to begin using roboduck. Once you have an account ([sign up here](https://platform.openai.com/signup)), you can visit https://platform.openai.com/account/api-keys to retrieve your key. Your simplest option is then to call `roboduck.set_openai_api_key(api_key, update_config_=True)` which essentially does the following: 
 
 ```bash
 mkdir ~/.roboduck
 echo "openai_api_key: your_api_key" > ~/.roboduck/config.yaml
 ```
 
 Manually setting an OPENAI_API_KEY environment variable also works.
```

### Comparing `roboduck-0.5.0/README.md` & `roboduck-0.5.1/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -28,15 +28,15 @@
 
 ```
 pip install roboduck
 ```
 
 ### API Key Setup
 
-You need an openai API key to begin using roboduck. Once you have an account ([sign up here](https://platform.openai.com/signup)), you can visit https://platform.openai.com/account/api-keys to retrieve your key. Your simplest option is then to call `roboduck.set_openai_api_key(api_key, update_config=True)` which essentially does the following: 
+You need an openai API key to begin using roboduck. Once you have an account ([sign up here](https://platform.openai.com/signup)), you can visit https://platform.openai.com/account/api-keys to retrieve your key. Your simplest option is then to call `roboduck.set_openai_api_key(api_key, update_config_=True)` which essentially does the following: 
 
 ```bash
 mkdir ~/.roboduck
 echo "openai_api_key: your_api_key" > ~/.roboduck/config.yaml
 ```
 
 Manually setting an OPENAI_API_KEY environment variable also works.
```

### Comparing `roboduck-0.5.0/roboduck/__init__.py` & `roboduck-0.5.1/roboduck/__init__.py`

 * *Files 21% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 from roboduck.debug import duck, DuckDB, CodeCompletionCache
 from roboduck.langchain.chat import Chat, DummyChatModel
 from roboduck.config import update_config, load_config, set_openai_api_key
 from roboduck.ipy_utils import is_colab
 from roboduck.utils import available_models
 
 
-__version__ = '0.5.0'
+__version__ = '0.5.1'
 set_openai_api_key()
 if is_colab():
     warnings.warn(
         'It looks like you\'re using Google Colab, which may make your '
         'roboduck experience slightly sub-optimal (e.g. typing can be a bit '
         'laggy).'
     )
```

### Comparing `roboduck-0.5.0/roboduck/cli/cli.py` & `roboduck-0.5.1/roboduck/cli/cli.py`

 * *Files identical despite different names*

### Comparing `roboduck-0.5.0/roboduck/config.py` & `roboduck-0.5.1/roboduck/config.py`

 * *Files identical despite different names*

### Comparing `roboduck-0.5.0/roboduck/debug.py` & `roboduck-0.5.1/roboduck/debug.py`

 * *Files identical despite different names*

### Comparing `roboduck-0.5.0/roboduck/decorators.py` & `roboduck-0.5.1/roboduck/decorators.py`

 * *Files identical despite different names*

### Comparing `roboduck-0.5.0/roboduck/errors.py` & `roboduck-0.5.1/roboduck/errors.py`

 * *Files identical despite different names*

### Comparing `roboduck-0.5.0/roboduck/ipy_utils.py` & `roboduck-0.5.1/roboduck/ipy_utils.py`

 * *Files identical despite different names*

### Comparing `roboduck-0.5.0/roboduck/langchain/callbacks.py` & `roboduck-0.5.1/roboduck/langchain/callbacks.py`

 * *Files identical despite different names*

### Comparing `roboduck-0.5.0/roboduck/langchain/chat.py` & `roboduck-0.5.1/roboduck/langchain/chat.py`

 * *Files identical despite different names*

### Comparing `roboduck-0.5.0/roboduck/langchain/utils.py` & `roboduck-0.5.1/roboduck/langchain/utils.py`

 * *Files identical despite different names*

### Comparing `roboduck-0.5.0/roboduck/logging.py` & `roboduck-0.5.1/roboduck/logging.py`

 * *Files identical despite different names*

### Comparing `roboduck-0.5.0/roboduck/magic.py` & `roboduck-0.5.1/roboduck/magic.py`

 * *Files identical despite different names*

### Comparing `roboduck-0.5.0/roboduck/prompts/chat/__template__.yaml` & `roboduck-0.5.1/roboduck/prompts/chat/__template__.yaml`

 * *Files identical despite different names*

### Comparing `roboduck-0.5.0/roboduck/prompts/chat/debug.yaml` & `roboduck-0.5.1/roboduck/prompts/chat/debug.yaml`

 * *Files identical despite different names*

### Comparing `roboduck-0.5.0/roboduck/prompts/chat/debug_full.yaml` & `roboduck-0.5.1/roboduck/prompts/chat/debug_full.yaml`

 * *Files identical despite different names*

### Comparing `roboduck-0.5.0/roboduck/prompts/chat/debug_full_stack_trace.yaml` & `roboduck-0.5.1/roboduck/prompts/chat/debug_full_stack_trace.yaml`

 * *Files identical despite different names*

### Comparing `roboduck-0.5.0/roboduck/prompts/chat/debug_stack_trace.yaml` & `roboduck-0.5.1/roboduck/prompts/chat/debug_stack_trace.yaml`

 * *Files identical despite different names*

### Comparing `roboduck-0.5.0/roboduck/prompts/utils.py` & `roboduck-0.5.1/roboduck/prompts/utils.py`

 * *Files identical despite different names*

### Comparing `roboduck-0.5.0/roboduck/utils.py` & `roboduck-0.5.1/roboduck/utils.py`

 * *Files identical despite different names*

### Comparing `roboduck-0.5.0/roboduck.egg-info/PKG-INFO` & `roboduck-0.5.1/roboduck.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: roboduck
-Version: 0.5.0
+Version: 0.5.1
 Summary: A natural language debugger.
 Author: Harrison Mamin
 Author-email: harrisonmamin@gmail.com
 License: UNKNOWN
 Project-URL: Documentation, https://hdmamin.github.io/roboduck/
 Project-URL: Repository, https://github.com/hdmamin/roboduck
 Keywords: debugging,llm,language model,dev tools,errors,jupyter magic,gpt,openai,langchain
@@ -42,15 +42,15 @@
 
 ```
 pip install roboduck
 ```
 
 ### API Key Setup
 
-You need an openai API key to begin using roboduck. Once you have an account ([sign up here](https://platform.openai.com/signup)), you can visit https://platform.openai.com/account/api-keys to retrieve your key. Your simplest option is then to call `roboduck.set_openai_api_key(api_key, update_config=True)` which essentially does the following: 
+You need an openai API key to begin using roboduck. Once you have an account ([sign up here](https://platform.openai.com/signup)), you can visit https://platform.openai.com/account/api-keys to retrieve your key. Your simplest option is then to call `roboduck.set_openai_api_key(api_key, update_config_=True)` which essentially does the following: 
 
 ```bash
 mkdir ~/.roboduck
 echo "openai_api_key: your_api_key" > ~/.roboduck/config.yaml
 ```
 
 Manually setting an OPENAI_API_KEY environment variable also works.
```

### Comparing `roboduck-0.5.0/roboduck.egg-info/SOURCES.txt` & `roboduck-0.5.1/roboduck.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `roboduck-0.5.0/setup.py` & `roboduck-0.5.1/setup.py`

 * *Files identical despite different names*

