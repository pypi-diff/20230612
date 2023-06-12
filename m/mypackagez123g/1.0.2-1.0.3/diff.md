# Comparing `tmp/mypackagez123g-1.0.2.tar.gz` & `tmp/mypackagez123g-1.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mypackagez123g-1.0.2.tar", max compression
+gzip compressed data, was "mypackagez123g-1.0.3.tar", max compression
```

## Comparing `mypackagez123g-1.0.2.tar` & `mypackagez123g-1.0.3.tar`

### file list

```diff
@@ -1,4 +1,4 @@
--rw-r--r--   0        0        0        0 2023-06-12 21:44:39.248168 mypackagez123g-1.0.2/README.md
--rw-r--r--   0        0        0        0 2023-06-12 21:44:39.248168 mypackagez123g-1.0.2/mypackagez123g/__init__.py
--rw-r--r--   0        0        0      267 2023-06-12 21:45:02.492222 mypackagez123g-1.0.2/pyproject.toml
--rw-r--r--   0        0        0      436 1970-01-01 00:00:00.000000 mypackagez123g-1.0.2/PKG-INFO
+-rw-r--r--   0        0        0        0 2023-06-12 21:50:59.673174 mypackagez123g-1.0.3/README.md
+-rw-r--r--   0        0        0        0 2023-06-12 21:50:59.673174 mypackagez123g-1.0.3/mypackagez123g/__init__.py
+-rw-r--r--   0        0        0      267 2023-06-12 21:51:13.341523 mypackagez123g-1.0.3/pyproject.toml
+-rw-r--r--   0        0        0      436 1970-01-01 00:00:00.000000 mypackagez123g-1.0.3/PKG-INFO
```

