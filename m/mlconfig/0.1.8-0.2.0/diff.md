# Comparing `tmp/mlconfig-0.1.8-py3-none-any.whl.zip` & `tmp/mlconfig-0.2.0-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,11 +1,9 @@
-Zip file size: 5547 bytes, number of entries: 9
--rw-r--r--  2.0 unx      151 b- defN 80-Jan-01 00:00 mlconfig/__init__.py
--rw-r--r--  2.0 unx     2046 b- defN 80-Jan-01 00:00 mlconfig/collections.py
--rw-r--r--  2.0 unx     5363 b- defN 80-Jan-01 00:00 mlconfig/config.py
--rw-r--r--  2.0 unx      790 b- defN 80-Jan-01 00:00 mlconfig/torch/__init__.py
--rw-r--r--  2.0 unx     1283 b- defN 80-Jan-01 00:00 mlconfig/utils.py
--rw-r--r--  2.0 unx     1066 b- defN 80-Jan-01 00:00 mlconfig-0.1.8.dist-info/LICENSE
-?rw-r--r--  2.0 unx       88 b- defN 16-Jan-01 00:00 mlconfig-0.1.8.dist-info/WHEEL
-?rw-r--r--  2.0 unx      521 b- defN 16-Jan-01 00:00 mlconfig-0.1.8.dist-info/METADATA
-?rw-r--r--  2.0 unx      684 b- defN 16-Jan-01 00:00 mlconfig-0.1.8.dist-info/RECORD
-9 files, 11992 bytes uncompressed, 4381 bytes compressed:  63.5%
+Zip file size: 3412 bytes, number of entries: 7
+-rw-r--r--  2.0 unx      105 b- defN 80-Jan-01 00:00 mlconfig/__init__.py
+-rw-r--r--  2.0 unx     1961 b- defN 80-Jan-01 00:00 mlconfig/conf.py
+-rw-r--r--  2.0 unx     1001 b- defN 80-Jan-01 00:00 mlconfig/torch/__init__.py
+-rw-r--r--  2.0 unx     1066 b- defN 80-Jan-01 00:00 mlconfig-0.2.0.dist-info/LICENSE
+-rw-r--r--  2.0 unx      457 b- defN 80-Jan-01 00:00 mlconfig-0.2.0.dist-info/METADATA
+-rw-r--r--  2.0 unx       88 b- defN 80-Jan-01 00:00 mlconfig-0.2.0.dist-info/WHEEL
+?rw-r--r--  2.0 unx      529 b- defN 16-Jan-01 00:00 mlconfig-0.2.0.dist-info/RECORD
+7 files, 5207 bytes uncompressed, 2482 bytes compressed:  52.3%
```

## zipnote {}

```diff
@@ -1,28 +1,22 @@
 Filename: mlconfig/__init__.py
 Comment: 
 
-Filename: mlconfig/collections.py
-Comment: 
-
-Filename: mlconfig/config.py
+Filename: mlconfig/conf.py
 Comment: 
 
 Filename: mlconfig/torch/__init__.py
 Comment: 
 
-Filename: mlconfig/utils.py
-Comment: 
-
-Filename: mlconfig-0.1.8.dist-info/LICENSE
+Filename: mlconfig-0.2.0.dist-info/LICENSE
 Comment: 
 
-Filename: mlconfig-0.1.8.dist-info/WHEEL
+Filename: mlconfig-0.2.0.dist-info/METADATA
 Comment: 
 
-Filename: mlconfig-0.1.8.dist-info/METADATA
+Filename: mlconfig-0.2.0.dist-info/WHEEL
 Comment: 
 
-Filename: mlconfig-0.1.8.dist-info/RECORD
+Filename: mlconfig-0.2.0.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## mlconfig/__init__.py

```diff
@@ -1,5 +1,4 @@
-from .config import Config
-from .config import getcls
-from .config import load
-from .config import register
-from .config import set_key_of_func_or_cls
+from .conf import getcls
+from .conf import instantiate
+from .conf import load
+from .conf import register
```

## mlconfig/torch/__init__.py

```diff
@@ -15,21 +15,27 @@
         if isinstance(attr, type) and issubclass(attr, superclass):
             if attr is superclass:
                 continue
 
             if prefix is not None:
                 name = prefix + sep + name
 
-            mlconfig.register(attr, name=name)
+            mlconfig.conf(attr, name=name)
+
+
+def get_lr_scheduler_class():
+    # PyTorch 2.0 renamed LRScheduler to _LRScheduler
+    name = 'LRScheduler' if hasattr(optim.lr_scheduler, 'LRScheduler') else '_LRScheduler'
+    return getattr(optim.lr_scheduler, name)
 
 
 register_torch_optimizers = functools.partial(
     _register_classes,
     module=optim,
     superclass=optim.Optimizer,
 )
 
 register_torch_schedulers = functools.partial(
     _register_classes,
     module=optim.lr_scheduler,
-    superclass=optim.lr_scheduler._LRScheduler,
+    superclass=get_lr_scheduler_class(),
 )
```

## Comparing `mlconfig-0.1.8.dist-info/LICENSE` & `mlconfig-0.2.0.dist-info/LICENSE`

 * *Files identical despite different names*

