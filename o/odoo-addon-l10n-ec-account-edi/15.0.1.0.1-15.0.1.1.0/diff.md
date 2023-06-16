# Comparing `tmp/odoo_addon_l10n_ec_account_edi-15.0.1.0.1-py3-none-any.whl.zip` & `tmp/odoo_addon_l10n_ec_account_edi-15.0.1.1.0-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,66 +1,70 @@
-Zip file size: 119177 bytes, number of entries: 64
--rw-r--r--  2.0 unx        0 b- defN 23-May-07 22:26 odoo/addons/l10n_ec_account_edi/README.rst
--rw-r--r--  2.0 unx       63 b- defN 23-May-07 22:26 odoo/addons/l10n_ec_account_edi/__init__.py
--rw-r--r--  2.0 unx     1639 b- defN 23-May-07 22:26 odoo/addons/l10n_ec_account_edi/__manifest__.py
--rw-r--r--  2.0 unx      240 b- defN 23-May-07 22:26 odoo/addons/l10n_ec_account_edi/data/edi_format_data.xml
--rw-r--r--  2.0 unx     3880 b- defN 23-May-07 22:26 odoo/addons/l10n_ec_account_edi/data/edi_templates/edi_credit_note.xml
--rw-r--r--  2.0 unx     2687 b- defN 23-May-07 22:26 odoo/addons/l10n_ec_account_edi/data/edi_templates/edi_debit_note.xml
--rw-r--r--  2.0 unx     1337 b- defN 23-May-07 22:26 odoo/addons/l10n_ec_account_edi/data/edi_templates/edi_info_tributaria_data.xml
--rw-r--r--  2.0 unx     4444 b- defN 23-May-07 22:26 odoo/addons/l10n_ec_account_edi/data/edi_templates/edi_invoice.xml
--rw-r--r--  2.0 unx     4334 b- defN 23-May-07 22:26 odoo/addons/l10n_ec_account_edi/data/edi_templates/edi_liquidation.xml
--rw-r--r--  2.0 unx    15160 b- defN 23-May-07 22:26 odoo/addons/l10n_ec_account_edi/data/xsd/ComprobanteRetencion_V1.0.0.xsd
--rw-r--r--  2.0 unx    26969 b- defN 23-May-07 22:26 odoo/addons/l10n_ec_account_edi/data/xsd/ComprobanteRetencion_V2.0.0.xsd
--rw-r--r--  2.0 unx    20198 b- defN 23-May-07 22:26 odoo/addons/l10n_ec_account_edi/data/xsd/GuiaRemision_V1.0.0.xsd
--rw-r--r--  2.0 unx    20198 b- defN 23-May-07 22:26 odoo/addons/l10n_ec_account_edi/data/xsd/GuiaRemision_V1.1.0.xsd
--rw-r--r--  2.0 unx    27328 b- defN 23-May-07 22:26 odoo/addons/l10n_ec_account_edi/data/xsd/LiquidacionCompra_V1.0.0.xsd
--rw-r--r--  2.0 unx    27329 b- defN 23-May-07 22:26 odoo/addons/l10n_ec_account_edi/data/xsd/LiquidacionCompra_V1.1.0.xsd
--rw-r--r--  2.0 unx    20937 b- defN 23-May-07 22:26 odoo/addons/l10n_ec_account_edi/data/xsd/NotaCredito_V1.0.0.xsd
--rw-r--r--  2.0 unx    20937 b- defN 23-May-07 22:26 odoo/addons/l10n_ec_account_edi/data/xsd/NotaCredito_V1.1.0.xsd
--rw-r--r--  2.0 unx    23726 b- defN 23-May-07 22:26 odoo/addons/l10n_ec_account_edi/data/xsd/NotaDebito_V1.0.0.xsd
--rw-r--r--  2.0 unx    34032 b- defN 23-May-07 22:26 odoo/addons/l10n_ec_account_edi/data/xsd/factura_V1.0.0.xsd
--rw-r--r--  2.0 unx    35400 b- defN 23-May-07 22:26 odoo/addons/l10n_ec_account_edi/data/xsd/factura_V1.1.0.xsd
--rw-r--r--  2.0 unx    38832 b- defN 23-May-07 22:26 odoo/addons/l10n_ec_account_edi/data/xsd/factura_V2.0.0.xsd
--rw-r--r--  2.0 unx    39442 b- defN 23-May-07 22:26 odoo/addons/l10n_ec_account_edi/data/xsd/factura_V2.1.0.xsd
--rw-r--r--  2.0 unx    35948 b- defN 23-May-07 22:26 odoo/addons/l10n_ec_account_edi/i18n/l10n_ec_account_edi.pot
--rw-r--r--  2.0 unx      214 b- defN 23-May-07 22:26 odoo/addons/l10n_ec_account_edi/models/__init__.py
--rw-r--r--  2.0 unx    29194 b- defN 23-May-07 22:26 odoo/addons/l10n_ec_account_edi/models/account_edi_document.py
--rw-r--r--  2.0 unx    13990 b- defN 23-May-07 22:26 odoo/addons/l10n_ec_account_edi/models/account_edi_format.py
--rw-r--r--  2.0 unx    11989 b- defN 23-May-07 22:26 odoo/addons/l10n_ec_account_edi/models/account_move.py
--rw-r--r--  2.0 unx     3968 b- defN 23-May-07 22:26 odoo/addons/l10n_ec_account_edi/models/account_move_line.py
--rw-r--r--  2.0 unx     1582 b- defN 23-May-07 22:26 odoo/addons/l10n_ec_account_edi/models/res_company.py
--rw-r--r--  2.0 unx     1130 b- defN 23-May-07 22:26 odoo/addons/l10n_ec_account_edi/models/res_config_settings.py
--rw-r--r--  2.0 unx     9386 b- defN 23-May-07 22:26 odoo/addons/l10n_ec_account_edi/models/sri_key_type.py
--rw-r--r--  2.0 unx        0 b- defN 23-May-07 22:26 odoo/addons/l10n_ec_account_edi/report/__init__.py
--rw-r--r--  2.0 unx    11186 b- defN 23-May-07 22:26 odoo/addons/l10n_ec_account_edi/report/edi_report_templates.xml
--rw-r--r--  2.0 unx     4823 b- defN 23-May-07 22:26 odoo/addons/l10n_ec_account_edi/report/report_edi_credit_note.xml
--rw-r--r--  2.0 unx     3827 b- defN 23-May-07 22:26 odoo/addons/l10n_ec_account_edi/report/report_edi_debit_note.xml
--rw-r--r--  2.0 unx     4063 b- defN 23-May-07 22:26 odoo/addons/l10n_ec_account_edi/report/report_edi_invoice.xml
--rw-r--r--  2.0 unx     3961 b- defN 23-May-07 22:26 odoo/addons/l10n_ec_account_edi/report/report_edi_liquidation.xml
--rw-r--r--  2.0 unx     5285 b- defN 23-May-07 22:26 odoo/addons/l10n_ec_account_edi/report/report_invoice.xml
--rw-r--r--  2.0 unx      281 b- defN 23-May-07 22:26 odoo/addons/l10n_ec_account_edi/security/ir.model.access.csv
--rw-r--r--  2.0 unx     9455 b- defN 23-May-07 22:26 odoo/addons/l10n_ec_account_edi/static/description/icon.png
--rw-r--r--  2.0 unx     1648 b- defN 23-May-07 22:26 odoo/addons/l10n_ec_account_edi/static/src/scss/report_layout.scss
--rw-r--r--  2.0 unx      297 b- defN 23-May-07 22:26 odoo/addons/l10n_ec_account_edi/tests/__init__.py
--rw-r--r--  2.0 unx    10192 b- defN 23-May-07 22:26 odoo/addons/l10n_ec_account_edi/tests/test_common.py
--rw-r--r--  2.0 unx     7264 b- defN 23-May-07 22:26 odoo/addons/l10n_ec_account_edi/tests/test_edi_common.py
--rw-r--r--  2.0 unx     1044 b- defN 23-May-07 22:26 odoo/addons/l10n_ec_account_edi/tests/test_edi_format.py
--rw-r--r--  2.0 unx     8777 b- defN 23-May-07 22:26 odoo/addons/l10n_ec_account_edi/tests/test_l10n_ec_edi_credit_note.py
--rw-r--r--  2.0 unx     8739 b- defN 23-May-07 22:26 odoo/addons/l10n_ec_account_edi/tests/test_l10n_ec_edi_debit_note.py
--rw-r--r--  2.0 unx      687 b- defN 23-May-07 22:26 odoo/addons/l10n_ec_account_edi/tests/test_l10n_ec_edi_key_type.py
--rw-r--r--  2.0 unx    10707 b- defN 23-May-07 22:26 odoo/addons/l10n_ec_account_edi/tests/test_l10n_ec_edi_liquidation.py
--rw-r--r--  2.0 unx    11492 b- defN 23-May-07 22:26 odoo/addons/l10n_ec_account_edi/tests/test_l10n_ec_edi_out_invoice.py
--rw-r--r--  2.0 unx     3299 b- defN 23-May-07 22:26 odoo/addons/l10n_ec_account_edi/tests/certificates/test.p12
--rw-r--r--  2.0 unx     4076 b- defN 23-May-07 22:26 odoo/addons/l10n_ec_account_edi/views/account_edi_document_view.xml
--rw-r--r--  2.0 unx     8908 b- defN 23-May-07 22:26 odoo/addons/l10n_ec_account_edi/views/account_move_view.xml
--rw-r--r--  2.0 unx      791 b- defN 23-May-07 22:26 odoo/addons/l10n_ec_account_edi/views/menu_root.xml
--rw-r--r--  2.0 unx     7196 b- defN 23-May-07 22:26 odoo/addons/l10n_ec_account_edi/views/res_config_settings_view.xml
--rw-r--r--  2.0 unx     4533 b- defN 23-May-07 22:26 odoo/addons/l10n_ec_account_edi/views/sri_key_type_view.xml
--rw-r--r--  2.0 unx       69 b- defN 23-May-07 22:26 odoo/addons/l10n_ec_account_edi/wizard/__init__.py
--rw-r--r--  2.0 unx      583 b- defN 23-May-07 22:26 odoo/addons/l10n_ec_account_edi/wizard/account_debit_note.py
--rw-r--r--  2.0 unx      289 b- defN 23-May-07 22:26 odoo/addons/l10n_ec_account_edi/wizard/account_move_reversal.py
--rw-r--r--  2.0 unx      850 b- defN 23-May-07 22:26 odoo/addons/l10n_ec_account_edi/wizard/account_move_reversal_view.xml
--rw-r--r--  2.0 unx      825 b- defN 23-May-07 22:27 odoo_addon_l10n_ec_account_edi-15.0.1.0.1.dist-info/METADATA
--rw-r--r--  2.0 unx       92 b- defN 23-May-07 22:27 odoo_addon_l10n_ec_account_edi-15.0.1.0.1.dist-info/WHEEL
--rw-r--r--  2.0 unx        5 b- defN 23-May-07 22:27 odoo_addon_l10n_ec_account_edi-15.0.1.0.1.dist-info/top_level.txt
-?rw-rw-r--  2.0 unx     7486 b- defN 23-May-07 22:27 odoo_addon_l10n_ec_account_edi-15.0.1.0.1.dist-info/RECORD
-64 files, 619243 bytes uncompressed, 106499 bytes compressed:  82.8%
+Zip file size: 122886 bytes, number of entries: 68
+-rw-r--r--  2.0 unx        0 b- defN 23-Jun-16 08:59 odoo/addons/l10n_ec_account_edi/README.rst
+-rw-r--r--  2.0 unx       63 b- defN 23-Jun-16 08:59 odoo/addons/l10n_ec_account_edi/__init__.py
+-rw-r--r--  2.0 unx     1743 b- defN 23-Jun-16 08:59 odoo/addons/l10n_ec_account_edi/__manifest__.py
+-rw-r--r--  2.0 unx      891 b- defN 23-Jun-16 08:59 odoo/addons/l10n_ec_account_edi/data/cron_send_email_electronic_documents.xml
+-rw-r--r--  2.0 unx      240 b- defN 23-Jun-16 08:59 odoo/addons/l10n_ec_account_edi/data/edi_format_data.xml
+-rw-r--r--  2.0 unx      213 b- defN 23-Jun-16 08:59 odoo/addons/l10n_ec_account_edi/data/email_template_edi_invoice.xml
+-rw-r--r--  2.0 unx     3880 b- defN 23-Jun-16 08:59 odoo/addons/l10n_ec_account_edi/data/edi_templates/edi_credit_note.xml
+-rw-r--r--  2.0 unx     2687 b- defN 23-Jun-16 08:59 odoo/addons/l10n_ec_account_edi/data/edi_templates/edi_debit_note.xml
+-rw-r--r--  2.0 unx     1343 b- defN 23-Jun-16 08:59 odoo/addons/l10n_ec_account_edi/data/edi_templates/edi_info_tributaria_data.xml
+-rw-r--r--  2.0 unx     4444 b- defN 23-Jun-16 08:59 odoo/addons/l10n_ec_account_edi/data/edi_templates/edi_invoice.xml
+-rw-r--r--  2.0 unx     4334 b- defN 23-Jun-16 08:59 odoo/addons/l10n_ec_account_edi/data/edi_templates/edi_liquidation.xml
+-rw-r--r--  2.0 unx    15160 b- defN 23-Jun-16 08:59 odoo/addons/l10n_ec_account_edi/data/xsd/ComprobanteRetencion_V1.0.0.xsd
+-rw-r--r--  2.0 unx    26969 b- defN 23-Jun-16 08:59 odoo/addons/l10n_ec_account_edi/data/xsd/ComprobanteRetencion_V2.0.0.xsd
+-rw-r--r--  2.0 unx    20198 b- defN 23-Jun-16 08:59 odoo/addons/l10n_ec_account_edi/data/xsd/GuiaRemision_V1.0.0.xsd
+-rw-r--r--  2.0 unx    20198 b- defN 23-Jun-16 08:59 odoo/addons/l10n_ec_account_edi/data/xsd/GuiaRemision_V1.1.0.xsd
+-rw-r--r--  2.0 unx    27328 b- defN 23-Jun-16 08:59 odoo/addons/l10n_ec_account_edi/data/xsd/LiquidacionCompra_V1.0.0.xsd
+-rw-r--r--  2.0 unx    27329 b- defN 23-Jun-16 08:59 odoo/addons/l10n_ec_account_edi/data/xsd/LiquidacionCompra_V1.1.0.xsd
+-rw-r--r--  2.0 unx    20937 b- defN 23-Jun-16 08:59 odoo/addons/l10n_ec_account_edi/data/xsd/NotaCredito_V1.0.0.xsd
+-rw-r--r--  2.0 unx    20937 b- defN 23-Jun-16 08:59 odoo/addons/l10n_ec_account_edi/data/xsd/NotaCredito_V1.1.0.xsd
+-rw-r--r--  2.0 unx    23726 b- defN 23-Jun-16 08:59 odoo/addons/l10n_ec_account_edi/data/xsd/NotaDebito_V1.0.0.xsd
+-rw-r--r--  2.0 unx    34032 b- defN 23-Jun-16 08:59 odoo/addons/l10n_ec_account_edi/data/xsd/factura_V1.0.0.xsd
+-rw-r--r--  2.0 unx    35400 b- defN 23-Jun-16 08:59 odoo/addons/l10n_ec_account_edi/data/xsd/factura_V1.1.0.xsd
+-rw-r--r--  2.0 unx    38832 b- defN 23-Jun-16 08:59 odoo/addons/l10n_ec_account_edi/data/xsd/factura_V2.0.0.xsd
+-rw-r--r--  2.0 unx    39442 b- defN 23-Jun-16 08:59 odoo/addons/l10n_ec_account_edi/data/xsd/factura_V2.1.0.xsd
+-rw-r--r--  2.0 unx    38352 b- defN 23-Jun-16 08:59 odoo/addons/l10n_ec_account_edi/i18n/l10n_ec_account_edi.pot
+-rw-r--r--  2.0 unx      251 b- defN 23-Jun-16 08:59 odoo/addons/l10n_ec_account_edi/models/__init__.py
+-rw-r--r--  2.0 unx    30588 b- defN 23-Jun-16 08:59 odoo/addons/l10n_ec_account_edi/models/account_edi_document.py
+-rw-r--r--  2.0 unx    13990 b- defN 23-Jun-16 08:59 odoo/addons/l10n_ec_account_edi/models/account_edi_format.py
+-rw-r--r--  2.0 unx    12622 b- defN 23-Jun-16 08:59 odoo/addons/l10n_ec_account_edi/models/account_move.py
+-rw-r--r--  2.0 unx     3968 b- defN 23-Jun-16 08:59 odoo/addons/l10n_ec_account_edi/models/account_move_line.py
+-rw-r--r--  2.0 unx      346 b- defN 23-Jun-16 08:59 odoo/addons/l10n_ec_account_edi/models/additional_information.py
+-rw-r--r--  2.0 unx     1582 b- defN 23-Jun-16 08:59 odoo/addons/l10n_ec_account_edi/models/res_company.py
+-rw-r--r--  2.0 unx     1130 b- defN 23-Jun-16 08:59 odoo/addons/l10n_ec_account_edi/models/res_config_settings.py
+-rw-r--r--  2.0 unx     9386 b- defN 23-Jun-16 08:59 odoo/addons/l10n_ec_account_edi/models/sri_key_type.py
+-rw-r--r--  2.0 unx        0 b- defN 23-Jun-16 08:59 odoo/addons/l10n_ec_account_edi/report/__init__.py
+-rw-r--r--  2.0 unx    11272 b- defN 23-Jun-16 08:59 odoo/addons/l10n_ec_account_edi/report/edi_report_templates.xml
+-rw-r--r--  2.0 unx     4823 b- defN 23-Jun-16 08:59 odoo/addons/l10n_ec_account_edi/report/report_edi_credit_note.xml
+-rw-r--r--  2.0 unx     3827 b- defN 23-Jun-16 08:59 odoo/addons/l10n_ec_account_edi/report/report_edi_debit_note.xml
+-rw-r--r--  2.0 unx     4063 b- defN 23-Jun-16 08:59 odoo/addons/l10n_ec_account_edi/report/report_edi_invoice.xml
+-rw-r--r--  2.0 unx     3961 b- defN 23-Jun-16 08:59 odoo/addons/l10n_ec_account_edi/report/report_edi_liquidation.xml
+-rw-r--r--  2.0 unx     5285 b- defN 23-Jun-16 08:59 odoo/addons/l10n_ec_account_edi/report/report_invoice.xml
+-rw-r--r--  2.0 unx      458 b- defN 23-Jun-16 08:59 odoo/addons/l10n_ec_account_edi/security/ir.model.access.csv
+-rw-r--r--  2.0 unx     9455 b- defN 23-Jun-16 08:59 odoo/addons/l10n_ec_account_edi/static/description/icon.png
+-rw-r--r--  2.0 unx     1648 b- defN 23-Jun-16 08:59 odoo/addons/l10n_ec_account_edi/static/src/scss/report_layout.scss
+-rw-r--r--  2.0 unx      329 b- defN 23-Jun-16 08:59 odoo/addons/l10n_ec_account_edi/tests/__init__.py
+-rw-r--r--  2.0 unx    10570 b- defN 23-Jun-16 08:59 odoo/addons/l10n_ec_account_edi/tests/test_common.py
+-rw-r--r--  2.0 unx     7264 b- defN 23-Jun-16 08:59 odoo/addons/l10n_ec_account_edi/tests/test_edi_common.py
+-rw-r--r--  2.0 unx     1044 b- defN 23-Jun-16 08:59 odoo/addons/l10n_ec_account_edi/tests/test_edi_format.py
+-rw-r--r--  2.0 unx     8777 b- defN 23-Jun-16 08:59 odoo/addons/l10n_ec_account_edi/tests/test_l10n_ec_edi_credit_note.py
+-rw-r--r--  2.0 unx     8739 b- defN 23-Jun-16 08:59 odoo/addons/l10n_ec_account_edi/tests/test_l10n_ec_edi_debit_note.py
+-rw-r--r--  2.0 unx      687 b- defN 23-Jun-16 08:59 odoo/addons/l10n_ec_account_edi/tests/test_l10n_ec_edi_key_type.py
+-rw-r--r--  2.0 unx    10707 b- defN 23-Jun-16 08:59 odoo/addons/l10n_ec_account_edi/tests/test_l10n_ec_edi_liquidation.py
+-rw-r--r--  2.0 unx    12377 b- defN 23-Jun-16 08:59 odoo/addons/l10n_ec_account_edi/tests/test_l10n_ec_edi_out_invoice.py
+-rw-r--r--  2.0 unx     2132 b- defN 23-Jun-16 08:59 odoo/addons/l10n_ec_account_edi/tests/test_l10n_ec_mail.py
+-rw-r--r--  2.0 unx     3299 b- defN 23-Jun-16 08:59 odoo/addons/l10n_ec_account_edi/tests/certificates/test.p12
+-rw-r--r--  2.0 unx     4076 b- defN 23-Jun-16 08:59 odoo/addons/l10n_ec_account_edi/views/account_edi_document_view.xml
+-rw-r--r--  2.0 unx    10295 b- defN 23-Jun-16 08:59 odoo/addons/l10n_ec_account_edi/views/account_move_view.xml
+-rw-r--r--  2.0 unx      791 b- defN 23-Jun-16 08:59 odoo/addons/l10n_ec_account_edi/views/menu_root.xml
+-rw-r--r--  2.0 unx     7196 b- defN 23-Jun-16 08:59 odoo/addons/l10n_ec_account_edi/views/res_config_settings_view.xml
+-rw-r--r--  2.0 unx     4533 b- defN 23-Jun-16 08:59 odoo/addons/l10n_ec_account_edi/views/sri_key_type_view.xml
+-rw-r--r--  2.0 unx       69 b- defN 23-Jun-16 08:59 odoo/addons/l10n_ec_account_edi/wizard/__init__.py
+-rw-r--r--  2.0 unx      583 b- defN 23-Jun-16 08:59 odoo/addons/l10n_ec_account_edi/wizard/account_debit_note.py
+-rw-r--r--  2.0 unx      289 b- defN 23-Jun-16 08:59 odoo/addons/l10n_ec_account_edi/wizard/account_move_reversal.py
+-rw-r--r--  2.0 unx      850 b- defN 23-Jun-16 08:59 odoo/addons/l10n_ec_account_edi/wizard/account_move_reversal_view.xml
+-rw-r--r--  2.0 unx      825 b- defN 23-Jun-16 08:59 odoo_addon_l10n_ec_account_edi-15.0.1.1.0.dist-info/METADATA
+-rw-r--r--  2.0 unx       92 b- defN 23-Jun-16 08:59 odoo_addon_l10n_ec_account_edi-15.0.1.1.0.dist-info/WHEEL
+-rw-r--r--  2.0 unx        5 b- defN 23-Jun-16 08:59 odoo_addon_l10n_ec_account_edi-15.0.1.1.0.dist-info/top_level.txt
+?rw-rw-r--  2.0 unx     7978 b- defN 23-Jun-16 08:59 odoo_addon_l10n_ec_account_edi-15.0.1.1.0.dist-info/RECORD
+68 files, 630840 bytes uncompressed, 109372 bytes compressed:  82.7%
```

## zipnote {}

```diff
@@ -3,17 +3,23 @@
 
 Filename: odoo/addons/l10n_ec_account_edi/__init__.py
 Comment: 
 
 Filename: odoo/addons/l10n_ec_account_edi/__manifest__.py
 Comment: 
 
+Filename: odoo/addons/l10n_ec_account_edi/data/cron_send_email_electronic_documents.xml
+Comment: 
+
 Filename: odoo/addons/l10n_ec_account_edi/data/edi_format_data.xml
 Comment: 
 
+Filename: odoo/addons/l10n_ec_account_edi/data/email_template_edi_invoice.xml
+Comment: 
+
 Filename: odoo/addons/l10n_ec_account_edi/data/edi_templates/edi_credit_note.xml
 Comment: 
 
 Filename: odoo/addons/l10n_ec_account_edi/data/edi_templates/edi_debit_note.xml
 Comment: 
 
 Filename: odoo/addons/l10n_ec_account_edi/data/edi_templates/edi_info_tributaria_data.xml
@@ -78,14 +84,17 @@
 
 Filename: odoo/addons/l10n_ec_account_edi/models/account_move.py
 Comment: 
 
 Filename: odoo/addons/l10n_ec_account_edi/models/account_move_line.py
 Comment: 
 
+Filename: odoo/addons/l10n_ec_account_edi/models/additional_information.py
+Comment: 
+
 Filename: odoo/addons/l10n_ec_account_edi/models/res_company.py
 Comment: 
 
 Filename: odoo/addons/l10n_ec_account_edi/models/res_config_settings.py
 Comment: 
 
 Filename: odoo/addons/l10n_ec_account_edi/models/sri_key_type.py
@@ -144,14 +153,17 @@
 
 Filename: odoo/addons/l10n_ec_account_edi/tests/test_l10n_ec_edi_liquidation.py
 Comment: 
 
 Filename: odoo/addons/l10n_ec_account_edi/tests/test_l10n_ec_edi_out_invoice.py
 Comment: 
 
+Filename: odoo/addons/l10n_ec_account_edi/tests/test_l10n_ec_mail.py
+Comment: 
+
 Filename: odoo/addons/l10n_ec_account_edi/tests/certificates/test.p12
 Comment: 
 
 Filename: odoo/addons/l10n_ec_account_edi/views/account_edi_document_view.xml
 Comment: 
 
 Filename: odoo/addons/l10n_ec_account_edi/views/account_move_view.xml
@@ -174,20 +186,20 @@
 
 Filename: odoo/addons/l10n_ec_account_edi/wizard/account_move_reversal.py
 Comment: 
 
 Filename: odoo/addons/l10n_ec_account_edi/wizard/account_move_reversal_view.xml
 Comment: 
 
-Filename: odoo_addon_l10n_ec_account_edi-15.0.1.0.1.dist-info/METADATA
+Filename: odoo_addon_l10n_ec_account_edi-15.0.1.1.0.dist-info/METADATA
 Comment: 
 
-Filename: odoo_addon_l10n_ec_account_edi-15.0.1.0.1.dist-info/WHEEL
+Filename: odoo_addon_l10n_ec_account_edi-15.0.1.1.0.dist-info/WHEEL
 Comment: 
 
-Filename: odoo_addon_l10n_ec_account_edi-15.0.1.0.1.dist-info/top_level.txt
+Filename: odoo_addon_l10n_ec_account_edi-15.0.1.1.0.dist-info/top_level.txt
 Comment: 
 
-Filename: odoo_addon_l10n_ec_account_edi-15.0.1.0.1.dist-info/RECORD
+Filename: odoo_addon_l10n_ec_account_edi-15.0.1.1.0.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## odoo/addons/l10n_ec_account_edi/__manifest__.py

```diff
@@ -2,27 +2,29 @@
     "name": "Electronic Ecuadorian Localization",
     "summary": "Electronic data interchange adapted Ecuadorian localization",
     "category": "Account",
     "author": "Odoo Community Association (OCA), "
     "Carlos Lopez, Renan Nazate, Yazber Romero, Luis Romero, Jorge Quiguango",
     "website": "https://github.com/OCA/l10n-ecuador",
     "license": "AGPL-3",
-    "version": "15.0.1.0.1",
+    "version": "15.0.1.1.0",
     "depends": ["account", "account_edi", "l10n_ec", "l10n_ec_base"],
     "external_dependencies": {
         "python": ["cryptography==36.0.0", "xmlsig==0.1.9", "xades==0.2.4", "zeep"]
     },
     "data": [
         "security/ir.model.access.csv",
         "data/edi_format_data.xml",
         "data/edi_templates/edi_info_tributaria_data.xml",
         "data/edi_templates/edi_invoice.xml",
         "data/edi_templates/edi_liquidation.xml",
         "data/edi_templates/edi_credit_note.xml",
         "data/edi_templates/edi_debit_note.xml",
+        "data/cron_send_email_electronic_documents.xml",
+        "data/email_template_edi_invoice.xml",
         "report/edi_report_templates.xml",
         "report/report_edi_invoice.xml",
         "report/report_edi_liquidation.xml",
         "report/report_edi_credit_note.xml",
         "report/report_invoice.xml",
         "report/report_edi_debit_note.xml",
         "wizard/account_move_reversal_view.xml",
```

## odoo/addons/l10n_ec_account_edi/data/edi_templates/edi_info_tributaria_data.xml

 * *Format-specific differences are supported for XML files but no file-specific differences were detected; falling back to a binary diff. file(1) reports: XML 1.0 document, ASCII text*

```diff
@@ -67,18 +67,18 @@
 00000420: 696e 666f 4164 6963 696f 6e61 6c22 2074  infoAdicional" t
 00000430: 2d61 733d 2263 616d 706f 4164 6963 696f  -as="campoAdicio
 00000440: 6e61 6c22 3e0a 2020 2020 2020 2020 2020  nal">.          
 00000450: 2020 2020 2020 3c63 616d 706f 4164 6963        <campoAdic
 00000460: 696f 6e61 6c20 742d 6174 742d 6e6f 6d62  ional t-att-nomb
 00000470: 7265 3d22 6361 6d70 6f41 6469 6369 6f6e  re="campoAdicion
 00000480: 616c 2e67 6574 2827 6e61 6d65 2729 223e  al.get('name')">
-00000490: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-000004a0: 2020 2020 203c 7420 742d 6f75 743d 2263       <t t-out="c
-000004b0: 616d 706f 4164 6963 696f 6e61 6c2e 6765  ampoAdicional.ge
-000004c0: 7428 2764 6573 6372 6970 7469 6f6e 2729  t('description')
-000004d0: 2220 2f3e 0a20 2020 2020 2020 2020 2020  " />.           
-000004e0: 2020 2020 203c 2f63 616d 706f 4164 6963       </campoAdic
-000004f0: 696f 6e61 6c3e 0a20 2020 2020 2020 2020  ional>.         
-00000500: 2020 203c 2f74 3e0a 2020 2020 2020 2020     </t>.        
-00000510: 3c2f 696e 666f 4164 6963 696f 6e61 6c3e  </infoAdicional>
-00000520: 0a20 2020 203c 2f74 656d 706c 6174 653e  .    </template>
-00000530: 0a3c 2f6f 646f 6f3e 0a                   .</odoo>.
+00000490: 3c74 0a20 2020 2020 2020 2020 2020 2020  <t.             
+000004a0: 2020 2020 2020 2020 2020 2074 2d6f 7574             t-out
+000004b0: 3d22 6361 6d70 6f41 6469 6369 6f6e 616c  ="campoAdicional
+000004c0: 2e67 6574 2827 6465 7363 7269 7074 696f  .get('descriptio
+000004d0: 6e27 2922 0a20 2020 2020 2020 2020 2020  n')".           
+000004e0: 2020 2020 2020 2020 202f 3e3c 2f63 616d           /></cam
+000004f0: 706f 4164 6963 696f 6e61 6c3e 0a20 2020  poAdicional>.   
+00000500: 2020 2020 2020 2020 203c 2f74 3e0a 2020           </t>.  
+00000510: 2020 2020 2020 3c2f 696e 666f 4164 6963        </infoAdic
+00000520: 696f 6e61 6c3e 0a20 2020 203c 2f74 656d  ional>.    </tem
+00000530: 706c 6174 653e 0a3c 2f6f 646f 6f3e 0a    plate>.</odoo>.
```

## odoo/addons/l10n_ec_account_edi/i18n/l10n_ec_account_edi.pot

```diff
@@ -261,14 +261,19 @@
 #: model:ir.model.fields,field_description:l10n_ec_account_edi.field_account_edi_document__l10n_ec_xml_access_key
 #: model:ir.model.fields,field_description:l10n_ec_account_edi.field_account_move__l10n_ec_authorization_date
 #: model:ir.model.fields,field_description:l10n_ec_account_edi.field_account_payment__l10n_ec_authorization_date
 msgid "Access Key(EC)"
 msgstr ""
 
 #. module: l10n_ec_account_edi
+#: model:ir.model.fields,field_description:l10n_ec_account_edi.field_l10n_ec_additional_information__move_id
+msgid "Account Move"
+msgstr ""
+
+#. module: l10n_ec_account_edi
 #: model:ir.model,name:l10n_ec_account_edi.model_account_move_reversal
 msgid "Account Move Reversal"
 msgstr ""
 
 #. module: l10n_ec_account_edi
 #: model:ir.model.fields,field_description:l10n_ec_account_edi.field_sri_key_type__active
 msgid "Active?"
@@ -276,14 +281,26 @@
 
 #. module: l10n_ec_account_edi
 #: model:ir.model,name:l10n_ec_account_edi.model_account_debit_note
 msgid "Add Debit Note wizard"
 msgstr ""
 
 #. module: l10n_ec_account_edi
+#: model_terms:ir.ui.view,arch_db:l10n_ec_account_edi.view_move_form_additional_information_extend
+msgid "Additional Info"
+msgstr ""
+
+#. module: l10n_ec_account_edi
+#: model:ir.model.fields,field_description:l10n_ec_account_edi.field_account_bank_statement_line__l10n_ec_additional_information_move_ids
+#: model:ir.model.fields,field_description:l10n_ec_account_edi.field_account_move__l10n_ec_additional_information_move_ids
+#: model:ir.model.fields,field_description:l10n_ec_account_edi.field_account_payment__l10n_ec_additional_information_move_ids
+msgid "Additional Information"
+msgstr ""
+
+#. module: l10n_ec_account_edi
 #: model:ir.model.fields,help:l10n_ec_account_edi.field_account_bank_statement_line__l10n_latam_internal_type
 #: model:ir.model.fields,help:l10n_ec_account_edi.field_account_move__l10n_latam_internal_type
 #: model:ir.model.fields,help:l10n_ec_account_edi.field_account_payment__l10n_latam_internal_type
 msgid ""
 "Analog to odoo account.move.move_type but with more options allowing to "
 "identify the kind of document we are working with. (not only related to "
 "account.move, could be for documents of other models like stock.picking)"
@@ -354,30 +371,32 @@
 msgid "Create a vendor liquidation of purchases"
 msgstr ""
 
 #. module: l10n_ec_account_edi
 #: model_terms:ir.actions.act_window,help:l10n_ec_account_edi.action_move_debit_note_type
 msgid ""
 "Create debit note, register payments and keep track of the discussions with your\n"
-"                    vendors."
+"                vendors."
 msgstr ""
 
 #. module: l10n_ec_account_edi
 #: model_terms:ir.actions.act_window,help:l10n_ec_account_edi.action_move_liquidation_of_purchases_type
 msgid ""
 "Create liquidation of purchases, register payments and keep track of the discussions with your\n"
-"                    vendors."
+"                vendors."
 msgstr ""
 
 #. module: l10n_ec_account_edi
+#: model:ir.model.fields,field_description:l10n_ec_account_edi.field_l10n_ec_additional_information__create_uid
 #: model:ir.model.fields,field_description:l10n_ec_account_edi.field_sri_key_type__create_uid
 msgid "Created by"
 msgstr ""
 
 #. module: l10n_ec_account_edi
+#: model:ir.model.fields,field_description:l10n_ec_account_edi.field_l10n_ec_additional_information__create_date
 #: model:ir.model.fields,field_description:l10n_ec_account_edi.field_sri_key_type__create_date
 msgid "Created on"
 msgstr ""
 
 #. module: l10n_ec_account_edi
 #: model_terms:ir.ui.view,arch_db:l10n_ec_account_edi.res_config_settings_l10n_ec_edi
 msgid "Credit Note"
@@ -443,21 +462,27 @@
 #: model_terms:ir.ui.view,arch_db:l10n_ec_account_edi.e_credit_note_document_body
 #: model_terms:ir.ui.view,arch_db:l10n_ec_account_edi.e_invoice_document_body
 #: model_terms:ir.ui.view,arch_db:l10n_ec_account_edi.e_liquidation_document_body
 msgid "Descripción"
 msgstr ""
 
 #. module: l10n_ec_account_edi
+#: model:ir.model.fields,field_description:l10n_ec_account_edi.field_l10n_ec_additional_information__description
+msgid "Description"
+msgstr ""
+
+#. module: l10n_ec_account_edi
 #: model_terms:ir.ui.view,arch_db:l10n_ec_account_edi.e_credit_note_document_body
 #: model_terms:ir.ui.view,arch_db:l10n_ec_account_edi.e_invoice_document_body
 #: model_terms:ir.ui.view,arch_db:l10n_ec_account_edi.e_liquidation_document_body
 msgid "Descuento"
 msgstr ""
 
 #. module: l10n_ec_account_edi
+#: model:ir.model.fields,field_description:l10n_ec_account_edi.field_l10n_ec_additional_information__display_name
 #: model:ir.model.fields,field_description:l10n_ec_account_edi.field_sri_key_type__display_name
 msgid "Display Name"
 msgstr ""
 
 #. module: l10n_ec_account_edi
 #: model:ir.model.fields,field_description:l10n_ec_account_edi.field_account_edi_document__l10n_ec_document_date
 msgid "Document Emission Date"
@@ -587,14 +612,15 @@
 
 #. module: l10n_ec_account_edi
 #: model_terms:ir.ui.view,arch_db:l10n_ec_account_edi.electronic_report_common_payment_info
 msgid "Forma de Pago"
 msgstr ""
 
 #. module: l10n_ec_account_edi
+#: model:ir.model.fields,field_description:l10n_ec_account_edi.field_l10n_ec_additional_information__id
 #: model:ir.model.fields,field_description:l10n_ec_account_edi.field_sri_key_type__id
 msgid "ID"
 msgstr ""
 
 #. module: l10n_ec_account_edi
 #: code:addons/l10n_ec_account_edi/models/account_move.py:0
 #, python-format
@@ -627,14 +653,19 @@
 #: model:ir.model.fields,field_description:l10n_ec_account_edi.field_account_bank_statement_line__l10n_ec_is_edi_doc
 #: model:ir.model.fields,field_description:l10n_ec_account_edi.field_account_move__l10n_ec_is_edi_doc
 #: model:ir.model.fields,field_description:l10n_ec_account_edi.field_account_payment__l10n_ec_is_edi_doc
 msgid "Is Ecuadorian Electronic Document"
 msgstr ""
 
 #. module: l10n_ec_account_edi
+#: model:ir.model,name:l10n_ec_account_edi.model_l10n_ec_additional_information
+msgid "Is optional for electronic documents"
+msgstr ""
+
+#. module: l10n_ec_account_edi
 #: model:ir.model,name:l10n_ec_account_edi.model_account_move
 msgid "Journal Entry"
 msgstr ""
 
 #. module: l10n_ec_account_edi
 #: model:ir.model,name:l10n_ec_account_edi.model_account_move_line
 msgid "Journal Item"
@@ -657,29 +688,32 @@
 #. module: l10n_ec_account_edi
 #: model_terms:ir.ui.view,arch_db:l10n_ec_account_edi.account_edi_document_view_form
 #: model_terms:ir.ui.view,arch_db:l10n_ec_account_edi.account_edi_document_view_tree
 msgid "Last Error Message"
 msgstr ""
 
 #. module: l10n_ec_account_edi
+#: model:ir.model.fields,field_description:l10n_ec_account_edi.field_l10n_ec_additional_information____last_update
 #: model:ir.model.fields,field_description:l10n_ec_account_edi.field_sri_key_type____last_update
 msgid "Last Modified on"
 msgstr ""
 
 #. module: l10n_ec_account_edi
 #: model:ir.model.fields,field_description:l10n_ec_account_edi.field_account_edi_document__l10n_ec_last_sent_date
 msgid "Last Sent Date"
 msgstr ""
 
 #. module: l10n_ec_account_edi
+#: model:ir.model.fields,field_description:l10n_ec_account_edi.field_l10n_ec_additional_information__write_uid
 #: model:ir.model.fields,field_description:l10n_ec_account_edi.field_sri_key_type__write_uid
 msgid "Last Updated by"
 msgstr ""
 
 #. module: l10n_ec_account_edi
+#: model:ir.model.fields,field_description:l10n_ec_account_edi.field_l10n_ec_additional_information__write_date
 #: model:ir.model.fields,field_description:l10n_ec_account_edi.field_sri_key_type__write_date
 msgid "Last Updated on"
 msgstr ""
 
 #. module: l10n_ec_account_edi
 #: model_terms:ir.ui.view,arch_db:l10n_ec_account_edi.res_config_settings_l10n_ec_edi
 msgid "Limit Amount"
@@ -693,14 +727,15 @@
 #. module: l10n_ec_account_edi
 #: model:ir.actions.act_window,name:l10n_ec_account_edi.action_move_liquidation_of_purchases_type
 #: model:ir.ui.menu,name:l10n_ec_account_edi.menu_action_move_liquidation_of_purchases_type
 msgid "Liquidation of Purchase"
 msgstr ""
 
 #. module: l10n_ec_account_edi
+#: model:ir.model.fields,field_description:l10n_ec_account_edi.field_l10n_ec_additional_information__name
 #: model:ir.model.fields,field_description:l10n_ec_account_edi.field_sri_key_type__name
 msgid "Name"
 msgstr ""
 
 #. module: l10n_ec_account_edi
 #: model:ir.model.fields,field_description:l10n_ec_account_edi.field_sri_key_type__issuer_common_name
 msgid "Organization (Issuer)"
@@ -793,14 +828,21 @@
 "Select 'Sale' for customer invoices journals.\n"
 "Select 'Purchase' for vendor bills journals.\n"
 "Select 'Cash' or 'Bank' for journals that are used in customer or vendor payments.\n"
 "Select 'General' for miscellaneous operations journals."
 msgstr ""
 
 #. module: l10n_ec_account_edi
+#: model:ir.actions.server,name:l10n_ec_account_edi.ir_cron_send_email_electronic_documents_ir_actions_server
+#: model:ir.cron,cron_name:l10n_ec_account_edi.ir_cron_send_email_electronic_documents
+#: model:ir.cron,name:l10n_ec_account_edi.ir_cron_send_email_electronic_documents
+msgid "Send email with authorized electronic documents(Ecuador)"
+msgstr ""
+
+#. module: l10n_ec_account_edi
 #: model:ir.model.fields,field_description:l10n_ec_account_edi.field_sri_key_type__subject_serial_number
 msgid "Serial Number(Subject)"
 msgstr ""
 
 #. module: l10n_ec_account_edi
 #: model:ir.model.fields,field_description:l10n_ec_account_edi.field_sri_key_type__cert_serial_number
 msgid "Serial number (certificate)"
```

## odoo/addons/l10n_ec_account_edi/models/__init__.py

```diff
@@ -1,7 +1,8 @@
 from . import account_move
 from . import account_move_line
 from . import account_edi_format
 from . import account_edi_document
 from . import sri_key_type
 from . import res_company
 from . import res_config_settings
+from . import additional_information
```

## odoo/addons/l10n_ec_account_edi/models/account_edi_document.py

```diff
@@ -348,22 +348,25 @@
             xml_file = ViewModel._render_template(
                 "l10n_ec_account_edi.ec_edi_debit_note",
                 self._l10n_ec_get_info_debit_note(),
             )
         # TODO: agregar logica para demas tipos de documento
         return xml_file
 
-    def _l10n_ec_get_info_aditional(self):
-        info_data = [
-            {
-                "name": "OtroCampo",
-                "description": "Otra Informacion",
-            }
-        ]
-        # TODO: agregar logica para informacion adicional
+    def _l10n_ec_get_info_additional(self):
+        additional_information = self.move_id.l10n_ec_additional_information_move_ids
+        info_data = []
+
+        for line in additional_information:
+            info_data.append(
+                {
+                    "name": line.name,
+                    "description": line.description,
+                }
+            )
         return info_data
 
     def _l10n_ec_get_info_invoice(self):
         self.ensure_one()
         invoice = self.move_id
         date_invoice = invoice.invoice_date
         company = invoice.company_id or self.env.company
@@ -399,15 +402,15 @@
             "moneda": currency_name,
             "pagos": invoice._l10n_ec_get_payment_data(),
             "valorRetIva": False,
             "valorRetRenta": False,
             "detalles": self._l10n_ec_header_get_document_lines_edi_data(taxes_data),
             "retenciones": False,
             "infoSustitutivaGuiaRemision": False,
-            "infoAdicional": self._l10n_ec_get_info_aditional(),
+            "infoAdicional": self._l10n_ec_get_info_additional(),
         }
         invoice_data.update(self._l10n_ec_get_info_tributaria(invoice))
         return invoice_data
 
     def _l10n_ec_get_info_liquidation(self):
         self.ensure_one()
         invoice = self.move_id
@@ -443,15 +446,15 @@
             "importeTotal": self._l10n_ec_number_format(amount_total, 6),
             "moneda": currency_name,
             "pagos": invoice._l10n_ec_get_payment_data(),
             "valorRetIva": False,
             "valorRetRenta": False,
             "detalles": self._l10n_ec_header_get_document_lines_edi_data(taxes_data),
             "retenciones": False,
-            "infoAdicional": self._l10n_ec_get_info_aditional(),
+            "infoAdicional": self._l10n_ec_get_info_additional(),
         }
         invoice_data.update(self._l10n_ec_get_info_tributaria(invoice))
         return invoice_data
 
     def _l10n_ec_get_info_credit_note(self):
         self.ensure_one()
         credit_note = self.move_id
@@ -499,15 +502,15 @@
             "moneda": currency_name,
             "pagos": credit_note._l10n_ec_get_payment_data(),
             "valorRetIva": False,
             "valorRetRenta": False,
             "detalles": self._l10n_ec_header_get_document_lines_edi_data(taxes_data),
             "retenciones": False,
             "infoSustitutivaGuiaRemision": False,
-            "infoAdicional": self._l10n_ec_get_info_aditional(),
+            "infoAdicional": self._l10n_ec_get_info_additional(),
         }
         credit_note_data.update(self._l10n_ec_get_info_tributaria(credit_note))
         return credit_note_data
 
     def _l10n_ec_edi_send_xml(self, client_ws, xml_file):
         """
         Enviar a validar el comprobante con la clave de acceso
@@ -676,12 +679,49 @@
             "totalSinImpuestos": self._l10n_ec_number_format(
                 debit_note.amount_untaxed, 6
             ),
             "totalConImpuestos": self.l10n_ec_header_get_total_with_taxes(taxes_data),
             "importeTotal": self._l10n_ec_number_format(amount_total, 6),
             "pagos": debit_note._l10n_ec_get_payment_data(),
             "detalles": self._l10n_ec_header_get_document_lines_edi_data(taxes_data),
-            "infoAdicional": self._l10n_ec_get_info_aditional(),
+            "infoAdicional": self._l10n_ec_get_info_additional(),
         }
 
         debit_note_dict.update(self._l10n_ec_get_info_tributaria(debit_note))
         return debit_note_dict
+
+    @api.model
+    def l10n_ec_send_mail_to_partners(self):
+        all_companies = self.env["res.company"].search(
+            [
+                ("partner_id.country_id.code", "=", "EC"),
+                ("l10n_ec_type_environment", "=", "production"),
+            ]
+        )
+        for company in all_companies:
+            self.with_company(company).l10n_ec_send_mail_to_partner()
+        return True
+
+    @api.model
+    def l10n_ec_send_mail_to_partner(self):
+        commom_domain = [
+            ("state", "=", "posted"),
+            ("is_move_sent", "=", False),
+            ("l10n_ec_authorization_date", "!=", False),
+        ]
+        account_moves = self.env["account.move"].search(
+            commom_domain
+            + [
+                ("partner_id.vat", "not in", ["9999999999999", "9999999999"]),
+            ]
+        )
+        for account_move in account_moves:
+            account_move.l10n_ec_send_email()
+
+        # Update documents with final consumer
+        account_moves_with_final_consumer = self.env["account.move"].search(
+            commom_domain
+            + [
+                ("partner_id.vat", "in", ["9999999999999", "9999999999"]),
+            ]
+        )
+        account_moves_with_final_consumer.write({"is_move_sent": True})
```

## odoo/addons/l10n_ec_account_edi/models/account_move.py

```diff
@@ -47,14 +47,18 @@
     l10n_ec_legacy_document_date = fields.Date(string="External Document Date")
     l10n_ec_legacy_document_number = fields.Char(string="External Document Number")
     l10n_ec_legacy_document_authorization = fields.Char(
         string="External Authorization Number", size=49
     )
     l10n_ec_reason = fields.Char(string="Refund Reason", size=300)
 
+    l10n_ec_additional_information_move_ids = fields.One2many(
+        "l10n.ec.additional.information", "move_id", string="Additional Information"
+    )
+
     @api.depends("invoice_date", "invoice_date_due")
     def _compute_l10n_ec_credit_days(self):
         now = fields.Date.context_today(self)
         for invoice in self:
             date_invoice = invoice.invoice_date or now
             date_due = invoice.invoice_date_due or date_invoice
             invoice.l10n_ec_credit_days = (date_due - date_invoice).days
@@ -302,7 +306,18 @@
         move_vals = super()._reverse_move_vals(default_values, cancel)
         move_vals.update(
             l10n_ec_legacy_document_number=self.l10n_latam_document_number,
             l10n_ec_legacy_document_date=self.invoice_date,
             l10n_ec_legacy_document_authorization=self.l10n_ec_xml_access_key,
         )
         return move_vals
+
+    def l10n_ec_send_email(self):
+        WizardInvoiceSent = self.env["account.invoice.send"]
+        self.ensure_one()
+        res = self.with_context(discard_logo_check=True).action_invoice_sent()
+        context = res["context"]
+        send_mail = WizardInvoiceSent.with_context(**context).create({})
+        # enviar factura automaticamente por correo
+        # simular onchange y accion
+        send_mail.onchange_template_id()
+        send_mail.send_and_print_action()
```

## odoo/addons/l10n_ec_account_edi/report/edi_report_templates.xml

### odoo/addons/l10n_ec_account_edi/report/edi_report_templates.xml

```diff
@@ -134,19 +134,19 @@
         <br/>
       </t>
       <t t-if="partner.email or (partner.child_ids and partner.child_ids[0].email)" name="email">
         <strong>Email:</strong>
         <span t-out="partner.email or (partner.child_ids and partner.child_ids[0].email) or ''"/>
         <br/>
       </t>
-      <t t-if="'l10n_ec_info_aditional_ids' in o">
-        <t t-foreach="o.l10n_ec_info_aditional_ids" t-as="info_aditional">
-          <strong t-field="info_aditional.name"/>
+      <t t-if="'l10n_ec_additional_information_move_ids' in o">
+        <t t-foreach="o.l10n_ec_additional_information_move_ids" t-as="info_additional">
+          <strong t-field="info_additional.name"/>
           :
-          <span t-field="info_aditional.description"/>
+          <span t-field="info_additional.description"/>
           <br/>
         </t>
       </t>
     </div>
   </template>
   <template id="electronic_report_common_payment_info">
     <table class="table table-sm table-bordered-black small">
```

## odoo/addons/l10n_ec_account_edi/security/ir.model.access.csv

```diff
@@ -1,3 +1,4 @@
 "id","name","model_id:id","group_id:id","perm_read","perm_write","perm_create","perm_unlink"
 access_model_sri_key_type_user,sri.key.type.user,model_sri_key_type,base.group_user,1,0,0,0
 access_model_sri_key_type_admin,sri.key.type.admin,model_sri_key_type,base.group_system,1,1,1,0
+l10n_ec_account_edi.access_l10n_ec_additional_information,access_l10n_ec_additional_information,l10n_ec_account_edi.model_l10n_ec_additional_information,base.group_user,1,1,1,1
```

## odoo/addons/l10n_ec_account_edi/tests/__init__.py

```diff
@@ -2,7 +2,8 @@
 from . import test_edi_common
 from . import test_edi_format
 from . import test_l10n_ec_edi_key_type
 from . import test_l10n_ec_edi_out_invoice
 from . import test_l10n_ec_edi_liquidation
 from . import test_l10n_ec_edi_credit_note
 from . import test_l10n_ec_edi_debit_note
+from . import test_l10n_ec_mail
```

## odoo/addons/l10n_ec_account_edi/tests/test_common.py

```diff
@@ -66,15 +66,23 @@
                 "vat": "12345678",
                 "l10n_latam_identification_type_id": cls.env.ref(
                     "l10n_ec.ec_passport"
                 ).id,
                 "country_id": cls.env.ref("base.co").id,
             }
         )
-
+        cls.partner_with_email = cls.Partner.create(
+            {
+                "name": "SERVICIO DE RENTAS INTERNAS",
+                "vat": "1760013210001",
+                "l10n_latam_identification_type_id": cls.env.ref("l10n_ec.ec_ruc").id,
+                "country_id": cls.env.ref("base.ec").id,
+                "email": "my_email@test.com.ec",
+            }
+        )
         # Impuestos
         cls.tax_group_vat = cls.TaxGroup.search(
             [("l10n_ec_type", "=", "vat12")], limit=1
         )
         cls.taxes_zero_vat = cls.Tax.search(
             [("tax_group_id.l10n_ec_type", "=", "zero_vat")], limit=2
         )
```

## odoo/addons/l10n_ec_account_edi/tests/test_l10n_ec_edi_out_invoice.py

```diff
@@ -260,7 +260,25 @@
         self._setup_edi_company_ec()
         invoice = self._l10n_ec_prepare_edi_out_invoice()
         with Form(invoice) as form:
             with form.invoice_line_ids.edit(0) as line:
                 line.quantity = 0
         with self.assertRaises(UserError):
             invoice.action_post()
+
+    def test_l10n_ec_out_invoice_with_additional_info(self):
+        """Crear factura electronica con informacion adicional"""
+        self._setup_edi_company_ec()
+        invoice = self._l10n_ec_prepare_edi_out_invoice(auto_post=False)
+        with Form(invoice) as form:
+            with form.l10n_ec_additional_information_move_ids.new() as line:
+                line.name = "Test"
+                line.description = "ABC"
+        invoice.action_post()
+        edi_doc = invoice._get_edi_document(self.edi_format)
+        edi_doc._process_documents_web_services(with_commit=False)
+        self.assertEqual(invoice.state, "posted")
+        self.assertTrue(edi_doc.l10n_ec_xml_access_key)
+        self.assertEqual(len(invoice.l10n_ec_additional_information_move_ids), 1)
+        self.assertEqual(
+            invoice.l10n_ec_additional_information_move_ids[0].name, "Test"
+        )
```

## odoo/addons/l10n_ec_account_edi/views/account_move_view.xml

### odoo/addons/l10n_ec_account_edi/views/account_move_view.xml

```diff
@@ -27,40 +27,67 @@
     </field>
   </record>
   <!--Modifica Dominio y Contexto de Facturas de Proveedor para separar Facturas de Liquidacion de Compras-->
   <record id="account.action_move_in_invoice_type" model="ir.actions.act_window">
     <field name="domain">[('move_type', '=', 'in_invoice'), ('l10n_latam_internal_type', '=', 'invoice')]</field>
     <field name="context">{'default_move_type': 'in_invoice', 'internal_type': 'invoice'}</field>
   </record>
+  <!-- Additional Information -->
+  <record id="view_move_form_additional_information_extend" model="ir.ui.view">
+    <field name="name">account.move.form</field>
+    <field name="model">account.move</field>
+    <field name="inherit_id" ref="account.view_move_form"/>
+    <field name="arch" type="xml">
+      <xpath expr="//page[@id='other_tab']" position="before">
+        <page string="Additional Info" name="l10n_ec_additional_information" attrs="{'invisible':[('move_type', 'not in', ('out_invoice', 'out_refund'))]}">
+          <field name="l10n_ec_additional_information_move_ids" attrs="{'readonly': [('state', '!=', 'draft')]}">
+            <tree editable="bottom">
+              <field name="name"/>
+              <field name="description"/>
+            </tree>
+            <form>
+              <group>
+                <field name="name"/>
+                <field name="description"/>
+              </group>
+            </form>
+          </field>
+        </page>
+      </xpath>
+    </field>
+  </record>
   <!--Crear vista principal para liquidacion de compras-->
   <record id="account_invoice_liquidation_purchase_form_view" model="ir.ui.view">
     <field name="name">account.invoice.liquidation.form</field>
     <field name="model">account.move</field>
     <field name="priority" eval="50"/>
     <field name="mode">primary</field>
     <field name="inherit_id" ref="account.view_move_form"/>
     <field name="arch" type="xml">
       <xpath expr="//field[@name='l10n_ec_electronic_authorization']" position="attributes">
         <attribute name="attrs">{'invisible': True,
-                         'required': False}</attribute>
+                    'required': False}</attribute>
+      </xpath>
+      <xpath expr="//page[@name='l10n_ec_additional_information']" position="attributes">
+        <attribute name="attrs">{'invisible': False}</attribute>
       </xpath>
     </field>
   </record>
   <record id="action_move_liquidation_of_purchases_type" model="ir.actions.act_window">
     <field name="name">Liquidation of Purchase</field>
     <field name="res_model">account.move</field>
     <field name="view_mode">tree,kanban,form</field>
     <field name="view_id" ref="account.view_invoice_tree"/>
     <field name="search_view_id" ref="account.view_account_invoice_filter"/>
     <field name="domain">[('move_type', '=', 'in_invoice'), ('l10n_latam_internal_type', '=', 'purchase_liquidation')]</field>
     <field name="context">{'default_move_type': 'in_invoice', 'internal_type': 'purchase_liquidation'}</field>
     <field name="help" type="html">
       <p class="o_view_nocontent_smiling_face">Create a vendor liquidation of purchases</p>
       <p>Create liquidation of purchases, register payments and keep track of the discussions with your
-                    vendors.</p>
+                vendors.</p>
     </field>
   </record>
   <record id="action_move_liquidation_purchase_tree" model="ir.actions.act_window.view">
     <field name="sequence" eval="1"/>
     <field name="view_mode">tree</field>
     <field name="view_id" ref="account.view_invoice_tree"/>
     <field name="act_window_id" ref="action_move_liquidation_of_purchases_type"/>
@@ -85,15 +112,15 @@
     <field name="view_id" ref="account.view_invoice_tree"/>
     <field name="search_view_id" ref="account.view_account_invoice_filter"/>
     <field name="domain">[('move_type', '=', 'out_invoice'), ('l10n_latam_internal_type', '=', 'debit_note')]</field>
     <field name="context">{'default_move_type': 'out_invoice', 'internal_type': 'debit_note'}</field>
     <field name="help" type="html">
       <p class="o_view_nocontent_smiling_face">Create a debit note</p>
       <p>Create debit note, register payments and keep track of the discussions with your
-                    vendors.</p>
+                vendors.</p>
     </field>
   </record>
   <record id="action_move_debit_note_tree" model="ir.actions.act_window.view">
     <field name="sequence" eval="1"/>
     <field name="view_mode">tree</field>
     <field name="view_id" ref="account.view_invoice_tree"/>
     <field name="act_window_id" ref="action_move_debit_note_type"/>
```

## Comparing `odoo_addon_l10n_ec_account_edi-15.0.1.0.1.dist-info/METADATA` & `odoo_addon_l10n_ec_account_edi-15.0.1.1.0.dist-info/METADATA`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: odoo-addon-l10n-ec-account-edi
-Version: 15.0.1.0.1
+Version: 15.0.1.1.0
 Summary: Electronic data interchange adapted Ecuadorian localization
 Home-page: https://github.com/OCA/l10n-ecuador
 Author: Odoo Community Association (OCA), Carlos Lopez, Renan Nazate, Yazber Romero, Luis Romero, Jorge Quiguango
 Author-email: support@odoo-community.org
 License: AGPL-3
 Platform: UNKNOWN
 Classifier: Programming Language :: Python
```

## Comparing `odoo_addon_l10n_ec_account_edi-15.0.1.0.1.dist-info/RECORD` & `odoo_addon_l10n_ec_account_edi-15.0.1.1.0.dist-info/RECORD`

 * *Files 4% similar despite different names*

```diff
@@ -1,14 +1,16 @@
 odoo/addons/l10n_ec_account_edi/README.rst,sha256=47DEQpj8HBSa-_TImW-5JCeuQeRkm5NMpJWZG3hSuFU,0
 odoo/addons/l10n_ec_account_edi/__init__.py,sha256=UHmJ4-K0Z9SSh8ZnvYvgtSBkR3jQZK1N3-YPO2pkNoo,63
-odoo/addons/l10n_ec_account_edi/__manifest__.py,sha256=DsLoX1nDv57TMw_VvkggpUh6WErJcBzdOOFxnWHK_MY,1639
+odoo/addons/l10n_ec_account_edi/__manifest__.py,sha256=3cF5Yg_r3v5ieoCxeAhWO6OlqP8kcdmRfmfo5hIjHvc,1743
+odoo/addons/l10n_ec_account_edi/data/cron_send_email_electronic_documents.xml,sha256=WKzLXW3n3HbrZQAkbgfoywE4fM1MdlDBzNTztO_ELjI,891
 odoo/addons/l10n_ec_account_edi/data/edi_format_data.xml,sha256=8avT5XUwyVM5YSKQNhzHkWNSe8NKGOUYOTahzVaf6s0,240
+odoo/addons/l10n_ec_account_edi/data/email_template_edi_invoice.xml,sha256=2TZH50YE34nD1uaeFDi_SitalULmDpvNIb9UbmACWc8,213
 odoo/addons/l10n_ec_account_edi/data/edi_templates/edi_credit_note.xml,sha256=IYvuo70m893id0kLTAIpNRKDJr-GNwvU3bFStHuMZ6w,3880
 odoo/addons/l10n_ec_account_edi/data/edi_templates/edi_debit_note.xml,sha256=F6csQ6WNh5KHQnCuA7FtJRDmOz9MghtyJ4-AOyetRJM,2687
-odoo/addons/l10n_ec_account_edi/data/edi_templates/edi_info_tributaria_data.xml,sha256=QdceDqviN19zZF2rTgKMASEwJxuU-0RmYZWeU6Pzo1I,1337
+odoo/addons/l10n_ec_account_edi/data/edi_templates/edi_info_tributaria_data.xml,sha256=94ZyaGFy20-M6_J5DpG-KqP9uidPaOY22NgHQezL3wc,1343
 odoo/addons/l10n_ec_account_edi/data/edi_templates/edi_invoice.xml,sha256=HPym_0hJoV8k2NpbOIUVhXilpXFPGwZUQRKIKnukI5Y,4444
 odoo/addons/l10n_ec_account_edi/data/edi_templates/edi_liquidation.xml,sha256=XrQYgaZt0ssARRq7y4YMDtmiwk5RbFWSkAqUMP9d3Ds,4334
 odoo/addons/l10n_ec_account_edi/data/xsd/ComprobanteRetencion_V1.0.0.xsd,sha256=yzChNaPe4H7nwiRDQuM8AcCtnmouWuSneq_BRq-cU1A,15160
 odoo/addons/l10n_ec_account_edi/data/xsd/ComprobanteRetencion_V2.0.0.xsd,sha256=o0sc5JFJE0V-nSztcaa94MEU3wUtAAUdW5keJs-SBEU,26969
 odoo/addons/l10n_ec_account_edi/data/xsd/GuiaRemision_V1.0.0.xsd,sha256=NepKeRvXV6lCq6PEeygzYIAk2U1muf4HXLE-1wf_52U,20198
 odoo/addons/l10n_ec_account_edi/data/xsd/GuiaRemision_V1.1.0.xsd,sha256=afCc1CII7Wsc3MvNdomzuyuAsH4XUCWp_7xKVWLHw-0,20198
 odoo/addons/l10n_ec_account_edi/data/xsd/LiquidacionCompra_V1.0.0.xsd,sha256=XNt3NuaL7UnTIkqGHsOoIemOpgt0OKUjYUhX1aBHCuY,27328
@@ -16,49 +18,51 @@
 odoo/addons/l10n_ec_account_edi/data/xsd/NotaCredito_V1.0.0.xsd,sha256=EEo5HsS5I4ye9TovOmLFyKm4wjyEy7GJGvPGwskkLeU,20937
 odoo/addons/l10n_ec_account_edi/data/xsd/NotaCredito_V1.1.0.xsd,sha256=zQZXh4GgbFPZVUbDQPHCIiQxYtHEgz4d5oSV-hM-HAw,20937
 odoo/addons/l10n_ec_account_edi/data/xsd/NotaDebito_V1.0.0.xsd,sha256=yLcELk1zAncfGw6Pc2ESYvSFZ0Di41ZeM7xPnAWgL5o,23726
 odoo/addons/l10n_ec_account_edi/data/xsd/factura_V1.0.0.xsd,sha256=PBAl7uzIHgJA5pwhsQoS_WCrEtcw00S2RwdBY-UoUpo,34032
 odoo/addons/l10n_ec_account_edi/data/xsd/factura_V1.1.0.xsd,sha256=vX15X0TLv-zvmVdETTzCiOZ80oMpRU__VUCHXH0hKIs,35400
 odoo/addons/l10n_ec_account_edi/data/xsd/factura_V2.0.0.xsd,sha256=iKb9E50Z9591VJhgNy-lryarhffp5X0SGW3K6Ni4bt8,38832
 odoo/addons/l10n_ec_account_edi/data/xsd/factura_V2.1.0.xsd,sha256=hac9spxWL8J9v_YT-pQMLg0kHKjYfXiEVWUEreIsu6s,39442
-odoo/addons/l10n_ec_account_edi/i18n/l10n_ec_account_edi.pot,sha256=bizyaYfEHlii9td3PYtZCZYkCh8Hzj0lxSlYf3y1mQ8,35948
-odoo/addons/l10n_ec_account_edi/models/__init__.py,sha256=9tE6k0ej0kxp63fZ7sqczuEKLKsX17qCxbiHiqghtm0,214
-odoo/addons/l10n_ec_account_edi/models/account_edi_document.py,sha256=PLyHT1kz47SqqPq_JYst353DqiZlTb89KByUFdIu1xE,29194
+odoo/addons/l10n_ec_account_edi/i18n/l10n_ec_account_edi.pot,sha256=HRThNLgYh96CcONwVyOPNR-qgO2K6dNrOmKvs0aoSf8,38352
+odoo/addons/l10n_ec_account_edi/models/__init__.py,sha256=bBJcg75smrrulSjX8fhEBSUCGliy8PWk72D4B2eel1g,251
+odoo/addons/l10n_ec_account_edi/models/account_edi_document.py,sha256=Q5mKLwfxxDtRuYAVizmEfiY2CMbKHLF0YwVPgHZlJWc,30588
 odoo/addons/l10n_ec_account_edi/models/account_edi_format.py,sha256=a4vjEPLHBjFEs7vEx6ombHSRYOqFy-XLi8_dZ-wdcL0,13990
-odoo/addons/l10n_ec_account_edi/models/account_move.py,sha256=OyNh96yEPIRuxuSmD6JHwapuBeWQcFwsYMQ6FyO7fXY,11989
+odoo/addons/l10n_ec_account_edi/models/account_move.py,sha256=p3b-JHlYOyLAGa1R_9_4TKscX4bhed266PI6sDUS7uc,12622
 odoo/addons/l10n_ec_account_edi/models/account_move_line.py,sha256=7U4FRFflkgxd1zQJawUJ3_hcbzBQ7cBcZY18-gQPp6g,3968
+odoo/addons/l10n_ec_account_edi/models/additional_information.py,sha256=QZUNV7GBwA90Iaex59SEF2Ua1GRYDUljLMKWZNCVXzY,346
 odoo/addons/l10n_ec_account_edi/models/res_company.py,sha256=6wJ10C8p3gwA2fRtEsA42K2vzXSoKpJDW31UQBgleQ8,1582
 odoo/addons/l10n_ec_account_edi/models/res_config_settings.py,sha256=o3pTdYckpgZ0HcOpNpQoApzZbSVu9TJF_P00_cYPhvk,1130
 odoo/addons/l10n_ec_account_edi/models/sri_key_type.py,sha256=biVTRyUCMdZ_DvqALwFe9cOsOhGENX-iBLL7Ihw6OcI,9386
 odoo/addons/l10n_ec_account_edi/report/__init__.py,sha256=47DEQpj8HBSa-_TImW-5JCeuQeRkm5NMpJWZG3hSuFU,0
-odoo/addons/l10n_ec_account_edi/report/edi_report_templates.xml,sha256=ZTlO8pTgQzE7mZj6akcE4-WQx6T-6Sep55G6O8VberQ,11186
+odoo/addons/l10n_ec_account_edi/report/edi_report_templates.xml,sha256=m_WLr9U0LH3T720fD8pjgRN9YtxZVTm91cewQuYDe8I,11272
 odoo/addons/l10n_ec_account_edi/report/report_edi_credit_note.xml,sha256=vbel9VM2_elSKcNnsYURJ1mPWaScAdPKOHHe8sjnZhA,4823
 odoo/addons/l10n_ec_account_edi/report/report_edi_debit_note.xml,sha256=wslJRxwayNZKzWbKSjvEYGk_wSjBnXQmNfH-gqvcyZA,3827
 odoo/addons/l10n_ec_account_edi/report/report_edi_invoice.xml,sha256=8Z6pRUOrEjxzVG1Ts4oaNIUDovkjkMK-5xPqJsTcvrE,4063
 odoo/addons/l10n_ec_account_edi/report/report_edi_liquidation.xml,sha256=3tj-WL66nXYd0kFVxVMC8t5AK0RGl8PHO7xbcu2D2PE,3961
 odoo/addons/l10n_ec_account_edi/report/report_invoice.xml,sha256=at2P92H9UynCB7rW0itl6DaM49CEIk_7tJDrgdpoLXs,5285
-odoo/addons/l10n_ec_account_edi/security/ir.model.access.csv,sha256=BU13i9f7QvFqvfVy8P2ka5Whb97Rl6Vj0cwvTkAax9c,281
+odoo/addons/l10n_ec_account_edi/security/ir.model.access.csv,sha256=eoz7YNPrczEHhQekod1Mie_3HJKf7HDchAeUw84qwUc,458
 odoo/addons/l10n_ec_account_edi/static/description/icon.png,sha256=6xBPJauaFOF0KDHfHgQopSc28kKvxMaeoQFQWZtfZDo,9455
 odoo/addons/l10n_ec_account_edi/static/src/scss/report_layout.scss,sha256=HjzFplHdWrTcqh01TNGruWUpK2EK1QSkMLHSOQghZQA,1648
-odoo/addons/l10n_ec_account_edi/tests/__init__.py,sha256=mTo8fnbpoeD6arpZzQE4WRppsB6ZNCGkdC4IEpaB3Ls,297
-odoo/addons/l10n_ec_account_edi/tests/test_common.py,sha256=jA0MN7QizyO0rU51BZrqZ7k2wj5512TXL9_Fva9Uo8A,10192
+odoo/addons/l10n_ec_account_edi/tests/__init__.py,sha256=1BhwpFSPX7G4DhtVpb2snI6JjQnY-S_BsxNQm6lCK3I,329
+odoo/addons/l10n_ec_account_edi/tests/test_common.py,sha256=ahZROTMRoUPan1Ze0wbrmUtPMPju7l9BpYUa04OFtLw,10570
 odoo/addons/l10n_ec_account_edi/tests/test_edi_common.py,sha256=wh71LZ85XktShwhKOkf0U0iiOwpRND57rW-jLP6HWAc,7264
 odoo/addons/l10n_ec_account_edi/tests/test_edi_format.py,sha256=0NdSG_HT0pbgtfXET0CyBPP2xed_tOWTKE2geLZPnCs,1044
 odoo/addons/l10n_ec_account_edi/tests/test_l10n_ec_edi_credit_note.py,sha256=iLQuSAEnbtZMUo0pmuzQMzt-0ES6HEC5Qq8bZVRo_Zw,8777
 odoo/addons/l10n_ec_account_edi/tests/test_l10n_ec_edi_debit_note.py,sha256=OulSL510Q5yNI3ig7Flmp9odN_H1VifmimahXnJLI9A,8739
 odoo/addons/l10n_ec_account_edi/tests/test_l10n_ec_edi_key_type.py,sha256=bW3vbezIxV3F5F0YpD2dclADRFtkjryxdQ3oyxVFMRI,687
 odoo/addons/l10n_ec_account_edi/tests/test_l10n_ec_edi_liquidation.py,sha256=XDV6wG6YDpek3KSvik2BLdcFg1WUQ_tnepITlc4yjqg,10707
-odoo/addons/l10n_ec_account_edi/tests/test_l10n_ec_edi_out_invoice.py,sha256=Fba6lA15RSTK3d1YDhkV2QoLnNrsn6Azk7MURp2s5K8,11492
+odoo/addons/l10n_ec_account_edi/tests/test_l10n_ec_edi_out_invoice.py,sha256=8s7Dd2v9vIfALUwY35PwY_GyMOV6Q8j5Ar5BmWJU9qI,12377
+odoo/addons/l10n_ec_account_edi/tests/test_l10n_ec_mail.py,sha256=XlXgILWdltCE5Lw5cBcJbIN-y6wiTwmvTBadUMjzKL4,2132
 odoo/addons/l10n_ec_account_edi/tests/certificates/test.p12,sha256=YnjU29tnlR2EeJfqT6qmql97fy2HmvjscflXmWFKTHY,3299
 odoo/addons/l10n_ec_account_edi/views/account_edi_document_view.xml,sha256=SXO0eYZJJ4AYqNUPPRmvO0XsCFOOMOCyMf0F9Yt2M9M,4076
-odoo/addons/l10n_ec_account_edi/views/account_move_view.xml,sha256=kaxcB2hPM75BpKirq1K6P7wO81NFRfIdlcz2RtQU6ss,8908
+odoo/addons/l10n_ec_account_edi/views/account_move_view.xml,sha256=l1758-F_PtTpiYtnmKZEBrLqRYA7gf5KMmQrYEpvwAg,10295
 odoo/addons/l10n_ec_account_edi/views/menu_root.xml,sha256=cyjsw7BH5M6vtvzRQm6VmwCJrTwphI6uicoN-7VOfdQ,791
 odoo/addons/l10n_ec_account_edi/views/res_config_settings_view.xml,sha256=YTJQZkODn6r-542I5x40F88PBjVpOWqnhaqvSQOsWuI,7196
 odoo/addons/l10n_ec_account_edi/views/sri_key_type_view.xml,sha256=jA8QVB5IDXvG913SimZMbkbdBkNIICp9YvGIKtLrjUM,4533
 odoo/addons/l10n_ec_account_edi/wizard/__init__.py,sha256=mjfud8f0cURtE6Zw8LKYT07fOksyOWa-oZZrCsGeAYc,69
 odoo/addons/l10n_ec_account_edi/wizard/account_debit_note.py,sha256=bfeBNr_gF6wk2YLJSalRvFCoOqHM_IsBM8iSlRlpzjc,583
 odoo/addons/l10n_ec_account_edi/wizard/account_move_reversal.py,sha256=PGnfgj3LfftBE_Mx3yECykuTMxNFay2AaiBrekm9lzg,289
 odoo/addons/l10n_ec_account_edi/wizard/account_move_reversal_view.xml,sha256=UChY2QRXoRCOlcIp3AZpw8oSgFYSEhXtfyLMNZ5n9go,850
-odoo_addon_l10n_ec_account_edi-15.0.1.0.1.dist-info/METADATA,sha256=yEzfHpjqxbZkMnygdDhVd6apbLwxX-Uq_9VHteqrwIw,825
-odoo_addon_l10n_ec_account_edi-15.0.1.0.1.dist-info/WHEEL,sha256=2wepM1nk4DS4eFpYrW1TTqPcoGNfHhhO_i5m4cOimbo,92
-odoo_addon_l10n_ec_account_edi-15.0.1.0.1.dist-info/top_level.txt,sha256=qBj40grFkGOfDZ2WDSw3y1RnDlgG0u8rP8pvGNdbz4w,5
-odoo_addon_l10n_ec_account_edi-15.0.1.0.1.dist-info/RECORD,,
+odoo_addon_l10n_ec_account_edi-15.0.1.1.0.dist-info/METADATA,sha256=yroUipXmzQTPaeUYKGfUbZQDdPdkkvR78NNq76GAkWI,825
+odoo_addon_l10n_ec_account_edi-15.0.1.1.0.dist-info/WHEEL,sha256=2wepM1nk4DS4eFpYrW1TTqPcoGNfHhhO_i5m4cOimbo,92
+odoo_addon_l10n_ec_account_edi-15.0.1.1.0.dist-info/top_level.txt,sha256=qBj40grFkGOfDZ2WDSw3y1RnDlgG0u8rP8pvGNdbz4w,5
+odoo_addon_l10n_ec_account_edi-15.0.1.1.0.dist-info/RECORD,,
```

