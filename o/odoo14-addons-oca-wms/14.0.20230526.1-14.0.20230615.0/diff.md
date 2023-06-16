# Comparing `tmp/odoo14_addons_oca_wms-14.0.20230526.1-py3-none-any.whl.zip` & `tmp/odoo14_addons_oca_wms-14.0.20230615.0-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,6 +1,6 @@
-Zip file size: 1773 bytes, number of entries: 4
--rw-r--r--  2.0 unx     3483 b- defN 23-May-27 05:37 odoo14_addons_oca_wms-14.0.20230526.1.dist-info/METADATA
--rw-r--r--  2.0 unx       92 b- defN 23-May-27 05:37 odoo14_addons_oca_wms-14.0.20230526.1.dist-info/WHEEL
--rw-r--r--  2.0 unx        1 b- defN 23-May-27 05:37 odoo14_addons_oca_wms-14.0.20230526.1.dist-info/top_level.txt
-?rw-rw-r--  2.0 unx      393 b- defN 23-May-27 05:37 odoo14_addons_oca_wms-14.0.20230526.1.dist-info/RECORD
-4 files, 3969 bytes uncompressed, 999 bytes compressed:  74.8%
+Zip file size: 1784 bytes, number of entries: 4
+-rw-r--r--  2.0 unx     3559 b- defN 23-Jun-16 08:00 odoo14_addons_oca_wms-14.0.20230615.0.dist-info/METADATA
+-rw-r--r--  2.0 unx       92 b- defN 23-Jun-16 08:00 odoo14_addons_oca_wms-14.0.20230615.0.dist-info/WHEEL
+-rw-r--r--  2.0 unx        1 b- defN 23-Jun-16 08:00 odoo14_addons_oca_wms-14.0.20230615.0.dist-info/top_level.txt
+?rw-rw-r--  2.0 unx      393 b- defN 23-Jun-16 08:00 odoo14_addons_oca_wms-14.0.20230615.0.dist-info/RECORD
+4 files, 4045 bytes uncompressed, 1010 bytes compressed:  75.0%
```

## zipnote {}

```diff
@@ -1,13 +1,13 @@
-Filename: odoo14_addons_oca_wms-14.0.20230526.1.dist-info/METADATA
+Filename: odoo14_addons_oca_wms-14.0.20230615.0.dist-info/METADATA
 Comment: 
 
-Filename: odoo14_addons_oca_wms-14.0.20230526.1.dist-info/WHEEL
+Filename: odoo14_addons_oca_wms-14.0.20230615.0.dist-info/WHEEL
 Comment: 
 
-Filename: odoo14_addons_oca_wms-14.0.20230526.1.dist-info/top_level.txt
+Filename: odoo14_addons_oca_wms-14.0.20230615.0.dist-info/top_level.txt
 Comment: 
 
-Filename: odoo14_addons_oca_wms-14.0.20230526.1.dist-info/RECORD
+Filename: odoo14_addons_oca_wms-14.0.20230615.0.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## Comparing `odoo14_addons_oca_wms-14.0.20230526.1.dist-info/METADATA` & `odoo14_addons_oca_wms-14.0.20230615.0.dist-info/METADATA`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: odoo14-addons-oca-wms
-Version: 14.0.20230526.1
+Version: 14.0.20230615.0
 Summary: Meta package for oca-wms Odoo addons
 Home-page: UNKNOWN
 License: UNKNOWN
 Platform: UNKNOWN
 Classifier: Programming Language :: Python
 Classifier: Framework :: Odoo
 Classifier: Framework :: Odoo :: 14.0
@@ -33,14 +33,15 @@
 Requires-Dist: odoo14-addon-shopfloor-mobile-base-auth-api-key
 Requires-Dist: odoo14-addon-shopfloor-mobile-base-auth-user
 Requires-Dist: odoo14-addon-shopfloor-packing-info
 Requires-Dist: odoo14-addon-shopfloor-reception
 Requires-Dist: odoo14-addon-shopfloor-reception-mobile
 Requires-Dist: odoo14-addon-shopfloor-rest-log
 Requires-Dist: odoo14-addon-shopfloor-single-product-transfer
+Requires-Dist: odoo14-addon-shopfloor-single-product-transfer-force-package
 Requires-Dist: odoo14-addon-shopfloor-single-product-transfer-mobile
 Requires-Dist: odoo14-addon-shopfloor-workstation
 Requires-Dist: odoo14-addon-shopfloor-workstation-label-printer
 Requires-Dist: odoo14-addon-shopfloor-workstation-mobile
 Requires-Dist: odoo14-addon-stock-available-to-promise-release
 Requires-Dist: odoo14-addon-stock-available-to-promise-release-dynamic-routing
 Requires-Dist: odoo14-addon-stock-checkout-sync
```

