# Comparing `tmp/RepRepBuild-0.8.0.tar.gz` & `tmp/RepRepBuild-0.9.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "RepRepBuild-0.8.0.tar", last modified: Fri May 26 15:53:59 2023, max compression
+gzip compressed data, was "RepRepBuild-0.9.0.tar", last modified: Fri Jun 16 10:01:22 2023, max compression
```

## Comparing `RepRepBuild-0.8.0.tar` & `RepRepBuild-0.9.0.tar`

### file list

```diff
@@ -1,37 +1,37 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 15:53:59.209849 RepRepBuild-0.8.0/
--rw-r--r--   0 runner    (1001) docker     (123)      283 2023-05-26 15:53:48.000000 RepRepBuild-0.8.0/.editorconfig
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 15:53:59.209849 RepRepBuild-0.8.0/.github/
--rw-r--r--   0 runner    (1001) docker     (123)      257 2023-05-26 15:53:48.000000 RepRepBuild-0.8.0/.github/dependabot.yaml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 15:53:59.209849 RepRepBuild-0.8.0/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (123)     1038 2023-05-26 15:53:48.000000 RepRepBuild-0.8.0/.github/workflows/pypi.yaml
--rw-r--r--   0 runner    (1001) docker     (123)       58 2023-05-26 15:53:48.000000 RepRepBuild-0.8.0/.gitignore
--rw-r--r--   0 runner    (1001) docker     (123)     1006 2023-05-26 15:53:48.000000 RepRepBuild-0.8.0/.pre-commit-config.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     4855 2023-05-26 15:53:48.000000 RepRepBuild-0.8.0/CHANGELOG.md
--rw-r--r--   0 runner    (1001) docker     (123)    35149 2023-05-26 15:53:48.000000 RepRepBuild-0.8.0/COPYING
--rw-r--r--   0 runner    (1001) docker     (123)      188 2023-05-26 15:53:48.000000 RepRepBuild-0.8.0/DEVELOPMENT.md
--rw-r--r--   0 runner    (1001) docker     (123)      775 2023-05-26 15:53:48.000000 RepRepBuild-0.8.0/HEADER
--rw-r--r--   0 runner    (1001) docker     (123)    43046 2023-05-26 15:53:59.209849 RepRepBuild-0.8.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1392 2023-05-26 15:53:48.000000 RepRepBuild-0.8.0/README.md
--rw-r--r--   0 runner    (1001) docker     (123)     2027 2023-05-26 15:53:48.000000 RepRepBuild-0.8.0/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-26 15:53:59.209849 RepRepBuild-0.8.0/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 15:53:59.205849 RepRepBuild-0.8.0/src/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 15:53:59.209849 RepRepBuild-0.8.0/src/RepRepBuild.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    43046 2023-05-26 15:53:59.000000 RepRepBuild-0.8.0/src/RepRepBuild.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      735 2023-05-26 15:53:59.000000 RepRepBuild-0.8.0/src/RepRepBuild.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-26 15:53:59.000000 RepRepBuild-0.8.0/src/RepRepBuild.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      362 2023-05-26 15:53:59.000000 RepRepBuild-0.8.0/src/RepRepBuild.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)       42 2023-05-26 15:53:59.000000 RepRepBuild-0.8.0/src/RepRepBuild.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       12 2023-05-26 15:53:59.000000 RepRepBuild-0.8.0/src/RepRepBuild.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 15:53:59.209849 RepRepBuild-0.8.0/src/reprepbuild/
--rw-r--r--   0 runner    (1001) docker     (123)      939 2023-05-26 15:53:48.000000 RepRepBuild-0.8.0/src/reprepbuild/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    11553 2023-05-26 15:53:48.000000 RepRepBuild-0.8.0/src/reprepbuild/__main__.py
--rw-r--r--   0 runner    (1001) docker     (123)      160 2023-05-26 15:53:59.000000 RepRepBuild-0.8.0/src/reprepbuild/_version.py
--rw-r--r--   0 runner    (1001) docker     (123)     1803 2023-05-26 15:53:48.000000 RepRepBuild-0.8.0/src/reprepbuild/articlezip.py
--rw-r--r--   0 runner    (1001) docker     (123)     3517 2023-05-26 15:53:48.000000 RepRepBuild-0.8.0/src/reprepbuild/bibtex.py
--rw-r--r--   0 runner    (1001) docker     (123)     3933 2023-05-26 15:53:48.000000 RepRepBuild-0.8.0/src/reprepbuild/latex.py
--rw-r--r--   0 runner    (1001) docker     (123)     4530 2023-05-26 15:53:48.000000 RepRepBuild-0.8.0/src/reprepbuild/latexdep.py
--rw-r--r--   0 runner    (1001) docker     (123)     1792 2023-05-26 15:53:48.000000 RepRepBuild-0.8.0/src/reprepbuild/normalizepdf.py
--rw-r--r--   0 runner    (1001) docker     (123)     3952 2023-05-26 15:53:48.000000 RepRepBuild-0.8.0/src/reprepbuild/pythonscript.py
--rw-r--r--   0 runner    (1001) docker     (123)     2889 2023-05-26 15:53:48.000000 RepRepBuild-0.8.0/src/reprepbuild/repeat.py
--rw-r--r--   0 runner    (1001) docker     (123)     6733 2023-05-26 15:53:48.000000 RepRepBuild-0.8.0/src/reprepbuild/utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     2340 2023-05-26 15:53:48.000000 RepRepBuild-0.8.0/src/reprepbuild/zip.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 10:01:22.060119 RepRepBuild-0.9.0/
+-rw-r--r--   0 runner    (1001) docker     (123)      283 2023-06-16 10:01:12.000000 RepRepBuild-0.9.0/.editorconfig
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 10:01:22.052119 RepRepBuild-0.9.0/.github/
+-rw-r--r--   0 runner    (1001) docker     (123)      257 2023-06-16 10:01:12.000000 RepRepBuild-0.9.0/.github/dependabot.yaml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 10:01:22.052119 RepRepBuild-0.9.0/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (123)     1038 2023-06-16 10:01:12.000000 RepRepBuild-0.9.0/.github/workflows/pypi.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)       58 2023-06-16 10:01:12.000000 RepRepBuild-0.9.0/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (123)     1006 2023-06-16 10:01:12.000000 RepRepBuild-0.9.0/.pre-commit-config.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     5172 2023-06-16 10:01:12.000000 RepRepBuild-0.9.0/CHANGELOG.md
+-rw-r--r--   0 runner    (1001) docker     (123)    35149 2023-06-16 10:01:12.000000 RepRepBuild-0.9.0/COPYING
+-rw-r--r--   0 runner    (1001) docker     (123)      188 2023-06-16 10:01:12.000000 RepRepBuild-0.9.0/DEVELOPMENT.md
+-rw-r--r--   0 runner    (1001) docker     (123)      775 2023-06-16 10:01:12.000000 RepRepBuild-0.9.0/HEADER
+-rw-r--r--   0 runner    (1001) docker     (123)    43046 2023-06-16 10:01:22.060119 RepRepBuild-0.9.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1392 2023-06-16 10:01:12.000000 RepRepBuild-0.9.0/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)     2038 2023-06-16 10:01:12.000000 RepRepBuild-0.9.0/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-16 10:01:22.060119 RepRepBuild-0.9.0/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 10:01:22.048119 RepRepBuild-0.9.0/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 10:01:22.056119 RepRepBuild-0.9.0/src/RepRepBuild.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    43046 2023-06-16 10:01:22.000000 RepRepBuild-0.9.0/src/RepRepBuild.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      735 2023-06-16 10:01:22.000000 RepRepBuild-0.9.0/src/RepRepBuild.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-16 10:01:22.000000 RepRepBuild-0.9.0/src/RepRepBuild.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      362 2023-06-16 10:01:22.000000 RepRepBuild-0.9.0/src/RepRepBuild.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       42 2023-06-16 10:01:22.000000 RepRepBuild-0.9.0/src/RepRepBuild.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       12 2023-06-16 10:01:22.000000 RepRepBuild-0.9.0/src/RepRepBuild.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 10:01:22.056119 RepRepBuild-0.9.0/src/reprepbuild/
+-rw-r--r--   0 runner    (1001) docker     (123)      939 2023-06-16 10:01:12.000000 RepRepBuild-0.9.0/src/reprepbuild/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11515 2023-06-16 10:01:12.000000 RepRepBuild-0.9.0/src/reprepbuild/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      160 2023-06-16 10:01:21.000000 RepRepBuild-0.9.0/src/reprepbuild/_version.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1803 2023-06-16 10:01:12.000000 RepRepBuild-0.9.0/src/reprepbuild/articlezip.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3517 2023-06-16 10:01:12.000000 RepRepBuild-0.9.0/src/reprepbuild/bibtex.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3933 2023-06-16 10:01:12.000000 RepRepBuild-0.9.0/src/reprepbuild/latex.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4530 2023-06-16 10:01:12.000000 RepRepBuild-0.9.0/src/reprepbuild/latexdep.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1792 2023-06-16 10:01:12.000000 RepRepBuild-0.9.0/src/reprepbuild/normalizepdf.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3963 2023-06-16 10:01:12.000000 RepRepBuild-0.9.0/src/reprepbuild/pythonscript.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2889 2023-06-16 10:01:12.000000 RepRepBuild-0.9.0/src/reprepbuild/repeat.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6733 2023-06-16 10:01:12.000000 RepRepBuild-0.9.0/src/reprepbuild/utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2340 2023-06-16 10:01:12.000000 RepRepBuild-0.9.0/src/reprepbuild/zip.py
```

### Comparing `RepRepBuild-0.8.0/.github/workflows/pypi.yaml` & `RepRepBuild-0.9.0/.github/workflows/pypi.yaml`

 * *Files identical despite different names*

### Comparing `RepRepBuild-0.8.0/.pre-commit-config.yaml` & `RepRepBuild-0.9.0/.pre-commit-config.yaml`

 * *Files 2% similar despite different names*

```diff
@@ -25,14 +25,14 @@
   hooks:
     - id: remove-crlf
 - repo: https://github.com/psf/black
   rev: 23.3.0
   hooks:
     - id: black
 - repo: https://github.com/charliermarsh/ruff-pre-commit
-  rev: 'v0.0.269'
+  rev: 'v0.0.272'
   hooks:
     - id: ruff
 - repo: https://github.com/python-jsonschema/check-jsonschema
-  rev: 0.23.0
+  rev: 0.23.1
   hooks:
     - id: check-github-workflows
```

### Comparing `RepRepBuild-0.8.0/CHANGELOG.md` & `RepRepBuild-0.9.0/CHANGELOG.md`

 * *Files 7% similar despite different names*

```diff
@@ -3,14 +3,23 @@
 All notable changes to this project will be documented in this file.
 
 The format is based on [Keep a Changelog](https://keepachangelog.com/en/1.1.0/),
 and this project adheres to [Semantic Versioning](https://semver.org/spec/v2.0.0.html).
 
 ## [Unreleased]
 
+## [0.9.0] - 2023-06-16
+
+## Changed
+
+- The variable `REPREPBUILD_CASE_FMT` is no longer prefixed with the script name
+  to create filenames for log and dependency files.
+  Instead, it is used as such, without prefixing anything to it.
+- A plain `dataset` directory is now also recognized and turned into a ZIP file.
+
 ## [0.8.0] - 2023-05-26
 
 ### Fixed
 
 - Added sanity check to `rrr` command.
 
 ### Changed
```

### Comparing `RepRepBuild-0.8.0/COPYING` & `RepRepBuild-0.9.0/COPYING`

 * *Files identical despite different names*

### Comparing `RepRepBuild-0.8.0/HEADER` & `RepRepBuild-0.9.0/HEADER`

 * *Files identical despite different names*

### Comparing `RepRepBuild-0.8.0/PKG-INFO` & `RepRepBuild-0.9.0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: RepRepBuild
-Version: 0.8.0
+Version: 0.9.0
 Summary: Build tool for Reproducible Reporting
 Author-email: Toon Verstraelen <toon.verstraelen@ugent.be>
 License:                     GNU GENERAL PUBLIC LICENSE
                                Version 3, 29 June 2007
         
          Copyright (C) 2007 Free Software Foundation, Inc. <https://fsf.org/>
          Everyone is permitted to copy and distribute verbatim copies
```

### Comparing `RepRepBuild-0.8.0/README.md` & `RepRepBuild-0.9.0/README.md`

 * *Files identical despite different names*

### Comparing `RepRepBuild-0.8.0/pyproject.toml` & `RepRepBuild-0.9.0/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -56,13 +56,13 @@
 line-length = 100
 target-version = ['py310']
 
 [tool.ruff]
 select = ["E", "F", "UP", "B", "I", "PGH", "PL", "RUF"]
 line-length = 100
 target-version = "py310"
-ignore = ["PLR2004", "PLR0913", "PLR0912", "PLW2901", "PLR0915"]
+ignore = ["PLR2004", "PLR0913", "PLR0912", "PLW2901", "PLR0915", "PLC1901"]
 
 [tool.setuptools_scm]
 write_to = "src/reprepbuild/_version.py"
 version_scheme = "post-release"
 local_scheme = "no-local-version"
```

### Comparing `RepRepBuild-0.8.0/src/RepRepBuild.egg-info/PKG-INFO` & `RepRepBuild-0.9.0/src/RepRepBuild.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: RepRepBuild
-Version: 0.8.0
+Version: 0.9.0
 Summary: Build tool for Reproducible Reporting
 Author-email: Toon Verstraelen <toon.verstraelen@ugent.be>
 License:                     GNU GENERAL PUBLIC LICENSE
                                Version 3, 29 June 2007
         
          Copyright (C) 2007 Free Software Foundation, Inc. <https://fsf.org/>
          Everyone is permitted to copy and distribute verbatim copies
```

### Comparing `RepRepBuild-0.8.0/src/RepRepBuild.egg-info/SOURCES.txt` & `RepRepBuild-0.9.0/src/RepRepBuild.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `RepRepBuild-0.8.0/src/reprepbuild/__init__.py` & `RepRepBuild-0.9.0/src/reprepbuild/__init__.py`

 * *Files identical despite different names*

### Comparing `RepRepBuild-0.8.0/src/reprepbuild/__main__.py` & `RepRepBuild-0.9.0/src/reprepbuild/__main__.py`

 * *Files 7% similar despite different names*

```diff
@@ -62,15 +62,18 @@
     "copy": {"command": "cp $in $out"},
     "latexdiff": {"command": f"latexdiff --append-context2cmd={LATEXDIFF_CONTEXT2CMD} $in > $out"},
     "reprozip": {"command": "rr-zip $out $in"},
     "reproarticlezip": {"command": "rr-article-zip $out $in"},
     "svgtopdf": {
         "command": "inkscape $in --export-filename=$out --export-type=pdf; rr-normalize-pdf $out"
     },
-    "pythonscript": {"command": "rr-python-script $in -- $argstr > $out", "depfile": "$noext.d"},
+    "pythonscript": {
+        "command": "rr-python-script $in -- $argstr > $out",
+        "depfile": "$out_prefix.d",
+    },
 }
 
 
 def latex_pattern(path):
     """Make ninja build commands to compile latex with pdflatex."""
     result = re.match(r"latex-(?P<prefix>[a-z0-9-]+)/(?P=prefix).tex$", path)
     if not result:
@@ -162,24 +165,22 @@
             "inputs": fixpath(f"{prefix}-diff.pdf"),
             "default": True,
         }
 
 
 def dataset_pattern(path):
     """Make ninja build commands to ZIP datasets."""
-    result = re.match(r"dataset-(?P<name>[a-z][a-z0-9-]*)/README.md$", path)
+    result = re.match(r"(?P<name>dataset[a-z0-9-]*)/README.md$", path)
     if not result:
         return
     name = result.group("name")
     yield {
-        "outputs": f"uploads/dataset-{name}.zip",
+        "outputs": f"uploads/{name}.zip",
         "rule": "reprozip",
-        "inputs": [
-            path for path in glob(f"dataset-{name}/**", recursive=True) if not os.path.isdir(path)
-        ],
+        "inputs": [path for path in glob(f"{name}/**", recursive=True) if not os.path.isdir(path)],
         "pool": "console",
         "default": True,
     }
 
 
 def svg_pattern(path):
     """Make ninja build commands to convert SVG to PDF files."""
@@ -200,15 +201,15 @@
     # for any valid python file
     if not re.match(r"(?P<name>results(-[a-z0-9_-]*)?/[a-zA-Z0-9/_-]*).py$", path):
         return
 
     # Call reprepbuild_info as if the script is running in its own directory.
     orig_workdir = os.getcwd()
     workdir, fn_py = os.path.split(path)
-    prefix = fn_py[:-3]
+    script_prefix = fn_py[:-3]
     try:
         # Load the script in its own directory
         os.chdir(workdir)
         pythonscript = import_python_path(fn_py)
 
         # Ignore script if the import failed.
         if pythonscript is None:
@@ -229,27 +230,27 @@
         def fixpath(fn_local):
             return os.path.normpath(os.path.join(workdir, fn_local))
 
         # Loop over all cases to make build records
         for script_args in build_cases:
             build_info = reprepbuild_info(*script_args)
             argstr = format_case_args(script_args, case_fmt)
-            prefix_argstr = prefix if len(argstr) == 0 else f"{prefix}_{argstr}"
-            fn_log = fixpath(f"{prefix_argstr}.log")
+            out_prefix = fixpath(script_prefix if argstr == "" else argstr)
+            fn_log = f"{out_prefix}.log"
             implicit_inputs = [fixpath(ipath) for ipath in build_info.get("inputs", [])]
             implicit_outputs = [fixpath(opath) for opath in build_info.get("outputs", [])]
             yield {
                 "inputs": path,
                 "implicit": implicit_inputs,
                 "rule": "pythonscript",
                 "implicit_outputs": implicit_outputs,
                 "outputs": fn_log,
                 "variables": {
                     "argstr": argstr,
-                    "noext": fixpath(f"{prefix_argstr}"),
+                    "out_prefix": out_prefix,
                 },
                 "default": True,
             }
     finally:
         os.chdir(orig_workdir)
```

### Comparing `RepRepBuild-0.8.0/src/reprepbuild/articlezip.py` & `RepRepBuild-0.9.0/src/reprepbuild/articlezip.py`

 * *Files identical despite different names*

### Comparing `RepRepBuild-0.8.0/src/reprepbuild/bibtex.py` & `RepRepBuild-0.9.0/src/reprepbuild/bibtex.py`

 * *Files identical despite different names*

### Comparing `RepRepBuild-0.8.0/src/reprepbuild/latex.py` & `RepRepBuild-0.9.0/src/reprepbuild/latex.py`

 * *Files identical despite different names*

### Comparing `RepRepBuild-0.8.0/src/reprepbuild/latexdep.py` & `RepRepBuild-0.9.0/src/reprepbuild/latexdep.py`

 * *Files identical despite different names*

### Comparing `RepRepBuild-0.8.0/src/reprepbuild/normalizepdf.py` & `RepRepBuild-0.9.0/src/reprepbuild/normalizepdf.py`

 * *Files identical despite different names*

### Comparing `RepRepBuild-0.8.0/src/reprepbuild/pythonscript.py` & `RepRepBuild-0.9.0/src/reprepbuild/pythonscript.py`

 * *Files 11% similar despite different names*

```diff
@@ -51,15 +51,15 @@
 
 def run_script(path_py, argstr):
     """Run the python script and collected module dependencies."""
     if not path_py.endswith(".py"):
         print(f"Python script must have `.py` extension. Got {path_py}")
         return 2
     workdir, fn_py = os.path.split(path_py)
-    prefix = fn_py[:-3]
+    script_prefix = fn_py[:-3]
     orig_workdir = os.getcwd()
 
     # Check whether we're already in the eighties. (compatibility with ZIP)
     if os.environ.get("SOURCE_DATE_EPOCH") != "315532800":
         print("SOURCE_DATE_EPOCH is not set to 315532800.")
         return -3
 
@@ -97,17 +97,17 @@
         imported_paths.add(module_path)
 
     # Write the depfile.
     def fixpath(fn_local):
         return os.path.normpath(os.path.join(workdir, fn_local))
 
     # Note: only explicit outputs must be added to the depfile, not the implicit ones.
-    noext = fixpath(prefix if len(argstr) == 0 else f"{prefix}_{argstr}")
-    outputs = [(f"{noext}.log")]
-    path_dep = f"{noext}.d"
+    out_prefix = fixpath(script_prefix if argstr == "" else argstr)
+    outputs = [(f"{out_prefix}.log")]
+    path_dep = f"{out_prefix}.d"
     write_dep(path_dep, outputs, imported_paths)
 
     return result
 
 
 if __name__ == "__main__":
     main()
```

### Comparing `RepRepBuild-0.8.0/src/reprepbuild/repeat.py` & `RepRepBuild-0.9.0/src/reprepbuild/repeat.py`

 * *Files identical despite different names*

### Comparing `RepRepBuild-0.8.0/src/reprepbuild/utils.py` & `RepRepBuild-0.9.0/src/reprepbuild/utils.py`

 * *Files identical despite different names*

### Comparing `RepRepBuild-0.8.0/src/reprepbuild/zip.py` & `RepRepBuild-0.9.0/src/reprepbuild/zip.py`

 * *Files identical despite different names*

