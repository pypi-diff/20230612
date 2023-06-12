# Comparing `tmp/feincms3_data-0.5.1.tar.gz` & `tmp/feincms3_data-0.6.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "feincms3_data-0.5.1.tar", last modified: Wed Mar 15 09:15:41 2023, max compression
+gzip compressed data, last modified: Sun Feb  2 00:00:00 2020, max compression
```

## Comparing `feincms3_data-0.5.1.tar` & `feincms3_data-0.6.0.tar`

### file list

```diff
@@ -1,24 +1,29 @@
-drwxr-xr-x   0 matthias  (1000) matthias  (1000)        0 2023-03-15 09:15:41.536018 feincms3_data-0.5.1/
--rw-r--r--   0 matthias  (1000) matthias  (1000)     1548 2022-08-12 14:48:09.000000 feincms3_data-0.5.1/LICENSE
--rw-r--r--   0 matthias  (1000) matthias  (1000)      181 2022-08-12 14:48:09.000000 feincms3_data-0.5.1/MANIFEST.in
--rw-r--r--   0 matthias  (1000) matthias  (1000)     6271 2023-03-15 09:15:41.536018 feincms3_data-0.5.1/PKG-INFO
--rw-r--r--   0 matthias  (1000) matthias  (1000)     5251 2023-03-15 08:51:28.000000 feincms3_data-0.5.1/README.rst
-drwxr-xr-x   0 matthias  (1000) matthias  (1000)        0 2023-03-15 09:15:41.535018 feincms3_data-0.5.1/feincms3_data/
--rw-r--r--   0 matthias  (1000) matthias  (1000)       62 2023-03-15 09:15:19.000000 feincms3_data-0.5.1/feincms3_data/__init__.py
--rw-r--r--   0 matthias  (1000) matthias  (1000)     7818 2023-03-15 09:09:02.000000 feincms3_data-0.5.1/feincms3_data/data.py
-drwxr-xr-x   0 matthias  (1000) matthias  (1000)        0 2023-03-15 09:15:41.536018 feincms3_data-0.5.1/feincms3_data/management/
--rw-r--r--   0 matthias  (1000) matthias  (1000)        0 2023-03-15 09:09:02.000000 feincms3_data-0.5.1/feincms3_data/management/__init__.py
-drwxr-xr-x   0 matthias  (1000) matthias  (1000)        0 2023-03-15 09:15:41.536018 feincms3_data-0.5.1/feincms3_data/management/commands/
--rw-r--r--   0 matthias  (1000) matthias  (1000)        0 2023-03-15 09:09:02.000000 feincms3_data-0.5.1/feincms3_data/management/commands/__init__.py
--rw-r--r--   0 matthias  (1000) matthias  (1000)      745 2023-03-15 09:15:31.000000 feincms3_data-0.5.1/feincms3_data/management/commands/f3dumpdata.py
--rw-r--r--   0 matthias  (1000) matthias  (1000)      983 2023-03-15 09:09:02.000000 feincms3_data-0.5.1/feincms3_data/management/commands/f3loaddata.py
--rw-r--r--   0 matthias  (1000) matthias  (1000)      333 2023-03-15 09:09:02.000000 feincms3_data-0.5.1/feincms3_data/serializers.py
-drwxr-xr-x   0 matthias  (1000) matthias  (1000)        0 2023-03-15 09:15:41.536018 feincms3_data-0.5.1/feincms3_data.egg-info/
--rw-r--r--   0 matthias  (1000) matthias  (1000)     6271 2023-03-15 09:15:41.000000 feincms3_data-0.5.1/feincms3_data.egg-info/PKG-INFO
--rw-r--r--   0 matthias  (1000) matthias  (1000)      525 2023-03-15 09:15:41.000000 feincms3_data-0.5.1/feincms3_data.egg-info/SOURCES.txt
--rw-r--r--   0 matthias  (1000) matthias  (1000)        1 2023-03-15 09:15:41.000000 feincms3_data-0.5.1/feincms3_data.egg-info/dependency_links.txt
--rw-r--r--   0 matthias  (1000) matthias  (1000)        1 2022-09-05 12:07:00.000000 feincms3_data-0.5.1/feincms3_data.egg-info/not-zip-safe
--rw-r--r--   0 matthias  (1000) matthias  (1000)       30 2023-03-15 09:15:41.000000 feincms3_data-0.5.1/feincms3_data.egg-info/requires.txt
--rw-r--r--   0 matthias  (1000) matthias  (1000)       14 2023-03-15 09:15:41.000000 feincms3_data-0.5.1/feincms3_data.egg-info/top_level.txt
--rw-r--r--   0 matthias  (1000) matthias  (1000)     1258 2023-03-15 09:15:41.536018 feincms3_data-0.5.1/setup.cfg
--rwxr-xr-x   0 matthias  (1000) matthias  (1000)       62 2022-08-12 14:48:09.000000 feincms3_data-0.5.1/setup.py
+-rw-r--r--   0        0        0      200 2020-02-02 00:00:00.000000 feincms3_data-0.6.0/.editorconfig
+-rw-r--r--   0        0        0     1336 2020-02-02 00:00:00.000000 feincms3_data-0.6.0/.pre-commit-config.yaml
+-rw-r--r--   0        0        0      134 2020-02-02 00:00:00.000000 feincms3_data-0.6.0/.readthedocs.yml
+-rw-r--r--   0        0        0     3284 2020-02-02 00:00:00.000000 feincms3_data-0.6.0/CHANGELOG.rst
+-rw-r--r--   0        0        0      592 2020-02-02 00:00:00.000000 feincms3_data-0.6.0/tox.ini
+-rw-r--r--   0        0        0      855 2020-02-02 00:00:00.000000 feincms3_data-0.6.0/.github/workflows/tests.yml
+-rw-r--r--   0        0        0      604 2020-02-02 00:00:00.000000 feincms3_data-0.6.0/docs/Makefile
+-rw-r--r--   0        0        0     1314 2020-02-02 00:00:00.000000 feincms3_data-0.6.0/docs/conf.py
+-rw-r--r--   0        0        0       57 2020-02-02 00:00:00.000000 feincms3_data-0.6.0/docs/index.rst
+-rw-r--r--   0        0        0      765 2020-02-02 00:00:00.000000 feincms3_data-0.6.0/docs/make.bat
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 feincms3_data-0.6.0/docs/requirements.txt
+-rw-r--r--   0        0        0       22 2020-02-02 00:00:00.000000 feincms3_data-0.6.0/feincms3_data/__init__.py
+-rw-r--r--   0        0        0     8010 2020-02-02 00:00:00.000000 feincms3_data-0.6.0/feincms3_data/data.py
+-rw-r--r--   0        0        0      333 2020-02-02 00:00:00.000000 feincms3_data-0.6.0/feincms3_data/serializers.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 feincms3_data-0.6.0/feincms3_data/management/__init__.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 feincms3_data-0.6.0/feincms3_data/management/commands/__init__.py
+-rw-r--r--   0        0        0      755 2020-02-02 00:00:00.000000 feincms3_data-0.6.0/feincms3_data/management/commands/f3dumpdata.py
+-rw-r--r--   0        0        0      983 2020-02-02 00:00:00.000000 feincms3_data-0.6.0/feincms3_data/management/commands/f3loaddata.py
+-rwxr-xr-x   0        0        0      331 2020-02-02 00:00:00.000000 feincms3_data-0.6.0/tests/manage.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 feincms3_data-0.6.0/tests/testapp/__init__.py
+-rw-r--r--   0        0        0     1245 2020-02-02 00:00:00.000000 feincms3_data-0.6.0/tests/testapp/models.py
+-rw-r--r--   0        0        0     1730 2020-02-02 00:00:00.000000 feincms3_data-0.6.0/tests/testapp/settings.py
+-rw-r--r--   0        0        0      209 2020-02-02 00:00:00.000000 feincms3_data-0.6.0/tests/testapp/specs.py
+-rw-r--r--   0        0        0    18692 2020-02-02 00:00:00.000000 feincms3_data-0.6.0/tests/testapp/test_data.py
+-rw-r--r--   0        0        0      156 2020-02-02 00:00:00.000000 feincms3_data-0.6.0/.gitignore
+-rw-r--r--   0        0        0     1548 2020-02-02 00:00:00.000000 feincms3_data-0.6.0/LICENSE
+-rw-r--r--   0        0        0     5251 2020-02-02 00:00:00.000000 feincms3_data-0.6.0/README.rst
+-rw-r--r--   0        0        0     2110 2020-02-02 00:00:00.000000 feincms3_data-0.6.0/pyproject.toml
+-rw-r--r--   0        0        0     6324 2020-02-02 00:00:00.000000 feincms3_data-0.6.0/PKG-INFO
```

### Comparing `feincms3_data-0.5.1/LICENSE` & `feincms3_data-0.6.0/LICENSE`

 * *Files identical despite different names*

### Comparing `feincms3_data-0.5.1/PKG-INFO` & `feincms3_data-0.6.0/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,33 +1,33 @@
 Metadata-Version: 2.1
-Name: feincms3_data
-Version: 0.5.1
-Home-page: https://github.com/matthiask/feincms3-data/
-Author: Matthias Kestenholz
-Author-email: mk@feinheit.ch
+Name: feincms3-data
+Version: 0.6.0
+Project-URL: Homepage, https://github.com/matthiask/feincms3-data/
+Author-email: Matthias Kestenholz <mk@feinheit.ch>
 License: BSD-3-Clause
-Platform: OS Independent
+License-File: LICENSE
 Classifier: Environment :: Web Environment
 Classifier: Framework :: Django
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: BSD License
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python
-Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3 :: Only
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
 Classifier: Topic :: Internet :: WWW/HTTP :: Dynamic Content
 Classifier: Topic :: Software Development
 Classifier: Topic :: Software Development :: Libraries :: Application Frameworks
 Requires-Python: >=3.8
-Description-Content-Type: text/x-rst
+Requires-Dist: django>=3.2
 Provides-Extra: tests
-License-File: LICENSE
+Requires-Dist: coverage; extra == 'tests'
+Description-Content-Type: text/x-rst
 
 =============
 feincms3-data
 =============
 
 .. image:: https://github.com/matthiask/feincms3-data/actions/workflows/tests.yml/badge.svg
     :target: https://github.com/matthiask/feincms3-data/
```

### Comparing `feincms3_data-0.5.1/README.rst` & `feincms3_data-0.6.0/README.rst`

 * *Files identical despite different names*

### Comparing `feincms3_data-0.5.1/feincms3_data/data.py` & `feincms3_data-0.6.0/feincms3_data/data.py`

 * *Files 4% similar despite different names*

```diff
@@ -34,15 +34,19 @@
 def _random_values():
     """Generate a stream of values which are unlikely to cause conflicts"""
     prefix = get_random_string(20)
     for i in count():
         yield f"{prefix}-{i}"
 
 
-class InvalidSpec(Exception):
+class InvalidVersionError(Exception):
+    pass
+
+
+class InvalidSpecError(Exception):
     pass
 
 
 _valid_keys = {
     "model",
     "filter",
     # Flags:
@@ -51,62 +55,62 @@
     "save_as_new",
     "defer_values",
 }
 
 
 def _validate_spec(spec):
     if "model" not in spec:
-        raise InvalidSpec(f"The spec {spec!r} requires a 'model' key")
+        raise InvalidSpecError(f"The spec {spec!r} requires a 'model' key")
     if unknown := (set(spec.keys()) - _valid_keys):
-        raise InvalidSpec(f"The spec {spec!r} contains unknown keys: {unknown!r}")
+        raise InvalidSpecError(f"The spec {spec!r} contains unknown keys: {unknown!r}")
     return spec
 
 
 def specs_for_models(models, spec=None):
     spec = {} if spec is None else spec
-    return (_validate_spec({**spec, "model": cls._meta.label_lower}) for cls in models)
+    return [_validate_spec({**spec, "model": cls._meta.label_lower}) for cls in models]
 
 
 def specs_for_derived_models(cls, spec=None):
     return specs_for_models(_only_concrete_models(_all_subclasses(cls)), spec)
 
 
 def specs_for_app_models(app, spec=None):
     return specs_for_models(apps.get_app_config(app).get_models(), spec)
 
 
 def _model_queryset(spec):
     queryset = apps.get_model(spec["model"])._default_manager.all()
-    if filter := spec.get("filter"):
-        queryset = queryset.filter(**filter)
+    if f := spec.get("filter"):
+        queryset = queryset.filter(**f)
     return queryset
 
 
 def silence(*a):
     pass
 
 
-def dump_specs(specs, *, mappers=None):
+def dump_specs(specs, *, mappers=None, objects=None):
     stream = io.StringIO()
     stream.write('{"version": 1, "specs": ')
     json.dump(specs, stream)
     stream.write(', "objects": ')
     serializer = JSONSerializer(mappers=mappers or {})
-    serializer.serialize(
-        chain.from_iterable(_model_queryset(spec) for spec in specs),
-        stream=stream,
-    )
+    if objects is None:
+        objects = chain.from_iterable(_model_queryset(spec) for spec in specs)
+    serializer.serialize(objects, stream=stream)
     stream.write("}")
     return stream.getvalue()
 
 
 def load_dump(
     data, *, progress=silence, ignorenonexistent=False, using=DEFAULT_DB_ALIAS
 ):
-    assert data["version"] == 1
+    if data["version"] != 1:
+        raise InvalidVersionError(f"Invalid dump version {data.get('version')!r}")
     for spec in data["specs"]:
         _validate_spec(spec)
 
     objects = defaultdict(list)
     seen_pks = defaultdict(set)
 
     # Yes, that is a bit stupid
@@ -136,15 +140,15 @@
             _finalize(
                 progress,
                 connection,
                 models,
             )
 
 
-def _load_dump(
+def _load_dump(  # noqa: PLR0913
     data,
     objects,
     progress,
     seen_pks,
     save_as_new_models,
     models,
 ):
```

### Comparing `feincms3_data-0.5.1/feincms3_data/management/commands/f3dumpdata.py` & `feincms3_data-0.6.0/feincms3_data/management/commands/f3dumpdata.py`

 * *Files 2% similar despite different names*

```diff
@@ -16,9 +16,9 @@
     def handle(self, *args, **options):
         dataset, sep, args = options["dataset"].partition(":")
         try:
             ds = DATASETS[dataset]
         except KeyError:
             raise CommandError(
                 f"Invalid dataset {dataset}; should be one of {', '.join(DATASETS)}"
-            )
+            ) from None
         self.stdout.write(dump_specs(ds["specs"](args), mappers=ds.get("mappers")))
```

### Comparing `feincms3_data-0.5.1/feincms3_data/management/commands/f3loaddata.py` & `feincms3_data-0.6.0/feincms3_data/management/commands/f3loaddata.py`

 * *Files identical despite different names*

