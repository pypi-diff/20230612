# Comparing `tmp/celery-redbeat-2.1.0.tar.gz` & `tmp/celery-redbeat-2.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/celery-redbeat-2.1.0.tar", last modified: Thu May 18 00:47:09 2023, max compression
+gzip compressed data, was "dist/celery-redbeat-2.1.1.tar", last modified: Sun Jun 11 23:43:42 2023, max compression
```

## Comparing `celery-redbeat-2.1.0.tar` & `celery-redbeat-2.1.1.tar`

### file list

```diff
@@ -1,28 +1,28 @@
-drwxr-xr-x   0 marcs      (501) staff       (20)        0 2023-05-18 00:47:09.420850 celery-redbeat-2.1.0/
--rw-r--r--   0 marcs      (501) staff       (20)     2384 2023-05-18 00:47:07.000000 celery-redbeat-2.1.0/CHANGES.txt
--rw-r--r--   0 marcs      (501) staff       (20)    11358 2019-03-06 01:10:25.000000 celery-redbeat-2.1.0/LICENSE
--rw-r--r--   0 marcs      (501) staff       (20)       78 2019-03-06 01:10:25.000000 celery-redbeat-2.1.0/MANIFEST.in
--rw-r--r--   0 marcs      (501) staff       (20)     3395 2023-05-18 00:47:09.421111 celery-redbeat-2.1.0/PKG-INFO
--rw-r--r--   0 marcs      (501) staff       (20)     2424 2023-04-29 15:07:05.000000 celery-redbeat-2.1.0/README.rst
-drwxr-xr-x   0 marcs      (501) staff       (20)        0 2023-05-18 00:47:09.407755 celery-redbeat-2.1.0/celery_redbeat.egg-info/
--rw-r--r--   0 marcs      (501) staff       (20)     3395 2023-05-18 00:47:09.000000 celery-redbeat-2.1.0/celery_redbeat.egg-info/PKG-INFO
--rw-r--r--   0 marcs      (501) staff       (20)      490 2023-05-18 00:47:09.000000 celery-redbeat-2.1.0/celery_redbeat.egg-info/SOURCES.txt
--rw-r--r--   0 marcs      (501) staff       (20)        1 2023-05-18 00:47:09.000000 celery-redbeat-2.1.0/celery_redbeat.egg-info/dependency_links.txt
--rw-r--r--   0 marcs      (501) staff       (20)       48 2023-05-18 00:47:09.000000 celery-redbeat-2.1.0/celery_redbeat.egg-info/requires.txt
--rw-r--r--   0 marcs      (501) staff       (20)        8 2023-05-18 00:47:09.000000 celery-redbeat-2.1.0/celery_redbeat.egg-info/top_level.txt
--rw-r--r--   0 marcs      (501) staff       (20)      477 2023-04-29 15:06:44.000000 celery-redbeat-2.1.0/exampleconf.py
--rw-r--r--   0 marcs      (501) staff       (20)      120 2023-05-18 00:23:38.000000 celery-redbeat-2.1.0/pyproject.toml
-drwxr-xr-x   0 marcs      (501) staff       (20)        0 2023-05-18 00:47:09.412590 celery-redbeat-2.1.0/redbeat/
--rw-r--r--   0 marcs      (501) staff       (20)       72 2023-04-29 15:06:44.000000 celery-redbeat-2.1.0/redbeat/__init__.py
--rw-r--r--   0 marcs      (501) staff       (20)     4598 2023-04-29 15:06:44.000000 celery-redbeat-2.1.0/redbeat/decoder.py
--rw-r--r--   0 marcs      (501) staff       (20)    18020 2023-05-03 19:24:54.000000 celery-redbeat-2.1.0/redbeat/schedulers.py
--rw-r--r--   0 marcs      (501) staff       (20)     3593 2023-04-29 15:06:44.000000 celery-redbeat-2.1.0/redbeat/schedules.py
--rw-r--r--   0 marcs      (501) staff       (20)      172 2023-05-18 00:47:09.422385 celery-redbeat-2.1.0/setup.cfg
--rw-r--r--   0 marcs      (501) staff       (20)     1256 2023-05-17 23:41:44.000000 celery-redbeat-2.1.0/setup.py
-drwxr-xr-x   0 marcs      (501) staff       (20)        0 2023-05-18 00:47:09.419923 celery-redbeat-2.1.0/tests/
--rw-r--r--   0 marcs      (501) staff       (20)     1490 2023-04-29 15:06:44.000000 celery-redbeat-2.1.0/tests/test_config.py
--rw-r--r--   0 marcs      (501) staff       (20)     4399 2023-04-29 15:06:44.000000 celery-redbeat-2.1.0/tests/test_entry.py
--rw-r--r--   0 marcs      (501) staff       (20)     7629 2023-04-29 15:06:44.000000 celery-redbeat-2.1.0/tests/test_json.py
--rw-r--r--   0 marcs      (501) staff       (20)    13799 2023-04-29 15:08:53.000000 celery-redbeat-2.1.0/tests/test_scheduler.py
--rw-r--r--   0 marcs      (501) staff       (20)     3589 2023-04-29 15:06:44.000000 celery-redbeat-2.1.0/tests/test_schedules.py
--rw-r--r--   0 marcs      (501) staff       (20)      543 2023-04-29 15:06:44.000000 celery-redbeat-2.1.0/tests/test_utils.py
+drwxr-xr-x   0 marcs      (501) staff       (20)        0 2023-06-11 23:43:42.020491 celery-redbeat-2.1.1/
+-rw-r--r--   0 marcs      (501) staff       (20)     2493 2023-06-11 23:41:18.000000 celery-redbeat-2.1.1/CHANGES.txt
+-rw-r--r--   0 marcs      (501) staff       (20)    11358 2019-03-06 01:10:25.000000 celery-redbeat-2.1.1/LICENSE
+-rw-r--r--   0 marcs      (501) staff       (20)       78 2019-03-06 01:10:25.000000 celery-redbeat-2.1.1/MANIFEST.in
+-rw-r--r--   0 marcs      (501) staff       (20)     3395 2023-06-11 23:43:42.020756 celery-redbeat-2.1.1/PKG-INFO
+-rw-r--r--   0 marcs      (501) staff       (20)     2424 2023-04-29 15:07:05.000000 celery-redbeat-2.1.1/README.rst
+drwxr-xr-x   0 marcs      (501) staff       (20)        0 2023-06-11 23:43:42.007816 celery-redbeat-2.1.1/celery_redbeat.egg-info/
+-rw-r--r--   0 marcs      (501) staff       (20)     3395 2023-06-11 23:43:41.000000 celery-redbeat-2.1.1/celery_redbeat.egg-info/PKG-INFO
+-rw-r--r--   0 marcs      (501) staff       (20)      490 2023-06-11 23:43:41.000000 celery-redbeat-2.1.1/celery_redbeat.egg-info/SOURCES.txt
+-rw-r--r--   0 marcs      (501) staff       (20)        1 2023-06-11 23:43:41.000000 celery-redbeat-2.1.1/celery_redbeat.egg-info/dependency_links.txt
+-rw-r--r--   0 marcs      (501) staff       (20)      103 2023-06-11 23:43:41.000000 celery-redbeat-2.1.1/celery_redbeat.egg-info/requires.txt
+-rw-r--r--   0 marcs      (501) staff       (20)        8 2023-06-11 23:43:41.000000 celery-redbeat-2.1.1/celery_redbeat.egg-info/top_level.txt
+-rw-r--r--   0 marcs      (501) staff       (20)      477 2023-04-29 15:06:44.000000 celery-redbeat-2.1.1/exampleconf.py
+-rw-r--r--   0 marcs      (501) staff       (20)      120 2023-05-18 00:23:38.000000 celery-redbeat-2.1.1/pyproject.toml
+drwxr-xr-x   0 marcs      (501) staff       (20)        0 2023-06-11 23:43:42.013350 celery-redbeat-2.1.1/redbeat/
+-rw-r--r--   0 marcs      (501) staff       (20)       72 2023-04-29 15:06:44.000000 celery-redbeat-2.1.1/redbeat/__init__.py
+-rw-r--r--   0 marcs      (501) staff       (20)     4680 2023-06-11 23:35:17.000000 celery-redbeat-2.1.1/redbeat/decoder.py
+-rw-r--r--   0 marcs      (501) staff       (20)    18020 2023-05-03 19:24:54.000000 celery-redbeat-2.1.1/redbeat/schedulers.py
+-rw-r--r--   0 marcs      (501) staff       (20)     3593 2023-04-29 15:06:44.000000 celery-redbeat-2.1.1/redbeat/schedules.py
+-rw-r--r--   0 marcs      (501) staff       (20)      172 2023-06-11 23:43:42.021810 celery-redbeat-2.1.1/setup.cfg
+-rw-r--r--   0 marcs      (501) staff       (20)     1358 2023-06-11 23:38:27.000000 celery-redbeat-2.1.1/setup.py
+drwxr-xr-x   0 marcs      (501) staff       (20)        0 2023-06-11 23:43:42.019699 celery-redbeat-2.1.1/tests/
+-rw-r--r--   0 marcs      (501) staff       (20)     1490 2023-04-29 15:06:44.000000 celery-redbeat-2.1.1/tests/test_config.py
+-rw-r--r--   0 marcs      (501) staff       (20)     4399 2023-04-29 15:06:44.000000 celery-redbeat-2.1.1/tests/test_entry.py
+-rw-r--r--   0 marcs      (501) staff       (20)     7685 2023-06-11 23:35:17.000000 celery-redbeat-2.1.1/tests/test_json.py
+-rw-r--r--   0 marcs      (501) staff       (20)    13799 2023-04-29 15:08:53.000000 celery-redbeat-2.1.1/tests/test_scheduler.py
+-rw-r--r--   0 marcs      (501) staff       (20)     3589 2023-04-29 15:06:44.000000 celery-redbeat-2.1.1/tests/test_schedules.py
+-rw-r--r--   0 marcs      (501) staff       (20)      543 2023-04-29 15:06:44.000000 celery-redbeat-2.1.1/tests/test_utils.py
```

### Comparing `celery-redbeat-2.1.0/CHANGES.txt` & `celery-redbeat-2.1.1/CHANGES.txt`

 * *Files 6% similar despite different names*

```diff
@@ -1,8 +1,12 @@
-2.1.0 ()
+2.1.1 (2023-06-11)
+---------------------
+ - fix compatability with Celery 5.3.0, thanks @jkseppan
+
+2.1.0 (2023-05-17)
 ---------------------
  - BREAKING, drop for support for EOL Python < 3.8
  - log message cleanup, thanks @joekohlsdorf
  - ensure lock is owned before releasing, fixing #223, thanks @michaelbukachi
  - fix #238, #208, failure to aquire lock on startup leads to multiple task executions, thanks @Junzki, @nicklyra, @nigel-gott
  - Add options support for RedBeatSchedulerEntry, thanks @anton-petrov
```

### Comparing `celery-redbeat-2.1.0/LICENSE` & `celery-redbeat-2.1.1/LICENSE`

 * *Files identical despite different names*

### Comparing `celery-redbeat-2.1.0/PKG-INFO` & `celery-redbeat-2.1.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: celery-redbeat
-Version: 2.1.0
+Version: 2.1.1
 Summary: A Celery Beat Scheduler using Redis for persistent storage
 Home-page: https://github.com/sibson/redbeat
 Author: Marc Sibson
 Author-email: sibson+redbeat@gmail.com
 License: Apache License, Version 2.0
 Keywords: python,celery,beat,redis
 Classifier: Development Status :: 5 - Production/Stable
```

### Comparing `celery-redbeat-2.1.0/README.rst` & `celery-redbeat-2.1.1/README.rst`

 * *Files identical despite different names*

### Comparing `celery-redbeat-2.1.0/celery_redbeat.egg-info/PKG-INFO` & `celery-redbeat-2.1.1/celery_redbeat.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: celery-redbeat
-Version: 2.1.0
+Version: 2.1.1
 Summary: A Celery Beat Scheduler using Redis for persistent storage
 Home-page: https://github.com/sibson/redbeat
 Author: Marc Sibson
 Author-email: sibson+redbeat@gmail.com
 License: Apache License, Version 2.0
 Keywords: python,celery,beat,redis
 Classifier: Development Status :: 5 - Production/Stable
```

### Comparing `celery-redbeat-2.1.0/redbeat/decoder.py` & `celery-redbeat-2.1.1/redbeat/decoder.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,15 +1,19 @@
 import calendar
 import json
-from datetime import datetime
+from datetime import datetime, timedelta, timezone
 
 from celery.schedules import crontab, schedule
-from celery.utils.time import FixedOffset, timezone
 from dateutil.rrule import weekday
 
+try:
+    import zoneinfo
+except ImportError:
+    from backports import zoneinfo
+
 from .schedules import rrule
 
 
 def to_timestamp(dt):
     """convert local tz aware datetime to seconds since the epoch"""
     return calendar.timegm(dt.utctimetuple())
 
@@ -20,15 +24,15 @@
 
     # Python 3: utcoffset / timedelta(minutes=1)
     return utcoffset.total_seconds() / 60 if utcoffset else 0
 
 
 def from_timestamp(seconds, tz_minutes=0):
     """convert seconds since the epoch to an UTC aware datetime"""
-    tz = FixedOffset(tz_minutes) if tz_minutes else timezone.utc
+    tz = timezone(timedelta(minutes=tz_minutes)) if tz_minutes else timezone.utc
     return datetime.fromtimestamp(seconds, tz=tz)
 
 
 class RedBeatJSONDecoder(json.JSONDecoder):
     def __init__(self, *args, **kargs):
         super().__init__(object_hook=self.dict_to_object, *args, **kargs)
 
@@ -37,17 +41,17 @@
             return d
 
         objtype = d.pop('__type__')
 
         if objtype == 'datetime':
             zone = d.pop('timezone', 'UTC')
             try:
-                tzinfo = FixedOffset(zone / 60)
+                tzinfo = timezone(timedelta(minutes=(zone / 60)))
             except TypeError:
-                tzinfo = timezone.get_timezone(zone)
+                tzinfo = zoneinfo.ZoneInfo(zone)
             return datetime(tzinfo=tzinfo, **d)
 
         if objtype == 'interval':
             return schedule(run_every=d['every'], relative=d['relative'])
 
         if objtype == 'crontab':
             return crontab(**d)
@@ -70,18 +74,18 @@
 
 
 class RedBeatJSONEncoder(json.JSONEncoder):
     def default(self, obj):
         if isinstance(obj, datetime):
             if obj.tzinfo is None:
                 timezone = 'UTC'
-            elif obj.tzinfo.zone is None:
-                timezone = obj.tzinfo.utcoffset(None).total_seconds()
+            elif hasattr(obj.tzinfo, 'key'):
+                timezone = obj.tzinfo.key
             else:
-                timezone = obj.tzinfo.zone
+                timezone = obj.tzinfo.utcoffset(None).total_seconds()
 
             return {
                 '__type__': 'datetime',
                 'year': obj.year,
                 'month': obj.month,
                 'day': obj.day,
                 'hour': obj.hour,
```

### Comparing `celery-redbeat-2.1.0/redbeat/schedulers.py` & `celery-redbeat-2.1.1/redbeat/schedulers.py`

 * *Files identical despite different names*

### Comparing `celery-redbeat-2.1.0/redbeat/schedules.py` & `celery-redbeat-2.1.1/redbeat/schedules.py`

 * *Files identical despite different names*

### Comparing `celery-redbeat-2.1.0/setup.py` & `celery-redbeat-2.1.1/setup.py`

 * *Files 23% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 
 long_description = open('README.rst').read()
 
 setup(
     name="celery-redbeat",
     description="A Celery Beat Scheduler using Redis for persistent storage",
     long_description=long_description,
-    version="2.1.0",
+    version="2.1.1",
     url="https://github.com/sibson/redbeat",
     license="Apache License, Version 2.0",
     author="Marc Sibson",
     author_email="sibson+redbeat@gmail.com",
     keywords="python celery beat redis".split(),
     packages=["redbeat"],
     classifiers=[
@@ -23,10 +23,16 @@
         'Programming Language :: Python :: 3.8',
         'Programming Language :: Python :: 3.9',
         'Programming Language :: Python :: 3.10',
         'Programming Language :: Python :: 3.11',
         'Programming Language :: Python :: Implementation :: CPython',
         'Operating System :: OS Independent',
     ],
-    install_requires=['redis>=3.2', 'celery>=5.0', 'python-dateutil', 'tenacity'],
+    install_requires=[
+        'redis>=3.2',
+        'celery>=5.0',
+        'python-dateutil',
+        'tenacity',
+        'backports.zoneinfo>=0.2.1; python_version < "3.9.0"',
+    ],
     tests_require=['pytest'],
 )
```

### Comparing `celery-redbeat-2.1.0/tests/test_config.py` & `celery-redbeat-2.1.1/tests/test_config.py`

 * *Files identical despite different names*

### Comparing `celery-redbeat-2.1.0/tests/test_entry.py` & `celery-redbeat-2.1.1/tests/test_entry.py`

 * *Files identical despite different names*

### Comparing `celery-redbeat-2.1.0/tests/test_json.py` & `celery-redbeat-2.1.1/tests/test_json.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,18 +1,22 @@
 import json
-from datetime import datetime
+from datetime import datetime, timedelta, timezone
 from unittest import TestCase
 
 from celery.schedules import crontab, schedule
-from celery.utils.time import FixedOffset, timezone
 from dateutil import rrule as dateutil_rrule
 
 from redbeat.decoder import RedBeatJSONDecoder, RedBeatJSONEncoder
 from redbeat.schedules import rrule
 
+try:
+    import zoneinfo
+except ImportError:
+    from backports import zoneinfo
+
 
 class JSONTestCase(TestCase):
     def dumps(self, d):
         return json.dumps(d, cls=RedBeatJSONEncoder)
 
     def loads(self, d):
         return json.loads(d, cls=RedBeatJSONDecoder)
@@ -95,22 +99,22 @@
         dt = self.now()
         result = self.dumps(dt)
 
         expected = self.datetime_as_dict(__type__='datetime', timezone='UTC')
         self.assertEqual(json.loads(result), expected)
 
     def test_datetime_with_tz(self):
-        dt = self.now(tzinfo=timezone.get_timezone('Asia/Shanghai'))
+        dt = self.now(tzinfo=zoneinfo.ZoneInfo('Asia/Shanghai'))
         result = self.dumps(dt)
 
         expected = self.datetime_as_dict(timezone='Asia/Shanghai', __type__='datetime')
         self.assertEqual(json.loads(result), expected)
 
     def test_datetime_with_fixedoffset(self):
-        dt = self.now(tzinfo=FixedOffset(4 * 60))
+        dt = self.now(tzinfo=timezone(timedelta(hours=4)))
         result = self.dumps(dt)
 
         expected = self.datetime_as_dict(timezone=4 * 60 * 60.0)
         expected['__type__'] = 'datetime'
         self.assertEqual(json.loads(result), expected)
 
     def test_schedule(self):
@@ -130,15 +134,15 @@
             until=datetime(2015, 12, 31, 12, 59, 22, tzinfo=timezone.utc),
             count=1,
         )
         result = self.dumps(r)
         self.assertEqual(json.loads(result), self.rrule())
 
     def test_rrule_timezone(self):
-        tz = timezone.get_timezone('US/Eastern')
+        tz = zoneinfo.ZoneInfo('US/Eastern')
 
         start1 = datetime(2015, 12, 30, 12, 59, 22, tzinfo=timezone.utc)
         start2 = start1.astimezone(tz)
 
         r1 = rrule('MINUTELY', dtstart=start1, count=1)
         r2 = rrule('MINUTELY', dtstart=start2, count=1)
 
@@ -205,22 +209,22 @@
         self.assertEqual(result, datetime(tzinfo=timezone.utc, **d))
 
     def test_datetime_with_timezone(self):
         d = self.datetime_as_dict(__type__='datetime', timezone='Asia/Shanghai')
         result = self.loads(json.dumps(d))
         d.pop('__type__')
         d.pop('timezone')
-        self.assertEqual(result, datetime(tzinfo=timezone.get_timezone('Asia/Shanghai'), **d))
+        self.assertEqual(result, datetime(tzinfo=zoneinfo.ZoneInfo('Asia/Shanghai'), **d))
 
     def test_datetime_with_fixed_offset(self):
         d = self.datetime_as_dict(__type__='datetime', timezone=5 * 60 * 60)
         result = self.loads(json.dumps(d))
         d.pop('__type__')
         d.pop('timezone')
-        self.assertEqual(result, datetime(tzinfo=FixedOffset(5 * 60), **d))
+        self.assertEqual(result, datetime(tzinfo=timezone(timedelta(hours=5)), **d))
 
     def test_schedule(self):
         d = self.schedule()
 
         result = self.loads(json.dumps(d))
         self.assertEqual(result, schedule(run_every=60))
```

### Comparing `celery-redbeat-2.1.0/tests/test_scheduler.py` & `celery-redbeat-2.1.1/tests/test_scheduler.py`

 * *Files identical despite different names*

### Comparing `celery-redbeat-2.1.0/tests/test_schedules.py` & `celery-redbeat-2.1.1/tests/test_schedules.py`

 * *Files identical despite different names*

### Comparing `celery-redbeat-2.1.0/tests/test_utils.py` & `celery-redbeat-2.1.1/tests/test_utils.py`

 * *Files identical despite different names*

