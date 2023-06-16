# Comparing `tmp/expert_intelligence_toolbox-0.0.4.tar.gz` & `tmp/expert_intelligence_toolbox-0.0.5.tar.gz`

## Comparing `expert_intelligence_toolbox-0.0.4.tar` & `expert_intelligence_toolbox-0.0.5.tar`

### file list

```diff
@@ -1,7 +1,9 @@
--rw-r--r--   0        0        0        6 2020-02-02 00:00:00.000000 expert_intelligence_toolbox-0.0.4/requirements.txt
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 expert_intelligence_toolbox-0.0.4/src/expert_intelligence_toolbox/__init__.py
--rw-r--r--   0        0        0       70 2020-02-02 00:00:00.000000 expert_intelligence_toolbox-0.0.4/src/expert_intelligence_toolbox/example.py
--rw-r--r--   0        0        0     1089 2020-02-02 00:00:00.000000 expert_intelligence_toolbox-0.0.4/LICENSE
--rw-r--r--   0        0        0     2576 2020-02-02 00:00:00.000000 expert_intelligence_toolbox-0.0.4/README.md
--rw-r--r--   0        0        0      671 2020-02-02 00:00:00.000000 expert_intelligence_toolbox-0.0.4/pyproject.toml
--rw-r--r--   0        0        0     3117 2020-02-02 00:00:00.000000 expert_intelligence_toolbox-0.0.4/PKG-INFO
+-rw-r--r--   0        0        0      102 2020-02-02 00:00:00.000000 expert_intelligence_toolbox-0.0.5/requirements.txt
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 expert_intelligence_toolbox-0.0.5/src/expert_intelligence_toolbox/__init__.py
+-rw-r--r--   0        0        0       64 2020-02-02 00:00:00.000000 expert_intelligence_toolbox-0.0.5/src/expert_intelligence_toolbox/example.py
+-rw-r--r--   0        0        0     2669 2020-02-02 00:00:00.000000 expert_intelligence_toolbox-0.0.5/src/expert_intelligence_toolbox/snowflake_connector.py
+-rw-r--r--   0        0        0       13 2020-02-02 00:00:00.000000 expert_intelligence_toolbox-0.0.5/.gitignore
+-rw-r--r--   0        0        0     1068 2020-02-02 00:00:00.000000 expert_intelligence_toolbox-0.0.5/LICENSE
+-rw-r--r--   0        0        0     2527 2020-02-02 00:00:00.000000 expert_intelligence_toolbox-0.0.5/README.md
+-rw-r--r--   0        0        0      650 2020-02-02 00:00:00.000000 expert_intelligence_toolbox-0.0.5/pyproject.toml
+-rw-r--r--   0        0        0     3117 2020-02-02 00:00:00.000000 expert_intelligence_toolbox-0.0.5/PKG-INFO
```

### Comparing `expert_intelligence_toolbox-0.0.4/LICENSE` & `expert_intelligence_toolbox-0.0.5/LICENSE`

 * *Ordering differences only*

 * *Files 12% similar despite different names*

```diff
@@ -1,21 +1,21 @@
-MIT License
-
-Copyright (c) 2023 Point-Topic
-
-Permission is hereby granted, free of charge, to any person obtaining a copy
-of this software and associated documentation files (the "Software"), to deal
-in the Software without restriction, including without limitation the rights
-to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
-copies of the Software, and to permit persons to whom the Software is
-furnished to do so, subject to the following conditions:
-
-The above copyright notice and this permission notice shall be included in all
-copies or substantial portions of the Software.
-
-THE SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF ANY KIND, EXPRESS OR
-IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY,
-FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE
-AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER
-LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,
-OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE
-SOFTWARE.
+MIT License
+
+Copyright (c) 2023 Point-Topic
+
+Permission is hereby granted, free of charge, to any person obtaining a copy
+of this software and associated documentation files (the "Software"), to deal
+in the Software without restriction, including without limitation the rights
+to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
+copies of the Software, and to permit persons to whom the Software is
+furnished to do so, subject to the following conditions:
+
+The above copyright notice and this permission notice shall be included in all
+copies or substantial portions of the Software.
+
+THE SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF ANY KIND, EXPRESS OR
+IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY,
+FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE
+AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER
+LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,
+OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE
+SOFTWARE.
```

### Comparing `expert_intelligence_toolbox-0.0.4/README.md` & `expert_intelligence_toolbox-0.0.5/README.md`

 * *Ordering differences only*

 * *Files 12% similar despite different names*

```diff
@@ -1,50 +1,50 @@
-# expert_intelligence_toolbox
-This is an experimental v0.1, which currently serves no function other than testing.
-Hello update.
-
-## Internal:
-Follow this:
-https://packaging.python.org/en/latest/tutorials/packaging-projects/
-
-A package needs:
-
-- pyproject.toml (used to define the metadata and configuration for your package. It provides information such as the package name, version, dependencies, and other details required for installation and distribution.)
-- README.md: This file contains the documentation and information about your package. It is commonly written in Markdown format and serves as the main entry point for users and developers to understand how to use your package.
-
-- LICENSE: This file includes the license under which your package is distributed. It is important to choose and include the appropriate license file, as we discussed in the previous response.
-
-- requirements.txt or pyproject.toml: These files are used to specify the dependencies required by your package. requirements.txt is a common format that lists the package names and versions, while pyproject.toml is used in the context of projects using the Poetry dependency manager.
-
-
-# How to get the package ready.
-
-1 - Make a 'wheel' and source distribution file (you pack the source code as binary and tar file)
-`py -m pip install --upgrade build`
-`py -m build`
-
-2 - go to https://test.pypi.org/account/register/ and complete the steps on that page. Verify your email address.
-
-3 - To securely upload your project, you’ll need a PyPI API token. Create one at https://test.pypi.org/manage/account/#api-tokens, setting the “Scope” to “Entire account”. Don’t close the page until you have copied and saved the token — you won’t see that token again.
-
-4 - Upload to PyPI test index
-`py -m pip install --upgrade twine`
-`py -m twine upload --repository testpypi dist/*`
-Username: __token__
-PW: enter your token here (WARNING - CTRL-V WILL NOT WORK. IN VSCODE: Edit --> Paste)
-
-5 - you can pull your own package from 
-py -m pip install --index-url https://test.pypi.org/simple/ --no-deps expert_intelligence_toolbox
-
-6 - make a real package
-delete `dist` directory
-`py -m build`
-`py -m twine upload dist/*`
-Username: __token__
-PW: enter your token here (WARNING - CTRL-V WILL NOT WORK. IN VSCODE: Edit --> Paste)
-
-
-5 - What if you make any changes? Just repeat.
-Change version number in pyproject.toml
-`py -m build`
-`twine upload --skip-existing dist/*`
+# expert_intelligence_toolbox
+This is an experimental v0.1, which currently serves no function other than testing.
+Hello update.
+
+## Internal:
+Follow this:
+https://packaging.python.org/en/latest/tutorials/packaging-projects/
+
+A package needs:
+
+- pyproject.toml (used to define the metadata and configuration for your package. It provides information such as the package name, version, dependencies, and other details required for installation and distribution.)
+- README.md: This file contains the documentation and information about your package. It is commonly written in Markdown format and serves as the main entry point for users and developers to understand how to use your package.
+
+- LICENSE: This file includes the license under which your package is distributed. It is important to choose and include the appropriate license file, as we discussed in the previous response.
+
+- requirements.txt or pyproject.toml: These files are used to specify the dependencies required by your package. requirements.txt is a common format that lists the package names and versions, while pyproject.toml is used in the context of projects using the Poetry dependency manager.
+
+
+# How to get the package ready.
+
+1 - Make a 'wheel' and source distribution file (you pack the source code as binary and tar file)
+`py -m pip install --upgrade build`
+`py -m build`
+
+2 - go to https://test.pypi.org/account/register/ and complete the steps on that page. Verify your email address.
+
+3 - To securely upload your project, you’ll need a PyPI API token. Create one at https://test.pypi.org/manage/account/#api-tokens, setting the “Scope” to “Entire account”. Don’t close the page until you have copied and saved the token — you won’t see that token again.
+
+4 - Upload to PyPI test index
+`py -m pip install --upgrade twine`
+`py -m twine upload --repository testpypi dist/*`
+Username: __token__
+PW: enter your token here (WARNING - CTRL-V WILL NOT WORK. IN VSCODE: Edit --> Paste)
+
+5 - you can pull your own package from 
+py -m pip install --index-url https://test.pypi.org/simple/ --no-deps expert_intelligence_toolbox
+
+6 - make a real package
+delete `dist` directory
+`py -m build`
+`py -m twine upload dist/*`
+Username: __token__
+PW: enter your token here (WARNING - CTRL-V WILL NOT WORK. IN VSCODE: Edit --> Paste)
+
+
+5 - What if you make any changes? Just repeat.
+Change version number in pyproject.toml
+`py -m build`
+`twine upload --skip-existing dist/*`
 `twine upload --skip-existing --repository testpypi dist/*` (for testpypi)
```

### Comparing `expert_intelligence_toolbox-0.0.4/PKG-INFO` & `expert_intelligence_toolbox-0.0.5/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: expert_intelligence_toolbox
-Version: 0.0.4
+Version: 0.0.5
 Summary: This is (for now) a test.
 Project-URL: Homepage, https://github.com/Point-Topic/expert_intelligence_toolbox
 Project-URL: Bug Tracker, https://github.com/Point-Topic/expert_intelligence_toolbox/issues
 Author-email: Arnold Kuersteiner <arnold.kuersteiner@expert-intelligence.com>
 License-File: LICENSE
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

