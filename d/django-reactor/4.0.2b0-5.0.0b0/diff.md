# Comparing `tmp/django-reactor-4.0.2b0.tar.gz` & `tmp/django-reactor-5.0.0b0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "django-reactor-4.0.2b0.tar", last modified: Thu Jun  1 11:51:42 2023, max compression
+gzip compressed data, was "django-reactor-5.0.0b0.tar", last modified: Mon Jun 12 07:51:20 2023, max compression
```

## Comparing `django-reactor-4.0.2b0.tar` & `django-reactor-5.0.0b0.tar`

### file list

```diff
@@ -1,36 +1,36 @@
-drwxr-xr-x   0 xigurat   (1000) xigurat   (1001)        0 2023-06-01 11:51:42.263051 django-reactor-4.0.2b0/
--rw-r--r--   0 xigurat   (1000) xigurat   (1001)       72 2023-06-01 09:36:11.000000 django-reactor-4.0.2b0/MANIFEST.in
--rw-r--r--   0 xigurat   (1000) xigurat   (1001)    17217 2023-06-01 11:51:42.263051 django-reactor-4.0.2b0/PKG-INFO
--rw-r--r--   0 xigurat   (1000) xigurat   (1001)    16358 2023-06-01 09:30:39.000000 django-reactor-4.0.2b0/README.md
-drwxr-xr-x   0 xigurat   (1000) xigurat   (1001)        0 2023-06-01 11:51:42.259718 django-reactor-4.0.2b0/django_reactor.egg-info/
--rw-r--r--   0 xigurat   (1000) xigurat   (1001)    17217 2023-06-01 11:51:42.000000 django-reactor-4.0.2b0/django_reactor.egg-info/PKG-INFO
--rw-r--r--   0 xigurat   (1000) xigurat   (1001)      683 2023-06-01 11:51:42.000000 django-reactor-4.0.2b0/django_reactor.egg-info/SOURCES.txt
--rw-r--r--   0 xigurat   (1000) xigurat   (1001)        1 2023-06-01 11:51:42.000000 django-reactor-4.0.2b0/django_reactor.egg-info/dependency_links.txt
--rw-r--r--   0 xigurat   (1000) xigurat   (1001)        1 2023-06-01 11:50:12.000000 django-reactor-4.0.2b0/django_reactor.egg-info/not-zip-safe
--rw-r--r--   0 xigurat   (1000) xigurat   (1001)      161 2023-06-01 11:51:42.000000 django-reactor-4.0.2b0/django_reactor.egg-info/requires.txt
--rw-r--r--   0 xigurat   (1000) xigurat   (1001)        8 2023-06-01 11:51:42.000000 django-reactor-4.0.2b0/django_reactor.egg-info/top_level.txt
--rw-r--r--   0 xigurat   (1000) xigurat   (1001)      478 2023-05-31 14:49:19.000000 django-reactor-4.0.2b0/pyproject.toml
-drwxr-xr-x   0 xigurat   (1000) xigurat   (1001)        0 2023-06-01 11:51:42.263051 django-reactor-4.0.2b0/reactor/
--rw-r--r--   0 xigurat   (1000) xigurat   (1001)        0 2023-05-31 13:32:27.000000 django-reactor-4.0.2b0/reactor/__init__.py
--rw-r--r--   0 xigurat   (1000) xigurat   (1001)      291 2023-05-31 13:32:27.000000 django-reactor-4.0.2b0/reactor/apps.py
--rw-r--r--   0 xigurat   (1000) xigurat   (1001)     5598 2022-07-30 12:06:00.000000 django-reactor-4.0.2b0/reactor/auto_broadcast.py
--rw-r--r--   0 xigurat   (1000) xigurat   (1001)    12284 2023-05-31 13:32:27.000000 django-reactor-4.0.2b0/reactor/component.py
--rw-r--r--   0 xigurat   (1000) xigurat   (1001)     6382 2023-05-31 13:32:27.000000 django-reactor-4.0.2b0/reactor/consumer.py
--rw-r--r--   0 xigurat   (1000) xigurat   (1001)     3933 2022-07-30 12:06:00.000000 django-reactor-4.0.2b0/reactor/event_transpiler.py
--rw-r--r--   0 xigurat   (1000) xigurat   (1001)     1123 2022-07-30 12:06:00.000000 django-reactor-4.0.2b0/reactor/fields.py
--rw-r--r--   0 xigurat   (1000) xigurat   (1001)      411 2023-05-31 13:32:27.000000 django-reactor-4.0.2b0/reactor/log.py
--rw-r--r--   0 xigurat   (1000) xigurat   (1001)     2553 2023-05-31 13:32:27.000000 django-reactor-4.0.2b0/reactor/repository.py
--rw-r--r--   0 xigurat   (1000) xigurat   (1001)      434 2022-07-30 12:06:00.000000 django-reactor-4.0.2b0/reactor/serializer.py
--rw-r--r--   0 xigurat   (1000) xigurat   (1001)     1462 2023-05-31 13:32:27.000000 django-reactor-4.0.2b0/reactor/settings.py
-drwxr-xr-x   0 xigurat   (1000) xigurat   (1001)        0 2023-06-01 11:51:42.259718 django-reactor-4.0.2b0/reactor/static/
-drwxr-xr-x   0 xigurat   (1000) xigurat   (1001)        0 2023-06-01 11:51:42.263051 django-reactor-4.0.2b0/reactor/static/reactor/
--rw-r--r--   0 xigurat   (1000) xigurat   (1001)    21841 2023-05-31 14:25:44.000000 django-reactor-4.0.2b0/reactor/static/reactor/reactor.min.js
-drwxr-xr-x   0 xigurat   (1000) xigurat   (1001)        0 2023-06-01 11:51:42.263051 django-reactor-4.0.2b0/reactor/templates/
--rw-r--r--   0 xigurat   (1000) xigurat   (1001)      444 2022-07-30 12:06:00.000000 django-reactor-4.0.2b0/reactor/templates/reactor_header.html
-drwxr-xr-x   0 xigurat   (1000) xigurat   (1001)        0 2023-06-01 11:51:42.263051 django-reactor-4.0.2b0/reactor/templatetags/
--rw-r--r--   0 xigurat   (1000) xigurat   (1001)        0 2022-07-30 12:06:00.000000 django-reactor-4.0.2b0/reactor/templatetags/__init__.py
--rw-r--r--   0 xigurat   (1000) xigurat   (1001)     3514 2023-05-31 13:32:27.000000 django-reactor-4.0.2b0/reactor/templatetags/reactor.py
--rw-r--r--   0 xigurat   (1000) xigurat   (1001)      165 2022-07-30 12:06:00.000000 django-reactor-4.0.2b0/reactor/urls.py
--rw-r--r--   0 xigurat   (1000) xigurat   (1001)     2806 2022-07-30 12:06:00.000000 django-reactor-4.0.2b0/reactor/utils.py
--rw-r--r--   0 xigurat   (1000) xigurat   (1001)     1316 2023-06-01 11:51:42.263051 django-reactor-4.0.2b0/setup.cfg
--rw-r--r--   0 xigurat   (1000) xigurat   (1001)       39 2023-06-01 09:29:36.000000 django-reactor-4.0.2b0/setup.py
+drwxr-xr-x   0 xigurat   (1000) xigurat   (1001)        0 2023-06-12 07:51:20.094159 django-reactor-5.0.0b0/
+-rw-r--r--   0 xigurat   (1000) xigurat   (1001)       72 2023-06-01 12:00:36.000000 django-reactor-5.0.0b0/MANIFEST.in
+-rw-r--r--   0 xigurat   (1000) xigurat   (1001)    16764 2023-06-12 07:51:20.094159 django-reactor-5.0.0b0/PKG-INFO
+-rw-r--r--   0 xigurat   (1000) xigurat   (1001)    15905 2023-06-10 22:13:11.000000 django-reactor-5.0.0b0/README.md
+drwxr-xr-x   0 xigurat   (1000) xigurat   (1001)        0 2023-06-12 07:51:20.094159 django-reactor-5.0.0b0/django_reactor.egg-info/
+-rw-r--r--   0 xigurat   (1000) xigurat   (1001)    16764 2023-06-12 07:51:20.000000 django-reactor-5.0.0b0/django_reactor.egg-info/PKG-INFO
+-rw-r--r--   0 xigurat   (1000) xigurat   (1001)      684 2023-06-12 07:51:20.000000 django-reactor-5.0.0b0/django_reactor.egg-info/SOURCES.txt
+-rw-r--r--   0 xigurat   (1000) xigurat   (1001)        1 2023-06-12 07:51:20.000000 django-reactor-5.0.0b0/django_reactor.egg-info/dependency_links.txt
+-rw-r--r--   0 xigurat   (1000) xigurat   (1001)        1 2023-06-01 11:50:12.000000 django-reactor-5.0.0b0/django_reactor.egg-info/not-zip-safe
+-rw-r--r--   0 xigurat   (1000) xigurat   (1001)      180 2023-06-12 07:51:20.000000 django-reactor-5.0.0b0/django_reactor.egg-info/requires.txt
+-rw-r--r--   0 xigurat   (1000) xigurat   (1001)        8 2023-06-12 07:51:20.000000 django-reactor-5.0.0b0/django_reactor.egg-info/top_level.txt
+-rw-r--r--   0 xigurat   (1000) xigurat   (1001)      451 2023-06-10 22:13:11.000000 django-reactor-5.0.0b0/pyproject.toml
+drwxr-xr-x   0 xigurat   (1000) xigurat   (1001)        0 2023-06-12 07:51:20.094159 django-reactor-5.0.0b0/reactor/
+-rw-r--r--   0 xigurat   (1000) xigurat   (1001)        0 2023-05-31 13:32:27.000000 django-reactor-5.0.0b0/reactor/__init__.py
+-rw-r--r--   0 xigurat   (1000) xigurat   (1001)      291 2023-06-06 12:12:16.000000 django-reactor-5.0.0b0/reactor/apps.py
+-rw-r--r--   0 xigurat   (1000) xigurat   (1001)     5661 2023-06-10 22:13:11.000000 django-reactor-5.0.0b0/reactor/auto_broadcast.py
+-rw-r--r--   0 xigurat   (1000) xigurat   (1001)    13782 2023-06-10 22:13:11.000000 django-reactor-5.0.0b0/reactor/component.py
+-rw-r--r--   0 xigurat   (1000) xigurat   (1001)     6125 2023-06-10 22:13:11.000000 django-reactor-5.0.0b0/reactor/consumer.py
+-rw-r--r--   0 xigurat   (1000) xigurat   (1001)     3990 2023-06-12 07:48:44.000000 django-reactor-5.0.0b0/reactor/event_transpiler.py
+-rw-r--r--   0 xigurat   (1000) xigurat   (1001)      411 2023-05-31 13:32:27.000000 django-reactor-5.0.0b0/reactor/log.py
+-rw-r--r--   0 xigurat   (1000) xigurat   (1001)     3045 2023-06-10 22:13:11.000000 django-reactor-5.0.0b0/reactor/repository.py
+-rw-r--r--   0 xigurat   (1000) xigurat   (1001)      874 2023-06-10 22:13:11.000000 django-reactor-5.0.0b0/reactor/schemas.py
+-rw-r--r--   0 xigurat   (1000) xigurat   (1001)      765 2023-06-10 22:13:11.000000 django-reactor-5.0.0b0/reactor/serializer.py
+-rw-r--r--   0 xigurat   (1000) xigurat   (1001)      590 2023-06-12 07:48:55.000000 django-reactor-5.0.0b0/reactor/settings.py
+drwxr-xr-x   0 xigurat   (1000) xigurat   (1001)        0 2023-06-12 07:51:20.094159 django-reactor-5.0.0b0/reactor/static/
+drwxr-xr-x   0 xigurat   (1000) xigurat   (1001)        0 2023-06-12 07:51:20.094159 django-reactor-5.0.0b0/reactor/static/reactor/
+-rw-r--r--   0 xigurat   (1000) xigurat   (1001)    22594 2023-06-12 07:51:19.000000 django-reactor-5.0.0b0/reactor/static/reactor/reactor.min.js
+drwxr-xr-x   0 xigurat   (1000) xigurat   (1001)        0 2023-06-12 07:51:20.094159 django-reactor-5.0.0b0/reactor/templates/
+-rw-r--r--   0 xigurat   (1000) xigurat   (1001)      444 2022-07-30 12:06:00.000000 django-reactor-5.0.0b0/reactor/templates/reactor_header.html
+drwxr-xr-x   0 xigurat   (1000) xigurat   (1001)        0 2023-06-12 07:51:20.094159 django-reactor-5.0.0b0/reactor/templatetags/
+-rw-r--r--   0 xigurat   (1000) xigurat   (1001)        0 2022-07-30 12:06:00.000000 django-reactor-5.0.0b0/reactor/templatetags/__init__.py
+-rw-r--r--   0 xigurat   (1000) xigurat   (1001)     3524 2023-06-10 22:13:11.000000 django-reactor-5.0.0b0/reactor/templatetags/reactor.py
+-rw-r--r--   0 xigurat   (1000) xigurat   (1001)      165 2022-07-30 12:06:00.000000 django-reactor-5.0.0b0/reactor/urls.py
+-rw-r--r--   0 xigurat   (1000) xigurat   (1001)     2733 2023-06-10 22:13:11.000000 django-reactor-5.0.0b0/reactor/utils.py
+-rw-r--r--   0 xigurat   (1000) xigurat   (1001)     1336 2023-06-12 07:51:20.097492 django-reactor-5.0.0b0/setup.cfg
+-rw-r--r--   0 xigurat   (1000) xigurat   (1001)       39 2023-06-01 09:29:36.000000 django-reactor-5.0.0b0/setup.py
```

### Comparing `django-reactor-4.0.2b0/PKG-INFO` & `django-reactor-5.0.0b0/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: django-reactor
-Version: 4.0.2b0
+Version: 5.0.0b0
 Summary: Brings LiveView from Phoenix framework into Django
 Home-page: https://github.com/edelvalle/reactor
 Author: Eddy Ernesto del Valle Pino
 Author-email: eddy@edelvalle.me
 License: MIT
 Classifier: Development Status :: 4 - Beta
 Classifier: Environment :: Web Environment
@@ -187,47 +187,45 @@
 ```
 
 ## Settings:
 
 Default settings of reactor are:
 
 ```python
+
+from reactor.schemas import AutoBroadcast
+
 REACTOR = {
+    "TRANSPILER_CACHE_SIZE": 1024,
     "USE_HTML_DIFF": True,
     "USE_HMIN": False,
     "BOOST_PAGES": False,
-    "RECEIVER_PREFIX": "recv_",
     "TRANSPILER_CACHE_NAME": "reactor:transpiler",
-    "AUTO_BROADCAST": False,
+    "AUTO_BROADCAST": AutoBroadcast(
+        # model-a
+        model: bool = False
+        # model-a.1234
+        model_pk: bool = False
+        # model-b.9876.model-a-set
+        related: bool = False
+        # model-b.9876.model-a-set
+        # model-a.1234.model-b-set
+        m2m: bool = False
+        # this is a set of tuples of ('app_label', 'ModelName')
+        # to subscribe for the auto broadcast
+        senders: set[tuple[str, str]] = Field(default_factory=set)
+    ),
 }
 ```
 
+- `TRANSPILER_CACHE_SIZE`: this is the size of an LRU dict used to cache javascript event halder transpilations.
 - `USE_HTML_DIFF`: when enabled uses `difflib` to create diffs to patch the front-end, reducing bandwidth. If disabled it sends the full HTML content every time.
 - `REACTOR_USE_HMIN`: when enabled and django-hmin is installed will use it to minified the HTML of the components and save bandwidth.
-- `RECEIVER_PREFIX`: is the prefix of the event handlers of the components.
-- `TRANSPILER_CACHE_NAME`: which django cache (by name) to use for the event handler transpiler cache. This cache will be accessed with very high frequency so is advisable to use something that works in local memory. By default `LocMemCache(params={"timeout": 3600, "max_entries": 1024, "cull_frequency": 32})` is used if no cache is configured for this name.
 - `AUTO_BROADCAST`: Controls which signals are sent to `Component.mutation` when a model is mutated.
 
-```python
-{
-    # model-a
-    'MODEL': True,
-
-    # model-a.1234
-    'MODEL_PK': True,
-
-    # model-b.9876.model-a-set
-    'RELATED': True,
-
-    # model-b.9876.model-a-set
-    # model-a.1234.model-b-set
-    'M2M': True,
-}
-```
-
 ## Back-end APIs
 
 ### Template tags and filters of `reactor` library
 
 - `{% reactor_header %}`: that includes the necessary JavaScript to make this library work. ~10Kb of minified JS, compressed with gz or brotli.
 - `{% component 'Component' param1=1 param2=2 %}`: Renders a component by its name and passing whatever parameters you put there to the `XComponent.new` method that constructs the component instance.
 - `{% on 'click' 'event_handler' param1=1 param2=2 %}`: Binds an event handler with paramters to some event. Look at [Event binding in the front-end](#event-binding-in-the-front-end)
@@ -244,74 +242,62 @@
 {% component 'Component' param1=1 param2=2 %}
 ```
 
 This passes those parameter there to `Component.new` that should return the component instance and then the component get's rendered in the template and is sent to the client.
 
 ### Joins
 
-When the component arrives to the front-end if it is a root component (has no parent components) it "joins" the backend. Sends it's serialized state to the backend which rebuilds the component and calls `Component.joined`.
+When the component arrives to the front-end it "joins" the backend. Sends it's serialized state to the backend which rebuilds the component and calls `Component.joined`.
 
-After that the component is rendered and the render is sent to the front-end. Why? Because could be that the client was online while some change in the backend happened.
+After that the component is rendered and the render is sent to the front-end. Why? Because could be that the client was online while some change in the backend happened and the component needs to be updated.
 
 ### User events
 
 When a component or its parent has joined it can send user events to the client. Using the `on` template tag, this events are sent to the backend and then the componet is rendered again.
 
 ### Subscriptions
 
 Every time a component joins or responds to an event the `Componet._subscriptions` set is reviewed to check if the component subscribes or not to some channel.
 
-- In case a mutation in a model occurs `Component.mutation(channel: str, instance: Model, action: reactor.auto_broadcast.Action)` will be called.
+- In case a mutation in a model occurs `Component.mutation(channel: str, action: reactor.auto_broadcast.Action, instance: Model)` will be called.
 - In case you broadcast a message using `reactor.component.broadcast(channel, **kwargs)` this message will be sent to any component subscribed to `channel` using the method `Component.notification(channel, **kwargs)`.
 
 ### Disconnection
 
 If the component is destroyed using the `Component.destroy` or just desapears from the front-end it is removed from the backend. If the the websocket closes all components in that connection are removed from the backend and the state of those componets stay just in the front-end in the seralized form awaiting for the front-end to join again.
 
 #### Component API
 
 Each component is a Pydantic model so it can serialize itself. I would advice not to mess with the `__init__` method.
 Instead use the class method `new` to create the instance.
 
 ##### Rendering
 
-- `new`: Class method that responsable for the component initialization, pass what ever you need to bootstrap the component state and read from the database. Should return the component instance.
 - `_extends`: (default: `"div"`) Tag name HTML element the component extends. (Each component is a HTML5 component so it should extend some HTML tag)
 - `_template_name`: Contains the path of the template of the component.
 - `_exclude_fields`: (default: `{"user", "reactor"}`) Which fields to exclude from state serialization during rendering
 - `_url_params`: (default: `{}`) Indicates which local attribute should be persisted in the URL as a GET parameter, being the key a local attribute name and the value the name of the GET parameter that will contain the value of the local attribute.
 
-##### Caching
-
-Component caching:
-
-If you set a cache named `"reactor"`, that cache will be used for components.
-
-- `_cache_key`: (default: `None`) If defined as a string is used as a cache key for rendering.
-- `_cache_time`: (default: `300` seconds) The retention time of the cache.
-- `_cache_touch`: (default: `True`) If enabled everytime the component is rendered the cache is refreshed extending the retention time.
-
-Transpiled event handler:
-
-If you set a cache named `"reactor:transpiler"` that one will be use, [by default `LocMemCache` is used](#settings).
-
 #### Subscriptions
 
 - `_subscriptions`: (default: `set()`) Defines which channels is this component subscribed to.
-- `mutation(channel, instance, action)` Called when autobroadcast is enabled and a model you are subscribed to changes.
+- `mutation(channel, action, instance)` Called when autobroadcast is enabled and a model you are subscribed to changes.
 - `notification(channel, **kwargs)` Called when `reactor.component.broadcast(channel, **kwargs)` is used to send an arbitrary notification to components.
 
 #### Actions
 
 - `destroy()`: Removes the component from the interface.
 - `focus_on(selector: str)`: Makes the front-end look for that `selector` and run `.focus()` on it.
-- `reactor.freeze()`: Prevents the component from being rendered again.
-- `reactor.redirect_to(to, **kwargs)`: Loads a new page and changes the url in the front-end.
+- `skip_render()`: Prevents the component from being rendered once.
+- `send_render()`: Send a signal to request render the component ahead of time.
+- `dom(_action: DomAction, id: str, component_or_template, **kwargs)`: Can append, prepend, insert befor or after certain HTMLElement ID in the dom, the component or template, rendered using the `kwargs`.
+- `freeze()`: Prevents the component from being rendered again.
+- `reactor.redirect_to(to, **kwargs)`: Changes the URL of the front-end and triggers a page load for that new URL
 - `reactor.replace_to(to, **kwargs)`: Changes the current URL for another one.
-- `reactor.push_to(to, **kwargs)`: Like redirect, but instead of loading from the server pushes the content of the page via websocket.
+- `reactor.push_to(to, **kwargs)`: Changs the URL of the front-end adding a new history entry but does not fetch the new URL from the backend.
 - `reactor.send(_channel: str, _topic: str, **kwargs)`: Sends a message over a channel.
 
 ## Front-end APIs
 
 - `reactor.send(element, name, args)`: Sends a reactor user event to `element`, where `name` is the event handler and `args` is a JS object containing the implicit arguments of the call.
 
 ### Event binding in the front-end
@@ -389,15 +375,15 @@
 ```html
 <button {% on 'click 'inc' amount=2 %}>Increment</button>
 ```
 
 You will need an event handler in that component in the back-end:
 
 ```python
-def recv_inc(self, amount: int):
+async def inc(self, amount: int):
     ...
 ```
 
 It is good if you annotate the signature so the types are validated and converted if they have to be.
 
 ## More complex components
```

### Comparing `django-reactor-4.0.2b0/README.md` & `django-reactor-5.0.0b0/README.md`

 * *Files 4% similar despite different names*

```diff
@@ -163,47 +163,45 @@
 ```
 
 ## Settings:
 
 Default settings of reactor are:
 
 ```python
+
+from reactor.schemas import AutoBroadcast
+
 REACTOR = {
+    "TRANSPILER_CACHE_SIZE": 1024,
     "USE_HTML_DIFF": True,
     "USE_HMIN": False,
     "BOOST_PAGES": False,
-    "RECEIVER_PREFIX": "recv_",
     "TRANSPILER_CACHE_NAME": "reactor:transpiler",
-    "AUTO_BROADCAST": False,
+    "AUTO_BROADCAST": AutoBroadcast(
+        # model-a
+        model: bool = False
+        # model-a.1234
+        model_pk: bool = False
+        # model-b.9876.model-a-set
+        related: bool = False
+        # model-b.9876.model-a-set
+        # model-a.1234.model-b-set
+        m2m: bool = False
+        # this is a set of tuples of ('app_label', 'ModelName')
+        # to subscribe for the auto broadcast
+        senders: set[tuple[str, str]] = Field(default_factory=set)
+    ),
 }
 ```
 
+- `TRANSPILER_CACHE_SIZE`: this is the size of an LRU dict used to cache javascript event halder transpilations.
 - `USE_HTML_DIFF`: when enabled uses `difflib` to create diffs to patch the front-end, reducing bandwidth. If disabled it sends the full HTML content every time.
 - `REACTOR_USE_HMIN`: when enabled and django-hmin is installed will use it to minified the HTML of the components and save bandwidth.
-- `RECEIVER_PREFIX`: is the prefix of the event handlers of the components.
-- `TRANSPILER_CACHE_NAME`: which django cache (by name) to use for the event handler transpiler cache. This cache will be accessed with very high frequency so is advisable to use something that works in local memory. By default `LocMemCache(params={"timeout": 3600, "max_entries": 1024, "cull_frequency": 32})` is used if no cache is configured for this name.
 - `AUTO_BROADCAST`: Controls which signals are sent to `Component.mutation` when a model is mutated.
 
-```python
-{
-    # model-a
-    'MODEL': True,
-
-    # model-a.1234
-    'MODEL_PK': True,
-
-    # model-b.9876.model-a-set
-    'RELATED': True,
-
-    # model-b.9876.model-a-set
-    # model-a.1234.model-b-set
-    'M2M': True,
-}
-```
-
 ## Back-end APIs
 
 ### Template tags and filters of `reactor` library
 
 - `{% reactor_header %}`: that includes the necessary JavaScript to make this library work. ~10Kb of minified JS, compressed with gz or brotli.
 - `{% component 'Component' param1=1 param2=2 %}`: Renders a component by its name and passing whatever parameters you put there to the `XComponent.new` method that constructs the component instance.
 - `{% on 'click' 'event_handler' param1=1 param2=2 %}`: Binds an event handler with paramters to some event. Look at [Event binding in the front-end](#event-binding-in-the-front-end)
@@ -220,74 +218,62 @@
 {% component 'Component' param1=1 param2=2 %}
 ```
 
 This passes those parameter there to `Component.new` that should return the component instance and then the component get's rendered in the template and is sent to the client.
 
 ### Joins
 
-When the component arrives to the front-end if it is a root component (has no parent components) it "joins" the backend. Sends it's serialized state to the backend which rebuilds the component and calls `Component.joined`.
+When the component arrives to the front-end it "joins" the backend. Sends it's serialized state to the backend which rebuilds the component and calls `Component.joined`.
 
-After that the component is rendered and the render is sent to the front-end. Why? Because could be that the client was online while some change in the backend happened.
+After that the component is rendered and the render is sent to the front-end. Why? Because could be that the client was online while some change in the backend happened and the component needs to be updated.
 
 ### User events
 
 When a component or its parent has joined it can send user events to the client. Using the `on` template tag, this events are sent to the backend and then the componet is rendered again.
 
 ### Subscriptions
 
 Every time a component joins or responds to an event the `Componet._subscriptions` set is reviewed to check if the component subscribes or not to some channel.
 
-- In case a mutation in a model occurs `Component.mutation(channel: str, instance: Model, action: reactor.auto_broadcast.Action)` will be called.
+- In case a mutation in a model occurs `Component.mutation(channel: str, action: reactor.auto_broadcast.Action, instance: Model)` will be called.
 - In case you broadcast a message using `reactor.component.broadcast(channel, **kwargs)` this message will be sent to any component subscribed to `channel` using the method `Component.notification(channel, **kwargs)`.
 
 ### Disconnection
 
 If the component is destroyed using the `Component.destroy` or just desapears from the front-end it is removed from the backend. If the the websocket closes all components in that connection are removed from the backend and the state of those componets stay just in the front-end in the seralized form awaiting for the front-end to join again.
 
 #### Component API
 
 Each component is a Pydantic model so it can serialize itself. I would advice not to mess with the `__init__` method.
 Instead use the class method `new` to create the instance.
 
 ##### Rendering
 
-- `new`: Class method that responsable for the component initialization, pass what ever you need to bootstrap the component state and read from the database. Should return the component instance.
 - `_extends`: (default: `"div"`) Tag name HTML element the component extends. (Each component is a HTML5 component so it should extend some HTML tag)
 - `_template_name`: Contains the path of the template of the component.
 - `_exclude_fields`: (default: `{"user", "reactor"}`) Which fields to exclude from state serialization during rendering
 - `_url_params`: (default: `{}`) Indicates which local attribute should be persisted in the URL as a GET parameter, being the key a local attribute name and the value the name of the GET parameter that will contain the value of the local attribute.
 
-##### Caching
-
-Component caching:
-
-If you set a cache named `"reactor"`, that cache will be used for components.
-
-- `_cache_key`: (default: `None`) If defined as a string is used as a cache key for rendering.
-- `_cache_time`: (default: `300` seconds) The retention time of the cache.
-- `_cache_touch`: (default: `True`) If enabled everytime the component is rendered the cache is refreshed extending the retention time.
-
-Transpiled event handler:
-
-If you set a cache named `"reactor:transpiler"` that one will be use, [by default `LocMemCache` is used](#settings).
-
 #### Subscriptions
 
 - `_subscriptions`: (default: `set()`) Defines which channels is this component subscribed to.
-- `mutation(channel, instance, action)` Called when autobroadcast is enabled and a model you are subscribed to changes.
+- `mutation(channel, action, instance)` Called when autobroadcast is enabled and a model you are subscribed to changes.
 - `notification(channel, **kwargs)` Called when `reactor.component.broadcast(channel, **kwargs)` is used to send an arbitrary notification to components.
 
 #### Actions
 
 - `destroy()`: Removes the component from the interface.
 - `focus_on(selector: str)`: Makes the front-end look for that `selector` and run `.focus()` on it.
-- `reactor.freeze()`: Prevents the component from being rendered again.
-- `reactor.redirect_to(to, **kwargs)`: Loads a new page and changes the url in the front-end.
+- `skip_render()`: Prevents the component from being rendered once.
+- `send_render()`: Send a signal to request render the component ahead of time.
+- `dom(_action: DomAction, id: str, component_or_template, **kwargs)`: Can append, prepend, insert befor or after certain HTMLElement ID in the dom, the component or template, rendered using the `kwargs`.
+- `freeze()`: Prevents the component from being rendered again.
+- `reactor.redirect_to(to, **kwargs)`: Changes the URL of the front-end and triggers a page load for that new URL
 - `reactor.replace_to(to, **kwargs)`: Changes the current URL for another one.
-- `reactor.push_to(to, **kwargs)`: Like redirect, but instead of loading from the server pushes the content of the page via websocket.
+- `reactor.push_to(to, **kwargs)`: Changs the URL of the front-end adding a new history entry but does not fetch the new URL from the backend.
 - `reactor.send(_channel: str, _topic: str, **kwargs)`: Sends a message over a channel.
 
 ## Front-end APIs
 
 - `reactor.send(element, name, args)`: Sends a reactor user event to `element`, where `name` is the event handler and `args` is a JS object containing the implicit arguments of the call.
 
 ### Event binding in the front-end
@@ -365,15 +351,15 @@
 ```html
 <button {% on 'click 'inc' amount=2 %}>Increment</button>
 ```
 
 You will need an event handler in that component in the back-end:
 
 ```python
-def recv_inc(self, amount: int):
+async def inc(self, amount: int):
     ...
 ```
 
 It is good if you annotate the signature so the types are validated and converted if they have to be.
 
 ## More complex components
```

### Comparing `django-reactor-4.0.2b0/django_reactor.egg-info/PKG-INFO` & `django-reactor-5.0.0b0/django_reactor.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: django-reactor
-Version: 4.0.2b0
+Version: 5.0.0b0
 Summary: Brings LiveView from Phoenix framework into Django
 Home-page: https://github.com/edelvalle/reactor
 Author: Eddy Ernesto del Valle Pino
 Author-email: eddy@edelvalle.me
 License: MIT
 Classifier: Development Status :: 4 - Beta
 Classifier: Environment :: Web Environment
@@ -187,47 +187,45 @@
 ```
 
 ## Settings:
 
 Default settings of reactor are:
 
 ```python
+
+from reactor.schemas import AutoBroadcast
+
 REACTOR = {
+    "TRANSPILER_CACHE_SIZE": 1024,
     "USE_HTML_DIFF": True,
     "USE_HMIN": False,
     "BOOST_PAGES": False,
-    "RECEIVER_PREFIX": "recv_",
     "TRANSPILER_CACHE_NAME": "reactor:transpiler",
-    "AUTO_BROADCAST": False,
+    "AUTO_BROADCAST": AutoBroadcast(
+        # model-a
+        model: bool = False
+        # model-a.1234
+        model_pk: bool = False
+        # model-b.9876.model-a-set
+        related: bool = False
+        # model-b.9876.model-a-set
+        # model-a.1234.model-b-set
+        m2m: bool = False
+        # this is a set of tuples of ('app_label', 'ModelName')
+        # to subscribe for the auto broadcast
+        senders: set[tuple[str, str]] = Field(default_factory=set)
+    ),
 }
 ```
 
+- `TRANSPILER_CACHE_SIZE`: this is the size of an LRU dict used to cache javascript event halder transpilations.
 - `USE_HTML_DIFF`: when enabled uses `difflib` to create diffs to patch the front-end, reducing bandwidth. If disabled it sends the full HTML content every time.
 - `REACTOR_USE_HMIN`: when enabled and django-hmin is installed will use it to minified the HTML of the components and save bandwidth.
-- `RECEIVER_PREFIX`: is the prefix of the event handlers of the components.
-- `TRANSPILER_CACHE_NAME`: which django cache (by name) to use for the event handler transpiler cache. This cache will be accessed with very high frequency so is advisable to use something that works in local memory. By default `LocMemCache(params={"timeout": 3600, "max_entries": 1024, "cull_frequency": 32})` is used if no cache is configured for this name.
 - `AUTO_BROADCAST`: Controls which signals are sent to `Component.mutation` when a model is mutated.
 
-```python
-{
-    # model-a
-    'MODEL': True,
-
-    # model-a.1234
-    'MODEL_PK': True,
-
-    # model-b.9876.model-a-set
-    'RELATED': True,
-
-    # model-b.9876.model-a-set
-    # model-a.1234.model-b-set
-    'M2M': True,
-}
-```
-
 ## Back-end APIs
 
 ### Template tags and filters of `reactor` library
 
 - `{% reactor_header %}`: that includes the necessary JavaScript to make this library work. ~10Kb of minified JS, compressed with gz or brotli.
 - `{% component 'Component' param1=1 param2=2 %}`: Renders a component by its name and passing whatever parameters you put there to the `XComponent.new` method that constructs the component instance.
 - `{% on 'click' 'event_handler' param1=1 param2=2 %}`: Binds an event handler with paramters to some event. Look at [Event binding in the front-end](#event-binding-in-the-front-end)
@@ -244,74 +242,62 @@
 {% component 'Component' param1=1 param2=2 %}
 ```
 
 This passes those parameter there to `Component.new` that should return the component instance and then the component get's rendered in the template and is sent to the client.
 
 ### Joins
 
-When the component arrives to the front-end if it is a root component (has no parent components) it "joins" the backend. Sends it's serialized state to the backend which rebuilds the component and calls `Component.joined`.
+When the component arrives to the front-end it "joins" the backend. Sends it's serialized state to the backend which rebuilds the component and calls `Component.joined`.
 
-After that the component is rendered and the render is sent to the front-end. Why? Because could be that the client was online while some change in the backend happened.
+After that the component is rendered and the render is sent to the front-end. Why? Because could be that the client was online while some change in the backend happened and the component needs to be updated.
 
 ### User events
 
 When a component or its parent has joined it can send user events to the client. Using the `on` template tag, this events are sent to the backend and then the componet is rendered again.
 
 ### Subscriptions
 
 Every time a component joins or responds to an event the `Componet._subscriptions` set is reviewed to check if the component subscribes or not to some channel.
 
-- In case a mutation in a model occurs `Component.mutation(channel: str, instance: Model, action: reactor.auto_broadcast.Action)` will be called.
+- In case a mutation in a model occurs `Component.mutation(channel: str, action: reactor.auto_broadcast.Action, instance: Model)` will be called.
 - In case you broadcast a message using `reactor.component.broadcast(channel, **kwargs)` this message will be sent to any component subscribed to `channel` using the method `Component.notification(channel, **kwargs)`.
 
 ### Disconnection
 
 If the component is destroyed using the `Component.destroy` or just desapears from the front-end it is removed from the backend. If the the websocket closes all components in that connection are removed from the backend and the state of those componets stay just in the front-end in the seralized form awaiting for the front-end to join again.
 
 #### Component API
 
 Each component is a Pydantic model so it can serialize itself. I would advice not to mess with the `__init__` method.
 Instead use the class method `new` to create the instance.
 
 ##### Rendering
 
-- `new`: Class method that responsable for the component initialization, pass what ever you need to bootstrap the component state and read from the database. Should return the component instance.
 - `_extends`: (default: `"div"`) Tag name HTML element the component extends. (Each component is a HTML5 component so it should extend some HTML tag)
 - `_template_name`: Contains the path of the template of the component.
 - `_exclude_fields`: (default: `{"user", "reactor"}`) Which fields to exclude from state serialization during rendering
 - `_url_params`: (default: `{}`) Indicates which local attribute should be persisted in the URL as a GET parameter, being the key a local attribute name and the value the name of the GET parameter that will contain the value of the local attribute.
 
-##### Caching
-
-Component caching:
-
-If you set a cache named `"reactor"`, that cache will be used for components.
-
-- `_cache_key`: (default: `None`) If defined as a string is used as a cache key for rendering.
-- `_cache_time`: (default: `300` seconds) The retention time of the cache.
-- `_cache_touch`: (default: `True`) If enabled everytime the component is rendered the cache is refreshed extending the retention time.
-
-Transpiled event handler:
-
-If you set a cache named `"reactor:transpiler"` that one will be use, [by default `LocMemCache` is used](#settings).
-
 #### Subscriptions
 
 - `_subscriptions`: (default: `set()`) Defines which channels is this component subscribed to.
-- `mutation(channel, instance, action)` Called when autobroadcast is enabled and a model you are subscribed to changes.
+- `mutation(channel, action, instance)` Called when autobroadcast is enabled and a model you are subscribed to changes.
 - `notification(channel, **kwargs)` Called when `reactor.component.broadcast(channel, **kwargs)` is used to send an arbitrary notification to components.
 
 #### Actions
 
 - `destroy()`: Removes the component from the interface.
 - `focus_on(selector: str)`: Makes the front-end look for that `selector` and run `.focus()` on it.
-- `reactor.freeze()`: Prevents the component from being rendered again.
-- `reactor.redirect_to(to, **kwargs)`: Loads a new page and changes the url in the front-end.
+- `skip_render()`: Prevents the component from being rendered once.
+- `send_render()`: Send a signal to request render the component ahead of time.
+- `dom(_action: DomAction, id: str, component_or_template, **kwargs)`: Can append, prepend, insert befor or after certain HTMLElement ID in the dom, the component or template, rendered using the `kwargs`.
+- `freeze()`: Prevents the component from being rendered again.
+- `reactor.redirect_to(to, **kwargs)`: Changes the URL of the front-end and triggers a page load for that new URL
 - `reactor.replace_to(to, **kwargs)`: Changes the current URL for another one.
-- `reactor.push_to(to, **kwargs)`: Like redirect, but instead of loading from the server pushes the content of the page via websocket.
+- `reactor.push_to(to, **kwargs)`: Changs the URL of the front-end adding a new history entry but does not fetch the new URL from the backend.
 - `reactor.send(_channel: str, _topic: str, **kwargs)`: Sends a message over a channel.
 
 ## Front-end APIs
 
 - `reactor.send(element, name, args)`: Sends a reactor user event to `element`, where `name` is the event handler and `args` is a JS object containing the implicit arguments of the call.
 
 ### Event binding in the front-end
@@ -389,15 +375,15 @@
 ```html
 <button {% on 'click 'inc' amount=2 %}>Increment</button>
 ```
 
 You will need an event handler in that component in the back-end:
 
 ```python
-def recv_inc(self, amount: int):
+async def inc(self, amount: int):
     ...
 ```
 
 It is good if you annotate the signature so the types are validated and converted if they have to be.
 
 ## More complex components
```

### Comparing `django-reactor-4.0.2b0/django_reactor.egg-info/SOURCES.txt` & `django-reactor-5.0.0b0/django_reactor.egg-info/SOURCES.txt`

 * *Files 9% similar despite different names*

```diff
@@ -11,17 +11,17 @@
 django_reactor.egg-info/top_level.txt
 reactor/__init__.py
 reactor/apps.py
 reactor/auto_broadcast.py
 reactor/component.py
 reactor/consumer.py
 reactor/event_transpiler.py
-reactor/fields.py
 reactor/log.py
 reactor/repository.py
+reactor/schemas.py
 reactor/serializer.py
 reactor/settings.py
 reactor/urls.py
 reactor/utils.py
 reactor/static/reactor/reactor.min.js
 reactor/templates/reactor_header.html
 reactor/templatetags/__init__.py
```

### Comparing `django-reactor-4.0.2b0/reactor/component.py` & `django-reactor-5.0.0b0/reactor/component.py`

 * *Files 8% similar despite different names*

```diff
@@ -3,27 +3,28 @@
 from asyncio import iscoroutine, iscoroutinefunction
 from functools import reduce
 from uuid import uuid4
 
 from asgiref.sync import async_to_sync
 from channels.db import database_sync_to_async as db
 from channels.layers import BaseChannelLayer
+from django.apps import apps
 from django.contrib.auth.base_user import AbstractBaseUser
 from django.contrib.auth.models import AnonymousUser
 from django.db import models
 from django.http import HttpRequest
 from django.shortcuts import resolve_url  # type: ignore
 from django.template import loader
 from django.utils.html import format_html
 from django.utils.safestring import SafeString, SafeText, mark_safe
 from pydantic import BaseModel, validate_arguments
-from pydantic.fields import Field
+from pydantic.fields import Field, ModelField
 
-from . import serializer, settings, utils
-from .auto_broadcast import Action
+from . import settings, utils
+from .schemas import DomAction, ModelAction
 
 if settings.USE_HMIN:
     try:
         from hmin.base import html_minify  # type: ignore
     except ImportError as e:
         raise ImportError(
             "If you enable REACTOR['USE_HMIN'] you need to install django-hmin"
@@ -33,15 +34,16 @@
     def html_minify(html: str) -> str:
         return html
 
 
 ComponentState = Context = MessagePayload = dict[str, t.Any]
 RedirectDestination = t.Callable[(...), t.Any] | models.Model | str
 HTMLDiff = list[str | int]
-User = AnonymousUser | AbstractBaseUser
+ComponentOrHtml = t.Union["Component", SafeString]
+P = t.ParamSpec("P")
 
 
 class Template(t.Protocol):
     def render(
         self,
         context: Context | dict[str, t.Any] | None = ...,
         request: HttpRequest | None = ...,
@@ -49,14 +51,22 @@
         ...
 
 
 class Repo(t.Protocol):
     pass
 
 
+ScrollPosition = (
+    t.Literal["start"]
+    | t.Literal["end"]
+    | t.Literal["center"]
+    | t.Literal["nearest"]
+)
+
+
 __all__ = ("Component", "broadcast")
 
 
 def broadcast(channel: str, **kwargs: t.Any):
     utils.send_to(channel, type="notification", kwargs=kwargs)
 
 
@@ -68,107 +78,120 @@
         channel_name: str | None = None,
         channel_layer: BaseChannelLayer | None = None,
         parent_id: str | None = None,
     ):
         self.channel_name = channel_name
         self.channel_layer = channel_layer
         self.parent_id = parent_id
-        self._destroyed = False
-        self._is_frozen = False
-        self._redirected_to = None
+        self._is_frozen: bool = False
+        self._redirected_to: str | None = None
+        self._last_sent_html: list[str] = []
+        self._skip_render: bool = False
+
+    def clone(self):
+        return type(self)(
+            channel_name=self.channel_name,
+            channel_layer=self.channel_layer,
+        )
+
+    def skip_render(self):
+        self._skip_render = True
+
+    def force_render(self):
+        self._skip_render = False
         self._last_sent_html = []
 
     async def destroy(self, component_id: str):
-        if not self._destroyed:
-            self._destroyed = True
-            await self.send("remove", id=component_id)
+        self.freeze()
+        await self.send("remove", id=component_id)
 
     def freeze(self):
         self._is_frozen = True
 
-    async def redirect_to(self, to: t.Any, **kwargs: t.Any):
-        await self._redirect(to, kwargs)
-
-    async def replace_to(self, to: RedirectDestination, **kwargs: t.Any):
-        await self._redirect(to, kwargs, replace=True)
-
-    async def push_to(self, to: RedirectDestination, **kwargs: t.Any):
-        await self._push(to, kwargs)
-
-    async def send_render(self, component_id: str):
-        await self.send("render", id=component_id)
-
-    async def _redirect(
-        self,
-        to: RedirectDestination,
-        kwargs: t.Any,
-        replace: bool = False,
-    ):
+    async def redirect_to(self, to: RedirectDestination, **kwargs: t.Any):
         url = resolve_url(to, **kwargs)
         self._redirected_to = url
         if self.channel_name:
             self.freeze()
-            await self.send("redirect_to", url=url, replace=replace)
+            await self.send("url_change", command="redirect", url=url)
 
-    async def _push(self, to: RedirectDestination, kwargs: Context):
+    async def replace_to(self, to: RedirectDestination, **kwargs):
         url = resolve_url(to, **kwargs)
-        self._redirected_to = url
-        if self.channel_name:
-            self.freeze()
-            await self.send("push_page", url=url)
+        await self.send("url_change", command="replace", url=url)
+
+    async def push_to(self, to: RedirectDestination, **kwargs):
+        url = resolve_url(to, **kwargs)
+        await self.send("url_change", command="push", url=url)
 
     async def render_diff(
         self, component: "Component", repo: Repo
     ) -> HTMLDiff | None:
-        html = await db(self.render)(component, repo)
-        if html and self._last_sent_html != (html := html.split(" ")):
-            if settings.USE_HTML_DIFF:
-                diff: HTMLDiff = []
-                for x in difflib.ndiff(self._last_sent_html, html):
-                    indicator = x[0]
-                    if indicator == " ":
-                        diff.append(1)
-                    elif indicator == "+":
-                        diff.append(x[2:])
-                    elif indicator == "-":
-                        diff.append(-1)
-
-                if diff:
-                    diff = reduce(compress_diff, diff[1:], diff[:1])
-            else:
-                diff = html  # type: ignore
-            self._last_sent_html = html
-            return diff
+        if self._skip_render:
+            self._skip_render = False
+        else:
+            html = await db(self.render)(component, repo)
+            if html and self._last_sent_html != (html := html.split(" ")):
+                if settings.USE_HTML_DIFF:
+                    diff: HTMLDiff = []
+                    for x in difflib.ndiff(self._last_sent_html, html):
+                        indicator = x[0]
+                        if indicator == " ":
+                            diff.append(1)
+                        elif indicator == "+":
+                            diff.append(x[2:])
+                        elif indicator == "-":
+                            diff.append(-1)
+
+                    if diff:
+                        diff = reduce(compress_diff, diff[1:], diff[:1])
+                else:
+                    diff = html  # type: ignore
+                self._last_sent_html = html
+                return diff
 
     def render(self, component: "Component", repo: Repo) -> None | SafeText:
         html = None
         if not self.channel_name and self._redirected_to:
             html = format_html(
                 '<meta http-equiv="refresh" content="0; url={url}">',
                 url=self._redirected_to,
             )
-        elif not (self._is_frozen or self._redirected_to):
-            key = component._cache_key
-            key = key and f"{component._fqn}:{key}"
-
-            if key is not None:
-                html = settings.cache.get(key)
-
-            if html is None:
-                template = component._get_template()
-                context = self._get_context(component, repo)
-                html = template.render(context).strip()
-                html = html_minify(html)
-
-            if key and component._cache_touch:
-                settings.cache.set(key, html, component._cache_time)
-
+        elif not (self._is_frozen or self._redirected_to) and html is None:
+            template = component._get_template()
+            context = self._get_context(component, repo)
+            html = template.render(context).strip()
+            html = html_minify(html)
         if html:
             return mark_safe(html)
 
+    async def send_dom_action(
+        self,
+        action: DomAction,
+        id: str,
+        html: SafeString,
+    ):
+        await self.send("dom_action", action=action.value, id=id, html=html)
+
+    async def scroll_into_view(
+        self,
+        id: str,
+        behavoir: t.Literal["smooth"]
+        | t.Literal["instant"]
+        | t.Literal["auto"] = "auto",
+        block: ScrollPosition = "start",
+        inline: ScrollPosition = "nearest",
+    ):
+        await self.send(
+            "scroll_into_view",
+            id=id,
+            behavoir=behavoir,
+            block=block,
+            inline=inline,
+        )
+
     async def send(self, _command: str, **kwargs: t.Any):
         if self.channel_name:
             await self.send_to(self.channel_name, _command, **kwargs)
 
     async def send_to(self, _channel: str, _command: str, **kwargs: t.Any):
         if self.channel_layer:
             await self.channel_layer.send(
@@ -184,22 +207,20 @@
         self,
         component: "Component",
         repo: Repo,
     ) -> Context:
         context = {}
 
         for attr_name in dir(component):
-            if not attr_name.startswith("_") or not attr_name.startswith(
-                settings.RECEIVER_PREFIX
-            ):
+            if not attr_name.startswith("_"):
                 attr = getattr(component, attr_name)
-                if iscoroutine(attr) or iscoroutinefunction(attr):
-                    attr = async_to_sync(attr)
-                context[attr_name] = attr
-
+                if not callable(attr):
+                    if iscoroutine(attr) or iscoroutinefunction(attr):
+                        attr = async_to_sync(attr)
+                    context[attr_name] = attr
         return dict(
             context,
             this=component,
             reactor_repository=repo,
         )
 
 
@@ -211,54 +232,67 @@
         if same_sign:
             diff[-1] += diff_item
         else:
             diff.append(diff_item)
     return diff
 
 
+def load_model_instance(model, v, fields, field: ModelField, config):
+    if v is None or isinstance(v, field.type_):
+        return v
+    else:
+        return field.type_.objects.filter(pk=v).first()
+
+
+def load_queryset(model, v, fields, field: ModelField, config):
+    if isinstance(v, field.type_):
+        return v
+    else:
+        return apps.get_model(v["app"], v["model"]).objects.filter(  # type: ignore
+            pk__in=v["ids"]
+        )
+
+
 class Component(BaseModel):
     __name__: str
 
     _all: dict[str, t.Type["Component"]] = {}
     _urls = {}
     _name: str = ...  # type: ignore
     _template_name: str = ...  # type: ignore
-    _template_engine: Template
+    _templates: dict[str, Template] = {}
     _fqn: str
     _tag_name: str
     _url_params: t.Mapping[str, str] = {}  # local_attr_name -> url_param_name
 
     # HTML tag that this component extends
     _extends = "div"
 
     # fields to exclude from the component state during serialization
     _exclude_fields = {"user", "reactor"}
 
-    # Cache: the render of the component can be cached if you define a cache key
-    _cache_key: str | None = None
-    # expiration time of the cache
-    _cache_time = 300
-    # if True will refresh the cache on each render
-    _cache_touch = True
-
     # Subscriptions: you can define here which channels this component is
     # subscribed to
     _subscriptions: set[str] = set()
 
     class Config:
         arbitrary_types_allowed = True
         validate_assignment = True
-        json_encoders = {  # type: ignore
-            models.Model: lambda x: serializer.encode(x),  # type: ignore
-            models.QuerySet: lambda qs: [x.pk for x in qs],  # type: ignore
+        json_encoders = {
+            models.Model: lambda x: x.pk,
+            models.QuerySet: lambda qs: {
+                "app": qs.model._meta.app_label,
+                "model": qs.model._meta.model_name,
+                "ids": [x.pk for x in qs],
+            },
         }
 
     def __init_subclass__(
         cls: t.Type["Component"], name: str | None = None, public: bool = True
-    ) -> t.Type["Component"]:
+    ):
         if public:
             name = name or cls.__name__
             cls._all[name] = cls
             # Component name
             cls._name = name
             # Fully qualified name
             cls._fqn = f"{cls.__module__}.{name}"
@@ -269,128 +303,146 @@
             cls._tag_name = "x-" + name
 
         for attr_name in vars(cls):
             attr = getattr(cls, attr_name)
             if (
                 not attr_name.startswith("_")
                 and attr_name.islower()
-                and attr_name.startswith(settings.RECEIVER_PREFIX)
                 and callable(attr)
             ):
                 setattr(
                     cls,
                     attr_name,
                     validate_arguments(
                         config={"arbitrary_types_allowed": True}
                     )(attr),
                 )
 
-        return super().__init_subclass__()  # type: ignore
+        # Hook up the Model loaders
+        for field in cls.__fields__.values():
+            if field.pre_validators is None:
+                try:
+                    is_model = issubclass(field.type_, models.Model)
+                    is_qs = issubclass(field.type_, models.QuerySet)  # type: ignore
+                except TypeError:
+                    is_model = False
+                    is_qs = False
+
+                if is_model:
+                    field.pre_validators = [load_model_instance]
+                elif is_qs:
+                    field.pre_validators = [load_queryset]
+
+        super().__init_subclass__()
 
     @classmethod
-    def _new(
+    def _build(
         cls,
         _component_name: str,
         state: ComponentState,
-        user: User,
+        user: AnonymousUser | AbstractBaseUser | None = None,
         channel_name: str | None = None,
         channel_layer: BaseChannelLayer | None = None,
         parent_id: str | None = None,
     ) -> "Component":
         if _component_name not in cls._all:
             raise ComponentNotFound(
-                f"Could not find requested component '{_component_name}'. "
-                f"Did you load the component?"
+                (
+                    f"Could not find requested component '{_component_name}'. "
+                    f"Did you load the component?"
+                )
             )
 
         # TODO: rename state to initial_state
         instance = cls._all[_component_name].new(
-            reactor=ReactorMeta(
-                channel_name=channel_name,
-                channel_layer=channel_layer,
-                parent_id=parent_id,
-            ),
-            user=user,
-            **state,
-        )
-        return instance
-
-    @classmethod
-    async def _rebuild(
-        cls,
-        _component_name: str,
-        state: ComponentState,
-        user: User,
-        channel_name: str | None = None,
-        parent_id: str | None = None,
-    ):
-        if _component_name not in cls._all:
-            raise ComponentNotFound(
-                f"Could not find requested component '{_component_name}'. "
-                f"Did you load the component?"
-            )
-
-        # TODO: rename state to initial_state
-        instance = cls._all[_component_name](
             user=user or AnonymousUser(),
             reactor=ReactorMeta(
                 channel_name=channel_name,
+                channel_layer=channel_layer,
                 parent_id=parent_id,
             ),
             **state,
         )
-        await instance.joined()
         return instance
 
     @classmethod
-    def _get_template(cls) -> Template:
+    def _get_template(cls, template_name: str | None = None) -> Template:
+        template_name = template_name or cls._template_name
         if settings.DEBUG:
-            return cls._load_template()
+            return loader.get_template(template_name)
         else:
-            if (template := getattr(cls, "_template_engine", None)) is None:
-                template = cls._load_template()
-                setattr(cls, "_template_engine", template)
+            if (template := cls._templates.get(template_name)) is None:
+                template = loader.get_template(template_name)
+                cls._templates[template_name] = template
             return template
 
-    @classmethod
-    def _load_template(cls) -> Template:
-        if isinstance(cls._template_name, (list, tuple)):
-            return loader.select_template(cls._template_name)
-        else:
-            return loader.get_template(cls._template_name)
-
     # State
     id: str = Field(default_factory=lambda: f"rx-{uuid4()}")
-    user: User
+    user: AnonymousUser | AbstractBaseUser
     reactor: ReactorMeta
 
     @classmethod
     def new(cls, **kwargs: t.Any):
         return cls(**kwargs)
 
     async def joined(self):
         ...
 
-    async def mutation(self, channel: str, instance: t.Any, action: Action.T):
+    async def mutation(
+        self, channel: str, action: ModelAction, instance: t.Any
+    ):
         ...
 
     async def notification(self, channel: str, **kwargs: t.Any):
         ...
 
     async def destroy(self):
         await self.reactor.destroy(self.id)
 
     async def send_render(self):
-        await self.reactor.send_render(self.id)
+        await self.reactor.send("send_render", id=self.id)
+
+    async def focus_on(self, selector: str):
+        await self.reactor.send("focus_on", selector=selector)
+
+    # Dom operations
+
+    def skip_render(self):
+        self.reactor.skip_render()
+
+    def force_render(self):
+        self.reactor.force_render()
+
+    async def dom(
+        self,
+        _action: DomAction,
+        _id: str,
+        _component_class_or_template_name: t.Type["Component"] | str,
+        **kwargs,
+    ):
+        if isinstance(_component_class_or_template_name, str):
+            template = self._get_template(_component_class_or_template_name)
+            html = await db(template.render)(kwargs)
+        else:
+            from .repository import ComponentRepository
+
+            component = _component_class_or_template_name.new(
+                reactor=self.reactor.clone(),
+                user=self.user,
+                **kwargs,
+            )
+            html = await db(component._render)(
+                ComponentRepository(user=self.user)
+            )
+        await self.reactor.send_dom_action(_action, _id, html)
+
+    # Internal render operations
 
-    def render(self, repo: Repo):
+    def _render(self, repo: Repo):
         return self.reactor.render(self, repo)
 
-    def render_diff(self, repo: Repo):
+    def _render_diff(self, repo: Repo):
         return self.reactor.render_diff(self, repo)
 
-    async def focus_on(self, selector: str):
-        await self.reactor.send("focus_on", selector=selector)
-
 
 class ComponentNotFound(LookupError):
     pass
```

### Comparing `django-reactor-4.0.2b0/reactor/consumer.py` & `django-reactor-5.0.0b0/reactor/consumer.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,19 +1,15 @@
 import json
 import logging
 import typing as t
 
-from channels.db import database_sync_to_async as db
 from channels.generic.websocket import AsyncJsonWebsocketConsumer
 from django.contrib.auth.models import AnonymousUser
 from django.core.signing import Signer
-from django.http.response import HttpResponse
-from django.test import Client
 from django.utils.datastructures import MultiValueDict
-
 from reactor.component import Component
 
 from . import serializer
 from .repository import ComponentRepository
 from .utils import parse_request_data
 
 log = logging.getLogger("reactor")
@@ -36,20 +32,34 @@
     # Fronted commands
 
     async def receive_json(self, content):
         await getattr(self, f'command_{content["command"]}')(
             **content["payload"]
         )
 
-    async def command_join(self, name, state):
-        state = json.loads(Signer().unsign(state))
-        log.debug(f"<<< JOIN {name} {state}")
-        component = await self.repo.join(name, state)
-        await self.send_render(component)
-        await self.update_to_which_channels_im_subscribed_to()
+    async def command_join(
+        self,
+        name: str,
+        state: str,
+        parent_id: str | None = None,
+    ):
+        decoded_state: dict[str, t.Any] = json.loads(Signer().unsign(state))
+        log.debug(f"<<< JOIN {name} {decoded_state}")
+        try:
+            component, created = await self.repo.join(
+                name, decoded_state, parent_id=parent_id
+            )
+        except Exception as e:
+            log.exception(e)
+            if id := decoded_state.get("id"):
+                await self.component_remove(id)
+        else:
+            if created:
+                await self.send_render(component)
+            await self.update_to_which_channels_im_subscribed_to()
 
     async def command_leave(self, id):
         log.debug(f"<<< LEAVE {id}")
         self.repo.remove(id)
 
     async def command_user_event(
         self, id, command, implicit_args, explicit_args
@@ -72,48 +82,32 @@
         await self.send_command("remove", {"id": id})
 
     async def component_send_render(self, id):
         log.debug(f">>> SEND-RENDER {id}")
         if component := self.repo.get(id):
             await self.send_render(component)
 
+    async def component_dom_action(self, action, id, html):
+        log.debug(f">>> DOM {action.upper()} {id}")
+        await self.send_command(action, {"id": id, "html": html})
+
+    async def component_scroll_into_view(self, id, behavoir, block, inline):
+        log.debug(f">>> SCROLL-INTO-VIEW {id}")
+        await self.send_command(
+            "scroll_into_view",
+            {"id": id, "behavoir": behavoir, "block": block, "inline": inline},
+        )
+
     async def component_focus_on(self, selector):
         log.debug(f'>>> FOCUS ON "{selector}"')
         await self.send_command("focus_on", {"selector": selector})
 
-    async def component_redirect_to(self, url: str, replace: bool = False):
-        action = "REPLACE WITH" if replace else "REDIRECT TO"
-        log.debug(f'>>> {action} "{url}"')
-        await self.send_command("visit", {"url": url, "replace": replace})
-
-    async def component_push_page(self, url: str):
-        try:
-            log.debug(f'>>> PUSH PAGE "{url}"')
-            client = Client()
-            if not isinstance(self.user, AnonymousUser):
-                await db(client.force_login)(self.user)
-            response: HttpResponse = await db(client.get)(
-                url,
-                follow=True,
-            )
-            redirects: list[tuple(str, int)] = response.redirect_chain  # type: ignore
-            if redirects:
-                page_url, _status = redirects[-1]
-            else:
-                page_url = url
-            await self.send_command(
-                "page",
-                {
-                    "url": page_url,
-                    "content": response.content.decode().strip(),
-                },
-            )
-        except Exception as e:
-            log.debug(f'>>> PUSH FAILED "{e}"')
-            await self.component_redirect_to(url)
+    async def component_url_change(self, command: str, url: str):
+        log.debug(f'>>> URL {command.upper()} "{url}"')
+        await self.send_command("url_change", {"url": url, "command": command})
 
     # Incoming messages from subscriptions
 
     async def model_mutation(self, data):
         # The signature here is coupled to:
         #   `reactor.auto_broadcast.notify_mutation`
         await self._dispatch_notifications(
@@ -139,15 +133,15 @@
             await getattr(component, receiver)(channel, **kwargs)
             await self.send_render(component)
         await self.update_to_which_channels_im_subscribed_to()
 
     # Reply to front-end
 
     async def send_render(self, component: Component):
-        diff = await component.render_diff(self.repo)
+        diff = await component._render_diff(self.repo)
         if diff is not None:
             log.debug(f">>> RENDER {component._name} {component.id}")
             await self.send_command(
                 "render",
                 {"id": component.id, "diff": diff},
             )
             if url_params := {
```

### Comparing `django-reactor-4.0.2b0/reactor/event_transpiler.py` & `django-reactor-5.0.0b0/reactor/event_transpiler.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,22 +1,25 @@
 import json
 import typing as t
 
 from django.core.serializers.json import DjangoJSONEncoder
+from lru import LRU
 
-from . import settings
+from .settings import TRANSPILER_CACHE_SIZE
 
 Stack = list[t.Any]
 
+CACHE: dict[str, str | None] = LRU(TRANSPILER_CACHE_SIZE)
+
 
 def transpile(event_and_modifiers: str, command: str, kwargs: dict[str, t.Any]):
     """Translates from from the tag `on` in to JavaScript"""
     name, *modifiers = event_and_modifiers.split(".")
     cache_key = f"_handler:{modifiers}.{command}.{kwargs}"
-    code: t.Optional[str] = settings.transpiler_cache.get(cache_key)
+    code: t.Optional[str] = CACHE.get(cache_key)
     if code is None:
         if not modifiers or modifiers[-1] != "inlinejs":
             modifiers.append("_reactor_code")
         code = command
         stack: Stack = [kwargs]
         while modifiers:
             modifier = modifiers.pop()
@@ -24,15 +27,15 @@
                 Modifiers, modifier, None
             )
             if handler:
                 code = handler(code, stack)
             else:
                 stack.append(modifier)
 
-        settings.transpiler_cache.set(cache_key, code)
+        CACHE[cache_key] = code
     return "on" + name, code
 
 
 class Modifiers:
     @staticmethod
     def _reactor_code(code: str, stack: Stack):
         kwargs = json.dumps(stack.pop(), cls=DjangoJSONEncoder)
```

### Comparing `django-reactor-4.0.2b0/reactor/repository.py` & `django-reactor-5.0.0b0/reactor/repository.py`

 * *Files 27% similar despite different names*

```diff
@@ -1,68 +1,77 @@
 from functools import reduce
 
+from channels.db import database_sync_to_async as db
 from channels.layers import BaseChannelLayer
 from django.contrib.auth.models import AbstractBaseUser, AnonymousUser
 
-from . import settings
 from .component import Component, MessagePayload
 from .utils import filter_parameters
 
 
 class ComponentRepository:
     user: AnonymousUser | AbstractBaseUser
 
     def __init__(
         self,
-        user: AbstractBaseUser | None = None,
+        user: AnonymousUser | AbstractBaseUser | None = None,
         channel_name: str | None = None,
         channel_layer: BaseChannelLayer | None = None,
     ):
         self.channel_name = channel_name
         self.channel_layer = channel_layer
         self.user = user or AnonymousUser()
         self.components: dict[str, Component] = {}
 
     def get(self, component_id: str) -> Component | None:
         return self.components.get(component_id)
 
-    def new(
+    def build(
         self, name: str, state: MessagePayload, parent_id: str | None = None
-    ) -> Component:
-        component = Component._new(
-            name,
-            state,
-            user=self.user,
-            channel_name=self.channel_name,
-            channel_layer=self.channel_layer,
-            parent_id=parent_id,
-        )
-        return self._register_component(component)
+    ) -> tuple[Component, bool]:
+        if (component_id := state.get("id")) and (
+            component := self.components.get(component_id)
+        ):
+            # override with the passed state but preserve the rest of the state
+            for key, value in state.items():
+                setattr(component, key, value)
+            component.reactor.parent_id = parent_id
+            return component, False
+        else:
+            component = Component._build(
+                name,
+                state,
+                user=self.user,
+                channel_name=self.channel_name,
+                channel_layer=self.channel_layer,
+                parent_id=parent_id,
+            )
+            return self.register_component(component), True
 
-    async def join(self, name, state, parent_id=None) -> Component:
-        component = await Component._rebuild(
-            name,
-            state,
-            user=self.user,
-            channel_name=self.channel_name,
-            parent_id=parent_id,
+    async def join(
+        self, name: str, state: MessagePayload, parent_id: str | None = None
+    ) -> tuple[Component, bool]:
+        component, created = await db(self.build)(
+            name, state, parent_id=parent_id
         )
-        return self._register_component(component)
+        if created:
+            await component.joined()
+        return component, created
 
-    def _register_component(self, component):
+    def register_component(self, component: Component):
         self.components[component.id] = component
         return component
 
     def remove(self, id):
         self.components.pop(id, None)
 
     async def dispatch_event(self, id, command, kwargs):
         assert not command.startswith("_")
         component = self.components[id]
-        handler = getattr(component, settings.RECEIVER_PREFIX + command)
+        handler = getattr(component, command)
         await handler(**filter_parameters(handler, kwargs))
         return component
 
     def components_subscribed_to(self, channel):
         # XXX: There is a list() here because the dict can change size during
         # iteration
         for component in list(self.components.values()):
```

### Comparing `django-reactor-4.0.2b0/reactor/static/reactor/reactor.min.js` & `django-reactor-5.0.0b0/reactor/static/reactor/reactor.min.js`

 * *Files 8% similar despite different names*

#### js-beautify {}

```diff
@@ -1,378 +1,384 @@
 (() => {
-    var _e = Object.defineProperty;
-    var me = (t, e, n) => e in t ? _e(t, e, {
+    var ye = Object.defineProperty;
+    var we = (t, e, n) => e in t ? ye(t, e, {
         enumerable: !0,
         configurable: !0,
         writable: !0,
         value: n
     }) : t[e] = n;
-    var H = (t, e, n) => (me(t, typeof e != "symbol" ? e + "" : e, n), n);
-    var re = 11;
+    var H = (t, e, n) => (we(t, typeof e != "symbol" ? e + "" : e, n), n);
+    var oe = 11;
 
-    function ge(t, e) {
+    function Ee(t, e) {
         var n = e.attributes,
-            i, r, o, s, u;
-        if (!(e.nodeType === re || t.nodeType === re)) {
-            for (var d = n.length - 1; d >= 0; d--) i = n[d], r = i.name, o = i.namespaceURI, s = i.value, o ? (r = i.localName || r, u = t.getAttributeNS(o, r), u !== s && (i.prefix === "xmlns" && (r = i.name), t.setAttributeNS(o, r, s))) : (u = t.getAttribute(r), u !== s && t.setAttribute(r, s));
-            for (var _ = t.attributes, b = _.length - 1; b >= 0; b--) i = _[b], r = i.name, o = i.namespaceURI, o ? (r = i.localName || r, e.hasAttributeNS(o, r) || t.removeAttributeNS(o, r)) : e.hasAttribute(r) || t.removeAttribute(r)
+            i, r, o, a, u;
+        if (!(e.nodeType === oe || t.nodeType === oe)) {
+            for (var d = n.length - 1; d >= 0; d--) i = n[d], r = i.name, o = i.namespaceURI, a = i.value, o ? (r = i.localName || r, u = t.getAttributeNS(o, r), u !== a && (i.prefix === "xmlns" && (r = i.name), t.setAttributeNS(o, r, a))) : (u = t.getAttribute(r), u !== a && t.setAttribute(r, a));
+            for (var m = t.attributes, L = m.length - 1; L >= 0; L--) i = m[L], r = i.name, o = i.namespaceURI, o ? (r = i.localName || r, e.hasAttributeNS(o, r) || t.removeAttributeNS(o, r)) : e.hasAttribute(r) || t.removeAttribute(r)
         }
     }
-    var q, ye = "http://www.w3.org/1999/xhtml",
-        p = typeof document == "undefined" ? void 0 : document,
-        be = !!p && "content" in p.createElement("template"),
-        we = !!p && p.createRange && "createContextualFragment" in p.createRange();
+    var W, Te = "http://www.w3.org/1999/xhtml",
+        _ = typeof document == "undefined" ? void 0 : document,
+        Se = !!_ && "content" in _.createElement("template"),
+        Oe = !!_ && _.createRange && "createContextualFragment" in _.createRange();
 
-    function Ee(t) {
-        var e = p.createElement("template");
+    function Ce(t) {
+        var e = _.createElement("template");
         return e.innerHTML = t, e.content.childNodes[0]
     }
 
-    function Te(t) {
-        q || (q = p.createRange(), q.selectNode(p.body));
-        var e = q.createContextualFragment(t);
+    function Le(t) {
+        W || (W = _.createRange(), W.selectNode(_.body));
+        var e = W.createContextualFragment(t);
         return e.childNodes[0]
     }
 
-    function Se(t) {
-        var e = p.createElement("body");
+    function Ae(t) {
+        var e = _.createElement("body");
         return e.innerHTML = t, e.childNodes[0]
     }
 
-    function Oe(t) {
-        return t = t.trim(), be ? Ee(t) : we ? Te(t) : Se(t)
+    function Ne(t) {
+        return t = t.trim(), Se ? Ce(t) : Oe ? Le(t) : Ae(t)
     }
 
     function V(t, e) {
         var n = t.nodeName,
             i = e.nodeName,
             r, o;
         return n === i ? !0 : (r = n.charCodeAt(0), o = i.charCodeAt(0), r <= 90 && o >= 97 ? n === i.toUpperCase() : o <= 90 && r >= 97 ? i === n.toUpperCase() : !1)
     }
 
-    function Ce(t, e) {
-        return !e || e === ye ? p.createElement(t) : p.createElementNS(e, t)
+    function ke(t, e) {
+        return !e || e === Te ? _.createElement(t) : _.createElementNS(e, t)
     }
 
-    function Le(t, e) {
+    function Re(t, e) {
         for (var n = t.firstChild; n;) {
             var i = n.nextSibling;
             e.appendChild(n), n = i
         }
         return e
     }
 
-    function Q(t, e, n) {
+    function Y(t, e, n) {
         t[n] !== e[n] && (t[n] = e[n], t[n] ? t.setAttribute(n, "") : t.removeAttribute(n))
     }
-    var ie = {
+    var ae = {
             OPTION: function(t, e) {
                 var n = t.parentNode;
                 if (n) {
                     var i = n.nodeName.toUpperCase();
                     i === "OPTGROUP" && (n = n.parentNode, i = n && n.nodeName.toUpperCase()), i === "SELECT" && !n.hasAttribute("multiple") && (t.hasAttribute("selected") && !e.selected && (t.setAttribute("selected", "selected"), t.removeAttribute("selected")), n.selectedIndex = -1)
                 }
-                Q(t, e, "selected")
+                Y(t, e, "selected")
             },
             INPUT: function(t, e) {
-                Q(t, e, "checked"), Q(t, e, "disabled"), t.value !== e.value && (t.value = e.value), e.hasAttribute("value") || t.removeAttribute("value")
+                Y(t, e, "checked"), Y(t, e, "disabled"), t.value !== e.value && (t.value = e.value), e.hasAttribute("value") || t.removeAttribute("value")
             },
             TEXTAREA: function(t, e) {
                 var n = e.value;
                 t.value !== n && (t.value = n);
                 var i = t.firstChild;
                 if (i) {
                     var r = i.nodeValue;
                     if (r == n || !n && r == t.placeholder) return;
                     i.nodeValue = n
                 }
             },
             SELECT: function(t, e) {
                 if (!e.hasAttribute("multiple")) {
-                    for (var n = -1, i = 0, r = t.firstChild, o, s; r;)
-                        if (s = r.nodeName && r.nodeName.toUpperCase(), s === "OPTGROUP") o = r, r = o.firstChild;
+                    for (var n = -1, i = 0, r = t.firstChild, o, a; r;)
+                        if (a = r.nodeName && r.nodeName.toUpperCase(), a === "OPTGROUP") o = r, r = o.firstChild;
                         else {
-                            if (s === "OPTION") {
+                            if (a === "OPTION") {
                                 if (r.hasAttribute("selected")) {
                                     n = i;
                                     break
                                 }
                                 i++
                             }
                             r = r.nextSibling, !r && o && (r = o.nextSibling, o = null)
                         } t.selectedIndex = n
                 }
             }
         },
-        x = 1,
-        Ne = 11,
-        oe = 3,
-        se = 8;
+        U = 1,
+        se = 11,
+        ce = 3,
+        le = 8;
 
-    function N() {}
+    function S() {}
 
-    function Ae(t) {
+    function xe(t) {
         if (t) return t.getAttribute && t.getAttribute("id") || t.id
     }
 
-    function Re(t) {
+    function Pe(t) {
         return function(n, i, r) {
             if (r || (r = {}), typeof i == "string")
                 if (n.nodeName === "#document" || n.nodeName === "HTML" || n.nodeName === "BODY") {
                     var o = i;
-                    i = p.createElement("html"), i.innerHTML = o
-                } else i = Oe(i);
-            var s = r.getNodeKey || Ae,
-                u = r.onBeforeNodeAdded || N,
-                d = r.onNodeAdded || N,
-                _ = r.onBeforeElUpdated || N,
-                b = r.onElUpdated || N,
-                D = r.onBeforeNodeDiscarded || N,
-                C = r.onNodeDiscarded || N,
-                U = r.onBeforeElChildrenUpdated || N,
-                m = r.childrenOnly === !0,
-                g = Object.create(null),
+                    i = _.createElement("html"), i.innerHTML = o
+                } else i = Ne(i);
+            else i.nodeType === se && (i = i.firstElementChild);
+            var a = r.getNodeKey || xe,
+                u = r.onBeforeNodeAdded || S,
+                d = r.onNodeAdded || S,
+                m = r.onBeforeElUpdated || S,
+                L = r.onElUpdated || S,
+                $ = r.onBeforeNodeDiscarded || S,
+                g = r.onNodeDiscarded || S,
+                M = r.onBeforeElChildrenUpdated || S,
+                j = r.skipFromChildren || S,
+                P = r.addChild || function(c, s) {
+                    return c.appendChild(s)
+                },
+                k = r.childrenOnly === !0,
+                v = Object.create(null),
                 y = [];
 
-            function L(l) {
-                y.push(l)
+            function b(c) {
+                y.push(c)
             }
 
-            function Z(l, c) {
-                if (l.nodeType === x)
-                    for (var a = l.firstChild; a;) {
-                        var f = void 0;
-                        c && (f = s(a)) ? L(f) : (C(a), a.firstChild && Z(a, c)), a = a.nextSibling
+            function D(c, s) {
+                if (c.nodeType === U)
+                    for (var h = c.firstChild; h;) {
+                        var l = void 0;
+                        s && (l = a(h)) ? b(l) : (g(h), h.firstChild && D(h, s)), h = h.nextSibling
                     }
             }
 
-            function M(l, c, a) {
-                D(l) !== !1 && (c && c.removeChild(l), C(l), Z(l, a))
+            function I(c, s, h) {
+                $(c) !== !1 && (s && s.removeChild(c), g(c), D(c, h))
             }
 
-            function ee(l) {
-                if (l.nodeType === x || l.nodeType === Ne)
-                    for (var c = l.firstChild; c;) {
-                        var a = s(c);
-                        a && (g[a] = c), ee(c), c = c.nextSibling
+            function ne(c) {
+                if (c.nodeType === U || c.nodeType === se)
+                    for (var s = c.firstChild; s;) {
+                        var h = a(s);
+                        h && (v[h] = s), ne(s), s = s.nextSibling
                     }
             }
-            ee(n);
+            ne(n);
 
-            function F(l) {
-                d(l);
-                for (var c = l.firstChild; c;) {
-                    var a = c.nextSibling,
-                        f = s(c);
-                    if (f) {
-                        var v = g[f];
-                        v && V(c, v) ? (c.parentNode.replaceChild(v, c), j(v, c)) : F(c)
-                    } else F(c);
-                    c = a
+            function Q(c) {
+                d(c);
+                for (var s = c.firstChild; s;) {
+                    var h = s.nextSibling,
+                        l = a(s);
+                    if (l) {
+                        var f = v[l];
+                        f && V(s, f) ? (s.parentNode.replaceChild(f, s), B(f, s)) : Q(s)
+                    } else Q(s);
+                    s = h
                 }
             }
 
-            function he(l, c, a) {
-                for (; c;) {
-                    var f = c.nextSibling;
-                    (a = s(c)) ? L(a): M(c, l, !0), c = f
+            function me(c, s, h) {
+                for (; s;) {
+                    var l = s.nextSibling;
+                    (h = a(s)) ? b(h): I(s, c, !0), s = l
                 }
             }
 
-            function j(l, c, a) {
-                var f = s(c);
-                f && delete g[f], !(!a && (_(l, c) === !1 || (t(l, c), b(l), U(l, c) === !1))) && (l.nodeName !== "TEXTAREA" ? pe(l, c) : ie.TEXTAREA(l, c))
+            function B(c, s, h) {
+                var l = a(s);
+                l && delete v[l], !(!h && (m(c, s) === !1 || (t(c, s), L(c), M(c, s) === !1))) && (c.nodeName !== "TEXTAREA" ? ge(c, s) : ae.TEXTAREA(c, s))
             }
 
-            function pe(l, c) {
-                var a = c.firstChild,
-                    f = l.firstChild,
-                    v, w, P, G, E;
-                e: for (; a;) {
-                    for (G = a.nextSibling, v = s(a); f;) {
-                        if (P = f.nextSibling, a.isSameNode && a.isSameNode(f)) {
-                            a = G, f = P;
+            function ge(c, s) {
+                var h = j(c),
+                    l = s.firstChild,
+                    f = c.firstChild,
+                    R, w, x, G, E;
+                e: for (; l;) {
+                    for (G = l.nextSibling, R = a(l); !h && f;) {
+                        if (x = f.nextSibling, l.isSameNode && l.isSameNode(f)) {
+                            l = G, f = x;
                             continue e
                         }
-                        w = s(f);
-                        var B = f.nodeType,
+                        w = a(f);
+                        var q = f.nodeType,
                             T = void 0;
-                        if (B === a.nodeType && (B === x ? (v ? v !== w && ((E = g[v]) ? P === E ? T = !1 : (l.insertBefore(E, f), w ? L(w) : M(f, l, !0), f = E) : T = !1) : w && (T = !1), T = T !== !1 && V(f, a), T && j(f, a)) : (B === oe || B == se) && (T = !0, f.nodeValue !== a.nodeValue && (f.nodeValue = a.nodeValue))), T) {
-                            a = G, f = P;
+                        if (q === l.nodeType && (q === U ? (R ? R !== w && ((E = v[R]) ? x === E ? T = !1 : (c.insertBefore(E, f), w ? b(w) : I(f, c, !0), f = E) : T = !1) : w && (T = !1), T = T !== !1 && V(f, l), T && B(f, l)) : (q === ce || q == le) && (T = !0, f.nodeValue !== l.nodeValue && (f.nodeValue = l.nodeValue))), T) {
+                            l = G, f = x;
                             continue e
                         }
-                        w ? L(w) : M(f, l, !0), f = P
+                        w ? b(w) : I(f, c, !0), f = x
                     }
-                    if (v && (E = g[v]) && V(E, a)) l.appendChild(E), j(E, a);
+                    if (R && (E = v[R]) && V(E, l)) h || P(c, E), B(E, l);
                     else {
-                        var J = u(a);
-                        J !== !1 && (J && (a = J), a.actualize && (a = a.actualize(l.ownerDocument || p)), l.appendChild(a), F(a))
+                        var X = u(l);
+                        X !== !1 && (X && (l = X), l.actualize && (l = l.actualize(c.ownerDocument || _)), P(c, l), Q(l))
                     }
-                    a = G, f = P
+                    l = G, f = x
                 }
-                he(l, f, w);
-                var ne = ie[l.nodeName];
-                ne && ne(l, c)
-            }
-            var h = n,
-                I = h.nodeType,
-                te = i.nodeType;
-            if (!m) {
-                if (I === x) te === x ? V(n, i) || (C(n), h = Le(n, Ce(i.nodeName, i.namespaceURI))) : h = i;
-                else if (I === oe || I === se) {
-                    if (te === I) return h.nodeValue !== i.nodeValue && (h.nodeValue = i.nodeValue), h;
-                    h = i
+                me(c, f, w);
+                var ie = ae[c.nodeName];
+                ie && ie(c, s)
+            }
+            var p = n,
+                F = p.nodeType,
+                re = i.nodeType;
+            if (!k) {
+                if (F === U) re === U ? V(n, i) || (g(n), p = Re(n, ke(i.nodeName, i.namespaceURI))) : p = i;
+                else if (F === ce || F === le) {
+                    if (re === F) return p.nodeValue !== i.nodeValue && (p.nodeValue = i.nodeValue), p;
+                    p = i
                 }
             }
-            if (h === i) C(n);
+            if (p === i) g(n);
             else {
-                if (i.isSameNode && i.isSameNode(h)) return;
-                if (j(h, i, m), y)
-                    for (var z = 0, ve = y.length; z < ve; z++) {
-                        var $ = g[y[z]];
-                        $ && M($, $.parentNode, !1)
+                if (i.isSameNode && i.isSameNode(p)) return;
+                if (B(p, i, k), y)
+                    for (var J = 0, be = y.length; J < be; J++) {
+                        var K = v[y[J]];
+                        K && I(K, K.parentNode, !1)
                     }
             }
-            return !m && h !== n && n.parentNode && (h.actualize && (h = h.actualize(n.ownerDocument || p)), n.parentNode.replaceChild(h, n)), h
+            return !k && p !== n && n.parentNode && (p.actualize && (p = p.actualize(n.ownerDocument || _)), n.parentNode.replaceChild(p, n)), p
         }
     }
-    var Pe = Re(ge),
-        ae = Pe;
-    var K = function(t, e) {
-        return K = Object.setPrototypeOf || {
+    var De = Pe(Ee),
+        ue = De;
+    var Z = function(t, e) {
+        return Z = Object.setPrototypeOf || {
             __proto__: []
         }
         instanceof Array && function(n, i) {
             n.__proto__ = i
         } || function(n, i) {
             for (var r in i) i.hasOwnProperty(r) && (n[r] = i[r])
-        }, K(t, e)
+        }, Z(t, e)
     };
 
-    function ce(t, e) {
-        K(t, e);
+    function de(t, e) {
+        Z(t, e);
 
         function n() {
             this.constructor = t
         }
         t.prototype = e === null ? Object.create(e) : (n.prototype = e.prototype, new n)
     }
 
-    function xe(t) {
+    function Ue(t) {
         var e = typeof Symbol == "function" && t[Symbol.iterator],
             n = 0;
         return e ? e.call(t) : {
             next: function() {
                 return t && n >= t.length && (t = void 0), {
                     value: t && t[n++],
                     done: !t
                 }
             }
         }
     }
 
-    function ke(t, e) {
+    function Me(t, e) {
         var n = typeof Symbol == "function" && t[Symbol.iterator];
         if (!n) return t;
         var i = n.call(t),
             r, o = [],
-            s;
+            a;
         try {
             for (;
                 (e === void 0 || e-- > 0) && !(r = i.next()).done;) o.push(r.value)
         } catch (u) {
-            s = {
+            a = {
                 error: u
             }
         } finally {
             try {
                 r && !r.done && (n = i.return) && n.call(i)
             } finally {
-                if (s) throw s.error
+                if (a) throw a.error
             }
         }
         return o
     }
 
-    function De() {
-        for (var t = [], e = 0; e < arguments.length; e++) t = t.concat(ke(arguments[e]));
+    function je() {
+        for (var t = [], e = 0; e < arguments.length; e++) t = t.concat(Me(arguments[e]));
         return t
     }
-    var le = function() {
+    var fe = function() {
             function t(e, n) {
                 this.target = n, this.type = e
             }
             return t
         }(),
-        Ue = function(t) {
-            ce(e, t);
+        Ie = function(t) {
+            de(e, t);
 
             function e(n, i) {
                 var r = t.call(this, "error", i) || this;
                 return r.message = n.message, r.error = n, r
             }
             return e
-        }(le),
-        Me = function(t) {
-            ce(e, t);
+        }(fe),
+        Be = function(t) {
+            de(e, t);
 
             function e(n, i, r) {
                 n === void 0 && (n = 1e3), i === void 0 && (i = "");
                 var o = t.call(this, "close", r) || this;
                 return o.wasClean = !0, o.code = n, o.reason = i, o
             }
             return e
-        }(le);
-    var je = function() {
+        }(fe);
+    var Fe = function() {
             if (typeof WebSocket != "undefined") return WebSocket
         },
-        Ie = function(t) {
+        Ge = function(t) {
             return typeof t != "undefined" && !!t && t.CLOSING === 2
         },
         A = {
             maxReconnectionDelay: 1e4,
             minReconnectionDelay: 1e3 + Math.random() * 4e3,
             minUptime: 5e3,
             reconnectionDelayGrowFactor: 1.3,
             connectionTimeout: 4e3,
             maxRetries: 1 / 0,
             maxEnqueuedMessages: 1 / 0,
             startClosed: !1,
             debug: !1
         },
-        Ge = function() {
+        qe = function() {
             function t(e, n, i) {
                 var r = this;
                 i === void 0 && (i = {}), this._listeners = {
                     error: [],
                     message: [],
                     open: [],
                     close: []
                 }, this._retryCount = -1, this._shouldReconnect = !0, this._connectLock = !1, this._binaryType = "blob", this._closeCalled = !1, this._messageQueue = [], this.onclose = null, this.onerror = null, this.onmessage = null, this.onopen = null, this._handleOpen = function(o) {
                     r._debug("open event");
-                    var s = r._options.minUptime,
-                        u = s === void 0 ? A.minUptime : s;
+                    var a = r._options.minUptime,
+                        u = a === void 0 ? A.minUptime : a;
                     clearTimeout(r._connectTimeout), r._uptimeTimeout = setTimeout(function() {
                         return r._acceptOpen()
                     }, u), r._ws.binaryType = r._binaryType, r._messageQueue.forEach(function(d) {
                         return r._ws.send(d)
                     }), r._messageQueue = [], r.onopen && r.onopen(o), r._listeners.open.forEach(function(d) {
                         return r._callEventListener(o, d)
                     })
                 }, this._handleMessage = function(o) {
-                    r._debug("message event"), r.onmessage && r.onmessage(o), r._listeners.message.forEach(function(s) {
-                        return r._callEventListener(o, s)
+                    r._debug("message event"), r.onmessage && r.onmessage(o), r._listeners.message.forEach(function(a) {
+                        return r._callEventListener(o, a)
                     })
                 }, this._handleError = function(o) {
-                    r._debug("error event", o.message), r._disconnect(void 0, o.message === "TIMEOUT" ? "timeout" : void 0), r.onerror && r.onerror(o), r._debug("exec error listeners"), r._listeners.error.forEach(function(s) {
-                        return r._callEventListener(o, s)
+                    r._debug("error event", o.message), r._disconnect(void 0, o.message === "TIMEOUT" ? "timeout" : void 0), r.onerror && r.onerror(o), r._debug("exec error listeners"), r._listeners.error.forEach(function(a) {
+                        return r._callEventListener(o, a)
                     }), r._connect()
                 }, this._handleClose = function(o) {
-                    r._debug("close event"), r._clearTimeouts(), r._shouldReconnect && r._connect(), r.onclose && r.onclose(o), r._listeners.close.forEach(function(s) {
-                        return r._callEventListener(o, s)
+                    r._debug("close event"), r._clearTimeouts(), r._shouldReconnect && r._connect(), r.onclose && r.onclose(o), r._listeners.close.forEach(function(a) {
+                        return r._callEventListener(o, a)
                     })
                 }, this._url = e, this._protocols = n, this._options = i, this._options.startClosed && (this._shouldReconnect = !1), this._connect()
             }
             return Object.defineProperty(t, "CONNECTING", {
                 get: function() {
                     return 0
                 },
@@ -488,45 +494,45 @@
                     this._messageQueue.length < i && (this._debug("enqueue", e), this._messageQueue.push(e))
                 }
             }, t.prototype.addEventListener = function(e, n) {
                 this._listeners[e] && this._listeners[e].push(n)
             }, t.prototype.dispatchEvent = function(e) {
                 var n, i, r = this._listeners[e.type];
                 if (r) try {
-                    for (var o = xe(r), s = o.next(); !s.done; s = o.next()) {
-                        var u = s.value;
+                    for (var o = Ue(r), a = o.next(); !a.done; a = o.next()) {
+                        var u = a.value;
                         this._callEventListener(e, u)
                     }
                 } catch (d) {
                     n = {
                         error: d
                     }
                 } finally {
                     try {
-                        s && !s.done && (i = o.return) && i.call(o)
+                        a && !a.done && (i = o.return) && i.call(o)
                     } finally {
                         if (n) throw n.error
                     }
                 }
                 return !0
             }, t.prototype.removeEventListener = function(e, n) {
                 this._listeners[e] && (this._listeners[e] = this._listeners[e].filter(function(i) {
                     return i !== n
                 }))
             }, t.prototype._debug = function() {
                 for (var e = [], n = 0; n < arguments.length; n++) e[n] = arguments[n];
-                this._options.debug && console.log.apply(console, De(["RWS>"], e))
+                this._options.debug && console.log.apply(console, je(["RWS>"], e))
             }, t.prototype._getNextDelay = function() {
                 var e = this._options,
                     n = e.reconnectionDelayGrowFactor,
                     i = n === void 0 ? A.reconnectionDelayGrowFactor : n,
                     r = e.minReconnectionDelay,
                     o = r === void 0 ? A.minReconnectionDelay : r,
-                    s = e.maxReconnectionDelay,
-                    u = s === void 0 ? A.maxReconnectionDelay : s,
+                    a = e.maxReconnectionDelay,
+                    u = a === void 0 ? A.maxReconnectionDelay : a,
                     d = 0;
                 return this._retryCount > 0 && (d = o * Math.pow(i, this._retryCount - 1), d > u && (d = u)), this._debug("next delay", d), d
             }, t.prototype._wait = function() {
                 var e = this;
                 return new Promise(function(n) {
                     setTimeout(n, e._getNextDelay())
                 })
@@ -542,114 +548,109 @@
                 var e = this;
                 if (!(this._connectLock || !this._shouldReconnect)) {
                     this._connectLock = !0;
                     var n = this._options,
                         i = n.maxRetries,
                         r = i === void 0 ? A.maxRetries : i,
                         o = n.connectionTimeout,
-                        s = o === void 0 ? A.connectionTimeout : o,
+                        a = o === void 0 ? A.connectionTimeout : o,
                         u = n.WebSocket,
-                        d = u === void 0 ? je() : u;
+                        d = u === void 0 ? Fe() : u;
                     if (this._retryCount >= r) {
                         this._debug("max retries reached", this._retryCount, ">=", r);
                         return
                     }
-                    if (this._retryCount++, this._debug("connect", this._retryCount), this._removeListeners(), !Ie(d)) throw Error("No valid WebSocket class provided");
+                    if (this._retryCount++, this._debug("connect", this._retryCount), this._removeListeners(), !Ge(d)) throw Error("No valid WebSocket class provided");
                     this._wait().then(function() {
                         return e._getNextUrl(e._url)
-                    }).then(function(_) {
+                    }).then(function(m) {
                         e._closeCalled || (e._debug("connect", {
-                            url: _,
+                            url: m,
                             protocols: e._protocols
-                        }), e._ws = e._protocols ? new d(_, e._protocols) : new d(_), e._ws.binaryType = e._binaryType, e._connectLock = !1, e._addListeners(), e._connectTimeout = setTimeout(function() {
+                        }), e._ws = e._protocols ? new d(m, e._protocols) : new d(m), e._ws.binaryType = e._binaryType, e._connectLock = !1, e._addListeners(), e._connectTimeout = setTimeout(function() {
                             return e._handleTimeout()
-                        }, s))
+                        }, a))
                     })
                 }
             }, t.prototype._handleTimeout = function() {
-                this._debug("timeout event"), this._handleError(new Ue(Error("TIMEOUT"), this))
+                this._debug("timeout event"), this._handleError(new Ie(Error("TIMEOUT"), this))
             }, t.prototype._disconnect = function(e, n) {
                 if (e === void 0 && (e = 1e3), this._clearTimeouts(), !!this._ws) {
                     this._removeListeners();
                     try {
-                        this._ws.close(e, n), this._handleClose(new Me(e, n, this))
+                        this._ws.close(e, n), this._handleClose(new Be(e, n, this))
                     } catch {}
                 }
             }, t.prototype._acceptOpen = function() {
                 this._debug("accept open"), this._retryCount = 0
             }, t.prototype._callEventListener = function(e, n) {
                 "handleEvent" in n ? n.handleEvent(e) : n(e)
             }, t.prototype._removeListeners = function() {
                 !this._ws || (this._debug("removeListeners"), this._ws.removeEventListener("open", this._handleOpen), this._ws.removeEventListener("close", this._handleClose), this._ws.removeEventListener("message", this._handleMessage), this._ws.removeEventListener("error", this._handleError))
             }, t.prototype._addListeners = function() {
                 !this._ws || (this._debug("addListeners"), this._ws.addEventListener("open", this._handleOpen), this._ws.addEventListener("close", this._handleClose), this._ws.addEventListener("message", this._handleMessage), this._ws.addEventListener("error", this._handleError))
             }, t.prototype._clearTimeouts = function() {
                 clearTimeout(this._connectTimeout), clearTimeout(this._uptimeTimeout)
             }, t
         }(),
-        X = Ge;
-    var W = JSON.parse(document.querySelector("meta[name=reactor-boost]")?.dataset.enabled || "false");
-    console.log("BOOST_PAGES", W);
+        ee = qe;
+    var z = JSON.parse(document.querySelector("meta[name=reactor-boost]")?.dataset.enabled || "false");
+    console.log("BOOST_PAGES", z);
 
-    function ue() {
-        if (W)
-            for (let t of document.querySelectorAll("a[href]")) fe(t)
+    function he() {
+        if (z)
+            for (let t of document.querySelectorAll("a[href]")) pe(t)
     }
 
-    function fe(t) {
-        W && t.tagName?.toLowerCase() === "a" && t.hasAttribute("href") && !(t.boosted || t.hasAttribute("onclick") || t.hasAttribute(":no-boost")) && (t.boosted = !0, t.addEventListener("click", Be))
+    function pe(t) {
+        z && t.tagName?.toLowerCase() === "a" && t.hasAttribute("href") && !(t.boosted || t.hasAttribute("onclick") || t.hasAttribute("target") || t.hasAttribute(":no-boost")) && (t.boosted = !0, t.addEventListener("click", He))
     }
 
-    function Be(t) {
-        t.preventDefault(), R.load(t.target.href)
+    function He(t) {
+        t.preventDefault();
+        let e = t.target.tagName?.toLowerCase === "a" ? t.target.href : t.target.closest("a").href;
+        N.load(e)
     }
 
-    function Y(t, e) {
+    function _e(t, e) {
         console.log("replaceBodyContent", e);
         let n = document.createElement("html");
         n.innerHTML = t, window.requestAnimationFrame(() => {
-            e?.beforeReplace && e.beforeReplace(n), document.body = n.querySelector("body"), ue(), e?.afterReplace && e.afterReplace(n)
+            e?.beforeReplace && e.beforeReplace(n), document.body = n.querySelector("body"), he(), e?.afterReplace && e.afterReplace(n), document.querySelector("[autofocus]")?.focus()
         })
     }
 
-    function He(t) {
+    function We(t) {
         return t.startsWith("http://") || t.startsWith("https://") ? new URL(t).origin === document.location.origin : !0
     }
-    var k = class {
+    var te = class {
             static async load(e) {
-                W ? (this._saveCurrentPage(), console.log(e), He(e) ? (this.push(e), await this.restoreFromCurrentPath()) : location.assign(e)) : location.assign(e)
-            }
-            static loadContent(e, n) {
-                console.log("Load content", e), Y(n, {
-                    beforeReplace(i) {
-                        k._saveCurrentPage(), k.push(e), document.title = i.querySelector("title")?.text ?? ""
-                    }
-                })
+                z ? (this._saveCurrentPage(), console.log(e), We(e) ? (this.push(e), await this.restoreFromCurrentPath()) : location.assign(e)) : location.assign(e)
             }
             static async restoreFromCurrentPath() {
                 this._saveCurrentPage();
                 let e = window.location.pathname + window.location.search;
                 console.log("Restoring Page:", e);
                 let n = this._get(e);
-                n && (Y(n.content, {
+                n && (_e(n.content, {
                     beforeReplace() {
                         document.title = n.title
                     },
                     afterReplace() {
                         window.scrollTo(0, n.scroll)
                     }
                 }), console.log("currentPath", e), this.currentPath = e);
                 let i = await fetch(window.location.href),
                     r = await i.text();
-                this.replace(i.url), Y(r, {
+                this.replace(i.url), _e(r, {
                     beforeReplace(o) {
                         document.title = o.querySelector("title")?.text ?? ""
                     },
                     afterReplace() {
-                        k._saveCurrentPage()
+                        te._saveCurrentPage()
                     }
                 })
             }
             static back() {
                 window.history.back()
             }
             static push(e) {
@@ -674,102 +675,146 @@
                     url: e
                 }) => e))
             }
             static _get(e) {
                 return this.cache.find(n => n.url == e)
             }
         },
-        R = k;
-    H(R, "maxSize", 10), H(R, "cache", []), H(R, "currentPath", window.location.pathname + window.location.search);
+        N = te;
+    H(N, "maxSize", 10), H(N, "cache", []), H(N, "currentPath", window.location.pathname + window.location.search);
     window.addEventListener("popstate", t => {
-        R.restoreFromCurrentPath()
+        N.restoreFromCurrentPath()
     });
     window.addEventListener("load", () => {
-        ue()
+        he()
     });
-    var S = {
-        boostElement: fe,
-        HistoryCache: R
+    var O = {
+        boostElement: pe,
+        HistoryCache: N
     };
-    var de = class extends EventTarget {
+    var Ve = new DOMParser,
+        ve = class extends EventTarget {
             open(e = "__reactor__") {
                 let n = location.protocol.replace("http", "ws");
-                this.socket = new X(`${n}//${location.host}/${e}`, [], {
+                this.socket = new ee(`${n}//${location.host}/${e}`, [], {
                     maxEnqueuedMessages: 0
                 }), this.socket.addEventListener("open", () => {
                     console.log("WS: OPEN"), this.dispatchEvent(new Event("open"))
                 }), this.socket.addEventListener("message", i => this._processMessage(i)), this.socket.addEventListener("close", () => {
                     console.log("WS: CLOSE"), this.dispatchEvent(new Event("close"))
                 })
             }
             get isOpen() {
-                return this.socket?.readyState == X.OPEN
+                return this.socket?.readyState == ee.OPEN
             }
             _processMessage(e) {
                 let {
                     command: n,
                     payload: i
                 } = JSON.parse(e.data);
                 switch (n) {
                     case "render":
                         var {
                             id: r, diff: o
                         } = i;
                         console.log("<<< RENDER", r), document.getElementById(r)?.applyDiff(o);
                         break;
+                    case "append":
+                    case "prepend":
+                    case "insert_after":
+                    case "insert_before":
+                    case "replace_with":
+                        var {
+                            id: r, html: a
+                        } = i;
+                        console.log(`<<< ${n.toUpperCase()}`, r), a = Ve.parseFromString(a, "text/html").body.firstChild;
+                        var u = document.getElementById(r);
+                        switch (n) {
+                            case "append":
+                                u?.append(a);
+                                break;
+                            case "prepend":
+                                u?.prepend(a);
+                                break;
+                            case "insert_after":
+                                u?.after(a);
+                                break;
+                            case "insert_before":
+                                u?.before(a);
+                                break;
+                            case "replace_with":
+                                u?.replaceWith(a);
+                                break
+                        }
+                        break;
                     case "remove":
                         var {
                             id: r
                         } = i;
                         console.log("<<< REMOVE", r), document.getElementById(r)?.remove();
                         break;
                     case "focus_on":
                         var {
-                            selector: s
+                            selector: d
+                        } = i;
+                        console.log("<<< FOCUS-ON", `"${d}"`, document.querySelector(d)), window.requestAnimationFrame(() => document.querySelector(d)?.focus());
+                        break;
+                    case "scroll_into_view":
+                        var {
+                            id: r, behavior: m, block: L, inline: $
                         } = i;
-                        console.log("<<< FOCUS-ON", `"${s}"`), document.querySelector(s)?.focus();
+                        window.requestAnimationFrame(() => document.getElementById(r)?.scrollIntoView({
+                            behavior: m,
+                            block: L,
+                            inline: $
+                        }));
                         break;
-                    case "visit":
+                    case "url_change":
                         var {
-                            url: u, replace: d
+                            url: g
                         } = i;
-                        d ? (console.log("<< REPLACE", u), S.HistoryCache.replace(u)) : (console.log("<< VISIT", u), S.HistoryCache.load(u));
+                        switch (console.log("<< URL", i.command, g), i.command) {
+                            case "redirect":
+                                O.HistoryCache.load(g);
+                                break;
+                            case "replace":
+                                O.HistoryCache.replace(g);
+                                break;
+                            case "push":
+                                O.HistoryCache.push(g);
+                                break
+                        }
                         break;
                     case "set_url_params":
                         console.log("<< SET URL PARAMS", i);
-                        let b = document.location.search.slice(1),
-                            D = {};
-                        b.length && (D = b.split("&").map(m => m.split("=")).reduce((m, g) => {
-                            let [y, L] = g;
-                            return m[y] = L === void 0 ? void 0 : decodeURIComponent(L), m
+                        let M = document.location.search.slice(1),
+                            j = {};
+                        M.length && (j = M.split("&").map(v => v.split("=")).reduce((v, y) => {
+                            let [b, D] = y;
+                            return v[b] = D === void 0 ? void 0 : decodeURIComponent(D), v
                         }, {}));
-                        let C = Object.entries(Object.assign(D, i)).map(m => {
-                                let [g, y] = m;
-                                return g + (y === void 0 ? "" : `=${encodeURIComponent(y)}`)
+                        let P = Object.entries(Object.assign(j, i)).map(v => {
+                                let [y, b] = v;
+                                return y + (b === void 0 ? "" : `=${encodeURIComponent(b)}`)
                             }),
-                            U = document.location.pathname;
-                        C.length && (U += "?" + C.join("&")), S.HistoryCache.replace(U);
-                        break;
-                    case "page":
-                        var {
-                            url: u, content: _
-                        } = i;
-                        console.log("<< PAGE", `"${u}"`), S.HistoryCache.loadContent(u, _);
+                            k = document.location.pathname;
+                        P.length && (k += "?" + P.join("&")), O.HistoryCache.replace(k);
                         break;
                     case "back":
-                        S.HistoryCache.back();
+                        O.HistoryCache.back();
                         break;
                     default:
                         console.error(`Unknown command "${n}"`, i)
                 }
             }
-            sendJoin(e, n) {
-                console.log(">>> JOIN", e), this._send("join", {
+            sendJoin(e, n, i) {
+                this._send("join", {
                     name: e,
-                    state: n
+                    parent_id: n,
+                    state: i
                 })
             }
             sendLeave(e) {
                 console.log(">>> LEAVE", e), this._send("leave", {
                     id: e
                 })
             }
@@ -784,93 +829,93 @@
             _send(e, n) {
                 this.isOpen && this.socket.send(JSON.stringify({
                     command: e,
                     payload: n
                 }))
             }
         },
-        O = new de;
+        C = new ve;
     for ({
             dataset
         }
         of document.querySelectorAll("meta[name=reactor-component]")) {
         let t = document.createElement(dataset.extends);
         class e extends t.constructor {
             constructor(...i) {
                 super(...i);
                 this._lastReceivedHtml = [], this.joinBind = () => this.join(), this.wentOffline = () => this.classList.add("reactor-disconnected")
             }
             connectedCallback() {
-                O.addEventListener("open", this.joinBind), O.addEventListener("close", this.wentOffline), this.join()
+                C.addEventListener("open", this.joinBind), C.addEventListener("close", this.wentOffline), this.join()
             }
             disconnectedCallback() {
-                O.removeEventListener("open", this.joinBind), O.removeEventListener("close", this.wentOffline), O.sendLeave(this.id)
+                C.removeEventListener("open", this.joinBind), C.removeEventListener("close", this.wentOffline), C.sendLeave(this.id)
             }
             join() {
-                this.classList.remove("reactor-disconnected"), this.isRoot && O.sendJoin(this.dataset.name, this.dataset.state)
+                this.classList.remove("reactor-disconnected"), C.sendJoin(this.dataset.name, this.parentId, this.dataset.state)
             }
             applyDiff(i) {
                 let r = this.getHtml(i);
                 window.requestAnimationFrame(() => {
-                    ae(this, r, {
+                    ue(this, r, {
                         onBeforeNodeAdded(o) {
-                            S.boostElement(o)
+                            O.boostElement(o)
                         },
                         onElUpdated(o) {
-                            S.boostElement(o)
+                            O.boostElement(o)
                         }
                     })
                 })
             }
             getHtml(i) {
                 let r = [],
                     o = 0;
-                for (let s of i) typeof s == "string" ? r.push(s) : s < 0 ? o -= s : (r.push(...this._lastReceivedHtml.slice(o, o + s)), o += s);
+                for (let a of i) typeof a == "string" ? r.push(a) : a < 0 ? o -= a : (r.push(...this._lastReceivedHtml.slice(o, o + a)), o += a);
                 return this._lastReceivedHtml = r, r.join(" ")
             }
-            get isRoot() {
-                return !this.parentComponent
+            get parentId() {
+                return this.parentComponent?.id
             }
             get parentComponent() {
                 return this.parentElement?.closest("[reactor-component]")
             }
             dispatch(i, r, o) {
-                O.sendUserEvent(this.id, i, this.serialize(o), r)
+                C.sendUserEvent(this.id, i, this.serialize(o), r)
             }
             serialize(i) {
                 let r = {};
                 for (let o of i.querySelectorAll("[name]")) {
                     if (o.closest("[reactor-component]") !== this) continue;
-                    let s = null;
+                    let a = null;
                     switch (o.type.toLowerCase()) {
                         case "checkbox":
                         case "radio":
-                            s = o.checked ? o.value || !0 : null;
+                            a = o.checked ? o.value || !0 : null;
                             break;
                         case "select-multiple":
-                            s = o.selectedOptions.map(u => u.value);
+                            a = o.selectedOptions.map(u => u.value);
                             break;
                         default:
-                            s = o.value;
+                            a = o.value;
                             break
                     }
-                    if (s !== null) {
+                    if (a !== null) {
                         let u = o.getAttribute("name"),
                             d = r[u] ?? [];
-                        d.push(s), r[u] = d
+                        d.push(a), r[u] = d
                     }
                 }
                 return r
             }
         }
         customElements.define(dataset.tagName, e, {
             extends: dataset.extends
         })
     }
-    O.open();
+    C.open();
     debounceTimeouts = {};
     window.reactor = {
         send(t, e, n) {
             let i = t.closest("[reactor-component]");
             if (i !== null) {
                 let r = t.closest("form"),
                     o = i.contains(r) ? r : i;
```

### Comparing `django-reactor-4.0.2b0/reactor/templatetags/reactor.py` & `django-reactor-5.0.0b0/reactor/templatetags/reactor.py`

 * *Files 3% similar despite different names*

```diff
@@ -22,21 +22,23 @@
         ],
         "BOOST_PAGES": settings.BOOST_PAGES,
     }
 
 
 @register.simple_tag(takes_context=True)
 def tag_header(context):
-    component = context["this"]
+    component: Component = context["this"]
     return format_html(
-        'is="{tag_name}" '
-        'id="{id}" '
-        'data-name="{name}" '
-        'data-state="{state}"'
-        "reactor-component",
+        (
+            'is="{tag_name}" '
+            'id="{id}" '
+            'data-name="{name}" '
+            'data-state="{state}" '
+            "reactor-component"
+        ),
         tag_name=component._tag_name,
         id=component.id,
         name=component._name,
         state=Signer().sign(component.json(exclude=component._exclude_fields)),
     )
 
 
@@ -46,27 +48,26 @@
     parent_id = parent.id if parent else None
 
     repo: ComponentRepository = context.get(
         "reactor_repository",
         ComponentRepository(user=context.get("user")),
     )
 
-    component = repo.new(_name, state=kwargs, parent_id=parent_id)
-    return component.render(repo) or ""
+    component, _created = repo.build(_name, state=kwargs, parent_id=parent_id)
+    return component._render(repo) or ""
 
 
 @register.simple_tag(takes_context=True)
 def on(context, _event_and_modifiers, _command, **kwargs: t.Any):
     component: t.Optional[Component] = context.get("this")
 
     assert component, "Can't find a component in this context"
-    attr_name = settings.RECEIVER_PREFIX + _command
-    handler = getattr(component, attr_name, None)
-    assert handler, f"Missing handler: {component._name}.{attr_name}"
-    assert callable(handler), f"Not callable: {component._name}.{attr_name}"
+    handler = getattr(component, _command, None)
+    assert handler, f"Missing handler: {component._name}.{_command}"
+    assert callable(handler), f"Not callable: {component._name}.{_command}"
 
     event, code = transpile(_event_and_modifiers, _command, kwargs)
     return format_html('{event}="{code}"', event=event, code=code)
 
 
 @register.filter(name="str")
 def to_string(value):
```

### Comparing `django-reactor-4.0.2b0/reactor/utils.py` & `django-reactor-5.0.0b0/reactor/utils.py`

 * *Files 6% similar despite different names*

```diff
@@ -14,25 +14,21 @@
         from django.db.transaction import on_commit  # type: ignore
 
         on_commit(lambda: f(*args, **kwargs))
 
     return wrapper
 
 
+@on_commit
 def send_to(channel: t.Optional[str], type: str, **kwargs: t.Any):
     """Sends a message of `type` to the"""
     if channel:
-
-        @on_commit
-        def send_message():
-            async_to_sync(get_channel_layer().group_send)(
-                channel, dict(type=type, channel=channel, **kwargs)
-            )
-
-        send_message()
+        async_to_sync(get_channel_layer().group_send)(
+            channel, dict(type=type, channel=channel, **kwargs)
+        )
 
 
 # Introspection
 
 
 def filter_parameters(f, kwargs):
     has_kwargs = any(
```

### Comparing `django-reactor-4.0.2b0/setup.cfg` & `django-reactor-5.0.0b0/setup.cfg`

 * *Files 16% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [metadata]
 name = django-reactor
-version = 4.0.2b0
+version = 5.0.0b0
 description = Brings LiveView from Phoenix framework into Django
 long_description = file: README.md
 long_description_content_type = text/markdown
 classifiers = 
 	Development Status :: 4 - Beta
 	Environment :: Web Environment
 	Framework :: Django
@@ -26,14 +26,15 @@
 zip_safe = False
 packages = find:
 include_package_data = True
 python_requires = >=3.9
 install_requires = 
 	channels>=4,<5
 	pydantic>=1.8,<2
+	lru-dict>=1.2.0,<2
 
 [options.extras_require]
 dev = 
 	black
 	djlint
 	flake8
 	ipython
```

