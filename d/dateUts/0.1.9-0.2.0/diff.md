# Comparing `tmp/dateUts-0.1.9.tar.gz` & `tmp/dateUts-0.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dateUts-0.1.9.tar", last modified: Wed May  3 14:21:43 2023, max compression
+gzip compressed data, was "dateUts-0.2.0.tar", last modified: Fri Jun 16 18:43:40 2023, max compression
```

## Comparing `dateUts-0.1.9.tar` & `dateUts-0.2.0.tar`

### file list

```diff
@@ -1,17 +1,17 @@
-drwxrwxrwx   0        0        0        0 2023-05-03 14:21:43.112556 dateUts-0.1.9/
--rw-rw-rw-   0        0        0      644 2023-04-26 21:23:08.000000 dateUts-0.1.9/CHANGELOG.txt
--rw-rw-rw-   0        0        0     1058 2023-04-26 21:06:44.000000 dateUts-0.1.9/LICENCE.txt
--rw-rw-rw-   0        0        0       30 2023-04-26 21:06:44.000000 dateUts-0.1.9/MANIFEST.in
--rw-rw-rw-   0        0        0     4331 2023-05-03 14:21:43.111559 dateUts-0.1.9/PKG-INFO
--rw-rw-rw-   0        0        0     3159 2023-04-26 21:06:44.000000 dateUts-0.1.9/README.md
--rw-rw-rw-   0        0        0      122 2023-04-26 21:06:44.000000 dateUts-0.1.9/commands.txt
-drwxrwxrwx   0        0        0        0 2023-05-03 14:21:43.075655 dateUts-0.1.9/dateUts/
--rw-rw-rw-   0        0        0     5835 2023-05-03 14:20:17.000000 dateUts-0.1.9/dateUts/__init__.py
-drwxrwxrwx   0        0        0        0 2023-05-03 14:21:43.110561 dateUts-0.1.9/dateUts.egg-info/
--rw-rw-rw-   0        0        0     4331 2023-05-03 14:21:42.000000 dateUts-0.1.9/dateUts.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      243 2023-05-03 14:21:42.000000 dateUts-0.1.9/dateUts.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-05-03 14:21:42.000000 dateUts-0.1.9/dateUts.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       23 2023-05-03 14:21:42.000000 dateUts-0.1.9/dateUts.egg-info/requires.txt
--rw-rw-rw-   0        0        0        8 2023-05-03 14:21:42.000000 dateUts-0.1.9/dateUts.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-05-03 14:21:43.112556 dateUts-0.1.9/setup.cfg
--rw-rw-rw-   0        0        0      761 2023-05-03 14:21:19.000000 dateUts-0.1.9/setup.py
+drwxrwxrwx   0        0        0        0 2023-06-16 18:43:40.725201 dateUts-0.2.0/
+-rw-rw-rw-   0        0        0      644 2023-04-26 21:23:08.000000 dateUts-0.2.0/CHANGELOG.txt
+-rw-rw-rw-   0        0        0     1058 2023-04-26 21:06:44.000000 dateUts-0.2.0/LICENCE.txt
+-rw-rw-rw-   0        0        0       30 2023-04-26 21:06:44.000000 dateUts-0.2.0/MANIFEST.in
+-rw-rw-rw-   0        0        0     4331 2023-06-16 18:43:40.723206 dateUts-0.2.0/PKG-INFO
+-rw-rw-rw-   0        0        0     3159 2023-04-26 21:06:44.000000 dateUts-0.2.0/README.md
+-rw-rw-rw-   0        0        0      122 2023-04-26 21:06:44.000000 dateUts-0.2.0/commands.txt
+drwxrwxrwx   0        0        0        0 2023-06-16 18:43:40.690295 dateUts-0.2.0/dateUts/
+-rw-rw-rw-   0        0        0     5860 2023-06-16 18:42:07.000000 dateUts-0.2.0/dateUts/__init__.py
+drwxrwxrwx   0        0        0        0 2023-06-16 18:43:40.722209 dateUts-0.2.0/dateUts.egg-info/
+-rw-rw-rw-   0        0        0     4331 2023-06-16 18:43:40.000000 dateUts-0.2.0/dateUts.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      243 2023-06-16 18:43:40.000000 dateUts-0.2.0/dateUts.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-06-16 18:43:40.000000 dateUts-0.2.0/dateUts.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       23 2023-06-16 18:43:40.000000 dateUts-0.2.0/dateUts.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        8 2023-06-16 18:43:40.000000 dateUts-0.2.0/dateUts.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-06-16 18:43:40.725201 dateUts-0.2.0/setup.cfg
+-rw-rw-rw-   0        0        0      761 2023-06-16 18:43:28.000000 dateUts-0.2.0/setup.py
```

### Comparing `dateUts-0.1.9/CHANGELOG.txt` & `dateUts-0.2.0/CHANGELOG.txt`

 * *Files identical despite different names*

### Comparing `dateUts-0.1.9/LICENCE.txt` & `dateUts-0.2.0/LICENCE.txt`

 * *Files identical despite different names*

### Comparing `dateUts-0.1.9/PKG-INFO` & `dateUts-0.2.0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dateUts
-Version: 0.1.9
+Version: 0.2.0
 Summary: Date package
 Home-page: 
 Author: Melque Lima
 Author-email: melque_ex@yahoo.com.br
 License: MIT
 Keywords: dateUts
 Classifier: Development Status :: 5 - Production/Stable
```

### Comparing `dateUts-0.1.9/README.md` & `dateUts-0.2.0/README.md`

 * *Files identical despite different names*

### Comparing `dateUts-0.1.9/dateUts/__init__.py` & `dateUts-0.2.0/dateUts/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -159,30 +159,32 @@
     try:
         dt = datetime.strptime(dt,fmt)
     except ValueError:
         return False
 
     return True
 
-def firstDay(sql_dte:str|date,fmt:str=None):
+def firstDay(sql_dte:date,fmt:str=None):
     dte = sql_dte if isinstance(sql_dte,date) or isinstance(sql_dte,DateUts) else sqlToDate(sql_dte)
     dte = fmtDate(dte,"%Y-%m-01")
     firstDay = sqlToDate(dte)
     return fmtDate(firstDay,fmt)
 
-def lastDay(sql_dte:str|date,fmt:str=None):
+def lastDay(sql_dte:date,fmt:str=None):
     dte = sql_dte if isinstance(sql_dte,date) or isinstance(sql_dte,DateUts) else sqlToDate(sql_dte)
     dte = sqlToDate(dateAdd(dte,1,"month",fmt="%Y-%m-01"))
     dte = dateAdd(dte,-1,"day")
     return fmtDate(dte,fmt)
 
 
 
 Fnc_noWeekends = lambda dt:dt.weekday() not in [5,6]
 
+
+#a = fmtDate("202306","%Y%m")
 #a = dateRange(firstDay(today()).date,lastDay(today()).date,filter_lbd = Fnc_noWeekends)
 #a[0].weekday()
 # a = DateUts(dt.now())
 # print(a)
 # a = lastWorkingDate(fmt="%Y-%m-%d")
 # rng = dateRange(sqlToDate("2022-05-01"),sqlToDate("2022-05-10"))
 # rng = dateRange(sqlToDate("2022-05-10"),sqlToDate("2022-05-01"))
```

### Comparing `dateUts-0.1.9/dateUts.egg-info/PKG-INFO` & `dateUts-0.2.0/dateUts.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dateUts
-Version: 0.1.9
+Version: 0.2.0
 Summary: Date package
 Home-page: 
 Author: Melque Lima
 Author-email: melque_ex@yahoo.com.br
 License: MIT
 Keywords: dateUts
 Classifier: Development Status :: 5 - Production/Stable
```

### Comparing `dateUts-0.1.9/setup.py` & `dateUts-0.2.0/setup.py`

 * *Files 18% similar despite different names*

```diff
@@ -6,15 +6,15 @@
   'Operating System :: Microsoft :: Windows :: Windows 10',
   'License :: OSI Approved :: MIT License',
   'Programming Language :: Python :: 3'
 ]
  
 setup(
   name='dateUts',
-  version='0.1.9',
+  version='0.2.0',
   description='Date package',
   long_description=open('README.md').read() + '\n\n' + open('CHANGELOG.txt').read(),
   long_description_content_type='text/markdown',
   url='',  
   author='Melque Lima',
   author_email='melque_ex@yahoo.com.br',
   license='MIT',
```

