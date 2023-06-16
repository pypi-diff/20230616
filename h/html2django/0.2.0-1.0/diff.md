# Comparing `tmp/html2django-0.2.0.tar.gz` & `tmp/html2django-1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "html2django-0.2.0.tar", last modified: Fri Jun 16 09:33:31 2023, max compression
+gzip compressed data, was "html2django-1.0.tar", last modified: Fri Apr 14 08:01:00 2023, max compression
```

## Comparing `html2django-0.2.0.tar` & `html2django-1.0.tar`

### file list

```diff
@@ -1,16 +1,17 @@
-drwxrwxr-x   0 haxsys    (1000) haxsys    (1000)        0 2023-06-16 09:33:31.939443 html2django-0.2.0/
--rw-rw-r--   0 haxsys    (1000) haxsys    (1000)     3785 2023-06-16 09:33:31.939443 html2django-0.2.0/PKG-INFO
--rw-rw-r--   0 haxsys    (1000) haxsys    (1000)     3147 2023-06-16 09:32:34.000000 html2django-0.2.0/README.md
-drwxrwxr-x   0 haxsys    (1000) haxsys    (1000)        0 2023-06-16 09:33:31.935443 html2django-0.2.0/html2django/
--rw-rw-r--   0 haxsys    (1000) haxsys    (1000)       32 2023-06-16 09:20:52.000000 html2django-0.2.0/html2django/__init__.py
--rw-rw-r--   0 haxsys    (1000) haxsys    (1000)     3157 2023-04-14 07:41:34.000000 html2django-0.2.0/html2django/djangohtml.py
-drwxrwxr-x   0 haxsys    (1000) haxsys    (1000)        0 2023-06-16 09:33:31.939443 html2django-0.2.0/html2django.egg-info/
--rw-rw-r--   0 haxsys    (1000) haxsys    (1000)     3785 2023-06-16 09:33:31.000000 html2django-0.2.0/html2django.egg-info/PKG-INFO
--rw-rw-r--   0 haxsys    (1000) haxsys    (1000)      295 2023-06-16 09:33:31.000000 html2django-0.2.0/html2django.egg-info/SOURCES.txt
--rw-rw-r--   0 haxsys    (1000) haxsys    (1000)        1 2023-06-16 09:33:31.000000 html2django-0.2.0/html2django.egg-info/dependency_links.txt
--rw-rw-r--   0 haxsys    (1000) haxsys    (1000)       65 2023-06-16 09:33:31.000000 html2django-0.2.0/html2django.egg-info/entry_points.txt
--rw-rw-r--   0 haxsys    (1000) haxsys    (1000)       15 2023-06-16 09:33:31.000000 html2django-0.2.0/html2django.egg-info/requires.txt
--rw-rw-r--   0 haxsys    (1000) haxsys    (1000)       12 2023-06-16 09:33:31.000000 html2django-0.2.0/html2django.egg-info/top_level.txt
--rw-rw-r--   0 haxsys    (1000) haxsys    (1000)       86 2023-04-13 16:24:18.000000 html2django-0.2.0/pyproject.toml
--rw-rw-r--   0 haxsys    (1000) haxsys    (1000)       38 2023-06-16 09:33:31.939443 html2django-0.2.0/setup.cfg
--rw-rw-r--   0 haxsys    (1000) haxsys    (1000)     1076 2023-06-16 09:20:31.000000 html2django-0.2.0/setup.py
+drwxrwxr-x   0 haxsys    (1000) haxsys    (1000)        0 2023-04-14 08:01:00.051199 html2django-1.0/
+-rw-rw-r--   0 haxsys    (1000) haxsys    (1000)     1081 2023-04-13 10:17:55.000000 html2django-1.0/LICENSE.txt
+-rw-rw-r--   0 haxsys    (1000) haxsys    (1000)     2850 2023-04-14 08:01:00.051199 html2django-1.0/PKG-INFO
+-rw-rw-r--   0 haxsys    (1000) haxsys    (1000)     2188 2023-04-14 07:39:31.000000 html2django-1.0/README.md
+drwxrwxr-x   0 haxsys    (1000) haxsys    (1000)        0 2023-04-14 08:01:00.003195 html2django-1.0/html2django/
+-rw-rw-r--   0 haxsys    (1000) haxsys    (1000)        0 2023-04-13 09:23:08.000000 html2django-1.0/html2django/__init__.py
+-rw-rw-r--   0 haxsys    (1000) haxsys    (1000)     3157 2023-04-14 07:41:34.000000 html2django-1.0/html2django/djangohtml.py
+drwxrwxr-x   0 haxsys    (1000) haxsys    (1000)        0 2023-04-14 08:01:00.051199 html2django-1.0/html2django.egg-info/
+-rw-rw-r--   0 haxsys    (1000) haxsys    (1000)     2850 2023-04-14 08:00:59.000000 html2django-1.0/html2django.egg-info/PKG-INFO
+-rw-rw-r--   0 haxsys    (1000) haxsys    (1000)      307 2023-04-14 08:00:59.000000 html2django-1.0/html2django.egg-info/SOURCES.txt
+-rw-rw-r--   0 haxsys    (1000) haxsys    (1000)        1 2023-04-14 08:00:59.000000 html2django-1.0/html2django.egg-info/dependency_links.txt
+-rw-rw-r--   0 haxsys    (1000) haxsys    (1000)       52 2023-04-14 08:00:59.000000 html2django-1.0/html2django.egg-info/entry_points.txt
+-rw-rw-r--   0 haxsys    (1000) haxsys    (1000)       15 2023-04-14 08:00:59.000000 html2django-1.0/html2django.egg-info/requires.txt
+-rw-rw-r--   0 haxsys    (1000) haxsys    (1000)       12 2023-04-14 08:00:59.000000 html2django-1.0/html2django.egg-info/top_level.txt
+-rw-rw-r--   0 haxsys    (1000) haxsys    (1000)       86 2023-04-13 16:24:18.000000 html2django-1.0/pyproject.toml
+-rw-rw-r--   0 haxsys    (1000) haxsys    (1000)       38 2023-04-14 08:01:00.051199 html2django-1.0/setup.cfg
+-rw-rw-r--   0 haxsys    (1000) haxsys    (1000)     1061 2023-04-14 08:00:03.000000 html2django-1.0/setup.py
```

### Comparing `html2django-0.2.0/PKG-INFO` & `html2django-1.0/PKG-INFO`

 * *Files 18% similar despite different names*

```diff
@@ -1,39 +1,26 @@
 Metadata-Version: 2.1
 Name: html2django
-Version: 0.2.0
+Version: 1.0
 Summary: A Python script to modify HTML files for Django templates
 Home-page: https://github.com/haxsysgit/html2django
 Author: Elenasulu Arinze
 Author-email: pentacker@gmail.com
 Classifier: Development Status :: 3 - Alpha
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
+License-File: LICENSE.txt
 
 
-<!-- Badges -->
-[![PyPI version](https://badge.fury.io/py/html2django.svg)](https://pypi.org/project/html2django/)
-[![contributions welcome](https://img.shields.io/badge/contributions-welcome-brightgreen.svg?style=flat)](https://github.com/haxsysgit/html2django/)
-[![License](https://img.shields.io/github/license/haxsysgit/html2django?color=brightgreen)](https://github.com/haxsysgit/html2django/blob/main/license.md)
-[![OpenIssues](https://img.shields.io/github/issues/haxsysgit/html2django?color=important)](https://github.com/haxsysgit/html2django/issues)
-<!--LineBreak-->
-[![Windows](https://img.shields.io/badge/Windows-white?style=flat-square&logo=windows&logoColor=blue)](https://github.com/haxsysgit/html2django/)
-[![Ubuntu](https://img.shields.io/badge/Ubuntu-white?style=flat-square&logo=ubuntu&logoColor=E95420)](https://github.com/haxsysgit/html2django/)
-<!-- Badges -->
-
-# html2django
-
-- Convert your html static tags to django static template
-
 ## Description
 
 Modifies the HTML content of a file to replace all <link> tags' href attributes, all <script> tags' src attributes, and all <img> src attributes by default, also provides support for custom modification of tags and attribute with Django template tags, and adds {% load static %} to the beginning of the file.
 
 
 ## Installation
```

#### html2text {}

 * *error from `html2text {}`:*

 * *File "/tmp/diffoscope_liikg85q_/tmp9um57tjt_TarContainer/0/1", line 124, column 0: CDATA terminal not found*

 * *File "/tmp/diffoscope_liikg85q_/tmp9um57tjt_TarContainer/0/1", line 124, column 0: CDATA terminal not found*

```diff
@@ -1,29 +1,17 @@
-Metadata-Version: 2.1 Name: html2django Version: 0.2.0 Summary: A Python script
+Metadata-Version: 2.1 Name: html2django Version: 1.0 Summary: A Python script
 to modify HTML files for Django templates Home-page: https://github.com/
 haxsysgit/html2django Author: Elenasulu Arinze Author-email:
 pentacker@gmail.com Classifier: Development Status :: 3 - Alpha Classifier:
 License :: OSI Approved :: MIT License Classifier: Operating System :: OS
 Independent Classifier: Programming Language :: Python :: 3 Classifier:
 Programming Language :: Python :: 3.7 Classifier: Programming Language ::
 Python :: 3.8 Classifier: Programming Language :: Python :: 3.9 Requires-
-Python: >=3.7 Description-Content-Type: text/markdown  [![PyPI version](https:/
-/badge.fury.io/py/html2django.svg)](https://pypi.org/project/html2django/) [!
-[contributions welcome](https://img.shields.io/badge/contributions-welcome-
-brightgreen.svg?style=flat)](https://github.com/haxsysgit/html2django/) [!
-[License](https://img.shields.io/github/license/haxsysgit/
-html2django?color=brightgreen)](https://github.com/haxsysgit/html2django/blob/
-main/license.md) [![OpenIssues](https://img.shields.io/github/issues/haxsysgit/
-html2django?color=important)](https://github.com/haxsysgit/html2django/issues)
-[![Windows](https://img.shields.io/badge/Windows-white?style=flat-
-square&logo=windows&logoColor=blue)](https://github.com/haxsysgit/html2django/
-) [![Ubuntu](https://img.shields.io/badge/Ubuntu-white?style=flat-
-square&logo=ubuntu&logoColor=E95420)](https://github.com/haxsysgit/html2django/
-)  # html2django - Convert your html static tags to django static template ##
-Description Modifies the HTML content of a file to replace all
+Python: >=3.7 Description-Content-Type: text/markdown License-File: LICENSE.txt
+## Description Modifies the HTML content of a file to replace all
  tags' href attributes, all
 ****** Hello, World! ******
 [image.png]
 ``` Running the djangoify() function on this file: ```python djangoify
 ('index.html') ``` will modify the file to look like this: ```html {% load
 static %}
 ****** Hello, World! ******
```

### Comparing `html2django-0.2.0/README.md` & `html2django-1.0/README.md`

 * *Files 14% similar despite different names*

```diff
@@ -1,22 +1,8 @@
 
-<!-- Badges -->
-[![PyPI version](https://badge.fury.io/py/html2django.svg)](https://pypi.org/project/html2django/)
-[![contributions welcome](https://img.shields.io/badge/contributions-welcome-brightgreen.svg?style=flat)](https://github.com/haxsysgit/html2django/)
-[![License](https://img.shields.io/github/license/haxsysgit/html2django?color=brightgreen)](https://github.com/haxsysgit/html2django/blob/main/license.md)
-[![OpenIssues](https://img.shields.io/github/issues/haxsysgit/html2django?color=important)](https://github.com/haxsysgit/html2django/issues)
-<!--LineBreak-->
-[![Windows](https://img.shields.io/badge/Windows-white?style=flat-square&logo=windows&logoColor=blue)](https://github.com/haxsysgit/html2django/)
-[![Ubuntu](https://img.shields.io/badge/Ubuntu-white?style=flat-square&logo=ubuntu&logoColor=E95420)](https://github.com/haxsysgit/html2django/)
-<!-- Badges -->
-
-# html2django
-
-- Convert your html static tags to django static template
-
 ## Description
 
 Modifies the HTML content of a file to replace all <link> tags' href attributes, all <script> tags' src attributes, and all <img> src attributes by default, also provides support for custom modification of tags and attribute with Django template tags, and adds {% load static %} to the beginning of the file.
 
 
 ## Installation
```

#### html2text {}

 * *error from `html2text {}`:*

 * *File "/tmp/diffoscope_liikg85q_/tmp9um57tjt_TarContainer/0/2.md", line 106, column 43: CDATA terminal not found*

 * *File "/tmp/diffoscope_liikg85q_/tmp9um57tjt_TarContainer/0/2.md", line 106, column 43: CDATA terminal not found*

```diff
@@ -1,21 +1,8 @@
-  [![PyPI version](https://badge.fury.io/py/html2django.svg)](https://pypi.org/
-project/html2django/) [![contributions welcome](https://img.shields.io/badge/
-contributions-welcome-brightgreen.svg?style=flat)](https://github.com/
-haxsysgit/html2django/) [![License](https://img.shields.io/github/license/
-haxsysgit/html2django?color=brightgreen)](https://github.com/haxsysgit/
-html2django/blob/main/license.md) [![OpenIssues](https://img.shields.io/github/
-issues/haxsysgit/html2django?color=important)](https://github.com/haxsysgit/
-html2django/issues)  [![Windows](https://img.shields.io/badge/Windows-
-white?style=flat-square&logo=windows&logoColor=blue)](https://github.com/
-haxsysgit/html2django/) [![Ubuntu](https://img.shields.io/badge/Ubuntu-
-white?style=flat-square&logo=ubuntu&logoColor=E95420)](https://github.com/
-haxsysgit/html2django/)  # html2django - Convert your html static tags to
-django static template ## Description Modifies the HTML content of a file to
-replace all
+ ## Description Modifies the HTML content of a file to replace all
  tags' href attributes, all
 ****** Hello, World! ******
 [image.png]
 ``` Running the djangoify() function on this file: ```python djangoify
 ('index.html') ``` will modify the file to look like this: ```html {% load
 static %}
 ****** Hello, World! ******
```

### Comparing `html2django-0.2.0/html2django/djangohtml.py` & `html2django-1.0/html2django/djangohtml.py`

 * *Files identical despite different names*

### Comparing `html2django-0.2.0/html2django.egg-info/PKG-INFO` & `html2django-1.0/html2django.egg-info/PKG-INFO`

 * *Files 18% similar despite different names*

```diff
@@ -1,39 +1,26 @@
 Metadata-Version: 2.1
 Name: html2django
-Version: 0.2.0
+Version: 1.0
 Summary: A Python script to modify HTML files for Django templates
 Home-page: https://github.com/haxsysgit/html2django
 Author: Elenasulu Arinze
 Author-email: pentacker@gmail.com
 Classifier: Development Status :: 3 - Alpha
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
+License-File: LICENSE.txt
 
 
-<!-- Badges -->
-[![PyPI version](https://badge.fury.io/py/html2django.svg)](https://pypi.org/project/html2django/)
-[![contributions welcome](https://img.shields.io/badge/contributions-welcome-brightgreen.svg?style=flat)](https://github.com/haxsysgit/html2django/)
-[![License](https://img.shields.io/github/license/haxsysgit/html2django?color=brightgreen)](https://github.com/haxsysgit/html2django/blob/main/license.md)
-[![OpenIssues](https://img.shields.io/github/issues/haxsysgit/html2django?color=important)](https://github.com/haxsysgit/html2django/issues)
-<!--LineBreak-->
-[![Windows](https://img.shields.io/badge/Windows-white?style=flat-square&logo=windows&logoColor=blue)](https://github.com/haxsysgit/html2django/)
-[![Ubuntu](https://img.shields.io/badge/Ubuntu-white?style=flat-square&logo=ubuntu&logoColor=E95420)](https://github.com/haxsysgit/html2django/)
-<!-- Badges -->
-
-# html2django
-
-- Convert your html static tags to django static template
-
 ## Description
 
 Modifies the HTML content of a file to replace all <link> tags' href attributes, all <script> tags' src attributes, and all <img> src attributes by default, also provides support for custom modification of tags and attribute with Django template tags, and adds {% load static %} to the beginning of the file.
 
 
 ## Installation
```

#### html2text {}

 * *error from `html2text {}`:*

 * *File "/tmp/diffoscope_liikg85q_/tmp9um57tjt_TarContainer/0/7", line 124, column 0: CDATA terminal not found*

 * *File "/tmp/diffoscope_liikg85q_/tmp9um57tjt_TarContainer/0/7", line 124, column 0: CDATA terminal not found*

```diff
@@ -1,29 +1,17 @@
-Metadata-Version: 2.1 Name: html2django Version: 0.2.0 Summary: A Python script
+Metadata-Version: 2.1 Name: html2django Version: 1.0 Summary: A Python script
 to modify HTML files for Django templates Home-page: https://github.com/
 haxsysgit/html2django Author: Elenasulu Arinze Author-email:
 pentacker@gmail.com Classifier: Development Status :: 3 - Alpha Classifier:
 License :: OSI Approved :: MIT License Classifier: Operating System :: OS
 Independent Classifier: Programming Language :: Python :: 3 Classifier:
 Programming Language :: Python :: 3.7 Classifier: Programming Language ::
 Python :: 3.8 Classifier: Programming Language :: Python :: 3.9 Requires-
-Python: >=3.7 Description-Content-Type: text/markdown  [![PyPI version](https:/
-/badge.fury.io/py/html2django.svg)](https://pypi.org/project/html2django/) [!
-[contributions welcome](https://img.shields.io/badge/contributions-welcome-
-brightgreen.svg?style=flat)](https://github.com/haxsysgit/html2django/) [!
-[License](https://img.shields.io/github/license/haxsysgit/
-html2django?color=brightgreen)](https://github.com/haxsysgit/html2django/blob/
-main/license.md) [![OpenIssues](https://img.shields.io/github/issues/haxsysgit/
-html2django?color=important)](https://github.com/haxsysgit/html2django/issues)
-[![Windows](https://img.shields.io/badge/Windows-white?style=flat-
-square&logo=windows&logoColor=blue)](https://github.com/haxsysgit/html2django/
-) [![Ubuntu](https://img.shields.io/badge/Ubuntu-white?style=flat-
-square&logo=ubuntu&logoColor=E95420)](https://github.com/haxsysgit/html2django/
-)  # html2django - Convert your html static tags to django static template ##
-Description Modifies the HTML content of a file to replace all
+Python: >=3.7 Description-Content-Type: text/markdown License-File: LICENSE.txt
+## Description Modifies the HTML content of a file to replace all
  tags' href attributes, all
 ****** Hello, World! ******
 [image.png]
 ``` Running the djangoify() function on this file: ```python djangoify
 ('index.html') ``` will modify the file to look like this: ```html {% load
 static %}
 ****** Hello, World! ******
```

### Comparing `html2django-0.2.0/setup.py` & `html2django-1.0/setup.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 from setuptools import setup,find_packages
 
 with open('README.md', 'r', encoding='utf-8') as fh:
     long_description = fh.read()
 
 setup(
     name='html2django',
-    version='0.2.0',
+    version='1.0',
     author='Elenasulu Arinze',
     author_email='pentacker@gmail.com',
     description='A Python script to modify HTML files for Django templates',
     long_description=long_description,
     long_description_content_type='text/markdown',
     url='https://github.com/haxsysgit/html2django',
     packages=find_packages(),
@@ -24,11 +24,11 @@
     ],
     python_requires='>=3.7',
     install_requires=[
         'beautifulsoup4',
     ],
     entry_points={
         'console_scripts': [
-            'html2django = html2django.djangohtml:djangoify',
+            'djangohtml = djangohtml:djangoify',
         ],
     },
 )
```

