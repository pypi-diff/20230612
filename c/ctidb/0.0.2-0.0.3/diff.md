# Comparing `tmp/ctidb-0.0.2.tar.gz` & `tmp/ctidb-0.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist\ctidb-0.0.2.tar", last modified: Mon Jun 12 08:53:56 2023, max compression
+gzip compressed data, was "dist\ctidb-0.0.3.tar", last modified: Mon Jun 12 09:20:58 2023, max compression
```

## Comparing `ctidb-0.0.2.tar` & `ctidb-0.0.3.tar`

### file list

```diff
@@ -1,15 +1,14 @@
-drwxrwxrwx   0        0        0        0 2023-06-12 08:53:56.000000 ctidb-0.0.2/
--rw-rw-rw-   0        0        0     3571 2023-06-12 08:53:56.000000 ctidb-0.0.2/PKG-INFO
--rw-rw-rw-   0        0        0        8 2023-06-12 06:58:55.000000 ctidb-0.0.2/README.md
--rw-rw-rw-   0        0        0     2072 2023-06-12 08:38:13.000000 ctidb-0.0.2/README.rst
-drwxrwxrwx   0        0        0        0 2023-06-12 08:53:56.000000 ctidb-0.0.2/ctidb/
--rw-rw-rw-   0        0        0      436 2023-06-12 08:53:49.000000 ctidb-0.0.2/ctidb/__init__.py
--rw-rw-rw-   0        0        0    15647 2023-06-09 06:07:30.000000 ctidb-0.0.2/ctidb/reader.py
-drwxrwxrwx   0        0        0        0 2023-06-12 08:53:56.000000 ctidb-0.0.2/ctidb.egg-info/
--rw-rw-rw-   0        0        0     3571 2023-06-12 08:53:56.000000 ctidb-0.0.2/ctidb.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      207 2023-06-12 08:53:56.000000 ctidb-0.0.2/ctidb.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-06-12 08:53:56.000000 ctidb-0.0.2/ctidb.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        2 2023-06-12 05:52:23.000000 ctidb-0.0.2/ctidb.egg-info/not-zip-safe
--rw-rw-rw-   0        0        0        6 2023-06-12 08:53:56.000000 ctidb-0.0.2/ctidb.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-06-12 08:53:56.000000 ctidb-0.0.2/setup.cfg
--rw-rw-rw-   0        0        0     1762 2023-06-12 08:50:47.000000 ctidb-0.0.2/setup.py
+drwxrwxrwx   0        0        0        0 2023-06-12 09:20:58.000000 ctidb-0.0.3/
+-rw-rw-rw-   0        0        0     3202 2023-06-12 09:20:58.000000 ctidb-0.0.3/PKG-INFO
+-rw-rw-rw-   0        0        0     1766 2023-06-12 09:19:34.000000 ctidb-0.0.3/README.rst
+drwxrwxrwx   0        0        0        0 2023-06-12 09:20:58.000000 ctidb-0.0.3/ctidb/
+-rw-rw-rw-   0        0        0      436 2023-06-12 09:20:19.000000 ctidb-0.0.3/ctidb/__init__.py
+-rw-rw-rw-   0        0        0    15647 2023-06-12 09:07:31.000000 ctidb-0.0.3/ctidb/reader.py
+drwxrwxrwx   0        0        0        0 2023-06-12 09:20:58.000000 ctidb-0.0.3/ctidb.egg-info/
+-rw-rw-rw-   0        0        0     3202 2023-06-12 09:20:58.000000 ctidb-0.0.3/ctidb.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      197 2023-06-12 09:20:58.000000 ctidb-0.0.3/ctidb.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-06-12 09:20:58.000000 ctidb-0.0.3/ctidb.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        2 2023-06-12 09:11:31.000000 ctidb-0.0.3/ctidb.egg-info/not-zip-safe
+-rw-rw-rw-   0        0        0        6 2023-06-12 09:20:58.000000 ctidb-0.0.3/ctidb.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-06-12 09:20:58.000000 ctidb-0.0.3/setup.cfg
+-rw-rw-rw-   0        0        0     1762 2023-06-12 09:07:31.000000 ctidb-0.0.3/setup.py
```

### Comparing `ctidb-0.0.2/README.rst` & `ctidb-0.0.3/README.rst`

 * *Files 9% similar despite different names*

```diff
@@ -41,32 +41,25 @@
 
 **NOTE**:
 To look up an IP address, use the ``get`` method on this object. The method will return the
 corresponding values for the IP address from the database (e.g., a dictionary
 for GeoIP2/GeoLite2 databases). If the database does not contain a record for
 that IP address, the method will return ``None``.
 
-If you wish to also retrieve the prefix length for the record, use the
-``get_with_prefix_len`` method. This returns a tuple containing the record
-followed by the network prefix length associated with the record.
-
 Example
 -------
 
 .. code-block:: pycon
 
     >>> import ctidb
     >>>
     >>> with ctidb.CCtiReader('criminalip.ctidb') as reader:
     >>>
-    >>>     reader.get('152.216.7.110')
+    >>>     reader.get('223.26.31.75')
     {'country': ... }
-    >>>
-    >>>     reader.get_with_prefix_len('152.216.7.110')
-    ({'country': ... }, 24)
 
 Exceptions
 ----------
 
 The module will return an ``InvalidDatabaseError`` if the database is corrupt
 or otherwise invalid. A ``ValueError`` will be thrown if you look up an
 invalid IP address or an IPv6 address in an IPv4 database.
```

### Comparing `ctidb-0.0.2/ctidb/reader.py` & `ctidb-0.0.3/ctidb/reader.py`

 * *Files identical despite different names*

### Comparing `ctidb-0.0.2/setup.py` & `ctidb-0.0.3/setup.py`

 * *Files identical despite different names*

