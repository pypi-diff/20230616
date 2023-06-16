# Comparing `tmp/visuallm-0.1.7.tar.gz` & `tmp/visuallm-0.1.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "visuallm-0.1.7.tar", last modified: Thu Jun 15 16:35:28 2023, max compression
+gzip compressed data, was "visuallm-0.1.8.tar", last modified: Fri Jun 16 07:31:50 2023, max compression
```

## Comparing `visuallm-0.1.7.tar` & `visuallm-0.1.8.tar`

### file list

```diff
@@ -1,38 +1,38 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 16:35:28.180137 visuallm-0.1.7/
--rw-r--r--   0 runner    (1001) docker     (123)     1075 2023-06-15 16:35:16.000000 visuallm-0.1.7/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)       20 2023-06-15 16:35:16.000000 visuallm-0.1.7/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)    20371 2023-06-15 16:35:28.180137 visuallm-0.1.7/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    19777 2023-06-15 16:35:16.000000 visuallm-0.1.7/README.md
--rw-r--r--   0 runner    (1001) docker     (123)     1246 2023-06-15 16:35:16.000000 visuallm-0.1.7/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-15 16:35:28.180137 visuallm-0.1.7/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 16:35:28.176137 visuallm-0.1.7/visuallm/
--rw-r--r--   0 runner    (1001) docker     (123)     2777 2023-06-15 16:35:16.000000 visuallm-0.1.7/visuallm/component_base.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 16:35:28.176137 visuallm-0.1.7/visuallm/components/
--rw-r--r--   0 runner    (1001) docker     (123)     1527 2023-06-15 16:35:16.000000 visuallm-0.1.7/visuallm/components/DatasetVisualizationComponent.py
--rw-r--r--   0 runner    (1001) docker     (123)     7071 2023-06-15 16:35:16.000000 visuallm-0.1.7/visuallm/components/GenerationComponent.py
--rw-r--r--   0 runner    (1001) docker     (123)     4992 2023-06-15 16:35:16.000000 visuallm-0.1.7/visuallm/components/NextTokenPredictionComponent.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 16:35:28.176137 visuallm-0.1.7/visuallm/components/mixins/
--rw-r--r--   0 runner    (1001) docker     (123)     5850 2023-06-15 16:35:16.000000 visuallm-0.1.7/visuallm/components/mixins/data_preparation_mixin.py
--rw-r--r--   0 runner    (1001) docker     (123)     3244 2023-06-15 16:35:16.000000 visuallm-0.1.7/visuallm/components/mixins/generation_selectors_mixin.py
--rw-r--r--   0 runner    (1001) docker     (123)     6144 2023-06-15 16:35:16.000000 visuallm-0.1.7/visuallm/components/mixins/metrics_mixin.py
--rw-r--r--   0 runner    (1001) docker     (123)     3378 2023-06-15 16:35:16.000000 visuallm-0.1.7/visuallm/components/mixins/model_selection_mixin.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 16:35:28.176137 visuallm-0.1.7/visuallm/dist/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 16:35:28.176137 visuallm-0.1.7/visuallm/dist/assets/
--rw-r--r--   0 runner    (1001) docker     (123)   201746 2023-06-15 16:35:16.000000 visuallm-0.1.7/visuallm/dist/assets/index-9006265c.js
--rw-r--r--   0 runner    (1001) docker     (123)     7891 2023-06-15 16:35:16.000000 visuallm-0.1.7/visuallm/dist/assets/index-d8f16c2e.css
--rw-r--r--   0 runner    (1001) docker     (123)     4286 2023-06-15 16:35:16.000000 visuallm-0.1.7/visuallm/dist/favicon.ico
--rw-r--r--   0 runner    (1001) docker     (123)      424 2023-06-15 16:35:16.000000 visuallm-0.1.7/visuallm/dist/index.html
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 16:35:28.180137 visuallm-0.1.7/visuallm/elements/
--rw-r--r--   0 runner    (1001) docker     (123)     5705 2023-06-15 16:35:16.000000 visuallm-0.1.7/visuallm/elements/barchart_element.py
--rw-r--r--   0 runner    (1001) docker     (123)     2162 2023-06-15 16:35:16.000000 visuallm-0.1.7/visuallm/elements/element_base.py
--rw-r--r--   0 runner    (1001) docker     (123)      968 2023-06-15 16:35:16.000000 visuallm-0.1.7/visuallm/elements/plain_text_element.py
--rw-r--r--   0 runner    (1001) docker     (123)     9952 2023-06-15 16:35:16.000000 visuallm-0.1.7/visuallm/elements/selector_elements.py
--rw-r--r--   0 runner    (1001) docker     (123)     4188 2023-06-15 16:35:16.000000 visuallm-0.1.7/visuallm/elements/table_element.py
--rw-r--r--   0 runner    (1001) docker     (123)     1462 2023-06-15 16:35:16.000000 visuallm-0.1.7/visuallm/elements/utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     2049 2023-06-15 16:35:16.000000 visuallm-0.1.7/visuallm/server.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 16:35:28.176137 visuallm-0.1.7/visuallm.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    20371 2023-06-15 16:35:28.000000 visuallm-0.1.7/visuallm.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      946 2023-06-15 16:35:28.000000 visuallm-0.1.7/visuallm.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-15 16:35:28.000000 visuallm-0.1.7/visuallm.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       69 2023-06-15 16:35:28.000000 visuallm-0.1.7/visuallm.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        9 2023-06-15 16:35:28.000000 visuallm-0.1.7/visuallm.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 07:31:50.872942 visuallm-0.1.8/
+-rw-r--r--   0 runner    (1001) docker     (123)     1075 2023-06-16 07:31:36.000000 visuallm-0.1.8/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)       20 2023-06-16 07:31:36.000000 visuallm-0.1.8/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)    19599 2023-06-16 07:31:50.872942 visuallm-0.1.8/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    19005 2023-06-16 07:31:36.000000 visuallm-0.1.8/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)     1246 2023-06-16 07:31:36.000000 visuallm-0.1.8/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-16 07:31:50.872942 visuallm-0.1.8/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 07:31:50.872942 visuallm-0.1.8/visuallm/
+-rw-r--r--   0 runner    (1001) docker     (123)     2777 2023-06-16 07:31:36.000000 visuallm-0.1.8/visuallm/component_base.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 07:31:50.872942 visuallm-0.1.8/visuallm/components/
+-rw-r--r--   0 runner    (1001) docker     (123)     1527 2023-06-16 07:31:36.000000 visuallm-0.1.8/visuallm/components/DatasetVisualizationComponent.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7071 2023-06-16 07:31:36.000000 visuallm-0.1.8/visuallm/components/GenerationComponent.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4992 2023-06-16 07:31:36.000000 visuallm-0.1.8/visuallm/components/NextTokenPredictionComponent.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 07:31:50.872942 visuallm-0.1.8/visuallm/components/mixins/
+-rw-r--r--   0 runner    (1001) docker     (123)     5850 2023-06-16 07:31:36.000000 visuallm-0.1.8/visuallm/components/mixins/data_preparation_mixin.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3244 2023-06-16 07:31:36.000000 visuallm-0.1.8/visuallm/components/mixins/generation_selectors_mixin.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6144 2023-06-16 07:31:36.000000 visuallm-0.1.8/visuallm/components/mixins/metrics_mixin.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3378 2023-06-16 07:31:36.000000 visuallm-0.1.8/visuallm/components/mixins/model_selection_mixin.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 07:31:50.872942 visuallm-0.1.8/visuallm/dist/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 07:31:50.872942 visuallm-0.1.8/visuallm/dist/assets/
+-rw-r--r--   0 runner    (1001) docker     (123)   201746 2023-06-16 07:31:36.000000 visuallm-0.1.8/visuallm/dist/assets/index-9006265c.js
+-rw-r--r--   0 runner    (1001) docker     (123)     7891 2023-06-16 07:31:36.000000 visuallm-0.1.8/visuallm/dist/assets/index-d8f16c2e.css
+-rw-r--r--   0 runner    (1001) docker     (123)     4286 2023-06-16 07:31:36.000000 visuallm-0.1.8/visuallm/dist/favicon.ico
+-rw-r--r--   0 runner    (1001) docker     (123)      424 2023-06-16 07:31:36.000000 visuallm-0.1.8/visuallm/dist/index.html
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 07:31:50.872942 visuallm-0.1.8/visuallm/elements/
+-rw-r--r--   0 runner    (1001) docker     (123)     5705 2023-06-16 07:31:36.000000 visuallm-0.1.8/visuallm/elements/barchart_element.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2162 2023-06-16 07:31:36.000000 visuallm-0.1.8/visuallm/elements/element_base.py
+-rw-r--r--   0 runner    (1001) docker     (123)      968 2023-06-16 07:31:36.000000 visuallm-0.1.8/visuallm/elements/plain_text_element.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9952 2023-06-16 07:31:36.000000 visuallm-0.1.8/visuallm/elements/selector_elements.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4188 2023-06-16 07:31:36.000000 visuallm-0.1.8/visuallm/elements/table_element.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1462 2023-06-16 07:31:36.000000 visuallm-0.1.8/visuallm/elements/utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2049 2023-06-16 07:31:36.000000 visuallm-0.1.8/visuallm/server.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 07:31:50.872942 visuallm-0.1.8/visuallm.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    19599 2023-06-16 07:31:50.000000 visuallm-0.1.8/visuallm.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      946 2023-06-16 07:31:50.000000 visuallm-0.1.8/visuallm.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-16 07:31:50.000000 visuallm-0.1.8/visuallm.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       69 2023-06-16 07:31:50.000000 visuallm-0.1.8/visuallm.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        9 2023-06-16 07:31:50.000000 visuallm-0.1.8/visuallm.egg-info/top_level.txt
```

### Comparing `visuallm-0.1.7/LICENSE` & `visuallm-0.1.8/LICENSE`

 * *Files identical despite different names*

### Comparing `visuallm-0.1.7/PKG-INFO` & `visuallm-0.1.8/README.md`

 * *Files 3% similar despite different names*

```diff
@@ -1,47 +1,32 @@
-Metadata-Version: 2.1
-Name: visuallm
-Version: 0.1.7
-Summary: Visualization tool for various generation tasks on Language Models. 
-Author-email: "Frantisek Trebuna (gortibaldik)" <ferotre@gmail.com>
-Project-URL: Homepage, https://github.com/gortibaldik/visuallm
-Project-URL: Bug Tracker, https://github.com/gortibaldik/visuallm/issues
-Classifier: Programming Language :: Python :: 3
-Classifier: License :: OSI Approved :: MIT License
-Classifier: Operating System :: OS Independent
-Requires-Python: >=3.9
-Description-Content-Type: text/markdown
-Provides-Extra: huggingface
-License-File: LICENSE
-
 # Conditional Language Model Generation Visualization
 
-## VERSION: `0.1.7`
+## VERSION: `0.1.8`
 
 - when evaluating language models it is often pain to see what is generated and why
 - this little package is a `vue.js` frontend together with `flask` backend and it is designed to easily show some interesting visualizations on conditional generation models
 - it handles frontend-backend communication as well as frontend rendering
 - hence the developper can focus only on ML aspects of his work!
 
-## Installation
+<!-- ## Installation
 
 - install from pypi:
-  - `pip install visuallm`
+  - `pip install visuallm` -->
 
 ## Usage
 
 The library is composed of three parts:
 
-1. Server - `llm_generation_server.server.Server`
-2. Component - `llm_generation_server.component_base.ComponentBase`
-3. Elements - `llm_generation_server.elements.*`
+1. Server - `visuallm.server.Server`
+2. Component - `visuallm.component_base.ComponentBase`
+3. Elements - `visuallm.elements.*`
 
 ### Expected Workflow
 
-1. Create a class inheriting from `llm_generation_server.component_base.ComponentBase`. In `__init__` you should:
+1. Create a class inheriting from `visuallm.component_base.ComponentBase`. In `__init__` you should:
 
 - create all the elements from which the page should be composed
 
 <!-- MARKDOWN-AUTO-DOCS:START (CODE:src=./examples_py/simple_component.py&lines=1-15&header=# ./examples_py/simple_component.py lines 1-15)-->
 <!-- The below code snippet is automatically added from ./examples_py/simple_component.py -->
 ```py
 # ./examples_py/simple_component.py lines 1-15
@@ -334,45 +319,23 @@
 class TwoTablesComponent(ComponentBase):
     def __init__(self):
 ```
 <!-- MARKDOWN-AUTO-DOCS:END-->
 
 Secondly, we will create the links in such a way, that links going within the same table will be colored orange (the default color), while the links going to the other table will be colored light blue. Also links within one table will be thin, while links to the other table will be thick (`Importance` parameter).
 
-<!-- MARKDOWN-AUTO-DOCS:START (CODE:src=./examples_py/two_tables_component.py&header=# ./examples_py/two_tables_component.py lines 69-99&lines=69-99)-->
+<!-- MARKDOWN-AUTO-DOCS:START (CODE:src=./examples_py/two_tables_component.py&header=# ./examples_py/two_tables_component.py lines 65-69&lines=65-69)-->
 <!-- The below code snippet is automatically added from ./examples_py/two_tables_component.py -->
 ```py
-# ./examples_py/two_tables_component.py lines 69-99
+# ./examples_py/two_tables_component.py lines 65-69
+        # add links pointing from each row of the second table to all the rows
+        # of the first table and also to all the rows of the second table
+        # upwards
+        for j in range(len(rows[1]) - 1, 0, -1):
             # links going from the row j of the second table to all the upper
-            # rows in the second table
-            for i in range(j):
-                self.table_element.add_link_between_rows(
-                    LinkBetweenRows(
-                        TABLE_NAMES[1],
-                        j,
-                        TABLE_NAMES[1],
-                        i,
-                        Importance=1,
-                        Label="to_second_table",
-                    )
-                )
-
-            # links going from the row j to all the rows in the first table
-            for i in range(len(rows[0])):
-                self.table_element.add_link_between_rows(
-                    LinkBetweenRows(
-                        TABLE_NAMES[1],
-                        j,
-                        TABLE_NAMES[0],
-                        i,
-                        Label="to_first_table",
-                        Importance=4,
-                        Color=Colors.LIGHT_BLUE,
-                    )
-                )
 ```
 <!-- MARKDOWN-AUTO-DOCS:END-->
 
 ![table_advanced](./readme_images/table_advanced.png)
 
 #### BarChart Element
```

### Comparing `visuallm-0.1.7/README.md` & `visuallm-0.1.8/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,32 +1,47 @@
+Metadata-Version: 2.1
+Name: visuallm
+Version: 0.1.8
+Summary: Visualization tool for various generation tasks on Language Models. 
+Author-email: "Frantisek Trebuna (gortibaldik)" <ferotre@gmail.com>
+Project-URL: Homepage, https://github.com/gortibaldik/visuallm
+Project-URL: Bug Tracker, https://github.com/gortibaldik/visuallm/issues
+Classifier: Programming Language :: Python :: 3
+Classifier: License :: OSI Approved :: MIT License
+Classifier: Operating System :: OS Independent
+Requires-Python: >=3.9
+Description-Content-Type: text/markdown
+Provides-Extra: huggingface
+License-File: LICENSE
+
 # Conditional Language Model Generation Visualization
 
-## VERSION: `0.1.7`
+## VERSION: `0.1.8`
 
 - when evaluating language models it is often pain to see what is generated and why
 - this little package is a `vue.js` frontend together with `flask` backend and it is designed to easily show some interesting visualizations on conditional generation models
 - it handles frontend-backend communication as well as frontend rendering
 - hence the developper can focus only on ML aspects of his work!
 
-## Installation
+<!-- ## Installation
 
 - install from pypi:
-  - `pip install visuallm`
+  - `pip install visuallm` -->
 
 ## Usage
 
 The library is composed of three parts:
 
-1. Server - `llm_generation_server.server.Server`
-2. Component - `llm_generation_server.component_base.ComponentBase`
-3. Elements - `llm_generation_server.elements.*`
+1. Server - `visuallm.server.Server`
+2. Component - `visuallm.component_base.ComponentBase`
+3. Elements - `visuallm.elements.*`
 
 ### Expected Workflow
 
-1. Create a class inheriting from `llm_generation_server.component_base.ComponentBase`. In `__init__` you should:
+1. Create a class inheriting from `visuallm.component_base.ComponentBase`. In `__init__` you should:
 
 - create all the elements from which the page should be composed
 
 <!-- MARKDOWN-AUTO-DOCS:START (CODE:src=./examples_py/simple_component.py&lines=1-15&header=# ./examples_py/simple_component.py lines 1-15)-->
 <!-- The below code snippet is automatically added from ./examples_py/simple_component.py -->
 ```py
 # ./examples_py/simple_component.py lines 1-15
@@ -319,45 +334,23 @@
 class TwoTablesComponent(ComponentBase):
     def __init__(self):
 ```
 <!-- MARKDOWN-AUTO-DOCS:END-->
 
 Secondly, we will create the links in such a way, that links going within the same table will be colored orange (the default color), while the links going to the other table will be colored light blue. Also links within one table will be thin, while links to the other table will be thick (`Importance` parameter).
 
-<!-- MARKDOWN-AUTO-DOCS:START (CODE:src=./examples_py/two_tables_component.py&header=# ./examples_py/two_tables_component.py lines 69-99&lines=69-99)-->
+<!-- MARKDOWN-AUTO-DOCS:START (CODE:src=./examples_py/two_tables_component.py&header=# ./examples_py/two_tables_component.py lines 65-69&lines=65-69)-->
 <!-- The below code snippet is automatically added from ./examples_py/two_tables_component.py -->
 ```py
-# ./examples_py/two_tables_component.py lines 69-99
+# ./examples_py/two_tables_component.py lines 65-69
+        # add links pointing from each row of the second table to all the rows
+        # of the first table and also to all the rows of the second table
+        # upwards
+        for j in range(len(rows[1]) - 1, 0, -1):
             # links going from the row j of the second table to all the upper
-            # rows in the second table
-            for i in range(j):
-                self.table_element.add_link_between_rows(
-                    LinkBetweenRows(
-                        TABLE_NAMES[1],
-                        j,
-                        TABLE_NAMES[1],
-                        i,
-                        Importance=1,
-                        Label="to_second_table",
-                    )
-                )
-
-            # links going from the row j to all the rows in the first table
-            for i in range(len(rows[0])):
-                self.table_element.add_link_between_rows(
-                    LinkBetweenRows(
-                        TABLE_NAMES[1],
-                        j,
-                        TABLE_NAMES[0],
-                        i,
-                        Label="to_first_table",
-                        Importance=4,
-                        Color=Colors.LIGHT_BLUE,
-                    )
-                )
 ```
 <!-- MARKDOWN-AUTO-DOCS:END-->
 
 ![table_advanced](./readme_images/table_advanced.png)
 
 #### BarChart Element
```

### Comparing `visuallm-0.1.7/pyproject.toml` & `visuallm-0.1.8/pyproject.toml`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [project]
 name = "visuallm"
-version = "0.1.7"
+version = "0.1.8"
 authors = [
   { name="Frantisek Trebuna (gortibaldik)", email="ferotre@gmail.com" },
 ]
 description = "Visualization tool for various generation tasks on Language Models. "
 readme = "README.md"
 requires-python = ">=3.9"
 classifiers = [
@@ -34,15 +34,15 @@
 [tool.setuptools.package-dir]
 visuallm = "visuallm"
 
 [tool.isort]
 profile = "black"
 
 [tool.bumpver]
-current_version = "0.1.7"
+current_version = "0.1.8"
 version_pattern = "MAJOR.MINOR.PATCH"
 commit_message = "bump version {old_version} -> {new_version}"
 commit = true
 tag = true
 push = true
 
 [tool.bumpver.file_patterns]
```

### Comparing `visuallm-0.1.7/visuallm/component_base.py` & `visuallm-0.1.8/visuallm/component_base.py`

 * *Files identical despite different names*

### Comparing `visuallm-0.1.7/visuallm/components/DatasetVisualizationComponent.py` & `visuallm-0.1.8/visuallm/components/DatasetVisualizationComponent.py`

 * *Files identical despite different names*

### Comparing `visuallm-0.1.7/visuallm/components/GenerationComponent.py` & `visuallm-0.1.8/visuallm/components/GenerationComponent.py`

 * *Files identical despite different names*

### Comparing `visuallm-0.1.7/visuallm/components/NextTokenPredictionComponent.py` & `visuallm-0.1.8/visuallm/components/NextTokenPredictionComponent.py`

 * *Files identical despite different names*

### Comparing `visuallm-0.1.7/visuallm/components/mixins/data_preparation_mixin.py` & `visuallm-0.1.8/visuallm/components/mixins/data_preparation_mixin.py`

 * *Files identical despite different names*

### Comparing `visuallm-0.1.7/visuallm/components/mixins/generation_selectors_mixin.py` & `visuallm-0.1.8/visuallm/components/mixins/generation_selectors_mixin.py`

 * *Files identical despite different names*

### Comparing `visuallm-0.1.7/visuallm/components/mixins/metrics_mixin.py` & `visuallm-0.1.8/visuallm/components/mixins/metrics_mixin.py`

 * *Files identical despite different names*

### Comparing `visuallm-0.1.7/visuallm/components/mixins/model_selection_mixin.py` & `visuallm-0.1.8/visuallm/components/mixins/model_selection_mixin.py`

 * *Files identical despite different names*

### Comparing `visuallm-0.1.7/visuallm/dist/assets/index-9006265c.js` & `visuallm-0.1.8/visuallm/dist/assets/index-9006265c.js`

 * *Files identical despite different names*

### Comparing `visuallm-0.1.7/visuallm/dist/assets/index-d8f16c2e.css` & `visuallm-0.1.8/visuallm/dist/assets/index-d8f16c2e.css`

 * *Files identical despite different names*

### Comparing `visuallm-0.1.7/visuallm/dist/favicon.ico` & `visuallm-0.1.8/visuallm/dist/favicon.ico`

 * *Files identical despite different names*

### Comparing `visuallm-0.1.7/visuallm/elements/barchart_element.py` & `visuallm-0.1.8/visuallm/elements/barchart_element.py`

 * *Files identical despite different names*

### Comparing `visuallm-0.1.7/visuallm/elements/element_base.py` & `visuallm-0.1.8/visuallm/elements/element_base.py`

 * *Files identical despite different names*

### Comparing `visuallm-0.1.7/visuallm/elements/plain_text_element.py` & `visuallm-0.1.8/visuallm/elements/plain_text_element.py`

 * *Files identical despite different names*

### Comparing `visuallm-0.1.7/visuallm/elements/selector_elements.py` & `visuallm-0.1.8/visuallm/elements/selector_elements.py`

 * *Files identical despite different names*

### Comparing `visuallm-0.1.7/visuallm/elements/table_element.py` & `visuallm-0.1.8/visuallm/elements/table_element.py`

 * *Files identical despite different names*

### Comparing `visuallm-0.1.7/visuallm/elements/utils.py` & `visuallm-0.1.8/visuallm/elements/utils.py`

 * *Files identical despite different names*

### Comparing `visuallm-0.1.7/visuallm/server.py` & `visuallm-0.1.8/visuallm/server.py`

 * *Files identical despite different names*

### Comparing `visuallm-0.1.7/visuallm.egg-info/PKG-INFO` & `visuallm-0.1.8/visuallm.egg-info/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,47 +1,47 @@
 Metadata-Version: 2.1
 Name: visuallm
-Version: 0.1.7
+Version: 0.1.8
 Summary: Visualization tool for various generation tasks on Language Models. 
 Author-email: "Frantisek Trebuna (gortibaldik)" <ferotre@gmail.com>
 Project-URL: Homepage, https://github.com/gortibaldik/visuallm
 Project-URL: Bug Tracker, https://github.com/gortibaldik/visuallm/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.9
 Description-Content-Type: text/markdown
 Provides-Extra: huggingface
 License-File: LICENSE
 
 # Conditional Language Model Generation Visualization
 
-## VERSION: `0.1.7`
+## VERSION: `0.1.8`
 
 - when evaluating language models it is often pain to see what is generated and why
 - this little package is a `vue.js` frontend together with `flask` backend and it is designed to easily show some interesting visualizations on conditional generation models
 - it handles frontend-backend communication as well as frontend rendering
 - hence the developper can focus only on ML aspects of his work!
 
-## Installation
+<!-- ## Installation
 
 - install from pypi:
-  - `pip install visuallm`
+  - `pip install visuallm` -->
 
 ## Usage
 
 The library is composed of three parts:
 
-1. Server - `llm_generation_server.server.Server`
-2. Component - `llm_generation_server.component_base.ComponentBase`
-3. Elements - `llm_generation_server.elements.*`
+1. Server - `visuallm.server.Server`
+2. Component - `visuallm.component_base.ComponentBase`
+3. Elements - `visuallm.elements.*`
 
 ### Expected Workflow
 
-1. Create a class inheriting from `llm_generation_server.component_base.ComponentBase`. In `__init__` you should:
+1. Create a class inheriting from `visuallm.component_base.ComponentBase`. In `__init__` you should:
 
 - create all the elements from which the page should be composed
 
 <!-- MARKDOWN-AUTO-DOCS:START (CODE:src=./examples_py/simple_component.py&lines=1-15&header=# ./examples_py/simple_component.py lines 1-15)-->
 <!-- The below code snippet is automatically added from ./examples_py/simple_component.py -->
 ```py
 # ./examples_py/simple_component.py lines 1-15
@@ -334,45 +334,23 @@
 class TwoTablesComponent(ComponentBase):
     def __init__(self):
 ```
 <!-- MARKDOWN-AUTO-DOCS:END-->
 
 Secondly, we will create the links in such a way, that links going within the same table will be colored orange (the default color), while the links going to the other table will be colored light blue. Also links within one table will be thin, while links to the other table will be thick (`Importance` parameter).
 
-<!-- MARKDOWN-AUTO-DOCS:START (CODE:src=./examples_py/two_tables_component.py&header=# ./examples_py/two_tables_component.py lines 69-99&lines=69-99)-->
+<!-- MARKDOWN-AUTO-DOCS:START (CODE:src=./examples_py/two_tables_component.py&header=# ./examples_py/two_tables_component.py lines 65-69&lines=65-69)-->
 <!-- The below code snippet is automatically added from ./examples_py/two_tables_component.py -->
 ```py
-# ./examples_py/two_tables_component.py lines 69-99
+# ./examples_py/two_tables_component.py lines 65-69
+        # add links pointing from each row of the second table to all the rows
+        # of the first table and also to all the rows of the second table
+        # upwards
+        for j in range(len(rows[1]) - 1, 0, -1):
             # links going from the row j of the second table to all the upper
-            # rows in the second table
-            for i in range(j):
-                self.table_element.add_link_between_rows(
-                    LinkBetweenRows(
-                        TABLE_NAMES[1],
-                        j,
-                        TABLE_NAMES[1],
-                        i,
-                        Importance=1,
-                        Label="to_second_table",
-                    )
-                )
-
-            # links going from the row j to all the rows in the first table
-            for i in range(len(rows[0])):
-                self.table_element.add_link_between_rows(
-                    LinkBetweenRows(
-                        TABLE_NAMES[1],
-                        j,
-                        TABLE_NAMES[0],
-                        i,
-                        Label="to_first_table",
-                        Importance=4,
-                        Color=Colors.LIGHT_BLUE,
-                    )
-                )
 ```
 <!-- MARKDOWN-AUTO-DOCS:END-->
 
 ![table_advanced](./readme_images/table_advanced.png)
 
 #### BarChart Element
```

### Comparing `visuallm-0.1.7/visuallm.egg-info/SOURCES.txt` & `visuallm-0.1.8/visuallm.egg-info/SOURCES.txt`

 * *Files identical despite different names*

