# Comparing `tmp/pp_project_pkg-1.0.202306160150-py3-none-any.whl.zip` & `tmp/pp_project_pkg-1.0.202306160314-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,14 +1,14 @@
-Zip file size: 7972 bytes, number of entries: 12
+Zip file size: 7988 bytes, number of entries: 12
 -rw-rw-r--  2.0 unx       71 b- defN 23-Jun-07 11:24 pp_project_pkg/__init__.py
 -rw-rw-r--  2.0 unx      577 b- defN 23-Jun-07 11:24 pp_project_pkg/newsvendor.py
 -rw-rw-r--  2.0 unx     7115 b- defN 23-Jun-07 11:24 pp_project_pkg/pp_tables.py
--rw-rw-r--  2.0 unx     2955 b- defN 23-Jun-16 01:48 pp_project_pkg/utils.py
--rw-rw-r--  2.0 unx      396 b- defN 23-Jun-16 01:50 pp_project_pkg/version.py
+-rw-rw-r--  2.0 unx     3004 b- defN 23-Jun-16 03:14 pp_project_pkg/utils.py
+-rw-rw-r--  2.0 unx      396 b- defN 23-Jun-16 03:14 pp_project_pkg/version.py
 -rw-rw-r--  2.0 unx     4391 b- defN 23-Jun-16 01:49 pp_project_pkg/wrangling.py
--rwxrwxr-x  2.0 unx       65 b- defN 23-Jun-02 12:43 pp_project_pkg-1.0.202306160150.data/scripts/get_tables.py
--rwxrwxr-x  2.0 unx     1316 b- defN 23-Jun-07 11:24 pp_project_pkg-1.0.202306160150.data/scripts/pp_project_run.py
--rw-rw-r--  2.0 unx      191 b- defN 23-Jun-16 01:52 pp_project_pkg-1.0.202306160150.dist-info/METADATA
--rw-rw-r--  2.0 unx       92 b- defN 23-Jun-16 01:52 pp_project_pkg-1.0.202306160150.dist-info/WHEEL
--rw-rw-r--  2.0 unx       15 b- defN 23-Jun-16 01:52 pp_project_pkg-1.0.202306160150.dist-info/top_level.txt
-?rw-rw-r--  2.0 unx     1095 b- defN 23-Jun-16 01:52 pp_project_pkg-1.0.202306160150.dist-info/RECORD
-12 files, 18279 bytes uncompressed, 6086 bytes compressed:  66.7%
+-rwxrwxr-x  2.0 unx       65 b- defN 23-Jun-02 12:43 pp_project_pkg-1.0.202306160314.data/scripts/get_tables.py
+-rwxrwxr-x  2.0 unx     1316 b- defN 23-Jun-07 11:24 pp_project_pkg-1.0.202306160314.data/scripts/pp_project_run.py
+-rw-rw-r--  2.0 unx      191 b- defN 23-Jun-16 03:15 pp_project_pkg-1.0.202306160314.dist-info/METADATA
+-rw-rw-r--  2.0 unx       92 b- defN 23-Jun-16 03:15 pp_project_pkg-1.0.202306160314.dist-info/WHEEL
+-rw-rw-r--  2.0 unx       15 b- defN 23-Jun-16 03:15 pp_project_pkg-1.0.202306160314.dist-info/top_level.txt
+?rw-rw-r--  2.0 unx     1095 b- defN 23-Jun-16 03:15 pp_project_pkg-1.0.202306160314.dist-info/RECORD
+12 files, 18328 bytes uncompressed, 6102 bytes compressed:  66.7%
```

## zipnote {}

```diff
@@ -12,26 +12,26 @@
 
 Filename: pp_project_pkg/version.py
 Comment: 
 
 Filename: pp_project_pkg/wrangling.py
 Comment: 
 
-Filename: pp_project_pkg-1.0.202306160150.data/scripts/get_tables.py
+Filename: pp_project_pkg-1.0.202306160314.data/scripts/get_tables.py
 Comment: 
 
-Filename: pp_project_pkg-1.0.202306160150.data/scripts/pp_project_run.py
+Filename: pp_project_pkg-1.0.202306160314.data/scripts/pp_project_run.py
 Comment: 
 
-Filename: pp_project_pkg-1.0.202306160150.dist-info/METADATA
+Filename: pp_project_pkg-1.0.202306160314.dist-info/METADATA
 Comment: 
 
-Filename: pp_project_pkg-1.0.202306160150.dist-info/WHEEL
+Filename: pp_project_pkg-1.0.202306160314.dist-info/WHEEL
 Comment: 
 
-Filename: pp_project_pkg-1.0.202306160150.dist-info/top_level.txt
+Filename: pp_project_pkg-1.0.202306160314.dist-info/top_level.txt
 Comment: 
 
-Filename: pp_project_pkg-1.0.202306160150.dist-info/RECORD
+Filename: pp_project_pkg-1.0.202306160314.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## pp_project_pkg/utils.py

```diff
@@ -1,12 +1,12 @@
 import wml.visionml as wv
 import datetime
 import mb.pandas as pd
 
-__all__ = ['site_date_res','check_if_valid_date']
+__all__ = ['site_date_res','check_if_valid_date','check_report_close_date','create_date_table']
 
 
 def site_date_res(site_id= 30607):
     """
     Get the site date report closure data
     Args:
         site_id : Site id for fetching the date wise result. Site_id : 30607 (Waldof)
@@ -55,15 +55,15 @@
     Output:
         pd.DataFrame
     """    
     date_index = pd.date_range(start=start_date, end=end_date, freq='D')
     df = pd.DataFrame({'datetime': date_index.date,'closed':None})
     return df
 
-def check_if_valid_dates(site_res,start_date='2023-06-06', end_date='2023-12-31'):
+def check_report_close_date(site_res,start_date='2023-06-06', end_date='2023-12-31'):
     """
     Check if the dates has closed the report.
 
     Args:
         site_res: complete report of the site_data_res
         date: string value of date. format : '2023-06-06'.
         today: string value of today's date. format : '2023-06-06'
```

## pp_project_pkg/version.py

```diff
@@ -1,11 +1,11 @@
 VERSION_YEAR = 2023
 VERSION_MONTH = int('06')
 VERSION_DAY = int('16')
-VERSION_HOUR = int('01')
-VERSION_MINUTE = int('50')
+VERSION_HOUR = int('03')
+VERSION_MINUTE = int('14')
 MAJOR_VERSION = 1
 MINOR_VERSION = 0
-PATCH_VERSION = 202306160150
-version_date = '2023/06/16 01:50'
+PATCH_VERSION = 202306160314
+version_date = '2023/06/16 03:14'
 version = '{}.{}.{}'.format(MAJOR_VERSION, MINOR_VERSION, PATCH_VERSION)
 __all__  = ['MAJOR_VERSION', 'MINOR_VERSION', 'PATCH_VERSION', 'version_date', 'version']
```

## Comparing `pp_project_pkg-1.0.202306160150.data/scripts/pp_project_run.py` & `pp_project_pkg-1.0.202306160314.data/scripts/pp_project_run.py`

 * *Files identical despite different names*

## Comparing `pp_project_pkg-1.0.202306160150.dist-info/RECORD` & `pp_project_pkg-1.0.202306160314.dist-info/RECORD`

 * *Files 18% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 pp_project_pkg/__init__.py,sha256=9idX2X6SQKZg--ziGy6Ii9OB-kz9hOX1nEG9a0xEW9g,71
 pp_project_pkg/newsvendor.py,sha256=E6JHp0Vtmq63toKM6bO3xTAdCgwmAZzRua-w10wrc5Y,577
 pp_project_pkg/pp_tables.py,sha256=8rqVp4P9nF13UbBmN_R7vGK7MeY4BkeG2ibDa7jLRpg,7115
-pp_project_pkg/utils.py,sha256=1tzGiab-R2zWoFSr-Mq-6yQsne3HAFYTGaNqCnrzRkA,2955
-pp_project_pkg/version.py,sha256=n3uo1qPBIdbom_St2lwgYZ_JfWI4Yv919BZFwPyFEYQ,396
+pp_project_pkg/utils.py,sha256=aRS8ermeFuS_UuJfDMDS5-WB_euxC3pn7eKI8PUgLRY,3004
+pp_project_pkg/version.py,sha256=wIFrj2e1PHhGkpKim9hHp6qbbGpcGnFfm7p2qfMqnaY,396
 pp_project_pkg/wrangling.py,sha256=rTDhW4hNytVSargqNoJlub_wyN37zPElVtKNc2TaRlw,4391
-pp_project_pkg-1.0.202306160150.data/scripts/get_tables.py,sha256=E5FmW2bHAU9NPORQMG85RzGtXOGjjzbATEa5lLGjyk4,65
-pp_project_pkg-1.0.202306160150.data/scripts/pp_project_run.py,sha256=hNrYjtDlo7nX9pwMbM7un9R7ToKRdjVosBt3qErKtaA,1316
-pp_project_pkg-1.0.202306160150.dist-info/METADATA,sha256=APUnZWgwrznnMNiUH2gnvtzcX4pHcbdsa5OA40AFpog,191
-pp_project_pkg-1.0.202306160150.dist-info/WHEEL,sha256=g4nMs7d-Xl9-xC9XovUrsDHGXt-FT0E17Yqo92DEfvY,92
-pp_project_pkg-1.0.202306160150.dist-info/top_level.txt,sha256=2V1bEC5qsYRo1f2gAotX3L3S5xl1nIUxjITUTeRd8yQ,15
-pp_project_pkg-1.0.202306160150.dist-info/RECORD,,
+pp_project_pkg-1.0.202306160314.data/scripts/get_tables.py,sha256=E5FmW2bHAU9NPORQMG85RzGtXOGjjzbATEa5lLGjyk4,65
+pp_project_pkg-1.0.202306160314.data/scripts/pp_project_run.py,sha256=hNrYjtDlo7nX9pwMbM7un9R7ToKRdjVosBt3qErKtaA,1316
+pp_project_pkg-1.0.202306160314.dist-info/METADATA,sha256=0XoDCt9Jmx0eVX1GuU4F-AuWzMRtrDs1-DxF3PuTV6I,191
+pp_project_pkg-1.0.202306160314.dist-info/WHEEL,sha256=g4nMs7d-Xl9-xC9XovUrsDHGXt-FT0E17Yqo92DEfvY,92
+pp_project_pkg-1.0.202306160314.dist-info/top_level.txt,sha256=2V1bEC5qsYRo1f2gAotX3L3S5xl1nIUxjITUTeRd8yQ,15
+pp_project_pkg-1.0.202306160314.dist-info/RECORD,,
```

