# Comparing `tmp/vocab-coverage-0.3.tar.gz` & `tmp/vocab-coverage-0.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "vocab-coverage-0.3.tar", last modified: Fri Jun 16 06:55:49 2023, max compression
+gzip compressed data, was "vocab-coverage-0.4.tar", last modified: Fri Jun 16 08:04:58 2023, max compression
```

## Comparing `vocab-coverage-0.3.tar` & `vocab-coverage-0.4.tar`

### file list

```diff
@@ -1,18 +1,19 @@
-drwxr-xr-x   0 tao        (502) staff       (20)        0 2023-06-16 06:55:49.920357 vocab-coverage-0.3/
--rw-r--r--   0 tao        (502) staff       (20)    11357 2023-06-15 09:34:29.000000 vocab-coverage-0.3/LICENSE
--rw-r--r--   0 tao        (502) staff       (20)     9064 2023-06-16 06:55:49.920191 vocab-coverage-0.3/PKG-INFO
--rw-r--r--   0 tao        (502) staff       (20)     8149 2023-06-15 08:53:12.000000 vocab-coverage-0.3/README.md
--rw-r--r--   0 tao        (502) staff       (20)       38 2023-06-16 06:55:49.920397 vocab-coverage-0.3/setup.cfg
--rw-r--r--   0 tao        (502) staff       (20)     1485 2023-06-16 06:55:24.000000 vocab-coverage-0.3/setup.py
-drwxr-xr-x   0 tao        (502) staff       (20)        0 2023-06-16 06:55:49.919189 vocab-coverage-0.3/vocab_coverage/
--rw-r--r--   0 tao        (502) staff       (20)       66 2023-06-16 06:00:34.000000 vocab-coverage-0.3/vocab_coverage/__init__.py
--rw-r--r--   0 tao        (502) staff       (20)     4401 2023-06-16 05:50:29.000000 vocab-coverage-0.3/vocab_coverage/charsets.py
--rw-r--r--   0 tao        (502) staff       (20)     3002 2023-06-16 05:34:42.000000 vocab-coverage-0.3/vocab_coverage/draw.py
--rw-r--r--   0 tao        (502) staff       (20)     6004 2023-06-16 05:34:26.000000 vocab-coverage-0.3/vocab_coverage/model.py
-drwxr-xr-x   0 tao        (502) staff       (20)        0 2023-06-16 06:55:49.919989 vocab-coverage-0.3/vocab_coverage.egg-info/
--rw-r--r--   0 tao        (502) staff       (20)     9064 2023-06-16 06:55:49.000000 vocab-coverage-0.3/vocab_coverage.egg-info/PKG-INFO
--rw-r--r--   0 tao        (502) staff       (20)      357 2023-06-16 06:55:49.000000 vocab-coverage-0.3/vocab_coverage.egg-info/SOURCES.txt
--rw-r--r--   0 tao        (502) staff       (20)        1 2023-06-16 06:55:49.000000 vocab-coverage-0.3/vocab_coverage.egg-info/dependency_links.txt
--rw-r--r--   0 tao        (502) staff       (20)       61 2023-06-16 06:55:49.000000 vocab-coverage-0.3/vocab_coverage.egg-info/entry_points.txt
--rw-r--r--   0 tao        (502) staff       (20)      114 2023-06-16 06:55:49.000000 vocab-coverage-0.3/vocab_coverage.egg-info/requires.txt
--rw-r--r--   0 tao        (502) staff       (20)       15 2023-06-16 06:55:49.000000 vocab-coverage-0.3/vocab_coverage.egg-info/top_level.txt
+drwxr-xr-x   0 tao        (502) staff       (20)        0 2023-06-16 08:04:58.017979 vocab-coverage-0.4/
+-rw-r--r--   0 tao        (502) staff       (20)    11357 2023-06-15 09:34:29.000000 vocab-coverage-0.4/LICENSE
+-rw-r--r--   0 tao        (502) staff       (20)     9038 2023-06-16 08:04:58.017828 vocab-coverage-0.4/PKG-INFO
+-rw-r--r--   0 tao        (502) staff       (20)     8149 2023-06-15 08:53:12.000000 vocab-coverage-0.4/README.md
+-rw-r--r--   0 tao        (502) staff       (20)       38 2023-06-16 08:04:58.018039 vocab-coverage-0.4/setup.cfg
+-rw-r--r--   0 tao        (502) staff       (20)     1401 2023-06-16 07:49:50.000000 vocab-coverage-0.4/setup.py
+drwxr-xr-x   0 tao        (502) staff       (20)        0 2023-06-16 08:04:58.016943 vocab-coverage-0.4/vocab_coverage/
+-rw-r--r--   0 tao        (502) staff       (20)      128 2023-06-16 07:49:46.000000 vocab-coverage-0.4/vocab_coverage/__init__.py
+-rw-r--r--   0 tao        (502) staff       (20)     4166 2023-06-16 07:57:21.000000 vocab-coverage-0.4/vocab_coverage/charsets.py
+-rw-r--r--   0 tao        (502) staff       (20)     3002 2023-06-16 05:34:42.000000 vocab-coverage-0.4/vocab_coverage/draw.py
+-rw-r--r--   0 tao        (502) staff       (20)     1645 2023-06-16 07:57:38.000000 vocab-coverage-0.4/vocab_coverage/main.py
+-rw-r--r--   0 tao        (502) staff       (20)     5196 2023-06-16 07:57:33.000000 vocab-coverage-0.4/vocab_coverage/model.py
+drwxr-xr-x   0 tao        (502) staff       (20)        0 2023-06-16 08:04:58.017632 vocab-coverage-0.4/vocab_coverage.egg-info/
+-rw-r--r--   0 tao        (502) staff       (20)     9038 2023-06-16 08:04:57.000000 vocab-coverage-0.4/vocab_coverage.egg-info/PKG-INFO
+-rw-r--r--   0 tao        (502) staff       (20)      380 2023-06-16 08:04:57.000000 vocab-coverage-0.4/vocab_coverage.egg-info/SOURCES.txt
+-rw-r--r--   0 tao        (502) staff       (20)        1 2023-06-16 08:04:57.000000 vocab-coverage-0.4/vocab_coverage.egg-info/dependency_links.txt
+-rw-r--r--   0 tao        (502) staff       (20)       55 2023-06-16 08:04:57.000000 vocab-coverage-0.4/vocab_coverage.egg-info/entry_points.txt
+-rw-r--r--   0 tao        (502) staff       (20)      101 2023-06-16 08:04:57.000000 vocab-coverage-0.4/vocab_coverage.egg-info/requires.txt
+-rw-r--r--   0 tao        (502) staff       (20)       15 2023-06-16 08:04:57.000000 vocab-coverage-0.4/vocab_coverage.egg-info/top_level.txt
```

### Comparing `vocab-coverage-0.3/LICENSE` & `vocab-coverage-0.4/LICENSE`

 * *Files identical despite different names*

### Comparing `vocab-coverage-0.3/PKG-INFO` & `vocab-coverage-0.4/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: vocab-coverage
-Version: 0.3
+Version: 0.4
 Summary: A Python package designed to perform coverage analysis on Chinese vocabulary for language models.
 Home-page: https://github.com/twang2218/vocab-coverage
 Author: Tao Wang
 Author-email: twang2218@gmail.com
 License: Apache License 2.0
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
@@ -13,15 +13,14 @@
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3
 Classifier: Topic :: Scientific/Engineering :: Artificial Intelligence
 Classifier: Topic :: Scientific/Engineering :: Information Analysis
 Classifier: Topic :: Text Processing :: Linguistic
 Description-Content-Type: text/markdown
-Provides-Extra: generator
 License-File: LICENSE
 
 # 语言模型中文识字率分析
 
 - [语言模型中文识字率分析](#语言模型中文识字率分析)
   - [项目介绍](#项目介绍)
   - [分析结果](#分析结果)
```

### Comparing `vocab-coverage-0.3/README.md` & `vocab-coverage-0.4/README.md`

 * *Files identical despite different names*

### Comparing `vocab-coverage-0.3/setup.py` & `vocab-coverage-0.4/setup.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,29 +1,25 @@
 from setuptools import setup, find_packages
 
 setup(
     name='vocab-coverage',
-    version='0.3',
+    version='0.4',
     packages=find_packages(),
     install_requires=[
         'Pillow',
         'protobuf==3.20.0',
         'sentencepiece',
         'tiktoken',
         'torch',
         'transformers',
+        'beautifulsoup4',
+        'bs4',
+        'pandas',
+        'requests',
     ],
-    extras_require={
-        'generator': [
-            'beautifulsoup4',
-            'bs4',
-            'pandas',
-            'requests',
-        ],
-    },
     description='A Python package designed to perform coverage analysis on Chinese vocabulary for language models.',
     long_description_content_type="text/markdown",
     long_description=open('README.md').read(),
     author='Tao Wang',
     author_email='twang2218@gmail.com',
     url='https://github.com/twang2218/vocab-coverage',
     license='Apache License 2.0',
@@ -37,12 +33,12 @@
         "Programming Language :: Python :: 3",
         "Topic :: Scientific/Engineering :: Artificial Intelligence",
         "Topic :: Scientific/Engineering :: Information Analysis",
         "Topic :: Text Processing :: Linguistic",
     ],
     entry_points={
         'console_scripts': [
-            'vocab-coverage = vocab_coverage.model:main',
+            'vocab-coverage = vocab_coverage:main',
         ],
     },
 )
```

### Comparing `vocab-coverage-0.3/vocab_coverage/charsets.py` & `vocab-coverage-0.4/vocab_coverage/charsets.py`

 * *Files 8% similar despite different names*

```diff
@@ -97,13 +97,7 @@
     charset['《Unicode中日韩统一表意文字》(增)'] = extra_chars
 
     print(f"共有{sum([len(c) for c in charset.values()])}个汉字")
 
     # 保存到JSON文件
     with open(filename, 'w') as f:
         json.dump(charset, f, ensure_ascii=False, indent=4)
-
-if __name__ == '__main__':
-    parser = argparse.ArgumentParser()
-    parser.add_argument("--charset_file", type=str, default="charset.json", help="字表文件")
-    args = parser.parse_args()
-    generate_charsets(args.charset_file)
```

### Comparing `vocab-coverage-0.3/vocab_coverage/draw.py` & `vocab-coverage-0.4/vocab_coverage/draw.py`

 * *Files identical despite different names*

### Comparing `vocab-coverage-0.3/vocab_coverage.egg-info/PKG-INFO` & `vocab-coverage-0.4/vocab_coverage.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: vocab-coverage
-Version: 0.3
+Version: 0.4
 Summary: A Python package designed to perform coverage analysis on Chinese vocabulary for language models.
 Home-page: https://github.com/twang2218/vocab-coverage
 Author: Tao Wang
 Author-email: twang2218@gmail.com
 License: Apache License 2.0
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
@@ -13,15 +13,14 @@
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3
 Classifier: Topic :: Scientific/Engineering :: Artificial Intelligence
 Classifier: Topic :: Scientific/Engineering :: Information Analysis
 Classifier: Topic :: Text Processing :: Linguistic
 Description-Content-Type: text/markdown
-Provides-Extra: generator
 License-File: LICENSE
 
 # 语言模型中文识字率分析
 
 - [语言模型中文识字率分析](#语言模型中文识字率分析)
   - [项目介绍](#项目介绍)
   - [分析结果](#分析结果)
```

