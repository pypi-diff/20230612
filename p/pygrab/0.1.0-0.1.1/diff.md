# Comparing `tmp/pygrab-0.1.0.tar.gz` & `tmp/pygrab-0.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pygrab-0.1.0.tar", last modified: Wed May 31 05:44:58 2023, max compression
+gzip compressed data, was "pygrab-0.1.1.tar", last modified: Mon Jun 12 05:44:03 2023, max compression
```

## Comparing `pygrab-0.1.0.tar` & `pygrab-0.1.1.tar`

### file list

```diff
@@ -1,14 +1,14 @@
-drwxrwxrwx   0        0        0        0 2023-05-31 05:44:58.110000 pygrab-0.1.0/
--rw-rw-rw-   0        0        0      183 2023-05-31 05:44:58.098000 pygrab-0.1.0/PKG-INFO
--rw-rw-rw-   0        0        0      341 2023-05-31 05:39:15.000000 pygrab-0.1.0/README.md
-drwxrwxrwx   0        0        0        0 2023-05-31 05:44:57.992000 pygrab-0.1.0/pygrab/
--rw-rw-rw-   0        0        0       21 2023-05-30 03:16:15.000000 pygrab-0.1.0/pygrab/__init__.py
--rw-rw-rw-   0        0        0    10511 2023-05-31 05:32:43.000000 pygrab-0.1.0/pygrab/pygrab.py
-drwxrwxrwx   0        0        0        0 2023-05-31 05:44:58.081000 pygrab-0.1.0/pygrab.egg-info/
--rw-rw-rw-   0        0        0      183 2023-05-31 05:44:57.000000 pygrab-0.1.0/pygrab.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      203 2023-05-31 05:44:57.000000 pygrab-0.1.0/pygrab.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-05-31 05:44:57.000000 pygrab-0.1.0/pygrab.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       19 2023-05-31 05:44:57.000000 pygrab-0.1.0/pygrab.egg-info/requires.txt
--rw-rw-rw-   0        0        0        7 2023-05-31 05:44:57.000000 pygrab-0.1.0/pygrab.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-05-31 05:44:58.107000 pygrab-0.1.0/setup.cfg
--rw-rw-rw-   0        0        0      338 2023-05-31 05:42:52.000000 pygrab-0.1.0/setup.py
+drwxrwxrwx   0        0        0        0 2023-06-12 05:44:03.458000 pygrab-0.1.1/
+-rw-rw-rw-   0        0        0      262 2023-06-12 05:44:03.451000 pygrab-0.1.1/PKG-INFO
+-rw-rw-rw-   0        0        0      341 2023-05-31 05:39:20.000000 pygrab-0.1.1/README.md
+drwxrwxrwx   0        0        0        0 2023-06-12 05:44:03.394000 pygrab-0.1.1/pygrab/
+-rw-rw-rw-   0        0        0       21 2023-05-30 03:16:15.000000 pygrab-0.1.1/pygrab/__init__.py
+-rw-rw-rw-   0        0        0    12049 2023-06-12 05:33:10.000000 pygrab-0.1.1/pygrab/pygrab.py
+drwxrwxrwx   0        0        0        0 2023-06-12 05:44:03.444000 pygrab-0.1.1/pygrab.egg-info/
+-rw-rw-rw-   0        0        0      262 2023-06-12 05:44:03.000000 pygrab-0.1.1/pygrab.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      203 2023-06-12 05:44:03.000000 pygrab-0.1.1/pygrab.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-06-12 05:44:03.000000 pygrab-0.1.1/pygrab.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       19 2023-06-12 05:44:03.000000 pygrab-0.1.1/pygrab.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        7 2023-06-12 05:44:03.000000 pygrab-0.1.1/pygrab.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-06-12 05:44:03.456000 pygrab-0.1.1/setup.cfg
+-rw-rw-rw-   0        0        0      338 2023-06-12 05:41:49.000000 pygrab-0.1.1/setup.py
```

### Comparing `pygrab-0.1.0/pygrab/pygrab.py` & `pygrab-0.1.1/pygrab/pygrab.py`

 * *Files 11% similar despite different names*

```diff
@@ -150,30 +150,76 @@
         **kwargs: Arbitrary keyword arguments to pass to the get function.
 
     Returns:
         list: A list of responses from the grabbed URLs.
     """
     # only import if async functionality is needed
     import threading as _threading
-    import time
+    import time as _time
     if type(urls) == str:
         return [get(urls, use_proxy=use_proxy, retries=retries, encoding=encoding, enable_js=enable_js, *args, **kwargs)]
 
     result = []
     threads = []
     for url in urls:
         threads.append(_threading.Thread(target=__grab_thread_wrapper, args=[url, result, args, kwargs, use_proxy, retries, enable_js]))
         threads[-1].start()
-        time.sleep(time_rest)
+        _time.sleep(time_rest)
     
     for thread in threads:
         thread.join()
         
     return result
 
+def download(url: str, name:str=None, use_proxy=False, retries=5) -> None:
+    if '.' not in url:
+        raise Exception("Argument 'url' needs a filepath extention")
+    
+
+    if name is not None:
+        if '.' not in name:
+            if '.' in url:
+                name += '.' + url.split('.')[-1]
+        elif name.split('.')[-1] != url.split('.')[-1]:
+            raise Exception ("File extentions for 'url' and 'name' must match.")
+    elif '/' in url:
+        name = url.split('/')[-1]
+    else:
+        name=url
+        
+
+    response = get(url, use_proxy=use_proxy, retries=retries)
+
+    if response.status_code == 200:
+        with open(name, 'wb') as f:
+            f.write(response.content)
+    else:
+        raise Exception(f"Error fetching url. Status code - {response.status_code}")
+
+def download_async(urls:list, names:list=None, use_proxy=False, retries=5, time_rest=0) -> None:
+    if names is not None:
+        if len(urls) != len(names):
+            raise Exception("Lists 'url' and 'name' must be of equal length.")
+    else:
+        names = [None for _ in range(len(urls))]
+
+    # only import if async functionality is needed
+    import threading as _threading
+    import time as _time
+
+    threads = []
+    for url, name in zip(urls, names):
+        threads.append(_threading.Thread(target=download, args=[url, name, use_proxy, retries]))
+        threads[-1].start()
+        _time.sleep(time_rest)
+    
+    for thread in threads:
+        thread.join()
+    
+
 def head(url, **kwargs):
     return _requests.head(url, **kwargs)
 
 def post(url:str, data=None, json=None, local_save_type:str=None, encoding:str='utf-8', **kwargs):
     local_file_starts = ['./', 'C:', '/'] 
     
     if any([url.startswith(i) for i in local_file_starts]):
```

