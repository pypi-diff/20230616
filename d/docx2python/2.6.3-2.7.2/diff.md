# Comparing `tmp/docx2python-2.6.3.tar.gz` & `tmp/docx2python-2.7.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "docx2python-2.6.3.tar", max compression
+gzip compressed data, was "docx2python-2.7.2.tar", max compression
```

## Comparing `docx2python-2.6.3.tar` & `docx2python-2.7.2.tar`

### file list

```diff
@@ -1,21 +1,21 @@
--rw-r--r--   0        0        0      240 2023-04-27 18:33:43.953747 docx2python-2.6.3/docx2python/__init__.py
--rw-r--r--   0        0        0     4945 2023-04-27 18:33:43.953747 docx2python-2.6.3/docx2python/attribute_register.py
--rw-r--r--   0        0        0     5272 2023-04-27 18:33:43.953747 docx2python-2.6.3/docx2python/bullets_and_numbering.py
--rw-r--r--   0        0        0     9246 2023-04-27 18:33:43.953747 docx2python-2.6.3/docx2python/depth_collector.py
--rw-r--r--   0        0        0     6857 2023-04-27 18:33:43.953747 docx2python-2.6.3/docx2python/docx_context.py
--rw-r--r--   0        0        0     8410 2023-04-27 18:33:43.953747 docx2python-2.6.3/docx2python/docx_output.py
--rw-r--r--   0        0        0    16656 2023-04-27 18:33:43.953747 docx2python-2.6.3/docx2python/docx_reader.py
--rw-r--r--   0        0        0    10196 2023-04-27 18:33:43.953747 docx2python-2.6.3/docx2python/docx_text.py
--rw-r--r--   0        0        0     3244 2023-04-27 18:33:43.969370 docx2python-2.6.3/docx2python/forms.py
--rw-r--r--   0        0        0     9725 2023-04-27 18:33:43.969370 docx2python-2.6.3/docx2python/iterators.py
--rw-r--r--   0        0        0     1939 2023-04-27 18:33:43.969370 docx2python-2.6.3/docx2python/main.py
--rw-r--r--   0        0        0     5291 2023-04-27 18:33:43.969370 docx2python-2.6.3/docx2python/merge_runs.py
--rw-r--r--   0        0        0     2857 2023-04-27 18:33:43.969370 docx2python-2.6.3/docx2python/namespace.py
--rw-r--r--   0        0        0     3587 2023-04-27 18:33:43.969370 docx2python-2.6.3/docx2python/numbering_formats.py
--rw-r--r--   0        0        0        0 2023-04-27 18:33:43.969370 docx2python-2.6.3/docx2python/py.typed
--rw-r--r--   0        0        0    10053 2023-04-27 18:33:43.969370 docx2python-2.6.3/docx2python/text_runs.py
--rw-r--r--   0        0        0     4525 2023-04-27 18:33:43.969370 docx2python-2.6.3/docx2python/utilities.py
--rw-r--r--   0        0        0     1097 2023-04-27 18:33:43.953747 docx2python-2.6.3/LICENSE.txt
--rw-r--r--   0        0        0     1486 2023-04-27 18:33:43.969370 docx2python-2.6.3/pyproject.toml
--rw-r--r--   0        0        0    13515 2023-04-27 18:33:43.953747 docx2python-2.6.3/README.md
--rw-r--r--   0        0        0    13730 1970-01-01 00:00:00.000000 docx2python-2.6.3/PKG-INFO
+-rw-r--r--   0        0        0      240 2023-01-19 19:29:25.943561 docx2python-2.7.2/docx2python/__init__.py
+-rw-r--r--   0        0        0     4977 2023-06-14 22:17:55.360593 docx2python-2.7.2/docx2python/attribute_register.py
+-rw-r--r--   0        0        0     5272 2023-01-19 19:29:25.944712 docx2python-2.7.2/docx2python/bullets_and_numbering.py
+-rw-r--r--   0        0        0     9246 2023-05-03 15:35:58.417678 docx2python-2.7.2/docx2python/depth_collector.py
+-rw-r--r--   0        0        0     6857 2023-04-27 14:43:36.300114 docx2python-2.7.2/docx2python/docx_context.py
+-rw-r--r--   0        0        0     8410 2023-01-27 18:14:24.180137 docx2python-2.7.2/docx2python/docx_output.py
+-rw-r--r--   0        0        0    16656 2023-01-23 22:13:46.338596 docx2python-2.7.2/docx2python/docx_reader.py
+-rw-r--r--   0        0        0    10473 2023-06-16 01:58:00.213479 docx2python-2.7.2/docx2python/docx_text.py
+-rw-r--r--   0        0        0     3244 2023-01-19 19:29:25.947556 docx2python-2.7.2/docx2python/forms.py
+-rw-r--r--   0        0        0     9725 2023-01-19 19:29:25.947999 docx2python-2.7.2/docx2python/iterators.py
+-rw-r--r--   0        0        0     1939 2023-01-23 22:13:46.340597 docx2python-2.7.2/docx2python/main.py
+-rw-r--r--   0        0        0     5291 2023-01-19 19:29:25.949121 docx2python-2.7.2/docx2python/merge_runs.py
+-rw-r--r--   0        0        0     2942 2023-06-14 22:17:55.361917 docx2python-2.7.2/docx2python/namespace.py
+-rw-r--r--   0        0        0     3587 2023-01-19 19:29:25.949556 docx2python-2.7.2/docx2python/numbering_formats.py
+-rw-r--r--   0        0        0        0 2023-02-03 22:08:10.380704 docx2python-2.7.2/docx2python/py.typed
+-rw-r--r--   0        0        0    10053 2023-01-23 22:13:46.340597 docx2python-2.7.2/docx2python/text_runs.py
+-rw-r--r--   0        0        0     4525 2023-04-27 14:43:36.301404 docx2python-2.7.2/docx2python/utilities.py
+-rw-r--r--   0        0        0     1097 2023-01-19 19:29:25.942725 docx2python-2.7.2/LICENSE.txt
+-rw-r--r--   0        0        0     1486 2023-06-16 02:38:10.617710 docx2python-2.7.2/pyproject.toml
+-rw-r--r--   0        0        0    13515 2023-06-16 01:42:45.207612 docx2python-2.7.2/README.md
+-rw-r--r--   0        0        0    13730 1970-01-01 00:00:00.000000 docx2python-2.7.2/PKG-INFO
```

### Comparing `docx2python-2.6.3/docx2python/attribute_register.py` & `docx2python-2.7.2/docx2python/attribute_register.py`

 * *Files 2% similar despite different names*

```diff
@@ -87,14 +87,15 @@
     ENDNOTE_REFERENCE = qn("w:endnoteReference")
     FOOTNOTE = qn("w:footnote")
     FOOTNOTE_REFERENCE = qn("w:footnoteReference")
     FORM_CHECKBOX = qn("w:checkBox")
     FORM_DDLIST = qn("w:ddList")  # drop-down form
     HYPERLINK = qn("w:hyperlink")
     IMAGE = qn("a:blip")
+    IMAGE_ALT = qn("wp:docPr")
     IMAGEDATA = qn("v:imagedata")
     MATH = qn("m:oMath")
     PARAGRAPH = qn("w:p")
     PAR_PROPERTIES = qn("w:pPr")
     RUN = qn("w:r")
     RUN_PROPERTIES = qn("w:rPr")
     SYM = qn("w:sym")
```

### Comparing `docx2python-2.6.3/docx2python/bullets_and_numbering.py` & `docx2python-2.7.2/docx2python/bullets_and_numbering.py`

 * *Files identical despite different names*

### Comparing `docx2python-2.6.3/docx2python/depth_collector.py` & `docx2python-2.7.2/docx2python/depth_collector.py`

 * *Files identical despite different names*

### Comparing `docx2python-2.6.3/docx2python/docx_context.py` & `docx2python-2.7.2/docx2python/docx_context.py`

 * *Files identical despite different names*

### Comparing `docx2python-2.6.3/docx2python/docx_output.py` & `docx2python-2.7.2/docx2python/docx_output.py`

 * *Files identical despite different names*

### Comparing `docx2python-2.6.3/docx2python/docx_reader.py` & `docx2python-2.7.2/docx2python/docx_reader.py`

 * *Files identical despite different names*

### Comparing `docx2python-2.6.3/docx2python/docx_text.py` & `docx2python-2.7.2/docx2python/docx_text.py`

 * *Files 2% similar despite different names*

```diff
@@ -86,15 +86,16 @@
         :param tree_: a sequence of elements which may contain a paragraph
         :return: depth of the first paragraph found, or None if no paragraph found
         """
         if not tree_:
             return None
         if any(x.tag == Tags.PARAGRAPH for x in tree_):
             return max(4 - _depth, 1)
-        return search_at_depth(sum([list(x) for x in tree_], []), _depth + 1)
+        grandchildren = [list(x) for x in tree_]
+        return search_at_depth([x for y in grandchildren for x in y], _depth + 1)
 
     return search_at_depth([tree])
 
 
 def get_paragraphs(file: File, root: EtreeElement) -> list[str]:
     """Return a list of paragraphs from the document
 
@@ -235,14 +236,19 @@
 
         elif tree.tag == Tags.IMAGE:
             with suppress(KeyError):
                 rId = tree.attrib[qn("r:embed")]
                 image = file.rels[rId]
                 tables.insert_text_as_new_run(f"----{image}----")
 
+        elif tree.tag == Tags.IMAGE_ALT:
+            with suppress(KeyError):
+                description = tree.attrib["descr"]
+                tables.insert_text_as_new_run(f"----Image alt text---->{description}<")
+
         elif tree.tag == Tags.IMAGEDATA:
             with suppress(KeyError):
                 rId = tree.attrib[qn("r:id")]
                 image = file.rels[rId]
                 tables.insert_text_as_new_run(f"----{image}----")
 
         elif tree.tag == Tags.TAB:
```

### Comparing `docx2python-2.6.3/docx2python/forms.py` & `docx2python-2.7.2/docx2python/forms.py`

 * *Files identical despite different names*

### Comparing `docx2python-2.6.3/docx2python/iterators.py` & `docx2python-2.7.2/docx2python/iterators.py`

 * *Files identical despite different names*

### Comparing `docx2python-2.6.3/docx2python/main.py` & `docx2python-2.7.2/docx2python/main.py`

 * *Files identical despite different names*

### Comparing `docx2python-2.6.3/docx2python/merge_runs.py` & `docx2python-2.7.2/docx2python/merge_runs.py`

 * *Files identical despite different names*

### Comparing `docx2python-2.6.3/docx2python/namespace.py` & `docx2python-2.7.2/docx2python/namespace.py`

 * *Files 1% similar despite different names*

```diff
@@ -52,14 +52,15 @@
     "cp": "http://schemas.openxmlformats.org/package/2006/metadata/core-properties",
     "dc": "http://purl.org/dc/elements/1.1/",
     "dcterms": "http://purl.org/dc/terms/",
     "m": "http://schemas.openxmlformats.org/officeDocument/2006/math",
     "r": "http://schemas.openxmlformats.org/officeDocument/2006/relationships",
     "v": "urn:schemas-microsoft-com:vml",
     "w": "http://schemas.openxmlformats.org/wordprocessingml/2006/main",
+    "wp": "http://schemas.openxmlformats.org/drawingml/2006/wordprocessingDrawing",
 }
 
 
 def qn(tag: str) -> str:
     """
     Turn a namespace-prefixed tag into a Clark-notation qualified tag.
```

### Comparing `docx2python-2.6.3/docx2python/numbering_formats.py` & `docx2python-2.7.2/docx2python/numbering_formats.py`

 * *Files identical despite different names*

### Comparing `docx2python-2.6.3/docx2python/text_runs.py` & `docx2python-2.7.2/docx2python/text_runs.py`

 * *Files identical despite different names*

### Comparing `docx2python-2.6.3/docx2python/utilities.py` & `docx2python-2.7.2/docx2python/utilities.py`

 * *Files identical despite different names*

### Comparing `docx2python-2.6.3/LICENSE.txt` & `docx2python-2.7.2/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `docx2python-2.6.3/pyproject.toml` & `docx2python-2.7.2/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "docx2python"
-version = "2.6.3"
+version = "2.7.2"
 description = "Extract content from docx files"
 authors = ["Shay Hill <shay_public@hotmail.com>"]
 license = "MIT"
 readme = "README.md"
 
 [tool.poetry.dependencies]
 python = "^3.8"
@@ -14,15 +14,15 @@
 pytest = "^7.2.0"
 types-lxml = "^2022.11.8"
 commitizen = "^2.39.1"
 pre-commit = "^3.0.4"
 
 [tool.commitizen]
 name = "cz_conventional_commits"
-version = "2.7.0"
+version = "2.7.2"
 tag_format = "$version"
 version_files = [
     "pyproject.toml:^version"
 ]
 
 [build-system]
 requires = ["poetry-core"]
```

### Comparing `docx2python-2.6.3/README.md` & `docx2python-2.7.2/README.md`

 * *Files identical despite different names*

### Comparing `docx2python-2.6.3/PKG-INFO` & `docx2python-2.7.2/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: docx2python
-Version: 2.6.3
+Version: 2.7.2
 Summary: Extract content from docx files
 License: MIT
 Author: Shay Hill
 Author-email: shay_public@hotmail.com
 Requires-Python: >=3.8,<4.0
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
```

