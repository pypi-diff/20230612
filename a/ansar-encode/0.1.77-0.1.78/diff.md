# Comparing `tmp/ansar-encode-0.1.77.tar.gz` & `tmp/ansar-encode-0.1.78.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ansar-encode-0.1.77.tar", last modified: Mon May 22 09:53:30 2023, max compression
+gzip compressed data, was "ansar-encode-0.1.78.tar", last modified: Mon Jun 12 06:34:35 2023, max compression
```

## Comparing `ansar-encode-0.1.77.tar` & `ansar-encode-0.1.78.tar`

### file list

```diff
@@ -1,31 +1,31 @@
-drwxrwxr-x   0 scott     (1000) scott     (1000)        0 2023-05-22 09:53:30.870462 ansar-encode-0.1.77/
--rw-rw-r--   0 scott     (1000) scott     (1000)     1106 2023-04-19 07:09:52.000000 ansar-encode-0.1.77/LICENSE
--rw-rw-r--   0 scott     (1000) scott     (1000)     1482 2023-05-22 09:53:30.870462 ansar-encode-0.1.77/PKG-INFO
--rw-rw-r--   0 scott     (1000) scott     (1000)      830 2023-04-19 07:09:52.000000 ansar-encode-0.1.77/README.md
--rw-rw-r--   0 scott     (1000) scott     (1000)      309 2023-04-19 07:09:52.000000 ansar-encode-0.1.77/pyproject.toml
--rw-rw-r--   0 scott     (1000) scott     (1000)       38 2023-05-22 09:53:30.870462 ansar-encode-0.1.77/setup.cfg
--rw-rw-r--   0 scott     (1000) scott     (1000)     1971 2023-04-19 07:09:52.000000 ansar-encode-0.1.77/setup.py
-drwxrwxr-x   0 scott     (1000) scott     (1000)        0 2023-05-22 09:53:30.870462 ansar-encode-0.1.77/src/
-drwxrwxr-x   0 scott     (1000) scott     (1000)        0 2023-05-22 09:53:30.870462 ansar-encode-0.1.77/src/ansar/
-drwxrwxr-x   0 scott     (1000) scott     (1000)        0 2023-05-22 09:53:30.870462 ansar-encode-0.1.77/src/ansar/command/
--rw-rw-r--   0 scott     (1000) scott     (1000)    12104 2023-04-19 07:09:52.000000 ansar-encode-0.1.77/src/ansar/command/show_release.py
-drwxrwxr-x   0 scott     (1000) scott     (1000)        0 2023-05-22 09:53:30.870462 ansar-encode-0.1.77/src/ansar/encode/
--rw-rw-r--   0 scott     (1000) scott     (1000)     4931 2023-05-22 09:53:27.000000 ansar-encode-0.1.77/src/ansar/encode/__init__.py
--rw-rw-r--   0 scott     (1000) scott     (1000)    37139 2023-04-19 07:09:52.000000 ansar-encode-0.1.77/src/ansar/encode/codec.py
--rw-rw-r--   0 scott     (1000) scott     (1000)    16843 2023-04-19 07:09:52.000000 ansar-encode-0.1.77/src/ansar/encode/convert.py
--rw-rw-r--   0 scott     (1000) scott     (1000)    11271 2023-05-22 09:25:36.000000 ansar-encode-0.1.77/src/ansar/encode/file.py
--rw-rw-r--   0 scott     (1000) scott     (1000)    19680 2023-05-22 09:46:06.000000 ansar-encode-0.1.77/src/ansar/encode/folder.py
--rw-rw-r--   0 scott     (1000) scott     (1000)     3719 2023-04-19 07:09:52.000000 ansar-encode-0.1.77/src/ansar/encode/json.py
--rw-rw-r--   0 scott     (1000) scott     (1000)    33766 2023-04-19 07:09:52.000000 ansar-encode-0.1.77/src/ansar/encode/message.py
--rw-rw-r--   0 scott     (1000) scott     (1000)    10956 2023-04-19 07:09:52.000000 ansar-encode-0.1.77/src/ansar/encode/portable.py
--rw-rw-r--   0 scott     (1000) scott     (1000)     3334 2023-04-19 07:09:52.000000 ansar-encode-0.1.77/src/ansar/encode/release.py
--rw-rw-r--   0 scott     (1000) scott     (1000)     6244 2023-04-29 20:35:19.000000 ansar-encode-0.1.77/src/ansar/encode/runtime.py
--rw-rw-r--   0 scott     (1000) scott     (1000)     1814 2023-04-19 07:09:52.000000 ansar-encode-0.1.77/src/ansar/encode/version.py
--rw-rw-r--   0 scott     (1000) scott     (1000)    11517 2023-04-19 07:09:52.000000 ansar-encode-0.1.77/src/ansar/encode/xml.py
-drwxrwxr-x   0 scott     (1000) scott     (1000)        0 2023-05-22 09:53:30.870462 ansar-encode-0.1.77/src/ansar_encode.egg-info/
--rw-rw-r--   0 scott     (1000) scott     (1000)     1482 2023-05-22 09:53:30.000000 ansar-encode-0.1.77/src/ansar_encode.egg-info/PKG-INFO
--rw-rw-r--   0 scott     (1000) scott     (1000)      642 2023-05-22 09:53:30.000000 ansar-encode-0.1.77/src/ansar_encode.egg-info/SOURCES.txt
--rw-rw-r--   0 scott     (1000) scott     (1000)        1 2023-05-22 09:53:30.000000 ansar-encode-0.1.77/src/ansar_encode.egg-info/dependency_links.txt
--rw-rw-r--   0 scott     (1000) scott     (1000)       68 2023-05-22 09:53:30.000000 ansar-encode-0.1.77/src/ansar_encode.egg-info/entry_points.txt
--rw-rw-r--   0 scott     (1000) scott     (1000)       41 2023-05-22 09:53:30.000000 ansar-encode-0.1.77/src/ansar_encode.egg-info/requires.txt
--rw-rw-r--   0 scott     (1000) scott     (1000)        6 2023-05-22 09:53:30.000000 ansar-encode-0.1.77/src/ansar_encode.egg-info/top_level.txt
+drwxrwxr-x   0 scott     (1000) scott     (1000)        0 2023-06-12 06:34:35.356512 ansar-encode-0.1.78/
+-rw-rw-r--   0 scott     (1000) scott     (1000)     1106 2023-04-19 07:09:52.000000 ansar-encode-0.1.78/LICENSE
+-rw-rw-r--   0 scott     (1000) scott     (1000)     1482 2023-06-12 06:34:35.356512 ansar-encode-0.1.78/PKG-INFO
+-rw-rw-r--   0 scott     (1000) scott     (1000)      830 2023-04-19 07:09:52.000000 ansar-encode-0.1.78/README.md
+-rw-rw-r--   0 scott     (1000) scott     (1000)      309 2023-04-19 07:09:52.000000 ansar-encode-0.1.78/pyproject.toml
+-rw-rw-r--   0 scott     (1000) scott     (1000)       38 2023-06-12 06:34:35.356512 ansar-encode-0.1.78/setup.cfg
+-rw-rw-r--   0 scott     (1000) scott     (1000)     1971 2023-04-19 07:09:52.000000 ansar-encode-0.1.78/setup.py
+drwxrwxr-x   0 scott     (1000) scott     (1000)        0 2023-06-12 06:34:35.356512 ansar-encode-0.1.78/src/
+drwxrwxr-x   0 scott     (1000) scott     (1000)        0 2023-06-12 06:34:35.356512 ansar-encode-0.1.78/src/ansar/
+drwxrwxr-x   0 scott     (1000) scott     (1000)        0 2023-06-12 06:34:35.356512 ansar-encode-0.1.78/src/ansar/command/
+-rw-rw-r--   0 scott     (1000) scott     (1000)    12104 2023-04-19 07:09:52.000000 ansar-encode-0.1.78/src/ansar/command/show_release.py
+drwxrwxr-x   0 scott     (1000) scott     (1000)        0 2023-06-12 06:34:35.356512 ansar-encode-0.1.78/src/ansar/encode/
+-rw-rw-r--   0 scott     (1000) scott     (1000)     4943 2023-06-12 06:34:32.000000 ansar-encode-0.1.78/src/ansar/encode/__init__.py
+-rw-rw-r--   0 scott     (1000) scott     (1000)    37139 2023-04-19 07:09:52.000000 ansar-encode-0.1.78/src/ansar/encode/codec.py
+-rw-rw-r--   0 scott     (1000) scott     (1000)    16843 2023-04-19 07:09:52.000000 ansar-encode-0.1.78/src/ansar/encode/convert.py
+-rw-rw-r--   0 scott     (1000) scott     (1000)    11271 2023-05-22 09:25:36.000000 ansar-encode-0.1.78/src/ansar/encode/file.py
+-rw-rw-r--   0 scott     (1000) scott     (1000)    19680 2023-05-22 09:46:06.000000 ansar-encode-0.1.78/src/ansar/encode/folder.py
+-rw-rw-r--   0 scott     (1000) scott     (1000)     3719 2023-04-19 07:09:52.000000 ansar-encode-0.1.78/src/ansar/encode/json.py
+-rw-rw-r--   0 scott     (1000) scott     (1000)    33766 2023-04-19 07:09:52.000000 ansar-encode-0.1.78/src/ansar/encode/message.py
+-rw-rw-r--   0 scott     (1000) scott     (1000)    10956 2023-04-19 07:09:52.000000 ansar-encode-0.1.78/src/ansar/encode/portable.py
+-rw-rw-r--   0 scott     (1000) scott     (1000)     3334 2023-04-19 07:09:52.000000 ansar-encode-0.1.78/src/ansar/encode/release.py
+-rw-rw-r--   0 scott     (1000) scott     (1000)     6335 2023-06-12 06:19:56.000000 ansar-encode-0.1.78/src/ansar/encode/runtime.py
+-rw-rw-r--   0 scott     (1000) scott     (1000)     1814 2023-04-19 07:09:52.000000 ansar-encode-0.1.78/src/ansar/encode/version.py
+-rw-rw-r--   0 scott     (1000) scott     (1000)    11517 2023-04-19 07:09:52.000000 ansar-encode-0.1.78/src/ansar/encode/xml.py
+drwxrwxr-x   0 scott     (1000) scott     (1000)        0 2023-06-12 06:34:35.356512 ansar-encode-0.1.78/src/ansar_encode.egg-info/
+-rw-rw-r--   0 scott     (1000) scott     (1000)     1482 2023-06-12 06:34:35.000000 ansar-encode-0.1.78/src/ansar_encode.egg-info/PKG-INFO
+-rw-rw-r--   0 scott     (1000) scott     (1000)      642 2023-06-12 06:34:35.000000 ansar-encode-0.1.78/src/ansar_encode.egg-info/SOURCES.txt
+-rw-rw-r--   0 scott     (1000) scott     (1000)        1 2023-06-12 06:34:35.000000 ansar-encode-0.1.78/src/ansar_encode.egg-info/dependency_links.txt
+-rw-rw-r--   0 scott     (1000) scott     (1000)       68 2023-06-12 06:34:35.000000 ansar-encode-0.1.78/src/ansar_encode.egg-info/entry_points.txt
+-rw-rw-r--   0 scott     (1000) scott     (1000)       41 2023-06-12 06:34:35.000000 ansar-encode-0.1.78/src/ansar_encode.egg-info/requires.txt
+-rw-rw-r--   0 scott     (1000) scott     (1000)        6 2023-06-12 06:34:35.000000 ansar-encode-0.1.78/src/ansar_encode.egg-info/top_level.txt
```

### Comparing `ansar-encode-0.1.77/LICENSE` & `ansar-encode-0.1.78/LICENSE`

 * *Files identical despite different names*

### Comparing `ansar-encode-0.1.77/PKG-INFO` & `ansar-encode-0.1.78/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ansar-encode
-Version: 0.1.77
+Version: 0.1.78
 Summary: Persistence of complex application data
 Author: Scott Woods
 Author-email: Scott Woods <scott.suzuki@gmail.com>
 Project-URL: Documentation, http://ansar-encode-manual.s3-website-ap-southeast-2.amazonaws.com/0.1.1
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Developers
 Classifier: Programming Language :: Python :: 3
```

### Comparing `ansar-encode-0.1.77/README.md` & `ansar-encode-0.1.78/README.md`

 * *Files identical despite different names*

### Comparing `ansar-encode-0.1.77/setup.py` & `ansar-encode-0.1.78/setup.py`

 * *Files identical despite different names*

### Comparing `ansar-encode-0.1.77/src/ansar/command/show_release.py` & `ansar-encode-0.1.78/src/ansar/command/show_release.py`

 * *Files identical despite different names*

### Comparing `ansar-encode-0.1.77/src/ansar/encode/__init__.py` & `ansar-encode-0.1.78/src/ansar/encode/__init__.py`

 * *Files 3% similar despite different names*

```diff
@@ -21,16 +21,16 @@
 # OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE
 # SOFTWARE.
 
 """Persistence of complex application data.
 
 Repo: git@github.com:mr-ansar/ansar-encode.git
 Branch: main
-Commit: e9552778e711a638a9c22dd7006f8ee06fd28ca6
-Version: 0.1.76 (2023-05-22@21:53:27+NZST)
+Commit: 9b1b58561ae82d48307c62377790e60ab3773aa3
+Version: 0.1.77 (2023-06-12@18:34:32+NZST)
 """
 
 from .portable import Boolean
 from .portable import Byte, Character, Rune
 from .portable import Integer2, Integer4, Integer8
 from .portable import Unsigned2, Unsigned4, Unsigned8
 from .portable import Float4, Float8
@@ -49,15 +49,15 @@
 from .portable import is_portable, is_container, is_structural, is_portable_class, is_container_class
 from .portable import NO_SUCH_ADDRESS
 from .portable import is_address, address_on_proxy
 from .portable import deque
 
 from .runtime import USER_LOG_FAULT, USER_LOG_WARNING, USER_LOG_CONSOLE, USER_LOG_OBJECT, USER_LOG_TRACE, USER_LOG_DEBUG, USER_LOG_NONE
 from .runtime import TAG_CREATED, TAG_DESTROYED, TAG_SENT, TAG_RECEIVED, TAG_STARTED, TAG_ENDED
-from .runtime import TAG_FAULT, TAG_WARNING, TAG_CONSOLE, TAG_TRACE, TAG_DEBUG, TAG_CHECK
+from .runtime import TAG_FAULT, TAG_WARNING, TAG_CONSOLE, TAG_TRACE, TAG_DEBUG, TAG_CHECK, TAG_SAMPLE
 from .runtime import tag_to_number
 from .runtime import Runtime
 from .runtime import CodingProblem, PlatformFailure
 
 from .message import MessageError, MessageRegistrationError
 from .message import Message, is_message, is_message_class
 from .message import Unknown, Incognito
```

### Comparing `ansar-encode-0.1.77/src/ansar/encode/codec.py` & `ansar-encode-0.1.78/src/ansar/encode/codec.py`

 * *Files identical despite different names*

### Comparing `ansar-encode-0.1.77/src/ansar/encode/convert.py` & `ansar-encode-0.1.78/src/ansar/encode/convert.py`

 * *Files identical despite different names*

### Comparing `ansar-encode-0.1.77/src/ansar/encode/file.py` & `ansar-encode-0.1.78/src/ansar/encode/file.py`

 * *Files identical despite different names*

### Comparing `ansar-encode-0.1.77/src/ansar/encode/folder.py` & `ansar-encode-0.1.78/src/ansar/encode/folder.py`

 * *Files identical despite different names*

### Comparing `ansar-encode-0.1.77/src/ansar/encode/json.py` & `ansar-encode-0.1.78/src/ansar/encode/json.py`

 * *Files identical despite different names*

### Comparing `ansar-encode-0.1.77/src/ansar/encode/message.py` & `ansar-encode-0.1.78/src/ansar/encode/message.py`

 * *Files identical despite different names*

### Comparing `ansar-encode-0.1.77/src/ansar/encode/portable.py` & `ansar-encode-0.1.78/src/ansar/encode/portable.py`

 * *Files identical despite different names*

### Comparing `ansar-encode-0.1.77/src/ansar/encode/release.py` & `ansar-encode-0.1.78/src/ansar/encode/release.py`

 * *Files identical despite different names*

### Comparing `ansar-encode-0.1.77/src/ansar/encode/runtime.py` & `ansar-encode-0.1.78/src/ansar/encode/runtime.py`

 * *Files 3% similar despite different names*

```diff
@@ -51,14 +51,15 @@
     'TAG_ENDED',
 
     'TAG_FAULT',
     'TAG_WARNING',
     'TAG_CONSOLE',
     'TAG_TRACE',
     'TAG_DEBUG',
+    'TAG_SAMPLE',
     'TAG_CHECK',
 
     'tag_to_number',
 
     'Runtime',
     'CodingProblem',
     'PlatformFailure',
@@ -87,20 +88,21 @@
 TAG_FAULT     = '!'     # Compromised.
 TAG_WARNING   = '?'     # May be compromised.
 TAG_CONSOLE   = '^'     # Application milestone.
 
 TAG_TRACE     = '~'     # Technical, networks, files and devices.
 TAG_DEBUG     = '_'     # Developer, raw.
 
+TAG_SAMPLE    = '&'		# Sample of local data.
 TAG_CHECK     = '='		# Check a condition.
 
 TAG_LEVEL = {
     TAG_FAULT: USER_LOG_FAULT,
     TAG_WARNING: USER_LOG_WARNING, TAG_CHECK: USER_LOG_WARNING,
-    TAG_CONSOLE: USER_LOG_CONSOLE,
+    TAG_CONSOLE: USER_LOG_CONSOLE, TAG_SAMPLE: USER_LOG_TRACE,
     TAG_CREATED: USER_LOG_OBJECT, TAG_DESTROYED: USER_LOG_OBJECT, TAG_SENT: USER_LOG_OBJECT, TAG_RECEIVED: USER_LOG_OBJECT,
     TAG_STARTED: USER_LOG_OBJECT, TAG_ENDED: USER_LOG_OBJECT,
     TAG_TRACE: USER_LOG_TRACE,
     TAG_DEBUG: USER_LOG_DEBUG
 }
 
 def tag_to_number(tag):
```

### Comparing `ansar-encode-0.1.77/src/ansar/encode/version.py` & `ansar-encode-0.1.78/src/ansar/encode/version.py`

 * *Files identical despite different names*

### Comparing `ansar-encode-0.1.77/src/ansar/encode/xml.py` & `ansar-encode-0.1.78/src/ansar/encode/xml.py`

 * *Files identical despite different names*

### Comparing `ansar-encode-0.1.77/src/ansar_encode.egg-info/PKG-INFO` & `ansar-encode-0.1.78/src/ansar_encode.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ansar-encode
-Version: 0.1.77
+Version: 0.1.78
 Summary: Persistence of complex application data
 Author: Scott Woods
 Author-email: Scott Woods <scott.suzuki@gmail.com>
 Project-URL: Documentation, http://ansar-encode-manual.s3-website-ap-southeast-2.amazonaws.com/0.1.1
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Developers
 Classifier: Programming Language :: Python :: 3
```

### Comparing `ansar-encode-0.1.77/src/ansar_encode.egg-info/SOURCES.txt` & `ansar-encode-0.1.78/src/ansar_encode.egg-info/SOURCES.txt`

 * *Files identical despite different names*

