# Comparing `tmp/ovos-PHAL-plugin-alsa-0.0.2a2.tar.gz` & `tmp/ovos-PHAL-plugin-alsa-0.0.3a2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ovos-PHAL-plugin-alsa-0.0.2a2.tar", last modified: Wed Jun 14 21:23:34 2023, max compression
+gzip compressed data, was "ovos-PHAL-plugin-alsa-0.0.3a2.tar", last modified: Fri Jun 16 16:57:31 2023, max compression
```

## Comparing `ovos-PHAL-plugin-alsa-0.0.2a2.tar` & `ovos-PHAL-plugin-alsa-0.0.3a2.tar`

### file list

```diff
@@ -1,15 +1,16 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 21:23:34.693368 ovos-PHAL-plugin-alsa-0.0.2a2/
--rw-r--r--   0 runner    (1001) docker     (123)      622 2023-06-14 21:23:34.693368 ovos-PHAL-plugin-alsa-0.0.2a2/PKG-INFO
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 21:23:34.689368 ovos-PHAL-plugin-alsa-0.0.2a2/ovos_PHAL_plugin_alsa/
--rw-r--r--   0 runner    (1001) docker     (123)     7801 2023-06-14 21:23:25.000000 ovos-PHAL-plugin-alsa-0.0.2a2/ovos_PHAL_plugin_alsa/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      177 2023-06-14 21:23:28.000000 ovos-PHAL-plugin-alsa-0.0.2a2/ovos_PHAL_plugin_alsa/version.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 21:23:34.693368 ovos-PHAL-plugin-alsa-0.0.2a2/ovos_PHAL_plugin_alsa.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)      622 2023-06-14 21:23:34.000000 ovos-PHAL-plugin-alsa-0.0.2a2/ovos_PHAL_plugin_alsa.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      387 2023-06-14 21:23:34.000000 ovos-PHAL-plugin-alsa-0.0.2a2/ovos_PHAL_plugin_alsa.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-14 21:23:34.000000 ovos-PHAL-plugin-alsa-0.0.2a2/ovos_PHAL_plugin_alsa.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       88 2023-06-14 21:23:34.000000 ovos-PHAL-plugin-alsa-0.0.2a2/ovos_PHAL_plugin_alsa.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)       61 2023-06-14 21:23:34.000000 ovos-PHAL-plugin-alsa-0.0.2a2/ovos_PHAL_plugin_alsa.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       22 2023-06-14 21:23:34.000000 ovos-PHAL-plugin-alsa-0.0.2a2/ovos_PHAL_plugin_alsa.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-14 21:23:34.000000 ovos-PHAL-plugin-alsa-0.0.2a2/ovos_PHAL_plugin_alsa.egg-info/zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-14 21:23:34.693368 ovos-PHAL-plugin-alsa-0.0.2a2/setup.cfg
--rwxr-xr-x   0 runner    (1001) docker     (123)     2748 2023-06-14 21:23:25.000000 ovos-PHAL-plugin-alsa-0.0.2a2/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 16:57:31.303150 ovos-PHAL-plugin-alsa-0.0.3a2/
+-rw-r--r--   0 runner    (1001) docker     (123)      963 2023-06-16 16:57:31.303150 ovos-PHAL-plugin-alsa-0.0.3a2/PKG-INFO
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 16:57:31.303150 ovos-PHAL-plugin-alsa-0.0.3a2/ovos_PHAL_plugin_alsa/
+-rw-r--r--   0 runner    (1001) docker     (123)     7801 2023-06-16 16:57:27.000000 ovos-PHAL-plugin-alsa-0.0.3a2/ovos_PHAL_plugin_alsa/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    87676 2023-06-16 16:57:27.000000 ovos-PHAL-plugin-alsa-0.0.3a2/ovos_PHAL_plugin_alsa/blop-mark-diangelo.wav
+-rw-r--r--   0 runner    (1001) docker     (123)      177 2023-06-16 16:57:27.000000 ovos-PHAL-plugin-alsa-0.0.3a2/ovos_PHAL_plugin_alsa/version.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 16:57:31.303150 ovos-PHAL-plugin-alsa-0.0.3a2/ovos_PHAL_plugin_alsa.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)      963 2023-06-16 16:57:31.000000 ovos-PHAL-plugin-alsa-0.0.3a2/ovos_PHAL_plugin_alsa.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      432 2023-06-16 16:57:31.000000 ovos-PHAL-plugin-alsa-0.0.3a2/ovos_PHAL_plugin_alsa.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-16 16:57:31.000000 ovos-PHAL-plugin-alsa-0.0.3a2/ovos_PHAL_plugin_alsa.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       89 2023-06-16 16:57:31.000000 ovos-PHAL-plugin-alsa-0.0.3a2/ovos_PHAL_plugin_alsa.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       61 2023-06-16 16:57:31.000000 ovos-PHAL-plugin-alsa-0.0.3a2/ovos_PHAL_plugin_alsa.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       22 2023-06-16 16:57:31.000000 ovos-PHAL-plugin-alsa-0.0.3a2/ovos_PHAL_plugin_alsa.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-16 16:57:31.000000 ovos-PHAL-plugin-alsa-0.0.3a2/ovos_PHAL_plugin_alsa.egg-info/zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-16 16:57:31.303150 ovos-PHAL-plugin-alsa-0.0.3a2/setup.cfg
+-rwxr-xr-x   0 runner    (1001) docker     (123)     2990 2023-06-16 16:57:27.000000 ovos-PHAL-plugin-alsa-0.0.3a2/setup.py
```

### Comparing `ovos-PHAL-plugin-alsa-0.0.2a2/ovos_PHAL_plugin_alsa/__init__.py` & `ovos-PHAL-plugin-alsa-0.0.3a2/ovos_PHAL_plugin_alsa/__init__.py`

 * *Files identical despite different names*

### Comparing `ovos-PHAL-plugin-alsa-0.0.2a2/setup.py` & `ovos-PHAL-plugin-alsa-0.0.3a2/setup.py`

 * *Files 11% similar despite different names*

```diff
@@ -45,19 +45,28 @@
         requirements = f.read().splitlines()
         if 'MYCROFT_LOOSE_REQUIREMENTS' in os.environ:
             print('USING LOOSE REQUIREMENTS!')
             requirements = [r.replace('==', '>=').replace('~=', '>=') for r in requirements]
         return [pkg for pkg in requirements
                 if pkg.strip() and not pkg.startswith("#")]
 
+
+def get_description():
+    with open(os.path.join(BASEDIR, "readme.md"), "r") as f:
+        long_description = f.read()
+    return long_description
+
+
 PLUGIN_ENTRY_POINT = 'ovos-PHAL-plugin-alsa=ovos_PHAL_plugin_alsa:AlsaVolumeControlPlugin'
 setup(
     name='ovos-PHAL-plugin-alsa',
     version=get_version(),
     description='A volume control plugin for OpenVoiceOS hardware abstraction layer',
+    long_description=get_description(),
+    long_description_content_type="text/markdown",
     url='https://github.com/OpenVoiceOS/ovos-PHAL-plugin-alsa',
     author='JarbasAi',
     author_email='jarbasai@mailfence.com',
     license='Apache-2.0',
     packages=['ovos_PHAL_plugin_alsa'],
     package_data={'': package_files('ovos_PHAL_plugin_alsa')},
     install_requires=required("requirements.txt"),
```

