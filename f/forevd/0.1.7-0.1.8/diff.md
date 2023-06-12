# Comparing `tmp/forevd-0.1.7.tar.gz` & `tmp/forevd-0.1.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "forevd-0.1.7.tar", max compression
+gzip compressed data, was "forevd-0.1.8.tar", max compression
```

## Comparing `forevd-0.1.7.tar` & `forevd-0.1.8.tar`

### file list

```diff
@@ -1,12 +1,12 @@
--rw-r--r--   0        0        0    11357 2023-06-06 22:07:52.728894 forevd-0.1.7/LICENSE
--rw-r--r--   0        0        0     4065 2023-06-06 22:07:52.732894 forevd-0.1.7/README.md
--rw-r--r--   0        0        0        0 2023-06-06 22:07:52.732894 forevd-0.1.7/forevd/__init__.py
--rw-r--r--   0        0        0     5879 2023-06-06 22:07:52.732894 forevd-0.1.7/forevd/__main__.py
--rw-r--r--   0        0        0     1543 2023-06-06 22:07:52.732894 forevd-0.1.7/forevd/apache/__init__.py
--rw-r--r--   0        0        0     4779 2023-06-06 22:07:52.732894 forevd-0.1.7/forevd/apache/httpd.conf
--rw-r--r--   0        0        0      216 2023-06-06 22:07:52.732894 forevd-0.1.7/forevd/app.py
--rw-r--r--   0        0        0        0 2023-06-06 22:07:52.732894 forevd-0.1.7/forevd/resources/__init__.py
--rw-r--r--   0        0        0        0 2023-06-06 22:07:52.732894 forevd-0.1.7/forevd/resources/logging/__init__.py
--rw-r--r--   0        0        0      387 2023-06-06 22:07:52.732894 forevd-0.1.7/forevd/resources/logging/cli.conf
--rw-r--r--   0        0        0      884 2023-06-06 22:07:52.732894 forevd-0.1.7/pyproject.toml
--rw-r--r--   0        0        0     4770 1970-01-01 00:00:00.000000 forevd-0.1.7/PKG-INFO
+-rw-r--r--   0        0        0    11357 2023-06-12 16:29:28.917774 forevd-0.1.8/LICENSE
+-rw-r--r--   0        0        0     4065 2023-06-12 16:29:28.917774 forevd-0.1.8/README.md
+-rw-r--r--   0        0        0        0 2023-06-12 16:29:28.921774 forevd-0.1.8/forevd/__init__.py
+-rw-r--r--   0        0        0     5879 2023-06-12 16:29:28.921774 forevd-0.1.8/forevd/__main__.py
+-rw-r--r--   0        0        0     1543 2023-06-12 16:29:28.921774 forevd-0.1.8/forevd/apache/__init__.py
+-rw-r--r--   0        0        0     4777 2023-06-12 16:29:28.921774 forevd-0.1.8/forevd/apache/httpd.conf
+-rw-r--r--   0        0        0      216 2023-06-12 16:29:28.921774 forevd-0.1.8/forevd/app.py
+-rw-r--r--   0        0        0        0 2023-06-12 16:29:28.921774 forevd-0.1.8/forevd/resources/__init__.py
+-rw-r--r--   0        0        0        0 2023-06-12 16:29:28.921774 forevd-0.1.8/forevd/resources/logging/__init__.py
+-rw-r--r--   0        0        0      387 2023-06-12 16:29:28.921774 forevd-0.1.8/forevd/resources/logging/cli.conf
+-rw-r--r--   0        0        0      884 2023-06-12 16:29:28.921774 forevd-0.1.8/pyproject.toml
+-rw-r--r--   0        0        0     4770 1970-01-01 00:00:00.000000 forevd-0.1.8/PKG-INFO
```

### Comparing `forevd-0.1.7/LICENSE` & `forevd-0.1.8/LICENSE`

 * *Files identical despite different names*

### Comparing `forevd-0.1.7/README.md` & `forevd-0.1.8/README.md`

 * *Files identical despite different names*

### Comparing `forevd-0.1.7/forevd/__main__.py` & `forevd-0.1.8/forevd/__main__.py`

 * *Files identical despite different names*

### Comparing `forevd-0.1.7/forevd/apache/__init__.py` & `forevd-0.1.8/forevd/apache/__init__.py`

 * *Files identical despite different names*

### Comparing `forevd-0.1.7/forevd/apache/httpd.conf` & `forevd-0.1.8/forevd/apache/httpd.conf`

 * *Files 2% similar despite different names*

```diff
@@ -122,15 +122,15 @@
     {% if "include" in location -%}
     {{ location["include"] }}
     {% endif -%}
 
     ProxyPass {{ location["backend"] }}
     ProxyPassReverse {{ location["backend"] }}
 
-    {% if "mtls" in location %}
+    {% if location["mtls"] %}
     SSLOptions +StdEnvVars
     SSLUserName SSL_CLIENT_S_DN_CN
     SSLVerifyCLient {{ location["mtls"] }}
 
     RequestHeader set X-Remote-User %{SSL_CLIENT_S_DN_CN}e
     RequestHeader set X-SSL-certificate "%{SSL_CLIENT_CERT}s" "expr=-n %{SSL_CLIENT_CERT}"
     {% endif %}
```

### Comparing `forevd-0.1.7/pyproject.toml` & `forevd-0.1.8/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "forevd"
-version = "0.1.7"
+version = "0.1.8"
 description = "Forward and reverse proxy using apache or nginx"
 authors = ["Erick Bourgeois <erick@jeb.ca>"]
 license = "LICENSE"
 readme = "README.md"
 
 [tool.poetry.dependencies]
 python = "^3.9"
```

### Comparing `forevd-0.1.7/PKG-INFO` & `forevd-0.1.8/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: forevd
-Version: 0.1.7
+Version: 0.1.8
 Summary: Forward and reverse proxy using apache or nginx
 License: LICENSE
 Author: Erick Bourgeois
 Author-email: erick@jeb.ca
 Requires-Python: >=3.9,<4.0
 Classifier: License :: Other/Proprietary License
 Classifier: Programming Language :: Python :: 3
```

