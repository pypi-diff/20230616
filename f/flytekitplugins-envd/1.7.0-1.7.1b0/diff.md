# Comparing `tmp/flytekitplugins-envd-1.7.0.tar.gz` & `tmp/flytekitplugins-envd-1.7.1b0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "flytekitplugins-envd-1.7.0.tar", last modified: Wed Jun 14 04:33:29 2023, max compression
+gzip compressed data, was "flytekitplugins-envd-1.7.1b0.tar", last modified: Fri Jun 16 18:14:19 2023, max compression
```

## Comparing `flytekitplugins-envd-1.7.0.tar` & `flytekitplugins-envd-1.7.1b0.tar`

### file list

```diff
@@ -1,17 +1,17 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 04:33:29.001332 flytekitplugins-envd-1.7.0/
--rw-r--r--   0 runner    (1001) docker     (123)      886 2023-06-14 04:33:29.001332 flytekitplugins-envd-1.7.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      797 2023-06-14 04:33:05.000000 flytekitplugins-envd-1.7.0/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 04:33:29.001332 flytekitplugins-envd-1.7.0/flytekitplugins/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 04:33:29.001332 flytekitplugins-envd-1.7.0/flytekitplugins/envd/
--rw-r--r--   0 runner    (1001) docker     (123)      255 2023-06-14 04:33:05.000000 flytekitplugins-envd-1.7.0/flytekitplugins/envd/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2791 2023-06-14 04:33:05.000000 flytekitplugins-envd-1.7.0/flytekitplugins/envd/image_builder.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 04:33:29.001332 flytekitplugins-envd-1.7.0/flytekitplugins_envd.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)      886 2023-06-14 04:33:28.000000 flytekitplugins-envd-1.7.0/flytekitplugins_envd.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      408 2023-06-14 04:33:28.000000 flytekitplugins-envd-1.7.0/flytekitplugins_envd.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-14 04:33:28.000000 flytekitplugins-envd-1.7.0/flytekitplugins_envd.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       47 2023-06-14 04:33:28.000000 flytekitplugins-envd-1.7.0/flytekitplugins_envd.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)       16 2023-06-14 04:33:28.000000 flytekitplugins-envd-1.7.0/flytekitplugins_envd.egg-info/namespace_packages.txt
--rw-r--r--   0 runner    (1001) docker     (123)       22 2023-06-14 04:33:28.000000 flytekitplugins-envd-1.7.0/flytekitplugins_envd.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       16 2023-06-14 04:33:28.000000 flytekitplugins-envd-1.7.0/flytekitplugins_envd.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-14 04:33:29.001332 flytekitplugins-envd-1.7.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1320 2023-06-14 04:33:24.000000 flytekitplugins-envd-1.7.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 18:14:19.694435 flytekitplugins-envd-1.7.1b0/
+-rw-r--r--   0 runner    (1001) docker     (123)      888 2023-06-16 18:14:19.694435 flytekitplugins-envd-1.7.1b0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      797 2023-06-16 18:13:54.000000 flytekitplugins-envd-1.7.1b0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 18:14:19.690436 flytekitplugins-envd-1.7.1b0/flytekitplugins/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 18:14:19.690436 flytekitplugins-envd-1.7.1b0/flytekitplugins/envd/
+-rw-r--r--   0 runner    (1001) docker     (123)      255 2023-06-16 18:13:54.000000 flytekitplugins-envd-1.7.1b0/flytekitplugins/envd/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3307 2023-06-16 18:13:54.000000 flytekitplugins-envd-1.7.1b0/flytekitplugins/envd/image_builder.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 18:14:19.694435 flytekitplugins-envd-1.7.1b0/flytekitplugins_envd.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)      888 2023-06-16 18:14:19.000000 flytekitplugins-envd-1.7.1b0/flytekitplugins_envd.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      408 2023-06-16 18:14:19.000000 flytekitplugins-envd-1.7.1b0/flytekitplugins_envd.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-16 18:14:19.000000 flytekitplugins-envd-1.7.1b0/flytekitplugins_envd.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       47 2023-06-16 18:14:19.000000 flytekitplugins-envd-1.7.1b0/flytekitplugins_envd.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       16 2023-06-16 18:14:19.000000 flytekitplugins-envd-1.7.1b0/flytekitplugins_envd.egg-info/namespace_packages.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       22 2023-06-16 18:14:19.000000 flytekitplugins-envd-1.7.1b0/flytekitplugins_envd.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       16 2023-06-16 18:14:19.000000 flytekitplugins-envd-1.7.1b0/flytekitplugins_envd.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-16 18:14:19.694435 flytekitplugins-envd-1.7.1b0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1322 2023-06-16 18:14:14.000000 flytekitplugins-envd-1.7.1b0/setup.py
```

### Comparing `flytekitplugins-envd-1.7.0/PKG-INFO` & `flytekitplugins-envd-1.7.1b0/PKG-INFO`

 * *Files 12% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: flytekitplugins-envd
-Version: 1.7.0
+Version: 1.7.1b0
 Summary: This package enables users to easily build a Docker image for tasks or workflows.
 Author: flyteorg
 Author-email: admin@flyte.org
 License: apache2
 Classifier: Intended Audience :: Science/Research
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: Apache Software License
```

### Comparing `flytekitplugins-envd-1.7.0/README.md` & `flytekitplugins-envd-1.7.1b0/README.md`

 * *Files identical despite different names*

### Comparing `flytekitplugins-envd-1.7.0/flytekitplugins/envd/image_builder.py` & `flytekitplugins-envd-1.7.1b0/flytekitplugins/envd/image_builder.py`

 * *Files 12% similar despite different names*

```diff
@@ -32,36 +32,46 @@
             raise Exception(
                 f"failed to build the imageSpec at {cfg_path} with error {stderr}",
             )
 
 
 def create_envd_config(image_spec: ImageSpec) -> str:
     base_image = DefaultImages.default_image() if image_spec.base_image is None else image_spec.base_image
+    if image_spec.cuda:
+        if image_spec.python_version is None:
+            raise Exception("python_version is required when cuda and cudnn are specified")
+        base_image = "ubuntu20.04"
+
     packages = [] if image_spec.packages is None else image_spec.packages
     apt_packages = [] if image_spec.apt_packages is None else image_spec.apt_packages
     env = {"PYTHONPATH": "/root", _F_IMG_ID: image_spec.image_name()}
     if image_spec.env:
         env.update(image_spec.env)
+    pip_index = "https://pypi.org/simple" if image_spec.pip_index is None else image_spec.pip_index
 
     envd_config = f"""# syntax=v1
 
 def build():
     base(image="{base_image}", dev=False)
     install.python_packages(name = [{', '.join(map(str, map(lambda x: f'"{x}"', packages)))}])
     install.apt_packages(name = [{', '.join(map(str, map(lambda x: f'"{x}"', apt_packages)))}])
     runtime.environ(env={env})
+    config.pip_index(url = "{pip_index}")
 """
+    ctx = context_manager.FlyteContextManager.current_context()
+    cfg_path = ctx.file_access.get_random_local_path("build.envd")
+    pathlib.Path(cfg_path).parent.mkdir(parents=True, exist_ok=True)
 
     if image_spec.python_version:
         # Indentation is required by envd
         envd_config += f'    install.python(version="{image_spec.python_version}")\n'
 
-    ctx = context_manager.FlyteContextManager.current_context()
-    cfg_path = ctx.file_access.get_random_local_path("build.envd")
-    pathlib.Path(cfg_path).parent.mkdir(parents=True, exist_ok=True)
+    if image_spec.cuda:
+        cudnn = image_spec.cudnn if image_spec.cudnn else ""
+        envd_config += f'    install.cuda(version="{image_spec.cuda}", cudnn="{cudnn}")\n'
 
     if image_spec.source_root:
         shutil.copytree(image_spec.source_root, pathlib.Path(cfg_path).parent, dirs_exist_ok=True)
         # Indentation is required by envd
         envd_config += '    io.copy(host_path="./", envd_path="/root")'
 
     with open(cfg_path, "w+") as f:
```

### Comparing `flytekitplugins-envd-1.7.0/flytekitplugins_envd.egg-info/PKG-INFO` & `flytekitplugins-envd-1.7.1b0/flytekitplugins_envd.egg-info/PKG-INFO`

 * *Files 12% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: flytekitplugins-envd
-Version: 1.7.0
+Version: 1.7.1b0
 Summary: This package enables users to easily build a Docker image for tasks or workflows.
 Author: flyteorg
 Author-email: admin@flyte.org
 License: apache2
 Classifier: Intended Audience :: Science/Research
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: Apache Software License
```

### Comparing `flytekitplugins-envd-1.7.0/setup.py` & `flytekitplugins-envd-1.7.1b0/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 
 PLUGIN_NAME = "envd"
 
 microlib_name = f"flytekitplugins-{PLUGIN_NAME}"
 
 plugin_requires = ["flytekit", "envd>=0.3.22"]
 
-__version__ = "1.7.0"
+__version__ = "1.7.1b0"
 
 setup(
     name=microlib_name,
     version=__version__,
     author="flyteorg",
     author_email="admin@flyte.org",
     description="This package enables users to easily build a Docker image for tasks or workflows.",
```

