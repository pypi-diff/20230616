# Comparing `tmp/gtki_module_exex-0.0.4-py3-none-any.whl.zip` & `tmp/gtki_module_exex-0.0.5-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,13 +1,13 @@
-Zip file size: 6283 bytes, number of entries: 11
+Zip file size: 6291 bytes, number of entries: 11
 -rw-rw-rw-  2.0 fat        0 b- defN 22-Jun-09 04:59 gtki_module_exex/__init__.py
--rw-rw-rw-  2.0 fat     6319 b- defN 23-Jun-16 14:34 gtki_module_exex/main.py
+-rw-rw-rw-  2.0 fat     6335 b- defN 23-Jun-16 14:54 gtki_module_exex/main.py
 -rw-rw-rw-  2.0 fat     1431 b- defN 23-Jun-15 14:51 gtki_module_exex/mixins.py
 -rw-rw-rw-  2.0 fat        0 b- defN 22-Jun-09 05:22 gtki_module_exex/tests/__init__.py
 -rw-rw-rw-  2.0 fat     2319 b- defN 23-Jun-16 14:37 gtki_module_exex/tests/main_tests.py
 -rw-rw-rw-  2.0 fat     1007 b- defN 22-Jun-09 05:55 gtki_module_exex/tests/mixins_tests.py
--rw-rw-rw-  2.0 fat     1091 b- defN 23-Jun-16 14:40 gtki_module_exex-0.0.4.dist-info/LICENSE
--rw-rw-rw-  2.0 fat      279 b- defN 23-Jun-16 14:40 gtki_module_exex-0.0.4.dist-info/METADATA
--rw-rw-rw-  2.0 fat       92 b- defN 23-Jun-16 14:40 gtki_module_exex-0.0.4.dist-info/WHEEL
--rw-rw-rw-  2.0 fat       17 b- defN 23-Jun-16 14:40 gtki_module_exex-0.0.4.dist-info/top_level.txt
--rw-rw-r--  2.0 fat      952 b- defN 23-Jun-16 14:40 gtki_module_exex-0.0.4.dist-info/RECORD
-11 files, 13507 bytes uncompressed, 4645 bytes compressed:  65.6%
+-rw-rw-rw-  2.0 fat     1091 b- defN 23-Jun-16 14:54 gtki_module_exex-0.0.5.dist-info/LICENSE
+-rw-rw-rw-  2.0 fat      279 b- defN 23-Jun-16 14:54 gtki_module_exex-0.0.5.dist-info/METADATA
+-rw-rw-rw-  2.0 fat       92 b- defN 23-Jun-16 14:54 gtki_module_exex-0.0.5.dist-info/WHEEL
+-rw-rw-rw-  2.0 fat       17 b- defN 23-Jun-16 14:54 gtki_module_exex-0.0.5.dist-info/top_level.txt
+-rw-rw-r--  2.0 fat      952 b- defN 23-Jun-16 14:54 gtki_module_exex-0.0.5.dist-info/RECORD
+11 files, 13523 bytes uncompressed, 4653 bytes compressed:  65.6%
```

## zipnote {}

```diff
@@ -12,23 +12,23 @@
 
 Filename: gtki_module_exex/tests/main_tests.py
 Comment: 
 
 Filename: gtki_module_exex/tests/mixins_tests.py
 Comment: 
 
-Filename: gtki_module_exex-0.0.4.dist-info/LICENSE
+Filename: gtki_module_exex-0.0.5.dist-info/LICENSE
 Comment: 
 
-Filename: gtki_module_exex-0.0.4.dist-info/METADATA
+Filename: gtki_module_exex-0.0.5.dist-info/METADATA
 Comment: 
 
-Filename: gtki_module_exex-0.0.4.dist-info/WHEEL
+Filename: gtki_module_exex-0.0.5.dist-info/WHEEL
 Comment: 
 
-Filename: gtki_module_exex-0.0.4.dist-info/top_level.txt
+Filename: gtki_module_exex-0.0.5.dist-info/top_level.txt
 Comment: 
 
-Filename: gtki_module_exex-0.0.4.dist-info/RECORD
+Filename: gtki_module_exex-0.0.5.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## gtki_module_exex/main.py

```diff
@@ -123,15 +123,15 @@
     def create_document(self, day=None):
         if not day:
             day = datetime.datetime.now()
         self.create_day_header(day.strftime("%#d/%m/%Y"))
         self.set_column_width()
         start_row = self.set_column_names()
         start_row += 1
-        for tc in ["ТКО", "ПО", "Хвосты"]:
+        for tc in ["ТКО", "ПО", "Хвосты", "Прочее"]:
             start_row = self.operate_trash_cat(tc, day.strftime("%Y.%m.%d"), start_row=start_row)
             if start_row:
                 start_row += 2
         self.workbook.close()
 
     def set_column_names(self):
         col_num = 0
```

## Comparing `gtki_module_exex-0.0.4.dist-info/LICENSE` & `gtki_module_exex-0.0.5.dist-info/LICENSE`

 * *Files identical despite different names*

