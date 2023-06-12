# Comparing `tmp/django-synkroni-0.4.9.tar.gz` & `tmp/django-synkroni-0.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "django-synkroni-0.4.9.tar", last modified: Mon Jun 12 06:27:37 2023, max compression
+gzip compressed data, was "django-synkroni-0.5.tar", last modified: Mon Jun 12 06:25:01 2023, max compression
```

## Comparing `django-synkroni-0.4.9.tar` & `django-synkroni-0.5.tar`

### file list

```diff
@@ -1,31 +1,31 @@
-drwxr-xr-x   0 aha        (501) staff       (20)        0 2023-06-12 06:27:37.355263 django-synkroni-0.4.9/
--rw-r--r--   0 aha        (501) staff       (20)       75 2021-09-06 06:31:51.000000 django-synkroni-0.4.9/MANIFEST.in
--rw-r--r--   0 aha        (501) staff       (20)      242 2023-06-12 06:27:37.355096 django-synkroni-0.4.9/PKG-INFO
-drwxr-xr-x   0 aha        (501) staff       (20)        0 2023-06-12 06:27:37.352328 django-synkroni-0.4.9/django_synkroni.egg-info/
--rw-r--r--   0 aha        (501) staff       (20)      242 2023-06-12 06:27:37.000000 django-synkroni-0.4.9/django_synkroni.egg-info/PKG-INFO
--rw-r--r--   0 aha        (501) staff       (20)      592 2023-06-12 06:27:37.000000 django-synkroni-0.4.9/django_synkroni.egg-info/SOURCES.txt
--rw-r--r--   0 aha        (501) staff       (20)        1 2023-06-12 06:27:37.000000 django-synkroni-0.4.9/django_synkroni.egg-info/dependency_links.txt
--rw-r--r--   0 aha        (501) staff       (20)       47 2023-06-12 06:27:37.000000 django-synkroni-0.4.9/django_synkroni.egg-info/entry_points.txt
--rw-r--r--   0 aha        (501) staff       (20)     6752 2023-06-12 06:27:37.000000 django-synkroni-0.4.9/django_synkroni.egg-info/historia.json
--rw-r--r--   0 aha        (501) staff       (20)        1 2021-09-06 06:32:14.000000 django-synkroni-0.4.9/django_synkroni.egg-info/not-zip-safe
--rw-r--r--   0 aha        (501) staff       (20)       34 2023-06-12 06:27:37.000000 django-synkroni-0.4.9/django_synkroni.egg-info/requires.txt
--rw-r--r--   0 aha        (501) staff       (20)        9 2023-06-12 06:27:37.000000 django-synkroni-0.4.9/django_synkroni.egg-info/top_level.txt
--rw-r--r--   0 aha        (501) staff       (20)       80 2023-06-12 06:21:01.000000 django-synkroni-0.4.9/pyproject.toml
--rw-r--r--   0 aha        (501) staff       (20)       38 2023-06-12 06:27:37.355301 django-synkroni-0.4.9/setup.cfg
--rw-r--r--   0 aha        (501) staff       (20)      576 2023-06-12 06:20:49.000000 django-synkroni-0.4.9/setup.py
-drwxr-xr-x   0 aha        (501) staff       (20)        0 2023-06-12 06:27:37.354214 django-synkroni-0.4.9/synkroni/
--rw-r--r--   0 aha        (501) staff       (20)      107 2021-04-07 18:03:12.000000 django-synkroni-0.4.9/synkroni/__init__.py
--rw-r--r--   0 aha        (501) staff       (20)      683 2021-09-20 10:38:01.000000 django-synkroni-0.4.9/synkroni/json.py
--rw-r--r--   0 aha        (501) staff       (20)      261 2021-09-20 10:38:01.000000 django-synkroni-0.4.9/synkroni/komennot.py
--rw-r--r--   0 aha        (501) staff       (20)      159 2021-04-08 18:06:03.000000 django-synkroni-0.4.9/synkroni/mallit.py
--rw-r--r--   0 aha        (501) staff       (20)       22 2021-04-08 17:56:03.000000 django-synkroni-0.4.9/synkroni/models.py
-drwxr-xr-x   0 aha        (501) staff       (20)        0 2023-06-12 06:27:37.350088 django-synkroni-0.4.9/synkroni/static/
-drwxr-xr-x   0 aha        (501) staff       (20)        0 2023-06-12 06:27:37.350138 django-synkroni-0.4.9/synkroni/static/synkroni/
-drwxr-xr-x   0 aha        (501) staff       (20)        0 2023-06-12 06:27:37.354518 django-synkroni-0.4.9/synkroni/static/synkroni/js/
--rw-r--r--   0 aha        (501) staff       (20)     9447 2022-09-27 07:22:03.000000 django-synkroni-0.4.9/synkroni/static/synkroni/js/synkroni.js
--rw-r--r--   0 aha        (501) staff       (20)     2688 2022-11-18 14:29:51.000000 django-synkroni-0.4.9/synkroni/synkroni.py
-drwxr-xr-x   0 aha        (501) staff       (20)        0 2023-06-12 06:27:37.350261 django-synkroni-0.4.9/synkroni/templates/
-drwxr-xr-x   0 aha        (501) staff       (20)        0 2023-06-12 06:27:37.354818 django-synkroni-0.4.9/synkroni/templates/synkroni/
--rw-r--r--   0 aha        (501) staff       (20)      859 2022-05-04 12:06:11.000000 django-synkroni-0.4.9/synkroni/templates/synkroni/synkroni.html
--rw-r--r--   0 aha        (501) staff       (20)     2092 2023-06-12 06:27:27.000000 django-synkroni-0.4.9/synkroni/toiminnot.py
--rw-r--r--   0 aha        (501) staff       (20)     5565 2022-11-18 14:29:51.000000 django-synkroni-0.4.9/synkroni/websocket.py
+drwxr-xr-x   0 aha        (501) staff       (20)        0 2023-06-12 06:25:01.249438 django-synkroni-0.5/
+-rw-r--r--   0 aha        (501) staff       (20)       75 2021-09-06 06:31:51.000000 django-synkroni-0.5/MANIFEST.in
+-rw-r--r--   0 aha        (501) staff       (20)      240 2023-06-12 06:25:01.249285 django-synkroni-0.5/PKG-INFO
+drwxr-xr-x   0 aha        (501) staff       (20)        0 2023-06-12 06:25:01.246614 django-synkroni-0.5/django_synkroni.egg-info/
+-rw-r--r--   0 aha        (501) staff       (20)      240 2023-06-12 06:25:01.000000 django-synkroni-0.5/django_synkroni.egg-info/PKG-INFO
+-rw-r--r--   0 aha        (501) staff       (20)      592 2023-06-12 06:25:01.000000 django-synkroni-0.5/django_synkroni.egg-info/SOURCES.txt
+-rw-r--r--   0 aha        (501) staff       (20)        1 2023-06-12 06:25:01.000000 django-synkroni-0.5/django_synkroni.egg-info/dependency_links.txt
+-rw-r--r--   0 aha        (501) staff       (20)       47 2023-06-12 06:25:01.000000 django-synkroni-0.5/django_synkroni.egg-info/entry_points.txt
+-rw-r--r--   0 aha        (501) staff       (20)     6944 2023-06-12 06:25:01.000000 django-synkroni-0.5/django_synkroni.egg-info/historia.json
+-rw-r--r--   0 aha        (501) staff       (20)        1 2021-09-06 06:32:14.000000 django-synkroni-0.5/django_synkroni.egg-info/not-zip-safe
+-rw-r--r--   0 aha        (501) staff       (20)       34 2023-06-12 06:25:01.000000 django-synkroni-0.5/django_synkroni.egg-info/requires.txt
+-rw-r--r--   0 aha        (501) staff       (20)        9 2023-06-12 06:25:01.000000 django-synkroni-0.5/django_synkroni.egg-info/top_level.txt
+-rw-r--r--   0 aha        (501) staff       (20)       80 2023-06-12 06:21:01.000000 django-synkroni-0.5/pyproject.toml
+-rw-r--r--   0 aha        (501) staff       (20)       38 2023-06-12 06:25:01.249481 django-synkroni-0.5/setup.cfg
+-rw-r--r--   0 aha        (501) staff       (20)      576 2023-06-12 06:20:49.000000 django-synkroni-0.5/setup.py
+drwxr-xr-x   0 aha        (501) staff       (20)        0 2023-06-12 06:25:01.248422 django-synkroni-0.5/synkroni/
+-rw-r--r--   0 aha        (501) staff       (20)      107 2021-04-07 18:03:12.000000 django-synkroni-0.5/synkroni/__init__.py
+-rw-r--r--   0 aha        (501) staff       (20)      683 2021-09-20 10:38:01.000000 django-synkroni-0.5/synkroni/json.py
+-rw-r--r--   0 aha        (501) staff       (20)      261 2021-09-20 10:38:01.000000 django-synkroni-0.5/synkroni/komennot.py
+-rw-r--r--   0 aha        (501) staff       (20)      159 2021-04-08 18:06:03.000000 django-synkroni-0.5/synkroni/mallit.py
+-rw-r--r--   0 aha        (501) staff       (20)       22 2021-04-08 17:56:03.000000 django-synkroni-0.5/synkroni/models.py
+drwxr-xr-x   0 aha        (501) staff       (20)        0 2023-06-12 06:25:01.244742 django-synkroni-0.5/synkroni/static/
+drwxr-xr-x   0 aha        (501) staff       (20)        0 2023-06-12 06:25:01.244793 django-synkroni-0.5/synkroni/static/synkroni/
+drwxr-xr-x   0 aha        (501) staff       (20)        0 2023-06-12 06:25:01.248713 django-synkroni-0.5/synkroni/static/synkroni/js/
+-rw-r--r--   0 aha        (501) staff       (20)     9447 2022-09-27 07:22:03.000000 django-synkroni-0.5/synkroni/static/synkroni/js/synkroni.js
+-rw-r--r--   0 aha        (501) staff       (20)     2688 2022-11-18 14:29:51.000000 django-synkroni-0.5/synkroni/synkroni.py
+drwxr-xr-x   0 aha        (501) staff       (20)        0 2023-06-12 06:25:01.244918 django-synkroni-0.5/synkroni/templates/
+drwxr-xr-x   0 aha        (501) staff       (20)        0 2023-06-12 06:25:01.249089 django-synkroni-0.5/synkroni/templates/synkroni/
+-rw-r--r--   0 aha        (501) staff       (20)      859 2022-05-04 12:06:11.000000 django-synkroni-0.5/synkroni/templates/synkroni/synkroni.html
+-rw-r--r--   0 aha        (501) staff       (20)     2080 2023-06-08 12:38:34.000000 django-synkroni-0.5/synkroni/toiminnot.py
+-rw-r--r--   0 aha        (501) staff       (20)     5565 2022-11-18 14:29:51.000000 django-synkroni-0.5/synkroni/websocket.py
```

### Comparing `django-synkroni-0.4.9/django_synkroni.egg-info/SOURCES.txt` & `django-synkroni-0.5/django_synkroni.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `django-synkroni-0.4.9/django_synkroni.egg-info/historia.json` & `django-synkroni-0.5/django_synkroni.egg-info/historia.json`

 * *Files 2% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9743589743589743%*

 * *Differences: {'insert': "[(0, OrderedDict([('revisio', '058f3de1f888379881e82044d569970a3c884381'), ('versio', "*

 * *           "'0.5'), ('kuvaus', 'Muutettu `toiminnot.muuttaa_tietoja` asynkroniseksi "*

 * *           "kontekstinkäsittelijäksi')]))]"}*

```diff
@@ -1,9 +1,14 @@
 [
     {
+        "kuvaus": "Muutettu `toiminnot.muuttaa_tietoja` asynkroniseksi kontekstink\u00e4sittelij\u00e4ksi",
+        "revisio": "058f3de1f888379881e82044d569970a3c884381",
+        "versio": "0.5"
+    },
+    {
         "kuvaus": "P\u00e4ivitetty versiointij\u00e4rjestelm\u00e4",
         "revisio": "a3c6dfc33ea6c98b28f8b5a3929e27e70055e3c0",
         "versio": "0.4.9"
     },
     {
         "kuvaus": "Lis\u00e4tty `Toiminnot.mittaa_toiminnon_kesto`-metodi",
         "revisio": "51fab908f6db02be338eceda5f18acb195df77f7",
```

### Comparing `django-synkroni-0.4.9/setup.py` & `django-synkroni-0.5/setup.py`

 * *Files identical despite different names*

### Comparing `django-synkroni-0.4.9/synkroni/json.py` & `django-synkroni-0.5/synkroni/json.py`

 * *Files identical despite different names*

### Comparing `django-synkroni-0.4.9/synkroni/static/synkroni/js/synkroni.js` & `django-synkroni-0.5/synkroni/static/synkroni/js/synkroni.js`

 * *Files identical despite different names*

### Comparing `django-synkroni-0.4.9/synkroni/synkroni.py` & `django-synkroni-0.5/synkroni/synkroni.py`

 * *Files identical despite different names*

### Comparing `django-synkroni-0.4.9/synkroni/templates/synkroni/synkroni.html` & `django-synkroni-0.5/synkroni/templates/synkroni/synkroni.html`

 * *Files identical despite different names*

### Comparing `django-synkroni-0.4.9/synkroni/websocket.py` & `django-synkroni-0.5/synkroni/websocket.py`

 * *Files identical despite different names*

