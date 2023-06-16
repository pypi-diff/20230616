# Comparing `tmp/deadcode-0.0.1.tar.gz` & `tmp/deadcode-0.0.2.tar.gz`

## Comparing `deadcode-0.0.1.tar` & `deadcode-0.0.2.tar`

### file list

```diff
@@ -1,18 +1,16 @@
--rw-r--r--   0        0        0      197 2020-02-02 00:00:00.000000 deadcode-0.0.1/.flake8
--rw-r--r--   0        0        0      390 2020-02-02 00:00:00.000000 deadcode-0.0.1/Makefile
--rw-r--r--   0        0        0     3169 2020-02-02 00:00:00.000000 deadcode-0.0.1/notes
--rw-r--r--   0        0        0      661 2020-02-02 00:00:00.000000 deadcode-0.0.1/requirements-dev.txt
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 deadcode-0.0.1/requirements.txt
--rw-r--r--   0        0        0      132 2020-02-02 00:00:00.000000 deadcode-0.0.1/dead_code/Makefile
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 deadcode-0.0.1/dead_code/__init__.py
--rw-r--r--   0        0        0     2512 2020-02-02 00:00:00.000000 deadcode-0.0.1/dead_code/cli.py
--rw-r--r--   0        0        0      122 2020-02-02 00:00:00.000000 deadcode-0.0.1/dead_code/tests/module_a.py
--rw-r--r--   0        0        0       80 2020-02-02 00:00:00.000000 deadcode-0.0.1/dead_code/tests/module_b.py
--rw-r--r--   0        0        0      561 2020-02-02 00:00:00.000000 deadcode-0.0.1/dead_code/tests/test_dead_code_finder.py
--rw-r--r--   0        0        0      365 2020-02-02 00:00:00.000000 deadcode-0.0.1/dead_code/tests/test_case1/hello_world.py
--rw-r--r--   0        0        0       42 2020-02-02 00:00:00.000000 deadcode-0.0.1/dead_code/tests/test_case1/subdir/one_more_file.py
--rw-r--r--   0        0        0       23 2020-02-02 00:00:00.000000 deadcode-0.0.1/dead_code/tests/test_case1/subdir/another_subdir/__init__.py
--rw-r--r--   0        0        0     3078 2020-02-02 00:00:00.000000 deadcode-0.0.1/.gitignore
--rw-r--r--   0        0        0      219 2020-02-02 00:00:00.000000 deadcode-0.0.1/README.md
--rw-r--r--   0        0        0     1299 2020-02-02 00:00:00.000000 deadcode-0.0.1/pyproject.toml
--rw-r--r--   0        0        0      879 2020-02-02 00:00:00.000000 deadcode-0.0.1/PKG-INFO
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 deadcode-0.0.2/deadcode/__init__.py
+-rw-r--r--   0        0        0     4604 2020-02-02 00:00:00.000000 deadcode-0.0.2/deadcode/cli.py
+-rw-r--r--   0        0        0      347 2020-02-02 00:00:00.000000 deadcode-0.0.2/deadcode/data_types.py
+-rw-r--r--   0        0        0      637 2020-02-02 00:00:00.000000 deadcode-0.0.2/deadcode/utils.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 deadcode-0.0.2/deadcode/actions/__init__.py
+-rw-r--r--   0        0        0     1242 2020-02-02 00:00:00.000000 deadcode-0.0.2/deadcode/actions/argument_parsing.py
+-rw-r--r--   0        0        0      122 2020-02-02 00:00:00.000000 deadcode-0.0.2/deadcode/tests/module_a.py
+-rw-r--r--   0        0        0       80 2020-02-02 00:00:00.000000 deadcode-0.0.2/deadcode/tests/module_b.py
+-rw-r--r--   0        0        0     3542 2020-02-02 00:00:00.000000 deadcode-0.0.2/deadcode/tests/test_deadcode.py
+-rw-r--r--   0        0        0      364 2020-02-02 00:00:00.000000 deadcode-0.0.2/deadcode/tests/test_case1/hello_world.py
+-rw-r--r--   0        0        0       40 2020-02-02 00:00:00.000000 deadcode-0.0.2/deadcode/tests/test_case1/subdir/one_more_file.py
+-rw-r--r--   0        0        0       22 2020-02-02 00:00:00.000000 deadcode-0.0.2/deadcode/tests/test_case1/subdir/another_subdir/__init__.py
+-rw-r--r--   0        0        0     3078 2020-02-02 00:00:00.000000 deadcode-0.0.2/.gitignore
+-rw-r--r--   0        0        0      219 2020-02-02 00:00:00.000000 deadcode-0.0.2/README.md
+-rw-r--r--   0        0        0     1356 2020-02-02 00:00:00.000000 deadcode-0.0.2/pyproject.toml
+-rw-r--r--   0        0        0     1000 2020-02-02 00:00:00.000000 deadcode-0.0.2/PKG-INFO
```

### Comparing `deadcode-0.0.1/.gitignore` & `deadcode-0.0.2/.gitignore`

 * *Files identical despite different names*

### Comparing `deadcode-0.0.1/PKG-INFO` & `deadcode-0.0.2/PKG-INFO`

 * *Files 18% similar despite different names*

```diff
@@ -1,11 +1,13 @@
 Metadata-Version: 2.1
 Name: deadcode
-Version: 0.0.1
+Version: 0.0.2
 Summary: Find and remove dead code.
+Project-URL: Homepage, https://github.com/albertas/deadcode
+Project-URL: Documentation, https://deadcode.readthedocs.io/
 Author-email: Albertas Gimbutas <albertasgim@gmail.com>
 Classifier: Development Status :: 3 - Alpha
 Classifier: License :: OSI Approved :: GNU Affero General Public License v3
 Classifier: Natural Language :: English
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3.8
```

