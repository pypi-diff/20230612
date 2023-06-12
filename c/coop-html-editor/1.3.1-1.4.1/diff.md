# Comparing `tmp/coop_html_editor-1.3.1.tar.gz` & `tmp/coop_html_editor-1.4.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/coop_html_editor-1.3.1.tar", last modified: Fri Aug 30 10:40:05 2019, max compression
+gzip compressed data, was "coop_html_editor-1.4.1.tar", last modified: Mon Jun 12 12:55:08 2023, max compression
```

## Comparing `coop_html_editor-1.3.1.tar` & `coop_html_editor-1.4.1.tar`

### file list

```diff
@@ -1,2620 +1,802 @@
-drwxr-xr-x   0 lucjean    (501) staff       (20)        0 2019-08-30 10:40:05.000000 coop_html_editor-1.3.1/
--rw-r--r--   0 lucjean    (501) staff       (20)     6379 2019-08-30 10:40:05.000000 coop_html_editor-1.3.1/PKG-INFO
-drwxr-xr-x   0 lucjean    (501) staff       (20)        0 2019-08-30 10:39:36.000000 coop_html_editor-1.3.1/coop_html_editor.egg-info/
--rw-r--r--   0 lucjean    (501) staff       (20)     6379 2019-08-30 10:39:34.000000 coop_html_editor-1.3.1/coop_html_editor.egg-info/PKG-INFO
--rw-r--r--   0 lucjean    (501) staff       (20)   159926 2019-08-29 14:49:30.000000 coop_html_editor-1.3.1/coop_html_editor.egg-info/SOURCES.txt.py
--rw-r--r--   0 lucjean    (501) staff       (20)        1 2019-08-29 13:12:49.000000 coop_html_editor-1.3.1/coop_html_editor.egg-info/not-zip-safe
--rw-r--r--   0 lucjean    (501) staff       (20)        1 2019-08-29 14:49:30.000000 coop_html_editor-1.3.1/coop_html_editor.egg-info/dependency_links.txt.py
--rw-r--r--   0 lucjean    (501) staff       (20)   160102 2019-08-30 10:39:34.000000 coop_html_editor-1.3.1/coop_html_editor.egg-info/SOURCES.txt
--rw-r--r--   0 lucjean    (501) staff       (20)       26 2019-08-30 10:39:34.000000 coop_html_editor-1.3.1/coop_html_editor.egg-info/requires.txt
--rw-r--r--   0 lucjean    (501) staff       (20)       17 2019-08-29 14:49:30.000000 coop_html_editor-1.3.1/coop_html_editor.egg-info/top_level.txt.py
--rw-r--r--   0 lucjean    (501) staff       (20)       26 2019-08-29 14:49:30.000000 coop_html_editor-1.3.1/coop_html_editor.egg-info/requires.txt.py
--rw-r--r--   0 lucjean    (501) staff       (20)       17 2019-08-30 10:39:34.000000 coop_html_editor-1.3.1/coop_html_editor.egg-info/top_level.txt
--rw-r--r--   0 lucjean    (501) staff       (20)        1 2019-08-30 10:39:34.000000 coop_html_editor-1.3.1/coop_html_editor.egg-info/dependency_links.txt
-drwxr-xr-x   0 lucjean    (501) staff       (20)        0 2019-08-30 10:39:36.000000 coop_html_editor-1.3.1/coop_html_editor/
-drwxr-xr-x   0 lucjean    (501) staff       (20)        0 2019-08-30 10:40:05.000000 coop_html_editor-1.3.1/coop_html_editor/templatetags/
--rw-r--r--   0 lucjean    (501) staff       (20)       23 2019-08-29 13:07:46.000000 coop_html_editor-1.3.1/coop_html_editor/templatetags/__init__.py
--rw-r--r--   0 lucjean    (501) staff       (20)     5574 2019-08-29 13:07:46.000000 coop_html_editor-1.3.1/coop_html_editor/templatetags/html_editor_utils.py
-drwxr-xr-x   0 lucjean    (501) staff       (20)        0 2019-08-30 10:39:35.000000 coop_html_editor-1.3.1/coop_html_editor/locale/
-drwxr-xr-x   0 lucjean    (501) staff       (20)        0 2019-08-30 10:39:35.000000 coop_html_editor-1.3.1/coop_html_editor/locale/fr/
-drwxr-xr-x   0 lucjean    (501) staff       (20)        0 2019-08-30 10:39:36.000000 coop_html_editor-1.3.1/coop_html_editor/locale/fr/LC_MESSAGES/
--rw-r--r--   0 lucjean    (501) staff       (20)      673 2019-08-29 13:07:37.000000 coop_html_editor-1.3.1/coop_html_editor/locale/fr/LC_MESSAGES/django.mo
--rw-r--r--   0 lucjean    (501) staff       (20)     1531 2019-08-29 13:07:37.000000 coop_html_editor-1.3.1/coop_html_editor/locale/fr/LC_MESSAGES/django.po
--rw-r--r--   0 lucjean    (501) staff       (20)      340 2019-08-30 10:27:55.000000 coop_html_editor-1.3.1/coop_html_editor/__init__.py
--rw-r--r--   0 lucjean    (501) staff       (20)      189 2019-08-29 13:07:37.000000 coop_html_editor-1.3.1/coop_html_editor/apps.py
--rw-r--r--   0 lucjean    (501) staff       (20)     5279 2019-08-29 13:07:46.000000 coop_html_editor-1.3.1/coop_html_editor/widgets.py
--rw-r--r--   0 lucjean    (501) staff       (20)     1823 2019-08-29 13:07:37.000000 coop_html_editor-1.3.1/coop_html_editor/forms.py
--rw-r--r--   0 lucjean    (501) staff       (20)     1202 2019-08-29 13:07:46.000000 coop_html_editor-1.3.1/coop_html_editor/utils.py
-drwxr-xr-x   0 lucjean    (501) staff       (20)        0 2019-08-30 10:39:35.000000 coop_html_editor-1.3.1/coop_html_editor/static/
-drwxr-xr-x   0 lucjean    (501) staff       (20)        0 2019-08-30 10:39:54.000000 coop_html_editor-1.3.1/coop_html_editor/static/ckeditor.4.6.2/
--rw-r--r--   0 lucjean    (501) staff       (20)    76251 2019-08-29 13:07:41.000000 coop_html_editor-1.3.1/coop_html_editor/static/ckeditor.4.6.2/LICENSE.md
-drwxr-xr-x   0 lucjean    (501) staff       (20)        0 2019-08-30 10:39:54.000000 coop_html_editor-1.3.1/coop_html_editor/static/ckeditor.4.6.2/plugins/
-drwxr-xr-x   0 lucjean    (501) staff       (20)        0 2019-08-30 10:40:03.000000 coop_html_editor-1.3.1/coop_html_editor/static/ckeditor.4.6.2/plugins/wsc/
--rw-r--r--   0 lucjean    (501) staff       (20)     1474 2019-08-29 13:07:45.000000 coop_html_editor-1.3.1/coop_html_editor/static/ckeditor.4.6.2/plugins/wsc/LICENSE.md
-drwxr-xr-x   0 lucjean    (501) staff       (20)        0 2019-08-30 10:39:35.000000 coop_html_editor-1.3.1/coop_html_editor/static/ckeditor.4.6.2/plugins/wsc/skins/
-drwxr-xr-x   0 lucjean    (501) staff       (20)        0 2019-08-30 10:40:03.000000 coop_html_editor-1.3.1/coop_html_editor/static/ckeditor.4.6.2/plugins/wsc/skins/moono-lisa/
--rw-r--r--   0 lucjean    (501) staff       (20)     1306 2019-08-29 13:07:45.000000 coop_html_editor-1.3.1/coop_html_editor/static/ckeditor.4.6.2/plugins/wsc/skins/moono-lisa/wsc.css
--rw-r--r--   0 lucjean    (501) staff       (20)      970 2019-08-29 13:07:45.000000 coop_html_editor-1.3.1/coop_html_editor/static/ckeditor.4.6.2/plugins/wsc/README.md
-drwxr-xr-x   0 lucjean    (501) staff       (20)        0 2019-08-30 10:40:03.000000 coop_html_editor-1.3.1/coop_html_editor/static/ckeditor.4.6.2/plugins/wsc/dialogs/
--rw-r--r--   0 lucjean    (501) staff       (20)     1232 2019-08-29 13:07:45.000000 coop_html_editor-1.3.1/coop_html_editor/static/ckeditor.4.6.2/plugins/wsc/dialogs/wsc.css
--rw-r--r--   0 lucjean    (501) staff       (20)     1935 2019-08-29 13:07:45.000000 coop_html_editor-1.3.1/coop_html_editor/static/ckeditor.4.6.2/plugins/wsc/dialogs/tmpFrameset.html
--rw-r--r--   0 lucjean    (501) staff       (20)     1690 2019-08-29 13:07:45.000000 coop_html_editor-1.3.1/coop_html_editor/static/ckeditor.4.6.2/plugins/wsc/dialogs/ciframe.html
--rw-r--r--   0 lucjean    (501) staff       (20)    48295 2019-08-29 13:07:45.000000 coop_html_editor-1.3.1/coop_html_editor/static/ckeditor.4.6.2/plugins/wsc/dialogs/wsc.js
--rw-r--r--   0 lucjean    (501) staff       (20)     3438 2019-08-29 13:07:45.000000 coop_html_editor-1.3.1/coop_html_editor/static/ckeditor.4.6.2/plugins/wsc/dialogs/wsc_ie.js
-drwxr-xr-x   0 lucjean    (501) staff       (20)        0 2019-08-30 10:39:35.000000 coop_html_editor-1.3.1/coop_html_editor/static/ckeditor.4.6.2/plugins/magicline/
-drwxr-xr-x   0 lucjean    (501) staff       (20)        0 2019-08-30 10:39:59.000000 coop_html_editor-1.3.1/coop_html_editor/static/ckeditor.4.6.2/plugins/magicline/images/
--rw-r--r--   0 lucjean    (501) staff       (20)      138 2019-08-29 13:07:42.000000 coop_html_editor-1.3.1/coop_html_editor/static/ckeditor.4.6.2/plugins/magicline/images/icon-rtl.png
--rw-r--r--   0 lucjean    (501) staff       (20)      133 2019-08-29 13:07:42.000000 coop_html_editor-1.3.1/coop_html_editor/static/ckeditor.4.6.2/plugins/magicline/images/icon.png
-drwxr-xr-x   0 lucjean    (501) staff       (20)        0 2019-08-30 10:39:59.000000 coop_html_editor-1.3.1/coop_html_editor/static/ckeditor.4.6.2/plugins/magicline/images/hidpi/
--rw-r--r--   0 lucjean    (501) staff       (20)      176 2019-08-29 13:07:42.000000 coop_html_editor-1.3.1/coop_html_editor/static/ckeditor.4.6.2/plugins/magicline/images/hidpi/icon-rtl.png
--rw-r--r--   0 lucjean    (501) staff       (20)      199 2019-08-29 13:07:42.000000 coop_html_editor-1.3.1/coop_html_editor/static/ckeditor.4.6.2/plugins/magicline/images/hidpi/icon.png
-drwxr-xr-x   0 lucjean    (501) staff       (20)        0 2019-08-30 10:40:02.000000 coop_html_editor-1.3.1/coop_html_editor/static/ckeditor.4.6.2/plugins/widget/
-drwxr-xr-x   0 lucjean    (501) staff       (20)        0 2019-08-30 10:40:02.000000 coop_html_editor-1.3.1/coop_html_editor/static/ckeditor.4.6.2/plugins/widget/images/
--rw-r--r--   0 lucjean    (501) staff       (20)      220 2019-08-29 13:07:43.000000 coop_html_editor-1.3.1/coop_html_editor/static/ckeditor.4.6.2/plugins/widget/images/handle.png
-drwxr-xr-x   0 lucjean    (501) staff       (20)        0 2019-08-30 10:40:03.000000 coop_html_editor-1.3.1/coop_html_editor/static/ckeditor.4.6.2/plugins/widget/lang/
--rw-r--r--   0 lucjean    (501) staff       (20)      282 2019-08-29 13:07:45.000000 coop_html_editor-1.3.1/coop_html_editor/static/ckeditor.4.6.2/plugins/widget/lang/pt.js
--rw-r--r--   0 lucjean    (501) staff       (20)      296 2019-08-29 13:07:45.000000 coop_html_editor-1.3.1/coop_html_editor/static/ckeditor.4.6.2/plugins/widget/lang/vi.js
--rw-r--r--   0 lucjean    (501) staff       (20)      291 2019-08-29 13:07:44.000000 coop_html_editor-1.3.1/coop_html_editor/static/ckeditor.4.6.2/plugins/widget/lang/lv.js
--rw-r--r--   0 lucjean    (501) staff       (20)      282 2019-08-29 13:07:43.000000 coop_html_editor-1.3.1/coop_html_editor/static/ckeditor.4.6.2/plugins/widget/lang/gl.js
--rw-r--r--   0 lucjean    (501) staff       (20)      283 2019-08-29 13:07:44.000000 coop_html_editor-1.3.1/coop_html_editor/static/ckeditor.4.6.2/plugins/widget/lang/pl.js
--rw-r--r--   0 lucjean    (501) staff       (20)      351 2019-08-29 13:07:43.000000 coop_html_editor-1.3.1/coop_html_editor/static/ckeditor.4.6.2/plugins/widget/lang/el.js
--rw-r--r--   0 lucjean    (501) staff       (20)      291 2019-08-29 13:07:45.000000 coop_html_editor-1.3.1/coop_html_editor/static/ckeditor.4.6.2/plugins/widget/lang/sl.js
--rw-r--r--   0 lucjean    (501) staff       (20)      301 2019-08-29 13:07:44.000000 coop_html_editor-1.3.1/coop_html_editor/static/ckeditor.4.6.2/plugins/widget/lang/ko.js
--rw-r--r--   0 lucjean    (501) staff       (20)      283 2019-08-29 13:07:44.000000 coop_html_editor-1.3.1/coop_html_editor/static/ckeditor.4.6.2/plugins/widget/lang/hr.js
--rw-r--r--   0 lucjean    (501) staff       (20)      290 2019-08-29 13:07:43.000000 coop_html_editor-1.3.1/coop_html_editor/static/ckeditor.4.6.2/plugins/widget/lang/fi.js
--rw-r--r--   0 lucjean    (501) staff       (20)      323 2019-08-29 13:07:45.000000 coop_html_editor-1.3.1/coop_html_editor/static/ckeditor.4.6.2/plugins/widget/lang/ru.js
--rw-r--r--   0 lucjean    (501) staff       (20)      281 2019-08-29 13:07:43.000000 coop_html_editor-1.3.1/coop_html_editor/static/ckeditor.4.6.2/plugins/widget/lang/eu.js
--rw-r--r--   0 lucjean    (501) staff       (20)      270 2019-08-29 13:07:44.000000 coop_html_editor-1.3.1/coop_html_editor/static/ckeditor.4.6.2/plugins/widget/lang/no.js
--rw-r--r--   0 lucjean    (501) staff       (20)      290 2019-08-29 13:07:45.000000 coop_html_editor-1.3.1/coop_html_editor/static/ckeditor.4.6.2/plugins/widget/lang/sq.js
--rw-r--r--   0 lucjean    (501) staff       (20)      317 2019-08-29 13:07:45.000000 coop_html_editor-1.3.1/coop_html_editor/static/ckeditor.4.6.2/plugins/widget/lang/tt.js
--rw-r--r--   0 lucjean    (501) staff       (20)      280 2019-08-29 13:07:44.000000 coop_html_editor-1.3.1/coop_html_editor/static/ckeditor.4.6.2/plugins/widget/lang/ja.js
--rw-r--r--   0 lucjean    (501) staff       (20)      283 2019-08-29 13:07:44.000000 coop_html_editor-1.3.1/coop_html_editor/static/ckeditor.4.6.2/plugins/widget/lang/he.js
--rw-r--r--   0 lucjean    (501) staff       (20)      293 2019-08-29 13:07:45.000000 coop_html_editor-1.3.1/coop_html_editor/static/ckeditor.4.6.2/plugins/widget/lang/ug.js
--rw-r--r--   0 lucjean    (501) staff       (20)      311 2019-08-29 13:07:43.000000 coop_html_editor-1.3.1/coop_html_editor/static/ckeditor.4.6.2/plugins/widget/lang/bg.js
--rw-r--r--   0 lucjean    (501) staff       (20)      280 2019-08-29 13:07:43.000000 coop_html_editor-1.3.1/coop_html_editor/static/ckeditor.4.6.2/plugins/widget/lang/af.js
--rw-r--r--   0 lucjean    (501) staff       (20)      288 2019-08-29 13:07:44.000000 coop_html_editor-1.3.1/coop_html_editor/static/ckeditor.4.6.2/plugins/widget/lang/id.js
--rw-r--r--   0 lucjean    (501) staff       (20)      266 2019-08-29 13:07:43.000000 coop_html_editor-1.3.1/coop_html_editor/static/ckeditor.4.6.2/plugins/widget/lang/az.js
--rw-r--r--   0 lucjean    (501) staff       (20)      273 2019-08-29 13:07:43.000000 coop_html_editor-1.3.1/coop_html_editor/static/ckeditor.4.6.2/plugins/widget/lang/ca.js
--rw-r--r--   0 lucjean    (501) staff       (20)      277 2019-08-29 13:07:43.000000 coop_html_editor-1.3.1/coop_html_editor/static/ckeditor.4.6.2/plugins/widget/lang/cy.js
--rw-r--r--   0 lucjean    (501) staff       (20)      270 2019-08-29 13:07:44.000000 coop_html_editor-1.3.1/coop_html_editor/static/ckeditor.4.6.2/plugins/widget/lang/nb.js
--rw-r--r--   0 lucjean    (501) staff       (20)      274 2019-08-29 13:07:45.000000 coop_html_editor-1.3.1/coop_html_editor/static/ckeditor.4.6.2/plugins/widget/lang/zh-cn.js
--rw-r--r--   0 lucjean    (501) staff       (20)      294 2019-08-29 13:07:43.000000 coop_html_editor-1.3.1/coop_html_editor/static/ckeditor.4.6.2/plugins/widget/lang/de-ch.js
--rw-r--r--   0 lucjean    (501) staff       (20)      273 2019-08-29 13:07:45.000000 coop_html_editor-1.3.1/coop_html_editor/static/ckeditor.4.6.2/plugins/widget/lang/pt-br.js
--rw-r--r--   0 lucjean    (501) staff       (20)      274 2019-08-29 13:07:44.000000 coop_html_editor-1.3.1/coop_html_editor/static/ckeditor.4.6.2/plugins/widget/lang/oc.js
--rw-r--r--   0 lucjean    (501) staff       (20)      282 2019-08-29 13:07:43.000000 coop_html_editor-1.3.1/coop_html_editor/static/ckeditor.4.6.2/plugins/widget/lang/da.js
--rw-r--r--   0 lucjean    (501) staff       (20)      301 2019-08-29 13:07:43.000000 coop_html_editor-1.3.1/coop_html_editor/static/ckeditor.4.6.2/plugins/widget/lang/fa.js
--rw-r--r--   0 lucjean    (501) staff       (20)      287 2019-08-29 13:07:43.000000 coop_html_editor-1.3.1/coop_html_editor/static/ckeditor.4.6.2/plugins/widget/lang/de.js
--rw-r--r--   0 lucjean    (501) staff       (20)      266 2019-08-29 13:07:43.000000 coop_html_editor-1.3.1/coop_html_editor/static/ckeditor.4.6.2/plugins/widget/lang/en.js
--rw-r--r--   0 lucjean    (501) staff       (20)      302 2019-08-29 13:07:44.000000 coop_html_editor-1.3.1/coop_html_editor/static/ckeditor.4.6.2/plugins/widget/lang/ku.js
--rw-r--r--   0 lucjean    (501) staff       (20)      275 2019-08-29 13:07:45.000000 coop_html_editor-1.3.1/coop_html_editor/static/ckeditor.4.6.2/plugins/widget/lang/sv.js
--rw-r--r--   0 lucjean    (501) staff       (20)      262 2019-08-29 13:07:45.000000 coop_html_editor-1.3.1/coop_html_editor/static/ckeditor.4.6.2/plugins/widget/lang/zh.js
--rw-r--r--   0 lucjean    (501) staff       (20)      318 2019-08-29 13:07:45.000000 coop_html_editor-1.3.1/coop_html_editor/static/ckeditor.4.6.2/plugins/widget/lang/uk.js
--rw-r--r--   0 lucjean    (501) staff       (20)      291 2019-08-29 13:07:43.000000 coop_html_editor-1.3.1/coop_html_editor/static/ckeditor.4.6.2/plugins/widget/lang/cs.js
--rw-r--r--   0 lucjean    (501) staff       (20)      339 2019-08-29 13:07:44.000000 coop_html_editor-1.3.1/coop_html_editor/static/ckeditor.4.6.2/plugins/widget/lang/km.js
--rw-r--r--   0 lucjean    (501) staff       (20)      280 2019-08-29 13:07:43.000000 coop_html_editor-1.3.1/coop_html_editor/static/ckeditor.4.6.2/plugins/widget/lang/fr.js
--rw-r--r--   0 lucjean    (501) staff       (20)      275 2019-08-29 13:07:44.000000 coop_html_editor-1.3.1/coop_html_editor/static/ckeditor.4.6.2/plugins/widget/lang/nl.js
--rw-r--r--   0 lucjean    (501) staff       (20)      280 2019-08-29 13:07:43.000000 coop_html_editor-1.3.1/coop_html_editor/static/ckeditor.4.6.2/plugins/widget/lang/en-gb.js
--rw-r--r--   0 lucjean    (501) staff       (20)      288 2019-08-29 13:07:44.000000 coop_html_editor-1.3.1/coop_html_editor/static/ckeditor.4.6.2/plugins/widget/lang/hu.js
--rw-r--r--   0 lucjean    (501) staff       (20)      290 2019-08-29 13:07:43.000000 coop_html_editor-1.3.1/coop_html_editor/static/ckeditor.4.6.2/plugins/widget/lang/ar.js
--rw-r--r--   0 lucjean    (501) staff       (20)      291 2019-08-29 13:07:45.000000 coop_html_editor-1.3.1/coop_html_editor/static/ckeditor.4.6.2/plugins/widget/lang/sk.js
--rw-r--r--   0 lucjean    (501) staff       (20)      279 2019-08-29 13:07:44.000000 coop_html_editor-1.3.1/coop_html_editor/static/ckeditor.4.6.2/plugins/widget/lang/it.js
--rw-r--r--   0 lucjean    (501) staff       (20)      280 2019-08-29 13:07:43.000000 coop_html_editor-1.3.1/coop_html_editor/static/ckeditor.4.6.2/plugins/widget/lang/es.js
--rw-r--r--   0 lucjean    (501) staff       (20)      279 2019-08-29 13:07:43.000000 coop_html_editor-1.3.1/coop_html_editor/static/ckeditor.4.6.2/plugins/widget/lang/eo.js
--rw-r--r--   0 lucjean    (501) staff       (20)      297 2019-08-29 13:07:45.000000 coop_html_editor-1.3.1/coop_html_editor/static/ckeditor.4.6.2/plugins/widget/lang/tr.js
-drwxr-xr-x   0 lucjean    (501) staff       (20)        0 2019-08-30 10:40:02.000000 coop_html_editor-1.3.1/coop_html_editor/static/ckeditor.4.6.2/plugins/widget/dev/
--rw-r--r--   0 lucjean    (501) staff       (20)     3699 2019-08-29 13:07:43.000000 coop_html_editor-1.3.1/coop_html_editor/static/ckeditor.4.6.2/plugins/widget/dev/console.js
--rw-r--r--   0 lucjean    (501) staff       (20)    11091 2019-08-29 13:07:43.000000 coop_html_editor-1.3.1/coop_html_editor/static/ckeditor.4.6.2/plugins/widget/dev/nestedwidgets.html
--rw-r--r--   0 lucjean    (501) staff       (20)     9707 2019-08-29 13:07:43.000000 coop_html_editor-1.3.1/coop_html_editor/static/ckeditor.4.6.2/plugins/widget/dev/widgetstyles.html
-drwxr-xr-x   0 lucjean    (501) staff       (20)        0 2019-08-30 10:40:02.000000 coop_html_editor-1.3.1/coop_html_editor/static/ckeditor.4.6.2/plugins/widget/dev/assets/
--rw-r--r--   0 lucjean    (501) staff       (20)      315 2019-08-29 13:07:43.000000 coop_html_editor-1.3.1/coop_html_editor/static/ckeditor.4.6.2/plugins/widget/dev/assets/contents.css
-drwxr-xr-x   0 lucjean    (501) staff       (20)        0 2019-08-30 10:40:02.000000 coop_html_editor-1.3.1/coop_html_editor/static/ckeditor.4.6.2/plugins/widget/dev/assets/simplebox/
--rw-r--r--   0 lucjean    (501) staff       (20)      635 2019-08-29 13:07:43.000000 coop_html_editor-1.3.1/coop_html_editor/static/ckeditor.4.6.2/plugins/widget/dev/assets/simplebox/contents.css
-drwxr-xr-x   0 lucjean    (501) staff       (20)        0 2019-08-30 10:40:02.000000 coop_html_editor-1.3.1/coop_html_editor/static/ckeditor.4.6.2/plugins/widget/dev/assets/simplebox/dialogs/
--rw-r--r--   0 lucjean    (501) staff       (20)     1596 2019-08-29 13:07:43.000000 coop_html_editor-1.3.1/coop_html_editor/static/ckeditor.4.6.2/plugins/widget/dev/assets/simplebox/dialogs/simplebox.js
--rw-r--r--   0 lucjean    (501) staff       (20)     4748 2019-08-29 13:07:43.000000 coop_html_editor-1.3.1/coop_html_editor/static/ckeditor.4.6.2/plugins/widget/dev/assets/simplebox/plugin.js
--rw-r--r--   0 lucjean    (501) staff       (20)    17932 2019-08-29 13:07:43.000000 coop_html_editor-1.3.1/coop_html_editor/static/ckeditor.4.6.2/plugins/widget/dev/assets/sample.jpg
--rw-r--r--   0 lucjean    (501) staff       (20)   136176 2019-08-29 13:07:45.000000 coop_html_editor-1.3.1/coop_html_editor/static/ckeditor.4.6.2/plugins/widget/plugin.js
-drwxr-xr-x   0 lucjean    (501) staff       (20)        0 2019-08-30 10:39:58.000000 coop_html_editor-1.3.1/coop_html_editor/static/ckeditor.4.6.2/plugins/embed/
--rw-r--r--   0 lucjean    (501) staff       (20)     3135 2019-08-29 13:07:42.000000 coop_html_editor-1.3.1/coop_html_editor/static/ckeditor.4.6.2/plugins/embed/plugin.js
-drwxr-xr-x   0 lucjean    (501) staff       (20)        0 2019-08-30 10:39:58.000000 coop_html_editor-1.3.1/coop_html_editor/static/ckeditor.4.6.2/plugins/embedbase/
-drwxr-xr-x   0 lucjean    (501) staff       (20)        0 2019-08-30 10:39:59.000000 coop_html_editor-1.3.1/coop_html_editor/static/ckeditor.4.6.2/plugins/embedbase/lang/
--rw-r--r--   0 lucjean    (501) staff       (20)      725 2019-08-29 13:07:42.000000 coop_html_editor-1.3.1/coop_html_editor/static/ckeditor.4.6.2/plugins/embedbase/lang/pt.js
--rw-r--r--   0 lucjean    (501) staff       (20)      706 2019-08-29 13:07:42.000000 coop_html_editor-1.3.1/coop_html_editor/static/ckeditor.4.6.2/plugins/embedbase/lang/gl.js
--rw-r--r--   0 lucjean    (501) staff       (20)      767 2019-08-29 13:07:42.000000 coop_html_editor-1.3.1/coop_html_editor/static/ckeditor.4.6.2/plugins/embedbase/lang/pl.js
--rw-r--r--   0 lucjean    (501) staff       (20)      779 2019-08-29 13:07:42.000000 coop_html_editor-1.3.1/coop_html_editor/static/ckeditor.4.6.2/plugins/embedbase/lang/ko.js
--rw-r--r--   0 lucjean    (501) staff       (20)      852 2019-08-29 13:07:42.000000 coop_html_editor-1.3.1/coop_html_editor/static/ckeditor.4.6.2/plugins/embedbase/lang/ru.js
--rw-r--r--   0 lucjean    (501) staff       (20)      679 2019-08-29 13:07:42.000000 coop_html_editor-1.3.1/coop_html_editor/static/ckeditor.4.6.2/plugins/embedbase/lang/eu.js
--rw-r--r--   0 lucjean    (501) staff       (20)      753 2019-08-29 13:07:42.000000 coop_html_editor-1.3.1/coop_html_editor/static/ckeditor.4.6.2/plugins/embedbase/lang/ja.js
--rw-r--r--   0 lucjean    (501) staff       (20)      768 2019-08-29 13:07:42.000000 coop_html_editor-1.3.1/coop_html_editor/static/ckeditor.4.6.2/plugins/embedbase/lang/ug.js
--rw-r--r--   0 lucjean    (501) staff       (20)      723 2019-08-29 13:07:42.000000 coop_html_editor-1.3.1/coop_html_editor/static/ckeditor.4.6.2/plugins/embedbase/lang/id.js
--rw-r--r--   0 lucjean    (501) staff       (20)      757 2019-08-29 13:07:42.000000 coop_html_editor-1.3.1/coop_html_editor/static/ckeditor.4.6.2/plugins/embedbase/lang/az.js
--rw-r--r--   0 lucjean    (501) staff       (20)      759 2019-08-29 13:07:42.000000 coop_html_editor-1.3.1/coop_html_editor/static/ckeditor.4.6.2/plugins/embedbase/lang/ca.js
--rw-r--r--   0 lucjean    (501) staff       (20)      655 2019-08-29 13:07:42.000000 coop_html_editor-1.3.1/coop_html_editor/static/ckeditor.4.6.2/plugins/embedbase/lang/nb.js
--rw-r--r--   0 lucjean    (501) staff       (20)      573 2019-08-29 13:07:42.000000 coop_html_editor-1.3.1/coop_html_editor/static/ckeditor.4.6.2/plugins/embedbase/lang/zh-cn.js
--rw-r--r--   0 lucjean    (501) staff       (20)      734 2019-08-29 13:07:42.000000 coop_html_editor-1.3.1/coop_html_editor/static/ckeditor.4.6.2/plugins/embedbase/lang/de-ch.js
--rw-r--r--   0 lucjean    (501) staff       (20)      702 2019-08-29 13:07:42.000000 coop_html_editor-1.3.1/coop_html_editor/static/ckeditor.4.6.2/plugins/embedbase/lang/pt-br.js
--rw-r--r--   0 lucjean    (501) staff       (20)      736 2019-08-29 13:07:42.000000 coop_html_editor-1.3.1/coop_html_editor/static/ckeditor.4.6.2/plugins/embedbase/lang/oc.js
--rw-r--r--   0 lucjean    (501) staff       (20)      648 2019-08-29 13:07:42.000000 coop_html_editor-1.3.1/coop_html_editor/static/ckeditor.4.6.2/plugins/embedbase/lang/da.js
--rw-r--r--   0 lucjean    (501) staff       (20)      731 2019-08-29 13:07:42.000000 coop_html_editor-1.3.1/coop_html_editor/static/ckeditor.4.6.2/plugins/embedbase/lang/de.js
--rw-r--r--   0 lucjean    (501) staff       (20)      643 2019-08-29 13:07:42.000000 coop_html_editor-1.3.1/coop_html_editor/static/ckeditor.4.6.2/plugins/embedbase/lang/en.js
--rw-r--r--   0 lucjean    (501) staff       (20)      964 2019-08-29 13:07:42.000000 coop_html_editor-1.3.1/coop_html_editor/static/ckeditor.4.6.2/plugins/embedbase/lang/ku.js
--rw-r--r--   0 lucjean    (501) staff       (20)      669 2019-08-29 13:07:42.000000 coop_html_editor-1.3.1/coop_html_editor/static/ckeditor.4.6.2/plugins/embedbase/lang/sv.js
--rw-r--r--   0 lucjean    (501) staff       (20)      626 2019-08-29 13:07:42.000000 coop_html_editor-1.3.1/coop_html_editor/static/ckeditor.4.6.2/plugins/embedbase/lang/zh.js
--rw-r--r--   0 lucjean    (501) staff       (20)      910 2019-08-29 13:07:42.000000 coop_html_editor-1.3.1/coop_html_editor/static/ckeditor.4.6.2/plugins/embedbase/lang/uk.js
--rw-r--r--   0 lucjean    (501) staff       (20)      636 2019-08-29 13:07:42.000000 coop_html_editor-1.3.1/coop_html_editor/static/ckeditor.4.6.2/plugins/embedbase/lang/cs.js
--rw-r--r--   0 lucjean    (501) staff       (20)      742 2019-08-29 13:07:42.000000 coop_html_editor-1.3.1/coop_html_editor/static/ckeditor.4.6.2/plugins/embedbase/lang/fr.js
--rw-r--r--   0 lucjean    (501) staff       (20)      686 2019-08-29 13:07:42.000000 coop_html_editor-1.3.1/coop_html_editor/static/ckeditor.4.6.2/plugins/embedbase/lang/nl.js
--rw-r--r--   0 lucjean    (501) staff       (20)      741 2019-08-29 13:07:42.000000 coop_html_editor-1.3.1/coop_html_editor/static/ckeditor.4.6.2/plugins/embedbase/lang/it.js
--rw-r--r--   0 lucjean    (501) staff       (20)      685 2019-08-29 13:07:42.000000 coop_html_editor-1.3.1/coop_html_editor/static/ckeditor.4.6.2/plugins/embedbase/lang/es.js
--rw-r--r--   0 lucjean    (501) staff       (20)      771 2019-08-29 13:07:42.000000 coop_html_editor-1.3.1/coop_html_editor/static/ckeditor.4.6.2/plugins/embedbase/lang/eo.js
--rw-r--r--   0 lucjean    (501) staff       (20)      690 2019-08-29 13:07:42.000000 coop_html_editor-1.3.1/coop_html_editor/static/ckeditor.4.6.2/plugins/embedbase/lang/tr.js
-drwxr-xr-x   0 lucjean    (501) staff       (20)        0 2019-08-30 10:39:58.000000 coop_html_editor-1.3.1/coop_html_editor/static/ckeditor.4.6.2/plugins/embedbase/dialogs/
--rw-r--r--   0 lucjean    (501) staff       (20)     2203 2019-08-29 13:07:42.000000 coop_html_editor-1.3.1/coop_html_editor/static/ckeditor.4.6.2/plugins/embedbase/dialogs/embedbase.js
--rw-r--r--   0 lucjean    (501) staff       (20)    21596 2019-08-29 13:07:42.000000 coop_html_editor-1.3.1/coop_html_editor/static/ckeditor.4.6.2/plugins/embedbase/plugin.js
-drwxr-xr-x   0 lucjean    (501) staff       (20)        0 2019-08-30 10:39:59.000000 coop_html_editor-1.3.1/coop_html_editor/static/ckeditor.4.6.2/plugins/notification/
-drwxr-xr-x   0 lucjean    (501) staff       (20)        0 2019-08-30 10:40:00.000000 coop_html_editor-1.3.1/coop_html_editor/static/ckeditor.4.6.2/plugins/notification/lang/
--rw-r--r--   0 lucjean    (501) staff       (20)      234 2019-08-29 13:07:42.000000 coop_html_editor-1.3.1/coop_html_editor/static/ckeditor.4.6.2/plugins/notification/lang/pt.js
--rw-r--r--   0 lucjean    (501) staff       (20)      232 2019-08-29 13:07:42.000000 coop_html_editor-1.3.1/coop_html_editor/static/ckeditor.4.6.2/plugins/notification/lang/gl.js
--rw-r--r--   0 lucjean    (501) staff       (20)      244 2019-08-29 13:07:42.000000 coop_html_editor-1.3.1/coop_html_editor/static/ckeditor.4.6.2/plugins/notification/lang/pl.js
--rw-r--r--   0 lucjean    (501) staff       (20)      227 2019-08-29 13:07:42.000000 coop_html_editor-1.3.1/coop_html_editor/static/ckeditor.4.6.2/plugins/notification/lang/ko.js
--rw-r--r--   0 lucjean    (501) staff       (20)      247 2019-08-29 13:07:42.000000 coop_html_editor-1.3.1/coop_html_editor/static/ckeditor.4.6.2/plugins/notification/lang/ru.js
--rw-r--r--   0 lucjean    (501) staff       (20)      231 2019-08-29 13:07:42.000000 coop_html_editor-1.3.1/coop_html_editor/static/ckeditor.4.6.2/plugins/notification/lang/eu.js
--rw-r--r--   0 lucjean    (501) staff       (20)      237 2019-08-29 13:07:42.000000 coop_html_editor-1.3.1/coop_html_editor/static/ckeditor.4.6.2/plugins/notification/lang/ja.js
--rw-r--r--   0 lucjean    (501) staff       (20)      242 2019-08-29 13:07:42.000000 coop_html_editor-1.3.1/coop_html_editor/static/ckeditor.4.6.2/plugins/notification/lang/ug.js
--rw-r--r--   0 lucjean    (501) staff       (20)      231 2019-08-29 13:07:42.000000 coop_html_editor-1.3.1/coop_html_editor/static/ckeditor.4.6.2/plugins/notification/lang/id.js
--rw-r--r--   0 lucjean    (501) staff       (20)      248 2019-08-29 13:07:42.000000 coop_html_editor-1.3.1/coop_html_editor/static/ckeditor.4.6.2/plugins/notification/lang/az.js
--rw-r--r--   0 lucjean    (501) staff       (20)      231 2019-08-29 13:07:42.000000 coop_html_editor-1.3.1/coop_html_editor/static/ckeditor.4.6.2/plugins/notification/lang/ca.js
--rw-r--r--   0 lucjean    (501) staff       (20)      226 2019-08-29 13:07:42.000000 coop_html_editor-1.3.1/coop_html_editor/static/ckeditor.4.6.2/plugins/notification/lang/nb.js
--rw-r--r--   0 lucjean    (501) staff       (20)      228 2019-08-29 13:07:42.000000 coop_html_editor-1.3.1/coop_html_editor/static/ckeditor.4.6.2/plugins/notification/lang/zh-cn.js
--rw-r--r--   0 lucjean    (501) staff       (20)      242 2019-08-29 13:07:42.000000 coop_html_editor-1.3.1/coop_html_editor/static/ckeditor.4.6.2/plugins/notification/lang/de-ch.js
--rw-r--r--   0 lucjean    (501) staff       (20)      235 2019-08-29 13:07:42.000000 coop_html_editor-1.3.1/coop_html_editor/static/ckeditor.4.6.2/plugins/notification/lang/pt-br.js
--rw-r--r--   0 lucjean    (501) staff       (20)      231 2019-08-29 13:07:42.000000 coop_html_editor-1.3.1/coop_html_editor/static/ckeditor.4.6.2/plugins/notification/lang/oc.js
--rw-r--r--   0 lucjean    (501) staff       (20)      230 2019-08-29 13:07:42.000000 coop_html_editor-1.3.1/coop_html_editor/static/ckeditor.4.6.2/plugins/notification/lang/da.js
--rw-r--r--   0 lucjean    (501) staff       (20)      239 2019-08-29 13:07:42.000000 coop_html_editor-1.3.1/coop_html_editor/static/ckeditor.4.6.2/plugins/notification/lang/de.js
--rw-r--r--   0 lucjean    (501) staff       (20)      230 2019-08-29 13:07:42.000000 coop_html_editor-1.3.1/coop_html_editor/static/ckeditor.4.6.2/plugins/notification/lang/en.js
--rw-r--r--   0 lucjean    (501) staff       (20)      252 2019-08-29 13:07:42.000000 coop_html_editor-1.3.1/coop_html_editor/static/ckeditor.4.6.2/plugins/notification/lang/ku.js
--rw-r--r--   0 lucjean    (501) staff       (20)      230 2019-08-29 13:07:42.000000 coop_html_editor-1.3.1/coop_html_editor/static/ckeditor.4.6.2/plugins/notification/lang/sv.js
--rw-r--r--   0 lucjean    (501) staff       (20)      228 2019-08-29 13:07:42.000000 coop_html_editor-1.3.1/coop_html_editor/static/ckeditor.4.6.2/plugins/notification/lang/zh.js
--rw-r--r--   0 lucjean    (501) staff       (20)      246 2019-08-29 13:07:42.000000 coop_html_editor-1.3.1/coop_html_editor/static/ckeditor.4.6.2/plugins/notification/lang/uk.js
--rw-r--r--   0 lucjean    (501) staff       (20)      230 2019-08-29 13:07:42.000000 coop_html_editor-1.3.1/coop_html_editor/static/ckeditor.4.6.2/plugins/notification/lang/cs.js
--rw-r--r--   0 lucjean    (501) staff       (20)      282 2019-08-29 13:07:42.000000 coop_html_editor-1.3.1/coop_html_editor/static/ckeditor.4.6.2/plugins/notification/lang/km.js
--rw-r--r--   0 lucjean    (501) staff       (20)      231 2019-08-29 13:07:42.000000 coop_html_editor-1.3.1/coop_html_editor/static/ckeditor.4.6.2/plugins/notification/lang/fr.js
--rw-r--r--   0 lucjean    (501) staff       (20)      227 2019-08-29 13:07:42.000000 coop_html_editor-1.3.1/coop_html_editor/static/ckeditor.4.6.2/plugins/notification/lang/nl.js
--rw-r--r--   0 lucjean    (501) staff       (20)      226 2019-08-29 13:07:42.000000 coop_html_editor-1.3.1/coop_html_editor/static/ckeditor.4.6.2/plugins/notification/lang/it.js
--rw-r--r--   0 lucjean    (501) staff       (20)      232 2019-08-29 13:07:42.000000 coop_html_editor-1.3.1/coop_html_editor/static/ckeditor.4.6.2/plugins/notification/lang/es.js
--rw-r--r--   0 lucjean    (501) staff       (20)      224 2019-08-29 13:07:42.000000 coop_html_editor-1.3.1/coop_html_editor/static/ckeditor.4.6.2/plugins/notification/lang/eo.js
--rw-r--r--   0 lucjean    (501) staff       (20)      232 2019-08-29 13:07:42.000000 coop_html_editor-1.3.1/coop_html_editor/static/ckeditor.4.6.2/plugins/notification/lang/tr.js
--rw-r--r--   0 lucjean    (501) staff       (20)    33609 2019-08-29 13:07:42.000000 coop_html_editor-1.3.1/coop_html_editor/static/ckeditor.4.6.2/plugins/notification/plugin.js
-drwxr-xr-x   0 lucjean    (501) staff       (20)        0 2019-08-30 10:39:35.000000 coop_html_editor-1.3.1/coop_html_editor/static/ckeditor.4.6.2/plugins/tabletools/
-drwxr-xr-x   0 lucjean    (501) staff       (20)        0 2019-08-30 10:40:01.000000 coop_html_editor-1.3.1/coop_html_editor/static/ckeditor.4.6.2/plugins/tabletools/dialogs/
--rw-r--r--   0 lucjean    (501) staff       (20)     6715 2019-08-29 13:07:43.000000 coop_html_editor-1.3.1/coop_html_editor/static/ckeditor.4.6.2/plugins/tabletools/dialogs/tableCell.js
-drwxr-xr-x   0 lucjean    (501) staff       (20)        0 2019-08-30 10:39:35.000000 coop_html_editor-1.3.1/coop_html_editor/static/ckeditor.4.6.2/plugins/pastefromword/
-drwxr-xr-x   0 lucjean    (501) staff       (20)        0 2019-08-30 10:40:00.000000 coop_html_editor-1.3.1/coop_html_editor/static/ckeditor.4.6.2/plugins/pastefromword/filter/
--rw-r--r--   0 lucjean    (501) staff       (20)    19971 2019-08-29 13:07:42.000000 coop_html_editor-1.3.1/coop_html_editor/static/ckeditor.4.6.2/plugins/pastefromword/filter/default.js
-drwxr-xr-x   0 lucjean    (501) staff       (20)        0 2019-08-30 10:40:01.000000 coop_html_editor-1.3.1/coop_html_editor/static/ckeditor.4.6.2/plugins/toolbar/
-drwxr-xr-x   0 lucjean    (501) staff       (20)        0 2019-08-30 10:40:02.000000 coop_html_editor-1.3.1/coop_html_editor/static/ckeditor.4.6.2/plugins/toolbar/lang/
--rw-r--r--   0 lucjean    (501) staff       (20)      573 2019-08-29 13:07:43.000000 coop_html_editor-1.3.1/coop_html_editor/static/ckeditor.4.6.2/plugins/toolbar/lang/sr-latn.js
--rw-r--r--   0 lucjean    (501) staff       (20)      653 2019-08-29 13:07:43.000000 coop_html_editor-1.3.1/coop_html_editor/static/ckeditor.4.6.2/plugins/toolbar/lang/pt.js
--rw-r--r--   0 lucjean    (501) staff       (20)      621 2019-08-29 13:07:43.000000 coop_html_editor-1.3.1/coop_html_editor/static/ckeditor.4.6.2/plugins/toolbar/lang/vi.js
--rw-r--r--   0 lucjean    (501) staff       (20)      586 2019-08-29 13:07:43.000000 coop_html_editor-1.3.1/coop_html_editor/static/ckeditor.4.6.2/plugins/toolbar/lang/lv.js
--rw-r--r--   0 lucjean    (501) staff       (20)      640 2019-08-29 13:07:43.000000 coop_html_editor-1.3.1/coop_html_editor/static/ckeditor.4.6.2/plugins/toolbar/lang/gl.js
--rw-r--r--   0 lucjean    (501) staff       (20)      605 2019-08-29 13:07:43.000000 coop_html_editor-1.3.1/coop_html_editor/static/ckeditor.4.6.2/plugins/toolbar/lang/pl.js
--rw-r--r--   0 lucjean    (501) staff       (20)      694 2019-08-29 13:07:43.000000 coop_html_editor-1.3.1/coop_html_editor/static/ckeditor.4.6.2/plugins/toolbar/lang/mn.js
--rw-r--r--   0 lucjean    (501) staff       (20)      599 2019-08-29 13:07:43.000000 coop_html_editor-1.3.1/coop_html_editor/static/ckeditor.4.6.2/plugins/toolbar/lang/en-ca.js
--rw-r--r--   0 lucjean    (501) staff       (20)      764 2019-08-29 13:07:43.000000 coop_html_editor-1.3.1/coop_html_editor/static/ckeditor.4.6.2/plugins/toolbar/lang/el.js
--rw-r--r--   0 lucjean    (501) staff       (20)      614 2019-08-29 13:07:43.000000 coop_html_editor-1.3.1/coop_html_editor/static/ckeditor.4.6.2/plugins/toolbar/lang/et.js
--rw-r--r--   0 lucjean    (501) staff       (20)      596 2019-08-29 13:07:43.000000 coop_html_editor-1.3.1/coop_html_editor/static/ckeditor.4.6.2/plugins/toolbar/lang/is.js
--rw-r--r--   0 lucjean    (501) staff       (20)      603 2019-08-29 13:07:43.000000 coop_html_editor-1.3.1/coop_html_editor/static/ckeditor.4.6.2/plugins/toolbar/lang/sl.js
--rw-r--r--   0 lucjean    (501) staff       (20)      576 2019-08-29 13:07:43.000000 coop_html_editor-1.3.1/coop_html_editor/static/ckeditor.4.6.2/plugins/toolbar/lang/ko.js
--rw-r--r--   0 lucjean    (501) staff       (20)      602 2019-08-29 13:07:43.000000 coop_html_editor-1.3.1/coop_html_editor/static/ckeditor.4.6.2/plugins/toolbar/lang/hr.js
--rw-r--r--   0 lucjean    (501) staff       (20)      596 2019-08-29 13:07:43.000000 coop_html_editor-1.3.1/coop_html_editor/static/ckeditor.4.6.2/plugins/toolbar/lang/ms.js
--rw-r--r--   0 lucjean    (501) staff       (20)      600 2019-08-29 13:07:43.000000 coop_html_editor-1.3.1/coop_html_editor/static/ckeditor.4.6.2/plugins/toolbar/lang/fi.js
--rw-r--r--   0 lucjean    (501) staff       (20)      707 2019-08-29 13:07:43.000000 coop_html_editor-1.3.1/coop_html_editor/static/ckeditor.4.6.2/plugins/toolbar/lang/th.js
--rw-r--r--   0 lucjean    (501) staff       (20)      813 2019-08-29 13:07:43.000000 coop_html_editor-1.3.1/coop_html_editor/static/ckeditor.4.6.2/plugins/toolbar/lang/ru.js
--rw-r--r--   0 lucjean    (501) staff       (20)      610 2019-08-29 13:07:43.000000 coop_html_editor-1.3.1/coop_html_editor/static/ckeditor.4.6.2/plugins/toolbar/lang/eu.js
--rw-r--r--   0 lucjean    (501) staff       (20)      596 2019-08-29 13:07:43.000000 coop_html_editor-1.3.1/coop_html_editor/static/ckeditor.4.6.2/plugins/toolbar/lang/mk.js
--rw-r--r--   0 lucjean    (501) staff       (20)      593 2019-08-29 13:07:43.000000 coop_html_editor-1.3.1/coop_html_editor/static/ckeditor.4.6.2/plugins/toolbar/lang/no.js
--rw-r--r--   0 lucjean    (501) staff       (20)      585 2019-08-29 13:07:43.000000 coop_html_editor-1.3.1/coop_html_editor/static/ckeditor.4.6.2/plugins/toolbar/lang/sq.js
--rw-r--r--   0 lucjean    (501) staff       (20)      798 2019-08-29 13:07:43.000000 coop_html_editor-1.3.1/coop_html_editor/static/ckeditor.4.6.2/plugins/toolbar/lang/gu.js
--rw-r--r--   0 lucjean    (501) staff       (20)      860 2019-08-29 13:07:43.000000 coop_html_editor-1.3.1/coop_html_editor/static/ckeditor.4.6.2/plugins/toolbar/lang/si.js
--rw-r--r--   0 lucjean    (501) staff       (20)      714 2019-08-29 13:07:43.000000 coop_html_editor-1.3.1/coop_html_editor/static/ckeditor.4.6.2/plugins/toolbar/lang/tt.js
--rw-r--r--   0 lucjean    (501) staff       (20)      590 2019-08-29 13:07:43.000000 coop_html_editor-1.3.1/coop_html_editor/static/ckeditor.4.6.2/plugins/toolbar/lang/ja.js
--rw-r--r--   0 lucjean    (501) staff       (20)      884 2019-08-29 13:07:43.000000 coop_html_editor-1.3.1/coop_html_editor/static/ckeditor.4.6.2/plugins/toolbar/lang/ka.js
--rw-r--r--   0 lucjean    (501) staff       (20)      686 2019-08-29 13:07:43.000000 coop_html_editor-1.3.1/coop_html_editor/static/ckeditor.4.6.2/plugins/toolbar/lang/he.js
--rw-r--r--   0 lucjean    (501) staff       (20)      699 2019-08-29 13:07:43.000000 coop_html_editor-1.3.1/coop_html_editor/static/ckeditor.4.6.2/plugins/toolbar/lang/ug.js
--rw-r--r--   0 lucjean    (501) staff       (20)      789 2019-08-29 13:07:43.000000 coop_html_editor-1.3.1/coop_html_editor/static/ckeditor.4.6.2/plugins/toolbar/lang/bg.js
--rw-r--r--   0 lucjean    (501) staff       (20)      571 2019-08-29 13:07:43.000000 coop_html_editor-1.3.1/coop_html_editor/static/ckeditor.4.6.2/plugins/toolbar/lang/af.js
--rw-r--r--   0 lucjean    (501) staff       (20)      583 2019-08-29 13:07:43.000000 coop_html_editor-1.3.1/coop_html_editor/static/ckeditor.4.6.2/plugins/toolbar/lang/id.js
--rw-r--r--   0 lucjean    (501) staff       (20)      606 2019-08-29 13:07:43.000000 coop_html_editor-1.3.1/coop_html_editor/static/ckeditor.4.6.2/plugins/toolbar/lang/az.js
--rw-r--r--   0 lucjean    (501) staff       (20)      588 2019-08-29 13:07:43.000000 coop_html_editor-1.3.1/coop_html_editor/static/ckeditor.4.6.2/plugins/toolbar/lang/en-au.js
--rw-r--r--   0 lucjean    (501) staff       (20)      591 2019-08-29 13:07:43.000000 coop_html_editor-1.3.1/coop_html_editor/static/ckeditor.4.6.2/plugins/toolbar/lang/ca.js
--rw-r--r--   0 lucjean    (501) staff       (20)      603 2019-08-29 13:07:43.000000 coop_html_editor-1.3.1/coop_html_editor/static/ckeditor.4.6.2/plugins/toolbar/lang/cy.js
--rw-r--r--   0 lucjean    (501) staff       (20)      593 2019-08-29 13:07:43.000000 coop_html_editor-1.3.1/coop_html_editor/static/ckeditor.4.6.2/plugins/toolbar/lang/nb.js
--rw-r--r--   0 lucjean    (501) staff       (20)      559 2019-08-29 13:07:43.000000 coop_html_editor-1.3.1/coop_html_editor/static/ckeditor.4.6.2/plugins/toolbar/lang/zh-cn.js
--rw-r--r--   0 lucjean    (501) staff       (20)      613 2019-08-29 13:07:43.000000 coop_html_editor-1.3.1/coop_html_editor/static/ckeditor.4.6.2/plugins/toolbar/lang/de-ch.js
--rw-r--r--   0 lucjean    (501) staff       (20)      633 2019-08-29 13:07:43.000000 coop_html_editor-1.3.1/coop_html_editor/static/ckeditor.4.6.2/plugins/toolbar/lang/pt-br.js
--rw-r--r--   0 lucjean    (501) staff       (20)      623 2019-08-29 13:07:43.000000 coop_html_editor-1.3.1/coop_html_editor/static/ckeditor.4.6.2/plugins/toolbar/lang/oc.js
--rw-r--r--   0 lucjean    (501) staff       (20)      615 2019-08-29 13:07:43.000000 coop_html_editor-1.3.1/coop_html_editor/static/ckeditor.4.6.2/plugins/toolbar/lang/da.js
--rw-r--r--   0 lucjean    (501) staff       (20)      707 2019-08-29 13:07:43.000000 coop_html_editor-1.3.1/coop_html_editor/static/ckeditor.4.6.2/plugins/toolbar/lang/fa.js
--rw-r--r--   0 lucjean    (501) staff       (20)      610 2019-08-29 13:07:43.000000 coop_html_editor-1.3.1/coop_html_editor/static/ckeditor.4.6.2/plugins/toolbar/lang/de.js
--rw-r--r--   0 lucjean    (501) staff       (20)      563 2019-08-29 13:07:43.000000 coop_html_editor-1.3.1/coop_html_editor/static/ckeditor.4.6.2/plugins/toolbar/lang/en.js
--rw-r--r--   0 lucjean    (501) staff       (20)      596 2019-08-29 13:07:43.000000 coop_html_editor-1.3.1/coop_html_editor/static/ckeditor.4.6.2/plugins/toolbar/lang/bs.js
--rw-r--r--   0 lucjean    (501) staff       (20)      743 2019-08-29 13:07:43.000000 coop_html_editor-1.3.1/coop_html_editor/static/ckeditor.4.6.2/plugins/toolbar/lang/ku.js
--rw-r--r--   0 lucjean    (501) staff       (20)      585 2019-08-29 13:07:43.000000 coop_html_editor-1.3.1/coop_html_editor/static/ckeditor.4.6.2/plugins/toolbar/lang/sv.js
--rw-r--r--   0 lucjean    (501) staff       (20)      571 2019-08-29 13:07:43.000000 coop_html_editor-1.3.1/coop_html_editor/static/ckeditor.4.6.2/plugins/toolbar/lang/zh.js
--rw-r--r--   0 lucjean    (501) staff       (20)      604 2019-08-29 13:07:43.000000 coop_html_editor-1.3.1/coop_html_editor/static/ckeditor.4.6.2/plugins/toolbar/lang/hi.js
--rw-r--r--   0 lucjean    (501) staff       (20)      818 2019-08-29 13:07:43.000000 coop_html_editor-1.3.1/coop_html_editor/static/ckeditor.4.6.2/plugins/toolbar/lang/uk.js
--rw-r--r--   0 lucjean    (501) staff       (20)      605 2019-08-29 13:07:43.000000 coop_html_editor-1.3.1/coop_html_editor/static/ckeditor.4.6.2/plugins/toolbar/lang/cs.js
--rw-r--r--   0 lucjean    (501) staff       (20)      859 2019-08-29 13:07:43.000000 coop_html_editor-1.3.1/coop_html_editor/static/ckeditor.4.6.2/plugins/toolbar/lang/km.js
--rw-r--r--   0 lucjean    (501) staff       (20)      627 2019-08-29 13:07:43.000000 coop_html_editor-1.3.1/coop_html_editor/static/ckeditor.4.6.2/plugins/toolbar/lang/fr.js
--rw-r--r--   0 lucjean    (501) staff       (20)      592 2019-08-29 13:07:43.000000 coop_html_editor-1.3.1/coop_html_editor/static/ckeditor.4.6.2/plugins/toolbar/lang/nl.js
--rw-r--r--   0 lucjean    (501) staff       (20)      628 2019-08-29 13:07:43.000000 coop_html_editor-1.3.1/coop_html_editor/static/ckeditor.4.6.2/plugins/toolbar/lang/fr-ca.js
--rw-r--r--   0 lucjean    (501) staff       (20)      566 2019-08-29 13:07:43.000000 coop_html_editor-1.3.1/coop_html_editor/static/ckeditor.4.6.2/plugins/toolbar/lang/en-gb.js
--rw-r--r--   0 lucjean    (501) staff       (20)      628 2019-08-29 13:07:43.000000 coop_html_editor-1.3.1/coop_html_editor/static/ckeditor.4.6.2/plugins/toolbar/lang/sr.js
--rw-r--r--   0 lucjean    (501) staff       (20)      632 2019-08-29 13:07:43.000000 coop_html_editor-1.3.1/coop_html_editor/static/ckeditor.4.6.2/plugins/toolbar/lang/hu.js
--rw-r--r--   0 lucjean    (501) staff       (20)      623 2019-08-29 13:07:43.000000 coop_html_editor-1.3.1/coop_html_editor/static/ckeditor.4.6.2/plugins/toolbar/lang/lt.js
--rw-r--r--   0 lucjean    (501) staff       (20)      576 2019-08-29 13:07:43.000000 coop_html_editor-1.3.1/coop_html_editor/static/ckeditor.4.6.2/plugins/toolbar/lang/fo.js
--rw-r--r--   0 lucjean    (501) staff       (20)      665 2019-08-29 13:07:43.000000 coop_html_editor-1.3.1/coop_html_editor/static/ckeditor.4.6.2/plugins/toolbar/lang/ar.js
--rw-r--r--   0 lucjean    (501) staff       (20)      632 2019-08-29 13:07:43.000000 coop_html_editor-1.3.1/coop_html_editor/static/ckeditor.4.6.2/plugins/toolbar/lang/sk.js
--rw-r--r--   0 lucjean    (501) staff       (20)      584 2019-08-29 13:07:43.000000 coop_html_editor-1.3.1/coop_html_editor/static/ckeditor.4.6.2/plugins/toolbar/lang/it.js
--rw-r--r--   0 lucjean    (501) staff       (20)      642 2019-08-29 13:07:43.000000 coop_html_editor-1.3.1/coop_html_editor/static/ckeditor.4.6.2/plugins/toolbar/lang/es.js
--rw-r--r--   0 lucjean    (501) staff       (20)      596 2019-08-29 13:07:43.000000 coop_html_editor-1.3.1/coop_html_editor/static/ckeditor.4.6.2/plugins/toolbar/lang/bn.js
--rw-r--r--   0 lucjean    (501) staff       (20)      589 2019-08-29 13:07:43.000000 coop_html_editor-1.3.1/coop_html_editor/static/ckeditor.4.6.2/plugins/toolbar/lang/eo.js
--rw-r--r--   0 lucjean    (501) staff       (20)      573 2019-08-29 13:07:43.000000 coop_html_editor-1.3.1/coop_html_editor/static/ckeditor.4.6.2/plugins/toolbar/lang/ro.js
--rw-r--r--   0 lucjean    (501) staff       (20)      606 2019-08-29 13:07:43.000000 coop_html_editor-1.3.1/coop_html_editor/static/ckeditor.4.6.2/plugins/toolbar/lang/tr.js
-drwxr-xr-x   0 lucjean    (501) staff       (20)        0 2019-08-30 10:40:02.000000 coop_html_editor-1.3.1/coop_html_editor/static/ckeditor.4.6.2/plugins/toolbar/samples/
--rw-r--r--   0 lucjean    (501) staff       (20)     8665 2019-08-29 13:07:43.000000 coop_html_editor-1.3.1/coop_html_editor/static/ckeditor.4.6.2/plugins/toolbar/samples/toolbar.html
--rw-r--r--   0 lucjean    (501) staff       (20)    25525 2019-08-29 13:07:43.000000 coop_html_editor-1.3.1/coop_html_editor/static/ckeditor.4.6.2/plugins/toolbar/plugin.js
-drwxr-xr-x   0 lucjean    (501) staff       (20)        0 2019-08-30 10:39:55.000000 coop_html_editor-1.3.1/coop_html_editor/static/ckeditor.4.6.2/plugins/btgrid/
--rw-r--r--   0 lucjean    (501) staff       (20)      570 2019-08-29 13:07:42.000000 coop_html_editor-1.3.1/coop_html_editor/static/ckeditor.4.6.2/plugins/btgrid/bower.json
--rw-r--r--   0 lucjean    (501) staff       (20)      548 2019-08-29 13:07:42.000000 coop_html_editor-1.3.1/coop_html_editor/static/ckeditor.4.6.2/plugins/btgrid/README.md
-drwxr-xr-x   0 lucjean    (501) staff       (20)        0 2019-08-30 10:39:55.000000 coop_html_editor-1.3.1/coop_html_editor/static/ckeditor.4.6.2/plugins/btgrid/lang/
--rw-r--r--   0 lucjean    (501) staff       (20)      556 2019-08-29 13:07:42.000000 coop_html_editor-1.3.1/coop_html_editor/static/ckeditor.4.6.2/plugins/btgrid/lang/ru.js
--rw-r--r--   0 lucjean    (501) staff       (20)      365 2019-08-29 13:07:42.000000 coop_html_editor-1.3.1/coop_html_editor/static/ckeditor.4.6.2/plugins/btgrid/lang/en.js
--rw-r--r--   0 lucjean    (501) staff       (20)      369 2019-08-29 13:07:42.000000 coop_html_editor-1.3.1/coop_html_editor/static/ckeditor.4.6.2/plugins/btgrid/lang/fr.js
--rw-r--r--   0 lucjean    (501) staff       (20)      330 2019-08-29 13:07:42.000000 coop_html_editor-1.3.1/coop_html_editor/static/ckeditor.4.6.2/plugins/btgrid/lang/nl.js
-drwxr-xr-x   0 lucjean    (501) staff       (20)        0 2019-08-30 10:39:55.000000 coop_html_editor-1.3.1/coop_html_editor/static/ckeditor.4.6.2/plugins/btgrid/styles/
--rw-r--r--   0 lucjean    (501) staff       (20)     1432 2019-08-29 13:07:42.000000 coop_html_editor-1.3.1/coop_html_editor/static/ckeditor.4.6.2/plugins/btgrid/styles/editor.css
-drwxr-xr-x   0 lucjean    (501) staff       (20)        0 2019-08-30 10:39:55.000000 coop_html_editor-1.3.1/coop_html_editor/static/ckeditor.4.6.2/plugins/btgrid/dialogs/
--rw-r--r--   0 lucjean    (501) staff       (20)     2392 2019-08-29 13:07:42.000000 coop_html_editor-1.3.1/coop_html_editor/static/ckeditor.4.6.2/plugins/btgrid/dialogs/btgrid.js
--rw-r--r--   0 lucjean    (501) staff       (20)     1072 2019-08-29 13:07:42.000000 coop_html_editor-1.3.1/coop_html_editor/static/ckeditor.4.6.2/plugins/btgrid/LICENSE.txt
--rw-r--r--   0 lucjean    (501) staff       (20)     3240 2019-08-29 13:07:42.000000 coop_html_editor-1.3.1/coop_html_editor/static/ckeditor.4.6.2/plugins/btgrid/plugin.js
-drwxr-xr-x   0 lucjean    (501) staff       (20)        0 2019-08-30 10:39:35.000000 coop_html_editor-1.3.1/coop_html_editor/static/ckeditor.4.6.2/plugins/about/
-drwxr-xr-x   0 lucjean    (501) staff       (20)        0 2019-08-30 10:39:55.000000 coop_html_editor-1.3.1/coop_html_editor/static/ckeditor.4.6.2/plugins/about/dialogs/
--rw-r--r--   0 lucjean    (501) staff       (20)     1886 2019-08-29 13:07:42.000000 coop_html_editor-1.3.1/coop_html_editor/static/ckeditor.4.6.2/plugins/about/dialogs/about.js
-drwxr-xr-x   0 lucjean    (501) staff       (20)        0 2019-08-30 10:39:55.000000 coop_html_editor-1.3.1/coop_html_editor/static/ckeditor.4.6.2/plugins/about/dialogs/hidpi/
--rw-r--r--   0 lucjean    (501) staff       (20)    13339 2019-08-29 13:07:42.000000 coop_html_editor-1.3.1/coop_html_editor/static/ckeditor.4.6.2/plugins/about/dialogs/hidpi/logo_ckeditor.png
--rw-r--r--   0 lucjean    (501) staff       (20)     6757 2019-08-29 13:07:42.000000 coop_html_editor-1.3.1/coop_html_editor/static/ckeditor.4.6.2/plugins/about/dialogs/logo_ckeditor.png
-drwxr-xr-x   0 lucjean    (501) staff       (20)        0 2019-08-30 10:40:02.000000 coop_html_editor-1.3.1/coop_html_editor/static/ckeditor.4.6.2/plugins/videoembed/
-drwxr-xr-x   0 lucjean    (501) staff       (20)        0 2019-08-30 10:40:02.000000 coop_html_editor-1.3.1/coop_html_editor/static/ckeditor.4.6.2/plugins/videoembed/lang/
--rwxr-xr-x   0 lucjean    (501) staff       (20)      256 2019-08-29 13:07:43.000000 coop_html_editor-1.3.1/coop_html_editor/static/ckeditor.4.6.2/plugins/videoembed/lang/en.js
--rwxr-xr-x   0 lucjean    (501) staff       (20)      289 2019-08-29 13:07:43.000000 coop_html_editor-1.3.1/coop_html_editor/static/ckeditor.4.6.2/plugins/videoembed/lang/fr.js
-drwxr-xr-x   0 lucjean    (501) staff       (20)        0 2019-08-30 10:40:02.000000 coop_html_editor-1.3.1/coop_html_editor/static/ckeditor.4.6.2/plugins/videoembed/dialogs/
--rwxr-xr-x   0 lucjean    (501) staff       (20)     4089 2019-08-29 13:07:43.000000 coop_html_editor-1.3.1/coop_html_editor/static/ckeditor.4.6.2/plugins/videoembed/dialogs/videoembedDialog.js
--rwxr-xr-x   0 lucjean    (501) staff       (20)      761 2019-08-29 13:07:43.000000 coop_html_editor-1.3.1/coop_html_editor/static/ckeditor.4.6.2/plugins/videoembed/plugin.js
-drwxr-xr-x   0 lucjean    (501) staff       (20)        0 2019-08-30 10:39:35.000000 coop_html_editor-1.3.1/coop_html_editor/static/ckeditor.4.6.2/plugins/image/
-drwxr-xr-x   0 lucjean    (501) staff       (20)        0 2019-08-30 10:39:59.000000 coop_html_editor-1.3.1/coop_html_editor/static/ckeditor.4.6.2/plugins/image/images/
--rw-r--r--   0 lucjean    (501) staff       (20)     1610 2019-08-29 13:07:42.000000 coop_html_editor-1.3.1/coop_html_editor/static/ckeditor.4.6.2/plugins/image/images/noimage.png
-drwxr-xr-x   0 lucjean    (501) staff       (20)        0 2019-08-30 10:39:59.000000 coop_html_editor-1.3.1/coop_html_editor/static/ckeditor.4.6.2/plugins/image/dialogs/
--rw-r--r--   0 lucjean    (501) staff       (20)    21266 2019-08-29 13:07:42.000000 coop_html_editor-1.3.1/coop_html_editor/static/ckeditor.4.6.2/plugins/image/dialogs/image.js
-drwxr-xr-x   0 lucjean    (501) staff       (20)        0 2019-08-30 10:39:58.000000 coop_html_editor-1.3.1/coop_html_editor/static/ckeditor.4.6.2/plugins/dialog/
--rw-r--r--   0 lucjean    (501) staff       (20)      148 2019-08-29 13:07:42.000000 coop_html_editor-1.3.1/coop_html_editor/static/ckeditor.4.6.2/plugins/dialog/dialogDefinition.js
-drwxr-xr-x   0 lucjean    (501) staff       (20)        0 2019-08-30 10:39:55.000000 coop_html_editor-1.3.1/coop_html_editor/static/ckeditor.4.6.2/plugins/button/
-drwxr-xr-x   0 lucjean    (501) staff       (20)        0 2019-08-30 10:39:56.000000 coop_html_editor-1.3.1/coop_html_editor/static/ckeditor.4.6.2/plugins/button/lang/
--rw-r--r--   0 lucjean    (501) staff       (20)      245 2019-08-29 13:07:42.000000 coop_html_editor-1.3.1/coop_html_editor/static/ckeditor.4.6.2/plugins/button/lang/pt.js
--rw-r--r--   0 lucjean    (501) staff       (20)      245 2019-08-29 13:07:42.000000 coop_html_editor-1.3.1/coop_html_editor/static/ckeditor.4.6.2/plugins/button/lang/vi.js
--rw-r--r--   0 lucjean    (501) staff       (20)      246 2019-08-29 13:07:42.000000 coop_html_editor-1.3.1/coop_html_editor/static/ckeditor.4.6.2/plugins/button/lang/gl.js
--rw-r--r--   0 lucjean    (501) staff       (20)      241 2019-08-29 13:07:42.000000 coop_html_editor-1.3.1/coop_html_editor/static/ckeditor.4.6.2/plugins/button/lang/pl.js
--rw-r--r--   0 lucjean    (501) staff       (20)      254 2019-08-29 13:07:42.000000 coop_html_editor-1.3.1/coop_html_editor/static/ckeditor.4.6.2/plugins/button/lang/el.js
--rw-r--r--   0 lucjean    (501) staff       (20)      241 2019-08-29 13:07:42.000000 coop_html_editor-1.3.1/coop_html_editor/static/ckeditor.4.6.2/plugins/button/lang/sl.js
--rw-r--r--   0 lucjean    (501) staff       (20)      243 2019-08-29 13:07:42.000000 coop_html_editor-1.3.1/coop_html_editor/static/ckeditor.4.6.2/plugins/button/lang/ko.js
--rw-r--r--   0 lucjean    (501) staff       (20)      241 2019-08-29 13:07:42.000000 coop_html_editor-1.3.1/coop_html_editor/static/ckeditor.4.6.2/plugins/button/lang/fi.js
--rw-r--r--   0 lucjean    (501) staff       (20)      248 2019-08-29 13:07:42.000000 coop_html_editor-1.3.1/coop_html_editor/static/ckeditor.4.6.2/plugins/button/lang/ru.js
--rw-r--r--   0 lucjean    (501) staff       (20)      243 2019-08-29 13:07:42.000000 coop_html_editor-1.3.1/coop_html_editor/static/ckeditor.4.6.2/plugins/button/lang/eu.js
--rw-r--r--   0 lucjean    (501) staff       (20)      239 2019-08-29 13:07:42.000000 coop_html_editor-1.3.1/coop_html_editor/static/ckeditor.4.6.2/plugins/button/lang/no.js
--rw-r--r--   0 lucjean    (501) staff       (20)      246 2019-08-29 13:07:42.000000 coop_html_editor-1.3.1/coop_html_editor/static/ckeditor.4.6.2/plugins/button/lang/sq.js
--rw-r--r--   0 lucjean    (501) staff       (20)      252 2019-08-29 13:07:42.000000 coop_html_editor-1.3.1/coop_html_editor/static/ckeditor.4.6.2/plugins/button/lang/tt.js
--rw-r--r--   0 lucjean    (501) staff       (20)      243 2019-08-29 13:07:42.000000 coop_html_editor-1.3.1/coop_html_editor/static/ckeditor.4.6.2/plugins/button/lang/ja.js
--rw-r--r--   0 lucjean    (501) staff       (20)      242 2019-08-29 13:07:42.000000 coop_html_editor-1.3.1/coop_html_editor/static/ckeditor.4.6.2/plugins/button/lang/he.js
--rw-r--r--   0 lucjean    (501) staff       (20)      250 2019-08-29 13:07:42.000000 coop_html_editor-1.3.1/coop_html_editor/static/ckeditor.4.6.2/plugins/button/lang/ug.js
--rw-r--r--   0 lucjean    (501) staff       (20)      248 2019-08-29 13:07:42.000000 coop_html_editor-1.3.1/coop_html_editor/static/ckeditor.4.6.2/plugins/button/lang/bg.js
--rw-r--r--   0 lucjean    (501) staff       (20)      241 2019-08-29 13:07:42.000000 coop_html_editor-1.3.1/coop_html_editor/static/ckeditor.4.6.2/plugins/button/lang/af.js
--rw-r--r--   0 lucjean    (501) staff       (20)      240 2019-08-29 13:07:42.000000 coop_html_editor-1.3.1/coop_html_editor/static/ckeditor.4.6.2/plugins/button/lang/id.js
--rw-r--r--   0 lucjean    (501) staff       (20)      242 2019-08-29 13:07:42.000000 coop_html_editor-1.3.1/coop_html_editor/static/ckeditor.4.6.2/plugins/button/lang/az.js
--rw-r--r--   0 lucjean    (501) staff       (20)      245 2019-08-29 13:07:42.000000 coop_html_editor-1.3.1/coop_html_editor/static/ckeditor.4.6.2/plugins/button/lang/ca.js
--rw-r--r--   0 lucjean    (501) staff       (20)      239 2019-08-29 13:07:42.000000 coop_html_editor-1.3.1/coop_html_editor/static/ckeditor.4.6.2/plugins/button/lang/nb.js
--rw-r--r--   0 lucjean    (501) staff       (20)      248 2019-08-29 13:07:42.000000 coop_html_editor-1.3.1/coop_html_editor/static/ckeditor.4.6.2/plugins/button/lang/zh-cn.js
--rw-r--r--   0 lucjean    (501) staff       (20)      248 2019-08-29 13:07:42.000000 coop_html_editor-1.3.1/coop_html_editor/static/ckeditor.4.6.2/plugins/button/lang/de-ch.js
--rw-r--r--   0 lucjean    (501) staff       (20)      248 2019-08-29 13:07:42.000000 coop_html_editor-1.3.1/coop_html_editor/static/ckeditor.4.6.2/plugins/button/lang/pt-br.js
--rw-r--r--   0 lucjean    (501) staff       (20)      245 2019-08-29 13:07:42.000000 coop_html_editor-1.3.1/coop_html_editor/static/ckeditor.4.6.2/plugins/button/lang/oc.js
--rw-r--r--   0 lucjean    (501) staff       (20)      239 2019-08-29 13:07:42.000000 coop_html_editor-1.3.1/coop_html_editor/static/ckeditor.4.6.2/plugins/button/lang/da.js
--rw-r--r--   0 lucjean    (501) staff       (20)      253 2019-08-29 13:07:42.000000 coop_html_editor-1.3.1/coop_html_editor/static/ckeditor.4.6.2/plugins/button/lang/fa.js
--rw-r--r--   0 lucjean    (501) staff       (20)      245 2019-08-29 13:07:42.000000 coop_html_editor-1.3.1/coop_html_editor/static/ckeditor.4.6.2/plugins/button/lang/de.js
--rw-r--r--   0 lucjean    (501) staff       (20)      242 2019-08-29 13:07:42.000000 coop_html_editor-1.3.1/coop_html_editor/static/ckeditor.4.6.2/plugins/button/lang/en.js
--rw-r--r--   0 lucjean    (501) staff       (20)      256 2019-08-29 13:07:42.000000 coop_html_editor-1.3.1/coop_html_editor/static/ckeditor.4.6.2/plugins/button/lang/ku.js
--rw-r--r--   0 lucjean    (501) staff       (20)      238 2019-08-29 13:07:42.000000 coop_html_editor-1.3.1/coop_html_editor/static/ckeditor.4.6.2/plugins/button/lang/sv.js
--rw-r--r--   0 lucjean    (501) staff       (20)      243 2019-08-29 13:07:42.000000 coop_html_editor-1.3.1/coop_html_editor/static/ckeditor.4.6.2/plugins/button/lang/zh.js
--rw-r--r--   0 lucjean    (501) staff       (20)      248 2019-08-29 13:07:42.000000 coop_html_editor-1.3.1/coop_html_editor/static/ckeditor.4.6.2/plugins/button/lang/uk.js
--rw-r--r--   0 lucjean    (501) staff       (20)      242 2019-08-29 13:07:42.000000 coop_html_editor-1.3.1/coop_html_editor/static/ckeditor.4.6.2/plugins/button/lang/cs.js
--rw-r--r--   0 lucjean    (501) staff       (20)      273 2019-08-29 13:07:42.000000 coop_html_editor-1.3.1/coop_html_editor/static/ckeditor.4.6.2/plugins/button/lang/km.js
--rw-r--r--   0 lucjean    (501) staff       (20)      247 2019-08-29 13:07:42.000000 coop_html_editor-1.3.1/coop_html_editor/static/ckeditor.4.6.2/plugins/button/lang/fr.js
--rw-r--r--   0 lucjean    (501) staff       (20)      246 2019-08-29 13:07:42.000000 coop_html_editor-1.3.1/coop_html_editor/static/ckeditor.4.6.2/plugins/button/lang/nl.js
--rw-r--r--   0 lucjean    (501) staff       (20)      245 2019-08-29 13:07:42.000000 coop_html_editor-1.3.1/coop_html_editor/static/ckeditor.4.6.2/plugins/button/lang/en-gb.js
--rw-r--r--   0 lucjean    (501) staff       (20)      246 2019-08-29 13:07:42.000000 coop_html_editor-1.3.1/coop_html_editor/static/ckeditor.4.6.2/plugins/button/lang/hu.js
--rw-r--r--   0 lucjean    (501) staff       (20)      244 2019-08-29 13:07:42.000000 coop_html_editor-1.3.1/coop_html_editor/static/ckeditor.4.6.2/plugins/button/lang/lt.js
--rw-r--r--   0 lucjean    (501) staff       (20)      242 2019-08-29 13:07:42.000000 coop_html_editor-1.3.1/coop_html_editor/static/ckeditor.4.6.2/plugins/button/lang/ar.js
--rw-r--r--   0 lucjean    (501) staff       (20)      242 2019-08-29 13:07:42.000000 coop_html_editor-1.3.1/coop_html_editor/static/ckeditor.4.6.2/plugins/button/lang/sk.js
--rw-r--r--   0 lucjean    (501) staff       (20)      245 2019-08-29 13:07:42.000000 coop_html_editor-1.3.1/coop_html_editor/static/ckeditor.4.6.2/plugins/button/lang/it.js
--rw-r--r--   0 lucjean    (501) staff       (20)      246 2019-08-29 13:07:42.000000 coop_html_editor-1.3.1/coop_html_editor/static/ckeditor.4.6.2/plugins/button/lang/es.js
--rw-r--r--   0 lucjean    (501) staff       (20)      243 2019-08-29 13:07:42.000000 coop_html_editor-1.3.1/coop_html_editor/static/ckeditor.4.6.2/plugins/button/lang/eo.js
--rw-r--r--   0 lucjean    (501) staff       (20)      242 2019-08-29 13:07:42.000000 coop_html_editor-1.3.1/coop_html_editor/static/ckeditor.4.6.2/plugins/button/lang/ro.js
--rw-r--r--   0 lucjean    (501) staff       (20)      244 2019-08-29 13:07:42.000000 coop_html_editor-1.3.1/coop_html_editor/static/ckeditor.4.6.2/plugins/button/lang/tr.js
--rw-r--r--   0 lucjean    (501) staff       (20)    11829 2019-08-29 13:07:42.000000 coop_html_editor-1.3.1/coop_html_editor/static/ckeditor.4.6.2/plugins/button/plugin.js
--rw-r--r--   0 lucjean    (501) staff       (20)     6057 2019-08-29 13:07:42.000000 coop_html_editor-1.3.1/coop_html_editor/static/ckeditor.4.6.2/plugins/icons.png
-drwxr-xr-x   0 lucjean    (501) staff       (20)        0 2019-08-30 10:39:59.000000 coop_html_editor-1.3.1/coop_html_editor/static/ckeditor.4.6.2/plugins/lineutils/
-drwxr-xr-x   0 lucjean    (501) staff       (20)        0 2019-08-30 10:39:59.000000 coop_html_editor-1.3.1/coop_html_editor/static/ckeditor.4.6.2/plugins/lineutils/dev/
--rw-r--r--   0 lucjean    (501) staff       (20)     9083 2019-08-29 13:07:42.000000 coop_html_editor-1.3.1/coop_html_editor/static/ckeditor.4.6.2/plugins/lineutils/dev/magicfinger.html
--rw-r--r--   0 lucjean    (501) staff       (20)     7933 2019-08-29 13:07:42.000000 coop_html_editor-1.3.1/coop_html_editor/static/ckeditor.4.6.2/plugins/lineutils/dev/dnd.html
--rw-r--r--   0 lucjean    (501) staff       (20)    28852 2019-08-29 13:07:42.000000 coop_html_editor-1.3.1/coop_html_editor/static/ckeditor.4.6.2/plugins/lineutils/plugin.js
-drwxr-xr-x   0 lucjean    (501) staff       (20)        0 2019-08-30 10:39:35.000000 coop_html_editor-1.3.1/coop_html_editor/static/ckeditor.4.6.2/plugins/link/
-drwxr-xr-x   0 lucjean    (501) staff       (20)        0 2019-08-30 10:39:59.000000 coop_html_editor-1.3.1/coop_html_editor/static/ckeditor.4.6.2/plugins/link/images/
-drwxr-xr-x   0 lucjean    (501) staff       (20)        0 2019-08-30 10:39:59.000000 coop_html_editor-1.3.1/coop_html_editor/static/ckeditor.4.6.2/plugins/link/images/hidpi/
--rw-r--r--   0 lucjean    (501) staff       (20)     1109 2019-08-29 13:07:42.000000 coop_html_editor-1.3.1/coop_html_editor/static/ckeditor.4.6.2/plugins/link/images/hidpi/anchor.png
--rw-r--r--   0 lucjean    (501) staff       (20)      752 2019-08-29 13:07:42.000000 coop_html_editor-1.3.1/coop_html_editor/static/ckeditor.4.6.2/plugins/link/images/anchor.png
-drwxr-xr-x   0 lucjean    (501) staff       (20)        0 2019-08-30 10:39:59.000000 coop_html_editor-1.3.1/coop_html_editor/static/ckeditor.4.6.2/plugins/link/dialogs/
--rw-r--r--   0 lucjean    (501) staff       (20)    12093 2019-08-29 13:07:42.000000 coop_html_editor-1.3.1/coop_html_editor/static/ckeditor.4.6.2/plugins/link/dialogs/link.js
--rw-r--r--   0 lucjean    (501) staff       (20)     1629 2019-08-29 13:07:42.000000 coop_html_editor-1.3.1/coop_html_editor/static/ckeditor.4.6.2/plugins/link/dialogs/anchor.js
-drwxr-xr-x   0 lucjean    (501) staff       (20)        0 2019-08-30 10:39:35.000000 coop_html_editor-1.3.1/coop_html_editor/static/ckeditor.4.6.2/plugins/table/
-drwxr-xr-x   0 lucjean    (501) staff       (20)        0 2019-08-30 10:40:01.000000 coop_html_editor-1.3.1/coop_html_editor/static/ckeditor.4.6.2/plugins/table/dialogs/
--rw-r--r--   0 lucjean    (501) staff       (20)     8807 2019-08-29 13:07:43.000000 coop_html_editor-1.3.1/coop_html_editor/static/ckeditor.4.6.2/plugins/table/dialogs/table.js
-drwxr-xr-x   0 lucjean    (501) staff       (20)        0 2019-08-30 10:40:03.000000 coop_html_editor-1.3.1/coop_html_editor/static/ckeditor.4.6.2/plugins/widgetselection/
--rw-r--r--   0 lucjean    (501) staff       (20)    11474 2019-08-29 13:07:45.000000 coop_html_editor-1.3.1/coop_html_editor/static/ckeditor.4.6.2/plugins/widgetselection/plugin.js
--rw-r--r--   0 lucjean    (501) staff       (20)    20877 2019-08-29 13:07:42.000000 coop_html_editor-1.3.1/coop_html_editor/static/ckeditor.4.6.2/plugins/icons_hidpi.png
-drwxr-xr-x   0 lucjean    (501) staff       (20)        0 2019-08-30 10:39:35.000000 coop_html_editor-1.3.1/coop_html_editor/static/ckeditor.4.6.2/plugins/a11yhelp/
-drwxr-xr-x   0 lucjean    (501) staff       (20)        0 2019-08-30 10:39:55.000000 coop_html_editor-1.3.1/coop_html_editor/static/ckeditor.4.6.2/plugins/a11yhelp/dialogs/
--rw-r--r--   0 lucjean    (501) staff       (20)     2879 2019-08-29 13:07:41.000000 coop_html_editor-1.3.1/coop_html_editor/static/ckeditor.4.6.2/plugins/a11yhelp/dialogs/a11yhelp.js
-drwxr-xr-x   0 lucjean    (501) staff       (20)        0 2019-08-30 10:39:55.000000 coop_html_editor-1.3.1/coop_html_editor/static/ckeditor.4.6.2/plugins/a11yhelp/dialogs/lang/
--rw-r--r--   0 lucjean    (501) staff       (20)     3862 2019-08-29 13:07:41.000000 coop_html_editor-1.3.1/coop_html_editor/static/ckeditor.4.6.2/plugins/a11yhelp/dialogs/lang/sr-latn.js
--rw-r--r--   0 lucjean    (501) staff       (20)     4409 2019-08-29 13:07:41.000000 coop_html_editor-1.3.1/coop_html_editor/static/ckeditor.4.6.2/plugins/a11yhelp/dialogs/lang/pt.js
--rw-r--r--   0 lucjean    (501) staff       (20)     5145 2019-08-29 13:07:42.000000 coop_html_editor-1.3.1/coop_html_editor/static/ckeditor.4.6.2/plugins/a11yhelp/dialogs/lang/vi.js
--rw-r--r--   0 lucjean    (501) staff       (20)     4580 2019-08-29 13:07:41.000000 coop_html_editor-1.3.1/coop_html_editor/static/ckeditor.4.6.2/plugins/a11yhelp/dialogs/lang/lv.js
--rw-r--r--   0 lucjean    (501) staff       (20)     4370 2019-08-29 13:07:41.000000 coop_html_editor-1.3.1/coop_html_editor/static/ckeditor.4.6.2/plugins/a11yhelp/dialogs/lang/gl.js
--rw-r--r--   0 lucjean    (501) staff       (20)     4840 2019-08-29 13:07:41.000000 coop_html_editor-1.3.1/coop_html_editor/static/ckeditor.4.6.2/plugins/a11yhelp/dialogs/lang/pl.js
--rw-r--r--   0 lucjean    (501) staff       (20)     3865 2019-08-29 13:07:41.000000 coop_html_editor-1.3.1/coop_html_editor/static/ckeditor.4.6.2/plugins/a11yhelp/dialogs/lang/mn.js
--rw-r--r--   0 lucjean    (501) staff       (20)     6879 2019-08-29 13:07:41.000000 coop_html_editor-1.3.1/coop_html_editor/static/ckeditor.4.6.2/plugins/a11yhelp/dialogs/lang/el.js
--rw-r--r--   0 lucjean    (501) staff       (20)     3867 2019-08-29 13:07:41.000000 coop_html_editor-1.3.1/coop_html_editor/static/ckeditor.4.6.2/plugins/a11yhelp/dialogs/lang/et.js
--rw-r--r--   0 lucjean    (501) staff       (20)     4292 2019-08-29 13:07:41.000000 coop_html_editor-1.3.1/coop_html_editor/static/ckeditor.4.6.2/plugins/a11yhelp/dialogs/lang/sl.js
--rw-r--r--   0 lucjean    (501) staff       (20)     5469 2019-08-29 13:07:41.000000 coop_html_editor-1.3.1/coop_html_editor/static/ckeditor.4.6.2/plugins/a11yhelp/dialogs/lang/ko.js
--rw-r--r--   0 lucjean    (501) staff       (20)     4041 2019-08-29 13:07:41.000000 coop_html_editor-1.3.1/coop_html_editor/static/ckeditor.4.6.2/plugins/a11yhelp/dialogs/lang/hr.js
--rw-r--r--   0 lucjean    (501) staff       (20)     4504 2019-08-29 13:07:41.000000 coop_html_editor-1.3.1/coop_html_editor/static/ckeditor.4.6.2/plugins/a11yhelp/dialogs/lang/fi.js
--rw-r--r--   0 lucjean    (501) staff       (20)     4236 2019-08-29 13:07:41.000000 coop_html_editor-1.3.1/coop_html_editor/static/ckeditor.4.6.2/plugins/a11yhelp/dialogs/lang/th.js
--rw-r--r--   0 lucjean    (501) staff       (20)     6477 2019-08-29 13:07:41.000000 coop_html_editor-1.3.1/coop_html_editor/static/ckeditor.4.6.2/plugins/a11yhelp/dialogs/lang/ru.js
--rw-r--r--   0 lucjean    (501) staff       (20)     4360 2019-08-29 13:07:41.000000 coop_html_editor-1.3.1/coop_html_editor/static/ckeditor.4.6.2/plugins/a11yhelp/dialogs/lang/eu.js
--rw-r--r--   0 lucjean    (501) staff       (20)     4250 2019-08-29 13:07:41.000000 coop_html_editor-1.3.1/coop_html_editor/static/ckeditor.4.6.2/plugins/a11yhelp/dialogs/lang/mk.js
--rw-r--r--   0 lucjean    (501) staff       (20)     4169 2019-08-29 13:07:41.000000 coop_html_editor-1.3.1/coop_html_editor/static/ckeditor.4.6.2/plugins/a11yhelp/dialogs/lang/no.js
--rw-r--r--   0 lucjean    (501) staff       (20)     3938 2019-08-29 13:07:41.000000 coop_html_editor-1.3.1/coop_html_editor/static/ckeditor.4.6.2/plugins/a11yhelp/dialogs/lang/sq.js
--rw-r--r--   0 lucjean    (501) staff       (20)     4068 2019-08-29 13:07:41.000000 coop_html_editor-1.3.1/coop_html_editor/static/ckeditor.4.6.2/plugins/a11yhelp/dialogs/lang/gu.js
--rw-r--r--   0 lucjean    (501) staff       (20)     5890 2019-08-29 13:07:41.000000 coop_html_editor-1.3.1/coop_html_editor/static/ckeditor.4.6.2/plugins/a11yhelp/dialogs/lang/si.js
--rw-r--r--   0 lucjean    (501) staff       (20)     4177 2019-08-29 13:07:42.000000 coop_html_editor-1.3.1/coop_html_editor/static/ckeditor.4.6.2/plugins/a11yhelp/dialogs/lang/tt.js
--rw-r--r--   0 lucjean    (501) staff       (20)     4954 2019-08-29 13:07:41.000000 coop_html_editor-1.3.1/coop_html_editor/static/ckeditor.4.6.2/plugins/a11yhelp/dialogs/lang/ja.js
--rw-r--r--   0 lucjean    (501) staff       (20)     4699 2019-08-29 13:07:41.000000 coop_html_editor-1.3.1/coop_html_editor/static/ckeditor.4.6.2/plugins/a11yhelp/dialogs/lang/he.js
--rw-r--r--   0 lucjean    (501) staff       (20)     6793 2019-08-29 13:07:42.000000 coop_html_editor-1.3.1/coop_html_editor/static/ckeditor.4.6.2/plugins/a11yhelp/dialogs/lang/ug.js
--rw-r--r--   0 lucjean    (501) staff       (20)     3859 2019-08-29 13:07:41.000000 coop_html_editor-1.3.1/coop_html_editor/static/ckeditor.4.6.2/plugins/a11yhelp/dialogs/lang/bg.js
--rw-r--r--   0 lucjean    (501) staff       (20)     3901 2019-08-29 13:07:41.000000 coop_html_editor-1.3.1/coop_html_editor/static/ckeditor.4.6.2/plugins/a11yhelp/dialogs/lang/af.js
--rw-r--r--   0 lucjean    (501) staff       (20)     3909 2019-08-29 13:07:41.000000 coop_html_editor-1.3.1/coop_html_editor/static/ckeditor.4.6.2/plugins/a11yhelp/dialogs/lang/id.js
--rw-r--r--   0 lucjean    (501) staff       (20)     4194 2019-08-29 13:07:41.000000 coop_html_editor-1.3.1/coop_html_editor/static/ckeditor.4.6.2/plugins/a11yhelp/dialogs/lang/az.js
--rw-r--r--   0 lucjean    (501) staff       (20)     4657 2019-08-29 13:07:41.000000 coop_html_editor-1.3.1/coop_html_editor/static/ckeditor.4.6.2/plugins/a11yhelp/dialogs/lang/ca.js
--rw-r--r--   0 lucjean    (501) staff       (20)     4134 2019-08-29 13:07:41.000000 coop_html_editor-1.3.1/coop_html_editor/static/ckeditor.4.6.2/plugins/a11yhelp/dialogs/lang/cy.js
--rw-r--r--   0 lucjean    (501) staff       (20)      869 2019-08-29 13:07:41.000000 coop_html_editor-1.3.1/coop_html_editor/static/ckeditor.4.6.2/plugins/a11yhelp/dialogs/lang/_translationstatus.txt
--rw-r--r--   0 lucjean    (501) staff       (20)     4324 2019-08-29 13:07:41.000000 coop_html_editor-1.3.1/coop_html_editor/static/ckeditor.4.6.2/plugins/a11yhelp/dialogs/lang/nb.js
--rw-r--r--   0 lucjean    (501) staff       (20)     4022 2019-08-29 13:07:42.000000 coop_html_editor-1.3.1/coop_html_editor/static/ckeditor.4.6.2/plugins/a11yhelp/dialogs/lang/zh-cn.js
--rw-r--r--   0 lucjean    (501) staff       (20)     4447 2019-08-29 13:07:41.000000 coop_html_editor-1.3.1/coop_html_editor/static/ckeditor.4.6.2/plugins/a11yhelp/dialogs/lang/de-ch.js
--rw-r--r--   0 lucjean    (501) staff       (20)     4543 2019-08-29 13:07:41.000000 coop_html_editor-1.3.1/coop_html_editor/static/ckeditor.4.6.2/plugins/a11yhelp/dialogs/lang/pt-br.js
--rw-r--r--   0 lucjean    (501) staff       (20)     4968 2019-08-29 13:07:41.000000 coop_html_editor-1.3.1/coop_html_editor/static/ckeditor.4.6.2/plugins/a11yhelp/dialogs/lang/oc.js
--rw-r--r--   0 lucjean    (501) staff       (20)     4030 2019-08-29 13:07:41.000000 coop_html_editor-1.3.1/coop_html_editor/static/ckeditor.4.6.2/plugins/a11yhelp/dialogs/lang/da.js
--rw-r--r--   0 lucjean    (501) staff       (20)     5715 2019-08-29 13:07:41.000000 coop_html_editor-1.3.1/coop_html_editor/static/ckeditor.4.6.2/plugins/a11yhelp/dialogs/lang/fa.js
--rw-r--r--   0 lucjean    (501) staff       (20)     4444 2019-08-29 13:07:41.000000 coop_html_editor-1.3.1/coop_html_editor/static/ckeditor.4.6.2/plugins/a11yhelp/dialogs/lang/de.js
--rw-r--r--   0 lucjean    (501) staff       (20)     3858 2019-08-29 13:07:41.000000 coop_html_editor-1.3.1/coop_html_editor/static/ckeditor.4.6.2/plugins/a11yhelp/dialogs/lang/en.js
--rw-r--r--   0 lucjean    (501) staff       (20)     5364 2019-08-29 13:07:41.000000 coop_html_editor-1.3.1/coop_html_editor/static/ckeditor.4.6.2/plugins/a11yhelp/dialogs/lang/ku.js
--rw-r--r--   0 lucjean    (501) staff       (20)     4235 2019-08-29 13:07:41.000000 coop_html_editor-1.3.1/coop_html_editor/static/ckeditor.4.6.2/plugins/a11yhelp/dialogs/lang/sv.js
--rw-r--r--   0 lucjean    (501) staff       (20)     4061 2019-08-29 13:07:42.000000 coop_html_editor-1.3.1/coop_html_editor/static/ckeditor.4.6.2/plugins/a11yhelp/dialogs/lang/zh.js
--rw-r--r--   0 lucjean    (501) staff       (20)     3872 2019-08-29 13:07:41.000000 coop_html_editor-1.3.1/coop_html_editor/static/ckeditor.4.6.2/plugins/a11yhelp/dialogs/lang/hi.js
--rw-r--r--   0 lucjean    (501) staff       (20)     6737 2019-08-29 13:07:42.000000 coop_html_editor-1.3.1/coop_html_editor/static/ckeditor.4.6.2/plugins/a11yhelp/dialogs/lang/uk.js
--rw-r--r--   0 lucjean    (501) staff       (20)     4714 2019-08-29 13:07:41.000000 coop_html_editor-1.3.1/coop_html_editor/static/ckeditor.4.6.2/plugins/a11yhelp/dialogs/lang/cs.js
--rw-r--r--   0 lucjean    (501) staff       (20)     4876 2019-08-29 13:07:41.000000 coop_html_editor-1.3.1/coop_html_editor/static/ckeditor.4.6.2/plugins/a11yhelp/dialogs/lang/km.js
--rw-r--r--   0 lucjean    (501) staff       (20)     5155 2019-08-29 13:07:41.000000 coop_html_editor-1.3.1/coop_html_editor/static/ckeditor.4.6.2/plugins/a11yhelp/dialogs/lang/fr.js
--rw-r--r--   0 lucjean    (501) staff       (20)     4393 2019-08-29 13:07:41.000000 coop_html_editor-1.3.1/coop_html_editor/static/ckeditor.4.6.2/plugins/a11yhelp/dialogs/lang/nl.js
--rw-r--r--   0 lucjean    (501) staff       (20)     4666 2019-08-29 13:07:41.000000 coop_html_editor-1.3.1/coop_html_editor/static/ckeditor.4.6.2/plugins/a11yhelp/dialogs/lang/fr-ca.js
--rw-r--r--   0 lucjean    (501) staff       (20)     3861 2019-08-29 13:07:41.000000 coop_html_editor-1.3.1/coop_html_editor/static/ckeditor.4.6.2/plugins/a11yhelp/dialogs/lang/en-gb.js
--rw-r--r--   0 lucjean    (501) staff       (20)     3861 2019-08-29 13:07:41.000000 coop_html_editor-1.3.1/coop_html_editor/static/ckeditor.4.6.2/plugins/a11yhelp/dialogs/lang/sr.js
--rw-r--r--   0 lucjean    (501) staff       (20)     4604 2019-08-29 13:07:41.000000 coop_html_editor-1.3.1/coop_html_editor/static/ckeditor.4.6.2/plugins/a11yhelp/dialogs/lang/hu.js
--rw-r--r--   0 lucjean    (501) staff       (20)     3867 2019-08-29 13:07:41.000000 coop_html_editor-1.3.1/coop_html_editor/static/ckeditor.4.6.2/plugins/a11yhelp/dialogs/lang/lt.js
--rw-r--r--   0 lucjean    (501) staff       (20)     3860 2019-08-29 13:07:41.000000 coop_html_editor-1.3.1/coop_html_editor/static/ckeditor.4.6.2/plugins/a11yhelp/dialogs/lang/fo.js
--rw-r--r--   0 lucjean    (501) staff       (20)     3875 2019-08-29 13:07:41.000000 coop_html_editor-1.3.1/coop_html_editor/static/ckeditor.4.6.2/plugins/a11yhelp/dialogs/lang/ar.js
--rw-r--r--   0 lucjean    (501) staff       (20)     4576 2019-08-29 13:07:41.000000 coop_html_editor-1.3.1/coop_html_editor/static/ckeditor.4.6.2/plugins/a11yhelp/dialogs/lang/sk.js
--rw-r--r--   0 lucjean    (501) staff       (20)     4805 2019-08-29 13:07:41.000000 coop_html_editor-1.3.1/coop_html_editor/static/ckeditor.4.6.2/plugins/a11yhelp/dialogs/lang/it.js
--rw-r--r--   0 lucjean    (501) staff       (20)     4669 2019-08-29 13:07:41.000000 coop_html_editor-1.3.1/coop_html_editor/static/ckeditor.4.6.2/plugins/a11yhelp/dialogs/lang/es.js
--rw-r--r--   0 lucjean    (501) staff       (20)     4660 2019-08-29 13:07:41.000000 coop_html_editor-1.3.1/coop_html_editor/static/ckeditor.4.6.2/plugins/a11yhelp/dialogs/lang/eo.js
--rw-r--r--   0 lucjean    (501) staff       (20)     4139 2019-08-29 13:07:41.000000 coop_html_editor-1.3.1/coop_html_editor/static/ckeditor.4.6.2/plugins/a11yhelp/dialogs/lang/ro.js
--rw-r--r--   0 lucjean    (501) staff       (20)     4436 2019-08-29 13:07:42.000000 coop_html_editor-1.3.1/coop_html_editor/static/ckeditor.4.6.2/plugins/a11yhelp/dialogs/lang/tr.js
-drwxr-xr-x   0 lucjean    (501) staff       (20)        0 2019-08-30 10:40:00.000000 coop_html_editor-1.3.1/coop_html_editor/static/ckeditor.4.6.2/plugins/sourcedialog/
-drwxr-xr-x   0 lucjean    (501) staff       (20)        0 2019-08-30 10:40:01.000000 coop_html_editor-1.3.1/coop_html_editor/static/ckeditor.4.6.2/plugins/sourcedialog/lang/
--rw-r--r--   0 lucjean    (501) staff       (20)      237 2019-08-29 13:07:42.000000 coop_html_editor-1.3.1/coop_html_editor/static/ckeditor.4.6.2/plugins/sourcedialog/lang/sr-latn.js
--rw-r--r--   0 lucjean    (501) staff       (20)      234 2019-08-29 13:07:42.000000 coop_html_editor-1.3.1/coop_html_editor/static/ckeditor.4.6.2/plugins/sourcedialog/lang/pt.js
--rw-r--r--   0 lucjean    (501) staff       (20)      240 2019-08-29 13:07:42.000000 coop_html_editor-1.3.1/coop_html_editor/static/ckeditor.4.6.2/plugins/sourcedialog/lang/vi.js
--rw-r--r--   0 lucjean    (501) staff       (20)      242 2019-08-29 13:07:42.000000 coop_html_editor-1.3.1/coop_html_editor/static/ckeditor.4.6.2/plugins/sourcedialog/lang/lv.js
--rw-r--r--   0 lucjean    (501) staff       (20)      234 2019-08-29 13:07:42.000000 coop_html_editor-1.3.1/coop_html_editor/static/ckeditor.4.6.2/plugins/sourcedialog/lang/gl.js
--rw-r--r--   0 lucjean    (501) staff       (20)      262 2019-08-29 13:07:42.000000 coop_html_editor-1.3.1/coop_html_editor/static/ckeditor.4.6.2/plugins/sourcedialog/lang/pl.js
--rw-r--r--   0 lucjean    (501) staff       (20)      236 2019-08-29 13:07:42.000000 coop_html_editor-1.3.1/coop_html_editor/static/ckeditor.4.6.2/plugins/sourcedialog/lang/mn.js
--rw-r--r--   0 lucjean    (501) staff       (20)      239 2019-08-29 13:07:42.000000 coop_html_editor-1.3.1/coop_html_editor/static/ckeditor.4.6.2/plugins/sourcedialog/lang/en-ca.js
--rw-r--r--   0 lucjean    (501) staff       (20)      252 2019-08-29 13:07:42.000000 coop_html_editor-1.3.1/coop_html_editor/static/ckeditor.4.6.2/plugins/sourcedialog/lang/el.js
--rw-r--r--   0 lucjean    (501) staff       (20)      244 2019-08-29 13:07:42.000000 coop_html_editor-1.3.1/coop_html_editor/static/ckeditor.4.6.2/plugins/sourcedialog/lang/et.js
--rw-r--r--   0 lucjean    (501) staff       (20)      236 2019-08-29 13:07:42.000000 coop_html_editor-1.3.1/coop_html_editor/static/ckeditor.4.6.2/plugins/sourcedialog/lang/is.js
--rw-r--r--   0 lucjean    (501) staff       (20)      248 2019-08-29 13:07:42.000000 coop_html_editor-1.3.1/coop_html_editor/static/ckeditor.4.6.2/plugins/sourcedialog/lang/sl.js
--rw-r--r--   0 lucjean    (501) staff       (20)      236 2019-08-29 13:07:42.000000 coop_html_editor-1.3.1/coop_html_editor/static/ckeditor.4.6.2/plugins/sourcedialog/lang/ko.js
--rw-r--r--   0 lucjean    (501) staff       (20)      232 2019-08-29 13:07:42.000000 coop_html_editor-1.3.1/coop_html_editor/static/ckeditor.4.6.2/plugins/sourcedialog/lang/hr.js
--rw-r--r--   0 lucjean    (501) staff       (20)      236 2019-08-29 13:07:42.000000 coop_html_editor-1.3.1/coop_html_editor/static/ckeditor.4.6.2/plugins/sourcedialog/lang/ms.js
--rw-r--r--   0 lucjean    (501) staff       (20)      234 2019-08-29 13:07:42.000000 coop_html_editor-1.3.1/coop_html_editor/static/ckeditor.4.6.2/plugins/sourcedialog/lang/fi.js
--rw-r--r--   0 lucjean    (501) staff       (20)      270 2019-08-29 13:07:42.000000 coop_html_editor-1.3.1/coop_html_editor/static/ckeditor.4.6.2/plugins/sourcedialog/lang/th.js
--rw-r--r--   0 lucjean    (501) staff       (20)      256 2019-08-29 13:07:42.000000 coop_html_editor-1.3.1/coop_html_editor/static/ckeditor.4.6.2/plugins/sourcedialog/lang/ru.js
--rw-r--r--   0 lucjean    (501) staff       (20)      242 2019-08-29 13:07:42.000000 coop_html_editor-1.3.1/coop_html_editor/static/ckeditor.4.6.2/plugins/sourcedialog/lang/eu.js
--rw-r--r--   0 lucjean    (501) staff       (20)      234 2019-08-29 13:07:42.000000 coop_html_editor-1.3.1/coop_html_editor/static/ckeditor.4.6.2/plugins/sourcedialog/lang/no.js
--rw-r--r--   0 lucjean    (501) staff       (20)      236 2019-08-29 13:07:42.000000 coop_html_editor-1.3.1/coop_html_editor/static/ckeditor.4.6.2/plugins/sourcedialog/lang/sq.js
--rw-r--r--   0 lucjean    (501) staff       (20)      356 2019-08-29 13:07:42.000000 coop_html_editor-1.3.1/coop_html_editor/static/ckeditor.4.6.2/plugins/sourcedialog/lang/gu.js
--rw-r--r--   0 lucjean    (501) staff       (20)      278 2019-08-29 13:07:42.000000 coop_html_editor-1.3.1/coop_html_editor/static/ckeditor.4.6.2/plugins/sourcedialog/lang/si.js
--rw-r--r--   0 lucjean    (501) staff       (20)      252 2019-08-29 13:07:42.000000 coop_html_editor-1.3.1/coop_html_editor/static/ckeditor.4.6.2/plugins/sourcedialog/lang/tt.js
--rw-r--r--   0 lucjean    (501) staff       (20)      242 2019-08-29 13:07:42.000000 coop_html_editor-1.3.1/coop_html_editor/static/ckeditor.4.6.2/plugins/sourcedialog/lang/ja.js
--rw-r--r--   0 lucjean    (501) staff       (20)      260 2019-08-29 13:07:42.000000 coop_html_editor-1.3.1/coop_html_editor/static/ckeditor.4.6.2/plugins/sourcedialog/lang/ka.js
--rw-r--r--   0 lucjean    (501) staff       (20)      240 2019-08-29 13:07:42.000000 coop_html_editor-1.3.1/coop_html_editor/static/ckeditor.4.6.2/plugins/sourcedialog/lang/he.js
--rw-r--r--   0 lucjean    (501) staff       (20)      244 2019-08-29 13:07:42.000000 coop_html_editor-1.3.1/coop_html_editor/static/ckeditor.4.6.2/plugins/sourcedialog/lang/ug.js
--rw-r--r--   0 lucjean    (501) staff       (20)      256 2019-08-29 13:07:42.000000 coop_html_editor-1.3.1/coop_html_editor/static/ckeditor.4.6.2/plugins/sourcedialog/lang/bg.js
--rw-r--r--   0 lucjean    (501) staff       (20)      232 2019-08-29 13:07:42.000000 coop_html_editor-1.3.1/coop_html_editor/static/ckeditor.4.6.2/plugins/sourcedialog/lang/af.js
--rw-r--r--   0 lucjean    (501) staff       (20)      236 2019-08-29 13:07:42.000000 coop_html_editor-1.3.1/coop_html_editor/static/ckeditor.4.6.2/plugins/sourcedialog/lang/id.js
--rw-r--r--   0 lucjean    (501) staff       (20)      238 2019-08-29 13:07:42.000000 coop_html_editor-1.3.1/coop_html_editor/static/ckeditor.4.6.2/plugins/sourcedialog/lang/az.js
--rw-r--r--   0 lucjean    (501) staff       (20)      239 2019-08-29 13:07:42.000000 coop_html_editor-1.3.1/coop_html_editor/static/ckeditor.4.6.2/plugins/sourcedialog/lang/en-au.js
--rw-r--r--   0 lucjean    (501) staff       (20)      242 2019-08-29 13:07:42.000000 coop_html_editor-1.3.1/coop_html_editor/static/ckeditor.4.6.2/plugins/sourcedialog/lang/ca.js
--rw-r--r--   0 lucjean    (501) staff       (20)      232 2019-08-29 13:07:42.000000 coop_html_editor-1.3.1/coop_html_editor/static/ckeditor.4.6.2/plugins/sourcedialog/lang/cy.js
--rw-r--r--   0 lucjean    (501) staff       (20)      234 2019-08-29 13:07:42.000000 coop_html_editor-1.3.1/coop_html_editor/static/ckeditor.4.6.2/plugins/sourcedialog/lang/nb.js
--rw-r--r--   0 lucjean    (501) staff       (20)      239 2019-08-29 13:07:42.000000 coop_html_editor-1.3.1/coop_html_editor/static/ckeditor.4.6.2/plugins/sourcedialog/lang/zh-cn.js
--rw-r--r--   0 lucjean    (501) staff       (20)      245 2019-08-29 13:07:42.000000 coop_html_editor-1.3.1/coop_html_editor/static/ckeditor.4.6.2/plugins/sourcedialog/lang/de-ch.js
--rw-r--r--   0 lucjean    (501) staff       (20)      253 2019-08-29 13:07:42.000000 coop_html_editor-1.3.1/coop_html_editor/static/ckeditor.4.6.2/plugins/sourcedialog/lang/pt-br.js
--rw-r--r--   0 lucjean    (501) staff       (20)      232 2019-08-29 13:07:42.000000 coop_html_editor-1.3.1/coop_html_editor/static/ckeditor.4.6.2/plugins/sourcedialog/lang/oc.js
--rw-r--r--   0 lucjean    (501) staff       (20)      234 2019-08-29 13:07:42.000000 coop_html_editor-1.3.1/coop_html_editor/static/ckeditor.4.6.2/plugins/sourcedialog/lang/da.js
--rw-r--r--   0 lucjean    (501) staff       (20)      240 2019-08-29 13:07:42.000000 coop_html_editor-1.3.1/coop_html_editor/static/ckeditor.4.6.2/plugins/sourcedialog/lang/fa.js
--rw-r--r--   0 lucjean    (501) staff       (20)      242 2019-08-29 13:07:42.000000 coop_html_editor-1.3.1/coop_html_editor/static/ckeditor.4.6.2/plugins/sourcedialog/lang/de.js
--rw-r--r--   0 lucjean    (501) staff       (20)      236 2019-08-29 13:07:42.000000 coop_html_editor-1.3.1/coop_html_editor/static/ckeditor.4.6.2/plugins/sourcedialog/lang/en.js
--rw-r--r--   0 lucjean    (501) staff       (20)      242 2019-08-29 13:07:42.000000 coop_html_editor-1.3.1/coop_html_editor/static/ckeditor.4.6.2/plugins/sourcedialog/lang/bs.js
--rw-r--r--   0 lucjean    (501) staff       (20)      252 2019-08-29 13:07:42.000000 coop_html_editor-1.3.1/coop_html_editor/static/ckeditor.4.6.2/plugins/sourcedialog/lang/ku.js
--rw-r--r--   0 lucjean    (501) staff       (20)      236 2019-08-29 13:07:42.000000 coop_html_editor-1.3.1/coop_html_editor/static/ckeditor.4.6.2/plugins/sourcedialog/lang/sv.js
--rw-r--r--   0 lucjean    (501) staff       (20)      242 2019-08-29 13:07:42.000000 coop_html_editor-1.3.1/coop_html_editor/static/ckeditor.4.6.2/plugins/sourcedialog/lang/zh.js
--rw-r--r--   0 lucjean    (501) staff       (20)      254 2019-08-29 13:07:42.000000 coop_html_editor-1.3.1/coop_html_editor/static/ckeditor.4.6.2/plugins/sourcedialog/lang/hi.js
--rw-r--r--   0 lucjean    (501) staff       (20)      252 2019-08-29 13:07:42.000000 coop_html_editor-1.3.1/coop_html_editor/static/ckeditor.4.6.2/plugins/sourcedialog/lang/uk.js
--rw-r--r--   0 lucjean    (501) staff       (20)      234 2019-08-29 13:07:42.000000 coop_html_editor-1.3.1/coop_html_editor/static/ckeditor.4.6.2/plugins/sourcedialog/lang/cs.js
--rw-r--r--   0 lucjean    (501) staff       (20)      278 2019-08-29 13:07:42.000000 coop_html_editor-1.3.1/coop_html_editor/static/ckeditor.4.6.2/plugins/sourcedialog/lang/km.js
--rw-r--r--   0 lucjean    (501) staff       (20)      236 2019-08-29 13:07:42.000000 coop_html_editor-1.3.1/coop_html_editor/static/ckeditor.4.6.2/plugins/sourcedialog/lang/fr.js
--rw-r--r--   0 lucjean    (501) staff       (20)      240 2019-08-29 13:07:42.000000 coop_html_editor-1.3.1/coop_html_editor/static/ckeditor.4.6.2/plugins/sourcedialog/lang/nl.js
--rw-r--r--   0 lucjean    (501) staff       (20)      239 2019-08-29 13:07:42.000000 coop_html_editor-1.3.1/coop_html_editor/static/ckeditor.4.6.2/plugins/sourcedialog/lang/fr-ca.js
--rw-r--r--   0 lucjean    (501) staff       (20)      239 2019-08-29 13:07:42.000000 coop_html_editor-1.3.1/coop_html_editor/static/ckeditor.4.6.2/plugins/sourcedialog/lang/en-gb.js
--rw-r--r--   0 lucjean    (501) staff       (20)      234 2019-08-29 13:07:42.000000 coop_html_editor-1.3.1/coop_html_editor/static/ckeditor.4.6.2/plugins/sourcedialog/lang/sr.js
--rw-r--r--   0 lucjean    (501) staff       (20)      246 2019-08-29 13:07:42.000000 coop_html_editor-1.3.1/coop_html_editor/static/ckeditor.4.6.2/plugins/sourcedialog/lang/hu.js
--rw-r--r--   0 lucjean    (501) staff       (20)      242 2019-08-29 13:07:42.000000 coop_html_editor-1.3.1/coop_html_editor/static/ckeditor.4.6.2/plugins/sourcedialog/lang/lt.js
--rw-r--r--   0 lucjean    (501) staff       (20)      234 2019-08-29 13:07:42.000000 coop_html_editor-1.3.1/coop_html_editor/static/ckeditor.4.6.2/plugins/sourcedialog/lang/fo.js
--rw-r--r--   0 lucjean    (501) staff       (20)      248 2019-08-29 13:07:42.000000 coop_html_editor-1.3.1/coop_html_editor/static/ckeditor.4.6.2/plugins/sourcedialog/lang/ar.js
--rw-r--r--   0 lucjean    (501) staff       (20)      234 2019-08-29 13:07:42.000000 coop_html_editor-1.3.1/coop_html_editor/static/ckeditor.4.6.2/plugins/sourcedialog/lang/sk.js
--rw-r--r--   0 lucjean    (501) staff       (20)      240 2019-08-29 13:07:42.000000 coop_html_editor-1.3.1/coop_html_editor/static/ckeditor.4.6.2/plugins/sourcedialog/lang/it.js
--rw-r--r--   0 lucjean    (501) staff       (20)      246 2019-08-29 13:07:42.000000 coop_html_editor-1.3.1/coop_html_editor/static/ckeditor.4.6.2/plugins/sourcedialog/lang/es.js
--rw-r--r--   0 lucjean    (501) staff       (20)      248 2019-08-29 13:07:42.000000 coop_html_editor-1.3.1/coop_html_editor/static/ckeditor.4.6.2/plugins/sourcedialog/lang/bn.js
--rw-r--r--   0 lucjean    (501) staff       (20)      234 2019-08-29 13:07:42.000000 coop_html_editor-1.3.1/coop_html_editor/static/ckeditor.4.6.2/plugins/sourcedialog/lang/eo.js
--rw-r--r--   0 lucjean    (501) staff       (20)      234 2019-08-29 13:07:42.000000 coop_html_editor-1.3.1/coop_html_editor/static/ckeditor.4.6.2/plugins/sourcedialog/lang/ro.js
--rw-r--r--   0 lucjean    (501) staff       (20)      236 2019-08-29 13:07:42.000000 coop_html_editor-1.3.1/coop_html_editor/static/ckeditor.4.6.2/plugins/sourcedialog/lang/tr.js
-drwxr-xr-x   0 lucjean    (501) staff       (20)        0 2019-08-30 10:40:01.000000 coop_html_editor-1.3.1/coop_html_editor/static/ckeditor.4.6.2/plugins/sourcedialog/samples/
--rw-r--r--   0 lucjean    (501) staff       (20)     3907 2019-08-29 13:07:42.000000 coop_html_editor-1.3.1/coop_html_editor/static/ckeditor.4.6.2/plugins/sourcedialog/samples/sourcedialog.html
-drwxr-xr-x   0 lucjean    (501) staff       (20)        0 2019-08-30 10:40:00.000000 coop_html_editor-1.3.1/coop_html_editor/static/ckeditor.4.6.2/plugins/sourcedialog/dialogs/
--rw-r--r--   0 lucjean    (501) staff       (20)     2204 2019-08-29 13:07:42.000000 coop_html_editor-1.3.1/coop_html_editor/static/ckeditor.4.6.2/plugins/sourcedialog/dialogs/sourcedialog.js
--rw-r--r--   0 lucjean    (501) staff       (20)     1193 2019-08-29 13:07:42.000000 coop_html_editor-1.3.1/coop_html_editor/static/ckeditor.4.6.2/plugins/sourcedialog/plugin.js
-drwxr-xr-x   0 lucjean    (501) staff       (20)        0 2019-08-30 10:39:35.000000 coop_html_editor-1.3.1/coop_html_editor/static/ckeditor.4.6.2/plugins/specialchar/
-drwxr-xr-x   0 lucjean    (501) staff       (20)        0 2019-08-30 10:40:01.000000 coop_html_editor-1.3.1/coop_html_editor/static/ckeditor.4.6.2/plugins/specialchar/dialogs/
--rw-r--r--   0 lucjean    (501) staff       (20)     5055 2019-08-29 13:07:43.000000 coop_html_editor-1.3.1/coop_html_editor/static/ckeditor.4.6.2/plugins/specialchar/dialogs/specialchar.js
-drwxr-xr-x   0 lucjean    (501) staff       (20)        0 2019-08-30 10:40:01.000000 coop_html_editor-1.3.1/coop_html_editor/static/ckeditor.4.6.2/plugins/specialchar/dialogs/lang/
--rw-r--r--   0 lucjean    (501) staff       (20)     4791 2019-08-29 13:07:42.000000 coop_html_editor-1.3.1/coop_html_editor/static/ckeditor.4.6.2/plugins/specialchar/dialogs/lang/pt.js
--rw-r--r--   0 lucjean    (501) staff       (20)     6081 2019-08-29 13:07:43.000000 coop_html_editor-1.3.1/coop_html_editor/static/ckeditor.4.6.2/plugins/specialchar/dialogs/lang/vi.js
--rw-r--r--   0 lucjean    (501) staff       (20)     5018 2019-08-29 13:07:42.000000 coop_html_editor-1.3.1/coop_html_editor/static/ckeditor.4.6.2/plugins/specialchar/dialogs/lang/lv.js
--rw-r--r--   0 lucjean    (501) staff       (20)     5000 2019-08-29 13:07:42.000000 coop_html_editor-1.3.1/coop_html_editor/static/ckeditor.4.6.2/plugins/specialchar/dialogs/lang/gl.js
--rw-r--r--   0 lucjean    (501) staff       (20)     4325 2019-08-29 13:07:42.000000 coop_html_editor-1.3.1/coop_html_editor/static/ckeditor.4.6.2/plugins/specialchar/dialogs/lang/pl.js
--rw-r--r--   0 lucjean    (501) staff       (20)     7728 2019-08-29 13:07:42.000000 coop_html_editor-1.3.1/coop_html_editor/static/ckeditor.4.6.2/plugins/specialchar/dialogs/lang/el.js
--rw-r--r--   0 lucjean    (501) staff       (20)     4488 2019-08-29 13:07:42.000000 coop_html_editor-1.3.1/coop_html_editor/static/ckeditor.4.6.2/plugins/specialchar/dialogs/lang/et.js
--rw-r--r--   0 lucjean    (501) staff       (20)     4345 2019-08-29 13:07:42.000000 coop_html_editor-1.3.1/coop_html_editor/static/ckeditor.4.6.2/plugins/specialchar/dialogs/lang/sl.js
--rw-r--r--   0 lucjean    (501) staff       (20)     4920 2019-08-29 13:07:42.000000 coop_html_editor-1.3.1/coop_html_editor/static/ckeditor.4.6.2/plugins/specialchar/dialogs/lang/ko.js
--rw-r--r--   0 lucjean    (501) staff       (20)     4520 2019-08-29 13:07:42.000000 coop_html_editor-1.3.1/coop_html_editor/static/ckeditor.4.6.2/plugins/specialchar/dialogs/lang/hr.js
--rw-r--r--   0 lucjean    (501) staff       (20)     4581 2019-08-29 13:07:42.000000 coop_html_editor-1.3.1/coop_html_editor/static/ckeditor.4.6.2/plugins/specialchar/dialogs/lang/fi.js
--rw-r--r--   0 lucjean    (501) staff       (20)     4672 2019-08-29 13:07:42.000000 coop_html_editor-1.3.1/coop_html_editor/static/ckeditor.4.6.2/plugins/specialchar/dialogs/lang/th.js
--rw-r--r--   0 lucjean    (501) staff       (20)     7543 2019-08-29 13:07:42.000000 coop_html_editor-1.3.1/coop_html_editor/static/ckeditor.4.6.2/plugins/specialchar/dialogs/lang/ru.js
--rw-r--r--   0 lucjean    (501) staff       (20)     4545 2019-08-29 13:07:42.000000 coop_html_editor-1.3.1/coop_html_editor/static/ckeditor.4.6.2/plugins/specialchar/dialogs/lang/eu.js
--rw-r--r--   0 lucjean    (501) staff       (20)     3428 2019-08-29 13:07:42.000000 coop_html_editor-1.3.1/coop_html_editor/static/ckeditor.4.6.2/plugins/specialchar/dialogs/lang/no.js
--rw-r--r--   0 lucjean    (501) staff       (20)     4974 2019-08-29 13:07:42.000000 coop_html_editor-1.3.1/coop_html_editor/static/ckeditor.4.6.2/plugins/specialchar/dialogs/lang/sq.js
--rw-r--r--   0 lucjean    (501) staff       (20)     4884 2019-08-29 13:07:42.000000 coop_html_editor-1.3.1/coop_html_editor/static/ckeditor.4.6.2/plugins/specialchar/dialogs/lang/si.js
--rw-r--r--   0 lucjean    (501) staff       (20)     6725 2019-08-29 13:07:43.000000 coop_html_editor-1.3.1/coop_html_editor/static/ckeditor.4.6.2/plugins/specialchar/dialogs/lang/tt.js
--rw-r--r--   0 lucjean    (501) staff       (20)     3980 2019-08-29 13:07:42.000000 coop_html_editor-1.3.1/coop_html_editor/static/ckeditor.4.6.2/plugins/specialchar/dialogs/lang/ja.js
--rw-r--r--   0 lucjean    (501) staff       (20)     4982 2019-08-29 13:07:42.000000 coop_html_editor-1.3.1/coop_html_editor/static/ckeditor.4.6.2/plugins/specialchar/dialogs/lang/he.js
--rw-r--r--   0 lucjean    (501) staff       (20)     4999 2019-08-29 13:07:43.000000 coop_html_editor-1.3.1/coop_html_editor/static/ckeditor.4.6.2/plugins/specialchar/dialogs/lang/ug.js
--rw-r--r--   0 lucjean    (501) staff       (20)     4735 2019-08-29 13:07:42.000000 coop_html_editor-1.3.1/coop_html_editor/static/ckeditor.4.6.2/plugins/specialchar/dialogs/lang/bg.js
--rw-r--r--   0 lucjean    (501) staff       (20)     4529 2019-08-29 13:07:42.000000 coop_html_editor-1.3.1/coop_html_editor/static/ckeditor.4.6.2/plugins/specialchar/dialogs/lang/af.js
--rw-r--r--   0 lucjean    (501) staff       (20)     4552 2019-08-29 13:07:42.000000 coop_html_editor-1.3.1/coop_html_editor/static/ckeditor.4.6.2/plugins/specialchar/dialogs/lang/id.js
--rw-r--r--   0 lucjean    (501) staff       (20)     3389 2019-08-29 13:07:42.000000 coop_html_editor-1.3.1/coop_html_editor/static/ckeditor.4.6.2/plugins/specialchar/dialogs/lang/az.js
--rw-r--r--   0 lucjean    (501) staff       (20)     5010 2019-08-29 13:07:42.000000 coop_html_editor-1.3.1/coop_html_editor/static/ckeditor.4.6.2/plugins/specialchar/dialogs/lang/ca.js
--rw-r--r--   0 lucjean    (501) staff       (20)     4891 2019-08-29 13:07:42.000000 coop_html_editor-1.3.1/coop_html_editor/static/ckeditor.4.6.2/plugins/specialchar/dialogs/lang/cy.js
--rw-r--r--   0 lucjean    (501) staff       (20)      720 2019-08-29 13:07:42.000000 coop_html_editor-1.3.1/coop_html_editor/static/ckeditor.4.6.2/plugins/specialchar/dialogs/lang/_translationstatus.txt
--rw-r--r--   0 lucjean    (501) staff       (20)     3428 2019-08-29 13:07:42.000000 coop_html_editor-1.3.1/coop_html_editor/static/ckeditor.4.6.2/plugins/specialchar/dialogs/lang/nb.js
--rw-r--r--   0 lucjean    (501) staff       (20)     4377 2019-08-29 13:07:43.000000 coop_html_editor-1.3.1/coop_html_editor/static/ckeditor.4.6.2/plugins/specialchar/dialogs/lang/zh-cn.js
--rw-r--r--   0 lucjean    (501) staff       (20)     4783 2019-08-29 13:07:42.000000 coop_html_editor-1.3.1/coop_html_editor/static/ckeditor.4.6.2/plugins/specialchar/dialogs/lang/de-ch.js
--rw-r--r--   0 lucjean    (501) staff       (20)     3826 2019-08-29 13:07:42.000000 coop_html_editor-1.3.1/coop_html_editor/static/ckeditor.4.6.2/plugins/specialchar/dialogs/lang/pt-br.js
--rw-r--r--   0 lucjean    (501) staff       (20)     3826 2019-08-29 13:07:42.000000 coop_html_editor-1.3.1/coop_html_editor/static/ckeditor.4.6.2/plugins/specialchar/dialogs/lang/oc.js
--rw-r--r--   0 lucjean    (501) staff       (20)     3360 2019-08-29 13:07:42.000000 coop_html_editor-1.3.1/coop_html_editor/static/ckeditor.4.6.2/plugins/specialchar/dialogs/lang/da.js
--rw-r--r--   0 lucjean    (501) staff       (20)     5768 2019-08-29 13:07:42.000000 coop_html_editor-1.3.1/coop_html_editor/static/ckeditor.4.6.2/plugins/specialchar/dialogs/lang/fa.js
--rw-r--r--   0 lucjean    (501) staff       (20)     4780 2019-08-29 13:07:42.000000 coop_html_editor-1.3.1/coop_html_editor/static/ckeditor.4.6.2/plugins/specialchar/dialogs/lang/de.js
--rw-r--r--   0 lucjean    (501) staff       (20)     4543 2019-08-29 13:07:42.000000 coop_html_editor-1.3.1/coop_html_editor/static/ckeditor.4.6.2/plugins/specialchar/dialogs/lang/en.js
--rw-r--r--   0 lucjean    (501) staff       (20)     7560 2019-08-29 13:07:42.000000 coop_html_editor-1.3.1/coop_html_editor/static/ckeditor.4.6.2/plugins/specialchar/dialogs/lang/ku.js
--rw-r--r--   0 lucjean    (501) staff       (20)     3480 2019-08-29 13:07:42.000000 coop_html_editor-1.3.1/coop_html_editor/static/ckeditor.4.6.2/plugins/specialchar/dialogs/lang/sv.js
--rw-r--r--   0 lucjean    (501) staff       (20)     4157 2019-08-29 13:07:43.000000 coop_html_editor-1.3.1/coop_html_editor/static/ckeditor.4.6.2/plugins/specialchar/dialogs/lang/zh.js
--rw-r--r--   0 lucjean    (501) staff       (20)     6366 2019-08-29 13:07:43.000000 coop_html_editor-1.3.1/coop_html_editor/static/ckeditor.4.6.2/plugins/specialchar/dialogs/lang/uk.js
--rw-r--r--   0 lucjean    (501) staff       (20)     4967 2019-08-29 13:07:42.000000 coop_html_editor-1.3.1/coop_html_editor/static/ckeditor.4.6.2/plugins/specialchar/dialogs/lang/cs.js
--rw-r--r--   0 lucjean    (501) staff       (20)     4747 2019-08-29 13:07:42.000000 coop_html_editor-1.3.1/coop_html_editor/static/ckeditor.4.6.2/plugins/specialchar/dialogs/lang/km.js
--rw-r--r--   0 lucjean    (501) staff       (20)     3852 2019-08-29 13:07:42.000000 coop_html_editor-1.3.1/coop_html_editor/static/ckeditor.4.6.2/plugins/specialchar/dialogs/lang/fr.js
--rw-r--r--   0 lucjean    (501) staff       (20)     4722 2019-08-29 13:07:42.000000 coop_html_editor-1.3.1/coop_html_editor/static/ckeditor.4.6.2/plugins/specialchar/dialogs/lang/nl.js
--rw-r--r--   0 lucjean    (501) staff       (20)     3216 2019-08-29 13:07:42.000000 coop_html_editor-1.3.1/coop_html_editor/static/ckeditor.4.6.2/plugins/specialchar/dialogs/lang/fr-ca.js
--rw-r--r--   0 lucjean    (501) staff       (20)     4546 2019-08-29 13:07:42.000000 coop_html_editor-1.3.1/coop_html_editor/static/ckeditor.4.6.2/plugins/specialchar/dialogs/lang/en-gb.js
--rw-r--r--   0 lucjean    (501) staff       (20)     4131 2019-08-29 13:07:42.000000 coop_html_editor-1.3.1/coop_html_editor/static/ckeditor.4.6.2/plugins/specialchar/dialogs/lang/hu.js
--rw-r--r--   0 lucjean    (501) staff       (20)     4588 2019-08-29 13:07:42.000000 coop_html_editor-1.3.1/coop_html_editor/static/ckeditor.4.6.2/plugins/specialchar/dialogs/lang/lt.js
--rw-r--r--   0 lucjean    (501) staff       (20)     4778 2019-08-29 13:07:42.000000 coop_html_editor-1.3.1/coop_html_editor/static/ckeditor.4.6.2/plugins/specialchar/dialogs/lang/ar.js
--rw-r--r--   0 lucjean    (501) staff       (20)     4760 2019-08-29 13:07:42.000000 coop_html_editor-1.3.1/coop_html_editor/static/ckeditor.4.6.2/plugins/specialchar/dialogs/lang/sk.js
--rw-r--r--   0 lucjean    (501) staff       (20)     5016 2019-08-29 13:07:42.000000 coop_html_editor-1.3.1/coop_html_editor/static/ckeditor.4.6.2/plugins/specialchar/dialogs/lang/it.js
--rw-r--r--   0 lucjean    (501) staff       (20)     4943 2019-08-29 13:07:42.000000 coop_html_editor-1.3.1/coop_html_editor/static/ckeditor.4.6.2/plugins/specialchar/dialogs/lang/es.js
--rw-r--r--   0 lucjean    (501) staff       (20)     4064 2019-08-29 13:07:42.000000 coop_html_editor-1.3.1/coop_html_editor/static/ckeditor.4.6.2/plugins/specialchar/dialogs/lang/eo.js
--rw-r--r--   0 lucjean    (501) staff       (20)     4475 2019-08-29 13:07:43.000000 coop_html_editor-1.3.1/coop_html_editor/static/ckeditor.4.6.2/plugins/specialchar/dialogs/lang/tr.js
-drwxr-xr-x   0 lucjean    (501) staff       (20)        0 2019-08-30 10:40:00.000000 coop_html_editor-1.3.1/coop_html_editor/static/ckeditor.4.6.2/plugins/scayt/
--rw-r--r--   0 lucjean    (501) staff       (20)     1476 2019-08-29 13:07:42.000000 coop_html_editor-1.3.1/coop_html_editor/static/ckeditor.4.6.2/plugins/scayt/LICENSE.md
--rw-r--r--   0 lucjean    (501) staff       (20)     1451 2019-08-29 13:07:42.000000 coop_html_editor-1.3.1/coop_html_editor/static/ckeditor.4.6.2/plugins/scayt/CHANGELOG.md
-drwxr-xr-x   0 lucjean    (501) staff       (20)        0 2019-08-30 10:39:35.000000 coop_html_editor-1.3.1/coop_html_editor/static/ckeditor.4.6.2/plugins/scayt/skins/
-drwxr-xr-x   0 lucjean    (501) staff       (20)        0 2019-08-30 10:40:00.000000 coop_html_editor-1.3.1/coop_html_editor/static/ckeditor.4.6.2/plugins/scayt/skins/moono-lisa/
--rw-r--r--   0 lucjean    (501) staff       (20)      330 2019-08-29 13:07:42.000000 coop_html_editor-1.3.1/coop_html_editor/static/ckeditor.4.6.2/plugins/scayt/skins/moono-lisa/scayt.css
--rw-r--r--   0 lucjean    (501) staff       (20)      979 2019-08-29 13:07:42.000000 coop_html_editor-1.3.1/coop_html_editor/static/ckeditor.4.6.2/plugins/scayt/README.md
-drwxr-xr-x   0 lucjean    (501) staff       (20)        0 2019-08-30 10:40:00.000000 coop_html_editor-1.3.1/coop_html_editor/static/ckeditor.4.6.2/plugins/scayt/dialogs/
--rw-r--r--   0 lucjean    (501) staff       (20)     1302 2019-08-29 13:07:42.000000 coop_html_editor-1.3.1/coop_html_editor/static/ckeditor.4.6.2/plugins/scayt/dialogs/toolbar.css
--rw-r--r--   0 lucjean    (501) staff       (20)     9577 2019-08-29 13:07:42.000000 coop_html_editor-1.3.1/coop_html_editor/static/ckeditor.4.6.2/plugins/scayt/dialogs/options.js
-drwxr-xr-x   0 lucjean    (501) staff       (20)        0 2019-08-30 10:40:00.000000 coop_html_editor-1.3.1/coop_html_editor/static/ckeditor.4.6.2/plugins/notificationaggregator/
--rw-r--r--   0 lucjean    (501) staff       (20)    15081 2019-08-29 13:07:42.000000 coop_html_editor-1.3.1/coop_html_editor/static/ckeditor.4.6.2/plugins/notificationaggregator/plugin.js
-drwxr-xr-x   0 lucjean    (501) staff       (20)        0 2019-08-30 10:39:56.000000 coop_html_editor-1.3.1/coop_html_editor/static/ckeditor.4.6.2/plugins/clipboard/
-drwxr-xr-x   0 lucjean    (501) staff       (20)        0 2019-08-30 10:39:58.000000 coop_html_editor-1.3.1/coop_html_editor/static/ckeditor.4.6.2/plugins/clipboard/lang/
--rw-r--r--   0 lucjean    (501) staff       (20)      996 2019-08-29 13:07:42.000000 coop_html_editor-1.3.1/coop_html_editor/static/ckeditor.4.6.2/plugins/clipboard/lang/sr-latn.js
--rw-r--r--   0 lucjean    (501) staff       (20)      934 2019-08-29 13:07:42.000000 coop_html_editor-1.3.1/coop_html_editor/static/ckeditor.4.6.2/plugins/clipboard/lang/pt.js
--rw-r--r--   0 lucjean    (501) staff       (20)     1091 2019-08-29 13:07:42.000000 coop_html_editor-1.3.1/coop_html_editor/static/ckeditor.4.6.2/plugins/clipboard/lang/vi.js
--rw-r--r--   0 lucjean    (501) staff       (20)      997 2019-08-29 13:07:42.000000 coop_html_editor-1.3.1/coop_html_editor/static/ckeditor.4.6.2/plugins/clipboard/lang/lv.js
--rw-r--r--   0 lucjean    (501) staff       (20)      887 2019-08-29 13:07:42.000000 coop_html_editor-1.3.1/coop_html_editor/static/ckeditor.4.6.2/plugins/clipboard/lang/gl.js
--rw-r--r--   0 lucjean    (501) staff       (20)      885 2019-08-29 13:07:42.000000 coop_html_editor-1.3.1/coop_html_editor/static/ckeditor.4.6.2/plugins/clipboard/lang/pl.js
--rw-r--r--   0 lucjean    (501) staff       (20)     1215 2019-08-29 13:07:42.000000 coop_html_editor-1.3.1/coop_html_editor/static/ckeditor.4.6.2/plugins/clipboard/lang/mn.js
--rw-r--r--   0 lucjean    (501) staff       (20)      907 2019-08-29 13:07:42.000000 coop_html_editor-1.3.1/coop_html_editor/static/ckeditor.4.6.2/plugins/clipboard/lang/en-ca.js
--rw-r--r--   0 lucjean    (501) staff       (20)     1444 2019-08-29 13:07:42.000000 coop_html_editor-1.3.1/coop_html_editor/static/ckeditor.4.6.2/plugins/clipboard/lang/el.js
--rw-r--r--   0 lucjean    (501) staff       (20)      928 2019-08-29 13:07:42.000000 coop_html_editor-1.3.1/coop_html_editor/static/ckeditor.4.6.2/plugins/clipboard/lang/et.js
--rw-r--r--   0 lucjean    (501) staff       (20)      879 2019-08-29 13:07:42.000000 coop_html_editor-1.3.1/coop_html_editor/static/ckeditor.4.6.2/plugins/clipboard/lang/is.js
--rw-r--r--   0 lucjean    (501) staff       (20)      875 2019-08-29 13:07:42.000000 coop_html_editor-1.3.1/coop_html_editor/static/ckeditor.4.6.2/plugins/clipboard/lang/sl.js
--rw-r--r--   0 lucjean    (501) staff       (20)      915 2019-08-29 13:07:42.000000 coop_html_editor-1.3.1/coop_html_editor/static/ckeditor.4.6.2/plugins/clipboard/lang/ko.js
--rw-r--r--   0 lucjean    (501) staff       (20)      933 2019-08-29 13:07:42.000000 coop_html_editor-1.3.1/coop_html_editor/static/ckeditor.4.6.2/plugins/clipboard/lang/hr.js
--rw-r--r--   0 lucjean    (501) staff       (20)      878 2019-08-29 13:07:42.000000 coop_html_editor-1.3.1/coop_html_editor/static/ckeditor.4.6.2/plugins/clipboard/lang/ms.js
--rw-r--r--   0 lucjean    (501) staff       (20)      807 2019-08-29 13:07:42.000000 coop_html_editor-1.3.1/coop_html_editor/static/ckeditor.4.6.2/plugins/clipboard/lang/fi.js
--rw-r--r--   0 lucjean    (501) staff       (20)     1532 2019-08-29 13:07:42.000000 coop_html_editor-1.3.1/coop_html_editor/static/ckeditor.4.6.2/plugins/clipboard/lang/th.js
--rw-r--r--   0 lucjean    (501) staff       (20)     1432 2019-08-29 13:07:42.000000 coop_html_editor-1.3.1/coop_html_editor/static/ckeditor.4.6.2/plugins/clipboard/lang/ru.js
--rw-r--r--   0 lucjean    (501) staff       (20)      894 2019-08-29 13:07:42.000000 coop_html_editor-1.3.1/coop_html_editor/static/ckeditor.4.6.2/plugins/clipboard/lang/eu.js
--rw-r--r--   0 lucjean    (501) staff       (20)     1462 2019-08-29 13:07:42.000000 coop_html_editor-1.3.1/coop_html_editor/static/ckeditor.4.6.2/plugins/clipboard/lang/mk.js
--rw-r--r--   0 lucjean    (501) staff       (20)      873 2019-08-29 13:07:42.000000 coop_html_editor-1.3.1/coop_html_editor/static/ckeditor.4.6.2/plugins/clipboard/lang/no.js
--rw-r--r--   0 lucjean    (501) staff       (20)     1063 2019-08-29 13:07:42.000000 coop_html_editor-1.3.1/coop_html_editor/static/ckeditor.4.6.2/plugins/clipboard/lang/sq.js
--rw-r--r--   0 lucjean    (501) staff       (20)     1286 2019-08-29 13:07:42.000000 coop_html_editor-1.3.1/coop_html_editor/static/ckeditor.4.6.2/plugins/clipboard/lang/gu.js
--rw-r--r--   0 lucjean    (501) staff       (20)     1035 2019-08-29 13:07:42.000000 coop_html_editor-1.3.1/coop_html_editor/static/ckeditor.4.6.2/plugins/clipboard/lang/si.js
--rw-r--r--   0 lucjean    (501) staff       (20)     1078 2019-08-29 13:07:42.000000 coop_html_editor-1.3.1/coop_html_editor/static/ckeditor.4.6.2/plugins/clipboard/lang/tt.js
--rw-r--r--   0 lucjean    (501) staff       (20)     1204 2019-08-29 13:07:42.000000 coop_html_editor-1.3.1/coop_html_editor/static/ckeditor.4.6.2/plugins/clipboard/lang/ja.js
--rw-r--r--   0 lucjean    (501) staff       (20)     1743 2019-08-29 13:07:42.000000 coop_html_editor-1.3.1/coop_html_editor/static/ckeditor.4.6.2/plugins/clipboard/lang/ka.js
--rw-r--r--   0 lucjean    (501) staff       (20)     1034 2019-08-29 13:07:42.000000 coop_html_editor-1.3.1/coop_html_editor/static/ckeditor.4.6.2/plugins/clipboard/lang/he.js
--rw-r--r--   0 lucjean    (501) staff       (20)     1481 2019-08-29 13:07:42.000000 coop_html_editor-1.3.1/coop_html_editor/static/ckeditor.4.6.2/plugins/clipboard/lang/ug.js
--rw-r--r--   0 lucjean    (501) staff       (20)     1318 2019-08-29 13:07:42.000000 coop_html_editor-1.3.1/coop_html_editor/static/ckeditor.4.6.2/plugins/clipboard/lang/bg.js
--rw-r--r--   0 lucjean    (501) staff       (20)      833 2019-08-29 13:07:42.000000 coop_html_editor-1.3.1/coop_html_editor/static/ckeditor.4.6.2/plugins/clipboard/lang/af.js
--rw-r--r--   0 lucjean    (501) staff       (20)      920 2019-08-29 13:07:42.000000 coop_html_editor-1.3.1/coop_html_editor/static/ckeditor.4.6.2/plugins/clipboard/lang/id.js
--rw-r--r--   0 lucjean    (501) staff       (20)      606 2019-08-29 13:07:42.000000 coop_html_editor-1.3.1/coop_html_editor/static/ckeditor.4.6.2/plugins/clipboard/lang/az.js
--rw-r--r--   0 lucjean    (501) staff       (20)      907 2019-08-29 13:07:42.000000 coop_html_editor-1.3.1/coop_html_editor/static/ckeditor.4.6.2/plugins/clipboard/lang/en-au.js
--rw-r--r--   0 lucjean    (501) staff       (20)      963 2019-08-29 13:07:42.000000 coop_html_editor-1.3.1/coop_html_editor/static/ckeditor.4.6.2/plugins/clipboard/lang/ca.js
--rw-r--r--   0 lucjean    (501) staff       (20)      957 2019-08-29 13:07:42.000000 coop_html_editor-1.3.1/coop_html_editor/static/ckeditor.4.6.2/plugins/clipboard/lang/cy.js
--rw-r--r--   0 lucjean    (501) staff       (20)      889 2019-08-29 13:07:42.000000 coop_html_editor-1.3.1/coop_html_editor/static/ckeditor.4.6.2/plugins/clipboard/lang/nb.js
--rw-r--r--   0 lucjean    (501) staff       (20)      861 2019-08-29 13:07:42.000000 coop_html_editor-1.3.1/coop_html_editor/static/ckeditor.4.6.2/plugins/clipboard/lang/zh-cn.js
--rw-r--r--   0 lucjean    (501) staff       (20)     1055 2019-08-29 13:07:42.000000 coop_html_editor-1.3.1/coop_html_editor/static/ckeditor.4.6.2/plugins/clipboard/lang/de-ch.js
--rw-r--r--   0 lucjean    (501) staff       (20)     1012 2019-08-29 13:07:42.000000 coop_html_editor-1.3.1/coop_html_editor/static/ckeditor.4.6.2/plugins/clipboard/lang/pt-br.js
--rw-r--r--   0 lucjean    (501) staff       (20)     1042 2019-08-29 13:07:42.000000 coop_html_editor-1.3.1/coop_html_editor/static/ckeditor.4.6.2/plugins/clipboard/lang/oc.js
--rw-r--r--   0 lucjean    (501) staff       (20)      970 2019-08-29 13:07:42.000000 coop_html_editor-1.3.1/coop_html_editor/static/ckeditor.4.6.2/plugins/clipboard/lang/da.js
--rw-r--r--   0 lucjean    (501) staff       (20)     1351 2019-08-29 13:07:42.000000 coop_html_editor-1.3.1/coop_html_editor/static/ckeditor.4.6.2/plugins/clipboard/lang/fa.js
--rw-r--r--   0 lucjean    (501) staff       (20)     1052 2019-08-29 13:07:42.000000 coop_html_editor-1.3.1/coop_html_editor/static/ckeditor.4.6.2/plugins/clipboard/lang/de.js
--rw-r--r--   0 lucjean    (501) staff       (20)      893 2019-08-29 13:07:42.000000 coop_html_editor-1.3.1/coop_html_editor/static/ckeditor.4.6.2/plugins/clipboard/lang/en.js
--rw-r--r--   0 lucjean    (501) staff       (20)      927 2019-08-29 13:07:42.000000 coop_html_editor-1.3.1/coop_html_editor/static/ckeditor.4.6.2/plugins/clipboard/lang/bs.js
--rw-r--r--   0 lucjean    (501) staff       (20)     1339 2019-08-29 13:07:42.000000 coop_html_editor-1.3.1/coop_html_editor/static/ckeditor.4.6.2/plugins/clipboard/lang/ku.js
--rw-r--r--   0 lucjean    (501) staff       (20)      845 2019-08-29 13:07:42.000000 coop_html_editor-1.3.1/coop_html_editor/static/ckeditor.4.6.2/plugins/clipboard/lang/sv.js
--rw-r--r--   0 lucjean    (501) staff       (20)      825 2019-08-29 13:07:42.000000 coop_html_editor-1.3.1/coop_html_editor/static/ckeditor.4.6.2/plugins/clipboard/lang/zh.js
--rw-r--r--   0 lucjean    (501) staff       (20)     1410 2019-08-29 13:07:42.000000 coop_html_editor-1.3.1/coop_html_editor/static/ckeditor.4.6.2/plugins/clipboard/lang/hi.js
--rw-r--r--   0 lucjean    (501) staff       (20)     1528 2019-08-29 13:07:42.000000 coop_html_editor-1.3.1/coop_html_editor/static/ckeditor.4.6.2/plugins/clipboard/lang/uk.js
--rw-r--r--   0 lucjean    (501) staff       (20)     1080 2019-08-29 13:07:42.000000 coop_html_editor-1.3.1/coop_html_editor/static/ckeditor.4.6.2/plugins/clipboard/lang/cs.js
--rw-r--r--   0 lucjean    (501) staff       (20)     2033 2019-08-29 13:07:42.000000 coop_html_editor-1.3.1/coop_html_editor/static/ckeditor.4.6.2/plugins/clipboard/lang/km.js
--rw-r--r--   0 lucjean    (501) staff       (20)     1075 2019-08-29 13:07:42.000000 coop_html_editor-1.3.1/coop_html_editor/static/ckeditor.4.6.2/plugins/clipboard/lang/fr.js
--rw-r--r--   0 lucjean    (501) staff       (20)      939 2019-08-29 13:07:42.000000 coop_html_editor-1.3.1/coop_html_editor/static/ckeditor.4.6.2/plugins/clipboard/lang/nl.js
--rw-r--r--   0 lucjean    (501) staff       (20)     1007 2019-08-29 13:07:42.000000 coop_html_editor-1.3.1/coop_html_editor/static/ckeditor.4.6.2/plugins/clipboard/lang/fr-ca.js
--rw-r--r--   0 lucjean    (501) staff       (20)      896 2019-08-29 13:07:42.000000 coop_html_editor-1.3.1/coop_html_editor/static/ckeditor.4.6.2/plugins/clipboard/lang/en-gb.js
--rw-r--r--   0 lucjean    (501) staff       (20)     1375 2019-08-29 13:07:42.000000 coop_html_editor-1.3.1/coop_html_editor/static/ckeditor.4.6.2/plugins/clipboard/lang/sr.js
--rw-r--r--   0 lucjean    (501) staff       (20)     1005 2019-08-29 13:07:42.000000 coop_html_editor-1.3.1/coop_html_editor/static/ckeditor.4.6.2/plugins/clipboard/lang/hu.js
--rw-r--r--   0 lucjean    (501) staff       (20)      980 2019-08-29 13:07:42.000000 coop_html_editor-1.3.1/coop_html_editor/static/ckeditor.4.6.2/plugins/clipboard/lang/lt.js
--rw-r--r--   0 lucjean    (501) staff       (20)      920 2019-08-29 13:07:42.000000 coop_html_editor-1.3.1/coop_html_editor/static/ckeditor.4.6.2/plugins/clipboard/lang/fo.js
--rw-r--r--   0 lucjean    (501) staff       (20)     1168 2019-08-29 13:07:42.000000 coop_html_editor-1.3.1/coop_html_editor/static/ckeditor.4.6.2/plugins/clipboard/lang/ar.js
--rw-r--r--   0 lucjean    (501) staff       (20)      928 2019-08-29 13:07:42.000000 coop_html_editor-1.3.1/coop_html_editor/static/ckeditor.4.6.2/plugins/clipboard/lang/sk.js
--rw-r--r--   0 lucjean    (501) staff       (20)      921 2019-08-29 13:07:42.000000 coop_html_editor-1.3.1/coop_html_editor/static/ckeditor.4.6.2/plugins/clipboard/lang/it.js
--rw-r--r--   0 lucjean    (501) staff       (20)      947 2019-08-29 13:07:42.000000 coop_html_editor-1.3.1/coop_html_editor/static/ckeditor.4.6.2/plugins/clipboard/lang/es.js
--rw-r--r--   0 lucjean    (501) staff       (20)     1543 2019-08-29 13:07:42.000000 coop_html_editor-1.3.1/coop_html_editor/static/ckeditor.4.6.2/plugins/clipboard/lang/bn.js
--rw-r--r--   0 lucjean    (501) staff       (20)      900 2019-08-29 13:07:42.000000 coop_html_editor-1.3.1/coop_html_editor/static/ckeditor.4.6.2/plugins/clipboard/lang/eo.js
--rw-r--r--   0 lucjean    (501) staff       (20)     1062 2019-08-29 13:07:42.000000 coop_html_editor-1.3.1/coop_html_editor/static/ckeditor.4.6.2/plugins/clipboard/lang/ro.js
--rw-r--r--   0 lucjean    (501) staff       (20)      966 2019-08-29 13:07:42.000000 coop_html_editor-1.3.1/coop_html_editor/static/ckeditor.4.6.2/plugins/clipboard/lang/tr.js
-drwxr-xr-x   0 lucjean    (501) staff       (20)        0 2019-08-30 10:39:56.000000 coop_html_editor-1.3.1/coop_html_editor/static/ckeditor.4.6.2/plugins/clipboard/dialogs/
--rw-r--r--   0 lucjean    (501) staff       (20)     3963 2019-08-29 13:07:42.000000 coop_html_editor-1.3.1/coop_html_editor/static/ckeditor.4.6.2/plugins/clipboard/dialogs/paste.js
-drwxr-xr-x   0 lucjean    (501) staff       (20)        0 2019-08-30 10:39:56.000000 coop_html_editor-1.3.1/coop_html_editor/static/ckeditor.4.6.2/plugins/clipboard/dev/
--rw-r--r--   0 lucjean    (501) staff       (20)     1077 2019-08-29 13:07:42.000000 coop_html_editor-1.3.1/coop_html_editor/static/ckeditor.4.6.2/plugins/clipboard/dev/console.js
--rw-r--r--   0 lucjean    (501) staff       (20)    14102 2019-08-29 13:07:42.000000 coop_html_editor-1.3.1/coop_html_editor/static/ckeditor.4.6.2/plugins/clipboard/dev/dnd.html
--rw-r--r--   0 lucjean    (501) staff       (20)     5581 2019-08-29 13:07:42.000000 coop_html_editor-1.3.1/coop_html_editor/static/ckeditor.4.6.2/plugins/clipboard/dev/clipboard.html
--rw-r--r--   0 lucjean    (501) staff       (20)   100076 2019-08-29 13:07:42.000000 coop_html_editor-1.3.1/coop_html_editor/static/ckeditor.4.6.2/plugins/clipboard/plugin.js
--rw-r--r--   0 lucjean    (501) staff       (20)     2955 2019-08-29 13:07:41.000000 coop_html_editor-1.3.1/coop_html_editor/static/ckeditor.4.6.2/contents.css
-drwxr-xr-x   0 lucjean    (501) staff       (20)        0 2019-08-30 10:39:35.000000 coop_html_editor-1.3.1/coop_html_editor/static/ckeditor.4.6.2/skins/
-drwxr-xr-x   0 lucjean    (501) staff       (20)        0 2019-08-30 10:40:05.000000 coop_html_editor-1.3.1/coop_html_editor/static/ckeditor.4.6.2/skins/moono-lisa/
--rw-r--r--   0 lucjean    (501) staff       (20)    37414 2019-08-29 13:07:45.000000 coop_html_editor-1.3.1/coop_html_editor/static/ckeditor.4.6.2/skins/moono-lisa/editor_iequirks.css
--rw-r--r--   0 lucjean    (501) staff       (20)    35766 2019-08-29 13:07:45.000000 coop_html_editor-1.3.1/coop_html_editor/static/ckeditor.4.6.2/skins/moono-lisa/editor.css
-drwxr-xr-x   0 lucjean    (501) staff       (20)        0 2019-08-30 10:40:05.000000 coop_html_editor-1.3.1/coop_html_editor/static/ckeditor.4.6.2/skins/moono-lisa/images/
--rw-r--r--   0 lucjean    (501) staff       (20)      506 2019-08-29 13:07:45.000000 coop_html_editor-1.3.1/coop_html_editor/static/ckeditor.4.6.2/skins/moono-lisa/images/lock.png
--rw-r--r--   0 lucjean    (501) staff       (20)     2984 2019-08-29 13:07:45.000000 coop_html_editor-1.3.1/coop_html_editor/static/ckeditor.4.6.2/skins/moono-lisa/images/spinner.gif
--rw-r--r--   0 lucjean    (501) staff       (20)      191 2019-08-29 13:07:45.000000 coop_html_editor-1.3.1/coop_html_editor/static/ckeditor.4.6.2/skins/moono-lisa/images/arrow.png
--rw-r--r--   0 lucjean    (501) staff       (20)      511 2019-08-29 13:07:45.000000 coop_html_editor-1.3.1/coop_html_editor/static/ckeditor.4.6.2/skins/moono-lisa/images/lock-open.png
-drwxr-xr-x   0 lucjean    (501) staff       (20)        0 2019-08-30 10:40:05.000000 coop_html_editor-1.3.1/coop_html_editor/static/ckeditor.4.6.2/skins/moono-lisa/images/hidpi/
--rw-r--r--   0 lucjean    (501) staff       (20)     1062 2019-08-29 13:07:45.000000 coop_html_editor-1.3.1/coop_html_editor/static/ckeditor.4.6.2/skins/moono-lisa/images/hidpi/lock.png
--rw-r--r--   0 lucjean    (501) staff       (20)     1071 2019-08-29 13:07:45.000000 coop_html_editor-1.3.1/coop_html_editor/static/ckeditor.4.6.2/skins/moono-lisa/images/hidpi/lock-open.png
--rw-r--r--   0 lucjean    (501) staff       (20)     1623 2019-08-29 13:07:45.000000 coop_html_editor-1.3.1/coop_html_editor/static/ckeditor.4.6.2/skins/moono-lisa/images/hidpi/refresh.png
--rw-r--r--   0 lucjean    (501) staff       (20)     1238 2019-08-29 13:07:45.000000 coop_html_editor-1.3.1/coop_html_editor/static/ckeditor.4.6.2/skins/moono-lisa/images/hidpi/close.png
--rw-r--r--   0 lucjean    (501) staff       (20)      757 2019-08-29 13:07:45.000000 coop_html_editor-1.3.1/coop_html_editor/static/ckeditor.4.6.2/skins/moono-lisa/images/refresh.png
--rw-r--r--   0 lucjean    (501) staff       (20)      615 2019-08-29 13:07:45.000000 coop_html_editor-1.3.1/coop_html_editor/static/ckeditor.4.6.2/skins/moono-lisa/images/close.png
--rw-r--r--   0 lucjean    (501) staff       (20)    36765 2019-08-29 13:07:45.000000 coop_html_editor-1.3.1/coop_html_editor/static/ckeditor.4.6.2/skins/moono-lisa/editor_ie.css
--rw-r--r--   0 lucjean    (501) staff       (20)    37571 2019-08-29 13:07:45.000000 coop_html_editor-1.3.1/coop_html_editor/static/ckeditor.4.6.2/skins/moono-lisa/editor_ie8.css
--rw-r--r--   0 lucjean    (501) staff       (20)    14490 2019-08-29 13:07:45.000000 coop_html_editor-1.3.1/coop_html_editor/static/ckeditor.4.6.2/skins/moono-lisa/dialog_iequirks.css
--rw-r--r--   0 lucjean    (501) staff       (20)     2224 2019-08-29 13:07:45.000000 coop_html_editor-1.3.1/coop_html_editor/static/ckeditor.4.6.2/skins/moono-lisa/readme.md
--rw-r--r--   0 lucjean    (501) staff       (20)     6057 2019-08-29 13:07:45.000000 coop_html_editor-1.3.1/coop_html_editor/static/ckeditor.4.6.2/skins/moono-lisa/icons.png
--rw-r--r--   0 lucjean    (501) staff       (20)    35847 2019-08-29 13:07:45.000000 coop_html_editor-1.3.1/coop_html_editor/static/ckeditor.4.6.2/skins/moono-lisa/editor_gecko.css
--rw-r--r--   0 lucjean    (501) staff       (20)    14461 2019-08-29 13:07:45.000000 coop_html_editor-1.3.1/coop_html_editor/static/ckeditor.4.6.2/skins/moono-lisa/dialog_ie.css
--rw-r--r--   0 lucjean    (501) staff       (20)    13550 2019-08-29 13:07:45.000000 coop_html_editor-1.3.1/coop_html_editor/static/ckeditor.4.6.2/skins/moono-lisa/dialog.css
--rw-r--r--   0 lucjean    (501) staff       (20)    20877 2019-08-29 13:07:45.000000 coop_html_editor-1.3.1/coop_html_editor/static/ckeditor.4.6.2/skins/moono-lisa/icons_hidpi.png
--rw-r--r--   0 lucjean    (501) staff       (20)    14944 2019-08-29 13:07:45.000000 coop_html_editor-1.3.1/coop_html_editor/static/ckeditor.4.6.2/skins/moono-lisa/dialog_ie8.css
--rw-r--r--   0 lucjean    (501) staff       (20)     1321 2019-08-29 13:07:41.000000 coop_html_editor-1.3.1/coop_html_editor/static/ckeditor.4.6.2/config.js
--rw-r--r--   0 lucjean    (501) staff       (20)   535544 2019-08-29 13:07:41.000000 coop_html_editor-1.3.1/coop_html_editor/static/ckeditor.4.6.2/ckeditor.js
--rw-r--r--   0 lucjean    (501) staff       (20)     1342 2019-08-29 13:07:41.000000 coop_html_editor-1.3.1/coop_html_editor/static/ckeditor.4.6.2/README.md
-drwxr-xr-x   0 lucjean    (501) staff       (20)        0 2019-08-30 10:39:54.000000 coop_html_editor-1.3.1/coop_html_editor/static/ckeditor.4.6.2/lang/
--rw-r--r--   0 lucjean    (501) staff       (20)    11251 2019-08-29 13:07:41.000000 coop_html_editor-1.3.1/coop_html_editor/static/ckeditor.4.6.2/lang/en.js
--rw-r--r--   0 lucjean    (501) staff       (20)    13074 2019-08-29 13:07:41.000000 coop_html_editor-1.3.1/coop_html_editor/static/ckeditor.4.6.2/lang/fr.js
-drwxr-xr-x   0 lucjean    (501) staff       (20)        0 2019-08-30 10:40:03.000000 coop_html_editor-1.3.1/coop_html_editor/static/ckeditor.4.6.2/samples/
--rw-r--r--   0 lucjean    (501) staff       (20)     6692 2019-08-29 13:07:45.000000 coop_html_editor-1.3.1/coop_html_editor/static/ckeditor.4.6.2/samples/index.html
-drwxr-xr-x   0 lucjean    (501) staff       (20)        0 2019-08-30 10:40:03.000000 coop_html_editor-1.3.1/coop_html_editor/static/ckeditor.4.6.2/samples/css/
--rw-r--r--   0 lucjean    (501) staff       (20)    67258 2019-08-29 13:07:45.000000 coop_html_editor-1.3.1/coop_html_editor/static/ckeditor.4.6.2/samples/css/samples.css
-drwxr-xr-x   0 lucjean    (501) staff       (20)        0 2019-08-30 10:40:03.000000 coop_html_editor-1.3.1/coop_html_editor/static/ckeditor.4.6.2/samples/js/
--rw-r--r--   0 lucjean    (501) staff       (20)     6408 2019-08-29 13:07:45.000000 coop_html_editor-1.3.1/coop_html_editor/static/ckeditor.4.6.2/samples/js/sf.js
--rw-r--r--   0 lucjean    (501) staff       (20)     1574 2019-08-29 13:07:45.000000 coop_html_editor-1.3.1/coop_html_editor/static/ckeditor.4.6.2/samples/js/sample.js
-drwxr-xr-x   0 lucjean    (501) staff       (20)        0 2019-08-30 10:40:03.000000 coop_html_editor-1.3.1/coop_html_editor/static/ckeditor.4.6.2/samples/old/
--rw-r--r--   0 lucjean    (501) staff       (20)     7027 2019-08-29 13:07:45.000000 coop_html_editor-1.3.1/coop_html_editor/static/ckeditor.4.6.2/samples/old/xhtmlstyle.html
--rw-r--r--   0 lucjean    (501) staff       (20)     5758 2019-08-29 13:07:45.000000 coop_html_editor-1.3.1/coop_html_editor/static/ckeditor.4.6.2/samples/old/index.html
-drwxr-xr-x   0 lucjean    (501) staff       (20)        0 2019-08-30 10:40:04.000000 coop_html_editor-1.3.1/coop_html_editor/static/ckeditor.4.6.2/samples/old/magicline/
--rw-r--r--   0 lucjean    (501) staff       (20)     8380 2019-08-29 13:07:45.000000 coop_html_editor-1.3.1/coop_html_editor/static/ckeditor.4.6.2/samples/old/magicline/magicline.html
--rw-r--r--   0 lucjean    (501) staff       (20)     2404 2019-08-29 13:07:45.000000 coop_html_editor-1.3.1/coop_html_editor/static/ckeditor.4.6.2/samples/old/tabindex.html
-drwxr-xr-x   0 lucjean    (501) staff       (20)        0 2019-08-30 10:40:04.000000 coop_html_editor-1.3.1/coop_html_editor/static/ckeditor.4.6.2/samples/old/toolbar/
--rw-r--r--   0 lucjean    (501) staff       (20)     8900 2019-08-29 13:07:45.000000 coop_html_editor-1.3.1/coop_html_editor/static/ckeditor.4.6.2/samples/old/toolbar/toolbar.html
--rw-r--r--   0 lucjean    (501) staff       (20)     2259 2019-08-29 13:07:45.000000 coop_html_editor-1.3.1/coop_html_editor/static/ckeditor.4.6.2/samples/old/appendto.html
--rw-r--r--   0 lucjean    (501) staff       (20)     4670 2019-08-29 13:07:45.000000 coop_html_editor-1.3.1/coop_html_editor/static/ckeditor.4.6.2/samples/old/divreplace.html
--rw-r--r--   0 lucjean    (501) staff       (20)     7511 2019-08-29 13:07:45.000000 coop_html_editor-1.3.1/coop_html_editor/static/ckeditor.4.6.2/samples/old/jquery.html
--rw-r--r--   0 lucjean    (501) staff       (20)    10195 2019-08-29 13:07:45.000000 coop_html_editor-1.3.1/coop_html_editor/static/ckeditor.4.6.2/samples/old/inlineall.html
-drwxr-xr-x   0 lucjean    (501) staff       (20)        0 2019-08-30 10:40:04.000000 coop_html_editor-1.3.1/coop_html_editor/static/ckeditor.4.6.2/samples/old/wysiwygarea/
--rw-r--r--   0 lucjean    (501) staff       (20)     8106 2019-08-29 13:07:45.000000 coop_html_editor-1.3.1/coop_html_editor/static/ckeditor.4.6.2/samples/old/wysiwygarea/fullpage.html
-drwxr-xr-x   0 lucjean    (501) staff       (20)        0 2019-08-30 10:40:04.000000 coop_html_editor-1.3.1/coop_html_editor/static/ckeditor.4.6.2/samples/old/htmlwriter/
--rw-r--r--   0 lucjean    (501) staff       (20)     7321 2019-08-29 13:07:45.000000 coop_html_editor-1.3.1/coop_html_editor/static/ckeditor.4.6.2/samples/old/htmlwriter/outputhtml.html
--rw-r--r--   0 lucjean    (501) staff       (20)    10108 2019-08-29 13:07:45.000000 coop_html_editor-1.3.1/coop_html_editor/static/ckeditor.4.6.2/samples/old/htmlwriter/outputforflash.html
-drwxr-xr-x   0 lucjean    (501) staff       (20)        0 2019-08-30 10:39:35.000000 coop_html_editor-1.3.1/coop_html_editor/static/ckeditor.4.6.2/samples/old/htmlwriter/assets/
-drwxr-xr-x   0 lucjean    (501) staff       (20)        0 2019-08-30 10:40:04.000000 coop_html_editor-1.3.1/coop_html_editor/static/ckeditor.4.6.2/samples/old/htmlwriter/assets/outputforflash/
--rw-r--r--   0 lucjean    (501) staff       (20)     9589 2019-08-29 13:07:45.000000 coop_html_editor-1.3.1/coop_html_editor/static/ckeditor.4.6.2/samples/old/htmlwriter/assets/outputforflash/swfobject.js
--rw-r--r--   0 lucjean    (501) staff       (20)    15571 2019-08-29 13:07:45.000000 coop_html_editor-1.3.1/coop_html_editor/static/ckeditor.4.6.2/samples/old/htmlwriter/assets/outputforflash/outputforflash.swf
--rw-r--r--   0 lucjean    (501) staff       (20)    85504 2019-08-29 13:07:45.000000 coop_html_editor-1.3.1/coop_html_editor/static/ckeditor.4.6.2/samples/old/htmlwriter/assets/outputforflash/outputforflash.fla
-drwxr-xr-x   0 lucjean    (501) staff       (20)        0 2019-08-30 10:40:03.000000 coop_html_editor-1.3.1/coop_html_editor/static/ckeditor.4.6.2/samples/old/dialog/
--rw-r--r--   0 lucjean    (501) staff       (20)     7345 2019-08-29 13:07:45.000000 coop_html_editor-1.3.1/coop_html_editor/static/ckeditor.4.6.2/samples/old/dialog/dialog.html
-drwxr-xr-x   0 lucjean    (501) staff       (20)        0 2019-08-30 10:40:03.000000 coop_html_editor-1.3.1/coop_html_editor/static/ckeditor.4.6.2/samples/old/dialog/assets/
--rw-r--r--   0 lucjean    (501) staff       (20)      877 2019-08-29 13:07:45.000000 coop_html_editor-1.3.1/coop_html_editor/static/ckeditor.4.6.2/samples/old/dialog/assets/my_dialog.js
--rw-r--r--   0 lucjean    (501) staff       (20)     4920 2019-08-29 13:07:45.000000 coop_html_editor-1.3.1/coop_html_editor/static/ckeditor.4.6.2/samples/old/inlinetextarea.html
--rw-r--r--   0 lucjean    (501) staff       (20)     7011 2019-08-29 13:07:45.000000 coop_html_editor-1.3.1/coop_html_editor/static/ckeditor.4.6.2/samples/old/replacebyclass.html
--rw-r--r--   0 lucjean    (501) staff       (20)      789 2019-08-29 13:07:45.000000 coop_html_editor-1.3.1/coop_html_editor/static/ckeditor.4.6.2/samples/old/sample_posteddata.php
--rw-r--r--   0 lucjean    (501) staff       (20)    47482 2019-08-29 13:07:45.000000 coop_html_editor-1.3.1/coop_html_editor/static/ckeditor.4.6.2/samples/old/datafiltering.html
--rw-r--r--   0 lucjean    (501) staff       (20)     6914 2019-08-29 13:07:45.000000 coop_html_editor-1.3.1/coop_html_editor/static/ckeditor.4.6.2/samples/old/replacebycode.html
--rw-r--r--   0 lucjean    (501) staff       (20)     4495 2019-08-29 13:07:45.000000 coop_html_editor-1.3.1/coop_html_editor/static/ckeditor.4.6.2/samples/old/uilanguages.html
--rw-r--r--   0 lucjean    (501) staff       (20)     2706 2019-08-29 13:07:45.000000 coop_html_editor-1.3.1/coop_html_editor/static/ckeditor.4.6.2/samples/old/ajax.html
-drwxr-xr-x   0 lucjean    (501) staff       (20)        0 2019-08-30 10:40:04.000000 coop_html_editor-1.3.1/coop_html_editor/static/ckeditor.4.6.2/samples/old/enterkey/
--rw-r--r--   0 lucjean    (501) staff       (20)     4352 2019-08-29 13:07:45.000000 coop_html_editor-1.3.1/coop_html_editor/static/ckeditor.4.6.2/samples/old/enterkey/enterkey.html
--rw-r--r--   0 lucjean    (501) staff       (20)     7179 2019-08-29 13:07:45.000000 coop_html_editor-1.3.1/coop_html_editor/static/ckeditor.4.6.2/samples/old/api.html
--rw-r--r--   0 lucjean    (501) staff       (20)     6190 2019-08-29 13:07:45.000000 coop_html_editor-1.3.1/coop_html_editor/static/ckeditor.4.6.2/samples/old/inlinebycode.html
-drwxr-xr-x   0 lucjean    (501) staff       (20)        0 2019-08-30 10:40:03.000000 coop_html_editor-1.3.1/coop_html_editor/static/ckeditor.4.6.2/samples/old/assets/
-drwxr-xr-x   0 lucjean    (501) staff       (20)        0 2019-08-30 10:40:03.000000 coop_html_editor-1.3.1/coop_html_editor/static/ckeditor.4.6.2/samples/old/assets/uilanguages/
--rw-r--r--   0 lucjean    (501) staff       (20)     1416 2019-08-29 13:07:45.000000 coop_html_editor-1.3.1/coop_html_editor/static/ckeditor.4.6.2/samples/old/assets/uilanguages/languages.js
--rw-r--r--   0 lucjean    (501) staff       (20)     1443 2019-08-29 13:07:45.000000 coop_html_editor-1.3.1/coop_html_editor/static/ckeditor.4.6.2/samples/old/assets/posteddata.php
-drwxr-xr-x   0 lucjean    (501) staff       (20)        0 2019-08-30 10:40:03.000000 coop_html_editor-1.3.1/coop_html_editor/static/ckeditor.4.6.2/samples/old/assets/outputxhtml/
--rw-r--r--   0 lucjean    (501) staff       (20)     2143 2019-08-29 13:07:45.000000 coop_html_editor-1.3.1/coop_html_editor/static/ckeditor.4.6.2/samples/old/assets/outputxhtml/outputxhtml.css
--rw-r--r--   0 lucjean    (501) staff       (20)    14449 2019-08-29 13:07:45.000000 coop_html_editor-1.3.1/coop_html_editor/static/ckeditor.4.6.2/samples/old/assets/sample.jpg
-drwxr-xr-x   0 lucjean    (501) staff       (20)        0 2019-08-30 10:40:03.000000 coop_html_editor-1.3.1/coop_html_editor/static/ckeditor.4.6.2/samples/old/assets/inlineall/
--rw-r--r--   0 lucjean    (501) staff       (20)     4283 2019-08-29 13:07:45.000000 coop_html_editor-1.3.1/coop_html_editor/static/ckeditor.4.6.2/samples/old/assets/inlineall/logo.png
--rw-r--r--   0 lucjean    (501) staff       (20)     1675 2019-08-29 13:07:45.000000 coop_html_editor-1.3.1/coop_html_editor/static/ckeditor.4.6.2/samples/old/sample.js
--rw-r--r--   0 lucjean    (501) staff       (20)     5094 2019-08-29 13:07:45.000000 coop_html_editor-1.3.1/coop_html_editor/static/ckeditor.4.6.2/samples/old/sample.css
--rw-r--r--   0 lucjean    (501) staff       (20)     2604 2019-08-29 13:07:45.000000 coop_html_editor-1.3.1/coop_html_editor/static/ckeditor.4.6.2/samples/old/uicolor.html
--rw-r--r--   0 lucjean    (501) staff       (20)     2886 2019-08-29 13:07:45.000000 coop_html_editor-1.3.1/coop_html_editor/static/ckeditor.4.6.2/samples/old/readonly.html
-drwxr-xr-x   0 lucjean    (501) staff       (20)        0 2019-08-30 10:40:03.000000 coop_html_editor-1.3.1/coop_html_editor/static/ckeditor.4.6.2/samples/img/
--rw-r--r--   0 lucjean    (501) staff       (20)      123 2019-08-29 13:07:45.000000 coop_html_editor-1.3.1/coop_html_editor/static/ckeditor.4.6.2/samples/img/header-separator.png
--rw-r--r--   0 lucjean    (501) staff       (20)     5891 2019-08-29 13:07:45.000000 coop_html_editor-1.3.1/coop_html_editor/static/ckeditor.4.6.2/samples/img/logo.png
--rw-r--r--   0 lucjean    (501) staff       (20)    13086 2019-08-29 13:07:45.000000 coop_html_editor-1.3.1/coop_html_editor/static/ckeditor.4.6.2/samples/img/header-bg.png
--rw-r--r--   0 lucjean    (501) staff       (20)      383 2019-08-29 13:07:45.000000 coop_html_editor-1.3.1/coop_html_editor/static/ckeditor.4.6.2/samples/img/github-top.png
--rw-r--r--   0 lucjean    (501) staff       (20)    12029 2019-08-29 13:07:45.000000 coop_html_editor-1.3.1/coop_html_editor/static/ckeditor.4.6.2/samples/img/navigation-tip.png
-drwxr-xr-x   0 lucjean    (501) staff       (20)        0 2019-08-30 10:40:04.000000 coop_html_editor-1.3.1/coop_html_editor/static/ckeditor.4.6.2/samples/toolbarconfigurator/
--rw-r--r--   0 lucjean    (501) staff       (20)    15449 2019-08-29 13:07:45.000000 coop_html_editor-1.3.1/coop_html_editor/static/ckeditor.4.6.2/samples/toolbarconfigurator/index.html
-drwxr-xr-x   0 lucjean    (501) staff       (20)        0 2019-08-30 10:40:04.000000 coop_html_editor-1.3.1/coop_html_editor/static/ckeditor.4.6.2/samples/toolbarconfigurator/css/
--rw-r--r--   0 lucjean    (501) staff       (20)     1758 2019-08-29 13:07:45.000000 coop_html_editor-1.3.1/coop_html_editor/static/ckeditor.4.6.2/samples/toolbarconfigurator/css/fontello.css
-drwxr-xr-x   0 lucjean    (501) staff       (20)        0 2019-08-30 10:40:04.000000 coop_html_editor-1.3.1/coop_html_editor/static/ckeditor.4.6.2/samples/toolbarconfigurator/js/
--rw-r--r--   0 lucjean    (501) staff       (20)     3819 2019-08-29 13:07:45.000000 coop_html_editor-1.3.1/coop_html_editor/static/ckeditor.4.6.2/samples/toolbarconfigurator/js/fulltoolbareditor.js
--rw-r--r--   0 lucjean    (501) staff       (20)     6523 2019-08-29 13:07:45.000000 coop_html_editor-1.3.1/coop_html_editor/static/ckeditor.4.6.2/samples/toolbarconfigurator/js/abstracttoolbarmodifier.js
--rw-r--r--   0 lucjean    (501) staff       (20)     6850 2019-08-29 13:07:45.000000 coop_html_editor-1.3.1/coop_html_editor/static/ckeditor.4.6.2/samples/toolbarconfigurator/js/toolbartextmodifier.js
--rw-r--r--   0 lucjean    (501) staff       (20)    16651 2019-08-29 13:07:45.000000 coop_html_editor-1.3.1/coop_html_editor/static/ckeditor.4.6.2/samples/toolbarconfigurator/js/toolbarmodifier.js
-drwxr-xr-x   0 lucjean    (501) staff       (20)        0 2019-08-30 10:39:35.000000 coop_html_editor-1.3.1/coop_html_editor/static/ckeditor.4.6.2/samples/toolbarconfigurator/lib/
-drwxr-xr-x   0 lucjean    (501) staff       (20)        0 2019-08-30 10:40:04.000000 coop_html_editor-1.3.1/coop_html_editor/static/ckeditor.4.6.2/samples/toolbarconfigurator/lib/codemirror/
--rw-r--r--   0 lucjean    (501) staff       (20)      851 2019-08-29 13:07:45.000000 coop_html_editor-1.3.1/coop_html_editor/static/ckeditor.4.6.2/samples/toolbarconfigurator/lib/codemirror/neo.css
--rw-r--r--   0 lucjean    (501) staff       (20)      700 2019-08-29 13:07:45.000000 coop_html_editor-1.3.1/coop_html_editor/static/ckeditor.4.6.2/samples/toolbarconfigurator/lib/codemirror/show-hint.css
--rw-r--r--   0 lucjean    (501) staff       (20)   148874 2019-08-29 13:07:45.000000 coop_html_editor-1.3.1/coop_html_editor/static/ckeditor.4.6.2/samples/toolbarconfigurator/lib/codemirror/codemirror.js
--rw-r--r--   0 lucjean    (501) staff       (20)     1094 2019-08-29 13:07:45.000000 coop_html_editor-1.3.1/coop_html_editor/static/ckeditor.4.6.2/samples/toolbarconfigurator/lib/codemirror/LICENSE
--rw-r--r--   0 lucjean    (501) staff       (20)     8096 2019-08-29 13:07:45.000000 coop_html_editor-1.3.1/coop_html_editor/static/ckeditor.4.6.2/samples/toolbarconfigurator/lib/codemirror/codemirror.css
--rw-r--r--   0 lucjean    (501) staff       (20)     8080 2019-08-29 13:07:45.000000 coop_html_editor-1.3.1/coop_html_editor/static/ckeditor.4.6.2/samples/toolbarconfigurator/lib/codemirror/show-hint.js
--rw-r--r--   0 lucjean    (501) staff       (20)    12285 2019-08-29 13:07:45.000000 coop_html_editor-1.3.1/coop_html_editor/static/ckeditor.4.6.2/samples/toolbarconfigurator/lib/codemirror/javascript.js
-drwxr-xr-x   0 lucjean    (501) staff       (20)        0 2019-08-30 10:40:04.000000 coop_html_editor-1.3.1/coop_html_editor/static/ckeditor.4.6.2/samples/toolbarconfigurator/font/
--rw-r--r--   0 lucjean    (501) staff       (20)     4820 2019-08-29 13:07:45.000000 coop_html_editor-1.3.1/coop_html_editor/static/ckeditor.4.6.2/samples/toolbarconfigurator/font/fontello.ttf
--rw-r--r--   0 lucjean    (501) staff       (20)     2904 2019-08-29 13:07:45.000000 coop_html_editor-1.3.1/coop_html_editor/static/ckeditor.4.6.2/samples/toolbarconfigurator/font/fontello.woff
--rw-r--r--   0 lucjean    (501) staff       (20)      557 2019-08-29 13:07:45.000000 coop_html_editor-1.3.1/coop_html_editor/static/ckeditor.4.6.2/samples/toolbarconfigurator/font/config.json
--rw-r--r--   0 lucjean    (501) staff       (20)     4988 2019-08-29 13:07:45.000000 coop_html_editor-1.3.1/coop_html_editor/static/ckeditor.4.6.2/samples/toolbarconfigurator/font/fontello.eot
--rw-r--r--   0 lucjean    (501) staff       (20)     1701 2019-08-29 13:07:45.000000 coop_html_editor-1.3.1/coop_html_editor/static/ckeditor.4.6.2/samples/toolbarconfigurator/font/fontello.svg
--rw-r--r--   0 lucjean    (501) staff       (20)      188 2019-08-29 13:07:45.000000 coop_html_editor-1.3.1/coop_html_editor/static/ckeditor.4.6.2/samples/toolbarconfigurator/font/LICENSE.txt
-drwxr-xr-x   0 lucjean    (501) staff       (20)        0 2019-08-30 10:39:54.000000 coop_html_editor-1.3.1/coop_html_editor/static/ckeditor.4.6.2/adapters/
--rw-r--r--   0 lucjean    (501) staff       (20)     3179 2019-08-29 13:07:41.000000 coop_html_editor-1.3.1/coop_html_editor/static/ckeditor.4.6.2/adapters/jquery.js
--rw-r--r--   0 lucjean    (501) staff       (20)   153288 2019-08-29 13:07:41.000000 coop_html_editor-1.3.1/coop_html_editor/static/ckeditor.4.6.2/CHANGES.md
--rw-r--r--   0 lucjean    (501) staff       (20)     2173 2019-08-29 13:07:41.000000 coop_html_editor-1.3.1/coop_html_editor/static/ckeditor.4.6.2/build-config.js
--rw-r--r--   0 lucjean    (501) staff       (20)     5516 2019-08-29 13:07:45.000000 coop_html_editor-1.3.1/coop_html_editor/static/ckeditor.4.6.2/styles.js
-drwxr-xr-x   0 lucjean    (501) staff       (20)        0 2019-08-30 10:39:35.000000 coop_html_editor-1.3.1/coop_html_editor/static/html-editor/
-drwxr-xr-x   0 lucjean    (501) staff       (20)        0 2019-08-30 10:40:05.000000 coop_html_editor-1.3.1/coop_html_editor/static/html-editor/css/
--rw-r--r--   0 lucjean    (501) staff       (20)      178 2019-08-29 13:07:45.000000 coop_html_editor-1.3.1/coop_html_editor/static/html-editor/css/aloha.css
--rw-r--r--   0 lucjean    (501) staff       (20)      179 2019-08-29 13:07:45.000000 coop_html_editor-1.3.1/coop_html_editor/static/html-editor/css/aloha-fixes.css
-drwxr-xr-x   0 lucjean    (501) staff       (20)        0 2019-08-30 10:40:05.000000 coop_html_editor-1.3.1/coop_html_editor/static/html-editor/js/
--rw-r--r--   0 lucjean    (501) staff       (20)      949 2019-08-29 13:07:45.000000 coop_html_editor-1.3.1/coop_html_editor/static/html-editor/js/aloha-init.js
-drwxr-xr-x   0 lucjean    (501) staff       (20)        0 2019-08-30 10:40:05.000000 coop_html_editor-1.3.1/coop_html_editor/static/js/
--rw-r--r--   0 lucjean    (501) staff       (20)    94840 2019-08-29 13:07:46.000000 coop_html_editor-1.3.1/coop_html_editor/static/js/jquery-1.7.2.min.js
--rw-r--r--   0 lucjean    (501) staff       (20)   252881 2019-08-29 13:07:46.000000 coop_html_editor-1.3.1/coop_html_editor/static/js/jquery-1.7.2.js
-drwxr-xr-x   0 lucjean    (501) staff       (20)        0 2019-08-30 10:39:36.000000 coop_html_editor-1.3.1/coop_html_editor/static/aloha.0.23.26/
-drwxr-xr-x   0 lucjean    (501) staff       (20)        0 2019-08-30 10:39:35.000000 coop_html_editor-1.3.1/coop_html_editor/static/aloha.0.23.26/demo/
-drwxr-xr-x   0 lucjean    (501) staff       (20)        0 2019-08-30 10:39:38.000000 coop_html_editor-1.3.1/coop_html_editor/static/aloha.0.23.26/demo/world/
--rw-r--r--   0 lucjean    (501) staff       (20)     5801 2019-08-29 13:07:38.000000 coop_html_editor-1.3.1/coop_html_editor/static/aloha.0.23.26/demo/world/index.html
-drwxr-xr-x   0 lucjean    (501) staff       (20)        0 2019-08-30 10:39:38.000000 coop_html_editor-1.3.1/coop_html_editor/static/aloha.0.23.26/demo/world/js/
--rw-r--r--   0 lucjean    (501) staff       (20)     4516 2019-08-29 13:07:38.000000 coop_html_editor-1.3.1/coop_html_editor/static/aloha.0.23.26/demo/world/js/aloha-config.js
--rw-r--r--   0 lucjean    (501) staff       (20)     2830 2019-08-29 13:07:38.000000 coop_html_editor-1.3.1/coop_html_editor/static/aloha.0.23.26/demo/world/index.css
-drwxr-xr-x   0 lucjean    (501) staff       (20)        0 2019-08-30 10:39:38.000000 coop_html_editor-1.3.1/coop_html_editor/static/aloha.0.23.26/demo/simple/
--rw-r--r--   0 lucjean    (501) staff       (20)      742 2019-08-29 13:07:38.000000 coop_html_editor-1.3.1/coop_html_editor/static/aloha.0.23.26/demo/simple/index.html
--rw-r--r--   0 lucjean    (501) staff       (20)      732 2019-08-29 13:07:38.000000 coop_html_editor-1.3.1/coop_html_editor/static/aloha.0.23.26/demo/simple/index.css
-drwxr-xr-x   0 lucjean    (501) staff       (20)        0 2019-08-30 10:39:37.000000 coop_html_editor-1.3.1/coop_html_editor/static/aloha.0.23.26/demo/common/
--rw-r--r--   0 lucjean    (501) staff       (20)      167 2019-08-29 13:07:37.000000 coop_html_editor-1.3.1/coop_html_editor/static/aloha.0.23.26/demo/common/external-link-ltr-icon.png
--rw-r--r--   0 lucjean    (501) staff       (20)     1395 2019-08-29 13:07:37.000000 coop_html_editor-1.3.1/coop_html_editor/static/aloha.0.23.26/demo/common/index.css
--rw-r--r--   0 lucjean    (501) staff       (20)      154 2019-08-29 13:07:37.000000 coop_html_editor-1.3.1/coop_html_editor/static/aloha.0.23.26/demo/common/background.png
-drwxr-xr-x   0 lucjean    (501) staff       (20)        0 2019-08-30 10:39:38.000000 coop_html_editor-1.3.1/coop_html_editor/static/aloha.0.23.26/demo/textarea/
--rw-r--r--   0 lucjean    (501) staff       (20)     3947 2019-08-29 13:07:38.000000 coop_html_editor-1.3.1/coop_html_editor/static/aloha.0.23.26/demo/textarea/index.php
-drwxr-xr-x   0 lucjean    (501) staff       (20)        0 2019-08-30 10:39:36.000000 coop_html_editor-1.3.1/coop_html_editor/static/aloha.0.23.26/demo/boilerplate/
--rw-r--r--   0 lucjean    (501) staff       (20)     6358 2019-08-29 13:07:37.000000 coop_html_editor-1.3.1/coop_html_editor/static/aloha.0.23.26/demo/boilerplate/captioned-image.html
--rw-r--r--   0 lucjean    (501) staff       (20)     3860 2019-08-29 13:07:37.000000 coop_html_editor-1.3.1/coop_html_editor/static/aloha.0.23.26/demo/boilerplate/ribbon-example.js
--rw-r--r--   0 lucjean    (501) staff       (20)      539 2019-08-29 13:07:37.000000 coop_html_editor-1.3.1/coop_html_editor/static/aloha.0.23.26/demo/boilerplate/favicon.ico
--rw-r--r--   0 lucjean    (501) staff       (20)    12113 2019-08-29 13:07:37.000000 coop_html_editor-1.3.1/coop_html_editor/static/aloha.0.23.26/demo/boilerplate/index.html
--rw-r--r--   0 lucjean    (501) staff       (20)      528 2019-08-29 13:07:37.000000 coop_html_editor-1.3.1/coop_html_editor/static/aloha.0.23.26/demo/boilerplate/apple-touch-icon.png
-drwxr-xr-x   0 lucjean    (501) staff       (20)        0 2019-08-30 10:39:36.000000 coop_html_editor-1.3.1/coop_html_editor/static/aloha.0.23.26/demo/boilerplate/css/
--rw-r--r--   0 lucjean    (501) staff       (20)    12958 2019-08-29 13:07:37.000000 coop_html_editor-1.3.1/coop_html_editor/static/aloha.0.23.26/demo/boilerplate/css/style.css
--rw-r--r--   0 lucjean    (501) staff       (20)     1755 2019-08-29 13:07:37.000000 coop_html_editor-1.3.1/coop_html_editor/static/aloha.0.23.26/demo/boilerplate/humans.txt
--rw-r--r--   0 lucjean    (501) staff       (20)      880 2019-08-29 13:07:37.000000 coop_html_editor-1.3.1/coop_html_editor/static/aloha.0.23.26/demo/boilerplate/apple-touch-icon-114x114-precomposed.png
-drwxr-xr-x   0 lucjean    (501) staff       (20)        0 2019-08-30 10:39:37.000000 coop_html_editor-1.3.1/coop_html_editor/static/aloha.0.23.26/demo/boilerplate/js/
--rw-r--r--   0 lucjean    (501) staff       (20)     1560 2019-08-29 13:07:37.000000 coop_html_editor-1.3.1/coop_html_editor/static/aloha.0.23.26/demo/boilerplate/js/aloha-boilerplate.js
-drwxr-xr-x   0 lucjean    (501) staff       (20)        0 2019-08-30 10:39:37.000000 coop_html_editor-1.3.1/coop_html_editor/static/aloha.0.23.26/demo/boilerplate/js/libs/
--rw-r--r--   0 lucjean    (501) staff       (20)     7019 2019-08-29 13:07:37.000000 coop_html_editor-1.3.1/coop_html_editor/static/aloha.0.23.26/demo/boilerplate/js/libs/dd_belatedpng.js
--rw-r--r--   0 lucjean    (501) staff       (20)     9021 2019-08-29 13:07:37.000000 coop_html_editor-1.3.1/coop_html_editor/static/aloha.0.23.26/demo/boilerplate/js/libs/modernizr-1.7.min.js
--rw-r--r--   0 lucjean    (501) staff       (20)   234994 2019-08-29 13:07:37.000000 coop_html_editor-1.3.1/coop_html_editor/static/aloha.0.23.26/demo/boilerplate/js/libs/jquery-1.6.1.js
--rw-r--r--   0 lucjean    (501) staff       (20)     6404 2019-08-29 13:07:37.000000 coop_html_editor-1.3.1/coop_html_editor/static/aloha.0.23.26/demo/boilerplate/js/aloha-config.js
-drwxr-xr-x   0 lucjean    (501) staff       (20)        0 2019-08-30 10:39:37.000000 coop_html_editor-1.3.1/coop_html_editor/static/aloha.0.23.26/demo/boilerplate/img/
--rw-r--r--   0 lucjean    (501) staff       (20)      252 2019-08-29 13:07:37.000000 coop_html_editor-1.3.1/coop_html_editor/static/aloha.0.23.26/demo/boilerplate/img/navigation-bg-hover.png
--rw-r--r--   0 lucjean    (501) staff       (20)      750 2019-08-29 13:07:37.000000 coop_html_editor-1.3.1/coop_html_editor/static/aloha.0.23.26/demo/boilerplate/img/stage-switcher-tab-bg-active.png
--rw-r--r--   0 lucjean    (501) staff       (20)   260785 2019-08-29 13:07:37.000000 coop_html_editor-1.3.1/coop_html_editor/static/aloha.0.23.26/demo/boilerplate/img/stage-bg-formats.png
--rw-r--r--   0 lucjean    (501) staff       (20)      140 2019-08-29 13:07:37.000000 coop_html_editor-1.3.1/coop_html_editor/static/aloha.0.23.26/demo/boilerplate/img/stage-switcher-tab-bg.png
--rw-r--r--   0 lucjean    (501) staff       (20)   431334 2019-08-29 13:07:37.000000 coop_html_editor-1.3.1/coop_html_editor/static/aloha.0.23.26/demo/boilerplate/img/stage-bg-comments.png
--rw-r--r--   0 lucjean    (501) staff       (20)      870 2019-08-29 13:07:37.000000 coop_html_editor-1.3.1/coop_html_editor/static/aloha.0.23.26/demo/boilerplate/img/stage-icon-comments.png
--rw-r--r--   0 lucjean    (501) staff       (20)     2177 2019-08-29 13:07:37.000000 coop_html_editor-1.3.1/coop_html_editor/static/aloha.0.23.26/demo/boilerplate/img/loading.gif
--rw-r--r--   0 lucjean    (501) staff       (20)     7853 2019-08-29 13:07:37.000000 coop_html_editor-1.3.1/coop_html_editor/static/aloha.0.23.26/demo/boilerplate/img/aloha-editor-logo.png
--rw-r--r--   0 lucjean    (501) staff       (20)      828 2019-08-29 13:07:37.000000 coop_html_editor-1.3.1/coop_html_editor/static/aloha.0.23.26/demo/boilerplate/img/stage-switcher-tab-bg-hover.png
--rw-r--r--   0 lucjean    (501) staff       (20)      276 2019-08-29 13:07:37.000000 coop_html_editor-1.3.1/coop_html_editor/static/aloha.0.23.26/demo/boilerplate/img/stage-icon-formats.png
--rw-r--r--   0 lucjean    (501) staff       (20)      210 2019-08-29 13:07:37.000000 coop_html_editor-1.3.1/coop_html_editor/static/aloha.0.23.26/demo/boilerplate/img/navigation-bg.png
--rw-r--r--   0 lucjean    (501) staff       (20)   470732 2019-08-29 13:07:37.000000 coop_html_editor-1.3.1/coop_html_editor/static/aloha.0.23.26/demo/boilerplate/img/stage-bg-boxes.png
--rw-r--r--   0 lucjean    (501) staff       (20)      236 2019-08-29 13:07:37.000000 coop_html_editor-1.3.1/coop_html_editor/static/aloha.0.23.26/demo/boilerplate/img/stage-icon-boxes.png
--rw-r--r--   0 lucjean    (501) staff       (20)     2563 2019-08-29 13:07:37.000000 coop_html_editor-1.3.1/coop_html_editor/static/aloha.0.23.26/demo/boilerplate/img/stage-switcher-bg.png
--rw-r--r--   0 lucjean    (501) staff       (20)    51237 2019-08-29 13:07:37.000000 coop_html_editor-1.3.1/coop_html_editor/static/aloha.0.23.26/demo/boilerplate/img/stage-bg-tables.jpg
--rw-r--r--   0 lucjean    (501) staff       (20)   411434 2019-08-29 13:07:37.000000 coop_html_editor-1.3.1/coop_html_editor/static/aloha.0.23.26/demo/boilerplate/img/stage-bg-tables.png
--rw-r--r--   0 lucjean    (501) staff       (20)      484 2019-08-29 13:07:37.000000 coop_html_editor-1.3.1/coop_html_editor/static/aloha.0.23.26/demo/boilerplate/img/stage-icon-images.png
--rw-r--r--   0 lucjean    (501) staff       (20)     1440 2019-08-29 13:07:37.000000 coop_html_editor-1.3.1/coop_html_editor/static/aloha.0.23.26/demo/boilerplate/img/loading1.gif
--rw-r--r--   0 lucjean    (501) staff       (20)     1415 2019-08-29 13:07:37.000000 coop_html_editor-1.3.1/coop_html_editor/static/aloha.0.23.26/demo/boilerplate/img/stage-bg.png
--rw-r--r--   0 lucjean    (501) staff       (20)   419532 2019-08-29 13:07:37.000000 coop_html_editor-1.3.1/coop_html_editor/static/aloha.0.23.26/demo/boilerplate/img/stage-bg-images.png
--rw-r--r--   0 lucjean    (501) staff       (20)      110 2019-08-29 13:07:37.000000 coop_html_editor-1.3.1/coop_html_editor/static/aloha.0.23.26/demo/boilerplate/img/stage-icon-tables.png
--rw-r--r--   0 lucjean    (501) staff       (20)      528 2019-08-29 13:07:37.000000 coop_html_editor-1.3.1/coop_html_editor/static/aloha.0.23.26/demo/boilerplate/apple-touch-icon-precomposed.png
--rw-r--r--   0 lucjean    (501) staff       (20)      189 2019-08-29 13:07:37.000000 coop_html_editor-1.3.1/coop_html_editor/static/aloha.0.23.26/demo/boilerplate/fake-jquery.js
--rw-r--r--   0 lucjean    (501) staff       (20)      107 2019-08-29 13:07:37.000000 coop_html_editor-1.3.1/coop_html_editor/static/aloha.0.23.26/demo/boilerplate/robots.txt
--rw-r--r--   0 lucjean    (501) staff       (20)      619 2019-08-29 13:07:37.000000 coop_html_editor-1.3.1/coop_html_editor/static/aloha.0.23.26/demo/boilerplate/apple-touch-icon-72x72-precomposed.png
--rw-r--r--   0 lucjean    (501) staff       (20)      528 2019-08-29 13:07:37.000000 coop_html_editor-1.3.1/coop_html_editor/static/aloha.0.23.26/demo/boilerplate/apple-touch-icon-57x57-precomposed.png
--rw-r--r--   0 lucjean    (501) staff       (20)      802 2019-08-29 13:07:37.000000 coop_html_editor-1.3.1/coop_html_editor/static/aloha.0.23.26/demo/boilerplate/crossdomain.xml
-drwxr-xr-x   0 lucjean    (501) staff       (20)        0 2019-08-30 10:39:37.000000 coop_html_editor-1.3.1/coop_html_editor/static/aloha.0.23.26/demo/commands/
--rw-r--r--   0 lucjean    (501) staff       (20)      476 2019-08-29 13:07:37.000000 coop_html_editor-1.3.1/coop_html_editor/static/aloha.0.23.26/demo/commands/index.html
--rw-r--r--   0 lucjean    (501) staff       (20)     1131 2019-08-29 13:07:37.000000 coop_html_editor-1.3.1/coop_html_editor/static/aloha.0.23.26/demo/commands/commands-demo.js
-drwxr-xr-x   0 lucjean    (501) staff       (20)        0 2019-08-30 10:39:38.000000 coop_html_editor-1.3.1/coop_html_editor/static/aloha.0.23.26/demo/dev-table-resize/
--rw-r--r--   0 lucjean    (501) staff       (20)     3416 2019-08-29 13:07:38.000000 coop_html_editor-1.3.1/coop_html_editor/static/aloha.0.23.26/demo/dev-table-resize/index.html
-drwxr-xr-x   0 lucjean    (501) staff       (20)        0 2019-08-30 10:39:38.000000 coop_html_editor-1.3.1/coop_html_editor/static/aloha.0.23.26/demo/dev-table-resize/js/
--rw-r--r--   0 lucjean    (501) staff       (20)     4587 2019-08-29 13:07:38.000000 coop_html_editor-1.3.1/coop_html_editor/static/aloha.0.23.26/demo/dev-table-resize/js/aloha-config.js
--rw-r--r--   0 lucjean    (501) staff       (20)     3179 2019-08-29 13:07:38.000000 coop_html_editor-1.3.1/coop_html_editor/static/aloha.0.23.26/demo/dev-table-resize/index.css
-drwxr-xr-x   0 lucjean    (501) staff       (20)        0 2019-08-30 10:39:37.000000 coop_html_editor-1.3.1/coop_html_editor/static/aloha.0.23.26/demo/demo-app/
--rw-r--r--   0 lucjean    (501) staff       (20)     2298 2019-08-29 13:07:38.000000 coop_html_editor-1.3.1/coop_html_editor/static/aloha.0.23.26/demo/demo-app/page.html
--rw-r--r--   0 lucjean    (501) staff       (20)     3290 2019-08-29 13:07:38.000000 coop_html_editor-1.3.1/coop_html_editor/static/aloha.0.23.26/demo/demo-app/index.html
--rw-r--r--   0 lucjean    (501) staff       (20)     3804 2019-08-29 13:07:38.000000 coop_html_editor-1.3.1/coop_html_editor/static/aloha.0.23.26/demo/demo-app/feedback.html
-drwxr-xr-x   0 lucjean    (501) staff       (20)        0 2019-08-30 10:39:37.000000 coop_html_editor-1.3.1/coop_html_editor/static/aloha.0.23.26/demo/demo-app/app/
-drwxr-xr-x   0 lucjean    (501) staff       (20)        0 2019-08-30 10:39:35.000000 coop_html_editor-1.3.1/coop_html_editor/static/aloha.0.23.26/demo/demo-app/app/aloha-plugins/
-drwxr-xr-x   0 lucjean    (501) staff       (20)        0 2019-08-30 10:39:35.000000 coop_html_editor-1.3.1/coop_html_editor/static/aloha.0.23.26/demo/demo-app/app/aloha-plugins/cms/
-drwxr-xr-x   0 lucjean    (501) staff       (20)        0 2019-08-30 10:39:37.000000 coop_html_editor-1.3.1/coop_html_editor/static/aloha.0.23.26/demo/demo-app/app/aloha-plugins/cms/extra/
--rw-r--r--   0 lucjean    (501) staff       (20)     2264 2019-08-29 13:07:38.000000 coop_html_editor-1.3.1/coop_html_editor/static/aloha.0.23.26/demo/demo-app/app/aloha-plugins/cms/extra/cms-linklist.js
-drwxr-xr-x   0 lucjean    (501) staff       (20)        0 2019-08-30 10:39:37.000000 coop_html_editor-1.3.1/coop_html_editor/static/aloha.0.23.26/demo/demo-app/app/aloha-plugins/cms/lib/
--rw-r--r--   0 lucjean    (501) staff       (20)      498 2019-08-29 13:07:38.000000 coop_html_editor-1.3.1/coop_html_editor/static/aloha.0.23.26/demo/demo-app/app/aloha-plugins/cms/lib/cms-plugin.js
-drwxr-xr-x   0 lucjean    (501) staff       (20)        0 2019-08-30 10:39:37.000000 coop_html_editor-1.3.1/coop_html_editor/static/aloha.0.23.26/demo/demo-app/app/css/
--rw-r--r--   0 lucjean    (501) staff       (20)    56339 2019-08-29 13:07:38.000000 coop_html_editor-1.3.1/coop_html_editor/static/aloha.0.23.26/demo/demo-app/app/css/bootstrap.css
--rw-r--r--   0 lucjean    (501) staff       (20)      257 2019-08-29 13:07:38.000000 coop_html_editor-1.3.1/coop_html_editor/static/aloha.0.23.26/demo/demo-app/app/css/aloha-editor-demo.css
-drwxr-xr-x   0 lucjean    (501) staff       (20)        0 2019-08-30 10:39:37.000000 coop_html_editor-1.3.1/coop_html_editor/static/aloha.0.23.26/demo/demo-app/app/js/
--rw-r--r--   0 lucjean    (501) staff       (20)     1418 2019-08-29 13:07:38.000000 coop_html_editor-1.3.1/coop_html_editor/static/aloha.0.23.26/demo/demo-app/app/js/aloha-save-to-backend.js
--rw-r--r--   0 lucjean    (501) staff       (20)     4896 2019-08-29 13:07:38.000000 coop_html_editor-1.3.1/coop_html_editor/static/aloha.0.23.26/demo/demo-app/app/js/demo-app-load.js
--rw-r--r--   0 lucjean    (501) staff       (20)     1940 2019-08-29 13:07:38.000000 coop_html_editor-1.3.1/coop_html_editor/static/aloha.0.23.26/demo/demo-app/app/js/demo-app.js
-drwxr-xr-x   0 lucjean    (501) staff       (20)        0 2019-08-30 10:39:37.000000 coop_html_editor-1.3.1/coop_html_editor/static/aloha.0.23.26/demo/demo-app/app/js/bootstrap/
--rw-r--r--   0 lucjean    (501) staff       (20)     3002 2019-08-29 13:07:38.000000 coop_html_editor-1.3.1/coop_html_editor/static/aloha.0.23.26/demo/demo-app/app/js/bootstrap/bootstrap-scrollspy.js
--rw-r--r--   0 lucjean    (501) staff       (20)     1690 2019-08-29 13:07:38.000000 coop_html_editor-1.3.1/coop_html_editor/static/aloha.0.23.26/demo/demo-app/app/js/bootstrap/bootstrap-dropdown.js
--rw-r--r--   0 lucjean    (501) staff       (20)     1789 2019-08-29 13:07:38.000000 coop_html_editor-1.3.1/coop_html_editor/static/aloha.0.23.26/demo/demo-app/app/js/bootstrap/bootstrap-buttons.js
--rw-r--r--   0 lucjean    (501) staff       (20)     2737 2019-08-29 13:07:38.000000 coop_html_editor-1.3.1/coop_html_editor/static/aloha.0.23.26/demo/demo-app/app/js/bootstrap/bootstrap-popover.js
--rw-r--r--   0 lucjean    (501) staff       (20)     6424 2019-08-29 13:07:38.000000 coop_html_editor-1.3.1/coop_html_editor/static/aloha.0.23.26/demo/demo-app/app/js/bootstrap/bootstrap-modal.js
--rw-r--r--   0 lucjean    (501) staff       (20)     8233 2019-08-29 13:07:38.000000 coop_html_editor-1.3.1/coop_html_editor/static/aloha.0.23.26/demo/demo-app/app/js/bootstrap/bootstrap-twipsy.js
--rw-r--r--   0 lucjean    (501) staff       (20)     2166 2019-08-29 13:07:38.000000 coop_html_editor-1.3.1/coop_html_editor/static/aloha.0.23.26/demo/demo-app/app/js/bootstrap/bootstrap-tabs.js
--rw-r--r--   0 lucjean    (501) staff       (20)     3373 2019-08-29 13:07:38.000000 coop_html_editor-1.3.1/coop_html_editor/static/aloha.0.23.26/demo/demo-app/app/js/bootstrap/bootstrap-alerts.js
--rw-r--r--   0 lucjean    (501) staff       (20)     1099 2019-08-29 13:07:38.000000 coop_html_editor-1.3.1/coop_html_editor/static/aloha.0.23.26/demo/demo-app/app/js/aloha-read-from-backend.js
--rw-r--r--   0 lucjean    (501) staff       (20)    94020 2019-08-29 13:07:38.000000 coop_html_editor-1.3.1/coop_html_editor/static/aloha.0.23.26/demo/demo-app/app/js/jquery-1.7.min.js
--rw-r--r--   0 lucjean    (501) staff       (20)      842 2019-08-29 13:07:38.000000 coop_html_editor-1.3.1/coop_html_editor/static/aloha.0.23.26/demo/demo-app/app/js/demo-app-prepare.js
--rw-r--r--   0 lucjean    (501) staff       (20)     1954 2019-08-29 13:07:38.000000 coop_html_editor-1.3.1/coop_html_editor/static/aloha.0.23.26/demo/demo-app/app/save-to-db.php
--rw-r--r--   0 lucjean    (501) staff       (20)     1600 2019-08-29 13:07:38.000000 coop_html_editor-1.3.1/coop_html_editor/static/aloha.0.23.26/demo/demo-app/app/demo-app-linklist.php
--rw-r--r--   0 lucjean    (501) staff       (20)      622 2019-08-29 13:07:38.000000 coop_html_editor-1.3.1/coop_html_editor/static/aloha.0.23.26/demo/demo-app/app/save-to-session.php
-drwxr-xr-x   0 lucjean    (501) staff       (20)        0 2019-08-30 10:39:37.000000 coop_html_editor-1.3.1/coop_html_editor/static/aloha.0.23.26/demo/demo-app/app/aloha-editor/
--rw-r--r--   0 lucjean    (501) staff       (20)      240 2019-08-29 13:07:38.000000 coop_html_editor-1.3.1/coop_html_editor/static/aloha.0.23.26/demo/demo-app/app/aloha-editor/INSTALL-ALOHA-EDITOR.txt
--rw-r--r--   0 lucjean    (501) staff       (20)     1494 2019-08-29 13:07:38.000000 coop_html_editor-1.3.1/coop_html_editor/static/aloha.0.23.26/demo/demo-app/app/read-from-db.php
-drwxr-xr-x   0 lucjean    (501) staff       (20)        0 2019-08-30 10:39:37.000000 coop_html_editor-1.3.1/coop_html_editor/static/aloha.0.23.26/demo/demo-app/app/aloha-config/
--rw-r--r--   0 lucjean    (501) staff       (20)     4462 2019-08-29 13:07:38.000000 coop_html_editor-1.3.1/coop_html_editor/static/aloha.0.23.26/demo/demo-app/app/aloha-config/full.js
--rw-r--r--   0 lucjean    (501) staff       (20)     4462 2019-08-29 13:07:37.000000 coop_html_editor-1.3.1/coop_html_editor/static/aloha.0.23.26/demo/demo-app/app/aloha-config/default.js
--rw-r--r--   0 lucjean    (501) staff       (20)      487 2019-08-29 13:07:38.000000 coop_html_editor-1.3.1/coop_html_editor/static/aloha.0.23.26/demo/demo-app/app/aloha-config/minimal.js
--rw-r--r--   0 lucjean    (501) staff       (20)      610 2019-08-29 13:07:38.000000 coop_html_editor-1.3.1/coop_html_editor/static/aloha.0.23.26/demo/demo-app/app/aloha-config/minimal-demo.js
-drwxr-xr-x   0 lucjean    (501) staff       (20)        0 2019-08-30 10:39:37.000000 coop_html_editor-1.3.1/coop_html_editor/static/aloha.0.23.26/demo/demo-app/app/lib/
--rw-r--r--   0 lucjean    (501) staff       (20)     3477 2019-08-29 13:07:38.000000 coop_html_editor-1.3.1/coop_html_editor/static/aloha.0.23.26/demo/demo-app/app/lib/JSLikeHTMLElement.php
--rw-r--r--   0 lucjean    (501) staff       (20)      563 2019-08-29 13:07:38.000000 coop_html_editor-1.3.1/coop_html_editor/static/aloha.0.23.26/demo/demo-app/app/system-check.php
--rw-r--r--   0 lucjean    (501) staff       (20)      988 2019-08-29 13:07:38.000000 coop_html_editor-1.3.1/coop_html_editor/static/aloha.0.23.26/demo/demo-app/app/save-to-file.php
--rw-r--r--   0 lucjean    (501) staff       (20)        0 2019-08-29 13:07:38.000000 coop_html_editor-1.3.1/coop_html_editor/static/aloha.0.23.26/demo/demo-app/app/demo-app.log
--rw-r--r--   0 lucjean    (501) staff       (20)      693 2019-08-29 13:07:38.000000 coop_html_editor-1.3.1/coop_html_editor/static/aloha.0.23.26/demo/demo-app/app/read-from-session.php
--rw-r--r--   0 lucjean    (501) staff       (20)     2064 2019-08-29 13:07:38.000000 coop_html_editor-1.3.1/coop_html_editor/static/aloha.0.23.26/demo/demo-app/sitemap.html
--rw-r--r--   0 lucjean    (501) staff       (20)     2423 2019-08-29 13:07:38.000000 coop_html_editor-1.3.1/coop_html_editor/static/aloha.0.23.26/demo/demo-app/textarea.html
-drwxr-xr-x   0 lucjean    (501) staff       (20)        0 2019-08-30 10:39:38.000000 coop_html_editor-1.3.1/coop_html_editor/static/aloha.0.23.26/demo/demo-app/uploads/
--rw-r--r--   0 lucjean    (501) staff       (20)   356253 2019-08-29 13:07:38.000000 coop_html_editor-1.3.1/coop_html_editor/static/aloha.0.23.26/demo/demo-app/uploads/jQuery-1.6-Visual-Cheat-Sheet.pdf
--rw-r--r--   0 lucjean    (501) staff       (20)     9115 2019-08-29 13:07:38.000000 coop_html_editor-1.3.1/coop_html_editor/static/aloha.0.23.26/demo/demo-app/uploads/AlohaEditor-HTML5-technology-512.png
--rw-r--r--   0 lucjean    (501) staff       (20)  1110937 2019-08-29 13:07:38.000000 coop_html_editor-1.3.1/coop_html_editor/static/aloha.0.23.26/demo/demo-app/uploads/AlohaEditor-HTML5-WYSIWYG-about.pdf
--rw-r--r--   0 lucjean    (501) staff       (20)     7886 2019-08-29 13:07:38.000000 coop_html_editor-1.3.1/coop_html_editor/static/aloha.0.23.26/demo/demo-app/uploads/moby-dick.jpg
--rw-r--r--   0 lucjean    (501) staff       (20)     7853 2019-08-29 13:07:38.000000 coop_html_editor-1.3.1/coop_html_editor/static/aloha.0.23.26/demo/demo-app/uploads/AlohaEditor-HTML5-contenteditable-transparent-256.png
--rw-r--r--   0 lucjean    (501) staff       (20)     6801 2019-08-29 13:07:38.000000 coop_html_editor-1.3.1/coop_html_editor/static/aloha.0.23.26/demo/demo-app/mobydick.html
--rw-r--r--   0 lucjean    (501) staff       (20)      271 2019-08-29 13:07:37.000000 coop_html_editor-1.3.1/coop_html_editor/static/aloha.0.23.26/demo/demo-app/README.txt
-drwxr-xr-x   0 lucjean    (501) staff       (20)        0 2019-08-30 10:39:38.000000 coop_html_editor-1.3.1/coop_html_editor/static/aloha.0.23.26/demo/impress.js/
--rw-r--r--   0 lucjean    (501) staff       (20)     6239 2019-08-29 13:07:38.000000 coop_html_editor-1.3.1/coop_html_editor/static/aloha.0.23.26/demo/impress.js/index.html
-drwxr-xr-x   0 lucjean    (501) staff       (20)        0 2019-08-30 10:39:38.000000 coop_html_editor-1.3.1/coop_html_editor/static/aloha.0.23.26/demo/impress.js/app/
--rw-r--r--   0 lucjean    (501) staff       (20)      601 2019-08-29 13:07:38.000000 coop_html_editor-1.3.1/coop_html_editor/static/aloha.0.23.26/demo/impress.js/app/index.php
--rw-r--r--   0 lucjean    (501) staff       (20)      527 2019-08-29 13:07:38.000000 coop_html_editor-1.3.1/coop_html_editor/static/aloha.0.23.26/demo/impress.js/app/save-to-session.php
--rw-r--r--   0 lucjean    (501) staff       (20)      446 2019-08-29 13:07:38.000000 coop_html_editor-1.3.1/coop_html_editor/static/aloha.0.23.26/demo/impress.js/app/read-from-session.php
-drwxr-xr-x   0 lucjean    (501) staff       (20)        0 2019-08-30 10:39:38.000000 coop_html_editor-1.3.1/coop_html_editor/static/aloha.0.23.26/demo/impress.js/css/
--rw-r--r--   0 lucjean    (501) staff       (20)    12761 2019-08-29 13:07:38.000000 coop_html_editor-1.3.1/coop_html_editor/static/aloha.0.23.26/demo/impress.js/css/impress-demo.css
-drwxr-xr-x   0 lucjean    (501) staff       (20)        0 2019-08-30 10:39:38.000000 coop_html_editor-1.3.1/coop_html_editor/static/aloha.0.23.26/demo/impress.js/js/
--rw-r--r--   0 lucjean    (501) staff       (20)    10242 2019-08-29 13:07:38.000000 coop_html_editor-1.3.1/coop_html_editor/static/aloha.0.23.26/demo/impress.js/js/impress.js
--rw-r--r--   0 lucjean    (501) staff       (20)     2336 2019-08-29 13:07:38.000000 coop_html_editor-1.3.1/coop_html_editor/static/aloha.0.23.26/demo/impress.js/js/app.js
--rw-r--r--   0 lucjean    (501) staff       (20)      305 2019-08-29 13:07:38.000000 coop_html_editor-1.3.1/coop_html_editor/static/aloha.0.23.26/demo/impress.js/js/aloha-config.js
--rw-r--r--   0 lucjean    (501) staff       (20)     1518 2019-08-29 13:07:38.000000 coop_html_editor-1.3.1/coop_html_editor/static/aloha.0.23.26/demo/impress.js/README.md
-drwxr-xr-x   0 lucjean    (501) staff       (20)        0 2019-08-30 10:39:36.000000 coop_html_editor-1.3.1/coop_html_editor/static/aloha.0.23.26/demo/block/
--rw-r--r--   0 lucjean    (501) staff       (20)    24541 2019-08-29 13:07:37.000000 coop_html_editor-1.3.1/coop_html_editor/static/aloha.0.23.26/demo/block/index.html
--rw-r--r--   0 lucjean    (501) staff       (20)     6913 2019-08-29 13:07:37.000000 coop_html_editor-1.3.1/coop_html_editor/static/aloha.0.23.26/demo/block/dragdrop.html
--rw-r--r--   0 lucjean    (501) staff       (20)     3825 2019-08-29 13:07:37.000000 coop_html_editor-1.3.1/coop_html_editor/static/aloha.0.23.26/demo/block/index.css
-drwxr-xr-x   0 lucjean    (501) staff       (20)        0 2019-08-30 10:39:35.000000 coop_html_editor-1.3.1/coop_html_editor/static/aloha.0.23.26/demo/block/blockdemo/
-drwxr-xr-x   0 lucjean    (501) staff       (20)        0 2019-08-30 10:39:36.000000 coop_html_editor-1.3.1/coop_html_editor/static/aloha.0.23.26/demo/block/blockdemo/res/
--rw-r--r--   0 lucjean    (501) staff       (20)      546 2019-08-29 13:07:37.000000 coop_html_editor-1.3.1/coop_html_editor/static/aloha.0.23.26/demo/block/blockdemo/res/vcard.html
-drwxr-xr-x   0 lucjean    (501) staff       (20)        0 2019-08-30 10:39:36.000000 coop_html_editor-1.3.1/coop_html_editor/static/aloha.0.23.26/demo/block/blockdemo/css/
--rw-r--r--   0 lucjean    (501) staff       (20)     1117 2019-08-29 13:07:37.000000 coop_html_editor-1.3.1/coop_html_editor/static/aloha.0.23.26/demo/block/blockdemo/css/block.css
-drwxr-xr-x   0 lucjean    (501) staff       (20)        0 2019-08-30 10:39:36.000000 coop_html_editor-1.3.1/coop_html_editor/static/aloha.0.23.26/demo/block/blockdemo/img/
--rw-r--r--   0 lucjean    (501) staff       (20)     4627 2019-08-29 13:07:37.000000 coop_html_editor-1.3.1/coop_html_editor/static/aloha.0.23.26/demo/block/blockdemo/img/stock-quote-aapl.gif
--rw-r--r--   0 lucjean    (501) staff       (20)     3422 2019-08-29 13:07:37.000000 coop_html_editor-1.3.1/coop_html_editor/static/aloha.0.23.26/demo/block/blockdemo/img/stock-quote-msft.gif
-drwxr-xr-x   0 lucjean    (501) staff       (20)        0 2019-08-30 10:39:36.000000 coop_html_editor-1.3.1/coop_html_editor/static/aloha.0.23.26/demo/block/blockdemo/lib/
--rw-r--r--   0 lucjean    (501) staff       (20)     8545 2019-08-29 13:07:37.000000 coop_html_editor-1.3.1/coop_html_editor/static/aloha.0.23.26/demo/block/blockdemo/lib/block.js
--rw-r--r--   0 lucjean    (501) staff       (20)     2245 2019-08-29 13:07:37.000000 coop_html_editor-1.3.1/coop_html_editor/static/aloha.0.23.26/demo/block/blockdemo/lib/blockdemo-plugin.js
-drwxr-xr-x   0 lucjean    (501) staff       (20)        0 2019-08-30 10:39:36.000000 coop_html_editor-1.3.1/coop_html_editor/static/aloha.0.23.26/demo/block/blockdemo/vendor/
--rw-r--r--   0 lucjean    (501) staff       (20)    28078 2019-08-29 13:07:37.000000 coop_html_editor-1.3.1/coop_html_editor/static/aloha.0.23.26/demo/block/blockdemo/vendor/underscore.js
-drwxr-xr-x   0 lucjean    (501) staff       (20)        0 2019-08-30 10:39:36.000000 coop_html_editor-1.3.1/coop_html_editor/static/aloha.0.23.26/css/
--rw-r--r--   0 lucjean    (501) staff       (20)      380 2019-08-29 13:07:37.000000 coop_html_editor-1.3.1/coop_html_editor/static/aloha.0.23.26/css/aloha-core.css
--rw-r--r--   0 lucjean    (501) staff       (20)     1204 2019-08-29 13:07:37.000000 coop_html_editor-1.3.1/coop_html_editor/static/aloha.0.23.26/css/aloha-common-extra.css
--rw-r--r--   0 lucjean    (501) staff       (20)    72377 2019-08-29 13:07:37.000000 coop_html_editor-1.3.1/coop_html_editor/static/aloha.0.23.26/css/aloha.css
--rw-r--r--   0 lucjean    (501) staff       (20)     7095 2019-08-29 13:07:37.000000 coop_html_editor-1.3.1/coop_html_editor/static/aloha.0.23.26/css/aloha-sidebar.css
--rw-r--r--   0 lucjean    (501) staff       (20)      575 2019-08-29 13:07:37.000000 coop_html_editor-1.3.1/coop_html_editor/static/aloha.0.23.26/css/aloha-reset.css
-drwxr-xr-x   0 lucjean    (501) staff       (20)        0 2019-08-30 10:39:35.000000 coop_html_editor-1.3.1/coop_html_editor/static/aloha.0.23.26/plugins/
-drwxr-xr-x   0 lucjean    (501) staff       (20)        0 2019-08-30 10:39:35.000000 coop_html_editor-1.3.1/coop_html_editor/static/aloha.0.23.26/plugins/common/
-drwxr-xr-x   0 lucjean    (501) staff       (20)        0 2019-08-30 10:39:35.000000 coop_html_editor-1.3.1/coop_html_editor/static/aloha.0.23.26/plugins/common/ui/
-drwxr-xr-x   0 lucjean    (501) staff       (20)        0 2019-08-30 10:39:41.000000 coop_html_editor-1.3.1/coop_html_editor/static/aloha.0.23.26/plugins/common/ui/css/
--rw-r--r--   0 lucjean    (501) staff       (20)    25956 2019-08-29 13:07:39.000000 coop_html_editor-1.3.1/coop_html_editor/static/aloha.0.23.26/plugins/common/ui/css/ui.css
--rw-r--r--   0 lucjean    (501) staff       (20)    26175 2019-08-29 13:07:39.000000 coop_html_editor-1.3.1/coop_html_editor/static/aloha.0.23.26/plugins/common/ui/css/jquery-ui-1.9m6.css
-drwxr-xr-x   0 lucjean    (501) staff       (20)        0 2019-08-30 10:39:35.000000 coop_html_editor-1.3.1/coop_html_editor/static/aloha.0.23.26/plugins/common/ui/nls/
-drwxr-xr-x   0 lucjean    (501) staff       (20)        0 2019-08-30 10:39:42.000000 coop_html_editor-1.3.1/coop_html_editor/static/aloha.0.23.26/plugins/common/ui/nls/zh-hans/
--rw-r--r--   0 lucjean    (501) staff       (20)     1723 2019-08-29 13:07:39.000000 coop_html_editor-1.3.1/coop_html_editor/static/aloha.0.23.26/plugins/common/ui/nls/zh-hans/i18n.js
-drwxr-xr-x   0 lucjean    (501) staff       (20)        0 2019-08-30 10:39:42.000000 coop_html_editor-1.3.1/coop_html_editor/static/aloha.0.23.26/plugins/common/ui/nls/ca/
--rw-r--r--   0 lucjean    (501) staff       (20)     1982 2019-08-29 13:07:39.000000 coop_html_editor-1.3.1/coop_html_editor/static/aloha.0.23.26/plugins/common/ui/nls/ca/i18n.js
-drwxr-xr-x   0 lucjean    (501) staff       (20)        0 2019-08-30 10:39:42.000000 coop_html_editor-1.3.1/coop_html_editor/static/aloha.0.23.26/plugins/common/ui/nls/ru/
--rw-r--r--   0 lucjean    (501) staff       (20)     2573 2019-08-29 13:07:39.000000 coop_html_editor-1.3.1/coop_html_editor/static/aloha.0.23.26/plugins/common/ui/nls/ru/i18n.js
-drwxr-xr-x   0 lucjean    (501) staff       (20)        0 2019-08-30 10:39:42.000000 coop_html_editor-1.3.1/coop_html_editor/static/aloha.0.23.26/plugins/common/ui/nls/uk/
--rw-r--r--   0 lucjean    (501) staff       (20)     2547 2019-08-29 13:07:39.000000 coop_html_editor-1.3.1/coop_html_editor/static/aloha.0.23.26/plugins/common/ui/nls/uk/i18n.js
-drwxr-xr-x   0 lucjean    (501) staff       (20)        0 2019-08-30 10:39:42.000000 coop_html_editor-1.3.1/coop_html_editor/static/aloha.0.23.26/plugins/common/ui/nls/mk/
--rw-r--r--   0 lucjean    (501) staff       (20)     2467 2019-08-29 13:07:39.000000 coop_html_editor-1.3.1/coop_html_editor/static/aloha.0.23.26/plugins/common/ui/nls/mk/i18n.js
-drwxr-xr-x   0 lucjean    (501) staff       (20)        0 2019-08-30 10:39:42.000000 coop_html_editor-1.3.1/coop_html_editor/static/aloha.0.23.26/plugins/common/ui/nls/pt-br/
--rw-r--r--   0 lucjean    (501) staff       (20)     1894 2019-08-29 13:07:39.000000 coop_html_editor-1.3.1/coop_html_editor/static/aloha.0.23.26/plugins/common/ui/nls/pt-br/i18n.js
-drwxr-xr-x   0 lucjean    (501) staff       (20)        0 2019-08-30 10:39:42.000000 coop_html_editor-1.3.1/coop_html_editor/static/aloha.0.23.26/plugins/common/ui/nls/de/
--rw-r--r--   0 lucjean    (501) staff       (20)     1990 2019-08-29 13:07:39.000000 coop_html_editor-1.3.1/coop_html_editor/static/aloha.0.23.26/plugins/common/ui/nls/de/i18n.js
-drwxr-xr-x   0 lucjean    (501) staff       (20)        0 2019-08-30 10:39:42.000000 coop_html_editor-1.3.1/coop_html_editor/static/aloha.0.23.26/plugins/common/ui/img/
--rw-r--r--   0 lucjean    (501) staff       (20)      698 2019-08-29 13:07:39.000000 coop_html_editor-1.3.1/coop_html_editor/static/aloha.0.23.26/plugins/common/ui/img/blockquote.png
-drwxr-xr-x   0 lucjean    (501) staff       (20)        0 2019-08-30 10:39:42.000000 coop_html_editor-1.3.1/coop_html_editor/static/aloha.0.23.26/plugins/common/ui/img/jqueryui/
--rw-r--r--   0 lucjean    (501) staff       (20)     3702 2019-08-29 13:07:39.000000 coop_html_editor-1.3.1/coop_html_editor/static/aloha.0.23.26/plugins/common/ui/img/jqueryui/ui-icons_222222_256x240.png
--rw-r--r--   0 lucjean    (501) staff       (20)      288 2019-08-29 13:07:39.000000 coop_html_editor-1.3.1/coop_html_editor/static/aloha.0.23.26/plugins/common/ui/img/outdent.png
--rw-r--r--   0 lucjean    (501) staff       (20)      849 2019-08-29 13:07:39.000000 coop_html_editor-1.3.1/coop_html_editor/static/aloha.0.23.26/plugins/common/ui/img/language-annotation.png
--rw-r--r--   0 lucjean    (501) staff       (20)      290 2019-08-29 13:07:39.000000 coop_html_editor-1.3.1/coop_html_editor/static/aloha.0.23.26/plugins/common/ui/img/indent.png
--rw-r--r--   0 lucjean    (501) staff       (20)      226 2019-08-29 13:07:39.000000 coop_html_editor-1.3.1/coop_html_editor/static/aloha.0.23.26/plugins/common/ui/img/character-picker.png
--rw-r--r--   0 lucjean    (501) staff       (20)     5832 2019-08-29 13:07:39.000000 coop_html_editor-1.3.1/coop_html_editor/static/aloha.0.23.26/plugins/common/ui/img/format-inline.png
--rw-r--r--   0 lucjean    (501) staff       (20)      178 2019-08-29 13:07:39.000000 coop_html_editor-1.3.1/coop_html_editor/static/aloha.0.23.26/plugins/common/ui/img/em.png
--rw-r--r--   0 lucjean    (501) staff       (20)      207 2019-08-29 13:07:39.000000 coop_html_editor-1.3.1/coop_html_editor/static/aloha.0.23.26/plugins/common/ui/img/multisplit-open.gif
--rw-r--r--   0 lucjean    (501) staff       (20)      210 2019-08-29 13:07:39.000000 coop_html_editor-1.3.1/coop_html_editor/static/aloha.0.23.26/plugins/common/ui/img/multisplit-close.gif
--rw-r--r--   0 lucjean    (501) staff       (20)      135 2019-08-29 13:07:39.000000 coop_html_editor-1.3.1/coop_html_editor/static/aloha.0.23.26/plugins/common/ui/img/metaview.png
--rw-r--r--   0 lucjean    (501) staff       (20)     2492 2019-08-29 13:07:39.000000 coop_html_editor-1.3.1/coop_html_editor/static/aloha.0.23.26/plugins/common/ui/img/format-block.png
-drwxr-xr-x   0 lucjean    (501) staff       (20)        0 2019-08-30 10:39:42.000000 coop_html_editor-1.3.1/coop_html_editor/static/aloha.0.23.26/plugins/common/ui/img/metaview/
--rw-r--r--   0 lucjean    (501) staff       (20)      135 2019-08-29 13:07:39.000000 coop_html_editor-1.3.1/coop_html_editor/static/aloha.0.23.26/plugins/common/ui/img/metaview/blockquote.png
--rw-r--r--   0 lucjean    (501) staff       (20)       87 2019-08-29 13:07:39.000000 coop_html_editor-1.3.1/coop_html_editor/static/aloha.0.23.26/plugins/common/ui/img/metaview/td.png
--rw-r--r--   0 lucjean    (501) staff       (20)      122 2019-08-29 13:07:39.000000 coop_html_editor-1.3.1/coop_html_editor/static/aloha.0.23.26/plugins/common/ui/img/metaview/pre.png
--rw-r--r--   0 lucjean    (501) staff       (20)       99 2019-08-29 13:07:39.000000 coop_html_editor-1.3.1/coop_html_editor/static/aloha.0.23.26/plugins/common/ui/img/metaview/div.png
--rw-r--r--   0 lucjean    (501) staff       (20)       86 2019-08-29 13:07:39.000000 coop_html_editor-1.3.1/coop_html_editor/static/aloha.0.23.26/plugins/common/ui/img/metaview/dl.png
--rw-r--r--   0 lucjean    (501) staff       (20)      116 2019-08-29 13:07:39.000000 coop_html_editor-1.3.1/coop_html_editor/static/aloha.0.23.26/plugins/common/ui/img/metaview/h5.png
--rw-r--r--   0 lucjean    (501) staff       (20)      115 2019-08-29 13:07:39.000000 coop_html_editor-1.3.1/coop_html_editor/static/aloha.0.23.26/plugins/common/ui/img/metaview/h4.png
--rw-r--r--   0 lucjean    (501) staff       (20)      116 2019-08-29 13:07:39.000000 coop_html_editor-1.3.1/coop_html_editor/static/aloha.0.23.26/plugins/common/ui/img/metaview/h6.png
--rw-r--r--   0 lucjean    (501) staff       (20)       87 2019-08-29 13:07:39.000000 coop_html_editor-1.3.1/coop_html_editor/static/aloha.0.23.26/plugins/common/ui/img/metaview/dt.png
--rw-r--r--   0 lucjean    (501) staff       (20)      395 2019-08-29 13:07:39.000000 coop_html_editor-1.3.1/coop_html_editor/static/aloha.0.23.26/plugins/common/ui/img/metaview/cite.png
--rw-r--r--   0 lucjean    (501) staff       (20)      114 2019-08-29 13:07:39.000000 coop_html_editor-1.3.1/coop_html_editor/static/aloha.0.23.26/plugins/common/ui/img/metaview/h3.png
--rw-r--r--   0 lucjean    (501) staff       (20)      116 2019-08-29 13:07:39.000000 coop_html_editor-1.3.1/coop_html_editor/static/aloha.0.23.26/plugins/common/ui/img/metaview/h2.png
--rw-r--r--   0 lucjean    (501) staff       (20)       87 2019-08-29 13:07:39.000000 coop_html_editor-1.3.1/coop_html_editor/static/aloha.0.23.26/plugins/common/ui/img/metaview/dd.png
--rw-r--r--   0 lucjean    (501) staff       (20)      111 2019-08-29 13:07:39.000000 coop_html_editor-1.3.1/coop_html_editor/static/aloha.0.23.26/plugins/common/ui/img/metaview/h1.png
--rw-r--r--   0 lucjean    (501) staff       (20)      213 2019-08-29 13:07:39.000000 coop_html_editor-1.3.1/coop_html_editor/static/aloha.0.23.26/plugins/common/ui/img/metaview/anchor.png
--rw-r--r--   0 lucjean    (501) staff       (20)       91 2019-08-29 13:07:39.000000 coop_html_editor-1.3.1/coop_html_editor/static/aloha.0.23.26/plugins/common/ui/img/metaview/th.png
--rw-r--r--   0 lucjean    (501) staff       (20)      122 2019-08-29 13:07:39.000000 coop_html_editor-1.3.1/coop_html_editor/static/aloha.0.23.26/plugins/common/ui/img/metaview/caption.png
--rw-r--r--   0 lucjean    (501) staff       (20)      116 2019-08-29 13:07:39.000000 coop_html_editor-1.3.1/coop_html_editor/static/aloha.0.23.26/plugins/common/ui/img/metaview/table.png
--rw-r--r--   0 lucjean    (501) staff       (20)      113 2019-08-29 13:07:39.000000 coop_html_editor-1.3.1/coop_html_editor/static/aloha.0.23.26/plugins/common/ui/img/metaview/p.png
--rw-r--r--   0 lucjean    (501) staff       (20)      241 2019-08-29 13:07:39.000000 coop_html_editor-1.3.1/coop_html_editor/static/aloha.0.23.26/plugins/common/ui/img/metaview/q.png
--rw-r--r--   0 lucjean    (501) staff       (20)      206 2019-08-29 13:07:39.000000 coop_html_editor-1.3.1/coop_html_editor/static/aloha.0.23.26/plugins/common/ui/img/strong.png
--rw-r--r--   0 lucjean    (501) staff       (20)      128 2019-08-29 13:07:39.000000 coop_html_editor-1.3.1/coop_html_editor/static/aloha.0.23.26/plugins/common/ui/img/justify.png
--rw-r--r--   0 lucjean    (501) staff       (20)      241 2019-08-29 13:07:39.000000 coop_html_editor-1.3.1/coop_html_editor/static/aloha.0.23.26/plugins/common/ui/img/quote.png
--rw-r--r--   0 lucjean    (501) staff       (20)      649 2019-08-29 13:07:39.000000 coop_html_editor-1.3.1/coop_html_editor/static/aloha.0.23.26/plugins/common/ui/img/tree.png
--rw-r--r--   0 lucjean    (501) staff       (20)      193 2019-08-29 13:07:39.000000 coop_html_editor-1.3.1/coop_html_editor/static/aloha.0.23.26/plugins/common/ui/img/removeformat.png
-drwxr-xr-x   0 lucjean    (501) staff       (20)        0 2019-08-30 10:39:42.000000 coop_html_editor-1.3.1/coop_html_editor/static/aloha.0.23.26/plugins/common/ui/lib/
--rw-r--r--   0 lucjean    (501) staff       (20)     1560 2019-08-29 13:07:39.000000 coop_html_editor-1.3.1/coop_html_editor/static/aloha.0.23.26/plugins/common/ui/lib/autocomplete.js
--rw-r--r--   0 lucjean    (501) staff       (20)      247 2019-08-29 13:07:39.000000 coop_html_editor-1.3.1/coop_html_editor/static/aloha.0.23.26/plugins/common/ui/lib/arena.js
--rw-r--r--   0 lucjean    (501) staff       (20)      613 2019-08-29 13:07:39.000000 coop_html_editor-1.3.1/coop_html_editor/static/aloha.0.23.26/plugins/common/ui/lib/text.js
-drwxr-xr-x   0 lucjean    (501) staff       (20)        0 2019-08-30 10:39:35.000000 coop_html_editor-1.3.1/coop_html_editor/static/aloha.0.23.26/plugins/common/characterpicker/
-drwxr-xr-x   0 lucjean    (501) staff       (20)        0 2019-08-30 10:39:39.000000 coop_html_editor-1.3.1/coop_html_editor/static/aloha.0.23.26/plugins/common/characterpicker/css/
--rw-r--r--   0 lucjean    (501) staff       (20)      764 2019-08-29 13:07:38.000000 coop_html_editor-1.3.1/coop_html_editor/static/aloha.0.23.26/plugins/common/characterpicker/css/characterpicker.css
-drwxr-xr-x   0 lucjean    (501) staff       (20)        0 2019-08-30 10:39:35.000000 coop_html_editor-1.3.1/coop_html_editor/static/aloha.0.23.26/plugins/common/characterpicker/nls/
-drwxr-xr-x   0 lucjean    (501) staff       (20)        0 2019-08-30 10:39:40.000000 coop_html_editor-1.3.1/coop_html_editor/static/aloha.0.23.26/plugins/common/characterpicker/nls/zh-hans/
--rw-r--r--   0 lucjean    (501) staff       (20)       66 2019-08-29 13:07:38.000000 coop_html_editor-1.3.1/coop_html_editor/static/aloha.0.23.26/plugins/common/characterpicker/nls/zh-hans/i18n.js
-drwxr-xr-x   0 lucjean    (501) staff       (20)        0 2019-08-30 10:39:40.000000 coop_html_editor-1.3.1/coop_html_editor/static/aloha.0.23.26/plugins/common/characterpicker/nls/ca/
--rw-r--r--   0 lucjean    (501) staff       (20)       78 2019-08-29 13:07:38.000000 coop_html_editor-1.3.1/coop_html_editor/static/aloha.0.23.26/plugins/common/characterpicker/nls/ca/i18n.js
-drwxr-xr-x   0 lucjean    (501) staff       (20)        0 2019-08-30 10:39:40.000000 coop_html_editor-1.3.1/coop_html_editor/static/aloha.0.23.26/plugins/common/characterpicker/nls/ru/
--rw-r--r--   0 lucjean    (501) staff       (20)       83 2019-08-29 13:07:38.000000 coop_html_editor-1.3.1/coop_html_editor/static/aloha.0.23.26/plugins/common/characterpicker/nls/ru/i18n.js
-drwxr-xr-x   0 lucjean    (501) staff       (20)        0 2019-08-30 10:39:40.000000 coop_html_editor-1.3.1/coop_html_editor/static/aloha.0.23.26/plugins/common/characterpicker/nls/uk/
--rw-r--r--   0 lucjean    (501) staff       (20)       83 2019-08-29 13:07:38.000000 coop_html_editor-1.3.1/coop_html_editor/static/aloha.0.23.26/plugins/common/characterpicker/nls/uk/i18n.js
-drwxr-xr-x   0 lucjean    (501) staff       (20)        0 2019-08-30 10:39:40.000000 coop_html_editor-1.3.1/coop_html_editor/static/aloha.0.23.26/plugins/common/characterpicker/nls/mk/
--rw-r--r--   0 lucjean    (501) staff       (20)      100 2019-08-29 13:07:38.000000 coop_html_editor-1.3.1/coop_html_editor/static/aloha.0.23.26/plugins/common/characterpicker/nls/mk/i18n.js
-drwxr-xr-x   0 lucjean    (501) staff       (20)        0 2019-08-30 10:39:40.000000 coop_html_editor-1.3.1/coop_html_editor/static/aloha.0.23.26/plugins/common/characterpicker/nls/pt-br/
--rw-r--r--   0 lucjean    (501) staff       (20)       77 2019-08-29 13:07:38.000000 coop_html_editor-1.3.1/coop_html_editor/static/aloha.0.23.26/plugins/common/characterpicker/nls/pt-br/i18n.js
-drwxr-xr-x   0 lucjean    (501) staff       (20)        0 2019-08-30 10:39:40.000000 coop_html_editor-1.3.1/coop_html_editor/static/aloha.0.23.26/plugins/common/characterpicker/nls/de/
--rw-r--r--   0 lucjean    (501) staff       (20)       69 2019-08-29 13:07:38.000000 coop_html_editor-1.3.1/coop_html_editor/static/aloha.0.23.26/plugins/common/characterpicker/nls/de/i18n.js
-drwxr-xr-x   0 lucjean    (501) staff       (20)        0 2019-08-30 10:39:40.000000 coop_html_editor-1.3.1/coop_html_editor/static/aloha.0.23.26/plugins/common/characterpicker/img/
--rw-r--r--   0 lucjean    (501) staff       (20)      226 2019-08-29 13:07:38.000000 coop_html_editor-1.3.1/coop_html_editor/static/aloha.0.23.26/plugins/common/characterpicker/img/icon.png
-drwxr-xr-x   0 lucjean    (501) staff       (20)        0 2019-08-30 10:39:40.000000 coop_html_editor-1.3.1/coop_html_editor/static/aloha.0.23.26/plugins/common/highlighteditables/
-drwxr-xr-x   0 lucjean    (501) staff       (20)        0 2019-08-30 10:39:40.000000 coop_html_editor-1.3.1/coop_html_editor/static/aloha.0.23.26/plugins/common/highlighteditables/css/
--rw-r--r--   0 lucjean    (501) staff       (20)      362 2019-08-29 13:07:38.000000 coop_html_editor-1.3.1/coop_html_editor/static/aloha.0.23.26/plugins/common/highlighteditables/css/highlighteditables.css
--rw-r--r--   0 lucjean    (501) staff       (20)        3 2019-08-29 13:07:38.000000 coop_html_editor-1.3.1/coop_html_editor/static/aloha.0.23.26/plugins/common/highlighteditables/package.json
-drwxr-xr-x   0 lucjean    (501) staff       (20)        0 2019-08-30 10:39:40.000000 coop_html_editor-1.3.1/coop_html_editor/static/aloha.0.23.26/plugins/common/contenthandler/
--rw-r--r--   0 lucjean    (501) staff       (20)        0 2019-08-29 13:07:38.000000 coop_html_editor-1.3.1/coop_html_editor/static/aloha.0.23.26/plugins/common/contenthandler/README.md
--rw-r--r--   0 lucjean    (501) staff       (20)        2 2019-08-29 13:07:38.000000 coop_html_editor-1.3.1/coop_html_editor/static/aloha.0.23.26/plugins/common/contenthandler/package.json
-drwxr-xr-x   0 lucjean    (501) staff       (20)        0 2019-08-30 10:39:40.000000 coop_html_editor-1.3.1/coop_html_editor/static/aloha.0.23.26/plugins/common/contenthandler/lib/
--rw-r--r--   0 lucjean    (501) staff       (20)    18160 2019-08-29 13:07:38.000000 coop_html_editor-1.3.1/coop_html_editor/static/aloha.0.23.26/plugins/common/contenthandler/lib/oembedcontenthandler.js
-drwxr-xr-x   0 lucjean    (501) staff       (20)        0 2019-08-30 10:39:42.000000 coop_html_editor-1.3.1/coop_html_editor/static/aloha.0.23.26/plugins/common/undo/
-drwxr-xr-x   0 lucjean    (501) staff       (20)        0 2019-08-30 10:39:42.000000 coop_html_editor-1.3.1/coop_html_editor/static/aloha.0.23.26/plugins/common/undo/demo/
--rw-r--r--   0 lucjean    (501) staff       (20)     4156 2019-08-29 13:07:39.000000 coop_html_editor-1.3.1/coop_html_editor/static/aloha.0.23.26/plugins/common/undo/demo/index.html
--rw-r--r--   0 lucjean    (501) staff       (20)      787 2019-08-29 13:07:39.000000 coop_html_editor-1.3.1/coop_html_editor/static/aloha.0.23.26/plugins/common/undo/demo/index.css
--rw-r--r--   0 lucjean    (501) staff       (20)       91 2019-08-29 13:07:39.000000 coop_html_editor-1.3.1/coop_html_editor/static/aloha.0.23.26/plugins/common/undo/package.json
-drwxr-xr-x   0 lucjean    (501) staff       (20)        0 2019-08-30 10:39:42.000000 coop_html_editor-1.3.1/coop_html_editor/static/aloha.0.23.26/plugins/common/undo/lib/
--rw-r--r--   0 lucjean    (501) staff       (20)     5059 2019-08-29 13:07:39.000000 coop_html_editor-1.3.1/coop_html_editor/static/aloha.0.23.26/plugins/common/undo/lib/undo-plugin.js
-drwxr-xr-x   0 lucjean    (501) staff       (20)        0 2019-08-30 10:39:42.000000 coop_html_editor-1.3.1/coop_html_editor/static/aloha.0.23.26/plugins/common/undo/vendor/
--rw-r--r--   0 lucjean    (501) staff       (20)    74554 2019-08-29 13:07:39.000000 coop_html_editor-1.3.1/coop_html_editor/static/aloha.0.23.26/plugins/common/undo/vendor/diff_match_patch_uncompressed.js
--rw-r--r--   0 lucjean    (501) staff       (20)     2377 2019-08-29 13:07:39.000000 coop_html_editor-1.3.1/coop_html_editor/static/aloha.0.23.26/plugins/common/undo/vendor/undo.js
-drwxr-xr-x   0 lucjean    (501) staff       (20)        0 2019-08-30 10:39:40.000000 coop_html_editor-1.3.1/coop_html_editor/static/aloha.0.23.26/plugins/common/image/
-drwxr-xr-x   0 lucjean    (501) staff       (20)        0 2019-08-30 10:39:40.000000 coop_html_editor-1.3.1/coop_html_editor/static/aloha.0.23.26/plugins/common/image/demo/
--rw-r--r--   0 lucjean    (501) staff       (20)     3393 2019-08-29 13:07:39.000000 coop_html_editor-1.3.1/coop_html_editor/static/aloha.0.23.26/plugins/common/image/demo/index.html
--rw-r--r--   0 lucjean    (501) staff       (20)    74949 2019-08-29 13:07:39.000000 coop_html_editor-1.3.1/coop_html_editor/static/aloha.0.23.26/plugins/common/image/demo/cropnresize.jpg
--rw-r--r--   0 lucjean    (501) staff       (20)      537 2019-08-29 13:07:39.000000 coop_html_editor-1.3.1/coop_html_editor/static/aloha.0.23.26/plugins/common/image/demo/crop.php
--rw-r--r--   0 lucjean    (501) staff       (20)     2865 2019-08-29 13:07:39.000000 coop_html_editor-1.3.1/coop_html_editor/static/aloha.0.23.26/plugins/common/image/demo/crop.html
-drwxr-xr-x   0 lucjean    (501) staff       (20)        0 2019-08-30 10:39:40.000000 coop_html_editor-1.3.1/coop_html_editor/static/aloha.0.23.26/plugins/common/image/test/
--rw-r--r--   0 lucjean    (501) staff       (20)      991 2019-08-29 13:07:39.000000 coop_html_editor-1.3.1/coop_html_editor/static/aloha.0.23.26/plugins/common/image/test/test.html
--rw-r--r--   0 lucjean    (501) staff       (20)      206 2019-08-29 13:07:39.000000 coop_html_editor-1.3.1/coop_html_editor/static/aloha.0.23.26/plugins/common/image/test/test.css
-drwxr-xr-x   0 lucjean    (501) staff       (20)        0 2019-08-30 10:39:40.000000 coop_html_editor-1.3.1/coop_html_editor/static/aloha.0.23.26/plugins/common/image/css/
--rw-r--r--   0 lucjean    (501) staff       (20)     2815 2019-08-29 13:07:39.000000 coop_html_editor-1.3.1/coop_html_editor/static/aloha.0.23.26/plugins/common/image/css/image.css
-drwxr-xr-x   0 lucjean    (501) staff       (20)        0 2019-08-30 10:39:35.000000 coop_html_editor-1.3.1/coop_html_editor/static/aloha.0.23.26/plugins/common/image/nls/
-drwxr-xr-x   0 lucjean    (501) staff       (20)        0 2019-08-30 10:39:40.000000 coop_html_editor-1.3.1/coop_html_editor/static/aloha.0.23.26/plugins/common/image/nls/zh-hans/
--rw-r--r--   0 lucjean    (501) staff       (20)     1027 2019-08-29 13:07:39.000000 coop_html_editor-1.3.1/coop_html_editor/static/aloha.0.23.26/plugins/common/image/nls/zh-hans/i18n.js
-drwxr-xr-x   0 lucjean    (501) staff       (20)        0 2019-08-30 10:39:40.000000 coop_html_editor-1.3.1/coop_html_editor/static/aloha.0.23.26/plugins/common/image/nls/ca/
--rw-r--r--   0 lucjean    (501) staff       (20)     1191 2019-08-29 13:07:39.000000 coop_html_editor-1.3.1/coop_html_editor/static/aloha.0.23.26/plugins/common/image/nls/ca/i18n.js
-drwxr-xr-x   0 lucjean    (501) staff       (20)        0 2019-08-30 10:39:40.000000 coop_html_editor-1.3.1/coop_html_editor/static/aloha.0.23.26/plugins/common/image/nls/ru/
--rw-r--r--   0 lucjean    (501) staff       (20)     1615 2019-08-29 13:07:39.000000 coop_html_editor-1.3.1/coop_html_editor/static/aloha.0.23.26/plugins/common/image/nls/ru/i18n.js
-drwxr-xr-x   0 lucjean    (501) staff       (20)        0 2019-08-30 10:39:40.000000 coop_html_editor-1.3.1/coop_html_editor/static/aloha.0.23.26/plugins/common/image/nls/uk/
--rw-r--r--   0 lucjean    (501) staff       (20)     1569 2019-08-29 13:07:39.000000 coop_html_editor-1.3.1/coop_html_editor/static/aloha.0.23.26/plugins/common/image/nls/uk/i18n.js
-drwxr-xr-x   0 lucjean    (501) staff       (20)        0 2019-08-30 10:39:40.000000 coop_html_editor-1.3.1/coop_html_editor/static/aloha.0.23.26/plugins/common/image/nls/mk/
--rw-r--r--   0 lucjean    (501) staff       (20)     1491 2019-08-29 13:07:39.000000 coop_html_editor-1.3.1/coop_html_editor/static/aloha.0.23.26/plugins/common/image/nls/mk/i18n.js
-drwxr-xr-x   0 lucjean    (501) staff       (20)        0 2019-08-30 10:39:40.000000 coop_html_editor-1.3.1/coop_html_editor/static/aloha.0.23.26/plugins/common/image/nls/pt-br/
--rw-r--r--   0 lucjean    (501) staff       (20)     1161 2019-08-29 13:07:39.000000 coop_html_editor-1.3.1/coop_html_editor/static/aloha.0.23.26/plugins/common/image/nls/pt-br/i18n.js
-drwxr-xr-x   0 lucjean    (501) staff       (20)        0 2019-08-30 10:39:40.000000 coop_html_editor-1.3.1/coop_html_editor/static/aloha.0.23.26/plugins/common/image/nls/de/
--rw-r--r--   0 lucjean    (501) staff       (20)     1144 2019-08-29 13:07:39.000000 coop_html_editor-1.3.1/coop_html_editor/static/aloha.0.23.26/plugins/common/image/nls/de/i18n.js
--rw-r--r--   0 lucjean    (501) staff       (20)     2545 2019-08-29 13:07:39.000000 coop_html_editor-1.3.1/coop_html_editor/static/aloha.0.23.26/plugins/common/image/README.md
-drwxr-xr-x   0 lucjean    (501) staff       (20)        0 2019-08-30 10:39:40.000000 coop_html_editor-1.3.1/coop_html_editor/static/aloha.0.23.26/plugins/common/image/img/
--rw-r--r--   0 lucjean    (501) staff       (20)     1259 2019-08-29 13:07:39.000000 coop_html_editor-1.3.1/coop_html_editor/static/aloha.0.23.26/plugins/common/image/img/cropnresize.png
--rw-r--r--   0 lucjean    (501) staff       (20)      556 2019-08-29 13:07:39.000000 coop_html_editor-1.3.1/coop_html_editor/static/aloha.0.23.26/plugins/common/image/img/image-title.png
--rw-r--r--   0 lucjean    (501) staff       (20)      241 2019-08-29 13:07:39.000000 coop_html_editor-1.3.1/coop_html_editor/static/aloha.0.23.26/plugins/common/image/img/size-increase.gif
--rw-r--r--   0 lucjean    (501) staff       (20)      685 2019-08-29 13:07:39.000000 coop_html_editor-1.3.1/coop_html_editor/static/aloha.0.23.26/plugins/common/image/img/blank.jpg
--rw-r--r--   0 lucjean    (501) staff       (20)      345 2019-08-29 13:07:39.000000 coop_html_editor-1.3.1/coop_html_editor/static/aloha.0.23.26/plugins/common/image/img/size-decrease.gif
--rw-r--r--   0 lucjean    (501) staff       (20)      613 2019-08-29 13:07:39.000000 coop_html_editor-1.3.1/coop_html_editor/static/aloha.0.23.26/plugins/common/image/img/image.gif
--rw-r--r--   0 lucjean    (501) staff       (20)      856 2019-08-29 13:07:39.000000 coop_html_editor-1.3.1/coop_html_editor/static/aloha.0.23.26/plugins/common/image/img/crop-buttons.gif
--rw-r--r--   0 lucjean    (501) staff       (20)      666 2019-08-29 13:07:39.000000 coop_html_editor-1.3.1/coop_html_editor/static/aloha.0.23.26/plugins/common/image/img/image-align-right.png
--rw-r--r--   0 lucjean    (501) staff       (20)      358 2019-08-29 13:07:39.000000 coop_html_editor-1.3.1/coop_html_editor/static/aloha.0.23.26/plugins/common/image/img/padding-decrease.gif
--rw-r--r--   0 lucjean    (501) staff       (20)      614 2019-08-29 13:07:39.000000 coop_html_editor-1.3.1/coop_html_editor/static/aloha.0.23.26/plugins/common/image/img/handle-sw.png
--rw-r--r--   0 lucjean    (501) staff       (20)      630 2019-08-29 13:07:39.000000 coop_html_editor-1.3.1/coop_html_editor/static/aloha.0.23.26/plugins/common/image/img/image-align-none.png
--rw-r--r--   0 lucjean    (501) staff       (20)      358 2019-08-29 13:07:39.000000 coop_html_editor-1.3.1/coop_html_editor/static/aloha.0.23.26/plugins/common/image/img/padding-increase.gif
--rw-r--r--   0 lucjean    (501) staff       (20)      204 2019-08-29 13:07:39.000000 coop_html_editor-1.3.1/coop_html_editor/static/aloha.0.23.26/plugins/common/image/img/image-border.png
--rw-r--r--   0 lucjean    (501) staff       (20)      582 2019-08-29 13:07:39.000000 coop_html_editor-1.3.1/coop_html_editor/static/aloha.0.23.26/plugins/common/image/img/page.png
--rw-r--r--   0 lucjean    (501) staff       (20)      697 2019-08-29 13:07:39.000000 coop_html_editor-1.3.1/coop_html_editor/static/aloha.0.23.26/plugins/common/image/img/image-align-left.png
--rw-r--r--   0 lucjean    (501) staff       (20)        3 2019-08-29 13:07:39.000000 coop_html_editor-1.3.1/coop_html_editor/static/aloha.0.23.26/plugins/common/image/package.json
-drwxr-xr-x   0 lucjean    (501) staff       (20)        0 2019-08-30 10:39:40.000000 coop_html_editor-1.3.1/coop_html_editor/static/aloha.0.23.26/plugins/common/image/lib/
--rw-r--r--   0 lucjean    (501) staff       (20)        0 2019-08-29 13:07:39.000000 coop_html_editor-1.3.1/coop_html_editor/static/aloha.0.23.26/plugins/common/image/lib/image-plugin-actions.js
-drwxr-xr-x   0 lucjean    (501) staff       (20)        0 2019-08-30 10:39:35.000000 coop_html_editor-1.3.1/coop_html_editor/static/aloha.0.23.26/plugins/common/image/vendor/
-drwxr-xr-x   0 lucjean    (501) staff       (20)        0 2019-08-30 10:39:35.000000 coop_html_editor-1.3.1/coop_html_editor/static/aloha.0.23.26/plugins/common/image/vendor/ui/
-drwxr-xr-x   0 lucjean    (501) staff       (20)        0 2019-08-30 10:39:35.000000 coop_html_editor-1.3.1/coop_html_editor/static/aloha.0.23.26/plugins/common/image/vendor/ui/ui-lightness/
-drwxr-xr-x   0 lucjean    (501) staff       (20)        0 2019-08-30 10:39:40.000000 coop_html_editor-1.3.1/coop_html_editor/static/aloha.0.23.26/plugins/common/image/vendor/ui/ui-lightness/images/
--rw-r--r--   0 lucjean    (501) staff       (20)     3702 2019-08-29 13:07:39.000000 coop_html_editor-1.3.1/coop_html_editor/static/aloha.0.23.26/plugins/common/image/vendor/ui/ui-lightness/images/ui-icons_ef8c08_256x240.png
--rw-r--r--   0 lucjean    (501) staff       (20)      154 2019-08-29 13:07:39.000000 coop_html_editor-1.3.1/coop_html_editor/static/aloha.0.23.26/plugins/common/image/vendor/ui/ui-lightness/images/ui-bg_diagonals-thick_18_b81900_40x40.png
--rw-r--r--   0 lucjean    (501) staff       (20)      103 2019-08-29 13:07:39.000000 coop_html_editor-1.3.1/coop_html_editor/static/aloha.0.23.26/plugins/common/image/vendor/ui/ui-lightness/images/ui-bg_glass_100_f6f6f6_1x400.png
--rw-r--r--   0 lucjean    (501) staff       (20)     1986 2019-08-29 13:07:39.000000 coop_html_editor-1.3.1/coop_html_editor/static/aloha.0.23.26/plugins/common/image/vendor/ui/ui-lightness/images/ui-bg_gloss-wave_35_f6a828_500x100.png
--rw-r--r--   0 lucjean    (501) staff       (20)       88 2019-08-29 13:07:39.000000 coop_html_editor-1.3.1/coop_html_editor/static/aloha.0.23.26/plugins/common/image/vendor/ui/ui-lightness/images/ui-bg_highlight-soft_100_eeeeee_1x100.png
--rw-r--r--   0 lucjean    (501) staff       (20)      126 2019-08-29 13:07:39.000000 coop_html_editor-1.3.1/coop_html_editor/static/aloha.0.23.26/plugins/common/image/vendor/ui/ui-lightness/images/ui-bg_highlight-soft_75_ffe45c_1x100.png
--rw-r--r--   0 lucjean    (501) staff       (20)       95 2019-08-29 13:07:39.000000 coop_html_editor-1.3.1/coop_html_editor/static/aloha.0.23.26/plugins/common/image/vendor/ui/ui-lightness/images/ui-bg_glass_65_ffffff_1x400.png
--rw-r--r--   0 lucjean    (501) staff       (20)     3702 2019-08-29 13:07:39.000000 coop_html_editor-1.3.1/coop_html_editor/static/aloha.0.23.26/plugins/common/image/vendor/ui/ui-lightness/images/ui-icons_228ef1_256x240.png
--rw-r--r--   0 lucjean    (501) staff       (20)      154 2019-08-29 13:07:39.000000 coop_html_editor-1.3.1/coop_html_editor/static/aloha.0.23.26/plugins/common/image/vendor/ui/ui-lightness/images/ui-bg_diagonals-thick_20_666666_40x40.png
--rw-r--r--   0 lucjean    (501) staff       (20)      115 2019-08-29 13:07:39.000000 coop_html_editor-1.3.1/coop_html_editor/static/aloha.0.23.26/plugins/common/image/vendor/ui/ui-lightness/images/ui-bg_glass_100_fdf5ce_1x400.png
--rw-r--r--   0 lucjean    (501) staff       (20)     3702 2019-08-29 13:07:39.000000 coop_html_editor-1.3.1/coop_html_editor/static/aloha.0.23.26/plugins/common/image/vendor/ui/ui-lightness/images/ui-icons_ffffff_256x240.png
--rw-r--r--   0 lucjean    (501) staff       (20)     3702 2019-08-29 13:07:39.000000 coop_html_editor-1.3.1/coop_html_editor/static/aloha.0.23.26/plugins/common/image/vendor/ui/ui-lightness/images/ui-icons_222222_256x240.png
--rw-r--r--   0 lucjean    (501) staff       (20)     3702 2019-08-29 13:07:39.000000 coop_html_editor-1.3.1/coop_html_editor/static/aloha.0.23.26/plugins/common/image/vendor/ui/ui-lightness/images/ui-icons_ffd27a_256x240.png
--rw-r--r--   0 lucjean    (501) staff       (20)       87 2019-08-29 13:07:39.000000 coop_html_editor-1.3.1/coop_html_editor/static/aloha.0.23.26/plugins/common/image/vendor/ui/ui-lightness/images/ui-bg_flat_10_000000_40x100.png
-drwxr-xr-x   0 lucjean    (501) staff       (20)        0 2019-08-30 10:39:40.000000 coop_html_editor-1.3.1/coop_html_editor/static/aloha.0.23.26/plugins/common/image/vendor/jcrop/
--rw-r--r--   0 lucjean    (501) staff       (20)      323 2019-08-29 13:07:39.000000 coop_html_editor-1.3.1/coop_html_editor/static/aloha.0.23.26/plugins/common/image/vendor/jcrop/jcrop.gif
--rw-r--r--   0 lucjean    (501) staff       (20)     1006 2019-08-29 13:07:39.000000 coop_html_editor-1.3.1/coop_html_editor/static/aloha.0.23.26/plugins/common/image/vendor/jcrop/jquery.jcrop.css
-drwxr-xr-x   0 lucjean    (501) staff       (20)        0 2019-08-30 10:39:39.000000 coop_html_editor-1.3.1/coop_html_editor/static/aloha.0.23.26/plugins/common/align/
--rw-r--r--   0 lucjean    (501) staff       (20)     7652 2019-08-29 13:07:38.000000 coop_html_editor-1.3.1/coop_html_editor/static/aloha.0.23.26/plugins/common/align/LICENSE
-drwxr-xr-x   0 lucjean    (501) staff       (20)        0 2019-08-30 10:39:39.000000 coop_html_editor-1.3.1/coop_html_editor/static/aloha.0.23.26/plugins/common/align/css/
--rw-r--r--   0 lucjean    (501) staff       (20)      588 2019-08-29 13:07:38.000000 coop_html_editor-1.3.1/coop_html_editor/static/aloha.0.23.26/plugins/common/align/css/align.css
-drwxr-xr-x   0 lucjean    (501) staff       (20)        0 2019-08-30 10:39:35.000000 coop_html_editor-1.3.1/coop_html_editor/static/aloha.0.23.26/plugins/common/align/nls/
-drwxr-xr-x   0 lucjean    (501) staff       (20)        0 2019-08-30 10:39:39.000000 coop_html_editor-1.3.1/coop_html_editor/static/aloha.0.23.26/plugins/common/align/nls/zh-hans/
--rw-r--r--   0 lucjean    (501) staff       (20)      198 2019-08-29 13:07:38.000000 coop_html_editor-1.3.1/coop_html_editor/static/aloha.0.23.26/plugins/common/align/nls/zh-hans/i18n.js
-drwxr-xr-x   0 lucjean    (501) staff       (20)        0 2019-08-30 10:39:39.000000 coop_html_editor-1.3.1/coop_html_editor/static/aloha.0.23.26/plugins/common/align/nls/ca/
--rw-r--r--   0 lucjean    (501) staff       (20)      202 2019-08-29 13:07:38.000000 coop_html_editor-1.3.1/coop_html_editor/static/aloha.0.23.26/plugins/common/align/nls/ca/i18n.js
-drwxr-xr-x   0 lucjean    (501) staff       (20)        0 2019-08-30 10:39:39.000000 coop_html_editor-1.3.1/coop_html_editor/static/aloha.0.23.26/plugins/common/align/nls/ru/
--rw-r--r--   0 lucjean    (501) staff       (20)      246 2019-08-29 13:07:38.000000 coop_html_editor-1.3.1/coop_html_editor/static/aloha.0.23.26/plugins/common/align/nls/ru/i18n.js
-drwxr-xr-x   0 lucjean    (501) staff       (20)        0 2019-08-30 10:39:39.000000 coop_html_editor-1.3.1/coop_html_editor/static/aloha.0.23.26/plugins/common/align/nls/uk/
--rw-r--r--   0 lucjean    (501) staff       (20)      248 2019-08-29 13:07:38.000000 coop_html_editor-1.3.1/coop_html_editor/static/aloha.0.23.26/plugins/common/align/nls/uk/i18n.js
-drwxr-xr-x   0 lucjean    (501) staff       (20)        0 2019-08-30 10:39:39.000000 coop_html_editor-1.3.1/coop_html_editor/static/aloha.0.23.26/plugins/common/align/nls/mk/
--rw-r--r--   0 lucjean    (501) staff       (20)      259 2019-08-29 13:07:38.000000 coop_html_editor-1.3.1/coop_html_editor/static/aloha.0.23.26/plugins/common/align/nls/mk/i18n.js
-drwxr-xr-x   0 lucjean    (501) staff       (20)        0 2019-08-30 10:39:39.000000 coop_html_editor-1.3.1/coop_html_editor/static/aloha.0.23.26/plugins/common/align/nls/pt-br/
--rw-r--r--   0 lucjean    (501) staff       (20)      201 2019-08-29 13:07:38.000000 coop_html_editor-1.3.1/coop_html_editor/static/aloha.0.23.26/plugins/common/align/nls/pt-br/i18n.js
-drwxr-xr-x   0 lucjean    (501) staff       (20)        0 2019-08-30 10:39:39.000000 coop_html_editor-1.3.1/coop_html_editor/static/aloha.0.23.26/plugins/common/align/nls/de/
--rw-r--r--   0 lucjean    (501) staff       (20)      346 2019-08-29 13:07:38.000000 coop_html_editor-1.3.1/coop_html_editor/static/aloha.0.23.26/plugins/common/align/nls/de/i18n.js
--rw-r--r--   0 lucjean    (501) staff       (20)      267 2019-08-29 13:07:38.000000 coop_html_editor-1.3.1/coop_html_editor/static/aloha.0.23.26/plugins/common/align/README
-drwxr-xr-x   0 lucjean    (501) staff       (20)        0 2019-08-30 10:39:39.000000 coop_html_editor-1.3.1/coop_html_editor/static/aloha.0.23.26/plugins/common/align/img/
--rw-r--r--   0 lucjean    (501) staff       (20)      127 2019-08-29 13:07:38.000000 coop_html_editor-1.3.1/coop_html_editor/static/aloha.0.23.26/plugins/common/align/img/align.png
--rw-r--r--   0 lucjean    (501) staff       (20)       49 2019-08-29 13:07:38.000000 coop_html_editor-1.3.1/coop_html_editor/static/aloha.0.23.26/plugins/common/align/package.json
-drwxr-xr-x   0 lucjean    (501) staff       (20)        0 2019-08-30 10:39:35.000000 coop_html_editor-1.3.1/coop_html_editor/static/aloha.0.23.26/plugins/common/link/
-drwxr-xr-x   0 lucjean    (501) staff       (20)        0 2019-08-30 10:39:40.000000 coop_html_editor-1.3.1/coop_html_editor/static/aloha.0.23.26/plugins/common/link/css/
--rw-r--r--   0 lucjean    (501) staff       (20)      938 2019-08-29 13:07:39.000000 coop_html_editor-1.3.1/coop_html_editor/static/aloha.0.23.26/plugins/common/link/css/link.css
-drwxr-xr-x   0 lucjean    (501) staff       (20)        0 2019-08-30 10:39:35.000000 coop_html_editor-1.3.1/coop_html_editor/static/aloha.0.23.26/plugins/common/link/nls/
-drwxr-xr-x   0 lucjean    (501) staff       (20)        0 2019-08-30 10:39:41.000000 coop_html_editor-1.3.1/coop_html_editor/static/aloha.0.23.26/plugins/common/link/nls/zh-hans/
--rw-r--r--   0 lucjean    (501) staff       (20)      447 2019-08-29 13:07:39.000000 coop_html_editor-1.3.1/coop_html_editor/static/aloha.0.23.26/plugins/common/link/nls/zh-hans/i18n.js
-drwxr-xr-x   0 lucjean    (501) staff       (20)        0 2019-08-30 10:39:41.000000 coop_html_editor-1.3.1/coop_html_editor/static/aloha.0.23.26/plugins/common/link/nls/ca/
--rw-r--r--   0 lucjean    (501) staff       (20)      458 2019-08-29 13:07:39.000000 coop_html_editor-1.3.1/coop_html_editor/static/aloha.0.23.26/plugins/common/link/nls/ca/i18n.js
-drwxr-xr-x   0 lucjean    (501) staff       (20)        0 2019-08-30 10:39:41.000000 coop_html_editor-1.3.1/coop_html_editor/static/aloha.0.23.26/plugins/common/link/nls/ru/
--rw-r--r--   0 lucjean    (501) staff       (20)      590 2019-08-29 13:07:39.000000 coop_html_editor-1.3.1/coop_html_editor/static/aloha.0.23.26/plugins/common/link/nls/ru/i18n.js
-drwxr-xr-x   0 lucjean    (501) staff       (20)        0 2019-08-30 10:39:41.000000 coop_html_editor-1.3.1/coop_html_editor/static/aloha.0.23.26/plugins/common/link/nls/uk/
--rw-r--r--   0 lucjean    (501) staff       (20)      616 2019-08-29 13:07:39.000000 coop_html_editor-1.3.1/coop_html_editor/static/aloha.0.23.26/plugins/common/link/nls/uk/i18n.js
-drwxr-xr-x   0 lucjean    (501) staff       (20)        0 2019-08-30 10:39:41.000000 coop_html_editor-1.3.1/coop_html_editor/static/aloha.0.23.26/plugins/common/link/nls/mk/
--rw-r--r--   0 lucjean    (501) staff       (20)      510 2019-08-29 13:07:39.000000 coop_html_editor-1.3.1/coop_html_editor/static/aloha.0.23.26/plugins/common/link/nls/mk/i18n.js
-drwxr-xr-x   0 lucjean    (501) staff       (20)        0 2019-08-30 10:39:41.000000 coop_html_editor-1.3.1/coop_html_editor/static/aloha.0.23.26/plugins/common/link/nls/pt-br/
--rw-r--r--   0 lucjean    (501) staff       (20)      430 2019-08-29 13:07:39.000000 coop_html_editor-1.3.1/coop_html_editor/static/aloha.0.23.26/plugins/common/link/nls/pt-br/i18n.js
-drwxr-xr-x   0 lucjean    (501) staff       (20)        0 2019-08-30 10:39:41.000000 coop_html_editor-1.3.1/coop_html_editor/static/aloha.0.23.26/plugins/common/link/nls/de/
--rw-r--r--   0 lucjean    (501) staff       (20)      471 2019-08-29 13:07:39.000000 coop_html_editor-1.3.1/coop_html_editor/static/aloha.0.23.26/plugins/common/link/nls/de/i18n.js
-drwxr-xr-x   0 lucjean    (501) staff       (20)        0 2019-08-30 10:39:41.000000 coop_html_editor-1.3.1/coop_html_editor/static/aloha.0.23.26/plugins/common/link/extra/
--rw-r--r--   0 lucjean    (501) staff       (20)     7425 2019-08-29 13:07:39.000000 coop_html_editor-1.3.1/coop_html_editor/static/aloha.0.23.26/plugins/common/link/extra/slowlinklist.js
--rw-r--r--   0 lucjean    (501) staff       (20)     7303 2019-08-29 13:07:39.000000 coop_html_editor-1.3.1/coop_html_editor/static/aloha.0.23.26/plugins/common/link/extra/delicious.js
--rw-r--r--   0 lucjean    (501) staff       (20)     7686 2019-08-29 13:07:39.000000 coop_html_editor-1.3.1/coop_html_editor/static/aloha.0.23.26/plugins/common/link/extra/linklist.js
-drwxr-xr-x   0 lucjean    (501) staff       (20)        0 2019-08-30 10:39:41.000000 coop_html_editor-1.3.1/coop_html_editor/static/aloha.0.23.26/plugins/common/table/
-drwxr-xr-x   0 lucjean    (501) staff       (20)        0 2019-08-30 10:39:41.000000 coop_html_editor-1.3.1/coop_html_editor/static/aloha.0.23.26/plugins/common/table/css/
--rw-r--r--   0 lucjean    (501) staff       (20)     3082 2019-08-29 13:07:39.000000 coop_html_editor-1.3.1/coop_html_editor/static/aloha.0.23.26/plugins/common/table/css/table.css
-drwxr-xr-x   0 lucjean    (501) staff       (20)        0 2019-08-30 10:39:35.000000 coop_html_editor-1.3.1/coop_html_editor/static/aloha.0.23.26/plugins/common/table/nls/
-drwxr-xr-x   0 lucjean    (501) staff       (20)        0 2019-08-30 10:39:41.000000 coop_html_editor-1.3.1/coop_html_editor/static/aloha.0.23.26/plugins/common/table/nls/zh-hans/
--rw-r--r--   0 lucjean    (501) staff       (20)     1319 2019-08-29 13:07:39.000000 coop_html_editor-1.3.1/coop_html_editor/static/aloha.0.23.26/plugins/common/table/nls/zh-hans/i18n.js
-drwxr-xr-x   0 lucjean    (501) staff       (20)        0 2019-08-30 10:39:41.000000 coop_html_editor-1.3.1/coop_html_editor/static/aloha.0.23.26/plugins/common/table/nls/ca/
--rw-r--r--   0 lucjean    (501) staff       (20)     1572 2019-08-29 13:07:39.000000 coop_html_editor-1.3.1/coop_html_editor/static/aloha.0.23.26/plugins/common/table/nls/ca/i18n.js
-drwxr-xr-x   0 lucjean    (501) staff       (20)        0 2019-08-30 10:39:41.000000 coop_html_editor-1.3.1/coop_html_editor/static/aloha.0.23.26/plugins/common/table/nls/ru/
--rw-r--r--   0 lucjean    (501) staff       (20)     2143 2019-08-29 13:07:39.000000 coop_html_editor-1.3.1/coop_html_editor/static/aloha.0.23.26/plugins/common/table/nls/ru/i18n.js
-drwxr-xr-x   0 lucjean    (501) staff       (20)        0 2019-08-30 10:39:41.000000 coop_html_editor-1.3.1/coop_html_editor/static/aloha.0.23.26/plugins/common/table/nls/uk/
--rw-r--r--   0 lucjean    (501) staff       (20)     2065 2019-08-29 13:07:39.000000 coop_html_editor-1.3.1/coop_html_editor/static/aloha.0.23.26/plugins/common/table/nls/uk/i18n.js
-drwxr-xr-x   0 lucjean    (501) staff       (20)        0 2019-08-30 10:39:41.000000 coop_html_editor-1.3.1/coop_html_editor/static/aloha.0.23.26/plugins/common/table/nls/mk/
--rw-r--r--   0 lucjean    (501) staff       (20)     2044 2019-08-29 13:07:39.000000 coop_html_editor-1.3.1/coop_html_editor/static/aloha.0.23.26/plugins/common/table/nls/mk/i18n.js
-drwxr-xr-x   0 lucjean    (501) staff       (20)        0 2019-08-30 10:39:41.000000 coop_html_editor-1.3.1/coop_html_editor/static/aloha.0.23.26/plugins/common/table/nls/pt-br/
--rw-r--r--   0 lucjean    (501) staff       (20)     1540 2019-08-29 13:07:39.000000 coop_html_editor-1.3.1/coop_html_editor/static/aloha.0.23.26/plugins/common/table/nls/pt-br/i18n.js
-drwxr-xr-x   0 lucjean    (501) staff       (20)        0 2019-08-30 10:39:41.000000 coop_html_editor-1.3.1/coop_html_editor/static/aloha.0.23.26/plugins/common/table/nls/de/
--rw-r--r--   0 lucjean    (501) staff       (20)     1614 2019-08-29 13:07:39.000000 coop_html_editor-1.3.1/coop_html_editor/static/aloha.0.23.26/plugins/common/table/nls/de/i18n.js
-drwxr-xr-x   0 lucjean    (501) staff       (20)        0 2019-08-30 10:39:41.000000 coop_html_editor-1.3.1/coop_html_editor/static/aloha.0.23.26/plugins/common/table/img/
--rw-r--r--   0 lucjean    (501) staff       (20)      664 2019-08-29 13:07:39.000000 coop_html_editor-1.3.1/coop_html_editor/static/aloha.0.23.26/plugins/common/table/img/wai-red.png
--rw-r--r--   0 lucjean    (501) staff       (20)    11120 2019-08-29 13:07:39.000000 coop_html_editor-1.3.1/coop_html_editor/static/aloha.0.23.26/plugins/common/table/img/table_layout.png
--rw-r--r--   0 lucjean    (501) staff       (20)       55 2019-08-29 13:07:39.000000 coop_html_editor-1.3.1/coop_html_editor/static/aloha.0.23.26/plugins/common/table/img/left.cur
--rw-r--r--   0 lucjean    (501) staff       (20)      501 2019-08-29 13:07:39.000000 coop_html_editor-1.3.1/coop_html_editor/static/aloha.0.23.26/plugins/common/table/img/wai-green.png
--rw-r--r--   0 lucjean    (501) staff       (20)      183 2019-08-29 13:07:39.000000 coop_html_editor-1.3.1/coop_html_editor/static/aloha.0.23.26/plugins/common/table/img/down.cur
--rw-r--r--   0 lucjean    (501) staff       (20)        3 2019-08-29 13:07:39.000000 coop_html_editor-1.3.1/coop_html_editor/static/aloha.0.23.26/plugins/common/table/package.json
-drwxr-xr-x   0 lucjean    (501) staff       (20)        0 2019-08-30 10:39:41.000000 coop_html_editor-1.3.1/coop_html_editor/static/aloha.0.23.26/plugins/common/list/
-drwxr-xr-x   0 lucjean    (501) staff       (20)        0 2019-08-30 10:39:35.000000 coop_html_editor-1.3.1/coop_html_editor/static/aloha.0.23.26/plugins/common/list/nls/
-drwxr-xr-x   0 lucjean    (501) staff       (20)        0 2019-08-30 10:39:41.000000 coop_html_editor-1.3.1/coop_html_editor/static/aloha.0.23.26/plugins/common/list/nls/zh-hans/
--rw-r--r--   0 lucjean    (501) staff       (20)      247 2019-08-29 13:07:39.000000 coop_html_editor-1.3.1/coop_html_editor/static/aloha.0.23.26/plugins/common/list/nls/zh-hans/i18n.js
-drwxr-xr-x   0 lucjean    (501) staff       (20)        0 2019-08-30 10:39:41.000000 coop_html_editor-1.3.1/coop_html_editor/static/aloha.0.23.26/plugins/common/list/nls/ca/
--rw-r--r--   0 lucjean    (501) staff       (20)      293 2019-08-29 13:07:39.000000 coop_html_editor-1.3.1/coop_html_editor/static/aloha.0.23.26/plugins/common/list/nls/ca/i18n.js
-drwxr-xr-x   0 lucjean    (501) staff       (20)        0 2019-08-30 10:39:41.000000 coop_html_editor-1.3.1/coop_html_editor/static/aloha.0.23.26/plugins/common/list/nls/ru/
--rw-r--r--   0 lucjean    (501) staff       (20)      342 2019-08-29 13:07:39.000000 coop_html_editor-1.3.1/coop_html_editor/static/aloha.0.23.26/plugins/common/list/nls/ru/i18n.js
-drwxr-xr-x   0 lucjean    (501) staff       (20)        0 2019-08-30 10:39:41.000000 coop_html_editor-1.3.1/coop_html_editor/static/aloha.0.23.26/plugins/common/list/nls/uk/
--rw-r--r--   0 lucjean    (501) staff       (20)      375 2019-08-29 13:07:39.000000 coop_html_editor-1.3.1/coop_html_editor/static/aloha.0.23.26/plugins/common/list/nls/uk/i18n.js
-drwxr-xr-x   0 lucjean    (501) staff       (20)        0 2019-08-30 10:39:41.000000 coop_html_editor-1.3.1/coop_html_editor/static/aloha.0.23.26/plugins/common/list/nls/mk/
--rw-r--r--   0 lucjean    (501) staff       (20)      413 2019-08-29 13:07:39.000000 coop_html_editor-1.3.1/coop_html_editor/static/aloha.0.23.26/plugins/common/list/nls/mk/i18n.js
-drwxr-xr-x   0 lucjean    (501) staff       (20)        0 2019-08-30 10:39:41.000000 coop_html_editor-1.3.1/coop_html_editor/static/aloha.0.23.26/plugins/common/list/nls/pt-br/
--rw-r--r--   0 lucjean    (501) staff       (20)      262 2019-08-29 13:07:39.000000 coop_html_editor-1.3.1/coop_html_editor/static/aloha.0.23.26/plugins/common/list/nls/pt-br/i18n.js
-drwxr-xr-x   0 lucjean    (501) staff       (20)        0 2019-08-30 10:39:41.000000 coop_html_editor-1.3.1/coop_html_editor/static/aloha.0.23.26/plugins/common/list/nls/de/
--rw-r--r--   0 lucjean    (501) staff       (20)      271 2019-08-29 13:07:39.000000 coop_html_editor-1.3.1/coop_html_editor/static/aloha.0.23.26/plugins/common/list/nls/de/i18n.js
--rw-r--r--   0 lucjean    (501) staff       (20)        3 2019-08-29 13:07:39.000000 coop_html_editor-1.3.1/coop_html_editor/static/aloha.0.23.26/plugins/common/list/package.json
-drwxr-xr-x   0 lucjean    (501) staff       (20)        0 2019-08-30 10:39:35.000000 coop_html_editor-1.3.1/coop_html_editor/static/aloha.0.23.26/plugins/common/format/
-drwxr-xr-x   0 lucjean    (501) staff       (20)        0 2019-08-30 10:39:35.000000 coop_html_editor-1.3.1/coop_html_editor/static/aloha.0.23.26/plugins/common/format/nls/
-drwxr-xr-x   0 lucjean    (501) staff       (20)        0 2019-08-30 10:39:40.000000 coop_html_editor-1.3.1/coop_html_editor/static/aloha.0.23.26/plugins/common/format/nls/zh-hans/
--rw-r--r--   0 lucjean    (501) staff       (20)     1727 2019-08-29 13:07:38.000000 coop_html_editor-1.3.1/coop_html_editor/static/aloha.0.23.26/plugins/common/format/nls/zh-hans/i18n.js
-drwxr-xr-x   0 lucjean    (501) staff       (20)        0 2019-08-30 10:39:40.000000 coop_html_editor-1.3.1/coop_html_editor/static/aloha.0.23.26/plugins/common/format/nls/ca/
--rw-r--r--   0 lucjean    (501) staff       (20)     1823 2019-08-29 13:07:38.000000 coop_html_editor-1.3.1/coop_html_editor/static/aloha.0.23.26/plugins/common/format/nls/ca/i18n.js
-drwxr-xr-x   0 lucjean    (501) staff       (20)        0 2019-08-30 10:39:40.000000 coop_html_editor-1.3.1/coop_html_editor/static/aloha.0.23.26/plugins/common/format/nls/ru/
--rw-r--r--   0 lucjean    (501) staff       (20)     2109 2019-08-29 13:07:38.000000 coop_html_editor-1.3.1/coop_html_editor/static/aloha.0.23.26/plugins/common/format/nls/ru/i18n.js
-drwxr-xr-x   0 lucjean    (501) staff       (20)        0 2019-08-30 10:39:40.000000 coop_html_editor-1.3.1/coop_html_editor/static/aloha.0.23.26/plugins/common/format/nls/uk/
--rw-r--r--   0 lucjean    (501) staff       (20)     2075 2019-08-29 13:07:38.000000 coop_html_editor-1.3.1/coop_html_editor/static/aloha.0.23.26/plugins/common/format/nls/uk/i18n.js
-drwxr-xr-x   0 lucjean    (501) staff       (20)        0 2019-08-30 10:39:40.000000 coop_html_editor-1.3.1/coop_html_editor/static/aloha.0.23.26/plugins/common/format/nls/mk/
--rw-r--r--   0 lucjean    (501) staff       (20)     1977 2019-08-29 13:07:38.000000 coop_html_editor-1.3.1/coop_html_editor/static/aloha.0.23.26/plugins/common/format/nls/mk/i18n.js
-drwxr-xr-x   0 lucjean    (501) staff       (20)        0 2019-08-30 10:39:40.000000 coop_html_editor-1.3.1/coop_html_editor/static/aloha.0.23.26/plugins/common/format/nls/pt-br/
--rw-r--r--   0 lucjean    (501) staff       (20)     1797 2019-08-29 13:07:38.000000 coop_html_editor-1.3.1/coop_html_editor/static/aloha.0.23.26/plugins/common/format/nls/pt-br/i18n.js
-drwxr-xr-x   0 lucjean    (501) staff       (20)        0 2019-08-30 10:39:40.000000 coop_html_editor-1.3.1/coop_html_editor/static/aloha.0.23.26/plugins/common/format/nls/de/
--rw-r--r--   0 lucjean    (501) staff       (20)     1840 2019-08-29 13:07:38.000000 coop_html_editor-1.3.1/coop_html_editor/static/aloha.0.23.26/plugins/common/format/nls/de/i18n.js
-drwxr-xr-x   0 lucjean    (501) staff       (20)        0 2019-08-30 10:39:40.000000 coop_html_editor-1.3.1/coop_html_editor/static/aloha.0.23.26/plugins/common/format/img/
--rw-r--r--   0 lucjean    (501) staff       (20)      178 2019-08-29 13:07:38.000000 coop_html_editor-1.3.1/coop_html_editor/static/aloha.0.23.26/plugins/common/format/img/em.png
--rw-r--r--   0 lucjean    (501) staff       (20)      206 2019-08-29 13:07:38.000000 coop_html_editor-1.3.1/coop_html_editor/static/aloha.0.23.26/plugins/common/format/img/strong.png
-drwxr-xr-x   0 lucjean    (501) staff       (20)        0 2019-08-30 10:39:40.000000 coop_html_editor-1.3.1/coop_html_editor/static/aloha.0.23.26/plugins/common/commands/
-drwxr-xr-x   0 lucjean    (501) staff       (20)        0 2019-08-30 10:39:40.000000 coop_html_editor-1.3.1/coop_html_editor/static/aloha.0.23.26/plugins/common/commands/css/
--rw-r--r--   0 lucjean    (501) staff       (20)        0 2019-08-29 13:07:38.000000 coop_html_editor-1.3.1/coop_html_editor/static/aloha.0.23.26/plugins/common/commands/css/abbr.css
--rw-r--r--   0 lucjean    (501) staff       (20)        3 2019-08-29 13:07:38.000000 coop_html_editor-1.3.1/coop_html_editor/static/aloha.0.23.26/plugins/common/commands/package.json
-drwxr-xr-x   0 lucjean    (501) staff       (20)        0 2019-08-30 10:39:39.000000 coop_html_editor-1.3.1/coop_html_editor/static/aloha.0.23.26/plugins/common/abbr/
-drwxr-xr-x   0 lucjean    (501) staff       (20)        0 2019-08-30 10:39:39.000000 coop_html_editor-1.3.1/coop_html_editor/static/aloha.0.23.26/plugins/common/abbr/css/
--rw-r--r--   0 lucjean    (501) staff       (20)      115 2019-08-29 13:07:38.000000 coop_html_editor-1.3.1/coop_html_editor/static/aloha.0.23.26/plugins/common/abbr/css/abbr.css
-drwxr-xr-x   0 lucjean    (501) staff       (20)        0 2019-08-30 10:39:35.000000 coop_html_editor-1.3.1/coop_html_editor/static/aloha.0.23.26/plugins/common/abbr/nls/
-drwxr-xr-x   0 lucjean    (501) staff       (20)        0 2019-08-30 10:39:39.000000 coop_html_editor-1.3.1/coop_html_editor/static/aloha.0.23.26/plugins/common/abbr/nls/zh-hans/
--rw-r--r--   0 lucjean    (501) staff       (20)      177 2019-08-29 13:07:38.000000 coop_html_editor-1.3.1/coop_html_editor/static/aloha.0.23.26/plugins/common/abbr/nls/zh-hans/i18n.js
-drwxr-xr-x   0 lucjean    (501) staff       (20)        0 2019-08-30 10:39:39.000000 coop_html_editor-1.3.1/coop_html_editor/static/aloha.0.23.26/plugins/common/abbr/nls/ca/
--rw-r--r--   0 lucjean    (501) staff       (20)      198 2019-08-29 13:07:38.000000 coop_html_editor-1.3.1/coop_html_editor/static/aloha.0.23.26/plugins/common/abbr/nls/ca/i18n.js
-drwxr-xr-x   0 lucjean    (501) staff       (20)        0 2019-08-30 10:39:39.000000 coop_html_editor-1.3.1/coop_html_editor/static/aloha.0.23.26/plugins/common/abbr/nls/ru/
--rw-r--r--   0 lucjean    (501) staff       (20)      261 2019-08-29 13:07:38.000000 coop_html_editor-1.3.1/coop_html_editor/static/aloha.0.23.26/plugins/common/abbr/nls/ru/i18n.js
-drwxr-xr-x   0 lucjean    (501) staff       (20)        0 2019-08-30 10:39:39.000000 coop_html_editor-1.3.1/coop_html_editor/static/aloha.0.23.26/plugins/common/abbr/nls/uk/
--rw-r--r--   0 lucjean    (501) staff       (20)      247 2019-08-29 13:07:38.000000 coop_html_editor-1.3.1/coop_html_editor/static/aloha.0.23.26/plugins/common/abbr/nls/uk/i18n.js
-drwxr-xr-x   0 lucjean    (501) staff       (20)        0 2019-08-30 10:39:39.000000 coop_html_editor-1.3.1/coop_html_editor/static/aloha.0.23.26/plugins/common/abbr/nls/mk/
--rw-r--r--   0 lucjean    (501) staff       (20)      227 2019-08-29 13:07:38.000000 coop_html_editor-1.3.1/coop_html_editor/static/aloha.0.23.26/plugins/common/abbr/nls/mk/i18n.js
-drwxr-xr-x   0 lucjean    (501) staff       (20)        0 2019-08-30 10:39:39.000000 coop_html_editor-1.3.1/coop_html_editor/static/aloha.0.23.26/plugins/common/abbr/nls/pt-br/
--rw-r--r--   0 lucjean    (501) staff       (20)      199 2019-08-29 13:07:38.000000 coop_html_editor-1.3.1/coop_html_editor/static/aloha.0.23.26/plugins/common/abbr/nls/pt-br/i18n.js
-drwxr-xr-x   0 lucjean    (501) staff       (20)        0 2019-08-30 10:39:39.000000 coop_html_editor-1.3.1/coop_html_editor/static/aloha.0.23.26/plugins/common/abbr/nls/de/
--rw-r--r--   0 lucjean    (501) staff       (20)      188 2019-08-29 13:07:38.000000 coop_html_editor-1.3.1/coop_html_editor/static/aloha.0.23.26/plugins/common/abbr/nls/de/i18n.js
-drwxr-xr-x   0 lucjean    (501) staff       (20)        0 2019-08-30 10:39:39.000000 coop_html_editor-1.3.1/coop_html_editor/static/aloha.0.23.26/plugins/common/abbr/img/
--rw-r--r--   0 lucjean    (501) staff       (20)      262 2019-08-29 13:07:38.000000 coop_html_editor-1.3.1/coop_html_editor/static/aloha.0.23.26/plugins/common/abbr/img/remabbr.png
--rw-r--r--   0 lucjean    (501) staff       (20)        3 2019-08-29 13:07:38.000000 coop_html_editor-1.3.1/coop_html_editor/static/aloha.0.23.26/plugins/common/abbr/package.json
-drwxr-xr-x   0 lucjean    (501) staff       (20)        0 2019-08-30 10:39:35.000000 coop_html_editor-1.3.1/coop_html_editor/static/aloha.0.23.26/plugins/common/horizontalruler/
-drwxr-xr-x   0 lucjean    (501) staff       (20)        0 2019-08-30 10:39:40.000000 coop_html_editor-1.3.1/coop_html_editor/static/aloha.0.23.26/plugins/common/horizontalruler/css/
--rw-r--r--   0 lucjean    (501) staff       (20)       87 2019-08-29 13:07:38.000000 coop_html_editor-1.3.1/coop_html_editor/static/aloha.0.23.26/plugins/common/horizontalruler/css/horizontalruler.css
-drwxr-xr-x   0 lucjean    (501) staff       (20)        0 2019-08-30 10:39:35.000000 coop_html_editor-1.3.1/coop_html_editor/static/aloha.0.23.26/plugins/common/horizontalruler/nls/
-drwxr-xr-x   0 lucjean    (501) staff       (20)        0 2019-08-30 10:39:40.000000 coop_html_editor-1.3.1/coop_html_editor/static/aloha.0.23.26/plugins/common/horizontalruler/nls/zh-hans/
--rw-r--r--   0 lucjean    (501) staff       (20)       65 2019-08-29 13:07:39.000000 coop_html_editor-1.3.1/coop_html_editor/static/aloha.0.23.26/plugins/common/horizontalruler/nls/zh-hans/i18n.js
-drwxr-xr-x   0 lucjean    (501) staff       (20)        0 2019-08-30 10:39:40.000000 coop_html_editor-1.3.1/coop_html_editor/static/aloha.0.23.26/plugins/common/horizontalruler/nls/ca/
--rw-r--r--   0 lucjean    (501) staff       (20)       69 2019-08-29 13:07:38.000000 coop_html_editor-1.3.1/coop_html_editor/static/aloha.0.23.26/plugins/common/horizontalruler/nls/ca/i18n.js
-drwxr-xr-x   0 lucjean    (501) staff       (20)        0 2019-08-30 10:39:40.000000 coop_html_editor-1.3.1/coop_html_editor/static/aloha.0.23.26/plugins/common/horizontalruler/nls/ru/
--rw-r--r--   0 lucjean    (501) staff       (20)      101 2019-08-29 13:07:38.000000 coop_html_editor-1.3.1/coop_html_editor/static/aloha.0.23.26/plugins/common/horizontalruler/nls/ru/i18n.js
-drwxr-xr-x   0 lucjean    (501) staff       (20)        0 2019-08-30 10:39:40.000000 coop_html_editor-1.3.1/coop_html_editor/static/aloha.0.23.26/plugins/common/horizontalruler/nls/uk/
--rw-r--r--   0 lucjean    (501) staff       (20)       95 2019-08-29 13:07:38.000000 coop_html_editor-1.3.1/coop_html_editor/static/aloha.0.23.26/plugins/common/horizontalruler/nls/uk/i18n.js
-drwxr-xr-x   0 lucjean    (501) staff       (20)        0 2019-08-30 10:39:40.000000 coop_html_editor-1.3.1/coop_html_editor/static/aloha.0.23.26/plugins/common/horizontalruler/nls/mk/
--rw-r--r--   0 lucjean    (501) staff       (20)       93 2019-08-29 13:07:38.000000 coop_html_editor-1.3.1/coop_html_editor/static/aloha.0.23.26/plugins/common/horizontalruler/nls/mk/i18n.js
-drwxr-xr-x   0 lucjean    (501) staff       (20)        0 2019-08-30 10:39:40.000000 coop_html_editor-1.3.1/coop_html_editor/static/aloha.0.23.26/plugins/common/horizontalruler/nls/pt-br/
--rw-r--r--   0 lucjean    (501) staff       (20)       68 2019-08-29 13:07:38.000000 coop_html_editor-1.3.1/coop_html_editor/static/aloha.0.23.26/plugins/common/horizontalruler/nls/pt-br/i18n.js
-drwxr-xr-x   0 lucjean    (501) staff       (20)        0 2019-08-30 10:39:40.000000 coop_html_editor-1.3.1/coop_html_editor/static/aloha.0.23.26/plugins/common/horizontalruler/nls/de/
--rw-r--r--   0 lucjean    (501) staff       (20)       68 2019-08-29 13:07:38.000000 coop_html_editor-1.3.1/coop_html_editor/static/aloha.0.23.26/plugins/common/horizontalruler/nls/de/i18n.js
-drwxr-xr-x   0 lucjean    (501) staff       (20)        0 2019-08-30 10:39:40.000000 coop_html_editor-1.3.1/coop_html_editor/static/aloha.0.23.26/plugins/common/horizontalruler/img/
--rw-r--r--   0 lucjean    (501) staff       (20)      104 2019-08-29 13:07:38.000000 coop_html_editor-1.3.1/coop_html_editor/static/aloha.0.23.26/plugins/common/horizontalruler/img/icon.png
-drwxr-xr-x   0 lucjean    (501) staff       (20)        0 2019-08-30 10:39:41.000000 coop_html_editor-1.3.1/coop_html_editor/static/aloha.0.23.26/plugins/common/paste/
--rw-r--r--   0 lucjean    (501) staff       (20)      131 2019-08-29 13:07:39.000000 coop_html_editor-1.3.1/coop_html_editor/static/aloha.0.23.26/plugins/common/paste/package.json
-drwxr-xr-x   0 lucjean    (501) staff       (20)        0 2019-08-30 10:39:39.000000 coop_html_editor-1.3.1/coop_html_editor/static/aloha.0.23.26/plugins/common/block/
-drwxr-xr-x   0 lucjean    (501) staff       (20)        0 2019-08-30 10:39:39.000000 coop_html_editor-1.3.1/coop_html_editor/static/aloha.0.23.26/plugins/common/block/css/
--rw-r--r--   0 lucjean    (501) staff       (20)     2829 2019-08-29 13:07:38.000000 coop_html_editor-1.3.1/coop_html_editor/static/aloha.0.23.26/plugins/common/block/css/block.css
-drwxr-xr-x   0 lucjean    (501) staff       (20)        0 2019-08-30 10:39:35.000000 coop_html_editor-1.3.1/coop_html_editor/static/aloha.0.23.26/plugins/common/block/nls/
-drwxr-xr-x   0 lucjean    (501) staff       (20)        0 2019-08-30 10:39:39.000000 coop_html_editor-1.3.1/coop_html_editor/static/aloha.0.23.26/plugins/common/block/nls/zh-hans/
--rw-r--r--   0 lucjean    (501) staff       (20)       68 2019-08-29 13:07:38.000000 coop_html_editor-1.3.1/coop_html_editor/static/aloha.0.23.26/plugins/common/block/nls/zh-hans/i18n.js
-drwxr-xr-x   0 lucjean    (501) staff       (20)        0 2019-08-30 10:39:39.000000 coop_html_editor-1.3.1/coop_html_editor/static/aloha.0.23.26/plugins/common/block/nls/ca/
--rw-r--r--   0 lucjean    (501) staff       (20)      115 2019-08-29 13:07:38.000000 coop_html_editor-1.3.1/coop_html_editor/static/aloha.0.23.26/plugins/common/block/nls/ca/i18n.js
-drwxr-xr-x   0 lucjean    (501) staff       (20)        0 2019-08-30 10:39:39.000000 coop_html_editor-1.3.1/coop_html_editor/static/aloha.0.23.26/plugins/common/block/nls/ru/
--rw-r--r--   0 lucjean    (501) staff       (20)       88 2019-08-29 13:07:38.000000 coop_html_editor-1.3.1/coop_html_editor/static/aloha.0.23.26/plugins/common/block/nls/ru/i18n.js
-drwxr-xr-x   0 lucjean    (501) staff       (20)        0 2019-08-30 10:39:39.000000 coop_html_editor-1.3.1/coop_html_editor/static/aloha.0.23.26/plugins/common/block/nls/uk/
--rw-r--r--   0 lucjean    (501) staff       (20)       80 2019-08-29 13:07:38.000000 coop_html_editor-1.3.1/coop_html_editor/static/aloha.0.23.26/plugins/common/block/nls/uk/i18n.js
-drwxr-xr-x   0 lucjean    (501) staff       (20)        0 2019-08-30 10:39:39.000000 coop_html_editor-1.3.1/coop_html_editor/static/aloha.0.23.26/plugins/common/block/nls/mk/
--rw-r--r--   0 lucjean    (501) staff       (20)      102 2019-08-29 13:07:38.000000 coop_html_editor-1.3.1/coop_html_editor/static/aloha.0.23.26/plugins/common/block/nls/mk/i18n.js
-drwxr-xr-x   0 lucjean    (501) staff       (20)        0 2019-08-30 10:39:39.000000 coop_html_editor-1.3.1/coop_html_editor/static/aloha.0.23.26/plugins/common/block/nls/pt-br/
--rw-r--r--   0 lucjean    (501) staff       (20)       70 2019-08-29 13:07:38.000000 coop_html_editor-1.3.1/coop_html_editor/static/aloha.0.23.26/plugins/common/block/nls/pt-br/i18n.js
-drwxr-xr-x   0 lucjean    (501) staff       (20)        0 2019-08-30 10:39:39.000000 coop_html_editor-1.3.1/coop_html_editor/static/aloha.0.23.26/plugins/common/block/nls/de/
--rw-r--r--   0 lucjean    (501) staff       (20)       72 2019-08-29 13:07:38.000000 coop_html_editor-1.3.1/coop_html_editor/static/aloha.0.23.26/plugins/common/block/nls/de/i18n.js
--rw-r--r--   0 lucjean    (501) staff       (20)        0 2019-08-29 13:07:38.000000 coop_html_editor-1.3.1/coop_html_editor/static/aloha.0.23.26/plugins/common/block/README
-drwxr-xr-x   0 lucjean    (501) staff       (20)        0 2019-08-30 10:39:39.000000 coop_html_editor-1.3.1/coop_html_editor/static/aloha.0.23.26/plugins/common/block/img/
--rw-r--r--   0 lucjean    (501) staff       (20)      178 2019-08-29 13:07:38.000000 coop_html_editor-1.3.1/coop_html_editor/static/aloha.0.23.26/plugins/common/block/img/toolbar-draghandle.gif
--rw-r--r--   0 lucjean    (501) staff       (20)      273 2019-08-29 13:07:38.000000 coop_html_editor-1.3.1/coop_html_editor/static/aloha.0.23.26/plugins/common/block/package.json
-drwxr-xr-x   0 lucjean    (501) staff       (20)        0 2019-08-30 10:39:35.000000 coop_html_editor-1.3.1/coop_html_editor/static/aloha.0.23.26/plugins/extra/
-drwxr-xr-x   0 lucjean    (501) staff       (20)        0 2019-08-30 10:39:50.000000 coop_html_editor-1.3.1/coop_html_editor/static/aloha.0.23.26/plugins/extra/imagebrowser/
-drwxr-xr-x   0 lucjean    (501) staff       (20)        0 2019-08-30 10:39:35.000000 coop_html_editor-1.3.1/coop_html_editor/static/aloha.0.23.26/plugins/extra/imagebrowser/nls/
-drwxr-xr-x   0 lucjean    (501) staff       (20)        0 2019-08-30 10:39:50.000000 coop_html_editor-1.3.1/coop_html_editor/static/aloha.0.23.26/plugins/extra/imagebrowser/nls/zh-hans/
--rw-r--r--   0 lucjean    (501) staff       (20)      176 2019-08-29 13:07:40.000000 coop_html_editor-1.3.1/coop_html_editor/static/aloha.0.23.26/plugins/extra/imagebrowser/nls/zh-hans/i18n.js
-drwxr-xr-x   0 lucjean    (501) staff       (20)        0 2019-08-30 10:39:50.000000 coop_html_editor-1.3.1/coop_html_editor/static/aloha.0.23.26/plugins/extra/imagebrowser/nls/ca/
--rw-r--r--   0 lucjean    (501) staff       (20)      192 2019-08-29 13:07:40.000000 coop_html_editor-1.3.1/coop_html_editor/static/aloha.0.23.26/plugins/extra/imagebrowser/nls/ca/i18n.js
-drwxr-xr-x   0 lucjean    (501) staff       (20)        0 2019-08-30 10:39:50.000000 coop_html_editor-1.3.1/coop_html_editor/static/aloha.0.23.26/plugins/extra/imagebrowser/nls/ru/
--rw-r--r--   0 lucjean    (501) staff       (20)      268 2019-08-29 13:07:40.000000 coop_html_editor-1.3.1/coop_html_editor/static/aloha.0.23.26/plugins/extra/imagebrowser/nls/ru/i18n.js
-drwxr-xr-x   0 lucjean    (501) staff       (20)        0 2019-08-30 10:39:50.000000 coop_html_editor-1.3.1/coop_html_editor/static/aloha.0.23.26/plugins/extra/imagebrowser/nls/uk/
--rw-r--r--   0 lucjean    (501) staff       (20)      260 2019-08-29 13:07:40.000000 coop_html_editor-1.3.1/coop_html_editor/static/aloha.0.23.26/plugins/extra/imagebrowser/nls/uk/i18n.js
-drwxr-xr-x   0 lucjean    (501) staff       (20)        0 2019-08-30 10:39:50.000000 coop_html_editor-1.3.1/coop_html_editor/static/aloha.0.23.26/plugins/extra/imagebrowser/nls/mk/
--rw-r--r--   0 lucjean    (501) staff       (20)      214 2019-08-29 13:07:40.000000 coop_html_editor-1.3.1/coop_html_editor/static/aloha.0.23.26/plugins/extra/imagebrowser/nls/mk/i18n.js
-drwxr-xr-x   0 lucjean    (501) staff       (20)        0 2019-08-30 10:39:50.000000 coop_html_editor-1.3.1/coop_html_editor/static/aloha.0.23.26/plugins/extra/imagebrowser/nls/pt-br/
--rw-r--r--   0 lucjean    (501) staff       (20)      182 2019-08-29 13:07:40.000000 coop_html_editor-1.3.1/coop_html_editor/static/aloha.0.23.26/plugins/extra/imagebrowser/nls/pt-br/i18n.js
-drwxr-xr-x   0 lucjean    (501) staff       (20)        0 2019-08-30 10:39:50.000000 coop_html_editor-1.3.1/coop_html_editor/static/aloha.0.23.26/plugins/extra/imagebrowser/nls/de/
--rw-r--r--   0 lucjean    (501) staff       (20)      178 2019-08-29 13:07:40.000000 coop_html_editor-1.3.1/coop_html_editor/static/aloha.0.23.26/plugins/extra/imagebrowser/nls/de/i18n.js
--rw-r--r--   0 lucjean    (501) staff       (20)        0 2019-08-29 13:07:40.000000 coop_html_editor-1.3.1/coop_html_editor/static/aloha.0.23.26/plugins/extra/imagebrowser/README
-drwxr-xr-x   0 lucjean    (501) staff       (20)        0 2019-08-30 10:39:43.000000 coop_html_editor-1.3.1/coop_html_editor/static/aloha.0.23.26/plugins/extra/comments/
-drwxr-xr-x   0 lucjean    (501) staff       (20)        0 2019-08-30 10:39:43.000000 coop_html_editor-1.3.1/coop_html_editor/static/aloha.0.23.26/plugins/extra/comments/img/
--rw-r--r--   0 lucjean    (501) staff       (20)     2237 2019-08-29 13:07:39.000000 coop_html_editor-1.3.1/coop_html_editor/static/aloha.0.23.26/plugins/extra/comments/img/add.png
--rw-r--r--   0 lucjean    (501) staff       (20)     1387 2019-08-29 13:07:39.000000 coop_html_editor-1.3.1/coop_html_editor/static/aloha.0.23.26/plugins/extra/comments/img/textbox.png
--rw-r--r--   0 lucjean    (501) staff       (20)      954 2019-08-29 13:07:39.000000 coop_html_editor-1.3.1/coop_html_editor/static/aloha.0.23.26/plugins/extra/comments/img/comments.png
--rw-r--r--   0 lucjean    (501) staff       (20)       75 2019-08-29 13:07:39.000000 coop_html_editor-1.3.1/coop_html_editor/static/aloha.0.23.26/plugins/extra/comments/img/hr.png
--rw-r--r--   0 lucjean    (501) staff       (20)    10427 2019-08-29 13:07:39.000000 coop_html_editor-1.3.1/coop_html_editor/static/aloha.0.23.26/plugins/extra/comments/img/add-icon.png
--rw-r--r--   0 lucjean    (501) staff       (20)        2 2019-08-29 13:07:39.000000 coop_html_editor-1.3.1/coop_html_editor/static/aloha.0.23.26/plugins/extra/comments/package.json
-drwxr-xr-x   0 lucjean    (501) staff       (20)        0 2019-08-30 10:39:43.000000 coop_html_editor-1.3.1/coop_html_editor/static/aloha.0.23.26/plugins/extra/comments/lib/
--rw-r--r--   0 lucjean    (501) staff       (20)     9857 2019-08-29 13:07:39.000000 coop_html_editor-1.3.1/coop_html_editor/static/aloha.0.23.26/plugins/extra/comments/lib/comments.css
--rw-r--r--   0 lucjean    (501) staff       (20)    22158 2019-08-29 13:07:39.000000 coop_html_editor-1.3.1/coop_html_editor/static/aloha.0.23.26/plugins/extra/comments/lib/comments-plugin.js
-drwxr-xr-x   0 lucjean    (501) staff       (20)        0 2019-08-30 10:39:35.000000 coop_html_editor-1.3.1/coop_html_editor/static/aloha.0.23.26/plugins/extra/flag-icons/
-drwxr-xr-x   0 lucjean    (501) staff       (20)        0 2019-08-30 10:39:35.000000 coop_html_editor-1.3.1/coop_html_editor/static/aloha.0.23.26/plugins/extra/flag-icons/img/
-drwxr-xr-x   0 lucjean    (501) staff       (20)        0 2019-08-30 10:39:48.000000 coop_html_editor-1.3.1/coop_html_editor/static/aloha.0.23.26/plugins/extra/flag-icons/img/flags/
--rw-r--r--   0 lucjean    (501) staff       (20)      165 2019-08-29 13:07:40.000000 coop_html_editor-1.3.1/coop_html_editor/static/aloha.0.23.26/plugins/extra/flag-icons/img/flags/tg.png
--rw-r--r--   0 lucjean    (501) staff       (20)      437 2019-08-29 13:07:40.000000 coop_html_editor-1.3.1/coop_html_editor/static/aloha.0.23.26/plugins/extra/flag-icons/img/flags/vo.png
--rw-r--r--   0 lucjean    (501) staff       (20)      394 2019-08-29 13:07:39.000000 coop_html_editor-1.3.1/coop_html_editor/static/aloha.0.23.26/plugins/extra/flag-icons/img/flags/me.png
--rw-r--r--   0 lucjean    (501) staff       (20)      263 2019-08-29 13:07:39.000000 coop_html_editor-1.3.1/coop_html_editor/static/aloha.0.23.26/plugins/extra/flag-icons/img/flags/la.png
--rw-r--r--   0 lucjean    (501) staff       (20)      408 2019-08-29 13:07:40.000000 coop_html_editor-1.3.1/coop_html_editor/static/aloha.0.23.26/plugins/extra/flag-icons/img/flags/mr.png
--rw-r--r--   0 lucjean    (501) staff       (20)      372 2019-08-29 13:07:40.000000 coop_html_editor-1.3.1/coop_html_editor/static/aloha.0.23.26/plugins/extra/flag-icons/img/flags/ni.png
--rw-r--r--   0 lucjean    (501) staff       (20)      339 2019-08-29 13:07:39.000000 coop_html_editor-1.3.1/coop_html_editor/static/aloha.0.23.26/plugins/extra/flag-icons/img/flags/lv.png
--rw-r--r--   0 lucjean    (501) staff       (20)      339 2019-08-29 13:07:40.000000 coop_html_editor-1.3.1/coop_html_editor/static/aloha.0.23.26/plugins/extra/flag-icons/img/flags/om.png
--rw-r--r--   0 lucjean    (501) staff       (20)      420 2019-08-29 13:07:39.000000 coop_html_editor-1.3.1/coop_html_editor/static/aloha.0.23.26/plugins/extra/flag-icons/img/flags/af.png
--rw-r--r--   0 lucjean    (501) staff       (20)      337 2019-08-29 13:07:39.000000 coop_html_editor-1.3.1/coop_html_editor/static/aloha.0.23.26/plugins/extra/flag-icons/img/flags/cy.png
--rw-r--r--   0 lucjean    (501) staff       (20)      311 2019-08-29 13:07:39.000000 coop_html_editor-1.3.1/coop_html_editor/static/aloha.0.23.26/plugins/extra/flag-icons/img/flags/bj.png
--rw-r--r--   0 lucjean    (501) staff       (20)      349 2019-08-29 13:07:39.000000 coop_html_editor-1.3.1/coop_html_editor/static/aloha.0.23.26/plugins/extra/flag-icons/img/flags/cn.png
--rw-r--r--   0 lucjean    (501) staff       (20)      330 2019-08-29 13:07:39.000000 coop_html_editor-1.3.1/coop_html_editor/static/aloha.0.23.26/plugins/extra/flag-icons/img/flags/co.png
--rw-r--r--   0 lucjean    (501) staff       (20)      498 2019-08-29 13:07:39.000000 coop_html_editor-1.3.1/coop_html_editor/static/aloha.0.23.26/plugins/extra/flag-icons/img/flags/cx.png
--rw-r--r--   0 lucjean    (501) staff       (20)      456 2019-08-29 13:07:39.000000 coop_html_editor-1.3.1/coop_html_editor/static/aloha.0.23.26/plugins/extra/flag-icons/img/flags/ag.png
--rw-r--r--   0 lucjean    (501) staff       (20)      497 2019-08-29 13:07:40.000000 coop_html_editor-1.3.1/coop_html_editor/static/aloha.0.23.26/plugins/extra/flag-icons/img/flags/ms.png
--rw-r--r--   0 lucjean    (501) staff       (20)      404 2019-08-29 13:07:39.000000 coop_html_editor-1.3.1/coop_html_editor/static/aloha.0.23.26/plugins/extra/flag-icons/img/flags/md.png
--rw-r--r--   0 lucjean    (501) staff       (20)      359 2019-08-29 13:07:40.000000 coop_html_editor-1.3.1/coop_html_editor/static/aloha.0.23.26/plugins/extra/flag-icons/img/flags/zm.png
--rw-r--r--   0 lucjean    (501) staff       (20)      324 2019-08-29 13:07:40.000000 coop_html_editor-1.3.1/coop_html_editor/static/aloha.0.23.26/plugins/extra/flag-icons/img/flags/vn.png
--rw-r--r--   0 lucjean    (501) staff       (20)      399 2019-08-29 13:07:40.000000 coop_html_editor-1.3.1/coop_html_editor/static/aloha.0.23.26/plugins/extra/flag-icons/img/flags/tf.png
--rw-r--r--   0 lucjean    (501) staff       (20)      378 2019-08-29 13:07:40.000000 coop_html_editor-1.3.1/coop_html_editor/static/aloha.0.23.26/plugins/extra/flag-icons/img/flags/td.png
--rw-r--r--   0 lucjean    (501) staff       (20)      456 2019-08-29 13:07:40.000000 coop_html_editor-1.3.1/coop_html_editor/static/aloha.0.23.26/plugins/extra/flag-icons/img/flags/yt.png
--rw-r--r--   0 lucjean    (501) staff       (20)      393 2019-08-29 13:07:39.000000 coop_html_editor-1.3.1/coop_html_editor/static/aloha.0.23.26/plugins/extra/flag-icons/img/flags/lb.png
--rw-r--r--   0 lucjean    (501) staff       (20)      338 2019-08-29 13:07:39.000000 coop_html_editor-1.3.1/coop_html_editor/static/aloha.0.23.26/plugins/extra/flag-icons/img/flags/lu.png
--rw-r--r--   0 lucjean    (501) staff       (20)      541 2019-08-29 13:07:40.000000 coop_html_editor-1.3.1/coop_html_editor/static/aloha.0.23.26/plugins/extra/flag-icons/img/flags/mq.png
--rw-r--r--   0 lucjean    (501) staff       (20)      367 2019-08-29 13:07:39.000000 coop_html_editor-1.3.1/coop_html_editor/static/aloha.0.23.26/plugins/extra/flag-icons/img/flags/cz.png
--rw-r--r--   0 lucjean    (501) staff       (20)      277 2019-08-29 13:07:39.000000 coop_html_editor-1.3.1/coop_html_editor/static/aloha.0.23.26/plugins/extra/flag-icons/img/flags/ae.png
--rw-r--r--   0 lucjean    (501) staff       (20)      347 2019-08-29 13:07:39.000000 coop_html_editor-1.3.1/coop_html_editor/static/aloha.0.23.26/plugins/extra/flag-icons/img/flags/cm.png
--rw-r--r--   0 lucjean    (501) staff       (20)      350 2019-08-29 13:07:39.000000 coop_html_editor-1.3.1/coop_html_editor/static/aloha.0.23.26/plugins/extra/flag-icons/img/flags/fam.png
--rw-r--r--   0 lucjean    (501) staff       (20)      566 2019-08-29 13:07:39.000000 coop_html_editor-1.3.1/coop_html_editor/static/aloha.0.23.26/plugins/extra/flag-icons/img/flags/bi.png
--rw-r--r--   0 lucjean    (501) staff       (20)      367 2019-08-29 13:07:39.000000 coop_html_editor-1.3.1/coop_html_editor/static/aloha.0.23.26/plugins/extra/flag-icons/img/flags/ar.png
--rw-r--r--   0 lucjean    (501) staff       (20)      540 2019-08-29 13:07:39.000000 coop_html_editor-1.3.1/coop_html_editor/static/aloha.0.23.26/plugins/extra/flag-icons/img/flags/as.png
--rw-r--r--   0 lucjean    (501) staff       (20)      345 2019-08-29 13:07:39.000000 coop_html_editor-1.3.1/coop_html_editor/static/aloha.0.23.26/plugins/extra/flag-icons/img/flags/bh.png
--rw-r--r--   0 lucjean    (501) staff       (20)      324 2019-08-29 13:07:39.000000 coop_html_editor-1.3.1/coop_html_editor/static/aloha.0.23.26/plugins/extra/flag-icons/img/flags/cl.png
--rw-r--r--   0 lucjean    (501) staff       (20)      454 2019-08-29 13:07:39.000000 coop_html_editor-1.3.1/coop_html_editor/static/aloha.0.23.26/plugins/extra/flag-icons/img/flags/ad.png
--rw-r--r--   0 lucjean    (501) staff       (20)      481 2019-08-29 13:07:40.000000 coop_html_editor-1.3.1/coop_html_editor/static/aloha.0.23.26/plugins/extra/flag-icons/img/flags/mp.png
--rw-r--r--   0 lucjean    (501) staff       (20)      345 2019-08-29 13:07:39.000000 coop_html_editor-1.3.1/coop_html_editor/static/aloha.0.23.26/plugins/extra/flag-icons/img/flags/lt.png
--rw-r--r--   0 lucjean    (501) staff       (20)      313 2019-08-29 13:07:39.000000 coop_html_editor-1.3.1/coop_html_editor/static/aloha.0.23.26/plugins/extra/flag-icons/img/flags/mg.png
--rw-r--r--   0 lucjean    (501) staff       (20)      462 2019-08-29 13:07:39.000000 coop_html_editor-1.3.1/coop_html_editor/static/aloha.0.23.26/plugins/extra/flag-icons/img/flags/lc.png
--rw-r--r--   0 lucjean    (501) staff       (20)      366 2019-08-29 13:07:40.000000 coop_html_editor-1.3.1/coop_html_editor/static/aloha.0.23.26/plugins/extra/flag-icons/img/flags/tr.png
--rw-r--r--   0 lucjean    (501) staff       (20)      304 2019-08-29 13:07:40.000000 coop_html_editor-1.3.1/coop_html_editor/static/aloha.0.23.26/plugins/extra/flag-icons/img/flags/ua.png
--rw-r--r--   0 lucjean    (501) staff       (20)      554 2019-08-29 13:07:40.000000 coop_html_editor-1.3.1/coop_html_editor/static/aloha.0.23.26/plugins/extra/flag-icons/img/flags/scotland.png
--rw-r--r--   0 lucjean    (501) staff       (20)      377 2019-08-29 13:07:40.000000 coop_html_editor-1.3.1/coop_html_editor/static/aloha.0.23.26/plugins/extra/flag-icons/img/flags/te.png
--rw-r--r--   0 lucjean    (501) staff       (20)      443 2019-08-29 13:07:40.000000 coop_html_editor-1.3.1/coop_html_editor/static/aloha.0.23.26/plugins/extra/flag-icons/img/flags/tv.png
--rw-r--r--   0 lucjean    (501) staff       (20)      198 2019-08-29 13:07:40.000000 coop_html_editor-1.3.1/coop_html_editor/static/aloha.0.23.26/plugins/extra/flag-icons/img/flags/ur.png
--rw-r--r--   0 lucjean    (501) staff       (20)      523 2019-08-29 13:07:40.000000 coop_html_editor-1.3.1/coop_html_editor/static/aloha.0.23.26/plugins/extra/flag-icons/img/flags/vi.png
--rw-r--r--   0 lucjean    (501) staff       (20)      292 2019-08-29 13:07:40.000000 coop_html_editor-1.3.1/coop_html_editor/static/aloha.0.23.26/plugins/extra/flag-icons/img/flags/ta.png
--rw-r--r--   0 lucjean    (501) staff       (20)      296 2019-08-29 13:07:40.000000 coop_html_editor-1.3.1/coop_html_editor/static/aloha.0.23.26/plugins/extra/flag-icons/img/flags/mt.png
--rw-r--r--   0 lucjean    (501) staff       (20)      397 2019-08-29 13:07:40.000000 coop_html_editor-1.3.1/coop_html_editor/static/aloha.0.23.26/plugins/extra/flag-icons/img/flags/no.png
--rw-r--r--   0 lucjean    (501) staff       (20)      173 2019-08-29 13:07:39.000000 coop_html_editor-1.3.1/coop_html_editor/static/aloha.0.23.26/plugins/extra/flag-icons/img/flags/lg.png
--rw-r--r--   0 lucjean    (501) staff       (20)      254 2019-08-29 13:07:39.000000 coop_html_editor-1.3.1/coop_html_editor/static/aloha.0.23.26/plugins/extra/flag-icons/img/flags/mc.png
--rw-r--r--   0 lucjean    (501) staff       (20)      239 2019-08-29 13:07:39.000000 coop_html_editor-1.3.1/coop_html_editor/static/aloha.0.23.26/plugins/extra/flag-icons/img/flags/ch.png
--rw-r--r--   0 lucjean    (501) staff       (20)      393 2019-08-29 13:07:39.000000 coop_html_editor-1.3.1/coop_html_editor/static/aloha.0.23.26/plugins/extra/flag-icons/img/flags/aw.png
--rw-r--r--   0 lucjean    (501) staff       (20)      476 2019-08-29 13:07:39.000000 coop_html_editor-1.3.1/coop_html_editor/static/aloha.0.23.26/plugins/extra/flag-icons/img/flags/bz.png
--rw-r--r--   0 lucjean    (501) staff       (20)      243 2019-08-29 13:07:39.000000 coop_html_editor-1.3.1/coop_html_editor/static/aloha.0.23.26/plugins/extra/flag-icons/img/flags/aa.png
--rw-r--r--   0 lucjean    (501) staff       (20)       98 2019-08-29 13:07:39.000000 coop_html_editor-1.3.1/coop_html_editor/static/aloha.0.23.26/plugins/extra/flag-icons/img/flags/av.png
--rw-r--r--   0 lucjean    (501) staff       (20)      499 2019-08-29 13:07:39.000000 coop_html_editor-1.3.1/coop_html_editor/static/aloha.0.23.26/plugins/extra/flag-icons/img/flags/bm.png
--rw-r--r--   0 lucjean    (501) staff       (20)      306 2019-08-29 13:07:39.000000 coop_html_editor-1.3.1/coop_html_editor/static/aloha.0.23.26/plugins/extra/flag-icons/img/flags/ci.png
--rw-r--r--   0 lucjean    (501) staff       (20)      227 2019-08-29 13:07:40.000000 coop_html_editor-1.3.1/coop_html_editor/static/aloha.0.23.26/plugins/extra/flag-icons/img/flags/ny.png
--rw-r--r--   0 lucjean    (501) staff       (20)      397 2019-08-29 13:07:40.000000 coop_html_editor-1.3.1/coop_html_editor/static/aloha.0.23.26/plugins/extra/flag-icons/img/flags/nn.png
--rw-r--r--   0 lucjean    (501) staff       (20)      360 2019-08-29 13:07:40.000000 coop_html_editor-1.3.1/coop_html_editor/static/aloha.0.23.26/plugins/extra/flag-icons/img/flags/mu.png
--rw-r--r--   0 lucjean    (501) staff       (20)      492 2019-08-29 13:07:40.000000 coop_html_editor-1.3.1/coop_html_editor/static/aloha.0.23.26/plugins/extra/flag-icons/img/flags/us.png
--rw-r--r--   0 lucjean    (501) staff       (20)      152 2019-08-29 13:07:39.000000 coop_html_editor-1.3.1/coop_html_editor/static/aloha.0.23.26/plugins/extra/flag-icons/img/flags/LICENSE
--rw-r--r--   0 lucjean    (501) staff       (20)      330 2019-08-29 13:07:40.000000 coop_html_editor-1.3.1/coop_html_editor/static/aloha.0.23.26/plugins/extra/flag-icons/img/flags/tw.png
--rw-r--r--   0 lucjean    (501) staff       (20)      302 2019-08-29 13:07:40.000000 coop_html_editor-1.3.1/coop_html_editor/static/aloha.0.23.26/plugins/extra/flag-icons/img/flags/ye.png
--rw-r--r--   0 lucjean    (501) staff       (20)      365 2019-08-29 13:07:40.000000 coop_html_editor-1.3.1/coop_html_editor/static/aloha.0.23.26/plugins/extra/flag-icons/img/flags/mw.png
--rw-r--r--   0 lucjean    (501) staff       (20)      310 2019-08-29 13:07:40.000000 coop_html_editor-1.3.1/coop_html_editor/static/aloha.0.23.26/plugins/extra/flag-icons/img/flags/nl.png
--rw-r--r--   0 lucjean    (501) staff       (20)      500 2019-08-29 13:07:39.000000 coop_html_editor-1.3.1/coop_html_editor/static/aloha.0.23.26/plugins/extra/flag-icons/img/flags/ls.png
--rw-r--r--   0 lucjean    (501) staff       (20)      341 2019-08-29 13:07:39.000000 coop_html_editor-1.3.1/coop_html_editor/static/aloha.0.23.26/plugins/extra/flag-icons/img/flags/bo.png
--rw-r--r--   0 lucjean    (501) staff       (20)      290 2019-08-29 13:07:39.000000 coop_html_editor-1.3.1/coop_html_editor/static/aloha.0.23.26/plugins/extra/flag-icons/img/flags/at.png
--rw-r--r--   0 lucjean    (501) staff       (20)      495 2019-08-29 13:07:39.000000 coop_html_editor-1.3.1/coop_html_editor/static/aloha.0.23.26/plugins/extra/flag-icons/img/flags/ck.png
--rw-r--r--   0 lucjean    (501) staff       (20)      382 2019-08-29 13:07:39.000000 coop_html_editor-1.3.1/coop_html_editor/static/aloha.0.23.26/plugins/extra/flag-icons/img/flags/by.png
--rw-r--r--   0 lucjean    (501) staff       (20)      306 2019-08-29 13:07:39.000000 coop_html_editor-1.3.1/coop_html_editor/static/aloha.0.23.26/plugins/extra/flag-icons/img/flags/ab.png
--rw-r--r--   0 lucjean    (501) staff       (20)      580 2019-08-29 13:07:39.000000 coop_html_editor-1.3.1/coop_html_editor/static/aloha.0.23.26/plugins/extra/flag-icons/img/flags/au.png
--rw-r--r--   0 lucjean    (501) staff       (20)      502 2019-08-29 13:07:39.000000 coop_html_editor-1.3.1/coop_html_editor/static/aloha.0.23.26/plugins/extra/flag-icons/img/flags/bn.png
--rw-r--r--   0 lucjean    (501) staff       (20)      293 2019-08-29 13:07:39.000000 coop_html_editor-1.3.1/coop_html_editor/static/aloha.0.23.26/plugins/extra/flag-icons/img/flags/ma.png
--rw-r--r--   0 lucjean    (501) staff       (20)      529 2019-08-29 13:07:40.000000 coop_html_editor-1.3.1/coop_html_editor/static/aloha.0.23.26/plugins/extra/flag-icons/img/flags/nz.png
--rw-r--r--   0 lucjean    (501) staff       (20)      365 2019-08-29 13:07:39.000000 coop_html_editor-1.3.1/coop_html_editor/static/aloha.0.23.26/plugins/extra/flag-icons/img/flags/lr.png
--rw-r--r--   0 lucjean    (501) staff       (20)      391 2019-08-29 13:07:40.000000 coop_html_editor-1.3.1/coop_html_editor/static/aloha.0.23.26/plugins/extra/flag-icons/img/flags/mv.png
--rw-r--r--   0 lucjean    (501) staff       (20)      349 2019-08-29 13:07:40.000000 coop_html_editor-1.3.1/coop_html_editor/static/aloha.0.23.26/plugins/extra/flag-icons/img/flags/zh.png
--rw-r--r--   0 lucjean    (501) staff       (20)      509 2019-08-29 13:07:40.000000 coop_html_editor-1.3.1/coop_html_editor/static/aloha.0.23.26/plugins/extra/flag-icons/img/flags/tc.png
--rw-r--r--   0 lucjean    (501) staff       (20)      388 2019-08-29 13:07:40.000000 coop_html_editor-1.3.1/coop_html_editor/static/aloha.0.23.26/plugins/extra/flag-icons/img/flags/ug.png
--rw-r--r--   0 lucjean    (501) staff       (20)      356 2019-08-29 13:07:40.000000 coop_html_editor-1.3.1/coop_html_editor/static/aloha.0.23.26/plugins/extra/flag-icons/img/flags/wo.png
--rw-r--r--   0 lucjean    (501) staff       (20)      486 2019-08-29 13:07:40.000000 coop_html_editor-1.3.1/coop_html_editor/static/aloha.0.23.26/plugins/extra/flag-icons/img/flags/tt.png
--rw-r--r--   0 lucjean    (501) staff       (20)      331 2019-08-29 13:07:40.000000 coop_html_editor-1.3.1/coop_html_editor/static/aloha.0.23.26/plugins/extra/flag-icons/img/flags/sw.png
--rw-r--r--   0 lucjean    (501) staff       (20)      243 2019-08-29 13:07:40.000000 coop_html_editor-1.3.1/coop_html_editor/static/aloha.0.23.26/plugins/extra/flag-icons/img/flags/pl.png
--rw-r--r--   0 lucjean    (501) staff       (20)      376 2019-08-29 13:07:40.000000 coop_html_editor-1.3.1/coop_html_editor/static/aloha.0.23.26/plugins/extra/flag-icons/img/flags/rs.png
--rw-r--r--   0 lucjean    (501) staff       (20)      377 2019-08-29 13:07:39.000000 coop_html_editor-1.3.1/coop_html_editor/static/aloha.0.23.26/plugins/extra/flag-icons/img/flags/in.png
--rw-r--r--   0 lucjean    (501) staff       (20)      493 2019-08-29 13:07:39.000000 coop_html_editor-1.3.1/coop_html_editor/static/aloha.0.23.26/plugins/extra/flag-icons/img/flags/ge.png
--rw-r--r--   0 lucjean    (501) staff       (20)      157 2019-08-29 13:07:39.000000 coop_html_editor-1.3.1/coop_html_editor/static/aloha.0.23.26/plugins/extra/flag-icons/img/flags/fa.png
--rw-r--r--   0 lucjean    (501) staff       (20)      391 2019-08-29 13:07:39.000000 coop_html_editor-1.3.1/coop_html_editor/static/aloha.0.23.26/plugins/extra/flag-icons/img/flags/gr.png
--rw-r--r--   0 lucjean    (501) staff       (20)      391 2019-08-29 13:07:39.000000 coop_html_editor-1.3.1/coop_html_editor/static/aloha.0.23.26/plugins/extra/flag-icons/img/flags/el.png
--rw-r--r--   0 lucjean    (501) staff       (20)      522 2019-08-29 13:07:39.000000 coop_html_editor-1.3.1/coop_html_editor/static/aloha.0.23.26/plugins/extra/flag-icons/img/flags/gs.png
--rw-r--r--   0 lucjean    (501) staff       (20)      461 2019-08-29 13:07:39.000000 coop_html_editor-1.3.1/coop_html_editor/static/aloha.0.23.26/plugins/extra/flag-icons/img/flags/gd.png
--rw-r--r--   0 lucjean    (501) staff       (20)      575 2019-08-29 13:07:39.000000 coop_html_editor-1.3.1/coop_html_editor/static/aloha.0.23.26/plugins/extra/flag-icons/img/flags/io.png
--rw-r--r--   0 lucjean    (501) staff       (20)      393 2019-08-29 13:07:39.000000 coop_html_editor-1.3.1/coop_html_editor/static/aloha.0.23.26/plugins/extra/flag-icons/img/flags/hk.png
--rw-r--r--   0 lucjean    (501) staff       (20)      424 2019-08-29 13:07:39.000000 coop_html_editor-1.3.1/coop_html_editor/static/aloha.0.23.26/plugins/extra/flag-icons/img/flags/kp.png
--rw-r--r--   0 lucjean    (501) staff       (20)      354 2019-08-29 13:07:39.000000 coop_html_editor-1.3.1/coop_html_editor/static/aloha.0.23.26/plugins/extra/flag-icons/img/flags/kg.png
--rw-r--r--   0 lucjean    (501) staff       (20)      572 2019-08-29 13:07:40.000000 coop_html_editor-1.3.1/coop_html_editor/static/aloha.0.23.26/plugins/extra/flag-icons/img/flags/pm.png
--rw-r--r--   0 lucjean    (501) staff       (20)      373 2019-08-29 13:07:40.000000 coop_html_editor-1.3.1/coop_html_editor/static/aloha.0.23.26/plugins/extra/flag-icons/img/flags/sv.png
--rw-r--r--   0 lucjean    (501) staff       (20)      369 2019-08-29 13:07:40.000000 coop_html_editor-1.3.1/coop_html_editor/static/aloha.0.23.26/plugins/extra/flag-icons/img/flags/re.png
--rw-r--r--   0 lucjean    (501) staff       (20)      428 2019-08-29 13:07:40.000000 coop_html_editor-1.3.1/coop_html_editor/static/aloha.0.23.26/plugins/extra/flag-icons/img/flags/sa.png
--rw-r--r--   0 lucjean    (501) staff       (20)      481 2019-08-29 13:07:40.000000 coop_html_editor-1.3.1/coop_html_editor/static/aloha.0.23.26/plugins/extra/flag-icons/img/flags/sc.png
--rw-r--r--   0 lucjean    (501) staff       (20)      429 2019-08-29 13:07:40.000000 coop_html_editor-1.3.1/coop_html_editor/static/aloha.0.23.26/plugins/extra/flag-icons/img/flags/st.png
--rw-r--r--   0 lucjean    (501) staff       (20)      307 2019-08-29 13:07:39.000000 coop_html_editor-1.3.1/coop_html_editor/static/aloha.0.23.26/plugins/extra/flag-icons/img/flags/ja.png
--rw-r--r--   0 lucjean    (501) staff       (20)      435 2019-08-29 13:07:39.000000 coop_html_editor-1.3.1/coop_html_editor/static/aloha.0.23.26/plugins/extra/flag-icons/img/flags/ke.png
--rw-r--r--   0 lucjean    (501) staff       (20)      177 2019-08-29 13:07:39.000000 coop_html_editor-1.3.1/coop_html_editor/static/aloha.0.23.26/plugins/extra/flag-icons/img/flags/jv.png
--rw-r--r--   0 lucjean    (501) staff       (20)      507 2019-08-29 13:07:39.000000 coop_html_editor-1.3.1/coop_html_editor/static/aloha.0.23.26/plugins/extra/flag-icons/img/flags/kr.png
--rw-r--r--   0 lucjean    (501) staff       (20)      377 2019-08-29 13:07:39.000000 coop_html_editor-1.3.1/coop_html_editor/static/aloha.0.23.26/plugins/extra/flag-icons/img/flags/hi.png
--rw-r--r--   0 lucjean    (501) staff       (20)      369 2019-08-29 13:07:39.000000 coop_html_editor-1.3.1/coop_html_editor/static/aloha.0.23.26/plugins/extra/flag-icons/img/flags/gf.png
--rw-r--r--   0 lucjean    (501) staff       (20)      378 2019-08-29 13:07:39.000000 coop_html_editor-1.3.1/coop_html_editor/static/aloha.0.23.26/plugins/extra/flag-icons/img/flags/en.png
--rw-r--r--   0 lucjean    (501) staff       (20)      430 2019-08-29 13:07:39.000000 coop_html_editor-1.3.1/coop_html_editor/static/aloha.0.23.26/plugins/extra/flag-icons/img/flags/dj.png
--rw-r--r--   0 lucjean    (501) staff       (20)      405 2019-08-29 13:07:39.000000 coop_html_editor-1.3.1/coop_html_editor/static/aloha.0.23.26/plugins/extra/flag-icons/img/flags/gq.png
--rw-r--r--   0 lucjean    (501) staff       (20)      353 2019-08-29 13:07:39.000000 coop_html_editor-1.3.1/coop_html_editor/static/aloha.0.23.26/plugins/extra/flag-icons/img/flags/gp.png
--rw-r--r--   0 lucjean    (501) staff       (20)      352 2019-08-29 13:07:39.000000 coop_html_editor-1.3.1/coop_html_editor/static/aloha.0.23.26/plugins/extra/flag-icons/img/flags/dk.png
--rw-r--r--   0 lucjean    (501) staff       (20)      144 2019-08-29 13:07:39.000000 coop_html_editor-1.3.1/coop_html_editor/static/aloha.0.23.26/plugins/extra/flag-icons/img/flags/eo.png
--rw-r--r--   0 lucjean    (501) staff       (20)      249 2019-08-29 13:07:39.000000 coop_html_editor-1.3.1/coop_html_editor/static/aloha.0.23.26/plugins/extra/flag-icons/img/flags/ks.png
--rw-r--r--   0 lucjean    (501) staff       (20)      326 2019-08-29 13:07:39.000000 coop_html_editor-1.3.1/coop_html_editor/static/aloha.0.23.26/plugins/extra/flag-icons/img/flags/il.png
--rw-r--r--   0 lucjean    (501) staff       (20)      547 2019-08-29 13:07:40.000000 coop_html_editor-1.3.1/coop_html_editor/static/aloha.0.23.26/plugins/extra/flag-icons/img/flags/pn.png
--rw-r--r--   0 lucjean    (501) staff       (20)       86 2019-08-29 13:07:40.000000 coop_html_editor-1.3.1/coop_html_editor/static/aloha.0.23.26/plugins/extra/flag-icons/img/flags/su.png
--rw-r--r--   0 lucjean    (501) staff       (20)      520 2019-08-29 13:07:40.000000 coop_html_editor-1.3.1/coop_html_editor/static/aloha.0.23.26/plugins/extra/flag-icons/img/flags/sb.png
--rw-r--r--   0 lucjean    (501) staff       (20)      344 2019-08-29 13:07:40.000000 coop_html_editor-1.3.1/coop_html_editor/static/aloha.0.23.26/plugins/extra/flag-icons/img/flags/py.png
--rw-r--r--   0 lucjean    (501) staff       (20)      299 2019-08-29 13:07:40.000000 coop_html_editor-1.3.1/coop_html_editor/static/aloha.0.23.26/plugins/extra/flag-icons/img/flags/ru.png
--rw-r--r--   0 lucjean    (501) staff       (20)      266 2019-08-29 13:07:40.000000 coop_html_editor-1.3.1/coop_html_editor/static/aloha.0.23.26/plugins/extra/flag-icons/img/flags/sq.png
--rw-r--r--   0 lucjean    (501) staff       (20)      351 2019-08-29 13:07:39.000000 coop_html_editor-1.3.1/coop_html_editor/static/aloha.0.23.26/plugins/extra/flag-icons/img/flags/kw.png
--rw-r--r--   0 lucjean    (501) staff       (20)      368 2019-08-29 13:07:39.000000 coop_html_editor-1.3.1/coop_html_editor/static/aloha.0.23.26/plugins/extra/flag-icons/img/flags/do.png
--rw-r--r--   0 lucjean    (501) staff       (20)      333 2019-08-29 13:07:39.000000 coop_html_editor-1.3.1/coop_html_editor/static/aloha.0.23.26/plugins/extra/flag-icons/img/flags/gt.png
--rw-r--r--   0 lucjean    (501) staff       (20)      545 2019-08-29 13:07:39.000000 coop_html_editor-1.3.1/coop_html_editor/static/aloha.0.23.26/plugins/extra/flag-icons/img/flags/gb.png
--rw-r--r--   0 lucjean    (501) staff       (20)      178 2019-08-29 13:07:39.000000 coop_html_editor-1.3.1/coop_html_editor/static/aloha.0.23.26/plugins/extra/flag-icons/img/flags/ff.png
--rw-r--r--   0 lucjean    (501) staff       (20)      384 2019-08-29 13:07:39.000000 coop_html_editor-1.3.1/coop_html_editor/static/aloha.0.23.26/plugins/extra/flag-icons/img/flags/gu.png
--rw-r--r--   0 lucjean    (501) staff       (20)      162 2019-08-29 13:07:39.000000 coop_html_editor-1.3.1/coop_html_editor/static/aloha.0.23.26/plugins/extra/flag-icons/img/flags/ka.png
--rw-r--r--   0 lucjean    (501) staff       (20)       92 2019-08-29 13:07:39.000000 coop_html_editor-1.3.1/coop_html_editor/static/aloha.0.23.26/plugins/extra/flag-icons/img/flags/hz.png
--rw-r--r--   0 lucjean    (501) staff       (20)      580 2019-08-29 13:07:39.000000 coop_html_editor-1.3.1/coop_html_editor/static/aloha.0.23.26/plugins/extra/flag-icons/img/flags/hm.png
--rw-r--r--   0 lucjean    (501) staff       (20)       95 2019-08-29 13:07:39.000000 coop_html_editor-1.3.1/coop_html_editor/static/aloha.0.23.26/plugins/extra/flag-icons/img/flags/kv.png
--rw-r--r--   0 lucjean    (501) staff       (20)      349 2019-08-29 13:07:39.000000 coop_html_editor-1.3.1/coop_html_editor/static/aloha.0.23.26/plugins/extra/flag-icons/img/flags/ii.png
--rw-r--r--   0 lucjean    (501) staff       (20)      350 2019-08-29 13:07:40.000000 coop_html_editor-1.3.1/coop_html_editor/static/aloha.0.23.26/plugins/extra/flag-icons/img/flags/sg.png
--rw-r--r--   0 lucjean    (501) staff       (20)      448 2019-08-29 13:07:40.000000 coop_html_editor-1.3.1/coop_html_editor/static/aloha.0.23.26/plugins/extra/flag-icons/img/flags/pk.png
--rw-r--r--   0 lucjean    (501) staff       (20)      370 2019-08-29 13:07:40.000000 coop_html_editor-1.3.1/coop_html_editor/static/aloha.0.23.26/plugins/extra/flag-icons/img/flags/sr.png
--rw-r--r--   0 lucjean    (501) staff       (20)      389 2019-08-29 13:07:40.000000 coop_html_editor-1.3.1/coop_html_editor/static/aloha.0.23.26/plugins/extra/flag-icons/img/flags/se.png
--rw-r--r--   0 lucjean    (501) staff       (20)      323 2019-08-29 13:07:39.000000 coop_html_editor-1.3.1/coop_html_editor/static/aloha.0.23.26/plugins/extra/flag-icons/img/flags/ho.png
--rw-r--r--   0 lucjean    (501) staff       (20)      307 2019-08-29 13:07:39.000000 coop_html_editor-1.3.1/coop_html_editor/static/aloha.0.23.26/plugins/extra/flag-icons/img/flags/jp.png
--rw-r--r--   0 lucjean    (501) staff       (20)      346 2019-08-29 13:07:39.000000 coop_html_editor-1.3.1/coop_html_editor/static/aloha.0.23.26/plugins/extra/flag-icons/img/flags/gw.png
--rw-r--r--   0 lucjean    (501) staff       (20)      388 2019-08-29 13:07:39.000000 coop_html_editor-1.3.1/coop_html_editor/static/aloha.0.23.26/plugins/extra/flag-icons/img/flags/eh.png
--rw-r--r--   0 lucjean    (501) staff       (20)      454 2019-08-29 13:07:39.000000 coop_html_editor-1.3.1/coop_html_editor/static/aloha.0.23.26/plugins/extra/flag-icons/img/flags/dz.png
--rw-r--r--   0 lucjean    (501) staff       (20)      342 2019-08-29 13:07:39.000000 coop_html_editor-1.3.1/coop_html_editor/static/aloha.0.23.26/plugins/extra/flag-icons/img/flags/ga.png
--rw-r--r--   0 lucjean    (501) staff       (20)      369 2019-08-29 13:07:39.000000 coop_html_editor-1.3.1/coop_html_editor/static/aloha.0.23.26/plugins/extra/flag-icons/img/flags/fr.png
--rw-r--r--   0 lucjean    (501) staff       (20)      219 2019-08-29 13:07:39.000000 coop_html_editor-1.3.1/coop_html_editor/static/aloha.0.23.26/plugins/extra/flag-icons/img/flags/gv.png
--rw-r--r--   0 lucjean    (501) staff       (20)      508 2019-08-29 13:07:39.000000 coop_html_editor-1.3.1/coop_html_editor/static/aloha.0.23.26/plugins/extra/flag-icons/img/flags/dm.png
--rw-r--r--   0 lucjean    (501) staff       (20)      121 2019-08-29 13:07:39.000000 coop_html_editor-1.3.1/coop_html_editor/static/aloha.0.23.26/plugins/extra/flag-icons/img/flags/hy.png
--rw-r--r--   0 lucjean    (501) staff       (20)      411 2019-08-29 13:07:39.000000 coop_html_editor-1.3.1/coop_html_editor/static/aloha.0.23.26/plugins/extra/flag-icons/img/flags/hn.png
--rw-r--r--   0 lucjean    (501) staff       (20)      183 2019-08-29 13:07:39.000000 coop_html_editor-1.3.1/coop_html_editor/static/aloha.0.23.26/plugins/extra/flag-icons/img/flags/ku.png
--rw-r--r--   0 lucjean    (501) staff       (20)      364 2019-08-29 13:07:40.000000 coop_html_editor-1.3.1/coop_html_editor/static/aloha.0.23.26/plugins/extra/flag-icons/img/flags/sd.png
--rw-r--r--   0 lucjean    (501) staff       (20)      382 2019-08-29 13:07:40.000000 coop_html_editor-1.3.1/coop_html_editor/static/aloha.0.23.26/plugins/extra/flag-icons/img/flags/rw.png
--rw-r--r--   0 lucjean    (501) staff       (20)      416 2019-08-29 13:07:40.000000 coop_html_editor-1.3.1/coop_html_editor/static/aloha.0.23.26/plugins/extra/flag-icons/img/flags/ph.png
--rw-r--r--   0 lucjean    (501) staff       (20)      260 2019-08-29 13:07:40.000000 coop_html_editor-1.3.1/coop_html_editor/static/aloha.0.23.26/plugins/extra/flag-icons/img/flags/ss.png
--rw-r--r--   0 lucjean    (501) staff       (20)      343 2019-08-29 13:07:40.000000 coop_html_editor-1.3.1/coop_html_editor/static/aloha.0.23.26/plugins/extra/flag-icons/img/flags/qa.png
--rw-r--r--   0 lucjean    (501) staff       (20)      264 2019-08-29 13:07:40.000000 coop_html_editor-1.3.1/coop_html_editor/static/aloha.0.23.26/plugins/extra/flag-icons/img/flags/pe.png
--rw-r--r--   0 lucjean    (501) staff       (20)      333 2019-08-29 13:07:40.000000 coop_html_editor-1.3.1/coop_html_editor/static/aloha.0.23.26/plugins/extra/flag-icons/img/flags/rm.png
--rw-r--r--   0 lucjean    (501) staff       (20)      445 2019-08-29 13:07:40.000000 coop_html_editor-1.3.1/coop_html_editor/static/aloha.0.23.26/plugins/extra/flag-icons/img/flags/pr.png
--rw-r--r--   0 lucjean    (501) staff       (20)      383 2019-08-29 13:07:40.000000 coop_html_editor-1.3.1/coop_html_editor/static/aloha.0.23.26/plugins/extra/flag-icons/img/flags/si.png
--rw-r--r--   0 lucjean    (501) staff       (20)       86 2019-08-29 13:07:39.000000 coop_html_editor-1.3.1/coop_html_editor/static/aloha.0.23.26/plugins/extra/flag-icons/img/flags/ig.png
--rw-r--r--   0 lucjean    (501) staff       (20)      327 2019-08-29 13:07:39.000000 coop_html_editor-1.3.1/coop_html_editor/static/aloha.0.23.26/plugins/extra/flag-icons/img/flags/ht.png
--rw-r--r--   0 lucjean    (501) staff       (20)      507 2019-08-29 13:07:39.000000 coop_html_editor-1.3.1/coop_html_editor/static/aloha.0.23.26/plugins/extra/flag-icons/img/flags/ko.png
--rw-r--r--   0 lucjean    (501) staff       (20)      344 2019-08-29 13:07:39.000000 coop_html_editor-1.3.1/coop_html_editor/static/aloha.0.23.26/plugins/extra/flag-icons/img/flags/es.png
--rw-r--r--   0 lucjean    (501) staff       (20)      351 2019-08-29 13:07:39.000000 coop_html_editor-1.3.1/coop_html_editor/static/aloha.0.23.26/plugins/extra/flag-icons/img/flags/gl.png
--rw-r--r--   0 lucjean    (501) staff       (20)      173 2019-08-29 13:07:39.000000 coop_html_editor-1.3.1/coop_html_editor/static/aloha.0.23.26/plugins/extra/flag-icons/img/flags/dv.png
--rw-r--r--   0 lucjean    (501) staff       (20)      363 2019-08-29 13:07:39.000000 coop_html_editor-1.3.1/coop_html_editor/static/aloha.0.23.26/plugins/extra/flag-icons/img/flags/gm.png
--rw-r--r--   0 lucjean    (501) staff       (20)      497 2019-08-29 13:07:39.000000 coop_html_editor-1.3.1/coop_html_editor/static/aloha.0.23.26/plugins/extra/flag-icons/img/flags/er.png
--rw-r--r--   0 lucjean    (501) staff       (20)      368 2019-08-29 13:07:39.000000 coop_html_editor-1.3.1/coop_html_editor/static/aloha.0.23.26/plugins/extra/flag-icons/img/flags/fi.png
--rw-r--r--   0 lucjean    (501) staff       (20)      352 2019-08-29 13:07:39.000000 coop_html_editor-1.3.1/coop_html_editor/static/aloha.0.23.26/plugins/extra/flag-icons/img/flags/da.png
--rw-r--r--   0 lucjean    (501) staff       (20)      297 2019-08-29 13:07:39.000000 coop_html_editor-1.3.1/coop_html_editor/static/aloha.0.23.26/plugins/extra/flag-icons/img/flags/ee.png
--rw-r--r--   0 lucjean    (501) staff       (20)      480 2019-08-29 13:07:39.000000 coop_html_editor-1.3.1/coop_html_editor/static/aloha.0.23.26/plugins/extra/flag-icons/img/flags/kn.png
--rw-r--r--   0 lucjean    (501) staff       (20)      293 2019-08-29 13:07:39.000000 coop_html_editor-1.3.1/coop_html_editor/static/aloha.0.23.26/plugins/extra/flag-icons/img/flags/hu.png
--rw-r--r--   0 lucjean    (501) staff       (20)      403 2019-08-29 13:07:39.000000 coop_html_editor-1.3.1/coop_html_editor/static/aloha.0.23.26/plugins/extra/flag-icons/img/flags/iq.png
--rw-r--r--   0 lucjean    (501) staff       (20)      532 2019-08-29 13:07:39.000000 coop_html_editor-1.3.1/coop_html_editor/static/aloha.0.23.26/plugins/extra/flag-icons/img/flags/ky.png
--rw-r--r--   0 lucjean    (501) staff       (20)      524 2019-08-29 13:07:40.000000 coop_html_editor-1.3.1/coop_html_editor/static/aloha.0.23.26/plugins/extra/flag-icons/img/flags/sh.png
--rw-r--r--   0 lucjean    (501) staff       (20)      348 2019-08-29 13:07:40.000000 coop_html_editor-1.3.1/coop_html_editor/static/aloha.0.23.26/plugins/extra/flag-icons/img/flags/ps.png
--rw-r--r--   0 lucjean    (501) staff       (20)      379 2019-08-29 13:07:40.000000 coop_html_editor-1.3.1/coop_html_editor/static/aloha.0.23.26/plugins/extra/flag-icons/img/flags/pf.png
--rw-r--r--   0 lucjean    (501) staff       (20)      397 2019-08-29 13:07:40.000000 coop_html_editor-1.3.1/coop_html_editor/static/aloha.0.23.26/plugins/extra/flag-icons/img/flags/sj.png
--rw-r--r--   0 lucjean    (501) staff       (20)      357 2019-08-29 13:07:40.000000 coop_html_editor-1.3.1/coop_html_editor/static/aloha.0.23.26/plugins/extra/flag-icons/img/flags/rn.png
--rw-r--r--   0 lucjean    (501) staff       (20)      301 2019-08-29 13:07:39.000000 coop_html_editor-1.3.1/coop_html_editor/static/aloha.0.23.26/plugins/extra/flag-icons/img/flags/id.png
--rw-r--r--   0 lucjean    (501) staff       (20)      268 2019-08-29 13:07:39.000000 coop_html_editor-1.3.1/coop_html_editor/static/aloha.0.23.26/plugins/extra/flag-icons/img/flags/kl.png
--rw-r--r--   0 lucjean    (501) staff       (20)      410 2019-08-29 13:07:39.000000 coop_html_editor-1.3.1/coop_html_editor/static/aloha.0.23.26/plugins/extra/flag-icons/img/flags/is.png
--rw-r--r--   0 lucjean    (501) staff       (20)      348 2019-08-29 13:07:39.000000 coop_html_editor-1.3.1/coop_html_editor/static/aloha.0.23.26/plugins/extra/flag-icons/img/flags/eg.png
--rw-r--r--   0 lucjean    (501) staff       (20)      526 2019-08-29 13:07:39.000000 coop_html_editor-1.3.1/coop_html_editor/static/aloha.0.23.26/plugins/extra/flag-icons/img/flags/fk.png
--rw-r--r--   0 lucjean    (501) staff       (20)      517 2019-08-29 13:07:39.000000 coop_html_editor-1.3.1/coop_html_editor/static/aloha.0.23.26/plugins/extra/flag-icons/img/flags/fj.png
--rw-r--r--   0 lucjean    (501) staff       (20)      319 2019-08-29 13:07:39.000000 coop_html_editor-1.3.1/coop_html_editor/static/aloha.0.23.26/plugins/extra/flag-icons/img/flags/gn.png
--rw-r--r--   0 lucjean    (501) staff       (20)      521 2019-08-29 13:07:39.000000 coop_html_editor-1.3.1/coop_html_editor/static/aloha.0.23.26/plugins/extra/flag-icons/img/flags/gy.png
--rw-r--r--   0 lucjean    (501) staff       (20)      398 2019-08-29 13:07:39.000000 coop_html_editor-1.3.1/coop_html_editor/static/aloha.0.23.26/plugins/extra/flag-icons/img/flags/ir.png
--rw-r--r--   0 lucjean    (501) staff       (20)      456 2019-08-29 13:07:39.000000 coop_html_editor-1.3.1/coop_html_editor/static/aloha.0.23.26/plugins/extra/flag-icons/img/flags/km.png
--rw-r--r--   0 lucjean    (501) staff       (20)      333 2019-08-29 13:07:39.000000 coop_html_editor-1.3.1/coop_html_editor/static/aloha.0.23.26/plugins/extra/flag-icons/img/flags/ie.png
--rw-r--r--   0 lucjean    (501) staff       (20)      341 2019-08-29 13:07:39.000000 coop_html_editor-1.3.1/coop_html_editor/static/aloha.0.23.26/plugins/extra/flag-icons/img/flags/ha.png
--rw-r--r--   0 lucjean    (501) staff       (20)      459 2019-08-29 13:07:39.000000 coop_html_editor-1.3.1/coop_html_editor/static/aloha.0.23.26/plugins/extra/flag-icons/img/flags/kz.png
--rw-r--r--   0 lucjean    (501) staff       (20)      333 2019-08-29 13:07:40.000000 coop_html_editor-1.3.1/coop_html_editor/static/aloha.0.23.26/plugins/extra/flag-icons/img/flags/ro.png
--rw-r--r--   0 lucjean    (501) staff       (20)      439 2019-08-29 13:07:40.000000 coop_html_editor-1.3.1/coop_html_editor/static/aloha.0.23.26/plugins/extra/flag-icons/img/flags/sk.png
--rw-r--r--   0 lucjean    (501) staff       (20)      438 2019-08-29 13:07:40.000000 coop_html_editor-1.3.1/coop_html_editor/static/aloha.0.23.26/plugins/extra/flag-icons/img/flags/pg.png
--rw-r--r--   0 lucjean    (501) staff       (20)      407 2019-08-29 13:07:40.000000 coop_html_editor-1.3.1/coop_html_editor/static/aloha.0.23.26/plugins/extra/flag-icons/img/flags/pt.png
--rw-r--r--   0 lucjean    (501) staff       (20)      376 2019-08-29 13:07:40.000000 coop_html_editor-1.3.1/coop_html_editor/static/aloha.0.23.26/plugins/extra/flag-icons/img/flags/so.png
--rw-r--r--   0 lucjean    (501) staff       (20)      386 2019-08-29 13:07:39.000000 coop_html_editor-1.3.1/coop_html_editor/static/aloha.0.23.26/plugins/extra/flag-icons/img/flags/hr.png
--rw-r--r--   0 lucjean    (501) staff       (20)      523 2019-08-29 13:07:39.000000 coop_html_editor-1.3.1/coop_html_editor/static/aloha.0.23.26/plugins/extra/flag-icons/img/flags/ki.png
--rw-r--r--   0 lucjean    (501) staff       (20)      508 2019-08-29 13:07:39.000000 coop_html_editor-1.3.1/coop_html_editor/static/aloha.0.23.26/plugins/extra/flag-icons/img/flags/jm.png
--rw-r--r--   0 lucjean    (501) staff       (20)      161 2019-08-29 13:07:39.000000 coop_html_editor-1.3.1/coop_html_editor/static/aloha.0.23.26/plugins/extra/flag-icons/img/flags/he.png
--rw-r--r--   0 lucjean    (501) staff       (20)      227 2019-08-29 13:07:39.000000 coop_html_editor-1.3.1/coop_html_editor/static/aloha.0.23.26/plugins/extra/flag-icons/img/flags/eu.png
--rw-r--r--   0 lucjean    (501) staff       (20)      590 2019-08-29 13:07:39.000000 coop_html_editor-1.3.1/coop_html_editor/static/aloha.0.23.26/plugins/extra/flag-icons/img/flags/fy.png
--rw-r--r--   0 lucjean    (501) staff       (20)      355 2019-08-29 13:07:39.000000 coop_html_editor-1.3.1/coop_html_editor/static/aloha.0.23.26/plugins/extra/flag-icons/img/flags/ec.png
--rw-r--r--   0 lucjean    (501) staff       (20)      445 2019-08-29 13:07:39.000000 coop_html_editor-1.3.1/coop_html_editor/static/aloha.0.23.26/plugins/extra/flag-icons/img/flags/et.png
--rw-r--r--   0 lucjean    (501) staff       (20)      377 2019-08-29 13:07:39.000000 coop_html_editor-1.3.1/coop_html_editor/static/aloha.0.23.26/plugins/extra/flag-icons/img/flags/fo.png
--rw-r--r--   0 lucjean    (501) staff       (20)      422 2019-08-29 13:07:39.000000 coop_html_editor-1.3.1/coop_html_editor/static/aloha.0.23.26/plugins/extra/flag-icons/img/flags/kh.png
--rw-r--r--   0 lucjean    (501) staff       (20)      322 2019-08-29 13:07:40.000000 coop_html_editor-1.3.1/coop_html_editor/static/aloha.0.23.26/plugins/extra/flag-icons/img/flags/sy.png
--rw-r--r--   0 lucjean    (501) staff       (20)      356 2019-08-29 13:07:40.000000 coop_html_editor-1.3.1/coop_html_editor/static/aloha.0.23.26/plugins/extra/flag-icons/img/flags/sn.png
--rw-r--r--   0 lucjean    (501) staff       (20)      424 2019-08-29 13:07:40.000000 coop_html_editor-1.3.1/coop_html_editor/static/aloha.0.23.26/plugins/extra/flag-icons/img/flags/pw.png
--rw-r--r--   0 lucjean    (501) staff       (20)      321 2019-08-29 13:07:40.000000 coop_html_editor-1.3.1/coop_html_editor/static/aloha.0.23.26/plugins/extra/flag-icons/img/flags/sl.png
--rw-r--r--   0 lucjean    (501) staff       (20)      409 2019-08-29 13:07:39.000000 coop_html_editor-1.3.1/coop_html_editor/static/aloha.0.23.26/plugins/extra/flag-icons/img/flags/fm.png
--rw-r--r--   0 lucjean    (501) staff       (20)      369 2019-08-29 13:07:39.000000 coop_html_editor-1.3.1/coop_html_editor/static/aloha.0.23.26/plugins/extra/flag-icons/img/flags/gi.png
--rw-r--r--   0 lucjean    (501) staff       (20)      364 2019-08-29 13:07:39.000000 coop_html_editor-1.3.1/coop_html_editor/static/aloha.0.23.26/plugins/extra/flag-icons/img/flags/de.png
--rw-r--r--   0 lucjean    (501) staff       (20)      336 2019-08-29 13:07:39.000000 coop_html_editor-1.3.1/coop_html_editor/static/aloha.0.23.26/plugins/extra/flag-icons/img/flags/gh.png
--rw-r--r--   0 lucjean    (501) staff       (20)      234 2019-08-29 13:07:39.000000 coop_html_editor-1.3.1/coop_html_editor/static/aloha.0.23.26/plugins/extra/flag-icons/img/flags/kk.png
--rw-r--r--   0 lucjean    (501) staff       (20)      353 2019-08-29 13:07:39.000000 coop_html_editor-1.3.1/coop_html_editor/static/aloha.0.23.26/plugins/extra/flag-icons/img/flags/jo.png
--rw-r--r--   0 lucjean    (501) staff       (20)      283 2019-08-29 13:07:39.000000 coop_html_editor-1.3.1/coop_html_editor/static/aloha.0.23.26/plugins/extra/flag-icons/img/flags/it.png
--rw-r--r--   0 lucjean    (501) staff       (20)      390 2019-08-29 13:07:40.000000 coop_html_editor-1.3.1/coop_html_editor/static/aloha.0.23.26/plugins/extra/flag-icons/img/flags/pa.png
--rw-r--r--   0 lucjean    (501) staff       (20)      508 2019-08-29 13:07:40.000000 coop_html_editor-1.3.1/coop_html_editor/static/aloha.0.23.26/plugins/extra/flag-icons/img/flags/sz.png
--rw-r--r--   0 lucjean    (501) staff       (20)      396 2019-08-29 13:07:40.000000 coop_html_editor-1.3.1/coop_html_editor/static/aloha.0.23.26/plugins/extra/flag-icons/img/flags/sm.png
--rw-r--r--   0 lucjean    (501) staff       (20)      185 2019-08-29 13:07:40.000000 coop_html_editor-1.3.1/coop_html_editor/static/aloha.0.23.26/plugins/extra/flag-icons/img/flags/ty.png
--rw-r--r--   0 lucjean    (501) staff       (20)      367 2019-08-29 13:07:40.000000 coop_html_editor-1.3.1/coop_html_editor/static/aloha.0.23.26/plugins/extra/flag-icons/img/flags/tn.png
--rw-r--r--   0 lucjean    (501) staff       (20)       92 2019-08-29 13:07:40.000000 coop_html_editor-1.3.1/coop_html_editor/static/aloha.0.23.26/plugins/extra/flag-icons/img/flags/os.png
--rw-r--r--   0 lucjean    (501) staff       (20)      322 2019-08-29 13:07:39.000000 coop_html_editor-1.3.1/coop_html_editor/static/aloha.0.23.26/plugins/extra/flag-icons/img/flags/ml.png
--rw-r--r--   0 lucjean    (501) staff       (20)      380 2019-08-29 13:07:39.000000 coop_html_editor-1.3.1/coop_html_editor/static/aloha.0.23.26/plugins/extra/flag-icons/img/flags/cg.png
--rw-r--r--   0 lucjean    (501) staff       (20)      480 2019-08-29 13:07:39.000000 coop_html_editor-1.3.1/coop_html_editor/static/aloha.0.23.26/plugins/extra/flag-icons/img/flags/ax.png
--rw-r--r--   0 lucjean    (501) staff       (20)      395 2019-08-29 13:07:39.000000 coop_html_editor-1.3.1/coop_html_editor/static/aloha.0.23.26/plugins/extra/flag-icons/img/flags/ao.png
--rw-r--r--   0 lucjean    (501) staff       (20)      471 2019-08-29 13:07:39.000000 coop_html_editor-1.3.1/coop_html_editor/static/aloha.0.23.26/plugins/extra/flag-icons/img/flags/bt.png
--rw-r--r--   0 lucjean    (501) staff       (20)      365 2019-08-29 13:07:39.000000 coop_html_editor-1.3.1/coop_html_editor/static/aloha.0.23.26/plugins/extra/flag-icons/img/flags/an.png
--rw-r--r--   0 lucjean    (501) staff       (20)      525 2019-08-29 13:07:39.000000 coop_html_editor-1.3.1/coop_html_editor/static/aloha.0.23.26/plugins/extra/flag-icons/img/flags/ay.png
--rw-r--r--   0 lucjean    (501) staff       (20)      403 2019-08-29 13:07:39.000000 coop_html_editor-1.3.1/coop_html_editor/static/aloha.0.23.26/plugins/extra/flag-icons/img/flags/bb.png
--rw-r--r--   0 lucjean    (501) staff       (20)      456 2019-08-29 13:07:39.000000 coop_html_editor-1.3.1/coop_html_editor/static/aloha.0.23.26/plugins/extra/flag-icons/img/flags/cf.png
--rw-r--r--   0 lucjean    (501) staff       (20)      336 2019-08-29 13:07:39.000000 coop_html_editor-1.3.1/coop_html_editor/static/aloha.0.23.26/plugins/extra/flag-icons/img/flags/mm.png
--rw-r--r--   0 lucjean    (501) staff       (20)      432 2019-08-29 13:07:40.000000 coop_html_editor-1.3.1/coop_html_editor/static/aloha.0.23.26/plugins/extra/flag-icons/img/flags/nv.png
--rw-r--r--   0 lucjean    (501) staff       (20)      399 2019-08-29 13:07:39.000000 coop_html_editor-1.3.1/coop_html_editor/static/aloha.0.23.26/plugins/extra/flag-icons/img/flags/li.png
--rw-r--r--   0 lucjean    (501) staff       (20)      377 2019-08-29 13:07:40.000000 coop_html_editor-1.3.1/coop_html_editor/static/aloha.0.23.26/plugins/extra/flag-icons/img/flags/or.png
--rw-r--r--   0 lucjean    (501) staff       (20)      559 2019-08-29 13:07:40.000000 coop_html_editor-1.3.1/coop_html_editor/static/aloha.0.23.26/plugins/extra/flag-icons/img/flags/na.png
--rw-r--r--   0 lucjean    (501) staff       (20)      439 2019-08-29 13:07:40.000000 coop_html_editor-1.3.1/coop_html_editor/static/aloha.0.23.26/plugins/extra/flag-icons/img/flags/mz.png
--rw-r--r--   0 lucjean    (501) staff       (20)      324 2019-08-29 13:07:40.000000 coop_html_editor-1.3.1/coop_html_editor/static/aloha.0.23.26/plugins/extra/flag-icons/img/flags/uk.png
--rw-r--r--   0 lucjean    (501) staff       (20)      302 2019-08-29 13:07:40.000000 coop_html_editor-1.3.1/coop_html_editor/static/aloha.0.23.26/plugins/extra/flag-icons/img/flags/to.png
--rw-r--r--   0 lucjean    (501) staff       (20)      510 2019-08-29 13:07:40.000000 coop_html_editor-1.3.1/coop_html_editor/static/aloha.0.23.26/plugins/extra/flag-icons/img/flags/vg.png
--rw-r--r--   0 lucjean    (501) staff       (20)      412 2019-08-29 13:07:40.000000 coop_html_editor-1.3.1/coop_html_editor/static/aloha.0.23.26/plugins/extra/flag-icons/img/flags/ve.png
--rw-r--r--   0 lucjean    (501) staff       (20)      514 2019-08-29 13:07:40.000000 coop_html_editor-1.3.1/coop_html_editor/static/aloha.0.23.26/plugins/extra/flag-icons/img/flags/tz.png
--rw-r--r--   0 lucjean    (501) staff       (20)      294 2019-08-29 13:07:40.000000 coop_html_editor-1.3.1/coop_html_editor/static/aloha.0.23.26/plugins/extra/flag-icons/img/flags/wa.png
--rw-r--r--   0 lucjean    (501) staff       (20)      456 2019-08-29 13:07:40.000000 coop_html_editor-1.3.1/coop_html_editor/static/aloha.0.23.26/plugins/extra/flag-icons/img/flags/tm.png
--rw-r--r--   0 lucjean    (501) staff       (20)      424 2019-08-29 13:07:40.000000 coop_html_editor-1.3.1/coop_html_editor/static/aloha.0.23.26/plugins/extra/flag-icons/img/flags/mx.png
--rw-r--r--   0 lucjean    (501) staff       (20)      470 2019-08-29 13:07:40.000000 coop_html_editor-1.3.1/coop_html_editor/static/aloha.0.23.26/plugins/extra/flag-icons/img/flags/nc.png
--rw-r--r--   0 lucjean    (501) staff       (20)      456 2019-08-29 13:07:39.000000 coop_html_editor-1.3.1/coop_html_editor/static/aloha.0.23.26/plugins/extra/flag-icons/img/flags/mo.png
--rw-r--r--   0 lucjean    (501) staff       (20)      464 2019-08-29 13:07:39.000000 coop_html_editor-1.3.1/coop_html_editor/static/aloha.0.23.26/plugins/extra/flag-icons/img/flags/lk.png
--rw-r--r--   0 lucjean    (501) staff       (20)      477 2019-08-29 13:07:39.000000 coop_html_editor-1.3.1/coop_html_editor/static/aloha.0.23.26/plugins/extra/flag-icons/img/flags/cd.png
--rw-r--r--   0 lucjean    (501) staff       (20)      434 2019-08-29 13:07:39.000000 coop_html_editor-1.3.1/coop_html_editor/static/aloha.0.23.26/plugins/extra/flag-icons/img/flags/al.png
--rw-r--r--   0 lucjean    (501) staff       (20)      327 2019-08-29 13:07:39.000000 coop_html_editor-1.3.1/coop_html_editor/static/aloha.0.23.26/plugins/extra/flag-icons/img/flags/bw.png
--rw-r--r--   0 lucjean    (501) staff       (20)      321 2019-08-29 13:07:39.000000 coop_html_editor-1.3.1/coop_html_editor/static/aloha.0.23.26/plugins/extra/flag-icons/img/flags/cs.png
--rw-r--r--   0 lucjean    (501) staff       (20)      349 2019-08-29 13:07:39.000000 coop_html_editor-1.3.1/coop_html_editor/static/aloha.0.23.26/plugins/extra/flag-icons/img/flags/cr.png
--rw-r--r--   0 lucjean    (501) staff       (20)      397 2019-08-29 13:07:39.000000 coop_html_editor-1.3.1/coop_html_editor/static/aloha.0.23.26/plugins/extra/flag-icons/img/flags/bv.png
--rw-r--r--   0 lucjean    (501) staff       (20)      332 2019-08-29 13:07:39.000000 coop_html_editor-1.3.1/coop_html_editor/static/aloha.0.23.26/plugins/extra/flag-icons/img/flags/am.png
--rw-r--r--   0 lucjean    (501) staff       (20)      110 2019-08-29 13:07:39.000000 coop_html_editor-1.3.1/coop_html_editor/static/aloha.0.23.26/plugins/extra/flag-icons/img/flags/ce.png
--rw-r--r--   0 lucjean    (501) staff       (20)      423 2019-08-29 13:07:39.000000 coop_html_editor-1.3.1/coop_html_editor/static/aloha.0.23.26/plugins/extra/flag-icons/img/flags/az.png
--rw-r--r--   0 lucjean    (501) staff       (20)      471 2019-08-29 13:07:39.000000 coop_html_editor-1.3.1/coop_html_editor/static/aloha.0.23.26/plugins/extra/flag-icons/img/flags/ba.png
--rw-r--r--   0 lucjean    (501) staff       (20)      343 2019-08-29 13:07:39.000000 coop_html_editor-1.3.1/coop_html_editor/static/aloha.0.23.26/plugins/extra/flag-icons/img/flags/mn.png
--rw-r--r--   0 lucjean    (501) staff       (20)      468 2019-08-29 13:07:40.000000 coop_html_editor-1.3.1/coop_html_editor/static/aloha.0.23.26/plugins/extra/flag-icons/img/flags/nu.png
--rw-r--r--   0 lucjean    (501) staff       (20)      397 2019-08-29 13:07:40.000000 coop_html_editor-1.3.1/coop_html_editor/static/aloha.0.23.26/plugins/extra/flag-icons/img/flags/nb.png
--rw-r--r--   0 lucjean    (501) staff       (20)      464 2019-08-29 13:07:40.000000 coop_html_editor-1.3.1/coop_html_editor/static/aloha.0.23.26/plugins/extra/flag-icons/img/flags/my.png
--rw-r--r--   0 lucjean    (501) staff       (20)      418 2019-08-29 13:07:39.000000 coop_html_editor-1.3.1/coop_html_editor/static/aloha.0.23.26/plugins/extra/flag-icons/img/flags/europeanunion.png
--rw-r--r--   0 lucjean    (501) staff       (20)      395 2019-08-29 13:07:40.000000 coop_html_editor-1.3.1/coop_html_editor/static/aloha.0.23.26/plugins/extra/flag-icons/img/flags/tl.png
--rw-r--r--   0 lucjean    (501) staff       (20)      352 2019-08-29 13:07:40.000000 coop_html_editor-1.3.1/coop_html_editor/static/aloha.0.23.26/plugins/extra/flag-icons/img/flags/ws.png
--rw-r--r--   0 lucjean    (501) staff       (20)      327 2019-08-29 13:07:40.000000 coop_html_editor-1.3.1/coop_html_editor/static/aloha.0.23.26/plugins/extra/flag-icons/img/flags/th.png
--rw-r--r--   0 lucjean    (501) staff       (20)      251 2019-08-29 13:07:39.000000 coop_html_editor-1.3.1/coop_html_editor/static/aloha.0.23.26/plugins/extra/flag-icons/img/flags/ln.png
--rw-r--r--   0 lucjean    (501) staff       (20)      474 2019-08-29 13:07:40.000000 coop_html_editor-1.3.1/coop_html_editor/static/aloha.0.23.26/plugins/extra/flag-icons/img/flags/nf.png
--rw-r--r--   0 lucjean    (501) staff       (20)      277 2019-08-29 13:07:39.000000 coop_html_editor-1.3.1/coop_html_editor/static/aloha.0.23.26/plugins/extra/flag-icons/img/flags/ly.png
--rw-r--r--   0 lucjean    (501) staff       (20)      516 2019-08-29 13:07:39.000000 coop_html_editor-1.3.1/coop_html_editor/static/aloha.0.23.26/plugins/extra/flag-icons/img/flags/ai.png
--rw-r--r--   0 lucjean    (501) staff       (20)      486 2019-08-29 13:07:39.000000 coop_html_editor-1.3.1/coop_html_editor/static/aloha.0.23.26/plugins/extra/flag-icons/img/flags/br.png
--rw-r--r--   0 lucjean    (501) staff       (20)      441 2019-08-29 13:07:39.000000 coop_html_editor-1.3.1/coop_html_editor/static/aloha.0.23.26/plugins/extra/flag-icons/img/flags/cv.png
--rw-r--r--   0 lucjean    (501) staff       (20)      294 2019-08-29 13:07:39.000000 coop_html_editor-1.3.1/coop_html_editor/static/aloha.0.23.26/plugins/extra/flag-icons/img/flags/be.png
--rw-r--r--   0 lucjean    (501) staff       (20)      471 2019-08-29 13:07:39.000000 coop_html_editor-1.3.1/coop_html_editor/static/aloha.0.23.26/plugins/extra/flag-icons/img/flags/ca.png
--rw-r--r--   0 lucjean    (501) staff       (20)      372 2019-08-29 13:07:39.000000 coop_html_editor-1.3.1/coop_html_editor/static/aloha.0.23.26/plugins/extra/flag-icons/img/flags/bd.png
--rw-r--r--   0 lucjean    (501) staff       (20)      391 2019-08-29 13:07:39.000000 coop_html_editor-1.3.1/coop_html_editor/static/aloha.0.23.26/plugins/extra/flag-icons/img/flags/bs.png
--rw-r--r--   0 lucjean    (501) staff       (20)      369 2019-08-29 13:07:40.000000 coop_html_editor-1.3.1/coop_html_editor/static/aloha.0.23.26/plugins/extra/flag-icons/img/flags/oc.png
--rw-r--r--   0 lucjean    (501) staff       (20)      341 2019-08-29 13:07:40.000000 coop_html_editor-1.3.1/coop_html_editor/static/aloha.0.23.26/plugins/extra/flag-icons/img/flags/ng.png
--rw-r--r--   0 lucjean    (501) staff       (20)      149 2019-08-29 13:07:39.000000 coop_html_editor-1.3.1/coop_html_editor/static/aloha.0.23.26/plugins/extra/flag-icons/img/flags/lo.png
--rw-r--r--   0 lucjean    (501) staff       (20)      449 2019-08-29 13:07:39.000000 coop_html_editor-1.3.1/coop_html_editor/static/aloha.0.23.26/plugins/extra/flag-icons/img/flags/mk.png
--rw-r--r--   0 lucjean    (501) staff       (20)      349 2019-08-29 13:07:40.000000 coop_html_editor-1.3.1/coop_html_editor/static/aloha.0.23.26/plugins/extra/flag-icons/img/flags/np.png
--rw-r--r--   0 lucjean    (501) staff       (20)      419 2019-08-29 13:07:40.000000 coop_html_editor-1.3.1/coop_html_editor/static/aloha.0.23.26/plugins/extra/flag-icons/img/flags/va.png
--rw-r--r--   0 lucjean    (501) staff       (20)      411 2019-08-29 13:07:40.000000 coop_html_editor-1.3.1/coop_html_editor/static/aloha.0.23.26/plugins/extra/flag-icons/img/flags/uz.png
--rw-r--r--   0 lucjean    (501) staff       (20)      557 2019-08-29 13:07:40.000000 coop_html_editor-1.3.1/coop_html_editor/static/aloha.0.23.26/plugins/extra/flag-icons/img/flags/wales.png
--rw-r--r--   0 lucjean    (501) staff       (20)      344 2019-08-29 13:07:40.000000 coop_html_editor-1.3.1/coop_html_editor/static/aloha.0.23.26/plugins/extra/flag-icons/img/flags/ti.png
--rw-r--r--   0 lucjean    (501) staff       (20)      455 2019-08-29 13:07:40.000000 coop_html_editor-1.3.1/coop_html_editor/static/aloha.0.23.26/plugins/extra/flag-icons/img/flags/um.png
--rw-r--r--   0 lucjean    (501) staff       (20)      522 2019-08-29 13:07:40.000000 coop_html_editor-1.3.1/coop_html_editor/static/aloha.0.23.26/plugins/extra/flag-icons/img/flags/tk.png
--rw-r--r--   0 lucjean    (501) staff       (20)      412 2019-08-29 13:07:40.000000 coop_html_editor-1.3.1/coop_html_editor/static/aloha.0.23.26/plugins/extra/flag-icons/img/flags/vc.png
--rw-r--r--   0 lucjean    (501) staff       (20)      153 2019-08-29 13:07:40.000000 coop_html_editor-1.3.1/coop_html_editor/static/aloha.0.23.26/plugins/extra/flag-icons/img/flags/xh.png
--rw-r--r--   0 lucjean    (501) staff       (20)      462 2019-08-29 13:07:40.000000 coop_html_editor-1.3.1/coop_html_editor/static/aloha.0.23.26/plugins/extra/flag-icons/img/flags/zw.png
--rw-r--r--   0 lucjean    (501) staff       (20)      391 2019-08-29 13:07:40.000000 coop_html_editor-1.3.1/coop_html_editor/static/aloha.0.23.26/plugins/extra/flag-icons/img/flags/nr.png
--rw-r--r--   0 lucjean    (501) staff       (20)      300 2019-08-29 13:07:39.000000 coop_html_editor-1.3.1/coop_html_editor/static/aloha.0.23.26/plugins/extra/flag-icons/img/flags/mi.png
--rw-r--r--   0 lucjean    (501) staff       (20)      393 2019-08-29 13:07:40.000000 coop_html_editor-1.3.1/coop_html_editor/static/aloha.0.23.26/plugins/extra/flag-icons/img/flags/ne.png
--rw-r--r--   0 lucjean    (501) staff       (20)      445 2019-08-29 13:07:39.000000 coop_html_editor-1.3.1/coop_html_editor/static/aloha.0.23.26/plugins/extra/flag-icons/img/flags/cu.png
--rw-r--r--   0 lucjean    (501) staff       (20)      341 2019-08-29 13:07:39.000000 coop_html_editor-1.3.1/coop_html_editor/static/aloha.0.23.26/plugins/extra/flag-icons/img/flags/bf.png
--rw-r--r--   0 lucjean    (501) staff       (20)      320 2019-08-29 13:07:39.000000 coop_html_editor-1.3.1/coop_html_editor/static/aloha.0.23.26/plugins/extra/flag-icons/img/flags/bg.png
--rw-r--r--   0 lucjean    (501) staff       (20)      496 2019-08-29 13:07:39.000000 coop_html_editor-1.3.1/coop_html_editor/static/aloha.0.23.26/plugins/extra/flag-icons/img/flags/cc.png
--rw-r--r--   0 lucjean    (501) staff       (20)      159 2019-08-29 13:07:39.000000 coop_html_editor-1.3.1/coop_html_editor/static/aloha.0.23.26/plugins/extra/flag-icons/img/flags/ak.png
--rw-r--r--   0 lucjean    (501) staff       (20)      523 2019-08-29 13:07:40.000000 coop_html_editor-1.3.1/coop_html_editor/static/aloha.0.23.26/plugins/extra/flag-icons/img/flags/nd.png
--rw-r--r--   0 lucjean    (501) staff       (20)      518 2019-08-29 13:07:39.000000 coop_html_editor-1.3.1/coop_html_editor/static/aloha.0.23.26/plugins/extra/flag-icons/img/flags/mh.png
--rw-r--r--   0 lucjean    (501) staff       (20)      523 2019-08-29 13:07:40.000000 coop_html_editor-1.3.1/coop_html_editor/static/aloha.0.23.26/plugins/extra/flag-icons/img/flags/za.png
--rw-r--r--   0 lucjean    (501) staff       (20)      353 2019-08-29 13:07:39.000000 coop_html_editor-1.3.1/coop_html_editor/static/aloha.0.23.26/plugins/extra/flag-icons/img/flags/catalonia.png
--rw-r--r--   0 lucjean    (501) staff       (20)      411 2019-08-29 13:07:40.000000 coop_html_editor-1.3.1/coop_html_editor/static/aloha.0.23.26/plugins/extra/flag-icons/img/flags/uy.png
--rw-r--r--   0 lucjean    (501) staff       (20)      438 2019-08-29 13:07:40.000000 coop_html_editor-1.3.1/coop_html_editor/static/aloha.0.23.26/plugins/extra/flag-icons/img/flags/wf.png
--rw-r--r--   0 lucjean    (501) staff       (20)      450 2019-08-29 13:07:40.000000 coop_html_editor-1.3.1/coop_html_editor/static/aloha.0.23.26/plugins/extra/flag-icons/img/flags/vu.png
--rw-r--r--   0 lucjean    (501) staff       (20)      367 2019-08-29 13:07:40.000000 coop_html_editor-1.3.1/coop_html_editor/static/aloha.0.23.26/plugins/extra/flag-icons/img/flags/tj.png
-drwxr-xr-x   0 lucjean    (501) staff       (20)        0 2019-08-30 10:39:54.000000 coop_html_editor-1.3.1/coop_html_editor/static/aloha.0.23.26/plugins/extra/toc/
-drwxr-xr-x   0 lucjean    (501) staff       (20)        0 2019-08-30 10:39:35.000000 coop_html_editor-1.3.1/coop_html_editor/static/aloha.0.23.26/plugins/extra/toc/nls/
-drwxr-xr-x   0 lucjean    (501) staff       (20)        0 2019-08-30 10:39:54.000000 coop_html_editor-1.3.1/coop_html_editor/static/aloha.0.23.26/plugins/extra/toc/nls/zh-hans/
--rw-r--r--   0 lucjean    (501) staff       (20)       54 2019-08-29 13:07:41.000000 coop_html_editor-1.3.1/coop_html_editor/static/aloha.0.23.26/plugins/extra/toc/nls/zh-hans/i18n.js
-drwxr-xr-x   0 lucjean    (501) staff       (20)        0 2019-08-30 10:39:54.000000 coop_html_editor-1.3.1/coop_html_editor/static/aloha.0.23.26/plugins/extra/toc/nls/ca/
--rw-r--r--   0 lucjean    (501) staff       (20)       61 2019-08-29 13:07:41.000000 coop_html_editor-1.3.1/coop_html_editor/static/aloha.0.23.26/plugins/extra/toc/nls/ca/i18n.js
-drwxr-xr-x   0 lucjean    (501) staff       (20)        0 2019-08-30 10:39:54.000000 coop_html_editor-1.3.1/coop_html_editor/static/aloha.0.23.26/plugins/extra/toc/nls/ru/
--rw-r--r--   0 lucjean    (501) staff       (20)       62 2019-08-29 13:07:41.000000 coop_html_editor-1.3.1/coop_html_editor/static/aloha.0.23.26/plugins/extra/toc/nls/ru/i18n.js
-drwxr-xr-x   0 lucjean    (501) staff       (20)        0 2019-08-30 10:39:54.000000 coop_html_editor-1.3.1/coop_html_editor/static/aloha.0.23.26/plugins/extra/toc/nls/uk/
--rw-r--r--   0 lucjean    (501) staff       (20)       52 2019-08-29 13:07:41.000000 coop_html_editor-1.3.1/coop_html_editor/static/aloha.0.23.26/plugins/extra/toc/nls/uk/i18n.js
-drwxr-xr-x   0 lucjean    (501) staff       (20)        0 2019-08-30 10:39:54.000000 coop_html_editor-1.3.1/coop_html_editor/static/aloha.0.23.26/plugins/extra/toc/nls/mk/
--rw-r--r--   0 lucjean    (501) staff       (20)       76 2019-08-29 13:07:41.000000 coop_html_editor-1.3.1/coop_html_editor/static/aloha.0.23.26/plugins/extra/toc/nls/mk/i18n.js
-drwxr-xr-x   0 lucjean    (501) staff       (20)        0 2019-08-30 10:39:54.000000 coop_html_editor-1.3.1/coop_html_editor/static/aloha.0.23.26/plugins/extra/toc/nls/pt-br/
--rw-r--r--   0 lucjean    (501) staff       (20)       61 2019-08-29 13:07:41.000000 coop_html_editor-1.3.1/coop_html_editor/static/aloha.0.23.26/plugins/extra/toc/nls/pt-br/i18n.js
-drwxr-xr-x   0 lucjean    (501) staff       (20)        0 2019-08-30 10:39:54.000000 coop_html_editor-1.3.1/coop_html_editor/static/aloha.0.23.26/plugins/extra/toc/nls/de/
--rw-r--r--   0 lucjean    (501) staff       (20)       60 2019-08-29 13:07:41.000000 coop_html_editor-1.3.1/coop_html_editor/static/aloha.0.23.26/plugins/extra/toc/nls/de/i18n.js
--rw-r--r--   0 lucjean    (501) staff       (20)        3 2019-08-29 13:07:41.000000 coop_html_editor-1.3.1/coop_html_editor/static/aloha.0.23.26/plugins/extra/toc/package.json
-drwxr-xr-x   0 lucjean    (501) staff       (20)        0 2019-08-30 10:39:35.000000 coop_html_editor-1.3.1/coop_html_editor/static/aloha.0.23.26/plugins/extra/sourceview/
-drwxr-xr-x   0 lucjean    (501) staff       (20)        0 2019-08-30 10:39:53.000000 coop_html_editor-1.3.1/coop_html_editor/static/aloha.0.23.26/plugins/extra/sourceview/css/
--rw-r--r--   0 lucjean    (501) staff       (20)      489 2019-08-29 13:07:41.000000 coop_html_editor-1.3.1/coop_html_editor/static/aloha.0.23.26/plugins/extra/sourceview/css/sourceview.css
-drwxr-xr-x   0 lucjean    (501) staff       (20)        0 2019-08-30 10:39:53.000000 coop_html_editor-1.3.1/coop_html_editor/static/aloha.0.23.26/plugins/extra/sourceview/lib/
--rw-r--r--   0 lucjean    (501) staff       (20)     7855 2019-08-29 13:07:41.000000 coop_html_editor-1.3.1/coop_html_editor/static/aloha.0.23.26/plugins/extra/sourceview/lib/sourceview-plugin.js
-drwxr-xr-x   0 lucjean    (501) staff       (20)        0 2019-08-30 10:39:53.000000 coop_html_editor-1.3.1/coop_html_editor/static/aloha.0.23.26/plugins/extra/sourceview/vendor/
--rw-r--r--   0 lucjean    (501) staff       (20)    16948 2019-08-29 13:07:41.000000 coop_html_editor-1.3.1/coop_html_editor/static/aloha.0.23.26/plugins/extra/sourceview/vendor/htmlbeautifier.js
-drwxr-xr-x   0 lucjean    (501) staff       (20)        0 2019-08-30 10:39:54.000000 coop_html_editor-1.3.1/coop_html_editor/static/aloha.0.23.26/plugins/extra/speak/
-drwxr-xr-x   0 lucjean    (501) staff       (20)        0 2019-08-30 10:39:54.000000 coop_html_editor-1.3.1/coop_html_editor/static/aloha.0.23.26/plugins/extra/speak/css/
--rw-r--r--   0 lucjean    (501) staff       (20)       80 2019-08-29 13:07:41.000000 coop_html_editor-1.3.1/coop_html_editor/static/aloha.0.23.26/plugins/extra/speak/css/speak.css
--rw-r--r--   0 lucjean    (501) staff       (20)        0 2019-08-29 13:07:41.000000 coop_html_editor-1.3.1/coop_html_editor/static/aloha.0.23.26/plugins/extra/speak/README
-drwxr-xr-x   0 lucjean    (501) staff       (20)        0 2019-08-30 10:39:54.000000 coop_html_editor-1.3.1/coop_html_editor/static/aloha.0.23.26/plugins/extra/speak/img/
--rw-r--r--   0 lucjean    (501) staff       (20)      760 2019-08-29 13:07:41.000000 coop_html_editor-1.3.1/coop_html_editor/static/aloha.0.23.26/plugins/extra/speak/img/speaker.png
--rw-r--r--   0 lucjean    (501) staff       (20)        3 2019-08-29 13:07:41.000000 coop_html_editor-1.3.1/coop_html_editor/static/aloha.0.23.26/plugins/extra/speak/package.json
-drwxr-xr-x   0 lucjean    (501) staff       (20)        0 2019-08-30 10:39:54.000000 coop_html_editor-1.3.1/coop_html_editor/static/aloha.0.23.26/plugins/extra/speak/lib/
--rw-r--r--   0 lucjean    (501) staff       (20)     2159 2019-08-29 13:07:41.000000 coop_html_editor-1.3.1/coop_html_editor/static/aloha.0.23.26/plugins/extra/speak/lib/speak-plugin.js
--rw-r--r--   0 lucjean    (501) staff       (20)  3435808 2019-08-29 13:07:41.000000 coop_html_editor-1.3.1/coop_html_editor/static/aloha.0.23.26/plugins/extra/speak/lib/speak.js
-drwxr-xr-x   0 lucjean    (501) staff       (20)        0 2019-08-30 10:39:48.000000 coop_html_editor-1.3.1/coop_html_editor/static/aloha.0.23.26/plugins/extra/formatlesspaste/
-drwxr-xr-x   0 lucjean    (501) staff       (20)        0 2019-08-30 10:39:48.000000 coop_html_editor-1.3.1/coop_html_editor/static/aloha.0.23.26/plugins/extra/formatlesspaste/css/
--rw-r--r--   0 lucjean    (501) staff       (20)      268 2019-08-29 13:07:40.000000 coop_html_editor-1.3.1/coop_html_editor/static/aloha.0.23.26/plugins/extra/formatlesspaste/css/formatless.css
-drwxr-xr-x   0 lucjean    (501) staff       (20)        0 2019-08-30 10:39:35.000000 coop_html_editor-1.3.1/coop_html_editor/static/aloha.0.23.26/plugins/extra/formatlesspaste/nls/
-drwxr-xr-x   0 lucjean    (501) staff       (20)        0 2019-08-30 10:39:48.000000 coop_html_editor-1.3.1/coop_html_editor/static/aloha.0.23.26/plugins/extra/formatlesspaste/nls/zh-hans/
--rw-r--r--   0 lucjean    (501) staff       (20)       72 2019-08-29 13:07:40.000000 coop_html_editor-1.3.1/coop_html_editor/static/aloha.0.23.26/plugins/extra/formatlesspaste/nls/zh-hans/i18n.js
-drwxr-xr-x   0 lucjean    (501) staff       (20)        0 2019-08-30 10:39:48.000000 coop_html_editor-1.3.1/coop_html_editor/static/aloha.0.23.26/plugins/extra/formatlesspaste/nls/ca/
--rw-r--r--   0 lucjean    (501) staff       (20)       97 2019-08-29 13:07:40.000000 coop_html_editor-1.3.1/coop_html_editor/static/aloha.0.23.26/plugins/extra/formatlesspaste/nls/ca/i18n.js
-drwxr-xr-x   0 lucjean    (501) staff       (20)        0 2019-08-30 10:39:48.000000 coop_html_editor-1.3.1/coop_html_editor/static/aloha.0.23.26/plugins/extra/formatlesspaste/nls/ru/
--rw-r--r--   0 lucjean    (501) staff       (20)      128 2019-08-29 13:07:40.000000 coop_html_editor-1.3.1/coop_html_editor/static/aloha.0.23.26/plugins/extra/formatlesspaste/nls/ru/i18n.js
-drwxr-xr-x   0 lucjean    (501) staff       (20)        0 2019-08-30 10:39:48.000000 coop_html_editor-1.3.1/coop_html_editor/static/aloha.0.23.26/plugins/extra/formatlesspaste/nls/uk/
--rw-r--r--   0 lucjean    (501) staff       (20)      116 2019-08-29 13:07:40.000000 coop_html_editor-1.3.1/coop_html_editor/static/aloha.0.23.26/plugins/extra/formatlesspaste/nls/uk/i18n.js
-drwxr-xr-x   0 lucjean    (501) staff       (20)        0 2019-08-30 10:39:48.000000 coop_html_editor-1.3.1/coop_html_editor/static/aloha.0.23.26/plugins/extra/formatlesspaste/nls/mk/
--rw-r--r--   0 lucjean    (501) staff       (20)      107 2019-08-29 13:07:40.000000 coop_html_editor-1.3.1/coop_html_editor/static/aloha.0.23.26/plugins/extra/formatlesspaste/nls/mk/i18n.js
-drwxr-xr-x   0 lucjean    (501) staff       (20)        0 2019-08-30 10:39:48.000000 coop_html_editor-1.3.1/coop_html_editor/static/aloha.0.23.26/plugins/extra/formatlesspaste/nls/pt-br/
--rw-r--r--   0 lucjean    (501) staff       (20)       82 2019-08-29 13:07:40.000000 coop_html_editor-1.3.1/coop_html_editor/static/aloha.0.23.26/plugins/extra/formatlesspaste/nls/pt-br/i18n.js
-drwxr-xr-x   0 lucjean    (501) staff       (20)        0 2019-08-30 10:39:48.000000 coop_html_editor-1.3.1/coop_html_editor/static/aloha.0.23.26/plugins/extra/formatlesspaste/nls/de/
--rw-r--r--   0 lucjean    (501) staff       (20)       87 2019-08-29 13:07:40.000000 coop_html_editor-1.3.1/coop_html_editor/static/aloha.0.23.26/plugins/extra/formatlesspaste/nls/de/i18n.js
--rw-r--r--   0 lucjean    (501) staff       (20)       93 2019-08-29 13:07:40.000000 coop_html_editor-1.3.1/coop_html_editor/static/aloha.0.23.26/plugins/extra/formatlesspaste/README.md
-drwxr-xr-x   0 lucjean    (501) staff       (20)        0 2019-08-30 10:39:48.000000 coop_html_editor-1.3.1/coop_html_editor/static/aloha.0.23.26/plugins/extra/formatlesspaste/img/
--rw-r--r--   0 lucjean    (501) staff       (20)      266 2019-08-29 13:07:40.000000 coop_html_editor-1.3.1/coop_html_editor/static/aloha.0.23.26/plugins/extra/formatlesspaste/img/button.png
--rw-r--r--   0 lucjean    (501) staff       (20)      125 2019-08-29 13:07:40.000000 coop_html_editor-1.3.1/coop_html_editor/static/aloha.0.23.26/plugins/extra/formatlesspaste/package.json
-drwxr-xr-x   0 lucjean    (501) staff       (20)        0 2019-08-30 10:39:35.000000 coop_html_editor-1.3.1/coop_html_editor/static/aloha.0.23.26/plugins/extra/proxy/
-drwxr-xr-x   0 lucjean    (501) staff       (20)        0 2019-08-30 10:39:53.000000 coop_html_editor-1.3.1/coop_html_editor/static/aloha.0.23.26/plugins/extra/proxy/adapter/
--rw-r--r--   0 lucjean    (501) staff       (20)     7323 2019-08-29 13:07:41.000000 coop_html_editor-1.3.1/coop_html_editor/static/aloha.0.23.26/plugins/extra/proxy/adapter/proxy.php
-drwxr-xr-x   0 lucjean    (501) staff       (20)        0 2019-08-30 10:39:53.000000 coop_html_editor-1.3.1/coop_html_editor/static/aloha.0.23.26/plugins/extra/proxy/lib/
--rw-r--r--   0 lucjean    (501) staff       (20)      981 2019-08-29 13:07:41.000000 coop_html_editor-1.3.1/coop_html_editor/static/aloha.0.23.26/plugins/extra/proxy/lib/proxy-plugin.js
-drwxr-xr-x   0 lucjean    (501) staff       (20)        0 2019-08-30 10:39:43.000000 coop_html_editor-1.3.1/coop_html_editor/static/aloha.0.23.26/plugins/extra/cite/
-drwxr-xr-x   0 lucjean    (501) staff       (20)        0 2019-08-30 10:39:43.000000 coop_html_editor-1.3.1/coop_html_editor/static/aloha.0.23.26/plugins/extra/cite/css/
--rw-r--r--   0 lucjean    (501) staff       (20)      879 2019-08-29 13:07:39.000000 coop_html_editor-1.3.1/coop_html_editor/static/aloha.0.23.26/plugins/extra/cite/css/cite.css
-drwxr-xr-x   0 lucjean    (501) staff       (20)        0 2019-08-30 10:39:35.000000 coop_html_editor-1.3.1/coop_html_editor/static/aloha.0.23.26/plugins/extra/cite/nls/
-drwxr-xr-x   0 lucjean    (501) staff       (20)        0 2019-08-30 10:39:43.000000 coop_html_editor-1.3.1/coop_html_editor/static/aloha.0.23.26/plugins/extra/cite/nls/zh-hans/
--rw-r--r--   0 lucjean    (501) staff       (20)      131 2019-08-29 13:07:39.000000 coop_html_editor-1.3.1/coop_html_editor/static/aloha.0.23.26/plugins/extra/cite/nls/zh-hans/i18n.js
-drwxr-xr-x   0 lucjean    (501) staff       (20)        0 2019-08-30 10:39:43.000000 coop_html_editor-1.3.1/coop_html_editor/static/aloha.0.23.26/plugins/extra/cite/nls/ca/
--rw-r--r--   0 lucjean    (501) staff       (20)      150 2019-08-29 13:07:39.000000 coop_html_editor-1.3.1/coop_html_editor/static/aloha.0.23.26/plugins/extra/cite/nls/ca/i18n.js
-drwxr-xr-x   0 lucjean    (501) staff       (20)        0 2019-08-30 10:39:43.000000 coop_html_editor-1.3.1/coop_html_editor/static/aloha.0.23.26/plugins/extra/cite/nls/ru/
--rw-r--r--   0 lucjean    (501) staff       (20)      216 2019-08-29 13:07:39.000000 coop_html_editor-1.3.1/coop_html_editor/static/aloha.0.23.26/plugins/extra/cite/nls/ru/i18n.js
-drwxr-xr-x   0 lucjean    (501) staff       (20)        0 2019-08-30 10:39:43.000000 coop_html_editor-1.3.1/coop_html_editor/static/aloha.0.23.26/plugins/extra/cite/nls/uk/
--rw-r--r--   0 lucjean    (501) staff       (20)      200 2019-08-29 13:07:39.000000 coop_html_editor-1.3.1/coop_html_editor/static/aloha.0.23.26/plugins/extra/cite/nls/uk/i18n.js
-drwxr-xr-x   0 lucjean    (501) staff       (20)        0 2019-08-30 10:39:43.000000 coop_html_editor-1.3.1/coop_html_editor/static/aloha.0.23.26/plugins/extra/cite/nls/mk/
--rw-r--r--   0 lucjean    (501) staff       (20)      231 2019-08-29 13:07:39.000000 coop_html_editor-1.3.1/coop_html_editor/static/aloha.0.23.26/plugins/extra/cite/nls/mk/i18n.js
-drwxr-xr-x   0 lucjean    (501) staff       (20)        0 2019-08-30 10:39:43.000000 coop_html_editor-1.3.1/coop_html_editor/static/aloha.0.23.26/plugins/extra/cite/nls/pt-br/
--rw-r--r--   0 lucjean    (501) staff       (20)      152 2019-08-29 13:07:39.000000 coop_html_editor-1.3.1/coop_html_editor/static/aloha.0.23.26/plugins/extra/cite/nls/pt-br/i18n.js
-drwxr-xr-x   0 lucjean    (501) staff       (20)        0 2019-08-30 10:39:43.000000 coop_html_editor-1.3.1/coop_html_editor/static/aloha.0.23.26/plugins/extra/cite/nls/de/
--rw-r--r--   0 lucjean    (501) staff       (20)      135 2019-08-29 13:07:39.000000 coop_html_editor-1.3.1/coop_html_editor/static/aloha.0.23.26/plugins/extra/cite/nls/de/i18n.js
--rw-r--r--   0 lucjean    (501) staff       (20)        0 2019-08-29 13:07:39.000000 coop_html_editor-1.3.1/coop_html_editor/static/aloha.0.23.26/plugins/extra/cite/README
-drwxr-xr-x   0 lucjean    (501) staff       (20)        0 2019-08-30 10:39:43.000000 coop_html_editor-1.3.1/coop_html_editor/static/aloha.0.23.26/plugins/extra/cite/img/
--rw-r--r--   0 lucjean    (501) staff       (20)      698 2019-08-29 13:07:39.000000 coop_html_editor-1.3.1/coop_html_editor/static/aloha.0.23.26/plugins/extra/cite/img/blockquote.png
--rw-r--r--   0 lucjean    (501) staff       (20)      241 2019-08-29 13:07:39.000000 coop_html_editor-1.3.1/coop_html_editor/static/aloha.0.23.26/plugins/extra/cite/img/icon_cite.png
--rw-r--r--   0 lucjean    (501) staff       (20)        3 2019-08-29 13:07:39.000000 coop_html_editor-1.3.1/coop_html_editor/static/aloha.0.23.26/plugins/extra/cite/package.json
-drwxr-xr-x   0 lucjean    (501) staff       (20)        0 2019-08-30 10:39:35.000000 coop_html_editor-1.3.1/coop_html_editor/static/aloha.0.23.26/plugins/extra/textcolor/
-drwxr-xr-x   0 lucjean    (501) staff       (20)        0 2019-08-30 10:39:54.000000 coop_html_editor-1.3.1/coop_html_editor/static/aloha.0.23.26/plugins/extra/textcolor/css/
--rw-r--r--   0 lucjean    (501) staff       (20)     1338 2019-08-29 13:07:41.000000 coop_html_editor-1.3.1/coop_html_editor/static/aloha.0.23.26/plugins/extra/textcolor/css/textcolor.css
-drwxr-xr-x   0 lucjean    (501) staff       (20)        0 2019-08-30 10:39:54.000000 coop_html_editor-1.3.1/coop_html_editor/static/aloha.0.23.26/plugins/extra/textcolor/nls/
-drwxr-xr-x   0 lucjean    (501) staff       (20)        0 2019-08-30 10:39:54.000000 coop_html_editor-1.3.1/coop_html_editor/static/aloha.0.23.26/plugins/extra/textcolor/nls/de/
--rw-r--r--   0 lucjean    (501) staff       (20)       62 2019-08-29 13:07:41.000000 coop_html_editor-1.3.1/coop_html_editor/static/aloha.0.23.26/plugins/extra/textcolor/nls/de/i18n.js
--rw-r--r--   0 lucjean    (501) staff       (20)       91 2019-08-29 13:07:41.000000 coop_html_editor-1.3.1/coop_html_editor/static/aloha.0.23.26/plugins/extra/textcolor/nls/i18n.js
-drwxr-xr-x   0 lucjean    (501) staff       (20)        0 2019-08-30 10:39:54.000000 coop_html_editor-1.3.1/coop_html_editor/static/aloha.0.23.26/plugins/extra/textcolor/img/
--rw-r--r--   0 lucjean    (501) staff       (20)     2968 2019-08-29 13:07:41.000000 coop_html_editor-1.3.1/coop_html_editor/static/aloha.0.23.26/plugins/extra/textcolor/img/icon.png
-drwxr-xr-x   0 lucjean    (501) staff       (20)        0 2019-08-30 10:39:54.000000 coop_html_editor-1.3.1/coop_html_editor/static/aloha.0.23.26/plugins/extra/textcolor/lib/
--rw-r--r--   0 lucjean    (501) staff       (20)    12591 2019-08-29 13:07:41.000000 coop_html_editor-1.3.1/coop_html_editor/static/aloha.0.23.26/plugins/extra/textcolor/lib/textcolor-plugin.js
-drwxr-xr-x   0 lucjean    (501) staff       (20)        0 2019-08-30 10:39:52.000000 coop_html_editor-1.3.1/coop_html_editor/static/aloha.0.23.26/plugins/extra/linkchecker/
-drwxr-xr-x   0 lucjean    (501) staff       (20)        0 2019-08-30 10:39:52.000000 coop_html_editor-1.3.1/coop_html_editor/static/aloha.0.23.26/plugins/extra/linkchecker/demo/
--rw-r--r--   0 lucjean    (501) staff       (20)     4116 2019-08-29 13:07:41.000000 coop_html_editor-1.3.1/coop_html_editor/static/aloha.0.23.26/plugins/extra/linkchecker/demo/index.html
--rw-r--r--   0 lucjean    (501) staff       (20)      787 2019-08-29 13:07:41.000000 coop_html_editor-1.3.1/coop_html_editor/static/aloha.0.23.26/plugins/extra/linkchecker/demo/index.css
-drwxr-xr-x   0 lucjean    (501) staff       (20)        0 2019-08-30 10:39:52.000000 coop_html_editor-1.3.1/coop_html_editor/static/aloha.0.23.26/plugins/extra/linkchecker/nls/
-drwxr-xr-x   0 lucjean    (501) staff       (20)        0 2019-08-30 10:39:52.000000 coop_html_editor-1.3.1/coop_html_editor/static/aloha.0.23.26/plugins/extra/linkchecker/nls/zh-hans/
--rw-r--r--   0 lucjean    (501) staff       (20)     2235 2019-08-29 13:07:41.000000 coop_html_editor-1.3.1/coop_html_editor/static/aloha.0.23.26/plugins/extra/linkchecker/nls/zh-hans/i18n.js
-drwxr-xr-x   0 lucjean    (501) staff       (20)        0 2019-08-30 10:39:52.000000 coop_html_editor-1.3.1/coop_html_editor/static/aloha.0.23.26/plugins/extra/linkchecker/nls/ca/
--rw-r--r--   0 lucjean    (501) staff       (20)     2807 2019-08-29 13:07:41.000000 coop_html_editor-1.3.1/coop_html_editor/static/aloha.0.23.26/plugins/extra/linkchecker/nls/ca/i18n.js
-drwxr-xr-x   0 lucjean    (501) staff       (20)        0 2019-08-30 10:39:52.000000 coop_html_editor-1.3.1/coop_html_editor/static/aloha.0.23.26/plugins/extra/linkchecker/nls/ru/
--rw-r--r--   0 lucjean    (501) staff       (20)     3828 2019-08-29 13:07:41.000000 coop_html_editor-1.3.1/coop_html_editor/static/aloha.0.23.26/plugins/extra/linkchecker/nls/ru/i18n.js
-drwxr-xr-x   0 lucjean    (501) staff       (20)        0 2019-08-30 10:39:52.000000 coop_html_editor-1.3.1/coop_html_editor/static/aloha.0.23.26/plugins/extra/linkchecker/nls/uk/
--rw-r--r--   0 lucjean    (501) staff       (20)     3841 2019-08-29 13:07:41.000000 coop_html_editor-1.3.1/coop_html_editor/static/aloha.0.23.26/plugins/extra/linkchecker/nls/uk/i18n.js
-drwxr-xr-x   0 lucjean    (501) staff       (20)        0 2019-08-30 10:39:52.000000 coop_html_editor-1.3.1/coop_html_editor/static/aloha.0.23.26/plugins/extra/linkchecker/nls/mk/
--rw-r--r--   0 lucjean    (501) staff       (20)     3870 2019-08-29 13:07:41.000000 coop_html_editor-1.3.1/coop_html_editor/static/aloha.0.23.26/plugins/extra/linkchecker/nls/mk/i18n.js
-drwxr-xr-x   0 lucjean    (501) staff       (20)        0 2019-08-30 10:39:52.000000 coop_html_editor-1.3.1/coop_html_editor/static/aloha.0.23.26/plugins/extra/linkchecker/nls/pt-br/
--rw-r--r--   0 lucjean    (501) staff       (20)     2490 2019-08-29 13:07:41.000000 coop_html_editor-1.3.1/coop_html_editor/static/aloha.0.23.26/plugins/extra/linkchecker/nls/pt-br/i18n.js
-drwxr-xr-x   0 lucjean    (501) staff       (20)        0 2019-08-30 10:39:52.000000 coop_html_editor-1.3.1/coop_html_editor/static/aloha.0.23.26/plugins/extra/linkchecker/nls/de/
--rw-r--r--   0 lucjean    (501) staff       (20)     3384 2019-08-29 13:07:41.000000 coop_html_editor-1.3.1/coop_html_editor/static/aloha.0.23.26/plugins/extra/linkchecker/nls/de/i18n.js
--rw-r--r--   0 lucjean    (501) staff       (20)     2515 2019-08-29 13:07:41.000000 coop_html_editor-1.3.1/coop_html_editor/static/aloha.0.23.26/plugins/extra/linkchecker/nls/i18n.js
--rw-r--r--   0 lucjean    (501) staff       (20)     7226 2019-08-29 13:07:41.000000 coop_html_editor-1.3.1/coop_html_editor/static/aloha.0.23.26/plugins/extra/linkchecker/proxy.php.example
--rw-r--r--   0 lucjean    (501) staff       (20)        3 2019-08-29 13:07:41.000000 coop_html_editor-1.3.1/coop_html_editor/static/aloha.0.23.26/plugins/extra/linkchecker/package.json
-drwxr-xr-x   0 lucjean    (501) staff       (20)        0 2019-08-30 10:39:52.000000 coop_html_editor-1.3.1/coop_html_editor/static/aloha.0.23.26/plugins/extra/linkchecker/src/
--rw-r--r--   0 lucjean    (501) staff       (20)     8258 2019-08-29 13:07:41.000000 coop_html_editor-1.3.1/coop_html_editor/static/aloha.0.23.26/plugins/extra/linkchecker/src/linkchecker.js
--rw-r--r--   0 lucjean    (501) staff       (20)      264 2019-08-29 13:07:41.000000 coop_html_editor-1.3.1/coop_html_editor/static/aloha.0.23.26/plugins/extra/linkchecker/src/linkchecker.css
-drwxr-xr-x   0 lucjean    (501) staff       (20)        0 2019-08-30 10:39:48.000000 coop_html_editor-1.3.1/coop_html_editor/static/aloha.0.23.26/plugins/extra/googletranslate/
-drwxr-xr-x   0 lucjean    (501) staff       (20)        0 2019-08-30 10:39:48.000000 coop_html_editor-1.3.1/coop_html_editor/static/aloha.0.23.26/plugins/extra/googletranslate/css/
--rw-r--r--   0 lucjean    (501) staff       (20)      417 2019-08-29 13:07:40.000000 coop_html_editor-1.3.1/coop_html_editor/static/aloha.0.23.26/plugins/extra/googletranslate/css/googletranslate.css
--rw-r--r--   0 lucjean    (501) staff       (20)     1019 2019-08-29 13:07:40.000000 coop_html_editor-1.3.1/coop_html_editor/static/aloha.0.23.26/plugins/extra/googletranslate/README.md
-drwxr-xr-x   0 lucjean    (501) staff       (20)        0 2019-08-30 10:39:49.000000 coop_html_editor-1.3.1/coop_html_editor/static/aloha.0.23.26/plugins/extra/googletranslate/img/
--rw-r--r--   0 lucjean    (501) staff       (20)      410 2019-08-29 13:07:40.000000 coop_html_editor-1.3.1/coop_html_editor/static/aloha.0.23.26/plugins/extra/googletranslate/img/tg.png
--rw-r--r--   0 lucjean    (501) staff       (20)      394 2019-08-29 13:07:40.000000 coop_html_editor-1.3.1/coop_html_editor/static/aloha.0.23.26/plugins/extra/googletranslate/img/me.png
--rw-r--r--   0 lucjean    (501) staff       (20)      415 2019-08-29 13:07:40.000000 coop_html_editor-1.3.1/coop_html_editor/static/aloha.0.23.26/plugins/extra/googletranslate/img/la.png
--rw-r--r--   0 lucjean    (501) staff       (20)      408 2019-08-29 13:07:40.000000 coop_html_editor-1.3.1/coop_html_editor/static/aloha.0.23.26/plugins/extra/googletranslate/img/mr.png
--rw-r--r--   0 lucjean    (501) staff       (20)      372 2019-08-29 13:07:40.000000 coop_html_editor-1.3.1/coop_html_editor/static/aloha.0.23.26/plugins/extra/googletranslate/img/ni.png
--rw-r--r--   0 lucjean    (501) staff       (20)      339 2019-08-29 13:07:40.000000 coop_html_editor-1.3.1/coop_html_editor/static/aloha.0.23.26/plugins/extra/googletranslate/img/lv.png
--rw-r--r--   0 lucjean    (501) staff       (20)      339 2019-08-29 13:07:40.000000 coop_html_editor-1.3.1/coop_html_editor/static/aloha.0.23.26/plugins/extra/googletranslate/img/om.png
--rw-r--r--   0 lucjean    (501) staff       (20)      420 2019-08-29 13:07:40.000000 coop_html_editor-1.3.1/coop_html_editor/static/aloha.0.23.26/plugins/extra/googletranslate/img/af.png
--rw-r--r--   0 lucjean    (501) staff       (20)      337 2019-08-29 13:07:40.000000 coop_html_editor-1.3.1/coop_html_editor/static/aloha.0.23.26/plugins/extra/googletranslate/img/cy.png
--rw-r--r--   0 lucjean    (501) staff       (20)      311 2019-08-29 13:07:40.000000 coop_html_editor-1.3.1/coop_html_editor/static/aloha.0.23.26/plugins/extra/googletranslate/img/bj.png
--rw-r--r--   0 lucjean    (501) staff       (20)      349 2019-08-29 13:07:40.000000 coop_html_editor-1.3.1/coop_html_editor/static/aloha.0.23.26/plugins/extra/googletranslate/img/cn.png
--rw-r--r--   0 lucjean    (501) staff       (20)      330 2019-08-29 13:07:40.000000 coop_html_editor-1.3.1/coop_html_editor/static/aloha.0.23.26/plugins/extra/googletranslate/img/co.png
--rw-r--r--   0 lucjean    (501) staff       (20)      498 2019-08-29 13:07:40.000000 coop_html_editor-1.3.1/coop_html_editor/static/aloha.0.23.26/plugins/extra/googletranslate/img/cx.png
--rw-r--r--   0 lucjean    (501) staff       (20)      456 2019-08-29 13:07:40.000000 coop_html_editor-1.3.1/coop_html_editor/static/aloha.0.23.26/plugins/extra/googletranslate/img/ag.png
--rw-r--r--   0 lucjean    (501) staff       (20)      497 2019-08-29 13:07:40.000000 coop_html_editor-1.3.1/coop_html_editor/static/aloha.0.23.26/plugins/extra/googletranslate/img/ms.png
--rw-r--r--   0 lucjean    (501) staff       (20)      404 2019-08-29 13:07:40.000000 coop_html_editor-1.3.1/coop_html_editor/static/aloha.0.23.26/plugins/extra/googletranslate/img/md.png
--rw-r--r--   0 lucjean    (501) staff       (20)      359 2019-08-29 13:07:40.000000 coop_html_editor-1.3.1/coop_html_editor/static/aloha.0.23.26/plugins/extra/googletranslate/img/zm.png
--rw-r--r--   0 lucjean    (501) staff       (20)      324 2019-08-29 13:07:40.000000 coop_html_editor-1.3.1/coop_html_editor/static/aloha.0.23.26/plugins/extra/googletranslate/img/vn.png
--rw-r--r--   0 lucjean    (501) staff       (20)      399 2019-08-29 13:07:40.000000 coop_html_editor-1.3.1/coop_html_editor/static/aloha.0.23.26/plugins/extra/googletranslate/img/tf.png
--rw-r--r--   0 lucjean    (501) staff       (20)      378 2019-08-29 13:07:40.000000 coop_html_editor-1.3.1/coop_html_editor/static/aloha.0.23.26/plugins/extra/googletranslate/img/td.png
--rw-r--r--   0 lucjean    (501) staff       (20)      456 2019-08-29 13:07:40.000000 coop_html_editor-1.3.1/coop_html_editor/static/aloha.0.23.26/plugins/extra/googletranslate/img/yt.png
--rw-r--r--   0 lucjean    (501) staff       (20)      393 2019-08-29 13:07:40.000000 coop_html_editor-1.3.1/coop_html_editor/static/aloha.0.23.26/plugins/extra/googletranslate/img/lb.png
--rw-r--r--   0 lucjean    (501) staff       (20)      338 2019-08-29 13:07:40.000000 coop_html_editor-1.3.1/coop_html_editor/static/aloha.0.23.26/plugins/extra/googletranslate/img/lu.png
--rw-r--r--   0 lucjean    (501) staff       (20)      541 2019-08-29 13:07:40.000000 coop_html_editor-1.3.1/coop_html_editor/static/aloha.0.23.26/plugins/extra/googletranslate/img/mq.png
--rw-r--r--   0 lucjean    (501) staff       (20)      367 2019-08-29 13:07:40.000000 coop_html_editor-1.3.1/coop_html_editor/static/aloha.0.23.26/plugins/extra/googletranslate/img/cz.png
--rw-r--r--   0 lucjean    (501) staff       (20)      277 2019-08-29 13:07:40.000000 coop_html_editor-1.3.1/coop_html_editor/static/aloha.0.23.26/plugins/extra/googletranslate/img/ae.png
--rw-r--r--   0 lucjean    (501) staff       (20)      347 2019-08-29 13:07:40.000000 coop_html_editor-1.3.1/coop_html_editor/static/aloha.0.23.26/plugins/extra/googletranslate/img/cm.png
--rw-r--r--   0 lucjean    (501) staff       (20)      350 2019-08-29 13:07:40.000000 coop_html_editor-1.3.1/coop_html_editor/static/aloha.0.23.26/plugins/extra/googletranslate/img/fam.png
--rw-r--r--   0 lucjean    (501) staff       (20)      566 2019-08-29 13:07:40.000000 coop_html_editor-1.3.1/coop_html_editor/static/aloha.0.23.26/plugins/extra/googletranslate/img/bi.png
--rw-r--r--   0 lucjean    (501) staff       (20)      367 2019-08-29 13:07:40.000000 coop_html_editor-1.3.1/coop_html_editor/static/aloha.0.23.26/plugins/extra/googletranslate/img/ar.png
--rw-r--r--   0 lucjean    (501) staff       (20)      540 2019-08-29 13:07:40.000000 coop_html_editor-1.3.1/coop_html_editor/static/aloha.0.23.26/plugins/extra/googletranslate/img/as.png
--rw-r--r--   0 lucjean    (501) staff       (20)      345 2019-08-29 13:07:40.000000 coop_html_editor-1.3.1/coop_html_editor/static/aloha.0.23.26/plugins/extra/googletranslate/img/bh.png
--rw-r--r--   0 lucjean    (501) staff       (20)      324 2019-08-29 13:07:40.000000 coop_html_editor-1.3.1/coop_html_editor/static/aloha.0.23.26/plugins/extra/googletranslate/img/cl.png
--rw-r--r--   0 lucjean    (501) staff       (20)      454 2019-08-29 13:07:40.000000 coop_html_editor-1.3.1/coop_html_editor/static/aloha.0.23.26/plugins/extra/googletranslate/img/ad.png
--rw-r--r--   0 lucjean    (501) staff       (20)      481 2019-08-29 13:07:40.000000 coop_html_editor-1.3.1/coop_html_editor/static/aloha.0.23.26/plugins/extra/googletranslate/img/mp.png
--rw-r--r--   0 lucjean    (501) staff       (20)      345 2019-08-29 13:07:40.000000 coop_html_editor-1.3.1/coop_html_editor/static/aloha.0.23.26/plugins/extra/googletranslate/img/lt.png
--rw-r--r--   0 lucjean    (501) staff       (20)      313 2019-08-29 13:07:40.000000 coop_html_editor-1.3.1/coop_html_editor/static/aloha.0.23.26/plugins/extra/googletranslate/img/mg.png
--rw-r--r--   0 lucjean    (501) staff       (20)      462 2019-08-29 13:07:40.000000 coop_html_editor-1.3.1/coop_html_editor/static/aloha.0.23.26/plugins/extra/googletranslate/img/lc.png
--rw-r--r--   0 lucjean    (501) staff       (20)      366 2019-08-29 13:07:40.000000 coop_html_editor-1.3.1/coop_html_editor/static/aloha.0.23.26/plugins/extra/googletranslate/img/tr.png
--rw-r--r--   0 lucjean    (501) staff       (20)      304 2019-08-29 13:07:40.000000 coop_html_editor-1.3.1/coop_html_editor/static/aloha.0.23.26/plugins/extra/googletranslate/img/ua.png
--rw-r--r--   0 lucjean    (501) staff       (20)      554 2019-08-29 13:07:40.000000 coop_html_editor-1.3.1/coop_html_editor/static/aloha.0.23.26/plugins/extra/googletranslate/img/scotland.png
--rw-r--r--   0 lucjean    (501) staff       (20)      443 2019-08-29 13:07:40.000000 coop_html_editor-1.3.1/coop_html_editor/static/aloha.0.23.26/plugins/extra/googletranslate/img/tv.png
--rw-r--r--   0 lucjean    (501) staff       (20)      523 2019-08-29 13:07:40.000000 coop_html_editor-1.3.1/coop_html_editor/static/aloha.0.23.26/plugins/extra/googletranslate/img/vi.png
--rw-r--r--   0 lucjean    (501) staff       (20)      296 2019-08-29 13:07:40.000000 coop_html_editor-1.3.1/coop_html_editor/static/aloha.0.23.26/plugins/extra/googletranslate/img/mt.png
--rw-r--r--   0 lucjean    (501) staff       (20)      397 2019-08-29 13:07:40.000000 coop_html_editor-1.3.1/coop_html_editor/static/aloha.0.23.26/plugins/extra/googletranslate/img/no.png
--rw-r--r--   0 lucjean    (501) staff       (20)      254 2019-08-29 13:07:40.000000 coop_html_editor-1.3.1/coop_html_editor/static/aloha.0.23.26/plugins/extra/googletranslate/img/mc.png
--rw-r--r--   0 lucjean    (501) staff       (20)      239 2019-08-29 13:07:40.000000 coop_html_editor-1.3.1/coop_html_editor/static/aloha.0.23.26/plugins/extra/googletranslate/img/ch.png
--rw-r--r--   0 lucjean    (501) staff       (20)      393 2019-08-29 13:07:40.000000 coop_html_editor-1.3.1/coop_html_editor/static/aloha.0.23.26/plugins/extra/googletranslate/img/aw.png
--rw-r--r--   0 lucjean    (501) staff       (20)      476 2019-08-29 13:07:40.000000 coop_html_editor-1.3.1/coop_html_editor/static/aloha.0.23.26/plugins/extra/googletranslate/img/bz.png
--rw-r--r--   0 lucjean    (501) staff       (20)      499 2019-08-29 13:07:40.000000 coop_html_editor-1.3.1/coop_html_editor/static/aloha.0.23.26/plugins/extra/googletranslate/img/bm.png
--rw-r--r--   0 lucjean    (501) staff       (20)      306 2019-08-29 13:07:40.000000 coop_html_editor-1.3.1/coop_html_editor/static/aloha.0.23.26/plugins/extra/googletranslate/img/ci.png
--rw-r--r--   0 lucjean    (501) staff       (20)      360 2019-08-29 13:07:40.000000 coop_html_editor-1.3.1/coop_html_editor/static/aloha.0.23.26/plugins/extra/googletranslate/img/mu.png
--rw-r--r--   0 lucjean    (501) staff       (20)      492 2019-08-29 13:07:40.000000 coop_html_editor-1.3.1/coop_html_editor/static/aloha.0.23.26/plugins/extra/googletranslate/img/us.png
--rw-r--r--   0 lucjean    (501) staff       (20)      330 2019-08-29 13:07:40.000000 coop_html_editor-1.3.1/coop_html_editor/static/aloha.0.23.26/plugins/extra/googletranslate/img/tw.png
--rw-r--r--   0 lucjean    (501) staff       (20)      302 2019-08-29 13:07:40.000000 coop_html_editor-1.3.1/coop_html_editor/static/aloha.0.23.26/plugins/extra/googletranslate/img/ye.png
--rw-r--r--   0 lucjean    (501) staff       (20)      365 2019-08-29 13:07:40.000000 coop_html_editor-1.3.1/coop_html_editor/static/aloha.0.23.26/plugins/extra/googletranslate/img/mw.png
--rw-r--r--   0 lucjean    (501) staff       (20)      310 2019-08-29 13:07:40.000000 coop_html_editor-1.3.1/coop_html_editor/static/aloha.0.23.26/plugins/extra/googletranslate/img/nl.png
--rw-r--r--   0 lucjean    (501) staff       (20)      500 2019-08-29 13:07:40.000000 coop_html_editor-1.3.1/coop_html_editor/static/aloha.0.23.26/plugins/extra/googletranslate/img/ls.png
--rw-r--r--   0 lucjean    (501) staff       (20)      341 2019-08-29 13:07:40.000000 coop_html_editor-1.3.1/coop_html_editor/static/aloha.0.23.26/plugins/extra/googletranslate/img/bo.png
--rw-r--r--   0 lucjean    (501) staff       (20)      290 2019-08-29 13:07:40.000000 coop_html_editor-1.3.1/coop_html_editor/static/aloha.0.23.26/plugins/extra/googletranslate/img/at.png
--rw-r--r--   0 lucjean    (501) staff       (20)      495 2019-08-29 13:07:40.000000 coop_html_editor-1.3.1/coop_html_editor/static/aloha.0.23.26/plugins/extra/googletranslate/img/ck.png
--rw-r--r--   0 lucjean    (501) staff       (20)      382 2019-08-29 13:07:40.000000 coop_html_editor-1.3.1/coop_html_editor/static/aloha.0.23.26/plugins/extra/googletranslate/img/by.png
--rw-r--r--   0 lucjean    (501) staff       (20)      580 2019-08-29 13:07:40.000000 coop_html_editor-1.3.1/coop_html_editor/static/aloha.0.23.26/plugins/extra/googletranslate/img/au.png
--rw-r--r--   0 lucjean    (501) staff       (20)      502 2019-08-29 13:07:40.000000 coop_html_editor-1.3.1/coop_html_editor/static/aloha.0.23.26/plugins/extra/googletranslate/img/bn.png
--rw-r--r--   0 lucjean    (501) staff       (20)      293 2019-08-29 13:07:40.000000 coop_html_editor-1.3.1/coop_html_editor/static/aloha.0.23.26/plugins/extra/googletranslate/img/ma.png
--rw-r--r--   0 lucjean    (501) staff       (20)      529 2019-08-29 13:07:40.000000 coop_html_editor-1.3.1/coop_html_editor/static/aloha.0.23.26/plugins/extra/googletranslate/img/nz.png
--rw-r--r--   0 lucjean    (501) staff       (20)      365 2019-08-29 13:07:40.000000 coop_html_editor-1.3.1/coop_html_editor/static/aloha.0.23.26/plugins/extra/googletranslate/img/lr.png
--rw-r--r--   0 lucjean    (501) staff       (20)      391 2019-08-29 13:07:40.000000 coop_html_editor-1.3.1/coop_html_editor/static/aloha.0.23.26/plugins/extra/googletranslate/img/mv.png
--rw-r--r--   0 lucjean    (501) staff       (20)      509 2019-08-29 13:07:40.000000 coop_html_editor-1.3.1/coop_html_editor/static/aloha.0.23.26/plugins/extra/googletranslate/img/tc.png
--rw-r--r--   0 lucjean    (501) staff       (20)      388 2019-08-29 13:07:40.000000 coop_html_editor-1.3.1/coop_html_editor/static/aloha.0.23.26/plugins/extra/googletranslate/img/ug.png
--rw-r--r--   0 lucjean    (501) staff       (20)      486 2019-08-29 13:07:40.000000 coop_html_editor-1.3.1/coop_html_editor/static/aloha.0.23.26/plugins/extra/googletranslate/img/tt.png
--rw-r--r--   0 lucjean    (501) staff       (20)      243 2019-08-29 13:07:40.000000 coop_html_editor-1.3.1/coop_html_editor/static/aloha.0.23.26/plugins/extra/googletranslate/img/pl.png
--rw-r--r--   0 lucjean    (501) staff       (20)      376 2019-08-29 13:07:40.000000 coop_html_editor-1.3.1/coop_html_editor/static/aloha.0.23.26/plugins/extra/googletranslate/img/rs.png
--rw-r--r--   0 lucjean    (501) staff       (20)      377 2019-08-29 13:07:40.000000 coop_html_editor-1.3.1/coop_html_editor/static/aloha.0.23.26/plugins/extra/googletranslate/img/in.png
--rw-r--r--   0 lucjean    (501) staff       (20)      493 2019-08-29 13:07:40.000000 coop_html_editor-1.3.1/coop_html_editor/static/aloha.0.23.26/plugins/extra/googletranslate/img/ge.png
--rw-r--r--   0 lucjean    (501) staff       (20)      391 2019-08-29 13:07:40.000000 coop_html_editor-1.3.1/coop_html_editor/static/aloha.0.23.26/plugins/extra/googletranslate/img/gr.png
--rw-r--r--   0 lucjean    (501) staff       (20)      522 2019-08-29 13:07:40.000000 coop_html_editor-1.3.1/coop_html_editor/static/aloha.0.23.26/plugins/extra/googletranslate/img/gs.png
--rw-r--r--   0 lucjean    (501) staff       (20)      461 2019-08-29 13:07:40.000000 coop_html_editor-1.3.1/coop_html_editor/static/aloha.0.23.26/plugins/extra/googletranslate/img/gd.png
--rw-r--r--   0 lucjean    (501) staff       (20)      575 2019-08-29 13:07:40.000000 coop_html_editor-1.3.1/coop_html_editor/static/aloha.0.23.26/plugins/extra/googletranslate/img/io.png
--rw-r--r--   0 lucjean    (501) staff       (20)      393 2019-08-29 13:07:40.000000 coop_html_editor-1.3.1/coop_html_editor/static/aloha.0.23.26/plugins/extra/googletranslate/img/hk.png
--rw-r--r--   0 lucjean    (501) staff       (20)      424 2019-08-29 13:07:40.000000 coop_html_editor-1.3.1/coop_html_editor/static/aloha.0.23.26/plugins/extra/googletranslate/img/kp.png
--rw-r--r--   0 lucjean    (501) staff       (20)      354 2019-08-29 13:07:40.000000 coop_html_editor-1.3.1/coop_html_editor/static/aloha.0.23.26/plugins/extra/googletranslate/img/kg.png
--rw-r--r--   0 lucjean    (501) staff       (20)      572 2019-08-29 13:07:40.000000 coop_html_editor-1.3.1/coop_html_editor/static/aloha.0.23.26/plugins/extra/googletranslate/img/pm.png
--rw-r--r--   0 lucjean    (501) staff       (20)      373 2019-08-29 13:07:40.000000 coop_html_editor-1.3.1/coop_html_editor/static/aloha.0.23.26/plugins/extra/googletranslate/img/sv.png
--rw-r--r--   0 lucjean    (501) staff       (20)      369 2019-08-29 13:07:40.000000 coop_html_editor-1.3.1/coop_html_editor/static/aloha.0.23.26/plugins/extra/googletranslate/img/re.png
--rw-r--r--   0 lucjean    (501) staff       (20)      428 2019-08-29 13:07:40.000000 coop_html_editor-1.3.1/coop_html_editor/static/aloha.0.23.26/plugins/extra/googletranslate/img/sa.png
--rw-r--r--   0 lucjean    (501) staff       (20)      481 2019-08-29 13:07:40.000000 coop_html_editor-1.3.1/coop_html_editor/static/aloha.0.23.26/plugins/extra/googletranslate/img/sc.png
--rw-r--r--   0 lucjean    (501) staff       (20)      429 2019-08-29 13:07:40.000000 coop_html_editor-1.3.1/coop_html_editor/static/aloha.0.23.26/plugins/extra/googletranslate/img/st.png
--rw-r--r--   0 lucjean    (501) staff       (20)      435 2019-08-29 13:07:40.000000 coop_html_editor-1.3.1/coop_html_editor/static/aloha.0.23.26/plugins/extra/googletranslate/img/ke.png
--rw-r--r--   0 lucjean    (501) staff       (20)      507 2019-08-29 13:07:40.000000 coop_html_editor-1.3.1/coop_html_editor/static/aloha.0.23.26/plugins/extra/googletranslate/img/kr.png
--rw-r--r--   0 lucjean    (501) staff       (20)      369 2019-08-29 13:07:40.000000 coop_html_editor-1.3.1/coop_html_editor/static/aloha.0.23.26/plugins/extra/googletranslate/img/gf.png
--rw-r--r--   0 lucjean    (501) staff       (20)      378 2019-08-29 13:07:40.000000 coop_html_editor-1.3.1/coop_html_editor/static/aloha.0.23.26/plugins/extra/googletranslate/img/en.png
--rw-r--r--   0 lucjean    (501) staff       (20)      430 2019-08-29 13:07:40.000000 coop_html_editor-1.3.1/coop_html_editor/static/aloha.0.23.26/plugins/extra/googletranslate/img/dj.png
--rw-r--r--   0 lucjean    (501) staff       (20)      405 2019-08-29 13:07:40.000000 coop_html_editor-1.3.1/coop_html_editor/static/aloha.0.23.26/plugins/extra/googletranslate/img/gq.png
--rw-r--r--   0 lucjean    (501) staff       (20)      353 2019-08-29 13:07:40.000000 coop_html_editor-1.3.1/coop_html_editor/static/aloha.0.23.26/plugins/extra/googletranslate/img/gp.png
--rw-r--r--   0 lucjean    (501) staff       (20)      352 2019-08-29 13:07:40.000000 coop_html_editor-1.3.1/coop_html_editor/static/aloha.0.23.26/plugins/extra/googletranslate/img/dk.png
--rw-r--r--   0 lucjean    (501) staff       (20)      326 2019-08-29 13:07:40.000000 coop_html_editor-1.3.1/coop_html_editor/static/aloha.0.23.26/plugins/extra/googletranslate/img/il.png
--rw-r--r--   0 lucjean    (501) staff       (20)      547 2019-08-29 13:07:40.000000 coop_html_editor-1.3.1/coop_html_editor/static/aloha.0.23.26/plugins/extra/googletranslate/img/pn.png
--rw-r--r--   0 lucjean    (501) staff       (20)      520 2019-08-29 13:07:40.000000 coop_html_editor-1.3.1/coop_html_editor/static/aloha.0.23.26/plugins/extra/googletranslate/img/sb.png
--rw-r--r--   0 lucjean    (501) staff       (20)      344 2019-08-29 13:07:40.000000 coop_html_editor-1.3.1/coop_html_editor/static/aloha.0.23.26/plugins/extra/googletranslate/img/py.png
--rw-r--r--   0 lucjean    (501) staff       (20)      299 2019-08-29 13:07:40.000000 coop_html_editor-1.3.1/coop_html_editor/static/aloha.0.23.26/plugins/extra/googletranslate/img/ru.png
--rw-r--r--   0 lucjean    (501) staff       (20)      351 2019-08-29 13:07:40.000000 coop_html_editor-1.3.1/coop_html_editor/static/aloha.0.23.26/plugins/extra/googletranslate/img/kw.png
--rw-r--r--   0 lucjean    (501) staff       (20)      368 2019-08-29 13:07:40.000000 coop_html_editor-1.3.1/coop_html_editor/static/aloha.0.23.26/plugins/extra/googletranslate/img/do.png
--rw-r--r--   0 lucjean    (501) staff       (20)      333 2019-08-29 13:07:40.000000 coop_html_editor-1.3.1/coop_html_editor/static/aloha.0.23.26/plugins/extra/googletranslate/img/gt.png
--rw-r--r--   0 lucjean    (501) staff       (20)      545 2019-08-29 13:07:40.000000 coop_html_editor-1.3.1/coop_html_editor/static/aloha.0.23.26/plugins/extra/googletranslate/img/gb.png
--rw-r--r--   0 lucjean    (501) staff       (20)      384 2019-08-29 13:07:40.000000 coop_html_editor-1.3.1/coop_html_editor/static/aloha.0.23.26/plugins/extra/googletranslate/img/gu.png
--rw-r--r--   0 lucjean    (501) staff       (20)      580 2019-08-29 13:07:40.000000 coop_html_editor-1.3.1/coop_html_editor/static/aloha.0.23.26/plugins/extra/googletranslate/img/hm.png
--rw-r--r--   0 lucjean    (501) staff       (20)      350 2019-08-29 13:07:40.000000 coop_html_editor-1.3.1/coop_html_editor/static/aloha.0.23.26/plugins/extra/googletranslate/img/sg.png
--rw-r--r--   0 lucjean    (501) staff       (20)      448 2019-08-29 13:07:40.000000 coop_html_editor-1.3.1/coop_html_editor/static/aloha.0.23.26/plugins/extra/googletranslate/img/pk.png
--rw-r--r--   0 lucjean    (501) staff       (20)      370 2019-08-29 13:07:40.000000 coop_html_editor-1.3.1/coop_html_editor/static/aloha.0.23.26/plugins/extra/googletranslate/img/sr.png
--rw-r--r--   0 lucjean    (501) staff       (20)      389 2019-08-29 13:07:40.000000 coop_html_editor-1.3.1/coop_html_editor/static/aloha.0.23.26/plugins/extra/googletranslate/img/se.png
--rw-r--r--   0 lucjean    (501) staff       (20)      307 2019-08-29 13:07:40.000000 coop_html_editor-1.3.1/coop_html_editor/static/aloha.0.23.26/plugins/extra/googletranslate/img/jp.png
--rw-r--r--   0 lucjean    (501) staff       (20)      346 2019-08-29 13:07:40.000000 coop_html_editor-1.3.1/coop_html_editor/static/aloha.0.23.26/plugins/extra/googletranslate/img/gw.png
--rw-r--r--   0 lucjean    (501) staff       (20)      388 2019-08-29 13:07:40.000000 coop_html_editor-1.3.1/coop_html_editor/static/aloha.0.23.26/plugins/extra/googletranslate/img/eh.png
--rw-r--r--   0 lucjean    (501) staff       (20)      454 2019-08-29 13:07:40.000000 coop_html_editor-1.3.1/coop_html_editor/static/aloha.0.23.26/plugins/extra/googletranslate/img/dz.png
--rw-r--r--   0 lucjean    (501) staff       (20)      342 2019-08-29 13:07:40.000000 coop_html_editor-1.3.1/coop_html_editor/static/aloha.0.23.26/plugins/extra/googletranslate/img/ga.png
--rw-r--r--   0 lucjean    (501) staff       (20)      369 2019-08-29 13:07:40.000000 coop_html_editor-1.3.1/coop_html_editor/static/aloha.0.23.26/plugins/extra/googletranslate/img/fr.png
--rw-r--r--   0 lucjean    (501) staff       (20)      508 2019-08-29 13:07:40.000000 coop_html_editor-1.3.1/coop_html_editor/static/aloha.0.23.26/plugins/extra/googletranslate/img/dm.png
--rw-r--r--   0 lucjean    (501) staff       (20)      411 2019-08-29 13:07:40.000000 coop_html_editor-1.3.1/coop_html_editor/static/aloha.0.23.26/plugins/extra/googletranslate/img/hn.png
--rw-r--r--   0 lucjean    (501) staff       (20)      364 2019-08-29 13:07:40.000000 coop_html_editor-1.3.1/coop_html_editor/static/aloha.0.23.26/plugins/extra/googletranslate/img/sd.png
--rw-r--r--   0 lucjean    (501) staff       (20)      382 2019-08-29 13:07:40.000000 coop_html_editor-1.3.1/coop_html_editor/static/aloha.0.23.26/plugins/extra/googletranslate/img/rw.png
--rw-r--r--   0 lucjean    (501) staff       (20)      416 2019-08-29 13:07:40.000000 coop_html_editor-1.3.1/coop_html_editor/static/aloha.0.23.26/plugins/extra/googletranslate/img/ph.png
--rw-r--r--   0 lucjean    (501) staff       (20)      343 2019-08-29 13:07:40.000000 coop_html_editor-1.3.1/coop_html_editor/static/aloha.0.23.26/plugins/extra/googletranslate/img/qa.png
--rw-r--r--   0 lucjean    (501) staff       (20)      264 2019-08-29 13:07:40.000000 coop_html_editor-1.3.1/coop_html_editor/static/aloha.0.23.26/plugins/extra/googletranslate/img/pe.png
--rw-r--r--   0 lucjean    (501) staff       (20)      445 2019-08-29 13:07:40.000000 coop_html_editor-1.3.1/coop_html_editor/static/aloha.0.23.26/plugins/extra/googletranslate/img/pr.png
--rw-r--r--   0 lucjean    (501) staff       (20)      383 2019-08-29 13:07:40.000000 coop_html_editor-1.3.1/coop_html_editor/static/aloha.0.23.26/plugins/extra/googletranslate/img/si.png
--rw-r--r--   0 lucjean    (501) staff       (20)      327 2019-08-29 13:07:40.000000 coop_html_editor-1.3.1/coop_html_editor/static/aloha.0.23.26/plugins/extra/googletranslate/img/ht.png
--rw-r--r--   0 lucjean    (501) staff       (20)      344 2019-08-29 13:07:40.000000 coop_html_editor-1.3.1/coop_html_editor/static/aloha.0.23.26/plugins/extra/googletranslate/img/es.png
--rw-r--r--   0 lucjean    (501) staff       (20)      351 2019-08-29 13:07:40.000000 coop_html_editor-1.3.1/coop_html_editor/static/aloha.0.23.26/plugins/extra/googletranslate/img/gl.png
--rw-r--r--   0 lucjean    (501) staff       (20)      363 2019-08-29 13:07:40.000000 coop_html_editor-1.3.1/coop_html_editor/static/aloha.0.23.26/plugins/extra/googletranslate/img/gm.png
--rw-r--r--   0 lucjean    (501) staff       (20)      497 2019-08-29 13:07:40.000000 coop_html_editor-1.3.1/coop_html_editor/static/aloha.0.23.26/plugins/extra/googletranslate/img/er.png
--rw-r--r--   0 lucjean    (501) staff       (20)      368 2019-08-29 13:07:40.000000 coop_html_editor-1.3.1/coop_html_editor/static/aloha.0.23.26/plugins/extra/googletranslate/img/fi.png
--rw-r--r--   0 lucjean    (501) staff       (20)      297 2019-08-29 13:07:40.000000 coop_html_editor-1.3.1/coop_html_editor/static/aloha.0.23.26/plugins/extra/googletranslate/img/ee.png
--rw-r--r--   0 lucjean    (501) staff       (20)      480 2019-08-29 13:07:40.000000 coop_html_editor-1.3.1/coop_html_editor/static/aloha.0.23.26/plugins/extra/googletranslate/img/kn.png
--rw-r--r--   0 lucjean    (501) staff       (20)      293 2019-08-29 13:07:40.000000 coop_html_editor-1.3.1/coop_html_editor/static/aloha.0.23.26/plugins/extra/googletranslate/img/hu.png
--rw-r--r--   0 lucjean    (501) staff       (20)      403 2019-08-29 13:07:40.000000 coop_html_editor-1.3.1/coop_html_editor/static/aloha.0.23.26/plugins/extra/googletranslate/img/iq.png
--rw-r--r--   0 lucjean    (501) staff       (20)      532 2019-08-29 13:07:40.000000 coop_html_editor-1.3.1/coop_html_editor/static/aloha.0.23.26/plugins/extra/googletranslate/img/ky.png
--rw-r--r--   0 lucjean    (501) staff       (20)      524 2019-08-29 13:07:40.000000 coop_html_editor-1.3.1/coop_html_editor/static/aloha.0.23.26/plugins/extra/googletranslate/img/sh.png
--rw-r--r--   0 lucjean    (501) staff       (20)      348 2019-08-29 13:07:40.000000 coop_html_editor-1.3.1/coop_html_editor/static/aloha.0.23.26/plugins/extra/googletranslate/img/ps.png
--rw-r--r--   0 lucjean    (501) staff       (20)      379 2019-08-29 13:07:40.000000 coop_html_editor-1.3.1/coop_html_editor/static/aloha.0.23.26/plugins/extra/googletranslate/img/pf.png
--rw-r--r--   0 lucjean    (501) staff       (20)      397 2019-08-29 13:07:40.000000 coop_html_editor-1.3.1/coop_html_editor/static/aloha.0.23.26/plugins/extra/googletranslate/img/sj.png
--rw-r--r--   0 lucjean    (501) staff       (20)      301 2019-08-29 13:07:40.000000 coop_html_editor-1.3.1/coop_html_editor/static/aloha.0.23.26/plugins/extra/googletranslate/img/id.png
--rw-r--r--   0 lucjean    (501) staff       (20)      410 2019-08-29 13:07:40.000000 coop_html_editor-1.3.1/coop_html_editor/static/aloha.0.23.26/plugins/extra/googletranslate/img/is.png
--rw-r--r--   0 lucjean    (501) staff       (20)      348 2019-08-29 13:07:40.000000 coop_html_editor-1.3.1/coop_html_editor/static/aloha.0.23.26/plugins/extra/googletranslate/img/eg.png
--rw-r--r--   0 lucjean    (501) staff       (20)      526 2019-08-29 13:07:40.000000 coop_html_editor-1.3.1/coop_html_editor/static/aloha.0.23.26/plugins/extra/googletranslate/img/fk.png
--rw-r--r--   0 lucjean    (501) staff       (20)      517 2019-08-29 13:07:40.000000 coop_html_editor-1.3.1/coop_html_editor/static/aloha.0.23.26/plugins/extra/googletranslate/img/fj.png
--rw-r--r--   0 lucjean    (501) staff       (20)      319 2019-08-29 13:07:40.000000 coop_html_editor-1.3.1/coop_html_editor/static/aloha.0.23.26/plugins/extra/googletranslate/img/gn.png
--rw-r--r--   0 lucjean    (501) staff       (20)      521 2019-08-29 13:07:40.000000 coop_html_editor-1.3.1/coop_html_editor/static/aloha.0.23.26/plugins/extra/googletranslate/img/gy.png
--rw-r--r--   0 lucjean    (501) staff       (20)      398 2019-08-29 13:07:40.000000 coop_html_editor-1.3.1/coop_html_editor/static/aloha.0.23.26/plugins/extra/googletranslate/img/ir.png
--rw-r--r--   0 lucjean    (501) staff       (20)      456 2019-08-29 13:07:40.000000 coop_html_editor-1.3.1/coop_html_editor/static/aloha.0.23.26/plugins/extra/googletranslate/img/km.png
--rw-r--r--   0 lucjean    (501) staff       (20)      333 2019-08-29 13:07:40.000000 coop_html_editor-1.3.1/coop_html_editor/static/aloha.0.23.26/plugins/extra/googletranslate/img/ie.png
--rw-r--r--   0 lucjean    (501) staff       (20)      459 2019-08-29 13:07:40.000000 coop_html_editor-1.3.1/coop_html_editor/static/aloha.0.23.26/plugins/extra/googletranslate/img/kz.png
--rw-r--r--   0 lucjean    (501) staff       (20)      333 2019-08-29 13:07:40.000000 coop_html_editor-1.3.1/coop_html_editor/static/aloha.0.23.26/plugins/extra/googletranslate/img/ro.png
--rw-r--r--   0 lucjean    (501) staff       (20)      439 2019-08-29 13:07:40.000000 coop_html_editor-1.3.1/coop_html_editor/static/aloha.0.23.26/plugins/extra/googletranslate/img/sk.png
--rw-r--r--   0 lucjean    (501) staff       (20)      438 2019-08-29 13:07:40.000000 coop_html_editor-1.3.1/coop_html_editor/static/aloha.0.23.26/plugins/extra/googletranslate/img/pg.png
--rw-r--r--   0 lucjean    (501) staff       (20)      407 2019-08-29 13:07:40.000000 coop_html_editor-1.3.1/coop_html_editor/static/aloha.0.23.26/plugins/extra/googletranslate/img/pt.png
--rw-r--r--   0 lucjean    (501) staff       (20)      376 2019-08-29 13:07:40.000000 coop_html_editor-1.3.1/coop_html_editor/static/aloha.0.23.26/plugins/extra/googletranslate/img/so.png
--rw-r--r--   0 lucjean    (501) staff       (20)      386 2019-08-29 13:07:40.000000 coop_html_editor-1.3.1/coop_html_editor/static/aloha.0.23.26/plugins/extra/googletranslate/img/hr.png
--rw-r--r--   0 lucjean    (501) staff       (20)      551 2019-08-29 13:07:40.000000 coop_html_editor-1.3.1/coop_html_editor/static/aloha.0.23.26/plugins/extra/googletranslate/img/ki.png
--rw-r--r--   0 lucjean    (501) staff       (20)      508 2019-08-29 13:07:40.000000 coop_html_editor-1.3.1/coop_html_editor/static/aloha.0.23.26/plugins/extra/googletranslate/img/jm.png
--rw-r--r--   0 lucjean    (501) staff       (20)      355 2019-08-29 13:07:40.000000 coop_html_editor-1.3.1/coop_html_editor/static/aloha.0.23.26/plugins/extra/googletranslate/img/ec.png
--rw-r--r--   0 lucjean    (501) staff       (20)      445 2019-08-29 13:07:40.000000 coop_html_editor-1.3.1/coop_html_editor/static/aloha.0.23.26/plugins/extra/googletranslate/img/et.png
--rw-r--r--   0 lucjean    (501) staff       (20)      377 2019-08-29 13:07:40.000000 coop_html_editor-1.3.1/coop_html_editor/static/aloha.0.23.26/plugins/extra/googletranslate/img/fo.png
--rw-r--r--   0 lucjean    (501) staff       (20)      422 2019-08-29 13:07:40.000000 coop_html_editor-1.3.1/coop_html_editor/static/aloha.0.23.26/plugins/extra/googletranslate/img/kh.png
--rw-r--r--   0 lucjean    (501) staff       (20)      322 2019-08-29 13:07:40.000000 coop_html_editor-1.3.1/coop_html_editor/static/aloha.0.23.26/plugins/extra/googletranslate/img/sy.png
--rw-r--r--   0 lucjean    (501) staff       (20)      356 2019-08-29 13:07:40.000000 coop_html_editor-1.3.1/coop_html_editor/static/aloha.0.23.26/plugins/extra/googletranslate/img/sn.png
--rw-r--r--   0 lucjean    (501) staff       (20)      424 2019-08-29 13:07:40.000000 coop_html_editor-1.3.1/coop_html_editor/static/aloha.0.23.26/plugins/extra/googletranslate/img/pw.png
--rw-r--r--   0 lucjean    (501) staff       (20)      321 2019-08-29 13:07:40.000000 coop_html_editor-1.3.1/coop_html_editor/static/aloha.0.23.26/plugins/extra/googletranslate/img/sl.png
--rw-r--r--   0 lucjean    (501) staff       (20)      409 2019-08-29 13:07:40.000000 coop_html_editor-1.3.1/coop_html_editor/static/aloha.0.23.26/plugins/extra/googletranslate/img/fm.png
--rw-r--r--   0 lucjean    (501) staff       (20)      369 2019-08-29 13:07:40.000000 coop_html_editor-1.3.1/coop_html_editor/static/aloha.0.23.26/plugins/extra/googletranslate/img/gi.png
--rw-r--r--   0 lucjean    (501) staff       (20)      364 2019-08-29 13:07:40.000000 coop_html_editor-1.3.1/coop_html_editor/static/aloha.0.23.26/plugins/extra/googletranslate/img/de.png
--rw-r--r--   0 lucjean    (501) staff       (20)      336 2019-08-29 13:07:40.000000 coop_html_editor-1.3.1/coop_html_editor/static/aloha.0.23.26/plugins/extra/googletranslate/img/gh.png
--rw-r--r--   0 lucjean    (501) staff       (20)      353 2019-08-29 13:07:40.000000 coop_html_editor-1.3.1/coop_html_editor/static/aloha.0.23.26/plugins/extra/googletranslate/img/jo.png
--rw-r--r--   0 lucjean    (501) staff       (20)      283 2019-08-29 13:07:40.000000 coop_html_editor-1.3.1/coop_html_editor/static/aloha.0.23.26/plugins/extra/googletranslate/img/it.png
--rw-r--r--   0 lucjean    (501) staff       (20)      390 2019-08-29 13:07:40.000000 coop_html_editor-1.3.1/coop_html_editor/static/aloha.0.23.26/plugins/extra/googletranslate/img/pa.png
--rw-r--r--   0 lucjean    (501) staff       (20)      508 2019-08-29 13:07:40.000000 coop_html_editor-1.3.1/coop_html_editor/static/aloha.0.23.26/plugins/extra/googletranslate/img/sz.png
--rw-r--r--   0 lucjean    (501) staff       (20)      396 2019-08-29 13:07:40.000000 coop_html_editor-1.3.1/coop_html_editor/static/aloha.0.23.26/plugins/extra/googletranslate/img/sm.png
--rw-r--r--   0 lucjean    (501) staff       (20)      367 2019-08-29 13:07:40.000000 coop_html_editor-1.3.1/coop_html_editor/static/aloha.0.23.26/plugins/extra/googletranslate/img/tn.png
--rw-r--r--   0 lucjean    (501) staff       (20)      322 2019-08-29 13:07:40.000000 coop_html_editor-1.3.1/coop_html_editor/static/aloha.0.23.26/plugins/extra/googletranslate/img/ml.png
--rw-r--r--   0 lucjean    (501) staff       (20)      380 2019-08-29 13:07:40.000000 coop_html_editor-1.3.1/coop_html_editor/static/aloha.0.23.26/plugins/extra/googletranslate/img/cg.png
--rw-r--r--   0 lucjean    (501) staff       (20)      480 2019-08-29 13:07:40.000000 coop_html_editor-1.3.1/coop_html_editor/static/aloha.0.23.26/plugins/extra/googletranslate/img/ax.png
--rw-r--r--   0 lucjean    (501) staff       (20)      395 2019-08-29 13:07:40.000000 coop_html_editor-1.3.1/coop_html_editor/static/aloha.0.23.26/plugins/extra/googletranslate/img/ao.png
--rw-r--r--   0 lucjean    (501) staff       (20)      471 2019-08-29 13:07:40.000000 coop_html_editor-1.3.1/coop_html_editor/static/aloha.0.23.26/plugins/extra/googletranslate/img/bt.png
--rw-r--r--   0 lucjean    (501) staff       (20)      365 2019-08-29 13:07:40.000000 coop_html_editor-1.3.1/coop_html_editor/static/aloha.0.23.26/plugins/extra/googletranslate/img/an.png
--rw-r--r--   0 lucjean    (501) staff       (20)      403 2019-08-29 13:07:40.000000 coop_html_editor-1.3.1/coop_html_editor/static/aloha.0.23.26/plugins/extra/googletranslate/img/bb.png
--rw-r--r--   0 lucjean    (501) staff       (20)      456 2019-08-29 13:07:40.000000 coop_html_editor-1.3.1/coop_html_editor/static/aloha.0.23.26/plugins/extra/googletranslate/img/cf.png
--rw-r--r--   0 lucjean    (501) staff       (20)      336 2019-08-29 13:07:40.000000 coop_html_editor-1.3.1/coop_html_editor/static/aloha.0.23.26/plugins/extra/googletranslate/img/mm.png
--rw-r--r--   0 lucjean    (501) staff       (20)      399 2019-08-29 13:07:40.000000 coop_html_editor-1.3.1/coop_html_editor/static/aloha.0.23.26/plugins/extra/googletranslate/img/li.png
--rw-r--r--   0 lucjean    (501) staff       (20)      559 2019-08-29 13:07:40.000000 coop_html_editor-1.3.1/coop_html_editor/static/aloha.0.23.26/plugins/extra/googletranslate/img/na.png
--rw-r--r--   0 lucjean    (501) staff       (20)      439 2019-08-29 13:07:40.000000 coop_html_editor-1.3.1/coop_html_editor/static/aloha.0.23.26/plugins/extra/googletranslate/img/mz.png
--rw-r--r--   0 lucjean    (501) staff       (20)      302 2019-08-29 13:07:40.000000 coop_html_editor-1.3.1/coop_html_editor/static/aloha.0.23.26/plugins/extra/googletranslate/img/to.png
--rw-r--r--   0 lucjean    (501) staff       (20)      510 2019-08-29 13:07:40.000000 coop_html_editor-1.3.1/coop_html_editor/static/aloha.0.23.26/plugins/extra/googletranslate/img/vg.png
--rw-r--r--   0 lucjean    (501) staff       (20)      412 2019-08-29 13:07:40.000000 coop_html_editor-1.3.1/coop_html_editor/static/aloha.0.23.26/plugins/extra/googletranslate/img/ve.png
--rw-r--r--   0 lucjean    (501) staff       (20)      514 2019-08-29 13:07:40.000000 coop_html_editor-1.3.1/coop_html_editor/static/aloha.0.23.26/plugins/extra/googletranslate/img/tz.png
--rw-r--r--   0 lucjean    (501) staff       (20)      456 2019-08-29 13:07:40.000000 coop_html_editor-1.3.1/coop_html_editor/static/aloha.0.23.26/plugins/extra/googletranslate/img/tm.png
--rw-r--r--   0 lucjean    (501) staff       (20)      424 2019-08-29 13:07:40.000000 coop_html_editor-1.3.1/coop_html_editor/static/aloha.0.23.26/plugins/extra/googletranslate/img/mx.png
--rw-r--r--   0 lucjean    (501) staff       (20)      470 2019-08-29 13:07:40.000000 coop_html_editor-1.3.1/coop_html_editor/static/aloha.0.23.26/plugins/extra/googletranslate/img/nc.png
--rw-r--r--   0 lucjean    (501) staff       (20)      456 2019-08-29 13:07:40.000000 coop_html_editor-1.3.1/coop_html_editor/static/aloha.0.23.26/plugins/extra/googletranslate/img/mo.png
--rw-r--r--   0 lucjean    (501) staff       (20)      464 2019-08-29 13:07:40.000000 coop_html_editor-1.3.1/coop_html_editor/static/aloha.0.23.26/plugins/extra/googletranslate/img/lk.png
--rw-r--r--   0 lucjean    (501) staff       (20)      477 2019-08-29 13:07:40.000000 coop_html_editor-1.3.1/coop_html_editor/static/aloha.0.23.26/plugins/extra/googletranslate/img/cd.png
--rw-r--r--   0 lucjean    (501) staff       (20)      434 2019-08-29 13:07:40.000000 coop_html_editor-1.3.1/coop_html_editor/static/aloha.0.23.26/plugins/extra/googletranslate/img/al.png
--rw-r--r--   0 lucjean    (501) staff       (20)      327 2019-08-29 13:07:40.000000 coop_html_editor-1.3.1/coop_html_editor/static/aloha.0.23.26/plugins/extra/googletranslate/img/bw.png
--rw-r--r--   0 lucjean    (501) staff       (20)      321 2019-08-29 13:07:40.000000 coop_html_editor-1.3.1/coop_html_editor/static/aloha.0.23.26/plugins/extra/googletranslate/img/cs.png
--rw-r--r--   0 lucjean    (501) staff       (20)      349 2019-08-29 13:07:40.000000 coop_html_editor-1.3.1/coop_html_editor/static/aloha.0.23.26/plugins/extra/googletranslate/img/cr.png
--rw-r--r--   0 lucjean    (501) staff       (20)      397 2019-08-29 13:07:40.000000 coop_html_editor-1.3.1/coop_html_editor/static/aloha.0.23.26/plugins/extra/googletranslate/img/bv.png
--rw-r--r--   0 lucjean    (501) staff       (20)      332 2019-08-29 13:07:40.000000 coop_html_editor-1.3.1/coop_html_editor/static/aloha.0.23.26/plugins/extra/googletranslate/img/am.png
--rw-r--r--   0 lucjean    (501) staff       (20)      423 2019-08-29 13:07:40.000000 coop_html_editor-1.3.1/coop_html_editor/static/aloha.0.23.26/plugins/extra/googletranslate/img/az.png
--rw-r--r--   0 lucjean    (501) staff       (20)      471 2019-08-29 13:07:40.000000 coop_html_editor-1.3.1/coop_html_editor/static/aloha.0.23.26/plugins/extra/googletranslate/img/ba.png
--rw-r--r--   0 lucjean    (501) staff       (20)      343 2019-08-29 13:07:40.000000 coop_html_editor-1.3.1/coop_html_editor/static/aloha.0.23.26/plugins/extra/googletranslate/img/mn.png
--rw-r--r--   0 lucjean    (501) staff       (20)      468 2019-08-29 13:07:40.000000 coop_html_editor-1.3.1/coop_html_editor/static/aloha.0.23.26/plugins/extra/googletranslate/img/nu.png
--rw-r--r--   0 lucjean    (501) staff       (20)      464 2019-08-29 13:07:40.000000 coop_html_editor-1.3.1/coop_html_editor/static/aloha.0.23.26/plugins/extra/googletranslate/img/my.png
--rw-r--r--   0 lucjean    (501) staff       (20)      418 2019-08-29 13:07:40.000000 coop_html_editor-1.3.1/coop_html_editor/static/aloha.0.23.26/plugins/extra/googletranslate/img/europeanunion.png
--rw-r--r--   0 lucjean    (501) staff       (20)      395 2019-08-29 13:07:40.000000 coop_html_editor-1.3.1/coop_html_editor/static/aloha.0.23.26/plugins/extra/googletranslate/img/tl.png
--rw-r--r--   0 lucjean    (501) staff       (20)      352 2019-08-29 13:07:40.000000 coop_html_editor-1.3.1/coop_html_editor/static/aloha.0.23.26/plugins/extra/googletranslate/img/ws.png
--rw-r--r--   0 lucjean    (501) staff       (20)      327 2019-08-29 13:07:40.000000 coop_html_editor-1.3.1/coop_html_editor/static/aloha.0.23.26/plugins/extra/googletranslate/img/th.png
--rw-r--r--   0 lucjean    (501) staff       (20)      474 2019-08-29 13:07:40.000000 coop_html_editor-1.3.1/coop_html_editor/static/aloha.0.23.26/plugins/extra/googletranslate/img/nf.png
--rw-r--r--   0 lucjean    (501) staff       (20)      277 2019-08-29 13:07:40.000000 coop_html_editor-1.3.1/coop_html_editor/static/aloha.0.23.26/plugins/extra/googletranslate/img/ly.png
--rw-r--r--   0 lucjean    (501) staff       (20)      516 2019-08-29 13:07:40.000000 coop_html_editor-1.3.1/coop_html_editor/static/aloha.0.23.26/plugins/extra/googletranslate/img/ai.png
--rw-r--r--   0 lucjean    (501) staff       (20)      486 2019-08-29 13:07:40.000000 coop_html_editor-1.3.1/coop_html_editor/static/aloha.0.23.26/plugins/extra/googletranslate/img/br.png
--rw-r--r--   0 lucjean    (501) staff       (20)      441 2019-08-29 13:07:40.000000 coop_html_editor-1.3.1/coop_html_editor/static/aloha.0.23.26/plugins/extra/googletranslate/img/cv.png
--rw-r--r--   0 lucjean    (501) staff       (20)      294 2019-08-29 13:07:40.000000 coop_html_editor-1.3.1/coop_html_editor/static/aloha.0.23.26/plugins/extra/googletranslate/img/be.png
--rw-r--r--   0 lucjean    (501) staff       (20)      471 2019-08-29 13:07:40.000000 coop_html_editor-1.3.1/coop_html_editor/static/aloha.0.23.26/plugins/extra/googletranslate/img/ca.png
--rw-r--r--   0 lucjean    (501) staff       (20)      372 2019-08-29 13:07:40.000000 coop_html_editor-1.3.1/coop_html_editor/static/aloha.0.23.26/plugins/extra/googletranslate/img/bd.png
--rw-r--r--   0 lucjean    (501) staff       (20)      391 2019-08-29 13:07:40.000000 coop_html_editor-1.3.1/coop_html_editor/static/aloha.0.23.26/plugins/extra/googletranslate/img/bs.png
--rw-r--r--   0 lucjean    (501) staff       (20)      341 2019-08-29 13:07:40.000000 coop_html_editor-1.3.1/coop_html_editor/static/aloha.0.23.26/plugins/extra/googletranslate/img/ng.png
--rw-r--r--   0 lucjean    (501) staff       (20)      449 2019-08-29 13:07:40.000000 coop_html_editor-1.3.1/coop_html_editor/static/aloha.0.23.26/plugins/extra/googletranslate/img/mk.png
--rw-r--r--   0 lucjean    (501) staff       (20)      349 2019-08-29 13:07:40.000000 coop_html_editor-1.3.1/coop_html_editor/static/aloha.0.23.26/plugins/extra/googletranslate/img/np.png
--rw-r--r--   0 lucjean    (501) staff       (20)      419 2019-08-29 13:07:40.000000 coop_html_editor-1.3.1/coop_html_editor/static/aloha.0.23.26/plugins/extra/googletranslate/img/va.png
--rw-r--r--   0 lucjean    (501) staff       (20)      411 2019-08-29 13:07:40.000000 coop_html_editor-1.3.1/coop_html_editor/static/aloha.0.23.26/plugins/extra/googletranslate/img/uz.png
--rw-r--r--   0 lucjean    (501) staff       (20)      557 2019-08-29 13:07:40.000000 coop_html_editor-1.3.1/coop_html_editor/static/aloha.0.23.26/plugins/extra/googletranslate/img/wales.png
--rw-r--r--   0 lucjean    (501) staff       (20)      455 2019-08-29 13:07:40.000000 coop_html_editor-1.3.1/coop_html_editor/static/aloha.0.23.26/plugins/extra/googletranslate/img/um.png
--rw-r--r--   0 lucjean    (501) staff       (20)      522 2019-08-29 13:07:40.000000 coop_html_editor-1.3.1/coop_html_editor/static/aloha.0.23.26/plugins/extra/googletranslate/img/tk.png
--rw-r--r--   0 lucjean    (501) staff       (20)      412 2019-08-29 13:07:40.000000 coop_html_editor-1.3.1/coop_html_editor/static/aloha.0.23.26/plugins/extra/googletranslate/img/vc.png
--rw-r--r--   0 lucjean    (501) staff       (20)      462 2019-08-29 13:07:40.000000 coop_html_editor-1.3.1/coop_html_editor/static/aloha.0.23.26/plugins/extra/googletranslate/img/zw.png
--rw-r--r--   0 lucjean    (501) staff       (20)      391 2019-08-29 13:07:40.000000 coop_html_editor-1.3.1/coop_html_editor/static/aloha.0.23.26/plugins/extra/googletranslate/img/nr.png
--rw-r--r--   0 lucjean    (501) staff       (20)      393 2019-08-29 13:07:40.000000 coop_html_editor-1.3.1/coop_html_editor/static/aloha.0.23.26/plugins/extra/googletranslate/img/ne.png
--rw-r--r--   0 lucjean    (501) staff       (20)      445 2019-08-29 13:07:40.000000 coop_html_editor-1.3.1/coop_html_editor/static/aloha.0.23.26/plugins/extra/googletranslate/img/cu.png
--rw-r--r--   0 lucjean    (501) staff       (20)      341 2019-08-29 13:07:40.000000 coop_html_editor-1.3.1/coop_html_editor/static/aloha.0.23.26/plugins/extra/googletranslate/img/bf.png
--rw-r--r--   0 lucjean    (501) staff       (20)      320 2019-08-29 13:07:40.000000 coop_html_editor-1.3.1/coop_html_editor/static/aloha.0.23.26/plugins/extra/googletranslate/img/bg.png
--rw-r--r--   0 lucjean    (501) staff       (20)      496 2019-08-29 13:07:40.000000 coop_html_editor-1.3.1/coop_html_editor/static/aloha.0.23.26/plugins/extra/googletranslate/img/cc.png
--rw-r--r--   0 lucjean    (501) staff       (20)      518 2019-08-29 13:07:40.000000 coop_html_editor-1.3.1/coop_html_editor/static/aloha.0.23.26/plugins/extra/googletranslate/img/mh.png
--rw-r--r--   0 lucjean    (501) staff       (20)      523 2019-08-29 13:07:40.000000 coop_html_editor-1.3.1/coop_html_editor/static/aloha.0.23.26/plugins/extra/googletranslate/img/za.png
--rw-r--r--   0 lucjean    (501) staff       (20)      353 2019-08-29 13:07:40.000000 coop_html_editor-1.3.1/coop_html_editor/static/aloha.0.23.26/plugins/extra/googletranslate/img/catalonia.png
--rw-r--r--   0 lucjean    (501) staff       (20)      411 2019-08-29 13:07:40.000000 coop_html_editor-1.3.1/coop_html_editor/static/aloha.0.23.26/plugins/extra/googletranslate/img/uy.png
--rw-r--r--   0 lucjean    (501) staff       (20)      438 2019-08-29 13:07:40.000000 coop_html_editor-1.3.1/coop_html_editor/static/aloha.0.23.26/plugins/extra/googletranslate/img/wf.png
--rw-r--r--   0 lucjean    (501) staff       (20)      450 2019-08-29 13:07:40.000000 coop_html_editor-1.3.1/coop_html_editor/static/aloha.0.23.26/plugins/extra/googletranslate/img/vu.png
--rw-r--r--   0 lucjean    (501) staff       (20)      367 2019-08-29 13:07:40.000000 coop_html_editor-1.3.1/coop_html_editor/static/aloha.0.23.26/plugins/extra/googletranslate/img/tj.png
--rw-r--r--   0 lucjean    (501) staff       (20)        3 2019-08-29 13:07:40.000000 coop_html_editor-1.3.1/coop_html_editor/static/aloha.0.23.26/plugins/extra/googletranslate/package.json
-drwxr-xr-x   0 lucjean    (501) staff       (20)        0 2019-08-30 10:39:49.000000 coop_html_editor-1.3.1/coop_html_editor/static/aloha.0.23.26/plugins/extra/googletranslate/lib/
--rw-r--r--   0 lucjean    (501) staff       (20)     6636 2019-08-29 13:07:40.000000 coop_html_editor-1.3.1/coop_html_editor/static/aloha.0.23.26/plugins/extra/googletranslate/lib/googletranslate-plugin.js
-drwxr-xr-x   0 lucjean    (501) staff       (20)        0 2019-08-30 10:39:35.000000 coop_html_editor-1.3.1/coop_html_editor/static/aloha.0.23.26/plugins/extra/captioned-image/
-drwxr-xr-x   0 lucjean    (501) staff       (20)        0 2019-08-30 10:39:42.000000 coop_html_editor-1.3.1/coop_html_editor/static/aloha.0.23.26/plugins/extra/captioned-image/css/
--rw-r--r--   0 lucjean    (501) staff       (20)      780 2019-08-29 13:07:39.000000 coop_html_editor-1.3.1/coop_html_editor/static/aloha.0.23.26/plugins/extra/captioned-image/css/captioned-image.css
-drwxr-xr-x   0 lucjean    (501) staff       (20)        0 2019-08-30 10:39:42.000000 coop_html_editor-1.3.1/coop_html_editor/static/aloha.0.23.26/plugins/extra/captioned-image/lib/
--rw-r--r--   0 lucjean    (501) staff       (20)    15730 2019-08-29 13:07:39.000000 coop_html_editor-1.3.1/coop_html_editor/static/aloha.0.23.26/plugins/extra/captioned-image/lib/captioned-image-plugin.js
-drwxr-xr-x   0 lucjean    (501) staff       (20)        0 2019-08-30 10:39:53.000000 coop_html_editor-1.3.1/coop_html_editor/static/aloha.0.23.26/plugins/extra/ribbon/
-drwxr-xr-x   0 lucjean    (501) staff       (20)        0 2019-08-30 10:39:53.000000 coop_html_editor-1.3.1/coop_html_editor/static/aloha.0.23.26/plugins/extra/ribbon/css/
--rw-r--r--   0 lucjean    (501) staff       (20)     1759 2019-08-29 13:07:41.000000 coop_html_editor-1.3.1/coop_html_editor/static/aloha.0.23.26/plugins/extra/ribbon/css/ribbon.css
--rw-r--r--   0 lucjean    (501) staff       (20)      298 2019-08-29 13:07:41.000000 coop_html_editor-1.3.1/coop_html_editor/static/aloha.0.23.26/plugins/extra/ribbon/README.md
-drwxr-xr-x   0 lucjean    (501) staff       (20)        0 2019-08-30 10:39:53.000000 coop_html_editor-1.3.1/coop_html_editor/static/aloha.0.23.26/plugins/extra/ribbon/img/
--rw-r--r--   0 lucjean    (501) staff       (20)      292 2019-08-29 13:07:41.000000 coop_html_editor-1.3.1/coop_html_editor/static/aloha.0.23.26/plugins/extra/ribbon/img/fade-out.png
--rw-r--r--   0 lucjean    (501) staff       (20)      278 2019-08-29 13:07:41.000000 coop_html_editor-1.3.1/coop_html_editor/static/aloha.0.23.26/plugins/extra/ribbon/img/fade-in.png
--rw-r--r--   0 lucjean    (501) staff       (20)        3 2019-08-29 13:07:41.000000 coop_html_editor-1.3.1/coop_html_editor/static/aloha.0.23.26/plugins/extra/ribbon/package.json
-drwxr-xr-x   0 lucjean    (501) staff       (20)        0 2019-08-30 10:39:50.000000 coop_html_editor-1.3.1/coop_html_editor/static/aloha.0.23.26/plugins/extra/linkbrowser/
-drwxr-xr-x   0 lucjean    (501) staff       (20)        0 2019-08-30 10:39:35.000000 coop_html_editor-1.3.1/coop_html_editor/static/aloha.0.23.26/plugins/extra/linkbrowser/nls/
-drwxr-xr-x   0 lucjean    (501) staff       (20)        0 2019-08-30 10:39:52.000000 coop_html_editor-1.3.1/coop_html_editor/static/aloha.0.23.26/plugins/extra/linkbrowser/nls/zh-hans/
--rw-r--r--   0 lucjean    (501) staff       (20)      174 2019-08-29 13:07:41.000000 coop_html_editor-1.3.1/coop_html_editor/static/aloha.0.23.26/plugins/extra/linkbrowser/nls/zh-hans/i18n.js
-drwxr-xr-x   0 lucjean    (501) staff       (20)        0 2019-08-30 10:39:52.000000 coop_html_editor-1.3.1/coop_html_editor/static/aloha.0.23.26/plugins/extra/linkbrowser/nls/ca/
--rw-r--r--   0 lucjean    (501) staff       (20)      192 2019-08-29 13:07:41.000000 coop_html_editor-1.3.1/coop_html_editor/static/aloha.0.23.26/plugins/extra/linkbrowser/nls/ca/i18n.js
-drwxr-xr-x   0 lucjean    (501) staff       (20)        0 2019-08-30 10:39:52.000000 coop_html_editor-1.3.1/coop_html_editor/static/aloha.0.23.26/plugins/extra/linkbrowser/nls/ru/
--rw-r--r--   0 lucjean    (501) staff       (20)      226 2019-08-29 13:07:41.000000 coop_html_editor-1.3.1/coop_html_editor/static/aloha.0.23.26/plugins/extra/linkbrowser/nls/ru/i18n.js
-drwxr-xr-x   0 lucjean    (501) staff       (20)        0 2019-08-30 10:39:52.000000 coop_html_editor-1.3.1/coop_html_editor/static/aloha.0.23.26/plugins/extra/linkbrowser/nls/uk/
--rw-r--r--   0 lucjean    (501) staff       (20)      250 2019-08-29 13:07:41.000000 coop_html_editor-1.3.1/coop_html_editor/static/aloha.0.23.26/plugins/extra/linkbrowser/nls/uk/i18n.js
-drwxr-xr-x   0 lucjean    (501) staff       (20)        0 2019-08-30 10:39:52.000000 coop_html_editor-1.3.1/coop_html_editor/static/aloha.0.23.26/plugins/extra/linkbrowser/nls/mk/
--rw-r--r--   0 lucjean    (501) staff       (20)      202 2019-08-29 13:07:41.000000 coop_html_editor-1.3.1/coop_html_editor/static/aloha.0.23.26/plugins/extra/linkbrowser/nls/mk/i18n.js
-drwxr-xr-x   0 lucjean    (501) staff       (20)        0 2019-08-30 10:39:52.000000 coop_html_editor-1.3.1/coop_html_editor/static/aloha.0.23.26/plugins/extra/linkbrowser/nls/pt-br/
--rw-r--r--   0 lucjean    (501) staff       (20)      172 2019-08-29 13:07:41.000000 coop_html_editor-1.3.1/coop_html_editor/static/aloha.0.23.26/plugins/extra/linkbrowser/nls/pt-br/i18n.js
-drwxr-xr-x   0 lucjean    (501) staff       (20)        0 2019-08-30 10:39:52.000000 coop_html_editor-1.3.1/coop_html_editor/static/aloha.0.23.26/plugins/extra/linkbrowser/nls/de/
--rw-r--r--   0 lucjean    (501) staff       (20)      189 2019-08-29 13:07:41.000000 coop_html_editor-1.3.1/coop_html_editor/static/aloha.0.23.26/plugins/extra/linkbrowser/nls/de/i18n.js
--rw-r--r--   0 lucjean    (501) staff       (20)        0 2019-08-29 13:07:40.000000 coop_html_editor-1.3.1/coop_html_editor/static/aloha.0.23.26/plugins/extra/linkbrowser/README
-drwxr-xr-x   0 lucjean    (501) staff       (20)        0 2019-08-30 10:39:35.000000 coop_html_editor-1.3.1/coop_html_editor/static/aloha.0.23.26/plugins/extra/linkbrowser/img/
-drwxr-xr-x   0 lucjean    (501) staff       (20)        0 2019-08-30 10:39:52.000000 coop_html_editor-1.3.1/coop_html_editor/static/aloha.0.23.26/plugins/extra/linkbrowser/img/flags/
--rw-r--r--   0 lucjean    (501) staff       (20)      410 2019-08-29 13:07:41.000000 coop_html_editor-1.3.1/coop_html_editor/static/aloha.0.23.26/plugins/extra/linkbrowser/img/flags/tg.png
--rw-r--r--   0 lucjean    (501) staff       (20)      394 2019-08-29 13:07:41.000000 coop_html_editor-1.3.1/coop_html_editor/static/aloha.0.23.26/plugins/extra/linkbrowser/img/flags/me.png
--rw-r--r--   0 lucjean    (501) staff       (20)      415 2019-08-29 13:07:41.000000 coop_html_editor-1.3.1/coop_html_editor/static/aloha.0.23.26/plugins/extra/linkbrowser/img/flags/la.png
--rw-r--r--   0 lucjean    (501) staff       (20)      408 2019-08-29 13:07:41.000000 coop_html_editor-1.3.1/coop_html_editor/static/aloha.0.23.26/plugins/extra/linkbrowser/img/flags/mr.png
--rw-r--r--   0 lucjean    (501) staff       (20)      372 2019-08-29 13:07:41.000000 coop_html_editor-1.3.1/coop_html_editor/static/aloha.0.23.26/plugins/extra/linkbrowser/img/flags/ni.png
--rw-r--r--   0 lucjean    (501) staff       (20)      339 2019-08-29 13:07:41.000000 coop_html_editor-1.3.1/coop_html_editor/static/aloha.0.23.26/plugins/extra/linkbrowser/img/flags/lv.png
--rw-r--r--   0 lucjean    (501) staff       (20)      339 2019-08-29 13:07:41.000000 coop_html_editor-1.3.1/coop_html_editor/static/aloha.0.23.26/plugins/extra/linkbrowser/img/flags/om.png
--rw-r--r--   0 lucjean    (501) staff       (20)      420 2019-08-29 13:07:40.000000 coop_html_editor-1.3.1/coop_html_editor/static/aloha.0.23.26/plugins/extra/linkbrowser/img/flags/af.png
--rw-r--r--   0 lucjean    (501) staff       (20)      337 2019-08-29 13:07:40.000000 coop_html_editor-1.3.1/coop_html_editor/static/aloha.0.23.26/plugins/extra/linkbrowser/img/flags/cy.png
--rw-r--r--   0 lucjean    (501) staff       (20)      311 2019-08-29 13:07:40.000000 coop_html_editor-1.3.1/coop_html_editor/static/aloha.0.23.26/plugins/extra/linkbrowser/img/flags/bj.png
--rw-r--r--   0 lucjean    (501) staff       (20)      349 2019-08-29 13:07:40.000000 coop_html_editor-1.3.1/coop_html_editor/static/aloha.0.23.26/plugins/extra/linkbrowser/img/flags/cn.png
--rw-r--r--   0 lucjean    (501) staff       (20)      330 2019-08-29 13:07:40.000000 coop_html_editor-1.3.1/coop_html_editor/static/aloha.0.23.26/plugins/extra/linkbrowser/img/flags/co.png
--rw-r--r--   0 lucjean    (501) staff       (20)      498 2019-08-29 13:07:40.000000 coop_html_editor-1.3.1/coop_html_editor/static/aloha.0.23.26/plugins/extra/linkbrowser/img/flags/cx.png
--rw-r--r--   0 lucjean    (501) staff       (20)      456 2019-08-29 13:07:40.000000 coop_html_editor-1.3.1/coop_html_editor/static/aloha.0.23.26/plugins/extra/linkbrowser/img/flags/ag.png
--rw-r--r--   0 lucjean    (501) staff       (20)      497 2019-08-29 13:07:41.000000 coop_html_editor-1.3.1/coop_html_editor/static/aloha.0.23.26/plugins/extra/linkbrowser/img/flags/ms.png
--rw-r--r--   0 lucjean    (501) staff       (20)      404 2019-08-29 13:07:41.000000 coop_html_editor-1.3.1/coop_html_editor/static/aloha.0.23.26/plugins/extra/linkbrowser/img/flags/md.png
--rw-r--r--   0 lucjean    (501) staff       (20)      359 2019-08-29 13:07:41.000000 coop_html_editor-1.3.1/coop_html_editor/static/aloha.0.23.26/plugins/extra/linkbrowser/img/flags/zm.png
--rw-r--r--   0 lucjean    (501) staff       (20)      324 2019-08-29 13:07:41.000000 coop_html_editor-1.3.1/coop_html_editor/static/aloha.0.23.26/plugins/extra/linkbrowser/img/flags/vn.png
--rw-r--r--   0 lucjean    (501) staff       (20)      399 2019-08-29 13:07:41.000000 coop_html_editor-1.3.1/coop_html_editor/static/aloha.0.23.26/plugins/extra/linkbrowser/img/flags/tf.png
--rw-r--r--   0 lucjean    (501) staff       (20)      378 2019-08-29 13:07:41.000000 coop_html_editor-1.3.1/coop_html_editor/static/aloha.0.23.26/plugins/extra/linkbrowser/img/flags/td.png
--rw-r--r--   0 lucjean    (501) staff       (20)      456 2019-08-29 13:07:41.000000 coop_html_editor-1.3.1/coop_html_editor/static/aloha.0.23.26/plugins/extra/linkbrowser/img/flags/yt.png
--rw-r--r--   0 lucjean    (501) staff       (20)      393 2019-08-29 13:07:41.000000 coop_html_editor-1.3.1/coop_html_editor/static/aloha.0.23.26/plugins/extra/linkbrowser/img/flags/lb.png
--rw-r--r--   0 lucjean    (501) staff       (20)      338 2019-08-29 13:07:41.000000 coop_html_editor-1.3.1/coop_html_editor/static/aloha.0.23.26/plugins/extra/linkbrowser/img/flags/lu.png
--rw-r--r--   0 lucjean    (501) staff       (20)      541 2019-08-29 13:07:41.000000 coop_html_editor-1.3.1/coop_html_editor/static/aloha.0.23.26/plugins/extra/linkbrowser/img/flags/mq.png
--rw-r--r--   0 lucjean    (501) staff       (20)      367 2019-08-29 13:07:40.000000 coop_html_editor-1.3.1/coop_html_editor/static/aloha.0.23.26/plugins/extra/linkbrowser/img/flags/cz.png
--rw-r--r--   0 lucjean    (501) staff       (20)      277 2019-08-29 13:07:40.000000 coop_html_editor-1.3.1/coop_html_editor/static/aloha.0.23.26/plugins/extra/linkbrowser/img/flags/ae.png
--rw-r--r--   0 lucjean    (501) staff       (20)      347 2019-08-29 13:07:40.000000 coop_html_editor-1.3.1/coop_html_editor/static/aloha.0.23.26/plugins/extra/linkbrowser/img/flags/cm.png
--rw-r--r--   0 lucjean    (501) staff       (20)      350 2019-08-29 13:07:40.000000 coop_html_editor-1.3.1/coop_html_editor/static/aloha.0.23.26/plugins/extra/linkbrowser/img/flags/fam.png
--rw-r--r--   0 lucjean    (501) staff       (20)      566 2019-08-29 13:07:40.000000 coop_html_editor-1.3.1/coop_html_editor/static/aloha.0.23.26/plugins/extra/linkbrowser/img/flags/bi.png
--rw-r--r--   0 lucjean    (501) staff       (20)      367 2019-08-29 13:07:40.000000 coop_html_editor-1.3.1/coop_html_editor/static/aloha.0.23.26/plugins/extra/linkbrowser/img/flags/ar.png
--rw-r--r--   0 lucjean    (501) staff       (20)      540 2019-08-29 13:07:40.000000 coop_html_editor-1.3.1/coop_html_editor/static/aloha.0.23.26/plugins/extra/linkbrowser/img/flags/as.png
--rw-r--r--   0 lucjean    (501) staff       (20)      345 2019-08-29 13:07:40.000000 coop_html_editor-1.3.1/coop_html_editor/static/aloha.0.23.26/plugins/extra/linkbrowser/img/flags/bh.png
--rw-r--r--   0 lucjean    (501) staff       (20)      324 2019-08-29 13:07:40.000000 coop_html_editor-1.3.1/coop_html_editor/static/aloha.0.23.26/plugins/extra/linkbrowser/img/flags/cl.png
--rw-r--r--   0 lucjean    (501) staff       (20)      454 2019-08-29 13:07:40.000000 coop_html_editor-1.3.1/coop_html_editor/static/aloha.0.23.26/plugins/extra/linkbrowser/img/flags/ad.png
--rw-r--r--   0 lucjean    (501) staff       (20)      481 2019-08-29 13:07:41.000000 coop_html_editor-1.3.1/coop_html_editor/static/aloha.0.23.26/plugins/extra/linkbrowser/img/flags/mp.png
--rw-r--r--   0 lucjean    (501) staff       (20)      345 2019-08-29 13:07:41.000000 coop_html_editor-1.3.1/coop_html_editor/static/aloha.0.23.26/plugins/extra/linkbrowser/img/flags/lt.png
--rw-r--r--   0 lucjean    (501) staff       (20)      313 2019-08-29 13:07:41.000000 coop_html_editor-1.3.1/coop_html_editor/static/aloha.0.23.26/plugins/extra/linkbrowser/img/flags/mg.png
--rw-r--r--   0 lucjean    (501) staff       (20)      462 2019-08-29 13:07:41.000000 coop_html_editor-1.3.1/coop_html_editor/static/aloha.0.23.26/plugins/extra/linkbrowser/img/flags/lc.png
--rw-r--r--   0 lucjean    (501) staff       (20)      366 2019-08-29 13:07:41.000000 coop_html_editor-1.3.1/coop_html_editor/static/aloha.0.23.26/plugins/extra/linkbrowser/img/flags/tr.png
--rw-r--r--   0 lucjean    (501) staff       (20)      304 2019-08-29 13:07:41.000000 coop_html_editor-1.3.1/coop_html_editor/static/aloha.0.23.26/plugins/extra/linkbrowser/img/flags/ua.png
--rw-r--r--   0 lucjean    (501) staff       (20)      554 2019-08-29 13:07:41.000000 coop_html_editor-1.3.1/coop_html_editor/static/aloha.0.23.26/plugins/extra/linkbrowser/img/flags/scotland.png
--rw-r--r--   0 lucjean    (501) staff       (20)      443 2019-08-29 13:07:41.000000 coop_html_editor-1.3.1/coop_html_editor/static/aloha.0.23.26/plugins/extra/linkbrowser/img/flags/tv.png
--rw-r--r--   0 lucjean    (501) staff       (20)      523 2019-08-29 13:07:41.000000 coop_html_editor-1.3.1/coop_html_editor/static/aloha.0.23.26/plugins/extra/linkbrowser/img/flags/vi.png
--rw-r--r--   0 lucjean    (501) staff       (20)      296 2019-08-29 13:07:41.000000 coop_html_editor-1.3.1/coop_html_editor/static/aloha.0.23.26/plugins/extra/linkbrowser/img/flags/mt.png
--rw-r--r--   0 lucjean    (501) staff       (20)      397 2019-08-29 13:07:41.000000 coop_html_editor-1.3.1/coop_html_editor/static/aloha.0.23.26/plugins/extra/linkbrowser/img/flags/no.png
--rw-r--r--   0 lucjean    (501) staff       (20)      254 2019-08-29 13:07:41.000000 coop_html_editor-1.3.1/coop_html_editor/static/aloha.0.23.26/plugins/extra/linkbrowser/img/flags/mc.png
--rw-r--r--   0 lucjean    (501) staff       (20)      239 2019-08-29 13:07:40.000000 coop_html_editor-1.3.1/coop_html_editor/static/aloha.0.23.26/plugins/extra/linkbrowser/img/flags/ch.png
--rw-r--r--   0 lucjean    (501) staff       (20)      393 2019-08-29 13:07:40.000000 coop_html_editor-1.3.1/coop_html_editor/static/aloha.0.23.26/plugins/extra/linkbrowser/img/flags/aw.png
--rw-r--r--   0 lucjean    (501) staff       (20)      476 2019-08-29 13:07:40.000000 coop_html_editor-1.3.1/coop_html_editor/static/aloha.0.23.26/plugins/extra/linkbrowser/img/flags/bz.png
--rw-r--r--   0 lucjean    (501) staff       (20)      499 2019-08-29 13:07:40.000000 coop_html_editor-1.3.1/coop_html_editor/static/aloha.0.23.26/plugins/extra/linkbrowser/img/flags/bm.png
--rw-r--r--   0 lucjean    (501) staff       (20)      306 2019-08-29 13:07:40.000000 coop_html_editor-1.3.1/coop_html_editor/static/aloha.0.23.26/plugins/extra/linkbrowser/img/flags/ci.png
--rw-r--r--   0 lucjean    (501) staff       (20)      360 2019-08-29 13:07:41.000000 coop_html_editor-1.3.1/coop_html_editor/static/aloha.0.23.26/plugins/extra/linkbrowser/img/flags/mu.png
--rw-r--r--   0 lucjean    (501) staff       (20)      492 2019-08-29 13:07:41.000000 coop_html_editor-1.3.1/coop_html_editor/static/aloha.0.23.26/plugins/extra/linkbrowser/img/flags/us.png
--rw-r--r--   0 lucjean    (501) staff       (20)      330 2019-08-29 13:07:41.000000 coop_html_editor-1.3.1/coop_html_editor/static/aloha.0.23.26/plugins/extra/linkbrowser/img/flags/tw.png
--rw-r--r--   0 lucjean    (501) staff       (20)      302 2019-08-29 13:07:41.000000 coop_html_editor-1.3.1/coop_html_editor/static/aloha.0.23.26/plugins/extra/linkbrowser/img/flags/ye.png
--rw-r--r--   0 lucjean    (501) staff       (20)      365 2019-08-29 13:07:41.000000 coop_html_editor-1.3.1/coop_html_editor/static/aloha.0.23.26/plugins/extra/linkbrowser/img/flags/mw.png
--rw-r--r--   0 lucjean    (501) staff       (20)      310 2019-08-29 13:07:41.000000 coop_html_editor-1.3.1/coop_html_editor/static/aloha.0.23.26/plugins/extra/linkbrowser/img/flags/nl.png
--rw-r--r--   0 lucjean    (501) staff       (20)      500 2019-08-29 13:07:41.000000 coop_html_editor-1.3.1/coop_html_editor/static/aloha.0.23.26/plugins/extra/linkbrowser/img/flags/ls.png
--rw-r--r--   0 lucjean    (501) staff       (20)      341 2019-08-29 13:07:40.000000 coop_html_editor-1.3.1/coop_html_editor/static/aloha.0.23.26/plugins/extra/linkbrowser/img/flags/bo.png
--rw-r--r--   0 lucjean    (501) staff       (20)      290 2019-08-29 13:07:40.000000 coop_html_editor-1.3.1/coop_html_editor/static/aloha.0.23.26/plugins/extra/linkbrowser/img/flags/at.png
--rw-r--r--   0 lucjean    (501) staff       (20)      495 2019-08-29 13:07:40.000000 coop_html_editor-1.3.1/coop_html_editor/static/aloha.0.23.26/plugins/extra/linkbrowser/img/flags/ck.png
--rw-r--r--   0 lucjean    (501) staff       (20)      382 2019-08-29 13:07:40.000000 coop_html_editor-1.3.1/coop_html_editor/static/aloha.0.23.26/plugins/extra/linkbrowser/img/flags/by.png
--rw-r--r--   0 lucjean    (501) staff       (20)      580 2019-08-29 13:07:40.000000 coop_html_editor-1.3.1/coop_html_editor/static/aloha.0.23.26/plugins/extra/linkbrowser/img/flags/au.png
--rw-r--r--   0 lucjean    (501) staff       (20)      502 2019-08-29 13:07:40.000000 coop_html_editor-1.3.1/coop_html_editor/static/aloha.0.23.26/plugins/extra/linkbrowser/img/flags/bn.png
--rw-r--r--   0 lucjean    (501) staff       (20)      293 2019-08-29 13:07:41.000000 coop_html_editor-1.3.1/coop_html_editor/static/aloha.0.23.26/plugins/extra/linkbrowser/img/flags/ma.png
--rw-r--r--   0 lucjean    (501) staff       (20)      529 2019-08-29 13:07:41.000000 coop_html_editor-1.3.1/coop_html_editor/static/aloha.0.23.26/plugins/extra/linkbrowser/img/flags/nz.png
--rw-r--r--   0 lucjean    (501) staff       (20)      365 2019-08-29 13:07:41.000000 coop_html_editor-1.3.1/coop_html_editor/static/aloha.0.23.26/plugins/extra/linkbrowser/img/flags/lr.png
--rw-r--r--   0 lucjean    (501) staff       (20)      391 2019-08-29 13:07:41.000000 coop_html_editor-1.3.1/coop_html_editor/static/aloha.0.23.26/plugins/extra/linkbrowser/img/flags/mv.png
--rw-r--r--   0 lucjean    (501) staff       (20)      509 2019-08-29 13:07:41.000000 coop_html_editor-1.3.1/coop_html_editor/static/aloha.0.23.26/plugins/extra/linkbrowser/img/flags/tc.png
--rw-r--r--   0 lucjean    (501) staff       (20)      388 2019-08-29 13:07:41.000000 coop_html_editor-1.3.1/coop_html_editor/static/aloha.0.23.26/plugins/extra/linkbrowser/img/flags/ug.png
--rw-r--r--   0 lucjean    (501) staff       (20)      486 2019-08-29 13:07:41.000000 coop_html_editor-1.3.1/coop_html_editor/static/aloha.0.23.26/plugins/extra/linkbrowser/img/flags/tt.png
--rw-r--r--   0 lucjean    (501) staff       (20)      243 2019-08-29 13:07:41.000000 coop_html_editor-1.3.1/coop_html_editor/static/aloha.0.23.26/plugins/extra/linkbrowser/img/flags/pl.png
--rw-r--r--   0 lucjean    (501) staff       (20)      376 2019-08-29 13:07:41.000000 coop_html_editor-1.3.1/coop_html_editor/static/aloha.0.23.26/plugins/extra/linkbrowser/img/flags/rs.png
--rw-r--r--   0 lucjean    (501) staff       (20)      377 2019-08-29 13:07:40.000000 coop_html_editor-1.3.1/coop_html_editor/static/aloha.0.23.26/plugins/extra/linkbrowser/img/flags/in.png
--rw-r--r--   0 lucjean    (501) staff       (20)      493 2019-08-29 13:07:40.000000 coop_html_editor-1.3.1/coop_html_editor/static/aloha.0.23.26/plugins/extra/linkbrowser/img/flags/ge.png
--rw-r--r--   0 lucjean    (501) staff       (20)      391 2019-08-29 13:07:40.000000 coop_html_editor-1.3.1/coop_html_editor/static/aloha.0.23.26/plugins/extra/linkbrowser/img/flags/gr.png
--rw-r--r--   0 lucjean    (501) staff       (20)      522 2019-08-29 13:07:40.000000 coop_html_editor-1.3.1/coop_html_editor/static/aloha.0.23.26/plugins/extra/linkbrowser/img/flags/gs.png
--rw-r--r--   0 lucjean    (501) staff       (20)      461 2019-08-29 13:07:40.000000 coop_html_editor-1.3.1/coop_html_editor/static/aloha.0.23.26/plugins/extra/linkbrowser/img/flags/gd.png
--rw-r--r--   0 lucjean    (501) staff       (20)      575 2019-08-29 13:07:40.000000 coop_html_editor-1.3.1/coop_html_editor/static/aloha.0.23.26/plugins/extra/linkbrowser/img/flags/io.png
--rw-r--r--   0 lucjean    (501) staff       (20)      393 2019-08-29 13:07:40.000000 coop_html_editor-1.3.1/coop_html_editor/static/aloha.0.23.26/plugins/extra/linkbrowser/img/flags/hk.png
--rw-r--r--   0 lucjean    (501) staff       (20)      424 2019-08-29 13:07:40.000000 coop_html_editor-1.3.1/coop_html_editor/static/aloha.0.23.26/plugins/extra/linkbrowser/img/flags/kp.png
--rw-r--r--   0 lucjean    (501) staff       (20)      354 2019-08-29 13:07:40.000000 coop_html_editor-1.3.1/coop_html_editor/static/aloha.0.23.26/plugins/extra/linkbrowser/img/flags/kg.png
--rw-r--r--   0 lucjean    (501) staff       (20)      572 2019-08-29 13:07:41.000000 coop_html_editor-1.3.1/coop_html_editor/static/aloha.0.23.26/plugins/extra/linkbrowser/img/flags/pm.png
--rw-r--r--   0 lucjean    (501) staff       (20)      373 2019-08-29 13:07:41.000000 coop_html_editor-1.3.1/coop_html_editor/static/aloha.0.23.26/plugins/extra/linkbrowser/img/flags/sv.png
--rw-r--r--   0 lucjean    (501) staff       (20)      369 2019-08-29 13:07:41.000000 coop_html_editor-1.3.1/coop_html_editor/static/aloha.0.23.26/plugins/extra/linkbrowser/img/flags/re.png
--rw-r--r--   0 lucjean    (501) staff       (20)      428 2019-08-29 13:07:41.000000 coop_html_editor-1.3.1/coop_html_editor/static/aloha.0.23.26/plugins/extra/linkbrowser/img/flags/sa.png
--rw-r--r--   0 lucjean    (501) staff       (20)      481 2019-08-29 13:07:41.000000 coop_html_editor-1.3.1/coop_html_editor/static/aloha.0.23.26/plugins/extra/linkbrowser/img/flags/sc.png
--rw-r--r--   0 lucjean    (501) staff       (20)      429 2019-08-29 13:07:41.000000 coop_html_editor-1.3.1/coop_html_editor/static/aloha.0.23.26/plugins/extra/linkbrowser/img/flags/st.png
--rw-r--r--   0 lucjean    (501) staff       (20)      435 2019-08-29 13:07:40.000000 coop_html_editor-1.3.1/coop_html_editor/static/aloha.0.23.26/plugins/extra/linkbrowser/img/flags/ke.png
--rw-r--r--   0 lucjean    (501) staff       (20)      507 2019-08-29 13:07:41.000000 coop_html_editor-1.3.1/coop_html_editor/static/aloha.0.23.26/plugins/extra/linkbrowser/img/flags/kr.png
--rw-r--r--   0 lucjean    (501) staff       (20)      369 2019-08-29 13:07:40.000000 coop_html_editor-1.3.1/coop_html_editor/static/aloha.0.23.26/plugins/extra/linkbrowser/img/flags/gf.png
--rw-r--r--   0 lucjean    (501) staff       (20)      378 2019-08-29 13:07:40.000000 coop_html_editor-1.3.1/coop_html_editor/static/aloha.0.23.26/plugins/extra/linkbrowser/img/flags/en.png
--rw-r--r--   0 lucjean    (501) staff       (20)      430 2019-08-29 13:07:40.000000 coop_html_editor-1.3.1/coop_html_editor/static/aloha.0.23.26/plugins/extra/linkbrowser/img/flags/dj.png
--rw-r--r--   0 lucjean    (501) staff       (20)      405 2019-08-29 13:07:40.000000 coop_html_editor-1.3.1/coop_html_editor/static/aloha.0.23.26/plugins/extra/linkbrowser/img/flags/gq.png
--rw-r--r--   0 lucjean    (501) staff       (20)      353 2019-08-29 13:07:40.000000 coop_html_editor-1.3.1/coop_html_editor/static/aloha.0.23.26/plugins/extra/linkbrowser/img/flags/gp.png
--rw-r--r--   0 lucjean    (501) staff       (20)      352 2019-08-29 13:07:40.000000 coop_html_editor-1.3.1/coop_html_editor/static/aloha.0.23.26/plugins/extra/linkbrowser/img/flags/dk.png
--rw-r--r--   0 lucjean    (501) staff       (20)      326 2019-08-29 13:07:40.000000 coop_html_editor-1.3.1/coop_html_editor/static/aloha.0.23.26/plugins/extra/linkbrowser/img/flags/il.png
--rw-r--r--   0 lucjean    (501) staff       (20)      547 2019-08-29 13:07:41.000000 coop_html_editor-1.3.1/coop_html_editor/static/aloha.0.23.26/plugins/extra/linkbrowser/img/flags/pn.png
--rw-r--r--   0 lucjean    (501) staff       (20)      520 2019-08-29 13:07:41.000000 coop_html_editor-1.3.1/coop_html_editor/static/aloha.0.23.26/plugins/extra/linkbrowser/img/flags/sb.png
--rw-r--r--   0 lucjean    (501) staff       (20)      344 2019-08-29 13:07:41.000000 coop_html_editor-1.3.1/coop_html_editor/static/aloha.0.23.26/plugins/extra/linkbrowser/img/flags/py.png
--rw-r--r--   0 lucjean    (501) staff       (20)      299 2019-08-29 13:07:41.000000 coop_html_editor-1.3.1/coop_html_editor/static/aloha.0.23.26/plugins/extra/linkbrowser/img/flags/ru.png
--rw-r--r--   0 lucjean    (501) staff       (20)      351 2019-08-29 13:07:41.000000 coop_html_editor-1.3.1/coop_html_editor/static/aloha.0.23.26/plugins/extra/linkbrowser/img/flags/kw.png
--rw-r--r--   0 lucjean    (501) staff       (20)      368 2019-08-29 13:07:40.000000 coop_html_editor-1.3.1/coop_html_editor/static/aloha.0.23.26/plugins/extra/linkbrowser/img/flags/do.png
--rw-r--r--   0 lucjean    (501) staff       (20)      333 2019-08-29 13:07:40.000000 coop_html_editor-1.3.1/coop_html_editor/static/aloha.0.23.26/plugins/extra/linkbrowser/img/flags/gt.png
--rw-r--r--   0 lucjean    (501) staff       (20)      545 2019-08-29 13:07:40.000000 coop_html_editor-1.3.1/coop_html_editor/static/aloha.0.23.26/plugins/extra/linkbrowser/img/flags/gb.png
--rw-r--r--   0 lucjean    (501) staff       (20)      384 2019-08-29 13:07:40.000000 coop_html_editor-1.3.1/coop_html_editor/static/aloha.0.23.26/plugins/extra/linkbrowser/img/flags/gu.png
--rw-r--r--   0 lucjean    (501) staff       (20)      580 2019-08-29 13:07:40.000000 coop_html_editor-1.3.1/coop_html_editor/static/aloha.0.23.26/plugins/extra/linkbrowser/img/flags/hm.png
--rw-r--r--   0 lucjean    (501) staff       (20)      350 2019-08-29 13:07:41.000000 coop_html_editor-1.3.1/coop_html_editor/static/aloha.0.23.26/plugins/extra/linkbrowser/img/flags/sg.png
--rw-r--r--   0 lucjean    (501) staff       (20)      448 2019-08-29 13:07:41.000000 coop_html_editor-1.3.1/coop_html_editor/static/aloha.0.23.26/plugins/extra/linkbrowser/img/flags/pk.png
--rw-r--r--   0 lucjean    (501) staff       (20)      370 2019-08-29 13:07:41.000000 coop_html_editor-1.3.1/coop_html_editor/static/aloha.0.23.26/plugins/extra/linkbrowser/img/flags/sr.png
--rw-r--r--   0 lucjean    (501) staff       (20)      389 2019-08-29 13:07:41.000000 coop_html_editor-1.3.1/coop_html_editor/static/aloha.0.23.26/plugins/extra/linkbrowser/img/flags/se.png
--rw-r--r--   0 lucjean    (501) staff       (20)      307 2019-08-29 13:07:40.000000 coop_html_editor-1.3.1/coop_html_editor/static/aloha.0.23.26/plugins/extra/linkbrowser/img/flags/jp.png
--rw-r--r--   0 lucjean    (501) staff       (20)      346 2019-08-29 13:07:40.000000 coop_html_editor-1.3.1/coop_html_editor/static/aloha.0.23.26/plugins/extra/linkbrowser/img/flags/gw.png
--rw-r--r--   0 lucjean    (501) staff       (20)      388 2019-08-29 13:07:40.000000 coop_html_editor-1.3.1/coop_html_editor/static/aloha.0.23.26/plugins/extra/linkbrowser/img/flags/eh.png
--rw-r--r--   0 lucjean    (501) staff       (20)      454 2019-08-29 13:07:40.000000 coop_html_editor-1.3.1/coop_html_editor/static/aloha.0.23.26/plugins/extra/linkbrowser/img/flags/dz.png
--rw-r--r--   0 lucjean    (501) staff       (20)      342 2019-08-29 13:07:40.000000 coop_html_editor-1.3.1/coop_html_editor/static/aloha.0.23.26/plugins/extra/linkbrowser/img/flags/ga.png
--rw-r--r--   0 lucjean    (501) staff       (20)      369 2019-08-29 13:07:40.000000 coop_html_editor-1.3.1/coop_html_editor/static/aloha.0.23.26/plugins/extra/linkbrowser/img/flags/fr.png
--rw-r--r--   0 lucjean    (501) staff       (20)      508 2019-08-29 13:07:40.000000 coop_html_editor-1.3.1/coop_html_editor/static/aloha.0.23.26/plugins/extra/linkbrowser/img/flags/dm.png
--rw-r--r--   0 lucjean    (501) staff       (20)      411 2019-08-29 13:07:40.000000 coop_html_editor-1.3.1/coop_html_editor/static/aloha.0.23.26/plugins/extra/linkbrowser/img/flags/hn.png
--rw-r--r--   0 lucjean    (501) staff       (20)      364 2019-08-29 13:07:41.000000 coop_html_editor-1.3.1/coop_html_editor/static/aloha.0.23.26/plugins/extra/linkbrowser/img/flags/sd.png
--rw-r--r--   0 lucjean    (501) staff       (20)      382 2019-08-29 13:07:41.000000 coop_html_editor-1.3.1/coop_html_editor/static/aloha.0.23.26/plugins/extra/linkbrowser/img/flags/rw.png
--rw-r--r--   0 lucjean    (501) staff       (20)      416 2019-08-29 13:07:41.000000 coop_html_editor-1.3.1/coop_html_editor/static/aloha.0.23.26/plugins/extra/linkbrowser/img/flags/ph.png
--rw-r--r--   0 lucjean    (501) staff       (20)      343 2019-08-29 13:07:41.000000 coop_html_editor-1.3.1/coop_html_editor/static/aloha.0.23.26/plugins/extra/linkbrowser/img/flags/qa.png
--rw-r--r--   0 lucjean    (501) staff       (20)      264 2019-08-29 13:07:41.000000 coop_html_editor-1.3.1/coop_html_editor/static/aloha.0.23.26/plugins/extra/linkbrowser/img/flags/pe.png
--rw-r--r--   0 lucjean    (501) staff       (20)      445 2019-08-29 13:07:41.000000 coop_html_editor-1.3.1/coop_html_editor/static/aloha.0.23.26/plugins/extra/linkbrowser/img/flags/pr.png
--rw-r--r--   0 lucjean    (501) staff       (20)      383 2019-08-29 13:07:41.000000 coop_html_editor-1.3.1/coop_html_editor/static/aloha.0.23.26/plugins/extra/linkbrowser/img/flags/si.png
--rw-r--r--   0 lucjean    (501) staff       (20)      327 2019-08-29 13:07:40.000000 coop_html_editor-1.3.1/coop_html_editor/static/aloha.0.23.26/plugins/extra/linkbrowser/img/flags/ht.png
--rw-r--r--   0 lucjean    (501) staff       (20)      344 2019-08-29 13:07:40.000000 coop_html_editor-1.3.1/coop_html_editor/static/aloha.0.23.26/plugins/extra/linkbrowser/img/flags/es.png
--rw-r--r--   0 lucjean    (501) staff       (20)      351 2019-08-29 13:07:40.000000 coop_html_editor-1.3.1/coop_html_editor/static/aloha.0.23.26/plugins/extra/linkbrowser/img/flags/gl.png
--rw-r--r--   0 lucjean    (501) staff       (20)      363 2019-08-29 13:07:40.000000 coop_html_editor-1.3.1/coop_html_editor/static/aloha.0.23.26/plugins/extra/linkbrowser/img/flags/gm.png
--rw-r--r--   0 lucjean    (501) staff       (20)      497 2019-08-29 13:07:40.000000 coop_html_editor-1.3.1/coop_html_editor/static/aloha.0.23.26/plugins/extra/linkbrowser/img/flags/er.png
--rw-r--r--   0 lucjean    (501) staff       (20)      368 2019-08-29 13:07:40.000000 coop_html_editor-1.3.1/coop_html_editor/static/aloha.0.23.26/plugins/extra/linkbrowser/img/flags/fi.png
--rw-r--r--   0 lucjean    (501) staff       (20)      297 2019-08-29 13:07:40.000000 coop_html_editor-1.3.1/coop_html_editor/static/aloha.0.23.26/plugins/extra/linkbrowser/img/flags/ee.png
--rw-r--r--   0 lucjean    (501) staff       (20)      480 2019-08-29 13:07:40.000000 coop_html_editor-1.3.1/coop_html_editor/static/aloha.0.23.26/plugins/extra/linkbrowser/img/flags/kn.png
--rw-r--r--   0 lucjean    (501) staff       (20)      293 2019-08-29 13:07:40.000000 coop_html_editor-1.3.1/coop_html_editor/static/aloha.0.23.26/plugins/extra/linkbrowser/img/flags/hu.png
--rw-r--r--   0 lucjean    (501) staff       (20)      403 2019-08-29 13:07:40.000000 coop_html_editor-1.3.1/coop_html_editor/static/aloha.0.23.26/plugins/extra/linkbrowser/img/flags/iq.png
--rw-r--r--   0 lucjean    (501) staff       (20)      532 2019-08-29 13:07:41.000000 coop_html_editor-1.3.1/coop_html_editor/static/aloha.0.23.26/plugins/extra/linkbrowser/img/flags/ky.png
--rw-r--r--   0 lucjean    (501) staff       (20)      524 2019-08-29 13:07:41.000000 coop_html_editor-1.3.1/coop_html_editor/static/aloha.0.23.26/plugins/extra/linkbrowser/img/flags/sh.png
--rw-r--r--   0 lucjean    (501) staff       (20)      348 2019-08-29 13:07:41.000000 coop_html_editor-1.3.1/coop_html_editor/static/aloha.0.23.26/plugins/extra/linkbrowser/img/flags/ps.png
--rw-r--r--   0 lucjean    (501) staff       (20)      379 2019-08-29 13:07:41.000000 coop_html_editor-1.3.1/coop_html_editor/static/aloha.0.23.26/plugins/extra/linkbrowser/img/flags/pf.png
--rw-r--r--   0 lucjean    (501) staff       (20)      397 2019-08-29 13:07:41.000000 coop_html_editor-1.3.1/coop_html_editor/static/aloha.0.23.26/plugins/extra/linkbrowser/img/flags/sj.png
--rw-r--r--   0 lucjean    (501) staff       (20)      301 2019-08-29 13:07:40.000000 coop_html_editor-1.3.1/coop_html_editor/static/aloha.0.23.26/plugins/extra/linkbrowser/img/flags/id.png
--rw-r--r--   0 lucjean    (501) staff       (20)      410 2019-08-29 13:07:40.000000 coop_html_editor-1.3.1/coop_html_editor/static/aloha.0.23.26/plugins/extra/linkbrowser/img/flags/is.png
--rw-r--r--   0 lucjean    (501) staff       (20)      348 2019-08-29 13:07:40.000000 coop_html_editor-1.3.1/coop_html_editor/static/aloha.0.23.26/plugins/extra/linkbrowser/img/flags/eg.png
--rw-r--r--   0 lucjean    (501) staff       (20)      526 2019-08-29 13:07:40.000000 coop_html_editor-1.3.1/coop_html_editor/static/aloha.0.23.26/plugins/extra/linkbrowser/img/flags/fk.png
--rw-r--r--   0 lucjean    (501) staff       (20)      517 2019-08-29 13:07:40.000000 coop_html_editor-1.3.1/coop_html_editor/static/aloha.0.23.26/plugins/extra/linkbrowser/img/flags/fj.png
--rw-r--r--   0 lucjean    (501) staff       (20)      319 2019-08-29 13:07:40.000000 coop_html_editor-1.3.1/coop_html_editor/static/aloha.0.23.26/plugins/extra/linkbrowser/img/flags/gn.png
--rw-r--r--   0 lucjean    (501) staff       (20)      521 2019-08-29 13:07:40.000000 coop_html_editor-1.3.1/coop_html_editor/static/aloha.0.23.26/plugins/extra/linkbrowser/img/flags/gy.png
--rw-r--r--   0 lucjean    (501) staff       (20)      398 2019-08-29 13:07:40.000000 coop_html_editor-1.3.1/coop_html_editor/static/aloha.0.23.26/plugins/extra/linkbrowser/img/flags/ir.png
--rw-r--r--   0 lucjean    (501) staff       (20)      456 2019-08-29 13:07:40.000000 coop_html_editor-1.3.1/coop_html_editor/static/aloha.0.23.26/plugins/extra/linkbrowser/img/flags/km.png
--rw-r--r--   0 lucjean    (501) staff       (20)      333 2019-08-29 13:07:40.000000 coop_html_editor-1.3.1/coop_html_editor/static/aloha.0.23.26/plugins/extra/linkbrowser/img/flags/ie.png
--rw-r--r--   0 lucjean    (501) staff       (20)      459 2019-08-29 13:07:41.000000 coop_html_editor-1.3.1/coop_html_editor/static/aloha.0.23.26/plugins/extra/linkbrowser/img/flags/kz.png
--rw-r--r--   0 lucjean    (501) staff       (20)      333 2019-08-29 13:07:41.000000 coop_html_editor-1.3.1/coop_html_editor/static/aloha.0.23.26/plugins/extra/linkbrowser/img/flags/ro.png
--rw-r--r--   0 lucjean    (501) staff       (20)      439 2019-08-29 13:07:41.000000 coop_html_editor-1.3.1/coop_html_editor/static/aloha.0.23.26/plugins/extra/linkbrowser/img/flags/sk.png
--rw-r--r--   0 lucjean    (501) staff       (20)      438 2019-08-29 13:07:41.000000 coop_html_editor-1.3.1/coop_html_editor/static/aloha.0.23.26/plugins/extra/linkbrowser/img/flags/pg.png
--rw-r--r--   0 lucjean    (501) staff       (20)      407 2019-08-29 13:07:41.000000 coop_html_editor-1.3.1/coop_html_editor/static/aloha.0.23.26/plugins/extra/linkbrowser/img/flags/pt.png
--rw-r--r--   0 lucjean    (501) staff       (20)      376 2019-08-29 13:07:41.000000 coop_html_editor-1.3.1/coop_html_editor/static/aloha.0.23.26/plugins/extra/linkbrowser/img/flags/so.png
--rw-r--r--   0 lucjean    (501) staff       (20)      386 2019-08-29 13:07:40.000000 coop_html_editor-1.3.1/coop_html_editor/static/aloha.0.23.26/plugins/extra/linkbrowser/img/flags/hr.png
--rw-r--r--   0 lucjean    (501) staff       (20)      551 2019-08-29 13:07:40.000000 coop_html_editor-1.3.1/coop_html_editor/static/aloha.0.23.26/plugins/extra/linkbrowser/img/flags/ki.png
--rw-r--r--   0 lucjean    (501) staff       (20)      508 2019-08-29 13:07:40.000000 coop_html_editor-1.3.1/coop_html_editor/static/aloha.0.23.26/plugins/extra/linkbrowser/img/flags/jm.png
--rw-r--r--   0 lucjean    (501) staff       (20)      355 2019-08-29 13:07:40.000000 coop_html_editor-1.3.1/coop_html_editor/static/aloha.0.23.26/plugins/extra/linkbrowser/img/flags/ec.png
--rw-r--r--   0 lucjean    (501) staff       (20)      445 2019-08-29 13:07:40.000000 coop_html_editor-1.3.1/coop_html_editor/static/aloha.0.23.26/plugins/extra/linkbrowser/img/flags/et.png
--rw-r--r--   0 lucjean    (501) staff       (20)      377 2019-08-29 13:07:40.000000 coop_html_editor-1.3.1/coop_html_editor/static/aloha.0.23.26/plugins/extra/linkbrowser/img/flags/fo.png
--rw-r--r--   0 lucjean    (501) staff       (20)      422 2019-08-29 13:07:40.000000 coop_html_editor-1.3.1/coop_html_editor/static/aloha.0.23.26/plugins/extra/linkbrowser/img/flags/kh.png
--rw-r--r--   0 lucjean    (501) staff       (20)      322 2019-08-29 13:07:41.000000 coop_html_editor-1.3.1/coop_html_editor/static/aloha.0.23.26/plugins/extra/linkbrowser/img/flags/sy.png
--rw-r--r--   0 lucjean    (501) staff       (20)      356 2019-08-29 13:07:41.000000 coop_html_editor-1.3.1/coop_html_editor/static/aloha.0.23.26/plugins/extra/linkbrowser/img/flags/sn.png
--rw-r--r--   0 lucjean    (501) staff       (20)      424 2019-08-29 13:07:41.000000 coop_html_editor-1.3.1/coop_html_editor/static/aloha.0.23.26/plugins/extra/linkbrowser/img/flags/pw.png
--rw-r--r--   0 lucjean    (501) staff       (20)      321 2019-08-29 13:07:41.000000 coop_html_editor-1.3.1/coop_html_editor/static/aloha.0.23.26/plugins/extra/linkbrowser/img/flags/sl.png
--rw-r--r--   0 lucjean    (501) staff       (20)      409 2019-08-29 13:07:40.000000 coop_html_editor-1.3.1/coop_html_editor/static/aloha.0.23.26/plugins/extra/linkbrowser/img/flags/fm.png
--rw-r--r--   0 lucjean    (501) staff       (20)      369 2019-08-29 13:07:40.000000 coop_html_editor-1.3.1/coop_html_editor/static/aloha.0.23.26/plugins/extra/linkbrowser/img/flags/gi.png
--rw-r--r--   0 lucjean    (501) staff       (20)      364 2019-08-29 13:07:40.000000 coop_html_editor-1.3.1/coop_html_editor/static/aloha.0.23.26/plugins/extra/linkbrowser/img/flags/de.png
--rw-r--r--   0 lucjean    (501) staff       (20)      336 2019-08-29 13:07:40.000000 coop_html_editor-1.3.1/coop_html_editor/static/aloha.0.23.26/plugins/extra/linkbrowser/img/flags/gh.png
--rw-r--r--   0 lucjean    (501) staff       (20)      353 2019-08-29 13:07:40.000000 coop_html_editor-1.3.1/coop_html_editor/static/aloha.0.23.26/plugins/extra/linkbrowser/img/flags/jo.png
--rw-r--r--   0 lucjean    (501) staff       (20)      283 2019-08-29 13:07:40.000000 coop_html_editor-1.3.1/coop_html_editor/static/aloha.0.23.26/plugins/extra/linkbrowser/img/flags/it.png
--rw-r--r--   0 lucjean    (501) staff       (20)      390 2019-08-29 13:07:41.000000 coop_html_editor-1.3.1/coop_html_editor/static/aloha.0.23.26/plugins/extra/linkbrowser/img/flags/pa.png
--rw-r--r--   0 lucjean    (501) staff       (20)      508 2019-08-29 13:07:41.000000 coop_html_editor-1.3.1/coop_html_editor/static/aloha.0.23.26/plugins/extra/linkbrowser/img/flags/sz.png
--rw-r--r--   0 lucjean    (501) staff       (20)      396 2019-08-29 13:07:41.000000 coop_html_editor-1.3.1/coop_html_editor/static/aloha.0.23.26/plugins/extra/linkbrowser/img/flags/sm.png
--rw-r--r--   0 lucjean    (501) staff       (20)      367 2019-08-29 13:07:41.000000 coop_html_editor-1.3.1/coop_html_editor/static/aloha.0.23.26/plugins/extra/linkbrowser/img/flags/tn.png
--rw-r--r--   0 lucjean    (501) staff       (20)      322 2019-08-29 13:07:41.000000 coop_html_editor-1.3.1/coop_html_editor/static/aloha.0.23.26/plugins/extra/linkbrowser/img/flags/ml.png
--rw-r--r--   0 lucjean    (501) staff       (20)      380 2019-08-29 13:07:40.000000 coop_html_editor-1.3.1/coop_html_editor/static/aloha.0.23.26/plugins/extra/linkbrowser/img/flags/cg.png
--rw-r--r--   0 lucjean    (501) staff       (20)      480 2019-08-29 13:07:40.000000 coop_html_editor-1.3.1/coop_html_editor/static/aloha.0.23.26/plugins/extra/linkbrowser/img/flags/ax.png
--rw-r--r--   0 lucjean    (501) staff       (20)      395 2019-08-29 13:07:40.000000 coop_html_editor-1.3.1/coop_html_editor/static/aloha.0.23.26/plugins/extra/linkbrowser/img/flags/ao.png
--rw-r--r--   0 lucjean    (501) staff       (20)      471 2019-08-29 13:07:40.000000 coop_html_editor-1.3.1/coop_html_editor/static/aloha.0.23.26/plugins/extra/linkbrowser/img/flags/bt.png
--rw-r--r--   0 lucjean    (501) staff       (20)      365 2019-08-29 13:07:40.000000 coop_html_editor-1.3.1/coop_html_editor/static/aloha.0.23.26/plugins/extra/linkbrowser/img/flags/an.png
--rw-r--r--   0 lucjean    (501) staff       (20)      403 2019-08-29 13:07:40.000000 coop_html_editor-1.3.1/coop_html_editor/static/aloha.0.23.26/plugins/extra/linkbrowser/img/flags/bb.png
--rw-r--r--   0 lucjean    (501) staff       (20)      456 2019-08-29 13:07:40.000000 coop_html_editor-1.3.1/coop_html_editor/static/aloha.0.23.26/plugins/extra/linkbrowser/img/flags/cf.png
--rw-r--r--   0 lucjean    (501) staff       (20)      336 2019-08-29 13:07:41.000000 coop_html_editor-1.3.1/coop_html_editor/static/aloha.0.23.26/plugins/extra/linkbrowser/img/flags/mm.png
--rw-r--r--   0 lucjean    (501) staff       (20)      399 2019-08-29 13:07:41.000000 coop_html_editor-1.3.1/coop_html_editor/static/aloha.0.23.26/plugins/extra/linkbrowser/img/flags/li.png
--rw-r--r--   0 lucjean    (501) staff       (20)      559 2019-08-29 13:07:41.000000 coop_html_editor-1.3.1/coop_html_editor/static/aloha.0.23.26/plugins/extra/linkbrowser/img/flags/na.png
--rw-r--r--   0 lucjean    (501) staff       (20)      439 2019-08-29 13:07:41.000000 coop_html_editor-1.3.1/coop_html_editor/static/aloha.0.23.26/plugins/extra/linkbrowser/img/flags/mz.png
--rw-r--r--   0 lucjean    (501) staff       (20)      302 2019-08-29 13:07:41.000000 coop_html_editor-1.3.1/coop_html_editor/static/aloha.0.23.26/plugins/extra/linkbrowser/img/flags/to.png
--rw-r--r--   0 lucjean    (501) staff       (20)      510 2019-08-29 13:07:41.000000 coop_html_editor-1.3.1/coop_html_editor/static/aloha.0.23.26/plugins/extra/linkbrowser/img/flags/vg.png
--rw-r--r--   0 lucjean    (501) staff       (20)      412 2019-08-29 13:07:41.000000 coop_html_editor-1.3.1/coop_html_editor/static/aloha.0.23.26/plugins/extra/linkbrowser/img/flags/ve.png
--rw-r--r--   0 lucjean    (501) staff       (20)      514 2019-08-29 13:07:41.000000 coop_html_editor-1.3.1/coop_html_editor/static/aloha.0.23.26/plugins/extra/linkbrowser/img/flags/tz.png
--rw-r--r--   0 lucjean    (501) staff       (20)      456 2019-08-29 13:07:41.000000 coop_html_editor-1.3.1/coop_html_editor/static/aloha.0.23.26/plugins/extra/linkbrowser/img/flags/tm.png
--rw-r--r--   0 lucjean    (501) staff       (20)      424 2019-08-29 13:07:41.000000 coop_html_editor-1.3.1/coop_html_editor/static/aloha.0.23.26/plugins/extra/linkbrowser/img/flags/mx.png
--rw-r--r--   0 lucjean    (501) staff       (20)      470 2019-08-29 13:07:41.000000 coop_html_editor-1.3.1/coop_html_editor/static/aloha.0.23.26/plugins/extra/linkbrowser/img/flags/nc.png
--rw-r--r--   0 lucjean    (501) staff       (20)      456 2019-08-29 13:07:41.000000 coop_html_editor-1.3.1/coop_html_editor/static/aloha.0.23.26/plugins/extra/linkbrowser/img/flags/mo.png
--rw-r--r--   0 lucjean    (501) staff       (20)      464 2019-08-29 13:07:41.000000 coop_html_editor-1.3.1/coop_html_editor/static/aloha.0.23.26/plugins/extra/linkbrowser/img/flags/lk.png
--rw-r--r--   0 lucjean    (501) staff       (20)      477 2019-08-29 13:07:40.000000 coop_html_editor-1.3.1/coop_html_editor/static/aloha.0.23.26/plugins/extra/linkbrowser/img/flags/cd.png
--rw-r--r--   0 lucjean    (501) staff       (20)      434 2019-08-29 13:07:40.000000 coop_html_editor-1.3.1/coop_html_editor/static/aloha.0.23.26/plugins/extra/linkbrowser/img/flags/al.png
--rw-r--r--   0 lucjean    (501) staff       (20)      327 2019-08-29 13:07:40.000000 coop_html_editor-1.3.1/coop_html_editor/static/aloha.0.23.26/plugins/extra/linkbrowser/img/flags/bw.png
--rw-r--r--   0 lucjean    (501) staff       (20)      321 2019-08-29 13:07:40.000000 coop_html_editor-1.3.1/coop_html_editor/static/aloha.0.23.26/plugins/extra/linkbrowser/img/flags/cs.png
--rw-r--r--   0 lucjean    (501) staff       (20)      349 2019-08-29 13:07:40.000000 coop_html_editor-1.3.1/coop_html_editor/static/aloha.0.23.26/plugins/extra/linkbrowser/img/flags/cr.png
--rw-r--r--   0 lucjean    (501) staff       (20)      397 2019-08-29 13:07:40.000000 coop_html_editor-1.3.1/coop_html_editor/static/aloha.0.23.26/plugins/extra/linkbrowser/img/flags/bv.png
--rw-r--r--   0 lucjean    (501) staff       (20)      332 2019-08-29 13:07:40.000000 coop_html_editor-1.3.1/coop_html_editor/static/aloha.0.23.26/plugins/extra/linkbrowser/img/flags/am.png
--rw-r--r--   0 lucjean    (501) staff       (20)      423 2019-08-29 13:07:40.000000 coop_html_editor-1.3.1/coop_html_editor/static/aloha.0.23.26/plugins/extra/linkbrowser/img/flags/az.png
--rw-r--r--   0 lucjean    (501) staff       (20)      471 2019-08-29 13:07:40.000000 coop_html_editor-1.3.1/coop_html_editor/static/aloha.0.23.26/plugins/extra/linkbrowser/img/flags/ba.png
--rw-r--r--   0 lucjean    (501) staff       (20)      343 2019-08-29 13:07:41.000000 coop_html_editor-1.3.1/coop_html_editor/static/aloha.0.23.26/plugins/extra/linkbrowser/img/flags/mn.png
--rw-r--r--   0 lucjean    (501) staff       (20)      468 2019-08-29 13:07:41.000000 coop_html_editor-1.3.1/coop_html_editor/static/aloha.0.23.26/plugins/extra/linkbrowser/img/flags/nu.png
--rw-r--r--   0 lucjean    (501) staff       (20)      464 2019-08-29 13:07:41.000000 coop_html_editor-1.3.1/coop_html_editor/static/aloha.0.23.26/plugins/extra/linkbrowser/img/flags/my.png
--rw-r--r--   0 lucjean    (501) staff       (20)      418 2019-08-29 13:07:40.000000 coop_html_editor-1.3.1/coop_html_editor/static/aloha.0.23.26/plugins/extra/linkbrowser/img/flags/europeanunion.png
--rw-r--r--   0 lucjean    (501) staff       (20)      395 2019-08-29 13:07:41.000000 coop_html_editor-1.3.1/coop_html_editor/static/aloha.0.23.26/plugins/extra/linkbrowser/img/flags/tl.png
--rw-r--r--   0 lucjean    (501) staff       (20)      352 2019-08-29 13:07:41.000000 coop_html_editor-1.3.1/coop_html_editor/static/aloha.0.23.26/plugins/extra/linkbrowser/img/flags/ws.png
--rw-r--r--   0 lucjean    (501) staff       (20)      327 2019-08-29 13:07:41.000000 coop_html_editor-1.3.1/coop_html_editor/static/aloha.0.23.26/plugins/extra/linkbrowser/img/flags/th.png
--rw-r--r--   0 lucjean    (501) staff       (20)      474 2019-08-29 13:07:41.000000 coop_html_editor-1.3.1/coop_html_editor/static/aloha.0.23.26/plugins/extra/linkbrowser/img/flags/nf.png
--rw-r--r--   0 lucjean    (501) staff       (20)      277 2019-08-29 13:07:41.000000 coop_html_editor-1.3.1/coop_html_editor/static/aloha.0.23.26/plugins/extra/linkbrowser/img/flags/ly.png
--rw-r--r--   0 lucjean    (501) staff       (20)      516 2019-08-29 13:07:40.000000 coop_html_editor-1.3.1/coop_html_editor/static/aloha.0.23.26/plugins/extra/linkbrowser/img/flags/ai.png
--rw-r--r--   0 lucjean    (501) staff       (20)      486 2019-08-29 13:07:40.000000 coop_html_editor-1.3.1/coop_html_editor/static/aloha.0.23.26/plugins/extra/linkbrowser/img/flags/br.png
--rw-r--r--   0 lucjean    (501) staff       (20)      441 2019-08-29 13:07:40.000000 coop_html_editor-1.3.1/coop_html_editor/static/aloha.0.23.26/plugins/extra/linkbrowser/img/flags/cv.png
--rw-r--r--   0 lucjean    (501) staff       (20)      294 2019-08-29 13:07:40.000000 coop_html_editor-1.3.1/coop_html_editor/static/aloha.0.23.26/plugins/extra/linkbrowser/img/flags/be.png
--rw-r--r--   0 lucjean    (501) staff       (20)      471 2019-08-29 13:07:40.000000 coop_html_editor-1.3.1/coop_html_editor/static/aloha.0.23.26/plugins/extra/linkbrowser/img/flags/ca.png
--rw-r--r--   0 lucjean    (501) staff       (20)      372 2019-08-29 13:07:40.000000 coop_html_editor-1.3.1/coop_html_editor/static/aloha.0.23.26/plugins/extra/linkbrowser/img/flags/bd.png
--rw-r--r--   0 lucjean    (501) staff       (20)      391 2019-08-29 13:07:40.000000 coop_html_editor-1.3.1/coop_html_editor/static/aloha.0.23.26/plugins/extra/linkbrowser/img/flags/bs.png
--rw-r--r--   0 lucjean    (501) staff       (20)      341 2019-08-29 13:07:41.000000 coop_html_editor-1.3.1/coop_html_editor/static/aloha.0.23.26/plugins/extra/linkbrowser/img/flags/ng.png
--rw-r--r--   0 lucjean    (501) staff       (20)      449 2019-08-29 13:07:41.000000 coop_html_editor-1.3.1/coop_html_editor/static/aloha.0.23.26/plugins/extra/linkbrowser/img/flags/mk.png
--rw-r--r--   0 lucjean    (501) staff       (20)      349 2019-08-29 13:07:41.000000 coop_html_editor-1.3.1/coop_html_editor/static/aloha.0.23.26/plugins/extra/linkbrowser/img/flags/np.png
--rw-r--r--   0 lucjean    (501) staff       (20)      419 2019-08-29 13:07:41.000000 coop_html_editor-1.3.1/coop_html_editor/static/aloha.0.23.26/plugins/extra/linkbrowser/img/flags/va.png
--rw-r--r--   0 lucjean    (501) staff       (20)      411 2019-08-29 13:07:41.000000 coop_html_editor-1.3.1/coop_html_editor/static/aloha.0.23.26/plugins/extra/linkbrowser/img/flags/uz.png
--rw-r--r--   0 lucjean    (501) staff       (20)      557 2019-08-29 13:07:41.000000 coop_html_editor-1.3.1/coop_html_editor/static/aloha.0.23.26/plugins/extra/linkbrowser/img/flags/wales.png
--rw-r--r--   0 lucjean    (501) staff       (20)      455 2019-08-29 13:07:41.000000 coop_html_editor-1.3.1/coop_html_editor/static/aloha.0.23.26/plugins/extra/linkbrowser/img/flags/um.png
--rw-r--r--   0 lucjean    (501) staff       (20)      522 2019-08-29 13:07:41.000000 coop_html_editor-1.3.1/coop_html_editor/static/aloha.0.23.26/plugins/extra/linkbrowser/img/flags/tk.png
--rw-r--r--   0 lucjean    (501) staff       (20)      412 2019-08-29 13:07:41.000000 coop_html_editor-1.3.1/coop_html_editor/static/aloha.0.23.26/plugins/extra/linkbrowser/img/flags/vc.png
--rw-r--r--   0 lucjean    (501) staff       (20)      462 2019-08-29 13:07:41.000000 coop_html_editor-1.3.1/coop_html_editor/static/aloha.0.23.26/plugins/extra/linkbrowser/img/flags/zw.png
--rw-r--r--   0 lucjean    (501) staff       (20)      391 2019-08-29 13:07:41.000000 coop_html_editor-1.3.1/coop_html_editor/static/aloha.0.23.26/plugins/extra/linkbrowser/img/flags/nr.png
--rw-r--r--   0 lucjean    (501) staff       (20)      393 2019-08-29 13:07:41.000000 coop_html_editor-1.3.1/coop_html_editor/static/aloha.0.23.26/plugins/extra/linkbrowser/img/flags/ne.png
--rw-r--r--   0 lucjean    (501) staff       (20)      445 2019-08-29 13:07:40.000000 coop_html_editor-1.3.1/coop_html_editor/static/aloha.0.23.26/plugins/extra/linkbrowser/img/flags/cu.png
--rw-r--r--   0 lucjean    (501) staff       (20)      341 2019-08-29 13:07:40.000000 coop_html_editor-1.3.1/coop_html_editor/static/aloha.0.23.26/plugins/extra/linkbrowser/img/flags/bf.png
--rw-r--r--   0 lucjean    (501) staff       (20)      320 2019-08-29 13:07:40.000000 coop_html_editor-1.3.1/coop_html_editor/static/aloha.0.23.26/plugins/extra/linkbrowser/img/flags/bg.png
--rw-r--r--   0 lucjean    (501) staff       (20)      496 2019-08-29 13:07:40.000000 coop_html_editor-1.3.1/coop_html_editor/static/aloha.0.23.26/plugins/extra/linkbrowser/img/flags/cc.png
--rw-r--r--   0 lucjean    (501) staff       (20)      518 2019-08-29 13:07:41.000000 coop_html_editor-1.3.1/coop_html_editor/static/aloha.0.23.26/plugins/extra/linkbrowser/img/flags/mh.png
--rw-r--r--   0 lucjean    (501) staff       (20)      523 2019-08-29 13:07:41.000000 coop_html_editor-1.3.1/coop_html_editor/static/aloha.0.23.26/plugins/extra/linkbrowser/img/flags/za.png
--rw-r--r--   0 lucjean    (501) staff       (20)      353 2019-08-29 13:07:40.000000 coop_html_editor-1.3.1/coop_html_editor/static/aloha.0.23.26/plugins/extra/linkbrowser/img/flags/catalonia.png
--rw-r--r--   0 lucjean    (501) staff       (20)      411 2019-08-29 13:07:41.000000 coop_html_editor-1.3.1/coop_html_editor/static/aloha.0.23.26/plugins/extra/linkbrowser/img/flags/uy.png
--rw-r--r--   0 lucjean    (501) staff       (20)      438 2019-08-29 13:07:41.000000 coop_html_editor-1.3.1/coop_html_editor/static/aloha.0.23.26/plugins/extra/linkbrowser/img/flags/wf.png
--rw-r--r--   0 lucjean    (501) staff       (20)      450 2019-08-29 13:07:41.000000 coop_html_editor-1.3.1/coop_html_editor/static/aloha.0.23.26/plugins/extra/linkbrowser/img/flags/vu.png
--rw-r--r--   0 lucjean    (501) staff       (20)      367 2019-08-29 13:07:41.000000 coop_html_editor-1.3.1/coop_html_editor/static/aloha.0.23.26/plugins/extra/linkbrowser/img/flags/tj.png
-drwxr-xr-x   0 lucjean    (501) staff       (20)        0 2019-08-30 10:39:52.000000 coop_html_editor-1.3.1/coop_html_editor/static/aloha.0.23.26/plugins/extra/metaview/
-drwxr-xr-x   0 lucjean    (501) staff       (20)        0 2019-08-30 10:39:52.000000 coop_html_editor-1.3.1/coop_html_editor/static/aloha.0.23.26/plugins/extra/metaview/css/
--rw-r--r--   0 lucjean    (501) staff       (20)     3512 2019-08-29 13:07:41.000000 coop_html_editor-1.3.1/coop_html_editor/static/aloha.0.23.26/plugins/extra/metaview/css/metaview.css
-drwxr-xr-x   0 lucjean    (501) staff       (20)        0 2019-08-30 10:39:35.000000 coop_html_editor-1.3.1/coop_html_editor/static/aloha.0.23.26/plugins/extra/metaview/nls/
-drwxr-xr-x   0 lucjean    (501) staff       (20)        0 2019-08-30 10:39:53.000000 coop_html_editor-1.3.1/coop_html_editor/static/aloha.0.23.26/plugins/extra/metaview/nls/zh-hans/
--rw-r--r--   0 lucjean    (501) staff       (20)       90 2019-08-29 13:07:41.000000 coop_html_editor-1.3.1/coop_html_editor/static/aloha.0.23.26/plugins/extra/metaview/nls/zh-hans/i18n.js
-drwxr-xr-x   0 lucjean    (501) staff       (20)        0 2019-08-30 10:39:53.000000 coop_html_editor-1.3.1/coop_html_editor/static/aloha.0.23.26/plugins/extra/metaview/nls/ca/
--rw-r--r--   0 lucjean    (501) staff       (20)      103 2019-08-29 13:07:41.000000 coop_html_editor-1.3.1/coop_html_editor/static/aloha.0.23.26/plugins/extra/metaview/nls/ca/i18n.js
-drwxr-xr-x   0 lucjean    (501) staff       (20)        0 2019-08-30 10:39:53.000000 coop_html_editor-1.3.1/coop_html_editor/static/aloha.0.23.26/plugins/extra/metaview/nls/ru/
--rw-r--r--   0 lucjean    (501) staff       (20)      131 2019-08-29 13:07:41.000000 coop_html_editor-1.3.1/coop_html_editor/static/aloha.0.23.26/plugins/extra/metaview/nls/ru/i18n.js
-drwxr-xr-x   0 lucjean    (501) staff       (20)        0 2019-08-30 10:39:53.000000 coop_html_editor-1.3.1/coop_html_editor/static/aloha.0.23.26/plugins/extra/metaview/nls/uk/
--rw-r--r--   0 lucjean    (501) staff       (20)      131 2019-08-29 13:07:41.000000 coop_html_editor-1.3.1/coop_html_editor/static/aloha.0.23.26/plugins/extra/metaview/nls/uk/i18n.js
-drwxr-xr-x   0 lucjean    (501) staff       (20)        0 2019-08-30 10:39:53.000000 coop_html_editor-1.3.1/coop_html_editor/static/aloha.0.23.26/plugins/extra/metaview/nls/mk/
--rw-r--r--   0 lucjean    (501) staff       (20)      120 2019-08-29 13:07:41.000000 coop_html_editor-1.3.1/coop_html_editor/static/aloha.0.23.26/plugins/extra/metaview/nls/mk/i18n.js
-drwxr-xr-x   0 lucjean    (501) staff       (20)        0 2019-08-30 10:39:53.000000 coop_html_editor-1.3.1/coop_html_editor/static/aloha.0.23.26/plugins/extra/metaview/nls/pt-br/
--rw-r--r--   0 lucjean    (501) staff       (20)       86 2019-08-29 13:07:41.000000 coop_html_editor-1.3.1/coop_html_editor/static/aloha.0.23.26/plugins/extra/metaview/nls/pt-br/i18n.js
-drwxr-xr-x   0 lucjean    (501) staff       (20)        0 2019-08-30 10:39:53.000000 coop_html_editor-1.3.1/coop_html_editor/static/aloha.0.23.26/plugins/extra/metaview/nls/de/
--rw-r--r--   0 lucjean    (501) staff       (20)      103 2019-08-29 13:07:41.000000 coop_html_editor-1.3.1/coop_html_editor/static/aloha.0.23.26/plugins/extra/metaview/nls/de/i18n.js
--rw-r--r--   0 lucjean    (501) staff       (20)        0 2019-08-29 13:07:41.000000 coop_html_editor-1.3.1/coop_html_editor/static/aloha.0.23.26/plugins/extra/metaview/README
-drwxr-xr-x   0 lucjean    (501) staff       (20)        0 2019-08-30 10:39:53.000000 coop_html_editor-1.3.1/coop_html_editor/static/aloha.0.23.26/plugins/extra/metaview/img/
--rw-r--r--   0 lucjean    (501) staff       (20)      135 2019-08-29 13:07:41.000000 coop_html_editor-1.3.1/coop_html_editor/static/aloha.0.23.26/plugins/extra/metaview/img/blockquote.png
--rw-r--r--   0 lucjean    (501) staff       (20)       87 2019-08-29 13:07:41.000000 coop_html_editor-1.3.1/coop_html_editor/static/aloha.0.23.26/plugins/extra/metaview/img/td.png
--rw-r--r--   0 lucjean    (501) staff       (20)      122 2019-08-29 13:07:41.000000 coop_html_editor-1.3.1/coop_html_editor/static/aloha.0.23.26/plugins/extra/metaview/img/pre.png
--rw-r--r--   0 lucjean    (501) staff       (20)      241 2019-08-29 13:07:41.000000 coop_html_editor-1.3.1/coop_html_editor/static/aloha.0.23.26/plugins/extra/metaview/img/icon_cite.png
--rw-r--r--   0 lucjean    (501) staff       (20)       99 2019-08-29 13:07:41.000000 coop_html_editor-1.3.1/coop_html_editor/static/aloha.0.23.26/plugins/extra/metaview/img/div.png
--rw-r--r--   0 lucjean    (501) staff       (20)       86 2019-08-29 13:07:41.000000 coop_html_editor-1.3.1/coop_html_editor/static/aloha.0.23.26/plugins/extra/metaview/img/dl.png
--rw-r--r--   0 lucjean    (501) staff       (20)      116 2019-08-29 13:07:41.000000 coop_html_editor-1.3.1/coop_html_editor/static/aloha.0.23.26/plugins/extra/metaview/img/h5.png
--rw-r--r--   0 lucjean    (501) staff       (20)      115 2019-08-29 13:07:41.000000 coop_html_editor-1.3.1/coop_html_editor/static/aloha.0.23.26/plugins/extra/metaview/img/h4.png
--rw-r--r--   0 lucjean    (501) staff       (20)      116 2019-08-29 13:07:41.000000 coop_html_editor-1.3.1/coop_html_editor/static/aloha.0.23.26/plugins/extra/metaview/img/h6.png
--rw-r--r--   0 lucjean    (501) staff       (20)       87 2019-08-29 13:07:41.000000 coop_html_editor-1.3.1/coop_html_editor/static/aloha.0.23.26/plugins/extra/metaview/img/dt.png
--rw-r--r--   0 lucjean    (501) staff       (20)      395 2019-08-29 13:07:41.000000 coop_html_editor-1.3.1/coop_html_editor/static/aloha.0.23.26/plugins/extra/metaview/img/cite.png
--rw-r--r--   0 lucjean    (501) staff       (20)      104 2019-08-29 13:07:41.000000 coop_html_editor-1.3.1/coop_html_editor/static/aloha.0.23.26/plugins/extra/metaview/img/hr.png
--rw-r--r--   0 lucjean    (501) staff       (20)      114 2019-08-29 13:07:41.000000 coop_html_editor-1.3.1/coop_html_editor/static/aloha.0.23.26/plugins/extra/metaview/img/h3.png
--rw-r--r--   0 lucjean    (501) staff       (20)      116 2019-08-29 13:07:41.000000 coop_html_editor-1.3.1/coop_html_editor/static/aloha.0.23.26/plugins/extra/metaview/img/h2.png
--rw-r--r--   0 lucjean    (501) staff       (20)       87 2019-08-29 13:07:41.000000 coop_html_editor-1.3.1/coop_html_editor/static/aloha.0.23.26/plugins/extra/metaview/img/dd.png
--rw-r--r--   0 lucjean    (501) staff       (20)      111 2019-08-29 13:07:41.000000 coop_html_editor-1.3.1/coop_html_editor/static/aloha.0.23.26/plugins/extra/metaview/img/h1.png
--rw-r--r--   0 lucjean    (501) staff       (20)      213 2019-08-29 13:07:41.000000 coop_html_editor-1.3.1/coop_html_editor/static/aloha.0.23.26/plugins/extra/metaview/img/anchor.png
--rw-r--r--   0 lucjean    (501) staff       (20)       91 2019-08-29 13:07:41.000000 coop_html_editor-1.3.1/coop_html_editor/static/aloha.0.23.26/plugins/extra/metaview/img/th.png
--rw-r--r--   0 lucjean    (501) staff       (20)      122 2019-08-29 13:07:41.000000 coop_html_editor-1.3.1/coop_html_editor/static/aloha.0.23.26/plugins/extra/metaview/img/caption.png
--rw-r--r--   0 lucjean    (501) staff       (20)      116 2019-08-29 13:07:41.000000 coop_html_editor-1.3.1/coop_html_editor/static/aloha.0.23.26/plugins/extra/metaview/img/table.png
--rw-r--r--   0 lucjean    (501) staff       (20)      113 2019-08-29 13:07:41.000000 coop_html_editor-1.3.1/coop_html_editor/static/aloha.0.23.26/plugins/extra/metaview/img/p.png
--rw-r--r--   0 lucjean    (501) staff       (20)      135 2019-08-29 13:07:41.000000 coop_html_editor-1.3.1/coop_html_editor/static/aloha.0.23.26/plugins/extra/metaview/img/button.png
-drwxr-xr-x   0 lucjean    (501) staff       (20)        0 2019-08-30 10:39:54.000000 coop_html_editor-1.3.1/coop_html_editor/static/aloha.0.23.26/plugins/extra/zemanta/
-drwxr-xr-x   0 lucjean    (501) staff       (20)        0 2019-08-30 10:39:54.000000 coop_html_editor-1.3.1/coop_html_editor/static/aloha.0.23.26/plugins/extra/zemanta/css/
--rw-r--r--   0 lucjean    (501) staff       (20)      375 2019-08-29 13:07:41.000000 coop_html_editor-1.3.1/coop_html_editor/static/aloha.0.23.26/plugins/extra/zemanta/css/zemanta-widget-alohaeditor.css
-drwxr-xr-x   0 lucjean    (501) staff       (20)        0 2019-08-30 10:39:54.000000 coop_html_editor-1.3.1/coop_html_editor/static/aloha.0.23.26/plugins/extra/zemanta/nls/
-drwxr-xr-x   0 lucjean    (501) staff       (20)        0 2019-08-30 10:39:54.000000 coop_html_editor-1.3.1/coop_html_editor/static/aloha.0.23.26/plugins/extra/zemanta/nls/zh-hans/
--rw-r--r--   0 lucjean    (501) staff       (20)      211 2019-08-29 13:07:41.000000 coop_html_editor-1.3.1/coop_html_editor/static/aloha.0.23.26/plugins/extra/zemanta/nls/zh-hans/i18n.js
-drwxr-xr-x   0 lucjean    (501) staff       (20)        0 2019-08-30 10:39:54.000000 coop_html_editor-1.3.1/coop_html_editor/static/aloha.0.23.26/plugins/extra/zemanta/nls/ca/
--rw-r--r--   0 lucjean    (501) staff       (20)      236 2019-08-29 13:07:41.000000 coop_html_editor-1.3.1/coop_html_editor/static/aloha.0.23.26/plugins/extra/zemanta/nls/ca/i18n.js
-drwxr-xr-x   0 lucjean    (501) staff       (20)        0 2019-08-30 10:39:54.000000 coop_html_editor-1.3.1/coop_html_editor/static/aloha.0.23.26/plugins/extra/zemanta/nls/ru/
--rw-r--r--   0 lucjean    (501) staff       (20)      315 2019-08-29 13:07:41.000000 coop_html_editor-1.3.1/coop_html_editor/static/aloha.0.23.26/plugins/extra/zemanta/nls/ru/i18n.js
-drwxr-xr-x   0 lucjean    (501) staff       (20)        0 2019-08-30 10:39:54.000000 coop_html_editor-1.3.1/coop_html_editor/static/aloha.0.23.26/plugins/extra/zemanta/nls/uk/
--rw-r--r--   0 lucjean    (501) staff       (20)      307 2019-08-29 13:07:41.000000 coop_html_editor-1.3.1/coop_html_editor/static/aloha.0.23.26/plugins/extra/zemanta/nls/uk/i18n.js
-drwxr-xr-x   0 lucjean    (501) staff       (20)        0 2019-08-30 10:39:54.000000 coop_html_editor-1.3.1/coop_html_editor/static/aloha.0.23.26/plugins/extra/zemanta/nls/mk/
--rw-r--r--   0 lucjean    (501) staff       (20)      308 2019-08-29 13:07:41.000000 coop_html_editor-1.3.1/coop_html_editor/static/aloha.0.23.26/plugins/extra/zemanta/nls/mk/i18n.js
-drwxr-xr-x   0 lucjean    (501) staff       (20)        0 2019-08-30 10:39:54.000000 coop_html_editor-1.3.1/coop_html_editor/static/aloha.0.23.26/plugins/extra/zemanta/nls/pt-br/
--rw-r--r--   0 lucjean    (501) staff       (20)      231 2019-08-29 13:07:41.000000 coop_html_editor-1.3.1/coop_html_editor/static/aloha.0.23.26/plugins/extra/zemanta/nls/pt-br/i18n.js
-drwxr-xr-x   0 lucjean    (501) staff       (20)        0 2019-08-30 10:39:54.000000 coop_html_editor-1.3.1/coop_html_editor/static/aloha.0.23.26/plugins/extra/zemanta/nls/de/
--rw-r--r--   0 lucjean    (501) staff       (20)      231 2019-08-29 13:07:41.000000 coop_html_editor-1.3.1/coop_html_editor/static/aloha.0.23.26/plugins/extra/zemanta/nls/de/i18n.js
--rw-r--r--   0 lucjean    (501) staff       (20)      340 2019-08-29 13:07:41.000000 coop_html_editor-1.3.1/coop_html_editor/static/aloha.0.23.26/plugins/extra/zemanta/nls/i18n.js
--rw-r--r--   0 lucjean    (501) staff       (20)      189 2019-08-29 13:07:41.000000 coop_html_editor-1.3.1/coop_html_editor/static/aloha.0.23.26/plugins/extra/zemanta/README
-drwxr-xr-x   0 lucjean    (501) staff       (20)        0 2019-08-30 10:39:54.000000 coop_html_editor-1.3.1/coop_html_editor/static/aloha.0.23.26/plugins/extra/zemanta/img/
--rw-r--r--   0 lucjean    (501) staff       (20)      622 2019-08-29 13:07:41.000000 coop_html_editor-1.3.1/coop_html_editor/static/aloha.0.23.26/plugins/extra/zemanta/img/zemanta-mini-logo.png
-drwxr-xr-x   0 lucjean    (501) staff       (20)        0 2019-08-30 10:39:54.000000 coop_html_editor-1.3.1/coop_html_editor/static/aloha.0.23.26/plugins/extra/zemanta/lib/
--rw-r--r--   0 lucjean    (501) staff       (20)     7958 2019-08-29 13:07:41.000000 coop_html_editor-1.3.1/coop_html_editor/static/aloha.0.23.26/plugins/extra/zemanta/lib/zemanta-plugin.js
-drwxr-xr-x   0 lucjean    (501) staff       (20)        0 2019-08-30 10:39:42.000000 coop_html_editor-1.3.1/coop_html_editor/static/aloha.0.23.26/plugins/extra/attributes/
-drwxr-xr-x   0 lucjean    (501) staff       (20)        0 2019-08-30 10:39:42.000000 coop_html_editor-1.3.1/coop_html_editor/static/aloha.0.23.26/plugins/extra/attributes/css/
--rw-r--r--   0 lucjean    (501) staff       (20)      643 2019-08-29 13:07:39.000000 coop_html_editor-1.3.1/coop_html_editor/static/aloha.0.23.26/plugins/extra/attributes/css/attributes.css
-drwxr-xr-x   0 lucjean    (501) staff       (20)        0 2019-08-30 10:39:42.000000 coop_html_editor-1.3.1/coop_html_editor/static/aloha.0.23.26/plugins/extra/attributes/nls/
-drwxr-xr-x   0 lucjean    (501) staff       (20)        0 2019-08-30 10:39:42.000000 coop_html_editor-1.3.1/coop_html_editor/static/aloha.0.23.26/plugins/extra/attributes/nls/zh-hans/
--rw-r--r--   0 lucjean    (501) staff       (20)      121 2019-08-29 13:07:39.000000 coop_html_editor-1.3.1/coop_html_editor/static/aloha.0.23.26/plugins/extra/attributes/nls/zh-hans/i18n.js
-drwxr-xr-x   0 lucjean    (501) staff       (20)        0 2019-08-30 10:39:42.000000 coop_html_editor-1.3.1/coop_html_editor/static/aloha.0.23.26/plugins/extra/attributes/nls/ca/
--rw-r--r--   0 lucjean    (501) staff       (20)      130 2019-08-29 13:07:39.000000 coop_html_editor-1.3.1/coop_html_editor/static/aloha.0.23.26/plugins/extra/attributes/nls/ca/i18n.js
-drwxr-xr-x   0 lucjean    (501) staff       (20)        0 2019-08-30 10:39:42.000000 coop_html_editor-1.3.1/coop_html_editor/static/aloha.0.23.26/plugins/extra/attributes/nls/ru/
--rw-r--r--   0 lucjean    (501) staff       (20)      147 2019-08-29 13:07:39.000000 coop_html_editor-1.3.1/coop_html_editor/static/aloha.0.23.26/plugins/extra/attributes/nls/ru/i18n.js
-drwxr-xr-x   0 lucjean    (501) staff       (20)        0 2019-08-30 10:39:42.000000 coop_html_editor-1.3.1/coop_html_editor/static/aloha.0.23.26/plugins/extra/attributes/nls/uk/
--rw-r--r--   0 lucjean    (501) staff       (20)      145 2019-08-29 13:07:39.000000 coop_html_editor-1.3.1/coop_html_editor/static/aloha.0.23.26/plugins/extra/attributes/nls/uk/i18n.js
-drwxr-xr-x   0 lucjean    (501) staff       (20)        0 2019-08-30 10:39:42.000000 coop_html_editor-1.3.1/coop_html_editor/static/aloha.0.23.26/plugins/extra/attributes/nls/mk/
--rw-r--r--   0 lucjean    (501) staff       (20)      141 2019-08-29 13:07:39.000000 coop_html_editor-1.3.1/coop_html_editor/static/aloha.0.23.26/plugins/extra/attributes/nls/mk/i18n.js
-drwxr-xr-x   0 lucjean    (501) staff       (20)        0 2019-08-30 10:39:42.000000 coop_html_editor-1.3.1/coop_html_editor/static/aloha.0.23.26/plugins/extra/attributes/nls/pt-br/
--rw-r--r--   0 lucjean    (501) staff       (20)      121 2019-08-29 13:07:39.000000 coop_html_editor-1.3.1/coop_html_editor/static/aloha.0.23.26/plugins/extra/attributes/nls/pt-br/i18n.js
-drwxr-xr-x   0 lucjean    (501) staff       (20)        0 2019-08-30 10:39:42.000000 coop_html_editor-1.3.1/coop_html_editor/static/aloha.0.23.26/plugins/extra/attributes/nls/de/
--rw-r--r--   0 lucjean    (501) staff       (20)      126 2019-08-29 13:07:39.000000 coop_html_editor-1.3.1/coop_html_editor/static/aloha.0.23.26/plugins/extra/attributes/nls/de/i18n.js
--rw-r--r--   0 lucjean    (501) staff       (20)      241 2019-08-29 13:07:39.000000 coop_html_editor-1.3.1/coop_html_editor/static/aloha.0.23.26/plugins/extra/attributes/nls/i18n.js
--rw-r--r--   0 lucjean    (501) staff       (20)        0 2019-08-29 13:07:39.000000 coop_html_editor-1.3.1/coop_html_editor/static/aloha.0.23.26/plugins/extra/attributes/README
-drwxr-xr-x   0 lucjean    (501) staff       (20)        0 2019-08-30 10:39:42.000000 coop_html_editor-1.3.1/coop_html_editor/static/aloha.0.23.26/plugins/extra/attributes/lib/
--rw-r--r--   0 lucjean    (501) staff       (20)     8179 2019-08-29 13:07:39.000000 coop_html_editor-1.3.1/coop_html_editor/static/aloha.0.23.26/plugins/extra/attributes/lib/attributes-plugin.js
-drwxr-xr-x   0 lucjean    (501) staff       (20)        0 2019-08-30 10:39:43.000000 coop_html_editor-1.3.1/coop_html_editor/static/aloha.0.23.26/plugins/extra/draganddropfiles/
-drwxr-xr-x   0 lucjean    (501) staff       (20)        0 2019-08-30 10:39:43.000000 coop_html_editor-1.3.1/coop_html_editor/static/aloha.0.23.26/plugins/extra/draganddropfiles/demo/
--rw-r--r--   0 lucjean    (501) staff       (20)     4873 2019-08-29 13:07:39.000000 coop_html_editor-1.3.1/coop_html_editor/static/aloha.0.23.26/plugins/extra/draganddropfiles/demo/index.html
-drwxr-xr-x   0 lucjean    (501) staff       (20)        0 2019-08-30 10:39:43.000000 coop_html_editor-1.3.1/coop_html_editor/static/aloha.0.23.26/plugins/extra/draganddropfiles/demo/specs/
--rw-r--r--   0 lucjean    (501) staff       (20)    39725 2019-08-29 13:07:39.000000 coop_html_editor-1.3.1/coop_html_editor/static/aloha.0.23.26/plugins/extra/draganddropfiles/demo/specs/DragnDropnImage.graphml
--rw-r--r--   0 lucjean    (501) staff       (20)      853 2019-08-29 13:07:39.000000 coop_html_editor-1.3.1/coop_html_editor/static/aloha.0.23.26/plugins/extra/draganddropfiles/demo/index.css
--rw-r--r--   0 lucjean    (501) staff       (20)       25 2019-08-29 13:07:39.000000 coop_html_editor-1.3.1/coop_html_editor/static/aloha.0.23.26/plugins/extra/draganddropfiles/demo/.gitignore
--rw-r--r--   0 lucjean    (501) staff       (20)      616 2019-08-29 13:07:39.000000 coop_html_editor-1.3.1/coop_html_editor/static/aloha.0.23.26/plugins/extra/draganddropfiles/demo/upload.php.example
--rw-r--r--   0 lucjean    (501) staff       (20)      853 2019-08-29 13:07:39.000000 coop_html_editor-1.3.1/coop_html_editor/static/aloha.0.23.26/plugins/extra/draganddropfiles/demo/style.css
-drwxr-xr-x   0 lucjean    (501) staff       (20)        0 2019-08-30 10:39:43.000000 coop_html_editor-1.3.1/coop_html_editor/static/aloha.0.23.26/plugins/extra/draganddropfiles/demo/migration/
--rw-r--r--   0 lucjean    (501) staff       (20)    11160 2019-08-29 13:07:39.000000 coop_html_editor-1.3.1/coop_html_editor/static/aloha.0.23.26/plugins/extra/draganddropfiles/demo/migration/index.html
--rw-r--r--   0 lucjean    (501) staff       (20)     2827 2019-08-29 13:07:39.000000 coop_html_editor-1.3.1/coop_html_editor/static/aloha.0.23.26/plugins/extra/draganddropfiles/demo/migration/index.css
-drwxr-xr-x   0 lucjean    (501) staff       (20)        0 2019-08-30 10:39:43.000000 coop_html_editor-1.3.1/coop_html_editor/static/aloha.0.23.26/plugins/extra/draganddropfiles/nls/
-drwxr-xr-x   0 lucjean    (501) staff       (20)        0 2019-08-30 10:39:43.000000 coop_html_editor-1.3.1/coop_html_editor/static/aloha.0.23.26/plugins/extra/draganddropfiles/nls/zh-hans/
--rw-r--r--   0 lucjean    (501) staff       (20)       48 2019-08-29 13:07:39.000000 coop_html_editor-1.3.1/coop_html_editor/static/aloha.0.23.26/plugins/extra/draganddropfiles/nls/zh-hans/i18n.js
-drwxr-xr-x   0 lucjean    (501) staff       (20)        0 2019-08-30 10:39:43.000000 coop_html_editor-1.3.1/coop_html_editor/static/aloha.0.23.26/plugins/extra/draganddropfiles/nls/ca/
--rw-r--r--   0 lucjean    (501) staff       (20)       47 2019-08-29 13:07:39.000000 coop_html_editor-1.3.1/coop_html_editor/static/aloha.0.23.26/plugins/extra/draganddropfiles/nls/ca/i18n.js
-drwxr-xr-x   0 lucjean    (501) staff       (20)        0 2019-08-30 10:39:43.000000 coop_html_editor-1.3.1/coop_html_editor/static/aloha.0.23.26/plugins/extra/draganddropfiles/nls/ru/
--rw-r--r--   0 lucjean    (501) staff       (20)       50 2019-08-29 13:07:39.000000 coop_html_editor-1.3.1/coop_html_editor/static/aloha.0.23.26/plugins/extra/draganddropfiles/nls/ru/i18n.js
-drwxr-xr-x   0 lucjean    (501) staff       (20)        0 2019-08-30 10:39:43.000000 coop_html_editor-1.3.1/coop_html_editor/static/aloha.0.23.26/plugins/extra/draganddropfiles/nls/uk/
--rw-r--r--   0 lucjean    (501) staff       (20)       50 2019-08-29 13:07:39.000000 coop_html_editor-1.3.1/coop_html_editor/static/aloha.0.23.26/plugins/extra/draganddropfiles/nls/uk/i18n.js
-drwxr-xr-x   0 lucjean    (501) staff       (20)        0 2019-08-30 10:39:43.000000 coop_html_editor-1.3.1/coop_html_editor/static/aloha.0.23.26/plugins/extra/draganddropfiles/nls/mk/
--rw-r--r--   0 lucjean    (501) staff       (20)       58 2019-08-29 13:07:39.000000 coop_html_editor-1.3.1/coop_html_editor/static/aloha.0.23.26/plugins/extra/draganddropfiles/nls/mk/i18n.js
-drwxr-xr-x   0 lucjean    (501) staff       (20)        0 2019-08-30 10:39:43.000000 coop_html_editor-1.3.1/coop_html_editor/static/aloha.0.23.26/plugins/extra/draganddropfiles/nls/pt-br/
--rw-r--r--   0 lucjean    (501) staff       (20)       49 2019-08-29 13:07:39.000000 coop_html_editor-1.3.1/coop_html_editor/static/aloha.0.23.26/plugins/extra/draganddropfiles/nls/pt-br/i18n.js
-drwxr-xr-x   0 lucjean    (501) staff       (20)        0 2019-08-30 10:39:43.000000 coop_html_editor-1.3.1/coop_html_editor/static/aloha.0.23.26/plugins/extra/draganddropfiles/nls/de/
--rw-r--r--   0 lucjean    (501) staff       (20)       47 2019-08-29 13:07:39.000000 coop_html_editor-1.3.1/coop_html_editor/static/aloha.0.23.26/plugins/extra/draganddropfiles/nls/de/i18n.js
--rw-r--r--   0 lucjean    (501) staff       (20)      168 2019-08-29 13:07:39.000000 coop_html_editor-1.3.1/coop_html_editor/static/aloha.0.23.26/plugins/extra/draganddropfiles/nls/i18n.js
--rw-r--r--   0 lucjean    (501) staff       (20)       64 2019-08-29 13:07:39.000000 coop_html_editor-1.3.1/coop_html_editor/static/aloha.0.23.26/plugins/extra/draganddropfiles/TODO.md
--rw-r--r--   0 lucjean    (501) staff       (20)      169 2019-08-29 13:07:39.000000 coop_html_editor-1.3.1/coop_html_editor/static/aloha.0.23.26/plugins/extra/draganddropfiles/README.md
-drwxr-xr-x   0 lucjean    (501) staff       (20)        0 2019-08-30 10:39:43.000000 coop_html_editor-1.3.1/coop_html_editor/static/aloha.0.23.26/plugins/extra/draganddropfiles/img/
--rw-r--r--   0 lucjean    (501) staff       (20)      481 2019-08-29 13:07:39.000000 coop_html_editor-1.3.1/coop_html_editor/static/aloha.0.23.26/plugins/extra/draganddropfiles/img/tick.png
--rw-r--r--   0 lucjean    (501) staff       (20)      770 2019-08-29 13:07:39.000000 coop_html_editor-1.3.1/coop_html_editor/static/aloha.0.23.26/plugins/extra/draganddropfiles/img/loading.gif
--rw-r--r--   0 lucjean    (501) staff       (20)      688 2019-08-29 13:07:39.000000 coop_html_editor-1.3.1/coop_html_editor/static/aloha.0.23.26/plugins/extra/draganddropfiles/img/hourglass.png
--rw-r--r--   0 lucjean    (501) staff       (20)      600 2019-08-29 13:07:39.000000 coop_html_editor-1.3.1/coop_html_editor/static/aloha.0.23.26/plugins/extra/draganddropfiles/img/cross.png
--rw-r--r--   0 lucjean    (501) staff       (20)      582 2019-08-29 13:07:39.000000 coop_html_editor-1.3.1/coop_html_editor/static/aloha.0.23.26/plugins/extra/draganddropfiles/img/page.png
--rw-r--r--   0 lucjean    (501) staff       (20)        3 2019-08-29 13:07:39.000000 coop_html_editor-1.3.1/coop_html_editor/static/aloha.0.23.26/plugins/extra/draganddropfiles/package.json
-drwxr-xr-x   0 lucjean    (501) staff       (20)        0 2019-08-30 10:39:43.000000 coop_html_editor-1.3.1/coop_html_editor/static/aloha.0.23.26/plugins/extra/draganddropfiles/lib/
--rw-r--r--   0 lucjean    (501) staff       (20)      150 2019-08-29 13:07:39.000000 coop_html_editor-1.3.1/coop_html_editor/static/aloha.0.23.26/plugins/extra/draganddropfiles/lib/draganddropfiles-plugin.js
--rw-r--r--   0 lucjean    (501) staff       (20)     1993 2019-08-29 13:07:39.000000 coop_html_editor-1.3.1/coop_html_editor/static/aloha.0.23.26/plugins/extra/draganddropfiles/lib/dragndropfiles.css
--rw-r--r--   0 lucjean    (501) staff       (20)    11867 2019-08-29 13:07:39.000000 coop_html_editor-1.3.1/coop_html_editor/static/aloha.0.23.26/plugins/extra/draganddropfiles/lib/dragndropfiles.js
--rw-r--r--   0 lucjean    (501) staff       (20)    10200 2019-08-29 13:07:39.000000 coop_html_editor-1.3.1/coop_html_editor/static/aloha.0.23.26/plugins/extra/draganddropfiles/lib/dropfilesrepository.js
-drwxr-xr-x   0 lucjean    (501) staff       (20)        0 2019-08-30 10:39:54.000000 coop_html_editor-1.3.1/coop_html_editor/static/aloha.0.23.26/plugins/extra/wai-lang/
-drwxr-xr-x   0 lucjean    (501) staff       (20)        0 2019-08-30 10:39:54.000000 coop_html_editor-1.3.1/coop_html_editor/static/aloha.0.23.26/plugins/extra/wai-lang/css/
--rw-r--r--   0 lucjean    (501) staff       (20)      565 2019-08-29 13:07:41.000000 coop_html_editor-1.3.1/coop_html_editor/static/aloha.0.23.26/plugins/extra/wai-lang/css/wai-lang.css
-drwxr-xr-x   0 lucjean    (501) staff       (20)        0 2019-08-30 10:39:35.000000 coop_html_editor-1.3.1/coop_html_editor/static/aloha.0.23.26/plugins/extra/wai-lang/nls/
-drwxr-xr-x   0 lucjean    (501) staff       (20)        0 2019-08-30 10:39:54.000000 coop_html_editor-1.3.1/coop_html_editor/static/aloha.0.23.26/plugins/extra/wai-lang/nls/zh-hans/
--rw-r--r--   0 lucjean    (501) staff       (20)      173 2019-08-29 13:07:41.000000 coop_html_editor-1.3.1/coop_html_editor/static/aloha.0.23.26/plugins/extra/wai-lang/nls/zh-hans/i18n.js
-drwxr-xr-x   0 lucjean    (501) staff       (20)        0 2019-08-30 10:39:54.000000 coop_html_editor-1.3.1/coop_html_editor/static/aloha.0.23.26/plugins/extra/wai-lang/nls/ca/
--rw-r--r--   0 lucjean    (501) staff       (20)      206 2019-08-29 13:07:41.000000 coop_html_editor-1.3.1/coop_html_editor/static/aloha.0.23.26/plugins/extra/wai-lang/nls/ca/i18n.js
-drwxr-xr-x   0 lucjean    (501) staff       (20)        0 2019-08-30 10:39:54.000000 coop_html_editor-1.3.1/coop_html_editor/static/aloha.0.23.26/plugins/extra/wai-lang/nls/ru/
--rw-r--r--   0 lucjean    (501) staff       (20)      262 2019-08-29 13:07:41.000000 coop_html_editor-1.3.1/coop_html_editor/static/aloha.0.23.26/plugins/extra/wai-lang/nls/ru/i18n.js
-drwxr-xr-x   0 lucjean    (501) staff       (20)        0 2019-08-30 10:39:54.000000 coop_html_editor-1.3.1/coop_html_editor/static/aloha.0.23.26/plugins/extra/wai-lang/nls/uk/
--rw-r--r--   0 lucjean    (501) staff       (20)      236 2019-08-29 13:07:41.000000 coop_html_editor-1.3.1/coop_html_editor/static/aloha.0.23.26/plugins/extra/wai-lang/nls/uk/i18n.js
-drwxr-xr-x   0 lucjean    (501) staff       (20)        0 2019-08-30 10:39:54.000000 coop_html_editor-1.3.1/coop_html_editor/static/aloha.0.23.26/plugins/extra/wai-lang/nls/mk/
--rw-r--r--   0 lucjean    (501) staff       (20)      254 2019-08-29 13:07:41.000000 coop_html_editor-1.3.1/coop_html_editor/static/aloha.0.23.26/plugins/extra/wai-lang/nls/mk/i18n.js
-drwxr-xr-x   0 lucjean    (501) staff       (20)        0 2019-08-30 10:39:54.000000 coop_html_editor-1.3.1/coop_html_editor/static/aloha.0.23.26/plugins/extra/wai-lang/nls/pt-br/
--rw-r--r--   0 lucjean    (501) staff       (20)      212 2019-08-29 13:07:41.000000 coop_html_editor-1.3.1/coop_html_editor/static/aloha.0.23.26/plugins/extra/wai-lang/nls/pt-br/i18n.js
-drwxr-xr-x   0 lucjean    (501) staff       (20)        0 2019-08-30 10:39:54.000000 coop_html_editor-1.3.1/coop_html_editor/static/aloha.0.23.26/plugins/extra/wai-lang/nls/de/
--rw-r--r--   0 lucjean    (501) staff       (20)      201 2019-08-29 13:07:41.000000 coop_html_editor-1.3.1/coop_html_editor/static/aloha.0.23.26/plugins/extra/wai-lang/nls/de/i18n.js
--rw-r--r--   0 lucjean    (501) staff       (20)      618 2019-08-29 13:07:41.000000 coop_html_editor-1.3.1/coop_html_editor/static/aloha.0.23.26/plugins/extra/wai-lang/README.md
-drwxr-xr-x   0 lucjean    (501) staff       (20)        0 2019-08-30 10:39:54.000000 coop_html_editor-1.3.1/coop_html_editor/static/aloha.0.23.26/plugins/extra/wai-lang/img/
--rw-r--r--   0 lucjean    (501) staff       (20)      866 2019-08-29 13:07:41.000000 coop_html_editor-1.3.1/coop_html_editor/static/aloha.0.23.26/plugins/extra/wai-lang/img/remove-button.png
--rw-r--r--   0 lucjean    (501) staff       (20)      849 2019-08-29 13:07:41.000000 coop_html_editor-1.3.1/coop_html_editor/static/aloha.0.23.26/plugins/extra/wai-lang/img/button.png
-drwxr-xr-x   0 lucjean    (501) staff       (20)        0 2019-08-30 10:39:54.000000 coop_html_editor-1.3.1/coop_html_editor/static/aloha.0.23.26/plugins/extra/wai-lang/lib/
--rw-r--r--   0 lucjean    (501) staff       (20)    26333 2019-08-29 13:07:41.000000 coop_html_editor-1.3.1/coop_html_editor/static/aloha.0.23.26/plugins/extra/wai-lang/lib/iso639-2-de.js
--rw-r--r--   0 lucjean    (501) staff       (20)     9403 2019-08-29 13:07:41.000000 coop_html_editor-1.3.1/coop_html_editor/static/aloha.0.23.26/plugins/extra/wai-lang/lib/iso639-1-en.js
--rw-r--r--   0 lucjean    (501) staff       (20)     9550 2019-08-29 13:07:41.000000 coop_html_editor-1.3.1/coop_html_editor/static/aloha.0.23.26/plugins/extra/wai-lang/lib/iso639-1-de.js
--rw-r--r--   0 lucjean    (501) staff       (20)    25970 2019-08-29 13:07:41.000000 coop_html_editor-1.3.1/coop_html_editor/static/aloha.0.23.26/plugins/extra/wai-lang/lib/iso639-2-en.js
-drwxr-xr-x   0 lucjean    (501) staff       (20)        0 2019-08-30 10:39:35.000000 coop_html_editor-1.3.1/coop_html_editor/static/aloha.0.23.26/plugins/extra/profiler/
-drwxr-xr-x   0 lucjean    (501) staff       (20)        0 2019-08-30 10:39:53.000000 coop_html_editor-1.3.1/coop_html_editor/static/aloha.0.23.26/plugins/extra/profiler/css/
--rw-r--r--   0 lucjean    (501) staff       (20)      856 2019-08-29 13:07:41.000000 coop_html_editor-1.3.1/coop_html_editor/static/aloha.0.23.26/plugins/extra/profiler/css/profiler.css
-drwxr-xr-x   0 lucjean    (501) staff       (20)        0 2019-08-30 10:39:53.000000 coop_html_editor-1.3.1/coop_html_editor/static/aloha.0.23.26/plugins/extra/profiler/lib/
--rw-r--r--   0 lucjean    (501) staff       (20)     8683 2019-08-29 13:07:41.000000 coop_html_editor-1.3.1/coop_html_editor/static/aloha.0.23.26/plugins/extra/profiler/lib/profiler-plugin.js
-drwxr-xr-x   0 lucjean    (501) staff       (20)        0 2019-08-30 10:39:53.000000 coop_html_editor-1.3.1/coop_html_editor/static/aloha.0.23.26/plugins/extra/numerated-headers/
-drwxr-xr-x   0 lucjean    (501) staff       (20)        0 2019-08-30 10:39:53.000000 coop_html_editor-1.3.1/coop_html_editor/static/aloha.0.23.26/plugins/extra/numerated-headers/demo/
--rw-r--r--   0 lucjean    (501) staff       (20)     3025 2019-08-29 13:07:41.000000 coop_html_editor-1.3.1/coop_html_editor/static/aloha.0.23.26/plugins/extra/numerated-headers/demo/index.html
-drwxr-xr-x   0 lucjean    (501) staff       (20)        0 2019-08-30 10:39:53.000000 coop_html_editor-1.3.1/coop_html_editor/static/aloha.0.23.26/plugins/extra/numerated-headers/demo/js/
--rw-r--r--   0 lucjean    (501) staff       (20)     4521 2019-08-29 13:07:41.000000 coop_html_editor-1.3.1/coop_html_editor/static/aloha.0.23.26/plugins/extra/numerated-headers/demo/js/aloha-config.js
--rw-r--r--   0 lucjean    (501) staff       (20)     2858 2019-08-29 13:07:41.000000 coop_html_editor-1.3.1/coop_html_editor/static/aloha.0.23.26/plugins/extra/numerated-headers/demo/index.css
-drwxr-xr-x   0 lucjean    (501) staff       (20)        0 2019-08-30 10:39:53.000000 coop_html_editor-1.3.1/coop_html_editor/static/aloha.0.23.26/plugins/extra/numerated-headers/css/
--rw-r--r--   0 lucjean    (501) staff       (20)      271 2019-08-29 13:07:41.000000 coop_html_editor-1.3.1/coop_html_editor/static/aloha.0.23.26/plugins/extra/numerated-headers/css/numerated-headers.css
-drwxr-xr-x   0 lucjean    (501) staff       (20)        0 2019-08-30 10:39:35.000000 coop_html_editor-1.3.1/coop_html_editor/static/aloha.0.23.26/plugins/extra/numerated-headers/nls/
-drwxr-xr-x   0 lucjean    (501) staff       (20)        0 2019-08-30 10:39:53.000000 coop_html_editor-1.3.1/coop_html_editor/static/aloha.0.23.26/plugins/extra/numerated-headers/nls/zh-hans/
--rw-r--r--   0 lucjean    (501) staff       (20)      121 2019-08-29 13:07:41.000000 coop_html_editor-1.3.1/coop_html_editor/static/aloha.0.23.26/plugins/extra/numerated-headers/nls/zh-hans/i18n.js
-drwxr-xr-x   0 lucjean    (501) staff       (20)        0 2019-08-30 10:39:53.000000 coop_html_editor-1.3.1/coop_html_editor/static/aloha.0.23.26/plugins/extra/numerated-headers/nls/ca/
--rw-r--r--   0 lucjean    (501) staff       (20)      130 2019-08-29 13:07:41.000000 coop_html_editor-1.3.1/coop_html_editor/static/aloha.0.23.26/plugins/extra/numerated-headers/nls/ca/i18n.js
-drwxr-xr-x   0 lucjean    (501) staff       (20)        0 2019-08-30 10:39:53.000000 coop_html_editor-1.3.1/coop_html_editor/static/aloha.0.23.26/plugins/extra/numerated-headers/nls/ru/
--rw-r--r--   0 lucjean    (501) staff       (20)      147 2019-08-29 13:07:41.000000 coop_html_editor-1.3.1/coop_html_editor/static/aloha.0.23.26/plugins/extra/numerated-headers/nls/ru/i18n.js
-drwxr-xr-x   0 lucjean    (501) staff       (20)        0 2019-08-30 10:39:53.000000 coop_html_editor-1.3.1/coop_html_editor/static/aloha.0.23.26/plugins/extra/numerated-headers/nls/uk/
--rw-r--r--   0 lucjean    (501) staff       (20)      145 2019-08-29 13:07:41.000000 coop_html_editor-1.3.1/coop_html_editor/static/aloha.0.23.26/plugins/extra/numerated-headers/nls/uk/i18n.js
-drwxr-xr-x   0 lucjean    (501) staff       (20)        0 2019-08-30 10:39:53.000000 coop_html_editor-1.3.1/coop_html_editor/static/aloha.0.23.26/plugins/extra/numerated-headers/nls/mk/
--rw-r--r--   0 lucjean    (501) staff       (20)      143 2019-08-29 13:07:41.000000 coop_html_editor-1.3.1/coop_html_editor/static/aloha.0.23.26/plugins/extra/numerated-headers/nls/mk/i18n.js
-drwxr-xr-x   0 lucjean    (501) staff       (20)        0 2019-08-30 10:39:53.000000 coop_html_editor-1.3.1/coop_html_editor/static/aloha.0.23.26/plugins/extra/numerated-headers/nls/pt-br/
--rw-r--r--   0 lucjean    (501) staff       (20)      121 2019-08-29 13:07:41.000000 coop_html_editor-1.3.1/coop_html_editor/static/aloha.0.23.26/plugins/extra/numerated-headers/nls/pt-br/i18n.js
-drwxr-xr-x   0 lucjean    (501) staff       (20)        0 2019-08-30 10:39:53.000000 coop_html_editor-1.3.1/coop_html_editor/static/aloha.0.23.26/plugins/extra/numerated-headers/nls/de/
--rw-r--r--   0 lucjean    (501) staff       (20)      208 2019-08-29 13:07:41.000000 coop_html_editor-1.3.1/coop_html_editor/static/aloha.0.23.26/plugins/extra/numerated-headers/nls/de/i18n.js
--rw-r--r--   0 lucjean    (501) staff       (20)        0 2019-08-29 13:07:41.000000 coop_html_editor-1.3.1/coop_html_editor/static/aloha.0.23.26/plugins/extra/numerated-headers/README
-drwxr-xr-x   0 lucjean    (501) staff       (20)        0 2019-08-30 10:39:53.000000 coop_html_editor-1.3.1/coop_html_editor/static/aloha.0.23.26/plugins/extra/numerated-headers/img/
--rw-r--r--   0 lucjean    (501) staff       (20)      136 2019-08-29 13:07:41.000000 coop_html_editor-1.3.1/coop_html_editor/static/aloha.0.23.26/plugins/extra/numerated-headers/img/headers.png
-drwxr-xr-x   0 lucjean    (501) staff       (20)        0 2019-08-30 10:39:49.000000 coop_html_editor-1.3.1/coop_html_editor/static/aloha.0.23.26/plugins/extra/headerids/
-drwxr-xr-x   0 lucjean    (501) staff       (20)        0 2019-08-30 10:39:49.000000 coop_html_editor-1.3.1/coop_html_editor/static/aloha.0.23.26/plugins/extra/headerids/css/
--rw-r--r--   0 lucjean    (501) staff       (20)      271 2019-08-29 13:07:40.000000 coop_html_editor-1.3.1/coop_html_editor/static/aloha.0.23.26/plugins/extra/headerids/css/headerids.css
-drwxr-xr-x   0 lucjean    (501) staff       (20)        0 2019-08-30 10:39:35.000000 coop_html_editor-1.3.1/coop_html_editor/static/aloha.0.23.26/plugins/extra/headerids/nls/
-drwxr-xr-x   0 lucjean    (501) staff       (20)        0 2019-08-30 10:39:50.000000 coop_html_editor-1.3.1/coop_html_editor/static/aloha.0.23.26/plugins/extra/headerids/nls/zh-hans/
--rw-r--r--   0 lucjean    (501) staff       (20)      163 2019-08-29 13:07:40.000000 coop_html_editor-1.3.1/coop_html_editor/static/aloha.0.23.26/plugins/extra/headerids/nls/zh-hans/i18n.js
-drwxr-xr-x   0 lucjean    (501) staff       (20)        0 2019-08-30 10:39:49.000000 coop_html_editor-1.3.1/coop_html_editor/static/aloha.0.23.26/plugins/extra/headerids/nls/ca/
--rw-r--r--   0 lucjean    (501) staff       (20)      171 2019-08-29 13:07:40.000000 coop_html_editor-1.3.1/coop_html_editor/static/aloha.0.23.26/plugins/extra/headerids/nls/ca/i18n.js
-drwxr-xr-x   0 lucjean    (501) staff       (20)        0 2019-08-30 10:39:50.000000 coop_html_editor-1.3.1/coop_html_editor/static/aloha.0.23.26/plugins/extra/headerids/nls/ru/
--rw-r--r--   0 lucjean    (501) staff       (20)      217 2019-08-29 13:07:40.000000 coop_html_editor-1.3.1/coop_html_editor/static/aloha.0.23.26/plugins/extra/headerids/nls/ru/i18n.js
-drwxr-xr-x   0 lucjean    (501) staff       (20)        0 2019-08-30 10:39:50.000000 coop_html_editor-1.3.1/coop_html_editor/static/aloha.0.23.26/plugins/extra/headerids/nls/uk/
--rw-r--r--   0 lucjean    (501) staff       (20)      209 2019-08-29 13:07:40.000000 coop_html_editor-1.3.1/coop_html_editor/static/aloha.0.23.26/plugins/extra/headerids/nls/uk/i18n.js
-drwxr-xr-x   0 lucjean    (501) staff       (20)        0 2019-08-30 10:39:50.000000 coop_html_editor-1.3.1/coop_html_editor/static/aloha.0.23.26/plugins/extra/headerids/nls/mk/
--rw-r--r--   0 lucjean    (501) staff       (20)      197 2019-08-29 13:07:40.000000 coop_html_editor-1.3.1/coop_html_editor/static/aloha.0.23.26/plugins/extra/headerids/nls/mk/i18n.js
-drwxr-xr-x   0 lucjean    (501) staff       (20)        0 2019-08-30 10:39:50.000000 coop_html_editor-1.3.1/coop_html_editor/static/aloha.0.23.26/plugins/extra/headerids/nls/pt-br/
--rw-r--r--   0 lucjean    (501) staff       (20)      165 2019-08-29 13:07:40.000000 coop_html_editor-1.3.1/coop_html_editor/static/aloha.0.23.26/plugins/extra/headerids/nls/pt-br/i18n.js
-drwxr-xr-x   0 lucjean    (501) staff       (20)        0 2019-08-30 10:39:49.000000 coop_html_editor-1.3.1/coop_html_editor/static/aloha.0.23.26/plugins/extra/headerids/nls/de/
--rw-r--r--   0 lucjean    (501) staff       (20)      166 2019-08-29 13:07:40.000000 coop_html_editor-1.3.1/coop_html_editor/static/aloha.0.23.26/plugins/extra/headerids/nls/de/i18n.js
--rw-r--r--   0 lucjean    (501) staff       (20)        0 2019-08-29 13:07:40.000000 coop_html_editor-1.3.1/coop_html_editor/static/aloha.0.23.26/plugins/extra/headerids/README
-drwxr-xr-x   0 lucjean    (501) staff       (20)        0 2019-08-30 10:39:50.000000 coop_html_editor-1.3.1/coop_html_editor/static/aloha.0.23.26/plugins/extra/hints/
-drwxr-xr-x   0 lucjean    (501) staff       (20)        0 2019-08-30 10:39:50.000000 coop_html_editor-1.3.1/coop_html_editor/static/aloha.0.23.26/plugins/extra/hints/css/
--rw-r--r--   0 lucjean    (501) staff       (20)     2134 2019-08-29 13:07:40.000000 coop_html_editor-1.3.1/coop_html_editor/static/aloha.0.23.26/plugins/extra/hints/css/hints.css
--rw-r--r--   0 lucjean    (501) staff       (20)      431 2019-08-29 13:07:40.000000 coop_html_editor-1.3.1/coop_html_editor/static/aloha.0.23.26/plugins/extra/hints/README.md
--rw-r--r--   0 lucjean    (501) staff       (20)       91 2019-08-29 13:07:40.000000 coop_html_editor-1.3.1/coop_html_editor/static/aloha.0.23.26/plugins/extra/hints/package.json
-drwxr-xr-x   0 lucjean    (501) staff       (20)        0 2019-08-30 10:39:50.000000 coop_html_editor-1.3.1/coop_html_editor/static/aloha.0.23.26/plugins/extra/hints/lib/
--rw-r--r--   0 lucjean    (501) staff       (20)     3656 2019-08-29 13:07:40.000000 coop_html_editor-1.3.1/coop_html_editor/static/aloha.0.23.26/plugins/extra/hints/lib/hints-plugin.js
-drwxr-xr-x   0 lucjean    (501) staff       (20)        0 2019-08-30 10:39:50.000000 coop_html_editor-1.3.1/coop_html_editor/static/aloha.0.23.26/plugins/extra/hints/vendor/
--rw-r--r--   0 lucjean    (501) staff       (20)     9358 2019-08-29 13:07:40.000000 coop_html_editor-1.3.1/coop_html_editor/static/aloha.0.23.26/plugins/extra/hints/vendor/tipsy.js
-drwxr-xr-x   0 lucjean    (501) staff       (20)        0 2019-08-30 10:39:35.000000 coop_html_editor-1.3.1/coop_html_editor/static/aloha.0.23.26/plugins/extra/validation/
-drwxr-xr-x   0 lucjean    (501) staff       (20)        0 2019-08-30 10:39:54.000000 coop_html_editor-1.3.1/coop_html_editor/static/aloha.0.23.26/plugins/extra/validation/lib/
--rw-r--r--   0 lucjean    (501) staff       (20)     7189 2019-08-29 13:07:41.000000 coop_html_editor-1.3.1/coop_html_editor/static/aloha.0.23.26/plugins/extra/validation/lib/validation-plugin.js
--rw-r--r--   0 lucjean    (501) staff       (20)     5710 2019-08-29 13:07:37.000000 coop_html_editor-1.3.1/coop_html_editor/static/aloha.0.23.26/build.txt
-drwxr-xr-x   0 lucjean    (501) staff       (20)        0 2019-08-30 10:39:38.000000 coop_html_editor-1.3.1/coop_html_editor/static/aloha.0.23.26/img/
--rw-r--r--   0 lucjean    (501) staff       (20)      226 2019-08-29 13:07:38.000000 coop_html_editor-1.3.1/coop_html_editor/static/aloha.0.23.26/img/breadcrumb-divider.png
--rw-r--r--   0 lucjean    (501) staff       (20)     2492 2019-08-29 13:07:38.000000 coop_html_editor-1.3.1/coop_html_editor/static/aloha.0.23.26/img/base-multi.png
--rw-r--r--   0 lucjean    (501) staff       (20)      333 2019-08-29 13:07:38.000000 coop_html_editor-1.3.1/coop_html_editor/static/aloha.0.23.26/img/pin.png
--rw-r--r--   0 lucjean    (501) staff       (20)      123 2019-08-29 13:07:38.000000 coop_html_editor-1.3.1/coop_html_editor/static/aloha.0.23.26/img/maximize.png
--rw-r--r--   0 lucjean    (501) staff       (20)      288 2019-08-29 13:07:38.000000 coop_html_editor-1.3.1/coop_html_editor/static/aloha.0.23.26/img/text_indent_remove.png
--rw-r--r--   0 lucjean    (501) staff       (20)      207 2019-08-29 13:07:38.000000 coop_html_editor-1.3.1/coop_html_editor/static/aloha.0.23.26/img/multisplit-open.gif
--rw-r--r--   0 lucjean    (501) staff       (20)      210 2019-08-29 13:07:38.000000 coop_html_editor-1.3.1/coop_html_editor/static/aloha.0.23.26/img/multisplit-close.gif
--rw-r--r--   0 lucjean    (501) staff       (20)      494 2019-08-29 13:07:38.000000 coop_html_editor-1.3.1/coop_html_editor/static/aloha.0.23.26/img/arrow.png
--rw-r--r--   0 lucjean    (501) staff       (20)      276 2019-08-29 13:07:38.000000 coop_html_editor-1.3.1/coop_html_editor/static/aloha.0.23.26/img/arrow-down.png
--rw-r--r--   0 lucjean    (501) staff       (20)      112 2019-08-29 13:07:38.000000 coop_html_editor-1.3.1/coop_html_editor/static/aloha.0.23.26/img/grabhandle.png
--rw-r--r--   0 lucjean    (501) staff       (20)      273 2019-08-29 13:07:38.000000 coop_html_editor-1.3.1/coop_html_editor/static/aloha.0.23.26/img/arrow-left.png
--rw-r--r--   0 lucjean    (501) staff       (20)      929 2019-08-29 13:07:38.000000 coop_html_editor-1.3.1/coop_html_editor/static/aloha.0.23.26/img/multisplit-base.jpg
--rw-r--r--   0 lucjean    (501) staff       (20)      193 2019-08-29 13:07:38.000000 coop_html_editor-1.3.1/coop_html_editor/static/aloha.0.23.26/img/removeformat.png
--rw-r--r--   0 lucjean    (501) staff       (20)     5832 2019-08-29 13:07:38.000000 coop_html_editor-1.3.1/coop_html_editor/static/aloha.0.23.26/img/base.png
--rw-r--r--   0 lucjean    (501) staff       (20)      290 2019-08-29 13:07:38.000000 coop_html_editor-1.3.1/coop_html_editor/static/aloha.0.23.26/img/text_indent.png
--rw-r--r--   0 lucjean    (501) staff       (20)   205446 2019-08-29 13:07:38.000000 coop_html_editor-1.3.1/coop_html_editor/static/aloha.0.23.26/img/bg.png
--rw-r--r--   0 lucjean    (501) staff       (20)     2014 2019-08-29 13:07:38.000000 coop_html_editor-1.3.1/coop_html_editor/static/aloha.0.23.26/img/gentics-logo.png
--rw-r--r--   0 lucjean    (501) staff       (20)      899 2019-08-29 13:07:38.000000 coop_html_editor-1.3.1/coop_html_editor/static/aloha.0.23.26/package.json
-drwxr-xr-x   0 lucjean    (501) staff       (20)        0 2019-08-30 10:39:38.000000 coop_html_editor-1.3.1/coop_html_editor/static/aloha.0.23.26/lib/
-drwxr-xr-x   0 lucjean    (501) staff       (20)        0 2019-08-30 10:39:39.000000 coop_html_editor-1.3.1/coop_html_editor/static/aloha.0.23.26/lib/util/
--rw-r--r--   0 lucjean    (501) staff       (20)     2955 2019-08-29 13:07:38.000000 coop_html_editor-1.3.1/coop_html_editor/static/aloha.0.23.26/lib/util/boundary-markers.js
--rw-r--r--   0 lucjean    (501) staff       (20)    26731 2019-08-29 13:07:38.000000 coop_html_editor-1.3.1/coop_html_editor/static/aloha.0.23.26/lib/util/range-context.js
--rw-r--r--   0 lucjean    (501) staff       (20)  1310361 2019-08-29 13:07:38.000000 coop_html_editor-1.3.1/coop_html_editor/static/aloha.0.23.26/lib/aloha-full.min.js
--rw-r--r--   0 lucjean    (501) staff       (20)  1199591 2019-08-29 13:07:38.000000 coop_html_editor-1.3.1/coop_html_editor/static/aloha.0.23.26/lib/aloha-bare.min.js
--rw-r--r--   0 lucjean    (501) staff       (20)  3222235 2019-08-29 13:07:38.000000 coop_html_editor-1.3.1/coop_html_editor/static/aloha.0.23.26/lib/aloha-full.js
--rw-r--r--   0 lucjean    (501) staff       (20)    81039 2019-08-29 13:07:38.000000 coop_html_editor-1.3.1/coop_html_editor/static/aloha.0.23.26/lib/require.js
-drwxr-xr-x   0 lucjean    (501) staff       (20)        0 2019-08-30 10:39:35.000000 coop_html_editor-1.3.1/coop_html_editor/static/aloha.0.23.26/lib/aloha/
-drwxr-xr-x   0 lucjean    (501) staff       (20)        0 2019-08-30 10:39:35.000000 coop_html_editor-1.3.1/coop_html_editor/static/aloha.0.23.26/lib/aloha/nls/
-drwxr-xr-x   0 lucjean    (501) staff       (20)        0 2019-08-30 10:39:38.000000 coop_html_editor-1.3.1/coop_html_editor/static/aloha.0.23.26/lib/aloha/nls/zh-hans/
--rw-r--r--   0 lucjean    (501) staff       (20)      332 2019-08-29 13:07:38.000000 coop_html_editor-1.3.1/coop_html_editor/static/aloha.0.23.26/lib/aloha/nls/zh-hans/i18n.js
-drwxr-xr-x   0 lucjean    (501) staff       (20)        0 2019-08-30 10:39:38.000000 coop_html_editor-1.3.1/coop_html_editor/static/aloha.0.23.26/lib/aloha/nls/ca/
--rw-r--r--   0 lucjean    (501) staff       (20)      377 2019-08-29 13:07:38.000000 coop_html_editor-1.3.1/coop_html_editor/static/aloha.0.23.26/lib/aloha/nls/ca/i18n.js
-drwxr-xr-x   0 lucjean    (501) staff       (20)        0 2019-08-30 10:39:38.000000 coop_html_editor-1.3.1/coop_html_editor/static/aloha.0.23.26/lib/aloha/nls/ru/
--rw-r--r--   0 lucjean    (501) staff       (20)      441 2019-08-29 13:07:38.000000 coop_html_editor-1.3.1/coop_html_editor/static/aloha.0.23.26/lib/aloha/nls/ru/i18n.js
-drwxr-xr-x   0 lucjean    (501) staff       (20)        0 2019-08-30 10:39:38.000000 coop_html_editor-1.3.1/coop_html_editor/static/aloha.0.23.26/lib/aloha/nls/uk/
--rw-r--r--   0 lucjean    (501) staff       (20)      453 2019-08-29 13:07:38.000000 coop_html_editor-1.3.1/coop_html_editor/static/aloha.0.23.26/lib/aloha/nls/uk/i18n.js
-drwxr-xr-x   0 lucjean    (501) staff       (20)        0 2019-08-30 10:39:38.000000 coop_html_editor-1.3.1/coop_html_editor/static/aloha.0.23.26/lib/aloha/nls/mk/
--rw-r--r--   0 lucjean    (501) staff       (20)      405 2019-08-29 13:07:38.000000 coop_html_editor-1.3.1/coop_html_editor/static/aloha.0.23.26/lib/aloha/nls/mk/i18n.js
-drwxr-xr-x   0 lucjean    (501) staff       (20)        0 2019-08-30 10:39:38.000000 coop_html_editor-1.3.1/coop_html_editor/static/aloha.0.23.26/lib/aloha/nls/pt-br/
--rw-r--r--   0 lucjean    (501) staff       (20)      360 2019-08-29 13:07:38.000000 coop_html_editor-1.3.1/coop_html_editor/static/aloha.0.23.26/lib/aloha/nls/pt-br/i18n.js
-drwxr-xr-x   0 lucjean    (501) staff       (20)        0 2019-08-30 10:39:38.000000 coop_html_editor-1.3.1/coop_html_editor/static/aloha.0.23.26/lib/aloha/nls/de/
--rw-r--r--   0 lucjean    (501) staff       (20)      367 2019-08-29 13:07:38.000000 coop_html_editor-1.3.1/coop_html_editor/static/aloha.0.23.26/lib/aloha/nls/de/i18n.js
--rw-r--r--   0 lucjean    (501) staff       (20)  1199591 2019-08-29 13:07:38.000000 coop_html_editor-1.3.1/coop_html_editor/static/aloha.0.23.26/lib/aloha.js
--rw-r--r--   0 lucjean    (501) staff       (20)    14274 2019-08-29 13:07:38.000000 coop_html_editor-1.3.1/coop_html_editor/static/aloha.0.23.26/lib/css.js
--rw-r--r--   0 lucjean    (501) staff       (20)  2887024 2019-08-29 13:07:38.000000 coop_html_editor-1.3.1/coop_html_editor/static/aloha.0.23.26/lib/aloha-bare.js
--rw-r--r--   0 lucjean    (501) staff       (20)    12511 2019-08-29 13:07:38.000000 coop_html_editor-1.3.1/coop_html_editor/static/aloha.0.23.26/lib/text.js
-drwxr-xr-x   0 lucjean    (501) staff       (20)        0 2019-08-30 10:39:39.000000 coop_html_editor-1.3.1/coop_html_editor/static/aloha.0.23.26/lib/vendor/
-drwxr-xr-x   0 lucjean    (501) staff       (20)        0 2019-08-30 10:39:35.000000 coop_html_editor-1.3.1/coop_html_editor/static/aloha.0.23.26/lib/vendor/repository-browser/
-drwxr-xr-x   0 lucjean    (501) staff       (20)        0 2019-08-30 10:39:39.000000 coop_html_editor-1.3.1/coop_html_editor/static/aloha.0.23.26/lib/vendor/repository-browser/css/
--rw-r--r--   0 lucjean    (501) staff       (20)     2957 2019-08-29 13:07:38.000000 coop_html_editor-1.3.1/coop_html_editor/static/aloha.0.23.26/lib/vendor/repository-browser/css/jstree.css
--rw-r--r--   0 lucjean    (501) staff       (20)    21932 2019-08-29 13:07:38.000000 coop_html_editor-1.3.1/coop_html_editor/static/aloha.0.23.26/lib/vendor/repository-browser/css/repository-browser.css
-drwxr-xr-x   0 lucjean    (501) staff       (20)        0 2019-08-30 10:39:39.000000 coop_html_editor-1.3.1/coop_html_editor/static/aloha.0.23.26/lib/vendor/repository-browser/js/
--rw-r--r--   0 lucjean    (501) staff       (20)    17352 2019-08-29 13:07:38.000000 coop_html_editor-1.3.1/coop_html_editor/static/aloha.0.23.26/lib/vendor/repository-browser/js/repository-browser.js
-drwxr-xr-x   0 lucjean    (501) staff       (20)        0 2019-08-30 10:39:39.000000 coop_html_editor-1.3.1/coop_html_editor/static/aloha.0.23.26/lib/vendor/repository-browser/img/
--rw-r--r--   0 lucjean    (501) staff       (20)      402 2019-08-29 13:07:38.000000 coop_html_editor-1.3.1/coop_html_editor/static/aloha.0.23.26/lib/vendor/repository-browser/img/sort-alphabet-descending.png
--rw-r--r--   0 lucjean    (501) staff       (20)      465 2019-08-29 13:07:38.000000 coop_html_editor-1.3.1/coop_html_editor/static/aloha.0.23.26/lib/vendor/repository-browser/img/folder-horizontal-open.png
--rw-r--r--   0 lucjean    (501) staff       (20)      585 2019-08-29 13:07:38.000000 coop_html_editor-1.3.1/coop_html_editor/static/aloha.0.23.26/lib/vendor/repository-browser/img/folder-open.png
--rw-r--r--   0 lucjean    (501) staff       (20)      606 2019-08-29 13:07:38.000000 coop_html_editor-1.3.1/coop_html_editor/static/aloha.0.23.26/lib/vendor/repository-browser/img/arrow-stop.png
--rw-r--r--   0 lucjean    (501) staff       (20)      404 2019-08-29 13:07:38.000000 coop_html_editor-1.3.1/coop_html_editor/static/aloha.0.23.26/lib/vendor/repository-browser/img/sort-alphabet.png
--rw-r--r--   0 lucjean    (501) staff       (20)      537 2019-08-29 13:07:38.000000 coop_html_editor-1.3.1/coop_html_editor/static/aloha.0.23.26/lib/vendor/repository-browser/img/arrow-180.png
--rw-r--r--   0 lucjean    (501) staff       (20)      531 2019-08-29 13:07:38.000000 coop_html_editor-1.3.1/coop_html_editor/static/aloha.0.23.26/lib/vendor/repository-browser/img/arrow.png
--rw-r--r--   0 lucjean    (501) staff       (20)      256 2019-08-29 13:07:38.000000 coop_html_editor-1.3.1/coop_html_editor/static/aloha.0.23.26/lib/vendor/repository-browser/img/control-stop-square-small.png
--rw-r--r--   0 lucjean    (501) staff       (20)      636 2019-08-29 13:07:38.000000 coop_html_editor-1.3.1/coop_html_editor/static/aloha.0.23.26/lib/vendor/repository-browser/img/magnifier-left.png
--rw-r--r--   0 lucjean    (501) staff       (20)      612 2019-08-29 13:07:38.000000 coop_html_editor-1.3.1/coop_html_editor/static/aloha.0.23.26/lib/vendor/repository-browser/img/arrow-stop-180.png
--rw-r--r--   0 lucjean    (501) staff       (20)      370 2019-08-29 13:07:38.000000 coop_html_editor-1.3.1/coop_html_editor/static/aloha.0.23.26/lib/vendor/repository-browser/img/arrow-000-medium.png
--rw-r--r--   0 lucjean    (501) staff       (20)      582 2019-08-29 13:07:38.000000 coop_html_editor-1.3.1/coop_html_editor/static/aloha.0.23.26/lib/vendor/repository-browser/img/page.png
--rw-r--r--   0 lucjean    (501) staff       (20)     1440 2019-08-29 13:07:38.000000 coop_html_editor-1.3.1/coop_html_editor/static/aloha.0.23.26/lib/vendor/repository-browser/img/throbber.gif
--rw-r--r--   0 lucjean    (501) staff       (20)      553 2019-08-29 13:07:38.000000 coop_html_editor-1.3.1/coop_html_editor/static/aloha.0.23.26/lib/vendor/repository-browser/img/picture.png
--rw-r--r--   0 lucjean    (501) staff       (20)      327 2019-08-29 13:07:38.000000 coop_html_editor-1.3.1/coop_html_editor/static/aloha.0.23.26/lib/vendor/repository-browser/img/arrow-315-medium.png
--rw-r--r--   0 lucjean    (501) staff       (20)    17967 2019-08-29 13:07:38.000000 coop_html_editor-1.3.1/coop_html_editor/static/aloha.0.23.26/lib/vendor/ierange-m2.js
--rw-r--r--   0 lucjean    (501) staff       (20)     2567 2019-08-29 13:07:38.000000 coop_html_editor-1.3.1/coop_html_editor/static/aloha.0.23.26/lib/vendor/3rdparty.txt
--rw-r--r--   0 lucjean    (501) staff       (20)   216748 2019-08-29 13:07:38.000000 coop_html_editor-1.3.1/coop_html_editor/static/aloha.0.23.26/lib/vendor/jquery-1.5.1.js
--rw-r--r--   0 lucjean    (501) staff       (20)   253493 2019-08-29 13:07:38.000000 coop_html_editor-1.3.1/coop_html_editor/static/aloha.0.23.26/lib/vendor/jquery-1.7.2.js
--rw-r--r--   0 lucjean    (501) staff       (20)   248235 2019-08-29 13:07:38.000000 coop_html_editor-1.3.1/coop_html_editor/static/aloha.0.23.26/lib/vendor/jquery-1.7.1.js
--rw-r--r--   0 lucjean    (501) staff       (20)   235603 2019-08-29 13:07:38.000000 coop_html_editor-1.3.1/coop_html_editor/static/aloha.0.23.26/lib/vendor/jquery-1.6.1.js
--rw-r--r--   0 lucjean    (501) staff       (20)     3892 2019-08-29 13:07:38.000000 coop_html_editor-1.3.1/coop_html_editor/static/aloha.0.23.26/lib/vendor/grid.locale.en.js
-drwxr-xr-x   0 lucjean    (501) staff       (20)        0 2019-08-30 10:39:35.000000 coop_html_editor-1.3.1/coop_html_editor/static/aloha.0.23.26/lib/vendor/pubsub/
-drwxr-xr-x   0 lucjean    (501) staff       (20)        0 2019-08-30 10:39:39.000000 coop_html_editor-1.3.1/coop_html_editor/static/aloha.0.23.26/lib/vendor/pubsub/js/
--rw-r--r--   0 lucjean    (501) staff       (20)      619 2019-08-29 13:07:38.000000 coop_html_editor-1.3.1/coop_html_editor/static/aloha.0.23.26/lib/vendor/pubsub/js/pubsub.js
--rw-r--r--   0 lucjean    (501) staff       (20)     4421 2019-08-29 13:07:38.000000 coop_html_editor-1.3.1/coop_html_editor/static/aloha.0.23.26/lib/vendor/grid.locale.de.js
--rw-r--r--   0 lucjean    (501) staff       (20)   232636 2019-08-29 13:07:38.000000 coop_html_editor-1.3.1/coop_html_editor/static/aloha.0.23.26/lib/vendor/jquery-1.6.js
--rw-r--r--   0 lucjean    (501) staff       (20)      679 2019-08-29 13:07:38.000000 coop_html_editor-1.3.1/coop_html_editor/static/aloha.0.23.26/lib/aloha-jquery-noconflict.js
--rw-r--r--   0 lucjean    (501) staff       (20)     4090 2019-08-29 13:36:08.000000 coop_html_editor-1.3.1/coop_html_editor/settings.py
-drwxr-xr-x   0 lucjean    (501) staff       (20)        0 2019-08-30 10:39:35.000000 coop_html_editor-1.3.1/coop_html_editor/templates/
-drwxr-xr-x   0 lucjean    (501) staff       (20)        0 2019-08-30 10:40:05.000000 coop_html_editor-1.3.1/coop_html_editor/templates/html_editor/
--rw-r--r--   0 lucjean    (501) staff       (20)     2675 2019-08-29 13:07:46.000000 coop_html_editor-1.3.1/coop_html_editor/templates/html_editor/image_browser.html
--rw-r--r--   0 lucjean    (501) staff       (20)     3307 2019-08-29 13:07:46.000000 coop_html_editor-1.3.1/coop_html_editor/templates/html_editor/link_browser.html
--rw-r--r--   0 lucjean    (501) staff       (20)      249 2019-08-29 13:07:46.000000 coop_html_editor-1.3.1/coop_html_editor/templates/html_editor/aloha_input.html
--rw-r--r--   0 lucjean    (501) staff       (20)     6338 2019-08-29 13:07:46.000000 coop_html_editor-1.3.1/coop_html_editor/templates/html_editor/aloha_init.js
--rw-r--r--   0 lucjean    (501) staff       (20)      247 2019-08-29 13:07:46.000000 coop_html_editor-1.3.1/coop_html_editor/templates/html_editor/ckeditor_input.html
--rw-r--r--   0 lucjean    (501) staff       (20)     1404 2019-08-29 13:07:46.000000 coop_html_editor-1.3.1/coop_html_editor/templates/html_editor/ckeditor_config.js
--rw-r--r--   0 lucjean    (501) staff       (20)     2454 2019-08-29 13:07:46.000000 coop_html_editor-1.3.1/coop_html_editor/templates/html_editor/ckeditor-init.js
--rw-r--r--   0 lucjean    (501) staff       (20)      464 2019-08-29 13:07:46.000000 coop_html_editor-1.3.1/coop_html_editor/urls.py
--rw-r--r--   0 lucjean    (501) staff       (20)     2739 2019-08-29 13:07:46.000000 coop_html_editor-1.3.1/coop_html_editor/views.py
--rw-r--r--   0 lucjean    (501) staff       (20)      171 2019-08-29 13:07:37.000000 coop_html_editor-1.3.1/MANIFEST.in
--rw-r--r--   0 lucjean    (501) staff       (20)      756 2019-08-29 13:07:46.000000 coop_html_editor-1.3.1/setup.py
--rw-r--r--   0 lucjean    (501) staff       (20)       38 2019-08-30 10:40:05.000000 coop_html_editor-1.3.1/setup.cfg
--rw-r--r--   0 lucjean    (501) staff       (20)     4938 2019-08-30 10:38:50.000000 coop_html_editor-1.3.1/README.rst
+drwxrwxr-x   0 lucjean   (1001) lucjean   (1001)        0 2023-06-12 12:55:08.827913 coop_html_editor-1.4.1/
+-rw-rw-r--   0 lucjean   (1001) lucjean   (1001)      171 2023-05-22 07:01:38.000000 coop_html_editor-1.4.1/MANIFEST.in
+-rw-rw-r--   0 lucjean   (1001) lucjean   (1001)     5228 2023-06-12 12:55:08.827913 coop_html_editor-1.4.1/PKG-INFO
+-rw-rw-r--   0 lucjean   (1001) lucjean   (1001)     4938 2023-05-22 13:08:00.000000 coop_html_editor-1.4.1/README.rst
+drwxrwxr-x   0 lucjean   (1001) lucjean   (1001)        0 2023-06-12 12:55:08.707913 coop_html_editor-1.4.1/coop_html_editor/
+-rw-rw-r--   0 lucjean   (1001) lucjean   (1001)      340 2023-06-12 12:48:33.000000 coop_html_editor-1.4.1/coop_html_editor/__init__.py
+-rw-rw-r--   0 lucjean   (1001) lucjean   (1001)      189 2023-05-22 07:01:38.000000 coop_html_editor-1.4.1/coop_html_editor/apps.py
+-rw-rw-r--   0 lucjean   (1001) lucjean   (1001)     1810 2023-06-12 12:48:33.000000 coop_html_editor-1.4.1/coop_html_editor/forms.py
+drwxrwxr-x   0 lucjean   (1001) lucjean   (1001)        0 2023-06-12 12:55:08.703912 coop_html_editor-1.4.1/coop_html_editor/locale/
+drwxrwxr-x   0 lucjean   (1001) lucjean   (1001)        0 2023-06-12 12:55:08.703912 coop_html_editor-1.4.1/coop_html_editor/locale/fr/
+drwxrwxr-x   0 lucjean   (1001) lucjean   (1001)        0 2023-06-12 12:55:08.711912 coop_html_editor-1.4.1/coop_html_editor/locale/fr/LC_MESSAGES/
+-rw-rw-r--   0 lucjean   (1001) lucjean   (1001)      673 2023-05-22 07:01:38.000000 coop_html_editor-1.4.1/coop_html_editor/locale/fr/LC_MESSAGES/django.mo
+-rw-rw-r--   0 lucjean   (1001) lucjean   (1001)     1531 2023-05-22 07:01:38.000000 coop_html_editor-1.4.1/coop_html_editor/locale/fr/LC_MESSAGES/django.po
+-rw-rw-r--   0 lucjean   (1001) lucjean   (1001)     2118 2023-06-12 12:48:33.000000 coop_html_editor-1.4.1/coop_html_editor/settings.py
+drwxrwxr-x   0 lucjean   (1001) lucjean   (1001)        0 2023-06-12 12:55:08.707913 coop_html_editor-1.4.1/coop_html_editor/static/
+drwxrwxr-x   0 lucjean   (1001) lucjean   (1001)        0 2023-06-12 12:55:08.711912 coop_html_editor-1.4.1/coop_html_editor/static/ckeditor.4.6.2/
+-rw-rw-r--   0 lucjean   (1001) lucjean   (1001)   153288 2023-05-22 07:01:38.000000 coop_html_editor-1.4.1/coop_html_editor/static/ckeditor.4.6.2/CHANGES.md
+-rw-rw-r--   0 lucjean   (1001) lucjean   (1001)    76251 2023-05-22 07:01:38.000000 coop_html_editor-1.4.1/coop_html_editor/static/ckeditor.4.6.2/LICENSE.md
+-rw-rw-r--   0 lucjean   (1001) lucjean   (1001)     1342 2023-05-22 07:01:38.000000 coop_html_editor-1.4.1/coop_html_editor/static/ckeditor.4.6.2/README.md
+drwxrwxr-x   0 lucjean   (1001) lucjean   (1001)        0 2023-06-12 12:55:08.711912 coop_html_editor-1.4.1/coop_html_editor/static/ckeditor.4.6.2/adapters/
+-rw-rw-r--   0 lucjean   (1001) lucjean   (1001)     3179 2023-05-22 07:01:38.000000 coop_html_editor-1.4.1/coop_html_editor/static/ckeditor.4.6.2/adapters/jquery.js
+-rw-rw-r--   0 lucjean   (1001) lucjean   (1001)     2173 2023-05-22 07:01:38.000000 coop_html_editor-1.4.1/coop_html_editor/static/ckeditor.4.6.2/build-config.js
+-rw-rw-r--   0 lucjean   (1001) lucjean   (1001)   535544 2023-05-22 07:01:38.000000 coop_html_editor-1.4.1/coop_html_editor/static/ckeditor.4.6.2/ckeditor.js
+-rw-rw-r--   0 lucjean   (1001) lucjean   (1001)     1321 2023-05-22 07:01:38.000000 coop_html_editor-1.4.1/coop_html_editor/static/ckeditor.4.6.2/config.js
+-rw-rw-r--   0 lucjean   (1001) lucjean   (1001)     2955 2023-05-22 07:01:38.000000 coop_html_editor-1.4.1/coop_html_editor/static/ckeditor.4.6.2/contents.css
+drwxrwxr-x   0 lucjean   (1001) lucjean   (1001)        0 2023-06-12 12:55:08.711912 coop_html_editor-1.4.1/coop_html_editor/static/ckeditor.4.6.2/lang/
+-rw-rw-r--   0 lucjean   (1001) lucjean   (1001)    11251 2023-05-22 07:01:38.000000 coop_html_editor-1.4.1/coop_html_editor/static/ckeditor.4.6.2/lang/en.js
+-rw-rw-r--   0 lucjean   (1001) lucjean   (1001)    13074 2023-05-22 07:01:38.000000 coop_html_editor-1.4.1/coop_html_editor/static/ckeditor.4.6.2/lang/fr.js
+drwxrwxr-x   0 lucjean   (1001) lucjean   (1001)        0 2023-06-12 12:55:08.711912 coop_html_editor-1.4.1/coop_html_editor/static/ckeditor.4.6.2/plugins/
+drwxrwxr-x   0 lucjean   (1001) lucjean   (1001)        0 2023-06-12 12:55:08.703912 coop_html_editor-1.4.1/coop_html_editor/static/ckeditor.4.6.2/plugins/a11yhelp/
+drwxrwxr-x   0 lucjean   (1001) lucjean   (1001)        0 2023-06-12 12:55:08.711912 coop_html_editor-1.4.1/coop_html_editor/static/ckeditor.4.6.2/plugins/a11yhelp/dialogs/
+-rw-rw-r--   0 lucjean   (1001) lucjean   (1001)     2879 2023-05-22 07:01:38.000000 coop_html_editor-1.4.1/coop_html_editor/static/ckeditor.4.6.2/plugins/a11yhelp/dialogs/a11yhelp.js
+drwxrwxr-x   0 lucjean   (1001) lucjean   (1001)        0 2023-06-12 12:55:08.723913 coop_html_editor-1.4.1/coop_html_editor/static/ckeditor.4.6.2/plugins/a11yhelp/dialogs/lang/
+-rw-rw-r--   0 lucjean   (1001) lucjean   (1001)      869 2023-05-22 07:01:38.000000 coop_html_editor-1.4.1/coop_html_editor/static/ckeditor.4.6.2/plugins/a11yhelp/dialogs/lang/_translationstatus.txt
+-rw-rw-r--   0 lucjean   (1001) lucjean   (1001)     3901 2023-05-22 07:01:38.000000 coop_html_editor-1.4.1/coop_html_editor/static/ckeditor.4.6.2/plugins/a11yhelp/dialogs/lang/af.js
+-rw-rw-r--   0 lucjean   (1001) lucjean   (1001)     3875 2023-05-22 07:01:38.000000 coop_html_editor-1.4.1/coop_html_editor/static/ckeditor.4.6.2/plugins/a11yhelp/dialogs/lang/ar.js
+-rw-rw-r--   0 lucjean   (1001) lucjean   (1001)     4194 2023-05-22 07:01:38.000000 coop_html_editor-1.4.1/coop_html_editor/static/ckeditor.4.6.2/plugins/a11yhelp/dialogs/lang/az.js
+-rw-rw-r--   0 lucjean   (1001) lucjean   (1001)     3859 2023-05-22 07:01:38.000000 coop_html_editor-1.4.1/coop_html_editor/static/ckeditor.4.6.2/plugins/a11yhelp/dialogs/lang/bg.js
+-rw-rw-r--   0 lucjean   (1001) lucjean   (1001)     4657 2023-05-22 07:01:38.000000 coop_html_editor-1.4.1/coop_html_editor/static/ckeditor.4.6.2/plugins/a11yhelp/dialogs/lang/ca.js
+-rw-rw-r--   0 lucjean   (1001) lucjean   (1001)     4714 2023-05-22 07:01:38.000000 coop_html_editor-1.4.1/coop_html_editor/static/ckeditor.4.6.2/plugins/a11yhelp/dialogs/lang/cs.js
+-rw-rw-r--   0 lucjean   (1001) lucjean   (1001)     4134 2023-05-22 07:01:38.000000 coop_html_editor-1.4.1/coop_html_editor/static/ckeditor.4.6.2/plugins/a11yhelp/dialogs/lang/cy.js
+-rw-rw-r--   0 lucjean   (1001) lucjean   (1001)     4030 2023-05-22 07:01:38.000000 coop_html_editor-1.4.1/coop_html_editor/static/ckeditor.4.6.2/plugins/a11yhelp/dialogs/lang/da.js
+-rw-rw-r--   0 lucjean   (1001) lucjean   (1001)     4447 2023-05-22 07:01:38.000000 coop_html_editor-1.4.1/coop_html_editor/static/ckeditor.4.6.2/plugins/a11yhelp/dialogs/lang/de-ch.js
+-rw-rw-r--   0 lucjean   (1001) lucjean   (1001)     4444 2023-05-22 07:01:38.000000 coop_html_editor-1.4.1/coop_html_editor/static/ckeditor.4.6.2/plugins/a11yhelp/dialogs/lang/de.js
+-rw-rw-r--   0 lucjean   (1001) lucjean   (1001)     6879 2023-05-22 07:01:38.000000 coop_html_editor-1.4.1/coop_html_editor/static/ckeditor.4.6.2/plugins/a11yhelp/dialogs/lang/el.js
+-rw-rw-r--   0 lucjean   (1001) lucjean   (1001)     3861 2023-05-22 07:01:38.000000 coop_html_editor-1.4.1/coop_html_editor/static/ckeditor.4.6.2/plugins/a11yhelp/dialogs/lang/en-gb.js
+-rw-rw-r--   0 lucjean   (1001) lucjean   (1001)     3858 2023-05-22 07:01:38.000000 coop_html_editor-1.4.1/coop_html_editor/static/ckeditor.4.6.2/plugins/a11yhelp/dialogs/lang/en.js
+-rw-rw-r--   0 lucjean   (1001) lucjean   (1001)     4660 2023-05-22 07:01:38.000000 coop_html_editor-1.4.1/coop_html_editor/static/ckeditor.4.6.2/plugins/a11yhelp/dialogs/lang/eo.js
+-rw-rw-r--   0 lucjean   (1001) lucjean   (1001)     4669 2023-05-22 07:01:38.000000 coop_html_editor-1.4.1/coop_html_editor/static/ckeditor.4.6.2/plugins/a11yhelp/dialogs/lang/es.js
+-rw-rw-r--   0 lucjean   (1001) lucjean   (1001)     3867 2023-05-22 07:01:38.000000 coop_html_editor-1.4.1/coop_html_editor/static/ckeditor.4.6.2/plugins/a11yhelp/dialogs/lang/et.js
+-rw-rw-r--   0 lucjean   (1001) lucjean   (1001)     4360 2023-05-22 07:01:38.000000 coop_html_editor-1.4.1/coop_html_editor/static/ckeditor.4.6.2/plugins/a11yhelp/dialogs/lang/eu.js
+-rw-rw-r--   0 lucjean   (1001) lucjean   (1001)     5715 2023-05-22 07:01:38.000000 coop_html_editor-1.4.1/coop_html_editor/static/ckeditor.4.6.2/plugins/a11yhelp/dialogs/lang/fa.js
+-rw-rw-r--   0 lucjean   (1001) lucjean   (1001)     4504 2023-05-22 07:01:38.000000 coop_html_editor-1.4.1/coop_html_editor/static/ckeditor.4.6.2/plugins/a11yhelp/dialogs/lang/fi.js
+-rw-rw-r--   0 lucjean   (1001) lucjean   (1001)     3860 2023-05-22 07:01:38.000000 coop_html_editor-1.4.1/coop_html_editor/static/ckeditor.4.6.2/plugins/a11yhelp/dialogs/lang/fo.js
+-rw-rw-r--   0 lucjean   (1001) lucjean   (1001)     4666 2023-05-22 07:01:38.000000 coop_html_editor-1.4.1/coop_html_editor/static/ckeditor.4.6.2/plugins/a11yhelp/dialogs/lang/fr-ca.js
+-rw-rw-r--   0 lucjean   (1001) lucjean   (1001)     5155 2023-05-22 07:01:38.000000 coop_html_editor-1.4.1/coop_html_editor/static/ckeditor.4.6.2/plugins/a11yhelp/dialogs/lang/fr.js
+-rw-rw-r--   0 lucjean   (1001) lucjean   (1001)     4370 2023-05-22 07:01:38.000000 coop_html_editor-1.4.1/coop_html_editor/static/ckeditor.4.6.2/plugins/a11yhelp/dialogs/lang/gl.js
+-rw-rw-r--   0 lucjean   (1001) lucjean   (1001)     4068 2023-05-22 07:01:38.000000 coop_html_editor-1.4.1/coop_html_editor/static/ckeditor.4.6.2/plugins/a11yhelp/dialogs/lang/gu.js
+-rw-rw-r--   0 lucjean   (1001) lucjean   (1001)     4699 2023-05-22 07:01:38.000000 coop_html_editor-1.4.1/coop_html_editor/static/ckeditor.4.6.2/plugins/a11yhelp/dialogs/lang/he.js
+-rw-rw-r--   0 lucjean   (1001) lucjean   (1001)     3872 2023-05-22 07:01:38.000000 coop_html_editor-1.4.1/coop_html_editor/static/ckeditor.4.6.2/plugins/a11yhelp/dialogs/lang/hi.js
+-rw-rw-r--   0 lucjean   (1001) lucjean   (1001)     4041 2023-05-22 07:01:38.000000 coop_html_editor-1.4.1/coop_html_editor/static/ckeditor.4.6.2/plugins/a11yhelp/dialogs/lang/hr.js
+-rw-rw-r--   0 lucjean   (1001) lucjean   (1001)     4604 2023-05-22 07:01:38.000000 coop_html_editor-1.4.1/coop_html_editor/static/ckeditor.4.6.2/plugins/a11yhelp/dialogs/lang/hu.js
+-rw-rw-r--   0 lucjean   (1001) lucjean   (1001)     3909 2023-05-22 07:01:38.000000 coop_html_editor-1.4.1/coop_html_editor/static/ckeditor.4.6.2/plugins/a11yhelp/dialogs/lang/id.js
+-rw-rw-r--   0 lucjean   (1001) lucjean   (1001)     4805 2023-05-22 07:01:38.000000 coop_html_editor-1.4.1/coop_html_editor/static/ckeditor.4.6.2/plugins/a11yhelp/dialogs/lang/it.js
+-rw-rw-r--   0 lucjean   (1001) lucjean   (1001)     4954 2023-05-22 07:01:38.000000 coop_html_editor-1.4.1/coop_html_editor/static/ckeditor.4.6.2/plugins/a11yhelp/dialogs/lang/ja.js
+-rw-rw-r--   0 lucjean   (1001) lucjean   (1001)     4876 2023-05-22 07:01:38.000000 coop_html_editor-1.4.1/coop_html_editor/static/ckeditor.4.6.2/plugins/a11yhelp/dialogs/lang/km.js
+-rw-rw-r--   0 lucjean   (1001) lucjean   (1001)     5469 2023-05-22 07:01:38.000000 coop_html_editor-1.4.1/coop_html_editor/static/ckeditor.4.6.2/plugins/a11yhelp/dialogs/lang/ko.js
+-rw-rw-r--   0 lucjean   (1001) lucjean   (1001)     5364 2023-05-22 07:01:38.000000 coop_html_editor-1.4.1/coop_html_editor/static/ckeditor.4.6.2/plugins/a11yhelp/dialogs/lang/ku.js
+-rw-rw-r--   0 lucjean   (1001) lucjean   (1001)     3867 2023-05-22 07:01:38.000000 coop_html_editor-1.4.1/coop_html_editor/static/ckeditor.4.6.2/plugins/a11yhelp/dialogs/lang/lt.js
+-rw-rw-r--   0 lucjean   (1001) lucjean   (1001)     4580 2023-05-22 07:01:38.000000 coop_html_editor-1.4.1/coop_html_editor/static/ckeditor.4.6.2/plugins/a11yhelp/dialogs/lang/lv.js
+-rw-rw-r--   0 lucjean   (1001) lucjean   (1001)     4250 2023-05-22 07:01:38.000000 coop_html_editor-1.4.1/coop_html_editor/static/ckeditor.4.6.2/plugins/a11yhelp/dialogs/lang/mk.js
+-rw-rw-r--   0 lucjean   (1001) lucjean   (1001)     3865 2023-05-22 07:01:38.000000 coop_html_editor-1.4.1/coop_html_editor/static/ckeditor.4.6.2/plugins/a11yhelp/dialogs/lang/mn.js
+-rw-rw-r--   0 lucjean   (1001) lucjean   (1001)     4324 2023-05-22 07:01:38.000000 coop_html_editor-1.4.1/coop_html_editor/static/ckeditor.4.6.2/plugins/a11yhelp/dialogs/lang/nb.js
+-rw-rw-r--   0 lucjean   (1001) lucjean   (1001)     4393 2023-05-22 07:01:38.000000 coop_html_editor-1.4.1/coop_html_editor/static/ckeditor.4.6.2/plugins/a11yhelp/dialogs/lang/nl.js
+-rw-rw-r--   0 lucjean   (1001) lucjean   (1001)     4169 2023-05-22 07:01:38.000000 coop_html_editor-1.4.1/coop_html_editor/static/ckeditor.4.6.2/plugins/a11yhelp/dialogs/lang/no.js
+-rw-rw-r--   0 lucjean   (1001) lucjean   (1001)     4968 2023-05-22 07:01:38.000000 coop_html_editor-1.4.1/coop_html_editor/static/ckeditor.4.6.2/plugins/a11yhelp/dialogs/lang/oc.js
+-rw-rw-r--   0 lucjean   (1001) lucjean   (1001)     4840 2023-05-22 07:01:38.000000 coop_html_editor-1.4.1/coop_html_editor/static/ckeditor.4.6.2/plugins/a11yhelp/dialogs/lang/pl.js
+-rw-rw-r--   0 lucjean   (1001) lucjean   (1001)     4543 2023-05-22 07:01:38.000000 coop_html_editor-1.4.1/coop_html_editor/static/ckeditor.4.6.2/plugins/a11yhelp/dialogs/lang/pt-br.js
+-rw-rw-r--   0 lucjean   (1001) lucjean   (1001)     4409 2023-05-22 07:01:38.000000 coop_html_editor-1.4.1/coop_html_editor/static/ckeditor.4.6.2/plugins/a11yhelp/dialogs/lang/pt.js
+-rw-rw-r--   0 lucjean   (1001) lucjean   (1001)     4139 2023-05-22 07:01:38.000000 coop_html_editor-1.4.1/coop_html_editor/static/ckeditor.4.6.2/plugins/a11yhelp/dialogs/lang/ro.js
+-rw-rw-r--   0 lucjean   (1001) lucjean   (1001)     6477 2023-05-22 07:01:38.000000 coop_html_editor-1.4.1/coop_html_editor/static/ckeditor.4.6.2/plugins/a11yhelp/dialogs/lang/ru.js
+-rw-rw-r--   0 lucjean   (1001) lucjean   (1001)     5890 2023-05-22 07:01:38.000000 coop_html_editor-1.4.1/coop_html_editor/static/ckeditor.4.6.2/plugins/a11yhelp/dialogs/lang/si.js
+-rw-rw-r--   0 lucjean   (1001) lucjean   (1001)     4576 2023-05-22 07:01:38.000000 coop_html_editor-1.4.1/coop_html_editor/static/ckeditor.4.6.2/plugins/a11yhelp/dialogs/lang/sk.js
+-rw-rw-r--   0 lucjean   (1001) lucjean   (1001)     4292 2023-05-22 07:01:38.000000 coop_html_editor-1.4.1/coop_html_editor/static/ckeditor.4.6.2/plugins/a11yhelp/dialogs/lang/sl.js
+-rw-rw-r--   0 lucjean   (1001) lucjean   (1001)     3938 2023-05-22 07:01:38.000000 coop_html_editor-1.4.1/coop_html_editor/static/ckeditor.4.6.2/plugins/a11yhelp/dialogs/lang/sq.js
+-rw-rw-r--   0 lucjean   (1001) lucjean   (1001)     3862 2023-05-22 07:01:38.000000 coop_html_editor-1.4.1/coop_html_editor/static/ckeditor.4.6.2/plugins/a11yhelp/dialogs/lang/sr-latn.js
+-rw-rw-r--   0 lucjean   (1001) lucjean   (1001)     3861 2023-05-22 07:01:38.000000 coop_html_editor-1.4.1/coop_html_editor/static/ckeditor.4.6.2/plugins/a11yhelp/dialogs/lang/sr.js
+-rw-rw-r--   0 lucjean   (1001) lucjean   (1001)     4235 2023-05-22 07:01:38.000000 coop_html_editor-1.4.1/coop_html_editor/static/ckeditor.4.6.2/plugins/a11yhelp/dialogs/lang/sv.js
+-rw-rw-r--   0 lucjean   (1001) lucjean   (1001)     4236 2023-05-22 07:01:38.000000 coop_html_editor-1.4.1/coop_html_editor/static/ckeditor.4.6.2/plugins/a11yhelp/dialogs/lang/th.js
+-rw-rw-r--   0 lucjean   (1001) lucjean   (1001)     4436 2023-05-22 07:01:38.000000 coop_html_editor-1.4.1/coop_html_editor/static/ckeditor.4.6.2/plugins/a11yhelp/dialogs/lang/tr.js
+-rw-rw-r--   0 lucjean   (1001) lucjean   (1001)     4177 2023-05-22 07:01:38.000000 coop_html_editor-1.4.1/coop_html_editor/static/ckeditor.4.6.2/plugins/a11yhelp/dialogs/lang/tt.js
+-rw-rw-r--   0 lucjean   (1001) lucjean   (1001)     6793 2023-05-22 07:01:38.000000 coop_html_editor-1.4.1/coop_html_editor/static/ckeditor.4.6.2/plugins/a11yhelp/dialogs/lang/ug.js
+-rw-rw-r--   0 lucjean   (1001) lucjean   (1001)     6737 2023-05-22 07:01:38.000000 coop_html_editor-1.4.1/coop_html_editor/static/ckeditor.4.6.2/plugins/a11yhelp/dialogs/lang/uk.js
+-rw-rw-r--   0 lucjean   (1001) lucjean   (1001)     5145 2023-05-22 07:01:38.000000 coop_html_editor-1.4.1/coop_html_editor/static/ckeditor.4.6.2/plugins/a11yhelp/dialogs/lang/vi.js
+-rw-rw-r--   0 lucjean   (1001) lucjean   (1001)     4022 2023-05-22 07:01:38.000000 coop_html_editor-1.4.1/coop_html_editor/static/ckeditor.4.6.2/plugins/a11yhelp/dialogs/lang/zh-cn.js
+-rw-rw-r--   0 lucjean   (1001) lucjean   (1001)     4061 2023-05-22 07:01:38.000000 coop_html_editor-1.4.1/coop_html_editor/static/ckeditor.4.6.2/plugins/a11yhelp/dialogs/lang/zh.js
+drwxrwxr-x   0 lucjean   (1001) lucjean   (1001)        0 2023-06-12 12:55:08.703912 coop_html_editor-1.4.1/coop_html_editor/static/ckeditor.4.6.2/plugins/about/
+drwxrwxr-x   0 lucjean   (1001) lucjean   (1001)        0 2023-06-12 12:55:08.723913 coop_html_editor-1.4.1/coop_html_editor/static/ckeditor.4.6.2/plugins/about/dialogs/
+-rw-rw-r--   0 lucjean   (1001) lucjean   (1001)     1886 2023-05-22 07:01:38.000000 coop_html_editor-1.4.1/coop_html_editor/static/ckeditor.4.6.2/plugins/about/dialogs/about.js
+drwxrwxr-x   0 lucjean   (1001) lucjean   (1001)        0 2023-06-12 12:55:08.723913 coop_html_editor-1.4.1/coop_html_editor/static/ckeditor.4.6.2/plugins/about/dialogs/hidpi/
+-rw-rw-r--   0 lucjean   (1001) lucjean   (1001)    13339 2023-05-22 07:01:38.000000 coop_html_editor-1.4.1/coop_html_editor/static/ckeditor.4.6.2/plugins/about/dialogs/hidpi/logo_ckeditor.png
+-rw-rw-r--   0 lucjean   (1001) lucjean   (1001)     6757 2023-05-22 07:01:38.000000 coop_html_editor-1.4.1/coop_html_editor/static/ckeditor.4.6.2/plugins/about/dialogs/logo_ckeditor.png
+drwxrwxr-x   0 lucjean   (1001) lucjean   (1001)        0 2023-06-12 12:55:08.727913 coop_html_editor-1.4.1/coop_html_editor/static/ckeditor.4.6.2/plugins/btgrid/
+-rw-rw-r--   0 lucjean   (1001) lucjean   (1001)     1072 2023-05-22 07:01:38.000000 coop_html_editor-1.4.1/coop_html_editor/static/ckeditor.4.6.2/plugins/btgrid/LICENSE.txt
+-rw-rw-r--   0 lucjean   (1001) lucjean   (1001)      548 2023-05-22 07:01:38.000000 coop_html_editor-1.4.1/coop_html_editor/static/ckeditor.4.6.2/plugins/btgrid/README.md
+-rw-rw-r--   0 lucjean   (1001) lucjean   (1001)      570 2023-05-22 07:01:38.000000 coop_html_editor-1.4.1/coop_html_editor/static/ckeditor.4.6.2/plugins/btgrid/bower.json
+drwxrwxr-x   0 lucjean   (1001) lucjean   (1001)        0 2023-06-12 12:55:08.727913 coop_html_editor-1.4.1/coop_html_editor/static/ckeditor.4.6.2/plugins/btgrid/dialogs/
+-rw-rw-r--   0 lucjean   (1001) lucjean   (1001)     2392 2023-05-22 07:01:38.000000 coop_html_editor-1.4.1/coop_html_editor/static/ckeditor.4.6.2/plugins/btgrid/dialogs/btgrid.js
+drwxrwxr-x   0 lucjean   (1001) lucjean   (1001)        0 2023-06-12 12:55:08.727913 coop_html_editor-1.4.1/coop_html_editor/static/ckeditor.4.6.2/plugins/btgrid/lang/
+-rw-rw-r--   0 lucjean   (1001) lucjean   (1001)      365 2023-05-22 07:01:38.000000 coop_html_editor-1.4.1/coop_html_editor/static/ckeditor.4.6.2/plugins/btgrid/lang/en.js
+-rw-rw-r--   0 lucjean   (1001) lucjean   (1001)      369 2023-05-22 07:01:38.000000 coop_html_editor-1.4.1/coop_html_editor/static/ckeditor.4.6.2/plugins/btgrid/lang/fr.js
+-rw-rw-r--   0 lucjean   (1001) lucjean   (1001)      330 2023-05-22 07:01:38.000000 coop_html_editor-1.4.1/coop_html_editor/static/ckeditor.4.6.2/plugins/btgrid/lang/nl.js
+-rw-rw-r--   0 lucjean   (1001) lucjean   (1001)      556 2023-05-22 07:01:38.000000 coop_html_editor-1.4.1/coop_html_editor/static/ckeditor.4.6.2/plugins/btgrid/lang/ru.js
+-rw-rw-r--   0 lucjean   (1001) lucjean   (1001)     3209 2023-05-22 07:01:38.000000 coop_html_editor-1.4.1/coop_html_editor/static/ckeditor.4.6.2/plugins/btgrid/plugin.js
+drwxrwxr-x   0 lucjean   (1001) lucjean   (1001)        0 2023-06-12 12:55:08.727913 coop_html_editor-1.4.1/coop_html_editor/static/ckeditor.4.6.2/plugins/btgrid/styles/
+-rw-rw-r--   0 lucjean   (1001) lucjean   (1001)     1432 2023-05-22 07:01:38.000000 coop_html_editor-1.4.1/coop_html_editor/static/ckeditor.4.6.2/plugins/btgrid/styles/editor.css
+drwxrwxr-x   0 lucjean   (1001) lucjean   (1001)        0 2023-06-12 12:55:08.727913 coop_html_editor-1.4.1/coop_html_editor/static/ckeditor.4.6.2/plugins/button/
+drwxrwxr-x   0 lucjean   (1001) lucjean   (1001)        0 2023-06-12 12:55:08.735913 coop_html_editor-1.4.1/coop_html_editor/static/ckeditor.4.6.2/plugins/button/lang/
+-rw-rw-r--   0 lucjean   (1001) lucjean   (1001)      241 2023-05-22 07:01:38.000000 coop_html_editor-1.4.1/coop_html_editor/static/ckeditor.4.6.2/plugins/button/lang/af.js
+-rw-rw-r--   0 lucjean   (1001) lucjean   (1001)      242 2023-05-22 07:01:38.000000 coop_html_editor-1.4.1/coop_html_editor/static/ckeditor.4.6.2/plugins/button/lang/ar.js
+-rw-rw-r--   0 lucjean   (1001) lucjean   (1001)      242 2023-05-22 07:01:38.000000 coop_html_editor-1.4.1/coop_html_editor/static/ckeditor.4.6.2/plugins/button/lang/az.js
+-rw-rw-r--   0 lucjean   (1001) lucjean   (1001)      248 2023-05-22 07:01:38.000000 coop_html_editor-1.4.1/coop_html_editor/static/ckeditor.4.6.2/plugins/button/lang/bg.js
+-rw-rw-r--   0 lucjean   (1001) lucjean   (1001)      245 2023-05-22 07:01:38.000000 coop_html_editor-1.4.1/coop_html_editor/static/ckeditor.4.6.2/plugins/button/lang/ca.js
+-rw-rw-r--   0 lucjean   (1001) lucjean   (1001)      242 2023-05-22 07:01:38.000000 coop_html_editor-1.4.1/coop_html_editor/static/ckeditor.4.6.2/plugins/button/lang/cs.js
+-rw-rw-r--   0 lucjean   (1001) lucjean   (1001)      239 2023-05-22 07:01:38.000000 coop_html_editor-1.4.1/coop_html_editor/static/ckeditor.4.6.2/plugins/button/lang/da.js
+-rw-rw-r--   0 lucjean   (1001) lucjean   (1001)      248 2023-05-22 07:01:38.000000 coop_html_editor-1.4.1/coop_html_editor/static/ckeditor.4.6.2/plugins/button/lang/de-ch.js
+-rw-rw-r--   0 lucjean   (1001) lucjean   (1001)      245 2023-05-22 07:01:38.000000 coop_html_editor-1.4.1/coop_html_editor/static/ckeditor.4.6.2/plugins/button/lang/de.js
+-rw-rw-r--   0 lucjean   (1001) lucjean   (1001)      254 2023-05-22 07:01:38.000000 coop_html_editor-1.4.1/coop_html_editor/static/ckeditor.4.6.2/plugins/button/lang/el.js
+-rw-rw-r--   0 lucjean   (1001) lucjean   (1001)      245 2023-05-22 07:01:38.000000 coop_html_editor-1.4.1/coop_html_editor/static/ckeditor.4.6.2/plugins/button/lang/en-gb.js
+-rw-rw-r--   0 lucjean   (1001) lucjean   (1001)      242 2023-05-22 07:01:38.000000 coop_html_editor-1.4.1/coop_html_editor/static/ckeditor.4.6.2/plugins/button/lang/en.js
+-rw-rw-r--   0 lucjean   (1001) lucjean   (1001)      243 2023-05-22 07:01:38.000000 coop_html_editor-1.4.1/coop_html_editor/static/ckeditor.4.6.2/plugins/button/lang/eo.js
+-rw-rw-r--   0 lucjean   (1001) lucjean   (1001)      246 2023-05-22 07:01:38.000000 coop_html_editor-1.4.1/coop_html_editor/static/ckeditor.4.6.2/plugins/button/lang/es.js
+-rw-rw-r--   0 lucjean   (1001) lucjean   (1001)      243 2023-05-22 07:01:38.000000 coop_html_editor-1.4.1/coop_html_editor/static/ckeditor.4.6.2/plugins/button/lang/eu.js
+-rw-rw-r--   0 lucjean   (1001) lucjean   (1001)      253 2023-05-22 07:01:38.000000 coop_html_editor-1.4.1/coop_html_editor/static/ckeditor.4.6.2/plugins/button/lang/fa.js
+-rw-rw-r--   0 lucjean   (1001) lucjean   (1001)      241 2023-05-22 07:01:38.000000 coop_html_editor-1.4.1/coop_html_editor/static/ckeditor.4.6.2/plugins/button/lang/fi.js
+-rw-rw-r--   0 lucjean   (1001) lucjean   (1001)      247 2023-05-22 07:01:38.000000 coop_html_editor-1.4.1/coop_html_editor/static/ckeditor.4.6.2/plugins/button/lang/fr.js
+-rw-rw-r--   0 lucjean   (1001) lucjean   (1001)      246 2023-05-22 07:01:38.000000 coop_html_editor-1.4.1/coop_html_editor/static/ckeditor.4.6.2/plugins/button/lang/gl.js
+-rw-rw-r--   0 lucjean   (1001) lucjean   (1001)      242 2023-05-22 07:01:38.000000 coop_html_editor-1.4.1/coop_html_editor/static/ckeditor.4.6.2/plugins/button/lang/he.js
+-rw-rw-r--   0 lucjean   (1001) lucjean   (1001)      246 2023-05-22 07:01:38.000000 coop_html_editor-1.4.1/coop_html_editor/static/ckeditor.4.6.2/plugins/button/lang/hu.js
+-rw-rw-r--   0 lucjean   (1001) lucjean   (1001)      240 2023-05-22 07:01:38.000000 coop_html_editor-1.4.1/coop_html_editor/static/ckeditor.4.6.2/plugins/button/lang/id.js
+-rw-rw-r--   0 lucjean   (1001) lucjean   (1001)      245 2023-05-22 07:01:38.000000 coop_html_editor-1.4.1/coop_html_editor/static/ckeditor.4.6.2/plugins/button/lang/it.js
+-rw-rw-r--   0 lucjean   (1001) lucjean   (1001)      243 2023-05-22 07:01:38.000000 coop_html_editor-1.4.1/coop_html_editor/static/ckeditor.4.6.2/plugins/button/lang/ja.js
+-rw-rw-r--   0 lucjean   (1001) lucjean   (1001)      273 2023-05-22 07:01:38.000000 coop_html_editor-1.4.1/coop_html_editor/static/ckeditor.4.6.2/plugins/button/lang/km.js
+-rw-rw-r--   0 lucjean   (1001) lucjean   (1001)      243 2023-05-22 07:01:38.000000 coop_html_editor-1.4.1/coop_html_editor/static/ckeditor.4.6.2/plugins/button/lang/ko.js
+-rw-rw-r--   0 lucjean   (1001) lucjean   (1001)      256 2023-05-22 07:01:38.000000 coop_html_editor-1.4.1/coop_html_editor/static/ckeditor.4.6.2/plugins/button/lang/ku.js
+-rw-rw-r--   0 lucjean   (1001) lucjean   (1001)      244 2023-05-22 07:01:38.000000 coop_html_editor-1.4.1/coop_html_editor/static/ckeditor.4.6.2/plugins/button/lang/lt.js
+-rw-rw-r--   0 lucjean   (1001) lucjean   (1001)      239 2023-05-22 07:01:38.000000 coop_html_editor-1.4.1/coop_html_editor/static/ckeditor.4.6.2/plugins/button/lang/nb.js
+-rw-rw-r--   0 lucjean   (1001) lucjean   (1001)      246 2023-05-22 07:01:38.000000 coop_html_editor-1.4.1/coop_html_editor/static/ckeditor.4.6.2/plugins/button/lang/nl.js
+-rw-rw-r--   0 lucjean   (1001) lucjean   (1001)      239 2023-05-22 07:01:38.000000 coop_html_editor-1.4.1/coop_html_editor/static/ckeditor.4.6.2/plugins/button/lang/no.js
+-rw-rw-r--   0 lucjean   (1001) lucjean   (1001)      245 2023-05-22 07:01:38.000000 coop_html_editor-1.4.1/coop_html_editor/static/ckeditor.4.6.2/plugins/button/lang/oc.js
+-rw-rw-r--   0 lucjean   (1001) lucjean   (1001)      241 2023-05-22 07:01:38.000000 coop_html_editor-1.4.1/coop_html_editor/static/ckeditor.4.6.2/plugins/button/lang/pl.js
+-rw-rw-r--   0 lucjean   (1001) lucjean   (1001)      248 2023-05-22 07:01:38.000000 coop_html_editor-1.4.1/coop_html_editor/static/ckeditor.4.6.2/plugins/button/lang/pt-br.js
+-rw-rw-r--   0 lucjean   (1001) lucjean   (1001)      245 2023-05-22 07:01:38.000000 coop_html_editor-1.4.1/coop_html_editor/static/ckeditor.4.6.2/plugins/button/lang/pt.js
+-rw-rw-r--   0 lucjean   (1001) lucjean   (1001)      242 2023-05-22 07:01:38.000000 coop_html_editor-1.4.1/coop_html_editor/static/ckeditor.4.6.2/plugins/button/lang/ro.js
+-rw-rw-r--   0 lucjean   (1001) lucjean   (1001)      248 2023-05-22 07:01:38.000000 coop_html_editor-1.4.1/coop_html_editor/static/ckeditor.4.6.2/plugins/button/lang/ru.js
+-rw-rw-r--   0 lucjean   (1001) lucjean   (1001)      242 2023-05-22 07:01:38.000000 coop_html_editor-1.4.1/coop_html_editor/static/ckeditor.4.6.2/plugins/button/lang/sk.js
+-rw-rw-r--   0 lucjean   (1001) lucjean   (1001)      241 2023-05-22 07:01:38.000000 coop_html_editor-1.4.1/coop_html_editor/static/ckeditor.4.6.2/plugins/button/lang/sl.js
+-rw-rw-r--   0 lucjean   (1001) lucjean   (1001)      246 2023-05-22 07:01:38.000000 coop_html_editor-1.4.1/coop_html_editor/static/ckeditor.4.6.2/plugins/button/lang/sq.js
+-rw-rw-r--   0 lucjean   (1001) lucjean   (1001)      238 2023-05-22 07:01:38.000000 coop_html_editor-1.4.1/coop_html_editor/static/ckeditor.4.6.2/plugins/button/lang/sv.js
+-rw-rw-r--   0 lucjean   (1001) lucjean   (1001)      244 2023-05-22 07:01:38.000000 coop_html_editor-1.4.1/coop_html_editor/static/ckeditor.4.6.2/plugins/button/lang/tr.js
+-rw-rw-r--   0 lucjean   (1001) lucjean   (1001)      252 2023-05-22 07:01:38.000000 coop_html_editor-1.4.1/coop_html_editor/static/ckeditor.4.6.2/plugins/button/lang/tt.js
+-rw-rw-r--   0 lucjean   (1001) lucjean   (1001)      250 2023-05-22 07:01:38.000000 coop_html_editor-1.4.1/coop_html_editor/static/ckeditor.4.6.2/plugins/button/lang/ug.js
+-rw-rw-r--   0 lucjean   (1001) lucjean   (1001)      248 2023-05-22 07:01:38.000000 coop_html_editor-1.4.1/coop_html_editor/static/ckeditor.4.6.2/plugins/button/lang/uk.js
+-rw-rw-r--   0 lucjean   (1001) lucjean   (1001)      245 2023-05-22 07:01:38.000000 coop_html_editor-1.4.1/coop_html_editor/static/ckeditor.4.6.2/plugins/button/lang/vi.js
+-rw-rw-r--   0 lucjean   (1001) lucjean   (1001)      248 2023-05-22 07:01:38.000000 coop_html_editor-1.4.1/coop_html_editor/static/ckeditor.4.6.2/plugins/button/lang/zh-cn.js
+-rw-rw-r--   0 lucjean   (1001) lucjean   (1001)      243 2023-05-22 07:01:38.000000 coop_html_editor-1.4.1/coop_html_editor/static/ckeditor.4.6.2/plugins/button/lang/zh.js
+-rw-rw-r--   0 lucjean   (1001) lucjean   (1001)    11829 2023-05-22 07:01:38.000000 coop_html_editor-1.4.1/coop_html_editor/static/ckeditor.4.6.2/plugins/button/plugin.js
+drwxrwxr-x   0 lucjean   (1001) lucjean   (1001)        0 2023-06-12 12:55:08.735913 coop_html_editor-1.4.1/coop_html_editor/static/ckeditor.4.6.2/plugins/clipboard/
+drwxrwxr-x   0 lucjean   (1001) lucjean   (1001)        0 2023-06-12 12:55:08.735913 coop_html_editor-1.4.1/coop_html_editor/static/ckeditor.4.6.2/plugins/clipboard/dev/
+-rw-rw-r--   0 lucjean   (1001) lucjean   (1001)     5581 2023-05-22 07:01:38.000000 coop_html_editor-1.4.1/coop_html_editor/static/ckeditor.4.6.2/plugins/clipboard/dev/clipboard.html
+-rw-rw-r--   0 lucjean   (1001) lucjean   (1001)     1077 2023-05-22 07:01:38.000000 coop_html_editor-1.4.1/coop_html_editor/static/ckeditor.4.6.2/plugins/clipboard/dev/console.js
+-rw-rw-r--   0 lucjean   (1001) lucjean   (1001)    14102 2023-05-22 07:01:38.000000 coop_html_editor-1.4.1/coop_html_editor/static/ckeditor.4.6.2/plugins/clipboard/dev/dnd.html
+drwxrwxr-x   0 lucjean   (1001) lucjean   (1001)        0 2023-06-12 12:55:08.735913 coop_html_editor-1.4.1/coop_html_editor/static/ckeditor.4.6.2/plugins/clipboard/dialogs/
+-rw-rw-r--   0 lucjean   (1001) lucjean   (1001)     3963 2023-05-22 07:01:38.000000 coop_html_editor-1.4.1/coop_html_editor/static/ckeditor.4.6.2/plugins/clipboard/dialogs/paste.js
+drwxrwxr-x   0 lucjean   (1001) lucjean   (1001)        0 2023-06-12 12:55:08.747913 coop_html_editor-1.4.1/coop_html_editor/static/ckeditor.4.6.2/plugins/clipboard/lang/
+-rw-rw-r--   0 lucjean   (1001) lucjean   (1001)      833 2023-05-22 07:01:38.000000 coop_html_editor-1.4.1/coop_html_editor/static/ckeditor.4.6.2/plugins/clipboard/lang/af.js
+-rw-rw-r--   0 lucjean   (1001) lucjean   (1001)     1168 2023-05-22 07:01:38.000000 coop_html_editor-1.4.1/coop_html_editor/static/ckeditor.4.6.2/plugins/clipboard/lang/ar.js
+-rw-rw-r--   0 lucjean   (1001) lucjean   (1001)      606 2023-05-22 07:01:38.000000 coop_html_editor-1.4.1/coop_html_editor/static/ckeditor.4.6.2/plugins/clipboard/lang/az.js
+-rw-rw-r--   0 lucjean   (1001) lucjean   (1001)     1318 2023-05-22 07:01:38.000000 coop_html_editor-1.4.1/coop_html_editor/static/ckeditor.4.6.2/plugins/clipboard/lang/bg.js
+-rw-rw-r--   0 lucjean   (1001) lucjean   (1001)     1543 2023-05-22 07:01:38.000000 coop_html_editor-1.4.1/coop_html_editor/static/ckeditor.4.6.2/plugins/clipboard/lang/bn.js
+-rw-rw-r--   0 lucjean   (1001) lucjean   (1001)      927 2023-05-22 07:01:38.000000 coop_html_editor-1.4.1/coop_html_editor/static/ckeditor.4.6.2/plugins/clipboard/lang/bs.js
+-rw-rw-r--   0 lucjean   (1001) lucjean   (1001)      963 2023-05-22 07:01:38.000000 coop_html_editor-1.4.1/coop_html_editor/static/ckeditor.4.6.2/plugins/clipboard/lang/ca.js
+-rw-rw-r--   0 lucjean   (1001) lucjean   (1001)     1080 2023-05-22 07:01:38.000000 coop_html_editor-1.4.1/coop_html_editor/static/ckeditor.4.6.2/plugins/clipboard/lang/cs.js
+-rw-rw-r--   0 lucjean   (1001) lucjean   (1001)      957 2023-05-22 07:01:38.000000 coop_html_editor-1.4.1/coop_html_editor/static/ckeditor.4.6.2/plugins/clipboard/lang/cy.js
+-rw-rw-r--   0 lucjean   (1001) lucjean   (1001)      970 2023-05-22 07:01:38.000000 coop_html_editor-1.4.1/coop_html_editor/static/ckeditor.4.6.2/plugins/clipboard/lang/da.js
+-rw-rw-r--   0 lucjean   (1001) lucjean   (1001)     1055 2023-05-22 07:01:38.000000 coop_html_editor-1.4.1/coop_html_editor/static/ckeditor.4.6.2/plugins/clipboard/lang/de-ch.js
+-rw-rw-r--   0 lucjean   (1001) lucjean   (1001)     1052 2023-05-22 07:01:38.000000 coop_html_editor-1.4.1/coop_html_editor/static/ckeditor.4.6.2/plugins/clipboard/lang/de.js
+-rw-rw-r--   0 lucjean   (1001) lucjean   (1001)     1444 2023-05-22 07:01:38.000000 coop_html_editor-1.4.1/coop_html_editor/static/ckeditor.4.6.2/plugins/clipboard/lang/el.js
+-rw-rw-r--   0 lucjean   (1001) lucjean   (1001)      907 2023-05-22 07:01:38.000000 coop_html_editor-1.4.1/coop_html_editor/static/ckeditor.4.6.2/plugins/clipboard/lang/en-au.js
+-rw-rw-r--   0 lucjean   (1001) lucjean   (1001)      907 2023-05-22 07:01:38.000000 coop_html_editor-1.4.1/coop_html_editor/static/ckeditor.4.6.2/plugins/clipboard/lang/en-ca.js
+-rw-rw-r--   0 lucjean   (1001) lucjean   (1001)      896 2023-05-22 07:01:38.000000 coop_html_editor-1.4.1/coop_html_editor/static/ckeditor.4.6.2/plugins/clipboard/lang/en-gb.js
+-rw-rw-r--   0 lucjean   (1001) lucjean   (1001)      893 2023-05-22 07:01:38.000000 coop_html_editor-1.4.1/coop_html_editor/static/ckeditor.4.6.2/plugins/clipboard/lang/en.js
+-rw-rw-r--   0 lucjean   (1001) lucjean   (1001)      900 2023-05-22 07:01:38.000000 coop_html_editor-1.4.1/coop_html_editor/static/ckeditor.4.6.2/plugins/clipboard/lang/eo.js
+-rw-rw-r--   0 lucjean   (1001) lucjean   (1001)      947 2023-05-22 07:01:38.000000 coop_html_editor-1.4.1/coop_html_editor/static/ckeditor.4.6.2/plugins/clipboard/lang/es.js
+-rw-rw-r--   0 lucjean   (1001) lucjean   (1001)      928 2023-05-22 07:01:38.000000 coop_html_editor-1.4.1/coop_html_editor/static/ckeditor.4.6.2/plugins/clipboard/lang/et.js
+-rw-rw-r--   0 lucjean   (1001) lucjean   (1001)      894 2023-05-22 07:01:38.000000 coop_html_editor-1.4.1/coop_html_editor/static/ckeditor.4.6.2/plugins/clipboard/lang/eu.js
+-rw-rw-r--   0 lucjean   (1001) lucjean   (1001)     1351 2023-05-22 07:01:38.000000 coop_html_editor-1.4.1/coop_html_editor/static/ckeditor.4.6.2/plugins/clipboard/lang/fa.js
+-rw-rw-r--   0 lucjean   (1001) lucjean   (1001)      807 2023-05-22 07:01:38.000000 coop_html_editor-1.4.1/coop_html_editor/static/ckeditor.4.6.2/plugins/clipboard/lang/fi.js
+-rw-rw-r--   0 lucjean   (1001) lucjean   (1001)      920 2023-05-22 07:01:38.000000 coop_html_editor-1.4.1/coop_html_editor/static/ckeditor.4.6.2/plugins/clipboard/lang/fo.js
+-rw-rw-r--   0 lucjean   (1001) lucjean   (1001)     1007 2023-05-22 07:01:38.000000 coop_html_editor-1.4.1/coop_html_editor/static/ckeditor.4.6.2/plugins/clipboard/lang/fr-ca.js
+-rw-rw-r--   0 lucjean   (1001) lucjean   (1001)     1075 2023-05-22 07:01:38.000000 coop_html_editor-1.4.1/coop_html_editor/static/ckeditor.4.6.2/plugins/clipboard/lang/fr.js
+-rw-rw-r--   0 lucjean   (1001) lucjean   (1001)      887 2023-05-22 07:01:38.000000 coop_html_editor-1.4.1/coop_html_editor/static/ckeditor.4.6.2/plugins/clipboard/lang/gl.js
+-rw-rw-r--   0 lucjean   (1001) lucjean   (1001)     1286 2023-05-22 07:01:38.000000 coop_html_editor-1.4.1/coop_html_editor/static/ckeditor.4.6.2/plugins/clipboard/lang/gu.js
+-rw-rw-r--   0 lucjean   (1001) lucjean   (1001)     1034 2023-05-22 07:01:38.000000 coop_html_editor-1.4.1/coop_html_editor/static/ckeditor.4.6.2/plugins/clipboard/lang/he.js
+-rw-rw-r--   0 lucjean   (1001) lucjean   (1001)     1410 2023-05-22 07:01:38.000000 coop_html_editor-1.4.1/coop_html_editor/static/ckeditor.4.6.2/plugins/clipboard/lang/hi.js
+-rw-rw-r--   0 lucjean   (1001) lucjean   (1001)      933 2023-05-22 07:01:38.000000 coop_html_editor-1.4.1/coop_html_editor/static/ckeditor.4.6.2/plugins/clipboard/lang/hr.js
+-rw-rw-r--   0 lucjean   (1001) lucjean   (1001)     1005 2023-05-22 07:01:38.000000 coop_html_editor-1.4.1/coop_html_editor/static/ckeditor.4.6.2/plugins/clipboard/lang/hu.js
+-rw-rw-r--   0 lucjean   (1001) lucjean   (1001)      920 2023-05-22 07:01:38.000000 coop_html_editor-1.4.1/coop_html_editor/static/ckeditor.4.6.2/plugins/clipboard/lang/id.js
+-rw-rw-r--   0 lucjean   (1001) lucjean   (1001)      879 2023-05-22 07:01:38.000000 coop_html_editor-1.4.1/coop_html_editor/static/ckeditor.4.6.2/plugins/clipboard/lang/is.js
+-rw-rw-r--   0 lucjean   (1001) lucjean   (1001)      921 2023-05-22 07:01:38.000000 coop_html_editor-1.4.1/coop_html_editor/static/ckeditor.4.6.2/plugins/clipboard/lang/it.js
+-rw-rw-r--   0 lucjean   (1001) lucjean   (1001)     1204 2023-05-22 07:01:38.000000 coop_html_editor-1.4.1/coop_html_editor/static/ckeditor.4.6.2/plugins/clipboard/lang/ja.js
+-rw-rw-r--   0 lucjean   (1001) lucjean   (1001)     1743 2023-05-22 07:01:38.000000 coop_html_editor-1.4.1/coop_html_editor/static/ckeditor.4.6.2/plugins/clipboard/lang/ka.js
+-rw-rw-r--   0 lucjean   (1001) lucjean   (1001)     2033 2023-05-22 07:01:38.000000 coop_html_editor-1.4.1/coop_html_editor/static/ckeditor.4.6.2/plugins/clipboard/lang/km.js
+-rw-rw-r--   0 lucjean   (1001) lucjean   (1001)      915 2023-05-22 07:01:38.000000 coop_html_editor-1.4.1/coop_html_editor/static/ckeditor.4.6.2/plugins/clipboard/lang/ko.js
+-rw-rw-r--   0 lucjean   (1001) lucjean   (1001)     1339 2023-05-22 07:01:38.000000 coop_html_editor-1.4.1/coop_html_editor/static/ckeditor.4.6.2/plugins/clipboard/lang/ku.js
+-rw-rw-r--   0 lucjean   (1001) lucjean   (1001)      980 2023-05-22 07:01:38.000000 coop_html_editor-1.4.1/coop_html_editor/static/ckeditor.4.6.2/plugins/clipboard/lang/lt.js
+-rw-rw-r--   0 lucjean   (1001) lucjean   (1001)      997 2023-05-22 07:01:38.000000 coop_html_editor-1.4.1/coop_html_editor/static/ckeditor.4.6.2/plugins/clipboard/lang/lv.js
+-rw-rw-r--   0 lucjean   (1001) lucjean   (1001)     1462 2023-05-22 07:01:38.000000 coop_html_editor-1.4.1/coop_html_editor/static/ckeditor.4.6.2/plugins/clipboard/lang/mk.js
+-rw-rw-r--   0 lucjean   (1001) lucjean   (1001)     1215 2023-05-22 07:01:38.000000 coop_html_editor-1.4.1/coop_html_editor/static/ckeditor.4.6.2/plugins/clipboard/lang/mn.js
+-rw-rw-r--   0 lucjean   (1001) lucjean   (1001)      878 2023-05-22 07:01:38.000000 coop_html_editor-1.4.1/coop_html_editor/static/ckeditor.4.6.2/plugins/clipboard/lang/ms.js
+-rw-rw-r--   0 lucjean   (1001) lucjean   (1001)      889 2023-05-22 07:01:38.000000 coop_html_editor-1.4.1/coop_html_editor/static/ckeditor.4.6.2/plugins/clipboard/lang/nb.js
+-rw-rw-r--   0 lucjean   (1001) lucjean   (1001)      939 2023-05-22 07:01:38.000000 coop_html_editor-1.4.1/coop_html_editor/static/ckeditor.4.6.2/plugins/clipboard/lang/nl.js
+-rw-rw-r--   0 lucjean   (1001) lucjean   (1001)      873 2023-05-22 07:01:38.000000 coop_html_editor-1.4.1/coop_html_editor/static/ckeditor.4.6.2/plugins/clipboard/lang/no.js
+-rw-rw-r--   0 lucjean   (1001) lucjean   (1001)     1042 2023-05-22 07:01:38.000000 coop_html_editor-1.4.1/coop_html_editor/static/ckeditor.4.6.2/plugins/clipboard/lang/oc.js
+-rw-rw-r--   0 lucjean   (1001) lucjean   (1001)      885 2023-05-22 07:01:38.000000 coop_html_editor-1.4.1/coop_html_editor/static/ckeditor.4.6.2/plugins/clipboard/lang/pl.js
+-rw-rw-r--   0 lucjean   (1001) lucjean   (1001)     1012 2023-05-22 07:01:38.000000 coop_html_editor-1.4.1/coop_html_editor/static/ckeditor.4.6.2/plugins/clipboard/lang/pt-br.js
+-rw-rw-r--   0 lucjean   (1001) lucjean   (1001)      934 2023-05-22 07:01:38.000000 coop_html_editor-1.4.1/coop_html_editor/static/ckeditor.4.6.2/plugins/clipboard/lang/pt.js
+-rw-rw-r--   0 lucjean   (1001) lucjean   (1001)     1062 2023-05-22 07:01:38.000000 coop_html_editor-1.4.1/coop_html_editor/static/ckeditor.4.6.2/plugins/clipboard/lang/ro.js
+-rw-rw-r--   0 lucjean   (1001) lucjean   (1001)     1432 2023-05-22 07:01:38.000000 coop_html_editor-1.4.1/coop_html_editor/static/ckeditor.4.6.2/plugins/clipboard/lang/ru.js
+-rw-rw-r--   0 lucjean   (1001) lucjean   (1001)     1035 2023-05-22 07:01:38.000000 coop_html_editor-1.4.1/coop_html_editor/static/ckeditor.4.6.2/plugins/clipboard/lang/si.js
+-rw-rw-r--   0 lucjean   (1001) lucjean   (1001)      928 2023-05-22 07:01:38.000000 coop_html_editor-1.4.1/coop_html_editor/static/ckeditor.4.6.2/plugins/clipboard/lang/sk.js
+-rw-rw-r--   0 lucjean   (1001) lucjean   (1001)      875 2023-05-22 07:01:38.000000 coop_html_editor-1.4.1/coop_html_editor/static/ckeditor.4.6.2/plugins/clipboard/lang/sl.js
+-rw-rw-r--   0 lucjean   (1001) lucjean   (1001)     1063 2023-05-22 07:01:38.000000 coop_html_editor-1.4.1/coop_html_editor/static/ckeditor.4.6.2/plugins/clipboard/lang/sq.js
+-rw-rw-r--   0 lucjean   (1001) lucjean   (1001)      996 2023-05-22 07:01:38.000000 coop_html_editor-1.4.1/coop_html_editor/static/ckeditor.4.6.2/plugins/clipboard/lang/sr-latn.js
+-rw-rw-r--   0 lucjean   (1001) lucjean   (1001)     1375 2023-05-22 07:01:38.000000 coop_html_editor-1.4.1/coop_html_editor/static/ckeditor.4.6.2/plugins/clipboard/lang/sr.js
+-rw-rw-r--   0 lucjean   (1001) lucjean   (1001)      845 2023-05-22 07:01:38.000000 coop_html_editor-1.4.1/coop_html_editor/static/ckeditor.4.6.2/plugins/clipboard/lang/sv.js
+-rw-rw-r--   0 lucjean   (1001) lucjean   (1001)     1532 2023-05-22 07:01:38.000000 coop_html_editor-1.4.1/coop_html_editor/static/ckeditor.4.6.2/plugins/clipboard/lang/th.js
+-rw-rw-r--   0 lucjean   (1001) lucjean   (1001)      966 2023-05-22 07:01:38.000000 coop_html_editor-1.4.1/coop_html_editor/static/ckeditor.4.6.2/plugins/clipboard/lang/tr.js
+-rw-rw-r--   0 lucjean   (1001) lucjean   (1001)     1078 2023-05-22 07:01:38.000000 coop_html_editor-1.4.1/coop_html_editor/static/ckeditor.4.6.2/plugins/clipboard/lang/tt.js
+-rw-rw-r--   0 lucjean   (1001) lucjean   (1001)     1481 2023-05-22 07:01:38.000000 coop_html_editor-1.4.1/coop_html_editor/static/ckeditor.4.6.2/plugins/clipboard/lang/ug.js
+-rw-rw-r--   0 lucjean   (1001) lucjean   (1001)     1528 2023-05-22 07:01:38.000000 coop_html_editor-1.4.1/coop_html_editor/static/ckeditor.4.6.2/plugins/clipboard/lang/uk.js
+-rw-rw-r--   0 lucjean   (1001) lucjean   (1001)     1091 2023-05-22 07:01:38.000000 coop_html_editor-1.4.1/coop_html_editor/static/ckeditor.4.6.2/plugins/clipboard/lang/vi.js
+-rw-rw-r--   0 lucjean   (1001) lucjean   (1001)      861 2023-05-22 07:01:38.000000 coop_html_editor-1.4.1/coop_html_editor/static/ckeditor.4.6.2/plugins/clipboard/lang/zh-cn.js
+-rw-rw-r--   0 lucjean   (1001) lucjean   (1001)      825 2023-05-22 07:01:38.000000 coop_html_editor-1.4.1/coop_html_editor/static/ckeditor.4.6.2/plugins/clipboard/lang/zh.js
+-rw-rw-r--   0 lucjean   (1001) lucjean   (1001)   100076 2023-05-22 07:01:38.000000 coop_html_editor-1.4.1/coop_html_editor/static/ckeditor.4.6.2/plugins/clipboard/plugin.js
+drwxrwxr-x   0 lucjean   (1001) lucjean   (1001)        0 2023-06-12 12:55:08.747913 coop_html_editor-1.4.1/coop_html_editor/static/ckeditor.4.6.2/plugins/dialog/
+-rw-rw-r--   0 lucjean   (1001) lucjean   (1001)      148 2023-05-22 07:01:38.000000 coop_html_editor-1.4.1/coop_html_editor/static/ckeditor.4.6.2/plugins/dialog/dialogDefinition.js
+drwxrwxr-x   0 lucjean   (1001) lucjean   (1001)        0 2023-06-12 12:55:08.747913 coop_html_editor-1.4.1/coop_html_editor/static/ckeditor.4.6.2/plugins/embed/
+-rw-rw-r--   0 lucjean   (1001) lucjean   (1001)     3135 2023-05-22 07:01:38.000000 coop_html_editor-1.4.1/coop_html_editor/static/ckeditor.4.6.2/plugins/embed/plugin.js
+drwxrwxr-x   0 lucjean   (1001) lucjean   (1001)        0 2023-06-12 12:55:08.747913 coop_html_editor-1.4.1/coop_html_editor/static/ckeditor.4.6.2/plugins/embedbase/
+drwxrwxr-x   0 lucjean   (1001) lucjean   (1001)        0 2023-06-12 12:55:08.747913 coop_html_editor-1.4.1/coop_html_editor/static/ckeditor.4.6.2/plugins/embedbase/dialogs/
+-rw-rw-r--   0 lucjean   (1001) lucjean   (1001)     2203 2023-05-22 07:01:38.000000 coop_html_editor-1.4.1/coop_html_editor/static/ckeditor.4.6.2/plugins/embedbase/dialogs/embedbase.js
+drwxrwxr-x   0 lucjean   (1001) lucjean   (1001)        0 2023-06-12 12:55:08.751913 coop_html_editor-1.4.1/coop_html_editor/static/ckeditor.4.6.2/plugins/embedbase/lang/
+-rw-rw-r--   0 lucjean   (1001) lucjean   (1001)      757 2023-05-22 07:01:38.000000 coop_html_editor-1.4.1/coop_html_editor/static/ckeditor.4.6.2/plugins/embedbase/lang/az.js
+-rw-rw-r--   0 lucjean   (1001) lucjean   (1001)      759 2023-05-22 07:01:38.000000 coop_html_editor-1.4.1/coop_html_editor/static/ckeditor.4.6.2/plugins/embedbase/lang/ca.js
+-rw-rw-r--   0 lucjean   (1001) lucjean   (1001)      636 2023-05-22 07:01:38.000000 coop_html_editor-1.4.1/coop_html_editor/static/ckeditor.4.6.2/plugins/embedbase/lang/cs.js
+-rw-rw-r--   0 lucjean   (1001) lucjean   (1001)      648 2023-05-22 07:01:38.000000 coop_html_editor-1.4.1/coop_html_editor/static/ckeditor.4.6.2/plugins/embedbase/lang/da.js
+-rw-rw-r--   0 lucjean   (1001) lucjean   (1001)      734 2023-05-22 07:01:38.000000 coop_html_editor-1.4.1/coop_html_editor/static/ckeditor.4.6.2/plugins/embedbase/lang/de-ch.js
+-rw-rw-r--   0 lucjean   (1001) lucjean   (1001)      731 2023-05-22 07:01:38.000000 coop_html_editor-1.4.1/coop_html_editor/static/ckeditor.4.6.2/plugins/embedbase/lang/de.js
+-rw-rw-r--   0 lucjean   (1001) lucjean   (1001)      643 2023-05-22 07:01:38.000000 coop_html_editor-1.4.1/coop_html_editor/static/ckeditor.4.6.2/plugins/embedbase/lang/en.js
+-rw-rw-r--   0 lucjean   (1001) lucjean   (1001)      771 2023-05-22 07:01:38.000000 coop_html_editor-1.4.1/coop_html_editor/static/ckeditor.4.6.2/plugins/embedbase/lang/eo.js
+-rw-rw-r--   0 lucjean   (1001) lucjean   (1001)      685 2023-05-22 07:01:38.000000 coop_html_editor-1.4.1/coop_html_editor/static/ckeditor.4.6.2/plugins/embedbase/lang/es.js
+-rw-rw-r--   0 lucjean   (1001) lucjean   (1001)      679 2023-05-22 07:01:38.000000 coop_html_editor-1.4.1/coop_html_editor/static/ckeditor.4.6.2/plugins/embedbase/lang/eu.js
+-rw-rw-r--   0 lucjean   (1001) lucjean   (1001)      742 2023-05-22 07:01:38.000000 coop_html_editor-1.4.1/coop_html_editor/static/ckeditor.4.6.2/plugins/embedbase/lang/fr.js
+-rw-rw-r--   0 lucjean   (1001) lucjean   (1001)      706 2023-05-22 07:01:38.000000 coop_html_editor-1.4.1/coop_html_editor/static/ckeditor.4.6.2/plugins/embedbase/lang/gl.js
+-rw-rw-r--   0 lucjean   (1001) lucjean   (1001)      723 2023-05-22 07:01:38.000000 coop_html_editor-1.4.1/coop_html_editor/static/ckeditor.4.6.2/plugins/embedbase/lang/id.js
+-rw-rw-r--   0 lucjean   (1001) lucjean   (1001)      741 2023-05-22 07:01:38.000000 coop_html_editor-1.4.1/coop_html_editor/static/ckeditor.4.6.2/plugins/embedbase/lang/it.js
+-rw-rw-r--   0 lucjean   (1001) lucjean   (1001)      753 2023-05-22 07:01:38.000000 coop_html_editor-1.4.1/coop_html_editor/static/ckeditor.4.6.2/plugins/embedbase/lang/ja.js
+-rw-rw-r--   0 lucjean   (1001) lucjean   (1001)      779 2023-05-22 07:01:38.000000 coop_html_editor-1.4.1/coop_html_editor/static/ckeditor.4.6.2/plugins/embedbase/lang/ko.js
+-rw-rw-r--   0 lucjean   (1001) lucjean   (1001)      964 2023-05-22 07:01:38.000000 coop_html_editor-1.4.1/coop_html_editor/static/ckeditor.4.6.2/plugins/embedbase/lang/ku.js
+-rw-rw-r--   0 lucjean   (1001) lucjean   (1001)      655 2023-05-22 07:01:38.000000 coop_html_editor-1.4.1/coop_html_editor/static/ckeditor.4.6.2/plugins/embedbase/lang/nb.js
+-rw-rw-r--   0 lucjean   (1001) lucjean   (1001)      686 2023-05-22 07:01:38.000000 coop_html_editor-1.4.1/coop_html_editor/static/ckeditor.4.6.2/plugins/embedbase/lang/nl.js
+-rw-rw-r--   0 lucjean   (1001) lucjean   (1001)      736 2023-05-22 07:01:38.000000 coop_html_editor-1.4.1/coop_html_editor/static/ckeditor.4.6.2/plugins/embedbase/lang/oc.js
+-rw-rw-r--   0 lucjean   (1001) lucjean   (1001)      767 2023-05-22 07:01:38.000000 coop_html_editor-1.4.1/coop_html_editor/static/ckeditor.4.6.2/plugins/embedbase/lang/pl.js
+-rw-rw-r--   0 lucjean   (1001) lucjean   (1001)      702 2023-05-22 07:01:38.000000 coop_html_editor-1.4.1/coop_html_editor/static/ckeditor.4.6.2/plugins/embedbase/lang/pt-br.js
+-rw-rw-r--   0 lucjean   (1001) lucjean   (1001)      725 2023-05-22 07:01:38.000000 coop_html_editor-1.4.1/coop_html_editor/static/ckeditor.4.6.2/plugins/embedbase/lang/pt.js
+-rw-rw-r--   0 lucjean   (1001) lucjean   (1001)      852 2023-05-22 07:01:38.000000 coop_html_editor-1.4.1/coop_html_editor/static/ckeditor.4.6.2/plugins/embedbase/lang/ru.js
+-rw-rw-r--   0 lucjean   (1001) lucjean   (1001)      669 2023-05-22 07:01:38.000000 coop_html_editor-1.4.1/coop_html_editor/static/ckeditor.4.6.2/plugins/embedbase/lang/sv.js
+-rw-rw-r--   0 lucjean   (1001) lucjean   (1001)      690 2023-05-22 07:01:38.000000 coop_html_editor-1.4.1/coop_html_editor/static/ckeditor.4.6.2/plugins/embedbase/lang/tr.js
+-rw-rw-r--   0 lucjean   (1001) lucjean   (1001)      768 2023-05-22 07:01:38.000000 coop_html_editor-1.4.1/coop_html_editor/static/ckeditor.4.6.2/plugins/embedbase/lang/ug.js
+-rw-rw-r--   0 lucjean   (1001) lucjean   (1001)      910 2023-05-22 07:01:38.000000 coop_html_editor-1.4.1/coop_html_editor/static/ckeditor.4.6.2/plugins/embedbase/lang/uk.js
+-rw-rw-r--   0 lucjean   (1001) lucjean   (1001)      573 2023-05-22 07:01:38.000000 coop_html_editor-1.4.1/coop_html_editor/static/ckeditor.4.6.2/plugins/embedbase/lang/zh-cn.js
+-rw-rw-r--   0 lucjean   (1001) lucjean   (1001)      626 2023-05-22 07:01:38.000000 coop_html_editor-1.4.1/coop_html_editor/static/ckeditor.4.6.2/plugins/embedbase/lang/zh.js
+-rw-rw-r--   0 lucjean   (1001) lucjean   (1001)    21596 2023-05-22 07:01:38.000000 coop_html_editor-1.4.1/coop_html_editor/static/ckeditor.4.6.2/plugins/embedbase/plugin.js
+-rw-rw-r--   0 lucjean   (1001) lucjean   (1001)     6057 2023-05-22 07:01:38.000000 coop_html_editor-1.4.1/coop_html_editor/static/ckeditor.4.6.2/plugins/icons.png
+-rw-rw-r--   0 lucjean   (1001) lucjean   (1001)    20877 2023-05-22 07:01:38.000000 coop_html_editor-1.4.1/coop_html_editor/static/ckeditor.4.6.2/plugins/icons_hidpi.png
+drwxrwxr-x   0 lucjean   (1001) lucjean   (1001)        0 2023-06-12 12:55:08.703912 coop_html_editor-1.4.1/coop_html_editor/static/ckeditor.4.6.2/plugins/image/
+drwxrwxr-x   0 lucjean   (1001) lucjean   (1001)        0 2023-06-12 12:55:08.751913 coop_html_editor-1.4.1/coop_html_editor/static/ckeditor.4.6.2/plugins/image/dialogs/
+-rw-rw-r--   0 lucjean   (1001) lucjean   (1001)    21266 2023-05-22 07:01:38.000000 coop_html_editor-1.4.1/coop_html_editor/static/ckeditor.4.6.2/plugins/image/dialogs/image.js
+drwxrwxr-x   0 lucjean   (1001) lucjean   (1001)        0 2023-06-12 12:55:08.755913 coop_html_editor-1.4.1/coop_html_editor/static/ckeditor.4.6.2/plugins/image/images/
+-rw-rw-r--   0 lucjean   (1001) lucjean   (1001)     1610 2023-05-22 07:01:38.000000 coop_html_editor-1.4.1/coop_html_editor/static/ckeditor.4.6.2/plugins/image/images/noimage.png
+drwxrwxr-x   0 lucjean   (1001) lucjean   (1001)        0 2023-06-12 12:55:08.755913 coop_html_editor-1.4.1/coop_html_editor/static/ckeditor.4.6.2/plugins/lineutils/
+drwxrwxr-x   0 lucjean   (1001) lucjean   (1001)        0 2023-06-12 12:55:08.755913 coop_html_editor-1.4.1/coop_html_editor/static/ckeditor.4.6.2/plugins/lineutils/dev/
+-rw-rw-r--   0 lucjean   (1001) lucjean   (1001)     7933 2023-05-22 07:01:38.000000 coop_html_editor-1.4.1/coop_html_editor/static/ckeditor.4.6.2/plugins/lineutils/dev/dnd.html
+-rw-rw-r--   0 lucjean   (1001) lucjean   (1001)     9083 2023-05-22 07:01:38.000000 coop_html_editor-1.4.1/coop_html_editor/static/ckeditor.4.6.2/plugins/lineutils/dev/magicfinger.html
+-rw-rw-r--   0 lucjean   (1001) lucjean   (1001)    28852 2023-05-22 07:01:38.000000 coop_html_editor-1.4.1/coop_html_editor/static/ckeditor.4.6.2/plugins/lineutils/plugin.js
+drwxrwxr-x   0 lucjean   (1001) lucjean   (1001)        0 2023-06-12 12:55:08.703912 coop_html_editor-1.4.1/coop_html_editor/static/ckeditor.4.6.2/plugins/link/
+drwxrwxr-x   0 lucjean   (1001) lucjean   (1001)        0 2023-06-12 12:55:08.755913 coop_html_editor-1.4.1/coop_html_editor/static/ckeditor.4.6.2/plugins/link/dialogs/
+-rw-rw-r--   0 lucjean   (1001) lucjean   (1001)     1629 2023-05-22 07:01:38.000000 coop_html_editor-1.4.1/coop_html_editor/static/ckeditor.4.6.2/plugins/link/dialogs/anchor.js
+-rw-rw-r--   0 lucjean   (1001) lucjean   (1001)    12093 2023-05-22 07:01:38.000000 coop_html_editor-1.4.1/coop_html_editor/static/ckeditor.4.6.2/plugins/link/dialogs/link.js
+drwxrwxr-x   0 lucjean   (1001) lucjean   (1001)        0 2023-06-12 12:55:08.755913 coop_html_editor-1.4.1/coop_html_editor/static/ckeditor.4.6.2/plugins/link/images/
+-rw-rw-r--   0 lucjean   (1001) lucjean   (1001)      752 2023-05-22 07:01:38.000000 coop_html_editor-1.4.1/coop_html_editor/static/ckeditor.4.6.2/plugins/link/images/anchor.png
+drwxrwxr-x   0 lucjean   (1001) lucjean   (1001)        0 2023-06-12 12:55:08.755913 coop_html_editor-1.4.1/coop_html_editor/static/ckeditor.4.6.2/plugins/link/images/hidpi/
+-rw-rw-r--   0 lucjean   (1001) lucjean   (1001)     1109 2023-05-22 07:01:38.000000 coop_html_editor-1.4.1/coop_html_editor/static/ckeditor.4.6.2/plugins/link/images/hidpi/anchor.png
+drwxrwxr-x   0 lucjean   (1001) lucjean   (1001)        0 2023-06-12 12:55:08.703912 coop_html_editor-1.4.1/coop_html_editor/static/ckeditor.4.6.2/plugins/magicline/
+drwxrwxr-x   0 lucjean   (1001) lucjean   (1001)        0 2023-06-12 12:55:08.755913 coop_html_editor-1.4.1/coop_html_editor/static/ckeditor.4.6.2/plugins/magicline/images/
+drwxrwxr-x   0 lucjean   (1001) lucjean   (1001)        0 2023-06-12 12:55:08.755913 coop_html_editor-1.4.1/coop_html_editor/static/ckeditor.4.6.2/plugins/magicline/images/hidpi/
+-rw-rw-r--   0 lucjean   (1001) lucjean   (1001)      176 2023-05-22 07:01:38.000000 coop_html_editor-1.4.1/coop_html_editor/static/ckeditor.4.6.2/plugins/magicline/images/hidpi/icon-rtl.png
+-rw-rw-r--   0 lucjean   (1001) lucjean   (1001)      199 2023-05-22 07:01:38.000000 coop_html_editor-1.4.1/coop_html_editor/static/ckeditor.4.6.2/plugins/magicline/images/hidpi/icon.png
+-rw-rw-r--   0 lucjean   (1001) lucjean   (1001)      138 2023-05-22 07:01:38.000000 coop_html_editor-1.4.1/coop_html_editor/static/ckeditor.4.6.2/plugins/magicline/images/icon-rtl.png
+-rw-rw-r--   0 lucjean   (1001) lucjean   (1001)      133 2023-05-22 07:01:38.000000 coop_html_editor-1.4.1/coop_html_editor/static/ckeditor.4.6.2/plugins/magicline/images/icon.png
+drwxrwxr-x   0 lucjean   (1001) lucjean   (1001)        0 2023-06-12 12:55:08.755913 coop_html_editor-1.4.1/coop_html_editor/static/ckeditor.4.6.2/plugins/notification/
+drwxrwxr-x   0 lucjean   (1001) lucjean   (1001)        0 2023-06-12 12:55:08.759913 coop_html_editor-1.4.1/coop_html_editor/static/ckeditor.4.6.2/plugins/notification/lang/
+-rw-rw-r--   0 lucjean   (1001) lucjean   (1001)      248 2023-05-22 07:01:38.000000 coop_html_editor-1.4.1/coop_html_editor/static/ckeditor.4.6.2/plugins/notification/lang/az.js
+-rw-rw-r--   0 lucjean   (1001) lucjean   (1001)      231 2023-05-22 07:01:38.000000 coop_html_editor-1.4.1/coop_html_editor/static/ckeditor.4.6.2/plugins/notification/lang/ca.js
+-rw-rw-r--   0 lucjean   (1001) lucjean   (1001)      230 2023-05-22 07:01:38.000000 coop_html_editor-1.4.1/coop_html_editor/static/ckeditor.4.6.2/plugins/notification/lang/cs.js
+-rw-rw-r--   0 lucjean   (1001) lucjean   (1001)      230 2023-05-22 07:01:38.000000 coop_html_editor-1.4.1/coop_html_editor/static/ckeditor.4.6.2/plugins/notification/lang/da.js
+-rw-rw-r--   0 lucjean   (1001) lucjean   (1001)      242 2023-05-22 07:01:38.000000 coop_html_editor-1.4.1/coop_html_editor/static/ckeditor.4.6.2/plugins/notification/lang/de-ch.js
+-rw-rw-r--   0 lucjean   (1001) lucjean   (1001)      239 2023-05-22 07:01:38.000000 coop_html_editor-1.4.1/coop_html_editor/static/ckeditor.4.6.2/plugins/notification/lang/de.js
+-rw-rw-r--   0 lucjean   (1001) lucjean   (1001)      230 2023-05-22 07:01:38.000000 coop_html_editor-1.4.1/coop_html_editor/static/ckeditor.4.6.2/plugins/notification/lang/en.js
+-rw-rw-r--   0 lucjean   (1001) lucjean   (1001)      224 2023-05-22 07:01:38.000000 coop_html_editor-1.4.1/coop_html_editor/static/ckeditor.4.6.2/plugins/notification/lang/eo.js
+-rw-rw-r--   0 lucjean   (1001) lucjean   (1001)      232 2023-05-22 07:01:38.000000 coop_html_editor-1.4.1/coop_html_editor/static/ckeditor.4.6.2/plugins/notification/lang/es.js
+-rw-rw-r--   0 lucjean   (1001) lucjean   (1001)      231 2023-05-22 07:01:38.000000 coop_html_editor-1.4.1/coop_html_editor/static/ckeditor.4.6.2/plugins/notification/lang/eu.js
+-rw-rw-r--   0 lucjean   (1001) lucjean   (1001)      231 2023-05-22 07:01:38.000000 coop_html_editor-1.4.1/coop_html_editor/static/ckeditor.4.6.2/plugins/notification/lang/fr.js
+-rw-rw-r--   0 lucjean   (1001) lucjean   (1001)      232 2023-05-22 07:01:38.000000 coop_html_editor-1.4.1/coop_html_editor/static/ckeditor.4.6.2/plugins/notification/lang/gl.js
+-rw-rw-r--   0 lucjean   (1001) lucjean   (1001)      231 2023-05-22 07:01:38.000000 coop_html_editor-1.4.1/coop_html_editor/static/ckeditor.4.6.2/plugins/notification/lang/id.js
+-rw-rw-r--   0 lucjean   (1001) lucjean   (1001)      226 2023-05-22 07:01:38.000000 coop_html_editor-1.4.1/coop_html_editor/static/ckeditor.4.6.2/plugins/notification/lang/it.js
+-rw-rw-r--   0 lucjean   (1001) lucjean   (1001)      237 2023-05-22 07:01:38.000000 coop_html_editor-1.4.1/coop_html_editor/static/ckeditor.4.6.2/plugins/notification/lang/ja.js
+-rw-rw-r--   0 lucjean   (1001) lucjean   (1001)      282 2023-05-22 07:01:38.000000 coop_html_editor-1.4.1/coop_html_editor/static/ckeditor.4.6.2/plugins/notification/lang/km.js
+-rw-rw-r--   0 lucjean   (1001) lucjean   (1001)      227 2023-05-22 07:01:38.000000 coop_html_editor-1.4.1/coop_html_editor/static/ckeditor.4.6.2/plugins/notification/lang/ko.js
+-rw-rw-r--   0 lucjean   (1001) lucjean   (1001)      252 2023-05-22 07:01:38.000000 coop_html_editor-1.4.1/coop_html_editor/static/ckeditor.4.6.2/plugins/notification/lang/ku.js
+-rw-rw-r--   0 lucjean   (1001) lucjean   (1001)      226 2023-05-22 07:01:38.000000 coop_html_editor-1.4.1/coop_html_editor/static/ckeditor.4.6.2/plugins/notification/lang/nb.js
+-rw-rw-r--   0 lucjean   (1001) lucjean   (1001)      227 2023-05-22 07:01:38.000000 coop_html_editor-1.4.1/coop_html_editor/static/ckeditor.4.6.2/plugins/notification/lang/nl.js
+-rw-rw-r--   0 lucjean   (1001) lucjean   (1001)      231 2023-05-22 07:01:38.000000 coop_html_editor-1.4.1/coop_html_editor/static/ckeditor.4.6.2/plugins/notification/lang/oc.js
+-rw-rw-r--   0 lucjean   (1001) lucjean   (1001)      244 2023-05-22 07:01:38.000000 coop_html_editor-1.4.1/coop_html_editor/static/ckeditor.4.6.2/plugins/notification/lang/pl.js
+-rw-rw-r--   0 lucjean   (1001) lucjean   (1001)      235 2023-05-22 07:01:38.000000 coop_html_editor-1.4.1/coop_html_editor/static/ckeditor.4.6.2/plugins/notification/lang/pt-br.js
+-rw-rw-r--   0 lucjean   (1001) lucjean   (1001)      234 2023-05-22 07:01:38.000000 coop_html_editor-1.4.1/coop_html_editor/static/ckeditor.4.6.2/plugins/notification/lang/pt.js
+-rw-rw-r--   0 lucjean   (1001) lucjean   (1001)      247 2023-05-22 07:01:38.000000 coop_html_editor-1.4.1/coop_html_editor/static/ckeditor.4.6.2/plugins/notification/lang/ru.js
+-rw-rw-r--   0 lucjean   (1001) lucjean   (1001)      230 2023-05-22 07:01:38.000000 coop_html_editor-1.4.1/coop_html_editor/static/ckeditor.4.6.2/plugins/notification/lang/sv.js
+-rw-rw-r--   0 lucjean   (1001) lucjean   (1001)      232 2023-05-22 07:01:38.000000 coop_html_editor-1.4.1/coop_html_editor/static/ckeditor.4.6.2/plugins/notification/lang/tr.js
+-rw-rw-r--   0 lucjean   (1001) lucjean   (1001)      242 2023-05-22 07:01:38.000000 coop_html_editor-1.4.1/coop_html_editor/static/ckeditor.4.6.2/plugins/notification/lang/ug.js
+-rw-rw-r--   0 lucjean   (1001) lucjean   (1001)      246 2023-05-22 07:01:38.000000 coop_html_editor-1.4.1/coop_html_editor/static/ckeditor.4.6.2/plugins/notification/lang/uk.js
+-rw-rw-r--   0 lucjean   (1001) lucjean   (1001)      228 2023-05-22 07:01:38.000000 coop_html_editor-1.4.1/coop_html_editor/static/ckeditor.4.6.2/plugins/notification/lang/zh-cn.js
+-rw-rw-r--   0 lucjean   (1001) lucjean   (1001)      228 2023-05-22 07:01:38.000000 coop_html_editor-1.4.1/coop_html_editor/static/ckeditor.4.6.2/plugins/notification/lang/zh.js
+-rw-rw-r--   0 lucjean   (1001) lucjean   (1001)    33609 2023-05-22 07:01:38.000000 coop_html_editor-1.4.1/coop_html_editor/static/ckeditor.4.6.2/plugins/notification/plugin.js
+drwxrwxr-x   0 lucjean   (1001) lucjean   (1001)        0 2023-06-12 12:55:08.759913 coop_html_editor-1.4.1/coop_html_editor/static/ckeditor.4.6.2/plugins/notificationaggregator/
+-rw-rw-r--   0 lucjean   (1001) lucjean   (1001)    15081 2023-05-22 07:01:38.000000 coop_html_editor-1.4.1/coop_html_editor/static/ckeditor.4.6.2/plugins/notificationaggregator/plugin.js
+drwxrwxr-x   0 lucjean   (1001) lucjean   (1001)        0 2023-06-12 12:55:08.703912 coop_html_editor-1.4.1/coop_html_editor/static/ckeditor.4.6.2/plugins/pastefromword/
+drwxrwxr-x   0 lucjean   (1001) lucjean   (1001)        0 2023-06-12 12:55:08.763913 coop_html_editor-1.4.1/coop_html_editor/static/ckeditor.4.6.2/plugins/pastefromword/filter/
+-rw-rw-r--   0 lucjean   (1001) lucjean   (1001)    19971 2023-05-22 07:01:38.000000 coop_html_editor-1.4.1/coop_html_editor/static/ckeditor.4.6.2/plugins/pastefromword/filter/default.js
+drwxrwxr-x   0 lucjean   (1001) lucjean   (1001)        0 2023-06-12 12:55:08.763913 coop_html_editor-1.4.1/coop_html_editor/static/ckeditor.4.6.2/plugins/scayt/
+-rw-rw-r--   0 lucjean   (1001) lucjean   (1001)     1451 2023-05-22 07:01:38.000000 coop_html_editor-1.4.1/coop_html_editor/static/ckeditor.4.6.2/plugins/scayt/CHANGELOG.md
+-rw-rw-r--   0 lucjean   (1001) lucjean   (1001)     1476 2023-05-22 07:01:38.000000 coop_html_editor-1.4.1/coop_html_editor/static/ckeditor.4.6.2/plugins/scayt/LICENSE.md
+-rw-rw-r--   0 lucjean   (1001) lucjean   (1001)      979 2023-05-22 07:01:38.000000 coop_html_editor-1.4.1/coop_html_editor/static/ckeditor.4.6.2/plugins/scayt/README.md
+drwxrwxr-x   0 lucjean   (1001) lucjean   (1001)        0 2023-06-12 12:55:08.763913 coop_html_editor-1.4.1/coop_html_editor/static/ckeditor.4.6.2/plugins/scayt/dialogs/
+-rw-rw-r--   0 lucjean   (1001) lucjean   (1001)     9577 2023-05-22 07:01:38.000000 coop_html_editor-1.4.1/coop_html_editor/static/ckeditor.4.6.2/plugins/scayt/dialogs/options.js
+-rw-rw-r--   0 lucjean   (1001) lucjean   (1001)     1302 2023-05-22 07:01:38.000000 coop_html_editor-1.4.1/coop_html_editor/static/ckeditor.4.6.2/plugins/scayt/dialogs/toolbar.css
+drwxrwxr-x   0 lucjean   (1001) lucjean   (1001)        0 2023-06-12 12:55:08.703912 coop_html_editor-1.4.1/coop_html_editor/static/ckeditor.4.6.2/plugins/scayt/skins/
+drwxrwxr-x   0 lucjean   (1001) lucjean   (1001)        0 2023-06-12 12:55:08.763913 coop_html_editor-1.4.1/coop_html_editor/static/ckeditor.4.6.2/plugins/scayt/skins/moono-lisa/
+-rw-rw-r--   0 lucjean   (1001) lucjean   (1001)      330 2023-05-22 07:01:38.000000 coop_html_editor-1.4.1/coop_html_editor/static/ckeditor.4.6.2/plugins/scayt/skins/moono-lisa/scayt.css
+drwxrwxr-x   0 lucjean   (1001) lucjean   (1001)        0 2023-06-12 12:55:08.763913 coop_html_editor-1.4.1/coop_html_editor/static/ckeditor.4.6.2/plugins/sourcedialog/
+drwxrwxr-x   0 lucjean   (1001) lucjean   (1001)        0 2023-06-12 12:55:08.763913 coop_html_editor-1.4.1/coop_html_editor/static/ckeditor.4.6.2/plugins/sourcedialog/dialogs/
+-rw-rw-r--   0 lucjean   (1001) lucjean   (1001)     2204 2023-05-22 07:01:38.000000 coop_html_editor-1.4.1/coop_html_editor/static/ckeditor.4.6.2/plugins/sourcedialog/dialogs/sourcedialog.js
+drwxrwxr-x   0 lucjean   (1001) lucjean   (1001)        0 2023-06-12 12:55:08.775913 coop_html_editor-1.4.1/coop_html_editor/static/ckeditor.4.6.2/plugins/sourcedialog/lang/
+-rw-rw-r--   0 lucjean   (1001) lucjean   (1001)      232 2023-05-22 07:01:38.000000 coop_html_editor-1.4.1/coop_html_editor/static/ckeditor.4.6.2/plugins/sourcedialog/lang/af.js
+-rw-rw-r--   0 lucjean   (1001) lucjean   (1001)      248 2023-05-22 07:01:38.000000 coop_html_editor-1.4.1/coop_html_editor/static/ckeditor.4.6.2/plugins/sourcedialog/lang/ar.js
+-rw-rw-r--   0 lucjean   (1001) lucjean   (1001)      238 2023-05-22 07:01:38.000000 coop_html_editor-1.4.1/coop_html_editor/static/ckeditor.4.6.2/plugins/sourcedialog/lang/az.js
+-rw-rw-r--   0 lucjean   (1001) lucjean   (1001)      256 2023-05-22 07:01:38.000000 coop_html_editor-1.4.1/coop_html_editor/static/ckeditor.4.6.2/plugins/sourcedialog/lang/bg.js
+-rw-rw-r--   0 lucjean   (1001) lucjean   (1001)      248 2023-05-22 07:01:38.000000 coop_html_editor-1.4.1/coop_html_editor/static/ckeditor.4.6.2/plugins/sourcedialog/lang/bn.js
+-rw-rw-r--   0 lucjean   (1001) lucjean   (1001)      242 2023-05-22 07:01:38.000000 coop_html_editor-1.4.1/coop_html_editor/static/ckeditor.4.6.2/plugins/sourcedialog/lang/bs.js
+-rw-rw-r--   0 lucjean   (1001) lucjean   (1001)      242 2023-05-22 07:01:38.000000 coop_html_editor-1.4.1/coop_html_editor/static/ckeditor.4.6.2/plugins/sourcedialog/lang/ca.js
+-rw-rw-r--   0 lucjean   (1001) lucjean   (1001)      234 2023-05-22 07:01:38.000000 coop_html_editor-1.4.1/coop_html_editor/static/ckeditor.4.6.2/plugins/sourcedialog/lang/cs.js
+-rw-rw-r--   0 lucjean   (1001) lucjean   (1001)      232 2023-05-22 07:01:38.000000 coop_html_editor-1.4.1/coop_html_editor/static/ckeditor.4.6.2/plugins/sourcedialog/lang/cy.js
+-rw-rw-r--   0 lucjean   (1001) lucjean   (1001)      234 2023-05-22 07:01:38.000000 coop_html_editor-1.4.1/coop_html_editor/static/ckeditor.4.6.2/plugins/sourcedialog/lang/da.js
+-rw-rw-r--   0 lucjean   (1001) lucjean   (1001)      245 2023-05-22 07:01:38.000000 coop_html_editor-1.4.1/coop_html_editor/static/ckeditor.4.6.2/plugins/sourcedialog/lang/de-ch.js
+-rw-rw-r--   0 lucjean   (1001) lucjean   (1001)      242 2023-05-22 07:01:38.000000 coop_html_editor-1.4.1/coop_html_editor/static/ckeditor.4.6.2/plugins/sourcedialog/lang/de.js
+-rw-rw-r--   0 lucjean   (1001) lucjean   (1001)      252 2023-05-22 07:01:38.000000 coop_html_editor-1.4.1/coop_html_editor/static/ckeditor.4.6.2/plugins/sourcedialog/lang/el.js
+-rw-rw-r--   0 lucjean   (1001) lucjean   (1001)      239 2023-05-22 07:01:38.000000 coop_html_editor-1.4.1/coop_html_editor/static/ckeditor.4.6.2/plugins/sourcedialog/lang/en-au.js
+-rw-rw-r--   0 lucjean   (1001) lucjean   (1001)      239 2023-05-22 07:01:38.000000 coop_html_editor-1.4.1/coop_html_editor/static/ckeditor.4.6.2/plugins/sourcedialog/lang/en-ca.js
+-rw-rw-r--   0 lucjean   (1001) lucjean   (1001)      239 2023-05-22 07:01:38.000000 coop_html_editor-1.4.1/coop_html_editor/static/ckeditor.4.6.2/plugins/sourcedialog/lang/en-gb.js
+-rw-rw-r--   0 lucjean   (1001) lucjean   (1001)      236 2023-05-22 07:01:38.000000 coop_html_editor-1.4.1/coop_html_editor/static/ckeditor.4.6.2/plugins/sourcedialog/lang/en.js
+-rw-rw-r--   0 lucjean   (1001) lucjean   (1001)      234 2023-05-22 07:01:38.000000 coop_html_editor-1.4.1/coop_html_editor/static/ckeditor.4.6.2/plugins/sourcedialog/lang/eo.js
+-rw-rw-r--   0 lucjean   (1001) lucjean   (1001)      246 2023-05-22 07:01:38.000000 coop_html_editor-1.4.1/coop_html_editor/static/ckeditor.4.6.2/plugins/sourcedialog/lang/es.js
+-rw-rw-r--   0 lucjean   (1001) lucjean   (1001)      244 2023-05-22 07:01:38.000000 coop_html_editor-1.4.1/coop_html_editor/static/ckeditor.4.6.2/plugins/sourcedialog/lang/et.js
+-rw-rw-r--   0 lucjean   (1001) lucjean   (1001)      242 2023-05-22 07:01:38.000000 coop_html_editor-1.4.1/coop_html_editor/static/ckeditor.4.6.2/plugins/sourcedialog/lang/eu.js
+-rw-rw-r--   0 lucjean   (1001) lucjean   (1001)      240 2023-05-22 07:01:38.000000 coop_html_editor-1.4.1/coop_html_editor/static/ckeditor.4.6.2/plugins/sourcedialog/lang/fa.js
+-rw-rw-r--   0 lucjean   (1001) lucjean   (1001)      234 2023-05-22 07:01:38.000000 coop_html_editor-1.4.1/coop_html_editor/static/ckeditor.4.6.2/plugins/sourcedialog/lang/fi.js
+-rw-rw-r--   0 lucjean   (1001) lucjean   (1001)      234 2023-05-22 07:01:38.000000 coop_html_editor-1.4.1/coop_html_editor/static/ckeditor.4.6.2/plugins/sourcedialog/lang/fo.js
+-rw-rw-r--   0 lucjean   (1001) lucjean   (1001)      239 2023-05-22 07:01:38.000000 coop_html_editor-1.4.1/coop_html_editor/static/ckeditor.4.6.2/plugins/sourcedialog/lang/fr-ca.js
+-rw-rw-r--   0 lucjean   (1001) lucjean   (1001)      236 2023-05-22 07:01:38.000000 coop_html_editor-1.4.1/coop_html_editor/static/ckeditor.4.6.2/plugins/sourcedialog/lang/fr.js
+-rw-rw-r--   0 lucjean   (1001) lucjean   (1001)      234 2023-05-22 07:01:38.000000 coop_html_editor-1.4.1/coop_html_editor/static/ckeditor.4.6.2/plugins/sourcedialog/lang/gl.js
+-rw-rw-r--   0 lucjean   (1001) lucjean   (1001)      356 2023-05-22 07:01:38.000000 coop_html_editor-1.4.1/coop_html_editor/static/ckeditor.4.6.2/plugins/sourcedialog/lang/gu.js
+-rw-rw-r--   0 lucjean   (1001) lucjean   (1001)      240 2023-05-22 07:01:38.000000 coop_html_editor-1.4.1/coop_html_editor/static/ckeditor.4.6.2/plugins/sourcedialog/lang/he.js
+-rw-rw-r--   0 lucjean   (1001) lucjean   (1001)      254 2023-05-22 07:01:38.000000 coop_html_editor-1.4.1/coop_html_editor/static/ckeditor.4.6.2/plugins/sourcedialog/lang/hi.js
+-rw-rw-r--   0 lucjean   (1001) lucjean   (1001)      232 2023-05-22 07:01:38.000000 coop_html_editor-1.4.1/coop_html_editor/static/ckeditor.4.6.2/plugins/sourcedialog/lang/hr.js
+-rw-rw-r--   0 lucjean   (1001) lucjean   (1001)      246 2023-05-22 07:01:38.000000 coop_html_editor-1.4.1/coop_html_editor/static/ckeditor.4.6.2/plugins/sourcedialog/lang/hu.js
+-rw-rw-r--   0 lucjean   (1001) lucjean   (1001)      236 2023-05-22 07:01:38.000000 coop_html_editor-1.4.1/coop_html_editor/static/ckeditor.4.6.2/plugins/sourcedialog/lang/id.js
+-rw-rw-r--   0 lucjean   (1001) lucjean   (1001)      236 2023-05-22 07:01:38.000000 coop_html_editor-1.4.1/coop_html_editor/static/ckeditor.4.6.2/plugins/sourcedialog/lang/is.js
+-rw-rw-r--   0 lucjean   (1001) lucjean   (1001)      240 2023-05-22 07:01:38.000000 coop_html_editor-1.4.1/coop_html_editor/static/ckeditor.4.6.2/plugins/sourcedialog/lang/it.js
+-rw-rw-r--   0 lucjean   (1001) lucjean   (1001)      242 2023-05-22 07:01:38.000000 coop_html_editor-1.4.1/coop_html_editor/static/ckeditor.4.6.2/plugins/sourcedialog/lang/ja.js
+-rw-rw-r--   0 lucjean   (1001) lucjean   (1001)      260 2023-05-22 07:01:38.000000 coop_html_editor-1.4.1/coop_html_editor/static/ckeditor.4.6.2/plugins/sourcedialog/lang/ka.js
+-rw-rw-r--   0 lucjean   (1001) lucjean   (1001)      278 2023-05-22 07:01:38.000000 coop_html_editor-1.4.1/coop_html_editor/static/ckeditor.4.6.2/plugins/sourcedialog/lang/km.js
+-rw-rw-r--   0 lucjean   (1001) lucjean   (1001)      236 2023-05-22 07:01:38.000000 coop_html_editor-1.4.1/coop_html_editor/static/ckeditor.4.6.2/plugins/sourcedialog/lang/ko.js
+-rw-rw-r--   0 lucjean   (1001) lucjean   (1001)      252 2023-05-22 07:01:38.000000 coop_html_editor-1.4.1/coop_html_editor/static/ckeditor.4.6.2/plugins/sourcedialog/lang/ku.js
+-rw-rw-r--   0 lucjean   (1001) lucjean   (1001)      242 2023-05-22 07:01:38.000000 coop_html_editor-1.4.1/coop_html_editor/static/ckeditor.4.6.2/plugins/sourcedialog/lang/lt.js
+-rw-rw-r--   0 lucjean   (1001) lucjean   (1001)      242 2023-05-22 07:01:38.000000 coop_html_editor-1.4.1/coop_html_editor/static/ckeditor.4.6.2/plugins/sourcedialog/lang/lv.js
+-rw-rw-r--   0 lucjean   (1001) lucjean   (1001)      236 2023-05-22 07:01:38.000000 coop_html_editor-1.4.1/coop_html_editor/static/ckeditor.4.6.2/plugins/sourcedialog/lang/mn.js
+-rw-rw-r--   0 lucjean   (1001) lucjean   (1001)      236 2023-05-22 07:01:38.000000 coop_html_editor-1.4.1/coop_html_editor/static/ckeditor.4.6.2/plugins/sourcedialog/lang/ms.js
+-rw-rw-r--   0 lucjean   (1001) lucjean   (1001)      234 2023-05-22 07:01:38.000000 coop_html_editor-1.4.1/coop_html_editor/static/ckeditor.4.6.2/plugins/sourcedialog/lang/nb.js
+-rw-rw-r--   0 lucjean   (1001) lucjean   (1001)      240 2023-05-22 07:01:38.000000 coop_html_editor-1.4.1/coop_html_editor/static/ckeditor.4.6.2/plugins/sourcedialog/lang/nl.js
+-rw-rw-r--   0 lucjean   (1001) lucjean   (1001)      234 2023-05-22 07:01:38.000000 coop_html_editor-1.4.1/coop_html_editor/static/ckeditor.4.6.2/plugins/sourcedialog/lang/no.js
+-rw-rw-r--   0 lucjean   (1001) lucjean   (1001)      232 2023-05-22 07:01:38.000000 coop_html_editor-1.4.1/coop_html_editor/static/ckeditor.4.6.2/plugins/sourcedialog/lang/oc.js
+-rw-rw-r--   0 lucjean   (1001) lucjean   (1001)      262 2023-05-22 07:01:38.000000 coop_html_editor-1.4.1/coop_html_editor/static/ckeditor.4.6.2/plugins/sourcedialog/lang/pl.js
+-rw-rw-r--   0 lucjean   (1001) lucjean   (1001)      253 2023-05-22 07:01:38.000000 coop_html_editor-1.4.1/coop_html_editor/static/ckeditor.4.6.2/plugins/sourcedialog/lang/pt-br.js
+-rw-rw-r--   0 lucjean   (1001) lucjean   (1001)      234 2023-05-22 07:01:38.000000 coop_html_editor-1.4.1/coop_html_editor/static/ckeditor.4.6.2/plugins/sourcedialog/lang/pt.js
+-rw-rw-r--   0 lucjean   (1001) lucjean   (1001)      234 2023-05-22 07:01:38.000000 coop_html_editor-1.4.1/coop_html_editor/static/ckeditor.4.6.2/plugins/sourcedialog/lang/ro.js
+-rw-rw-r--   0 lucjean   (1001) lucjean   (1001)      256 2023-05-22 07:01:38.000000 coop_html_editor-1.4.1/coop_html_editor/static/ckeditor.4.6.2/plugins/sourcedialog/lang/ru.js
+-rw-rw-r--   0 lucjean   (1001) lucjean   (1001)      278 2023-05-22 07:01:38.000000 coop_html_editor-1.4.1/coop_html_editor/static/ckeditor.4.6.2/plugins/sourcedialog/lang/si.js
+-rw-rw-r--   0 lucjean   (1001) lucjean   (1001)      234 2023-05-22 07:01:38.000000 coop_html_editor-1.4.1/coop_html_editor/static/ckeditor.4.6.2/plugins/sourcedialog/lang/sk.js
+-rw-rw-r--   0 lucjean   (1001) lucjean   (1001)      248 2023-05-22 07:01:38.000000 coop_html_editor-1.4.1/coop_html_editor/static/ckeditor.4.6.2/plugins/sourcedialog/lang/sl.js
+-rw-rw-r--   0 lucjean   (1001) lucjean   (1001)      236 2023-05-22 07:01:38.000000 coop_html_editor-1.4.1/coop_html_editor/static/ckeditor.4.6.2/plugins/sourcedialog/lang/sq.js
+-rw-rw-r--   0 lucjean   (1001) lucjean   (1001)      237 2023-05-22 07:01:38.000000 coop_html_editor-1.4.1/coop_html_editor/static/ckeditor.4.6.2/plugins/sourcedialog/lang/sr-latn.js
+-rw-rw-r--   0 lucjean   (1001) lucjean   (1001)      234 2023-05-22 07:01:38.000000 coop_html_editor-1.4.1/coop_html_editor/static/ckeditor.4.6.2/plugins/sourcedialog/lang/sr.js
+-rw-rw-r--   0 lucjean   (1001) lucjean   (1001)      236 2023-05-22 07:01:38.000000 coop_html_editor-1.4.1/coop_html_editor/static/ckeditor.4.6.2/plugins/sourcedialog/lang/sv.js
+-rw-rw-r--   0 lucjean   (1001) lucjean   (1001)      270 2023-05-22 07:01:38.000000 coop_html_editor-1.4.1/coop_html_editor/static/ckeditor.4.6.2/plugins/sourcedialog/lang/th.js
+-rw-rw-r--   0 lucjean   (1001) lucjean   (1001)      236 2023-05-22 07:01:38.000000 coop_html_editor-1.4.1/coop_html_editor/static/ckeditor.4.6.2/plugins/sourcedialog/lang/tr.js
+-rw-rw-r--   0 lucjean   (1001) lucjean   (1001)      252 2023-05-22 07:01:38.000000 coop_html_editor-1.4.1/coop_html_editor/static/ckeditor.4.6.2/plugins/sourcedialog/lang/tt.js
+-rw-rw-r--   0 lucjean   (1001) lucjean   (1001)      244 2023-05-22 07:01:38.000000 coop_html_editor-1.4.1/coop_html_editor/static/ckeditor.4.6.2/plugins/sourcedialog/lang/ug.js
+-rw-rw-r--   0 lucjean   (1001) lucjean   (1001)      252 2023-05-22 07:01:38.000000 coop_html_editor-1.4.1/coop_html_editor/static/ckeditor.4.6.2/plugins/sourcedialog/lang/uk.js
+-rw-rw-r--   0 lucjean   (1001) lucjean   (1001)      240 2023-05-22 07:01:38.000000 coop_html_editor-1.4.1/coop_html_editor/static/ckeditor.4.6.2/plugins/sourcedialog/lang/vi.js
+-rw-rw-r--   0 lucjean   (1001) lucjean   (1001)      239 2023-05-22 07:01:38.000000 coop_html_editor-1.4.1/coop_html_editor/static/ckeditor.4.6.2/plugins/sourcedialog/lang/zh-cn.js
+-rw-rw-r--   0 lucjean   (1001) lucjean   (1001)      242 2023-05-22 07:01:38.000000 coop_html_editor-1.4.1/coop_html_editor/static/ckeditor.4.6.2/plugins/sourcedialog/lang/zh.js
+-rw-rw-r--   0 lucjean   (1001) lucjean   (1001)     1193 2023-05-22 07:01:38.000000 coop_html_editor-1.4.1/coop_html_editor/static/ckeditor.4.6.2/plugins/sourcedialog/plugin.js
+drwxrwxr-x   0 lucjean   (1001) lucjean   (1001)        0 2023-06-12 12:55:08.775913 coop_html_editor-1.4.1/coop_html_editor/static/ckeditor.4.6.2/plugins/sourcedialog/samples/
+-rw-rw-r--   0 lucjean   (1001) lucjean   (1001)     3907 2023-05-22 07:01:38.000000 coop_html_editor-1.4.1/coop_html_editor/static/ckeditor.4.6.2/plugins/sourcedialog/samples/sourcedialog.html
+drwxrwxr-x   0 lucjean   (1001) lucjean   (1001)        0 2023-06-12 12:55:08.703912 coop_html_editor-1.4.1/coop_html_editor/static/ckeditor.4.6.2/plugins/specialchar/
+drwxrwxr-x   0 lucjean   (1001) lucjean   (1001)        0 2023-06-12 12:55:08.775913 coop_html_editor-1.4.1/coop_html_editor/static/ckeditor.4.6.2/plugins/specialchar/dialogs/
+drwxrwxr-x   0 lucjean   (1001) lucjean   (1001)        0 2023-06-12 12:55:08.783913 coop_html_editor-1.4.1/coop_html_editor/static/ckeditor.4.6.2/plugins/specialchar/dialogs/lang/
+-rw-rw-r--   0 lucjean   (1001) lucjean   (1001)      720 2023-05-22 07:01:38.000000 coop_html_editor-1.4.1/coop_html_editor/static/ckeditor.4.6.2/plugins/specialchar/dialogs/lang/_translationstatus.txt
+-rw-rw-r--   0 lucjean   (1001) lucjean   (1001)     4529 2023-05-22 07:01:38.000000 coop_html_editor-1.4.1/coop_html_editor/static/ckeditor.4.6.2/plugins/specialchar/dialogs/lang/af.js
+-rw-rw-r--   0 lucjean   (1001) lucjean   (1001)     4778 2023-05-22 07:01:38.000000 coop_html_editor-1.4.1/coop_html_editor/static/ckeditor.4.6.2/plugins/specialchar/dialogs/lang/ar.js
+-rw-rw-r--   0 lucjean   (1001) lucjean   (1001)     3389 2023-05-22 07:01:38.000000 coop_html_editor-1.4.1/coop_html_editor/static/ckeditor.4.6.2/plugins/specialchar/dialogs/lang/az.js
+-rw-rw-r--   0 lucjean   (1001) lucjean   (1001)     4735 2023-05-22 07:01:38.000000 coop_html_editor-1.4.1/coop_html_editor/static/ckeditor.4.6.2/plugins/specialchar/dialogs/lang/bg.js
+-rw-rw-r--   0 lucjean   (1001) lucjean   (1001)     5010 2023-05-22 07:01:38.000000 coop_html_editor-1.4.1/coop_html_editor/static/ckeditor.4.6.2/plugins/specialchar/dialogs/lang/ca.js
+-rw-rw-r--   0 lucjean   (1001) lucjean   (1001)     4967 2023-05-22 07:01:38.000000 coop_html_editor-1.4.1/coop_html_editor/static/ckeditor.4.6.2/plugins/specialchar/dialogs/lang/cs.js
+-rw-rw-r--   0 lucjean   (1001) lucjean   (1001)     4891 2023-05-22 07:01:38.000000 coop_html_editor-1.4.1/coop_html_editor/static/ckeditor.4.6.2/plugins/specialchar/dialogs/lang/cy.js
+-rw-rw-r--   0 lucjean   (1001) lucjean   (1001)     3360 2023-05-22 07:01:38.000000 coop_html_editor-1.4.1/coop_html_editor/static/ckeditor.4.6.2/plugins/specialchar/dialogs/lang/da.js
+-rw-rw-r--   0 lucjean   (1001) lucjean   (1001)     4783 2023-05-22 07:01:38.000000 coop_html_editor-1.4.1/coop_html_editor/static/ckeditor.4.6.2/plugins/specialchar/dialogs/lang/de-ch.js
+-rw-rw-r--   0 lucjean   (1001) lucjean   (1001)     4780 2023-05-22 07:01:38.000000 coop_html_editor-1.4.1/coop_html_editor/static/ckeditor.4.6.2/plugins/specialchar/dialogs/lang/de.js
+-rw-rw-r--   0 lucjean   (1001) lucjean   (1001)     7728 2023-05-22 07:01:38.000000 coop_html_editor-1.4.1/coop_html_editor/static/ckeditor.4.6.2/plugins/specialchar/dialogs/lang/el.js
+-rw-rw-r--   0 lucjean   (1001) lucjean   (1001)     4546 2023-05-22 07:01:38.000000 coop_html_editor-1.4.1/coop_html_editor/static/ckeditor.4.6.2/plugins/specialchar/dialogs/lang/en-gb.js
+-rw-rw-r--   0 lucjean   (1001) lucjean   (1001)     4543 2023-05-22 07:01:38.000000 coop_html_editor-1.4.1/coop_html_editor/static/ckeditor.4.6.2/plugins/specialchar/dialogs/lang/en.js
+-rw-rw-r--   0 lucjean   (1001) lucjean   (1001)     4064 2023-05-22 07:01:38.000000 coop_html_editor-1.4.1/coop_html_editor/static/ckeditor.4.6.2/plugins/specialchar/dialogs/lang/eo.js
+-rw-rw-r--   0 lucjean   (1001) lucjean   (1001)     4943 2023-05-22 07:01:38.000000 coop_html_editor-1.4.1/coop_html_editor/static/ckeditor.4.6.2/plugins/specialchar/dialogs/lang/es.js
+-rw-rw-r--   0 lucjean   (1001) lucjean   (1001)     4488 2023-05-22 07:01:38.000000 coop_html_editor-1.4.1/coop_html_editor/static/ckeditor.4.6.2/plugins/specialchar/dialogs/lang/et.js
+-rw-rw-r--   0 lucjean   (1001) lucjean   (1001)     4545 2023-05-22 07:01:38.000000 coop_html_editor-1.4.1/coop_html_editor/static/ckeditor.4.6.2/plugins/specialchar/dialogs/lang/eu.js
+-rw-rw-r--   0 lucjean   (1001) lucjean   (1001)     5768 2023-05-22 07:01:38.000000 coop_html_editor-1.4.1/coop_html_editor/static/ckeditor.4.6.2/plugins/specialchar/dialogs/lang/fa.js
+-rw-rw-r--   0 lucjean   (1001) lucjean   (1001)     4581 2023-05-22 07:01:38.000000 coop_html_editor-1.4.1/coop_html_editor/static/ckeditor.4.6.2/plugins/specialchar/dialogs/lang/fi.js
+-rw-rw-r--   0 lucjean   (1001) lucjean   (1001)     3216 2023-05-22 07:01:38.000000 coop_html_editor-1.4.1/coop_html_editor/static/ckeditor.4.6.2/plugins/specialchar/dialogs/lang/fr-ca.js
+-rw-rw-r--   0 lucjean   (1001) lucjean   (1001)     3852 2023-05-22 07:01:38.000000 coop_html_editor-1.4.1/coop_html_editor/static/ckeditor.4.6.2/plugins/specialchar/dialogs/lang/fr.js
+-rw-rw-r--   0 lucjean   (1001) lucjean   (1001)     5000 2023-05-22 07:01:38.000000 coop_html_editor-1.4.1/coop_html_editor/static/ckeditor.4.6.2/plugins/specialchar/dialogs/lang/gl.js
+-rw-rw-r--   0 lucjean   (1001) lucjean   (1001)     4982 2023-05-22 07:01:38.000000 coop_html_editor-1.4.1/coop_html_editor/static/ckeditor.4.6.2/plugins/specialchar/dialogs/lang/he.js
+-rw-rw-r--   0 lucjean   (1001) lucjean   (1001)     4520 2023-05-22 07:01:38.000000 coop_html_editor-1.4.1/coop_html_editor/static/ckeditor.4.6.2/plugins/specialchar/dialogs/lang/hr.js
+-rw-rw-r--   0 lucjean   (1001) lucjean   (1001)     4131 2023-05-22 07:01:38.000000 coop_html_editor-1.4.1/coop_html_editor/static/ckeditor.4.6.2/plugins/specialchar/dialogs/lang/hu.js
+-rw-rw-r--   0 lucjean   (1001) lucjean   (1001)     4552 2023-05-22 07:01:38.000000 coop_html_editor-1.4.1/coop_html_editor/static/ckeditor.4.6.2/plugins/specialchar/dialogs/lang/id.js
+-rw-rw-r--   0 lucjean   (1001) lucjean   (1001)     5016 2023-05-22 07:01:38.000000 coop_html_editor-1.4.1/coop_html_editor/static/ckeditor.4.6.2/plugins/specialchar/dialogs/lang/it.js
+-rw-rw-r--   0 lucjean   (1001) lucjean   (1001)     3980 2023-05-22 07:01:38.000000 coop_html_editor-1.4.1/coop_html_editor/static/ckeditor.4.6.2/plugins/specialchar/dialogs/lang/ja.js
+-rw-rw-r--   0 lucjean   (1001) lucjean   (1001)     4747 2023-05-22 07:01:38.000000 coop_html_editor-1.4.1/coop_html_editor/static/ckeditor.4.6.2/plugins/specialchar/dialogs/lang/km.js
+-rw-rw-r--   0 lucjean   (1001) lucjean   (1001)     4920 2023-05-22 07:01:38.000000 coop_html_editor-1.4.1/coop_html_editor/static/ckeditor.4.6.2/plugins/specialchar/dialogs/lang/ko.js
+-rw-rw-r--   0 lucjean   (1001) lucjean   (1001)     7560 2023-05-22 07:01:38.000000 coop_html_editor-1.4.1/coop_html_editor/static/ckeditor.4.6.2/plugins/specialchar/dialogs/lang/ku.js
+-rw-rw-r--   0 lucjean   (1001) lucjean   (1001)     4588 2023-05-22 07:01:38.000000 coop_html_editor-1.4.1/coop_html_editor/static/ckeditor.4.6.2/plugins/specialchar/dialogs/lang/lt.js
+-rw-rw-r--   0 lucjean   (1001) lucjean   (1001)     5018 2023-05-22 07:01:38.000000 coop_html_editor-1.4.1/coop_html_editor/static/ckeditor.4.6.2/plugins/specialchar/dialogs/lang/lv.js
+-rw-rw-r--   0 lucjean   (1001) lucjean   (1001)     3428 2023-05-22 07:01:38.000000 coop_html_editor-1.4.1/coop_html_editor/static/ckeditor.4.6.2/plugins/specialchar/dialogs/lang/nb.js
+-rw-rw-r--   0 lucjean   (1001) lucjean   (1001)     4722 2023-05-22 07:01:38.000000 coop_html_editor-1.4.1/coop_html_editor/static/ckeditor.4.6.2/plugins/specialchar/dialogs/lang/nl.js
+-rw-rw-r--   0 lucjean   (1001) lucjean   (1001)     3428 2023-05-22 07:01:38.000000 coop_html_editor-1.4.1/coop_html_editor/static/ckeditor.4.6.2/plugins/specialchar/dialogs/lang/no.js
+-rw-rw-r--   0 lucjean   (1001) lucjean   (1001)     3826 2023-05-22 07:01:38.000000 coop_html_editor-1.4.1/coop_html_editor/static/ckeditor.4.6.2/plugins/specialchar/dialogs/lang/oc.js
+-rw-rw-r--   0 lucjean   (1001) lucjean   (1001)     4325 2023-05-22 07:01:38.000000 coop_html_editor-1.4.1/coop_html_editor/static/ckeditor.4.6.2/plugins/specialchar/dialogs/lang/pl.js
+-rw-rw-r--   0 lucjean   (1001) lucjean   (1001)     3826 2023-05-22 07:01:38.000000 coop_html_editor-1.4.1/coop_html_editor/static/ckeditor.4.6.2/plugins/specialchar/dialogs/lang/pt-br.js
+-rw-rw-r--   0 lucjean   (1001) lucjean   (1001)     4791 2023-05-22 07:01:38.000000 coop_html_editor-1.4.1/coop_html_editor/static/ckeditor.4.6.2/plugins/specialchar/dialogs/lang/pt.js
+-rw-rw-r--   0 lucjean   (1001) lucjean   (1001)     7543 2023-05-22 07:01:38.000000 coop_html_editor-1.4.1/coop_html_editor/static/ckeditor.4.6.2/plugins/specialchar/dialogs/lang/ru.js
+-rw-rw-r--   0 lucjean   (1001) lucjean   (1001)     4884 2023-05-22 07:01:38.000000 coop_html_editor-1.4.1/coop_html_editor/static/ckeditor.4.6.2/plugins/specialchar/dialogs/lang/si.js
+-rw-rw-r--   0 lucjean   (1001) lucjean   (1001)     4760 2023-05-22 07:01:38.000000 coop_html_editor-1.4.1/coop_html_editor/static/ckeditor.4.6.2/plugins/specialchar/dialogs/lang/sk.js
+-rw-rw-r--   0 lucjean   (1001) lucjean   (1001)     4345 2023-05-22 07:01:38.000000 coop_html_editor-1.4.1/coop_html_editor/static/ckeditor.4.6.2/plugins/specialchar/dialogs/lang/sl.js
+-rw-rw-r--   0 lucjean   (1001) lucjean   (1001)     4974 2023-05-22 07:01:38.000000 coop_html_editor-1.4.1/coop_html_editor/static/ckeditor.4.6.2/plugins/specialchar/dialogs/lang/sq.js
+-rw-rw-r--   0 lucjean   (1001) lucjean   (1001)     3480 2023-05-22 07:01:38.000000 coop_html_editor-1.4.1/coop_html_editor/static/ckeditor.4.6.2/plugins/specialchar/dialogs/lang/sv.js
+-rw-rw-r--   0 lucjean   (1001) lucjean   (1001)     4672 2023-05-22 07:01:38.000000 coop_html_editor-1.4.1/coop_html_editor/static/ckeditor.4.6.2/plugins/specialchar/dialogs/lang/th.js
+-rw-rw-r--   0 lucjean   (1001) lucjean   (1001)     4475 2023-05-22 07:01:38.000000 coop_html_editor-1.4.1/coop_html_editor/static/ckeditor.4.6.2/plugins/specialchar/dialogs/lang/tr.js
+-rw-rw-r--   0 lucjean   (1001) lucjean   (1001)     6725 2023-05-22 07:01:38.000000 coop_html_editor-1.4.1/coop_html_editor/static/ckeditor.4.6.2/plugins/specialchar/dialogs/lang/tt.js
+-rw-rw-r--   0 lucjean   (1001) lucjean   (1001)     4999 2023-05-22 07:01:38.000000 coop_html_editor-1.4.1/coop_html_editor/static/ckeditor.4.6.2/plugins/specialchar/dialogs/lang/ug.js
+-rw-rw-r--   0 lucjean   (1001) lucjean   (1001)     6366 2023-05-22 07:01:38.000000 coop_html_editor-1.4.1/coop_html_editor/static/ckeditor.4.6.2/plugins/specialchar/dialogs/lang/uk.js
+-rw-rw-r--   0 lucjean   (1001) lucjean   (1001)     6081 2023-05-22 07:01:38.000000 coop_html_editor-1.4.1/coop_html_editor/static/ckeditor.4.6.2/plugins/specialchar/dialogs/lang/vi.js
+-rw-rw-r--   0 lucjean   (1001) lucjean   (1001)     4377 2023-05-22 07:01:38.000000 coop_html_editor-1.4.1/coop_html_editor/static/ckeditor.4.6.2/plugins/specialchar/dialogs/lang/zh-cn.js
+-rw-rw-r--   0 lucjean   (1001) lucjean   (1001)     4157 2023-05-22 07:01:38.000000 coop_html_editor-1.4.1/coop_html_editor/static/ckeditor.4.6.2/plugins/specialchar/dialogs/lang/zh.js
+-rw-rw-r--   0 lucjean   (1001) lucjean   (1001)     5055 2023-05-22 07:01:38.000000 coop_html_editor-1.4.1/coop_html_editor/static/ckeditor.4.6.2/plugins/specialchar/dialogs/specialchar.js
+drwxrwxr-x   0 lucjean   (1001) lucjean   (1001)        0 2023-06-12 12:55:08.703912 coop_html_editor-1.4.1/coop_html_editor/static/ckeditor.4.6.2/plugins/table/
+drwxrwxr-x   0 lucjean   (1001) lucjean   (1001)        0 2023-06-12 12:55:08.783913 coop_html_editor-1.4.1/coop_html_editor/static/ckeditor.4.6.2/plugins/table/dialogs/
+-rw-rw-r--   0 lucjean   (1001) lucjean   (1001)     8807 2023-05-22 07:01:38.000000 coop_html_editor-1.4.1/coop_html_editor/static/ckeditor.4.6.2/plugins/table/dialogs/table.js
+drwxrwxr-x   0 lucjean   (1001) lucjean   (1001)        0 2023-06-12 12:55:08.703912 coop_html_editor-1.4.1/coop_html_editor/static/ckeditor.4.6.2/plugins/tabletools/
+drwxrwxr-x   0 lucjean   (1001) lucjean   (1001)        0 2023-06-12 12:55:08.783913 coop_html_editor-1.4.1/coop_html_editor/static/ckeditor.4.6.2/plugins/tabletools/dialogs/
+-rw-rw-r--   0 lucjean   (1001) lucjean   (1001)     6715 2023-05-22 07:01:38.000000 coop_html_editor-1.4.1/coop_html_editor/static/ckeditor.4.6.2/plugins/tabletools/dialogs/tableCell.js
+drwxrwxr-x   0 lucjean   (1001) lucjean   (1001)        0 2023-06-12 12:55:08.783913 coop_html_editor-1.4.1/coop_html_editor/static/ckeditor.4.6.2/plugins/toolbar/
+drwxrwxr-x   0 lucjean   (1001) lucjean   (1001)        0 2023-06-12 12:55:08.799913 coop_html_editor-1.4.1/coop_html_editor/static/ckeditor.4.6.2/plugins/toolbar/lang/
+-rw-rw-r--   0 lucjean   (1001) lucjean   (1001)      571 2023-05-22 07:01:38.000000 coop_html_editor-1.4.1/coop_html_editor/static/ckeditor.4.6.2/plugins/toolbar/lang/af.js
+-rw-rw-r--   0 lucjean   (1001) lucjean   (1001)      665 2023-05-22 07:01:38.000000 coop_html_editor-1.4.1/coop_html_editor/static/ckeditor.4.6.2/plugins/toolbar/lang/ar.js
+-rw-rw-r--   0 lucjean   (1001) lucjean   (1001)      606 2023-05-22 07:01:38.000000 coop_html_editor-1.4.1/coop_html_editor/static/ckeditor.4.6.2/plugins/toolbar/lang/az.js
+-rw-rw-r--   0 lucjean   (1001) lucjean   (1001)      789 2023-05-22 07:01:38.000000 coop_html_editor-1.4.1/coop_html_editor/static/ckeditor.4.6.2/plugins/toolbar/lang/bg.js
+-rw-rw-r--   0 lucjean   (1001) lucjean   (1001)      596 2023-05-22 07:01:38.000000 coop_html_editor-1.4.1/coop_html_editor/static/ckeditor.4.6.2/plugins/toolbar/lang/bn.js
+-rw-rw-r--   0 lucjean   (1001) lucjean   (1001)      596 2023-05-22 07:01:38.000000 coop_html_editor-1.4.1/coop_html_editor/static/ckeditor.4.6.2/plugins/toolbar/lang/bs.js
+-rw-rw-r--   0 lucjean   (1001) lucjean   (1001)      591 2023-05-22 07:01:38.000000 coop_html_editor-1.4.1/coop_html_editor/static/ckeditor.4.6.2/plugins/toolbar/lang/ca.js
+-rw-rw-r--   0 lucjean   (1001) lucjean   (1001)      605 2023-05-22 07:01:38.000000 coop_html_editor-1.4.1/coop_html_editor/static/ckeditor.4.6.2/plugins/toolbar/lang/cs.js
+-rw-rw-r--   0 lucjean   (1001) lucjean   (1001)      603 2023-05-22 07:01:38.000000 coop_html_editor-1.4.1/coop_html_editor/static/ckeditor.4.6.2/plugins/toolbar/lang/cy.js
+-rw-rw-r--   0 lucjean   (1001) lucjean   (1001)      615 2023-05-22 07:01:38.000000 coop_html_editor-1.4.1/coop_html_editor/static/ckeditor.4.6.2/plugins/toolbar/lang/da.js
+-rw-rw-r--   0 lucjean   (1001) lucjean   (1001)      613 2023-05-22 07:01:38.000000 coop_html_editor-1.4.1/coop_html_editor/static/ckeditor.4.6.2/plugins/toolbar/lang/de-ch.js
+-rw-rw-r--   0 lucjean   (1001) lucjean   (1001)      610 2023-05-22 07:01:38.000000 coop_html_editor-1.4.1/coop_html_editor/static/ckeditor.4.6.2/plugins/toolbar/lang/de.js
+-rw-rw-r--   0 lucjean   (1001) lucjean   (1001)      764 2023-05-22 07:01:38.000000 coop_html_editor-1.4.1/coop_html_editor/static/ckeditor.4.6.2/plugins/toolbar/lang/el.js
+-rw-rw-r--   0 lucjean   (1001) lucjean   (1001)      588 2023-05-22 07:01:38.000000 coop_html_editor-1.4.1/coop_html_editor/static/ckeditor.4.6.2/plugins/toolbar/lang/en-au.js
+-rw-rw-r--   0 lucjean   (1001) lucjean   (1001)      599 2023-05-22 07:01:38.000000 coop_html_editor-1.4.1/coop_html_editor/static/ckeditor.4.6.2/plugins/toolbar/lang/en-ca.js
+-rw-rw-r--   0 lucjean   (1001) lucjean   (1001)      566 2023-05-22 07:01:38.000000 coop_html_editor-1.4.1/coop_html_editor/static/ckeditor.4.6.2/plugins/toolbar/lang/en-gb.js
+-rw-rw-r--   0 lucjean   (1001) lucjean   (1001)      563 2023-05-22 07:01:38.000000 coop_html_editor-1.4.1/coop_html_editor/static/ckeditor.4.6.2/plugins/toolbar/lang/en.js
+-rw-rw-r--   0 lucjean   (1001) lucjean   (1001)      589 2023-05-22 07:01:38.000000 coop_html_editor-1.4.1/coop_html_editor/static/ckeditor.4.6.2/plugins/toolbar/lang/eo.js
+-rw-rw-r--   0 lucjean   (1001) lucjean   (1001)      642 2023-05-22 07:01:38.000000 coop_html_editor-1.4.1/coop_html_editor/static/ckeditor.4.6.2/plugins/toolbar/lang/es.js
+-rw-rw-r--   0 lucjean   (1001) lucjean   (1001)      614 2023-05-22 07:01:38.000000 coop_html_editor-1.4.1/coop_html_editor/static/ckeditor.4.6.2/plugins/toolbar/lang/et.js
+-rw-rw-r--   0 lucjean   (1001) lucjean   (1001)      610 2023-05-22 07:01:38.000000 coop_html_editor-1.4.1/coop_html_editor/static/ckeditor.4.6.2/plugins/toolbar/lang/eu.js
+-rw-rw-r--   0 lucjean   (1001) lucjean   (1001)      707 2023-05-22 07:01:38.000000 coop_html_editor-1.4.1/coop_html_editor/static/ckeditor.4.6.2/plugins/toolbar/lang/fa.js
+-rw-rw-r--   0 lucjean   (1001) lucjean   (1001)      600 2023-05-22 07:01:38.000000 coop_html_editor-1.4.1/coop_html_editor/static/ckeditor.4.6.2/plugins/toolbar/lang/fi.js
+-rw-rw-r--   0 lucjean   (1001) lucjean   (1001)      576 2023-05-22 07:01:38.000000 coop_html_editor-1.4.1/coop_html_editor/static/ckeditor.4.6.2/plugins/toolbar/lang/fo.js
+-rw-rw-r--   0 lucjean   (1001) lucjean   (1001)      628 2023-05-22 07:01:38.000000 coop_html_editor-1.4.1/coop_html_editor/static/ckeditor.4.6.2/plugins/toolbar/lang/fr-ca.js
+-rw-rw-r--   0 lucjean   (1001) lucjean   (1001)      627 2023-05-22 07:01:38.000000 coop_html_editor-1.4.1/coop_html_editor/static/ckeditor.4.6.2/plugins/toolbar/lang/fr.js
+-rw-rw-r--   0 lucjean   (1001) lucjean   (1001)      640 2023-05-22 07:01:38.000000 coop_html_editor-1.4.1/coop_html_editor/static/ckeditor.4.6.2/plugins/toolbar/lang/gl.js
+-rw-rw-r--   0 lucjean   (1001) lucjean   (1001)      798 2023-05-22 07:01:38.000000 coop_html_editor-1.4.1/coop_html_editor/static/ckeditor.4.6.2/plugins/toolbar/lang/gu.js
+-rw-rw-r--   0 lucjean   (1001) lucjean   (1001)      686 2023-05-22 07:01:38.000000 coop_html_editor-1.4.1/coop_html_editor/static/ckeditor.4.6.2/plugins/toolbar/lang/he.js
+-rw-rw-r--   0 lucjean   (1001) lucjean   (1001)      604 2023-05-22 07:01:38.000000 coop_html_editor-1.4.1/coop_html_editor/static/ckeditor.4.6.2/plugins/toolbar/lang/hi.js
+-rw-rw-r--   0 lucjean   (1001) lucjean   (1001)      602 2023-05-22 07:01:38.000000 coop_html_editor-1.4.1/coop_html_editor/static/ckeditor.4.6.2/plugins/toolbar/lang/hr.js
+-rw-rw-r--   0 lucjean   (1001) lucjean   (1001)      632 2023-05-22 07:01:38.000000 coop_html_editor-1.4.1/coop_html_editor/static/ckeditor.4.6.2/plugins/toolbar/lang/hu.js
+-rw-rw-r--   0 lucjean   (1001) lucjean   (1001)      583 2023-05-22 07:01:38.000000 coop_html_editor-1.4.1/coop_html_editor/static/ckeditor.4.6.2/plugins/toolbar/lang/id.js
+-rw-rw-r--   0 lucjean   (1001) lucjean   (1001)      596 2023-05-22 07:01:38.000000 coop_html_editor-1.4.1/coop_html_editor/static/ckeditor.4.6.2/plugins/toolbar/lang/is.js
+-rw-rw-r--   0 lucjean   (1001) lucjean   (1001)      584 2023-05-22 07:01:38.000000 coop_html_editor-1.4.1/coop_html_editor/static/ckeditor.4.6.2/plugins/toolbar/lang/it.js
+-rw-rw-r--   0 lucjean   (1001) lucjean   (1001)      590 2023-05-22 07:01:38.000000 coop_html_editor-1.4.1/coop_html_editor/static/ckeditor.4.6.2/plugins/toolbar/lang/ja.js
+-rw-rw-r--   0 lucjean   (1001) lucjean   (1001)      884 2023-05-22 07:01:38.000000 coop_html_editor-1.4.1/coop_html_editor/static/ckeditor.4.6.2/plugins/toolbar/lang/ka.js
+-rw-rw-r--   0 lucjean   (1001) lucjean   (1001)      859 2023-05-22 07:01:38.000000 coop_html_editor-1.4.1/coop_html_editor/static/ckeditor.4.6.2/plugins/toolbar/lang/km.js
+-rw-rw-r--   0 lucjean   (1001) lucjean   (1001)      576 2023-05-22 07:01:38.000000 coop_html_editor-1.4.1/coop_html_editor/static/ckeditor.4.6.2/plugins/toolbar/lang/ko.js
+-rw-rw-r--   0 lucjean   (1001) lucjean   (1001)      743 2023-05-22 07:01:38.000000 coop_html_editor-1.4.1/coop_html_editor/static/ckeditor.4.6.2/plugins/toolbar/lang/ku.js
+-rw-rw-r--   0 lucjean   (1001) lucjean   (1001)      623 2023-05-22 07:01:38.000000 coop_html_editor-1.4.1/coop_html_editor/static/ckeditor.4.6.2/plugins/toolbar/lang/lt.js
+-rw-rw-r--   0 lucjean   (1001) lucjean   (1001)      586 2023-05-22 07:01:38.000000 coop_html_editor-1.4.1/coop_html_editor/static/ckeditor.4.6.2/plugins/toolbar/lang/lv.js
+-rw-rw-r--   0 lucjean   (1001) lucjean   (1001)      596 2023-05-22 07:01:38.000000 coop_html_editor-1.4.1/coop_html_editor/static/ckeditor.4.6.2/plugins/toolbar/lang/mk.js
+-rw-rw-r--   0 lucjean   (1001) lucjean   (1001)      694 2023-05-22 07:01:38.000000 coop_html_editor-1.4.1/coop_html_editor/static/ckeditor.4.6.2/plugins/toolbar/lang/mn.js
+-rw-rw-r--   0 lucjean   (1001) lucjean   (1001)      596 2023-05-22 07:01:38.000000 coop_html_editor-1.4.1/coop_html_editor/static/ckeditor.4.6.2/plugins/toolbar/lang/ms.js
+-rw-rw-r--   0 lucjean   (1001) lucjean   (1001)      593 2023-05-22 07:01:38.000000 coop_html_editor-1.4.1/coop_html_editor/static/ckeditor.4.6.2/plugins/toolbar/lang/nb.js
+-rw-rw-r--   0 lucjean   (1001) lucjean   (1001)      592 2023-05-22 07:01:38.000000 coop_html_editor-1.4.1/coop_html_editor/static/ckeditor.4.6.2/plugins/toolbar/lang/nl.js
+-rw-rw-r--   0 lucjean   (1001) lucjean   (1001)      593 2023-05-22 07:01:38.000000 coop_html_editor-1.4.1/coop_html_editor/static/ckeditor.4.6.2/plugins/toolbar/lang/no.js
+-rw-rw-r--   0 lucjean   (1001) lucjean   (1001)      623 2023-05-22 07:01:38.000000 coop_html_editor-1.4.1/coop_html_editor/static/ckeditor.4.6.2/plugins/toolbar/lang/oc.js
+-rw-rw-r--   0 lucjean   (1001) lucjean   (1001)      605 2023-05-22 07:01:38.000000 coop_html_editor-1.4.1/coop_html_editor/static/ckeditor.4.6.2/plugins/toolbar/lang/pl.js
+-rw-rw-r--   0 lucjean   (1001) lucjean   (1001)      633 2023-05-22 07:01:38.000000 coop_html_editor-1.4.1/coop_html_editor/static/ckeditor.4.6.2/plugins/toolbar/lang/pt-br.js
+-rw-rw-r--   0 lucjean   (1001) lucjean   (1001)      653 2023-05-22 07:01:38.000000 coop_html_editor-1.4.1/coop_html_editor/static/ckeditor.4.6.2/plugins/toolbar/lang/pt.js
+-rw-rw-r--   0 lucjean   (1001) lucjean   (1001)      573 2023-05-22 07:01:38.000000 coop_html_editor-1.4.1/coop_html_editor/static/ckeditor.4.6.2/plugins/toolbar/lang/ro.js
+-rw-rw-r--   0 lucjean   (1001) lucjean   (1001)      813 2023-05-22 07:01:38.000000 coop_html_editor-1.4.1/coop_html_editor/static/ckeditor.4.6.2/plugins/toolbar/lang/ru.js
+-rw-rw-r--   0 lucjean   (1001) lucjean   (1001)      860 2023-05-22 07:01:38.000000 coop_html_editor-1.4.1/coop_html_editor/static/ckeditor.4.6.2/plugins/toolbar/lang/si.js
+-rw-rw-r--   0 lucjean   (1001) lucjean   (1001)      632 2023-05-22 07:01:38.000000 coop_html_editor-1.4.1/coop_html_editor/static/ckeditor.4.6.2/plugins/toolbar/lang/sk.js
+-rw-rw-r--   0 lucjean   (1001) lucjean   (1001)      603 2023-05-22 07:01:38.000000 coop_html_editor-1.4.1/coop_html_editor/static/ckeditor.4.6.2/plugins/toolbar/lang/sl.js
+-rw-rw-r--   0 lucjean   (1001) lucjean   (1001)      585 2023-05-22 07:01:38.000000 coop_html_editor-1.4.1/coop_html_editor/static/ckeditor.4.6.2/plugins/toolbar/lang/sq.js
+-rw-rw-r--   0 lucjean   (1001) lucjean   (1001)      573 2023-05-22 07:01:38.000000 coop_html_editor-1.4.1/coop_html_editor/static/ckeditor.4.6.2/plugins/toolbar/lang/sr-latn.js
+-rw-rw-r--   0 lucjean   (1001) lucjean   (1001)      628 2023-05-22 07:01:38.000000 coop_html_editor-1.4.1/coop_html_editor/static/ckeditor.4.6.2/plugins/toolbar/lang/sr.js
+-rw-rw-r--   0 lucjean   (1001) lucjean   (1001)      585 2023-05-22 07:01:38.000000 coop_html_editor-1.4.1/coop_html_editor/static/ckeditor.4.6.2/plugins/toolbar/lang/sv.js
+-rw-rw-r--   0 lucjean   (1001) lucjean   (1001)      707 2023-05-22 07:01:38.000000 coop_html_editor-1.4.1/coop_html_editor/static/ckeditor.4.6.2/plugins/toolbar/lang/th.js
+-rw-rw-r--   0 lucjean   (1001) lucjean   (1001)      606 2023-05-22 07:01:38.000000 coop_html_editor-1.4.1/coop_html_editor/static/ckeditor.4.6.2/plugins/toolbar/lang/tr.js
+-rw-rw-r--   0 lucjean   (1001) lucjean   (1001)      714 2023-05-22 07:01:38.000000 coop_html_editor-1.4.1/coop_html_editor/static/ckeditor.4.6.2/plugins/toolbar/lang/tt.js
+-rw-rw-r--   0 lucjean   (1001) lucjean   (1001)      699 2023-05-22 07:01:38.000000 coop_html_editor-1.4.1/coop_html_editor/static/ckeditor.4.6.2/plugins/toolbar/lang/ug.js
+-rw-rw-r--   0 lucjean   (1001) lucjean   (1001)      818 2023-05-22 07:01:38.000000 coop_html_editor-1.4.1/coop_html_editor/static/ckeditor.4.6.2/plugins/toolbar/lang/uk.js
+-rw-rw-r--   0 lucjean   (1001) lucjean   (1001)      621 2023-05-22 07:01:38.000000 coop_html_editor-1.4.1/coop_html_editor/static/ckeditor.4.6.2/plugins/toolbar/lang/vi.js
+-rw-rw-r--   0 lucjean   (1001) lucjean   (1001)      559 2023-05-22 07:01:38.000000 coop_html_editor-1.4.1/coop_html_editor/static/ckeditor.4.6.2/plugins/toolbar/lang/zh-cn.js
+-rw-rw-r--   0 lucjean   (1001) lucjean   (1001)      571 2023-05-22 07:01:38.000000 coop_html_editor-1.4.1/coop_html_editor/static/ckeditor.4.6.2/plugins/toolbar/lang/zh.js
+-rw-rw-r--   0 lucjean   (1001) lucjean   (1001)    25525 2023-05-22 07:01:38.000000 coop_html_editor-1.4.1/coop_html_editor/static/ckeditor.4.6.2/plugins/toolbar/plugin.js
+drwxrwxr-x   0 lucjean   (1001) lucjean   (1001)        0 2023-06-12 12:55:08.799913 coop_html_editor-1.4.1/coop_html_editor/static/ckeditor.4.6.2/plugins/toolbar/samples/
+-rw-rw-r--   0 lucjean   (1001) lucjean   (1001)     8665 2023-05-22 07:01:38.000000 coop_html_editor-1.4.1/coop_html_editor/static/ckeditor.4.6.2/plugins/toolbar/samples/toolbar.html
+drwxrwxr-x   0 lucjean   (1001) lucjean   (1001)        0 2023-06-12 12:55:08.799913 coop_html_editor-1.4.1/coop_html_editor/static/ckeditor.4.6.2/plugins/videoembed/
+drwxrwxr-x   0 lucjean   (1001) lucjean   (1001)        0 2023-06-12 12:55:08.799913 coop_html_editor-1.4.1/coop_html_editor/static/ckeditor.4.6.2/plugins/videoembed/dialogs/
+-rwxrwxr-x   0 lucjean   (1001) lucjean   (1001)     4089 2023-05-22 07:01:38.000000 coop_html_editor-1.4.1/coop_html_editor/static/ckeditor.4.6.2/plugins/videoembed/dialogs/videoembedDialog.js
+drwxrwxr-x   0 lucjean   (1001) lucjean   (1001)        0 2023-06-12 12:55:08.799913 coop_html_editor-1.4.1/coop_html_editor/static/ckeditor.4.6.2/plugins/videoembed/lang/
+-rwxrwxr-x   0 lucjean   (1001) lucjean   (1001)      256 2023-05-22 07:01:38.000000 coop_html_editor-1.4.1/coop_html_editor/static/ckeditor.4.6.2/plugins/videoembed/lang/en.js
+-rwxrwxr-x   0 lucjean   (1001) lucjean   (1001)      289 2023-05-22 07:01:38.000000 coop_html_editor-1.4.1/coop_html_editor/static/ckeditor.4.6.2/plugins/videoembed/lang/fr.js
+-rwxrwxr-x   0 lucjean   (1001) lucjean   (1001)      761 2023-05-22 07:01:38.000000 coop_html_editor-1.4.1/coop_html_editor/static/ckeditor.4.6.2/plugins/videoembed/plugin.js
+drwxrwxr-x   0 lucjean   (1001) lucjean   (1001)        0 2023-06-12 12:55:08.799913 coop_html_editor-1.4.1/coop_html_editor/static/ckeditor.4.6.2/plugins/widget/
+drwxrwxr-x   0 lucjean   (1001) lucjean   (1001)        0 2023-06-12 12:55:08.799913 coop_html_editor-1.4.1/coop_html_editor/static/ckeditor.4.6.2/plugins/widget/dev/
+drwxrwxr-x   0 lucjean   (1001) lucjean   (1001)        0 2023-06-12 12:55:08.799913 coop_html_editor-1.4.1/coop_html_editor/static/ckeditor.4.6.2/plugins/widget/dev/assets/
+-rw-rw-r--   0 lucjean   (1001) lucjean   (1001)      315 2023-05-22 07:01:38.000000 coop_html_editor-1.4.1/coop_html_editor/static/ckeditor.4.6.2/plugins/widget/dev/assets/contents.css
+-rw-rw-r--   0 lucjean   (1001) lucjean   (1001)    17932 2023-05-22 07:01:38.000000 coop_html_editor-1.4.1/coop_html_editor/static/ckeditor.4.6.2/plugins/widget/dev/assets/sample.jpg
+drwxrwxr-x   0 lucjean   (1001) lucjean   (1001)        0 2023-06-12 12:55:08.799913 coop_html_editor-1.4.1/coop_html_editor/static/ckeditor.4.6.2/plugins/widget/dev/assets/simplebox/
+-rw-rw-r--   0 lucjean   (1001) lucjean   (1001)      635 2023-05-22 07:01:38.000000 coop_html_editor-1.4.1/coop_html_editor/static/ckeditor.4.6.2/plugins/widget/dev/assets/simplebox/contents.css
+drwxrwxr-x   0 lucjean   (1001) lucjean   (1001)        0 2023-06-12 12:55:08.799913 coop_html_editor-1.4.1/coop_html_editor/static/ckeditor.4.6.2/plugins/widget/dev/assets/simplebox/dialogs/
+-rw-rw-r--   0 lucjean   (1001) lucjean   (1001)     1596 2023-05-22 07:01:38.000000 coop_html_editor-1.4.1/coop_html_editor/static/ckeditor.4.6.2/plugins/widget/dev/assets/simplebox/dialogs/simplebox.js
+-rw-rw-r--   0 lucjean   (1001) lucjean   (1001)     4748 2023-05-22 07:01:38.000000 coop_html_editor-1.4.1/coop_html_editor/static/ckeditor.4.6.2/plugins/widget/dev/assets/simplebox/plugin.js
+-rw-rw-r--   0 lucjean   (1001) lucjean   (1001)     3699 2023-05-22 07:01:38.000000 coop_html_editor-1.4.1/coop_html_editor/static/ckeditor.4.6.2/plugins/widget/dev/console.js
+-rw-rw-r--   0 lucjean   (1001) lucjean   (1001)    11091 2023-05-22 07:01:38.000000 coop_html_editor-1.4.1/coop_html_editor/static/ckeditor.4.6.2/plugins/widget/dev/nestedwidgets.html
+-rw-rw-r--   0 lucjean   (1001) lucjean   (1001)     9707 2023-05-22 07:01:38.000000 coop_html_editor-1.4.1/coop_html_editor/static/ckeditor.4.6.2/plugins/widget/dev/widgetstyles.html
+drwxrwxr-x   0 lucjean   (1001) lucjean   (1001)        0 2023-06-12 12:55:08.799913 coop_html_editor-1.4.1/coop_html_editor/static/ckeditor.4.6.2/plugins/widget/images/
+-rw-rw-r--   0 lucjean   (1001) lucjean   (1001)      220 2023-05-22 07:01:38.000000 coop_html_editor-1.4.1/coop_html_editor/static/ckeditor.4.6.2/plugins/widget/images/handle.png
+drwxrwxr-x   0 lucjean   (1001) lucjean   (1001)        0 2023-06-12 12:55:08.807913 coop_html_editor-1.4.1/coop_html_editor/static/ckeditor.4.6.2/plugins/widget/lang/
+-rw-rw-r--   0 lucjean   (1001) lucjean   (1001)      280 2023-05-22 07:01:38.000000 coop_html_editor-1.4.1/coop_html_editor/static/ckeditor.4.6.2/plugins/widget/lang/af.js
+-rw-rw-r--   0 lucjean   (1001) lucjean   (1001)      290 2023-05-22 07:01:38.000000 coop_html_editor-1.4.1/coop_html_editor/static/ckeditor.4.6.2/plugins/widget/lang/ar.js
+-rw-rw-r--   0 lucjean   (1001) lucjean   (1001)      266 2023-05-22 07:01:38.000000 coop_html_editor-1.4.1/coop_html_editor/static/ckeditor.4.6.2/plugins/widget/lang/az.js
+-rw-rw-r--   0 lucjean   (1001) lucjean   (1001)      311 2023-05-22 07:01:38.000000 coop_html_editor-1.4.1/coop_html_editor/static/ckeditor.4.6.2/plugins/widget/lang/bg.js
+-rw-rw-r--   0 lucjean   (1001) lucjean   (1001)      273 2023-05-22 07:01:38.000000 coop_html_editor-1.4.1/coop_html_editor/static/ckeditor.4.6.2/plugins/widget/lang/ca.js
+-rw-rw-r--   0 lucjean   (1001) lucjean   (1001)      291 2023-05-22 07:01:38.000000 coop_html_editor-1.4.1/coop_html_editor/static/ckeditor.4.6.2/plugins/widget/lang/cs.js
+-rw-rw-r--   0 lucjean   (1001) lucjean   (1001)      277 2023-05-22 07:01:38.000000 coop_html_editor-1.4.1/coop_html_editor/static/ckeditor.4.6.2/plugins/widget/lang/cy.js
+-rw-rw-r--   0 lucjean   (1001) lucjean   (1001)      282 2023-05-22 07:01:38.000000 coop_html_editor-1.4.1/coop_html_editor/static/ckeditor.4.6.2/plugins/widget/lang/da.js
+-rw-rw-r--   0 lucjean   (1001) lucjean   (1001)      294 2023-05-22 07:01:38.000000 coop_html_editor-1.4.1/coop_html_editor/static/ckeditor.4.6.2/plugins/widget/lang/de-ch.js
+-rw-rw-r--   0 lucjean   (1001) lucjean   (1001)      287 2023-05-22 07:01:38.000000 coop_html_editor-1.4.1/coop_html_editor/static/ckeditor.4.6.2/plugins/widget/lang/de.js
+-rw-rw-r--   0 lucjean   (1001) lucjean   (1001)      351 2023-05-22 07:01:38.000000 coop_html_editor-1.4.1/coop_html_editor/static/ckeditor.4.6.2/plugins/widget/lang/el.js
+-rw-rw-r--   0 lucjean   (1001) lucjean   (1001)      280 2023-05-22 07:01:38.000000 coop_html_editor-1.4.1/coop_html_editor/static/ckeditor.4.6.2/plugins/widget/lang/en-gb.js
+-rw-rw-r--   0 lucjean   (1001) lucjean   (1001)      266 2023-05-22 07:01:38.000000 coop_html_editor-1.4.1/coop_html_editor/static/ckeditor.4.6.2/plugins/widget/lang/en.js
+-rw-rw-r--   0 lucjean   (1001) lucjean   (1001)      279 2023-05-22 07:01:38.000000 coop_html_editor-1.4.1/coop_html_editor/static/ckeditor.4.6.2/plugins/widget/lang/eo.js
+-rw-rw-r--   0 lucjean   (1001) lucjean   (1001)      280 2023-05-22 07:01:38.000000 coop_html_editor-1.4.1/coop_html_editor/static/ckeditor.4.6.2/plugins/widget/lang/es.js
+-rw-rw-r--   0 lucjean   (1001) lucjean   (1001)      281 2023-05-22 07:01:38.000000 coop_html_editor-1.4.1/coop_html_editor/static/ckeditor.4.6.2/plugins/widget/lang/eu.js
+-rw-rw-r--   0 lucjean   (1001) lucjean   (1001)      301 2023-05-22 07:01:38.000000 coop_html_editor-1.4.1/coop_html_editor/static/ckeditor.4.6.2/plugins/widget/lang/fa.js
+-rw-rw-r--   0 lucjean   (1001) lucjean   (1001)      290 2023-05-22 07:01:38.000000 coop_html_editor-1.4.1/coop_html_editor/static/ckeditor.4.6.2/plugins/widget/lang/fi.js
+-rw-rw-r--   0 lucjean   (1001) lucjean   (1001)      280 2023-05-22 07:01:38.000000 coop_html_editor-1.4.1/coop_html_editor/static/ckeditor.4.6.2/plugins/widget/lang/fr.js
+-rw-rw-r--   0 lucjean   (1001) lucjean   (1001)      282 2023-05-22 07:01:38.000000 coop_html_editor-1.4.1/coop_html_editor/static/ckeditor.4.6.2/plugins/widget/lang/gl.js
+-rw-rw-r--   0 lucjean   (1001) lucjean   (1001)      283 2023-05-22 07:01:38.000000 coop_html_editor-1.4.1/coop_html_editor/static/ckeditor.4.6.2/plugins/widget/lang/he.js
+-rw-rw-r--   0 lucjean   (1001) lucjean   (1001)      283 2023-05-22 07:01:38.000000 coop_html_editor-1.4.1/coop_html_editor/static/ckeditor.4.6.2/plugins/widget/lang/hr.js
+-rw-rw-r--   0 lucjean   (1001) lucjean   (1001)      288 2023-05-22 07:01:38.000000 coop_html_editor-1.4.1/coop_html_editor/static/ckeditor.4.6.2/plugins/widget/lang/hu.js
+-rw-rw-r--   0 lucjean   (1001) lucjean   (1001)      288 2023-05-22 07:01:38.000000 coop_html_editor-1.4.1/coop_html_editor/static/ckeditor.4.6.2/plugins/widget/lang/id.js
+-rw-rw-r--   0 lucjean   (1001) lucjean   (1001)      279 2023-05-22 07:01:38.000000 coop_html_editor-1.4.1/coop_html_editor/static/ckeditor.4.6.2/plugins/widget/lang/it.js
+-rw-rw-r--   0 lucjean   (1001) lucjean   (1001)      280 2023-05-22 07:01:38.000000 coop_html_editor-1.4.1/coop_html_editor/static/ckeditor.4.6.2/plugins/widget/lang/ja.js
+-rw-rw-r--   0 lucjean   (1001) lucjean   (1001)      339 2023-05-22 07:01:38.000000 coop_html_editor-1.4.1/coop_html_editor/static/ckeditor.4.6.2/plugins/widget/lang/km.js
+-rw-rw-r--   0 lucjean   (1001) lucjean   (1001)      301 2023-05-22 07:01:38.000000 coop_html_editor-1.4.1/coop_html_editor/static/ckeditor.4.6.2/plugins/widget/lang/ko.js
+-rw-rw-r--   0 lucjean   (1001) lucjean   (1001)      302 2023-05-22 07:01:38.000000 coop_html_editor-1.4.1/coop_html_editor/static/ckeditor.4.6.2/plugins/widget/lang/ku.js
+-rw-rw-r--   0 lucjean   (1001) lucjean   (1001)      291 2023-05-22 07:01:38.000000 coop_html_editor-1.4.1/coop_html_editor/static/ckeditor.4.6.2/plugins/widget/lang/lv.js
+-rw-rw-r--   0 lucjean   (1001) lucjean   (1001)      270 2023-05-22 07:01:38.000000 coop_html_editor-1.4.1/coop_html_editor/static/ckeditor.4.6.2/plugins/widget/lang/nb.js
+-rw-rw-r--   0 lucjean   (1001) lucjean   (1001)      275 2023-05-22 07:01:38.000000 coop_html_editor-1.4.1/coop_html_editor/static/ckeditor.4.6.2/plugins/widget/lang/nl.js
+-rw-rw-r--   0 lucjean   (1001) lucjean   (1001)      270 2023-05-22 07:01:38.000000 coop_html_editor-1.4.1/coop_html_editor/static/ckeditor.4.6.2/plugins/widget/lang/no.js
+-rw-rw-r--   0 lucjean   (1001) lucjean   (1001)      274 2023-05-22 07:01:38.000000 coop_html_editor-1.4.1/coop_html_editor/static/ckeditor.4.6.2/plugins/widget/lang/oc.js
+-rw-rw-r--   0 lucjean   (1001) lucjean   (1001)      283 2023-05-22 07:01:38.000000 coop_html_editor-1.4.1/coop_html_editor/static/ckeditor.4.6.2/plugins/widget/lang/pl.js
+-rw-rw-r--   0 lucjean   (1001) lucjean   (1001)      273 2023-05-22 07:01:38.000000 coop_html_editor-1.4.1/coop_html_editor/static/ckeditor.4.6.2/plugins/widget/lang/pt-br.js
+-rw-rw-r--   0 lucjean   (1001) lucjean   (1001)      282 2023-05-22 07:01:38.000000 coop_html_editor-1.4.1/coop_html_editor/static/ckeditor.4.6.2/plugins/widget/lang/pt.js
+-rw-rw-r--   0 lucjean   (1001) lucjean   (1001)      323 2023-05-22 07:01:38.000000 coop_html_editor-1.4.1/coop_html_editor/static/ckeditor.4.6.2/plugins/widget/lang/ru.js
+-rw-rw-r--   0 lucjean   (1001) lucjean   (1001)      291 2023-05-22 07:01:38.000000 coop_html_editor-1.4.1/coop_html_editor/static/ckeditor.4.6.2/plugins/widget/lang/sk.js
+-rw-rw-r--   0 lucjean   (1001) lucjean   (1001)      291 2023-05-22 07:01:38.000000 coop_html_editor-1.4.1/coop_html_editor/static/ckeditor.4.6.2/plugins/widget/lang/sl.js
+-rw-rw-r--   0 lucjean   (1001) lucjean   (1001)      290 2023-05-22 07:01:38.000000 coop_html_editor-1.4.1/coop_html_editor/static/ckeditor.4.6.2/plugins/widget/lang/sq.js
+-rw-rw-r--   0 lucjean   (1001) lucjean   (1001)      275 2023-05-22 07:01:38.000000 coop_html_editor-1.4.1/coop_html_editor/static/ckeditor.4.6.2/plugins/widget/lang/sv.js
+-rw-rw-r--   0 lucjean   (1001) lucjean   (1001)      297 2023-05-22 07:01:38.000000 coop_html_editor-1.4.1/coop_html_editor/static/ckeditor.4.6.2/plugins/widget/lang/tr.js
+-rw-rw-r--   0 lucjean   (1001) lucjean   (1001)      317 2023-05-22 07:01:38.000000 coop_html_editor-1.4.1/coop_html_editor/static/ckeditor.4.6.2/plugins/widget/lang/tt.js
+-rw-rw-r--   0 lucjean   (1001) lucjean   (1001)      293 2023-05-22 07:01:38.000000 coop_html_editor-1.4.1/coop_html_editor/static/ckeditor.4.6.2/plugins/widget/lang/ug.js
+-rw-rw-r--   0 lucjean   (1001) lucjean   (1001)      318 2023-05-22 07:01:38.000000 coop_html_editor-1.4.1/coop_html_editor/static/ckeditor.4.6.2/plugins/widget/lang/uk.js
+-rw-rw-r--   0 lucjean   (1001) lucjean   (1001)      296 2023-05-22 07:01:38.000000 coop_html_editor-1.4.1/coop_html_editor/static/ckeditor.4.6.2/plugins/widget/lang/vi.js
+-rw-rw-r--   0 lucjean   (1001) lucjean   (1001)      274 2023-05-22 07:01:38.000000 coop_html_editor-1.4.1/coop_html_editor/static/ckeditor.4.6.2/plugins/widget/lang/zh-cn.js
+-rw-rw-r--   0 lucjean   (1001) lucjean   (1001)      262 2023-05-22 07:01:38.000000 coop_html_editor-1.4.1/coop_html_editor/static/ckeditor.4.6.2/plugins/widget/lang/zh.js
+-rw-rw-r--   0 lucjean   (1001) lucjean   (1001)   136176 2023-05-22 07:01:38.000000 coop_html_editor-1.4.1/coop_html_editor/static/ckeditor.4.6.2/plugins/widget/plugin.js
+drwxrwxr-x   0 lucjean   (1001) lucjean   (1001)        0 2023-06-12 12:55:08.807913 coop_html_editor-1.4.1/coop_html_editor/static/ckeditor.4.6.2/plugins/widgetselection/
+-rw-rw-r--   0 lucjean   (1001) lucjean   (1001)    11474 2023-05-22 07:01:38.000000 coop_html_editor-1.4.1/coop_html_editor/static/ckeditor.4.6.2/plugins/widgetselection/plugin.js
+drwxrwxr-x   0 lucjean   (1001) lucjean   (1001)        0 2023-06-12 12:55:08.811913 coop_html_editor-1.4.1/coop_html_editor/static/ckeditor.4.6.2/plugins/wsc/
+-rw-rw-r--   0 lucjean   (1001) lucjean   (1001)     1474 2023-05-22 07:01:38.000000 coop_html_editor-1.4.1/coop_html_editor/static/ckeditor.4.6.2/plugins/wsc/LICENSE.md
+-rw-rw-r--   0 lucjean   (1001) lucjean   (1001)      970 2023-05-22 07:01:38.000000 coop_html_editor-1.4.1/coop_html_editor/static/ckeditor.4.6.2/plugins/wsc/README.md
+drwxrwxr-x   0 lucjean   (1001) lucjean   (1001)        0 2023-06-12 12:55:08.811913 coop_html_editor-1.4.1/coop_html_editor/static/ckeditor.4.6.2/plugins/wsc/dialogs/
+-rw-rw-r--   0 lucjean   (1001) lucjean   (1001)     1690 2023-05-22 07:01:38.000000 coop_html_editor-1.4.1/coop_html_editor/static/ckeditor.4.6.2/plugins/wsc/dialogs/ciframe.html
+-rw-rw-r--   0 lucjean   (1001) lucjean   (1001)     1935 2023-05-22 07:01:38.000000 coop_html_editor-1.4.1/coop_html_editor/static/ckeditor.4.6.2/plugins/wsc/dialogs/tmpFrameset.html
+-rw-rw-r--   0 lucjean   (1001) lucjean   (1001)     1232 2023-05-22 07:01:38.000000 coop_html_editor-1.4.1/coop_html_editor/static/ckeditor.4.6.2/plugins/wsc/dialogs/wsc.css
+-rw-rw-r--   0 lucjean   (1001) lucjean   (1001)    48295 2023-05-22 07:01:38.000000 coop_html_editor-1.4.1/coop_html_editor/static/ckeditor.4.6.2/plugins/wsc/dialogs/wsc.js
+-rw-rw-r--   0 lucjean   (1001) lucjean   (1001)     3438 2023-05-22 07:01:38.000000 coop_html_editor-1.4.1/coop_html_editor/static/ckeditor.4.6.2/plugins/wsc/dialogs/wsc_ie.js
+drwxrwxr-x   0 lucjean   (1001) lucjean   (1001)        0 2023-06-12 12:55:08.707913 coop_html_editor-1.4.1/coop_html_editor/static/ckeditor.4.6.2/plugins/wsc/skins/
+drwxrwxr-x   0 lucjean   (1001) lucjean   (1001)        0 2023-06-12 12:55:08.811913 coop_html_editor-1.4.1/coop_html_editor/static/ckeditor.4.6.2/plugins/wsc/skins/moono-lisa/
+-rw-rw-r--   0 lucjean   (1001) lucjean   (1001)     1306 2023-05-22 07:01:38.000000 coop_html_editor-1.4.1/coop_html_editor/static/ckeditor.4.6.2/plugins/wsc/skins/moono-lisa/wsc.css
+drwxrwxr-x   0 lucjean   (1001) lucjean   (1001)        0 2023-06-12 12:55:08.811913 coop_html_editor-1.4.1/coop_html_editor/static/ckeditor.4.6.2/samples/
+drwxrwxr-x   0 lucjean   (1001) lucjean   (1001)        0 2023-06-12 12:55:08.811913 coop_html_editor-1.4.1/coop_html_editor/static/ckeditor.4.6.2/samples/css/
+-rw-rw-r--   0 lucjean   (1001) lucjean   (1001)    67258 2023-05-22 07:01:38.000000 coop_html_editor-1.4.1/coop_html_editor/static/ckeditor.4.6.2/samples/css/samples.css
+drwxrwxr-x   0 lucjean   (1001) lucjean   (1001)        0 2023-06-12 12:55:08.811913 coop_html_editor-1.4.1/coop_html_editor/static/ckeditor.4.6.2/samples/img/
+-rw-rw-r--   0 lucjean   (1001) lucjean   (1001)      383 2023-05-22 07:01:38.000000 coop_html_editor-1.4.1/coop_html_editor/static/ckeditor.4.6.2/samples/img/github-top.png
+-rw-rw-r--   0 lucjean   (1001) lucjean   (1001)    13086 2023-05-22 07:01:38.000000 coop_html_editor-1.4.1/coop_html_editor/static/ckeditor.4.6.2/samples/img/header-bg.png
+-rw-rw-r--   0 lucjean   (1001) lucjean   (1001)      123 2023-05-22 07:01:38.000000 coop_html_editor-1.4.1/coop_html_editor/static/ckeditor.4.6.2/samples/img/header-separator.png
+-rw-rw-r--   0 lucjean   (1001) lucjean   (1001)     5891 2023-05-22 07:01:38.000000 coop_html_editor-1.4.1/coop_html_editor/static/ckeditor.4.6.2/samples/img/logo.png
+-rw-rw-r--   0 lucjean   (1001) lucjean   (1001)    12029 2023-05-22 07:01:38.000000 coop_html_editor-1.4.1/coop_html_editor/static/ckeditor.4.6.2/samples/img/navigation-tip.png
+-rw-rw-r--   0 lucjean   (1001) lucjean   (1001)     6692 2023-05-22 07:01:38.000000 coop_html_editor-1.4.1/coop_html_editor/static/ckeditor.4.6.2/samples/index.html
+drwxrwxr-x   0 lucjean   (1001) lucjean   (1001)        0 2023-06-12 12:55:08.811913 coop_html_editor-1.4.1/coop_html_editor/static/ckeditor.4.6.2/samples/js/
+-rw-rw-r--   0 lucjean   (1001) lucjean   (1001)     1574 2023-05-22 07:01:38.000000 coop_html_editor-1.4.1/coop_html_editor/static/ckeditor.4.6.2/samples/js/sample.js
+-rw-rw-r--   0 lucjean   (1001) lucjean   (1001)     6408 2023-05-22 07:01:38.000000 coop_html_editor-1.4.1/coop_html_editor/static/ckeditor.4.6.2/samples/js/sf.js
+drwxrwxr-x   0 lucjean   (1001) lucjean   (1001)        0 2023-06-12 12:55:08.815913 coop_html_editor-1.4.1/coop_html_editor/static/ckeditor.4.6.2/samples/old/
+-rw-rw-r--   0 lucjean   (1001) lucjean   (1001)     2706 2023-05-22 07:01:38.000000 coop_html_editor-1.4.1/coop_html_editor/static/ckeditor.4.6.2/samples/old/ajax.html
+-rw-rw-r--   0 lucjean   (1001) lucjean   (1001)     7179 2023-05-22 07:01:38.000000 coop_html_editor-1.4.1/coop_html_editor/static/ckeditor.4.6.2/samples/old/api.html
+-rw-rw-r--   0 lucjean   (1001) lucjean   (1001)     2259 2023-05-22 07:01:38.000000 coop_html_editor-1.4.1/coop_html_editor/static/ckeditor.4.6.2/samples/old/appendto.html
+drwxrwxr-x   0 lucjean   (1001) lucjean   (1001)        0 2023-06-12 12:55:08.815913 coop_html_editor-1.4.1/coop_html_editor/static/ckeditor.4.6.2/samples/old/assets/
+drwxrwxr-x   0 lucjean   (1001) lucjean   (1001)        0 2023-06-12 12:55:08.815913 coop_html_editor-1.4.1/coop_html_editor/static/ckeditor.4.6.2/samples/old/assets/inlineall/
+-rw-rw-r--   0 lucjean   (1001) lucjean   (1001)     4283 2023-05-22 07:01:38.000000 coop_html_editor-1.4.1/coop_html_editor/static/ckeditor.4.6.2/samples/old/assets/inlineall/logo.png
+drwxrwxr-x   0 lucjean   (1001) lucjean   (1001)        0 2023-06-12 12:55:08.819913 coop_html_editor-1.4.1/coop_html_editor/static/ckeditor.4.6.2/samples/old/assets/outputxhtml/
+-rw-rw-r--   0 lucjean   (1001) lucjean   (1001)     2143 2023-05-22 07:01:38.000000 coop_html_editor-1.4.1/coop_html_editor/static/ckeditor.4.6.2/samples/old/assets/outputxhtml/outputxhtml.css
+-rw-rw-r--   0 lucjean   (1001) lucjean   (1001)     1443 2023-05-22 07:01:38.000000 coop_html_editor-1.4.1/coop_html_editor/static/ckeditor.4.6.2/samples/old/assets/posteddata.php
+-rw-rw-r--   0 lucjean   (1001) lucjean   (1001)    14449 2023-05-22 07:01:38.000000 coop_html_editor-1.4.1/coop_html_editor/static/ckeditor.4.6.2/samples/old/assets/sample.jpg
+drwxrwxr-x   0 lucjean   (1001) lucjean   (1001)        0 2023-06-12 12:55:08.819913 coop_html_editor-1.4.1/coop_html_editor/static/ckeditor.4.6.2/samples/old/assets/uilanguages/
+-rw-rw-r--   0 lucjean   (1001) lucjean   (1001)     1416 2023-05-22 07:01:38.000000 coop_html_editor-1.4.1/coop_html_editor/static/ckeditor.4.6.2/samples/old/assets/uilanguages/languages.js
+-rw-rw-r--   0 lucjean   (1001) lucjean   (1001)    47482 2023-05-22 07:01:38.000000 coop_html_editor-1.4.1/coop_html_editor/static/ckeditor.4.6.2/samples/old/datafiltering.html
+drwxrwxr-x   0 lucjean   (1001) lucjean   (1001)        0 2023-06-12 12:55:08.819913 coop_html_editor-1.4.1/coop_html_editor/static/ckeditor.4.6.2/samples/old/dialog/
+drwxrwxr-x   0 lucjean   (1001) lucjean   (1001)        0 2023-06-12 12:55:08.819913 coop_html_editor-1.4.1/coop_html_editor/static/ckeditor.4.6.2/samples/old/dialog/assets/
+-rw-rw-r--   0 lucjean   (1001) lucjean   (1001)      877 2023-05-22 07:01:38.000000 coop_html_editor-1.4.1/coop_html_editor/static/ckeditor.4.6.2/samples/old/dialog/assets/my_dialog.js
+-rw-rw-r--   0 lucjean   (1001) lucjean   (1001)     7345 2023-05-22 07:01:38.000000 coop_html_editor-1.4.1/coop_html_editor/static/ckeditor.4.6.2/samples/old/dialog/dialog.html
+-rw-rw-r--   0 lucjean   (1001) lucjean   (1001)     4670 2023-05-22 07:01:38.000000 coop_html_editor-1.4.1/coop_html_editor/static/ckeditor.4.6.2/samples/old/divreplace.html
+drwxrwxr-x   0 lucjean   (1001) lucjean   (1001)        0 2023-06-12 12:55:08.819913 coop_html_editor-1.4.1/coop_html_editor/static/ckeditor.4.6.2/samples/old/enterkey/
+-rw-rw-r--   0 lucjean   (1001) lucjean   (1001)     4352 2023-05-22 07:01:38.000000 coop_html_editor-1.4.1/coop_html_editor/static/ckeditor.4.6.2/samples/old/enterkey/enterkey.html
+drwxrwxr-x   0 lucjean   (1001) lucjean   (1001)        0 2023-06-12 12:55:08.819913 coop_html_editor-1.4.1/coop_html_editor/static/ckeditor.4.6.2/samples/old/htmlwriter/
+drwxrwxr-x   0 lucjean   (1001) lucjean   (1001)        0 2023-06-12 12:55:08.707913 coop_html_editor-1.4.1/coop_html_editor/static/ckeditor.4.6.2/samples/old/htmlwriter/assets/
+drwxrwxr-x   0 lucjean   (1001) lucjean   (1001)        0 2023-06-12 12:55:08.819913 coop_html_editor-1.4.1/coop_html_editor/static/ckeditor.4.6.2/samples/old/htmlwriter/assets/outputforflash/
+-rw-rw-r--   0 lucjean   (1001) lucjean   (1001)    85504 2023-05-22 07:01:38.000000 coop_html_editor-1.4.1/coop_html_editor/static/ckeditor.4.6.2/samples/old/htmlwriter/assets/outputforflash/outputforflash.fla
+-rw-rw-r--   0 lucjean   (1001) lucjean   (1001)    15571 2023-05-22 07:01:38.000000 coop_html_editor-1.4.1/coop_html_editor/static/ckeditor.4.6.2/samples/old/htmlwriter/assets/outputforflash/outputforflash.swf
+-rw-rw-r--   0 lucjean   (1001) lucjean   (1001)     9589 2023-05-22 07:01:38.000000 coop_html_editor-1.4.1/coop_html_editor/static/ckeditor.4.6.2/samples/old/htmlwriter/assets/outputforflash/swfobject.js
+-rw-rw-r--   0 lucjean   (1001) lucjean   (1001)    10108 2023-05-22 07:01:38.000000 coop_html_editor-1.4.1/coop_html_editor/static/ckeditor.4.6.2/samples/old/htmlwriter/outputforflash.html
+-rw-rw-r--   0 lucjean   (1001) lucjean   (1001)     7321 2023-05-22 07:01:38.000000 coop_html_editor-1.4.1/coop_html_editor/static/ckeditor.4.6.2/samples/old/htmlwriter/outputhtml.html
+-rw-rw-r--   0 lucjean   (1001) lucjean   (1001)     5758 2023-05-22 07:01:38.000000 coop_html_editor-1.4.1/coop_html_editor/static/ckeditor.4.6.2/samples/old/index.html
+-rw-rw-r--   0 lucjean   (1001) lucjean   (1001)    10195 2023-05-22 07:01:38.000000 coop_html_editor-1.4.1/coop_html_editor/static/ckeditor.4.6.2/samples/old/inlineall.html
+-rw-rw-r--   0 lucjean   (1001) lucjean   (1001)     6190 2023-05-22 07:01:38.000000 coop_html_editor-1.4.1/coop_html_editor/static/ckeditor.4.6.2/samples/old/inlinebycode.html
+-rw-rw-r--   0 lucjean   (1001) lucjean   (1001)     4920 2023-05-22 07:01:38.000000 coop_html_editor-1.4.1/coop_html_editor/static/ckeditor.4.6.2/samples/old/inlinetextarea.html
+-rw-rw-r--   0 lucjean   (1001) lucjean   (1001)     7511 2023-05-22 07:01:38.000000 coop_html_editor-1.4.1/coop_html_editor/static/ckeditor.4.6.2/samples/old/jquery.html
+drwxrwxr-x   0 lucjean   (1001) lucjean   (1001)        0 2023-06-12 12:55:08.819913 coop_html_editor-1.4.1/coop_html_editor/static/ckeditor.4.6.2/samples/old/magicline/
+-rw-rw-r--   0 lucjean   (1001) lucjean   (1001)     8380 2023-05-22 07:01:38.000000 coop_html_editor-1.4.1/coop_html_editor/static/ckeditor.4.6.2/samples/old/magicline/magicline.html
+-rw-rw-r--   0 lucjean   (1001) lucjean   (1001)     2886 2023-05-22 07:01:38.000000 coop_html_editor-1.4.1/coop_html_editor/static/ckeditor.4.6.2/samples/old/readonly.html
+-rw-rw-r--   0 lucjean   (1001) lucjean   (1001)     7011 2023-05-22 07:01:38.000000 coop_html_editor-1.4.1/coop_html_editor/static/ckeditor.4.6.2/samples/old/replacebyclass.html
+-rw-rw-r--   0 lucjean   (1001) lucjean   (1001)     6914 2023-05-22 07:01:38.000000 coop_html_editor-1.4.1/coop_html_editor/static/ckeditor.4.6.2/samples/old/replacebycode.html
+-rw-rw-r--   0 lucjean   (1001) lucjean   (1001)     5094 2023-05-22 07:01:38.000000 coop_html_editor-1.4.1/coop_html_editor/static/ckeditor.4.6.2/samples/old/sample.css
+-rw-rw-r--   0 lucjean   (1001) lucjean   (1001)     1675 2023-05-22 07:01:38.000000 coop_html_editor-1.4.1/coop_html_editor/static/ckeditor.4.6.2/samples/old/sample.js
+-rw-rw-r--   0 lucjean   (1001) lucjean   (1001)      789 2023-05-22 07:01:38.000000 coop_html_editor-1.4.1/coop_html_editor/static/ckeditor.4.6.2/samples/old/sample_posteddata.php
+-rw-rw-r--   0 lucjean   (1001) lucjean   (1001)     2404 2023-05-22 07:01:38.000000 coop_html_editor-1.4.1/coop_html_editor/static/ckeditor.4.6.2/samples/old/tabindex.html
+drwxrwxr-x   0 lucjean   (1001) lucjean   (1001)        0 2023-06-12 12:55:08.819913 coop_html_editor-1.4.1/coop_html_editor/static/ckeditor.4.6.2/samples/old/toolbar/
+-rw-rw-r--   0 lucjean   (1001) lucjean   (1001)     8900 2023-05-22 07:01:38.000000 coop_html_editor-1.4.1/coop_html_editor/static/ckeditor.4.6.2/samples/old/toolbar/toolbar.html
+-rw-rw-r--   0 lucjean   (1001) lucjean   (1001)     2604 2023-05-22 07:01:38.000000 coop_html_editor-1.4.1/coop_html_editor/static/ckeditor.4.6.2/samples/old/uicolor.html
+-rw-rw-r--   0 lucjean   (1001) lucjean   (1001)     4495 2023-05-22 07:01:38.000000 coop_html_editor-1.4.1/coop_html_editor/static/ckeditor.4.6.2/samples/old/uilanguages.html
+drwxrwxr-x   0 lucjean   (1001) lucjean   (1001)        0 2023-06-12 12:55:08.819913 coop_html_editor-1.4.1/coop_html_editor/static/ckeditor.4.6.2/samples/old/wysiwygarea/
+-rw-rw-r--   0 lucjean   (1001) lucjean   (1001)     8106 2023-05-22 07:01:38.000000 coop_html_editor-1.4.1/coop_html_editor/static/ckeditor.4.6.2/samples/old/wysiwygarea/fullpage.html
+-rw-rw-r--   0 lucjean   (1001) lucjean   (1001)     7027 2023-05-22 07:01:38.000000 coop_html_editor-1.4.1/coop_html_editor/static/ckeditor.4.6.2/samples/old/xhtmlstyle.html
+drwxrwxr-x   0 lucjean   (1001) lucjean   (1001)        0 2023-06-12 12:55:08.819913 coop_html_editor-1.4.1/coop_html_editor/static/ckeditor.4.6.2/samples/toolbarconfigurator/
+drwxrwxr-x   0 lucjean   (1001) lucjean   (1001)        0 2023-06-12 12:55:08.819913 coop_html_editor-1.4.1/coop_html_editor/static/ckeditor.4.6.2/samples/toolbarconfigurator/css/
+-rw-rw-r--   0 lucjean   (1001) lucjean   (1001)     1758 2023-05-22 07:01:38.000000 coop_html_editor-1.4.1/coop_html_editor/static/ckeditor.4.6.2/samples/toolbarconfigurator/css/fontello.css
+drwxrwxr-x   0 lucjean   (1001) lucjean   (1001)        0 2023-06-12 12:55:08.819913 coop_html_editor-1.4.1/coop_html_editor/static/ckeditor.4.6.2/samples/toolbarconfigurator/font/
+-rw-rw-r--   0 lucjean   (1001) lucjean   (1001)      188 2023-05-22 07:01:38.000000 coop_html_editor-1.4.1/coop_html_editor/static/ckeditor.4.6.2/samples/toolbarconfigurator/font/LICENSE.txt
+-rw-rw-r--   0 lucjean   (1001) lucjean   (1001)      557 2023-05-22 07:01:38.000000 coop_html_editor-1.4.1/coop_html_editor/static/ckeditor.4.6.2/samples/toolbarconfigurator/font/config.json
+-rw-rw-r--   0 lucjean   (1001) lucjean   (1001)     4988 2023-05-22 07:01:38.000000 coop_html_editor-1.4.1/coop_html_editor/static/ckeditor.4.6.2/samples/toolbarconfigurator/font/fontello.eot
+-rw-rw-r--   0 lucjean   (1001) lucjean   (1001)     1701 2023-05-22 07:01:38.000000 coop_html_editor-1.4.1/coop_html_editor/static/ckeditor.4.6.2/samples/toolbarconfigurator/font/fontello.svg
+-rw-rw-r--   0 lucjean   (1001) lucjean   (1001)     4820 2023-05-22 07:01:38.000000 coop_html_editor-1.4.1/coop_html_editor/static/ckeditor.4.6.2/samples/toolbarconfigurator/font/fontello.ttf
+-rw-rw-r--   0 lucjean   (1001) lucjean   (1001)     2904 2023-05-22 07:01:38.000000 coop_html_editor-1.4.1/coop_html_editor/static/ckeditor.4.6.2/samples/toolbarconfigurator/font/fontello.woff
+-rw-rw-r--   0 lucjean   (1001) lucjean   (1001)    15449 2023-05-22 07:01:38.000000 coop_html_editor-1.4.1/coop_html_editor/static/ckeditor.4.6.2/samples/toolbarconfigurator/index.html
+drwxrwxr-x   0 lucjean   (1001) lucjean   (1001)        0 2023-06-12 12:55:08.823913 coop_html_editor-1.4.1/coop_html_editor/static/ckeditor.4.6.2/samples/toolbarconfigurator/js/
+-rw-rw-r--   0 lucjean   (1001) lucjean   (1001)     6523 2023-05-22 07:01:38.000000 coop_html_editor-1.4.1/coop_html_editor/static/ckeditor.4.6.2/samples/toolbarconfigurator/js/abstracttoolbarmodifier.js
+-rw-rw-r--   0 lucjean   (1001) lucjean   (1001)     3819 2023-05-22 07:01:38.000000 coop_html_editor-1.4.1/coop_html_editor/static/ckeditor.4.6.2/samples/toolbarconfigurator/js/fulltoolbareditor.js
+-rw-rw-r--   0 lucjean   (1001) lucjean   (1001)    16651 2023-05-22 07:01:38.000000 coop_html_editor-1.4.1/coop_html_editor/static/ckeditor.4.6.2/samples/toolbarconfigurator/js/toolbarmodifier.js
+-rw-rw-r--   0 lucjean   (1001) lucjean   (1001)     6850 2023-05-22 07:01:38.000000 coop_html_editor-1.4.1/coop_html_editor/static/ckeditor.4.6.2/samples/toolbarconfigurator/js/toolbartextmodifier.js
+drwxrwxr-x   0 lucjean   (1001) lucjean   (1001)        0 2023-06-12 12:55:08.707913 coop_html_editor-1.4.1/coop_html_editor/static/ckeditor.4.6.2/samples/toolbarconfigurator/lib/
+drwxrwxr-x   0 lucjean   (1001) lucjean   (1001)        0 2023-06-12 12:55:08.823913 coop_html_editor-1.4.1/coop_html_editor/static/ckeditor.4.6.2/samples/toolbarconfigurator/lib/codemirror/
+-rw-rw-r--   0 lucjean   (1001) lucjean   (1001)     1094 2023-05-22 07:01:38.000000 coop_html_editor-1.4.1/coop_html_editor/static/ckeditor.4.6.2/samples/toolbarconfigurator/lib/codemirror/LICENSE
+-rw-rw-r--   0 lucjean   (1001) lucjean   (1001)     8096 2023-05-22 07:01:38.000000 coop_html_editor-1.4.1/coop_html_editor/static/ckeditor.4.6.2/samples/toolbarconfigurator/lib/codemirror/codemirror.css
+-rw-rw-r--   0 lucjean   (1001) lucjean   (1001)   148874 2023-05-22 07:01:38.000000 coop_html_editor-1.4.1/coop_html_editor/static/ckeditor.4.6.2/samples/toolbarconfigurator/lib/codemirror/codemirror.js
+-rw-rw-r--   0 lucjean   (1001) lucjean   (1001)    12285 2023-05-22 07:01:38.000000 coop_html_editor-1.4.1/coop_html_editor/static/ckeditor.4.6.2/samples/toolbarconfigurator/lib/codemirror/javascript.js
+-rw-rw-r--   0 lucjean   (1001) lucjean   (1001)      851 2023-05-22 07:01:38.000000 coop_html_editor-1.4.1/coop_html_editor/static/ckeditor.4.6.2/samples/toolbarconfigurator/lib/codemirror/neo.css
+-rw-rw-r--   0 lucjean   (1001) lucjean   (1001)      700 2023-05-22 07:01:38.000000 coop_html_editor-1.4.1/coop_html_editor/static/ckeditor.4.6.2/samples/toolbarconfigurator/lib/codemirror/show-hint.css
+-rw-rw-r--   0 lucjean   (1001) lucjean   (1001)     8080 2023-05-22 07:01:38.000000 coop_html_editor-1.4.1/coop_html_editor/static/ckeditor.4.6.2/samples/toolbarconfigurator/lib/codemirror/show-hint.js
+drwxrwxr-x   0 lucjean   (1001) lucjean   (1001)        0 2023-06-12 12:55:08.707913 coop_html_editor-1.4.1/coop_html_editor/static/ckeditor.4.6.2/skins/
+drwxrwxr-x   0 lucjean   (1001) lucjean   (1001)        0 2023-06-12 12:55:08.823913 coop_html_editor-1.4.1/coop_html_editor/static/ckeditor.4.6.2/skins/moono-lisa/
+-rw-rw-r--   0 lucjean   (1001) lucjean   (1001)    13550 2023-05-22 07:01:38.000000 coop_html_editor-1.4.1/coop_html_editor/static/ckeditor.4.6.2/skins/moono-lisa/dialog.css
+-rw-rw-r--   0 lucjean   (1001) lucjean   (1001)    14461 2023-05-22 07:01:38.000000 coop_html_editor-1.4.1/coop_html_editor/static/ckeditor.4.6.2/skins/moono-lisa/dialog_ie.css
+-rw-rw-r--   0 lucjean   (1001) lucjean   (1001)    14944 2023-05-22 07:01:38.000000 coop_html_editor-1.4.1/coop_html_editor/static/ckeditor.4.6.2/skins/moono-lisa/dialog_ie8.css
+-rw-rw-r--   0 lucjean   (1001) lucjean   (1001)    14490 2023-05-22 07:01:38.000000 coop_html_editor-1.4.1/coop_html_editor/static/ckeditor.4.6.2/skins/moono-lisa/dialog_iequirks.css
+-rw-rw-r--   0 lucjean   (1001) lucjean   (1001)    35766 2023-05-22 07:01:38.000000 coop_html_editor-1.4.1/coop_html_editor/static/ckeditor.4.6.2/skins/moono-lisa/editor.css
+-rw-rw-r--   0 lucjean   (1001) lucjean   (1001)    35847 2023-05-22 07:01:38.000000 coop_html_editor-1.4.1/coop_html_editor/static/ckeditor.4.6.2/skins/moono-lisa/editor_gecko.css
+-rw-rw-r--   0 lucjean   (1001) lucjean   (1001)    36765 2023-05-22 07:01:38.000000 coop_html_editor-1.4.1/coop_html_editor/static/ckeditor.4.6.2/skins/moono-lisa/editor_ie.css
+-rw-rw-r--   0 lucjean   (1001) lucjean   (1001)    37571 2023-05-22 07:01:38.000000 coop_html_editor-1.4.1/coop_html_editor/static/ckeditor.4.6.2/skins/moono-lisa/editor_ie8.css
+-rw-rw-r--   0 lucjean   (1001) lucjean   (1001)    37414 2023-05-22 07:01:38.000000 coop_html_editor-1.4.1/coop_html_editor/static/ckeditor.4.6.2/skins/moono-lisa/editor_iequirks.css
+-rw-rw-r--   0 lucjean   (1001) lucjean   (1001)     6057 2023-05-22 07:01:38.000000 coop_html_editor-1.4.1/coop_html_editor/static/ckeditor.4.6.2/skins/moono-lisa/icons.png
+-rw-rw-r--   0 lucjean   (1001) lucjean   (1001)    20877 2023-05-22 07:01:38.000000 coop_html_editor-1.4.1/coop_html_editor/static/ckeditor.4.6.2/skins/moono-lisa/icons_hidpi.png
+drwxrwxr-x   0 lucjean   (1001) lucjean   (1001)        0 2023-06-12 12:55:08.823913 coop_html_editor-1.4.1/coop_html_editor/static/ckeditor.4.6.2/skins/moono-lisa/images/
+-rw-rw-r--   0 lucjean   (1001) lucjean   (1001)      191 2023-05-22 07:01:38.000000 coop_html_editor-1.4.1/coop_html_editor/static/ckeditor.4.6.2/skins/moono-lisa/images/arrow.png
+-rw-rw-r--   0 lucjean   (1001) lucjean   (1001)      615 2023-05-22 07:01:38.000000 coop_html_editor-1.4.1/coop_html_editor/static/ckeditor.4.6.2/skins/moono-lisa/images/close.png
+drwxrwxr-x   0 lucjean   (1001) lucjean   (1001)        0 2023-06-12 12:55:08.827913 coop_html_editor-1.4.1/coop_html_editor/static/ckeditor.4.6.2/skins/moono-lisa/images/hidpi/
+-rw-rw-r--   0 lucjean   (1001) lucjean   (1001)     1238 2023-05-22 07:01:38.000000 coop_html_editor-1.4.1/coop_html_editor/static/ckeditor.4.6.2/skins/moono-lisa/images/hidpi/close.png
+-rw-rw-r--   0 lucjean   (1001) lucjean   (1001)     1071 2023-05-22 07:01:38.000000 coop_html_editor-1.4.1/coop_html_editor/static/ckeditor.4.6.2/skins/moono-lisa/images/hidpi/lock-open.png
+-rw-rw-r--   0 lucjean   (1001) lucjean   (1001)     1062 2023-05-22 07:01:38.000000 coop_html_editor-1.4.1/coop_html_editor/static/ckeditor.4.6.2/skins/moono-lisa/images/hidpi/lock.png
+-rw-rw-r--   0 lucjean   (1001) lucjean   (1001)     1623 2023-05-22 07:01:38.000000 coop_html_editor-1.4.1/coop_html_editor/static/ckeditor.4.6.2/skins/moono-lisa/images/hidpi/refresh.png
+-rw-rw-r--   0 lucjean   (1001) lucjean   (1001)      511 2023-05-22 07:01:38.000000 coop_html_editor-1.4.1/coop_html_editor/static/ckeditor.4.6.2/skins/moono-lisa/images/lock-open.png
+-rw-rw-r--   0 lucjean   (1001) lucjean   (1001)      506 2023-05-22 07:01:38.000000 coop_html_editor-1.4.1/coop_html_editor/static/ckeditor.4.6.2/skins/moono-lisa/images/lock.png
+-rw-rw-r--   0 lucjean   (1001) lucjean   (1001)      757 2023-05-22 07:01:38.000000 coop_html_editor-1.4.1/coop_html_editor/static/ckeditor.4.6.2/skins/moono-lisa/images/refresh.png
+-rw-rw-r--   0 lucjean   (1001) lucjean   (1001)     2984 2023-05-22 07:01:38.000000 coop_html_editor-1.4.1/coop_html_editor/static/ckeditor.4.6.2/skins/moono-lisa/images/spinner.gif
+-rw-rw-r--   0 lucjean   (1001) lucjean   (1001)     2224 2023-05-22 07:01:38.000000 coop_html_editor-1.4.1/coop_html_editor/static/ckeditor.4.6.2/skins/moono-lisa/readme.md
+-rw-rw-r--   0 lucjean   (1001) lucjean   (1001)     5516 2023-05-22 07:01:38.000000 coop_html_editor-1.4.1/coop_html_editor/static/ckeditor.4.6.2/styles.js
+drwxrwxr-x   0 lucjean   (1001) lucjean   (1001)        0 2023-06-12 12:55:08.827913 coop_html_editor-1.4.1/coop_html_editor/static/js/
+-rw-rw-r--   0 lucjean   (1001) lucjean   (1001)   252881 2023-05-22 07:01:38.000000 coop_html_editor-1.4.1/coop_html_editor/static/js/jquery-1.7.2.js
+-rw-rw-r--   0 lucjean   (1001) lucjean   (1001)    94840 2023-05-22 07:01:38.000000 coop_html_editor-1.4.1/coop_html_editor/static/js/jquery-1.7.2.min.js
+drwxrwxr-x   0 lucjean   (1001) lucjean   (1001)        0 2023-06-12 12:55:08.707913 coop_html_editor-1.4.1/coop_html_editor/templates/
+drwxrwxr-x   0 lucjean   (1001) lucjean   (1001)        0 2023-06-12 12:55:08.827913 coop_html_editor-1.4.1/coop_html_editor/templates/html_editor/
+-rw-rw-r--   0 lucjean   (1001) lucjean   (1001)     2486 2023-05-22 07:01:38.000000 coop_html_editor-1.4.1/coop_html_editor/templates/html_editor/ckeditor-init.js
+-rw-rw-r--   0 lucjean   (1001) lucjean   (1001)     1442 2023-05-22 07:01:38.000000 coop_html_editor-1.4.1/coop_html_editor/templates/html_editor/ckeditor_config.js
+-rw-rw-r--   0 lucjean   (1001) lucjean   (1001)      247 2023-05-22 07:01:38.000000 coop_html_editor-1.4.1/coop_html_editor/templates/html_editor/ckeditor_input.html
+-rw-rw-r--   0 lucjean   (1001) lucjean   (1001)     2675 2023-05-22 07:01:38.000000 coop_html_editor-1.4.1/coop_html_editor/templates/html_editor/image_browser.html
+-rw-rw-r--   0 lucjean   (1001) lucjean   (1001)     3307 2023-05-22 07:01:38.000000 coop_html_editor-1.4.1/coop_html_editor/templates/html_editor/link_browser.html
+drwxrwxr-x   0 lucjean   (1001) lucjean   (1001)        0 2023-06-12 12:55:08.827913 coop_html_editor-1.4.1/coop_html_editor/templatetags/
+-rw-rw-r--   0 lucjean   (1001) lucjean   (1001)       23 2023-05-22 07:01:38.000000 coop_html_editor-1.4.1/coop_html_editor/templatetags/__init__.py
+-rw-rw-r--   0 lucjean   (1001) lucjean   (1001)     5578 2023-06-12 12:48:33.000000 coop_html_editor-1.4.1/coop_html_editor/templatetags/html_editor_utils.py
+-rw-rw-r--   0 lucjean   (1001) lucjean   (1001)      451 2023-06-12 12:48:33.000000 coop_html_editor-1.4.1/coop_html_editor/urls.py
+-rw-rw-r--   0 lucjean   (1001) lucjean   (1001)     1069 2023-06-12 12:48:33.000000 coop_html_editor-1.4.1/coop_html_editor/utils.py
+-rw-rw-r--   0 lucjean   (1001) lucjean   (1001)     2466 2023-06-12 12:48:33.000000 coop_html_editor-1.4.1/coop_html_editor/views.py
+-rw-rw-r--   0 lucjean   (1001) lucjean   (1001)     2013 2023-06-12 12:48:33.000000 coop_html_editor-1.4.1/coop_html_editor/widgets.py
+drwxrwxr-x   0 lucjean   (1001) lucjean   (1001)        0 2023-06-12 12:55:08.707913 coop_html_editor-1.4.1/coop_html_editor.egg-info/
+-rw-rw-r--   0 lucjean   (1001) lucjean   (1001)     5228 2023-06-12 12:55:08.000000 coop_html_editor-1.4.1/coop_html_editor.egg-info/PKG-INFO
+-rw-rw-r--   0 lucjean   (1001) lucjean   (1001)    47644 2023-06-12 12:55:08.000000 coop_html_editor-1.4.1/coop_html_editor.egg-info/SOURCES.txt
+-rw-rw-r--   0 lucjean   (1001) lucjean   (1001)        1 2023-06-12 12:55:08.000000 coop_html_editor-1.4.1/coop_html_editor.egg-info/dependency_links.txt
+-rw-rw-r--   0 lucjean   (1001) lucjean   (1001)        1 2023-05-22 10:25:46.000000 coop_html_editor-1.4.1/coop_html_editor.egg-info/not-zip-safe
+-rw-rw-r--   0 lucjean   (1001) lucjean   (1001)       26 2023-06-12 12:55:08.000000 coop_html_editor-1.4.1/coop_html_editor.egg-info/requires.txt
+-rw-rw-r--   0 lucjean   (1001) lucjean   (1001)       17 2023-06-12 12:55:08.000000 coop_html_editor-1.4.1/coop_html_editor.egg-info/top_level.txt
+-rw-rw-r--   0 lucjean   (1001) lucjean   (1001)       38 2023-06-12 12:55:08.827913 coop_html_editor-1.4.1/setup.cfg
+-rw-rw-r--   0 lucjean   (1001) lucjean   (1001)      756 2023-05-22 07:01:38.000000 coop_html_editor-1.4.1/setup.py
```

### filetype from file(1)

```diff
@@ -1 +1 @@
-POSIX tar archive (GNU)
+POSIX tar archive
```

### Comparing `coop_html_editor-1.3.1/PKG-INFO` & `coop_html_editor-1.4.1/coop_html_editor.egg-info/PKG-INFO`

 * *Files 14% similar despite different names*

```diff
@@ -1,151 +1,150 @@
-Metadata-Version: 1.1
-Name: coop_html_editor
-Version: 1.3.1
+Metadata-Version: 2.1
+Name: coop-html-editor
+Version: 1.4.1
 Summary: integration for Inline HTML editor
 Home-page: https://github.com/ljean/coop_html_editor/
+Download-URL: https://github.com/ljean/coop_html_editor/tarball/master
 Author: Luc Jean
 Author-email: ljean@apidev.fr
 License: BSD
-Download-URL: https://github.com/ljean/coop_html_editor/tarball/master
-Description: coop HTML Editor
-        ===============================================
-        
-        * `What is coop_html_editor good for?`_
-        * `Quick start`_
-        * `Settings`_
-        
-        .. _What is coop_html_editor good for?: #good-for
-        .. _Quick start?: #quick-start
-        .. _Settings?: #settings
-        
-        .. _good-for:
-        
-        What is coop_html_editor good for?
-        ------------------------------------
-        coop_html_editor is a backend for using inline HTML editor into a Django site.
-        It enables inline editing for your HTML content.
-        It includes a django Form and a Widget helper.
-        It supports Aloha Editor and CK Editor
-        
-        .. _quick-start:
-        
-        Quick start
-        ------------------------------------
-        In settings.py, add 'coop_html_editor' to the INSTALLED_APPS
-        In urls.py add ``(r'^html-editor/', include('coop_html_editor.urls'))`` to your urlpatterns
-        
-        Then create a form. For example something like ::
-        
-            import floppyforms.__future__ as floppyforms
-            from models import Note
-            from coop_html_editor.widgets import get_inline_html_widget
-            
-            class NoteForm(floppyforms.ModelForm):
-                class Meta:
-                    model = Note
-                    fields = ('text',)
-                    widgets = {
-                        'text': get_inline_html_widget(),
-                    }
-        
-        
-        Let's assume that you've a ``form`` variable pointing on an instance of a NoteForm.
-        In the template file, call the form and don't forget to put ``{{form.media}}`` in the headers.
-        
-        .. _settings:
-        
-        Settings
-        ------------------------------------
-        
-        The following constants can be set in your django project settings.py
-        
-        You can choose between 2 HTML editors : Aloha editor or CkEditor. We recommend to use CkEditor but keep Aloha by default
-        for compatibility. Add one the 2 lines below in your settings.py
-        
-        In settings::
-        
-            COOP_HTML_EDITOR = 'aloha'
-            COOP_HTML_EDITOR = 'ck-editor'
-        
-        You can tune your editor by changing the settings below. The values in this README correspond to defaults
-        
-        For both, we package a default version than can be overriden by copying your own version folder in ste static files
-        and define the new version by
-        
-        In settings::
-        
-            ALOHA_VERSION = "aloha.0.23.26"
-            CKEDITOR_VERSION = "ckeditor.4.6.2"
-        
-        The initialisation code of the editor is set in a javascript file. You can change the file to use by seetings
-        
-        In settings::
-        
-            ALOHA_INIT_JS_TEMPLATE = "html_editor/aloha_init.js"
-            CKEDITOR_INIT_JS_TEMPLATE = "html_editor/ckeditor-init.js"
-        
-        If you choose CkEditor, you can add your own styles
-        
-        In settings::
-        
-            CKEDITOR_CSS_CLASSES = [
-                 "{name: 'Highlight', element: 'span', attributes: {'class': 'highlight'}}",
-                 "{name: 'Red Title', element: 'h3', styles: {color: '#880000'}}",
-            ]
-        
-        
-        InlineHtmlInput has a "provider" that allows you to add local links to your models (articles, contacts, whatever) easily, through an autocomplete field that will search for objects based on rules you defined for each model :
-        
-        * search this kind of models using get_absolute_url()
-        * search this kind of models using another method
-        * search this kind of models using a specified model field
-        
-        You can set the ``HTML_EDITOR_LINK_MODELS`` setting in your settings.py to tell which django models will be available in the auto-complete field of the "add link" widget like this ::
-        
-            HTML_EDITOR_LINK_MODELS = ('coop_local.Article', 'calendar.Event', )
-            
-            
-        djaloha requires jquery and is provided by default with jquery.1.7.2. You can change the jquery version if needed ::
-        
-            HTML_EDITOR_JQUERY = 'js/jquery.1.7.2.js'
-            
-            
-        Aloha has a nice plugin architecture. coop_html_editor includes by default the main Aloha plugins. You may want to have a different set of plugins.
-        Please refer to the Aloha docs for more information on plugins ::
-        
-            ALOHA_PLUGINS = (
-                "common/format",
-                "common/highlighteditables",
-                "common/list",
-                "common/link",
-                "common/undo",
-                "common/paste",
-                "common/commands",
-                "common/image",
-                "common/align",
-                "extra/attributes",
-                "common/characterpicker",
-                "common/abbr",
-                "common/horizontalruler",
-                "common/table",
-                "extra/browser",
-            )
-            
-        
-        Please note that the ``ALOHA_PLUGINS`` setting is a global setting. If you need to change the set of plugins for a specific form field, you
-        can pass a similar tuple in the ``aloha_plugins`` attribute of your ``coop_html_editor`` widget.
-        The ``extra_aloha_plugins`` attribute will add additional plugins to the default set.
-        
-        ``HTML_EDITOR_INIT_URL`` setting make possible to overload the aloha init file of djaloha.
-        ``html_editor_init_url`` attribute of ``InlineHtmlInput`` can also be used to overload it for a specific form field.
-        
-        License
-        =======
-        
-        coop_html_editor is based on apidev-djaloha is a fork from credis/djaloha (see http://github.com/credis/djaloha)
-        
-        coop_html_editor uses the BSD license. see license.txt
-        
-        Djaloha development was funded by `CREDIS <http://credis.org/>`_, FSE (European Social Fund) and Conseil Regional d'Auvergne.
-        
-Platform: UNKNOWN
+
+coop HTML Editor
+===============================================
+
+* `What is coop_html_editor good for?`_
+* `Quick start`_
+* `Settings`_
+
+.. _What is coop_html_editor good for?: #good-for
+.. _Quick start?: #quick-start
+.. _Settings?: #settings
+
+.. _good-for:
+
+What is coop_html_editor good for?
+------------------------------------
+coop_html_editor is a backend for using inline HTML editor into a Django site.
+It enables inline editing for your HTML content.
+It includes a django Form and a Widget helper.
+It supports Aloha Editor and CK Editor
+
+.. _quick-start:
+
+Quick start
+------------------------------------
+In settings.py, add 'coop_html_editor' to the INSTALLED_APPS
+In urls.py add ``(r'^html-editor/', include('coop_html_editor.urls'))`` to your urlpatterns
+
+Then create a form. For example something like ::
+
+    import floppyforms.__future__ as floppyforms
+    from models import Note
+    from coop_html_editor.widgets import get_inline_html_widget
+    
+    class NoteForm(floppyforms.ModelForm):
+        class Meta:
+            model = Note
+            fields = ('text',)
+            widgets = {
+                'text': get_inline_html_widget(),
+            }
+
+
+Let's assume that you've a ``form`` variable pointing on an instance of a NoteForm.
+In the template file, call the form and don't forget to put ``{{form.media}}`` in the headers.
+
+.. _settings:
+
+Settings
+------------------------------------
+
+The following constants can be set in your django project settings.py
+
+You can choose between 2 HTML editors : Aloha editor or CkEditor. We recommend to use CkEditor but keep Aloha by default
+for compatibility. Add one the 2 lines below in your settings.py
+
+In settings::
+
+    COOP_HTML_EDITOR = 'aloha'
+    COOP_HTML_EDITOR = 'ck-editor'
+
+You can tune your editor by changing the settings below. The values in this README correspond to defaults
+
+For both, we package a default version than can be overriden by copying your own version folder in ste static files
+and define the new version by
+
+In settings::
+
+    ALOHA_VERSION = "aloha.0.23.26"
+    CKEDITOR_VERSION = "ckeditor.4.6.2"
+
+The initialisation code of the editor is set in a javascript file. You can change the file to use by seetings
+
+In settings::
+
+    ALOHA_INIT_JS_TEMPLATE = "html_editor/aloha_init.js"
+    CKEDITOR_INIT_JS_TEMPLATE = "html_editor/ckeditor-init.js"
+
+If you choose CkEditor, you can add your own styles
+
+In settings::
+
+    CKEDITOR_CSS_CLASSES = [
+         "{name: 'Highlight', element: 'span', attributes: {'class': 'highlight'}}",
+         "{name: 'Red Title', element: 'h3', styles: {color: '#880000'}}",
+    ]
+
+
+InlineHtmlInput has a "provider" that allows you to add local links to your models (articles, contacts, whatever) easily, through an autocomplete field that will search for objects based on rules you defined for each model :
+
+* search this kind of models using get_absolute_url()
+* search this kind of models using another method
+* search this kind of models using a specified model field
+
+You can set the ``HTML_EDITOR_LINK_MODELS`` setting in your settings.py to tell which django models will be available in the auto-complete field of the "add link" widget like this ::
+
+    HTML_EDITOR_LINK_MODELS = ('coop_local.Article', 'calendar.Event', )
+    
+    
+djaloha requires jquery and is provided by default with jquery.1.7.2. You can change the jquery version if needed ::
+
+    HTML_EDITOR_JQUERY = 'js/jquery.1.7.2.js'
+    
+    
+Aloha has a nice plugin architecture. coop_html_editor includes by default the main Aloha plugins. You may want to have a different set of plugins.
+Please refer to the Aloha docs for more information on plugins ::
+
+    ALOHA_PLUGINS = (
+        "common/format",
+        "common/highlighteditables",
+        "common/list",
+        "common/link",
+        "common/undo",
+        "common/paste",
+        "common/commands",
+        "common/image",
+        "common/align",
+        "extra/attributes",
+        "common/characterpicker",
+        "common/abbr",
+        "common/horizontalruler",
+        "common/table",
+        "extra/browser",
+    )
+    
+
+Please note that the ``ALOHA_PLUGINS`` setting is a global setting. If you need to change the set of plugins for a specific form field, you
+can pass a similar tuple in the ``aloha_plugins`` attribute of your ``coop_html_editor`` widget.
+The ``extra_aloha_plugins`` attribute will add additional plugins to the default set.
+
+``HTML_EDITOR_INIT_URL`` setting make possible to overload the aloha init file of djaloha.
+``html_editor_init_url`` attribute of ``InlineHtmlInput`` can also be used to overload it for a specific form field.
+
+License
+=======
+
+coop_html_editor is based on apidev-djaloha is a fork from credis/djaloha (see http://github.com/credis/djaloha)
+
+coop_html_editor uses the BSD license. see license.txt
+
+Djaloha development was funded by `CREDIS <http://credis.org/>`_, FSE (European Social Fund) and Conseil Regional d'Auvergne.
```

### Comparing `coop_html_editor-1.3.1/coop_html_editor.egg-info/PKG-INFO` & `coop_html_editor-1.4.1/PKG-INFO`

 * *Files 15% similar despite different names*

```diff
@@ -1,151 +1,150 @@
-Metadata-Version: 1.1
-Name: coop-html-editor
-Version: 1.3.1
+Metadata-Version: 2.1
+Name: coop_html_editor
+Version: 1.4.1
 Summary: integration for Inline HTML editor
 Home-page: https://github.com/ljean/coop_html_editor/
+Download-URL: https://github.com/ljean/coop_html_editor/tarball/master
 Author: Luc Jean
 Author-email: ljean@apidev.fr
 License: BSD
-Download-URL: https://github.com/ljean/coop_html_editor/tarball/master
-Description: coop HTML Editor
-        ===============================================
-        
-        * `What is coop_html_editor good for?`_
-        * `Quick start`_
-        * `Settings`_
-        
-        .. _What is coop_html_editor good for?: #good-for
-        .. _Quick start?: #quick-start
-        .. _Settings?: #settings
-        
-        .. _good-for:
-        
-        What is coop_html_editor good for?
-        ------------------------------------
-        coop_html_editor is a backend for using inline HTML editor into a Django site.
-        It enables inline editing for your HTML content.
-        It includes a django Form and a Widget helper.
-        It supports Aloha Editor and CK Editor
-        
-        .. _quick-start:
-        
-        Quick start
-        ------------------------------------
-        In settings.py, add 'coop_html_editor' to the INSTALLED_APPS
-        In urls.py add ``(r'^html-editor/', include('coop_html_editor.urls'))`` to your urlpatterns
-        
-        Then create a form. For example something like ::
-        
-            import floppyforms.__future__ as floppyforms
-            from models import Note
-            from coop_html_editor.widgets import get_inline_html_widget
-            
-            class NoteForm(floppyforms.ModelForm):
-                class Meta:
-                    model = Note
-                    fields = ('text',)
-                    widgets = {
-                        'text': get_inline_html_widget(),
-                    }
-        
-        
-        Let's assume that you've a ``form`` variable pointing on an instance of a NoteForm.
-        In the template file, call the form and don't forget to put ``{{form.media}}`` in the headers.
-        
-        .. _settings:
-        
-        Settings
-        ------------------------------------
-        
-        The following constants can be set in your django project settings.py
-        
-        You can choose between 2 HTML editors : Aloha editor or CkEditor. We recommend to use CkEditor but keep Aloha by default
-        for compatibility. Add one the 2 lines below in your settings.py
-        
-        In settings::
-        
-            COOP_HTML_EDITOR = 'aloha'
-            COOP_HTML_EDITOR = 'ck-editor'
-        
-        You can tune your editor by changing the settings below. The values in this README correspond to defaults
-        
-        For both, we package a default version than can be overriden by copying your own version folder in ste static files
-        and define the new version by
-        
-        In settings::
-        
-            ALOHA_VERSION = "aloha.0.23.26"
-            CKEDITOR_VERSION = "ckeditor.4.6.2"
-        
-        The initialisation code of the editor is set in a javascript file. You can change the file to use by seetings
-        
-        In settings::
-        
-            ALOHA_INIT_JS_TEMPLATE = "html_editor/aloha_init.js"
-            CKEDITOR_INIT_JS_TEMPLATE = "html_editor/ckeditor-init.js"
-        
-        If you choose CkEditor, you can add your own styles
-        
-        In settings::
-        
-            CKEDITOR_CSS_CLASSES = [
-                 "{name: 'Highlight', element: 'span', attributes: {'class': 'highlight'}}",
-                 "{name: 'Red Title', element: 'h3', styles: {color: '#880000'}}",
-            ]
-        
-        
-        InlineHtmlInput has a "provider" that allows you to add local links to your models (articles, contacts, whatever) easily, through an autocomplete field that will search for objects based on rules you defined for each model :
-        
-        * search this kind of models using get_absolute_url()
-        * search this kind of models using another method
-        * search this kind of models using a specified model field
-        
-        You can set the ``HTML_EDITOR_LINK_MODELS`` setting in your settings.py to tell which django models will be available in the auto-complete field of the "add link" widget like this ::
-        
-            HTML_EDITOR_LINK_MODELS = ('coop_local.Article', 'calendar.Event', )
-            
-            
-        djaloha requires jquery and is provided by default with jquery.1.7.2. You can change the jquery version if needed ::
-        
-            HTML_EDITOR_JQUERY = 'js/jquery.1.7.2.js'
-            
-            
-        Aloha has a nice plugin architecture. coop_html_editor includes by default the main Aloha plugins. You may want to have a different set of plugins.
-        Please refer to the Aloha docs for more information on plugins ::
-        
-            ALOHA_PLUGINS = (
-                "common/format",
-                "common/highlighteditables",
-                "common/list",
-                "common/link",
-                "common/undo",
-                "common/paste",
-                "common/commands",
-                "common/image",
-                "common/align",
-                "extra/attributes",
-                "common/characterpicker",
-                "common/abbr",
-                "common/horizontalruler",
-                "common/table",
-                "extra/browser",
-            )
-            
-        
-        Please note that the ``ALOHA_PLUGINS`` setting is a global setting. If you need to change the set of plugins for a specific form field, you
-        can pass a similar tuple in the ``aloha_plugins`` attribute of your ``coop_html_editor`` widget.
-        The ``extra_aloha_plugins`` attribute will add additional plugins to the default set.
-        
-        ``HTML_EDITOR_INIT_URL`` setting make possible to overload the aloha init file of djaloha.
-        ``html_editor_init_url`` attribute of ``InlineHtmlInput`` can also be used to overload it for a specific form field.
-        
-        License
-        =======
-        
-        coop_html_editor is based on apidev-djaloha is a fork from credis/djaloha (see http://github.com/credis/djaloha)
-        
-        coop_html_editor uses the BSD license. see license.txt
-        
-        Djaloha development was funded by `CREDIS <http://credis.org/>`_, FSE (European Social Fund) and Conseil Regional d'Auvergne.
-        
-Platform: UNKNOWN
+
+coop HTML Editor
+===============================================
+
+* `What is coop_html_editor good for?`_
+* `Quick start`_
+* `Settings`_
+
+.. _What is coop_html_editor good for?: #good-for
+.. _Quick start?: #quick-start
+.. _Settings?: #settings
+
+.. _good-for:
+
+What is coop_html_editor good for?
+------------------------------------
+coop_html_editor is a backend for using inline HTML editor into a Django site.
+It enables inline editing for your HTML content.
+It includes a django Form and a Widget helper.
+It supports Aloha Editor and CK Editor
+
+.. _quick-start:
+
+Quick start
+------------------------------------
+In settings.py, add 'coop_html_editor' to the INSTALLED_APPS
+In urls.py add ``(r'^html-editor/', include('coop_html_editor.urls'))`` to your urlpatterns
+
+Then create a form. For example something like ::
+
+    import floppyforms.__future__ as floppyforms
+    from models import Note
+    from coop_html_editor.widgets import get_inline_html_widget
+    
+    class NoteForm(floppyforms.ModelForm):
+        class Meta:
+            model = Note
+            fields = ('text',)
+            widgets = {
+                'text': get_inline_html_widget(),
+            }
+
+
+Let's assume that you've a ``form`` variable pointing on an instance of a NoteForm.
+In the template file, call the form and don't forget to put ``{{form.media}}`` in the headers.
+
+.. _settings:
+
+Settings
+------------------------------------
+
+The following constants can be set in your django project settings.py
+
+You can choose between 2 HTML editors : Aloha editor or CkEditor. We recommend to use CkEditor but keep Aloha by default
+for compatibility. Add one the 2 lines below in your settings.py
+
+In settings::
+
+    COOP_HTML_EDITOR = 'aloha'
+    COOP_HTML_EDITOR = 'ck-editor'
+
+You can tune your editor by changing the settings below. The values in this README correspond to defaults
+
+For both, we package a default version than can be overriden by copying your own version folder in ste static files
+and define the new version by
+
+In settings::
+
+    ALOHA_VERSION = "aloha.0.23.26"
+    CKEDITOR_VERSION = "ckeditor.4.6.2"
+
+The initialisation code of the editor is set in a javascript file. You can change the file to use by seetings
+
+In settings::
+
+    ALOHA_INIT_JS_TEMPLATE = "html_editor/aloha_init.js"
+    CKEDITOR_INIT_JS_TEMPLATE = "html_editor/ckeditor-init.js"
+
+If you choose CkEditor, you can add your own styles
+
+In settings::
+
+    CKEDITOR_CSS_CLASSES = [
+         "{name: 'Highlight', element: 'span', attributes: {'class': 'highlight'}}",
+         "{name: 'Red Title', element: 'h3', styles: {color: '#880000'}}",
+    ]
+
+
+InlineHtmlInput has a "provider" that allows you to add local links to your models (articles, contacts, whatever) easily, through an autocomplete field that will search for objects based on rules you defined for each model :
+
+* search this kind of models using get_absolute_url()
+* search this kind of models using another method
+* search this kind of models using a specified model field
+
+You can set the ``HTML_EDITOR_LINK_MODELS`` setting in your settings.py to tell which django models will be available in the auto-complete field of the "add link" widget like this ::
+
+    HTML_EDITOR_LINK_MODELS = ('coop_local.Article', 'calendar.Event', )
+    
+    
+djaloha requires jquery and is provided by default with jquery.1.7.2. You can change the jquery version if needed ::
+
+    HTML_EDITOR_JQUERY = 'js/jquery.1.7.2.js'
+    
+    
+Aloha has a nice plugin architecture. coop_html_editor includes by default the main Aloha plugins. You may want to have a different set of plugins.
+Please refer to the Aloha docs for more information on plugins ::
+
+    ALOHA_PLUGINS = (
+        "common/format",
+        "common/highlighteditables",
+        "common/list",
+        "common/link",
+        "common/undo",
+        "common/paste",
+        "common/commands",
+        "common/image",
+        "common/align",
+        "extra/attributes",
+        "common/characterpicker",
+        "common/abbr",
+        "common/horizontalruler",
+        "common/table",
+        "extra/browser",
+    )
+    
+
+Please note that the ``ALOHA_PLUGINS`` setting is a global setting. If you need to change the set of plugins for a specific form field, you
+can pass a similar tuple in the ``aloha_plugins`` attribute of your ``coop_html_editor`` widget.
+The ``extra_aloha_plugins`` attribute will add additional plugins to the default set.
+
+``HTML_EDITOR_INIT_URL`` setting make possible to overload the aloha init file of djaloha.
+``html_editor_init_url`` attribute of ``InlineHtmlInput`` can also be used to overload it for a specific form field.
+
+License
+=======
+
+coop_html_editor is based on apidev-djaloha is a fork from credis/djaloha (see http://github.com/credis/djaloha)
+
+coop_html_editor uses the BSD license. see license.txt
+
+Djaloha development was funded by `CREDIS <http://credis.org/>`_, FSE (European Social Fund) and Conseil Regional d'Auvergne.
```

### Comparing `coop_html_editor-1.3.1/coop_html_editor/templatetags/html_editor_utils.py` & `coop_html_editor-1.4.1/coop_html_editor/templatetags/html_editor_utils.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 # -*- coding: utf-8 -*-
 """template tags"""
 
 from django import template
+from django.apps import apps
 
 from ..forms import InlineHtmlForm
-from ..utils import get_model
 
 
 register = template.Library()
 
 
 @register.filter
 def convert_crlf(value):
@@ -144,15 +144,15 @@
 def get_html_editor_args(parser, token):
     """get templatetag args"""
     full_model_name = token.split_contents()[1]
     lookups = token.split_contents()[2].split(';')
     field_name = token.split_contents()[3]
 
     app_name, model_name = full_model_name.split('.')
-    model_class = get_model(app_name, model_name)
+    model_class = apps.get_model(app_name, model_name)
 
     lookup = {}
     for lookup_item in lookups:
         try:
             key, value = lookup_item.split('=')
         except ValueError:
             raise template.TemplateSyntaxError(
```

### Comparing `coop_html_editor-1.3.1/coop_html_editor/locale/fr/LC_MESSAGES/django.mo` & `coop_html_editor-1.4.1/coop_html_editor/locale/fr/LC_MESSAGES/django.mo`

 * *Files identical despite different names*

### Comparing `coop_html_editor-1.3.1/coop_html_editor/locale/fr/LC_MESSAGES/django.po` & `coop_html_editor-1.4.1/coop_html_editor/locale/fr/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `coop_html_editor-1.3.1/coop_html_editor/forms.py` & `coop_html_editor-1.4.1/coop_html_editor/forms.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 # -*- coding: utf-8 -*-
 """form base classes for integration"""
 
-from django.utils.encoding import smart_text
+from django.utils.encoding import smart_str
 
-import floppyforms.__future__ as forms
+import floppyforms as forms
 
 from .settings import get_field_prefix
 from .widgets import get_inline_html_widget
 
 
 class InlineHtmlForm(forms.Form):
     """Base class for form with inline html editor"""
@@ -37,15 +37,15 @@
         )
 
     def get_inline_html_widget(self):
         return get_inline_html_widget()
 
     def save(self):
         """save associated object"""
-        value = smart_text(self.cleaned_data[self._form_field])
+        value = smart_str(self.cleaned_data[self._form_field])
         obj = self._model_class.objects.get_or_create(**self._lookup)[0]
         setattr(obj, self._field_name, value)
         obj.save()
     
     def as_is(self):
         """return html without parent tag"""
         return self._html_output(
```

### Comparing `coop_html_editor-1.3.1/coop_html_editor/utils.py` & `coop_html_editor-1.4.1/coop_html_editor/utils.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,33 +1,26 @@
 # -*- coding: utf-8 -*-
 """utilities"""
 
-from django import VERSION
-
-if VERSION >= (1, 8, 0):
-    from django.apps import apps
-    get_model = apps.get_model
-else:
-    from django.db.models import get_model
-
+from django.apps import apps
 from .forms import InlineHtmlForm
 from .settings import get_field_prefix
 
 
 def extract_forms_args(data):
     """get the form arguments from POST data"""
     forms_args = []
     field_prefix = get_field_prefix()
     for field in data:
         if field.find(field_prefix) == 0:
             args = field.split("__")
             if len(args) > 4:
                 app_name = args[1]
                 model_name = args[2]
-                model_class = get_model(app_name, model_name)
+                model_class = apps.get_model(app_name, model_name)
                 field_name = args[-1]
                 lookup = {}
                 for (key, value) in zip(args[3:-1:2], args[4:-1:2]):
                     lookup[key] = value
                 forms_args.append((model_class, lookup, field_name))
     return forms_args
```

### Comparing `coop_html_editor-1.3.1/coop_html_editor/static/ckeditor.4.6.2/LICENSE.md` & `coop_html_editor-1.4.1/coop_html_editor/static/ckeditor.4.6.2/LICENSE.md`

 * *Files identical despite different names*

### Comparing `coop_html_editor-1.3.1/coop_html_editor/static/ckeditor.4.6.2/plugins/wsc/LICENSE.md` & `coop_html_editor-1.4.1/coop_html_editor/static/ckeditor.4.6.2/plugins/wsc/LICENSE.md`

 * *Files identical despite different names*

### Comparing `coop_html_editor-1.3.1/coop_html_editor/static/ckeditor.4.6.2/plugins/wsc/skins/moono-lisa/wsc.css` & `coop_html_editor-1.4.1/coop_html_editor/static/ckeditor.4.6.2/plugins/wsc/skins/moono-lisa/wsc.css`

 * *Files identical despite different names*

### Comparing `coop_html_editor-1.3.1/coop_html_editor/static/ckeditor.4.6.2/plugins/wsc/README.md` & `coop_html_editor-1.4.1/coop_html_editor/static/ckeditor.4.6.2/plugins/wsc/README.md`

 * *Files identical despite different names*

### Comparing `coop_html_editor-1.3.1/coop_html_editor/static/ckeditor.4.6.2/plugins/wsc/dialogs/wsc.css` & `coop_html_editor-1.4.1/coop_html_editor/static/ckeditor.4.6.2/plugins/wsc/dialogs/wsc.css`

 * *Files identical despite different names*

### Comparing `coop_html_editor-1.3.1/coop_html_editor/static/ckeditor.4.6.2/plugins/wsc/dialogs/tmpFrameset.html` & `coop_html_editor-1.4.1/coop_html_editor/static/ckeditor.4.6.2/plugins/wsc/dialogs/tmpFrameset.html`

 * *Files identical despite different names*

### Comparing `coop_html_editor-1.3.1/coop_html_editor/static/ckeditor.4.6.2/plugins/wsc/dialogs/ciframe.html` & `coop_html_editor-1.4.1/coop_html_editor/static/ckeditor.4.6.2/plugins/wsc/dialogs/ciframe.html`

 * *Files identical despite different names*

### Comparing `coop_html_editor-1.3.1/coop_html_editor/static/ckeditor.4.6.2/plugins/wsc/dialogs/wsc.js` & `coop_html_editor-1.4.1/coop_html_editor/static/ckeditor.4.6.2/plugins/wsc/dialogs/wsc.js`

 * *Files identical despite different names*

### Comparing `coop_html_editor-1.3.1/coop_html_editor/static/ckeditor.4.6.2/plugins/wsc/dialogs/wsc_ie.js` & `coop_html_editor-1.4.1/coop_html_editor/static/ckeditor.4.6.2/plugins/wsc/dialogs/wsc_ie.js`

 * *Files identical despite different names*

### Comparing `coop_html_editor-1.3.1/coop_html_editor/static/ckeditor.4.6.2/plugins/widget/dev/console.js` & `coop_html_editor-1.4.1/coop_html_editor/static/ckeditor.4.6.2/plugins/widget/dev/console.js`

 * *Files identical despite different names*

### Comparing `coop_html_editor-1.3.1/coop_html_editor/static/ckeditor.4.6.2/plugins/widget/dev/nestedwidgets.html` & `coop_html_editor-1.4.1/coop_html_editor/static/ckeditor.4.6.2/plugins/widget/dev/nestedwidgets.html`

 * *Files identical despite different names*

### Comparing `coop_html_editor-1.3.1/coop_html_editor/static/ckeditor.4.6.2/plugins/widget/dev/widgetstyles.html` & `coop_html_editor-1.4.1/coop_html_editor/static/ckeditor.4.6.2/plugins/widget/dev/widgetstyles.html`

 * *Files identical despite different names*

### Comparing `coop_html_editor-1.3.1/coop_html_editor/static/ckeditor.4.6.2/plugins/widget/dev/assets/simplebox/contents.css` & `coop_html_editor-1.4.1/coop_html_editor/static/ckeditor.4.6.2/plugins/widget/dev/assets/simplebox/contents.css`

 * *Files identical despite different names*

### Comparing `coop_html_editor-1.3.1/coop_html_editor/static/ckeditor.4.6.2/plugins/widget/dev/assets/simplebox/dialogs/simplebox.js` & `coop_html_editor-1.4.1/coop_html_editor/static/ckeditor.4.6.2/plugins/widget/dev/assets/simplebox/dialogs/simplebox.js`

 * *Files identical despite different names*

### Comparing `coop_html_editor-1.3.1/coop_html_editor/static/ckeditor.4.6.2/plugins/widget/dev/assets/simplebox/plugin.js` & `coop_html_editor-1.4.1/coop_html_editor/static/ckeditor.4.6.2/plugins/widget/dev/assets/simplebox/plugin.js`

 * *Files identical despite different names*

### Comparing `coop_html_editor-1.3.1/coop_html_editor/static/ckeditor.4.6.2/plugins/widget/dev/assets/sample.jpg` & `coop_html_editor-1.4.1/coop_html_editor/static/ckeditor.4.6.2/plugins/widget/dev/assets/sample.jpg`

 * *Files identical despite different names*

### Comparing `coop_html_editor-1.3.1/coop_html_editor/static/ckeditor.4.6.2/plugins/widget/plugin.js` & `coop_html_editor-1.4.1/coop_html_editor/static/ckeditor.4.6.2/plugins/widget/plugin.js`

 * *Files identical despite different names*

### Comparing `coop_html_editor-1.3.1/coop_html_editor/static/ckeditor.4.6.2/plugins/embed/plugin.js` & `coop_html_editor-1.4.1/coop_html_editor/static/ckeditor.4.6.2/plugins/embed/plugin.js`

 * *Files identical despite different names*

### Comparing `coop_html_editor-1.3.1/coop_html_editor/static/ckeditor.4.6.2/plugins/embedbase/lang/pt.js` & `coop_html_editor-1.4.1/coop_html_editor/static/ckeditor.4.6.2/plugins/embedbase/lang/pt.js`

 * *Files identical despite different names*

### Comparing `coop_html_editor-1.3.1/coop_html_editor/static/ckeditor.4.6.2/plugins/embedbase/lang/gl.js` & `coop_html_editor-1.4.1/coop_html_editor/static/ckeditor.4.6.2/plugins/embedbase/lang/gl.js`

 * *Files identical despite different names*

### Comparing `coop_html_editor-1.3.1/coop_html_editor/static/ckeditor.4.6.2/plugins/embedbase/lang/pl.js` & `coop_html_editor-1.4.1/coop_html_editor/static/ckeditor.4.6.2/plugins/embedbase/lang/pl.js`

 * *Files identical despite different names*

### Comparing `coop_html_editor-1.3.1/coop_html_editor/static/ckeditor.4.6.2/plugins/embedbase/lang/ko.js` & `coop_html_editor-1.4.1/coop_html_editor/static/ckeditor.4.6.2/plugins/embedbase/lang/ko.js`

 * *Files identical despite different names*

### Comparing `coop_html_editor-1.3.1/coop_html_editor/static/ckeditor.4.6.2/plugins/embedbase/lang/ru.js` & `coop_html_editor-1.4.1/coop_html_editor/static/ckeditor.4.6.2/plugins/embedbase/lang/ru.js`

 * *Files identical despite different names*

### Comparing `coop_html_editor-1.3.1/coop_html_editor/static/ckeditor.4.6.2/plugins/embedbase/lang/eu.js` & `coop_html_editor-1.4.1/coop_html_editor/static/ckeditor.4.6.2/plugins/embedbase/lang/eu.js`

 * *Files identical despite different names*

### Comparing `coop_html_editor-1.3.1/coop_html_editor/static/ckeditor.4.6.2/plugins/embedbase/lang/ja.js` & `coop_html_editor-1.4.1/coop_html_editor/static/ckeditor.4.6.2/plugins/embedbase/lang/ja.js`

 * *Files identical despite different names*

### Comparing `coop_html_editor-1.3.1/coop_html_editor/static/ckeditor.4.6.2/plugins/embedbase/lang/ug.js` & `coop_html_editor-1.4.1/coop_html_editor/static/ckeditor.4.6.2/plugins/embedbase/lang/ug.js`

 * *Files identical despite different names*

### Comparing `coop_html_editor-1.3.1/coop_html_editor/static/ckeditor.4.6.2/plugins/embedbase/lang/id.js` & `coop_html_editor-1.4.1/coop_html_editor/static/ckeditor.4.6.2/plugins/embedbase/lang/id.js`

 * *Files identical despite different names*

### Comparing `coop_html_editor-1.3.1/coop_html_editor/static/ckeditor.4.6.2/plugins/embedbase/lang/az.js` & `coop_html_editor-1.4.1/coop_html_editor/static/ckeditor.4.6.2/plugins/embedbase/lang/az.js`

 * *Files identical despite different names*

### Comparing `coop_html_editor-1.3.1/coop_html_editor/static/ckeditor.4.6.2/plugins/embedbase/lang/ca.js` & `coop_html_editor-1.4.1/coop_html_editor/static/ckeditor.4.6.2/plugins/embedbase/lang/ca.js`

 * *Files identical despite different names*

### Comparing `coop_html_editor-1.3.1/coop_html_editor/static/ckeditor.4.6.2/plugins/embedbase/lang/nb.js` & `coop_html_editor-1.4.1/coop_html_editor/static/ckeditor.4.6.2/plugins/embedbase/lang/nb.js`

 * *Files identical despite different names*

### Comparing `coop_html_editor-1.3.1/coop_html_editor/static/ckeditor.4.6.2/plugins/embedbase/lang/zh-cn.js` & `coop_html_editor-1.4.1/coop_html_editor/static/ckeditor.4.6.2/plugins/embedbase/lang/zh-cn.js`

 * *Files identical despite different names*

### Comparing `coop_html_editor-1.3.1/coop_html_editor/static/ckeditor.4.6.2/plugins/embedbase/lang/de-ch.js` & `coop_html_editor-1.4.1/coop_html_editor/static/ckeditor.4.6.2/plugins/embedbase/lang/de-ch.js`

 * *Files identical despite different names*

### Comparing `coop_html_editor-1.3.1/coop_html_editor/static/ckeditor.4.6.2/plugins/embedbase/lang/pt-br.js` & `coop_html_editor-1.4.1/coop_html_editor/static/ckeditor.4.6.2/plugins/embedbase/lang/pt-br.js`

 * *Files identical despite different names*

### Comparing `coop_html_editor-1.3.1/coop_html_editor/static/ckeditor.4.6.2/plugins/embedbase/lang/oc.js` & `coop_html_editor-1.4.1/coop_html_editor/static/ckeditor.4.6.2/plugins/embedbase/lang/oc.js`

 * *Files identical despite different names*

### Comparing `coop_html_editor-1.3.1/coop_html_editor/static/ckeditor.4.6.2/plugins/embedbase/lang/da.js` & `coop_html_editor-1.4.1/coop_html_editor/static/ckeditor.4.6.2/plugins/embedbase/lang/da.js`

 * *Files identical despite different names*

### Comparing `coop_html_editor-1.3.1/coop_html_editor/static/ckeditor.4.6.2/plugins/embedbase/lang/de.js` & `coop_html_editor-1.4.1/coop_html_editor/static/ckeditor.4.6.2/plugins/embedbase/lang/de.js`

 * *Files identical despite different names*

### Comparing `coop_html_editor-1.3.1/coop_html_editor/static/ckeditor.4.6.2/plugins/embedbase/lang/en.js` & `coop_html_editor-1.4.1/coop_html_editor/static/ckeditor.4.6.2/plugins/embedbase/lang/en.js`

 * *Files identical despite different names*

### Comparing `coop_html_editor-1.3.1/coop_html_editor/static/ckeditor.4.6.2/plugins/embedbase/lang/ku.js` & `coop_html_editor-1.4.1/coop_html_editor/static/ckeditor.4.6.2/plugins/embedbase/lang/ku.js`

 * *Files identical despite different names*

### Comparing `coop_html_editor-1.3.1/coop_html_editor/static/ckeditor.4.6.2/plugins/embedbase/lang/sv.js` & `coop_html_editor-1.4.1/coop_html_editor/static/ckeditor.4.6.2/plugins/embedbase/lang/sv.js`

 * *Files identical despite different names*

### Comparing `coop_html_editor-1.3.1/coop_html_editor/static/ckeditor.4.6.2/plugins/embedbase/lang/zh.js` & `coop_html_editor-1.4.1/coop_html_editor/static/ckeditor.4.6.2/plugins/embedbase/lang/zh.js`

 * *Files identical despite different names*

### Comparing `coop_html_editor-1.3.1/coop_html_editor/static/ckeditor.4.6.2/plugins/embedbase/lang/uk.js` & `coop_html_editor-1.4.1/coop_html_editor/static/ckeditor.4.6.2/plugins/embedbase/lang/uk.js`

 * *Files identical despite different names*

### Comparing `coop_html_editor-1.3.1/coop_html_editor/static/ckeditor.4.6.2/plugins/embedbase/lang/cs.js` & `coop_html_editor-1.4.1/coop_html_editor/static/ckeditor.4.6.2/plugins/embedbase/lang/cs.js`

 * *Files identical despite different names*

### Comparing `coop_html_editor-1.3.1/coop_html_editor/static/ckeditor.4.6.2/plugins/embedbase/lang/fr.js` & `coop_html_editor-1.4.1/coop_html_editor/static/ckeditor.4.6.2/plugins/embedbase/lang/fr.js`

 * *Files identical despite different names*

### Comparing `coop_html_editor-1.3.1/coop_html_editor/static/ckeditor.4.6.2/plugins/embedbase/lang/nl.js` & `coop_html_editor-1.4.1/coop_html_editor/static/ckeditor.4.6.2/plugins/embedbase/lang/nl.js`

 * *Files identical despite different names*

### Comparing `coop_html_editor-1.3.1/coop_html_editor/static/ckeditor.4.6.2/plugins/embedbase/lang/it.js` & `coop_html_editor-1.4.1/coop_html_editor/static/ckeditor.4.6.2/plugins/embedbase/lang/it.js`

 * *Files identical despite different names*

### Comparing `coop_html_editor-1.3.1/coop_html_editor/static/ckeditor.4.6.2/plugins/embedbase/lang/es.js` & `coop_html_editor-1.4.1/coop_html_editor/static/ckeditor.4.6.2/plugins/embedbase/lang/es.js`

 * *Files identical despite different names*

### Comparing `coop_html_editor-1.3.1/coop_html_editor/static/ckeditor.4.6.2/plugins/embedbase/lang/eo.js` & `coop_html_editor-1.4.1/coop_html_editor/static/ckeditor.4.6.2/plugins/embedbase/lang/eo.js`

 * *Files identical despite different names*

### Comparing `coop_html_editor-1.3.1/coop_html_editor/static/ckeditor.4.6.2/plugins/embedbase/lang/tr.js` & `coop_html_editor-1.4.1/coop_html_editor/static/ckeditor.4.6.2/plugins/embedbase/lang/tr.js`

 * *Files identical despite different names*

### Comparing `coop_html_editor-1.3.1/coop_html_editor/static/ckeditor.4.6.2/plugins/embedbase/dialogs/embedbase.js` & `coop_html_editor-1.4.1/coop_html_editor/static/ckeditor.4.6.2/plugins/embedbase/dialogs/embedbase.js`

 * *Files identical despite different names*

### Comparing `coop_html_editor-1.3.1/coop_html_editor/static/ckeditor.4.6.2/plugins/embedbase/plugin.js` & `coop_html_editor-1.4.1/coop_html_editor/static/ckeditor.4.6.2/plugins/embedbase/plugin.js`

 * *Files identical despite different names*

### Comparing `coop_html_editor-1.3.1/coop_html_editor/static/ckeditor.4.6.2/plugins/notification/plugin.js` & `coop_html_editor-1.4.1/coop_html_editor/static/ckeditor.4.6.2/plugins/notification/plugin.js`

 * *Files identical despite different names*

### Comparing `coop_html_editor-1.3.1/coop_html_editor/static/ckeditor.4.6.2/plugins/tabletools/dialogs/tableCell.js` & `coop_html_editor-1.4.1/coop_html_editor/static/ckeditor.4.6.2/plugins/tabletools/dialogs/tableCell.js`

 * *Files identical despite different names*

### Comparing `coop_html_editor-1.3.1/coop_html_editor/static/ckeditor.4.6.2/plugins/pastefromword/filter/default.js` & `coop_html_editor-1.4.1/coop_html_editor/static/ckeditor.4.6.2/plugins/pastefromword/filter/default.js`

 * *Files identical despite different names*

### Comparing `coop_html_editor-1.3.1/coop_html_editor/static/ckeditor.4.6.2/plugins/toolbar/lang/sr-latn.js` & `coop_html_editor-1.4.1/coop_html_editor/static/ckeditor.4.6.2/plugins/toolbar/lang/sr-latn.js`

 * *Files identical despite different names*

### Comparing `coop_html_editor-1.3.1/coop_html_editor/static/ckeditor.4.6.2/plugins/toolbar/lang/pt.js` & `coop_html_editor-1.4.1/coop_html_editor/static/ckeditor.4.6.2/plugins/toolbar/lang/pt.js`

 * *Files identical despite different names*

### Comparing `coop_html_editor-1.3.1/coop_html_editor/static/ckeditor.4.6.2/plugins/toolbar/lang/vi.js` & `coop_html_editor-1.4.1/coop_html_editor/static/ckeditor.4.6.2/plugins/toolbar/lang/vi.js`

 * *Files identical despite different names*

### Comparing `coop_html_editor-1.3.1/coop_html_editor/static/ckeditor.4.6.2/plugins/toolbar/lang/lv.js` & `coop_html_editor-1.4.1/coop_html_editor/static/ckeditor.4.6.2/plugins/toolbar/lang/lv.js`

 * *Files identical despite different names*

### Comparing `coop_html_editor-1.3.1/coop_html_editor/static/ckeditor.4.6.2/plugins/toolbar/lang/gl.js` & `coop_html_editor-1.4.1/coop_html_editor/static/ckeditor.4.6.2/plugins/toolbar/lang/gl.js`

 * *Files identical despite different names*

### Comparing `coop_html_editor-1.3.1/coop_html_editor/static/ckeditor.4.6.2/plugins/toolbar/lang/pl.js` & `coop_html_editor-1.4.1/coop_html_editor/static/ckeditor.4.6.2/plugins/toolbar/lang/pl.js`

 * *Files identical despite different names*

### Comparing `coop_html_editor-1.3.1/coop_html_editor/static/ckeditor.4.6.2/plugins/toolbar/lang/mn.js` & `coop_html_editor-1.4.1/coop_html_editor/static/ckeditor.4.6.2/plugins/toolbar/lang/mn.js`

 * *Files identical despite different names*

### Comparing `coop_html_editor-1.3.1/coop_html_editor/static/ckeditor.4.6.2/plugins/toolbar/lang/en-ca.js` & `coop_html_editor-1.4.1/coop_html_editor/static/ckeditor.4.6.2/plugins/toolbar/lang/en-ca.js`

 * *Files identical despite different names*

### Comparing `coop_html_editor-1.3.1/coop_html_editor/static/ckeditor.4.6.2/plugins/toolbar/lang/el.js` & `coop_html_editor-1.4.1/coop_html_editor/static/ckeditor.4.6.2/plugins/toolbar/lang/el.js`

 * *Files identical despite different names*

### Comparing `coop_html_editor-1.3.1/coop_html_editor/static/ckeditor.4.6.2/plugins/toolbar/lang/et.js` & `coop_html_editor-1.4.1/coop_html_editor/static/ckeditor.4.6.2/plugins/toolbar/lang/et.js`

 * *Files identical despite different names*

### Comparing `coop_html_editor-1.3.1/coop_html_editor/static/ckeditor.4.6.2/plugins/toolbar/lang/is.js` & `coop_html_editor-1.4.1/coop_html_editor/static/ckeditor.4.6.2/plugins/toolbar/lang/is.js`

 * *Files identical despite different names*

### Comparing `coop_html_editor-1.3.1/coop_html_editor/static/ckeditor.4.6.2/plugins/toolbar/lang/sl.js` & `coop_html_editor-1.4.1/coop_html_editor/static/ckeditor.4.6.2/plugins/toolbar/lang/sl.js`

 * *Files identical despite different names*

### Comparing `coop_html_editor-1.3.1/coop_html_editor/static/ckeditor.4.6.2/plugins/toolbar/lang/ko.js` & `coop_html_editor-1.4.1/coop_html_editor/static/ckeditor.4.6.2/plugins/toolbar/lang/ko.js`

 * *Files identical despite different names*

### Comparing `coop_html_editor-1.3.1/coop_html_editor/static/ckeditor.4.6.2/plugins/toolbar/lang/hr.js` & `coop_html_editor-1.4.1/coop_html_editor/static/ckeditor.4.6.2/plugins/toolbar/lang/hr.js`

 * *Files identical despite different names*

### Comparing `coop_html_editor-1.3.1/coop_html_editor/static/ckeditor.4.6.2/plugins/toolbar/lang/ms.js` & `coop_html_editor-1.4.1/coop_html_editor/static/ckeditor.4.6.2/plugins/toolbar/lang/ms.js`

 * *Files identical despite different names*

### Comparing `coop_html_editor-1.3.1/coop_html_editor/static/ckeditor.4.6.2/plugins/toolbar/lang/fi.js` & `coop_html_editor-1.4.1/coop_html_editor/static/ckeditor.4.6.2/plugins/toolbar/lang/fi.js`

 * *Files identical despite different names*

### Comparing `coop_html_editor-1.3.1/coop_html_editor/static/ckeditor.4.6.2/plugins/toolbar/lang/th.js` & `coop_html_editor-1.4.1/coop_html_editor/static/ckeditor.4.6.2/plugins/toolbar/lang/th.js`

 * *Files identical despite different names*

### Comparing `coop_html_editor-1.3.1/coop_html_editor/static/ckeditor.4.6.2/plugins/toolbar/lang/ru.js` & `coop_html_editor-1.4.1/coop_html_editor/static/ckeditor.4.6.2/plugins/toolbar/lang/ru.js`

 * *Files identical despite different names*

### Comparing `coop_html_editor-1.3.1/coop_html_editor/static/ckeditor.4.6.2/plugins/toolbar/lang/eu.js` & `coop_html_editor-1.4.1/coop_html_editor/static/ckeditor.4.6.2/plugins/toolbar/lang/eu.js`

 * *Files identical despite different names*

### Comparing `coop_html_editor-1.3.1/coop_html_editor/static/ckeditor.4.6.2/plugins/toolbar/lang/mk.js` & `coop_html_editor-1.4.1/coop_html_editor/static/ckeditor.4.6.2/plugins/toolbar/lang/mk.js`

 * *Files identical despite different names*

### Comparing `coop_html_editor-1.3.1/coop_html_editor/static/ckeditor.4.6.2/plugins/toolbar/lang/no.js` & `coop_html_editor-1.4.1/coop_html_editor/static/ckeditor.4.6.2/plugins/toolbar/lang/no.js`

 * *Files identical despite different names*

### Comparing `coop_html_editor-1.3.1/coop_html_editor/static/ckeditor.4.6.2/plugins/toolbar/lang/sq.js` & `coop_html_editor-1.4.1/coop_html_editor/static/ckeditor.4.6.2/plugins/toolbar/lang/sq.js`

 * *Files identical despite different names*

### Comparing `coop_html_editor-1.3.1/coop_html_editor/static/ckeditor.4.6.2/plugins/toolbar/lang/gu.js` & `coop_html_editor-1.4.1/coop_html_editor/static/ckeditor.4.6.2/plugins/toolbar/lang/gu.js`

 * *Files identical despite different names*

### Comparing `coop_html_editor-1.3.1/coop_html_editor/static/ckeditor.4.6.2/plugins/toolbar/lang/si.js` & `coop_html_editor-1.4.1/coop_html_editor/static/ckeditor.4.6.2/plugins/toolbar/lang/si.js`

 * *Files identical despite different names*

### Comparing `coop_html_editor-1.3.1/coop_html_editor/static/ckeditor.4.6.2/plugins/toolbar/lang/tt.js` & `coop_html_editor-1.4.1/coop_html_editor/static/ckeditor.4.6.2/plugins/toolbar/lang/tt.js`

 * *Files identical despite different names*

### Comparing `coop_html_editor-1.3.1/coop_html_editor/static/ckeditor.4.6.2/plugins/toolbar/lang/ja.js` & `coop_html_editor-1.4.1/coop_html_editor/static/ckeditor.4.6.2/plugins/toolbar/lang/ja.js`

 * *Files identical despite different names*

### Comparing `coop_html_editor-1.3.1/coop_html_editor/static/ckeditor.4.6.2/plugins/toolbar/lang/ka.js` & `coop_html_editor-1.4.1/coop_html_editor/static/ckeditor.4.6.2/plugins/toolbar/lang/ka.js`

 * *Files identical despite different names*

### Comparing `coop_html_editor-1.3.1/coop_html_editor/static/ckeditor.4.6.2/plugins/toolbar/lang/he.js` & `coop_html_editor-1.4.1/coop_html_editor/static/ckeditor.4.6.2/plugins/toolbar/lang/he.js`

 * *Files identical despite different names*

### Comparing `coop_html_editor-1.3.1/coop_html_editor/static/ckeditor.4.6.2/plugins/toolbar/lang/ug.js` & `coop_html_editor-1.4.1/coop_html_editor/static/ckeditor.4.6.2/plugins/toolbar/lang/ug.js`

 * *Files identical despite different names*

### Comparing `coop_html_editor-1.3.1/coop_html_editor/static/ckeditor.4.6.2/plugins/toolbar/lang/bg.js` & `coop_html_editor-1.4.1/coop_html_editor/static/ckeditor.4.6.2/plugins/toolbar/lang/bg.js`

 * *Files identical despite different names*

### Comparing `coop_html_editor-1.3.1/coop_html_editor/static/ckeditor.4.6.2/plugins/toolbar/lang/af.js` & `coop_html_editor-1.4.1/coop_html_editor/static/ckeditor.4.6.2/plugins/toolbar/lang/af.js`

 * *Files identical despite different names*

### Comparing `coop_html_editor-1.3.1/coop_html_editor/static/ckeditor.4.6.2/plugins/toolbar/lang/id.js` & `coop_html_editor-1.4.1/coop_html_editor/static/ckeditor.4.6.2/plugins/toolbar/lang/id.js`

 * *Files identical despite different names*

### Comparing `coop_html_editor-1.3.1/coop_html_editor/static/ckeditor.4.6.2/plugins/toolbar/lang/az.js` & `coop_html_editor-1.4.1/coop_html_editor/static/ckeditor.4.6.2/plugins/toolbar/lang/az.js`

 * *Files identical despite different names*

### Comparing `coop_html_editor-1.3.1/coop_html_editor/static/ckeditor.4.6.2/plugins/toolbar/lang/en-au.js` & `coop_html_editor-1.4.1/coop_html_editor/static/ckeditor.4.6.2/plugins/toolbar/lang/en-au.js`

 * *Files identical despite different names*

### Comparing `coop_html_editor-1.3.1/coop_html_editor/static/ckeditor.4.6.2/plugins/toolbar/lang/ca.js` & `coop_html_editor-1.4.1/coop_html_editor/static/ckeditor.4.6.2/plugins/toolbar/lang/ca.js`

 * *Files identical despite different names*

### Comparing `coop_html_editor-1.3.1/coop_html_editor/static/ckeditor.4.6.2/plugins/toolbar/lang/cy.js` & `coop_html_editor-1.4.1/coop_html_editor/static/ckeditor.4.6.2/plugins/toolbar/lang/cy.js`

 * *Files identical despite different names*

### Comparing `coop_html_editor-1.3.1/coop_html_editor/static/ckeditor.4.6.2/plugins/toolbar/lang/nb.js` & `coop_html_editor-1.4.1/coop_html_editor/static/ckeditor.4.6.2/plugins/toolbar/lang/nb.js`

 * *Files identical despite different names*

### Comparing `coop_html_editor-1.3.1/coop_html_editor/static/ckeditor.4.6.2/plugins/toolbar/lang/zh-cn.js` & `coop_html_editor-1.4.1/coop_html_editor/static/ckeditor.4.6.2/plugins/toolbar/lang/zh-cn.js`

 * *Files identical despite different names*

### Comparing `coop_html_editor-1.3.1/coop_html_editor/static/ckeditor.4.6.2/plugins/toolbar/lang/de-ch.js` & `coop_html_editor-1.4.1/coop_html_editor/static/ckeditor.4.6.2/plugins/toolbar/lang/de-ch.js`

 * *Files identical despite different names*

### Comparing `coop_html_editor-1.3.1/coop_html_editor/static/ckeditor.4.6.2/plugins/toolbar/lang/pt-br.js` & `coop_html_editor-1.4.1/coop_html_editor/static/ckeditor.4.6.2/plugins/toolbar/lang/pt-br.js`

 * *Files identical despite different names*

### Comparing `coop_html_editor-1.3.1/coop_html_editor/static/ckeditor.4.6.2/plugins/toolbar/lang/oc.js` & `coop_html_editor-1.4.1/coop_html_editor/static/ckeditor.4.6.2/plugins/toolbar/lang/oc.js`

 * *Files identical despite different names*

### Comparing `coop_html_editor-1.3.1/coop_html_editor/static/ckeditor.4.6.2/plugins/toolbar/lang/da.js` & `coop_html_editor-1.4.1/coop_html_editor/static/ckeditor.4.6.2/plugins/toolbar/lang/da.js`

 * *Files identical despite different names*

### Comparing `coop_html_editor-1.3.1/coop_html_editor/static/ckeditor.4.6.2/plugins/toolbar/lang/fa.js` & `coop_html_editor-1.4.1/coop_html_editor/static/ckeditor.4.6.2/plugins/toolbar/lang/fa.js`

 * *Files identical despite different names*

### Comparing `coop_html_editor-1.3.1/coop_html_editor/static/ckeditor.4.6.2/plugins/toolbar/lang/de.js` & `coop_html_editor-1.4.1/coop_html_editor/static/ckeditor.4.6.2/plugins/toolbar/lang/de.js`

 * *Files identical despite different names*

### Comparing `coop_html_editor-1.3.1/coop_html_editor/static/ckeditor.4.6.2/plugins/toolbar/lang/en.js` & `coop_html_editor-1.4.1/coop_html_editor/static/ckeditor.4.6.2/plugins/toolbar/lang/en.js`

 * *Files identical despite different names*

### Comparing `coop_html_editor-1.3.1/coop_html_editor/static/ckeditor.4.6.2/plugins/toolbar/lang/bs.js` & `coop_html_editor-1.4.1/coop_html_editor/static/ckeditor.4.6.2/plugins/toolbar/lang/bs.js`

 * *Files identical despite different names*

### Comparing `coop_html_editor-1.3.1/coop_html_editor/static/ckeditor.4.6.2/plugins/toolbar/lang/ku.js` & `coop_html_editor-1.4.1/coop_html_editor/static/ckeditor.4.6.2/plugins/toolbar/lang/ku.js`

 * *Files identical despite different names*

### Comparing `coop_html_editor-1.3.1/coop_html_editor/static/ckeditor.4.6.2/plugins/toolbar/lang/sv.js` & `coop_html_editor-1.4.1/coop_html_editor/static/ckeditor.4.6.2/plugins/toolbar/lang/sv.js`

 * *Files identical despite different names*

### Comparing `coop_html_editor-1.3.1/coop_html_editor/static/ckeditor.4.6.2/plugins/toolbar/lang/zh.js` & `coop_html_editor-1.4.1/coop_html_editor/static/ckeditor.4.6.2/plugins/toolbar/lang/zh.js`

 * *Files identical despite different names*

### Comparing `coop_html_editor-1.3.1/coop_html_editor/static/ckeditor.4.6.2/plugins/toolbar/lang/hi.js` & `coop_html_editor-1.4.1/coop_html_editor/static/ckeditor.4.6.2/plugins/toolbar/lang/hi.js`

 * *Files identical despite different names*

### Comparing `coop_html_editor-1.3.1/coop_html_editor/static/ckeditor.4.6.2/plugins/toolbar/lang/uk.js` & `coop_html_editor-1.4.1/coop_html_editor/static/ckeditor.4.6.2/plugins/toolbar/lang/uk.js`

 * *Files identical despite different names*

### Comparing `coop_html_editor-1.3.1/coop_html_editor/static/ckeditor.4.6.2/plugins/toolbar/lang/cs.js` & `coop_html_editor-1.4.1/coop_html_editor/static/ckeditor.4.6.2/plugins/toolbar/lang/cs.js`

 * *Files identical despite different names*

### Comparing `coop_html_editor-1.3.1/coop_html_editor/static/ckeditor.4.6.2/plugins/toolbar/lang/km.js` & `coop_html_editor-1.4.1/coop_html_editor/static/ckeditor.4.6.2/plugins/toolbar/lang/km.js`

 * *Files identical despite different names*

### Comparing `coop_html_editor-1.3.1/coop_html_editor/static/ckeditor.4.6.2/plugins/toolbar/lang/fr.js` & `coop_html_editor-1.4.1/coop_html_editor/static/ckeditor.4.6.2/plugins/toolbar/lang/fr.js`

 * *Files identical despite different names*

### Comparing `coop_html_editor-1.3.1/coop_html_editor/static/ckeditor.4.6.2/plugins/toolbar/lang/nl.js` & `coop_html_editor-1.4.1/coop_html_editor/static/ckeditor.4.6.2/plugins/toolbar/lang/nl.js`

 * *Files identical despite different names*

### Comparing `coop_html_editor-1.3.1/coop_html_editor/static/ckeditor.4.6.2/plugins/toolbar/lang/fr-ca.js` & `coop_html_editor-1.4.1/coop_html_editor/static/ckeditor.4.6.2/plugins/toolbar/lang/fr-ca.js`

 * *Files identical despite different names*

### Comparing `coop_html_editor-1.3.1/coop_html_editor/static/ckeditor.4.6.2/plugins/toolbar/lang/en-gb.js` & `coop_html_editor-1.4.1/coop_html_editor/static/ckeditor.4.6.2/plugins/toolbar/lang/en-gb.js`

 * *Files identical despite different names*

### Comparing `coop_html_editor-1.3.1/coop_html_editor/static/ckeditor.4.6.2/plugins/toolbar/lang/sr.js` & `coop_html_editor-1.4.1/coop_html_editor/static/ckeditor.4.6.2/plugins/toolbar/lang/sr.js`

 * *Files identical despite different names*

### Comparing `coop_html_editor-1.3.1/coop_html_editor/static/ckeditor.4.6.2/plugins/toolbar/lang/hu.js` & `coop_html_editor-1.4.1/coop_html_editor/static/ckeditor.4.6.2/plugins/toolbar/lang/hu.js`

 * *Files identical despite different names*

### Comparing `coop_html_editor-1.3.1/coop_html_editor/static/ckeditor.4.6.2/plugins/toolbar/lang/lt.js` & `coop_html_editor-1.4.1/coop_html_editor/static/ckeditor.4.6.2/plugins/toolbar/lang/lt.js`

 * *Files identical despite different names*

### Comparing `coop_html_editor-1.3.1/coop_html_editor/static/ckeditor.4.6.2/plugins/toolbar/lang/fo.js` & `coop_html_editor-1.4.1/coop_html_editor/static/ckeditor.4.6.2/plugins/toolbar/lang/fo.js`

 * *Files identical despite different names*

### Comparing `coop_html_editor-1.3.1/coop_html_editor/static/ckeditor.4.6.2/plugins/toolbar/lang/ar.js` & `coop_html_editor-1.4.1/coop_html_editor/static/ckeditor.4.6.2/plugins/toolbar/lang/ar.js`

 * *Files identical despite different names*

### Comparing `coop_html_editor-1.3.1/coop_html_editor/static/ckeditor.4.6.2/plugins/toolbar/lang/sk.js` & `coop_html_editor-1.4.1/coop_html_editor/static/ckeditor.4.6.2/plugins/toolbar/lang/sk.js`

 * *Files identical despite different names*

### Comparing `coop_html_editor-1.3.1/coop_html_editor/static/ckeditor.4.6.2/plugins/toolbar/lang/it.js` & `coop_html_editor-1.4.1/coop_html_editor/static/ckeditor.4.6.2/plugins/toolbar/lang/it.js`

 * *Files identical despite different names*

### Comparing `coop_html_editor-1.3.1/coop_html_editor/static/ckeditor.4.6.2/plugins/toolbar/lang/es.js` & `coop_html_editor-1.4.1/coop_html_editor/static/ckeditor.4.6.2/plugins/toolbar/lang/es.js`

 * *Files identical despite different names*

### Comparing `coop_html_editor-1.3.1/coop_html_editor/static/ckeditor.4.6.2/plugins/toolbar/lang/bn.js` & `coop_html_editor-1.4.1/coop_html_editor/static/ckeditor.4.6.2/plugins/toolbar/lang/bn.js`

 * *Files identical despite different names*

### Comparing `coop_html_editor-1.3.1/coop_html_editor/static/ckeditor.4.6.2/plugins/toolbar/lang/eo.js` & `coop_html_editor-1.4.1/coop_html_editor/static/ckeditor.4.6.2/plugins/toolbar/lang/eo.js`

 * *Files identical despite different names*

### Comparing `coop_html_editor-1.3.1/coop_html_editor/static/ckeditor.4.6.2/plugins/toolbar/lang/ro.js` & `coop_html_editor-1.4.1/coop_html_editor/static/ckeditor.4.6.2/plugins/toolbar/lang/ro.js`

 * *Files identical despite different names*

### Comparing `coop_html_editor-1.3.1/coop_html_editor/static/ckeditor.4.6.2/plugins/toolbar/lang/tr.js` & `coop_html_editor-1.4.1/coop_html_editor/static/ckeditor.4.6.2/plugins/toolbar/lang/tr.js`

 * *Files identical despite different names*

### Comparing `coop_html_editor-1.3.1/coop_html_editor/static/ckeditor.4.6.2/plugins/toolbar/samples/toolbar.html` & `coop_html_editor-1.4.1/coop_html_editor/static/ckeditor.4.6.2/plugins/toolbar/samples/toolbar.html`

 * *Files identical despite different names*

### Comparing `coop_html_editor-1.3.1/coop_html_editor/static/ckeditor.4.6.2/plugins/toolbar/plugin.js` & `coop_html_editor-1.4.1/coop_html_editor/static/ckeditor.4.6.2/plugins/toolbar/plugin.js`

 * *Files identical despite different names*

### Comparing `coop_html_editor-1.3.1/coop_html_editor/static/ckeditor.4.6.2/plugins/btgrid/bower.json` & `coop_html_editor-1.4.1/coop_html_editor/static/ckeditor.4.6.2/plugins/btgrid/bower.json`

 * *Files identical despite different names*

### Comparing `coop_html_editor-1.3.1/coop_html_editor/static/ckeditor.4.6.2/plugins/btgrid/README.md` & `coop_html_editor-1.4.1/coop_html_editor/static/ckeditor.4.6.2/plugins/btgrid/README.md`

 * *Files identical despite different names*

### Comparing `coop_html_editor-1.3.1/coop_html_editor/static/ckeditor.4.6.2/plugins/btgrid/lang/ru.js` & `coop_html_editor-1.4.1/coop_html_editor/static/ckeditor.4.6.2/plugins/btgrid/lang/ru.js`

 * *Files identical despite different names*

### Comparing `coop_html_editor-1.3.1/coop_html_editor/static/ckeditor.4.6.2/plugins/btgrid/styles/editor.css` & `coop_html_editor-1.4.1/coop_html_editor/static/ckeditor.4.6.2/plugins/btgrid/styles/editor.css`

 * *Files identical despite different names*

### Comparing `coop_html_editor-1.3.1/coop_html_editor/static/ckeditor.4.6.2/plugins/btgrid/dialogs/btgrid.js` & `coop_html_editor-1.4.1/coop_html_editor/static/ckeditor.4.6.2/plugins/btgrid/dialogs/btgrid.js`

 * *Files identical despite different names*

### Comparing `coop_html_editor-1.3.1/coop_html_editor/static/ckeditor.4.6.2/plugins/btgrid/LICENSE.txt` & `coop_html_editor-1.4.1/coop_html_editor/static/ckeditor.4.6.2/plugins/btgrid/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `coop_html_editor-1.3.1/coop_html_editor/static/ckeditor.4.6.2/plugins/btgrid/plugin.js` & `coop_html_editor-1.4.1/coop_html_editor/static/ckeditor.4.6.2/plugins/btgrid/plugin.js`

 * *Files 2% similar despite different names*

#### js-beautify {}

```diff
@@ -3,15 +3,14 @@
         lang: 'en,ru,fr,nl',
         requires: 'widget,dialog',
         icons: 'btgrid',
         init: function(editor) {
             var maxGridColumns = 12;
             var lang = editor.lang.btgrid;
 
-            console.log('>btgrid');
             CKEDITOR.dialog.add('btgrid', this.path + 'dialogs/btgrid.js');
 
             editor.addContentsCss(this.path + 'styles/editor.css');
             // Add widget
             editor.ui.addButton('btgrid', {
                 label: lang.createBtGrid,
                 command: 'btgrid',
```

### Comparing `coop_html_editor-1.3.1/coop_html_editor/static/ckeditor.4.6.2/plugins/about/dialogs/about.js` & `coop_html_editor-1.4.1/coop_html_editor/static/ckeditor.4.6.2/plugins/about/dialogs/about.js`

 * *Files identical despite different names*

### Comparing `coop_html_editor-1.3.1/coop_html_editor/static/ckeditor.4.6.2/plugins/about/dialogs/hidpi/logo_ckeditor.png` & `coop_html_editor-1.4.1/coop_html_editor/static/ckeditor.4.6.2/plugins/about/dialogs/hidpi/logo_ckeditor.png`

 * *Files identical despite different names*

### Comparing `coop_html_editor-1.3.1/coop_html_editor/static/ckeditor.4.6.2/plugins/about/dialogs/logo_ckeditor.png` & `coop_html_editor-1.4.1/coop_html_editor/static/ckeditor.4.6.2/plugins/about/dialogs/logo_ckeditor.png`

 * *Files identical despite different names*

### Comparing `coop_html_editor-1.3.1/coop_html_editor/static/ckeditor.4.6.2/plugins/videoembed/dialogs/videoembedDialog.js` & `coop_html_editor-1.4.1/coop_html_editor/static/ckeditor.4.6.2/plugins/videoembed/dialogs/videoembedDialog.js`

 * *Files identical despite different names*

### Comparing `coop_html_editor-1.3.1/coop_html_editor/static/ckeditor.4.6.2/plugins/videoembed/plugin.js` & `coop_html_editor-1.4.1/coop_html_editor/static/ckeditor.4.6.2/plugins/videoembed/plugin.js`

 * *Files identical despite different names*

### Comparing `coop_html_editor-1.3.1/coop_html_editor/static/ckeditor.4.6.2/plugins/image/images/noimage.png` & `coop_html_editor-1.4.1/coop_html_editor/static/ckeditor.4.6.2/plugins/image/images/noimage.png`

 * *Files identical despite different names*

### Comparing `coop_html_editor-1.3.1/coop_html_editor/static/ckeditor.4.6.2/plugins/image/dialogs/image.js` & `coop_html_editor-1.4.1/coop_html_editor/static/ckeditor.4.6.2/plugins/image/dialogs/image.js`

 * *Files identical despite different names*

### Comparing `coop_html_editor-1.3.1/coop_html_editor/static/ckeditor.4.6.2/plugins/button/plugin.js` & `coop_html_editor-1.4.1/coop_html_editor/static/ckeditor.4.6.2/plugins/button/plugin.js`

 * *Files identical despite different names*

### Comparing `coop_html_editor-1.3.1/coop_html_editor/static/ckeditor.4.6.2/plugins/icons.png` & `coop_html_editor-1.4.1/coop_html_editor/static/ckeditor.4.6.2/plugins/icons.png`

 * *Files identical despite different names*

### Comparing `coop_html_editor-1.3.1/coop_html_editor/static/ckeditor.4.6.2/plugins/lineutils/dev/magicfinger.html` & `coop_html_editor-1.4.1/coop_html_editor/static/ckeditor.4.6.2/plugins/lineutils/dev/magicfinger.html`

 * *Files identical despite different names*

### Comparing `coop_html_editor-1.3.1/coop_html_editor/static/ckeditor.4.6.2/plugins/lineutils/dev/dnd.html` & `coop_html_editor-1.4.1/coop_html_editor/static/ckeditor.4.6.2/plugins/lineutils/dev/dnd.html`

 * *Files identical despite different names*

### Comparing `coop_html_editor-1.3.1/coop_html_editor/static/ckeditor.4.6.2/plugins/lineutils/plugin.js` & `coop_html_editor-1.4.1/coop_html_editor/static/ckeditor.4.6.2/plugins/lineutils/plugin.js`

 * *Files identical despite different names*

### Comparing `coop_html_editor-1.3.1/coop_html_editor/static/ckeditor.4.6.2/plugins/link/images/hidpi/anchor.png` & `coop_html_editor-1.4.1/coop_html_editor/static/ckeditor.4.6.2/plugins/link/images/hidpi/anchor.png`

 * *Files identical despite different names*

### Comparing `coop_html_editor-1.3.1/coop_html_editor/static/ckeditor.4.6.2/plugins/link/images/anchor.png` & `coop_html_editor-1.4.1/coop_html_editor/static/ckeditor.4.6.2/plugins/link/images/anchor.png`

 * *Files identical despite different names*

### Comparing `coop_html_editor-1.3.1/coop_html_editor/static/ckeditor.4.6.2/plugins/link/dialogs/link.js` & `coop_html_editor-1.4.1/coop_html_editor/static/ckeditor.4.6.2/plugins/link/dialogs/link.js`

 * *Files identical despite different names*

### Comparing `coop_html_editor-1.3.1/coop_html_editor/static/ckeditor.4.6.2/plugins/link/dialogs/anchor.js` & `coop_html_editor-1.4.1/coop_html_editor/static/ckeditor.4.6.2/plugins/link/dialogs/anchor.js`

 * *Files identical despite different names*

### Comparing `coop_html_editor-1.3.1/coop_html_editor/static/ckeditor.4.6.2/plugins/table/dialogs/table.js` & `coop_html_editor-1.4.1/coop_html_editor/static/ckeditor.4.6.2/plugins/table/dialogs/table.js`

 * *Files identical despite different names*

### Comparing `coop_html_editor-1.3.1/coop_html_editor/static/ckeditor.4.6.2/plugins/widgetselection/plugin.js` & `coop_html_editor-1.4.1/coop_html_editor/static/ckeditor.4.6.2/plugins/widgetselection/plugin.js`

 * *Files identical despite different names*

### Comparing `coop_html_editor-1.3.1/coop_html_editor/static/ckeditor.4.6.2/plugins/icons_hidpi.png` & `coop_html_editor-1.4.1/coop_html_editor/static/ckeditor.4.6.2/plugins/icons_hidpi.png`

 * *Files identical despite different names*

### Comparing `coop_html_editor-1.3.1/coop_html_editor/static/ckeditor.4.6.2/plugins/a11yhelp/dialogs/a11yhelp.js` & `coop_html_editor-1.4.1/coop_html_editor/static/ckeditor.4.6.2/plugins/a11yhelp/dialogs/a11yhelp.js`

 * *Files identical despite different names*

### Comparing `coop_html_editor-1.3.1/coop_html_editor/static/ckeditor.4.6.2/plugins/a11yhelp/dialogs/lang/sr-latn.js` & `coop_html_editor-1.4.1/coop_html_editor/static/ckeditor.4.6.2/plugins/a11yhelp/dialogs/lang/sr-latn.js`

 * *Files identical despite different names*

### Comparing `coop_html_editor-1.3.1/coop_html_editor/static/ckeditor.4.6.2/plugins/a11yhelp/dialogs/lang/pt.js` & `coop_html_editor-1.4.1/coop_html_editor/static/ckeditor.4.6.2/plugins/a11yhelp/dialogs/lang/pt.js`

 * *Files identical despite different names*

### Comparing `coop_html_editor-1.3.1/coop_html_editor/static/ckeditor.4.6.2/plugins/a11yhelp/dialogs/lang/vi.js` & `coop_html_editor-1.4.1/coop_html_editor/static/ckeditor.4.6.2/plugins/a11yhelp/dialogs/lang/vi.js`

 * *Files identical despite different names*

### Comparing `coop_html_editor-1.3.1/coop_html_editor/static/ckeditor.4.6.2/plugins/a11yhelp/dialogs/lang/lv.js` & `coop_html_editor-1.4.1/coop_html_editor/static/ckeditor.4.6.2/plugins/a11yhelp/dialogs/lang/lv.js`

 * *Files identical despite different names*

### Comparing `coop_html_editor-1.3.1/coop_html_editor/static/ckeditor.4.6.2/plugins/a11yhelp/dialogs/lang/gl.js` & `coop_html_editor-1.4.1/coop_html_editor/static/ckeditor.4.6.2/plugins/a11yhelp/dialogs/lang/gl.js`

 * *Files identical despite different names*

### Comparing `coop_html_editor-1.3.1/coop_html_editor/static/ckeditor.4.6.2/plugins/a11yhelp/dialogs/lang/pl.js` & `coop_html_editor-1.4.1/coop_html_editor/static/ckeditor.4.6.2/plugins/a11yhelp/dialogs/lang/pl.js`

 * *Files identical despite different names*

### Comparing `coop_html_editor-1.3.1/coop_html_editor/static/ckeditor.4.6.2/plugins/a11yhelp/dialogs/lang/mn.js` & `coop_html_editor-1.4.1/coop_html_editor/static/ckeditor.4.6.2/plugins/a11yhelp/dialogs/lang/mn.js`

 * *Files identical despite different names*

### Comparing `coop_html_editor-1.3.1/coop_html_editor/static/ckeditor.4.6.2/plugins/a11yhelp/dialogs/lang/el.js` & `coop_html_editor-1.4.1/coop_html_editor/static/ckeditor.4.6.2/plugins/a11yhelp/dialogs/lang/el.js`

 * *Files identical despite different names*

### Comparing `coop_html_editor-1.3.1/coop_html_editor/static/ckeditor.4.6.2/plugins/a11yhelp/dialogs/lang/et.js` & `coop_html_editor-1.4.1/coop_html_editor/static/ckeditor.4.6.2/plugins/a11yhelp/dialogs/lang/et.js`

 * *Files identical despite different names*

### Comparing `coop_html_editor-1.3.1/coop_html_editor/static/ckeditor.4.6.2/plugins/a11yhelp/dialogs/lang/sl.js` & `coop_html_editor-1.4.1/coop_html_editor/static/ckeditor.4.6.2/plugins/a11yhelp/dialogs/lang/sl.js`

 * *Files identical despite different names*

### Comparing `coop_html_editor-1.3.1/coop_html_editor/static/ckeditor.4.6.2/plugins/a11yhelp/dialogs/lang/ko.js` & `coop_html_editor-1.4.1/coop_html_editor/static/ckeditor.4.6.2/plugins/a11yhelp/dialogs/lang/ko.js`

 * *Files identical despite different names*

### Comparing `coop_html_editor-1.3.1/coop_html_editor/static/ckeditor.4.6.2/plugins/a11yhelp/dialogs/lang/hr.js` & `coop_html_editor-1.4.1/coop_html_editor/static/ckeditor.4.6.2/plugins/a11yhelp/dialogs/lang/hr.js`

 * *Files identical despite different names*

### Comparing `coop_html_editor-1.3.1/coop_html_editor/static/ckeditor.4.6.2/plugins/a11yhelp/dialogs/lang/fi.js` & `coop_html_editor-1.4.1/coop_html_editor/static/ckeditor.4.6.2/plugins/a11yhelp/dialogs/lang/fi.js`

 * *Files identical despite different names*

### Comparing `coop_html_editor-1.3.1/coop_html_editor/static/ckeditor.4.6.2/plugins/a11yhelp/dialogs/lang/th.js` & `coop_html_editor-1.4.1/coop_html_editor/static/ckeditor.4.6.2/plugins/a11yhelp/dialogs/lang/th.js`

 * *Files identical despite different names*

### Comparing `coop_html_editor-1.3.1/coop_html_editor/static/ckeditor.4.6.2/plugins/a11yhelp/dialogs/lang/ru.js` & `coop_html_editor-1.4.1/coop_html_editor/static/ckeditor.4.6.2/plugins/a11yhelp/dialogs/lang/ru.js`

 * *Files identical despite different names*

### Comparing `coop_html_editor-1.3.1/coop_html_editor/static/ckeditor.4.6.2/plugins/a11yhelp/dialogs/lang/eu.js` & `coop_html_editor-1.4.1/coop_html_editor/static/ckeditor.4.6.2/plugins/a11yhelp/dialogs/lang/eu.js`

 * *Files identical despite different names*

### Comparing `coop_html_editor-1.3.1/coop_html_editor/static/ckeditor.4.6.2/plugins/a11yhelp/dialogs/lang/mk.js` & `coop_html_editor-1.4.1/coop_html_editor/static/ckeditor.4.6.2/plugins/a11yhelp/dialogs/lang/mk.js`

 * *Files identical despite different names*

### Comparing `coop_html_editor-1.3.1/coop_html_editor/static/ckeditor.4.6.2/plugins/a11yhelp/dialogs/lang/no.js` & `coop_html_editor-1.4.1/coop_html_editor/static/ckeditor.4.6.2/plugins/a11yhelp/dialogs/lang/no.js`

 * *Files identical despite different names*

### Comparing `coop_html_editor-1.3.1/coop_html_editor/static/ckeditor.4.6.2/plugins/a11yhelp/dialogs/lang/sq.js` & `coop_html_editor-1.4.1/coop_html_editor/static/ckeditor.4.6.2/plugins/a11yhelp/dialogs/lang/sq.js`

 * *Files identical despite different names*

### Comparing `coop_html_editor-1.3.1/coop_html_editor/static/ckeditor.4.6.2/plugins/a11yhelp/dialogs/lang/gu.js` & `coop_html_editor-1.4.1/coop_html_editor/static/ckeditor.4.6.2/plugins/a11yhelp/dialogs/lang/gu.js`

 * *Files identical despite different names*

### Comparing `coop_html_editor-1.3.1/coop_html_editor/static/ckeditor.4.6.2/plugins/a11yhelp/dialogs/lang/si.js` & `coop_html_editor-1.4.1/coop_html_editor/static/ckeditor.4.6.2/plugins/a11yhelp/dialogs/lang/si.js`

 * *Files identical despite different names*

### Comparing `coop_html_editor-1.3.1/coop_html_editor/static/ckeditor.4.6.2/plugins/a11yhelp/dialogs/lang/tt.js` & `coop_html_editor-1.4.1/coop_html_editor/static/ckeditor.4.6.2/plugins/a11yhelp/dialogs/lang/tt.js`

 * *Files identical despite different names*

### Comparing `coop_html_editor-1.3.1/coop_html_editor/static/ckeditor.4.6.2/plugins/a11yhelp/dialogs/lang/ja.js` & `coop_html_editor-1.4.1/coop_html_editor/static/ckeditor.4.6.2/plugins/a11yhelp/dialogs/lang/ja.js`

 * *Files identical despite different names*

### Comparing `coop_html_editor-1.3.1/coop_html_editor/static/ckeditor.4.6.2/plugins/a11yhelp/dialogs/lang/he.js` & `coop_html_editor-1.4.1/coop_html_editor/static/ckeditor.4.6.2/plugins/a11yhelp/dialogs/lang/he.js`

 * *Files identical despite different names*

### Comparing `coop_html_editor-1.3.1/coop_html_editor/static/ckeditor.4.6.2/plugins/a11yhelp/dialogs/lang/ug.js` & `coop_html_editor-1.4.1/coop_html_editor/static/ckeditor.4.6.2/plugins/a11yhelp/dialogs/lang/ug.js`

 * *Files identical despite different names*

### Comparing `coop_html_editor-1.3.1/coop_html_editor/static/ckeditor.4.6.2/plugins/a11yhelp/dialogs/lang/bg.js` & `coop_html_editor-1.4.1/coop_html_editor/static/ckeditor.4.6.2/plugins/a11yhelp/dialogs/lang/bg.js`

 * *Files identical despite different names*

### Comparing `coop_html_editor-1.3.1/coop_html_editor/static/ckeditor.4.6.2/plugins/a11yhelp/dialogs/lang/af.js` & `coop_html_editor-1.4.1/coop_html_editor/static/ckeditor.4.6.2/plugins/a11yhelp/dialogs/lang/af.js`

 * *Files identical despite different names*

### Comparing `coop_html_editor-1.3.1/coop_html_editor/static/ckeditor.4.6.2/plugins/a11yhelp/dialogs/lang/id.js` & `coop_html_editor-1.4.1/coop_html_editor/static/ckeditor.4.6.2/plugins/a11yhelp/dialogs/lang/id.js`

 * *Files identical despite different names*

### Comparing `coop_html_editor-1.3.1/coop_html_editor/static/ckeditor.4.6.2/plugins/a11yhelp/dialogs/lang/az.js` & `coop_html_editor-1.4.1/coop_html_editor/static/ckeditor.4.6.2/plugins/a11yhelp/dialogs/lang/az.js`

 * *Files identical despite different names*

### Comparing `coop_html_editor-1.3.1/coop_html_editor/static/ckeditor.4.6.2/plugins/a11yhelp/dialogs/lang/ca.js` & `coop_html_editor-1.4.1/coop_html_editor/static/ckeditor.4.6.2/plugins/a11yhelp/dialogs/lang/ca.js`

 * *Files identical despite different names*

### Comparing `coop_html_editor-1.3.1/coop_html_editor/static/ckeditor.4.6.2/plugins/a11yhelp/dialogs/lang/cy.js` & `coop_html_editor-1.4.1/coop_html_editor/static/ckeditor.4.6.2/plugins/a11yhelp/dialogs/lang/cy.js`

 * *Files identical despite different names*

### Comparing `coop_html_editor-1.3.1/coop_html_editor/static/ckeditor.4.6.2/plugins/a11yhelp/dialogs/lang/_translationstatus.txt` & `coop_html_editor-1.4.1/coop_html_editor/static/ckeditor.4.6.2/plugins/a11yhelp/dialogs/lang/_translationstatus.txt`

 * *Files identical despite different names*

### Comparing `coop_html_editor-1.3.1/coop_html_editor/static/ckeditor.4.6.2/plugins/a11yhelp/dialogs/lang/nb.js` & `coop_html_editor-1.4.1/coop_html_editor/static/ckeditor.4.6.2/plugins/a11yhelp/dialogs/lang/nb.js`

 * *Files identical despite different names*

### Comparing `coop_html_editor-1.3.1/coop_html_editor/static/ckeditor.4.6.2/plugins/a11yhelp/dialogs/lang/zh-cn.js` & `coop_html_editor-1.4.1/coop_html_editor/static/ckeditor.4.6.2/plugins/a11yhelp/dialogs/lang/zh-cn.js`

 * *Files identical despite different names*

### Comparing `coop_html_editor-1.3.1/coop_html_editor/static/ckeditor.4.6.2/plugins/a11yhelp/dialogs/lang/de-ch.js` & `coop_html_editor-1.4.1/coop_html_editor/static/ckeditor.4.6.2/plugins/a11yhelp/dialogs/lang/de-ch.js`

 * *Files identical despite different names*

### Comparing `coop_html_editor-1.3.1/coop_html_editor/static/ckeditor.4.6.2/plugins/a11yhelp/dialogs/lang/pt-br.js` & `coop_html_editor-1.4.1/coop_html_editor/static/ckeditor.4.6.2/plugins/a11yhelp/dialogs/lang/pt-br.js`

 * *Files identical despite different names*

### Comparing `coop_html_editor-1.3.1/coop_html_editor/static/ckeditor.4.6.2/plugins/a11yhelp/dialogs/lang/oc.js` & `coop_html_editor-1.4.1/coop_html_editor/static/ckeditor.4.6.2/plugins/a11yhelp/dialogs/lang/oc.js`

 * *Files identical despite different names*

### Comparing `coop_html_editor-1.3.1/coop_html_editor/static/ckeditor.4.6.2/plugins/a11yhelp/dialogs/lang/da.js` & `coop_html_editor-1.4.1/coop_html_editor/static/ckeditor.4.6.2/plugins/a11yhelp/dialogs/lang/da.js`

 * *Files identical despite different names*

### Comparing `coop_html_editor-1.3.1/coop_html_editor/static/ckeditor.4.6.2/plugins/a11yhelp/dialogs/lang/fa.js` & `coop_html_editor-1.4.1/coop_html_editor/static/ckeditor.4.6.2/plugins/a11yhelp/dialogs/lang/fa.js`

 * *Files identical despite different names*

### Comparing `coop_html_editor-1.3.1/coop_html_editor/static/ckeditor.4.6.2/plugins/a11yhelp/dialogs/lang/de.js` & `coop_html_editor-1.4.1/coop_html_editor/static/ckeditor.4.6.2/plugins/a11yhelp/dialogs/lang/de.js`

 * *Files identical despite different names*

### Comparing `coop_html_editor-1.3.1/coop_html_editor/static/ckeditor.4.6.2/plugins/a11yhelp/dialogs/lang/en.js` & `coop_html_editor-1.4.1/coop_html_editor/static/ckeditor.4.6.2/plugins/a11yhelp/dialogs/lang/en.js`

 * *Files identical despite different names*

### Comparing `coop_html_editor-1.3.1/coop_html_editor/static/ckeditor.4.6.2/plugins/a11yhelp/dialogs/lang/ku.js` & `coop_html_editor-1.4.1/coop_html_editor/static/ckeditor.4.6.2/plugins/a11yhelp/dialogs/lang/ku.js`

 * *Files identical despite different names*

### Comparing `coop_html_editor-1.3.1/coop_html_editor/static/ckeditor.4.6.2/plugins/a11yhelp/dialogs/lang/sv.js` & `coop_html_editor-1.4.1/coop_html_editor/static/ckeditor.4.6.2/plugins/a11yhelp/dialogs/lang/sv.js`

 * *Files identical despite different names*

### Comparing `coop_html_editor-1.3.1/coop_html_editor/static/ckeditor.4.6.2/plugins/a11yhelp/dialogs/lang/zh.js` & `coop_html_editor-1.4.1/coop_html_editor/static/ckeditor.4.6.2/plugins/a11yhelp/dialogs/lang/zh.js`

 * *Files identical despite different names*

### Comparing `coop_html_editor-1.3.1/coop_html_editor/static/ckeditor.4.6.2/plugins/a11yhelp/dialogs/lang/hi.js` & `coop_html_editor-1.4.1/coop_html_editor/static/ckeditor.4.6.2/plugins/a11yhelp/dialogs/lang/hi.js`

 * *Files identical despite different names*

### Comparing `coop_html_editor-1.3.1/coop_html_editor/static/ckeditor.4.6.2/plugins/a11yhelp/dialogs/lang/uk.js` & `coop_html_editor-1.4.1/coop_html_editor/static/ckeditor.4.6.2/plugins/a11yhelp/dialogs/lang/uk.js`

 * *Files identical despite different names*

### Comparing `coop_html_editor-1.3.1/coop_html_editor/static/ckeditor.4.6.2/plugins/a11yhelp/dialogs/lang/cs.js` & `coop_html_editor-1.4.1/coop_html_editor/static/ckeditor.4.6.2/plugins/a11yhelp/dialogs/lang/cs.js`

 * *Files identical despite different names*

### Comparing `coop_html_editor-1.3.1/coop_html_editor/static/ckeditor.4.6.2/plugins/a11yhelp/dialogs/lang/km.js` & `coop_html_editor-1.4.1/coop_html_editor/static/ckeditor.4.6.2/plugins/a11yhelp/dialogs/lang/km.js`

 * *Files identical despite different names*

### Comparing `coop_html_editor-1.3.1/coop_html_editor/static/ckeditor.4.6.2/plugins/a11yhelp/dialogs/lang/fr.js` & `coop_html_editor-1.4.1/coop_html_editor/static/ckeditor.4.6.2/plugins/a11yhelp/dialogs/lang/fr.js`

 * *Files identical despite different names*

### Comparing `coop_html_editor-1.3.1/coop_html_editor/static/ckeditor.4.6.2/plugins/a11yhelp/dialogs/lang/nl.js` & `coop_html_editor-1.4.1/coop_html_editor/static/ckeditor.4.6.2/plugins/a11yhelp/dialogs/lang/nl.js`

 * *Files identical despite different names*

### Comparing `coop_html_editor-1.3.1/coop_html_editor/static/ckeditor.4.6.2/plugins/a11yhelp/dialogs/lang/fr-ca.js` & `coop_html_editor-1.4.1/coop_html_editor/static/ckeditor.4.6.2/plugins/a11yhelp/dialogs/lang/fr-ca.js`

 * *Files identical despite different names*

### Comparing `coop_html_editor-1.3.1/coop_html_editor/static/ckeditor.4.6.2/plugins/a11yhelp/dialogs/lang/en-gb.js` & `coop_html_editor-1.4.1/coop_html_editor/static/ckeditor.4.6.2/plugins/a11yhelp/dialogs/lang/en-gb.js`

 * *Files identical despite different names*

### Comparing `coop_html_editor-1.3.1/coop_html_editor/static/ckeditor.4.6.2/plugins/a11yhelp/dialogs/lang/sr.js` & `coop_html_editor-1.4.1/coop_html_editor/static/ckeditor.4.6.2/plugins/a11yhelp/dialogs/lang/sr.js`

 * *Files identical despite different names*

### Comparing `coop_html_editor-1.3.1/coop_html_editor/static/ckeditor.4.6.2/plugins/a11yhelp/dialogs/lang/hu.js` & `coop_html_editor-1.4.1/coop_html_editor/static/ckeditor.4.6.2/plugins/a11yhelp/dialogs/lang/hu.js`

 * *Files identical despite different names*

### Comparing `coop_html_editor-1.3.1/coop_html_editor/static/ckeditor.4.6.2/plugins/a11yhelp/dialogs/lang/lt.js` & `coop_html_editor-1.4.1/coop_html_editor/static/ckeditor.4.6.2/plugins/a11yhelp/dialogs/lang/lt.js`

 * *Files identical despite different names*

### Comparing `coop_html_editor-1.3.1/coop_html_editor/static/ckeditor.4.6.2/plugins/a11yhelp/dialogs/lang/fo.js` & `coop_html_editor-1.4.1/coop_html_editor/static/ckeditor.4.6.2/plugins/a11yhelp/dialogs/lang/fo.js`

 * *Files identical despite different names*

### Comparing `coop_html_editor-1.3.1/coop_html_editor/static/ckeditor.4.6.2/plugins/a11yhelp/dialogs/lang/ar.js` & `coop_html_editor-1.4.1/coop_html_editor/static/ckeditor.4.6.2/plugins/a11yhelp/dialogs/lang/ar.js`

 * *Files identical despite different names*

### Comparing `coop_html_editor-1.3.1/coop_html_editor/static/ckeditor.4.6.2/plugins/a11yhelp/dialogs/lang/sk.js` & `coop_html_editor-1.4.1/coop_html_editor/static/ckeditor.4.6.2/plugins/a11yhelp/dialogs/lang/sk.js`

 * *Files identical despite different names*

### Comparing `coop_html_editor-1.3.1/coop_html_editor/static/ckeditor.4.6.2/plugins/a11yhelp/dialogs/lang/it.js` & `coop_html_editor-1.4.1/coop_html_editor/static/ckeditor.4.6.2/plugins/a11yhelp/dialogs/lang/it.js`

 * *Files identical despite different names*

### Comparing `coop_html_editor-1.3.1/coop_html_editor/static/ckeditor.4.6.2/plugins/a11yhelp/dialogs/lang/es.js` & `coop_html_editor-1.4.1/coop_html_editor/static/ckeditor.4.6.2/plugins/a11yhelp/dialogs/lang/es.js`

 * *Files identical despite different names*

### Comparing `coop_html_editor-1.3.1/coop_html_editor/static/ckeditor.4.6.2/plugins/a11yhelp/dialogs/lang/eo.js` & `coop_html_editor-1.4.1/coop_html_editor/static/ckeditor.4.6.2/plugins/a11yhelp/dialogs/lang/eo.js`

 * *Files identical despite different names*

### Comparing `coop_html_editor-1.3.1/coop_html_editor/static/ckeditor.4.6.2/plugins/a11yhelp/dialogs/lang/ro.js` & `coop_html_editor-1.4.1/coop_html_editor/static/ckeditor.4.6.2/plugins/a11yhelp/dialogs/lang/ro.js`

 * *Files identical despite different names*

### Comparing `coop_html_editor-1.3.1/coop_html_editor/static/ckeditor.4.6.2/plugins/a11yhelp/dialogs/lang/tr.js` & `coop_html_editor-1.4.1/coop_html_editor/static/ckeditor.4.6.2/plugins/a11yhelp/dialogs/lang/tr.js`

 * *Files identical despite different names*

### Comparing `coop_html_editor-1.3.1/coop_html_editor/static/ckeditor.4.6.2/plugins/sourcedialog/samples/sourcedialog.html` & `coop_html_editor-1.4.1/coop_html_editor/static/ckeditor.4.6.2/plugins/sourcedialog/samples/sourcedialog.html`

 * *Files identical despite different names*

### Comparing `coop_html_editor-1.3.1/coop_html_editor/static/ckeditor.4.6.2/plugins/sourcedialog/dialogs/sourcedialog.js` & `coop_html_editor-1.4.1/coop_html_editor/static/ckeditor.4.6.2/plugins/sourcedialog/dialogs/sourcedialog.js`

 * *Files identical despite different names*

### Comparing `coop_html_editor-1.3.1/coop_html_editor/static/ckeditor.4.6.2/plugins/sourcedialog/plugin.js` & `coop_html_editor-1.4.1/coop_html_editor/static/ckeditor.4.6.2/plugins/sourcedialog/plugin.js`

 * *Files identical despite different names*

### Comparing `coop_html_editor-1.3.1/coop_html_editor/static/ckeditor.4.6.2/plugins/specialchar/dialogs/specialchar.js` & `coop_html_editor-1.4.1/coop_html_editor/static/ckeditor.4.6.2/plugins/specialchar/dialogs/specialchar.js`

 * *Files identical despite different names*

### Comparing `coop_html_editor-1.3.1/coop_html_editor/static/ckeditor.4.6.2/plugins/specialchar/dialogs/lang/pt.js` & `coop_html_editor-1.4.1/coop_html_editor/static/ckeditor.4.6.2/plugins/specialchar/dialogs/lang/pt.js`

 * *Files identical despite different names*

### Comparing `coop_html_editor-1.3.1/coop_html_editor/static/ckeditor.4.6.2/plugins/specialchar/dialogs/lang/vi.js` & `coop_html_editor-1.4.1/coop_html_editor/static/ckeditor.4.6.2/plugins/specialchar/dialogs/lang/vi.js`

 * *Files identical despite different names*

### Comparing `coop_html_editor-1.3.1/coop_html_editor/static/ckeditor.4.6.2/plugins/specialchar/dialogs/lang/lv.js` & `coop_html_editor-1.4.1/coop_html_editor/static/ckeditor.4.6.2/plugins/specialchar/dialogs/lang/lv.js`

 * *Files identical despite different names*

### Comparing `coop_html_editor-1.3.1/coop_html_editor/static/ckeditor.4.6.2/plugins/specialchar/dialogs/lang/gl.js` & `coop_html_editor-1.4.1/coop_html_editor/static/ckeditor.4.6.2/plugins/specialchar/dialogs/lang/gl.js`

 * *Files identical despite different names*

### Comparing `coop_html_editor-1.3.1/coop_html_editor/static/ckeditor.4.6.2/plugins/specialchar/dialogs/lang/pl.js` & `coop_html_editor-1.4.1/coop_html_editor/static/ckeditor.4.6.2/plugins/specialchar/dialogs/lang/pl.js`

 * *Files identical despite different names*

### Comparing `coop_html_editor-1.3.1/coop_html_editor/static/ckeditor.4.6.2/plugins/specialchar/dialogs/lang/el.js` & `coop_html_editor-1.4.1/coop_html_editor/static/ckeditor.4.6.2/plugins/specialchar/dialogs/lang/el.js`

 * *Files identical despite different names*

### Comparing `coop_html_editor-1.3.1/coop_html_editor/static/ckeditor.4.6.2/plugins/specialchar/dialogs/lang/et.js` & `coop_html_editor-1.4.1/coop_html_editor/static/ckeditor.4.6.2/plugins/specialchar/dialogs/lang/et.js`

 * *Files identical despite different names*

### Comparing `coop_html_editor-1.3.1/coop_html_editor/static/ckeditor.4.6.2/plugins/specialchar/dialogs/lang/sl.js` & `coop_html_editor-1.4.1/coop_html_editor/static/ckeditor.4.6.2/plugins/specialchar/dialogs/lang/sl.js`

 * *Files identical despite different names*

### Comparing `coop_html_editor-1.3.1/coop_html_editor/static/ckeditor.4.6.2/plugins/specialchar/dialogs/lang/ko.js` & `coop_html_editor-1.4.1/coop_html_editor/static/ckeditor.4.6.2/plugins/specialchar/dialogs/lang/ko.js`

 * *Files identical despite different names*

### Comparing `coop_html_editor-1.3.1/coop_html_editor/static/ckeditor.4.6.2/plugins/specialchar/dialogs/lang/hr.js` & `coop_html_editor-1.4.1/coop_html_editor/static/ckeditor.4.6.2/plugins/specialchar/dialogs/lang/hr.js`

 * *Files identical despite different names*

### Comparing `coop_html_editor-1.3.1/coop_html_editor/static/ckeditor.4.6.2/plugins/specialchar/dialogs/lang/fi.js` & `coop_html_editor-1.4.1/coop_html_editor/static/ckeditor.4.6.2/plugins/specialchar/dialogs/lang/fi.js`

 * *Files identical despite different names*

### Comparing `coop_html_editor-1.3.1/coop_html_editor/static/ckeditor.4.6.2/plugins/specialchar/dialogs/lang/th.js` & `coop_html_editor-1.4.1/coop_html_editor/static/ckeditor.4.6.2/plugins/specialchar/dialogs/lang/th.js`

 * *Files identical despite different names*

### Comparing `coop_html_editor-1.3.1/coop_html_editor/static/ckeditor.4.6.2/plugins/specialchar/dialogs/lang/ru.js` & `coop_html_editor-1.4.1/coop_html_editor/static/ckeditor.4.6.2/plugins/specialchar/dialogs/lang/ru.js`

 * *Files identical despite different names*

### Comparing `coop_html_editor-1.3.1/coop_html_editor/static/ckeditor.4.6.2/plugins/specialchar/dialogs/lang/eu.js` & `coop_html_editor-1.4.1/coop_html_editor/static/ckeditor.4.6.2/plugins/specialchar/dialogs/lang/eu.js`

 * *Files identical despite different names*

### Comparing `coop_html_editor-1.3.1/coop_html_editor/static/ckeditor.4.6.2/plugins/specialchar/dialogs/lang/no.js` & `coop_html_editor-1.4.1/coop_html_editor/static/ckeditor.4.6.2/plugins/specialchar/dialogs/lang/no.js`

 * *Files identical despite different names*

### Comparing `coop_html_editor-1.3.1/coop_html_editor/static/ckeditor.4.6.2/plugins/specialchar/dialogs/lang/sq.js` & `coop_html_editor-1.4.1/coop_html_editor/static/ckeditor.4.6.2/plugins/specialchar/dialogs/lang/sq.js`

 * *Files identical despite different names*

### Comparing `coop_html_editor-1.3.1/coop_html_editor/static/ckeditor.4.6.2/plugins/specialchar/dialogs/lang/si.js` & `coop_html_editor-1.4.1/coop_html_editor/static/ckeditor.4.6.2/plugins/specialchar/dialogs/lang/si.js`

 * *Files identical despite different names*

### Comparing `coop_html_editor-1.3.1/coop_html_editor/static/ckeditor.4.6.2/plugins/specialchar/dialogs/lang/tt.js` & `coop_html_editor-1.4.1/coop_html_editor/static/ckeditor.4.6.2/plugins/specialchar/dialogs/lang/tt.js`

 * *Files identical despite different names*

### Comparing `coop_html_editor-1.3.1/coop_html_editor/static/ckeditor.4.6.2/plugins/specialchar/dialogs/lang/ja.js` & `coop_html_editor-1.4.1/coop_html_editor/static/ckeditor.4.6.2/plugins/specialchar/dialogs/lang/ja.js`

 * *Files identical despite different names*

### Comparing `coop_html_editor-1.3.1/coop_html_editor/static/ckeditor.4.6.2/plugins/specialchar/dialogs/lang/he.js` & `coop_html_editor-1.4.1/coop_html_editor/static/ckeditor.4.6.2/plugins/specialchar/dialogs/lang/he.js`

 * *Files identical despite different names*

### Comparing `coop_html_editor-1.3.1/coop_html_editor/static/ckeditor.4.6.2/plugins/specialchar/dialogs/lang/ug.js` & `coop_html_editor-1.4.1/coop_html_editor/static/ckeditor.4.6.2/plugins/specialchar/dialogs/lang/ug.js`

 * *Files identical despite different names*

### Comparing `coop_html_editor-1.3.1/coop_html_editor/static/ckeditor.4.6.2/plugins/specialchar/dialogs/lang/bg.js` & `coop_html_editor-1.4.1/coop_html_editor/static/ckeditor.4.6.2/plugins/specialchar/dialogs/lang/bg.js`

 * *Files identical despite different names*

### Comparing `coop_html_editor-1.3.1/coop_html_editor/static/ckeditor.4.6.2/plugins/specialchar/dialogs/lang/af.js` & `coop_html_editor-1.4.1/coop_html_editor/static/ckeditor.4.6.2/plugins/specialchar/dialogs/lang/af.js`

 * *Files identical despite different names*

### Comparing `coop_html_editor-1.3.1/coop_html_editor/static/ckeditor.4.6.2/plugins/specialchar/dialogs/lang/id.js` & `coop_html_editor-1.4.1/coop_html_editor/static/ckeditor.4.6.2/plugins/specialchar/dialogs/lang/id.js`

 * *Files identical despite different names*

### Comparing `coop_html_editor-1.3.1/coop_html_editor/static/ckeditor.4.6.2/plugins/specialchar/dialogs/lang/az.js` & `coop_html_editor-1.4.1/coop_html_editor/static/ckeditor.4.6.2/plugins/specialchar/dialogs/lang/az.js`

 * *Files identical despite different names*

### Comparing `coop_html_editor-1.3.1/coop_html_editor/static/ckeditor.4.6.2/plugins/specialchar/dialogs/lang/ca.js` & `coop_html_editor-1.4.1/coop_html_editor/static/ckeditor.4.6.2/plugins/specialchar/dialogs/lang/ca.js`

 * *Files identical despite different names*

### Comparing `coop_html_editor-1.3.1/coop_html_editor/static/ckeditor.4.6.2/plugins/specialchar/dialogs/lang/cy.js` & `coop_html_editor-1.4.1/coop_html_editor/static/ckeditor.4.6.2/plugins/specialchar/dialogs/lang/cy.js`

 * *Files identical despite different names*

### Comparing `coop_html_editor-1.3.1/coop_html_editor/static/ckeditor.4.6.2/plugins/specialchar/dialogs/lang/_translationstatus.txt` & `coop_html_editor-1.4.1/coop_html_editor/static/ckeditor.4.6.2/plugins/specialchar/dialogs/lang/_translationstatus.txt`

 * *Files identical despite different names*

### Comparing `coop_html_editor-1.3.1/coop_html_editor/static/ckeditor.4.6.2/plugins/specialchar/dialogs/lang/nb.js` & `coop_html_editor-1.4.1/coop_html_editor/static/ckeditor.4.6.2/plugins/specialchar/dialogs/lang/nb.js`

 * *Files identical despite different names*

### Comparing `coop_html_editor-1.3.1/coop_html_editor/static/ckeditor.4.6.2/plugins/specialchar/dialogs/lang/zh-cn.js` & `coop_html_editor-1.4.1/coop_html_editor/static/ckeditor.4.6.2/plugins/specialchar/dialogs/lang/zh-cn.js`

 * *Files identical despite different names*

### Comparing `coop_html_editor-1.3.1/coop_html_editor/static/ckeditor.4.6.2/plugins/specialchar/dialogs/lang/de-ch.js` & `coop_html_editor-1.4.1/coop_html_editor/static/ckeditor.4.6.2/plugins/specialchar/dialogs/lang/de-ch.js`

 * *Files identical despite different names*

### Comparing `coop_html_editor-1.3.1/coop_html_editor/static/ckeditor.4.6.2/plugins/specialchar/dialogs/lang/pt-br.js` & `coop_html_editor-1.4.1/coop_html_editor/static/ckeditor.4.6.2/plugins/specialchar/dialogs/lang/pt-br.js`

 * *Files identical despite different names*

### Comparing `coop_html_editor-1.3.1/coop_html_editor/static/ckeditor.4.6.2/plugins/specialchar/dialogs/lang/oc.js` & `coop_html_editor-1.4.1/coop_html_editor/static/ckeditor.4.6.2/plugins/specialchar/dialogs/lang/oc.js`

 * *Files identical despite different names*

### Comparing `coop_html_editor-1.3.1/coop_html_editor/static/ckeditor.4.6.2/plugins/specialchar/dialogs/lang/da.js` & `coop_html_editor-1.4.1/coop_html_editor/static/ckeditor.4.6.2/plugins/specialchar/dialogs/lang/da.js`

 * *Files identical despite different names*

### Comparing `coop_html_editor-1.3.1/coop_html_editor/static/ckeditor.4.6.2/plugins/specialchar/dialogs/lang/fa.js` & `coop_html_editor-1.4.1/coop_html_editor/static/ckeditor.4.6.2/plugins/specialchar/dialogs/lang/fa.js`

 * *Files identical despite different names*

### Comparing `coop_html_editor-1.3.1/coop_html_editor/static/ckeditor.4.6.2/plugins/specialchar/dialogs/lang/de.js` & `coop_html_editor-1.4.1/coop_html_editor/static/ckeditor.4.6.2/plugins/specialchar/dialogs/lang/de.js`

 * *Files identical despite different names*

### Comparing `coop_html_editor-1.3.1/coop_html_editor/static/ckeditor.4.6.2/plugins/specialchar/dialogs/lang/en.js` & `coop_html_editor-1.4.1/coop_html_editor/static/ckeditor.4.6.2/plugins/specialchar/dialogs/lang/en.js`

 * *Files identical despite different names*

### Comparing `coop_html_editor-1.3.1/coop_html_editor/static/ckeditor.4.6.2/plugins/specialchar/dialogs/lang/ku.js` & `coop_html_editor-1.4.1/coop_html_editor/static/ckeditor.4.6.2/plugins/specialchar/dialogs/lang/ku.js`

 * *Files identical despite different names*

### Comparing `coop_html_editor-1.3.1/coop_html_editor/static/ckeditor.4.6.2/plugins/specialchar/dialogs/lang/sv.js` & `coop_html_editor-1.4.1/coop_html_editor/static/ckeditor.4.6.2/plugins/specialchar/dialogs/lang/sv.js`

 * *Files identical despite different names*

### Comparing `coop_html_editor-1.3.1/coop_html_editor/static/ckeditor.4.6.2/plugins/specialchar/dialogs/lang/zh.js` & `coop_html_editor-1.4.1/coop_html_editor/static/ckeditor.4.6.2/plugins/specialchar/dialogs/lang/zh.js`

 * *Files identical despite different names*

### Comparing `coop_html_editor-1.3.1/coop_html_editor/static/ckeditor.4.6.2/plugins/specialchar/dialogs/lang/uk.js` & `coop_html_editor-1.4.1/coop_html_editor/static/ckeditor.4.6.2/plugins/specialchar/dialogs/lang/uk.js`

 * *Files identical despite different names*

### Comparing `coop_html_editor-1.3.1/coop_html_editor/static/ckeditor.4.6.2/plugins/specialchar/dialogs/lang/cs.js` & `coop_html_editor-1.4.1/coop_html_editor/static/ckeditor.4.6.2/plugins/specialchar/dialogs/lang/cs.js`

 * *Files identical despite different names*

### Comparing `coop_html_editor-1.3.1/coop_html_editor/static/ckeditor.4.6.2/plugins/specialchar/dialogs/lang/km.js` & `coop_html_editor-1.4.1/coop_html_editor/static/ckeditor.4.6.2/plugins/specialchar/dialogs/lang/km.js`

 * *Files identical despite different names*

### Comparing `coop_html_editor-1.3.1/coop_html_editor/static/ckeditor.4.6.2/plugins/specialchar/dialogs/lang/fr.js` & `coop_html_editor-1.4.1/coop_html_editor/static/ckeditor.4.6.2/plugins/specialchar/dialogs/lang/fr.js`

 * *Files identical despite different names*

### Comparing `coop_html_editor-1.3.1/coop_html_editor/static/ckeditor.4.6.2/plugins/specialchar/dialogs/lang/nl.js` & `coop_html_editor-1.4.1/coop_html_editor/static/ckeditor.4.6.2/plugins/specialchar/dialogs/lang/nl.js`

 * *Files identical despite different names*

### Comparing `coop_html_editor-1.3.1/coop_html_editor/static/ckeditor.4.6.2/plugins/specialchar/dialogs/lang/fr-ca.js` & `coop_html_editor-1.4.1/coop_html_editor/static/ckeditor.4.6.2/plugins/specialchar/dialogs/lang/fr-ca.js`

 * *Files identical despite different names*

### Comparing `coop_html_editor-1.3.1/coop_html_editor/static/ckeditor.4.6.2/plugins/specialchar/dialogs/lang/en-gb.js` & `coop_html_editor-1.4.1/coop_html_editor/static/ckeditor.4.6.2/plugins/specialchar/dialogs/lang/en-gb.js`

 * *Files identical despite different names*

### Comparing `coop_html_editor-1.3.1/coop_html_editor/static/ckeditor.4.6.2/plugins/specialchar/dialogs/lang/hu.js` & `coop_html_editor-1.4.1/coop_html_editor/static/ckeditor.4.6.2/plugins/specialchar/dialogs/lang/hu.js`

 * *Files identical despite different names*

### Comparing `coop_html_editor-1.3.1/coop_html_editor/static/ckeditor.4.6.2/plugins/specialchar/dialogs/lang/lt.js` & `coop_html_editor-1.4.1/coop_html_editor/static/ckeditor.4.6.2/plugins/specialchar/dialogs/lang/lt.js`

 * *Files identical despite different names*

### Comparing `coop_html_editor-1.3.1/coop_html_editor/static/ckeditor.4.6.2/plugins/specialchar/dialogs/lang/ar.js` & `coop_html_editor-1.4.1/coop_html_editor/static/ckeditor.4.6.2/plugins/specialchar/dialogs/lang/ar.js`

 * *Files identical despite different names*

### Comparing `coop_html_editor-1.3.1/coop_html_editor/static/ckeditor.4.6.2/plugins/specialchar/dialogs/lang/sk.js` & `coop_html_editor-1.4.1/coop_html_editor/static/ckeditor.4.6.2/plugins/specialchar/dialogs/lang/sk.js`

 * *Files identical despite different names*

### Comparing `coop_html_editor-1.3.1/coop_html_editor/static/ckeditor.4.6.2/plugins/specialchar/dialogs/lang/it.js` & `coop_html_editor-1.4.1/coop_html_editor/static/ckeditor.4.6.2/plugins/specialchar/dialogs/lang/it.js`

 * *Files identical despite different names*

### Comparing `coop_html_editor-1.3.1/coop_html_editor/static/ckeditor.4.6.2/plugins/specialchar/dialogs/lang/es.js` & `coop_html_editor-1.4.1/coop_html_editor/static/ckeditor.4.6.2/plugins/specialchar/dialogs/lang/es.js`

 * *Files identical despite different names*

### Comparing `coop_html_editor-1.3.1/coop_html_editor/static/ckeditor.4.6.2/plugins/specialchar/dialogs/lang/eo.js` & `coop_html_editor-1.4.1/coop_html_editor/static/ckeditor.4.6.2/plugins/specialchar/dialogs/lang/eo.js`

 * *Files identical despite different names*

### Comparing `coop_html_editor-1.3.1/coop_html_editor/static/ckeditor.4.6.2/plugins/specialchar/dialogs/lang/tr.js` & `coop_html_editor-1.4.1/coop_html_editor/static/ckeditor.4.6.2/plugins/specialchar/dialogs/lang/tr.js`

 * *Files identical despite different names*

### Comparing `coop_html_editor-1.3.1/coop_html_editor/static/ckeditor.4.6.2/plugins/scayt/LICENSE.md` & `coop_html_editor-1.4.1/coop_html_editor/static/ckeditor.4.6.2/plugins/scayt/LICENSE.md`

 * *Files identical despite different names*

### Comparing `coop_html_editor-1.3.1/coop_html_editor/static/ckeditor.4.6.2/plugins/scayt/CHANGELOG.md` & `coop_html_editor-1.4.1/coop_html_editor/static/ckeditor.4.6.2/plugins/scayt/CHANGELOG.md`

 * *Files identical despite different names*

### Comparing `coop_html_editor-1.3.1/coop_html_editor/static/ckeditor.4.6.2/plugins/scayt/README.md` & `coop_html_editor-1.4.1/coop_html_editor/static/ckeditor.4.6.2/plugins/scayt/README.md`

 * *Files identical despite different names*

### Comparing `coop_html_editor-1.3.1/coop_html_editor/static/ckeditor.4.6.2/plugins/scayt/dialogs/toolbar.css` & `coop_html_editor-1.4.1/coop_html_editor/static/ckeditor.4.6.2/plugins/scayt/dialogs/toolbar.css`

 * *Files identical despite different names*

### Comparing `coop_html_editor-1.3.1/coop_html_editor/static/ckeditor.4.6.2/plugins/scayt/dialogs/options.js` & `coop_html_editor-1.4.1/coop_html_editor/static/ckeditor.4.6.2/plugins/scayt/dialogs/options.js`

 * *Files identical despite different names*

### Comparing `coop_html_editor-1.3.1/coop_html_editor/static/ckeditor.4.6.2/plugins/notificationaggregator/plugin.js` & `coop_html_editor-1.4.1/coop_html_editor/static/ckeditor.4.6.2/plugins/notificationaggregator/plugin.js`

 * *Files identical despite different names*

### Comparing `coop_html_editor-1.3.1/coop_html_editor/static/ckeditor.4.6.2/plugins/clipboard/lang/sr-latn.js` & `coop_html_editor-1.4.1/coop_html_editor/static/ckeditor.4.6.2/plugins/clipboard/lang/sr-latn.js`

 * *Files identical despite different names*

### Comparing `coop_html_editor-1.3.1/coop_html_editor/static/ckeditor.4.6.2/plugins/clipboard/lang/pt.js` & `coop_html_editor-1.4.1/coop_html_editor/static/ckeditor.4.6.2/plugins/clipboard/lang/pt.js`

 * *Files identical despite different names*

### Comparing `coop_html_editor-1.3.1/coop_html_editor/static/ckeditor.4.6.2/plugins/clipboard/lang/vi.js` & `coop_html_editor-1.4.1/coop_html_editor/static/ckeditor.4.6.2/plugins/clipboard/lang/vi.js`

 * *Files identical despite different names*

### Comparing `coop_html_editor-1.3.1/coop_html_editor/static/ckeditor.4.6.2/plugins/clipboard/lang/lv.js` & `coop_html_editor-1.4.1/coop_html_editor/static/ckeditor.4.6.2/plugins/clipboard/lang/lv.js`

 * *Files identical despite different names*

### Comparing `coop_html_editor-1.3.1/coop_html_editor/static/ckeditor.4.6.2/plugins/clipboard/lang/gl.js` & `coop_html_editor-1.4.1/coop_html_editor/static/ckeditor.4.6.2/plugins/clipboard/lang/gl.js`

 * *Files identical despite different names*

### Comparing `coop_html_editor-1.3.1/coop_html_editor/static/ckeditor.4.6.2/plugins/clipboard/lang/pl.js` & `coop_html_editor-1.4.1/coop_html_editor/static/ckeditor.4.6.2/plugins/clipboard/lang/pl.js`

 * *Files identical despite different names*

### Comparing `coop_html_editor-1.3.1/coop_html_editor/static/ckeditor.4.6.2/plugins/clipboard/lang/mn.js` & `coop_html_editor-1.4.1/coop_html_editor/static/ckeditor.4.6.2/plugins/clipboard/lang/mn.js`

 * *Files identical despite different names*

### Comparing `coop_html_editor-1.3.1/coop_html_editor/static/ckeditor.4.6.2/plugins/clipboard/lang/en-ca.js` & `coop_html_editor-1.4.1/coop_html_editor/static/ckeditor.4.6.2/plugins/clipboard/lang/en-ca.js`

 * *Files identical despite different names*

### Comparing `coop_html_editor-1.3.1/coop_html_editor/static/ckeditor.4.6.2/plugins/clipboard/lang/el.js` & `coop_html_editor-1.4.1/coop_html_editor/static/ckeditor.4.6.2/plugins/clipboard/lang/el.js`

 * *Files identical despite different names*

### Comparing `coop_html_editor-1.3.1/coop_html_editor/static/ckeditor.4.6.2/plugins/clipboard/lang/et.js` & `coop_html_editor-1.4.1/coop_html_editor/static/ckeditor.4.6.2/plugins/clipboard/lang/et.js`

 * *Files identical despite different names*

### Comparing `coop_html_editor-1.3.1/coop_html_editor/static/ckeditor.4.6.2/plugins/clipboard/lang/is.js` & `coop_html_editor-1.4.1/coop_html_editor/static/ckeditor.4.6.2/plugins/clipboard/lang/is.js`

 * *Files identical despite different names*

### Comparing `coop_html_editor-1.3.1/coop_html_editor/static/ckeditor.4.6.2/plugins/clipboard/lang/sl.js` & `coop_html_editor-1.4.1/coop_html_editor/static/ckeditor.4.6.2/plugins/clipboard/lang/sl.js`

 * *Files identical despite different names*

### Comparing `coop_html_editor-1.3.1/coop_html_editor/static/ckeditor.4.6.2/plugins/clipboard/lang/ko.js` & `coop_html_editor-1.4.1/coop_html_editor/static/ckeditor.4.6.2/plugins/clipboard/lang/ko.js`

 * *Files identical despite different names*

### Comparing `coop_html_editor-1.3.1/coop_html_editor/static/ckeditor.4.6.2/plugins/clipboard/lang/hr.js` & `coop_html_editor-1.4.1/coop_html_editor/static/ckeditor.4.6.2/plugins/clipboard/lang/hr.js`

 * *Files identical despite different names*

### Comparing `coop_html_editor-1.3.1/coop_html_editor/static/ckeditor.4.6.2/plugins/clipboard/lang/ms.js` & `coop_html_editor-1.4.1/coop_html_editor/static/ckeditor.4.6.2/plugins/clipboard/lang/ms.js`

 * *Files identical despite different names*

### Comparing `coop_html_editor-1.3.1/coop_html_editor/static/ckeditor.4.6.2/plugins/clipboard/lang/fi.js` & `coop_html_editor-1.4.1/coop_html_editor/static/ckeditor.4.6.2/plugins/clipboard/lang/fi.js`

 * *Files identical despite different names*

### Comparing `coop_html_editor-1.3.1/coop_html_editor/static/ckeditor.4.6.2/plugins/clipboard/lang/th.js` & `coop_html_editor-1.4.1/coop_html_editor/static/ckeditor.4.6.2/plugins/clipboard/lang/th.js`

 * *Files identical despite different names*

### Comparing `coop_html_editor-1.3.1/coop_html_editor/static/ckeditor.4.6.2/plugins/clipboard/lang/ru.js` & `coop_html_editor-1.4.1/coop_html_editor/static/ckeditor.4.6.2/plugins/clipboard/lang/ru.js`

 * *Files identical despite different names*

### Comparing `coop_html_editor-1.3.1/coop_html_editor/static/ckeditor.4.6.2/plugins/clipboard/lang/eu.js` & `coop_html_editor-1.4.1/coop_html_editor/static/ckeditor.4.6.2/plugins/clipboard/lang/eu.js`

 * *Files identical despite different names*

### Comparing `coop_html_editor-1.3.1/coop_html_editor/static/ckeditor.4.6.2/plugins/clipboard/lang/mk.js` & `coop_html_editor-1.4.1/coop_html_editor/static/ckeditor.4.6.2/plugins/clipboard/lang/mk.js`

 * *Files identical despite different names*

### Comparing `coop_html_editor-1.3.1/coop_html_editor/static/ckeditor.4.6.2/plugins/clipboard/lang/no.js` & `coop_html_editor-1.4.1/coop_html_editor/static/ckeditor.4.6.2/plugins/clipboard/lang/no.js`

 * *Files identical despite different names*

### Comparing `coop_html_editor-1.3.1/coop_html_editor/static/ckeditor.4.6.2/plugins/clipboard/lang/sq.js` & `coop_html_editor-1.4.1/coop_html_editor/static/ckeditor.4.6.2/plugins/clipboard/lang/sq.js`

 * *Files identical despite different names*

### Comparing `coop_html_editor-1.3.1/coop_html_editor/static/ckeditor.4.6.2/plugins/clipboard/lang/gu.js` & `coop_html_editor-1.4.1/coop_html_editor/static/ckeditor.4.6.2/plugins/clipboard/lang/gu.js`

 * *Files identical despite different names*

### Comparing `coop_html_editor-1.3.1/coop_html_editor/static/ckeditor.4.6.2/plugins/clipboard/lang/si.js` & `coop_html_editor-1.4.1/coop_html_editor/static/ckeditor.4.6.2/plugins/clipboard/lang/si.js`

 * *Files identical despite different names*

### Comparing `coop_html_editor-1.3.1/coop_html_editor/static/ckeditor.4.6.2/plugins/clipboard/lang/tt.js` & `coop_html_editor-1.4.1/coop_html_editor/static/ckeditor.4.6.2/plugins/clipboard/lang/tt.js`

 * *Files identical despite different names*

### Comparing `coop_html_editor-1.3.1/coop_html_editor/static/ckeditor.4.6.2/plugins/clipboard/lang/ja.js` & `coop_html_editor-1.4.1/coop_html_editor/static/ckeditor.4.6.2/plugins/clipboard/lang/ja.js`

 * *Files identical despite different names*

### Comparing `coop_html_editor-1.3.1/coop_html_editor/static/ckeditor.4.6.2/plugins/clipboard/lang/ka.js` & `coop_html_editor-1.4.1/coop_html_editor/static/ckeditor.4.6.2/plugins/clipboard/lang/ka.js`

 * *Files identical despite different names*

### Comparing `coop_html_editor-1.3.1/coop_html_editor/static/ckeditor.4.6.2/plugins/clipboard/lang/he.js` & `coop_html_editor-1.4.1/coop_html_editor/static/ckeditor.4.6.2/plugins/clipboard/lang/he.js`

 * *Files identical despite different names*

### Comparing `coop_html_editor-1.3.1/coop_html_editor/static/ckeditor.4.6.2/plugins/clipboard/lang/ug.js` & `coop_html_editor-1.4.1/coop_html_editor/static/ckeditor.4.6.2/plugins/clipboard/lang/ug.js`

 * *Files identical despite different names*

### Comparing `coop_html_editor-1.3.1/coop_html_editor/static/ckeditor.4.6.2/plugins/clipboard/lang/bg.js` & `coop_html_editor-1.4.1/coop_html_editor/static/ckeditor.4.6.2/plugins/clipboard/lang/bg.js`

 * *Files identical despite different names*

### Comparing `coop_html_editor-1.3.1/coop_html_editor/static/ckeditor.4.6.2/plugins/clipboard/lang/af.js` & `coop_html_editor-1.4.1/coop_html_editor/static/ckeditor.4.6.2/plugins/clipboard/lang/af.js`

 * *Files identical despite different names*

### Comparing `coop_html_editor-1.3.1/coop_html_editor/static/ckeditor.4.6.2/plugins/clipboard/lang/id.js` & `coop_html_editor-1.4.1/coop_html_editor/static/ckeditor.4.6.2/plugins/clipboard/lang/id.js`

 * *Files identical despite different names*

### Comparing `coop_html_editor-1.3.1/coop_html_editor/static/ckeditor.4.6.2/plugins/clipboard/lang/az.js` & `coop_html_editor-1.4.1/coop_html_editor/static/ckeditor.4.6.2/plugins/clipboard/lang/az.js`

 * *Files identical despite different names*

### Comparing `coop_html_editor-1.3.1/coop_html_editor/static/ckeditor.4.6.2/plugins/clipboard/lang/en-au.js` & `coop_html_editor-1.4.1/coop_html_editor/static/ckeditor.4.6.2/plugins/clipboard/lang/en-au.js`

 * *Files identical despite different names*

### Comparing `coop_html_editor-1.3.1/coop_html_editor/static/ckeditor.4.6.2/plugins/clipboard/lang/ca.js` & `coop_html_editor-1.4.1/coop_html_editor/static/ckeditor.4.6.2/plugins/clipboard/lang/ca.js`

 * *Files identical despite different names*

### Comparing `coop_html_editor-1.3.1/coop_html_editor/static/ckeditor.4.6.2/plugins/clipboard/lang/cy.js` & `coop_html_editor-1.4.1/coop_html_editor/static/ckeditor.4.6.2/plugins/clipboard/lang/cy.js`

 * *Files identical despite different names*

### Comparing `coop_html_editor-1.3.1/coop_html_editor/static/ckeditor.4.6.2/plugins/clipboard/lang/nb.js` & `coop_html_editor-1.4.1/coop_html_editor/static/ckeditor.4.6.2/plugins/clipboard/lang/nb.js`

 * *Files identical despite different names*

### Comparing `coop_html_editor-1.3.1/coop_html_editor/static/ckeditor.4.6.2/plugins/clipboard/lang/zh-cn.js` & `coop_html_editor-1.4.1/coop_html_editor/static/ckeditor.4.6.2/plugins/clipboard/lang/zh-cn.js`

 * *Files identical despite different names*

### Comparing `coop_html_editor-1.3.1/coop_html_editor/static/ckeditor.4.6.2/plugins/clipboard/lang/de-ch.js` & `coop_html_editor-1.4.1/coop_html_editor/static/ckeditor.4.6.2/plugins/clipboard/lang/de-ch.js`

 * *Files identical despite different names*

### Comparing `coop_html_editor-1.3.1/coop_html_editor/static/ckeditor.4.6.2/plugins/clipboard/lang/pt-br.js` & `coop_html_editor-1.4.1/coop_html_editor/static/ckeditor.4.6.2/plugins/clipboard/lang/pt-br.js`

 * *Files identical despite different names*

### Comparing `coop_html_editor-1.3.1/coop_html_editor/static/ckeditor.4.6.2/plugins/clipboard/lang/oc.js` & `coop_html_editor-1.4.1/coop_html_editor/static/ckeditor.4.6.2/plugins/clipboard/lang/oc.js`

 * *Files identical despite different names*

### Comparing `coop_html_editor-1.3.1/coop_html_editor/static/ckeditor.4.6.2/plugins/clipboard/lang/da.js` & `coop_html_editor-1.4.1/coop_html_editor/static/ckeditor.4.6.2/plugins/clipboard/lang/da.js`

 * *Files identical despite different names*

### Comparing `coop_html_editor-1.3.1/coop_html_editor/static/ckeditor.4.6.2/plugins/clipboard/lang/fa.js` & `coop_html_editor-1.4.1/coop_html_editor/static/ckeditor.4.6.2/plugins/clipboard/lang/fa.js`

 * *Files identical despite different names*

### Comparing `coop_html_editor-1.3.1/coop_html_editor/static/ckeditor.4.6.2/plugins/clipboard/lang/de.js` & `coop_html_editor-1.4.1/coop_html_editor/static/ckeditor.4.6.2/plugins/clipboard/lang/de.js`

 * *Files identical despite different names*

### Comparing `coop_html_editor-1.3.1/coop_html_editor/static/ckeditor.4.6.2/plugins/clipboard/lang/en.js` & `coop_html_editor-1.4.1/coop_html_editor/static/ckeditor.4.6.2/plugins/clipboard/lang/en.js`

 * *Files identical despite different names*

### Comparing `coop_html_editor-1.3.1/coop_html_editor/static/ckeditor.4.6.2/plugins/clipboard/lang/bs.js` & `coop_html_editor-1.4.1/coop_html_editor/static/ckeditor.4.6.2/plugins/clipboard/lang/bs.js`

 * *Files identical despite different names*

### Comparing `coop_html_editor-1.3.1/coop_html_editor/static/ckeditor.4.6.2/plugins/clipboard/lang/ku.js` & `coop_html_editor-1.4.1/coop_html_editor/static/ckeditor.4.6.2/plugins/clipboard/lang/ku.js`

 * *Files identical despite different names*

### Comparing `coop_html_editor-1.3.1/coop_html_editor/static/ckeditor.4.6.2/plugins/clipboard/lang/sv.js` & `coop_html_editor-1.4.1/coop_html_editor/static/ckeditor.4.6.2/plugins/clipboard/lang/sv.js`

 * *Files identical despite different names*

### Comparing `coop_html_editor-1.3.1/coop_html_editor/static/ckeditor.4.6.2/plugins/clipboard/lang/zh.js` & `coop_html_editor-1.4.1/coop_html_editor/static/ckeditor.4.6.2/plugins/clipboard/lang/zh.js`

 * *Files identical despite different names*

### Comparing `coop_html_editor-1.3.1/coop_html_editor/static/ckeditor.4.6.2/plugins/clipboard/lang/hi.js` & `coop_html_editor-1.4.1/coop_html_editor/static/ckeditor.4.6.2/plugins/clipboard/lang/hi.js`

 * *Files identical despite different names*

### Comparing `coop_html_editor-1.3.1/coop_html_editor/static/ckeditor.4.6.2/plugins/clipboard/lang/uk.js` & `coop_html_editor-1.4.1/coop_html_editor/static/ckeditor.4.6.2/plugins/clipboard/lang/uk.js`

 * *Files identical despite different names*

### Comparing `coop_html_editor-1.3.1/coop_html_editor/static/ckeditor.4.6.2/plugins/clipboard/lang/cs.js` & `coop_html_editor-1.4.1/coop_html_editor/static/ckeditor.4.6.2/plugins/clipboard/lang/cs.js`

 * *Files identical despite different names*

### Comparing `coop_html_editor-1.3.1/coop_html_editor/static/ckeditor.4.6.2/plugins/clipboard/lang/km.js` & `coop_html_editor-1.4.1/coop_html_editor/static/ckeditor.4.6.2/plugins/clipboard/lang/km.js`

 * *Files identical despite different names*

### Comparing `coop_html_editor-1.3.1/coop_html_editor/static/ckeditor.4.6.2/plugins/clipboard/lang/fr.js` & `coop_html_editor-1.4.1/coop_html_editor/static/ckeditor.4.6.2/plugins/clipboard/lang/fr.js`

 * *Files identical despite different names*

### Comparing `coop_html_editor-1.3.1/coop_html_editor/static/ckeditor.4.6.2/plugins/clipboard/lang/nl.js` & `coop_html_editor-1.4.1/coop_html_editor/static/ckeditor.4.6.2/plugins/clipboard/lang/nl.js`

 * *Files identical despite different names*

### Comparing `coop_html_editor-1.3.1/coop_html_editor/static/ckeditor.4.6.2/plugins/clipboard/lang/fr-ca.js` & `coop_html_editor-1.4.1/coop_html_editor/static/ckeditor.4.6.2/plugins/clipboard/lang/fr-ca.js`

 * *Files identical despite different names*

### Comparing `coop_html_editor-1.3.1/coop_html_editor/static/ckeditor.4.6.2/plugins/clipboard/lang/en-gb.js` & `coop_html_editor-1.4.1/coop_html_editor/static/ckeditor.4.6.2/plugins/clipboard/lang/en-gb.js`

 * *Files identical despite different names*

### Comparing `coop_html_editor-1.3.1/coop_html_editor/static/ckeditor.4.6.2/plugins/clipboard/lang/sr.js` & `coop_html_editor-1.4.1/coop_html_editor/static/ckeditor.4.6.2/plugins/clipboard/lang/sr.js`

 * *Files identical despite different names*

### Comparing `coop_html_editor-1.3.1/coop_html_editor/static/ckeditor.4.6.2/plugins/clipboard/lang/hu.js` & `coop_html_editor-1.4.1/coop_html_editor/static/ckeditor.4.6.2/plugins/clipboard/lang/hu.js`

 * *Files identical despite different names*

### Comparing `coop_html_editor-1.3.1/coop_html_editor/static/ckeditor.4.6.2/plugins/clipboard/lang/lt.js` & `coop_html_editor-1.4.1/coop_html_editor/static/ckeditor.4.6.2/plugins/clipboard/lang/lt.js`

 * *Files identical despite different names*

### Comparing `coop_html_editor-1.3.1/coop_html_editor/static/ckeditor.4.6.2/plugins/clipboard/lang/fo.js` & `coop_html_editor-1.4.1/coop_html_editor/static/ckeditor.4.6.2/plugins/clipboard/lang/fo.js`

 * *Files identical despite different names*

### Comparing `coop_html_editor-1.3.1/coop_html_editor/static/ckeditor.4.6.2/plugins/clipboard/lang/ar.js` & `coop_html_editor-1.4.1/coop_html_editor/static/ckeditor.4.6.2/plugins/clipboard/lang/ar.js`

 * *Files identical despite different names*

### Comparing `coop_html_editor-1.3.1/coop_html_editor/static/ckeditor.4.6.2/plugins/clipboard/lang/sk.js` & `coop_html_editor-1.4.1/coop_html_editor/static/ckeditor.4.6.2/plugins/clipboard/lang/sk.js`

 * *Files identical despite different names*

### Comparing `coop_html_editor-1.3.1/coop_html_editor/static/ckeditor.4.6.2/plugins/clipboard/lang/it.js` & `coop_html_editor-1.4.1/coop_html_editor/static/ckeditor.4.6.2/plugins/clipboard/lang/it.js`

 * *Files identical despite different names*

### Comparing `coop_html_editor-1.3.1/coop_html_editor/static/ckeditor.4.6.2/plugins/clipboard/lang/es.js` & `coop_html_editor-1.4.1/coop_html_editor/static/ckeditor.4.6.2/plugins/clipboard/lang/es.js`

 * *Files identical despite different names*

### Comparing `coop_html_editor-1.3.1/coop_html_editor/static/ckeditor.4.6.2/plugins/clipboard/lang/bn.js` & `coop_html_editor-1.4.1/coop_html_editor/static/ckeditor.4.6.2/plugins/clipboard/lang/bn.js`

 * *Files identical despite different names*

### Comparing `coop_html_editor-1.3.1/coop_html_editor/static/ckeditor.4.6.2/plugins/clipboard/lang/eo.js` & `coop_html_editor-1.4.1/coop_html_editor/static/ckeditor.4.6.2/plugins/clipboard/lang/eo.js`

 * *Files identical despite different names*

### Comparing `coop_html_editor-1.3.1/coop_html_editor/static/ckeditor.4.6.2/plugins/clipboard/lang/ro.js` & `coop_html_editor-1.4.1/coop_html_editor/static/ckeditor.4.6.2/plugins/clipboard/lang/ro.js`

 * *Files identical despite different names*

### Comparing `coop_html_editor-1.3.1/coop_html_editor/static/ckeditor.4.6.2/plugins/clipboard/lang/tr.js` & `coop_html_editor-1.4.1/coop_html_editor/static/ckeditor.4.6.2/plugins/clipboard/lang/tr.js`

 * *Files identical despite different names*

### Comparing `coop_html_editor-1.3.1/coop_html_editor/static/ckeditor.4.6.2/plugins/clipboard/dialogs/paste.js` & `coop_html_editor-1.4.1/coop_html_editor/static/ckeditor.4.6.2/plugins/clipboard/dialogs/paste.js`

 * *Files identical despite different names*

### Comparing `coop_html_editor-1.3.1/coop_html_editor/static/ckeditor.4.6.2/plugins/clipboard/dev/console.js` & `coop_html_editor-1.4.1/coop_html_editor/static/ckeditor.4.6.2/plugins/clipboard/dev/console.js`

 * *Files identical despite different names*

### Comparing `coop_html_editor-1.3.1/coop_html_editor/static/ckeditor.4.6.2/plugins/clipboard/dev/dnd.html` & `coop_html_editor-1.4.1/coop_html_editor/static/ckeditor.4.6.2/plugins/clipboard/dev/dnd.html`

 * *Files identical despite different names*

### Comparing `coop_html_editor-1.3.1/coop_html_editor/static/ckeditor.4.6.2/plugins/clipboard/dev/clipboard.html` & `coop_html_editor-1.4.1/coop_html_editor/static/ckeditor.4.6.2/plugins/clipboard/dev/clipboard.html`

 * *Files identical despite different names*

### Comparing `coop_html_editor-1.3.1/coop_html_editor/static/ckeditor.4.6.2/plugins/clipboard/plugin.js` & `coop_html_editor-1.4.1/coop_html_editor/static/ckeditor.4.6.2/plugins/clipboard/plugin.js`

 * *Files identical despite different names*

### Comparing `coop_html_editor-1.3.1/coop_html_editor/static/ckeditor.4.6.2/contents.css` & `coop_html_editor-1.4.1/coop_html_editor/static/ckeditor.4.6.2/contents.css`

 * *Files identical despite different names*

### Comparing `coop_html_editor-1.3.1/coop_html_editor/static/ckeditor.4.6.2/skins/moono-lisa/editor_iequirks.css` & `coop_html_editor-1.4.1/coop_html_editor/static/ckeditor.4.6.2/skins/moono-lisa/editor_iequirks.css`

 * *Files identical despite different names*

### Comparing `coop_html_editor-1.3.1/coop_html_editor/static/ckeditor.4.6.2/skins/moono-lisa/editor.css` & `coop_html_editor-1.4.1/coop_html_editor/static/ckeditor.4.6.2/skins/moono-lisa/editor.css`

 * *Files identical despite different names*

### Comparing `coop_html_editor-1.3.1/coop_html_editor/static/ckeditor.4.6.2/skins/moono-lisa/images/spinner.gif` & `coop_html_editor-1.4.1/coop_html_editor/static/ckeditor.4.6.2/skins/moono-lisa/images/spinner.gif`

 * *Files identical despite different names*

### Comparing `coop_html_editor-1.3.1/coop_html_editor/static/ckeditor.4.6.2/skins/moono-lisa/images/hidpi/lock.png` & `coop_html_editor-1.4.1/coop_html_editor/static/ckeditor.4.6.2/skins/moono-lisa/images/hidpi/lock.png`

 * *Files identical despite different names*

### Comparing `coop_html_editor-1.3.1/coop_html_editor/static/ckeditor.4.6.2/skins/moono-lisa/images/hidpi/lock-open.png` & `coop_html_editor-1.4.1/coop_html_editor/static/ckeditor.4.6.2/skins/moono-lisa/images/hidpi/lock-open.png`

 * *Files identical despite different names*

### Comparing `coop_html_editor-1.3.1/coop_html_editor/static/ckeditor.4.6.2/skins/moono-lisa/images/hidpi/refresh.png` & `coop_html_editor-1.4.1/coop_html_editor/static/ckeditor.4.6.2/skins/moono-lisa/images/hidpi/refresh.png`

 * *Files identical despite different names*

### Comparing `coop_html_editor-1.3.1/coop_html_editor/static/ckeditor.4.6.2/skins/moono-lisa/images/hidpi/close.png` & `coop_html_editor-1.4.1/coop_html_editor/static/ckeditor.4.6.2/skins/moono-lisa/images/hidpi/close.png`

 * *Files identical despite different names*

### Comparing `coop_html_editor-1.3.1/coop_html_editor/static/ckeditor.4.6.2/skins/moono-lisa/images/refresh.png` & `coop_html_editor-1.4.1/coop_html_editor/static/ckeditor.4.6.2/skins/moono-lisa/images/refresh.png`

 * *Files identical despite different names*

### Comparing `coop_html_editor-1.3.1/coop_html_editor/static/ckeditor.4.6.2/skins/moono-lisa/images/close.png` & `coop_html_editor-1.4.1/coop_html_editor/static/ckeditor.4.6.2/skins/moono-lisa/images/close.png`

 * *Files identical despite different names*

### Comparing `coop_html_editor-1.3.1/coop_html_editor/static/ckeditor.4.6.2/skins/moono-lisa/editor_ie.css` & `coop_html_editor-1.4.1/coop_html_editor/static/ckeditor.4.6.2/skins/moono-lisa/editor_ie.css`

 * *Files identical despite different names*

### Comparing `coop_html_editor-1.3.1/coop_html_editor/static/ckeditor.4.6.2/skins/moono-lisa/editor_ie8.css` & `coop_html_editor-1.4.1/coop_html_editor/static/ckeditor.4.6.2/skins/moono-lisa/editor_ie8.css`

 * *Files identical despite different names*

### Comparing `coop_html_editor-1.3.1/coop_html_editor/static/ckeditor.4.6.2/skins/moono-lisa/dialog_iequirks.css` & `coop_html_editor-1.4.1/coop_html_editor/static/ckeditor.4.6.2/skins/moono-lisa/dialog_iequirks.css`

 * *Files identical despite different names*

### Comparing `coop_html_editor-1.3.1/coop_html_editor/static/ckeditor.4.6.2/skins/moono-lisa/readme.md` & `coop_html_editor-1.4.1/coop_html_editor/static/ckeditor.4.6.2/skins/moono-lisa/readme.md`

 * *Files identical despite different names*

### Comparing `coop_html_editor-1.3.1/coop_html_editor/static/ckeditor.4.6.2/skins/moono-lisa/icons.png` & `coop_html_editor-1.4.1/coop_html_editor/static/ckeditor.4.6.2/skins/moono-lisa/icons.png`

 * *Files identical despite different names*

### Comparing `coop_html_editor-1.3.1/coop_html_editor/static/ckeditor.4.6.2/skins/moono-lisa/editor_gecko.css` & `coop_html_editor-1.4.1/coop_html_editor/static/ckeditor.4.6.2/skins/moono-lisa/editor_gecko.css`

 * *Files identical despite different names*

### Comparing `coop_html_editor-1.3.1/coop_html_editor/static/ckeditor.4.6.2/skins/moono-lisa/dialog_ie.css` & `coop_html_editor-1.4.1/coop_html_editor/static/ckeditor.4.6.2/skins/moono-lisa/dialog_ie.css`

 * *Files identical despite different names*

### Comparing `coop_html_editor-1.3.1/coop_html_editor/static/ckeditor.4.6.2/skins/moono-lisa/dialog.css` & `coop_html_editor-1.4.1/coop_html_editor/static/ckeditor.4.6.2/skins/moono-lisa/dialog.css`

 * *Files identical despite different names*

### Comparing `coop_html_editor-1.3.1/coop_html_editor/static/ckeditor.4.6.2/skins/moono-lisa/icons_hidpi.png` & `coop_html_editor-1.4.1/coop_html_editor/static/ckeditor.4.6.2/skins/moono-lisa/icons_hidpi.png`

 * *Files identical despite different names*

### Comparing `coop_html_editor-1.3.1/coop_html_editor/static/ckeditor.4.6.2/skins/moono-lisa/dialog_ie8.css` & `coop_html_editor-1.4.1/coop_html_editor/static/ckeditor.4.6.2/skins/moono-lisa/dialog_ie8.css`

 * *Files identical despite different names*

### Comparing `coop_html_editor-1.3.1/coop_html_editor/static/ckeditor.4.6.2/config.js` & `coop_html_editor-1.4.1/coop_html_editor/static/ckeditor.4.6.2/config.js`

 * *Files identical despite different names*

### Comparing `coop_html_editor-1.3.1/coop_html_editor/static/ckeditor.4.6.2/ckeditor.js` & `coop_html_editor-1.4.1/coop_html_editor/static/ckeditor.4.6.2/ckeditor.js`

 * *Files identical despite different names*

### Comparing `coop_html_editor-1.3.1/coop_html_editor/static/ckeditor.4.6.2/README.md` & `coop_html_editor-1.4.1/coop_html_editor/static/ckeditor.4.6.2/README.md`

 * *Files identical despite different names*

### Comparing `coop_html_editor-1.3.1/coop_html_editor/static/ckeditor.4.6.2/lang/en.js` & `coop_html_editor-1.4.1/coop_html_editor/static/ckeditor.4.6.2/lang/en.js`

 * *Files identical despite different names*

### Comparing `coop_html_editor-1.3.1/coop_html_editor/static/ckeditor.4.6.2/lang/fr.js` & `coop_html_editor-1.4.1/coop_html_editor/static/ckeditor.4.6.2/lang/fr.js`

 * *Files identical despite different names*

### Comparing `coop_html_editor-1.3.1/coop_html_editor/static/ckeditor.4.6.2/samples/index.html` & `coop_html_editor-1.4.1/coop_html_editor/static/ckeditor.4.6.2/samples/index.html`

 * *Files identical despite different names*

### Comparing `coop_html_editor-1.3.1/coop_html_editor/static/ckeditor.4.6.2/samples/css/samples.css` & `coop_html_editor-1.4.1/coop_html_editor/static/ckeditor.4.6.2/samples/css/samples.css`

 * *Files identical despite different names*

### Comparing `coop_html_editor-1.3.1/coop_html_editor/static/ckeditor.4.6.2/samples/js/sf.js` & `coop_html_editor-1.4.1/coop_html_editor/static/ckeditor.4.6.2/samples/js/sf.js`

 * *Files identical despite different names*

### Comparing `coop_html_editor-1.3.1/coop_html_editor/static/ckeditor.4.6.2/samples/js/sample.js` & `coop_html_editor-1.4.1/coop_html_editor/static/ckeditor.4.6.2/samples/js/sample.js`

 * *Files identical despite different names*

### Comparing `coop_html_editor-1.3.1/coop_html_editor/static/ckeditor.4.6.2/samples/old/xhtmlstyle.html` & `coop_html_editor-1.4.1/coop_html_editor/static/ckeditor.4.6.2/samples/old/xhtmlstyle.html`

 * *Files identical despite different names*

### Comparing `coop_html_editor-1.3.1/coop_html_editor/static/ckeditor.4.6.2/samples/old/index.html` & `coop_html_editor-1.4.1/coop_html_editor/static/ckeditor.4.6.2/samples/old/index.html`

 * *Files identical despite different names*

### Comparing `coop_html_editor-1.3.1/coop_html_editor/static/ckeditor.4.6.2/samples/old/magicline/magicline.html` & `coop_html_editor-1.4.1/coop_html_editor/static/ckeditor.4.6.2/samples/old/magicline/magicline.html`

 * *Files identical despite different names*

### Comparing `coop_html_editor-1.3.1/coop_html_editor/static/ckeditor.4.6.2/samples/old/tabindex.html` & `coop_html_editor-1.4.1/coop_html_editor/static/ckeditor.4.6.2/samples/old/tabindex.html`

 * *Files identical despite different names*

### Comparing `coop_html_editor-1.3.1/coop_html_editor/static/ckeditor.4.6.2/samples/old/toolbar/toolbar.html` & `coop_html_editor-1.4.1/coop_html_editor/static/ckeditor.4.6.2/samples/old/toolbar/toolbar.html`

 * *Files identical despite different names*

### Comparing `coop_html_editor-1.3.1/coop_html_editor/static/ckeditor.4.6.2/samples/old/appendto.html` & `coop_html_editor-1.4.1/coop_html_editor/static/ckeditor.4.6.2/samples/old/appendto.html`

 * *Files identical despite different names*

### Comparing `coop_html_editor-1.3.1/coop_html_editor/static/ckeditor.4.6.2/samples/old/divreplace.html` & `coop_html_editor-1.4.1/coop_html_editor/static/ckeditor.4.6.2/samples/old/divreplace.html`

 * *Files identical despite different names*

### Comparing `coop_html_editor-1.3.1/coop_html_editor/static/ckeditor.4.6.2/samples/old/jquery.html` & `coop_html_editor-1.4.1/coop_html_editor/static/ckeditor.4.6.2/samples/old/jquery.html`

 * *Files identical despite different names*

### Comparing `coop_html_editor-1.3.1/coop_html_editor/static/ckeditor.4.6.2/samples/old/inlineall.html` & `coop_html_editor-1.4.1/coop_html_editor/static/ckeditor.4.6.2/samples/old/inlineall.html`

 * *Files identical despite different names*

### Comparing `coop_html_editor-1.3.1/coop_html_editor/static/ckeditor.4.6.2/samples/old/wysiwygarea/fullpage.html` & `coop_html_editor-1.4.1/coop_html_editor/static/ckeditor.4.6.2/samples/old/wysiwygarea/fullpage.html`

 * *Files identical despite different names*

### Comparing `coop_html_editor-1.3.1/coop_html_editor/static/ckeditor.4.6.2/samples/old/htmlwriter/outputhtml.html` & `coop_html_editor-1.4.1/coop_html_editor/static/ckeditor.4.6.2/samples/old/htmlwriter/outputhtml.html`

 * *Files identical despite different names*

### Comparing `coop_html_editor-1.3.1/coop_html_editor/static/ckeditor.4.6.2/samples/old/htmlwriter/outputforflash.html` & `coop_html_editor-1.4.1/coop_html_editor/static/ckeditor.4.6.2/samples/old/htmlwriter/outputforflash.html`

 * *Files identical despite different names*

### Comparing `coop_html_editor-1.3.1/coop_html_editor/static/ckeditor.4.6.2/samples/old/htmlwriter/assets/outputforflash/swfobject.js` & `coop_html_editor-1.4.1/coop_html_editor/static/ckeditor.4.6.2/samples/old/htmlwriter/assets/outputforflash/swfobject.js`

 * *Files identical despite different names*

### Comparing `coop_html_editor-1.3.1/coop_html_editor/static/ckeditor.4.6.2/samples/old/htmlwriter/assets/outputforflash/outputforflash.swf` & `coop_html_editor-1.4.1/coop_html_editor/static/ckeditor.4.6.2/samples/old/htmlwriter/assets/outputforflash/outputforflash.swf`

 * *Files identical despite different names*

### Comparing `coop_html_editor-1.3.1/coop_html_editor/static/ckeditor.4.6.2/samples/old/htmlwriter/assets/outputforflash/outputforflash.fla` & `coop_html_editor-1.4.1/coop_html_editor/static/ckeditor.4.6.2/samples/old/htmlwriter/assets/outputforflash/outputforflash.fla`

 * *Files identical despite different names*

### Comparing `coop_html_editor-1.3.1/coop_html_editor/static/ckeditor.4.6.2/samples/old/dialog/dialog.html` & `coop_html_editor-1.4.1/coop_html_editor/static/ckeditor.4.6.2/samples/old/dialog/dialog.html`

 * *Files identical despite different names*

### Comparing `coop_html_editor-1.3.1/coop_html_editor/static/ckeditor.4.6.2/samples/old/dialog/assets/my_dialog.js` & `coop_html_editor-1.4.1/coop_html_editor/static/ckeditor.4.6.2/samples/old/dialog/assets/my_dialog.js`

 * *Files identical despite different names*

### Comparing `coop_html_editor-1.3.1/coop_html_editor/static/ckeditor.4.6.2/samples/old/inlinetextarea.html` & `coop_html_editor-1.4.1/coop_html_editor/static/ckeditor.4.6.2/samples/old/inlinetextarea.html`

 * *Files identical despite different names*

### Comparing `coop_html_editor-1.3.1/coop_html_editor/static/ckeditor.4.6.2/samples/old/replacebyclass.html` & `coop_html_editor-1.4.1/coop_html_editor/static/ckeditor.4.6.2/samples/old/replacebyclass.html`

 * *Files identical despite different names*

### Comparing `coop_html_editor-1.3.1/coop_html_editor/static/ckeditor.4.6.2/samples/old/sample_posteddata.php` & `coop_html_editor-1.4.1/coop_html_editor/static/ckeditor.4.6.2/samples/old/sample_posteddata.php`

 * *Files identical despite different names*

### Comparing `coop_html_editor-1.3.1/coop_html_editor/static/ckeditor.4.6.2/samples/old/datafiltering.html` & `coop_html_editor-1.4.1/coop_html_editor/static/ckeditor.4.6.2/samples/old/datafiltering.html`

 * *Files identical despite different names*

### Comparing `coop_html_editor-1.3.1/coop_html_editor/static/ckeditor.4.6.2/samples/old/replacebycode.html` & `coop_html_editor-1.4.1/coop_html_editor/static/ckeditor.4.6.2/samples/old/replacebycode.html`

 * *Files identical despite different names*

### Comparing `coop_html_editor-1.3.1/coop_html_editor/static/ckeditor.4.6.2/samples/old/uilanguages.html` & `coop_html_editor-1.4.1/coop_html_editor/static/ckeditor.4.6.2/samples/old/uilanguages.html`

 * *Files identical despite different names*

### Comparing `coop_html_editor-1.3.1/coop_html_editor/static/ckeditor.4.6.2/samples/old/ajax.html` & `coop_html_editor-1.4.1/coop_html_editor/static/ckeditor.4.6.2/samples/old/ajax.html`

 * *Files identical despite different names*

### Comparing `coop_html_editor-1.3.1/coop_html_editor/static/ckeditor.4.6.2/samples/old/enterkey/enterkey.html` & `coop_html_editor-1.4.1/coop_html_editor/static/ckeditor.4.6.2/samples/old/enterkey/enterkey.html`

 * *Files identical despite different names*

### Comparing `coop_html_editor-1.3.1/coop_html_editor/static/ckeditor.4.6.2/samples/old/api.html` & `coop_html_editor-1.4.1/coop_html_editor/static/ckeditor.4.6.2/samples/old/api.html`

 * *Files identical despite different names*

### Comparing `coop_html_editor-1.3.1/coop_html_editor/static/ckeditor.4.6.2/samples/old/inlinebycode.html` & `coop_html_editor-1.4.1/coop_html_editor/static/ckeditor.4.6.2/samples/old/inlinebycode.html`

 * *Files identical despite different names*

### Comparing `coop_html_editor-1.3.1/coop_html_editor/static/ckeditor.4.6.2/samples/old/assets/uilanguages/languages.js` & `coop_html_editor-1.4.1/coop_html_editor/static/ckeditor.4.6.2/samples/old/assets/uilanguages/languages.js`

 * *Files identical despite different names*

### Comparing `coop_html_editor-1.3.1/coop_html_editor/static/ckeditor.4.6.2/samples/old/assets/posteddata.php` & `coop_html_editor-1.4.1/coop_html_editor/static/ckeditor.4.6.2/samples/old/assets/posteddata.php`

 * *Files identical despite different names*

### Comparing `coop_html_editor-1.3.1/coop_html_editor/static/ckeditor.4.6.2/samples/old/assets/outputxhtml/outputxhtml.css` & `coop_html_editor-1.4.1/coop_html_editor/static/ckeditor.4.6.2/samples/old/assets/outputxhtml/outputxhtml.css`

 * *Files identical despite different names*

### Comparing `coop_html_editor-1.3.1/coop_html_editor/static/ckeditor.4.6.2/samples/old/assets/sample.jpg` & `coop_html_editor-1.4.1/coop_html_editor/static/ckeditor.4.6.2/samples/old/assets/sample.jpg`

 * *Files identical despite different names*

### Comparing `coop_html_editor-1.3.1/coop_html_editor/static/ckeditor.4.6.2/samples/old/assets/inlineall/logo.png` & `coop_html_editor-1.4.1/coop_html_editor/static/ckeditor.4.6.2/samples/old/assets/inlineall/logo.png`

 * *Files identical despite different names*

### Comparing `coop_html_editor-1.3.1/coop_html_editor/static/ckeditor.4.6.2/samples/old/sample.js` & `coop_html_editor-1.4.1/coop_html_editor/static/ckeditor.4.6.2/samples/old/sample.js`

 * *Files identical despite different names*

### Comparing `coop_html_editor-1.3.1/coop_html_editor/static/ckeditor.4.6.2/samples/old/sample.css` & `coop_html_editor-1.4.1/coop_html_editor/static/ckeditor.4.6.2/samples/old/sample.css`

 * *Files identical despite different names*

### Comparing `coop_html_editor-1.3.1/coop_html_editor/static/ckeditor.4.6.2/samples/old/uicolor.html` & `coop_html_editor-1.4.1/coop_html_editor/static/ckeditor.4.6.2/samples/old/uicolor.html`

 * *Files identical despite different names*

### Comparing `coop_html_editor-1.3.1/coop_html_editor/static/ckeditor.4.6.2/samples/old/readonly.html` & `coop_html_editor-1.4.1/coop_html_editor/static/ckeditor.4.6.2/samples/old/readonly.html`

 * *Files identical despite different names*

### Comparing `coop_html_editor-1.3.1/coop_html_editor/static/ckeditor.4.6.2/samples/img/logo.png` & `coop_html_editor-1.4.1/coop_html_editor/static/ckeditor.4.6.2/samples/img/logo.png`

 * *Files identical despite different names*

### Comparing `coop_html_editor-1.3.1/coop_html_editor/static/ckeditor.4.6.2/samples/img/header-bg.png` & `coop_html_editor-1.4.1/coop_html_editor/static/ckeditor.4.6.2/samples/img/header-bg.png`

 * *Files identical despite different names*

### Comparing `coop_html_editor-1.3.1/coop_html_editor/static/ckeditor.4.6.2/samples/img/navigation-tip.png` & `coop_html_editor-1.4.1/coop_html_editor/static/ckeditor.4.6.2/samples/img/navigation-tip.png`

 * *Files identical despite different names*

### Comparing `coop_html_editor-1.3.1/coop_html_editor/static/ckeditor.4.6.2/samples/toolbarconfigurator/index.html` & `coop_html_editor-1.4.1/coop_html_editor/static/ckeditor.4.6.2/samples/toolbarconfigurator/index.html`

 * *Files identical despite different names*

### Comparing `coop_html_editor-1.3.1/coop_html_editor/static/ckeditor.4.6.2/samples/toolbarconfigurator/css/fontello.css` & `coop_html_editor-1.4.1/coop_html_editor/static/ckeditor.4.6.2/samples/toolbarconfigurator/css/fontello.css`

 * *Files identical despite different names*

### Comparing `coop_html_editor-1.3.1/coop_html_editor/static/ckeditor.4.6.2/samples/toolbarconfigurator/js/fulltoolbareditor.js` & `coop_html_editor-1.4.1/coop_html_editor/static/ckeditor.4.6.2/samples/toolbarconfigurator/js/fulltoolbareditor.js`

 * *Files identical despite different names*

### Comparing `coop_html_editor-1.3.1/coop_html_editor/static/ckeditor.4.6.2/samples/toolbarconfigurator/js/abstracttoolbarmodifier.js` & `coop_html_editor-1.4.1/coop_html_editor/static/ckeditor.4.6.2/samples/toolbarconfigurator/js/abstracttoolbarmodifier.js`

 * *Files identical despite different names*

### Comparing `coop_html_editor-1.3.1/coop_html_editor/static/ckeditor.4.6.2/samples/toolbarconfigurator/js/toolbartextmodifier.js` & `coop_html_editor-1.4.1/coop_html_editor/static/ckeditor.4.6.2/samples/toolbarconfigurator/js/toolbartextmodifier.js`

 * *Files identical despite different names*

### Comparing `coop_html_editor-1.3.1/coop_html_editor/static/ckeditor.4.6.2/samples/toolbarconfigurator/js/toolbarmodifier.js` & `coop_html_editor-1.4.1/coop_html_editor/static/ckeditor.4.6.2/samples/toolbarconfigurator/js/toolbarmodifier.js`

 * *Files identical despite different names*

### Comparing `coop_html_editor-1.3.1/coop_html_editor/static/ckeditor.4.6.2/samples/toolbarconfigurator/lib/codemirror/neo.css` & `coop_html_editor-1.4.1/coop_html_editor/static/ckeditor.4.6.2/samples/toolbarconfigurator/lib/codemirror/neo.css`

 * *Files identical despite different names*

### Comparing `coop_html_editor-1.3.1/coop_html_editor/static/ckeditor.4.6.2/samples/toolbarconfigurator/lib/codemirror/show-hint.css` & `coop_html_editor-1.4.1/coop_html_editor/static/ckeditor.4.6.2/samples/toolbarconfigurator/lib/codemirror/show-hint.css`

 * *Files identical despite different names*

### Comparing `coop_html_editor-1.3.1/coop_html_editor/static/ckeditor.4.6.2/samples/toolbarconfigurator/lib/codemirror/codemirror.js` & `coop_html_editor-1.4.1/coop_html_editor/static/ckeditor.4.6.2/samples/toolbarconfigurator/lib/codemirror/codemirror.js`

 * *Files identical despite different names*

### Comparing `coop_html_editor-1.3.1/coop_html_editor/static/ckeditor.4.6.2/samples/toolbarconfigurator/lib/codemirror/LICENSE` & `coop_html_editor-1.4.1/coop_html_editor/static/ckeditor.4.6.2/samples/toolbarconfigurator/lib/codemirror/LICENSE`

 * *Files identical despite different names*

### Comparing `coop_html_editor-1.3.1/coop_html_editor/static/ckeditor.4.6.2/samples/toolbarconfigurator/lib/codemirror/codemirror.css` & `coop_html_editor-1.4.1/coop_html_editor/static/ckeditor.4.6.2/samples/toolbarconfigurator/lib/codemirror/codemirror.css`

 * *Files identical despite different names*

### Comparing `coop_html_editor-1.3.1/coop_html_editor/static/ckeditor.4.6.2/samples/toolbarconfigurator/lib/codemirror/show-hint.js` & `coop_html_editor-1.4.1/coop_html_editor/static/ckeditor.4.6.2/samples/toolbarconfigurator/lib/codemirror/show-hint.js`

 * *Files identical despite different names*

### Comparing `coop_html_editor-1.3.1/coop_html_editor/static/ckeditor.4.6.2/samples/toolbarconfigurator/lib/codemirror/javascript.js` & `coop_html_editor-1.4.1/coop_html_editor/static/ckeditor.4.6.2/samples/toolbarconfigurator/lib/codemirror/javascript.js`

 * *Files identical despite different names*

### Comparing `coop_html_editor-1.3.1/coop_html_editor/static/ckeditor.4.6.2/samples/toolbarconfigurator/font/fontello.ttf` & `coop_html_editor-1.4.1/coop_html_editor/static/ckeditor.4.6.2/samples/toolbarconfigurator/font/fontello.ttf`

 * *Files identical despite different names*

### Comparing `coop_html_editor-1.3.1/coop_html_editor/static/ckeditor.4.6.2/samples/toolbarconfigurator/font/fontello.woff` & `coop_html_editor-1.4.1/coop_html_editor/static/ckeditor.4.6.2/samples/toolbarconfigurator/font/fontello.woff`

 * *Files identical despite different names*

### Comparing `coop_html_editor-1.3.1/coop_html_editor/static/ckeditor.4.6.2/samples/toolbarconfigurator/font/config.json` & `coop_html_editor-1.4.1/coop_html_editor/static/ckeditor.4.6.2/samples/toolbarconfigurator/font/config.json`

 * *Files identical despite different names*

### Comparing `coop_html_editor-1.3.1/coop_html_editor/static/ckeditor.4.6.2/samples/toolbarconfigurator/font/fontello.eot` & `coop_html_editor-1.4.1/coop_html_editor/static/ckeditor.4.6.2/samples/toolbarconfigurator/font/fontello.eot`

 * *Files identical despite different names*

### Comparing `coop_html_editor-1.3.1/coop_html_editor/static/ckeditor.4.6.2/samples/toolbarconfigurator/font/fontello.svg` & `coop_html_editor-1.4.1/coop_html_editor/static/ckeditor.4.6.2/samples/toolbarconfigurator/font/fontello.svg`

 * *Files identical despite different names*

### Comparing `coop_html_editor-1.3.1/coop_html_editor/static/ckeditor.4.6.2/adapters/jquery.js` & `coop_html_editor-1.4.1/coop_html_editor/static/ckeditor.4.6.2/adapters/jquery.js`

 * *Files identical despite different names*

### Comparing `coop_html_editor-1.3.1/coop_html_editor/static/ckeditor.4.6.2/CHANGES.md` & `coop_html_editor-1.4.1/coop_html_editor/static/ckeditor.4.6.2/CHANGES.md`

 * *Files identical despite different names*

### Comparing `coop_html_editor-1.3.1/coop_html_editor/static/ckeditor.4.6.2/build-config.js` & `coop_html_editor-1.4.1/coop_html_editor/static/ckeditor.4.6.2/build-config.js`

 * *Files identical despite different names*

### Comparing `coop_html_editor-1.3.1/coop_html_editor/static/ckeditor.4.6.2/styles.js` & `coop_html_editor-1.4.1/coop_html_editor/static/ckeditor.4.6.2/styles.js`

 * *Files identical despite different names*

### Comparing `coop_html_editor-1.3.1/coop_html_editor/static/js/jquery-1.7.2.min.js` & `coop_html_editor-1.4.1/coop_html_editor/static/js/jquery-1.7.2.min.js`

 * *Files identical despite different names*

### Comparing `coop_html_editor-1.3.1/coop_html_editor/static/js/jquery-1.7.2.js` & `coop_html_editor-1.4.1/coop_html_editor/static/js/jquery-1.7.2.js`

 * *Files identical despite different names*

### Comparing `coop_html_editor-1.3.1/coop_html_editor/templates/html_editor/image_browser.html` & `coop_html_editor-1.4.1/coop_html_editor/templates/html_editor/image_browser.html`

 * *Files identical despite different names*

### Comparing `coop_html_editor-1.3.1/coop_html_editor/templates/html_editor/link_browser.html` & `coop_html_editor-1.4.1/coop_html_editor/templates/html_editor/link_browser.html`

 * *Files identical despite different names*

### Comparing `coop_html_editor-1.3.1/coop_html_editor/templates/html_editor/ckeditor_config.js` & `coop_html_editor-1.4.1/coop_html_editor/templates/html_editor/ckeditor_config.js`

 * *Files 13% similar despite different names*

#### js-beautify {}

```diff
@@ -47,10 +47,10 @@
     config.extraPlugins = 'sourcedialog,embed,btgrid,videoembed';
 
     // Simplify the dialog windows.
     config.removeDialogTabs = 'image:advanced;link:advanced';
 
     config.stylesSet = 'cms_styles';
 
-    config.extraAllowedContent = 'img[*](*);video[*](*);video source[*](*)';
-
+    config.extraAllowedContent = 'i[*](*);img[*](*);video[*](*);video source[*](*)';
+    config.allowedContent = true;
 };
```

### Comparing `coop_html_editor-1.3.1/coop_html_editor/templates/html_editor/ckeditor-init.js` & `coop_html_editor-1.4.1/coop_html_editor/templates/html_editor/ckeditor-init.js`

 * *Files 2% similar despite different names*

#### js-beautify {}

```diff
@@ -1,9 +1,9 @@
 CKEDITOR.disableAutoInline = true;
-
+CKEDITOR.dtd.$removeEmpty.i = 0;
 /**
  *
  * Transform images and document links when dropped in editor from media-library
  *
  */
 var adaptDroppedElement = function() {
```

### Comparing `coop_html_editor-1.3.1/coop_html_editor/views.py` & `coop_html_editor-1.4.1/coop_html_editor/views.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,38 +1,32 @@
 # -*- coding: utf-8 -*-
 """view for aloha editor"""
 
 from django.shortcuts import render
 
 from . import settings
-from .utils import get_model
+from django.apps import apps
 
 from coop_cms.utils import paginate
 
 
 def html_editor_init(request):
     """
     Build the javascript file which is initializing the aloha-editor
     Run the javascript code for the AlohaInput widget
     """
     
     links = []
     for full_model_name in settings.link_models():
         app_name, model_name = full_model_name.split('.')
-        model = get_model(app_name, model_name)
+        model = apps.get_model(app_name, model_name)
         if model:
             links.extend(model.objects.all())
 
     editors_config = {
-        'aloha': {
-            'jquery_no_conflict': settings.jquery_no_conflict(),
-            'sidebar_disabled': 'true' if settings.sidebar_disabled() else 'false',
-            'css_classes': settings.css_classes(),
-            'resize_disabled': settings.resize_disabled(),
-        },
         'ck-editor': {
             'css_classes': settings.css_classes(),
             'image_default_class': settings.image_default_class(),
         }
     }
 
     editor_name = settings.get_html_editor()
@@ -61,15 +55,15 @@
 
 def browser_urls(request):
     """display link browser"""
 
     links = []
     for full_model_name in settings.link_models():
         app_name, model_name = full_model_name.split('.')
-        model = get_model(app_name, model_name)
+        model = apps.get_model(app_name, model_name)
         if model:
             links.extend(model.objects.all().order_by("-id"))
 
     page_obj = paginate(request, links, 10)
     
     context = {
         'links': links,
@@ -86,15 +80,15 @@
 
 def browser_images(request):
     """display image browser"""
 
     images = []
     for full_model_name in settings.image_models():
         app_name, model_name = full_model_name.split('.')
-        model = get_model(app_name, model_name)
+        model = apps.get_model(app_name, model_name)
         if model:
             images.extend(model.objects.all().order_by("-id"))
 
     page_obj = paginate(request, images, 20)
     
     context = {
         'images': images,
@@ -102,8 +96,8 @@
         'page_obj': page_obj
     }
 
     return render(
         request,
         'html_editor/image_browser.html',
         context
-    )
+    )
```

### Comparing `coop_html_editor-1.3.1/setup.py` & `coop_html_editor-1.4.1/setup.py`

 * *Files identical despite different names*

### Comparing `coop_html_editor-1.3.1/README.rst` & `coop_html_editor-1.4.1/README.rst`

 * *Files identical despite different names*

