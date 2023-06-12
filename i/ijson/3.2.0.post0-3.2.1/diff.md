# Comparing `tmp/ijson-3.2.0.post0.tar.gz` & `tmp/ijson-3.2.1-pp37-pypy37_pp73-macosx_10_9_x86_64.whl.zip`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/ijson-3.2.0.post0.tar", last modified: Wed Jan  4 00:14:03 2023, max compression
+Zip archive data, at least v2.0 to extract, compression method=deflate
```

## filetype from diffoscope

```diff
@@ -1 +1 @@
-GzipFile
+ZipFile
```

