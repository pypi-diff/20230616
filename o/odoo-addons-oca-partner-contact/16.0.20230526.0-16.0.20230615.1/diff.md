# Comparing `tmp/odoo_addons_oca_partner_contact-16.0.20230526.0-py3-none-any.whl.zip` & `tmp/odoo_addons_oca_partner_contact-16.0.20230615.1-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,6 +1,6 @@
-Zip file size: 1722 bytes, number of entries: 4
--rw-r--r--  2.0 unx     2718 b- defN 23-May-27 04:21 odoo_addons_oca_partner_contact-16.0.20230526.0.dist-info/METADATA
--rw-r--r--  2.0 unx       92 b- defN 23-May-27 04:21 odoo_addons_oca_partner_contact-16.0.20230526.0.dist-info/WHEEL
--rw-r--r--  2.0 unx        1 b- defN 23-May-27 04:21 odoo_addons_oca_partner_contact-16.0.20230526.0.dist-info/top_level.txt
-?rw-rw-r--  2.0 unx      433 b- defN 23-May-27 04:21 odoo_addons_oca_partner_contact-16.0.20230526.0.dist-info/RECORD
-4 files, 3244 bytes uncompressed, 868 bytes compressed:  73.2%
+Zip file size: 1740 bytes, number of entries: 4
+-rw-r--r--  2.0 unx     2863 b- defN 23-Jun-16 05:49 odoo_addons_oca_partner_contact-16.0.20230615.1.dist-info/METADATA
+-rw-r--r--  2.0 unx       92 b- defN 23-Jun-16 05:49 odoo_addons_oca_partner_contact-16.0.20230615.1.dist-info/WHEEL
+-rw-r--r--  2.0 unx        1 b- defN 23-Jun-16 05:49 odoo_addons_oca_partner_contact-16.0.20230615.1.dist-info/top_level.txt
+?rw-rw-r--  2.0 unx      433 b- defN 23-Jun-16 05:49 odoo_addons_oca_partner_contact-16.0.20230615.1.dist-info/RECORD
+4 files, 3389 bytes uncompressed, 886 bytes compressed:  73.9%
```

## zipnote {}

```diff
@@ -1,13 +1,13 @@
-Filename: odoo_addons_oca_partner_contact-16.0.20230526.0.dist-info/METADATA
+Filename: odoo_addons_oca_partner_contact-16.0.20230615.1.dist-info/METADATA
 Comment: 
 
-Filename: odoo_addons_oca_partner_contact-16.0.20230526.0.dist-info/WHEEL
+Filename: odoo_addons_oca_partner_contact-16.0.20230615.1.dist-info/WHEEL
 Comment: 
 
-Filename: odoo_addons_oca_partner_contact-16.0.20230526.0.dist-info/top_level.txt
+Filename: odoo_addons_oca_partner_contact-16.0.20230615.1.dist-info/top_level.txt
 Comment: 
 
-Filename: odoo_addons_oca_partner_contact-16.0.20230526.0.dist-info/RECORD
+Filename: odoo_addons_oca_partner_contact-16.0.20230615.1.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## Comparing `odoo_addons_oca_partner_contact-16.0.20230526.0.dist-info/METADATA` & `odoo_addons_oca_partner_contact-16.0.20230615.1.dist-info/METADATA`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: odoo-addons-oca-partner-contact
-Version: 16.0.20230526.0
+Version: 16.0.20230615.1
 Summary: Meta package for oca-partner-contact Odoo addons
 Home-page: UNKNOWN
 License: UNKNOWN
 Platform: UNKNOWN
 Classifier: Programming Language :: Python
 Classifier: Framework :: Odoo
 Classifier: Framework :: Odoo :: 16.0
@@ -17,14 +17,15 @@
 Requires-Dist: odoo-addon-partner-address-street3 (<16.1dev,>=16.0dev)
 Requires-Dist: odoo-addon-partner-address-two-lines (<16.1dev,>=16.0dev)
 Requires-Dist: odoo-addon-partner-affiliate (<16.1dev,>=16.0dev)
 Requires-Dist: odoo-addon-partner-company-default (<16.1dev,>=16.0dev)
 Requires-Dist: odoo-addon-partner-company-type (<16.1dev,>=16.0dev)
 Requires-Dist: odoo-addon-partner-contact-access-link (<16.1dev,>=16.0dev)
 Requires-Dist: odoo-addon-partner-contact-address-default (<16.1dev,>=16.0dev)
+Requires-Dist: odoo-addon-partner-contact-age-range (<16.1dev,>=16.0dev)
 Requires-Dist: odoo-addon-partner-contact-birthdate (<16.1dev,>=16.0dev)
 Requires-Dist: odoo-addon-partner-contact-gender (<16.1dev,>=16.0dev)
 Requires-Dist: odoo-addon-partner-contact-job-position (<16.1dev,>=16.0dev)
 Requires-Dist: odoo-addon-partner-contact-lang (<16.1dev,>=16.0dev)
 Requires-Dist: odoo-addon-partner-contact-nationality (<16.1dev,>=16.0dev)
 Requires-Dist: odoo-addon-partner-contact-personal-information-page (<16.1dev,>=16.0dev)
 Requires-Dist: odoo-addon-partner-disable-gravatar (<16.1dev,>=16.0dev)
@@ -34,14 +35,15 @@
 Requires-Dist: odoo-addon-partner-firstname (<16.1dev,>=16.0dev)
 Requires-Dist: odoo-addon-partner-identification (<16.1dev,>=16.0dev)
 Requires-Dist: odoo-addon-partner-industry-secondary (<16.1dev,>=16.0dev)
 Requires-Dist: odoo-addon-partner-interest-group (<16.1dev,>=16.0dev)
 Requires-Dist: odoo-addon-partner-manual-rank (<16.1dev,>=16.0dev)
 Requires-Dist: odoo-addon-partner-middlename (<16.1dev,>=16.0dev)
 Requires-Dist: odoo-addon-partner-multi-relation (<16.1dev,>=16.0dev)
+Requires-Dist: odoo-addon-partner-pricelist-search (<16.1dev,>=16.0dev)
 Requires-Dist: odoo-addon-partner-ref-unique (<16.1dev,>=16.0dev)
 Requires-Dist: odoo-addon-partner-second-lastname (<16.1dev,>=16.0dev)
 Requires-Dist: odoo-addon-partner-tz (<16.1dev,>=16.0dev)
 Requires-Dist: odoo-addon-partner-vat-unique (<16.1dev,>=16.0dev)
 
 UNKNOWN
```

