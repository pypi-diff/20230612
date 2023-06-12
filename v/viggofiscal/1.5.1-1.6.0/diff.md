# Comparing `tmp/viggofiscal-1.5.1.tar.gz` & `tmp/viggofiscal-1.6.0-py3-none-any.whl.zip`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "viggofiscal-1.5.1.tar", last modified: Tue Jun  6 12:18:18 2023, max compression
+Zip archive data, at least v2.0 to extract, compression method=deflate
```

## filetype from diffoscope

```diff
@@ -1 +1 @@
-GzipFile
+ZipFile
```

