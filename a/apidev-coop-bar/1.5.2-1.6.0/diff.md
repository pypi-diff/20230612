# Comparing `tmp/apidev-coop_bar-1.5.2.tar.gz` & `tmp/apidev-coop_bar-1.6.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/apidev-coop_bar-1.5.2.tar", last modified: Thu Nov 14 22:00:41 2019, max compression
+gzip compressed data, was "apidev-coop_bar-1.6.0.tar", last modified: Mon Jun 12 12:54:32 2023, max compression
```

## Comparing `apidev-coop_bar-1.5.2.tar` & `apidev-coop_bar-1.6.0.tar`

### file list

```diff
@@ -1,31 +1,26 @@
-drwxr-xr-x   0 lucjean    (501) staff       (20)        0 2019-11-14 22:00:41.000000 apidev-coop_bar-1.5.2/
--rw-r--r--   0 lucjean    (501) staff       (20)      243 2019-08-29 13:03:06.000000 apidev-coop_bar-1.5.2/MANIFEST.in
--rw-r--r--   0 lucjean    (501) staff       (20)     3407 2019-11-14 22:00:41.000000 apidev-coop_bar-1.5.2/PKG-INFO
--rwxr-xr-x   0 lucjean    (501) staff       (20)     2072 2019-08-29 13:03:06.000000 apidev-coop_bar-1.5.2/README.rst
-drwxr-xr-x   0 lucjean    (501) staff       (20)        0 2019-11-14 22:00:40.000000 apidev-coop_bar-1.5.2/apidev_coop_bar.egg-info/
--rw-r--r--   0 lucjean    (501) staff       (20)     3407 2019-11-14 22:00:39.000000 apidev-coop_bar-1.5.2/apidev_coop_bar.egg-info/PKG-INFO
--rw-r--r--   0 lucjean    (501) staff       (20)      615 2019-11-14 22:00:40.000000 apidev-coop_bar-1.5.2/apidev_coop_bar.egg-info/SOURCES.txt
--rw-r--r--   0 lucjean    (501) staff       (20)      484 2019-08-29 14:49:29.000000 apidev-coop_bar-1.5.2/apidev_coop_bar.egg-info/SOURCES.txt.py
--rw-r--r--   0 lucjean    (501) staff       (20)        1 2019-11-14 22:00:39.000000 apidev-coop_bar-1.5.2/apidev_coop_bar.egg-info/dependency_links.txt
--rw-r--r--   0 lucjean    (501) staff       (20)        1 2019-08-29 14:49:29.000000 apidev-coop_bar-1.5.2/apidev_coop_bar.egg-info/dependency_links.txt.py
--rw-r--r--   0 lucjean    (501) staff       (20)        1 2019-08-29 13:12:17.000000 apidev-coop_bar-1.5.2/apidev_coop_bar.egg-info/not-zip-safe
--rw-r--r--   0 lucjean    (501) staff       (20)        9 2019-11-14 22:00:39.000000 apidev-coop_bar-1.5.2/apidev_coop_bar.egg-info/top_level.txt
--rw-r--r--   0 lucjean    (501) staff       (20)        9 2019-08-29 14:49:29.000000 apidev-coop_bar-1.5.2/apidev_coop_bar.egg-info/top_level.txt.py
-drwxr-xr-x   0 lucjean    (501) staff       (20)        0 2019-11-14 22:00:40.000000 apidev-coop_bar-1.5.2/coop_bar/
--rwxr-xr-x   0 lucjean    (501) staff       (20)      270 2019-11-14 21:59:33.000000 apidev-coop_bar-1.5.2/coop_bar/__init__.py
--rw-r--r--   0 lucjean    (501) staff       (20)      218 2019-08-29 13:03:06.000000 apidev-coop_bar-1.5.2/coop_bar/apps.py
--rw-r--r--   0 lucjean    (501) staff       (20)     3796 2019-08-29 13:03:06.000000 apidev-coop_bar-1.5.2/coop_bar/bar.py
-drwxr-xr-x   0 lucjean    (501) staff       (20)        0 2019-11-14 22:00:40.000000 apidev-coop_bar-1.5.2/coop_bar/static/
-drwxr-xr-x   0 lucjean    (501) staff       (20)        0 2019-11-14 22:00:40.000000 apidev-coop_bar-1.5.2/coop_bar/static/css/
--rw-r--r--   0 lucjean    (501) staff       (20)     1998 2019-08-29 13:03:06.000000 apidev-coop_bar-1.5.2/coop_bar/static/css/coop_bar.css
-drwxr-xr-x   0 lucjean    (501) staff       (20)        0 2019-11-14 22:00:41.000000 apidev-coop_bar-1.5.2/coop_bar/static/js/
--rwxr-xr-x   0 lucjean    (501) staff       (20)     2657 2019-08-29 13:03:06.000000 apidev-coop_bar-1.5.2/coop_bar/static/js/humanmsg.js
-drwxr-xr-x   0 lucjean    (501) staff       (20)        0 2019-11-14 22:00:41.000000 apidev-coop_bar-1.5.2/coop_bar/templates/
--rwxr-xr-x   0 lucjean    (501) staff       (20)      372 2019-08-29 13:03:06.000000 apidev-coop_bar-1.5.2/coop_bar/templates/coop_bar.html
-drwxr-xr-x   0 lucjean    (501) staff       (20)        0 2019-11-14 22:00:41.000000 apidev-coop_bar-1.5.2/coop_bar/templatetags/
--rwxr-xr-x   0 lucjean    (501) staff       (20)       25 2019-08-29 13:03:06.000000 apidev-coop_bar-1.5.2/coop_bar/templatetags/__init__.py
--rw-r--r--   0 lucjean    (501) staff       (20)     1987 2019-11-14 20:40:18.000000 apidev-coop_bar-1.5.2/coop_bar/templatetags/coop_bar_tags.py
--rwxr-xr-x   0 lucjean    (501) staff       (20)      152 2019-08-29 13:03:06.000000 apidev-coop_bar-1.5.2/coop_bar/urls.py
--rw-r--r--   0 lucjean    (501) staff       (20)     1119 2019-08-29 16:49:41.000000 apidev-coop_bar-1.5.2/coop_bar/utils.py
--rw-r--r--   0 lucjean    (501) staff       (20)       38 2019-11-14 22:00:41.000000 apidev-coop_bar-1.5.2/setup.cfg
--rw-r--r--   0 lucjean    (501) staff       (20)     1362 2019-08-29 13:03:06.000000 apidev-coop_bar-1.5.2/setup.py
+drwxrwxr-x   0 lucjean   (1001) lucjean   (1001)        0 2023-06-12 12:54:32.463626 apidev-coop_bar-1.6.0/
+-rw-rw-r--   0 lucjean   (1001) lucjean   (1001)      243 2023-05-22 07:02:21.000000 apidev-coop_bar-1.6.0/MANIFEST.in
+-rw-rw-r--   0 lucjean   (1001) lucjean   (1001)     2872 2023-06-12 12:54:32.463626 apidev-coop_bar-1.6.0/PKG-INFO
+-rwxrwxr-x   0 lucjean   (1001) lucjean   (1001)     2072 2023-05-22 07:02:21.000000 apidev-coop_bar-1.6.0/README.rst
+drwxrwxr-x   0 lucjean   (1001) lucjean   (1001)        0 2023-06-12 12:54:32.463626 apidev-coop_bar-1.6.0/apidev_coop_bar.egg-info/
+-rw-rw-r--   0 lucjean   (1001) lucjean   (1001)     2872 2023-06-12 12:54:32.000000 apidev-coop_bar-1.6.0/apidev_coop_bar.egg-info/PKG-INFO
+-rw-rw-r--   0 lucjean   (1001) lucjean   (1001)      453 2023-06-12 12:54:32.000000 apidev-coop_bar-1.6.0/apidev_coop_bar.egg-info/SOURCES.txt
+-rw-rw-r--   0 lucjean   (1001) lucjean   (1001)        1 2023-06-12 12:54:32.000000 apidev-coop_bar-1.6.0/apidev_coop_bar.egg-info/dependency_links.txt
+-rw-rw-r--   0 lucjean   (1001) lucjean   (1001)        1 2023-05-22 10:13:33.000000 apidev-coop_bar-1.6.0/apidev_coop_bar.egg-info/not-zip-safe
+-rw-rw-r--   0 lucjean   (1001) lucjean   (1001)        9 2023-06-12 12:54:32.000000 apidev-coop_bar-1.6.0/apidev_coop_bar.egg-info/top_level.txt
+drwxrwxr-x   0 lucjean   (1001) lucjean   (1001)        0 2023-06-12 12:54:32.463626 apidev-coop_bar-1.6.0/coop_bar/
+-rwxrwxr-x   0 lucjean   (1001) lucjean   (1001)      230 2023-06-12 12:49:28.000000 apidev-coop_bar-1.6.0/coop_bar/__init__.py
+-rw-rw-r--   0 lucjean   (1001) lucjean   (1001)      178 2023-06-12 12:49:28.000000 apidev-coop_bar-1.6.0/coop_bar/apps.py
+-rw-rw-r--   0 lucjean   (1001) lucjean   (1001)     3869 2023-06-12 12:49:28.000000 apidev-coop_bar-1.6.0/coop_bar/bar.py
+drwxrwxr-x   0 lucjean   (1001) lucjean   (1001)        0 2023-06-12 12:54:32.459626 apidev-coop_bar-1.6.0/coop_bar/static/
+drwxrwxr-x   0 lucjean   (1001) lucjean   (1001)        0 2023-06-12 12:54:32.463626 apidev-coop_bar-1.6.0/coop_bar/static/css/
+-rw-rw-r--   0 lucjean   (1001) lucjean   (1001)     1998 2023-05-22 07:02:21.000000 apidev-coop_bar-1.6.0/coop_bar/static/css/coop_bar.css
+drwxrwxr-x   0 lucjean   (1001) lucjean   (1001)        0 2023-06-12 12:54:32.463626 apidev-coop_bar-1.6.0/coop_bar/templates/
+-rwxrwxr-x   0 lucjean   (1001) lucjean   (1001)      372 2023-05-22 07:02:21.000000 apidev-coop_bar-1.6.0/coop_bar/templates/coop_bar.html
+drwxrwxr-x   0 lucjean   (1001) lucjean   (1001)        0 2023-06-12 12:54:32.463626 apidev-coop_bar-1.6.0/coop_bar/templatetags/
+-rwxrwxr-x   0 lucjean   (1001) lucjean   (1001)       25 2023-05-22 07:02:21.000000 apidev-coop_bar-1.6.0/coop_bar/templatetags/__init__.py
+-rw-rw-r--   0 lucjean   (1001) lucjean   (1001)     1926 2023-06-12 12:49:28.000000 apidev-coop_bar-1.6.0/coop_bar/templatetags/coop_bar_tags.py
+-rwxrwxr-x   0 lucjean   (1001) lucjean   (1001)      103 2023-06-12 12:49:28.000000 apidev-coop_bar-1.6.0/coop_bar/urls.py
+-rw-rw-r--   0 lucjean   (1001) lucjean   (1001)     1079 2023-06-12 12:49:28.000000 apidev-coop_bar-1.6.0/coop_bar/utils.py
+-rw-rw-r--   0 lucjean   (1001) lucjean   (1001)       38 2023-06-12 12:54:32.463626 apidev-coop_bar-1.6.0/setup.cfg
+-rw-rw-r--   0 lucjean   (1001) lucjean   (1001)     1328 2023-06-12 12:49:28.000000 apidev-coop_bar-1.6.0/setup.py
```

### filetype from file(1)

```diff
@@ -1 +1 @@
-POSIX tar archive (GNU)
+POSIX tar archive
```

### Comparing `apidev-coop_bar-1.5.2/PKG-INFO` & `apidev-coop_bar-1.6.0/PKG-INFO`

 * *Files 9% similar despite different names*

```diff
@@ -1,85 +1,84 @@
-Metadata-Version: 1.1
+Metadata-Version: 2.1
 Name: apidev-coop_bar
-Version: 1.5.2
+Version: 1.6.0
 Summary: Pluggable admin bar system , works well with coop_cms
 Home-page: https://github.com/ljean/coop-bar/
+Download-URL: https://github.com/ljean/coop-bar/tarball/master
 Author: Luc Jean
 Author-email: ljean@apidev.fr
 License: BSD
-Download-URL: https://github.com/ljean/coop-bar/tarball/master
-Description: apidev-coop_bar, configurable toolbar
-        ===============================================
-        
-        * `What is coop_bar good for?`_
-        * `Quick start`_
-        
-        .. _What is coop_bar good for?: #good-for
-        .. _Quick start?: #quick-start
-        
-        .. _good-for:
-        
-        What is coop_bar good for?
-        ------------------------------------
-        coop_bar is a django app which provides an menu bar with external auto-registred menu items.
-        
-        .. _quick-start:
-        
-        Quick start
-        ------------------------------------
-        In settings.py, add 'coop_bar' (with an underscore) to the INSTALLED_APPS 
-        In urls.py add (r'^coop_bar/', include('coop_bar.urls')) to your urlpatterns
-        
-        For each app needing to add links to coop_bar, create a coop_bar_cfg.py file
-        In this file, add a load_commands function as follows ::
-        
-            from django.core.urlresolvers import reverse
-            from django.utils.translation import ugettext as _
-            
-            def django_admin_command(request, context):
-                if request and request.user.is_staff: #request might be None
-                    return u'<a href="{0}">{1}</a>'.format(reverse("admin:index"), _('Admin'))
-            
-            def load_commands(coop_bar):
-                coop_bar.register_command(django_admin_command)
-            
-        
-        In load_commands, you can register as much callback functions as you want. A callback (django_admin_command in the previous example)
-        is just a function with request and context as args. It returns some html code to display in the bar or None.
-        
-        In your base.html, add the following template tags::
-        
-            {% load coop_bar_tags %}
-            <html>
-            <head>
-                ...
-                {% coop_bar_headers %}
-            </head>
-            <body>
-                ...
-                {% coop_bar %}
-            </body>
-        
-        
-        License
-        =======
-        
-        apidev-coop_bar in a fork of credis/coop-bar (see https://github.com/credis/coop-bar).
-        
-        `Fugue icon set <http://p.yusukekamiyamane.com/>`_  by Yusuke Kamiyamane. All rights reserved. Licensed under a Creative Commons Attribution 3.0 License.
-        
-        apidev-coop_bar itself uses the BSD license: see license.txt
-        
-        credis/coop-bar development was funded by `CREDIS <http://credis.org/>`_, FSE (European Social Fund) and Conseil Regional d'Auvergne.
-        
-Platform: UNKNOWN
 Classifier: Development Status :: 4 - Beta
 Classifier: Environment :: Web Environment
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: BSD License
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python
 Classifier: Framework :: Django
 Classifier: Natural Language :: English
 Classifier: Natural Language :: French
 Classifier: Topic :: Internet :: WWW/HTTP :: Dynamic Content
 Classifier: Topic :: Internet :: WWW/HTTP :: WSGI :: Application
+
+apidev-coop_bar, configurable toolbar
+===============================================
+
+* `What is coop_bar good for?`_
+* `Quick start`_
+
+.. _What is coop_bar good for?: #good-for
+.. _Quick start?: #quick-start
+
+.. _good-for:
+
+What is coop_bar good for?
+------------------------------------
+coop_bar is a django app which provides an menu bar with external auto-registred menu items.
+
+.. _quick-start:
+
+Quick start
+------------------------------------
+In settings.py, add 'coop_bar' (with an underscore) to the INSTALLED_APPS 
+In urls.py add (r'^coop_bar/', include('coop_bar.urls')) to your urlpatterns
+
+For each app needing to add links to coop_bar, create a coop_bar_cfg.py file
+In this file, add a load_commands function as follows ::
+
+    from django.core.urlresolvers import reverse
+    from django.utils.translation import ugettext as _
+    
+    def django_admin_command(request, context):
+        if request and request.user.is_staff: #request might be None
+            return u'<a href="{0}">{1}</a>'.format(reverse("admin:index"), _('Admin'))
+    
+    def load_commands(coop_bar):
+        coop_bar.register_command(django_admin_command)
+    
+
+In load_commands, you can register as much callback functions as you want. A callback (django_admin_command in the previous example)
+is just a function with request and context as args. It returns some html code to display in the bar or None.
+
+In your base.html, add the following template tags::
+
+    {% load coop_bar_tags %}
+    <html>
+    <head>
+        ...
+        {% coop_bar_headers %}
+    </head>
+    <body>
+        ...
+        {% coop_bar %}
+    </body>
+
+
+License
+=======
+
+apidev-coop_bar in a fork of credis/coop-bar (see https://github.com/credis/coop-bar).
+
+`Fugue icon set <http://p.yusukekamiyamane.com/>`_  by Yusuke Kamiyamane. All rights reserved. Licensed under a Creative Commons Attribution 3.0 License.
+
+apidev-coop_bar itself uses the BSD license: see license.txt
+
+credis/coop-bar development was funded by `CREDIS <http://credis.org/>`_, FSE (European Social Fund) and Conseil Regional d'Auvergne.
```

### Comparing `apidev-coop_bar-1.5.2/README.rst` & `apidev-coop_bar-1.6.0/README.rst`

 * *Files identical despite different names*

### Comparing `apidev-coop_bar-1.5.2/apidev_coop_bar.egg-info/PKG-INFO` & `apidev-coop_bar-1.6.0/apidev_coop_bar.egg-info/PKG-INFO`

 * *Files 9% similar despite different names*

```diff
@@ -1,85 +1,84 @@
-Metadata-Version: 1.1
+Metadata-Version: 2.1
 Name: apidev-coop-bar
-Version: 1.5.2
+Version: 1.6.0
 Summary: Pluggable admin bar system , works well with coop_cms
 Home-page: https://github.com/ljean/coop-bar/
+Download-URL: https://github.com/ljean/coop-bar/tarball/master
 Author: Luc Jean
 Author-email: ljean@apidev.fr
 License: BSD
-Download-URL: https://github.com/ljean/coop-bar/tarball/master
-Description: apidev-coop_bar, configurable toolbar
-        ===============================================
-        
-        * `What is coop_bar good for?`_
-        * `Quick start`_
-        
-        .. _What is coop_bar good for?: #good-for
-        .. _Quick start?: #quick-start
-        
-        .. _good-for:
-        
-        What is coop_bar good for?
-        ------------------------------------
-        coop_bar is a django app which provides an menu bar with external auto-registred menu items.
-        
-        .. _quick-start:
-        
-        Quick start
-        ------------------------------------
-        In settings.py, add 'coop_bar' (with an underscore) to the INSTALLED_APPS 
-        In urls.py add (r'^coop_bar/', include('coop_bar.urls')) to your urlpatterns
-        
-        For each app needing to add links to coop_bar, create a coop_bar_cfg.py file
-        In this file, add a load_commands function as follows ::
-        
-            from django.core.urlresolvers import reverse
-            from django.utils.translation import ugettext as _
-            
-            def django_admin_command(request, context):
-                if request and request.user.is_staff: #request might be None
-                    return u'<a href="{0}">{1}</a>'.format(reverse("admin:index"), _('Admin'))
-            
-            def load_commands(coop_bar):
-                coop_bar.register_command(django_admin_command)
-            
-        
-        In load_commands, you can register as much callback functions as you want. A callback (django_admin_command in the previous example)
-        is just a function with request and context as args. It returns some html code to display in the bar or None.
-        
-        In your base.html, add the following template tags::
-        
-            {% load coop_bar_tags %}
-            <html>
-            <head>
-                ...
-                {% coop_bar_headers %}
-            </head>
-            <body>
-                ...
-                {% coop_bar %}
-            </body>
-        
-        
-        License
-        =======
-        
-        apidev-coop_bar in a fork of credis/coop-bar (see https://github.com/credis/coop-bar).
-        
-        `Fugue icon set <http://p.yusukekamiyamane.com/>`_  by Yusuke Kamiyamane. All rights reserved. Licensed under a Creative Commons Attribution 3.0 License.
-        
-        apidev-coop_bar itself uses the BSD license: see license.txt
-        
-        credis/coop-bar development was funded by `CREDIS <http://credis.org/>`_, FSE (European Social Fund) and Conseil Regional d'Auvergne.
-        
-Platform: UNKNOWN
 Classifier: Development Status :: 4 - Beta
 Classifier: Environment :: Web Environment
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: BSD License
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python
 Classifier: Framework :: Django
 Classifier: Natural Language :: English
 Classifier: Natural Language :: French
 Classifier: Topic :: Internet :: WWW/HTTP :: Dynamic Content
 Classifier: Topic :: Internet :: WWW/HTTP :: WSGI :: Application
+
+apidev-coop_bar, configurable toolbar
+===============================================
+
+* `What is coop_bar good for?`_
+* `Quick start`_
+
+.. _What is coop_bar good for?: #good-for
+.. _Quick start?: #quick-start
+
+.. _good-for:
+
+What is coop_bar good for?
+------------------------------------
+coop_bar is a django app which provides an menu bar with external auto-registred menu items.
+
+.. _quick-start:
+
+Quick start
+------------------------------------
+In settings.py, add 'coop_bar' (with an underscore) to the INSTALLED_APPS 
+In urls.py add (r'^coop_bar/', include('coop_bar.urls')) to your urlpatterns
+
+For each app needing to add links to coop_bar, create a coop_bar_cfg.py file
+In this file, add a load_commands function as follows ::
+
+    from django.core.urlresolvers import reverse
+    from django.utils.translation import ugettext as _
+    
+    def django_admin_command(request, context):
+        if request and request.user.is_staff: #request might be None
+            return u'<a href="{0}">{1}</a>'.format(reverse("admin:index"), _('Admin'))
+    
+    def load_commands(coop_bar):
+        coop_bar.register_command(django_admin_command)
+    
+
+In load_commands, you can register as much callback functions as you want. A callback (django_admin_command in the previous example)
+is just a function with request and context as args. It returns some html code to display in the bar or None.
+
+In your base.html, add the following template tags::
+
+    {% load coop_bar_tags %}
+    <html>
+    <head>
+        ...
+        {% coop_bar_headers %}
+    </head>
+    <body>
+        ...
+        {% coop_bar %}
+    </body>
+
+
+License
+=======
+
+apidev-coop_bar in a fork of credis/coop-bar (see https://github.com/credis/coop-bar).
+
+`Fugue icon set <http://p.yusukekamiyamane.com/>`_  by Yusuke Kamiyamane. All rights reserved. Licensed under a Creative Commons Attribution 3.0 License.
+
+apidev-coop_bar itself uses the BSD license: see license.txt
+
+credis/coop-bar development was funded by `CREDIS <http://credis.org/>`_, FSE (European Social Fund) and Conseil Regional d'Auvergne.
```

### Comparing `apidev-coop_bar-1.5.2/coop_bar/bar.py` & `apidev-coop_bar-1.6.0/coop_bar/bar.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,11 +1,9 @@
 # -*- coding: utf-8 -*-
 
-from __future__ import unicode_literals
-
 from importlib import import_module
 
 from django.conf import settings
 
 
 class CoopBar:
     """The main class"""
@@ -23,20 +21,23 @@
             if coop_bar_modules:
                 for module_name in coop_bar_modules:
                     try:
                         app_admin_bar_module = import_module(module_name)
                         loader_fct = getattr(app_admin_bar_module, 'load_commands')
                         loader_fct(self)
                     except ImportError as msg:
-                        raise ImportError("coop_bar : error while loading '{0}': {1}".format(module_name, msg))
+                        text = "coop_bar : error while loading '{0}': {1}".format(module_name, msg)
+                        raise ImportError(text)
+                    except Exception as msg2:
+                        raise
             else:
                 for app in settings.INSTALLED_APPS:
                     try:
                         # load dynamically the admin_bar module of all apps
-                        app_admin_bar_module = import_module(app+'.coop_bar_cfg')
+                        app_admin_bar_module = import_module(app + '.coop_bar_cfg')
                         if hasattr(app_admin_bar_module, 'load_commands'):
                             # call the load_commands function in this module
                             # This function should call the AdminBar:register_command for
                             # every item it want to insert in the bar
                             loader_fct = getattr(app_admin_bar_module, 'load_commands')
                             loader_fct(self)
                     except ImportError as msg:
```

### Comparing `apidev-coop_bar-1.5.2/coop_bar/static/css/coop_bar.css` & `apidev-coop_bar-1.6.0/coop_bar/static/css/coop_bar.css`

 * *Files identical despite different names*

### Comparing `apidev-coop_bar-1.5.2/coop_bar/templatetags/coop_bar_tags.py` & `apidev-coop_bar-1.6.0/coop_bar/templatetags/coop_bar_tags.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,19 +1,17 @@
 # -*- coding: utf-8 -*-
 
-from __future__ import unicode_literals
-
 from django import template
 from django.conf import settings
 from django.template.loader import get_template
 from django.utils.safestring import mark_safe
 
-from coop_bar import get_version
-from coop_bar.bar import CoopBar
-from coop_bar.utils import context_to_dict
+from .. import get_version
+from ..bar import CoopBar
+from ..utils import context_to_dict
 
 register = template.Library()
 
 
 class CoopBarNode(template.Node):
 
     def render(self, context):
```

### Comparing `apidev-coop_bar-1.5.2/coop_bar/utils.py` & `apidev-coop_bar-1.6.0/coop_bar/utils.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,11 +1,9 @@
 # -*- coding: utf-8 -*-
 
-from __future__ import unicode_literals
-
 from django.conf import settings
 
 
 def make_link(url, label, icon, id=None, classes=None):
     """make a link"""
     icon_url = icon
     extra_args = ['id="{0}"'.format(id)] if id else []
@@ -30,8 +28,8 @@
 
 
 def context_to_dict(context):
     """convert a django context to a dict"""
     the_dict = {}
     for elt in context:
         the_dict.update(dict(elt))
-    return the_dict
+    return the_dict
```

### Comparing `apidev-coop_bar-1.5.2/setup.py` & `apidev-coop_bar-1.6.0/setup.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,25 +1,23 @@
 # -*- coding: utf-8 -*-
 
-from __future__ import unicode_literals
-
 import os
 
 try:
     from setuptools import setup, find_packages
 except ImportError:
     import ez_setup
     ez_setup.use_setuptools()
     from setuptools import setup, find_packages
 
 VERSION = __import__('coop_bar').__version__
 
 
-def read(fname):
-    return open(os.path.join(os.path.dirname(__file__), fname)).read()
+def read(file_name):
+    return open(os.path.join(os.path.dirname(__file__), file_name)).read()
 
 
 setup(
     name='apidev-coop_bar',
     version=VERSION,
     description='Pluggable admin bar system , works well with coop_cms',
     long_description=open('README.rst').read(),
@@ -41,8 +39,7 @@
         'Framework :: Django',
         'Natural Language :: English',
         'Natural Language :: French',
         'Topic :: Internet :: WWW/HTTP :: Dynamic Content',
         'Topic :: Internet :: WWW/HTTP :: WSGI :: Application',
     ],
 )
-
```

