# Comparing `tmp/bl_hector-0.1.0a3.tar.gz` & `tmp/bl_hector-0.1.0a4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "bl_hector-0.1.0a3.tar", max compression
+gzip compressed data, was "bl_hector-0.1.0a4.tar", max compression
```

## Comparing `bl_hector-0.1.0a3.tar` & `bl_hector-0.1.0a4.tar`

### file list

```diff
@@ -1,88 +1,90 @@
--rw-r--r--   0        0        0    34523 2023-05-31 09:45:12.827540 bl_hector-0.1.0a3/LICENSE
--rw-r--r--   0        0        0     1264 2023-06-09 06:16:19.346310 bl_hector-0.1.0a3/README.md
--rw-r--r--   0        0        0      807 2023-06-07 16:14:27.658555 bl_hector-0.1.0a3/bl_hector/__init__.py
--rw-r--r--   0        0        0      721 2023-06-07 16:14:27.658555 bl_hector-0.1.0a3/bl_hector/application/__init__.py
--rw-r--r--   0        0        0      721 2023-06-07 16:14:27.658555 bl_hector-0.1.0a3/bl_hector/application/use_cases/__init__.py
--rw-r--r--   0        0        0     2378 2023-06-09 06:16:19.346310 bl_hector-0.1.0a3/bl_hector/application/use_cases/add_book.py
--rw-r--r--   0        0        0     1981 2023-06-09 06:16:19.350310 bl_hector-0.1.0a3/bl_hector/application/use_cases/display_book.py
--rw-r--r--   0        0        0     3472 2023-06-09 06:16:19.350310 bl_hector-0.1.0a3/bl_hector/application/use_cases/import_books.py
--rw-r--r--   0        0        0     1846 2023-06-09 06:16:19.350310 bl_hector-0.1.0a3/bl_hector/application/use_cases/look_up_book.py
--rw-r--r--   0        0        0     2690 2023-06-09 06:16:19.350310 bl_hector-0.1.0a3/bl_hector/application/use_cases/search_books.py
--rw-r--r--   0        0        0     2442 2023-06-09 06:16:19.350310 bl_hector-0.1.0a3/bl_hector/application/use_cases/update_book.py
--rw-r--r--   0        0        0      944 2023-06-07 16:14:27.658555 bl_hector-0.1.0a3/bl_hector/configuration/__init__.py
--rw-r--r--   0        0        0      981 2023-06-07 16:14:27.658555 bl_hector-0.1.0a3/bl_hector/configuration/cli.py
--rw-r--r--   0        0        0      986 2023-06-07 16:14:27.658555 bl_hector-0.1.0a3/bl_hector/configuration/wsgi.py
--rw-r--r--   0        0        0      721 2023-06-07 16:14:27.658555 bl_hector-0.1.0a3/bl_hector/domain/__init__.py
--rw-r--r--   0        0        0      721 2023-06-07 16:14:27.658555 bl_hector-0.1.0a3/bl_hector/domain/administration/__init__.py
--rw-r--r--   0        0        0     1272 2023-06-07 16:14:27.658555 bl_hector-0.1.0a3/bl_hector/domain/administration/entities.py
--rw-r--r--   0        0        0     1452 2023-06-07 16:14:27.658555 bl_hector-0.1.0a3/bl_hector/domain/administration/repositories.py
--rw-r--r--   0        0        0     1196 2023-06-07 16:14:27.658555 bl_hector-0.1.0a3/bl_hector/domain/administration/services.py
--rw-r--r--   0        0        0      931 2023-06-07 16:14:27.658555 bl_hector-0.1.0a3/bl_hector/domain/administration/value_objects.py
--rw-r--r--   0        0        0      721 2023-06-07 16:14:27.658555 bl_hector-0.1.0a3/bl_hector/domain/collection_management/__init__.py
--rw-r--r--   0        0        0     1449 2023-06-09 06:16:19.350310 bl_hector-0.1.0a3/bl_hector/domain/collection_management/entities.py
--rw-r--r--   0        0        0      996 2023-06-07 16:14:27.658555 bl_hector-0.1.0a3/bl_hector/domain/collection_management/exceptions.py
--rw-r--r--   0        0        0     1509 2023-06-07 16:14:27.658555 bl_hector-0.1.0a3/bl_hector/domain/collection_management/repositories.py
--rw-r--r--   0        0        0      958 2023-06-07 16:14:27.658555 bl_hector-0.1.0a3/bl_hector/domain/collection_management/services.py
--rw-r--r--   0        0        0     3309 2023-06-07 16:14:27.658555 bl_hector-0.1.0a3/bl_hector/domain/collection_management/value_objects.py
--rw-r--r--   0        0        0      721 2023-06-07 16:14:27.658555 bl_hector-0.1.0a3/bl_hector/infrastructure/__init__.py
--rw-r--r--   0        0        0     2553 2023-06-09 06:16:19.354310 bl_hector-0.1.0a3/bl_hector/infrastructure/flask/__init__.py
--rw-r--r--   0        0        0     1064 2023-06-07 16:14:27.658555 bl_hector-0.1.0a3/bl_hector/infrastructure/flask/aliases/__init__.py
--rw-r--r--   0        0        0     1733 2023-06-09 06:16:19.354310 bl_hector-0.1.0a3/bl_hector/infrastructure/flask/auth/__init__.py
--rw-r--r--   0        0        0     3942 2023-06-07 16:14:27.658555 bl_hector-0.1.0a3/bl_hector/infrastructure/flask/books/__init__.py
--rw-r--r--   0        0        0     2899 2023-06-07 16:14:27.662555 bl_hector-0.1.0a3/bl_hector/infrastructure/flask/services.py
--rw-r--r--   0        0        0   207302 2023-06-07 16:14:27.662555 bl_hector-0.1.0a3/bl_hector/infrastructure/flask/static/css/bulma@0.9.4.min.css
--rw-r--r--   0        0        0    73117 2023-06-07 16:14:27.662555 bl_hector-0.1.0a3/bl_hector/infrastructure/flask/static/css/font-awesome@5.14.0.css
--rw-r--r--   0        0        0      482 2023-06-07 16:14:27.662555 bl_hector-0.1.0a3/bl_hector/infrastructure/flask/static/css/hector.css
--rw-r--r--   0        0        0      655 2023-06-07 16:14:27.662555 bl_hector-0.1.0a3/bl_hector/infrastructure/flask/static/favicon.svg
--rw-r--r--   0        0        0    35880 2023-06-07 16:14:27.662555 bl_hector-0.1.0a3/bl_hector/infrastructure/flask/static/img/placeholders/1280x960.png
--rw-r--r--   0        0        0      928 2023-06-07 16:14:27.662555 bl_hector-0.1.0a3/bl_hector/infrastructure/flask/static/img/placeholders/320x480.png
--rw-r--r--   0        0        0     3602 2023-06-07 16:14:27.662555 bl_hector-0.1.0a3/bl_hector/infrastructure/flask/static/img/placeholders/96x96.png
--rw-r--r--   0        0        0    42819 2023-06-07 16:14:27.670555 bl_hector-0.1.0a3/bl_hector/infrastructure/flask/static/js/htmx@1.9.2.min.js
--rw-r--r--   0        0        0    97249 2023-06-07 16:14:27.670555 bl_hector-0.1.0a3/bl_hector/infrastructure/flask/static/js/hyperscript@0.9.8.min.js
--rw-r--r--   0        0        0     6828 2023-06-07 16:14:27.670555 bl_hector-0.1.0a3/bl_hector/infrastructure/flask/static/js/simplewebauthn-browser@7.2.0.umd.min.js
--rw-r--r--   0        0        0   186112 2023-06-07 16:14:27.670555 bl_hector-0.1.0a3/bl_hector/infrastructure/flask/static/webfonts/fa-brands-400.ttf
--rw-r--r--   0        0        0   107460 2023-06-07 16:14:27.674555 bl_hector-0.1.0a3/bl_hector/infrastructure/flask/static/webfonts/fa-brands-400.woff2
--rw-r--r--   0        0        0    62048 2023-06-07 16:14:27.674555 bl_hector-0.1.0a3/bl_hector/infrastructure/flask/static/webfonts/fa-regular-400.ttf
--rw-r--r--   0        0        0    25096 2023-06-07 16:14:27.674555 bl_hector-0.1.0a3/bl_hector/infrastructure/flask/static/webfonts/fa-regular-400.woff2
--rw-r--r--   0        0        0   397728 2023-06-07 16:14:27.674555 bl_hector-0.1.0a3/bl_hector/infrastructure/flask/static/webfonts/fa-solid-900.ttf
--rw-r--r--   0        0        0   150472 2023-06-07 16:14:27.674555 bl_hector-0.1.0a3/bl_hector/infrastructure/flask/static/webfonts/fa-solid-900.woff2
--rw-r--r--   0        0        0     1802 2023-06-07 16:14:27.674555 bl_hector-0.1.0a3/bl_hector/infrastructure/flask/utils.py
--rw-r--r--   0        0        0     4400 2023-06-09 06:16:19.354310 bl_hector-0.1.0a3/bl_hector/infrastructure/flask/webauthn/__init__.py
--rw-r--r--   0        0        0     3119 2023-06-07 16:14:27.674555 bl_hector-0.1.0a3/bl_hector/infrastructure/flask/webauthn/security.py
--rw-r--r--   0        0        0     1641 2023-06-07 16:14:27.674555 bl_hector-0.1.0a3/bl_hector/infrastructure/isbnlib/__init__.py
--rw-r--r--   0        0        0     1775 2023-06-09 06:16:19.354310 bl_hector-0.1.0a3/bl_hector/infrastructure/settings.py
--rw-r--r--   0        0        0      721 2023-06-07 16:14:27.674555 bl_hector-0.1.0a3/bl_hector/infrastructure/sqlalchemy/__init__.py
--rw-r--r--   0        0        0     7982 2023-06-07 16:14:27.674555 bl_hector-0.1.0a3/bl_hector/infrastructure/sqlalchemy/repositories.py
--rw-r--r--   0        0        0     2058 2023-06-07 16:14:27.674555 bl_hector-0.1.0a3/bl_hector/infrastructure/typer/__init__.py
--rw-r--r--   0        0        0     2718 2023-06-07 16:14:27.682555 bl_hector-0.1.0a3/bl_hector/infrastructure/typer/books.py
--rw-r--r--   0        0        0     1866 2023-06-07 16:14:27.682555 bl_hector-0.1.0a3/bl_hector/infrastructure/typer/services.py
--rw-r--r--   0        0        0      810 2023-06-07 16:14:27.682555 bl_hector-0.1.0a3/bl_hector/interfaces/__init__.py
--rw-r--r--   0        0        0     3454 2023-06-07 16:14:27.682555 bl_hector-0.1.0a3/bl_hector/interfaces/from_dict.py
--rw-r--r--   0        0        0     1517 2023-06-07 16:14:27.682555 bl_hector-0.1.0a3/bl_hector/interfaces/from_json.py
--rw-r--r--   0        0        0     1435 2023-06-07 17:00:49.589157 bl_hector-0.1.0a3/bl_hector/interfaces/l10n/__init__.py
--rw-r--r--   0        0        0     3901 2023-06-09 06:16:19.354310 bl_hector-0.1.0a3/bl_hector/interfaces/l10n/en-GB/main.ftl
--rw-r--r--   0        0        0     4397 2023-06-09 06:16:19.354310 bl_hector-0.1.0a3/bl_hector/interfaces/l10n/fr-FR/main.ftl
--rw-r--r--   0        0        0     1407 2023-06-07 16:14:27.682555 bl_hector-0.1.0a3/bl_hector/interfaces/to_http/__init__.py
--rw-r--r--   0        0        0    13523 2023-06-09 06:16:19.358310 bl_hector-0.1.0a3/bl_hector/interfaces/to_http/as_html/__init__.py
--rw-r--r--   0        0        0     1254 2023-06-09 06:16:19.358310 bl_hector-0.1.0a3/bl_hector/interfaces/to_http/as_html/templates/auth/login.pug
--rw-r--r--   0        0        0     3951 2023-06-07 16:14:27.682555 bl_hector-0.1.0a3/bl_hector/interfaces/to_http/as_html/templates/books/add.pug
--rw-r--r--   0        0        0     2001 2023-06-07 16:57:40.623777 bl_hector-0.1.0a3/bl_hector/interfaces/to_http/as_html/templates/books/display.pug
--rw-r--r--   0        0        0     1612 2023-06-07 16:14:27.682555 bl_hector-0.1.0a3/bl_hector/interfaces/to_http/as_html/templates/books/mixins/render_isbn.pug
--rw-r--r--   0        0        0     4925 2023-06-07 16:14:27.682555 bl_hector-0.1.0a3/bl_hector/interfaces/to_http/as_html/templates/books/search.pug
--rw-r--r--   0        0        0     3255 2023-06-07 16:58:07.111390 bl_hector-0.1.0a3/bl_hector/interfaces/to_http/as_html/templates/books/update.pug
--rw-r--r--   0        0        0      978 2023-06-07 16:14:27.682555 bl_hector-0.1.0a3/bl_hector/interfaces/to_http/as_html/templates/error.pug
--rw-r--r--   0        0        0     2043 2023-06-07 16:57:22.668045 bl_hector-0.1.0a3/bl_hector/interfaces/to_http/as_html/templates/layout.pug
--rw-r--r--   0        0        0     1122 2023-06-07 16:14:27.682555 bl_hector-0.1.0a3/bl_hector/interfaces/to_http/as_html/templates/mixins/flash.pug
--rw-r--r--   0        0        0     3812 2023-06-07 16:14:27.682555 bl_hector-0.1.0a3/bl_hector/interfaces/to_http/as_html/templates/mixins/form.pug
--rw-r--r--   0        0        0     2010 2023-06-09 06:16:19.358310 bl_hector-0.1.0a3/bl_hector/interfaces/to_http/as_html/templates/mixins/navbar.pug
--rw-r--r--   0        0        0     2010 2023-06-07 16:14:27.682555 bl_hector-0.1.0a3/bl_hector/interfaces/to_http/as_html/templates/webauthn/login.pug
--rw-r--r--   0        0        0     2045 2023-06-07 16:14:27.682555 bl_hector-0.1.0a3/bl_hector/interfaces/to_http/as_html/templates/webauthn/register.pug
--rw-r--r--   0        0        0     1310 2023-06-07 16:14:27.682555 bl_hector-0.1.0a3/bl_hector/interfaces/to_http/as_json/__init__.py
--rw-r--r--   0        0        0     1211 2023-06-07 16:14:27.682555 bl_hector-0.1.0a3/bl_hector/interfaces/to_terminal/__init__.py
--rw-r--r--   0        0        0     1818 2023-06-09 06:16:19.358310 bl_hector-0.1.0a3/bl_hector/interfaces/to_terminal/as_json.py
--rw-r--r--   0        0        0     4250 2023-06-09 06:16:19.358310 bl_hector-0.1.0a3/bl_hector/interfaces/to_terminal/as_text.py
--rw-r--r--   0        0        0     1519 2023-06-07 16:14:27.682555 bl_hector-0.1.0a3/bl_hector/interfaces/utils.py
--rw-r--r--   0        0        0     5187 2023-06-09 06:16:19.362310 bl_hector-0.1.0a3/bl_hector/interfaces/validators.py
--rw-r--r--   0        0        0     1407 2023-06-09 06:18:32.252717 bl_hector-0.1.0a3/pyproject.toml
--rw-r--r--   0        0        0     3829 2023-06-09 06:19:45.006316 bl_hector-0.1.0a3/setup.py
--rw-r--r--   0        0        0     2216 2023-06-09 06:19:45.007271 bl_hector-0.1.0a3/PKG-INFO
+-rw-r--r--   0        0        0    34523 2023-06-01 06:44:39.561559 bl_hector-0.1.0a4/LICENSE
+-rw-r--r--   0        0        0     1264 2023-06-08 11:40:14.535293 bl_hector-0.1.0a4/README.md
+-rw-r--r--   0        0        0      807 2023-06-08 06:35:01.974074 bl_hector-0.1.0a4/bl_hector/__init__.py
+-rw-r--r--   0        0        0      721 2023-06-08 06:35:01.974074 bl_hector-0.1.0a4/bl_hector/application/__init__.py
+-rw-r--r--   0        0        0      721 2023-06-08 06:35:01.974074 bl_hector-0.1.0a4/bl_hector/application/use_cases/__init__.py
+-rw-r--r--   0        0        0     3639 2023-06-12 06:39:33.409846 bl_hector-0.1.0a4/bl_hector/application/use_cases/add_book.py
+-rw-r--r--   0        0        0     1981 2023-06-08 13:54:13.278547 bl_hector-0.1.0a4/bl_hector/application/use_cases/display_book.py
+-rw-r--r--   0        0        0     3472 2023-06-08 13:55:05.761614 bl_hector-0.1.0a4/bl_hector/application/use_cases/import_books.py
+-rw-r--r--   0        0        0     1846 2023-06-08 13:57:02.571540 bl_hector-0.1.0a4/bl_hector/application/use_cases/look_up_book.py
+-rw-r--r--   0        0        0     3755 2023-06-12 06:39:33.409846 bl_hector-0.1.0a4/bl_hector/application/use_cases/search_books.py
+-rw-r--r--   0        0        0     3612 2023-06-12 06:39:33.413846 bl_hector-0.1.0a4/bl_hector/application/use_cases/update_book.py
+-rw-r--r--   0        0        0      944 2023-06-08 06:35:01.974074 bl_hector-0.1.0a4/bl_hector/configuration/__init__.py
+-rw-r--r--   0        0        0      981 2023-06-08 06:35:01.974074 bl_hector-0.1.0a4/bl_hector/configuration/cli.py
+-rw-r--r--   0        0        0      986 2023-06-08 06:35:01.974074 bl_hector-0.1.0a4/bl_hector/configuration/wsgi.py
+-rw-r--r--   0        0        0      721 2023-06-08 06:35:01.974074 bl_hector-0.1.0a4/bl_hector/domain/__init__.py
+-rw-r--r--   0        0        0      721 2023-06-08 06:35:01.974074 bl_hector-0.1.0a4/bl_hector/domain/administration/__init__.py
+-rw-r--r--   0        0        0     1272 2023-06-08 06:35:01.974074 bl_hector-0.1.0a4/bl_hector/domain/administration/entities.py
+-rw-r--r--   0        0        0      808 2023-06-12 06:39:33.413846 bl_hector-0.1.0a4/bl_hector/domain/administration/enumerations.py
+-rw-r--r--   0        0        0     1659 2023-06-12 06:39:33.413846 bl_hector-0.1.0a4/bl_hector/domain/administration/repositories.py
+-rw-r--r--   0        0        0     1196 2023-06-08 06:35:01.974074 bl_hector-0.1.0a4/bl_hector/domain/administration/services.py
+-rw-r--r--   0        0        0      931 2023-06-08 06:35:01.974074 bl_hector-0.1.0a4/bl_hector/domain/administration/value_objects.py
+-rw-r--r--   0        0        0      721 2023-06-08 06:35:01.974074 bl_hector-0.1.0a4/bl_hector/domain/collection_management/__init__.py
+-rw-r--r--   0        0        0     1449 2023-06-08 14:33:06.629178 bl_hector-0.1.0a4/bl_hector/domain/collection_management/entities.py
+-rw-r--r--   0        0        0      996 2023-06-08 06:35:01.974074 bl_hector-0.1.0a4/bl_hector/domain/collection_management/exceptions.py
+-rw-r--r--   0        0        0     1509 2023-06-08 06:35:01.974074 bl_hector-0.1.0a4/bl_hector/domain/collection_management/repositories.py
+-rw-r--r--   0        0        0      958 2023-06-08 06:35:01.974074 bl_hector-0.1.0a4/bl_hector/domain/collection_management/services.py
+-rw-r--r--   0        0        0     1804 2023-06-12 06:39:33.413846 bl_hector-0.1.0a4/bl_hector/domain/collection_management/validators.py
+-rw-r--r--   0        0        0     3309 2023-06-08 13:46:42.562514 bl_hector-0.1.0a4/bl_hector/domain/collection_management/value_objects.py
+-rw-r--r--   0        0        0     1124 2023-06-12 06:39:33.413846 bl_hector-0.1.0a4/bl_hector/infrastructure/__init__.py
+-rw-r--r--   0        0        0     3406 2023-06-12 06:39:33.413846 bl_hector-0.1.0a4/bl_hector/infrastructure/flask/__init__.py
+-rw-r--r--   0        0        0     1064 2023-06-08 06:35:01.974074 bl_hector-0.1.0a4/bl_hector/infrastructure/flask/aliases/__init__.py
+-rw-r--r--   0        0        0     1693 2023-06-12 06:39:33.413846 bl_hector-0.1.0a4/bl_hector/infrastructure/flask/auth/__init__.py
+-rw-r--r--   0        0        0     3966 2023-06-12 06:39:33.413846 bl_hector-0.1.0a4/bl_hector/infrastructure/flask/books/__init__.py
+-rw-r--r--   0        0        0     3121 2023-06-12 06:39:33.413846 bl_hector-0.1.0a4/bl_hector/infrastructure/flask/services.py
+-rw-r--r--   0        0        0   207302 2023-06-08 06:35:01.974074 bl_hector-0.1.0a4/bl_hector/infrastructure/flask/static/css/bulma@0.9.4.min.css
+-rw-r--r--   0        0        0    73117 2023-06-08 06:35:01.978074 bl_hector-0.1.0a4/bl_hector/infrastructure/flask/static/css/font-awesome@5.14.0.css
+-rw-r--r--   0        0        0      584 2023-06-12 06:39:33.413846 bl_hector-0.1.0a4/bl_hector/infrastructure/flask/static/css/hector.css
+-rw-r--r--   0        0        0      655 2023-06-08 06:35:01.978074 bl_hector-0.1.0a4/bl_hector/infrastructure/flask/static/favicon.svg
+-rw-r--r--   0        0        0    35880 2023-06-08 06:35:01.978074 bl_hector-0.1.0a4/bl_hector/infrastructure/flask/static/img/placeholders/1280x960.png
+-rw-r--r--   0        0        0      928 2023-06-08 06:35:01.978074 bl_hector-0.1.0a4/bl_hector/infrastructure/flask/static/img/placeholders/320x480.png
+-rw-r--r--   0        0        0     3602 2023-06-08 06:35:01.978074 bl_hector-0.1.0a4/bl_hector/infrastructure/flask/static/img/placeholders/96x96.png
+-rw-r--r--   0        0        0    42819 2023-06-08 06:35:01.978074 bl_hector-0.1.0a4/bl_hector/infrastructure/flask/static/js/htmx@1.9.2.min.js
+-rw-r--r--   0        0        0    97249 2023-06-08 06:35:01.978074 bl_hector-0.1.0a4/bl_hector/infrastructure/flask/static/js/hyperscript@0.9.8.min.js
+-rw-r--r--   0        0        0     6828 2023-06-08 06:35:01.978074 bl_hector-0.1.0a4/bl_hector/infrastructure/flask/static/js/simplewebauthn-browser@7.2.0.umd.min.js
+-rw-r--r--   0        0        0   186112 2023-06-08 06:35:01.982074 bl_hector-0.1.0a4/bl_hector/infrastructure/flask/static/webfonts/fa-brands-400.ttf
+-rw-r--r--   0        0        0   107460 2023-06-08 06:35:01.982074 bl_hector-0.1.0a4/bl_hector/infrastructure/flask/static/webfonts/fa-brands-400.woff2
+-rw-r--r--   0        0        0    62048 2023-06-08 06:35:01.982074 bl_hector-0.1.0a4/bl_hector/infrastructure/flask/static/webfonts/fa-regular-400.ttf
+-rw-r--r--   0        0        0    25096 2023-06-08 06:35:01.982074 bl_hector-0.1.0a4/bl_hector/infrastructure/flask/static/webfonts/fa-regular-400.woff2
+-rw-r--r--   0        0        0   397728 2023-06-08 06:35:01.982074 bl_hector-0.1.0a4/bl_hector/infrastructure/flask/static/webfonts/fa-solid-900.ttf
+-rw-r--r--   0        0        0   150472 2023-06-08 06:35:01.982074 bl_hector-0.1.0a4/bl_hector/infrastructure/flask/static/webfonts/fa-solid-900.woff2
+-rw-r--r--   0        0        0     1265 2023-06-12 06:39:33.413846 bl_hector-0.1.0a4/bl_hector/infrastructure/flask/utils.py
+-rw-r--r--   0        0        0     4544 2023-06-12 06:52:18.855459 bl_hector-0.1.0a4/bl_hector/infrastructure/flask/webauthn/__init__.py
+-rw-r--r--   0        0        0     3282 2023-06-12 06:52:18.855459 bl_hector-0.1.0a4/bl_hector/infrastructure/flask/webauthn/security.py
+-rw-r--r--   0        0        0     1641 2023-06-08 06:35:01.982074 bl_hector-0.1.0a4/bl_hector/infrastructure/isbnlib/__init__.py
+-rw-r--r--   0        0        0     1940 2023-06-12 06:39:33.413846 bl_hector-0.1.0a4/bl_hector/infrastructure/settings.py
+-rw-r--r--   0        0        0      721 2023-06-08 06:35:01.982074 bl_hector-0.1.0a4/bl_hector/infrastructure/sqlalchemy/__init__.py
+-rw-r--r--   0        0        0     7982 2023-06-12 06:52:18.855459 bl_hector-0.1.0a4/bl_hector/infrastructure/sqlalchemy/repositories.py
+-rw-r--r--   0        0        0     2058 2023-06-08 06:35:01.982074 bl_hector-0.1.0a4/bl_hector/infrastructure/typer/__init__.py
+-rw-r--r--   0        0        0     2842 2023-06-12 06:39:33.413846 bl_hector-0.1.0a4/bl_hector/infrastructure/typer/books.py
+-rw-r--r--   0        0        0     1866 2023-06-08 06:35:01.982074 bl_hector-0.1.0a4/bl_hector/infrastructure/typer/services.py
+-rw-r--r--   0        0        0     1351 2023-06-12 06:39:33.413846 bl_hector-0.1.0a4/bl_hector/interfaces/__init__.py
+-rw-r--r--   0        0        0      761 2023-06-12 06:39:33.413846 bl_hector-0.1.0a4/bl_hector/interfaces/exceptions.py
+-rw-r--r--   0        0        0     3371 2023-06-12 06:39:33.413846 bl_hector-0.1.0a4/bl_hector/interfaces/from_dict.py
+-rw-r--r--   0        0        0     1609 2023-06-12 06:39:33.413846 bl_hector-0.1.0a4/bl_hector/interfaces/from_json.py
+-rw-r--r--   0        0        0     1435 2023-06-08 06:35:01.986074 bl_hector-0.1.0a4/bl_hector/interfaces/l10n/__init__.py
+-rw-r--r--   0        0        0     4049 2023-06-12 06:39:33.413846 bl_hector-0.1.0a4/bl_hector/interfaces/l10n/en-GB/main.ftl
+-rw-r--r--   0        0        0     4591 2023-06-12 06:39:33.413846 bl_hector-0.1.0a4/bl_hector/interfaces/l10n/fr-FR/main.ftl
+-rw-r--r--   0        0        0     1407 2023-06-08 06:35:01.986074 bl_hector-0.1.0a4/bl_hector/interfaces/to_http/__init__.py
+-rw-r--r--   0        0        0    14491 2023-06-12 06:39:33.413846 bl_hector-0.1.0a4/bl_hector/interfaces/to_http/as_html/__init__.py
+-rw-r--r--   0        0        0     1247 2023-06-12 06:39:33.413846 bl_hector-0.1.0a4/bl_hector/interfaces/to_http/as_html/templates/auth/login.pug
+-rw-r--r--   0        0        0     4098 2023-06-12 06:39:33.413846 bl_hector-0.1.0a4/bl_hector/interfaces/to_http/as_html/templates/books/add.pug
+-rw-r--r--   0        0        0     2014 2023-06-12 06:39:33.413846 bl_hector-0.1.0a4/bl_hector/interfaces/to_http/as_html/templates/books/display.pug
+-rw-r--r--   0        0        0     2048 2023-06-12 06:39:33.413846 bl_hector-0.1.0a4/bl_hector/interfaces/to_http/as_html/templates/books/mixins/render_isbn.pug
+-rw-r--r--   0        0        0     5577 2023-06-12 06:39:33.413846 bl_hector-0.1.0a4/bl_hector/interfaces/to_http/as_html/templates/books/search.pug
+-rw-r--r--   0        0        0     3391 2023-06-12 06:39:33.413846 bl_hector-0.1.0a4/bl_hector/interfaces/to_http/as_html/templates/books/update.pug
+-rw-r--r--   0        0        0      982 2023-06-12 06:39:33.413846 bl_hector-0.1.0a4/bl_hector/interfaces/to_http/as_html/templates/error.pug
+-rw-r--r--   0        0        0     2026 2023-06-12 06:39:33.413846 bl_hector-0.1.0a4/bl_hector/interfaces/to_http/as_html/templates/layout.pug
+-rw-r--r--   0        0        0     1122 2023-06-08 06:35:01.986074 bl_hector-0.1.0a4/bl_hector/interfaces/to_http/as_html/templates/mixins/flash.pug
+-rw-r--r--   0        0        0     4134 2023-06-12 06:39:33.413846 bl_hector-0.1.0a4/bl_hector/interfaces/to_http/as_html/templates/mixins/form.pug
+-rw-r--r--   0        0        0     1992 2023-06-12 06:39:33.413846 bl_hector-0.1.0a4/bl_hector/interfaces/to_http/as_html/templates/mixins/navbar.pug
+-rw-r--r--   0        0        0     2010 2023-06-08 06:35:01.986074 bl_hector-0.1.0a4/bl_hector/interfaces/to_http/as_html/templates/webauthn/login.pug
+-rw-r--r--   0        0        0     2045 2023-06-08 06:35:01.986074 bl_hector-0.1.0a4/bl_hector/interfaces/to_http/as_html/templates/webauthn/register.pug
+-rw-r--r--   0        0        0     1310 2023-06-08 06:35:01.986074 bl_hector-0.1.0a4/bl_hector/interfaces/to_http/as_json/__init__.py
+-rw-r--r--   0        0        0     1211 2023-06-08 06:35:01.986074 bl_hector-0.1.0a4/bl_hector/interfaces/to_terminal/__init__.py
+-rw-r--r--   0        0        0     1818 2023-06-08 13:41:47.687677 bl_hector-0.1.0a4/bl_hector/interfaces/to_terminal/as_json.py
+-rw-r--r--   0        0        0     4445 2023-06-12 06:39:33.413846 bl_hector-0.1.0a4/bl_hector/interfaces/to_terminal/as_text.py
+-rw-r--r--   0        0        0     1519 2023-06-08 06:35:01.986074 bl_hector-0.1.0a4/bl_hector/interfaces/utils.py
+-rw-r--r--   0        0        0     1407 2023-06-12 06:54:40.105308 bl_hector-0.1.0a4/pyproject.toml
+-rw-r--r--   0        0        0     3829 2023-06-12 06:55:23.850654 bl_hector-0.1.0a4/setup.py
+-rw-r--r--   0        0        0     2216 2023-06-12 06:55:23.850896 bl_hector-0.1.0a4/PKG-INFO
```

### Comparing `bl_hector-0.1.0a3/LICENSE` & `bl_hector-0.1.0a4/LICENSE`

 * *Files identical despite different names*

### Comparing `bl_hector-0.1.0a3/README.md` & `bl_hector-0.1.0a4/README.md`

 * *Files identical despite different names*

### Comparing `bl_hector-0.1.0a3/bl_hector/__init__.py` & `bl_hector-0.1.0a4/bl_hector/__init__.py`

 * *Files identical despite different names*

### Comparing `bl_hector-0.1.0a3/bl_hector/application/__init__.py` & `bl_hector-0.1.0a4/bl_hector/application/__init__.py`

 * *Files identical despite different names*

### Comparing `bl_hector-0.1.0a3/bl_hector/application/use_cases/__init__.py` & `bl_hector-0.1.0a4/bl_hector/application/use_cases/__init__.py`

 * *Files identical despite different names*

### Comparing `bl_hector-0.1.0a3/bl_hector/application/use_cases/add_book.py` & `bl_hector-0.1.0a4/bl_hector/interfaces/to_terminal/as_json.py`

 * *Files 21% similar despite different names*

```diff
@@ -10,70 +10,41 @@
 # but WITHOUT ANY WARRANTY; without even the implied warranty of
 # MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the
 # GNU Affero General Public License for more details.
 #
 # You should have received a copy of the GNU Affero General Public License
 # along with this program. If not, see <http://www.gnu.org/licenses/>.
 
-from abc import ABC, abstractmethod
-from dataclasses import dataclass
+import json
+from typing import Callable
 
 from bl_hector.domain.collection_management.entities import Book
-from bl_hector.domain.collection_management.exceptions import IncorrectValue
-from bl_hector.domain.collection_management.repositories import Books
-from bl_hector.domain.collection_management.value_objects import (
-    Author,
-    Cover,
-    Genre,
-    Isbn,
-    Title,
-    Year,
-)
-
-
-@dataclass(frozen=True)
-class Request:
-    isbn: str
-    title: str
-    year: int
-    authors: list[str]
-    genres: list[str]
-    cover: str = ""
-
-
-class Presenter(ABC):
-    @abstractmethod
-    def bad_request(self) -> None:
-        ...
-
-    @abstractmethod
-    def book_already_exists(self, book: Book) -> None:
-        ...
-
-    @abstractmethod
-    def book_added(self, book: Book) -> None:
-        ...
-
-
-@dataclass(frozen=True)
-class Interactor:
-    presenter: Presenter
-    books: Books
-
-    def execute(self, request: Request) -> None:
-        try:
-            book = Book.instanciate(
-                Isbn.instanciate(request.isbn),
-                Title.instanciate(request.title),
-                Year.instanciate(request.year),
-                [Author.instanciate(a) for a in request.authors if a],
-                [Genre.instanciate(g) for g in request.genres if g],
-                Cover.instanciate(request.cover) if request.cover else None,
-            )
-        except IncorrectValue:
-            return self.presenter.bad_request()
+from bl_hector.domain.collection_management.value_objects import Isbn
+from bl_hector.interfaces.to_terminal import ExitCodes, LookUpBookInterface
 
-        if books := self.books.search(isbn=book.isbn):
-            return self.presenter.book_already_exists(books[0])
 
-        self.books.add(book)
-        self.presenter.book_added(book)
+class LookUpBook(LookUpBookInterface):
+    def __init__(self, printer: Callable[[str], None]) -> None:
+        self.__printer = printer
+        self.__exit_code = ExitCodes.USAGE
+
+    def not_an_isbn(self, isbn: str) -> None:
+        self.__exit_code = ExitCodes.BAD_REQUEST
+
+    def book_not_found(self, isbn: Isbn) -> None:
+        self.__exit_code = ExitCodes.NOT_FOUND
+
+    def book(self, book: Book) -> None:
+        self.__exit_code = ExitCodes.OK
+        data = {
+            "isbn": str(book.isbn),
+            "title": str(book.title),
+            "year": int(book.year),
+            "authors": [str(b) for b in book.authors],
+        }
+        if book.genres:
+            data["genres"] = [str(g) for g in book.genres]
+
+        self.__printer(json.dumps(data))
+
+    def exit_code(self) -> int:
+        return self.__exit_code.value
```

### Comparing `bl_hector-0.1.0a3/bl_hector/application/use_cases/display_book.py` & `bl_hector-0.1.0a4/bl_hector/application/use_cases/display_book.py`

 * *Files identical despite different names*

### Comparing `bl_hector-0.1.0a3/bl_hector/application/use_cases/import_books.py` & `bl_hector-0.1.0a4/bl_hector/application/use_cases/import_books.py`

 * *Files identical despite different names*

### Comparing `bl_hector-0.1.0a3/bl_hector/application/use_cases/look_up_book.py` & `bl_hector-0.1.0a4/bl_hector/application/use_cases/look_up_book.py`

 * *Files identical despite different names*

### Comparing `bl_hector-0.1.0a3/bl_hector/application/use_cases/update_book.py` & `bl_hector-0.1.0a4/bl_hector/application/use_cases/update_book.py`

 * *Files 25% similar despite different names*

```diff
@@ -11,16 +11,21 @@
 # MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the
 # GNU Affero General Public License for more details.
 #
 # You should have received a copy of the GNU Affero General Public License
 # along with this program. If not, see <http://www.gnu.org/licenses/>.
 
 from abc import ABC, abstractmethod
-from dataclasses import dataclass
+from dataclasses import dataclass, fields
+from typing import Optional
 
+from bl_hector.domain.administration.enumerations import Permissions as P
+from bl_hector.domain.administration.repositories import Permissions
+from bl_hector.domain.administration.value_objects import UserId
+from bl_hector.domain.collection_management import validators
 from bl_hector.domain.collection_management.entities import Book
 from bl_hector.domain.collection_management.exceptions import IncorrectValue
 from bl_hector.domain.collection_management.repositories import Books
 from bl_hector.domain.collection_management.value_objects import (
     Author,
     Cover,
     Genre,
@@ -28,25 +33,40 @@
     Title,
     Year,
 )
 
 
 @dataclass(frozen=True)
 class Request:
+    user_id: str
     isbn: str
     title: str
     year: int
     authors: list[str]
     genres: list[str]
     cover: str = ""
 
 
+@dataclass
+class Errors:
+    title: Optional[IncorrectValue] = None
+    year: Optional[IncorrectValue] = None
+    authors: Optional[IncorrectValue] = None
+
+    def __bool__(self) -> bool:
+        return any([getattr(self, f.name) for f in fields(self)])
+
+
 class Presenter(ABC):
     @abstractmethod
-    def bad_request(self) -> None:
+    def not_authorized(self) -> None:
+        ...
+
+    @abstractmethod
+    def bad_request(self, errors: Errors) -> None:
         ...
 
     @abstractmethod
     def book_not_found(self, isbn: Isbn) -> None:
         ...
 
     @abstractmethod
@@ -54,27 +74,41 @@
         ...
 
 
 @dataclass(frozen=True)
 class Interactor:
     presenter: Presenter
     books: Books
+    permissions: Permissions
 
     def execute(self, request: Request) -> None:
-        try:
-            # There's no business logic to apply when updating a book.
-            book = Book.instanciate(
-                Isbn.instanciate(request.isbn),
-                Title.instanciate(request.title),
-                Year.instanciate(request.year),
-                [Author.instanciate(a) for a in request.authors if a],
-                [Genre.instanciate(g) for g in request.genres if g],
-                Cover.instanciate(request.cover) if request.cover else None,
-            )
-        except IncorrectValue:
-            return self.presenter.bad_request()
+        if not self.__is_authorized(request.user_id):
+            return self.presenter.not_authorized()
+
+        if errors := self.__validate_request(request):
+            return self.presenter.bad_request(errors)
+
+        # There's no business logic to apply when updating a book.
+        book = Book.instanciate(
+            Isbn.instanciate(request.isbn),
+            Title.instanciate(request.title),
+            Year.instanciate(request.year),
+            [Author.instanciate(a) for a in request.authors if a],
+            [Genre.instanciate(g) for g in request.genres if g],
+            Cover.instanciate(request.cover) if request.cover else None,
+        )
 
         if not self.books.search(isbn=book.isbn):
             return self.presenter.book_not_found(book.isbn)
 
         self.books.update(book)
         self.presenter.book_updated(book)
+
+    def __is_authorized(self, user_id: str) -> bool:
+        return self.permissions.is_authorized_to(UserId(user_id), P.UPDATE_BOOK)
+
+    def __validate_request(self, request: Request) -> Errors:
+        return Errors(
+            title=validators.title(request.title),
+            year=validators.year(request.year),
+            authors=validators.authors(request.authors),
+        )
```

### Comparing `bl_hector-0.1.0a3/bl_hector/configuration/__init__.py` & `bl_hector-0.1.0a4/bl_hector/configuration/__init__.py`

 * *Files identical despite different names*

### Comparing `bl_hector-0.1.0a3/bl_hector/configuration/cli.py` & `bl_hector-0.1.0a4/bl_hector/configuration/cli.py`

 * *Files identical despite different names*

### Comparing `bl_hector-0.1.0a3/bl_hector/configuration/wsgi.py` & `bl_hector-0.1.0a4/bl_hector/configuration/wsgi.py`

 * *Files identical despite different names*

### Comparing `bl_hector-0.1.0a3/bl_hector/domain/__init__.py` & `bl_hector-0.1.0a4/bl_hector/domain/__init__.py`

 * *Files identical despite different names*

### Comparing `bl_hector-0.1.0a3/bl_hector/domain/administration/__init__.py` & `bl_hector-0.1.0a4/bl_hector/domain/administration/__init__.py`

 * *Files identical despite different names*

### Comparing `bl_hector-0.1.0a3/bl_hector/domain/administration/entities.py` & `bl_hector-0.1.0a4/bl_hector/domain/administration/entities.py`

 * *Files identical despite different names*

### Comparing `bl_hector-0.1.0a3/bl_hector/domain/administration/repositories.py` & `bl_hector-0.1.0a4/bl_hector/domain/administration/repositories.py`

 * *Files 11% similar despite different names*

```diff
@@ -15,14 +15,16 @@
 # along with this program. If not, see <http://www.gnu.org/licenses/>.
 
 import datetime
 from abc import ABC, abstractmethod
 from typing import Optional
 
 from .entities import Challenge, Credential, User
+from .enumerations import Permissions as P
+from .value_objects import UserId
 
 
 class Users(ABC):
     @abstractmethod
     def by_login(self, login: str) -> Optional[User]:
         ...
 
@@ -45,7 +47,13 @@
     @abstractmethod
     def valid_for(self, user: User, now: datetime.datetime) -> Optional[Challenge]:
         ...
 
     @abstractmethod
     def add(self, challenge: Challenge) -> None:
         ...
+
+
+class Permissions(ABC):
+    @abstractmethod
+    def is_authorized_to(self, user_id: UserId, permission: P) -> bool:
+        ...
```

### Comparing `bl_hector-0.1.0a3/bl_hector/domain/administration/services.py` & `bl_hector-0.1.0a4/bl_hector/domain/administration/services.py`

 * *Files identical despite different names*

### Comparing `bl_hector-0.1.0a3/bl_hector/domain/administration/value_objects.py` & `bl_hector-0.1.0a4/bl_hector/domain/administration/value_objects.py`

 * *Files identical despite different names*

### Comparing `bl_hector-0.1.0a3/bl_hector/domain/collection_management/__init__.py` & `bl_hector-0.1.0a4/bl_hector/domain/collection_management/__init__.py`

 * *Files identical despite different names*

### Comparing `bl_hector-0.1.0a3/bl_hector/domain/collection_management/entities.py` & `bl_hector-0.1.0a4/bl_hector/domain/collection_management/entities.py`

 * *Files identical despite different names*

### Comparing `bl_hector-0.1.0a3/bl_hector/domain/collection_management/exceptions.py` & `bl_hector-0.1.0a4/bl_hector/domain/collection_management/exceptions.py`

 * *Files identical despite different names*

### Comparing `bl_hector-0.1.0a3/bl_hector/domain/collection_management/repositories.py` & `bl_hector-0.1.0a4/bl_hector/domain/collection_management/repositories.py`

 * *Files identical despite different names*

### Comparing `bl_hector-0.1.0a3/bl_hector/domain/collection_management/services.py` & `bl_hector-0.1.0a4/bl_hector/domain/collection_management/services.py`

 * *Files identical despite different names*

### Comparing `bl_hector-0.1.0a3/bl_hector/domain/collection_management/value_objects.py` & `bl_hector-0.1.0a4/bl_hector/domain/collection_management/value_objects.py`

 * *Files identical despite different names*

### Comparing `bl_hector-0.1.0a3/bl_hector/infrastructure/__init__.py` & `bl_hector-0.1.0a4/bl_hector/infrastructure/sqlalchemy/__init__.py`

 * *Files identical despite different names*

### Comparing `bl_hector-0.1.0a3/bl_hector/infrastructure/flask/__init__.py` & `bl_hector-0.1.0a4/bl_hector/infrastructure/flask/__init__.py`

 * *Files 11% similar despite different names*

```diff
@@ -10,60 +10,82 @@
 # but WITHOUT ANY WARRANTY; without even the implied warranty of
 # MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the
 # GNU Affero General Public License for more details.
 #
 # You should have received a copy of the GNU Affero General Public License
 # along with this program. If not, see <http://www.gnu.org/licenses/>.
 
+from http import HTTPStatus as HTTP
+from typing import Any
+
 from flask import Flask, g, get_flashed_messages, request, url_for
 from werkzeug.middleware.proxy_fix import ProxyFix
 
 from bl_hector import __version__
 from bl_hector.infrastructure.flask import services
 from bl_hector.infrastructure.flask.aliases import blueprint as aliases
 from bl_hector.infrastructure.flask.auth import blueprint as auth
 from bl_hector.infrastructure.flask.books import blueprint as books
+from bl_hector.infrastructure.flask.utils import presenter_to_response
 from bl_hector.infrastructure.settings import WsgiSettings
-from bl_hector.interfaces import l10n
+from bl_hector.interfaces import exceptions, l10n
+from bl_hector.interfaces.to_http.as_html import JinjaPresenter
 
 
 def build_app(settings: WsgiSettings) -> Flask:
     services.define_settings(settings)
 
     app = Flask(__name__)
 
-    # FIXME make it configurable?!
-    app.wsgi_app = ProxyFix(app.wsgi_app, x_host=1)  # type: ignore
+    if settings.PROXIED:
+        app.wsgi_app = ProxyFix(  # type: ignore[method-assign]
+            app.wsgi_app, x_for=1, x_proto=1, x_host=1, x_prefix=1
+        )
 
     app.config.update(
         SECRET_KEY=settings.SECRET_KEY,
     )
 
     register_blueprints(app, settings)
     register_jinja_globals()
 
-    app.teardown_appcontext(services.close_connection)
+    app.teardown_appcontext(services.teardown_connection)
 
     @app.before_request
     def guess_locale() -> None:
         g.locale = (
             request.accept_languages.best_match(l10n.LOCALES) or l10n.DEFAULT_LOCALE
         )
 
+    @app.errorhandler(exceptions.BadRequest)  # type: ignore[type-var]
+    @presenter_to_response
+    def handle_bad_request(e: Exception) -> Any:
+        presenter = JinjaPresenter(
+            "error",
+            message="You submitted a bad request! This should have never happened!?",
+        )
+        presenter.set_status_code(HTTP.BAD_REQUEST)
+        return presenter
+
     return app
 
 
 def register_blueprints(app: Flask, settings: WsgiSettings) -> None:
     app.register_blueprint(aliases, url_prefix="/")
-    app.register_blueprint(auth, url_prefix="/auth")
     app.register_blueprint(books, url_prefix="/books")
+
+    app.register_blueprint(auth, url_prefix="/auth")
+    app.auth_links = []  # type: ignore[attr-defined]
     if settings.WEBAUTHN:
         from bl_hector.infrastructure.flask.webauthn import blueprint as webauthn
 
         app.register_blueprint(webauthn, url_prefix="/auth/webauthn")
+        app.auth_links.append(  # type: ignore[attr-defined]
+            {"route": "webauthn.login", "label": "WebAuthn", "icon": "key"}
+        )
 
 
 def register_jinja_globals() -> None:
     from bl_hector.interfaces.to_http import as_html as presenters
 
     presenters.register_jinja_global("version", __version__)
     presenters.register_jinja_global("url_for", url_for)
```

### Comparing `bl_hector-0.1.0a3/bl_hector/infrastructure/flask/aliases/__init__.py` & `bl_hector-0.1.0a4/bl_hector/infrastructure/flask/aliases/__init__.py`

 * *Files identical despite different names*

### Comparing `bl_hector-0.1.0a3/bl_hector/infrastructure/flask/auth/__init__.py` & `bl_hector-0.1.0a4/bl_hector/infrastructure/flask/auth/__init__.py`

 * *Files 8% similar despite different names*

```diff
@@ -12,15 +12,15 @@
 # GNU Affero General Public License for more details.
 #
 # You should have received a copy of the GNU Affero General Public License
 # along with this program. If not, see <http://www.gnu.org/licenses/>.
 
 from typing import Any
 
-from flask import Blueprint, session, url_for
+from flask import Blueprint, current_app, session, url_for
 
 from bl_hector.infrastructure.flask import services
 from bl_hector.infrastructure.flask.utils import presenter_to_response
 from bl_hector.interfaces.to_http import Redirection, as_html
 
 blueprint = Blueprint("auth", __name__)
 
@@ -30,25 +30,22 @@
 def root() -> Any:
     return Redirection(url_for("books.search"))
 
 
 @blueprint.get("/login")
 @presenter_to_response
 def login() -> Any:
-    links = []
-    if services.settings().WEBAUTHN:
-        links.append(
-            {"url": url_for("webauthn.login"), "label": "WebAuthn", "icon": "key"}
-        )
-
-    if not links:
+    auth_links = current_app.auth_links  # type: ignore[attr-defined]
+    if not auth_links:
         return Redirection(url_for("aliases.root"))
-    if len(links) == 1:
-        return Redirection(links[0]["url"])
-    return as_html.JinjaPresenter("auth/login", links=links, user=services.get_user())
+    if len(auth_links) == 1:
+        return Redirection(url_for(auth_links[0]["route"]))
+    return as_html.JinjaPresenter(
+        "auth/login", links=auth_links, user=services.get_user()
+    )
 
 
 @blueprint.get("/logout")
 @presenter_to_response
 def logout() -> Any:
     session.clear()
     return Redirection(url_for("aliases.root"))
```

### Comparing `bl_hector-0.1.0a3/bl_hector/infrastructure/flask/books/__init__.py` & `bl_hector-0.1.0a4/bl_hector/infrastructure/flask/books/__init__.py`

 * *Files 10% similar despite different names*

```diff
@@ -22,18 +22,15 @@
     add_book,
     display_book,
     look_up_book,
     search_books,
     update_book,
 )
 from bl_hector.infrastructure.flask import services
-from bl_hector.infrastructure.flask.utils import (
-    permission_required,
-    presenter_to_response,
-)
+from bl_hector.infrastructure.flask.utils import presenter_to_response
 from bl_hector.interfaces import from_dict as controllers
 from bl_hector.interfaces.to_http import as_html as presenters
 
 blueprint = Blueprint("books", __name__)
 
 
 def notify(message: str, type: str) -> None:
@@ -53,31 +50,28 @@
     controller = controllers.SearchBooks(
         request.args, page_size=presenters.SearchBooks.PAGE_SIZE
     )
     controller.call(interactor)
     return presenter
 
 
-@blueprint.post("@isbn")
+@blueprint.get("__new__")
 @presenter_to_response
-def validate_isbn() -> Any:
-    return presenters.ValidateIsbn(request.form, user=services.get_user())
+def add() -> Any:
+    return presenters.AddBook(request.form, user=services.get_user())
 
 
-@blueprint.route("__new__", methods=["GET", "POST"])
-@permission_required("add-book")  # type: ignore[misc]
+@blueprint.post("__new__")
 @presenter_to_response
-def add() -> Any:
-    presenter = presenters.AddBook(
-        request.form,
-        notify=notify,
-        user=services.get_user(),
+def add_POST() -> Any:
+    presenter = presenters.AddBook(request.form, notify=notify, user=services.get_user())
+    interactor = add_book.Interactor(
+        presenter, services.get_books(), services.get_permissions()
     )
-    interactor = add_book.Interactor(presenter, services.get_books())
-    controller = controllers.AddBook(request.form)
+    controller = controllers.AddBook(request.form, str(services.get_user().id))
     controller.call(interactor)
     return presenter
 
 
 @blueprint.post("__info__")
 @presenter_to_response
 def look_up() -> Any:
@@ -93,29 +87,35 @@
     presenter = presenters.DisplayBook(notify=notify, user=services.get_user())
     interactor = display_book.Interactor(presenter, services.get_books())
     interactor.execute(display_book.Request(isbn))
     return presenter
 
 
 @blueprint.get("<string:isbn>/__edit__")
-@permission_required("update-book")  # type: ignore[misc]
 @presenter_to_response
 def update(isbn: str) -> Any:
     presenter = presenters.DisplayBookToUpdate(
         isbn, notify=notify, user=services.get_user()
     )
     interactor = display_book.Interactor(presenter, services.get_books())
     interactor.execute(display_book.Request(isbn))
     return presenter
 
 
 @blueprint.post("<string:isbn>/__edit__")
-@permission_required("update-book")  # type: ignore[misc]
 @presenter_to_response
 def update_POST(isbn: str) -> Any:
     presenter = presenters.UpdateBook(
         isbn, request.form, notify=notify, user=services.get_user()
     )
-    interactor = update_book.Interactor(presenter, services.get_books())
-    controller = controllers.UpdateBook(isbn, request.form)
+    interactor = update_book.Interactor(
+        presenter, services.get_books(), services.get_permissions()
+    )
+    controller = controllers.UpdateBook(isbn, request.form, str(services.get_user().id))
     controller.call(interactor)
     return presenter
+
+
+@blueprint.post("@isbn")
+@presenter_to_response
+def validate_isbn() -> Any:
+    return presenters.ValidateIsbn(request.form, user=services.get_user())
```

### Comparing `bl_hector-0.1.0a3/bl_hector/infrastructure/flask/services.py` & `bl_hector-0.1.0a4/bl_hector/infrastructure/flask/services.py`

 * *Files 9% similar despite different names*

```diff
@@ -18,14 +18,16 @@
 from urllib.parse import urlparse
 
 from flask import g, request, session
 from sqlalchemy import create_engine
 from sqlalchemy.engine import Connection
 
 from bl_hector.domain.administration.entities import RelyingParty
+from bl_hector.domain.administration.repositories import Permissions
+from bl_hector.infrastructure import FakePermissions
 from bl_hector.infrastructure.isbnlib import InfoProvider
 from bl_hector.infrastructure.settings import WsgiSettings
 from bl_hector.infrastructure.sqlalchemy.repositories import (
     Books,
     Challenges,
     Credentials,
     Users,
@@ -36,57 +38,61 @@
 
 
 def define_settings(settings: WsgiSettings) -> None:
     global __SETTINGS
     __SETTINGS = settings
 
 
-def settings() -> WsgiSettings:
+def get_settings() -> WsgiSettings:
     if not __SETTINGS:
         raise RuntimeError("You must define the settings!")
     return __SETTINGS
 
 
-def connection() -> Connection:
-    s = settings()
+def get_connection() -> Connection:
+    s = get_settings()
     if "connection" not in g:
         options: dict[str, Any] = {}
         if s.DEBUG_SQL:
             options["echo"] = True
             options["echo_pool"] = "debug"
 
         engine = create_engine(s.DSN, **options)
         g.setdefault("connection", engine.connect())
 
     return g.connection  # type: ignore[no-any-return]
 
 
-def close_connection(exception: Optional[BaseException]) -> None:
+def teardown_connection(exception: Optional[BaseException]) -> None:
     if connection := g.pop("connection", None):
         if exception:
             connection.rollback()
         else:
             connection.commit()
         connection.close()
 
 
 def get_books() -> Books:
-    return Books(connection())
+    return Books(get_connection())
 
 
 def get_users() -> Users:
-    return Users(connection())
+    return Users(get_connection())
 
 
 def get_credentials() -> Credentials:
-    return Credentials(connection())
+    return Credentials(get_connection())
 
 
 def get_challenges() -> Challenges:
-    return Challenges(connection())
+    return Challenges(get_connection())
+
+
+def get_permissions() -> Permissions:
+    return FakePermissions()
 
 
 def get_info_provider() -> InfoProvider:
     return InfoProvider()
 
 
 def get_user() -> User:
```

### Comparing `bl_hector-0.1.0a3/bl_hector/infrastructure/flask/static/css/bulma@0.9.4.min.css` & `bl_hector-0.1.0a4/bl_hector/infrastructure/flask/static/css/bulma@0.9.4.min.css`

 * *Files identical despite different names*

### Comparing `bl_hector-0.1.0a3/bl_hector/infrastructure/flask/static/css/font-awesome@5.14.0.css` & `bl_hector-0.1.0a4/bl_hector/infrastructure/flask/static/css/font-awesome@5.14.0.css`

 * *Files identical despite different names*

### Comparing `bl_hector-0.1.0a3/bl_hector/infrastructure/flask/static/favicon.svg` & `bl_hector-0.1.0a4/bl_hector/infrastructure/flask/static/favicon.svg`

 * *Files identical despite different names*

### Comparing `bl_hector-0.1.0a3/bl_hector/infrastructure/flask/static/img/placeholders/1280x960.png` & `bl_hector-0.1.0a4/bl_hector/infrastructure/flask/static/img/placeholders/1280x960.png`

 * *Files identical despite different names*

### Comparing `bl_hector-0.1.0a3/bl_hector/infrastructure/flask/static/img/placeholders/320x480.png` & `bl_hector-0.1.0a4/bl_hector/infrastructure/flask/static/img/placeholders/320x480.png`

 * *Files identical despite different names*

### Comparing `bl_hector-0.1.0a3/bl_hector/infrastructure/flask/static/img/placeholders/96x96.png` & `bl_hector-0.1.0a4/bl_hector/infrastructure/flask/static/img/placeholders/96x96.png`

 * *Files identical despite different names*

### Comparing `bl_hector-0.1.0a3/bl_hector/infrastructure/flask/static/js/htmx@1.9.2.min.js` & `bl_hector-0.1.0a4/bl_hector/infrastructure/flask/static/js/htmx@1.9.2.min.js`

 * *Files identical despite different names*

### Comparing `bl_hector-0.1.0a3/bl_hector/infrastructure/flask/static/js/hyperscript@0.9.8.min.js` & `bl_hector-0.1.0a4/bl_hector/infrastructure/flask/static/js/hyperscript@0.9.8.min.js`

 * *Files identical despite different names*

### Comparing `bl_hector-0.1.0a3/bl_hector/infrastructure/flask/static/js/simplewebauthn-browser@7.2.0.umd.min.js` & `bl_hector-0.1.0a4/bl_hector/infrastructure/flask/static/js/simplewebauthn-browser@7.2.0.umd.min.js`

 * *Files identical despite different names*

### Comparing `bl_hector-0.1.0a3/bl_hector/infrastructure/flask/static/webfonts/fa-brands-400.ttf` & `bl_hector-0.1.0a4/bl_hector/infrastructure/flask/static/webfonts/fa-brands-400.ttf`

 * *Files identical despite different names*

### Comparing `bl_hector-0.1.0a3/bl_hector/infrastructure/flask/static/webfonts/fa-brands-400.woff2` & `bl_hector-0.1.0a4/bl_hector/infrastructure/flask/static/webfonts/fa-brands-400.woff2`

 * *Files identical despite different names*

### Comparing `bl_hector-0.1.0a3/bl_hector/infrastructure/flask/static/webfonts/fa-regular-400.ttf` & `bl_hector-0.1.0a4/bl_hector/infrastructure/flask/static/webfonts/fa-regular-400.ttf`

 * *Files identical despite different names*

### Comparing `bl_hector-0.1.0a3/bl_hector/infrastructure/flask/static/webfonts/fa-regular-400.woff2` & `bl_hector-0.1.0a4/bl_hector/infrastructure/flask/static/webfonts/fa-regular-400.woff2`

 * *Files identical despite different names*

### Comparing `bl_hector-0.1.0a3/bl_hector/infrastructure/flask/static/webfonts/fa-solid-900.ttf` & `bl_hector-0.1.0a4/bl_hector/infrastructure/flask/static/webfonts/fa-solid-900.ttf`

 * *Files identical despite different names*

### Comparing `bl_hector-0.1.0a3/bl_hector/infrastructure/flask/static/webfonts/fa-solid-900.woff2` & `bl_hector-0.1.0a4/bl_hector/infrastructure/flask/static/webfonts/fa-solid-900.woff2`

 * *Files identical despite different names*

### Comparing `bl_hector-0.1.0a3/bl_hector/infrastructure/flask/utils.py` & `bl_hector-0.1.0a4/bl_hector/infrastructure/flask/utils.py`

 * *Files 14% similar despite different names*

```diff
@@ -11,18 +11,17 @@
 # MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the
 # GNU Affero General Public License for more details.
 #
 # You should have received a copy of the GNU Affero General Public License
 # along with this program. If not, see <http://www.gnu.org/licenses/>.
 
 from functools import wraps
-from http import HTTPStatus as HTTP
 from typing import Any, Callable
 
-from flask import Response, session
+from flask import Response
 
 from bl_hector.interfaces.to_http import HttpPresenter
 
 
 def presenter_to_response(f: Callable[..., HttpPresenter]) -> Callable[[], Response]:
     @wraps(f)
     def decorated_function(*args: Any, **kwargs: Any) -> Response:
@@ -30,22 +29,7 @@
         return Response(
             status=presenter.status_code(),
             headers=presenter.headers(),
             response=presenter.data(),
         )
 
     return decorated_function
-
-
-# FIXME improve typing
-def permission_required(permission: str) -> Any:
-    def wrapper(f: Any) -> Callable[[], Response]:
-        @wraps(f)
-        def decorated_function(*args: Any, **kwargs: Any) -> Response:
-            # TODO improve permission verification
-            if not session.get("user_id", ""):
-                return Response(status=HTTP.FORBIDDEN)
-            return f(*args, **kwargs)  # type: ignore [no-any-return]
-
-        return decorated_function
-
-    return wrapper
```

### Comparing `bl_hector-0.1.0a3/bl_hector/infrastructure/flask/webauthn/__init__.py` & `bl_hector-0.1.0a4/bl_hector/infrastructure/flask/webauthn/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -20,24 +20,23 @@
 from uuid import uuid4
 
 from flask import Blueprint, request, session, url_for
 
 from bl_hector.domain.administration.entities import User
 from bl_hector.domain.administration.services import create_challenge_for
 from bl_hector.domain.administration.value_objects import UserId
+from bl_hector.infrastructure import ONLY_USER
 from bl_hector.infrastructure.flask import services
 from bl_hector.infrastructure.flask.utils import presenter_to_response
 from bl_hector.interfaces.to_http import Redirection, as_html, as_json
 
 from . import security
 
 blueprint = Blueprint("webauthn", __name__)
 
-ONLY_USER = "admin"
-
 
 @blueprint.get("/login")
 @presenter_to_response
 def login() -> Any:
     # For the time being, Hector only has one user with one credential
     if not (user := services.get_users().by_login(ONLY_USER)):
         return Redirection(url_for("webauthn.register"))
@@ -53,14 +52,39 @@
         user=services.get_user(),
         options=security.authentication_options(
             services.get_relying_party(), user, credentials, challenge
         ),
     )
 
 
+@blueprint.post("/verify-credential")
+@presenter_to_response
+def verify_credential() -> Any:
+    if not (user := services.get_users().by_login(ONLY_USER)):
+        return as_json.Dict({"verified": False}, status_code=HTTP.BAD_REQUEST)
+
+    if not (challenge := services.get_challenges().valid_for(user, dt.now())):
+        return as_json.Dict({"verified": False}, status_code=HTTP.BAD_REQUEST)
+
+    if not (credentials := services.get_credentials().for_user(user)):
+        return as_json.Dict({"verified": False}, status_code=HTTP.BAD_REQUEST)
+
+    if not security.verify_credentials(
+        request.get_data(),
+        challenge,
+        services.get_relying_party(),
+        user,
+        credentials,
+    ):
+        return as_json.Dict({"verified": False}, status_code=HTTP.BAD_REQUEST)
+
+    session["user_id"] = user.id
+    return as_json.Dict({"verified": True}, status_code=HTTP.OK)
+
+
 @blueprint.get("/register")
 @presenter_to_response
 def register() -> Any:
     if not (user := services.get_users().by_login(ONLY_USER)):
         user = User(UserId(str(uuid4())), ONLY_USER, "The only user")
         services.get_users().add(user)
 
@@ -84,45 +108,22 @@
 def add_credential() -> Any:
     if not (user := services.get_users().by_login(ONLY_USER)):
         return as_json.Dict({"verified": False}, status_code=HTTP.BAD_REQUEST)
 
     if not (challenge := services.get_challenges().valid_for(user, dt.now())):
         return as_json.Dict({"verified": False}, status_code=HTTP.BAD_REQUEST)
 
-    services.get_credentials().add(
-        security.parse_credentials(
+    if not (
+        credential := security.parse_credentials(
             request.get_data(), challenge, services.get_relying_party(), user
         )
-    )
-
-    return as_json.Dict({"verified": True}, status_code=HTTP.CREATED)
-
-
-@blueprint.post("/verify-credential")
-@presenter_to_response
-def verify_credential() -> Any:
-    if not (user := services.get_users().by_login(ONLY_USER)):
-        return as_json.Dict({"verified": False}, status_code=HTTP.BAD_REQUEST)
-
-    if not (challenge := services.get_challenges().valid_for(user, dt.now())):
-        return as_json.Dict({"verified": False}, status_code=HTTP.BAD_REQUEST)
-
-    if not (credentials := services.get_credentials().for_user(user)):
-        return as_json.Dict({"verified": False}, status_code=HTTP.BAD_REQUEST)
-
-    if not security.verify_credentials(
-        request.get_data(),
-        challenge,
-        services.get_relying_party(),
-        user,
-        credentials,
     ):
         return as_json.Dict({"verified": False}, status_code=HTTP.BAD_REQUEST)
 
-    session["user_id"] = user.id
-    return as_json.Dict({"verified": True}, status_code=HTTP.OK)
+    services.get_credentials().add(credential)
+    return as_json.Dict({"verified": True}, status_code=HTTP.CREATED)
 
 
 @blueprint.get("/logout")
 @presenter_to_response
 def logout() -> Any:
     return Redirection(url_for("auth.logout"))
```

### Comparing `bl_hector-0.1.0a3/bl_hector/infrastructure/flask/webauthn/security.py` & `bl_hector-0.1.0a4/bl_hector/infrastructure/flask/webauthn/security.py`

 * *Files 23% similar despite different names*

```diff
@@ -11,14 +11,15 @@
 # MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the
 # GNU Affero General Public License for more details.
 #
 # You should have received a copy of the GNU Affero General Public License
 # along with this program. If not, see <http://www.gnu.org/licenses/>.
 
 import logging
+from typing import Optional
 
 import webauthn
 from webauthn.helpers.structs import (
     AuthenticationCredential,
     PublicKeyCredentialDescriptor,
     RegistrationCredential,
 )
@@ -42,24 +43,28 @@
         challenge=bytes(challenge),
     )
     return webauthn.options_to_json(pcco)
 
 
 def parse_credentials(
     data: bytes, challenge: Challenge, rp: RelyingParty, user: User
-) -> Credential:
-    verification = webauthn.verify_registration_response(
-        credential=RegistrationCredential.parse_raw(data),
-        expected_challenge=bytes(challenge),
-        expected_origin=rp.origin,
-        expected_rp_id=rp.id,
-    )
-    return Credential(
-        verification.credential_id, verification.credential_public_key, user.id
-    )
+) -> Optional[Credential]:
+    try:
+        verification = webauthn.verify_registration_response(
+            credential=RegistrationCredential.parse_raw(data),
+            expected_challenge=bytes(challenge),
+            expected_origin=rp.origin,
+            expected_rp_id=rp.id,
+        )
+        return Credential(
+            verification.credential_id, verification.credential_public_key, user.id
+        )
+    except Exception as exc:
+        logging.exception(exc)
+        return None
 
 
 def authentication_options(
     rp: RelyingParty, user: User, credentials: list[Credential], challenge: Challenge
 ) -> str:
     allowed_credentials = [
         PublicKeyCredentialDescriptor(id=credential.id) for credential in credentials
```

### Comparing `bl_hector-0.1.0a3/bl_hector/infrastructure/isbnlib/__init__.py` & `bl_hector-0.1.0a4/bl_hector/infrastructure/isbnlib/__init__.py`

 * *Files identical despite different names*

### Comparing `bl_hector-0.1.0a3/bl_hector/infrastructure/settings.py` & `bl_hector-0.1.0a4/bl_hector/infrastructure/settings.py`

 * *Files 14% similar despite different names*

```diff
@@ -29,14 +29,19 @@
     """The data source name to access the database.
     See: <https://docs.sqlalchemy.org/en/20/core/engines.html#database-urls>."""
 
     DEBUG_SQL: bool = False
     """To enable SqlAlchemy logging.
     See: <https://docs.sqlalchemy.org/en/20/core/engines.html#configuring-logging>."""
 
+    PROXIED: bool = False
+    """To let Flask know that it runs behind a proxy.
+    See: <https://flask.palletsprojects.com/en/2.3.x/deploying/proxy_fix/>.
+    """
+
     WEBAUTHN: bool = False
     """To WebAuthn authentication.
     Extra dependencies must be installed: `bl-hector[webauthn]`.
     """
 
 
 @dataclass(frozen=True)
```

### Comparing `bl_hector-0.1.0a3/bl_hector/infrastructure/sqlalchemy/__init__.py` & `bl_hector-0.1.0a4/bl_hector/interfaces/exceptions.py`

 * *Files 8% similar despite different names*

```diff
@@ -9,7 +9,11 @@
 # This program is distributed in the hope that it will be useful,
 # but WITHOUT ANY WARRANTY; without even the implied warranty of
 # MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the
 # GNU Affero General Public License for more details.
 #
 # You should have received a copy of the GNU Affero General Public License
 # along with this program. If not, see <http://www.gnu.org/licenses/>.
+
+
+class BadRequest(Exception):
+    pass
```

### Comparing `bl_hector-0.1.0a3/bl_hector/infrastructure/sqlalchemy/repositories.py` & `bl_hector-0.1.0a4/bl_hector/infrastructure/sqlalchemy/repositories.py`

 * *Files identical despite different names*

### Comparing `bl_hector-0.1.0a3/bl_hector/infrastructure/typer/__init__.py` & `bl_hector-0.1.0a4/bl_hector/infrastructure/typer/__init__.py`

 * *Files identical despite different names*

### Comparing `bl_hector-0.1.0a3/bl_hector/infrastructure/typer/books.py` & `bl_hector-0.1.0a4/bl_hector/infrastructure/typer/books.py`

 * *Files 4% similar despite different names*

```diff
@@ -16,14 +16,15 @@
 
 import sys
 
 import typer
 from typing_extensions import Annotated
 
 from bl_hector.application.use_cases import add_book, import_books, look_up_book
+from bl_hector.infrastructure import ONLY_USER, FakePermissions
 from bl_hector.infrastructure.typer import services
 from bl_hector.interfaces import from_json as controllers
 from bl_hector.interfaces.to_terminal import LookUpBookInterface, as_json, as_text
 
 cmd = typer.Typer()
 
 
@@ -45,20 +46,21 @@
     interactor.execute(look_up_book.Request(isbn))
     raise typer.Exit(presenter.exit_code())
 
 
 @cmd.command()
 def add(ctx: typer.Context) -> None:
     """Add a book to the collection."""
+    permissions = FakePermissions()
     with services.get_books(ctx.obj) as books:
         presenter = as_text.AddBook(
             lambda m: typer.echo(m), translator=services.get_translator()
         )
-        interactor = add_book.Interactor(presenter, books)
-        controller = controllers.AddBook(sys.stdin.readline())
+        interactor = add_book.Interactor(presenter, books, permissions)
+        controller = controllers.AddBook(sys.stdin.readline(), ONLY_USER)
         controller.call(interactor)
         raise typer.Exit(presenter.exit_code())
 
 
 @cmd.command("import")
 def import_(ctx: typer.Context, path: str) -> None:
     """Import a list of books to the collection."""
```

### Comparing `bl_hector-0.1.0a3/bl_hector/infrastructure/typer/services.py` & `bl_hector-0.1.0a4/bl_hector/infrastructure/typer/services.py`

 * *Files identical despite different names*

### Comparing `bl_hector-0.1.0a3/bl_hector/interfaces/__init__.py` & `bl_hector-0.1.0a4/bl_hector/domain/administration/enumerations.py`

 * *Files 8% similar despite different names*

```diff
@@ -10,15 +10,10 @@
 # but WITHOUT ANY WARRANTY; without even the implied warranty of
 # MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the
 # GNU Affero General Public License for more details.
 #
 # You should have received a copy of the GNU Affero General Public License
 # along with this program. If not, see <http://www.gnu.org/licenses/>.
 
+from enum import Enum
 
-from dataclasses import dataclass
-
-
-@dataclass
-class User:
-    id: str
-    locale: str
+Permissions = Enum("Permissions", ["ADD_BOOK", "UPDATE_BOOK"])
```

### Comparing `bl_hector-0.1.0a3/bl_hector/interfaces/from_dict.py` & `bl_hector-0.1.0a4/bl_hector/interfaces/from_dict.py`

 * *Files 19% similar despite different names*

```diff
@@ -15,88 +15,76 @@
 # along with this program. If not, see <http://www.gnu.org/licenses/>.
 
 from typing import Any, Optional
 
 from werkzeug.datastructures import MultiDict
 
 from bl_hector.application.use_cases import add_book, search_books, update_book
-from bl_hector.interfaces import validators
+from bl_hector.interfaces.exceptions import BadRequest
 
 
 class SearchBooks:
     def __init__(
         self, data: MultiDict[str, Any], /, *, page_size: Optional[int] = None
     ) -> None:
-        self.__data = data
-        self.__page_size = page_size
+        self.__do_search = bool(data)
+        self.request = search_books.Request(
+            isbn=str(v) if (v := data.get("isbn")) else None,
+            title=str(v) if (v := data.get("title")) else None,
+            year=int(v) if (v := data.get("year")) else None,
+            author=str(v) if (v := data.get("author")) else None,
+            genre=str(v) if (v := data.get("genre")) else None,
+            page_number=int(v) if (v := data.get("page")) else 1,
+            page_size=page_size,
+        )
 
     def call(self, interactor: search_books.Interactor) -> None:
-        if not self.__data:
-            return
-
-        validator = validators.SearchBooks(self.__data)
-        if not validator.is_ok:
-            return
-
-        d = self.__data
-        interactor.execute(
-            search_books.Request(
-                isbn=str(v) if (v := d.get("isbn")) else None,
-                title=str(v) if (v := d.get("title")) else None,
-                year=int(v) if (v := d.get("year")) else None,
-                author=str(v) if (v := d.get("author")) else None,
-                genre=str(v) if (v := d.get("genre")) else None,
-                page_number=int(v) if (v := d.get("page")) else None,
-                page_size=self.__page_size,
-            )
-        )
+        if self.__do_search:
+            interactor.execute(self.request)
 
 
 class AddBook:
-    def __init__(self, data: MultiDict[str, Any]) -> None:
-        self.__data = data
+    request: Optional[add_book.Request] = None
 
-    def call(self, interactor: add_book.Interactor) -> None:
-        if not self.__data:
-            return
-
-        validator = validators.AddBook(self.__data)
-        if not validator.is_ok:
-            return
-
-        d = self.__data
-        interactor.execute(
-            add_book.Request(
-                isbn=str(d.get("isbn", "")),
-                title=str(d.get("title", "")),
-                year=int(d.get("year", "")),
-                authors=[a.strip() for a in d.get("authors", "").split(",")],
-                genres=[g.strip() for g in d.get("genres", "").split(",")],
-                cover=str(d.get("cover", "")),
+    def __init__(self, data: MultiDict[str, Any], user_id: str = "") -> None:
+        try:
+            self.request = add_book.Request(
+                user_id=user_id,
+                isbn=str(data.get("isbn", "")),
+                title=str(data.get("title", "")),
+                year=int(data.get("year", "")),
+                authors=[a.strip() for a in data.get("authors", "").split(",")],
+                genres=[g.strip() for g in data.get("genres", "").split(",")],
+                cover=str(data.get("cover", "")),
             )
-        )
+        except Exception:
+            pass
 
+    def call(self, interactor: add_book.Interactor) -> None:
+        if self.request:
+            interactor.execute(self.request)
+        else:
+            raise BadRequest()
 
-class UpdateBook:
-    def __init__(self, isbn: str, data: MultiDict[str, Any]) -> None:
-        self.__isbn = isbn
-        self.__data = data
 
-    def call(self, interactor: update_book.Interactor) -> None:
-        if not self.__data:
-            return
+class UpdateBook:
+    request: Optional[update_book.Request] = None
 
-        validator = validators.UpdateBook(self.__data)
-        if not validator.is_ok:
-            return
-
-        d = self.__data
-        interactor.execute(
-            update_book.Request(
-                isbn=self.__isbn,
-                title=str(d.get("title", "")),
-                year=int(d.get("year", "")),
-                authors=[a.strip() for a in d.get("authors", "").split(",")],
-                genres=[g.strip() for g in d.get("genres", "").split(",")],
-                cover=str(d.get("cover", "")),
+    def __init__(self, isbn: str, data: MultiDict[str, Any], user_id: str = "") -> None:
+        try:
+            self.request = update_book.Request(
+                user_id=user_id,
+                isbn=isbn,
+                title=str(data.get("title", "")),
+                year=int(data.get("year", "")),
+                authors=[a.strip() for a in data.get("authors", "").split(",")],
+                genres=[g.strip() for g in data.get("genres", "").split(",")],
+                cover=str(data.get("cover", "")),
             )
-        )
+        except Exception:
+            pass
+
+    def call(self, interactor: update_book.Interactor) -> None:
+        if self.request:
+            interactor.execute(self.request)
+        else:
+            raise BadRequest()
```

### Comparing `bl_hector-0.1.0a3/bl_hector/interfaces/from_json.py` & `bl_hector-0.1.0a4/bl_hector/interfaces/from_json.py`

 * *Files 5% similar despite different names*

```diff
@@ -17,30 +17,32 @@
 import json
 import logging
 
 from bl_hector.application.use_cases import add_book
 
 
 class AddBook:
-    def __init__(self, data: str) -> None:
+    def __init__(self, data: str, user_id: str = "") -> None:
         self.__data = data
+        self.__user_id = user_id
 
     def call(self, interactor: add_book.Interactor) -> None:
         if not self.__data:
             return
 
         try:
             data = json.loads(self.__data)
         except Exception as exc:
             logging.error(f"AddBook: {exc}")
             logging.exception(exc)
             data = {}
 
         interactor.execute(
             add_book.Request(
+                user_id=self.__user_id,
                 isbn=str(data.get("isbn", "")),
                 title=str(data.get("title", "")),
                 year=int(data.get("year", "0")),
                 authors=data.get("authors", []),
                 genres=data.get("genres", []),
             )
         )
```

### Comparing `bl_hector-0.1.0a3/bl_hector/interfaces/l10n/__init__.py` & `bl_hector-0.1.0a4/bl_hector/interfaces/l10n/__init__.py`

 * *Files identical despite different names*

### Comparing `bl_hector-0.1.0a3/bl_hector/interfaces/l10n/en-GB/main.ftl` & `bl_hector-0.1.0a4/bl_hector/interfaces/l10n/en-GB/main.ftl`

 * *Files 4% similar despite different names*

```diff
@@ -30,15 +30,15 @@
 license = Code is licensed under <a href="{ $url }">{ $name }</a>.
 
 # name (string) The name of the information to display
 # value (string) The value of the information to display
 info-line = { $name }: { $value }
 
 access-forbidden = Access forbidden!
-access-unauthorised = Access unauthorised!
+access-not-authorized = Access unauthorised!
 an-error-occurred = An error occurred!
 
 book = book
 books = books
 book-isbn = ISBN
 book-isbn-description = The ISBN assigned to the book, for instance 978-0-7653-9277-0.
 book-title = title
@@ -50,14 +50,15 @@
 book-authors = authors
 book-authors-description = The list of authors of the book, comma separated.
 book-genre = genre
 book-genre-description = One of the genres the book belongs to.
 book-genres = genres
 book-genres-description = The list of genres the book belongs to, comma separated.
 
+unknown-error = An unknown error has occurred!
 mandatory-value = This value is mandatory!
 incorrect-value = Incorrect value!
 not-an-isbn = This is not an ISBN!
 
 auth-login-title = Log in
 # method (string) The sign in method
 auth-login-method = Sign in using { $method }
@@ -72,14 +73,15 @@
 webauthn-login-failure = You couldn't be logged in!?
 
 add-book-requires-authentification = You must be authenticated before adding a book!
 add-book-title = Add a new book to the collection
 add-book-action = Add a book
 add-book-cancel = Cancel
 add-book-add = Add
+add-book-cover-help = Click to upload a cover
 
 search-books-title = Search for a book
 search-books-action = Look up book
 search-books-clear = Clear
 search-books-search = Search
 search-books-no-result = No matching book!
 search-books-previous-page = Previous
@@ -92,13 +94,14 @@
 # isbn (string) The ISBN of the book
 update-book-title = Edit information for `{ $isbn }`
 update-book-action = Edit
 update-book-failure = Book cannot be updated!
 update-book-success = Book has been updated!
 update-book-cancel = Cancel
 update-book-update = Save
+update-book-cover-help = Click to upload a new cover
 
 book-already-exists = Book already in the collection!
 book-added = Book successfully added!
 book-not-found = Book not found!
 book-cannot-be-added = The book cannot be added!
 books-cannot-be-found = The search cannot be performed!
```

#### html2text {}

```diff
@@ -11,41 +11,42 @@
 menu-logout = Log out # version (string) The version of the software. # years
 (string) The years the copyright applies to. # holders (string) The names of
 the copyright holders. copyright = Version { $version } Â© { $years }
 { $holders }. # name (string) The name of the license. # url (string) The URL
 of the license file. license = Code is licensed under {_$name_}. # name
 (string) The name of the information to display # value (string) The value of
 the information to display info-line = { $name }: { $value } access-forbidden =
-Access forbidden! access-unauthorised = Access unauthorised! an-error-occurred
-= An error occurred! book = book books = books book-isbn = ISBN book-isbn-
-description = The ISBN assigned to the book, for instance 978-0-7653-9277-0.
-book-title = title book-title-description = The title of the book. book-year =
-year book-year-description = The year the book was published in. book-author =
-author book-author-description = One of the authors of the book. book-authors =
-authors book-authors-description = The list of authors of the book, comma
+Access forbidden! access-not-authorized = Access unauthorised! an-error-
+occurred = An error occurred! book = book books = books book-isbn = ISBN book-
+isbn-description = The ISBN assigned to the book, for instance 978-0-7653-9277-
+0. book-title = title book-title-description = The title of the book. book-year
+= year book-year-description = The year the book was published in. book-author
+= author book-author-description = One of the authors of the book. book-authors
+= authors book-authors-description = The list of authors of the book, comma
 separated. book-genre = genre book-genre-description = One of the genres the
 book belongs to. book-genres = genres book-genres-description = The list of
-genres the book belongs to, comma separated. mandatory-value = This value is
-mandatory! incorrect-value = Incorrect value! not-an-isbn = This is not an
-ISBN! auth-login-title = Log in # method (string) The sign in method auth-
-login-method = Sign in using { $method } webauthn-register-title = Device
-registration webauthn-register-description = Your browser should be asking you
-to tap your security deviceâ¦ webauthn-register-success = Your security device
-has been succesfully registered! webauthn-register-failure = Your security
-device could not be registered!? webauthn-login-title = Log in webauthn-login-
-description = Your browser should be asking you to tap your security deviceâ¦
-webauthn-login-failure = You couldn't be logged in!? add-book-requires-
-authentification = You must be authenticated before adding a book! add-book-
-title = Add a new book to the collection add-book-action = Add a book add-book-
-cancel = Cancel add-book-add = Add search-books-title = Search for a book
-search-books-action = Look up book search-books-clear = Clear search-books-
-search = Search search-books-no-result = No matching book! search-books-
-previous-page = Previous search-books-next-page = Next # title (string) The
-title of the book display-book-title = Details for "{ $title }" update-book-
-requires-authentification = You must be authenticated before editing a book! #
-isbn (string) The ISBN of the book update-book-title = Edit information for `
-{ $isbn }` update-book-action = Edit update-book-failure = Book cannot be
+genres the book belongs to, comma separated. unknown-error = An unknown error
+has occurred! mandatory-value = This value is mandatory! incorrect-value =
+Incorrect value! not-an-isbn = This is not an ISBN! auth-login-title = Log in #
+method (string) The sign in method auth-login-method = Sign in using { $method
+} webauthn-register-title = Device registration webauthn-register-description =
+Your browser should be asking you to tap your security deviceâ¦ webauthn-
+register-success = Your security device has been succesfully registered!
+webauthn-register-failure = Your security device could not be registered!?
+webauthn-login-title = Log in webauthn-login-description = Your browser should
+be asking you to tap your security deviceâ¦ webauthn-login-failure = You
+couldn't be logged in!? add-book-requires-authentification = You must be
+authenticated before adding a book! add-book-title = Add a new book to the
+collection add-book-action = Add a book add-book-cancel = Cancel add-book-add =
+Add add-book-cover-help = Click to upload a cover search-books-title = Search
+for a book search-books-action = Look up book search-books-clear = Clear
+search-books-search = Search search-books-no-result = No matching book! search-
+books-previous-page = Previous search-books-next-page = Next # title (string)
+The title of the book display-book-title = Details for "{ $title }" update-
+book-requires-authentification = You must be authenticated before editing a
+book! # isbn (string) The ISBN of the book update-book-title = Edit information
+for `{ $isbn }` update-book-action = Edit update-book-failure = Book cannot be
 updated! update-book-success = Book has been updated! update-book-cancel =
-Cancel update-book-update = Save book-already-exists = Book already in the
-collection! book-added = Book successfully added! book-not-found = Book not
-found! book-cannot-be-added = The book cannot be added! books-cannot-be-found =
-The search cannot be performed!
+Cancel update-book-update = Save update-book-cover-help = Click to upload a new
+cover book-already-exists = Book already in the collection! book-added = Book
+successfully added! book-not-found = Book not found! book-cannot-be-added = The
+book cannot be added! books-cannot-be-found = The search cannot be performed!
```

### Comparing `bl_hector-0.1.0a3/bl_hector/interfaces/l10n/fr-FR/main.ftl` & `bl_hector-0.1.0a4/bl_hector/interfaces/l10n/fr-FR/main.ftl`

 * *Files 10% similar despite different names*

```diff
@@ -30,15 +30,15 @@
 license = Le code est sous licence <a href="{ $url }">{ $name }</a>.
 
 # name (string) The name of the information to display
 # value (string) The value of the information to display
 info-line = { $name } : { $value }
 
 access-forbidden = Accès interdit !
-access-unauthorised = Accès non authorisé !
+access-not-authorized = Accès non authorisé !
 an-error-occurred = Une erreur s'est produite !
 
 book = livre
 books = livres
 book-isbn = ISBN
 book-isbn-description = Le numéro ISBN assigné au livre, par exemple 978-0-7653-9277-0.
 book-title = titre
@@ -50,14 +50,15 @@
 book-authors = aut·rice·eur·s
 book-authors-description = La liste des aut·rice·eur·s du livre, séparé·e·s par des virgules.
 book-genre = genre
 book-genre-description = Un des genres auxquels le livre se rattache.
 book-genres = genres
 book-genres-description = La liste des genres auxquels le livre se rattache, séparés par des virgules.
 
+unknown-error = Une erreur inconnue s'est produite !
 mandatory-value = Cette valeur est obligatoire !
 incorrect-value = Cette valeur est incorrecte !
 not-an-isbn = Ceci n'est pas un ISBN !
 
 auth-login-title = Connexion
 # method (string) The sign in method
 auth-login-method = Sign in using { $method }
@@ -72,14 +73,15 @@
 webauthn-login-failure = Vous n'avez pas pu être connecté·e !?
 
 add-book-requires-authentification = Vous devez être authentifié·e pour pouvoir ajouter un livre !
 add-book-title = Ajouter un nouveau livre à la collection
 add-book-action = Ajouter un livre
 add-book-cancel = Annuler
 add-book-add = Ajouter
+add-book-cover-help = Cliquez pour téléverser une couverture
 
 search-books-title = Chercher un livre dans la collection
 search-books-action = Chercher un livre
 search-books-clear = Réinitialiser
 search-books-search = Chercher
 search-books-no-result = Aucun livre ne correspond !
 search-books-previous-page = Précédent
@@ -92,13 +94,14 @@
 # isbn (string) The ISBN of the book
 update-book-title = Éditer les informations de `{ $isbn }`
 update-book-action = Éditer
 update-book-failure = Le livre n'a pas pu être mis à jour !
 update-book-success = Le livre a bien été mis à jour !
 update-book-cancel = Annuler
 update-book-update = Enregistrer
+update-book-cover-help = Cliquez pour téléverser une nouvelle couverture
 
 book-already-exists = Ce livre est déjà dans la collection !
 book-added = Le livre a bien été ajouté.
 book-not-found = Le livre n'a pas été trouvé !
 book-cannot-be-added = Le livre n'a pas pu être ajouté !
 books-cannot-be-found = La recherche n'a pas pu être effectuée !
```

#### html2text {}

```diff
@@ -11,47 +11,50 @@
 connecter menu-logout = Se dÃ©connecter # version (string) The version of the
 software. # years (string) The years the copyright applies to. # holders
 (string) The names of the copyright holders. copyright = Version { $version }
 Â© { $years } { $holders }. # name (string) The name of the license. # url
 (string) The URL of the license file. license = Le code est sous licence
 {_$name_}. # name (string) The name of the information to display # value
 (string) The value of the information to display info-line = { $name }Â :
-{ $value } access-forbidden = AccÃ¨s interditÂ ! access-unauthorised = AccÃ¨s
+{ $value } access-forbidden = AccÃ¨s interditÂ ! access-not-authorized = AccÃ¨s
 non authorisÃ©Â ! an-error-occurred = Une erreur s'est produiteÂ ! book = livre
 books = livres book-isbn = ISBN book-isbn-description = Le numÃ©ro ISBN
 assignÃ© au livre, par exemple 978-0-7653-9277-0. book-title = titre book-
 title-description = Le titre du livre. book-year = annÃ©e book-year-description
 = L'annÃ©e de publication du livre. book-author = autÂ·riceÂ·eur book-author-
 description = UnÂ·e des autÂ·riceÂ·eurÂ·s du livre. book-authors =
 autÂ·riceÂ·eurÂ·s book-authors-description = La liste des autÂ·riceÂ·eurÂ·s du
 livre, sÃ©parÃ©Â·eÂ·s par des virgules. book-genre = genre book-genre-
 description = Un des genres auxquels le livre se rattache. book-genres = genres
 book-genres-description = La liste des genres auxquels le livre se rattache,
-sÃ©parÃ©s par des virgules. mandatory-value = Cette valeur est obligatoireÂ !
-incorrect-value = Cette valeur est incorrecteÂ ! not-an-isbn = Ceci n'est pas
-un ISBNÂ ! auth-login-title = Connexion # method (string) The sign in method
-auth-login-method = Sign in using { $method } webauthn-register-title =
-Association du dispositif de sÃ©curitÃ© webauthn-register-description = Votre
-navigateur devrait Ãªtre en train de vous demander de toucher votre dispositif
-de sÃ©curitÃ©â¦ webauthn-register-success = Votre dispositif de sÃ©curitÃ© a
-Ã©tÃ© correctement associÃ©Â ! webauthn-register-failure = Votre dispositif de
-sÃ©curitÃ© n'a pas pu Ãªtre associÃ©Â !? webauthn-login-title = Connexion
-webauthn-login-description = Votre navigateur devrait Ãªtre en train de vous
-demander de toucher votre dispositif de sÃ©curitÃ©â¦ webauthn-login-failure =
-Vous n'avez pas pu Ãªtre connectÃ©Â·eÂ !? add-book-requires-authentification =
-Vous devez Ãªtre authentifiÃ©Â·e pour pouvoir ajouter un livreÂ ! add-book-
-title = Ajouter un nouveau livre Ã  la collection add-book-action = Ajouter un
-livre add-book-cancel = Annuler add-book-add = Ajouter search-books-title =
-Chercher un livre dans la collection search-books-action = Chercher un livre
-search-books-clear = RÃ©initialiser search-books-search = Chercher search-
-books-no-result = Aucun livre ne correspondÂ ! search-books-previous-page =
-PrÃ©cÃ©dent search-books-next-page = Suivant # title (string) The title of the
-book display-book-title = DÃ©tails pour Â«Â { $title }Â Â» update-book-
-requires-authentification = Vous devez Ãªtre authentifiÃ©Â·e pour pouvoir
-Ã©diter un livreÂ ! # isbn (string) The ISBN of the book update-book-title =
-Ãditer les informations de `{ $isbn }` update-book-action = Ãditer update-
-book-failure = Le livre n'a pas pu Ãªtre mis Ã  jourÂ ! update-book-success =
-Le livre a bien Ã©tÃ© mis Ã  jourÂ ! update-book-cancel = Annuler update-book-
-update = Enregistrer book-already-exists = Ce livre est dÃ©jÃ  dans la
-collectionÂ ! book-added = Le livre a bien Ã©tÃ© ajoutÃ©. book-not-found = Le
-livre n'a pas Ã©tÃ© trouvÃ©Â ! book-cannot-be-added = Le livre n'a pas pu Ãªtre
-ajoutÃ©Â ! books-cannot-be-found = La recherche n'a pas pu Ãªtre effectuÃ©eÂ !
+sÃ©parÃ©s par des virgules. unknown-error = Une erreur inconnue s'est
+produiteÂ ! mandatory-value = Cette valeur est obligatoireÂ ! incorrect-value =
+Cette valeur est incorrecteÂ ! not-an-isbn = Ceci n'est pas un ISBNÂ ! auth-
+login-title = Connexion # method (string) The sign in method auth-login-method
+= Sign in using { $method } webauthn-register-title = Association du dispositif
+de sÃ©curitÃ© webauthn-register-description = Votre navigateur devrait Ãªtre en
+train de vous demander de toucher votre dispositif de sÃ©curitÃ©â¦ webauthn-
+register-success = Votre dispositif de sÃ©curitÃ© a Ã©tÃ© correctement
+associÃ©Â ! webauthn-register-failure = Votre dispositif de sÃ©curitÃ© n'a pas
+pu Ãªtre associÃ©Â !? webauthn-login-title = Connexion webauthn-login-
+description = Votre navigateur devrait Ãªtre en train de vous demander de
+toucher votre dispositif de sÃ©curitÃ©â¦ webauthn-login-failure = Vous n'avez
+pas pu Ãªtre connectÃ©Â·eÂ !? add-book-requires-authentification = Vous devez
+Ãªtre authentifiÃ©Â·e pour pouvoir ajouter un livreÂ ! add-book-title = Ajouter
+un nouveau livre Ã  la collection add-book-action = Ajouter un livre add-book-
+cancel = Annuler add-book-add = Ajouter add-book-cover-help = Cliquez pour
+tÃ©lÃ©verser une couverture search-books-title = Chercher un livre dans la
+collection search-books-action = Chercher un livre search-books-clear =
+RÃ©initialiser search-books-search = Chercher search-books-no-result = Aucun
+livre ne correspondÂ ! search-books-previous-page = PrÃ©cÃ©dent search-books-
+next-page = Suivant # title (string) The title of the book display-book-title =
+DÃ©tails pour Â«Â { $title }Â Â» update-book-requires-authentification = Vous
+devez Ãªtre authentifiÃ©Â·e pour pouvoir Ã©diter un livreÂ ! # isbn (string)
+The ISBN of the book update-book-title = Ãditer les informations de `{ $isbn
+}` update-book-action = Ãditer update-book-failure = Le livre n'a pas pu Ãªtre
+mis Ã  jourÂ ! update-book-success = Le livre a bien Ã©tÃ© mis Ã  jourÂ !
+update-book-cancel = Annuler update-book-update = Enregistrer update-book-
+cover-help = Cliquez pour tÃ©lÃ©verser une nouvelle couverture book-already-
+exists = Ce livre est dÃ©jÃ  dans la collectionÂ ! book-added = Le livre a bien
+Ã©tÃ© ajoutÃ©. book-not-found = Le livre n'a pas Ã©tÃ© trouvÃ©Â ! book-cannot-
+be-added = Le livre n'a pas pu Ãªtre ajoutÃ©Â ! books-cannot-be-found = La
+recherche n'a pas pu Ãªtre effectuÃ©eÂ !
```

### Comparing `bl_hector-0.1.0a3/bl_hector/interfaces/to_http/__init__.py` & `bl_hector-0.1.0a4/bl_hector/interfaces/to_http/__init__.py`

 * *Files identical despite different names*

### Comparing `bl_hector-0.1.0a3/bl_hector/interfaces/to_http/as_html/__init__.py` & `bl_hector-0.1.0a4/bl_hector/interfaces/to_http/as_html/__init__.py`

 * *Files 14% similar despite different names*

```diff
@@ -26,17 +26,19 @@
 from bl_hector.application.use_cases import (
     add_book,
     display_book,
     look_up_book,
     search_books,
     update_book,
 )
+from bl_hector.domain.collection_management import exceptions as errors
+from bl_hector.domain.collection_management import validators
 from bl_hector.domain.collection_management.entities import Book
 from bl_hector.domain.collection_management.value_objects import Isbn
-from bl_hector.interfaces import User, l10n, validators
+from bl_hector.interfaces import User, l10n
 from bl_hector.interfaces.to_http import HttpPresenter
 
 ENVIRONMENT = Environment(
     loader=FileSystemLoader([Path(__file__).parent / "templates"]),
     autoescape=select_autoescape(),
     extensions=["bl_hector.interfaces.utils.PatchedPyPugJSExtension"],
 )
@@ -62,26 +64,36 @@
         user: Optional[User] = None,
         **context: Any,
     ) -> None:
         self.__status_code = HTTP.OK
         self.__headers = {"Content-Type": "text/html; charset=UTF-8"}
         self.__template = template if template.endswith(".pug") else f"{template}.pug"
         self.__fragment = fragment
+        self.__user = user
         self.__context: dict[str, Any] = {**context, "_": self._, "user": user}
         self.__error = ""
 
         self.__adapt_to(user)
 
     def __adapt_to(self, user: Optional[User] = None) -> None:
         locale = user.locale if (user and user.locale) else l10n.DEFAULT_LOCALE
         self.__localization = l10n.localization(locale)
 
     def _(self, message_id: str, **kwargs: Any) -> str:
         return str(self.__localization.format_value(message_id, kwargs))
 
+    def translate_error(self, error: Optional[errors.IncorrectValue] = None) -> str:
+        if not error:
+            return ""
+
+        # FIXME: Dispatching errors based on class is not very LSP!?
+        if isinstance(error, errors.IncorrectValue):
+            return self._("incorrect-value")
+        return self._("unknown-error")
+
     def status_code(self) -> int:
         return int(self.__status_code)
 
     def headers(self) -> dict[str, str]:
         return self.__headers
 
     def data(self) -> str:
@@ -99,25 +111,27 @@
 
     def redirect(self, url: str, status_code: HTTP = HTTP.SEE_OTHER) -> None:
         if "Content-Type" in self.__headers:
             del self.__headers["Content-Type"]
         self.__headers["Location"] = url
         self.set_status_code(status_code)
 
-    def access_not_allowed(self, login: str) -> None:
-        if login:
+    def not_authorized(self) -> None:
+        if self.__user:
             self.set_status_code(HTTP.FORBIDDEN)
             self.__error = self._("access-forbidden")
         else:
             self.set_status_code(HTTP.UNAUTHORIZED)
-            self.__error = self._("access-unauthorised")
+            self.__error = self._("access-not-authorized")
 
     def render(self, **context: Any) -> str:
         if self.__error:
-            return ENVIRONMENT.get_template("error.pug").render(message=self.__error)
+            return ENVIRONMENT.get_template("error.pug").render(
+                **self.__context, **context, message=self.__error
+            )
         if self.__fragment:
             return render_block(  # type: ignore
                 ENVIRONMENT,
                 self.__template,
                 self.__fragment,
                 **self.__context,
                 **context,
@@ -140,20 +154,14 @@
     ) -> None:
         super().__init__("books/search", fragment=fragment, user=user)
         self.__data = data
         self.__context: dict[str, Any] = {"errors": {}}
 
         self.__set_page_urls()
 
-        if data:
-            if result := validators.SearchBooks(data):
-                self.__context["books"] = []
-            else:
-                self.__context["errors"] = result.get_errors(self._)
-
     def __set_page_urls(self) -> None:
         self.__context["previous_page_url"] = self.__build_url(
             {**self.__data, "page": self.__previous_page_number()}
         )
         # FIXME How to know if there are more results?!
         self.__context["next_page_url"] = self.__build_url(
             {**self.__data, "page": self.__next_page_number()}
@@ -175,75 +183,69 @@
         if n := int(self.__data.get("page", "0")):
             return f"{n - 1}"
         return ""
 
     def render(self, **context: Any) -> str:
         return super().render(**self.__context, **context, data=self.__data)
 
-    def bad_request(self) -> None:
-        # FIXME setting status code to 404 is not supported by htmx!?
-        self.__context["error"] = self._("books-cannot-be-found")
+    def bad_request(self, errors: search_books.Errors) -> None:
+        self.set_status_code(HTTP.OK)
+        self.__context["errors"] = {
+            "isbn": self.translate_error(errors.isbn),
+            "title": self.translate_error(errors.title),
+            "year": self.translate_error(errors.year),
+            "author": self.translate_error(errors.author),
+            "genre": self.translate_error(errors.genre),
+        }
 
     def book(self, book: Book) -> None:
         if "books" not in self.__context:
             self.__context["books"] = []
         self.__context["books"].append(
             {
                 "isbn": str(book.isbn),
                 "title": str(book.title),
                 "year": int(book.year),
-                "authors": ", ".join(str(a) for a in book.authors),
-                "genres": ", ".join(str(g) for g in book.genres),
+                "authors": [str(a) for a in book.authors],
+                "genres": [str(g) for g in book.genres],
                 "cover": str(book.cover) if book.cover else "",
             }
         )
 
 
-class ValidateIsbn(JinjaPresenter):
-    def __init__(
-        self, data: MultiDict[str, Any], /, *, user: Optional[User] = None
-    ) -> None:
-        super().__init__("books/search", fragment="isbn", user=user)
-        self.__data = data
-
-    def render(self, **context: Any) -> str:
-        return super().render(
-            **context,
-            data=self.__data,
-            errors=validators.SearchBooks(self.__data).get_errors(self._),
-        )
-
-
 class AddBook(JinjaPresenter, add_book.Presenter):
     def __init__(
         self,
         data: MultiDict[str, Any],
         /,
         *,
         notify: Callable[[str, str], None] = lambda m, t: None,
         user: Optional[User] = None,
     ) -> None:
         super().__init__("books/add", user=user)
+        self.set_status_code(HTTP.FORBIDDEN)
         self.__data = data
         self.__notify = notify
         self.__context: dict[str, Any] = {"errors": {}}
 
-        if data:
-            self.__context["errors"] = validators.AddBook(data).get_errors(self._)
-
     def render(self, **context: Any) -> str:
         return super().render(**self.__context, **context, data=self.__data)
 
-    def bad_request(self) -> None:
-        # FIXME setting status code to 404 is not supported by htmx!?
-        self.__context["error"] = self._("book-cannot-be-added")
+    def bad_request(self, errors: add_book.Errors) -> None:
+        self.set_status_code(HTTP.OK)
+        self.__context["errors"] = {
+            "isbn": self.translate_error(errors.isbn),
+            "title": self.translate_error(errors.title),
+            "year": self.translate_error(errors.year),
+            "authors": self.translate_error(errors.authors),
+        }
 
     def book_already_exists(self, book: Book) -> None:
         self.__notify(self._("book-already-exists"), "info")
-        self.redirect(url_for("books.search", isbn=str(book.isbn)))
+        self.redirect(url_for("books.display", isbn=str(book.isbn)))
 
     def book_added(self, book: Book) -> None:
         self.__notify(self._("book-added"), "success")
         self.redirect(url_for("books.search", isbn=str(book.isbn)))
 
 
 class LookUpBook(JinjaPresenter, look_up_book.Presenter):
@@ -359,26 +361,46 @@
         data: MultiDict[str, Any],
         /,
         *,
         notify: Callable[[str, str], None] = lambda m, t: None,
         user: Optional[User] = None,
     ) -> None:
         super().__init__("books/update", user=user)
+        self.set_status_code(HTTP.FORBIDDEN)
         self.__data = data
         self.__notify = notify
-        self.__context: dict[str, Any] = {"isbn": isbn}
-        self.__context["errors"] = validators.UpdateBook(data).get_errors(self._)
+        self.__context: dict[str, Any] = {"isbn": isbn, "errors": {}}
 
     def render(self, **context: Any) -> str:
         return super().render(**self.__context, **context, data=self.__data)
 
-    def bad_request(self) -> None:
-        # FIXME setting status code to 404 is not supported by htmx!?
-        self.__context["error"] = self._("update-book-failure")
+    def bad_request(self, errors: update_book.Errors) -> None:
+        self.set_status_code(HTTP.OK)
+        self.__context["errors"] = {
+            "title": self.translate_error(errors.title),
+            "year": self.translate_error(errors.year),
+            "authors": self.translate_error(errors.authors),
+        }
 
     def book_not_found(self, isbn: Isbn) -> None:
         self.__notify(self._("book-not-found"), "warning")
         self.redirect(url_for("books.search"))
 
     def book_updated(self, book: Book) -> None:
         self.__notify(self._("update-book-success"), "success")
         self.redirect(url_for("books.display", isbn=str(book.isbn)))
+
+
+class ValidateIsbn(JinjaPresenter):
+    def __init__(
+        self, data: MultiDict[str, Any], /, *, user: Optional[User] = None
+    ) -> None:
+        super().__init__("books/search", fragment="isbn", user=user)
+        self.__data = data
+        self.__errors = {}
+
+        if isbn := data.get("isbn", ""):
+            errors = add_book.Errors(isbn=validators.isbn(isbn))
+            self.__errors["isbn"] = self.translate_error(errors.isbn)
+
+    def render(self, **context: Any) -> str:
+        return super().render(**context, data=self.__data, errors=self.__errors)
```

### Comparing `bl_hector-0.1.0a3/bl_hector/interfaces/to_http/as_html/templates/auth/login.pug` & `bl_hector-0.1.0a4/bl_hector/interfaces/to_http/as_html/templates/auth/login.pug`

 * *Files 4% similar despite different names*

```diff
@@ -23,13 +23,13 @@
   section.section
     .container
       h1.title.is-3.has-text-centered= _("auth-login-title")
 
       .columns
         .column
         .column
-          .buttons(hx-boost="false")
+          .buttons
             each link in links
-              a.button.is-fullwidth(href="#{link.url}")
+              a.button.is-fullwidth(href="#{url_for(link.route)}")
                 span.icon: i.fas(class="fa-#{link.icon}")
                 span= _("auth-login-method", method=link.label)
         .column
```

### Comparing `bl_hector-0.1.0a3/bl_hector/interfaces/to_http/as_html/templates/books/add.pug` & `bl_hector-0.1.0a4/bl_hector/interfaces/to_http/as_html/templates/books/add.pug`

 * *Files 7% similar despite different names*

```diff
@@ -47,42 +47,44 @@
                   accept="image/*"
                   type="file"
                   _="on change set img to #cover then set inp to #coverInput then js(me, img, inp) loadIntoImage(me, img, inp)"
                 )
                 img#cover.cover.is-2by3(
                   src="#{data.cover or url_for('static', filename='img/placeholders/320x480.png')}"
                   alt="Book cover"
+                  title=_("add-book-cover-help")
+                  style="cursor: pointer"
                   _="on click set target to #coverUploader js(target) target.click()"
                 )
                 input#coverInput.is-hidden(
                   name="cover"
                   type="text"
                   value="#{data.cover}"
                 )
               .column
                 block isbn
                   .field.is-horizontal(_="on load remove @disabled from .button")
                     .field-body
                       include books/mixins/render_isbn
-                      +isbn_field(data.isbn, errors.isbn)
+                      +isbn_field(data.isbn, errors.isbn, required="1")
 
                       .field.is-narrow
                         p.control
                           button.button.is-info(
                             hx-post="#{url_for('books.look_up')}"
                             hx-target="#form"
                             disabled
                             _="on htmx:beforeSend add .is-loading add @disabled"
                           )
                             span.icon: i.fas.fa-search
                             span= _("search-books-action")
 
-                +text_field("title", data.title, errors.title, description=_("book-title-description"), icon="file", placeholder=_('book-title'))
-                +number_field("year", data.year, errors.year, description=_("book-year-description"), icon="calendar", placeholder=_('book-year'))
-                +text_field("authors", data.authors, errors.authors, description=_("book-authors-description"), icon="users", placeholder=_('book-authors'))
+                +text_field("title", data.title, errors.title, required="1", description=_("book-title-description"), icon="file", placeholder=_('book-title'))
+                +number_field("year", data.year, errors.year, required="1", description=_("book-year-description"), icon="calendar", placeholder=_('book-year'))
+                +text_field("authors", data.authors, errors.authors, required="1", description=_("book-authors-description"), icon="users", placeholder=_('book-authors'))
                 +text_field("genres", data.genres, errors.genres, description=_("book-genres-description"), icon="crown", placeholder=_('book-genres'))
 
                 .field
                   p.control
                     a.button.is-light(href="#{url_for('books.search')}")
                       span.icon: i.fas.fa-times
                       span= _("add-book-cancel")
```

### Comparing `bl_hector-0.1.0a3/bl_hector/interfaces/to_http/as_html/templates/books/display.pug` & `bl_hector-0.1.0a4/bl_hector/interfaces/to_http/as_html/templates/books/display.pug`

 * *Files 9% similar despite different names*

```diff
@@ -19,15 +19,15 @@
 block title
   title= _("hector") + " – " + _("display-book-title", title=book.title)
 
 block content
   section.section
     .container
       .buttons.is-pulled-right
-        if user.id
+        if user.can_update_book
           a.button.is-link(href="#{url_for('books.update', isbn=book.isbn)}")
             span.icon: i.fas.fa-edit
             span= _("update-book-action")
         else
           button.button.is-link.is-disabled(disabled title=_("update-book-requires-authentification"))
             span.icon: i.fas.fa-edit
             span= _("update-book-action")
```

### Comparing `bl_hector-0.1.0a3/bl_hector/interfaces/to_http/as_html/templates/books/mixins/render_isbn.pug` & `bl_hector-0.1.0a4/bl_hector/interfaces/to_http/as_html/templates/books/mixins/render_isbn.pug`

 * *Files 15% similar despite different names*

```diff
@@ -12,36 +12,52 @@
 //- GNU Affero General Public License for more details.
 //-
 //- You should have received a copy of the GNU Affero General Public License
 //- along with this program. If not, see <http://www.gnu.org/licenses/>.
 
 include mixins/form
 
-mixin isbn_field(value, error)
+mixin isbn_field(value, error, required="")
   .field
     p.control.has-icons-left.has-icons-right
       if error
         - var classes = "is-danger"
       elif value
         - var classes = "is-success"
       else
         - var classes = ""
 
-      input.input(
-        type="text"
-        id="isbn"
-        name="isbn"
-        class=classes
-        value=value
-        placeholder=_("book-isbn")
-        hx-post=url_for("books.validate_isbn")
-        hx-trigger="search, change, keyup delay:200ms changed"
-        hx-target="closest .field"
-        hx-swap="outerHTML"
-      )
+      //- TODO find a better way to set required!
+      if required
+        input.input(
+          type="text"
+          id="isbn"
+          name="isbn"
+          class=classes
+          value=value
+          required
+          placeholder=_("book-isbn")
+          hx-post=url_for("books.validate_isbn")
+          hx-trigger="search, blur"
+          hx-target="closest .field"
+          hx-swap="outerHTML"
+        )
+      else
+        input.input(
+          type="text"
+          id="isbn"
+          name="isbn"
+          class=classes
+          value=value
+          placeholder=_("book-isbn")
+          hx-post=url_for("books.validate_isbn")
+          hx-trigger="search, blur"
+          hx-target="closest .field"
+          hx-swap="outerHTML"
+        )
       span.icon.is-small.is-left: i.fas.fa-book
       if value
         span.icon.is-small.is-right
           if error
             i.fas.fa-exclamation-triangle
           else
             i.fas.fa-check
```

### Comparing `bl_hector-0.1.0a3/bl_hector/interfaces/to_http/as_html/templates/books/search.pug` & `bl_hector-0.1.0a4/bl_hector/interfaces/to_http/as_html/templates/books/search.pug`

 * *Files 8% similar despite different names*

```diff
@@ -19,15 +19,15 @@
 block title
   title= _("hector") + " – " + _("search-books-title")
 
 block content
   section.section
     .container
       .buttons.is-pulled-right
-        if user.id
+        if user.can_add_book
           a.button.is-link(href="#{url_for('books.add')}")
             span.icon: i.fas.fa-plus
             span= _("add-book-action")
         else
           button.button.is-link.is-disabled(disabled title=_("add-book-requires-authentification"))
             span.icon: i.fas.fa-plus
             span= _("add-book-action")
@@ -77,21 +77,30 @@
                       .card-content
                         .media
                           .media-left(style="width: 5em")
                             figure.image.cover.is-2by3
                               img(src="#{book.cover or url_for('static', filename='img/placeholders/320x480.png')}" alt="Book cover")
                           .media-content
                             h2.title.is-4(title="#{book.title}")= book.title|truncate(20)
-                            p.subtitle.is-6= book.authors
+                            p.subtitle.is-6
+                              each author in book.authors
+                                if author == book.authors[-1]
+                                  | #[a(href="#{url_for('books.search', author=author)}") #{author}]
+                                else
+                                  | #[a(href="#{url_for('books.search', author=author)}") #{author}], 
                             p
                               small
                                 | #[time(datetime="#{book.year}-01-01") #{book.year}] / 
-                                a(href="#{url_for('books.display', isbn=book.isbn)}" hx-boost="false") #{book.isbn}
+                                a(href="#{url_for('books.display', isbn=book.isbn)}") #{book.isbn}
                                 br
-                                | #{book.genres}
+                                each genre in book.genres
+                                  if genre == book.genres[-1]
+                                    | #[a(href="#{url_for('books.search', genre=genre)}") #{genre}]
+                                  else
+                                    | #[a(href="#{url_for('books.search', genre=genre)}") #{genre}], 
 
               #indicator.buttons.is-centered.mt-3.htmx-indicator.is-hidden(_="on load remove .is-hidden")
                   button.button.is-white.is-loading Loading indicator
 
               if previous_page_url or next_page_url:
                 .buttons.is-centered.mt-3(_="on load remove me")
                   if previous_page_url:
```

### Comparing `bl_hector-0.1.0a3/bl_hector/interfaces/to_http/as_html/templates/books/update.pug` & `bl_hector-0.1.0a4/bl_hector/interfaces/to_http/as_html/templates/books/update.pug`

 * *Files 10% similar despite different names*

```diff
@@ -47,25 +47,27 @@
                   accept="image/*"
                   type="file"
                   _="on change set img to #cover then set inp to #coverInput then js(me, img, inp) loadIntoImage(me, img, inp)"
                 )
                 img#cover.cover.is-2by3(
                   src="#{data.cover or url_for('static', filename='img/placeholders/320x480.png')}"
                   alt="Book cover"
+                  title=_("update-book-cover-help")
+                  style="cursor: pointer"
                   _="on click set target to #coverUploader js(target) target.click()"
                 )
                 input#coverInput.is-hidden(
                   name="cover"
                   type="text"
                   value="#{data.cover}"
                 )
               .column
-                +text_field("title", data.title, errors.title, description=_("book-title-description"), icon="file", placeholder=_('book-title'))
-                +number_field("year", data.year, errors.year, description=_("book-year-description"), icon="calendar", placeholder=_('book-year'))
-                +text_field("authors", data.authors, errors.authors, description=_("book-authors-description"), icon="users", placeholder=_('book-authors'))
+                +text_field("title", data.title, errors.title, required="1", description=_("book-title-description"), icon="file", placeholder=_('book-title'))
+                +number_field("year", data.year, errors.year, required="1", description=_("book-year-description"), icon="calendar", placeholder=_('book-year'))
+                +text_field("authors", data.authors, errors.authors, required="1", description=_("book-authors-description"), icon="users", placeholder=_('book-authors'))
                 +text_field("genres", data.genres, errors.genres, description=_("book-genres-description"), icon="crown", placeholder=_('book-genres'))
 
                 .field
                   p.control
                     a.button.is-light(href="#{url_for('books.display', isbn=data.isbn)}")
                       span.icon: i.fas.fa-times
                       span= _("update-book-cancel")
```

### Comparing `bl_hector-0.1.0a3/bl_hector/interfaces/to_http/as_html/templates/error.pug` & `bl_hector-0.1.0a4/bl_hector/interfaces/to_http/as_html/templates/error.pug`

 * *Files 12% similar despite different names*

```diff
@@ -13,16 +13,16 @@
 //-
 //- You should have received a copy of the GNU Affero General Public License
 //- along with this program. If not, see <http://www.gnu.org/licenses/>.
 
 extends layout
 
 block title
-  | #{_("an-error-occured")}
+  title= _("an-error-occurred")
 
 block content
   section.section.is-medium
     article.message.is-danger
       .message-header
-        p= _("an-error-occured")
+        p= _("an-error-occurred")
       .message-body
         p #{message}
```

### Comparing `bl_hector-0.1.0a3/bl_hector/interfaces/to_http/as_html/templates/layout.pug` & `bl_hector-0.1.0a4/bl_hector/interfaces/to_http/as_html/templates/layout.pug`

 * *Files 5% similar despite different names*

```diff
@@ -29,15 +29,15 @@
     link(rel="icon" type="image/svg" href="#{url_for('static', filename='favicon.svg')}")
     link(rel="stylesheet" href="#{url_for('static', filename='css/bulma@0.9.4.min.css')}")
     link(rel="stylesheet" href="#{url_for('static', filename='css/font-awesome@5.14.0.css')}")
     link(rel="stylesheet" href="#{url_for('static', filename='css/hector.css')}")
     block links
     block head_scripts
 
-  body(hx-boost="true")
+  body
     +navbar()
 
     .page
       - var messages = get_flashed_messages(with_categories=true)
       +flash(messages)
 
       block content
```

### Comparing `bl_hector-0.1.0a3/bl_hector/interfaces/to_http/as_html/templates/mixins/flash.pug` & `bl_hector-0.1.0a4/bl_hector/interfaces/to_http/as_html/templates/mixins/flash.pug`

 * *Files identical despite different names*

### Comparing `bl_hector-0.1.0a3/bl_hector/interfaces/to_http/as_html/templates/mixins/form.pug` & `bl_hector-0.1.0a4/bl_hector/interfaces/to_http/as_html/templates/mixins/form.pug`

 * *Files 8% similar despite different names*

```diff
@@ -14,45 +14,49 @@
 //- You should have received a copy of the GNU Affero General Public License
 //- along with this program. If not, see <http://www.gnu.org/licenses/>.
 
 
 mixin hidden_input(name, value)
   input(type="hidden" name=name value=value)
 
-mixin input(type, name, value, icon="", placeholder="", error="")
+mixin input(type, name, value, required="", icon="", placeholder="", error="")
   - var classes = "has-icons-left" if icon else ""
   p.control.has-icons-right(class=classes)
     - var classes = "is-danger" if error else ""
-    input.input(id=name name=name type=type placeholder=placeholder value=value class=classes)
+    //- TODO find a better way to set required!
+    if required
+      input.input(id=name name=name type=type placeholder=placeholder value=value class=classes required)
+    else
+      input.input(id=name name=name type=type placeholder=placeholder value=value class=classes)
     if icon
       span.icon.is-small.is-left: i.fas(class="fa-#{icon}")
 
-mixin text_input(name, value, icon="", placeholder="", error="")
-  +input("text", name, value, icon=icon, placeholder=placeholder, error=error)
+mixin text_input(name, value, required="", icon="", placeholder="", error="")
+  +input("text", name, value, required=required, icon=icon, placeholder=placeholder, error=error)
 
-mixin number_input(name, value, icon="", placeholder="", error="")
-  +input("number", name, value, icon=icon, placeholder=placeholder, error=error)
+mixin number_input(name, value, required="", icon="", placeholder="", error="")
+  +input("number", name, value, required=required, icon=icon, placeholder=placeholder, error=error)
 
 mixin help_message(value)
   if value
     p.help= value
 
 mixin error_message(error)
   if error
     p.help.is-danger= error
 
-mixin text_field(name, value, error, description="", icon="", placeholder="")
+mixin text_field(name, value, error, required="", description="", icon="", placeholder="")
   .field
-    +text_input(name, value, error=error, icon=icon, placeholder=placeholder)
+    +text_input(name, value, error=error, required=required, icon=icon, placeholder=placeholder)
     +error_message(error)
     +help_message(description)
 
-mixin number_field(name, value, error, description="", icon="", placeholder="")
+mixin number_field(name, value, error, required="", description="", icon="", placeholder="")
   .field
-    +number_input(name, value, error=error, icon=icon, placeholder=placeholder)
+    +number_input(name, value, error=error, required=required, icon=icon, placeholder=placeholder)
     +error_message(error)
     +help_message(description)
 
 // - -----------------------------------------------------------------------
 
 mixin render_field(field, icon="", placeholder="")
   - var required = ""
```

### Comparing `bl_hector-0.1.0a3/bl_hector/interfaces/to_http/as_html/templates/mixins/navbar.pug` & `bl_hector-0.1.0a4/bl_hector/interfaces/to_http/as_html/templates/mixins/navbar.pug`

 * *Files 2% similar despite different names*

```diff
@@ -33,15 +33,15 @@
       #navbarHector.navbar-menu
         .navbar-start
           a.navbar-item(href="#{url_for('books.search')}")= _("menu-books")
         .navbar-end
           .navbar-item
             .field.is-grouped
               //- Auth pages contains JS and should be properly loaded.
-              p.control(hx-boost="false")
+              p.control
                 if user.id
                   a.button.is-success.is-light(href="#{url_for('auth.logout')}")
                     span.icon: i.fa.fa-lock
                     span= _("menu-logout")
                 else
                   a.button.is-warning.is-light(href="#{url_for('auth.login')}")
                     span.icon: i.fa.fa-lock-open
```

### Comparing `bl_hector-0.1.0a3/bl_hector/interfaces/to_http/as_html/templates/webauthn/login.pug` & `bl_hector-0.1.0a4/bl_hector/interfaces/to_http/as_html/templates/webauthn/login.pug`

 * *Files identical despite different names*

### Comparing `bl_hector-0.1.0a3/bl_hector/interfaces/to_http/as_html/templates/webauthn/register.pug` & `bl_hector-0.1.0a4/bl_hector/interfaces/to_http/as_html/templates/webauthn/register.pug`

 * *Files identical despite different names*

### Comparing `bl_hector-0.1.0a3/bl_hector/interfaces/to_http/as_json/__init__.py` & `bl_hector-0.1.0a4/bl_hector/interfaces/to_http/as_json/__init__.py`

 * *Files identical despite different names*

### Comparing `bl_hector-0.1.0a3/bl_hector/interfaces/to_terminal/__init__.py` & `bl_hector-0.1.0a4/bl_hector/interfaces/to_terminal/__init__.py`

 * *Files identical despite different names*

### Comparing `bl_hector-0.1.0a3/bl_hector/interfaces/to_terminal/as_json.py` & `bl_hector-0.1.0a4/bl_hector/infrastructure/__init__.py`

 * *Files 22% similar despite different names*

```diff
@@ -10,41 +10,18 @@
 # but WITHOUT ANY WARRANTY; without even the implied warranty of
 # MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the
 # GNU Affero General Public License for more details.
 #
 # You should have received a copy of the GNU Affero General Public License
 # along with this program. If not, see <http://www.gnu.org/licenses/>.
 
-import json
-from typing import Callable
+from bl_hector.domain.administration.enumerations import Permissions as P
+from bl_hector.domain.administration.repositories import Permissions
+from bl_hector.domain.administration.value_objects import UserId
 
-from bl_hector.domain.collection_management.entities import Book
-from bl_hector.domain.collection_management.value_objects import Isbn
-from bl_hector.interfaces.to_terminal import ExitCodes, LookUpBookInterface
+ONLY_USER = "admin"
 
 
-class LookUpBook(LookUpBookInterface):
-    def __init__(self, printer: Callable[[str], None]) -> None:
-        self.__printer = printer
-        self.__exit_code = ExitCodes.USAGE
-
-    def not_an_isbn(self, isbn: str) -> None:
-        self.__exit_code = ExitCodes.BAD_REQUEST
-
-    def book_not_found(self, isbn: Isbn) -> None:
-        self.__exit_code = ExitCodes.NOT_FOUND
-
-    def book(self, book: Book) -> None:
-        self.__exit_code = ExitCodes.OK
-        data = {
-            "isbn": str(book.isbn),
-            "title": str(book.title),
-            "year": int(book.year),
-            "authors": [str(b) for b in book.authors],
-        }
-        if book.genres:
-            data["genres"] = [str(g) for g in book.genres]
-
-        self.__printer(json.dumps(data))
-
-    def exit_code(self) -> int:
-        return self.__exit_code.value
+class FakePermissions(Permissions):
+    def is_authorized_to(self, user_id: UserId, permission: P) -> bool:
+        print(repr(user_id))
+        return bool(str(user_id))
```

### Comparing `bl_hector-0.1.0a3/bl_hector/interfaces/to_terminal/as_text.py` & `bl_hector-0.1.0a4/bl_hector/interfaces/to_terminal/as_text.py`

 * *Files 2% similar despite different names*

```diff
@@ -67,15 +67,20 @@
         *,
         translator: Translator = DummyTranslator(),
     ) -> None:
         self.__printer = printer
         self.__exit_code = ExitCodes.USAGE
         self._ = translator
 
-    def bad_request(self) -> None:
+    def not_authorized(self) -> None:
+        self.__exit_code = ExitCodes.USAGE
+        self.__printer(self._("access-not-authorized"))
+
+    def bad_request(self, errors: add_book.Errors) -> None:
+        # TODO: display errors.
         self.__exit_code = ExitCodes.BAD_REQUEST
         self.__printer(self._("book-cannot-be-added"))
 
     def book_already_exists(self, book: Book) -> None:
         self.__exit_code = ExitCodes.BAD_REQUEST
         self.__printer(self._("book-already-exists"))
```

### Comparing `bl_hector-0.1.0a3/bl_hector/interfaces/utils.py` & `bl_hector-0.1.0a4/bl_hector/interfaces/utils.py`

 * *Files identical despite different names*

### Comparing `bl_hector-0.1.0a3/pyproject.toml` & `bl_hector-0.1.0a4/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "bl_hector"
-version = "0.1.0-alpha.3"
+version = "0.1.0-alpha.4"
 description = "A collection manager."
 authors = ["Tanguy Le Carrour <tanguy@bioneland.org>"]
 license = "AGPL-3.0-or-later"
 readme = "README.md"
 
 exclude = [
     "**/*_spec.py",
```

### Comparing `bl_hector-0.1.0a3/setup.py` & `bl_hector-0.1.0a4/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -55,15 +55,15 @@
 {'webauthn': ['webauthn>=1.8.1,<2.0.0']}
 
 entry_points = \
 {'console_scripts': ['hector = bl_hector.configuration.cli:cli']}
 
 setup_kwargs = {
     'name': 'bl-hector',
-    'version': '0.1.0a3',
+    'version': '0.1.0a4',
     'description': 'A collection manager.',
     'long_description': '# Hector — a collection manager\n\n## Install\n\nFor the time being, Hector cannot be installed from PyPI.\nSee [CONTRIBUTING.md]() to set up a development environment.\n\n\n## Configure\n\nHector is configured using environment variables.\nAll the variable names are prefixed with `HECTOR_`.\n\n```console\n$ export HECTOR_SECRET_KEY="XXXXXXXX-XXXX-XXXX-XXXX-XXXXXXXXXXXX"\n$ export HECTOR_DSN="sqlite:///data.sqlite"\n```\n\nThe secret can be generated using the `token_hex()` function from\nthe Python\'s `secrets` module.\n\nAdditional Python database drivers might be required depending on the DSN.\n\nSee [the `settings` module](bl_hector/infrastructure/settings.py) for\na comprehensive list of configuration variables.\n\n\n## Authentication\n\nTo enable WebAuthn authentication, you must install extra dependencies (`bl-hector[webauthn]`)\nand enable it explicitly:\n\n```console\n$ export HECTOR_WEBAUTHN=1\n```\n\n\n## Initialise\n\nOnce configured, you must initialise Hector\'s database with the dedicated command:\n\n```console\n$ hector init-db\n```\n\n\n## Run\n\nHector being a Flask application, it can be run using any WSGI server,\nfor instance, with [Gunicorn](https://gunicorn.org):\n\n```console\n$ gunicorn --access-logfile="-" -w 4 -b 127.0.0.1:3000 "bl_hector.configuration.wsgi:app()"\n```\n',
     'author': 'Tanguy Le Carrour',
     'author_email': 'tanguy@bioneland.org',
     'maintainer': None,
     'maintainer_email': None,
     'url': None,
```

### Comparing `bl_hector-0.1.0a3/PKG-INFO` & `bl_hector-0.1.0a4/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: bl-hector
-Version: 0.1.0a3
+Version: 0.1.0a4
 Summary: A collection manager.
 License: AGPL-3.0-or-later
 Author: Tanguy Le Carrour
 Author-email: tanguy@bioneland.org
 Requires-Python: >=3.9,<4.0
 Classifier: License :: OSI Approved :: GNU Affero General Public License v3 or later (AGPLv3+)
 Classifier: Programming Language :: Python :: 3
```

