# Comparing `tmp/pybuildkite-1.2.2.tar.gz` & `tmp/pybuildkite-1.2.3-py3-none-any.whl.zip`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/pybuildkite-1.2.2.tar", last modified: Tue Dec 20 19:50:18 2022, max compression
+Zip archive data, at least v2.0 to extract, compression method=deflate
```

## filetype from diffoscope

```diff
@@ -1 +1 @@
-GzipFile
+ZipFile
```

