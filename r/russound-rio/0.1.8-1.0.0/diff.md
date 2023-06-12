# Comparing `tmp/russound_rio-0.1.8.tar.gz` & `tmp/russound_rio-1.0.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "russound_rio-0.1.8.tar", last modified: Mon Jul 18 23:22:38 2022, max compression
+gzip compressed data, was "russound_rio-1.0.0.tar", last modified: Mon Jun 12 20:04:59 2023, max compression
```

## Comparing `russound_rio-0.1.8.tar` & `russound_rio-1.0.0.tar`

### file list

```diff
@@ -1,15 +1,17 @@
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-07-18 23:22:38.757357 russound_rio-0.1.8/
--rw-r--r--   0 runner    (1001) docker     (121)     1070 2022-07-18 23:22:29.000000 russound_rio-0.1.8/LICENSE
--rw-r--r--   0 runner    (1001) docker     (121)       20 2022-07-18 23:22:29.000000 russound_rio-0.1.8/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (121)      712 2022-07-18 23:22:38.757357 russound_rio-0.1.8/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)      495 2022-07-18 23:22:29.000000 russound_rio-0.1.8/README.rst
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-07-18 23:22:38.757357 russound_rio-0.1.8/russound_rio/
--rw-r--r--   0 runner    (1001) docker     (121)      171 2022-07-18 23:22:29.000000 russound_rio-0.1.8/russound_rio/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)    13986 2022-07-18 23:22:29.000000 russound_rio-0.1.8/russound_rio/rio.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-07-18 23:22:38.757357 russound_rio-0.1.8/russound_rio.egg-info/
--rw-r--r--   0 runner    (1001) docker     (121)      712 2022-07-18 23:22:38.000000 russound_rio-0.1.8/russound_rio.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)      228 2022-07-18 23:22:38.000000 russound_rio-0.1.8/russound_rio.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (121)        1 2022-07-18 23:22:38.000000 russound_rio-0.1.8/russound_rio.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (121)       13 2022-07-18 23:22:38.000000 russound_rio-0.1.8/russound_rio.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (121)       38 2022-07-18 23:22:38.757357 russound_rio-0.1.8/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (121)      360 2022-07-18 23:22:29.000000 russound_rio-0.1.8/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-12 20:04:59.136518 russound_rio-1.0.0/
+-rw-r--r--   0 runner    (1001) docker     (123)     1071 2023-06-12 20:04:46.000000 russound_rio-1.0.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)       20 2023-06-12 20:04:46.000000 russound_rio-1.0.0/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)      727 2023-06-12 20:04:59.136518 russound_rio-1.0.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      511 2023-06-12 20:04:46.000000 russound_rio-1.0.0/README.rst
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-12 20:04:59.132518 russound_rio-1.0.0/russound_rio/
+-rw-r--r--   0 runner    (1001) docker     (123)      171 2023-06-12 20:04:46.000000 russound_rio-1.0.0/russound_rio/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13651 2023-06-12 20:04:46.000000 russound_rio-1.0.0/russound_rio/rio.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-12 20:04:59.132518 russound_rio-1.0.0/russound_rio.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)      727 2023-06-12 20:04:59.000000 russound_rio-1.0.0/russound_rio.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      249 2023-06-12 20:04:59.000000 russound_rio-1.0.0/russound_rio.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-12 20:04:59.000000 russound_rio-1.0.0/russound_rio.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       13 2023-06-12 20:04:59.000000 russound_rio-1.0.0/russound_rio.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-12 20:04:59.136518 russound_rio-1.0.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      359 2023-06-12 20:04:46.000000 russound_rio-1.0.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-12 20:04:59.132518 russound_rio-1.0.0/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)      259 2023-06-12 20:04:46.000000 russound_rio-1.0.0/tests/test_zoneid.py
```

### Comparing `russound_rio-0.1.8/LICENSE` & `russound_rio-1.0.0/LICENSE`

 * *Files 23% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 MIT License
 
-Copyright (c) 2017 Martin Donlon
+Copyright (c) 2023 Chris Phillips
 
 Permission is hereby granted, free of charge, to any person obtaining a copy
 of this software and associated documentation files (the "Software"), to deal
 in the Software without restriction, including without limitation the rights
 to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
 copies of the Software, and to permit persons to whom the Software is
 furnished to do so, subject to the following conditions:
```

### Comparing `russound_rio-0.1.8/russound_rio/rio.py` & `russound_rio-1.0.0/russound_rio/rio.py`

 * *Files 18% similar despite different names*

```diff
@@ -150,24 +150,23 @@
             zone_id = ZoneID(controller=p['controller'], zone=p['zone'])
             self._store_cached_zone_variable(zone_id,
                                              p['variable'],
                                              p['value'])
 
         return ty, p['value']
 
-    @asyncio.coroutine
-    def _ioloop(self, reader, writer):
+    async def _ioloop(self, reader, writer):
         queue_future = ensure_future(
                 self._cmd_queue.get())
         net_future = ensure_future(
                 reader.readline())
         try:
             logger.debug("Starting IO loop")
             while True:
-                done, pending = yield from asyncio.wait(
+                done, pending = await asyncio.wait(
                         [queue_future, net_future],
                         return_when=asyncio.FIRST_COMPLETED)
 
                 if net_future in done:
                     response = net_future.result()
                     try:
                         self._process_response(response)
@@ -176,21 +175,21 @@
                     net_future = ensure_future(
                             reader.readline())
 
                 if queue_future in done:
                     cmd, future = queue_future.result()
                     cmd += '\r'
                     writer.write(bytearray(cmd, 'utf-8'))
-                    yield from writer.drain()
+                    await writer.drain()
 
                     queue_future = ensure_future(
                             self._cmd_queue.get())
 
                     while True:
-                        response = yield from net_future
+                        response = await net_future
                         net_future = ensure_future(
                                 reader.readline())
                         try:
                             ty, value = self._process_response(response)
                             if ty == 'S':
                                 future.set_result(value)
                                 break
@@ -204,19 +203,18 @@
             queue_future.cancel()
             net_future.cancel()
             raise
         except Exception:
             logger.exception("Unhandled exception in IO loop")
             raise
 
-    @asyncio.coroutine
-    def _send_cmd(self, cmd):
+    async def _send_cmd(self, cmd):
         future = asyncio.Future()
-        yield from self._cmd_queue.put((cmd, future))
-        r = yield from future
+        await self._cmd_queue.put((cmd, future))
+        r = await future
         return r
 
     def add_zone_callback(self, callback):
         """
         Registers a callback to be called whenever a zone variable changes.
         The callback will be passed three arguments: the zone_id, the variable
         name and the variable value.
@@ -239,162 +237,149 @@
 
     def remove_source_callback(self, source_id, callback):
         """
         Removes a previously registered zone callback.
         """
         self._source_callbacks.remove(callback)
 
-    @asyncio.coroutine
-    def connect(self):
+    async def connect(self):
         """
         Connect to the controller and start processing responses.
         """
         logger.info("Connecting to %s:%s", self._host, self._port)
-        reader, writer = yield from asyncio.open_connection(
+        reader, writer = await asyncio.open_connection(
                 self._host, self._port)
         self._ioloop_future = ensure_future(
                 self._ioloop(reader, writer))
         logger.info("Connected")
 
-    @asyncio.coroutine
-    def close(self):
+    async def close(self):
         """
         Disconnect from the controller.
         """
         logger.info("Closing connection to %s:%s", self._host, self._port)
         self._ioloop_future.cancel()
         try:
-            yield from self._ioloop_future
+            await self._ioloop_future
         except asyncio.CancelledError:
             pass
 
-    @asyncio.coroutine
-    def set_zone_variable(self, zone_id, variable, value):
+    async def set_zone_variable(self, zone_id, variable, value):
         """
         Set a zone variable to a new value.
         """
         return self._send_cmd("SET %s.%s=\"%s\"" % (
             zone_id.device_str(), variable, value))
 
-    @asyncio.coroutine
-    def get_zone_variable(self, zone_id, variable):
+    async def get_zone_variable(self, zone_id, variable):
         """ Retrieve the current value of a zone variable.  If the variable is
         not found in the local cache then the value is requested from the
         controller.  """
 
         try:
             return self._retrieve_cached_zone_variable(zone_id, variable)
         except UncachedVariable:
-            return (yield from self._send_cmd("GET %s.%s" % (
+            return (await self._send_cmd("GET %s.%s" % (
                 zone_id.device_str(), variable)))
 
     def get_cached_zone_variable(self, zone_id, variable, default=None):
         """ Retrieve the current value of a zone variable from the cache or
         return the default value if the variable is not present. """
 
         try:
             return self._retrieve_cached_zone_variable(zone_id, variable)
         except UncachedVariable:
             return default
 
-    @asyncio.coroutine
-    def watch_zone(self, zone_id):
+    async def watch_zone(self, zone_id):
         """ Add a zone to the watchlist.
         Zones on the watchlist will push all
         state changes (and those of the source they are currently connected to)
         back to the client """
-        r = yield from self._send_cmd(
+        r = await self._send_cmd(
                 "WATCH %s ON" % (zone_id.device_str(), ))
         self._watched_zones.add(zone_id)
         return r
 
-    @asyncio.coroutine
-    def unwatch_zone(self, zone_id):
+    async def unwatch_zone(self, zone_id):
         """ Remove a zone from the watchlist. """
         self._watched_zones.remove(zone_id)
-        return (yield from
+        return (await
                 self._send_cmd("WATCH %s OFF" % (zone_id.device_str(), )))
 
-    @asyncio.coroutine
-    def send_zone_event(self, zone_id, event_name, *args):
+    async def send_zone_event(self, zone_id, event_name, *args):
         """ Send an event to a zone. """
         cmd = "EVENT %s!%s %s" % (
                 zone_id.device_str(), event_name,
                 " ".join(str(x) for x in args))
-        return (yield from self._send_cmd(cmd))
+        return (await self._send_cmd(cmd))
 
-    @asyncio.coroutine
-    def enumerate_zones(self):
+    async def enumerate_zones(self):
         """ Return a list of (zone_id, zone_name) tuples """
         zones = []
         for controller in range(1, 8):
             for zone in range(1, 17):
                 zone_id = ZoneID(zone, controller)
                 try:
-                    name = yield from self.get_zone_variable(zone_id, 'name')
+                    name = await self.get_zone_variable(zone_id, 'name')
                     if name:
                         zones.append((zone_id, name))
                 except CommandException:
                     break
         return zones
 
-    @asyncio.coroutine
-    def set_source_variable(self, source_id, variable, value):
+    async def set_source_variable(self, source_id, variable, value):
         """ Change the value of a source variable. """
         source_id = int(source_id)
         return self._send_cmd("SET S[%d].%s=\"%s\"" % (
             source_id, variable, value))
 
-    @asyncio.coroutine
-    def get_source_variable(self, source_id, variable):
+    async def get_source_variable(self, source_id, variable):
         """ Get the current value of a source variable. If the variable is not
         in the cache it will be retrieved from the controller. """
 
         source_id = int(source_id)
         try:
             return self._retrieve_cached_source_variable(
                     source_id, variable)
         except UncachedVariable:
-            return (yield from self._send_cmd("GET S[%d].%s" % (
+            return (await self._send_cmd("GET S[%d].%s" % (
                 source_id, variable)))
 
     def get_cached_source_variable(self, source_id, variable, default=None):
         """ Get the cached value of a source variable. If the variable is not
         cached return the default value. """
 
         source_id = int(source_id)
         try:
             return self._retrieve_cached_source_variable(
                     source_id, variable)
         except UncachedVariable:
             return default
 
-    @asyncio.coroutine
-    def watch_source(self, source_id):
+    async def watch_source(self, source_id):
         """ Add a souce to the watchlist. """
         source_id = int(source_id)
-        r = yield from self._send_cmd(
+        r = await self._send_cmd(
                 "WATCH S[%d] ON" % (source_id, ))
         self._watched_source.add(source_id)
         return r
 
-    @asyncio.coroutine
-    def unwatch_source(self, source_id):
+    async def unwatch_source(self, source_id):
         """ Remove a souce from the watchlist. """
         source_id = int(source_id)
         self._watched_sources.remove(source_id)
-        return (yield from
+        return (await
                 self._send_cmd("WATCH S[%d] OFF" % (
                     source_id, )))
 
-    @asyncio.coroutine
-    def enumerate_sources(self):
+    async def enumerate_sources(self):
         """ Return a list of (source_id, source_name) tuples """
         sources = []
         for source_id in range(1, 17):
             try:
-                name = yield from self.get_source_variable(source_id, 'name')
+                name = await self.get_source_variable(source_id, 'name')
                 if name:
                     sources.append((source_id, name))
             except CommandException:
                 break
         return sources
```

