# Comparing `tmp/stc-geck-1.1.0.tar.gz` & `tmp/stc-geck-1.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "stc-geck-1.1.0.tar", last modified: Fri Jun 16 10:05:20 2023, max compression
+gzip compressed data, was "stc-geck-1.1.1.tar", last modified: Fri Jun 16 13:34:46 2023, max compression
```

## Comparing `stc-geck-1.1.0.tar` & `stc-geck-1.1.1.tar`

### file list

```diff
@@ -1,18 +1,18 @@
-drwxr-xr-x   0 pasha      (501) staff       (20)        0 2023-06-16 10:05:20.395720 stc-geck-1.1.0/
--rw-r--r--   0 pasha      (501) staff       (20)       24 2022-12-01 11:19:40.000000 stc-geck-1.1.0/MANIFEST.in
--rw-r--r--   0 pasha      (501) staff       (20)      344 2023-06-16 10:05:20.395443 stc-geck-1.1.0/PKG-INFO
--rw-r--r--   0 pasha      (501) staff       (20)        0 2023-04-25 17:50:47.000000 stc-geck-1.1.0/README.md
--rw-r--r--   0 pasha      (501) staff       (20)      600 2023-06-16 10:05:02.000000 stc-geck-1.1.0/pyproject.toml
--rw-r--r--   0 pasha      (501) staff       (20)       82 2023-06-16 08:01:51.000000 stc-geck-1.1.0/requirements.txt
--rw-r--r--   0 pasha      (501) staff       (20)       38 2023-06-16 10:05:20.395818 stc-geck-1.1.0/setup.cfg
-drwxr-xr-x   0 pasha      (501) staff       (20)        0 2023-06-16 10:05:20.392783 stc-geck-1.1.0/stc_geck/
--rw-r--r--   0 pasha      (501) staff       (20)     6043 2023-06-16 07:46:13.000000 stc-geck-1.1.0/stc_geck/cli.py
--rw-r--r--   0 pasha      (501) staff       (20)     4768 2023-06-16 07:57:24.000000 stc-geck-1.1.0/stc_geck/client.py
--rw-r--r--   0 pasha      (501) staff       (20)     1149 2023-06-15 11:53:46.000000 stc-geck-1.1.0/stc_geck/utils.py
-drwxr-xr-x   0 pasha      (501) staff       (20)        0 2023-06-16 10:05:20.395022 stc-geck-1.1.0/stc_geck.egg-info/
--rw-r--r--   0 pasha      (501) staff       (20)      344 2023-06-16 10:05:20.000000 stc-geck-1.1.0/stc_geck.egg-info/PKG-INFO
--rw-r--r--   0 pasha      (501) staff       (20)      300 2023-06-16 10:05:20.000000 stc-geck-1.1.0/stc_geck.egg-info/SOURCES.txt
--rw-r--r--   0 pasha      (501) staff       (20)        1 2023-06-16 10:05:20.000000 stc-geck-1.1.0/stc_geck.egg-info/dependency_links.txt
--rw-r--r--   0 pasha      (501) staff       (20)       43 2023-06-16 10:05:20.000000 stc-geck-1.1.0/stc_geck.egg-info/entry_points.txt
--rw-r--r--   0 pasha      (501) staff       (20)       83 2023-06-16 10:05:20.000000 stc-geck-1.1.0/stc_geck.egg-info/requires.txt
--rw-r--r--   0 pasha      (501) staff       (20)        9 2023-06-16 10:05:20.000000 stc-geck-1.1.0/stc_geck.egg-info/top_level.txt
+drwxr-xr-x   0 pasha      (501) staff       (20)        0 2023-06-16 13:34:46.205801 stc-geck-1.1.1/
+-rw-r--r--   0 pasha      (501) staff       (20)       24 2022-12-01 11:19:40.000000 stc-geck-1.1.1/MANIFEST.in
+-rw-r--r--   0 pasha      (501) staff       (20)      344 2023-06-16 13:34:46.205529 stc-geck-1.1.1/PKG-INFO
+-rw-r--r--   0 pasha      (501) staff       (20)        0 2023-04-25 17:50:47.000000 stc-geck-1.1.1/README.md
+-rw-r--r--   0 pasha      (501) staff       (20)      600 2023-06-16 13:34:19.000000 stc-geck-1.1.1/pyproject.toml
+-rw-r--r--   0 pasha      (501) staff       (20)       82 2023-06-16 08:01:51.000000 stc-geck-1.1.1/requirements.txt
+-rw-r--r--   0 pasha      (501) staff       (20)       38 2023-06-16 13:34:46.205904 stc-geck-1.1.1/setup.cfg
+drwxr-xr-x   0 pasha      (501) staff       (20)        0 2023-06-16 13:34:46.202698 stc-geck-1.1.1/stc_geck/
+-rw-r--r--   0 pasha      (501) staff       (20)     6043 2023-06-16 07:46:13.000000 stc-geck-1.1.1/stc_geck/cli.py
+-rw-r--r--   0 pasha      (501) staff       (20)     4762 2023-06-16 13:34:11.000000 stc-geck-1.1.1/stc_geck/client.py
+-rw-r--r--   0 pasha      (501) staff       (20)     1149 2023-06-15 11:53:46.000000 stc-geck-1.1.1/stc_geck/utils.py
+drwxr-xr-x   0 pasha      (501) staff       (20)        0 2023-06-16 13:34:46.204996 stc-geck-1.1.1/stc_geck.egg-info/
+-rw-r--r--   0 pasha      (501) staff       (20)      344 2023-06-16 13:34:46.000000 stc-geck-1.1.1/stc_geck.egg-info/PKG-INFO
+-rw-r--r--   0 pasha      (501) staff       (20)      300 2023-06-16 13:34:46.000000 stc-geck-1.1.1/stc_geck.egg-info/SOURCES.txt
+-rw-r--r--   0 pasha      (501) staff       (20)        1 2023-06-16 13:34:46.000000 stc-geck-1.1.1/stc_geck.egg-info/dependency_links.txt
+-rw-r--r--   0 pasha      (501) staff       (20)       43 2023-06-16 13:34:46.000000 stc-geck-1.1.1/stc_geck.egg-info/entry_points.txt
+-rw-r--r--   0 pasha      (501) staff       (20)       83 2023-06-16 13:34:46.000000 stc-geck-1.1.1/stc_geck.egg-info/requires.txt
+-rw-r--r--   0 pasha      (501) staff       (20)        9 2023-06-16 13:34:46.000000 stc-geck-1.1.1/stc_geck.egg-info/top_level.txt
```

### Comparing `stc-geck-1.1.0/pyproject.toml` & `stc-geck-1.1.1/pyproject.toml`

 * *Files 18% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools<65.0"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "stc-geck"
-version = "1.1.0"
+version = "1.1.1"
 authors = [{ name = "Interdimensional Walker" }]
 description = "GECK (Garden Of Eden Creation Kit) is a toolkit for setting up and maintaning STC"
 readme = "README.md"
 requires-python = ">=3.8"
 classifiers = [
     "Programming Language :: Python :: 3.8",
 ]
```

### Comparing `stc-geck-1.1.0/stc_geck/cli.py` & `stc-geck-1.1.1/stc_geck/cli.py`

 * *Files identical despite different names*

### Comparing `stc-geck-1.1.0/stc_geck/client.py` & `stc-geck-1.1.1/stc_geck/client.py`

 * *Files 2% similar despite different names*

```diff
@@ -96,15 +96,15 @@
                     'method': 'GET',
                     'url_template': f'{full_path}{{file_name}}',
                     'headers_template': headers_template,
                     'cache_config': {'cache_size': 536870912},
                 }}
                 if host_header := await detect_host_header(full_path):
                     headers_template['host'] = host_header
-                server_config['core']['index_aliases'][index] = {
+                server_config['core']['indices'][index] = {
                     'query_parser_config': query_parser_config,
                     'config': remote_index_config,
                     'field_triggers': {},
                 }
             self.summa_embed_server = summa_embed.SummaEmbedServerBin(server_config)
             await self.summa_embed_server.start()
         await self.summa_client.start()
```

### Comparing `stc-geck-1.1.0/stc_geck/utils.py` & `stc-geck-1.1.1/stc_geck/utils.py`

 * *Files identical despite different names*

