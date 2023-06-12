# Comparing `tmp/aa-simplewiki-1.0.1.tar.gz` & `tmp/aa-simplewiki-1.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "aa-simplewiki-1.0.1.tar", last modified: Thu May 11 04:40:44 2023, max compression
+gzip compressed data, was "aa-simplewiki-1.0.2.tar", last modified: Mon Jun 12 04:03:55 2023, max compression
```

## Comparing `aa-simplewiki-1.0.1.tar` & `aa-simplewiki-1.0.2.tar`

### file list

```diff
@@ -1,78 +1,78 @@
-drwxrwxr-x   0 sonenn    (1000) sonenn    (1000)        0 2023-05-11 04:40:44.736061 aa-simplewiki-1.0.1/
--rw-rw-r--   0 sonenn    (1000) sonenn    (1000)    35164 2023-05-10 22:52:34.000000 aa-simplewiki-1.0.1/LICENSE
--rw-rw-r--   0 sonenn    (1000) sonenn    (1000)      123 2023-05-10 22:52:34.000000 aa-simplewiki-1.0.1/MANIFEST.in
--rw-rw-r--   0 sonenn    (1000) sonenn    (1000)     5719 2023-05-11 04:40:44.736061 aa-simplewiki-1.0.1/PKG-INFO
--rw-rw-r--   0 sonenn    (1000) sonenn    (1000)     4701 2023-05-10 22:52:34.000000 aa-simplewiki-1.0.1/README.md
-drwxrwxr-x   0 sonenn    (1000) sonenn    (1000)        0 2023-05-11 04:40:44.724061 aa-simplewiki-1.0.1/aa_simplewiki.egg-info/
--rw-rw-r--   0 sonenn    (1000) sonenn    (1000)     5719 2023-05-11 04:40:44.000000 aa-simplewiki-1.0.1/aa_simplewiki.egg-info/PKG-INFO
--rw-rw-r--   0 sonenn    (1000) sonenn    (1000)     2607 2023-05-11 04:40:44.000000 aa-simplewiki-1.0.1/aa_simplewiki.egg-info/SOURCES.txt
--rw-rw-r--   0 sonenn    (1000) sonenn    (1000)        1 2023-05-11 04:40:44.000000 aa-simplewiki-1.0.1/aa_simplewiki.egg-info/dependency_links.txt
--rw-rw-r--   0 sonenn    (1000) sonenn    (1000)        1 2023-05-11 04:40:44.000000 aa-simplewiki-1.0.1/aa_simplewiki.egg-info/not-zip-safe
--rw-rw-r--   0 sonenn    (1000) sonenn    (1000)       24 2023-05-11 04:40:44.000000 aa-simplewiki-1.0.1/aa_simplewiki.egg-info/requires.txt
--rw-rw-r--   0 sonenn    (1000) sonenn    (1000)       20 2023-05-11 04:40:44.000000 aa-simplewiki-1.0.1/aa_simplewiki.egg-info/top_level.txt
--rw-rw-r--   0 sonenn    (1000) sonenn    (1000)      104 2023-05-10 22:52:34.000000 aa-simplewiki-1.0.1/pyproject.toml
--rw-rw-r--   0 sonenn    (1000) sonenn    (1000)     1462 2023-05-11 04:40:44.740062 aa-simplewiki-1.0.1/setup.cfg
--rw-rw-r--   0 sonenn    (1000) sonenn    (1000)     1205 2023-05-11 04:38:56.000000 aa-simplewiki-1.0.1/setup.py
-drwxrwxr-x   0 sonenn    (1000) sonenn    (1000)        0 2023-05-11 04:40:44.728061 aa-simplewiki-1.0.1/simplewiki/
--rw-rw-r--   0 sonenn    (1000) sonenn    (1000)       48 2023-05-11 04:39:37.000000 aa-simplewiki-1.0.1/simplewiki/__init__.py
--rw-rw-r--   0 sonenn    (1000) sonenn    (1000)      231 2023-05-10 22:52:34.000000 aa-simplewiki-1.0.1/simplewiki/admin.py
--rw-rw-r--   0 sonenn    (1000) sonenn    (1000)    11877 2023-05-10 22:52:34.000000 aa-simplewiki-1.0.1/simplewiki/admin_helper_menus.py
--rw-rw-r--   0 sonenn    (1000) sonenn    (1000)     8956 2023-05-10 22:52:34.000000 aa-simplewiki-1.0.1/simplewiki/admin_helper_sections.py
--rw-rw-r--   0 sonenn    (1000) sonenn    (1000)      169 2023-05-10 22:52:34.000000 aa-simplewiki-1.0.1/simplewiki/app_settings.py
--rw-rw-r--   0 sonenn    (1000) sonenn    (1000)      284 2023-05-10 22:52:34.000000 aa-simplewiki-1.0.1/simplewiki/apps.py
--rw-rw-r--   0 sonenn    (1000) sonenn    (1000)     1076 2023-05-10 22:52:34.000000 aa-simplewiki-1.0.1/simplewiki/auth_hooks.py
-drwxrwxr-x   0 sonenn    (1000) sonenn    (1000)        0 2023-05-11 04:40:44.732061 aa-simplewiki-1.0.1/simplewiki/migrations/
--rw-rw-r--   0 sonenn    (1000) sonenn    (1000)     1489 2023-05-10 22:52:34.000000 aa-simplewiki-1.0.1/simplewiki/migrations/0001_initial.py
--rw-rw-r--   0 sonenn    (1000) sonenn    (1000)      395 2023-05-10 22:52:34.000000 aa-simplewiki-1.0.1/simplewiki/migrations/0002_pageitem_page_title.py
--rw-rw-r--   0 sonenn    (1000) sonenn    (1000)      401 2023-05-10 22:52:34.000000 aa-simplewiki-1.0.1/simplewiki/migrations/0003_menuitem_icon.py
--rw-rw-r--   0 sonenn    (1000) sonenn    (1000)     1532 2023-05-10 22:52:34.000000 aa-simplewiki-1.0.1/simplewiki/migrations/0004_pageitem_icon_alter_menuitem_icon_and_more.py
--rw-rw-r--   0 sonenn    (1000) sonenn    (1000)     1522 2023-05-10 22:52:34.000000 aa-simplewiki-1.0.1/simplewiki/migrations/0005_alter_menuitem_icon_alter_pageitem_content_and_more.py
--rw-rw-r--   0 sonenn    (1000) sonenn    (1000)      374 2023-05-10 22:52:34.000000 aa-simplewiki-1.0.1/simplewiki/migrations/0006_rename_pageitem_sectionitem.py
--rw-rw-r--   0 sonenn    (1000) sonenn    (1000)      392 2023-05-10 22:52:34.000000 aa-simplewiki-1.0.1/simplewiki/migrations/0007_rename_page_title_sectionitem_section_title.py
--rw-rw-r--   0 sonenn    (1000) sonenn    (1000)     1657 2023-05-10 22:52:34.000000 aa-simplewiki-1.0.1/simplewiki/migrations/0008_alter_general_options_alter_menuitem_icon_and_more.py
--rw-rw-r--   0 sonenn    (1000) sonenn    (1000)      658 2023-05-10 22:52:34.000000 aa-simplewiki-1.0.1/simplewiki/migrations/0009_remove_menuitem_name_menuitem_path.py
--rw-rw-r--   0 sonenn    (1000) sonenn    (1000)      381 2023-05-10 22:52:34.000000 aa-simplewiki-1.0.1/simplewiki/migrations/0010_rename_path_menuitem_name.py
--rw-rw-r--   0 sonenn    (1000) sonenn    (1000)      372 2023-05-10 22:52:34.000000 aa-simplewiki-1.0.1/simplewiki/migrations/0011_rename_name_menuitem_path.py
--rw-rw-r--   0 sonenn    (1000) sonenn    (1000)      576 2023-05-10 22:52:34.000000 aa-simplewiki-1.0.1/simplewiki/migrations/0012_menuitem_group.py
--rw-rw-r--   0 sonenn    (1000) sonenn    (1000)      579 2023-05-10 22:52:34.000000 aa-simplewiki-1.0.1/simplewiki/migrations/0013_alter_menuitem_group.py
--rw-rw-r--   0 sonenn    (1000) sonenn    (1000)     3030 2023-05-10 22:52:34.000000 aa-simplewiki-1.0.1/simplewiki/migrations/0014_alter_menuitem_group_alter_menuitem_icon_and_more.py
--rw-rw-r--   0 sonenn    (1000) sonenn    (1000)      685 2023-05-10 22:52:34.000000 aa-simplewiki-1.0.1/simplewiki/migrations/0015_rename_menu_name_sectionitem_menu_path_and_more.py
--rw-rw-r--   0 sonenn    (1000) sonenn    (1000)      407 2023-05-10 22:52:34.000000 aa-simplewiki-1.0.1/simplewiki/migrations/0016_rename_section_title_sectionitem_title.py
--rw-rw-r--   0 sonenn    (1000) sonenn    (1000)      831 2023-05-10 22:52:34.000000 aa-simplewiki-1.0.1/simplewiki/migrations/0017_alter_sectionitem_content_alter_sectionitem_title.py
--rw-rw-r--   0 sonenn    (1000) sonenn    (1000)      399 2023-05-10 22:52:34.000000 aa-simplewiki-1.0.1/simplewiki/migrations/0018_rename_group_menuitem_groups.py
--rw-rw-r--   0 sonenn    (1000) sonenn    (1000)      492 2023-05-10 22:52:34.000000 aa-simplewiki-1.0.1/simplewiki/migrations/0019_alter_general_options.py
--rw-rw-r--   0 sonenn    (1000) sonenn    (1000)      538 2023-05-10 22:52:34.000000 aa-simplewiki-1.0.1/simplewiki/migrations/0020_menuitem_parent.py
--rw-rw-r--   0 sonenn    (1000) sonenn    (1000)        0 2023-05-10 22:52:34.000000 aa-simplewiki-1.0.1/simplewiki/migrations/__init__.py
--rw-rw-r--   0 sonenn    (1000) sonenn    (1000)     4236 2023-05-10 22:52:34.000000 aa-simplewiki-1.0.1/simplewiki/models.py
-drwxrwxr-x   0 sonenn    (1000) sonenn    (1000)        0 2023-05-11 04:40:44.724061 aa-simplewiki-1.0.1/simplewiki/static/
-drwxrwxr-x   0 sonenn    (1000) sonenn    (1000)        0 2023-05-11 04:40:44.732061 aa-simplewiki-1.0.1/simplewiki/static/simplewiki/
--rw-rw-r--   0 sonenn    (1000) sonenn    (1000)        0 2023-05-10 22:52:34.000000 aa-simplewiki-1.0.1/simplewiki/static/simplewiki/.gitkeep
--rw-rw-r--   0 sonenn    (1000) sonenn    (1000)      199 2023-05-10 22:52:34.000000 aa-simplewiki-1.0.1/simplewiki/static/simplewiki/custom.css
--rw-rw-r--   0 sonenn    (1000) sonenn    (1000)      226 2023-05-10 22:52:34.000000 aa-simplewiki-1.0.1/simplewiki/tasks.py
-drwxrwxr-x   0 sonenn    (1000) sonenn    (1000)        0 2023-05-11 04:40:44.724061 aa-simplewiki-1.0.1/simplewiki/templates/
-drwxrwxr-x   0 sonenn    (1000) sonenn    (1000)        0 2023-05-11 04:40:44.732061 aa-simplewiki-1.0.1/simplewiki/templates/simplewiki/
--rw-rw-r--   0 sonenn    (1000) sonenn    (1000)     6324 2023-05-10 22:52:34.000000 aa-simplewiki-1.0.1/simplewiki/templates/simplewiki/base.html
--rw-rw-r--   0 sonenn    (1000) sonenn    (1000)     1076 2023-05-10 22:52:34.000000 aa-simplewiki-1.0.1/simplewiki/templates/simplewiki/dynamic_page.html
-drwxrwxr-x   0 sonenn    (1000) sonenn    (1000)        0 2023-05-11 04:40:44.736061 aa-simplewiki-1.0.1/simplewiki/templates/simplewiki/editor/
--rw-rw-r--   0 sonenn    (1000) sonenn    (1000)     6630 2023-05-11 04:36:11.000000 aa-simplewiki-1.0.1/simplewiki/templates/simplewiki/editor/editor_menus.html
--rw-rw-r--   0 sonenn    (1000) sonenn    (1000)     9500 2023-05-10 22:52:34.000000 aa-simplewiki-1.0.1/simplewiki/templates/simplewiki/editor/editor_sections.html
-drwxrwxr-x   0 sonenn    (1000) sonenn    (1000)        0 2023-05-11 04:40:44.736061 aa-simplewiki-1.0.1/simplewiki/templates/simplewiki/editor/partials/
--rw-rw-r--   0 sonenn    (1000) sonenn    (1000)     2320 2023-05-10 23:16:59.000000 aa-simplewiki-1.0.1/simplewiki/templates/simplewiki/editor/partials/_create_menu.html
--rw-rw-r--   0 sonenn    (1000) sonenn    (1000)     2468 2023-05-10 23:16:44.000000 aa-simplewiki-1.0.1/simplewiki/templates/simplewiki/editor/partials/_edit_menu.html
--rw-rw-r--   0 sonenn    (1000) sonenn    (1000)      593 2023-05-10 22:52:34.000000 aa-simplewiki-1.0.1/simplewiki/templates/simplewiki/error.html
--rw-rw-r--   0 sonenn    (1000) sonenn    (1000)      460 2023-05-10 22:52:34.000000 aa-simplewiki-1.0.1/simplewiki/templates/simplewiki/index.html
--rw-rw-r--   0 sonenn    (1000) sonenn    (1000)     1578 2023-05-10 22:52:34.000000 aa-simplewiki-1.0.1/simplewiki/templates/simplewiki/search.html
-drwxrwxr-x   0 sonenn    (1000) sonenn    (1000)        0 2023-05-11 04:40:44.736061 aa-simplewiki-1.0.1/simplewiki/templatetags/
--rw-rw-r--   0 sonenn    (1000) sonenn    (1000)     2121 2023-05-10 22:52:34.000000 aa-simplewiki-1.0.1/simplewiki/templatetags/custom_filters.py
--rw-rw-r--   0 sonenn    (1000) sonenn    (1000)      407 2023-05-10 22:52:34.000000 aa-simplewiki-1.0.1/simplewiki/templatetags/markdown_filters.py
-drwxrwxr-x   0 sonenn    (1000) sonenn    (1000)        0 2023-05-11 04:40:44.736061 aa-simplewiki-1.0.1/simplewiki/tests/
--rw-rw-r--   0 sonenn    (1000) sonenn    (1000)       27 2023-05-10 22:52:34.000000 aa-simplewiki-1.0.1/simplewiki/tests/__init__.py
--rw-rw-r--   0 sonenn    (1000) sonenn    (1000)      448 2023-05-10 22:52:34.000000 aa-simplewiki-1.0.1/simplewiki/tests/test_example.py
--rw-rw-r--   0 sonenn    (1000) sonenn    (1000)      488 2023-05-10 22:52:34.000000 aa-simplewiki-1.0.1/simplewiki/urls.py
--rw-rw-r--   0 sonenn    (1000) sonenn    (1000)    12689 2023-05-10 22:52:34.000000 aa-simplewiki-1.0.1/simplewiki/views.py
-drwxrwxr-x   0 sonenn    (1000) sonenn    (1000)        0 2023-05-11 04:40:44.736061 aa-simplewiki-1.0.1/testauth/
--rw-rw-r--   0 sonenn    (1000) sonenn    (1000)       52 2023-05-10 22:52:34.000000 aa-simplewiki-1.0.1/testauth/__init__.py
--rw-rw-r--   0 sonenn    (1000) sonenn    (1000)      654 2023-05-10 22:52:34.000000 aa-simplewiki-1.0.1/testauth/celery.py
--rw-rw-r--   0 sonenn    (1000) sonenn    (1000)     9481 2023-05-10 22:52:34.000000 aa-simplewiki-1.0.1/testauth/settings.py
--rw-rw-r--   0 sonenn    (1000) sonenn    (1000)      167 2023-05-10 22:52:34.000000 aa-simplewiki-1.0.1/testauth/urls.py
--rw-rw-r--   0 sonenn    (1000) sonenn    (1000)      425 2023-05-10 22:52:34.000000 aa-simplewiki-1.0.1/testauth/wsgi.py
+drwxrwxr-x   0 sonnen    (1000) sonnen    (1000)        0 2023-06-12 04:03:55.409730 aa-simplewiki-1.0.2/
+-rw-rw-r--   0 sonnen    (1000) sonnen    (1000)    35164 2023-06-12 03:22:47.000000 aa-simplewiki-1.0.2/LICENSE
+-rw-rw-r--   0 sonnen    (1000) sonnen    (1000)      123 2023-06-12 03:22:47.000000 aa-simplewiki-1.0.2/MANIFEST.in
+-rw-rw-r--   0 sonnen    (1000) sonnen    (1000)     5719 2023-06-12 04:03:55.409730 aa-simplewiki-1.0.2/PKG-INFO
+-rw-rw-r--   0 sonnen    (1000) sonnen    (1000)     4701 2023-06-12 03:22:47.000000 aa-simplewiki-1.0.2/README.md
+drwxrwxr-x   0 sonnen    (1000) sonnen    (1000)        0 2023-06-12 04:03:55.405730 aa-simplewiki-1.0.2/aa_simplewiki.egg-info/
+-rw-rw-r--   0 sonnen    (1000) sonnen    (1000)     5719 2023-06-12 04:03:55.000000 aa-simplewiki-1.0.2/aa_simplewiki.egg-info/PKG-INFO
+-rw-rw-r--   0 sonnen    (1000) sonnen    (1000)     2607 2023-06-12 04:03:55.000000 aa-simplewiki-1.0.2/aa_simplewiki.egg-info/SOURCES.txt
+-rw-rw-r--   0 sonnen    (1000) sonnen    (1000)        1 2023-06-12 04:03:55.000000 aa-simplewiki-1.0.2/aa_simplewiki.egg-info/dependency_links.txt
+-rw-rw-r--   0 sonnen    (1000) sonnen    (1000)        1 2023-06-12 03:50:34.000000 aa-simplewiki-1.0.2/aa_simplewiki.egg-info/not-zip-safe
+-rw-rw-r--   0 sonnen    (1000) sonnen    (1000)       24 2023-06-12 04:03:55.000000 aa-simplewiki-1.0.2/aa_simplewiki.egg-info/requires.txt
+-rw-rw-r--   0 sonnen    (1000) sonnen    (1000)       20 2023-06-12 04:03:55.000000 aa-simplewiki-1.0.2/aa_simplewiki.egg-info/top_level.txt
+-rw-rw-r--   0 sonnen    (1000) sonnen    (1000)      104 2023-06-12 03:22:47.000000 aa-simplewiki-1.0.2/pyproject.toml
+-rw-rw-r--   0 sonnen    (1000) sonnen    (1000)     1462 2023-06-12 04:03:55.413730 aa-simplewiki-1.0.2/setup.cfg
+-rw-rw-r--   0 sonnen    (1000) sonnen    (1000)     1205 2023-06-12 03:50:11.000000 aa-simplewiki-1.0.2/setup.py
+drwxrwxr-x   0 sonnen    (1000) sonnen    (1000)        0 2023-06-12 04:03:55.405730 aa-simplewiki-1.0.2/simplewiki/
+-rw-rw-r--   0 sonnen    (1000) sonnen    (1000)       47 2023-06-12 03:51:40.000000 aa-simplewiki-1.0.2/simplewiki/__init__.py
+-rw-rw-r--   0 sonnen    (1000) sonnen    (1000)      231 2023-06-12 03:22:47.000000 aa-simplewiki-1.0.2/simplewiki/admin.py
+-rw-rw-r--   0 sonnen    (1000) sonnen    (1000)    11916 2023-06-12 03:28:56.000000 aa-simplewiki-1.0.2/simplewiki/admin_helper_menus.py
+-rw-rw-r--   0 sonnen    (1000) sonnen    (1000)     8956 2023-06-12 03:22:47.000000 aa-simplewiki-1.0.2/simplewiki/admin_helper_sections.py
+-rw-rw-r--   0 sonnen    (1000) sonnen    (1000)      169 2023-06-12 03:22:47.000000 aa-simplewiki-1.0.2/simplewiki/app_settings.py
+-rw-rw-r--   0 sonnen    (1000) sonnen    (1000)      284 2023-06-12 03:22:47.000000 aa-simplewiki-1.0.2/simplewiki/apps.py
+-rw-rw-r--   0 sonnen    (1000) sonnen    (1000)     1076 2023-06-12 03:22:47.000000 aa-simplewiki-1.0.2/simplewiki/auth_hooks.py
+drwxrwxr-x   0 sonnen    (1000) sonnen    (1000)        0 2023-06-12 04:03:55.409730 aa-simplewiki-1.0.2/simplewiki/migrations/
+-rw-rw-r--   0 sonnen    (1000) sonnen    (1000)     1489 2023-06-12 03:22:47.000000 aa-simplewiki-1.0.2/simplewiki/migrations/0001_initial.py
+-rw-rw-r--   0 sonnen    (1000) sonnen    (1000)      395 2023-06-12 03:22:47.000000 aa-simplewiki-1.0.2/simplewiki/migrations/0002_pageitem_page_title.py
+-rw-rw-r--   0 sonnen    (1000) sonnen    (1000)      401 2023-06-12 03:22:47.000000 aa-simplewiki-1.0.2/simplewiki/migrations/0003_menuitem_icon.py
+-rw-rw-r--   0 sonnen    (1000) sonnen    (1000)     1532 2023-06-12 03:22:47.000000 aa-simplewiki-1.0.2/simplewiki/migrations/0004_pageitem_icon_alter_menuitem_icon_and_more.py
+-rw-rw-r--   0 sonnen    (1000) sonnen    (1000)     1522 2023-06-12 03:22:47.000000 aa-simplewiki-1.0.2/simplewiki/migrations/0005_alter_menuitem_icon_alter_pageitem_content_and_more.py
+-rw-rw-r--   0 sonnen    (1000) sonnen    (1000)      374 2023-06-12 03:22:47.000000 aa-simplewiki-1.0.2/simplewiki/migrations/0006_rename_pageitem_sectionitem.py
+-rw-rw-r--   0 sonnen    (1000) sonnen    (1000)      392 2023-06-12 03:22:47.000000 aa-simplewiki-1.0.2/simplewiki/migrations/0007_rename_page_title_sectionitem_section_title.py
+-rw-rw-r--   0 sonnen    (1000) sonnen    (1000)     1657 2023-06-12 03:22:47.000000 aa-simplewiki-1.0.2/simplewiki/migrations/0008_alter_general_options_alter_menuitem_icon_and_more.py
+-rw-rw-r--   0 sonnen    (1000) sonnen    (1000)      658 2023-06-12 03:22:47.000000 aa-simplewiki-1.0.2/simplewiki/migrations/0009_remove_menuitem_name_menuitem_path.py
+-rw-rw-r--   0 sonnen    (1000) sonnen    (1000)      381 2023-06-12 03:22:47.000000 aa-simplewiki-1.0.2/simplewiki/migrations/0010_rename_path_menuitem_name.py
+-rw-rw-r--   0 sonnen    (1000) sonnen    (1000)      372 2023-06-12 03:22:47.000000 aa-simplewiki-1.0.2/simplewiki/migrations/0011_rename_name_menuitem_path.py
+-rw-rw-r--   0 sonnen    (1000) sonnen    (1000)      576 2023-06-12 03:22:47.000000 aa-simplewiki-1.0.2/simplewiki/migrations/0012_menuitem_group.py
+-rw-rw-r--   0 sonnen    (1000) sonnen    (1000)      579 2023-06-12 03:22:47.000000 aa-simplewiki-1.0.2/simplewiki/migrations/0013_alter_menuitem_group.py
+-rw-rw-r--   0 sonnen    (1000) sonnen    (1000)     3030 2023-06-12 03:22:47.000000 aa-simplewiki-1.0.2/simplewiki/migrations/0014_alter_menuitem_group_alter_menuitem_icon_and_more.py
+-rw-rw-r--   0 sonnen    (1000) sonnen    (1000)      685 2023-06-12 03:22:47.000000 aa-simplewiki-1.0.2/simplewiki/migrations/0015_rename_menu_name_sectionitem_menu_path_and_more.py
+-rw-rw-r--   0 sonnen    (1000) sonnen    (1000)      407 2023-06-12 03:22:47.000000 aa-simplewiki-1.0.2/simplewiki/migrations/0016_rename_section_title_sectionitem_title.py
+-rw-rw-r--   0 sonnen    (1000) sonnen    (1000)      831 2023-06-12 03:22:47.000000 aa-simplewiki-1.0.2/simplewiki/migrations/0017_alter_sectionitem_content_alter_sectionitem_title.py
+-rw-rw-r--   0 sonnen    (1000) sonnen    (1000)      399 2023-06-12 03:22:47.000000 aa-simplewiki-1.0.2/simplewiki/migrations/0018_rename_group_menuitem_groups.py
+-rw-rw-r--   0 sonnen    (1000) sonnen    (1000)      492 2023-06-12 03:22:47.000000 aa-simplewiki-1.0.2/simplewiki/migrations/0019_alter_general_options.py
+-rw-rw-r--   0 sonnen    (1000) sonnen    (1000)      538 2023-06-12 03:22:47.000000 aa-simplewiki-1.0.2/simplewiki/migrations/0020_menuitem_parent.py
+-rw-rw-r--   0 sonnen    (1000) sonnen    (1000)        0 2023-06-12 03:22:47.000000 aa-simplewiki-1.0.2/simplewiki/migrations/__init__.py
+-rw-rw-r--   0 sonnen    (1000) sonnen    (1000)     4236 2023-06-12 03:22:47.000000 aa-simplewiki-1.0.2/simplewiki/models.py
+drwxrwxr-x   0 sonnen    (1000) sonnen    (1000)        0 2023-06-12 04:03:55.405730 aa-simplewiki-1.0.2/simplewiki/static/
+drwxrwxr-x   0 sonnen    (1000) sonnen    (1000)        0 2023-06-12 04:03:55.409730 aa-simplewiki-1.0.2/simplewiki/static/simplewiki/
+-rw-rw-r--   0 sonnen    (1000) sonnen    (1000)        0 2023-06-12 03:22:47.000000 aa-simplewiki-1.0.2/simplewiki/static/simplewiki/.gitkeep
+-rw-rw-r--   0 sonnen    (1000) sonnen    (1000)      199 2023-06-12 03:22:47.000000 aa-simplewiki-1.0.2/simplewiki/static/simplewiki/custom.css
+-rw-rw-r--   0 sonnen    (1000) sonnen    (1000)      226 2023-06-12 03:22:47.000000 aa-simplewiki-1.0.2/simplewiki/tasks.py
+drwxrwxr-x   0 sonnen    (1000) sonnen    (1000)        0 2023-06-12 04:03:55.405730 aa-simplewiki-1.0.2/simplewiki/templates/
+drwxrwxr-x   0 sonnen    (1000) sonnen    (1000)        0 2023-06-12 04:03:55.409730 aa-simplewiki-1.0.2/simplewiki/templates/simplewiki/
+-rw-rw-r--   0 sonnen    (1000) sonnen    (1000)     6324 2023-06-12 03:22:47.000000 aa-simplewiki-1.0.2/simplewiki/templates/simplewiki/base.html
+-rw-rw-r--   0 sonnen    (1000) sonnen    (1000)     1076 2023-06-12 03:22:47.000000 aa-simplewiki-1.0.2/simplewiki/templates/simplewiki/dynamic_page.html
+drwxrwxr-x   0 sonnen    (1000) sonnen    (1000)        0 2023-06-12 04:03:55.409730 aa-simplewiki-1.0.2/simplewiki/templates/simplewiki/editor/
+-rw-rw-r--   0 sonnen    (1000) sonnen    (1000)     6630 2023-06-12 03:22:47.000000 aa-simplewiki-1.0.2/simplewiki/templates/simplewiki/editor/editor_menus.html
+-rw-rw-r--   0 sonnen    (1000) sonnen    (1000)     9500 2023-06-12 03:22:47.000000 aa-simplewiki-1.0.2/simplewiki/templates/simplewiki/editor/editor_sections.html
+drwxrwxr-x   0 sonnen    (1000) sonnen    (1000)        0 2023-06-12 04:03:55.409730 aa-simplewiki-1.0.2/simplewiki/templates/simplewiki/editor/partials/
+-rw-rw-r--   0 sonnen    (1000) sonnen    (1000)     2320 2023-06-12 03:22:47.000000 aa-simplewiki-1.0.2/simplewiki/templates/simplewiki/editor/partials/_create_menu.html
+-rw-rw-r--   0 sonnen    (1000) sonnen    (1000)     2468 2023-06-12 03:22:47.000000 aa-simplewiki-1.0.2/simplewiki/templates/simplewiki/editor/partials/_edit_menu.html
+-rw-rw-r--   0 sonnen    (1000) sonnen    (1000)      593 2023-06-12 03:22:47.000000 aa-simplewiki-1.0.2/simplewiki/templates/simplewiki/error.html
+-rw-rw-r--   0 sonnen    (1000) sonnen    (1000)      460 2023-06-12 03:22:47.000000 aa-simplewiki-1.0.2/simplewiki/templates/simplewiki/index.html
+-rw-rw-r--   0 sonnen    (1000) sonnen    (1000)     1578 2023-06-12 03:22:47.000000 aa-simplewiki-1.0.2/simplewiki/templates/simplewiki/search.html
+drwxrwxr-x   0 sonnen    (1000) sonnen    (1000)        0 2023-06-12 04:03:55.409730 aa-simplewiki-1.0.2/simplewiki/templatetags/
+-rw-rw-r--   0 sonnen    (1000) sonnen    (1000)     2327 2023-06-12 03:43:22.000000 aa-simplewiki-1.0.2/simplewiki/templatetags/custom_filters.py
+-rw-rw-r--   0 sonnen    (1000) sonnen    (1000)      407 2023-06-12 03:22:47.000000 aa-simplewiki-1.0.2/simplewiki/templatetags/markdown_filters.py
+drwxrwxr-x   0 sonnen    (1000) sonnen    (1000)        0 2023-06-12 04:03:55.409730 aa-simplewiki-1.0.2/simplewiki/tests/
+-rw-rw-r--   0 sonnen    (1000) sonnen    (1000)       27 2023-06-12 03:22:47.000000 aa-simplewiki-1.0.2/simplewiki/tests/__init__.py
+-rw-rw-r--   0 sonnen    (1000) sonnen    (1000)      448 2023-06-12 03:22:47.000000 aa-simplewiki-1.0.2/simplewiki/tests/test_example.py
+-rw-rw-r--   0 sonnen    (1000) sonnen    (1000)      488 2023-06-12 03:22:47.000000 aa-simplewiki-1.0.2/simplewiki/urls.py
+-rw-rw-r--   0 sonnen    (1000) sonnen    (1000)    12859 2023-06-12 03:44:46.000000 aa-simplewiki-1.0.2/simplewiki/views.py
+drwxrwxr-x   0 sonnen    (1000) sonnen    (1000)        0 2023-06-12 04:03:55.409730 aa-simplewiki-1.0.2/testauth/
+-rw-rw-r--   0 sonnen    (1000) sonnen    (1000)       52 2023-06-12 03:22:47.000000 aa-simplewiki-1.0.2/testauth/__init__.py
+-rw-rw-r--   0 sonnen    (1000) sonnen    (1000)      654 2023-06-12 03:22:47.000000 aa-simplewiki-1.0.2/testauth/celery.py
+-rw-rw-r--   0 sonnen    (1000) sonnen    (1000)     9481 2023-06-12 03:22:47.000000 aa-simplewiki-1.0.2/testauth/settings.py
+-rw-rw-r--   0 sonnen    (1000) sonnen    (1000)      167 2023-06-12 03:22:47.000000 aa-simplewiki-1.0.2/testauth/urls.py
+-rw-rw-r--   0 sonnen    (1000) sonnen    (1000)      425 2023-06-12 03:22:47.000000 aa-simplewiki-1.0.2/testauth/wsgi.py
```

### Comparing `aa-simplewiki-1.0.1/LICENSE` & `aa-simplewiki-1.0.2/LICENSE`

 * *Files identical despite different names*

### Comparing `aa-simplewiki-1.0.1/PKG-INFO` & `aa-simplewiki-1.0.2/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: aa-simplewiki
-Version: 1.0.1
+Version: 1.0.2
 Summary: Alliance Auth Wiki Plugin
 Home-page: https://github.com/meowosaurus/aa-simplewiki
 Author: Meowosaurus
 Author-email: info@bjsonnen.de
 Maintainer: Peter Pfeufer
 Maintainer-email: development@ppfeufer.de
 License: GNU General Public License v3 (GPLv3)
```

### Comparing `aa-simplewiki-1.0.1/README.md` & `aa-simplewiki-1.0.2/README.md`

 * *Files identical despite different names*

### Comparing `aa-simplewiki-1.0.1/aa_simplewiki.egg-info/PKG-INFO` & `aa-simplewiki-1.0.2/aa_simplewiki.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: aa-simplewiki
-Version: 1.0.1
+Version: 1.0.2
 Summary: Alliance Auth Wiki Plugin
 Home-page: https://github.com/meowosaurus/aa-simplewiki
 Author: Meowosaurus
 Author-email: info@bjsonnen.de
 Maintainer: Peter Pfeufer
 Maintainer-email: development@ppfeufer.de
 License: GNU General Public License v3 (GPLv3)
```

### Comparing `aa-simplewiki-1.0.1/aa_simplewiki.egg-info/SOURCES.txt` & `aa-simplewiki-1.0.2/aa_simplewiki.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `aa-simplewiki-1.0.1/setup.cfg` & `aa-simplewiki-1.0.2/setup.cfg`

 * *Files identical despite different names*

### Comparing `aa-simplewiki-1.0.1/setup.py` & `aa-simplewiki-1.0.2/setup.py`

 * *Files identical despite different names*

### Comparing `aa-simplewiki-1.0.1/simplewiki/admin_helper_menus.py` & `aa-simplewiki-1.0.2/simplewiki/admin_helper_menus.py`

 * *Files 0% similar despite different names*

```diff
@@ -61,15 +61,17 @@
                 context.update({'error_code': '#1003'})
                 context.update({'error_django': str(e)})
                 return render(request, 'simplewiki/error.html', context)
             except Exception as e:
                 return render(request, 'simplewiki/error.html', gen_error_context(context, '#1003', e))
 
         # Take all inputs from the group multiple select and put them in a string, seperated by a comma
-        group_string = ""
+        #group_string = ""
+        group_string = str()
+        
         try:
             
             groups = request.POST.getlist('group_select')
 
             for group_item in groups:
                 group_string += group_item
                 group_string += ","
```

### Comparing `aa-simplewiki-1.0.1/simplewiki/admin_helper_sections.py` & `aa-simplewiki-1.0.2/simplewiki/admin_helper_sections.py`

 * *Files identical despite different names*

### Comparing `aa-simplewiki-1.0.1/simplewiki/auth_hooks.py` & `aa-simplewiki-1.0.2/simplewiki/auth_hooks.py`

 * *Files identical despite different names*

### Comparing `aa-simplewiki-1.0.1/simplewiki/migrations/0001_initial.py` & `aa-simplewiki-1.0.2/simplewiki/migrations/0001_initial.py`

 * *Files identical despite different names*

### Comparing `aa-simplewiki-1.0.1/simplewiki/migrations/0004_pageitem_icon_alter_menuitem_icon_and_more.py` & `aa-simplewiki-1.0.2/simplewiki/migrations/0004_pageitem_icon_alter_menuitem_icon_and_more.py`

 * *Files identical despite different names*

### Comparing `aa-simplewiki-1.0.1/simplewiki/migrations/0005_alter_menuitem_icon_alter_pageitem_content_and_more.py` & `aa-simplewiki-1.0.2/simplewiki/migrations/0005_alter_menuitem_icon_alter_pageitem_content_and_more.py`

 * *Files identical despite different names*

### Comparing `aa-simplewiki-1.0.1/simplewiki/migrations/0008_alter_general_options_alter_menuitem_icon_and_more.py` & `aa-simplewiki-1.0.2/simplewiki/migrations/0008_alter_general_options_alter_menuitem_icon_and_more.py`

 * *Files identical despite different names*

### Comparing `aa-simplewiki-1.0.1/simplewiki/migrations/0009_remove_menuitem_name_menuitem_path.py` & `aa-simplewiki-1.0.2/simplewiki/migrations/0009_remove_menuitem_name_menuitem_path.py`

 * *Files identical despite different names*

### Comparing `aa-simplewiki-1.0.1/simplewiki/migrations/0012_menuitem_group.py` & `aa-simplewiki-1.0.2/simplewiki/migrations/0012_menuitem_group.py`

 * *Files identical despite different names*

### Comparing `aa-simplewiki-1.0.1/simplewiki/migrations/0013_alter_menuitem_group.py` & `aa-simplewiki-1.0.2/simplewiki/migrations/0013_alter_menuitem_group.py`

 * *Files identical despite different names*

### Comparing `aa-simplewiki-1.0.1/simplewiki/migrations/0014_alter_menuitem_group_alter_menuitem_icon_and_more.py` & `aa-simplewiki-1.0.2/simplewiki/migrations/0014_alter_menuitem_group_alter_menuitem_icon_and_more.py`

 * *Files identical despite different names*

### Comparing `aa-simplewiki-1.0.1/simplewiki/migrations/0015_rename_menu_name_sectionitem_menu_path_and_more.py` & `aa-simplewiki-1.0.2/simplewiki/migrations/0015_rename_menu_name_sectionitem_menu_path_and_more.py`

 * *Files identical despite different names*

### Comparing `aa-simplewiki-1.0.1/simplewiki/migrations/0017_alter_sectionitem_content_alter_sectionitem_title.py` & `aa-simplewiki-1.0.2/simplewiki/migrations/0017_alter_sectionitem_content_alter_sectionitem_title.py`

 * *Files identical despite different names*

### Comparing `aa-simplewiki-1.0.1/simplewiki/migrations/0020_menuitem_parent.py` & `aa-simplewiki-1.0.2/simplewiki/migrations/0020_menuitem_parent.py`

 * *Files identical despite different names*

### Comparing `aa-simplewiki-1.0.1/simplewiki/models.py` & `aa-simplewiki-1.0.2/simplewiki/models.py`

 * *Files identical despite different names*

### Comparing `aa-simplewiki-1.0.1/simplewiki/templates/simplewiki/base.html` & `aa-simplewiki-1.0.2/simplewiki/templates/simplewiki/base.html`

 * *Files identical despite different names*

### Comparing `aa-simplewiki-1.0.1/simplewiki/templates/simplewiki/dynamic_page.html` & `aa-simplewiki-1.0.2/simplewiki/templates/simplewiki/dynamic_page.html`

 * *Files identical despite different names*

### Comparing `aa-simplewiki-1.0.1/simplewiki/templates/simplewiki/editor/editor_menus.html` & `aa-simplewiki-1.0.2/simplewiki/templates/simplewiki/editor/editor_menus.html`

 * *Files identical despite different names*

### Comparing `aa-simplewiki-1.0.1/simplewiki/templates/simplewiki/editor/editor_sections.html` & `aa-simplewiki-1.0.2/simplewiki/templates/simplewiki/editor/editor_sections.html`

 * *Files identical despite different names*

### Comparing `aa-simplewiki-1.0.1/simplewiki/templates/simplewiki/editor/partials/_create_menu.html` & `aa-simplewiki-1.0.2/simplewiki/templates/simplewiki/editor/partials/_create_menu.html`

 * *Files identical despite different names*

### Comparing `aa-simplewiki-1.0.1/simplewiki/templates/simplewiki/editor/partials/_edit_menu.html` & `aa-simplewiki-1.0.2/simplewiki/templates/simplewiki/editor/partials/_edit_menu.html`

 * *Files identical despite different names*

### Comparing `aa-simplewiki-1.0.1/simplewiki/templates/simplewiki/error.html` & `aa-simplewiki-1.0.2/simplewiki/templates/simplewiki/error.html`

 * *Files identical despite different names*

### Comparing `aa-simplewiki-1.0.1/simplewiki/templates/simplewiki/search.html` & `aa-simplewiki-1.0.2/simplewiki/templates/simplewiki/search.html`

 * *Files identical despite different names*

### Comparing `aa-simplewiki-1.0.1/simplewiki/templatetags/custom_filters.py` & `aa-simplewiki-1.0.2/simplewiki/templatetags/custom_filters.py`

 * *Files 5% similar despite different names*

```diff
@@ -13,23 +13,25 @@
         user_groups: All groups held by the user
         group_list: All groups required by the menu
 
     Returns:
         bool: Returns true if the user is at least in one of the required groups
     """
 
+    # Try to split group lists into any array based on comma
     try:
         if group_list is not None and isinstance(group_list, str):
             group_names = group_list.split(',')
         else:
             return False
     except Exception as e:
         return False
 
-    return any(group_name in user_groups for group_name in group_names)
+    # Check if the user has any groups or if the menu doesn't even require any groups
+    return any(group_name in user_groups for group_name in group_names) or any(group_name == "none" for group_name in group_names)
 
 def add_group_space(text: str) -> str:
     return text.replace(',', ', ')
 
 def has_menu_children(menu_item):
     # If any other menu has menu_item as parent
     return MenuItem.objects.filter(parent=menu_item.path).exists()
```

### Comparing `aa-simplewiki-1.0.1/simplewiki/views.py` & `aa-simplewiki-1.0.2/simplewiki/views.py`

 * *Files 5% similar despite different names*

```diff
@@ -88,28 +88,30 @@
             if first_menu_submenus.count() > 0:
                 for first_menu_item in first_menu_submenus:
                     # If the submenu has any groups
                     if first_menu_item.groups:
                         group_names = first_menu_item.groups.split(',')
                         user_groups = list(request.user.groups.values_list('name', flat=True))
 
+                        print(group_names)
+
                         # If the user has the right to access this submenu
-                        if any(group_name in user_groups for group_name in group_names):
+                        if any(group_name in user_groups for group_name in group_names) or any(element == "none" for element in group_names):
                             return redirect('simplewiki:dynamic_menu', first_menu_item)
                     else:
                         return redirect('simplewiki:dynamic_menu', first_menu_item)
             # If the menu doesn't have submenus
             else:
                 # If the parent menu has any groups
                 if parent_menu_item.groups:
                     group_names = parent_menu_item.groups.split(',')
                     user_groups = list(request.user.groups.values_list('name', flat=True))
 
                     # If the user has the right to access the parent menu
-                    if any(group_name in user_groups for group_name in group_names):
+                    if any(group_name in user_groups for group_name in group_names) or any(element == "none" for element in group_names):
                         return redirect('simplewiki:dynamic_menu', parent_menu_item)
                 else:
                     return redirect('simplewiki:dynamic_menu', parent_menu_item)
 
         # If there are no menus the user has permission to access
         error_code = "#1000"
         error_message = "You don't have the permission to access any menus. Please contact the administrator."
@@ -151,19 +153,19 @@
     requested_menu = MenuItem.objects.get(path=menu_name)
 
     # Split all group names. All group names need to be seperated by a comma
     try:
         group_names = requested_menu.groups.split(',')
     except Exception as e:
         group_names = ""
-    
+
     context.update({'group_names': group_names})
 
     #if not requested_menu.groups or requested_menu.groups in list(request.user.groups.values_list('name', flat=True)):
-    if not requested_menu.groups or any(group_name in request.user.groups.values_list('name', flat=True) for group_name in group_names):
+    if any(group_name in request.user.groups.values_list('name', flat=True) for group_name in group_names) or any(element == "none" for element in group_names):
         return render(request, 'simplewiki/dynamic_page.html', context)
     else:
         # If more then two groups are required
         if len(requested_menu.groups.split(',')) > 1:
             group_plural = "groups"
         else:
             group_plural = "group"
```

### Comparing `aa-simplewiki-1.0.1/testauth/celery.py` & `aa-simplewiki-1.0.2/testauth/celery.py`

 * *Files identical despite different names*

### Comparing `aa-simplewiki-1.0.1/testauth/settings.py` & `aa-simplewiki-1.0.2/testauth/settings.py`

 * *Files identical despite different names*

