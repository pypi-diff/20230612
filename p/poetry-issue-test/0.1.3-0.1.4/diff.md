# Comparing `tmp/poetry_issue_test-0.1.3.tar.gz` & `tmp/poetry_issue_test-0.1.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "poetry_issue_test-0.1.3.tar", max compression
+gzip compressed data, was "poetry_issue_test-0.1.4.tar", max compression
```

## Comparing `poetry_issue_test-0.1.3.tar` & `poetry_issue_test-0.1.4.tar`

### file list

```diff
@@ -1,5 +1,5 @@
--rw-r--r--   0        0        0    11357 2023-06-12 10:38:36.662892 poetry_issue_test-0.1.3/LICENSE
--rw-r--r--   0        0        0        0 2023-06-12 10:25:39.552911 poetry_issue_test-0.1.3/README.md
--rw-r--r--   0        0        0        0 2023-06-12 10:25:12.826245 poetry_issue_test-0.1.3/poetry_test/__init__.py
--rw-r--r--   0        0        0      501 2023-06-12 12:48:33.723215 poetry_issue_test-0.1.3/pyproject.toml
--rw-r--r--   0        0        0      464 1970-01-01 00:00:00.000000 poetry_issue_test-0.1.3/PKG-INFO
+-rw-r--r--   0        0        0    11357 2023-06-12 10:38:36.662892 poetry_issue_test-0.1.4/LICENSE
+-rw-r--r--   0        0        0        0 2023-06-12 10:25:39.552911 poetry_issue_test-0.1.4/README.md
+-rw-r--r--   0        0        0        0 2023-06-12 10:25:12.826245 poetry_issue_test-0.1.4/poetry_test/__init__.py
+-rw-r--r--   0        0        0      502 2023-06-12 12:49:46.909880 poetry_issue_test-0.1.4/pyproject.toml
+-rw-r--r--   0        0        0      464 1970-01-01 00:00:00.000000 poetry_issue_test-0.1.4/PKG-INFO
```

### Comparing `poetry_issue_test-0.1.3/LICENSE` & `poetry_issue_test-0.1.4/LICENSE`

 * *Files identical despite different names*

