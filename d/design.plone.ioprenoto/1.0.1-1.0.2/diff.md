# Comparing `tmp/design.plone.ioprenoto-1.0.1.tar.gz` & `tmp/design.plone.ioprenoto-1.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "design.plone.ioprenoto-1.0.1.tar", last modified: Thu Apr  6 15:54:42 2023, max compression
+gzip compressed data, was "design.plone.ioprenoto-1.0.2.tar", last modified: Mon Jun 12 12:43:34 2023, max compression
```

## Comparing `design.plone.ioprenoto-1.0.1.tar` & `design.plone.ioprenoto-1.0.2.tar`

### file list

```diff
@@ -1,89 +1,101 @@
-drwxr-xr-x   0 roman      (502) staff       (20)        0 2023-04-06 15:54:42.736051 design.plone.ioprenoto-1.0.1/
--rw-r--r--   0 roman      (502) staff       (20)      180 2023-04-06 15:54:42.000000 design.plone.ioprenoto-1.0.1/CHANGES.rst
--rw-r--r--   0 roman      (502) staff       (20)       58 2023-04-06 15:54:42.000000 design.plone.ioprenoto-1.0.1/CONTRIBUTORS.rst
--rw-r--r--   0 roman      (502) staff       (20)     1338 2023-04-06 15:54:42.000000 design.plone.ioprenoto-1.0.1/DEVELOP.rst
--rw-r--r--   0 roman      (502) staff       (20)    18092 2023-04-06 15:54:42.000000 design.plone.ioprenoto-1.0.1/LICENSE.GPL
--rw-r--r--   0 roman      (502) staff       (20)      662 2023-04-06 15:54:42.000000 design.plone.ioprenoto-1.0.1/LICENSE.rst
--rw-r--r--   0 roman      (502) staff       (20)      116 2023-04-06 15:54:42.000000 design.plone.ioprenoto-1.0.1/MANIFEST.in
--rw-r--r--   0 roman      (502) staff       (20)     5182 2023-04-06 15:54:42.736219 design.plone.ioprenoto-1.0.1/PKG-INFO
--rw-r--r--   0 roman      (502) staff       (20)     2759 2023-04-06 15:54:42.000000 design.plone.ioprenoto-1.0.1/README.rst
-drwxr-xr-x   0 roman      (502) staff       (20)        0 2023-04-06 15:54:42.721346 design.plone.ioprenoto-1.0.1/docs/
--rw-r--r--   0 roman      (502) staff       (20)     7986 2023-04-06 15:54:42.000000 design.plone.ioprenoto-1.0.1/docs/conf.py
--rw-r--r--   0 roman      (502) staff       (20)       89 2023-04-06 15:54:42.000000 design.plone.ioprenoto-1.0.1/docs/index.rst
--rw-r--r--   0 roman      (502) staff       (20)      340 2023-04-06 15:54:42.736756 design.plone.ioprenoto-1.0.1/setup.cfg
--rw-r--r--   0 roman      (502) staff       (20)     2736 2023-04-06 15:54:42.000000 design.plone.ioprenoto-1.0.1/setup.py
-drwxr-xr-x   0 roman      (502) staff       (20)        0 2023-04-06 15:54:42.715663 design.plone.ioprenoto-1.0.1/src/
-drwxr-xr-x   0 roman      (502) staff       (20)        0 2023-04-06 15:54:42.721612 design.plone.ioprenoto-1.0.1/src/design/
--rw-r--r--   0 roman      (502) staff       (20)       80 2023-04-06 15:54:42.000000 design.plone.ioprenoto-1.0.1/src/design/__init__.py
-drwxr-xr-x   0 roman      (502) staff       (20)        0 2023-04-06 15:54:42.724110 design.plone.ioprenoto-1.0.1/src/design/plone/
--rw-r--r--   0 roman      (502) staff       (20)       80 2023-04-06 15:54:42.000000 design.plone.ioprenoto-1.0.1/src/design/plone/__init__.py
-drwxr-xr-x   0 roman      (502) staff       (20)        0 2023-04-06 15:54:42.725775 design.plone.ioprenoto-1.0.1/src/design/plone/ioprenoto/
--rw-r--r--   0 roman      (502) staff       (20)      139 2023-04-06 15:54:42.000000 design.plone.ioprenoto-1.0.1/src/design/plone/ioprenoto/__init__.py
-drwxr-xr-x   0 roman      (502) staff       (20)        0 2023-04-06 15:54:42.727124 design.plone.ioprenoto-1.0.1/src/design/plone/ioprenoto/behaviors/
--rw-r--r--   0 roman      (502) staff       (20)        0 2023-04-06 15:54:42.000000 design.plone.ioprenoto-1.0.1/src/design/plone/ioprenoto/behaviors/__init__.py
--rw-r--r--   0 roman      (502) staff       (20)     1145 2023-04-06 15:54:42.000000 design.plone.ioprenoto-1.0.1/src/design/plone/ioprenoto/behaviors/configure.zcml
--rw-r--r--   0 roman      (502) staff       (20)      471 2023-04-06 15:54:42.000000 design.plone.ioprenoto-1.0.1/src/design/plone/ioprenoto/behaviors/orario_di_apertura.py
--rw-r--r--   0 roman      (502) staff       (20)     1128 2023-04-06 15:54:42.000000 design.plone.ioprenoto-1.0.1/src/design/plone/ioprenoto/behaviors/punto_di_contatto.py
--rw-r--r--   0 roman      (502) staff       (20)     1123 2023-04-06 15:54:42.000000 design.plone.ioprenoto-1.0.1/src/design/plone/ioprenoto/behaviors/uffici_correlati.py
-drwxr-xr-x   0 roman      (502) staff       (20)        0 2023-04-06 15:54:42.727586 design.plone.ioprenoto-1.0.1/src/design/plone/ioprenoto/browser/
--rw-r--r--   0 roman      (502) staff       (20)        0 2023-04-06 15:54:42.000000 design.plone.ioprenoto-1.0.1/src/design/plone/ioprenoto/browser/__init__.py
--rw-r--r--   0 roman      (502) staff       (20)      628 2023-04-06 15:54:42.000000 design.plone.ioprenoto-1.0.1/src/design/plone/ioprenoto/browser/configure.zcml
-drwxr-xr-x   0 roman      (502) staff       (20)        0 2023-04-06 15:54:42.727848 design.plone.ioprenoto-1.0.1/src/design/plone/ioprenoto/browser/overrides/
--rw-r--r--   0 roman      (502) staff       (20)        0 2023-04-06 15:54:42.000000 design.plone.ioprenoto-1.0.1/src/design/plone/ioprenoto/browser/overrides/.gitkeep
-drwxr-xr-x   0 roman      (502) staff       (20)        0 2023-04-06 15:54:42.728043 design.plone.ioprenoto-1.0.1/src/design/plone/ioprenoto/browser/static/
--rw-r--r--   0 roman      (502) staff       (20)        0 2023-04-06 15:54:42.000000 design.plone.ioprenoto-1.0.1/src/design/plone/ioprenoto/browser/static/.gitkeep
--rw-r--r--   0 roman      (502) staff       (20)     1464 2023-04-06 15:54:42.000000 design.plone.ioprenoto-1.0.1/src/design/plone/ioprenoto/configure.zcml
--rw-r--r--   0 roman      (502) staff       (20)      270 2023-04-06 15:54:42.000000 design.plone.ioprenoto-1.0.1/src/design/plone/ioprenoto/interfaces.py
-drwxr-xr-x   0 roman      (502) staff       (20)        0 2023-04-06 15:54:42.729544 design.plone.ioprenoto-1.0.1/src/design/plone/ioprenoto/locales/
--rw-r--r--   0 roman      (502) staff       (20)      611 2023-04-06 15:54:42.000000 design.plone.ioprenoto-1.0.1/src/design/plone/ioprenoto/locales/README.rst
--rw-r--r--   0 roman      (502) staff       (20)        0 2023-04-06 15:54:42.000000 design.plone.ioprenoto-1.0.1/src/design/plone/ioprenoto/locales/__init__.py
--rw-r--r--   0 roman      (502) staff       (20)        0 2023-04-06 15:54:42.000000 design.plone.ioprenoto-1.0.1/src/design/plone/ioprenoto/locales/design.plone.ioprenoto.pot
-drwxr-xr-x   0 roman      (502) staff       (20)        0 2023-04-06 15:54:42.716891 design.plone.ioprenoto-1.0.1/src/design/plone/ioprenoto/locales/en/
-drwxr-xr-x   0 roman      (502) staff       (20)        0 2023-04-06 15:54:42.729877 design.plone.ioprenoto-1.0.1/src/design/plone/ioprenoto/locales/en/LC_MESSAGES/
--rw-r--r--   0 roman      (502) staff       (20)        0 2023-04-06 15:54:42.000000 design.plone.ioprenoto-1.0.1/src/design/plone/ioprenoto/locales/en/LC_MESSAGES/design.plone.ioprenoto.po
--rw-r--r--   0 roman      (502) staff       (20)     1760 2023-04-06 15:54:42.000000 design.plone.ioprenoto-1.0.1/src/design/plone/ioprenoto/locales/update.py
--rwxr-xr-x   0 roman      (502) staff       (20)      503 2023-04-06 15:54:42.000000 design.plone.ioprenoto-1.0.1/src/design/plone/ioprenoto/locales/update.sh
--rw-r--r--   0 roman      (502) staff       (20)      414 2023-04-06 15:54:42.000000 design.plone.ioprenoto-1.0.1/src/design/plone/ioprenoto/permissions.zcml
-drwxr-xr-x   0 roman      (502) staff       (20)        0 2023-04-06 15:54:42.717558 design.plone.ioprenoto-1.0.1/src/design/plone/ioprenoto/profiles/
-drwxr-xr-x   0 roman      (502) staff       (20)        0 2023-04-06 15:54:42.730981 design.plone.ioprenoto-1.0.1/src/design/plone/ioprenoto/profiles/default/
--rw-r--r--   0 roman      (502) staff       (20)      191 2023-04-06 15:54:42.000000 design.plone.ioprenoto-1.0.1/src/design/plone/ioprenoto/profiles/default/browserlayer.xml
--rw-r--r--   0 roman      (502) staff       (20)      105 2023-04-06 15:54:42.000000 design.plone.ioprenoto-1.0.1/src/design/plone/ioprenoto/profiles/default/catalog.xml
--rw-r--r--   0 roman      (502) staff       (20)      191 2023-04-06 15:54:42.000000 design.plone.ioprenoto-1.0.1/src/design/plone/ioprenoto/profiles/default/metadata.xml
-drwxr-xr-x   0 roman      (502) staff       (20)        0 2023-04-06 15:54:42.731252 design.plone.ioprenoto-1.0.1/src/design/plone/ioprenoto/profiles/default/registry/
--rw-r--r--   0 roman      (502) staff       (20)      180 2023-04-06 15:54:42.000000 design.plone.ioprenoto-1.0.1/src/design/plone/ioprenoto/profiles/default/registry/main.xml
--rw-r--r--   0 roman      (502) staff       (20)      339 2023-04-06 15:54:42.000000 design.plone.ioprenoto-1.0.1/src/design/plone/ioprenoto/profiles/default/rolemap.xml
-drwxr-xr-x   0 roman      (502) staff       (20)        0 2023-04-06 15:54:42.731525 design.plone.ioprenoto-1.0.1/src/design/plone/ioprenoto/profiles/default/types/
--rw-r--r--   0 roman      (502) staff       (20)      476 2023-04-06 15:54:42.000000 design.plone.ioprenoto-1.0.1/src/design/plone/ioprenoto/profiles/default/types/PrenotazioniFolder.xml
-drwxr-xr-x   0 roman      (502) staff       (20)        0 2023-04-06 15:54:42.731796 design.plone.ioprenoto-1.0.1/src/design/plone/ioprenoto/profiles/uninstall/
--rw-r--r--   0 roman      (502) staff       (20)      132 2023-04-06 15:54:42.000000 design.plone.ioprenoto-1.0.1/src/design/plone/ioprenoto/profiles/uninstall/browserlayer.xml
-drwxr-xr-x   0 roman      (502) staff       (20)        0 2023-04-06 15:54:42.732280 design.plone.ioprenoto-1.0.1/src/design/plone/ioprenoto/restapi/
--rw-r--r--   0 roman      (502) staff       (20)        0 2023-04-06 15:54:42.000000 design.plone.ioprenoto-1.0.1/src/design/plone/ioprenoto/restapi/__init__.py
--rw-r--r--   0 roman      (502) staff       (20)      246 2023-04-06 15:54:42.000000 design.plone.ioprenoto-1.0.1/src/design/plone/ioprenoto/restapi/configure.zcml
-drwxr-xr-x   0 roman      (502) staff       (20)        0 2023-04-06 15:54:42.732760 design.plone.ioprenoto-1.0.1/src/design/plone/ioprenoto/restapi/serializers/
--rw-r--r--   0 roman      (502) staff       (20)        0 2023-04-06 15:54:42.000000 design.plone.ioprenoto-1.0.1/src/design/plone/ioprenoto/restapi/serializers/__init__.py
--rw-r--r--   0 roman      (502) staff       (20)      166 2023-04-06 15:54:42.000000 design.plone.ioprenoto-1.0.1/src/design/plone/ioprenoto/restapi/serializers/configure.zcml
-drwxr-xr-x   0 roman      (502) staff       (20)        0 2023-04-06 15:54:42.733829 design.plone.ioprenoto-1.0.1/src/design/plone/ioprenoto/restapi/serializers/ovverrides/
--rw-r--r--   0 roman      (502) staff       (20)        0 2023-04-06 15:54:42.000000 design.plone.ioprenoto-1.0.1/src/design/plone/ioprenoto/restapi/serializers/ovverrides/__init__.py
--rw-r--r--   0 roman      (502) staff       (20)      414 2023-04-06 15:54:42.000000 design.plone.ioprenoto-1.0.1/src/design/plone/ioprenoto/restapi/serializers/ovverrides/configure.zcml
--rw-r--r--   0 roman      (502) staff       (20)     1745 2023-04-06 15:54:42.000000 design.plone.ioprenoto-1.0.1/src/design/plone/ioprenoto/restapi/serializers/ovverrides/prenotazioniFolder.py
--rw-r--r--   0 roman      (502) staff       (20)     3329 2023-04-06 15:54:42.000000 design.plone.ioprenoto-1.0.1/src/design/plone/ioprenoto/restapi/serializers/ovverrides/servizio.py
--rw-r--r--   0 roman      (502) staff       (20)      794 2023-04-06 15:54:42.000000 design.plone.ioprenoto-1.0.1/src/design/plone/ioprenoto/setuphandlers.py
--rw-r--r--   0 roman      (502) staff       (20)     4058 2023-04-06 15:54:42.000000 design.plone.ioprenoto-1.0.1/src/design/plone/ioprenoto/testing.py
-drwxr-xr-x   0 roman      (502) staff       (20)        0 2023-04-06 15:54:42.735467 design.plone.ioprenoto-1.0.1/src/design/plone/ioprenoto/tests/
--rw-r--r--   0 roman      (502) staff       (20)        0 2023-04-06 15:54:42.000000 design.plone.ioprenoto-1.0.1/src/design/plone/ioprenoto/tests/__init__.py
-drwxr-xr-x   0 roman      (502) staff       (20)        0 2023-04-06 15:54:42.735805 design.plone.ioprenoto-1.0.1/src/design/plone/ioprenoto/tests/robot/
--rw-r--r--   0 roman      (502) staff       (20)     2019 2023-04-06 15:54:42.000000 design.plone.ioprenoto-1.0.1/src/design/plone/ioprenoto/tests/robot/test_example.robot
--rw-r--r--   0 roman      (502) staff       (20)      923 2023-04-06 15:54:42.000000 design.plone.ioprenoto-1.0.1/src/design/plone/ioprenoto/tests/test_PrenotazioniFolder_ct.py
--rw-r--r--   0 roman      (502) staff       (20)     2230 2023-04-06 15:54:42.000000 design.plone.ioprenoto-1.0.1/src/design/plone/ioprenoto/tests/test_restapi_serializers_ovverrides_prenotazioni_folder.py
--rw-r--r--   0 roman      (502) staff       (20)     2809 2023-04-06 15:54:42.000000 design.plone.ioprenoto-1.0.1/src/design/plone/ioprenoto/tests/test_restapi_serializers_ovverrides_serzvizio.py
--rw-r--r--   0 roman      (502) staff       (20)      961 2023-04-06 15:54:42.000000 design.plone.ioprenoto-1.0.1/src/design/plone/ioprenoto/tests/test_robot.py
--rw-r--r--   0 roman      (502) staff       (20)     2509 2023-04-06 15:54:42.000000 design.plone.ioprenoto-1.0.1/src/design/plone/ioprenoto/tests/test_setup.py
-drwxr-xr-x   0 roman      (502) staff       (20)        0 2023-04-06 15:54:42.723855 design.plone.ioprenoto-1.0.1/src/design.plone.ioprenoto.egg-info/
--rw-r--r--   0 roman      (502) staff       (20)     5182 2023-04-06 15:54:42.000000 design.plone.ioprenoto-1.0.1/src/design.plone.ioprenoto.egg-info/PKG-INFO
--rw-r--r--   0 roman      (502) staff       (20)     3015 2023-04-06 15:54:42.000000 design.plone.ioprenoto-1.0.1/src/design.plone.ioprenoto.egg-info/SOURCES.txt
--rw-r--r--   0 roman      (502) staff       (20)        1 2023-04-06 15:54:42.000000 design.plone.ioprenoto-1.0.1/src/design.plone.ioprenoto.egg-info/dependency_links.txt
--rw-r--r--   0 roman      (502) staff       (20)      147 2023-04-06 15:54:42.000000 design.plone.ioprenoto-1.0.1/src/design.plone.ioprenoto.egg-info/entry_points.txt
--rw-r--r--   0 roman      (502) staff       (20)       20 2023-04-06 15:54:42.000000 design.plone.ioprenoto-1.0.1/src/design.plone.ioprenoto.egg-info/namespace_packages.txt
--rw-r--r--   0 roman      (502) staff       (20)        1 2023-04-06 15:54:42.000000 design.plone.ioprenoto-1.0.1/src/design.plone.ioprenoto.egg-info/not-zip-safe
--rw-r--r--   0 roman      (502) staff       (20)      281 2023-04-06 15:54:42.000000 design.plone.ioprenoto-1.0.1/src/design.plone.ioprenoto.egg-info/requires.txt
--rw-r--r--   0 roman      (502) staff       (20)        7 2023-04-06 15:54:42.000000 design.plone.ioprenoto-1.0.1/src/design.plone.ioprenoto.egg-info/top_level.txt
+drwxrwxr-x   0 mauro     (1000) mauro     (1000)        0 2023-06-12 12:43:34.779759 design.plone.ioprenoto-1.0.2/
+-rw-rw-r--   0 mauro     (1000) mauro     (1000)      367 2023-06-12 12:43:34.000000 design.plone.ioprenoto-1.0.2/CHANGES.rst
+-rw-rw-r--   0 mauro     (1000) mauro     (1000)       58 2023-06-12 12:43:34.000000 design.plone.ioprenoto-1.0.2/CONTRIBUTORS.rst
+-rw-rw-r--   0 mauro     (1000) mauro     (1000)     1338 2023-06-12 12:43:34.000000 design.plone.ioprenoto-1.0.2/DEVELOP.rst
+-rw-rw-r--   0 mauro     (1000) mauro     (1000)    18092 2023-06-12 12:43:34.000000 design.plone.ioprenoto-1.0.2/LICENSE.GPL
+-rw-rw-r--   0 mauro     (1000) mauro     (1000)      662 2023-06-12 12:43:34.000000 design.plone.ioprenoto-1.0.2/LICENSE.rst
+-rw-rw-r--   0 mauro     (1000) mauro     (1000)      116 2023-06-12 12:43:34.000000 design.plone.ioprenoto-1.0.2/MANIFEST.in
+-rw-rw-r--   0 mauro     (1000) mauro     (1000)     5953 2023-06-12 12:43:34.779759 design.plone.ioprenoto-1.0.2/PKG-INFO
+-rw-rw-r--   0 mauro     (1000) mauro     (1000)     4344 2023-06-12 12:43:34.000000 design.plone.ioprenoto-1.0.2/README.rst
+drwxrwxr-x   0 mauro     (1000) mauro     (1000)        0 2023-06-12 12:43:34.779759 design.plone.ioprenoto-1.0.2/docs/
+-rw-rw-r--   0 mauro     (1000) mauro     (1000)     7986 2023-06-12 12:43:34.000000 design.plone.ioprenoto-1.0.2/docs/conf.py
+-rw-rw-r--   0 mauro     (1000) mauro     (1000)       89 2023-06-12 12:43:34.000000 design.plone.ioprenoto-1.0.2/docs/index.rst
+-rw-rw-r--   0 mauro     (1000) mauro     (1000)      340 2023-06-12 12:43:34.779759 design.plone.ioprenoto-1.0.2/setup.cfg
+-rw-rw-r--   0 mauro     (1000) mauro     (1000)     2786 2023-06-12 12:43:34.000000 design.plone.ioprenoto-1.0.2/setup.py
+drwxrwxr-x   0 mauro     (1000) mauro     (1000)        0 2023-06-12 12:43:34.775759 design.plone.ioprenoto-1.0.2/src/
+drwxrwxr-x   0 mauro     (1000) mauro     (1000)        0 2023-06-12 12:43:34.779759 design.plone.ioprenoto-1.0.2/src/design/
+-rw-rw-r--   0 mauro     (1000) mauro     (1000)       80 2023-06-12 12:43:34.000000 design.plone.ioprenoto-1.0.2/src/design/__init__.py
+drwxrwxr-x   0 mauro     (1000) mauro     (1000)        0 2023-06-12 12:43:34.779759 design.plone.ioprenoto-1.0.2/src/design/plone/
+-rw-rw-r--   0 mauro     (1000) mauro     (1000)       80 2023-06-12 12:43:34.000000 design.plone.ioprenoto-1.0.2/src/design/plone/__init__.py
+drwxrwxr-x   0 mauro     (1000) mauro     (1000)        0 2023-06-12 12:43:34.779759 design.plone.ioprenoto-1.0.2/src/design/plone/ioprenoto/
+-rw-rw-r--   0 mauro     (1000) mauro     (1000)      139 2023-06-12 12:43:34.000000 design.plone.ioprenoto-1.0.2/src/design/plone/ioprenoto/__init__.py
+drwxrwxr-x   0 mauro     (1000) mauro     (1000)        0 2023-06-12 12:43:34.779759 design.plone.ioprenoto-1.0.2/src/design/plone/ioprenoto/adapters/
+-rw-rw-r--   0 mauro     (1000) mauro     (1000)       24 2023-06-12 12:43:34.000000 design.plone.ioprenoto-1.0.2/src/design/plone/ioprenoto/adapters/__init__.py
+-rw-rw-r--   0 mauro     (1000) mauro     (1000)      562 2023-06-12 12:43:34.000000 design.plone.ioprenoto-1.0.2/src/design/plone/ioprenoto/adapters/configure.zcml
+-rw-rw-r--   0 mauro     (1000) mauro     (1000)     1015 2023-06-12 12:43:34.000000 design.plone.ioprenoto-1.0.2/src/design/plone/ioprenoto/adapters/stringinterp.py
+drwxrwxr-x   0 mauro     (1000) mauro     (1000)        0 2023-06-12 12:43:34.779759 design.plone.ioprenoto-1.0.2/src/design/plone/ioprenoto/behaviors/
+-rw-rw-r--   0 mauro     (1000) mauro     (1000)        0 2023-06-12 12:43:34.000000 design.plone.ioprenoto-1.0.2/src/design/plone/ioprenoto/behaviors/__init__.py
+-rw-rw-r--   0 mauro     (1000) mauro     (1000)     1392 2023-06-12 12:43:34.000000 design.plone.ioprenoto-1.0.2/src/design/plone/ioprenoto/behaviors/additional_fields.py
+-rw-rw-r--   0 mauro     (1000) mauro     (1000)      591 2023-06-12 12:43:34.000000 design.plone.ioprenoto-1.0.2/src/design/plone/ioprenoto/behaviors/configure.zcml
+drwxrwxr-x   0 mauro     (1000) mauro     (1000)        0 2023-06-12 12:43:34.779759 design.plone.ioprenoto-1.0.2/src/design/plone/ioprenoto/browser/
+-rw-rw-r--   0 mauro     (1000) mauro     (1000)        0 2023-06-12 12:43:34.000000 design.plone.ioprenoto-1.0.2/src/design/plone/ioprenoto/browser/__init__.py
+-rw-rw-r--   0 mauro     (1000) mauro     (1000)      628 2023-06-12 12:43:34.000000 design.plone.ioprenoto-1.0.2/src/design/plone/ioprenoto/browser/configure.zcml
+drwxrwxr-x   0 mauro     (1000) mauro     (1000)        0 2023-06-12 12:43:34.779759 design.plone.ioprenoto-1.0.2/src/design/plone/ioprenoto/browser/overrides/
+-rw-rw-r--   0 mauro     (1000) mauro     (1000)        0 2023-06-12 12:43:34.000000 design.plone.ioprenoto-1.0.2/src/design/plone/ioprenoto/browser/overrides/.gitkeep
+drwxrwxr-x   0 mauro     (1000) mauro     (1000)        0 2023-06-12 12:43:34.779759 design.plone.ioprenoto-1.0.2/src/design/plone/ioprenoto/browser/static/
+-rw-rw-r--   0 mauro     (1000) mauro     (1000)        0 2023-06-12 12:43:34.000000 design.plone.ioprenoto-1.0.2/src/design/plone/ioprenoto/browser/static/.gitkeep
+-rw-rw-r--   0 mauro     (1000) mauro     (1000)     1530 2023-06-12 12:43:34.000000 design.plone.ioprenoto-1.0.2/src/design/plone/ioprenoto/configure.zcml
+drwxrwxr-x   0 mauro     (1000) mauro     (1000)        0 2023-06-12 12:43:34.779759 design.plone.ioprenoto-1.0.2/src/design/plone/ioprenoto/events/
+-rw-rw-r--   0 mauro     (1000) mauro     (1000)       24 2023-06-12 12:43:34.000000 design.plone.ioprenoto-1.0.2/src/design/plone/ioprenoto/events/__init__.py
+-rw-rw-r--   0 mauro     (1000) mauro     (1000)      431 2023-06-12 12:43:34.000000 design.plone.ioprenoto-1.0.2/src/design/plone/ioprenoto/events/configure.zcml
+-rw-rw-r--   0 mauro     (1000) mauro     (1000)      136 2023-06-12 12:43:34.000000 design.plone.ioprenoto-1.0.2/src/design/plone/ioprenoto/events/on_create.py
+-rw-rw-r--   0 mauro     (1000) mauro     (1000)      270 2023-06-12 12:43:34.000000 design.plone.ioprenoto-1.0.2/src/design/plone/ioprenoto/interfaces.py
+drwxrwxr-x   0 mauro     (1000) mauro     (1000)        0 2023-06-12 12:43:34.779759 design.plone.ioprenoto-1.0.2/src/design/plone/ioprenoto/locales/
+-rw-rw-r--   0 mauro     (1000) mauro     (1000)      611 2023-06-12 12:43:34.000000 design.plone.ioprenoto-1.0.2/src/design/plone/ioprenoto/locales/README.rst
+-rw-rw-r--   0 mauro     (1000) mauro     (1000)        0 2023-06-12 12:43:34.000000 design.plone.ioprenoto-1.0.2/src/design/plone/ioprenoto/locales/__init__.py
+-rw-rw-r--   0 mauro     (1000) mauro     (1000)        0 2023-06-12 12:43:34.000000 design.plone.ioprenoto-1.0.2/src/design/plone/ioprenoto/locales/design.plone.ioprenoto.pot
+drwxrwxr-x   0 mauro     (1000) mauro     (1000)        0 2023-06-12 12:43:34.779759 design.plone.ioprenoto-1.0.2/src/design/plone/ioprenoto/locales/en/
+drwxrwxr-x   0 mauro     (1000) mauro     (1000)        0 2023-06-12 12:43:34.779759 design.plone.ioprenoto-1.0.2/src/design/plone/ioprenoto/locales/en/LC_MESSAGES/
+-rw-rw-r--   0 mauro     (1000) mauro     (1000)        0 2023-06-12 12:43:34.000000 design.plone.ioprenoto-1.0.2/src/design/plone/ioprenoto/locales/en/LC_MESSAGES/design.plone.ioprenoto.po
+-rw-rw-r--   0 mauro     (1000) mauro     (1000)     1760 2023-06-12 12:43:34.000000 design.plone.ioprenoto-1.0.2/src/design/plone/ioprenoto/locales/update.py
+-rwxrwxr-x   0 mauro     (1000) mauro     (1000)      503 2023-06-12 12:43:34.000000 design.plone.ioprenoto-1.0.2/src/design/plone/ioprenoto/locales/update.sh
+-rw-rw-r--   0 mauro     (1000) mauro     (1000)      273 2023-06-12 12:43:34.000000 design.plone.ioprenoto-1.0.2/src/design/plone/ioprenoto/permissions.zcml
+drwxrwxr-x   0 mauro     (1000) mauro     (1000)        0 2023-06-12 12:43:34.779759 design.plone.ioprenoto-1.0.2/src/design/plone/ioprenoto/profiles/
+drwxrwxr-x   0 mauro     (1000) mauro     (1000)        0 2023-06-12 12:43:34.779759 design.plone.ioprenoto-1.0.2/src/design/plone/ioprenoto/profiles/default/
+-rw-rw-r--   0 mauro     (1000) mauro     (1000)      191 2023-06-12 12:43:34.000000 design.plone.ioprenoto-1.0.2/src/design/plone/ioprenoto/profiles/default/browserlayer.xml
+-rw-rw-r--   0 mauro     (1000) mauro     (1000)      105 2023-06-12 12:43:34.000000 design.plone.ioprenoto-1.0.2/src/design/plone/ioprenoto/profiles/default/catalog.xml
+-rw-rw-r--   0 mauro     (1000) mauro     (1000)      191 2023-06-12 12:43:34.000000 design.plone.ioprenoto-1.0.2/src/design/plone/ioprenoto/profiles/default/metadata.xml
+drwxrwxr-x   0 mauro     (1000) mauro     (1000)        0 2023-06-12 12:43:34.779759 design.plone.ioprenoto-1.0.2/src/design/plone/ioprenoto/profiles/default/registry/
+-rw-rw-r--   0 mauro     (1000) mauro     (1000)      180 2023-06-12 12:43:34.000000 design.plone.ioprenoto-1.0.2/src/design/plone/ioprenoto/profiles/default/registry/main.xml
+-rw-rw-r--   0 mauro     (1000) mauro     (1000)      340 2023-06-12 12:43:34.000000 design.plone.ioprenoto-1.0.2/src/design/plone/ioprenoto/profiles/default/rolemap.xml
+drwxrwxr-x   0 mauro     (1000) mauro     (1000)        0 2023-06-12 12:43:34.779759 design.plone.ioprenoto-1.0.2/src/design/plone/ioprenoto/profiles/default/types/
+-rw-rw-r--   0 mauro     (1000) mauro     (1000)      325 2023-06-12 12:43:34.000000 design.plone.ioprenoto-1.0.2/src/design/plone/ioprenoto/profiles/default/types/PrenotazioniFolder.xml
+drwxrwxr-x   0 mauro     (1000) mauro     (1000)        0 2023-06-12 12:43:34.779759 design.plone.ioprenoto-1.0.2/src/design/plone/ioprenoto/profiles/uninstall/
+-rw-rw-r--   0 mauro     (1000) mauro     (1000)      132 2023-06-12 12:43:34.000000 design.plone.ioprenoto-1.0.2/src/design/plone/ioprenoto/profiles/uninstall/browserlayer.xml
+drwxrwxr-x   0 mauro     (1000) mauro     (1000)        0 2023-06-12 12:43:34.779759 design.plone.ioprenoto-1.0.2/src/design/plone/ioprenoto/restapi/
+-rw-rw-r--   0 mauro     (1000) mauro     (1000)        0 2023-06-12 12:43:34.000000 design.plone.ioprenoto-1.0.2/src/design/plone/ioprenoto/restapi/__init__.py
+-rw-rw-r--   0 mauro     (1000) mauro     (1000)      280 2023-06-12 12:43:34.000000 design.plone.ioprenoto-1.0.2/src/design/plone/ioprenoto/restapi/configure.zcml
+drwxrwxr-x   0 mauro     (1000) mauro     (1000)        0 2023-06-12 12:43:34.779759 design.plone.ioprenoto-1.0.2/src/design/plone/ioprenoto/restapi/serializers/
+-rw-rw-r--   0 mauro     (1000) mauro     (1000)        0 2023-06-12 12:43:34.000000 design.plone.ioprenoto-1.0.2/src/design/plone/ioprenoto/restapi/serializers/__init__.py
+-rw-rw-r--   0 mauro     (1000) mauro     (1000)      166 2023-06-12 12:43:34.000000 design.plone.ioprenoto-1.0.2/src/design/plone/ioprenoto/restapi/serializers/configure.zcml
+drwxrwxr-x   0 mauro     (1000) mauro     (1000)        0 2023-06-12 12:43:34.779759 design.plone.ioprenoto-1.0.2/src/design/plone/ioprenoto/restapi/serializers/ovverrides/
+-rw-rw-r--   0 mauro     (1000) mauro     (1000)        0 2023-06-12 12:43:34.000000 design.plone.ioprenoto-1.0.2/src/design/plone/ioprenoto/restapi/serializers/ovverrides/__init__.py
+-rw-rw-r--   0 mauro     (1000) mauro     (1000)      414 2023-06-12 12:43:34.000000 design.plone.ioprenoto-1.0.2/src/design/plone/ioprenoto/restapi/serializers/ovverrides/configure.zcml
+-rw-rw-r--   0 mauro     (1000) mauro     (1000)     1685 2023-06-12 12:43:34.000000 design.plone.ioprenoto-1.0.2/src/design/plone/ioprenoto/restapi/serializers/ovverrides/prenotazioniFolder.py
+-rw-rw-r--   0 mauro     (1000) mauro     (1000)     2773 2023-06-12 12:43:34.000000 design.plone.ioprenoto-1.0.2/src/design/plone/ioprenoto/restapi/serializers/ovverrides/servizio.py
+drwxrwxr-x   0 mauro     (1000) mauro     (1000)        0 2023-06-12 12:43:34.779759 design.plone.ioprenoto-1.0.2/src/design/plone/ioprenoto/restapi/services/
+drwxrwxr-x   0 mauro     (1000) mauro     (1000)        0 2023-06-12 12:43:34.779759 design.plone.ioprenoto-1.0.2/src/design/plone/ioprenoto/restapi/services/bookable_list/
+-rw-rw-r--   0 mauro     (1000) mauro     (1000)      476 2023-06-12 12:43:34.000000 design.plone.ioprenoto-1.0.2/src/design/plone/ioprenoto/restapi/services/bookable_list/configure.zcml
+-rw-rw-r--   0 mauro     (1000) mauro     (1000)     6147 2023-06-12 12:43:34.000000 design.plone.ioprenoto-1.0.2/src/design/plone/ioprenoto/restapi/services/bookable_list/get.py
+-rw-rw-r--   0 mauro     (1000) mauro     (1000)      167 2023-06-12 12:43:34.000000 design.plone.ioprenoto-1.0.2/src/design/plone/ioprenoto/restapi/services/configure.zcml
+-rw-rw-r--   0 mauro     (1000) mauro     (1000)      794 2023-06-12 12:43:34.000000 design.plone.ioprenoto-1.0.2/src/design/plone/ioprenoto/setuphandlers.py
+-rw-rw-r--   0 mauro     (1000) mauro     (1000)     1930 2023-06-12 12:43:34.000000 design.plone.ioprenoto-1.0.2/src/design/plone/ioprenoto/testing.py
+drwxrwxr-x   0 mauro     (1000) mauro     (1000)        0 2023-06-12 12:43:34.779759 design.plone.ioprenoto-1.0.2/src/design/plone/ioprenoto/tests/
+-rw-rw-r--   0 mauro     (1000) mauro     (1000)        0 2023-06-12 12:43:34.000000 design.plone.ioprenoto-1.0.2/src/design/plone/ioprenoto/tests/__init__.py
+drwxrwxr-x   0 mauro     (1000) mauro     (1000)        0 2023-06-12 12:43:34.779759 design.plone.ioprenoto-1.0.2/src/design/plone/ioprenoto/tests/robot/
+-rw-rw-r--   0 mauro     (1000) mauro     (1000)     2019 2023-06-12 12:43:34.000000 design.plone.ioprenoto-1.0.2/src/design/plone/ioprenoto/tests/robot/test_example.robot
+-rw-rw-r--   0 mauro     (1000) mauro     (1000)     1231 2023-06-12 12:43:34.000000 design.plone.ioprenoto-1.0.2/src/design/plone/ioprenoto/tests/test_PrenotazioniFolder_ct.py
+-rw-rw-r--   0 mauro     (1000) mauro     (1000)     2221 2023-06-12 12:43:34.000000 design.plone.ioprenoto-1.0.2/src/design/plone/ioprenoto/tests/test_restapi_serializers_ovverrides_prenotazioni_folder.py
+-rw-rw-r--   0 mauro     (1000) mauro     (1000)     2800 2023-06-12 12:43:34.000000 design.plone.ioprenoto-1.0.2/src/design/plone/ioprenoto/tests/test_restapi_serializers_ovverrides_serzvizio.py
+-rw-rw-r--   0 mauro     (1000) mauro     (1000)     6427 2023-06-12 12:43:34.000000 design.plone.ioprenoto-1.0.2/src/design/plone/ioprenoto/tests/test_restapi_service_bookable_uo_list.py
+-rw-rw-r--   0 mauro     (1000) mauro     (1000)     2459 2023-06-12 12:43:34.000000 design.plone.ioprenoto-1.0.2/src/design/plone/ioprenoto/tests/test_setup.py
+-rw-rw-r--   0 mauro     (1000) mauro     (1000)     4095 2023-06-12 12:43:34.000000 design.plone.ioprenoto-1.0.2/src/design/plone/ioprenoto/tests/test_stringinterp_overrides.py
+drwxrwxr-x   0 mauro     (1000) mauro     (1000)        0 2023-06-12 12:43:34.779759 design.plone.ioprenoto-1.0.2/src/design.plone.ioprenoto.egg-info/
+-rw-rw-r--   0 mauro     (1000) mauro     (1000)     5953 2023-06-12 12:43:34.000000 design.plone.ioprenoto-1.0.2/src/design.plone.ioprenoto.egg-info/PKG-INFO
+-rw-rw-r--   0 mauro     (1000) mauro     (1000)     3480 2023-06-12 12:43:34.000000 design.plone.ioprenoto-1.0.2/src/design.plone.ioprenoto.egg-info/SOURCES.txt
+-rw-rw-r--   0 mauro     (1000) mauro     (1000)        1 2023-06-12 12:43:34.000000 design.plone.ioprenoto-1.0.2/src/design.plone.ioprenoto.egg-info/dependency_links.txt
+-rw-rw-r--   0 mauro     (1000) mauro     (1000)      127 2023-06-12 12:43:34.000000 design.plone.ioprenoto-1.0.2/src/design.plone.ioprenoto.egg-info/entry_points.txt
+-rw-rw-r--   0 mauro     (1000) mauro     (1000)       20 2023-06-12 12:43:34.000000 design.plone.ioprenoto-1.0.2/src/design.plone.ioprenoto.egg-info/namespace_packages.txt
+-rw-rw-r--   0 mauro     (1000) mauro     (1000)        1 2023-06-12 12:43:34.000000 design.plone.ioprenoto-1.0.2/src/design.plone.ioprenoto.egg-info/not-zip-safe
+-rw-rw-r--   0 mauro     (1000) mauro     (1000)      281 2023-06-12 12:43:34.000000 design.plone.ioprenoto-1.0.2/src/design.plone.ioprenoto.egg-info/requires.txt
+-rw-rw-r--   0 mauro     (1000) mauro     (1000)        7 2023-06-12 12:43:34.000000 design.plone.ioprenoto-1.0.2/src/design.plone.ioprenoto.egg-info/top_level.txt
```

### Comparing `design.plone.ioprenoto-1.0.1/DEVELOP.rst` & `design.plone.ioprenoto-1.0.2/DEVELOP.rst`

 * *Files identical despite different names*

### Comparing `design.plone.ioprenoto-1.0.1/LICENSE.GPL` & `design.plone.ioprenoto-1.0.2/LICENSE.GPL`

 * *Files identical despite different names*

### Comparing `design.plone.ioprenoto-1.0.1/LICENSE.rst` & `design.plone.ioprenoto-1.0.2/LICENSE.rst`

 * *Files identical despite different names*

### Comparing `design.plone.ioprenoto-1.0.1/docs/conf.py` & `design.plone.ioprenoto-1.0.2/docs/conf.py`

 * *Files identical despite different names*

### Comparing `design.plone.ioprenoto-1.0.1/setup.py` & `design.plone.ioprenoto-1.0.2/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -12,40 +12,41 @@
         open("CHANGES.rst").read(),
     ]
 )
 
 
 setup(
     name="design.plone.ioprenoto",
-    version="1.0.1",
+    version="1.0.2",
     description="An add-on for Plone",
     long_description=long_description,
     # Get more from https://pypi.org/classifiers/
     classifiers=[
         "Environment :: Web Environment",
         "Framework :: Plone",
         "Framework :: Plone :: Addon",
         "Framework :: Plone :: 5.2",
         "Framework :: Plone :: 6.0",
         "Programming Language :: Python",
-        "Programming Language :: Python :: 3.7",
         "Programming Language :: Python :: 3.8",
         "Programming Language :: Python :: 3.9",
+        "Programming Language :: Python :: 3.10",
+        "Programming Language :: Python :: 3.11",
         "Operating System :: OS Independent",
         "License :: OSI Approved :: GNU General Public License v2 (GPLv2)",
-        "Development Status :: 4 - Beta"
+        "Development Status :: 4 - Beta",
     ],
     keywords="Python Plone CMS",
     author="RedTurtle",
     author_email="info@redturtle.it",
     url="https://github.com/collective/design.plone.ioprenoto",
     project_urls={
         "PyPI": "https://pypi.org/project/design.plone.ioprenoto/",
-        "Source": "https://github.com/collective/design.plone.ioprenoto",
-        "Tracker": "https://github.com/collective/design.plone.ioprenoto/issues",
+        "Source": "https://github.com/RedTurtle/design.plone.ioprenoto",
+        "Tracker": "https://github.com/RedTurtle/design.plone.ioprenoto/issues",
         # 'Documentation': 'https://design.plone.ioprenoto.readthedocs.io/en/latest/',
     },
     license="GPL version 2",
     packages=find_packages("src", exclude=["ez_setup"]),
     namespace_packages=["design", "design.plone"],
     package_dir={"": "src"},
     include_package_data=True,
```

### Comparing `design.plone.ioprenoto-1.0.1/src/design/plone/ioprenoto/behaviors/punto_di_contatto.py` & `design.plone.ioprenoto-1.0.2/src/design/plone/ioprenoto/behaviors/additional_fields.py`

 * *Files 27% similar despite different names*

```diff
@@ -1,36 +1,44 @@
 from design.plone.ioprenoto import _
-from plone.app.vocabularies.catalog import CatalogSource
-from plone.app.z3cform.widget import RelatedItemsFieldWidget
-from plone.autoform import directives
 from plone.autoform.interfaces import IFormFieldProvider
+from plone.app.z3cform.widget import RelatedItemsFieldWidget
+from plone.app.vocabularies.catalog import CatalogSource
 from plone.supermodel import model
+from plone.autoform import directives
+from zope.interface import provider
+from zope.schema import Text
 from z3c.relationfield.schema import RelationChoice
 from z3c.relationfield.schema import RelationList
-from zope.interface import provider
 
 
 @provider(IFormFieldProvider)
-class IPuntoDiContatto(model.Schema):
-    """Add tags to content"""
+class IAdditionalFields(model.Schema):
+    """Add fields to content"""
 
-    punto_di_contatto = RelationList(
-        title=_("Punto di contatto"),
+    orario_di_apertura = Text(
+        title=_("Orario di apertura"),
+        description=_("Orario di apertura della stanza prenotazioni"),
+        required=False,
+    )
+    uffici_correlati = RelationList(
+        title=_("Uffici corellati"),
+        description=_("Uffici correlati al contesto corrente"),
         value_type=RelationChoice(
-            title=_("Punto di contatto"),
-            source=CatalogSource(portal_type="PuntoDiContatto"),
+            title=_("Ufficio"),
+            source=CatalogSource(portal_type="UnitaOrganizzativa"),
         ),
     )
+
     directives.widget(
-        "punto_di_contatto",
+        "uffici_correlati",
         RelatedItemsFieldWidget,
         vocabulary="plone.app.vocabularies.Catalog",
         pattern_options={
-            "maximumSelectionSize": 1,
-            "selectableTypes": ["PuntoDiContatto"],
+            "maximumSelectionSize": 100,
+            "selectableTypes": ["UnitaOrganizzativa"],
         },
     )
 
 
-class PuntoDiContatto(object):
+class AdditionalFields(object):
     def __init__(self, context):
         self.context = context
```

### Comparing `design.plone.ioprenoto-1.0.1/src/design/plone/ioprenoto/browser/configure.zcml` & `design.plone.ioprenoto-1.0.2/src/design/plone/ioprenoto/browser/configure.zcml`

 * *Files identical despite different names*

### Comparing `design.plone.ioprenoto-1.0.1/src/design/plone/ioprenoto/configure.zcml` & `design.plone.ioprenoto-1.0.2/src/design/plone/ioprenoto/configure.zcml`

 * *Files 7% similar despite different names*

```diff
@@ -10,15 +10,17 @@
 
   <!--
     Be careful if you use general includeDependencies, it can have side effects!
     Better import explicit packages or configurations ;)
   -->
   <!--<includeDependencies package="." />-->
 
+  <include package=".adapters" />
   <include package=".browser" />
+  <include package=".events" />
   <include package=".behaviors" />
   <include package=".restapi" />
 
   <include file="permissions.zcml" />
 
   <genericsetup:registerProfile
       name="default"
```

### Comparing `design.plone.ioprenoto-1.0.1/src/design/plone/ioprenoto/locales/README.rst` & `design.plone.ioprenoto-1.0.2/src/design/plone/ioprenoto/locales/README.rst`

 * *Files identical despite different names*

### Comparing `design.plone.ioprenoto-1.0.1/src/design/plone/ioprenoto/locales/update.py` & `design.plone.ioprenoto-1.0.2/src/design/plone/ioprenoto/locales/update.py`

 * *Files identical despite different names*

### Comparing `design.plone.ioprenoto-1.0.1/src/design/plone/ioprenoto/restapi/serializers/ovverrides/prenotazioniFolder.py` & `design.plone.ioprenoto-1.0.2/src/design/plone/ioprenoto/restapi/serializers/ovverrides/prenotazioniFolder.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,16 +1,14 @@
 from design.plone.ioprenoto.interfaces import IDesignPloneIoprenotoLayer
 from plone import api
 from plone.restapi.interfaces import ISerializeToJson
 from plone.restapi.interfaces import ISerializeToJsonSummary
 from plone.restapi.serializer.dxcontent import SerializeFolderToJson
 from plone.restapi.serializer.summary import DefaultJSONSummarySerializer
-from redturtle.prenotazioni.content.prenotazioni_folder import (
-    IPrenotazioniFolder,
-)
+from redturtle.prenotazioni.content.prenotazioni_folder import IPrenotazioniFolder
 from zope.component import adapter
 from zope.interface import implementer
 
 
 PRENOTAZIONI_MANAGE_PERMISSION = "redturtle.prenotazioni.ManagePrenotazioni"
 PRENOTAZIONE_APPUNTAMENTO_ADDRESS = "prenotazione-appuntamento"
 
@@ -31,17 +29,15 @@
         return super().__call__(*args, **kwargs)
 
 
 @implementer(ISerializeToJson)
 @adapter(IPrenotazioniFolder, IDesignPloneIoprenotoLayer)
 class SerializePrenotazioniFolderToJson(SerializeFolderToJson):
     def __call__(self, *args, **kwargs):
-        if not api.user.has_permission(
-            PRENOTAZIONI_MANAGE_PERMISSION, user=api.user.get_current()
-        ):
+        if not api.user.has_permission(PRENOTAZIONI_MANAGE_PERMISSION):
             self.request.response.redirect(
                 self.context.portal_url() + "/" + PRENOTAZIONE_APPUNTAMENTO_ADDRESS
             )
 
             return
 
         return super().__call__(*args, **kwargs)
```

### Comparing `design.plone.ioprenoto-1.0.1/src/design/plone/ioprenoto/restapi/serializers/ovverrides/servizio.py` & `design.plone.ioprenoto-1.0.2/src/design/plone/ioprenoto/restapi/serializers/ovverrides/servizio.py`

 * *Files 19% similar despite different names*

```diff
@@ -11,94 +11,71 @@
 from zope.component import adapter
 from zope.component import getUtility
 from zope.interface import implementer
 from zope.intid.interfaces import IIntIds
 from zope.intid.interfaces import IntIdMissingError
 
 
-class CartellaPrenotazioneBackreferences:
-    @staticmethod
-    def has_backreferences(service):
-        """Returns backreferences to PrenotazioniFolder throught correlated UO"""
-
-        referenced_uo = [
-            i.to_object
-            for i in (
-                CartellaPrenotazioneBackreferences.get_referenced_relations_from_obj
-            )(service)
-            if i.to_object.portal_type == "UnitaOrganizzativa"
-        ]
-        pernotazioni_folder_refencing_uo = []
-
-        for uo in referenced_uo:
-            folders = [
-                i
-                for i in (
-                    CartellaPrenotazioneBackreferences.get_referenced_relations_to_obj
-                )(uo)
-                if i.from_object.portal_type == "PrenotazioniFolder"
-            ]
-
-            if folders:
-                pernotazioni_folder_refencing_uo += folders
-
-        return bool(pernotazioni_folder_refencing_uo)
-
-    @staticmethod
-    def get_referenced_relations_from_obj(obj):
-        catalog = getUtility(ICatalog)
-        intids = getUtility(IIntIds)
-
-        try:
-            relations = catalog.findRelations(
-                dict(
-                    from_id=intids.getId(aq_inner(obj)),
-                )
+def has_backreferences(service):
+    """Returns true if service has backreferences to PrenotazioniFolder
+    throught correlated UO"""
+    for ref_ou in get_referenced_relations_from_obj(service):
+        if ref_ou.to_object and ref_ou.to_object.portal_type == "UnitaOrganizzativa":
+            for ref_pf in get_referenced_relations_to_obj(ref_ou.to_object):
+                if (
+                    ref_pf.from_object
+                    and ref_pf.from_object.portal_type == "PrenotazioniFolder"
+                ):
+                    return True
+    return False
+
+
+def get_referenced_relations_from_obj(obj):
+    catalog = getUtility(ICatalog)
+    intids = getUtility(IIntIds)
+    try:
+        relations = catalog.findRelations(
+            dict(
+                from_id=intids.getId(aq_inner(obj)),
             )
-        except IntIdMissingError:
-            return []
+        )
+    except IntIdMissingError:
+        return []
+    return list(relations)
 
-        return list(relations)
 
-    @staticmethod
-    def get_referenced_relations_to_obj(obj):
-        catalog = getUtility(ICatalog)
-        intids = getUtility(IIntIds)
-
-        try:
-            relations = catalog.findRelations(
-                dict(
-                    to_id=intids.getId(aq_inner(obj)),
-                )
+def get_referenced_relations_to_obj(obj):
+    catalog = getUtility(ICatalog)
+    intids = getUtility(IIntIds)
+    try:
+        relations = catalog.findRelations(
+            dict(
+                to_id=intids.getId(aq_inner(obj)),
             )
-        except IntIdMissingError:
-            return []
-
-        return list(relations)
+        )
+    except IntIdMissingError:
+        return []
+    return list(relations)
 
 
 @implementer(ISerializeToJsonSummary)
 @adapter(IServizio, IDesignPloneIoprenotoLayer)
 class SerializeServizioToJsonSummary(ServizioSummaryOriginal):
     def __call__(self, *args, **kwargs):
         result = super().__call__(*args, **kwargs)
-
         if result:
-            result[
-                "referenced_by_prenotazioni_folder"
-            ] = CartellaPrenotazioneBackreferences.has_backreferences(self.context)
-
+            result["referenced_by_prenotazioni_folder"] = has_backreferences(
+                self.context
+            )
         return result
 
 
 @implementer(ISerializeToJson)
 @adapter(IServizio, IDesignPloneIoprenotoLayer)
 class SerializeServizioToJson(SerializeFolderToJson):
     def __call__(self, *args, **kwargs):
         result = super().__call__(*args, **kwargs)
-
         if result:
-            result[
-                "referenced_by_prenotazioni_folder"
-            ] = CartellaPrenotazioneBackreferences.has_backreferences(self.context)
-
+            result["referenced_by_prenotazioni_folder"] = has_backreferences(
+                self.context
+            )
         return result
```

### Comparing `design.plone.ioprenoto-1.0.1/src/design/plone/ioprenoto/setuphandlers.py` & `design.plone.ioprenoto-1.0.2/src/design/plone/ioprenoto/setuphandlers.py`

 * *Files identical despite different names*

### Comparing `design.plone.ioprenoto-1.0.1/src/design/plone/ioprenoto/tests/robot/test_example.robot` & `design.plone.ioprenoto-1.0.2/src/design/plone/ioprenoto/tests/robot/test_example.robot`

 * *Files identical despite different names*

### Comparing `design.plone.ioprenoto-1.0.1/src/design/plone/ioprenoto/tests/test_PrenotazioniFolder_ct.py` & `design.plone.ioprenoto-1.0.2/src/design/plone/ioprenoto/tests/test_PrenotazioniFolder_ct.py`

 * *Files 23% similar despite different names*

```diff
@@ -1,29 +1,37 @@
 # -*- coding: utf-8 -*-
 
-from design.plone.ioprenoto.testing import (
-    DESIGN_PLONE_IOPRENOTO_INTEGRATION_TESTING,
-)
+from design.plone.ioprenoto.testing import DESIGN_PLONE_IOPRENOTO_INTEGRATION_TESTING
 from plone import api
+from plone.app.testing import setRoles
+from plone.app.testing import TEST_USER_ID
 
 import unittest
 
 
 class TestPrenotazioniFolder(unittest.TestCase):
     layer = DESIGN_PLONE_IOPRENOTO_INTEGRATION_TESTING
 
     def setUp(self):
         """Custom shared utility setup for tests."""
         self.portal = self.layer["portal"]
+        self.request = self.layer["request"]
+
+        setRoles(self.portal, TEST_USER_ID, ["Manager"])
+
+        self.prenotazioni_folder = api.content.create(
+            type="PrenotazioniFolder",
+            title="Prenotazioni Folder",
+            container=self.portal,
+        )
 
     def test_behaviors_enabled_for_persona(self):
         """Test that PrenotazioniFolder has all the behaviors
         assigned by this product
         """
         portal_types = api.portal.get_tool(name="portal_types")
 
-        for behavior in (
-            "design.plone.ioprenoto.behaviors.uffici_correlati",
-            "design.plone.ioprenoto.behaviors.punto_di_contatto",
-            "design.plone.ioprenoto.behaviors.orario_di_apertura",
-        ):
+        for behavior in ("design.plone.ioprenoto.behaviors.additional_fields",):
             self.assertIn(behavior, portal_types["PrenotazioniFolder"].behaviors)
+
+    def test_exclude_from_nav(self):
+        self.assertTrue(self.prenotazioni_folder.exclude_from_nav)
```

### Comparing `design.plone.ioprenoto-1.0.1/src/design/plone/ioprenoto/tests/test_restapi_serializers_ovverrides_prenotazioni_folder.py` & `design.plone.ioprenoto-1.0.2/src/design/plone/ioprenoto/tests/test_restapi_serializers_ovverrides_prenotazioni_folder.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,9 @@
 # -*- coding: utf-8 -*-
-from design.plone.ioprenoto.testing import (
-    DESIGN_PLONE_IOPRENOTO_API_FUNCTIONAL_TESTING,
-)
+from design.plone.ioprenoto.testing import DESIGN_PLONE_IOPRENOTO_API_FUNCTIONAL_TESTING
 from plone import api
 from plone.app.testing import setRoles
 from plone.app.testing import SITE_OWNER_NAME
 from plone.app.testing import SITE_OWNER_PASSWORD
 from plone.app.testing import TEST_USER_ID
 from plone.app.testing import TEST_USER_NAME
 from plone.app.testing import TEST_USER_PASSWORD
```

### Comparing `design.plone.ioprenoto-1.0.1/src/design/plone/ioprenoto/tests/test_restapi_serializers_ovverrides_serzvizio.py` & `design.plone.ioprenoto-1.0.2/src/design/plone/ioprenoto/tests/test_restapi_serializers_ovverrides_serzvizio.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,11 +1,9 @@
 # -*- coding: utf-8 -*-
-from design.plone.ioprenoto.testing import (
-    DESIGN_PLONE_IOPRENOTO_API_FUNCTIONAL_TESTING,
-)
+from design.plone.ioprenoto.testing import DESIGN_PLONE_IOPRENOTO_API_FUNCTIONAL_TESTING
 from plone import api
 from plone.app.testing import setRoles
 from plone.app.testing import SITE_OWNER_NAME
 from plone.app.testing import SITE_OWNER_PASSWORD
 from plone.app.testing import TEST_USER_ID
 from plone.restapi.testing import RelativeSession
 from transaction import commit
```

### Comparing `design.plone.ioprenoto-1.0.1/src/design/plone/ioprenoto/tests/test_setup.py` & `design.plone.ioprenoto-1.0.2/src/design/plone/ioprenoto/tests/test_setup.py`

 * *Files 14% similar despite different names*

```diff
@@ -31,17 +31,15 @@
 
     def test_product_installed(self):
         """Test if design.plone.ioprenoto is installed."""
         self.assertTrue(self.installer.is_product_installed("design.plone.ioprenoto"))
 
     def test_browserlayer(self):
         """Test that IDesignPloneIoprenotoLayer is registered."""
-        from design.plone.ioprenoto.interfaces import (
-            IDesignPloneIoprenotoLayer,
-        )
+        from design.plone.ioprenoto.interfaces import IDesignPloneIoprenotoLayer
         from plone.browserlayer import utils
 
         self.assertIn(IDesignPloneIoprenotoLayer, utils.registered_layers())
 
 
 class TestUninstall(unittest.TestCase):
     layer = DESIGN_PLONE_IOPRENOTO_INTEGRATION_TESTING
@@ -59,13 +57,11 @@
 
     def test_product_uninstalled(self):
         """Test if design.plone.ioprenoto is cleanly uninstalled."""
         self.assertFalse(self.installer.is_product_installed("design.plone.ioprenoto"))
 
     def test_browserlayer_removed(self):
         """Test that IDesignPloneIoprenotoLayer is removed."""
-        from design.plone.ioprenoto.interfaces import (
-            IDesignPloneIoprenotoLayer,
-        )
+        from design.plone.ioprenoto.interfaces import IDesignPloneIoprenotoLayer
         from plone.browserlayer import utils
 
         self.assertNotIn(IDesignPloneIoprenotoLayer, utils.registered_layers())
```

### Comparing `design.plone.ioprenoto-1.0.1/src/design.plone.ioprenoto.egg-info/SOURCES.txt` & `design.plone.ioprenoto-1.0.2/src/design.plone.ioprenoto.egg-info/SOURCES.txt`

 * *Files 12% similar despite different names*

```diff
@@ -21,23 +21,27 @@
 src/design/plone/__init__.py
 src/design/plone/ioprenoto/__init__.py
 src/design/plone/ioprenoto/configure.zcml
 src/design/plone/ioprenoto/interfaces.py
 src/design/plone/ioprenoto/permissions.zcml
 src/design/plone/ioprenoto/setuphandlers.py
 src/design/plone/ioprenoto/testing.py
+src/design/plone/ioprenoto/adapters/__init__.py
+src/design/plone/ioprenoto/adapters/configure.zcml
+src/design/plone/ioprenoto/adapters/stringinterp.py
 src/design/plone/ioprenoto/behaviors/__init__.py
+src/design/plone/ioprenoto/behaviors/additional_fields.py
 src/design/plone/ioprenoto/behaviors/configure.zcml
-src/design/plone/ioprenoto/behaviors/orario_di_apertura.py
-src/design/plone/ioprenoto/behaviors/punto_di_contatto.py
-src/design/plone/ioprenoto/behaviors/uffici_correlati.py
 src/design/plone/ioprenoto/browser/__init__.py
 src/design/plone/ioprenoto/browser/configure.zcml
 src/design/plone/ioprenoto/browser/overrides/.gitkeep
 src/design/plone/ioprenoto/browser/static/.gitkeep
+src/design/plone/ioprenoto/events/__init__.py
+src/design/plone/ioprenoto/events/configure.zcml
+src/design/plone/ioprenoto/events/on_create.py
 src/design/plone/ioprenoto/locales/README.rst
 src/design/plone/ioprenoto/locales/__init__.py
 src/design/plone/ioprenoto/locales/design.plone.ioprenoto.pot
 src/design/plone/ioprenoto/locales/update.py
 src/design/plone/ioprenoto/locales/update.sh
 src/design/plone/ioprenoto/locales/en/LC_MESSAGES/design.plone.ioprenoto.po
 src/design/plone/ioprenoto/profiles/default/browserlayer.xml
@@ -51,14 +55,18 @@
 src/design/plone/ioprenoto/restapi/configure.zcml
 src/design/plone/ioprenoto/restapi/serializers/__init__.py
 src/design/plone/ioprenoto/restapi/serializers/configure.zcml
 src/design/plone/ioprenoto/restapi/serializers/ovverrides/__init__.py
 src/design/plone/ioprenoto/restapi/serializers/ovverrides/configure.zcml
 src/design/plone/ioprenoto/restapi/serializers/ovverrides/prenotazioniFolder.py
 src/design/plone/ioprenoto/restapi/serializers/ovverrides/servizio.py
+src/design/plone/ioprenoto/restapi/services/configure.zcml
+src/design/plone/ioprenoto/restapi/services/bookable_list/configure.zcml
+src/design/plone/ioprenoto/restapi/services/bookable_list/get.py
 src/design/plone/ioprenoto/tests/__init__.py
 src/design/plone/ioprenoto/tests/test_PrenotazioniFolder_ct.py
 src/design/plone/ioprenoto/tests/test_restapi_serializers_ovverrides_prenotazioni_folder.py
 src/design/plone/ioprenoto/tests/test_restapi_serializers_ovverrides_serzvizio.py
-src/design/plone/ioprenoto/tests/test_robot.py
+src/design/plone/ioprenoto/tests/test_restapi_service_bookable_uo_list.py
 src/design/plone/ioprenoto/tests/test_setup.py
+src/design/plone/ioprenoto/tests/test_stringinterp_overrides.py
 src/design/plone/ioprenoto/tests/robot/test_example.robot
```

