# Comparing `tmp/openai-ratelimiter-0.1.tar.gz` & `tmp/openai_ratelimiter-0.2-py3-none-any.whl.zip`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "openai-ratelimiter-0.1.tar", last modified: Wed Jun 14 18:46:22 2023, max compression
+Zip archive data, at least v2.0 to extract, compression method=deflate
```

## filetype from diffoscope

```diff
@@ -1 +1 @@
-GzipFile
+ZipFile
```

