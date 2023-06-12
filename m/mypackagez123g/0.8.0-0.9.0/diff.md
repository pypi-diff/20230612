# Comparing `tmp/mypackagez123g-0.8.0.tar.gz` & `tmp/mypackagez123g-0.9.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mypackagez123g-0.8.0.tar", max compression
+gzip compressed data, was "mypackagez123g-0.9.0.tar", max compression
```

## Comparing `mypackagez123g-0.8.0.tar` & `mypackagez123g-0.9.0.tar`

### file list

```diff
@@ -1,4 +1,4 @@
--rw-r--r--   0        0        0        0 2023-06-12 21:14:01.709521 mypackagez123g-0.8.0/README.md
--rw-r--r--   0        0        0        0 2023-06-12 21:14:01.709521 mypackagez123g-0.8.0/mypackagez123g/__init__.py
--rw-r--r--   0        0        0      267 2023-06-12 21:14:16.757695 mypackagez123g-0.8.0/pyproject.toml
--rw-r--r--   0        0        0      436 1970-01-01 00:00:00.000000 mypackagez123g-0.8.0/PKG-INFO
+-rw-r--r--   0        0        0        0 2023-06-12 21:21:05.891860 mypackagez123g-0.9.0/README.md
+-rw-r--r--   0        0        0        0 2023-06-12 21:21:05.891860 mypackagez123g-0.9.0/mypackagez123g/__init__.py
+-rw-r--r--   0        0        0      267 2023-06-12 21:21:25.204142 mypackagez123g-0.9.0/pyproject.toml
+-rw-r--r--   0        0        0      436 1970-01-01 00:00:00.000000 mypackagez123g-0.9.0/PKG-INFO
```

