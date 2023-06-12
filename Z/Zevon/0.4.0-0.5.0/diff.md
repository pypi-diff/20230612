# Comparing `tmp/Zevon-0.4.0.tar.gz` & `tmp/Zevon-0.5.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "Zevon-0.4.0.tar", last modified: Thu Jan 12 21:15:59 2023, max compression
+gzip compressed data, was "Zevon-0.5.0.tar", last modified: Mon Jun 12 14:08:00 2023, max compression
```

## Comparing `Zevon-0.4.0.tar` & `Zevon-0.5.0.tar`

### file list

```diff
@@ -1,17 +1,17 @@
-drwxr-xr-x   0 duket     (1000) duket     (1000)        0 2023-01-12 21:15:59.453747 Zevon-0.4.0/
--rw-r--r--   0 duket     (1000) duket     (1000)     1070 2022-07-05 15:43:03.000000 Zevon-0.4.0/LICENSE
--rw-r--r--   0 duket     (1000) duket     (1000)      270 2023-01-12 21:15:59.453747 Zevon-0.4.0/PKG-INFO
--rw-r--r--   0 duket     (1000) duket     (1000)       14 2023-01-12 21:15:15.000000 Zevon-0.4.0/README.md
-drwxr-xr-x   0 duket     (1000) duket     (1000)        0 2023-01-12 21:15:59.453747 Zevon-0.4.0/Zevon.egg-info/
--rw-r--r--   0 duket     (1000) duket     (1000)      270 2023-01-12 21:15:59.000000 Zevon-0.4.0/Zevon.egg-info/PKG-INFO
--rw-r--r--   0 duket     (1000) duket     (1000)      259 2023-01-12 21:15:59.000000 Zevon-0.4.0/Zevon.egg-info/SOURCES.txt
--rw-r--r--   0 duket     (1000) duket     (1000)        1 2023-01-12 21:15:59.000000 Zevon-0.4.0/Zevon.egg-info/dependency_links.txt
--rw-r--r--   0 duket     (1000) duket     (1000)       25 2023-01-12 21:15:59.000000 Zevon-0.4.0/Zevon.egg-info/requires.txt
--rw-r--r--   0 duket     (1000) duket     (1000)        6 2023-01-12 21:15:59.000000 Zevon-0.4.0/Zevon.egg-info/top_level.txt
--rw-r--r--   0 duket     (1000) duket     (1000)      344 2023-01-12 21:15:59.453747 Zevon-0.4.0/setup.cfg
--rw-r--r--   0 duket     (1000) duket     (1000)      355 2023-01-12 21:15:15.000000 Zevon-0.4.0/setup.py
-drwxr-xr-x   0 duket     (1000) duket     (1000)        0 2023-01-12 21:15:59.453747 Zevon-0.4.0/zevon/
--rw-r--r--   0 duket     (1000) duket     (1000)      121 2023-01-12 21:15:15.000000 Zevon-0.4.0/zevon/__init__.py
--rw-r--r--   0 duket     (1000) duket     (1000)     5066 2023-01-12 17:51:02.000000 Zevon-0.4.0/zevon/flask_lambda.py
--rw-r--r--   0 duket     (1000) duket     (1000)     3468 2022-07-05 15:43:03.000000 Zevon-0.4.0/zevon/sample_event.py
--rw-r--r--   0 duket     (1000) duket     (1000)     1106 2023-01-12 21:15:15.000000 Zevon-0.4.0/zevon/welcome.py
+drwxrwxr-x   0 duket     (1001) duket     (1001)        0 2023-06-12 14:08:00.943187 Zevon-0.5.0/
+-rw-rw-r--   0 duket     (1001) duket     (1001)     1070 2022-01-31 14:48:14.000000 Zevon-0.5.0/LICENSE
+-rw-rw-r--   0 duket     (1001) duket     (1001)      270 2023-06-12 14:08:00.943187 Zevon-0.5.0/PKG-INFO
+-rw-rw-r--   0 duket     (1001) duket     (1001)       14 2023-06-09 14:15:22.000000 Zevon-0.5.0/README.md
+drwxrwxr-x   0 duket     (1001) duket     (1001)        0 2023-06-12 14:08:00.943187 Zevon-0.5.0/Zevon.egg-info/
+-rw-rw-r--   0 duket     (1001) duket     (1001)      270 2023-06-12 14:08:00.000000 Zevon-0.5.0/Zevon.egg-info/PKG-INFO
+-rw-rw-r--   0 duket     (1001) duket     (1001)      259 2023-06-12 14:08:00.000000 Zevon-0.5.0/Zevon.egg-info/SOURCES.txt
+-rw-rw-r--   0 duket     (1001) duket     (1001)        1 2023-06-12 14:08:00.000000 Zevon-0.5.0/Zevon.egg-info/dependency_links.txt
+-rw-rw-r--   0 duket     (1001) duket     (1001)       26 2023-06-12 14:08:00.000000 Zevon-0.5.0/Zevon.egg-info/requires.txt
+-rw-rw-r--   0 duket     (1001) duket     (1001)        6 2023-06-12 14:08:00.000000 Zevon-0.5.0/Zevon.egg-info/top_level.txt
+-rw-rw-r--   0 duket     (1001) duket     (1001)      344 2023-06-12 14:08:00.947186 Zevon-0.5.0/setup.cfg
+-rw-rw-r--   0 duket     (1001) duket     (1001)      356 2023-06-09 14:15:22.000000 Zevon-0.5.0/setup.py
+drwxrwxr-x   0 duket     (1001) duket     (1001)        0 2023-06-12 14:08:00.943187 Zevon-0.5.0/zevon/
+-rw-rw-r--   0 duket     (1001) duket     (1001)      121 2023-06-09 14:15:22.000000 Zevon-0.5.0/zevon/__init__.py
+-rw-rw-r--   0 duket     (1001) duket     (1001)     5641 2023-06-09 14:05:35.000000 Zevon-0.5.0/zevon/flask_lambda.py
+-rw-rw-r--   0 duket     (1001) duket     (1001)     3468 2022-01-31 14:48:14.000000 Zevon-0.5.0/zevon/sample_event.py
+-rw-rw-r--   0 duket     (1001) duket     (1001)     1106 2023-06-09 14:15:22.000000 Zevon-0.5.0/zevon/welcome.py
```

### Comparing `Zevon-0.4.0/LICENSE` & `Zevon-0.5.0/LICENSE`

 * *Files identical despite different names*

### Comparing `Zevon-0.4.0/zevon/flask_lambda.py` & `Zevon-0.5.0/zevon/flask_lambda.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,7 +1,8 @@
+import os
 import sys
 import json
 import logging
 import base64
 import datetime
 import time
 from io import StringIO
@@ -19,14 +20,23 @@
     'image',
     'font'
 ]
 
 init_time = int(time.time())
 logger = logging.getLogger(__name__)
 
+log_levels = {
+    'DEBUG': logging.DEBUG,
+    'INFO': logging.INFO,
+    'WARNING': logging.WARNING,
+    'ERROR': logging.ERROR
+}
+log_level = os.environ.get('ZEVON_LOG_LEVEL', 'WARNING')
+logger.setLevel(log_levels.get(log_level, logging.WARNING))
+
 
 def json_converter(o):
     '''
     Helper thing to convert dates for JSON modulet.
 
     Args:
         o - the thing to dump as string.
@@ -58,14 +68,21 @@
     return request_data
 
 
 def make_environ(event):
     logger.info(json.dumps(event, indent=2))
     environ = {}
 
+    caller = event.get('requestContext', {}).get('identity', {}).get('userArn', 'anonymous')
+
+    if caller is None:
+        caller = 'anonymous'
+
+    event['headers']['x-zvn-caller'] = caller
+    logger.info(f'{caller=} [e00da0624721]')
     for hdr_name, hdr_value in event['headers'].items():
         hdr_name = hdr_name.replace('-', '_').upper()
         if hdr_name in ['CONTENT_TYPE', 'CONTENT_LENGTH']:
             environ[hdr_name] = hdr_value
             continue
 
         http_hdr_name = 'HTTP_{}'.format(hdr_name)
@@ -120,15 +137,19 @@
 
     def start_response(self, status, response_headers, exc_info=None):
         self.status = int(status[:3])
         self.response_headers = dict(response_headers)
 
 
 class FlaskLambda(Flask):
+    def get_event(self):
+        return self.event
+
     def __call__(self, event, context):
+        self.event = event
         self.request_data = create_request_data(event)
         if 'httpMethod' not in event:
             # In this "context" `event` is `environ` and
             # `context` is `start_response`, meaning the request didn't
             # occur via API Gateway and Lambda
             return super(FlaskLambda, self).__call__(event, context)
```

### Comparing `Zevon-0.4.0/zevon/sample_event.py` & `Zevon-0.5.0/zevon/sample_event.py`

 * *Files identical despite different names*

### Comparing `Zevon-0.4.0/zevon/welcome.py` & `Zevon-0.5.0/zevon/welcome.py`

 * *Files 1% similar despite different names*

```diff
@@ -15,11 +15,11 @@
                 <li>Deploy AWS Lambda created with this tool. It generates a CloudFormation file and creates a stack from that template.</li>
                 <li>Optionally, integrate the new lambda with an AWS API Gateway, i.e. make a Flask application</li>
                 <li>Optionally, subscribe the new lambda to an SNS topic</li>
                 <li>Optionally, trust an arbitrary AWS service like cognito or S3</li>
             </ul>
         </div>
         <div>
-            Zevon version: 0.4.0
+            Zevon version: 0.5.0
         </div>
     </body>
 </html>'''
```

#### html2text {}

```diff
@@ -5,9 +5,9 @@
       lambda function or a Flask based microservice.
     * Deploy AWS Lambda created with this tool. It generates a CloudFormation
       file and creates a stack from that template.
     * Optionally, integrate the new lambda with an AWS API Gateway, i.e. make a
       Flask application
     * Optionally, subscribe the new lambda to an SNS topic
     * Optionally, trust an arbitrary AWS service like cognito or S3
-Zevon version: 0.4.0
+Zevon version: 0.5.0
 '''
```

