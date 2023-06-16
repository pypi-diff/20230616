# Comparing `tmp/PenguLogger-0.1.tar.gz` & `tmp/PenguLogger-0.1.1-py3-none-any.whl.zip`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "PenguLogger-0.1.tar", last modified: Fri Jun 16 01:47:54 2023, max compression
+Zip archive data, at least v2.0 to extract, compression method=deflate
```

## filetype from diffoscope

```diff
@@ -1 +1 @@
-GzipFile
+ZipFile
```

