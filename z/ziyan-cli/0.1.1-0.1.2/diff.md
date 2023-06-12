# Comparing `tmp/ziyan_cli-0.1.1.tar.gz` & `tmp/ziyan_cli-0.1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ziyan_cli-0.1.1.tar", max compression
+gzip compressed data, was "ziyan_cli-0.1.2.tar", max compression
```

## Comparing `ziyan_cli-0.1.1.tar` & `ziyan_cli-0.1.2.tar`

### file list

```diff
@@ -1,4 +1,4 @@
--rw-r--r--   0        0        0      298 2023-06-12 02:26:18.024347 ziyan_cli-0.1.1/pyproject.toml
--rw-r--r--   0        0        0     1228 2023-06-12 02:22:52.722636 ziyan_cli-0.1.1/ziyan_cli/__init__.py
--rw-r--r--   0        0        0      495 2023-06-12 02:26:27.484438 ziyan_cli-0.1.1/setup.py
--rw-r--r--   0        0        0      242 2023-06-12 02:26:27.484703 ziyan_cli-0.1.1/PKG-INFO
+-rw-r--r--   0        0        0      298 2023-06-12 03:32:39.804762 ziyan_cli-0.1.2/pyproject.toml
+-rw-r--r--   0        0        0     1614 2023-06-12 03:31:06.091509 ziyan_cli-0.1.2/ziyan_cli/__init__.py
+-rw-r--r--   0        0        0      495 2023-06-12 03:32:42.458207 ziyan_cli-0.1.2/setup.py
+-rw-r--r--   0        0        0      242 2023-06-12 03:32:42.458472 ziyan_cli-0.1.2/PKG-INFO
```

