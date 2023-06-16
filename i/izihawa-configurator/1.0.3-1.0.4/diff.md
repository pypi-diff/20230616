# Comparing `tmp/izihawa_configurator-1.0.3-py3-none-any.whl.zip` & `tmp/izihawa_configurator-1.0.4-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,7 +1,7 @@
-Zip file size: 3099 bytes, number of entries: 5
--rw-r--r--  2.0 unx     5654 b- defN 23-Jun-16 14:17 izihawa_configurator/__init__.py
+Zip file size: 2945 bytes, number of entries: 5
+-rw-r--r--  2.0 unx     5169 b- defN 23-Jun-16 14:21 izihawa_configurator/__init__.py
 -rw-r--r--  2.0 unx       52 b- defN 22-Oct-25 09:23 izihawa_configurator/exceptions.py
-?rw-------  2.0 unx       91 b- defN 23-Jun-16 14:18 izihawa_configurator-1.0.3.dist-info/WHEEL
-?rw-------  2.0 unx      465 b- defN 23-Jun-16 14:18 izihawa_configurator-1.0.3.dist-info/METADATA
-?rw-------  2.0 unx      422 b- defN 23-Jun-16 14:18 izihawa_configurator-1.0.3.dist-info/RECORD
-5 files, 6684 bytes uncompressed, 2305 bytes compressed:  65.5%
+?rw-------  2.0 unx       91 b- defN 23-Jun-16 14:21 izihawa_configurator-1.0.4.dist-info/WHEEL
+?rw-------  2.0 unx      465 b- defN 23-Jun-16 14:21 izihawa_configurator-1.0.4.dist-info/METADATA
+?rw-------  2.0 unx      422 b- defN 23-Jun-16 14:21 izihawa_configurator-1.0.4.dist-info/RECORD
+5 files, 6199 bytes uncompressed, 2151 bytes compressed:  65.3%
```

## zipnote {}

```diff
@@ -1,16 +1,16 @@
 Filename: izihawa_configurator/__init__.py
 Comment: 
 
 Filename: izihawa_configurator/exceptions.py
 Comment: 
 
-Filename: izihawa_configurator-1.0.3.dist-info/WHEEL
+Filename: izihawa_configurator-1.0.4.dist-info/WHEEL
 Comment: 
 
-Filename: izihawa_configurator-1.0.3.dist-info/METADATA
+Filename: izihawa_configurator-1.0.4.dist-info/METADATA
 Comment: 
 
-Filename: izihawa_configurator-1.0.3.dist-info/RECORD
+Filename: izihawa_configurator-1.0.4.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## izihawa_configurator/__init__.py

```diff
@@ -1,22 +1,18 @@
 import json
 import os
 import os.path
-import re
 from types import ModuleType
 
 import yaml
 from izihawa_configurator.exceptions import UnknownConfigFormatError
 from izihawa_utils.common import smart_merge_dicts, unflatten
 from jinja2 import Template
 
 
-array_regex = re.compile(r"\[([!\"#$%&'()*+,-./:;<=>?@^_`{|}~])]")
-
-
 class ConfigObject(dict):
     def __getattr__(self, name):
         try:
             return self[name]
         except KeyError as e:
             raise AttributeError(e)
 
@@ -61,21 +57,15 @@
         env_dict = {}
 
         if env_prefix:
             env_prefix = env_prefix.lower()
             for name, value in os.environ.items():
                 if name.lower().startswith(env_prefix):
                     stripped_name = name[len(env_prefix):].lstrip('_')
-                    array_regex_result = array_regex.match(stripped_name[-3:])
-                    if array_regex_result and array_regex_result.group(1):
-                        if stripped_name not in env_dict:
-                            env_dict[stripped_name[:-3]] = []
-                        env_dict[stripped_name[:-3]].append(value.split(array_regex_result.group(1)))
-                    else:
-                        env_dict[stripped_name] = yaml.safe_load(value)
+                    env_dict[stripped_name] = yaml.safe_load(value)
             env_dict = unflatten(env_dict, sep=env_key_separator)
 
         for config in ([os.environ] + configs + [env_dict]):
             file_found = self.update(config)
             if not file_found:
                 self._omitted_files.append(config)
```

