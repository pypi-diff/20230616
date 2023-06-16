# Comparing `tmp/gpboost-1.2.0.tar.gz` & `tmp/gpboost-1.2.1-py3-none-macosx_10_9_x86_64.whl.zip`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "gpboost-1.2.0.tar", last modified: Sat Jun 10 06:14:35 2023, max compression
+Zip archive data, at least v2.0 to extract, compression method=deflate
```

## filetype from diffoscope

```diff
@@ -1 +1 @@
-GzipFile
+ZipFile
```

