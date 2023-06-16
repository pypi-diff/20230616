# Comparing `tmp/digital_unit-1.6b0.tar.gz` & `tmp/digital_unit-1.6b1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "digital_unit-1.6b0.tar", last modified: Sun May 28 08:18:06 2023, max compression
+gzip compressed data, was "digital_unit-1.6b1.tar", last modified: Fri Jun 16 13:47:32 2023, max compression
```

## Comparing `digital_unit-1.6b0.tar` & `digital_unit-1.6b1.tar`

### file list

```diff
@@ -1,18 +1,19 @@
-drwxrwxrwx   0        0        0        0 2023-05-28 08:18:06.072172 digital_unit-1.6b0/
--rw-rw-rw-   0        0        0     1668 2023-05-28 08:18:06.072172 digital_unit-1.6b0/PKG-INFO
--rw-rw-rw-   0        0        0     1383 2023-05-28 08:12:19.000000 digital_unit-1.6b0/README.md
-drwxrwxrwx   0        0        0        0 2023-05-28 08:18:06.054184 digital_unit-1.6b0/digital_unit/
--rw-rw-rw-   0        0        0     1166 2023-05-28 08:07:32.000000 digital_unit-1.6b0/digital_unit/Area.py
--rw-rw-rw-   0        0        0      925 2023-05-28 08:08:29.000000 digital_unit-1.6b0/digital_unit/Lenth.py
--rw-rw-rw-   0        0        0      570 2023-05-28 08:17:58.000000 digital_unit-1.6b0/digital_unit/Temperature.py
--rw-rw-rw-   0        0        0     1159 2023-05-28 08:06:54.000000 digital_unit-1.6b0/digital_unit/Volume.py
--rw-rw-rw-   0        0        0      209 2023-05-28 07:44:32.000000 digital_unit-1.6b0/digital_unit/__init__.py
--rw-rw-rw-   0        0        0     1115 2023-05-28 08:05:25.000000 digital_unit-1.6b0/digital_unit/root.py
--rw-rw-rw-   0        0        0      330 2023-05-28 08:11:42.000000 digital_unit-1.6b0/digital_unit/sample.py
-drwxrwxrwx   0        0        0        0 2023-05-28 08:18:06.068171 digital_unit-1.6b0/digital_unit.egg-info/
--rw-rw-rw-   0        0        0     1668 2023-05-28 08:18:05.000000 digital_unit-1.6b0/digital_unit.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      358 2023-05-28 08:18:05.000000 digital_unit-1.6b0/digital_unit.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-05-28 08:18:05.000000 digital_unit-1.6b0/digital_unit.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       13 2023-05-28 08:18:05.000000 digital_unit-1.6b0/digital_unit.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       86 2023-05-28 08:18:06.074171 digital_unit-1.6b0/setup.cfg
--rw-rw-rw-   0        0        0      956 2023-05-28 08:09:55.000000 digital_unit-1.6b0/setup.py
+drwxrwxrwx   0        0        0        0 2023-06-16 13:47:32.213064 digital_unit-1.6b1/
+-rw-rw-rw-   0        0        0     1080 2023-06-16 13:35:10.000000 digital_unit-1.6b1/LICENSE
+-rw-rw-rw-   0        0        0     1697 2023-06-16 13:47:32.215060 digital_unit-1.6b1/PKG-INFO
+-rw-rw-rw-   0        0        0     1389 2023-06-16 13:43:19.000000 digital_unit-1.6b1/README.md
+drwxrwxrwx   0        0        0        0 2023-06-16 13:47:32.136201 digital_unit-1.6b1/digital_unit/
+-rw-rw-rw-   0        0        0     1166 2023-06-16 13:35:10.000000 digital_unit-1.6b1/digital_unit/Area.py
+-rw-rw-rw-   0        0        0      925 2023-06-16 13:35:10.000000 digital_unit-1.6b1/digital_unit/Lenth.py
+-rw-rw-rw-   0        0        0      570 2023-06-16 13:35:10.000000 digital_unit-1.6b1/digital_unit/Temperature.py
+-rw-rw-rw-   0        0        0     1159 2023-06-16 13:35:10.000000 digital_unit-1.6b1/digital_unit/Volume.py
+-rw-rw-rw-   0        0        0      141 2023-06-16 13:41:50.000000 digital_unit-1.6b1/digital_unit/__init__.py
+-rw-rw-rw-   0        0        0     1115 2023-06-16 13:35:10.000000 digital_unit-1.6b1/digital_unit/root.py
+-rw-rw-rw-   0        0        0      330 2023-06-16 13:35:10.000000 digital_unit-1.6b1/digital_unit/sample.py
+drwxrwxrwx   0        0        0        0 2023-06-16 13:47:32.199084 digital_unit-1.6b1/digital_unit.egg-info/
+-rw-rw-rw-   0        0        0     1697 2023-06-16 13:47:31.000000 digital_unit-1.6b1/digital_unit.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      343 2023-06-16 13:47:31.000000 digital_unit-1.6b1/digital_unit.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-06-16 13:47:31.000000 digital_unit-1.6b1/digital_unit.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       13 2023-06-16 13:47:31.000000 digital_unit-1.6b1/digital_unit.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       86 2023-06-16 13:47:32.221051 digital_unit-1.6b1/setup.cfg
+-rw-rw-rw-   0        0        0      956 2023-06-16 13:41:54.000000 digital_unit-1.6b1/setup.py
```

### Comparing `digital_unit-1.6b0/PKG-INFO` & `digital_unit-1.6b1/digital_unit.egg-info/PKG-INFO`

 * *Files 13% similar despite different names*

```diff
@@ -1,19 +1,20 @@
 Metadata-Version: 2.1
-Name: digital_unit
-Version: 1.6b0
+Name: digital-unit
+Version: 1.6b1
 Summary: number and units
 Author: st201109
 Author-email: st20110913@outlook.com
 License: MIT
 Keywords: SOME,MEANINGFULL,MATH
 Classifier: Programming Language :: Python :: 3.6
 Description-Content-Type: text/markdown
+License-File: LICENSE
 
-# 包 digital_unit 1.6
+# 包 digital_unit 1.6b1
 （language：Chinese）
 
 这是一个有关**数据的单位**的包,如长度、面积、体积等，可以用它来表示一个数量的单位
 使用示例
 ``` python
 from digital_unit import CentiMeter,MilliMeter, Number
 
@@ -21,21 +22,21 @@
 if __name__ == '__main__':
     _1cm = Number(1.0, CentiMeter()) # Create the data. Don't forget the parentheses!
     print(_1cm)
     _1cm.change_unit(MilliMeter()) # Changes to the unit. Don't forget the parentheses!
     print(_1cm)
 ```
 使用`Number(NUMBER, UNIT())`来创建实例，使用`XXX.change_unit(NEWUNIT())`来修改单位。
-## 1.6版本新增
-Temperature(温度系列)
+## 1.6b1版本新增
+修改了导入方式。
 
-## 1.6版本修正
+## 1.6b1版本修正
 无
 
-# package digital_unit 1.6
+# package digital_unit 1.6b1
 (language: English)
 
 This is **a unit of data** related to packages, such as length, area, volume, etc., it can be used to represent a number of units
 Use the sample
 ```python
 from digital_unit import CentiMeter, MilliMeter, Number
 
@@ -43,12 +44,12 @@
 _1cm = Number(1.0,CentiMeter()) # Create the data. Don 't forget the parentheses.
 print(_1cm)
 _1cm.Change_unit(MilliMeter()) #Changes to the unit. Don 't forget the parentheses.
 print(_1cm)
 ```
 Using ` Number(NUBER, UNIT()) ` to create an instance, use ` XXX.Change_unit(NEWUNIT ()) ` to modify the UNIT
 
-## Added in version 1.6
-Temperature (Temperature series)
+## Added in version 1.6b1
+Modified the import method.
 
-## Corrected in version 1.6
+## Corrected in version 1.6b1
 None
```

### Comparing `digital_unit-1.6b0/README.md` & `digital_unit-1.6b1/README.md`

 * *Files 13% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# 包 digital_unit 1.6
+# 包 digital_unit 1.6b1
 （language：Chinese）
 
 这是一个有关**数据的单位**的包,如长度、面积、体积等，可以用它来表示一个数量的单位
 使用示例
 ``` python
 from digital_unit import CentiMeter,MilliMeter, Number
 
@@ -10,21 +10,21 @@
 if __name__ == '__main__':
     _1cm = Number(1.0, CentiMeter()) # Create the data. Don't forget the parentheses!
     print(_1cm)
     _1cm.change_unit(MilliMeter()) # Changes to the unit. Don't forget the parentheses!
     print(_1cm)
 ```
 使用`Number(NUMBER, UNIT())`来创建实例，使用`XXX.change_unit(NEWUNIT())`来修改单位。
-## 1.6版本新增
-Temperature(温度系列)
+## 1.6b1版本新增
+修改了导入方式。
 
-## 1.6版本修正
+## 1.6b1版本修正
 无
 
-# package digital_unit 1.6
+# package digital_unit 1.6b1
 (language: English)
 
 This is **a unit of data** related to packages, such as length, area, volume, etc., it can be used to represent a number of units
 Use the sample
 ```python
 from digital_unit import CentiMeter, MilliMeter, Number
 
@@ -32,12 +32,12 @@
 _1cm = Number(1.0,CentiMeter()) # Create the data. Don 't forget the parentheses.
 print(_1cm)
 _1cm.Change_unit(MilliMeter()) #Changes to the unit. Don 't forget the parentheses.
 print(_1cm)
 ```
 Using ` Number(NUBER, UNIT()) ` to create an instance, use ` XXX.Change_unit(NEWUNIT ()) ` to modify the UNIT
 
-## Added in version 1.6
-Temperature (Temperature series)
+## Added in version 1.6b1
+Modified the import method.
 
-## Corrected in version 1.6
+## Corrected in version 1.6b1
 None
```

### Comparing `digital_unit-1.6b0/digital_unit/Area.py` & `digital_unit-1.6b1/digital_unit/Area.py`

 * *Files identical despite different names*

### Comparing `digital_unit-1.6b0/digital_unit/Lenth.py` & `digital_unit-1.6b1/digital_unit/Lenth.py`

 * *Files identical despite different names*

### Comparing `digital_unit-1.6b0/digital_unit/Temperature.py` & `digital_unit-1.6b1/digital_unit/Temperature.py`

 * *Files identical despite different names*

### Comparing `digital_unit-1.6b0/digital_unit/Volume.py` & `digital_unit-1.6b1/digital_unit/Volume.py`

 * *Files identical despite different names*

### Comparing `digital_unit-1.6b0/digital_unit/root.py` & `digital_unit-1.6b1/digital_unit/root.py`

 * *Files identical despite different names*

### Comparing `digital_unit-1.6b0/digital_unit.egg-info/PKG-INFO` & `digital_unit-1.6b1/PKG-INFO`

 * *Files 23% similar despite different names*

```diff
@@ -1,19 +1,20 @@
 Metadata-Version: 2.1
-Name: digital-unit
-Version: 1.6b0
+Name: digital_unit
+Version: 1.6b1
 Summary: number and units
 Author: st201109
 Author-email: st20110913@outlook.com
 License: MIT
 Keywords: SOME,MEANINGFULL,MATH
 Classifier: Programming Language :: Python :: 3.6
 Description-Content-Type: text/markdown
+License-File: LICENSE
 
-# 包 digital_unit 1.6
+# 包 digital_unit 1.6b1
 （language：Chinese）
 
 这是一个有关**数据的单位**的包,如长度、面积、体积等，可以用它来表示一个数量的单位
 使用示例
 ``` python
 from digital_unit import CentiMeter,MilliMeter, Number
 
@@ -21,21 +22,21 @@
 if __name__ == '__main__':
     _1cm = Number(1.0, CentiMeter()) # Create the data. Don't forget the parentheses!
     print(_1cm)
     _1cm.change_unit(MilliMeter()) # Changes to the unit. Don't forget the parentheses!
     print(_1cm)
 ```
 使用`Number(NUMBER, UNIT())`来创建实例，使用`XXX.change_unit(NEWUNIT())`来修改单位。
-## 1.6版本新增
-Temperature(温度系列)
+## 1.6b1版本新增
+修改了导入方式。
 
-## 1.6版本修正
+## 1.6b1版本修正
 无
 
-# package digital_unit 1.6
+# package digital_unit 1.6b1
 (language: English)
 
 This is **a unit of data** related to packages, such as length, area, volume, etc., it can be used to represent a number of units
 Use the sample
 ```python
 from digital_unit import CentiMeter, MilliMeter, Number
 
@@ -43,12 +44,12 @@
 _1cm = Number(1.0,CentiMeter()) # Create the data. Don 't forget the parentheses.
 print(_1cm)
 _1cm.Change_unit(MilliMeter()) #Changes to the unit. Don 't forget the parentheses.
 print(_1cm)
 ```
 Using ` Number(NUBER, UNIT()) ` to create an instance, use ` XXX.Change_unit(NEWUNIT ()) ` to modify the UNIT
 
-## Added in version 1.6
-Temperature (Temperature series)
+## Added in version 1.6b1
+Modified the import method.
 
-## Corrected in version 1.6
+## Corrected in version 1.6b1
 None
```

### Comparing `digital_unit-1.6b0/setup.py` & `digital_unit-1.6b1/setup.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 from distutils.core import setup
 with open("README.md", "r", encoding="utf-8") as fh:
     long_description = fh.read()
 setup(
   name = 'digital_unit',         # How you named your package folder (MyLib)
   packages = ['digital_unit'],   # Chose the same as "name"
-  version = '1.6b0',      # Start with a small number and increase it with every change you make
+  version = '1.6b1',      # Start with a small number and increase it with every change you make
   license='MIT',        # Chose a license from here: https://help.github.com/articles/licensing-a-repository
   description = 'number and units',   # Give a short description about your library
   author = 'st201109',                   # Type in your name
   author_email = 'st20110913@outlook.com',      # Type in your E-Mail
   
   keywords = ['SOME', 'MEANINGFULL', 'MATH'],   # Keywords that define your package best
   long_description = long_description,
```

