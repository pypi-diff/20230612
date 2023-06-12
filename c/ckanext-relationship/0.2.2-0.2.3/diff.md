# Comparing `tmp/ckanext-relationship-0.2.2.tar.gz` & `tmp/ckanext-relationship-0.2.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ckanext-relationship-0.2.2.tar", last modified: Sat Jun 10 18:46:39 2023, max compression
+gzip compressed data, was "ckanext-relationship-0.2.3.tar", last modified: Mon Jun 12 15:38:35 2023, max compression
```

## Comparing `ckanext-relationship-0.2.2.tar` & `ckanext-relationship-0.2.3.tar`

### file list

```diff
@@ -1,60 +1,60 @@
-drwxrwxr-x   0 aleks     (1000) aleks     (1000)        0 2023-06-10 18:46:39.149577 ckanext-relationship-0.2.2/
--rw-rw-r--   0 aleks     (1000) aleks     (1000)    34500 2023-03-05 23:40:30.000000 ckanext-relationship-0.2.2/LICENSE
--rw-rw-r--   0 aleks     (1000) aleks     (1000)      216 2023-03-05 23:40:30.000000 ckanext-relationship-0.2.2/MANIFEST.in
--rw-rw-r--   0 aleks     (1000) aleks     (1000)     4884 2023-06-10 18:46:39.149577 ckanext-relationship-0.2.2/PKG-INFO
--rw-rw-r--   0 aleks     (1000) aleks     (1000)     4414 2023-06-10 09:09:04.000000 ckanext-relationship-0.2.2/README.md
-drwxrwxr-x   0 aleks     (1000) aleks     (1000)        0 2023-06-10 18:46:39.145577 ckanext-relationship-0.2.2/ckanext/
--rw-rw-r--   0 aleks     (1000) aleks     (1000)      221 2023-06-10 09:09:04.000000 ckanext-relationship-0.2.2/ckanext/__init__.py
-drwxrwxr-x   0 aleks     (1000) aleks     (1000)        0 2023-06-10 18:46:39.145577 ckanext-relationship-0.2.2/ckanext/relationship/
--rw-rw-r--   0 aleks     (1000) aleks     (1000)        0 2023-03-05 23:40:30.000000 ckanext-relationship-0.2.2/ckanext/relationship/__init__.py
-drwxrwxr-x   0 aleks     (1000) aleks     (1000)        0 2023-06-10 18:46:39.145577 ckanext-relationship-0.2.2/ckanext/relationship/assets/
-drwxrwxr-x   0 aleks     (1000) aleks     (1000)        0 2023-06-10 18:46:39.145577 ckanext-relationship-0.2.2/ckanext/relationship/assets/js/
--rw-rw-r--   0 aleks     (1000) aleks     (1000)    10889 2023-06-10 18:34:43.000000 ckanext-relationship-0.2.2/ckanext/relationship/assets/js/relationship-autocomplete.js
--rw-rw-r--   0 aleks     (1000) aleks     (1000)      340 2023-06-10 09:09:10.000000 ckanext-relationship-0.2.2/ckanext/relationship/assets/webassets.yml
--rw-rw-r--   0 aleks     (1000) aleks     (1000)     2535 2023-06-10 09:11:53.000000 ckanext-relationship-0.2.2/ckanext/relationship/helpers.py
-drwxrwxr-x   0 aleks     (1000) aleks     (1000)        0 2023-06-10 18:46:39.145577 ckanext-relationship-0.2.2/ckanext/relationship/logic/
--rw-rw-r--   0 aleks     (1000) aleks     (1000)        0 2023-03-05 23:40:30.000000 ckanext-relationship-0.2.2/ckanext/relationship/logic/__init__.py
--rw-rw-r--   0 aleks     (1000) aleks     (1000)     5522 2023-06-10 09:09:04.000000 ckanext-relationship-0.2.2/ckanext/relationship/logic/action.py
--rw-rw-r--   0 aleks     (1000) aleks     (1000)      598 2023-06-10 09:09:04.000000 ckanext-relationship-0.2.2/ckanext/relationship/logic/auth.py
--rw-rw-r--   0 aleks     (1000) aleks     (1000)     1885 2023-06-10 09:09:04.000000 ckanext-relationship-0.2.2/ckanext/relationship/logic/schema.py
--rw-rw-r--   0 aleks     (1000) aleks     (1000)     2702 2023-06-10 18:38:05.000000 ckanext-relationship-0.2.2/ckanext/relationship/logic/validators.py
-drwxrwxr-x   0 aleks     (1000) aleks     (1000)        0 2023-06-10 18:46:39.145577 ckanext-relationship-0.2.2/ckanext/relationship/migration/
-drwxrwxr-x   0 aleks     (1000) aleks     (1000)        0 2023-06-10 18:46:39.145577 ckanext-relationship-0.2.2/ckanext/relationship/migration/relationship/
--rw-rw-r--   0 aleks     (1000) aleks     (1000)     1820 2023-03-05 23:40:30.000000 ckanext-relationship-0.2.2/ckanext/relationship/migration/relationship/alembic.ini
--rw-rw-r--   0 aleks     (1000) aleks     (1000)     2228 2023-06-10 09:09:04.000000 ckanext-relationship-0.2.2/ckanext/relationship/migration/relationship/env.py
--rw-rw-r--   0 aleks     (1000) aleks     (1000)      494 2023-03-05 23:40:30.000000 ckanext-relationship-0.2.2/ckanext/relationship/migration/relationship/script.py.mako
-drwxrwxr-x   0 aleks     (1000) aleks     (1000)        0 2023-06-10 18:46:39.145577 ckanext-relationship-0.2.2/ckanext/relationship/migration/relationship/versions/
--rw-rw-r--   0 aleks     (1000) aleks     (1000)      660 2023-06-10 09:09:04.000000 ckanext-relationship-0.2.2/ckanext/relationship/migration/relationship/versions/520e6ea9f57c_create_relationship_table.py
-drwxrwxr-x   0 aleks     (1000) aleks     (1000)        0 2023-06-10 18:46:39.145577 ckanext-relationship-0.2.2/ckanext/relationship/model/
--rw-rw-r--   0 aleks     (1000) aleks     (1000)        0 2023-03-05 23:40:30.000000 ckanext-relationship-0.2.2/ckanext/relationship/model/__init__.py
--rw-rw-r--   0 aleks     (1000) aleks     (1000)       83 2023-03-05 23:40:30.000000 ckanext-relationship-0.2.2/ckanext/relationship/model/base.py
--rw-rw-r--   0 aleks     (1000) aleks     (1000)     3064 2023-06-10 09:09:04.000000 ckanext-relationship-0.2.2/ckanext/relationship/model/relationship.py
--rw-rw-r--   0 aleks     (1000) aleks     (1000)     4769 2023-06-10 09:11:35.000000 ckanext-relationship-0.2.2/ckanext/relationship/plugin.py
--rw-rw-r--   0 aleks     (1000) aleks     (1000)      323 2023-03-05 23:40:30.000000 ckanext-relationship-0.2.2/ckanext/relationship/presets.yaml
-drwxrwxr-x   0 aleks     (1000) aleks     (1000)        0 2023-06-10 18:46:39.145577 ckanext-relationship-0.2.2/ckanext/relationship/templates/
--rw-rw-r--   0 aleks     (1000) aleks     (1000)      126 2023-06-10 09:09:10.000000 ckanext-relationship-0.2.2/ckanext/relationship/templates/page.html
-drwxrwxr-x   0 aleks     (1000) aleks     (1000)        0 2023-06-10 18:46:39.145577 ckanext-relationship-0.2.2/ckanext/relationship/templates/relationship/
-drwxrwxr-x   0 aleks     (1000) aleks     (1000)        0 2023-06-10 18:46:39.149577 ckanext-relationship-0.2.2/ckanext/relationship/templates/relationship/snippets/
--rw-rw-r--   0 aleks     (1000) aleks     (1000)       43 2023-06-10 09:09:10.000000 ckanext-relationship-0.2.2/ckanext/relationship/templates/relationship/snippets/asset.html
-drwxrwxr-x   0 aleks     (1000) aleks     (1000)        0 2023-06-10 18:46:39.145577 ckanext-relationship-0.2.2/ckanext/relationship/templates/scheming/
-drwxrwxr-x   0 aleks     (1000) aleks     (1000)        0 2023-06-10 18:46:39.149577 ckanext-relationship-0.2.2/ckanext/relationship/templates/scheming/display_snippets/
--rw-rw-r--   0 aleks     (1000) aleks     (1000)      658 2023-03-05 23:40:30.000000 ckanext-relationship-0.2.2/ckanext/relationship/templates/scheming/display_snippets/related_entity.html
-drwxrwxr-x   0 aleks     (1000) aleks     (1000)        0 2023-06-10 18:46:39.149577 ckanext-relationship-0.2.2/ckanext/relationship/templates/scheming/form_snippets/
--rw-rw-r--   0 aleks     (1000) aleks     (1000)     2036 2023-06-10 11:22:47.000000 ckanext-relationship-0.2.2/ckanext/relationship/templates/scheming/form_snippets/related_entity.html
--rw-rw-r--   0 aleks     (1000) aleks     (1000)     1150 2023-06-10 09:49:04.000000 ckanext-relationship-0.2.2/ckanext/relationship/templates/scheming/form_snippets/related_entity_with_autocomplete.html
-drwxrwxr-x   0 aleks     (1000) aleks     (1000)        0 2023-06-10 18:46:39.149577 ckanext-relationship-0.2.2/ckanext/relationship/tests/
--rw-rw-r--   0 aleks     (1000) aleks     (1000)        0 2023-03-05 23:40:30.000000 ckanext-relationship-0.2.2/ckanext/relationship/tests/__init__.py
--rw-rw-r--   0 aleks     (1000) aleks     (1000)     1218 2023-06-10 09:09:04.000000 ckanext-relationship-0.2.2/ckanext/relationship/tests/test_plugin.py
--rw-rw-r--   0 aleks     (1000) aleks     (1000)     2213 2023-06-10 09:09:04.000000 ckanext-relationship-0.2.2/ckanext/relationship/utils.py
--rw-rw-r--   0 aleks     (1000) aleks     (1000)     1316 2023-06-10 18:38:05.000000 ckanext-relationship-0.2.2/ckanext/relationship/views.py
-drwxrwxr-x   0 aleks     (1000) aleks     (1000)        0 2023-06-10 18:46:39.149577 ckanext-relationship-0.2.2/ckanext_relationship.egg-info/
--rw-rw-r--   0 aleks     (1000) aleks     (1000)     4884 2023-06-10 18:46:39.000000 ckanext-relationship-0.2.2/ckanext_relationship.egg-info/PKG-INFO
--rw-rw-r--   0 aleks     (1000) aleks     (1000)     1664 2023-06-10 18:46:39.000000 ckanext-relationship-0.2.2/ckanext_relationship.egg-info/SOURCES.txt
--rw-rw-r--   0 aleks     (1000) aleks     (1000)        1 2023-06-10 18:46:39.000000 ckanext-relationship-0.2.2/ckanext_relationship.egg-info/dependency_links.txt
--rw-rw-r--   0 aleks     (1000) aleks     (1000)      134 2023-06-10 18:46:39.000000 ckanext-relationship-0.2.2/ckanext_relationship.egg-info/entry_points.txt
--rw-rw-r--   0 aleks     (1000) aleks     (1000)        8 2023-06-10 18:46:39.000000 ckanext-relationship-0.2.2/ckanext_relationship.egg-info/namespace_packages.txt
--rw-rw-r--   0 aleks     (1000) aleks     (1000)        8 2023-06-10 18:46:39.000000 ckanext-relationship-0.2.2/ckanext_relationship.egg-info/top_level.txt
--rw-rw-r--   0 aleks     (1000) aleks     (1000)     2979 2023-06-10 09:09:04.000000 ckanext-relationship-0.2.2/pyproject.toml
--rw-rw-r--   0 aleks     (1000) aleks     (1000)       23 2023-03-05 23:40:30.000000 ckanext-relationship-0.2.2/requirements.txt
--rw-rw-r--   0 aleks     (1000) aleks     (1000)      613 2023-06-10 18:46:39.149577 ckanext-relationship-0.2.2/setup.cfg
--rw-rw-r--   0 aleks     (1000) aleks     (1000)     3727 2023-06-10 18:38:51.000000 ckanext-relationship-0.2.2/setup.py
+drwxrwxr-x   0 aleks     (1000) aleks     (1000)        0 2023-06-12 15:38:35.371760 ckanext-relationship-0.2.3/
+-rw-rw-r--   0 aleks     (1000) aleks     (1000)    34500 2023-03-05 23:40:30.000000 ckanext-relationship-0.2.3/LICENSE
+-rw-rw-r--   0 aleks     (1000) aleks     (1000)      216 2023-03-05 23:40:30.000000 ckanext-relationship-0.2.3/MANIFEST.in
+-rw-rw-r--   0 aleks     (1000) aleks     (1000)     4884 2023-06-12 15:38:35.375760 ckanext-relationship-0.2.3/PKG-INFO
+-rw-rw-r--   0 aleks     (1000) aleks     (1000)     4414 2023-06-10 09:09:04.000000 ckanext-relationship-0.2.3/README.md
+drwxrwxr-x   0 aleks     (1000) aleks     (1000)        0 2023-06-12 15:38:35.371760 ckanext-relationship-0.2.3/ckanext/
+-rw-rw-r--   0 aleks     (1000) aleks     (1000)      221 2023-06-10 09:09:04.000000 ckanext-relationship-0.2.3/ckanext/__init__.py
+drwxrwxr-x   0 aleks     (1000) aleks     (1000)        0 2023-06-12 15:38:35.371760 ckanext-relationship-0.2.3/ckanext/relationship/
+-rw-rw-r--   0 aleks     (1000) aleks     (1000)        0 2023-03-05 23:40:30.000000 ckanext-relationship-0.2.3/ckanext/relationship/__init__.py
+drwxrwxr-x   0 aleks     (1000) aleks     (1000)        0 2023-06-12 15:38:35.371760 ckanext-relationship-0.2.3/ckanext/relationship/assets/
+drwxrwxr-x   0 aleks     (1000) aleks     (1000)        0 2023-06-12 15:38:35.371760 ckanext-relationship-0.2.3/ckanext/relationship/assets/js/
+-rw-rw-r--   0 aleks     (1000) aleks     (1000)    10889 2023-06-10 18:34:43.000000 ckanext-relationship-0.2.3/ckanext/relationship/assets/js/relationship-autocomplete.js
+-rw-rw-r--   0 aleks     (1000) aleks     (1000)      340 2023-06-10 09:09:10.000000 ckanext-relationship-0.2.3/ckanext/relationship/assets/webassets.yml
+-rw-rw-r--   0 aleks     (1000) aleks     (1000)     3484 2023-06-12 15:32:03.000000 ckanext-relationship-0.2.3/ckanext/relationship/helpers.py
+drwxrwxr-x   0 aleks     (1000) aleks     (1000)        0 2023-06-12 15:38:35.371760 ckanext-relationship-0.2.3/ckanext/relationship/logic/
+-rw-rw-r--   0 aleks     (1000) aleks     (1000)        0 2023-03-05 23:40:30.000000 ckanext-relationship-0.2.3/ckanext/relationship/logic/__init__.py
+-rw-rw-r--   0 aleks     (1000) aleks     (1000)     5522 2023-06-10 09:09:04.000000 ckanext-relationship-0.2.3/ckanext/relationship/logic/action.py
+-rw-rw-r--   0 aleks     (1000) aleks     (1000)      598 2023-06-10 09:09:04.000000 ckanext-relationship-0.2.3/ckanext/relationship/logic/auth.py
+-rw-rw-r--   0 aleks     (1000) aleks     (1000)     1885 2023-06-10 09:09:04.000000 ckanext-relationship-0.2.3/ckanext/relationship/logic/schema.py
+-rw-rw-r--   0 aleks     (1000) aleks     (1000)     2702 2023-06-12 15:32:05.000000 ckanext-relationship-0.2.3/ckanext/relationship/logic/validators.py
+drwxrwxr-x   0 aleks     (1000) aleks     (1000)        0 2023-06-12 15:38:35.371760 ckanext-relationship-0.2.3/ckanext/relationship/migration/
+drwxrwxr-x   0 aleks     (1000) aleks     (1000)        0 2023-06-12 15:38:35.371760 ckanext-relationship-0.2.3/ckanext/relationship/migration/relationship/
+-rw-rw-r--   0 aleks     (1000) aleks     (1000)     1820 2023-03-05 23:40:30.000000 ckanext-relationship-0.2.3/ckanext/relationship/migration/relationship/alembic.ini
+-rw-rw-r--   0 aleks     (1000) aleks     (1000)     2228 2023-06-10 09:09:04.000000 ckanext-relationship-0.2.3/ckanext/relationship/migration/relationship/env.py
+-rw-rw-r--   0 aleks     (1000) aleks     (1000)      494 2023-03-05 23:40:30.000000 ckanext-relationship-0.2.3/ckanext/relationship/migration/relationship/script.py.mako
+drwxrwxr-x   0 aleks     (1000) aleks     (1000)        0 2023-06-12 15:38:35.371760 ckanext-relationship-0.2.3/ckanext/relationship/migration/relationship/versions/
+-rw-rw-r--   0 aleks     (1000) aleks     (1000)      660 2023-06-10 09:09:04.000000 ckanext-relationship-0.2.3/ckanext/relationship/migration/relationship/versions/520e6ea9f57c_create_relationship_table.py
+drwxrwxr-x   0 aleks     (1000) aleks     (1000)        0 2023-06-12 15:38:35.371760 ckanext-relationship-0.2.3/ckanext/relationship/model/
+-rw-rw-r--   0 aleks     (1000) aleks     (1000)        0 2023-03-05 23:40:30.000000 ckanext-relationship-0.2.3/ckanext/relationship/model/__init__.py
+-rw-rw-r--   0 aleks     (1000) aleks     (1000)       83 2023-03-05 23:40:30.000000 ckanext-relationship-0.2.3/ckanext/relationship/model/base.py
+-rw-rw-r--   0 aleks     (1000) aleks     (1000)     3064 2023-06-10 09:09:04.000000 ckanext-relationship-0.2.3/ckanext/relationship/model/relationship.py
+-rw-rw-r--   0 aleks     (1000) aleks     (1000)     4769 2023-06-10 09:11:35.000000 ckanext-relationship-0.2.3/ckanext/relationship/plugin.py
+-rw-rw-r--   0 aleks     (1000) aleks     (1000)      323 2023-03-05 23:40:30.000000 ckanext-relationship-0.2.3/ckanext/relationship/presets.yaml
+drwxrwxr-x   0 aleks     (1000) aleks     (1000)        0 2023-06-12 15:38:35.371760 ckanext-relationship-0.2.3/ckanext/relationship/templates/
+-rw-rw-r--   0 aleks     (1000) aleks     (1000)      126 2023-06-10 09:09:10.000000 ckanext-relationship-0.2.3/ckanext/relationship/templates/page.html
+drwxrwxr-x   0 aleks     (1000) aleks     (1000)        0 2023-06-12 15:38:35.371760 ckanext-relationship-0.2.3/ckanext/relationship/templates/relationship/
+drwxrwxr-x   0 aleks     (1000) aleks     (1000)        0 2023-06-12 15:38:35.371760 ckanext-relationship-0.2.3/ckanext/relationship/templates/relationship/snippets/
+-rw-rw-r--   0 aleks     (1000) aleks     (1000)       43 2023-06-10 09:09:10.000000 ckanext-relationship-0.2.3/ckanext/relationship/templates/relationship/snippets/asset.html
+drwxrwxr-x   0 aleks     (1000) aleks     (1000)        0 2023-06-12 15:38:35.371760 ckanext-relationship-0.2.3/ckanext/relationship/templates/scheming/
+drwxrwxr-x   0 aleks     (1000) aleks     (1000)        0 2023-06-12 15:38:35.371760 ckanext-relationship-0.2.3/ckanext/relationship/templates/scheming/display_snippets/
+-rw-rw-r--   0 aleks     (1000) aleks     (1000)      658 2023-03-05 23:40:30.000000 ckanext-relationship-0.2.3/ckanext/relationship/templates/scheming/display_snippets/related_entity.html
+drwxrwxr-x   0 aleks     (1000) aleks     (1000)        0 2023-06-12 15:38:35.371760 ckanext-relationship-0.2.3/ckanext/relationship/templates/scheming/form_snippets/
+-rw-rw-r--   0 aleks     (1000) aleks     (1000)     1570 2023-06-12 14:38:30.000000 ckanext-relationship-0.2.3/ckanext/relationship/templates/scheming/form_snippets/related_entity.html
+-rw-rw-r--   0 aleks     (1000) aleks     (1000)     1253 2023-06-12 15:10:19.000000 ckanext-relationship-0.2.3/ckanext/relationship/templates/scheming/form_snippets/related_entity_with_autocomplete.html
+drwxrwxr-x   0 aleks     (1000) aleks     (1000)        0 2023-06-12 15:38:35.371760 ckanext-relationship-0.2.3/ckanext/relationship/tests/
+-rw-rw-r--   0 aleks     (1000) aleks     (1000)        0 2023-03-05 23:40:30.000000 ckanext-relationship-0.2.3/ckanext/relationship/tests/__init__.py
+-rw-rw-r--   0 aleks     (1000) aleks     (1000)     1218 2023-06-10 09:09:04.000000 ckanext-relationship-0.2.3/ckanext/relationship/tests/test_plugin.py
+-rw-rw-r--   0 aleks     (1000) aleks     (1000)     2213 2023-06-10 09:09:04.000000 ckanext-relationship-0.2.3/ckanext/relationship/utils.py
+-rw-rw-r--   0 aleks     (1000) aleks     (1000)     1633 2023-06-12 15:32:03.000000 ckanext-relationship-0.2.3/ckanext/relationship/views.py
+drwxrwxr-x   0 aleks     (1000) aleks     (1000)        0 2023-06-12 15:38:35.371760 ckanext-relationship-0.2.3/ckanext_relationship.egg-info/
+-rw-rw-r--   0 aleks     (1000) aleks     (1000)     4884 2023-06-12 15:38:35.000000 ckanext-relationship-0.2.3/ckanext_relationship.egg-info/PKG-INFO
+-rw-rw-r--   0 aleks     (1000) aleks     (1000)     1664 2023-06-12 15:38:35.000000 ckanext-relationship-0.2.3/ckanext_relationship.egg-info/SOURCES.txt
+-rw-rw-r--   0 aleks     (1000) aleks     (1000)        1 2023-06-12 15:38:35.000000 ckanext-relationship-0.2.3/ckanext_relationship.egg-info/dependency_links.txt
+-rw-rw-r--   0 aleks     (1000) aleks     (1000)      134 2023-06-12 15:38:35.000000 ckanext-relationship-0.2.3/ckanext_relationship.egg-info/entry_points.txt
+-rw-rw-r--   0 aleks     (1000) aleks     (1000)        8 2023-06-12 15:38:35.000000 ckanext-relationship-0.2.3/ckanext_relationship.egg-info/namespace_packages.txt
+-rw-rw-r--   0 aleks     (1000) aleks     (1000)        8 2023-06-12 15:38:35.000000 ckanext-relationship-0.2.3/ckanext_relationship.egg-info/top_level.txt
+-rw-rw-r--   0 aleks     (1000) aleks     (1000)     2979 2023-06-10 09:09:04.000000 ckanext-relationship-0.2.3/pyproject.toml
+-rw-rw-r--   0 aleks     (1000) aleks     (1000)       23 2023-03-05 23:40:30.000000 ckanext-relationship-0.2.3/requirements.txt
+-rw-rw-r--   0 aleks     (1000) aleks     (1000)      613 2023-06-12 15:38:35.375760 ckanext-relationship-0.2.3/setup.cfg
+-rw-rw-r--   0 aleks     (1000) aleks     (1000)     3727 2023-06-12 15:36:32.000000 ckanext-relationship-0.2.3/setup.py
```

### Comparing `ckanext-relationship-0.2.2/LICENSE` & `ckanext-relationship-0.2.3/LICENSE`

 * *Files identical despite different names*

### Comparing `ckanext-relationship-0.2.2/PKG-INFO` & `ckanext-relationship-0.2.3/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ckanext-relationship
-Version: 0.2.2
+Version: 0.2.3
 Home-page: https://github.com/DataShades/ckanext-relationship
 Author: Oleksandr Ivaniuk
 Author-email: aleks.ivaniuk@gmail.com
 License: AGPL
 Keywords: CKAN
 Classifier: Development Status :: 4 - Beta
 Classifier: License :: OSI Approved :: GNU Affero General Public License v3 or later (AGPLv3+)
```

### Comparing `ckanext-relationship-0.2.2/README.md` & `ckanext-relationship-0.2.3/README.md`

 * *Files identical despite different names*

### Comparing `ckanext-relationship-0.2.2/ckanext/relationship/assets/js/relationship-autocomplete.js` & `ckanext-relationship-0.2.3/ckanext/relationship/assets/js/relationship-autocomplete.js`

 * *Files identical despite different names*

### Comparing `ckanext-relationship-0.2.2/ckanext/relationship/helpers.py` & `ckanext-relationship-0.2.3/ckanext/relationship/helpers.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,23 +1,24 @@
 from __future__ import annotations
 
 import json
+from typing import Any
 
 import ckan.plugins.toolkit as tk
+from ckan import authz
 
 
 def relationship_get_entity_list(entity, entity_type, include_private=True):
     """Return ids list of specified entity (entity, entity_type)"""
     context = {}
     if entity == "package":
         entity_list = tk.get_action("package_search")(
             context,
             {
                 "fq": f"type:{entity_type}",
-                "fl": "id, name, title",
                 "rows": 1000,
                 "include_private": include_private,
             },
         )
         entity_list = entity_list["results"]
     else:
         entity_list = tk.get_action("relationship_get_entity_list")(
@@ -70,7 +71,39 @@
     for pkg_id in selected_ids:
         try:
             pkg_dict = tk.get_action("package_show")({}, {"id": pkg_id})
             selected_pkgs.append({"name": pkg_dict["id"], "title": pkg_dict["title"]})
         except Exception:
             continue
     return json.dumps(selected_pkgs)
+
+
+def relationship_get_choices_for_related_entity_field(
+    field: dict[str, Any], current_entity_id: str | None
+) -> list[str | None]:
+    entities = relationship_get_entity_list(
+        field["related_entity"], field["related_entity_type"]
+    )
+
+    choices = []
+
+    for entity in entities:
+        if entity["id"] == current_entity_id:
+            continue
+
+        if field.get("updatable_only", False) and not tk.h.check_access(
+            field["related_entity"] + "_update", {"id": entity["id"]}
+        ):
+            continue
+
+        if (
+            field.get("owned_only", False)
+            and not authz.is_sysadmin(tk.current_user.id)
+            and field["related_entity"] == "package"
+            and tk.current_user.id != entity["creator_user_id"]
+        ):
+            continue
+
+        choices.append((entity["id"], entity.get("title") or entity.get("name")))
+
+    choices.sort(key=lambda x: x[1])
+    return choices
```

### Comparing `ckanext-relationship-0.2.2/ckanext/relationship/logic/action.py` & `ckanext-relationship-0.2.3/ckanext/relationship/logic/action.py`

 * *Files identical despite different names*

### Comparing `ckanext-relationship-0.2.2/ckanext/relationship/logic/auth.py` & `ckanext-relationship-0.2.3/ckanext/relationship/logic/auth.py`

 * *Files identical despite different names*

### Comparing `ckanext-relationship-0.2.2/ckanext/relationship/logic/schema.py` & `ckanext-relationship-0.2.3/ckanext/relationship/logic/schema.py`

 * *Files identical despite different names*

### Comparing `ckanext-relationship-0.2.2/ckanext/relationship/logic/validators.py` & `ckanext-relationship-0.2.3/ckanext/relationship/logic/validators.py`

 * *Files identical despite different names*

### Comparing `ckanext-relationship-0.2.2/ckanext/relationship/migration/relationship/alembic.ini` & `ckanext-relationship-0.2.3/ckanext/relationship/migration/relationship/alembic.ini`

 * *Files identical despite different names*

### Comparing `ckanext-relationship-0.2.2/ckanext/relationship/migration/relationship/env.py` & `ckanext-relationship-0.2.3/ckanext/relationship/migration/relationship/env.py`

 * *Files identical despite different names*

### Comparing `ckanext-relationship-0.2.2/ckanext/relationship/migration/relationship/versions/520e6ea9f57c_create_relationship_table.py` & `ckanext-relationship-0.2.3/ckanext/relationship/migration/relationship/versions/520e6ea9f57c_create_relationship_table.py`

 * *Files identical despite different names*

### Comparing `ckanext-relationship-0.2.2/ckanext/relationship/model/relationship.py` & `ckanext-relationship-0.2.3/ckanext/relationship/model/relationship.py`

 * *Files identical despite different names*

### Comparing `ckanext-relationship-0.2.2/ckanext/relationship/plugin.py` & `ckanext-relationship-0.2.3/ckanext/relationship/plugin.py`

 * *Files identical despite different names*

### Comparing `ckanext-relationship-0.2.2/ckanext/relationship/templates/scheming/display_snippets/related_entity.html` & `ckanext-relationship-0.2.3/ckanext/relationship/templates/scheming/display_snippets/related_entity.html`

 * *Files identical despite different names*

### Comparing `ckanext-relationship-0.2.2/ckanext/relationship/templates/scheming/form_snippets/related_entity.html` & `ckanext-relationship-0.2.3/ckanext/relationship/templates/scheming/form_snippets/related_entity.html`

 * *Files 24% similar despite different names*

```diff
@@ -18,26 +18,15 @@
         label=h.scheming_language_text(field.label),
         classes=classes,
         error=errors[field.field_name],
         is_required=h.scheming_field_required(field),
         extra_html=help_text()
         ) %}
 
-  {% set current_entity_id = data.get('id', None) %}
-  {% set entities = h.relationship_get_entity_list(field.related_entity, field.related_entity_type) %}
-  {% set choices = [] %}
-
-  {% for entity in entities if entity.id != current_entity_id %}
-    {% if not field.get('updatable_only', false) or
-          h.check_access(field.related_entity ~ '_update', {'id': entity.id }) %}
-      {% do choices.append((entity.id, entity.get('title') or entity.get('name'))) %}
-    {% endif %}
-  {% endfor %}
-
-  {% set choices = choices|sort(case_sensitive=false, attribute=1) %}
+  {% set choices = h.relationship_get_choices_for_related_entity_field(field, data.get('id', None)) %}
 
   {% if not h.scheming_field_required(field) and not field.multiple %}
     {% do choices.insert(0, ('', 'No relation')) %}
   {% endif %}
 
   <select {% if field.multiple %}multiple{% endif %}
           size='{{ field.get('select_size', field.choices|length) }}'
```

### Comparing `ckanext-relationship-0.2.2/ckanext/relationship/templates/scheming/form_snippets/related_entity_with_autocomplete.html` & `ckanext-relationship-0.2.3/ckanext/relationship/templates/scheming/form_snippets/related_entity_with_autocomplete.html`

 * *Files 8% similar despite different names*

```diff
@@ -9,15 +9,15 @@
 
 {% set attrs = {
     "data-module": "relationship-autocomplete",
     "data-module-key": "name",
     "data-module-label": "title",
     "data-module-tags": "true",
     "data-module-createtags": "false",
-    "data-module-source": "/api/util/relationships/autocomplete?incomplete=?&entity_type=%s&updatable_only=%s"|format(field.related_entity_type, field.updatable_only),
+    "data-module-source": "/api/util/relationships/autocomplete?incomplete=?&current_entity_id=%s&entity_type=%s&updatable_only=%s&owned_only=%s"|format(data.get('id', None), field.related_entity_type, field.get('updatable_only', false), field.get('owned_only', false)),
     "data-module-selected": selected_json,
 } %}
 
 {% call form.input(
     field.field_name,
     id='field-' + field.field_name,
     label=h.scheming_language_text(field.label),
```

### Comparing `ckanext-relationship-0.2.2/ckanext/relationship/tests/test_plugin.py` & `ckanext-relationship-0.2.3/ckanext/relationship/tests/test_plugin.py`

 * *Files identical despite different names*

### Comparing `ckanext-relationship-0.2.2/ckanext/relationship/utils.py` & `ckanext-relationship-0.2.3/ckanext/relationship/utils.py`

 * *Files identical despite different names*

### Comparing `ckanext-relationship-0.2.2/ckanext_relationship.egg-info/PKG-INFO` & `ckanext-relationship-0.2.3/ckanext_relationship.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ckanext-relationship
-Version: 0.2.2
+Version: 0.2.3
 Home-page: https://github.com/DataShades/ckanext-relationship
 Author: Oleksandr Ivaniuk
 Author-email: aleks.ivaniuk@gmail.com
 License: AGPL
 Keywords: CKAN
 Classifier: Development Status :: 4 - Beta
 Classifier: License :: OSI Approved :: GNU Affero General Public License v3 or later (AGPLv3+)
```

### Comparing `ckanext-relationship-0.2.2/ckanext_relationship.egg-info/SOURCES.txt` & `ckanext-relationship-0.2.3/ckanext_relationship.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `ckanext-relationship-0.2.2/pyproject.toml` & `ckanext-relationship-0.2.3/pyproject.toml`

 * *Files identical despite different names*

### Comparing `ckanext-relationship-0.2.2/setup.cfg` & `ckanext-relationship-0.2.3/setup.cfg`

 * *Files identical despite different names*

### Comparing `ckanext-relationship-0.2.2/setup.py` & `ckanext-relationship-0.2.3/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -12,15 +12,15 @@
     long_description = f.read()
 
 setup(
     name="""ckanext-relationship""",
     # Versions should comply with PEP440.  For a discussion on single-sourcing
     # the version across setup.py and the project code, see
     # http://packaging.python.org/en/latest/tutorial.html#version
-    version="0.2.2",
+    version="0.2.3",
     description="""""",
     long_description=long_description,
     long_description_content_type="text/markdown",
     # The project's main homepage.
     url="https://github.com/DataShades/ckanext-relationship",
     # Author details
     author="""Oleksandr Ivaniuk""",
```

