# Comparing `tmp/zen-models-0.0.1.tar.gz` & `tmp/zen_models-0.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "zen-models-0.0.1.tar", last modified: Thu Jun 15 11:34:02 2023, max compression
+gzip compressed data, was "zen_models-0.0.2.tar", last modified: Fri Jun 16 06:08:11 2023, max compression
```

## Comparing `zen-models-0.0.1.tar` & `zen_models-0.0.2.tar`

### file list

```diff
@@ -1,12 +1,14 @@
-drwxr-xr-x   0 ravivats   (501) staff       (20)        0 2023-06-15 11:34:02.091145 zen-models-0.0.1/
--rw-r--r--   0 ravivats   (501) staff       (20)      160 2023-06-15 11:34:02.091192 zen-models-0.0.1/PKG-INFO
--rw-r--r--   0 ravivats   (501) staff       (20)      183 2023-06-15 08:49:53.000000 zen-models-0.0.1/README.txt
--rw-r--r--   0 ravivats   (501) staff       (20)      107 2023-06-15 11:34:02.091389 zen-models-0.0.1/setup.cfg
--rw-r--r--   0 ravivats   (501) staff       (20)      423 2023-06-15 11:03:45.000000 zen-models-0.0.1/setup.py
-drwxr-xr-x   0 ravivats   (501) staff       (20)        0 2023-06-15 11:34:02.089910 zen-models-0.0.1/src/
-drwxr-xr-x   0 ravivats   (501) staff       (20)        0 2023-06-15 11:34:02.091042 zen-models-0.0.1/src/zen_models.egg-info/
--rw-r--r--   0 ravivats   (501) staff       (20)      160 2023-06-15 11:34:02.000000 zen-models-0.0.1/src/zen_models.egg-info/PKG-INFO
--rw-r--r--   0 ravivats   (501) staff       (20)      218 2023-06-15 11:34:02.000000 zen-models-0.0.1/src/zen_models.egg-info/SOURCES.txt
--rw-r--r--   0 ravivats   (501) staff       (20)        1 2023-06-15 11:34:02.000000 zen-models-0.0.1/src/zen_models.egg-info/dependency_links.txt
--rw-r--r--   0 ravivats   (501) staff       (20)       19 2023-06-15 11:34:02.000000 zen-models-0.0.1/src/zen_models.egg-info/requires.txt
--rw-r--r--   0 ravivats   (501) staff       (20)        1 2023-06-15 11:34:02.000000 zen-models-0.0.1/src/zen_models.egg-info/top_level.txt
+drwxr-xr-x   0 ravivats   (501) staff       (20)        0 2023-06-16 06:08:11.605618 zen_models-0.0.2/
+-rw-r--r--   0 ravivats   (501) staff       (20)      396 2023-06-16 06:08:11.605672 zen_models-0.0.2/PKG-INFO
+-rw-r--r--   0 ravivats   (501) staff       (20)      183 2023-06-15 08:49:53.000000 zen_models-0.0.2/README.txt
+-rw-r--r--   0 ravivats   (501) staff       (20)      107 2023-06-16 06:08:11.605882 zen_models-0.0.2/setup.cfg
+-rw-r--r--   0 ravivats   (501) staff       (20)      531 2023-06-16 06:03:52.000000 zen_models-0.0.2/setup.py
+drwxr-xr-x   0 ravivats   (501) staff       (20)        0 2023-06-16 06:08:11.604401 zen_models-0.0.2/zen_models/
+-rw-r--r--   0 ravivats   (501) staff       (20)        0 2023-06-15 07:38:38.000000 zen_models-0.0.2/zen_models/__init__.py
+-rw-r--r--   0 ravivats   (501) staff       (20)    57783 2023-06-15 12:00:23.000000 zen_models-0.0.2/zen_models/zen_models.py
+drwxr-xr-x   0 ravivats   (501) staff       (20)        0 2023-06-16 06:08:11.605487 zen_models-0.0.2/zen_models.egg-info/
+-rw-r--r--   0 ravivats   (501) staff       (20)      396 2023-06-16 06:08:11.000000 zen_models-0.0.2/zen_models.egg-info/PKG-INFO
+-rw-r--r--   0 ravivats   (501) staff       (20)      246 2023-06-16 06:08:11.000000 zen_models-0.0.2/zen_models.egg-info/SOURCES.txt
+-rw-r--r--   0 ravivats   (501) staff       (20)        1 2023-06-16 06:08:11.000000 zen_models-0.0.2/zen_models.egg-info/dependency_links.txt
+-rw-r--r--   0 ravivats   (501) staff       (20)       11 2023-06-16 06:08:11.000000 zen_models-0.0.2/zen_models.egg-info/requires.txt
+-rw-r--r--   0 ravivats   (501) staff       (20)       11 2023-06-16 06:08:11.000000 zen_models-0.0.2/zen_models.egg-info/top_level.txt
```

