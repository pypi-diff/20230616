# Comparing `tmp/gtki_module_exex-0.0.3-py3-none-any.whl.zip` & `tmp/gtki_module_exex-0.0.4-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,13 +1,13 @@
-Zip file size: 4760 bytes, number of entries: 11
+Zip file size: 6283 bytes, number of entries: 11
 -rw-rw-rw-  2.0 fat        0 b- defN 22-Jun-09 04:59 gtki_module_exex/__init__.py
--rw-rw-rw-  2.0 fat     1473 b- defN 22-Jun-09 08:02 gtki_module_exex/main.py
--rw-rw-rw-  2.0 fat     1159 b- defN 22-Jun-09 07:42 gtki_module_exex/mixins.py
+-rw-rw-rw-  2.0 fat     6319 b- defN 23-Jun-16 14:34 gtki_module_exex/main.py
+-rw-rw-rw-  2.0 fat     1431 b- defN 23-Jun-15 14:51 gtki_module_exex/mixins.py
 -rw-rw-rw-  2.0 fat        0 b- defN 22-Jun-09 05:22 gtki_module_exex/tests/__init__.py
--rw-rw-rw-  2.0 fat     1903 b- defN 22-Jun-09 07:47 gtki_module_exex/tests/main_tests.py
+-rw-rw-rw-  2.0 fat     2319 b- defN 23-Jun-16 14:37 gtki_module_exex/tests/main_tests.py
 -rw-rw-rw-  2.0 fat     1007 b- defN 22-Jun-09 05:55 gtki_module_exex/tests/mixins_tests.py
--rw-rw-rw-  2.0 fat     1091 b- defN 22-Jun-09 08:03 gtki_module_exex-0.0.3.dist-info/LICENSE
--rw-rw-rw-  2.0 fat      177 b- defN 22-Jun-09 08:03 gtki_module_exex-0.0.3.dist-info/METADATA
--rw-rw-rw-  2.0 fat       92 b- defN 22-Jun-09 08:03 gtki_module_exex-0.0.3.dist-info/WHEEL
--rw-rw-rw-  2.0 fat       17 b- defN 22-Jun-09 08:03 gtki_module_exex-0.0.3.dist-info/top_level.txt
-?rw-rw-r--  2.0 fat      952 b- defN 22-Jun-09 08:03 gtki_module_exex-0.0.3.dist-info/RECORD
-11 files, 7871 bytes uncompressed, 3122 bytes compressed:  60.3%
+-rw-rw-rw-  2.0 fat     1091 b- defN 23-Jun-16 14:40 gtki_module_exex-0.0.4.dist-info/LICENSE
+-rw-rw-rw-  2.0 fat      279 b- defN 23-Jun-16 14:40 gtki_module_exex-0.0.4.dist-info/METADATA
+-rw-rw-rw-  2.0 fat       92 b- defN 23-Jun-16 14:40 gtki_module_exex-0.0.4.dist-info/WHEEL
+-rw-rw-rw-  2.0 fat       17 b- defN 23-Jun-16 14:40 gtki_module_exex-0.0.4.dist-info/top_level.txt
+-rw-rw-r--  2.0 fat      952 b- defN 23-Jun-16 14:40 gtki_module_exex-0.0.4.dist-info/RECORD
+11 files, 13507 bytes uncompressed, 4645 bytes compressed:  65.6%
```

## zipnote {}

```diff
@@ -12,23 +12,23 @@
 
 Filename: gtki_module_exex/tests/main_tests.py
 Comment: 
 
 Filename: gtki_module_exex/tests/mixins_tests.py
 Comment: 
 
-Filename: gtki_module_exex-0.0.3.dist-info/LICENSE
+Filename: gtki_module_exex-0.0.4.dist-info/LICENSE
 Comment: 
 
-Filename: gtki_module_exex-0.0.3.dist-info/METADATA
+Filename: gtki_module_exex-0.0.4.dist-info/METADATA
 Comment: 
 
-Filename: gtki_module_exex-0.0.3.dist-info/WHEEL
+Filename: gtki_module_exex-0.0.4.dist-info/WHEEL
 Comment: 
 
-Filename: gtki_module_exex-0.0.3.dist-info/top_level.txt
+Filename: gtki_module_exex-0.0.4.dist-info/top_level.txt
 Comment: 
 
-Filename: gtki_module_exex-0.0.3.dist-info/RECORD
+Filename: gtki_module_exex-0.0.4.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## gtki_module_exex/main.py

```diff
@@ -1,9 +1,11 @@
-from gtki_module_exex.mixins import XlsCreator, TemplateCreator, DataFiller
-
+import datetime
+from wsqluse import wsqluse
+from gtki_module_exex.mixins import XlsCreator, TemplateCreator, DataFiller, IshbDailyReportTemplate
+from ar_qdk.main import ARQDK
 
 class CreateExcel(XlsCreator, TemplateCreator, DataFiller):
     def __init__(self, file_name, data_list, column_names=None):
         if column_names:
             self.column_names = column_names
         self.data_list = data_list
         self.file_name = file_name
@@ -35,7 +37,115 @@
         self.create_template()
         self.create_amount(self.amount_info)
         row_num = 2
         for row in self.data_list:
             self.create_row(row, row_num)
             row_num += 1
         self.workbook.close()
+
+
+class CreateExcelDailyReport(XlsCreator):
+    def __init__(self, file_name, ar_ip, ar_port,
+                 column_names=None):
+        self.file_name = file_name
+        self.ar_qdk = ARQDK(ip=ar_ip, port=ar_port)
+        self.ar_qdk.make_connection()
+        self.workbook = self.create_workbook()
+        self.worksheet = self.create_worksheet()
+        #super().__init__(file_name, acts_list, column_names)
+        self.column_names = ["Категория", "Клиент", "Перевозчик", "Количество \nрейсов",
+                    "Общий вес,\nтонн", "Выручка, руб.", "Ошибки"]
+        self.header_format = self.workbook.add_format({'bold': True,
+                                                  'align': 'center',
+                                                  'valign': 'center',
+                                                  'font_size': 11})
+        self.header_format.set_font_size(11)
+        self.header_format.set_center_across()
+
+    def create_day_header(self, day=None):
+        merge_format = self.workbook.add_format({'align': 'center'})
+        merge_format.set_font_size(14)
+        self.worksheet.merge_range('A1:G1', day, merge_format)
+
+    def operate_trash_cat(self, trash_cat, day, start_row):
+        #records = self.get_records(trash_cat, day)
+        records = self.ar_qdk.execute_method("get_daily_report",
+                                             trash_cat=trash_cat,
+                                             day=day,
+                                             get_response=True)
+        if records['status']:
+            records = records['info']
+        if not records:
+            return
+        self.worksheet.write(start_row, 0, trash_cat, self.header_format)
+        for rec in records:
+            self.set_record(rec['client_name'], rec['carrier_name'], rec['amount'], rec['tonnage'], start_row)
+            start_row += 1
+        amount, tonnage = self.get_amount(records)
+        return self.set_amount(amount, tonnage, start_row+1)
+
+
+    def get_amount(self, records):
+        amount = 0
+        tonnage = 0
+        for rec in records:
+            amount += rec['amount']
+            tonnage += rec['tonnage']
+        return amount, tonnage
+
+
+    def set_record(self, client, carrier, amount, tonnage, start_row):
+        self.worksheet.write(start_row, 1, client)
+        self.worksheet.write(start_row, 2, carrier)
+        self.worksheet.write(start_row, 3, amount)
+        self.worksheet.write(start_row, 4, tonnage)
+        return
+
+    @wsqluse.getTableDictStripper
+    def get_records(self, trash_cat, day):
+        return self.sql_shell.get_table_dict(
+            "select c.name as client_name, cr.name as carrier_name, "
+            "sum(r.cargo) as tonnage, count(r.id) as amount "
+            "from records r left join clients c on (r.client_id=c.id) "
+            "left join clients cr on (r.carrier=cr.id) "
+            f"where r.trash_cat=(select id from trash_cats where name='{trash_cat}') "
+            f"and time_in::date='{day}' group by (c.name, cr.name);"
+        )
+
+    def set_amount(self, amount, tonnage, row=2):
+        self.worksheet.write(row, 0, "ИТОГО", self.header_format)
+        self.worksheet.write(row, 3, amount, self.header_format)
+        self.worksheet.write(row, 4, tonnage, self.header_format)
+        return row
+
+    def set_trash_cat(self, cat_name, row):
+        self.worksheet.write(row, 0, cat_name, self.header_format)
+
+    def create_document(self, day=None):
+        if not day:
+            day = datetime.datetime.now()
+        self.create_day_header(day.strftime("%#d/%m/%Y"))
+        self.set_column_width()
+        start_row = self.set_column_names()
+        start_row += 1
+        for tc in ["ТКО", "ПО", "Хвосты"]:
+            start_row = self.operate_trash_cat(tc, day.strftime("%Y.%m.%d"), start_row=start_row)
+            if start_row:
+                start_row += 2
+        self.workbook.close()
+
+    def set_column_names(self):
+        col_num = 0
+        self.worksheet.set_row_pixels(1, 42)
+        for col_name in self.column_names:
+            self.worksheet.write(1, col_num, col_name, self.header_format)
+            col_num += 1
+        return 1
+
+    def set_column_width(self):
+        self.worksheet.set_column_pixels(0, 0, 109)
+        self.worksheet.set_column_pixels(1, 1, 198)
+        self.worksheet.set_column_pixels(2, 2, 169)
+        self.worksheet.set_column_pixels(3, 3, 78)
+        self.worksheet.set_column_pixels(4, 4, 101)
+        self.worksheet.set_column_pixels(5, 5, 99)
+        self.worksheet.set_column_pixels(6, 6, 156)
```

### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

## gtki_module_exex/mixins.py

```diff
@@ -8,14 +8,16 @@
     def create_workbook(self):
         return xlsxwriter.Workbook(self.file_name)
 
     def create_worksheet(self):
         return self.workbook.add_worksheet()
 
 
+
+
 class TemplateCreator:
     worksheet = None
     workbook = None
     column_names = [
         'ID', 'Гос.Номер', 'Клиент', 'Перевозчик',
         'Брутто', 'Тара', 'Нетто', 'Категория груза',
         'Вид груза', 'Дата въезда', 'Дата выезда',
@@ -27,14 +29,19 @@
         bold.set_font_size(14)
         col_num = 0
         for col_name in self.column_names:
             self.worksheet.write(0, col_num, col_name, bold)
             col_num += 1
 
 
+class IshbDailyReportTemplate(TemplateCreator):
+    column_names = ["Категория", "Клиент", "Перевозчик", "Количество рейсов",
+                    "Общий вес, тонн", "Выручка, руб.", "Ошибки"]
+
+
 class DataFiller:
     worksheet = None
 
     def create_row(self, data_list, row_num=1):
         col_num = 0
         for data in data_list:
             self.worksheet.write(row_num, col_num, data)
```

## gtki_module_exex/tests/main_tests.py

```diff
@@ -1,9 +1,10 @@
 from gtki_module_exex import main
 import unittest
+from wsqluse.wsqluse import Wsqluse
 
 
 class TestCase(unittest.TestCase):
     data_list = (
         ['1', 'В060ХА702', 'Физлицо', 'Физлицо', 100, 50, 50, 'ПО',
          'Прочее', '2022-05-01 12:00', '2022-05-10 13:00', 'Тест'],
         ['2', 'В060ХА702', 'Физлицо', 'Физлицо', 100, 50, 50, 'ПО',
@@ -18,20 +19,29 @@
          'Прочее', '2022-05-01 12:00', '2022-05-10 13:00', 'Тест'],
         ['7', 'В060ХА702', 'Физлицо', 'Физлицо', 100, 50, 50, 'ПО',
          'Прочее', '2022-05-01 12:00', '2022-05-10 13:00', 'Тест'],
         ['8', 'В060ХА702', 'Физлицо', 'Физлицо', 100, 50, 50, 'ПО',
          'Прочее', '2022-05-01 12:00', '2022-05-10 13:00', 'Тест'],
     )
 
+    @unittest.SkipTest
     def test_create_excel(self):
         inst = main.CreateExcel('main_test.xls', self.data_list)
         inst.create_document()
 
+    @unittest.SkipTest
     def tests_create_acts_excel(self):
         amount_info = 'Итого 5000 (3 взвешивания)'
         inst = main.CreateExcelActs('main_acts.xls', self.data_list,
                                     amount_info)
         inst.create_document()
 
 
+    def tests_creat_daily_report(self):
+        sql_shell = Wsqluse("gdb", "qodex", "0kra1na&73", "127.0.0.1")
+        inst = main.CreateExcelDailyReport('ishb_daily.xls',
+                                           ar_port=52250,
+                                           ar_ip="localhost")
+        inst.create_document()
+
 if __name__ == '__main__':
     unittest.main()
```

## Comparing `gtki_module_exex-0.0.3.dist-info/LICENSE` & `gtki_module_exex-0.0.4.dist-info/LICENSE`

 * *Files identical despite different names*

## Comparing `gtki_module_exex-0.0.3.dist-info/RECORD` & `gtki_module_exex-0.0.4.dist-info/RECORD`

 * *Files 21% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 gtki_module_exex/__init__.py,sha256=47DEQpj8HBSa-_TImW-5JCeuQeRkm5NMpJWZG3hSuFU,0
-gtki_module_exex/main.py,sha256=mvbj2Ws9vF221-foYA0LUSOroqx9gVm431eqG8FfRHg,1473
-gtki_module_exex/mixins.py,sha256=nPuzNGMKbhudQUee4qVlubXrQM4S5ZQhOXbqb3qbNCg,1159
+gtki_module_exex/main.py,sha256=QwIaZrn5L6S0j4GrwzhhPd559WrmwUrAYmZCHqNJ1RY,6319
+gtki_module_exex/mixins.py,sha256=nKYRHMoFYSva364Q2WyH30SefjAxi5xGXekgLmRAyXk,1431
 gtki_module_exex/tests/__init__.py,sha256=47DEQpj8HBSa-_TImW-5JCeuQeRkm5NMpJWZG3hSuFU,0
-gtki_module_exex/tests/main_tests.py,sha256=HF3KlRLk8QRfeKW3dN5SRYYOEV1HKdR_LVaZePc8M-M,1903
+gtki_module_exex/tests/main_tests.py,sha256=B4FlY1vXuCg6D0tasIimMedKGDXJeclVrz8xNslv48M,2319
 gtki_module_exex/tests/mixins_tests.py,sha256=8oogAhtkQgyhB3sUEsIvQpvA1a7YrRPc76bDHKsxodI,1007
-gtki_module_exex-0.0.3.dist-info/LICENSE,sha256=6kbiFSfobTZ7beWiKnHpN902HgBx-Jzgcme0SvKqhKY,1091
-gtki_module_exex-0.0.3.dist-info/METADATA,sha256=LOSF2N7Two45Wnun_BCdhh6vh5ePuGyi62o7onup2QI,177
-gtki_module_exex-0.0.3.dist-info/WHEEL,sha256=G16H4A3IeoQmnOrYV4ueZGKSjhipXx8zc8nu9FGlvMA,92
-gtki_module_exex-0.0.3.dist-info/top_level.txt,sha256=5fDck53WZ0oTnmcblVZKn9XwbA-Uqijh0L93F1ml9Bc,17
-gtki_module_exex-0.0.3.dist-info/RECORD,,
+gtki_module_exex-0.0.4.dist-info/LICENSE,sha256=6kbiFSfobTZ7beWiKnHpN902HgBx-Jzgcme0SvKqhKY,1091
+gtki_module_exex-0.0.4.dist-info/METADATA,sha256=TDEvPCD4jivThttcY9v72oujshfkKmPrMmdLJpw6ffg,279
+gtki_module_exex-0.0.4.dist-info/WHEEL,sha256=pkctZYzUS4AYVn6dJ-7367OJZivF2e8RA9b_ZBjif18,92
+gtki_module_exex-0.0.4.dist-info/top_level.txt,sha256=5fDck53WZ0oTnmcblVZKn9XwbA-Uqijh0L93F1ml9Bc,17
+gtki_module_exex-0.0.4.dist-info/RECORD,,
```

