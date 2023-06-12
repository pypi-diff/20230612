# Comparing `tmp/starmoth-0.4.0.tar.gz` & `tmp/starmoth-0.4.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "starmoth-0.4.0.tar", last modified: Fri Jun  2 16:09:42 2023, max compression
+gzip compressed data, was "starmoth-0.4.1.tar", last modified: Mon Jun 12 18:46:53 2023, max compression
```

## Comparing `starmoth-0.4.0.tar` & `starmoth-0.4.1.tar`

### file list

```diff
@@ -1,23 +1,23 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-02 16:09:42.476009 starmoth-0.4.0/
--rw-r--r--   0 root         (0) root         (0)     1572 2023-06-02 16:09:42.472009 starmoth-0.4.0/PKG-INFO
--rw-rw-rw-   0 root         (0) root         (0)     1288 2023-05-17 18:11:33.000000 starmoth-0.4.0/README.md
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-02 16:09:42.468009 starmoth-0.4.0/moth/
--rw-rw-rw-   0 root         (0) root         (0)     4042 2023-05-30 20:12:28.000000 starmoth-0.4.0/moth/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-02 16:09:42.468009 starmoth-0.4.0/moth/cli/
--rw-rw-rw-   0 root         (0) root         (0)     1925 2023-05-11 20:09:31.000000 starmoth-0.4.0/moth/cli/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-02 16:09:42.468009 starmoth-0.4.0/moth/driver/
--rw-rw-rw-   0 root         (0) root         (0)     2121 2023-05-30 20:12:28.000000 starmoth-0.4.0/moth/driver/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-02 16:09:42.472009 starmoth-0.4.0/moth/message/
--rw-rw-rw-   0 root         (0) root         (0)     7186 2023-05-30 20:12:28.000000 starmoth-0.4.0/moth/message/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)      156 2023-03-01 19:53:50.000000 starmoth-0.4.0/moth/message/exceptions.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-02 16:09:42.472009 starmoth-0.4.0/moth/server/
--rw-rw-rw-   0 root         (0) root         (0)     5763 2023-05-30 20:12:28.000000 starmoth-0.4.0/moth/server/__init__.py
--rw-r--r--   0 root         (0) root         (0)       38 2023-06-02 16:09:42.476009 starmoth-0.4.0/setup.cfg
--rw-rw-rw-   0 root         (0) root         (0)      853 2023-03-01 19:53:50.000000 starmoth-0.4.0/setup.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-02 16:09:42.472009 starmoth-0.4.0/starmoth.egg-info/
--rw-r--r--   0 root         (0) root         (0)     1572 2023-06-02 16:09:42.000000 starmoth-0.4.0/starmoth.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      350 2023-06-02 16:09:42.000000 starmoth-0.4.0/starmoth.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-06-02 16:09:42.000000 starmoth-0.4.0/starmoth.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)       38 2023-06-02 16:09:42.000000 starmoth-0.4.0/starmoth.egg-info/entry_points.txt
--rw-r--r--   0 root         (0) root         (0)       43 2023-06-02 16:09:42.000000 starmoth-0.4.0/starmoth.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)        5 2023-06-02 16:09:42.000000 starmoth-0.4.0/starmoth.egg-info/top_level.txt
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-12 18:46:53.632138 starmoth-0.4.1/
+-rw-r--r--   0 root         (0) root         (0)     1572 2023-06-12 18:46:53.632138 starmoth-0.4.1/PKG-INFO
+-rw-rw-rw-   0 root         (0) root         (0)     1288 2023-06-12 18:02:40.000000 starmoth-0.4.1/README.md
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-12 18:46:53.624137 starmoth-0.4.1/moth/
+-rw-rw-rw-   0 root         (0) root         (0)     4276 2023-06-12 18:02:40.000000 starmoth-0.4.1/moth/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-12 18:46:53.624137 starmoth-0.4.1/moth/cli/
+-rw-rw-rw-   0 root         (0) root         (0)     1925 2023-05-11 20:09:31.000000 starmoth-0.4.1/moth/cli/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-12 18:46:53.628137 starmoth-0.4.1/moth/driver/
+-rw-rw-rw-   0 root         (0) root         (0)     2121 2023-05-30 20:12:28.000000 starmoth-0.4.1/moth/driver/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-12 18:46:53.628137 starmoth-0.4.1/moth/message/
+-rw-rw-rw-   0 root         (0) root         (0)     7186 2023-06-12 18:02:40.000000 starmoth-0.4.1/moth/message/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)      156 2023-03-01 19:53:50.000000 starmoth-0.4.1/moth/message/exceptions.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-12 18:46:53.628137 starmoth-0.4.1/moth/server/
+-rw-rw-rw-   0 root         (0) root         (0)     5763 2023-06-12 18:02:40.000000 starmoth-0.4.1/moth/server/__init__.py
+-rw-r--r--   0 root         (0) root         (0)       38 2023-06-12 18:46:53.632138 starmoth-0.4.1/setup.cfg
+-rw-rw-rw-   0 root         (0) root         (0)      853 2023-03-01 19:53:50.000000 starmoth-0.4.1/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-12 18:46:53.632138 starmoth-0.4.1/starmoth.egg-info/
+-rw-r--r--   0 root         (0) root         (0)     1572 2023-06-12 18:46:53.000000 starmoth-0.4.1/starmoth.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      350 2023-06-12 18:46:53.000000 starmoth-0.4.1/starmoth.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-06-12 18:46:53.000000 starmoth-0.4.1/starmoth.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)       38 2023-06-12 18:46:53.000000 starmoth-0.4.1/starmoth.egg-info/entry_points.txt
+-rw-r--r--   0 root         (0) root         (0)       43 2023-06-12 18:46:53.000000 starmoth-0.4.1/starmoth.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)        5 2023-06-12 18:46:53.000000 starmoth-0.4.1/starmoth.egg-info/top_level.txt
```

### Comparing `starmoth-0.4.0/PKG-INFO` & `starmoth-0.4.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: starmoth
-Version: 0.4.0
+Version: 0.4.1
 Summary: A small wrapper library to help test systems using STAR
 Author: Gudjon Magnusson
 Author-email: gmagnusson@fraunhofer.org
 Keywords: Fraunhofer,STAR,testing
 Requires-Python: >=3.7, <4
 Description-Content-Type: text/markdown
```

### Comparing `starmoth-0.4.0/README.md` & `starmoth-0.4.1/README.md`

 * *Files identical despite different names*

### Comparing `starmoth-0.4.0/moth/__init__.py` & `starmoth-0.4.1/moth/__init__.py`

 * *Files 4% similar despite different names*

```diff
@@ -58,41 +58,52 @@
     def _req_loop(self, socket):
         pool = zmq.Poller()
         pool.register(socket, zmq.POLLIN)
 
         last_heartbeat = None
         last_heartbeat_sent = time.time()
         result_queue = queue.Queue()
+        prompt_queue = queue.Queue()
+
+        # Workers to handle prompts
+        def prompt_loop():
+            while not self.stop:
+                func = self._PROMPT_FUNCTIONS[0]
+                message = prompt_queue.get()
+                result_queue.put(func(message))
+
+        threading.Thread(target=prompt_loop, daemon=True).start()
 
         while not self.stop:
             try:
                 events = dict(pool.poll(1000))
 
                 while not result_queue.empty():
                     result = result_queue.get()
                     socket.send(result.serialize_envelope())
 
                 if events:
+                    # Check if the prompt queue is empty
                     msg_bytes = socket.recv()
                     message = parse_message(msg_bytes)
 
                     if isinstance(message, ImagePromptMsg):
-                        func = self._PROMPT_FUNCTIONS[0]
-
-                        # Start the func in a new thread
-                        threading.Thread(target=lambda result_queue, func, message: result_queue.put(func(message)), args=(result_queue, func, message)).start()
+                        prompt_queue.put(message)
 
                     if isinstance(message, HeartbeatMsg):
                         last_heartbeat = time.time()
 
                     if isinstance(message, HandshakeResponseMsg):
                         print("Connected to server")
                         last_heartbeat = time.time()
 
-                if last_heartbeat is not None and time.time() - last_heartbeat > self.HEARTBEAT_TIMEOUT:
+                if (
+                    last_heartbeat is not None
+                    and time.time() - last_heartbeat > self.HEARTBEAT_TIMEOUT
+                ):
                     print("Lost connection to server")
                     self.stop = True
 
                 if time.time() - last_heartbeat_sent > self.HEARTBEAT_INTERVAL:
                     try:
                         socket.send(HeartbeatMsg().serialize_envelope())
                         last_heartbeat_sent = time.time()
```

### Comparing `starmoth-0.4.0/moth/cli/__init__.py` & `starmoth-0.4.1/moth/cli/__init__.py`

 * *Files identical despite different names*

### Comparing `starmoth-0.4.0/moth/driver/__init__.py` & `starmoth-0.4.1/moth/driver/__init__.py`

 * *Files identical despite different names*

### Comparing `starmoth-0.4.0/moth/message/__init__.py` & `starmoth-0.4.1/moth/message/__init__.py`

 * *Files identical despite different names*

### Comparing `starmoth-0.4.0/moth/server/__init__.py` & `starmoth-0.4.1/moth/server/__init__.py`

 * *Files identical despite different names*

### Comparing `starmoth-0.4.0/setup.py` & `starmoth-0.4.1/setup.py`

 * *Files identical despite different names*

### Comparing `starmoth-0.4.0/starmoth.egg-info/PKG-INFO` & `starmoth-0.4.1/starmoth.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: starmoth
-Version: 0.4.0
+Version: 0.4.1
 Summary: A small wrapper library to help test systems using STAR
 Author: Gudjon Magnusson
 Author-email: gmagnusson@fraunhofer.org
 Keywords: Fraunhofer,STAR,testing
 Requires-Python: >=3.7, <4
 Description-Content-Type: text/markdown
```

