# Comparing `tmp/pmr2.wfctrl-0.2.tar.gz` & `tmp/pmr2.wfctrl-0.4.0.zip`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/pmr2.wfctrl-0.2.tar", last modified: Mon Jul 14 02:48:18 2014, max compression
+Zip archive data, at least v2.0 to extract, compression method=store
```

## filetype from diffoscope

```diff
@@ -1 +1 @@
-GzipFile
+ZipFile
```

