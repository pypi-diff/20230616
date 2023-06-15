# Comparing `tmp/satori_playbook_validator-2.1.1.tar.gz` & `tmp/satori_playbook_validator-2.1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "satori_playbook_validator-2.1.1.tar", last modified: Wed Jun 14 04:32:27 2023, max compression
+gzip compressed data, was "satori_playbook_validator-2.1.2.tar", last modified: Thu Jun 15 22:25:32 2023, max compression
```

## Comparing `satori_playbook_validator-2.1.1.tar` & `satori_playbook_validator-2.1.2.tar`

### file list

```diff
@@ -1,13 +1,13 @@
--rw-r--r--   0        0        0       30 2023-06-14 04:32:12.568708 satori_playbook_validator-2.1.1/README.md
--rw-r--r--   0        0        0      474 2023-06-14 04:32:27.104775 satori_playbook_validator-2.1.1/pyproject.toml
--rw-r--r--   0        0        0      176 2023-06-14 04:32:12.568708 satori_playbook_validator-2.1.1/src/satorici/validator/__init__.py
--rw-r--r--   0        0        0     5273 2023-06-14 04:32:12.568708 satori_playbook_validator-2.1.1/src/satorici/validator/_validator.py
--rw-r--r--   0        0        0      223 2023-06-14 04:32:12.568708 satori_playbook_validator-2.1.1/src/satorici/validator/exceptions.py
--rw-r--r--   0        0        0      267 2023-06-14 04:32:12.568708 satori_playbook_validator-2.1.1/src/satorici/validator/schemas/command.json
--rw-r--r--   0        0        0      251 2023-06-14 04:32:12.568708 satori_playbook_validator-2.1.1/src/satorici/validator/schemas/import.json
--rw-r--r--   0        0        0     2197 2023-06-14 04:32:12.568708 satori_playbook_validator-2.1.1/src/satorici/validator/schemas/input.json
--rw-r--r--   0        0        0     1049 2023-06-14 04:32:12.568708 satori_playbook_validator-2.1.1/src/satorici/validator/schemas/settings.json
--rw-r--r--   0        0        0     1837 2023-06-14 04:32:12.568708 satori_playbook_validator-2.1.1/src/satorici/validator/schemas/test.json
--rw-r--r--   0        0        0      874 2023-06-14 04:32:12.568708 satori_playbook_validator-2.1.1/tests/test_playbook_validator.py
--rw-r--r--   0        0        0     2469 2023-06-14 04:32:12.568708 satori_playbook_validator-2.1.1/tests/test_reference_finder.py
--rw-r--r--   0        0        0      259 1970-01-01 00:00:00.000000 satori_playbook_validator-2.1.1/PKG-INFO
+-rw-r--r--   0        0        0       30 2023-06-15 22:25:17.934955 satori_playbook_validator-2.1.2/README.md
+-rw-r--r--   0        0        0      474 2023-06-15 22:25:32.139214 satori_playbook_validator-2.1.2/pyproject.toml
+-rw-r--r--   0        0        0      176 2023-06-15 22:25:17.934955 satori_playbook_validator-2.1.2/src/satorici/validator/__init__.py
+-rw-r--r--   0        0        0     5141 2023-06-15 22:25:17.934955 satori_playbook_validator-2.1.2/src/satorici/validator/_validator.py
+-rw-r--r--   0        0        0      223 2023-06-15 22:25:17.934955 satori_playbook_validator-2.1.2/src/satorici/validator/exceptions.py
+-rw-r--r--   0        0        0      267 2023-06-15 22:25:17.934955 satori_playbook_validator-2.1.2/src/satorici/validator/schemas/command.json
+-rw-r--r--   0        0        0      251 2023-06-15 22:25:17.934955 satori_playbook_validator-2.1.2/src/satorici/validator/schemas/import.json
+-rw-r--r--   0        0        0     2197 2023-06-15 22:25:17.934955 satori_playbook_validator-2.1.2/src/satorici/validator/schemas/input.json
+-rw-r--r--   0        0        0     1049 2023-06-15 22:25:17.934955 satori_playbook_validator-2.1.2/src/satorici/validator/schemas/settings.json
+-rw-r--r--   0        0        0     1888 2023-06-15 22:25:17.934955 satori_playbook_validator-2.1.2/src/satorici/validator/schemas/test.json
+-rw-r--r--   0        0        0      874 2023-06-15 22:25:17.934955 satori_playbook_validator-2.1.2/tests/test_playbook_validator.py
+-rw-r--r--   0        0        0     2469 2023-06-15 22:25:17.934955 satori_playbook_validator-2.1.2/tests/test_reference_finder.py
+-rw-r--r--   0        0        0      259 1970-01-01 00:00:00.000000 satori_playbook_validator-2.1.2/PKG-INFO
```

### Comparing `satori_playbook_validator-2.1.1/src/satorici/validator/_validator.py` & `satori_playbook_validator-2.1.2/src/satorici/validator/_validator.py`

 * *Files 4% similar despite different names*

```diff
@@ -172,18 +172,14 @@
 
     if not isinstance(config, dict):
         raise TypeError("config must be a dict")
 
     config_copy = deepcopy(config)
 
     try:
-        if "settings" in config_copy:
-            settings_schema(config_copy["settings"])
-            del config_copy["settings"]
-
         test_schema(config_copy)
     except JsonSchemaValueException as e:
         raise PlaybookValidationError(e.message)
 
     add_parent_info(config_copy)
     iterate_dict(config_copy)
```

### Comparing `satori_playbook_validator-2.1.1/src/satorici/validator/schemas/input.json` & `satori_playbook_validator-2.1.2/src/satorici/validator/schemas/input.json`

 * *Files identical despite different names*

### Comparing `satori_playbook_validator-2.1.1/src/satorici/validator/schemas/settings.json` & `satori_playbook_validator-2.1.2/src/satorici/validator/schemas/settings.json`

 * *Files identical despite different names*

### Comparing `satori_playbook_validator-2.1.1/src/satorici/validator/schemas/test.json` & `satori_playbook_validator-2.1.2/src/satorici/validator/schemas/test.json`

 * *Files 1% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9910714285714286%*

 * *Differences: {"'properties'": "{'settings': {replace: OrderedDict([('$ref', 'file://./settings.json')])}}"}*

```diff
@@ -64,14 +64,16 @@
         },
         "assertKilled": {
             "type": "boolean"
         },
         "assertReturnCode": {
             "type": "integer"
         },
-        "settings": false
+        "settings": {
+            "$ref": "file://./settings.json"
+        }
     },
     "propertyNames": {
         "pattern": "^[\\w-]+$"
     },
     "type": "object"
 }
```

### Comparing `satori_playbook_validator-2.1.1/tests/test_playbook_validator.py` & `satori_playbook_validator-2.1.2/tests/test_playbook_validator.py`

 * *Files identical despite different names*

### Comparing `satori_playbook_validator-2.1.1/tests/test_reference_finder.py` & `satori_playbook_validator-2.1.2/tests/test_reference_finder.py`

 * *Files identical despite different names*

