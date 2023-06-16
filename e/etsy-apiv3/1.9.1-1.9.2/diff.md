# Comparing `tmp/etsy-apiv3-1.9.1.tar.gz` & `tmp/etsy_apiv3-1.9.2-py3-none-any.whl.zip`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "etsy-apiv3-1.9.1.tar", last modified: Wed May 31 13:58:47 2023, max compression
+Zip archive data, at least v2.0 to extract, compression method=deflate
```

## filetype from diffoscope

```diff
@@ -1 +1 @@
-GzipFile
+ZipFile
```

