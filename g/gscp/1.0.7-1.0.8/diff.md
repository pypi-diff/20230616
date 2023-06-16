# Comparing `tmp/gscp-1.0.7.tar.gz` & `tmp/gscp-1.0.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "gscp-1.0.7.tar", max compression
+gzip compressed data, was "gscp-1.0.8.tar", max compression
```

## Comparing `gscp-1.0.7.tar` & `gscp-1.0.8.tar`

### file list

```diff
@@ -1,13 +1,13 @@
--rw-r--r--   0        0        0        0 2023-06-13 16:16:02.479786 gscp-1.0.7/gscp/__init__.py
--rw-r--r--   0        0        0     2168 2023-06-13 16:16:02.479786 gscp-1.0.7/gscp/__main__.py
--rw-r--r--   0        0        0     1369 2023-06-13 16:16:02.479786 gscp-1.0.7/gscp/commit.py
--rw-r--r--   0        0        0       66 2023-06-13 16:16:02.479786 gscp-1.0.7/gscp/entry.py
--rw-r--r--   0        0        0      510 2023-06-13 16:16:02.479786 gscp-1.0.7/gscp/git.py
--rw-r--r--   0        0        0     2500 2023-06-13 16:16:02.479786 gscp-1.0.7/gscp/push_pull.py
--rw-r--r--   0        0        0      200 2023-06-13 16:16:02.479786 gscp-1.0.7/gscp/stage.py
--rw-r--r--   0        0        0     1363 2023-06-13 16:16:02.479786 gscp-1.0.7/gscp/version.py
--rw-r--r--   0        0        0     2929 2023-06-13 16:16:02.479786 gscp-1.0.7/gscp/wrappers.py
--rw-r--r--   0        0        0     1089 2023-06-13 16:16:02.479786 gscp-1.0.7/LICENSE
--rw-r--r--   0        0        0     1022 2023-06-13 16:16:02.479786 gscp-1.0.7/pyproject.toml
--rw-r--r--   0        0        0     1691 2023-06-13 16:16:02.479786 gscp-1.0.7/README.md
--rw-r--r--   0        0        0     2151 1970-01-01 00:00:00.000000 gscp-1.0.7/PKG-INFO
+-rw-r--r--   0        0        0        0 2023-06-16 17:59:37.508886 gscp-1.0.8/gscp/__init__.py
+-rw-r--r--   0        0        0     2145 2023-06-16 17:59:37.508886 gscp-1.0.8/gscp/__main__.py
+-rw-r--r--   0        0        0     1369 2023-06-16 17:59:37.508886 gscp-1.0.8/gscp/commit.py
+-rw-r--r--   0        0        0       66 2023-06-16 17:59:37.508886 gscp-1.0.8/gscp/entry.py
+-rw-r--r--   0        0        0      510 2023-06-16 17:59:37.508886 gscp-1.0.8/gscp/git.py
+-rw-r--r--   0        0        0     2500 2023-06-16 17:59:37.508886 gscp-1.0.8/gscp/push_pull.py
+-rw-r--r--   0        0        0      200 2023-06-16 17:59:37.508886 gscp-1.0.8/gscp/stage.py
+-rw-r--r--   0        0        0     1363 2023-06-16 17:59:37.508886 gscp-1.0.8/gscp/version.py
+-rw-r--r--   0        0        0     2929 2023-06-16 17:59:37.508886 gscp-1.0.8/gscp/wrappers.py
+-rw-r--r--   0        0        0     1089 2023-06-16 17:59:37.508886 gscp-1.0.8/LICENSE
+-rw-r--r--   0        0        0     1022 2023-06-16 17:59:37.508886 gscp-1.0.8/pyproject.toml
+-rw-r--r--   0        0        0     1691 2023-06-16 17:59:37.508886 gscp-1.0.8/README.md
+-rw-r--r--   0        0        0     2151 1970-01-01 00:00:00.000000 gscp-1.0.8/PKG-INFO
```

### Comparing `gscp-1.0.7/gscp/__main__.py` & `gscp-1.0.8/gscp/__main__.py`

 * *Files 14% similar despite different names*

```diff
@@ -57,29 +57,28 @@
     )
 
     return parser
 
 
 def main() -> None:
     console = Console()
-    in_repo = git_is_in_repo()
-
-    if not in_repo:
-        console.print("You are not in a git repository", style="bold red")
-        exit(1)
 
     parser = _create_argparser()
     args = parser.parse_args()
 
     commit_push_only = cast(bool, args.commit_push)
     message = args.message if args.message else ""
     no_verify = cast(bool, args.no_verify)
     amend = cast(bool, args.amend)
     force = cast(bool, args.force)
 
+    if not git_is_in_repo():
+        console.print("You are not in a git repository", style="bold red")
+        exit(1)
+
     if not commit_push_only:
         stage(console)
 
     if commit(message, amend=amend, no_verify=no_verify, console=console):
         push(force=force or amend)
```

### Comparing `gscp-1.0.7/gscp/commit.py` & `gscp-1.0.8/gscp/commit.py`

 * *Files identical despite different names*

### Comparing `gscp-1.0.7/gscp/push_pull.py` & `gscp-1.0.8/gscp/push_pull.py`

 * *Files identical despite different names*

### Comparing `gscp-1.0.7/gscp/version.py` & `gscp-1.0.8/gscp/version.py`

 * *Files identical despite different names*

### Comparing `gscp-1.0.7/gscp/wrappers.py` & `gscp-1.0.8/gscp/wrappers.py`

 * *Files identical despite different names*

### Comparing `gscp-1.0.7/LICENSE` & `gscp-1.0.8/LICENSE`

 * *Files identical despite different names*

### Comparing `gscp-1.0.7/pyproject.toml` & `gscp-1.0.8/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "gscp"
-version = "1.0.7"
+version = "1.0.8"
 description = "A tool to quickly commit your work with git."
 authors = ["Samuel Yvon <samuelyvon9@gmail.com>"]
 readme = "README.md"
 packages = [{ include = "gscp" }]
 
 [tool.poetry.dependencies]
 rich = "^13.3.2"
```

### Comparing `gscp-1.0.7/README.md` & `gscp-1.0.8/README.md`

 * *Files identical despite different names*

### Comparing `gscp-1.0.7/PKG-INFO` & `gscp-1.0.8/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: gscp
-Version: 1.0.7
+Version: 1.0.8
 Summary: A tool to quickly commit your work with git.
 Author: Samuel Yvon
 Author-email: samuelyvon9@gmail.com
 Requires-Python: >=3.8,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
```

