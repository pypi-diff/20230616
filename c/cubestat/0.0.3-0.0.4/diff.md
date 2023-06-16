# Comparing `tmp/cubestat-0.0.3.tar.gz` & `tmp/cubestat-0.0.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "cubestat-0.0.3.tar", last modified: Thu Jun 15 02:34:08 2023, max compression
+gzip compressed data, was "cubestat-0.0.4.tar", last modified: Fri Jun 16 01:06:54 2023, max compression
```

## Comparing `cubestat-0.0.3.tar` & `cubestat-0.0.4.tar`

### file list

```diff
@@ -1,16 +1,18 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 02:34:08.900593 cubestat-0.0.3/
--rw-r--r--   0 runner    (1001) docker     (123)     1076 2023-06-15 02:33:53.000000 cubestat-0.0.3/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)      338 2023-06-15 02:34:08.900593 cubestat-0.0.3/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     3023 2023-06-15 02:33:53.000000 cubestat-0.0.3/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 02:34:08.900593 cubestat-0.0.3/cubestat/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-15 02:33:53.000000 cubestat-0.0.3/cubestat/__init__.py
--rwxr-xr-x   0 runner    (1001) docker     (123)    15826 2023-06-15 02:33:53.000000 cubestat-0.0.3/cubestat/cubestat.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 02:34:08.900593 cubestat-0.0.3/cubestat.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)      338 2023-06-15 02:34:08.000000 cubestat-0.0.3/cubestat.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      262 2023-06-15 02:34:08.000000 cubestat-0.0.3/cubestat.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-15 02:34:08.000000 cubestat-0.0.3/cubestat.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       52 2023-06-15 02:34:08.000000 cubestat-0.0.3/cubestat.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)       14 2023-06-15 02:34:08.000000 cubestat-0.0.3/cubestat.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        9 2023-06-15 02:34:08.000000 cubestat-0.0.3/cubestat.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-15 02:34:08.900593 cubestat-0.0.3/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)      587 2023-06-15 02:33:53.000000 cubestat-0.0.3/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 01:06:54.213167 cubestat-0.0.4/
+-rw-r--r--   0 runner    (1001) docker     (123)     1076 2023-06-16 01:06:44.000000 cubestat-0.0.4/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)      338 2023-06-16 01:06:54.213167 cubestat-0.0.4/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     3024 2023-06-16 01:06:44.000000 cubestat-0.0.4/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 01:06:54.213167 cubestat-0.0.4/cubestat/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-16 01:06:44.000000 cubestat-0.0.4/cubestat/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1641 2023-06-16 01:06:44.000000 cubestat-0.0.4/cubestat/apple_reader.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)    10901 2023-06-16 01:06:44.000000 cubestat-0.0.4/cubestat/cubestat.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2685 2023-06-16 01:06:44.000000 cubestat-0.0.4/cubestat/linux_reader.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 01:06:54.213167 cubestat-0.0.4/cubestat.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)      338 2023-06-16 01:06:54.000000 cubestat-0.0.4/cubestat.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      312 2023-06-16 01:06:54.000000 cubestat-0.0.4/cubestat.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-16 01:06:54.000000 cubestat-0.0.4/cubestat.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       52 2023-06-16 01:06:54.000000 cubestat-0.0.4/cubestat.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       52 2023-06-16 01:06:54.000000 cubestat-0.0.4/cubestat.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        9 2023-06-16 01:06:54.000000 cubestat-0.0.4/cubestat.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-16 01:06:54.213167 cubestat-0.0.4/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      645 2023-06-16 01:06:44.000000 cubestat-0.0.4/setup.py
```

### Comparing `cubestat-0.0.3/LICENSE` & `cubestat-0.0.4/LICENSE`

 * *Files identical despite different names*

### Comparing `cubestat-0.0.3/README.md` & `cubestat-0.0.4/README.md`

 * *Files 4% similar despite different names*

```diff
@@ -63,8 +63,8 @@
 We can see model training (on GPU), self-play (done on 4 performance CPU cores) and model evaluation, which runs inference on Neural Engine:
 ![Self-play + training + eval](static/selfplay.png)
 
 Another example running [GPT inference on ggml](https://github.com/ggerganov/ggml): 
 ![GPT inference](static/ggml_gpt.png)
 
 Multi-gpu example - training [nano GPT](https://github.com/karpathy/nanoGPT) on 4 GPU instance:
-![nanoGPT](static/ggml_gpt.png)
+![multigpu](static/multigpu.png)
```

### Comparing `cubestat-0.0.3/setup.py` & `cubestat-0.0.4/setup.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,18 +1,21 @@
 from setuptools import setup, find_packages
 
 setup(
     name='cubestat',
-    version='0.0.3',
+    version='0.0.4',
     author='Oleksandr Kuvshynov',
     author_email='okuvshynov@gmail.com',
     description='Horizon chart in terminal for CPU/GPU/ANE monitoring',
     long_description='Horizon chart in terminal. Supports CPU/GPU/ANE monitoring for Apple M1/M2, nVidia GPUs',
     packages=find_packages(),
-    install_requires=['psutil>=5.9.5'],
+    install_requires=[
+        'psutil>=5.9.5',
+        'pynvml; platform_system=="Linux"'
+    ],
     url='https://github.com/okuvshynov/cubestat',
     entry_points={
         'console_scripts': [
             'cubestat = cubestat.cubestat:main'
         ]
     },
 )
```

