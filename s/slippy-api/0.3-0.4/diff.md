# Comparing `tmp/slippy_api-0.3.tar.gz` & `tmp/slippy_api-0.4-py3-none-any.whl.zip`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "slippy_api-0.3.tar", last modified: Wed May  3 21:51:38 2023, max compression
+Zip archive data, at least v2.0 to extract, compression method=deflate
```

## filetype from diffoscope

```diff
@@ -1 +1 @@
-GzipFile
+ZipFile
```

