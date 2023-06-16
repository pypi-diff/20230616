# Comparing `tmp/datarangers-sdk-python-1.0.5.tar.gz` & `tmp/datarangers_sdk_python-1.1.1-py3-none-any.whl.zip`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "datarangers-sdk-python-1.0.5.tar", last modified: Wed May 12 02:16:18 2021, max compression
+Zip archive data, at least v2.0 to extract, compression method=deflate
```

## filetype from diffoscope

```diff
@@ -1 +1 @@
-GzipFile
+ZipFile
```

