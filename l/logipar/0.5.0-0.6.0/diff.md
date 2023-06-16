# Comparing `tmp/logipar-0.5.0.tar.gz` & `tmp/logipar-0.6.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist\logipar-0.5.0.tar", last modified: Thu Jun 15 02:31:09 2023, max compression
+gzip compressed data, was "dist\logipar-0.6.0.tar", last modified: Fri Jun 16 20:15:26 2023, max compression
```

## Comparing `logipar-0.5.0.tar` & `logipar-0.6.0.tar`

### file list

```diff
@@ -1,12 +1,12 @@
-drwxrwxrwx   0        0        0        0 2023-06-15 02:31:09.011197 logipar-0.5.0/
--rw-rw-rw-   0        0        0    20313 2023-06-15 02:31:09.008412 logipar-0.5.0/PKG-INFO
-drwxrwxrwx   0        0        0        0 2023-06-15 02:31:08.989060 logipar-0.5.0/logipar/
--rw-rw-rw-   0        0        0       66 2023-06-15 01:57:32.000000 logipar-0.5.0/logipar/__init__.py
--rw-rw-rw-   0        0        0    39640 2023-06-15 02:14:12.000000 logipar-0.5.0/logipar/logipar.py
-drwxrwxrwx   0        0        0        0 2023-06-15 02:31:09.007415 logipar-0.5.0/logipar.egg-info/
--rw-rw-rw-   0        0        0    20313 2023-06-15 02:31:08.000000 logipar-0.5.0/logipar.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      171 2023-06-15 02:31:08.000000 logipar-0.5.0/logipar.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-06-15 02:31:08.000000 logipar-0.5.0/logipar.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        8 2023-06-15 02:31:08.000000 logipar-0.5.0/logipar.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-06-15 02:31:09.011197 logipar-0.5.0/setup.cfg
--rw-rw-rw-   0        0        0      569 2023-06-15 02:29:15.000000 logipar-0.5.0/setup.py
+drwxrwxrwx   0        0        0        0 2023-06-16 20:15:26.445412 logipar-0.6.0/
+-rw-rw-rw-   0        0        0    20313 2023-06-16 20:15:26.444413 logipar-0.6.0/PKG-INFO
+drwxrwxrwx   0        0        0        0 2023-06-16 20:15:26.428413 logipar-0.6.0/logipar/
+-rw-rw-rw-   0        0        0       66 2023-06-15 01:57:32.000000 logipar-0.6.0/logipar/__init__.py
+-rw-rw-rw-   0        0        0    39770 2023-06-16 20:10:08.000000 logipar-0.6.0/logipar/logipar.py
+drwxrwxrwx   0        0        0        0 2023-06-16 20:15:26.443412 logipar-0.6.0/logipar.egg-info/
+-rw-rw-rw-   0        0        0    20313 2023-06-16 20:15:26.000000 logipar-0.6.0/logipar.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      171 2023-06-16 20:15:26.000000 logipar-0.6.0/logipar.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-06-16 20:15:26.000000 logipar-0.6.0/logipar.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        8 2023-06-16 20:15:26.000000 logipar-0.6.0/logipar.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-06-16 20:15:26.445412 logipar-0.6.0/setup.cfg
+-rw-rw-rw-   0        0        0      569 2023-06-16 20:15:16.000000 logipar-0.6.0/setup.py
```

### Comparing `logipar-0.5.0/PKG-INFO` & `logipar-0.6.0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: logipar
-Version: 0.5.0
+Version: 0.6.0
 Summary: A logic string parser
 Home-page: https://github.com/altef/logipar
 Author: Brad Gill
 Author-email: brad@alteredeffect.com
 License: UNKNOWN
 Description: [![npm](https://img.shields.io/npm/v/logipar)](https://npmjs.com/package/logipar) [![pypi](https://img.shields.io/pypi/v/logipar)](https://pypi.org/project/logipar/) [![haxelib install logipar](https://img.shields.io/badge/haxelib-logipar-orange, "haxelib install logipar")](https://lib.haxe.org/p/logipar/) [![php phar](https://img.shields.io/badge/php-Logipar.phar-orange, "PHP Logipar.phar")](https://github.com/altef/logipar/blob/master/php/Logipar.phar)
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: logipar Version: 0.5.0 Summary: A logic string
+Metadata-Version: 2.1 Name: logipar Version: 0.6.0 Summary: A logic string
 parser Home-page: https://github.com/altef/logipar Author: Brad Gill Author-
 email: brad@alteredeffect.com License: UNKNOWN Description: [![npm](https://
 img.shields.io/npm/v/logipar)](https://npmjs.com/package/logipar) [![pypi]
 (https://img.shields.io/pypi/v/logipar)](https://pypi.org/project/logipar/) [!
 [haxelib install logipar](https://img.shields.io/badge/haxelib-logipar-orange,
 "haxelib install logipar")](https://lib.haxe.org/p/logipar/) [![php phar]
 (https://img.shields.io/badge/php-Logipar.phar-orange, "PHP Logipar.phar")]
```

### Comparing `logipar-0.5.0/logipar/logipar.py` & `logipar-0.6.0/logipar/logipar.py`

 * *Files 1% similar despite different names*

```diff
@@ -361,15 +361,15 @@
 
 
 
 class Logipar:
     _hx_class_name = "Logipar"
     __slots__ = ("quotations", "caseSensitive", "mergeAdjacentLiterals", "syntax", "tree")
     _hx_fields = ["quotations", "caseSensitive", "mergeAdjacentLiterals", "syntax", "tree"]
-    _hx_methods = ["overwrite", "parse", "stringify", "walk", "filterFunction", "toString", "equals", "mergeLiterals", "treeify", "shunt", "tentativelyLower", "tokenize", "tokenType", "typeize"]
+    _hx_methods = ["overwrite", "prepareTokens", "parse", "stringify", "walk", "filterFunction", "toString", "equals", "mergeLiterals", "treeify", "shunt", "tentativelyLower", "tokenize", "tokenType", "typeize"]
 
     def __init__(self):
         self.tree = None
         _g = haxe_ds_StringMap()
         _g.h["AND"] = "AND"
         _g.h["OR"] = "OR"
         _g.h["XOR"] = "XOR"
@@ -381,19 +381,23 @@
         self.caseSensitive = True
         self.quotations = ["\"", "'"]
 
     def overwrite(self,op,value):
         if (op in self.syntax.h):
             self.syntax.h[op] = value
 
-    def parse(self,logic_string):
+    def prepareTokens(self,logic_string):
         tokens = self.tokenize(logic_string)
         types = self.typeize(tokens)
         if self.mergeAdjacentLiterals:
             types = self.mergeLiterals(types)
+        return types
+
+    def parse(self,logic_string):
+        types = self.prepareTokens(logic_string)
         reversepolish = self.shunt(types)
         self.tree = self.treeify(reversepolish)
         return self.tree
 
     def stringify(self,f = None):
         if (self.tree is None):
             return None
```

### Comparing `logipar-0.5.0/logipar.egg-info/PKG-INFO` & `logipar-0.6.0/logipar.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: logipar
-Version: 0.5.0
+Version: 0.6.0
 Summary: A logic string parser
 Home-page: https://github.com/altef/logipar
 Author: Brad Gill
 Author-email: brad@alteredeffect.com
 License: UNKNOWN
 Description: [![npm](https://img.shields.io/npm/v/logipar)](https://npmjs.com/package/logipar) [![pypi](https://img.shields.io/pypi/v/logipar)](https://pypi.org/project/logipar/) [![haxelib install logipar](https://img.shields.io/badge/haxelib-logipar-orange, "haxelib install logipar")](https://lib.haxe.org/p/logipar/) [![php phar](https://img.shields.io/badge/php-Logipar.phar-orange, "PHP Logipar.phar")](https://github.com/altef/logipar/blob/master/php/Logipar.phar)
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: logipar Version: 0.5.0 Summary: A logic string
+Metadata-Version: 2.1 Name: logipar Version: 0.6.0 Summary: A logic string
 parser Home-page: https://github.com/altef/logipar Author: Brad Gill Author-
 email: brad@alteredeffect.com License: UNKNOWN Description: [![npm](https://
 img.shields.io/npm/v/logipar)](https://npmjs.com/package/logipar) [![pypi]
 (https://img.shields.io/pypi/v/logipar)](https://pypi.org/project/logipar/) [!
 [haxelib install logipar](https://img.shields.io/badge/haxelib-logipar-orange,
 "haxelib install logipar")](https://lib.haxe.org/p/logipar/) [![php phar]
 (https://img.shields.io/badge/php-Logipar.phar-orange, "PHP Logipar.phar")]
```

### Comparing `logipar-0.5.0/setup.py` & `logipar-0.6.0/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import setuptools
 
 with open("../../readme.md", "r", encoding="utf-8") as fh:
 	long_description = fh.read()
 
 setuptools.setup(
 	name="logipar",
-	version="0.5.0",
+	version="0.6.0",
 	author="Brad Gill",
 	author_email="brad@alteredeffect.com",
 	description="A logic string parser",
 	long_description=long_description,
 	long_description_content_type="text/markdown",
 	url="https://github.com/altef/logipar",
 	packages=setuptools.find_packages(),
```

