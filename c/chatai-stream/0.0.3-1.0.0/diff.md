# Comparing `tmp/chatai-stream-0.0.3.tar.gz` & `tmp/chatai-stream-1.0.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "chatai-stream-0.0.3.tar", last modified: Wed Jun  7 14:57:23 2023, max compression
+gzip compressed data, was "chatai-stream-1.0.0.tar", last modified: Mon Jun 12 17:36:35 2023, max compression
```

## Comparing `chatai-stream-0.0.3.tar` & `chatai-stream-1.0.0.tar`

### file list

```diff
@@ -1,16 +1,16 @@
-drwxr-xr-x   0 GeneralYadoc  (1001) GeneralYadoc  (1001)        0 2023-06-07 14:57:23.756641 chatai-stream-0.0.3/
--rw-r--r--   0 GeneralYadoc  (1001) GeneralYadoc  (1001)     1069 2023-05-28 11:25:30.000000 chatai-stream-0.0.3/LICENSE
--rw-r--r--   0 GeneralYadoc  (1001) GeneralYadoc  (1001)      594 2023-06-07 14:57:23.756641 chatai-stream-0.0.3/PKG-INFO
--rw-r--r--   0 GeneralYadoc  (1001) GeneralYadoc  (1001)     8103 2023-06-06 12:52:21.000000 chatai-stream-0.0.3/README.md
--rw-r--r--   0 GeneralYadoc  (1001) GeneralYadoc  (1001)       38 2023-06-07 14:57:23.756641 chatai-stream-0.0.3/setup.cfg
--rw-r--r--   0 GeneralYadoc  (1001) GeneralYadoc  (1001)     1162 2023-06-07 14:34:45.000000 chatai-stream-0.0.3/setup.py
-drwxr-xr-x   0 GeneralYadoc  (1001) GeneralYadoc  (1001)        0 2023-06-07 14:57:23.756641 chatai-stream-0.0.3/src/
--rw-r--r--   0 GeneralYadoc  (1001) GeneralYadoc  (1001)     1610 2023-06-07 14:17:02.000000 chatai-stream-0.0.3/src/ChatAIStream.py
--rw-r--r--   0 GeneralYadoc  (1001) GeneralYadoc  (1001)       51 2023-06-07 14:35:24.000000 chatai-stream-0.0.3/src/__init__.py
-drwxr-xr-x   0 GeneralYadoc  (1001) GeneralYadoc  (1001)        0 2023-06-07 14:57:23.756641 chatai-stream-0.0.3/src/chatai_stream.egg-info/
--rw-r--r--   0 GeneralYadoc  (1001) GeneralYadoc  (1001)      594 2023-06-07 14:57:23.000000 chatai-stream-0.0.3/src/chatai_stream.egg-info/PKG-INFO
--rw-r--r--   0 GeneralYadoc  (1001) GeneralYadoc  (1001)      306 2023-06-07 14:57:23.000000 chatai-stream-0.0.3/src/chatai_stream.egg-info/SOURCES.txt
--rw-r--r--   0 GeneralYadoc  (1001) GeneralYadoc  (1001)        1 2023-06-07 14:57:23.000000 chatai-stream-0.0.3/src/chatai_stream.egg-info/dependency_links.txt
--rw-r--r--   0 GeneralYadoc  (1001) GeneralYadoc  (1001)        1 2023-06-06 12:52:21.000000 chatai-stream-0.0.3/src/chatai_stream.egg-info/not-zip-safe
--rw-r--r--   0 GeneralYadoc  (1001) GeneralYadoc  (1001)       44 2023-06-07 14:57:23.000000 chatai-stream-0.0.3/src/chatai_stream.egg-info/requires.txt
--rw-r--r--   0 GeneralYadoc  (1001) GeneralYadoc  (1001)       22 2023-06-07 14:57:23.000000 chatai-stream-0.0.3/src/chatai_stream.egg-info/top_level.txt
+drwxr-xr-x   0 GeneralYadoc  (1001) GeneralYadoc  (1001)        0 2023-06-12 17:36:35.188883 chatai-stream-1.0.0/
+-rw-r--r--   0 GeneralYadoc  (1001) GeneralYadoc  (1001)     1069 2023-05-28 11:25:30.000000 chatai-stream-1.0.0/LICENSE
+-rw-r--r--   0 GeneralYadoc  (1001) GeneralYadoc  (1001)      594 2023-06-12 17:36:35.188883 chatai-stream-1.0.0/PKG-INFO
+-rw-r--r--   0 GeneralYadoc  (1001) GeneralYadoc  (1001)     8218 2023-06-12 17:34:29.000000 chatai-stream-1.0.0/README.md
+-rw-r--r--   0 GeneralYadoc  (1001) GeneralYadoc  (1001)       38 2023-06-12 17:36:35.188883 chatai-stream-1.0.0/setup.cfg
+-rw-r--r--   0 GeneralYadoc  (1001) GeneralYadoc  (1001)     1162 2023-06-12 17:34:29.000000 chatai-stream-1.0.0/setup.py
+drwxr-xr-x   0 GeneralYadoc  (1001) GeneralYadoc  (1001)        0 2023-06-12 17:36:35.188883 chatai-stream-1.0.0/src/
+-rw-r--r--   0 GeneralYadoc  (1001) GeneralYadoc  (1001)     1695 2023-06-12 17:34:29.000000 chatai-stream-1.0.0/src/ChatAIStream.py
+-rw-r--r--   0 GeneralYadoc  (1001) GeneralYadoc  (1001)       51 2023-06-12 17:34:29.000000 chatai-stream-1.0.0/src/__init__.py
+drwxr-xr-x   0 GeneralYadoc  (1001) GeneralYadoc  (1001)        0 2023-06-12 17:36:35.188883 chatai-stream-1.0.0/src/chatai_stream.egg-info/
+-rw-r--r--   0 GeneralYadoc  (1001) GeneralYadoc  (1001)      594 2023-06-12 17:36:35.000000 chatai-stream-1.0.0/src/chatai_stream.egg-info/PKG-INFO
+-rw-r--r--   0 GeneralYadoc  (1001) GeneralYadoc  (1001)      306 2023-06-12 17:36:35.000000 chatai-stream-1.0.0/src/chatai_stream.egg-info/SOURCES.txt
+-rw-r--r--   0 GeneralYadoc  (1001) GeneralYadoc  (1001)        1 2023-06-12 17:36:35.000000 chatai-stream-1.0.0/src/chatai_stream.egg-info/dependency_links.txt
+-rw-r--r--   0 GeneralYadoc  (1001) GeneralYadoc  (1001)        1 2023-06-12 17:34:29.000000 chatai-stream-1.0.0/src/chatai_stream.egg-info/not-zip-safe
+-rw-r--r--   0 GeneralYadoc  (1001) GeneralYadoc  (1001)       44 2023-06-12 17:36:35.000000 chatai-stream-1.0.0/src/chatai_stream.egg-info/requires.txt
+-rw-r--r--   0 GeneralYadoc  (1001) GeneralYadoc  (1001)       22 2023-06-12 17:36:35.000000 chatai-stream-1.0.0/src/chatai_stream.egg-info/top_level.txt
```

### Comparing `chatai-stream-0.0.3/LICENSE` & `chatai-stream-1.0.0/LICENSE`

 * *Files identical despite different names*

### Comparing `chatai-stream-0.0.3/PKG-INFO` & `chatai-stream-1.0.0/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: chatai-stream
-Version: 0.0.3
+Version: 1.0.0
 Summary: ChatGPT reacts YouTube chat messages.
 Home-page: https://github.com/GeneralYadoc/ChatAIStream
 Author: General Yadoc
 Author-email: 133023047+GeneralYadoc@users.noreply.github.com
 License: MIT
 Platform: UNKNOWN
 Classifier: Development Status :: 4 - Beta
```

### Comparing `chatai-stream-0.0.3/README.md` & `chatai-stream-1.0.0/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -118,15 +118,15 @@
   The outputs of the right window are provided by this sample.<br>
   Left outputs are also available by ChatAIStream.
   ![](ReadMeParts/ChatAIAgent.gif)
 
 ## Arguments of Constructor
 - ChatAIStream object can be configured with following params given to constructor.
 
-  ### steamParams
+  ### streamParams
     | name | description | default |
     |------|------------|---------|
     | video_id | String following after 'v=' in url of target YouTube live | - |
     | get_item_cb | Chat items are thrown to this callback | None |
     | pre_filter_cb | Filter set before internal queue | None |
     | post_filter_cb | Filter set between internal queue and get_item_cb | None |
     | max_queue_size | Max slots of internal queue (0 is no limit) | 1000 |
@@ -166,14 +166,17 @@
 - No arguments required, nothing returns.
 
 ### disconnect()
 - Request to terminate YouTube Chat polling, ChatGPT conversation and calling user callbacks.
 - Internal process will be terminated soon after.
 - No arguments required, nothing returns.
 
+### full_messages_for_ask()
+- Indicate whether the queue which spools messages to send ChatAI is full or not.
+
 And other [threading.Thread](https://docs.python.org/3/library/threading.html) public pethods are available.
 
 ## Callbacks
 ### get_item_cb
 - Callback for getting YouTube chat items.
 - You can implement several processes in it.
 - YouTube chat item is thrown as an argument.
```

### Comparing `chatai-stream-0.0.3/setup.py` & `chatai-stream-1.0.0/setup.py`

 * *Files 8% similar despite different names*

```diff
@@ -8,15 +8,15 @@
 
 def _requires_from_file(filename):
     return open(filename).read().splitlines()
 
 
 setup(
     name="chatai-stream",
-    version="0.0.3",
+    version="1.0.0",
     license="MIT",
     description="ChatGPT reacts YouTube chat messages.",
     author="General Yadoc",
     author_email="133023047+GeneralYadoc@users.noreply.github.com",
     classifiers=[
         'Development Status :: 4 - Beta',
         'Programming Language :: Python',
```

### Comparing `chatai-stream-0.0.3/src/ChatAIStream.py` & `chatai-stream-1.0.0/src/ChatAIStream.py`

 * *Files 8% similar despite different names*

```diff
@@ -11,39 +11,42 @@
 
 @dataclass
 class params():
   stream_params: streamParams
   ai_params: aiParams
 
 class ChatAIStream(threading.Thread):
-  def my_pre_filter_cb(self, c):
+  def __my_pre_filter_cb(self, c):
     prefiltered_c = c
     if prefiltered_c and self.pre_filter_cb:
       prefiltered_c = self.pre_filter_cb(prefiltered_c)
     prefiltered_c.message = re.sub(r':[^:]+:', ".", prefiltered_c.message)
     prefiltered_c.message = re.sub(r'^[\.]+', "", prefiltered_c.message)
     return None if prefiltered_c.message == "" else prefiltered_c
 
-  def ask_stream_message_to_ai(self, c):
+  def __ask_stream_message_to_ai(self, c):
     if self.get_stream_message_cb:
       self.get_stream_message_cb(c)
     if self.ai_agent:
       self.ai_agent.put_message(ca.userMessage(message=c.message, extern=c))
   
   def __init__( self, params):
     self.get_stream_message_cb=params.stream_params.get_item_cb
-    params.stream_params.get_item_cb=self.ask_stream_message_to_ai
+    params.stream_params.get_item_cb=self.__ask_stream_message_to_ai
     self.pre_filter_cb=params.stream_params.pre_filter_cb
-    params.stream_params.pre_filter_cb=self.my_pre_filter_cb
+    params.stream_params.pre_filter_cb=self.__my_pre_filter_cb
 
     self.ai_agent = ca.ChatAIAgent( params.ai_params )
     self.stream_agent = sca.StreamChatAgent( params.stream_params )
     
     super(ChatAIStream, self).__init__(daemon=True)
   
+  def full_messages_for_ask(self):
+    return self.ai_agent.full_messages()
+
   def run(self):
     self.stream_agent.start()
     self.ai_agent.start()
 
   def connect(self):
     self.start()
     self.join()
```

### Comparing `chatai-stream-0.0.3/src/chatai_stream.egg-info/PKG-INFO` & `chatai-stream-1.0.0/src/chatai_stream.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: chatai-stream
-Version: 0.0.3
+Version: 1.0.0
 Summary: ChatGPT reacts YouTube chat messages.
 Home-page: https://github.com/GeneralYadoc/ChatAIStream
 Author: General Yadoc
 Author-email: 133023047+GeneralYadoc@users.noreply.github.com
 License: MIT
 Platform: UNKNOWN
 Classifier: Development Status :: 4 - Beta
```

