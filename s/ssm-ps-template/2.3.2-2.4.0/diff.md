# Comparing `tmp/ssm-ps-template-2.3.2.tar.gz` & `tmp/ssm-ps-template-2.4.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ssm-ps-template-2.3.2.tar", last modified: Thu Jun 15 23:04:14 2023, max compression
+gzip compressed data, was "ssm-ps-template-2.4.0.tar", last modified: Fri Jun 16 16:25:02 2023, max compression
```

## Comparing `ssm-ps-template-2.3.2.tar` & `ssm-ps-template-2.4.0.tar`

### file list

```diff
@@ -1,26 +1,26 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-15 23:04:14.803370 ssm-ps-template-2.3.2/
--rw-r--r--   0 root         (0) root         (0)     1495 2023-06-15 23:04:04.000000 ssm-ps-template-2.3.2/LICENSE.txt
--rw-r--r--   0 root         (0) root         (0)    12318 2023-06-15 23:04:14.803370 ssm-ps-template-2.3.2/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     9682 2023-06-15 23:04:04.000000 ssm-ps-template-2.3.2/README.md
--rw-r--r--   0 root         (0) root         (0)     1875 2023-06-15 23:04:04.000000 ssm-ps-template-2.3.2/pyproject.toml
--rw-r--r--   0 root         (0) root         (0)       38 2023-06-15 23:04:14.803370 ssm-ps-template-2.3.2/setup.cfg
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-15 23:04:14.803370 ssm-ps-template-2.3.2/ssm_ps_template/
--rw-r--r--   0 root         (0) root         (0)      148 2023-06-15 23:04:04.000000 ssm-ps-template-2.3.2/ssm_ps_template/__init__.py
--rw-r--r--   0 root         (0) root         (0)     3254 2023-06-15 23:04:04.000000 ssm-ps-template-2.3.2/ssm_ps_template/__main__.py
--rw-r--r--   0 root         (0) root         (0)     2364 2023-06-15 23:04:04.000000 ssm-ps-template-2.3.2/ssm_ps_template/config.py
--rw-r--r--   0 root         (0) root         (0)     1825 2023-06-15 23:04:04.000000 ssm-ps-template-2.3.2/ssm_ps_template/discovery.py
--rw-r--r--   0 root         (0) root         (0)     2834 2023-06-15 23:04:04.000000 ssm-ps-template-2.3.2/ssm_ps_template/render.py
--rw-r--r--   0 root         (0) root         (0)     3462 2023-06-15 23:04:04.000000 ssm-ps-template-2.3.2/ssm_ps_template/ssm.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-15 23:04:14.803370 ssm-ps-template-2.3.2/ssm_ps_template.egg-info/
--rw-r--r--   0 root         (0) root         (0)    12318 2023-06-15 23:04:14.000000 ssm-ps-template-2.3.2/ssm_ps_template.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      535 2023-06-15 23:04:14.000000 ssm-ps-template-2.3.2/ssm_ps_template.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-06-15 23:04:14.000000 ssm-ps-template-2.3.2/ssm_ps_template.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)       66 2023-06-15 23:04:14.000000 ssm-ps-template-2.3.2/ssm_ps_template.egg-info/entry_points.txt
--rw-r--r--   0 root         (0) root         (0)      242 2023-06-15 23:04:14.000000 ssm-ps-template-2.3.2/ssm_ps_template.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)       16 2023-06-15 23:04:14.000000 ssm-ps-template-2.3.2/ssm_ps_template.egg-info/top_level.txt
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-15 23:04:14.803370 ssm-ps-template-2.3.2/tests/
--rw-r--r--   0 root         (0) root         (0)     2833 2023-06-15 23:04:04.000000 ssm-ps-template-2.3.2/tests/test_config.py
--rw-r--r--   0 root         (0) root         (0)      784 2023-06-15 23:04:04.000000 ssm-ps-template-2.3.2/tests/test_discovery.py
--rw-r--r--   0 root         (0) root         (0)     1332 2023-06-15 23:04:04.000000 ssm-ps-template-2.3.2/tests/test_main.py
--rw-r--r--   0 root         (0) root         (0)     2191 2023-06-15 23:04:04.000000 ssm-ps-template-2.3.2/tests/test_render.py
--rw-r--r--   0 root         (0) root         (0)     3119 2023-06-15 23:04:04.000000 ssm-ps-template-2.3.2/tests/test_ssm.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-16 16:25:02.580162 ssm-ps-template-2.4.0/
+-rw-r--r--   0 root         (0) root         (0)     1495 2023-06-16 16:24:52.000000 ssm-ps-template-2.4.0/LICENSE.txt
+-rw-r--r--   0 root         (0) root         (0)    12692 2023-06-16 16:25:02.580162 ssm-ps-template-2.4.0/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)    10056 2023-06-16 16:24:52.000000 ssm-ps-template-2.4.0/README.md
+-rw-r--r--   0 root         (0) root         (0)     1875 2023-06-16 16:24:52.000000 ssm-ps-template-2.4.0/pyproject.toml
+-rw-r--r--   0 root         (0) root         (0)       38 2023-06-16 16:25:02.580162 ssm-ps-template-2.4.0/setup.cfg
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-16 16:25:02.580162 ssm-ps-template-2.4.0/ssm_ps_template/
+-rw-r--r--   0 root         (0) root         (0)      148 2023-06-16 16:24:52.000000 ssm-ps-template-2.4.0/ssm_ps_template/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     4072 2023-06-16 16:24:52.000000 ssm-ps-template-2.4.0/ssm_ps_template/__main__.py
+-rw-r--r--   0 root         (0) root         (0)     2814 2023-06-16 16:24:52.000000 ssm-ps-template-2.4.0/ssm_ps_template/config.py
+-rw-r--r--   0 root         (0) root         (0)     1825 2023-06-16 16:24:52.000000 ssm-ps-template-2.4.0/ssm_ps_template/discovery.py
+-rw-r--r--   0 root         (0) root         (0)     2834 2023-06-16 16:24:52.000000 ssm-ps-template-2.4.0/ssm_ps_template/render.py
+-rw-r--r--   0 root         (0) root         (0)     3462 2023-06-16 16:24:52.000000 ssm-ps-template-2.4.0/ssm_ps_template/ssm.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-16 16:25:02.580162 ssm-ps-template-2.4.0/ssm_ps_template.egg-info/
+-rw-r--r--   0 root         (0) root         (0)    12692 2023-06-16 16:25:02.000000 ssm-ps-template-2.4.0/ssm_ps_template.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      535 2023-06-16 16:25:02.000000 ssm-ps-template-2.4.0/ssm_ps_template.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-06-16 16:25:02.000000 ssm-ps-template-2.4.0/ssm_ps_template.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)       66 2023-06-16 16:25:02.000000 ssm-ps-template-2.4.0/ssm_ps_template.egg-info/entry_points.txt
+-rw-r--r--   0 root         (0) root         (0)      242 2023-06-16 16:25:02.000000 ssm-ps-template-2.4.0/ssm_ps_template.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)       16 2023-06-16 16:25:02.000000 ssm-ps-template-2.4.0/ssm_ps_template.egg-info/top_level.txt
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-16 16:25:02.580162 ssm-ps-template-2.4.0/tests/
+-rw-r--r--   0 root         (0) root         (0)     3021 2023-06-16 16:24:52.000000 ssm-ps-template-2.4.0/tests/test_config.py
+-rw-r--r--   0 root         (0) root         (0)      784 2023-06-16 16:24:52.000000 ssm-ps-template-2.4.0/tests/test_discovery.py
+-rw-r--r--   0 root         (0) root         (0)     2753 2023-06-16 16:24:52.000000 ssm-ps-template-2.4.0/tests/test_main.py
+-rw-r--r--   0 root         (0) root         (0)     2191 2023-06-16 16:24:52.000000 ssm-ps-template-2.4.0/tests/test_render.py
+-rw-r--r--   0 root         (0) root         (0)     3119 2023-06-16 16:24:52.000000 ssm-ps-template-2.4.0/tests/test_ssm.py
```

### Comparing `ssm-ps-template-2.3.2/LICENSE.txt` & `ssm-ps-template-2.4.0/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `ssm-ps-template-2.3.2/PKG-INFO` & `ssm-ps-template-2.4.0/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ssm-ps-template
-Version: 2.3.2
+Version: 2.4.0
 Summary: CLI for rendering configuration templates with SSM Parameter Store as a data source
 Author-email: "Gavin M. Roy" <gavinmroy@gmail.com>
 License: Copyright (c) 2023 Gavin M. Roy
         All rights reserved.
         
         Redistribution and use in source and binary forms, with or without modification,
         are permitted provided that the following conditions are met:
@@ -142,21 +142,26 @@
 | `profile`             | Specify the AWS profile to use. If unspecified will default to the `AWS_DEFAULT_PROFILE` environment variable or is unspecified  |
 | `region`              | Specify the AWS region to use. If unspecified it will default to the `AWS_DEFAULT_REGION` environment variable or is unspecified |
 | `replace_underscores` | Replace underscores with dashes when asking for values from SSM Parameter Store                                                  |
 | `verbose`             | Turn debug logging on. Possible values are `true` and `false`                                                                    |
 
 ### Template Configuration Directives
 
-The `templates` directive in the configuration is an array of objects, defined by a `source` and `destination`.
+The `templates` directive in the configuration is an array of objects:
 
 | Directive     | Description                                                                          |
 |---------------|--------------------------------------------------------------------------------------|
 | `source`      | The source file of the template                                                      |
 | `destination` | The destination path to write the rendered template to                               |
 | `prefix`      | The prefix to prepend variables with if they do not start with a forward-slash (`/`) |
+| `user`        | An optional username or uid to set as the owner of the rendered file                 |
+| `group`       | An optional group or gid to set as the group of the rendered file                    |
+| `mode`        | Optional file mode and permissions set using chmod                                   |
+
+If there are parent directories in the `destination` path that do not exist, they will be created.
 
 ### Extended Templating Functionality
 
 In addition to the base functionality exposed by Jinja2, the following Python functions have been added:
 
 | Function                 | Definition                                                                                                                                          |
 |--------------------------|-----------------------------------------------------------------------------------------------------------------------------------------------------|
```

### Comparing `ssm-ps-template-2.3.2/README.md` & `ssm-ps-template-2.4.0/README.md`

 * *Files 8% similar despite different names*

```diff
@@ -93,21 +93,26 @@
 | `profile`             | Specify the AWS profile to use. If unspecified will default to the `AWS_DEFAULT_PROFILE` environment variable or is unspecified  |
 | `region`              | Specify the AWS region to use. If unspecified it will default to the `AWS_DEFAULT_REGION` environment variable or is unspecified |
 | `replace_underscores` | Replace underscores with dashes when asking for values from SSM Parameter Store                                                  |
 | `verbose`             | Turn debug logging on. Possible values are `true` and `false`                                                                    |
 
 ### Template Configuration Directives
 
-The `templates` directive in the configuration is an array of objects, defined by a `source` and `destination`.
+The `templates` directive in the configuration is an array of objects:
 
 | Directive     | Description                                                                          |
 |---------------|--------------------------------------------------------------------------------------|
 | `source`      | The source file of the template                                                      |
 | `destination` | The destination path to write the rendered template to                               |
 | `prefix`      | The prefix to prepend variables with if they do not start with a forward-slash (`/`) |
+| `user`        | An optional username or uid to set as the owner of the rendered file                 |
+| `group`       | An optional group or gid to set as the group of the rendered file                    |
+| `mode`        | Optional file mode and permissions set using chmod                                   |
+
+If there are parent directories in the `destination` path that do not exist, they will be created.
 
 ### Extended Templating Functionality
 
 In addition to the base functionality exposed by Jinja2, the following Python functions have been added:
 
 | Function                 | Definition                                                                                                                                          |
 |--------------------------|-----------------------------------------------------------------------------------------------------------------------------------------------------|
```

### Comparing `ssm-ps-template-2.3.2/pyproject.toml` & `ssm-ps-template-2.4.0/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [project]
 name = "ssm-ps-template"
-version = "2.3.2"
+version = "2.4.0"
 description = "CLI for rendering configuration templates with SSM Parameter Store as a data source"
 authors = [
     {name = "Gavin M. Roy", email="gavinmroy@gmail.com"}
 ]
 classifiers = [
     "Topic :: Software Development",
     "License :: OSI Approved :: BSD License",
@@ -17,15 +17,15 @@
     "Topic :: Text Processing",
     "Topic :: Utilities"
 ]
 dependencies = [
     "boto3>=1.26,<2",
     "flatdict>=4,<5",
     "jinja2>=3,<4",
-    "pyyaml>=5.3.1,<6",
+    "pyyaml>=5.3.1,<7",
     "toml>=0.10,<1"
 ]
 keywords = ["aws", "ssm", "parameter store", "templating"]
 license = {file = "LICENSE.txt"}
 readme = "README.md"
 requires-python = ">=3.9"
```

### Comparing `ssm-ps-template-2.3.2/ssm_ps_template/__main__.py` & `ssm-ps-template-2.4.0/ssm_ps_template/__main__.py`

 * *Files 21% similar despite different names*

```diff
@@ -1,21 +1,36 @@
 import argparse
+import grp
 import logging
 import os
+import pwd
 import sys
 import time
 import typing
 from importlib import metadata
 
 from ssm_ps_template import config, discovery, render, ssm
 
 LOGGER = logging.getLogger(__name__)
 LOGGING_FORMAT = '%(message)s'
 
 
+def chown(path: str,
+          user: typing.Union[int, str, None],
+          group: typing.Union[int, str, None]) -> typing.NoReturn:
+    kwargs = {'path': path}
+    if user is not None and not str(user).isnumeric():
+        user = pwd.getpwnam(str(user)).pw_uid
+    kwargs['uid'] = int(user) if user else os.getuid()
+    if group is not None and not str(group).isnumeric():
+        group = grp.getgrnam(str(group)).gr_gid
+    kwargs['gid'] = int(group) if group else os.getgid()
+    os.chown(**kwargs)
+
+
 def parse_cli_arguments(args: typing.Optional[typing.List[str]] = None) \
         -> argparse.Namespace:
     parser = argparse.ArgumentParser(
         description='Command line application to render templates with data '
                     'from SSM Parameter Store',
         formatter_class=argparse.ArgumentDefaultsHelpFormatter)
     parser.add_argument(
@@ -60,17 +75,25 @@
         try:
             values = parameter_store.fetch_variables(
                 variables, prefix, args.replace_underscores)
         except ssm.SSMClientException as err:
             LOGGER.error('Error fetching parameters: %s', err)
             sys.exit(1)
 
+        if not template.destination.parent.exists():
+            template.destination.parent.mkdir(parents=True, exist_ok=True)
+
         renderer = render.Renderer(source=template.source)
-        with template.destination.open('w') as handle:
-            handle.write(renderer.render(values))
+        template.destination.write_text(renderer.render(values))
+
+        if template.user or template.group:
+            chown(str(template.destination), template.user, template.group)
+
+        if template.mode:
+            template.destination.chmod(template.mode)
 
         LOGGER.info('Rendered %s in %0.2f seconds', template.destination,
                     time.time() - start_time)
 
 
 def main():  # pragma: no cover
     args = parse_cli_arguments()
```

### Comparing `ssm-ps-template-2.3.2/ssm_ps_template/config.py` & `ssm-ps-template-2.4.0/ssm_ps_template/config.py`

 * *Files 10% similar despite different names*

```diff
@@ -9,14 +9,17 @@
 
 
 @dataclasses.dataclass
 class Template:
     source: pathlib.Path
     destination: pathlib.Path
     prefix: typing.Optional[str]
+    user: typing.Union[int, str, None]
+    group: typing.Union[int, str, None]
+    mode: typing.Optional[str]
 
 
 @dataclasses.dataclass
 class Configuration:
     endpoint_url: typing.Optional[str]
     profile: typing.Optional[str]
     region: typing.Optional[str]
@@ -25,18 +28,23 @@
     verbose: bool
 
 
 def _load_configuration(value: dict) -> Configuration:
     templates = []
     try:
         for template in value['templates'] or []:
+            mode = int(template.get('mode'), 8) \
+                if template.get('mode') else None
             templates.append(_entry_to_template(
                 source=template['source'],
                 destination=template['destination'],
-                prefix=template.get('prefix')))
+                prefix=template.get('prefix'),
+                user=template.get('user'),
+                group=template.get('group'),
+                mode=mode))
     except KeyError as error:
         raise argparse.ArgumentTypeError(
             f'Failed to load configuration due to invalid key: {error}')
     return Configuration(
         endpoint_url=value.get('endpoint_url'),
         profile=value.get('profile'),
         region=value.get('region'),
@@ -48,15 +56,18 @@
 def _entry_to_template(**kwargs) -> Template:
     source = pathlib.Path(kwargs['source'])
     if not source.exists():
         raise argparse.ArgumentTypeError(
             f'Specified template {source} does not exist')
     return Template(source=source,
                     destination=pathlib.Path(kwargs['destination']),
-                    prefix=kwargs['prefix'])
+                    prefix=kwargs['prefix'],
+                    user=kwargs['user'],
+                    group=kwargs['group'],
+                    mode=kwargs['mode'])
 
 
 def configuration_file(value: str) -> Configuration:
     """Load the configuration from the specified path"""
     path = pathlib.Path(value)
     if not path.exists():
         raise argparse.ArgumentTypeError(f'{value} does not exist')
```

### Comparing `ssm-ps-template-2.3.2/ssm_ps_template/discovery.py` & `ssm-ps-template-2.4.0/ssm_ps_template/discovery.py`

 * *Files identical despite different names*

### Comparing `ssm-ps-template-2.3.2/ssm_ps_template/render.py` & `ssm-ps-template-2.4.0/ssm_ps_template/render.py`

 * *Files identical despite different names*

### Comparing `ssm-ps-template-2.3.2/ssm_ps_template/ssm.py` & `ssm-ps-template-2.4.0/ssm_ps_template/ssm.py`

 * *Files identical despite different names*

### Comparing `ssm-ps-template-2.3.2/ssm_ps_template.egg-info/PKG-INFO` & `ssm-ps-template-2.4.0/ssm_ps_template.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ssm-ps-template
-Version: 2.3.2
+Version: 2.4.0
 Summary: CLI for rendering configuration templates with SSM Parameter Store as a data source
 Author-email: "Gavin M. Roy" <gavinmroy@gmail.com>
 License: Copyright (c) 2023 Gavin M. Roy
         All rights reserved.
         
         Redistribution and use in source and binary forms, with or without modification,
         are permitted provided that the following conditions are met:
@@ -142,21 +142,26 @@
 | `profile`             | Specify the AWS profile to use. If unspecified will default to the `AWS_DEFAULT_PROFILE` environment variable or is unspecified  |
 | `region`              | Specify the AWS region to use. If unspecified it will default to the `AWS_DEFAULT_REGION` environment variable or is unspecified |
 | `replace_underscores` | Replace underscores with dashes when asking for values from SSM Parameter Store                                                  |
 | `verbose`             | Turn debug logging on. Possible values are `true` and `false`                                                                    |
 
 ### Template Configuration Directives
 
-The `templates` directive in the configuration is an array of objects, defined by a `source` and `destination`.
+The `templates` directive in the configuration is an array of objects:
 
 | Directive     | Description                                                                          |
 |---------------|--------------------------------------------------------------------------------------|
 | `source`      | The source file of the template                                                      |
 | `destination` | The destination path to write the rendered template to                               |
 | `prefix`      | The prefix to prepend variables with if they do not start with a forward-slash (`/`) |
+| `user`        | An optional username or uid to set as the owner of the rendered file                 |
+| `group`       | An optional group or gid to set as the group of the rendered file                    |
+| `mode`        | Optional file mode and permissions set using chmod                                   |
+
+If there are parent directories in the `destination` path that do not exist, they will be created.
 
 ### Extended Templating Functionality
 
 In addition to the base functionality exposed by Jinja2, the following Python functions have been added:
 
 | Function                 | Definition                                                                                                                                          |
 |--------------------------|-----------------------------------------------------------------------------------------------------------------------------------------------------|
```

### Comparing `ssm-ps-template-2.3.2/ssm_ps_template.egg-info/SOURCES.txt` & `ssm-ps-template-2.4.0/ssm_ps_template.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `ssm-ps-template-2.3.2/tests/test_config.py` & `ssm-ps-template-2.4.0/tests/test_config.py`

 * *Files 6% similar despite different names*

```diff
@@ -15,19 +15,25 @@
 
     def setUp(self) -> None:
         self.expectation = config.Configuration(
             templates=[
                 config.Template(
                     source=relative_test_data_path('config/case1a.tmpl'),
                     destination=pathlib.Path('build/case1a.out'),
-                    prefix='/foo/bar/baz'),
+                    prefix='/foo/bar/baz',
+                    user=None,
+                    group=None,
+                    mode=None),
                 config.Template(
                     source=relative_test_data_path('config/case1b.tmpl'),
                     destination=pathlib.Path('build/case1b.out'),
-                    prefix=None)],
+                    prefix=None,
+                    user=None,
+                    group=None,
+                    mode=None)],
             endpoint_url=None,
             profile=None,
             region=None,
             replace_underscores=False,
             verbose=False)
 
     def test_load_json_file(self):
```

### Comparing `ssm-ps-template-2.3.2/tests/test_discovery.py` & `ssm-ps-template-2.4.0/tests/test_discovery.py`

 * *Files identical despite different names*

### Comparing `ssm-ps-template-2.3.2/tests/test_render.py` & `ssm-ps-template-2.4.0/tests/test_render.py`

 * *Files identical despite different names*

### Comparing `ssm-ps-template-2.3.2/tests/test_ssm.py` & `ssm-ps-template-2.4.0/tests/test_ssm.py`

 * *Files identical despite different names*

