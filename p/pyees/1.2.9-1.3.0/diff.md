# Comparing `tmp/pyees-1.2.9.tar.gz` & `tmp/pyees-1.3.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pyees-1.2.9.tar", last modified: Thu Jun 15 11:42:07 2023, max compression
+gzip compressed data, was "pyees-1.3.0.tar", last modified: Fri Jun 16 06:36:49 2023, max compression
```

## Comparing `pyees-1.2.9.tar` & `pyees-1.3.0.tar`

### file list

```diff
@@ -1,29 +1,29 @@
-drwxrwxrwx   0        0        0        0 2023-06-15 11:42:07.318090 pyees-1.2.9/
--rw-rw-rw-   0        0        0     1085 2022-02-05 11:46:00.000000 pyees-1.2.9/LICENSE.txt
--rw-rw-rw-   0        0        0      768 2023-06-15 11:42:07.333715 pyees-1.2.9/PKG-INFO
--rw-rw-rw-   0        0        0     1017 2023-03-10 10:19:19.000000 pyees-1.2.9/README.md
-drwxrwxrwx   0        0        0        0 2023-06-15 11:42:07.052459 pyees-1.2.9/pyees/
--rw-rw-rw-   0        0        0      320 2023-05-12 12:42:57.000000 pyees-1.2.9/pyees/__init__.py
--rw-rw-rw-   0        0        0    12841 2023-05-16 05:19:59.000000 pyees-1.2.9/pyees/fit.py
--rw-rw-rw-   0        0        0      811 2023-04-03 12:11:18.000000 pyees-1.2.9/pyees/profilePyees.py
--rw-rw-rw-   0        0        0     9126 2023-05-11 09:38:14.000000 pyees-1.2.9/pyees/prop.py
--rw-rw-rw-   0        0        0    17718 2023-05-12 12:35:32.000000 pyees-1.2.9/pyees/sheet.py
--rw-rw-rw-   0        0        0    10197 2023-05-16 06:21:10.000000 pyees-1.2.9/pyees/solve.py
--rw-rw-rw-   0        0        0     1406 2022-03-24 20:23:42.000000 pyees-1.2.9/pyees/stackOverflowODR.py
--rw-rw-rw-   0        0        0     7669 2023-04-27 10:39:41.000000 pyees-1.2.9/pyees/testFit.py
--rw-rw-rw-   0        0        0    12431 2023-05-11 09:11:30.000000 pyees-1.2.9/pyees/testProp.py
--rw-rw-rw-   0        0        0     1044 2023-05-12 12:42:48.000000 pyees-1.2.9/pyees/testPyees.py
--rw-rw-rw-   0        0        0    15668 2023-05-12 12:42:26.000000 pyees-1.2.9/pyees/testSheet.py
--rw-rw-rw-   0        0        0    20218 2023-04-05 08:10:48.000000 pyees-1.2.9/pyees/testSolve.py
--rw-rw-rw-   0        0        0     9094 2023-05-12 06:37:13.000000 pyees-1.2.9/pyees/testUnit.py
--rw-rw-rw-   0        0        0    82221 2023-06-15 11:40:52.000000 pyees-1.2.9/pyees/testVariable.py
--rw-rw-rw-   0        0        0    44623 2023-06-15 11:34:25.000000 pyees-1.2.9/pyees/unit.py
--rw-rw-rw-   0        0        0    35132 2023-06-15 11:40:28.000000 pyees-1.2.9/pyees/variable.py
-drwxrwxrwx   0        0        0        0 2023-06-15 11:42:07.271214 pyees-1.2.9/pyees.egg-info/
--rw-rw-rw-   0        0        0      768 2023-06-15 11:42:05.000000 pyees-1.2.9/pyees.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      471 2023-06-15 11:42:05.000000 pyees-1.2.9/pyees.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-06-15 11:42:05.000000 pyees-1.2.9/pyees.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       40 2023-06-15 11:42:05.000000 pyees-1.2.9/pyees.egg-info/requires.txt
--rw-rw-rw-   0        0        0        6 2023-06-15 11:42:05.000000 pyees-1.2.9/pyees.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       86 2023-06-15 11:42:07.349341 pyees-1.2.9/setup.cfg
--rw-rw-rw-   0        0        0     1224 2023-06-15 11:41:54.000000 pyees-1.2.9/setup.py
+drwxrwxrwx   0        0        0        0 2023-06-16 06:36:49.895972 pyees-1.3.0/
+-rw-rw-rw-   0        0        0     1085 2022-02-05 11:46:00.000000 pyees-1.3.0/LICENSE.txt
+-rw-rw-rw-   0        0        0      768 2023-06-16 06:36:49.911600 pyees-1.3.0/PKG-INFO
+-rw-rw-rw-   0        0        0     1017 2023-03-10 10:19:19.000000 pyees-1.3.0/README.md
+drwxrwxrwx   0        0        0        0 2023-06-16 06:36:49.677206 pyees-1.3.0/pyees/
+-rw-rw-rw-   0        0        0      320 2023-05-12 12:42:57.000000 pyees-1.3.0/pyees/__init__.py
+-rw-rw-rw-   0        0        0    12841 2023-05-16 05:19:59.000000 pyees-1.3.0/pyees/fit.py
+-rw-rw-rw-   0        0        0      811 2023-04-03 12:11:18.000000 pyees-1.3.0/pyees/profilePyees.py
+-rw-rw-rw-   0        0        0     9126 2023-05-11 09:38:14.000000 pyees-1.3.0/pyees/prop.py
+-rw-rw-rw-   0        0        0    17755 2023-06-16 06:36:14.000000 pyees-1.3.0/pyees/sheet.py
+-rw-rw-rw-   0        0        0    10197 2023-05-16 06:21:10.000000 pyees-1.3.0/pyees/solve.py
+-rw-rw-rw-   0        0        0     1406 2022-03-24 20:23:42.000000 pyees-1.3.0/pyees/stackOverflowODR.py
+-rw-rw-rw-   0        0        0     7669 2023-04-27 10:39:41.000000 pyees-1.3.0/pyees/testFit.py
+-rw-rw-rw-   0        0        0    12431 2023-05-11 09:11:30.000000 pyees-1.3.0/pyees/testProp.py
+-rw-rw-rw-   0        0        0     1044 2023-05-12 12:42:48.000000 pyees-1.3.0/pyees/testPyees.py
+-rw-rw-rw-   0        0        0    15668 2023-05-12 12:42:26.000000 pyees-1.3.0/pyees/testSheet.py
+-rw-rw-rw-   0        0        0    20218 2023-04-05 08:10:48.000000 pyees-1.3.0/pyees/testSolve.py
+-rw-rw-rw-   0        0        0     9094 2023-05-12 06:37:13.000000 pyees-1.3.0/pyees/testUnit.py
+-rw-rw-rw-   0        0        0    82221 2023-06-15 11:40:52.000000 pyees-1.3.0/pyees/testVariable.py
+-rw-rw-rw-   0        0        0    44623 2023-06-15 11:34:25.000000 pyees-1.3.0/pyees/unit.py
+-rw-rw-rw-   0        0        0    35132 2023-06-15 11:40:28.000000 pyees-1.3.0/pyees/variable.py
+drwxrwxrwx   0        0        0        0 2023-06-16 06:36:49.849095 pyees-1.3.0/pyees.egg-info/
+-rw-rw-rw-   0        0        0      768 2023-06-16 06:36:48.000000 pyees-1.3.0/pyees.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      471 2023-06-16 06:36:48.000000 pyees-1.3.0/pyees.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-06-16 06:36:48.000000 pyees-1.3.0/pyees.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       40 2023-06-16 06:36:48.000000 pyees-1.3.0/pyees.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        6 2023-06-16 06:36:48.000000 pyees-1.3.0/pyees.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       86 2023-06-16 06:36:49.942852 pyees-1.3.0/setup.cfg
+-rw-rw-rw-   0        0        0     1224 2023-06-16 06:36:37.000000 pyees-1.3.0/setup.py
```

### Comparing `pyees-1.2.9/LICENSE.txt` & `pyees-1.3.0/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `pyees-1.2.9/PKG-INFO` & `pyees-1.3.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyees
-Version: 1.2.9
+Version: 1.3.0
 Summary: EES but for python. Pyees can be used do perform uncertanty (error) propagation. Furthermore, it can solve nonlinear systems of equations and look up material properties.
 Home-page: https://github.com/jacobv95/pyees
 Download-URL: https://github.com/jacobv95/pyees/archive/refs/tags/v1.0.tar.gz
 Author: Jacob Vestergaard
 Author-email: jacobvestergaard95@gmail.com
 License: MIT
 Keywords: python,data processing,uncertanty,EES
```

### Comparing `pyees-1.2.9/README.md` & `pyees-1.3.0/README.md`

 * *Files identical despite different names*

### Comparing `pyees-1.2.9/pyees/fit.py` & `pyees-1.3.0/pyees/fit.py`

 * *Files identical despite different names*

### Comparing `pyees-1.2.9/pyees/profilePyees.py` & `pyees-1.3.0/pyees/profilePyees.py`

 * *Files identical despite different names*

### Comparing `pyees-1.2.9/pyees/prop.py` & `pyees-1.3.0/pyees/prop.py`

 * *Files identical despite different names*

### Comparing `pyees-1.2.9/pyees/sheet.py` & `pyees-1.3.0/pyees/sheet.py`

 * *Files 0% similar despite different names*

```diff
@@ -224,29 +224,31 @@
         num = 0
         for c in col:
             if c in string.ascii_letters:
                 num = num * 26 + (ord(c.upper()) - ord('A')) + 1
         return num
 
     def formatHeaders(self, header):
+
         out = []
         for head in header:
             if head is None:
                 out.append('')
                 continue
             # remove symbols and replace with _
             head = re.sub(r'[^\w]', '_', head)
-
+            
             # remove multiple consequtive _
             done = False
             a = head
             while not done:
                 b = a.replace('__', '_')
                 if a == b:
                     done = True
+                a = b
 
             # add "_" to the begining of the name if the first letter is a digit
             if head[0].isnumeric():
                 head = '_' + head
 
             # remove "_" if the last letter is "_"
             if head[-1] == "_" and len(head) != 1:
```

### Comparing `pyees-1.2.9/pyees/solve.py` & `pyees-1.3.0/pyees/solve.py`

 * *Files identical despite different names*

### Comparing `pyees-1.2.9/pyees/stackOverflowODR.py` & `pyees-1.3.0/pyees/stackOverflowODR.py`

 * *Files identical despite different names*

### Comparing `pyees-1.2.9/pyees/testFit.py` & `pyees-1.3.0/pyees/testFit.py`

 * *Files identical despite different names*

### Comparing `pyees-1.2.9/pyees/testProp.py` & `pyees-1.3.0/pyees/testProp.py`

 * *Files identical despite different names*

### Comparing `pyees-1.2.9/pyees/testPyees.py` & `pyees-1.3.0/pyees/testPyees.py`

 * *Files identical despite different names*

### Comparing `pyees-1.2.9/pyees/testSheet.py` & `pyees-1.3.0/pyees/testSheet.py`

 * *Files identical despite different names*

### Comparing `pyees-1.2.9/pyees/testSolve.py` & `pyees-1.3.0/pyees/testSolve.py`

 * *Files identical despite different names*

### Comparing `pyees-1.2.9/pyees/testUnit.py` & `pyees-1.3.0/pyees/testUnit.py`

 * *Files identical despite different names*

### Comparing `pyees-1.2.9/pyees/testVariable.py` & `pyees-1.3.0/pyees/testVariable.py`

 * *Files identical despite different names*

### Comparing `pyees-1.2.9/pyees/unit.py` & `pyees-1.3.0/pyees/unit.py`

 * *Files identical despite different names*

### Comparing `pyees-1.2.9/pyees/variable.py` & `pyees-1.3.0/pyees/variable.py`

 * *Files identical despite different names*

### Comparing `pyees-1.2.9/pyees.egg-info/PKG-INFO` & `pyees-1.3.0/pyees.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyees
-Version: 1.2.9
+Version: 1.3.0
 Summary: EES but for python. Pyees can be used do perform uncertanty (error) propagation. Furthermore, it can solve nonlinear systems of equations and look up material properties.
 Home-page: https://github.com/jacobv95/pyees
 Download-URL: https://github.com/jacobv95/pyees/archive/refs/tags/v1.0.tar.gz
 Author: Jacob Vestergaard
 Author-email: jacobvestergaard95@gmail.com
 License: MIT
 Keywords: python,data processing,uncertanty,EES
```

### Comparing `pyees-1.2.9/setup.py` & `pyees-1.3.0/setup.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from distutils.core import setup
 setup(
     name='pyees',
     packages=['pyees'],
-    version='1.2.9',
+    version='1.3.0',
     license='MIT',
     description='EES but for python. Pyees can be used do perform uncertanty (error) propagation. Furthermore, it can solve nonlinear systems of equations and look up material properties.',
     author='Jacob Vestergaard',
     author_email='jacobvestergaard95@gmail.com',
     url='https://github.com/jacobv95/pyees',
     download_url='https://github.com/jacobv95/pyees/archive/refs/tags/v1.0.tar.gz',
     keywords=['python', 'data processing', 'uncertanty', 'EES'],
```

