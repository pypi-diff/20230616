# Comparing `tmp/kompiler-1.2.0.tar.gz` & `tmp/kompiler-1.2.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "kompiler-1.2.0.tar", last modified: Tue Feb  8 03:18:11 2022, max compression
+gzip compressed data, was "kompiler-1.2.1.tar", last modified: Fri Jun 16 07:23:51 2023, max compression
```

## Comparing `kompiler-1.2.0.tar` & `kompiler-1.2.1.tar`

### file list

```diff
@@ -1,17 +1,17 @@
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-02-08 03:18:11.172407 kompiler-1.2.0/
--rw-r--r--   0 runner    (1001) docker     (121)     1069 2022-02-08 03:17:52.000000 kompiler-1.2.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (121)     1148 2022-02-08 03:18:11.172407 kompiler-1.2.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)      512 2022-02-08 03:17:52.000000 kompiler-1.2.0/README.md
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-02-08 03:18:11.172407 kompiler-1.2.0/kompiler/
--rw-r--r--   0 runner    (1001) docker     (121)      546 2022-02-08 03:17:52.000000 kompiler-1.2.0/kompiler/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     2234 2022-02-08 03:17:52.000000 kompiler-1.2.0/kompiler/__main__.py
--rw-r--r--   0 runner    (1001) docker     (121)     1320 2022-02-08 03:17:52.000000 kompiler-1.2.0/kompiler/constants.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-02-08 03:18:11.172407 kompiler-1.2.0/kompiler.egg-info/
--rw-r--r--   0 runner    (1001) docker     (121)     1148 2022-02-08 03:18:11.000000 kompiler-1.2.0/kompiler.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)      268 2022-02-08 03:18:11.000000 kompiler-1.2.0/kompiler.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (121)        1 2022-02-08 03:18:11.000000 kompiler-1.2.0/kompiler.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (121)       53 2022-02-08 03:18:11.000000 kompiler-1.2.0/kompiler.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (121)        9 2022-02-08 03:18:11.000000 kompiler-1.2.0/kompiler.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (121)      135 2022-02-08 03:17:52.000000 kompiler-1.2.0/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (121)       38 2022-02-08 03:18:11.172407 kompiler-1.2.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (121)      934 2022-02-08 03:17:52.000000 kompiler-1.2.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 07:23:51.650146 kompiler-1.2.1/
+-rw-r--r--   0 runner    (1001) docker     (123)     1069 2023-06-16 07:23:35.000000 kompiler-1.2.1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     1112 2023-06-16 07:23:51.650146 kompiler-1.2.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      512 2023-06-16 07:23:35.000000 kompiler-1.2.1/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 07:23:51.650146 kompiler-1.2.1/kompiler/
+-rw-r--r--   0 runner    (1001) docker     (123)      546 2023-06-16 07:23:35.000000 kompiler-1.2.1/kompiler/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2234 2023-06-16 07:23:35.000000 kompiler-1.2.1/kompiler/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1320 2023-06-16 07:23:35.000000 kompiler-1.2.1/kompiler/constants.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 07:23:51.650146 kompiler-1.2.1/kompiler.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     1112 2023-06-16 07:23:51.000000 kompiler-1.2.1/kompiler.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      268 2023-06-16 07:23:51.000000 kompiler-1.2.1/kompiler.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-16 07:23:51.000000 kompiler-1.2.1/kompiler.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       52 2023-06-16 07:23:51.000000 kompiler-1.2.1/kompiler.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        9 2023-06-16 07:23:51.000000 kompiler-1.2.1/kompiler.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      135 2023-06-16 07:23:35.000000 kompiler-1.2.1/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-16 07:23:51.650146 kompiler-1.2.1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      934 2023-06-16 07:23:35.000000 kompiler-1.2.1/setup.py
```

### Comparing `kompiler-1.2.0/LICENSE` & `kompiler-1.2.1/LICENSE`

 * *Files identical despite different names*

### Comparing `kompiler-1.2.0/PKG-INFO` & `kompiler-1.2.1/PKG-INFO`

 * *Files 15% similar despite different names*

```diff
@@ -1,17 +1,15 @@
 Metadata-Version: 2.1
 Name: kompiler
-Version: 1.2.0
+Version: 1.2.1
 Summary: A package for auto compiling C++ files as soon as they are saved.
 Home-page: https://github.com/garvit-joshi/kompiler
 Author: Garvit Joshi
 Author-email: garvitjoshi9@gmail.com
-License: UNKNOWN
 Keywords: C++ Compiling g++
-Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Classifier: Topic :: Education
 Classifier: Programming Language :: C++
 Classifier: Topic :: Utilities
 Requires-Python: >=3.5
@@ -27,8 +25,7 @@
     ❯ kompiler hello.cpp
         Command used for compiling: g++ hello.cpp
     ❯ kompiler hello.cpp -std=c++11 -O2 -Wall hello.cpp -o hello
         Command used for compiling: g++ -std=c++11 -O2 -Wall hello.cpp -o hello
     ❯ kompiler 3.cpp -std=c++11 -O2 -Wall 3.cpp -o hello "&&" ./hello
         Command used for compiling: g++ -std=c++11 -O2 -Wall 3.cpp -o hello && ./hello
 ```
-
```

### Comparing `kompiler-1.2.0/README.md` & `kompiler-1.2.1/README.md`

 * *Files identical despite different names*

### Comparing `kompiler-1.2.0/kompiler/__init__.py` & `kompiler-1.2.1/kompiler/__init__.py`

 * *Files identical despite different names*

### Comparing `kompiler-1.2.0/kompiler/__main__.py` & `kompiler-1.2.1/kompiler/__main__.py`

 * *Files identical despite different names*

### Comparing `kompiler-1.2.0/kompiler/constants.py` & `kompiler-1.2.1/kompiler/constants.py`

 * *Files 7% similar despite different names*

```diff
@@ -6,15 +6,15 @@
 # FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE
 # AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER
 # LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,
 # OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE
 # SOFTWARE.
 
 
-VERSION_NO = "1.2.0"
+VERSION_NO = "1.2.1"
 
 VERSION = "Kompiler: v"+VERSION_NO
 
 ABOUT = """
 Kompiler: A package for auto compiling C++ files as soon as they are saved.\n
 Source Code: https://github.com/garvit-joshi/kompiler/
 pip: https://pypi.org/project/kompiler/
```

### Comparing `kompiler-1.2.0/kompiler.egg-info/PKG-INFO` & `kompiler-1.2.1/kompiler.egg-info/PKG-INFO`

 * *Files 15% similar despite different names*

```diff
@@ -1,17 +1,15 @@
 Metadata-Version: 2.1
 Name: kompiler
-Version: 1.2.0
+Version: 1.2.1
 Summary: A package for auto compiling C++ files as soon as they are saved.
 Home-page: https://github.com/garvit-joshi/kompiler
 Author: Garvit Joshi
 Author-email: garvitjoshi9@gmail.com
-License: UNKNOWN
 Keywords: C++ Compiling g++
-Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Classifier: Topic :: Education
 Classifier: Programming Language :: C++
 Classifier: Topic :: Utilities
 Requires-Python: >=3.5
@@ -27,8 +25,7 @@
     ❯ kompiler hello.cpp
         Command used for compiling: g++ hello.cpp
     ❯ kompiler hello.cpp -std=c++11 -O2 -Wall hello.cpp -o hello
         Command used for compiling: g++ -std=c++11 -O2 -Wall hello.cpp -o hello
     ❯ kompiler 3.cpp -std=c++11 -O2 -Wall 3.cpp -o hello "&&" ./hello
         Command used for compiling: g++ -std=c++11 -O2 -Wall 3.cpp -o hello && ./hello
 ```
-
```

### Comparing `kompiler-1.2.0/setup.py` & `kompiler-1.2.1/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import setuptools
 
 with open("README.md", "r", encoding="utf8") as fh:
     long_description = fh.read()
 
 setuptools.setup(
     name="kompiler",
-    version="1.2.0",
+    version="1.2.1",
     author="Garvit Joshi",
     author_email="garvitjoshi9@gmail.com",
     description="A package for auto compiling C++ files as soon as they are saved.",
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="https://github.com/garvit-joshi/kompiler",
     packages=["kompiler"],
```

