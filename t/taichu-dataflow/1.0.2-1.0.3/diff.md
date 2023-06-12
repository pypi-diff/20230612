# Comparing `tmp/taichu-dataflow-1.0.2.tar.gz` & `tmp/taichu_dataflow-1.0.3-py3-none-any.whl.zip`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "taichu-dataflow-1.0.2.tar", last modified: Mon Jun 12 06:26:23 2023, max compression
+Zip archive data, at least v2.0 to extract, compression method=deflate
```

## filetype from diffoscope

```diff
@@ -1 +1 @@
-GzipFile
+ZipFile
```

