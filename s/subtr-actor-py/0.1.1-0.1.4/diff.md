# Comparing `tmp/subtr_actor_py-0.1.1.tar.gz` & `tmp/subtr_actor_py-0.1.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "subtr_actor_py-0.1.1.tar", max compression
+gzip compressed data
```

## Comparing `subtr_actor_py-0.1.1.tar` & `subtr_actor_py-0.1.4.tar`

### file list

```diff
@@ -1,5 +1,13 @@
--rw-r--r--   0        0        0      100 2023-06-13 08:24:40.792859 subtr_actor_py-0.1.1/README.md
--rw-r--r--   0        0        0      569 2023-06-13 09:16:20.873912 subtr_actor_py-0.1.1/pyproject.toml
--rw-r--r--   0        0        0      143 2023-06-13 08:23:53.279298 subtr_actor_py-0.1.1/subtr_actor/__init__.py
--rw-r--r--   0        0        0      543 2023-06-13 08:16:27.228171 subtr_actor_py-0.1.1/subtr_actor/subtr_actor.pyi
--rw-r--r--   0        0        0      901 1970-01-01 00:00:00.000000 subtr_actor_py-0.1.1/PKG-INFO
+-rw-r--r--   0        0        0      339 1970-01-01 00:00:00.000000 subtr_actor_py-0.1.4/Cargo.toml
+-rw-r--r--   0     1000      100       10 2023-06-13 08:24:28.000000 subtr_actor_py-0.1.4/.gitignore
+-rw-r--r--   0     1000      100      100 2023-06-13 08:24:40.000000 subtr_actor_py-0.1.4/README.md
+-rw-r--r--   0     1000      100     2978 2023-06-16 07:29:03.000000 subtr_actor_py-0.1.4/flake.lock
+-rw-r--r--   0     1000      100      930 2023-06-13 08:16:27.000000 subtr_actor_py-0.1.4/flake.nix
+-rw-r--r--   0     1000      100    50684 2023-06-16 07:58:11.000000 subtr_actor_py-0.1.4/poetry.lock
+-rw-r--r--   0     1000      100      620 2023-06-16 07:57:59.000000 subtr_actor_py-0.1.4/pyproject.toml
+-rw-r--r--   0     1000      100     7714 2023-06-16 07:53:30.000000 subtr_actor_py-0.1.4/src/lib.rs
+-rw-r--r--   0     1000      100  1565088 2023-06-16 07:21:34.000000 subtr_actor_py-0.1.4/tests/029103f9-4d58-4964-b47a-539b32f6fb33.replay
+-rw-r--r--   0     1000      100       73 2023-06-16 07:25:57.000000 subtr_actor_py-0.1.4/tests/__init__.py
+-rw-r--r--   0     1000      100      226 2023-06-16 07:26:02.000000 subtr_actor_py-0.1.4/tests/test_filepath_functions.py
+-rw-r--r--   0     1000      100    15492 2023-06-16 07:54:24.000000 subtr_actor_py-0.1.4/Cargo.lock
+-rw-r--r--   0        0        0      324 1970-01-01 00:00:00.000000 subtr_actor_py-0.1.4/PKG-INFO
```

### filetype from file(1)

```diff
@@ -1 +1 @@
-POSIX tar archive
+POSIX tar archive (GNU)
```

### Comparing `subtr_actor_py-0.1.1/pyproject.toml` & `subtr_actor_py-0.1.4/pyproject.toml`

 * *Files 13% similar despite different names*

```diff
@@ -1,23 +1,25 @@
 [tool.poetry]
 name = "subtr-actor-py"
-version = "0.1.1"
+version = "0.1.4"
 description = "Python bindings for the Rocket League replay processing library subtr-actor."
 authors = ["Ivan Malison <ivanmalison@gmail.com>"]
 license = "MIT"
 readme = "README.md"
 repository = "https://github.com/rlrml/subtr-actor-py"
-packages = [{include = "subtr_actor"}]
+packages = [{include = "subtr_actor", from="subtr_actor"}]
 
 [tool.poetry.dependencies]
-python = "^3.6"
+python = ">=3.7,<4.0"
 
 [tool.poetry.dev-dependencies]
 wheel = "*"
 maturin = "^0.14.2"
+pytest = "*"
+twine = "*"
 
 [tool.maturin]
 features = ["pyo3/extension-module"]
 
 [build-system]
 requires = ["maturin>=0.14,<0.15"]
 build-backend = "maturin"
```

