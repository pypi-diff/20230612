# Comparing `tmp/otel_tracer-0.0.2-py3-none-any.whl.zip` & `tmp/otel_tracer-0.0.3-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,9 +1,9 @@
-Zip file size: 2189 bytes, number of entries: 7
+Zip file size: 2195 bytes, number of entries: 7
 -rw-r--r--  2.0 unx        0 b- defN 23-Jun-12 04:21 otel_tracer/__init__.py
 -rw-r--r--  2.0 unx        0 b- defN 23-Jun-12 04:35 otel_tracer/tracing/__init__.py
 -rw-r--r--  2.0 unx     1550 b- defN 23-Jun-12 07:28 otel_tracer/tracing/tracer.py
--rw-r--r--  2.0 unx      802 b- defN 23-Jun-12 08:03 otel_tracer-0.0.2.dist-info/METADATA
--rw-r--r--  2.0 unx       92 b- defN 23-Jun-12 08:03 otel_tracer-0.0.2.dist-info/WHEEL
--rw-r--r--  2.0 unx       12 b- defN 23-Jun-12 08:03 otel_tracer-0.0.2.dist-info/top_level.txt
-?rw-rw-r--  2.0 unx      561 b- defN 23-Jun-12 08:03 otel_tracer-0.0.2.dist-info/RECORD
-7 files, 3017 bytes uncompressed, 1181 bytes compressed:  60.9%
+-rw-r--r--  2.0 unx      854 b- defN 23-Jun-12 08:31 otel_tracer-0.0.3.dist-info/METADATA
+-rw-r--r--  2.0 unx       92 b- defN 23-Jun-12 08:31 otel_tracer-0.0.3.dist-info/WHEEL
+-rw-r--r--  2.0 unx       12 b- defN 23-Jun-12 08:31 otel_tracer-0.0.3.dist-info/top_level.txt
+?rw-rw-r--  2.0 unx      561 b- defN 23-Jun-12 08:31 otel_tracer-0.0.3.dist-info/RECORD
+7 files, 3069 bytes uncompressed, 1187 bytes compressed:  61.3%
```

## zipnote {}

```diff
@@ -3,20 +3,20 @@
 
 Filename: otel_tracer/tracing/__init__.py
 Comment: 
 
 Filename: otel_tracer/tracing/tracer.py
 Comment: 
 
-Filename: otel_tracer-0.0.2.dist-info/METADATA
+Filename: otel_tracer-0.0.3.dist-info/METADATA
 Comment: 
 
-Filename: otel_tracer-0.0.2.dist-info/WHEEL
+Filename: otel_tracer-0.0.3.dist-info/WHEEL
 Comment: 
 
-Filename: otel_tracer-0.0.2.dist-info/top_level.txt
+Filename: otel_tracer-0.0.3.dist-info/top_level.txt
 Comment: 
 
-Filename: otel_tracer-0.0.2.dist-info/RECORD
+Filename: otel_tracer-0.0.3.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## Comparing `otel_tracer-0.0.2.dist-info/METADATA` & `otel_tracer-0.0.3.dist-info/METADATA`

 * *Files 5% similar despite different names*

```diff
@@ -1,20 +1,21 @@
 Metadata-Version: 2.1
 Name: otel-tracer
-Version: 0.0.2
+Version: 0.0.3
 Summary: common python utilities for otel
 Home-page: UNKNOWN
 Author: VxRail
 Author-email: UNKNOWN
 License: ToBeDone
 Platform: python3
 Requires-Dist: flask
 Requires-Dist: opentelemetry-api
 Requires-Dist: opentelemetry-exporter-jaeger-thrift
 Requires-Dist: opentelemetry-exporter-otlp-proto-grpc
+Requires-Dist: opentelemetry-instrumentation-celery
 Requires-Dist: opentelemetry-instrumentation-flask
 Requires-Dist: opentelemetry-instrumentation-pika
 Requires-Dist: opentelemetry-instrumentation-redis
 Requires-Dist: opentelemetry-instrumentation-requests
 Requires-Dist: opentelemetry-instrumentation-sqlalchemy
 Requires-Dist: opentelemetry-sdk
 Requires-Dist: opentelemetry-semantic-conventions
```

## Comparing `otel_tracer-0.0.2.dist-info/RECORD` & `otel_tracer-0.0.3.dist-info/RECORD`

 * *Files 6% similar despite different names*

```diff
@@ -1,7 +1,7 @@
 otel_tracer/__init__.py,sha256=47DEQpj8HBSa-_TImW-5JCeuQeRkm5NMpJWZG3hSuFU,0
 otel_tracer/tracing/__init__.py,sha256=47DEQpj8HBSa-_TImW-5JCeuQeRkm5NMpJWZG3hSuFU,0
 otel_tracer/tracing/tracer.py,sha256=7fGT0kPmNvd2wUpwbsMIjnjjaQKK6v8KlyB_LAztRAI,1550
-otel_tracer-0.0.2.dist-info/METADATA,sha256=9VmF25RLfj_NW0VN533h81wW6fibgsQdMPzsu-9cXHI,802
-otel_tracer-0.0.2.dist-info/WHEEL,sha256=g4nMs7d-Xl9-xC9XovUrsDHGXt-FT0E17Yqo92DEfvY,92
-otel_tracer-0.0.2.dist-info/top_level.txt,sha256=llJBDjZB1BQSEOpLnQesdrfISu_CEXguxypv2CGx0aY,12
-otel_tracer-0.0.2.dist-info/RECORD,,
+otel_tracer-0.0.3.dist-info/METADATA,sha256=iSmJAS3CczXCr4dz1I6_ZS76PZW6Pt9XK9hyoK_nsZI,854
+otel_tracer-0.0.3.dist-info/WHEEL,sha256=g4nMs7d-Xl9-xC9XovUrsDHGXt-FT0E17Yqo92DEfvY,92
+otel_tracer-0.0.3.dist-info/top_level.txt,sha256=llJBDjZB1BQSEOpLnQesdrfISu_CEXguxypv2CGx0aY,12
+otel_tracer-0.0.3.dist-info/RECORD,,
```

