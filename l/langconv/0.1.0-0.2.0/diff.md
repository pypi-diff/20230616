# Comparing `tmp/langconv-0.1.0.tar.gz` & `tmp/langconv-0.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "langconv-0.1.0.tar", max compression
+gzip compressed data, was "langconv-0.2.0.tar", max compression
```

## Comparing `langconv-0.1.0.tar` & `langconv-0.2.0.tar`

### file list

```diff
@@ -1,15 +1,15 @@
--rw-r--r--   0        0        0        0 2023-06-13 11:02:31.374106 langconv-0.1.0/langconv/__init__.py
--rw-r--r--   0        0        0     8878 2023-06-16 07:07:36.316833 langconv-0.1.0/langconv/converter.py
--rw-r--r--   0        0        0    59813 2023-06-13 11:02:31.378101 langconv-0.1.0/langconv/data/zh/CN.json
--rw-r--r--   0        0        0    84966 2023-06-13 11:02:31.388106 langconv-0.1.0/langconv/data/zh/hans.json
--rw-r--r--   0        0        0   223215 2023-06-13 11:02:31.392105 langconv-0.1.0/langconv/data/zh/hant.json
--rw-r--r--   0        0        0    69719 2023-06-13 11:02:31.380105 langconv-0.1.0/langconv/data/zh/HK.json
--rw-r--r--   0        0        0      993 2023-06-13 11:02:31.383107 langconv-0.1.0/langconv/data/zh/LICENSE.md
--rw-r--r--   0        0        0    29369 2023-06-13 11:02:31.386103 langconv-0.1.0/langconv/data/zh/TW.json
--rw-r--r--   0        0        0      895 2023-06-16 07:07:36.317833 langconv-0.1.0/langconv/language/__init__.py
--rw-r--r--   0        0        0      604 2023-06-14 06:26:52.301870 langconv-0.1.0/langconv/language/zh.py
--rw-r--r--   0        0        0     3122 2023-06-16 07:07:36.317833 langconv-0.1.0/langconv/trie.py
--rw-r--r--   0        0        0      839 2023-06-16 07:07:36.319833 langconv-0.1.0/pyproject.toml
--rw-r--r--   0        0        0        0 2023-06-03 06:49:29.628350 langconv-0.1.0/README.md
--rw-r--r--   0        0        0      671 1970-01-01 00:00:00.000000 langconv-0.1.0/setup.py
--rw-r--r--   0        0        0      374 1970-01-01 00:00:00.000000 langconv-0.1.0/PKG-INFO
+-rw-r--r--   0        0        0        0 2023-06-13 11:02:31.374106 langconv-0.2.0/langconv/__init__.py
+-rw-r--r--   0        0        0     8878 2023-06-16 07:07:36.316833 langconv-0.2.0/langconv/converter.py
+-rw-r--r--   0        0        0    59813 2023-06-13 11:02:31.378101 langconv-0.2.0/langconv/data/zh/CN.json
+-rw-r--r--   0        0        0    84966 2023-06-13 11:02:31.388106 langconv-0.2.0/langconv/data/zh/hans.json
+-rw-r--r--   0        0        0   223215 2023-06-13 11:02:31.392105 langconv-0.2.0/langconv/data/zh/hant.json
+-rw-r--r--   0        0        0    69719 2023-06-13 11:02:31.380105 langconv-0.2.0/langconv/data/zh/HK.json
+-rw-r--r--   0        0        0      993 2023-06-13 11:02:31.383107 langconv-0.2.0/langconv/data/zh/LICENSE.md
+-rw-r--r--   0        0        0    29369 2023-06-13 11:02:31.386103 langconv-0.2.0/langconv/data/zh/TW.json
+-rw-r--r--   0        0        0      895 2023-06-16 07:07:36.317833 langconv-0.2.0/langconv/language/__init__.py
+-rw-r--r--   0        0        0      604 2023-06-14 06:26:52.301870 langconv-0.2.0/langconv/language/zh.py
+-rw-r--r--   0        0        0     3202 2023-06-16 07:25:08.114094 langconv-0.2.0/langconv/trie.py
+-rw-r--r--   0        0        0      838 2023-06-16 07:26:56.381785 langconv-0.2.0/pyproject.toml
+-rw-r--r--   0        0        0        0 2023-06-03 06:49:29.628350 langconv-0.2.0/README.md
+-rw-r--r--   0        0        0      670 1970-01-01 00:00:00.000000 langconv-0.2.0/setup.py
+-rw-r--r--   0        0        0      524 1970-01-01 00:00:00.000000 langconv-0.2.0/PKG-INFO
```

### Comparing `langconv-0.1.0/langconv/converter.py` & `langconv-0.2.0/langconv/converter.py`

 * *Files identical despite different names*

### Comparing `langconv-0.1.0/langconv/data/zh/CN.json` & `langconv-0.2.0/langconv/data/zh/CN.json`

 * *Files identical despite different names*

### Comparing `langconv-0.1.0/langconv/data/zh/hans.json` & `langconv-0.2.0/langconv/data/zh/hans.json`

 * *Files identical despite different names*

### Comparing `langconv-0.1.0/langconv/data/zh/hant.json` & `langconv-0.2.0/langconv/data/zh/hant.json`

 * *Files identical despite different names*

### Comparing `langconv-0.1.0/langconv/data/zh/HK.json` & `langconv-0.2.0/langconv/data/zh/HK.json`

 * *Files identical despite different names*

### Comparing `langconv-0.1.0/langconv/data/zh/LICENSE.md` & `langconv-0.2.0/langconv/data/zh/LICENSE.md`

 * *Files identical despite different names*

### Comparing `langconv-0.1.0/langconv/data/zh/TW.json` & `langconv-0.2.0/langconv/data/zh/TW.json`

 * *Files identical despite different names*

### Comparing `langconv-0.1.0/langconv/language/__init__.py` & `langconv-0.2.0/langconv/language/__init__.py`

 * *Files identical despite different names*

### Comparing `langconv-0.1.0/langconv/language/zh.py` & `langconv-0.2.0/langconv/language/zh.py`

 * *Files identical despite different names*

### Comparing `langconv-0.1.0/langconv/trie.py` & `langconv-0.2.0/langconv/trie.py`

 * *Files 4% similar despite different names*

```diff
@@ -53,23 +53,23 @@
             if parent is None:
                 self.root = Node('', '', '')
                 break
             parent.children.pop(node.key, None)
             node = parent
             if hasattr(node, 'children') and len(node.children) > 0:
                 break
-            node.parent.children.pop(node.key, None)
+            node.parent.children.pop(node.key, None) # type: ignore If it has a parent, then parent must has children
             node = node.parent
 
     def longest_prefix(self, key: str) -> Node | None:
         node = self.root
         longest_match = None
         for char in key:
             child_node = node.get_child(char)
-            if child_node is None or not key.startswith(child_node.full_key):
+            if child_node is None or key[0:len(child_node.full_key)] != child_node.full_key:
                 break
             node = child_node
             longest_match = node
         while longest_match is not None and not longest_match.value:
             longest_match = longest_match.parent
         return longest_match
```

### Comparing `langconv-0.1.0/pyproject.toml` & `langconv-0.2.0/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,16 +1,16 @@
 [tool.poetry]
 name = "langconv"
-version = "0.1.0"
+version = "0.2.0"
 description = ""
 authors = ["Dianliang233 <dianliang233@gmail.com>"]
 readme = "README.md"
 
 [tool.poetry.dependencies]
-python = "^3.11"
+python = "^3.8"
 attrs = "^23.1.0"
 iso639-lang = "^2.1.0"
 
 [tool.poetry.group.dev.dependencies]
 autopep8 = "^2.0.2"
 ruff = "^0.0.267"
 pytest = "^7.3.1"
```

### Comparing `langconv-0.1.0/setup.py` & `langconv-0.2.0/setup.py`

 * *Files 15% similar despite different names*

```diff
@@ -8,23 +8,23 @@
 {'': ['*'], 'langconv': ['data/zh/*']}
 
 install_requires = \
 ['attrs>=23.1.0,<24.0.0', 'iso639-lang>=2.1.0,<3.0.0']
 
 setup_kwargs = {
     'name': 'langconv',
-    'version': '0.1.0',
+    'version': '0.2.0',
     'description': '',
     'long_description': '',
     'author': 'Dianliang233',
     'author_email': 'dianliang233@gmail.com',
     'maintainer': 'None',
     'maintainer_email': 'None',
     'url': 'None',
     'packages': packages,
     'package_data': package_data,
     'install_requires': install_requires,
-    'python_requires': '>=3.11,<4.0',
+    'python_requires': '>=3.8,<4.0',
 }
 
 
 setup(**setup_kwargs)
```

