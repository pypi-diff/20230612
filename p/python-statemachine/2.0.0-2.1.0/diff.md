# Comparing `tmp/python_statemachine-2.0.0.tar.gz` & `tmp/python_statemachine-2.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "python_statemachine-2.0.0.tar", max compression
+gzip compressed data, was "python_statemachine-2.1.0.tar", max compression
```

## Comparing `python_statemachine-2.0.0.tar` & `python_statemachine-2.1.0.tar`

### file list

```diff
@@ -1,30 +1,31 @@
--rw-r--r--   0        0        0     1074 2023-01-12 02:09:26.102515 python_statemachine-2.0.0/LICENSE
--rw-r--r--   0        0        0     9017 2023-03-05 18:33:06.733302 python_statemachine-2.0.0/README.md
--rw-r--r--   0        0        0     3878 2023-03-05 22:12:14.963306 python_statemachine-2.0.0/pyproject.toml
--rw-r--r--   0        0        0      192 2023-03-05 21:00:56.603303 python_statemachine-2.0.0/statemachine/__init__.py
--rw-r--r--   0        0        0     5582 2023-03-05 20:54:27.723304 python_statemachine-2.0.0/statemachine/callbacks.py
--rw-r--r--   0        0        0        0 2023-01-12 02:09:26.112515 python_statemachine-2.0.0/statemachine/contrib/__init__.py
--rw-r--r--   0        0        0     6748 2023-02-11 14:38:42.139628 python_statemachine-2.0.0/statemachine/contrib/diagram.py
--rw-r--r--   0        0        0     2598 2023-03-04 21:01:58.766581 python_statemachine-2.0.0/statemachine/dispatcher.py
--rw-r--r--   0        0        0     2106 2023-03-05 20:54:27.723304 python_statemachine-2.0.0/statemachine/event.py
--rw-r--r--   0        0        0     2257 2023-03-05 18:33:06.733302 python_statemachine-2.0.0/statemachine/event_data.py
--rw-r--r--   0        0        0      731 2023-01-27 15:22:34.528394 python_statemachine-2.0.0/statemachine/events.py
--rw-r--r--   0        0        0      952 2023-03-05 18:33:06.733302 python_statemachine-2.0.0/statemachine/exceptions.py
--rw-r--r--   0        0        0     4815 2023-03-04 21:02:13.886582 python_statemachine-2.0.0/statemachine/factory.py
--rw-r--r--   0        0        0      359 2023-01-12 02:09:26.112515 python_statemachine-2.0.0/statemachine/graph.py
--rw-r--r--   0        0        0      362 2023-03-04 21:01:58.766581 python_statemachine-2.0.0/statemachine/i18n.py
--rw-r--r--   0        0        0      452 2023-03-05 21:52:02.723307 python_statemachine-2.0.0/statemachine/locale/en/LC_MESSAGES/statemachine.mo
--rw-r--r--   0        0        0     1685 2023-03-05 21:51:15.653307 python_statemachine-2.0.0/statemachine/locale/en/LC_MESSAGES/statemachine.po
--rw-r--r--   0        0        0     1914 2023-03-05 21:52:02.733307 python_statemachine-2.0.0/statemachine/locale/pt_BR/LC_MESSAGES/statemachine.mo
--rw-r--r--   0        0        0     2375 2023-03-05 21:51:21.823307 python_statemachine-2.0.0/statemachine/locale/pt_BR/LC_MESSAGES/statemachine.po
--rw-r--r--   0        0        0     1055 2023-03-05 20:42:52.873306 python_statemachine-2.0.0/statemachine/mixins.py
--rw-r--r--   0        0        0      132 2023-01-27 15:22:34.528394 python_statemachine-2.0.0/statemachine/model.py
--rw-r--r--   0        0        0      933 2023-01-27 15:22:34.528394 python_statemachine-2.0.0/statemachine/registry.py
--rw-r--r--   0        0        0     6149 2023-03-02 20:56:10.368071 python_statemachine-2.0.0/statemachine/signature.py
--rw-r--r--   0        0        0     7052 2023-03-05 18:33:06.733302 python_statemachine-2.0.0/statemachine/state.py
--rw-r--r--   0        0        0    11157 2023-03-05 18:33:06.733302 python_statemachine-2.0.0/statemachine/statemachine.py
--rw-r--r--   0        0        0     4637 2023-03-05 20:54:27.723304 python_statemachine-2.0.0/statemachine/transition.py
--rw-r--r--   0        0        0     2149 2023-02-22 20:41:50.222256 python_statemachine-2.0.0/statemachine/transition_list.py
--rw-r--r--   0        0        0      416 2023-03-04 21:01:58.766581 python_statemachine-2.0.0/statemachine/utils.py
--rw-r--r--   0        0        0    10112 1970-01-01 00:00:00.000000 python_statemachine-2.0.0/setup.py
--rw-r--r--   0        0        0    10161 1970-01-01 00:00:00.000000 python_statemachine-2.0.0/PKG-INFO
+-rw-r--r--   0        0        0     1074 2023-01-12 02:09:26.102515 python_statemachine-2.1.0/LICENSE
+-rw-r--r--   0        0        0    10510 2023-06-12 01:16:16.754636 python_statemachine-2.1.0/README.md
+-rw-r--r--   0        0        0     3966 2023-06-12 01:17:52.284641 python_statemachine-2.1.0/pyproject.toml
+-rw-r--r--   0        0        0      192 2023-06-12 01:17:52.284641 python_statemachine-2.1.0/statemachine/__init__.py
+-rw-r--r--   0        0        0     5714 2023-06-12 01:16:16.754636 python_statemachine-2.1.0/statemachine/callbacks.py
+-rw-r--r--   0        0        0        0 2023-01-12 02:09:26.112515 python_statemachine-2.1.0/statemachine/contrib/__init__.py
+-rw-r--r--   0        0        0     6748 2023-03-05 22:27:00.883303 python_statemachine-2.1.0/statemachine/contrib/diagram.py
+-rw-r--r--   0        0        0     2884 2023-06-12 01:16:16.754636 python_statemachine-2.1.0/statemachine/dispatcher.py
+-rw-r--r--   0        0        0     2106 2023-03-13 01:49:09.127086 python_statemachine-2.1.0/statemachine/event.py
+-rw-r--r--   0        0        0     2257 2023-03-13 01:45:45.507089 python_statemachine-2.1.0/statemachine/event_data.py
+-rw-r--r--   0        0        0      731 2023-03-05 22:27:00.883303 python_statemachine-2.1.0/statemachine/events.py
+-rw-r--r--   0        0        0      952 2023-03-13 01:45:45.507089 python_statemachine-2.1.0/statemachine/exceptions.py
+-rw-r--r--   0        0        0     5557 2023-06-12 01:16:16.754636 python_statemachine-2.1.0/statemachine/factory.py
+-rw-r--r--   0        0        0      359 2023-01-12 02:09:26.112515 python_statemachine-2.1.0/statemachine/graph.py
+-rw-r--r--   0        0        0      362 2023-03-05 22:27:00.883303 python_statemachine-2.1.0/statemachine/i18n.py
+-rw-r--r--   0        0        0      452 2023-06-12 01:10:29.514642 python_statemachine-2.1.0/statemachine/locale/en/LC_MESSAGES/statemachine.mo
+-rw-r--r--   0        0        0     1685 2023-06-12 01:17:52.284641 python_statemachine-2.1.0/statemachine/locale/en/LC_MESSAGES/statemachine.po
+-rw-r--r--   0        0        0     1914 2023-06-12 01:10:29.514642 python_statemachine-2.1.0/statemachine/locale/pt_BR/LC_MESSAGES/statemachine.mo
+-rw-r--r--   0        0        0     2375 2023-06-12 01:17:52.284641 python_statemachine-2.1.0/statemachine/locale/pt_BR/LC_MESSAGES/statemachine.po
+-rw-r--r--   0        0        0     1055 2023-03-13 01:45:45.507089 python_statemachine-2.1.0/statemachine/mixins.py
+-rw-r--r--   0        0        0      211 2023-06-12 01:16:16.764636 python_statemachine-2.1.0/statemachine/model.py
+-rw-r--r--   0        0        0      959 2023-06-12 01:16:16.764636 python_statemachine-2.1.0/statemachine/registry.py
+-rw-r--r--   0        0        0     6260 2023-06-12 01:16:16.764636 python_statemachine-2.1.0/statemachine/signature.py
+-rw-r--r--   0        0        0     7057 2023-06-12 01:16:16.764636 python_statemachine-2.1.0/statemachine/state.py
+-rw-r--r--   0        0        0    11608 2023-06-12 01:16:16.764636 python_statemachine-2.1.0/statemachine/statemachine.py
+-rw-r--r--   0        0        0     4151 2023-06-12 01:16:16.764636 python_statemachine-2.1.0/statemachine/states.py
+-rw-r--r--   0        0        0     4637 2023-03-13 01:45:45.507089 python_statemachine-2.1.0/statemachine/transition.py
+-rw-r--r--   0        0        0     5949 2023-06-12 01:16:16.764636 python_statemachine-2.1.0/statemachine/transition_list.py
+-rw-r--r--   0        0        0      367 2023-06-12 01:16:16.764636 python_statemachine-2.1.0/statemachine/utils.py
+-rw-r--r--   0        0        0    11639 1970-01-01 00:00:00.000000 python_statemachine-2.1.0/setup.py
+-rw-r--r--   0        0        0    11654 1970-01-01 00:00:00.000000 python_statemachine-2.1.0/PKG-INFO
```

### Comparing `python_statemachine-2.0.0/LICENSE` & `python_statemachine-2.1.0/LICENSE`

 * *Files identical despite different names*

### Comparing `python_statemachine-2.0.0/README.md` & `python_statemachine-2.1.0/README.md`

 * *Files 18% similar despite different names*

```diff
@@ -55,19 +55,19 @@
 
 >>> class TrafficLightMachine(StateMachine):
 ...     "A traffic light machine"
 ...     green = State(initial=True)
 ...     yellow = State()
 ...     red = State()
 ...
-...     cycle = green.to(yellow) | yellow.to(red) | red.to(green)
-...
-...     slowdown = green.to(yellow)
-...     stop = yellow.to(red)
-...     go = red.to(green)
+...     cycle = (
+...         green.to(yellow)
+...         | yellow.to(red)
+...         | red.to(green)
+...     )
 ...
 ...     def before_cycle(self, event: str, source: State, target: State, message: str = ""):
 ...         message = ". " + message if message else ""
 ...         return f"Running {event} from {source.id} to {target.id}{message}"
 ...
 ...     def on_enter_red(self):
 ...         print("Don't move.")
@@ -76,132 +76,171 @@
 ...         print("Go ahead!")
 
 ```
 
 You can now create an instance:
 
 ```py
->>> traffic_light = TrafficLightMachine()
+>>> sm = TrafficLightMachine()
 
 ```
 
-Then start sending events:
+This state machine can be represented graphically as follows:
 
 ```py
->>> traffic_light.cycle()
-'Running cycle from green to yellow'
+>>> img_path = "docs/images/readme_trafficlightmachine.png"
+>>> sm._graph().write_png(img_path)
 
 ```
 
-You can inspect the current state:
+![](https://raw.githubusercontent.com/fgmacedo/python-statemachine/develop/docs/images/readme_trafficlightmachine.png)
+
+
+Where on the `TrafficLightMachine`, we've defined `green`, `yellow`, and `red` as states, and
+one event called `cycle`, which is bound to the transitions from `green` to `yellow`, `yellow` to `red`,
+and `red` to `green`. We also have defined three callbacks by name convention, `before_cycle`, `on_enter_red`, and `on_exit_red`.
+
+
+Then start sending events to your new state machine:
 
 ```py
->>> traffic_light.current_state.id
-'yellow'
+>>> sm.send("cycle")
+'Running cycle from green to yellow'
 
 ```
 
-A `State` human-readable name is automatically derived from the `State.id`:
+That's it. This is all an external object needs to know about your state machine: How to send events.
+Ideally, all states, transitions, and actions should be kept internally and not checked externally to avoid unnecessary coupling.
+
+But if your use case needs, you can inspect state machine properties, like the current state:
 
 ```py
->>> traffic_light.current_state.name
-'Yellow'
+>>> sm.current_state.id
+'yellow'
 
 ```
 
 Or get a complete state representation for debugging purposes:
 
 ```py
->>> traffic_light.current_state
+>>> sm.current_state
 State('Yellow', id='yellow', value='yellow', initial=False, final=False)
 
 ```
 
-The ``State`` instance can also be checked by equality:
+The `State` instance can also be checked by equality:
 
 ```py
->>> traffic_light.current_state == TrafficLightMachine.yellow
+>>> sm.current_state == TrafficLightMachine.yellow
 True
 
->>> traffic_light.current_state == traffic_light.yellow
+>>> sm.current_state == sm.yellow
 True
 
 ```
 
-But for your convenience, can easily ask if a state is active at any time:
+Or you can check if a state is active at any time:
 
 ```py
->>> traffic_light.green.is_active
+>>> sm.green.is_active
 False
 
->>> traffic_light.yellow.is_active
+>>> sm.yellow.is_active
 True
 
->>> traffic_light.red.is_active
+>>> sm.red.is_active
 False
 
 ```
 
 Easily iterate over all states:
 
 ```py
->>> [s.id for s in traffic_light.states]
+>>> [s.id for s in sm.states]
 ['green', 'red', 'yellow']
 
 ```
 
 Or over events:
 
 ```py
->>> [t.name for t in traffic_light.events]
-['cycle', 'go', 'slowdown', 'stop']
+>>> [t.name for t in sm.events]
+['cycle']
 
 ```
 
 Call an event by its name:
 
 ```py
->>> traffic_light.cycle()
+>>> sm.cycle()
 Don't move.
 'Running cycle from yellow to red'
 
 ```
 Or send an event with the event name:
 
 ```py
->>> traffic_light.send('cycle')
+>>> sm.send('cycle')
 Go ahead!
 'Running cycle from red to green'
 
->>> traffic_light.green.is_active
+>>> sm.green.is_active
 True
 
 ```
-You can't run a transition from an invalid state:
+
+You can pass arbitrary positional or keyword arguments to the event, and
+they will be propagated to all actions and callbacks using something similar to dependency injection. In other words, the library will only inject the parameters declared on the
+callback method.
+
+Note how `before_cycle` was declared:
+
+```py
+def before_cycle(self, event: str, source: State, target: State, message: str = ""):
+    message = ". " + message if message else ""
+    return f"Running {event} from {source.id} to {target.id}{message}"
+```
+
+The params `event`, `source`, `target` (and others) are available built-in to be used on any action.
+The param `message` is user-defined, in our example we made it default empty so we can call `cycle` with
+or without a `message` parameter.
+
+If we pass a `message` parameter, it will be used on the `before_cycle` action:
+
+```py
+>>> sm.send("cycle", message="Please, now slowdown.")
+'Running cycle from green to yellow. Please, now slowdown.'
+
+```
+
+
+By default, events with transitions that cannot run from the current state or unknown events
+raise a `TransitionNotAllowed` exception:
 
 ```py
->>> traffic_light.go()
+>>> sm.send("go")
 Traceback (most recent call last):
-statemachine.exceptions.TransitionNotAllowed: Can't go when in Green.
+statemachine.exceptions.TransitionNotAllowed: Can't go when in Yellow.
 
 ```
+
 Keeping the same state as expected:
 
 ```py
->>> traffic_light.green.is_active
+>>> sm.yellow.is_active
 True
 
 ```
 
-And you can pass arbitrary positional or keyword arguments to the event, and
-they will be propagated to all actions and callbacks:
+A human-readable name is automatically derived from the `State.id`, which is used on the messages
+and in diagrams:
 
 ```py
->>> traffic_light.cycle(message="Please, now slowdown.")
-'Running cycle from green to yellow. Please, now slowdown.'
+>>> sm.current_state.name
+'Yellow'
 
 ```
 
 ## A more useful example
 
 A simple didactic state machine for controlling an `Order`:
```

### Comparing `python_statemachine-2.0.0/pyproject.toml` & `python_statemachine-2.1.0/pyproject.toml`

 * *Files 14% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "python-statemachine"
-version = "2.0.0"
+version = "2.1.0"
 description = "Python Finite State Machines made easy."
 authors = ["Fernando Macedo <fgmacedo@gmail.com>"]
 maintainers = [
     "Fernando Macedo <fgmacedo@gmail.com>",
 ]
 license = "MIT license"
 readme = "README.md"
@@ -36,26 +36,25 @@
 python = ">=3.7, <3.12"
 
 [tool.poetry.group.dev.dependencies]
 pytest = "^7.2.0"
 pytest-cov = "^4.0.0"
 pytest-sugar = "^0.9.6"
 pydot = "^1.4.2"
-ruff = "^0.0.220"
+ruff = "^0.0.257"
 pre-commit = "^2.21.0"
 mypy = "^0.991"
 black = "^22.12.0"
 pdbpp = "^0.10.3"
 
 [tool.poetry.group.docs.dependencies]
 Sphinx = "4.5.0"
 sphinx-rtd-theme = "1.1.1"
 myst-parser = "^0.18.1"
 sphinx-gallery = "^0.11.1"
-jupyterlite-sphinx = "^0.7.2"
 pillow = "^9.4.0"
 sphinx-autobuild = "^2021.3.14"
 
 [build-system]
 requires = ["poetry-core"]
 build-backend = "poetry.core.masonry.api"
 
@@ -96,14 +95,16 @@
     "UP", # pyupgrade
     "C",  # flake8-comprehensions
     "B",  # flake8-bugbear
     "PT", # flake8-pytest-style
 ]
 ignore = [
     "UP006", # `use-pep585-annotation` Requires Python3.9+
+    "UP035", # `use-pep585-annotation` Requires Python3.9+
+    "UP038", # `use-pep585-annotation` Requires Python3.9+
 ]
 
 line-length = 99
 
 # Exclude a variety of commonly ignored directories.
 exclude = [
     ".direnv",
```

### Comparing `python_statemachine-2.0.0/statemachine/callbacks.py` & `python_statemachine-2.1.0/statemachine/callbacks.py`

 * *Files 5% similar despite different names*

```diff
@@ -15,23 +15,24 @@
     """
 
     def __init__(self, func, suppress_errors=False, cond=None):
         self.func = func
         self.suppress_errors = suppress_errors
         self.cond = Callbacks(factory=ConditionWrapper).add(cond)
         self._callback = None
+        self._resolver_id = None
 
     def __repr__(self):
         return f"{type(self).__name__}({self.func!r})"
 
     def __str__(self):
         return getattr(self.func, "__name__", self.func)
 
     def __eq__(self, other):
-        return self.func == getattr(other, "func", other)
+        return self.func == other.func and self._resolver_id == other._resolver_id
 
     def __hash__(self):
         return id(self)
 
     def _update_func(self, func):
         self.func = func
 
@@ -41,14 +42,15 @@
 
         Args:
             resolver (callable): A method responsible to build and return a valid callable that
                 can receive arbitrary parameters like `*args, **kwargs`.
         """
         self.cond.setup(resolver)
         try:
+            self._resolver_id = getattr(resolver, "id", id(resolver))
             self._callback = resolver(self.func)
             return True
         except AttrNotFound:
             if not self.suppress_errors:
                 raise
             return False
 
@@ -140,23 +142,23 @@
             if callback.cond.all(*args, **kwargs)
         ]
 
     def all(self, *args, **kwargs):
         return all(condition(*args, **kwargs) for condition in self)
 
     def _add(self, func, resolver=None, prepend=False, **kwargs):
-        if func in self.items:
-            return
-
         resolver = resolver or self._resolver
 
         callback = self.factory(func, **kwargs)
         if resolver is not None and not callback.setup(resolver):
             return
 
+        if callback in self.items:
+            return
+
         if prepend:
             self.items.insert(0, callback)
         else:
             self.items.append(callback)
         return callback
 
     def add(self, callbacks, **kwargs):
```

### Comparing `python_statemachine-2.0.0/statemachine/contrib/diagram.py` & `python_statemachine-2.1.0/statemachine/contrib/diagram.py`

 * *Files identical despite different names*

### Comparing `python_statemachine-2.0.0/statemachine/dispatcher.py` & `python_statemachine-2.1.0/statemachine/dispatcher.py`

 * *Files 16% similar despite different names*

```diff
@@ -33,14 +33,36 @@
     else:
         raise AttrNotFound(
             _("Did not found name '{}' from model or statemachine").format(attr)
         )
     return func, config.obj
 
 
+def _build_attr_wrapper(attr: str, obj):
+    # if `attr` is not callable, then it's an attribute or property,
+    # so `func` contains it's current value.
+    # we'll build a method that get's the fresh value for each call
+    getter = attrgetter(attr)
+
+    def wrapper(*args, **kwargs):
+        return getter(obj)
+
+    return wrapper
+
+
+def _build_sm_event_wrapper(func):
+    "Events already have the 'machine' parameter defined."
+
+    def wrapper(*args, **kwargs):
+        kwargs.pop("machine", None)
+        return func(*args, **kwargs)
+
+    return wrapper
+
+
 def ensure_callable(attr, *objects):
     """Ensure that `attr` is a callable, if not, tries to retrieve one from any of the given
     `objects`.
 
     Args:
         attr (str or callable): A property/method name or a callable.
         objects: A list of objects instances that will serve as lookup for the given attr.
@@ -52,37 +74,28 @@
 
     # Setup configuration if not present to normalize the internal API
     configs = [ObjectConfig.from_obj(obj) for obj in objects]
 
     func, obj = _get_func_by_attr(attr, *configs)
 
     if not callable(func):
-        # if `attr` is not callable, then it's an attribute or property,
-        # so `func` contains it's current value.
-        # we'll build a method that get's the fresh value for each call
-        getter = attrgetter(attr)
-
-        def wrapper(*args, **kwargs):
-            return getter(obj)
-
-        return wrapper
+        return _build_attr_wrapper(attr, obj)
 
     if getattr(func, "_is_sm_event", False):
-        "Events already have the 'machine' parameter defined."
-
-        def wrapper(*args, **kwargs):
-            kwargs.pop("machine")
-            return func(*args, **kwargs)
-
-        return wrapper
+        return _build_sm_event_wrapper(func)
 
     return SignatureAdapter.wrap(func)
 
 
 def resolver_factory(*objects):
     """Factory that returns a configured resolver."""
 
+    objects = [ObjectConfig.from_obj(obj) for obj in objects]
+
     @wraps(ensure_callable)
     def wrapper(attr):
         return ensure_callable(attr, *objects)
 
+    resolver_id = ".".join(str(id(obj.obj)) for obj in objects)
+    wrapper.id = resolver_id
+
     return wrapper
```

### Comparing `python_statemachine-2.0.0/statemachine/event.py` & `python_statemachine-2.1.0/statemachine/event.py`

 * *Files identical despite different names*

### Comparing `python_statemachine-2.0.0/statemachine/event_data.py` & `python_statemachine-2.1.0/statemachine/event_data.py`

 * *Files identical despite different names*

### Comparing `python_statemachine-2.0.0/statemachine/events.py` & `python_statemachine-2.1.0/statemachine/events.py`

 * *Files identical despite different names*

### Comparing `python_statemachine-2.0.0/statemachine/exceptions.py` & `python_statemachine-2.1.0/statemachine/exceptions.py`

 * *Files identical despite different names*

### Comparing `python_statemachine-2.0.0/statemachine/factory.py` & `python_statemachine-2.1.0/statemachine/factory.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,35 +1,49 @@
+from typing import TYPE_CHECKING
+from typing import Any
+from typing import Dict
+from typing import Tuple
 from uuid import uuid4
 
 from . import registry
 from .event import Event
 from .event import trigger_event_factory
 from .exceptions import InvalidDefinition
 from .graph import visit_connected_states
 from .i18n import _
 from .state import State
+from .states import States
 from .transition import Transition
 from .transition_list import TransitionList
 
 
 class StateMachineMetaclass(type):
-    def __init__(cls, name, bases, attrs):
+    def __init__(cls, name: str, bases: Tuple[type], attrs: Dict[str, Any]):
         super().__init__(name, bases, attrs)
         registry.register(cls)
-        cls._abstract = True
         cls.name = cls.__name__
-        cls.states = []
-        cls._events = {}
-        cls.states_map = {}
+        cls.states: States = States()
+        cls.states_map: Dict[Any, State] = {}
+        """Map of ``state.value`` to the corresponding :ref:`state`."""
+
+        cls._abstract = True
+        cls._events: Dict[str, Event] = {}
+
         cls.add_inherited(bases)
         cls.add_from_attributes(attrs)
 
         cls._set_special_states()
         cls._check()
 
+    if TYPE_CHECKING:
+        """Makes mypy happy with dynamic created attributes"""
+
+        def __getattr__(self, attribute: str) -> Any:
+            ...
+
     def _set_special_states(cls):
         if not cls.states:
             return
         initials = [s for s in cls.states if s.initial]
         if len(initials) != 1:
             raise InvalidDefinition(
                 _(
@@ -91,21 +105,27 @@
 
             events = getattr(base, "_events", {})
             for event in events.values():
                 cls.add_event(event.name)
 
     def add_from_attributes(cls, attrs):
         for key, value in sorted(attrs.items(), key=lambda pair: pair[0]):
+            if isinstance(value, States):
+                cls._add_states_from_dict(value)
             if isinstance(value, State):
                 cls.add_state(key, value)
             elif isinstance(value, (Transition, TransitionList)):
                 cls.add_event(key, value)
             elif getattr(value, "_callbacks_to_update", None):
                 cls._add_unbounded_callback(key, value)
 
+    def _add_states_from_dict(cls, states):
+        for state_id, state in states.items():
+            cls.add_state(state_id, state)
+
     def _add_unbounded_callback(cls, attr_name, func):
         if func._is_event:
             # if func is an event, the `attr_name` will be replaced by an event trigger,
             # so we'll also give the ``func`` a new unique name to be used by the callback
             # machinery.
             cls.add_event(attr_name, func._transitions)
             attr_name = f"_{attr_name}_{uuid4().hex}"
@@ -114,14 +134,16 @@
         for ref in func._callbacks_to_update:
             ref(attr_name)
 
     def add_state(cls, id, state: State):
         state._set_id(id)
         cls.states.append(state)
         cls.states_map[state.value] = state
+        if not hasattr(cls, id):
+            setattr(cls, id, state)
 
         # also register all events associated directly with transitions
         for event in state.transitions.unique_events:
             cls.add_event(event)
 
     def add_event(cls, event, transitions=None):
         if transitions is not None:
```

### Comparing `python_statemachine-2.0.0/statemachine/locale/en/LC_MESSAGES/statemachine.po` & `python_statemachine-2.1.0/statemachine/locale/en/LC_MESSAGES/statemachine.po`

 * *Files 7% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 # This file is distributed under the same license as the PROJECT project.
 # Fernando Macedo <fgmacedo@gmail.com>, 2023.
 #
 msgid ""
 msgstr ""
-"Project-Id-Version: 2.0.0\n"
+"Project-Id-Version: 2.1.0\n"
 "Report-Msgid-Bugs-To: fgmacedo@gmail.com\n"
 "POT-Creation-Date: 2023-03-04 16:10-0300\n"
 "PO-Revision-Date: 2023-03-04 16:10-0300\n"
 "Last-Translator: Fernando Macedo <fgmacedo@gmail.com>\n"
 "MIME-Version: 1.0\n"
 "Content-Type: text/plain; charset=utf-8\n"
 "Content-Transfer-Encoding: 8bit\n"
```

### Comparing `python_statemachine-2.0.0/statemachine/locale/pt_BR/LC_MESSAGES/statemachine.mo` & `python_statemachine-2.1.0/statemachine/locale/pt_BR/LC_MESSAGES/statemachine.mo`

 * *Files 0% similar despite different names*

#### msgunfmt {}

```diff
@@ -1,10 +1,10 @@
 msgid ""
 msgstr ""
-"Project-Id-Version:  2.0.0\n"
+"Project-Id-Version:  2.1.0\n"
 "Report-Msgid-Bugs-To: fgmacedo@gmail.com\n"
 "POT-Creation-Date: 2023-03-04 16:10-0300\n"
 "PO-Revision-Date: 2023-03-04 16:10-0300\n"
 "Last-Translator: Fernando Macedo <fgmacedo@gmail.com>\n"
 "Language: pt_BR\n"
 "Language-Team: pt_BR <LL@li.org>\n"
 "Plural-Forms: nplurals=2; plural=(n > 1);\n"
```

### Comparing `python_statemachine-2.0.0/statemachine/locale/pt_BR/LC_MESSAGES/statemachine.po` & `python_statemachine-2.1.0/statemachine/locale/pt_BR/LC_MESSAGES/statemachine.po`

 * *Files 4% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 # This file is distributed under the same license as the PROJECT project.
 # Fernando Macedo <fgmacedo@gmail.com>, 2023.
 #
 msgid ""
 msgstr ""
-"Project-Id-Version: 2.0.0\n"
+"Project-Id-Version: 2.1.0\n"
 "Report-Msgid-Bugs-To: fgmacedo@gmail.com\n"
 "POT-Creation-Date: 2023-03-04 16:10-0300\n"
 "PO-Revision-Date: 2023-03-04 16:10-0300\n"
 "Last-Translator: Fernando Macedo <fgmacedo@gmail.com>\n"
 "MIME-Version: 1.0\n"
 "Content-Type: text/plain; charset=utf-8\n"
 "Content-Transfer-Encoding: 8bit\n"
```

### Comparing `python_statemachine-2.0.0/statemachine/mixins.py` & `python_statemachine-2.1.0/statemachine/mixins.py`

 * *Files identical despite different names*

### Comparing `python_statemachine-2.0.0/statemachine/registry.py` & `python_statemachine-2.1.0/statemachine/registry.py`

 * *Files 8% similar despite different names*

```diff
@@ -22,14 +22,15 @@
 
 def get_machine_cls(name):
     init_registry()
     if "." not in name:
         warnings.warn(
             """Use fully qualified names (<module>.<class>) for state machine mixins.""",
             DeprecationWarning,
+            stacklevel=2,
         )
     return _REGISTRY[name]
 
 
 def init_registry():
     global _initialized
     if not _initialized:
```

### Comparing `python_statemachine-2.0.0/statemachine/signature.py` & `python_statemachine-2.1.0/statemachine/signature.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,8 +1,9 @@
 import itertools
+from functools import partial
 from inspect import BoundArguments
 from inspect import Parameter
 from inspect import Signature
 from typing import Any
 from typing import Callable
 
 
@@ -11,15 +12,17 @@
 
     @classmethod
     def wrap(cls, method):
         """Build a wrapper that adapts the received arguments to the inner ``method`` signature"""
 
         sig = cls.from_callable(method)
         sig.method = method
-        sig.__name__ = method.__name__
+        sig.__name__ = (
+            method.func.__name__ if isinstance(method, partial) else method.__name__
+        )
         return sig
 
     def __call__(self, *args: Any, **kwargs: Any) -> Any:
         ba = self.bind_expected(*args, **kwargs)
         return self.method(*ba.args, **ba.kwargs)
 
     def bind_expected(self, *args: Any, **kwargs: Any) -> BoundArguments:  # noqa: C901
```

### Comparing `python_statemachine-2.0.0/statemachine/state.py` & `python_statemachine-2.1.0/statemachine/state.py`

 * *Files 1% similar despite different names*

```diff
@@ -48,15 +48,15 @@
     >>> closed = State('Closed', final=True)
 
     Transitions are declared using the :func:`State.to` or :func:`State.from_` (reversed) methods.
 
     >>> draft.to(producing)
     TransitionList([Transition(State('Draft', ...
 
-    The result is a `TransitionList`.
+    The result is a :ref:`TransitionList`.
     Don't worry about this internal class.
     But the good thing is that it implements the ``OR`` operator to combine transitions,
     so you can use the ``|`` syntax to compound a list of transitions and assign
     to the same event.
 
     You can declare all transitions for a state in one single line ...
```

### Comparing `python_statemachine-2.0.0/statemachine/statemachine.py` & `python_statemachine-2.1.0/statemachine/statemachine.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,24 +1,24 @@
 from collections import deque
 from typing import TYPE_CHECKING
 from typing import Any
 from typing import Dict  # deprecated since 3.9: https://peps.python.org/pep-0585/
-from typing import List  # deprecated since 3.9: https://peps.python.org/pep-0585/
 
 from .dispatcher import ObjectConfig
 from .dispatcher import resolver_factory
 from .event import Event
 from .event_data import EventData
 from .event_data import TriggerData
 from .exceptions import InvalidDefinition
 from .exceptions import InvalidStateValue
 from .exceptions import TransitionNotAllowed
 from .factory import StateMachineMetaclass
 from .i18n import _
 from .model import Model
+from .states import States
 from .transition import Transition
 
 if TYPE_CHECKING:
     from .state import State
 
 
 class StateMachine(metaclass=StateMachineMetaclass):
@@ -51,21 +51,14 @@
 
         try:
             sm.send("an-inexistent-event")
         except sm.TransitionNotAllowed:
             pass
     """
 
-    _events: Dict[Any, Any] = {}
-    states: List["State"] = []
-    """List of all state machine :ref:`states`."""
-
-    states_map: Dict[Any, "State"] = {}
-    """Map of ``state.value`` to the corresponding :ref:`state`."""
-
     def __init__(
         self,
         model: Any = None,
         state_field: str = "state",
         start_value: Any = None,
         rtc: bool = True,
         allow_event_without_transition: bool = False,
@@ -81,17 +74,23 @@
         assert hasattr(self, "_abstract")
         if self._abstract:
             raise InvalidDefinition(_("There are no states or transitions."))
 
         initial_transition = Transition(
             None, self._get_initial_state(), event="__initial__"
         )
-        self._setup(initial_transition)
+        self._setup(self.states, initial_transition)
         self._activate_initial_state(initial_transition)
 
+    if TYPE_CHECKING:
+        """Makes mypy happy with dynamic created attributes"""
+
+        def __getattr__(self, attribute: str) -> Any:
+            ...
+
     def __repr__(self):
         current_state_id = self.current_state.id if self.current_state_value else None
         return (
             f"{type(self).__name__}(model={self.model!r}, state_field={self.state_field!r}, "
             f"current_state={current_state_id!r})"
         )
 
@@ -137,25 +136,37 @@
 
     def _visit_states_and_transitions(self, visitor):
         for state in self.states:
             visitor(state)
             for transition in state.transitions:
                 visitor(transition)
 
-    def _setup(self, initial_transition):
+    def _setup(self, class_states: States, initial_transition: Transition):
+        """
+        Args:
+            class_states: The original (shared) instances of :ref:`State` living on the
+                user's concrete :ref:`StateMachine` class. These instances cannot be modified.
+                So we will clone the states in order to bind the new instances with concrete
+                actions and event handlers.
+
+            initial_transition: A special :ref:`transition` that triggers the enter on the
+                `initial` :ref:`State`.
+        """
         machine = ObjectConfig(self, skip_attrs=self._get_protected_attrs())
         model = ObjectConfig(self.model, skip_attrs={self.state_field})
         default_resolver = resolver_factory(machine, model)
 
         # clone states and transitions to avoid sharing callbacks references between instances
-        self.states_map = {
-            state.value: state.clone()._setup(self, default_resolver)
-            for state in self.states
+        self.states = States(
+            {s.id: s.clone()._setup(self, default_resolver) for s in class_states}
+        )
+
+        self.states_map: Dict[Any, State] = {
+            state.value: state for state in self.states
         }
-        self.states = list(self.states_map.values())
 
         for state in self.states:
             for transition in state.transitions:
                 transition._setup(self, default_resolver)
 
         initial_transition._setup(self, default_resolver)
         self.add_observer(machine, model)
```

### Comparing `python_statemachine-2.0.0/statemachine/transition.py` & `python_statemachine-2.1.0/statemachine/transition.py`

 * *Files identical despite different names*

### Comparing `python_statemachine-2.0.0/setup.py` & `python_statemachine-2.1.0/setup.py`

 * *Files 8% similar despite different names*

```diff
@@ -6,17 +6,17 @@
 
 package_data = \
 {'': ['*'],
  'statemachine': ['locale/en/LC_MESSAGES/*', 'locale/pt_BR/LC_MESSAGES/*']}
 
 setup_kwargs = {
     'name': 'python-statemachine',
-    'version': '2.0.0',
+    'version': '2.1.0',
     'description': 'Python Finite State Machines made easy.',
-    'long_description': '# Python StateMachine\n\n[![pypi](https://img.shields.io/pypi/v/python-statemachine.svg)](https://pypi.python.org/pypi/python-statemachine)\n[![downloads](https://img.shields.io/pypi/dm/python-statemachine.svg)](https://pypi.python.org/pypi/python-statemachine)\n[![build status](https://github.com/fgmacedo/python-statemachine/actions/workflows/python-package.yml/badge.svg?branch=develop)](https://github.com/fgmacedo/python-statemachine/actions/workflows/python-package.yml?query=branch%3Adevelop)\n[![Coverage report](https://codecov.io/gh/fgmacedo/python-statemachine/branch/develop/graph/badge.svg)](https://codecov.io/gh/fgmacedo/python-statemachine)\n[![Documentation Status](https://readthedocs.org/projects/python-statemachine/badge/?version=latest)](https://python-statemachine.readthedocs.io/en/latest/?badge=latest)\n[![GitHub commits since last release (main)](https://img.shields.io/github/commits-since/fgmacedo/python-statemachine/main/develop)](https://github.com/fgmacedo/python-statemachine/compare/main...develop)\n\n\nPython [finite-state machines](https://en.wikipedia.org/wiki/Finite-state_machine) made easy.\n\n\n* Free software: MIT license\n* Documentation: https://python-statemachine.readthedocs.io.\n\n\nWelcome to python-statemachine, an intuitive and powerful state machine framework designed for a\ngreat developer experience.\n\n🚀 With StateMachine, you can easily create complex, dynamic systems with clean, readable code.\n\n💡 Our framework makes it easy to understand and reason about the different states, events and\ntransitions in your system, so you can focus on building great products.\n\n🔒 python-statemachine also provides robust error handling and ensures that your system stays\nin a valid state at all times.\n\n\nA few reasons why you may consider using it:\n\n* 📈 python-statemachine is designed to help you build scalable,\n  maintainable systems that can handle any complexity.\n* 💪 You can easily create and manage multiple state machines within a single application.\n* 🚫 Prevents common mistakes and ensures that your system stays in a valid state at all times.\n\n\n## Getting started\n\n\nTo install Python State Machine, run this command in your terminal:\n\n    pip install python-statemachine\n\nTo generate diagrams from your machines, you\'ll also need `pydot` and `Graphviz`. You can\ninstall this library already with `pydot` dependency using the `extras` install option. See\nour docs for more details.\n\n    pip install python-statemachine[diagrams]\n\nDefine your state machine:\n\n```py\n>>> from statemachine import StateMachine, State\n\n>>> class TrafficLightMachine(StateMachine):\n...     "A traffic light machine"\n...     green = State(initial=True)\n...     yellow = State()\n...     red = State()\n...\n...     cycle = green.to(yellow) | yellow.to(red) | red.to(green)\n...\n...     slowdown = green.to(yellow)\n...     stop = yellow.to(red)\n...     go = red.to(green)\n...\n...     def before_cycle(self, event: str, source: State, target: State, message: str = ""):\n...         message = ". " + message if message else ""\n...         return f"Running {event} from {source.id} to {target.id}{message}"\n...\n...     def on_enter_red(self):\n...         print("Don\'t move.")\n...\n...     def on_exit_red(self):\n...         print("Go ahead!")\n\n```\n\nYou can now create an instance:\n\n```py\n>>> traffic_light = TrafficLightMachine()\n\n```\n\nThen start sending events:\n\n```py\n>>> traffic_light.cycle()\n\'Running cycle from green to yellow\'\n\n```\n\nYou can inspect the current state:\n\n```py\n>>> traffic_light.current_state.id\n\'yellow\'\n\n```\n\nA `State` human-readable name is automatically derived from the `State.id`:\n\n```py\n>>> traffic_light.current_state.name\n\'Yellow\'\n\n```\n\nOr get a complete state representation for debugging purposes:\n\n```py\n>>> traffic_light.current_state\nState(\'Yellow\', id=\'yellow\', value=\'yellow\', initial=False, final=False)\n\n```\n\nThe ``State`` instance can also be checked by equality:\n\n```py\n>>> traffic_light.current_state == TrafficLightMachine.yellow\nTrue\n\n>>> traffic_light.current_state == traffic_light.yellow\nTrue\n\n```\n\nBut for your convenience, can easily ask if a state is active at any time:\n\n```py\n>>> traffic_light.green.is_active\nFalse\n\n>>> traffic_light.yellow.is_active\nTrue\n\n>>> traffic_light.red.is_active\nFalse\n\n```\n\nEasily iterate over all states:\n\n```py\n>>> [s.id for s in traffic_light.states]\n[\'green\', \'red\', \'yellow\']\n\n```\n\nOr over events:\n\n```py\n>>> [t.name for t in traffic_light.events]\n[\'cycle\', \'go\', \'slowdown\', \'stop\']\n\n```\n\nCall an event by its name:\n\n```py\n>>> traffic_light.cycle()\nDon\'t move.\n\'Running cycle from yellow to red\'\n\n```\nOr send an event with the event name:\n\n```py\n>>> traffic_light.send(\'cycle\')\nGo ahead!\n\'Running cycle from red to green\'\n\n>>> traffic_light.green.is_active\nTrue\n\n```\nYou can\'t run a transition from an invalid state:\n\n```py\n>>> traffic_light.go()\nTraceback (most recent call last):\nstatemachine.exceptions.TransitionNotAllowed: Can\'t go when in Green.\n\n```\nKeeping the same state as expected:\n\n```py\n>>> traffic_light.green.is_active\nTrue\n\n```\n\nAnd you can pass arbitrary positional or keyword arguments to the event, and\nthey will be propagated to all actions and callbacks:\n\n```py\n>>> traffic_light.cycle(message="Please, now slowdown.")\n\'Running cycle from green to yellow. Please, now slowdown.\'\n\n```\n\n## A more useful example\n\nA simple didactic state machine for controlling an `Order`:\n\n```py\n>>> class OrderControl(StateMachine):\n...     waiting_for_payment = State(initial=True)\n...     processing = State()\n...     shipping = State()\n...     completed = State(final=True)\n...\n...     add_to_order = waiting_for_payment.to(waiting_for_payment)\n...     receive_payment = (\n...         waiting_for_payment.to(processing, cond="payments_enough")\n...         | waiting_for_payment.to(waiting_for_payment, unless="payments_enough")\n...     )\n...     process_order = processing.to(shipping, cond="payment_received")\n...     ship_order = shipping.to(completed)\n...\n...     def __init__(self):\n...         self.order_total = 0\n...         self.payments = []\n...         self.payment_received = False\n...         super(OrderControl, self).__init__()\n...\n...     def payments_enough(self, amount):\n...         return sum(self.payments) + amount >= self.order_total\n...\n...     def before_add_to_order(self, amount):\n...         self.order_total += amount\n...         return self.order_total\n...\n...     def before_receive_payment(self, amount):\n...         self.payments.append(amount)\n...         return self.payments\n...\n...     def after_receive_payment(self):\n...         self.payment_received = True\n...\n...     def on_enter_waiting_for_payment(self):\n...         self.payment_received = False\n\n```\n\nYou can use this machine as follows.\n\n```py\n>>> control = OrderControl()\n\n>>> control.add_to_order(3)\n3\n\n>>> control.add_to_order(7)\n10\n\n>>> control.receive_payment(4)\n[4]\n\n>>> control.current_state.id\n\'waiting_for_payment\'\n\n>>> control.current_state.name\n\'Waiting for payment\'\n\n>>> control.process_order()\nTraceback (most recent call last):\n...\nstatemachine.exceptions.TransitionNotAllowed: Can\'t process_order when in Waiting for payment.\n\n>>> control.receive_payment(6)\n[4, 6]\n\n>>> control.current_state.id\n\'processing\'\n\n>>> control.process_order()\n\n>>> control.ship_order()\n\n>>> control.payment_received\nTrue\n\n>>> control.order_total\n10\n\n>>> control.payments\n[4, 6]\n\n>>> control.completed.is_active\nTrue\n\n```\n\nThere\'s a lot more to cover, please take a look at our docs:\nhttps://python-statemachine.readthedocs.io.\n\n\n## Contributing to the project\n\n* <a class="github-button" href="https://github.com/fgmacedo/python-statemachine" data-icon="octicon-star" aria-label="Star fgmacedo/python-statemachine on GitHub">Star this project</a>\n* <a class="github-button" href="https://github.com/fgmacedo/python-statemachine/issues" data-icon="octicon-issue-opened" aria-label="Issue fgmacedo/python-statemachine on GitHub">Open an Issue</a>\n* <a class="github-button" href="https://github.com/fgmacedo/python-statemachine/fork" data-icon="octicon-repo-forked" aria-label="Fork fgmacedo/python-statemachine on GitHub">Fork</a>\n\n- If you found this project helpful, please consider giving it a star on GitHub.\n\n- **Contribute code**: If you would like to contribute code to this project, please submit a pull\nrequest. For more information on how to contribute, please see our [contributing.md]contributing.md) file.\n\n- **Report bugs**: If you find any bugs in this project, please report them by opening an issue\n  on our GitHub issue tracker.\n\n- **Suggest features**: If you have a great idea for a new feature, please let us know by opening\n  an issue on our GitHub issue tracker.\n\n- **Documentation**: Help improve this project\'s documentation by submitting pull requests.\n\n- **Promote the project**: Help spread the word about this project by sharing it on social media,\n  writing a blog post, or giving a talk about it. Tag me on Twitter\n  [@fgmacedo](https://twitter.com/fgmacedo) so I can share it too!\n',
+    'long_description': '# Python StateMachine\n\n[![pypi](https://img.shields.io/pypi/v/python-statemachine.svg)](https://pypi.python.org/pypi/python-statemachine)\n[![downloads](https://img.shields.io/pypi/dm/python-statemachine.svg)](https://pypi.python.org/pypi/python-statemachine)\n[![build status](https://github.com/fgmacedo/python-statemachine/actions/workflows/python-package.yml/badge.svg?branch=develop)](https://github.com/fgmacedo/python-statemachine/actions/workflows/python-package.yml?query=branch%3Adevelop)\n[![Coverage report](https://codecov.io/gh/fgmacedo/python-statemachine/branch/develop/graph/badge.svg)](https://codecov.io/gh/fgmacedo/python-statemachine)\n[![Documentation Status](https://readthedocs.org/projects/python-statemachine/badge/?version=latest)](https://python-statemachine.readthedocs.io/en/latest/?badge=latest)\n[![GitHub commits since last release (main)](https://img.shields.io/github/commits-since/fgmacedo/python-statemachine/main/develop)](https://github.com/fgmacedo/python-statemachine/compare/main...develop)\n\n\nPython [finite-state machines](https://en.wikipedia.org/wiki/Finite-state_machine) made easy.\n\n\n* Free software: MIT license\n* Documentation: https://python-statemachine.readthedocs.io.\n\n\nWelcome to python-statemachine, an intuitive and powerful state machine framework designed for a\ngreat developer experience.\n\n🚀 With StateMachine, you can easily create complex, dynamic systems with clean, readable code.\n\n💡 Our framework makes it easy to understand and reason about the different states, events and\ntransitions in your system, so you can focus on building great products.\n\n🔒 python-statemachine also provides robust error handling and ensures that your system stays\nin a valid state at all times.\n\n\nA few reasons why you may consider using it:\n\n* 📈 python-statemachine is designed to help you build scalable,\n  maintainable systems that can handle any complexity.\n* 💪 You can easily create and manage multiple state machines within a single application.\n* 🚫 Prevents common mistakes and ensures that your system stays in a valid state at all times.\n\n\n## Getting started\n\n\nTo install Python State Machine, run this command in your terminal:\n\n    pip install python-statemachine\n\nTo generate diagrams from your machines, you\'ll also need `pydot` and `Graphviz`. You can\ninstall this library already with `pydot` dependency using the `extras` install option. See\nour docs for more details.\n\n    pip install python-statemachine[diagrams]\n\nDefine your state machine:\n\n```py\n>>> from statemachine import StateMachine, State\n\n>>> class TrafficLightMachine(StateMachine):\n...     "A traffic light machine"\n...     green = State(initial=True)\n...     yellow = State()\n...     red = State()\n...\n...     cycle = (\n...         green.to(yellow)\n...         | yellow.to(red)\n...         | red.to(green)\n...     )\n...\n...     def before_cycle(self, event: str, source: State, target: State, message: str = ""):\n...         message = ". " + message if message else ""\n...         return f"Running {event} from {source.id} to {target.id}{message}"\n...\n...     def on_enter_red(self):\n...         print("Don\'t move.")\n...\n...     def on_exit_red(self):\n...         print("Go ahead!")\n\n```\n\nYou can now create an instance:\n\n```py\n>>> sm = TrafficLightMachine()\n\n```\n\nThis state machine can be represented graphically as follows:\n\n```py\n>>> img_path = "docs/images/readme_trafficlightmachine.png"\n>>> sm._graph().write_png(img_path)\n\n```\n\n![](https://raw.githubusercontent.com/fgmacedo/python-statemachine/develop/docs/images/readme_trafficlightmachine.png)\n\n\nWhere on the `TrafficLightMachine`, we\'ve defined `green`, `yellow`, and `red` as states, and\none event called `cycle`, which is bound to the transitions from `green` to `yellow`, `yellow` to `red`,\nand `red` to `green`. We also have defined three callbacks by name convention, `before_cycle`, `on_enter_red`, and `on_exit_red`.\n\n\nThen start sending events to your new state machine:\n\n```py\n>>> sm.send("cycle")\n\'Running cycle from green to yellow\'\n\n```\n\nThat\'s it. This is all an external object needs to know about your state machine: How to send events.\nIdeally, all states, transitions, and actions should be kept internally and not checked externally to avoid unnecessary coupling.\n\nBut if your use case needs, you can inspect state machine properties, like the current state:\n\n```py\n>>> sm.current_state.id\n\'yellow\'\n\n```\n\nOr get a complete state representation for debugging purposes:\n\n```py\n>>> sm.current_state\nState(\'Yellow\', id=\'yellow\', value=\'yellow\', initial=False, final=False)\n\n```\n\nThe `State` instance can also be checked by equality:\n\n```py\n>>> sm.current_state == TrafficLightMachine.yellow\nTrue\n\n>>> sm.current_state == sm.yellow\nTrue\n\n```\n\nOr you can check if a state is active at any time:\n\n```py\n>>> sm.green.is_active\nFalse\n\n>>> sm.yellow.is_active\nTrue\n\n>>> sm.red.is_active\nFalse\n\n```\n\nEasily iterate over all states:\n\n```py\n>>> [s.id for s in sm.states]\n[\'green\', \'red\', \'yellow\']\n\n```\n\nOr over events:\n\n```py\n>>> [t.name for t in sm.events]\n[\'cycle\']\n\n```\n\nCall an event by its name:\n\n```py\n>>> sm.cycle()\nDon\'t move.\n\'Running cycle from yellow to red\'\n\n```\nOr send an event with the event name:\n\n```py\n>>> sm.send(\'cycle\')\nGo ahead!\n\'Running cycle from red to green\'\n\n>>> sm.green.is_active\nTrue\n\n```\n\nYou can pass arbitrary positional or keyword arguments to the event, and\nthey will be propagated to all actions and callbacks using something similar to dependency injection. In other words, the library will only inject the parameters declared on the\ncallback method.\n\nNote how `before_cycle` was declared:\n\n```py\ndef before_cycle(self, event: str, source: State, target: State, message: str = ""):\n    message = ". " + message if message else ""\n    return f"Running {event} from {source.id} to {target.id}{message}"\n```\n\nThe params `event`, `source`, `target` (and others) are available built-in to be used on any action.\nThe param `message` is user-defined, in our example we made it default empty so we can call `cycle` with\nor without a `message` parameter.\n\nIf we pass a `message` parameter, it will be used on the `before_cycle` action:\n\n```py\n>>> sm.send("cycle", message="Please, now slowdown.")\n\'Running cycle from green to yellow. Please, now slowdown.\'\n\n```\n\n\nBy default, events with transitions that cannot run from the current state or unknown events\nraise a `TransitionNotAllowed` exception:\n\n```py\n>>> sm.send("go")\nTraceback (most recent call last):\nstatemachine.exceptions.TransitionNotAllowed: Can\'t go when in Yellow.\n\n```\n\nKeeping the same state as expected:\n\n```py\n>>> sm.yellow.is_active\nTrue\n\n```\n\nA human-readable name is automatically derived from the `State.id`, which is used on the messages\nand in diagrams:\n\n```py\n>>> sm.current_state.name\n\'Yellow\'\n\n```\n\n## A more useful example\n\nA simple didactic state machine for controlling an `Order`:\n\n```py\n>>> class OrderControl(StateMachine):\n...     waiting_for_payment = State(initial=True)\n...     processing = State()\n...     shipping = State()\n...     completed = State(final=True)\n...\n...     add_to_order = waiting_for_payment.to(waiting_for_payment)\n...     receive_payment = (\n...         waiting_for_payment.to(processing, cond="payments_enough")\n...         | waiting_for_payment.to(waiting_for_payment, unless="payments_enough")\n...     )\n...     process_order = processing.to(shipping, cond="payment_received")\n...     ship_order = shipping.to(completed)\n...\n...     def __init__(self):\n...         self.order_total = 0\n...         self.payments = []\n...         self.payment_received = False\n...         super(OrderControl, self).__init__()\n...\n...     def payments_enough(self, amount):\n...         return sum(self.payments) + amount >= self.order_total\n...\n...     def before_add_to_order(self, amount):\n...         self.order_total += amount\n...         return self.order_total\n...\n...     def before_receive_payment(self, amount):\n...         self.payments.append(amount)\n...         return self.payments\n...\n...     def after_receive_payment(self):\n...         self.payment_received = True\n...\n...     def on_enter_waiting_for_payment(self):\n...         self.payment_received = False\n\n```\n\nYou can use this machine as follows.\n\n```py\n>>> control = OrderControl()\n\n>>> control.add_to_order(3)\n3\n\n>>> control.add_to_order(7)\n10\n\n>>> control.receive_payment(4)\n[4]\n\n>>> control.current_state.id\n\'waiting_for_payment\'\n\n>>> control.current_state.name\n\'Waiting for payment\'\n\n>>> control.process_order()\nTraceback (most recent call last):\n...\nstatemachine.exceptions.TransitionNotAllowed: Can\'t process_order when in Waiting for payment.\n\n>>> control.receive_payment(6)\n[4, 6]\n\n>>> control.current_state.id\n\'processing\'\n\n>>> control.process_order()\n\n>>> control.ship_order()\n\n>>> control.payment_received\nTrue\n\n>>> control.order_total\n10\n\n>>> control.payments\n[4, 6]\n\n>>> control.completed.is_active\nTrue\n\n```\n\nThere\'s a lot more to cover, please take a look at our docs:\nhttps://python-statemachine.readthedocs.io.\n\n\n## Contributing to the project\n\n* <a class="github-button" href="https://github.com/fgmacedo/python-statemachine" data-icon="octicon-star" aria-label="Star fgmacedo/python-statemachine on GitHub">Star this project</a>\n* <a class="github-button" href="https://github.com/fgmacedo/python-statemachine/issues" data-icon="octicon-issue-opened" aria-label="Issue fgmacedo/python-statemachine on GitHub">Open an Issue</a>\n* <a class="github-button" href="https://github.com/fgmacedo/python-statemachine/fork" data-icon="octicon-repo-forked" aria-label="Fork fgmacedo/python-statemachine on GitHub">Fork</a>\n\n- If you found this project helpful, please consider giving it a star on GitHub.\n\n- **Contribute code**: If you would like to contribute code to this project, please submit a pull\nrequest. For more information on how to contribute, please see our [contributing.md]contributing.md) file.\n\n- **Report bugs**: If you find any bugs in this project, please report them by opening an issue\n  on our GitHub issue tracker.\n\n- **Suggest features**: If you have a great idea for a new feature, please let us know by opening\n  an issue on our GitHub issue tracker.\n\n- **Documentation**: Help improve this project\'s documentation by submitting pull requests.\n\n- **Promote the project**: Help spread the word about this project by sharing it on social media,\n  writing a blog post, or giving a talk about it. Tag me on Twitter\n  [@fgmacedo](https://twitter.com/fgmacedo) so I can share it too!\n',
     'author': 'Fernando Macedo',
     'author_email': 'fgmacedo@gmail.com',
     'maintainer': 'Fernando Macedo',
     'maintainer_email': 'fgmacedo@gmail.com',
     'url': 'https://github.com/fgmacedo/python-statemachine',
     'packages': packages,
     'package_data': package_data,
```

### Comparing `python_statemachine-2.0.0/PKG-INFO` & `python_statemachine-2.1.0/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: python-statemachine
-Version: 2.0.0
+Version: 2.1.0
 Summary: Python Finite State Machines made easy.
 Home-page: https://github.com/fgmacedo/python-statemachine
 License: MIT
 Author: Fernando Macedo
 Author-email: fgmacedo@gmail.com
 Maintainer: Fernando Macedo
 Maintainer-email: fgmacedo@gmail.com
@@ -84,19 +84,19 @@
 
 >>> class TrafficLightMachine(StateMachine):
 ...     "A traffic light machine"
 ...     green = State(initial=True)
 ...     yellow = State()
 ...     red = State()
 ...
-...     cycle = green.to(yellow) | yellow.to(red) | red.to(green)
-...
-...     slowdown = green.to(yellow)
-...     stop = yellow.to(red)
-...     go = red.to(green)
+...     cycle = (
+...         green.to(yellow)
+...         | yellow.to(red)
+...         | red.to(green)
+...     )
 ...
 ...     def before_cycle(self, event: str, source: State, target: State, message: str = ""):
 ...         message = ". " + message if message else ""
 ...         return f"Running {event} from {source.id} to {target.id}{message}"
 ...
 ...     def on_enter_red(self):
 ...         print("Don't move.")
@@ -105,132 +105,171 @@
 ...         print("Go ahead!")
 
 ```
 
 You can now create an instance:
 
 ```py
->>> traffic_light = TrafficLightMachine()
+>>> sm = TrafficLightMachine()
 
 ```
 
-Then start sending events:
+This state machine can be represented graphically as follows:
 
 ```py
->>> traffic_light.cycle()
-'Running cycle from green to yellow'
+>>> img_path = "docs/images/readme_trafficlightmachine.png"
+>>> sm._graph().write_png(img_path)
 
 ```
 
-You can inspect the current state:
+![](https://raw.githubusercontent.com/fgmacedo/python-statemachine/develop/docs/images/readme_trafficlightmachine.png)
+
+
+Where on the `TrafficLightMachine`, we've defined `green`, `yellow`, and `red` as states, and
+one event called `cycle`, which is bound to the transitions from `green` to `yellow`, `yellow` to `red`,
+and `red` to `green`. We also have defined three callbacks by name convention, `before_cycle`, `on_enter_red`, and `on_exit_red`.
+
+
+Then start sending events to your new state machine:
 
 ```py
->>> traffic_light.current_state.id
-'yellow'
+>>> sm.send("cycle")
+'Running cycle from green to yellow'
 
 ```
 
-A `State` human-readable name is automatically derived from the `State.id`:
+That's it. This is all an external object needs to know about your state machine: How to send events.
+Ideally, all states, transitions, and actions should be kept internally and not checked externally to avoid unnecessary coupling.
+
+But if your use case needs, you can inspect state machine properties, like the current state:
 
 ```py
->>> traffic_light.current_state.name
-'Yellow'
+>>> sm.current_state.id
+'yellow'
 
 ```
 
 Or get a complete state representation for debugging purposes:
 
 ```py
->>> traffic_light.current_state
+>>> sm.current_state
 State('Yellow', id='yellow', value='yellow', initial=False, final=False)
 
 ```
 
-The ``State`` instance can also be checked by equality:
+The `State` instance can also be checked by equality:
 
 ```py
->>> traffic_light.current_state == TrafficLightMachine.yellow
+>>> sm.current_state == TrafficLightMachine.yellow
 True
 
->>> traffic_light.current_state == traffic_light.yellow
+>>> sm.current_state == sm.yellow
 True
 
 ```
 
-But for your convenience, can easily ask if a state is active at any time:
+Or you can check if a state is active at any time:
 
 ```py
->>> traffic_light.green.is_active
+>>> sm.green.is_active
 False
 
->>> traffic_light.yellow.is_active
+>>> sm.yellow.is_active
 True
 
->>> traffic_light.red.is_active
+>>> sm.red.is_active
 False
 
 ```
 
 Easily iterate over all states:
 
 ```py
->>> [s.id for s in traffic_light.states]
+>>> [s.id for s in sm.states]
 ['green', 'red', 'yellow']
 
 ```
 
 Or over events:
 
 ```py
->>> [t.name for t in traffic_light.events]
-['cycle', 'go', 'slowdown', 'stop']
+>>> [t.name for t in sm.events]
+['cycle']
 
 ```
 
 Call an event by its name:
 
 ```py
->>> traffic_light.cycle()
+>>> sm.cycle()
 Don't move.
 'Running cycle from yellow to red'
 
 ```
 Or send an event with the event name:
 
 ```py
->>> traffic_light.send('cycle')
+>>> sm.send('cycle')
 Go ahead!
 'Running cycle from red to green'
 
->>> traffic_light.green.is_active
+>>> sm.green.is_active
 True
 
 ```
-You can't run a transition from an invalid state:
+
+You can pass arbitrary positional or keyword arguments to the event, and
+they will be propagated to all actions and callbacks using something similar to dependency injection. In other words, the library will only inject the parameters declared on the
+callback method.
+
+Note how `before_cycle` was declared:
+
+```py
+def before_cycle(self, event: str, source: State, target: State, message: str = ""):
+    message = ". " + message if message else ""
+    return f"Running {event} from {source.id} to {target.id}{message}"
+```
+
+The params `event`, `source`, `target` (and others) are available built-in to be used on any action.
+The param `message` is user-defined, in our example we made it default empty so we can call `cycle` with
+or without a `message` parameter.
+
+If we pass a `message` parameter, it will be used on the `before_cycle` action:
+
+```py
+>>> sm.send("cycle", message="Please, now slowdown.")
+'Running cycle from green to yellow. Please, now slowdown.'
+
+```
+
+
+By default, events with transitions that cannot run from the current state or unknown events
+raise a `TransitionNotAllowed` exception:
 
 ```py
->>> traffic_light.go()
+>>> sm.send("go")
 Traceback (most recent call last):
-statemachine.exceptions.TransitionNotAllowed: Can't go when in Green.
+statemachine.exceptions.TransitionNotAllowed: Can't go when in Yellow.
 
 ```
+
 Keeping the same state as expected:
 
 ```py
->>> traffic_light.green.is_active
+>>> sm.yellow.is_active
 True
 
 ```
 
-And you can pass arbitrary positional or keyword arguments to the event, and
-they will be propagated to all actions and callbacks:
+A human-readable name is automatically derived from the `State.id`, which is used on the messages
+and in diagrams:
 
 ```py
->>> traffic_light.cycle(message="Please, now slowdown.")
-'Running cycle from green to yellow. Please, now slowdown.'
+>>> sm.current_state.name
+'Yellow'
 
 ```
 
 ## A more useful example
 
 A simple didactic state machine for controlling an `Order`:
```

