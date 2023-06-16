# Comparing `tmp/yunopyutils-1.0.0a1.tar.gz` & `tmp/yunopyutils-1.0.0a2.tar.gz`

## Comparing `yunopyutils-1.0.0a1.tar` & `yunopyutils-1.0.0a2.tar`

### file list

```diff
@@ -1,10 +1,8 @@
--rw-r--r--   0        0        0     6148 2020-02-02 00:00:00.000000 yunopyutils-1.0.0a1/.DS_Store
--rw-r--r--   0        0        0      106 2020-02-02 00:00:00.000000 yunopyutils-1.0.0a1/.flake8
--rw-r--r--   0        0        0      222 2020-02-02 00:00:00.000000 yunopyutils-1.0.0a1/.pypirc
--rw-r--r--   0        0        0     4824 2020-02-02 00:00:00.000000 yunopyutils-1.0.0a1/pdm.lock
--rw-r--r--   0        0        0       57 2020-02-02 00:00:00.000000 yunopyutils-1.0.0a1/yunopyutils/__init__.py
--rwxr-xr-x   0        0        0     3206 2020-02-02 00:00:00.000000 yunopyutils-1.0.0a1/yunopyutils/logger/create_log.py
--rw-r--r--   0        0        0     3090 2020-02-02 00:00:00.000000 yunopyutils-1.0.0a1/.gitignore
--rw-r--r--   0        0        0       34 2020-02-02 00:00:00.000000 yunopyutils-1.0.0a1/README.md
--rw-r--r--   0        0        0      474 2020-02-02 00:00:00.000000 yunopyutils-1.0.0a1/pyproject.toml
--rw-r--r--   0        0        0      276 2020-02-02 00:00:00.000000 yunopyutils-1.0.0a1/PKG-INFO
+-rw-r--r--   0        0        0      106 2020-02-02 00:00:00.000000 yunopyutils-1.0.0a2/.flake8
+-rw-r--r--   0        0        0     4824 2020-02-02 00:00:00.000000 yunopyutils-1.0.0a2/pdm.lock
+-rw-r--r--   0        0        0       67 2020-02-02 00:00:00.000000 yunopyutils-1.0.0a2/yunopyutils/__init__.py
+-rwxr-xr-x   0        0        0     3214 2020-02-02 00:00:00.000000 yunopyutils-1.0.0a2/yunopyutils/logger/create_log.py
+-rw-r--r--   0        0        0     3121 2020-02-02 00:00:00.000000 yunopyutils-1.0.0a2/.gitignore
+-rw-r--r--   0        0        0      437 2020-02-02 00:00:00.000000 yunopyutils-1.0.0a2/README.md
+-rw-r--r--   0        0        0      550 2020-02-02 00:00:00.000000 yunopyutils-1.0.0a2/pyproject.toml
+-rw-r--r--   0        0        0      749 2020-02-02 00:00:00.000000 yunopyutils-1.0.0a2/PKG-INFO
```

### Comparing `yunopyutils-1.0.0a1/pdm.lock` & `yunopyutils-1.0.0a2/pdm.lock`

 * *Files identical despite different names*

### Comparing `yunopyutils-1.0.0a1/yunopyutils/logger/create_log.py` & `yunopyutils-1.0.0a2/yunopyutils/logger/create_log.py`

 * *Files 1% similar despite different names*

```diff
@@ -66,15 +66,15 @@
 
         if record.stack_info:
             message_dict["stack"] = self.formatStack(record.stack_info)
 
         return dumps(message_dict, default=str)
 
 
-def init(module, formatter: dict = _DEFAULT_FOMATTER):
+def build_logger(module, formatter: dict = _DEFAULT_FOMATTER):
     logger = getLogger(module)
     if _LOG_LEVEL == "debug":
         logger.setLevel(DEBUG)
     elif _LOG_LEVEL == "info":
         logger.setLevel(INFO)
     else:
         logger.setLevel(WARNING)
```

### Comparing `yunopyutils-1.0.0a1/.gitignore` & `yunopyutils-1.0.0a2/.gitignore`

 * *Files 5% similar despite different names*

```diff
@@ -155,7 +155,12 @@
 # PyCharm
 #  JetBrains specific template is maintained in a separate JetBrains.gitignore that can
 #  be found at https://github.com/github/gitignore/blob/main/Global/JetBrains.gitignore
 #  and can be added to the global gitignore or merged into this file.  For a more nuclear
 #  option (not recommended) you can uncomment the following to ignore the entire idea folder.
 #.idea/
 .pdm-python
+
+.pypirc
+
+# Mac Files
+.DS_Store
```

