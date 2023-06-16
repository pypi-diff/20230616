# Comparing `tmp/python-pdfbox-v2-2.0.28.3.tar.gz` & `tmp/python-pdfbox-v2-2.0.28.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "python-pdfbox-v2-2.0.28.3.tar", last modified: Tue Jun  6 11:06:49 2023, max compression
+gzip compressed data, was "python-pdfbox-v2-2.0.28.4.tar", last modified: Fri Jun 16 09:27:29 2023, max compression
```

## Comparing `python-pdfbox-v2-2.0.28.3.tar` & `python-pdfbox-v2-2.0.28.4.tar`

### file list

```diff
@@ -1,23 +1,23 @@
-drwxrwxrwx   0 codespace  (1000) codespace  (1000)        0 2023-06-06 11:06:49.961708 python-pdfbox-v2-2.0.28.3/
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)      479 2023-06-06 10:20:56.000000 python-pdfbox-v2-2.0.28.3/AUTHORS.rst
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)      617 2023-06-06 10:20:56.000000 python-pdfbox-v2-2.0.28.3/LICENSE.rst
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)     3056 2023-06-06 11:06:49.961708 python-pdfbox-v2-2.0.28.3/PKG-INFO
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)     2457 2023-06-06 10:20:56.000000 python-pdfbox-v2-2.0.28.3/README.rst
-drwxrwxrwx   0 codespace  (1000) codespace  (1000)        0 2023-06-06 11:06:49.941708 python-pdfbox-v2-2.0.28.3/pdfbox/
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)     7927 2023-06-06 11:05:40.000000 python-pdfbox-v2-2.0.28.3/pdfbox/__init__.py
--rw-rw-rw-   0 codespace  (1000) codespace  (1000) 10085495 2023-06-06 11:04:29.000000 python-pdfbox-v2-2.0.28.3/pdfbox/pdfbox-app-2.0.28.jar
-drwxrwxrwx   0 codespace  (1000) codespace  (1000)        0 2023-06-06 11:06:49.957708 python-pdfbox-v2-2.0.28.3/python_pdfbox_v2.egg-info/
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)     3056 2023-06-06 11:06:49.000000 python-pdfbox-v2-2.0.28.3/python_pdfbox_v2.egg-info/PKG-INFO
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)      403 2023-06-06 11:06:49.000000 python-pdfbox-v2-2.0.28.3/python_pdfbox_v2.egg-info/SOURCES.txt
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)        1 2023-06-06 11:06:49.000000 python-pdfbox-v2-2.0.28.3/python_pdfbox_v2.egg-info/dependency_links.txt
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)       18 2023-06-06 11:06:49.000000 python-pdfbox-v2-2.0.28.3/python_pdfbox_v2.egg-info/requires.txt
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)        7 2023-06-06 11:06:49.000000 python-pdfbox-v2-2.0.28.3/python_pdfbox_v2.egg-info/top_level.txt
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)       53 2023-06-06 11:06:49.961708 python-pdfbox-v2-2.0.28.3/setup.cfg
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)     1500 2023-06-06 11:05:40.000000 python-pdfbox-v2-2.0.28.3/setup.py
-drwxrwxrwx   0 codespace  (1000) codespace  (1000)        0 2023-06-06 11:06:49.961708 python-pdfbox-v2-2.0.28.3/tests/
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)    24649 2023-06-06 10:20:56.000000 python-pdfbox-v2-2.0.28.3/tests/test space.pdf
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)       71 2023-06-06 10:20:56.000000 python-pdfbox-v2-2.0.28.3/tests/test.md
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)    24649 2023-06-06 10:20:56.000000 python-pdfbox-v2-2.0.28.3/tests/test.pdf
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)     2830 2023-06-06 10:20:56.000000 python-pdfbox-v2-2.0.28.3/tests/test2.pdf
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)    84980 2023-06-06 10:20:56.000000 python-pdfbox-v2-2.0.28.3/tests/test3.pdf
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)     1798 2023-06-06 10:20:56.000000 python-pdfbox-v2-2.0.28.3/tests/test_pdfbox.py
+drwxrwxrwx   0 codespace  (1000) codespace  (1000)        0 2023-06-16 09:27:29.663660 python-pdfbox-v2-2.0.28.4/
+-rw-rw-rw-   0 codespace  (1000) codespace  (1000)      479 2023-06-06 10:20:56.000000 python-pdfbox-v2-2.0.28.4/AUTHORS.rst
+-rw-rw-rw-   0 codespace  (1000) codespace  (1000)      617 2023-06-06 10:20:56.000000 python-pdfbox-v2-2.0.28.4/LICENSE.rst
+-rw-rw-rw-   0 codespace  (1000) codespace  (1000)     3056 2023-06-16 09:27:29.663660 python-pdfbox-v2-2.0.28.4/PKG-INFO
+-rw-rw-rw-   0 codespace  (1000) codespace  (1000)     2457 2023-06-06 10:20:56.000000 python-pdfbox-v2-2.0.28.4/README.rst
+drwxrwxrwx   0 codespace  (1000) codespace  (1000)        0 2023-06-16 09:27:29.331660 python-pdfbox-v2-2.0.28.4/pdfbox/
+-rw-rw-rw-   0 codespace  (1000) codespace  (1000)     7061 2023-06-16 09:24:18.000000 python-pdfbox-v2-2.0.28.4/pdfbox/__init__.py
+-rw-rw-rw-   0 codespace  (1000) codespace  (1000) 10085495 2023-06-06 11:04:29.000000 python-pdfbox-v2-2.0.28.4/pdfbox/pdfbox-app-2.0.28.jar
+drwxrwxrwx   0 codespace  (1000) codespace  (1000)        0 2023-06-16 09:27:29.583660 python-pdfbox-v2-2.0.28.4/python_pdfbox_v2.egg-info/
+-rw-rw-rw-   0 codespace  (1000) codespace  (1000)     3056 2023-06-16 09:27:29.000000 python-pdfbox-v2-2.0.28.4/python_pdfbox_v2.egg-info/PKG-INFO
+-rw-rw-rw-   0 codespace  (1000) codespace  (1000)      403 2023-06-16 09:27:29.000000 python-pdfbox-v2-2.0.28.4/python_pdfbox_v2.egg-info/SOURCES.txt
+-rw-rw-rw-   0 codespace  (1000) codespace  (1000)        1 2023-06-16 09:27:29.000000 python-pdfbox-v2-2.0.28.4/python_pdfbox_v2.egg-info/dependency_links.txt
+-rw-rw-rw-   0 codespace  (1000) codespace  (1000)       18 2023-06-16 09:27:29.000000 python-pdfbox-v2-2.0.28.4/python_pdfbox_v2.egg-info/requires.txt
+-rw-rw-rw-   0 codespace  (1000) codespace  (1000)        7 2023-06-16 09:27:29.000000 python-pdfbox-v2-2.0.28.4/python_pdfbox_v2.egg-info/top_level.txt
+-rw-rw-rw-   0 codespace  (1000) codespace  (1000)       53 2023-06-16 09:27:29.667660 python-pdfbox-v2-2.0.28.4/setup.cfg
+-rw-rw-rw-   0 codespace  (1000) codespace  (1000)     1500 2023-06-16 09:26:27.000000 python-pdfbox-v2-2.0.28.4/setup.py
+drwxrwxrwx   0 codespace  (1000) codespace  (1000)        0 2023-06-16 09:27:29.663660 python-pdfbox-v2-2.0.28.4/tests/
+-rw-rw-rw-   0 codespace  (1000) codespace  (1000)    24649 2023-06-06 10:20:56.000000 python-pdfbox-v2-2.0.28.4/tests/test space.pdf
+-rw-rw-rw-   0 codespace  (1000) codespace  (1000)       71 2023-06-06 10:20:56.000000 python-pdfbox-v2-2.0.28.4/tests/test.md
+-rw-rw-rw-   0 codespace  (1000) codespace  (1000)    24649 2023-06-06 10:20:56.000000 python-pdfbox-v2-2.0.28.4/tests/test.pdf
+-rw-rw-rw-   0 codespace  (1000) codespace  (1000)     2830 2023-06-06 10:20:56.000000 python-pdfbox-v2-2.0.28.4/tests/test2.pdf
+-rw-rw-rw-   0 codespace  (1000) codespace  (1000)    84980 2023-06-06 10:20:56.000000 python-pdfbox-v2-2.0.28.4/tests/test3.pdf
+-rw-rw-rw-   0 codespace  (1000) codespace  (1000)     1798 2023-06-06 10:20:56.000000 python-pdfbox-v2-2.0.28.4/tests/test_pdfbox.py
```

### Comparing `python-pdfbox-v2-2.0.28.3/LICENSE.rst` & `python-pdfbox-v2-2.0.28.4/LICENSE.rst`

 * *Files identical despite different names*

### Comparing `python-pdfbox-v2-2.0.28.3/PKG-INFO` & `python-pdfbox-v2-2.0.28.4/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: python-pdfbox-v2
-Version: 2.0.28.3
+Version: 2.0.28.4
 Summary: Python interface to Apache PDFBox command-line tools.
 Home-page: https://github.com/py-hacks/python-pdfbox
 Author: Fakabbir Amin
 Author-email: f4amin@gmail.com
 License: Apache
 Classifier: Development Status :: 3 - Alpha
 Classifier: Environment :: Console
```

### Comparing `python-pdfbox-v2-2.0.28.3/README.rst` & `python-pdfbox-v2-2.0.28.4/README.rst`

 * *Files identical despite different names*

### Comparing `python-pdfbox-v2-2.0.28.3/pdfbox/__init__.py` & `python-pdfbox-v2-2.0.28.4/pdfbox/__init__.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,43 +1,18 @@
 #!/usr/bin/python3
 
 """
 Python interface to Apache PDFBox.
 """
 
-import hashlib
-import html.parser
 import os
 import pathlib
-import re
-import shutil
-import urllib.request
-
-import appdirs
 import jpype
 import jpype.imports
-import pkg_resources
-
-
-class _PDFBoxVersionsParser(html.parser.HTMLParser):
-    """
-    Class for parsing versions available on PDFBox archive site.
-    """
 
-    def feed(self, data):
-        self.result = []
-        super(_PDFBoxVersionsParser, self).feed(data)
-
-    def handle_starttag(self, tag, attrs):
-        if tag == 'a':
-            for a in attrs:
-                if a[0] == 'href':
-                    s = a[1].strip('/')
-                    if re.search('\d+\.\d+\.\d+.*', s):
-                        self.result.append(s)
 
 class PDFBox(object):
     """
     Python interface to Apache PDFBox.
 
     Methods
     -------
@@ -51,24 +26,14 @@
                   page=None, dpi=None, color=None, cropbox=None, time=True)
         Extract all pages of PDF file as images.
     extract_images(input_path, password=None, prefix=None,
                    directJPEG=False)
         Extract all images from a PDF file.
     """
 
-    def _verify_sha512(self, data, digest):
-        """
-        Verify SHA512 checksum.
-        """
-
-        return hashlib.sha512(data).hexdigest() == digest
-
-    def _get_compatible_pdfbox_url(self):
-        return pdfbox_2_0_27_url
-
     def _get_pdfbox_path(self):
         """
         Return path to local copy of PDFBox jar file.
         """
 
         # Use PDFBOX environmental variable if it exists:
         if 'PDFBOX' in os.environ:
```

### Comparing `python-pdfbox-v2-2.0.28.3/pdfbox/pdfbox-app-2.0.28.jar` & `python-pdfbox-v2-2.0.28.4/pdfbox/pdfbox-app-2.0.28.jar`

 * *Files identical despite different names*

### Comparing `python-pdfbox-v2-2.0.28.3/python_pdfbox_v2.egg-info/PKG-INFO` & `python-pdfbox-v2-2.0.28.4/python_pdfbox_v2.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: python-pdfbox-v2
-Version: 2.0.28.3
+Version: 2.0.28.4
 Summary: Python interface to Apache PDFBox command-line tools.
 Home-page: https://github.com/py-hacks/python-pdfbox
 Author: Fakabbir Amin
 Author-email: f4amin@gmail.com
 License: Apache
 Classifier: Development Status :: 3 - Alpha
 Classifier: Environment :: Console
```

### Comparing `python-pdfbox-v2-2.0.28.3/setup.py` & `python-pdfbox-v2-2.0.28.4/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 import os
 import re
 
 from setuptools import find_packages
 from setuptools import setup
 
 NAME =               'python-pdfbox-v2'
-VERSION =            '2.0.28.3'
+VERSION =            '2.0.28.4'
 AUTHOR =             'Fakabbir Amin'
 AUTHOR_EMAIL =       'f4amin@gmail.com'
 URL =                'https://github.com/py-hacks/python-pdfbox'
 DESCRIPTION =        'Python interface to Apache PDFBox command-line tools.'
 with open('README.rst', 'r') as f:
     LONG_DESCRIPTION = f.read()
 LONG_DESCRIPTION = re.search('.*(^Package Description.*)', LONG_DESCRIPTION, re.MULTILINE|re.DOTALL).group(1)
```

### Comparing `python-pdfbox-v2-2.0.28.3/tests/test space.pdf` & `python-pdfbox-v2-2.0.28.4/tests/test space.pdf`

 * *Files identical despite different names*

### Comparing `python-pdfbox-v2-2.0.28.3/tests/test.pdf` & `python-pdfbox-v2-2.0.28.4/tests/test.pdf`

 * *Files identical despite different names*

### Comparing `python-pdfbox-v2-2.0.28.3/tests/test2.pdf` & `python-pdfbox-v2-2.0.28.4/tests/test2.pdf`

 * *Files identical despite different names*

### Comparing `python-pdfbox-v2-2.0.28.3/tests/test3.pdf` & `python-pdfbox-v2-2.0.28.4/tests/test3.pdf`

 * *Files identical despite different names*

### Comparing `python-pdfbox-v2-2.0.28.3/tests/test_pdfbox.py` & `python-pdfbox-v2-2.0.28.4/tests/test_pdfbox.py`

 * *Files identical despite different names*

