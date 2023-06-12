# Comparing `tmp/iosense_connect-3.0.2.tar.gz` & `tmp/iosense_connect-3.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist\iosense_connect-3.0.2.tar", last modified: Wed Jun  7 07:12:14 2023, max compression
+gzip compressed data, was "dist\iosense_connect-3.0.3.tar", last modified: Mon Jun 12 05:17:42 2023, max compression
```

## Comparing `iosense_connect-3.0.2.tar` & `iosense_connect-3.0.3.tar`

### file list

```diff
@@ -1,15 +1,15 @@
-drwxrwxrwx   0        0        0        0 2023-06-07 07:12:14.461030 iosense_connect-3.0.2/
--rw-rw-rw-   0        0        0     1087 2023-04-28 09:03:25.000000 iosense_connect-3.0.2/LICENSE.txt
--rw-rw-rw-   0        0        0     1062 2023-06-07 07:12:14.459030 iosense_connect-3.0.2/PKG-INFO
--rw-rw-rw-   0        0        0      690 2023-04-28 09:03:25.000000 iosense_connect-3.0.2/README.md
-drwxrwxrwx   0        0        0        0 2023-06-07 07:12:14.315627 iosense_connect-3.0.2/iosense_connect/
--rw-rw-rw-   0        0        0       37 2023-03-23 09:15:17.000000 iosense_connect-3.0.2/iosense_connect/__init__.py
--rw-rw-rw-   0        0        0    23984 2023-06-07 07:12:00.000000 iosense_connect-3.0.2/iosense_connect/data_access.py
-drwxrwxrwx   0        0        0        0 2023-06-07 07:12:14.457011 iosense_connect-3.0.2/iosense_connect.egg-info/
--rw-rw-rw-   0        0        0     1062 2023-06-07 07:12:13.000000 iosense_connect-3.0.2/iosense_connect.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      283 2023-06-07 07:12:13.000000 iosense_connect-3.0.2/iosense_connect.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-06-07 07:12:13.000000 iosense_connect-3.0.2/iosense_connect.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       65 2023-06-07 07:12:13.000000 iosense_connect-3.0.2/iosense_connect.egg-info/requires.txt
--rw-rw-rw-   0        0        0       16 2023-06-07 07:12:13.000000 iosense_connect-3.0.2/iosense_connect.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-06-07 07:12:14.462029 iosense_connect-3.0.2/setup.cfg
--rw-rw-rw-   0        0        0      794 2023-06-07 07:12:00.000000 iosense_connect-3.0.2/setup.py
+drwxrwxrwx   0        0        0        0 2023-06-12 05:17:42.201183 iosense_connect-3.0.3/
+-rw-rw-rw-   0        0        0     1087 2023-04-28 09:03:25.000000 iosense_connect-3.0.3/LICENSE.txt
+-rw-rw-rw-   0        0        0     1062 2023-06-12 05:17:42.196819 iosense_connect-3.0.3/PKG-INFO
+-rw-rw-rw-   0        0        0      690 2023-04-28 09:03:25.000000 iosense_connect-3.0.3/README.md
+drwxrwxrwx   0        0        0        0 2023-06-12 05:17:42.089776 iosense_connect-3.0.3/iosense_connect/
+-rw-rw-rw-   0        0        0       37 2023-03-23 09:15:17.000000 iosense_connect-3.0.3/iosense_connect/__init__.py
+-rw-rw-rw-   0        0        0    24111 2023-06-12 05:17:33.000000 iosense_connect-3.0.3/iosense_connect/data_access.py
+drwxrwxrwx   0        0        0        0 2023-06-12 05:17:42.192513 iosense_connect-3.0.3/iosense_connect.egg-info/
+-rw-rw-rw-   0        0        0     1062 2023-06-12 05:17:40.000000 iosense_connect-3.0.3/iosense_connect.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      283 2023-06-12 05:17:41.000000 iosense_connect-3.0.3/iosense_connect.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-06-12 05:17:40.000000 iosense_connect-3.0.3/iosense_connect.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       65 2023-06-12 05:17:40.000000 iosense_connect-3.0.3/iosense_connect.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       16 2023-06-12 05:17:40.000000 iosense_connect-3.0.3/iosense_connect.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-06-12 05:17:42.201183 iosense_connect-3.0.3/setup.cfg
+-rw-rw-rw-   0        0        0      794 2023-06-12 05:17:34.000000 iosense_connect-3.0.3/setup.py
```

### Comparing `iosense_connect-3.0.2/LICENSE.txt` & `iosense_connect-3.0.3/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `iosense_connect-3.0.2/PKG-INFO` & `iosense_connect-3.0.3/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: iosense_connect
-Version: 3.0.2
+Version: 3.0.3
 Summary: iosense connect library
 Author: Faclon-Labs
 Author-email: reachus@faclon.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Description-Content-Type: text/markdown
```

### Comparing `iosense_connect-3.0.2/README.md` & `iosense_connect-3.0.3/README.md`

 * *Files identical despite different names*

### Comparing `iosense_connect-3.0.2/iosense_connect/data_access.py` & `iosense_connect-3.0.3/iosense_connect/data_access.py`

 * *Files 0% similar despite different names*

```diff
@@ -487,18 +487,20 @@
                             df =  df[sensors_filtered]
                         if len(sensors_filtered) == 0:
                             df = pd.DataFrame()
                         df.sort_values(['time'], inplace=True)
                         df.reset_index(drop=True, inplace=True)
                         last_date = str(df['time'].iloc[-1])
                         start_date = df['time'].iloc[-1].date() + timedelta(days=1)
-                        end_time = str(end_time)
 
                         last_date = datetime.strptime(last_date, "%Y-%m-%d %H:%M:%S.%f")
-                        end_time = datetime.strptime(end_time, "%Y-%m-%d %H:%M:%S.%f")
+                        try:
+                            end_time = datetime.strptime(str(end_time), "%Y-%m-%d %H:%M:%S.%f")
+                        except ValueError:
+                            end_time = datetime.strptime(str(end_time), "%Y-%m-%d %H:%M:%S")
 
                         if last_date.year != end_time.year and last_date.month != end_time.month and last_date.day != end_time.day and last_date.hour != end_time.hour:
                             df1 = DataAccess.fetch_data(self, device_id, start_time=str(start_date), alias=False,
                                                         end_time=end_time, sensors=sensors, echo=True,
                                                         onpremise=onpremise, IST=True)
                             df = pd.concat([df, df1])
                             df.reset_index(drop=True, inplace=True)
```

### Comparing `iosense_connect-3.0.2/iosense_connect.egg-info/PKG-INFO` & `iosense_connect-3.0.3/iosense_connect.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: iosense-connect
-Version: 3.0.2
+Version: 3.0.3
 Summary: iosense connect library
 Author: Faclon-Labs
 Author-email: reachus@faclon.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Description-Content-Type: text/markdown
```

### Comparing `iosense_connect-3.0.2/setup.py` & `iosense_connect-3.0.3/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import setuptools
 
 with open("README.md", "r", encoding = "utf-8") as fh:
     long_description = fh.read()
 
 setuptools.setup(
     name = "iosense_connect",
-    version = "3.0.2",
+    version = "3.0.3",
     author = "Faclon-Labs",
     author_email = "reachus@faclon.com",
     description = "iosense connect library",
     packages = ["iosense_connect"],
     long_description = long_description,
     long_description_content_type = "text/markdown",
     install_requires=[
```

