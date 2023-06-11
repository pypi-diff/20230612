# Comparing `tmp/coffeefetch-1.2.1.tar.gz` & `tmp/coffeefetch-1.2.2.tar.gz`

## Comparing `coffeefetch-1.2.1.tar` & `coffeefetch-1.2.2.tar`

### file list

```diff
@@ -1,9 +1,9 @@
--rw-r--r--   0        0        0       17 2020-02-02 00:00:00.000000 coffeefetch-1.2.1/requirements.txt
--rw-r--r--   0        0        0       35 2020-02-02 00:00:00.000000 coffeefetch-1.2.1/src/coffeefetch/__init__.py
--rw-r--r--   0        0        0      105 2020-02-02 00:00:00.000000 coffeefetch-1.2.1/src/coffeefetch/__main__.py
--rw-r--r--   0        0        0     5920 2020-02-02 00:00:00.000000 coffeefetch-1.2.1/src/coffeefetch/fetch.py
--rw-r--r--   0        0        0     1436 2020-02-02 00:00:00.000000 coffeefetch-1.2.1/src/coffeefetch/quotes/quotes.txt
--rw-r--r--   0        0        0     1091 2020-02-02 00:00:00.000000 coffeefetch-1.2.1/LICENCE
--rw-r--r--   0        0        0     1518 2020-02-02 00:00:00.000000 coffeefetch-1.2.1/README.md
--rw-r--r--   0        0        0      621 2020-02-02 00:00:00.000000 coffeefetch-1.2.1/pyproject.toml
--rw-r--r--   0        0        0     2010 2020-02-02 00:00:00.000000 coffeefetch-1.2.1/PKG-INFO
+-rw-r--r--   0        0        0       17 2020-02-02 00:00:00.000000 coffeefetch-1.2.2/requirements.txt
+-rw-r--r--   0        0        0       35 2020-02-02 00:00:00.000000 coffeefetch-1.2.2/src/coffeefetch/__init__.py
+-rw-r--r--   0        0        0      105 2020-02-02 00:00:00.000000 coffeefetch-1.2.2/src/coffeefetch/__main__.py
+-rw-r--r--   0        0        0     6377 2020-02-02 00:00:00.000000 coffeefetch-1.2.2/src/coffeefetch/fetch.py
+-rw-r--r--   0        0        0     1436 2020-02-02 00:00:00.000000 coffeefetch-1.2.2/src/coffeefetch/quotes/quotes.txt
+-rw-r--r--   0        0        0     1091 2020-02-02 00:00:00.000000 coffeefetch-1.2.2/LICENCE
+-rw-r--r--   0        0        0     1518 2020-02-02 00:00:00.000000 coffeefetch-1.2.2/README.md
+-rw-r--r--   0        0        0      621 2020-02-02 00:00:00.000000 coffeefetch-1.2.2/pyproject.toml
+-rw-r--r--   0        0        0     2010 2020-02-02 00:00:00.000000 coffeefetch-1.2.2/PKG-INFO
```

### Comparing `coffeefetch-1.2.1/src/coffeefetch/fetch.py` & `coffeefetch-1.2.2/src/coffeefetch/fetch.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 # TTY system information grabber, written in Python
 # Built to run on Unix-like systems, but may function on other systems
 # Written and tested by Logan Allen, 2023
 # PLEASE REPORT ANY ISSUES TO THE GITHUB REPOSITORY!!! www.github.com/TeaPixl
-from socket import gethostname, gethostbyname
 from platform import machine, system, processor, release
 from datetime import datetime
+import socket
 import psutil
 import logging
 import sys
 import time
 import getpass
 import shutil
 import random
@@ -27,14 +27,15 @@
                                   ██                ██  ██                              
                                   ██                ██████                              
                                     ██            ██                                    
                                 ████████████████████████                                
                                 ██                    ██                                
                                   ████████████████████"""
 
+# quote
 def quoteGen():
     try:
          path = os.path.dirname(__file__)
          realPath = "quotes/quotes.txt"
          location = os.path.join(path, realPath)
          with open(location, 'r') as f:
              quotes = [] # all quotes in list, randomly pick 1 out of 20
@@ -43,78 +44,97 @@
              chosen = random.choice(text)
              print("\n                             " + chosen)
     except Exception as e:
         logging.exception(e)
         print("\nQuoteGen failed... Proceeding.")
         pass
 
+# loading cursor
 def spinningCursor():
     try:
         while True:
             for cursor in "|/-\\":
                 yield cursor
     except Exception as e:
         logging.exception(e)
         print("spinningCursor failed... Proceeding.")
 
-def currentUser(): #current user
+# welcoming prompt
+def currentUser(): # current user
     user = getpass.getuser()
     print("Hello, " + user)
     
 def getTime():
     try:
         now = datetime.now()
         current_time = now.strftime("%H:%M:%S")
         print("It is: "+ current_time)
     except Exception as e:
         logging.exception(e)
         print("\nSomething's wrong, Unable to display the current time.")
         exit()
-        
+
+# sys. uptime
 def bootTime():
     return time.time() - psutil.boot_time()
 
 boot = bootTime()/60
 approxBoot = round(boot, 1)
 
+# get disk usage
 try:
     info = []
-    d = shutil.disk_usage("/") #tuple (total, used, free) *data in bytes
+    d = shutil.disk_usage("/") # tuple (total, used, free) *data in bytes
     info = list(d)
     info.pop(2)
     total = int(info[0]) / (1024 * 1024 * 1024)
     totalDisk = round(total, 1)
     used = int(info[1]) / (1024 * 1024 * 1024)
     usedDisk = round(used, 1)
     fraction = (usedDisk / totalDisk) *100
     newFraction = str(round(fraction, 1))
 except Exception as e:
     logging.exception(e)
     print("\nSomething went wrong while trying to access your disk.")
     exit()
 
+# get cpu freq.
 try:
     data = []
     cpuData = psutil.cpu_freq() # tuple (current, min, max)
     data = list(cpuData)
     floatFreq = int(data[0])/1000 #convert MHz to GHz
     freq = str(round(floatFreq, 2))
 except Exception as e:
     logging.exception(e)
     print("\nSomething went wrong while trying to access your CPU info.")
     exit()
 
+# get ip addr.
+try:
+    request = socket.socket(socket.AF_INET, socket.SOCK_DGRAM)
+    request.connect(("8.8.8.8", 80)) # connect to an addr. that is likely to be up
+    addr = request.getsockname()
+    ip = list(addr)
+    ip.pop(1)
+    realAddress = str(ip)[2:-2]
+except Exception as e:
+    logging.exception(e)
+    print("Failed to fetch socket name... Proceeding")
+    pass
+
+"""MAIN PROGRAM"""
 def main():
     try:
         data = [] # data fills list from 0-6
         data.append(str(system()))
         data.append(str(release()))
         data.append(str(machine()))
-        data.append(str(gethostname()))
-        data.append(str(gethostbyname(gethostname())))
+        data.append(str(socket.gethostname()))
+        data.append(realAddress)
         data.append(str(processor()))
         data.append(str(round(psutil.virtual_memory().total / (1024.0 **3)))+" GB") # total RAM
         usage = (psutil.virtual_memory()[2]) # RAM usage
         newUsage = str(round(usage))
         spinner = spinningCursor()
         for _ in range(7):
             sys.stdout.write(next(spinner))
@@ -137,9 +157,10 @@
         print("DISK:", newFraction + "% used / "+ str(totalDisk) +" GB total")
         print("*------------------------------*")
     except Exception as e:
         logging.exception(e)
         print("\nSomething has failed, please check for any issues!!!")
         exit()
 
+
 if __name__ == "__main__":
     main()
```

### Comparing `coffeefetch-1.2.1/src/coffeefetch/quotes/quotes.txt` & `coffeefetch-1.2.2/src/coffeefetch/quotes/quotes.txt`

 * *Files identical despite different names*

### Comparing `coffeefetch-1.2.1/LICENCE` & `coffeefetch-1.2.2/LICENCE`

 * *Files identical despite different names*

### Comparing `coffeefetch-1.2.1/README.md` & `coffeefetch-1.2.2/README.md`

 * *Files identical despite different names*

### Comparing `coffeefetch-1.2.1/pyproject.toml` & `coffeefetch-1.2.2/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["hatchling"]
 build-backend = "hatchling.build"
 
 [project]
 name = "coffeefetch"
-version = "1.2.1"
+version = "1.2.2"
 authors = [
   { name="Logan Allen", email="ltallen392@gmail.com" },
 ]
 description = "A lightweight system information grabber written in Python"
 readme = "README.md"
 requires-python = ">=3.7"
 classifiers = [
```

### Comparing `coffeefetch-1.2.1/PKG-INFO` & `coffeefetch-1.2.2/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: coffeefetch
-Version: 1.2.1
+Version: 1.2.2
 Summary: A lightweight system information grabber written in Python
 Project-URL: Homepage, https://github.com/TeaPixl/CoffeeFetch
 Project-URL: Bug Tracker, https://github.com/TeaPixl/CoffeeFetch/issues
 Author-email: Logan Allen <ltallen392@gmail.com>
 License-File: LICENCE
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: POSIX :: Linux
```

