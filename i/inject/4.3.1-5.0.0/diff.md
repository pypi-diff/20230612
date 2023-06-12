# Comparing `tmp/Inject-4.3.1.tar.gz` & `tmp/inject-5.0.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/Inject-4.3.1.tar", last modified: Mon Aug 17 17:52:23 2020, max compression
+gzip compressed data, last modified: Sun Feb  2 00:00:00 2020, max compression
```

## Comparing `Inject-4.3.1.tar` & `inject-5.0.0.tar`

### file list

```diff
@@ -1,27 +1,27 @@
-drwxr-xr-x   0 ivan       (501) staff       (20)        0 2020-08-17 17:52:23.000000 Inject-4.3.1/
--rw-r--r--   0 ivan       (501) staff       (20)     2434 2020-08-17 17:51:27.000000 Inject-4.3.1/CHANGES.md
-drwxr-xr-x   0 ivan       (501) staff       (20)        0 2020-08-17 17:52:23.000000 Inject-4.3.1/Inject.egg-info/
--rw-r--r--   0 ivan       (501) staff       (20)    11002 2020-08-17 17:52:23.000000 Inject-4.3.1/Inject.egg-info/PKG-INFO
--rw-r--r--   0 ivan       (501) staff       (20)      436 2020-08-17 17:52:23.000000 Inject-4.3.1/Inject.egg-info/SOURCES.txt
--rw-r--r--   0 ivan       (501) staff       (20)        1 2020-08-17 17:52:23.000000 Inject-4.3.1/Inject.egg-info/dependency_links.txt
--rw-r--r--   0 ivan       (501) staff       (20)        1 2019-07-30 08:30:56.000000 Inject-4.3.1/Inject.egg-info/not-zip-safe
--rw-r--r--   0 ivan       (501) staff       (20)        7 2020-08-17 17:52:23.000000 Inject-4.3.1/Inject.egg-info/top_level.txt
--rw-r--r--   0 ivan       (501) staff       (20)    11358 2017-09-12 16:25:21.000000 Inject-4.3.1/LICENSE
--rw-r--r--   0 ivan       (501) staff       (20)       93 2020-04-13 18:08:54.000000 Inject-4.3.1/MANIFEST.in
--rw-r--r--   0 ivan       (501) staff       (20)    11002 2020-08-17 17:52:23.000000 Inject-4.3.1/PKG-INFO
--rw-r--r--   0 ivan       (501) staff       (20)     7988 2020-08-11 09:09:40.000000 Inject-4.3.1/README.md
-drwxr-xr-x   0 ivan       (501) staff       (20)        0 2020-08-17 17:52:23.000000 Inject-4.3.1/inject/
--rw-r--r--   0 ivan       (501) staff       (20)    16293 2020-08-17 17:50:26.000000 Inject-4.3.1/inject/__init__.py
--rw-r--r--   0 ivan       (501) staff       (20)        0 2019-11-25 08:44:08.000000 Inject-4.3.1/inject/py.typed
--rw-r--r--   0 ivan       (501) staff       (20)       38 2020-08-17 17:52:23.000000 Inject-4.3.1/setup.cfg
--rw-r--r--   0 ivan       (501) staff       (20)     1109 2020-08-17 17:50:33.000000 Inject-4.3.1/setup.py
-drwxr-xr-x   0 ivan       (501) staff       (20)        0 2020-08-17 17:52:23.000000 Inject-4.3.1/test/
--rw-r--r--   0 ivan       (501) staff       (20)      662 2019-07-30 08:28:43.000000 Inject-4.3.1/test/test_attr.py
--rw-r--r--   0 ivan       (501) staff       (20)     6283 2020-05-13 11:44:20.000000 Inject-4.3.1/test/test_autoparams.py
--rw-r--r--   0 ivan       (501) staff       (20)     1528 2020-08-17 17:49:26.000000 Inject-4.3.1/test/test_binder.py
--rw-r--r--   0 ivan       (501) staff       (20)     3590 2020-08-11 09:09:40.000000 Inject-4.3.1/test/test_functional.py
--rw-r--r--   0 ivan       (501) staff       (20)     2090 2020-08-17 17:49:26.000000 Inject-4.3.1/test/test_inject_configuration.py
--rw-r--r--   0 ivan       (501) staff       (20)     1832 2020-05-13 11:29:26.000000 Inject-4.3.1/test/test_injector.py
--rw-r--r--   0 ivan       (501) staff       (20)      253 2019-07-30 08:28:43.000000 Inject-4.3.1/test/test_instance.py
--rw-r--r--   0 ivan       (501) staff       (20)      900 2020-08-11 09:09:40.000000 Inject-4.3.1/test/test_param.py
--rw-r--r--   0 ivan       (501) staff       (20)     5200 2020-08-11 09:09:40.000000 Inject-4.3.1/test/test_params.py
+-rw-r--r--   0        0        0      311 2020-02-02 00:00:00.000000 inject-5.0.0/.travis.yml
+-rw-r--r--   0        0        0     2498 2020-02-02 00:00:00.000000 inject-5.0.0/CHANGES.md
+-rw-r--r--   0        0        0       93 2020-02-02 00:00:00.000000 inject-5.0.0/MANIFEST.in
+-rw-r--r--   0        0        0     1189 2020-02-02 00:00:00.000000 inject-5.0.0/makefile
+-rw-r--r--   0        0        0      111 2020-02-02 00:00:00.000000 inject-5.0.0/.env/pyvenv.cfg
+-rw-r--r--   0        0        0    17679 2020-02-02 00:00:00.000000 inject-5.0.0/.env/man/man1/nosetests.1
+-rw-r--r--   0        0        0    17166 2020-02-02 00:00:00.000000 inject-5.0.0/src/inject/__init__.py
+-rw-r--r--   0        0        0      160 2020-02-02 00:00:00.000000 inject-5.0.0/src/inject/_version.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 inject-5.0.0/src/inject/py.typed
+-rw-r--r--   0        0        0      270 2020-02-02 00:00:00.000000 inject-5.0.0/test/__init__.py
+-rw-r--r--   0        0        0     1002 2020-02-02 00:00:00.000000 inject-5.0.0/test/test_attr.py
+-rw-r--r--   0        0        0     7302 2020-02-02 00:00:00.000000 inject-5.0.0/test/test_autoparams.py
+-rw-r--r--   0        0        0     1528 2020-02-02 00:00:00.000000 inject-5.0.0/test/test_binder.py
+-rw-r--r--   0        0        0     3590 2020-02-02 00:00:00.000000 inject-5.0.0/test/test_functional.py
+-rw-r--r--   0        0        0     2090 2020-02-02 00:00:00.000000 inject-5.0.0/test/test_inject_configuration.py
+-rw-r--r--   0        0        0     1832 2020-02-02 00:00:00.000000 inject-5.0.0/test/test_injector.py
+-rw-r--r--   0        0        0      253 2020-02-02 00:00:00.000000 inject-5.0.0/test/test_instance.py
+-rw-r--r--   0        0        0      900 2020-02-02 00:00:00.000000 inject-5.0.0/test/test_param.py
+-rw-r--r--   0        0        0     5200 2020-02-02 00:00:00.000000 inject-5.0.0/test/test_params.py
+-rw-r--r--   0        0        0     1030 2020-02-02 00:00:00.000000 inject-5.0.0/test37/test_dataclass.py
+-rw-r--r--   0        0        0      689 2020-02-02 00:00:00.000000 inject-5.0.0/test37/test_future.py
+-rw-r--r--   0        0        0     2817 2020-02-02 00:00:00.000000 inject-5.0.0/typeshed/pyi/inject/__init__.pyi
+-rw-r--r--   0        0        0      691 2020-02-02 00:00:00.000000 inject-5.0.0/.gitignore
+-rw-r--r--   0        0        0    11358 2020-02-02 00:00:00.000000 inject-5.0.0/LICENSE
+-rw-r--r--   0        0        0     8022 2020-02-02 00:00:00.000000 inject-5.0.0/README.md
+-rw-r--r--   0        0        0     3930 2020-02-02 00:00:00.000000 inject-5.0.0/pyproject.toml
+-rw-r--r--   0        0        0     9023 2020-02-02 00:00:00.000000 inject-5.0.0/PKG-INFO
```

### filetype from file(1)

```diff
@@ -1 +1 @@
-POSIX tar archive (GNU)
+POSIX tar archive
```

### Comparing `Inject-4.3.1/CHANGES.md` & `inject-5.0.0/CHANGES.md`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,13 @@
 python-inject changes
 =====================
 
+### 5.0.0 (2023-06-10)
+- Support for PEP0604 for Python>=3.10.
+
 ### 4.3.1 (2020-08-17)
 - Use assertRaisesRegex instead of assertRaisesRegexp to fix deprecation warnings.
 
 ### 4.3.0 (2020-08-11)
 - Support for classes in autoparams, #59.
 - Support for asyncio, #66.
```

### Comparing `Inject-4.3.1/Inject.egg-info/PKG-INFO` & `inject-5.0.0/PKG-INFO`

 * *Files 27% similar despite different names*

```diff
@@ -1,298 +1,302 @@
 Metadata-Version: 2.1
-Name: Inject
-Version: 4.3.1
-Summary: Python dependency injection framework
-Home-page: https://github.com/ivankorobkov/python-inject
-Author: Ivan Korobkov
-Author-email: ivan.korobkov@gmail.com
-License: Apache License 2.0
-Description: # python-inject [![Build Status](https://travis-ci.org/ivankorobkov/python-inject.svg?branch=master)](https://travis-ci.org/ivankorobkov/python-inject)
-        Dependency injection the python way, the good way. Not a port of Guice or Spring.
-        
-        ## Key features
-        * Fast.
-        * Thread-safe.
-        * Simple to use.
-        * Does not steal class constructors.
-        * Does not try to manage your application object graph.
-        * Transparently integrates into tests.
-        * Supports Python 3.5+ (`v4.*`) and Python 2.7–3.5 (`v3.*`).
-        * Supports type hinting in Python 3.5+.
-        * Autoparams leveraging type annotations.
-        
-        ## Python Support
-        
-        | Python | Inject Version |
-        |--------|----------------|
-        | 3.6+   | 4.1+           |
-        | 3.5    | 4.0            |
-        | < 3.5  | 3.*            |
-        
-        
-        ## Installation
-        Use pip to install the lastest version:
-        
-        ```bash
-        pip install inject
-        ```
-        
-        ## Autoparams example
-        `@inject.autoparams` returns a decorator which automatically injects arguments into a function 
-        that uses type annotations. This is supported only in Python >= 3.5.
-        
-        ```python
-        @inject.autoparams()
-        def refresh_cache(cache: RedisCache, db: DbInterface):
-            pass
-        ```
-        
-        There is an option to specify which arguments we want to inject without attempts of 
-        injecting everything:
-        
-        ```python
-        @inject.autoparams('cache', 'db')
-        def sign_up(name, email, cache: RedisCache, db: DbInterface):
-            pass
-        ```
-        
-        ## Step-by-step example
-        ```python
-        # Import the inject module.
-        import inject
-        
-        
-        # `inject.instance` requests dependencies from the injector.
-        def foo(bar):
-            cache = inject.instance(Cache)
-            cache.save('bar', bar)
-        
-        
-        # `inject.params` injects dependencies as keyword arguments or positional argument. 
-        # Also you can use @inject.autoparams in Python 3.5, see the example above.
-        @inject.params(cache=Cache, user=CurrentUser)
-        def baz(foo, cache=None, user=None):
-            cache.save('foo', foo, user)
-        
-        # this can be called in different ways:
-        # with injected arguments
-        baz('foo')
-        
-        # with positional arguments
-        baz('foo', my_cache)
-        
-        # with keyword arguments
-        baz('foo', my_cache, user=current_user)
-        
-        
-        # `inject.param` is deprecated, use `inject.params` instead.
-        @inject.param('cache', Cache)
-        def bar(foo, cache=None):
-            cache.save('foo', foo)
-        
-        
-        # `inject.attr` creates properties (descriptors) which request dependencies on access.
-        class User(object):
-            cache = inject.attr(Cache)
-                    
-            def __init__(self, id):
-                self.id = id
-        
-            def save(self):
-                self.cache.save('users', self)
-            
-            @classmethod
-            def load(cls, id):
-                return cls.cache.load('users', id)
-        
-        
-        # Create an optional configuration.
-        def my_config(binder):
-            binder.install(my_config2)  # Add bindings from another config.
-            binder.bind(Cache, RedisCache('localhost:1234'))
-        
-        # Configure a shared injector.
-        inject.configure(my_config)
-        
-        
-        # Instantiate User as a normal class. Its `cache` dependency is injected when accessed.
-        user = User(10)
-        user.save()
-        
-        # Call the functions, the dependencies are automatically injected.
-        foo('Hello')
-        bar('world')
-        ```
-        
-        
-        ## Usage with Django
-        Django can load some modules multiple times which can lead to 
-        `InjectorException: Injector is already configured`. You can use `configure_once` which
-        is guaranteed to run only once when the injector is absent:
-        ```python
-        import inject
-        inject.configure_once(my_config)
-        ```
-        
-        ## Testing
-        In tests use `inject.clear_and_configure(callable)` to create a new injector on setup,
-        and optionally `inject.clear()` to clean up on tear down:
-        ```python
-        class MyTest(unittest.TestCase):
-            def setUp(self):
-                inject.clear_and_configure(lambda binder: binder
-                    .bind(Cache, Mock()) \
-                    .bind(Validator, TestValidator()))
-            
-            def tearDown(self):
-                inject.clear()
-        ```
-        
-        ## Thread-safety
-        After configuration the injector is thread-safe and can be safely reused by multiple threads.
-        
-        ## Binding types
-        **Instance** bindings always return the same instance:
-        
-        ```python
-        redis = RedisCache(address='localhost:1234')
-        def config(binder):
-            binder.bind(Cache, redis)
-        ```
-            
-        **Constructor** bindings create a singleton on injection:
-        
-        ```python
-        def config(binder):
-            # Creates a redis cache singleton on first injection.
-            binder.bind_to_constructor(Cache, lambda: RedisCache(address='localhost:1234'))
-        ```
-        
-        **Provider** bindings call the provider on injection:
-        
-        ```python
-        def get_my_thread_local_cache():
-            pass
-        
-        def config(binder):
-            # Executes the provider on each injection.
-            binder.bind_to_provider(Cache, get_my_thread_local_cache) 
-        ```
-        
-        **Runtime** bindings automatically create singletons on injection, require no configuration.
-        For example, only the `Config` class binding is present, other bindings are runtime:
-        
-        ```python
-        class Config(object):
-            pass
-        
-        class Cache(object):
-            config = inject.attr(Config)
-        
-        class Db(object):
-            config = inject.attr(Config)
-        
-        class User(object):
-            cache = inject.attr(Cache)
-            db = inject.attr(Db)
-            
-            @classmethod
-            def load(cls, user_id):
-                return cls.cache.load('users', user_id) or cls.db.load('users', user_id)
-            
-        inject.configure(lambda binder: binder.bind(Config, load_config_file()))
-        user = User.load(10)
-        ```
-        ## Disabling runtime binding
-        Sometimes runtime binding leads to unexpected behaviour.  Say if you forget
-        to bind an instance to a class, `inject` will try to implicitly instantiate it.
-        
-        If an instance is unintentionally created with default arguments it may lead to
-        hard-to-debug bugs.  To disable runtime binding and make sure that only 
-        explicitly bound instances are injected, pass `bind_in_runtime=False` 
-        to `inject.configure`, `inject.configure_once` or `inject.clear_and_configure`.
-        
-        In this case `inject` immediately raises `InjectorException` when the code
-        tries to get an unbound instance.
-        
-        ## Keys
-        It is possible to use any hashable object as a binding key. For example:
-        
-        ```python
-        import inject
-        
-        inject.configure(lambda binder: \
-            binder.bind('host', 'localhost') \
-            binder.bind('port', 1234))
-        ```
-        
-        ## Why no scopes?
-        I've used Guice and Spring in Java for a lot of years, and I don't like their scopes.
-        `python-inject` by default creates objects as singletons. It does not need a prototype scope
-        as in Spring or NO_SCOPE as in Guice because `python-inject` does not steal your class 
-        constructors. Create instances the way you like and then inject dependencies into them.
-        
-        Other scopes such as a request scope or a session scope are fragile, introduce high coupling,
-        and are difficult to test. In `python-inject` write custom providers which can be thread-local, 
-        request-local, etc.
-        
-        For example, a thread-local current user provider:
-        
-        ```python
-        import inject
-        import threading
-        
-        # Given a user class.
-        class User(object):
-            pass
-        
-        # Create a thread-local current user storage.
-        _LOCAL = threading.local()
-        
-        def get_current_user():
-            return getattr(_LOCAL, 'user', None)
-        
-        def set_current_user(user):
-            _LOCAL.user = user
-        
-        # Bind User to a custom provider.
-        inject.configure(lambda binder: binder.bind_to_provider(User, get_current_user))
-        
-        # Inject the current user.
-        @inject.params(user=User)
-        def foo(user):
-            pass
-        ```
-        
-        ## Links
-        * Project: https://github.com/ivankorobkov/python-inject
-        
-        ## License
-        Apache License 2.0
-        
-        ## Contributors
-        * Ivan Korobkov [@ivankorobkov](https://github.com/ivankorobkov)
-        * Jaime Wyant [@jaimewyant](https://github.com/jaimewyant)
-        * Sebastian Buczyński [@Enforcer](https://github.com/Enforcer)
-        * Oleksandr Fedorov [@Fedorof](https://github.com/Fedorof)
-        * cselvaraj [@cselvaraj](https://github.com/cselvaraj)
-        * 陆雨晴 [@SixExtreme](https://github.com/SixExtreme)
-        * Andrew William Borba [@andrewborba10](https://github.com/andrewborba10)
-        * jdmeyer3 [@jdmeyer3](https://github.com/jdmeyer3)
-        * Alex Grover [@ajgrover](https://github.com/ajgrover)
-        * Harro van der Kroft [@wisepotato](https://github.com/wisepotato)
-        * Samiur Rahman [@samiur](https://github.com/samiur)
-        * 45deg [@45deg](https://github.com/45deg)
-        * Alexander Nicholas Costas [@ancostas](https://github.com/ancostas)
-        * Dmitry Balabka [@dbalabka](https://github.com/dbalabka)
-        
-Platform: UNKNOWN
+Name: inject
+Version: 5.0.0
+Summary: Python dependency injection framework.
+Project-URL: Homepage, https://github.com/ivankorobkov/python-inject
+Author-email: Ivan Korobkov <ivan.korobkov@gmail.com>
+Maintainer-email: Ivan Korobkov <ivan.korobkov@gmail.com>
+License-Expression: Apache-2.0
+License-File: LICENSE
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3.6
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
+Classifier: Programming Language :: Python :: 3.9
+Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
 Classifier: Topic :: Software Development :: Libraries :: Python Modules
 Description-Content-Type: text/markdown
+
+# python-inject [![Build Status](https://travis-ci.org/ivankorobkov/python-inject.svg?branch=master)](https://travis-ci.org/ivankorobkov/python-inject)
+Dependency injection the python way, the good way. Not a port of Guice or Spring.
+
+## Key features
+* Fast.
+* Thread-safe.
+* Simple to use.
+* Does not steal class constructors.
+* Does not try to manage your application object graph.
+* Transparently integrates into tests.
+* Supports Python 3.5+ (`v4.*`) and Python 2.7–3.5 (`v3.*`).
+* Supports type hinting in Python 3.5+.
+* Autoparams leveraging type annotations.
+
+## Python Support
+
+| Python  | Inject Version |
+|---------|----------------|
+| 3.9+    | 5.0+           |
+| 3.6-3.8 | 4.1+, < 5.0    |
+| 3.5     | 4.0            |
+| < 3.5   | 3.*            |
+
+
+## Installation
+Use pip to install the lastest version:
+
+```bash
+pip install inject
+```
+
+## Autoparams example
+`@inject.autoparams` returns a decorator which automatically injects arguments into a function 
+that uses type annotations. This is supported only in Python >= 3.5.
+
+```python
+@inject.autoparams()
+def refresh_cache(cache: RedisCache, db: DbInterface):
+    pass
+```
+
+There is an option to specify which arguments we want to inject without attempts of 
+injecting everything:
+
+```python
+@inject.autoparams('cache', 'db')
+def sign_up(name, email, cache: RedisCache, db: DbInterface):
+    pass
+```
+
+## Step-by-step example
+```python
+# Import the inject module.
+import inject
+
+
+# `inject.instance` requests dependencies from the injector.
+def foo(bar):
+    cache = inject.instance(Cache)
+    cache.save('bar', bar)
+
+
+# `inject.params` injects dependencies as keyword arguments or positional argument. 
+# Also you can use @inject.autoparams in Python 3.5, see the example above.
+@inject.params(cache=Cache, user=CurrentUser)
+def baz(foo, cache=None, user=None):
+    cache.save('foo', foo, user)
+
+# this can be called in different ways:
+# with injected arguments
+baz('foo')
+
+# with positional arguments
+baz('foo', my_cache)
+
+# with keyword arguments
+baz('foo', my_cache, user=current_user)
+
+
+# `inject.param` is deprecated, use `inject.params` instead.
+@inject.param('cache', Cache)
+def bar(foo, cache=None):
+    cache.save('foo', foo)
+
+
+# `inject.attr` creates properties (descriptors) which request dependencies on access.
+class User(object):
+    cache = inject.attr(Cache)
+            
+    def __init__(self, id):
+        self.id = id
+
+    def save(self):
+        self.cache.save('users', self)
+    
+    @classmethod
+    def load(cls, id):
+        return cls.cache.load('users', id)
+
+
+# Create an optional configuration.
+def my_config(binder):
+    binder.install(my_config2)  # Add bindings from another config.
+    binder.bind(Cache, RedisCache('localhost:1234'))
+
+# Configure a shared injector.
+inject.configure(my_config)
+
+
+# Instantiate User as a normal class. Its `cache` dependency is injected when accessed.
+user = User(10)
+user.save()
+
+# Call the functions, the dependencies are automatically injected.
+foo('Hello')
+bar('world')
+```
+
+
+## Usage with Django
+Django can load some modules multiple times which can lead to 
+`InjectorException: Injector is already configured`. You can use `configure_once` which
+is guaranteed to run only once when the injector is absent:
+```python
+import inject
+inject.configure_once(my_config)
+```
+
+## Testing
+In tests use `inject.clear_and_configure(callable)` to create a new injector on setup,
+and optionally `inject.clear()` to clean up on tear down:
+```python
+class MyTest(unittest.TestCase):
+    def setUp(self):
+        inject.clear_and_configure(lambda binder: binder
+            .bind(Cache, Mock()) \
+            .bind(Validator, TestValidator()))
+    
+    def tearDown(self):
+        inject.clear()
+```
+
+## Thread-safety
+After configuration the injector is thread-safe and can be safely reused by multiple threads.
+
+## Binding types
+**Instance** bindings always return the same instance:
+
+```python
+redis = RedisCache(address='localhost:1234')
+def config(binder):
+    binder.bind(Cache, redis)
+```
+    
+**Constructor** bindings create a singleton on injection:
+
+```python
+def config(binder):
+    # Creates a redis cache singleton on first injection.
+    binder.bind_to_constructor(Cache, lambda: RedisCache(address='localhost:1234'))
+```
+
+**Provider** bindings call the provider on injection:
+
+```python
+def get_my_thread_local_cache():
+    pass
+
+def config(binder):
+    # Executes the provider on each injection.
+    binder.bind_to_provider(Cache, get_my_thread_local_cache) 
+```
+
+**Runtime** bindings automatically create singletons on injection, require no configuration.
+For example, only the `Config` class binding is present, other bindings are runtime:
+
+```python
+class Config(object):
+    pass
+
+class Cache(object):
+    config = inject.attr(Config)
+
+class Db(object):
+    config = inject.attr(Config)
+
+class User(object):
+    cache = inject.attr(Cache)
+    db = inject.attr(Db)
+    
+    @classmethod
+    def load(cls, user_id):
+        return cls.cache.load('users', user_id) or cls.db.load('users', user_id)
+    
+inject.configure(lambda binder: binder.bind(Config, load_config_file()))
+user = User.load(10)
+```
+## Disabling runtime binding
+Sometimes runtime binding leads to unexpected behaviour.  Say if you forget
+to bind an instance to a class, `inject` will try to implicitly instantiate it.
+
+If an instance is unintentionally created with default arguments it may lead to
+hard-to-debug bugs.  To disable runtime binding and make sure that only 
+explicitly bound instances are injected, pass `bind_in_runtime=False` 
+to `inject.configure`, `inject.configure_once` or `inject.clear_and_configure`.
+
+In this case `inject` immediately raises `InjectorException` when the code
+tries to get an unbound instance.
+
+## Keys
+It is possible to use any hashable object as a binding key. For example:
+
+```python
+import inject
+
+inject.configure(lambda binder: \
+    binder.bind('host', 'localhost') \
+    binder.bind('port', 1234))
+```
+
+## Why no scopes?
+I've used Guice and Spring in Java for a lot of years, and I don't like their scopes.
+`python-inject` by default creates objects as singletons. It does not need a prototype scope
+as in Spring or NO_SCOPE as in Guice because `python-inject` does not steal your class 
+constructors. Create instances the way you like and then inject dependencies into them.
+
+Other scopes such as a request scope or a session scope are fragile, introduce high coupling,
+and are difficult to test. In `python-inject` write custom providers which can be thread-local, 
+request-local, etc.
+
+For example, a thread-local current user provider:
+
+```python
+import inject
+import threading
+
+# Given a user class.
+class User(object):
+    pass
+
+# Create a thread-local current user storage.
+_LOCAL = threading.local()
+
+def get_current_user():
+    return getattr(_LOCAL, 'user', None)
+
+def set_current_user(user):
+    _LOCAL.user = user
+
+# Bind User to a custom provider.
+inject.configure(lambda binder: binder.bind_to_provider(User, get_current_user))
+
+# Inject the current user.
+@inject.params(user=User)
+def foo(user):
+    pass
+```
+
+## Links
+* Project: https://github.com/ivankorobkov/python-inject
+
+## License
+Apache License 2.0
+
+## Contributors
+* Ivan Korobkov [@ivankorobkov](https://github.com/ivankorobkov)
+* Jaime Wyant [@jaimewyant](https://github.com/jaimewyant)
+* Sebastian Buczyński [@Enforcer](https://github.com/Enforcer)
+* Oleksandr Fedorov [@Fedorof](https://github.com/Fedorof)
+* cselvaraj [@cselvaraj](https://github.com/cselvaraj)
+* 陆雨晴 [@SixExtreme](https://github.com/SixExtreme)
+* Andrew William Borba [@andrewborba10](https://github.com/andrewborba10)
+* jdmeyer3 [@jdmeyer3](https://github.com/jdmeyer3)
+* Alex Grover [@ajgrover](https://github.com/ajgrover)
+* Harro van der Kroft [@wisepotato](https://github.com/wisepotato)
+* Samiur Rahman [@samiur](https://github.com/samiur)
+* 45deg [@45deg](https://github.com/45deg)
+* Alexander Nicholas Costas [@ancostas](https://github.com/ancostas)
+* Dmitry Balabka [@dbalabka](https://github.com/dbalabka)
```

### Comparing `Inject-4.3.1/LICENSE` & `inject-5.0.0/LICENSE`

 * *Files identical despite different names*

### Comparing `Inject-4.3.1/README.md` & `inject-5.0.0/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -10,19 +10,20 @@
 * Transparently integrates into tests.
 * Supports Python 3.5+ (`v4.*`) and Python 2.7–3.5 (`v3.*`).
 * Supports type hinting in Python 3.5+.
 * Autoparams leveraging type annotations.
 
 ## Python Support
 
-| Python | Inject Version |
-|--------|----------------|
-| 3.6+   | 4.1+           |
-| 3.5    | 4.0            |
-| < 3.5  | 3.*            |
+| Python  | Inject Version |
+|---------|----------------|
+| 3.9+    | 5.0+           |
+| 3.6-3.8 | 4.1+, < 5.0    |
+| 3.5     | 4.0            |
+| < 3.5   | 3.*            |
 
 
 ## Installation
 Use pip to install the lastest version:
 
 ```bash
 pip install inject
```

### Comparing `Inject-4.3.1/inject/__init__.py` & `inject-5.0.0/src/inject/__init__.py`

 * *Files 6% similar despite different names*

```diff
@@ -69,34 +69,36 @@
 
     def my_config(binder):
         binder.bind(Config, load_config_file())
 
     inject.configure(my_config)
 
 """
-__version__ = '4.3.1'
-__author__ = 'Ivan Korobkov <ivan.korobkov@gmail.com>'
-__license__ = 'Apache License 2.0'
-__url__ = 'https://github.com/ivan-korobkov/python-inject'
-
+from inject._version import __version__
 
 import inspect
 import logging
 import sys
 import threading
-import types
 from functools import wraps
 from typing import (Any, Awaitable, Callable, Dict, Generic, Hashable,
                     Optional, Type, TypeVar, Union, cast, get_type_hints,
                     overload)
 
-_NEW_TYPING = sys.version_info[:3] >= (3, 7, 0)  # PEP 560
+_HAS_PEP604_SUPPORT = sys.version_info[:3] >= (3, 10, 0)  # PEP 604
+if _HAS_PEP604_SUPPORT:
+    _HAS_PEP560_SUPPORT = True
+else:
+    _HAS_PEP560_SUPPORT = sys.version_info[:3] >= (3, 7, 0)  # PEP 560
 _RETURN = 'return'
 
-if _NEW_TYPING:
+if _HAS_PEP604_SUPPORT:
+    from types import UnionType
+    from typing import ForwardRef, _GenericAlias
+elif _HAS_PEP560_SUPPORT:
     from typing import ForwardRef, _GenericAlias
 else:
     from typing import _Union
 
 
 logger = logging.getLogger('inject')
 
@@ -175,25 +177,25 @@
         if self._is_forward_str(cls):
             ref = ForwardRef(cls)
             if ref in self._bindings:
                 raise InjectorException('Duplicate forward binding, i.e. "int" and int, key=%s', cls)
     
     def _maybe_bind_forward(self, cls: Binding, binding: Any) -> None:
         """Bind a string forward reference."""
-        if not _NEW_TYPING:
+        if not _HAS_PEP560_SUPPORT:
             return
         if not isinstance(cls, str):
             return
         
         ref = ForwardRef(cls)
         self._bindings[ref] = binding
         logger.debug('Bound forward ref "%s"', cls)
 
     def _is_forward_str(self, cls: Binding) -> bool:
-        return _NEW_TYPING and isinstance(cls, str)
+        return _HAS_PEP560_SUPPORT and isinstance(cls, str)
 
 
 class Injector(object):
     _bindings: Dict[Binding, Constructor]
 
     def __init__(self, config: Optional[BinderCallable] = None, bind_in_runtime: bool = True):
         self._bind_in_runtime = bind_in_runtime
@@ -270,14 +272,25 @@
     def __init__(self, cls: Binding) -> None:
         self._cls = cls
 
     def __get__(self, obj: Any, owner: Any) -> Injectable:
         return instance(self._cls)
 
 
+class _AttributeInjectionDataclass(Generic[T]):
+    def __init__(self, cls: Binding) -> None:
+        self._cls = cls
+
+    def __get__(self, instance, owner) -> T:
+        injector = get_injector()
+        if injector is not None:
+            return injector.get_instance(self._cls)
+        raise AttributeError
+
+
 class _ParameterInjection(Generic[T]):
     __slots__ = ('_name', '_cls')
 
     def __init__(self, name: str, cls: Optional[Binding] = None) -> None:
         self._name = name
         self._cls = cls
 
@@ -407,14 +420,24 @@
 @overload
 def attr(cls: Hashable) -> Injectable: ...
 
 def attr(cls: Binding) -> Injectable:
     """Return a attribute injection (descriptor)."""
     return _AttributeInjection(cls)
 
+@overload
+def attr_dc(cls: Type[T]) -> T: ...
+
+@overload
+def attr_dc(cls: Hashable) -> Injectable: ...
+
+def attr_dc(cls: Binding) -> Injectable:
+    """Return a attribute injection (descriptor)."""
+    return _AttributeInjectionDataclass(cls)
+
 
 def param(name: str, cls: Optional[Binding] = None) -> Callable:
     """Deprecated, use @inject.params. Return a decorator which injects an arg into a function."""
     return _ParameterInjection(name, cls)
 
 
 def params(**args_to_classes: Binding) -> Callable:
@@ -491,14 +514,18 @@
 
 def _is_union_type(typ):
     """Test if the type is a union type. Examples::
         is_union_type(int) == False
         is_union_type(Union) == True
         is_union_type(Union[int, int]) == False
         is_union_type(Union[T, int]) == True
-    
+
     Source: https://github.com/ilevkivskyi/typing_inspect/blob/master/typing_inspect.py
     """
-    if _NEW_TYPING:
+    if _HAS_PEP604_SUPPORT:
+        return (typ is Union or
+                isinstance(typ, UnionType) or
+                isinstance(typ, _GenericAlias) and typ.__origin__ is Union)
+    elif _HAS_PEP560_SUPPORT:
         return (typ is Union or
                 isinstance(typ, _GenericAlias) and typ.__origin__ is Union)
     return type(typ) is _Union
```

### Comparing `Inject-4.3.1/test/test_attr.py` & `inject-5.0.0/test/test_attr.py`

 * *Files 19% similar despite different names*

```diff
@@ -21,7 +21,21 @@
 
         inject.configure(lambda binder: binder.bind(int, 123))
         value0 = MyClass.field
         value1 = MyClass.field
 
         assert value0 == 123
         assert value1 == 123
+
+
+class TestInjectAttrDataclass(BaseTestInject):
+    def test_class_attr_dc(self):
+        class MyClass(object):
+            field = inject.attr_dc(int)
+
+        inject.configure(lambda binder: binder.bind(int, 123))
+        value0 = MyClass.field
+        value1 = MyClass.field
+
+        assert value0 == 123
+        assert value1 == 123
+
```

### Comparing `Inject-4.3.1/test/test_autoparams.py` & `inject-5.0.0/test/test_autoparams.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,7 +1,10 @@
+import sys
+from typing import Optional
+
 from test import BaseTestInject
 
 import inject
 
 
 class A: pass
 class B: pass
@@ -168,14 +171,47 @@
             return a, b, c
 
         def config(binder):
             binder.bind(A, 1)
             binder.bind(B, 2)
             binder.bind(C, 3)
 
+        inject.configure(config)
+
+        self.assertRaises(TypeError, test_func)
+        self.assertRaises(TypeError, test_func, a=1, c=3)
+
+    def test_autoparams_only_selected_with_optional(self):
+        @inject.autoparams('a', 'c')
+        def test_func(a: 'A', b: 'B', *, c: Optional[C] = None):
+            return a, b, c
+
+        def config(binder):
+            binder.bind(A, 1)
+            binder.bind(B, 2)
+            binder.bind(C, 3)
+
+        inject.configure(config)
+
+        self.assertRaises(TypeError, test_func)
+        self.assertRaises(TypeError, test_func, a=1, c=3)
+
+    def test_autoparams_only_selected_with_optional_pep604_union(self):
+        if not sys.version_info[:3] >= (3, 10, 0):
+            return
+
+        @inject.autoparams('a', 'c')
+        def test_func(a: 'A', b: 'B', *, c: C | None = None):
+            return a, b, c
+
+        def config(binder):
+            binder.bind(A, 1)
+            binder.bind(B, 2)
+            binder.bind(C, 3)
+
         inject.configure(config)
 
         self.assertRaises(TypeError, test_func)
         self.assertRaises(TypeError, test_func, a=1, c=3)
 
     def test_autoparams_omits_return_type(self):
         @inject.autoparams()
```

### Comparing `Inject-4.3.1/test/test_binder.py` & `inject-5.0.0/test/test_binder.py`

 * *Files identical despite different names*

### Comparing `Inject-4.3.1/test/test_functional.py` & `inject-5.0.0/test/test_functional.py`

 * *Files identical despite different names*

### Comparing `Inject-4.3.1/test/test_inject_configuration.py` & `inject-5.0.0/test/test_inject_configuration.py`

 * *Files identical despite different names*

### Comparing `Inject-4.3.1/test/test_injector.py` & `inject-5.0.0/test/test_injector.py`

 * *Files identical despite different names*

### Comparing `Inject-4.3.1/test/test_param.py` & `inject-5.0.0/test/test_param.py`

 * *Files identical despite different names*

### Comparing `Inject-4.3.1/test/test_params.py` & `inject-5.0.0/test/test_params.py`

 * *Files identical despite different names*

