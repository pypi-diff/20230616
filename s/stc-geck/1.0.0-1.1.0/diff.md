# Comparing `tmp/stc-geck-1.0.0.tar.gz` & `tmp/stc-geck-1.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "stc-geck-1.0.0.tar", last modified: Tue Jun  6 07:29:26 2023, max compression
+gzip compressed data, was "stc-geck-1.1.0.tar", last modified: Fri Jun 16 10:05:20 2023, max compression
```

## Comparing `stc-geck-1.0.0.tar` & `stc-geck-1.1.0.tar`

### file list

```diff
@@ -1,17 +1,18 @@
-drwxr-xr-x   0 pasha      (501) staff       (20)        0 2023-06-06 07:29:26.338956 stc-geck-1.0.0/
--rw-r--r--   0 pasha      (501) staff       (20)       24 2022-12-01 11:19:40.000000 stc-geck-1.0.0/MANIFEST.in
--rw-r--r--   0 pasha      (501) staff       (20)      344 2023-06-06 07:29:26.338276 stc-geck-1.0.0/PKG-INFO
--rw-r--r--   0 pasha      (501) staff       (20)        0 2023-04-25 17:50:47.000000 stc-geck-1.0.0/README.md
--rw-r--r--   0 pasha      (501) staff       (20)      604 2023-06-06 07:21:34.000000 stc-geck-1.0.0/pyproject.toml
--rw-r--r--   0 pasha      (501) staff       (20)       43 2023-06-03 20:43:36.000000 stc-geck-1.0.0/requirements.txt
--rw-r--r--   0 pasha      (501) staff       (20)       38 2023-06-06 07:29:26.339148 stc-geck-1.0.0/setup.cfg
-drwxr-xr-x   0 pasha      (501) staff       (20)        0 2023-06-06 07:29:26.333789 stc-geck-1.0.0/stc_geck/
--rw-r--r--   0 pasha      (501) staff       (20)     4509 2023-06-06 07:22:47.000000 stc-geck-1.0.0/stc_geck/cli.py
--rw-r--r--   0 pasha      (501) staff       (20)     3049 2023-06-06 07:21:50.000000 stc-geck-1.0.0/stc_geck/client.py
-drwxr-xr-x   0 pasha      (501) staff       (20)        0 2023-06-06 07:29:26.337519 stc-geck-1.0.0/stc_geck.egg-info/
--rw-r--r--   0 pasha      (501) staff       (20)      344 2023-06-06 07:29:26.000000 stc-geck-1.0.0/stc_geck.egg-info/PKG-INFO
--rw-r--r--   0 pasha      (501) staff       (20)      282 2023-06-06 07:29:26.000000 stc-geck-1.0.0/stc_geck.egg-info/SOURCES.txt
--rw-r--r--   0 pasha      (501) staff       (20)        1 2023-06-06 07:29:26.000000 stc-geck-1.0.0/stc_geck.egg-info/dependency_links.txt
--rw-r--r--   0 pasha      (501) staff       (20)       47 2023-06-06 07:29:26.000000 stc-geck-1.0.0/stc_geck.egg-info/entry_points.txt
--rw-r--r--   0 pasha      (501) staff       (20)       44 2023-06-06 07:29:26.000000 stc-geck-1.0.0/stc_geck.egg-info/requires.txt
--rw-r--r--   0 pasha      (501) staff       (20)        9 2023-06-06 07:29:26.000000 stc-geck-1.0.0/stc_geck.egg-info/top_level.txt
+drwxr-xr-x   0 pasha      (501) staff       (20)        0 2023-06-16 10:05:20.395720 stc-geck-1.1.0/
+-rw-r--r--   0 pasha      (501) staff       (20)       24 2022-12-01 11:19:40.000000 stc-geck-1.1.0/MANIFEST.in
+-rw-r--r--   0 pasha      (501) staff       (20)      344 2023-06-16 10:05:20.395443 stc-geck-1.1.0/PKG-INFO
+-rw-r--r--   0 pasha      (501) staff       (20)        0 2023-04-25 17:50:47.000000 stc-geck-1.1.0/README.md
+-rw-r--r--   0 pasha      (501) staff       (20)      600 2023-06-16 10:05:02.000000 stc-geck-1.1.0/pyproject.toml
+-rw-r--r--   0 pasha      (501) staff       (20)       82 2023-06-16 08:01:51.000000 stc-geck-1.1.0/requirements.txt
+-rw-r--r--   0 pasha      (501) staff       (20)       38 2023-06-16 10:05:20.395818 stc-geck-1.1.0/setup.cfg
+drwxr-xr-x   0 pasha      (501) staff       (20)        0 2023-06-16 10:05:20.392783 stc-geck-1.1.0/stc_geck/
+-rw-r--r--   0 pasha      (501) staff       (20)     6043 2023-06-16 07:46:13.000000 stc-geck-1.1.0/stc_geck/cli.py
+-rw-r--r--   0 pasha      (501) staff       (20)     4768 2023-06-16 07:57:24.000000 stc-geck-1.1.0/stc_geck/client.py
+-rw-r--r--   0 pasha      (501) staff       (20)     1149 2023-06-15 11:53:46.000000 stc-geck-1.1.0/stc_geck/utils.py
+drwxr-xr-x   0 pasha      (501) staff       (20)        0 2023-06-16 10:05:20.395022 stc-geck-1.1.0/stc_geck.egg-info/
+-rw-r--r--   0 pasha      (501) staff       (20)      344 2023-06-16 10:05:20.000000 stc-geck-1.1.0/stc_geck.egg-info/PKG-INFO
+-rw-r--r--   0 pasha      (501) staff       (20)      300 2023-06-16 10:05:20.000000 stc-geck-1.1.0/stc_geck.egg-info/SOURCES.txt
+-rw-r--r--   0 pasha      (501) staff       (20)        1 2023-06-16 10:05:20.000000 stc-geck-1.1.0/stc_geck.egg-info/dependency_links.txt
+-rw-r--r--   0 pasha      (501) staff       (20)       43 2023-06-16 10:05:20.000000 stc-geck-1.1.0/stc_geck.egg-info/entry_points.txt
+-rw-r--r--   0 pasha      (501) staff       (20)       83 2023-06-16 10:05:20.000000 stc-geck-1.1.0/stc_geck.egg-info/requires.txt
+-rw-r--r--   0 pasha      (501) staff       (20)        9 2023-06-16 10:05:20.000000 stc-geck-1.1.0/stc_geck.egg-info/top_level.txt
```

### Comparing `stc-geck-1.0.0/pyproject.toml` & `stc-geck-1.1.0/pyproject.toml`

 * *Files 3% similar despite different names*

```diff
@@ -1,25 +1,25 @@
 [build-system]
 requires = ["setuptools<65.0"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "stc-geck"
-version = "1.0.0"
+version = "1.1.0"
 authors = [{ name = "Interdimensional Walker" }]
 description = "GECK (Garden Of Eden Creation Kit) is a toolkit for setting up and maintaning STC"
 readme = "README.md"
 requires-python = ">=3.8"
 classifiers = [
     "Programming Language :: Python :: 3.8",
 ]
 dynamic = ["dependencies"]
 
 [project.scripts]
-stc-geck = "stc_geck.cli:main"
+geck = "stc_geck.cli:main"
 
 [project.urls]
 "Homepage" = "https://github.com/nexus-stc/stc"
 
 [tool.setuptools.dynamic]
 dependencies = {file = ["requirements.txt"]}
```

### Comparing `stc-geck-1.0.0/stc_geck/cli.py` & `stc-geck-1.1.0/stc_geck/cli.py`

 * *Files 23% similar despite different names*

```diff
@@ -1,9 +1,10 @@
 #!/usr/bin/env python3
 import json
+import logging
 import os.path
 import sys
 
 import fire
 from termcolor import colored
 
 from .client import StcGeck
@@ -21,54 +22,68 @@
     def __init__(self, query):
         self.query = query
 
     def __str__(self):
         return f'CidNotFound(query="{self.query}")'
 
 
-class StcGeckCli(StcGeck):
-    default_default_fields = {
-        'nexus_science': ['title', 'abstract', ],
-        'nexus_books': ['title', ],
-    }
-
+class StcGeckCli:
     def __init__(
-            self,
-            ipfs_http_endpoint: str = 'http://127.0.0.1:8080',
-            index_name: str = 'nexus_science',
-            timeout: int = 600,
+        self,
+        ipfs_http_endpoint: str,
+        ipfs_data_directory: str,
+        index_alias: str,
+        grpc_api_endpoint: str,
+        embed: bool,
+        timeout: int,
     ):
-        super().__init__(ipfs_http_endpoint=ipfs_http_endpoint,
-                         paths=(f'/ipns/standard-template-construct.org/data/{index_name}/',))
-        self.index_name = index_name
+        self.geck = StcGeck(
+            ipfs_http_base_url=ipfs_http_endpoint,
+            ipfs_data_directory=ipfs_data_directory,
+            index_aliases=(index_alias,),
+            grpc_api_endpoint=grpc_api_endpoint,
+            embed=embed,
+        )
+        self.index_alias = index_alias
         self.timeout = timeout
 
     async def search(self, query: str, limit: int = 1):
         """
         Searches in STC using default Summa match queries.
         Examples: `doi:10.1234/abc, isbns:9781234567890, "fetal hemoglobin"`
 
         :param query: query in Summa match format
         :param limit: how many results to return, higher values incurs LARGE performance penalty.
 
         :return: metadata records
         """
-        print(f"{colored('INFO', 'green')}: Setting up indices: {', '.join(self.paths)}...")
-        await self.start()
-        print(f"{colored('INFO', 'green')}: Searching {query}...")
-        response = await super().search([{
-            "index_alias": self.index_name,
-            "query": {
-                "match": {"value": query, "default_fields": self.default_default_fields[self.index_name],
-                          'field_boosts': {}}},
-            "collectors": [{"top_docs": {"limit": limit}}],
-            "is_fieldnorms_scoring_enabled": False,
-        }])
-        return list(
-            map(lambda x: json.loads(x.document), response.collector_outputs[0].documents.scored_documents))
+        print(f"{colored('INFO', 'green')}: Setting up indices: {self.index_alias}...")
+        async with self.geck as geck:
+            print(f"{colored('INFO', 'green')}: Searching {query}...")
+            response = await geck.get_summa_client().search([{
+                "index_alias": self.index_alias,
+                "query": {
+                    "match": {"value": query}
+                },
+                "collectors": [{"top_docs": {"limit": limit}}],
+                "is_fieldnorms_scoring_enabled": False,
+            }])
+            documents = list(map(lambda x: json.loads(x.document), response.collector_outputs[0].documents.scored_documents))
+            return documents
+
+    async def documents(self):
+        """
+        Stream all STC documents.
+
+        :return: metadata records
+        """
+        print(f"{colored('INFO', 'green')}: Setting up indices: {self.index_alias}...")
+        async with self.geck as geck:
+            async for document in geck.get_summa_client().documents(self.index_alias):
+                print(document)
 
     async def download(self, query: str, output_path: str):
         """
         Download file from STC using default Summa match queries.
         Examples: `doi:10.1234/abc, isbns:9781234567890`
 
         :param query: query in Summa match format
@@ -84,44 +99,71 @@
             if 'cid' in results[0]:
                 print(f"{colored('INFO', 'green')}: Receiving file {query}...")
                 if (real_extension := results[0].get('extension', 'pdf')) != output_path_ext:
                     print(
                         f"{colored('WARN', 'yellow')}: Receiving file extension `{real_extension}` "
                         f"is not matching with your output path extension `{output_path_ext}`. Changed to correct one.")
                     output_path_ext = real_extension
-                data = await super().download(results[0]["cid"], self.timeout)
+                data = await self.geck.download(results[0]["cid"], self.timeout)
                 final_file_name = output_path + '.' + output_path_ext
                 with open(final_file_name, 'wb') as f:
                     f.write(data)
                     f.close()
                     print(f"{colored('INFO', 'green')}: File {final_file_name} is written")
             else:
                 print(f"{colored('ERROR', 'red')}: Not found CID for {query}", file=sys.stderr)
         else:
             print(f"{colored('ERROR', 'red')}: Not found {query}", file=sys.stderr)
 
+    async def create_ipfs_directory(self, output_car: str, query: str = None, limit: int = 100):
+        """
+        Stream all STC documents.
+
+        :return: metadata records
+        """
+        print(f"{colored('INFO', 'green')}: Setting up indices: {self.index_alias}...")
+        async with self.geck as geck:
+            return await geck.create_ipfs_directory(self.index_alias, output_car, query, limit)
+
 
 async def stc_geck_cli(
-        ipfs_http_endpoint: str = 'http://127.0.0.1:8080',
-        index_name: str = 'nexus_science',
-        timeout: int = 600
+    ipfs_http_endpoint: str = 'http://127.0.0.1:8080',
+    ipfs_data_directory: str = '/ipns/standard-template-construct.org/data/',
+    index_alias: str = 'nexus_books',
+    grpc_api_endpoint: str = '127.0.0.1:37082',
+    embed: bool = True,
+    timeout: int = 600,
+    debug: bool = False,
 ):
     """
-
     :param ipfs_http_endpoint: IPFS HTTP API Endpoint
-    :param index_name: `nexus_books` (similar to LibGen) or `nexus_science` (similar to Crossref)
+    :param ipfs_data_directory: path to the directory with index
+    :param index_alias: `nexus_books` (similar to LibGen) or `nexus_science` (similar to Crossref)
+    :param grpc_api_endpoint: port used for Summa
+    :param embed: setup embedded Summa server
     :param timeout: timeout for requests to IPFS
+    :param debug: add debugging output
     :return:
     """
-    stc_geck_client = StcGeckCli(ipfs_http_endpoint, index_name, timeout)
+    logging.basicConfig(stream=sys.stdout, level=logging.INFO if debug else logging.ERROR)
+    stc_geck_client = StcGeckCli(
+        ipfs_http_endpoint=ipfs_http_endpoint,
+        ipfs_data_directory=ipfs_data_directory,
+        index_alias=index_alias,
+        grpc_api_endpoint=grpc_api_endpoint,
+        embed=embed,
+        timeout=timeout,
+    )
     return {
         'search': stc_geck_client.search,
         'download': stc_geck_client.download,
+        'documents': stc_geck_client.documents,
+        'create-ipfs-directory': stc_geck_client.create_ipfs_directory,
     }
 
 
 def main():
-    fire.Fire(stc_geck_cli, name='stc-geck')
+    fire.Fire(stc_geck_cli, name='geck')
 
 
 if __name__ == '__main__':
     main()
```

