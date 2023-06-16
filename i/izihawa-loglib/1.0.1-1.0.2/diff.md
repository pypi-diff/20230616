# Comparing `tmp/izihawa_loglib-1.0.1-py3-none-any.whl.zip` & `tmp/izihawa_loglib-1.0.2-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,8 +1,8 @@
-Zip file size: 3036 bytes, number of entries: 6
--rw-r--r--  2.0 unx      999 b- defN 23-May-04 16:11 izihawa_loglib/__init__.py
+Zip file size: 3050 bytes, number of entries: 6
+-rw-r--r--  2.0 unx     1028 b- defN 23-Jun-16 16:57 izihawa_loglib/__init__.py
 -rw-r--r--  2.0 unx     2750 b- defN 22-Oct-25 09:23 izihawa_loglib/formatters.py
 -rw-r--r--  2.0 unx     1073 b- defN 22-Oct-25 09:23 izihawa_loglib/handlers.py
-?rw-------  2.0 unx       91 b- defN 23-May-24 12:41 izihawa_loglib-1.0.1.dist-info/WHEEL
-?rw-------  2.0 unx      358 b- defN 23-May-24 12:41 izihawa_loglib-1.0.1.dist-info/METADATA
-?rw-------  2.0 unx      476 b- defN 23-May-24 12:41 izihawa_loglib-1.0.1.dist-info/RECORD
-6 files, 5747 bytes uncompressed, 2174 bytes compressed:  62.2%
+?rw-------  2.0 unx       91 b- defN 23-Jun-16 16:59 izihawa_loglib-1.0.2.dist-info/WHEEL
+?rw-------  2.0 unx      358 b- defN 23-Jun-16 16:59 izihawa_loglib-1.0.2.dist-info/METADATA
+?rw-------  2.0 unx      477 b- defN 23-Jun-16 16:59 izihawa_loglib-1.0.2.dist-info/RECORD
+6 files, 5777 bytes uncompressed, 2188 bytes compressed:  62.1%
```

## zipnote {}

```diff
@@ -3,17 +3,17 @@
 
 Filename: izihawa_loglib/formatters.py
 Comment: 
 
 Filename: izihawa_loglib/handlers.py
 Comment: 
 
-Filename: izihawa_loglib-1.0.1.dist-info/WHEEL
+Filename: izihawa_loglib-1.0.2.dist-info/WHEEL
 Comment: 
 
-Filename: izihawa_loglib-1.0.1.dist-info/METADATA
+Filename: izihawa_loglib-1.0.2.dist-info/METADATA
 Comment: 
 
-Filename: izihawa_loglib-1.0.1.dist-info/RECORD
+Filename: izihawa_loglib-1.0.2.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## izihawa_loglib/__init__.py

```diff
@@ -5,17 +5,17 @@
 from izihawa_utils.exceptions import BaseError
 from izihawa_utils.file import mkdir_p
 
 from .formatters import DefaultFormatter, DefaultHttpFormatter
 from .handlers import QueueHandler
 
 
-def configure_logging(config, make_path=True):
+def configure_logging(config, make_path=True, default_level=logging.INFO):
     if config.get('application', {}).get('debug', False) or 'logging' not in config:
-        logging.basicConfig(stream=sys.stdout, level=logging.INFO)
+        logging.basicConfig(stream=sys.stdout, level=default_level)
     else:
         if make_path:
             mkdir_p(config['log_path'])
         logging.config.dictConfig(config['logging'])
 
 
 def error_log(e, level=logging.ERROR, **fields):
```

