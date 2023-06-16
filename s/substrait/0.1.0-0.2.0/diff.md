# Comparing `tmp/substrait-0.1.0.tar.gz` & `tmp/substrait-0.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "substrait-0.1.0.tar", last modified: Tue May 30 19:42:04 2023, max compression
+gzip compressed data, was "substrait-0.2.0.tar", last modified: Fri Jun 16 20:34:07 2023, max compression
```

## Comparing `substrait-0.1.0.tar` & `substrait-0.2.0.tar`

### file list

```diff
@@ -1,46 +1,62 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 19:42:04.369334 substrait-0.1.0/
--rw-r--r--   0 runner    (1001) docker     (123)       45 2023-05-30 19:41:51.000000 substrait-0.1.0/.gitattributes
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 19:42:04.353334 substrait-0.1.0/.github/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 19:42:04.361334 substrait-0.1.0/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (123)     2139 2023-05-30 19:41:51.000000 substrait-0.1.0/.github/workflows/release.yml
--rw-r--r--   0 runner    (1001) docker     (123)      782 2023-05-30 19:41:51.000000 substrait-0.1.0/.github/workflows/test.yml
--rw-r--r--   0 runner    (1001) docker     (123)     2020 2023-05-30 19:41:51.000000 substrait-0.1.0/.gitignore
--rw-r--r--   0 runner    (1001) docker     (123)      115 2023-05-30 19:41:51.000000 substrait-0.1.0/.gitmodules
--rw-r--r--   0 runner    (1001) docker     (123)     1004 2023-05-30 19:41:51.000000 substrait-0.1.0/CONTRIBUTING.md
--rw-r--r--   0 runner    (1001) docker     (123)    11357 2023-05-30 19:41:51.000000 substrait-0.1.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     4468 2023-05-30 19:42:04.369334 substrait-0.1.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     4153 2023-05-30 19:41:51.000000 substrait-0.1.0/README.md
--rw-r--r--   0 runner    (1001) docker     (123)       65 2023-05-30 19:41:51.000000 substrait-0.1.0/buf.gen.yaml
--rw-r--r--   0 runner    (1001) docker     (123)       42 2023-05-30 19:41:51.000000 substrait-0.1.0/buf.work.yaml
--rw-r--r--   0 runner    (1001) docker     (123)       67 2023-05-30 19:41:51.000000 substrait-0.1.0/buf.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      286 2023-05-30 19:41:51.000000 substrait-0.1.0/environment.yml
--rwxr-xr-x   0 runner    (1001) docker     (123)      637 2023-05-30 19:41:51.000000 substrait-0.1.0/gen_proto.sh
--rw-r--r--   0 runner    (1001) docker     (123)      684 2023-05-30 19:41:51.000000 substrait-0.1.0/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-30 19:42:04.369334 substrait-0.1.0/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 19:42:04.357334 substrait-0.1.0/src/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 19:42:04.361334 substrait-0.1.0/src/substrait/
--rw-r--r--   0 runner    (1001) docker     (123)       72 2023-05-30 19:41:51.000000 substrait-0.1.0/src/substrait/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      160 2023-05-30 19:42:04.000000 substrait-0.1.0/src/substrait/_version.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 19:42:04.365334 substrait-0.1.0/src/substrait/gen/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-30 19:41:51.000000 substrait-0.1.0/src/substrait/gen/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 19:42:04.369334 substrait-0.1.0/src/substrait/gen/proto/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-30 19:41:51.000000 substrait-0.1.0/src/substrait/gen/proto/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    47948 2023-05-30 19:41:51.000000 substrait-0.1.0/src/substrait/gen/proto/algebra_pb2.py
--rw-r--r--   0 runner    (1001) docker     (123)     1527 2023-05-30 19:41:51.000000 substrait-0.1.0/src/substrait/gen/proto/capabilities_pb2.py
--rw-r--r--   0 runner    (1001) docker     (123)     2268 2023-05-30 19:41:51.000000 substrait-0.1.0/src/substrait/gen/proto/extended_expression_pb2.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 19:42:04.369334 substrait-0.1.0/src/substrait/gen/proto/extensions/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-30 19:41:51.000000 substrait-0.1.0/src/substrait/gen/proto/extensions/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3127 2023-05-30 19:41:51.000000 substrait-0.1.0/src/substrait/gen/proto/extensions/extensions_pb2.py
--rw-r--r--   0 runner    (1001) docker     (123)     7587 2023-05-30 19:41:51.000000 substrait-0.1.0/src/substrait/gen/proto/function_pb2.py
--rw-r--r--   0 runner    (1001) docker     (123)     8257 2023-05-30 19:41:51.000000 substrait-0.1.0/src/substrait/gen/proto/parameterized_types_pb2.py
--rw-r--r--   0 runner    (1001) docker     (123)     2341 2023-05-30 19:41:51.000000 substrait-0.1.0/src/substrait/gen/proto/plan_pb2.py
--rw-r--r--   0 runner    (1001) docker     (123)    10190 2023-05-30 19:41:51.000000 substrait-0.1.0/src/substrait/gen/proto/type_expressions_pb2.py
--rw-r--r--   0 runner    (1001) docker     (123)    10975 2023-05-30 19:41:51.000000 substrait-0.1.0/src/substrait/gen/proto/type_pb2.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 19:42:04.365334 substrait-0.1.0/src/substrait.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     4468 2023-05-30 19:42:04.000000 substrait-0.1.0/src/substrait.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      975 2023-05-30 19:42:04.000000 substrait-0.1.0/src/substrait.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-30 19:42:04.000000 substrait-0.1.0/src/substrait.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       88 2023-05-30 19:42:04.000000 substrait-0.1.0/src/substrait.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       10 2023-05-30 19:42:04.000000 substrait-0.1.0/src/substrait.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 19:42:04.369334 substrait-0.1.0/tests/
--rw-r--r--   0 runner    (1001) docker     (123)      660 2023-05-30 19:41:51.000000 substrait-0.1.0/tests/test_proto.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 20:34:07.669746 substrait-0.2.0/
+-rw-r--r--   0 runner    (1001) docker     (123)       97 2023-06-16 20:33:54.000000 substrait-0.2.0/.gitattributes
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 20:34:07.665746 substrait-0.2.0/.github/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 20:34:07.665746 substrait-0.2.0/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (123)     2160 2023-06-16 20:33:54.000000 substrait-0.2.0/.github/workflows/pr_title.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     1644 2023-06-16 20:33:54.000000 substrait-0.2.0/.github/workflows/release.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      782 2023-06-16 20:33:54.000000 substrait-0.2.0/.github/workflows/test.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     2020 2023-06-16 20:33:54.000000 substrait-0.2.0/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (123)      115 2023-06-16 20:33:54.000000 substrait-0.2.0/.gitmodules
+-rw-r--r--   0 runner    (1001) docker     (123)     1004 2023-06-16 20:33:54.000000 substrait-0.2.0/CONTRIBUTING.md
+-rw-r--r--   0 runner    (1001) docker     (123)    11357 2023-06-16 20:33:54.000000 substrait-0.2.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     4468 2023-06-16 20:34:07.669746 substrait-0.2.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     4153 2023-06-16 20:33:54.000000 substrait-0.2.0/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)       65 2023-06-16 20:33:54.000000 substrait-0.2.0/buf.gen.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)       42 2023-06-16 20:33:54.000000 substrait-0.2.0/buf.work.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)       67 2023-06-16 20:33:54.000000 substrait-0.2.0/buf.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      286 2023-06-16 20:33:54.000000 substrait-0.2.0/environment.yml
+-rwxr-xr-x   0 runner    (1001) docker     (123)      868 2023-06-16 20:33:54.000000 substrait-0.2.0/gen_proto.sh
+-rw-r--r--   0 runner    (1001) docker     (123)      650 2023-06-16 20:33:54.000000 substrait-0.2.0/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-16 20:34:07.669746 substrait-0.2.0/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 20:34:07.665746 substrait-0.2.0/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 20:34:07.665746 substrait-0.2.0/src/substrait/
+-rw-r--r--   0 runner    (1001) docker     (123)      179 2023-06-16 20:33:54.000000 substrait-0.2.0/src/substrait/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      160 2023-06-16 20:34:07.000000 substrait-0.2.0/src/substrait/_version.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 20:34:07.669746 substrait-0.2.0/src/substrait/extensions/
+-rw-r--r--   0 runner    (1001) docker     (123)      149 2023-06-16 20:33:54.000000 substrait-0.2.0/src/substrait/extensions/extension_types.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      722 2023-06-16 20:33:54.000000 substrait-0.2.0/src/substrait/extensions/functions_aggregate_approx.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      921 2023-06-16 20:33:54.000000 substrait-0.2.0/src/substrait/extensions/functions_aggregate_generic.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)    44516 2023-06-16 20:33:54.000000 substrait-0.2.0/src/substrait/extensions/functions_arithmetic.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     4467 2023-06-16 20:33:54.000000 substrait-0.2.0/src/substrait/extensions/functions_arithmetic_decimal.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     3252 2023-06-16 20:33:54.000000 substrait-0.2.0/src/substrait/extensions/functions_boolean.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     4956 2023-06-16 20:33:54.000000 substrait-0.2.0/src/substrait/extensions/functions_comparison.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)    23562 2023-06-16 20:33:54.000000 substrait-0.2.0/src/substrait/extensions/functions_datetime.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     4213 2023-06-16 20:33:54.000000 substrait-0.2.0/src/substrait/extensions/functions_logarithmic.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)    11507 2023-06-16 20:33:54.000000 substrait-0.2.0/src/substrait/extensions/functions_rounding.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      733 2023-06-16 20:33:54.000000 substrait-0.2.0/src/substrait/extensions/functions_set.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)    51027 2023-06-16 20:33:54.000000 substrait-0.2.0/src/substrait/extensions/functions_string.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      683 2023-06-16 20:33:54.000000 substrait-0.2.0/src/substrait/extensions/type_variations.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     1302 2023-06-16 20:33:54.000000 substrait-0.2.0/src/substrait/extensions/unknown.yaml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 20:34:07.669746 substrait-0.2.0/src/substrait/gen/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-16 20:33:54.000000 substrait-0.2.0/src/substrait/gen/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 20:34:07.669746 substrait-0.2.0/src/substrait/gen/proto/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-16 20:33:54.000000 substrait-0.2.0/src/substrait/gen/proto/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    47948 2023-06-16 20:33:54.000000 substrait-0.2.0/src/substrait/gen/proto/algebra_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1527 2023-06-16 20:33:54.000000 substrait-0.2.0/src/substrait/gen/proto/capabilities_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2268 2023-06-16 20:33:54.000000 substrait-0.2.0/src/substrait/gen/proto/extended_expression_pb2.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 20:34:07.669746 substrait-0.2.0/src/substrait/gen/proto/extensions/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-16 20:33:54.000000 substrait-0.2.0/src/substrait/gen/proto/extensions/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3127 2023-06-16 20:33:54.000000 substrait-0.2.0/src/substrait/gen/proto/extensions/extensions_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7587 2023-06-16 20:33:54.000000 substrait-0.2.0/src/substrait/gen/proto/function_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8257 2023-06-16 20:33:54.000000 substrait-0.2.0/src/substrait/gen/proto/parameterized_types_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2341 2023-06-16 20:33:54.000000 substrait-0.2.0/src/substrait/gen/proto/plan_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10190 2023-06-16 20:33:54.000000 substrait-0.2.0/src/substrait/gen/proto/type_expressions_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10975 2023-06-16 20:33:54.000000 substrait-0.2.0/src/substrait/gen/proto/type_pb2.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 20:34:07.669746 substrait-0.2.0/src/substrait.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     4468 2023-06-16 20:34:07.000000 substrait-0.2.0/src/substrait.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1701 2023-06-16 20:34:07.000000 substrait-0.2.0/src/substrait.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-16 20:34:07.000000 substrait-0.2.0/src/substrait.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       88 2023-06-16 20:34:07.000000 substrait-0.2.0/src/substrait.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       10 2023-06-16 20:34:07.000000 substrait-0.2.0/src/substrait.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 20:34:07.669746 substrait-0.2.0/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)      660 2023-06-16 20:33:54.000000 substrait-0.2.0/tests/test_proto.py
```

### Comparing `substrait-0.1.0/.github/workflows/release.yml` & `substrait-0.2.0/.github/workflows/release.yml`

 * *Files 21% similar despite different names*

```diff
@@ -61,23 +61,7 @@
         with:
           name: dist
           path: dist/
       - name: Publish package to PyPI
         uses: pypa/gh-action-pypi-publish@release/v1
         with:
           password: ${{ secrets.PYPI_API_TOKEN }}
-  publish_test:
-    name: Publish to Test PyPI
-    runs-on: ubuntu-latest
-    needs: build
-    if: github.ref == 'refs/heads/main'
-    steps:
-      - name: Download artifact
-        uses: actions/download-artifact@v3
-        with:
-          name: dist
-          path: dist/
-      - name: Publish package to Test PyPI
-        uses: pypa/gh-action-pypi-publish@release/v1
-        with:
-          password: ${{ secrets.TEST_PYPI_API_TOKEN }}
-          repository-url: https://test.pypi.org/legacy/
```

### Comparing `substrait-0.1.0/.github/workflows/test.yml` & `substrait-0.2.0/.github/workflows/test.yml`

 * *Files identical despite different names*

### Comparing `substrait-0.1.0/.gitignore` & `substrait-0.2.0/.gitignore`

 * *Files identical despite different names*

### Comparing `substrait-0.1.0/CONTRIBUTING.md` & `substrait-0.2.0/CONTRIBUTING.md`

 * *Files identical despite different names*

### Comparing `substrait-0.1.0/LICENSE` & `substrait-0.2.0/LICENSE`

 * *Files identical despite different names*

### Comparing `substrait-0.1.0/PKG-INFO` & `substrait-0.2.0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: substrait
-Version: 0.1.0
+Version: 0.2.0
 Summary: A python package for Substrait.
 Author-email: Substrait contributors <substrait@googlegroups.com>
 License: Apache-2.0
 Requires-Python: >=3.8.1
 Description-Content-Type: text/markdown
 Provides-Extra: gen_proto
 Provides-Extra: test
```

### Comparing `substrait-0.1.0/README.md` & `substrait-0.2.0/README.md`

 * *Files identical despite different names*

### Comparing `substrait-0.1.0/pyproject.toml` & `substrait-0.2.0/pyproject.toml`

 * *Files 14% similar despite different names*

```diff
@@ -6,15 +6,14 @@
 readme = "README.md"
 requires-python = ">=3.8.1"
 dependencies = ["protobuf >= 3.20"]
 dynamic = ["version"]
 
 [tool.setuptools_scm]
 write_to = "src/substrait/_version.py"
-local_scheme = "no-local-version"
 
 [project.optional-dependencies]
 gen_proto = ["protobuf == 3.20.1", "protoletariat >= 2.0.0"]
 test = ["pytest >= 7.0.0"]
 
 [tool.pytest.ini_options]
 pythonpath = "src"
```

### Comparing `substrait-0.1.0/src/substrait/gen/proto/algebra_pb2.py` & `substrait-0.2.0/src/substrait/gen/proto/algebra_pb2.py`

 * *Files identical despite different names*

### Comparing `substrait-0.1.0/src/substrait/gen/proto/capabilities_pb2.py` & `substrait-0.2.0/src/substrait/gen/proto/capabilities_pb2.py`

 * *Files identical despite different names*

### Comparing `substrait-0.1.0/src/substrait/gen/proto/extended_expression_pb2.py` & `substrait-0.2.0/src/substrait/gen/proto/extended_expression_pb2.py`

 * *Files identical despite different names*

### Comparing `substrait-0.1.0/src/substrait/gen/proto/extensions/extensions_pb2.py` & `substrait-0.2.0/src/substrait/gen/proto/extensions/extensions_pb2.py`

 * *Files identical despite different names*

### Comparing `substrait-0.1.0/src/substrait/gen/proto/function_pb2.py` & `substrait-0.2.0/src/substrait/gen/proto/function_pb2.py`

 * *Files identical despite different names*

### Comparing `substrait-0.1.0/src/substrait/gen/proto/parameterized_types_pb2.py` & `substrait-0.2.0/src/substrait/gen/proto/parameterized_types_pb2.py`

 * *Files identical despite different names*

### Comparing `substrait-0.1.0/src/substrait/gen/proto/plan_pb2.py` & `substrait-0.2.0/src/substrait/gen/proto/plan_pb2.py`

 * *Files identical despite different names*

### Comparing `substrait-0.1.0/src/substrait/gen/proto/type_expressions_pb2.py` & `substrait-0.2.0/src/substrait/gen/proto/type_expressions_pb2.py`

 * *Files identical despite different names*

### Comparing `substrait-0.1.0/src/substrait/gen/proto/type_pb2.py` & `substrait-0.2.0/src/substrait/gen/proto/type_pb2.py`

 * *Files identical despite different names*

### Comparing `substrait-0.1.0/src/substrait.egg-info/PKG-INFO` & `substrait-0.2.0/src/substrait.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: substrait
-Version: 0.1.0
+Version: 0.2.0
 Summary: A python package for Substrait.
 Author-email: Substrait contributors <substrait@googlegroups.com>
 License: Apache-2.0
 Requires-Python: >=3.8.1
 Description-Content-Type: text/markdown
 Provides-Extra: gen_proto
 Provides-Extra: test
```

### Comparing `substrait-0.1.0/src/substrait.egg-info/SOURCES.txt` & `substrait-0.2.0/src/substrait.egg-info/SOURCES.txt`

 * *Files 22% similar despite different names*

```diff
@@ -6,23 +6,38 @@
 README.md
 buf.gen.yaml
 buf.work.yaml
 buf.yaml
 environment.yml
 gen_proto.sh
 pyproject.toml
+.github/workflows/pr_title.yml
 .github/workflows/release.yml
 .github/workflows/test.yml
 src/substrait/__init__.py
 src/substrait/_version.py
 src/substrait.egg-info/PKG-INFO
 src/substrait.egg-info/SOURCES.txt
 src/substrait.egg-info/dependency_links.txt
 src/substrait.egg-info/requires.txt
 src/substrait.egg-info/top_level.txt
+src/substrait/extensions/extension_types.yaml
+src/substrait/extensions/functions_aggregate_approx.yaml
+src/substrait/extensions/functions_aggregate_generic.yaml
+src/substrait/extensions/functions_arithmetic.yaml
+src/substrait/extensions/functions_arithmetic_decimal.yaml
+src/substrait/extensions/functions_boolean.yaml
+src/substrait/extensions/functions_comparison.yaml
+src/substrait/extensions/functions_datetime.yaml
+src/substrait/extensions/functions_logarithmic.yaml
+src/substrait/extensions/functions_rounding.yaml
+src/substrait/extensions/functions_set.yaml
+src/substrait/extensions/functions_string.yaml
+src/substrait/extensions/type_variations.yaml
+src/substrait/extensions/unknown.yaml
 src/substrait/gen/__init__.py
 src/substrait/gen/proto/__init__.py
 src/substrait/gen/proto/algebra_pb2.py
 src/substrait/gen/proto/capabilities_pb2.py
 src/substrait/gen/proto/extended_expression_pb2.py
 src/substrait/gen/proto/function_pb2.py
 src/substrait/gen/proto/parameterized_types_pb2.py
```

### Comparing `substrait-0.1.0/tests/test_proto.py` & `substrait-0.2.0/tests/test_proto.py`

 * *Files identical despite different names*

