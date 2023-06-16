# Comparing `tmp/aleph-lang-0.9.0.tar.gz` & `tmp/aleph-lang-0.9.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "aleph-lang-0.9.0.tar", last modified: Wed Jun 14 06:09:51 2023, max compression
+gzip compressed data, was "aleph-lang-0.9.2.tar", last modified: Fri Jun 16 19:48:31 2023, max compression
```

## Comparing `aleph-lang-0.9.0.tar` & `aleph-lang-0.9.2.tar`

### file list

```diff
@@ -1,16 +1,16 @@
-drwxr-xr-x   0 anpaz      (501) staff       (20)        0 2023-06-14 06:09:51.894582 aleph-lang-0.9.0/
--rw-r--r--   0 anpaz      (501) staff       (20)     4470 2023-06-14 06:09:51.894034 aleph-lang-0.9.0/PKG-INFO
--rw-r--r--   0 anpaz      (501) staff       (20)     3933 2023-06-14 05:52:44.000000 aleph-lang-0.9.0/README.md
-drwxr-xr-x   0 anpaz      (501) staff       (20)        0 2023-06-14 06:09:51.887458 aleph-lang-0.9.0/aleph_lang/
--rw-r--r--   0 anpaz      (501) staff       (20)       79 2023-05-30 05:59:06.000000 aleph-lang-0.9.0/aleph_lang/__init__.py
--rw-r--r--   0 anpaz      (501) staff       (20)     7183 2023-06-14 05:57:52.000000 aleph-lang-0.9.0/aleph_lang/kets.py
-drwxr-xr-x   0 anpaz      (501) staff       (20)        0 2023-06-14 06:09:51.890545 aleph-lang-0.9.0/aleph_lang.egg-info/
--rw-r--r--   0 anpaz      (501) staff       (20)     4470 2023-06-14 06:09:51.000000 aleph-lang-0.9.0/aleph_lang.egg-info/PKG-INFO
--rw-r--r--   0 anpaz      (501) staff       (20)      248 2023-06-14 06:09:51.000000 aleph-lang-0.9.0/aleph_lang.egg-info/SOURCES.txt
--rw-r--r--   0 anpaz      (501) staff       (20)        1 2023-06-14 06:09:51.000000 aleph-lang-0.9.0/aleph_lang.egg-info/dependency_links.txt
--rw-r--r--   0 anpaz      (501) staff       (20)        9 2023-06-14 06:09:51.000000 aleph-lang-0.9.0/aleph_lang.egg-info/requires.txt
--rw-r--r--   0 anpaz      (501) staff       (20)       11 2023-06-14 06:09:51.000000 aleph-lang-0.9.0/aleph_lang.egg-info/top_level.txt
--rw-r--r--   0 anpaz      (501) staff       (20)       38 2023-06-14 06:09:51.894724 aleph-lang-0.9.0/setup.cfg
--rw-r--r--   0 anpaz      (501) staff       (20)      914 2023-06-14 06:07:21.000000 aleph-lang-0.9.0/setup.py
-drwxr-xr-x   0 anpaz      (501) staff       (20)        0 2023-06-14 06:09:51.891927 aleph-lang-0.9.0/tests/
--rw-r--r--   0 anpaz      (501) staff       (20)     6600 2023-05-30 17:28:01.000000 aleph-lang-0.9.0/tests/test_kets.py
+drwxr-xr-x   0 anpaz      (501) staff       (20)        0 2023-06-16 19:48:31.271818 aleph-lang-0.9.2/
+-rw-r--r--   0 anpaz      (501) staff       (20)     5786 2023-06-16 19:48:31.271161 aleph-lang-0.9.2/PKG-INFO
+-rw-r--r--   0 anpaz      (501) staff       (20)     5249 2023-06-16 18:52:07.000000 aleph-lang-0.9.2/README.md
+drwxr-xr-x   0 anpaz      (501) staff       (20)        0 2023-06-16 19:48:31.265282 aleph-lang-0.9.2/aleph_lang/
+-rw-r--r--   0 anpaz      (501) staff       (20)       79 2023-05-30 05:59:06.000000 aleph-lang-0.9.2/aleph_lang/__init__.py
+-rw-r--r--   0 anpaz      (501) staff       (20)     7183 2023-06-14 05:57:52.000000 aleph-lang-0.9.2/aleph_lang/kets.py
+drwxr-xr-x   0 anpaz      (501) staff       (20)        0 2023-06-16 19:48:31.268784 aleph-lang-0.9.2/aleph_lang.egg-info/
+-rw-r--r--   0 anpaz      (501) staff       (20)     5786 2023-06-16 19:48:31.000000 aleph-lang-0.9.2/aleph_lang.egg-info/PKG-INFO
+-rw-r--r--   0 anpaz      (501) staff       (20)      248 2023-06-16 19:48:31.000000 aleph-lang-0.9.2/aleph_lang.egg-info/SOURCES.txt
+-rw-r--r--   0 anpaz      (501) staff       (20)        1 2023-06-16 19:48:31.000000 aleph-lang-0.9.2/aleph_lang.egg-info/dependency_links.txt
+-rw-r--r--   0 anpaz      (501) staff       (20)        9 2023-06-16 19:48:31.000000 aleph-lang-0.9.2/aleph_lang.egg-info/requires.txt
+-rw-r--r--   0 anpaz      (501) staff       (20)       11 2023-06-16 19:48:31.000000 aleph-lang-0.9.2/aleph_lang.egg-info/top_level.txt
+-rw-r--r--   0 anpaz      (501) staff       (20)       38 2023-06-16 19:48:31.272044 aleph-lang-0.9.2/setup.cfg
+-rw-r--r--   0 anpaz      (501) staff       (20)      914 2023-06-16 19:42:50.000000 aleph-lang-0.9.2/setup.py
+drwxr-xr-x   0 anpaz      (501) staff       (20)        0 2023-06-16 19:48:31.269366 aleph-lang-0.9.2/tests/
+-rw-r--r--   0 anpaz      (501) staff       (20)     6600 2023-05-30 17:28:01.000000 aleph-lang-0.9.2/tests/test_kets.py
```

### Comparing `aleph-lang-0.9.0/PKG-INFO` & `aleph-lang-0.9.2/README.md`

 * *Files 18% similar despite different names*

```diff
@@ -1,87 +1,76 @@
-Metadata-Version: 2.1
-Name: aleph-lang
-Version: 0.9.0
-Summary: Python bindings for aleph, a high level programming model that can be embedded into classical languages to develop large scale quantum hybrid applications, without the quantum mechanics.
-Home-page: https://github.com/anpaz/aleph
-Author: Andrés Paz
-Author-email: anpaz@cs.washington.edu
-Classifier: Programming Language :: Python :: 3
-Classifier: License :: OSI Approved :: MIT License
-Classifier: Operating System :: OS Independent
-Description-Content-Type: text/markdown
-
 
 # aleph
 
 This package provides the Python bindings for `aleph`.
 
 `aleph` defines a high level programming model that can be embedded into classical languages to develop large scale quantum hybrid applications, without the quantum mechanics.
 
 ## Getting started
 
 To get started, install the aleph-lang package from PyPI:
 
-```
+```bash
 pip install aleph-lang
 ```
 
 
 ## Programming Model
 
 Expressions in Python take a single value, for example in the following program variable $x$ takes value 1:
 
-```
+```python
 x = 1
 print(x)
 
 # prints: 1
 ```
 
 `aleph` extends this model by allowing registers to take multiple values simultaneously. This is not achieved by defining a list structure that points to multiple values in memory, instead, all the values are in a single quantum register in *superposition*. We call this new type of register a Ket. 
 
 To construct a Ket in Python, create an instance of the `KetInt` or the `KetBool` class from the `aleph_lang` module. `KetInt` accepts an optional `width` argument to control the width (number of qubits) of the register, it defaults to 3. To read a value from a Ket use the `sample` method.
 
-```
+```python
 from aleph_lang import KetInt, sample
 
 random_number = KetInt(width=10)
 print(sample(random_number))
 
 #  it prints a number between 0 and 1023 (2^10 - 1).
 ```
 
-You can perform arithmetic and boolean expressions on Kets. Expression are applied simultaneoursly to all Ket elements on a single step using *quantum parallelism*. The result is a new Ket containing all possible outcomes of the evaluation.
+You can perform arithmetic and boolean expressions on Kets. Expression are applied simultaneously to all Ket elements on a single step using *quantum parallelism*. The result is a new Ket containing all possible outcomes of the evaluation.
 
 Input and output Kets of an expression are *entangled*, that is, when sampled the Ket's values are always correlated with each other. This entanglement is preserved across expressions. For example:
 
-```
+```python
 x = KetInt()
 y = x + 5
 z = 2 * y
 
 print(sample([x, y, z]))
 # prints [0, 5, 10] or [1, 6, 12] or [2, 7, 14] or ... [7, 12, 24)]
-# e.e. the value of the second element is the first plus five, 
+# e.g. the value of the second element is the first plus five, 
 # the third element is the second times two.
 ```
 
 You can filter the elements of a Ket using **where** expressions. For example, use `where_in` to filter the elements of a Ket to a specific list of items:
-```
+
+```python
 dice1 = KetInt().where_in(range(1,7))
 dice2 = KetInt().where_in(range(1,7))
 
 roll = dice1 + dice2
 print(sample([dice1, dice2, roll]))
 #prints [0,0,0] or [0,1,1] or [0,2,2] or ... [6,6,12]
 ```
 
 You can also filter the set of elements `sample` will return passing an optional `when` parameter; when provided, `sample` will return only elements that satisfy the given expression:
 
-```
+```python
 # Solve x + a == b * x 
 def solve_equation(a, b):
     x = KetInt()
     eq1 = x + a
     eq2 = b * x
 
     return sample(x, when=(eq1 == eq2))
@@ -91,27 +80,63 @@
 # prints 3
 ```
 
 Under the covers, **when** and **where** expressions use *amplitude amplification (a.k.a. Grover)* to amplify the probability of measuring the correct elements and filter out the rest.
 
 `sample` returns a single value; `aleph` also provides `histogram` to get the histogram resulting from the outcomes of sampling Kets multiple times; it takes a `rounds` parameter that indicates how many samples to take:
 
-```
+```python
 def dice_roll_histogram():
     dice1 = KetInt().where_in(range(1,7))
     dice2 = KetInt().where_in(range(1,7))
 
     roll = dice1 + dice2
     return histogram([roll], rounds=1000)
 ```
 
 
+It is safe to combine Kets with classical expressions, making it possible to create hybrid programs that leverage the host's language features. For example, the following function takes a graph information and the max number of colors to solve a graph coloring problem:
+
+```python
+# Solve a graph coloring problem, for the given number of nodes and list of edges.
+def graph_coloring(max_colors, nodes_count, edges):
+    def create_node():
+        w = width_for(max_colors)
+        return KetInt(width=w).where_less_than_equals(max_colors - 1)
+
+    def compare(edges):
+        if len(edges) == 1:
+            (left, right) = edges[0] 
+            return left != right
+        else:
+            head, *tail = edges
+            (left, right) = head
+            a = left != right
+            b = compare(tail)
+            return  a & b
+
+    nodes = [ create_node() for _ in range(nodes_count) ]
+    edges = [ (nodes[x], nodes[y]) for (x, y) in edges ]
+    filter = compare(edges)
+
+    ## Print to the console a graphviz representation
+    ## of the quantum graph:
+    ## tree(filter)
+
+    return sample(nodes, when=filter)
+
+max_colors = 3
+total_nodes = 4
+edges = [ (0, 1), (1, 2), (0, 2), (1, 3) ]
+print("graph coloring:", graph_coloring(max_colors, total_nodes, edges))
+```
+
 
 ## API server
 
 To simplify its setup `aleph` itself runs on the cloud. It uses an external service that at runtime keeps track of a program's quantum graph and enables its evaluation. No personal information is collected or accessible by the service. To change this behavior, you can run a local instance of the API server and set the `ALEPH_BASE_URL` environment variable to point to your local instance, for example:
 
-```
+```bash
 export ALEPH_BASE_URL=http://localhost:7071/
 ```
 
 Source code for `aleph`'s API server and instructions on how to build and run locally can be found at: https://github.com/anpaz/aleph/tree/main/src/api.
```

#### encoding

```diff
@@ -1 +1 @@
-utf-8
+us-ascii
```

### Comparing `aleph-lang-0.9.0/aleph_lang/kets.py` & `aleph-lang-0.9.2/aleph_lang/kets.py`

 * *Files identical despite different names*

### Comparing `aleph-lang-0.9.0/aleph_lang.egg-info/PKG-INFO` & `aleph-lang-0.9.2/PKG-INFO`

 * *Files 21% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: aleph-lang
-Version: 0.9.0
+Version: 0.9.2
 Summary: Python bindings for aleph, a high level programming model that can be embedded into classical languages to develop large scale quantum hybrid applications, without the quantum mechanics.
 Home-page: https://github.com/anpaz/aleph
 Author: Andrés Paz
 Author-email: anpaz@cs.washington.edu
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
@@ -17,71 +17,72 @@
 
 `aleph` defines a high level programming model that can be embedded into classical languages to develop large scale quantum hybrid applications, without the quantum mechanics.
 
 ## Getting started
 
 To get started, install the aleph-lang package from PyPI:
 
-```
+```bash
 pip install aleph-lang
 ```
 
 
 ## Programming Model
 
 Expressions in Python take a single value, for example in the following program variable $x$ takes value 1:
 
-```
+```python
 x = 1
 print(x)
 
 # prints: 1
 ```
 
 `aleph` extends this model by allowing registers to take multiple values simultaneously. This is not achieved by defining a list structure that points to multiple values in memory, instead, all the values are in a single quantum register in *superposition*. We call this new type of register a Ket. 
 
 To construct a Ket in Python, create an instance of the `KetInt` or the `KetBool` class from the `aleph_lang` module. `KetInt` accepts an optional `width` argument to control the width (number of qubits) of the register, it defaults to 3. To read a value from a Ket use the `sample` method.
 
-```
+```python
 from aleph_lang import KetInt, sample
 
 random_number = KetInt(width=10)
 print(sample(random_number))
 
 #  it prints a number between 0 and 1023 (2^10 - 1).
 ```
 
-You can perform arithmetic and boolean expressions on Kets. Expression are applied simultaneoursly to all Ket elements on a single step using *quantum parallelism*. The result is a new Ket containing all possible outcomes of the evaluation.
+You can perform arithmetic and boolean expressions on Kets. Expression are applied simultaneously to all Ket elements on a single step using *quantum parallelism*. The result is a new Ket containing all possible outcomes of the evaluation.
 
 Input and output Kets of an expression are *entangled*, that is, when sampled the Ket's values are always correlated with each other. This entanglement is preserved across expressions. For example:
 
-```
+```python
 x = KetInt()
 y = x + 5
 z = 2 * y
 
 print(sample([x, y, z]))
 # prints [0, 5, 10] or [1, 6, 12] or [2, 7, 14] or ... [7, 12, 24)]
-# e.e. the value of the second element is the first plus five, 
+# e.g. the value of the second element is the first plus five, 
 # the third element is the second times two.
 ```
 
 You can filter the elements of a Ket using **where** expressions. For example, use `where_in` to filter the elements of a Ket to a specific list of items:
-```
+
+```python
 dice1 = KetInt().where_in(range(1,7))
 dice2 = KetInt().where_in(range(1,7))
 
 roll = dice1 + dice2
 print(sample([dice1, dice2, roll]))
 #prints [0,0,0] or [0,1,1] or [0,2,2] or ... [6,6,12]
 ```
 
 You can also filter the set of elements `sample` will return passing an optional `when` parameter; when provided, `sample` will return only elements that satisfy the given expression:
 
-```
+```python
 # Solve x + a == b * x 
 def solve_equation(a, b):
     x = KetInt()
     eq1 = x + a
     eq2 = b * x
 
     return sample(x, when=(eq1 == eq2))
@@ -91,27 +92,63 @@
 # prints 3
 ```
 
 Under the covers, **when** and **where** expressions use *amplitude amplification (a.k.a. Grover)* to amplify the probability of measuring the correct elements and filter out the rest.
 
 `sample` returns a single value; `aleph` also provides `histogram` to get the histogram resulting from the outcomes of sampling Kets multiple times; it takes a `rounds` parameter that indicates how many samples to take:
 
-```
+```python
 def dice_roll_histogram():
     dice1 = KetInt().where_in(range(1,7))
     dice2 = KetInt().where_in(range(1,7))
 
     roll = dice1 + dice2
     return histogram([roll], rounds=1000)
 ```
 
 
+It is safe to combine Kets with classical expressions, making it possible to create hybrid programs that leverage the host's language features. For example, the following function takes a graph information and the max number of colors to solve a graph coloring problem:
+
+```python
+# Solve a graph coloring problem, for the given number of nodes and list of edges.
+def graph_coloring(max_colors, nodes_count, edges):
+    def create_node():
+        w = width_for(max_colors)
+        return KetInt(width=w).where_less_than_equals(max_colors - 1)
+
+    def compare(edges):
+        if len(edges) == 1:
+            (left, right) = edges[0] 
+            return left != right
+        else:
+            head, *tail = edges
+            (left, right) = head
+            a = left != right
+            b = compare(tail)
+            return  a & b
+
+    nodes = [ create_node() for _ in range(nodes_count) ]
+    edges = [ (nodes[x], nodes[y]) for (x, y) in edges ]
+    filter = compare(edges)
+
+    ## Print to the console a graphviz representation
+    ## of the quantum graph:
+    ## tree(filter)
+
+    return sample(nodes, when=filter)
+
+max_colors = 3
+total_nodes = 4
+edges = [ (0, 1), (1, 2), (0, 2), (1, 3) ]
+print("graph coloring:", graph_coloring(max_colors, total_nodes, edges))
+```
+
 
 ## API server
 
 To simplify its setup `aleph` itself runs on the cloud. It uses an external service that at runtime keeps track of a program's quantum graph and enables its evaluation. No personal information is collected or accessible by the service. To change this behavior, you can run a local instance of the API server and set the `ALEPH_BASE_URL` environment variable to point to your local instance, for example:
 
-```
+```bash
 export ALEPH_BASE_URL=http://localhost:7071/
 ```
 
 Source code for `aleph`'s API server and instructions on how to build and run locally can be found at: https://github.com/anpaz/aleph/tree/main/src/api.
```

### Comparing `aleph-lang-0.9.0/setup.py` & `aleph-lang-0.9.2/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 
 import setuptools
 import os
 
-version = os.environ.get('ALEPH_VERSION', '0.9.0')
+version = os.environ.get('ALEPH_VERSION', '0.9.2')
 
 with open("./README.md", "r") as fh:
     long_description = fh.read()
 
 setuptools.setup(
     name="aleph-lang",
     version=version,
```

### Comparing `aleph-lang-0.9.0/tests/test_kets.py` & `aleph-lang-0.9.2/tests/test_kets.py`

 * *Files identical despite different names*

