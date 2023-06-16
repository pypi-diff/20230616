# Comparing `tmp/sinricpro-2.7.1.tar.gz` & `tmp/sinricpro-2.7.2-py3-none-any.whl.zip`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "sinricpro-2.7.1.tar", last modified: Sat Jun 10 16:09:20 2023, max compression
+Zip archive data, at least v2.0 to extract, compression method=deflate
```

## filetype from diffoscope

```diff
@@ -1 +1 @@
-GzipFile
+ZipFile
```

