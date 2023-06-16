# Comparing `tmp/odoo14_addons_shopinvader_odoo_shopinvader_payment-14.0.20230315.0-py3-none-any.whl.zip` & `tmp/odoo14_addons_shopinvader_odoo_shopinvader_payment-14.0.20230615.0-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,6 +1,6 @@
-Zip file size: 1614 bytes, number of entries: 4
--rw-r--r--  2.0 unx      928 b- defN 23-Mar-16 02:36 odoo14_addons_shopinvader_odoo_shopinvader_payment-14.0.20230315.0.dist-info/METADATA
--rw-r--r--  2.0 unx       92 b- defN 23-Mar-16 02:36 odoo14_addons_shopinvader_odoo_shopinvader_payment-14.0.20230315.0.dist-info/WHEEL
--rw-r--r--  2.0 unx        1 b- defN 23-Mar-16 02:36 odoo14_addons_shopinvader_odoo_shopinvader_payment-14.0.20230315.0.dist-info/top_level.txt
-?rw-rw-r--  2.0 unx      508 b- defN 23-Mar-16 02:36 odoo14_addons_shopinvader_odoo_shopinvader_payment-14.0.20230315.0.dist-info/RECORD
-4 files, 1529 bytes uncompressed, 608 bytes compressed:  60.2%
+Zip file size: 1634 bytes, number of entries: 4
+-rw-r--r--  2.0 unx     1161 b- defN 23-Jun-16 02:40 odoo14_addons_shopinvader_odoo_shopinvader_payment-14.0.20230615.0.dist-info/METADATA
+-rw-r--r--  2.0 unx       92 b- defN 23-Jun-16 02:40 odoo14_addons_shopinvader_odoo_shopinvader_payment-14.0.20230615.0.dist-info/WHEEL
+-rw-r--r--  2.0 unx        1 b- defN 23-Jun-16 02:40 odoo14_addons_shopinvader_odoo_shopinvader_payment-14.0.20230615.0.dist-info/top_level.txt
+?rw-rw-r--  2.0 unx      509 b- defN 23-Jun-16 02:40 odoo14_addons_shopinvader_odoo_shopinvader_payment-14.0.20230615.0.dist-info/RECORD
+4 files, 1763 bytes uncompressed, 628 bytes compressed:  64.4%
```

## zipnote {}

```diff
@@ -1,13 +1,13 @@
-Filename: odoo14_addons_shopinvader_odoo_shopinvader_payment-14.0.20230315.0.dist-info/METADATA
+Filename: odoo14_addons_shopinvader_odoo_shopinvader_payment-14.0.20230615.0.dist-info/METADATA
 Comment: 
 
-Filename: odoo14_addons_shopinvader_odoo_shopinvader_payment-14.0.20230315.0.dist-info/WHEEL
+Filename: odoo14_addons_shopinvader_odoo_shopinvader_payment-14.0.20230615.0.dist-info/WHEEL
 Comment: 
 
-Filename: odoo14_addons_shopinvader_odoo_shopinvader_payment-14.0.20230315.0.dist-info/top_level.txt
+Filename: odoo14_addons_shopinvader_odoo_shopinvader_payment-14.0.20230615.0.dist-info/top_level.txt
 Comment: 
 
-Filename: odoo14_addons_shopinvader_odoo_shopinvader_payment-14.0.20230315.0.dist-info/RECORD
+Filename: odoo14_addons_shopinvader_odoo_shopinvader_payment-14.0.20230615.0.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## Comparing `odoo14_addons_shopinvader_odoo_shopinvader_payment-14.0.20230315.0.dist-info/METADATA` & `odoo14_addons_shopinvader_odoo_shopinvader_payment-14.0.20230615.0.dist-info/METADATA`

 * *Files 6% similar despite different names*

```diff
@@ -1,21 +1,25 @@
 Metadata-Version: 2.1
 Name: odoo14-addons-shopinvader-odoo-shopinvader-payment
-Version: 14.0.20230315.0
+Version: 14.0.20230615.0
 Summary: Meta package for shopinvader-odoo-shopinvader-payment Odoo addons
 Home-page: UNKNOWN
 License: UNKNOWN
 Platform: UNKNOWN
 Classifier: Programming Language :: Python
 Classifier: Framework :: Odoo
 Classifier: Framework :: Odoo :: 14.0
 Requires-Dist: odoo14-addon-invader-invoice-payment
 Requires-Dist: odoo14-addon-invader-payment
 Requires-Dist: odoo14-addon-invader-payment-adyen
+Requires-Dist: odoo14-addon-invader-payment-adyen-klarna
+Requires-Dist: odoo14-addon-invader-payment-adyen-klarna-invoice
+Requires-Dist: odoo14-addon-invader-payment-adyen-klarna-sale
 Requires-Dist: odoo14-addon-invader-payment-manual
+Requires-Dist: odoo14-addon-invader-payment-sale
 Requires-Dist: odoo14-addon-invader-payment-stripe
 Requires-Dist: odoo14-addon-shopinvader-invoice-payment
 Requires-Dist: odoo14-addon-shopinvader-payment
 Requires-Dist: odoo14-addon-shopinvader-payment-adyen
 Requires-Dist: odoo14-addon-shopinvader-payment-condition
 Requires-Dist: odoo14-addon-shopinvader-payment-manual
 Requires-Dist: odoo14-addon-shopinvader-payment-stripe
```

