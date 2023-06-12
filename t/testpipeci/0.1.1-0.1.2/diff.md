# Comparing `tmp/testpipeci-0.1.1.tar.gz` & `tmp/testpipeci-0.1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "testpipeci-0.1.1.tar", max compression
+gzip compressed data, was "testpipeci-0.1.2.tar", max compression
```

## Comparing `testpipeci-0.1.1.tar` & `testpipeci-0.1.2.tar`

### file list

```diff
@@ -1,5 +1,5 @@
--rw-r--r--   0        0        0        0 2023-06-12 02:28:16.536723 testpipeci-0.1.1/README.md
--rw-r--r--   0        0        0      404 2023-06-12 02:28:33.728736 testpipeci-0.1.1/pyproject.toml
--rw-r--r--   0        0        0        0 2023-06-12 02:28:16.536723 testpipeci-0.1.1/testpipeci/__init__.py
--rw-r--r--   0        0        0      122 2023-06-12 02:28:16.536723 testpipeci-0.1.1/testpipeci/cli.py
--rw-r--r--   0        0        0      381 1970-01-01 00:00:00.000000 testpipeci-0.1.1/PKG-INFO
+-rw-r--r--   0        0        0        0 2023-06-12 11:01:54.246711 testpipeci-0.1.2/README.md
+-rw-r--r--   0        0        0      404 2023-06-12 11:02:06.970697 testpipeci-0.1.2/pyproject.toml
+-rw-r--r--   0        0        0        0 2023-06-12 11:01:54.246711 testpipeci-0.1.2/testpipeci/__init__.py
+-rw-r--r--   0        0        0      122 2023-06-12 11:01:54.246711 testpipeci-0.1.2/testpipeci/cli.py
+-rw-r--r--   0        0        0      381 1970-01-01 00:00:00.000000 testpipeci-0.1.2/PKG-INFO
```

