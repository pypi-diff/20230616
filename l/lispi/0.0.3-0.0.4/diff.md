# Comparing `tmp/lispi-0.0.3.tar.gz` & `tmp/lispi-0.0.4.tar.gz`

## Comparing `lispi-0.0.3.tar` & `lispi-0.0.4.tar`

### file list

```diff
@@ -1,20 +1,20 @@
--rw-r--r--   0        0        0     6148 2020-02-02 00:00:00.000000 lispi-0.0.3/.DS_Store
--rw-r--r--   0        0        0       32 2020-02-02 00:00:00.000000 lispi-0.0.3/MANIFEST.in
--rw-r--r--   0        0        0     6461 2020-02-02 00:00:00.000000 lispi-0.0.3/requirements.txt
--rw-r--r--   0        0        0     6148 2020-02-02 00:00:00.000000 lispi-0.0.3/example/.DS_Store
--rw-r--r--   0        0        0    11232 2020-02-02 00:00:00.000000 lispi-0.0.3/example/original_example.ipynb
--rw-r--r--   0        0        0     8196 2020-02-02 00:00:00.000000 lispi-0.0.3/src/.DS_Store
--rw-r--r--   0        0        0     6148 2020-02-02 00:00:00.000000 lispi-0.0.3/src/lispi/.DS_Store
--rw-r--r--   0        0        0      146 2020-02-02 00:00:00.000000 lispi-0.0.3/src/lispi/__init__.py
--rw-r--r--   0        0        0     2311 2020-02-02 00:00:00.000000 lispi-0.0.3/src/lispi/__main__.py
--rw-r--r--   0        0        0      489 2020-02-02 00:00:00.000000 lispi-0.0.3/src/lispi/revealjs_template.py
--rw-r--r--   0        0        0     4420 2020-02-02 00:00:00.000000 lispi-0.0.3/src/lispi/slideEdit.py
--rw-r--r--   0        0        0     1746 2020-02-02 00:00:00.000000 lispi-0.0.3/src/lispi/text2audio.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 lispi-0.0.3/tests/test_audioText.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 lispi-0.0.3/tests/test_nbconvert.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 lispi-0.0.3/tests/test_pyscript.py
--rw-r--r--   0        0        0        6 2020-02-02 00:00:00.000000 lispi-0.0.3/.gitignore
--rw-r--r--   0        0        0     1073 2020-02-02 00:00:00.000000 lispi-0.0.3/LICENSE
--rw-r--r--   0        0        0     2255 2020-02-02 00:00:00.000000 lispi-0.0.3/README.md
--rw-r--r--   0        0        0     1236 2020-02-02 00:00:00.000000 lispi-0.0.3/pyproject.toml
--rw-r--r--   0        0        0     4197 2020-02-02 00:00:00.000000 lispi-0.0.3/PKG-INFO
+-rw-r--r--   0        0        0     6148 2020-02-02 00:00:00.000000 lispi-0.0.4/.DS_Store
+-rw-r--r--   0        0        0       32 2020-02-02 00:00:00.000000 lispi-0.0.4/MANIFEST.in
+-rw-r--r--   0        0        0     6461 2020-02-02 00:00:00.000000 lispi-0.0.4/requirements.txt
+-rw-r--r--   0        0        0     6148 2020-02-02 00:00:00.000000 lispi-0.0.4/example/.DS_Store
+-rw-r--r--   0        0        0     1707 2020-02-02 00:00:00.000000 lispi-0.0.4/example/original_example.ipynb
+-rw-r--r--   0        0        0     8196 2020-02-02 00:00:00.000000 lispi-0.0.4/src/.DS_Store
+-rw-r--r--   0        0        0     6148 2020-02-02 00:00:00.000000 lispi-0.0.4/src/lispi/.DS_Store
+-rw-r--r--   0        0        0      118 2020-02-02 00:00:00.000000 lispi-0.0.4/src/lispi/__init__.py
+-rw-r--r--   0        0        0     2319 2020-02-02 00:00:00.000000 lispi-0.0.4/src/lispi/__main__.py
+-rw-r--r--   0        0        0      489 2020-02-02 00:00:00.000000 lispi-0.0.4/src/lispi/revealjs_template.py
+-rw-r--r--   0        0        0     4422 2020-02-02 00:00:00.000000 lispi-0.0.4/src/lispi/slideEdit.py
+-rw-r--r--   0        0        0     1746 2020-02-02 00:00:00.000000 lispi-0.0.4/src/lispi/text2audio.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 lispi-0.0.4/tests/test_audioText.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 lispi-0.0.4/tests/test_nbconvert.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 lispi-0.0.4/tests/test_pyscript.py
+-rw-r--r--   0        0        0        6 2020-02-02 00:00:00.000000 lispi-0.0.4/.gitignore
+-rw-r--r--   0        0        0     1073 2020-02-02 00:00:00.000000 lispi-0.0.4/LICENSE
+-rw-r--r--   0        0        0     2255 2020-02-02 00:00:00.000000 lispi-0.0.4/README.md
+-rw-r--r--   0        0        0     1234 2020-02-02 00:00:00.000000 lispi-0.0.4/pyproject.toml
+-rw-r--r--   0        0        0     4197 2020-02-02 00:00:00.000000 lispi-0.0.4/PKG-INFO
```

### Comparing `lispi-0.0.3/.DS_Store` & `lispi-0.0.4/.DS_Store`

 * *Files 1% similar despite different names*

```diff
@@ -67,16 +67,16 @@
 00000420: 7370 626c 6f62 0000 00b8 6270 6c69 7374  spblob....bplist
 00000430: 3030 d601 0203 0405 0607 0807 080b 085d  00.............]
 00000440: 5368 6f77 5374 6174 7573 4261 725b 5368  ShowStatusBar[Sh
 00000450: 6f77 546f 6f6c 6261 725b 5368 6f77 5461  owToolbar[ShowTa
 00000460: 6256 6965 775f 1014 436f 6e74 6169 6e65  bView_..Containe
 00000470: 7253 686f 7753 6964 6562 6172 5c57 696e  rShowSidebar\Win
 00000480: 646f 7742 6f75 6e64 735b 5368 6f77 5369  dowBounds[ShowSi
-00000490: 6465 6261 7208 0908 095f 1018 7b7b 3330  debar...._..{{30
-000004a0: 352c 2032 3339 7d2c 207b 3932 302c 2034  5, 239}, {920, 4
+00000490: 6465 6261 7208 0908 095f 1018 7b7b 3335  debar...._..{{35
+000004a0: 372c 2031 3436 7d2c 207b 3932 302c 2034  7, 146}, {920, 4
 000004b0: 3336 7d7d 0908 1523 2f3b 525f 6b6c 6d6e  36}}...#/;R_klmn
 000004c0: 6f8a 0000 0000 0000 0101 0000 0000 0000  o...............
 000004d0: 000d 0000 0000 0000 0000 0000 0000 0000  ................
 000004e0: 008b 0000 0007 0065 0078 0061 006d 0070  .......e.x.a.m.p
 000004f0: 006c 0065 7653 726e 6c6f 6e67 0000 0001  .l.evSrnlong....
 00000500: 0000 0007 004c 0049 0043 0045 004e 0053  .....L.I.C.E.N.S
 00000510: 0045 496c 6f63 626c 6f62 0000 0010 0000  .EIlocblob......
```

### Comparing `lispi-0.0.3/requirements.txt` & `lispi-0.0.4/requirements.txt`

 * *Files identical despite different names*

### Comparing `lispi-0.0.3/example/.DS_Store` & `lispi-0.0.4/example/.DS_Store`

 * *Files identical despite different names*

### Comparing `lispi-0.0.3/src/.DS_Store` & `lispi-0.0.4/src/.DS_Store`

 * *Files 18% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 00000000: 0000 0001 4275 6431 0000 1800 0000 0800  ....Bud1........
 00000010: 0000 1800 0000 100b 0000 0000 0000 0000  ................
 00000020: 0000 0000 0000 0000 0000 0000 0000 0800  ................
 00000030: 0000 0800 0000 0000 0000 0000 0000 0000  ................
 00000040: 0000 0000 0000 0002 0000 0000 0000 000c  ................
-00000050: 0000 0001 0000 1000 0079 496c 6f63 626c  .........yIlocbl
+00000050: 0000 0001 0000 1000 0069 496c 6f63 626c  .........iIlocbl
 00000060: 6f62 0000 0000 0000 0000 0000 0000 0000  ob..............
 00000070: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 00000080: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 00000090: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 000000a0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 000000b0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 000000c0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
@@ -251,31 +251,31 @@
 00000fa0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 00000fb0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 00000fc0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 00000fd0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 00000fe0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 00000ff0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 00001000: 0000 0000 0000 0000 0000 000c 0000 0005  ................
-00001010: 006c 0069 0073 0070 0079 496c 6f63 626c  .l.i.s.p.yIlocbl
+00001010: 006c 0069 0073 0070 0069 496c 6f63 626c  .l.i.s.p.iIlocbl
 00001020: 6f62 0000 0010 0000 0041 0000 002e ffff  ob.......A......
 00001030: ffff ffff 0000 0000 0005 006c 0069 0073  ...........l.i.s
-00001040: 0070 0079 6277 7370 626c 6f62 0000 00b7  .p.ybwspblob....
+00001040: 0070 0069 6277 7370 626c 6f62 0000 00b7  .p.ibwspblob....
 00001050: 6270 6c69 7374 3030 d601 0203 0405 0607  bplist00........
 00001060: 0807 080b 085d 5368 6f77 5374 6174 7573  .....]ShowStatus
 00001070: 4261 725b 5368 6f77 546f 6f6c 6261 725b  Bar[ShowToolbar[
 00001080: 5368 6f77 5461 6256 6965 775f 1014 436f  ShowTabView_..Co
 00001090: 6e74 6169 6e65 7253 686f 7753 6964 6562  ntainerShowSideb
 000010a0: 6172 5c57 696e 646f 7742 6f75 6e64 735b  ar\WindowBounds[
 000010b0: 5368 6f77 5369 6465 6261 7208 0908 095f  ShowSidebar...._
 000010c0: 1017 7b7b 3838 2c20 3231 337d 2c20 7b39  ..{{88, 213}, {9
 000010d0: 3230 2c20 3433 367d 7d09 0815 232f 3b52  20, 436}}...#/;R
 000010e0: 5f6b 6c6d 6e6f 8900 0000 0000 0001 0100  _klmno..........
 000010f0: 0000 0000 0000 0d00 0000 0000 0000 0000  ................
 00001100: 0000 0000 0000 8a00 0000 0500 6c00 6900  ............l.i.
-00001110: 7300 7000 7969 6376 7062 6c6f 6200 0001  s.p.yicvpblob...
+00001110: 7300 7000 6969 6376 7062 6c6f 6200 0001  s.p.iicvpblob...
 00001120: 9462 706c 6973 7430 30de 0102 0304 0506  .bplist00.......
 00001130: 0708 090a 0b0c 0d0e 0f10 110f 120f 1313  ................
 00001140: 1415 1617 1619 5f10 1362 6163 6b67 726f  ......_..backgro
 00001150: 756e 6443 6f6c 6f72 426c 7565 5b67 7269  undColorBlue[gri
 00001160: 6453 7061 6369 6e67 5874 6578 7453 697a  dSpacingXtextSiz
 00001170: 655f 1012 6261 636b 6772 6f75 6e64 436f  e_..backgroundCo
 00001180: 6c6f 7252 6564 5e62 6163 6b67 726f 756e  lorRed^backgroun
@@ -294,15 +294,15 @@
 00001250: 0109 546e 616d 6509 2340 5000 0000 0000  ..Tname.#@P.....
 00001260: 0000 0800 2500 3b00 4700 5000 6500 7400  ....%.;.G.P.e.t.
 00001270: 8b00 9700 a300 b000 c500 d300 dd00 ef00  ................
 00001280: f801 0101 0a01 1301 1501 1e01 1f01 3001  ..............0.
 00001290: 3101 3601 3700 0000 0000 0002 0100 0000  1.6.7...........
 000012a0: 0000 0000 1a00 0000 0000 0000 0000 0000  ................
 000012b0: 0000 0001 4000 0000 0500 6c00 6900 7300  ....@.....l.i.s.
-000012c0: 7000 7976 5372 6e6c 6f6e 6700 0000 0100  p.yvSrnlong.....
+000012c0: 7000 6976 5372 6e6c 6f6e 6700 0000 0100  p.ivSrnlong.....
 000012d0: 0000 0900 6e00 6500 7700 2e00 6900 7000  ....n.e.w...i.p.
 000012e0: 7900 6e00 6249 6c6f 6362 6c6f 6200 0000  y.n.bIlocblob...
 000012f0: 1000 0001 1d00 0000 2eff ffff ffff ff00  ................
 00001300: 0000 0000 0f00 6e00 6500 7700 2e00 7300  ......n.e.w...s.
 00001310: 6c00 6900 6400 6500 7300 2e00 6800 7400  l.i.d.e.s...h.t.
 00001320: 6d00 6c49 6c6f 6362 6c6f 6200 0000 1000  m.lIlocblob.....
 00001330: 0001 8b00 0000 2eff ffff ffff ff00 0000  ................
```

### Comparing `lispi-0.0.3/src/lispi/.DS_Store` & `lispi-0.0.4/src/lispi/.DS_Store`

 * *Files identical despite different names*

### Comparing `lispi-0.0.3/src/lispi/__main__.py` & `lispi-0.0.4/src/lispi/__main__.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,52 +1,54 @@
 import os
 import subprocess
 import jupyter
 import shutil
+import pkg_resources
 import lispi
-from lispi import text2audio, slideEdit, revealjs_template
+from lispi import *
 
 def main():
     index = input("Enter the name of the notebook file: \n")
     if os.path.isfile(index+".ipynb"):
         text2audio.text2audio(index+".ipynb")
         revealjs_template.convert('nbconvert')
         subprocess.run(["jupyter", "nbconvert", index+".ipynb", "--to", "slides"])
         slideEdit._ess(index)
     elif index=="original_example":
         class Showcase:
             def __init__(self, index):
                 self._name = index
             def get_file(self):
-                examples_dir = os.path.join('example')
+                examples_dir = pkg_resources.resource_filename('lispi', '../../example/original_example.ipynb')
                 if not os.path.exists(os.path.join(os.getcwd(), 'output')):
                     os.makedirs(os.path.join(os.getcwd(), 'output'))
-                example_file_path = os.path.join(examples_dir, 'original_example.ipynb')
-                shutil.copy(example_file_path, os.getcwd())
-                self.example_file_path = os.path.join(os.getcwd(),'original_example.ipynb')
-                return self.example_file_path
+                shutil.copy(examples_dir, os.getcwd())
+                self.examples_dir = os.getcwd()
+                return self.examples_dir
         
         
-        example_file_path=Showcase(index).get_file()
-        text2audio.text2audio(example_file_path)
+        examples_dir=Showcase(index).get_file()
+        text2audio.text2audio(examples_dir+"/original_example.ipynb")
         revealjs_template.convert('nbconvert')
-        subprocess.run(["jupyter", "nbconvert", example_file_path, "--to", "slides"])
-        slideEdit._ess(os.path.join(examples_dir, 'original_example'))
-        source_file = os.path.join(examples_dir, 'original_example_ess.html')
-        destination_folder = "./output/"
+        subprocess.run(["jupyter", "nbconvert", examples_dir+"/original_example.ipynb", "--to", "slides"])
+        slideEdit._ess("original_example")
+        source_file = os.path.join(examples_dir, 'original_example_lispi.html')
+        destination_folder = "./output"
         _files = os.listdir(destination_folder)
         print(_files)
         for f in _files:
             item=os.path.join(destination_folder, f)
             print(item)
             if os.path.isfile(item):
                 os.remove(item)
             elif os.path.isdir(item):
                 shutil.rmtree(item)
-        
+                
+        os.remove("original_example.ipynb")
+        os.remove("original_example.slides.html")
         shutil.move(source_file, destination_folder)
         shutil.move(os.path.join(examples_dir, 'slides_audios'), destination_folder)
     else:
         print("\n")
         print(f"\"{index}.ipynb\" not found!")
         print("*********************************************")
         print("Make sure you have the notebook and try again!")
```

### Comparing `lispi-0.0.3/src/lispi/slideEdit.py` & `lispi-0.0.4/src/lispi/slideEdit.py`

 * *Files 1% similar despite different names*

```diff
@@ -69,9 +69,9 @@
       p_tag.insert_after(script_tag_pyScript)
       p_tag.insert_after(user_div)
 
 
   # Get the new HTML content
   _html = str(soup)
 
-  with open(notebook_file_name+'_ess.html', 'w') as file:
+  with open(notebook_file_name+'_lispi.html', 'w') as file:
       file.write(_html)
```

### Comparing `lispi-0.0.3/src/lispi/text2audio.py` & `lispi-0.0.4/src/lispi/text2audio.py`

 * *Files identical despite different names*

### Comparing `lispi-0.0.3/LICENSE` & `lispi-0.0.4/LICENSE`

 * *Files identical despite different names*

### Comparing `lispi-0.0.3/README.md` & `lispi-0.0.4/README.md`

 * *Files identical despite different names*

### Comparing `lispi-0.0.3/pyproject.toml` & `lispi-0.0.4/pyproject.toml`

 * *Files 9% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 build-backend = "hatchling.build"
 
 [tool.hatch.include]
 include = [".example/**"]
 
 [project]
 name = "lispi"
-version = "0.0.03"
+version = "0.0.4"
 authors = [
   { name="B7M", email="ibsnetwork001@gmail.com" },
 ]
 license = { file = "LICENSE" }
 description = "A simple python package for generating live notebooks where you can write code and run it in real time."
 readme = "README.md"
 requires-python = ">=3.7"
@@ -38,23 +38,22 @@
 Homepage = "https://github.com/B7M/lispi"
 
 [project.scripts]
 lispi = "lispi.__main__:main"
 
 
 [tool.bumpver]
-current_version = "0.0.03"
-version_pattern = "MAJOR.MINOR.PATCH"
+current_version = "0.0.4"
+version_pattern = "MAJOR.MINOR.PATCH[PYTAGNUM]"
 commit_message = "bump version {old_version} -> {new_version}"
 commit = true
 tag = true
 push = true
 
 [tool.bumpver.file_patterns]
 "pyproject.toml" = [
-    'current_version = "{version}"',
+    'version = "{version}"',
 ]
 "README.md" = [
     "{version}",
     "{pep440_version}",
-]
-
+]
```

### Comparing `lispi-0.0.3/PKG-INFO` & `lispi-0.0.4/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: lispi
-Version: 0.0.3
+Version: 0.0.4
 Summary: A simple python package for generating live notebooks where you can write code and run it in real time.
 Project-URL: Homepage, https://github.com/B7M/lispi
 Author-email: B7M <ibsnetwork001@gmail.com>
 License: Copyright (c) 2023 The Python Packaging Authority
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
         of this software and associated documentation files (the "Software"), to deal
```

