# Comparing `tmp/mkdocs_caption-0.0.2.tar.gz` & `tmp/mkdocs_caption-0.0.3.tar.gz`

## Comparing `mkdocs_caption-0.0.2.tar` & `mkdocs_caption-0.0.3.tar`

### file list

```diff
@@ -1,14 +1,14 @@
--rw-r--r--   0        0        0      190 2020-02-02 00:00:00.000000 mkdocs_caption-0.0.2/src/mkdocs_caption/__init__.py
--rw-r--r--   0        0        0      160 2020-02-02 00:00:00.000000 mkdocs_caption-0.0.2/src/mkdocs_caption/_version.py
--rw-r--r--   0        0        0     1383 2020-02-02 00:00:00.000000 mkdocs_caption-0.0.2/src/mkdocs_caption/config.py
--rw-r--r--   0        0        0     3418 2020-02-02 00:00:00.000000 mkdocs_caption-0.0.2/src/mkdocs_caption/custom.py
--rw-r--r--   0        0        0     1838 2020-02-02 00:00:00.000000 mkdocs_caption-0.0.2/src/mkdocs_caption/helper.py
--rw-r--r--   0        0        0     2549 2020-02-02 00:00:00.000000 mkdocs_caption-0.0.2/src/mkdocs_caption/image.py
--rw-r--r--   0        0        0     3270 2020-02-02 00:00:00.000000 mkdocs_caption-0.0.2/src/mkdocs_caption/plugin.py
--rw-r--r--   0        0        0     3878 2020-02-02 00:00:00.000000 mkdocs_caption-0.0.2/src/mkdocs_caption/table.py
--rw-r--r--   0        0        0      113 2020-02-02 00:00:00.000000 mkdocs_caption-0.0.2/tests/__init__.py
--rw-r--r--   0        0        0      124 2020-02-02 00:00:00.000000 mkdocs_caption-0.0.2/.gitignore
--rw-r--r--   0        0        0     1070 2020-02-02 00:00:00.000000 mkdocs_caption-0.0.2/LICENSE
--rw-r--r--   0        0        0     7581 2020-02-02 00:00:00.000000 mkdocs_caption-0.0.2/README.md
--rw-r--r--   0        0        0     3286 2020-02-02 00:00:00.000000 mkdocs_caption-0.0.2/pyproject.toml
--rw-r--r--   0        0        0     8537 2020-02-02 00:00:00.000000 mkdocs_caption-0.0.2/PKG-INFO
+-rw-r--r--   0        0        0      190 2020-02-02 00:00:00.000000 mkdocs_caption-0.0.3/src/mkdocs_caption/__init__.py
+-rw-r--r--   0        0        0      160 2020-02-02 00:00:00.000000 mkdocs_caption-0.0.3/src/mkdocs_caption/_version.py
+-rw-r--r--   0        0        0     1383 2020-02-02 00:00:00.000000 mkdocs_caption-0.0.3/src/mkdocs_caption/config.py
+-rw-r--r--   0        0        0     3418 2020-02-02 00:00:00.000000 mkdocs_caption-0.0.3/src/mkdocs_caption/custom.py
+-rw-r--r--   0        0        0     1838 2020-02-02 00:00:00.000000 mkdocs_caption-0.0.3/src/mkdocs_caption/helper.py
+-rw-r--r--   0        0        0     2549 2020-02-02 00:00:00.000000 mkdocs_caption-0.0.3/src/mkdocs_caption/image.py
+-rw-r--r--   0        0        0     3270 2020-02-02 00:00:00.000000 mkdocs_caption-0.0.3/src/mkdocs_caption/plugin.py
+-rw-r--r--   0        0        0     3996 2020-02-02 00:00:00.000000 mkdocs_caption-0.0.3/src/mkdocs_caption/table.py
+-rw-r--r--   0        0        0      113 2020-02-02 00:00:00.000000 mkdocs_caption-0.0.3/tests/__init__.py
+-rw-r--r--   0        0        0      124 2020-02-02 00:00:00.000000 mkdocs_caption-0.0.3/.gitignore
+-rw-r--r--   0        0        0     1070 2020-02-02 00:00:00.000000 mkdocs_caption-0.0.3/LICENSE
+-rw-r--r--   0        0        0     7581 2020-02-02 00:00:00.000000 mkdocs_caption-0.0.3/README.md
+-rw-r--r--   0        0        0     3286 2020-02-02 00:00:00.000000 mkdocs_caption-0.0.3/pyproject.toml
+-rw-r--r--   0        0        0     8537 2020-02-02 00:00:00.000000 mkdocs_caption-0.0.3/PKG-INFO
```

### Comparing `mkdocs_caption-0.0.2/src/mkdocs_caption/config.py` & `mkdocs_caption-0.0.3/src/mkdocs_caption/config.py`

 * *Files identical despite different names*

### Comparing `mkdocs_caption-0.0.2/src/mkdocs_caption/custom.py` & `mkdocs_caption-0.0.3/src/mkdocs_caption/custom.py`

 * *Files identical despite different names*

### Comparing `mkdocs_caption-0.0.2/src/mkdocs_caption/helper.py` & `mkdocs_caption-0.0.3/src/mkdocs_caption/helper.py`

 * *Files identical despite different names*

### Comparing `mkdocs_caption-0.0.2/src/mkdocs_caption/image.py` & `mkdocs_caption-0.0.3/src/mkdocs_caption/image.py`

 * *Files identical despite different names*

### Comparing `mkdocs_caption-0.0.2/src/mkdocs_caption/plugin.py` & `mkdocs_caption-0.0.3/src/mkdocs_caption/plugin.py`

 * *Files identical despite different names*

### Comparing `mkdocs_caption-0.0.2/src/mkdocs_caption/table.py` & `mkdocs_caption-0.0.3/src/mkdocs_caption/table.py`

 * *Files 11% similar despite different names*

```diff
@@ -61,18 +61,19 @@
     Args:
         tree: The root element of the XML tree.
         table_element: The table element to add the caption to.
         caption_element: The caption element to use for the caption text.
         index: The index of the table element.
     """
     caption_prefix = config.caption_prefix.format(index=index, identifier="Table")
+    caption_text = caption_element.text.replace(" & ", " &amp; ") if caption_element.text else ""
     try:
-        table_caption_element = etree.fromstring(f"<caption>{caption_prefix} {caption_element.text}</caption>")
+        table_caption_element = etree.fromstring(f"<caption>{caption_prefix} {caption_text}</caption>")
     except etree.XMLSyntaxError as e:
-        e.msg = f"Invalid XML in caption: {caption_element.text}"
+        e.msg = f"Invalid XML in caption: <caption>{caption_prefix} {caption_text}</caption>"
         raise e
     table_element.insert(0, table_caption_element)
 
     if "cols" in caption_element.attrib:
         table_element.insert(0, _create_colgroups(caption_element.attrib["cols"]))
         caption_element.attrib.pop("cols")
     table_element.attrib.update(caption_element.attrib)
```

### Comparing `mkdocs_caption-0.0.2/LICENSE` & `mkdocs_caption-0.0.3/LICENSE`

 * *Files identical despite different names*

### Comparing `mkdocs_caption-0.0.2/README.md` & `mkdocs_caption-0.0.3/README.md`

 * *Files identical despite different names*

### Comparing `mkdocs_caption-0.0.2/pyproject.toml` & `mkdocs_caption-0.0.3/pyproject.toml`

 * *Files identical despite different names*

### Comparing `mkdocs_caption-0.0.2/PKG-INFO` & `mkdocs_caption-0.0.3/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mkdocs-caption
-Version: 0.0.2
+Version: 0.0.3
 Project-URL: Documentation, https://github.com/tobiasah/mkdocs-caption#readme
 Project-URL: Issues, https://github.com/tobiasah/mkdocs-caption/issues
 Project-URL: Source, https://github.com/tobiasah/mkdocs-caption
 Author-email: Tobias Ahrens <tobias.ahrens@posteo.de>
 License-Expression: MIT
 License-File: LICENSE
 Classifier: Development Status :: 4 - Beta
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: mkdocs-caption Version: 0.0.2 Project-URL:
+Metadata-Version: 2.1 Name: mkdocs-caption Version: 0.0.3 Project-URL:
 Documentation, https://github.com/tobiasah/mkdocs-caption#readme Project-URL:
 Issues, https://github.com/tobiasah/mkdocs-caption/issues Project-URL: Source,
 https://github.com/tobiasah/mkdocs-caption Author-email: Tobias Ahrens
 ahrens@posteo.de> License-Expression: MIT License-File: LICENSE Classifier:
 Development Status :: 4 - Beta Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3.7 Classifier: Programming
 Language :: Python :: 3.8 Classifier: Programming Language :: Python :: 3.9
```

