# Comparing `tmp/papis-zotero-0.1.1.linux-x86_64.tar.gz` & `tmp/papis-zotero-0.1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "papis-zotero-0.1.1.linux-x86_64.tar", last modified: Tue May  9 20:09:28 2023, max compression
+gzip compressed data, was "papis-zotero-0.1.2.tar", last modified: Fri Jun 16 11:35:28 2023, max compression
```

## Comparing `papis-zotero-0.1.1.linux-x86_64.tar` & `papis-zotero-0.1.2.tar`

### file list

```diff
@@ -1,28 +1,22 @@
-drwxr-xr-x   0 gallo     (1000) users      (100)        0 2023-05-09 20:09:28.367884 ./
-drwxr-xr-x   0 gallo     (1000) users      (100)        0 2023-05-09 20:09:28.367884 ./home/
-drwxr-xr-x   0 gallo     (1000) users      (100)        0 2023-05-09 20:09:28.368884 ./home/gallo/
-drwxr-xr-x   0 gallo     (1000) users      (100)        0 2023-05-09 20:09:28.368884 ./home/gallo/software/
-drwxr-xr-x   0 gallo     (1000) users      (100)        0 2023-05-09 20:09:28.368884 ./home/gallo/software/papis/
-drwxr-xr-x   0 gallo     (1000) users      (100)        0 2023-05-09 20:09:28.368884 ./home/gallo/software/papis/env/
-drwxr-xr-x   0 gallo     (1000) users      (100)        0 2023-05-09 20:09:28.368884 ./home/gallo/software/papis/env/lib/
-drwxr-xr-x   0 gallo     (1000) users      (100)        0 2023-05-09 20:09:28.368884 ./home/gallo/software/papis/env/lib/python3.10/
-drwxr-xr-x   0 gallo     (1000) users      (100)        0 2023-05-09 20:09:28.490883 ./home/gallo/software/papis/env/lib/python3.10/site-packages/
-drwxr-xr-x   0 gallo     (1000) users      (100)        0 2023-05-09 20:09:28.371884 ./home/gallo/software/papis/env/lib/python3.10/site-packages/papis_zotero/
--rw-r--r--   0 gallo     (1000) users      (100)     2214 2023-05-09 19:52:11.000000 ./home/gallo/software/papis/env/lib/python3.10/site-packages/papis_zotero/__init__.py
-drwxr-xr-x   0 gallo     (1000) users      (100)        0 2023-05-09 20:09:28.375884 ./home/gallo/software/papis/env/lib/python3.10/site-packages/papis_zotero/__pycache__/
--rw-r--r--   0 gallo     (1000) users      (100)     2129 2023-05-09 20:09:28.373885 ./home/gallo/software/papis/env/lib/python3.10/site-packages/papis_zotero/__pycache__/__init__.cpython-310.pyc
--rw-r--r--   0 gallo     (1000) users      (100)     1731 2023-05-09 20:09:28.371884 ./home/gallo/software/papis/env/lib/python3.10/site-packages/papis_zotero/__pycache__/bibtex.cpython-310.pyc
--rw-r--r--   0 gallo     (1000) users      (100)     6999 2023-05-09 20:09:28.373885 ./home/gallo/software/papis/env/lib/python3.10/site-packages/papis_zotero/__pycache__/server.cpython-310.pyc
--rw-r--r--   0 gallo     (1000) users      (100)     7043 2023-05-09 20:09:28.375884 ./home/gallo/software/papis/env/lib/python3.10/site-packages/papis_zotero/__pycache__/sql.cpython-310.pyc
--rw-r--r--   0 gallo     (1000) users      (100)      484 2023-05-09 20:09:28.374884 ./home/gallo/software/papis/env/lib/python3.10/site-packages/papis_zotero/__pycache__/utils.cpython-310.pyc
--rw-r--r--   0 gallo     (1000) users      (100)     2215 2023-05-09 20:06:28.000000 ./home/gallo/software/papis/env/lib/python3.10/site-packages/papis_zotero/bibtex.py
--rw-r--r--   0 gallo     (1000) users      (100)     7952 2023-05-09 20:05:33.000000 ./home/gallo/software/papis/env/lib/python3.10/site-packages/papis_zotero/server.py
--rw-r--r--   0 gallo     (1000) users      (100)     9385 2023-05-09 20:04:40.000000 ./home/gallo/software/papis/env/lib/python3.10/site-packages/papis_zotero/sql.py
--rw-r--r--   0 gallo     (1000) users      (100)      230 2023-05-09 19:34:06.000000 ./home/gallo/software/papis/env/lib/python3.10/site-packages/papis_zotero/utils.py
-drwxr-xr-x   0 gallo     (1000) users      (100)        0 2023-05-09 20:09:28.491883 ./home/gallo/software/papis/env/lib/python3.10/site-packages/papis_zotero-0.1.1-py3.10.egg-info/
--rw-r--r--   0 gallo     (1000) users      (100)     4912 2023-05-09 20:09:28.457883 ./home/gallo/software/papis/env/lib/python3.10/site-packages/papis_zotero-0.1.1-py3.10.egg-info/PKG-INFO
--rw-r--r--   0 gallo     (1000) users      (100)      350 2023-05-09 20:09:28.490883 ./home/gallo/software/papis/env/lib/python3.10/site-packages/papis_zotero-0.1.1-py3.10.egg-info/SOURCES.txt
--rw-r--r--   0 gallo     (1000) users      (100)        1 2023-05-09 20:09:28.458883 ./home/gallo/software/papis/env/lib/python3.10/site-packages/papis_zotero-0.1.1-py3.10.egg-info/dependency_links.txt
--rw-r--r--   0 gallo     (1000) users      (100)       43 2023-05-09 20:09:28.458883 ./home/gallo/software/papis/env/lib/python3.10/site-packages/papis_zotero-0.1.1-py3.10.egg-info/entry_points.txt
--rw-r--r--   0 gallo     (1000) users      (100)       12 2023-05-09 20:09:28.458883 ./home/gallo/software/papis/env/lib/python3.10/site-packages/papis_zotero-0.1.1-py3.10.egg-info/requires.txt
--rw-r--r--   0 gallo     (1000) users      (100)       13 2023-05-09 20:09:28.458883 ./home/gallo/software/papis/env/lib/python3.10/site-packages/papis_zotero-0.1.1-py3.10.egg-info/top_level.txt
+drwxr-xr-x   0 gallo     (1000) users      (100)        0 2023-06-16 11:35:28.530495 papis-zotero-0.1.2/
+-rw-r--r--   0 gallo     (1000) users      (100)     5391 2023-06-16 11:35:28.531495 papis-zotero-0.1.2/PKG-INFO
+-rw-r--r--   0 gallo     (1000) users      (100)     4203 2023-06-16 11:33:17.000000 papis-zotero-0.1.2/README.rst
+drwxr-xr-x   0 gallo     (1000) users      (100)        0 2023-06-16 11:35:28.528495 papis-zotero-0.1.2/papis_zotero/
+-rw-r--r--   0 gallo     (1000) users      (100)     3438 2023-06-16 11:33:17.000000 papis-zotero-0.1.2/papis_zotero/__init__.py
+-rw-r--r--   0 gallo     (1000) users      (100)     2029 2023-06-16 11:33:17.000000 papis-zotero-0.1.2/papis_zotero/bibtex.py
+-rw-r--r--   0 gallo     (1000) users      (100)     6840 2023-06-16 11:33:17.000000 papis-zotero-0.1.2/papis_zotero/server.py
+-rw-r--r--   0 gallo     (1000) users      (100)     9124 2023-06-16 11:33:17.000000 papis-zotero-0.1.2/papis_zotero/sql.py
+-rw-r--r--   0 gallo     (1000) users      (100)     4260 2023-06-16 11:33:17.000000 papis-zotero-0.1.2/papis_zotero/utils.py
+drwxr-xr-x   0 gallo     (1000) users      (100)        0 2023-06-16 11:35:28.530495 papis-zotero-0.1.2/papis_zotero.egg-info/
+-rw-r--r--   0 gallo     (1000) users      (100)     5391 2023-06-16 11:35:28.000000 papis-zotero-0.1.2/papis_zotero.egg-info/PKG-INFO
+-rw-r--r--   0 gallo     (1000) users      (100)      416 2023-06-16 11:35:28.000000 papis-zotero-0.1.2/papis_zotero.egg-info/SOURCES.txt
+-rw-r--r--   0 gallo     (1000) users      (100)        1 2023-06-16 11:35:28.000000 papis-zotero-0.1.2/papis_zotero.egg-info/dependency_links.txt
+-rw-r--r--   0 gallo     (1000) users      (100)       43 2023-06-16 11:35:28.000000 papis-zotero-0.1.2/papis_zotero.egg-info/entry_points.txt
+-rw-r--r--   0 gallo     (1000) users      (100)      140 2023-06-16 11:35:28.000000 papis-zotero-0.1.2/papis_zotero.egg-info/requires.txt
+-rw-r--r--   0 gallo     (1000) users      (100)       13 2023-06-16 11:35:28.000000 papis-zotero-0.1.2/papis_zotero.egg-info/top_level.txt
+-rw-r--r--   0 gallo     (1000) users      (100)      479 2023-06-16 11:35:28.531495 papis-zotero-0.1.2/setup.cfg
+-rw-r--r--   0 gallo     (1000) users      (100)     1916 2023-06-16 11:34:25.000000 papis-zotero-0.1.2/setup.py
+drwxr-xr-x   0 gallo     (1000) users      (100)        0 2023-06-16 11:35:28.530495 papis-zotero-0.1.2/tests/
+-rw-r--r--   0 gallo     (1000) users      (100)     1160 2023-06-16 11:33:17.000000 papis-zotero-0.1.2/tests/test_bibtex.py
+-rw-r--r--   0 gallo     (1000) users      (100)      985 2023-06-16 11:33:17.000000 papis-zotero-0.1.2/tests/test_sql.py
+-rw-r--r--   0 gallo     (1000) users      (100)     8126 2023-06-16 11:33:17.000000 papis-zotero-0.1.2/tests/testlib.py
```

### Comparing `./home/gallo/software/papis/env/lib/python3.10/site-packages/papis_zotero/server.py` & `papis-zotero-0.1.2/papis_zotero/server.py`

 * *Files 21% similar despite different names*

```diff
@@ -1,252 +1,216 @@
-#! /usr/bin/env python3
-# -*- coding: utf-8 -*-
 """Start a web server listening on port 23119. This server is
 compatible with the `zotero connector`. This means that if zotero is
 *not* running, you can have items from your web browser added directly
 into papis.
 
 """
 
-import papis_zotero.utils
+import json
+import http.server
+from typing import Any, Dict, List
 
 import papis.api
-import papis.config
+import papis.crossref
 import papis.document
 import papis.commands.add
-import papis.crossref
+import papis.logging
 
-import urllib.request
-import urllib.error
+import papis_zotero.utils
 
-import re
-import json
-import logging
-import tempfile
-import http.server
+logger = papis.logging.get_logger(__name__)
+
+# NOTE: 5.0.75 was released in October 8, 2019 at the same time with Python 3.8
+ZOTERO_CONNECTOR_API_VERSION = 2
+ZOTERO_VERSION = "5.0.75"
+ZOTERO_PORT = 23119
+
+_k = papis.document.KeyConversionPair
+
+ZOTERO_TO_PAPIS_CONVERSIONS = [
+    _k("creators", [{
+        "key": "author_list",
+        "action": lambda a: zotero_authors(a)
+        }]),
+    _k("tags", [{
+        "key": "tags",
+        "action": lambda t: "; ".join(tag["tag"] for tag in t)
+        }]),
+    _k("date", [
+        {"key": "year", "action": lambda d: int(d.split("-")[0])},
+        {"key": "month", "action": lambda d: int(d.split("-")[1])},
+        ]),
+    _k("archiveID", [
+        {"key": "eprint", "action": lambda a: a.split(":")[-1]}
+        ]),
+    _k("type", [
+        {"key": "type", "action": papis_zotero.utils.ZOTERO_TO_PAPIS_TYPES.get}
+        ]),
+]
+
+
+def zotero_authors(creators: List[Dict[str, str]]) -> List[Dict[str, str]]:
+    authors = []
+    for creator in creators:
+        if creator["creatorType"] != "author":
+            continue
+
+        authors.append({
+            "given": creator["firstName"],
+            "family": creator["lastName"],
+        })
 
-logger = logging.getLogger("papis:zotero:server")
-logging.basicConfig(filename="", level=logging.INFO)
+    return authors
 
-connector_api_version = 2
-zotero_version = "5.0.25"
-zotero_port = 23119
-
-papis_translation = {
-    'abstractNote': 'abstract',
-    'publicationTitle': 'journal',
-    'DOI': 'doi',
-    'itemType': 'type',
-    'ISBN': 'isbn',
-}
-
-
-def zotero_data_to_papis_data(item):
-    """
-    {
-        'itemType': 'book',
-        'language': 'en',
-        'shortTitle': 'Nuclear Collective Motion',
-        'DOI': '10.1142/6721',
-        'accessDate': '2018-07-09T22:57:55Z',
-        'extra': 'DOI: 10.1142/6721',
-        'creators': [
-            {
-                'creatorType': 'author',
-                'firstName': 'David J',
-                'lastName': 'Rowe'
-            }
-        ],
-        'publisher': 'WORLD SCIENTIFIC',
-        'ISBN': '9789812790644 9789812790668',
-        'url': 'http://www.worldscientific.com/worldscibooks/10.1142/6721',
-        'notes': [],
-        'seeAlso': [],
-        'attachments': [
-            {
-                'url': 'https://...pdf/10.1103/physrevlett.121.090503',
-                'title': 'full text pdf',
-                'mimetype': 'application/pdf'
-            },
-            {
-                'url': 'https://...pdf/10.1103/physrevlett.121.090503',
-                'title': 'aps snapshot',
-                'mimetype': 'text/html'
-            }
-        ],
-        'tags': [],
-        'date': '05/2010',
-        'libraryCatalog': 'Crossref',
-        'title': 'Nuclear Collective Motion: Models and Theory',
-        'id': 'SL2sa7hx'
-    }
-    """
-
-    data = {}
-
-    for key in papis_translation.keys():
-        if item.get(key):
-            data[papis_translation[key]] = item.get(key)
+
+def zotero_data_to_papis_data(item: Dict[str, Any]) -> Dict[str, Any]:
+    item.pop("id", None)
+    item.pop("attachments", None)
+
+    for foreign_key, key in papis_zotero.utils.ZOTERO_TO_PAPIS_FIELDS.items():
+        if foreign_key in item:
+            item[key] = item.pop(foreign_key)
+
+    item = papis.document.keyconversion_to_data(ZOTERO_TO_PAPIS_CONVERSIONS,
+                                                item,
+                                                keep_unknown_keys=True)
+    for key in papis_zotero.utils.ZOTERO_EXCLUDED_FIELDS:
+        if key in item:
             del item[key]
 
-    # Maybe zotero has good tags
-    if isinstance(item.get('tags'), list):
+    # try to get information from Crossref as well
+    if "doi" in item:
         try:
-            data['tags'] = " ".join(item['tags'])
-        except:
-            pass
-        del item['tags']
-
-    if item.get('id'):
-        del item['id']
-
-    if item.get('attachments'):
-        del item['attachments']
-
-    # still get all information from zotero
-    data.update(item)
-
-    # and also get all infromation from crossref
-    if data.get('doi'):
-        crossref_data = papis.crossref.doi_to_data(data['doi'])
-        if crossref_data.get('title'):
-            del crossref_data['title']
-        logger.info("Updating also from crossref")
-        data.update(crossref_data)
+            crossref_data = papis.crossref.doi_to_data(item["doi"])
+            crossref_data.pop("title", None)
+            logger.info("Updating document with data from Crossref.")
+        except ValueError:
+            crossref_data = {}
 
-    return data
+        item.update(crossref_data)
 
+    logger.info("Document metadata: %s", item)
+    return item
 
-class PapisRequestHandler(http.server.BaseHTTPRequestHandler):
 
-    def log_message(self, fmt, *args):
-        global logger
-        logger.info(fmt % args)
-        return
+def download_zotero_attachments(attachments: List[Dict[str, str]]) -> List[str]:
+    files = []
+
+    for attachment in attachments:
+        logger.info("Checking attachment: %s", attachment)
+
+        mime = str(attachment.get("mimeType"))
+        if mime not in papis_zotero.utils.ZOTERO_SUPPORTED_MIMETYPES_TO_EXTENSION:
+            continue
+
+        url = attachment["url"]
+        extension = papis_zotero.utils.ZOTERO_SUPPORTED_MIMETYPES_TO_EXTENSION[mime]
+        logger.info("Downloading file (%s): '%s'.", mime, url)
+
+        filename = papis_zotero.utils.download_document(
+            url, expected_document_extension=extension)
+        if filename is not None:
+            files.append(filename)
+
+    return files
+
+
+class PapisRequestHandler(http.server.BaseHTTPRequestHandler):
+    def log_message(self, fmt: str, *args: Any) -> None:
+        logger.info(fmt, *args)
 
-    def set_zotero_headers(self):
-        self.send_header("X-Zotero-Version", zotero_version)
+    def set_zotero_headers(self) -> None:
+        self.send_header("X-Zotero-Version", ZOTERO_VERSION)
         self.send_header("X-Zotero-Connector-API-Version",
-                         connector_api_version)
+                         str(ZOTERO_CONNECTOR_API_VERSION))
         self.end_headers()
 
-    def read_input(self):
-        length = int(self.headers['content-length'])
+    def read_input(self) -> bytes:
+        length = int(self.headers["content-length"])
         return self.rfile.read(length)
 
-    def pong(self, POST=True):
-        global logger
-        logger.info("pong!")
-        # Pong must respond to ping on both GET and POST
-        # It must accepts application/json and text/plain
-        if not POST:  # GET
-            logger.debug("GET request")
-            self.send_response(200)
-            self.send_header("Content-Type", "text/html")
-            self.set_zotero_headers()
-            response = '''\
-            <!DOCTYPE html>
-            <html>
-                <head>
-                    <title>Zotero Connector Server is Available</title>
-                </head>
-                <body>
-                    Zotero Connector Server is Available
-                </body>
-            </html>
-            '''
-        else:  # POST
-            logger.debug("POST request")
-            self.send_response(200)
-            self.send_header("Content-Type", "application/json")
-            self.set_zotero_headers()
-            response = json.dumps({"prefs": {"automaticSnapshots": True}})
+    def do_GET(self) -> None:  # noqa: N802
+        logger.info("Received GET request at '%s'", self.path)
+        if self.path == "/connector/ping":
+            self.handle_get_ping()
+
+    def handle_get_ping(self) -> None:
+        self.send_response(200)
+        self.send_header("Content-Type", "text/html")
+        self.set_zotero_headers()
+        response = """\
+        <!DOCTYPE html>
+        <html>
+            <head>
+                <title>Zotero Connector Server is Available</title>
+            </head>
+            <body>
+                Zotero Connector Server is Available
+            </body>
+        </html>
+        """
+
+        self.wfile.write(response.encode("utf-8"))
 
-        self.wfile.write(bytes(response, "utf8"))
+    def do_POST(self) -> None:  # noqa: N802
+        logger.info("Received POST request at '%s'", self.path)
+        if self.path == "/connector/ping":
+            self.handle_post_ping()
+        elif self.path == "/connector/getSelectedCollection":
+            self.handle_post_collection()
+        elif self.path == "/connector/saveSnapshot":
+            self.handle_post_snapshot()
+        elif self.path == "/connector/saveItems":
+            self.handle_post_add()
 
-    def papis_collection(self):
+    def handle_post_ping(self) -> None:
+        self.send_response(200)
+        self.send_header("Content-Type", "application/json")
+        self.set_zotero_headers()
+        response = json.dumps({"prefs": {"automaticSnapshots": True}})
+
+        self.wfile.write(response.encode("utf-8"))
+
+    def handle_post_collection(self) -> None:
         self.send_response(200)
         self.send_header("Content-Type", "application/json")
         self.set_zotero_headers()
         papis_library = papis.api.get_lib_name()
+
         response = json.dumps({
             "libraryID": 1,
             "libraryName": papis_library,
-            # I'm not aware of a read-only papis mode
             "libraryEditable": True,
-            # collection-level parameters
             "editable": True,
-            # collection-level
             "id": None,
-            # collection if collection, else library
             "name": papis_library
         })
-        self.wfile.write(bytes(response, "utf8"))
 
-    def add(self):
-        logger.info("Adding paper from zotero connector")
+        self.wfile.write(response.encode("utf-8"))
+
+    def handle_post_add(self) -> None:
+        logger.info("Adding paper from the Zotero Connector.")
         rawinput = self.read_input()
-        data = json.loads(rawinput.decode('utf8'))
+        data = json.loads(rawinput.decode("utf-8"))
 
-        for item in data['items']:
-            files = []
-            if item.get('attachments') and len(item.get('attachments')) > 0:
-                for attachment in item.get('attachments'):
-                    mime = str(attachment.get('mimeType'))
-                    logger.info("Checking attachment (mime {0})".format(mime))
-                    if re.match(r'.*pdf.*', mime):
-                        url = attachment.get('url')
-                        logger.info("Downloading pdf '{0}'".format(url))
-                        try:
-                            pdfbuffer = urllib.request.urlopen(url).read()
-                        except urllib.error.HTTPError:
-                            logger.error(
-                                'Error downloading pdf, probably you do not'
-                                'have the rights for the journal.')
-                            continue
-
-                        pdfpath = tempfile.mktemp(suffix='.pdf')
-                        logger.info("Saving pdf in '{0}'".format(pdfpath))
-
-                        with open(pdfpath, 'wb+') as fd:
-                            fd.write(pdfbuffer)
-
-                        if papis_zotero.utils.is_pdf(pdfpath):
-                            files.append(pdfpath)
-                        else:
-                            logger.error(
-                                'File retrieved does not appear to be a pdf'
-                                'So no file will be saved...')
+        logger.info("Response: %s", data)
+        for item in data["items"]:
+            attachments = item.get("attachments", [])
+            if attachments:
+                files = download_zotero_attachments(attachments)
             else:
-                logger.warning("Document has no attachments")
+                logger.info("Document has no attachments.")
+                files = []
 
             papis_item = zotero_data_to_papis_data(item)
-            if len(files) == 0:
-                logger.warning('Not adding any attachments...')
-            logger.info("Adding paper")
+            logger.info("Adding paper to papis.")
             papis.commands.add.run(files, data=papis_item)
 
-        self.send_response(201)  # Created
+        self.send_response(201)
         self.set_zotero_headers()
-        # return the JSON data back
+
         self.wfile.write(rawinput)
 
-    def snapshot(self):
-        logger.warning("Snapshot not implemented")
+    def handle_post_snapshot(self) -> None:
+        logger.error("Snapshot not implemented!")
         self.send_response(201)
         self.set_zotero_headers()
-        return
-
-    def do_POST(self):
-        if self.path == "/connector/ping":
-            self.pong()
-        elif self.path == '/connector/getSelectedCollection':
-            self.papis_collection()
-        elif self.path == '/connector/saveSnapshot':
-            self.snapshot()
-        elif self.path == '/connector/saveItems':
-            self.add()
-        return
-
-    def do_GET(self):
-        if self.path == "/connector/ping":
-            self.pong(POST=False)
```

### Comparing `./home/gallo/software/papis/env/lib/python3.10/site-packages/papis_zotero-0.1.1-py3.10.egg-info/PKG-INFO` & `papis-zotero-0.1.2/PKG-INFO`

 * *Files 24% similar despite different names*

```diff
@@ -1,185 +1,159 @@
 Metadata-Version: 2.1
 Name: papis-zotero
-Version: 0.1.1
-Summary: Interact with zotero using papis
+Version: 0.1.2
+Summary: Interact with Zotero using papis
 Home-page: https://github.com/papis/papis-zotero
 Author: Alejandro Gallo
 Author-email: aamsgallo@gmail.com
 License: GPLv3
-Keywords: papis,zotero,bibtex,management,cli,biliography
+Keywords: bibtex,biliography,cli,management,papis,zotero
 Platform: linux
 Platform: osx
-Classifier: Environment :: Console
+Platform: win32
 Classifier: Environment :: Console :: Curses
+Classifier: Environment :: Console
 Classifier: Intended Audience :: Developers
+Classifier: Intended Audience :: Education
+Classifier: Intended Audience :: Science/Research
 Classifier: Intended Audience :: System Administrators
 Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
 Classifier: Operating System :: MacOS
+Classifier: Operating System :: Microsoft
+Classifier: Operating System :: OS Independent
 Classifier: Operating System :: POSIX
 Classifier: Operating System :: Unix
-Classifier: Programming Language :: Python :: 3.3
-Classifier: Programming Language :: Python :: 3.4
-Classifier: Programming Language :: Python :: 3.5
-Classifier: Programming Language :: Python :: 3.6
+Classifier: Programming Language :: Python :: 3 :: Only
+Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
+Classifier: Programming Language :: Python :: 3.8
+Classifier: Programming Language :: Python :: 3.9
 Classifier: Topic :: Utilities
+Provides-Extra: develop
 
 .. image:: https://badge.fury.io/py/papis-zotero.svg
     :target: https://badge.fury.io/py/papis-zotero
+.. image:: https://github.com/papis/papis-zotero/workflows/CI/badge.svg
+   :target: https://github.com/papis/papis-zotero/actions?query=branch%3Amaster+workflow%3ACI
 
-|ghbadge|
-
-ZOTERO COMPATIBILITY FOR PAPIS
+Zotero compatibility for papis
 ==============================
 
+Installation
+------------
 
-Importing using bibtex files
-----------------------------
-
-After installation check always the help options
-
-Now the zotero script is accessible from papis:
+To install the latest release from PyPI
 
 .. code:: bash
 
-  papis zotero -h
+    python -m pip install papis-zotero
 
-If you have a bibtex somewhere in your computer, you can use the script:
+To install the latest development version
 
 .. code:: bash
 
-  papis zotero import --from-bibtex library.bib
-
-.. warning::
-
-  Note that if your bibtex file has some pdf entries, i.e., it looks like:
-
-  .. code:: bibtex
+   python -m pip install papis-zotero@https://github.com/papis/papis-zotero.git#egg=papis-zotero
 
-    @article{Einstein1905Photon,
-      author = { A. Einstein },
-      doi = { 10.1002/andp.19053220607 },
-      journal = { Ann. Phys. },
-      pages = { 132--148 },
-      title = { Über einen die Erzeugung und Verwandlung des Lichtes betreffenden heuristischen Gesichtspunkt },
-      FILE = { path/to/some/relative/file.pdf },
-      volume = { 322 },
-      year = { 1905 },
-    }
-
-  then ``papis-zotero`` will interpret the path of the ``FILE`` entry
-  as a relative path, so you should run the command from where this relative path
-  makes sense.
+Development
+-----------
 
-Importing using zotero sql files
---------------------------------
+This project uses ``setup.py`` and ``setuptools`` for its build system.
+To develop the code, it is recommended to start up a
+`virtual environment <https://docs.python.org/3/library/venv.html>`__ and
+install the project in editable mode using, e.g.::
 
-There is also a script that decodes the
-``zotero.sqlite`` sqlite file that ``zotero`` uses to manage documents
-and creates papis Documents out of it.
+    python -m pip install -e '.[develop]'
 
-This script will retrieve the documents from zotero (be it ``pdf`` documents
-or something else) and important information like tags.
-
-Now you have to go to the directory where zotero saves all the information,
-it would look something like this on linux systems:
+After installation always check that the command is correctly recognized, e.g.
+by looking at the help output
 
 .. code:: bash
 
-  cd ~/.mozilla/firefox/zqb7ju1q.default/zotero
+    papis zotero --help
 
-Maybe the path is slightly different. It may vary from version to version from
-zotero.  In the zotero data directory there should be a file called
-``zotero.sqlite`` and there might be a ``storage`` directory with
-document data inside. These will be used by ``zotero-sql`` to
-retrieve information and files from.
+Importing from BibTeX
+---------------------
 
-Now you can use the script through
+Zotero supports exporting different variants of BibTeX or BibLaTeX files
+(from ``Files > Export Library``). The resulting ``bib`` file can be directly
+imported into ``papis`` using
 
 .. code:: bash
 
-  papis zotero import --from-sql-folder YOUR-SQL-FOLDER
-
-where ``YOUR-SQL-FOLDER`` is the folder containing the ``zotero.sqlite``
-folder.
-
-This script by default will create a directory named ``Documents`` (in your
-current directory) where papis documents are stored. You can add these document
-by simply moving them to your library folder
+   papis bibtex read library.bib import --all
 
-.. code::
+but a better choice is using this command, as it has better support for special
+Zotero fields. To import a given exported library run
 
-  mv Documents/*      /path/to/your/papis/library
+.. code:: bash
 
-or also by adding them through papis using the folder flag
+    papis zotero import --from-bibtex library.bib
 
-.. code::
+BibTeX files exported by Zotero can also include has some PDF entries, e.g.
+they can look like
 
-  papis add --from-folder Documents/ZOTERO_ID
+.. code:: bibtex
 
-or write a ``bash`` for-loop to do it with all the converted documents
+    @article{Einstein1905Photon,
+        author = { A. Einstein },
+        doi = { 10.1002/andp.19053220607 },
+        journal = { Ann. Phys. },
+        pages = { 132--148 },
+        title = { Über einen die Erzeugung und Verwandlung des Lichtes
+            betreffenden heuristischen Gesichtspunkt },
+        file = { Full Text:path/to/some/relative/file.pdf },
+        volume = { 322 },
+        year = { 1905 },
+    }
 
-.. code::
+From this, ``papis-zotero`` will interpret the path of the ``file`` entry
+as a relative path to ``library.bib`` passed to the import command using
+``--from-bibtex``. The files are skipped if they do not exist at the expected
+location.
+
+By default, ``papis-zotero`` will add the documents to your current library.
+When initially importing a big library, it is recommended to always import it
+into a scratch folder, so that you can check the import. This can be easily done
+using
 
-  for folder in Documents/* ; do papis add --from-folder $folder ; done
+.. code:: bash
 
-.. warning::
+    papis zotero import --from-bibtex library.bib --outfolder some/folder/lib
 
-   When importing, I recommend always import the library into a scatch folder,
-   so that you can make tests, this would look lik
+When you are ready you can move this folder to a final ``papis`` library.
 
-   .. code:: bash
-    
-      papis zotero import --from-sql YOUR-SQL-FILE --outfolder TEST_FOLDER
+Importing from Zotero SQLite
+----------------------------
 
-   When you are ready you can move this folder into your papis library yourself.
+Zotero also maintains a database of all its files and collections under a
+``zotero.sqlite`` file. You can check where this file is located by going to
+``Edit > Preferences > Advanced > Data Directory Location`` (may vary depending
+on the Zotero version). The Zotero data directory should contain the ``zotero.sqlite``
+file and a ``storage`` directory with the files for each document.
 
+The SQLite database maintained by Zotero can be imported directly (without
+using a BibTeX export) by ``papis-zotero``. This can be done by passing
 
+.. code:: bash
 
-Use zotero conectors
---------------------
+  papis zotero import --from-sql-folder <ZOTERO_DATA_DIRECTORY>
 
-Just install the zotero connector browser plugin
-`here <https://www.zotero.org/download/>`_
-and type
+where ``ZOTERO_DATA_DIRECTORY`` is the folder containing the ``zotero.sqlite``
+file. By default, ``papis-zotero`` will add the imported documents to your
+current library directory, but it can be customized using the
+``--outfolder`` argument.
+
+Using Zotero connectors
+-----------------------
+
+This plugin can also connect to a Zotero connector browser plugin. First, one
+such plugin should be installed from the
+`Zotero website <https://www.zotero.org/download/>`__. Then, make sure that
+Zotero itself is not running (and connected to the connector) and run
 
-::
+.. code:: bash
 
-  papis zotero serve
+    papis zotero serve
 
 to start listening to your browser for incoming data.  Whenever you click the
-zotero button to add a paper, papis will add this paper to the library.
-
-
-Installation from pypi
-----------------------
-
-Just run
-
-::
-
-  sudo pip3 install papis-zotero
-
-Installation
-------------
-
-The general command that you have to hit is by using the ``setup.py`` script:
-
-::
-
-  python3 setup.py install
-
-
-Again, if you want to install it locally because you don't have administrative rights
-in your computer you can just simply type
-
-::
-
-  python3 setup.py install --user
-
-If you want to develop on the code, you can also alternatively hit
-
-::
-
-  python3 setup.py develop --user
-
-.. |ghbadge| image:: https://github.com/papis/papis-zotero/workflows/CI/badge.svg
+Zotero button to add a paper, ``papis-zotero`` will add this paper to its
+library instead.
```

