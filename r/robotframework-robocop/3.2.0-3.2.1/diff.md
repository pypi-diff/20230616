# Comparing `tmp/robotframework-robocop-3.2.0.tar.gz` & `tmp/robotframework-robocop-3.2.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "robotframework-robocop-3.2.0.tar", last modified: Thu Jun 15 15:41:07 2023, max compression
+gzip compressed data, was "robotframework-robocop-3.2.1.tar", last modified: Fri Jun 16 15:20:37 2023, max compression
```

## Comparing `robotframework-robocop-3.2.0.tar` & `robotframework-robocop-3.2.1.tar`

### file list

```diff
@@ -1,43 +1,43 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 15:41:07.664914 robotframework-robocop-3.2.0/
--rw-r--r--   0 runner    (1001) docker     (123)    11357 2023-06-15 15:40:54.000000 robotframework-robocop-3.2.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)       44 2023-06-15 15:40:54.000000 robotframework-robocop-3.2.0/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)    14103 2023-06-15 15:41:07.664914 robotframework-robocop-3.2.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    12529 2023-06-15 15:40:54.000000 robotframework-robocop-3.2.0/README.md
--rw-r--r--   0 runner    (1001) docker     (123)      304 2023-06-15 15:40:54.000000 robotframework-robocop-3.2.0/pyproject.toml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 15:41:07.664914 robotframework-robocop-3.2.0/robocop/
--rw-r--r--   0 runner    (1001) docker     (123)      223 2023-06-15 15:40:54.000000 robotframework-robocop-3.2.0/robocop/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-15 15:40:54.000000 robotframework-robocop-3.2.0/robocop/__main__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 15:41:07.664914 robotframework-robocop-3.2.0/robocop/checkers/
--rw-r--r--   0 runner    (1001) docker     (123)     5897 2023-06-15 15:40:54.000000 robotframework-robocop-3.2.0/robocop/checkers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     9388 2023-06-15 15:40:54.000000 robotframework-robocop-3.2.0/robocop/checkers/comments.py
--rw-r--r--   0 runner    (1001) docker     (123)     4206 2023-06-15 15:40:54.000000 robotframework-robocop-3.2.0/robocop/checkers/documentation.py
--rw-r--r--   0 runner    (1001) docker     (123)    17339 2023-06-15 15:40:54.000000 robotframework-robocop-3.2.0/robocop/checkers/duplications.py
--rw-r--r--   0 runner    (1001) docker     (123)    22768 2023-06-15 15:40:54.000000 robotframework-robocop-3.2.0/robocop/checkers/errors.py
--rw-r--r--   0 runner    (1001) docker     (123)    27361 2023-06-15 15:40:54.000000 robotframework-robocop-3.2.0/robocop/checkers/lengths.py
--rw-r--r--   0 runner    (1001) docker     (123)    40684 2023-06-15 15:40:54.000000 robotframework-robocop-3.2.0/robocop/checkers/misc.py
--rw-r--r--   0 runner    (1001) docker     (123)    44284 2023-06-15 15:40:54.000000 robotframework-robocop-3.2.0/robocop/checkers/naming.py
--rw-r--r--   0 runner    (1001) docker     (123)    33602 2023-06-15 15:40:54.000000 robotframework-robocop-3.2.0/robocop/checkers/spacing.py
--rw-r--r--   0 runner    (1001) docker     (123)    11490 2023-06-15 15:40:54.000000 robotframework-robocop-3.2.0/robocop/checkers/tags.py
--rw-r--r--   0 runner    (1001) docker     (123)    24721 2023-06-15 15:40:54.000000 robotframework-robocop-3.2.0/robocop/config.py
--rw-r--r--   0 runner    (1001) docker     (123)     3463 2023-06-15 15:40:54.000000 robotframework-robocop-3.2.0/robocop/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (123)     2914 2023-06-15 15:40:54.000000 robotframework-robocop-3.2.0/robocop/files.py
--rw-r--r--   0 runner    (1001) docker     (123)    18783 2023-06-15 15:40:54.000000 robotframework-robocop-3.2.0/robocop/reports.py
--rw-r--r--   0 runner    (1001) docker     (123)    14683 2023-06-15 15:40:54.000000 robotframework-robocop-3.2.0/robocop/rules.py
--rw-r--r--   0 runner    (1001) docker     (123)    11064 2023-06-15 15:40:54.000000 robotframework-robocop-3.2.0/robocop/run.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 15:41:07.664914 robotframework-robocop-3.2.0/robocop/utils/
--rw-r--r--   0 runner    (1001) docker     (123)      608 2023-06-15 15:40:54.000000 robotframework-robocop-3.2.0/robocop/utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5086 2023-06-15 15:40:54.000000 robotframework-robocop-3.2.0/robocop/utils/disablers.py
--rw-r--r--   0 runner    (1001) docker     (123)     2303 2023-06-15 15:40:54.000000 robotframework-robocop-3.2.0/robocop/utils/file_types.py
--rw-r--r--   0 runner    (1001) docker     (123)    12577 2023-06-15 15:40:54.000000 robotframework-robocop-3.2.0/robocop/utils/misc.py
--rw-r--r--   0 runner    (1001) docker     (123)     4639 2023-06-15 15:40:54.000000 robotframework-robocop-3.2.0/robocop/utils/run_keywords.py
--rw-r--r--   0 runner    (1001) docker     (123)    13535 2023-06-15 15:40:54.000000 robotframework-robocop-3.2.0/robocop/utils/version_matching.py
--rw-r--r--   0 runner    (1001) docker     (123)       22 2023-06-15 15:40:54.000000 robotframework-robocop-3.2.0/robocop/version.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 15:41:07.664914 robotframework-robocop-3.2.0/robotframework_robocop.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    14103 2023-06-15 15:41:07.000000 robotframework-robocop-3.2.0/robotframework_robocop.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      950 2023-06-15 15:41:07.000000 robotframework-robocop-3.2.0/robotframework_robocop.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-15 15:41:07.000000 robotframework-robocop-3.2.0/robotframework_robocop.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       48 2023-06-15 15:41:07.000000 robotframework-robocop-3.2.0/robotframework_robocop.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)      198 2023-06-15 15:41:07.000000 robotframework-robocop-3.2.0/robotframework_robocop.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        8 2023-06-15 15:41:07.000000 robotframework-robocop-3.2.0/robotframework_robocop.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-15 15:41:07.664914 robotframework-robocop-3.2.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     2446 2023-06-15 15:40:54.000000 robotframework-robocop-3.2.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 15:20:37.845709 robotframework-robocop-3.2.1/
+-rw-r--r--   0 runner    (1001) docker     (123)    11357 2023-06-16 15:20:27.000000 robotframework-robocop-3.2.1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)       44 2023-06-16 15:20:27.000000 robotframework-robocop-3.2.1/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)    14103 2023-06-16 15:20:37.845709 robotframework-robocop-3.2.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    12529 2023-06-16 15:20:27.000000 robotframework-robocop-3.2.1/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)      304 2023-06-16 15:20:27.000000 robotframework-robocop-3.2.1/pyproject.toml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 15:20:37.841709 robotframework-robocop-3.2.1/robocop/
+-rw-r--r--   0 runner    (1001) docker     (123)      223 2023-06-16 15:20:27.000000 robotframework-robocop-3.2.1/robocop/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-16 15:20:27.000000 robotframework-robocop-3.2.1/robocop/__main__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 15:20:37.841709 robotframework-robocop-3.2.1/robocop/checkers/
+-rw-r--r--   0 runner    (1001) docker     (123)     5897 2023-06-16 15:20:27.000000 robotframework-robocop-3.2.1/robocop/checkers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9388 2023-06-16 15:20:27.000000 robotframework-robocop-3.2.1/robocop/checkers/comments.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4206 2023-06-16 15:20:27.000000 robotframework-robocop-3.2.1/robocop/checkers/documentation.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17339 2023-06-16 15:20:27.000000 robotframework-robocop-3.2.1/robocop/checkers/duplications.py
+-rw-r--r--   0 runner    (1001) docker     (123)    22768 2023-06-16 15:20:27.000000 robotframework-robocop-3.2.1/robocop/checkers/errors.py
+-rw-r--r--   0 runner    (1001) docker     (123)    27361 2023-06-16 15:20:27.000000 robotframework-robocop-3.2.1/robocop/checkers/lengths.py
+-rw-r--r--   0 runner    (1001) docker     (123)    41796 2023-06-16 15:20:27.000000 robotframework-robocop-3.2.1/robocop/checkers/misc.py
+-rw-r--r--   0 runner    (1001) docker     (123)    44284 2023-06-16 15:20:27.000000 robotframework-robocop-3.2.1/robocop/checkers/naming.py
+-rw-r--r--   0 runner    (1001) docker     (123)    33524 2023-06-16 15:20:27.000000 robotframework-robocop-3.2.1/robocop/checkers/spacing.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11490 2023-06-16 15:20:27.000000 robotframework-robocop-3.2.1/robocop/checkers/tags.py
+-rw-r--r--   0 runner    (1001) docker     (123)    24721 2023-06-16 15:20:27.000000 robotframework-robocop-3.2.1/robocop/config.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3463 2023-06-16 15:20:27.000000 robotframework-robocop-3.2.1/robocop/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2914 2023-06-16 15:20:27.000000 robotframework-robocop-3.2.1/robocop/files.py
+-rw-r--r--   0 runner    (1001) docker     (123)    18783 2023-06-16 15:20:27.000000 robotframework-robocop-3.2.1/robocop/reports.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14683 2023-06-16 15:20:27.000000 robotframework-robocop-3.2.1/robocop/rules.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11064 2023-06-16 15:20:27.000000 robotframework-robocop-3.2.1/robocop/run.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 15:20:37.845709 robotframework-robocop-3.2.1/robocop/utils/
+-rw-r--r--   0 runner    (1001) docker     (123)      608 2023-06-16 15:20:27.000000 robotframework-robocop-3.2.1/robocop/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5086 2023-06-16 15:20:27.000000 robotframework-robocop-3.2.1/robocop/utils/disablers.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2303 2023-06-16 15:20:27.000000 robotframework-robocop-3.2.1/robocop/utils/file_types.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12577 2023-06-16 15:20:27.000000 robotframework-robocop-3.2.1/robocop/utils/misc.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4639 2023-06-16 15:20:27.000000 robotframework-robocop-3.2.1/robocop/utils/run_keywords.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13535 2023-06-16 15:20:27.000000 robotframework-robocop-3.2.1/robocop/utils/version_matching.py
+-rw-r--r--   0 runner    (1001) docker     (123)       22 2023-06-16 15:20:27.000000 robotframework-robocop-3.2.1/robocop/version.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 15:20:37.845709 robotframework-robocop-3.2.1/robotframework_robocop.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    14103 2023-06-16 15:20:37.000000 robotframework-robocop-3.2.1/robotframework_robocop.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      950 2023-06-16 15:20:37.000000 robotframework-robocop-3.2.1/robotframework_robocop.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-16 15:20:37.000000 robotframework-robocop-3.2.1/robotframework_robocop.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       48 2023-06-16 15:20:37.000000 robotframework-robocop-3.2.1/robotframework_robocop.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      198 2023-06-16 15:20:37.000000 robotframework-robocop-3.2.1/robotframework_robocop.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        8 2023-06-16 15:20:37.000000 robotframework-robocop-3.2.1/robotframework_robocop.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-16 15:20:37.845709 robotframework-robocop-3.2.1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     2446 2023-06-16 15:20:27.000000 robotframework-robocop-3.2.1/setup.py
```

### Comparing `robotframework-robocop-3.2.0/LICENSE` & `robotframework-robocop-3.2.1/LICENSE`

 * *Files identical despite different names*

### Comparing `robotframework-robocop-3.2.0/PKG-INFO` & `robotframework-robocop-3.2.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: robotframework-robocop
-Version: 3.2.0
+Version: 3.2.1
 Summary: Static code analysis tool (linter) for Robot Framework
 Home-page: https://github.com/MarketSquare/robotframework-robocop
 Download-URL: https://pypi.org/project/robotframework-robocop
 Author: Bartlomiej Hirsz, Mateusz Nojek
 Author-email: bartek.hirsz@gmail.com, matnojek@gmail.com
 License: Apache License 2.0
 Project-URL: Documentation, https://robocop.readthedocs.io/en/stable
```

### Comparing `robotframework-robocop-3.2.0/README.md` & `robotframework-robocop-3.2.1/README.md`

 * *Files identical despite different names*

### Comparing `robotframework-robocop-3.2.0/robocop/checkers/__init__.py` & `robotframework-robocop-3.2.1/robocop/checkers/__init__.py`

 * *Files identical despite different names*

### Comparing `robotframework-robocop-3.2.0/robocop/checkers/comments.py` & `robotframework-robocop-3.2.1/robocop/checkers/comments.py`

 * *Files identical despite different names*

### Comparing `robotframework-robocop-3.2.0/robocop/checkers/documentation.py` & `robotframework-robocop-3.2.1/robocop/checkers/documentation.py`

 * *Files identical despite different names*

### Comparing `robotframework-robocop-3.2.0/robocop/checkers/duplications.py` & `robotframework-robocop-3.2.1/robocop/checkers/duplications.py`

 * *Files identical despite different names*

### Comparing `robotframework-robocop-3.2.0/robocop/checkers/errors.py` & `robotframework-robocop-3.2.1/robocop/checkers/errors.py`

 * *Files identical despite different names*

### Comparing `robotframework-robocop-3.2.0/robocop/checkers/lengths.py` & `robotframework-robocop-3.2.1/robocop/checkers/lengths.py`

 * *Files identical despite different names*

### Comparing `robotframework-robocop-3.2.0/robocop/checkers/misc.py` & `robotframework-robocop-3.2.1/robocop/checkers/misc.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,11 +1,12 @@
 """
 Miscellaneous checkers
 """
 from collections import namedtuple
+from dataclasses import dataclass
 from pathlib import Path
 
 from robot.api import Token
 from robot.errors import VariableError
 from robot.parsing.model.blocks import TestCaseSection
 from robot.parsing.model.statements import Arguments, KeywordCall, Return, Teardown
 from robot.utils import unescape
@@ -870,29 +871,34 @@
             name=token_type,
             statement_type="statement",
             node=node,
             col=token_col(node, token_type),
         )
 
 
-CachedVariable = namedtuple("CachedVariable", "name token")
+@dataclass
+class CachedVariable:
+    name: str
+    token: Token
+    is_used: bool
 
 
 class UnusedVariablesChecker(VisitorChecker):
     reports = (
         "unused-argument",
         "unused-variable",
         "argument-overwritten-before-usage",
         "variable-overwritten-before-usage",
     )
 
     def __init__(self):
         self.arguments = {}
         self.variables = [{}]  # variables are list of scope-dictionaries, to support IF branches
         self.ignore_overwriting = False  # temporarily ignore overwriting, e.g. in FOR loops
+        self.in_loop = False  # if we're in the loop we need to check whole scope for unused-variable
         super().__init__()
 
     def visit_TestCase(self, node):  # noqa
         self.variables = [{}]
         self.generic_visit(node)
         self.check_unused_variables()
 
@@ -903,37 +909,39 @@
         self.parse_embedded_arguments(name_token)
         # iterating there instead of using visit_Arguments, so we don't check keywords without arguments
         for statement in node.body:
             if isinstance(statement, Arguments):
                 self.parse_arguments(statement)
         self.generic_visit(node)
         for arg in self.arguments.values():
-            value, *_ = arg.token.value.split("=", maxsplit=1)
-            self.report_arg_or_var_rule("unused-argument", arg.token, value)
+            if not arg.is_used:
+                value, *_ = arg.token.value.split("=", maxsplit=1)
+                self.report_arg_or_var_rule("unused-argument", arg.token, value)
         self.check_unused_variables()
 
     def check_unused_variables(self):
         for scope in self.variables:
             for variable in scope.values():
-                self.report_arg_or_var_rule("unused-variable", variable.token, variable.name)
+                if not variable.is_used:
+                    self.report_arg_or_var_rule("unused-variable", variable.token, variable.name)
 
     def report_arg_or_var_rule(self, rule, token, value=None):
         if value is None:
             value = token.value
         self.report(
             rule,
             name=value,
             node=token,
             lineno=token.lineno,
             col=token.col_offset + 1,
             end_col=token.col_offset + len(value) + 1,
         )
 
     def add_argument(self, argument, normalized_name, token):
-        self.arguments[normalized_name] = CachedVariable(argument, token)
+        self.arguments[normalized_name] = CachedVariable(argument, token, False)
 
     def parse_arguments(self, node):
         """Store arguments from [Arguments]. Ignore @{args} and &{kwargs}, strip default values."""
         if get_errors(node):
             return
         for arg in node.get_tokens(Token.ARGUMENT):
             if arg.value[0] in ("@", "&"):  # ignore *args and &kwargs
@@ -963,33 +971,44 @@
         self.variables.append({})
         for item in node.body:
             self.visit(item)
         self.variables.pop()
         if node.orelse:
             self.visit(node.orelse)
 
+    def clear_variables_after_loop(self):
+        """Remove used variables after loop finishes."""
+        for index, scope in enumerate(self.variables):
+            self.variables[index] = {name: variable for name, variable in scope.items() if not variable.is_used}
+
     def visit_While(self, node):  # noqa
         if node.header.errors:
             return node
+        self.in_loop = True
         for token in node.header.get_tokens(Token.ARGUMENT):
             self.find_not_nested_variable(token.value, is_var=False)
         if node.limit:
             self.find_not_nested_variable(node.limit, is_var=False)
-        return self.generic_visit(node)
+        self.generic_visit(node)
+        self.in_loop = False
+        self.clear_variables_after_loop()
 
     def visit_For(self, node):  # noqa
         if getattr(node.header, "errors", None):
             return node
+        self.in_loop = True
         self.ignore_overwriting = True
         for token in node.header.get_tokens(Token.ARGUMENT):
             self.find_not_nested_variable(token.value, is_var=False)
         for token in node.header.get_tokens(Token.VARIABLE):
             self.handle_assign_variable(token, remove_equal=False)
         self.generic_visit(node)
         self.ignore_overwriting = False
+        self.in_loop = False
+        self.clear_variables_after_loop()
 
     visit_ForLoop = visit_For
 
     def visit_Try(self, node):  # noqa
         if node.errors or node.header.errors:
             return node
         if node.variable is not None:
@@ -1023,19 +1042,27 @@
             value = value.rstrip("=").strip()  # remove possible '=' and ' ='
         normalized = normalize_robot_var_name(value)  # remove ${ } and normalize
         if not normalized:  # ie. "${_}" -> ""
             return
         arg = self.arguments.pop(normalized, None)
         if arg is not None:
             self.report_arg_or_var_rule("argument-overwritten-before-usage", arg.token)
+        is_used = False
         for variable_scope in self.variables[::-1]:
-            variable = variable_scope.pop(normalized, None)
-            if variable is not None and not self.ignore_overwriting:
-                self.report_arg_or_var_rule("variable-overwritten-before-usage", variable.token, value)
-        self.variables[-1][normalized] = CachedVariable(value, token)
+            if normalized in variable_scope:
+                is_used = variable_scope[normalized].is_used or is_used
+                if not variable_scope[normalized].is_used and not self.ignore_overwriting:
+                    self.report_arg_or_var_rule(
+                        "variable-overwritten-before-usage", variable_scope[normalized].token, value
+                    )
+        if self.in_loop:
+            variable = CachedVariable(value, token, is_used)
+        else:
+            variable = CachedVariable(value, token, False)
+        self.variables[-1][normalized] = variable
 
     def find_not_nested_variable(self, value, is_var):
         """Find and process not nested variable.
 
         Search `value` string until there is ${variable} without other variables inside. Unescaped escaped syntax
         ($var or \\${var}). If variable does exist in assign variables or arguments, it is removed to denote it was
         used.
@@ -1090,20 +1117,22 @@
           arg["value"] -> arg
         """
         normalized = normalize_robot_name(variable_name)
         arg = self.arguments.pop(normalized, None)
         if arg is None:
             self.search_by_removing_attr_access(normalized, self.arguments)
         for variable_scope in self.variables[::-1]:
-            arg_var = variable_scope.pop(normalized, None)
-            if arg_var is None:
+            if normalized in variable_scope:
+                variable_scope[normalized].is_used = True
+            else:
                 self.search_by_removing_attr_access(normalized, variable_scope)
 
     @staticmethod
     def search_by_removing_attr_access(variable_name, variable_scope):
         """Search and remove variables from variable_scope by removing attribute access elements from the name."""
-        for attr_access in (".", "[", "("):  # ${arg.attr}
+        for attr_access in (".", "[", "(", "%", "+", "-", "*", "/"):  # ${arg.attr}
             if attr_access in variable_name:
                 name, _ = variable_name.split(attr_access, maxsplit=1)
-                arg_var = variable_scope.pop(name, None)
-                if arg_var is not None:
+                name = name.strip()
+                if name in variable_scope:
+                    variable_scope[name].is_used = True
                     return
```

### Comparing `robotframework-robocop-3.2.0/robocop/checkers/naming.py` & `robotframework-robocop-3.2.1/robocop/checkers/naming.py`

 * *Files identical despite different names*

### Comparing `robotframework-robocop-3.2.0/robocop/checkers/spacing.py` & `robotframework-robocop-3.2.1/robocop/checkers/spacing.py`

 * *Files 0% similar despite different names*

```diff
@@ -453,16 +453,14 @@
                     for statement in reversed(child.body):
                         if isinstance(statement, EmptyLine):
                             empty_lines += 1
                         else:
                             break
                 if isinstance(child, EmptyLine):
                     empty_lines += 1
-                elif isinstance(child, Comment):
-                    continue
                 else:
                     break
             if empty_lines != self.param("empty-lines-between-sections", "empty_lines"):
                 self.report(
                     "empty-lines-between-sections",
                     empty_lines=empty_lines,
                     allowed_empty_lines=self.param("empty-lines-between-sections", "empty_lines"),
```

### Comparing `robotframework-robocop-3.2.0/robocop/checkers/tags.py` & `robotframework-robocop-3.2.1/robocop/checkers/tags.py`

 * *Files identical despite different names*

### Comparing `robotframework-robocop-3.2.0/robocop/config.py` & `robotframework-robocop-3.2.1/robocop/config.py`

 * *Files identical despite different names*

### Comparing `robotframework-robocop-3.2.0/robocop/exceptions.py` & `robotframework-robocop-3.2.1/robocop/exceptions.py`

 * *Files identical despite different names*

### Comparing `robotframework-robocop-3.2.0/robocop/files.py` & `robotframework-robocop-3.2.1/robocop/files.py`

 * *Files identical despite different names*

### Comparing `robotframework-robocop-3.2.0/robocop/reports.py` & `robotframework-robocop-3.2.1/robocop/reports.py`

 * *Files identical despite different names*

### Comparing `robotframework-robocop-3.2.0/robocop/rules.py` & `robotframework-robocop-3.2.1/robocop/rules.py`

 * *Files identical despite different names*

### Comparing `robotframework-robocop-3.2.0/robocop/run.py` & `robotframework-robocop-3.2.1/robocop/run.py`

 * *Files identical despite different names*

### Comparing `robotframework-robocop-3.2.0/robocop/utils/__init__.py` & `robotframework-robocop-3.2.1/robocop/utils/__init__.py`

 * *Files identical despite different names*

### Comparing `robotframework-robocop-3.2.0/robocop/utils/disablers.py` & `robotframework-robocop-3.2.1/robocop/utils/disablers.py`

 * *Files identical despite different names*

### Comparing `robotframework-robocop-3.2.0/robocop/utils/file_types.py` & `robotframework-robocop-3.2.1/robocop/utils/file_types.py`

 * *Files identical despite different names*

### Comparing `robotframework-robocop-3.2.0/robocop/utils/misc.py` & `robotframework-robocop-3.2.1/robocop/utils/misc.py`

 * *Files identical despite different names*

### Comparing `robotframework-robocop-3.2.0/robocop/utils/run_keywords.py` & `robotframework-robocop-3.2.1/robocop/utils/run_keywords.py`

 * *Files identical despite different names*

### Comparing `robotframework-robocop-3.2.0/robocop/utils/version_matching.py` & `robotframework-robocop-3.2.1/robocop/utils/version_matching.py`

 * *Files identical despite different names*

### Comparing `robotframework-robocop-3.2.0/robotframework_robocop.egg-info/PKG-INFO` & `robotframework-robocop-3.2.1/robotframework_robocop.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: robotframework-robocop
-Version: 3.2.0
+Version: 3.2.1
 Summary: Static code analysis tool (linter) for Robot Framework
 Home-page: https://github.com/MarketSquare/robotframework-robocop
 Download-URL: https://pypi.org/project/robotframework-robocop
 Author: Bartlomiej Hirsz, Mateusz Nojek
 Author-email: bartek.hirsz@gmail.com, matnojek@gmail.com
 License: Apache License 2.0
 Project-URL: Documentation, https://robocop.readthedocs.io/en/stable
```

### Comparing `robotframework-robocop-3.2.0/robotframework_robocop.egg-info/SOURCES.txt` & `robotframework-robocop-3.2.1/robotframework_robocop.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `robotframework-robocop-3.2.0/setup.py` & `robotframework-robocop-3.2.1/setup.py`

 * *Files identical despite different names*

