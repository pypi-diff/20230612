# Comparing `tmp/apidev-coop_colorbox-1.5.1.tar.gz` & `tmp/apidev-coop_colorbox-1.6.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/apidev-coop_colorbox-1.5.1.tar", last modified: Fri Aug 30 10:36:16 2019, max compression
+gzip compressed data, was "apidev-coop_colorbox-1.6.0.tar", last modified: Mon Jun 12 12:53:56 2023, max compression
```

## Comparing `apidev-coop_colorbox-1.5.1.tar` & `apidev-coop_colorbox-1.6.0.tar`

### file list

```diff
@@ -1,89 +1,86 @@
-drwxr-xr-x   0 lucjean    (501) staff       (20)        0 2019-08-30 10:36:16.000000 apidev-coop_colorbox-1.5.1/
--rw-r--r--   0 lucjean    (501) staff       (20)     3953 2019-08-30 10:36:16.000000 apidev-coop_colorbox-1.5.1/PKG-INFO
--rw-r--r--   0 lucjean    (501) staff       (20)       93 2019-08-29 13:07:27.000000 apidev-coop_colorbox-1.5.1/MANIFEST.in
-drwxr-xr-x   0 lucjean    (501) staff       (20)        0 2019-08-30 10:36:13.000000 apidev-coop_colorbox-1.5.1/colorbox/
--rwxr-xr-x   0 lucjean    (501) staff       (20)      256 2019-08-30 10:27:45.000000 apidev-coop_colorbox-1.5.1/colorbox/__init__.py
--rw-r--r--   0 lucjean    (501) staff       (20)      203 2019-08-29 13:07:27.000000 apidev-coop_colorbox-1.5.1/colorbox/apps.py
--rwxr-xr-x   0 lucjean    (501) staff       (20)      258 2019-08-29 13:07:27.000000 apidev-coop_colorbox-1.5.1/colorbox/forms.py
--rwxr-xr-x   0 lucjean    (501) staff       (20)     1170 2019-08-29 13:07:27.000000 apidev-coop_colorbox-1.5.1/colorbox/utils.py
-drwxr-xr-x   0 lucjean    (501) staff       (20)        0 2019-08-30 10:36:13.000000 apidev-coop_colorbox-1.5.1/colorbox/static/
-drwxr-xr-x   0 lucjean    (501) staff       (20)        0 2019-08-30 10:36:13.000000 apidev-coop_colorbox-1.5.1/colorbox/static/css/
--rwxr-xr-x   0 lucjean    (501) staff       (20)     3874 2019-08-29 13:07:27.000000 apidev-coop_colorbox-1.5.1/colorbox/static/css/colorbox.css
-drwxr-xr-x   0 lucjean    (501) staff       (20)        0 2019-08-30 10:36:14.000000 apidev-coop_colorbox-1.5.1/colorbox/static/css/images/
--rwxr-xr-x   0 lucjean    (501) staff       (20)      112 2019-08-29 13:07:27.000000 apidev-coop_colorbox-1.5.1/colorbox/static/css/images/border.png
--rwxr-xr-x   0 lucjean    (501) staff       (20)     9427 2019-08-29 13:07:27.000000 apidev-coop_colorbox-1.5.1/colorbox/static/css/images/loading.gif
-drwxr-xr-x   0 lucjean    (501) staff       (20)        0 2019-08-30 10:36:14.000000 apidev-coop_colorbox-1.5.1/colorbox/static/css/images/ie6/
--rwxr-xr-x   0 lucjean    (501) staff       (20)      215 2019-08-29 13:07:27.000000 apidev-coop_colorbox-1.5.1/colorbox/static/css/images/ie6/borderBottomLeft.png
--rwxr-xr-x   0 lucjean    (501) staff       (20)      214 2019-08-29 13:07:27.000000 apidev-coop_colorbox-1.5.1/colorbox/static/css/images/ie6/borderTopRight.png
--rwxr-xr-x   0 lucjean    (501) staff       (20)      108 2019-08-29 13:07:27.000000 apidev-coop_colorbox-1.5.1/colorbox/static/css/images/ie6/borderMiddleLeft.png
--rwxr-xr-x   0 lucjean    (501) staff       (20)      111 2019-08-29 13:07:27.000000 apidev-coop_colorbox-1.5.1/colorbox/static/css/images/ie6/borderTopCenter.png
--rwxr-xr-x   0 lucjean    (501) staff       (20)      108 2019-08-29 13:07:27.000000 apidev-coop_colorbox-1.5.1/colorbox/static/css/images/ie6/borderMiddleRight.png
--rwxr-xr-x   0 lucjean    (501) staff       (20)      111 2019-08-29 13:07:27.000000 apidev-coop_colorbox-1.5.1/colorbox/static/css/images/ie6/borderBottomCenter.png
--rwxr-xr-x   0 lucjean    (501) staff       (20)      217 2019-08-29 13:07:27.000000 apidev-coop_colorbox-1.5.1/colorbox/static/css/images/ie6/borderBottomRight.png
--rwxr-xr-x   0 lucjean    (501) staff       (20)      216 2019-08-29 13:07:27.000000 apidev-coop_colorbox-1.5.1/colorbox/static/css/images/ie6/borderTopLeft.png
--rwxr-xr-x   0 lucjean    (501) staff       (20)      182 2019-08-29 13:07:27.000000 apidev-coop_colorbox-1.5.1/colorbox/static/css/images/overlay.png
--rwxr-xr-x   0 lucjean    (501) staff       (20)     2893 2019-08-29 13:07:27.000000 apidev-coop_colorbox-1.5.1/colorbox/static/css/images/controls.png
--rwxr-xr-x   0 lucjean    (501) staff       (20)      157 2019-08-29 13:07:27.000000 apidev-coop_colorbox-1.5.1/colorbox/static/css/images/loading_background.png
-drwxr-xr-x   0 lucjean    (501) staff       (20)        0 2019-08-30 10:36:14.000000 apidev-coop_colorbox-1.5.1/colorbox/static/js/
--rwxr-xr-x   0 lucjean    (501) staff       (20)    11885 2019-08-29 13:07:27.000000 apidev-coop_colorbox-1.5.1/colorbox/static/js/jquery.colorbox-min.js
--rwxr-xr-x   0 lucjean    (501) staff       (20)    29080 2019-08-29 13:07:27.000000 apidev-coop_colorbox-1.5.1/colorbox/static/js/jquery.colorbox.js
--rwxr-xr-x   0 lucjean    (501) staff       (20)     3216 2019-08-29 13:07:27.000000 apidev-coop_colorbox-1.5.1/colorbox/static/js/colorbox.coop.js
-drwxr-xr-x   0 lucjean    (501) staff       (20)        0 2019-08-30 10:36:15.000000 apidev-coop_colorbox-1.5.1/colorbox/static/js/i18n/
--rwxr-xr-x   0 lucjean    (501) staff       (20)      391 2019-08-29 13:07:27.000000 apidev-coop_colorbox-1.5.1/colorbox/static/js/i18n/jquery.colorbox-id.js
--rwxr-xr-x   0 lucjean    (501) staff       (20)      858 2019-08-29 13:07:27.000000 apidev-coop_colorbox-1.5.1/colorbox/static/js/i18n/jquery.colorbox-my.js
--rwxr-xr-x   0 lucjean    (501) staff       (20)      480 2019-08-29 13:07:27.000000 apidev-coop_colorbox-1.5.1/colorbox/static/js/i18n/jquery.colorbox-ja.js
--rwxr-xr-x   0 lucjean    (501) staff       (20)      571 2019-08-29 13:07:27.000000 apidev-coop_colorbox-1.5.1/colorbox/static/js/i18n/jquery.colorbox-bg.js
--rwxr-xr-x   0 lucjean    (501) staff       (20)      446 2019-08-29 13:07:27.000000 apidev-coop_colorbox-1.5.1/colorbox/static/js/i18n/jquery.colorbox-he.js
--rwxr-xr-x   0 lucjean    (501) staff       (20)      450 2019-08-29 13:07:27.000000 apidev-coop_colorbox-1.5.1/colorbox/static/js/i18n/jquery.colorbox-kr.js
--rwxr-xr-x   0 lucjean    (501) staff       (20)      454 2019-08-29 13:07:27.000000 apidev-coop_colorbox-1.5.1/colorbox/static/js/i18n/jquery.colorbox-si.js
--rwxr-xr-x   0 lucjean    (501) staff       (20)      408 2019-08-29 13:07:27.000000 apidev-coop_colorbox-1.5.1/colorbox/static/js/i18n/jquery.colorbox-fi.js
--rwxr-xr-x   0 lucjean    (501) staff       (20)      443 2019-08-29 13:07:27.000000 apidev-coop_colorbox-1.5.1/colorbox/static/js/i18n/jquery.colorbox-hr.js
--rwxr-xr-x   0 lucjean    (501) staff       (20)      437 2019-08-29 13:07:27.000000 apidev-coop_colorbox-1.5.1/colorbox/static/js/i18n/jquery.colorbox-no.js
--rwxr-xr-x   0 lucjean    (501) staff       (20)      566 2019-08-29 13:07:27.000000 apidev-coop_colorbox-1.5.1/colorbox/static/js/i18n/jquery.colorbox-ru.js
--rwxr-xr-x   0 lucjean    (501) staff       (20)      388 2019-08-29 13:07:27.000000 apidev-coop_colorbox-1.5.1/colorbox/static/js/i18n/jquery.colorbox-et.js
--rwxr-xr-x   0 lucjean    (501) staff       (20)      323 2019-08-29 13:07:27.000000 apidev-coop_colorbox-1.5.1/colorbox/static/js/i18n/jquery.colorbox-gl.js
--rwxr-xr-x   0 lucjean    (501) staff       (20)      479 2019-08-29 13:07:27.000000 apidev-coop_colorbox-1.5.1/colorbox/static/js/i18n/jquery.colorbox-pl.js
--rwxr-xr-x   0 lucjean    (501) staff       (20)      459 2019-08-29 13:07:27.000000 apidev-coop_colorbox-1.5.1/colorbox/static/js/i18n/jquery.colorbox-lv.js
--rwxr-xr-x   0 lucjean    (501) staff       (20)      472 2019-08-29 13:07:27.000000 apidev-coop_colorbox-1.5.1/colorbox/static/js/i18n/jquery.colorbox-ro.js
--rwxr-xr-x   0 lucjean    (501) staff       (20)      498 2019-08-29 13:07:27.000000 apidev-coop_colorbox-1.5.1/colorbox/static/js/i18n/jquery.colorbox-tr.js
--rwxr-xr-x   0 lucjean    (501) staff       (20)      482 2019-08-29 13:07:27.000000 apidev-coop_colorbox-1.5.1/colorbox/static/js/i18n/jquery.colorbox-ar.js
--rwxr-xr-x   0 lucjean    (501) staff       (20)      561 2019-08-29 13:07:27.000000 apidev-coop_colorbox-1.5.1/colorbox/static/js/i18n/jquery.colorbox-bn.js
--rwxr-xr-x   0 lucjean    (501) staff       (20)      334 2019-08-29 13:07:27.000000 apidev-coop_colorbox-1.5.1/colorbox/static/js/i18n/jquery.colorbox-es.js
--rwxr-xr-x   0 lucjean    (501) staff       (20)      439 2019-08-29 13:07:27.000000 apidev-coop_colorbox-1.5.1/colorbox/static/js/i18n/jquery.colorbox-it.js
--rwxr-xr-x   0 lucjean    (501) staff       (20)      437 2019-08-29 13:07:27.000000 apidev-coop_colorbox-1.5.1/colorbox/static/js/i18n/jquery.colorbox-sk.js
--rwxr-xr-x   0 lucjean    (501) staff       (20)      430 2019-08-29 13:07:27.000000 apidev-coop_colorbox-1.5.1/colorbox/static/js/i18n/jquery.colorbox-hu.js
--rwxr-xr-x   0 lucjean    (501) staff       (20)      507 2019-08-29 13:07:27.000000 apidev-coop_colorbox-1.5.1/colorbox/static/js/i18n/jquery.colorbox-sr.js
--rwxr-xr-x   0 lucjean    (501) staff       (20)      446 2019-08-29 13:07:27.000000 apidev-coop_colorbox-1.5.1/colorbox/static/js/i18n/jquery.colorbox-lt.js
--rwxr-xr-x   0 lucjean    (501) staff       (20)      412 2019-08-29 13:07:27.000000 apidev-coop_colorbox-1.5.1/colorbox/static/js/i18n/jquery.colorbox-sv.js
--rwxr-xr-x   0 lucjean    (501) staff       (20)      567 2019-08-29 13:07:27.000000 apidev-coop_colorbox-1.5.1/colorbox/static/js/i18n/jquery.colorbox-gr.js
--rwxr-xr-x   0 lucjean    (501) staff       (20)      458 2019-08-29 13:07:27.000000 apidev-coop_colorbox-1.5.1/colorbox/static/js/i18n/jquery.colorbox-cs.js
--rwxr-xr-x   0 lucjean    (501) staff       (20)      419 2019-08-29 13:07:27.000000 apidev-coop_colorbox-1.5.1/colorbox/static/js/i18n/jquery.colorbox-nl.js
--rwxr-xr-x   0 lucjean    (501) staff       (20)      470 2019-08-29 13:07:27.000000 apidev-coop_colorbox-1.5.1/colorbox/static/js/i18n/jquery.colorbox-fr.js
--rwxr-xr-x   0 lucjean    (501) staff       (20)      596 2019-08-29 13:07:27.000000 apidev-coop_colorbox-1.5.1/colorbox/static/js/i18n/jquery.colorbox-uk.js
--rwxr-xr-x   0 lucjean    (501) staff       (20)      725 2019-08-29 13:07:27.000000 apidev-coop_colorbox-1.5.1/colorbox/static/js/i18n/jquery.colorbox-fa.js
--rwxr-xr-x   0 lucjean    (501) staff       (20)      425 2019-08-29 13:07:27.000000 apidev-coop_colorbox-1.5.1/colorbox/static/js/i18n/jquery.colorbox-de.js
--rwxr-xr-x   0 lucjean    (501) staff       (20)      425 2019-08-29 13:07:27.000000 apidev-coop_colorbox-1.5.1/colorbox/static/js/i18n/jquery.colorbox-da.js
--rwxr-xr-x   0 lucjean    (501) staff       (20)      439 2019-08-29 13:07:27.000000 apidev-coop_colorbox-1.5.1/colorbox/static/js/i18n/jquery.colorbox-zh-CN.js
--rwxr-xr-x   0 lucjean    (501) staff       (20)      408 2019-08-29 13:07:27.000000 apidev-coop_colorbox-1.5.1/colorbox/static/js/i18n/jquery.colorbox-zh-TW.js
--rwxr-xr-x   0 lucjean    (501) staff       (20)      446 2019-08-29 13:07:27.000000 apidev-coop_colorbox-1.5.1/colorbox/static/js/i18n/jquery.colorbox-pt-BR.js
--rwxr-xr-x   0 lucjean    (501) staff       (20)      343 2019-08-29 13:07:27.000000 apidev-coop_colorbox-1.5.1/colorbox/static/js/i18n/jquery.colorbox-ca.js
--rwxr-xr-x   0 lucjean    (501) staff       (20)    44034 2019-08-29 13:07:27.000000 apidev-coop_colorbox-1.5.1/colorbox/static/js/jquery.form.js
--rwxr-xr-x   0 lucjean    (501) staff       (20)      886 2019-08-29 13:07:27.000000 apidev-coop_colorbox-1.5.1/colorbox/http.py
-drwxr-xr-x   0 lucjean    (501) staff       (20)        0 2019-08-30 10:36:13.000000 apidev-coop_colorbox-1.5.1/colorbox/templates/
-drwxr-xr-x   0 lucjean    (501) staff       (20)        0 2019-08-30 10:36:16.000000 apidev-coop_colorbox-1.5.1/colorbox/templates/colorbox/
--rwxr-xr-x   0 lucjean    (501) staff       (20)     1372 2019-08-29 13:07:27.000000 apidev-coop_colorbox-1.5.1/colorbox/templates/colorbox/popup_form_base.html
--rw-r--r--   0 lucjean    (501) staff       (20)      326 2019-08-29 13:07:27.000000 apidev-coop_colorbox-1.5.1/colorbox/templates/colorbox/popup_confirm.html
--rw-r--r--   0 lucjean    (501) staff       (20)     2475 2019-08-29 13:07:27.000000 apidev-coop_colorbox-1.5.1/colorbox/views.py
--rwxr-xr-x   0 lucjean    (501) staff       (20)     2378 2019-08-29 13:07:27.000000 apidev-coop_colorbox-1.5.1/colorbox/decorators.py
--rw-r--r--   0 lucjean    (501) staff       (20)     1290 2019-08-29 13:07:27.000000 apidev-coop_colorbox-1.5.1/setup.py
--rw-r--r--   0 lucjean    (501) staff       (20)       38 2019-08-30 10:36:16.000000 apidev-coop_colorbox-1.5.1/setup.cfg
--rwxr-xr-x   0 lucjean    (501) staff       (20)     2395 2019-08-30 10:35:46.000000 apidev-coop_colorbox-1.5.1/README.rst
-drwxr-xr-x   0 lucjean    (501) staff       (20)        0 2019-08-30 10:36:13.000000 apidev-coop_colorbox-1.5.1/apidev_coop_colorbox.egg-info/
--rw-r--r--   0 lucjean    (501) staff       (20)     3953 2019-08-30 10:36:12.000000 apidev-coop_colorbox-1.5.1/apidev_coop_colorbox.egg-info/PKG-INFO
--rw-r--r--   0 lucjean    (501) staff       (20)     3038 2019-08-29 14:49:29.000000 apidev-coop_colorbox-1.5.1/apidev_coop_colorbox.egg-info/SOURCES.txt.py
--rw-r--r--   0 lucjean    (501) staff       (20)        1 2019-08-29 13:12:34.000000 apidev-coop_colorbox-1.5.1/apidev_coop_colorbox.egg-info/not-zip-safe
--rw-r--r--   0 lucjean    (501) staff       (20)        1 2019-08-29 14:49:29.000000 apidev-coop_colorbox-1.5.1/apidev_coop_colorbox.egg-info/dependency_links.txt.py
--rw-r--r--   0 lucjean    (501) staff       (20)     3184 2019-08-30 10:36:12.000000 apidev-coop_colorbox-1.5.1/apidev_coop_colorbox.egg-info/SOURCES.txt
--rw-r--r--   0 lucjean    (501) staff       (20)        9 2019-08-29 14:49:29.000000 apidev-coop_colorbox-1.5.1/apidev_coop_colorbox.egg-info/top_level.txt.py
--rw-r--r--   0 lucjean    (501) staff       (20)        9 2019-08-30 10:36:12.000000 apidev-coop_colorbox-1.5.1/apidev_coop_colorbox.egg-info/top_level.txt
--rw-r--r--   0 lucjean    (501) staff       (20)        1 2019-08-30 10:36:12.000000 apidev-coop_colorbox-1.5.1/apidev_coop_colorbox.egg-info/dependency_links.txt
+drwxrwxr-x   0 lucjean   (1001) lucjean   (1001)        0 2023-06-12 12:53:56.871345 apidev-coop_colorbox-1.6.0/
+-rw-rw-r--   0 lucjean   (1001) lucjean   (1001)       93 2023-05-22 07:02:29.000000 apidev-coop_colorbox-1.6.0/MANIFEST.in
+-rw-rw-r--   0 lucjean   (1001) lucjean   (1001)     3202 2023-06-12 12:53:56.871345 apidev-coop_colorbox-1.6.0/PKG-INFO
+-rwxrwxr-x   0 lucjean   (1001) lucjean   (1001)     2395 2023-05-22 07:02:29.000000 apidev-coop_colorbox-1.6.0/README.rst
+drwxrwxr-x   0 lucjean   (1001) lucjean   (1001)        0 2023-06-12 12:53:56.859345 apidev-coop_colorbox-1.6.0/apidev_coop_colorbox.egg-info/
+-rw-rw-r--   0 lucjean   (1001) lucjean   (1001)     3202 2023-06-12 12:53:56.000000 apidev-coop_colorbox-1.6.0/apidev_coop_colorbox.egg-info/PKG-INFO
+-rw-rw-r--   0 lucjean   (1001) lucjean   (1001)     3038 2023-06-12 12:53:56.000000 apidev-coop_colorbox-1.6.0/apidev_coop_colorbox.egg-info/SOURCES.txt
+-rw-rw-r--   0 lucjean   (1001) lucjean   (1001)        1 2023-06-12 12:53:56.000000 apidev-coop_colorbox-1.6.0/apidev_coop_colorbox.egg-info/dependency_links.txt
+-rw-rw-r--   0 lucjean   (1001) lucjean   (1001)        1 2023-05-22 10:13:50.000000 apidev-coop_colorbox-1.6.0/apidev_coop_colorbox.egg-info/not-zip-safe
+-rw-rw-r--   0 lucjean   (1001) lucjean   (1001)        9 2023-06-12 12:53:56.000000 apidev-coop_colorbox-1.6.0/apidev_coop_colorbox.egg-info/top_level.txt
+drwxrwxr-x   0 lucjean   (1001) lucjean   (1001)        0 2023-06-12 12:53:56.863345 apidev-coop_colorbox-1.6.0/colorbox/
+-rwxrwxr-x   0 lucjean   (1001) lucjean   (1001)      214 2023-06-12 12:50:07.000000 apidev-coop_colorbox-1.6.0/colorbox/__init__.py
+-rw-rw-r--   0 lucjean   (1001) lucjean   (1001)      149 2023-06-12 12:50:07.000000 apidev-coop_colorbox-1.6.0/colorbox/apps.py
+-rwxrwxr-x   0 lucjean   (1001) lucjean   (1001)     2335 2023-06-12 12:50:07.000000 apidev-coop_colorbox-1.6.0/colorbox/decorators.py
+-rwxrwxr-x   0 lucjean   (1001) lucjean   (1001)      216 2023-06-12 12:50:07.000000 apidev-coop_colorbox-1.6.0/colorbox/forms.py
+-rwxrwxr-x   0 lucjean   (1001) lucjean   (1001)      845 2023-06-12 12:50:07.000000 apidev-coop_colorbox-1.6.0/colorbox/http.py
+drwxrwxr-x   0 lucjean   (1001) lucjean   (1001)        0 2023-06-12 12:53:56.859345 apidev-coop_colorbox-1.6.0/colorbox/static/
+drwxrwxr-x   0 lucjean   (1001) lucjean   (1001)        0 2023-06-12 12:53:56.863345 apidev-coop_colorbox-1.6.0/colorbox/static/css/
+-rwxrwxr-x   0 lucjean   (1001) lucjean   (1001)     3874 2023-05-22 07:02:29.000000 apidev-coop_colorbox-1.6.0/colorbox/static/css/colorbox.css
+drwxrwxr-x   0 lucjean   (1001) lucjean   (1001)        0 2023-06-12 12:53:56.863345 apidev-coop_colorbox-1.6.0/colorbox/static/css/images/
+-rwxrwxr-x   0 lucjean   (1001) lucjean   (1001)      112 2023-05-22 07:02:29.000000 apidev-coop_colorbox-1.6.0/colorbox/static/css/images/border.png
+-rwxrwxr-x   0 lucjean   (1001) lucjean   (1001)     2893 2023-05-22 07:02:29.000000 apidev-coop_colorbox-1.6.0/colorbox/static/css/images/controls.png
+drwxrwxr-x   0 lucjean   (1001) lucjean   (1001)        0 2023-06-12 12:53:56.863345 apidev-coop_colorbox-1.6.0/colorbox/static/css/images/ie6/
+-rwxrwxr-x   0 lucjean   (1001) lucjean   (1001)      111 2023-05-22 07:02:29.000000 apidev-coop_colorbox-1.6.0/colorbox/static/css/images/ie6/borderBottomCenter.png
+-rwxrwxr-x   0 lucjean   (1001) lucjean   (1001)      215 2023-05-22 07:02:29.000000 apidev-coop_colorbox-1.6.0/colorbox/static/css/images/ie6/borderBottomLeft.png
+-rwxrwxr-x   0 lucjean   (1001) lucjean   (1001)      217 2023-05-22 07:02:29.000000 apidev-coop_colorbox-1.6.0/colorbox/static/css/images/ie6/borderBottomRight.png
+-rwxrwxr-x   0 lucjean   (1001) lucjean   (1001)      108 2023-05-22 07:02:29.000000 apidev-coop_colorbox-1.6.0/colorbox/static/css/images/ie6/borderMiddleLeft.png
+-rwxrwxr-x   0 lucjean   (1001) lucjean   (1001)      108 2023-05-22 07:02:29.000000 apidev-coop_colorbox-1.6.0/colorbox/static/css/images/ie6/borderMiddleRight.png
+-rwxrwxr-x   0 lucjean   (1001) lucjean   (1001)      111 2023-05-22 07:02:29.000000 apidev-coop_colorbox-1.6.0/colorbox/static/css/images/ie6/borderTopCenter.png
+-rwxrwxr-x   0 lucjean   (1001) lucjean   (1001)      216 2023-05-22 07:02:29.000000 apidev-coop_colorbox-1.6.0/colorbox/static/css/images/ie6/borderTopLeft.png
+-rwxrwxr-x   0 lucjean   (1001) lucjean   (1001)      214 2023-05-22 07:02:29.000000 apidev-coop_colorbox-1.6.0/colorbox/static/css/images/ie6/borderTopRight.png
+-rwxrwxr-x   0 lucjean   (1001) lucjean   (1001)     9427 2023-05-22 07:02:29.000000 apidev-coop_colorbox-1.6.0/colorbox/static/css/images/loading.gif
+-rwxrwxr-x   0 lucjean   (1001) lucjean   (1001)      157 2023-05-22 07:02:29.000000 apidev-coop_colorbox-1.6.0/colorbox/static/css/images/loading_background.png
+-rwxrwxr-x   0 lucjean   (1001) lucjean   (1001)      182 2023-05-22 07:02:29.000000 apidev-coop_colorbox-1.6.0/colorbox/static/css/images/overlay.png
+drwxrwxr-x   0 lucjean   (1001) lucjean   (1001)        0 2023-06-12 12:53:56.863345 apidev-coop_colorbox-1.6.0/colorbox/static/js/
+-rwxrwxr-x   0 lucjean   (1001) lucjean   (1001)     3216 2023-05-22 07:02:29.000000 apidev-coop_colorbox-1.6.0/colorbox/static/js/colorbox.coop.js
+drwxrwxr-x   0 lucjean   (1001) lucjean   (1001)        0 2023-06-12 12:53:56.871345 apidev-coop_colorbox-1.6.0/colorbox/static/js/i18n/
+-rwxrwxr-x   0 lucjean   (1001) lucjean   (1001)      482 2023-05-22 07:02:29.000000 apidev-coop_colorbox-1.6.0/colorbox/static/js/i18n/jquery.colorbox-ar.js
+-rwxrwxr-x   0 lucjean   (1001) lucjean   (1001)      571 2023-05-22 07:02:29.000000 apidev-coop_colorbox-1.6.0/colorbox/static/js/i18n/jquery.colorbox-bg.js
+-rwxrwxr-x   0 lucjean   (1001) lucjean   (1001)      561 2023-05-22 07:02:29.000000 apidev-coop_colorbox-1.6.0/colorbox/static/js/i18n/jquery.colorbox-bn.js
+-rwxrwxr-x   0 lucjean   (1001) lucjean   (1001)      343 2023-05-22 07:02:29.000000 apidev-coop_colorbox-1.6.0/colorbox/static/js/i18n/jquery.colorbox-ca.js
+-rwxrwxr-x   0 lucjean   (1001) lucjean   (1001)      458 2023-05-22 07:02:29.000000 apidev-coop_colorbox-1.6.0/colorbox/static/js/i18n/jquery.colorbox-cs.js
+-rwxrwxr-x   0 lucjean   (1001) lucjean   (1001)      425 2023-05-22 07:02:29.000000 apidev-coop_colorbox-1.6.0/colorbox/static/js/i18n/jquery.colorbox-da.js
+-rwxrwxr-x   0 lucjean   (1001) lucjean   (1001)      425 2023-05-22 07:02:29.000000 apidev-coop_colorbox-1.6.0/colorbox/static/js/i18n/jquery.colorbox-de.js
+-rwxrwxr-x   0 lucjean   (1001) lucjean   (1001)      334 2023-05-22 07:02:29.000000 apidev-coop_colorbox-1.6.0/colorbox/static/js/i18n/jquery.colorbox-es.js
+-rwxrwxr-x   0 lucjean   (1001) lucjean   (1001)      388 2023-05-22 07:02:29.000000 apidev-coop_colorbox-1.6.0/colorbox/static/js/i18n/jquery.colorbox-et.js
+-rwxrwxr-x   0 lucjean   (1001) lucjean   (1001)      725 2023-05-22 07:02:29.000000 apidev-coop_colorbox-1.6.0/colorbox/static/js/i18n/jquery.colorbox-fa.js
+-rwxrwxr-x   0 lucjean   (1001) lucjean   (1001)      408 2023-05-22 07:02:29.000000 apidev-coop_colorbox-1.6.0/colorbox/static/js/i18n/jquery.colorbox-fi.js
+-rwxrwxr-x   0 lucjean   (1001) lucjean   (1001)      470 2023-05-22 07:02:29.000000 apidev-coop_colorbox-1.6.0/colorbox/static/js/i18n/jquery.colorbox-fr.js
+-rwxrwxr-x   0 lucjean   (1001) lucjean   (1001)      323 2023-05-22 07:02:29.000000 apidev-coop_colorbox-1.6.0/colorbox/static/js/i18n/jquery.colorbox-gl.js
+-rwxrwxr-x   0 lucjean   (1001) lucjean   (1001)      567 2023-05-22 07:02:29.000000 apidev-coop_colorbox-1.6.0/colorbox/static/js/i18n/jquery.colorbox-gr.js
+-rwxrwxr-x   0 lucjean   (1001) lucjean   (1001)      446 2023-05-22 07:02:29.000000 apidev-coop_colorbox-1.6.0/colorbox/static/js/i18n/jquery.colorbox-he.js
+-rwxrwxr-x   0 lucjean   (1001) lucjean   (1001)      443 2023-05-22 07:02:29.000000 apidev-coop_colorbox-1.6.0/colorbox/static/js/i18n/jquery.colorbox-hr.js
+-rwxrwxr-x   0 lucjean   (1001) lucjean   (1001)      430 2023-05-22 07:02:29.000000 apidev-coop_colorbox-1.6.0/colorbox/static/js/i18n/jquery.colorbox-hu.js
+-rwxrwxr-x   0 lucjean   (1001) lucjean   (1001)      391 2023-05-22 07:02:29.000000 apidev-coop_colorbox-1.6.0/colorbox/static/js/i18n/jquery.colorbox-id.js
+-rwxrwxr-x   0 lucjean   (1001) lucjean   (1001)      439 2023-05-22 07:02:29.000000 apidev-coop_colorbox-1.6.0/colorbox/static/js/i18n/jquery.colorbox-it.js
+-rwxrwxr-x   0 lucjean   (1001) lucjean   (1001)      480 2023-05-22 07:02:29.000000 apidev-coop_colorbox-1.6.0/colorbox/static/js/i18n/jquery.colorbox-ja.js
+-rwxrwxr-x   0 lucjean   (1001) lucjean   (1001)      450 2023-05-22 07:02:29.000000 apidev-coop_colorbox-1.6.0/colorbox/static/js/i18n/jquery.colorbox-kr.js
+-rwxrwxr-x   0 lucjean   (1001) lucjean   (1001)      446 2023-05-22 07:02:29.000000 apidev-coop_colorbox-1.6.0/colorbox/static/js/i18n/jquery.colorbox-lt.js
+-rwxrwxr-x   0 lucjean   (1001) lucjean   (1001)      459 2023-05-22 07:02:29.000000 apidev-coop_colorbox-1.6.0/colorbox/static/js/i18n/jquery.colorbox-lv.js
+-rwxrwxr-x   0 lucjean   (1001) lucjean   (1001)      858 2023-05-22 07:02:29.000000 apidev-coop_colorbox-1.6.0/colorbox/static/js/i18n/jquery.colorbox-my.js
+-rwxrwxr-x   0 lucjean   (1001) lucjean   (1001)      419 2023-05-22 07:02:29.000000 apidev-coop_colorbox-1.6.0/colorbox/static/js/i18n/jquery.colorbox-nl.js
+-rwxrwxr-x   0 lucjean   (1001) lucjean   (1001)      437 2023-05-22 07:02:29.000000 apidev-coop_colorbox-1.6.0/colorbox/static/js/i18n/jquery.colorbox-no.js
+-rwxrwxr-x   0 lucjean   (1001) lucjean   (1001)      479 2023-05-22 07:02:29.000000 apidev-coop_colorbox-1.6.0/colorbox/static/js/i18n/jquery.colorbox-pl.js
+-rwxrwxr-x   0 lucjean   (1001) lucjean   (1001)      446 2023-05-22 07:02:29.000000 apidev-coop_colorbox-1.6.0/colorbox/static/js/i18n/jquery.colorbox-pt-BR.js
+-rwxrwxr-x   0 lucjean   (1001) lucjean   (1001)      472 2023-05-22 07:02:29.000000 apidev-coop_colorbox-1.6.0/colorbox/static/js/i18n/jquery.colorbox-ro.js
+-rwxrwxr-x   0 lucjean   (1001) lucjean   (1001)      566 2023-05-22 07:02:29.000000 apidev-coop_colorbox-1.6.0/colorbox/static/js/i18n/jquery.colorbox-ru.js
+-rwxrwxr-x   0 lucjean   (1001) lucjean   (1001)      454 2023-05-22 07:02:29.000000 apidev-coop_colorbox-1.6.0/colorbox/static/js/i18n/jquery.colorbox-si.js
+-rwxrwxr-x   0 lucjean   (1001) lucjean   (1001)      437 2023-05-22 07:02:29.000000 apidev-coop_colorbox-1.6.0/colorbox/static/js/i18n/jquery.colorbox-sk.js
+-rwxrwxr-x   0 lucjean   (1001) lucjean   (1001)      507 2023-05-22 07:02:29.000000 apidev-coop_colorbox-1.6.0/colorbox/static/js/i18n/jquery.colorbox-sr.js
+-rwxrwxr-x   0 lucjean   (1001) lucjean   (1001)      412 2023-05-22 07:02:29.000000 apidev-coop_colorbox-1.6.0/colorbox/static/js/i18n/jquery.colorbox-sv.js
+-rwxrwxr-x   0 lucjean   (1001) lucjean   (1001)      498 2023-05-22 07:02:29.000000 apidev-coop_colorbox-1.6.0/colorbox/static/js/i18n/jquery.colorbox-tr.js
+-rwxrwxr-x   0 lucjean   (1001) lucjean   (1001)      596 2023-05-22 07:02:29.000000 apidev-coop_colorbox-1.6.0/colorbox/static/js/i18n/jquery.colorbox-uk.js
+-rwxrwxr-x   0 lucjean   (1001) lucjean   (1001)      439 2023-05-22 07:02:29.000000 apidev-coop_colorbox-1.6.0/colorbox/static/js/i18n/jquery.colorbox-zh-CN.js
+-rwxrwxr-x   0 lucjean   (1001) lucjean   (1001)      408 2023-05-22 07:02:29.000000 apidev-coop_colorbox-1.6.0/colorbox/static/js/i18n/jquery.colorbox-zh-TW.js
+-rwxrwxr-x   0 lucjean   (1001) lucjean   (1001)    11885 2023-05-22 07:02:29.000000 apidev-coop_colorbox-1.6.0/colorbox/static/js/jquery.colorbox-min.js
+-rwxrwxr-x   0 lucjean   (1001) lucjean   (1001)    29080 2023-05-22 07:02:29.000000 apidev-coop_colorbox-1.6.0/colorbox/static/js/jquery.colorbox.js
+-rwxrwxr-x   0 lucjean   (1001) lucjean   (1001)    44034 2023-05-22 07:02:29.000000 apidev-coop_colorbox-1.6.0/colorbox/static/js/jquery.form.js
+drwxrwxr-x   0 lucjean   (1001) lucjean   (1001)        0 2023-06-12 12:53:56.859345 apidev-coop_colorbox-1.6.0/colorbox/templates/
+drwxrwxr-x   0 lucjean   (1001) lucjean   (1001)        0 2023-06-12 12:53:56.871345 apidev-coop_colorbox-1.6.0/colorbox/templates/colorbox/
+-rw-rw-r--   0 lucjean   (1001) lucjean   (1001)      326 2023-05-22 07:02:29.000000 apidev-coop_colorbox-1.6.0/colorbox/templates/colorbox/popup_confirm.html
+-rwxrwxr-x   0 lucjean   (1001) lucjean   (1001)     1372 2023-05-22 07:02:29.000000 apidev-coop_colorbox-1.6.0/colorbox/templates/colorbox/popup_form_base.html
+-rwxrwxr-x   0 lucjean   (1001) lucjean   (1001)     1131 2023-06-12 12:50:07.000000 apidev-coop_colorbox-1.6.0/colorbox/utils.py
+-rw-rw-r--   0 lucjean   (1001) lucjean   (1001)     2431 2023-06-12 12:50:07.000000 apidev-coop_colorbox-1.6.0/colorbox/views.py
+-rw-rw-r--   0 lucjean   (1001) lucjean   (1001)       38 2023-06-12 12:53:56.871345 apidev-coop_colorbox-1.6.0/setup.cfg
+-rw-rw-r--   0 lucjean   (1001) lucjean   (1001)     1249 2023-06-12 12:50:07.000000 apidev-coop_colorbox-1.6.0/setup.py
```

### filetype from file(1)

```diff
@@ -1 +1 @@
-POSIX tar archive (GNU)
+POSIX tar archive
```

### Comparing `apidev-coop_colorbox-1.5.1/colorbox/static/css/colorbox.css` & `apidev-coop_colorbox-1.6.0/colorbox/static/css/colorbox.css`

 * *Files identical despite different names*

### Comparing `apidev-coop_colorbox-1.5.1/colorbox/static/css/images/loading.gif` & `apidev-coop_colorbox-1.6.0/colorbox/static/css/images/loading.gif`

 * *Files identical despite different names*

### Comparing `apidev-coop_colorbox-1.5.1/colorbox/static/css/images/controls.png` & `apidev-coop_colorbox-1.6.0/colorbox/static/css/images/controls.png`

 * *Files identical despite different names*

### Comparing `apidev-coop_colorbox-1.5.1/colorbox/static/js/jquery.colorbox-min.js` & `apidev-coop_colorbox-1.6.0/colorbox/static/js/jquery.colorbox-min.js`

 * *Files identical despite different names*

### Comparing `apidev-coop_colorbox-1.5.1/colorbox/static/js/jquery.colorbox.js` & `apidev-coop_colorbox-1.6.0/colorbox/static/js/jquery.colorbox.js`

 * *Files identical despite different names*

### Comparing `apidev-coop_colorbox-1.5.1/colorbox/static/js/colorbox.coop.js` & `apidev-coop_colorbox-1.6.0/colorbox/static/js/colorbox.coop.js`

 * *Files identical despite different names*

### Comparing `apidev-coop_colorbox-1.5.1/colorbox/static/js/i18n/jquery.colorbox-my.js` & `apidev-coop_colorbox-1.6.0/colorbox/static/js/i18n/jquery.colorbox-my.js`

 * *Files identical despite different names*

### Comparing `apidev-coop_colorbox-1.5.1/colorbox/static/js/i18n/jquery.colorbox-bg.js` & `apidev-coop_colorbox-1.6.0/colorbox/static/js/i18n/jquery.colorbox-bg.js`

 * *Files identical despite different names*

### Comparing `apidev-coop_colorbox-1.5.1/colorbox/static/js/i18n/jquery.colorbox-ru.js` & `apidev-coop_colorbox-1.6.0/colorbox/static/js/i18n/jquery.colorbox-ru.js`

 * *Files identical despite different names*

### Comparing `apidev-coop_colorbox-1.5.1/colorbox/static/js/i18n/jquery.colorbox-bn.js` & `apidev-coop_colorbox-1.6.0/colorbox/static/js/i18n/jquery.colorbox-bn.js`

 * *Files identical despite different names*

### Comparing `apidev-coop_colorbox-1.5.1/colorbox/static/js/i18n/jquery.colorbox-gr.js` & `apidev-coop_colorbox-1.6.0/colorbox/static/js/i18n/jquery.colorbox-gr.js`

 * *Files identical despite different names*

### Comparing `apidev-coop_colorbox-1.5.1/colorbox/static/js/i18n/jquery.colorbox-uk.js` & `apidev-coop_colorbox-1.6.0/colorbox/static/js/i18n/jquery.colorbox-uk.js`

 * *Files identical despite different names*

### Comparing `apidev-coop_colorbox-1.5.1/colorbox/static/js/i18n/jquery.colorbox-fa.js` & `apidev-coop_colorbox-1.6.0/colorbox/static/js/i18n/jquery.colorbox-fa.js`

 * *Files identical despite different names*

### Comparing `apidev-coop_colorbox-1.5.1/colorbox/static/js/jquery.form.js` & `apidev-coop_colorbox-1.6.0/colorbox/static/js/jquery.form.js`

 * *Files identical despite different names*

### Comparing `apidev-coop_colorbox-1.5.1/colorbox/http.py` & `apidev-coop_colorbox-1.6.0/colorbox/http.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,11 +1,9 @@
 # -*- coding: utf-8 -*-
 
-from __future__ import unicode_literals
-
 from django.http import HttpResponse
 
 
 class HttpResponseClosePopup(HttpResponse):
     """A HttpResponse with the right content for closing the colorbox"""
     def __init__(self):
         super(HttpResponseClosePopup, self).__init__("close_popup")
```

### Comparing `apidev-coop_colorbox-1.5.1/colorbox/templates/colorbox/popup_form_base.html` & `apidev-coop_colorbox-1.6.0/colorbox/templates/colorbox/popup_form_base.html`

 * *Files identical despite different names*

### Comparing `apidev-coop_colorbox-1.5.1/colorbox/views.py` & `apidev-coop_colorbox-1.6.0/colorbox/views.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,12 +1,10 @@
 # -*- coding: utf-8 -*-
 """some reusable views: inherit from them"""
 
-from __future__ import unicode_literals
-
 from django.views.generic.edit import FormView
 
 from django.utils.decorators import method_decorator
 from django.core.exceptions import PermissionDenied
 
 from .decorators import popup_redirect
 from .forms import ConfirmForm
@@ -80,10 +78,7 @@
 
         elif form.is_cancelled():
             response = self.form_cancelled()
             if response:
                 return response
 
         return HttpResponseClosePopup()
-
-
-
```

### Comparing `apidev-coop_colorbox-1.5.1/colorbox/decorators.py` & `apidev-coop_colorbox-1.6.0/colorbox/decorators.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,12 +1,10 @@
 # -*- coding: utf-8 -*-
 """decorator for managing colorbox"""
 
-from __future__ import unicode_literals
-
 import logging
 
 from django.http import HttpResponse, HttpResponseNotFound, Http404, HttpResponseForbidden
 from django.core.exceptions import PermissionDenied
 
 logger = logging.getLogger("colorbox")
```

#### html2text {}

```diff
@@ -1,17 +1,17 @@
-# -*- coding: utf-8 -*- """decorator for managing colorbox""" from __future__
-import unicode_literals import logging from django.http import HttpResponse,
-HttpResponseNotFound, Http404, HttpResponseForbidden from
-django.core.exceptions import PermissionDenied logger = logging.getLogger
-("colorbox") def popup_redirect(view_func): """manage redirection : close the
-coorbox. Very useful for form-based views""" def wrapper(request, *args,
-**kwargs): try: response = view_func(request, *args, **kwargs) except Http404:
-return HttpResponseNotFound() except PermissionDenied: return
-HttpResponseForbidden() except Exception as msg: logger.exception("exception in
-popup: {0}".format(msg)) raise if response.status_code == 302: script = '
+# -*- coding: utf-8 -*- """decorator for managing colorbox""" import logging
+from django.http import HttpResponse, HttpResponseNotFound, Http404,
+HttpResponseForbidden from django.core.exceptions import PermissionDenied
+logger = logging.getLogger("colorbox") def popup_redirect(view_func): """manage
+redirection : close the coorbox. Very useful for form-based views""" def
+wrapper(request, *args, **kwargs): try: response = view_func(request, *args,
+**kwargs) except Http404: return HttpResponseNotFound() except
+PermissionDenied: return HttpResponseForbidden() except Exception as msg:
+logger.exception("exception in popup: {0}".format(msg)) raise if
+response.status_code == 302: script = '
 '.format(response['Location']) return HttpResponse(script) elif
 response.status_code != 200: return HttpResponse(status=response.status_code)
 else: return response return wrapper def popup_reload(view_func): """manage
 redirection : reopen in a new coorbox.""" def wrapper(request, *args,
 **kwargs): try: response = view_func(request, *args, **kwargs) except Http404:
 return HttpResponseNotFound() except PermissionDenied: return
 HttpResponseForbidden() except Exception as msg: logger.exception("exception in
```

### Comparing `apidev-coop_colorbox-1.5.1/setup.py` & `apidev-coop_colorbox-1.6.0/setup.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,12 +1,10 @@
 #!/usr/bin/env python
 # -*- coding: utf-8 -*-
 
-from __future__ import unicode_literals
-
 try:
     from setuptools import setup, find_packages
 except ImportError:
     import ez_setup
     ez_setup.use_setuptools()
     from setuptools import setup, find_packages
```

### Comparing `apidev-coop_colorbox-1.5.1/README.rst` & `apidev-coop_colorbox-1.6.0/README.rst`

 * *Files identical despite different names*

### Comparing `apidev-coop_colorbox-1.5.1/apidev_coop_colorbox.egg-info/SOURCES.txt` & `apidev-coop_colorbox-1.6.0/apidev_coop_colorbox.egg-info/SOURCES.txt`

 * *Files 13% similar despite different names*

```diff
@@ -1,18 +1,15 @@
 MANIFEST.in
 README.rst
 setup.py
 apidev_coop_colorbox.egg-info/PKG-INFO
 apidev_coop_colorbox.egg-info/SOURCES.txt
-apidev_coop_colorbox.egg-info/SOURCES.txt.py
 apidev_coop_colorbox.egg-info/dependency_links.txt
-apidev_coop_colorbox.egg-info/dependency_links.txt.py
 apidev_coop_colorbox.egg-info/not-zip-safe
 apidev_coop_colorbox.egg-info/top_level.txt
-apidev_coop_colorbox.egg-info/top_level.txt.py
 colorbox/__init__.py
 colorbox/apps.py
 colorbox/decorators.py
 colorbox/forms.py
 colorbox/http.py
 colorbox/utils.py
 colorbox/views.py
```

