# Comparing `tmp/pyclickhouse3-0.9.34.tar.gz` & `tmp/pyclickhouse3-0.9.35.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pyclickhouse3-0.9.34.tar", last modified: Mon May 15 08:03:29 2023, max compression
+gzip compressed data, was "pyclickhouse3-0.9.35.tar", last modified: Mon Jun 12 12:44:37 2023, max compression
```

## Comparing `pyclickhouse3-0.9.34.tar` & `pyclickhouse3-0.9.35.tar`

### file list

```diff
@@ -1,25 +1,25 @@
-drwxr-xr-x   0 mfridental  (1001) clickhouse   (135)        0 2023-05-15 08:03:29.282693 pyclickhouse3-0.9.34/
--rwxr-xr-x   0 mfridental  (1001) clickhouse   (135)    11357 2021-02-10 13:45:49.000000 pyclickhouse3-0.9.34/LICENSE
--rw-r--r--   0 mfridental  (1001) clickhouse   (135)      463 2023-05-15 08:03:29.282693 pyclickhouse3-0.9.34/PKG-INFO
--rwxr-xr-x   0 mfridental  (1001) clickhouse   (135)     1779 2021-02-10 13:45:49.000000 pyclickhouse3-0.9.34/README.md
-drwxr-xr-x   0 mfridental  (1001) clickhouse   (135)        0 2023-05-15 08:03:29.282693 pyclickhouse3-0.9.34/pyclickhouse/
--rwxr-xr-x   0 mfridental  (1001) clickhouse   (135)     8887 2022-05-20 10:07:52.000000 pyclickhouse3-0.9.34/pyclickhouse/Connection.py
--rwxr-xr-x   0 mfridental  (1001) clickhouse   (135)    25465 2023-01-23 16:34:27.000000 pyclickhouse3-0.9.34/pyclickhouse/Cursor.py
--rwxr-xr-x   0 mfridental  (1001) clickhouse   (135)     3702 2021-09-29 15:05:05.000000 pyclickhouse3-0.9.34/pyclickhouse/FilterableCache.py
--rwxr-xr-x   0 mfridental  (1001) clickhouse   (135)       61 2021-02-10 13:45:49.000000 pyclickhouse3-0.9.34/pyclickhouse/__init__.py
--rwxr-xr-x   0 mfridental  (1001) clickhouse   (135)    23706 2023-05-15 08:02:24.000000 pyclickhouse3-0.9.34/pyclickhouse/formatter.py
-drwxr-xr-x   0 mfridental  (1001) clickhouse   (135)        0 2023-05-15 08:03:29.282693 pyclickhouse3-0.9.34/pyclickhouse3.egg-info/
--rw-r--r--   0 mfridental  (1001) clickhouse   (135)      463 2023-05-15 08:03:29.000000 pyclickhouse3-0.9.34/pyclickhouse3.egg-info/PKG-INFO
--rw-r--r--   0 mfridental  (1001) clickhouse   (135)      485 2023-05-15 08:03:29.000000 pyclickhouse3-0.9.34/pyclickhouse3.egg-info/SOURCES.txt
--rw-r--r--   0 mfridental  (1001) clickhouse   (135)        1 2023-05-15 08:03:29.000000 pyclickhouse3-0.9.34/pyclickhouse3.egg-info/dependency_links.txt
--rw-r--r--   0 mfridental  (1001) clickhouse   (135)        1 2021-02-10 13:40:28.000000 pyclickhouse3-0.9.34/pyclickhouse3.egg-info/not-zip-safe
--rw-r--r--   0 mfridental  (1001) clickhouse   (135)       25 2023-05-15 08:03:29.000000 pyclickhouse3-0.9.34/pyclickhouse3.egg-info/requires.txt
--rw-r--r--   0 mfridental  (1001) clickhouse   (135)       13 2023-05-15 08:03:29.000000 pyclickhouse3-0.9.34/pyclickhouse3.egg-info/top_level.txt
--rw-r--r--   0 mfridental  (1001) clickhouse   (135)      103 2021-02-10 13:45:49.000000 pyclickhouse3-0.9.34/pyproject.toml
--rwxr-xr-x   0 mfridental  (1001) clickhouse   (135)       79 2023-05-15 08:03:29.282693 pyclickhouse3-0.9.34/setup.cfg
--rwxr-xr-x   0 mfridental  (1001) clickhouse   (135)      683 2023-05-15 08:02:42.000000 pyclickhouse3-0.9.34/setup.py
-drwxr-xr-x   0 mfridental  (1001) clickhouse   (135)        0 2023-05-15 08:03:29.282693 pyclickhouse3-0.9.34/test/
--rwxr-xr-x   0 mfridental  (1001) clickhouse   (135)     1560 2023-01-23 10:37:59.000000 pyclickhouse3-0.9.34/test/test_compatibility.py
--rwxr-xr-x   0 mfridental  (1001) clickhouse   (135)     2613 2023-01-23 14:27:59.000000 pyclickhouse3-0.9.34/test/test_map.py
--rwxr-xr-x   0 mfridental  (1001) clickhouse   (135)    10330 2023-01-26 12:08:31.000000 pyclickhouse3-0.9.34/test/test_new.py
--rwxr-xr-x   0 mfridental  (1001) clickhouse   (135)     4759 2023-01-23 10:49:05.000000 pyclickhouse3-0.9.34/test/test_simple.py
+drwxr-xr-x   0 mfridental  (1001) clickhouse   (135)        0 2023-06-12 12:44:37.760345 pyclickhouse3-0.9.35/
+-rwxr-xr-x   0 mfridental  (1001) clickhouse   (135)    11357 2021-02-10 13:45:49.000000 pyclickhouse3-0.9.35/LICENSE
+-rw-r--r--   0 mfridental  (1001) clickhouse   (135)      463 2023-06-12 12:44:37.760345 pyclickhouse3-0.9.35/PKG-INFO
+-rwxr-xr-x   0 mfridental  (1001) clickhouse   (135)     1779 2021-02-10 13:45:49.000000 pyclickhouse3-0.9.35/README.md
+drwxr-xr-x   0 mfridental  (1001) clickhouse   (135)        0 2023-06-12 12:44:37.756345 pyclickhouse3-0.9.35/pyclickhouse/
+-rwxr-xr-x   0 mfridental  (1001) clickhouse   (135)     8887 2022-05-20 10:07:52.000000 pyclickhouse3-0.9.35/pyclickhouse/Connection.py
+-rwxr-xr-x   0 mfridental  (1001) clickhouse   (135)    25465 2023-01-23 16:34:27.000000 pyclickhouse3-0.9.35/pyclickhouse/Cursor.py
+-rwxr-xr-x   0 mfridental  (1001) clickhouse   (135)     3702 2021-09-29 15:05:05.000000 pyclickhouse3-0.9.35/pyclickhouse/FilterableCache.py
+-rwxr-xr-x   0 mfridental  (1001) clickhouse   (135)       61 2021-02-10 13:45:49.000000 pyclickhouse3-0.9.35/pyclickhouse/__init__.py
+-rwxr-xr-x   0 mfridental  (1001) clickhouse   (135)    24944 2023-06-12 12:37:31.000000 pyclickhouse3-0.9.35/pyclickhouse/formatter.py
+drwxr-xr-x   0 mfridental  (1001) clickhouse   (135)        0 2023-06-12 12:44:37.760345 pyclickhouse3-0.9.35/pyclickhouse3.egg-info/
+-rw-r--r--   0 mfridental  (1001) clickhouse   (135)      463 2023-06-12 12:44:37.000000 pyclickhouse3-0.9.35/pyclickhouse3.egg-info/PKG-INFO
+-rw-r--r--   0 mfridental  (1001) clickhouse   (135)      485 2023-06-12 12:44:37.000000 pyclickhouse3-0.9.35/pyclickhouse3.egg-info/SOURCES.txt
+-rw-r--r--   0 mfridental  (1001) clickhouse   (135)        1 2023-06-12 12:44:37.000000 pyclickhouse3-0.9.35/pyclickhouse3.egg-info/dependency_links.txt
+-rw-r--r--   0 mfridental  (1001) clickhouse   (135)        1 2021-02-10 13:40:28.000000 pyclickhouse3-0.9.35/pyclickhouse3.egg-info/not-zip-safe
+-rw-r--r--   0 mfridental  (1001) clickhouse   (135)       25 2023-06-12 12:44:37.000000 pyclickhouse3-0.9.35/pyclickhouse3.egg-info/requires.txt
+-rw-r--r--   0 mfridental  (1001) clickhouse   (135)       13 2023-06-12 12:44:37.000000 pyclickhouse3-0.9.35/pyclickhouse3.egg-info/top_level.txt
+-rw-r--r--   0 mfridental  (1001) clickhouse   (135)      103 2021-02-10 13:45:49.000000 pyclickhouse3-0.9.35/pyproject.toml
+-rwxr-xr-x   0 mfridental  (1001) clickhouse   (135)       79 2023-06-12 12:44:37.760345 pyclickhouse3-0.9.35/setup.cfg
+-rwxr-xr-x   0 mfridental  (1001) clickhouse   (135)      683 2023-06-12 12:43:38.000000 pyclickhouse3-0.9.35/setup.py
+drwxr-xr-x   0 mfridental  (1001) clickhouse   (135)        0 2023-06-12 12:44:37.760345 pyclickhouse3-0.9.35/test/
+-rwxr-xr-x   0 mfridental  (1001) clickhouse   (135)     1560 2023-01-23 10:37:59.000000 pyclickhouse3-0.9.35/test/test_compatibility.py
+-rwxr-xr-x   0 mfridental  (1001) clickhouse   (135)     2613 2023-01-23 14:27:59.000000 pyclickhouse3-0.9.35/test/test_map.py
+-rwxr-xr-x   0 mfridental  (1001) clickhouse   (135)    10653 2023-06-12 12:42:08.000000 pyclickhouse3-0.9.35/test/test_new.py
+-rwxr-xr-x   0 mfridental  (1001) clickhouse   (135)     4759 2023-01-23 10:49:05.000000 pyclickhouse3-0.9.35/test/test_simple.py
```

### Comparing `pyclickhouse3-0.9.34/LICENSE` & `pyclickhouse3-0.9.35/LICENSE`

 * *Files identical despite different names*

### Comparing `pyclickhouse3-0.9.34/README.md` & `pyclickhouse3-0.9.35/README.md`

 * *Files identical despite different names*

### Comparing `pyclickhouse3-0.9.34/pyclickhouse/Connection.py` & `pyclickhouse3-0.9.35/pyclickhouse/Connection.py`

 * *Files identical despite different names*

### Comparing `pyclickhouse3-0.9.34/pyclickhouse/Cursor.py` & `pyclickhouse3-0.9.35/pyclickhouse/Cursor.py`

 * *Files identical despite different names*

### Comparing `pyclickhouse3-0.9.34/pyclickhouse/FilterableCache.py` & `pyclickhouse3-0.9.35/pyclickhouse/FilterableCache.py`

 * *Files identical despite different names*

### Comparing `pyclickhouse3-0.9.34/pyclickhouse/formatter.py` & `pyclickhouse3-0.9.35/pyclickhouse/formatter.py`

 * *Files 3% similar despite different names*

```diff
@@ -331,14 +331,25 @@
                     escaped = '0000-00-00 00:00:00'
                 else:
                     escaped = '%04d-%02d-%02d %02d:%02d:%02d' % (value.year, value.month, value.day, value.hour, value.minute, value.second)
                 if inarray:
                     return "'%s'" % escaped
                 else:
                     return escaped
+            if type == 'DateTime64' or type.startswith('DateTime64('):
+                if value is None or value.replace(tzinfo=None) <= dt.datetime(1970,1,2,0,0,0):
+                    escaped = '0000-00-00 00:00:00,000'
+                else:
+                    escaped = '%04d-%02d-%02d %02d:%02d:%02d.%03d' % (value.year, value.month, value.day, value.hour,
+                                                                  value.minute, value.second,
+                                                                      int(value.microsecond/1000))
+                if inarray:
+                    return "'%s'" % escaped
+                else:
+                    return escaped
             if 'Array' in type:
                 if value is None:
                     return '[]'
                 return '[%s]' % ','.join([self.formatfield(x, type[6:-1], name, True) for x in value])
             if type.startswith('Map(') and type.endswith(')'):
                 if value is None:
                     return '{}'
@@ -388,14 +399,25 @@
                 value = value[:-1]
             if value == '0000-00-00 00:00:00' or value == '1970-01-01 86:28:16':
                 return None
             tmp = dt.datetime.strptime(value, '%Y-%m-%d %H:%M:%S')
             if type.startswith('DateTime('):
                 tmp = tmp.replace(tzinfo=tz.gettz(type.split('(')[1][2:-3]))
             return tmp
+        if type == 'DateTime64' or type.startswith('DateTime64('):
+            if value.startswith("'"):
+                value = value[1:]
+            if value.endswith("'"):
+                value = value[:-1]
+            if value.startswith('0000-00-00 00:00:00') or value.startswith('1970-01-01 86:28:16'):
+                return None
+            tmp = dt.datetime.strptime(value, '%Y-%m-%d %H:%M:%S.%f')
+            if type.startswith('DateTime64('):
+                tmp = tmp.replace(tzinfo=tz.gettz(type.split('(')[1][2:-3]))
+            return tmp
         if type.startswith('Array('):
             value = value.replace(',,', ",'',") # workaround empty string clickhouse bug
             parts = ast.literal_eval(value)
 
             def handle_dates(val, typ):
                 if typ.startswith('Date'):
                     return [self.unformatfield(x, typ) for x in val]
```

### Comparing `pyclickhouse3-0.9.34/test/test_compatibility.py` & `pyclickhouse3-0.9.35/test/test_compatibility.py`

 * *Files identical despite different names*

### Comparing `pyclickhouse3-0.9.34/test/test_map.py` & `pyclickhouse3-0.9.35/test/test_map.py`

 * *Files identical despite different names*

### Comparing `pyclickhouse3-0.9.34/test/test_new.py` & `pyclickhouse3-0.9.35/test/test_new.py`

 * *Files 2% similar despite different names*

```diff
@@ -14,14 +14,20 @@
 
     def test_array_serialization(self):
         self.cursor.select("select ['abc','def'] as t")
         result = self.cursor.fetchone()['t']
         assert result[0] == 'abc'
         assert result[1] == 'def'
 
+    def test_u64_serializaton(self):
+        self.cursor.ddl('create table t64 (ts DateTime64(3)) Engine=MergeTree order by ts')
+        self.cursor.bulkinsert('t64', [{'ts': dt.datetime.now()}], ['ts'], ['DateTime64(3)'])
+        self.cursor.select("""select ts from t64""")
+        assert 'ts' in self.cursor.fetchone()
+
     def test_unformat_of_commas(self):
         formatter = TabSeparatedWithNamesAndTypesFormatter()
         formatter.unformatfield("['abc',,'def']", 'Array(String)')  # boom
 
     def test_store_doc(self):
         doc = {'id': 3, 'historydate': dt.date(2019,6,7), 'Offer': {'price': 5, 'count': 1}, 'Images': [{'file': 'a', 'size': 400}, {'file': 'b', 'size': 500}]}
         self.cursor.ddl('drop table if exists docs')
```

### Comparing `pyclickhouse3-0.9.34/test/test_simple.py` & `pyclickhouse3-0.9.35/test/test_simple.py`

 * *Files identical despite different names*

