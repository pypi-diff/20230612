# Comparing `tmp/cssutils-2.7.0.tar.gz` & `tmp/cssutils-2.7.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "cssutils-2.7.0.tar", last modified: Fri Jun  9 01:46:59 2023, max compression
+gzip compressed data, was "cssutils-2.7.1.tar", last modified: Mon Jun 12 00:06:22 2023, max compression
```

## Comparing `cssutils-2.7.0.tar` & `cssutils-2.7.1.tar`

### file list

```diff
@@ -1,354 +1,354 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-09 01:46:59.229071 cssutils-2.7.0/
--rw-r--r--   0 runner    (1001) docker     (123)      133 2023-06-09 01:46:33.000000 cssutils-2.7.0/.coveragerc
--rw-r--r--   0 runner    (1001) docker     (123)      246 2023-06-09 01:46:33.000000 cssutils-2.7.0/.editorconfig
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-09 01:46:59.177068 cssutils-2.7.0/.github/
--rw-r--r--   0 runner    (1001) docker     (123)       24 2023-06-09 01:46:33.000000 cssutils-2.7.0/.github/FUNDING.yml
--rw-r--r--   0 runner    (1001) docker     (123)      148 2023-06-09 01:46:33.000000 cssutils-2.7.0/.github/dependabot.yml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-09 01:46:59.177068 cssutils-2.7.0/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (123)     3444 2023-06-09 01:46:33.000000 cssutils-2.7.0/.github/workflows/main.yml
--rw-r--r--   0 runner    (1001) docker     (123)       81 2023-06-09 01:46:33.000000 cssutils-2.7.0/.pre-commit-config.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      188 2023-06-09 01:46:33.000000 cssutils-2.7.0/.readthedocs.yaml
--rw-r--r--   0 runner    (1001) docker     (123)   122074 2023-06-09 01:46:33.000000 cssutils-2.7.0/CHANGES.rst
--rw-r--r--   0 runner    (1001) docker     (123)    35821 2023-06-09 01:46:33.000000 cssutils-2.7.0/COPYING
--rw-r--r--   0 runner    (1001) docker     (123)     7802 2023-06-09 01:46:33.000000 cssutils-2.7.0/COPYING.LESSER
--rw-r--r--   0 runner    (1001) docker     (123)     8409 2023-06-09 01:46:59.229071 cssutils-2.7.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     7480 2023-06-09 01:46:33.000000 cssutils-2.7.0/README.rst
--rw-r--r--   0 runner    (1001) docker     (123)      756 2023-06-09 01:46:33.000000 cssutils-2.7.0/conftest.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-09 01:46:59.181068 cssutils-2.7.0/cssutils/
--rw-r--r--   0 runner    (1001) docker     (123)    13946 2023-06-09 01:46:33.000000 cssutils-2.7.0/cssutils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1747 2023-06-09 01:46:33.000000 cssutils-2.7.0/cssutils/_fetch.py
--rw-r--r--   0 runner    (1001) docker     (123)     2495 2023-06-09 01:46:33.000000 cssutils-2.7.0/cssutils/_fetchgae.py
--rw-r--r--   0 runner    (1001) docker     (123)    22279 2023-06-09 01:46:33.000000 cssutils-2.7.0/cssutils/codec.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-09 01:46:59.185068 cssutils-2.7.0/cssutils/css/
--rw-r--r--   0 runner    (1001) docker     (123)     2125 2023-06-09 01:46:33.000000 cssutils-2.7.0/cssutils/css/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5943 2023-06-09 01:46:33.000000 cssutils-2.7.0/cssutils/css/colors.py
--rw-r--r--   0 runner    (1001) docker     (123)     5977 2023-06-09 01:46:33.000000 cssutils-2.7.0/cssutils/css/csscharsetrule.py
--rw-r--r--   0 runner    (1001) docker     (123)     2737 2023-06-09 01:46:33.000000 cssutils-2.7.0/cssutils/css/csscomment.py
--rw-r--r--   0 runner    (1001) docker     (123)     6531 2023-06-09 01:46:33.000000 cssutils-2.7.0/cssutils/css/cssfontfacerule.py
--rw-r--r--   0 runner    (1001) docker     (123)    14636 2023-06-09 01:46:33.000000 cssutils-2.7.0/cssutils/css/cssimportrule.py
--rw-r--r--   0 runner    (1001) docker     (123)    11980 2023-06-09 01:46:33.000000 cssutils-2.7.0/cssutils/css/cssmediarule.py
--rw-r--r--   0 runner    (1001) docker     (123)    11314 2023-06-09 01:46:33.000000 cssutils-2.7.0/cssutils/css/cssnamespacerule.py
--rw-r--r--   0 runner    (1001) docker     (123)    15491 2023-06-09 01:46:33.000000 cssutils-2.7.0/cssutils/css/csspagerule.py
--rw-r--r--   0 runner    (1001) docker     (123)     5190 2023-06-09 01:46:33.000000 cssutils-2.7.0/cssutils/css/cssproperties.py
--rw-r--r--   0 runner    (1001) docker     (123)    11407 2023-06-09 01:46:33.000000 cssutils-2.7.0/cssutils/css/cssrule.py
--rw-r--r--   0 runner    (1001) docker     (123)     1970 2023-06-09 01:46:33.000000 cssutils-2.7.0/cssutils/css/cssrulelist.py
--rw-r--r--   0 runner    (1001) docker     (123)    27117 2023-06-09 01:46:33.000000 cssutils-2.7.0/cssutils/css/cssstyledeclaration.py
--rw-r--r--   0 runner    (1001) docker     (123)     9277 2023-06-09 01:46:33.000000 cssutils-2.7.0/cssutils/css/cssstylerule.py
--rw-r--r--   0 runner    (1001) docker     (123)    33791 2023-06-09 01:46:33.000000 cssutils-2.7.0/cssutils/css/cssstylesheet.py
--rw-r--r--   0 runner    (1001) docker     (123)     8294 2023-06-09 01:46:33.000000 cssutils-2.7.0/cssutils/css/cssunknownrule.py
--rw-r--r--   0 runner    (1001) docker     (123)    47947 2023-06-09 01:46:33.000000 cssutils-2.7.0/cssutils/css/cssvalue.py
--rw-r--r--   0 runner    (1001) docker     (123)    11616 2023-06-09 01:46:33.000000 cssutils-2.7.0/cssutils/css/cssvariablesdeclaration.py
--rw-r--r--   0 runner    (1001) docker     (123)     7179 2023-06-09 01:46:33.000000 cssutils-2.7.0/cssutils/css/cssvariablesrule.py
--rw-r--r--   0 runner    (1001) docker     (123)     6885 2023-06-09 01:46:33.000000 cssutils-2.7.0/cssutils/css/marginrule.py
--rw-r--r--   0 runner    (1001) docker     (123)    18305 2023-06-09 01:46:33.000000 cssutils-2.7.0/cssutils/css/property.py
--rw-r--r--   0 runner    (1001) docker     (123)    32606 2023-06-09 01:46:33.000000 cssutils-2.7.0/cssutils/css/selector.py
--rw-r--r--   0 runner    (1001) docker     (123)     8376 2023-06-09 01:46:33.000000 cssutils-2.7.0/cssutils/css/selectorlist.py
--rw-r--r--   0 runner    (1001) docker     (123)    32593 2023-06-09 01:46:33.000000 cssutils-2.7.0/cssutils/css/value.py
--rw-r--r--   0 runner    (1001) docker     (123)     6047 2023-06-09 01:46:33.000000 cssutils-2.7.0/cssutils/css2productions.py
--rw-r--r--   0 runner    (1001) docker     (123)     4678 2023-06-09 01:46:33.000000 cssutils-2.7.0/cssutils/cssproductions.py
--rw-r--r--   0 runner    (1001) docker     (123)     3767 2023-06-09 01:46:33.000000 cssutils-2.7.0/cssutils/errorhandler.py
--rw-r--r--   0 runner    (1001) docker     (123)     3693 2023-06-09 01:46:33.000000 cssutils-2.7.0/cssutils/helper.py
--rw-r--r--   0 runner    (1001) docker     (123)     8552 2023-06-09 01:46:33.000000 cssutils-2.7.0/cssutils/parse.py
--rw-r--r--   0 runner    (1001) docker     (123)    27811 2023-06-09 01:46:33.000000 cssutils-2.7.0/cssutils/prodparser.py
--rw-r--r--   0 runner    (1001) docker     (123)    34876 2023-06-09 01:46:33.000000 cssutils-2.7.0/cssutils/profiles.py
--rw-r--r--   0 runner    (1001) docker     (123)    17249 2023-06-09 01:46:33.000000 cssutils-2.7.0/cssutils/sac.py
--rw-r--r--   0 runner    (1001) docker     (123)    12099 2023-06-09 01:46:33.000000 cssutils-2.7.0/cssutils/script.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-09 01:46:59.185068 cssutils-2.7.0/cssutils/scripts/
--rw-r--r--   0 runner    (1001) docker     (123)       61 2023-06-09 01:46:33.000000 cssutils-2.7.0/cssutils/scripts/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2451 2023-06-09 01:46:33.000000 cssutils-2.7.0/cssutils/scripts/csscapture.py
--rw-r--r--   0 runner    (1001) docker     (123)     3125 2023-06-09 01:46:33.000000 cssutils-2.7.0/cssutils/scripts/csscombine.py
--rw-r--r--   0 runner    (1001) docker     (123)     2078 2023-06-09 01:46:33.000000 cssutils-2.7.0/cssutils/scripts/cssparse.py
--rw-r--r--   0 runner    (1001) docker     (123)    42013 2023-06-09 01:46:33.000000 cssutils-2.7.0/cssutils/serialize.py
--rw-r--r--   0 runner    (1001) docker     (123)      549 2023-06-09 01:46:33.000000 cssutils-2.7.0/cssutils/settings.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-09 01:46:59.185068 cssutils-2.7.0/cssutils/stylesheets/
--rw-r--r--   0 runner    (1001) docker     (123)      351 2023-06-09 01:46:33.000000 cssutils-2.7.0/cssutils/stylesheets/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     8982 2023-06-09 01:46:33.000000 cssutils-2.7.0/cssutils/stylesheets/medialist.py
--rw-r--r--   0 runner    (1001) docker     (123)     7060 2023-06-09 01:46:33.000000 cssutils-2.7.0/cssutils/stylesheets/mediaquery.py
--rw-r--r--   0 runner    (1001) docker     (123)     5228 2023-06-09 01:46:33.000000 cssutils-2.7.0/cssutils/stylesheets/stylesheet.py
--rw-r--r--   0 runner    (1001) docker     (123)     1100 2023-06-09 01:46:33.000000 cssutils-2.7.0/cssutils/stylesheets/stylesheetlist.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-09 01:46:59.189069 cssutils-2.7.0/cssutils/tests/
--rw-r--r--   0 runner    (1001) docker     (123)       25 2023-06-09 01:46:33.000000 cssutils-2.7.0/cssutils/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1791 2023-06-09 01:46:33.000000 cssutils-2.7.0/cssutils/tests/basetest.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-09 01:46:59.197069 cssutils-2.7.0/cssutils/tests/sheets/
--rw-r--r--   0 runner    (1001) docker     (123)     4249 2023-06-09 01:46:33.000000 cssutils-2.7.0/cssutils/tests/sheets/096.css
--rw-r--r--   0 runner    (1001) docker     (123)     4249 2023-06-09 01:46:33.000000 cssutils-2.7.0/cssutils/tests/sheets/097.css
--rw-r--r--   0 runner    (1001) docker     (123)       59 2023-06-09 01:46:33.000000 cssutils-2.7.0/cssutils/tests/sheets/1.css
--rw-r--r--   0 runner    (1001) docker     (123)       71 2023-06-09 01:46:33.000000 cssutils-2.7.0/cssutils/tests/sheets/1ascii.css
--rw-r--r--   0 runner    (1001) docker     (123)       55 2023-06-09 01:46:33.000000 cssutils-2.7.0/cssutils/tests/sheets/1import.css
--rw-r--r--   0 runner    (1001) docker     (123)       32 2023-06-09 01:46:33.000000 cssutils-2.7.0/cssutils/tests/sheets/1inherit-ascii.css
--rw-r--r--   0 runner    (1001) docker     (123)       68 2023-06-09 01:46:33.000000 cssutils-2.7.0/cssutils/tests/sheets/1inherit-iso.css
--rw-r--r--   0 runner    (1001) docker     (123)       30 2023-06-09 01:46:33.000000 cssutils-2.7.0/cssutils/tests/sheets/1inherit-utf8.css
--rw-r--r--   0 runner    (1001) docker     (123)       65 2023-06-09 01:46:33.000000 cssutils-2.7.0/cssutils/tests/sheets/1utf.css
--rw-r--r--   0 runner    (1001) docker     (123)       39 2023-06-09 01:46:33.000000 cssutils-2.7.0/cssutils/tests/sheets/2inherit-iso.css
--rw-r--r--   0 runner    (1001) docker     (123)       36 2023-06-09 01:46:33.000000 cssutils-2.7.0/cssutils/tests/sheets/2resolve.css
--rw-r--r--   0 runner    (1001) docker     (123)     9502 2023-06-09 01:46:33.000000 cssutils-2.7.0/cssutils/tests/sheets/acid2.css
--rw-r--r--   0 runner    (1001) docker     (123)      264 2023-06-09 01:46:33.000000 cssutils-2.7.0/cssutils/tests/sheets/all.css
--rw-r--r--   0 runner    (1001) docker     (123)      137 2023-06-09 01:46:33.000000 cssutils-2.7.0/cssutils/tests/sheets/atrule.css
--rw-r--r--   0 runner    (1001) docker     (123)       73 2023-06-09 01:46:33.000000 cssutils-2.7.0/cssutils/tests/sheets/bad.css
--rw-r--r--   0 runner    (1001) docker     (123)       98 2023-06-09 01:46:33.000000 cssutils-2.7.0/cssutils/tests/sheets/basic.css
--rw-r--r--   0 runner    (1001) docker     (123)   208303 2023-06-09 01:46:33.000000 cssutils-2.7.0/cssutils/tests/sheets/bundle.css
--rw-r--r--   0 runner    (1001) docker     (123)       83 2023-06-09 01:46:33.000000 cssutils-2.7.0/cssutils/tests/sheets/cases.css
--rw-r--r--   0 runner    (1001) docker     (123)       97 2023-06-09 01:46:33.000000 cssutils-2.7.0/cssutils/tests/sheets/csscombine-1.css
--rw-r--r--   0 runner    (1001) docker     (123)      111 2023-06-09 01:46:33.000000 cssutils-2.7.0/cssutils/tests/sheets/csscombine-2.css
--rw-r--r--   0 runner    (1001) docker     (123)      220 2023-06-09 01:46:33.000000 cssutils-2.7.0/cssutils/tests/sheets/csscombine-proxy.css
--rw-r--r--   0 runner    (1001) docker     (123)     3851 2023-06-09 01:46:33.000000 cssutils-2.7.0/cssutils/tests/sheets/cthedot_default.css
--rw-r--r--   0 runner    (1001) docker     (123)     2797 2023-06-09 01:46:33.000000 cssutils-2.7.0/cssutils/tests/sheets/default_html4.css
--rw-r--r--   0 runner    (1001) docker     (123)      733 2023-06-09 01:46:33.000000 cssutils-2.7.0/cssutils/tests/sheets/hacks.css
--rw-r--r--   0 runner    (1001) docker     (123)      124 2023-06-09 01:46:33.000000 cssutils-2.7.0/cssutils/tests/sheets/html.css
--rw-r--r--   0 runner    (1001) docker     (123)     1503 2023-06-09 01:46:33.000000 cssutils-2.7.0/cssutils/tests/sheets/html20.css
--rw-r--r--   0 runner    (1001) docker     (123)     4274 2023-06-09 01:46:33.000000 cssutils-2.7.0/cssutils/tests/sheets/html40.css
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-09 01:46:59.197069 cssutils-2.7.0/cssutils/tests/sheets/images/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-09 01:46:33.000000 cssutils-2.7.0/cssutils/tests/sheets/images/example.gif
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-09 01:46:59.197069 cssutils-2.7.0/cssutils/tests/sheets/import/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-09 01:46:59.197069 cssutils-2.7.0/cssutils/tests/sheets/import/images2/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-09 01:46:33.000000 cssutils-2.7.0/cssutils/tests/sheets/import/images2/example2.gif
--rw-r--r--   0 runner    (1001) docker     (123)       88 2023-06-09 01:46:33.000000 cssutils-2.7.0/cssutils/tests/sheets/import/import-impossible.css
--rw-r--r--   0 runner    (1001) docker     (123)      427 2023-06-09 01:46:33.000000 cssutils-2.7.0/cssutils/tests/sheets/import/import2.css
--rw-r--r--   0 runner    (1001) docker     (123)      113 2023-06-09 01:46:33.000000 cssutils-2.7.0/cssutils/tests/sheets/import.css
--rw-r--r--   0 runner    (1001) docker     (123)      307 2023-06-09 01:46:33.000000 cssutils-2.7.0/cssutils/tests/sheets/import3.css
--rw-r--r--   0 runner    (1001) docker     (123)     9402 2023-06-09 01:46:33.000000 cssutils-2.7.0/cssutils/tests/sheets/ll.css
--rw-r--r--   0 runner    (1001) docker     (123)    97995 2023-06-09 01:46:33.000000 cssutils-2.7.0/cssutils/tests/sheets/ll2.css
--rw-r--r--   0 runner    (1001) docker     (123)       29 2023-06-09 01:46:33.000000 cssutils-2.7.0/cssutils/tests/sheets/multiple-values.css
--rw-r--r--   0 runner    (1001) docker     (123)       41 2023-06-09 01:46:33.000000 cssutils-2.7.0/cssutils/tests/sheets/page_test.css
--rw-r--r--   0 runner    (1001) docker     (123)    17998 2023-06-09 01:46:33.000000 cssutils-2.7.0/cssutils/tests/sheets/sample_5.css
--rw-r--r--   0 runner    (1001) docker     (123)     7662 2023-06-09 01:46:33.000000 cssutils-2.7.0/cssutils/tests/sheets/sample_7.css
--rw-r--r--   0 runner    (1001) docker     (123)      305 2023-06-09 01:46:33.000000 cssutils-2.7.0/cssutils/tests/sheets/simple.css
--rw-r--r--   0 runner    (1001) docker     (123)      113 2023-06-09 01:46:33.000000 cssutils-2.7.0/cssutils/tests/sheets/single-color.css
--rw-r--r--   0 runner    (1001) docker     (123)    18645 2023-06-09 01:46:33.000000 cssutils-2.7.0/cssutils/tests/sheets/slashcode.css
--rw-r--r--   0 runner    (1001) docker     (123)      677 2023-06-09 01:46:33.000000 cssutils-2.7.0/cssutils/tests/sheets/t-HACKS.css
--rw-r--r--   0 runner    (1001) docker     (123)     9268 2023-06-09 01:46:33.000000 cssutils-2.7.0/cssutils/tests/sheets/test-unicode.css
--rw-r--r--   0 runner    (1001) docker     (123)     4369 2023-06-09 01:46:33.000000 cssutils-2.7.0/cssutils/tests/sheets/test.css
--rw-r--r--   0 runner    (1001) docker     (123)     8665 2023-06-09 01:46:33.000000 cssutils-2.7.0/cssutils/tests/sheets/tigris.css
--rw-r--r--   0 runner    (1001) docker     (123)     9082 2023-06-09 01:46:33.000000 cssutils-2.7.0/cssutils/tests/sheets/tigris2.css
--rw-r--r--   0 runner    (1001) docker     (123)      296 2023-06-09 01:46:33.000000 cssutils-2.7.0/cssutils/tests/sheets/u_simple.css
--rw-r--r--   0 runner    (1001) docker     (123)       29 2023-06-09 01:46:33.000000 cssutils-2.7.0/cssutils/tests/sheets/v_simple.css
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-09 01:46:59.197069 cssutils-2.7.0/cssutils/tests/sheets/var/
--rw-r--r--   0 runner    (1001) docker     (123)      133 2023-06-09 01:46:33.000000 cssutils-2.7.0/cssutils/tests/sheets/var/start.css
--rw-r--r--   0 runner    (1001) docker     (123)      290 2023-06-09 01:46:33.000000 cssutils-2.7.0/cssutils/tests/sheets/var/use.css
--rw-r--r--   0 runner    (1001) docker     (123)       41 2023-06-09 01:46:33.000000 cssutils-2.7.0/cssutils/tests/sheets/var/vars.css
--rw-r--r--   0 runner    (1001) docker     (123)       33 2023-06-09 01:46:33.000000 cssutils-2.7.0/cssutils/tests/sheets/var/vars2.css
--rw-r--r--   0 runner    (1001) docker     (123)      222 2023-06-09 01:46:33.000000 cssutils-2.7.0/cssutils/tests/sheets/vars.css
--rw-r--r--   0 runner    (1001) docker     (123)      254 2023-06-09 01:46:33.000000 cssutils-2.7.0/cssutils/tests/sheets/varsimport.css
--rw-r--r--   0 runner    (1001) docker     (123)     4910 2023-06-09 01:46:33.000000 cssutils-2.7.0/cssutils/tests/sheets/xhtml2.css
--rw-r--r--   0 runner    (1001) docker     (123)     4825 2023-06-09 01:46:33.000000 cssutils-2.7.0/cssutils/tests/sheets/xhtml22.css
--rw-r--r--   0 runner    (1001) docker     (123)      117 2023-06-09 01:46:33.000000 cssutils-2.7.0/cssutils/tests/sheets/yuck.css
--rw-r--r--   0 runner    (1001) docker     (123)    14389 2023-06-09 01:46:33.000000 cssutils-2.7.0/cssutils/tests/test_codec.py
--rw-r--r--   0 runner    (1001) docker     (123)     4034 2023-06-09 01:46:33.000000 cssutils-2.7.0/cssutils/tests/test_csscharsetrule.py
--rw-r--r--   0 runner    (1001) docker     (123)     1958 2023-06-09 01:46:33.000000 cssutils-2.7.0/cssutils/tests/test_csscomment.py
--rw-r--r--   0 runner    (1001) docker     (123)     8090 2023-06-09 01:46:33.000000 cssutils-2.7.0/cssutils/tests/test_cssfontfacerule.py
--rw-r--r--   0 runner    (1001) docker     (123)    16588 2023-06-09 01:46:33.000000 cssutils-2.7.0/cssutils/tests/test_cssimportrule.py
--rw-r--r--   0 runner    (1001) docker     (123)    17061 2023-06-09 01:46:33.000000 cssutils-2.7.0/cssutils/tests/test_cssmediarule.py
--rw-r--r--   0 runner    (1001) docker     (123)     8408 2023-06-09 01:46:33.000000 cssutils-2.7.0/cssutils/tests/test_cssnamespacerule.py
--rw-r--r--   0 runner    (1001) docker     (123)    13502 2023-06-09 01:46:33.000000 cssutils-2.7.0/cssutils/tests/test_csspagerule.py
--rw-r--r--   0 runner    (1001) docker     (123)     2360 2023-06-09 01:46:33.000000 cssutils-2.7.0/cssutils/tests/test_cssproperties.py
--rw-r--r--   0 runner    (1001) docker     (123)     8195 2023-06-09 01:46:33.000000 cssutils-2.7.0/cssutils/tests/test_cssrule.py
--rw-r--r--   0 runner    (1001) docker     (123)      995 2023-06-09 01:46:33.000000 cssutils-2.7.0/cssutils/tests/test_cssrulelist.py
--rw-r--r--   0 runner    (1001) docker     (123)    22222 2023-06-09 01:46:33.000000 cssutils-2.7.0/cssutils/tests/test_cssstyledeclaration.py
--rw-r--r--   0 runner    (1001) docker     (123)     8615 2023-06-09 01:46:33.000000 cssutils-2.7.0/cssutils/tests/test_cssstylerule.py
--rw-r--r--   0 runner    (1001) docker     (123)    32396 2023-06-09 01:46:33.000000 cssutils-2.7.0/cssutils/tests/test_cssstylesheet.py
--rw-r--r--   0 runner    (1001) docker     (123)     4862 2023-06-09 01:46:33.000000 cssutils-2.7.0/cssutils/tests/test_cssunknownrule.py
--rw-r--r--   0 runner    (1001) docker     (123)    16770 2023-06-09 01:46:33.000000 cssutils-2.7.0/cssutils/tests/test_cssutils.py
--rw-r--r--   0 runner    (1001) docker     (123)      498 2023-06-09 01:46:33.000000 cssutils-2.7.0/cssutils/tests/test_cssutilsimport.py
--rw-r--r--   0 runner    (1001) docker     (123)    33005 2023-06-09 01:46:33.000000 cssutils-2.7.0/cssutils/tests/test_cssvalue.py
--rw-r--r--   0 runner    (1001) docker     (123)    10065 2023-06-09 01:46:33.000000 cssutils-2.7.0/cssutils/tests/test_cssvariablesdeclaration.py
--rw-r--r--   0 runner    (1001) docker     (123)     4717 2023-06-09 01:46:33.000000 cssutils-2.7.0/cssutils/tests/test_cssvariablesrule.py
--rw-r--r--   0 runner    (1001) docker     (123)     1445 2023-06-09 01:46:33.000000 cssutils-2.7.0/cssutils/tests/test_domimplementation.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-09 01:46:59.197069 cssutils-2.7.0/cssutils/tests/test_encutils/
--rw-r--r--   0 runner    (1001) docker     (123)    17678 2023-06-09 01:46:33.000000 cssutils-2.7.0/cssutils/tests/test_encutils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4843 2023-06-09 01:46:33.000000 cssutils-2.7.0/cssutils/tests/test_errorhandler.py
--rw-r--r--   0 runner    (1001) docker     (123)     2740 2023-06-09 01:46:33.000000 cssutils-2.7.0/cssutils/tests/test_helper.py
--rw-r--r--   0 runner    (1001) docker     (123)     3188 2023-06-09 01:46:33.000000 cssutils-2.7.0/cssutils/tests/test_marginrule.py
--rw-r--r--   0 runner    (1001) docker     (123)     6311 2023-06-09 01:46:33.000000 cssutils-2.7.0/cssutils/tests/test_medialist.py
--rw-r--r--   0 runner    (1001) docker     (123)     3266 2023-06-09 01:46:33.000000 cssutils-2.7.0/cssutils/tests/test_mediaquery.py
--rw-r--r--   0 runner    (1001) docker     (123)    19546 2023-06-09 01:46:33.000000 cssutils-2.7.0/cssutils/tests/test_parse.py
--rw-r--r--   0 runner    (1001) docker     (123)    13854 2023-06-09 01:46:33.000000 cssutils-2.7.0/cssutils/tests/test_prodparser.py
--rw-r--r--   0 runner    (1001) docker     (123)    23382 2023-06-09 01:46:33.000000 cssutils-2.7.0/cssutils/tests/test_profiles.py
--rw-r--r--   0 runner    (1001) docker     (123)     8255 2023-06-09 01:46:33.000000 cssutils-2.7.0/cssutils/tests/test_properties.py
--rw-r--r--   0 runner    (1001) docker     (123)     8692 2023-06-09 01:46:33.000000 cssutils-2.7.0/cssutils/tests/test_property.py
--rw-r--r--   0 runner    (1001) docker     (123)     2193 2023-06-09 01:46:33.000000 cssutils-2.7.0/cssutils/tests/test_scripts_csscombine.py
--rw-r--r--   0 runner    (1001) docker     (123)    15914 2023-06-09 01:46:33.000000 cssutils-2.7.0/cssutils/tests/test_selector.py
--rw-r--r--   0 runner    (1001) docker     (123)     4315 2023-06-09 01:46:33.000000 cssutils-2.7.0/cssutils/tests/test_selectorlist.py
--rw-r--r--   0 runner    (1001) docker     (123)    25825 2023-06-09 01:46:33.000000 cssutils-2.7.0/cssutils/tests/test_serialize.py
--rw-r--r--   0 runner    (1001) docker     (123)      634 2023-06-09 01:46:33.000000 cssutils-2.7.0/cssutils/tests/test_settings.py
--rw-r--r--   0 runner    (1001) docker     (123)     1020 2023-06-09 01:46:33.000000 cssutils-2.7.0/cssutils/tests/test_stylesheet.py
--rw-r--r--   0 runner    (1001) docker     (123)    22391 2023-06-09 01:46:33.000000 cssutils-2.7.0/cssutils/tests/test_tokenize2.py
--rw-r--r--   0 runner    (1001) docker     (123)    20706 2023-06-09 01:46:33.000000 cssutils-2.7.0/cssutils/tests/test_util.py
--rw-r--r--   0 runner    (1001) docker     (123)    45998 2023-06-09 01:46:33.000000 cssutils-2.7.0/cssutils/tests/test_value.py
--rw-r--r--   0 runner    (1001) docker     (123)     1630 2023-06-09 01:46:33.000000 cssutils-2.7.0/cssutils/tests/test_x.py
--rw-r--r--   0 runner    (1001) docker     (123)    11762 2023-06-09 01:46:33.000000 cssutils-2.7.0/cssutils/tokenize2.py
--rw-r--r--   0 runner    (1001) docker     (123)    34374 2023-06-09 01:46:33.000000 cssutils-2.7.0/cssutils/util.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-09 01:46:59.181068 cssutils-2.7.0/cssutils.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     8409 2023-06-09 01:46:59.000000 cssutils-2.7.0/cssutils.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     8903 2023-06-09 01:46:59.000000 cssutils-2.7.0/cssutils.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-09 01:46:59.000000 cssutils-2.7.0/cssutils.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      152 2023-06-09 01:46:59.000000 cssutils-2.7.0/cssutils.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)      438 2023-06-09 01:46:59.000000 cssutils-2.7.0/cssutils.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       18 2023-06-09 01:46:59.000000 cssutils-2.7.0/cssutils.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-09 01:46:59.201069 cssutils-2.7.0/docs/
--rw-r--r--   0 runner    (1001) docker     (123)     2272 2023-06-09 01:46:33.000000 cssutils-2.7.0/docs/backlog.rst
--rw-r--r--   0 runner    (1001) docker     (123)       90 2023-06-09 01:46:33.000000 cssutils-2.7.0/docs/codec.rst
--rw-r--r--   0 runner    (1001) docker     (123)     1395 2023-06-09 01:46:33.000000 cssutils-2.7.0/docs/conf.py
--rw-r--r--   0 runner    (1001) docker     (123)     8701 2023-06-09 01:46:33.000000 cssutils-2.7.0/docs/css.rst
--rw-r--r--   0 runner    (1001) docker     (123)      110 2023-06-09 01:46:33.000000 cssutils-2.7.0/docs/encutils.rst
--rw-r--r--   0 runner    (1001) docker     (123)       81 2023-06-09 01:46:33.000000 cssutils-2.7.0/docs/history.rst
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-09 01:46:59.201069 cssutils-2.7.0/docs/html/
--rw-r--r--   0 runner    (1001) docker     (123)      234 2023-06-09 01:46:33.000000 cssutils-2.7.0/docs/html/.buildinfo
--rw-r--r--   0 runner    (1001) docker     (123)   217445 2023-06-09 01:46:33.000000 cssutils-2.7.0/docs/html/CHANGELOG.html
--rw-r--r--   0 runner    (1001) docker     (123)    17807 2023-06-09 01:46:33.000000 cssutils-2.7.0/docs/html/README.html
--rw-r--r--   0 runner    (1001) docker     (123)     3665 2023-06-09 01:46:33.000000 cssutils-2.7.0/docs/html/_2to3 py3.html
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-09 01:46:59.201069 cssutils-2.7.0/docs/html/_sources/
--rw-r--r--   0 runner    (1001) docker     (123)   116989 2023-06-09 01:46:33.000000 cssutils-2.7.0/docs/html/_sources/CHANGELOG.txt
--rw-r--r--   0 runner    (1001) docker     (123)     5751 2023-06-09 01:46:33.000000 cssutils-2.7.0/docs/html/_sources/README.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-09 01:46:59.209070 cssutils-2.7.0/docs/html/_sources/docs/
--rw-r--r--   0 runner    (1001) docker     (123)     2452 2023-06-09 01:46:33.000000 cssutils-2.7.0/docs/html/_sources/docs/backlog.txt
--rw-r--r--   0 runner    (1001) docker     (123)       96 2023-06-09 01:46:33.000000 cssutils-2.7.0/docs/html/_sources/docs/codec.txt
--rw-r--r--   0 runner    (1001) docker     (123)     8751 2023-06-09 01:46:33.000000 cssutils-2.7.0/docs/html/_sources/docs/css.txt
--rw-r--r--   0 runner    (1001) docker     (123)     6138 2023-06-09 01:46:33.000000 cssutils-2.7.0/docs/html/_sources/docs/cssstyledeclaration.txt
--rw-r--r--   0 runner    (1001) docker     (123)      133 2023-06-09 01:46:33.000000 cssutils-2.7.0/docs/html/_sources/docs/cssutils.txt
--rw-r--r--   0 runner    (1001) docker     (123)      117 2023-06-09 01:46:33.000000 cssutils-2.7.0/docs/html/_sources/docs/encutils.txt
--rw-r--r--   0 runner    (1001) docker     (123)     2812 2023-06-09 01:46:33.000000 cssutils-2.7.0/docs/html/_sources/docs/implementation.txt
--rw-r--r--   0 runner    (1001) docker     (123)      967 2023-06-09 01:46:33.000000 cssutils-2.7.0/docs/html/_sources/docs/logging.txt
--rw-r--r--   0 runner    (1001) docker     (123)     8190 2023-06-09 01:46:33.000000 cssutils-2.7.0/docs/html/_sources/docs/migrate.txt
--rw-r--r--   0 runner    (1001) docker     (123)     2481 2023-06-09 01:46:33.000000 cssutils-2.7.0/docs/html/_sources/docs/parse.txt
--rw-r--r--   0 runner    (1001) docker     (123)     2535 2023-06-09 01:46:33.000000 cssutils-2.7.0/docs/html/_sources/docs/profiles.txt
--rw-r--r--   0 runner    (1001) docker     (123)     6932 2023-06-09 01:46:33.000000 cssutils-2.7.0/docs/html/_sources/docs/scripts.txt
--rw-r--r--   0 runner    (1001) docker     (123)     1818 2023-06-09 01:46:33.000000 cssutils-2.7.0/docs/html/_sources/docs/serialize.txt
--rw-r--r--   0 runner    (1001) docker     (123)     1120 2023-06-09 01:46:33.000000 cssutils-2.7.0/docs/html/_sources/docs/settings.txt
--rw-r--r--   0 runner    (1001) docker     (123)      758 2023-06-09 01:46:33.000000 cssutils-2.7.0/docs/html/_sources/docs/stylesheets.txt
--rw-r--r--   0 runner    (1001) docker     (123)      359 2023-06-09 01:46:33.000000 cssutils-2.7.0/docs/html/_sources/docs/utilities.txt
--rw-r--r--   0 runner    (1001) docker     (123)      447 2023-06-09 01:46:33.000000 cssutils-2.7.0/docs/html/_sources/docs/variables.txt
--rw-r--r--   0 runner    (1001) docker     (123)     1240 2023-06-09 01:46:33.000000 cssutils-2.7.0/docs/html/_sources/index.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-09 01:46:59.213070 cssutils-2.7.0/docs/html/_static/
--rw-r--r--   0 runner    (1001) docker     (123)     8269 2023-06-09 01:46:33.000000 cssutils-2.7.0/docs/html/_static/basic.css
--rw-r--r--   0 runner    (1001) docker     (123)     4040 2023-06-09 01:46:33.000000 cssutils-2.7.0/docs/html/_static/default.css
--rw-r--r--   0 runner    (1001) docker     (123)     6871 2023-06-09 01:46:33.000000 cssutils-2.7.0/docs/html/_static/doctools.js
--rw-r--r--   0 runner    (1001) docker     (123)      392 2023-06-09 01:46:33.000000 cssutils-2.7.0/docs/html/_static/file.png
--rw-r--r--   0 runner    (1001) docker     (123)    72174 2023-06-09 01:46:33.000000 cssutils-2.7.0/docs/html/_static/jquery.js
--rw-r--r--   0 runner    (1001) docker     (123)      199 2023-06-09 01:46:33.000000 cssutils-2.7.0/docs/html/_static/minus.png
--rw-r--r--   0 runner    (1001) docker     (123)      199 2023-06-09 01:46:33.000000 cssutils-2.7.0/docs/html/_static/plus.png
--rw-r--r--   0 runner    (1001) docker     (123)     3993 2023-06-09 01:46:33.000000 cssutils-2.7.0/docs/html/_static/pygments.css
--rw-r--r--   0 runner    (1001) docker     (123)    14509 2023-06-09 01:46:33.000000 cssutils-2.7.0/docs/html/_static/searchtools.js
--rw-r--r--   0 runner    (1001) docker     (123)     4634 2023-06-09 01:46:33.000000 cssutils-2.7.0/docs/html/_static/sidebar.js
--rw-r--r--   0 runner    (1001) docker     (123)     8205 2023-06-09 01:46:33.000000 cssutils-2.7.0/docs/html/_static/underscore.js
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-09 01:46:59.213070 cssutils-2.7.0/docs/html/docs/
--rw-r--r--   0 runner    (1001) docker     (123)    10377 2023-06-09 01:46:33.000000 cssutils-2.7.0/docs/html/docs/backlog.html
--rw-r--r--   0 runner    (1001) docker     (123)     4328 2023-06-09 01:46:33.000000 cssutils-2.7.0/docs/html/docs/codec.html
--rw-r--r--   0 runner    (1001) docker     (123)   167032 2023-06-09 01:46:33.000000 cssutils-2.7.0/docs/html/docs/css.html
--rw-r--r--   0 runner    (1001) docker     (123)    24168 2023-06-09 01:46:33.000000 cssutils-2.7.0/docs/html/docs/encutils.html
--rw-r--r--   0 runner    (1001) docker     (123)     6609 2023-06-09 01:46:33.000000 cssutils-2.7.0/docs/html/docs/logging.html
--rw-r--r--   0 runner    (1001) docker     (123)    27207 2023-06-09 01:46:33.000000 cssutils-2.7.0/docs/html/docs/migrate.html
--rw-r--r--   0 runner    (1001) docker     (123)    28207 2023-06-09 01:46:33.000000 cssutils-2.7.0/docs/html/docs/parse.html
--rw-r--r--   0 runner    (1001) docker     (123)    22715 2023-06-09 01:46:33.000000 cssutils-2.7.0/docs/html/docs/profiles.html
--rw-r--r--   0 runner    (1001) docker     (123)    18744 2023-06-09 01:46:33.000000 cssutils-2.7.0/docs/html/docs/scripts.html
--rw-r--r--   0 runner    (1001) docker     (123)    15756 2023-06-09 01:46:33.000000 cssutils-2.7.0/docs/html/docs/serialize.html
--rw-r--r--   0 runner    (1001) docker     (123)     6593 2023-06-09 01:46:33.000000 cssutils-2.7.0/docs/html/docs/settings.html
--rw-r--r--   0 runner    (1001) docker     (123)    21169 2023-06-09 01:46:33.000000 cssutils-2.7.0/docs/html/docs/stylesheets.html
--rw-r--r--   0 runner    (1001) docker     (123)    11209 2023-06-09 01:46:33.000000 cssutils-2.7.0/docs/html/docs/utilities.html
--rw-r--r--   0 runner    (1001) docker     (123)     4762 2023-06-09 01:46:33.000000 cssutils-2.7.0/docs/html/docs/variables.html
--rw-r--r--   0 runner    (1001) docker     (123)    50793 2023-06-09 01:46:33.000000 cssutils-2.7.0/docs/html/genindex.html
--rw-r--r--   0 runner    (1001) docker     (123)    20302 2023-06-09 01:46:33.000000 cssutils-2.7.0/docs/html/index.html
--rw-r--r--   0 runner    (1001) docker     (123)     5133 2023-06-09 01:46:33.000000 cssutils-2.7.0/docs/html/py-modindex.html
--rw-r--r--   0 runner    (1001) docker     (123)     3370 2023-06-09 01:46:33.000000 cssutils-2.7.0/docs/html/search.html
--rw-r--r--   0 runner    (1001) docker     (123)    42048 2023-06-09 01:46:33.000000 cssutils-2.7.0/docs/html/searchindex.js
--rw-r--r--   0 runner    (1001) docker     (123)      691 2023-06-09 01:46:33.000000 cssutils-2.7.0/docs/index.rst
--rw-r--r--   0 runner    (1001) docker     (123)     2672 2023-06-09 01:46:33.000000 cssutils-2.7.0/docs/known issues.rst
--rw-r--r--   0 runner    (1001) docker     (123)      943 2023-06-09 01:46:33.000000 cssutils-2.7.0/docs/logging.rst
--rw-r--r--   0 runner    (1001) docker     (123)     7988 2023-06-09 01:46:33.000000 cssutils-2.7.0/docs/migrate.rst
--rw-r--r--   0 runner    (1001) docker     (123)     2506 2023-06-09 01:46:33.000000 cssutils-2.7.0/docs/parse.rst
--rw-r--r--   0 runner    (1001) docker     (123)     2475 2023-06-09 01:46:33.000000 cssutils-2.7.0/docs/profiles.rst
--rw-r--r--   0 runner    (1001) docker     (123)     6760 2023-06-09 01:46:33.000000 cssutils-2.7.0/docs/scripts.rst
--rw-r--r--   0 runner    (1001) docker     (123)     1744 2023-06-09 01:46:33.000000 cssutils-2.7.0/docs/serialize.rst
--rw-r--r--   0 runner    (1001) docker     (123)     1096 2023-06-09 01:46:33.000000 cssutils-2.7.0/docs/settings.rst
--rw-r--r--   0 runner    (1001) docker     (123)      728 2023-06-09 01:46:33.000000 cssutils-2.7.0/docs/stylesheets.rst
--rw-r--r--   0 runner    (1001) docker     (123)      341 2023-06-09 01:46:33.000000 cssutils-2.7.0/docs/utilities.rst
--rw-r--r--   0 runner    (1001) docker     (123)      414 2023-06-09 01:46:33.000000 cssutils-2.7.0/docs/variables.rst
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-09 01:46:59.217070 cssutils-2.7.0/encutils/
--rw-r--r--   0 runner    (1001) docker     (123)    21282 2023-06-09 01:46:33.000000 cssutils-2.7.0/encutils/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-09 01:46:59.221070 cssutils-2.7.0/examples/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-09 01:46:33.000000 cssutils-2.7.0/examples/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2929 2023-06-09 01:46:33.000000 cssutils-2.7.0/examples/build.py
--rw-r--r--   0 runner    (1001) docker     (123)      332 2023-06-09 01:46:33.000000 cssutils-2.7.0/examples/codec.py
--rw-r--r--   0 runner    (1001) docker     (123)     1668 2023-06-09 01:46:33.000000 cssutils-2.7.0/examples/cssencodings.py
--rw-r--r--   0 runner    (1001) docker     (123)      683 2023-06-09 01:46:33.000000 cssutils-2.7.0/examples/customlog.py
--rw-r--r--   0 runner    (1001) docker     (123)      894 2023-06-09 01:46:33.000000 cssutils-2.7.0/examples/imports.py
--rw-r--r--   0 runner    (1001) docker     (123)      561 2023-06-09 01:46:33.000000 cssutils-2.7.0/examples/minify.py
--rw-r--r--   0 runner    (1001) docker     (123)     1370 2023-06-09 01:46:33.000000 cssutils-2.7.0/examples/parse.py
--rw-r--r--   0 runner    (1001) docker     (123)     1482 2023-06-09 01:46:33.000000 cssutils-2.7.0/examples/properties_with_same_name.py
--rw-r--r--   0 runner    (1001) docker     (123)     1404 2023-06-09 01:46:33.000000 cssutils-2.7.0/examples/selectors_tolower.py
--rw-r--r--   0 runner    (1001) docker     (123)     1775 2023-06-09 01:46:33.000000 cssutils-2.7.0/examples/serialize.py
--rw-r--r--   0 runner    (1001) docker     (123)     7237 2023-06-09 01:46:33.000000 cssutils-2.7.0/examples/style.py
--rw-r--r--   0 runner    (1001) docker     (123)     1341 2023-06-09 01:46:33.000000 cssutils-2.7.0/examples/styledeclaration.py
--rw-r--r--   0 runner    (1001) docker     (123)     2179 2023-06-09 01:46:33.000000 cssutils-2.7.0/examples/testutil.py
--rw-r--r--   0 runner    (1001) docker     (123)     5683 2023-06-09 01:46:33.000000 cssutils-2.7.0/examples/website.py
--rw-r--r--   0 runner    (1001) docker     (123)      154 2023-06-09 01:46:33.000000 cssutils-2.7.0/mypy.ini
--rw-r--r--   0 runner    (1001) docker     (123)      376 2023-06-09 01:46:33.000000 cssutils-2.7.0/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)      842 2023-06-09 01:46:33.000000 cssutils-2.7.0/pytest.ini
--rw-r--r--   0 runner    (1001) docker     (123)       70 2023-06-09 01:46:33.000000 cssutils-2.7.0/ruff.toml
--rw-r--r--   0 runner    (1001) docker     (123)     1684 2023-06-09 01:46:59.229071 cssutils-2.7.0/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-09 01:46:59.225071 cssutils-2.7.0/sheets/
--rw-r--r--   0 runner    (1001) docker     (123)     4249 2023-06-09 01:46:33.000000 cssutils-2.7.0/sheets/096.css
--rw-r--r--   0 runner    (1001) docker     (123)     4249 2023-06-09 01:46:33.000000 cssutils-2.7.0/sheets/097.css
--rw-r--r--   0 runner    (1001) docker     (123)       59 2023-06-09 01:46:33.000000 cssutils-2.7.0/sheets/1.css
--rw-r--r--   0 runner    (1001) docker     (123)       71 2023-06-09 01:46:33.000000 cssutils-2.7.0/sheets/1ascii.css
--rw-r--r--   0 runner    (1001) docker     (123)       55 2023-06-09 01:46:33.000000 cssutils-2.7.0/sheets/1import.css
--rw-r--r--   0 runner    (1001) docker     (123)       32 2023-06-09 01:46:33.000000 cssutils-2.7.0/sheets/1inherit-ascii.css
--rw-r--r--   0 runner    (1001) docker     (123)       68 2023-06-09 01:46:33.000000 cssutils-2.7.0/sheets/1inherit-iso.css
--rw-r--r--   0 runner    (1001) docker     (123)       30 2023-06-09 01:46:33.000000 cssutils-2.7.0/sheets/1inherit-utf8.css
--rw-r--r--   0 runner    (1001) docker     (123)       65 2023-06-09 01:46:33.000000 cssutils-2.7.0/sheets/1utf.css
--rw-r--r--   0 runner    (1001) docker     (123)       39 2023-06-09 01:46:33.000000 cssutils-2.7.0/sheets/2inherit-iso.css
--rw-r--r--   0 runner    (1001) docker     (123)       36 2023-06-09 01:46:33.000000 cssutils-2.7.0/sheets/2resolve.css
--rw-r--r--   0 runner    (1001) docker     (123)     9502 2023-06-09 01:46:33.000000 cssutils-2.7.0/sheets/acid2.css
--rw-r--r--   0 runner    (1001) docker     (123)      264 2023-06-09 01:46:33.000000 cssutils-2.7.0/sheets/all.css
--rw-r--r--   0 runner    (1001) docker     (123)      137 2023-06-09 01:46:33.000000 cssutils-2.7.0/sheets/atrule.css
--rw-r--r--   0 runner    (1001) docker     (123)       73 2023-06-09 01:46:33.000000 cssutils-2.7.0/sheets/bad.css
--rw-r--r--   0 runner    (1001) docker     (123)       98 2023-06-09 01:46:33.000000 cssutils-2.7.0/sheets/basic.css
--rw-r--r--   0 runner    (1001) docker     (123)   208303 2023-06-09 01:46:33.000000 cssutils-2.7.0/sheets/bundle.css
--rw-r--r--   0 runner    (1001) docker     (123)       83 2023-06-09 01:46:33.000000 cssutils-2.7.0/sheets/cases.css
--rw-r--r--   0 runner    (1001) docker     (123)       97 2023-06-09 01:46:33.000000 cssutils-2.7.0/sheets/csscombine-1.css
--rw-r--r--   0 runner    (1001) docker     (123)      111 2023-06-09 01:46:33.000000 cssutils-2.7.0/sheets/csscombine-2.css
--rw-r--r--   0 runner    (1001) docker     (123)      220 2023-06-09 01:46:33.000000 cssutils-2.7.0/sheets/csscombine-proxy.css
--rw-r--r--   0 runner    (1001) docker     (123)     3851 2023-06-09 01:46:33.000000 cssutils-2.7.0/sheets/cthedot_default.css
--rw-r--r--   0 runner    (1001) docker     (123)     2797 2023-06-09 01:46:33.000000 cssutils-2.7.0/sheets/default_html4.css
--rw-r--r--   0 runner    (1001) docker     (123)      733 2023-06-09 01:46:33.000000 cssutils-2.7.0/sheets/hacks.css
--rw-r--r--   0 runner    (1001) docker     (123)      124 2023-06-09 01:46:33.000000 cssutils-2.7.0/sheets/html.css
--rw-r--r--   0 runner    (1001) docker     (123)     1503 2023-06-09 01:46:33.000000 cssutils-2.7.0/sheets/html20.css
--rw-r--r--   0 runner    (1001) docker     (123)     4274 2023-06-09 01:46:33.000000 cssutils-2.7.0/sheets/html40.css
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-09 01:46:59.225071 cssutils-2.7.0/sheets/images/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-09 01:46:33.000000 cssutils-2.7.0/sheets/images/example.gif
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-09 01:46:59.225071 cssutils-2.7.0/sheets/import/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-09 01:46:59.225071 cssutils-2.7.0/sheets/import/images2/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-09 01:46:33.000000 cssutils-2.7.0/sheets/import/images2/example2.gif
--rw-r--r--   0 runner    (1001) docker     (123)       88 2023-06-09 01:46:33.000000 cssutils-2.7.0/sheets/import/import-impossible.css
--rw-r--r--   0 runner    (1001) docker     (123)      427 2023-06-09 01:46:33.000000 cssutils-2.7.0/sheets/import/import2.css
--rw-r--r--   0 runner    (1001) docker     (123)      113 2023-06-09 01:46:33.000000 cssutils-2.7.0/sheets/import.css
--rw-r--r--   0 runner    (1001) docker     (123)      307 2023-06-09 01:46:33.000000 cssutils-2.7.0/sheets/import3.css
--rw-r--r--   0 runner    (1001) docker     (123)     9402 2023-06-09 01:46:33.000000 cssutils-2.7.0/sheets/ll.css
--rw-r--r--   0 runner    (1001) docker     (123)    97995 2023-06-09 01:46:33.000000 cssutils-2.7.0/sheets/ll2.css
--rw-r--r--   0 runner    (1001) docker     (123)       29 2023-06-09 01:46:33.000000 cssutils-2.7.0/sheets/multiple-values.css
--rw-r--r--   0 runner    (1001) docker     (123)       41 2023-06-09 01:46:33.000000 cssutils-2.7.0/sheets/page_test.css
--rw-r--r--   0 runner    (1001) docker     (123)    17998 2023-06-09 01:46:33.000000 cssutils-2.7.0/sheets/sample_5.css
--rw-r--r--   0 runner    (1001) docker     (123)     7662 2023-06-09 01:46:33.000000 cssutils-2.7.0/sheets/sample_7.css
--rw-r--r--   0 runner    (1001) docker     (123)      305 2023-06-09 01:46:33.000000 cssutils-2.7.0/sheets/simple.css
--rw-r--r--   0 runner    (1001) docker     (123)      113 2023-06-09 01:46:33.000000 cssutils-2.7.0/sheets/single-color.css
--rw-r--r--   0 runner    (1001) docker     (123)    18645 2023-06-09 01:46:33.000000 cssutils-2.7.0/sheets/slashcode.css
--rw-r--r--   0 runner    (1001) docker     (123)      677 2023-06-09 01:46:33.000000 cssutils-2.7.0/sheets/t-HACKS.css
--rw-r--r--   0 runner    (1001) docker     (123)     9268 2023-06-09 01:46:33.000000 cssutils-2.7.0/sheets/test-unicode.css
--rw-r--r--   0 runner    (1001) docker     (123)     4369 2023-06-09 01:46:33.000000 cssutils-2.7.0/sheets/test.css
--rw-r--r--   0 runner    (1001) docker     (123)     8665 2023-06-09 01:46:33.000000 cssutils-2.7.0/sheets/tigris.css
--rw-r--r--   0 runner    (1001) docker     (123)     9082 2023-06-09 01:46:33.000000 cssutils-2.7.0/sheets/tigris2.css
--rw-r--r--   0 runner    (1001) docker     (123)      296 2023-06-09 01:46:33.000000 cssutils-2.7.0/sheets/u_simple.css
--rw-r--r--   0 runner    (1001) docker     (123)       29 2023-06-09 01:46:33.000000 cssutils-2.7.0/sheets/v_simple.css
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-09 01:46:59.229071 cssutils-2.7.0/sheets/var/
--rw-r--r--   0 runner    (1001) docker     (123)      133 2023-06-09 01:46:33.000000 cssutils-2.7.0/sheets/var/start.css
--rw-r--r--   0 runner    (1001) docker     (123)      290 2023-06-09 01:46:33.000000 cssutils-2.7.0/sheets/var/use.css
--rw-r--r--   0 runner    (1001) docker     (123)       41 2023-06-09 01:46:33.000000 cssutils-2.7.0/sheets/var/vars.css
--rw-r--r--   0 runner    (1001) docker     (123)       33 2023-06-09 01:46:33.000000 cssutils-2.7.0/sheets/var/vars2.css
--rw-r--r--   0 runner    (1001) docker     (123)      222 2023-06-09 01:46:33.000000 cssutils-2.7.0/sheets/vars.css
--rw-r--r--   0 runner    (1001) docker     (123)      254 2023-06-09 01:46:33.000000 cssutils-2.7.0/sheets/varsimport.css
--rw-r--r--   0 runner    (1001) docker     (123)     4910 2023-06-09 01:46:33.000000 cssutils-2.7.0/sheets/xhtml2.css
--rw-r--r--   0 runner    (1001) docker     (123)     4825 2023-06-09 01:46:33.000000 cssutils-2.7.0/sheets/xhtml22.css
--rw-r--r--   0 runner    (1001) docker     (123)      117 2023-06-09 01:46:33.000000 cssutils-2.7.0/sheets/yuck.css
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-09 01:46:59.229071 cssutils-2.7.0/tools/
--rw-r--r--   0 runner    (1001) docker     (123)      767 2023-06-09 01:46:33.000000 cssutils-2.7.0/tools/speed.py
--rw-r--r--   0 runner    (1001) docker     (123)    37596 2023-06-09 01:46:33.000000 cssutils-2.7.0/tools/try.py
--rw-r--r--   0 runner    (1001) docker     (123)      795 2023-06-09 01:46:33.000000 cssutils-2.7.0/tox.ini
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-12 00:06:22.503588 cssutils-2.7.1/
+-rw-r--r--   0 runner    (1001) docker     (123)      133 2023-06-12 00:05:57.000000 cssutils-2.7.1/.coveragerc
+-rw-r--r--   0 runner    (1001) docker     (123)      246 2023-06-12 00:05:57.000000 cssutils-2.7.1/.editorconfig
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-12 00:06:22.463587 cssutils-2.7.1/.github/
+-rw-r--r--   0 runner    (1001) docker     (123)       24 2023-06-12 00:05:57.000000 cssutils-2.7.1/.github/FUNDING.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      148 2023-06-12 00:05:57.000000 cssutils-2.7.1/.github/dependabot.yml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-12 00:06:22.463587 cssutils-2.7.1/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (123)     3364 2023-06-12 00:05:57.000000 cssutils-2.7.1/.github/workflows/main.yml
+-rw-r--r--   0 runner    (1001) docker     (123)       81 2023-06-12 00:05:57.000000 cssutils-2.7.1/.pre-commit-config.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      188 2023-06-12 00:05:57.000000 cssutils-2.7.1/.readthedocs.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)   122153 2023-06-12 00:05:57.000000 cssutils-2.7.1/CHANGES.rst
+-rw-r--r--   0 runner    (1001) docker     (123)    35821 2023-06-12 00:05:57.000000 cssutils-2.7.1/COPYING
+-rw-r--r--   0 runner    (1001) docker     (123)     7802 2023-06-12 00:05:57.000000 cssutils-2.7.1/COPYING.LESSER
+-rw-r--r--   0 runner    (1001) docker     (123)     8205 2023-06-12 00:06:22.503588 cssutils-2.7.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     7276 2023-06-12 00:05:57.000000 cssutils-2.7.1/README.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      756 2023-06-12 00:05:57.000000 cssutils-2.7.1/conftest.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-12 00:06:22.463587 cssutils-2.7.1/cssutils/
+-rw-r--r--   0 runner    (1001) docker     (123)    13946 2023-06-12 00:05:57.000000 cssutils-2.7.1/cssutils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1747 2023-06-12 00:05:57.000000 cssutils-2.7.1/cssutils/_fetch.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2495 2023-06-12 00:05:57.000000 cssutils-2.7.1/cssutils/_fetchgae.py
+-rw-r--r--   0 runner    (1001) docker     (123)    22279 2023-06-12 00:05:57.000000 cssutils-2.7.1/cssutils/codec.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-12 00:06:22.467588 cssutils-2.7.1/cssutils/css/
+-rw-r--r--   0 runner    (1001) docker     (123)     2125 2023-06-12 00:05:57.000000 cssutils-2.7.1/cssutils/css/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5943 2023-06-12 00:05:57.000000 cssutils-2.7.1/cssutils/css/colors.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5977 2023-06-12 00:05:57.000000 cssutils-2.7.1/cssutils/css/csscharsetrule.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2737 2023-06-12 00:05:57.000000 cssutils-2.7.1/cssutils/css/csscomment.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6531 2023-06-12 00:05:57.000000 cssutils-2.7.1/cssutils/css/cssfontfacerule.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14672 2023-06-12 00:05:57.000000 cssutils-2.7.1/cssutils/css/cssimportrule.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12047 2023-06-12 00:05:57.000000 cssutils-2.7.1/cssutils/css/cssmediarule.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11314 2023-06-12 00:05:57.000000 cssutils-2.7.1/cssutils/css/cssnamespacerule.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15491 2023-06-12 00:05:57.000000 cssutils-2.7.1/cssutils/css/csspagerule.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5190 2023-06-12 00:05:57.000000 cssutils-2.7.1/cssutils/css/cssproperties.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11327 2023-06-12 00:05:57.000000 cssutils-2.7.1/cssutils/css/cssrule.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1978 2023-06-12 00:05:57.000000 cssutils-2.7.1/cssutils/css/cssrulelist.py
+-rw-r--r--   0 runner    (1001) docker     (123)    27105 2023-06-12 00:05:57.000000 cssutils-2.7.1/cssutils/css/cssstyledeclaration.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9277 2023-06-12 00:05:57.000000 cssutils-2.7.1/cssutils/css/cssstylerule.py
+-rw-r--r--   0 runner    (1001) docker     (123)    33799 2023-06-12 00:05:57.000000 cssutils-2.7.1/cssutils/css/cssstylesheet.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8294 2023-06-12 00:05:57.000000 cssutils-2.7.1/cssutils/css/cssunknownrule.py
+-rw-r--r--   0 runner    (1001) docker     (123)    47907 2023-06-12 00:05:57.000000 cssutils-2.7.1/cssutils/css/cssvalue.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11528 2023-06-12 00:05:57.000000 cssutils-2.7.1/cssutils/css/cssvariablesdeclaration.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7179 2023-06-12 00:05:57.000000 cssutils-2.7.1/cssutils/css/cssvariablesrule.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6885 2023-06-12 00:05:57.000000 cssutils-2.7.1/cssutils/css/marginrule.py
+-rw-r--r--   0 runner    (1001) docker     (123)    18379 2023-06-12 00:05:57.000000 cssutils-2.7.1/cssutils/css/property.py
+-rw-r--r--   0 runner    (1001) docker     (123)    32604 2023-06-12 00:05:57.000000 cssutils-2.7.1/cssutils/css/selector.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8366 2023-06-12 00:05:57.000000 cssutils-2.7.1/cssutils/css/selectorlist.py
+-rw-r--r--   0 runner    (1001) docker     (123)    32614 2023-06-12 00:05:57.000000 cssutils-2.7.1/cssutils/css/value.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6047 2023-06-12 00:05:57.000000 cssutils-2.7.1/cssutils/css2productions.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4678 2023-06-12 00:05:57.000000 cssutils-2.7.1/cssutils/cssproductions.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3767 2023-06-12 00:05:57.000000 cssutils-2.7.1/cssutils/errorhandler.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3693 2023-06-12 00:05:57.000000 cssutils-2.7.1/cssutils/helper.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8552 2023-06-12 00:05:57.000000 cssutils-2.7.1/cssutils/parse.py
+-rw-r--r--   0 runner    (1001) docker     (123)    27811 2023-06-12 00:05:57.000000 cssutils-2.7.1/cssutils/prodparser.py
+-rw-r--r--   0 runner    (1001) docker     (123)    34884 2023-06-12 00:05:57.000000 cssutils-2.7.1/cssutils/profiles.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17249 2023-06-12 00:05:57.000000 cssutils-2.7.1/cssutils/sac.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12099 2023-06-12 00:05:57.000000 cssutils-2.7.1/cssutils/script.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-12 00:06:22.467588 cssutils-2.7.1/cssutils/scripts/
+-rw-r--r--   0 runner    (1001) docker     (123)       61 2023-06-12 00:05:57.000000 cssutils-2.7.1/cssutils/scripts/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2451 2023-06-12 00:05:57.000000 cssutils-2.7.1/cssutils/scripts/csscapture.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3125 2023-06-12 00:05:57.000000 cssutils-2.7.1/cssutils/scripts/csscombine.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2078 2023-06-12 00:05:57.000000 cssutils-2.7.1/cssutils/scripts/cssparse.py
+-rw-r--r--   0 runner    (1001) docker     (123)    42013 2023-06-12 00:05:57.000000 cssutils-2.7.1/cssutils/serialize.py
+-rw-r--r--   0 runner    (1001) docker     (123)      549 2023-06-12 00:05:57.000000 cssutils-2.7.1/cssutils/settings.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-12 00:06:22.471588 cssutils-2.7.1/cssutils/stylesheets/
+-rw-r--r--   0 runner    (1001) docker     (123)      351 2023-06-12 00:05:57.000000 cssutils-2.7.1/cssutils/stylesheets/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8982 2023-06-12 00:05:57.000000 cssutils-2.7.1/cssutils/stylesheets/medialist.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7060 2023-06-12 00:05:57.000000 cssutils-2.7.1/cssutils/stylesheets/mediaquery.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5228 2023-06-12 00:05:57.000000 cssutils-2.7.1/cssutils/stylesheets/stylesheet.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1100 2023-06-12 00:05:57.000000 cssutils-2.7.1/cssutils/stylesheets/stylesheetlist.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-12 00:06:22.475588 cssutils-2.7.1/cssutils/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)       25 2023-06-12 00:05:57.000000 cssutils-2.7.1/cssutils/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1791 2023-06-12 00:05:57.000000 cssutils-2.7.1/cssutils/tests/basetest.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-12 00:06:22.479588 cssutils-2.7.1/cssutils/tests/sheets/
+-rw-r--r--   0 runner    (1001) docker     (123)     4249 2023-06-12 00:05:57.000000 cssutils-2.7.1/cssutils/tests/sheets/096.css
+-rw-r--r--   0 runner    (1001) docker     (123)     4249 2023-06-12 00:05:57.000000 cssutils-2.7.1/cssutils/tests/sheets/097.css
+-rw-r--r--   0 runner    (1001) docker     (123)       59 2023-06-12 00:05:57.000000 cssutils-2.7.1/cssutils/tests/sheets/1.css
+-rw-r--r--   0 runner    (1001) docker     (123)       71 2023-06-12 00:05:57.000000 cssutils-2.7.1/cssutils/tests/sheets/1ascii.css
+-rw-r--r--   0 runner    (1001) docker     (123)       55 2023-06-12 00:05:57.000000 cssutils-2.7.1/cssutils/tests/sheets/1import.css
+-rw-r--r--   0 runner    (1001) docker     (123)       32 2023-06-12 00:05:57.000000 cssutils-2.7.1/cssutils/tests/sheets/1inherit-ascii.css
+-rw-r--r--   0 runner    (1001) docker     (123)       68 2023-06-12 00:05:57.000000 cssutils-2.7.1/cssutils/tests/sheets/1inherit-iso.css
+-rw-r--r--   0 runner    (1001) docker     (123)       30 2023-06-12 00:05:57.000000 cssutils-2.7.1/cssutils/tests/sheets/1inherit-utf8.css
+-rw-r--r--   0 runner    (1001) docker     (123)       65 2023-06-12 00:05:57.000000 cssutils-2.7.1/cssutils/tests/sheets/1utf.css
+-rw-r--r--   0 runner    (1001) docker     (123)       39 2023-06-12 00:05:57.000000 cssutils-2.7.1/cssutils/tests/sheets/2inherit-iso.css
+-rw-r--r--   0 runner    (1001) docker     (123)       36 2023-06-12 00:05:57.000000 cssutils-2.7.1/cssutils/tests/sheets/2resolve.css
+-rw-r--r--   0 runner    (1001) docker     (123)     9502 2023-06-12 00:05:57.000000 cssutils-2.7.1/cssutils/tests/sheets/acid2.css
+-rw-r--r--   0 runner    (1001) docker     (123)      264 2023-06-12 00:05:57.000000 cssutils-2.7.1/cssutils/tests/sheets/all.css
+-rw-r--r--   0 runner    (1001) docker     (123)      137 2023-06-12 00:05:57.000000 cssutils-2.7.1/cssutils/tests/sheets/atrule.css
+-rw-r--r--   0 runner    (1001) docker     (123)       73 2023-06-12 00:05:57.000000 cssutils-2.7.1/cssutils/tests/sheets/bad.css
+-rw-r--r--   0 runner    (1001) docker     (123)       98 2023-06-12 00:05:57.000000 cssutils-2.7.1/cssutils/tests/sheets/basic.css
+-rw-r--r--   0 runner    (1001) docker     (123)   208303 2023-06-12 00:05:57.000000 cssutils-2.7.1/cssutils/tests/sheets/bundle.css
+-rw-r--r--   0 runner    (1001) docker     (123)       83 2023-06-12 00:05:57.000000 cssutils-2.7.1/cssutils/tests/sheets/cases.css
+-rw-r--r--   0 runner    (1001) docker     (123)       97 2023-06-12 00:05:57.000000 cssutils-2.7.1/cssutils/tests/sheets/csscombine-1.css
+-rw-r--r--   0 runner    (1001) docker     (123)      111 2023-06-12 00:05:57.000000 cssutils-2.7.1/cssutils/tests/sheets/csscombine-2.css
+-rw-r--r--   0 runner    (1001) docker     (123)      220 2023-06-12 00:05:57.000000 cssutils-2.7.1/cssutils/tests/sheets/csscombine-proxy.css
+-rw-r--r--   0 runner    (1001) docker     (123)     3851 2023-06-12 00:05:57.000000 cssutils-2.7.1/cssutils/tests/sheets/cthedot_default.css
+-rw-r--r--   0 runner    (1001) docker     (123)     2797 2023-06-12 00:05:57.000000 cssutils-2.7.1/cssutils/tests/sheets/default_html4.css
+-rw-r--r--   0 runner    (1001) docker     (123)      733 2023-06-12 00:05:57.000000 cssutils-2.7.1/cssutils/tests/sheets/hacks.css
+-rw-r--r--   0 runner    (1001) docker     (123)      124 2023-06-12 00:05:57.000000 cssutils-2.7.1/cssutils/tests/sheets/html.css
+-rw-r--r--   0 runner    (1001) docker     (123)     1503 2023-06-12 00:05:57.000000 cssutils-2.7.1/cssutils/tests/sheets/html20.css
+-rw-r--r--   0 runner    (1001) docker     (123)     4274 2023-06-12 00:05:57.000000 cssutils-2.7.1/cssutils/tests/sheets/html40.css
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-12 00:06:22.479588 cssutils-2.7.1/cssutils/tests/sheets/images/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-12 00:05:57.000000 cssutils-2.7.1/cssutils/tests/sheets/images/example.gif
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-12 00:06:22.479588 cssutils-2.7.1/cssutils/tests/sheets/import/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-12 00:06:22.479588 cssutils-2.7.1/cssutils/tests/sheets/import/images2/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-12 00:05:57.000000 cssutils-2.7.1/cssutils/tests/sheets/import/images2/example2.gif
+-rw-r--r--   0 runner    (1001) docker     (123)       88 2023-06-12 00:05:57.000000 cssutils-2.7.1/cssutils/tests/sheets/import/import-impossible.css
+-rw-r--r--   0 runner    (1001) docker     (123)      427 2023-06-12 00:05:57.000000 cssutils-2.7.1/cssutils/tests/sheets/import/import2.css
+-rw-r--r--   0 runner    (1001) docker     (123)      113 2023-06-12 00:05:57.000000 cssutils-2.7.1/cssutils/tests/sheets/import.css
+-rw-r--r--   0 runner    (1001) docker     (123)      307 2023-06-12 00:05:57.000000 cssutils-2.7.1/cssutils/tests/sheets/import3.css
+-rw-r--r--   0 runner    (1001) docker     (123)     9402 2023-06-12 00:05:57.000000 cssutils-2.7.1/cssutils/tests/sheets/ll.css
+-rw-r--r--   0 runner    (1001) docker     (123)    97995 2023-06-12 00:05:57.000000 cssutils-2.7.1/cssutils/tests/sheets/ll2.css
+-rw-r--r--   0 runner    (1001) docker     (123)       29 2023-06-12 00:05:57.000000 cssutils-2.7.1/cssutils/tests/sheets/multiple-values.css
+-rw-r--r--   0 runner    (1001) docker     (123)       41 2023-06-12 00:05:57.000000 cssutils-2.7.1/cssutils/tests/sheets/page_test.css
+-rw-r--r--   0 runner    (1001) docker     (123)    17998 2023-06-12 00:05:57.000000 cssutils-2.7.1/cssutils/tests/sheets/sample_5.css
+-rw-r--r--   0 runner    (1001) docker     (123)     7662 2023-06-12 00:05:57.000000 cssutils-2.7.1/cssutils/tests/sheets/sample_7.css
+-rw-r--r--   0 runner    (1001) docker     (123)      305 2023-06-12 00:05:57.000000 cssutils-2.7.1/cssutils/tests/sheets/simple.css
+-rw-r--r--   0 runner    (1001) docker     (123)      113 2023-06-12 00:05:57.000000 cssutils-2.7.1/cssutils/tests/sheets/single-color.css
+-rw-r--r--   0 runner    (1001) docker     (123)    18645 2023-06-12 00:05:57.000000 cssutils-2.7.1/cssutils/tests/sheets/slashcode.css
+-rw-r--r--   0 runner    (1001) docker     (123)      677 2023-06-12 00:05:57.000000 cssutils-2.7.1/cssutils/tests/sheets/t-HACKS.css
+-rw-r--r--   0 runner    (1001) docker     (123)     9268 2023-06-12 00:05:57.000000 cssutils-2.7.1/cssutils/tests/sheets/test-unicode.css
+-rw-r--r--   0 runner    (1001) docker     (123)     4369 2023-06-12 00:05:57.000000 cssutils-2.7.1/cssutils/tests/sheets/test.css
+-rw-r--r--   0 runner    (1001) docker     (123)     8665 2023-06-12 00:05:57.000000 cssutils-2.7.1/cssutils/tests/sheets/tigris.css
+-rw-r--r--   0 runner    (1001) docker     (123)     9082 2023-06-12 00:05:57.000000 cssutils-2.7.1/cssutils/tests/sheets/tigris2.css
+-rw-r--r--   0 runner    (1001) docker     (123)      296 2023-06-12 00:05:57.000000 cssutils-2.7.1/cssutils/tests/sheets/u_simple.css
+-rw-r--r--   0 runner    (1001) docker     (123)       29 2023-06-12 00:05:57.000000 cssutils-2.7.1/cssutils/tests/sheets/v_simple.css
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-12 00:06:22.479588 cssutils-2.7.1/cssutils/tests/sheets/var/
+-rw-r--r--   0 runner    (1001) docker     (123)      133 2023-06-12 00:05:57.000000 cssutils-2.7.1/cssutils/tests/sheets/var/start.css
+-rw-r--r--   0 runner    (1001) docker     (123)      290 2023-06-12 00:05:57.000000 cssutils-2.7.1/cssutils/tests/sheets/var/use.css
+-rw-r--r--   0 runner    (1001) docker     (123)       41 2023-06-12 00:05:57.000000 cssutils-2.7.1/cssutils/tests/sheets/var/vars.css
+-rw-r--r--   0 runner    (1001) docker     (123)       33 2023-06-12 00:05:57.000000 cssutils-2.7.1/cssutils/tests/sheets/var/vars2.css
+-rw-r--r--   0 runner    (1001) docker     (123)      222 2023-06-12 00:05:57.000000 cssutils-2.7.1/cssutils/tests/sheets/vars.css
+-rw-r--r--   0 runner    (1001) docker     (123)      254 2023-06-12 00:05:57.000000 cssutils-2.7.1/cssutils/tests/sheets/varsimport.css
+-rw-r--r--   0 runner    (1001) docker     (123)     4910 2023-06-12 00:05:57.000000 cssutils-2.7.1/cssutils/tests/sheets/xhtml2.css
+-rw-r--r--   0 runner    (1001) docker     (123)     4825 2023-06-12 00:05:57.000000 cssutils-2.7.1/cssutils/tests/sheets/xhtml22.css
+-rw-r--r--   0 runner    (1001) docker     (123)      117 2023-06-12 00:05:57.000000 cssutils-2.7.1/cssutils/tests/sheets/yuck.css
+-rw-r--r--   0 runner    (1001) docker     (123)    14389 2023-06-12 00:05:57.000000 cssutils-2.7.1/cssutils/tests/test_codec.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4034 2023-06-12 00:05:57.000000 cssutils-2.7.1/cssutils/tests/test_csscharsetrule.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1958 2023-06-12 00:05:57.000000 cssutils-2.7.1/cssutils/tests/test_csscomment.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8090 2023-06-12 00:05:57.000000 cssutils-2.7.1/cssutils/tests/test_cssfontfacerule.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16588 2023-06-12 00:05:57.000000 cssutils-2.7.1/cssutils/tests/test_cssimportrule.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17041 2023-06-12 00:05:57.000000 cssutils-2.7.1/cssutils/tests/test_cssmediarule.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8408 2023-06-12 00:05:57.000000 cssutils-2.7.1/cssutils/tests/test_cssnamespacerule.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13502 2023-06-12 00:05:57.000000 cssutils-2.7.1/cssutils/tests/test_csspagerule.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2360 2023-06-12 00:05:57.000000 cssutils-2.7.1/cssutils/tests/test_cssproperties.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8195 2023-06-12 00:05:57.000000 cssutils-2.7.1/cssutils/tests/test_cssrule.py
+-rw-r--r--   0 runner    (1001) docker     (123)      995 2023-06-12 00:05:57.000000 cssutils-2.7.1/cssutils/tests/test_cssrulelist.py
+-rw-r--r--   0 runner    (1001) docker     (123)    22222 2023-06-12 00:05:57.000000 cssutils-2.7.1/cssutils/tests/test_cssstyledeclaration.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8615 2023-06-12 00:05:57.000000 cssutils-2.7.1/cssutils/tests/test_cssstylerule.py
+-rw-r--r--   0 runner    (1001) docker     (123)    32396 2023-06-12 00:05:57.000000 cssutils-2.7.1/cssutils/tests/test_cssstylesheet.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4862 2023-06-12 00:05:57.000000 cssutils-2.7.1/cssutils/tests/test_cssunknownrule.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16770 2023-06-12 00:05:57.000000 cssutils-2.7.1/cssutils/tests/test_cssutils.py
+-rw-r--r--   0 runner    (1001) docker     (123)      498 2023-06-12 00:05:57.000000 cssutils-2.7.1/cssutils/tests/test_cssutilsimport.py
+-rw-r--r--   0 runner    (1001) docker     (123)    33005 2023-06-12 00:05:57.000000 cssutils-2.7.1/cssutils/tests/test_cssvalue.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10065 2023-06-12 00:05:57.000000 cssutils-2.7.1/cssutils/tests/test_cssvariablesdeclaration.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4717 2023-06-12 00:05:57.000000 cssutils-2.7.1/cssutils/tests/test_cssvariablesrule.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1445 2023-06-12 00:05:57.000000 cssutils-2.7.1/cssutils/tests/test_domimplementation.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-12 00:06:22.479588 cssutils-2.7.1/cssutils/tests/test_encutils/
+-rw-r--r--   0 runner    (1001) docker     (123)    17678 2023-06-12 00:05:57.000000 cssutils-2.7.1/cssutils/tests/test_encutils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4843 2023-06-12 00:05:57.000000 cssutils-2.7.1/cssutils/tests/test_errorhandler.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2740 2023-06-12 00:05:57.000000 cssutils-2.7.1/cssutils/tests/test_helper.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3188 2023-06-12 00:05:57.000000 cssutils-2.7.1/cssutils/tests/test_marginrule.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6311 2023-06-12 00:05:57.000000 cssutils-2.7.1/cssutils/tests/test_medialist.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3266 2023-06-12 00:05:57.000000 cssutils-2.7.1/cssutils/tests/test_mediaquery.py
+-rw-r--r--   0 runner    (1001) docker     (123)    19546 2023-06-12 00:05:57.000000 cssutils-2.7.1/cssutils/tests/test_parse.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13854 2023-06-12 00:05:57.000000 cssutils-2.7.1/cssutils/tests/test_prodparser.py
+-rw-r--r--   0 runner    (1001) docker     (123)    23382 2023-06-12 00:05:57.000000 cssutils-2.7.1/cssutils/tests/test_profiles.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8255 2023-06-12 00:05:57.000000 cssutils-2.7.1/cssutils/tests/test_properties.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8692 2023-06-12 00:05:57.000000 cssutils-2.7.1/cssutils/tests/test_property.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2193 2023-06-12 00:05:57.000000 cssutils-2.7.1/cssutils/tests/test_scripts_csscombine.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15914 2023-06-12 00:05:57.000000 cssutils-2.7.1/cssutils/tests/test_selector.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4315 2023-06-12 00:05:57.000000 cssutils-2.7.1/cssutils/tests/test_selectorlist.py
+-rw-r--r--   0 runner    (1001) docker     (123)    25825 2023-06-12 00:05:57.000000 cssutils-2.7.1/cssutils/tests/test_serialize.py
+-rw-r--r--   0 runner    (1001) docker     (123)      634 2023-06-12 00:05:57.000000 cssutils-2.7.1/cssutils/tests/test_settings.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1020 2023-06-12 00:05:57.000000 cssutils-2.7.1/cssutils/tests/test_stylesheet.py
+-rw-r--r--   0 runner    (1001) docker     (123)    22391 2023-06-12 00:05:57.000000 cssutils-2.7.1/cssutils/tests/test_tokenize2.py
+-rw-r--r--   0 runner    (1001) docker     (123)    20706 2023-06-12 00:05:57.000000 cssutils-2.7.1/cssutils/tests/test_util.py
+-rw-r--r--   0 runner    (1001) docker     (123)    45998 2023-06-12 00:05:57.000000 cssutils-2.7.1/cssutils/tests/test_value.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1630 2023-06-12 00:05:57.000000 cssutils-2.7.1/cssutils/tests/test_x.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11762 2023-06-12 00:05:57.000000 cssutils-2.7.1/cssutils/tokenize2.py
+-rw-r--r--   0 runner    (1001) docker     (123)    34381 2023-06-12 00:05:57.000000 cssutils-2.7.1/cssutils/util.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-12 00:06:22.467588 cssutils-2.7.1/cssutils.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     8205 2023-06-12 00:06:22.000000 cssutils-2.7.1/cssutils.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     8903 2023-06-12 00:06:22.000000 cssutils-2.7.1/cssutils.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-12 00:06:22.000000 cssutils-2.7.1/cssutils.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      152 2023-06-12 00:06:22.000000 cssutils-2.7.1/cssutils.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      438 2023-06-12 00:06:22.000000 cssutils-2.7.1/cssutils.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       18 2023-06-12 00:06:22.000000 cssutils-2.7.1/cssutils.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-12 00:06:22.483588 cssutils-2.7.1/docs/
+-rw-r--r--   0 runner    (1001) docker     (123)     2272 2023-06-12 00:05:57.000000 cssutils-2.7.1/docs/backlog.rst
+-rw-r--r--   0 runner    (1001) docker     (123)       90 2023-06-12 00:05:57.000000 cssutils-2.7.1/docs/codec.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     1395 2023-06-12 00:05:57.000000 cssutils-2.7.1/docs/conf.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8701 2023-06-12 00:05:57.000000 cssutils-2.7.1/docs/css.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      110 2023-06-12 00:05:57.000000 cssutils-2.7.1/docs/encutils.rst
+-rw-r--r--   0 runner    (1001) docker     (123)       81 2023-06-12 00:05:57.000000 cssutils-2.7.1/docs/history.rst
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-12 00:06:22.483588 cssutils-2.7.1/docs/html/
+-rw-r--r--   0 runner    (1001) docker     (123)      234 2023-06-12 00:05:57.000000 cssutils-2.7.1/docs/html/.buildinfo
+-rw-r--r--   0 runner    (1001) docker     (123)   217445 2023-06-12 00:05:57.000000 cssutils-2.7.1/docs/html/CHANGELOG.html
+-rw-r--r--   0 runner    (1001) docker     (123)    17807 2023-06-12 00:05:57.000000 cssutils-2.7.1/docs/html/README.html
+-rw-r--r--   0 runner    (1001) docker     (123)     3665 2023-06-12 00:05:57.000000 cssutils-2.7.1/docs/html/_2to3 py3.html
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-12 00:06:22.483588 cssutils-2.7.1/docs/html/_sources/
+-rw-r--r--   0 runner    (1001) docker     (123)   116989 2023-06-12 00:05:57.000000 cssutils-2.7.1/docs/html/_sources/CHANGELOG.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     5751 2023-06-12 00:05:57.000000 cssutils-2.7.1/docs/html/_sources/README.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-12 00:06:22.487588 cssutils-2.7.1/docs/html/_sources/docs/
+-rw-r--r--   0 runner    (1001) docker     (123)     2452 2023-06-12 00:05:57.000000 cssutils-2.7.1/docs/html/_sources/docs/backlog.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       96 2023-06-12 00:05:57.000000 cssutils-2.7.1/docs/html/_sources/docs/codec.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     8751 2023-06-12 00:05:57.000000 cssutils-2.7.1/docs/html/_sources/docs/css.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     6138 2023-06-12 00:05:57.000000 cssutils-2.7.1/docs/html/_sources/docs/cssstyledeclaration.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      133 2023-06-12 00:05:57.000000 cssutils-2.7.1/docs/html/_sources/docs/cssutils.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      117 2023-06-12 00:05:57.000000 cssutils-2.7.1/docs/html/_sources/docs/encutils.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     2812 2023-06-12 00:05:57.000000 cssutils-2.7.1/docs/html/_sources/docs/implementation.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      967 2023-06-12 00:05:57.000000 cssutils-2.7.1/docs/html/_sources/docs/logging.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     8190 2023-06-12 00:05:57.000000 cssutils-2.7.1/docs/html/_sources/docs/migrate.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     2481 2023-06-12 00:05:57.000000 cssutils-2.7.1/docs/html/_sources/docs/parse.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     2535 2023-06-12 00:05:57.000000 cssutils-2.7.1/docs/html/_sources/docs/profiles.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     6932 2023-06-12 00:05:57.000000 cssutils-2.7.1/docs/html/_sources/docs/scripts.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     1818 2023-06-12 00:05:57.000000 cssutils-2.7.1/docs/html/_sources/docs/serialize.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     1120 2023-06-12 00:05:57.000000 cssutils-2.7.1/docs/html/_sources/docs/settings.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      758 2023-06-12 00:05:57.000000 cssutils-2.7.1/docs/html/_sources/docs/stylesheets.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      359 2023-06-12 00:05:57.000000 cssutils-2.7.1/docs/html/_sources/docs/utilities.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      447 2023-06-12 00:05:57.000000 cssutils-2.7.1/docs/html/_sources/docs/variables.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     1240 2023-06-12 00:05:57.000000 cssutils-2.7.1/docs/html/_sources/index.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-12 00:06:22.487588 cssutils-2.7.1/docs/html/_static/
+-rw-r--r--   0 runner    (1001) docker     (123)     8269 2023-06-12 00:05:57.000000 cssutils-2.7.1/docs/html/_static/basic.css
+-rw-r--r--   0 runner    (1001) docker     (123)     4040 2023-06-12 00:05:57.000000 cssutils-2.7.1/docs/html/_static/default.css
+-rw-r--r--   0 runner    (1001) docker     (123)     6871 2023-06-12 00:05:57.000000 cssutils-2.7.1/docs/html/_static/doctools.js
+-rw-r--r--   0 runner    (1001) docker     (123)      392 2023-06-12 00:05:57.000000 cssutils-2.7.1/docs/html/_static/file.png
+-rw-r--r--   0 runner    (1001) docker     (123)    72174 2023-06-12 00:05:57.000000 cssutils-2.7.1/docs/html/_static/jquery.js
+-rw-r--r--   0 runner    (1001) docker     (123)      199 2023-06-12 00:05:57.000000 cssutils-2.7.1/docs/html/_static/minus.png
+-rw-r--r--   0 runner    (1001) docker     (123)      199 2023-06-12 00:05:57.000000 cssutils-2.7.1/docs/html/_static/plus.png
+-rw-r--r--   0 runner    (1001) docker     (123)     3993 2023-06-12 00:05:57.000000 cssutils-2.7.1/docs/html/_static/pygments.css
+-rw-r--r--   0 runner    (1001) docker     (123)    14509 2023-06-12 00:05:57.000000 cssutils-2.7.1/docs/html/_static/searchtools.js
+-rw-r--r--   0 runner    (1001) docker     (123)     4634 2023-06-12 00:05:57.000000 cssutils-2.7.1/docs/html/_static/sidebar.js
+-rw-r--r--   0 runner    (1001) docker     (123)     8205 2023-06-12 00:05:57.000000 cssutils-2.7.1/docs/html/_static/underscore.js
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-12 00:06:22.491588 cssutils-2.7.1/docs/html/docs/
+-rw-r--r--   0 runner    (1001) docker     (123)    10377 2023-06-12 00:05:57.000000 cssutils-2.7.1/docs/html/docs/backlog.html
+-rw-r--r--   0 runner    (1001) docker     (123)     4328 2023-06-12 00:05:57.000000 cssutils-2.7.1/docs/html/docs/codec.html
+-rw-r--r--   0 runner    (1001) docker     (123)   167032 2023-06-12 00:05:57.000000 cssutils-2.7.1/docs/html/docs/css.html
+-rw-r--r--   0 runner    (1001) docker     (123)    24168 2023-06-12 00:05:57.000000 cssutils-2.7.1/docs/html/docs/encutils.html
+-rw-r--r--   0 runner    (1001) docker     (123)     6609 2023-06-12 00:05:57.000000 cssutils-2.7.1/docs/html/docs/logging.html
+-rw-r--r--   0 runner    (1001) docker     (123)    27207 2023-06-12 00:05:57.000000 cssutils-2.7.1/docs/html/docs/migrate.html
+-rw-r--r--   0 runner    (1001) docker     (123)    28207 2023-06-12 00:05:57.000000 cssutils-2.7.1/docs/html/docs/parse.html
+-rw-r--r--   0 runner    (1001) docker     (123)    22715 2023-06-12 00:05:57.000000 cssutils-2.7.1/docs/html/docs/profiles.html
+-rw-r--r--   0 runner    (1001) docker     (123)    18744 2023-06-12 00:05:57.000000 cssutils-2.7.1/docs/html/docs/scripts.html
+-rw-r--r--   0 runner    (1001) docker     (123)    15756 2023-06-12 00:05:57.000000 cssutils-2.7.1/docs/html/docs/serialize.html
+-rw-r--r--   0 runner    (1001) docker     (123)     6593 2023-06-12 00:05:57.000000 cssutils-2.7.1/docs/html/docs/settings.html
+-rw-r--r--   0 runner    (1001) docker     (123)    21169 2023-06-12 00:05:57.000000 cssutils-2.7.1/docs/html/docs/stylesheets.html
+-rw-r--r--   0 runner    (1001) docker     (123)    11209 2023-06-12 00:05:57.000000 cssutils-2.7.1/docs/html/docs/utilities.html
+-rw-r--r--   0 runner    (1001) docker     (123)     4762 2023-06-12 00:05:57.000000 cssutils-2.7.1/docs/html/docs/variables.html
+-rw-r--r--   0 runner    (1001) docker     (123)    50793 2023-06-12 00:05:57.000000 cssutils-2.7.1/docs/html/genindex.html
+-rw-r--r--   0 runner    (1001) docker     (123)    20302 2023-06-12 00:05:57.000000 cssutils-2.7.1/docs/html/index.html
+-rw-r--r--   0 runner    (1001) docker     (123)     5133 2023-06-12 00:05:57.000000 cssutils-2.7.1/docs/html/py-modindex.html
+-rw-r--r--   0 runner    (1001) docker     (123)     3370 2023-06-12 00:05:57.000000 cssutils-2.7.1/docs/html/search.html
+-rw-r--r--   0 runner    (1001) docker     (123)    42048 2023-06-12 00:05:57.000000 cssutils-2.7.1/docs/html/searchindex.js
+-rw-r--r--   0 runner    (1001) docker     (123)      691 2023-06-12 00:05:57.000000 cssutils-2.7.1/docs/index.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     2672 2023-06-12 00:05:57.000000 cssutils-2.7.1/docs/known issues.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      944 2023-06-12 00:05:57.000000 cssutils-2.7.1/docs/logging.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     7988 2023-06-12 00:05:57.000000 cssutils-2.7.1/docs/migrate.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     2503 2023-06-12 00:05:57.000000 cssutils-2.7.1/docs/parse.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     2475 2023-06-12 00:05:57.000000 cssutils-2.7.1/docs/profiles.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     6881 2023-06-12 00:05:57.000000 cssutils-2.7.1/docs/scripts.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     1773 2023-06-12 00:05:57.000000 cssutils-2.7.1/docs/serialize.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     1095 2023-06-12 00:05:57.000000 cssutils-2.7.1/docs/settings.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      728 2023-06-12 00:05:57.000000 cssutils-2.7.1/docs/stylesheets.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      341 2023-06-12 00:05:57.000000 cssutils-2.7.1/docs/utilities.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      414 2023-06-12 00:05:57.000000 cssutils-2.7.1/docs/variables.rst
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-12 00:06:22.491588 cssutils-2.7.1/encutils/
+-rw-r--r--   0 runner    (1001) docker     (123)    21282 2023-06-12 00:05:57.000000 cssutils-2.7.1/encutils/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-12 00:06:22.491588 cssutils-2.7.1/examples/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-12 00:05:57.000000 cssutils-2.7.1/examples/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2929 2023-06-12 00:05:57.000000 cssutils-2.7.1/examples/build.py
+-rw-r--r--   0 runner    (1001) docker     (123)      332 2023-06-12 00:05:57.000000 cssutils-2.7.1/examples/codec.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1668 2023-06-12 00:05:57.000000 cssutils-2.7.1/examples/cssencodings.py
+-rw-r--r--   0 runner    (1001) docker     (123)      683 2023-06-12 00:05:57.000000 cssutils-2.7.1/examples/customlog.py
+-rw-r--r--   0 runner    (1001) docker     (123)      894 2023-06-12 00:05:57.000000 cssutils-2.7.1/examples/imports.py
+-rw-r--r--   0 runner    (1001) docker     (123)      561 2023-06-12 00:05:57.000000 cssutils-2.7.1/examples/minify.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1370 2023-06-12 00:05:57.000000 cssutils-2.7.1/examples/parse.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1482 2023-06-12 00:05:57.000000 cssutils-2.7.1/examples/properties_with_same_name.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1404 2023-06-12 00:05:57.000000 cssutils-2.7.1/examples/selectors_tolower.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1775 2023-06-12 00:05:57.000000 cssutils-2.7.1/examples/serialize.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7237 2023-06-12 00:05:57.000000 cssutils-2.7.1/examples/style.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1341 2023-06-12 00:05:57.000000 cssutils-2.7.1/examples/styledeclaration.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2159 2023-06-12 00:05:57.000000 cssutils-2.7.1/examples/testutil.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5683 2023-06-12 00:05:57.000000 cssutils-2.7.1/examples/website.py
+-rw-r--r--   0 runner    (1001) docker     (123)      154 2023-06-12 00:05:57.000000 cssutils-2.7.1/mypy.ini
+-rw-r--r--   0 runner    (1001) docker     (123)      376 2023-06-12 00:05:57.000000 cssutils-2.7.1/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)      842 2023-06-12 00:05:57.000000 cssutils-2.7.1/pytest.ini
+-rw-r--r--   0 runner    (1001) docker     (123)       70 2023-06-12 00:05:57.000000 cssutils-2.7.1/ruff.toml
+-rw-r--r--   0 runner    (1001) docker     (123)     1684 2023-06-12 00:06:22.503588 cssutils-2.7.1/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-12 00:06:22.499588 cssutils-2.7.1/sheets/
+-rw-r--r--   0 runner    (1001) docker     (123)     4249 2023-06-12 00:05:57.000000 cssutils-2.7.1/sheets/096.css
+-rw-r--r--   0 runner    (1001) docker     (123)     4249 2023-06-12 00:05:57.000000 cssutils-2.7.1/sheets/097.css
+-rw-r--r--   0 runner    (1001) docker     (123)       59 2023-06-12 00:05:57.000000 cssutils-2.7.1/sheets/1.css
+-rw-r--r--   0 runner    (1001) docker     (123)       71 2023-06-12 00:05:57.000000 cssutils-2.7.1/sheets/1ascii.css
+-rw-r--r--   0 runner    (1001) docker     (123)       55 2023-06-12 00:05:57.000000 cssutils-2.7.1/sheets/1import.css
+-rw-r--r--   0 runner    (1001) docker     (123)       32 2023-06-12 00:05:57.000000 cssutils-2.7.1/sheets/1inherit-ascii.css
+-rw-r--r--   0 runner    (1001) docker     (123)       68 2023-06-12 00:05:57.000000 cssutils-2.7.1/sheets/1inherit-iso.css
+-rw-r--r--   0 runner    (1001) docker     (123)       30 2023-06-12 00:05:57.000000 cssutils-2.7.1/sheets/1inherit-utf8.css
+-rw-r--r--   0 runner    (1001) docker     (123)       65 2023-06-12 00:05:57.000000 cssutils-2.7.1/sheets/1utf.css
+-rw-r--r--   0 runner    (1001) docker     (123)       39 2023-06-12 00:05:57.000000 cssutils-2.7.1/sheets/2inherit-iso.css
+-rw-r--r--   0 runner    (1001) docker     (123)       36 2023-06-12 00:05:57.000000 cssutils-2.7.1/sheets/2resolve.css
+-rw-r--r--   0 runner    (1001) docker     (123)     9502 2023-06-12 00:05:57.000000 cssutils-2.7.1/sheets/acid2.css
+-rw-r--r--   0 runner    (1001) docker     (123)      264 2023-06-12 00:05:57.000000 cssutils-2.7.1/sheets/all.css
+-rw-r--r--   0 runner    (1001) docker     (123)      137 2023-06-12 00:05:57.000000 cssutils-2.7.1/sheets/atrule.css
+-rw-r--r--   0 runner    (1001) docker     (123)       73 2023-06-12 00:05:57.000000 cssutils-2.7.1/sheets/bad.css
+-rw-r--r--   0 runner    (1001) docker     (123)       98 2023-06-12 00:05:57.000000 cssutils-2.7.1/sheets/basic.css
+-rw-r--r--   0 runner    (1001) docker     (123)   208303 2023-06-12 00:05:57.000000 cssutils-2.7.1/sheets/bundle.css
+-rw-r--r--   0 runner    (1001) docker     (123)       83 2023-06-12 00:05:57.000000 cssutils-2.7.1/sheets/cases.css
+-rw-r--r--   0 runner    (1001) docker     (123)       97 2023-06-12 00:05:57.000000 cssutils-2.7.1/sheets/csscombine-1.css
+-rw-r--r--   0 runner    (1001) docker     (123)      111 2023-06-12 00:05:57.000000 cssutils-2.7.1/sheets/csscombine-2.css
+-rw-r--r--   0 runner    (1001) docker     (123)      220 2023-06-12 00:05:57.000000 cssutils-2.7.1/sheets/csscombine-proxy.css
+-rw-r--r--   0 runner    (1001) docker     (123)     3851 2023-06-12 00:05:57.000000 cssutils-2.7.1/sheets/cthedot_default.css
+-rw-r--r--   0 runner    (1001) docker     (123)     2797 2023-06-12 00:05:57.000000 cssutils-2.7.1/sheets/default_html4.css
+-rw-r--r--   0 runner    (1001) docker     (123)      733 2023-06-12 00:05:57.000000 cssutils-2.7.1/sheets/hacks.css
+-rw-r--r--   0 runner    (1001) docker     (123)      124 2023-06-12 00:05:57.000000 cssutils-2.7.1/sheets/html.css
+-rw-r--r--   0 runner    (1001) docker     (123)     1503 2023-06-12 00:05:57.000000 cssutils-2.7.1/sheets/html20.css
+-rw-r--r--   0 runner    (1001) docker     (123)     4274 2023-06-12 00:05:57.000000 cssutils-2.7.1/sheets/html40.css
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-12 00:06:22.499588 cssutils-2.7.1/sheets/images/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-12 00:05:57.000000 cssutils-2.7.1/sheets/images/example.gif
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-12 00:06:22.499588 cssutils-2.7.1/sheets/import/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-12 00:06:22.499588 cssutils-2.7.1/sheets/import/images2/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-12 00:05:57.000000 cssutils-2.7.1/sheets/import/images2/example2.gif
+-rw-r--r--   0 runner    (1001) docker     (123)       88 2023-06-12 00:05:57.000000 cssutils-2.7.1/sheets/import/import-impossible.css
+-rw-r--r--   0 runner    (1001) docker     (123)      427 2023-06-12 00:05:57.000000 cssutils-2.7.1/sheets/import/import2.css
+-rw-r--r--   0 runner    (1001) docker     (123)      113 2023-06-12 00:05:57.000000 cssutils-2.7.1/sheets/import.css
+-rw-r--r--   0 runner    (1001) docker     (123)      307 2023-06-12 00:05:57.000000 cssutils-2.7.1/sheets/import3.css
+-rw-r--r--   0 runner    (1001) docker     (123)     9402 2023-06-12 00:05:57.000000 cssutils-2.7.1/sheets/ll.css
+-rw-r--r--   0 runner    (1001) docker     (123)    97995 2023-06-12 00:05:57.000000 cssutils-2.7.1/sheets/ll2.css
+-rw-r--r--   0 runner    (1001) docker     (123)       29 2023-06-12 00:05:57.000000 cssutils-2.7.1/sheets/multiple-values.css
+-rw-r--r--   0 runner    (1001) docker     (123)       41 2023-06-12 00:05:57.000000 cssutils-2.7.1/sheets/page_test.css
+-rw-r--r--   0 runner    (1001) docker     (123)    17998 2023-06-12 00:05:57.000000 cssutils-2.7.1/sheets/sample_5.css
+-rw-r--r--   0 runner    (1001) docker     (123)     7662 2023-06-12 00:05:57.000000 cssutils-2.7.1/sheets/sample_7.css
+-rw-r--r--   0 runner    (1001) docker     (123)      305 2023-06-12 00:05:57.000000 cssutils-2.7.1/sheets/simple.css
+-rw-r--r--   0 runner    (1001) docker     (123)      113 2023-06-12 00:05:57.000000 cssutils-2.7.1/sheets/single-color.css
+-rw-r--r--   0 runner    (1001) docker     (123)    18645 2023-06-12 00:05:57.000000 cssutils-2.7.1/sheets/slashcode.css
+-rw-r--r--   0 runner    (1001) docker     (123)      677 2023-06-12 00:05:57.000000 cssutils-2.7.1/sheets/t-HACKS.css
+-rw-r--r--   0 runner    (1001) docker     (123)     9268 2023-06-12 00:05:57.000000 cssutils-2.7.1/sheets/test-unicode.css
+-rw-r--r--   0 runner    (1001) docker     (123)     4369 2023-06-12 00:05:57.000000 cssutils-2.7.1/sheets/test.css
+-rw-r--r--   0 runner    (1001) docker     (123)     8665 2023-06-12 00:05:57.000000 cssutils-2.7.1/sheets/tigris.css
+-rw-r--r--   0 runner    (1001) docker     (123)     9082 2023-06-12 00:05:57.000000 cssutils-2.7.1/sheets/tigris2.css
+-rw-r--r--   0 runner    (1001) docker     (123)      296 2023-06-12 00:05:57.000000 cssutils-2.7.1/sheets/u_simple.css
+-rw-r--r--   0 runner    (1001) docker     (123)       29 2023-06-12 00:05:57.000000 cssutils-2.7.1/sheets/v_simple.css
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-12 00:06:22.503588 cssutils-2.7.1/sheets/var/
+-rw-r--r--   0 runner    (1001) docker     (123)      133 2023-06-12 00:05:57.000000 cssutils-2.7.1/sheets/var/start.css
+-rw-r--r--   0 runner    (1001) docker     (123)      290 2023-06-12 00:05:57.000000 cssutils-2.7.1/sheets/var/use.css
+-rw-r--r--   0 runner    (1001) docker     (123)       41 2023-06-12 00:05:57.000000 cssutils-2.7.1/sheets/var/vars.css
+-rw-r--r--   0 runner    (1001) docker     (123)       33 2023-06-12 00:05:57.000000 cssutils-2.7.1/sheets/var/vars2.css
+-rw-r--r--   0 runner    (1001) docker     (123)      222 2023-06-12 00:05:57.000000 cssutils-2.7.1/sheets/vars.css
+-rw-r--r--   0 runner    (1001) docker     (123)      254 2023-06-12 00:05:57.000000 cssutils-2.7.1/sheets/varsimport.css
+-rw-r--r--   0 runner    (1001) docker     (123)     4910 2023-06-12 00:05:57.000000 cssutils-2.7.1/sheets/xhtml2.css
+-rw-r--r--   0 runner    (1001) docker     (123)     4825 2023-06-12 00:05:57.000000 cssutils-2.7.1/sheets/xhtml22.css
+-rw-r--r--   0 runner    (1001) docker     (123)      117 2023-06-12 00:05:57.000000 cssutils-2.7.1/sheets/yuck.css
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-12 00:06:22.503588 cssutils-2.7.1/tools/
+-rw-r--r--   0 runner    (1001) docker     (123)      767 2023-06-12 00:05:57.000000 cssutils-2.7.1/tools/speed.py
+-rw-r--r--   0 runner    (1001) docker     (123)    37536 2023-06-12 00:05:57.000000 cssutils-2.7.1/tools/try.py
+-rw-r--r--   0 runner    (1001) docker     (123)      795 2023-06-12 00:05:57.000000 cssutils-2.7.1/tox.ini
```

### Comparing `cssutils-2.7.0/.github/workflows/main.yml` & `cssutils-2.7.1/.github/workflows/main.yml`

 * *Files 6% similar despite different names*

```diff
@@ -86,24 +86,21 @@
         with:
           python-version: ${{ matrix.python }}${{ matrix.dev }}
       - name: Install tox
         run: |
           python -m pip install tox
       - name: Run tests
         run: tox
-    # workaround for #36
-    continue-on-error: true
 
   check:  # This job does nothing and is only used for the branch protection
     if: always()
 
     needs:
     - test
-    # workaround for #36
-    # - docs
+    - docs
 
     runs-on: ubuntu-latest
 
     steps:
     - name: Decide whether the needed jobs succeeded or failed
       uses: re-actors/alls-green@release/v1
       with:
```

### Comparing `cssutils-2.7.0/CHANGES.rst` & `cssutils-2.7.1/CHANGES.rst`

 * *Files 0% similar despite different names*

```diff
@@ -1,7 +1,12 @@
+v2.7.1
+======
+
+#36: Refactored to restore docs builds without warning-errors.
+
 v2.7.0
 ======
 
 #35: Updated deprecated usage of ``cgi`` module.
 
 #34: Updated deprecated setup/teardown from ``nose`` in tests.
```

### Comparing `cssutils-2.7.0/COPYING` & `cssutils-2.7.1/COPYING`

 * *Files identical despite different names*

### Comparing `cssutils-2.7.0/COPYING.LESSER` & `cssutils-2.7.1/COPYING.LESSER`

 * *Files identical despite different names*

### Comparing `cssutils-2.7.0/PKG-INFO` & `cssutils-2.7.1/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cssutils
-Version: 2.7.0
+Version: 2.7.1
 Summary: A CSS Cascading Style Sheets library for Python
 Home-page: https://github.com/jaraco/cssutils
 Author: Christof Hoeke
 Author-email: c@cthedot.de
 Maintainer: Jason R. Coombs
 Maintainer-email: jaraco@jaraco.com
 Keywords: CSS,Cascading Style Sheets,CSSParser,DOM Level 2 Stylesheets,DOM Level 2 CSS
@@ -81,18 +81,14 @@
 `CSSOM <http://dev.w3.org/csswg/cssom/>`__
     A few details (mainly the NamespaceRule DOM) are taken from here. Plan is to move implementation to the stuff defined here which is newer but still no REC so might change anytime...
 
 The cssutils tokenizer is a customized implementation of `CSS3 Module: Syntax (W3C Working Draft 13 August 2003) <http://www.w3.org/TR/css3-syntax/>`_ which itself is based on the CSS 2.1 tokenizer. It tries to be as compliant as possible but uses some (helpful) parts of the CSS 2.1 tokenizer.
 
 I guess cssutils is neither CSS 2.1 nor CSS 3 compliant but tries to at least be able to parse both grammars including some more real world cases (some CSS hacks are actually parsed and serialized). Both official grammars are not final nor bugfree but still feasible. cssutils aim is not to be fully compliant to any CSS specification (the specifications seem to be in a constant flow anyway) but cssutils *should* be able to read and write as many as possible CSS stylesheets "in the wild" while at the same time implement the official APIs which are well documented. Some minor extensions are provided as well.
 
-Please visit http://cthedot.de/cssutils/ or https://bitbucket.org/cthedot/cssutils/ for more details.
-
-There is also a low-traffic `cssutils discussion group <http://groups.google.com/group/cssutils>`_.
-
 
 Compatibility
 =============
 
 cssutils is developed on modern Python versions. Check the package metadata
 for compatibilty.
```

### Comparing `cssutils-2.7.0/README.rst` & `cssutils-2.7.1/README.rst`

 * *Files 2% similar despite different names*

```diff
@@ -57,18 +57,14 @@
 `CSSOM <http://dev.w3.org/csswg/cssom/>`__
     A few details (mainly the NamespaceRule DOM) are taken from here. Plan is to move implementation to the stuff defined here which is newer but still no REC so might change anytime...
 
 The cssutils tokenizer is a customized implementation of `CSS3 Module: Syntax (W3C Working Draft 13 August 2003) <http://www.w3.org/TR/css3-syntax/>`_ which itself is based on the CSS 2.1 tokenizer. It tries to be as compliant as possible but uses some (helpful) parts of the CSS 2.1 tokenizer.
 
 I guess cssutils is neither CSS 2.1 nor CSS 3 compliant but tries to at least be able to parse both grammars including some more real world cases (some CSS hacks are actually parsed and serialized). Both official grammars are not final nor bugfree but still feasible. cssutils aim is not to be fully compliant to any CSS specification (the specifications seem to be in a constant flow anyway) but cssutils *should* be able to read and write as many as possible CSS stylesheets "in the wild" while at the same time implement the official APIs which are well documented. Some minor extensions are provided as well.
 
-Please visit http://cthedot.de/cssutils/ or https://bitbucket.org/cthedot/cssutils/ for more details.
-
-There is also a low-traffic `cssutils discussion group <http://groups.google.com/group/cssutils>`_.
-
 
 Compatibility
 =============
 
 cssutils is developed on modern Python versions. Check the package metadata
 for compatibilty.
```

### Comparing `cssutils-2.7.0/conftest.py` & `cssutils-2.7.1/conftest.py`

 * *Files identical despite different names*

### Comparing `cssutils-2.7.0/cssutils/__init__.py` & `cssutils-2.7.1/cssutils/__init__.py`

 * *Files identical despite different names*

### Comparing `cssutils-2.7.0/cssutils/_fetch.py` & `cssutils-2.7.1/cssutils/_fetch.py`

 * *Files identical despite different names*

### Comparing `cssutils-2.7.0/cssutils/_fetchgae.py` & `cssutils-2.7.1/cssutils/_fetchgae.py`

 * *Files identical despite different names*

### Comparing `cssutils-2.7.0/cssutils/codec.py` & `cssutils-2.7.1/cssutils/codec.py`

 * *Files identical despite different names*

### Comparing `cssutils-2.7.0/cssutils/css/__init__.py` & `cssutils-2.7.1/cssutils/css/__init__.py`

 * *Files identical despite different names*

### Comparing `cssutils-2.7.0/cssutils/css/colors.py` & `cssutils-2.7.1/cssutils/css/colors.py`

 * *Files identical despite different names*

### Comparing `cssutils-2.7.0/cssutils/css/csscharsetrule.py` & `cssutils-2.7.1/cssutils/css/csscharsetrule.py`

 * *Files identical despite different names*

### Comparing `cssutils-2.7.0/cssutils/css/csscomment.py` & `cssutils-2.7.1/cssutils/css/csscomment.py`

 * *Files identical despite different names*

### Comparing `cssutils-2.7.0/cssutils/css/cssfontfacerule.py` & `cssutils-2.7.1/cssutils/css/cssfontfacerule.py`

 * *Files identical despite different names*

### Comparing `cssutils-2.7.0/cssutils/css/cssimportrule.py` & `cssutils-2.7.1/cssutils/css/cssimportrule.py`

 * *Files 2% similar despite different names*

```diff
@@ -403,16 +403,19 @@
             # set title of imported sheet
             if self.styleSheet:
                 self.styleSheet.title = name
 
         else:
             self._log.error('CSSImportRule: Not a valid name: %s' % name)
 
+    def _getName(self):
+        return self._name
+
     name = property(
-        lambda self: self._name,
+        _getName,
         _setName,
         doc="An optional name for the imported sheet.",
     )
 
     styleSheet = property(
         lambda self: self._styleSheet,
         doc="(readonly) The style sheet referred to by this " "rule.",
```

### Comparing `cssutils-2.7.0/cssutils/css/cssmediarule.py` & `cssutils-2.7.1/cssutils/css/cssmediarule.py`

 * *Files 1% similar despite different names*

```diff
@@ -257,27 +257,32 @@
 
     cssText = property(
         _getCssText,
         _setCssText,
         doc="(DOM) The parsable textual representation of this " "rule.",
     )
 
-    def _setName(self, name):
+    @property
+    def name(self):
+        """An optional name for this media rule."""
+        return self._name
+
+    @name.setter
+    def name(self, name):
         if isinstance(name, str) or name is None:
             # "" or ''
             if not name:
                 name = None
 
             self._name = name
         else:
             self._log.error('CSSImportRule: Not a valid name: %s' % name)
 
-    name = property(
-        lambda self: self._name, _setName, doc="An optional name for this media rule."
-    )
+    def _setName(self, name):
+        self.name = name
 
     def _setMedia(self, media):
         """
         :param media:
             a :class:`~cssutils.stylesheets.MediaList` or string
         """
         self._checkReadonly()
```

### Comparing `cssutils-2.7.0/cssutils/css/cssnamespacerule.py` & `cssutils-2.7.1/cssutils/css/cssnamespacerule.py`

 * *Files identical despite different names*

### Comparing `cssutils-2.7.0/cssutils/css/csspagerule.py` & `cssutils-2.7.1/cssutils/css/csspagerule.py`

 * *Files identical despite different names*

### Comparing `cssutils-2.7.0/cssutils/css/cssproperties.py` & `cssutils-2.7.1/cssutils/css/cssproperties.py`

 * *Files identical despite different names*

### Comparing `cssutils-2.7.0/cssutils/css/cssrule.py` & `cssutils-2.7.1/cssutils/css/cssrule.py`

 * *Files 2% similar despite different names*

```diff
@@ -113,17 +113,18 @@
         lambda self: '',
         _setCssText,
         doc="(DOM) The parsable textual representation of the "
         "rule. This reflects the current state of the rule "
         "and not its initial value.",
     )
 
-    parent = property(
-        lambda self: self._parent, doc="The Parent Node of this CSSRule or None."
-    )
+    @property
+    def parent(self):
+        """The Parent Node of this CSSRule or None."""
+        return self._parent
 
     parentRule = property(
         lambda self: self._parentRule,
         doc="If this rule is contained inside another rule "
         "(e.g. a style rule inside an @media block), this "
         "is the containing rule. If this rule is not nested "
         "inside any other rules, this returns None.",
@@ -250,30 +251,26 @@
         if isinstance(rule, str):
             tempsheet = cssutils.css.CSSStyleSheet()
             tempsheet.cssText = rule
             if len(tempsheet.cssRules) != 1 or (
                 tempsheet.cssRules
                 and not isinstance(tempsheet.cssRules[0], cssutils.css.CSSRule)
             ):
-                self._log.error(
-                    '{}: Invalid Rule: {}'.format(self.__class__.__name__, rule)
-                )
+                self._log.error(f'{self.__class__.__name__}: Invalid Rule: {rule}')
                 return False, False
             rule = tempsheet.cssRules[0]
 
         elif isinstance(rule, cssutils.css.CSSRuleList):
             # insert all rules
             for i, r in enumerate(rule):
                 self.insertRule(r, index + i)
             return True, True
 
         elif not isinstance(rule, cssutils.css.CSSRule):
-            self._log.error(
-                '{}: Not a CSSRule: {}'.format(rule, self.__class__.__name__)
-            )
+            self._log.error(f'{rule}: Not a CSSRule: {self.__class__.__name__}')
             return False, False
 
         return rule, index
 
     def _finishInsertRule(self, rule, index):
         "add `rule` at `index`"
         rule._parentRule = self
```

### Comparing `cssutils-2.7.0/cssutils/css/cssrulelist.py` & `cssutils-2.7.1/cssutils/css/cssrulelist.py`

 * *Files 7% similar despite different names*

```diff
@@ -39,17 +39,18 @@
         CSSRuleList, or None if that is not a valid index.
         """
         try:
             return self[index]
         except IndexError:
             return None
 
-    length = property(
-        lambda self: len(self), doc="(DOM) The number of CSSRules in the list."
-    )
+    @property
+    def length(self):
+        """(DOM) The number of CSSRules in the list."""
+        return len(self)
 
     def rulesOfType(self, type):
         """Yield the rules which have the given `type` only, one of the
         constants defined in :class:`cssutils.css.CSSRule`."""
         for r in self:
             if r.type == type:
                 yield r
```

### Comparing `cssutils-2.7.0/cssutils/css/cssstyledeclaration.py` & `cssutils-2.7.1/cssutils/css/cssstyledeclaration.py`

 * *Files 1% similar despite different names*

```diff
@@ -662,15 +662,15 @@
             # not yet set or forced omit replace
             newp.parent = self
             self.seq._readonly = False
             self.seq.append(newp, 'Property')
             self.seq._readonly = True
 
         else:
-            self._log.warn('Invalid Property: {}: {} {}'.format(name, value, priority))
+            self._log.warn(f'Invalid Property: {name}: {value} {priority}')
 
     def item(self, index):
         """(DOM) Retrieve the properties that have been explicitly set in
         this declaration block. The order of the properties retrieved using
         this method does not have to be the order in which they were set.
         This method can be used to iterate over all properties in this
         declaration block.
```

### Comparing `cssutils-2.7.0/cssutils/css/cssstylerule.py` & `cssutils-2.7.1/cssutils/css/cssstylerule.py`

 * *Files identical despite different names*

### Comparing `cssutils-2.7.0/cssutils/css/cssstylesheet.py` & `cssutils-2.7.1/cssutils/css/cssstylesheet.py`

 * *Files 0% similar despite different names*

```diff
@@ -452,17 +452,18 @@
     encoding = property(
         _getEncoding,
         _setEncoding,
         "(cssutils) Reflect encoding of an @charset rule or 'utf-8' "
         "(default) if set to ``None``",
     )
 
-    namespaces = property(
-        lambda self: self._namespaces, doc="All Namespaces used in this CSSStyleSheet."
-    )
+    @property
+    def namespaces(self):
+        """All Namespaces used in this CSSStyleSheet."""
+        return self._namespaces
 
     def _updateVariables(self):
         """Updates self._variables, called when @import or @variables rules
         is added to sheet.
         """
         for r in self.cssRules.rulesOfType(CSSRule.IMPORT_RULE):
             s = r.styleSheet
```

### Comparing `cssutils-2.7.0/cssutils/css/cssunknownrule.py` & `cssutils-2.7.1/cssutils/css/cssunknownrule.py`

 * *Files identical despite different names*

### Comparing `cssutils-2.7.0/cssutils/css/cssvalue.py` & `cssutils-2.7.1/cssutils/css/cssvalue.py`

 * *Files 1% similar despite different names*

```diff
@@ -58,15 +58,15 @@
                 cssText = '%f' % cssText  # if it is a floating point number
 
             self.cssText = cssText
 
         self._readonly = readonly
 
     def __repr__(self):
-        return "cssutils.css.{}({!r})".format(self.__class__.__name__, self.cssText)
+        return f"cssutils.css.{self.__class__.__name__}({self.cssText!r})"
 
     def __str__(self):
         return (
             "<cssutils.css.%s object cssValueTypeString=%r cssText=%r at "
             "0x%x>"
             % (self.__class__.__name__, self.cssValueTypeString, self.cssText, id(self))
         )
@@ -796,15 +796,15 @@
                         self._getCSSPrimitiveTypeString(unitType),
                     )
                 )
 
         if val == int(val):
             val = int(val)
 
-        self.cssText = '{}{}'.format(val, dim)
+        self.cssText = f'{val}{dim}'
 
     def getStringValue(self):
         """(DOM) This method is used to get the string value. If the
         CSS value doesn't contain a string value, a DOMException is raised.
 
         Some properties (like 'font-family' or 'voice-family')
         convert a whitespace separated list of idents to a string.
@@ -1128,15 +1128,15 @@
             except AttributeError:
                 pass
             self.cssText = cssText
 
         self._readonly = readonly
 
     def __repr__(self):
-        return "cssutils.css.{}({!r})".format(self.__class__.__name__, self.cssText)
+        return f"cssutils.css.{self.__class__.__name__}({self.cssText!r})"
 
     def __str__(self):
         return "<cssutils.css.{} object colorType={!r} cssText={!r} at 0x{:x}>".format(
             self.__class__.__name__,
             self.colorType,
             self.cssText,
             id(self),
@@ -1309,15 +1309,15 @@
         :param readonly:
             defaults to False
         """
         self._name = None
         super().__init__(cssText=cssText, parent=parent, readonly=readonly)
 
     def __repr__(self):
-        return "cssutils.css.{}({!r})".format(self.__class__.__name__, self.cssText)
+        return f"cssutils.css.{self.__class__.__name__}({self.cssText!r})"
 
     def __str__(self):
         return "<cssutils.css.{} object name={!r} value={!r} at 0x{:x}>".format(
             self.__class__.__name__,
             self.name,
             self.value,
             id(self),
```

### Comparing `cssutils-2.7.0/cssutils/css/cssvariablesdeclaration.py` & `cssutils-2.7.1/cssutils/css/cssvariablesdeclaration.py`

 * *Files 2% similar despite different names*

```diff
@@ -282,28 +282,24 @@
         self._checkReadonly()
 
         # check name
         wellformed, seq, store, unused = ProdParser().parse(
             normalize(variableName), 'variableName', Sequence(PreDef.ident())
         )
         if not wellformed:
-            self._log.error(
-                'Invalid variableName: {!r}: {!r}'.format(variableName, value)
-            )
+            self._log.error(f'Invalid variableName: {variableName!r}: {value!r}')
         else:
             # check value
             if isinstance(value, PropertyValue):
                 v = value
             else:
                 v = PropertyValue(cssText=value, parent=self)
 
             if not v.wellformed:
-                self._log.error(
-                    'Invalid variable value: {!r}: {!r}'.format(variableName, value)
-                )
+                self._log.error(f'Invalid variable value: {variableName!r}: {value!r}')
             else:
                 # update seq
                 self.seq._readonly = False
 
                 variableName = normalize(variableName)
 
                 if variableName in self._vars:
```

### Comparing `cssutils-2.7.0/cssutils/css/cssvariablesrule.py` & `cssutils-2.7.1/cssutils/css/cssvariablesrule.py`

 * *Files identical despite different names*

### Comparing `cssutils-2.7.0/cssutils/css/marginrule.py` & `cssutils-2.7.1/cssutils/css/marginrule.py`

 * *Files identical despite different names*

### Comparing `cssutils-2.7.0/cssutils/css/property.py` & `cssutils-2.7.1/cssutils/css/property.py`

 * *Files 2% similar despite different names*

```diff
@@ -286,15 +286,24 @@
     def _setValue(self, value):
         self._setPropertyValue(value)
 
     value = property(
         _getValue, _setValue, doc="The textual value of this Properties propertyValue."
     )
 
-    def _setPriority(self, priority):  # noqa: C901
+    def _setPriority(self, priority):
+        self.priority = priority
+
+    @property
+    def priority(self):
+        """Priority of this property."""
+        return self._priority
+
+    @priority.setter
+    def priority(self, priority):  # noqa: C901
         """
         priority
             a string, currently either u'', u'!important' or u'important'
 
         Format::
 
             prio
@@ -367,31 +376,27 @@
             self._literalpriority = new['literalpriority']
             self._priority = self._normalize(self.literalpriority)
             self.seqs[2] = newseq
             # validate priority
             if self._priority not in ('', 'important'):
                 self._log.error('Property: No CSS priority value: %s' % self._priority)
 
-    priority = property(
-        lambda self: self._priority, _setPriority, doc="Priority of this property."
-    )
-
     literalpriority = property(
         lambda self: self._literalpriority,
         doc="Readonly literal (not normalized) priority of this property",
     )
 
-    def _setParent(self, parent):
-        self._parent = parent
+    @property
+    def parent(self):
+        """The Parent Node (normally a CSSStyledeclaration) of this Property"""
+        return self._parent
 
-    parent = property(
-        lambda self: self._parent,
-        _setParent,
-        doc="The Parent Node (normally a CSSStyledeclaration) of this " "Property",
-    )
+    @parent.setter
+    def parent(self, parent):
+        self._parent = parent
 
     def validate(self):  # noqa: C901
         """Validate value against `profiles` which are checked dynamically.
         properties in e.g. @font-face rules are checked against
         ``cssutils.profile.CSS3_FONT_FACE`` only.
 
         For each of the following cases a message is reported:
```

### Comparing `cssutils-2.7.0/cssutils/css/selector.py` & `cssutils-2.7.1/cssutils/css/selector.py`

 * *Files 1% similar despite different names*

```diff
@@ -122,15 +122,15 @@
         self._readonly = readonly
 
     def __repr__(self):
         if self.__getNamespaces():
             st = (self.selectorText, self._getUsedNamespaces())
         else:
             st = self.selectorText
-        return "cssutils.css.{}(selectorText={!r})".format(self.__class__.__name__, st)
+        return f"cssutils.css.{self.__class__.__name__}(selectorText={st!r})"
 
     def __str__(self):
         return (
             "<cssutils.css.%s object selectorText=%r specificity=%r"
             " _namespaces=%r at 0x%x>"
             % (
                 self.__class__.__name__,
@@ -177,17 +177,18 @@
         "CSSStyleSheet the namespaces of that sheet "
         "are mirrored here. While the Selector (or "
         "parent SelectorList or parentRule(s) of that "
         "are not attached a own dict of {prefix: "
         "namespaceURI} is used.",
     )
 
-    element = property(
-        lambda self: self._element, doc="Effective element target of this selector."
-    )
+    @property
+    def element(self):
+        """Effective element target of this selector."""
+        return self._element
 
     parent = property(
         lambda self: self._parent,
         doc="(DOM) The SelectorList that contains this Selector "
         "or None if this Selector is not attached to a "
         "SelectorList.",
     )
```

### Comparing `cssutils-2.7.0/cssutils/css/selectorlist.py` & `cssutils-2.7.1/cssutils/css/selectorlist.py`

 * *Files 2% similar despite different names*

```diff
@@ -43,15 +43,15 @@
         self._readonly = readonly
 
     def __repr__(self):
         if self._namespaces:
             st = (self.selectorText, self._namespaces)
         else:
             st = self.selectorText
-        return "cssutils.css.{}(selectorText={!r})".format(self.__class__.__name__, st)
+        return f"cssutils.css.{self.__class__.__name__}(selectorText={st!r})"
 
     def __str__(self):
         return "<cssutils.css.%s object selectorText=%r _namespaces=%r at " "0x%x>" % (
             self.__class__.__name__,
             self.selectorText,
             self._namespaces,
             id(self),
```

### Comparing `cssutils-2.7.0/cssutils/css/value.py` & `cssutils-2.7.1/cssutils/css/value.py`

 * *Files 2% similar despite different names*

```diff
@@ -67,15 +67,15 @@
             return None
 
     def __iter__(self):
         "Generator which iterates over values."
         yield from self.__items()
 
     def __repr__(self):
-        return "cssutils.css.{}({!r})".format(self.__class__.__name__, self.cssText)
+        return f"cssutils.css.{self.__class__.__name__}({self.cssText!r})"
 
     def __str__(self):
         return "<cssutils.css.%s object length=%r cssText=%r at " "0x%x>" % (
             self.__class__.__name__,
             self.length,
             self.cssText,
             id(self),
@@ -250,15 +250,15 @@
         self.parent = parent
         self.wellformed = False
 
         if cssText:
             self.cssText = cssText
 
     def __repr__(self):
-        return "cssutils.css.{}({!r})".format(self.__class__.__name__, self.cssText)
+        return f"cssutils.css.{self.__class__.__name__}({self.cssText!r})"
 
     def __str__(self):
         return (
             "<cssutils.css.{} object type={} value={!r} cssText={!r} at 0x{:x}>".format(
                 self.__class__.__name__,
                 self.type,
                 self.value,
@@ -287,20 +287,22 @@
 
     cssText = property(
         lambda self: cssutils.ser.do_css_Value(self),
         _setCssText,
         doc='String value of this value.',
     )
 
-    type = property(
-        lambda self: self._type,  # _setType,
-        doc="Type of this value, for now the production type "
-        "like e.g. `DIMENSION` or `STRING`. All types are "
-        "defined as constants in :class:`~cssutils.css.Value`.",
-    )
+    @property
+    def type(self):
+        """
+        Type of this value, for now the production type
+        like e.g. `DIMENSION` or `STRING`. All types are
+        defined as constants in :class:`~cssutils.css.Value`.
+        """
+        return self._type
 
     def _setValue(self, value):
         # TODO: check!
         self._value = value
 
     value = property(
         lambda self: self._value,
@@ -489,17 +491,18 @@
     )
 
     value = property(
         lambda self: cssutils.ser.do_css_CSSFunction(self, True),
         doc='Same as cssText but without comments.',
     )
 
-    type = property(
-        lambda self: Value.COLOR_VALUE, doc="Type is fixed to Value.COLOR_VALUE."
-    )
+    @property
+    def type(self):
+        """Type is fixed to Value.COLOR_VALUE."""
+        return Value.COLOR_VALUE
 
     def _getName(self):
         for n, v in list(self.COLORS.items()):
             if v == (self.red, self.green, self.blue, self.alpha):
                 return n
 
     colorType = property(
@@ -508,23 +511,29 @@
     )
 
     name = property(
         _getName, doc='Name of the color if known (in ColorValue.COLORS) ' 'else None'
     )
 
     red = property(lambda self: self._red, doc='red part as integer between 0 and 255')
-    green = property(
-        lambda self: self._green, doc='green part as integer between 0 and 255'
-    )
-    blue = property(
-        lambda self: self._blue, doc='blue part as integer between 0 and 255'
-    )
-    alpha = property(
-        lambda self: self._alpha, doc='alpha part as float between 0.0 and 1.0'
-    )
+
+    @property
+    def green(self):
+        """green part as integer between 0 and 255"""
+        return self._green
+
+    @property
+    def blue(self):
+        """blue part as integer between 0 and 255"""
+        return self._blue
+
+    @property
+    def alpha(self):
+        """alpha part as float between 0.0 and 1.0"""
+        return self._alpha
 
 
 class DimensionValue(Value):
     """
     A numerical value with an optional dimension like e.g. "px" or "%".
 
     Covers DIMENSION, PERCENTAGE or NUMBER values.
@@ -924,17 +933,18 @@
     name = property(
         lambda self: self._name,
         doc="The name identifier of this variable referring to "
         "a value in a "
         ":class:`cssutils.css.CSSVariablesDeclaration`.",
     )
 
-    fallback = property(
-        lambda self: self._fallback, doc="The fallback Value of this variable"
-    )
+    @property
+    def fallback(self):
+        """The fallback Value of this variable"""
+        return self._fallback
 
     type = property(lambda self: Value.VARIABLE, doc="Type is fixed to Value.VARIABLE.")
 
     def _getValue(self):
         "Find contained sheet and @variables there"
         rel = self
         while True:
```

### Comparing `cssutils-2.7.0/cssutils/css2productions.py` & `cssutils-2.7.1/cssutils/css2productions.py`

 * *Files identical despite different names*

### Comparing `cssutils-2.7.0/cssutils/cssproductions.py` & `cssutils-2.7.1/cssutils/cssproductions.py`

 * *Files identical despite different names*

### Comparing `cssutils-2.7.0/cssutils/errorhandler.py` & `cssutils-2.7.1/cssutils/errorhandler.py`

 * *Files identical despite different names*

### Comparing `cssutils-2.7.0/cssutils/helper.py` & `cssutils-2.7.1/cssutils/helper.py`

 * *Files identical despite different names*

### Comparing `cssutils-2.7.0/cssutils/parse.py` & `cssutils-2.7.1/cssutils/parse.py`

 * *Files identical despite different names*

### Comparing `cssutils-2.7.0/cssutils/prodparser.py` & `cssutils-2.7.1/cssutils/prodparser.py`

 * *Files identical despite different names*

### Comparing `cssutils-2.7.0/cssutils/profiles.py` & `cssutils-2.7.1/cssutils/profiles.py`

 * *Files 1% similar despite different names*

```diff
@@ -207,17 +207,18 @@
     )
 
     profiles = property(
         lambda self: self._profileNames,
         doc='Names of all profiles in order as defined.',
     )
 
-    knownNames = property(
-        lambda self: self._knownNames, doc="All known property names of all profiles."
-    )
+    @property
+    def knownNames(self):
+        """All known property names of all profiles."""
+        return self._knownNames
 
     def _resetProperties(self, newMacros=None):
         "reset all props from raw values as changes in macros happened"
         # base
         macros = Profiles._TOKEN_MACROS.copy()
         macros.update(Profiles._MACROS.copy())
```

### Comparing `cssutils-2.7.0/cssutils/sac.py` & `cssutils-2.7.1/cssutils/sac.py`

 * *Files identical despite different names*

### Comparing `cssutils-2.7.0/cssutils/script.py` & `cssutils-2.7.1/cssutils/script.py`

 * *Files identical despite different names*

### Comparing `cssutils-2.7.0/cssutils/scripts/csscapture.py` & `cssutils-2.7.1/cssutils/scripts/csscapture.py`

 * *Files identical despite different names*

### Comparing `cssutils-2.7.0/cssutils/scripts/csscombine.py` & `cssutils-2.7.1/cssutils/scripts/csscombine.py`

 * *Files identical despite different names*

### Comparing `cssutils-2.7.0/cssutils/scripts/cssparse.py` & `cssutils-2.7.1/cssutils/scripts/cssparse.py`

 * *Files identical despite different names*

### Comparing `cssutils-2.7.0/cssutils/serialize.py` & `cssutils-2.7.1/cssutils/serialize.py`

 * *Files identical despite different names*

### Comparing `cssutils-2.7.0/cssutils/settings.py` & `cssutils-2.7.1/cssutils/settings.py`

 * *Files identical despite different names*

### Comparing `cssutils-2.7.0/cssutils/stylesheets/medialist.py` & `cssutils-2.7.1/cssutils/stylesheets/medialist.py`

 * *Files identical despite different names*

### Comparing `cssutils-2.7.0/cssutils/stylesheets/mediaquery.py` & `cssutils-2.7.1/cssutils/stylesheets/mediaquery.py`

 * *Files identical despite different names*

### Comparing `cssutils-2.7.0/cssutils/stylesheets/stylesheet.py` & `cssutils-2.7.1/cssutils/stylesheets/stylesheet.py`

 * *Files identical despite different names*

### Comparing `cssutils-2.7.0/cssutils/stylesheets/stylesheetlist.py` & `cssutils-2.7.1/cssutils/stylesheets/stylesheetlist.py`

 * *Files identical despite different names*

### Comparing `cssutils-2.7.0/cssutils/tests/basetest.py` & `cssutils-2.7.1/cssutils/tests/basetest.py`

 * *Files identical despite different names*

### Comparing `cssutils-2.7.0/cssutils/tests/sheets/096.css` & `cssutils-2.7.1/cssutils/tests/sheets/096.css`

 * *Files identical despite different names*

### Comparing `cssutils-2.7.0/cssutils/tests/sheets/097.css` & `cssutils-2.7.1/cssutils/tests/sheets/097.css`

 * *Files identical despite different names*

### Comparing `cssutils-2.7.0/cssutils/tests/sheets/acid2.css` & `cssutils-2.7.1/cssutils/tests/sheets/acid2.css`

 * *Files identical despite different names*

### Comparing `cssutils-2.7.0/cssutils/tests/sheets/bundle.css` & `cssutils-2.7.1/cssutils/tests/sheets/bundle.css`

 * *Files identical despite different names*

### Comparing `cssutils-2.7.0/cssutils/tests/sheets/cthedot_default.css` & `cssutils-2.7.1/cssutils/tests/sheets/cthedot_default.css`

 * *Files identical despite different names*

### Comparing `cssutils-2.7.0/cssutils/tests/sheets/default_html4.css` & `cssutils-2.7.1/cssutils/tests/sheets/default_html4.css`

 * *Files identical despite different names*

### Comparing `cssutils-2.7.0/cssutils/tests/sheets/hacks.css` & `cssutils-2.7.1/cssutils/tests/sheets/hacks.css`

 * *Files identical despite different names*

### Comparing `cssutils-2.7.0/cssutils/tests/sheets/html20.css` & `cssutils-2.7.1/cssutils/tests/sheets/html20.css`

 * *Files identical despite different names*

### Comparing `cssutils-2.7.0/cssutils/tests/sheets/html40.css` & `cssutils-2.7.1/cssutils/tests/sheets/html40.css`

 * *Files identical despite different names*

### Comparing `cssutils-2.7.0/cssutils/tests/sheets/ll.css` & `cssutils-2.7.1/cssutils/tests/sheets/ll.css`

 * *Files identical despite different names*

### Comparing `cssutils-2.7.0/cssutils/tests/sheets/ll2.css` & `cssutils-2.7.1/cssutils/tests/sheets/ll2.css`

 * *Files identical despite different names*

### Comparing `cssutils-2.7.0/cssutils/tests/sheets/sample_5.css` & `cssutils-2.7.1/cssutils/tests/sheets/sample_5.css`

 * *Files identical despite different names*

### Comparing `cssutils-2.7.0/cssutils/tests/sheets/sample_7.css` & `cssutils-2.7.1/cssutils/tests/sheets/sample_7.css`

 * *Files identical despite different names*

### Comparing `cssutils-2.7.0/cssutils/tests/sheets/slashcode.css` & `cssutils-2.7.1/cssutils/tests/sheets/slashcode.css`

 * *Files identical despite different names*

### Comparing `cssutils-2.7.0/cssutils/tests/sheets/t-HACKS.css` & `cssutils-2.7.1/cssutils/tests/sheets/t-HACKS.css`

 * *Files identical despite different names*

### Comparing `cssutils-2.7.0/cssutils/tests/sheets/test-unicode.css` & `cssutils-2.7.1/cssutils/tests/sheets/test-unicode.css`

 * *Files identical despite different names*

### Comparing `cssutils-2.7.0/cssutils/tests/sheets/test.css` & `cssutils-2.7.1/cssutils/tests/sheets/test.css`

 * *Files identical despite different names*

### Comparing `cssutils-2.7.0/cssutils/tests/sheets/tigris.css` & `cssutils-2.7.1/cssutils/tests/sheets/tigris.css`

 * *Files identical despite different names*

### Comparing `cssutils-2.7.0/cssutils/tests/sheets/tigris2.css` & `cssutils-2.7.1/cssutils/tests/sheets/tigris2.css`

 * *Files identical despite different names*

### Comparing `cssutils-2.7.0/cssutils/tests/sheets/xhtml2.css` & `cssutils-2.7.1/cssutils/tests/sheets/xhtml2.css`

 * *Files identical despite different names*

### Comparing `cssutils-2.7.0/cssutils/tests/sheets/xhtml22.css` & `cssutils-2.7.1/cssutils/tests/sheets/xhtml22.css`

 * *Files identical despite different names*

### Comparing `cssutils-2.7.0/cssutils/tests/test_codec.py` & `cssutils-2.7.1/cssutils/tests/test_codec.py`

 * *Files identical despite different names*

### Comparing `cssutils-2.7.0/cssutils/tests/test_csscharsetrule.py` & `cssutils-2.7.1/cssutils/tests/test_csscharsetrule.py`

 * *Files identical despite different names*

### Comparing `cssutils-2.7.0/cssutils/tests/test_csscomment.py` & `cssutils-2.7.1/cssutils/tests/test_csscomment.py`

 * *Files identical despite different names*

### Comparing `cssutils-2.7.0/cssutils/tests/test_cssfontfacerule.py` & `cssutils-2.7.1/cssutils/tests/test_cssfontfacerule.py`

 * *Files identical despite different names*

### Comparing `cssutils-2.7.0/cssutils/tests/test_cssimportrule.py` & `cssutils-2.7.1/cssutils/tests/test_cssimportrule.py`

 * *Files identical despite different names*

### Comparing `cssutils-2.7.0/cssutils/tests/test_cssmediarule.py` & `cssutils-2.7.1/cssutils/tests/test_cssmediarule.py`

 * *Files 2% similar despite different names*

```diff
@@ -134,15 +134,15 @@
             ' /*1*/ only /*2*/ tv /*3*/ and /*4*/ (/*5*/ width) /*5*/ /*6*/, (color) and (height) ': None,
             '(color)and(width),(height)': ' (color) and (width), (height) ',
         }
         tests = {}
         for b, a in list(mls.items()):
             if a is None:
                 a = b
-            tests['@media{}{}'.format(b, style)] = '@media{}{}'.format(a, style)
+            tests[f'@media{b}{style}'] = f'@media{a}{style}'
 
         self.do_equal_p(tests)
         self.do_equal_r(tests)
 
         tests = {
             '@media only tv{}': '',
             '@media not tv{}': '',
```

### Comparing `cssutils-2.7.0/cssutils/tests/test_cssnamespacerule.py` & `cssutils-2.7.1/cssutils/tests/test_cssnamespacerule.py`

 * *Files identical despite different names*

### Comparing `cssutils-2.7.0/cssutils/tests/test_csspagerule.py` & `cssutils-2.7.1/cssutils/tests/test_csspagerule.py`

 * *Files identical despite different names*

### Comparing `cssutils-2.7.0/cssutils/tests/test_cssproperties.py` & `cssutils-2.7.1/cssutils/tests/test_cssproperties.py`

 * *Files identical despite different names*

### Comparing `cssutils-2.7.0/cssutils/tests/test_cssrule.py` & `cssutils-2.7.1/cssutils/tests/test_cssrule.py`

 * *Files identical despite different names*

### Comparing `cssutils-2.7.0/cssutils/tests/test_cssrulelist.py` & `cssutils-2.7.1/cssutils/tests/test_cssrulelist.py`

 * *Files identical despite different names*

### Comparing `cssutils-2.7.0/cssutils/tests/test_cssstyledeclaration.py` & `cssutils-2.7.1/cssutils/tests/test_cssstyledeclaration.py`

 * *Files identical despite different names*

### Comparing `cssutils-2.7.0/cssutils/tests/test_cssstylerule.py` & `cssutils-2.7.1/cssutils/tests/test_cssstylerule.py`

 * *Files identical despite different names*

### Comparing `cssutils-2.7.0/cssutils/tests/test_cssstylesheet.py` & `cssutils-2.7.1/cssutils/tests/test_cssstylesheet.py`

 * *Files identical despite different names*

### Comparing `cssutils-2.7.0/cssutils/tests/test_cssunknownrule.py` & `cssutils-2.7.1/cssutils/tests/test_cssunknownrule.py`

 * *Files identical despite different names*

### Comparing `cssutils-2.7.0/cssutils/tests/test_cssutils.py` & `cssutils-2.7.1/cssutils/tests/test_cssutils.py`

 * *Files identical despite different names*

### Comparing `cssutils-2.7.0/cssutils/tests/test_cssvalue.py` & `cssutils-2.7.1/cssutils/tests/test_cssvalue.py`

 * *Files identical despite different names*

### Comparing `cssutils-2.7.0/cssutils/tests/test_cssvariablesdeclaration.py` & `cssutils-2.7.1/cssutils/tests/test_cssvariablesdeclaration.py`

 * *Files identical despite different names*

### Comparing `cssutils-2.7.0/cssutils/tests/test_cssvariablesrule.py` & `cssutils-2.7.1/cssutils/tests/test_cssvariablesrule.py`

 * *Files identical despite different names*

### Comparing `cssutils-2.7.0/cssutils/tests/test_domimplementation.py` & `cssutils-2.7.1/cssutils/tests/test_domimplementation.py`

 * *Files identical despite different names*

### Comparing `cssutils-2.7.0/cssutils/tests/test_encutils/__init__.py` & `cssutils-2.7.1/cssutils/tests/test_encutils/__init__.py`

 * *Files identical despite different names*

### Comparing `cssutils-2.7.0/cssutils/tests/test_errorhandler.py` & `cssutils-2.7.1/cssutils/tests/test_errorhandler.py`

 * *Files identical despite different names*

### Comparing `cssutils-2.7.0/cssutils/tests/test_helper.py` & `cssutils-2.7.1/cssutils/tests/test_helper.py`

 * *Files identical despite different names*

### Comparing `cssutils-2.7.0/cssutils/tests/test_marginrule.py` & `cssutils-2.7.1/cssutils/tests/test_marginrule.py`

 * *Files identical despite different names*

### Comparing `cssutils-2.7.0/cssutils/tests/test_medialist.py` & `cssutils-2.7.1/cssutils/tests/test_medialist.py`

 * *Files identical despite different names*

### Comparing `cssutils-2.7.0/cssutils/tests/test_mediaquery.py` & `cssutils-2.7.1/cssutils/tests/test_mediaquery.py`

 * *Files identical despite different names*

### Comparing `cssutils-2.7.0/cssutils/tests/test_parse.py` & `cssutils-2.7.1/cssutils/tests/test_parse.py`

 * *Files identical despite different names*

### Comparing `cssutils-2.7.0/cssutils/tests/test_prodparser.py` & `cssutils-2.7.1/cssutils/tests/test_prodparser.py`

 * *Files identical despite different names*

### Comparing `cssutils-2.7.0/cssutils/tests/test_profiles.py` & `cssutils-2.7.1/cssutils/tests/test_profiles.py`

 * *Files identical despite different names*

### Comparing `cssutils-2.7.0/cssutils/tests/test_properties.py` & `cssutils-2.7.1/cssutils/tests/test_properties.py`

 * *Files identical despite different names*

### Comparing `cssutils-2.7.0/cssutils/tests/test_property.py` & `cssutils-2.7.1/cssutils/tests/test_property.py`

 * *Files identical despite different names*

### Comparing `cssutils-2.7.0/cssutils/tests/test_scripts_csscombine.py` & `cssutils-2.7.1/cssutils/tests/test_scripts_csscombine.py`

 * *Files identical despite different names*

### Comparing `cssutils-2.7.0/cssutils/tests/test_selector.py` & `cssutils-2.7.1/cssutils/tests/test_selector.py`

 * *Files identical despite different names*

### Comparing `cssutils-2.7.0/cssutils/tests/test_selectorlist.py` & `cssutils-2.7.1/cssutils/tests/test_selectorlist.py`

 * *Files identical despite different names*

### Comparing `cssutils-2.7.0/cssutils/tests/test_serialize.py` & `cssutils-2.7.1/cssutils/tests/test_serialize.py`

 * *Files identical despite different names*

### Comparing `cssutils-2.7.0/cssutils/tests/test_settings.py` & `cssutils-2.7.1/cssutils/tests/test_settings.py`

 * *Files identical despite different names*

### Comparing `cssutils-2.7.0/cssutils/tests/test_stylesheet.py` & `cssutils-2.7.1/cssutils/tests/test_stylesheet.py`

 * *Files identical despite different names*

### Comparing `cssutils-2.7.0/cssutils/tests/test_tokenize2.py` & `cssutils-2.7.1/cssutils/tests/test_tokenize2.py`

 * *Files identical despite different names*

### Comparing `cssutils-2.7.0/cssutils/tests/test_util.py` & `cssutils-2.7.1/cssutils/tests/test_util.py`

 * *Files identical despite different names*

### Comparing `cssutils-2.7.0/cssutils/tests/test_value.py` & `cssutils-2.7.1/cssutils/tests/test_value.py`

 * *Files identical despite different names*

### Comparing `cssutils-2.7.0/cssutils/tests/test_x.py` & `cssutils-2.7.1/cssutils/tests/test_x.py`

 * *Files identical despite different names*

### Comparing `cssutils-2.7.0/cssutils/tokenize2.py` & `cssutils-2.7.1/cssutils/tokenize2.py`

 * *Files identical despite different names*

### Comparing `cssutils-2.7.0/cssutils/util.py` & `cssutils-2.7.1/cssutils/util.py`

 * *Files 1% similar despite different names*

```diff
@@ -69,17 +69,18 @@
     def _clearSeq(self):
         self._seq.clear()
 
     def _tempSeq(self, readonly=False):
         "Get a writeable Seq() which is used to set ``seq`` later"
         return Seq(readonly=readonly)
 
-    seq = property(
-        lambda self: self._seq, doc="Internal readonly attribute, **DO NOT USE**!"
-    )
+    @property
+    def seq(self):
+        """Internal readonly attribute, **DO NOT USE**!"""
+        return self._seq
 
 
 class _NewListBase(_NewBase):
     """
     (EXPERIMENTAL)
     A base class used for list classes like stylesheets.MediaList
 
@@ -888,18 +889,18 @@
         """init"""
         super().__init__(parentStyleSheet=None, log=log)
         self.__namespaces = dict(*args)
 
     def __setitem__(self, prefix, namespaceURI):
         self.__namespaces[prefix] = namespaceURI
 
-    namespaces = property(
-        lambda self: self.__namespaces,
-        doc='Dict Wrapper for self.sheets @namespace rules.',
-    )
+    @property
+    def namespaces(self):
+        """Dict Wrapper for self.sheets @namespace rules."""
+        return self.__namespaces
 
     def __str__(self):
         return "<cssutils.util.{} object namespaces={!r} at 0x{:x}>".format(
             self.__class__.__name__,
             self.namespaces,
             id(self),
         )
```

### Comparing `cssutils-2.7.0/cssutils.egg-info/PKG-INFO` & `cssutils-2.7.1/cssutils.egg-info/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cssutils
-Version: 2.7.0
+Version: 2.7.1
 Summary: A CSS Cascading Style Sheets library for Python
 Home-page: https://github.com/jaraco/cssutils
 Author: Christof Hoeke
 Author-email: c@cthedot.de
 Maintainer: Jason R. Coombs
 Maintainer-email: jaraco@jaraco.com
 Keywords: CSS,Cascading Style Sheets,CSSParser,DOM Level 2 Stylesheets,DOM Level 2 CSS
@@ -81,18 +81,14 @@
 `CSSOM <http://dev.w3.org/csswg/cssom/>`__
     A few details (mainly the NamespaceRule DOM) are taken from here. Plan is to move implementation to the stuff defined here which is newer but still no REC so might change anytime...
 
 The cssutils tokenizer is a customized implementation of `CSS3 Module: Syntax (W3C Working Draft 13 August 2003) <http://www.w3.org/TR/css3-syntax/>`_ which itself is based on the CSS 2.1 tokenizer. It tries to be as compliant as possible but uses some (helpful) parts of the CSS 2.1 tokenizer.
 
 I guess cssutils is neither CSS 2.1 nor CSS 3 compliant but tries to at least be able to parse both grammars including some more real world cases (some CSS hacks are actually parsed and serialized). Both official grammars are not final nor bugfree but still feasible. cssutils aim is not to be fully compliant to any CSS specification (the specifications seem to be in a constant flow anyway) but cssutils *should* be able to read and write as many as possible CSS stylesheets "in the wild" while at the same time implement the official APIs which are well documented. Some minor extensions are provided as well.
 
-Please visit http://cthedot.de/cssutils/ or https://bitbucket.org/cthedot/cssutils/ for more details.
-
-There is also a low-traffic `cssutils discussion group <http://groups.google.com/group/cssutils>`_.
-
 
 Compatibility
 =============
 
 cssutils is developed on modern Python versions. Check the package metadata
 for compatibilty.
```

### Comparing `cssutils-2.7.0/cssutils.egg-info/SOURCES.txt` & `cssutils-2.7.1/cssutils.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `cssutils-2.7.0/docs/backlog.rst` & `cssutils-2.7.1/docs/backlog.rst`

 * *Files identical despite different names*

### Comparing `cssutils-2.7.0/docs/conf.py` & `cssutils-2.7.1/docs/conf.py`

 * *Files identical despite different names*

### Comparing `cssutils-2.7.0/docs/css.rst` & `cssutils-2.7.1/docs/css.rst`

 * *Files identical despite different names*

### Comparing `cssutils-2.7.0/docs/html/CHANGELOG.html` & `cssutils-2.7.1/docs/html/CHANGELOG.html`

 * *Files identical despite different names*

### Comparing `cssutils-2.7.0/docs/html/README.html` & `cssutils-2.7.1/docs/html/README.html`

 * *Files identical despite different names*

### Comparing `cssutils-2.7.0/docs/html/_2to3 py3.html` & `cssutils-2.7.1/docs/html/_2to3 py3.html`

 * *Files identical despite different names*

### Comparing `cssutils-2.7.0/docs/html/_sources/CHANGELOG.txt` & `cssutils-2.7.1/docs/html/_sources/CHANGELOG.txt`

 * *Files identical despite different names*

### Comparing `cssutils-2.7.0/docs/html/_sources/README.txt` & `cssutils-2.7.1/docs/html/_sources/README.txt`

 * *Files identical despite different names*

### Comparing `cssutils-2.7.0/docs/html/_sources/docs/backlog.txt` & `cssutils-2.7.1/docs/html/_sources/docs/backlog.txt`

 * *Files identical despite different names*

### Comparing `cssutils-2.7.0/docs/html/_sources/docs/css.txt` & `cssutils-2.7.1/docs/html/_sources/docs/css.txt`

 * *Files identical despite different names*

### Comparing `cssutils-2.7.0/docs/html/_sources/docs/cssstyledeclaration.txt` & `cssutils-2.7.1/docs/html/_sources/docs/cssstyledeclaration.txt`

 * *Files identical despite different names*

### Comparing `cssutils-2.7.0/docs/html/_sources/docs/implementation.txt` & `cssutils-2.7.1/docs/html/_sources/docs/implementation.txt`

 * *Files identical despite different names*

### Comparing `cssutils-2.7.0/docs/html/_sources/docs/logging.txt` & `cssutils-2.7.1/docs/html/_sources/docs/logging.txt`

 * *Files identical despite different names*

### Comparing `cssutils-2.7.0/docs/html/_sources/docs/migrate.txt` & `cssutils-2.7.1/docs/html/_sources/docs/migrate.txt`

 * *Files identical despite different names*

### Comparing `cssutils-2.7.0/docs/html/_sources/docs/parse.txt` & `cssutils-2.7.1/docs/html/_sources/docs/parse.txt`

 * *Files identical despite different names*

### Comparing `cssutils-2.7.0/docs/html/_sources/docs/profiles.txt` & `cssutils-2.7.1/docs/html/_sources/docs/profiles.txt`

 * *Files identical despite different names*

### Comparing `cssutils-2.7.0/docs/html/_sources/docs/scripts.txt` & `cssutils-2.7.1/docs/html/_sources/docs/scripts.txt`

 * *Files identical despite different names*

### Comparing `cssutils-2.7.0/docs/html/_sources/docs/serialize.txt` & `cssutils-2.7.1/docs/html/_sources/docs/serialize.txt`

 * *Files identical despite different names*

### Comparing `cssutils-2.7.0/docs/html/_sources/docs/settings.txt` & `cssutils-2.7.1/docs/html/_sources/docs/settings.txt`

 * *Files identical despite different names*

### Comparing `cssutils-2.7.0/docs/html/_sources/docs/stylesheets.txt` & `cssutils-2.7.1/docs/html/_sources/docs/stylesheets.txt`

 * *Files identical despite different names*

### Comparing `cssutils-2.7.0/docs/html/_sources/index.txt` & `cssutils-2.7.1/docs/html/_sources/index.txt`

 * *Files identical despite different names*

### Comparing `cssutils-2.7.0/docs/html/_static/basic.css` & `cssutils-2.7.1/docs/html/_static/basic.css`

 * *Files identical despite different names*

### Comparing `cssutils-2.7.0/docs/html/_static/default.css` & `cssutils-2.7.1/docs/html/_static/default.css`

 * *Files identical despite different names*

### Comparing `cssutils-2.7.0/docs/html/_static/doctools.js` & `cssutils-2.7.1/docs/html/_static/doctools.js`

 * *Files identical despite different names*

### Comparing `cssutils-2.7.0/docs/html/_static/jquery.js` & `cssutils-2.7.1/docs/html/_static/jquery.js`

 * *Files identical despite different names*

### Comparing `cssutils-2.7.0/docs/html/_static/pygments.css` & `cssutils-2.7.1/docs/html/_static/pygments.css`

 * *Files identical despite different names*

### Comparing `cssutils-2.7.0/docs/html/_static/searchtools.js` & `cssutils-2.7.1/docs/html/_static/searchtools.js`

 * *Files identical despite different names*

### Comparing `cssutils-2.7.0/docs/html/_static/sidebar.js` & `cssutils-2.7.1/docs/html/_static/sidebar.js`

 * *Files identical despite different names*

### Comparing `cssutils-2.7.0/docs/html/_static/underscore.js` & `cssutils-2.7.1/docs/html/_static/underscore.js`

 * *Files identical despite different names*

### Comparing `cssutils-2.7.0/docs/html/docs/backlog.html` & `cssutils-2.7.1/docs/html/docs/backlog.html`

 * *Files identical despite different names*

### Comparing `cssutils-2.7.0/docs/html/docs/codec.html` & `cssutils-2.7.1/docs/html/docs/codec.html`

 * *Files identical despite different names*

### Comparing `cssutils-2.7.0/docs/html/docs/css.html` & `cssutils-2.7.1/docs/html/docs/css.html`

 * *Files identical despite different names*

### Comparing `cssutils-2.7.0/docs/html/docs/encutils.html` & `cssutils-2.7.1/docs/html/docs/encutils.html`

 * *Files identical despite different names*

### Comparing `cssutils-2.7.0/docs/html/docs/logging.html` & `cssutils-2.7.1/docs/html/docs/logging.html`

 * *Files identical despite different names*

### Comparing `cssutils-2.7.0/docs/html/docs/migrate.html` & `cssutils-2.7.1/docs/html/docs/migrate.html`

 * *Files identical despite different names*

### Comparing `cssutils-2.7.0/docs/html/docs/parse.html` & `cssutils-2.7.1/docs/html/docs/parse.html`

 * *Files identical despite different names*

### Comparing `cssutils-2.7.0/docs/html/docs/profiles.html` & `cssutils-2.7.1/docs/html/docs/profiles.html`

 * *Files identical despite different names*

### Comparing `cssutils-2.7.0/docs/html/docs/scripts.html` & `cssutils-2.7.1/docs/html/docs/scripts.html`

 * *Files identical despite different names*

### Comparing `cssutils-2.7.0/docs/html/docs/serialize.html` & `cssutils-2.7.1/docs/html/docs/serialize.html`

 * *Files identical despite different names*

### Comparing `cssutils-2.7.0/docs/html/docs/settings.html` & `cssutils-2.7.1/docs/html/docs/settings.html`

 * *Files identical despite different names*

### Comparing `cssutils-2.7.0/docs/html/docs/stylesheets.html` & `cssutils-2.7.1/docs/html/docs/stylesheets.html`

 * *Files identical despite different names*

### Comparing `cssutils-2.7.0/docs/html/docs/utilities.html` & `cssutils-2.7.1/docs/html/docs/utilities.html`

 * *Files identical despite different names*

### Comparing `cssutils-2.7.0/docs/html/docs/variables.html` & `cssutils-2.7.1/docs/html/docs/variables.html`

 * *Files identical despite different names*

### Comparing `cssutils-2.7.0/docs/html/genindex.html` & `cssutils-2.7.1/docs/html/genindex.html`

 * *Files identical despite different names*

### Comparing `cssutils-2.7.0/docs/html/index.html` & `cssutils-2.7.1/docs/html/index.html`

 * *Files identical despite different names*

### Comparing `cssutils-2.7.0/docs/html/py-modindex.html` & `cssutils-2.7.1/docs/html/py-modindex.html`

 * *Files identical despite different names*

### Comparing `cssutils-2.7.0/docs/html/search.html` & `cssutils-2.7.1/docs/html/search.html`

 * *Files identical despite different names*

### Comparing `cssutils-2.7.0/docs/html/searchindex.js` & `cssutils-2.7.1/docs/html/searchindex.js`

 * *Files identical despite different names*

### Comparing `cssutils-2.7.0/docs/index.rst` & `cssutils-2.7.1/docs/index.rst`

 * *Files identical despite different names*

### Comparing `cssutils-2.7.0/docs/known issues.rst` & `cssutils-2.7.1/docs/known issues.rst`

 * *Files identical despite different names*

### Comparing `cssutils-2.7.0/docs/logging.rst` & `cssutils-2.7.1/docs/logging.rst`

 * *Ordering differences only*

 * *Files 0% similar despite different names*

```diff
@@ -18,8 +18,8 @@
 
 * ``log.addHandler(h)`` and ``log.removeHandler(h)``
 * ``log.*(msg)`` where ``*`` is one of ``debug``, ``info``, ``warn``, ``error`` or ``fatal``/``critical``
 
 Additional method: ``cssutils.log.setLog(newlog)``: To replace the default log which sends output to ``stderr``.
 
 
-See also :meth:`cssutils.css.Property.validate` for details on how properties log.
+See also :meth:`cssutils.css.Property.validate` for details on how properties log.
```

### Comparing `cssutils-2.7.0/docs/migrate.rst` & `cssutils-2.7.1/docs/migrate.rst`

 * *Files identical despite different names*

### Comparing `cssutils-2.7.0/docs/parse.rst` & `cssutils-2.7.1/docs/parse.rst`

 * *Files 2% similar despite different names*

```diff
@@ -34,15 +34,15 @@
 ``CSSParser``
 =============
 The parser is reusable.
 
 .. autoclass:: cssutils.CSSParser
    :members:
    :inherited-members:
-   
+
 
 The URL Fetcher
 ---------------
 If you want to control how imported stylesheets are read you may define a custom URL fetcher (e.g. would be needed on Google AppEngine as urllib2, which is normally used, is not available. A GAE specific fetcher is included in cssutils from 0.9.5a1 though.)
 
 A custom URL fetcher may be used during parsing via ``CSSParser.setFetcher(fetcher)`` (or as an init parameter). The so customized parser is reusable. The fetcher is called when an ``@import`` rule is found and the referenced stylesheet is about to be retrieved.
```

### Comparing `cssutils-2.7.0/docs/profiles.rst` & `cssutils-2.7.1/docs/profiles.rst`

 * *Files identical despite different names*

### Comparing `cssutils-2.7.0/docs/scripts.rst` & `cssutils-2.7.1/docs/scripts.rst`

 * *Files 8% similar despite different names*

```diff
@@ -110,54 +110,54 @@
 
 ``csscombine`` may also be used to change the encoding of the stylesheet if a target encoding is given.
 
 programmatic use
 ----------------
 example::
 
-	>>> from cssutils.script import csscombine
-	>>> proxypath = 'sheets/import.css'
-	>>> print csscombine(path=proxypath, sourceencoding=None, targetencoding='utf-8', minify=False)
-	INFO    Combining files from None
-	INFO    Processing @import u'import/import2.css'
-	INFO    Processing @import u'../import3.css'
-	INFO    @import: Adjusting paths for u'../import3.css'
-	INFO    Processing @import u'import-impossible.css'
-	INFO    @import: Adjusting paths for u'import-impossible.css'
-	WARNING Cannot combine imported sheet with given media as other rules then comments or stylerules found cssutils.css.CSSNamespaceRule(namespaceURI=u'y', prefix=u''), keeping u'@import "import-impossible.css" print;'
-	INFO    @import: Adjusting paths for u'import/import2.css'
-	INFO    Using target encoding: 'utf-8'
-	@charset "utf-8";
-	/* START @import "import/import2.css" */
-	@import "import-impossible.css" print;
-	/* START @import "../import3.css" */
-	/* import3 */
-	.import3 {
-	    /* from ./import/../import3.css */
-	    background: url(images/example3.gif);
-	    background: url(images/example3.gif);
-	    background: url(import/images2/example2.gif);
-	    background: url(import/images2/example2.gif);
-	    background: url(images/example3.gif)
-	    }
-	/* START @import "import-impossible.css" */
-	.import2 {
-	    /* sheets/import2.css */
-	    background: url(http://example.com/images/example.gif);
-	    background: url(//example.com/images/example.gif);
-	    background: url(/images/example.gif);
-	    background: url(import/images2/example.gif);
-	    background: url(import/images2/example.gif);
-	    background: url(images/example.gif);
-	    background: url(images/example.gif)
-	    }
-	.import {
-	    /* ./import.css */
-	    background-image: url(images/example.gif)
-	    }
+    >>> from cssutils.script import csscombine
+    >>> proxypath = 'sheets/import.css'
+    >>> print csscombine(path=proxypath, sourceencoding=None, targetencoding='utf-8', minify=False)
+    INFO    Combining files from None
+    INFO    Processing @import u'import/import2.css'
+    INFO    Processing @import u'../import3.css'
+    INFO    @import: Adjusting paths for u'../import3.css'
+    INFO    Processing @import u'import-impossible.css'
+    INFO    @import: Adjusting paths for u'import-impossible.css'
+    WARNING Cannot combine imported sheet with given media as other rules then comments or stylerules found cssutils.css.CSSNamespaceRule(namespaceURI=u'y', prefix=u''), keeping u'@import "import-impossible.css" print;'
+    INFO    @import: Adjusting paths for u'import/import2.css'
+    INFO    Using target encoding: 'utf-8'
+    @charset "utf-8";
+    /* START @import "import/import2.css" */
+    @import "import-impossible.css" print;
+    /* START @import "../import3.css" */
+    /* import3 */
+    .import3 {
+        /* from ./import/../import3.css */
+        background: url(images/example3.gif);
+        background: url(images/example3.gif);
+        background: url(import/images2/example2.gif);
+        background: url(import/images2/example2.gif);
+        background: url(images/example3.gif)
+        }
+    /* START @import "import-impossible.css" */
+    .import2 {
+        /* sheets/import2.css */
+        background: url(http://example.com/images/example.gif);
+        background: url(//example.com/images/example.gif);
+        background: url(/images/example.gif);
+        background: url(import/images2/example.gif);
+        background: url(import/images2/example.gif);
+        background: url(images/example.gif);
+        background: url(images/example.gif)
+        }
+    .import {
+        /* ./import.css */
+        background-image: url(images/example.gif)
+        }
 
 
 script use
 ----------
 Usage: csscombine-script.py [options] [path]
 
 Options:
@@ -166,8 +166,8 @@
   -s SOURCEENCODING, --sourceencoding=SOURCEENCODING
                         encoding of input, defaulting to "css". If given
                         overwrites other encoding information like @charset
                         declarations
   -t TARGETENCODING, --targetencoding=TARGETENCODING
                         encoding of output, defaulting to "UTF-8"
   -m, --minify          saves minified version of combined files, defaults to
-                        False
+                        False
```

### Comparing `cssutils-2.7.0/docs/serialize.rst` & `cssutils-2.7.1/docs/serialize.rst`

 * *Files 10% similar despite different names*

```diff
@@ -5,27 +5,27 @@
     object: cssutils.ser
 
 ===============
 serializing CSS
 ===============
 To serialize any stylesheet use::
 
-	print sheet.cssText
-	
+    print sheet.cssText
+
 Also most other objects have a similar property which contains the *text* content of each object. Some use a slightly different name (e.g. ``selectorText``) but all use the global serializer::
 
-	>>> sheet = cssutils.parseString('a, b { color: green }')
-	>>> print sheet.cssRules[0].cssText
-	a, b {
-	    color: green
-	    }
-	>>> print sheet.cssRules[0].selectorText
-	a, b
-	>>> print sheet.cssRules[0].selectorList[1].selectorText
-	b
+    >>> sheet = cssutils.parseString('a, b { color: green }')
+    >>> print sheet.cssRules[0].cssText
+    a, b {
+        color: green
+        }
+    >>> print sheet.cssRules[0].selectorText
+    a, b
+    >>> print sheet.cssRules[0].selectorList[1].selectorText
+    b
 
 
 .. _Preferences:
 
 .. index::
     single: cssutils.ser.prefs
     object: cssutils.ser.prefs
```

### Comparing `cssutils-2.7.0/docs/settings.rst` & `cssutils-2.7.1/docs/settings.rst`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 ====================
 extra settings
 ====================
 A single and **experimental** setting currently only:
 
 It is possible to at least parse sheets with Microsoft only property values for
  ``filter`` which start with ``progid:DXImageTransform.Microsoft.[...](``.
- 
+
 To enable these you need to set::
 
     >>> from cssutils import settings
     >>> settings.set('DXImageTransform.Microsoft', True)
     >>> cssutils.ser.prefs.useMinified()
     >>> text = 'a {filter: progid:DXImageTransform.Microsoft.BasicImage( rotation = 90 )}'
     >>> print cssutils.parseString(text).cssText
```

### Comparing `cssutils-2.7.0/docs/stylesheets.rst` & `cssutils-2.7.1/docs/stylesheets.rst`

 * *Files identical despite different names*

### Comparing `cssutils-2.7.0/encutils/__init__.py` & `cssutils-2.7.1/encutils/__init__.py`

 * *Files identical despite different names*

### Comparing `cssutils-2.7.0/examples/build.py` & `cssutils-2.7.1/examples/build.py`

 * *Files identical despite different names*

### Comparing `cssutils-2.7.0/examples/cssencodings.py` & `cssutils-2.7.1/examples/cssencodings.py`

 * *Files identical despite different names*

### Comparing `cssutils-2.7.0/examples/customlog.py` & `cssutils-2.7.1/examples/customlog.py`

 * *Files identical despite different names*

### Comparing `cssutils-2.7.0/examples/imports.py` & `cssutils-2.7.1/examples/imports.py`

 * *Files identical despite different names*

### Comparing `cssutils-2.7.0/examples/minify.py` & `cssutils-2.7.1/examples/minify.py`

 * *Files identical despite different names*

### Comparing `cssutils-2.7.0/examples/parse.py` & `cssutils-2.7.1/examples/parse.py`

 * *Files identical despite different names*

### Comparing `cssutils-2.7.0/examples/properties_with_same_name.py` & `cssutils-2.7.1/examples/properties_with_same_name.py`

 * *Files identical despite different names*

### Comparing `cssutils-2.7.0/examples/selectors_tolower.py` & `cssutils-2.7.1/examples/selectors_tolower.py`

 * *Files identical despite different names*

### Comparing `cssutils-2.7.0/examples/serialize.py` & `cssutils-2.7.1/examples/serialize.py`

 * *Files identical despite different names*

### Comparing `cssutils-2.7.0/examples/style.py` & `cssutils-2.7.1/examples/style.py`

 * *Files identical despite different names*

### Comparing `cssutils-2.7.0/examples/styledeclaration.py` & `cssutils-2.7.1/examples/styledeclaration.py`

 * *Files identical despite different names*

### Comparing `cssutils-2.7.0/examples/testutil.py` & `cssutils-2.7.1/examples/testutil.py`

 * *Files 8% similar despite different names*

```diff
@@ -50,17 +50,17 @@
         out = self._out.getvalue()
         err = self._err.getvalue()
 
         ok = out == expo and err == expe
         if not ok:
             print()
             if out != expo:
-                print('### out:\n{!r}\n### != expout:\n{!r}\n'.format(out, expo))
+                print(f'### out:\n{out!r}\n### != expout:\n{expo!r}\n')
             else:
-                print('### err:\n{!r}\n### != experr:\n{!r}\n'.format(err, expe))
+                print(f'### err:\n{err!r}\n### != experr:\n{expe!r}\n')
         return ok
 
 
 modules = 0
 errors = 0
```

### Comparing `cssutils-2.7.0/examples/website.py` & `cssutils-2.7.1/examples/website.py`

 * *Files identical despite different names*

### Comparing `cssutils-2.7.0/pytest.ini` & `cssutils-2.7.1/pytest.ini`

 * *Files identical despite different names*

### Comparing `cssutils-2.7.0/setup.cfg` & `cssutils-2.7.1/setup.cfg`

 * *Files identical despite different names*

### Comparing `cssutils-2.7.0/sheets/096.css` & `cssutils-2.7.1/sheets/096.css`

 * *Files identical despite different names*

### Comparing `cssutils-2.7.0/sheets/097.css` & `cssutils-2.7.1/sheets/097.css`

 * *Files identical despite different names*

### Comparing `cssutils-2.7.0/sheets/acid2.css` & `cssutils-2.7.1/sheets/acid2.css`

 * *Files identical despite different names*

### Comparing `cssutils-2.7.0/sheets/bundle.css` & `cssutils-2.7.1/sheets/bundle.css`

 * *Files identical despite different names*

### Comparing `cssutils-2.7.0/sheets/cthedot_default.css` & `cssutils-2.7.1/sheets/cthedot_default.css`

 * *Files identical despite different names*

### Comparing `cssutils-2.7.0/sheets/default_html4.css` & `cssutils-2.7.1/sheets/default_html4.css`

 * *Files identical despite different names*

### Comparing `cssutils-2.7.0/sheets/hacks.css` & `cssutils-2.7.1/sheets/hacks.css`

 * *Files identical despite different names*

### Comparing `cssutils-2.7.0/sheets/html20.css` & `cssutils-2.7.1/sheets/html20.css`

 * *Files identical despite different names*

### Comparing `cssutils-2.7.0/sheets/html40.css` & `cssutils-2.7.1/sheets/html40.css`

 * *Files identical despite different names*

### Comparing `cssutils-2.7.0/sheets/ll.css` & `cssutils-2.7.1/sheets/ll.css`

 * *Files identical despite different names*

### Comparing `cssutils-2.7.0/sheets/ll2.css` & `cssutils-2.7.1/sheets/ll2.css`

 * *Files identical despite different names*

### Comparing `cssutils-2.7.0/sheets/sample_5.css` & `cssutils-2.7.1/sheets/sample_5.css`

 * *Files identical despite different names*

### Comparing `cssutils-2.7.0/sheets/sample_7.css` & `cssutils-2.7.1/sheets/sample_7.css`

 * *Files identical despite different names*

### Comparing `cssutils-2.7.0/sheets/slashcode.css` & `cssutils-2.7.1/sheets/slashcode.css`

 * *Files identical despite different names*

### Comparing `cssutils-2.7.0/sheets/t-HACKS.css` & `cssutils-2.7.1/sheets/t-HACKS.css`

 * *Files identical despite different names*

### Comparing `cssutils-2.7.0/sheets/test-unicode.css` & `cssutils-2.7.1/sheets/test-unicode.css`

 * *Files identical despite different names*

### Comparing `cssutils-2.7.0/sheets/test.css` & `cssutils-2.7.1/sheets/test.css`

 * *Files identical despite different names*

### Comparing `cssutils-2.7.0/sheets/tigris.css` & `cssutils-2.7.1/sheets/tigris.css`

 * *Files identical despite different names*

### Comparing `cssutils-2.7.0/sheets/tigris2.css` & `cssutils-2.7.1/sheets/tigris2.css`

 * *Files identical despite different names*

### Comparing `cssutils-2.7.0/sheets/xhtml2.css` & `cssutils-2.7.1/sheets/xhtml2.css`

 * *Files identical despite different names*

### Comparing `cssutils-2.7.0/sheets/xhtml22.css` & `cssutils-2.7.1/sheets/xhtml22.css`

 * *Files identical despite different names*

### Comparing `cssutils-2.7.0/tools/speed.py` & `cssutils-2.7.1/tools/speed.py`

 * *Files identical despite different names*

### Comparing `cssutils-2.7.0/tools/try.py` & `cssutils-2.7.1/tools/try.py`

 * *Files 0% similar despite different names*

```diff
@@ -751,15 +751,15 @@
                 else:
                     newvalue.append(vi.cssText)
 
             p.value = ' '.join(newvalue)
 
         elif v.cssValueType == v.CSS_VARIABLE:
             if v.value:
-                print('+ Replacing {!r} with {!r}'.format(p.value, v.value))
+                print(f'+ Replacing {p.value!r} with {v.value!r}')
                 p.value = v.value
             else:
                 print('- No value found for %r' % p.value)
 
     # remove @variables rules
     for r in s:
         if r.VARIABLES_RULE == r.type:
@@ -1214,17 +1214,15 @@
                 allow_truncated parameter passed to fetch() was False.
         """
         from google.appengine.api import urlfetch
 
         try:
             r = urlfetch.fetch(url, method=urlfetch.GET)
         except urlfetch.Error as e:
-            cssutils.log.warn(
-                'Error opening url={!r}: {}'.format(url, e.message), error=IOError
-            )
+            cssutils.log.warn(f'Error opening url={url!r}: {e.message}', error=IOError)
         else:
             if r.status_code == 200:
                 # find mimetype and encoding
                 mimetype = 'application/octet-stream'
                 try:
                     import cgi
 
@@ -1233,15 +1231,15 @@
                 except KeyError:
                     encoding = None
 
                 return encoding, r.content
             else:
                 # TODO: 301 etc
                 cssutils.log.warn(
-                    'Error opening url={!r}: HTTP status {}'.format(url, r.status_code),
+                    f'Error opening url={url!r}: HTTP status {r.status_code}',
                     error=IOError,
                 )
 
     def fetcher(url):
         return 'text/css', 'ascii', '/*test*/'
 
     p = cssutils.CSSParser()  # fetcher=fetcher)
```

### Comparing `cssutils-2.7.0/tox.ini` & `cssutils-2.7.1/tox.ini`

 * *Files identical despite different names*

