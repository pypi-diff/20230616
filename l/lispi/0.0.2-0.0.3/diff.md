# Comparing `tmp/lispi-0.0.2.tar.gz` & `tmp/lispi-0.0.3.tar.gz`

## Comparing `lispi-0.0.2.tar` & `lispi-0.0.3.tar`

### file list

```diff
@@ -1,20 +1,20 @@
--rw-r--r--   0        0        0     6148 2020-02-02 00:00:00.000000 lispi-0.0.2/.DS_Store
--rw-r--r--   0        0        0       32 2020-02-02 00:00:00.000000 lispi-0.0.2/MANIFEST.in
--rw-r--r--   0        0        0     6461 2020-02-02 00:00:00.000000 lispi-0.0.2/requirements.txt
--rw-r--r--   0        0        0     6148 2020-02-02 00:00:00.000000 lispi-0.0.2/example/.DS_Store
--rw-r--r--   0        0        0    11232 2020-02-02 00:00:00.000000 lispi-0.0.2/example/original_example.ipynb
--rw-r--r--   0        0        0     8196 2020-02-02 00:00:00.000000 lispi-0.0.2/src/.DS_Store
--rw-r--r--   0        0        0     6148 2020-02-02 00:00:00.000000 lispi-0.0.2/src/lispy/.DS_Store
--rw-r--r--   0        0        0      228 2020-02-02 00:00:00.000000 lispi-0.0.2/src/lispy/__init__.py
--rw-r--r--   0        0        0     2311 2020-02-02 00:00:00.000000 lispi-0.0.2/src/lispy/__main__.py
--rw-r--r--   0        0        0      489 2020-02-02 00:00:00.000000 lispi-0.0.2/src/lispy/revealjs_template.py
--rw-r--r--   0        0        0     4420 2020-02-02 00:00:00.000000 lispi-0.0.2/src/lispy/slideEdit.py
--rw-r--r--   0        0        0     1746 2020-02-02 00:00:00.000000 lispi-0.0.2/src/lispy/text2audio.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 lispi-0.0.2/tests/test_audioText.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 lispi-0.0.2/tests/test_nbconvert.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 lispi-0.0.2/tests/test_pyscript.py
--rw-r--r--   0        0        0        6 2020-02-02 00:00:00.000000 lispi-0.0.2/.gitignore
--rw-r--r--   0        0        0     1073 2020-02-02 00:00:00.000000 lispi-0.0.2/LICENSE
--rw-r--r--   0        0        0     2221 2020-02-02 00:00:00.000000 lispi-0.0.2/README.md
--rw-r--r--   0        0        0     1236 2020-02-02 00:00:00.000000 lispi-0.0.2/pyproject.toml
--rw-r--r--   0        0        0     4163 2020-02-02 00:00:00.000000 lispi-0.0.2/PKG-INFO
+-rw-r--r--   0        0        0     6148 2020-02-02 00:00:00.000000 lispi-0.0.3/.DS_Store
+-rw-r--r--   0        0        0       32 2020-02-02 00:00:00.000000 lispi-0.0.3/MANIFEST.in
+-rw-r--r--   0        0        0     6461 2020-02-02 00:00:00.000000 lispi-0.0.3/requirements.txt
+-rw-r--r--   0        0        0     6148 2020-02-02 00:00:00.000000 lispi-0.0.3/example/.DS_Store
+-rw-r--r--   0        0        0    11232 2020-02-02 00:00:00.000000 lispi-0.0.3/example/original_example.ipynb
+-rw-r--r--   0        0        0     8196 2020-02-02 00:00:00.000000 lispi-0.0.3/src/.DS_Store
+-rw-r--r--   0        0        0     6148 2020-02-02 00:00:00.000000 lispi-0.0.3/src/lispi/.DS_Store
+-rw-r--r--   0        0        0      146 2020-02-02 00:00:00.000000 lispi-0.0.3/src/lispi/__init__.py
+-rw-r--r--   0        0        0     2311 2020-02-02 00:00:00.000000 lispi-0.0.3/src/lispi/__main__.py
+-rw-r--r--   0        0        0      489 2020-02-02 00:00:00.000000 lispi-0.0.3/src/lispi/revealjs_template.py
+-rw-r--r--   0        0        0     4420 2020-02-02 00:00:00.000000 lispi-0.0.3/src/lispi/slideEdit.py
+-rw-r--r--   0        0        0     1746 2020-02-02 00:00:00.000000 lispi-0.0.3/src/lispi/text2audio.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 lispi-0.0.3/tests/test_audioText.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 lispi-0.0.3/tests/test_nbconvert.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 lispi-0.0.3/tests/test_pyscript.py
+-rw-r--r--   0        0        0        6 2020-02-02 00:00:00.000000 lispi-0.0.3/.gitignore
+-rw-r--r--   0        0        0     1073 2020-02-02 00:00:00.000000 lispi-0.0.3/LICENSE
+-rw-r--r--   0        0        0     2255 2020-02-02 00:00:00.000000 lispi-0.0.3/README.md
+-rw-r--r--   0        0        0     1236 2020-02-02 00:00:00.000000 lispi-0.0.3/pyproject.toml
+-rw-r--r--   0        0        0     4197 2020-02-02 00:00:00.000000 lispi-0.0.3/PKG-INFO
```

### Comparing `lispi-0.0.2/.DS_Store` & `lispi-0.0.3/.DS_Store`

 * *Files identical despite different names*

### Comparing `lispi-0.0.2/requirements.txt` & `lispi-0.0.3/requirements.txt`

 * *Files identical despite different names*

### Comparing `lispi-0.0.2/example/.DS_Store` & `lispi-0.0.3/example/.DS_Store`

 * *Files identical despite different names*

### Comparing `lispi-0.0.2/example/original_example.ipynb` & `lispi-0.0.3/example/original_example.ipynb`

 * *Files identical despite different names*

### Comparing `lispi-0.0.2/src/.DS_Store` & `lispi-0.0.3/src/.DS_Store`

 * *Files identical despite different names*

### Comparing `lispi-0.0.2/src/lispy/.DS_Store` & `lispi-0.0.3/src/lispi/.DS_Store`

 * *Files identical despite different names*

### Comparing `lispi-0.0.2/src/lispy/__main__.py` & `lispi-0.0.3/src/lispi/__main__.py`

 * *Files identical despite different names*

### Comparing `lispi-0.0.2/src/lispy/slideEdit.py` & `lispi-0.0.3/src/lispi/slideEdit.py`

 * *Files identical despite different names*

### Comparing `lispi-0.0.2/src/lispy/text2audio.py` & `lispi-0.0.3/src/lispi/text2audio.py`

 * *Files identical despite different names*

### Comparing `lispi-0.0.2/LICENSE` & `lispi-0.0.3/LICENSE`

 * *Files identical despite different names*

### Comparing `lispi-0.0.2/README.md` & `lispi-0.0.3/README.md`

 * *Files 22% similar despite different names*

```diff
@@ -1,35 +1,35 @@
-# ESS Documentation
+# Lispi Documentation
 
 ## Introduction
 
-ESS (Educational Slide Studio) is a Python package that provides a convenient way to convert Jupyter notebooks into interactive slides. It allows users to create engaging presentations with interactive elements directly from the slides.
+Lispi (Educational Slide Studio) is a Python package that provides a convenient way to convert Jupyter notebooks into interactive slides. It allows users to create engaging presentations with interactive elements directly from the slides.
 
 ## Installation
 
-To install `ess` package, you can use pip, the Python package installer. Open your terminal and run the following command:
+To install `lispi` package, you can use pip, the Python package installer. Open your terminal and run the following command:
 
 ```
-pip install ess
+pip install lispi
 ```
 
 ## Usage
 
-To use ess, follow these steps:
+To use lispi, follow these steps:
 
-1. Import the `ess` class from the package:
+1. Import the `lispi` class from the package:
 
    ```python
-    import ess
+    import lispi
    ```
 
 2. Create an instance of the `InteractiveSlidesGenerator` class:
 
    ```python
-   generator = ess()
+   generator = lispi()
    ```
 
 3. Specify the Jupyter notebook file you want to convert:
 
    ```python
    notebook_file = "path/to/your/notebook.ipynb"
    ```
@@ -40,41 +40,41 @@
    generator.generate_slides(notebook_file)
    ```
 
 5. The package will convert the Jupyter notebook into interactive slides and save the output HTML file.
 
 ## Configuration
 
-Ess provides several configuration options to customize the output slides. You can pass these options as arguments when creating an instance of the `ess` class. Here are the available configuration options:
+Lispi provides several configuration options to customize the output slides. You can pass these options as arguments when creating an instance of the `lispi` class. Here are the available configuration options:
 
 - `audio`: Specify if you wish the output without audio (default: "unmute").
 - `output_file`: Specify the output file path for the generated slides (default: "output.html").
 
 Example:
 
 ```python
-generator = ess(
+generator = lispi(
     audio="unmute",
     output_file="path/to/output/slides.html"
 )
 ```
 
 ## Examples
 
-Here are a few examples demonstrating the usage of `ess`:
+Here are a few examples demonstrating the usage of `lispi`:
 
 ```python
-from ess import ess
+from lispi import lispi
 
-# Create an instance of the ess class
-generator = ess()
+# Create an instance of the lispi class
+generator = lispi()
 
 # Specify the Jupyter notebook file
 notebook_file = "path/to/your/notebook.ipynb"
 
 # Generate the interactive slides
 generator.generate_slides(notebook_file)
 ```
 
 ## Conclusion
 
-Ess package provides a convenient way to convert Jupyter notebooks into interactive slides. It allows users to create engaging presentations with interactive elements easily. By following the installation and usage instructions outlined in this documentation, you can leverage this package to generate interactive slides from your Jupyter notebooks effortlessly.
+Lispi package provides a convenient way to convert Jupyter notebooks into interactive slides. It allows users to create engaging presentations with interactive elements easily. By following the installation and usage instructions outlined in this documentation, you can leverage this package to generate interactive slides from your Jupyter notebooks effortlessly.
```

### Comparing `lispi-0.0.2/pyproject.toml` & `lispi-0.0.3/pyproject.toml`

 * *Files 7% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 build-backend = "hatchling.build"
 
 [tool.hatch.include]
 include = [".example/**"]
 
 [project]
 name = "lispi"
-version = "0.0.02"
+version = "0.0.03"
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
-current_version = "0.0.02"
+current_version = "0.0.03"
 version_pattern = "MAJOR.MINOR.PATCH"
 commit_message = "bump version {old_version} -> {new_version}"
 commit = true
 tag = true
 push = true
 
 [tool.bumpver.file_patterns]
```

### Comparing `lispi-0.0.2/PKG-INFO` & `lispi-0.0.3/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: lispi
-Version: 0.0.2
+Version: 0.0.3
 Summary: A simple python package for generating live notebooks where you can write code and run it in real time.
 Project-URL: Homepage, https://github.com/B7M/lispi
 Author-email: B7M <ibsnetwork001@gmail.com>
 License: Copyright (c) 2023 The Python Packaging Authority
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
         of this software and associated documentation files (the "Software"), to deal
@@ -34,42 +34,42 @@
 Requires-Dist: jupyter
 Requires-Dist: jupyterlab
 Requires-Dist: nbconvert
 Requires-Dist: nbformat
 Requires-Dist: tomli; python_version < '3.11'
 Description-Content-Type: text/markdown
 
-# ESS Documentation
+# Lispi Documentation
 
 ## Introduction
 
-ESS (Educational Slide Studio) is a Python package that provides a convenient way to convert Jupyter notebooks into interactive slides. It allows users to create engaging presentations with interactive elements directly from the slides.
+Lispi (Educational Slide Studio) is a Python package that provides a convenient way to convert Jupyter notebooks into interactive slides. It allows users to create engaging presentations with interactive elements directly from the slides.
 
 ## Installation
 
-To install `ess` package, you can use pip, the Python package installer. Open your terminal and run the following command:
+To install `lispi` package, you can use pip, the Python package installer. Open your terminal and run the following command:
 
 ```
-pip install ess
+pip install lispi
 ```
 
 ## Usage
 
-To use ess, follow these steps:
+To use lispi, follow these steps:
 
-1. Import the `ess` class from the package:
+1. Import the `lispi` class from the package:
 
    ```python
-    import ess
+    import lispi
    ```
 
 2. Create an instance of the `InteractiveSlidesGenerator` class:
 
    ```python
-   generator = ess()
+   generator = lispi()
    ```
 
 3. Specify the Jupyter notebook file you want to convert:
 
    ```python
    notebook_file = "path/to/your/notebook.ipynb"
    ```
@@ -80,41 +80,41 @@
    generator.generate_slides(notebook_file)
    ```
 
 5. The package will convert the Jupyter notebook into interactive slides and save the output HTML file.
 
 ## Configuration
 
-Ess provides several configuration options to customize the output slides. You can pass these options as arguments when creating an instance of the `ess` class. Here are the available configuration options:
+Lispi provides several configuration options to customize the output slides. You can pass these options as arguments when creating an instance of the `lispi` class. Here are the available configuration options:
 
 - `audio`: Specify if you wish the output without audio (default: "unmute").
 - `output_file`: Specify the output file path for the generated slides (default: "output.html").
 
 Example:
 
 ```python
-generator = ess(
+generator = lispi(
     audio="unmute",
     output_file="path/to/output/slides.html"
 )
 ```
 
 ## Examples
 
-Here are a few examples demonstrating the usage of `ess`:
+Here are a few examples demonstrating the usage of `lispi`:
 
 ```python
-from ess import ess
+from lispi import lispi
 
-# Create an instance of the ess class
-generator = ess()
+# Create an instance of the lispi class
+generator = lispi()
 
 # Specify the Jupyter notebook file
 notebook_file = "path/to/your/notebook.ipynb"
 
 # Generate the interactive slides
 generator.generate_slides(notebook_file)
 ```
 
 ## Conclusion
 
-Ess package provides a convenient way to convert Jupyter notebooks into interactive slides. It allows users to create engaging presentations with interactive elements easily. By following the installation and usage instructions outlined in this documentation, you can leverage this package to generate interactive slides from your Jupyter notebooks effortlessly.
+Lispi package provides a convenient way to convert Jupyter notebooks into interactive slides. It allows users to create engaging presentations with interactive elements easily. By following the installation and usage instructions outlined in this documentation, you can leverage this package to generate interactive slides from your Jupyter notebooks effortlessly.
```

