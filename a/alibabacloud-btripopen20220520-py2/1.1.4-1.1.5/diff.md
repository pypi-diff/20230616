# Comparing `tmp/alibabacloud_btripopen20220520_py2-1.1.4.tar.gz` & `tmp/alibabacloud_btripopen20220520_py2-1.1.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/alibabacloud_btripopen20220520_py2-1.1.4.tar", last modified: Thu Jun 15 03:38:12 2023, max compression
+gzip compressed data, was "dist/alibabacloud_btripopen20220520_py2-1.1.5.tar", last modified: Fri Jun 16 07:44:51 2023, max compression
```

## Comparing `alibabacloud_btripopen20220520_py2-1.1.4.tar` & `alibabacloud_btripopen20220520_py2-1.1.5.tar`

### file list

```diff
@@ -1,19 +1,19 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-15 03:38:12.000000 alibabacloud_btripopen20220520_py2-1.1.4/
--rw-r--r--   0 root         (0) root         (0)     3380 2023-06-15 03:38:12.000000 alibabacloud_btripopen20220520_py2-1.1.4/ChangeLog.md
--rw-r--r--   0 root         (0) root         (0)      588 2023-06-15 03:38:12.000000 alibabacloud_btripopen20220520_py2-1.1.4/LICENSE
--rw-r--r--   0 root         (0) root         (0)       28 2023-06-15 03:38:12.000000 alibabacloud_btripopen20220520_py2-1.1.4/MANIFEST.in
--rw-r--r--   0 root         (0) root         (0)     2508 2023-06-15 03:38:12.000000 alibabacloud_btripopen20220520_py2-1.1.4/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     1051 2023-06-15 03:38:12.000000 alibabacloud_btripopen20220520_py2-1.1.4/README-CN.md
--rw-r--r--   0 root         (0) root         (0)     1134 2023-06-15 03:38:12.000000 alibabacloud_btripopen20220520_py2-1.1.4/README.md
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-15 03:38:12.000000 alibabacloud_btripopen20220520_py2-1.1.4/alibabacloud_btripopen20220520/
--rw-r--r--   0 root         (0) root         (0)       21 2023-06-15 03:38:12.000000 alibabacloud_btripopen20220520_py2-1.1.4/alibabacloud_btripopen20220520/__init__.py
--rw-r--r--   0 root         (0) root         (0)   223404 2023-06-15 03:38:12.000000 alibabacloud_btripopen20220520_py2-1.1.4/alibabacloud_btripopen20220520/client.py
--rw-r--r--   0 root         (0) root         (0)  2002899 2023-06-15 03:38:12.000000 alibabacloud_btripopen20220520_py2-1.1.4/alibabacloud_btripopen20220520/models.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-15 03:38:12.000000 alibabacloud_btripopen20220520_py2-1.1.4/alibabacloud_btripopen20220520_py2.egg-info/
--rw-r--r--   0 root         (0) root         (0)     2508 2023-06-15 03:38:12.000000 alibabacloud_btripopen20220520_py2-1.1.4/alibabacloud_btripopen20220520_py2.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      488 2023-06-15 03:38:12.000000 alibabacloud_btripopen20220520_py2-1.1.4/alibabacloud_btripopen20220520_py2.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-06-15 03:38:12.000000 alibabacloud_btripopen20220520_py2-1.1.4/alibabacloud_btripopen20220520_py2.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)      172 2023-06-15 03:38:12.000000 alibabacloud_btripopen20220520_py2-1.1.4/alibabacloud_btripopen20220520_py2.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)       31 2023-06-15 03:38:12.000000 alibabacloud_btripopen20220520_py2-1.1.4/alibabacloud_btripopen20220520_py2.egg-info/top_level.txt
--rw-r--r--   0 root         (0) root         (0)       73 2023-06-15 03:38:12.000000 alibabacloud_btripopen20220520_py2-1.1.4/setup.cfg
--rw-r--r--   0 root         (0) root         (0)     2933 2023-06-15 03:38:12.000000 alibabacloud_btripopen20220520_py2-1.1.4/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-16 07:44:51.000000 alibabacloud_btripopen20220520_py2-1.1.5/
+-rw-r--r--   0 root         (0) root         (0)     3417 2023-06-16 07:44:51.000000 alibabacloud_btripopen20220520_py2-1.1.5/ChangeLog.md
+-rw-r--r--   0 root         (0) root         (0)      588 2023-06-16 07:44:51.000000 alibabacloud_btripopen20220520_py2-1.1.5/LICENSE
+-rw-r--r--   0 root         (0) root         (0)       28 2023-06-16 07:44:51.000000 alibabacloud_btripopen20220520_py2-1.1.5/MANIFEST.in
+-rw-r--r--   0 root         (0) root         (0)     2508 2023-06-16 07:44:51.000000 alibabacloud_btripopen20220520_py2-1.1.5/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     1051 2023-06-16 07:44:51.000000 alibabacloud_btripopen20220520_py2-1.1.5/README-CN.md
+-rw-r--r--   0 root         (0) root         (0)     1134 2023-06-16 07:44:51.000000 alibabacloud_btripopen20220520_py2-1.1.5/README.md
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-16 07:44:51.000000 alibabacloud_btripopen20220520_py2-1.1.5/alibabacloud_btripopen20220520/
+-rw-r--r--   0 root         (0) root         (0)       21 2023-06-16 07:44:51.000000 alibabacloud_btripopen20220520_py2-1.1.5/alibabacloud_btripopen20220520/__init__.py
+-rw-r--r--   0 root         (0) root         (0)   223404 2023-06-16 07:44:51.000000 alibabacloud_btripopen20220520_py2-1.1.5/alibabacloud_btripopen20220520/client.py
+-rw-r--r--   0 root         (0) root         (0)  2006169 2023-06-16 07:44:51.000000 alibabacloud_btripopen20220520_py2-1.1.5/alibabacloud_btripopen20220520/models.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-16 07:44:51.000000 alibabacloud_btripopen20220520_py2-1.1.5/alibabacloud_btripopen20220520_py2.egg-info/
+-rw-r--r--   0 root         (0) root         (0)     2508 2023-06-16 07:44:51.000000 alibabacloud_btripopen20220520_py2-1.1.5/alibabacloud_btripopen20220520_py2.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      488 2023-06-16 07:44:51.000000 alibabacloud_btripopen20220520_py2-1.1.5/alibabacloud_btripopen20220520_py2.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-06-16 07:44:51.000000 alibabacloud_btripopen20220520_py2-1.1.5/alibabacloud_btripopen20220520_py2.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)      172 2023-06-16 07:44:51.000000 alibabacloud_btripopen20220520_py2-1.1.5/alibabacloud_btripopen20220520_py2.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)       31 2023-06-16 07:44:51.000000 alibabacloud_btripopen20220520_py2-1.1.5/alibabacloud_btripopen20220520_py2.egg-info/top_level.txt
+-rw-r--r--   0 root         (0) root         (0)       73 2023-06-16 07:44:51.000000 alibabacloud_btripopen20220520_py2-1.1.5/setup.cfg
+-rw-r--r--   0 root         (0) root         (0)     2933 2023-06-16 07:44:51.000000 alibabacloud_btripopen20220520_py2-1.1.5/setup.py
```

### Comparing `alibabacloud_btripopen20220520_py2-1.1.4/ChangeLog.md` & `alibabacloud_btripopen20220520_py2-1.1.5/ChangeLog.md`

 * *Files 0% similar despite different names*

```diff
@@ -1,7 +1,10 @@
+2023-06-15 Version: 1.1.4
+- Update.
+
 2023-06-12 Version: 1.1.3
 - Update.
 
 2023-06-09 Version: 1.1.2
 - Update.
 
 2023-06-06 Version: 1.0.74
```

### Comparing `alibabacloud_btripopen20220520_py2-1.1.4/LICENSE` & `alibabacloud_btripopen20220520_py2-1.1.5/LICENSE`

 * *Files identical despite different names*

### Comparing `alibabacloud_btripopen20220520_py2-1.1.4/PKG-INFO` & `alibabacloud_btripopen20220520_py2-1.1.5/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: alibabacloud_btripopen20220520_py2
-Version: 1.1.4
+Version: 1.1.5
 Summary: Alibaba Cloud btripOpen (20220520) SDK Library for Python2
 Home-page: https://github.com/aliyun/alibabacloud-python2-sdk
 Author: Alibaba Cloud SDK
 Author-email: sdk-team@alibabacloud.com
 License: Apache License 2.0
 Description: English | [简体中文](README-CN.md)
         ![](https://aliyunsdk-pages.alicdn.com/icons/AlibabaCloud.svg)
```

### Comparing `alibabacloud_btripopen20220520_py2-1.1.4/README-CN.md` & `alibabacloud_btripopen20220520_py2-1.1.5/README-CN.md`

 * *Files identical despite different names*

### Comparing `alibabacloud_btripopen20220520_py2-1.1.4/README.md` & `alibabacloud_btripopen20220520_py2-1.1.5/README.md`

 * *Files identical despite different names*

### Comparing `alibabacloud_btripopen20220520_py2-1.1.4/alibabacloud_btripopen20220520/client.py` & `alibabacloud_btripopen20220520_py2-1.1.5/alibabacloud_btripopen20220520/client.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_btripopen20220520_py2-1.1.4/alibabacloud_btripopen20220520/models.py` & `alibabacloud_btripopen20220520_py2-1.1.5/alibabacloud_btripopen20220520/models.py`

 * *Files 1% similar despite different names*

```diff
@@ -39092,42 +39092,105 @@
         if m.get('reimb_order_no') is not None:
             self.reimb_order_no = m.get('reimb_order_no')
         if m.get('sub_corp_id') is not None:
             self.sub_corp_id = m.get('sub_corp_id')
         return self
 
 
+class QueryReimbursementOrderResponseBodyModuleExpensesExpenseCompositions(TeaModel):
+    def __init__(self, bill_settlement_id=None, fee_type=None, remark=None, remind_tag_list=None,
+                 settlement_amount=None, settlement_time=None, voucher_type=None):
+        self.bill_settlement_id = bill_settlement_id  # type: long
+        self.fee_type = fee_type  # type: str
+        self.remark = remark  # type: str
+        self.remind_tag_list = remind_tag_list  # type: list[str]
+        self.settlement_amount = settlement_amount  # type: str
+        self.settlement_time = settlement_time  # type: str
+        self.voucher_type = voucher_type  # type: int
+
+    def validate(self):
+        pass
+
+    def to_map(self):
+        _map = super(QueryReimbursementOrderResponseBodyModuleExpensesExpenseCompositions, self).to_map()
+        if _map is not None:
+            return _map
+
+        result = dict()
+        if self.bill_settlement_id is not None:
+            result['bill_settlement_id'] = self.bill_settlement_id
+        if self.fee_type is not None:
+            result['fee_type'] = self.fee_type
+        if self.remark is not None:
+            result['remark'] = self.remark
+        if self.remind_tag_list is not None:
+            result['remind_tag_list'] = self.remind_tag_list
+        if self.settlement_amount is not None:
+            result['settlement_amount'] = self.settlement_amount
+        if self.settlement_time is not None:
+            result['settlement_time'] = self.settlement_time
+        if self.voucher_type is not None:
+            result['voucher_type'] = self.voucher_type
+        return result
+
+    def from_map(self, m=None):
+        m = m or dict()
+        if m.get('bill_settlement_id') is not None:
+            self.bill_settlement_id = m.get('bill_settlement_id')
+        if m.get('fee_type') is not None:
+            self.fee_type = m.get('fee_type')
+        if m.get('remark') is not None:
+            self.remark = m.get('remark')
+        if m.get('remind_tag_list') is not None:
+            self.remind_tag_list = m.get('remind_tag_list')
+        if m.get('settlement_amount') is not None:
+            self.settlement_amount = m.get('settlement_amount')
+        if m.get('settlement_time') is not None:
+            self.settlement_time = m.get('settlement_time')
+        if m.get('voucher_type') is not None:
+            self.voucher_type = m.get('voucher_type')
+        return self
+
+
 class QueryReimbursementOrderResponseBodyModuleExpenses(TeaModel):
-    def __init__(self, amount=None, currency=None, expense_city=None, expense_time=None, expense_type=None,
-                 expense_type_code=None, reimb_expense_id=None, remark=None, settlement_type=None):
+    def __init__(self, amount=None, currency=None, expense_city=None, expense_compositions=None, expense_time=None,
+                 expense_type=None, expense_type_code=None, reimb_expense_id=None, remark=None, settlement_type=None):
         self.amount = amount  # type: str
         self.currency = currency  # type: str
         self.expense_city = expense_city  # type: str
+        self.expense_compositions = expense_compositions  # type: list[QueryReimbursementOrderResponseBodyModuleExpensesExpenseCompositions]
         self.expense_time = expense_time  # type: str
         self.expense_type = expense_type  # type: str
         self.expense_type_code = expense_type_code  # type: str
         self.reimb_expense_id = reimb_expense_id  # type: long
         self.remark = remark  # type: str
         self.settlement_type = settlement_type  # type: str
 
     def validate(self):
-        pass
+        if self.expense_compositions:
+            for k in self.expense_compositions:
+                if k:
+                    k.validate()
 
     def to_map(self):
         _map = super(QueryReimbursementOrderResponseBodyModuleExpenses, self).to_map()
         if _map is not None:
             return _map
 
         result = dict()
         if self.amount is not None:
             result['amount'] = self.amount
         if self.currency is not None:
             result['currency'] = self.currency
         if self.expense_city is not None:
             result['expense_city'] = self.expense_city
+        result['expense_compositions'] = []
+        if self.expense_compositions is not None:
+            for k in self.expense_compositions:
+                result['expense_compositions'].append(k.to_map() if k else None)
         if self.expense_time is not None:
             result['expense_time'] = self.expense_time
         if self.expense_type is not None:
             result['expense_type'] = self.expense_type
         if self.expense_type_code is not None:
             result['expense_type_code'] = self.expense_type_code
         if self.reimb_expense_id is not None:
@@ -39142,14 +39205,19 @@
         m = m or dict()
         if m.get('amount') is not None:
             self.amount = m.get('amount')
         if m.get('currency') is not None:
             self.currency = m.get('currency')
         if m.get('expense_city') is not None:
             self.expense_city = m.get('expense_city')
+        self.expense_compositions = []
+        if m.get('expense_compositions') is not None:
+            for k in m.get('expense_compositions'):
+                temp_model = QueryReimbursementOrderResponseBodyModuleExpensesExpenseCompositions()
+                self.expense_compositions.append(temp_model.from_map(k))
         if m.get('expense_time') is not None:
             self.expense_time = m.get('expense_time')
         if m.get('expense_type') is not None:
             self.expense_type = m.get('expense_type')
         if m.get('expense_type_code') is not None:
             self.expense_type_code = m.get('expense_type_code')
         if m.get('reimb_expense_id') is not None:
```

### Comparing `alibabacloud_btripopen20220520_py2-1.1.4/alibabacloud_btripopen20220520_py2.egg-info/PKG-INFO` & `alibabacloud_btripopen20220520_py2-1.1.5/alibabacloud_btripopen20220520_py2.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: alibabacloud-btripopen20220520-py2
-Version: 1.1.4
+Version: 1.1.5
 Summary: Alibaba Cloud btripOpen (20220520) SDK Library for Python2
 Home-page: https://github.com/aliyun/alibabacloud-python2-sdk
 Author: Alibaba Cloud SDK
 Author-email: sdk-team@alibabacloud.com
 License: Apache License 2.0
 Description: English | [简体中文](README-CN.md)
         ![](https://aliyunsdk-pages.alicdn.com/icons/AlibabaCloud.svg)
```

### Comparing `alibabacloud_btripopen20220520_py2-1.1.4/setup.py` & `alibabacloud_btripopen20220520_py2-1.1.5/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -21,15 +21,15 @@
 import os
 import sys
 from setuptools import setup, find_packages
 
 """
 setup module for alibabacloud_btripopen20220520_py2.
 
-Created on 15/06/2023
+Created on 16/06/2023
 
 @author: Alibaba Cloud SDK
 """
 
 PACKAGE = "alibabacloud_btripopen20220520"
 NAME = "alibabacloud_btripopen20220520_py2" or "alibabacloud-package"
 DESCRIPTION = "Alibaba Cloud btripOpen (20220520) SDK Library for Python2"
```

