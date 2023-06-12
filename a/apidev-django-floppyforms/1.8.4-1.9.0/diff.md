# Comparing `tmp/apidev_django-floppyforms-1.8.4.tar.gz` & `tmp/apidev_django-floppyforms-1.9.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/apidev_django-floppyforms-1.8.4.tar", last modified: Wed Jul 29 15:02:09 2020, max compression
+gzip compressed data, was "apidev_django-floppyforms-1.9.0.tar", last modified: Mon Jun 12 12:55:38 2023, max compression
```

## Comparing `apidev_django-floppyforms-1.8.4.tar` & `apidev_django-floppyforms-1.9.0.tar`

### file list

```diff
@@ -1,189 +1,192 @@
-drwxr-xr-x   0 lucjean    (501) staff       (20)        0 2020-07-29 15:02:09.570183 apidev_django-floppyforms-1.8.4/
--rw-r--r--   0 lucjean    (501) staff       (20)     8935 2020-07-28 08:29:05.000000 apidev_django-floppyforms-1.8.4/CHANGES.rst
--rw-r--r--   0 lucjean    (501) staff       (20)      340 2020-07-28 08:29:05.000000 apidev_django-floppyforms-1.8.4/MANIFEST.in
--rw-r--r--   0 lucjean    (501) staff       (20)    13338 2020-07-29 15:02:09.571229 apidev_django-floppyforms-1.8.4/PKG-INFO
--rw-r--r--   0 lucjean    (501) staff       (20)      680 2020-07-28 08:29:05.000000 apidev_django-floppyforms-1.8.4/README.rst
-drwxr-xr-x   0 lucjean    (501) staff       (20)        0 2020-07-29 15:02:07.718785 apidev_django-floppyforms-1.8.4/apidev_django_floppyforms.egg-info/
--rw-r--r--   0 lucjean    (501) staff       (20)    13338 2020-07-29 15:02:07.000000 apidev_django-floppyforms-1.8.4/apidev_django_floppyforms.egg-info/PKG-INFO
--rw-r--r--   0 lucjean    (501) staff       (20)     7134 2020-07-29 15:02:07.000000 apidev_django-floppyforms-1.8.4/apidev_django_floppyforms.egg-info/SOURCES.txt
--rw-r--r--   0 lucjean    (501) staff       (20)        1 2020-07-29 15:02:07.000000 apidev_django-floppyforms-1.8.4/apidev_django_floppyforms.egg-info/dependency_links.txt
--rw-r--r--   0 lucjean    (501) staff       (20)        1 2020-07-28 08:29:15.000000 apidev_django-floppyforms-1.8.4/apidev_django_floppyforms.egg-info/not-zip-safe
--rw-r--r--   0 lucjean    (501) staff       (20)       12 2020-07-29 15:02:07.000000 apidev_django-floppyforms-1.8.4/apidev_django_floppyforms.egg-info/top_level.txt
-drwxr-xr-x   0 lucjean    (501) staff       (20)        0 2020-07-29 15:02:07.863250 apidev_django-floppyforms-1.8.4/docs/
--rw-r--r--   0 lucjean    (501) staff       (20)     4638 2020-07-28 08:29:05.000000 apidev_django-floppyforms-1.8.4/docs/Makefile
--rw-r--r--   0 lucjean    (501) staff       (20)     3427 2020-07-28 08:29:05.000000 apidev_django-floppyforms-1.8.4/docs/bootstrap.rst
--rw-r--r--   0 lucjean    (501) staff       (20)       28 2020-07-28 08:29:05.000000 apidev_django-floppyforms-1.8.4/docs/changelog.rst
--rw-r--r--   0 lucjean    (501) staff       (20)     7318 2020-07-28 08:29:05.000000 apidev_django-floppyforms-1.8.4/docs/conf.py
--rw-r--r--   0 lucjean    (501) staff       (20)     3927 2020-07-28 08:29:05.000000 apidev_django-floppyforms-1.8.4/docs/customization.rst
--rw-r--r--   0 lucjean    (501) staff       (20)     7186 2020-07-28 08:29:05.000000 apidev_django-floppyforms-1.8.4/docs/differences.rst
--rw-r--r--   0 lucjean    (501) staff       (20)     6575 2020-07-28 08:29:05.000000 apidev_django-floppyforms-1.8.4/docs/examples.rst
--rw-r--r--   0 lucjean    (501) staff       (20)    15514 2020-07-28 08:29:05.000000 apidev_django-floppyforms-1.8.4/docs/geodjango.rst
-drwxr-xr-x   0 lucjean    (501) staff       (20)        0 2020-07-29 15:02:08.069677 apidev_django-floppyforms-1.8.4/docs/images/
--rw-r--r--   0 lucjean    (501) staff       (20)     2071 2020-07-28 08:29:05.000000 apidev_django-floppyforms-1.8.4/docs/images/datepicker-chromium.png
--rw-r--r--   0 lucjean    (501) staff       (20)    15545 2020-07-28 08:29:05.000000 apidev_django-floppyforms-1.8.4/docs/images/datepicker-jquery-ui.png
--rw-r--r--   0 lucjean    (501) staff       (20)   228293 2020-07-28 08:29:05.000000 apidev_django-floppyforms-1.8.4/docs/images/geomcollection.png
--rw-r--r--   0 lucjean    (501) staff       (20)   323935 2020-07-28 08:29:05.000000 apidev_django-floppyforms-1.8.4/docs/images/gmappoly.png
--rw-r--r--   0 lucjean    (501) staff       (20)    26810 2020-07-28 08:29:05.000000 apidev_django-floppyforms-1.8.4/docs/images/image_with_thumbnail.png
--rw-r--r--   0 lucjean    (501) staff       (20)   343359 2020-07-28 08:29:05.000000 apidev_django-floppyforms-1.8.4/docs/images/osmlinestring.png
--rw-r--r--   0 lucjean    (501) staff       (20)   119517 2020-07-28 08:29:05.000000 apidev_django-floppyforms-1.8.4/docs/images/pointfield.png
--rw-r--r--   0 lucjean    (501) staff       (20)      845 2020-07-28 08:29:05.000000 apidev_django-floppyforms-1.8.4/docs/images/slider-chromium.png
--rw-r--r--   0 lucjean    (501) staff       (20)     1452 2020-07-28 08:29:05.000000 apidev_django-floppyforms-1.8.4/docs/images/slider-jquery-ui.png
--rw-r--r--   0 lucjean    (501) staff       (20)     4163 2020-07-28 08:29:05.000000 apidev_django-floppyforms-1.8.4/docs/index.rst
--rw-r--r--   0 lucjean    (501) staff       (20)    11815 2020-07-28 08:29:05.000000 apidev_django-floppyforms-1.8.4/docs/layouts.rst
--rw-r--r--   0 lucjean    (501) staff       (20)     8377 2020-07-28 08:29:05.000000 apidev_django-floppyforms-1.8.4/docs/templatetags.rst
--rw-r--r--   0 lucjean    (501) staff       (20)     5354 2020-07-28 08:29:05.000000 apidev_django-floppyforms-1.8.4/docs/usage.rst
--rw-r--r--   0 lucjean    (501) staff       (20)     7732 2020-07-28 08:29:05.000000 apidev_django-floppyforms-1.8.4/docs/widgets-reference.rst
--rw-r--r--   0 lucjean    (501) staff       (20)     4460 2020-07-28 08:29:05.000000 apidev_django-floppyforms-1.8.4/docs/widgets.rst
-drwxr-xr-x   0 lucjean    (501) staff       (20)        0 2020-07-29 15:02:08.129984 apidev_django-floppyforms-1.8.4/floppyforms/
-drwxr-xr-x   0 lucjean    (501) staff       (20)        0 2020-07-29 15:02:08.149149 apidev_django-floppyforms-1.8.4/floppyforms/__future__/
--rw-r--r--   0 lucjean    (501) staff       (20)      245 2020-07-28 08:29:05.000000 apidev_django-floppyforms-1.8.4/floppyforms/__future__/__init__.py
--rw-r--r--   0 lucjean    (501) staff       (20)     5088 2020-07-28 08:29:05.000000 apidev_django-floppyforms-1.8.4/floppyforms/__future__/models.py
--rw-r--r--   0 lucjean    (501) staff       (20)      541 2020-07-29 15:01:07.000000 apidev_django-floppyforms-1.8.4/floppyforms/__init__.py
--rw-r--r--   0 lucjean    (501) staff       (20)     2380 2020-07-28 08:29:05.000000 apidev_django-floppyforms-1.8.4/floppyforms/compat.py
--rw-r--r--   0 lucjean    (501) staff       (20)     5608 2020-07-28 08:29:05.000000 apidev_django-floppyforms-1.8.4/floppyforms/fields.py
--rw-r--r--   0 lucjean    (501) staff       (20)     1054 2020-07-28 08:29:05.000000 apidev_django-floppyforms-1.8.4/floppyforms/forms.py
-drwxr-xr-x   0 lucjean    (501) staff       (20)        0 2020-07-29 15:02:08.181360 apidev_django-floppyforms-1.8.4/floppyforms/gis/
--rw-r--r--   0 lucjean    (501) staff       (20)       60 2020-07-28 08:29:05.000000 apidev_django-floppyforms-1.8.4/floppyforms/gis/__init__.py
--rw-r--r--   0 lucjean    (501) staff       (20)     3013 2020-07-28 08:29:05.000000 apidev_django-floppyforms-1.8.4/floppyforms/gis/fields.py
--rw-r--r--   0 lucjean    (501) staff       (20)     5627 2020-07-28 08:29:05.000000 apidev_django-floppyforms-1.8.4/floppyforms/gis/widgets.py
--rw-r--r--   0 lucjean    (501) staff       (20)     1093 2020-07-28 08:29:05.000000 apidev_django-floppyforms-1.8.4/floppyforms/models.py
-drwxr-xr-x   0 lucjean    (501) staff       (20)        0 2020-07-29 15:02:07.693203 apidev_django-floppyforms-1.8.4/floppyforms/static/
-drwxr-xr-x   0 lucjean    (501) staff       (20)        0 2020-07-29 15:02:07.693679 apidev_django-floppyforms-1.8.4/floppyforms/static/floppyforms/
-drwxr-xr-x   0 lucjean    (501) staff       (20)        0 2020-07-29 15:02:07.693387 apidev_django-floppyforms-1.8.4/floppyforms/static/floppyforms/gis/
-drwxr-xr-x   0 lucjean    (501) staff       (20)        0 2020-07-29 15:02:08.210283 apidev_django-floppyforms-1.8.4/floppyforms/static/floppyforms/gis/img/
--rw-r--r--   0 lucjean    (501) staff       (20)      711 2020-07-28 08:29:05.000000 apidev_django-floppyforms-1.8.4/floppyforms/static/floppyforms/gis/img/move_vertex_off.png
--rw-r--r--   0 lucjean    (501) staff       (20)      506 2020-07-28 08:29:05.000000 apidev_django-floppyforms-1.8.4/floppyforms/static/floppyforms/gis/img/move_vertex_on.png
-drwxr-xr-x   0 lucjean    (501) staff       (20)        0 2020-07-29 15:02:08.235118 apidev_django-floppyforms-1.8.4/floppyforms/static/floppyforms/js/
--rw-r--r--   0 lucjean    (501) staff       (20)    12292 2020-07-28 08:29:05.000000 apidev_django-floppyforms-1.8.4/floppyforms/static/floppyforms/js/MapWidget.js
-drwxr-xr-x   0 lucjean    (501) staff       (20)        0 2020-07-29 15:02:08.243276 apidev_django-floppyforms-1.8.4/floppyforms/static/floppyforms/openlayers/
--rw-r--r--   0 lucjean    (501) staff       (20)   770300 2020-07-28 08:29:05.000000 apidev_django-floppyforms-1.8.4/floppyforms/static/floppyforms/openlayers/OpenLayers.js
-drwxr-xr-x   0 lucjean    (501) staff       (20)        0 2020-07-29 15:02:07.693947 apidev_django-floppyforms-1.8.4/floppyforms/static/floppyforms/openlayers/theme/
-drwxr-xr-x   0 lucjean    (501) staff       (20)        0 2020-07-29 15:02:08.308101 apidev_django-floppyforms-1.8.4/floppyforms/static/floppyforms/openlayers/theme/default/
--rw-r--r--   0 lucjean    (501) staff       (20)      142 2020-07-28 08:29:05.000000 apidev_django-floppyforms-1.8.4/floppyforms/static/floppyforms/openlayers/theme/default/google.css
--rw-r--r--   0 lucjean    (501) staff       (20)      212 2020-07-28 08:29:05.000000 apidev_django-floppyforms-1.8.4/floppyforms/static/floppyforms/openlayers/theme/default/ie6-style.css
-drwxr-xr-x   0 lucjean    (501) staff       (20)        0 2020-07-29 15:02:08.688980 apidev_django-floppyforms-1.8.4/floppyforms/static/floppyforms/openlayers/theme/default/img/
--rw-r--r--   0 lucjean    (501) staff       (20)     1614 2020-07-28 08:29:05.000000 apidev_django-floppyforms-1.8.4/floppyforms/static/floppyforms/openlayers/theme/default/img/add_point_off.png
--rw-r--r--   0 lucjean    (501) staff       (20)     1464 2020-07-28 08:29:05.000000 apidev_django-floppyforms-1.8.4/floppyforms/static/floppyforms/openlayers/theme/default/img/add_point_on.png
--rw-r--r--   0 lucjean    (501) staff       (20)       42 2020-07-28 08:29:05.000000 apidev_django-floppyforms-1.8.4/floppyforms/static/floppyforms/openlayers/theme/default/img/blank.gif
--rw-r--r--   0 lucjean    (501) staff       (20)     1078 2020-07-28 08:29:05.000000 apidev_django-floppyforms-1.8.4/floppyforms/static/floppyforms/openlayers/theme/default/img/close.gif
--rw-r--r--   0 lucjean    (501) staff       (20)     1024 2020-07-28 08:29:05.000000 apidev_django-floppyforms-1.8.4/floppyforms/static/floppyforms/openlayers/theme/default/img/drag-rectangle-off.png
--rw-r--r--   0 lucjean    (501) staff       (20)     1041 2020-07-28 08:29:05.000000 apidev_django-floppyforms-1.8.4/floppyforms/static/floppyforms/openlayers/theme/default/img/drag-rectangle-on.png
--rw-r--r--   0 lucjean    (501) staff       (20)     1565 2020-07-28 08:29:05.000000 apidev_django-floppyforms-1.8.4/floppyforms/static/floppyforms/openlayers/theme/default/img/draw_line_off.png
--rw-r--r--   0 lucjean    (501) staff       (20)     1396 2020-07-28 08:29:05.000000 apidev_django-floppyforms-1.8.4/floppyforms/static/floppyforms/openlayers/theme/default/img/draw_line_on.png
--rw-r--r--   0 lucjean    (501) staff       (20)     1610 2020-07-28 08:29:05.000000 apidev_django-floppyforms-1.8.4/floppyforms/static/floppyforms/openlayers/theme/default/img/draw_point_off.png
--rw-r--r--   0 lucjean    (501) staff       (20)     1458 2020-07-28 08:29:05.000000 apidev_django-floppyforms-1.8.4/floppyforms/static/floppyforms/openlayers/theme/default/img/draw_point_on.png
--rw-r--r--   0 lucjean    (501) staff       (20)     1544 2020-07-28 08:29:05.000000 apidev_django-floppyforms-1.8.4/floppyforms/static/floppyforms/openlayers/theme/default/img/draw_polygon_off.png
--rw-r--r--   0 lucjean    (501) staff       (20)     1405 2020-07-28 08:29:05.000000 apidev_django-floppyforms-1.8.4/floppyforms/static/floppyforms/openlayers/theme/default/img/draw_polygon_on.png
--rw-r--r--   0 lucjean    (501) staff       (20)     2222 2020-07-28 08:29:05.000000 apidev_django-floppyforms-1.8.4/floppyforms/static/floppyforms/openlayers/theme/default/img/editing_tool_bar.png
--rw-r--r--   0 lucjean    (501) staff       (20)     1541 2020-07-28 08:29:05.000000 apidev_django-floppyforms-1.8.4/floppyforms/static/floppyforms/openlayers/theme/default/img/move_feature_off.png
--rw-r--r--   0 lucjean    (501) staff       (20)     1377 2020-07-28 08:29:05.000000 apidev_django-floppyforms-1.8.4/floppyforms/static/floppyforms/openlayers/theme/default/img/move_feature_on.png
--rw-r--r--   0 lucjean    (501) staff       (20)     6628 2020-07-28 08:29:05.000000 apidev_django-floppyforms-1.8.4/floppyforms/static/floppyforms/openlayers/theme/default/img/navigation_history.png
--rw-r--r--   0 lucjean    (501) staff       (20)       79 2020-07-28 08:29:05.000000 apidev_django-floppyforms-1.8.4/floppyforms/static/floppyforms/openlayers/theme/default/img/overview_replacement.gif
--rw-r--r--   0 lucjean    (501) staff       (20)      564 2020-07-28 08:29:05.000000 apidev_django-floppyforms-1.8.4/floppyforms/static/floppyforms/openlayers/theme/default/img/pan-panel-NOALPHA.png
--rw-r--r--   0 lucjean    (501) staff       (20)      814 2020-07-28 08:29:05.000000 apidev_django-floppyforms-1.8.4/floppyforms/static/floppyforms/openlayers/theme/default/img/pan-panel.png
--rw-r--r--   0 lucjean    (501) staff       (20)     1696 2020-07-28 08:29:05.000000 apidev_django-floppyforms-1.8.4/floppyforms/static/floppyforms/openlayers/theme/default/img/pan_off.png
--rw-r--r--   0 lucjean    (501) staff       (20)     1566 2020-07-28 08:29:05.000000 apidev_django-floppyforms-1.8.4/floppyforms/static/floppyforms/openlayers/theme/default/img/pan_on.png
--rw-r--r--   0 lucjean    (501) staff       (20)     3511 2020-07-28 08:29:05.000000 apidev_django-floppyforms-1.8.4/floppyforms/static/floppyforms/openlayers/theme/default/img/panning-hand-off.png
--rw-r--r--   0 lucjean    (501) staff       (20)     3565 2020-07-28 08:29:05.000000 apidev_django-floppyforms-1.8.4/floppyforms/static/floppyforms/openlayers/theme/default/img/panning-hand-on.png
--rw-r--r--   0 lucjean    (501) staff       (20)     1612 2020-07-28 08:29:05.000000 apidev_django-floppyforms-1.8.4/floppyforms/static/floppyforms/openlayers/theme/default/img/remove_point_off.png
--rw-r--r--   0 lucjean    (501) staff       (20)     1461 2020-07-28 08:29:05.000000 apidev_django-floppyforms-1.8.4/floppyforms/static/floppyforms/openlayers/theme/default/img/remove_point_on.png
--rw-r--r--   0 lucjean    (501) staff       (20)     1211 2020-07-28 08:29:05.000000 apidev_django-floppyforms-1.8.4/floppyforms/static/floppyforms/openlayers/theme/default/img/ruler.png
--rw-r--r--   0 lucjean    (501) staff       (20)      354 2020-07-28 08:29:05.000000 apidev_django-floppyforms-1.8.4/floppyforms/static/floppyforms/openlayers/theme/default/img/save_features_off.png
--rw-r--r--   0 lucjean    (501) staff       (20)      361 2020-07-28 08:29:05.000000 apidev_django-floppyforms-1.8.4/floppyforms/static/floppyforms/openlayers/theme/default/img/save_features_on.png
--rw-r--r--   0 lucjean    (501) staff       (20)     1499 2020-07-28 08:29:05.000000 apidev_django-floppyforms-1.8.4/floppyforms/static/floppyforms/openlayers/theme/default/img/view_next_off.png
--rw-r--r--   0 lucjean    (501) staff       (20)     1686 2020-07-28 08:29:05.000000 apidev_django-floppyforms-1.8.4/floppyforms/static/floppyforms/openlayers/theme/default/img/view_next_on.png
--rw-r--r--   0 lucjean    (501) staff       (20)     1476 2020-07-28 08:29:05.000000 apidev_django-floppyforms-1.8.4/floppyforms/static/floppyforms/openlayers/theme/default/img/view_previous_off.png
--rw-r--r--   0 lucjean    (501) staff       (20)     1592 2020-07-28 08:29:05.000000 apidev_django-floppyforms-1.8.4/floppyforms/static/floppyforms/openlayers/theme/default/img/view_previous_on.png
--rw-r--r--   0 lucjean    (501) staff       (20)     1173 2020-07-28 08:29:05.000000 apidev_django-floppyforms-1.8.4/floppyforms/static/floppyforms/openlayers/theme/default/img/zoom-panel-NOALPHA.png
--rw-r--r--   0 lucjean    (501) staff       (20)     1285 2020-07-28 08:29:05.000000 apidev_django-floppyforms-1.8.4/floppyforms/static/floppyforms/openlayers/theme/default/img/zoom-panel.png
--rw-r--r--   0 lucjean    (501) staff       (20)    10791 2020-07-28 08:29:05.000000 apidev_django-floppyforms-1.8.4/floppyforms/static/floppyforms/openlayers/theme/default/style.css
--rw-r--r--   0 lucjean    (501) staff       (20)     1799 2020-07-28 08:29:05.000000 apidev_django-floppyforms-1.8.4/floppyforms/static/floppyforms/openlayers/theme/default/style.mobile.css
-drwxr-xr-x   0 lucjean    (501) staff       (20)        0 2020-07-29 15:02:07.694534 apidev_django-floppyforms-1.8.4/floppyforms/templates/
-drwxr-xr-x   0 lucjean    (501) staff       (20)        0 2020-07-29 15:02:09.105346 apidev_django-floppyforms-1.8.4/floppyforms/templates/floppyforms/
--rw-r--r--   0 lucjean    (501) staff       (20)      107 2020-07-28 08:29:05.000000 apidev_django-floppyforms-1.8.4/floppyforms/templates/floppyforms/_render_as.html
--rw-r--r--   0 lucjean    (501) staff       (20)      492 2020-07-28 08:29:05.000000 apidev_django-floppyforms-1.8.4/floppyforms/templates/floppyforms/attrs.html
--rw-r--r--   0 lucjean    (501) staff       (20)       39 2020-07-28 08:29:05.000000 apidev_django-floppyforms-1.8.4/floppyforms/templates/floppyforms/checkbox.html
--rw-r--r--   0 lucjean    (501) staff       (20)      349 2020-07-28 08:29:05.000000 apidev_django-floppyforms-1.8.4/floppyforms/templates/floppyforms/checkbox_select.html
--rw-r--r--   0 lucjean    (501) staff       (20)      440 2020-07-28 08:29:05.000000 apidev_django-floppyforms-1.8.4/floppyforms/templates/floppyforms/clearable_input.html
--rw-r--r--   0 lucjean    (501) staff       (20)       39 2020-07-28 08:29:05.000000 apidev_django-floppyforms-1.8.4/floppyforms/templates/floppyforms/color.html
--rw-r--r--   0 lucjean    (501) staff       (20)       39 2020-07-28 08:29:05.000000 apidev_django-floppyforms-1.8.4/floppyforms/templates/floppyforms/date.html
--rw-r--r--   0 lucjean    (501) staff       (20)       39 2020-07-28 08:29:05.000000 apidev_django-floppyforms-1.8.4/floppyforms/templates/floppyforms/datetime.html
--rw-r--r--   0 lucjean    (501) staff       (20)       12 2020-07-28 08:29:05.000000 apidev_django-floppyforms-1.8.4/floppyforms/templates/floppyforms/dummy.html
--rw-r--r--   0 lucjean    (501) staff       (20)       39 2020-07-28 08:29:05.000000 apidev_django-floppyforms-1.8.4/floppyforms/templates/floppyforms/email.html
--rw-r--r--   0 lucjean    (501) staff       (20)      111 2020-07-28 08:29:05.000000 apidev_django-floppyforms-1.8.4/floppyforms/templates/floppyforms/errors.html
--rw-r--r--   0 lucjean    (501) staff       (20)       39 2020-07-28 08:29:05.000000 apidev_django-floppyforms-1.8.4/floppyforms/templates/floppyforms/file.html
-drwxr-xr-x   0 lucjean    (501) staff       (20)        0 2020-07-29 15:02:09.140460 apidev_django-floppyforms-1.8.4/floppyforms/templates/floppyforms/gis/
--rw-r--r--   0 lucjean    (501) staff       (20)      233 2020-07-28 08:29:05.000000 apidev_django-floppyforms-1.8.4/floppyforms/templates/floppyforms/gis/google.html
--rw-r--r--   0 lucjean    (501) staff       (20)     1630 2020-07-28 08:29:05.000000 apidev_django-floppyforms-1.8.4/floppyforms/templates/floppyforms/gis/openlayers.html
--rw-r--r--   0 lucjean    (501) staff       (20)      501 2020-07-28 08:29:05.000000 apidev_django-floppyforms-1.8.4/floppyforms/templates/floppyforms/gis/osm.html
--rw-r--r--   0 lucjean    (501) staff       (20)       39 2020-07-28 08:29:05.000000 apidev_django-floppyforms-1.8.4/floppyforms/templates/floppyforms/hidden.html
--rw-r--r--   0 lucjean    (501) staff       (20)      395 2020-07-28 08:29:05.000000 apidev_django-floppyforms-1.8.4/floppyforms/templates/floppyforms/input.html
--rw-r--r--   0 lucjean    (501) staff       (20)       39 2020-07-28 08:29:05.000000 apidev_django-floppyforms-1.8.4/floppyforms/templates/floppyforms/ipaddress.html
-drwxr-xr-x   0 lucjean    (501) staff       (20)        0 2020-07-29 15:02:09.185681 apidev_django-floppyforms-1.8.4/floppyforms/templates/floppyforms/layouts/
--rw-r--r--   0 lucjean    (501) staff       (20)       47 2020-07-28 08:29:05.000000 apidev_django-floppyforms-1.8.4/floppyforms/templates/floppyforms/layouts/default.html
--rw-r--r--   0 lucjean    (501) staff       (20)      996 2020-07-28 08:29:05.000000 apidev_django-floppyforms-1.8.4/floppyforms/templates/floppyforms/layouts/p.html
--rw-r--r--   0 lucjean    (501) staff       (20)     1027 2020-07-28 08:29:05.000000 apidev_django-floppyforms-1.8.4/floppyforms/templates/floppyforms/layouts/table.html
--rw-r--r--   0 lucjean    (501) staff       (20)     1002 2020-07-28 08:29:05.000000 apidev_django-floppyforms-1.8.4/floppyforms/templates/floppyforms/layouts/ul.html
--rw-r--r--   0 lucjean    (501) staff       (20)       39 2020-07-28 08:29:05.000000 apidev_django-floppyforms-1.8.4/floppyforms/templates/floppyforms/number.html
--rw-r--r--   0 lucjean    (501) staff       (20)       39 2020-07-28 08:29:05.000000 apidev_django-floppyforms-1.8.4/floppyforms/templates/floppyforms/password.html
--rw-r--r--   0 lucjean    (501) staff       (20)       39 2020-07-28 08:29:05.000000 apidev_django-floppyforms-1.8.4/floppyforms/templates/floppyforms/phonenumber.html
--rw-r--r--   0 lucjean    (501) staff       (20)      373 2020-07-28 08:29:05.000000 apidev_django-floppyforms-1.8.4/floppyforms/templates/floppyforms/radio.html
--rw-r--r--   0 lucjean    (501) staff       (20)       39 2020-07-28 08:29:05.000000 apidev_django-floppyforms-1.8.4/floppyforms/templates/floppyforms/range.html
-drwxr-xr-x   0 lucjean    (501) staff       (20)        0 2020-07-29 15:02:09.226697 apidev_django-floppyforms-1.8.4/floppyforms/templates/floppyforms/rows/
--rw-r--r--   0 lucjean    (501) staff       (20)       40 2020-07-28 08:29:05.000000 apidev_django-floppyforms-1.8.4/floppyforms/templates/floppyforms/rows/default.html
--rw-r--r--   0 lucjean    (501) staff       (20)     1012 2020-07-28 08:29:05.000000 apidev_django-floppyforms-1.8.4/floppyforms/templates/floppyforms/rows/li.html
--rw-r--r--   0 lucjean    (501) staff       (20)     1007 2020-07-28 08:29:05.000000 apidev_django-floppyforms-1.8.4/floppyforms/templates/floppyforms/rows/p.html
--rw-r--r--   0 lucjean    (501) staff       (20)     1062 2020-07-28 08:29:05.000000 apidev_django-floppyforms-1.8.4/floppyforms/templates/floppyforms/rows/tr.html
--rw-r--r--   0 lucjean    (501) staff       (20)       39 2020-07-28 08:29:05.000000 apidev_django-floppyforms-1.8.4/floppyforms/templates/floppyforms/search.html
--rw-r--r--   0 lucjean    (501) staff       (20)      523 2020-07-28 08:29:05.000000 apidev_django-floppyforms-1.8.4/floppyforms/templates/floppyforms/select.html
--rw-r--r--   0 lucjean    (501) staff       (20)      782 2020-07-28 08:29:05.000000 apidev_django-floppyforms-1.8.4/floppyforms/templates/floppyforms/select_date.html
--rw-r--r--   0 lucjean    (501) staff       (20)       39 2020-07-28 08:29:05.000000 apidev_django-floppyforms-1.8.4/floppyforms/templates/floppyforms/slug.html
--rw-r--r--   0 lucjean    (501) staff       (20)       39 2020-07-28 08:29:05.000000 apidev_django-floppyforms-1.8.4/floppyforms/templates/floppyforms/text.html
--rw-r--r--   0 lucjean    (501) staff       (20)      151 2020-07-28 08:29:05.000000 apidev_django-floppyforms-1.8.4/floppyforms/templates/floppyforms/textarea.html
--rw-r--r--   0 lucjean    (501) staff       (20)       39 2020-07-28 08:29:05.000000 apidev_django-floppyforms-1.8.4/floppyforms/templates/floppyforms/time.html
--rw-r--r--   0 lucjean    (501) staff       (20)       39 2020-07-28 08:29:05.000000 apidev_django-floppyforms-1.8.4/floppyforms/templates/floppyforms/url.html
-drwxr-xr-x   0 lucjean    (501) staff       (20)        0 2020-07-29 15:02:09.247318 apidev_django-floppyforms-1.8.4/floppyforms/templatetags/
--rw-r--r--   0 lucjean    (501) staff       (20)        0 2020-07-28 08:29:05.000000 apidev_django-floppyforms-1.8.4/floppyforms/templatetags/__init__.py
--rw-r--r--   0 lucjean    (501) staff       (20)    25911 2020-07-28 08:29:05.000000 apidev_django-floppyforms-1.8.4/floppyforms/templatetags/floppyforms.py
--rw-r--r--   0 lucjean    (501) staff       (20)      890 2020-07-28 08:30:27.000000 apidev_django-floppyforms-1.8.4/floppyforms/templatetags/floppyforms_internals.py
--rw-r--r--   0 lucjean    (501) staff       (20)    24892 2020-07-28 08:29:05.000000 apidev_django-floppyforms-1.8.4/floppyforms/widgets.py
-drwxr-xr-x   0 lucjean    (501) staff       (20)        0 2020-07-29 15:02:09.269091 apidev_django-floppyforms-1.8.4/requirements/
--rw-r--r--   0 lucjean    (501) staff       (20)       69 2020-07-28 08:29:05.000000 apidev_django-floppyforms-1.8.4/requirements/tests.txt
--rw-r--r--   0 lucjean    (501) staff       (20)       85 2020-07-29 15:02:09.574773 apidev_django-floppyforms-1.8.4/setup.cfg
--rw-r--r--   0 lucjean    (501) staff       (20)     2282 2020-07-28 08:29:05.000000 apidev_django-floppyforms-1.8.4/setup.py
-drwxr-xr-x   0 lucjean    (501) staff       (20)        0 2020-07-29 15:02:09.412771 apidev_django-floppyforms-1.8.4/tests/
--rw-r--r--   0 lucjean    (501) staff       (20)        0 2020-07-28 08:29:05.000000 apidev_django-floppyforms-1.8.4/tests/__init__.py
--rw-r--r--   0 lucjean    (501) staff       (20)      233 2020-07-28 08:29:05.000000 apidev_django-floppyforms-1.8.4/tests/base.py
--rw-r--r--   0 lucjean    (501) staff       (20)      280 2020-07-28 08:29:05.000000 apidev_django-floppyforms-1.8.4/tests/compat.py
-drwxr-xr-x   0 lucjean    (501) staff       (20)        0 2020-07-29 15:02:09.461501 apidev_django-floppyforms-1.8.4/tests/demo/
--rw-r--r--   0 lucjean    (501) staff       (20)        0 2020-07-28 08:29:05.000000 apidev_django-floppyforms-1.8.4/tests/demo/__init__.py
--rw-r--r--   0 lucjean    (501) staff       (20)     2904 2020-07-28 08:29:05.000000 apidev_django-floppyforms-1.8.4/tests/demo/forms.py
--rw-r--r--   0 lucjean    (501) staff       (20)      407 2020-07-28 08:29:05.000000 apidev_django-floppyforms-1.8.4/tests/demo/manage.py
--rw-r--r--   0 lucjean    (501) staff       (20)      616 2020-07-28 08:29:05.000000 apidev_django-floppyforms-1.8.4/tests/demo/settings.py
-drwxr-xr-x   0 lucjean    (501) staff       (20)        0 2020-07-29 15:02:07.696267 apidev_django-floppyforms-1.8.4/tests/demo/templates/
-drwxr-xr-x   0 lucjean    (501) staff       (20)        0 2020-07-29 15:02:09.473629 apidev_django-floppyforms-1.8.4/tests/demo/templates/demo/
--rw-r--r--   0 lucjean    (501) staff       (20)      303 2020-07-28 08:29:05.000000 apidev_django-floppyforms-1.8.4/tests/demo/templates/demo/index.html
--rw-r--r--   0 lucjean    (501) staff       (20)      121 2020-07-28 08:29:05.000000 apidev_django-floppyforms-1.8.4/tests/demo/urls.py
--rw-r--r--   0 lucjean    (501) staff       (20)      401 2020-07-28 08:29:05.000000 apidev_django-floppyforms-1.8.4/tests/demo/views.py
--rw-r--r--   0 lucjean    (501) staff       (20)     1717 2020-07-28 08:29:05.000000 apidev_django-floppyforms-1.8.4/tests/models.py
--rw-r--r--   0 lucjean    (501) staff       (20)     1107 2020-07-28 08:29:05.000000 apidev_django-floppyforms-1.8.4/tests/settings.py
-drwxr-xr-x   0 lucjean    (501) staff       (20)        0 2020-07-29 15:02:09.562126 apidev_django-floppyforms-1.8.4/tests/templates/
--rw-r--r--   0 lucjean    (501) staff       (20)       42 2020-07-28 08:29:05.000000 apidev_django-floppyforms-1.8.4/tests/templates/custom.html
--rw-r--r--   0 lucjean    (501) staff       (20)       78 2020-07-28 08:29:05.000000 apidev_django-floppyforms-1.8.4/tests/templates/extra_argument.html
--rw-r--r--   0 lucjean    (501) staff       (20)      161 2020-07-28 08:29:05.000000 apidev_django-floppyforms-1.8.4/tests/templates/extra_argument_with_config.html
--rw-r--r--   0 lucjean    (501) staff       (20)      142 2020-07-28 08:29:05.000000 apidev_django-floppyforms-1.8.4/tests/templates/formconfig_inside_only.html
--rw-r--r--   0 lucjean    (501) staff       (20)      109 2020-07-28 08:29:05.000000 apidev_django-floppyforms-1.8.4/tests/templates/media_widget.html
--rw-r--r--   0 lucjean    (501) staff       (20)      223 2020-07-28 08:29:05.000000 apidev_django-floppyforms-1.8.4/tests/templates/simple_form_tag.html
--rw-r--r--   0 lucjean    (501) staff       (20)       88 2020-07-28 08:29:05.000000 apidev_django-floppyforms-1.8.4/tests/templates/simple_formfield_tag.html
--rw-r--r--   0 lucjean    (501) staff       (20)      185 2020-07-28 08:29:05.000000 apidev_django-floppyforms-1.8.4/tests/templates/simple_formrow_tag.html
--rw-r--r--   0 lucjean    (501) staff       (20)      382 2020-07-28 08:29:05.000000 apidev_django-floppyforms-1.8.4/tests/templates/simple_formrow_tag_with_config.html
--rw-r--r--   0 lucjean    (501) staff       (20)      892 2020-07-28 08:29:05.000000 apidev_django-floppyforms-1.8.4/tests/test_deprecations.py
--rw-r--r--   0 lucjean    (501) staff       (20)     5842 2020-07-28 08:29:05.000000 apidev_django-floppyforms-1.8.4/tests/test_fields.py
--rw-r--r--   0 lucjean    (501) staff       (20)     5665 2020-07-28 08:29:05.000000 apidev_django-floppyforms-1.8.4/tests/test_forms.py
--rw-r--r--   0 lucjean    (501) staff       (20)    13294 2020-07-28 08:29:05.000000 apidev_django-floppyforms-1.8.4/tests/test_gis.py
--rw-r--r--   0 lucjean    (501) staff       (20)    28709 2020-07-28 08:29:05.000000 apidev_django-floppyforms-1.8.4/tests/test_layouts.py
--rw-r--r--   0 lucjean    (501) staff       (20)     8293 2020-07-28 08:29:05.000000 apidev_django-floppyforms-1.8.4/tests/test_modelforms.py
--rw-r--r--   0 lucjean    (501) staff       (20)     8582 2020-07-28 08:29:05.000000 apidev_django-floppyforms-1.8.4/tests/test_rendering.py
--rw-r--r--   0 lucjean    (501) staff       (20)    33976 2020-07-28 08:29:05.000000 apidev_django-floppyforms-1.8.4/tests/test_templatetags.py
--rw-r--r--   0 lucjean    (501) staff       (20)    50159 2020-07-28 08:29:05.000000 apidev_django-floppyforms-1.8.4/tests/test_widgets.py
--rw-r--r--   0 lucjean    (501) staff       (20)      282 2020-07-28 08:29:05.000000 apidev_django-floppyforms-1.8.4/tests/tests.py
+drwxrwxr-x   0 lucjean   (1001) lucjean   (1001)        0 2023-06-12 12:55:38.740151 apidev_django-floppyforms-1.9.0/
+-rw-rw-r--   0 lucjean   (1001) lucjean   (1001)     8935 2023-05-22 10:15:50.000000 apidev_django-floppyforms-1.9.0/CHANGES.rst
+-rw-rw-r--   0 lucjean   (1001) lucjean   (1001)     3133 2023-05-22 10:15:50.000000 apidev_django-floppyforms-1.9.0/LICENSE
+-rw-rw-r--   0 lucjean   (1001) lucjean   (1001)      340 2023-05-22 10:15:50.000000 apidev_django-floppyforms-1.9.0/MANIFEST.in
+-rw-rw-r--   0 lucjean   (1001) lucjean   (1001)    11073 2023-06-12 12:55:38.740151 apidev_django-floppyforms-1.9.0/PKG-INFO
+-rw-rw-r--   0 lucjean   (1001) lucjean   (1001)      680 2023-05-22 10:15:50.000000 apidev_django-floppyforms-1.9.0/README.rst
+drwxrwxr-x   0 lucjean   (1001) lucjean   (1001)        0 2023-06-12 12:55:38.720151 apidev_django-floppyforms-1.9.0/apidev_django_floppyforms.egg-info/
+-rw-rw-r--   0 lucjean   (1001) lucjean   (1001)    11073 2023-06-12 12:55:38.000000 apidev_django-floppyforms-1.9.0/apidev_django_floppyforms.egg-info/PKG-INFO
+-rw-rw-r--   0 lucjean   (1001) lucjean   (1001)     7185 2023-06-12 12:55:38.000000 apidev_django-floppyforms-1.9.0/apidev_django_floppyforms.egg-info/SOURCES.txt
+-rw-rw-r--   0 lucjean   (1001) lucjean   (1001)        1 2023-06-12 12:55:38.000000 apidev_django-floppyforms-1.9.0/apidev_django_floppyforms.egg-info/dependency_links.txt
+-rw-rw-r--   0 lucjean   (1001) lucjean   (1001)        1 2023-05-22 10:25:37.000000 apidev_django-floppyforms-1.9.0/apidev_django_floppyforms.egg-info/not-zip-safe
+-rw-rw-r--   0 lucjean   (1001) lucjean   (1001)       12 2023-06-12 12:55:38.000000 apidev_django-floppyforms-1.9.0/apidev_django_floppyforms.egg-info/top_level.txt
+drwxrwxr-x   0 lucjean   (1001) lucjean   (1001)        0 2023-06-12 12:55:38.724151 apidev_django-floppyforms-1.9.0/docs/
+-rw-rw-r--   0 lucjean   (1001) lucjean   (1001)     4638 2023-05-22 10:15:50.000000 apidev_django-floppyforms-1.9.0/docs/Makefile
+-rw-rw-r--   0 lucjean   (1001) lucjean   (1001)     3427 2023-05-22 10:15:50.000000 apidev_django-floppyforms-1.9.0/docs/bootstrap.rst
+-rw-rw-r--   0 lucjean   (1001) lucjean   (1001)       28 2023-05-22 10:15:50.000000 apidev_django-floppyforms-1.9.0/docs/changelog.rst
+-rw-rw-r--   0 lucjean   (1001) lucjean   (1001)     7318 2023-05-22 10:15:50.000000 apidev_django-floppyforms-1.9.0/docs/conf.py
+-rw-rw-r--   0 lucjean   (1001) lucjean   (1001)     3927 2023-05-22 10:15:50.000000 apidev_django-floppyforms-1.9.0/docs/customization.rst
+-rw-rw-r--   0 lucjean   (1001) lucjean   (1001)     7186 2023-05-22 10:15:50.000000 apidev_django-floppyforms-1.9.0/docs/differences.rst
+-rw-rw-r--   0 lucjean   (1001) lucjean   (1001)     6575 2023-05-22 10:15:50.000000 apidev_django-floppyforms-1.9.0/docs/examples.rst
+-rw-rw-r--   0 lucjean   (1001) lucjean   (1001)    15514 2023-05-22 10:15:50.000000 apidev_django-floppyforms-1.9.0/docs/geodjango.rst
+drwxrwxr-x   0 lucjean   (1001) lucjean   (1001)        0 2023-06-12 12:55:38.724151 apidev_django-floppyforms-1.9.0/docs/images/
+-rw-rw-r--   0 lucjean   (1001) lucjean   (1001)     2071 2023-05-22 10:15:50.000000 apidev_django-floppyforms-1.9.0/docs/images/datepicker-chromium.png
+-rw-rw-r--   0 lucjean   (1001) lucjean   (1001)    15545 2023-05-22 10:15:50.000000 apidev_django-floppyforms-1.9.0/docs/images/datepicker-jquery-ui.png
+-rw-rw-r--   0 lucjean   (1001) lucjean   (1001)   228293 2023-05-22 10:15:50.000000 apidev_django-floppyforms-1.9.0/docs/images/geomcollection.png
+-rw-rw-r--   0 lucjean   (1001) lucjean   (1001)   323935 2023-05-22 10:15:50.000000 apidev_django-floppyforms-1.9.0/docs/images/gmappoly.png
+-rw-rw-r--   0 lucjean   (1001) lucjean   (1001)    26810 2023-05-22 10:15:50.000000 apidev_django-floppyforms-1.9.0/docs/images/image_with_thumbnail.png
+-rw-rw-r--   0 lucjean   (1001) lucjean   (1001)   343359 2023-05-22 10:15:50.000000 apidev_django-floppyforms-1.9.0/docs/images/osmlinestring.png
+-rw-rw-r--   0 lucjean   (1001) lucjean   (1001)   119517 2023-05-22 10:15:50.000000 apidev_django-floppyforms-1.9.0/docs/images/pointfield.png
+-rw-rw-r--   0 lucjean   (1001) lucjean   (1001)      845 2023-05-22 10:15:50.000000 apidev_django-floppyforms-1.9.0/docs/images/slider-chromium.png
+-rw-rw-r--   0 lucjean   (1001) lucjean   (1001)     1452 2023-05-22 10:15:50.000000 apidev_django-floppyforms-1.9.0/docs/images/slider-jquery-ui.png
+-rw-rw-r--   0 lucjean   (1001) lucjean   (1001)     4163 2023-05-22 10:15:50.000000 apidev_django-floppyforms-1.9.0/docs/index.rst
+-rw-rw-r--   0 lucjean   (1001) lucjean   (1001)    11815 2023-05-22 10:15:50.000000 apidev_django-floppyforms-1.9.0/docs/layouts.rst
+-rw-rw-r--   0 lucjean   (1001) lucjean   (1001)     8377 2023-05-22 10:15:50.000000 apidev_django-floppyforms-1.9.0/docs/templatetags.rst
+-rw-rw-r--   0 lucjean   (1001) lucjean   (1001)     5354 2023-05-22 10:15:50.000000 apidev_django-floppyforms-1.9.0/docs/usage.rst
+-rw-rw-r--   0 lucjean   (1001) lucjean   (1001)     7732 2023-05-22 10:15:50.000000 apidev_django-floppyforms-1.9.0/docs/widgets-reference.rst
+-rw-rw-r--   0 lucjean   (1001) lucjean   (1001)     4460 2023-05-22 10:15:50.000000 apidev_django-floppyforms-1.9.0/docs/widgets.rst
+drwxrwxr-x   0 lucjean   (1001) lucjean   (1001)        0 2023-06-12 12:55:38.728151 apidev_django-floppyforms-1.9.0/floppyforms/
+drwxrwxr-x   0 lucjean   (1001) lucjean   (1001)        0 2023-06-12 12:55:38.728151 apidev_django-floppyforms-1.9.0/floppyforms/__deprecated__/
+-rw-r--r--   0 lucjean   (1001) lucjean   (1001)        0 2023-06-12 12:50:34.000000 apidev_django-floppyforms-1.9.0/floppyforms/__deprecated__/__init__.py
+-rw-r--r--   0 lucjean   (1001) lucjean   (1001)     1079 2023-06-12 12:50:34.000000 apidev_django-floppyforms-1.9.0/floppyforms/__deprecated__/models.py
+drwxrwxr-x   0 lucjean   (1001) lucjean   (1001)        0 2023-06-12 12:55:38.728151 apidev_django-floppyforms-1.9.0/floppyforms/__future__/
+-rw-rw-r--   0 lucjean   (1001) lucjean   (1001)      236 2023-06-12 12:50:34.000000 apidev_django-floppyforms-1.9.0/floppyforms/__future__/__init__.py
+-rw-rw-r--   0 lucjean   (1001) lucjean   (1001)      272 2023-06-12 12:50:34.000000 apidev_django-floppyforms-1.9.0/floppyforms/__init__.py
+-rw-rw-r--   0 lucjean   (1001) lucjean   (1001)     1741 2023-06-12 12:50:34.000000 apidev_django-floppyforms-1.9.0/floppyforms/compat.py
+-rw-rw-r--   0 lucjean   (1001) lucjean   (1001)     5545 2023-06-12 12:50:34.000000 apidev_django-floppyforms-1.9.0/floppyforms/fields.py
+-rw-rw-r--   0 lucjean   (1001) lucjean   (1001)      980 2023-06-12 12:50:34.000000 apidev_django-floppyforms-1.9.0/floppyforms/forms.py
+drwxrwxr-x   0 lucjean   (1001) lucjean   (1001)        0 2023-06-12 12:55:38.728151 apidev_django-floppyforms-1.9.0/floppyforms/gis/
+-rw-rw-r--   0 lucjean   (1001) lucjean   (1001)       60 2023-05-22 10:15:50.000000 apidev_django-floppyforms-1.9.0/floppyforms/gis/__init__.py
+-rw-rw-r--   0 lucjean   (1001) lucjean   (1001)     3013 2023-05-22 10:15:50.000000 apidev_django-floppyforms-1.9.0/floppyforms/gis/fields.py
+-rw-rw-r--   0 lucjean   (1001) lucjean   (1001)     5627 2023-05-22 10:15:50.000000 apidev_django-floppyforms-1.9.0/floppyforms/gis/widgets.py
+-rw-rw-r--   0 lucjean   (1001) lucjean   (1001)     4793 2023-06-12 12:50:34.000000 apidev_django-floppyforms-1.9.0/floppyforms/models.py
+drwxrwxr-x   0 lucjean   (1001) lucjean   (1001)        0 2023-06-12 12:55:38.720151 apidev_django-floppyforms-1.9.0/floppyforms/static/
+drwxrwxr-x   0 lucjean   (1001) lucjean   (1001)        0 2023-06-12 12:55:38.720151 apidev_django-floppyforms-1.9.0/floppyforms/static/floppyforms/
+drwxrwxr-x   0 lucjean   (1001) lucjean   (1001)        0 2023-06-12 12:55:38.720151 apidev_django-floppyforms-1.9.0/floppyforms/static/floppyforms/gis/
+drwxrwxr-x   0 lucjean   (1001) lucjean   (1001)        0 2023-06-12 12:55:38.728151 apidev_django-floppyforms-1.9.0/floppyforms/static/floppyforms/gis/img/
+-rw-rw-r--   0 lucjean   (1001) lucjean   (1001)      711 2023-05-22 10:15:50.000000 apidev_django-floppyforms-1.9.0/floppyforms/static/floppyforms/gis/img/move_vertex_off.png
+-rw-rw-r--   0 lucjean   (1001) lucjean   (1001)      506 2023-05-22 10:15:50.000000 apidev_django-floppyforms-1.9.0/floppyforms/static/floppyforms/gis/img/move_vertex_on.png
+drwxrwxr-x   0 lucjean   (1001) lucjean   (1001)        0 2023-06-12 12:55:38.728151 apidev_django-floppyforms-1.9.0/floppyforms/static/floppyforms/js/
+-rw-rw-r--   0 lucjean   (1001) lucjean   (1001)    12292 2023-05-22 10:15:50.000000 apidev_django-floppyforms-1.9.0/floppyforms/static/floppyforms/js/MapWidget.js
+drwxrwxr-x   0 lucjean   (1001) lucjean   (1001)        0 2023-06-12 12:55:38.728151 apidev_django-floppyforms-1.9.0/floppyforms/static/floppyforms/openlayers/
+-rw-rw-r--   0 lucjean   (1001) lucjean   (1001)   770300 2023-05-22 10:15:50.000000 apidev_django-floppyforms-1.9.0/floppyforms/static/floppyforms/openlayers/OpenLayers.js
+drwxrwxr-x   0 lucjean   (1001) lucjean   (1001)        0 2023-06-12 12:55:38.720151 apidev_django-floppyforms-1.9.0/floppyforms/static/floppyforms/openlayers/theme/
+drwxrwxr-x   0 lucjean   (1001) lucjean   (1001)        0 2023-06-12 12:55:38.728151 apidev_django-floppyforms-1.9.0/floppyforms/static/floppyforms/openlayers/theme/default/
+-rw-rw-r--   0 lucjean   (1001) lucjean   (1001)      142 2023-05-22 10:15:50.000000 apidev_django-floppyforms-1.9.0/floppyforms/static/floppyforms/openlayers/theme/default/google.css
+-rw-rw-r--   0 lucjean   (1001) lucjean   (1001)      212 2023-05-22 10:15:50.000000 apidev_django-floppyforms-1.9.0/floppyforms/static/floppyforms/openlayers/theme/default/ie6-style.css
+drwxrwxr-x   0 lucjean   (1001) lucjean   (1001)        0 2023-06-12 12:55:38.732151 apidev_django-floppyforms-1.9.0/floppyforms/static/floppyforms/openlayers/theme/default/img/
+-rw-rw-r--   0 lucjean   (1001) lucjean   (1001)     1614 2023-05-22 10:15:50.000000 apidev_django-floppyforms-1.9.0/floppyforms/static/floppyforms/openlayers/theme/default/img/add_point_off.png
+-rw-rw-r--   0 lucjean   (1001) lucjean   (1001)     1464 2023-05-22 10:15:50.000000 apidev_django-floppyforms-1.9.0/floppyforms/static/floppyforms/openlayers/theme/default/img/add_point_on.png
+-rw-rw-r--   0 lucjean   (1001) lucjean   (1001)       42 2023-05-22 10:15:50.000000 apidev_django-floppyforms-1.9.0/floppyforms/static/floppyforms/openlayers/theme/default/img/blank.gif
+-rw-rw-r--   0 lucjean   (1001) lucjean   (1001)     1078 2023-05-22 10:15:50.000000 apidev_django-floppyforms-1.9.0/floppyforms/static/floppyforms/openlayers/theme/default/img/close.gif
+-rw-rw-r--   0 lucjean   (1001) lucjean   (1001)     1024 2023-05-22 10:15:50.000000 apidev_django-floppyforms-1.9.0/floppyforms/static/floppyforms/openlayers/theme/default/img/drag-rectangle-off.png
+-rw-rw-r--   0 lucjean   (1001) lucjean   (1001)     1041 2023-05-22 10:15:50.000000 apidev_django-floppyforms-1.9.0/floppyforms/static/floppyforms/openlayers/theme/default/img/drag-rectangle-on.png
+-rw-rw-r--   0 lucjean   (1001) lucjean   (1001)     1565 2023-05-22 10:15:50.000000 apidev_django-floppyforms-1.9.0/floppyforms/static/floppyforms/openlayers/theme/default/img/draw_line_off.png
+-rw-rw-r--   0 lucjean   (1001) lucjean   (1001)     1396 2023-05-22 10:15:50.000000 apidev_django-floppyforms-1.9.0/floppyforms/static/floppyforms/openlayers/theme/default/img/draw_line_on.png
+-rw-rw-r--   0 lucjean   (1001) lucjean   (1001)     1610 2023-05-22 10:15:50.000000 apidev_django-floppyforms-1.9.0/floppyforms/static/floppyforms/openlayers/theme/default/img/draw_point_off.png
+-rw-rw-r--   0 lucjean   (1001) lucjean   (1001)     1458 2023-05-22 10:15:50.000000 apidev_django-floppyforms-1.9.0/floppyforms/static/floppyforms/openlayers/theme/default/img/draw_point_on.png
+-rw-rw-r--   0 lucjean   (1001) lucjean   (1001)     1544 2023-05-22 10:15:50.000000 apidev_django-floppyforms-1.9.0/floppyforms/static/floppyforms/openlayers/theme/default/img/draw_polygon_off.png
+-rw-rw-r--   0 lucjean   (1001) lucjean   (1001)     1405 2023-05-22 10:15:50.000000 apidev_django-floppyforms-1.9.0/floppyforms/static/floppyforms/openlayers/theme/default/img/draw_polygon_on.png
+-rw-rw-r--   0 lucjean   (1001) lucjean   (1001)     2222 2023-05-22 10:15:50.000000 apidev_django-floppyforms-1.9.0/floppyforms/static/floppyforms/openlayers/theme/default/img/editing_tool_bar.png
+-rw-rw-r--   0 lucjean   (1001) lucjean   (1001)     1541 2023-05-22 10:15:50.000000 apidev_django-floppyforms-1.9.0/floppyforms/static/floppyforms/openlayers/theme/default/img/move_feature_off.png
+-rw-rw-r--   0 lucjean   (1001) lucjean   (1001)     1377 2023-05-22 10:15:50.000000 apidev_django-floppyforms-1.9.0/floppyforms/static/floppyforms/openlayers/theme/default/img/move_feature_on.png
+-rw-rw-r--   0 lucjean   (1001) lucjean   (1001)     6628 2023-05-22 10:15:50.000000 apidev_django-floppyforms-1.9.0/floppyforms/static/floppyforms/openlayers/theme/default/img/navigation_history.png
+-rw-rw-r--   0 lucjean   (1001) lucjean   (1001)       79 2023-05-22 10:15:50.000000 apidev_django-floppyforms-1.9.0/floppyforms/static/floppyforms/openlayers/theme/default/img/overview_replacement.gif
+-rw-rw-r--   0 lucjean   (1001) lucjean   (1001)      564 2023-05-22 10:15:50.000000 apidev_django-floppyforms-1.9.0/floppyforms/static/floppyforms/openlayers/theme/default/img/pan-panel-NOALPHA.png
+-rw-rw-r--   0 lucjean   (1001) lucjean   (1001)      814 2023-05-22 10:15:50.000000 apidev_django-floppyforms-1.9.0/floppyforms/static/floppyforms/openlayers/theme/default/img/pan-panel.png
+-rw-rw-r--   0 lucjean   (1001) lucjean   (1001)     1696 2023-05-22 10:15:50.000000 apidev_django-floppyforms-1.9.0/floppyforms/static/floppyforms/openlayers/theme/default/img/pan_off.png
+-rw-rw-r--   0 lucjean   (1001) lucjean   (1001)     1566 2023-05-22 10:15:50.000000 apidev_django-floppyforms-1.9.0/floppyforms/static/floppyforms/openlayers/theme/default/img/pan_on.png
+-rw-rw-r--   0 lucjean   (1001) lucjean   (1001)     3511 2023-05-22 10:15:50.000000 apidev_django-floppyforms-1.9.0/floppyforms/static/floppyforms/openlayers/theme/default/img/panning-hand-off.png
+-rw-rw-r--   0 lucjean   (1001) lucjean   (1001)     3565 2023-05-22 10:15:50.000000 apidev_django-floppyforms-1.9.0/floppyforms/static/floppyforms/openlayers/theme/default/img/panning-hand-on.png
+-rw-rw-r--   0 lucjean   (1001) lucjean   (1001)     1612 2023-05-22 10:15:50.000000 apidev_django-floppyforms-1.9.0/floppyforms/static/floppyforms/openlayers/theme/default/img/remove_point_off.png
+-rw-rw-r--   0 lucjean   (1001) lucjean   (1001)     1461 2023-05-22 10:15:50.000000 apidev_django-floppyforms-1.9.0/floppyforms/static/floppyforms/openlayers/theme/default/img/remove_point_on.png
+-rw-rw-r--   0 lucjean   (1001) lucjean   (1001)     1211 2023-05-22 10:15:50.000000 apidev_django-floppyforms-1.9.0/floppyforms/static/floppyforms/openlayers/theme/default/img/ruler.png
+-rw-rw-r--   0 lucjean   (1001) lucjean   (1001)      354 2023-05-22 10:15:50.000000 apidev_django-floppyforms-1.9.0/floppyforms/static/floppyforms/openlayers/theme/default/img/save_features_off.png
+-rw-rw-r--   0 lucjean   (1001) lucjean   (1001)      361 2023-05-22 10:15:50.000000 apidev_django-floppyforms-1.9.0/floppyforms/static/floppyforms/openlayers/theme/default/img/save_features_on.png
+-rw-rw-r--   0 lucjean   (1001) lucjean   (1001)     1499 2023-05-22 10:15:50.000000 apidev_django-floppyforms-1.9.0/floppyforms/static/floppyforms/openlayers/theme/default/img/view_next_off.png
+-rw-rw-r--   0 lucjean   (1001) lucjean   (1001)     1686 2023-05-22 10:15:50.000000 apidev_django-floppyforms-1.9.0/floppyforms/static/floppyforms/openlayers/theme/default/img/view_next_on.png
+-rw-rw-r--   0 lucjean   (1001) lucjean   (1001)     1476 2023-05-22 10:15:50.000000 apidev_django-floppyforms-1.9.0/floppyforms/static/floppyforms/openlayers/theme/default/img/view_previous_off.png
+-rw-rw-r--   0 lucjean   (1001) lucjean   (1001)     1592 2023-05-22 10:15:50.000000 apidev_django-floppyforms-1.9.0/floppyforms/static/floppyforms/openlayers/theme/default/img/view_previous_on.png
+-rw-rw-r--   0 lucjean   (1001) lucjean   (1001)     1173 2023-05-22 10:15:50.000000 apidev_django-floppyforms-1.9.0/floppyforms/static/floppyforms/openlayers/theme/default/img/zoom-panel-NOALPHA.png
+-rw-rw-r--   0 lucjean   (1001) lucjean   (1001)     1285 2023-05-22 10:15:50.000000 apidev_django-floppyforms-1.9.0/floppyforms/static/floppyforms/openlayers/theme/default/img/zoom-panel.png
+-rw-rw-r--   0 lucjean   (1001) lucjean   (1001)    10791 2023-05-22 10:15:50.000000 apidev_django-floppyforms-1.9.0/floppyforms/static/floppyforms/openlayers/theme/default/style.css
+-rw-rw-r--   0 lucjean   (1001) lucjean   (1001)     1799 2023-05-22 10:15:50.000000 apidev_django-floppyforms-1.9.0/floppyforms/static/floppyforms/openlayers/theme/default/style.mobile.css
+drwxrwxr-x   0 lucjean   (1001) lucjean   (1001)        0 2023-06-12 12:55:38.720151 apidev_django-floppyforms-1.9.0/floppyforms/templates/
+drwxrwxr-x   0 lucjean   (1001) lucjean   (1001)        0 2023-06-12 12:55:38.736151 apidev_django-floppyforms-1.9.0/floppyforms/templates/floppyforms/
+-rw-rw-r--   0 lucjean   (1001) lucjean   (1001)      107 2023-05-22 10:15:50.000000 apidev_django-floppyforms-1.9.0/floppyforms/templates/floppyforms/_render_as.html
+-rw-rw-r--   0 lucjean   (1001) lucjean   (1001)      492 2023-05-22 10:15:50.000000 apidev_django-floppyforms-1.9.0/floppyforms/templates/floppyforms/attrs.html
+-rw-rw-r--   0 lucjean   (1001) lucjean   (1001)       39 2023-05-22 10:15:50.000000 apidev_django-floppyforms-1.9.0/floppyforms/templates/floppyforms/checkbox.html
+-rw-rw-r--   0 lucjean   (1001) lucjean   (1001)      349 2023-05-22 10:15:50.000000 apidev_django-floppyforms-1.9.0/floppyforms/templates/floppyforms/checkbox_select.html
+-rw-rw-r--   0 lucjean   (1001) lucjean   (1001)      440 2023-05-22 10:15:50.000000 apidev_django-floppyforms-1.9.0/floppyforms/templates/floppyforms/clearable_input.html
+-rw-rw-r--   0 lucjean   (1001) lucjean   (1001)       39 2023-05-22 10:15:50.000000 apidev_django-floppyforms-1.9.0/floppyforms/templates/floppyforms/color.html
+-rw-rw-r--   0 lucjean   (1001) lucjean   (1001)       39 2023-05-22 10:15:50.000000 apidev_django-floppyforms-1.9.0/floppyforms/templates/floppyforms/date.html
+-rw-rw-r--   0 lucjean   (1001) lucjean   (1001)       39 2023-05-22 10:15:50.000000 apidev_django-floppyforms-1.9.0/floppyforms/templates/floppyforms/datetime.html
+-rw-rw-r--   0 lucjean   (1001) lucjean   (1001)       12 2023-05-22 10:15:50.000000 apidev_django-floppyforms-1.9.0/floppyforms/templates/floppyforms/dummy.html
+-rw-rw-r--   0 lucjean   (1001) lucjean   (1001)       39 2023-05-22 10:15:50.000000 apidev_django-floppyforms-1.9.0/floppyforms/templates/floppyforms/email.html
+-rw-rw-r--   0 lucjean   (1001) lucjean   (1001)      111 2023-05-22 10:15:50.000000 apidev_django-floppyforms-1.9.0/floppyforms/templates/floppyforms/errors.html
+-rw-rw-r--   0 lucjean   (1001) lucjean   (1001)       39 2023-05-22 10:15:50.000000 apidev_django-floppyforms-1.9.0/floppyforms/templates/floppyforms/file.html
+drwxrwxr-x   0 lucjean   (1001) lucjean   (1001)        0 2023-06-12 12:55:38.736151 apidev_django-floppyforms-1.9.0/floppyforms/templates/floppyforms/gis/
+-rw-rw-r--   0 lucjean   (1001) lucjean   (1001)      233 2023-05-22 10:15:50.000000 apidev_django-floppyforms-1.9.0/floppyforms/templates/floppyforms/gis/google.html
+-rw-rw-r--   0 lucjean   (1001) lucjean   (1001)     1630 2023-05-22 10:15:50.000000 apidev_django-floppyforms-1.9.0/floppyforms/templates/floppyforms/gis/openlayers.html
+-rw-rw-r--   0 lucjean   (1001) lucjean   (1001)      501 2023-05-22 10:15:50.000000 apidev_django-floppyforms-1.9.0/floppyforms/templates/floppyforms/gis/osm.html
+-rw-rw-r--   0 lucjean   (1001) lucjean   (1001)       39 2023-05-22 10:15:50.000000 apidev_django-floppyforms-1.9.0/floppyforms/templates/floppyforms/hidden.html
+-rw-rw-r--   0 lucjean   (1001) lucjean   (1001)      395 2023-05-22 10:15:50.000000 apidev_django-floppyforms-1.9.0/floppyforms/templates/floppyforms/input.html
+-rw-rw-r--   0 lucjean   (1001) lucjean   (1001)       39 2023-05-22 10:15:50.000000 apidev_django-floppyforms-1.9.0/floppyforms/templates/floppyforms/ipaddress.html
+drwxrwxr-x   0 lucjean   (1001) lucjean   (1001)        0 2023-06-12 12:55:38.736151 apidev_django-floppyforms-1.9.0/floppyforms/templates/floppyforms/layouts/
+-rw-rw-r--   0 lucjean   (1001) lucjean   (1001)       47 2023-05-22 10:15:50.000000 apidev_django-floppyforms-1.9.0/floppyforms/templates/floppyforms/layouts/default.html
+-rw-rw-r--   0 lucjean   (1001) lucjean   (1001)      996 2023-05-22 10:15:50.000000 apidev_django-floppyforms-1.9.0/floppyforms/templates/floppyforms/layouts/p.html
+-rw-rw-r--   0 lucjean   (1001) lucjean   (1001)     1027 2023-05-22 10:15:50.000000 apidev_django-floppyforms-1.9.0/floppyforms/templates/floppyforms/layouts/table.html
+-rw-rw-r--   0 lucjean   (1001) lucjean   (1001)     1002 2023-05-22 10:15:50.000000 apidev_django-floppyforms-1.9.0/floppyforms/templates/floppyforms/layouts/ul.html
+-rw-rw-r--   0 lucjean   (1001) lucjean   (1001)       39 2023-05-22 10:15:50.000000 apidev_django-floppyforms-1.9.0/floppyforms/templates/floppyforms/number.html
+-rw-rw-r--   0 lucjean   (1001) lucjean   (1001)       39 2023-05-22 10:15:50.000000 apidev_django-floppyforms-1.9.0/floppyforms/templates/floppyforms/password.html
+-rw-rw-r--   0 lucjean   (1001) lucjean   (1001)       39 2023-05-22 10:15:50.000000 apidev_django-floppyforms-1.9.0/floppyforms/templates/floppyforms/phonenumber.html
+-rw-rw-r--   0 lucjean   (1001) lucjean   (1001)      373 2023-05-22 10:15:50.000000 apidev_django-floppyforms-1.9.0/floppyforms/templates/floppyforms/radio.html
+-rw-rw-r--   0 lucjean   (1001) lucjean   (1001)       39 2023-05-22 10:15:50.000000 apidev_django-floppyforms-1.9.0/floppyforms/templates/floppyforms/range.html
+drwxrwxr-x   0 lucjean   (1001) lucjean   (1001)        0 2023-06-12 12:55:38.736151 apidev_django-floppyforms-1.9.0/floppyforms/templates/floppyforms/rows/
+-rw-rw-r--   0 lucjean   (1001) lucjean   (1001)       40 2023-05-22 10:15:50.000000 apidev_django-floppyforms-1.9.0/floppyforms/templates/floppyforms/rows/default.html
+-rw-rw-r--   0 lucjean   (1001) lucjean   (1001)     1012 2023-05-22 10:15:50.000000 apidev_django-floppyforms-1.9.0/floppyforms/templates/floppyforms/rows/li.html
+-rw-rw-r--   0 lucjean   (1001) lucjean   (1001)     1007 2023-05-22 10:15:50.000000 apidev_django-floppyforms-1.9.0/floppyforms/templates/floppyforms/rows/p.html
+-rw-rw-r--   0 lucjean   (1001) lucjean   (1001)     1062 2023-05-22 10:15:50.000000 apidev_django-floppyforms-1.9.0/floppyforms/templates/floppyforms/rows/tr.html
+-rw-rw-r--   0 lucjean   (1001) lucjean   (1001)       39 2023-05-22 10:15:50.000000 apidev_django-floppyforms-1.9.0/floppyforms/templates/floppyforms/search.html
+-rw-rw-r--   0 lucjean   (1001) lucjean   (1001)      523 2023-05-22 10:15:50.000000 apidev_django-floppyforms-1.9.0/floppyforms/templates/floppyforms/select.html
+-rw-rw-r--   0 lucjean   (1001) lucjean   (1001)      782 2023-05-22 10:15:50.000000 apidev_django-floppyforms-1.9.0/floppyforms/templates/floppyforms/select_date.html
+-rw-rw-r--   0 lucjean   (1001) lucjean   (1001)       39 2023-05-22 10:15:50.000000 apidev_django-floppyforms-1.9.0/floppyforms/templates/floppyforms/slug.html
+-rw-rw-r--   0 lucjean   (1001) lucjean   (1001)       39 2023-05-22 10:15:50.000000 apidev_django-floppyforms-1.9.0/floppyforms/templates/floppyforms/text.html
+-rw-rw-r--   0 lucjean   (1001) lucjean   (1001)      151 2023-05-22 10:15:50.000000 apidev_django-floppyforms-1.9.0/floppyforms/templates/floppyforms/textarea.html
+-rw-rw-r--   0 lucjean   (1001) lucjean   (1001)       39 2023-05-22 10:15:50.000000 apidev_django-floppyforms-1.9.0/floppyforms/templates/floppyforms/time.html
+-rw-rw-r--   0 lucjean   (1001) lucjean   (1001)       39 2023-05-22 10:15:50.000000 apidev_django-floppyforms-1.9.0/floppyforms/templates/floppyforms/url.html
+drwxrwxr-x   0 lucjean   (1001) lucjean   (1001)        0 2023-06-12 12:55:38.736151 apidev_django-floppyforms-1.9.0/floppyforms/templatetags/
+-rw-rw-r--   0 lucjean   (1001) lucjean   (1001)        0 2023-05-22 10:15:50.000000 apidev_django-floppyforms-1.9.0/floppyforms/templatetags/__init__.py
+-rw-rw-r--   0 lucjean   (1001) lucjean   (1001)    25800 2023-06-12 12:50:34.000000 apidev_django-floppyforms-1.9.0/floppyforms/templatetags/floppyforms.py
+-rw-rw-r--   0 lucjean   (1001) lucjean   (1001)      890 2023-05-22 10:15:50.000000 apidev_django-floppyforms-1.9.0/floppyforms/templatetags/floppyforms_internals.py
+-rw-rw-r--   0 lucjean   (1001) lucjean   (1001)    24750 2023-06-12 12:50:34.000000 apidev_django-floppyforms-1.9.0/floppyforms/widgets.py
+drwxrwxr-x   0 lucjean   (1001) lucjean   (1001)        0 2023-06-12 12:55:38.736151 apidev_django-floppyforms-1.9.0/requirements/
+-rw-rw-r--   0 lucjean   (1001) lucjean   (1001)       69 2023-05-22 10:15:50.000000 apidev_django-floppyforms-1.9.0/requirements/tests.txt
+-rw-rw-r--   0 lucjean   (1001) lucjean   (1001)       85 2023-06-12 12:55:38.740151 apidev_django-floppyforms-1.9.0/setup.cfg
+-rw-rw-r--   0 lucjean   (1001) lucjean   (1001)     2282 2023-05-22 10:15:50.000000 apidev_django-floppyforms-1.9.0/setup.py
+drwxrwxr-x   0 lucjean   (1001) lucjean   (1001)        0 2023-06-12 12:55:38.736151 apidev_django-floppyforms-1.9.0/tests/
+-rw-rw-r--   0 lucjean   (1001) lucjean   (1001)        0 2023-05-22 10:15:50.000000 apidev_django-floppyforms-1.9.0/tests/__init__.py
+-rw-rw-r--   0 lucjean   (1001) lucjean   (1001)      233 2023-05-22 10:15:50.000000 apidev_django-floppyforms-1.9.0/tests/base.py
+-rw-rw-r--   0 lucjean   (1001) lucjean   (1001)      280 2023-05-22 10:15:50.000000 apidev_django-floppyforms-1.9.0/tests/compat.py
+drwxrwxr-x   0 lucjean   (1001) lucjean   (1001)        0 2023-06-12 12:55:38.736151 apidev_django-floppyforms-1.9.0/tests/demo/
+-rw-rw-r--   0 lucjean   (1001) lucjean   (1001)        0 2023-05-22 10:15:50.000000 apidev_django-floppyforms-1.9.0/tests/demo/__init__.py
+-rw-rw-r--   0 lucjean   (1001) lucjean   (1001)     2904 2023-05-22 10:15:50.000000 apidev_django-floppyforms-1.9.0/tests/demo/forms.py
+-rw-rw-r--   0 lucjean   (1001) lucjean   (1001)      407 2023-05-22 10:15:50.000000 apidev_django-floppyforms-1.9.0/tests/demo/manage.py
+-rw-rw-r--   0 lucjean   (1001) lucjean   (1001)      616 2023-05-22 10:15:50.000000 apidev_django-floppyforms-1.9.0/tests/demo/settings.py
+drwxrwxr-x   0 lucjean   (1001) lucjean   (1001)        0 2023-06-12 12:55:38.720151 apidev_django-floppyforms-1.9.0/tests/demo/templates/
+drwxrwxr-x   0 lucjean   (1001) lucjean   (1001)        0 2023-06-12 12:55:38.736151 apidev_django-floppyforms-1.9.0/tests/demo/templates/demo/
+-rw-rw-r--   0 lucjean   (1001) lucjean   (1001)      303 2023-05-22 10:15:50.000000 apidev_django-floppyforms-1.9.0/tests/demo/templates/demo/index.html
+-rw-rw-r--   0 lucjean   (1001) lucjean   (1001)      121 2023-05-22 10:15:50.000000 apidev_django-floppyforms-1.9.0/tests/demo/urls.py
+-rw-rw-r--   0 lucjean   (1001) lucjean   (1001)      401 2023-05-22 10:15:50.000000 apidev_django-floppyforms-1.9.0/tests/demo/views.py
+-rw-rw-r--   0 lucjean   (1001) lucjean   (1001)     1717 2023-05-22 10:15:50.000000 apidev_django-floppyforms-1.9.0/tests/models.py
+-rw-rw-r--   0 lucjean   (1001) lucjean   (1001)     1107 2023-05-22 10:15:50.000000 apidev_django-floppyforms-1.9.0/tests/settings.py
+drwxrwxr-x   0 lucjean   (1001) lucjean   (1001)        0 2023-06-12 12:55:38.740151 apidev_django-floppyforms-1.9.0/tests/templates/
+-rw-rw-r--   0 lucjean   (1001) lucjean   (1001)       42 2023-05-22 10:15:50.000000 apidev_django-floppyforms-1.9.0/tests/templates/custom.html
+-rw-rw-r--   0 lucjean   (1001) lucjean   (1001)       78 2023-05-22 10:15:50.000000 apidev_django-floppyforms-1.9.0/tests/templates/extra_argument.html
+-rw-rw-r--   0 lucjean   (1001) lucjean   (1001)      161 2023-05-22 10:15:50.000000 apidev_django-floppyforms-1.9.0/tests/templates/extra_argument_with_config.html
+-rw-rw-r--   0 lucjean   (1001) lucjean   (1001)      142 2023-05-22 10:15:50.000000 apidev_django-floppyforms-1.9.0/tests/templates/formconfig_inside_only.html
+-rw-rw-r--   0 lucjean   (1001) lucjean   (1001)      109 2023-05-22 10:15:50.000000 apidev_django-floppyforms-1.9.0/tests/templates/media_widget.html
+-rw-rw-r--   0 lucjean   (1001) lucjean   (1001)      223 2023-05-22 10:15:50.000000 apidev_django-floppyforms-1.9.0/tests/templates/simple_form_tag.html
+-rw-rw-r--   0 lucjean   (1001) lucjean   (1001)       88 2023-05-22 10:15:50.000000 apidev_django-floppyforms-1.9.0/tests/templates/simple_formfield_tag.html
+-rw-rw-r--   0 lucjean   (1001) lucjean   (1001)      185 2023-05-22 10:15:50.000000 apidev_django-floppyforms-1.9.0/tests/templates/simple_formrow_tag.html
+-rw-rw-r--   0 lucjean   (1001) lucjean   (1001)      382 2023-05-22 10:15:50.000000 apidev_django-floppyforms-1.9.0/tests/templates/simple_formrow_tag_with_config.html
+-rw-rw-r--   0 lucjean   (1001) lucjean   (1001)      892 2023-05-22 10:15:50.000000 apidev_django-floppyforms-1.9.0/tests/test_deprecations.py
+-rw-rw-r--   0 lucjean   (1001) lucjean   (1001)     5842 2023-05-22 10:15:50.000000 apidev_django-floppyforms-1.9.0/tests/test_fields.py
+-rw-rw-r--   0 lucjean   (1001) lucjean   (1001)     5665 2023-05-22 10:15:50.000000 apidev_django-floppyforms-1.9.0/tests/test_forms.py
+-rw-rw-r--   0 lucjean   (1001) lucjean   (1001)    13294 2023-05-22 10:15:50.000000 apidev_django-floppyforms-1.9.0/tests/test_gis.py
+-rw-rw-r--   0 lucjean   (1001) lucjean   (1001)    28709 2023-05-22 10:15:50.000000 apidev_django-floppyforms-1.9.0/tests/test_layouts.py
+-rw-rw-r--   0 lucjean   (1001) lucjean   (1001)     8293 2023-05-22 10:15:50.000000 apidev_django-floppyforms-1.9.0/tests/test_modelforms.py
+-rw-rw-r--   0 lucjean   (1001) lucjean   (1001)     8582 2023-05-22 10:15:50.000000 apidev_django-floppyforms-1.9.0/tests/test_rendering.py
+-rw-rw-r--   0 lucjean   (1001) lucjean   (1001)    33976 2023-05-22 10:15:50.000000 apidev_django-floppyforms-1.9.0/tests/test_templatetags.py
+-rw-rw-r--   0 lucjean   (1001) lucjean   (1001)    50159 2023-05-22 10:15:50.000000 apidev_django-floppyforms-1.9.0/tests/test_widgets.py
+-rw-rw-r--   0 lucjean   (1001) lucjean   (1001)      282 2023-05-22 10:15:50.000000 apidev_django-floppyforms-1.9.0/tests/tests.py
```

### Comparing `apidev_django-floppyforms-1.8.4/CHANGES.rst` & `apidev_django-floppyforms-1.9.0/CHANGES.rst`

 * *Files identical despite different names*

### Comparing `apidev_django-floppyforms-1.8.4/README.rst` & `apidev_django-floppyforms-1.9.0/README.rst`

 * *Files identical despite different names*

### Comparing `apidev_django-floppyforms-1.8.4/apidev_django_floppyforms.egg-info/SOURCES.txt` & `apidev_django-floppyforms-1.9.0/apidev_django_floppyforms.egg-info/SOURCES.txt`

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,9 @@
 CHANGES.rst
+LICENSE
 MANIFEST.in
 README.rst
 setup.cfg
 setup.py
 apidev_django_floppyforms.egg-info/PKG-INFO
 apidev_django_floppyforms.egg-info/SOURCES.txt
 apidev_django_floppyforms.egg-info/dependency_links.txt
@@ -33,16 +34,17 @@
 docs/images/slider-jquery-ui.png
 floppyforms/__init__.py
 floppyforms/compat.py
 floppyforms/fields.py
 floppyforms/forms.py
 floppyforms/models.py
 floppyforms/widgets.py
+floppyforms/__deprecated__/__init__.py
+floppyforms/__deprecated__/models.py
 floppyforms/__future__/__init__.py
-floppyforms/__future__/models.py
 floppyforms/gis/__init__.py
 floppyforms/gis/fields.py
 floppyforms/gis/widgets.py
 floppyforms/static/floppyforms/gis/img/move_vertex_off.png
 floppyforms/static/floppyforms/gis/img/move_vertex_on.png
 floppyforms/static/floppyforms/js/MapWidget.js
 floppyforms/static/floppyforms/openlayers/OpenLayers.js
```

### Comparing `apidev_django-floppyforms-1.8.4/docs/Makefile` & `apidev_django-floppyforms-1.9.0/docs/Makefile`

 * *Files identical despite different names*

### Comparing `apidev_django-floppyforms-1.8.4/docs/bootstrap.rst` & `apidev_django-floppyforms-1.9.0/docs/bootstrap.rst`

 * *Files identical despite different names*

### Comparing `apidev_django-floppyforms-1.8.4/docs/conf.py` & `apidev_django-floppyforms-1.9.0/docs/conf.py`

 * *Files identical despite different names*

### Comparing `apidev_django-floppyforms-1.8.4/docs/customization.rst` & `apidev_django-floppyforms-1.9.0/docs/customization.rst`

 * *Files identical despite different names*

### Comparing `apidev_django-floppyforms-1.8.4/docs/differences.rst` & `apidev_django-floppyforms-1.9.0/docs/differences.rst`

 * *Files identical despite different names*

### Comparing `apidev_django-floppyforms-1.8.4/docs/examples.rst` & `apidev_django-floppyforms-1.9.0/docs/examples.rst`

 * *Files identical despite different names*

### Comparing `apidev_django-floppyforms-1.8.4/docs/geodjango.rst` & `apidev_django-floppyforms-1.9.0/docs/geodjango.rst`

 * *Files identical despite different names*

### Comparing `apidev_django-floppyforms-1.8.4/docs/images/datepicker-chromium.png` & `apidev_django-floppyforms-1.9.0/docs/images/datepicker-chromium.png`

 * *Files identical despite different names*

### Comparing `apidev_django-floppyforms-1.8.4/docs/images/datepicker-jquery-ui.png` & `apidev_django-floppyforms-1.9.0/docs/images/datepicker-jquery-ui.png`

 * *Files identical despite different names*

### Comparing `apidev_django-floppyforms-1.8.4/docs/images/geomcollection.png` & `apidev_django-floppyforms-1.9.0/docs/images/geomcollection.png`

 * *Files identical despite different names*

### Comparing `apidev_django-floppyforms-1.8.4/docs/images/gmappoly.png` & `apidev_django-floppyforms-1.9.0/docs/images/gmappoly.png`

 * *Files identical despite different names*

### Comparing `apidev_django-floppyforms-1.8.4/docs/images/image_with_thumbnail.png` & `apidev_django-floppyforms-1.9.0/docs/images/image_with_thumbnail.png`

 * *Files identical despite different names*

### Comparing `apidev_django-floppyforms-1.8.4/docs/images/osmlinestring.png` & `apidev_django-floppyforms-1.9.0/docs/images/osmlinestring.png`

 * *Files identical despite different names*

### Comparing `apidev_django-floppyforms-1.8.4/docs/images/pointfield.png` & `apidev_django-floppyforms-1.9.0/docs/images/pointfield.png`

 * *Files identical despite different names*

### Comparing `apidev_django-floppyforms-1.8.4/docs/images/slider-chromium.png` & `apidev_django-floppyforms-1.9.0/docs/images/slider-chromium.png`

 * *Files identical despite different names*

### Comparing `apidev_django-floppyforms-1.8.4/docs/images/slider-jquery-ui.png` & `apidev_django-floppyforms-1.9.0/docs/images/slider-jquery-ui.png`

 * *Files identical despite different names*

### Comparing `apidev_django-floppyforms-1.8.4/docs/index.rst` & `apidev_django-floppyforms-1.9.0/docs/index.rst`

 * *Files identical despite different names*

### Comparing `apidev_django-floppyforms-1.8.4/docs/layouts.rst` & `apidev_django-floppyforms-1.9.0/docs/layouts.rst`

 * *Files identical despite different names*

### Comparing `apidev_django-floppyforms-1.8.4/docs/templatetags.rst` & `apidev_django-floppyforms-1.9.0/docs/templatetags.rst`

 * *Files identical despite different names*

### Comparing `apidev_django-floppyforms-1.8.4/docs/usage.rst` & `apidev_django-floppyforms-1.9.0/docs/usage.rst`

 * *Files identical despite different names*

### Comparing `apidev_django-floppyforms-1.8.4/docs/widgets-reference.rst` & `apidev_django-floppyforms-1.9.0/docs/widgets-reference.rst`

 * *Files identical despite different names*

### Comparing `apidev_django-floppyforms-1.8.4/docs/widgets.rst` & `apidev_django-floppyforms-1.9.0/docs/widgets.rst`

 * *Files identical despite different names*

### Comparing `apidev_django-floppyforms-1.8.4/floppyforms/__future__/models.py` & `apidev_django-floppyforms-1.9.0/floppyforms/models.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,43 +1,41 @@
 # flake8: noqa
 import django
 from django.db import models as db_models
-from django.forms.models import (ModelForm as _ModelForm,
-                                 ModelFormMetaclass as _ModelFormMetaclass,
-                                 modelform_factory as _modelform_factory,
-                                 modelformset_factory as _modelformset_factory,
-                                 inlineformset_factory as _inlineformset_factory,
-                                 model_to_dict, fields_for_model, BaseModelForm,
-                                 BaseModelFormSet,
-                                 BaseInlineFormSet)
-if django.VERSION < (1, 9):
-    from django.forms.models import save_instance
-from django.utils import six
-
-from floppyforms import fields
-from floppyforms.forms import LayoutRenderer
-from floppyforms.models import (ModelChoiceField, ModelMultipleChoiceField)
-from floppyforms.widgets import Textarea
+from django.forms.models import (
+    ModelForm as _ModelForm,
+    ModelFormMetaclass as _ModelFormMetaclass,
+    modelform_factory as _modelform_factory,
+    modelformset_factory as _modelformset_factory,
+    inlineformset_factory as _inlineformset_factory,
+    model_to_dict, fields_for_model, BaseModelForm,
+    BaseModelFormSet, BaseInlineFormSet
+)
+import six
+
+from . import fields
+from .forms import LayoutRenderer
+from .widgets import Textarea, Select, SelectMultiple, MultipleHiddenInput
+
+
+class ModelChoiceField(fields.Field, django.forms.ModelChoiceField):
+    widget = Select
+
+
+class ModelMultipleChoiceField(fields.Field, django.forms.ModelMultipleChoiceField):
+    widget = SelectMultiple
+    hidden_widget = MultipleHiddenInput
 
 
 __all__ = (
     'ModelForm', 'BaseModelForm', 'model_to_dict', 'fields_for_model',
     'ModelChoiceField', 'ModelMultipleChoiceField',
     'BaseModelFormSet', 'modelformset_factory', 'BaseInlineFormSet',
     'inlineformset_factory',
 )
-if django.VERSION < (1, 9):
-    __all__ += ('save_instance',)
-
-
-if django.VERSION > (1, 7):
-    from django.forms.models import ALL_FIELDS
-
-    __all__ = __all__ + ('ALL_FIELDS',)
-
 
 FORMFIELD_OVERRIDES = {
     db_models.BooleanField: {'form_class': fields.BooleanField},
     db_models.CharField: {'form_class': fields.CharField},
     db_models.CommaSeparatedIntegerField: {'form_class': fields.CharField},
     db_models.DateField: {'form_class': fields.DateField},
     db_models.DateTimeField: {'form_class': fields.DateTimeField},
```

### Comparing `apidev_django-floppyforms-1.8.4/floppyforms/compat.py` & `apidev_django-floppyforms-1.9.0/floppyforms/compat.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,55 +1,37 @@
 from contextlib import contextmanager
 
-import django
 from django.template import Context
 
-try:
-    from django.utils.datastructures import MultiValueDict, MergeDict
-    MULTIVALUE_DICT_TYPES = (MultiValueDict, MergeDict)
-except ImportError:
-    # Django >= 1.9
-    from django.utils.datastructures import MultiValueDict
-    MULTIVALUE_DICT_TYPES = (MultiValueDict,)
+from django.utils.datastructures import MultiValueDict
+MULTIVALUE_DICT_TYPES = (MultiValueDict,)
 
 
 REQUIRED_CONTEXT_ATTRIBTUES = (
     '_form_config',
     '_form_render',
 )
 
 
 # We need a custom subclass of dict here in order to allow setting attributes
 # on it like _form_config and _form_render.
 class DictContext(dict):
     pass
 
 
-if django.VERSION < (1, 8):
-    def get_template(context, template_name):
-        from django.template.loader import get_template
-        return get_template(template_name)
-
-    def get_context(context):
-        # Django < 1.8 only wants ``Context`` instances as context, no dict
-        # instances.
-        if not isinstance(context, Context):
-            context = Context(context)
-        return context
-
-else:
-    def get_template(context, template_name):
-        # Django 1.8 and higher support multiple template engines. We need to
-        # load child templates used in the floppyform template tags from the
-        # same engine. Otherwise this might get really confusing.
-        return context.template.engine.get_template(template_name)
-
-    def get_context(context):
-        # Django 1.8 only wants dicts as context, no ``Context`` instances.
-        return context
+def get_template(context, template_name):
+    # Django 1.8 and higher support multiple template engines. We need to
+    # load child templates used in the floppyform template tags from the
+    # same engine. Otherwise this might get really confusing.
+    return context.template.engine.get_template(template_name)
+
+
+def get_context(context):
+    # Django 1.8 only wants dicts as context, no ``Context`` instances.
+    return context
 
 
 def flatten_context(context):
     if isinstance(context, Context):
         flat = {}
         for d in context.dicts:
             flat.update(d)
```

### Comparing `apidev_django-floppyforms-1.8.4/floppyforms/fields.py` & `apidev_django-floppyforms-1.9.0/floppyforms/fields.py`

 * *Files 2% similar despite different names*

```diff
@@ -14,16 +14,14 @@
     'DateTimeField', 'EmailField', 'FileField', 'ImageField', 'URLField',
     'BooleanField', 'NullBooleanField', 'ChoiceField', 'MultipleChoiceField',
     'FloatField', 'DecimalField', 'SlugField', 'RegexField',
     'GenericIPAddressField', 'TypedChoiceField', 'FilePathField',
     'TypedMultipleChoiceField', 'ComboField', 'MultiValueField',
     'SplitDateTimeField',
 )
-if django.VERSION < (1, 9):
-    __all__ += ('IPAddressField',)
 
 
 class Field(forms.Field):
     widget = TextInput
     hidden_widget = HiddenInput
```

### Comparing `apidev_django-floppyforms-1.8.4/floppyforms/forms.py` & `apidev_django-floppyforms-1.9.0/floppyforms/forms.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,18 +1,16 @@
 from django import forms
 from django.template.loader import get_template
-from django.utils.encoding import python_2_unicode_compatible
 
 from .compat import get_context
 
 
-__all__ = ('BaseForm', 'Form',)
+__all__ = ('BaseForm', 'Form', 'LayoutRenderer')
 
 
-@python_2_unicode_compatible
 class LayoutRenderer(object):
     _render_as_template_name = 'floppyforms/_render_as.html'
 
     def _render_as(self, layout):
         template_node = get_template(self._render_as_template_name)
         context = get_context({
             'form': self,
```

### Comparing `apidev_django-floppyforms-1.8.4/floppyforms/gis/fields.py` & `apidev_django-floppyforms-1.9.0/floppyforms/gis/fields.py`

 * *Files identical despite different names*

### Comparing `apidev_django-floppyforms-1.8.4/floppyforms/gis/widgets.py` & `apidev_django-floppyforms-1.9.0/floppyforms/gis/widgets.py`

 * *Files identical despite different names*

### Comparing `apidev_django-floppyforms-1.8.4/floppyforms/models.py` & `apidev_django-floppyforms-1.9.0/floppyforms/__deprecated__/models.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,29 +1,29 @@
 import warnings
 
 from django.forms import models
 
-from .fields import Field
-from .forms import LayoutRenderer
-from .widgets import Select, SelectMultiple, MultipleHiddenInput
+from ..fields import Field
+from ..forms import LayoutRenderer
+from ..widgets import Select, SelectMultiple, MultipleHiddenInput
 
 __all__ = ('ModelForm', 'ModelChoiceField', 'ModelMultipleChoiceField')
 
 
 class ModelForm(LayoutRenderer, models.ModelForm):
     def __new__(cls, *args, **kwargs):
         url = 'https://github.com/gregmuellegger/django-floppyforms/tree/1.2.0/CHANGES.rst'
         warnings.warn(
             'The behaviour of subclasses of floppyforms.models.ModelForm will '
             'change with django-floppyforms 2.0. '
             'Use `import floppyforms.__future__ as forms` instead of '
             '`import floppyforms as forms` to use the new behaviour now. '
             'See announcement here: %s' % url,
             FutureWarning)
-        return super(ModelForm, cls).__new__(cls, *args, **kwargs)
+        return super(ModelForm, cls).__new__(cls)
 
 
 class ModelChoiceField(Field, models.ModelChoiceField):
     widget = Select
 
 
 class ModelMultipleChoiceField(Field, models.ModelMultipleChoiceField):
```

### Comparing `apidev_django-floppyforms-1.8.4/floppyforms/static/floppyforms/gis/img/move_vertex_off.png` & `apidev_django-floppyforms-1.9.0/floppyforms/static/floppyforms/gis/img/move_vertex_off.png`

 * *Files identical despite different names*

### Comparing `apidev_django-floppyforms-1.8.4/floppyforms/static/floppyforms/js/MapWidget.js` & `apidev_django-floppyforms-1.9.0/floppyforms/static/floppyforms/js/MapWidget.js`

 * *Files identical despite different names*

### Comparing `apidev_django-floppyforms-1.8.4/floppyforms/static/floppyforms/openlayers/OpenLayers.js` & `apidev_django-floppyforms-1.9.0/floppyforms/static/floppyforms/openlayers/OpenLayers.js`

 * *Files identical despite different names*

### Comparing `apidev_django-floppyforms-1.8.4/floppyforms/static/floppyforms/openlayers/theme/default/img/add_point_off.png` & `apidev_django-floppyforms-1.9.0/floppyforms/static/floppyforms/openlayers/theme/default/img/add_point_off.png`

 * *Files identical despite different names*

### Comparing `apidev_django-floppyforms-1.8.4/floppyforms/static/floppyforms/openlayers/theme/default/img/add_point_on.png` & `apidev_django-floppyforms-1.9.0/floppyforms/static/floppyforms/openlayers/theme/default/img/add_point_on.png`

 * *Files identical despite different names*

### Comparing `apidev_django-floppyforms-1.8.4/floppyforms/static/floppyforms/openlayers/theme/default/img/close.gif` & `apidev_django-floppyforms-1.9.0/floppyforms/static/floppyforms/openlayers/theme/default/img/close.gif`

 * *Files identical despite different names*

### Comparing `apidev_django-floppyforms-1.8.4/floppyforms/static/floppyforms/openlayers/theme/default/img/drag-rectangle-off.png` & `apidev_django-floppyforms-1.9.0/floppyforms/static/floppyforms/openlayers/theme/default/img/drag-rectangle-off.png`

 * *Files identical despite different names*

### Comparing `apidev_django-floppyforms-1.8.4/floppyforms/static/floppyforms/openlayers/theme/default/img/drag-rectangle-on.png` & `apidev_django-floppyforms-1.9.0/floppyforms/static/floppyforms/openlayers/theme/default/img/drag-rectangle-on.png`

 * *Files identical despite different names*

### Comparing `apidev_django-floppyforms-1.8.4/floppyforms/static/floppyforms/openlayers/theme/default/img/draw_line_off.png` & `apidev_django-floppyforms-1.9.0/floppyforms/static/floppyforms/openlayers/theme/default/img/draw_line_off.png`

 * *Files identical despite different names*

### Comparing `apidev_django-floppyforms-1.8.4/floppyforms/static/floppyforms/openlayers/theme/default/img/draw_line_on.png` & `apidev_django-floppyforms-1.9.0/floppyforms/static/floppyforms/openlayers/theme/default/img/draw_line_on.png`

 * *Files identical despite different names*

### Comparing `apidev_django-floppyforms-1.8.4/floppyforms/static/floppyforms/openlayers/theme/default/img/draw_point_off.png` & `apidev_django-floppyforms-1.9.0/floppyforms/static/floppyforms/openlayers/theme/default/img/draw_point_off.png`

 * *Files identical despite different names*

### Comparing `apidev_django-floppyforms-1.8.4/floppyforms/static/floppyforms/openlayers/theme/default/img/draw_point_on.png` & `apidev_django-floppyforms-1.9.0/floppyforms/static/floppyforms/openlayers/theme/default/img/draw_point_on.png`

 * *Files identical despite different names*

### Comparing `apidev_django-floppyforms-1.8.4/floppyforms/static/floppyforms/openlayers/theme/default/img/draw_polygon_off.png` & `apidev_django-floppyforms-1.9.0/floppyforms/static/floppyforms/openlayers/theme/default/img/draw_polygon_off.png`

 * *Files identical despite different names*

### Comparing `apidev_django-floppyforms-1.8.4/floppyforms/static/floppyforms/openlayers/theme/default/img/draw_polygon_on.png` & `apidev_django-floppyforms-1.9.0/floppyforms/static/floppyforms/openlayers/theme/default/img/draw_polygon_on.png`

 * *Files identical despite different names*

### Comparing `apidev_django-floppyforms-1.8.4/floppyforms/static/floppyforms/openlayers/theme/default/img/editing_tool_bar.png` & `apidev_django-floppyforms-1.9.0/floppyforms/static/floppyforms/openlayers/theme/default/img/editing_tool_bar.png`

 * *Files identical despite different names*

### Comparing `apidev_django-floppyforms-1.8.4/floppyforms/static/floppyforms/openlayers/theme/default/img/move_feature_off.png` & `apidev_django-floppyforms-1.9.0/floppyforms/static/floppyforms/openlayers/theme/default/img/move_feature_off.png`

 * *Files identical despite different names*

### Comparing `apidev_django-floppyforms-1.8.4/floppyforms/static/floppyforms/openlayers/theme/default/img/move_feature_on.png` & `apidev_django-floppyforms-1.9.0/floppyforms/static/floppyforms/openlayers/theme/default/img/move_feature_on.png`

 * *Files identical despite different names*

### Comparing `apidev_django-floppyforms-1.8.4/floppyforms/static/floppyforms/openlayers/theme/default/img/navigation_history.png` & `apidev_django-floppyforms-1.9.0/floppyforms/static/floppyforms/openlayers/theme/default/img/navigation_history.png`

 * *Files identical despite different names*

### Comparing `apidev_django-floppyforms-1.8.4/floppyforms/static/floppyforms/openlayers/theme/default/img/pan-panel-NOALPHA.png` & `apidev_django-floppyforms-1.9.0/floppyforms/static/floppyforms/openlayers/theme/default/img/pan-panel-NOALPHA.png`

 * *Files identical despite different names*

### Comparing `apidev_django-floppyforms-1.8.4/floppyforms/static/floppyforms/openlayers/theme/default/img/pan-panel.png` & `apidev_django-floppyforms-1.9.0/floppyforms/static/floppyforms/openlayers/theme/default/img/pan-panel.png`

 * *Files identical despite different names*

### Comparing `apidev_django-floppyforms-1.8.4/floppyforms/static/floppyforms/openlayers/theme/default/img/pan_off.png` & `apidev_django-floppyforms-1.9.0/floppyforms/static/floppyforms/openlayers/theme/default/img/pan_off.png`

 * *Files identical despite different names*

### Comparing `apidev_django-floppyforms-1.8.4/floppyforms/static/floppyforms/openlayers/theme/default/img/pan_on.png` & `apidev_django-floppyforms-1.9.0/floppyforms/static/floppyforms/openlayers/theme/default/img/pan_on.png`

 * *Files identical despite different names*

### Comparing `apidev_django-floppyforms-1.8.4/floppyforms/static/floppyforms/openlayers/theme/default/img/panning-hand-off.png` & `apidev_django-floppyforms-1.9.0/floppyforms/static/floppyforms/openlayers/theme/default/img/panning-hand-off.png`

 * *Files identical despite different names*

### Comparing `apidev_django-floppyforms-1.8.4/floppyforms/static/floppyforms/openlayers/theme/default/img/panning-hand-on.png` & `apidev_django-floppyforms-1.9.0/floppyforms/static/floppyforms/openlayers/theme/default/img/panning-hand-on.png`

 * *Files identical despite different names*

### Comparing `apidev_django-floppyforms-1.8.4/floppyforms/static/floppyforms/openlayers/theme/default/img/remove_point_off.png` & `apidev_django-floppyforms-1.9.0/floppyforms/static/floppyforms/openlayers/theme/default/img/remove_point_off.png`

 * *Files identical despite different names*

### Comparing `apidev_django-floppyforms-1.8.4/floppyforms/static/floppyforms/openlayers/theme/default/img/remove_point_on.png` & `apidev_django-floppyforms-1.9.0/floppyforms/static/floppyforms/openlayers/theme/default/img/remove_point_on.png`

 * *Files identical despite different names*

### Comparing `apidev_django-floppyforms-1.8.4/floppyforms/static/floppyforms/openlayers/theme/default/img/ruler.png` & `apidev_django-floppyforms-1.9.0/floppyforms/static/floppyforms/openlayers/theme/default/img/ruler.png`

 * *Files identical despite different names*

### Comparing `apidev_django-floppyforms-1.8.4/floppyforms/static/floppyforms/openlayers/theme/default/img/view_next_off.png` & `apidev_django-floppyforms-1.9.0/floppyforms/static/floppyforms/openlayers/theme/default/img/view_next_off.png`

 * *Files identical despite different names*

### Comparing `apidev_django-floppyforms-1.8.4/floppyforms/static/floppyforms/openlayers/theme/default/img/view_next_on.png` & `apidev_django-floppyforms-1.9.0/floppyforms/static/floppyforms/openlayers/theme/default/img/view_next_on.png`

 * *Files identical despite different names*

### Comparing `apidev_django-floppyforms-1.8.4/floppyforms/static/floppyforms/openlayers/theme/default/img/view_previous_off.png` & `apidev_django-floppyforms-1.9.0/floppyforms/static/floppyforms/openlayers/theme/default/img/view_previous_off.png`

 * *Files identical despite different names*

### Comparing `apidev_django-floppyforms-1.8.4/floppyforms/static/floppyforms/openlayers/theme/default/img/view_previous_on.png` & `apidev_django-floppyforms-1.9.0/floppyforms/static/floppyforms/openlayers/theme/default/img/view_previous_on.png`

 * *Files identical despite different names*

### Comparing `apidev_django-floppyforms-1.8.4/floppyforms/static/floppyforms/openlayers/theme/default/img/zoom-panel-NOALPHA.png` & `apidev_django-floppyforms-1.9.0/floppyforms/static/floppyforms/openlayers/theme/default/img/zoom-panel-NOALPHA.png`

 * *Files identical despite different names*

### Comparing `apidev_django-floppyforms-1.8.4/floppyforms/static/floppyforms/openlayers/theme/default/img/zoom-panel.png` & `apidev_django-floppyforms-1.9.0/floppyforms/static/floppyforms/openlayers/theme/default/img/zoom-panel.png`

 * *Files identical despite different names*

### Comparing `apidev_django-floppyforms-1.8.4/floppyforms/static/floppyforms/openlayers/theme/default/style.css` & `apidev_django-floppyforms-1.9.0/floppyforms/static/floppyforms/openlayers/theme/default/style.css`

 * *Files identical despite different names*

### Comparing `apidev_django-floppyforms-1.8.4/floppyforms/static/floppyforms/openlayers/theme/default/style.mobile.css` & `apidev_django-floppyforms-1.9.0/floppyforms/static/floppyforms/openlayers/theme/default/style.mobile.css`

 * *Files identical despite different names*

### Comparing `apidev_django-floppyforms-1.8.4/floppyforms/templates/floppyforms/gis/openlayers.html` & `apidev_django-floppyforms-1.9.0/floppyforms/templates/floppyforms/gis/openlayers.html`

 * *Files identical despite different names*

### Comparing `apidev_django-floppyforms-1.8.4/floppyforms/templates/floppyforms/layouts/p.html` & `apidev_django-floppyforms-1.9.0/floppyforms/templates/floppyforms/layouts/p.html`

 * *Files identical despite different names*

### Comparing `apidev_django-floppyforms-1.8.4/floppyforms/templates/floppyforms/layouts/table.html` & `apidev_django-floppyforms-1.9.0/floppyforms/templates/floppyforms/layouts/table.html`

 * *Files identical despite different names*

### Comparing `apidev_django-floppyforms-1.8.4/floppyforms/templates/floppyforms/layouts/ul.html` & `apidev_django-floppyforms-1.9.0/floppyforms/templates/floppyforms/layouts/ul.html`

 * *Files identical despite different names*

### Comparing `apidev_django-floppyforms-1.8.4/floppyforms/templates/floppyforms/rows/li.html` & `apidev_django-floppyforms-1.9.0/floppyforms/templates/floppyforms/rows/li.html`

 * *Files identical despite different names*

### Comparing `apidev_django-floppyforms-1.8.4/floppyforms/templates/floppyforms/rows/p.html` & `apidev_django-floppyforms-1.9.0/floppyforms/templates/floppyforms/rows/p.html`

 * *Files identical despite different names*

### Comparing `apidev_django-floppyforms-1.8.4/floppyforms/templates/floppyforms/rows/tr.html` & `apidev_django-floppyforms-1.9.0/floppyforms/templates/floppyforms/rows/tr.html`

 * *Files identical despite different names*

### Comparing `apidev_django-floppyforms-1.8.4/floppyforms/templates/floppyforms/select.html` & `apidev_django-floppyforms-1.9.0/floppyforms/templates/floppyforms/select.html`

 * *Files identical despite different names*

### Comparing `apidev_django-floppyforms-1.8.4/floppyforms/templates/floppyforms/select_date.html` & `apidev_django-floppyforms-1.9.0/floppyforms/templates/floppyforms/select_date.html`

 * *Files identical despite different names*

### Comparing `apidev_django-floppyforms-1.8.4/floppyforms/templatetags/floppyforms.py` & `apidev_django-floppyforms-1.9.0/floppyforms/templatetags/floppyforms.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,21 +1,17 @@
 import django
 from collections import defaultdict
 from contextlib import contextmanager
 
 from django.conf import settings
 
-try:
-    from django.forms.utils import ErrorList
-except ImportError:
-    # Fall back to old module name for Django <= 1.5
-    from django.forms.util import ErrorList
-from django.template import (Library, Node, Variable,
-                             TemplateSyntaxError, VariableDoesNotExist)
-from django.template.base import token_kwargs
+from django.forms.utils import ErrorList
+from django.template.base import Node, Variable, VariableDoesNotExist, token_kwargs
+from django.template.exceptions import TemplateSyntaxError
+from django.template.library import Library
 from django.utils.functional import empty
 
 from ..compat import get_template
 
 
 register = Library()
```

### Comparing `apidev_django-floppyforms-1.8.4/floppyforms/templatetags/floppyforms_internals.py` & `apidev_django-floppyforms-1.9.0/floppyforms/templatetags/floppyforms_internals.py`

 * *Files identical despite different names*

### Comparing `apidev_django-floppyforms-1.8.4/floppyforms/widgets.py` & `apidev_django-floppyforms-1.9.0/floppyforms/widgets.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,26 +1,23 @@
 from itertools import chain
 import re
 import datetime
+import six
 
 import django
 from django import forms
-try:
-    from django.forms.utils import to_current_timezone
-except ImportError:
-    # Fall back to old module name for Django <= 1.5
-    from django.forms.util import to_current_timezone
+from django.forms.utils import to_current_timezone
 from django.forms.widgets import FILE_INPUT_CONTRADICTION
 from django.conf import settings
 from django.template import loader
 from django.utils.html import conditional_escape
-from django.utils.translation import ugettext_lazy as _
-from django.utils import datetime_safe, formats, six
+from django.utils.translation import gettext_lazy as _
+from django.utils import datetime_safe, formats
 from django.utils.dates import MONTHS
-from django.utils.encoding import force_text
+from django.utils.encoding import force_str
 from django.utils.safestring import mark_safe
 
 from .compat import MULTIVALUE_DICT_TYPES, flatten_contexts
 
 
 RE_DATE = re.compile(r'(\d{4})-(\d\d?)-(\d\d?)$')
 
@@ -70,15 +67,15 @@
 
     def get_context_data(self):
         return {}
 
     def _format_value(self, value):
         if self.is_localized:
             value = formats.localize_input(value)
-        return force_text(value)
+        return force_str(value)
 
     def get_context(self, name, value, attrs=None):
         context = {
             'type': self.input_type,
             'name': name,
             'hidden': self.is_hidden,
             'required': self.is_required,
@@ -167,15 +164,15 @@
         inputs = []
         for i, v in enumerate(value):
             input_attrs = final_attrs.copy()
             if id_:
                 input_attrs['id'] = '%s_%s' % (id_, i)
             input_ = HiddenInput()
             input_.is_required = self.is_required
-            inputs.append(input_.render(name, force_text(v), input_attrs))
+            inputs.append(input_.render(name, force_str(v), input_attrs))
         return mark_safe("\n".join(inputs))
 
     def value_from_datadict(self, data, files, name):
         if isinstance(data, MULTIVALUE_DICT_TYPES):
             return data.getlist(name)
         return data.get(name, None)
 
@@ -283,15 +280,15 @@
     def __init__(self, attrs=None):
         default_attrs = {'cols': self.cols, 'rows': self.rows}
         if attrs:
             default_attrs.update(attrs)
         super(Textarea, self).__init__(default_attrs)
 
     def _format_value(self, value):
-        return conditional_escape(force_text(value))
+        return conditional_escape(force_str(value))
 
 
 class DateInput(Input):
     template_name = 'floppyforms/date.html'
     input_type = 'date'
     supports_microseconds = False
 
@@ -450,15 +447,15 @@
             context['attrs']['checked'] = True
         return context
 
     def _format_value(self, value):
         if value in ('', True, False, None):
             value = None
         else:
-            value = force_text(value)
+            value = force_str(value)
         return value
 
     def value_from_datadict(self, data, files, name):
         return forms.CheckboxInput.value_from_datadict(self, data, files, name)
 
     if django.VERSION < (1, 6):
         def _has_changed(self, initial, data):
@@ -497,29 +494,29 @@
         #   ]),
         # )
         groups = []
         for option_value, option_label in chain(self.choices, choices):
             if isinstance(option_label, (list, tuple)):
                 group = []
                 for val, lab in option_label:
-                    group.append((force_text(val), lab))
+                    group.append((force_str(val), lab))
                 groups.append((option_value, group))
             else:
-                option_value = force_text(option_value)
+                option_value = force_str(option_value)
                 if groups and groups[-1][0] is None:
                     groups[-1][1].append((option_value, option_label))
                 else:
                     groups.append((None, [(option_value, option_label)]))
         context["optgroups"] = groups
         return context
 
     def _format_value(self, value):
         if len(value) == 1 and value[0] is None:
             return []
-        return set(force_text(v) for v in value)
+        return set(force_str(v) for v in value)
 
 
 class NullBooleanSelect(Select):
     def __init__(self, attrs=None):
         choices = (('1', _('Unknown')),
                    ('2', _('Yes')),
                    ('3', _('No')))
@@ -553,31 +550,31 @@
 
 class SelectMultiple(Select):
     allow_multiple_selected = True
 
     def _format_value(self, value):
         if len(value) == 1 and value[0] is None:
             value = []
-        return [force_text(v) for v in value]
+        return [force_str(v) for v in value]
 
     def value_from_datadict(self, data, files, name):
         if isinstance(data, MULTIVALUE_DICT_TYPES):
             return data.getlist(name)
         return data.get(name, None)
 
     if django.VERSION < (1, 6):
         def _has_changed(self, initial, data):
             if initial is None:
                 initial = []
             if data is None:
                 data = []
             if len(initial) != len(data):
                 return True
-            initial_set = set([force_text(value) for value in initial])
-            data_set = set([force_text(value) for value in data])
+            initial_set = set([force_str(value) for value in initial])
+            data_set = set([force_str(value) for value in data])
             return data_set != initial_set
 
 
 class RadioSelect(Select):
     template_name = 'floppyforms/radio.html'
```

### Comparing `apidev_django-floppyforms-1.8.4/setup.py` & `apidev_django-floppyforms-1.9.0/setup.py`

 * *Files identical despite different names*

### Comparing `apidev_django-floppyforms-1.8.4/tests/demo/forms.py` & `apidev_django-floppyforms-1.9.0/tests/demo/forms.py`

 * *Files identical despite different names*

### Comparing `apidev_django-floppyforms-1.8.4/tests/demo/settings.py` & `apidev_django-floppyforms-1.9.0/tests/demo/settings.py`

 * *Files identical despite different names*

### Comparing `apidev_django-floppyforms-1.8.4/tests/models.py` & `apidev_django-floppyforms-1.9.0/tests/models.py`

 * *Files identical despite different names*

### Comparing `apidev_django-floppyforms-1.8.4/tests/settings.py` & `apidev_django-floppyforms-1.9.0/tests/settings.py`

 * *Files identical despite different names*

### Comparing `apidev_django-floppyforms-1.8.4/tests/test_deprecations.py` & `apidev_django-floppyforms-1.9.0/tests/test_deprecations.py`

 * *Files identical despite different names*

### Comparing `apidev_django-floppyforms-1.8.4/tests/test_fields.py` & `apidev_django-floppyforms-1.9.0/tests/test_fields.py`

 * *Files identical despite different names*

### Comparing `apidev_django-floppyforms-1.8.4/tests/test_forms.py` & `apidev_django-floppyforms-1.9.0/tests/test_forms.py`

 * *Files identical despite different names*

### Comparing `apidev_django-floppyforms-1.8.4/tests/test_gis.py` & `apidev_django-floppyforms-1.9.0/tests/test_gis.py`

 * *Files identical despite different names*

### Comparing `apidev_django-floppyforms-1.8.4/tests/test_layouts.py` & `apidev_django-floppyforms-1.9.0/tests/test_layouts.py`

 * *Files identical despite different names*

### Comparing `apidev_django-floppyforms-1.8.4/tests/test_modelforms.py` & `apidev_django-floppyforms-1.9.0/tests/test_modelforms.py`

 * *Files identical despite different names*

### Comparing `apidev_django-floppyforms-1.8.4/tests/test_rendering.py` & `apidev_django-floppyforms-1.9.0/tests/test_rendering.py`

 * *Files identical despite different names*

### Comparing `apidev_django-floppyforms-1.8.4/tests/test_templatetags.py` & `apidev_django-floppyforms-1.9.0/tests/test_templatetags.py`

 * *Files identical despite different names*

### Comparing `apidev_django-floppyforms-1.8.4/tests/test_widgets.py` & `apidev_django-floppyforms-1.9.0/tests/test_widgets.py`

 * *Files identical despite different names*

