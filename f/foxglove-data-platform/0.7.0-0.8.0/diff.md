# Comparing `tmp/foxglove-data-platform-0.7.0.tar.gz` & `tmp/foxglove-data-platform-0.8.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "foxglove-data-platform-0.7.0.tar", last modified: Tue May 23 18:22:20 2023, max compression
+gzip compressed data, was "foxglove-data-platform-0.8.0.tar", last modified: Mon Jun 12 20:23:11 2023, max compression
```

## Comparing `foxglove-data-platform-0.7.0.tar` & `foxglove-data-platform-0.8.0.tar`

### file list

```diff
@@ -1,33 +1,33 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 18:22:20.565392 foxglove-data-platform-0.7.0/
--rw-r--r--   0 runner    (1001) docker     (123)     1077 2023-05-23 18:21:48.000000 foxglove-data-platform-0.7.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     1090 2023-05-23 18:22:20.565392 foxglove-data-platform-0.7.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      684 2023-05-23 18:21:48.000000 foxglove-data-platform-0.7.0/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 18:22:20.561392 foxglove-data-platform-0.7.0/foxglove_data_platform/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-23 18:21:48.000000 foxglove-data-platform-0.7.0/foxglove_data_platform/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    26812 2023-05-23 18:21:48.000000 foxglove-data-platform-0.7.0/foxglove_data_platform/client.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-23 18:21:48.000000 foxglove-data-platform-0.7.0/foxglove_data_platform/py.typed
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 18:22:20.561392 foxglove-data-platform-0.7.0/foxglove_data_platform.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     1090 2023-05-23 18:22:20.000000 foxglove-data-platform-0.7.0/foxglove_data_platform.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      747 2023-05-23 18:22:20.000000 foxglove-data-platform-0.7.0/foxglove_data_platform.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-23 18:22:20.000000 foxglove-data-platform-0.7.0/foxglove_data_platform.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       33 2023-05-23 18:22:20.000000 foxglove-data-platform-0.7.0/foxglove_data_platform.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       29 2023-05-23 18:22:20.000000 foxglove-data-platform-0.7.0/foxglove_data_platform.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)      104 2023-05-23 18:21:48.000000 foxglove-data-platform-0.7.0/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)      607 2023-05-23 18:22:20.565392 foxglove-data-platform-0.7.0/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 18:22:20.565392 foxglove-data-platform-0.7.0/tests/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-23 18:21:48.000000 foxglove-data-platform-0.7.0/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)       69 2023-05-23 18:21:48.000000 foxglove-data-platform-0.7.0/tests/api_url.py
--rw-r--r--   0 runner    (1001) docker     (123)     3119 2023-05-23 18:21:48.000000 foxglove-data-platform-0.7.0/tests/generate.py
--rw-r--r--   0 runner    (1001) docker     (123)     1250 2023-05-23 18:21:48.000000 foxglove-data-platform-0.7.0/tests/string_message_pb2.py
--rw-r--r--   0 runner    (1001) docker     (123)     2014 2023-05-23 18:21:48.000000 foxglove-data-platform-0.7.0/tests/test_attachments.py
--rw-r--r--   0 runner    (1001) docker     (123)     1972 2023-05-23 18:21:48.000000 foxglove-data-platform-0.7.0/tests/test_client.py
--rw-r--r--   0 runner    (1001) docker     (123)      919 2023-05-23 18:21:48.000000 foxglove-data-platform-0.7.0/tests/test_coverage.py
--rw-r--r--   0 runner    (1001) docker     (123)     1817 2023-05-23 18:21:48.000000 foxglove-data-platform-0.7.0/tests/test_data.py
--rw-r--r--   0 runner    (1001) docker     (123)     1779 2023-05-23 18:21:48.000000 foxglove-data-platform-0.7.0/tests/test_devices.py
--rw-r--r--   0 runner    (1001) docker     (123)     2435 2023-05-23 18:21:48.000000 foxglove-data-platform-0.7.0/tests/test_events.py
--rw-r--r--   0 runner    (1001) docker     (123)     2407 2023-05-23 18:21:48.000000 foxglove-data-platform-0.7.0/tests/test_imports.py
--rw-r--r--   0 runner    (1001) docker     (123)      498 2023-05-23 18:21:48.000000 foxglove-data-platform-0.7.0/tests/test_json_messages.py
--rw-r--r--   0 runner    (1001) docker     (123)      930 2023-05-23 18:21:48.000000 foxglove-data-platform-0.7.0/tests/test_protobuf_messages.py
--rw-r--r--   0 runner    (1001) docker     (123)     2935 2023-05-23 18:21:48.000000 foxglove-data-platform-0.7.0/tests/test_recordings.py
--rw-r--r--   0 runner    (1001) docker     (123)      978 2023-05-23 18:21:48.000000 foxglove-data-platform-0.7.0/tests/test_ros1_messages.py
--rw-r--r--   0 runner    (1001) docker     (123)     1078 2023-05-23 18:21:48.000000 foxglove-data-platform-0.7.0/tests/test_ros2_messages.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-12 20:23:11.175753 foxglove-data-platform-0.8.0/
+-rw-r--r--   0 runner    (1001) docker     (123)     1077 2023-06-12 20:22:08.000000 foxglove-data-platform-0.8.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     1090 2023-06-12 20:23:11.175753 foxglove-data-platform-0.8.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      684 2023-06-12 20:22:08.000000 foxglove-data-platform-0.8.0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-12 20:23:11.171754 foxglove-data-platform-0.8.0/foxglove_data_platform/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-12 20:22:08.000000 foxglove-data-platform-0.8.0/foxglove_data_platform/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    29399 2023-06-12 20:22:08.000000 foxglove-data-platform-0.8.0/foxglove_data_platform/client.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-12 20:22:08.000000 foxglove-data-platform-0.8.0/foxglove_data_platform/py.typed
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-12 20:23:11.171754 foxglove-data-platform-0.8.0/foxglove_data_platform.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     1090 2023-06-12 20:23:11.000000 foxglove-data-platform-0.8.0/foxglove_data_platform.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      747 2023-06-12 20:23:11.000000 foxglove-data-platform-0.8.0/foxglove_data_platform.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-12 20:23:11.000000 foxglove-data-platform-0.8.0/foxglove_data_platform.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       33 2023-06-12 20:23:11.000000 foxglove-data-platform-0.8.0/foxglove_data_platform.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       29 2023-06-12 20:23:11.000000 foxglove-data-platform-0.8.0/foxglove_data_platform.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      104 2023-06-12 20:22:08.000000 foxglove-data-platform-0.8.0/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)      607 2023-06-12 20:23:11.175753 foxglove-data-platform-0.8.0/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-12 20:23:11.175753 foxglove-data-platform-0.8.0/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-12 20:22:08.000000 foxglove-data-platform-0.8.0/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)       69 2023-06-12 20:22:08.000000 foxglove-data-platform-0.8.0/tests/api_url.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3119 2023-06-12 20:22:08.000000 foxglove-data-platform-0.8.0/tests/generate.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1250 2023-06-12 20:22:08.000000 foxglove-data-platform-0.8.0/tests/string_message_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2219 2023-06-12 20:22:08.000000 foxglove-data-platform-0.8.0/tests/test_attachments.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2177 2023-06-12 20:22:08.000000 foxglove-data-platform-0.8.0/tests/test_client.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1081 2023-06-12 20:22:08.000000 foxglove-data-platform-0.8.0/tests/test_coverage.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1817 2023-06-12 20:22:08.000000 foxglove-data-platform-0.8.0/tests/test_data.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2388 2023-06-12 20:22:08.000000 foxglove-data-platform-0.8.0/tests/test_devices.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3839 2023-06-12 20:22:08.000000 foxglove-data-platform-0.8.0/tests/test_events.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2407 2023-06-12 20:22:08.000000 foxglove-data-platform-0.8.0/tests/test_imports.py
+-rw-r--r--   0 runner    (1001) docker     (123)      498 2023-06-12 20:22:08.000000 foxglove-data-platform-0.8.0/tests/test_json_messages.py
+-rw-r--r--   0 runner    (1001) docker     (123)      930 2023-06-12 20:22:08.000000 foxglove-data-platform-0.8.0/tests/test_protobuf_messages.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2935 2023-06-12 20:22:08.000000 foxglove-data-platform-0.8.0/tests/test_recordings.py
+-rw-r--r--   0 runner    (1001) docker     (123)      978 2023-06-12 20:22:08.000000 foxglove-data-platform-0.8.0/tests/test_ros1_messages.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1078 2023-06-12 20:22:08.000000 foxglove-data-platform-0.8.0/tests/test_ros2_messages.py
```

### Comparing `foxglove-data-platform-0.7.0/LICENSE` & `foxglove-data-platform-0.8.0/LICENSE`

 * *Files identical despite different names*

### Comparing `foxglove-data-platform-0.7.0/PKG-INFO` & `foxglove-data-platform-0.8.0/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: foxglove-data-platform
-Version: 0.7.0
+Version: 0.8.0
 Summary: Client library for Foxglove Data Platform.
 Home-page: https://github.com/foxglove/py-data-platform
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
```

### Comparing `foxglove-data-platform-0.7.0/README.md` & `foxglove-data-platform-0.8.0/README.md`

 * *Files identical despite different names*

### Comparing `foxglove-data-platform-0.7.0/foxglove_data_platform/client.py` & `foxglove-data-platform-0.8.0/foxglove_data_platform/client.py`

 * *Files 5% similar despite different names*

```diff
@@ -171,35 +171,42 @@
 
     def __url__(self, path: str):
         return f"https://{self.__host}{path}"
 
     def create_event(
         self,
         *,
-        device_id: str,
+        device_id: Optional[str] = None,
+        device_name: Optional[str] = None,
         start: datetime.datetime,
         end: Optional[datetime.datetime],
         metadata: Optional[Dict[str, str]] = {},
     ):
         """
         Creates a new event.
 
-        device_id: The unique of the device associated with this event.
+        device_id: The id of the device associated with this event.
+        device_name: The name of the device associated with this event.
         start: The event start time.
         end: The event end time. If not provided, an instantaneous event (with end == start)
             is created.
         metadata: Optional metadata attached to the event.
         """
         if end is None:
             end = start
+        if device_id is None and device_name is None:
+            raise RuntimeError(
+                "device_id or device_name must be provided to create_event"
+            )
         response = requests.post(
             self.__url__("/v1/events"),
             headers=self.__headers,
             json={
-                "deviceId": device_id,
+                "device.id": device_id,
+                "device.name": device_name,
                 "start": start.astimezone().isoformat(),
                 "end": end.astimezone().isoformat(),
                 "metadata": metadata,
             },
         )
 
         return _event_dict(json_or_raise(response))
@@ -220,38 +227,41 @@
         )
         return json_or_raise(response)
 
     def get_events(
         self,
         *,
         device_id: Optional[str] = None,
+        device_name: Optional[str] = None,
         sort_by: Optional[str] = None,
         sort_order: Optional[str] = None,
         limit: Optional[int] = None,
         offset: Optional[int] = None,
         start: Optional[datetime.datetime] = None,
         end: Optional[datetime.datetime] = None,
         query: Optional[str] = None,
     ):
         """
         Retrieves events.
 
         device_id: Id of the device associated with the events.
+        device_name: Name of the device associated with the events.
         sort_by: Optionally sort records by this field name (e.g. "device_id").
         sort_order: Optionally specify the sort order, either "asc" or "desc".
         limit: Optionally limit the number of records returned.
         offset: Optionally offset the results by this many records.
         start: Optionally exclude records before this time.
         end: Optionally exclude records after this time.
         query: optional query string to filter events by metadata.
             See https://foxglove.dev/docs/api#tag/Events/paths/~1events/get for a syntax definition
             of `query`.
         """
         params = {
-            "deviceId": device_id,
+            "device.id": device_id,
+            "device.name": device_name,
             "sortBy": camelize(sort_by),
             "sortOrder": sort_order,
             "limit": limit,
             "offset": offset,
             "start": start.astimezone().isoformat() if start else None,
             "end": end.astimezone().isoformat() if end else None,
             "query": query,
@@ -263,34 +273,43 @@
         )
 
         return [_event_dict(event) for event in json_or_raise(response)]
 
     def get_messages(
         self,
         *,
-        device_id: str,
+        device_id: Optional[str] = None,
+        device_name: Optional[str] = None,
         start: datetime.datetime,
         end: datetime.datetime,
         topics: List[str] = [],
     ):
         """
         Returns a list of tuples of (topic, raw mcap record, decoded message).
 
         device_id: The id of the device that originated the desired data.
         start: The earliest time from which to retrieve data.
         end: The latest time from which to retrieve data.
         topics: An optional list of topics to retrieve.
             All topics will be retrieved if this is omitted.
         """
+        if device_id is None and device_name is None:
+            raise RuntimeError(
+                "device_id or device_name must be provided to get_messages"
+            )
         if not McapSchema or not make_reader:
             raise RuntimeError(
                 "Mcap library not found. Please install the mcap library."
             )
         data = self.download_data(
-            device_id=device_id, start=start, end=end, topics=topics
+            device_name=device_name,
+            device_id=device_id,
+            start=start,
+            end=end,
+            topics=topics,
         )
         reader = make_reader(BytesIO(data))
         decoders = {}
         output_messages = []
         for schema, channel, message in reader.iter_messages():
             if schema.encoding not in decoders:
                 decoder = decoder_for_schema_encoding(schema.encoding)
@@ -333,33 +352,36 @@
         json = json_or_raise(link_response)
 
         return _download_stream_with_progress(json["link"], callback=callback)
 
     def download_data(
         self,
         *,
-        device_id: str,
+        device_id: Optional[str] = None,
+        device_name: Optional[str] = None,
         start: datetime.datetime,
         end: datetime.datetime,
         topics: List[str] = [],
         output_format: OutputFormat = OutputFormat.mcap0,
         callback: Optional[ProgressCallback] = None,
     ) -> bytes:
         """
         Returns raw data bytes for a device and time range.
 
         device_id: The id of the device that originated the desired data.
+        device_name: The name of the device that originated the desired data.
         start: The earliest time from which to retrieve data.
         end: The latest time from which to retrieve data.
         topics: An optional list of topics to retrieve.
             All topics will be retrieved if this is omitted.
         output_format: The output format of the data, either .bag or .mcap, defaulting to .mcap.
         """
         params = {
-            "deviceId": device_id,
+            "device.id": device_id,
+            "device.name": device_name,
             "end": end.astimezone().isoformat(),
             "outputFormat": output_format.value,
             "start": start.astimezone().isoformat(),
             "topics": topics,
         }
         link_response = requests.post(
             self.__url__("/v1/data/stream"),
@@ -373,55 +395,65 @@
 
     def get_coverage(
         self,
         *,
         start: datetime.datetime,
         end: datetime.datetime,
         device_id: Optional[str] = None,
+        device_name: Optional[str] = None,
         tolerance: Optional[int] = None,
     ):
         """
         List coverage ranges for data.
 
         :param start: The earliest time after which to retrieve data.
         :param end: The latest time before which to retrieve data.
         :param device_id: Optional device id to limit data by.
         :param tolerance: Minimum interval (in seconds) that ranges must be separated by
             to be considered discrete.
         """
         params = {
-            "deviceId": device_id,
+            "device.id": device_id,
+            "device.name": device_name,
             "tolerance": tolerance,
             "start": start.astimezone().isoformat(),
             "end": end.astimezone().isoformat(),
         }
         response = requests.get(
             self.__url__("/v1/data/coverage"),
             headers=self.__headers,
             params={k: v for k, v in params.items() if v is not None},
         )
         json = json_or_raise(response)
 
         return [
             {
                 "device_id": c["deviceId"],
+                "device": c["device"],
                 "start": arrow.get(c["start"]).datetime,
                 "end": arrow.get(c["end"]).datetime,
             }
             for c in json
         ]
 
-    def get_device(self, *, device_id: str):
+    def get_device(
+        self, *, device_id: Optional[str] = None, device_name: Optional[str] = None
+    ):
         """
-        Gets a single device by id.
+        Gets a single device by name or id.
 
         :param device_id: The id of the device to retrieve.
+        :param device_name: The name of the device to retrieve.
         """
+        if device_name and device_id:
+            raise RuntimeError("device_id and device_name are mutually exclusive")
+        if device_name is None and device_id is None:
+            raise RuntimeError("device_id or device_name must be provided")
         response = requests.get(
-            self.__url__(f"/v1/devices/{device_id}"),
+            self.__url__(f"/v1/devices/{device_name or device_id}"),
             headers=self.__headers,
         )
 
         device = json_or_raise(response)
 
         return {
             "id": device["id"],
@@ -470,24 +502,31 @@
         device = json_or_raise(response)
 
         return {
             "id": device["id"],
             "name": device["name"],
         }
 
-    def delete_device(self, *, device_id: str):
+    def delete_device(
+        self, *, device_id: Optional[str] = None, device_name: Optional[str] = None
+    ):
         """
         Deletes an existing device.
 
         Note: you must first delete all imports from the device; see `delete_import`.
 
         :param device_id: The id of the device.
+        :param device_name: The name of the device.
         """
+        if device_name and device_id:
+            raise RuntimeError("device_id and device_name are mutually exclusive")
+        if device_name is None and device_id is None:
+            raise RuntimeError("device_id or device_name must be provided")
         response = requests.delete(
-            self.__url__(f"/v1/devices/{device_id}"),
+            self.__url__(f"/v1/devices/{device_name or device_id}"),
             headers=self.__headers,
         )
         json_or_raise(response)
 
     def delete_import(self, *, device_id: Optional[str] = None, import_id: str):
         """
         Deletes an existing import.
@@ -567,28 +606,30 @@
             for i in json
         ]
 
     def get_recordings(
         self,
         *,
         device_id: Optional[str] = None,
+        device_name: Optional[str] = None,
         start: Optional[datetime.datetime] = None,
         end: Optional[datetime.datetime] = None,
         path: Optional[str] = None,
         site_id: Optional[str] = None,
         edge_site_id: Optional[str] = None,
         import_status: Optional[str] = None,
         limit: Optional[int] = None,
         offset: Optional[int] = None,
         sort_by: Optional[str] = None,
         sort_order: Optional[str] = None,
     ):
         """Fetches recordings.
 
         :param device_id: Optionally filter responses by this device ID.
+        :param device_name: Optionally filter responses by this device name.
         :param start: Optionally specify the start of an inclusive time range.
             Only recordings with messages within this time range will be returned.
         :param end: Optionally specify the end of an inclusive time range.
             Only recordings with messages within this time range will be returned.
         :param path: Optionally filter responses to recordings with a matching path.
         :param site_id: Optionally filter responses to recordings stored at this primary site.
         :param edge_site_id: Optionally filter responses to recordings stored at this edge site.
@@ -597,14 +638,15 @@
             Specifying duration sorts by the duration between the recording start and end fields.
         :param sort_order: Optionally specify the sort order, either "asc" or "desc".
         :param limit: Optionally limit the number of records returned.
         :param offset: Optionally offset the results by this many records.
         """
         all_params = {
             "device.id": device_id,
+            "device.name": device_name,
             "start": start.astimezone().isoformat() if start else None,
             "end": end.astimezone().isoformat() if end else None,
             "site.id": site_id,
             "edgeSite.id": edge_site_id,
             "importStatus": import_status,
             "path": path,
             "sortBy": camelize(sort_by),
@@ -644,34 +686,37 @@
 
         return out
 
     def get_attachments(
         self,
         *,
         device_id: Optional[str] = None,
+        device_name: Optional[str] = None,
         recording_id: Optional[str] = None,
         site_id: Optional[str] = None,
         limit: Optional[int] = None,
         offset: Optional[int] = None,
         sort_by: Optional[str] = None,
         sort_order: Optional[str] = None,
     ):
         """List recording attachments.
 
         :param device_id: Optionally filter responses by this device ID.
+        :param device_name: Optionally filter responses by this device name.
         :param recording_id: Optionally filter responses by this recording ID.
         :param site_id: Optionally filter responses by this site ID.
         :param sort_by: Optionally sort responses by this field name.
             currently only "log_time" is supported.
         :param sort_order: Optionally specify the sort order, either "asc" or "desc".
         :param limit: Optionally limit the number of records returned.
         :param offset: Optionally offset the results by this many records.
         """
         all_params = {
-            "deviceId": device_id,
+            "device.id": device_id,
+            "device.name": device_name,
             "siteId": site_id,
             "recordingId": recording_id,
             "sortBy": camelize(sort_by),
             "sortOrder": sort_order,
             "limit": limit,
             "offset": offset,
         }
@@ -681,14 +726,15 @@
             headers=self.__headers,
         )
         json = json_or_raise(response)
         return [
             {
                 "id": i["id"],
                 "recording_id": i["recordingId"],
+                "device": i["device"],
                 "site_id": i["siteId"],
                 "name": i["name"],
                 "media_type": i["mediaType"],
                 "size": i["size"],
                 "crc": i["crc"],
                 "fingerprint": i["fingerprint"],
                 "log_time": arrow.get(i["logTime"]).datetime,
@@ -714,24 +760,26 @@
             headers=self.__headers,
             callback=callback,
         )
 
     def get_topics(
         self,
         *,
-        device_id: str,
+        device_id: Optional[str] = None,
+        device_name: Optional[str] = None,
         start: datetime.datetime,
         end: datetime.datetime,
         include_schemas: bool = False,
     ):
         response = requests.get(
             self.__url__("/v1/data/topics"),
             headers=self.__headers,
             params={
-                "deviceId": device_id,
+                "device.id": device_id,
+                "device.name": device_name,
                 "start": start.astimezone().isoformat(),
                 "end": end.astimezone().isoformat(),
                 "includeSchemas": "true" if include_schemas else "false",
             },
         )
 
         json = json_or_raise(response)
@@ -749,33 +797,36 @@
                 result["schema"] = base64.b64decode(t["schema"])
             results.append(result)
         return results
 
     def upload_data(
         self,
         *,
-        device_id: str,
+        device_id: Optional[str] = None,
+        device_name: Optional[str] = None,
         filename: str,
         data: Union[bytes, IO[Any]],
         callback: Optional[SizeProgressCallback] = None,
     ):
         """
         Uploads data in bytes.
 
         device_id: Device id of the device from which this data originated.
+        device_name: Name id of the device from which this data originated.
         filename: A filename to associate with the data. The data format will be
             inferred from the file extension.
         data: The raw data in .bag or .mcap format.
         callback: An optional callback to report progress on the upload.
         """
         link_response = requests.post(
             self.__url__("/v1/data/upload"),
             headers=self.__headers,
             json={
-                "deviceId": device_id,
+                "device.id": device_id,
+                "device.name": device_name,
                 "filename": filename,
             },
         )
 
         json = json_or_raise(link_response)
 
         link = json["link"]
@@ -792,14 +843,15 @@
         }
 
 
 def _event_dict(json_event):
     return {
         "id": json_event["id"],
         "device_id": json_event["deviceId"],
+        "device": json_event["device"],
         "start": arrow.get(json_event["start"]).datetime,
         "end": arrow.get(json_event["end"]).datetime,
         "metadata": json_event["metadata"],
         "created_at": arrow.get(json_event["createdAt"]).datetime,
         "updated_at": arrow.get(json_event["updatedAt"]).datetime,
     }
```

### Comparing `foxglove-data-platform-0.7.0/foxglove_data_platform.egg-info/PKG-INFO` & `foxglove-data-platform-0.8.0/foxglove_data_platform.egg-info/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: foxglove-data-platform
-Version: 0.7.0
+Version: 0.8.0
 Summary: Client library for Foxglove Data Platform.
 Home-page: https://github.com/foxglove/py-data-platform
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
```

### Comparing `foxglove-data-platform-0.7.0/foxglove_data_platform.egg-info/SOURCES.txt` & `foxglove-data-platform-0.8.0/foxglove_data_platform.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `foxglove-data-platform-0.7.0/setup.cfg` & `foxglove-data-platform-0.8.0/setup.cfg`

 * *Files 19% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [metadata]
 name = foxglove-data-platform
-version = 0.7.0
+version = 0.8.0
 description = Client library for Foxglove Data Platform.
 long_description = file: README.md
 long_description_content_type = text/markdown
 url = https://github.com/foxglove/py-data-platform
 classifiers = 
 	Programming Language :: Python :: 3
 	License :: OSI Approved :: MIT License
```

### Comparing `foxglove-data-platform-0.7.0/tests/generate.py` & `foxglove-data-platform-0.8.0/tests/generate.py`

 * *Files identical despite different names*

### Comparing `foxglove-data-platform-0.7.0/tests/string_message_pb2.py` & `foxglove-data-platform-0.8.0/tests/string_message_pb2.py`

 * *Files identical despite different names*

### Comparing `foxglove-data-platform-0.7.0/tests/test_attachments.py` & `foxglove-data-platform-0.8.0/tests/test_attachments.py`

 * *Files 4% similar despite different names*

```diff
@@ -8,14 +8,15 @@
 
 fake = Faker()
 
 
 @responses.activate
 def test_get_attachments():
     device_id = fake.uuid4()
+    device_name = fake.name()
     attachment_id = fake.uuid4()
     recording_id = fake.uuid4()
     path = fake.file_name(extension="txt")
     media_type = fake.mime_type()
     size = fake.random_number()
     crc = fake.random_number()
     fingerprint = fake.uuid4()
@@ -25,14 +26,15 @@
     responses.add(
         responses.GET,
         api_url(f"/v1/recording-attachments"),
         json=[
             {
                 "id": attachment_id,
                 "recordingId": recording_id,
+                "device": {"id": device_id, "name": device_name},
                 "siteId": site_id,
                 "name": path,
                 "mediaType": media_type,
                 "size": size,
                 "crc": crc,
                 "fingerprint": fingerprint,
                 "logTime": now.isoformat(),
@@ -47,14 +49,18 @@
     )
     assert attachments == [
         {
             "id": attachment_id,
             "recording_id": recording_id,
             "site_id": site_id,
             "name": path,
+            "device": {
+                "id": device_id,
+                "name": device_name,
+            },
             "media_type": media_type,
             "size": size,
             "crc": crc,
             "fingerprint": fingerprint,
             "log_time": now,
             "create_time": now,
         },
```

### Comparing `foxglove-data-platform-0.7.0/tests/test_client.py` & `foxglove-data-platform-0.8.0/tests/test_client.py`

 * *Files 12% similar despite different names*

```diff
@@ -24,29 +24,33 @@
     with pytest.raises(RequestException) as exception:
         client.get_coverage(start=datetime.now(), end=datetime.now())
     assert exception.value.response.reason == reason
 
 
 @responses.activate
 def test_get_coverage():
+    device_id = fake.uuid4()
+    device_name = fake.name()
     responses.add(
         responses.GET,
         api_url("/v1/data/coverage"),
         json=[
             {
-                "deviceId": "device_id",
+                "deviceId": device_id,
+                "device": {"id": device_id, "name": device_name},
                 "start": datetime.now().isoformat(),
                 "end": datetime.now().isoformat(),
             }
         ],
     )
     client = Client("test")
     coverage_response = client.get_coverage(start=datetime.now(), end=datetime.now())
     assert len(coverage_response) == 1
-    assert coverage_response[0]["device_id"] == "device_id"
+    assert coverage_response[0]["device_id"] == device_id
+    assert coverage_response[0]["device"] == {"id": device_id, "name": device_name}
 
 
 @responses.activate
 def test_get_topics():
     responses.add(
         responses.GET,
         api_url("/v1/data/topics"),
```

### Comparing `foxglove-data-platform-0.7.0/tests/test_coverage.py` & `foxglove-data-platform-0.8.0/tests/test_coverage.py`

 * *Files 16% similar despite different names*

```diff
@@ -8,25 +8,28 @@
 
 fake = Faker()
 
 
 @responses.activate
 def test_get_coverage():
     device_id = fake.uuid4()
+    device_name = fake.name()
     responses.add(
         responses.GET,
         api_url(f"/v1/data/coverage"),
         json=[
             {
                 "deviceId": device_id,
+                "device": {"id": device_id, "name": device_name},
                 "start": datetime.now().isoformat(),
                 "end": datetime.now().isoformat(),
             },
             {
                 "deviceId": device_id,
+                "device": {"id": device_id, "name": device_name},
                 "start": datetime.now().isoformat(),
                 "end": datetime.now().isoformat(),
             },
         ],
     )
     client = Client("test")
     coverage = client.get_coverage(
```

### Comparing `foxglove-data-platform-0.7.0/tests/test_data.py` & `foxglove-data-platform-0.8.0/tests/test_data.py`

 * *Files identical despite different names*

### Comparing `foxglove-data-platform-0.7.0/tests/test_devices.py` & `foxglove-data-platform-0.8.0/tests/test_devices.py`

 * *Files 8% similar despite different names*

```diff
@@ -25,28 +25,42 @@
     device = client.create_device(name=name)
     assert device["name"] == name
 
 
 @responses.activate
 def test_get_device():
     id = fake.uuid4()
+    name = "name"
     responses.add(
         responses.GET,
         api_url(f"/v1/devices/{id}"),
         json={
             "id": id,
             "name": fake.sentence(2),
             "createdAt": datetime.now().isoformat(),
             "updatedAt": datetime.now().isoformat(),
         },
     )
     client = Client("test")
     device = client.get_device(device_id=id)
     assert device["id"] == id
 
+    responses.add(
+        responses.GET,
+        api_url(f"/v1/devices/{name}"),
+        json={
+            "id": id,
+            "name": fake.sentence(2),
+            "createdAt": datetime.now().isoformat(),
+            "updatedAt": datetime.now().isoformat(),
+        },
+    )
+    device = client.get_device(device_name=name)
+    assert device["id"] == id
+
 
 @responses.activate
 def test_get_devices():
     id = fake.uuid4()
     responses.add(
         responses.GET,
         api_url("/v1/devices"),
@@ -64,17 +78,28 @@
     assert len(devices) == 1
     assert devices[0]["id"] == id
 
 
 @responses.activate
 def test_delete_device():
     id = fake.uuid4()
+    name = "name"
     responses.add(
         responses.DELETE,
         api_url(f"/v1/devices/{id}"),
         json={"success": True},
     )
     client = Client("test")
     try:
         client.delete_device(device_id=id)
     except:
         assert False
+
+    responses.add(
+        responses.DELETE,
+        api_url(f"/v1/devices/{name}"),
+        json={"success": True},
+    )
+    try:
+        client.delete_device(device_name=name)
+    except:
+        assert False
```

### Comparing `foxglove-data-platform-0.7.0/tests/test_imports.py` & `foxglove-data-platform-0.8.0/tests/test_imports.py`

 * *Files identical despite different names*

### Comparing `foxglove-data-platform-0.7.0/tests/test_protobuf_messages.py` & `foxglove-data-platform-0.8.0/tests/test_protobuf_messages.py`

 * *Files identical despite different names*

### Comparing `foxglove-data-platform-0.7.0/tests/test_recordings.py` & `foxglove-data-platform-0.8.0/tests/test_recordings.py`

 * *Files identical despite different names*

### Comparing `foxglove-data-platform-0.7.0/tests/test_ros1_messages.py` & `foxglove-data-platform-0.8.0/tests/test_ros1_messages.py`

 * *Files identical despite different names*

### Comparing `foxglove-data-platform-0.7.0/tests/test_ros2_messages.py` & `foxglove-data-platform-0.8.0/tests/test_ros2_messages.py`

 * *Files identical despite different names*

