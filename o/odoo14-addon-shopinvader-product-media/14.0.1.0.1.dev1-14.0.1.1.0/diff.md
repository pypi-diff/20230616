# Comparing `tmp/odoo14_addon_shopinvader_product_media-14.0.1.0.1.dev1-py3-none-any.whl.zip` & `tmp/odoo14_addon_shopinvader_product_media-14.0.1.1.0-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,11 +1,11 @@
-Zip file size: 4725 bytes, number of entries: 9
--rw-r--r--  2.0 unx     1123 b- defN 21-Jul-07 20:24 odoo/addons/shopinvader_product_media/README.rst
--rw-r--r--  2.0 unx        0 b- defN 21-Jul-07 20:24 odoo/addons/shopinvader_product_media/__init__.py
--rw-r--r--  2.0 unx      614 b- defN 21-Jul-07 20:24 odoo/addons/shopinvader_product_media/__manifest__.py
--rw-r--r--  2.0 unx     1245 b- defN 21-Jul-07 20:24 odoo/addons/shopinvader_product_media/data/ir_product_export.xml
--rw-r--r--  2.0 unx      341 b- defN 21-Jul-07 20:24 odoo/addons/shopinvader_product_media/i18n/shopinvader_product_media.pot
--rw-r--r--  2.0 unx     1691 b- defN 21-Jul-07 20:24 odoo14_addon_shopinvader_product_media-14.0.1.0.1.dev1.dist-info/METADATA
--rw-r--r--  2.0 unx       92 b- defN 21-Jul-07 20:24 odoo14_addon_shopinvader_product_media-14.0.1.0.1.dev1.dist-info/WHEEL
--rw-r--r--  2.0 unx        5 b- defN 21-Jul-07 20:24 odoo14_addon_shopinvader_product_media-14.0.1.0.1.dev1.dist-info/top_level.txt
-?rw-rw-r--  2.0 unx     1027 b- defN 21-Jul-07 20:24 odoo14_addon_shopinvader_product_media-14.0.1.0.1.dev1.dist-info/RECORD
-9 files, 6138 bytes uncompressed, 2863 bytes compressed:  53.4%
+Zip file size: 4709 bytes, number of entries: 9
+-rw-r--r--  2.0 unx     1123 b- defN 23-Jun-16 14:19 odoo/addons/shopinvader_product_media/README.rst
+-rw-r--r--  2.0 unx        0 b- defN 23-Jun-16 14:19 odoo/addons/shopinvader_product_media/__init__.py
+-rw-r--r--  2.0 unx      614 b- defN 23-Jun-16 14:19 odoo/addons/shopinvader_product_media/__manifest__.py
+-rw-r--r--  2.0 unx     1545 b- defN 23-Jun-16 14:19 odoo/addons/shopinvader_product_media/data/ir_product_export.xml
+-rw-r--r--  2.0 unx      341 b- defN 23-Jun-16 14:19 odoo/addons/shopinvader_product_media/i18n/shopinvader_product_media.pot
+-rw-r--r--  2.0 unx     1724 b- defN 23-Jun-16 14:19 odoo14_addon_shopinvader_product_media-14.0.1.1.0.dist-info/METADATA
+-rw-r--r--  2.0 unx       92 b- defN 23-Jun-16 14:19 odoo14_addon_shopinvader_product_media-14.0.1.1.0.dist-info/WHEEL
+-rw-r--r--  2.0 unx        5 b- defN 23-Jun-16 14:19 odoo14_addon_shopinvader_product_media-14.0.1.1.0.dist-info/top_level.txt
+?rw-rw-r--  2.0 unx     1007 b- defN 23-Jun-16 14:19 odoo14_addon_shopinvader_product_media-14.0.1.1.0.dist-info/RECORD
+9 files, 6451 bytes uncompressed, 2887 bytes compressed:  55.2%
```

## zipnote {}

```diff
@@ -9,20 +9,20 @@
 
 Filename: odoo/addons/shopinvader_product_media/data/ir_product_export.xml
 Comment: 
 
 Filename: odoo/addons/shopinvader_product_media/i18n/shopinvader_product_media.pot
 Comment: 
 
-Filename: odoo14_addon_shopinvader_product_media-14.0.1.0.1.dev1.dist-info/METADATA
+Filename: odoo14_addon_shopinvader_product_media-14.0.1.1.0.dist-info/METADATA
 Comment: 
 
-Filename: odoo14_addon_shopinvader_product_media-14.0.1.0.1.dev1.dist-info/WHEEL
+Filename: odoo14_addon_shopinvader_product_media-14.0.1.1.0.dist-info/WHEEL
 Comment: 
 
-Filename: odoo14_addon_shopinvader_product_media-14.0.1.0.1.dev1.dist-info/top_level.txt
+Filename: odoo14_addon_shopinvader_product_media-14.0.1.1.0.dist-info/top_level.txt
 Comment: 
 
-Filename: odoo14_addon_shopinvader_product_media-14.0.1.0.1.dev1.dist-info/RECORD
+Filename: odoo14_addon_shopinvader_product_media-14.0.1.1.0.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## odoo/addons/shopinvader_product_media/__manifest__.py

```diff
@@ -1,15 +1,15 @@
 # Copyright 2016 Akretion (http://www.akretion.com)
 # Sébastien BEAU <sebastien.beau@akretion.com>
 # License AGPL-3.0 or later (http://www.gnu.org/licenses/agpl.html).
 
 {
     "name": "Shopinvader Product Media",
     "summary": "Index storage media data into external search engine",
-    "version": "14.0.1.0.0",
+    "version": "14.0.1.1.0",
     "category": "e-commerce",
     "website": "https://github.com/shopinvader/odoo-shopinvader",
     "author": "Akretion",
     "license": "AGPL-3",
     "installable": True,
     "auto_install": True,
     "depends": ["shopinvader", "storage_media_product"],
```

## odoo/addons/shopinvader_product_media/data/ir_product_export.xml

### odoo/addons/shopinvader_product_media/data/ir_product_export.xml

```diff
@@ -1,14 +1,19 @@
 <?xml version="1.0" encoding="utf-8"?>
 <odoo>
   <record id="ir_exp_shopinvader_variant_media_name" model="ir.exports.line">
     <field name="name">variant_media_ids/name</field>
     <field name="target">variant_media_ids:media/name</field>
     <field name="export_id" ref="shopinvader.ir_exp_shopinvader_variant"/>
   </record>
+  <record id="ir_exp_shopinvader_variant_media_description" model="ir.exports.line">
+    <field name="name">variant_media_ids/description</field>
+    <field name="target">variant_media_ids:media/description</field>
+    <field name="export_id" ref="shopinvader.ir_exp_shopinvader_variant"/>
+  </record>
   <record id="ir_exp_shopinvader_variant_media_url" model="ir.exports.line">
     <field name="name">variant_media_ids/url</field>
     <field name="target">variant_media_ids:media/url</field>
     <field name="export_id" ref="shopinvader.ir_exp_shopinvader_variant"/>
   </record>
   <record id="ir_exp_shopinvader_variant_media_type_name" model="ir.exports.line">
     <field name="name">variant_media_ids/media_type_id/name</field>
```

## Comparing `odoo14_addon_shopinvader_product_media-14.0.1.0.1.dev1.dist-info/METADATA` & `odoo14_addon_shopinvader_product_media-14.0.1.1.0.dist-info/METADATA`

 * *Files 4% similar despite different names*

```diff
@@ -1,17 +1,18 @@
 Metadata-Version: 2.1
 Name: odoo14-addon-shopinvader-product-media
-Version: 14.0.1.0.1.dev1
+Version: 14.0.1.1.0
 Summary: Index storage media data into external search engine
 Home-page: https://github.com/shopinvader/odoo-shopinvader
 Author: Akretion
 License: AGPL-3
 Platform: UNKNOWN
 Classifier: Programming Language :: Python
 Classifier: Framework :: Odoo
+Classifier: Framework :: Odoo :: 14.0
 Classifier: License :: OSI Approved :: GNU Affero General Public License v3
 Requires-Python: >=3.6
 Requires-Dist: odoo14-addon-shopinvader
 Requires-Dist: odoo14-addon-storage-media-product
 Requires-Dist: odoo (<14.1dev,>=14.0a)
 
 .. image:: https://img.shields.io/badge/licence-AGPL--3-blue.svg
```

