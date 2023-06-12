# Comparing `tmp/chatai-streamer-2.0.0.tar.gz` & `tmp/chatai-streamer-2.0.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "chatai-streamer-2.0.0.tar", last modified: Wed Jun  7 18:31:07 2023, max compression
+gzip compressed data, was "chatai-streamer-2.0.1.tar", last modified: Mon Jun 12 17:53:24 2023, max compression
```

## Comparing `chatai-streamer-2.0.0.tar` & `chatai-streamer-2.0.1.tar`

### file list

```diff
@@ -1,17 +1,17 @@
-drwxr-xr-x   0 GeneralYadoc  (1001) GeneralYadoc  (1001)        0 2023-06-07 18:31:07.236641 chatai-streamer-2.0.0/
--rw-r--r--   0 GeneralYadoc  (1001) GeneralYadoc  (1001)     1069 2023-05-28 12:23:33.000000 chatai-streamer-2.0.0/LICENSE
--rw-r--r--   0 GeneralYadoc  (1001) GeneralYadoc  (1001)      604 2023-06-07 18:31:07.236641 chatai-streamer-2.0.0/PKG-INFO
--rw-r--r--   0 GeneralYadoc  (1001) GeneralYadoc  (1001)    13838 2023-06-07 18:22:28.000000 chatai-streamer-2.0.0/README.md
--rw-r--r--   0 GeneralYadoc  (1001) GeneralYadoc  (1001)       38 2023-06-07 18:31:07.236641 chatai-streamer-2.0.0/setup.cfg
--rw-r--r--   0 GeneralYadoc  (1001) GeneralYadoc  (1001)     1172 2023-06-07 18:23:04.000000 chatai-streamer-2.0.0/setup.py
-drwxr-xr-x   0 GeneralYadoc  (1001) GeneralYadoc  (1001)        0 2023-06-07 18:31:07.236641 chatai-streamer-2.0.0/src/
--rwxr-xr-x   0 GeneralYadoc  (1001) GeneralYadoc  (1001)     2455 2023-06-07 18:21:52.000000 chatai-streamer-2.0.0/src/ChatAIStreamer.py
--rwxr-xr-x   0 GeneralYadoc  (1001) GeneralYadoc  (1001)     4821 2023-06-07 17:58:19.000000 chatai-streamer-2.0.0/src/GttsAIStreamer.py
--rw-r--r--   0 GeneralYadoc  (1001) GeneralYadoc  (1001)       83 2023-06-07 18:23:19.000000 chatai-streamer-2.0.0/src/__init__.py
-drwxr-xr-x   0 GeneralYadoc  (1001) GeneralYadoc  (1001)        0 2023-06-07 18:31:07.236641 chatai-streamer-2.0.0/src/chatai_streamer.egg-info/
--rw-r--r--   0 GeneralYadoc  (1001) GeneralYadoc  (1001)      604 2023-06-07 18:31:07.000000 chatai-streamer-2.0.0/src/chatai_streamer.egg-info/PKG-INFO
--rw-r--r--   0 GeneralYadoc  (1001) GeneralYadoc  (1001)      342 2023-06-07 18:31:07.000000 chatai-streamer-2.0.0/src/chatai_streamer.egg-info/SOURCES.txt
--rw-r--r--   0 GeneralYadoc  (1001) GeneralYadoc  (1001)        1 2023-06-07 18:31:07.000000 chatai-streamer-2.0.0/src/chatai_streamer.egg-info/dependency_links.txt
--rw-r--r--   0 GeneralYadoc  (1001) GeneralYadoc  (1001)        1 2023-06-06 13:54:02.000000 chatai-streamer-2.0.0/src/chatai_streamer.egg-info/not-zip-safe
--rw-r--r--   0 GeneralYadoc  (1001) GeneralYadoc  (1001)      104 2023-06-07 18:31:07.000000 chatai-streamer-2.0.0/src/chatai_streamer.egg-info/requires.txt
--rw-r--r--   0 GeneralYadoc  (1001) GeneralYadoc  (1001)       39 2023-06-07 18:31:07.000000 chatai-streamer-2.0.0/src/chatai_streamer.egg-info/top_level.txt
+drwxr-xr-x   0 GeneralYadoc  (1001) GeneralYadoc  (1001)        0 2023-06-12 17:53:24.008883 chatai-streamer-2.0.1/
+-rw-r--r--   0 GeneralYadoc  (1001) GeneralYadoc  (1001)     1069 2023-05-28 12:23:33.000000 chatai-streamer-2.0.1/LICENSE
+-rw-r--r--   0 GeneralYadoc  (1001) GeneralYadoc  (1001)      604 2023-06-12 17:53:24.008883 chatai-streamer-2.0.1/PKG-INFO
+-rw-r--r--   0 GeneralYadoc  (1001) GeneralYadoc  (1001)    13838 2023-06-08 17:50:05.000000 chatai-streamer-2.0.1/README.md
+-rw-r--r--   0 GeneralYadoc  (1001) GeneralYadoc  (1001)       38 2023-06-12 17:53:24.008883 chatai-streamer-2.0.1/setup.cfg
+-rw-r--r--   0 GeneralYadoc  (1001) GeneralYadoc  (1001)     1172 2023-06-12 17:50:32.000000 chatai-streamer-2.0.1/setup.py
+drwxr-xr-x   0 GeneralYadoc  (1001) GeneralYadoc  (1001)        0 2023-06-12 17:53:24.008883 chatai-streamer-2.0.1/src/
+-rwxr-xr-x   0 GeneralYadoc  (1001) GeneralYadoc  (1001)     2555 2023-06-12 17:50:32.000000 chatai-streamer-2.0.1/src/ChatAIStreamer.py
+-rwxr-xr-x   0 GeneralYadoc  (1001) GeneralYadoc  (1001)     4821 2023-06-07 17:58:19.000000 chatai-streamer-2.0.1/src/GttsAIStreamer.py
+-rw-r--r--   0 GeneralYadoc  (1001) GeneralYadoc  (1001)       83 2023-06-12 17:50:32.000000 chatai-streamer-2.0.1/src/__init__.py
+drwxr-xr-x   0 GeneralYadoc  (1001) GeneralYadoc  (1001)        0 2023-06-12 17:53:24.008883 chatai-streamer-2.0.1/src/chatai_streamer.egg-info/
+-rw-r--r--   0 GeneralYadoc  (1001) GeneralYadoc  (1001)      604 2023-06-12 17:53:23.000000 chatai-streamer-2.0.1/src/chatai_streamer.egg-info/PKG-INFO
+-rw-r--r--   0 GeneralYadoc  (1001) GeneralYadoc  (1001)      342 2023-06-12 17:53:23.000000 chatai-streamer-2.0.1/src/chatai_streamer.egg-info/SOURCES.txt
+-rw-r--r--   0 GeneralYadoc  (1001) GeneralYadoc  (1001)        1 2023-06-12 17:53:23.000000 chatai-streamer-2.0.1/src/chatai_streamer.egg-info/dependency_links.txt
+-rw-r--r--   0 GeneralYadoc  (1001) GeneralYadoc  (1001)        1 2023-06-12 17:50:32.000000 chatai-streamer-2.0.1/src/chatai_streamer.egg-info/not-zip-safe
+-rw-r--r--   0 GeneralYadoc  (1001) GeneralYadoc  (1001)      104 2023-06-12 17:53:23.000000 chatai-streamer-2.0.1/src/chatai_streamer.egg-info/requires.txt
+-rw-r--r--   0 GeneralYadoc  (1001) GeneralYadoc  (1001)       39 2023-06-12 17:53:23.000000 chatai-streamer-2.0.1/src/chatai_streamer.egg-info/top_level.txt
```

### Comparing `chatai-streamer-2.0.0/LICENSE` & `chatai-streamer-2.0.1/LICENSE`

 * *Files identical despite different names*

### Comparing `chatai-streamer-2.0.0/PKG-INFO` & `chatai-streamer-2.0.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: chatai-streamer
-Version: 2.0.0
+Version: 2.0.1
 Summary: ChatGPT answer aloud YouTube chat messages.
 Home-page: https://github.com/GeneralYadoc/ChatAIStreamer
 Author: General Yadoc
 Author-email: 133023047+GeneralYadoc@users.noreply.github.com
 License: MIT
 Platform: UNKNOWN
 Classifier: Development Status :: 4 - Beta
```

### Comparing `chatai-streamer-2.0.0/README.md` & `chatai-streamer-2.0.1/README.md`

 * *Files 0% similar despite different names*

```diff
@@ -237,15 +237,15 @@
   ```usage
   $ python3 ./sample.py VIDEO-ID OpenAI-API-KEY
   ```
 - Output of the sample<br>
   The outputs of the voices and the right window are provided by this sample.<br>
   Left outputs are also available by ChatAIStreamer.
   
-  [![GttsAIStreamer sample](ReadMeParts/ChatAIStreamer.png)](https://www.youtube.com/embed/sesl9VZHDA8)
+  [![GttsAIStreamer sample](ReadMeParts/ChatAIStreamer.png)](https://www.youtube.com/embed/k_7Ona9JuBo)
 
 ## Arguments of Constructor
 - ChatAIStreamer object can be configured with following params given to constructor.
 
   ### streamParams
     | name | description | default |
     |------|------------|---------|
```

### Comparing `chatai-streamer-2.0.0/setup.py` & `chatai-streamer-2.0.1/setup.py`

 * *Files 8% similar despite different names*

```diff
@@ -8,15 +8,15 @@
 
 def _requires_from_file(filename):
     return open(filename).read().splitlines()
 
 
 setup(
     name="chatai-streamer",
-    version="2.0.0",
+    version="2.0.1",
     license="MIT",
     description="ChatGPT answer aloud YouTube chat messages.",
     author="General Yadoc",
     author_email="133023047+GeneralYadoc@users.noreply.github.com",
     classifiers=[
         'Development Status :: 4 - Beta',
         'Programming Language :: Python',
```

### Comparing `chatai-streamer-2.0.0/src/ChatAIStreamer.py` & `chatai-streamer-2.0.1/src/ChatAIStreamer.py`

 * *Files 6% similar despite different names*

```diff
@@ -45,14 +45,17 @@
           self.answer_with_voice_cb(answer_slot.user_message, answer_slot.completion, voice)
 
   def my_answer_cb(self, user_message, completion):
     if self.answer_cb:
       self.answer_cb(user_message, completion)
     if self.voice_generator:
       while self.__keeping_connection and self.__answer_queue.full():
+        if self.full_messages_for_ask():
+          self.__answer_queue.get_nowait()
+          break
         time.sleep(0.01)
       if self.__keeping_connection:
         self.__answer_queue.put(answerSlot(user_message=user_message, completion=completion))
 
   def __init__(self, params):
     self.__keeping_connection = False
     self.voice_generator = params.streamer_params.voice_generator
```

### Comparing `chatai-streamer-2.0.0/src/GttsAIStreamer.py` & `chatai-streamer-2.0.1/src/GttsAIStreamer.py`

 * *Files identical despite different names*

### Comparing `chatai-streamer-2.0.0/src/chatai_streamer.egg-info/PKG-INFO` & `chatai-streamer-2.0.1/src/chatai_streamer.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: chatai-streamer
-Version: 2.0.0
+Version: 2.0.1
 Summary: ChatGPT answer aloud YouTube chat messages.
 Home-page: https://github.com/GeneralYadoc/ChatAIStreamer
 Author: General Yadoc
 Author-email: 133023047+GeneralYadoc@users.noreply.github.com
 License: MIT
 Platform: UNKNOWN
 Classifier: Development Status :: 4 - Beta
```

