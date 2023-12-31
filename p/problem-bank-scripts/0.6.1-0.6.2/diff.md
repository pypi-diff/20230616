# Comparing `tmp/problem_bank_scripts-0.6.1.tar.gz` & `tmp/problem_bank_scripts-0.6.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "problem_bank_scripts-0.6.1.tar", max compression
+gzip compressed data, was "problem_bank_scripts-0.6.2.tar", max compression
```

## Comparing `problem_bank_scripts-0.6.1.tar` & `problem_bank_scripts-0.6.2.tar`

### file list

```diff
@@ -1,11 +1,11 @@
--rwxr-xr-x   0        0        0        1 2021-05-16 14:07:02.985176 problem_bank_scripts-0.6.1/LICENSE
--rw-r--r--   0        0        0     1605 2023-06-15 01:42:11.784217 problem_bank_scripts-0.6.1/README.md
--rw-r--r--   0        0        0     1052 2023-06-15 17:32:46.057146 problem_bank_scripts-0.6.1/pyproject.toml
--rw-r--r--   0        0        0       59 2023-06-15 17:32:52.070048 problem_bank_scripts-0.6.1/src/problem_bank_scripts/__init__.py
--rw-r--r--   0        0        0     1757 2023-06-15 17:31:34.807559 problem_bank_scripts-0.6.1/src/problem_bank_scripts/attributions.json
--rw-r--r--   0        0        0    13476 2021-08-13 04:07:58.134898 problem_bank_scripts-0.6.1/src/problem_bank_scripts/prairielearn.py
--rw-r--r--   0        0        0    43049 2023-06-15 17:57:39.754420 problem_bank_scripts-0.6.1/src/problem_bank_scripts/problem_bank_scripts.py
--rw-r--r--   0        0        0      129 2022-06-24 05:48:29.289246 problem_bank_scripts-0.6.1/src/problem_bank_scripts/qti_export.py
--rw-r--r--   0        0        0    19225 2022-06-24 07:32:56.504377 problem_bank_scripts-0.6.1/src/problem_bank_scripts/webwork_to_md.py
--rw-r--r--   0        0        0     2647 2023-06-15 17:59:15.583256 problem_bank_scripts-0.6.1/setup.py
--rw-r--r--   0        0        0     2679 2023-06-15 17:59:15.583511 problem_bank_scripts-0.6.1/PKG-INFO
+-rwxr-xr-x   0        0        0        1 2021-05-16 14:07:02.985176 problem_bank_scripts-0.6.2/LICENSE
+-rw-r--r--   0        0        0     1605 2023-06-15 01:42:11.784217 problem_bank_scripts-0.6.2/README.md
+-rw-r--r--   0        0        0     1052 2023-06-16 02:56:32.963969 problem_bank_scripts-0.6.2/pyproject.toml
+-rw-r--r--   0        0        0       59 2023-06-16 02:56:39.428442 problem_bank_scripts-0.6.2/src/problem_bank_scripts/__init__.py
+-rw-r--r--   0        0        0     1757 2023-06-15 17:31:34.807559 problem_bank_scripts-0.6.2/src/problem_bank_scripts/attributions.json
+-rw-r--r--   0        0        0    13476 2021-08-13 04:07:58.134898 problem_bank_scripts-0.6.2/src/problem_bank_scripts/prairielearn.py
+-rw-r--r--   0        0        0    42101 2023-06-16 02:55:43.161647 problem_bank_scripts-0.6.2/src/problem_bank_scripts/problem_bank_scripts.py
+-rw-r--r--   0        0        0      129 2022-06-24 05:48:29.289246 problem_bank_scripts-0.6.2/src/problem_bank_scripts/qti_export.py
+-rw-r--r--   0        0        0    19225 2022-06-24 07:32:56.504377 problem_bank_scripts-0.6.2/src/problem_bank_scripts/webwork_to_md.py
+-rw-r--r--   0        0        0     2647 2023-06-16 02:56:59.648513 problem_bank_scripts-0.6.2/setup.py
+-rw-r--r--   0        0        0     2679 2023-06-16 02:56:59.648759 problem_bank_scripts-0.6.2/PKG-INFO
```

### Comparing `problem_bank_scripts-0.6.1/README.md` & `problem_bank_scripts-0.6.2/README.md`

 * *Files identical despite different names*

### Comparing `problem_bank_scripts-0.6.1/pyproject.toml` & `problem_bank_scripts-0.6.2/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "problem_bank_scripts"
-version = "0.6.1"
+version = "0.6.2"
 description = "A package with useful functions to convert between different problem bank formats."
 authors = ["Open Problem Bank Team"]
 license = "MIT"
 readme = "README.md"
 documentation = "https://problem_bank_scripts.readthedocs.io/en/latest/"
 homepage = "https://github.com/open-resources/problem_bank_scripts"
 repository = "https://github.com/open-resources/problem_bank_scripts"
```

### Comparing `problem_bank_scripts-0.6.1/src/problem_bank_scripts/attributions.json` & `problem_bank_scripts-0.6.2/src/problem_bank_scripts/attributions.json`

 * *Files identical despite different names*

### Comparing `problem_bank_scripts-0.6.1/src/problem_bank_scripts/prairielearn.py` & `problem_bank_scripts-0.6.2/src/problem_bank_scripts/prairielearn.py`

 * *Files identical despite different names*

### Comparing `problem_bank_scripts-0.6.1/src/problem_bank_scripts/problem_bank_scripts.py` & `problem_bank_scripts-0.6.2/src/problem_bank_scripts/problem_bank_scripts.py`

 * *Files 2% similar despite different names*

```diff
@@ -412,29 +412,24 @@
     """
     Args:
         output_path (Path): [description]
         parsed_question (dict]): [description]
     """
 
     # Deal with optional tags in info.json
-    optional = ""
+    # optional = ""
 
-    if parsed_question["header"].get("gradingMethod"):
-        optional += """\"gradingMethod": \"""" + parsed_question['header']['gradingMethod'] + """\",\n\t\t"""
-    if parsed_question["header"].get("partialCredit"):
-        optional += """\"partialCredit":""" + str(parsed_question['header']['partialCredit']).lower() + """,\n\t\t"""
-    if parsed_question["header"].get("dependencies"):
-        optional += """\"dependencies": """ + parsed_question['header']['dependencies'] + """,\n\t\t"""
-    if parsed_question["header"].get("singleVariant"):
-        optional += """\"singleVariant": """ + str(parsed_question['header']['singleVariant']).lower() + """,\n\t\t"""
-    if parsed_question["header"].get("showCorrectAnswer"):
-        optional += """\"showCorrectAnswer": """ + str(parsed_question['header']['showCorrectAnswer']).lower() + """,\n\t\t"""
-    if parsed_question["header"].get("externalGradingOptions"):
-        optional += """\"externalGradingOptions": """ + json.dumps(parsed_question['header']['externalGradingOptions']) + """,\n\t\t"""
-    optional = optional[:-4] + """\n"""
+    optional_keys = {
+        "gradingMethod",
+        "partialCredit",
+        "dependencies",
+        "singleVariant",
+        "showCorrectAnswer",
+        "externalGradingOptions",
+    }
 
     # Add tags based on part type
     q_types = []
 
     for pnum in range(1, parsed_question["num_parts"] + 1):
         part = "part" + f"{pnum}"
         q_types.append(parsed_question["header"][part]["type"])
@@ -443,38 +438,32 @@
     if len(q_types) > 1:
         auto_tags.append("multi_part")
     auto_tags.extend(list(set(q_types)))
 
     auto_tags.extend(parsed_question["header"]["tags"])
     auto_tags = [v for v in auto_tags if v != "unknown"]
 
-    # End add tags
-
-    pathlib.Path(output_path / "info.json").write_text(
-        """{
-            "uuid": \""""
-        + str(uuid.uuid3(uuid.NAMESPACE_DNS, str(output_path)))
-        + """\",
-            "title": \""""
-        + parsed_question["header"]["title"]
-        + """\",
-            "topic": \""""
-        + parsed_question["header"]["topic"]
-        + """\",
-            "tags":  """
-        + json.dumps(auto_tags)
-        + """,
-            "type": "v3\""""
-        + ((""",
-            """
-        + optional) if (optional) else ("""\n"""))
-        + """}""",
-        encoding="utf8",
+    info_json = {
+        "uuid": str(uuid.uuid3(uuid.NAMESPACE_DNS, str(output_path))),
+        "title": parsed_question["header"]["title"],
+        "topic": parsed_question["header"]["topic"],
+        "tags": auto_tags,
+        "type": "v3",
+    }
+    info_json.update(
+        {
+            key: parsed_question["header"][key]
+            for key in parsed_question["header"].keys() & optional_keys
+        }
     )
 
+    # End add tags
+    with pathlib.Path(output_path / "info.json").open("w") as output_file:
+        json.dump(info_json, output_file, indent=4)
+
 
 def assemble_server_py(parsed_question, location):
     """Assembles a string version of the server.py file from the YAML header of the md file.
 
     Args:
         parsed_question (_type_): dictionary that is created upon reading of the md problem.
         location (string): 'local' or 'prairielearn' ; the import statements are different depending on if it's local or on a PL server.
```

### Comparing `problem_bank_scripts-0.6.1/src/problem_bank_scripts/webwork_to_md.py` & `problem_bank_scripts-0.6.2/src/problem_bank_scripts/webwork_to_md.py`

 * *Files identical despite different names*

### Comparing `problem_bank_scripts-0.6.1/setup.py` & `problem_bank_scripts-0.6.2/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -18,15 +18,15 @@
  'numpy>=1.22,<2.0',
  'pandas>=1.2.4,<2.0.0',
  'problem-bank-helpers>=0.1.12,<0.2.0',
  'sympy>=1.8,<2.0']
 
 setup_kwargs = {
     'name': 'problem-bank-scripts',
-    'version': '0.6.1',
+    'version': '0.6.2',
     'description': 'A package with useful functions to convert between different problem bank formats.',
     'long_description': '# Problem Bank Scripts \n\n[![Python](https://img.shields.io/badge/python-3.9-blue)]()\n[![codecov](https://codecov.io/gh/open-resources/problem_bank_scripts/branch/main/graph/badge.svg)](https://codecov.io/gh/open-resources/problem_bank_scripts)\n[![Documentation Status](https://readthedocs.org/projects/problem_bank_scripts/badge/?version=latest)](https://problem_bank_scripts.readthedocs.io/en/latest/?badge=latest)\n\n\n## Installation\n\n```bash\n$ pip install -i https://test.pypi.org/simple/ problem_bank_scripts\n```\n\n## Update version\n\nHere are the steps to increment the version (replace patch with major/minor/patch)\n\n```\npoetry version patch\n\npico src/problem_bank_scripts/__init__.py\n\npico tests/test_problem_bank_scripts.py\n\npoetry run pytest\n\ncd docs; poetry run make html; cd ..\n\ngit add .; git commit -m "increment version"; git push\n\npoetry build\n\npoetry publish\n```\n\n\n## Features\n\n- TODO\n\n## Dependencies\n\n- TODO\n\n## Usage\n\n- TODO\n\n## Documentation\n\nThe official documentation is hosted on Read the Docs: https://problem_bank_scripts.readthedocs.io/en/latest/\n\n## Contributors\n\nWe welcome and recognize all contributions. You can see a list of current contributors in the [contributors tab](https://github.com/open-resources/problem_bank_scripts/graphs/contributors).\n\n### Credits\n\nThis package was created with Cookiecutter and the UBC-MDS/cookiecutter-ubc-mds project template, modified from the [pyOpenSci/cookiecutter-pyopensci](https://github.com/pyOpenSci/cookiecutter-pyopensci) project template and the [audreyr/cookiecutter-pypackage](https://github.com/audreyr/cookiecutter-pypackage).\n',
     'author': 'Open Problem Bank Team',
     'author_email': None,
     'maintainer': None,
     'maintainer_email': None,
     'url': 'https://github.com/open-resources/problem_bank_scripts',
```

### Comparing `problem_bank_scripts-0.6.1/PKG-INFO` & `problem_bank_scripts-0.6.2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: problem-bank-scripts
-Version: 0.6.1
+Version: 0.6.2
 Summary: A package with useful functions to convert between different problem bank formats.
 Home-page: https://github.com/open-resources/problem_bank_scripts
 License: MIT
 Author: Open Problem Bank Team
 Requires-Python: >=3.8,<4.0
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
```

