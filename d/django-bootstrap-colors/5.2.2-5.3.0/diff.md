# Comparing `tmp/django_bootstrap_colors-5.2.2-py3-none-any.whl.zip` & `tmp/django_bootstrap_colors-5.3.0-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,10 +1,10 @@
-Zip file size: 3773 bytes, number of entries: 8
+Zip file size: 3850 bytes, number of entries: 8
 -rw-r--r--  2.0 unx        0 b- defN 23-May-09 09:26 bootstrap_colors/__init__.py
--rw-r--r--  2.0 unx      464 b- defN 23-May-23 14:30 bootstrap_colors/views.py
--rw-r--r--  2.0 unx     1722 b- defN 23-May-09 09:13 bootstrap_colors/templates/bootstrap_colors.css
--rw-r--r--  2.0 unx     1065 b- defN 23-May-23 14:34 django_bootstrap_colors-5.2.2.dist-info/LICENSE
--rw-r--r--  2.0 unx     1206 b- defN 23-May-23 14:34 django_bootstrap_colors-5.2.2.dist-info/METADATA
--rw-r--r--  2.0 unx       92 b- defN 23-May-23 14:34 django_bootstrap_colors-5.2.2.dist-info/WHEEL
--rw-r--r--  2.0 unx       17 b- defN 23-May-23 14:34 django_bootstrap_colors-5.2.2.dist-info/top_level.txt
-?rw-rw-r--  2.0 unx      733 b- defN 23-May-23 14:34 django_bootstrap_colors-5.2.2.dist-info/RECORD
-8 files, 5299 bytes uncompressed, 2465 bytes compressed:  53.5%
+-rw-r--r--  2.0 unx      464 b- defN 23-Jun-05 16:33 bootstrap_colors/views.py
+-rw-r--r--  2.0 unx     1813 b- defN 23-Jun-12 14:11 bootstrap_colors/templates/bootstrap_colors.css
+-rw-r--r--  2.0 unx     1065 b- defN 23-Jun-12 14:16 django_bootstrap_colors-5.3.0.dist-info/LICENSE
+-rw-r--r--  2.0 unx     1303 b- defN 23-Jun-12 14:16 django_bootstrap_colors-5.3.0.dist-info/METADATA
+-rw-r--r--  2.0 unx       92 b- defN 23-Jun-12 14:16 django_bootstrap_colors-5.3.0.dist-info/WHEEL
+-rw-r--r--  2.0 unx       17 b- defN 23-Jun-12 14:16 django_bootstrap_colors-5.3.0.dist-info/top_level.txt
+?rw-rw-r--  2.0 unx      733 b- defN 23-Jun-12 14:16 django_bootstrap_colors-5.3.0.dist-info/RECORD
+8 files, 5487 bytes uncompressed, 2542 bytes compressed:  53.7%
```

## zipnote {}

```diff
@@ -3,23 +3,23 @@
 
 Filename: bootstrap_colors/views.py
 Comment: 
 
 Filename: bootstrap_colors/templates/bootstrap_colors.css
 Comment: 
 
-Filename: django_bootstrap_colors-5.2.2.dist-info/LICENSE
+Filename: django_bootstrap_colors-5.3.0.dist-info/LICENSE
 Comment: 
 
-Filename: django_bootstrap_colors-5.2.2.dist-info/METADATA
+Filename: django_bootstrap_colors-5.3.0.dist-info/METADATA
 Comment: 
 
-Filename: django_bootstrap_colors-5.2.2.dist-info/WHEEL
+Filename: django_bootstrap_colors-5.3.0.dist-info/WHEEL
 Comment: 
 
-Filename: django_bootstrap_colors-5.2.2.dist-info/top_level.txt
+Filename: django_bootstrap_colors-5.3.0.dist-info/top_level.txt
 Comment: 
 
-Filename: django_bootstrap_colors-5.2.2.dist-info/RECORD
+Filename: django_bootstrap_colors-5.3.0.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## bootstrap_colors/templates/bootstrap_colors.css

```diff
@@ -1,13 +1,20 @@
 :root {
     --bs-primary: {{ BOOTSTRAP_THEME_COLORS.0 }};
     --bs-link-color: {{ BOOTSTRAP_THEME_COLORS.0 }};
     --bs-link-hover-color: {{ BOOTSTRAP_THEME_COLORS.2 }};
 }
 
+a {
+    color: var(--bs-link-color);
+}
+a:hover {
+    color: var(--bs-link-hover-color);
+}
+
 .text-bg-primary {
     background-color: {{ BOOTSTRAP_THEME_COLORS.0 }} !important;
 }
 
 .btn-primary {
     --bs-btn-bg: {{ BOOTSTRAP_THEME_COLORS.0 }};
     --bs-btn-border-color: {{ BOOTSTRAP_THEME_COLORS.0 }};
```

## Comparing `django_bootstrap_colors-5.2.2.dist-info/LICENSE` & `django_bootstrap_colors-5.3.0.dist-info/LICENSE`

 * *Files identical despite different names*

## Comparing `django_bootstrap_colors-5.2.2.dist-info/METADATA` & `django_bootstrap_colors-5.3.0.dist-info/METADATA`

 * *Files 17% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: django-bootstrap-colors
-Version: 5.2.2
+Version: 5.3.0
 Summary: UNKNOWN
 Home-page: https://git.mpib-berlin.mpg.de/castellum/django-bootstrap-colors
 Author: Max-Planck-Gesellschaft
 License: MIT
 Platform: UNKNOWN
 Description-Content-Type: text/markdown
 License-File: LICENSE
@@ -16,14 +16,16 @@
 
 -   Add `bootstrap_colors` to `INSTALLED_APPS`
 -   Add `path('colors.css', BootstrapColorsView.as_view(), name='colors')` to
     `urls.py`
 -   Add `<link rel="stylesheet" type="text/css" href="{% url 'colors' %}">` to
     your template
 -   Set `BOOTSTRAP_THEME_COLORS` (Default: `['#0d6efd', '#0b5ed7', '#0a58ca']`)
+-   Optional: Configure caching, e.g. by using
+    `django.views.decorators.cache.cache_control`
 
 # Alternatives
 
 Bootstrap provides several ways to achieve this:
 
 -   **CSS custom properities**: It would be great if we could just change a few
     custom properties. Unfortunately they are not used in a way that would
```

## Comparing `django_bootstrap_colors-5.2.2.dist-info/RECORD` & `django_bootstrap_colors-5.3.0.dist-info/RECORD`

 * *Files 13% similar despite different names*

```diff
@@ -1,8 +1,8 @@
 bootstrap_colors/__init__.py,sha256=47DEQpj8HBSa-_TImW-5JCeuQeRkm5NMpJWZG3hSuFU,0
 bootstrap_colors/views.py,sha256=8ZOPNfkyZWTYz6BIlwGAGfRLPbBAUtwhsQ5ahOCzthY,464
-bootstrap_colors/templates/bootstrap_colors.css,sha256=HBRqKst05pET74i66wpBvek3KmdoZosERxA99BIqwqY,1722
-django_bootstrap_colors-5.2.2.dist-info/LICENSE,sha256=2PyjqrEsgnfGJ45bh-MInPp6o71wQ6QxjCODf4ufXAM,1065
-django_bootstrap_colors-5.2.2.dist-info/METADATA,sha256=4tGELzPBzYlGvmQEtBiOEjHObfhI9G1rJQ7ElkP01VM,1206
-django_bootstrap_colors-5.2.2.dist-info/WHEEL,sha256=G16H4A3IeoQmnOrYV4ueZGKSjhipXx8zc8nu9FGlvMA,92
-django_bootstrap_colors-5.2.2.dist-info/top_level.txt,sha256=EVK2cCc-6-m3DIbl6jIVv0O2p-ZH7DZUwK2ZkFK0tHA,17
-django_bootstrap_colors-5.2.2.dist-info/RECORD,,
+bootstrap_colors/templates/bootstrap_colors.css,sha256=r0l6rfYwgTC9Nj1WYvPFMWTGa-3sUb-aT0O5XAcs1w4,1813
+django_bootstrap_colors-5.3.0.dist-info/LICENSE,sha256=2PyjqrEsgnfGJ45bh-MInPp6o71wQ6QxjCODf4ufXAM,1065
+django_bootstrap_colors-5.3.0.dist-info/METADATA,sha256=GpYVJ1zoe2ScyjVQ8aIY172NkO-OBJe5o86mvXxknuM,1303
+django_bootstrap_colors-5.3.0.dist-info/WHEEL,sha256=G16H4A3IeoQmnOrYV4ueZGKSjhipXx8zc8nu9FGlvMA,92
+django_bootstrap_colors-5.3.0.dist-info/top_level.txt,sha256=EVK2cCc-6-m3DIbl6jIVv0O2p-ZH7DZUwK2ZkFK0tHA,17
+django_bootstrap_colors-5.3.0.dist-info/RECORD,,
```

