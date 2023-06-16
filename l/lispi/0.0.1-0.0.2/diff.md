# Comparing `tmp/lispi-0.0.1.tar.gz` & `tmp/lispi-0.0.2.tar.gz`

## Comparing `lispi-0.0.1.tar` & `lispi-0.0.2.tar`

### file list

```diff
@@ -1,20 +1,20 @@
--rw-r--r--   0        0        0     6148 2020-02-02 00:00:00.000000 lispi-0.0.1/.DS_Store
--rw-r--r--   0        0        0       32 2020-02-02 00:00:00.000000 lispi-0.0.1/MANIFEST.in
--rw-r--r--   0        0        0     6461 2020-02-02 00:00:00.000000 lispi-0.0.1/requirements.txt
--rw-r--r--   0        0        0     6148 2020-02-02 00:00:00.000000 lispi-0.0.1/example/.DS_Store
--rw-r--r--   0        0        0    11232 2020-02-02 00:00:00.000000 lispi-0.0.1/example/original_example.ipynb
--rw-r--r--   0        0        0     8196 2020-02-02 00:00:00.000000 lispi-0.0.1/src/.DS_Store
--rw-r--r--   0        0        0     6148 2020-02-02 00:00:00.000000 lispi-0.0.1/src/lispy/.DS_Store
--rw-r--r--   0        0        0      228 2020-02-02 00:00:00.000000 lispi-0.0.1/src/lispy/__init__.py
--rw-r--r--   0        0        0     2311 2020-02-02 00:00:00.000000 lispi-0.0.1/src/lispy/__main__.py
--rw-r--r--   0        0        0      489 2020-02-02 00:00:00.000000 lispi-0.0.1/src/lispy/revealjs_template.py
--rw-r--r--   0        0        0     4420 2020-02-02 00:00:00.000000 lispi-0.0.1/src/lispy/slideEdit.py
--rw-r--r--   0        0        0     1746 2020-02-02 00:00:00.000000 lispi-0.0.1/src/lispy/text2audio.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 lispi-0.0.1/tests/test_audioText.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 lispi-0.0.1/tests/test_nbconvert.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 lispi-0.0.1/tests/test_pyscript.py
--rw-r--r--   0        0        0        6 2020-02-02 00:00:00.000000 lispi-0.0.1/.gitignore
--rw-r--r--   0        0        0     1073 2020-02-02 00:00:00.000000 lispi-0.0.1/LICENSE
--rw-r--r--   0        0        0     2221 2020-02-02 00:00:00.000000 lispi-0.0.1/README.md
--rw-r--r--   0        0        0     1236 2020-02-02 00:00:00.000000 lispi-0.0.1/pyproject.toml
--rw-r--r--   0        0        0     4163 2020-02-02 00:00:00.000000 lispi-0.0.1/PKG-INFO
+-rw-r--r--   0        0        0     6148 2020-02-02 00:00:00.000000 lispi-0.0.2/.DS_Store
+-rw-r--r--   0        0        0       32 2020-02-02 00:00:00.000000 lispi-0.0.2/MANIFEST.in
+-rw-r--r--   0        0        0     6461 2020-02-02 00:00:00.000000 lispi-0.0.2/requirements.txt
+-rw-r--r--   0        0        0     6148 2020-02-02 00:00:00.000000 lispi-0.0.2/example/.DS_Store
+-rw-r--r--   0        0        0    11232 2020-02-02 00:00:00.000000 lispi-0.0.2/example/original_example.ipynb
+-rw-r--r--   0        0        0     8196 2020-02-02 00:00:00.000000 lispi-0.0.2/src/.DS_Store
+-rw-r--r--   0        0        0     6148 2020-02-02 00:00:00.000000 lispi-0.0.2/src/lispy/.DS_Store
+-rw-r--r--   0        0        0      228 2020-02-02 00:00:00.000000 lispi-0.0.2/src/lispy/__init__.py
+-rw-r--r--   0        0        0     2311 2020-02-02 00:00:00.000000 lispi-0.0.2/src/lispy/__main__.py
+-rw-r--r--   0        0        0      489 2020-02-02 00:00:00.000000 lispi-0.0.2/src/lispy/revealjs_template.py
+-rw-r--r--   0        0        0     4420 2020-02-02 00:00:00.000000 lispi-0.0.2/src/lispy/slideEdit.py
+-rw-r--r--   0        0        0     1746 2020-02-02 00:00:00.000000 lispi-0.0.2/src/lispy/text2audio.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 lispi-0.0.2/tests/test_audioText.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 lispi-0.0.2/tests/test_nbconvert.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 lispi-0.0.2/tests/test_pyscript.py
+-rw-r--r--   0        0        0        6 2020-02-02 00:00:00.000000 lispi-0.0.2/.gitignore
+-rw-r--r--   0        0        0     1073 2020-02-02 00:00:00.000000 lispi-0.0.2/LICENSE
+-rw-r--r--   0        0        0     2221 2020-02-02 00:00:00.000000 lispi-0.0.2/README.md
+-rw-r--r--   0        0        0     1236 2020-02-02 00:00:00.000000 lispi-0.0.2/pyproject.toml
+-rw-r--r--   0        0        0     4163 2020-02-02 00:00:00.000000 lispi-0.0.2/PKG-INFO
```

### Comparing `lispi-0.0.1/.DS_Store` & `lispi-0.0.2/.DS_Store`

 * *Files identical despite different names*

### Comparing `lispi-0.0.1/requirements.txt` & `lispi-0.0.2/requirements.txt`

 * *Files identical despite different names*

### Comparing `lispi-0.0.1/example/.DS_Store` & `lispi-0.0.2/example/.DS_Store`

 * *Files identical despite different names*

### Comparing `lispi-0.0.1/example/original_example.ipynb` & `lispi-0.0.2/example/original_example.ipynb`

 * *Files identical despite different names*

### Comparing `lispi-0.0.1/src/.DS_Store` & `lispi-0.0.2/src/.DS_Store`

 * *Files identical despite different names*

### Comparing `lispi-0.0.1/src/lispy/.DS_Store` & `lispi-0.0.2/src/lispy/.DS_Store`

 * *Files identical despite different names*

### Comparing `lispi-0.0.1/src/lispy/__main__.py` & `lispi-0.0.2/src/lispy/__main__.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 import os
 import subprocess
 import jupyter
 import shutil
-import lispy
-from lispy import text2audio, slideEdit, revealjs_template
+import lispi
+from lispi import text2audio, slideEdit, revealjs_template
 
 def main():
     index = input("Enter the name of the notebook file: \n")
     if os.path.isfile(index+".ipynb"):
         text2audio.text2audio(index+".ipynb")
         revealjs_template.convert('nbconvert')
         subprocess.run(["jupyter", "nbconvert", index+".ipynb", "--to", "slides"])
```

### Comparing `lispi-0.0.1/src/lispy/slideEdit.py` & `lispi-0.0.2/src/lispy/slideEdit.py`

 * *Files identical despite different names*

### Comparing `lispi-0.0.1/src/lispy/text2audio.py` & `lispi-0.0.2/src/lispy/text2audio.py`

 * *Files identical despite different names*

### Comparing `lispi-0.0.1/LICENSE` & `lispi-0.0.2/LICENSE`

 * *Files identical despite different names*

### Comparing `lispi-0.0.1/README.md` & `lispi-0.0.2/README.md`

 * *Files identical despite different names*

### Comparing `lispi-0.0.1/pyproject.toml` & `lispi-0.0.2/pyproject.toml`

 * *Files 18% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 build-backend = "hatchling.build"
 
 [tool.hatch.include]
 include = [".example/**"]
 
 [project]
 name = "lispi"
-version = "0.0.01"
+version = "0.0.02"
 authors = [
   { name="B7M", email="ibsnetwork001@gmail.com" },
 ]
 license = { file = "LICENSE" }
 description = "A simple python package for generating live notebooks where you can write code and run it in real time."
 readme = "README.md"
 requires-python = ">=3.7"
@@ -38,15 +38,15 @@
 Homepage = "https://github.com/B7M/lispi"
 
 [project.scripts]
 lispi = "lispi.__main__:main"
 
 
 [tool.bumpver]
-current_version = "0.0.01"
+current_version = "0.0.02"
 version_pattern = "MAJOR.MINOR.PATCH"
 commit_message = "bump version {old_version} -> {new_version}"
 commit = true
 tag = true
 push = true
 
 [tool.bumpver.file_patterns]
```

### Comparing `lispi-0.0.1/PKG-INFO` & `lispi-0.0.2/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: lispi
-Version: 0.0.1
+Version: 0.0.2
 Summary: A simple python package for generating live notebooks where you can write code and run it in real time.
 Project-URL: Homepage, https://github.com/B7M/lispi
 Author-email: B7M <ibsnetwork001@gmail.com>
 License: Copyright (c) 2023 The Python Packaging Authority
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
         of this software and associated documentation files (the "Software"), to deal
```

