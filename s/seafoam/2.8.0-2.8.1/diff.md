# Comparing `tmp/seafoam-2.8.0.tar.gz` & `tmp/seafoam-2.8.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "seafoam-2.8.0.tar", last modified: Sun Jun 11 17:23:18 2023, max compression
+gzip compressed data, was "seafoam-2.8.1.tar", last modified: Mon Jun 12 00:16:10 2023, max compression
```

## Comparing `seafoam-2.8.0.tar` & `seafoam-2.8.1.tar`

### file list

```diff
@@ -1,158 +1,158 @@
-drwxrwxrwx   0        0        0        0 2023-06-11 17:23:18.712158 seafoam-2.8.0/
--rw-rw-rw-   0        0        0     1133 2021-06-29 04:21:34.000000 seafoam-2.8.0/LICENSE.txt
--rw-rw-rw-   0        0        0      180 2021-07-05 16:41:31.000000 seafoam-2.8.0/MANIFEST.in
--rw-rw-rw-   0        0        0    30291 2023-06-11 17:23:18.713158 seafoam-2.8.0/PKG-INFO
--rw-rw-rw-   0        0        0    28868 2023-06-11 17:13:08.000000 seafoam-2.8.0/README.rst
-drwxrwxrwx   0        0        0        0 2023-06-11 17:23:16.071148 seafoam-2.8.0/docs/
--rw-rw-rw-   0        0        0     9471 2023-06-11 17:18:33.000000 seafoam-2.8.0/docs/CHANGELOG.rst
-drwxrwxrwx   0        0        0        0 2023-06-11 17:23:16.014664 seafoam-2.8.0/pelican/
-drwxrwxrwx   0        0        0        0 2023-06-11 17:23:16.015671 seafoam-2.8.0/pelican/plugins/
-drwxrwxrwx   0        0        0        0 2023-06-11 17:23:16.083126 seafoam-2.8.0/pelican/plugins/seafoam/
--rw-rw-rw-   0        0        0      829 2021-07-05 17:37:19.000000 seafoam-2.8.0/pelican/plugins/seafoam/__init__.py
--rw-rw-rw-   0        0        0      502 2023-06-11 17:23:00.000000 seafoam-2.8.0/pelican/plugins/seafoam/constants.py
--rw-rw-rw-   0        0        0     1005 2021-07-05 02:52:25.000000 seafoam-2.8.0/pelican/plugins/seafoam/formatting.py
--rw-rw-rw-   0        0        0     7606 2023-06-10 17:35:59.000000 seafoam-2.8.0/pelican/plugins/seafoam/initialize.py
-drwxrwxrwx   0        0        0        0 2023-06-11 17:23:16.021664 seafoam-2.8.0/pelican/plugins/seafoam/static/
-drwxrwxrwx   0        0        0        0 2023-06-11 17:23:16.089127 seafoam-2.8.0/pelican/plugins/seafoam/static/css/
--rw-rw-rw-   0        0        0   236354 2023-06-11 17:22:37.000000 seafoam-2.8.0/pelican/plugins/seafoam/static/css/bootstrap.seafoam.min.css
--rw-rw-rw-   0        0        0   235993 2023-06-11 17:22:40.000000 seafoam-2.8.0/pelican/plugins/seafoam/static/css/bootstrap.strathcona.min.css
-drwxrwxrwx   0        0        0        0 2023-06-11 17:23:16.293133 seafoam-2.8.0/pelican/plugins/seafoam/static/fonts/
--rw-rw-rw-   0        0        0   134808 2021-06-27 05:13:02.000000 seafoam-2.8.0/pelican/plugins/seafoam/static/fonts/FontAwesome.otf
-drwxrwxrwx   0        0        0        0 2023-06-11 17:23:16.708148 seafoam-2.8.0/pelican/plugins/seafoam/static/fonts/cabin/
--rw-rw-rw-   0        0        0     2104 2021-06-27 05:13:02.000000 seafoam-2.8.0/pelican/plugins/seafoam/static/fonts/cabin/FONTLOG.txt
--rw-rw-rw-   0        0        0     4460 2021-06-27 05:13:02.000000 seafoam-2.8.0/pelican/plugins/seafoam/static/fonts/cabin/OFL.txt
--rw-rw-rw-   0        0        0    18413 2023-06-10 17:35:59.000000 seafoam-2.8.0/pelican/plugins/seafoam/static/fonts/cabin/cabin-v26-latin-700.eot
--rw-rw-rw-   0        0        0    50449 2023-06-10 17:35:59.000000 seafoam-2.8.0/pelican/plugins/seafoam/static/fonts/cabin/cabin-v26-latin-700.svg
--rw-rw-rw-   0        0        0    35472 2023-06-10 17:35:59.000000 seafoam-2.8.0/pelican/plugins/seafoam/static/fonts/cabin/cabin-v26-latin-700.ttf
--rw-rw-rw-   0        0        0    19444 2023-06-10 17:35:59.000000 seafoam-2.8.0/pelican/plugins/seafoam/static/fonts/cabin/cabin-v26-latin-700.woff
--rw-rw-rw-   0        0        0    15168 2023-06-10 17:35:59.000000 seafoam-2.8.0/pelican/plugins/seafoam/static/fonts/cabin/cabin-v26-latin-700.woff2
--rw-rw-rw-   0        0        0    19294 2023-06-10 17:35:59.000000 seafoam-2.8.0/pelican/plugins/seafoam/static/fonts/cabin/cabin-v26-latin-700italic.eot
--rw-rw-rw-   0        0        0    56250 2023-06-10 17:35:59.000000 seafoam-2.8.0/pelican/plugins/seafoam/static/fonts/cabin/cabin-v26-latin-700italic.svg
--rw-rw-rw-   0        0        0    35176 2023-06-10 17:35:59.000000 seafoam-2.8.0/pelican/plugins/seafoam/static/fonts/cabin/cabin-v26-latin-700italic.ttf
--rw-rw-rw-   0        0        0    20280 2023-06-10 17:35:59.000000 seafoam-2.8.0/pelican/plugins/seafoam/static/fonts/cabin/cabin-v26-latin-700italic.woff
--rw-rw-rw-   0        0        0    15856 2023-06-10 17:35:59.000000 seafoam-2.8.0/pelican/plugins/seafoam/static/fonts/cabin/cabin-v26-latin-700italic.woff2
--rw-rw-rw-   0        0        0    19408 2023-06-10 17:35:59.000000 seafoam-2.8.0/pelican/plugins/seafoam/static/fonts/cabin/cabin-v26-latin-italic.eot
--rw-rw-rw-   0        0        0    56028 2023-06-10 17:35:59.000000 seafoam-2.8.0/pelican/plugins/seafoam/static/fonts/cabin/cabin-v26-latin-italic.svg
--rw-rw-rw-   0        0        0    35356 2023-06-10 17:35:59.000000 seafoam-2.8.0/pelican/plugins/seafoam/static/fonts/cabin/cabin-v26-latin-italic.ttf
--rw-rw-rw-   0        0        0    20416 2023-06-10 17:35:59.000000 seafoam-2.8.0/pelican/plugins/seafoam/static/fonts/cabin/cabin-v26-latin-italic.woff
--rw-rw-rw-   0        0        0    16020 2023-06-10 17:35:59.000000 seafoam-2.8.0/pelican/plugins/seafoam/static/fonts/cabin/cabin-v26-latin-italic.woff2
--rw-rw-rw-   0        0        0    18842 2023-06-10 17:35:59.000000 seafoam-2.8.0/pelican/plugins/seafoam/static/fonts/cabin/cabin-v26-latin-regular.eot
--rw-rw-rw-   0        0        0    50436 2023-06-10 17:35:59.000000 seafoam-2.8.0/pelican/plugins/seafoam/static/fonts/cabin/cabin-v26-latin-regular.svg
--rw-rw-rw-   0        0        0    35700 2023-06-10 17:35:59.000000 seafoam-2.8.0/pelican/plugins/seafoam/static/fonts/cabin/cabin-v26-latin-regular.ttf
--rw-rw-rw-   0        0        0    19916 2023-06-10 17:35:59.000000 seafoam-2.8.0/pelican/plugins/seafoam/static/fonts/cabin/cabin-v26-latin-regular.woff
--rw-rw-rw-   0        0        0    15476 2023-06-10 17:35:59.000000 seafoam-2.8.0/pelican/plugins/seafoam/static/fonts/cabin/cabin-v26-latin-regular.woff2
-drwxrwxrwx   0        0        0        0 2023-06-11 17:23:17.143122 seafoam-2.8.0/pelican/plugins/seafoam/static/fonts/eb-garamond/
--rw-rw-rw-   0        0        0    24884 2023-06-10 17:35:59.000000 seafoam-2.8.0/pelican/plugins/seafoam/static/fonts/eb-garamond/eb-garamond-v26-latin-700.eot
--rw-rw-rw-   0        0        0   128830 2023-06-10 17:35:59.000000 seafoam-2.8.0/pelican/plugins/seafoam/static/fonts/eb-garamond/eb-garamond-v26-latin-700.svg
--rw-rw-rw-   0        0        0    49124 2023-06-10 17:35:59.000000 seafoam-2.8.0/pelican/plugins/seafoam/static/fonts/eb-garamond/eb-garamond-v26-latin-700.ttf
--rw-rw-rw-   0        0        0    25788 2023-06-10 17:35:59.000000 seafoam-2.8.0/pelican/plugins/seafoam/static/fonts/eb-garamond/eb-garamond-v26-latin-700.woff
--rw-rw-rw-   0        0        0    21932 2023-06-10 17:35:59.000000 seafoam-2.8.0/pelican/plugins/seafoam/static/fonts/eb-garamond/eb-garamond-v26-latin-700.woff2
--rw-rw-rw-   0        0        0    25468 2023-06-10 17:35:59.000000 seafoam-2.8.0/pelican/plugins/seafoam/static/fonts/eb-garamond/eb-garamond-v26-latin-700italic.eot
--rw-rw-rw-   0        0        0   128299 2023-06-10 17:35:59.000000 seafoam-2.8.0/pelican/plugins/seafoam/static/fonts/eb-garamond/eb-garamond-v26-latin-700italic.svg
--rw-rw-rw-   0        0        0    47480 2023-06-10 17:35:59.000000 seafoam-2.8.0/pelican/plugins/seafoam/static/fonts/eb-garamond/eb-garamond-v26-latin-700italic.ttf
--rw-rw-rw-   0        0        0    26508 2023-06-10 17:35:59.000000 seafoam-2.8.0/pelican/plugins/seafoam/static/fonts/eb-garamond/eb-garamond-v26-latin-700italic.woff
--rw-rw-rw-   0        0        0    22480 2023-06-10 17:35:59.000000 seafoam-2.8.0/pelican/plugins/seafoam/static/fonts/eb-garamond/eb-garamond-v26-latin-700italic.woff2
--rw-rw-rw-   0        0        0    23567 2023-06-10 17:35:59.000000 seafoam-2.8.0/pelican/plugins/seafoam/static/fonts/eb-garamond/eb-garamond-v26-latin-italic.eot
--rw-rw-rw-   0        0        0   127687 2023-06-10 17:35:59.000000 seafoam-2.8.0/pelican/plugins/seafoam/static/fonts/eb-garamond/eb-garamond-v26-latin-italic.svg
--rw-rw-rw-   0        0        0    47032 2023-06-10 17:35:59.000000 seafoam-2.8.0/pelican/plugins/seafoam/static/fonts/eb-garamond/eb-garamond-v26-latin-italic.ttf
--rw-rw-rw-   0        0        0    24808 2023-06-10 17:35:59.000000 seafoam-2.8.0/pelican/plugins/seafoam/static/fonts/eb-garamond/eb-garamond-v26-latin-italic.woff
--rw-rw-rw-   0        0        0    21020 2023-06-10 17:35:59.000000 seafoam-2.8.0/pelican/plugins/seafoam/static/fonts/eb-garamond/eb-garamond-v26-latin-italic.woff2
--rw-rw-rw-   0        0        0    23239 2023-06-10 17:35:59.000000 seafoam-2.8.0/pelican/plugins/seafoam/static/fonts/eb-garamond/eb-garamond-v26-latin-regular.eot
--rw-rw-rw-   0        0        0   128551 2023-06-10 17:35:59.000000 seafoam-2.8.0/pelican/plugins/seafoam/static/fonts/eb-garamond/eb-garamond-v26-latin-regular.svg
--rw-rw-rw-   0        0        0    48900 2023-06-10 17:35:59.000000 seafoam-2.8.0/pelican/plugins/seafoam/static/fonts/eb-garamond/eb-garamond-v26-latin-regular.ttf
--rw-rw-rw-   0        0        0    24304 2023-06-10 17:35:59.000000 seafoam-2.8.0/pelican/plugins/seafoam/static/fonts/eb-garamond/eb-garamond-v26-latin-regular.woff
--rw-rw-rw-   0        0        0    20512 2023-06-10 17:35:59.000000 seafoam-2.8.0/pelican/plugins/seafoam/static/fonts/eb-garamond/eb-garamond-v26-latin-regular.woff2
-drwxrwxrwx   0        0        0        0 2023-06-11 17:23:17.245128 seafoam-2.8.0/pelican/plugins/seafoam/static/fonts/expletus-sans/
--rw-rw-rw-   0        0        0     4499 2021-06-27 05:13:02.000000 seafoam-2.8.0/pelican/plugins/seafoam/static/fonts/expletus-sans/OFL.txt
--rw-rw-rw-   0        0        0    11207 2023-06-10 17:35:59.000000 seafoam-2.8.0/pelican/plugins/seafoam/static/fonts/expletus-sans/expletus-sans-v24-latin-500.eot
--rw-rw-rw-   0        0        0    60057 2023-06-10 17:35:59.000000 seafoam-2.8.0/pelican/plugins/seafoam/static/fonts/expletus-sans/expletus-sans-v24-latin-500.svg
--rw-rw-rw-   0        0        0    18564 2023-06-10 17:35:59.000000 seafoam-2.8.0/pelican/plugins/seafoam/static/fonts/expletus-sans/expletus-sans-v24-latin-500.ttf
--rw-rw-rw-   0        0        0    13008 2023-06-10 17:35:59.000000 seafoam-2.8.0/pelican/plugins/seafoam/static/fonts/expletus-sans/expletus-sans-v24-latin-500.woff
--rw-rw-rw-   0        0        0    10084 2023-06-10 17:35:59.000000 seafoam-2.8.0/pelican/plugins/seafoam/static/fonts/expletus-sans/expletus-sans-v24-latin-500.woff2
--rw-rw-rw-   0        0        0   165742 2021-06-27 05:13:02.000000 seafoam-2.8.0/pelican/plugins/seafoam/static/fonts/fontawesome-webfont.eot
--rw-rw-rw-   0        0        0   447050 2021-06-27 05:13:02.000000 seafoam-2.8.0/pelican/plugins/seafoam/static/fonts/fontawesome-webfont.svg
--rw-rw-rw-   0        0        0   165548 2021-06-27 05:13:02.000000 seafoam-2.8.0/pelican/plugins/seafoam/static/fonts/fontawesome-webfont.ttf
--rw-rw-rw-   0        0        0    98024 2021-06-27 05:13:02.000000 seafoam-2.8.0/pelican/plugins/seafoam/static/fonts/fontawesome-webfont.woff
--rw-rw-rw-   0        0        0    77160 2021-06-27 05:13:02.000000 seafoam-2.8.0/pelican/plugins/seafoam/static/fonts/fontawesome-webfont.woff2
--rw-rw-rw-   0        0        0    20127 2021-06-27 05:13:02.000000 seafoam-2.8.0/pelican/plugins/seafoam/static/fonts/glyphicons-halflings-regular.eot
--rw-rw-rw-   0        0        0   109025 2021-06-27 05:13:02.000000 seafoam-2.8.0/pelican/plugins/seafoam/static/fonts/glyphicons-halflings-regular.svg
--rw-rw-rw-   0        0        0    45404 2021-06-27 05:13:02.000000 seafoam-2.8.0/pelican/plugins/seafoam/static/fonts/glyphicons-halflings-regular.ttf
--rw-rw-rw-   0        0        0    23424 2021-06-27 05:13:02.000000 seafoam-2.8.0/pelican/plugins/seafoam/static/fonts/glyphicons-halflings-regular.woff
--rw-rw-rw-   0        0        0    18028 2021-06-27 05:13:02.000000 seafoam-2.8.0/pelican/plugins/seafoam/static/fonts/glyphicons-halflings-regular.woff2
-drwxrwxrwx   0        0        0        0 2023-06-11 17:23:17.346127 seafoam-2.8.0/pelican/plugins/seafoam/static/fonts/vidaloka/
--rw-rw-rw-   0        0        0    30028 2023-06-10 17:35:59.000000 seafoam-2.8.0/pelican/plugins/seafoam/static/fonts/vidaloka/vidaloka-v18-latin-regular.eot
--rw-rw-rw-   0        0        0    81305 2023-06-10 17:35:59.000000 seafoam-2.8.0/pelican/plugins/seafoam/static/fonts/vidaloka/vidaloka-v18-latin-regular.svg
--rw-rw-rw-   0        0        0    78804 2023-06-10 17:35:59.000000 seafoam-2.8.0/pelican/plugins/seafoam/static/fonts/vidaloka/vidaloka-v18-latin-regular.ttf
--rw-rw-rw-   0        0        0    36788 2023-06-10 17:35:59.000000 seafoam-2.8.0/pelican/plugins/seafoam/static/fonts/vidaloka/vidaloka-v18-latin-regular.woff
--rw-rw-rw-   0        0        0    30116 2023-06-10 17:35:59.000000 seafoam-2.8.0/pelican/plugins/seafoam/static/fonts/vidaloka/vidaloka-v18-latin-regular.woff2
-drwxrwxrwx   0        0        0        0 2023-06-11 17:23:17.712122 seafoam-2.8.0/pelican/plugins/seafoam/static/js/
--rw-rw-rw-   0        0        0    72084 2021-06-27 05:13:02.000000 seafoam-2.8.0/pelican/plugins/seafoam/static/js/bootstrap.js
--rw-rw-rw-   0        0        0    37051 2021-06-27 05:13:02.000000 seafoam-2.8.0/pelican/plugins/seafoam/static/js/bootstrap.min.js
--rw-rw-rw-   0        0        0     2512 2021-06-27 05:13:02.000000 seafoam-2.8.0/pelican/plugins/seafoam/static/js/comments.js
--rw-rw-rw-   0        0        0     1520 2021-06-27 05:13:02.000000 seafoam-2.8.0/pelican/plugins/seafoam/static/js/github.js
--rw-rw-rw-   0        0        0     2558 2021-06-27 05:13:02.000000 seafoam-2.8.0/pelican/plugins/seafoam/static/js/jXHR.js
--rw-rw-rw-   0        0        0    86713 2021-06-27 05:13:02.000000 seafoam-2.8.0/pelican/plugins/seafoam/static/js/jquery.min.js
--rw-rw-rw-   0        0        0     4381 2021-06-27 05:13:02.000000 seafoam-2.8.0/pelican/plugins/seafoam/static/js/respond.min.js
-drwxrwxrwx   0        0        0        0 2023-06-11 17:23:17.870121 seafoam-2.8.0/pelican/plugins/seafoam/static/tipuesearch/
-drwxrwxrwx   0        0        0        0 2023-06-11 17:23:17.873127 seafoam-2.8.0/pelican/plugins/seafoam/static/tipuesearch/img/
--rw-rw-rw-   0        0        0      368 2021-06-27 05:13:02.000000 seafoam-2.8.0/pelican/plugins/seafoam/static/tipuesearch/img/search.png
--rw-rw-rw-   0        0        0     5734 2021-06-27 05:13:02.000000 seafoam-2.8.0/pelican/plugins/seafoam/static/tipuesearch/tipuesearch.css
--rw-rw-rw-   0        0        0    33779 2021-06-27 05:13:02.000000 seafoam-2.8.0/pelican/plugins/seafoam/static/tipuesearch/tipuesearch.js
--rw-rw-rw-   0        0        0    10697 2021-06-27 05:13:02.000000 seafoam-2.8.0/pelican/plugins/seafoam/static/tipuesearch/tipuesearch.min.js
--rw-rw-rw-   0        0        0     4537 2021-06-27 05:13:02.000000 seafoam-2.8.0/pelican/plugins/seafoam/static/tipuesearch/tipuesearch_content.js
--rw-rw-rw-   0        0        0     3670 2021-06-27 05:13:02.000000 seafoam-2.8.0/pelican/plugins/seafoam/static/tipuesearch/tipuesearch_set.js
-drwxrwxrwx   0        0        0        0 2023-06-11 17:23:18.128147 seafoam-2.8.0/pelican/plugins/seafoam/templates/
--rw-rw-rw-   0        0        0     1110 2021-06-27 05:13:02.000000 seafoam-2.8.0/pelican/plugins/seafoam/templates/404.html
--rw-rw-rw-   0        0        0     5399 2021-06-27 05:13:02.000000 seafoam-2.8.0/pelican/plugins/seafoam/templates/archives.html
--rw-rw-rw-   0        0        0     4597 2021-06-27 05:13:02.000000 seafoam-2.8.0/pelican/plugins/seafoam/templates/article.html
--rw-rw-rw-   0        0        0     1508 2021-06-27 05:13:02.000000 seafoam-2.8.0/pelican/plugins/seafoam/templates/article_list.html
--rw-rw-rw-   0        0        0      761 2021-06-27 05:13:02.000000 seafoam-2.8.0/pelican/plugins/seafoam/templates/author.html
--rw-rw-rw-   0        0        0      857 2021-06-27 05:13:02.000000 seafoam-2.8.0/pelican/plugins/seafoam/templates/authors.html
--rw-rw-rw-   0        0        0    14081 2023-06-10 17:35:59.000000 seafoam-2.8.0/pelican/plugins/seafoam/templates/base.html
--rw-rw-rw-   0        0        0     2053 2021-06-27 05:13:02.000000 seafoam-2.8.0/pelican/plugins/seafoam/templates/categories.html
--rw-rw-rw-   0        0        0      738 2021-06-27 05:13:02.000000 seafoam-2.8.0/pelican/plugins/seafoam/templates/category.html
-drwxrwxrwx   0        0        0        0 2023-06-11 17:23:18.616127 seafoam-2.8.0/pelican/plugins/seafoam/templates/includes/
--rw-rw-rw-   0        0        0      196 2021-06-27 05:13:02.000000 seafoam-2.8.0/pelican/plugins/seafoam/templates/includes/aboutme.html
--rw-rw-rw-   0        0        0      618 2023-06-10 17:35:59.000000 seafoam-2.8.0/pelican/plugins/seafoam/templates/includes/addthis.html
--rw-rw-rw-   0        0        0     1481 2021-06-27 05:13:02.000000 seafoam-2.8.0/pelican/plugins/seafoam/templates/includes/article_info.html
--rw-rw-rw-   0        0        0     2665 2023-06-10 17:35:59.000000 seafoam-2.8.0/pelican/plugins/seafoam/templates/includes/article_listing.html
--rw-rw-rw-   0        0        0      978 2021-06-27 05:13:02.000000 seafoam-2.8.0/pelican/plugins/seafoam/templates/includes/assets-css.html
--rw-rw-rw-   0        0        0      219 2021-06-27 05:13:02.000000 seafoam-2.8.0/pelican/plugins/seafoam/templates/includes/assets-js.html
--rw-rw-rw-   0        0        0     4405 2021-06-27 05:13:02.000000 seafoam-2.8.0/pelican/plugins/seafoam/templates/includes/cc-license.html
--rw-rw-rw-   0        0        0      553 2021-06-27 05:13:02.000000 seafoam-2.8.0/pelican/plugins/seafoam/templates/includes/comment_count.html
--rw-rw-rw-   0        0        0     1291 2021-06-27 05:13:02.000000 seafoam-2.8.0/pelican/plugins/seafoam/templates/includes/comments-js.html
--rw-rw-rw-   0        0        0     5874 2022-04-30 21:08:37.000000 seafoam-2.8.0/pelican/plugins/seafoam/templates/includes/comments.html
--rw-rw-rw-   0        0        0      741 2021-06-27 05:13:02.000000 seafoam-2.8.0/pelican/plugins/seafoam/templates/includes/disqus_script.html
--rw-rw-rw-   0        0        0     3364 2021-06-29 04:36:51.000000 seafoam-2.8.0/pelican/plugins/seafoam/templates/includes/footer.html
--rw-rw-rw-   0        0        0     1818 2023-06-10 17:44:17.000000 seafoam-2.8.0/pelican/plugins/seafoam/templates/includes/ga.html
--rw-rw-rw-   0        0        0     1308 2023-06-10 17:35:59.000000 seafoam-2.8.0/pelican/plugins/seafoam/templates/includes/github-js.html
--rw-rw-rw-   0        0        0      442 2023-06-10 17:35:59.000000 seafoam-2.8.0/pelican/plugins/seafoam/templates/includes/github.html
--rw-rw-rw-   0        0        0      434 2023-06-10 17:35:59.000000 seafoam-2.8.0/pelican/plugins/seafoam/templates/includes/links.html
--rw-rw-rw-   0        0        0     1991 2022-03-21 04:06:10.000000 seafoam-2.8.0/pelican/plugins/seafoam/templates/includes/neighbors.html
--rw-rw-rw-   0        0        0     2955 2021-06-27 05:13:02.000000 seafoam-2.8.0/pelican/plugins/seafoam/templates/includes/pagination.html
--rw-rw-rw-   0        0        0      872 2023-06-10 17:35:59.000000 seafoam-2.8.0/pelican/plugins/seafoam/templates/includes/piwik.html
--rw-rw-rw-   0        0        0      486 2021-06-27 05:13:02.000000 seafoam-2.8.0/pelican/plugins/seafoam/templates/includes/prjct.html
--rw-rw-rw-   0        0        0      357 2021-06-27 05:13:02.000000 seafoam-2.8.0/pelican/plugins/seafoam/templates/includes/related-posts.html
--rw-rw-rw-   0        0        0     3520 2021-10-24 02:08:02.000000 seafoam-2.8.0/pelican/plugins/seafoam/templates/includes/sidebar.html
--rw-rw-rw-   0        0        0      276 2021-06-27 05:13:02.000000 seafoam-2.8.0/pelican/plugins/seafoam/templates/includes/taglist.html
--rw-rw-rw-   0        0        0      296 2023-06-10 17:35:59.000000 seafoam-2.8.0/pelican/plugins/seafoam/templates/includes/translations.html
--rw-rw-rw-   0        0        0      703 2023-06-10 17:35:59.000000 seafoam-2.8.0/pelican/plugins/seafoam/templates/includes/twitter_timeline.html
--rw-rw-rw-   0        0        0      808 2023-06-10 17:35:59.000000 seafoam-2.8.0/pelican/plugins/seafoam/templates/index.html
--rw-rw-rw-   0        0        0     2473 2023-06-10 17:35:59.000000 seafoam-2.8.0/pelican/plugins/seafoam/templates/page.html
--rw-rw-rw-   0        0        0     7104 2021-06-27 05:13:02.000000 seafoam-2.8.0/pelican/plugins/seafoam/templates/period_archives.html
--rw-rw-rw-   0        0        0     4517 2021-06-27 05:13:02.000000 seafoam-2.8.0/pelican/plugins/seafoam/templates/prjct.html
--rw-rw-rw-   0        0        0     1507 2021-06-27 05:13:02.000000 seafoam-2.8.0/pelican/plugins/seafoam/templates/search.html
-drwxrwxrwx   0        0        0        0 2023-06-11 17:23:18.647159 seafoam-2.8.0/pelican/plugins/seafoam/templates/strathcona/
--rw-rw-rw-   0        0        0     8939 2023-06-10 17:35:59.000000 seafoam-2.8.0/pelican/plugins/seafoam/templates/strathcona/dual_pricing.html
--rw-rw-rw-   0        0        0     5443 2023-06-10 17:35:59.000000 seafoam-2.8.0/pelican/plugins/seafoam/templates/strathcona/pricing.html
--rw-rw-rw-   0        0        0      795 2021-10-24 02:08:02.000000 seafoam-2.8.0/pelican/plugins/seafoam/templates/tag.html
--rw-rw-rw-   0        0        0     2036 2021-10-24 02:08:02.000000 seafoam-2.8.0/pelican/plugins/seafoam/templates/tags.html
--rw-rw-rw-   0        0        0      429 2022-03-21 04:06:10.000000 seafoam-2.8.0/pyproject.toml
-drwxrwxrwx   0        0        0        0 2023-06-11 17:23:18.710158 seafoam-2.8.0/seafoam.egg-info/
--rw-rw-rw-   0        0        0    30291 2023-06-11 17:23:14.000000 seafoam-2.8.0/seafoam.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0     8286 2023-06-11 17:23:15.000000 seafoam-2.8.0/seafoam.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-06-11 17:23:14.000000 seafoam-2.8.0/seafoam.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0      235 2023-06-11 17:23:15.000000 seafoam-2.8.0/seafoam.egg-info/requires.txt
--rw-rw-rw-   0        0        0       41 2023-06-11 17:23:15.000000 seafoam-2.8.0/seafoam.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       74 2023-06-11 17:23:18.717167 seafoam-2.8.0/setup.cfg
--rw-rw-rw-   0        0        0     4767 2023-06-10 17:35:59.000000 seafoam-2.8.0/setup.py
+drwxrwxrwx   0        0        0        0 2023-06-12 00:16:10.708976 seafoam-2.8.1/
+-rw-rw-rw-   0        0        0     1133 2021-06-29 04:21:34.000000 seafoam-2.8.1/LICENSE.txt
+-rw-rw-rw-   0        0        0      180 2021-07-05 16:41:31.000000 seafoam-2.8.1/MANIFEST.in
+-rw-rw-rw-   0        0        0    30291 2023-06-12 00:16:10.709977 seafoam-2.8.1/PKG-INFO
+-rw-rw-rw-   0        0        0    28868 2023-06-11 23:27:14.000000 seafoam-2.8.1/README.rst
+drwxrwxrwx   0        0        0        0 2023-06-12 00:16:10.445990 seafoam-2.8.1/docs/
+-rw-rw-rw-   0        0        0     9539 2023-06-11 23:49:16.000000 seafoam-2.8.1/docs/CHANGELOG.rst
+drwxrwxrwx   0        0        0        0 2023-06-12 00:16:10.382944 seafoam-2.8.1/pelican/
+drwxrwxrwx   0        0        0        0 2023-06-12 00:16:10.383946 seafoam-2.8.1/pelican/plugins/
+drwxrwxrwx   0        0        0        0 2023-06-12 00:16:10.454987 seafoam-2.8.1/pelican/plugins/seafoam/
+-rw-rw-rw-   0        0        0      829 2021-07-05 17:37:19.000000 seafoam-2.8.1/pelican/plugins/seafoam/__init__.py
+-rw-rw-rw-   0        0        0      502 2023-06-12 00:16:05.000000 seafoam-2.8.1/pelican/plugins/seafoam/constants.py
+-rw-rw-rw-   0        0        0     1005 2021-07-05 02:52:25.000000 seafoam-2.8.1/pelican/plugins/seafoam/formatting.py
+-rw-rw-rw-   0        0        0     7606 2023-06-10 17:35:59.000000 seafoam-2.8.1/pelican/plugins/seafoam/initialize.py
+drwxrwxrwx   0        0        0        0 2023-06-12 00:16:10.388948 seafoam-2.8.1/pelican/plugins/seafoam/static/
+drwxrwxrwx   0        0        0        0 2023-06-12 00:16:10.458984 seafoam-2.8.1/pelican/plugins/seafoam/static/css/
+-rw-rw-rw-   0        0        0   236390 2023-06-11 23:48:08.000000 seafoam-2.8.1/pelican/plugins/seafoam/static/css/bootstrap.seafoam.min.css
+-rw-rw-rw-   0        0        0   235993 2023-06-11 23:48:09.000000 seafoam-2.8.1/pelican/plugins/seafoam/static/css/bootstrap.strathcona.min.css
+drwxrwxrwx   0        0        0        0 2023-06-12 00:16:10.479979 seafoam-2.8.1/pelican/plugins/seafoam/static/fonts/
+-rw-rw-rw-   0        0        0   134808 2021-06-27 05:13:02.000000 seafoam-2.8.1/pelican/plugins/seafoam/static/fonts/FontAwesome.otf
+drwxrwxrwx   0        0        0        0 2023-06-12 00:16:10.520980 seafoam-2.8.1/pelican/plugins/seafoam/static/fonts/cabin/
+-rw-rw-rw-   0        0        0     2104 2021-06-27 05:13:02.000000 seafoam-2.8.1/pelican/plugins/seafoam/static/fonts/cabin/FONTLOG.txt
+-rw-rw-rw-   0        0        0     4460 2021-06-27 05:13:02.000000 seafoam-2.8.1/pelican/plugins/seafoam/static/fonts/cabin/OFL.txt
+-rw-rw-rw-   0        0        0    18413 2023-06-10 17:35:59.000000 seafoam-2.8.1/pelican/plugins/seafoam/static/fonts/cabin/cabin-v26-latin-700.eot
+-rw-rw-rw-   0        0        0    50449 2023-06-10 17:35:59.000000 seafoam-2.8.1/pelican/plugins/seafoam/static/fonts/cabin/cabin-v26-latin-700.svg
+-rw-rw-rw-   0        0        0    35472 2023-06-10 17:35:59.000000 seafoam-2.8.1/pelican/plugins/seafoam/static/fonts/cabin/cabin-v26-latin-700.ttf
+-rw-rw-rw-   0        0        0    19444 2023-06-10 17:35:59.000000 seafoam-2.8.1/pelican/plugins/seafoam/static/fonts/cabin/cabin-v26-latin-700.woff
+-rw-rw-rw-   0        0        0    15168 2023-06-10 17:35:59.000000 seafoam-2.8.1/pelican/plugins/seafoam/static/fonts/cabin/cabin-v26-latin-700.woff2
+-rw-rw-rw-   0        0        0    19294 2023-06-10 17:35:59.000000 seafoam-2.8.1/pelican/plugins/seafoam/static/fonts/cabin/cabin-v26-latin-700italic.eot
+-rw-rw-rw-   0        0        0    56250 2023-06-10 17:35:59.000000 seafoam-2.8.1/pelican/plugins/seafoam/static/fonts/cabin/cabin-v26-latin-700italic.svg
+-rw-rw-rw-   0        0        0    35176 2023-06-10 17:35:59.000000 seafoam-2.8.1/pelican/plugins/seafoam/static/fonts/cabin/cabin-v26-latin-700italic.ttf
+-rw-rw-rw-   0        0        0    20280 2023-06-10 17:35:59.000000 seafoam-2.8.1/pelican/plugins/seafoam/static/fonts/cabin/cabin-v26-latin-700italic.woff
+-rw-rw-rw-   0        0        0    15856 2023-06-10 17:35:59.000000 seafoam-2.8.1/pelican/plugins/seafoam/static/fonts/cabin/cabin-v26-latin-700italic.woff2
+-rw-rw-rw-   0        0        0    19408 2023-06-10 17:35:59.000000 seafoam-2.8.1/pelican/plugins/seafoam/static/fonts/cabin/cabin-v26-latin-italic.eot
+-rw-rw-rw-   0        0        0    56028 2023-06-10 17:35:59.000000 seafoam-2.8.1/pelican/plugins/seafoam/static/fonts/cabin/cabin-v26-latin-italic.svg
+-rw-rw-rw-   0        0        0    35356 2023-06-10 17:35:59.000000 seafoam-2.8.1/pelican/plugins/seafoam/static/fonts/cabin/cabin-v26-latin-italic.ttf
+-rw-rw-rw-   0        0        0    20416 2023-06-10 17:35:59.000000 seafoam-2.8.1/pelican/plugins/seafoam/static/fonts/cabin/cabin-v26-latin-italic.woff
+-rw-rw-rw-   0        0        0    16020 2023-06-10 17:35:59.000000 seafoam-2.8.1/pelican/plugins/seafoam/static/fonts/cabin/cabin-v26-latin-italic.woff2
+-rw-rw-rw-   0        0        0    18842 2023-06-10 17:35:59.000000 seafoam-2.8.1/pelican/plugins/seafoam/static/fonts/cabin/cabin-v26-latin-regular.eot
+-rw-rw-rw-   0        0        0    50436 2023-06-10 17:35:59.000000 seafoam-2.8.1/pelican/plugins/seafoam/static/fonts/cabin/cabin-v26-latin-regular.svg
+-rw-rw-rw-   0        0        0    35700 2023-06-10 17:35:59.000000 seafoam-2.8.1/pelican/plugins/seafoam/static/fonts/cabin/cabin-v26-latin-regular.ttf
+-rw-rw-rw-   0        0        0    19916 2023-06-10 17:35:59.000000 seafoam-2.8.1/pelican/plugins/seafoam/static/fonts/cabin/cabin-v26-latin-regular.woff
+-rw-rw-rw-   0        0        0    15476 2023-06-10 17:35:59.000000 seafoam-2.8.1/pelican/plugins/seafoam/static/fonts/cabin/cabin-v26-latin-regular.woff2
+drwxrwxrwx   0        0        0        0 2023-06-12 00:16:10.555978 seafoam-2.8.1/pelican/plugins/seafoam/static/fonts/eb-garamond/
+-rw-rw-rw-   0        0        0    24884 2023-06-10 17:35:59.000000 seafoam-2.8.1/pelican/plugins/seafoam/static/fonts/eb-garamond/eb-garamond-v26-latin-700.eot
+-rw-rw-rw-   0        0        0   128830 2023-06-10 17:35:59.000000 seafoam-2.8.1/pelican/plugins/seafoam/static/fonts/eb-garamond/eb-garamond-v26-latin-700.svg
+-rw-rw-rw-   0        0        0    49124 2023-06-10 17:35:59.000000 seafoam-2.8.1/pelican/plugins/seafoam/static/fonts/eb-garamond/eb-garamond-v26-latin-700.ttf
+-rw-rw-rw-   0        0        0    25788 2023-06-10 17:35:59.000000 seafoam-2.8.1/pelican/plugins/seafoam/static/fonts/eb-garamond/eb-garamond-v26-latin-700.woff
+-rw-rw-rw-   0        0        0    21932 2023-06-10 17:35:59.000000 seafoam-2.8.1/pelican/plugins/seafoam/static/fonts/eb-garamond/eb-garamond-v26-latin-700.woff2
+-rw-rw-rw-   0        0        0    25468 2023-06-10 17:35:59.000000 seafoam-2.8.1/pelican/plugins/seafoam/static/fonts/eb-garamond/eb-garamond-v26-latin-700italic.eot
+-rw-rw-rw-   0        0        0   128299 2023-06-10 17:35:59.000000 seafoam-2.8.1/pelican/plugins/seafoam/static/fonts/eb-garamond/eb-garamond-v26-latin-700italic.svg
+-rw-rw-rw-   0        0        0    47480 2023-06-10 17:35:59.000000 seafoam-2.8.1/pelican/plugins/seafoam/static/fonts/eb-garamond/eb-garamond-v26-latin-700italic.ttf
+-rw-rw-rw-   0        0        0    26508 2023-06-10 17:35:59.000000 seafoam-2.8.1/pelican/plugins/seafoam/static/fonts/eb-garamond/eb-garamond-v26-latin-700italic.woff
+-rw-rw-rw-   0        0        0    22480 2023-06-10 17:35:59.000000 seafoam-2.8.1/pelican/plugins/seafoam/static/fonts/eb-garamond/eb-garamond-v26-latin-700italic.woff2
+-rw-rw-rw-   0        0        0    23567 2023-06-10 17:35:59.000000 seafoam-2.8.1/pelican/plugins/seafoam/static/fonts/eb-garamond/eb-garamond-v26-latin-italic.eot
+-rw-rw-rw-   0        0        0   127687 2023-06-10 17:35:59.000000 seafoam-2.8.1/pelican/plugins/seafoam/static/fonts/eb-garamond/eb-garamond-v26-latin-italic.svg
+-rw-rw-rw-   0        0        0    47032 2023-06-10 17:35:59.000000 seafoam-2.8.1/pelican/plugins/seafoam/static/fonts/eb-garamond/eb-garamond-v26-latin-italic.ttf
+-rw-rw-rw-   0        0        0    24808 2023-06-10 17:35:59.000000 seafoam-2.8.1/pelican/plugins/seafoam/static/fonts/eb-garamond/eb-garamond-v26-latin-italic.woff
+-rw-rw-rw-   0        0        0    21020 2023-06-10 17:35:59.000000 seafoam-2.8.1/pelican/plugins/seafoam/static/fonts/eb-garamond/eb-garamond-v26-latin-italic.woff2
+-rw-rw-rw-   0        0        0    23239 2023-06-10 17:35:59.000000 seafoam-2.8.1/pelican/plugins/seafoam/static/fonts/eb-garamond/eb-garamond-v26-latin-regular.eot
+-rw-rw-rw-   0        0        0   128551 2023-06-10 17:35:59.000000 seafoam-2.8.1/pelican/plugins/seafoam/static/fonts/eb-garamond/eb-garamond-v26-latin-regular.svg
+-rw-rw-rw-   0        0        0    48900 2023-06-10 17:35:59.000000 seafoam-2.8.1/pelican/plugins/seafoam/static/fonts/eb-garamond/eb-garamond-v26-latin-regular.ttf
+-rw-rw-rw-   0        0        0    24304 2023-06-10 17:35:59.000000 seafoam-2.8.1/pelican/plugins/seafoam/static/fonts/eb-garamond/eb-garamond-v26-latin-regular.woff
+-rw-rw-rw-   0        0        0    20512 2023-06-10 17:35:59.000000 seafoam-2.8.1/pelican/plugins/seafoam/static/fonts/eb-garamond/eb-garamond-v26-latin-regular.woff2
+drwxrwxrwx   0        0        0        0 2023-06-12 00:16:10.565976 seafoam-2.8.1/pelican/plugins/seafoam/static/fonts/expletus-sans/
+-rw-rw-rw-   0        0        0     4499 2021-06-27 05:13:02.000000 seafoam-2.8.1/pelican/plugins/seafoam/static/fonts/expletus-sans/OFL.txt
+-rw-rw-rw-   0        0        0    11207 2023-06-10 17:35:59.000000 seafoam-2.8.1/pelican/plugins/seafoam/static/fonts/expletus-sans/expletus-sans-v24-latin-500.eot
+-rw-rw-rw-   0        0        0    60057 2023-06-10 17:35:59.000000 seafoam-2.8.1/pelican/plugins/seafoam/static/fonts/expletus-sans/expletus-sans-v24-latin-500.svg
+-rw-rw-rw-   0        0        0    18564 2023-06-10 17:35:59.000000 seafoam-2.8.1/pelican/plugins/seafoam/static/fonts/expletus-sans/expletus-sans-v24-latin-500.ttf
+-rw-rw-rw-   0        0        0    13008 2023-06-10 17:35:59.000000 seafoam-2.8.1/pelican/plugins/seafoam/static/fonts/expletus-sans/expletus-sans-v24-latin-500.woff
+-rw-rw-rw-   0        0        0    10084 2023-06-10 17:35:59.000000 seafoam-2.8.1/pelican/plugins/seafoam/static/fonts/expletus-sans/expletus-sans-v24-latin-500.woff2
+-rw-rw-rw-   0        0        0   165742 2021-06-27 05:13:02.000000 seafoam-2.8.1/pelican/plugins/seafoam/static/fonts/fontawesome-webfont.eot
+-rw-rw-rw-   0        0        0   447050 2021-06-27 05:13:02.000000 seafoam-2.8.1/pelican/plugins/seafoam/static/fonts/fontawesome-webfont.svg
+-rw-rw-rw-   0        0        0   165548 2021-06-27 05:13:02.000000 seafoam-2.8.1/pelican/plugins/seafoam/static/fonts/fontawesome-webfont.ttf
+-rw-rw-rw-   0        0        0    98024 2021-06-27 05:13:02.000000 seafoam-2.8.1/pelican/plugins/seafoam/static/fonts/fontawesome-webfont.woff
+-rw-rw-rw-   0        0        0    77160 2021-06-27 05:13:02.000000 seafoam-2.8.1/pelican/plugins/seafoam/static/fonts/fontawesome-webfont.woff2
+-rw-rw-rw-   0        0        0    20127 2021-06-27 05:13:02.000000 seafoam-2.8.1/pelican/plugins/seafoam/static/fonts/glyphicons-halflings-regular.eot
+-rw-rw-rw-   0        0        0   109025 2021-06-27 05:13:02.000000 seafoam-2.8.1/pelican/plugins/seafoam/static/fonts/glyphicons-halflings-regular.svg
+-rw-rw-rw-   0        0        0    45404 2021-06-27 05:13:02.000000 seafoam-2.8.1/pelican/plugins/seafoam/static/fonts/glyphicons-halflings-regular.ttf
+-rw-rw-rw-   0        0        0    23424 2021-06-27 05:13:02.000000 seafoam-2.8.1/pelican/plugins/seafoam/static/fonts/glyphicons-halflings-regular.woff
+-rw-rw-rw-   0        0        0    18028 2021-06-27 05:13:02.000000 seafoam-2.8.1/pelican/plugins/seafoam/static/fonts/glyphicons-halflings-regular.woff2
+drwxrwxrwx   0        0        0        0 2023-06-12 00:16:10.574980 seafoam-2.8.1/pelican/plugins/seafoam/static/fonts/vidaloka/
+-rw-rw-rw-   0        0        0    30028 2023-06-10 17:35:59.000000 seafoam-2.8.1/pelican/plugins/seafoam/static/fonts/vidaloka/vidaloka-v18-latin-regular.eot
+-rw-rw-rw-   0        0        0    81305 2023-06-10 17:35:59.000000 seafoam-2.8.1/pelican/plugins/seafoam/static/fonts/vidaloka/vidaloka-v18-latin-regular.svg
+-rw-rw-rw-   0        0        0    78804 2023-06-10 17:35:59.000000 seafoam-2.8.1/pelican/plugins/seafoam/static/fonts/vidaloka/vidaloka-v18-latin-regular.ttf
+-rw-rw-rw-   0        0        0    36788 2023-06-10 17:35:59.000000 seafoam-2.8.1/pelican/plugins/seafoam/static/fonts/vidaloka/vidaloka-v18-latin-regular.woff
+-rw-rw-rw-   0        0        0    30116 2023-06-10 17:35:59.000000 seafoam-2.8.1/pelican/plugins/seafoam/static/fonts/vidaloka/vidaloka-v18-latin-regular.woff2
+drwxrwxrwx   0        0        0        0 2023-06-12 00:16:10.587981 seafoam-2.8.1/pelican/plugins/seafoam/static/js/
+-rw-rw-rw-   0        0        0    72084 2021-06-27 05:13:02.000000 seafoam-2.8.1/pelican/plugins/seafoam/static/js/bootstrap.js
+-rw-rw-rw-   0        0        0    37051 2021-06-27 05:13:02.000000 seafoam-2.8.1/pelican/plugins/seafoam/static/js/bootstrap.min.js
+-rw-rw-rw-   0        0        0     2512 2021-06-27 05:13:02.000000 seafoam-2.8.1/pelican/plugins/seafoam/static/js/comments.js
+-rw-rw-rw-   0        0        0     1520 2021-06-27 05:13:02.000000 seafoam-2.8.1/pelican/plugins/seafoam/static/js/github.js
+-rw-rw-rw-   0        0        0     2558 2021-06-27 05:13:02.000000 seafoam-2.8.1/pelican/plugins/seafoam/static/js/jXHR.js
+-rw-rw-rw-   0        0        0    86713 2021-06-27 05:13:02.000000 seafoam-2.8.1/pelican/plugins/seafoam/static/js/jquery.min.js
+-rw-rw-rw-   0        0        0     4381 2021-06-27 05:13:02.000000 seafoam-2.8.1/pelican/plugins/seafoam/static/js/respond.min.js
+drwxrwxrwx   0        0        0        0 2023-06-12 00:16:10.595982 seafoam-2.8.1/pelican/plugins/seafoam/static/tipuesearch/
+drwxrwxrwx   0        0        0        0 2023-06-12 00:16:10.596979 seafoam-2.8.1/pelican/plugins/seafoam/static/tipuesearch/img/
+-rw-rw-rw-   0        0        0      368 2021-06-27 05:13:02.000000 seafoam-2.8.1/pelican/plugins/seafoam/static/tipuesearch/img/search.png
+-rw-rw-rw-   0        0        0     5734 2021-06-27 05:13:02.000000 seafoam-2.8.1/pelican/plugins/seafoam/static/tipuesearch/tipuesearch.css
+-rw-rw-rw-   0        0        0    33779 2021-06-27 05:13:02.000000 seafoam-2.8.1/pelican/plugins/seafoam/static/tipuesearch/tipuesearch.js
+-rw-rw-rw-   0        0        0    10697 2021-06-27 05:13:02.000000 seafoam-2.8.1/pelican/plugins/seafoam/static/tipuesearch/tipuesearch.min.js
+-rw-rw-rw-   0        0        0     4537 2021-06-27 05:13:02.000000 seafoam-2.8.1/pelican/plugins/seafoam/static/tipuesearch/tipuesearch_content.js
+-rw-rw-rw-   0        0        0     3670 2021-06-27 05:13:02.000000 seafoam-2.8.1/pelican/plugins/seafoam/static/tipuesearch/tipuesearch_set.js
+drwxrwxrwx   0        0        0        0 2023-06-12 00:16:10.621976 seafoam-2.8.1/pelican/plugins/seafoam/templates/
+-rw-rw-rw-   0        0        0     1110 2021-06-27 05:13:02.000000 seafoam-2.8.1/pelican/plugins/seafoam/templates/404.html
+-rw-rw-rw-   0        0        0     5399 2021-06-27 05:13:02.000000 seafoam-2.8.1/pelican/plugins/seafoam/templates/archives.html
+-rw-rw-rw-   0        0        0     4597 2021-06-27 05:13:02.000000 seafoam-2.8.1/pelican/plugins/seafoam/templates/article.html
+-rw-rw-rw-   0        0        0     1508 2021-06-27 05:13:02.000000 seafoam-2.8.1/pelican/plugins/seafoam/templates/article_list.html
+-rw-rw-rw-   0        0        0      761 2021-06-27 05:13:02.000000 seafoam-2.8.1/pelican/plugins/seafoam/templates/author.html
+-rw-rw-rw-   0        0        0      857 2021-06-27 05:13:02.000000 seafoam-2.8.1/pelican/plugins/seafoam/templates/authors.html
+-rw-rw-rw-   0        0        0    14081 2023-06-10 17:35:59.000000 seafoam-2.8.1/pelican/plugins/seafoam/templates/base.html
+-rw-rw-rw-   0        0        0     2053 2021-06-27 05:13:02.000000 seafoam-2.8.1/pelican/plugins/seafoam/templates/categories.html
+-rw-rw-rw-   0        0        0      738 2021-06-27 05:13:02.000000 seafoam-2.8.1/pelican/plugins/seafoam/templates/category.html
+drwxrwxrwx   0        0        0        0 2023-06-12 00:16:10.664984 seafoam-2.8.1/pelican/plugins/seafoam/templates/includes/
+-rw-rw-rw-   0        0        0      196 2021-06-27 05:13:02.000000 seafoam-2.8.1/pelican/plugins/seafoam/templates/includes/aboutme.html
+-rw-rw-rw-   0        0        0      618 2023-06-10 17:35:59.000000 seafoam-2.8.1/pelican/plugins/seafoam/templates/includes/addthis.html
+-rw-rw-rw-   0        0        0     1481 2021-06-27 05:13:02.000000 seafoam-2.8.1/pelican/plugins/seafoam/templates/includes/article_info.html
+-rw-rw-rw-   0        0        0     2665 2023-06-10 17:35:59.000000 seafoam-2.8.1/pelican/plugins/seafoam/templates/includes/article_listing.html
+-rw-rw-rw-   0        0        0      978 2021-06-27 05:13:02.000000 seafoam-2.8.1/pelican/plugins/seafoam/templates/includes/assets-css.html
+-rw-rw-rw-   0        0        0      219 2021-06-27 05:13:02.000000 seafoam-2.8.1/pelican/plugins/seafoam/templates/includes/assets-js.html
+-rw-rw-rw-   0        0        0     4405 2021-06-27 05:13:02.000000 seafoam-2.8.1/pelican/plugins/seafoam/templates/includes/cc-license.html
+-rw-rw-rw-   0        0        0      553 2021-06-27 05:13:02.000000 seafoam-2.8.1/pelican/plugins/seafoam/templates/includes/comment_count.html
+-rw-rw-rw-   0        0        0     1291 2021-06-27 05:13:02.000000 seafoam-2.8.1/pelican/plugins/seafoam/templates/includes/comments-js.html
+-rw-rw-rw-   0        0        0     5874 2022-04-30 21:08:37.000000 seafoam-2.8.1/pelican/plugins/seafoam/templates/includes/comments.html
+-rw-rw-rw-   0        0        0      741 2021-06-27 05:13:02.000000 seafoam-2.8.1/pelican/plugins/seafoam/templates/includes/disqus_script.html
+-rw-rw-rw-   0        0        0     3364 2021-06-29 04:36:51.000000 seafoam-2.8.1/pelican/plugins/seafoam/templates/includes/footer.html
+-rw-rw-rw-   0        0        0     1818 2023-06-11 23:27:14.000000 seafoam-2.8.1/pelican/plugins/seafoam/templates/includes/ga.html
+-rw-rw-rw-   0        0        0     1308 2023-06-10 17:35:59.000000 seafoam-2.8.1/pelican/plugins/seafoam/templates/includes/github-js.html
+-rw-rw-rw-   0        0        0      442 2023-06-10 17:35:59.000000 seafoam-2.8.1/pelican/plugins/seafoam/templates/includes/github.html
+-rw-rw-rw-   0        0        0      434 2023-06-10 17:35:59.000000 seafoam-2.8.1/pelican/plugins/seafoam/templates/includes/links.html
+-rw-rw-rw-   0        0        0     1991 2022-03-21 04:06:10.000000 seafoam-2.8.1/pelican/plugins/seafoam/templates/includes/neighbors.html
+-rw-rw-rw-   0        0        0     2955 2021-06-27 05:13:02.000000 seafoam-2.8.1/pelican/plugins/seafoam/templates/includes/pagination.html
+-rw-rw-rw-   0        0        0      872 2023-06-10 17:35:59.000000 seafoam-2.8.1/pelican/plugins/seafoam/templates/includes/piwik.html
+-rw-rw-rw-   0        0        0      486 2021-06-27 05:13:02.000000 seafoam-2.8.1/pelican/plugins/seafoam/templates/includes/prjct.html
+-rw-rw-rw-   0        0        0      357 2021-06-27 05:13:02.000000 seafoam-2.8.1/pelican/plugins/seafoam/templates/includes/related-posts.html
+-rw-rw-rw-   0        0        0     3520 2021-10-24 02:08:02.000000 seafoam-2.8.1/pelican/plugins/seafoam/templates/includes/sidebar.html
+-rw-rw-rw-   0        0        0      276 2021-06-27 05:13:02.000000 seafoam-2.8.1/pelican/plugins/seafoam/templates/includes/taglist.html
+-rw-rw-rw-   0        0        0      296 2023-06-10 17:35:59.000000 seafoam-2.8.1/pelican/plugins/seafoam/templates/includes/translations.html
+-rw-rw-rw-   0        0        0      703 2023-06-10 17:35:59.000000 seafoam-2.8.1/pelican/plugins/seafoam/templates/includes/twitter_timeline.html
+-rw-rw-rw-   0        0        0      808 2023-06-10 17:35:59.000000 seafoam-2.8.1/pelican/plugins/seafoam/templates/index.html
+-rw-rw-rw-   0        0        0     2473 2023-06-10 17:35:59.000000 seafoam-2.8.1/pelican/plugins/seafoam/templates/page.html
+-rw-rw-rw-   0        0        0     7104 2021-06-27 05:13:02.000000 seafoam-2.8.1/pelican/plugins/seafoam/templates/period_archives.html
+-rw-rw-rw-   0        0        0     4517 2021-06-27 05:13:02.000000 seafoam-2.8.1/pelican/plugins/seafoam/templates/prjct.html
+-rw-rw-rw-   0        0        0     1507 2021-06-27 05:13:02.000000 seafoam-2.8.1/pelican/plugins/seafoam/templates/search.html
+drwxrwxrwx   0        0        0        0 2023-06-12 00:16:10.667984 seafoam-2.8.1/pelican/plugins/seafoam/templates/strathcona/
+-rw-rw-rw-   0        0        0     8939 2023-06-10 17:35:59.000000 seafoam-2.8.1/pelican/plugins/seafoam/templates/strathcona/dual_pricing.html
+-rw-rw-rw-   0        0        0     5443 2023-06-10 17:35:59.000000 seafoam-2.8.1/pelican/plugins/seafoam/templates/strathcona/pricing.html
+-rw-rw-rw-   0        0        0      795 2021-10-24 02:08:02.000000 seafoam-2.8.1/pelican/plugins/seafoam/templates/tag.html
+-rw-rw-rw-   0        0        0     2036 2021-10-24 02:08:02.000000 seafoam-2.8.1/pelican/plugins/seafoam/templates/tags.html
+-rw-rw-rw-   0        0        0      429 2022-03-21 04:06:10.000000 seafoam-2.8.1/pyproject.toml
+drwxrwxrwx   0        0        0        0 2023-06-12 00:16:10.706979 seafoam-2.8.1/seafoam.egg-info/
+-rw-rw-rw-   0        0        0    30291 2023-06-12 00:16:09.000000 seafoam-2.8.1/seafoam.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0     8286 2023-06-12 00:16:10.000000 seafoam-2.8.1/seafoam.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-06-12 00:16:09.000000 seafoam-2.8.1/seafoam.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0      235 2023-06-12 00:16:09.000000 seafoam-2.8.1/seafoam.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       41 2023-06-12 00:16:09.000000 seafoam-2.8.1/seafoam.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       74 2023-06-12 00:16:10.716977 seafoam-2.8.1/setup.cfg
+-rw-rw-rw-   0        0        0     4767 2023-06-10 17:35:59.000000 seafoam-2.8.1/setup.py
```

### Comparing `seafoam-2.8.0/LICENSE.txt` & `seafoam-2.8.1/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `seafoam-2.8.0/PKG-INFO` & `seafoam-2.8.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: seafoam
-Version: 2.8.0
+Version: 2.8.1
 Summary: Pelican theme, first used for Minchin.ca.
 Home-page: http://blog.minchin.ca/label/seafoam/
 Author: W. Minchin
 Author-email: w_minchin@hotmail.com
 License: MIT License
 Project-URL: Bug Tracker, https://github.com/MinchinWeb/seafoam/issues
 Project-URL: Changelog, https://github.com/MinchinWeb/seafoam/blob/master/docs/changelog.rst
```

### Comparing `seafoam-2.8.0/README.rst` & `seafoam-2.8.1/README.rst`

 * *Files identical despite different names*

### Comparing `seafoam-2.8.0/docs/CHANGELOG.rst` & `seafoam-2.8.1/docs/CHANGELOG.rst`

 * *Files 0% similar despite different names*

```diff
@@ -1,12 +1,14 @@
 Changelog
 =========
 
 .. Added, Changed, Depreciated, Removed, Fixed, Security
 
+- :release:`2.8.1 <2023-06-11>`
+- :bug:`-` fix link to font files
 - :release:`2.8.0 <2023-06-11>`
 - :feature:`20` add support for Google Analytics v4. Use
   ``GOOGLE_ANALYTICS_V4``. The previous version of Google Analytics is being
   deprecated, effective the end of June 2023.
 - :feature:`-` add ``DISPLAY_ARCHIVES_ON_MENU`` to control display of
   "Archives" link on navbar.
 - :feature:`-` add header image to pages (not just articles).
```

### Comparing `seafoam-2.8.0/pelican/plugins/seafoam/__init__.py` & `seafoam-2.8.1/pelican/plugins/seafoam/__init__.py`

 * *Files identical despite different names*

### Comparing `seafoam-2.8.0/pelican/plugins/seafoam/formatting.py` & `seafoam-2.8.1/pelican/plugins/seafoam/formatting.py`

 * *Files identical despite different names*

### Comparing `seafoam-2.8.0/pelican/plugins/seafoam/initialize.py` & `seafoam-2.8.1/pelican/plugins/seafoam/initialize.py`

 * *Files identical despite different names*

### Comparing `seafoam-2.8.0/pelican/plugins/seafoam/static/css/bootstrap.seafoam.min.css` & `seafoam-2.8.1/pelican/plugins/seafoam/static/css/bootstrap.seafoam.min.css`

 * *Files 0% similar despite different names*

```diff
@@ -9,17 +9,17 @@
 /* cabin-regular - latin */
 @font-face {
   font-display: swap;
   /* Check https://developer.mozilla.org/en-US/docs/Web/CSS/@font-face/font-display for other options. */
   font-family: 'Cabin';
   font-style: normal;
   font-weight: 400;
-  src: url('../fonts/cabin-v26-latin-regular.eot');
+  src: url('../fonts/cabin/cabin-v26-latin-regular.eot');
   /* IE9 Compat Modes */
-  src: local('Cabin'), local('Cabin-Regular'), url('../fonts/cabin-v26-latin-regular.eot?#iefix') format('embedded-opentype'), /* IE6-IE8 */ url('../fonts/cabin-v26-latin-regular.woff2') format('woff2'), /* Super Modern Browsers */ url('../fonts/cabin-v26-latin-regular.woff') format('woff'), /* Modern Browsers */ url('../fonts/cabin-v26-latin-regular.ttf') format('truetype'), /* Safari, Android, iOS */ url('../fonts/cabin-v26-latin-regular.svg#Cabin') format('svg');
+  src: local('Cabin'), local('Cabin-Regular'), url('../fonts/cabin/cabin-v26-latin-regular.eot?#iefix') format('embedded-opentype'), /* IE6-IE8 */ url('../fonts/cabin/cabin-v26-latin-regular.woff2') format('woff2'), /* Super Modern Browsers */ url('../fonts/cabin/cabin-v26-latin-regular.woff') format('woff'), /* Modern Browsers */ url('../fonts/cabin/cabin-v26-latin-regular.ttf') format('truetype'), /* Safari, Android, iOS */ url('../fonts/cabin/cabin-v26-latin-regular.svg#Cabin') format('svg');
   /* Legacy iOS */
 }
 /* cabin-italic - latin */
 @font-face {
   font-display: swap;
   /* Check https://developer.mozilla.org/en-US/docs/Web/CSS/@font-face/font-display for other options. */
   font-family: 'Cabin';
```

### Comparing `seafoam-2.8.0/pelican/plugins/seafoam/static/css/bootstrap.strathcona.min.css` & `seafoam-2.8.1/pelican/plugins/seafoam/static/css/bootstrap.strathcona.min.css`

 * *Files identical despite different names*

### Comparing `seafoam-2.8.0/pelican/plugins/seafoam/static/fonts/FontAwesome.otf` & `seafoam-2.8.1/pelican/plugins/seafoam/static/fonts/FontAwesome.otf`

 * *Files identical despite different names*

### Comparing `seafoam-2.8.0/pelican/plugins/seafoam/static/fonts/cabin/FONTLOG.txt` & `seafoam-2.8.1/pelican/plugins/seafoam/static/fonts/cabin/FONTLOG.txt`

 * *Files identical despite different names*

### Comparing `seafoam-2.8.0/pelican/plugins/seafoam/static/fonts/cabin/OFL.txt` & `seafoam-2.8.1/pelican/plugins/seafoam/static/fonts/cabin/OFL.txt`

 * *Files identical despite different names*

### Comparing `seafoam-2.8.0/pelican/plugins/seafoam/static/fonts/cabin/cabin-v26-latin-700.eot` & `seafoam-2.8.1/pelican/plugins/seafoam/static/fonts/cabin/cabin-v26-latin-700.eot`

 * *Files identical despite different names*

### Comparing `seafoam-2.8.0/pelican/plugins/seafoam/static/fonts/cabin/cabin-v26-latin-700.svg` & `seafoam-2.8.1/pelican/plugins/seafoam/static/fonts/cabin/cabin-v26-latin-700.svg`

 * *Files identical despite different names*

### Comparing `seafoam-2.8.0/pelican/plugins/seafoam/static/fonts/cabin/cabin-v26-latin-700.ttf` & `seafoam-2.8.1/pelican/plugins/seafoam/static/fonts/cabin/cabin-v26-latin-700.ttf`

 * *Files identical despite different names*

### Comparing `seafoam-2.8.0/pelican/plugins/seafoam/static/fonts/cabin/cabin-v26-latin-700.woff` & `seafoam-2.8.1/pelican/plugins/seafoam/static/fonts/cabin/cabin-v26-latin-700.woff`

 * *Files identical despite different names*

### Comparing `seafoam-2.8.0/pelican/plugins/seafoam/static/fonts/cabin/cabin-v26-latin-700.woff2` & `seafoam-2.8.1/pelican/plugins/seafoam/static/fonts/cabin/cabin-v26-latin-700.woff2`

 * *Files identical despite different names*

### Comparing `seafoam-2.8.0/pelican/plugins/seafoam/static/fonts/cabin/cabin-v26-latin-700italic.eot` & `seafoam-2.8.1/pelican/plugins/seafoam/static/fonts/cabin/cabin-v26-latin-700italic.eot`

 * *Files identical despite different names*

### Comparing `seafoam-2.8.0/pelican/plugins/seafoam/static/fonts/cabin/cabin-v26-latin-700italic.svg` & `seafoam-2.8.1/pelican/plugins/seafoam/static/fonts/cabin/cabin-v26-latin-700italic.svg`

 * *Files identical despite different names*

### Comparing `seafoam-2.8.0/pelican/plugins/seafoam/static/fonts/cabin/cabin-v26-latin-700italic.ttf` & `seafoam-2.8.1/pelican/plugins/seafoam/static/fonts/cabin/cabin-v26-latin-700italic.ttf`

 * *Files identical despite different names*

### Comparing `seafoam-2.8.0/pelican/plugins/seafoam/static/fonts/cabin/cabin-v26-latin-700italic.woff` & `seafoam-2.8.1/pelican/plugins/seafoam/static/fonts/cabin/cabin-v26-latin-700italic.woff`

 * *Files identical despite different names*

### Comparing `seafoam-2.8.0/pelican/plugins/seafoam/static/fonts/cabin/cabin-v26-latin-700italic.woff2` & `seafoam-2.8.1/pelican/plugins/seafoam/static/fonts/cabin/cabin-v26-latin-700italic.woff2`

 * *Files identical despite different names*

### Comparing `seafoam-2.8.0/pelican/plugins/seafoam/static/fonts/cabin/cabin-v26-latin-italic.eot` & `seafoam-2.8.1/pelican/plugins/seafoam/static/fonts/cabin/cabin-v26-latin-italic.eot`

 * *Files identical despite different names*

### Comparing `seafoam-2.8.0/pelican/plugins/seafoam/static/fonts/cabin/cabin-v26-latin-italic.svg` & `seafoam-2.8.1/pelican/plugins/seafoam/static/fonts/cabin/cabin-v26-latin-italic.svg`

 * *Files identical despite different names*

### Comparing `seafoam-2.8.0/pelican/plugins/seafoam/static/fonts/cabin/cabin-v26-latin-italic.ttf` & `seafoam-2.8.1/pelican/plugins/seafoam/static/fonts/cabin/cabin-v26-latin-italic.ttf`

 * *Files identical despite different names*

### Comparing `seafoam-2.8.0/pelican/plugins/seafoam/static/fonts/cabin/cabin-v26-latin-italic.woff` & `seafoam-2.8.1/pelican/plugins/seafoam/static/fonts/cabin/cabin-v26-latin-italic.woff`

 * *Files identical despite different names*

### Comparing `seafoam-2.8.0/pelican/plugins/seafoam/static/fonts/cabin/cabin-v26-latin-italic.woff2` & `seafoam-2.8.1/pelican/plugins/seafoam/static/fonts/cabin/cabin-v26-latin-italic.woff2`

 * *Files identical despite different names*

### Comparing `seafoam-2.8.0/pelican/plugins/seafoam/static/fonts/cabin/cabin-v26-latin-regular.eot` & `seafoam-2.8.1/pelican/plugins/seafoam/static/fonts/cabin/cabin-v26-latin-regular.eot`

 * *Files identical despite different names*

### Comparing `seafoam-2.8.0/pelican/plugins/seafoam/static/fonts/cabin/cabin-v26-latin-regular.svg` & `seafoam-2.8.1/pelican/plugins/seafoam/static/fonts/cabin/cabin-v26-latin-regular.svg`

 * *Files identical despite different names*

### Comparing `seafoam-2.8.0/pelican/plugins/seafoam/static/fonts/cabin/cabin-v26-latin-regular.ttf` & `seafoam-2.8.1/pelican/plugins/seafoam/static/fonts/cabin/cabin-v26-latin-regular.ttf`

 * *Files identical despite different names*

### Comparing `seafoam-2.8.0/pelican/plugins/seafoam/static/fonts/cabin/cabin-v26-latin-regular.woff` & `seafoam-2.8.1/pelican/plugins/seafoam/static/fonts/cabin/cabin-v26-latin-regular.woff`

 * *Files identical despite different names*

### Comparing `seafoam-2.8.0/pelican/plugins/seafoam/static/fonts/cabin/cabin-v26-latin-regular.woff2` & `seafoam-2.8.1/pelican/plugins/seafoam/static/fonts/cabin/cabin-v26-latin-regular.woff2`

 * *Files identical despite different names*

### Comparing `seafoam-2.8.0/pelican/plugins/seafoam/static/fonts/eb-garamond/eb-garamond-v26-latin-700.eot` & `seafoam-2.8.1/pelican/plugins/seafoam/static/fonts/eb-garamond/eb-garamond-v26-latin-700.eot`

 * *Files identical despite different names*

### Comparing `seafoam-2.8.0/pelican/plugins/seafoam/static/fonts/eb-garamond/eb-garamond-v26-latin-700.svg` & `seafoam-2.8.1/pelican/plugins/seafoam/static/fonts/eb-garamond/eb-garamond-v26-latin-700.svg`

 * *Files identical despite different names*

### Comparing `seafoam-2.8.0/pelican/plugins/seafoam/static/fonts/eb-garamond/eb-garamond-v26-latin-700.ttf` & `seafoam-2.8.1/pelican/plugins/seafoam/static/fonts/eb-garamond/eb-garamond-v26-latin-700.ttf`

 * *Files identical despite different names*

### Comparing `seafoam-2.8.0/pelican/plugins/seafoam/static/fonts/eb-garamond/eb-garamond-v26-latin-700.woff` & `seafoam-2.8.1/pelican/plugins/seafoam/static/fonts/eb-garamond/eb-garamond-v26-latin-700.woff`

 * *Files identical despite different names*

### Comparing `seafoam-2.8.0/pelican/plugins/seafoam/static/fonts/eb-garamond/eb-garamond-v26-latin-700.woff2` & `seafoam-2.8.1/pelican/plugins/seafoam/static/fonts/eb-garamond/eb-garamond-v26-latin-700.woff2`

 * *Files identical despite different names*

### Comparing `seafoam-2.8.0/pelican/plugins/seafoam/static/fonts/eb-garamond/eb-garamond-v26-latin-700italic.eot` & `seafoam-2.8.1/pelican/plugins/seafoam/static/fonts/eb-garamond/eb-garamond-v26-latin-700italic.eot`

 * *Files identical despite different names*

### Comparing `seafoam-2.8.0/pelican/plugins/seafoam/static/fonts/eb-garamond/eb-garamond-v26-latin-700italic.svg` & `seafoam-2.8.1/pelican/plugins/seafoam/static/fonts/eb-garamond/eb-garamond-v26-latin-700italic.svg`

 * *Files identical despite different names*

### Comparing `seafoam-2.8.0/pelican/plugins/seafoam/static/fonts/eb-garamond/eb-garamond-v26-latin-700italic.ttf` & `seafoam-2.8.1/pelican/plugins/seafoam/static/fonts/eb-garamond/eb-garamond-v26-latin-700italic.ttf`

 * *Files identical despite different names*

### Comparing `seafoam-2.8.0/pelican/plugins/seafoam/static/fonts/eb-garamond/eb-garamond-v26-latin-700italic.woff` & `seafoam-2.8.1/pelican/plugins/seafoam/static/fonts/eb-garamond/eb-garamond-v26-latin-700italic.woff`

 * *Files identical despite different names*

### Comparing `seafoam-2.8.0/pelican/plugins/seafoam/static/fonts/eb-garamond/eb-garamond-v26-latin-700italic.woff2` & `seafoam-2.8.1/pelican/plugins/seafoam/static/fonts/eb-garamond/eb-garamond-v26-latin-700italic.woff2`

 * *Files identical despite different names*

### Comparing `seafoam-2.8.0/pelican/plugins/seafoam/static/fonts/eb-garamond/eb-garamond-v26-latin-italic.eot` & `seafoam-2.8.1/pelican/plugins/seafoam/static/fonts/eb-garamond/eb-garamond-v26-latin-italic.eot`

 * *Files identical despite different names*

### Comparing `seafoam-2.8.0/pelican/plugins/seafoam/static/fonts/eb-garamond/eb-garamond-v26-latin-italic.svg` & `seafoam-2.8.1/pelican/plugins/seafoam/static/fonts/eb-garamond/eb-garamond-v26-latin-italic.svg`

 * *Files identical despite different names*

### Comparing `seafoam-2.8.0/pelican/plugins/seafoam/static/fonts/eb-garamond/eb-garamond-v26-latin-italic.ttf` & `seafoam-2.8.1/pelican/plugins/seafoam/static/fonts/eb-garamond/eb-garamond-v26-latin-italic.ttf`

 * *Files identical despite different names*

### Comparing `seafoam-2.8.0/pelican/plugins/seafoam/static/fonts/eb-garamond/eb-garamond-v26-latin-italic.woff` & `seafoam-2.8.1/pelican/plugins/seafoam/static/fonts/eb-garamond/eb-garamond-v26-latin-italic.woff`

 * *Files identical despite different names*

### Comparing `seafoam-2.8.0/pelican/plugins/seafoam/static/fonts/eb-garamond/eb-garamond-v26-latin-italic.woff2` & `seafoam-2.8.1/pelican/plugins/seafoam/static/fonts/eb-garamond/eb-garamond-v26-latin-italic.woff2`

 * *Files identical despite different names*

### Comparing `seafoam-2.8.0/pelican/plugins/seafoam/static/fonts/eb-garamond/eb-garamond-v26-latin-regular.eot` & `seafoam-2.8.1/pelican/plugins/seafoam/static/fonts/eb-garamond/eb-garamond-v26-latin-regular.eot`

 * *Files identical despite different names*

### Comparing `seafoam-2.8.0/pelican/plugins/seafoam/static/fonts/eb-garamond/eb-garamond-v26-latin-regular.svg` & `seafoam-2.8.1/pelican/plugins/seafoam/static/fonts/eb-garamond/eb-garamond-v26-latin-regular.svg`

 * *Files identical despite different names*

### Comparing `seafoam-2.8.0/pelican/plugins/seafoam/static/fonts/eb-garamond/eb-garamond-v26-latin-regular.ttf` & `seafoam-2.8.1/pelican/plugins/seafoam/static/fonts/eb-garamond/eb-garamond-v26-latin-regular.ttf`

 * *Files identical despite different names*

### Comparing `seafoam-2.8.0/pelican/plugins/seafoam/static/fonts/eb-garamond/eb-garamond-v26-latin-regular.woff` & `seafoam-2.8.1/pelican/plugins/seafoam/static/fonts/eb-garamond/eb-garamond-v26-latin-regular.woff`

 * *Files identical despite different names*

### Comparing `seafoam-2.8.0/pelican/plugins/seafoam/static/fonts/eb-garamond/eb-garamond-v26-latin-regular.woff2` & `seafoam-2.8.1/pelican/plugins/seafoam/static/fonts/eb-garamond/eb-garamond-v26-latin-regular.woff2`

 * *Files identical despite different names*

### Comparing `seafoam-2.8.0/pelican/plugins/seafoam/static/fonts/expletus-sans/OFL.txt` & `seafoam-2.8.1/pelican/plugins/seafoam/static/fonts/expletus-sans/OFL.txt`

 * *Files identical despite different names*

### Comparing `seafoam-2.8.0/pelican/plugins/seafoam/static/fonts/expletus-sans/expletus-sans-v24-latin-500.eot` & `seafoam-2.8.1/pelican/plugins/seafoam/static/fonts/expletus-sans/expletus-sans-v24-latin-500.eot`

 * *Files identical despite different names*

### Comparing `seafoam-2.8.0/pelican/plugins/seafoam/static/fonts/expletus-sans/expletus-sans-v24-latin-500.svg` & `seafoam-2.8.1/pelican/plugins/seafoam/static/fonts/expletus-sans/expletus-sans-v24-latin-500.svg`

 * *Files identical despite different names*

### Comparing `seafoam-2.8.0/pelican/plugins/seafoam/static/fonts/expletus-sans/expletus-sans-v24-latin-500.ttf` & `seafoam-2.8.1/pelican/plugins/seafoam/static/fonts/expletus-sans/expletus-sans-v24-latin-500.ttf`

 * *Files identical despite different names*

### Comparing `seafoam-2.8.0/pelican/plugins/seafoam/static/fonts/expletus-sans/expletus-sans-v24-latin-500.woff` & `seafoam-2.8.1/pelican/plugins/seafoam/static/fonts/expletus-sans/expletus-sans-v24-latin-500.woff`

 * *Files identical despite different names*

### Comparing `seafoam-2.8.0/pelican/plugins/seafoam/static/fonts/expletus-sans/expletus-sans-v24-latin-500.woff2` & `seafoam-2.8.1/pelican/plugins/seafoam/static/fonts/expletus-sans/expletus-sans-v24-latin-500.woff2`

 * *Files identical despite different names*

### Comparing `seafoam-2.8.0/pelican/plugins/seafoam/static/fonts/fontawesome-webfont.eot` & `seafoam-2.8.1/pelican/plugins/seafoam/static/fonts/fontawesome-webfont.eot`

 * *Files identical despite different names*

### Comparing `seafoam-2.8.0/pelican/plugins/seafoam/static/fonts/fontawesome-webfont.svg` & `seafoam-2.8.1/pelican/plugins/seafoam/static/fonts/fontawesome-webfont.svg`

 * *Files identical despite different names*

### Comparing `seafoam-2.8.0/pelican/plugins/seafoam/static/fonts/fontawesome-webfont.ttf` & `seafoam-2.8.1/pelican/plugins/seafoam/static/fonts/fontawesome-webfont.ttf`

 * *Files identical despite different names*

### Comparing `seafoam-2.8.0/pelican/plugins/seafoam/static/fonts/fontawesome-webfont.woff` & `seafoam-2.8.1/pelican/plugins/seafoam/static/fonts/fontawesome-webfont.woff`

 * *Files identical despite different names*

### Comparing `seafoam-2.8.0/pelican/plugins/seafoam/static/fonts/fontawesome-webfont.woff2` & `seafoam-2.8.1/pelican/plugins/seafoam/static/fonts/fontawesome-webfont.woff2`

 * *Files identical despite different names*

### Comparing `seafoam-2.8.0/pelican/plugins/seafoam/static/fonts/glyphicons-halflings-regular.eot` & `seafoam-2.8.1/pelican/plugins/seafoam/static/fonts/glyphicons-halflings-regular.eot`

 * *Files identical despite different names*

### Comparing `seafoam-2.8.0/pelican/plugins/seafoam/static/fonts/glyphicons-halflings-regular.svg` & `seafoam-2.8.1/pelican/plugins/seafoam/static/fonts/glyphicons-halflings-regular.svg`

 * *Files identical despite different names*

### Comparing `seafoam-2.8.0/pelican/plugins/seafoam/static/fonts/glyphicons-halflings-regular.ttf` & `seafoam-2.8.1/pelican/plugins/seafoam/static/fonts/glyphicons-halflings-regular.ttf`

 * *Files identical despite different names*

### Comparing `seafoam-2.8.0/pelican/plugins/seafoam/static/fonts/glyphicons-halflings-regular.woff` & `seafoam-2.8.1/pelican/plugins/seafoam/static/fonts/glyphicons-halflings-regular.woff`

 * *Files identical despite different names*

### Comparing `seafoam-2.8.0/pelican/plugins/seafoam/static/fonts/glyphicons-halflings-regular.woff2` & `seafoam-2.8.1/pelican/plugins/seafoam/static/fonts/glyphicons-halflings-regular.woff2`

 * *Files identical despite different names*

### Comparing `seafoam-2.8.0/pelican/plugins/seafoam/static/fonts/vidaloka/vidaloka-v18-latin-regular.eot` & `seafoam-2.8.1/pelican/plugins/seafoam/static/fonts/vidaloka/vidaloka-v18-latin-regular.eot`

 * *Files identical despite different names*

### Comparing `seafoam-2.8.0/pelican/plugins/seafoam/static/fonts/vidaloka/vidaloka-v18-latin-regular.svg` & `seafoam-2.8.1/pelican/plugins/seafoam/static/fonts/vidaloka/vidaloka-v18-latin-regular.svg`

 * *Files identical despite different names*

### Comparing `seafoam-2.8.0/pelican/plugins/seafoam/static/fonts/vidaloka/vidaloka-v18-latin-regular.ttf` & `seafoam-2.8.1/pelican/plugins/seafoam/static/fonts/vidaloka/vidaloka-v18-latin-regular.ttf`

 * *Files identical despite different names*

### Comparing `seafoam-2.8.0/pelican/plugins/seafoam/static/fonts/vidaloka/vidaloka-v18-latin-regular.woff` & `seafoam-2.8.1/pelican/plugins/seafoam/static/fonts/vidaloka/vidaloka-v18-latin-regular.woff`

 * *Files identical despite different names*

### Comparing `seafoam-2.8.0/pelican/plugins/seafoam/static/fonts/vidaloka/vidaloka-v18-latin-regular.woff2` & `seafoam-2.8.1/pelican/plugins/seafoam/static/fonts/vidaloka/vidaloka-v18-latin-regular.woff2`

 * *Files identical despite different names*

### Comparing `seafoam-2.8.0/pelican/plugins/seafoam/static/js/bootstrap.js` & `seafoam-2.8.1/pelican/plugins/seafoam/static/js/bootstrap.js`

 * *Files identical despite different names*

### Comparing `seafoam-2.8.0/pelican/plugins/seafoam/static/js/bootstrap.min.js` & `seafoam-2.8.1/pelican/plugins/seafoam/static/js/bootstrap.min.js`

 * *Files identical despite different names*

### Comparing `seafoam-2.8.0/pelican/plugins/seafoam/static/js/comments.js` & `seafoam-2.8.1/pelican/plugins/seafoam/static/js/comments.js`

 * *Files identical despite different names*

### Comparing `seafoam-2.8.0/pelican/plugins/seafoam/static/js/github.js` & `seafoam-2.8.1/pelican/plugins/seafoam/static/js/github.js`

 * *Files identical despite different names*

### Comparing `seafoam-2.8.0/pelican/plugins/seafoam/static/js/jXHR.js` & `seafoam-2.8.1/pelican/plugins/seafoam/static/js/jXHR.js`

 * *Files identical despite different names*

### Comparing `seafoam-2.8.0/pelican/plugins/seafoam/static/js/jquery.min.js` & `seafoam-2.8.1/pelican/plugins/seafoam/static/js/jquery.min.js`

 * *Files identical despite different names*

### Comparing `seafoam-2.8.0/pelican/plugins/seafoam/static/js/respond.min.js` & `seafoam-2.8.1/pelican/plugins/seafoam/static/js/respond.min.js`

 * *Files identical despite different names*

### Comparing `seafoam-2.8.0/pelican/plugins/seafoam/static/tipuesearch/tipuesearch.css` & `seafoam-2.8.1/pelican/plugins/seafoam/static/tipuesearch/tipuesearch.css`

 * *Files identical despite different names*

### Comparing `seafoam-2.8.0/pelican/plugins/seafoam/static/tipuesearch/tipuesearch.js` & `seafoam-2.8.1/pelican/plugins/seafoam/static/tipuesearch/tipuesearch.js`

 * *Files identical despite different names*

### Comparing `seafoam-2.8.0/pelican/plugins/seafoam/static/tipuesearch/tipuesearch.min.js` & `seafoam-2.8.1/pelican/plugins/seafoam/static/tipuesearch/tipuesearch.min.js`

 * *Files identical despite different names*

### Comparing `seafoam-2.8.0/pelican/plugins/seafoam/static/tipuesearch/tipuesearch_content.js` & `seafoam-2.8.1/pelican/plugins/seafoam/static/tipuesearch/tipuesearch_content.js`

 * *Files identical despite different names*

### Comparing `seafoam-2.8.0/pelican/plugins/seafoam/static/tipuesearch/tipuesearch_set.js` & `seafoam-2.8.1/pelican/plugins/seafoam/static/tipuesearch/tipuesearch_set.js`

 * *Files identical despite different names*

### Comparing `seafoam-2.8.0/pelican/plugins/seafoam/templates/404.html` & `seafoam-2.8.1/pelican/plugins/seafoam/templates/404.html`

 * *Files identical despite different names*

### Comparing `seafoam-2.8.0/pelican/plugins/seafoam/templates/archives.html` & `seafoam-2.8.1/pelican/plugins/seafoam/templates/archives.html`

 * *Files identical despite different names*

### Comparing `seafoam-2.8.0/pelican/plugins/seafoam/templates/article.html` & `seafoam-2.8.1/pelican/plugins/seafoam/templates/article.html`

 * *Files identical despite different names*

### Comparing `seafoam-2.8.0/pelican/plugins/seafoam/templates/article_list.html` & `seafoam-2.8.1/pelican/plugins/seafoam/templates/article_list.html`

 * *Files identical despite different names*

### Comparing `seafoam-2.8.0/pelican/plugins/seafoam/templates/author.html` & `seafoam-2.8.1/pelican/plugins/seafoam/templates/author.html`

 * *Files identical despite different names*

### Comparing `seafoam-2.8.0/pelican/plugins/seafoam/templates/authors.html` & `seafoam-2.8.1/pelican/plugins/seafoam/templates/authors.html`

 * *Files identical despite different names*

### Comparing `seafoam-2.8.0/pelican/plugins/seafoam/templates/base.html` & `seafoam-2.8.1/pelican/plugins/seafoam/templates/base.html`

 * *Files identical despite different names*

### Comparing `seafoam-2.8.0/pelican/plugins/seafoam/templates/categories.html` & `seafoam-2.8.1/pelican/plugins/seafoam/templates/categories.html`

 * *Files identical despite different names*

### Comparing `seafoam-2.8.0/pelican/plugins/seafoam/templates/category.html` & `seafoam-2.8.1/pelican/plugins/seafoam/templates/category.html`

 * *Files identical despite different names*

### Comparing `seafoam-2.8.0/pelican/plugins/seafoam/templates/includes/addthis.html` & `seafoam-2.8.1/pelican/plugins/seafoam/templates/includes/addthis.html`

 * *Files identical despite different names*

### Comparing `seafoam-2.8.0/pelican/plugins/seafoam/templates/includes/article_info.html` & `seafoam-2.8.1/pelican/plugins/seafoam/templates/includes/article_info.html`

 * *Files identical despite different names*

### Comparing `seafoam-2.8.0/pelican/plugins/seafoam/templates/includes/article_listing.html` & `seafoam-2.8.1/pelican/plugins/seafoam/templates/includes/article_listing.html`

 * *Files identical despite different names*

### Comparing `seafoam-2.8.0/pelican/plugins/seafoam/templates/includes/assets-css.html` & `seafoam-2.8.1/pelican/plugins/seafoam/templates/includes/assets-css.html`

 * *Files identical despite different names*

### Comparing `seafoam-2.8.0/pelican/plugins/seafoam/templates/includes/cc-license.html` & `seafoam-2.8.1/pelican/plugins/seafoam/templates/includes/cc-license.html`

 * *Files identical despite different names*

### Comparing `seafoam-2.8.0/pelican/plugins/seafoam/templates/includes/comment_count.html` & `seafoam-2.8.1/pelican/plugins/seafoam/templates/includes/comment_count.html`

 * *Files identical despite different names*

### Comparing `seafoam-2.8.0/pelican/plugins/seafoam/templates/includes/comments-js.html` & `seafoam-2.8.1/pelican/plugins/seafoam/templates/includes/comments-js.html`

 * *Files identical despite different names*

### Comparing `seafoam-2.8.0/pelican/plugins/seafoam/templates/includes/comments.html` & `seafoam-2.8.1/pelican/plugins/seafoam/templates/includes/comments.html`

 * *Files identical despite different names*

### Comparing `seafoam-2.8.0/pelican/plugins/seafoam/templates/includes/disqus_script.html` & `seafoam-2.8.1/pelican/plugins/seafoam/templates/includes/disqus_script.html`

 * *Files identical despite different names*

### Comparing `seafoam-2.8.0/pelican/plugins/seafoam/templates/includes/footer.html` & `seafoam-2.8.1/pelican/plugins/seafoam/templates/includes/footer.html`

 * *Files identical despite different names*

### Comparing `seafoam-2.8.0/pelican/plugins/seafoam/templates/includes/ga.html` & `seafoam-2.8.1/pelican/plugins/seafoam/templates/includes/ga.html`

 * *Files identical despite different names*

### Comparing `seafoam-2.8.0/pelican/plugins/seafoam/templates/includes/github-js.html` & `seafoam-2.8.1/pelican/plugins/seafoam/templates/includes/github-js.html`

 * *Files identical despite different names*

### Comparing `seafoam-2.8.0/pelican/plugins/seafoam/templates/includes/neighbors.html` & `seafoam-2.8.1/pelican/plugins/seafoam/templates/includes/neighbors.html`

 * *Files identical despite different names*

### Comparing `seafoam-2.8.0/pelican/plugins/seafoam/templates/includes/pagination.html` & `seafoam-2.8.1/pelican/plugins/seafoam/templates/includes/pagination.html`

 * *Files identical despite different names*

### Comparing `seafoam-2.8.0/pelican/plugins/seafoam/templates/includes/piwik.html` & `seafoam-2.8.1/pelican/plugins/seafoam/templates/includes/piwik.html`

 * *Files identical despite different names*

### Comparing `seafoam-2.8.0/pelican/plugins/seafoam/templates/includes/sidebar.html` & `seafoam-2.8.1/pelican/plugins/seafoam/templates/includes/sidebar.html`

 * *Files identical despite different names*

### Comparing `seafoam-2.8.0/pelican/plugins/seafoam/templates/includes/twitter_timeline.html` & `seafoam-2.8.1/pelican/plugins/seafoam/templates/includes/twitter_timeline.html`

 * *Files identical despite different names*

### Comparing `seafoam-2.8.0/pelican/plugins/seafoam/templates/index.html` & `seafoam-2.8.1/pelican/plugins/seafoam/templates/index.html`

 * *Files identical despite different names*

### Comparing `seafoam-2.8.0/pelican/plugins/seafoam/templates/page.html` & `seafoam-2.8.1/pelican/plugins/seafoam/templates/page.html`

 * *Files identical despite different names*

### Comparing `seafoam-2.8.0/pelican/plugins/seafoam/templates/period_archives.html` & `seafoam-2.8.1/pelican/plugins/seafoam/templates/period_archives.html`

 * *Files identical despite different names*

### Comparing `seafoam-2.8.0/pelican/plugins/seafoam/templates/prjct.html` & `seafoam-2.8.1/pelican/plugins/seafoam/templates/prjct.html`

 * *Files identical despite different names*

### Comparing `seafoam-2.8.0/pelican/plugins/seafoam/templates/search.html` & `seafoam-2.8.1/pelican/plugins/seafoam/templates/search.html`

 * *Files identical despite different names*

### Comparing `seafoam-2.8.0/pelican/plugins/seafoam/templates/strathcona/dual_pricing.html` & `seafoam-2.8.1/pelican/plugins/seafoam/templates/strathcona/dual_pricing.html`

 * *Files identical despite different names*

### Comparing `seafoam-2.8.0/pelican/plugins/seafoam/templates/strathcona/pricing.html` & `seafoam-2.8.1/pelican/plugins/seafoam/templates/strathcona/pricing.html`

 * *Files identical despite different names*

### Comparing `seafoam-2.8.0/pelican/plugins/seafoam/templates/tag.html` & `seafoam-2.8.1/pelican/plugins/seafoam/templates/tag.html`

 * *Files identical despite different names*

### Comparing `seafoam-2.8.0/pelican/plugins/seafoam/templates/tags.html` & `seafoam-2.8.1/pelican/plugins/seafoam/templates/tags.html`

 * *Files identical despite different names*

### Comparing `seafoam-2.8.0/seafoam.egg-info/PKG-INFO` & `seafoam-2.8.1/seafoam.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: seafoam
-Version: 2.8.0
+Version: 2.8.1
 Summary: Pelican theme, first used for Minchin.ca.
 Home-page: http://blog.minchin.ca/label/seafoam/
 Author: W. Minchin
 Author-email: w_minchin@hotmail.com
 License: MIT License
 Project-URL: Bug Tracker, https://github.com/MinchinWeb/seafoam/issues
 Project-URL: Changelog, https://github.com/MinchinWeb/seafoam/blob/master/docs/changelog.rst
```

### Comparing `seafoam-2.8.0/seafoam.egg-info/SOURCES.txt` & `seafoam-2.8.1/seafoam.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `seafoam-2.8.0/setup.py` & `seafoam-2.8.1/setup.py`

 * *Files identical despite different names*

