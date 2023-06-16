# Comparing `tmp/CSET-0.1.0.tar.gz` & `tmp/CSET-0.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "CSET-0.1.0.tar", last modified: Mon Apr 24 15:43:23 2023, max compression
+gzip compressed data, was "CSET-0.2.0.tar", last modified: Fri Jun 16 09:15:52 2023, max compression
```

## Comparing `CSET-0.1.0.tar` & `CSET-0.2.0.tar`

### file list

```diff
@@ -1,37 +1,37 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 15:43:23.135318 CSET-0.1.0/
--rw-r--r--   0 runner    (1001) docker     (123)    10996 2023-04-24 15:42:59.000000 CSET-0.1.0/LICENCE
--rw-r--r--   0 runner    (1001) docker     (123)     2016 2023-04-24 15:43:23.135318 CSET-0.1.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1512 2023-04-24 15:42:59.000000 CSET-0.1.0/README.md
--rw-r--r--   0 runner    (1001) docker     (123)     3464 2023-04-24 15:42:59.000000 CSET-0.1.0/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)      282 2023-04-24 15:43:23.135318 CSET-0.1.0/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 15:43:23.131318 CSET-0.1.0/src/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 15:43:23.135318 CSET-0.1.0/src/CSET/
--rw-r--r--   0 runner    (1001) docker     (123)     2085 2023-04-24 15:42:59.000000 CSET-0.1.0/src/CSET/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      706 2023-04-24 15:42:59.000000 CSET-0.1.0/src/CSET/__main__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 15:43:23.135318 CSET-0.1.0/src/CSET/operators/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 15:43:23.135318 CSET-0.1.0/src/CSET/operators/RECIPES/
--rw-r--r--   0 runner    (1001) docker     (123)      970 2023-04-24 15:42:59.000000 CSET-0.1.0/src/CSET/operators/RECIPES/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      873 2023-04-24 15:42:59.000000 CSET-0.1.0/src/CSET/operators/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3600 2023-04-24 15:42:59.000000 CSET-0.1.0/src/CSET/operators/_internal.py
--rw-r--r--   0 runner    (1001) docker     (123)     4397 2023-04-24 15:42:59.000000 CSET-0.1.0/src/CSET/operators/constraints.py
--rw-r--r--   0 runner    (1001) docker     (123)     1511 2023-04-24 15:42:59.000000 CSET-0.1.0/src/CSET/operators/filters.py
--rw-r--r--   0 runner    (1001) docker     (123)      914 2023-04-24 15:42:59.000000 CSET-0.1.0/src/CSET/operators/misc.py
--rw-r--r--   0 runner    (1001) docker     (123)     1389 2023-04-24 15:42:59.000000 CSET-0.1.0/src/CSET/operators/plot.py
--rw-r--r--   0 runner    (1001) docker     (123)     1386 2023-04-24 15:42:59.000000 CSET-0.1.0/src/CSET/operators/read.py
--rw-r--r--   0 runner    (1001) docker     (123)     1478 2023-04-24 15:42:59.000000 CSET-0.1.0/src/CSET/operators/write.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 15:43:23.135318 CSET-0.1.0/src/CSET.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     2016 2023-04-24 15:43:23.000000 CSET-0.1.0/src/CSET.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      725 2023-04-24 15:43:23.000000 CSET-0.1.0/src/CSET.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-24 15:43:23.000000 CSET-0.1.0/src/CSET.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       35 2023-04-24 15:43:23.000000 CSET-0.1.0/src/CSET.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)      115 2023-04-24 15:43:23.000000 CSET-0.1.0/src/CSET.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        5 2023-04-24 15:43:23.000000 CSET-0.1.0/src/CSET.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 15:43:23.135318 CSET-0.1.0/tests/
--rw-r--r--   0 runner    (1001) docker     (123)     1047 2023-04-24 15:42:59.000000 CSET-0.1.0/tests/test_cli.py
--rw-r--r--   0 runner    (1001) docker     (123)     3566 2023-04-24 15:42:59.000000 CSET-0.1.0/tests/test_constraints.py
--rw-r--r--   0 runner    (1001) docker     (123)     1480 2023-04-24 15:42:59.000000 CSET-0.1.0/tests/test_filters.py
--rw-r--r--   0 runner    (1001) docker     (123)      744 2023-04-24 15:42:59.000000 CSET-0.1.0/tests/test_misc.py
--rw-r--r--   0 runner    (1001) docker     (123)     1162 2023-04-24 15:42:59.000000 CSET-0.1.0/tests/test_plots.py
--rw-r--r--   0 runner    (1001) docker     (123)     1062 2023-04-24 15:42:59.000000 CSET-0.1.0/tests/test_read.py
--rw-r--r--   0 runner    (1001) docker     (123)     2661 2023-04-24 15:42:59.000000 CSET-0.1.0/tests/test_recipe_parser.py
--rw-r--r--   0 runner    (1001) docker     (123)     1291 2023-04-24 15:42:59.000000 CSET-0.1.0/tests/test_write.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 09:15:52.389007 CSET-0.2.0/
+-rw-r--r--   0 runner    (1001) docker     (123)    10996 2023-06-16 09:15:28.000000 CSET-0.2.0/LICENCE
+-rw-r--r--   0 runner    (1001) docker     (123)     2016 2023-06-16 09:15:52.389007 CSET-0.2.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1512 2023-06-16 09:15:28.000000 CSET-0.2.0/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)     3446 2023-06-16 09:15:28.000000 CSET-0.2.0/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)      282 2023-06-16 09:15:52.393007 CSET-0.2.0/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 09:15:52.385007 CSET-0.2.0/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 09:15:52.389007 CSET-0.2.0/src/CSET/
+-rw-r--r--   0 runner    (1001) docker     (123)     2321 2023-06-16 09:15:28.000000 CSET-0.2.0/src/CSET/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      706 2023-06-16 09:15:28.000000 CSET-0.2.0/src/CSET/__main__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 09:15:52.389007 CSET-0.2.0/src/CSET/operators/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 09:15:52.389007 CSET-0.2.0/src/CSET/operators/RECIPES/
+-rw-r--r--   0 runner    (1001) docker     (123)      970 2023-06-16 09:15:28.000000 CSET-0.2.0/src/CSET/operators/RECIPES/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      873 2023-06-16 09:15:28.000000 CSET-0.2.0/src/CSET/operators/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4544 2023-06-16 09:15:28.000000 CSET-0.2.0/src/CSET/operators/_internal.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4398 2023-06-16 09:15:28.000000 CSET-0.2.0/src/CSET/operators/constraints.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1501 2023-06-16 09:15:28.000000 CSET-0.2.0/src/CSET/operators/filters.py
+-rw-r--r--   0 runner    (1001) docker     (123)      995 2023-06-16 09:15:28.000000 CSET-0.2.0/src/CSET/operators/misc.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1379 2023-06-16 09:15:28.000000 CSET-0.2.0/src/CSET/operators/plot.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1376 2023-06-16 09:15:28.000000 CSET-0.2.0/src/CSET/operators/read.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1468 2023-06-16 09:15:28.000000 CSET-0.2.0/src/CSET/operators/write.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 09:15:52.389007 CSET-0.2.0/src/CSET.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     2016 2023-06-16 09:15:52.000000 CSET-0.2.0/src/CSET.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      725 2023-06-16 09:15:52.000000 CSET-0.2.0/src/CSET.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-16 09:15:52.000000 CSET-0.2.0/src/CSET.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       35 2023-06-16 09:15:52.000000 CSET-0.2.0/src/CSET.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       92 2023-06-16 09:15:52.000000 CSET-0.2.0/src/CSET.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        5 2023-06-16 09:15:52.000000 CSET-0.2.0/src/CSET.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 09:15:52.389007 CSET-0.2.0/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)     1336 2023-06-16 09:15:28.000000 CSET-0.2.0/tests/test_cli.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3650 2023-06-16 09:15:28.000000 CSET-0.2.0/tests/test_constraints.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1537 2023-06-16 09:15:28.000000 CSET-0.2.0/tests/test_filters.py
+-rw-r--r--   0 runner    (1001) docker     (123)      801 2023-06-16 09:15:28.000000 CSET-0.2.0/tests/test_misc.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1219 2023-06-16 09:15:28.000000 CSET-0.2.0/tests/test_plots.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1119 2023-06-16 09:15:28.000000 CSET-0.2.0/tests/test_read.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3980 2023-06-16 09:15:28.000000 CSET-0.2.0/tests/test_recipe_parser.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1461 2023-06-16 09:15:28.000000 CSET-0.2.0/tests/test_write.py
```

### Comparing `CSET-0.1.0/LICENCE` & `CSET-0.2.0/LICENCE`

 * *Files identical despite different names*

### Comparing `CSET-0.1.0/PKG-INFO` & `CSET-0.2.0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: CSET
-Version: 0.1.0
+Version: 0.2.0
 Summary: Convective Scale Evaluation Tool for evaluation and investigation of regional models.
 Author: Met Office, NIWA
 License: Apache-2.0
 Project-URL: Documentation, https://metoffice.github.io/CSET
 Project-URL: Source, https://github.com/MetOffice/CSET
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Topic :: Scientific/Engineering :: GIS
```

### Comparing `CSET-0.1.0/README.md` & `CSET-0.2.0/README.md`

 * *Files identical despite different names*

### Comparing `CSET-0.1.0/pyproject.toml` & `CSET-0.2.0/pyproject.toml`

 * *Files 8% similar despite different names*

```diff
@@ -1,23 +1,23 @@
 [project]
 name = "CSET"
-version = "0.1.0"
+version = "0.2.0"
 description = "Convective Scale Evaluation Tool for evaluation and investigation of regional models."
 authors = [{ name = "Met Office" }, { name = "NIWA" }]
 readme = "README.md"
 license = { text = "Apache-2.0" }
 requires-python = ">=3.8"
 classifiers = [
     "License :: OSI Approved :: Apache Software License",
     "Topic :: Scientific/Engineering :: GIS",
 ]
 dependencies = [
     "numpy",
     "scitools-iris",
-    "tomli >= 1.1.0 ; python_version < '3.11'",
+    "ruamel.yaml >= 0.17",
     "importlib_resources >= 3.0.0 ; python_version < '3.9'",
 ]
 
 [project.urls]
 Documentation = "https://metoffice.github.io/CSET"
 Source = "https://github.com/MetOffice/CSET"
 
@@ -25,15 +25,15 @@
 cset = "CSET:main"
 
 [build-system]
 requires = ["setuptools>=61.0"]
 build-backend = "setuptools.build_meta"
 
 [tool.pytest.ini_options]
-addopts = ["--import-mode=importlib", "--verbose", "--cov"]
+addopts = ["--import-mode=importlib", "--verbose", "--cov", "--cov-append"]
 pythonpath = ["src"]
 filterwarnings = ['ignore::DeprecationWarning:pytest']
 
 [tool.coverage.run]
 branch = true
 relative_files = true
 source = ["src"]
@@ -76,15 +76,15 @@
 conda_spec =
     py38-linux: {toxinidir}{/}requirements{/}locks{/}py38-lock-linux-64.txt
     py39-linux: {toxinidir}{/}requirements{/}locks{/}py39-lock-linux-64.txt
     py310-linux: {toxinidir}{/}requirements{/}locks{/}py310-lock-linux-64.txt
     py311-linux: {toxinidir}{/}requirements{/}locks{/}py311-lock-linux-64.txt
 usedevelop = true
 depends = coverage-clean
-commands = pytest --cov-append {posargs}
+commands = pytest {posargs}
 
 [testenv:py{38,39,310,311}-{linux,osx,win}-docs]
 description = Invoke sphinx-build to build the HTML docs.
 conda_spec =
     py38-linux: {toxinidir}{/}requirements{/}locks{/}py38-lock-linux-64.txt
     py39-linux: {toxinidir}{/}requirements{/}locks{/}py39-lock-linux-64.txt
     py310-linux: {toxinidir}{/}requirements{/}locks{/}py310-lock-linux-64.txt
```

### Comparing `CSET-0.1.0/src/CSET/__main__.py` & `CSET-0.2.0/src/CSET/__main__.py`

 * *Files identical despite different names*

### Comparing `CSET-0.1.0/src/CSET/operators/RECIPES/__init__.py` & `CSET-0.2.0/src/CSET/operators/RECIPES/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -18,8 +18,8 @@
 try:
     from importlib.resources import files
 except ImportError:
     # importlib has the files API from python 3.9
     from importlib_resources import files
 import CSET.operators.RECIPES as recipes
 
-extract_instant_air_temp = files(recipes).joinpath("extract_instant_air_temp.toml")
+extract_instant_air_temp = files(recipes).joinpath("extract_instant_air_temp.yaml")
```

### Comparing `CSET-0.1.0/src/CSET/operators/__init__.py` & `CSET-0.2.0/src/CSET/operators/__init__.py`

 * *Files identical despite different names*

### Comparing `CSET-0.1.0/src/CSET/operators/_internal.py` & `CSET-0.2.0/src/CSET/operators/_internal.py`

 * *Files 26% similar despite different names*

```diff
@@ -12,21 +12,17 @@
 # See the License for the specific language governing permissions and
 # limitations under the License.
 
 """Internal functions used to run operators."""
 
 import logging
 from pathlib import Path
-
-try:
-    import tomllib
-except ModuleNotFoundError:
-    # tomllib is in standard library from 3.11.
-    import tomli as tomllib
-
+from typing import Union
+import inspect
+import ruamel.yaml
 import CSET.operators
 
 
 def get_operator(name: str):
     """
     Gets an operator by its name.
 
@@ -60,62 +56,88 @@
             return operator
         else:
             raise AttributeError
     except (AttributeError, TypeError):
         raise ValueError(f"Unknown operator: {name}")
 
 
-def execute_recipe(recipe_file: Path, input_file: Path, output_file: Path) -> None:
+def execute_recipe(
+    recipe_yaml: Union[Path, str], input_file: Path, output_file: Path
+) -> None:
     """Parses and executes a recipe file.
 
     Parameters
     ----------
-    recipe_file: Path
-        Pathlike to a configuration file indicating the operators that need
-        running.
+    recipe_yaml: Path or str
+        Path to a file containing, or string of, a recipe's YAML describing the
+        operators that need running. If a Path is provided it is opened and
+        read.
 
     input_file: Path
         Pathlike to netCDF (or something else that iris read) file to be used as
         input.
 
     output_file: Path
         Pathlike indicating desired location of output.
 
     Raises
     ------
     FileNotFoundError
         The recipe or input file cannot be found.
 
     ValueError
-        The recipe file is not well formed.
+        The recipe is not well formed.
+
+    TypeError
+        The provided recipe is not a stream or Path.
     """
 
-    def step_parser(step, step_io, output_file_path: Path) -> str:
-        if "input" in step:
-            if type(step["input"]) == dict:
-                logging.debug(f"Recursing into input: {step['input']}")
-                step_io = step_parser(step["input"], step_io, output_file_path)
-            else:
-                step_io = step["input"]
+    def step_parser(step: dict, step_input: any, output_file_path: Path) -> str:
+        logging.debug(f"Executing step: {step}")
         kwargs = {}
-        if "args" in step:
-            for key in step["args"].keys():
-                if type(step["args"][key]) == dict:
-                    logging.debug(f"Recursing into args: {step['args']}")
-                    kwargs[key] = step_parser(
-                        step["args"][key], step_io, output_file_path
-                    )
-                elif step["args"][key] == "MAGIC_OUTPUT_PATH":
-                    kwargs[key] = output_file_path
-                else:
-                    kwargs[key] = step["args"][key]
-        operator = get_operator(step["operator"])
-        logging.info(f"operator = {step['operator']}")
-        logging.debug(f"step_input = {step_io}")
-        logging.debug(f"args = {kwargs}")
-        return operator(step_io, **kwargs)
-
-    with open(recipe_file, "rb") as f:
-        recipe = tomllib.load(f)
-    step_io = input_file
-    for step in recipe["steps"]:
-        step_io = step_parser(step, step_io, output_file)
+        for key in step.keys():
+            if key == "operator":
+                operator = get_operator(step["operator"])
+                logging.info(f"operator: {step['operator']}")
+            elif type(step[key]) == dict and "operator" in step[key]:
+                logging.debug(f"Recursing into argument: {key}")
+                kwargs[key] = step_parser(step[key], step_input, output_file_path)
+            elif step[key] == "CSET_OUTPUT_PATH":
+                kwargs[key] = output_file_path
+            else:
+                kwargs[key] = step[key]
+
+        logging.debug(f"args: {kwargs}")
+        logging.debug(f"step_input: {step_input}")
+
+        # If first argument of operator is explicitly defined, use that rather
+        # than step_input. This is known through introspection of the operator.
+        first_arg = next(iter(inspect.signature(operator).parameters.keys()))
+        logging.debug(f"first_arg: {first_arg}")
+        if first_arg not in kwargs:
+            return operator(step_input, **kwargs)
+        else:
+            return operator(**kwargs)
+
+    with ruamel.yaml.YAML(typ="safe", pure=True) as yaml:
+        try:
+            recipe = yaml.load(recipe_yaml)
+        except ruamel.yaml.parser.ParserError:
+            raise ValueError("ParserError: Invalid YAML")
+        except ruamel.yaml.error.YAMLStreamError:
+            raise TypeError("Must provide a stream (with a read method)")
+
+    logging.debug(recipe)
+    step_input = input_file
+    try:
+        if len(recipe["steps"]) < 1:
+            raise ValueError("Recipe must have at least 1 step.")
+        for step in recipe["steps"]:
+            step_input = step_parser(step, step_input, output_file)
+    except KeyError as err:
+        raise ValueError("Invalid Recipe:", err)
+    except TypeError as err:
+        if recipe is None:
+            raise ValueError("Recipe must have at least 1 step.")
+        # This should never be reached.
+        raise err  # pragma: no cover
+    logging.info(f"Recipe output: {step_input}")
```

### Comparing `CSET-0.1.0/src/CSET/operators/constraints.py` & `CSET-0.2.0/src/CSET/operators/constraints.py`

 * *Files 8% similar despite different names*

```diff
@@ -17,15 +17,15 @@
 """
 
 import iris
 import iris.cube
 from datetime import datetime
 
 
-def generate_stash_constraint(stash: str, **kwargs) -> iris.AttributeConstraint:
+def generate_stash_constraint(stash: str) -> iris.AttributeConstraint:
     """
     Operator that takes a stash string, and uses iris to generate a constraint
     to be passed into the read operator to minimize the CubeList the read
     operator loads and speed up loading.
 
     Arguments
     ---------
@@ -39,15 +39,15 @@
 
     # At a later stage str list an option to combine constraints. Arguments
     # could be a list of stash codes that combined build the constraint.
     stash_constraint = iris.AttributeConstraint(STASH=stash)
     return stash_constraint
 
 
-def generate_var_constraint(varname: str, **kwargs) -> iris.Constraint:
+def generate_var_constraint(varname: str) -> iris.Constraint:
     """
     Operator that takes a CF compliant variable name string, and uses iris to
     generate a constraint to be passed into the read operator to minimize the
     CubeList the read operator loads and speed up loading.
 
     Arguments
     ---------
@@ -59,15 +59,15 @@
     varname_constraint: iris.Constraint
     """
 
     varname_constraint = iris.Constraint(name=varname)
     return varname_constraint
 
 
-def generate_cell_methods_constraint(cell_methods: list, **kwargs) -> iris.Constraint:
+def generate_cell_methods_constraint(cell_methods: list) -> iris.Constraint:
     """
     Operator that takes a list of cell methods and generates a constraint from
     that.
 
     Arguments
     ---------
     cell_methods: list
@@ -85,15 +85,15 @@
             return False
 
     cell_methods_constraint = iris.Constraint(cube_func=check_cell_methods)
     return cell_methods_constraint
 
 
 def generate_time_constraint(
-    time_start: str, time_end: str = None, **kwargs
+    time_start: str, time_end: str = None
 ) -> iris.AttributeConstraint:
     """
     Operator that takes one or two ISO 8601 date strings, and returns a
     constraint that selects values between those dates (inclusive).
 
     Arguments
     ---------
@@ -114,35 +114,38 @@
         time_end = time_start
     elif type(time_end) == str:
         time_end = datetime.fromisoformat(time_end)
     time_constraint = iris.Constraint(time=lambda t: time_start <= t.point <= time_end)
     return time_constraint
 
 
-def combine_constraints(input_constraint: iris.Constraint, **kwargs) -> iris.Constraint:
+def combine_constraints(
+    constraint: iris.Constraint = iris.Constraint(), **kwargs
+) -> iris.Constraint:
     """
     Operator that combines multiple constraints into one.
 
     Arguments
     ---------
-    input_constraint: iris.Constraint
-        First constraint to combine.
+    constraint: iris.Constraint
+        First constraint to combine. This must be named "constraint".
     additional_constraint_1: iris.Constraint
         Second constraint to combine. This must be a named argument.
     additional_constraint_2: iris.Constraint
         There can be any number of additional constraint, they just need unique
         names.
+    ...
 
     Returns
     -------
     combined_constraint: iris.Constraint
 
     Raises
     ------
     TypeError
         If the provided arguments are not constraints.
     """
 
-    combined_constraint = input_constraint
-    for constraint in kwargs.values():
-        combined_constraint = combined_constraint & constraint
+    combined_constraint = constraint
+    for constr in kwargs.values():
+        combined_constraint = combined_constraint & constr
     return combined_constraint
```

### Comparing `CSET-0.1.0/src/CSET/operators/filters.py` & `CSET-0.2.0/src/CSET/operators/filters.py`

 * *Files 1% similar despite different names*

```diff
@@ -17,15 +17,15 @@
 """
 
 import iris
 import iris.cube
 
 
 def filter_cubes(
-    cubelist: iris.cube.CubeList, constraint: iris.Constraint, **kwargs
+    cubelist: iris.cube.CubeList, constraint: iris.Constraint
 ) -> iris.cube.Cube:
     """
     Filters a cubelist down to a single cube based on a constraint.
 
     Arguments
     ---------
     cubelist: iris.cube.CubeList
```

### Comparing `CSET-0.1.0/src/CSET/operators/misc.py` & `CSET-0.2.0/src/CSET/operators/misc.py`

 * *Files 12% similar despite different names*

```diff
@@ -23,13 +23,15 @@
     diagnostic chains.
 
     Arguments
     ---------
     x: Any
         Input to return.
 
+    Will silently accept any additional keyword arguments for testing purposes.
+
     Returns
     -------
     x: Any
         The input that was given.
     """
     return x
```

### Comparing `CSET-0.1.0/src/CSET/operators/plot.py` & `CSET-0.2.0/src/CSET/operators/plot.py`

 * *Files 1% similar despite different names*

```diff
@@ -19,15 +19,15 @@
 from pathlib import Path
 import iris
 import iris.cube
 import iris.quickplot as qplt
 import matplotlib.pyplot as plt
 
 
-def spatial_contour_plot(cube: iris.cube.Cube, file_path: Path, **kwargs) -> Path:
+def spatial_contour_plot(cube: iris.cube.Cube, file_path: Path) -> Path:
     """
     Plots a spatial variable onto a map.
 
     Parameters
     ----------
     cube: Cube
         An iris cube of the data to plot. It should be 2 dimensional (lat and lon).
```

### Comparing `CSET-0.1.0/src/CSET/operators/read.py` & `CSET-0.2.0/src/CSET/operators/read.py`

 * *Files 14% similar despite different names*

```diff
@@ -19,15 +19,15 @@
 from pathlib import Path
 
 import iris
 import iris.cube
 
 
 def read_cubes(
-    loadpath: Path, constraint: iris.Constraint = None, **kwargs
+    loadpath: Path, constraint: iris.Constraint = None
 ) -> iris.cube.CubeList:
     """
     Read operator that takes a path string (can include wildcards), and uses
     iris to load all the cubes matching stash and return a CubeList object.
 
     Arguments
     ---------
```

### Comparing `CSET-0.1.0/src/CSET/operators/write.py` & `CSET-0.2.0/src/CSET/operators/write.py`

 * *Files 3% similar despite different names*

```diff
@@ -20,15 +20,15 @@
 from typing import Union
 
 import iris
 import iris.cube
 
 
 def write_cube_to_nc(
-    cube: Union[iris.cube.Cube, iris.cube.CubeList], file_path: Path, **kwargs
+    cube: Union[iris.cube.Cube, iris.cube.CubeList], file_path: Path
 ) -> str:
     """
     A write operator that sits after the read operator. This operator expects
     an iris cube object that will then be passed to MET for further processing.
 
     Arguments
     ---------
```

### Comparing `CSET-0.1.0/src/CSET.egg-info/PKG-INFO` & `CSET-0.2.0/src/CSET.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: CSET
-Version: 0.1.0
+Version: 0.2.0
 Summary: Convective Scale Evaluation Tool for evaluation and investigation of regional models.
 Author: Met Office, NIWA
 License: Apache-2.0
 Project-URL: Documentation, https://metoffice.github.io/CSET
 Project-URL: Source, https://github.com/MetOffice/CSET
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Topic :: Scientific/Engineering :: GIS
```

### Comparing `CSET-0.1.0/src/CSET.egg-info/SOURCES.txt` & `CSET-0.2.0/src/CSET.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `CSET-0.1.0/tests/test_cli.py` & `CSET-0.2.0/tests/test_cli.py`

 * *Files 12% similar despite different names*

```diff
@@ -9,26 +9,44 @@
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 
 import subprocess
+import os
 
 
 def test_command_line_help():
     subprocess.run(["cset", "--help"])
     # test verbose options. This is really just to up the coverage number.
     subprocess.run(["cset", "-v"])
     subprocess.run(["cset", "-vv"])
 
 
 def test_recipe_execution():
     subprocess.run(
         [
             "cset",
             "operators",
-            "/dev/null",
-            "/dev/null",
-            "test/test_data/noop_recipe.toml",
+            os.devnull,
+            os.devnull,
+            "test/test_data/noop_recipe.yaml",
+        ]
+    )
+
+
+def test_environ_var_recipe():
+    os.environ[
+        "CSET_RECIPE"
+    ] = """
+        steps:
+          - operator: misc.noop
+        """
+    subprocess.run(
+        [
+            "cset",
+            "operators",
+            os.devnull,
+            os.devnull,
         ]
     )
```

### Comparing `CSET-0.1.0/tests/test_constraints.py` & `CSET-0.2.0/tests/test_constraints.py`

 * *Files 3% similar despite different names*

```diff
@@ -10,14 +10,17 @@
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 
 from CSET.operators import constraints
 from datetime import datetime
+import logging
+
+logging.basicConfig(level=logging.DEBUG)
 
 
 def test_generate_stash_constraint():
     """generate iris cube constraint for UM STASH code."""
     stash_constraint = constraints.generate_stash_constraint("m01s03i236")
     expected_stash_constraint = "AttributeConstraint({'STASH': 'm01s03i236'})"
     assert repr(stash_constraint) == expected_stash_constraint
@@ -43,20 +46,20 @@
     time_constraint = constraints.generate_time_constraint(
         "2023-03-24T00:00", "2023-03-24T06:00"
     )
     expected_time_constraint = "Constraint(coord_values={'time': <function generate_time_constraint.<locals>.<lambda> at "
     assert expected_time_constraint in repr(time_constraint)
     # Try with datatime.datatime dates
     time_constraint = constraints.generate_time_constraint(
-        datetime.fromisoformat("2023-03-24T00:00"),
-        datetime.fromisoformat("2023-03-24T06:00"),
+        datetime.fromisoformat("2023-03-24T00:00:00+00:00"),
+        datetime.fromisoformat("2023-03-24T06:00:00+00:00"),
     )
     assert expected_time_constraint in repr(time_constraint)
     # Try with implicit end
-    time_constraint = constraints.generate_time_constraint("2023-03-24T00:00")
+    time_constraint = constraints.generate_time_constraint("2023-03-24T00:00:00+00:00")
     assert expected_time_constraint in repr(time_constraint)
 
 
 def test_combine_constraints():
     """combine constraint"""
     stash_constraint = constraints.generate_stash_constraint("m01s03i236")
     var_constraint = constraints.generate_var_constraint("test")
```

### Comparing `CSET-0.1.0/tests/test_filters.py` & `CSET-0.2.0/tests/test_filters.py`

 * *Files 8% similar despite different names*

```diff
@@ -9,14 +9,17 @@
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 
 from CSET.operators import read, filters, constraints
+import logging
+
+logging.basicConfig(level=logging.DEBUG)
 
 
 def test_filters_operator():
     """Filter cube and verify."""
     cubes = read.read_cubes("tests/test_data/air_temp.nc")
     constraint = constraints.combine_constraints(
         constraints.generate_stash_constraint("m01s03i236"),
```

### Comparing `CSET-0.1.0/tests/test_misc.py` & `CSET-0.2.0/tests/test_misc.py`

 * *Files 26% similar despite different names*

```diff
@@ -9,14 +9,17 @@
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 
 from CSET.operators import misc
+import logging
+
+logging.basicConfig(level=logging.DEBUG)
 
 
 def test_noop_operator():
     """Passes through input unchanged."""
     a = 7
     b = misc.noop(a)
     assert a == b
```

### Comparing `CSET-0.1.0/tests/test_plots.py` & `CSET-0.2.0/tests/test_plots.py`

 * *Files 13% similar despite different names*

```diff
@@ -12,18 +12,21 @@
 # See the License for the specific language governing permissions and
 # limitations under the License.
 
 from pathlib import Path
 from uuid import uuid4
 import tempfile
 import CSET.operators._internal as internal
+import logging
 
+logging.basicConfig(level=logging.DEBUG)
 
-def test_spacial_plot():
-    """Plot spacial contour plot of instant air temp."""
+
+def test_spatial_plot():
+    """Plot spatial contour plot of instant air temp."""
     input_file = Path("tests/test_data/air_temp.nc")
-    recipe_file = Path("tests/test_data/plot_instant_air_temp.toml")
     output_file = Path(f"{tempfile.gettempdir()}/{uuid4()}")
+    recipe_file = Path("tests/test_data/plot_instant_air_temp.yaml")
     internal.execute_recipe(recipe_file, input_file, output_file)
     actual_output_file = output_file.with_suffix(".svg")
     assert actual_output_file.exists()
     actual_output_file.unlink()
```

### Comparing `CSET-0.1.0/tests/test_read.py` & `CSET-0.2.0/tests/test_read.py`

 * *Files 16% similar despite different names*

```diff
@@ -9,14 +9,17 @@
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 
 from CSET.operators import read
+import logging
+
+logging.basicConfig(level=logging.DEBUG)
 
 
 def test_read_cubes():
     """Read cube and verify."""
     cubes = read.read_cubes("tests/test_data/air_temp.nc")
     assert len(cubes) == 3
     expected_cubes = [
```

### Comparing `CSET-0.1.0/tests/test_write.py` & `CSET-0.2.0/tests/test_write.py`

 * *Files 21% similar despite different names*

```diff
@@ -8,27 +8,37 @@
 #
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 
-from CSET.operators import write, read
-from secrets import token_hex
 from pathlib import Path
+import logging
+import tempfile
+from uuid import uuid4
+import os
+
+from CSET.operators import write, read
+
+logging.basicConfig(level=logging.DEBUG)
 
 
 def test_write_cube_to_nc():
     """Write cube to Path and string path and verify."""
     cube = read.read_cubes("tests/test_data/air_temp.nc")[0]
+
     # Write to string
-    filename = f"/tmp/{token_hex(4)}_write_test_cube.nc"
+    filename = f"{tempfile.gettempdir()}/{uuid4()}.nc"
     write.write_cube_to_nc(cube, filename)
+    # Check that the cube was written correctly
+    written_cube = read.read_cubes(filename)[0]
+    assert written_cube == cube
+    os.unlink(filename)
+
     # Write to Path
-    filepath = Path(f"/tmp/{token_hex(4)}_write_test_cube.nc")
+    filepath = Path(f"{tempfile.gettempdir()}/{uuid4()}.nc")
     write.write_cube_to_nc(cube, filepath)
     # Check that the cube was written correctly
     written_cube = read.read_cubes(filepath)[0]
     assert written_cube == cube
-    # Clean up written files
     filepath.unlink()
-    Path(filename).unlink()
```

