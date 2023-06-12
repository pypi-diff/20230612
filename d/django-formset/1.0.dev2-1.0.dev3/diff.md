# Comparing `tmp/django-formset-1.0.dev2.tar.gz` & `tmp/django-formset-1.0.dev3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "django-formset-1.0.dev2.tar", last modified: Sun Jun 11 11:07:28 2023, max compression
+gzip compressed data, was "django-formset-1.0.dev3.tar", last modified: Mon Jun 12 21:30:44 2023, max compression
```

## Comparing `django-formset-1.0.dev2.tar` & `django-formset-1.0.dev3.tar`

### file list

```diff
@@ -1,261 +1,262 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-11 11:07:28.344778 django-formset-1.0.dev2/
--rw-r--r--   0 runner    (1001) docker     (123)     1079 2023-06-11 11:06:18.000000 django-formset-1.0.dev2/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)      244 2023-06-11 11:06:18.000000 django-formset-1.0.dev2/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)    14240 2023-06-11 11:07:28.344778 django-formset-1.0.dev2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    13295 2023-06-11 11:06:18.000000 django-formset-1.0.dev2/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-11 11:07:28.308778 django-formset-1.0.dev2/django_formset.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    14240 2023-06-11 11:07:28.000000 django-formset-1.0.dev2/django_formset.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    10212 2023-06-11 11:07:28.000000 django-formset-1.0.dev2/django_formset.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-11 11:07:28.000000 django-formset-1.0.dev2/django_formset.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-11 11:07:28.000000 django-formset-1.0.dev2/django_formset.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)       12 2023-06-11 11:07:28.000000 django-formset-1.0.dev2/django_formset.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       16 2023-06-11 11:07:28.000000 django-formset-1.0.dev2/django_formset.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-11 11:07:28.308778 django-formset-1.0.dev2/formset/
--rw-r--r--   0 runner    (1001) docker     (123)       25 2023-06-11 11:06:18.000000 django-formset-1.0.dev2/formset/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     8860 2023-06-11 11:06:18.000000 django-formset-1.0.dev2/formset/boundfield.py
--rw-r--r--   0 runner    (1001) docker     (123)     7637 2023-06-11 11:06:18.000000 django-formset-1.0.dev2/formset/calendar.py
--rw-r--r--   0 runner    (1001) docker     (123)    20763 2023-06-11 11:06:18.000000 django-formset-1.0.dev2/formset/collection.py
--rw-r--r--   0 runner    (1001) docker     (123)      101 2023-06-11 11:06:18.000000 django-formset-1.0.dev2/formset/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (123)     2913 2023-06-11 11:06:18.000000 django-formset-1.0.dev2/formset/fields.py
--rw-r--r--   0 runner    (1001) docker     (123)     2098 2023-06-11 11:06:18.000000 django-formset-1.0.dev2/formset/fieldset.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-11 11:07:28.304777 django-formset-1.0.dev2/formset/locale/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-11 11:07:28.304777 django-formset-1.0.dev2/formset/locale/de/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-11 11:07:28.308778 django-formset-1.0.dev2/formset/locale/de/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (123)     3444 2023-06-11 11:07:21.000000 django-formset-1.0.dev2/formset/locale/de/LC_MESSAGES/django.mo
--rw-r--r--   0 runner    (1001) docker     (123)     7554 2023-06-11 11:06:18.000000 django-formset-1.0.dev2/formset/locale/de/LC_MESSAGES/django.po
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-11 11:07:28.312778 django-formset-1.0.dev2/formset/renderers/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-11 11:06:18.000000 django-formset-1.0.dev2/formset/renderers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4271 2023-06-11 11:06:18.000000 django-formset-1.0.dev2/formset/renderers/bootstrap.py
--rw-r--r--   0 runner    (1001) docker     (123)     3302 2023-06-11 11:06:18.000000 django-formset-1.0.dev2/formset/renderers/bulma.py
--rw-r--r--   0 runner    (1001) docker     (123)     5684 2023-06-11 11:06:18.000000 django-formset-1.0.dev2/formset/renderers/default.py
--rw-r--r--   0 runner    (1001) docker     (123)     1964 2023-06-11 11:06:18.000000 django-formset-1.0.dev2/formset/renderers/foundation.py
--rw-r--r--   0 runner    (1001) docker     (123)     5111 2023-06-11 11:06:18.000000 django-formset-1.0.dev2/formset/renderers/tailwind.py
--rw-r--r--   0 runner    (1001) docker     (123)     2851 2023-06-11 11:06:18.000000 django-formset-1.0.dev2/formset/renderers/uikit.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-11 11:07:28.312778 django-formset-1.0.dev2/formset/richtext/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-11 11:06:18.000000 django-formset-1.0.dev2/formset/richtext/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     7308 2023-06-11 11:06:18.000000 django-formset-1.0.dev2/formset/richtext/controls.py
--rw-r--r--   0 runner    (1001) docker     (123)     1456 2023-06-11 11:06:18.000000 django-formset-1.0.dev2/formset/richtext/dialogs.py
--rw-r--r--   0 runner    (1001) docker     (123)      353 2023-06-11 11:06:18.000000 django-formset-1.0.dev2/formset/richtext/fields.py
--rw-r--r--   0 runner    (1001) docker     (123)     2043 2023-06-11 11:06:18.000000 django-formset-1.0.dev2/formset/richtext/widgets.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-11 11:07:28.304777 django-formset-1.0.dev2/formset/static/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-11 11:07:28.304777 django-formset-1.0.dev2/formset/static/formset/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-11 11:07:28.312778 django-formset-1.0.dev2/formset/static/formset/css/
--rw-r--r--   0 runner    (1001) docker     (123)     1895 2023-06-11 11:07:18.000000 django-formset-1.0.dev2/formset/static/formset/css/bootstrap5-extra.css
--rw-r--r--   0 runner    (1001) docker     (123)      567 2023-06-11 11:07:18.000000 django-formset-1.0.dev2/formset/static/formset/css/bootstrap5-extra.css.map
--rw-r--r--   0 runner    (1001) docker     (123)     1830 2023-06-11 11:07:18.000000 django-formset-1.0.dev2/formset/static/formset/css/collections.css
--rw-r--r--   0 runner    (1001) docker     (123)      354 2023-06-11 11:07:18.000000 django-formset-1.0.dev2/formset/static/formset/css/collections.css.map
--rw-r--r--   0 runner    (1001) docker     (123)    35875 2023-06-11 11:07:19.000000 django-formset-1.0.dev2/formset/static/formset/css/tailwind.css
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-11 11:07:28.312778 django-formset-1.0.dev2/formset/static/formset/icons/
--rw-r--r--   0 runner    (1001) docker     (123)     1516 2023-06-11 11:06:18.000000 django-formset-1.0.dev2/formset/static/formset/icons/file-audio.svg
--rw-r--r--   0 runner    (1001) docker     (123)      637 2023-06-11 11:06:18.000000 django-formset-1.0.dev2/formset/static/formset/icons/file-empty.svg
--rw-r--r--   0 runner    (1001) docker     (123)     1258 2023-06-11 11:06:18.000000 django-formset-1.0.dev2/formset/static/formset/icons/file-font.svg
--rw-r--r--   0 runner    (1001) docker     (123)     3181 2023-06-11 11:06:18.000000 django-formset-1.0.dev2/formset/static/formset/icons/file-missing.svg
--rw-r--r--   0 runner    (1001) docker     (123)     1958 2023-06-11 11:06:18.000000 django-formset-1.0.dev2/formset/static/formset/icons/file-pdf.svg
--rw-r--r--   0 runner    (1001) docker     (123)     1031 2023-06-11 11:06:18.000000 django-formset-1.0.dev2/formset/static/formset/icons/file-picture.svg
--rw-r--r--   0 runner    (1001) docker     (123)     2071 2023-06-11 11:06:18.000000 django-formset-1.0.dev2/formset/static/formset/icons/file-unknown.svg
--rw-r--r--   0 runner    (1001) docker     (123)     2911 2023-06-11 11:06:18.000000 django-formset-1.0.dev2/formset/static/formset/icons/file-video.svg
--rw-r--r--   0 runner    (1001) docker     (123)     1838 2023-06-11 11:06:18.000000 django-formset-1.0.dev2/formset/static/formset/icons/file-zip.svg
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-11 11:07:28.316778 django-formset-1.0.dev2/formset/static/formset/js/
--rw-r--r--   0 runner    (1001) docker     (123)    25407 2023-06-11 11:07:20.000000 django-formset-1.0.dev2/formset/static/formset/js/DateTimePicker-64ONYNKG.js
--rw-r--r--   0 runner    (1001) docker     (123)    55721 2023-06-11 11:07:20.000000 django-formset-1.0.dev2/formset/static/formset/js/DjangoSelectize-MICJ4DHH.js
--rw-r--r--   0 runner    (1001) docker     (123)    11534 2023-06-11 11:07:20.000000 django-formset-1.0.dev2/formset/static/formset/js/DjangoSlug-226MVQ6E.js
--rw-r--r--   0 runner    (1001) docker     (123)    12352 2023-06-11 11:07:20.000000 django-formset-1.0.dev2/formset/static/formset/js/DualSelector-XYVC5VWO.js
--rw-r--r--   0 runner    (1001) docker     (123)   316764 2023-06-11 11:07:20.000000 django-formset-1.0.dev2/formset/static/formset/js/RichtextArea-63COGKXW.js
--rw-r--r--   0 runner    (1001) docker     (123)      196 2023-06-11 11:07:20.000000 django-formset-1.0.dev2/formset/static/formset/js/SortableSelect-WBJL5XGS.js
--rw-r--r--   0 runner    (1001) docker     (123)     1713 2023-06-11 11:07:20.000000 django-formset-1.0.dev2/formset/static/formset/js/chunk-AELXO3WZ.js
--rw-r--r--   0 runner    (1001) docker     (123)    43947 2023-06-11 11:07:20.000000 django-formset-1.0.dev2/formset/static/formset/js/chunk-APVD22ED.js
--rw-r--r--   0 runner    (1001) docker     (123)    12466 2023-06-11 11:07:20.000000 django-formset-1.0.dev2/formset/static/formset/js/chunk-ISEEQP4V.js
--rw-r--r--   0 runner    (1001) docker     (123)     3967 2023-06-11 11:07:20.000000 django-formset-1.0.dev2/formset/static/formset/js/chunk-JSQHGMDY.js
--rw-r--r--   0 runner    (1001) docker     (123)     9669 2023-06-11 11:07:20.000000 django-formset-1.0.dev2/formset/static/formset/js/chunk-KDP4ZIAK.js
--rw-r--r--   0 runner    (1001) docker     (123)      544 2023-06-11 11:07:20.000000 django-formset-1.0.dev2/formset/static/formset/js/chunk-NLMHZ7JJ.js
--rw-r--r--   0 runner    (1001) docker     (123)     1850 2023-06-11 11:07:20.000000 django-formset-1.0.dev2/formset/static/formset/js/chunk-O5UGFU32.js
--rw-r--r--   0 runner    (1001) docker     (123)   106347 2023-06-11 11:07:20.000000 django-formset-1.0.dev2/formset/static/formset/js/django-formset.js
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-11 11:07:28.316778 django-formset-1.0.dev2/formset/static/formset/scss/
--rw-r--r--   0 runner    (1001) docker     (123)     2091 2023-06-11 11:06:18.000000 django-formset-1.0.dev2/formset/static/formset/scss/bootstrap5-extra.scss
--rw-r--r--   0 runner    (1001) docker     (123)     1497 2023-06-11 11:06:18.000000 django-formset-1.0.dev2/formset/static/formset/scss/collections.scss
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-11 11:07:28.304777 django-formset-1.0.dev2/formset/templates/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-11 11:07:28.304777 django-formset-1.0.dev2/formset/templates/admin/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-11 11:07:28.316778 django-formset-1.0.dev2/formset/templates/admin/formset/
--rw-r--r--   0 runner    (1001) docker     (123)      344 2023-06-11 11:06:18.000000 django-formset-1.0.dev2/formset/templates/admin/formset/change_form.html
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-11 11:07:28.316778 django-formset-1.0.dev2/formset/templates/calendar/
--rw-r--r--   0 runner    (1001) docker     (123)     1360 2023-06-11 11:06:18.000000 django-formset-1.0.dev2/formset/templates/calendar/hours.html
--rw-r--r--   0 runner    (1001) docker     (123)     1176 2023-06-11 11:06:18.000000 django-formset-1.0.dev2/formset/templates/calendar/months.html
--rw-r--r--   0 runner    (1001) docker     (123)     1208 2023-06-11 11:06:18.000000 django-formset-1.0.dev2/formset/templates/calendar/weeks.html
--rw-r--r--   0 runner    (1001) docker     (123)     1132 2023-06-11 11:06:18.000000 django-formset-1.0.dev2/formset/templates/calendar/years.html
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-11 11:07:28.320778 django-formset-1.0.dev2/formset/templates/formset/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-11 11:07:28.320778 django-formset-1.0.dev2/formset/templates/formset/bootstrap/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-11 11:07:28.320778 django-formset-1.0.dev2/formset/templates/formset/bootstrap/buttons/
--rw-r--r--   0 runner    (1001) docker     (123)      176 2023-06-11 11:06:18.000000 django-formset-1.0.dev2/formset/templates/formset/bootstrap/buttons/add_collection.html
--rw-r--r--   0 runner    (1001) docker     (123)      134 2023-06-11 11:06:18.000000 django-formset-1.0.dev2/formset/templates/formset/bootstrap/buttons/remove_collection.html
--rw-r--r--   0 runner    (1001) docker     (123)      194 2023-06-11 11:06:18.000000 django-formset-1.0.dev2/formset/templates/formset/bootstrap/buttons/richtext_align.html
--rw-r--r--   0 runner    (1001) docker     (123)      194 2023-06-11 11:06:18.000000 django-formset-1.0.dev2/formset/templates/formset/bootstrap/buttons/richtext_color.html
--rw-r--r--   0 runner    (1001) docker     (123)      196 2023-06-11 11:06:18.000000 django-formset-1.0.dev2/formset/templates/formset/bootstrap/buttons/richtext_heading.html
--rw-r--r--   0 runner    (1001) docker     (123)      511 2023-06-11 11:06:18.000000 django-formset-1.0.dev2/formset/templates/formset/bootstrap/field_group.html
--rw-r--r--   0 runner    (1001) docker     (123)      254 2023-06-11 11:06:18.000000 django-formset-1.0.dev2/formset/templates/formset/bootstrap/form.html
--rw-r--r--   0 runner    (1001) docker     (123)       55 2023-06-11 11:06:18.000000 django-formset-1.0.dev2/formset/templates/formset/bootstrap/help_text.html
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-11 11:07:28.320778 django-formset-1.0.dev2/formset/templates/formset/bootstrap/widgets/
--rw-r--r--   0 runner    (1001) docker     (123)      181 2023-06-11 11:06:18.000000 django-formset-1.0.dev2/formset/templates/formset/bootstrap/widgets/checkbox.html
--rw-r--r--   0 runner    (1001) docker     (123)      918 2023-06-11 11:06:18.000000 django-formset-1.0.dev2/formset/templates/formset/bootstrap/widgets/dual_selector.html
--rw-r--r--   0 runner    (1001) docker     (123)      637 2023-06-11 11:06:18.000000 django-formset-1.0.dev2/formset/templates/formset/bootstrap/widgets/file.html
--rw-r--r--   0 runner    (1001) docker     (123)      169 2023-06-11 11:06:18.000000 django-formset-1.0.dev2/formset/templates/formset/bootstrap/widgets/input_option.html
--rw-r--r--   0 runner    (1001) docker     (123)      468 2023-06-11 11:06:18.000000 django-formset-1.0.dev2/formset/templates/formset/bootstrap/widgets/multiple_input.html
--rw-r--r--   0 runner    (1001) docker     (123)       58 2023-06-11 11:06:18.000000 django-formset-1.0.dev2/formset/templates/formset/bootstrap/widgets/richtextarea.html
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-11 11:07:28.320778 django-formset-1.0.dev2/formset/templates/formset/bulma/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-11 11:07:28.320778 django-formset-1.0.dev2/formset/templates/formset/bulma/buttons/
--rw-r--r--   0 runner    (1001) docker     (123)      124 2023-06-11 11:06:18.000000 django-formset-1.0.dev2/formset/templates/formset/bulma/buttons/add_collection.html
--rw-r--r--   0 runner    (1001) docker     (123)      122 2023-06-11 11:06:18.000000 django-formset-1.0.dev2/formset/templates/formset/bulma/buttons/remove_collection.html
--rw-r--r--   0 runner    (1001) docker     (123)      364 2023-06-11 11:06:18.000000 django-formset-1.0.dev2/formset/templates/formset/bulma/field_group.html
--rw-r--r--   0 runner    (1001) docker     (123)      253 2023-06-11 11:06:18.000000 django-formset-1.0.dev2/formset/templates/formset/bulma/form.html
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-11 11:07:28.324778 django-formset-1.0.dev2/formset/templates/formset/bulma/widgets/
--rw-r--r--   0 runner    (1001) docker     (123)      141 2023-06-11 11:06:18.000000 django-formset-1.0.dev2/formset/templates/formset/bulma/widgets/checkbox.html
--rw-r--r--   0 runner    (1001) docker     (123)     1260 2023-06-11 11:06:18.000000 django-formset-1.0.dev2/formset/templates/formset/bulma/widgets/dual_selector.html
--rw-r--r--   0 runner    (1001) docker     (123)      669 2023-06-11 11:06:18.000000 django-formset-1.0.dev2/formset/templates/formset/bulma/widgets/file.html
--rw-r--r--   0 runner    (1001) docker     (123)      183 2023-06-11 11:06:18.000000 django-formset-1.0.dev2/formset/templates/formset/bulma/widgets/input_option.html
--rw-r--r--   0 runner    (1001) docker     (123)      396 2023-06-11 11:06:18.000000 django-formset-1.0.dev2/formset/templates/formset/bulma/widgets/multiple_input.html
--rw-r--r--   0 runner    (1001) docker     (123)      113 2023-06-11 11:06:18.000000 django-formset-1.0.dev2/formset/templates/formset/bulma/widgets/select.html
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-11 11:07:28.324778 django-formset-1.0.dev2/formset/templates/formset/default/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-11 11:07:28.324778 django-formset-1.0.dev2/formset/templates/formset/default/buttons/
--rw-r--r--   0 runner    (1001) docker     (123)      361 2023-06-11 11:06:18.000000 django-formset-1.0.dev2/formset/templates/formset/default/buttons/add_collection.html
--rw-r--r--   0 runner    (1001) docker     (123)      204 2023-06-11 11:06:18.000000 django-formset-1.0.dev2/formset/templates/formset/default/buttons/move_all_left.html
--rw-r--r--   0 runner    (1001) docker     (123)      207 2023-06-11 11:06:18.000000 django-formset-1.0.dev2/formset/templates/formset/default/buttons/move_all_right.html
--rw-r--r--   0 runner    (1001) docker     (123)      207 2023-06-11 11:06:18.000000 django-formset-1.0.dev2/formset/templates/formset/default/buttons/move_selected_left.html
--rw-r--r--   0 runner    (1001) docker     (123)      210 2023-06-11 11:06:18.000000 django-formset-1.0.dev2/formset/templates/formset/default/buttons/move_selected_right.html
--rw-r--r--   0 runner    (1001) docker     (123)      189 2023-06-11 11:06:18.000000 django-formset-1.0.dev2/formset/templates/formset/default/buttons/redo_selected.html
--rw-r--r--   0 runner    (1001) docker     (123)      233 2023-06-11 11:06:18.000000 django-formset-1.0.dev2/formset/templates/formset/default/buttons/remove_collection.html
--rw-r--r--   0 runner    (1001) docker     (123)      959 2023-06-11 11:06:18.000000 django-formset-1.0.dev2/formset/templates/formset/default/buttons/richtext_align.html
--rw-r--r--   0 runner    (1001) docker     (123)      692 2023-06-11 11:06:18.000000 django-formset-1.0.dev2/formset/templates/formset/default/buttons/richtext_color.html
--rw-r--r--   0 runner    (1001) docker     (123)      102 2023-06-11 11:06:18.000000 django-formset-1.0.dev2/formset/templates/formset/default/buttons/richtext_control.html
--rw-r--r--   0 runner    (1001) docker     (123)      843 2023-06-11 11:06:18.000000 django-formset-1.0.dev2/formset/templates/formset/default/buttons/richtext_heading.html
--rw-r--r--   0 runner    (1001) docker     (123)       92 2023-06-11 11:06:18.000000 django-formset-1.0.dev2/formset/templates/formset/default/buttons/richtext_separator.html
--rw-r--r--   0 runner    (1001) docker     (123)      189 2023-06-11 11:06:18.000000 django-formset-1.0.dev2/formset/templates/formset/default/buttons/undo_selected.html
--rw-r--r--   0 runner    (1001) docker     (123)     1504 2023-06-11 11:06:18.000000 django-formset-1.0.dev2/formset/templates/formset/default/collection.html
--rw-r--r--   0 runner    (1001) docker     (123)      864 2023-06-11 11:06:18.000000 django-formset-1.0.dev2/formset/templates/formset/default/dialog_form.html
--rw-r--r--   0 runner    (1001) docker     (123)      300 2023-06-11 11:06:18.000000 django-formset-1.0.dev2/formset/templates/formset/default/field_errors.html
--rw-r--r--   0 runner    (1001) docker     (123)      407 2023-06-11 11:06:18.000000 django-formset-1.0.dev2/formset/templates/formset/default/field_group.html
--rw-r--r--   0 runner    (1001) docker     (123)      677 2023-06-11 11:06:18.000000 django-formset-1.0.dev2/formset/templates/formset/default/fieldset.html
--rw-r--r--   0 runner    (1001) docker     (123)      415 2023-06-11 11:06:18.000000 django-formset-1.0.dev2/formset/templates/formset/default/form.html
--rw-r--r--   0 runner    (1001) docker     (123)       47 2023-06-11 11:06:18.000000 django-formset-1.0.dev2/formset/templates/formset/default/help_text.html
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-11 11:07:28.328778 django-formset-1.0.dev2/formset/templates/formset/default/widgets/
--rw-r--r--   0 runner    (1001) docker     (123)      149 2023-06-11 11:06:18.000000 django-formset-1.0.dev2/formset/templates/formset/default/widgets/datetimepicker.html
--rw-r--r--   0 runner    (1001) docker     (123)     2416 2023-06-11 11:06:18.000000 django-formset-1.0.dev2/formset/templates/formset/default/widgets/dual_selector.html
--rw-r--r--   0 runner    (1001) docker     (123)     1407 2023-06-11 11:06:18.000000 django-formset-1.0.dev2/formset/templates/formset/default/widgets/file.html
--rw-r--r--   0 runner    (1001) docker     (123)      454 2023-06-11 11:06:18.000000 django-formset-1.0.dev2/formset/templates/formset/default/widgets/multiple_input.html
--rw-r--r--   0 runner    (1001) docker     (123)      446 2023-06-11 11:06:18.000000 django-formset-1.0.dev2/formset/templates/formset/default/widgets/richtextarea.html
--rw-r--r--   0 runner    (1001) docker     (123)       48 2023-06-11 11:06:18.000000 django-formset-1.0.dev2/formset/templates/formset/default/widgets/select.html
--rw-r--r--   0 runner    (1001) docker     (123)     1048 2023-06-11 11:06:18.000000 django-formset-1.0.dev2/formset/templates/formset/default/widgets/selectize.html
--rw-r--r--   0 runner    (1001) docker     (123)      216 2023-06-11 11:06:18.000000 django-formset-1.0.dev2/formset/templates/formset/form_attrs.html
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-11 11:07:28.328778 django-formset-1.0.dev2/formset/templates/formset/foundation/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-11 11:07:28.328778 django-formset-1.0.dev2/formset/templates/formset/foundation/buttons/
--rw-r--r--   0 runner    (1001) docker     (123)      132 2023-06-11 11:06:18.000000 django-formset-1.0.dev2/formset/templates/formset/foundation/buttons/add_collection.html
--rw-r--r--   0 runner    (1001) docker     (123)      128 2023-06-11 11:06:18.000000 django-formset-1.0.dev2/formset/templates/formset/foundation/buttons/remove_collection.html
--rw-r--r--   0 runner    (1001) docker     (123)      390 2023-06-11 11:06:18.000000 django-formset-1.0.dev2/formset/templates/formset/foundation/field_group.html
--rw-r--r--   0 runner    (1001) docker     (123)      258 2023-06-11 11:06:18.000000 django-formset-1.0.dev2/formset/templates/formset/foundation/form.html
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-11 11:07:28.328778 django-formset-1.0.dev2/formset/templates/formset/foundation/widgets/
--rw-r--r--   0 runner    (1001) docker     (123)      123 2023-06-11 11:06:18.000000 django-formset-1.0.dev2/formset/templates/formset/foundation/widgets/checkbox.html
--rw-r--r--   0 runner    (1001) docker     (123)      835 2023-06-11 11:06:18.000000 django-formset-1.0.dev2/formset/templates/formset/foundation/widgets/dual_selector.html
--rw-r--r--   0 runner    (1001) docker     (123)      654 2023-06-11 11:06:18.000000 django-formset-1.0.dev2/formset/templates/formset/foundation/widgets/file.html
--rw-r--r--   0 runner    (1001) docker     (123)      145 2023-06-11 11:06:18.000000 django-formset-1.0.dev2/formset/templates/formset/foundation/widgets/inlined_input_option.html
--rw-r--r--   0 runner    (1001) docker     (123)      340 2023-06-11 11:06:18.000000 django-formset-1.0.dev2/formset/templates/formset/foundation/widgets/multiple_input.html
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-11 11:07:28.336778 django-formset-1.0.dev2/formset/templates/formset/icons/
--rw-r--r--   0 runner    (1001) docker     (123)      196 2023-06-11 11:06:18.000000 django-formset-1.0.dev2/formset/templates/formset/icons/add-fill.svg
--rw-r--r--   0 runner    (1001) docker     (123)      193 2023-06-11 11:06:18.000000 django-formset-1.0.dev2/formset/templates/formset/icons/align-center.svg
--rw-r--r--   0 runner    (1001) docker     (123)      193 2023-06-11 11:06:18.000000 django-formset-1.0.dev2/formset/templates/formset/icons/align-justify.svg
--rw-r--r--   0 runner    (1001) docker     (123)      193 2023-06-11 11:06:18.000000 django-formset-1.0.dev2/formset/templates/formset/icons/align-left.svg
--rw-r--r--   0 runner    (1001) docker     (123)      193 2023-06-11 11:06:18.000000 django-formset-1.0.dev2/formset/templates/formset/icons/align-right.svg
--rw-r--r--   0 runner    (1001) docker     (123)      237 2023-06-11 11:06:18.000000 django-formset-1.0.dev2/formset/templates/formset/icons/arrow-left.svg
--rw-r--r--   0 runner    (1001) docker     (123)      245 2023-06-11 11:06:18.000000 django-formset-1.0.dev2/formset/templates/formset/icons/arrow-right.svg
--rw-r--r--   0 runner    (1001) docker     (123)      248 2023-06-11 11:06:18.000000 django-formset-1.0.dev2/formset/templates/formset/icons/arrow-up.svg
--rw-r--r--   0 runner    (1001) docker     (123)      792 2023-06-11 11:06:18.000000 django-formset-1.0.dev2/formset/templates/formset/icons/blockquote.svg
--rw-r--r--   0 runner    (1001) docker     (123)      408 2023-06-11 11:06:18.000000 django-formset-1.0.dev2/formset/templates/formset/icons/bold.svg
--rw-r--r--   0 runner    (1001) docker     (123)      252 2023-06-11 11:06:18.000000 django-formset-1.0.dev2/formset/templates/formset/icons/bulletlist.svg
--rw-r--r--   0 runner    (1001) docker     (123)      463 2023-06-11 11:06:18.000000 django-formset-1.0.dev2/formset/templates/formset/icons/calendar-today.svg
--rw-r--r--   0 runner    (1001) docker     (123)      318 2023-06-11 11:06:18.000000 django-formset-1.0.dev2/formset/templates/formset/icons/chevron-double-left.svg
--rw-r--r--   0 runner    (1001) docker     (123)      312 2023-06-11 11:06:18.000000 django-formset-1.0.dev2/formset/templates/formset/icons/chevron-double-right.svg
--rw-r--r--   0 runner    (1001) docker     (123)      225 2023-06-11 11:06:18.000000 django-formset-1.0.dev2/formset/templates/formset/icons/chevron-left.svg
--rw-r--r--   0 runner    (1001) docker     (123)      228 2023-06-11 11:06:18.000000 django-formset-1.0.dev2/formset/templates/formset/icons/chevron-right.svg
--rw-r--r--   0 runner    (1001) docker     (123)      329 2023-06-11 11:06:18.000000 django-formset-1.0.dev2/formset/templates/formset/icons/clearformat.svg
--rw-r--r--   0 runner    (1001) docker     (123)      359 2023-06-11 11:06:18.000000 django-formset-1.0.dev2/formset/templates/formset/icons/codeblock.svg
--rw-r--r--   0 runner    (1001) docker     (123)      219 2023-06-11 11:06:18.000000 django-formset-1.0.dev2/formset/templates/formset/icons/decreasemargin.svg
--rw-r--r--   0 runner    (1001) docker     (123)      467 2023-06-11 11:06:18.000000 django-formset-1.0.dev2/formset/templates/formset/icons/delete-back.svg
--rw-r--r--   0 runner    (1001) docker     (123)      456 2023-06-11 11:06:18.000000 django-formset-1.0.dev2/formset/templates/formset/icons/double-chevron-left.svg
--rw-r--r--   0 runner    (1001) docker     (123)      463 2023-06-11 11:06:18.000000 django-formset-1.0.dev2/formset/templates/formset/icons/double-chevron-right.svg
--rw-r--r--   0 runner    (1001) docker     (123)      323 2023-06-11 11:06:18.000000 django-formset-1.0.dev2/formset/templates/formset/icons/hardbreak.svg
--rw-r--r--   0 runner    (1001) docker     (123)      195 2023-06-11 11:06:18.000000 django-formset-1.0.dev2/formset/templates/formset/icons/heading.svg
--rw-r--r--   0 runner    (1001) docker     (123)      239 2023-06-11 11:06:18.000000 django-formset-1.0.dev2/formset/templates/formset/icons/heading1.svg
--rw-r--r--   0 runner    (1001) docker     (123)      429 2023-06-11 11:06:18.000000 django-formset-1.0.dev2/formset/templates/formset/icons/heading2.svg
--rw-r--r--   0 runner    (1001) docker     (123)      457 2023-06-11 11:06:18.000000 django-formset-1.0.dev2/formset/templates/formset/icons/heading3.svg
--rw-r--r--   0 runner    (1001) docker     (123)      272 2023-06-11 11:06:18.000000 django-formset-1.0.dev2/formset/templates/formset/icons/heading4.svg
--rw-r--r--   0 runner    (1001) docker     (123)      431 2023-06-11 11:06:18.000000 django-formset-1.0.dev2/formset/templates/formset/icons/heading5.svg
--rw-r--r--   0 runner    (1001) docker     (123)      371 2023-06-11 11:06:18.000000 django-formset-1.0.dev2/formset/templates/formset/icons/heading6.svg
--rw-r--r--   0 runner    (1001) docker     (123)      182 2023-06-11 11:06:18.000000 django-formset-1.0.dev2/formset/templates/formset/icons/horizontalrule.svg
--rw-r--r--   0 runner    (1001) docker     (123)      397 2023-06-11 11:06:18.000000 django-formset-1.0.dev2/formset/templates/formset/icons/image.svg
--rw-r--r--   0 runner    (1001) docker     (123)      219 2023-06-11 11:06:18.000000 django-formset-1.0.dev2/formset/templates/formset/icons/increasemargin.svg
--rw-r--r--   0 runner    (1001) docker     (123)      214 2023-06-11 11:06:18.000000 django-formset-1.0.dev2/formset/templates/formset/icons/indentfirstline.svg
--rw-r--r--   0 runner    (1001) docker     (123)      218 2023-06-11 11:06:18.000000 django-formset-1.0.dev2/formset/templates/formset/icons/italic.svg
--rw-r--r--   0 runner    (1001) docker     (123)      632 2023-06-11 11:06:18.000000 django-formset-1.0.dev2/formset/templates/formset/icons/letters.svg
--rw-r--r--   0 runner    (1001) docker     (123)      475 2023-06-11 11:06:18.000000 django-formset-1.0.dev2/formset/templates/formset/icons/link.svg
--rw-r--r--   0 runner    (1001) docker     (123)      308 2023-06-11 11:06:18.000000 django-formset-1.0.dev2/formset/templates/formset/icons/orderedlist.svg
--rw-r--r--   0 runner    (1001) docker     (123)      214 2023-06-11 11:06:18.000000 django-formset-1.0.dev2/formset/templates/formset/icons/outdentfirstline.svg
--rw-r--r--   0 runner    (1001) docker     (123)     1226 2023-06-11 11:06:18.000000 django-formset-1.0.dev2/formset/templates/formset/icons/placeholder.svg
--rw-r--r--   0 runner    (1001) docker     (123)      529 2023-06-11 11:06:18.000000 django-formset-1.0.dev2/formset/templates/formset/icons/questionmark.svg
--rw-r--r--   0 runner    (1001) docker     (123)      280 2023-06-11 11:06:18.000000 django-formset-1.0.dev2/formset/templates/formset/icons/redo.svg
--rw-r--r--   0 runner    (1001) docker     (123)      457 2023-06-11 11:06:18.000000 django-formset-1.0.dev2/formset/templates/formset/icons/send.svg
--rw-r--r--   0 runner    (1001) docker     (123)      200 2023-06-11 11:06:18.000000 django-formset-1.0.dev2/formset/templates/formset/icons/separator.svg
--rw-r--r--   0 runner    (1001) docker     (123)      514 2023-06-11 11:06:18.000000 django-formset-1.0.dev2/formset/templates/formset/icons/subscript.svg
--rw-r--r--   0 runner    (1001) docker     (123)      501 2023-06-11 11:06:18.000000 django-formset-1.0.dev2/formset/templates/formset/icons/superscript.svg
--rw-r--r--   0 runner    (1001) docker     (123)      274 2023-06-11 11:06:18.000000 django-formset-1.0.dev2/formset/templates/formset/icons/textcolor.svg
--rw-r--r--   0 runner    (1001) docker     (123)      309 2023-06-11 11:06:18.000000 django-formset-1.0.dev2/formset/templates/formset/icons/trash.svg
--rw-r--r--   0 runner    (1001) docker     (123)      225 2023-06-11 11:06:18.000000 django-formset-1.0.dev2/formset/templates/formset/icons/underline.svg
--rw-r--r--   0 runner    (1001) docker     (123)      275 2023-06-11 11:06:18.000000 django-formset-1.0.dev2/formset/templates/formset/icons/undo.svg
--rw-r--r--   0 runner    (1001) docker     (123)      513 2023-06-11 11:06:18.000000 django-formset-1.0.dev2/formset/templates/formset/icons/unlink.svg
--rw-r--r--   0 runner    (1001) docker     (123)      109 2023-06-11 11:06:18.000000 django-formset-1.0.dev2/formset/templates/formset/non_field_errors.html
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-11 11:07:28.336778 django-formset-1.0.dev2/formset/templates/formset/tailwind/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-11 11:07:28.336778 django-formset-1.0.dev2/formset/templates/formset/tailwind/buttons/
--rw-r--r--   0 runner    (1001) docker     (123)      309 2023-06-11 11:06:18.000000 django-formset-1.0.dev2/formset/templates/formset/tailwind/buttons/add_collection.html
--rw-r--r--   0 runner    (1001) docker     (123)      262 2023-06-11 11:06:18.000000 django-formset-1.0.dev2/formset/templates/formset/tailwind/buttons/remove_collection.html
--rw-r--r--   0 runner    (1001) docker     (123)      376 2023-06-11 11:06:18.000000 django-formset-1.0.dev2/formset/templates/formset/tailwind/field_group.html
--rw-r--r--   0 runner    (1001) docker     (123)      256 2023-06-11 11:06:18.000000 django-formset-1.0.dev2/formset/templates/formset/tailwind/form.html
--rw-r--r--   0 runner    (1001) docker     (123)       48 2023-06-11 11:06:18.000000 django-formset-1.0.dev2/formset/templates/formset/tailwind/help_text.html
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-11 11:07:28.340778 django-formset-1.0.dev2/formset/templates/formset/tailwind/widgets/
--rw-r--r--   0 runner    (1001) docker     (123)      124 2023-06-11 11:06:18.000000 django-formset-1.0.dev2/formset/templates/formset/tailwind/widgets/checkbox.html
--rw-r--r--   0 runner    (1001) docker     (123)      884 2023-06-11 11:06:18.000000 django-formset-1.0.dev2/formset/templates/formset/tailwind/widgets/dual_selector.html
--rw-r--r--   0 runner    (1001) docker     (123)      611 2023-06-11 11:06:18.000000 django-formset-1.0.dev2/formset/templates/formset/tailwind/widgets/file.html
--rw-r--r--   0 runner    (1001) docker     (123)      144 2023-06-11 11:06:18.000000 django-formset-1.0.dev2/formset/templates/formset/tailwind/widgets/input_option.html
--rw-r--r--   0 runner    (1001) docker     (123)      454 2023-06-11 11:06:18.000000 django-formset-1.0.dev2/formset/templates/formset/tailwind/widgets/multiple_input.html
--rw-r--r--   0 runner    (1001) docker     (123)      449 2023-06-11 11:06:18.000000 django-formset-1.0.dev2/formset/templates/formset/tailwind/widgets/radio.html
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-11 11:07:28.340778 django-formset-1.0.dev2/formset/templates/formset/uikit/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-11 11:07:28.340778 django-formset-1.0.dev2/formset/templates/formset/uikit/buttons/
--rw-r--r--   0 runner    (1001) docker     (123)      113 2023-06-11 11:06:18.000000 django-formset-1.0.dev2/formset/templates/formset/uikit/buttons/add_collection.html
--rw-r--r--   0 runner    (1001) docker     (123)      116 2023-06-11 11:06:18.000000 django-formset-1.0.dev2/formset/templates/formset/uikit/buttons/remove_collection.html
--rw-r--r--   0 runner    (1001) docker     (123)      377 2023-06-11 11:06:18.000000 django-formset-1.0.dev2/formset/templates/formset/uikit/field_group.html
--rw-r--r--   0 runner    (1001) docker     (123)      253 2023-06-11 11:06:18.000000 django-formset-1.0.dev2/formset/templates/formset/uikit/form.html
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-11 11:07:28.340778 django-formset-1.0.dev2/formset/templates/formset/uikit/widgets/
--rw-r--r--   0 runner    (1001) docker     (123)      125 2023-06-11 11:06:18.000000 django-formset-1.0.dev2/formset/templates/formset/uikit/widgets/checkbox.html
--rw-r--r--   0 runner    (1001) docker     (123)      681 2023-06-11 11:06:18.000000 django-formset-1.0.dev2/formset/templates/formset/uikit/widgets/file.html
--rw-r--r--   0 runner    (1001) docker     (123)      227 2023-06-11 11:06:18.000000 django-formset-1.0.dev2/formset/templates/formset/uikit/widgets/input_option.html
--rw-r--r--   0 runner    (1001) docker     (123)      464 2023-06-11 11:06:18.000000 django-formset-1.0.dev2/formset/templates/formset/uikit/widgets/multiple_input.html
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-11 11:07:28.340778 django-formset-1.0.dev2/formset/templates/richtext/
--rw-r--r--   0 runner    (1001) docker     (123)      234 2023-06-11 11:06:18.000000 django-formset-1.0.dev2/formset/templates/richtext/bulletlist.html
--rw-r--r--   0 runner    (1001) docker     (123)      195 2023-06-11 11:06:18.000000 django-formset-1.0.dev2/formset/templates/richtext/doc.html
--rw-r--r--   0 runner    (1001) docker     (123)      272 2023-06-11 11:06:18.000000 django-formset-1.0.dev2/formset/templates/richtext/heading.html
--rw-r--r--   0 runner    (1001) docker     (123)        4 2023-06-11 11:06:18.000000 django-formset-1.0.dev2/formset/templates/richtext/horizontalrule.html
--rw-r--r--   0 runner    (1001) docker     (123)      201 2023-06-11 11:06:18.000000 django-formset-1.0.dev2/formset/templates/richtext/listitem.html
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-11 11:07:28.340778 django-formset-1.0.dev2/formset/templates/richtext/marks/
--rw-r--r--   0 runner    (1001) docker     (123)       27 2023-06-11 11:06:18.000000 django-formset-1.0.dev2/formset/templates/richtext/marks/bold.html
--rw-r--r--   0 runner    (1001) docker     (123)       23 2023-06-11 11:06:18.000000 django-formset-1.0.dev2/formset/templates/richtext/marks/code.html
--rw-r--r--   0 runner    (1001) docker     (123)       19 2023-06-11 11:06:18.000000 django-formset-1.0.dev2/formset/templates/richtext/marks/italic.html
--rw-r--r--   0 runner    (1001) docker     (123)       71 2023-06-11 11:06:18.000000 django-formset-1.0.dev2/formset/templates/richtext/marks/link.html
--rw-r--r--   0 runner    (1001) docker     (123)       17 2023-06-11 11:06:18.000000 django-formset-1.0.dev2/formset/templates/richtext/marks/underline.html
--rw-r--r--   0 runner    (1001) docker     (123)      201 2023-06-11 11:06:18.000000 django-formset-1.0.dev2/formset/templates/richtext/orderedlist.html
--rw-r--r--   0 runner    (1001) docker     (123)      204 2023-06-11 11:06:18.000000 django-formset-1.0.dev2/formset/templates/richtext/paragraph.html
--rw-r--r--   0 runner    (1001) docker     (123)      205 2023-06-11 11:06:18.000000 django-formset-1.0.dev2/formset/templates/richtext/text.html
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-11 11:07:28.340778 django-formset-1.0.dev2/formset/templatetags/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-11 11:06:18.000000 django-formset-1.0.dev2/formset/templatetags/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2428 2023-06-11 11:06:18.000000 django-formset-1.0.dev2/formset/templatetags/formsetify.py
--rw-r--r--   0 runner    (1001) docker     (123)      502 2023-06-11 11:06:18.000000 django-formset-1.0.dev2/formset/templatetags/richtext.py
--rw-r--r--   0 runner    (1001) docker     (123)     5703 2023-06-11 11:06:18.000000 django-formset-1.0.dev2/formset/upload.py
--rw-r--r--   0 runner    (1001) docker     (123)     5477 2023-06-11 11:06:18.000000 django-formset-1.0.dev2/formset/utils.py
--rw-r--r--   0 runner    (1001) docker     (123)    11553 2023-06-11 11:06:18.000000 django-formset-1.0.dev2/formset/views.py
--rw-r--r--   0 runner    (1001) docker     (123)    15216 2023-06-11 11:06:18.000000 django-formset-1.0.dev2/formset/widgets.py
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-11 11:07:28.344778 django-formset-1.0.dev2/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1390 2023-06-11 11:06:18.000000 django-formset-1.0.dev2/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-12 21:30:44.435379 django-formset-1.0.dev3/
+-rw-r--r--   0 runner    (1001) docker     (123)     1079 2023-06-12 21:29:25.000000 django-formset-1.0.dev3/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)      244 2023-06-12 21:29:25.000000 django-formset-1.0.dev3/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)    14240 2023-06-12 21:30:44.435379 django-formset-1.0.dev3/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    13295 2023-06-12 21:29:25.000000 django-formset-1.0.dev3/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-12 21:30:44.395378 django-formset-1.0.dev3/django_formset.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    14240 2023-06-12 21:30:44.000000 django-formset-1.0.dev3/django_formset.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    10260 2023-06-12 21:30:44.000000 django-formset-1.0.dev3/django_formset.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-12 21:30:44.000000 django-formset-1.0.dev3/django_formset.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-12 21:30:44.000000 django-formset-1.0.dev3/django_formset.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)       12 2023-06-12 21:30:44.000000 django-formset-1.0.dev3/django_formset.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       16 2023-06-12 21:30:44.000000 django-formset-1.0.dev3/django_formset.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-12 21:30:44.395378 django-formset-1.0.dev3/formset/
+-rw-r--r--   0 runner    (1001) docker     (123)       25 2023-06-12 21:29:25.000000 django-formset-1.0.dev3/formset/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8860 2023-06-12 21:29:25.000000 django-formset-1.0.dev3/formset/boundfield.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7637 2023-06-12 21:29:25.000000 django-formset-1.0.dev3/formset/calendar.py
+-rw-r--r--   0 runner    (1001) docker     (123)    20763 2023-06-12 21:29:25.000000 django-formset-1.0.dev3/formset/collection.py
+-rw-r--r--   0 runner    (1001) docker     (123)      101 2023-06-12 21:29:25.000000 django-formset-1.0.dev3/formset/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2913 2023-06-12 21:29:25.000000 django-formset-1.0.dev3/formset/fields.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2098 2023-06-12 21:29:25.000000 django-formset-1.0.dev3/formset/fieldset.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-12 21:30:44.387378 django-formset-1.0.dev3/formset/locale/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-12 21:30:44.387378 django-formset-1.0.dev3/formset/locale/de/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-12 21:30:44.395378 django-formset-1.0.dev3/formset/locale/de/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (123)     3444 2023-06-12 21:30:36.000000 django-formset-1.0.dev3/formset/locale/de/LC_MESSAGES/django.mo
+-rw-r--r--   0 runner    (1001) docker     (123)     7554 2023-06-12 21:29:25.000000 django-formset-1.0.dev3/formset/locale/de/LC_MESSAGES/django.po
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-12 21:30:44.399378 django-formset-1.0.dev3/formset/renderers/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-12 21:29:25.000000 django-formset-1.0.dev3/formset/renderers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5328 2023-06-12 21:29:25.000000 django-formset-1.0.dev3/formset/renderers/bootstrap.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3302 2023-06-12 21:29:25.000000 django-formset-1.0.dev3/formset/renderers/bulma.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6647 2023-06-12 21:29:25.000000 django-formset-1.0.dev3/formset/renderers/default.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1964 2023-06-12 21:29:25.000000 django-formset-1.0.dev3/formset/renderers/foundation.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5111 2023-06-12 21:29:25.000000 django-formset-1.0.dev3/formset/renderers/tailwind.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2851 2023-06-12 21:29:25.000000 django-formset-1.0.dev3/formset/renderers/uikit.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-12 21:30:44.399378 django-formset-1.0.dev3/formset/richtext/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-12 21:29:25.000000 django-formset-1.0.dev3/formset/richtext/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7308 2023-06-12 21:29:25.000000 django-formset-1.0.dev3/formset/richtext/controls.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1456 2023-06-12 21:29:25.000000 django-formset-1.0.dev3/formset/richtext/dialogs.py
+-rw-r--r--   0 runner    (1001) docker     (123)      353 2023-06-12 21:29:25.000000 django-formset-1.0.dev3/formset/richtext/fields.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2043 2023-06-12 21:29:25.000000 django-formset-1.0.dev3/formset/richtext/widgets.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-12 21:30:44.387378 django-formset-1.0.dev3/formset/static/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-12 21:30:44.387378 django-formset-1.0.dev3/formset/static/formset/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-12 21:30:44.399378 django-formset-1.0.dev3/formset/static/formset/css/
+-rw-r--r--   0 runner    (1001) docker     (123)     2401 2023-06-12 21:30:33.000000 django-formset-1.0.dev3/formset/static/formset/css/bootstrap5-extra.css
+-rw-r--r--   0 runner    (1001) docker     (123)      716 2023-06-12 21:30:33.000000 django-formset-1.0.dev3/formset/static/formset/css/bootstrap5-extra.css.map
+-rw-r--r--   0 runner    (1001) docker     (123)     1830 2023-06-12 21:30:33.000000 django-formset-1.0.dev3/formset/static/formset/css/collections.css
+-rw-r--r--   0 runner    (1001) docker     (123)      354 2023-06-12 21:30:33.000000 django-formset-1.0.dev3/formset/static/formset/css/collections.css.map
+-rw-r--r--   0 runner    (1001) docker     (123)    35875 2023-06-12 21:30:34.000000 django-formset-1.0.dev3/formset/static/formset/css/tailwind.css
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-12 21:30:44.403378 django-formset-1.0.dev3/formset/static/formset/icons/
+-rw-r--r--   0 runner    (1001) docker     (123)     1516 2023-06-12 21:29:25.000000 django-formset-1.0.dev3/formset/static/formset/icons/file-audio.svg
+-rw-r--r--   0 runner    (1001) docker     (123)      637 2023-06-12 21:29:25.000000 django-formset-1.0.dev3/formset/static/formset/icons/file-empty.svg
+-rw-r--r--   0 runner    (1001) docker     (123)     1258 2023-06-12 21:29:25.000000 django-formset-1.0.dev3/formset/static/formset/icons/file-font.svg
+-rw-r--r--   0 runner    (1001) docker     (123)     3181 2023-06-12 21:29:25.000000 django-formset-1.0.dev3/formset/static/formset/icons/file-missing.svg
+-rw-r--r--   0 runner    (1001) docker     (123)     1958 2023-06-12 21:29:25.000000 django-formset-1.0.dev3/formset/static/formset/icons/file-pdf.svg
+-rw-r--r--   0 runner    (1001) docker     (123)     1031 2023-06-12 21:29:25.000000 django-formset-1.0.dev3/formset/static/formset/icons/file-picture.svg
+-rw-r--r--   0 runner    (1001) docker     (123)     2071 2023-06-12 21:29:25.000000 django-formset-1.0.dev3/formset/static/formset/icons/file-unknown.svg
+-rw-r--r--   0 runner    (1001) docker     (123)     2911 2023-06-12 21:29:25.000000 django-formset-1.0.dev3/formset/static/formset/icons/file-video.svg
+-rw-r--r--   0 runner    (1001) docker     (123)     1838 2023-06-12 21:29:25.000000 django-formset-1.0.dev3/formset/static/formset/icons/file-zip.svg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-12 21:30:44.407378 django-formset-1.0.dev3/formset/static/formset/js/
+-rw-r--r--   0 runner    (1001) docker     (123)    25407 2023-06-12 21:30:35.000000 django-formset-1.0.dev3/formset/static/formset/js/DateTimePicker-OYPFNQAF.js
+-rw-r--r--   0 runner    (1001) docker     (123)    55721 2023-06-12 21:30:35.000000 django-formset-1.0.dev3/formset/static/formset/js/DjangoSelectize-H6QF7W4R.js
+-rw-r--r--   0 runner    (1001) docker     (123)    11534 2023-06-12 21:30:35.000000 django-formset-1.0.dev3/formset/static/formset/js/DjangoSlug-226MVQ6E.js
+-rw-r--r--   0 runner    (1001) docker     (123)    12352 2023-06-12 21:30:35.000000 django-formset-1.0.dev3/formset/static/formset/js/DualSelector-GVLJZFWV.js
+-rw-r--r--   0 runner    (1001) docker     (123)   316874 2023-06-12 21:30:35.000000 django-formset-1.0.dev3/formset/static/formset/js/RichtextArea-UTSZPGIP.js
+-rw-r--r--   0 runner    (1001) docker     (123)      196 2023-06-12 21:30:35.000000 django-formset-1.0.dev3/formset/static/formset/js/SortableSelect-4MNY532K.js
+-rw-r--r--   0 runner    (1001) docker     (123)     1713 2023-06-12 21:30:35.000000 django-formset-1.0.dev3/formset/static/formset/js/chunk-AELXO3WZ.js
+-rw-r--r--   0 runner    (1001) docker     (123)    43947 2023-06-12 21:30:35.000000 django-formset-1.0.dev3/formset/static/formset/js/chunk-APVD22ED.js
+-rw-r--r--   0 runner    (1001) docker     (123)     3967 2023-06-12 21:30:35.000000 django-formset-1.0.dev3/formset/static/formset/js/chunk-IE6INVWL.js
+-rw-r--r--   0 runner    (1001) docker     (123)    12466 2023-06-12 21:30:35.000000 django-formset-1.0.dev3/formset/static/formset/js/chunk-ISEEQP4V.js
+-rw-r--r--   0 runner    (1001) docker     (123)     9669 2023-06-12 21:30:35.000000 django-formset-1.0.dev3/formset/static/formset/js/chunk-KDP4ZIAK.js
+-rw-r--r--   0 runner    (1001) docker     (123)      544 2023-06-12 21:30:35.000000 django-formset-1.0.dev3/formset/static/formset/js/chunk-NLMHZ7JJ.js
+-rw-r--r--   0 runner    (1001) docker     (123)     1850 2023-06-12 21:30:35.000000 django-formset-1.0.dev3/formset/static/formset/js/chunk-O5UGFU32.js
+-rw-r--r--   0 runner    (1001) docker     (123)   106347 2023-06-12 21:30:35.000000 django-formset-1.0.dev3/formset/static/formset/js/django-formset.js
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-12 21:30:44.407378 django-formset-1.0.dev3/formset/static/formset/scss/
+-rw-r--r--   0 runner    (1001) docker     (123)     2284 2023-06-12 21:29:25.000000 django-formset-1.0.dev3/formset/static/formset/scss/bootstrap5-extra.scss
+-rw-r--r--   0 runner    (1001) docker     (123)     1497 2023-06-12 21:29:25.000000 django-formset-1.0.dev3/formset/static/formset/scss/collections.scss
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-12 21:30:44.391378 django-formset-1.0.dev3/formset/templates/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-12 21:30:44.387378 django-formset-1.0.dev3/formset/templates/admin/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-12 21:30:44.407378 django-formset-1.0.dev3/formset/templates/admin/formset/
+-rw-r--r--   0 runner    (1001) docker     (123)      344 2023-06-12 21:29:25.000000 django-formset-1.0.dev3/formset/templates/admin/formset/change_form.html
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-12 21:30:44.407378 django-formset-1.0.dev3/formset/templates/calendar/
+-rw-r--r--   0 runner    (1001) docker     (123)     1360 2023-06-12 21:29:25.000000 django-formset-1.0.dev3/formset/templates/calendar/hours.html
+-rw-r--r--   0 runner    (1001) docker     (123)     1176 2023-06-12 21:29:25.000000 django-formset-1.0.dev3/formset/templates/calendar/months.html
+-rw-r--r--   0 runner    (1001) docker     (123)     1208 2023-06-12 21:29:25.000000 django-formset-1.0.dev3/formset/templates/calendar/weeks.html
+-rw-r--r--   0 runner    (1001) docker     (123)     1132 2023-06-12 21:29:25.000000 django-formset-1.0.dev3/formset/templates/calendar/years.html
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-12 21:30:44.407378 django-formset-1.0.dev3/formset/templates/formset/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-12 21:30:44.407378 django-formset-1.0.dev3/formset/templates/formset/bootstrap/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-12 21:30:44.407378 django-formset-1.0.dev3/formset/templates/formset/bootstrap/buttons/
+-rw-r--r--   0 runner    (1001) docker     (123)      176 2023-06-12 21:29:25.000000 django-formset-1.0.dev3/formset/templates/formset/bootstrap/buttons/add_collection.html
+-rw-r--r--   0 runner    (1001) docker     (123)      134 2023-06-12 21:29:25.000000 django-formset-1.0.dev3/formset/templates/formset/bootstrap/buttons/remove_collection.html
+-rw-r--r--   0 runner    (1001) docker     (123)      194 2023-06-12 21:29:25.000000 django-formset-1.0.dev3/formset/templates/formset/bootstrap/buttons/richtext_align.html
+-rw-r--r--   0 runner    (1001) docker     (123)      194 2023-06-12 21:29:25.000000 django-formset-1.0.dev3/formset/templates/formset/bootstrap/buttons/richtext_color.html
+-rw-r--r--   0 runner    (1001) docker     (123)      196 2023-06-12 21:29:25.000000 django-formset-1.0.dev3/formset/templates/formset/bootstrap/buttons/richtext_heading.html
+-rw-r--r--   0 runner    (1001) docker     (123)      511 2023-06-12 21:29:25.000000 django-formset-1.0.dev3/formset/templates/formset/bootstrap/field_group.html
+-rw-r--r--   0 runner    (1001) docker     (123)      254 2023-06-12 21:29:25.000000 django-formset-1.0.dev3/formset/templates/formset/bootstrap/form.html
+-rw-r--r--   0 runner    (1001) docker     (123)       55 2023-06-12 21:29:25.000000 django-formset-1.0.dev3/formset/templates/formset/bootstrap/help_text.html
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-12 21:30:44.411378 django-formset-1.0.dev3/formset/templates/formset/bootstrap/widgets/
+-rw-r--r--   0 runner    (1001) docker     (123)      181 2023-06-12 21:29:25.000000 django-formset-1.0.dev3/formset/templates/formset/bootstrap/widgets/checkbox.html
+-rw-r--r--   0 runner    (1001) docker     (123)      918 2023-06-12 21:29:25.000000 django-formset-1.0.dev3/formset/templates/formset/bootstrap/widgets/dual_selector.html
+-rw-r--r--   0 runner    (1001) docker     (123)      637 2023-06-12 21:29:25.000000 django-formset-1.0.dev3/formset/templates/formset/bootstrap/widgets/file.html
+-rw-r--r--   0 runner    (1001) docker     (123)      169 2023-06-12 21:29:25.000000 django-formset-1.0.dev3/formset/templates/formset/bootstrap/widgets/input_option.html
+-rw-r--r--   0 runner    (1001) docker     (123)      468 2023-06-12 21:29:25.000000 django-formset-1.0.dev3/formset/templates/formset/bootstrap/widgets/multiple_input.html
+-rw-r--r--   0 runner    (1001) docker     (123)       58 2023-06-12 21:29:25.000000 django-formset-1.0.dev3/formset/templates/formset/bootstrap/widgets/richtextarea.html
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-12 21:30:44.411378 django-formset-1.0.dev3/formset/templates/formset/bulma/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-12 21:30:44.411378 django-formset-1.0.dev3/formset/templates/formset/bulma/buttons/
+-rw-r--r--   0 runner    (1001) docker     (123)      124 2023-06-12 21:29:25.000000 django-formset-1.0.dev3/formset/templates/formset/bulma/buttons/add_collection.html
+-rw-r--r--   0 runner    (1001) docker     (123)      122 2023-06-12 21:29:25.000000 django-formset-1.0.dev3/formset/templates/formset/bulma/buttons/remove_collection.html
+-rw-r--r--   0 runner    (1001) docker     (123)      364 2023-06-12 21:29:25.000000 django-formset-1.0.dev3/formset/templates/formset/bulma/field_group.html
+-rw-r--r--   0 runner    (1001) docker     (123)      253 2023-06-12 21:29:25.000000 django-formset-1.0.dev3/formset/templates/formset/bulma/form.html
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-12 21:30:44.411378 django-formset-1.0.dev3/formset/templates/formset/bulma/widgets/
+-rw-r--r--   0 runner    (1001) docker     (123)      141 2023-06-12 21:29:25.000000 django-formset-1.0.dev3/formset/templates/formset/bulma/widgets/checkbox.html
+-rw-r--r--   0 runner    (1001) docker     (123)     1260 2023-06-12 21:29:25.000000 django-formset-1.0.dev3/formset/templates/formset/bulma/widgets/dual_selector.html
+-rw-r--r--   0 runner    (1001) docker     (123)      669 2023-06-12 21:29:25.000000 django-formset-1.0.dev3/formset/templates/formset/bulma/widgets/file.html
+-rw-r--r--   0 runner    (1001) docker     (123)      183 2023-06-12 21:29:25.000000 django-formset-1.0.dev3/formset/templates/formset/bulma/widgets/input_option.html
+-rw-r--r--   0 runner    (1001) docker     (123)      396 2023-06-12 21:29:25.000000 django-formset-1.0.dev3/formset/templates/formset/bulma/widgets/multiple_input.html
+-rw-r--r--   0 runner    (1001) docker     (123)      113 2023-06-12 21:29:25.000000 django-formset-1.0.dev3/formset/templates/formset/bulma/widgets/select.html
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-12 21:30:44.411378 django-formset-1.0.dev3/formset/templates/formset/default/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-12 21:30:44.415378 django-formset-1.0.dev3/formset/templates/formset/default/buttons/
+-rw-r--r--   0 runner    (1001) docker     (123)      361 2023-06-12 21:29:25.000000 django-formset-1.0.dev3/formset/templates/formset/default/buttons/add_collection.html
+-rw-r--r--   0 runner    (1001) docker     (123)      204 2023-06-12 21:29:25.000000 django-formset-1.0.dev3/formset/templates/formset/default/buttons/move_all_left.html
+-rw-r--r--   0 runner    (1001) docker     (123)      207 2023-06-12 21:29:25.000000 django-formset-1.0.dev3/formset/templates/formset/default/buttons/move_all_right.html
+-rw-r--r--   0 runner    (1001) docker     (123)      207 2023-06-12 21:29:25.000000 django-formset-1.0.dev3/formset/templates/formset/default/buttons/move_selected_left.html
+-rw-r--r--   0 runner    (1001) docker     (123)      210 2023-06-12 21:29:25.000000 django-formset-1.0.dev3/formset/templates/formset/default/buttons/move_selected_right.html
+-rw-r--r--   0 runner    (1001) docker     (123)      189 2023-06-12 21:29:25.000000 django-formset-1.0.dev3/formset/templates/formset/default/buttons/redo_selected.html
+-rw-r--r--   0 runner    (1001) docker     (123)      233 2023-06-12 21:29:25.000000 django-formset-1.0.dev3/formset/templates/formset/default/buttons/remove_collection.html
+-rw-r--r--   0 runner    (1001) docker     (123)      959 2023-06-12 21:29:25.000000 django-formset-1.0.dev3/formset/templates/formset/default/buttons/richtext_align.html
+-rw-r--r--   0 runner    (1001) docker     (123)      692 2023-06-12 21:29:25.000000 django-formset-1.0.dev3/formset/templates/formset/default/buttons/richtext_color.html
+-rw-r--r--   0 runner    (1001) docker     (123)      102 2023-06-12 21:29:25.000000 django-formset-1.0.dev3/formset/templates/formset/default/buttons/richtext_control.html
+-rw-r--r--   0 runner    (1001) docker     (123)      843 2023-06-12 21:29:25.000000 django-formset-1.0.dev3/formset/templates/formset/default/buttons/richtext_heading.html
+-rw-r--r--   0 runner    (1001) docker     (123)       92 2023-06-12 21:29:25.000000 django-formset-1.0.dev3/formset/templates/formset/default/buttons/richtext_separator.html
+-rw-r--r--   0 runner    (1001) docker     (123)      189 2023-06-12 21:29:25.000000 django-formset-1.0.dev3/formset/templates/formset/default/buttons/undo_selected.html
+-rw-r--r--   0 runner    (1001) docker     (123)     1504 2023-06-12 21:29:25.000000 django-formset-1.0.dev3/formset/templates/formset/default/collection.html
+-rw-r--r--   0 runner    (1001) docker     (123)      864 2023-06-12 21:29:25.000000 django-formset-1.0.dev3/formset/templates/formset/default/dialog_form.html
+-rw-r--r--   0 runner    (1001) docker     (123)      300 2023-06-12 21:29:25.000000 django-formset-1.0.dev3/formset/templates/formset/default/field_errors.html
+-rw-r--r--   0 runner    (1001) docker     (123)      407 2023-06-12 21:29:25.000000 django-formset-1.0.dev3/formset/templates/formset/default/field_group.html
+-rw-r--r--   0 runner    (1001) docker     (123)      677 2023-06-12 21:29:25.000000 django-formset-1.0.dev3/formset/templates/formset/default/fieldset.html
+-rw-r--r--   0 runner    (1001) docker     (123)      415 2023-06-12 21:29:25.000000 django-formset-1.0.dev3/formset/templates/formset/default/form.html
+-rw-r--r--   0 runner    (1001) docker     (123)       47 2023-06-12 21:29:25.000000 django-formset-1.0.dev3/formset/templates/formset/default/help_text.html
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-12 21:30:44.415378 django-formset-1.0.dev3/formset/templates/formset/default/widgets/
+-rw-r--r--   0 runner    (1001) docker     (123)      149 2023-06-12 21:29:25.000000 django-formset-1.0.dev3/formset/templates/formset/default/widgets/datetimepicker.html
+-rw-r--r--   0 runner    (1001) docker     (123)     2416 2023-06-12 21:29:25.000000 django-formset-1.0.dev3/formset/templates/formset/default/widgets/dual_selector.html
+-rw-r--r--   0 runner    (1001) docker     (123)     1407 2023-06-12 21:29:25.000000 django-formset-1.0.dev3/formset/templates/formset/default/widgets/file.html
+-rw-r--r--   0 runner    (1001) docker     (123)      454 2023-06-12 21:29:25.000000 django-formset-1.0.dev3/formset/templates/formset/default/widgets/multiple_input.html
+-rw-r--r--   0 runner    (1001) docker     (123)      446 2023-06-12 21:29:25.000000 django-formset-1.0.dev3/formset/templates/formset/default/widgets/richtextarea.html
+-rw-r--r--   0 runner    (1001) docker     (123)       48 2023-06-12 21:29:25.000000 django-formset-1.0.dev3/formset/templates/formset/default/widgets/select.html
+-rw-r--r--   0 runner    (1001) docker     (123)     1048 2023-06-12 21:29:25.000000 django-formset-1.0.dev3/formset/templates/formset/default/widgets/selectize.html
+-rw-r--r--   0 runner    (1001) docker     (123)      216 2023-06-12 21:29:25.000000 django-formset-1.0.dev3/formset/templates/formset/form_attrs.html
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-12 21:30:44.415378 django-formset-1.0.dev3/formset/templates/formset/foundation/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-12 21:30:44.419378 django-formset-1.0.dev3/formset/templates/formset/foundation/buttons/
+-rw-r--r--   0 runner    (1001) docker     (123)      132 2023-06-12 21:29:25.000000 django-formset-1.0.dev3/formset/templates/formset/foundation/buttons/add_collection.html
+-rw-r--r--   0 runner    (1001) docker     (123)      128 2023-06-12 21:29:25.000000 django-formset-1.0.dev3/formset/templates/formset/foundation/buttons/remove_collection.html
+-rw-r--r--   0 runner    (1001) docker     (123)      390 2023-06-12 21:29:25.000000 django-formset-1.0.dev3/formset/templates/formset/foundation/field_group.html
+-rw-r--r--   0 runner    (1001) docker     (123)      258 2023-06-12 21:29:25.000000 django-formset-1.0.dev3/formset/templates/formset/foundation/form.html
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-12 21:30:44.419378 django-formset-1.0.dev3/formset/templates/formset/foundation/widgets/
+-rw-r--r--   0 runner    (1001) docker     (123)      123 2023-06-12 21:29:25.000000 django-formset-1.0.dev3/formset/templates/formset/foundation/widgets/checkbox.html
+-rw-r--r--   0 runner    (1001) docker     (123)      835 2023-06-12 21:29:25.000000 django-formset-1.0.dev3/formset/templates/formset/foundation/widgets/dual_selector.html
+-rw-r--r--   0 runner    (1001) docker     (123)      654 2023-06-12 21:29:25.000000 django-formset-1.0.dev3/formset/templates/formset/foundation/widgets/file.html
+-rw-r--r--   0 runner    (1001) docker     (123)      145 2023-06-12 21:29:25.000000 django-formset-1.0.dev3/formset/templates/formset/foundation/widgets/inlined_input_option.html
+-rw-r--r--   0 runner    (1001) docker     (123)      340 2023-06-12 21:29:25.000000 django-formset-1.0.dev3/formset/templates/formset/foundation/widgets/multiple_input.html
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-12 21:30:44.427379 django-formset-1.0.dev3/formset/templates/formset/icons/
+-rw-r--r--   0 runner    (1001) docker     (123)      196 2023-06-12 21:29:25.000000 django-formset-1.0.dev3/formset/templates/formset/icons/add-fill.svg
+-rw-r--r--   0 runner    (1001) docker     (123)      193 2023-06-12 21:29:25.000000 django-formset-1.0.dev3/formset/templates/formset/icons/align-center.svg
+-rw-r--r--   0 runner    (1001) docker     (123)      193 2023-06-12 21:29:25.000000 django-formset-1.0.dev3/formset/templates/formset/icons/align-justify.svg
+-rw-r--r--   0 runner    (1001) docker     (123)      193 2023-06-12 21:29:25.000000 django-formset-1.0.dev3/formset/templates/formset/icons/align-left.svg
+-rw-r--r--   0 runner    (1001) docker     (123)      193 2023-06-12 21:29:25.000000 django-formset-1.0.dev3/formset/templates/formset/icons/align-right.svg
+-rw-r--r--   0 runner    (1001) docker     (123)      237 2023-06-12 21:29:25.000000 django-formset-1.0.dev3/formset/templates/formset/icons/arrow-left.svg
+-rw-r--r--   0 runner    (1001) docker     (123)      245 2023-06-12 21:29:25.000000 django-formset-1.0.dev3/formset/templates/formset/icons/arrow-right.svg
+-rw-r--r--   0 runner    (1001) docker     (123)      248 2023-06-12 21:29:25.000000 django-formset-1.0.dev3/formset/templates/formset/icons/arrow-up.svg
+-rw-r--r--   0 runner    (1001) docker     (123)      792 2023-06-12 21:29:25.000000 django-formset-1.0.dev3/formset/templates/formset/icons/blockquote.svg
+-rw-r--r--   0 runner    (1001) docker     (123)      408 2023-06-12 21:29:25.000000 django-formset-1.0.dev3/formset/templates/formset/icons/bold.svg
+-rw-r--r--   0 runner    (1001) docker     (123)      252 2023-06-12 21:29:25.000000 django-formset-1.0.dev3/formset/templates/formset/icons/bulletlist.svg
+-rw-r--r--   0 runner    (1001) docker     (123)      463 2023-06-12 21:29:25.000000 django-formset-1.0.dev3/formset/templates/formset/icons/calendar-today.svg
+-rw-r--r--   0 runner    (1001) docker     (123)      318 2023-06-12 21:29:25.000000 django-formset-1.0.dev3/formset/templates/formset/icons/chevron-double-left.svg
+-rw-r--r--   0 runner    (1001) docker     (123)      312 2023-06-12 21:29:25.000000 django-formset-1.0.dev3/formset/templates/formset/icons/chevron-double-right.svg
+-rw-r--r--   0 runner    (1001) docker     (123)      225 2023-06-12 21:29:25.000000 django-formset-1.0.dev3/formset/templates/formset/icons/chevron-left.svg
+-rw-r--r--   0 runner    (1001) docker     (123)      228 2023-06-12 21:29:25.000000 django-formset-1.0.dev3/formset/templates/formset/icons/chevron-right.svg
+-rw-r--r--   0 runner    (1001) docker     (123)      329 2023-06-12 21:29:25.000000 django-formset-1.0.dev3/formset/templates/formset/icons/clearformat.svg
+-rw-r--r--   0 runner    (1001) docker     (123)      359 2023-06-12 21:29:25.000000 django-formset-1.0.dev3/formset/templates/formset/icons/codeblock.svg
+-rw-r--r--   0 runner    (1001) docker     (123)      219 2023-06-12 21:29:25.000000 django-formset-1.0.dev3/formset/templates/formset/icons/decreasemargin.svg
+-rw-r--r--   0 runner    (1001) docker     (123)      467 2023-06-12 21:29:25.000000 django-formset-1.0.dev3/formset/templates/formset/icons/delete-back.svg
+-rw-r--r--   0 runner    (1001) docker     (123)      456 2023-06-12 21:29:25.000000 django-formset-1.0.dev3/formset/templates/formset/icons/double-chevron-left.svg
+-rw-r--r--   0 runner    (1001) docker     (123)      463 2023-06-12 21:29:25.000000 django-formset-1.0.dev3/formset/templates/formset/icons/double-chevron-right.svg
+-rw-r--r--   0 runner    (1001) docker     (123)      323 2023-06-12 21:29:25.000000 django-formset-1.0.dev3/formset/templates/formset/icons/hardbreak.svg
+-rw-r--r--   0 runner    (1001) docker     (123)      195 2023-06-12 21:29:25.000000 django-formset-1.0.dev3/formset/templates/formset/icons/heading.svg
+-rw-r--r--   0 runner    (1001) docker     (123)      239 2023-06-12 21:29:25.000000 django-formset-1.0.dev3/formset/templates/formset/icons/heading1.svg
+-rw-r--r--   0 runner    (1001) docker     (123)      429 2023-06-12 21:29:25.000000 django-formset-1.0.dev3/formset/templates/formset/icons/heading2.svg
+-rw-r--r--   0 runner    (1001) docker     (123)      457 2023-06-12 21:29:25.000000 django-formset-1.0.dev3/formset/templates/formset/icons/heading3.svg
+-rw-r--r--   0 runner    (1001) docker     (123)      272 2023-06-12 21:29:25.000000 django-formset-1.0.dev3/formset/templates/formset/icons/heading4.svg
+-rw-r--r--   0 runner    (1001) docker     (123)      431 2023-06-12 21:29:25.000000 django-formset-1.0.dev3/formset/templates/formset/icons/heading5.svg
+-rw-r--r--   0 runner    (1001) docker     (123)      371 2023-06-12 21:29:25.000000 django-formset-1.0.dev3/formset/templates/formset/icons/heading6.svg
+-rw-r--r--   0 runner    (1001) docker     (123)      182 2023-06-12 21:29:25.000000 django-formset-1.0.dev3/formset/templates/formset/icons/horizontalrule.svg
+-rw-r--r--   0 runner    (1001) docker     (123)      397 2023-06-12 21:29:25.000000 django-formset-1.0.dev3/formset/templates/formset/icons/image.svg
+-rw-r--r--   0 runner    (1001) docker     (123)      219 2023-06-12 21:29:25.000000 django-formset-1.0.dev3/formset/templates/formset/icons/increasemargin.svg
+-rw-r--r--   0 runner    (1001) docker     (123)      214 2023-06-12 21:29:25.000000 django-formset-1.0.dev3/formset/templates/formset/icons/indentfirstline.svg
+-rw-r--r--   0 runner    (1001) docker     (123)      218 2023-06-12 21:29:25.000000 django-formset-1.0.dev3/formset/templates/formset/icons/italic.svg
+-rw-r--r--   0 runner    (1001) docker     (123)      632 2023-06-12 21:29:25.000000 django-formset-1.0.dev3/formset/templates/formset/icons/letters.svg
+-rw-r--r--   0 runner    (1001) docker     (123)      475 2023-06-12 21:29:25.000000 django-formset-1.0.dev3/formset/templates/formset/icons/link.svg
+-rw-r--r--   0 runner    (1001) docker     (123)      308 2023-06-12 21:29:25.000000 django-formset-1.0.dev3/formset/templates/formset/icons/orderedlist.svg
+-rw-r--r--   0 runner    (1001) docker     (123)      214 2023-06-12 21:29:25.000000 django-formset-1.0.dev3/formset/templates/formset/icons/outdentfirstline.svg
+-rw-r--r--   0 runner    (1001) docker     (123)     1226 2023-06-12 21:29:25.000000 django-formset-1.0.dev3/formset/templates/formset/icons/placeholder.svg
+-rw-r--r--   0 runner    (1001) docker     (123)      529 2023-06-12 21:29:25.000000 django-formset-1.0.dev3/formset/templates/formset/icons/questionmark.svg
+-rw-r--r--   0 runner    (1001) docker     (123)      280 2023-06-12 21:29:25.000000 django-formset-1.0.dev3/formset/templates/formset/icons/redo.svg
+-rw-r--r--   0 runner    (1001) docker     (123)      457 2023-06-12 21:29:25.000000 django-formset-1.0.dev3/formset/templates/formset/icons/send.svg
+-rw-r--r--   0 runner    (1001) docker     (123)      200 2023-06-12 21:29:25.000000 django-formset-1.0.dev3/formset/templates/formset/icons/separator.svg
+-rw-r--r--   0 runner    (1001) docker     (123)      514 2023-06-12 21:29:25.000000 django-formset-1.0.dev3/formset/templates/formset/icons/subscript.svg
+-rw-r--r--   0 runner    (1001) docker     (123)      501 2023-06-12 21:29:25.000000 django-formset-1.0.dev3/formset/templates/formset/icons/superscript.svg
+-rw-r--r--   0 runner    (1001) docker     (123)      274 2023-06-12 21:29:25.000000 django-formset-1.0.dev3/formset/templates/formset/icons/textcolor.svg
+-rw-r--r--   0 runner    (1001) docker     (123)      309 2023-06-12 21:29:25.000000 django-formset-1.0.dev3/formset/templates/formset/icons/trash.svg
+-rw-r--r--   0 runner    (1001) docker     (123)      225 2023-06-12 21:29:25.000000 django-formset-1.0.dev3/formset/templates/formset/icons/underline.svg
+-rw-r--r--   0 runner    (1001) docker     (123)      275 2023-06-12 21:29:25.000000 django-formset-1.0.dev3/formset/templates/formset/icons/undo.svg
+-rw-r--r--   0 runner    (1001) docker     (123)      513 2023-06-12 21:29:25.000000 django-formset-1.0.dev3/formset/templates/formset/icons/unlink.svg
+-rw-r--r--   0 runner    (1001) docker     (123)      109 2023-06-12 21:29:25.000000 django-formset-1.0.dev3/formset/templates/formset/non_field_errors.html
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-12 21:30:44.427379 django-formset-1.0.dev3/formset/templates/formset/tailwind/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-12 21:30:44.431378 django-formset-1.0.dev3/formset/templates/formset/tailwind/buttons/
+-rw-r--r--   0 runner    (1001) docker     (123)      309 2023-06-12 21:29:25.000000 django-formset-1.0.dev3/formset/templates/formset/tailwind/buttons/add_collection.html
+-rw-r--r--   0 runner    (1001) docker     (123)      262 2023-06-12 21:29:25.000000 django-formset-1.0.dev3/formset/templates/formset/tailwind/buttons/remove_collection.html
+-rw-r--r--   0 runner    (1001) docker     (123)      376 2023-06-12 21:29:25.000000 django-formset-1.0.dev3/formset/templates/formset/tailwind/field_group.html
+-rw-r--r--   0 runner    (1001) docker     (123)      256 2023-06-12 21:29:25.000000 django-formset-1.0.dev3/formset/templates/formset/tailwind/form.html
+-rw-r--r--   0 runner    (1001) docker     (123)       48 2023-06-12 21:29:25.000000 django-formset-1.0.dev3/formset/templates/formset/tailwind/help_text.html
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-12 21:30:44.431378 django-formset-1.0.dev3/formset/templates/formset/tailwind/widgets/
+-rw-r--r--   0 runner    (1001) docker     (123)      124 2023-06-12 21:29:25.000000 django-formset-1.0.dev3/formset/templates/formset/tailwind/widgets/checkbox.html
+-rw-r--r--   0 runner    (1001) docker     (123)      884 2023-06-12 21:29:25.000000 django-formset-1.0.dev3/formset/templates/formset/tailwind/widgets/dual_selector.html
+-rw-r--r--   0 runner    (1001) docker     (123)      611 2023-06-12 21:29:25.000000 django-formset-1.0.dev3/formset/templates/formset/tailwind/widgets/file.html
+-rw-r--r--   0 runner    (1001) docker     (123)      144 2023-06-12 21:29:25.000000 django-formset-1.0.dev3/formset/templates/formset/tailwind/widgets/input_option.html
+-rw-r--r--   0 runner    (1001) docker     (123)      454 2023-06-12 21:29:25.000000 django-formset-1.0.dev3/formset/templates/formset/tailwind/widgets/multiple_input.html
+-rw-r--r--   0 runner    (1001) docker     (123)      449 2023-06-12 21:29:25.000000 django-formset-1.0.dev3/formset/templates/formset/tailwind/widgets/radio.html
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-12 21:30:44.431378 django-formset-1.0.dev3/formset/templates/formset/uikit/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-12 21:30:44.431378 django-formset-1.0.dev3/formset/templates/formset/uikit/buttons/
+-rw-r--r--   0 runner    (1001) docker     (123)      113 2023-06-12 21:29:25.000000 django-formset-1.0.dev3/formset/templates/formset/uikit/buttons/add_collection.html
+-rw-r--r--   0 runner    (1001) docker     (123)      116 2023-06-12 21:29:25.000000 django-formset-1.0.dev3/formset/templates/formset/uikit/buttons/remove_collection.html
+-rw-r--r--   0 runner    (1001) docker     (123)      377 2023-06-12 21:29:25.000000 django-formset-1.0.dev3/formset/templates/formset/uikit/field_group.html
+-rw-r--r--   0 runner    (1001) docker     (123)      253 2023-06-12 21:29:25.000000 django-formset-1.0.dev3/formset/templates/formset/uikit/form.html
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-12 21:30:44.431378 django-formset-1.0.dev3/formset/templates/formset/uikit/widgets/
+-rw-r--r--   0 runner    (1001) docker     (123)      125 2023-06-12 21:29:25.000000 django-formset-1.0.dev3/formset/templates/formset/uikit/widgets/checkbox.html
+-rw-r--r--   0 runner    (1001) docker     (123)      681 2023-06-12 21:29:25.000000 django-formset-1.0.dev3/formset/templates/formset/uikit/widgets/file.html
+-rw-r--r--   0 runner    (1001) docker     (123)      227 2023-06-12 21:29:25.000000 django-formset-1.0.dev3/formset/templates/formset/uikit/widgets/input_option.html
+-rw-r--r--   0 runner    (1001) docker     (123)      464 2023-06-12 21:29:25.000000 django-formset-1.0.dev3/formset/templates/formset/uikit/widgets/multiple_input.html
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-12 21:30:44.435379 django-formset-1.0.dev3/formset/templates/richtext/
+-rw-r--r--   0 runner    (1001) docker     (123)      234 2023-06-12 21:29:25.000000 django-formset-1.0.dev3/formset/templates/richtext/bulletlist.html
+-rw-r--r--   0 runner    (1001) docker     (123)      195 2023-06-12 21:29:25.000000 django-formset-1.0.dev3/formset/templates/richtext/doc.html
+-rw-r--r--   0 runner    (1001) docker     (123)      272 2023-06-12 21:29:25.000000 django-formset-1.0.dev3/formset/templates/richtext/heading.html
+-rw-r--r--   0 runner    (1001) docker     (123)        4 2023-06-12 21:29:25.000000 django-formset-1.0.dev3/formset/templates/richtext/horizontalrule.html
+-rw-r--r--   0 runner    (1001) docker     (123)      201 2023-06-12 21:29:25.000000 django-formset-1.0.dev3/formset/templates/richtext/listitem.html
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-12 21:30:44.435379 django-formset-1.0.dev3/formset/templates/richtext/marks/
+-rw-r--r--   0 runner    (1001) docker     (123)       27 2023-06-12 21:29:25.000000 django-formset-1.0.dev3/formset/templates/richtext/marks/bold.html
+-rw-r--r--   0 runner    (1001) docker     (123)       23 2023-06-12 21:29:25.000000 django-formset-1.0.dev3/formset/templates/richtext/marks/code.html
+-rw-r--r--   0 runner    (1001) docker     (123)       19 2023-06-12 21:29:25.000000 django-formset-1.0.dev3/formset/templates/richtext/marks/italic.html
+-rw-r--r--   0 runner    (1001) docker     (123)       71 2023-06-12 21:29:25.000000 django-formset-1.0.dev3/formset/templates/richtext/marks/link.html
+-rw-r--r--   0 runner    (1001) docker     (123)      135 2023-06-12 21:29:25.000000 django-formset-1.0.dev3/formset/templates/richtext/marks/textcolor.html
+-rw-r--r--   0 runner    (1001) docker     (123)       17 2023-06-12 21:29:25.000000 django-formset-1.0.dev3/formset/templates/richtext/marks/underline.html
+-rw-r--r--   0 runner    (1001) docker     (123)      201 2023-06-12 21:29:25.000000 django-formset-1.0.dev3/formset/templates/richtext/orderedlist.html
+-rw-r--r--   0 runner    (1001) docker     (123)      274 2023-06-12 21:29:25.000000 django-formset-1.0.dev3/formset/templates/richtext/paragraph.html
+-rw-r--r--   0 runner    (1001) docker     (123)      200 2023-06-12 21:29:25.000000 django-formset-1.0.dev3/formset/templates/richtext/text.html
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-12 21:30:44.435379 django-formset-1.0.dev3/formset/templatetags/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-12 21:29:25.000000 django-formset-1.0.dev3/formset/templatetags/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2428 2023-06-12 21:29:25.000000 django-formset-1.0.dev3/formset/templatetags/formsetify.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1134 2023-06-12 21:29:25.000000 django-formset-1.0.dev3/formset/templatetags/richtext.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5703 2023-06-12 21:29:25.000000 django-formset-1.0.dev3/formset/upload.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5477 2023-06-12 21:29:25.000000 django-formset-1.0.dev3/formset/utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11553 2023-06-12 21:29:25.000000 django-formset-1.0.dev3/formset/views.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15216 2023-06-12 21:29:25.000000 django-formset-1.0.dev3/formset/widgets.py
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-12 21:30:44.435379 django-formset-1.0.dev3/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1390 2023-06-12 21:29:25.000000 django-formset-1.0.dev3/setup.py
```

### Comparing `django-formset-1.0.dev2/LICENSE` & `django-formset-1.0.dev3/LICENSE`

 * *Files identical despite different names*

### Comparing `django-formset-1.0.dev2/PKG-INFO` & `django-formset-1.0.dev3/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: django-formset
-Version: 1.0.dev2
+Version: 1.0.dev3
 Summary: Prevalidate Django Forms in the browser
 Home-page: https://github.com/jrief/django-formset
 Author: Jacob Rief
 Author-email: jacob.rief@gmail.com
 License: MIT
 Keywords: Django Forms,webcomponent
 Platform: OS Independent
```

### Comparing `django-formset-1.0.dev2/README.md` & `django-formset-1.0.dev3/README.md`

 * *Files identical despite different names*

### Comparing `django-formset-1.0.dev2/django_formset.egg-info/PKG-INFO` & `django-formset-1.0.dev3/django_formset.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: django-formset
-Version: 1.0.dev2
+Version: 1.0.dev3
 Summary: Prevalidate Django Forms in the browser
 Home-page: https://github.com/jrief/django-formset
 Author: Jacob Rief
 Author-email: jacob.rief@gmail.com
 License: MIT
 Keywords: Django Forms,webcomponent
 Platform: OS Independent
```

### Comparing `django-formset-1.0.dev2/django_formset.egg-info/SOURCES.txt` & `django-formset-1.0.dev3/django_formset.egg-info/SOURCES.txt`

 * *Files 1% similar despite different names*

```diff
@@ -43,24 +43,24 @@
 formset/static/formset/icons/file-font.svg
 formset/static/formset/icons/file-missing.svg
 formset/static/formset/icons/file-pdf.svg
 formset/static/formset/icons/file-picture.svg
 formset/static/formset/icons/file-unknown.svg
 formset/static/formset/icons/file-video.svg
 formset/static/formset/icons/file-zip.svg
-formset/static/formset/js/DateTimePicker-64ONYNKG.js
-formset/static/formset/js/DjangoSelectize-MICJ4DHH.js
+formset/static/formset/js/DateTimePicker-OYPFNQAF.js
+formset/static/formset/js/DjangoSelectize-H6QF7W4R.js
 formset/static/formset/js/DjangoSlug-226MVQ6E.js
-formset/static/formset/js/DualSelector-XYVC5VWO.js
-formset/static/formset/js/RichtextArea-63COGKXW.js
-formset/static/formset/js/SortableSelect-WBJL5XGS.js
+formset/static/formset/js/DualSelector-GVLJZFWV.js
+formset/static/formset/js/RichtextArea-UTSZPGIP.js
+formset/static/formset/js/SortableSelect-4MNY532K.js
 formset/static/formset/js/chunk-AELXO3WZ.js
 formset/static/formset/js/chunk-APVD22ED.js
+formset/static/formset/js/chunk-IE6INVWL.js
 formset/static/formset/js/chunk-ISEEQP4V.js
-formset/static/formset/js/chunk-JSQHGMDY.js
 formset/static/formset/js/chunk-KDP4ZIAK.js
 formset/static/formset/js/chunk-NLMHZ7JJ.js
 formset/static/formset/js/chunk-O5UGFU32.js
 formset/static/formset/js/django-formset.js
 formset/static/formset/scss/bootstrap5-extra.scss
 formset/static/formset/scss/collections.scss
 formset/templates/admin/formset/change_form.html
@@ -208,11 +208,12 @@
 formset/templates/richtext/orderedlist.html
 formset/templates/richtext/paragraph.html
 formset/templates/richtext/text.html
 formset/templates/richtext/marks/bold.html
 formset/templates/richtext/marks/code.html
 formset/templates/richtext/marks/italic.html
 formset/templates/richtext/marks/link.html
+formset/templates/richtext/marks/textcolor.html
 formset/templates/richtext/marks/underline.html
 formset/templatetags/__init__.py
 formset/templatetags/formsetify.py
 formset/templatetags/richtext.py
```

### Comparing `django-formset-1.0.dev2/formset/boundfield.py` & `django-formset-1.0.dev3/formset/boundfield.py`

 * *Files identical despite different names*

### Comparing `django-formset-1.0.dev2/formset/calendar.py` & `django-formset-1.0.dev3/formset/calendar.py`

 * *Files identical despite different names*

### Comparing `django-formset-1.0.dev2/formset/collection.py` & `django-formset-1.0.dev3/formset/collection.py`

 * *Files identical despite different names*

### Comparing `django-formset-1.0.dev2/formset/fields.py` & `django-formset-1.0.dev3/formset/fields.py`

 * *Files identical despite different names*

### Comparing `django-formset-1.0.dev2/formset/fieldset.py` & `django-formset-1.0.dev3/formset/fieldset.py`

 * *Files identical despite different names*

### Comparing `django-formset-1.0.dev2/formset/locale/de/LC_MESSAGES/django.mo` & `django-formset-1.0.dev3/formset/locale/de/LC_MESSAGES/django.mo`

 * *Files identical despite different names*

### Comparing `django-formset-1.0.dev2/formset/locale/de/LC_MESSAGES/django.po` & `django-formset-1.0.dev3/formset/locale/de/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `django-formset-1.0.dev2/formset/renderers/bootstrap.py` & `django-formset-1.0.dev3/formset/renderers/tailwind.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,95 +1,116 @@
 from formset.boundfield import ClassList
 from formset.renderers.default import FormRenderer as DefaultFormRenderer
 
 
 class FormRenderer(DefaultFormRenderer):
     max_options_per_line = 4
-    framework = 'bootstrap'
+    framework = 'tailwind'
 
     def __init__(self, **kwargs):
-        kwargs.setdefault('label_css_classes', 'form-label')
+        kwargs.setdefault('label_css_classes', 'formset-label')
         super().__init__(**kwargs)
 
     _template_mapping = dict(DefaultFormRenderer._template_mapping, **{
-        'django/forms/default.html': 'formset/bootstrap/form.html',
-        'django/forms/widgets/checkbox.html': 'formset/bootstrap/widgets/checkbox.html',
-        'django/forms/widgets/radio.html': 'formset/bootstrap/widgets/multiple_input.html',
-        'django/forms/widgets/checkbox_select.html': 'formset/bootstrap/widgets/multiple_input.html',
-        'formset/default/widgets/dual_selector.html': 'formset/bootstrap/widgets/dual_selector.html',
-        'formset/default/widgets/file.html': 'formset/bootstrap/widgets/file.html',
-        'formset/default/widgets/richtextarea.html': 'formset/bootstrap/widgets/richtextarea.html',
+        'django/forms/default.html': 'formset/tailwind/form.html',
+        'django/forms/widgets/checkbox.html': 'formset/tailwind/widgets/checkbox.html',
+        'django/forms/widgets/radio.html': 'formset/tailwind/widgets/multiple_input.html',
+        'formset/default/widgets/dual_selector.html': 'formset/tailwind/widgets/dual_selector.html',
+        'formset/default/widgets/file.html': 'formset/tailwind/widgets/file.html',
+        'django/forms/widgets/checkbox_select.html': 'formset/tailwind/widgets/multiple_input.html',
     })
 
-    def _amend_input(self, context):
-        super()._amend_input(context)
-        context['widget']['attrs']['class'].add('form-control')
+    def _amend_label(self, context):
+        return super()._amend_label(context, hide_checkbox_label=True)
+
+    def _amend_text_input(self, context):
+        context['widget']['attrs']['class'] = ClassList('formset-text-input')
         return context
 
-    def _amend_checkbox(self, context):
-        context['widget']['attrs']['class'] = ClassList('form-check-input')
+    def _amend_email_input(self, context):
+        context['widget']['attrs']['class'] = ClassList('formset-email-input')
+        return context
+
+    def _amend_date_input(self, context):
+        context['widget']['attrs']['class'] = ClassList('formset-date-input')
+        return context
+
+    def _amend_number_input(self, context):
+        context['widget']['attrs']['class'] = ClassList('formset-number-input')
+        return context
+
+    def _amend_password_input(self, context):
+        context['widget']['attrs']['class'] = ClassList('formset-password-input')
+        return context
+
+    def _amend_textarea(self, context):
+        context['widget']['attrs']['class'] = ClassList('formset-textarea')
         return context
 
     def _amend_select(self, context):
-        context['widget']['attrs']['class'] = ClassList('form-select')
+        if context['widget']['attrs'].get('multiple') is True:
+            context['widget']['attrs']['class'] = ClassList('formset-select-multiple')
+        else:
+            context['widget']['attrs']['class'] = ClassList('formset-select')
         return context
 
     def _amend_dual_selector(self, context):
         context.update(
-            select_classes='form-select',
-            lookup_field_classes='form-control form-control-sm',
+            select_classes=ClassList('formset-dual-selector-select'),
+            lookup_field_classes=ClassList('formset-dual-selector-lookup'),
         )
         return context
 
-    def _amend_file(self, context):
-        return context  # intentionally noop
-
-    def _amend_label(self, context):
-        return super()._amend_label(context, hide_checkbox_label=True)
+    def _amend_checkbox(self, context):
+        context['widget']['attrs']['class'] = ClassList('formset-checkbox')
+        return context
 
-    def _amend_multiple_input(self, context):
+    def _amend_multiple_input(self, context, css_class):
         context = super()._amend_multiple_input(context)
         for _, optgroup, _ in context['widget']['optgroups']:
             for option in optgroup:
-                option['attrs']['class'] = ClassList('form-check-input')
-                option['template_name'] = 'formset/bootstrap/widgets/input_option.html'
+                option['template_name'] = 'formset/tailwind/widgets/input_option.html'
+                option['attrs']['class'] = ClassList(css_class)
         return context
 
+    def _amend_checkbox_select(self, context):
+        return self._amend_multiple_input(context, 'formset-checkbox-multiple')
+
+    def _amend_radio(self, context):
+        return self._amend_multiple_input(context, 'formset-radio-select')
+
     def _amend_fieldset(self, context):
         context = super()._amend_fieldset(context)
         context.update(
-            help_text_template='formset/bootstrap/help_text.html',
+            help_text_template='formset/tailwind/help_text.html',
         )
         return context
 
     def _amend_collection(self, context):
         context = super()._amend_collection(context)
         context.update(
-            add_collection_button='formset/bootstrap/buttons/add_collection.html',
-            remove_collection_button='formset/bootstrap/buttons/remove_collection.html',
-            help_text_template='formset/bootstrap/help_text.html',
+            add_collection_button='formset/tailwind/buttons/add_collection.html',
+            remove_collection_button='formset/tailwind/buttons/remove_collection.html',
+            help_text_template='formset/tailwind/help_text.html',
         )
         return context
 
     _context_modifiers = dict(DefaultFormRenderer._context_modifiers, **{
         'django/forms/label.html': _amend_label,
-        'django/forms/widgets/text.html': _amend_input,
-        'django/forms/widgets/email.html': _amend_input,
-        'django/forms/widgets/date.html': _amend_input,
-        'django/forms/widgets/datetime.html': _amend_input,
-        'django/forms/widgets/number.html': _amend_input,
-        'django/forms/widgets/url.html': _amend_input,
-        'django/forms/widgets/password.html': _amend_input,
-        'django/forms/widgets/textarea.html': _amend_input,
+        'django/forms/widgets/text.html': _amend_text_input,
+        'django/forms/widgets/email.html': _amend_email_input,
+        'django/forms/widgets/date.html': _amend_date_input,
+        'django/forms/widgets/number.html': _amend_number_input,
+        'django/forms/widgets/password.html': _amend_password_input,
+        'django/forms/widgets/textarea.html': _amend_textarea,
         'django/forms/widgets/select.html': _amend_select,
         'django/forms/widgets/checkbox.html': _amend_checkbox,
-        'django/forms/widgets/checkbox_select.html': _amend_multiple_input,
-        'django/forms/widgets/radio.html': _amend_multiple_input,
-        'formset/default/widgets/datepicker.html': _amend_input,
-        'formset/default/widgets/datetimepicker.html': _amend_input,
-        'formset/default/widgets/file.html': _amend_file,
+        'django/forms/widgets/checkbox_select.html': _amend_checkbox_select,
+        'django/forms/widgets/radio.html': _amend_radio,
+        'formset/default/widgets/datepicker.html': _amend_date_input,
+        'formset/default/widgets/datetimepicker.html': _amend_date_input,
         'formset/default/widgets/selectize.html': _amend_select,
         'formset/default/widgets/dual_selector.html': _amend_dual_selector,
         'formset/default/fieldset.html': _amend_fieldset,
         'formset/default/collection.html': _amend_collection,
-        'formset/default/widgets/richtextarea.html': _amend_input,
+        'formset/default/widgets/richtextarea.html': _amend_textarea,
     })
```

### Comparing `django-formset-1.0.dev2/formset/renderers/bulma.py` & `django-formset-1.0.dev3/formset/renderers/bulma.py`

 * *Files identical despite different names*

### Comparing `django-formset-1.0.dev2/formset/renderers/foundation.py` & `django-formset-1.0.dev3/formset/renderers/foundation.py`

 * *Files identical despite different names*

### Comparing `django-formset-1.0.dev2/formset/renderers/tailwind.py` & `django-formset-1.0.dev3/formset/renderers/bootstrap.py`

 * *Files 27% similar despite different names*

```diff
@@ -1,116 +1,122 @@
 from formset.boundfield import ClassList
 from formset.renderers.default import FormRenderer as DefaultFormRenderer
 
+from django.utils.html import format_html
+
 
 class FormRenderer(DefaultFormRenderer):
     max_options_per_line = 4
-    framework = 'tailwind'
+    framework = 'bootstrap'
 
     def __init__(self, **kwargs):
-        kwargs.setdefault('label_css_classes', 'formset-label')
+        kwargs.setdefault('label_css_classes', 'form-label')
         super().__init__(**kwargs)
 
     _template_mapping = dict(DefaultFormRenderer._template_mapping, **{
-        'django/forms/default.html': 'formset/tailwind/form.html',
-        'django/forms/widgets/checkbox.html': 'formset/tailwind/widgets/checkbox.html',
-        'django/forms/widgets/radio.html': 'formset/tailwind/widgets/multiple_input.html',
-        'formset/default/widgets/dual_selector.html': 'formset/tailwind/widgets/dual_selector.html',
-        'formset/default/widgets/file.html': 'formset/tailwind/widgets/file.html',
-        'django/forms/widgets/checkbox_select.html': 'formset/tailwind/widgets/multiple_input.html',
+        'django/forms/default.html': 'formset/bootstrap/form.html',
+        'django/forms/widgets/checkbox.html': 'formset/bootstrap/widgets/checkbox.html',
+        'django/forms/widgets/radio.html': 'formset/bootstrap/widgets/multiple_input.html',
+        'django/forms/widgets/checkbox_select.html': 'formset/bootstrap/widgets/multiple_input.html',
+        'formset/default/widgets/dual_selector.html': 'formset/bootstrap/widgets/dual_selector.html',
+        'formset/default/widgets/file.html': 'formset/bootstrap/widgets/file.html',
+        'formset/default/widgets/richtextarea.html': 'formset/bootstrap/widgets/richtextarea.html',
     })
 
-    def _amend_label(self, context):
-        return super()._amend_label(context, hide_checkbox_label=True)
-
-    def _amend_text_input(self, context):
-        context['widget']['attrs']['class'] = ClassList('formset-text-input')
-        return context
-
-    def _amend_email_input(self, context):
-        context['widget']['attrs']['class'] = ClassList('formset-email-input')
-        return context
-
-    def _amend_date_input(self, context):
-        context['widget']['attrs']['class'] = ClassList('formset-date-input')
-        return context
-
-    def _amend_number_input(self, context):
-        context['widget']['attrs']['class'] = ClassList('formset-number-input')
-        return context
-
-    def _amend_password_input(self, context):
-        context['widget']['attrs']['class'] = ClassList('formset-password-input')
+    def _amend_input(self, context):
+        super()._amend_input(context)
+        context['widget']['attrs']['class'].add('form-control')
         return context
 
-    def _amend_textarea(self, context):
-        context['widget']['attrs']['class'] = ClassList('formset-textarea')
+    def _amend_checkbox(self, context):
+        context['widget']['attrs']['class'] = ClassList('form-check-input')
         return context
 
     def _amend_select(self, context):
-        if context['widget']['attrs'].get('multiple') is True:
-            context['widget']['attrs']['class'] = ClassList('formset-select-multiple')
-        else:
-            context['widget']['attrs']['class'] = ClassList('formset-select')
+        context['widget']['attrs']['class'] = ClassList('form-select')
         return context
 
     def _amend_dual_selector(self, context):
         context.update(
-            select_classes=ClassList('formset-dual-selector-select'),
-            lookup_field_classes=ClassList('formset-dual-selector-lookup'),
+            select_classes='form-select',
+            lookup_field_classes='form-control form-control-sm',
         )
         return context
 
-    def _amend_checkbox(self, context):
-        context['widget']['attrs']['class'] = ClassList('formset-checkbox')
-        return context
+    def _amend_file(self, context):
+        return context  # intentionally noop
 
-    def _amend_multiple_input(self, context, css_class):
+    def _amend_label(self, context):
+        return super()._amend_label(context, hide_checkbox_label=True)
+
+    def _amend_multiple_input(self, context):
         context = super()._amend_multiple_input(context)
         for _, optgroup, _ in context['widget']['optgroups']:
             for option in optgroup:
-                option['template_name'] = 'formset/tailwind/widgets/input_option.html'
-                option['attrs']['class'] = ClassList(css_class)
+                option['attrs']['class'] = ClassList('form-check-input')
+                option['template_name'] = 'formset/bootstrap/widgets/input_option.html'
         return context
 
-    def _amend_checkbox_select(self, context):
-        return self._amend_multiple_input(context, 'formset-checkbox-multiple')
-
-    def _amend_radio(self, context):
-        return self._amend_multiple_input(context, 'formset-radio-select')
-
     def _amend_fieldset(self, context):
         context = super()._amend_fieldset(context)
         context.update(
-            help_text_template='formset/tailwind/help_text.html',
+            help_text_template='formset/bootstrap/help_text.html',
         )
         return context
 
     def _amend_collection(self, context):
         context = super()._amend_collection(context)
         context.update(
-            add_collection_button='formset/tailwind/buttons/add_collection.html',
-            remove_collection_button='formset/tailwind/buttons/remove_collection.html',
-            help_text_template='formset/tailwind/help_text.html',
+            add_collection_button='formset/bootstrap/buttons/add_collection.html',
+            remove_collection_button='formset/bootstrap/buttons/remove_collection.html',
+            help_text_template='formset/bootstrap/help_text.html',
         )
         return context
 
     _context_modifiers = dict(DefaultFormRenderer._context_modifiers, **{
         'django/forms/label.html': _amend_label,
-        'django/forms/widgets/text.html': _amend_text_input,
-        'django/forms/widgets/email.html': _amend_email_input,
-        'django/forms/widgets/date.html': _amend_date_input,
-        'django/forms/widgets/number.html': _amend_number_input,
-        'django/forms/widgets/password.html': _amend_password_input,
-        'django/forms/widgets/textarea.html': _amend_textarea,
+        'django/forms/widgets/text.html': _amend_input,
+        'django/forms/widgets/email.html': _amend_input,
+        'django/forms/widgets/date.html': _amend_input,
+        'django/forms/widgets/datetime.html': _amend_input,
+        'django/forms/widgets/number.html': _amend_input,
+        'django/forms/widgets/url.html': _amend_input,
+        'django/forms/widgets/password.html': _amend_input,
+        'django/forms/widgets/textarea.html': _amend_input,
         'django/forms/widgets/select.html': _amend_select,
         'django/forms/widgets/checkbox.html': _amend_checkbox,
-        'django/forms/widgets/checkbox_select.html': _amend_checkbox_select,
-        'django/forms/widgets/radio.html': _amend_radio,
-        'formset/default/widgets/datepicker.html': _amend_date_input,
-        'formset/default/widgets/datetimepicker.html': _amend_date_input,
+        'django/forms/widgets/checkbox_select.html': _amend_multiple_input,
+        'django/forms/widgets/radio.html': _amend_multiple_input,
+        'formset/default/widgets/datepicker.html': _amend_input,
+        'formset/default/widgets/datetimepicker.html': _amend_input,
+        'formset/default/widgets/file.html': _amend_file,
         'formset/default/widgets/selectize.html': _amend_select,
         'formset/default/widgets/dual_selector.html': _amend_dual_selector,
         'formset/default/fieldset.html': _amend_fieldset,
         'formset/default/collection.html': _amend_collection,
-        'formset/default/widgets/richtextarea.html': _amend_textarea,
+        'formset/default/widgets/richtextarea.html': _amend_input,
     })
+
+
+def richtext_attributes(attrs):
+    """
+    Converts the internal representation of node attributes into a specific string such as
+    ``class="specfic-css-class"``. This enforces paragraph styling according to Bootstrap's best practice.
+    """
+    classes = []
+    for key, value in attrs.items():
+        if not value:
+            continue
+        if key == 'textIndent' and value == 'indent':
+            classes.append('text-indent')
+        elif key == 'textIndent' and value == 'outdent':
+            classes.append('text-outdent')
+        elif key == 'textMargin':
+            classes.append(f'text-margin-{value}')
+        elif key == 'textAlign' and value == 'left':
+            classes.append('text-start')
+        elif key == 'textAlign' and value == 'center':
+            classes.append('text-center')
+        elif key == 'textAlign' and value == 'right':
+            classes.append('text-end')
+    attributes = format_html(' class="{}"', ' '.join(classes)) if classes else ''
+    return attributes
```

### Comparing `django-formset-1.0.dev2/formset/renderers/uikit.py` & `django-formset-1.0.dev3/formset/renderers/uikit.py`

 * *Files identical despite different names*

### Comparing `django-formset-1.0.dev2/formset/richtext/controls.py` & `django-formset-1.0.dev3/formset/richtext/controls.py`

 * *Files identical despite different names*

### Comparing `django-formset-1.0.dev2/formset/richtext/dialogs.py` & `django-formset-1.0.dev3/formset/richtext/dialogs.py`

 * *Files identical despite different names*

### Comparing `django-formset-1.0.dev2/formset/richtext/widgets.py` & `django-formset-1.0.dev3/formset/richtext/widgets.py`

 * *Files identical despite different names*

### Comparing `django-formset-1.0.dev2/formset/static/formset/css/collections.css` & `django-formset-1.0.dev3/formset/static/formset/css/collections.css`

 * *Files identical despite different names*

### Comparing `django-formset-1.0.dev2/formset/static/formset/css/tailwind.css` & `django-formset-1.0.dev3/formset/static/formset/css/tailwind.css`

 * *Files identical despite different names*

### Comparing `django-formset-1.0.dev2/formset/static/formset/icons/file-audio.svg` & `django-formset-1.0.dev3/formset/static/formset/icons/file-audio.svg`

 * *Files identical despite different names*

### Comparing `django-formset-1.0.dev2/formset/static/formset/icons/file-empty.svg` & `django-formset-1.0.dev3/formset/static/formset/icons/file-empty.svg`

 * *Files identical despite different names*

### Comparing `django-formset-1.0.dev2/formset/static/formset/icons/file-font.svg` & `django-formset-1.0.dev3/formset/static/formset/icons/file-font.svg`

 * *Files identical despite different names*

### Comparing `django-formset-1.0.dev2/formset/static/formset/icons/file-missing.svg` & `django-formset-1.0.dev3/formset/static/formset/icons/file-missing.svg`

 * *Files identical despite different names*

### Comparing `django-formset-1.0.dev2/formset/static/formset/icons/file-pdf.svg` & `django-formset-1.0.dev3/formset/static/formset/icons/file-pdf.svg`

 * *Files identical despite different names*

### Comparing `django-formset-1.0.dev2/formset/static/formset/icons/file-picture.svg` & `django-formset-1.0.dev3/formset/static/formset/icons/file-picture.svg`

 * *Files identical despite different names*

### Comparing `django-formset-1.0.dev2/formset/static/formset/icons/file-unknown.svg` & `django-formset-1.0.dev3/formset/static/formset/icons/file-unknown.svg`

 * *Files identical despite different names*

### Comparing `django-formset-1.0.dev2/formset/static/formset/icons/file-video.svg` & `django-formset-1.0.dev3/formset/static/formset/icons/file-video.svg`

 * *Files identical despite different names*

### Comparing `django-formset-1.0.dev2/formset/static/formset/icons/file-zip.svg` & `django-formset-1.0.dev3/formset/static/formset/icons/file-zip.svg`

 * *Files identical despite different names*

### Comparing `django-formset-1.0.dev2/formset/static/formset/js/DateTimePicker-64ONYNKG.js` & `django-formset-1.0.dev3/formset/static/formset/js/DateTimePicker-OYPFNQAF.js`

 * *Files identical despite different names*

### Comparing `django-formset-1.0.dev2/formset/static/formset/js/DjangoSelectize-MICJ4DHH.js` & `django-formset-1.0.dev3/formset/static/formset/js/DjangoSelectize-H6QF7W4R.js`

 * *Files identical despite different names*

### Comparing `django-formset-1.0.dev2/formset/static/formset/js/DjangoSlug-226MVQ6E.js` & `django-formset-1.0.dev3/formset/static/formset/js/DjangoSlug-226MVQ6E.js`

 * *Files identical despite different names*

### Comparing `django-formset-1.0.dev2/formset/static/formset/js/DualSelector-XYVC5VWO.js` & `django-formset-1.0.dev3/formset/static/formset/js/DualSelector-GVLJZFWV.js`

 * *Files 1% similar despite different names*

#### js-beautify {}

```diff
@@ -1,14 +1,14 @@
 import {
     a as d
 } from "./chunk-AELXO3WZ.js";
 import {
     a as u,
     b as p
-} from "./chunk-JSQHGMDY.js";
+} from "./chunk-IE6INVWL.js";
 import "./chunk-APVD22ED.js";
 import {
     a as g
 } from "./chunk-KDP4ZIAK.js";
 import {
     a as r
 } from "./chunk-O5UGFU32.js";
```

### Comparing `django-formset-1.0.dev2/formset/static/formset/js/RichtextArea-63COGKXW.js` & `django-formset-1.0.dev3/formset/static/formset/js/RichtextArea-UTSZPGIP.js`

 * *Files 0% similar despite different names*

#### js-beautify {}

```diff
@@ -13127,14 +13127,17 @@
                         if (n.classList.contains(e)) return e
                 },
                 renderHTML: n => this.options.allowedClasses.length === 0 ? {
                     style: `color: ${n.textColor};`
                 } : {
                     class: n.textColor
                 }
+            },
+            classBased: {
+                default: this.options.allowedClasses.length !== 0
             }
         }
     },
     parseHTML() {
         return [{
             tag: "span",
             getAttrs: n => {
@@ -13153,15 +13156,16 @@
         return ["span", n, 0]
     },
     addCommands() {
         return {
             setColor: n => ({
                 commands: e
             }) => e.setMark(this.name, {
-                textColor: n
+                textColor: n,
+                classBased: this.options.allowedClasses.length !== 0
             }),
             unsetColor: () => ({
                 commands: n
             }) => n.unsetMark(this.name)
         }
     }
 });
```

### Comparing `django-formset-1.0.dev2/formset/static/formset/js/chunk-AELXO3WZ.js` & `django-formset-1.0.dev3/formset/static/formset/js/chunk-AELXO3WZ.js`

 * *Files identical despite different names*

### Comparing `django-formset-1.0.dev2/formset/static/formset/js/chunk-APVD22ED.js` & `django-formset-1.0.dev3/formset/static/formset/js/chunk-APVD22ED.js`

 * *Files identical despite different names*

### Comparing `django-formset-1.0.dev2/formset/static/formset/js/chunk-ISEEQP4V.js` & `django-formset-1.0.dev3/formset/static/formset/js/chunk-ISEEQP4V.js`

 * *Files identical despite different names*

### Comparing `django-formset-1.0.dev2/formset/static/formset/js/chunk-JSQHGMDY.js` & `django-formset-1.0.dev3/formset/static/formset/js/chunk-IE6INVWL.js`

 * *Files identical despite different names*

### Comparing `django-formset-1.0.dev2/formset/static/formset/js/chunk-KDP4ZIAK.js` & `django-formset-1.0.dev3/formset/static/formset/js/chunk-KDP4ZIAK.js`

 * *Files identical despite different names*

### Comparing `django-formset-1.0.dev2/formset/static/formset/js/chunk-NLMHZ7JJ.js` & `django-formset-1.0.dev3/formset/static/formset/js/chunk-NLMHZ7JJ.js`

 * *Files identical despite different names*

### Comparing `django-formset-1.0.dev2/formset/static/formset/js/chunk-O5UGFU32.js` & `django-formset-1.0.dev3/formset/static/formset/js/chunk-O5UGFU32.js`

 * *Files identical despite different names*

### Comparing `django-formset-1.0.dev2/formset/static/formset/js/django-formset.js` & `django-formset-1.0.dev3/formset/static/formset/js/django-formset.js`

 * *Files 1% similar despite different names*

#### js-beautify {}

```diff
@@ -3173,43 +3173,43 @@
 
     function n(s, u, f, d = void 0) {
         customElements.get(u) instanceof Function ? s() : (window.customElements.define(u, f, d), window.customElements.whenDefined(u).then(() => s()))
     }
 
     function i(s) {
         s.querySelector('select[is="django-selectize"]') && r.push(new Promise((u, f) => {
-            import("./DjangoSelectize-MICJ4DHH.js").then(({
+            import("./DjangoSelectize-H6QF7W4R.js").then(({
                 DjangoSelectizeElement: d
             }) => {
                 n(u, "django-selectize", d, {
                     extends: "select"
                 })
             }).catch(d => f(d))
         })), s.querySelector("django-sortable-select") ? r.push(new Promise((u, f) => {
-            import("./SortableSelect-WBJL5XGS.js").then(({
+            import("./SortableSelect-4MNY532K.js").then(({
                 SortableSelectElement: d
             }) => {
-                customElements.get("django-sortable-select") instanceof Function ? u() : window.customElements.define("django-sortable-select", d), import("./DualSelector-XYVC5VWO.js").then(({
+                customElements.get("django-sortable-select") instanceof Function ? u() : window.customElements.define("django-sortable-select", d), import("./DualSelector-GVLJZFWV.js").then(({
                     DualSelectorElement: h
                 }) => {
                     customElements.get("django-dual-selector") instanceof Function ? u() : (window.customElements.define("django-dual-selector", h, {
                         extends: "select"
                     }), Promise.all([window.customElements.whenDefined("django-sortable-select"), window.customElements.whenDefined("django-dual-selector")]).then(() => u()))
                 }).catch(h => f(h))
             }).catch(d => f(d))
         })) : s.querySelector('select[is="django-dual-selector"]') && r.push(new Promise((u, f) => {
-            import("./DualSelector-XYVC5VWO.js").then(({
+            import("./DualSelector-GVLJZFWV.js").then(({
                 DualSelectorElement: d
             }) => {
                 n(u, "django-dual-selector", d, {
                     extends: "select"
                 })
             }).catch(d => f(d))
         })), s.querySelector('textarea[is="django-richtext"]') && r.push(new Promise((u, f) => {
-            import("./RichtextArea-63COGKXW.js").then(({
+            import("./RichtextArea-UTSZPGIP.js").then(({
                 RichTextAreaElement: d
             }) => {
                 n(u, "django-richtext", d, {
                     extends: "textarea"
                 })
             }).catch(d => f(d))
         })), s.querySelector('input[is="django-slug"]') && r.push(new Promise((u, f) => {
@@ -3217,23 +3217,23 @@
                 DjangoSlugElement: d
             }) => {
                 n(u, "django-slug", d, {
                     extends: "input"
                 })
             }).catch(d => f(d))
         })), s.querySelector('input[is="django-datepicker"]') && r.push(new Promise((u, f) => {
-            import("./DateTimePicker-64ONYNKG.js").then(({
+            import("./DateTimePicker-OYPFNQAF.js").then(({
                 DatePickerElement: d
             }) => {
                 n(u, "django-datepicker", d, {
                     extends: "input"
                 })
             }).catch(d => f(d))
         })), s.querySelector('input[is="django-datetimepicker"]') && r.push(new Promise((u, f) => {
-            import("./DateTimePicker-64ONYNKG.js").then(({
+            import("./DateTimePicker-OYPFNQAF.js").then(({
                 DateTimePickerElement: d
             }) => {
                 n(u, "django-datetimepicker", d, {
                     extends: "input"
                 })
             }).catch(d => f(d))
         }))
```

### Comparing `django-formset-1.0.dev2/formset/static/formset/scss/bootstrap5-extra.scss` & `django-formset-1.0.dev3/formset/static/formset/scss/bootstrap5-extra.scss`

 * *Files 5% similar despite different names*

```diff
@@ -82,7 +82,20 @@
 			border-bottom-left-radius: $modal-content-inner-border-radius;
 			> * {
 				margin: 0.25rem;
 			}
 		}
 	}
 }
+
+.text-indent {
+	text-indent: 3em;
+}
+.text-outdent {
+	text-indent: -3em;
+	padding-left: 3em;
+}
+@for $indent from 1 through 10 {
+	.text-margin-#{$indent} {
+		margin-left: #{2 * $indent}em;
+	}
+}
```

### Comparing `django-formset-1.0.dev2/formset/static/formset/scss/collections.scss` & `django-formset-1.0.dev3/formset/static/formset/scss/collections.scss`

 * *Files identical despite different names*

### Comparing `django-formset-1.0.dev2/formset/templates/calendar/hours.html` & `django-formset-1.0.dev3/formset/templates/calendar/hours.html`

 * *Files identical despite different names*

### Comparing `django-formset-1.0.dev2/formset/templates/calendar/months.html` & `django-formset-1.0.dev3/formset/templates/calendar/months.html`

 * *Files identical despite different names*

### Comparing `django-formset-1.0.dev2/formset/templates/calendar/weeks.html` & `django-formset-1.0.dev3/formset/templates/calendar/weeks.html`

 * *Files identical despite different names*

### Comparing `django-formset-1.0.dev2/formset/templates/calendar/years.html` & `django-formset-1.0.dev3/formset/templates/calendar/years.html`

 * *Files identical despite different names*

### Comparing `django-formset-1.0.dev2/formset/templates/formset/bootstrap/widgets/dual_selector.html` & `django-formset-1.0.dev3/formset/templates/formset/bootstrap/widgets/dual_selector.html`

 * *Files identical despite different names*

### Comparing `django-formset-1.0.dev2/formset/templates/formset/bootstrap/widgets/file.html` & `django-formset-1.0.dev3/formset/templates/formset/bootstrap/widgets/file.html`

 * *Files identical despite different names*

### Comparing `django-formset-1.0.dev2/formset/templates/formset/bulma/widgets/dual_selector.html` & `django-formset-1.0.dev3/formset/templates/formset/bulma/widgets/dual_selector.html`

 * *Files identical despite different names*

### Comparing `django-formset-1.0.dev2/formset/templates/formset/bulma/widgets/file.html` & `django-formset-1.0.dev3/formset/templates/formset/bulma/widgets/file.html`

 * *Files identical despite different names*

### Comparing `django-formset-1.0.dev2/formset/templates/formset/default/buttons/richtext_align.html` & `django-formset-1.0.dev3/formset/templates/formset/default/buttons/richtext_align.html`

 * *Files identical despite different names*

### Comparing `django-formset-1.0.dev2/formset/templates/formset/default/buttons/richtext_color.html` & `django-formset-1.0.dev3/formset/templates/formset/default/buttons/richtext_color.html`

 * *Files identical despite different names*

### Comparing `django-formset-1.0.dev2/formset/templates/formset/default/buttons/richtext_heading.html` & `django-formset-1.0.dev3/formset/templates/formset/default/buttons/richtext_heading.html`

 * *Files identical despite different names*

### Comparing `django-formset-1.0.dev2/formset/templates/formset/default/collection.html` & `django-formset-1.0.dev3/formset/templates/formset/default/collection.html`

 * *Files identical despite different names*

### Comparing `django-formset-1.0.dev2/formset/templates/formset/default/dialog_form.html` & `django-formset-1.0.dev3/formset/templates/formset/default/dialog_form.html`

 * *Files identical despite different names*

### Comparing `django-formset-1.0.dev2/formset/templates/formset/default/fieldset.html` & `django-formset-1.0.dev3/formset/templates/formset/default/fieldset.html`

 * *Files identical despite different names*

### Comparing `django-formset-1.0.dev2/formset/templates/formset/default/widgets/dual_selector.html` & `django-formset-1.0.dev3/formset/templates/formset/default/widgets/dual_selector.html`

 * *Files identical despite different names*

### Comparing `django-formset-1.0.dev2/formset/templates/formset/default/widgets/file.html` & `django-formset-1.0.dev3/formset/templates/formset/default/widgets/file.html`

 * *Files identical despite different names*

### Comparing `django-formset-1.0.dev2/formset/templates/formset/default/widgets/selectize.html` & `django-formset-1.0.dev3/formset/templates/formset/default/widgets/selectize.html`

 * *Files identical despite different names*

### Comparing `django-formset-1.0.dev2/formset/templates/formset/foundation/widgets/dual_selector.html` & `django-formset-1.0.dev3/formset/templates/formset/foundation/widgets/dual_selector.html`

 * *Files identical despite different names*

### Comparing `django-formset-1.0.dev2/formset/templates/formset/foundation/widgets/file.html` & `django-formset-1.0.dev3/formset/templates/formset/foundation/widgets/file.html`

 * *Files identical despite different names*

### Comparing `django-formset-1.0.dev2/formset/templates/formset/icons/blockquote.svg` & `django-formset-1.0.dev3/formset/templates/formset/icons/blockquote.svg`

 * *Files identical despite different names*

### Comparing `django-formset-1.0.dev2/formset/templates/formset/icons/letters.svg` & `django-formset-1.0.dev3/formset/templates/formset/icons/letters.svg`

 * *Files identical despite different names*

### Comparing `django-formset-1.0.dev2/formset/templates/formset/icons/placeholder.svg` & `django-formset-1.0.dev3/formset/templates/formset/icons/placeholder.svg`

 * *Files identical despite different names*

### Comparing `django-formset-1.0.dev2/formset/templates/formset/icons/questionmark.svg` & `django-formset-1.0.dev3/formset/templates/formset/icons/questionmark.svg`

 * *Files identical despite different names*

### Comparing `django-formset-1.0.dev2/formset/templates/formset/icons/subscript.svg` & `django-formset-1.0.dev3/formset/templates/formset/icons/subscript.svg`

 * *Files identical despite different names*

### Comparing `django-formset-1.0.dev2/formset/templates/formset/icons/unlink.svg` & `django-formset-1.0.dev3/formset/templates/formset/icons/unlink.svg`

 * *Files identical despite different names*

### Comparing `django-formset-1.0.dev2/formset/templates/formset/tailwind/widgets/dual_selector.html` & `django-formset-1.0.dev3/formset/templates/formset/tailwind/widgets/dual_selector.html`

 * *Files identical despite different names*

### Comparing `django-formset-1.0.dev2/formset/templates/formset/tailwind/widgets/file.html` & `django-formset-1.0.dev3/formset/templates/formset/tailwind/widgets/file.html`

 * *Files identical despite different names*

### Comparing `django-formset-1.0.dev2/formset/templates/formset/uikit/widgets/file.html` & `django-formset-1.0.dev3/formset/templates/formset/uikit/widgets/file.html`

 * *Files identical despite different names*

### Comparing `django-formset-1.0.dev2/formset/templatetags/formsetify.py` & `django-formset-1.0.dev3/formset/templatetags/formsetify.py`

 * *Files identical despite different names*

### Comparing `django-formset-1.0.dev2/formset/upload.py` & `django-formset-1.0.dev3/formset/upload.py`

 * *Files identical despite different names*

### Comparing `django-formset-1.0.dev2/formset/utils.py` & `django-formset-1.0.dev3/formset/utils.py`

 * *Files identical despite different names*

### Comparing `django-formset-1.0.dev2/formset/views.py` & `django-formset-1.0.dev3/formset/views.py`

 * *Files identical despite different names*

### Comparing `django-formset-1.0.dev2/formset/widgets.py` & `django-formset-1.0.dev3/formset/widgets.py`

 * *Files identical despite different names*

### Comparing `django-formset-1.0.dev2/setup.py` & `django-formset-1.0.dev3/setup.py`

 * *Files identical despite different names*

