# Comparing `tmp/validio_cli-0.0.1.tar.gz` & `tmp/validio_cli-0.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "validio_cli-0.0.1.tar", max compression
+gzip compressed data, was "validio_cli-0.1.0.tar", max compression
```

## Comparing `validio_cli-0.0.1.tar` & `validio_cli-0.1.0.tar`

### file list

```diff
@@ -1,4 +1,20 @@
--rw-r--r--   0        0        0    11340 2023-05-04 06:18:28.957608 validio_cli-0.0.1/LICENSE
--rw-r--r--   0        0        0      883 2023-05-05 14:53:08.012149 validio_cli-0.0.1/pyproject.toml
--rw-r--r--   0        0        0        0 2023-05-04 06:18:28.958418 validio_cli-0.0.1/validio_cli/__init__.py
--rw-r--r--   0        0        0      506 1970-01-01 00:00:00.000000 validio_cli-0.0.1/PKG-INFO
+-rw-r--r--   0        0        0    11340 2023-06-12 09:21:56.805572 validio_cli-0.1.0/LICENSE
+-rw-r--r--   0        0        0     1738 2023-06-12 09:22:07.597616 validio_cli-0.1.0/pyproject.toml
+-rw-r--r--   0        0        0     5347 2023-06-12 09:21:56.805572 validio_cli-0.1.0/validio_cli/__init__.py
+-rw-r--r--   0        0        0     1327 2023-06-12 09:21:56.805572 validio_cli-0.1.0/validio_cli/bin/entities/channels.py
+-rw-r--r--   0        0        0    11656 2023-06-12 09:21:56.805572 validio_cli-0.1.0/validio_cli/bin/entities/code.py
+-rw-r--r--   0        0        0     3897 2023-06-12 09:21:56.805572 validio_cli-0.1.0/validio_cli/bin/entities/config.py
+-rw-r--r--   0        0        0     1171 2023-06-12 09:21:56.805572 validio_cli-0.1.0/validio_cli/bin/entities/credentials.py
+-rw-r--r--   0        0        0     1176 2023-06-12 09:21:56.805572 validio_cli-0.1.0/validio_cli/bin/entities/destinations.py
+-rw-r--r--   0        0        0     1716 2023-06-12 09:21:56.805572 validio_cli-0.1.0/validio_cli/bin/entities/notification_rules.py
+-rw-r--r--   0        0        0     3110 2023-06-12 09:21:56.805572 validio_cli-0.1.0/validio_cli/bin/entities/recommendations.py
+-rw-r--r--   0        0        0     1726 2023-06-12 09:21:56.805572 validio_cli-0.1.0/validio_cli/bin/entities/segmentations.py
+-rw-r--r--   0        0        0    25068 2023-06-12 09:21:56.805572 validio_cli-0.1.0/validio_cli/bin/entities/sources.py
+-rw-r--r--   0        0        0     1174 2023-06-12 09:21:56.805572 validio_cli-0.1.0/validio_cli/bin/entities/users.py
+-rw-r--r--   0        0        0     2470 2023-06-12 09:21:56.805572 validio_cli-0.1.0/validio_cli/bin/entities/validators.py
+-rw-r--r--   0        0        0     1686 2023-06-12 09:21:56.805572 validio_cli-0.1.0/validio_cli/bin/entities/windows.py
+-rw-r--r--   0        0        0     2747 2023-06-12 09:21:56.805572 validio_cli-0.1.0/validio_cli/bin/main.py
+-rw-r--r--   0        0        0     2587 2023-06-12 09:21:56.805572 validio_cli-0.1.0/validio_cli/components.py
+-rw-r--r--   0        0        0      265 2023-06-12 09:21:56.805572 validio_cli-0.1.0/validio_cli/metadata.py
+-rw-r--r--   0        0        0     1382 2023-06-12 09:21:56.805572 validio_cli-0.1.0/validio_cli/schema.py
+-rw-r--r--   0        0        0      847 1970-01-01 00:00:00.000000 validio_cli-0.1.0/PKG-INFO
```

### Comparing `validio_cli-0.0.1/LICENSE` & `validio_cli-0.1.0/LICENSE`

 * *Files identical despite different names*

