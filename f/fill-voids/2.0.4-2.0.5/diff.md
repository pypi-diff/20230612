# Comparing `tmp/fill_voids-2.0.4.tar.gz` & `tmp/fill_voids-2.0.5-pp39-pypy39_pp73-win_amd64.whl.zip`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "fill_voids-2.0.4.tar", last modified: Sat May  6 04:27:03 2023, max compression
+Zip archive data, at least v2.0 to extract, compression method=deflate
```

## filetype from diffoscope

```diff
@@ -1 +1 @@
-GzipFile
+ZipFile
```

