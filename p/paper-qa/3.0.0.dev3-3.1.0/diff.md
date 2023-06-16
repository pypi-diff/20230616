# Comparing `tmp/paper-qa-3.0.0.dev3.tar.gz` & `tmp/paper-qa-3.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "paper-qa-3.0.0.dev3.tar", last modified: Wed Jun 14 05:53:43 2023, max compression
+gzip compressed data, was "paper-qa-3.1.0.tar", last modified: Fri Jun 16 15:34:54 2023, max compression
```

## Comparing `paper-qa-3.0.0.dev3.tar` & `paper-qa-3.1.0.tar`

### file list

```diff
@@ -1,27 +1,27 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 05:53:43.152098 paper-qa-3.0.0.dev3/
--rw-r--r--   0 runner    (1001) docker     (123)    11357 2023-06-14 05:53:04.000000 paper-qa-3.0.0.dev3/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)    18141 2023-06-14 05:53:43.152098 paper-qa-3.0.0.dev3/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    17701 2023-06-14 05:53:04.000000 paper-qa-3.0.0.dev3/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 05:53:43.152098 paper-qa-3.0.0.dev3/paper_qa.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    18141 2023-06-14 05:53:43.000000 paper-qa-3.0.0.dev3/paper_qa.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      423 2023-06-14 05:53:43.000000 paper-qa-3.0.0.dev3/paper_qa.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-14 05:53:43.000000 paper-qa-3.0.0.dev3/paper_qa.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       89 2023-06-14 05:53:43.000000 paper-qa-3.0.0.dev3/paper_qa.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        8 2023-06-14 05:53:43.000000 paper-qa-3.0.0.dev3/paper_qa.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 05:53:43.152098 paper-qa-3.0.0.dev3/paperqa/
--rw-r--r--   0 runner    (1001) docker     (123)      173 2023-06-14 05:53:04.000000 paper-qa-3.0.0.dev3/paperqa/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3630 2023-06-14 05:53:04.000000 paper-qa-3.0.0.dev3/paperqa/chains.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 05:53:43.152098 paper-qa-3.0.0.dev3/paperqa/contrib/
--rw-r--r--   0 runner    (1001) docker     (123)       53 2023-06-14 05:53:04.000000 paper-qa-3.0.0.dev3/paperqa/contrib/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    12316 2023-06-14 05:53:04.000000 paper-qa-3.0.0.dev3/paperqa/contrib/zotero.py
--rw-r--r--   0 runner    (1001) docker     (123)    22301 2023-06-14 05:53:04.000000 paper-qa-3.0.0.dev3/paperqa/docs.py
--rw-r--r--   0 runner    (1001) docker     (123)       65 2023-06-14 05:53:04.000000 paper-qa-3.0.0.dev3/paperqa/paths.py
--rw-r--r--   0 runner    (1001) docker     (123)     2234 2023-06-14 05:53:04.000000 paper-qa-3.0.0.dev3/paperqa/prompts.py
--rw-r--r--   0 runner    (1001) docker     (123)     4868 2023-06-14 05:53:04.000000 paper-qa-3.0.0.dev3/paperqa/readers.py
--rw-r--r--   0 runner    (1001) docker     (123)     3761 2023-06-14 05:53:04.000000 paper-qa-3.0.0.dev3/paperqa/types.py
--rw-r--r--   0 runner    (1001) docker     (123)     2173 2023-06-14 05:53:04.000000 paper-qa-3.0.0.dev3/paperqa/utils.py
--rw-r--r--   0 runner    (1001) docker     (123)       27 2023-06-14 05:53:04.000000 paper-qa-3.0.0.dev3/paperqa/version.py
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-14 05:53:43.152098 paper-qa-3.0.0.dev3/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)      972 2023-06-14 05:53:04.000000 paper-qa-3.0.0.dev3/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 05:53:43.152098 paper-qa-3.0.0.dev3/tests/
--rw-r--r--   0 runner    (1001) docker     (123)    19821 2023-06-14 05:53:04.000000 paper-qa-3.0.0.dev3/tests/test_paperqa.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 15:34:54.380644 paper-qa-3.1.0/
+-rw-r--r--   0 runner    (1001) docker     (123)    11357 2023-06-16 15:34:17.000000 paper-qa-3.1.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)    18136 2023-06-16 15:34:54.380644 paper-qa-3.1.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    17701 2023-06-16 15:34:17.000000 paper-qa-3.1.0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 15:34:54.376644 paper-qa-3.1.0/paper_qa.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    18136 2023-06-16 15:34:54.000000 paper-qa-3.1.0/paper_qa.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      423 2023-06-16 15:34:54.000000 paper-qa-3.1.0/paper_qa.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-16 15:34:54.000000 paper-qa-3.1.0/paper_qa.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       89 2023-06-16 15:34:54.000000 paper-qa-3.1.0/paper_qa.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        8 2023-06-16 15:34:54.000000 paper-qa-3.1.0/paper_qa.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 15:34:54.376644 paper-qa-3.1.0/paperqa/
+-rw-r--r--   0 runner    (1001) docker     (123)      173 2023-06-16 15:34:17.000000 paper-qa-3.1.0/paperqa/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3630 2023-06-16 15:34:17.000000 paper-qa-3.1.0/paperqa/chains.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 15:34:54.380644 paper-qa-3.1.0/paperqa/contrib/
+-rw-r--r--   0 runner    (1001) docker     (123)       53 2023-06-16 15:34:17.000000 paper-qa-3.1.0/paperqa/contrib/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12316 2023-06-16 15:34:17.000000 paper-qa-3.1.0/paperqa/contrib/zotero.py
+-rw-r--r--   0 runner    (1001) docker     (123)    22435 2023-06-16 15:34:17.000000 paper-qa-3.1.0/paperqa/docs.py
+-rw-r--r--   0 runner    (1001) docker     (123)       65 2023-06-16 15:34:17.000000 paper-qa-3.1.0/paperqa/paths.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2234 2023-06-16 15:34:17.000000 paper-qa-3.1.0/paperqa/prompts.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4868 2023-06-16 15:34:17.000000 paper-qa-3.1.0/paperqa/readers.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3761 2023-06-16 15:34:17.000000 paper-qa-3.1.0/paperqa/types.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2173 2023-06-16 15:34:17.000000 paper-qa-3.1.0/paperqa/utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)       22 2023-06-16 15:34:17.000000 paper-qa-3.1.0/paperqa/version.py
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-16 15:34:54.380644 paper-qa-3.1.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      971 2023-06-16 15:34:17.000000 paper-qa-3.1.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 15:34:54.380644 paper-qa-3.1.0/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)    20285 2023-06-16 15:34:17.000000 paper-qa-3.1.0/tests/test_paperqa.py
```

### Comparing `paper-qa-3.0.0.dev3/LICENSE` & `paper-qa-3.1.0/LICENSE`

 * *Files identical despite different names*

### Comparing `paper-qa-3.0.0.dev3/PKG-INFO` & `paper-qa-3.1.0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: paper-qa
-Version: 3.0.0.dev3
+Version: 3.1.0
 Summary: LLM Chain for answering questions from docs 
 Home-page: https://github.com/whitead/paper-qa
 Author: Andrew White
 Author-email: white.d.andrew@gmail.com
 License: MIT
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `paper-qa-3.0.0.dev3/README.md` & `paper-qa-3.1.0/README.md`

 * *Files identical despite different names*

### Comparing `paper-qa-3.0.0.dev3/paper_qa.egg-info/PKG-INFO` & `paper-qa-3.1.0/paper_qa.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: paper-qa
-Version: 3.0.0.dev3
+Version: 3.1.0
 Summary: LLM Chain for answering questions from docs 
 Home-page: https://github.com/whitead/paper-qa
 Author: Andrew White
 Author-email: white.d.andrew@gmail.com
 License: MIT
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `paper-qa-3.0.0.dev3/paperqa/chains.py` & `paper-qa-3.1.0/paperqa/chains.py`

 * *Files identical despite different names*

### Comparing `paper-qa-3.0.0.dev3/paperqa/contrib/zotero.py` & `paper-qa-3.1.0/paperqa/contrib/zotero.py`

 * *Files identical despite different names*

### Comparing `paper-qa-3.0.0.dev3/paperqa/docs.py` & `paper-qa-3.1.0/paperqa/docs.py`

 * *Files 1% similar despite different names*

```diff
@@ -113,15 +113,15 @@
     def add_file(
         self,
         file: BinaryIO,
         citation: Optional[str] = None,
         docname: Optional[str] = None,
         dockey: Optional[DocKey] = None,
         chunk_chars: int = 3000,
-    ) -> str:
+    ) -> Optional[str]:
         """Add a document to the collection."""
         # just put in temp file and use existing method
         suffix = ".txt"
         if maybe_is_pdf(file):
             suffix = ".pdf"
         elif maybe_is_html(file):
             suffix = ".html"
@@ -140,15 +140,15 @@
     def add_url(
         self,
         url: str,
         citation: Optional[str] = None,
         docname: Optional[str] = None,
         dockey: Optional[DocKey] = None,
         chunk_chars: int = 3000,
-    ) -> str:
+    ) -> Optional[str]:
         """Add a document to the collection."""
         import urllib.request
 
         with urllib.request.urlopen(url) as f:
             # need to wrap to enable seek
             file = BytesIO(f.read())
             return self.add_file(
@@ -163,15 +163,15 @@
         self,
         path: Path,
         citation: Optional[str] = None,
         docname: Optional[str] = None,
         disable_check: bool = False,
         dockey: Optional[DocKey] = None,
         chunk_chars: int = 3000,
-    ) -> str:
+    ) -> Optional[str]:
         """Add a document to the collection."""
         if dockey is None:
             dockey = md5sum(path)
         if citation is None:
             # skip system because it's too hesitant to answer
             cite_chain = make_chain(
                 prompt=self.prompts.cite,
@@ -212,25 +212,29 @@
             len(texts) == 0
             or len(texts[0].text) < 10
             or (not disable_check and not maybe_is_text(texts[0].text))
         ):
             raise ValueError(
                 f"This does not look like a text document: {path}. Path disable_check to ignore this error."
             )
-        self.add_texts(texts, doc)
-        return docname
+        if self.add_texts(texts, doc):
+            return docname
+        return None
 
     def add_texts(
         self,
         texts: List[Text],
         doc: Doc,
-    ):
-        """Add chunked texts to the collection. This is useful if you have already chunked the texts yourself."""
+    ) -> bool:
+        """Add chunked texts to the collection. This is useful if you have already chunked the texts yourself.
+
+        Returns True if the document was added, False if it was already in the collection.
+        """
         if doc.dockey in self.docs:
-            raise ValueError(f"Document {doc.dockey} already in collection.")
+            return False
         if len(texts) == 0:
             raise ValueError("No texts to add.")
         if doc.docname in self.docnames:
             new_docname = self._get_unique_name(doc.docname)
             for t in texts:
                 t.name = t.name.replace(doc.docname, new_docname)
             doc.docname = new_docname
@@ -251,14 +255,15 @@
             except AttributeError:
                 raise ValueError("Need a vector store that supports adding embeddings.")
         if self.doc_index is not None:
             self.doc_index.add_texts([doc.citation], metadatas=[{"dockey": doc.dockey}])
         self.docs[doc.dockey] = doc
         self.texts += texts
         self.docnames.add(doc.docname)
+        return True
 
     def delete(
         self, name: Optional[str] = None, dockey: Optional[DocKey] = None
     ) -> None:
         """Delete a document from the collection."""
         if name is not None:
             doc = next((doc for doc in self.docs.values() if doc.docname == name), None)
```

### Comparing `paper-qa-3.0.0.dev3/paperqa/prompts.py` & `paper-qa-3.1.0/paperqa/prompts.py`

 * *Files identical despite different names*

### Comparing `paper-qa-3.0.0.dev3/paperqa/readers.py` & `paper-qa-3.1.0/paperqa/readers.py`

 * *Files identical despite different names*

### Comparing `paper-qa-3.0.0.dev3/paperqa/types.py` & `paper-qa-3.1.0/paperqa/types.py`

 * *Files identical despite different names*

### Comparing `paper-qa-3.0.0.dev3/paperqa/utils.py` & `paper-qa-3.1.0/paperqa/utils.py`

 * *Files identical despite different names*

### Comparing `paper-qa-3.0.0.dev3/setup.py` & `paper-qa-3.1.0/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -30,8 +30,8 @@
     long_description_content_type="text/markdown",
     classifiers=[
         "Programming Language :: Python :: 3",
         "License :: OSI Approved :: MIT License",
         "Operating System :: OS Independent",
     ],
 )
-1
+
```

### Comparing `paper-qa-3.0.0.dev3/tests/test_paperqa.py` & `paper-qa-3.1.0/tests/test_paperqa.py`

 * *Files 2% similar despite different names*

```diff
@@ -101,15 +101,15 @@
     with open(doc_path, "w", encoding="utf-8") as f:
         # get wiki page about politician
         r = requests.get("https://en.wikipedia.org/wiki/Frederick_Bates_(politician)")
         f.write(r.text)
     docs = Docs()
     docs.add(doc_path, "WikiMedia Foundation, 2023, Accessed now")
     evidence = docs.get_evidence(
-        Answer(question="For which state was he a governor"), k=1, max_sources=1
+        Answer(question="For which state was Bates a governor?"), k=1, max_sources=1
     )
     assert "Missouri" in evidence.context
     os.remove(doc_path)
 
 
 def test_query():
     docs = Docs()
@@ -117,14 +117,31 @@
         "https://en.wikipedia.org/wiki/Frederick_Bates_(politician)",
         citation="WikiMedia Foundation, 2023, Accessed now",
         dockey="test",
     )
     docs.query("What is Frederick Bates's greatest accomplishment?")
 
 
+def test_duplicate():
+    docs = Docs()
+    assert docs.add_url(
+        "https://en.wikipedia.org/wiki/Frederick_Bates_(politician)",
+        citation="WikiMedia Foundation, 2023, Accessed now",
+        dockey="test",
+    )
+    assert (
+        docs.add_url(
+            "https://en.wikipedia.org/wiki/Frederick_Bates_(politician)",
+            citation="WikiMedia Foundation, 2023, Accessed now",
+            dockey="test",
+        )
+        is None
+    )
+
+
 class Test(IsolatedAsyncioTestCase):
     async def test_aquery(self):
         docs = Docs()
         docs.add_url(
             "https://en.wikipedia.org/wiki/Frederick_Bates_(politician)",
             citation="WikiMedia Foundation, 2023, Accessed now",
             dockey="test",
```

