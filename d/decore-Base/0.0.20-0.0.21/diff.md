# Comparing `tmp/decore_Base-0.0.20.tar.gz` & `tmp/decore_Base-0.0.21.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "decore_Base-0.0.20.tar", last modified: Fri Jun 16 07:17:23 2023, max compression
+gzip compressed data, was "decore_Base-0.0.21.tar", last modified: Fri Jun 16 09:46:56 2023, max compression
```

## Comparing `decore_Base-0.0.20.tar` & `decore_Base-0.0.21.tar`

### file list

```diff
@@ -1,243 +1,236 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 07:17:23.316149 decore_Base-0.0.20/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 07:17:23.284149 decore_Base-0.0.20/.github/
--rw-r--r--   0 runner    (1001) docker     (123)      776 2023-06-16 07:17:11.000000 decore_Base-0.0.20/.github/FUNDING.yml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 07:17:23.284149 decore_Base-0.0.20/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (123)      436 2023-06-16 07:17:11.000000 decore_Base-0.0.20/.github/workflows/publish.yml
--rw-r--r--   0 runner    (1001) docker     (123)     2036 2023-06-16 07:17:11.000000 decore_Base-0.0.20/.gitignore
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 07:17:23.284149 decore_Base-0.0.20/.vscode/
--rw-r--r--   0 runner    (1001) docker     (123)     1244 2023-06-16 07:17:11.000000 decore_Base-0.0.20/.vscode/launch.json
--rw-r--r--   0 runner    (1001) docker     (123)      281 2023-06-16 07:17:11.000000 decore_Base-0.0.20/.vscode/settings.json
--rw-r--r--   0 runner    (1001) docker     (123)     1788 2023-06-16 07:17:11.000000 decore_Base-0.0.20/KOFI.md
--rw-r--r--   0 runner    (1001) docker     (123)    35148 2023-06-16 07:17:11.000000 decore_Base-0.0.20/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)    11734 2023-06-16 07:17:23.316149 decore_Base-0.0.20/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    10998 2023-06-16 07:17:11.000000 decore_Base-0.0.20/README.rst
--rw-r--r--   0 runner    (1001) docker     (123)    11971 2023-06-16 07:17:11.000000 decore_Base-0.0.20/README_DE.rst
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 07:17:23.284149 decore_Base-0.0.20/decore_Base.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    11734 2023-06-16 07:17:23.000000 decore_Base-0.0.20/decore_Base.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     8226 2023-06-16 07:17:23.000000 decore_Base-0.0.20/decore_Base.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-16 07:17:23.000000 decore_Base-0.0.20/decore_Base.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)     1174 2023-06-16 07:17:23.000000 decore_Base-0.0.20/decore_Base.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       12 2023-06-16 07:17:23.000000 decore_Base-0.0.20/decore_Base.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 07:17:23.288149 decore_Base-0.0.20/decore_base/
--rw-r--r--   0 runner    (1001) docker     (123)       55 2023-06-16 07:17:11.000000 decore_Base-0.0.20/decore_base/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 07:17:23.288149 decore_Base-0.0.20/decore_base/classes/
--rw-r--r--   0 runner    (1001) docker     (123)      388 2023-06-16 07:17:11.000000 decore_Base-0.0.20/decore_base/classes/decore_action.py
--rw-r--r--   0 runner    (1001) docker     (123)      319 2023-06-16 07:17:11.000000 decore_Base-0.0.20/decore_base/classes/decore_app.py
--rw-r--r--   0 runner    (1001) docker     (123)     1412 2023-06-16 07:17:11.000000 decore_Base-0.0.20/decore_base/classes/decore_base.py
--rw-r--r--   0 runner    (1001) docker     (123)      433 2023-06-16 07:17:11.000000 decore_Base-0.0.20/decore_base/classes/decore_dialog.py
--rw-r--r--   0 runner    (1001) docker     (123)      489 2023-06-16 07:17:11.000000 decore_Base-0.0.20/decore_base/classes/decore_element.py
--rw-r--r--   0 runner    (1001) docker     (123)      339 2023-06-16 07:17:11.000000 decore_Base-0.0.20/decore_base/classes/decore_function.py
--rw-r--r--   0 runner    (1001) docker     (123)     1434 2023-06-16 07:17:11.000000 decore_Base-0.0.20/decore_base/classes/decore_list.py
--rw-r--r--   0 runner    (1001) docker     (123)    15687 2023-06-16 07:17:11.000000 decore_Base-0.0.20/decore_base/classes/decore_model.py
--rw-r--r--   0 runner    (1001) docker     (123)      498 2023-06-16 07:17:11.000000 decore_Base-0.0.20/decore_base/classes/decore_object.py
--rw-r--r--   0 runner    (1001) docker     (123)     4896 2023-06-16 07:17:11.000000 decore_Base-0.0.20/decore_base/classes/decore_pool.py
--rw-r--r--   0 runner    (1001) docker     (123)     4033 2023-06-16 07:17:11.000000 decore_Base-0.0.20/decore_base/classes/decore_prompt.py
--rw-r--r--   0 runner    (1001) docker     (123)      664 2023-06-16 07:17:11.000000 decore_Base-0.0.20/decore_base/classes/decore_query.py
--rw-r--r--   0 runner    (1001) docker     (123)     1022 2023-06-16 07:17:11.000000 decore_Base-0.0.20/decore_base/classes/decore_return.py
--rw-r--r--   0 runner    (1001) docker     (123)     1536 2023-06-16 07:17:11.000000 decore_Base-0.0.20/decore_base/classes/decore_translate.py
--rw-r--r--   0 runner    (1001) docker     (123)      524 2023-06-16 07:17:11.000000 decore_Base-0.0.20/decore_base/classes/decore_view.py
--rw-r--r--   0 runner    (1001) docker     (123)      439 2023-06-16 07:17:11.000000 decore_Base-0.0.20/decore_base/classes/decore_widget.py
--rw-r--r--   0 runner    (1001) docker     (123)    17032 2023-06-16 07:17:11.000000 decore_Base-0.0.20/decore_base/decore.py
--rw-r--r--   0 runner    (1001) docker     (123)     2231 2023-06-16 07:17:11.000000 decore_Base-0.0.20/decore_base/globals.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 07:17:23.288149 decore_Base-0.0.20/decore_base/library/
--rw-r--r--   0 runner    (1001) docker     (123)      189 2023-06-16 07:17:11.000000 decore_Base-0.0.20/decore_base/library/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 07:17:23.288149 decore_Base-0.0.20/decore_base/library/particl_market/
--rw-r--r--   0 runner    (1001) docker     (123)       42 2023-06-16 07:17:11.000000 decore_Base-0.0.20/decore_base/library/particl_market/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    10733 2023-06-16 07:17:11.000000 decore_Base-0.0.20/decore_base/library/particl_market/particl_market.py
--rw-r--r--   0 runner    (1001) docker     (123)     3995 2023-06-16 07:17:11.000000 decore_Base-0.0.20/decore_base/library/powershell.py
--rw-r--r--   0 runner    (1001) docker     (123)    90489 2023-06-16 07:17:11.000000 decore_Base-0.0.20/decore_base/library/powershell2.py
--rw-r--r--   0 runner    (1001) docker     (123)      616 2023-06-16 07:17:11.000000 decore_Base-0.0.20/decore_base/library/return_value.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 07:17:23.288149 decore_Base-0.0.20/decore_base/library/roaster/
--rw-r--r--   0 runner    (1001) docker     (123)       91 2023-06-16 07:17:11.000000 decore_Base-0.0.20/decore_base/library/roaster/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4122 2023-06-16 07:17:11.000000 decore_Base-0.0.20/decore_base/library/roaster/roaster_client.py
--rw-r--r--   0 runner    (1001) docker     (123)    12453 2023-06-16 07:17:11.000000 decore_Base-0.0.20/decore_base/library/roaster/roaster_functions.py
--rw-r--r--   0 runner    (1001) docker     (123)     2186 2023-06-16 07:17:11.000000 decore_Base-0.0.20/decore_base/library/roaster/roaster_server.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 07:17:23.288149 decore_Base-0.0.20/decore_base/prepare/
--rw-r--r--   0 runner    (1001) docker     (123)     2034 2023-06-16 07:17:11.000000 decore_Base-0.0.20/decore_base/prepare/.gitignore
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 07:17:23.288149 decore_Base-0.0.20/decore_base/prepare/.vscode/
--rw-r--r--   0 runner    (1001) docker     (123)      557 2023-06-16 07:17:11.000000 decore_Base-0.0.20/decore_base/prepare/.vscode/launch.json
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 07:17:23.280149 decore_Base-0.0.20/decore_base/prepare/spa/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 07:17:23.288149 decore_Base-0.0.20/decore_base/prepare/spa/static/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 07:17:23.288149 decore_Base-0.0.20/decore_base/prepare/spa/static/css/
--rw-r--r--   0 runner    (1001) docker     (123)      685 2023-06-16 07:17:11.000000 decore_Base-0.0.20/decore_base/prepare/spa/static/css/586.ed179a62.css
--rw-r--r--   0 runner    (1001) docker     (123)      746 2023-06-16 07:17:11.000000 decore_Base-0.0.20/decore_base/prepare/spa/static/css/app.d398f07d.css
--rw-r--r--   0 runner    (1001) docker     (123)   466611 2023-06-16 07:17:11.000000 decore_Base-0.0.20/decore_base/prepare/spa/static/css/vendor.14c9ac7a.css
--rw-r--r--   0 runner    (1001) docker     (123)    15086 2023-06-16 07:17:11.000000 decore_Base-0.0.20/decore_base/prepare/spa/static/favicon.ico
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 07:17:23.292149 decore_Base-0.0.20/decore_base/prepare/spa/static/fonts/
--rw-r--r--   0 runner    (1001) docker     (123)    20436 2023-06-16 07:17:11.000000 decore_Base-0.0.20/decore_base/prepare/spa/static/fonts/KFOkCnqEu92Fr1MmgVxIIzQ.68bb21d0.woff
--rw-r--r--   0 runner    (1001) docker     (123)    20544 2023-06-16 07:17:11.000000 decore_Base-0.0.20/decore_base/prepare/spa/static/fonts/KFOlCnqEu92Fr1MmEU9fBBc-.48af7707.woff
--rw-r--r--   0 runner    (1001) docker     (123)    20416 2023-06-16 07:17:11.000000 decore_Base-0.0.20/decore_base/prepare/spa/static/fonts/KFOlCnqEu92Fr1MmSU5fBBc-.c2f7ab22.woff
--rw-r--r--   0 runner    (1001) docker     (123)    20408 2023-06-16 07:17:11.000000 decore_Base-0.0.20/decore_base/prepare/spa/static/fonts/KFOlCnqEu92Fr1MmWUlfBBc-.77ecb942.woff
--rw-r--r--   0 runner    (1001) docker     (123)    20424 2023-06-16 07:17:11.000000 decore_Base-0.0.20/decore_base/prepare/spa/static/fonts/KFOlCnqEu92Fr1MmYUtfBBc-.f5677eb2.woff
--rw-r--r--   0 runner    (1001) docker     (123)    20344 2023-06-16 07:17:11.000000 decore_Base-0.0.20/decore_base/prepare/spa/static/fonts/KFOmCnqEu92Fr1Mu4mxM.f1e2a767.woff
--rw-r--r--   0 runner    (1001) docker     (123)   164912 2023-06-16 07:17:11.000000 decore_Base-0.0.20/decore_base/prepare/spa/static/fonts/flUhRq6tzZclQEJ-Vdg-IuiaDsNa.4d73cb90.woff
--rw-r--r--   0 runner    (1001) docker     (123)   128360 2023-06-16 07:17:11.000000 decore_Base-0.0.20/decore_base/prepare/spa/static/fonts/flUhRq6tzZclQEJ-Vdg-IuiaDsNcIhQ8tQ.0383092b.woff2
--rw-r--r--   0 runner    (1001) docker     (123)   465188 2023-06-16 07:17:11.000000 decore_Base-0.0.20/decore_base/prepare/spa/static/fonts/materialdesignicons-webfont.d8e8e0f7.woff
--rw-r--r--   0 runner    (1001) docker     (123)   325244 2023-06-16 07:17:11.000000 decore_Base-0.0.20/decore_base/prepare/spa/static/fonts/materialdesignicons-webfont.e9db4005.woff2
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 07:17:23.292149 decore_Base-0.0.20/decore_base/prepare/spa/static/icons/
--rw-r--r--   0 runner    (1001) docker     (123)     8505 2023-06-16 07:17:11.000000 decore_Base-0.0.20/decore_base/prepare/spa/static/icons/favicon-128x128.png
--rw-r--r--   0 runner    (1001) docker     (123)      952 2023-06-16 07:17:11.000000 decore_Base-0.0.20/decore_base/prepare/spa/static/icons/favicon-16x16.png
--rw-r--r--   0 runner    (1001) docker     (123)     1601 2023-06-16 07:17:11.000000 decore_Base-0.0.20/decore_base/prepare/spa/static/icons/favicon-32x32.png
--rw-r--r--   0 runner    (1001) docker     (123)     6264 2023-06-16 07:17:11.000000 decore_Base-0.0.20/decore_base/prepare/spa/static/icons/favicon-96x96.png
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 07:17:23.296149 decore_Base-0.0.20/decore_base/prepare/spa/static/js/
--rw-r--r--   0 runner    (1001) docker     (123)    32954 2023-06-16 07:17:11.000000 decore_Base-0.0.20/decore_base/prepare/spa/static/js/586.aa14c175.js
--rw-r--r--   0 runner    (1001) docker     (123)      778 2023-06-16 07:17:11.000000 decore_Base-0.0.20/decore_base/prepare/spa/static/js/65.940d9b80.js
--rw-r--r--   0 runner    (1001) docker     (123)    18041 2023-06-16 07:17:11.000000 decore_Base-0.0.20/decore_base/prepare/spa/static/js/app.af6cbe84.js
--rw-r--r--   0 runner    (1001) docker     (123)   376226 2023-06-16 07:17:11.000000 decore_Base-0.0.20/decore_base/prepare/spa/static/js/vendor.0902ddb5.js
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 07:17:23.296149 decore_Base-0.0.20/decore_base/prepare/spa/templates/
--rw-r--r--   0 runner    (1001) docker     (123)     1055 2023-06-16 07:17:11.000000 decore_Base-0.0.20/decore_base/prepare/spa/templates/index.html
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 07:17:23.296149 decore_Base-0.0.20/decore_base/sample/
--rw-r--r--   0 runner    (1001) docker     (123)     2034 2023-06-16 07:17:11.000000 decore_Base-0.0.20/decore_base/sample/.gitignore
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 07:17:23.296149 decore_Base-0.0.20/decore_base/sample/.vscode/
--rw-r--r--   0 runner    (1001) docker     (123)      557 2023-06-16 07:17:11.000000 decore_Base-0.0.20/decore_base/sample/.vscode/launch.json
--rw-r--r--   0 runner    (1001) docker     (123)      125 2023-06-16 07:17:11.000000 decore_Base-0.0.20/decore_base/sample/.vscode/settings.json
--rw-r--r--   0 runner    (1001) docker     (123)      239 2023-06-16 07:17:11.000000 decore_Base-0.0.20/decore_base/sample/app.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 07:17:23.296149 decore_Base-0.0.20/decore_base/sample/bases/
--rw-r--r--   0 runner    (1001) docker     (123)      267 2023-06-16 07:17:11.000000 decore_Base-0.0.20/decore_base/sample/bases/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      563 2023-06-16 07:17:11.000000 decore_Base-0.0.20/decore_base/sample/bases/account_base.py
--rw-r--r--   0 runner    (1001) docker     (123)      620 2023-06-16 07:17:11.000000 decore_Base-0.0.20/decore_base/sample/bases/company_base.py
--rw-r--r--   0 runner    (1001) docker     (123)     2626 2023-06-16 07:17:11.000000 decore_Base-0.0.20/decore_base/sample/bases/global_management_base.py
--rw-r--r--   0 runner    (1001) docker     (123)      148 2023-06-16 07:17:11.000000 decore_Base-0.0.20/decore_base/sample/bases/information_stytem_base.py
--rw-r--r--   0 runner    (1001) docker     (123)     2493 2023-06-16 07:17:11.000000 decore_Base-0.0.20/decore_base/sample/bases/person_base.py
--rw-r--r--   0 runner    (1001) docker     (123)      889 2023-06-16 07:17:11.000000 decore_Base-0.0.20/decore_base/sample/bases/test_base.py
--rw-r--r--   0 runner    (1001) docker     (123)      226 2023-06-16 07:17:11.000000 decore_Base-0.0.20/decore_base/sample/config.json
--rw-r--r--   0 runner    (1001) docker     (123)      334 2023-06-16 07:17:11.000000 decore_Base-0.0.20/decore_base/sample/language.json
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 07:17:23.296149 decore_Base-0.0.20/decore_base/sample/models/
--rw-r--r--   0 runner    (1001) docker     (123)      293 2023-06-16 07:17:11.000000 decore_Base-0.0.20/decore_base/sample/models/account_model.py
--rw-r--r--   0 runner    (1001) docker     (123)      263 2023-06-16 07:17:11.000000 decore_Base-0.0.20/decore_base/sample/models/company_model.py
--rw-r--r--   0 runner    (1001) docker     (123)      783 2023-06-16 07:17:11.000000 decore_Base-0.0.20/decore_base/sample/models/person_model.py
--rw-r--r--   0 runner    (1001) docker     (123)     1084 2023-06-16 07:17:11.000000 decore_Base-0.0.20/decore_base/sample/models/test_model.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 07:17:23.284149 decore_Base-0.0.20/decore_base/sample/spa/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 07:17:23.296149 decore_Base-0.0.20/decore_base/sample/spa/static/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 07:17:23.296149 decore_Base-0.0.20/decore_base/sample/spa/static/css/
--rw-r--r--   0 runner    (1001) docker     (123)      685 2023-06-16 07:17:11.000000 decore_Base-0.0.20/decore_base/sample/spa/static/css/586.ed179a62.css
--rw-r--r--   0 runner    (1001) docker     (123)      746 2023-06-16 07:17:11.000000 decore_Base-0.0.20/decore_base/sample/spa/static/css/app.d398f07d.css
--rw-r--r--   0 runner    (1001) docker     (123)   466611 2023-06-16 07:17:11.000000 decore_Base-0.0.20/decore_base/sample/spa/static/css/vendor.14c9ac7a.css
--rw-r--r--   0 runner    (1001) docker     (123)    15086 2023-06-16 07:17:11.000000 decore_Base-0.0.20/decore_base/sample/spa/static/favicon.ico
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 07:17:23.300149 decore_Base-0.0.20/decore_base/sample/spa/static/fonts/
--rw-r--r--   0 runner    (1001) docker     (123)    20436 2023-06-16 07:17:11.000000 decore_Base-0.0.20/decore_base/sample/spa/static/fonts/KFOkCnqEu92Fr1MmgVxIIzQ.68bb21d0.woff
--rw-r--r--   0 runner    (1001) docker     (123)    20544 2023-06-16 07:17:11.000000 decore_Base-0.0.20/decore_base/sample/spa/static/fonts/KFOlCnqEu92Fr1MmEU9fBBc-.48af7707.woff
--rw-r--r--   0 runner    (1001) docker     (123)    20416 2023-06-16 07:17:11.000000 decore_Base-0.0.20/decore_base/sample/spa/static/fonts/KFOlCnqEu92Fr1MmSU5fBBc-.c2f7ab22.woff
--rw-r--r--   0 runner    (1001) docker     (123)    20408 2023-06-16 07:17:11.000000 decore_Base-0.0.20/decore_base/sample/spa/static/fonts/KFOlCnqEu92Fr1MmWUlfBBc-.77ecb942.woff
--rw-r--r--   0 runner    (1001) docker     (123)    20424 2023-06-16 07:17:11.000000 decore_Base-0.0.20/decore_base/sample/spa/static/fonts/KFOlCnqEu92Fr1MmYUtfBBc-.f5677eb2.woff
--rw-r--r--   0 runner    (1001) docker     (123)    20344 2023-06-16 07:17:11.000000 decore_Base-0.0.20/decore_base/sample/spa/static/fonts/KFOmCnqEu92Fr1Mu4mxM.f1e2a767.woff
--rw-r--r--   0 runner    (1001) docker     (123)   164912 2023-06-16 07:17:11.000000 decore_Base-0.0.20/decore_base/sample/spa/static/fonts/flUhRq6tzZclQEJ-Vdg-IuiaDsNa.4d73cb90.woff
--rw-r--r--   0 runner    (1001) docker     (123)   128360 2023-06-16 07:17:11.000000 decore_Base-0.0.20/decore_base/sample/spa/static/fonts/flUhRq6tzZclQEJ-Vdg-IuiaDsNcIhQ8tQ.0383092b.woff2
--rw-r--r--   0 runner    (1001) docker     (123)   465188 2023-06-16 07:17:11.000000 decore_Base-0.0.20/decore_base/sample/spa/static/fonts/materialdesignicons-webfont.d8e8e0f7.woff
--rw-r--r--   0 runner    (1001) docker     (123)   325244 2023-06-16 07:17:11.000000 decore_Base-0.0.20/decore_base/sample/spa/static/fonts/materialdesignicons-webfont.e9db4005.woff2
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 07:17:23.300149 decore_Base-0.0.20/decore_base/sample/spa/static/icons/
--rw-r--r--   0 runner    (1001) docker     (123)     8505 2023-06-16 07:17:11.000000 decore_Base-0.0.20/decore_base/sample/spa/static/icons/favicon-128x128.png
--rw-r--r--   0 runner    (1001) docker     (123)      952 2023-06-16 07:17:11.000000 decore_Base-0.0.20/decore_base/sample/spa/static/icons/favicon-16x16.png
--rw-r--r--   0 runner    (1001) docker     (123)     1601 2023-06-16 07:17:11.000000 decore_Base-0.0.20/decore_base/sample/spa/static/icons/favicon-32x32.png
--rw-r--r--   0 runner    (1001) docker     (123)     6264 2023-06-16 07:17:11.000000 decore_Base-0.0.20/decore_base/sample/spa/static/icons/favicon-96x96.png
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 07:17:23.300149 decore_Base-0.0.20/decore_base/sample/spa/static/js/
--rw-r--r--   0 runner    (1001) docker     (123)    32954 2023-06-16 07:17:11.000000 decore_Base-0.0.20/decore_base/sample/spa/static/js/586.aa14c175.js
--rw-r--r--   0 runner    (1001) docker     (123)      778 2023-06-16 07:17:11.000000 decore_Base-0.0.20/decore_base/sample/spa/static/js/65.940d9b80.js
--rw-r--r--   0 runner    (1001) docker     (123)    18041 2023-06-16 07:17:11.000000 decore_Base-0.0.20/decore_base/sample/spa/static/js/app.af6cbe84.js
--rw-r--r--   0 runner    (1001) docker     (123)   376226 2023-06-16 07:17:11.000000 decore_Base-0.0.20/decore_base/sample/spa/static/js/vendor.0902ddb5.js
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 07:17:23.300149 decore_Base-0.0.20/decore_base/sample/spa/templates/
--rw-r--r--   0 runner    (1001) docker     (123)     1055 2023-06-16 07:17:11.000000 decore_Base-0.0.20/decore_base/sample/spa/templates/index.html
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 07:17:23.304149 decore_Base-0.0.20/decore_base/sample/state/
--rw-r--r--   0 runner    (1001) docker     (123)  1363968 2023-06-16 07:17:11.000000 decore_Base-0.0.20/decore_base/sample/state/database.db
--rw-r--r--   0 runner    (1001) docker     (123)     1477 2023-06-16 07:17:11.000000 decore_Base-0.0.20/decore_base/sample/state/keybase.kdbx
--rw-r--r--   0 runner    (1001) docker     (123)    16384 2023-06-16 07:17:11.000000 decore_Base-0.0.20/decore_base/sample/state/querybase.db
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 07:17:23.304149 decore_Base-0.0.20/decore_base/uniform/
--rw-r--r--   0 runner    (1001) docker     (123)       28 2023-06-16 07:17:11.000000 decore_Base-0.0.20/decore_base/uniform/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      662 2023-06-16 07:17:11.000000 decore_Base-0.0.20/decore_base/uniform/conform_model.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 07:17:23.304149 decore_Base-0.0.20/decore_base/uniform/depricated/
--rw-r--r--   0 runner    (1001) docker     (123)     8692 2023-06-16 07:17:11.000000 decore_Base-0.0.20/decore_base/uniform/depricated/askform_base.py
--rw-r--r--   0 runner    (1001) docker     (123)     4515 2023-06-16 07:17:11.000000 decore_Base-0.0.20/decore_base/uniform/depricated/buyform_base.py
--rw-r--r--   0 runner    (1001) docker     (123)     7613 2023-06-16 07:17:11.000000 decore_Base-0.0.20/decore_base/uniform/depricated/conform_base.py
--rw-r--r--   0 runner    (1001) docker     (123)     1756 2023-06-16 07:17:11.000000 decore_Base-0.0.20/decore_base/uniform/depricated/deform_base.py
--rw-r--r--   0 runner    (1001) docker     (123)     2579 2023-06-16 07:17:11.000000 decore_Base-0.0.20/decore_base/uniform/perform_model.py
--rw-r--r--   0 runner    (1001) docker     (123)     2106 2023-06-16 07:17:11.000000 decore_Base-0.0.20/decore_base/uniform/reform_client_model.py
--rw-r--r--   0 runner    (1001) docker     (123)     1481 2023-06-16 07:17:11.000000 decore_Base-0.0.20/decore_base/uniform/reform_server_model.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 07:17:23.308149 decore_Base-0.0.20/docs/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-16 07:17:11.000000 decore_Base-0.0.20/docs/.nojekyll
--rw-r--r--   0 runner    (1001) docker     (123)       14 2023-06-16 07:17:11.000000 decore_Base-0.0.20/docs/CNAME
--rw-r--r--   0 runner    (1001) docker     (123)      634 2023-06-16 07:17:11.000000 decore_Base-0.0.20/docs/Makefile
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 07:17:23.308149 decore_Base-0.0.20/docs/_static/
--rw-r--r--   0 runner    (1001) docker     (123)    15086 2023-06-16 07:17:11.000000 decore_Base-0.0.20/docs/_static/favicon.ico
--rw-r--r--   0 runner    (1001) docker     (123)    21966 2023-06-16 07:17:11.000000 decore_Base-0.0.20/docs/_static/logo.png
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 07:17:23.308149 decore_Base-0.0.20/docs/_static/styles/
--rw-r--r--   0 runner    (1001) docker     (123)       50 2023-06-16 07:17:11.000000 decore_Base-0.0.20/docs/_static/styles/custom.css
--rw-r--r--   0 runner    (1001) docker     (123)     1507 2023-06-16 07:17:11.000000 decore_Base-0.0.20/docs/conf.py
--rw-r--r--   0 runner    (1001) docker     (123)      226 2023-06-16 07:17:11.000000 decore_Base-0.0.20/docs/config.json
--rw-r--r--   0 runner    (1001) docker     (123)       89 2023-06-16 07:17:11.000000 decore_Base-0.0.20/docs/decore.rst
--rw-r--r--   0 runner    (1001) docker     (123)       69 2023-06-16 07:17:11.000000 decore_Base-0.0.20/docs/index.html
--rw-r--r--   0 runner    (1001) docker     (123)      414 2023-06-16 07:17:11.000000 decore_Base-0.0.20/docs/index.rst
--rw-r--r--   0 runner    (1001) docker     (123)      334 2023-06-16 07:17:11.000000 decore_Base-0.0.20/docs/language.json
--rw-r--r--   0 runner    (1001) docker     (123)      763 2023-06-16 07:17:11.000000 decore_Base-0.0.20/docs/make.bat
--rw-r--r--   0 runner    (1001) docker     (123)       94 2023-06-16 07:17:11.000000 decore_Base-0.0.20/docs/model.rst
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 07:17:23.284149 decore_Base-0.0.20/docs/page/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 07:17:23.308149 decore_Base-0.0.20/docs/page/doctrees/
--rw-r--r--   0 runner    (1001) docker     (123)     2797 2023-06-16 07:17:11.000000 decore_Base-0.0.20/docs/page/doctrees/decore.doctree
--rw-r--r--   0 runner    (1001) docker     (123)    81813 2023-06-16 07:17:11.000000 decore_Base-0.0.20/docs/page/doctrees/environment.pickle
--rw-r--r--   0 runner    (1001) docker     (123)    42551 2023-06-16 07:17:11.000000 decore_Base-0.0.20/docs/page/doctrees/index.doctree
--rw-r--r--   0 runner    (1001) docker     (123)     2836 2023-06-16 07:17:11.000000 decore_Base-0.0.20/docs/page/doctrees/model.doctree
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 07:17:23.308149 decore_Base-0.0.20/docs/page/html/
--rw-r--r--   0 runner    (1001) docker     (123)      230 2023-06-16 07:17:11.000000 decore_Base-0.0.20/docs/page/html/.buildinfo
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 07:17:23.308149 decore_Base-0.0.20/docs/page/html/_sources/
--rw-r--r--   0 runner    (1001) docker     (123)       89 2023-06-16 07:17:11.000000 decore_Base-0.0.20/docs/page/html/_sources/decore.rst.txt
--rw-r--r--   0 runner    (1001) docker     (123)      414 2023-06-16 07:17:11.000000 decore_Base-0.0.20/docs/page/html/_sources/index.rst.txt
--rw-r--r--   0 runner    (1001) docker     (123)       94 2023-06-16 07:17:11.000000 decore_Base-0.0.20/docs/page/html/_sources/model.rst.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 07:17:23.312149 decore_Base-0.0.20/docs/page/html/_static/
--rw-r--r--   0 runner    (1001) docker     (123)    14813 2023-06-16 07:17:11.000000 decore_Base-0.0.20/docs/page/html/_static/basic.css
--rw-r--r--   0 runner    (1001) docker     (123)      313 2023-06-16 07:17:11.000000 decore_Base-0.0.20/docs/page/html/_static/check-solid.svg
--rw-r--r--   0 runner    (1001) docker     (123)     9031 2023-06-16 07:17:11.000000 decore_Base-0.0.20/docs/page/html/_static/clipboard.min.js
--rw-r--r--   0 runner    (1001) docker     (123)      411 2023-06-16 07:17:11.000000 decore_Base-0.0.20/docs/page/html/_static/copy-button.svg
--rw-r--r--   0 runner    (1001) docker     (123)     2060 2023-06-16 07:17:11.000000 decore_Base-0.0.20/docs/page/html/_static/copybutton.css
--rw-r--r--   0 runner    (1001) docker     (123)     8467 2023-06-16 07:17:11.000000 decore_Base-0.0.20/docs/page/html/_static/copybutton.js
--rw-r--r--   0 runner    (1001) docker     (123)     2698 2023-06-16 07:17:11.000000 decore_Base-0.0.20/docs/page/html/_static/copybutton_funcs.js
--rw-r--r--   0 runner    (1001) docker     (123)     4472 2023-06-16 07:17:11.000000 decore_Base-0.0.20/docs/page/html/_static/doctools.js
--rw-r--r--   0 runner    (1001) docker     (123)      420 2023-06-16 07:17:11.000000 decore_Base-0.0.20/docs/page/html/_static/documentation_options.js
--rw-r--r--   0 runner    (1001) docker     (123)    15086 2023-06-16 07:17:11.000000 decore_Base-0.0.20/docs/page/html/_static/favicon.ico
--rw-r--r--   0 runner    (1001) docker     (123)      286 2023-06-16 07:17:11.000000 decore_Base-0.0.20/docs/page/html/_static/file.png
--rw-r--r--   0 runner    (1001) docker     (123)     4758 2023-06-16 07:17:11.000000 decore_Base-0.0.20/docs/page/html/_static/language_data.js
--rw-r--r--   0 runner    (1001) docker     (123)    21966 2023-06-16 07:17:11.000000 decore_Base-0.0.20/docs/page/html/_static/logo.png
--rw-r--r--   0 runner    (1001) docker     (123)       90 2023-06-16 07:17:11.000000 decore_Base-0.0.20/docs/page/html/_static/minus.png
--rw-r--r--   0 runner    (1001) docker     (123)       90 2023-06-16 07:17:11.000000 decore_Base-0.0.20/docs/page/html/_static/plus.png
--rw-r--r--   0 runner    (1001) docker     (123)    12757 2023-06-16 07:17:11.000000 decore_Base-0.0.20/docs/page/html/_static/pygments.css
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 07:17:23.312149 decore_Base-0.0.20/docs/page/html/_static/scripts/
--rw-r--r--   0 runner    (1001) docker     (123)    80813 2023-06-16 07:17:11.000000 decore_Base-0.0.20/docs/page/html/_static/scripts/bootstrap.js
--rw-r--r--   0 runner    (1001) docker     (123)      237 2023-06-16 07:17:11.000000 decore_Base-0.0.20/docs/page/html/_static/scripts/bootstrap.js.LICENSE.txt
--rw-r--r--   0 runner    (1001) docker     (123)   335757 2023-06-16 07:17:11.000000 decore_Base-0.0.20/docs/page/html/_static/scripts/bootstrap.js.map
--rw-r--r--   0 runner    (1001) docker     (123)     4456 2023-06-16 07:17:11.000000 decore_Base-0.0.20/docs/page/html/_static/scripts/pydata-sphinx-theme.js
--rw-r--r--   0 runner    (1001) docker     (123)    19648 2023-06-16 07:17:11.000000 decore_Base-0.0.20/docs/page/html/_static/scripts/pydata-sphinx-theme.js.map
--rw-r--r--   0 runner    (1001) docker     (123)    18215 2023-06-16 07:17:11.000000 decore_Base-0.0.20/docs/page/html/_static/searchtools.js
--rw-r--r--   0 runner    (1001) docker     (123)     4712 2023-06-16 07:17:11.000000 decore_Base-0.0.20/docs/page/html/_static/sphinx_highlight.js
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 07:17:23.312149 decore_Base-0.0.20/docs/page/html/_static/styles/
--rw-r--r--   0 runner    (1001) docker     (123)   176654 2023-06-16 07:17:11.000000 decore_Base-0.0.20/docs/page/html/_static/styles/bootstrap.css
--rw-r--r--   0 runner    (1001) docker     (123)       50 2023-06-16 07:17:11.000000 decore_Base-0.0.20/docs/page/html/_static/styles/custom.css
--rw-r--r--   0 runner    (1001) docker     (123)    63341 2023-06-16 07:17:11.000000 decore_Base-0.0.20/docs/page/html/_static/styles/pydata-sphinx-theme.css
--rw-r--r--   0 runner    (1001) docker     (123)      106 2023-06-16 07:17:11.000000 decore_Base-0.0.20/docs/page/html/_static/styles/theme.css
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 07:17:23.284149 decore_Base-0.0.20/docs/page/html/_static/vendor/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 07:17:23.284149 decore_Base-0.0.20/docs/page/html/_static/vendor/fontawesome/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 07:17:23.312149 decore_Base-0.0.20/docs/page/html/_static/vendor/fontawesome/6.1.2/
--rw-r--r--   0 runner    (1001) docker     (123)     7427 2023-06-16 07:17:11.000000 decore_Base-0.0.20/docs/page/html/_static/vendor/fontawesome/6.1.2/LICENSE.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 07:17:23.312149 decore_Base-0.0.20/docs/page/html/_static/vendor/fontawesome/6.1.2/css/
--rw-r--r--   0 runner    (1001) docker     (123)   101691 2023-06-16 07:17:11.000000 decore_Base-0.0.20/docs/page/html/_static/vendor/fontawesome/6.1.2/css/all.min.css
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 07:17:23.316149 decore_Base-0.0.20/docs/page/html/_static/vendor/fontawesome/6.1.2/webfonts/
--rw-r--r--   0 runner    (1001) docker     (123)   181264 2023-06-16 07:17:11.000000 decore_Base-0.0.20/docs/page/html/_static/vendor/fontawesome/6.1.2/webfonts/fa-brands-400.ttf
--rw-r--r--   0 runner    (1001) docker     (123)   105112 2023-06-16 07:17:11.000000 decore_Base-0.0.20/docs/page/html/_static/vendor/fontawesome/6.1.2/webfonts/fa-brands-400.woff2
--rw-r--r--   0 runner    (1001) docker     (123)    60236 2023-06-16 07:17:11.000000 decore_Base-0.0.20/docs/page/html/_static/vendor/fontawesome/6.1.2/webfonts/fa-regular-400.ttf
--rw-r--r--   0 runner    (1001) docker     (123)    24028 2023-06-16 07:17:11.000000 decore_Base-0.0.20/docs/page/html/_static/vendor/fontawesome/6.1.2/webfonts/fa-regular-400.woff2
--rw-r--r--   0 runner    (1001) docker     (123)   389948 2023-06-16 07:17:11.000000 decore_Base-0.0.20/docs/page/html/_static/vendor/fontawesome/6.1.2/webfonts/fa-solid-900.ttf
--rw-r--r--   0 runner    (1001) docker     (123)   154840 2023-06-16 07:17:11.000000 decore_Base-0.0.20/docs/page/html/_static/vendor/fontawesome/6.1.2/webfonts/fa-solid-900.woff2
--rw-r--r--   0 runner    (1001) docker     (123)    10084 2023-06-16 07:17:11.000000 decore_Base-0.0.20/docs/page/html/_static/vendor/fontawesome/6.1.2/webfonts/fa-v4compatibility.ttf
--rw-r--r--   0 runner    (1001) docker     (123)     4776 2023-06-16 07:17:11.000000 decore_Base-0.0.20/docs/page/html/_static/vendor/fontawesome/6.1.2/webfonts/fa-v4compatibility.woff2
--rw-r--r--   0 runner    (1001) docker     (123)     1863 2023-06-16 07:17:11.000000 decore_Base-0.0.20/docs/page/html/_static/webpack-macros.html
--rw-r--r--   0 runner    (1001) docker     (123)    10984 2023-06-16 07:17:11.000000 decore_Base-0.0.20/docs/page/html/decore.html
--rw-r--r--   0 runner    (1001) docker     (123)    10630 2023-06-16 07:17:11.000000 decore_Base-0.0.20/docs/page/html/genindex.html
--rw-r--r--   0 runner    (1001) docker     (123)    42175 2023-06-16 07:17:11.000000 decore_Base-0.0.20/docs/page/html/index.html
--rw-r--r--   0 runner    (1001) docker     (123)    10994 2023-06-16 07:17:11.000000 decore_Base-0.0.20/docs/page/html/model.html
--rw-r--r--   0 runner    (1001) docker     (123)      319 2023-06-16 07:17:11.000000 decore_Base-0.0.20/docs/page/html/objects.inv
--rw-r--r--   0 runner    (1001) docker     (123)    10566 2023-06-16 07:17:11.000000 decore_Base-0.0.20/docs/page/html/py-modindex.html
--rw-r--r--   0 runner    (1001) docker     (123)    10622 2023-06-16 07:17:11.000000 decore_Base-0.0.20/docs/page/html/search.html
--rw-r--r--   0 runner    (1001) docker     (123)     5814 2023-06-16 07:17:11.000000 decore_Base-0.0.20/docs/page/html/searchindex.js
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 07:17:23.316149 decore_Base-0.0.20/docs/state/
--rw-r--r--   0 runner    (1001) docker     (123)     1269 2023-06-16 07:17:11.000000 decore_Base-0.0.20/docs/state/keybase.kdbx
--rw-r--r--   0 runner    (1001) docker     (123)    16384 2023-06-16 07:17:11.000000 decore_Base-0.0.20/docs/state/querybase.db
--rw-r--r--   0 runner    (1001) docker     (123)      138 2023-06-16 07:17:11.000000 decore_Base-0.0.20/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)     1174 2023-06-16 07:17:11.000000 decore_Base-0.0.20/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (123)     2053 2023-06-16 07:17:23.316149 decore_Base-0.0.20/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 09:46:56.134879 decore_Base-0.0.21/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 09:46:56.106879 decore_Base-0.0.21/.github/
+-rw-r--r--   0 runner    (1001) docker     (123)      776 2023-06-16 09:46:48.000000 decore_Base-0.0.21/.github/FUNDING.yml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 09:46:56.110879 decore_Base-0.0.21/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (123)      436 2023-06-16 09:46:48.000000 decore_Base-0.0.21/.github/workflows/publish.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     2032 2023-06-16 09:46:48.000000 decore_Base-0.0.21/.gitignore
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 09:46:56.110879 decore_Base-0.0.21/.vscode/
+-rw-r--r--   0 runner    (1001) docker     (123)     1244 2023-06-16 09:46:48.000000 decore_Base-0.0.21/.vscode/launch.json
+-rw-r--r--   0 runner    (1001) docker     (123)      281 2023-06-16 09:46:48.000000 decore_Base-0.0.21/.vscode/settings.json
+-rw-r--r--   0 runner    (1001) docker     (123)     1788 2023-06-16 09:46:48.000000 decore_Base-0.0.21/KOFI.md
+-rw-r--r--   0 runner    (1001) docker     (123)    35148 2023-06-16 09:46:48.000000 decore_Base-0.0.21/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)    12127 2023-06-16 09:46:56.134879 decore_Base-0.0.21/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    11391 2023-06-16 09:46:48.000000 decore_Base-0.0.21/README.rst
+-rw-r--r--   0 runner    (1001) docker     (123)    12373 2023-06-16 09:46:48.000000 decore_Base-0.0.21/README_DE.rst
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 09:46:56.110879 decore_Base-0.0.21/decore_Base.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    12127 2023-06-16 09:46:56.000000 decore_Base-0.0.21/decore_Base.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     8005 2023-06-16 09:46:56.000000 decore_Base-0.0.21/decore_Base.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-16 09:46:56.000000 decore_Base-0.0.21/decore_Base.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     1174 2023-06-16 09:46:56.000000 decore_Base-0.0.21/decore_Base.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       12 2023-06-16 09:46:56.000000 decore_Base-0.0.21/decore_Base.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 09:46:56.110879 decore_Base-0.0.21/decore_base/
+-rw-r--r--   0 runner    (1001) docker     (123)       55 2023-06-16 09:46:48.000000 decore_Base-0.0.21/decore_base/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 09:46:56.110879 decore_Base-0.0.21/decore_base/classes/
+-rw-r--r--   0 runner    (1001) docker     (123)      388 2023-06-16 09:46:48.000000 decore_Base-0.0.21/decore_base/classes/decore_action.py
+-rw-r--r--   0 runner    (1001) docker     (123)      319 2023-06-16 09:46:48.000000 decore_Base-0.0.21/decore_base/classes/decore_app.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1412 2023-06-16 09:46:48.000000 decore_Base-0.0.21/decore_base/classes/decore_base.py
+-rw-r--r--   0 runner    (1001) docker     (123)      433 2023-06-16 09:46:48.000000 decore_Base-0.0.21/decore_base/classes/decore_dialog.py
+-rw-r--r--   0 runner    (1001) docker     (123)      489 2023-06-16 09:46:48.000000 decore_Base-0.0.21/decore_base/classes/decore_element.py
+-rw-r--r--   0 runner    (1001) docker     (123)      339 2023-06-16 09:46:48.000000 decore_Base-0.0.21/decore_base/classes/decore_function.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1434 2023-06-16 09:46:48.000000 decore_Base-0.0.21/decore_base/classes/decore_list.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15687 2023-06-16 09:46:48.000000 decore_Base-0.0.21/decore_base/classes/decore_model.py
+-rw-r--r--   0 runner    (1001) docker     (123)      498 2023-06-16 09:46:48.000000 decore_Base-0.0.21/decore_base/classes/decore_object.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4896 2023-06-16 09:46:48.000000 decore_Base-0.0.21/decore_base/classes/decore_pool.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4033 2023-06-16 09:46:48.000000 decore_Base-0.0.21/decore_base/classes/decore_prompt.py
+-rw-r--r--   0 runner    (1001) docker     (123)      664 2023-06-16 09:46:48.000000 decore_Base-0.0.21/decore_base/classes/decore_query.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1022 2023-06-16 09:46:48.000000 decore_Base-0.0.21/decore_base/classes/decore_return.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1536 2023-06-16 09:46:48.000000 decore_Base-0.0.21/decore_base/classes/decore_translate.py
+-rw-r--r--   0 runner    (1001) docker     (123)      524 2023-06-16 09:46:48.000000 decore_Base-0.0.21/decore_base/classes/decore_view.py
+-rw-r--r--   0 runner    (1001) docker     (123)      439 2023-06-16 09:46:48.000000 decore_Base-0.0.21/decore_base/classes/decore_widget.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16832 2023-06-16 09:46:48.000000 decore_Base-0.0.21/decore_base/decore.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2231 2023-06-16 09:46:48.000000 decore_Base-0.0.21/decore_base/globals.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 09:46:56.110879 decore_Base-0.0.21/decore_base/library/
+-rw-r--r--   0 runner    (1001) docker     (123)      189 2023-06-16 09:46:48.000000 decore_Base-0.0.21/decore_base/library/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 09:46:56.110879 decore_Base-0.0.21/decore_base/library/particl_market/
+-rw-r--r--   0 runner    (1001) docker     (123)       42 2023-06-16 09:46:48.000000 decore_Base-0.0.21/decore_base/library/particl_market/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10733 2023-06-16 09:46:48.000000 decore_Base-0.0.21/decore_base/library/particl_market/particl_market.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3995 2023-06-16 09:46:48.000000 decore_Base-0.0.21/decore_base/library/powershell.py
+-rw-r--r--   0 runner    (1001) docker     (123)    90489 2023-06-16 09:46:48.000000 decore_Base-0.0.21/decore_base/library/powershell2.py
+-rw-r--r--   0 runner    (1001) docker     (123)      616 2023-06-16 09:46:48.000000 decore_Base-0.0.21/decore_base/library/return_value.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 09:46:56.110879 decore_Base-0.0.21/decore_base/library/roaster/
+-rw-r--r--   0 runner    (1001) docker     (123)       91 2023-06-16 09:46:48.000000 decore_Base-0.0.21/decore_base/library/roaster/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4122 2023-06-16 09:46:48.000000 decore_Base-0.0.21/decore_base/library/roaster/roaster_client.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12453 2023-06-16 09:46:48.000000 decore_Base-0.0.21/decore_base/library/roaster/roaster_functions.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2186 2023-06-16 09:46:48.000000 decore_Base-0.0.21/decore_base/library/roaster/roaster_server.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 09:46:56.110879 decore_Base-0.0.21/decore_base/prepare/
+-rw-r--r--   0 runner    (1001) docker     (123)     2034 2023-06-16 09:46:48.000000 decore_Base-0.0.21/decore_base/prepare/.gitignore
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 09:46:56.114879 decore_Base-0.0.21/decore_base/prepare/.vscode/
+-rw-r--r--   0 runner    (1001) docker     (123)      557 2023-06-16 09:46:48.000000 decore_Base-0.0.21/decore_base/prepare/.vscode/launch.json
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 09:46:56.106879 decore_Base-0.0.21/decore_base/prepare/spa/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 09:46:56.114879 decore_Base-0.0.21/decore_base/prepare/spa/static/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 09:46:56.114879 decore_Base-0.0.21/decore_base/prepare/spa/static/css/
+-rw-r--r--   0 runner    (1001) docker     (123)      685 2023-06-16 09:46:48.000000 decore_Base-0.0.21/decore_base/prepare/spa/static/css/586.ed179a62.css
+-rw-r--r--   0 runner    (1001) docker     (123)      746 2023-06-16 09:46:48.000000 decore_Base-0.0.21/decore_base/prepare/spa/static/css/app.d398f07d.css
+-rw-r--r--   0 runner    (1001) docker     (123)   466611 2023-06-16 09:46:48.000000 decore_Base-0.0.21/decore_base/prepare/spa/static/css/vendor.14c9ac7a.css
+-rw-r--r--   0 runner    (1001) docker     (123)    15086 2023-06-16 09:46:48.000000 decore_Base-0.0.21/decore_base/prepare/spa/static/favicon.ico
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 09:46:56.114879 decore_Base-0.0.21/decore_base/prepare/spa/static/fonts/
+-rw-r--r--   0 runner    (1001) docker     (123)    20436 2023-06-16 09:46:48.000000 decore_Base-0.0.21/decore_base/prepare/spa/static/fonts/KFOkCnqEu92Fr1MmgVxIIzQ.68bb21d0.woff
+-rw-r--r--   0 runner    (1001) docker     (123)    20544 2023-06-16 09:46:48.000000 decore_Base-0.0.21/decore_base/prepare/spa/static/fonts/KFOlCnqEu92Fr1MmEU9fBBc-.48af7707.woff
+-rw-r--r--   0 runner    (1001) docker     (123)    20416 2023-06-16 09:46:48.000000 decore_Base-0.0.21/decore_base/prepare/spa/static/fonts/KFOlCnqEu92Fr1MmSU5fBBc-.c2f7ab22.woff
+-rw-r--r--   0 runner    (1001) docker     (123)    20408 2023-06-16 09:46:48.000000 decore_Base-0.0.21/decore_base/prepare/spa/static/fonts/KFOlCnqEu92Fr1MmWUlfBBc-.77ecb942.woff
+-rw-r--r--   0 runner    (1001) docker     (123)    20424 2023-06-16 09:46:48.000000 decore_Base-0.0.21/decore_base/prepare/spa/static/fonts/KFOlCnqEu92Fr1MmYUtfBBc-.f5677eb2.woff
+-rw-r--r--   0 runner    (1001) docker     (123)    20344 2023-06-16 09:46:48.000000 decore_Base-0.0.21/decore_base/prepare/spa/static/fonts/KFOmCnqEu92Fr1Mu4mxM.f1e2a767.woff
+-rw-r--r--   0 runner    (1001) docker     (123)   164912 2023-06-16 09:46:48.000000 decore_Base-0.0.21/decore_base/prepare/spa/static/fonts/flUhRq6tzZclQEJ-Vdg-IuiaDsNa.4d73cb90.woff
+-rw-r--r--   0 runner    (1001) docker     (123)   128360 2023-06-16 09:46:48.000000 decore_Base-0.0.21/decore_base/prepare/spa/static/fonts/flUhRq6tzZclQEJ-Vdg-IuiaDsNcIhQ8tQ.0383092b.woff2
+-rw-r--r--   0 runner    (1001) docker     (123)   465188 2023-06-16 09:46:48.000000 decore_Base-0.0.21/decore_base/prepare/spa/static/fonts/materialdesignicons-webfont.d8e8e0f7.woff
+-rw-r--r--   0 runner    (1001) docker     (123)   325244 2023-06-16 09:46:48.000000 decore_Base-0.0.21/decore_base/prepare/spa/static/fonts/materialdesignicons-webfont.e9db4005.woff2
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 09:46:56.114879 decore_Base-0.0.21/decore_base/prepare/spa/static/icons/
+-rw-r--r--   0 runner    (1001) docker     (123)     8505 2023-06-16 09:46:48.000000 decore_Base-0.0.21/decore_base/prepare/spa/static/icons/favicon-128x128.png
+-rw-r--r--   0 runner    (1001) docker     (123)      952 2023-06-16 09:46:48.000000 decore_Base-0.0.21/decore_base/prepare/spa/static/icons/favicon-16x16.png
+-rw-r--r--   0 runner    (1001) docker     (123)     1601 2023-06-16 09:46:48.000000 decore_Base-0.0.21/decore_base/prepare/spa/static/icons/favicon-32x32.png
+-rw-r--r--   0 runner    (1001) docker     (123)     6264 2023-06-16 09:46:48.000000 decore_Base-0.0.21/decore_base/prepare/spa/static/icons/favicon-96x96.png
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 09:46:56.114879 decore_Base-0.0.21/decore_base/prepare/spa/static/js/
+-rw-r--r--   0 runner    (1001) docker     (123)    32954 2023-06-16 09:46:48.000000 decore_Base-0.0.21/decore_base/prepare/spa/static/js/586.aa14c175.js
+-rw-r--r--   0 runner    (1001) docker     (123)      778 2023-06-16 09:46:48.000000 decore_Base-0.0.21/decore_base/prepare/spa/static/js/65.940d9b80.js
+-rw-r--r--   0 runner    (1001) docker     (123)    18041 2023-06-16 09:46:48.000000 decore_Base-0.0.21/decore_base/prepare/spa/static/js/app.af6cbe84.js
+-rw-r--r--   0 runner    (1001) docker     (123)   376226 2023-06-16 09:46:48.000000 decore_Base-0.0.21/decore_base/prepare/spa/static/js/vendor.0902ddb5.js
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 09:46:56.118879 decore_Base-0.0.21/decore_base/prepare/spa/templates/
+-rw-r--r--   0 runner    (1001) docker     (123)     1055 2023-06-16 09:46:48.000000 decore_Base-0.0.21/decore_base/prepare/spa/templates/index.html
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 09:46:56.118879 decore_Base-0.0.21/decore_base/sample/
+-rw-r--r--   0 runner    (1001) docker     (123)     2034 2023-06-16 09:46:48.000000 decore_Base-0.0.21/decore_base/sample/.gitignore
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 09:46:56.118879 decore_Base-0.0.21/decore_base/sample/.vscode/
+-rw-r--r--   0 runner    (1001) docker     (123)      557 2023-06-16 09:46:48.000000 decore_Base-0.0.21/decore_base/sample/.vscode/launch.json
+-rw-r--r--   0 runner    (1001) docker     (123)      125 2023-06-16 09:46:48.000000 decore_Base-0.0.21/decore_base/sample/.vscode/settings.json
+-rw-r--r--   0 runner    (1001) docker     (123)      239 2023-06-16 09:46:48.000000 decore_Base-0.0.21/decore_base/sample/app.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 09:46:56.118879 decore_Base-0.0.21/decore_base/sample/bases/
+-rw-r--r--   0 runner    (1001) docker     (123)      267 2023-06-16 09:46:48.000000 decore_Base-0.0.21/decore_base/sample/bases/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      563 2023-06-16 09:46:48.000000 decore_Base-0.0.21/decore_base/sample/bases/account_base.py
+-rw-r--r--   0 runner    (1001) docker     (123)      620 2023-06-16 09:46:48.000000 decore_Base-0.0.21/decore_base/sample/bases/company_base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2626 2023-06-16 09:46:48.000000 decore_Base-0.0.21/decore_base/sample/bases/global_management_base.py
+-rw-r--r--   0 runner    (1001) docker     (123)      148 2023-06-16 09:46:48.000000 decore_Base-0.0.21/decore_base/sample/bases/information_stytem_base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2493 2023-06-16 09:46:48.000000 decore_Base-0.0.21/decore_base/sample/bases/person_base.py
+-rw-r--r--   0 runner    (1001) docker     (123)      889 2023-06-16 09:46:48.000000 decore_Base-0.0.21/decore_base/sample/bases/test_base.py
+-rw-r--r--   0 runner    (1001) docker     (123)      226 2023-06-16 09:46:48.000000 decore_Base-0.0.21/decore_base/sample/config.json
+-rw-r--r--   0 runner    (1001) docker     (123)      334 2023-06-16 09:46:48.000000 decore_Base-0.0.21/decore_base/sample/language.json
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 09:46:56.118879 decore_Base-0.0.21/decore_base/sample/models/
+-rw-r--r--   0 runner    (1001) docker     (123)      293 2023-06-16 09:46:48.000000 decore_Base-0.0.21/decore_base/sample/models/account_model.py
+-rw-r--r--   0 runner    (1001) docker     (123)      263 2023-06-16 09:46:48.000000 decore_Base-0.0.21/decore_base/sample/models/company_model.py
+-rw-r--r--   0 runner    (1001) docker     (123)      783 2023-06-16 09:46:48.000000 decore_Base-0.0.21/decore_base/sample/models/person_model.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1084 2023-06-16 09:46:48.000000 decore_Base-0.0.21/decore_base/sample/models/test_model.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 09:46:56.106879 decore_Base-0.0.21/decore_base/sample/spa/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 09:46:56.118879 decore_Base-0.0.21/decore_base/sample/spa/static/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 09:46:56.118879 decore_Base-0.0.21/decore_base/sample/spa/static/css/
+-rw-r--r--   0 runner    (1001) docker     (123)      685 2023-06-16 09:46:48.000000 decore_Base-0.0.21/decore_base/sample/spa/static/css/586.ed179a62.css
+-rw-r--r--   0 runner    (1001) docker     (123)      746 2023-06-16 09:46:48.000000 decore_Base-0.0.21/decore_base/sample/spa/static/css/app.d398f07d.css
+-rw-r--r--   0 runner    (1001) docker     (123)   466611 2023-06-16 09:46:48.000000 decore_Base-0.0.21/decore_base/sample/spa/static/css/vendor.14c9ac7a.css
+-rw-r--r--   0 runner    (1001) docker     (123)    15086 2023-06-16 09:46:48.000000 decore_Base-0.0.21/decore_base/sample/spa/static/favicon.ico
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 09:46:56.122879 decore_Base-0.0.21/decore_base/sample/spa/static/fonts/
+-rw-r--r--   0 runner    (1001) docker     (123)    20436 2023-06-16 09:46:48.000000 decore_Base-0.0.21/decore_base/sample/spa/static/fonts/KFOkCnqEu92Fr1MmgVxIIzQ.68bb21d0.woff
+-rw-r--r--   0 runner    (1001) docker     (123)    20544 2023-06-16 09:46:48.000000 decore_Base-0.0.21/decore_base/sample/spa/static/fonts/KFOlCnqEu92Fr1MmEU9fBBc-.48af7707.woff
+-rw-r--r--   0 runner    (1001) docker     (123)    20416 2023-06-16 09:46:48.000000 decore_Base-0.0.21/decore_base/sample/spa/static/fonts/KFOlCnqEu92Fr1MmSU5fBBc-.c2f7ab22.woff
+-rw-r--r--   0 runner    (1001) docker     (123)    20408 2023-06-16 09:46:48.000000 decore_Base-0.0.21/decore_base/sample/spa/static/fonts/KFOlCnqEu92Fr1MmWUlfBBc-.77ecb942.woff
+-rw-r--r--   0 runner    (1001) docker     (123)    20424 2023-06-16 09:46:48.000000 decore_Base-0.0.21/decore_base/sample/spa/static/fonts/KFOlCnqEu92Fr1MmYUtfBBc-.f5677eb2.woff
+-rw-r--r--   0 runner    (1001) docker     (123)    20344 2023-06-16 09:46:48.000000 decore_Base-0.0.21/decore_base/sample/spa/static/fonts/KFOmCnqEu92Fr1Mu4mxM.f1e2a767.woff
+-rw-r--r--   0 runner    (1001) docker     (123)   164912 2023-06-16 09:46:48.000000 decore_Base-0.0.21/decore_base/sample/spa/static/fonts/flUhRq6tzZclQEJ-Vdg-IuiaDsNa.4d73cb90.woff
+-rw-r--r--   0 runner    (1001) docker     (123)   128360 2023-06-16 09:46:48.000000 decore_Base-0.0.21/decore_base/sample/spa/static/fonts/flUhRq6tzZclQEJ-Vdg-IuiaDsNcIhQ8tQ.0383092b.woff2
+-rw-r--r--   0 runner    (1001) docker     (123)   465188 2023-06-16 09:46:48.000000 decore_Base-0.0.21/decore_base/sample/spa/static/fonts/materialdesignicons-webfont.d8e8e0f7.woff
+-rw-r--r--   0 runner    (1001) docker     (123)   325244 2023-06-16 09:46:48.000000 decore_Base-0.0.21/decore_base/sample/spa/static/fonts/materialdesignicons-webfont.e9db4005.woff2
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 09:46:56.122879 decore_Base-0.0.21/decore_base/sample/spa/static/icons/
+-rw-r--r--   0 runner    (1001) docker     (123)     8505 2023-06-16 09:46:48.000000 decore_Base-0.0.21/decore_base/sample/spa/static/icons/favicon-128x128.png
+-rw-r--r--   0 runner    (1001) docker     (123)      952 2023-06-16 09:46:48.000000 decore_Base-0.0.21/decore_base/sample/spa/static/icons/favicon-16x16.png
+-rw-r--r--   0 runner    (1001) docker     (123)     1601 2023-06-16 09:46:48.000000 decore_Base-0.0.21/decore_base/sample/spa/static/icons/favicon-32x32.png
+-rw-r--r--   0 runner    (1001) docker     (123)     6264 2023-06-16 09:46:48.000000 decore_Base-0.0.21/decore_base/sample/spa/static/icons/favicon-96x96.png
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 09:46:56.122879 decore_Base-0.0.21/decore_base/sample/spa/static/js/
+-rw-r--r--   0 runner    (1001) docker     (123)    32954 2023-06-16 09:46:48.000000 decore_Base-0.0.21/decore_base/sample/spa/static/js/586.aa14c175.js
+-rw-r--r--   0 runner    (1001) docker     (123)      778 2023-06-16 09:46:48.000000 decore_Base-0.0.21/decore_base/sample/spa/static/js/65.940d9b80.js
+-rw-r--r--   0 runner    (1001) docker     (123)    18041 2023-06-16 09:46:48.000000 decore_Base-0.0.21/decore_base/sample/spa/static/js/app.af6cbe84.js
+-rw-r--r--   0 runner    (1001) docker     (123)   376226 2023-06-16 09:46:48.000000 decore_Base-0.0.21/decore_base/sample/spa/static/js/vendor.0902ddb5.js
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 09:46:56.122879 decore_Base-0.0.21/decore_base/sample/spa/templates/
+-rw-r--r--   0 runner    (1001) docker     (123)     1055 2023-06-16 09:46:48.000000 decore_Base-0.0.21/decore_base/sample/spa/templates/index.html
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 09:46:56.126879 decore_Base-0.0.21/decore_base/sample/state/
+-rw-r--r--   0 runner    (1001) docker     (123)  1363968 2023-06-16 09:46:48.000000 decore_Base-0.0.21/decore_base/sample/state/database.db
+-rw-r--r--   0 runner    (1001) docker     (123)     1477 2023-06-16 09:46:48.000000 decore_Base-0.0.21/decore_base/sample/state/keybase.kdbx
+-rw-r--r--   0 runner    (1001) docker     (123)    16384 2023-06-16 09:46:48.000000 decore_Base-0.0.21/decore_base/sample/state/querybase.db
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 09:46:56.126879 decore_Base-0.0.21/decore_base/uniform/
+-rw-r--r--   0 runner    (1001) docker     (123)       28 2023-06-16 09:46:48.000000 decore_Base-0.0.21/decore_base/uniform/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      662 2023-06-16 09:46:48.000000 decore_Base-0.0.21/decore_base/uniform/conform_model.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 09:46:56.126879 decore_Base-0.0.21/decore_base/uniform/depricated/
+-rw-r--r--   0 runner    (1001) docker     (123)     8692 2023-06-16 09:46:48.000000 decore_Base-0.0.21/decore_base/uniform/depricated/askform_base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4515 2023-06-16 09:46:48.000000 decore_Base-0.0.21/decore_base/uniform/depricated/buyform_base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7613 2023-06-16 09:46:48.000000 decore_Base-0.0.21/decore_base/uniform/depricated/conform_base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1756 2023-06-16 09:46:48.000000 decore_Base-0.0.21/decore_base/uniform/depricated/deform_base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2579 2023-06-16 09:46:48.000000 decore_Base-0.0.21/decore_base/uniform/perform_model.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2106 2023-06-16 09:46:48.000000 decore_Base-0.0.21/decore_base/uniform/reform_client_model.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1481 2023-06-16 09:46:48.000000 decore_Base-0.0.21/decore_base/uniform/reform_server_model.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 09:46:56.126879 decore_Base-0.0.21/docs/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-16 09:46:48.000000 decore_Base-0.0.21/docs/.nojekyll
+-rw-r--r--   0 runner    (1001) docker     (123)       14 2023-06-16 09:46:48.000000 decore_Base-0.0.21/docs/CNAME
+-rw-r--r--   0 runner    (1001) docker     (123)      634 2023-06-16 09:46:48.000000 decore_Base-0.0.21/docs/Makefile
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 09:46:56.126879 decore_Base-0.0.21/docs/_static/
+-rw-r--r--   0 runner    (1001) docker     (123)    15086 2023-06-16 09:46:48.000000 decore_Base-0.0.21/docs/_static/favicon.ico
+-rw-r--r--   0 runner    (1001) docker     (123)    21966 2023-06-16 09:46:48.000000 decore_Base-0.0.21/docs/_static/logo.png
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 09:46:56.126879 decore_Base-0.0.21/docs/_static/styles/
+-rw-r--r--   0 runner    (1001) docker     (123)       50 2023-06-16 09:46:48.000000 decore_Base-0.0.21/docs/_static/styles/custom.css
+-rw-r--r--   0 runner    (1001) docker     (123)     1507 2023-06-16 09:46:48.000000 decore_Base-0.0.21/docs/conf.py
+-rw-r--r--   0 runner    (1001) docker     (123)      226 2023-06-16 09:46:48.000000 decore_Base-0.0.21/docs/config.json
+-rw-r--r--   0 runner    (1001) docker     (123)       89 2023-06-16 09:46:48.000000 decore_Base-0.0.21/docs/decore.rst.out
+-rw-r--r--   0 runner    (1001) docker     (123)       69 2023-06-16 09:46:48.000000 decore_Base-0.0.21/docs/index.html
+-rw-r--r--   0 runner    (1001) docker     (123)      414 2023-06-16 09:46:48.000000 decore_Base-0.0.21/docs/index.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      334 2023-06-16 09:46:48.000000 decore_Base-0.0.21/docs/language.json
+-rw-r--r--   0 runner    (1001) docker     (123)      763 2023-06-16 09:46:48.000000 decore_Base-0.0.21/docs/make.bat
+-rw-r--r--   0 runner    (1001) docker     (123)       94 2023-06-16 09:46:48.000000 decore_Base-0.0.21/docs/model.rst.out
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 09:46:56.106879 decore_Base-0.0.21/docs/page/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 09:46:56.126879 decore_Base-0.0.21/docs/page/doctrees/
+-rw-r--r--   0 runner    (1001) docker     (123)    77099 2023-06-16 09:46:48.000000 decore_Base-0.0.21/docs/page/doctrees/environment.pickle
+-rw-r--r--   0 runner    (1001) docker     (123)    44359 2023-06-16 09:46:48.000000 decore_Base-0.0.21/docs/page/doctrees/index.doctree
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 09:46:56.126879 decore_Base-0.0.21/docs/page/html/
+-rw-r--r--   0 runner    (1001) docker     (123)      230 2023-06-16 09:46:48.000000 decore_Base-0.0.21/docs/page/html/.buildinfo
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 09:46:56.126879 decore_Base-0.0.21/docs/page/html/_sources/
+-rw-r--r--   0 runner    (1001) docker     (123)      414 2023-06-16 09:46:48.000000 decore_Base-0.0.21/docs/page/html/_sources/index.rst.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 09:46:56.130879 decore_Base-0.0.21/docs/page/html/_static/
+-rw-r--r--   0 runner    (1001) docker     (123)    14813 2023-06-16 09:46:48.000000 decore_Base-0.0.21/docs/page/html/_static/basic.css
+-rw-r--r--   0 runner    (1001) docker     (123)      313 2023-06-16 09:46:48.000000 decore_Base-0.0.21/docs/page/html/_static/check-solid.svg
+-rw-r--r--   0 runner    (1001) docker     (123)     9031 2023-06-16 09:46:48.000000 decore_Base-0.0.21/docs/page/html/_static/clipboard.min.js
+-rw-r--r--   0 runner    (1001) docker     (123)      411 2023-06-16 09:46:48.000000 decore_Base-0.0.21/docs/page/html/_static/copy-button.svg
+-rw-r--r--   0 runner    (1001) docker     (123)     2060 2023-06-16 09:46:48.000000 decore_Base-0.0.21/docs/page/html/_static/copybutton.css
+-rw-r--r--   0 runner    (1001) docker     (123)     8467 2023-06-16 09:46:48.000000 decore_Base-0.0.21/docs/page/html/_static/copybutton.js
+-rw-r--r--   0 runner    (1001) docker     (123)     2698 2023-06-16 09:46:48.000000 decore_Base-0.0.21/docs/page/html/_static/copybutton_funcs.js
+-rw-r--r--   0 runner    (1001) docker     (123)     4472 2023-06-16 09:46:48.000000 decore_Base-0.0.21/docs/page/html/_static/doctools.js
+-rw-r--r--   0 runner    (1001) docker     (123)      420 2023-06-16 09:46:48.000000 decore_Base-0.0.21/docs/page/html/_static/documentation_options.js
+-rw-r--r--   0 runner    (1001) docker     (123)    15086 2023-06-16 09:46:48.000000 decore_Base-0.0.21/docs/page/html/_static/favicon.ico
+-rw-r--r--   0 runner    (1001) docker     (123)      286 2023-06-16 09:46:48.000000 decore_Base-0.0.21/docs/page/html/_static/file.png
+-rw-r--r--   0 runner    (1001) docker     (123)     4758 2023-06-16 09:46:48.000000 decore_Base-0.0.21/docs/page/html/_static/language_data.js
+-rw-r--r--   0 runner    (1001) docker     (123)    21966 2023-06-16 09:46:48.000000 decore_Base-0.0.21/docs/page/html/_static/logo.png
+-rw-r--r--   0 runner    (1001) docker     (123)       90 2023-06-16 09:46:48.000000 decore_Base-0.0.21/docs/page/html/_static/minus.png
+-rw-r--r--   0 runner    (1001) docker     (123)       90 2023-06-16 09:46:48.000000 decore_Base-0.0.21/docs/page/html/_static/plus.png
+-rw-r--r--   0 runner    (1001) docker     (123)    12757 2023-06-16 09:46:48.000000 decore_Base-0.0.21/docs/page/html/_static/pygments.css
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 09:46:56.130879 decore_Base-0.0.21/docs/page/html/_static/scripts/
+-rw-r--r--   0 runner    (1001) docker     (123)    80813 2023-06-16 09:46:48.000000 decore_Base-0.0.21/docs/page/html/_static/scripts/bootstrap.js
+-rw-r--r--   0 runner    (1001) docker     (123)      237 2023-06-16 09:46:48.000000 decore_Base-0.0.21/docs/page/html/_static/scripts/bootstrap.js.LICENSE.txt
+-rw-r--r--   0 runner    (1001) docker     (123)   335757 2023-06-16 09:46:48.000000 decore_Base-0.0.21/docs/page/html/_static/scripts/bootstrap.js.map
+-rw-r--r--   0 runner    (1001) docker     (123)     4456 2023-06-16 09:46:48.000000 decore_Base-0.0.21/docs/page/html/_static/scripts/pydata-sphinx-theme.js
+-rw-r--r--   0 runner    (1001) docker     (123)    19648 2023-06-16 09:46:48.000000 decore_Base-0.0.21/docs/page/html/_static/scripts/pydata-sphinx-theme.js.map
+-rw-r--r--   0 runner    (1001) docker     (123)    18215 2023-06-16 09:46:48.000000 decore_Base-0.0.21/docs/page/html/_static/searchtools.js
+-rw-r--r--   0 runner    (1001) docker     (123)     4712 2023-06-16 09:46:48.000000 decore_Base-0.0.21/docs/page/html/_static/sphinx_highlight.js
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 09:46:56.130879 decore_Base-0.0.21/docs/page/html/_static/styles/
+-rw-r--r--   0 runner    (1001) docker     (123)   176654 2023-06-16 09:46:48.000000 decore_Base-0.0.21/docs/page/html/_static/styles/bootstrap.css
+-rw-r--r--   0 runner    (1001) docker     (123)       50 2023-06-16 09:46:48.000000 decore_Base-0.0.21/docs/page/html/_static/styles/custom.css
+-rw-r--r--   0 runner    (1001) docker     (123)    63341 2023-06-16 09:46:48.000000 decore_Base-0.0.21/docs/page/html/_static/styles/pydata-sphinx-theme.css
+-rw-r--r--   0 runner    (1001) docker     (123)      106 2023-06-16 09:46:48.000000 decore_Base-0.0.21/docs/page/html/_static/styles/theme.css
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 09:46:56.106879 decore_Base-0.0.21/docs/page/html/_static/vendor/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 09:46:56.106879 decore_Base-0.0.21/docs/page/html/_static/vendor/fontawesome/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 09:46:56.130879 decore_Base-0.0.21/docs/page/html/_static/vendor/fontawesome/6.1.2/
+-rw-r--r--   0 runner    (1001) docker     (123)     7427 2023-06-16 09:46:48.000000 decore_Base-0.0.21/docs/page/html/_static/vendor/fontawesome/6.1.2/LICENSE.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 09:46:56.130879 decore_Base-0.0.21/docs/page/html/_static/vendor/fontawesome/6.1.2/css/
+-rw-r--r--   0 runner    (1001) docker     (123)   101691 2023-06-16 09:46:48.000000 decore_Base-0.0.21/docs/page/html/_static/vendor/fontawesome/6.1.2/css/all.min.css
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 09:46:56.134879 decore_Base-0.0.21/docs/page/html/_static/vendor/fontawesome/6.1.2/webfonts/
+-rw-r--r--   0 runner    (1001) docker     (123)   181264 2023-06-16 09:46:48.000000 decore_Base-0.0.21/docs/page/html/_static/vendor/fontawesome/6.1.2/webfonts/fa-brands-400.ttf
+-rw-r--r--   0 runner    (1001) docker     (123)   105112 2023-06-16 09:46:48.000000 decore_Base-0.0.21/docs/page/html/_static/vendor/fontawesome/6.1.2/webfonts/fa-brands-400.woff2
+-rw-r--r--   0 runner    (1001) docker     (123)    60236 2023-06-16 09:46:48.000000 decore_Base-0.0.21/docs/page/html/_static/vendor/fontawesome/6.1.2/webfonts/fa-regular-400.ttf
+-rw-r--r--   0 runner    (1001) docker     (123)    24028 2023-06-16 09:46:48.000000 decore_Base-0.0.21/docs/page/html/_static/vendor/fontawesome/6.1.2/webfonts/fa-regular-400.woff2
+-rw-r--r--   0 runner    (1001) docker     (123)   389948 2023-06-16 09:46:48.000000 decore_Base-0.0.21/docs/page/html/_static/vendor/fontawesome/6.1.2/webfonts/fa-solid-900.ttf
+-rw-r--r--   0 runner    (1001) docker     (123)   154840 2023-06-16 09:46:48.000000 decore_Base-0.0.21/docs/page/html/_static/vendor/fontawesome/6.1.2/webfonts/fa-solid-900.woff2
+-rw-r--r--   0 runner    (1001) docker     (123)    10084 2023-06-16 09:46:48.000000 decore_Base-0.0.21/docs/page/html/_static/vendor/fontawesome/6.1.2/webfonts/fa-v4compatibility.ttf
+-rw-r--r--   0 runner    (1001) docker     (123)     4776 2023-06-16 09:46:48.000000 decore_Base-0.0.21/docs/page/html/_static/vendor/fontawesome/6.1.2/webfonts/fa-v4compatibility.woff2
+-rw-r--r--   0 runner    (1001) docker     (123)     1863 2023-06-16 09:46:48.000000 decore_Base-0.0.21/docs/page/html/_static/webpack-macros.html
+-rw-r--r--   0 runner    (1001) docker     (123)     9600 2023-06-16 09:46:48.000000 decore_Base-0.0.21/docs/page/html/genindex.html
+-rw-r--r--   0 runner    (1001) docker     (123)    42841 2023-06-16 09:46:48.000000 decore_Base-0.0.21/docs/page/html/index.html
+-rw-r--r--   0 runner    (1001) docker     (123)      243 2023-06-16 09:46:48.000000 decore_Base-0.0.21/docs/page/html/objects.inv
+-rw-r--r--   0 runner    (1001) docker     (123)    10622 2023-06-16 09:46:48.000000 decore_Base-0.0.21/docs/page/html/search.html
+-rw-r--r--   0 runner    (1001) docker     (123)     5265 2023-06-16 09:46:48.000000 decore_Base-0.0.21/docs/page/html/searchindex.js
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 09:46:56.134879 decore_Base-0.0.21/docs/state/
+-rw-r--r--   0 runner    (1001) docker     (123)     1269 2023-06-16 09:46:48.000000 decore_Base-0.0.21/docs/state/keybase.kdbx
+-rw-r--r--   0 runner    (1001) docker     (123)    16384 2023-06-16 09:46:48.000000 decore_Base-0.0.21/docs/state/querybase.db
+-rw-r--r--   0 runner    (1001) docker     (123)      138 2023-06-16 09:46:48.000000 decore_Base-0.0.21/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)     1174 2023-06-16 09:46:48.000000 decore_Base-0.0.21/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     2053 2023-06-16 09:46:56.134879 decore_Base-0.0.21/setup.cfg
```

### Comparing `decore_Base-0.0.20/.github/FUNDING.yml` & `decore_Base-0.0.21/.github/FUNDING.yml`

 * *Files identical despite different names*

### Comparing `decore_Base-0.0.20/.gitignore` & `decore_Base-0.0.21/decore_base/prepare/.gitignore`

 * *Files 2% similar despite different names*

```diff
@@ -65,15 +65,15 @@
 instance/
 .webassets-cache
 
 # Scrapy stuff:
 .scrapy
 
 # Sphinx documentation
-# docs/_build/
+docs/_build/
 
 # PyBuilder
 .pybuilder/
 target/
 
 # Jupyter Notebook
 .ipynb_checkpoints
```

### Comparing `decore_Base-0.0.20/.vscode/launch.json` & `decore_Base-0.0.21/.vscode/launch.json`

 * *Files identical despite different names*

### Comparing `decore_Base-0.0.20/KOFI.md` & `decore_Base-0.0.21/KOFI.md`

 * *Files identical despite different names*

### Comparing `decore_Base-0.0.20/LICENSE` & `decore_Base-0.0.21/LICENSE`

 * *Files identical despite different names*

### Comparing `decore_Base-0.0.20/PKG-INFO` & `decore_Base-0.0.21/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: decore_Base
-Version: 0.0.20
+Version: 0.0.21
 Summary: decore Base is an out-of-the-box "Python to Vue.js" data application dashboard that helps you go from idea to view in a few simple steps. It is aimed at those who want to focus on the results of their algorithms , do scientific work, or perform teaching or learning functions.
 Home-page: https://www.decore.dev
 Author: Kemo Panzah
 Project-URL: Funding, https://ko-fi.com/decore_Base
 Project-URL: Source, https://github.com/KemoPanzah/decore_Base
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
@@ -131,14 +131,23 @@
    @decore.base(title='First Base', icon='mdi-home', model=First_model)
    class First_base:
       pass
 
 .. note::
    To use the previously created model, we import it into the Base class and pass it to the ``model`` parameter.
 
+.. warning::
+   In order for the Python interpreter to be able to process the base classes, we have to import them into the __init__.py file in the **bases** directory. The order of the individual imports also determines the order in **decore Front**.
+   
+   We edit the **__init__.py** file and insert the following code:
+
+   .. code-block:: python
+
+      from .first_base import First_base
+
 View
 ~~~~
 Views are used by the decore application to present the data sets in the **decore Front** web application.
 
 With the view decorator we can now create a view component and link it to the previously created base class.
 
 We now edit the **first_base.py** file again and extend the code as follows:
```

### Comparing `decore_Base-0.0.20/README.rst` & `decore_Base-0.0.21/README.rst`

 * *Files 3% similar despite different names*

```diff
@@ -117,14 +117,23 @@
    @decore.base(title='First Base', icon='mdi-home', model=First_model)
    class First_base:
       pass
 
 .. note::
    To use the previously created model, we import it into the Base class and pass it to the ``model`` parameter.
 
+.. warning::
+   In order for the Python interpreter to be able to process the base classes, we have to import them into the __init__.py file in the **bases** directory. The order of the individual imports also determines the order in **decore Front**.
+   
+   We edit the **__init__.py** file and insert the following code:
+
+   .. code-block:: python
+
+      from .first_base import First_base
+
 View
 ~~~~
 Views are used by the decore application to present the data sets in the **decore Front** web application.
 
 With the view decorator we can now create a view component and link it to the previously created base class.
 
 We now edit the **first_base.py** file again and extend the code as follows:
```

### Comparing `decore_Base-0.0.20/README_DE.rst` & `decore_Base-0.0.21/README_DE.rst`

 * *Files 2% similar despite different names*

```diff
@@ -117,14 +117,23 @@
    @decore.base(title='First Base', icon='mdi-home', model=First_model)
    class First_base:
       pass
 
 .. note::
    Um das zuvor erstellte Model zu verwenden, importieren wir dieses in die Base-Klasse und übergeben es dem Parameter ``model``.
 
+.. warning::
+   Damit der Python-Interpreter die Basisklassen auch verarbeiten kann, müssen wir diese in der __init__.py Datei im Verzeichnis **bases** importieren. Die Reihenfolge der einzelnen Importe gibt auch die Reihenfolge in **decore Front** vor.
+   
+   Wir editiren die Datei **__init__.py** und fügen folgenden Code ein:
+
+   .. code-block:: python
+
+      from .first_base import First_base
+
 View
 ~~~~
 Views dienen der decore Applikation als Präsentation der Datensätze in der **decore Front** Web-Anwendung.
 
 Mit dem View-Dekorator können wir nun eine View-Komponente erzeugen und diese mit der zuvor erstellten Base-Klasse verknüpfen.
 
 Wir editieren nun wieder die Datei **first_base.py** und erweitern den Code wie folgt:
```

### Comparing `decore_Base-0.0.20/decore_Base.egg-info/PKG-INFO` & `decore_Base-0.0.21/decore_Base.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: decore-Base
-Version: 0.0.20
+Version: 0.0.21
 Summary: decore Base is an out-of-the-box "Python to Vue.js" data application dashboard that helps you go from idea to view in a few simple steps. It is aimed at those who want to focus on the results of their algorithms , do scientific work, or perform teaching or learning functions.
 Home-page: https://www.decore.dev
 Author: Kemo Panzah
 Project-URL: Funding, https://ko-fi.com/decore_Base
 Project-URL: Source, https://github.com/KemoPanzah/decore_Base
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
@@ -131,14 +131,23 @@
    @decore.base(title='First Base', icon='mdi-home', model=First_model)
    class First_base:
       pass
 
 .. note::
    To use the previously created model, we import it into the Base class and pass it to the ``model`` parameter.
 
+.. warning::
+   In order for the Python interpreter to be able to process the base classes, we have to import them into the __init__.py file in the **bases** directory. The order of the individual imports also determines the order in **decore Front**.
+   
+   We edit the **__init__.py** file and insert the following code:
+
+   .. code-block:: python
+
+      from .first_base import First_base
+
 View
 ~~~~
 Views are used by the decore application to present the data sets in the **decore Front** web application.
 
 With the view decorator we can now create a view component and link it to the previously created base class.
 
 We now edit the **first_base.py** file again and extend the code as follows:
```

### Comparing `decore_Base-0.0.20/decore_Base.egg-info/SOURCES.txt` & `decore_Base-0.0.21/decore_Base.egg-info/SOURCES.txt`

 * *Files 5% similar despite different names*

```diff
@@ -122,39 +122,32 @@
 decore_base/uniform/depricated/conform_base.py
 decore_base/uniform/depricated/deform_base.py
 docs/.nojekyll
 docs/CNAME
 docs/Makefile
 docs/conf.py
 docs/config.json
-docs/decore.rst
+docs/decore.rst.out
 docs/index.html
 docs/index.rst
 docs/language.json
 docs/make.bat
-docs/model.rst
+docs/model.rst.out
 docs/_static/favicon.ico
 docs/_static/logo.png
 docs/_static/styles/custom.css
-docs/page/doctrees/decore.doctree
 docs/page/doctrees/environment.pickle
 docs/page/doctrees/index.doctree
-docs/page/doctrees/model.doctree
 docs/page/html/.buildinfo
-docs/page/html/decore.html
 docs/page/html/genindex.html
 docs/page/html/index.html
-docs/page/html/model.html
 docs/page/html/objects.inv
-docs/page/html/py-modindex.html
 docs/page/html/search.html
 docs/page/html/searchindex.js
-docs/page/html/_sources/decore.rst.txt
 docs/page/html/_sources/index.rst.txt
-docs/page/html/_sources/model.rst.txt
 docs/page/html/_static/basic.css
 docs/page/html/_static/check-solid.svg
 docs/page/html/_static/clipboard.min.js
 docs/page/html/_static/copy-button.svg
 docs/page/html/_static/copybutton.css
 docs/page/html/_static/copybutton.js
 docs/page/html/_static/copybutton_funcs.js
```

### Comparing `decore_Base-0.0.20/decore_Base.egg-info/requires.txt` & `decore_Base-0.0.21/decore_Base.egg-info/requires.txt`

 * *Files identical despite different names*

### Comparing `decore_Base-0.0.20/decore_base/classes/decore_base.py` & `decore_Base-0.0.21/decore_base/classes/decore_base.py`

 * *Files identical despite different names*

### Comparing `decore_Base-0.0.20/decore_base/classes/decore_list.py` & `decore_Base-0.0.21/decore_base/classes/decore_list.py`

 * *Files identical despite different names*

### Comparing `decore_Base-0.0.20/decore_base/classes/decore_model.py` & `decore_Base-0.0.21/decore_base/classes/decore_model.py`

 * *Files identical despite different names*

### Comparing `decore_Base-0.0.20/decore_base/classes/decore_pool.py` & `decore_Base-0.0.21/decore_base/classes/decore_pool.py`

 * *Files identical despite different names*

### Comparing `decore_Base-0.0.20/decore_base/classes/decore_prompt.py` & `decore_Base-0.0.21/decore_base/classes/decore_prompt.py`

 * *Files identical despite different names*

### Comparing `decore_Base-0.0.20/decore_base/classes/decore_query.py` & `decore_Base-0.0.21/decore_base/classes/decore_query.py`

 * *Files identical despite different names*

### Comparing `decore_Base-0.0.20/decore_base/classes/decore_return.py` & `decore_Base-0.0.21/decore_base/classes/decore_return.py`

 * *Files identical despite different names*

### Comparing `decore_Base-0.0.20/decore_base/classes/decore_translate.py` & `decore_Base-0.0.21/decore_base/classes/decore_translate.py`

 * *Files identical despite different names*

### Comparing `decore_Base-0.0.20/decore_base/classes/decore_view.py` & `decore_Base-0.0.21/decore_base/classes/decore_view.py`

 * *Files identical despite different names*

### Comparing `decore_Base-0.0.20/decore_base/decore.py` & `decore_Base-0.0.21/decore_base/decore.py`

 * *Files 7% similar despite different names*

```diff
@@ -79,127 +79,127 @@
             logger.info('Press CTRL+C to quit.')
             logger.setLevel(logging.WARNING)
             serve(self.api, host=HOST, port=PORT)
             
         else:
             self.api.run(HOST, PORT)
 
-    def app(self, p_title):
+    def app(self, title):
         '''Decorator for app registration'''
         def wrapper(func):
-            self.pool.register(Decore_app('app', None, None, None, p_title, None, func.__doc__))
+            self.pool.register(Decore_app('app', None, None, None, title, None, func.__doc__))
             self.pool.extend()
             i_base: Decore_base
             for i_base in self.pool.base_s:
                 i_base.start_shot()
                 i_base.start_work()
             self.start_api()
         return wrapper
 
-    def base(self, p_icon=None, p_title=None, p_desc=None, p_model=Decore_model):
+    def base(self, icon=None, title=None, desc=None, model=Decore_model):
         def wrapper(cls):
             class Base(cls, Decore_base):
                 def __init__(self):
                     cls.__init__(self)
                     Decore_base.__init__(self)
                    
             t_base = type(cls.__name__, (Base,), {})()
             t_base.id = cls.__name__
-            t_base.icon = p_icon
-            t_base.title = p_title
-            t_base.desc = p_desc
+            t_base.icon = icon
+            t_base.title = title
+            t_base.desc = desc
             t_base.doc = cls.__doc__
-            t_base.model = p_model.register()
-            t_base.field_s = p_model.field_s
-            t_base.rel_field_s = p_model.rel_field_s
-            t_base.schema = p_model.build_schema()
+            t_base.model = model.register()
+            t_base.field_s = model.field_s
+            t_base.rel_field_s = model.rel_field_s
+            t_base.schema = model.build_schema()
             self.pool.register(t_base)
         return wrapper
 
     l_view_type = Literal['table']
     l_view_pag_type = Literal['client']
 
-    def view(self, p_parent_id=None, p_icon=None, p_title=None, p_desc=None, p_type: l_view_type = 'table', p_active_s=[], p_filter_s=[], p_query={}, p_pag_type: l_view_pag_type = 'client', p_pag_recs=16):
+    def view(self, parent_id=None, icon=None, title=None, desc=None, type: l_view_type = 'table', fields=[], filter_s=[], query={}, pag_type: l_view_pag_type = 'client', pag_recs=16):
         def wrapper(func):
             t_parent_s = func.__qualname__.replace('.<locals>', '').rsplit('.')
-            if not p_parent_id:
+            if not parent_id:
                 t_parent_id = t_parent_s[-2]
             else:
-                t_parent_id = p_parent_id
+                t_parent_id = parent_id
             t_source_id = t_parent_s[0]
-            self.pool.register(Decore_view(func.__name__, t_parent_id, t_source_id, p_icon, p_title, p_desc, func.__doc__, p_type, p_active_s, p_filter_s, p_query, p_pag_type, p_pag_recs))
+            self.pool.register(Decore_view(func.__name__, t_parent_id, t_source_id, icon, title, desc, func.__doc__, type, fields, filter_s, query, pag_type, pag_recs))
             func()
         return wrapper
 
     l_dialog_type = Literal['standard', 'tabs', 'stepper']
     l_dialog_display = Literal['modal', 'drawer']
     l_dialog_activator = Literal['none', 'default-menu', 'item-menu', 'item-click']
 
     # TODO - Überprüfen ob element mit gleicher ID schon vorhanden ist und Execption
-    def dialog(self, p_parent_id=None, p_icon=None, p_title=None, p_desc=None, p_type: l_dialog_type = 'standard', p_display: l_dialog_display = 'drawer', p_activator: l_dialog_activator = 'none'):
+    def dialog(self, parent_id=None, icon=None, title=None, desc=None, type: l_dialog_type = 'standard', display: l_dialog_display = 'drawer', activator: l_dialog_activator = 'none'):
         def wrapper(func):
             t_parent_s = func.__qualname__.replace('.<locals>', '').rsplit('.')
-            if not p_parent_id:
+            if not parent_id:
                 t_parent_id = t_parent_s[-2]
             else:
-                t_parent_id = p_parent_id
+                t_parent_id = parent_id
             t_source_id = t_parent_s[0]
-            self.pool.register(Decore_dialog(func.__name__, t_parent_id, t_source_id, p_icon, p_title, p_desc, func.__doc__, p_type, p_display, p_activator))
+            self.pool.register(Decore_dialog(func.__name__, t_parent_id, t_source_id, icon, title, desc, func.__doc__, type, display, activator))
             func()
         return wrapper
 
     l_widget_type = Literal['default', 'info', 'form', 'table']
 
-    def widget(self, p_parent_id=None, p_icon=None, p_title=None, p_desc=None, p_type: l_widget_type = 'default', p_layout='cera', p_active_s=[]):
+    def widget(self, parent_id=None, icon=None, title=None, desc=None, type: l_widget_type = 'default', layout='cera', fields=[]):
         def wrapper(func):
             t_parent_s = func.__qualname__.replace('.<locals>', '').rsplit('.')
-            if not p_parent_id:
+            if not parent_id:
                 t_parent_id = t_parent_s[-2]
             else:
-                t_parent_id = p_parent_id
+                t_parent_id = parent_id
             t_source_id = t_parent_s[0]
-            self.pool.register(Decore_widget(func.__name__, t_parent_id, t_source_id, p_icon, p_title, p_desc, func.__doc__, p_type, p_layout, p_active_s))
+            self.pool.register(Decore_widget(func.__name__, t_parent_id, t_source_id, icon, title, desc, func.__doc__, type, layout, fields))
             func()
         return wrapper
 
     l_element_type = Literal['p', 'checkbox']
 
-    def element(self, p_parent_id=None, p_icon=None, p_title=None, p_desc=None, p_type: l_element_type = 'text', p_default=None, p_disable=False, p_schema=None):
+    def element(self, parent_id=None, icon=None, title=None, desc=None, type: l_element_type = 'text', default=None, disable=False, schema=None):
         def wrapper(func):
             t_parent_s = func.__qualname__.replace('.<locals>', '').rsplit('.')
-            if not p_parent_id:
+            if not parent_id:
                 t_parent_id = t_parent_s[-2]
             else:
-                t_parent_id = p_parent_id
+                t_parent_id = parent_id
             t_source_id = t_parent_s[0]
-            self.pool.register(Decore_element(func.__name__, t_parent_id, t_source_id, p_icon, p_title, p_desc, p_type, p_default, p_disable, p_schema, func))
+            self.pool.register(Decore_element(func.__name__, t_parent_id, t_source_id, icon, title, desc, type, default, disable, schema, func))
         return wrapper
 
     l_action_type = Literal['standard', 'submit', 'check', 'response', 'file', 'download']
     l_action_activator = Literal['none', 'default-menu', 'item-menu', 'item-click']
 
-    def action(self, p_parent_id=None, p_icon=None, p_title=None, p_desc=None, p_type: l_action_type = 'standard', p_activator: l_action_activator = 'none'):
+    def action(self, parent_id=None, icon=None, title=None, desc=None, type: l_action_type = 'standard', activator: l_action_activator = 'none'):
         def wrapper(func):
             t_parent_s = func.__qualname__.replace('.<locals>', '').rsplit('.')
-            if not p_parent_id:
+            if not parent_id:
                 t_parent_id = t_parent_s[-2]
             else:
-                t_parent_id = p_parent_id
+                t_parent_id = parent_id
             t_source_id = t_parent_s[0]
-            self.pool.register(Decore_action(func.__name__, t_parent_id, t_source_id, p_icon, p_title, p_desc, func.__doc__, p_type, p_activator, func))
+            self.pool.register(Decore_action(func.__name__, t_parent_id, t_source_id, icon, title, desc, func.__doc__, type, activator, func))
         return wrapper
 
     l_function_type = Literal['shot', 'work']
   
-    def function(self, p_type:l_function_type = 'shot'):
+    def function(self, type:l_function_type = 'shot'):
         def wrapper(func):
             t_parent_s = func.__qualname__.replace('.<locals>', '').rsplit('.')
             t_parent_id = t_parent_s[-2]
             t_source_id = t_parent_s[0]
-            self.pool.register(Decore_function(func.__name__, t_parent_id, t_source_id, None, None, None, func.__doc__, p_type, func))
+            self.pool.register(Decore_function(func.__name__, t_parent_id, t_source_id, None, None, None, func.__doc__, type, func))
         return wrapper
 
     def get_base_by_id(self, p_id):
         i_base: Decore_base
         for i_base in self.pool.base_s:
             if i_base.id == p_id:
                 return i_base
```

### Comparing `decore_Base-0.0.20/decore_base/globals.py` & `decore_Base-0.0.21/decore_base/globals.py`

 * *Files identical despite different names*

### Comparing `decore_Base-0.0.20/decore_base/library/particl_market/particl_market.py` & `decore_Base-0.0.21/decore_base/library/particl_market/particl_market.py`

 * *Files identical despite different names*

### Comparing `decore_Base-0.0.20/decore_base/library/powershell.py` & `decore_Base-0.0.21/decore_base/library/powershell.py`

 * *Files identical despite different names*

### Comparing `decore_Base-0.0.20/decore_base/library/powershell2.py` & `decore_Base-0.0.21/decore_base/library/powershell2.py`

 * *Files identical despite different names*

### Comparing `decore_Base-0.0.20/decore_base/library/return_value.py` & `decore_Base-0.0.21/decore_base/library/return_value.py`

 * *Files identical despite different names*

### Comparing `decore_Base-0.0.20/decore_base/library/roaster/roaster_client.py` & `decore_Base-0.0.21/decore_base/library/roaster/roaster_client.py`

 * *Files identical despite different names*

### Comparing `decore_Base-0.0.20/decore_base/library/roaster/roaster_functions.py` & `decore_Base-0.0.21/decore_base/library/roaster/roaster_functions.py`

 * *Files identical despite different names*

### Comparing `decore_Base-0.0.20/decore_base/library/roaster/roaster_server.py` & `decore_Base-0.0.21/decore_base/library/roaster/roaster_server.py`

 * *Files identical despite different names*

### Comparing `decore_Base-0.0.20/decore_base/prepare/.gitignore` & `decore_Base-0.0.21/decore_base/sample/.gitignore`

 * *Files identical despite different names*

### Comparing `decore_Base-0.0.20/decore_base/prepare/.vscode/launch.json` & `decore_Base-0.0.21/decore_base/prepare/.vscode/launch.json`

 * *Files identical despite different names*

### Comparing `decore_Base-0.0.20/decore_base/prepare/spa/static/css/586.ed179a62.css` & `decore_Base-0.0.21/decore_base/prepare/spa/static/css/586.ed179a62.css`

 * *Files identical despite different names*

### Comparing `decore_Base-0.0.20/decore_base/prepare/spa/static/css/app.d398f07d.css` & `decore_Base-0.0.21/decore_base/prepare/spa/static/css/app.d398f07d.css`

 * *Files identical despite different names*

### Comparing `decore_Base-0.0.20/decore_base/prepare/spa/static/css/vendor.14c9ac7a.css` & `decore_Base-0.0.21/decore_base/prepare/spa/static/css/vendor.14c9ac7a.css`

 * *Files identical despite different names*

### Comparing `decore_Base-0.0.20/decore_base/prepare/spa/static/favicon.ico` & `decore_Base-0.0.21/decore_base/prepare/spa/static/favicon.ico`

 * *Files identical despite different names*

### Comparing `decore_Base-0.0.20/decore_base/prepare/spa/static/fonts/KFOkCnqEu92Fr1MmgVxIIzQ.68bb21d0.woff` & `decore_Base-0.0.21/decore_base/prepare/spa/static/fonts/KFOkCnqEu92Fr1MmgVxIIzQ.68bb21d0.woff`

 * *Files identical despite different names*

### Comparing `decore_Base-0.0.20/decore_base/prepare/spa/static/fonts/KFOlCnqEu92Fr1MmEU9fBBc-.48af7707.woff` & `decore_Base-0.0.21/decore_base/prepare/spa/static/fonts/KFOlCnqEu92Fr1MmEU9fBBc-.48af7707.woff`

 * *Files identical despite different names*

### Comparing `decore_Base-0.0.20/decore_base/prepare/spa/static/fonts/KFOlCnqEu92Fr1MmSU5fBBc-.c2f7ab22.woff` & `decore_Base-0.0.21/decore_base/prepare/spa/static/fonts/KFOlCnqEu92Fr1MmSU5fBBc-.c2f7ab22.woff`

 * *Files identical despite different names*

### Comparing `decore_Base-0.0.20/decore_base/prepare/spa/static/fonts/KFOlCnqEu92Fr1MmWUlfBBc-.77ecb942.woff` & `decore_Base-0.0.21/decore_base/prepare/spa/static/fonts/KFOlCnqEu92Fr1MmWUlfBBc-.77ecb942.woff`

 * *Files identical despite different names*

### Comparing `decore_Base-0.0.20/decore_base/prepare/spa/static/fonts/KFOlCnqEu92Fr1MmYUtfBBc-.f5677eb2.woff` & `decore_Base-0.0.21/decore_base/prepare/spa/static/fonts/KFOlCnqEu92Fr1MmYUtfBBc-.f5677eb2.woff`

 * *Files identical despite different names*

### Comparing `decore_Base-0.0.20/decore_base/prepare/spa/static/fonts/KFOmCnqEu92Fr1Mu4mxM.f1e2a767.woff` & `decore_Base-0.0.21/decore_base/prepare/spa/static/fonts/KFOmCnqEu92Fr1Mu4mxM.f1e2a767.woff`

 * *Files identical despite different names*

### Comparing `decore_Base-0.0.20/decore_base/prepare/spa/static/fonts/flUhRq6tzZclQEJ-Vdg-IuiaDsNa.4d73cb90.woff` & `decore_Base-0.0.21/decore_base/prepare/spa/static/fonts/flUhRq6tzZclQEJ-Vdg-IuiaDsNa.4d73cb90.woff`

 * *Files identical despite different names*

### Comparing `decore_Base-0.0.20/decore_base/prepare/spa/static/fonts/flUhRq6tzZclQEJ-Vdg-IuiaDsNcIhQ8tQ.0383092b.woff2` & `decore_Base-0.0.21/decore_base/prepare/spa/static/fonts/flUhRq6tzZclQEJ-Vdg-IuiaDsNcIhQ8tQ.0383092b.woff2`

 * *Files identical despite different names*

### Comparing `decore_Base-0.0.20/decore_base/prepare/spa/static/fonts/materialdesignicons-webfont.d8e8e0f7.woff` & `decore_Base-0.0.21/decore_base/prepare/spa/static/fonts/materialdesignicons-webfont.d8e8e0f7.woff`

 * *Files identical despite different names*

### Comparing `decore_Base-0.0.20/decore_base/prepare/spa/static/fonts/materialdesignicons-webfont.e9db4005.woff2` & `decore_Base-0.0.21/decore_base/prepare/spa/static/fonts/materialdesignicons-webfont.e9db4005.woff2`

 * *Files identical despite different names*

### Comparing `decore_Base-0.0.20/decore_base/prepare/spa/static/icons/favicon-128x128.png` & `decore_Base-0.0.21/decore_base/prepare/spa/static/icons/favicon-128x128.png`

 * *Files identical despite different names*

### Comparing `decore_Base-0.0.20/decore_base/prepare/spa/static/icons/favicon-16x16.png` & `decore_Base-0.0.21/decore_base/prepare/spa/static/icons/favicon-16x16.png`

 * *Files identical despite different names*

### Comparing `decore_Base-0.0.20/decore_base/prepare/spa/static/icons/favicon-32x32.png` & `decore_Base-0.0.21/decore_base/prepare/spa/static/icons/favicon-32x32.png`

 * *Files identical despite different names*

### Comparing `decore_Base-0.0.20/decore_base/prepare/spa/static/icons/favicon-96x96.png` & `decore_Base-0.0.21/decore_base/prepare/spa/static/icons/favicon-96x96.png`

 * *Files identical despite different names*

### Comparing `decore_Base-0.0.20/decore_base/prepare/spa/static/js/586.aa14c175.js` & `decore_Base-0.0.21/decore_base/prepare/spa/static/js/586.aa14c175.js`

 * *Files identical despite different names*

### Comparing `decore_Base-0.0.20/decore_base/prepare/spa/static/js/65.940d9b80.js` & `decore_Base-0.0.21/decore_base/prepare/spa/static/js/65.940d9b80.js`

 * *Files identical despite different names*

### Comparing `decore_Base-0.0.20/decore_base/prepare/spa/static/js/app.af6cbe84.js` & `decore_Base-0.0.21/decore_base/prepare/spa/static/js/app.af6cbe84.js`

 * *Files identical despite different names*

### Comparing `decore_Base-0.0.20/decore_base/prepare/spa/static/js/vendor.0902ddb5.js` & `decore_Base-0.0.21/decore_base/prepare/spa/static/js/vendor.0902ddb5.js`

 * *Files identical despite different names*

### Comparing `decore_Base-0.0.20/decore_base/prepare/spa/templates/index.html` & `decore_Base-0.0.21/decore_base/prepare/spa/templates/index.html`

 * *Files identical despite different names*

### Comparing `decore_Base-0.0.20/decore_base/sample/.gitignore` & `decore_Base-0.0.21/.gitignore`

 * *Files 1% similar despite different names*

```diff
@@ -64,15 +64,15 @@
 # Flask stuff:
 instance/
 .webassets-cache
 
 # Scrapy stuff:
 .scrapy
 
-# Sphinx documentation
+Sphinx documentation
 docs/_build/
 
 # PyBuilder
 .pybuilder/
 target/
 
 # Jupyter Notebook
```

### Comparing `decore_Base-0.0.20/decore_base/sample/.vscode/launch.json` & `decore_Base-0.0.21/decore_base/sample/.vscode/launch.json`

 * *Files identical despite different names*

### Comparing `decore_Base-0.0.20/decore_base/sample/bases/account_base.py` & `decore_Base-0.0.21/decore_base/sample/bases/account_base.py`

 * *Files identical despite different names*

### Comparing `decore_Base-0.0.20/decore_base/sample/bases/company_base.py` & `decore_Base-0.0.21/decore_base/sample/bases/company_base.py`

 * *Files identical despite different names*

### Comparing `decore_Base-0.0.20/decore_base/sample/bases/global_management_base.py` & `decore_Base-0.0.21/decore_base/sample/bases/global_management_base.py`

 * *Files identical despite different names*

### Comparing `decore_Base-0.0.20/decore_base/sample/bases/person_base.py` & `decore_Base-0.0.21/decore_base/sample/bases/person_base.py`

 * *Files identical despite different names*

### Comparing `decore_Base-0.0.20/decore_base/sample/bases/test_base.py` & `decore_Base-0.0.21/decore_base/sample/bases/test_base.py`

 * *Files identical despite different names*

### Comparing `decore_Base-0.0.20/decore_base/sample/models/person_model.py` & `decore_Base-0.0.21/decore_base/sample/models/person_model.py`

 * *Files identical despite different names*

### Comparing `decore_Base-0.0.20/decore_base/sample/models/test_model.py` & `decore_Base-0.0.21/decore_base/sample/models/test_model.py`

 * *Files identical despite different names*

### Comparing `decore_Base-0.0.20/decore_base/sample/spa/static/css/586.ed179a62.css` & `decore_Base-0.0.21/decore_base/sample/spa/static/css/586.ed179a62.css`

 * *Files identical despite different names*

### Comparing `decore_Base-0.0.20/decore_base/sample/spa/static/css/app.d398f07d.css` & `decore_Base-0.0.21/decore_base/sample/spa/static/css/app.d398f07d.css`

 * *Files identical despite different names*

### Comparing `decore_Base-0.0.20/decore_base/sample/spa/static/css/vendor.14c9ac7a.css` & `decore_Base-0.0.21/decore_base/sample/spa/static/css/vendor.14c9ac7a.css`

 * *Files identical despite different names*

### Comparing `decore_Base-0.0.20/decore_base/sample/spa/static/favicon.ico` & `decore_Base-0.0.21/decore_base/sample/spa/static/favicon.ico`

 * *Files identical despite different names*

### Comparing `decore_Base-0.0.20/decore_base/sample/spa/static/fonts/KFOkCnqEu92Fr1MmgVxIIzQ.68bb21d0.woff` & `decore_Base-0.0.21/decore_base/sample/spa/static/fonts/KFOkCnqEu92Fr1MmgVxIIzQ.68bb21d0.woff`

 * *Files identical despite different names*

### Comparing `decore_Base-0.0.20/decore_base/sample/spa/static/fonts/KFOlCnqEu92Fr1MmEU9fBBc-.48af7707.woff` & `decore_Base-0.0.21/decore_base/sample/spa/static/fonts/KFOlCnqEu92Fr1MmEU9fBBc-.48af7707.woff`

 * *Files identical despite different names*

### Comparing `decore_Base-0.0.20/decore_base/sample/spa/static/fonts/KFOlCnqEu92Fr1MmSU5fBBc-.c2f7ab22.woff` & `decore_Base-0.0.21/decore_base/sample/spa/static/fonts/KFOlCnqEu92Fr1MmSU5fBBc-.c2f7ab22.woff`

 * *Files identical despite different names*

### Comparing `decore_Base-0.0.20/decore_base/sample/spa/static/fonts/KFOlCnqEu92Fr1MmWUlfBBc-.77ecb942.woff` & `decore_Base-0.0.21/decore_base/sample/spa/static/fonts/KFOlCnqEu92Fr1MmWUlfBBc-.77ecb942.woff`

 * *Files identical despite different names*

### Comparing `decore_Base-0.0.20/decore_base/sample/spa/static/fonts/KFOlCnqEu92Fr1MmYUtfBBc-.f5677eb2.woff` & `decore_Base-0.0.21/decore_base/sample/spa/static/fonts/KFOlCnqEu92Fr1MmYUtfBBc-.f5677eb2.woff`

 * *Files identical despite different names*

### Comparing `decore_Base-0.0.20/decore_base/sample/spa/static/fonts/KFOmCnqEu92Fr1Mu4mxM.f1e2a767.woff` & `decore_Base-0.0.21/decore_base/sample/spa/static/fonts/KFOmCnqEu92Fr1Mu4mxM.f1e2a767.woff`

 * *Files identical despite different names*

### Comparing `decore_Base-0.0.20/decore_base/sample/spa/static/fonts/flUhRq6tzZclQEJ-Vdg-IuiaDsNa.4d73cb90.woff` & `decore_Base-0.0.21/decore_base/sample/spa/static/fonts/flUhRq6tzZclQEJ-Vdg-IuiaDsNa.4d73cb90.woff`

 * *Files identical despite different names*

### Comparing `decore_Base-0.0.20/decore_base/sample/spa/static/fonts/flUhRq6tzZclQEJ-Vdg-IuiaDsNcIhQ8tQ.0383092b.woff2` & `decore_Base-0.0.21/decore_base/sample/spa/static/fonts/flUhRq6tzZclQEJ-Vdg-IuiaDsNcIhQ8tQ.0383092b.woff2`

 * *Files identical despite different names*

### Comparing `decore_Base-0.0.20/decore_base/sample/spa/static/fonts/materialdesignicons-webfont.d8e8e0f7.woff` & `decore_Base-0.0.21/decore_base/sample/spa/static/fonts/materialdesignicons-webfont.d8e8e0f7.woff`

 * *Files identical despite different names*

### Comparing `decore_Base-0.0.20/decore_base/sample/spa/static/fonts/materialdesignicons-webfont.e9db4005.woff2` & `decore_Base-0.0.21/decore_base/sample/spa/static/fonts/materialdesignicons-webfont.e9db4005.woff2`

 * *Files identical despite different names*

### Comparing `decore_Base-0.0.20/decore_base/sample/spa/static/icons/favicon-128x128.png` & `decore_Base-0.0.21/decore_base/sample/spa/static/icons/favicon-128x128.png`

 * *Files identical despite different names*

### Comparing `decore_Base-0.0.20/decore_base/sample/spa/static/icons/favicon-16x16.png` & `decore_Base-0.0.21/decore_base/sample/spa/static/icons/favicon-16x16.png`

 * *Files identical despite different names*

### Comparing `decore_Base-0.0.20/decore_base/sample/spa/static/icons/favicon-32x32.png` & `decore_Base-0.0.21/decore_base/sample/spa/static/icons/favicon-32x32.png`

 * *Files identical despite different names*

### Comparing `decore_Base-0.0.20/decore_base/sample/spa/static/icons/favicon-96x96.png` & `decore_Base-0.0.21/decore_base/sample/spa/static/icons/favicon-96x96.png`

 * *Files identical despite different names*

### Comparing `decore_Base-0.0.20/decore_base/sample/spa/static/js/586.aa14c175.js` & `decore_Base-0.0.21/decore_base/sample/spa/static/js/586.aa14c175.js`

 * *Files identical despite different names*

### Comparing `decore_Base-0.0.20/decore_base/sample/spa/static/js/65.940d9b80.js` & `decore_Base-0.0.21/decore_base/sample/spa/static/js/65.940d9b80.js`

 * *Files identical despite different names*

### Comparing `decore_Base-0.0.20/decore_base/sample/spa/static/js/app.af6cbe84.js` & `decore_Base-0.0.21/decore_base/sample/spa/static/js/app.af6cbe84.js`

 * *Files identical despite different names*

### Comparing `decore_Base-0.0.20/decore_base/sample/spa/static/js/vendor.0902ddb5.js` & `decore_Base-0.0.21/decore_base/sample/spa/static/js/vendor.0902ddb5.js`

 * *Files identical despite different names*

### Comparing `decore_Base-0.0.20/decore_base/sample/spa/templates/index.html` & `decore_Base-0.0.21/decore_base/sample/spa/templates/index.html`

 * *Files identical despite different names*

### Comparing `decore_Base-0.0.20/decore_base/sample/state/database.db` & `decore_Base-0.0.21/decore_base/sample/state/database.db`

 * *Files identical despite different names*

### Comparing `decore_Base-0.0.20/decore_base/sample/state/keybase.kdbx` & `decore_Base-0.0.21/decore_base/sample/state/keybase.kdbx`

 * *Files identical despite different names*

### Comparing `decore_Base-0.0.20/decore_base/sample/state/querybase.db` & `decore_Base-0.0.21/decore_base/sample/state/querybase.db`

 * *Files identical despite different names*

### Comparing `decore_Base-0.0.20/decore_base/uniform/conform_model.py` & `decore_Base-0.0.21/decore_base/uniform/conform_model.py`

 * *Files identical despite different names*

### Comparing `decore_Base-0.0.20/decore_base/uniform/depricated/askform_base.py` & `decore_Base-0.0.21/decore_base/uniform/depricated/askform_base.py`

 * *Files identical despite different names*

### Comparing `decore_Base-0.0.20/decore_base/uniform/depricated/buyform_base.py` & `decore_Base-0.0.21/decore_base/uniform/depricated/buyform_base.py`

 * *Files identical despite different names*

### Comparing `decore_Base-0.0.20/decore_base/uniform/depricated/conform_base.py` & `decore_Base-0.0.21/decore_base/uniform/depricated/conform_base.py`

 * *Files identical despite different names*

### Comparing `decore_Base-0.0.20/decore_base/uniform/depricated/deform_base.py` & `decore_Base-0.0.21/decore_base/uniform/depricated/deform_base.py`

 * *Files identical despite different names*

### Comparing `decore_Base-0.0.20/decore_base/uniform/perform_model.py` & `decore_Base-0.0.21/decore_base/uniform/perform_model.py`

 * *Files identical despite different names*

### Comparing `decore_Base-0.0.20/decore_base/uniform/reform_client_model.py` & `decore_Base-0.0.21/decore_base/uniform/reform_client_model.py`

 * *Files identical despite different names*

### Comparing `decore_Base-0.0.20/decore_base/uniform/reform_server_model.py` & `decore_Base-0.0.21/decore_base/uniform/reform_server_model.py`

 * *Files identical despite different names*

### Comparing `decore_Base-0.0.20/docs/Makefile` & `decore_Base-0.0.21/docs/Makefile`

 * *Files identical despite different names*

### Comparing `decore_Base-0.0.20/docs/_static/favicon.ico` & `decore_Base-0.0.21/docs/_static/favicon.ico`

 * *Files identical despite different names*

### Comparing `decore_Base-0.0.20/docs/_static/logo.png` & `decore_Base-0.0.21/docs/_static/logo.png`

 * *Files identical despite different names*

### Comparing `decore_Base-0.0.20/docs/conf.py` & `decore_Base-0.0.21/docs/conf.py`

 * *Files identical despite different names*

### Comparing `decore_Base-0.0.20/docs/make.bat` & `decore_Base-0.0.21/docs/make.bat`

 * *Files identical despite different names*

### Comparing `decore_Base-0.0.20/docs/page/doctrees/index.doctree` & `decore_Base-0.0.21/docs/page/doctrees/index.doctree`

 * *Files 2% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-00000000: 8005 952c a600 0000 0000 008c 0f73 7068  ...,.........sph
+00000000: 8005 953c ad00 0000 0000 008c 0f73 7068  ...<.........sph
 00000010: 696e 782e 6164 646e 6f64 6573 948c 0864  inx.addnodes...d
 00000020: 6f63 756d 656e 7494 9394 2981 947d 9428  ocument...)..}.(
 00000030: 8c09 7261 7773 6f75 7263 6594 8c00 948c  ..rawsource.....
 00000040: 0863 6869 6c64 7265 6e94 5d94 288c 0e64  .children.].(..d
 00000050: 6f63 7574 696c 732e 6e6f 6465 7394 8c07  ocutils.nodes...
 00000060: 636f 6d6d 656e 7494 9394 2981 947d 9428  comment...)..}.(
 00000070: 6805 8cd0 6465 636f 7265 2042 6173 6520  h...decore Base 
@@ -1334,1327 +1334,1440 @@
 00005350: 0500 0068 2668 0368 274e 6829 4e75 6265  ...h&h.h'Nh)Nube
 00005360: 6817 7d94 2868 195d 9468 1b5d 9468 1d5d  h.}.(h.].h.].h.]
 00005370: 9468 1f5d 9468 215d 9475 6825 6851 6827  .h.].h!].uh%hQh'
 00005380: 6850 6829 4b7a 6816 6a7c 0500 0075 6261  hPh)Kzh.j|...uba
 00005390: 6817 7d94 2868 195d 9468 1b5d 9468 1d5d  h.}.(h.].h.].h.]
 000053a0: 9468 1f5d 9468 215d 9475 6825 6a47 0400  .h.].h!].uh%jG..
 000053b0: 0068 166a e504 0000 6826 6803 6827 6850  .h.j....h&h.h'hP
-000053c0: 6829 4e75 6265 6817 7d94 2868 195d 948c  h)Nubeh.}.(h.]..
-000053d0: 0462 6173 6594 6168 1b5d 9468 1d5d 948c  .base.ah.].h.]..
-000053e0: 0462 6173 6594 6168 1f5d 9468 215d 9475  .base.ah.].h!].u
-000053f0: 6825 682a 6816 6a21 0300 0068 2668 0368  h%h*h.j!...h&h.h
-00005400: 2768 5068 294b 6a75 6268 2b29 8194 7d94  'hPh)Kjubh+)..}.
-00005410: 2868 0568 0668 075d 9428 6830 2981 947d  (h.h.h.].(h0)..}
-00005420: 9428 6805 8c04 5669 6577 9468 075d 9468  .(h...View.h.].h
-00005430: 118c 0456 6965 7794 8594 8194 7d94 2868  ...View.....}.(h
-00005440: 166a b005 0000 6826 6803 6827 4e68 294e  .j....h&h.h'Nh)N
-00005450: 7562 6168 177d 9428 6819 5d94 681b 5d94  ubah.}.(h.].h.].
-00005460: 681d 5d94 681f 5d94 6821 5d94 7568 2568  h.].h.].h!].uh%h
-00005470: 2f68 166a ad05 0000 6826 6803 6827 6850  /h.j....h&h.h'hP
-00005480: 6829 4b7d 7562 6852 2981 947d 9428 6805  h)K}ubhR)..}.(h.
-00005490: 8c6a 5669 6577 7320 6172 6520 7573 6564  .jViews are used
-000054a0: 2062 7920 7468 6520 6465 636f 7265 2061   by the decore a
-000054b0: 7070 6c69 6361 7469 6f6e 2074 6f20 7072  pplication to pr
-000054c0: 6573 656e 7420 7468 6520 6461 7461 2073  esent the data s
-000054d0: 6574 7320 696e 2074 6865 202a 2a64 6563  ets in the **dec
-000054e0: 6f72 6520 4672 6f6e 742a 2a20 7765 6220  ore Front** web 
-000054f0: 6170 706c 6963 6174 696f 6e2e 9468 075d  application..h.]
-00005500: 9428 6811 8c49 5669 6577 7320 6172 6520  .(h..IViews are 
-00005510: 7573 6564 2062 7920 7468 6520 6465 636f  used by the deco
-00005520: 7265 2061 7070 6c69 6361 7469 6f6e 2074  re application t
-00005530: 6f20 7072 6573 656e 7420 7468 6520 6461  o present the da
-00005540: 7461 2073 6574 7320 696e 2074 6865 2094  ta sets in the .
-00005550: 8594 8194 7d94 2868 166a be05 0000 6826  ....}.(h.j....h&
-00005560: 6803 6827 4e68 294e 7562 6866 2981 947d  h.h'Nh)Nubhf)..}
-00005570: 9428 6805 8c10 2a2a 6465 636f 7265 2046  .(h...**decore F
-00005580: 726f 6e74 2a2a 9468 075d 9468 118c 0c64  ront**.h.].h...d
-00005590: 6563 6f72 6520 4672 6f6e 7494 8594 8194  ecore Front.....
-000055a0: 7d94 2868 166a c605 0000 6826 6803 6827  }.(h.j....h&h.h'
-000055b0: 4e68 294e 7562 6168 177d 9428 6819 5d94  Nh)Nubah.}.(h.].
-000055c0: 681b 5d94 681d 5d94 681f 5d94 6821 5d94  h.].h.].h.].h!].
-000055d0: 7568 2568 6568 166a be05 0000 7562 6811  uh%heh.j....ubh.
-000055e0: 8c11 2077 6562 2061 7070 6c69 6361 7469  .. web applicati
-000055f0: 6f6e 2e94 8594 8194 7d94 2868 166a be05  on......}.(h.j..
-00005600: 0000 6826 6803 6827 4e68 294e 7562 6568  ..h&h.h'Nh)Nubeh
-00005610: 177d 9428 6819 5d94 681b 5d94 681d 5d94  .}.(h.].h.].h.].
-00005620: 681f 5d94 6821 5d94 7568 2568 5168 2768  h.].h!].uh%hQh'h
-00005630: 5068 294b 7e68 166a ad05 0000 6826 6803  Ph)K~h.j....h&h.
-00005640: 7562 6852 2981 947d 9428 6805 8c6c 5769  ubhR)..}.(h..lWi
-00005650: 7468 2074 6865 2076 6965 7720 6465 636f  th the view deco
-00005660: 7261 746f 7220 7765 2063 616e 206e 6f77  rator we can now
-00005670: 2063 7265 6174 6520 6120 7669 6577 2063   create a view c
-00005680: 6f6d 706f 6e65 6e74 2061 6e64 206c 696e  omponent and lin
-00005690: 6b20 6974 2074 6f20 7468 6520 7072 6576  k it to the prev
-000056a0: 696f 7573 6c79 2063 7265 6174 6564 2062  iously created b
-000056b0: 6173 6520 636c 6173 732e 9468 075d 9468  ase class..h.].h
-000056c0: 118c 6c57 6974 6820 7468 6520 7669 6577  ..lWith the view
-000056d0: 2064 6563 6f72 6174 6f72 2077 6520 6361   decorator we ca
-000056e0: 6e20 6e6f 7720 6372 6561 7465 2061 2076  n now create a v
-000056f0: 6965 7720 636f 6d70 6f6e 656e 7420 616e  iew component an
-00005700: 6420 6c69 6e6b 2069 7420 746f 2074 6865  d link it to the
-00005710: 2070 7265 7669 6f75 736c 7920 6372 6561   previously crea
-00005720: 7465 6420 6261 7365 2063 6c61 7373 2e94  ted base class..
-00005730: 8594 8194 7d94 2868 166a de05 0000 6826  ....}.(h.j....h&
-00005740: 6803 6827 4e68 294e 7562 6168 177d 9428  h.h'Nh)Nubah.}.(
-00005750: 6819 5d94 681b 5d94 681d 5d94 681f 5d94  h.].h.].h.].h.].
-00005760: 6821 5d94 7568 2568 5168 2768 5068 294b  h!].uh%hQh'hPh)K
-00005770: 8068 166a ad05 0000 6826 6803 7562 6852  .h.j....h&h.ubhR
-00005780: 2981 947d 9428 6805 8c4c 5765 206e 6f77  )..}.(h..LWe now
-00005790: 2065 6469 7420 7468 6520 2a2a 6669 7273   edit the **firs
-000057a0: 745f 6261 7365 2e70 792a 2a20 6669 6c65  t_base.py** file
-000057b0: 2061 6761 696e 2061 6e64 2065 7874 656e   again and exten
-000057c0: 6420 7468 6520 636f 6465 2061 7320 666f  d the code as fo
-000057d0: 6c6c 6f77 733a 9468 075d 9428 6811 8c10  llows:.h.].(h...
-000057e0: 5765 206e 6f77 2065 6469 7420 7468 6520  We now edit the 
-000057f0: 9485 9481 947d 9428 6816 6aec 0500 0068  .....}.(h.j....h
-00005800: 2668 0368 274e 6829 4e75 6268 6629 8194  &h.h'Nh)Nubhf)..
-00005810: 7d94 2868 058c 112a 2a66 6972 7374 5f62  }.(h...**first_b
-00005820: 6173 652e 7079 2a2a 9468 075d 9468 118c  ase.py**.h.].h..
-00005830: 0d66 6972 7374 5f62 6173 652e 7079 9485  .first_base.py..
-00005840: 9481 947d 9428 6816 6af4 0500 0068 2668  ...}.(h.j....h&h
-00005850: 0368 274e 6829 4e75 6261 6817 7d94 2868  .h'Nh)Nubah.}.(h
-00005860: 195d 9468 1b5d 9468 1d5d 9468 1f5d 9468  .].h.].h.].h.].h
-00005870: 215d 9475 6825 6865 6816 6aec 0500 0075  !].uh%heh.j....u
-00005880: 6268 118c 2b20 6669 6c65 2061 6761 696e  bh..+ file again
-00005890: 2061 6e64 2065 7874 656e 6420 7468 6520   and extend the 
-000058a0: 636f 6465 2061 7320 666f 6c6c 6f77 733a  code as follows:
-000058b0: 9485 9481 947d 9428 6816 6aec 0500 0068  .....}.(h.j....h
-000058c0: 2668 0368 274e 6829 4e75 6265 6817 7d94  &h.h'Nh)Nubeh.}.
-000058d0: 2868 195d 9468 1b5d 9468 1d5d 9468 1f5d  (h.].h.].h.].h.]
-000058e0: 9468 215d 9475 6825 6851 6827 6850 6829  .h!].uh%hQh'hPh)
-000058f0: 4b82 6816 6aad 0500 0068 2668 0375 626a  K.h.j....h&h.ubj
-00005900: 1802 0000 2981 947d 9428 6805 583a 0100  ....)..}.(h.X:..
-00005910: 0066 726f 6d20 6465 636f 7265 5f62 6173  .from decore_bas
-00005920: 6520 696d 706f 7274 2064 6563 6f72 650a  e import decore.
-00005930: 6672 6f6d 206d 6f64 656c 732e 6669 7273  from models.firs
-00005940: 745f 6d6f 6465 6c20 696d 706f 7274 2046  t_model import F
-00005950: 6972 7374 5f6d 6f64 656c 0a0a 4064 6563  irst_model..@dec
-00005960: 6f72 652e 6261 7365 2874 6974 6c65 3d27  ore.base(title='
-00005970: 4669 7273 7420 4261 7365 272c 2069 636f  First Base', ico
-00005980: 6e3d 276d 6469 2d68 6f6d 6527 2c20 6d6f  n='mdi-home', mo
-00005990: 6465 6c3d 4669 7273 745f 6d6f 6465 6c29  del=First_model)
-000059a0: 0a63 6c61 7373 2046 6972 7374 5f62 6173  .class First_bas
-000059b0: 653a 0a20 2020 4064 6563 6f72 652e 7669  e:.   @decore.vi
-000059c0: 6577 2874 6974 6c65 3d27 4669 7273 7420  ew(title='First 
-000059d0: 5669 6577 272c 2069 636f 6e3d 276d 6469  View', icon='mdi
-000059e0: 2d68 6f6d 6527 2c20 7479 7065 3d27 7461  -home', type='ta
-000059f0: 626c 6527 2c20 6669 656c 6473 3d5b 4669  ble', fields=[Fi
-00005a00: 7273 745f 6d6f 6465 6c2e 6669 7273 746e  rst_model.firstn
-00005a10: 616d 652c 2046 6972 7374 5f6d 6f64 656c  ame, First_model
-00005a20: 2e6c 6173 746e 616d 655d 290a 2020 2064  .lastname]).   d
-00005a30: 6566 2066 6972 7374 5f76 6965 7728 293a  ef first_view():
-00005a40: 0a20 2020 2020 2070 6173 7394 6807 5d94  .      pass.h.].
-00005a50: 6811 583a 0100 0066 726f 6d20 6465 636f  h.X:...from deco
-00005a60: 7265 5f62 6173 6520 696d 706f 7274 2064  re_base import d
-00005a70: 6563 6f72 650a 6672 6f6d 206d 6f64 656c  ecore.from model
-00005a80: 732e 6669 7273 745f 6d6f 6465 6c20 696d  s.first_model im
-00005a90: 706f 7274 2046 6972 7374 5f6d 6f64 656c  port First_model
-00005aa0: 0a0a 4064 6563 6f72 652e 6261 7365 2874  ..@decore.base(t
-00005ab0: 6974 6c65 3d27 4669 7273 7420 4261 7365  itle='First Base
-00005ac0: 272c 2069 636f 6e3d 276d 6469 2d68 6f6d  ', icon='mdi-hom
-00005ad0: 6527 2c20 6d6f 6465 6c3d 4669 7273 745f  e', model=First_
-00005ae0: 6d6f 6465 6c29 0a63 6c61 7373 2046 6972  model).class Fir
-00005af0: 7374 5f62 6173 653a 0a20 2020 4064 6563  st_base:.   @dec
-00005b00: 6f72 652e 7669 6577 2874 6974 6c65 3d27  ore.view(title='
-00005b10: 4669 7273 7420 5669 6577 272c 2069 636f  First View', ico
-00005b20: 6e3d 276d 6469 2d68 6f6d 6527 2c20 7479  n='mdi-home', ty
-00005b30: 7065 3d27 7461 626c 6527 2c20 6669 656c  pe='table', fiel
-00005b40: 6473 3d5b 4669 7273 745f 6d6f 6465 6c2e  ds=[First_model.
-00005b50: 6669 7273 746e 616d 652c 2046 6972 7374  firstname, First
-00005b60: 5f6d 6f64 656c 2e6c 6173 746e 616d 655d  _model.lastname]
-00005b70: 290a 2020 2064 6566 2066 6972 7374 5f76  ).   def first_v
-00005b80: 6965 7728 293a 0a20 2020 2020 2070 6173  iew():.      pas
-00005b90: 7394 8594 8194 7d94 6816 6a0c 0600 0073  s.....}.h.j....s
-00005ba0: 6261 6817 7d94 2868 195d 9468 1b5d 9468  bah.}.(h.].h.].h
-00005bb0: 1d5d 9468 1f5d 9468 215d 9468 2368 246a  .].h.].h!].h#h$j
-00005bc0: 2702 0000 896a 2802 0000 8c06 7079 7468  '....j(.....pyth
-00005bd0: 6f6e 946a 2a02 0000 7d94 7568 256a 1702  on.j*...}.uh%j..
-00005be0: 0000 6827 6850 6829 4b84 6816 6aad 0500  ..h'hPh)K.h.j...
-00005bf0: 0068 2668 0375 6265 6817 7d94 2868 195d  .h&h.ubeh.}.(h.]
-00005c00: 948c 0476 6965 7794 6168 1b5d 9468 1d5d  ...view.ah.].h.]
-00005c10: 948c 0476 6965 7794 6168 1f5d 9468 215d  ...view.ah.].h!]
-00005c20: 9475 6825 682a 6816 6a21 0300 0068 2668  .uh%h*h.j!...h&h
-00005c30: 0368 2768 5068 294b 7d75 6268 2b29 8194  .h'hPh)K}ubh+)..
-00005c40: 7d94 2868 0568 0668 075d 9428 6830 2981  }.(h.h.h.].(h0).
-00005c50: 947d 9428 6805 8c06 4469 616c 6f67 9468  .}.(h...Dialog.h
-00005c60: 075d 9468 118c 0644 6961 6c6f 6794 8594  .].h...Dialog...
-00005c70: 8194 7d94 2868 166a 2706 0000 6826 6803  ..}.(h.j'...h&h.
-00005c80: 6827 4e68 294e 7562 6168 177d 9428 6819  h'Nh)Nubah.}.(h.
-00005c90: 5d94 681b 5d94 681d 5d94 681f 5d94 6821  ].h.].h.].h.].h!
-00005ca0: 5d94 7568 2568 2f68 166a 2406 0000 6826  ].uh%h/h.j$...h&
-00005cb0: 6803 6827 6850 6829 4b90 7562 6852 2981  h.h'hPh)K.ubhR).
-00005cc0: 947d 9428 6805 8cfb 4469 616c 6f67 7320  .}.(h...Dialogs 
-00005cd0: 6172 6520 7468 6520 7375 7070 6f72 7469  are the supporti
-00005ce0: 6e67 2065 6c65 6d65 6e74 7320 666f 7220  ng elements for 
-00005cf0: 7769 6467 6574 7320 696e 2074 6865 202a  widgets in the *
-00005d00: 2a64 6563 6f72 6520 4672 6f6e 742a 2a20  *decore Front** 
-00005d10: 7765 6220 6170 706c 6963 6174 696f 6e2e  web application.
-00005d20: 2054 6865 7920 6361 6e20 6f6e 6c79 2062   They can only b
-00005d30: 6520 6164 6465 6420 746f 2076 6965 7773  e added to views
-00005d40: 2061 6e64 2063 6f6e 7472 6f6c 2074 6865   and control the
-00005d50: 2076 6973 6962 696c 6974 7920 616e 6420   visibility and 
-00005d60: 6469 7370 6c61 7920 7374 796c 6520 6f66  display style of
-00005d70: 2063 6869 6c64 2065 6c65 6d65 6e74 732e   child elements.
-00005d80: 2044 6961 6c6f 6773 2061 6c73 6f20 6765   Dialogs also ge
-00005d90: 7420 636f 6e74 726f 6c20 6f76 6572 2074  t control over t
-00005da0: 6865 2073 7562 6d69 7420 6675 6e63 7469  he submit functi
-00005db0: 6f6e 7320 6f66 2074 6865 2077 6964 6765  ons of the widge
-00005dc0: 7473 2e94 6807 5d94 2868 118c 3744 6961  ts..h.].(h..7Dia
-00005dd0: 6c6f 6773 2061 7265 2074 6865 2073 7570  logs are the sup
-00005de0: 706f 7274 696e 6720 656c 656d 656e 7473  porting elements
-00005df0: 2066 6f72 2077 6964 6765 7473 2069 6e20   for widgets in 
-00005e00: 7468 6520 9485 9481 947d 9428 6816 6a35  the .....}.(h.j5
-00005e10: 0600 0068 2668 0368 274e 6829 4e75 6268  ...h&h.h'Nh)Nubh
-00005e20: 6629 8194 7d94 2868 058c 102a 2a64 6563  f)..}.(h...**dec
-00005e30: 6f72 6520 4672 6f6e 742a 2a94 6807 5d94  ore Front**.h.].
-00005e40: 6811 8c0c 6465 636f 7265 2046 726f 6e74  h...decore Front
-00005e50: 9485 9481 947d 9428 6816 6a3d 0600 0068  .....}.(h.j=...h
-00005e60: 2668 0368 274e 6829 4e75 6261 6817 7d94  &h.h'Nh)Nubah.}.
-00005e70: 2868 195d 9468 1b5d 9468 1d5d 9468 1f5d  (h.].h.].h.].h.]
-00005e80: 9468 215d 9475 6825 6865 6816 6a35 0600  .h!].uh%heh.j5..
-00005e90: 0075 6268 118c b420 7765 6220 6170 706c  .ubh... web appl
-00005ea0: 6963 6174 696f 6e2e 2054 6865 7920 6361  ication. They ca
-00005eb0: 6e20 6f6e 6c79 2062 6520 6164 6465 6420  n only be added 
-00005ec0: 746f 2076 6965 7773 2061 6e64 2063 6f6e  to views and con
-00005ed0: 7472 6f6c 2074 6865 2076 6973 6962 696c  trol the visibil
-00005ee0: 6974 7920 616e 6420 6469 7370 6c61 7920  ity and display 
-00005ef0: 7374 796c 6520 6f66 2063 6869 6c64 2065  style of child e
-00005f00: 6c65 6d65 6e74 732e 2044 6961 6c6f 6773  lements. Dialogs
-00005f10: 2061 6c73 6f20 6765 7420 636f 6e74 726f   also get contro
-00005f20: 6c20 6f76 6572 2074 6865 2073 7562 6d69  l over the submi
-00005f30: 7420 6675 6e63 7469 6f6e 7320 6f66 2074  t functions of t
-00005f40: 6865 2077 6964 6765 7473 2e94 8594 8194  he widgets......
-00005f50: 7d94 2868 166a 3506 0000 6826 6803 6827  }.(h.j5...h&h.h'
-00005f60: 4e68 294e 7562 6568 177d 9428 6819 5d94  Nh)Nubeh.}.(h.].
-00005f70: 681b 5d94 681d 5d94 681f 5d94 6821 5d94  h.].h.].h.].h!].
-00005f80: 7568 2568 5168 2768 5068 294b 9168 166a  uh%hQh'hPh)K.h.j
-00005f90: 2406 0000 6826 6803 7562 6852 2981 947d  $...h&h.ubhR)..}
-00005fa0: 9428 6805 8c55 496e 206f 7572 2063 6173  .(h..UIn our cas
-00005fb0: 652c 2077 6520 6372 6561 7465 2061 2064  e, we create a d
-00005fc0: 6961 6f6c 6720 746f 2063 7265 6174 6520  iaolg to create 
-00005fd0: 6120 6e65 7720 7065 7273 6f6e 2077 6974  a new person wit
-00005fe0: 6820 6669 7273 7420 6e61 6d65 2061 6e64  h first name and
-00005ff0: 206c 6173 7420 6e61 6d65 2e94 6807 5d94   last name..h.].
-00006000: 6811 8c55 496e 206f 7572 2063 6173 652c  h..UIn our case,
-00006010: 2077 6520 6372 6561 7465 2061 2064 6961   we create a dia
-00006020: 6f6c 6720 746f 2063 7265 6174 6520 6120  olg to create a 
-00006030: 6e65 7720 7065 7273 6f6e 2077 6974 6820  new person with 
-00006040: 6669 7273 7420 6e61 6d65 2061 6e64 206c  first name and l
-00006050: 6173 7420 6e61 6d65 2e94 8594 8194 7d94  ast name......}.
-00006060: 2868 166a 5506 0000 6826 6803 6827 4e68  (h.jU...h&h.h'Nh
-00006070: 294e 7562 6168 177d 9428 6819 5d94 681b  )Nubah.}.(h.].h.
-00006080: 5d94 681d 5d94 681f 5d94 6821 5d94 7568  ].h.].h.].h!].uh
-00006090: 2568 5168 2768 5068 294b 9368 166a 2406  %hQh'hPh)K.h.j$.
-000060a0: 0000 6826 6803 7562 6852 2981 947d 9428  ..h&h.ubhR)..}.(
-000060b0: 6805 8c4f 4865 7265 2077 6520 676f 202e  h..OHere we go .
-000060c0: 2e2e 2061 6761 696e 2074 6865 2066 696c  .. again the fil
-000060d0: 6520 2a2a 6669 7273 745f 6261 7365 2e70  e **first_base.p
-000060e0: 792a 2a20 616e 6420 6578 7465 6e64 2074  y** and extend t
-000060f0: 6865 2063 6f64 6520 6173 2066 6f6c 6c6f  he code as follo
-00006100: 7773 3a94 6807 5d94 2868 118c 1e48 6572  ws:.h.].(h...Her
-00006110: 6520 7765 2067 6f20 e280 a620 6167 6169  e we go ... agai
-00006120: 6e20 7468 6520 6669 6c65 2094 8594 8194  n the file .....
-00006130: 7d94 2868 166a 6306 0000 6826 6803 6827  }.(h.jc...h&h.h'
-00006140: 4e68 294e 7562 6866 2981 947d 9428 6805  Nh)Nubhf)..}.(h.
-00006150: 8c11 2a2a 6669 7273 745f 6261 7365 2e70  ..**first_base.p
-00006160: 792a 2a94 6807 5d94 6811 8c0d 6669 7273  y**.h.].h...firs
-00006170: 745f 6261 7365 2e70 7994 8594 8194 7d94  t_base.py.....}.
-00006180: 2868 166a 6b06 0000 6826 6803 6827 4e68  (h.jk...h&h.h'Nh
-00006190: 294e 7562 6168 177d 9428 6819 5d94 681b  )Nubah.}.(h.].h.
-000061a0: 5d94 681d 5d94 681f 5d94 6821 5d94 7568  ].h.].h.].h!].uh
-000061b0: 2568 6568 166a 6306 0000 7562 6811 8c20  %heh.jc...ubh.. 
-000061c0: 2061 6e64 2065 7874 656e 6420 7468 6520   and extend the 
-000061d0: 636f 6465 2061 7320 666f 6c6c 6f77 733a  code as follows:
-000061e0: 9485 9481 947d 9428 6816 6a63 0600 0068  .....}.(h.jc...h
-000061f0: 2668 0368 274e 6829 4e75 6265 6817 7d94  &h.h'Nh)Nubeh.}.
-00006200: 2868 195d 9468 1b5d 9468 1d5d 9468 1f5d  (h.].h.].h.].h.]
-00006210: 9468 215d 9475 6825 6851 6827 6850 6829  .h!].uh%hQh'hPh)
-00006220: 4b95 6816 6a24 0600 0068 2668 0375 626a  K.h.j$...h&h.ubj
-00006230: 1802 0000 2981 947d 9428 6805 58d0 0100  ....)..}.(h.X...
-00006240: 0066 726f 6d20 6465 636f 7265 5f62 6173  .from decore_bas
-00006250: 6520 696d 706f 7274 2064 6563 6f72 650a  e import decore.
-00006260: 6672 6f6d 206d 6f64 656c 732e 6669 7273  from models.firs
-00006270: 745f 6d6f 6465 6c20 696d 706f 7274 2046  t_model import F
-00006280: 6972 7374 5f6d 6f64 656c 0a0a 4064 6563  irst_model..@dec
-00006290: 6f72 652e 6261 7365 2874 6974 6c65 3d27  ore.base(title='
-000062a0: 4d79 2046 6972 7374 2042 6173 6527 2c20  My First Base', 
-000062b0: 6963 6f6e 3d27 6d64 692d 686f 6d65 272c  icon='mdi-home',
-000062c0: 206d 6f64 656c 3d46 6972 7374 5f6d 6f64   model=First_mod
-000062d0: 656c 290a 636c 6173 7320 4669 7273 745f  el).class First_
-000062e0: 6261 7365 3a0a 2020 2040 6465 636f 7265  base:.   @decore
-000062f0: 2e76 6965 7728 7469 746c 653d 2750 6572  .view(title='Per
-00006300: 736f 6e27 2c20 6963 6f6e 3d27 6d64 692d  son', icon='mdi-
-00006310: 6163 636f 756e 7427 2c20 7479 7065 3d27  account', type='
-00006320: 7461 626c 6527 2c20 6669 656c 6473 3d5b  table', fields=[
-00006330: 4669 7273 745f 6d6f 6465 6c2e 6669 7273  First_model.firs
-00006340: 746e 616d 652c 2046 6972 7374 5f6d 6f64  tname, First_mod
-00006350: 656c 2e6c 6173 746e 616d 655d 290a 2020  el.lastname]).  
-00006360: 2064 6566 2066 6972 7374 5f76 6965 7728   def first_view(
-00006370: 293a 0a20 2020 2020 2040 6465 636f 7265  ):.      @decore
-00006380: 2e64 6961 6c6f 6728 7469 746c 653d 2741  .dialog(title='A
-00006390: 6464 2050 6572 736f 6e27 2c20 6963 6f6e  dd Person', icon
-000063a0: 3d27 6d64 692d 706c 7573 272c 2074 7970  ='mdi-plus', typ
-000063b0: 653d 2773 7461 6e64 6172 6427 2c20 6469  e='standard', di
-000063c0: 7370 6c61 793d 2764 7261 7765 7227 2c20  splay='drawer', 
-000063d0: 6163 7469 7661 746f 723d 2764 6566 6175  activator='defau
-000063e0: 6c74 2d6d 656e 7527 290a 2020 2020 2020  lt-menu').      
-000063f0: 6465 6620 6669 7273 745f 6469 616c 6f67  def first_dialog
-00006400: 2829 3a0a 2020 2020 2020 2020 2070 6173  ():.         pas
-00006410: 7394 6807 5d94 6811 58d0 0100 0066 726f  s.h.].h.X....fro
-00006420: 6d20 6465 636f 7265 5f62 6173 6520 696d  m decore_base im
-00006430: 706f 7274 2064 6563 6f72 650a 6672 6f6d  port decore.from
-00006440: 206d 6f64 656c 732e 6669 7273 745f 6d6f   models.first_mo
-00006450: 6465 6c20 696d 706f 7274 2046 6972 7374  del import First
-00006460: 5f6d 6f64 656c 0a0a 4064 6563 6f72 652e  _model..@decore.
-00006470: 6261 7365 2874 6974 6c65 3d27 4d79 2046  base(title='My F
-00006480: 6972 7374 2042 6173 6527 2c20 6963 6f6e  irst Base', icon
-00006490: 3d27 6d64 692d 686f 6d65 272c 206d 6f64  ='mdi-home', mod
-000064a0: 656c 3d46 6972 7374 5f6d 6f64 656c 290a  el=First_model).
-000064b0: 636c 6173 7320 4669 7273 745f 6261 7365  class First_base
-000064c0: 3a0a 2020 2040 6465 636f 7265 2e76 6965  :.   @decore.vie
-000064d0: 7728 7469 746c 653d 2750 6572 736f 6e27  w(title='Person'
-000064e0: 2c20 6963 6f6e 3d27 6d64 692d 6163 636f  , icon='mdi-acco
-000064f0: 756e 7427 2c20 7479 7065 3d27 7461 626c  unt', type='tabl
-00006500: 6527 2c20 6669 656c 6473 3d5b 4669 7273  e', fields=[Firs
-00006510: 745f 6d6f 6465 6c2e 6669 7273 746e 616d  t_model.firstnam
-00006520: 652c 2046 6972 7374 5f6d 6f64 656c 2e6c  e, First_model.l
-00006530: 6173 746e 616d 655d 290a 2020 2064 6566  astname]).   def
-00006540: 2066 6972 7374 5f76 6965 7728 293a 0a20   first_view():. 
-00006550: 2020 2020 2040 6465 636f 7265 2e64 6961       @decore.dia
-00006560: 6c6f 6728 7469 746c 653d 2741 6464 2050  log(title='Add P
-00006570: 6572 736f 6e27 2c20 6963 6f6e 3d27 6d64  erson', icon='md
-00006580: 692d 706c 7573 272c 2074 7970 653d 2773  i-plus', type='s
-00006590: 7461 6e64 6172 6427 2c20 6469 7370 6c61  tandard', displa
-000065a0: 793d 2764 7261 7765 7227 2c20 6163 7469  y='drawer', acti
-000065b0: 7661 746f 723d 2764 6566 6175 6c74 2d6d  vator='default-m
-000065c0: 656e 7527 290a 2020 2020 2020 6465 6620  enu').      def 
-000065d0: 6669 7273 745f 6469 616c 6f67 2829 3a0a  first_dialog():.
-000065e0: 2020 2020 2020 2020 2070 6173 7394 8594           pass...
-000065f0: 8194 7d94 6816 6a83 0600 0073 6261 6817  ..}.h.j....sbah.
-00006600: 7d94 2868 195d 9468 1b5d 9468 1d5d 9468  }.(h.].h.].h.].h
-00006610: 1f5d 9468 215d 9468 2368 246a 2702 0000  .].h!].h#h$j'...
-00006620: 896a 2802 0000 8c06 7079 7468 6f6e 946a  .j(.....python.j
-00006630: 2a02 0000 7d94 7568 256a 1702 0000 6827  *...}.uh%j....h'
-00006640: 6850 6829 4b97 6816 6a24 0600 0068 2668  hPh)K.h.j$...h&h
-00006650: 0375 6265 6817 7d94 2868 195d 948c 0664  .ubeh.}.(h.]...d
-00006660: 6961 6c6f 6794 6168 1b5d 9468 1d5d 948c  ialog.ah.].h.]..
-00006670: 0664 6961 6c6f 6794 6168 1f5d 9468 215d  .dialog.ah.].h!]
-00006680: 9475 6825 682a 6816 6a21 0300 0068 2668  .uh%h*h.j!...h&h
-00006690: 0368 2768 5068 294b 9075 6268 2b29 8194  .h'hPh)K.ubh+)..
-000066a0: 7d94 2868 0568 0668 075d 9428 6830 2981  }.(h.h.h.].(h0).
-000066b0: 947d 9428 6805 8c06 5769 6467 6574 9468  .}.(h...Widget.h
-000066c0: 075d 9468 118c 0657 6964 6765 7494 8594  .].h...Widget...
-000066d0: 8194 7d94 2868 166a 9e06 0000 6826 6803  ..}.(h.j....h&h.
-000066e0: 6827 4e68 294e 7562 6168 177d 9428 6819  h'Nh)Nubah.}.(h.
-000066f0: 5d94 681b 5d94 681d 5d94 681f 5d94 6821  ].h.].h.].h.].h!
-00006700: 5d94 7568 2568 2f68 166a 9b06 0000 6826  ].uh%h/h.j....h&
-00006710: 6803 6827 6850 6829 4ba5 7562 6852 2981  h.h'hPh)K.ubhR).
-00006720: 947d 9428 6805 8c88 5769 6467 6574 7320  .}.(h...Widgets 
-00006730: 6172 6520 636f 6d70 6f6e 656e 7473 2077  are components w
-00006740: 6974 6820 7768 6963 6820 7765 2063 616e  ith which we can
-00006750: 2070 6572 666f 726d 2069 6e74 6572 6163   perform interac
-00006760: 7469 6f6e 7320 6f6e 2074 6865 2073 696e  tions on the sin
-00006770: 676c 6520 7265 636f 7264 2e20 5468 6579  gle record. They
-00006780: 2063 616e 206f 6e6c 7920 6265 2061 6464   can only be add
-00006790: 6564 2074 6f20 6469 616c 6f67 7320 616e  ed to dialogs an
-000067a0: 6420 6172 6520 7374 6163 6b61 626c 652e  d are stackable.
-000067b0: 9468 075d 9468 118c 8857 6964 6765 7473  .h.].h...Widgets
-000067c0: 2061 7265 2063 6f6d 706f 6e65 6e74 7320   are components 
-000067d0: 7769 7468 2077 6869 6368 2077 6520 6361  with which we ca
-000067e0: 6e20 7065 7266 6f72 6d20 696e 7465 7261  n perform intera
-000067f0: 6374 696f 6e73 206f 6e20 7468 6520 7369  ctions on the si
-00006800: 6e67 6c65 2072 6563 6f72 642e 2054 6865  ngle record. The
-00006810: 7920 6361 6e20 6f6e 6c79 2062 6520 6164  y can only be ad
-00006820: 6465 6420 746f 2064 6961 6c6f 6773 2061  ded to dialogs a
-00006830: 6e64 2061 7265 2073 7461 636b 6162 6c65  nd are stackable
-00006840: 2e94 8594 8194 7d94 2868 166a ac06 0000  ......}.(h.j....
-00006850: 6826 6803 6827 4e68 294e 7562 6168 177d  h&h.h'Nh)Nubah.}
-00006860: 9428 6819 5d94 681b 5d94 681d 5d94 681f  .(h.].h.].h.].h.
-00006870: 5d94 6821 5d94 7568 2568 5168 2768 5068  ].h!].uh%hQh'hPh
-00006880: 294b a668 166a 9b06 0000 6826 6803 7562  )K.h.j....h&h.ub
-00006890: 6852 2981 947d 9428 6805 8c51 5768 6174  hR)..}.(h..QWhat
-000068a0: 2077 6520 6e65 6564 206e 6f77 2069 7320   we need now is 
-000068b0: 746f 2063 7265 6174 6520 616e 2069 6e70  to create an inp
-000068c0: 7574 2066 6f72 6d20 746f 2065 6e74 6572  ut form to enter
-000068d0: 2074 6865 2064 6174 6120 666f 7220 7468   the data for th
-000068e0: 6520 6e65 7720 7065 7273 6f6e 2e94 6807  e new person..h.
-000068f0: 5d94 6811 8c51 5768 6174 2077 6520 6e65  ].h..QWhat we ne
-00006900: 6564 206e 6f77 2069 7320 746f 2063 7265  ed now is to cre
-00006910: 6174 6520 616e 2069 6e70 7574 2066 6f72  ate an input for
-00006920: 6d20 746f 2065 6e74 6572 2074 6865 2064  m to enter the d
-00006930: 6174 6120 666f 7220 7468 6520 6e65 7720  ata for the new 
-00006940: 7065 7273 6f6e 2e94 8594 8194 7d94 2868  person......}.(h
-00006950: 166a ba06 0000 6826 6803 6827 4e68 294e  .j....h&h.h'Nh)N
-00006960: 7562 6168 177d 9428 6819 5d94 681b 5d94  ubah.}.(h.].h.].
-00006970: 681d 5d94 681f 5d94 6821 5d94 7568 2568  h.].h.].h!].uh%h
-00006980: 5168 2768 5068 294b a868 166a 9b06 0000  Qh'hPh)K.h.j....
-00006990: 6826 6803 7562 6a18 0200 0029 8194 7d94  h&h.ubj....)..}.
-000069a0: 2868 0558 7802 0000 6672 6f6d 2064 6563  (h.Xx...from dec
-000069b0: 6f72 655f 6261 7365 2069 6d70 6f72 7420  ore_base import 
-000069c0: 6465 636f 7265 0a66 726f 6d20 6d6f 6465  decore.from mode
-000069d0: 6c73 2e66 6972 7374 5f6d 6f64 656c 2069  ls.first_model i
-000069e0: 6d70 6f72 7420 4669 7273 745f 6d6f 6465  mport First_mode
-000069f0: 6c0a 0a40 6465 636f 7265 2e62 6173 6528  l..@decore.base(
-00006a00: 7469 746c 653d 274d 7920 4669 7273 7420  title='My First 
-00006a10: 4261 7365 272c 2069 636f 6e3d 276d 6469  Base', icon='mdi
-00006a20: 2d68 6f6d 6527 2c20 6d6f 6465 6c3d 4669  -home', model=Fi
-00006a30: 7273 745f 6d6f 6465 6c29 0a63 6c61 7373  rst_model).class
-00006a40: 2046 6972 7374 5f62 6173 653a 0a20 2020   First_base:.   
-00006a50: 4064 6563 6f72 652e 7669 6577 2874 6974  @decore.view(tit
-00006a60: 6c65 3d27 5065 7273 6f6e 272c 2069 636f  le='Person', ico
-00006a70: 6e3d 276d 6469 2d61 6363 6f75 6e74 272c  n='mdi-account',
-00006a80: 2074 7970 653d 2774 6162 6c65 272c 2066   type='table', f
-00006a90: 6965 6c64 733d 5b46 6972 7374 5f6d 6f64  ields=[First_mod
-00006aa0: 656c 2e66 6972 7374 6e61 6d65 2c20 4669  el.firstname, Fi
-00006ab0: 7273 745f 6d6f 6465 6c2e 6c61 7374 6e61  rst_model.lastna
-00006ac0: 6d65 5d29 0a20 2020 6465 6620 6669 7273  me]).   def firs
-00006ad0: 745f 7669 6577 2829 3a0a 2020 2020 2020  t_view():.      
-00006ae0: 4064 6563 6f72 652e 6469 616c 6f67 2874  @decore.dialog(t
-00006af0: 6974 6c65 3d27 4164 6420 5065 7273 6f6e  itle='Add Person
-00006b00: 272c 2069 636f 6e3d 276d 6469 2d70 6c75  ', icon='mdi-plu
-00006b10: 7327 2c20 7479 7065 3d27 7374 616e 6461  s', type='standa
-00006b20: 7264 272c 2064 6973 706c 6179 3d27 6472  rd', display='dr
-00006b30: 6177 6572 272c 2061 6374 6976 6174 6f72  awer', activator
-00006b40: 3d27 6465 6661 756c 742d 6d65 6e75 2729  ='default-menu')
-00006b50: 0a20 2020 2020 2064 6566 2066 6972 7374  .      def first
-00006b60: 5f64 6961 6c6f 6728 293a 0a20 2020 2020  _dialog():.     
-00006b70: 2020 2020 4064 6563 6f72 652e 7769 6467      @decore.widg
-00006b80: 6574 2874 6974 6c65 3d27 4164 6420 5065  et(title='Add Pe
-00006b90: 7273 6f6e 2046 6f72 6d27 2c20 6963 6f6e  rson Form', icon
-00006ba0: 3d27 6d64 692d 6163 636f 756e 7427 2c20  ='mdi-account', 
-00006bb0: 7479 7065 3d27 666f 726d 272c 2066 6965  type='form', fie
-00006bc0: 6c64 733d 5b46 6972 7374 5f6d 6f64 656c  lds=[First_model
-00006bd0: 2e66 6972 7374 6e61 6d65 2c20 4669 7273  .firstname, Firs
-00006be0: 745f 6d6f 6465 6c2e 6c61 7374 6e61 6d65  t_model.lastname
-00006bf0: 5d29 0a20 2020 2020 2020 2020 6465 6620  ]).         def 
-00006c00: 6669 7273 745f 7769 6467 6574 2829 3a0a  first_widget():.
-00006c10: 2020 2020 2020 2020 2020 2020 7061 7373              pass
-00006c20: 9468 075d 9468 1158 7802 0000 6672 6f6d  .h.].h.Xx...from
-00006c30: 2064 6563 6f72 655f 6261 7365 2069 6d70   decore_base imp
-00006c40: 6f72 7420 6465 636f 7265 0a66 726f 6d20  ort decore.from 
-00006c50: 6d6f 6465 6c73 2e66 6972 7374 5f6d 6f64  models.first_mod
-00006c60: 656c 2069 6d70 6f72 7420 4669 7273 745f  el import First_
-00006c70: 6d6f 6465 6c0a 0a40 6465 636f 7265 2e62  model..@decore.b
-00006c80: 6173 6528 7469 746c 653d 274d 7920 4669  ase(title='My Fi
-00006c90: 7273 7420 4261 7365 272c 2069 636f 6e3d  rst Base', icon=
-00006ca0: 276d 6469 2d68 6f6d 6527 2c20 6d6f 6465  'mdi-home', mode
-00006cb0: 6c3d 4669 7273 745f 6d6f 6465 6c29 0a63  l=First_model).c
-00006cc0: 6c61 7373 2046 6972 7374 5f62 6173 653a  lass First_base:
-00006cd0: 0a20 2020 4064 6563 6f72 652e 7669 6577  .   @decore.view
-00006ce0: 2874 6974 6c65 3d27 5065 7273 6f6e 272c  (title='Person',
-00006cf0: 2069 636f 6e3d 276d 6469 2d61 6363 6f75   icon='mdi-accou
-00006d00: 6e74 272c 2074 7970 653d 2774 6162 6c65  nt', type='table
-00006d10: 272c 2066 6965 6c64 733d 5b46 6972 7374  ', fields=[First
-00006d20: 5f6d 6f64 656c 2e66 6972 7374 6e61 6d65  _model.firstname
-00006d30: 2c20 4669 7273 745f 6d6f 6465 6c2e 6c61  , First_model.la
-00006d40: 7374 6e61 6d65 5d29 0a20 2020 6465 6620  stname]).   def 
-00006d50: 6669 7273 745f 7669 6577 2829 3a0a 2020  first_view():.  
-00006d60: 2020 2020 4064 6563 6f72 652e 6469 616c      @decore.dial
-00006d70: 6f67 2874 6974 6c65 3d27 4164 6420 5065  og(title='Add Pe
-00006d80: 7273 6f6e 272c 2069 636f 6e3d 276d 6469  rson', icon='mdi
-00006d90: 2d70 6c75 7327 2c20 7479 7065 3d27 7374  -plus', type='st
-00006da0: 616e 6461 7264 272c 2064 6973 706c 6179  andard', display
-00006db0: 3d27 6472 6177 6572 272c 2061 6374 6976  ='drawer', activ
-00006dc0: 6174 6f72 3d27 6465 6661 756c 742d 6d65  ator='default-me
-00006dd0: 6e75 2729 0a20 2020 2020 2064 6566 2066  nu').      def f
-00006de0: 6972 7374 5f64 6961 6c6f 6728 293a 0a20  irst_dialog():. 
-00006df0: 2020 2020 2020 2020 4064 6563 6f72 652e          @decore.
-00006e00: 7769 6467 6574 2874 6974 6c65 3d27 4164  widget(title='Ad
-00006e10: 6420 5065 7273 6f6e 2046 6f72 6d27 2c20  d Person Form', 
-00006e20: 6963 6f6e 3d27 6d64 692d 6163 636f 756e  icon='mdi-accoun
-00006e30: 7427 2c20 7479 7065 3d27 666f 726d 272c  t', type='form',
-00006e40: 2066 6965 6c64 733d 5b46 6972 7374 5f6d   fields=[First_m
-00006e50: 6f64 656c 2e66 6972 7374 6e61 6d65 2c20  odel.firstname, 
-00006e60: 4669 7273 745f 6d6f 6465 6c2e 6c61 7374  First_model.last
-00006e70: 6e61 6d65 5d29 0a20 2020 2020 2020 2020  name]).         
-00006e80: 6465 6620 6669 7273 745f 7769 6467 6574  def first_widget
-00006e90: 2829 3a0a 2020 2020 2020 2020 2020 2020  ():.            
-00006ea0: 7061 7373 9485 9481 947d 9468 166a c806  pass.....}.h.j..
-00006eb0: 0000 7362 6168 177d 9428 6819 5d94 681b  ..sbah.}.(h.].h.
-00006ec0: 5d94 681d 5d94 681f 5d94 6821 5d94 6823  ].h.].h.].h!].h#
-00006ed0: 6824 6a27 0200 0089 6a28 0200 008c 0670  h$j'....j(.....p
-00006ee0: 7974 686f 6e94 6a2a 0200 007d 9475 6825  ython.j*...}.uh%
-00006ef0: 6a17 0200 0068 2768 5068 294b aa68 166a  j....h'hPh)K.h.j
-00006f00: 9b06 0000 6826 6803 7562 6568 177d 9428  ....h&h.ubeh.}.(
-00006f10: 6819 5d94 8c06 7769 6467 6574 9461 681b  h.]...widget.ah.
-00006f20: 5d94 681d 5d94 8c06 7769 6467 6574 9461  ].h.]...widget.a
-00006f30: 681f 5d94 6821 5d94 7568 2568 2a68 166a  h.].h!].uh%h*h.j
-00006f40: 2103 0000 6826 6803 6827 6850 6829 4ba5  !...h&h.h'hPh)K.
-00006f50: 7562 682b 2981 947d 9428 6805 6806 6807  ubh+)..}.(h.h.h.
-00006f60: 5d94 2868 3029 8194 7d94 2868 058c 0641  ].(h0)..}.(h...A
-00006f70: 6374 696f 6e94 6807 5d94 6811 8c06 4163  ction.h.].h...Ac
-00006f80: 7469 6f6e 9485 9481 947d 9428 6816 6ae3  tion.....}.(h.j.
-00006f90: 0600 0068 2668 0368 274e 6829 4e75 6261  ...h&h.h'Nh)Nuba
-00006fa0: 6817 7d94 2868 195d 9468 1b5d 9468 1d5d  h.}.(h.].h.].h.]
-00006fb0: 9468 1f5d 9468 215d 9475 6825 682f 6816  .h.].h!].uh%h/h.
-00006fc0: 6ae0 0600 0068 2668 0368 2768 5068 294b  j....h&h.h'hPh)K
-00006fd0: ba75 6268 5229 8194 7d94 2868 058c b141  .ubhR)..}.(h...A
-00006fe0: 6374 696f 6e73 2061 7265 206d 6574 686f  ctions are metho
-00006ff0: 6473 2077 6974 6820 7768 6963 6820 2a2a  ds with which **
-00007000: 6465 636f 7265 2046 726f 6e74 2a2a 2063  decore Front** c
-00007010: 616e 2063 6f6d 6d75 6e69 6361 7465 2077  an communicate w
-00007020: 6974 6820 2a2a 6465 636f 7265 2042 6173  ith **decore Bas
-00007030: 652a 2a2e 2054 6865 7920 6361 6e20 6265  e**. They can be
-00007040: 2061 6464 6564 2074 6f20 7669 6577 7320   added to views 
-00007050: 616e 6420 7769 6467 6574 7320 616e 6420  and widgets and 
-00007060: 6172 6520 7468 6520 6f6e 6c79 2072 6561  are the only rea
-00007070: 6c20 636c 6173 7320 6d65 7468 6f64 7320  l class methods 
-00007080: 696e 2074 6865 206d 6574 6120 6b69 742e  in the meta kit.
-00007090: 9468 075d 9428 6811 8c1f 4163 7469 6f6e  .h.].(h...Action
-000070a0: 7320 6172 6520 6d65 7468 6f64 7320 7769  s are methods wi
-000070b0: 7468 2077 6869 6368 2094 8594 8194 7d94  th which .....}.
-000070c0: 2868 166a f106 0000 6826 6803 6827 4e68  (h.j....h&h.h'Nh
-000070d0: 294e 7562 6866 2981 947d 9428 6805 8c10  )Nubhf)..}.(h...
-000070e0: 2a2a 6465 636f 7265 2046 726f 6e74 2a2a  **decore Front**
-000070f0: 9468 075d 9468 118c 0c64 6563 6f72 6520  .h.].h...decore 
-00007100: 4672 6f6e 7494 8594 8194 7d94 2868 166a  Front.....}.(h.j
-00007110: f906 0000 6826 6803 6827 4e68 294e 7562  ....h&h.h'Nh)Nub
-00007120: 6168 177d 9428 6819 5d94 681b 5d94 681d  ah.}.(h.].h.].h.
-00007130: 5d94 681f 5d94 6821 5d94 7568 2568 6568  ].h.].h!].uh%heh
-00007140: 166a f106 0000 7562 6811 8c16 2063 616e  .j....ubh... can
-00007150: 2063 6f6d 6d75 6e69 6361 7465 2077 6974   communicate wit
-00007160: 6820 9485 9481 947d 9428 6816 6af1 0600  h .....}.(h.j...
-00007170: 0068 2668 0368 274e 6829 4e75 6268 6629  .h&h.h'Nh)Nubhf)
-00007180: 8194 7d94 2868 058c 0f2a 2a64 6563 6f72  ..}.(h...**decor
-00007190: 6520 4261 7365 2a2a 9468 075d 9468 118c  e Base**.h.].h..
-000071a0: 0b64 6563 6f72 6520 4261 7365 9485 9481  .decore Base....
-000071b0: 947d 9428 6816 6a0b 0700 0068 2668 0368  .}.(h.j....h&h.h
-000071c0: 274e 6829 4e75 6261 6817 7d94 2868 195d  'Nh)Nubah.}.(h.]
-000071d0: 9468 1b5d 9468 1d5d 9468 1f5d 9468 215d  .h.].h.].h.].h!]
-000071e0: 9475 6825 6865 6816 6af1 0600 0075 6268  .uh%heh.j....ubh
-000071f0: 118c 5d2e 2054 6865 7920 6361 6e20 6265  ..]. They can be
-00007200: 2061 6464 6564 2074 6f20 7669 6577 7320   added to views 
-00007210: 616e 6420 7769 6467 6574 7320 616e 6420  and widgets and 
-00007220: 6172 6520 7468 6520 6f6e 6c79 2072 6561  are the only rea
-00007230: 6c20 636c 6173 7320 6d65 7468 6f64 7320  l class methods 
-00007240: 696e 2074 6865 206d 6574 6120 6b69 742e  in the meta kit.
-00007250: 9485 9481 947d 9428 6816 6af1 0600 0068  .....}.(h.j....h
-00007260: 2668 0368 274e 6829 4e75 6265 6817 7d94  &h.h'Nh)Nubeh.}.
-00007270: 2868 195d 9468 1b5d 9468 1d5d 9468 1f5d  (h.].h.].h.].h.]
-00007280: 9468 215d 9475 6825 6851 6827 6850 6829  .h!].uh%hQh'hPh)
-00007290: 4bbb 6816 6ae0 0600 0068 2668 0375 6268  K.h.j....h&h.ubh
-000072a0: 5229 8194 7d94 2868 058c 6e57 6520 6e6f  R)..}.(h..nWe no
-000072b0: 7720 6e65 6564 2061 6e20 6163 7469 6f6e  w need an action
-000072c0: 2074 6f20 7374 6f72 6520 7468 6520 6461   to store the da
-000072d0: 7461 206f 6620 7468 6520 6e65 7720 7065  ta of the new pe
-000072e0: 7273 6f6e 2061 6e64 2065 7874 656e 6420  rson and extend 
-000072f0: 7468 6520 636f 6465 2069 6e20 2a2a 6669  the code in **fi
-00007300: 7273 745f 6261 7365 2e70 792a 2a20 6173  rst_base.py** as
-00007310: 2066 6f6c 6c6f 7773 3a94 6807 5d94 2868   follows:.h.].(h
-00007320: 118c 5157 6520 6e6f 7720 6e65 6564 2061  ..QWe now need a
-00007330: 6e20 6163 7469 6f6e 2074 6f20 7374 6f72  n action to stor
-00007340: 6520 7468 6520 6461 7461 206f 6620 7468  e the data of th
-00007350: 6520 6e65 7720 7065 7273 6f6e 2061 6e64  e new person and
-00007360: 2065 7874 656e 6420 7468 6520 636f 6465   extend the code
-00007370: 2069 6e20 9485 9481 947d 9428 6816 6a23   in .....}.(h.j#
-00007380: 0700 0068 2668 0368 274e 6829 4e75 6268  ...h&h.h'Nh)Nubh
-00007390: 6629 8194 7d94 2868 058c 112a 2a66 6972  f)..}.(h...**fir
-000073a0: 7374 5f62 6173 652e 7079 2a2a 9468 075d  st_base.py**.h.]
-000073b0: 9468 118c 0d66 6972 7374 5f62 6173 652e  .h...first_base.
-000073c0: 7079 9485 9481 947d 9428 6816 6a2b 0700  py.....}.(h.j+..
-000073d0: 0068 2668 0368 274e 6829 4e75 6261 6817  .h&h.h'Nh)Nubah.
-000073e0: 7d94 2868 195d 9468 1b5d 9468 1d5d 9468  }.(h.].h.].h.].h
-000073f0: 1f5d 9468 215d 9475 6825 6865 6816 6a23  .].h!].uh%heh.j#
-00007400: 0700 0075 6268 118c 0c20 6173 2066 6f6c  ...ubh... as fol
-00007410: 6c6f 7773 3a94 8594 8194 7d94 2868 166a  lows:.....}.(h.j
-00007420: 2307 0000 6826 6803 6827 4e68 294e 7562  #...h&h.h'Nh)Nub
-00007430: 6568 177d 9428 6819 5d94 681b 5d94 681d  eh.}.(h.].h.].h.
-00007440: 5d94 681f 5d94 6821 5d94 7568 2568 5168  ].h.].h!].uh%hQh
-00007450: 2768 5068 294b bd68 166a e006 0000 6826  'hPh)K.h.j....h&
-00007460: 6803 7562 6a18 0200 0029 8194 7d94 2868  h.ubj....)..}.(h
-00007470: 0558 5704 0000 6672 6f6d 2064 6563 6f72  .XW...from decor
-00007480: 655f 6261 7365 2069 6d70 6f72 7420 6465  e_base import de
-00007490: 636f 7265 0a66 726f 6d20 6d6f 6465 6c73  core.from models
-000074a0: 2e66 6972 7374 5f6d 6f64 656c 2069 6d70  .first_model imp
-000074b0: 6f72 7420 4669 7273 745f 6d6f 6465 6c0a  ort First_model.
-000074c0: 0a40 6465 636f 7265 2e62 6173 6528 7469  .@decore.base(ti
-000074d0: 746c 653d 274d 7920 4669 7273 7420 4261  tle='My First Ba
-000074e0: 7365 272c 2069 636f 6e3d 276d 6469 2d68  se', icon='mdi-h
-000074f0: 6f6d 6527 2c20 6d6f 6465 6c3d 4669 7273  ome', model=Firs
-00007500: 745f 6d6f 6465 6c29 0a63 6c61 7373 2046  t_model).class F
-00007510: 6972 7374 5f62 6173 653a 0a20 2020 4064  irst_base:.   @d
-00007520: 6563 6f72 652e 7669 6577 2874 6974 6c65  ecore.view(title
-00007530: 3d27 5065 7273 6f6e 272c 2069 636f 6e3d  ='Person', icon=
-00007540: 276d 6469 2d61 6363 6f75 6e74 272c 2074  'mdi-account', t
-00007550: 7970 653d 2774 6162 6c65 272c 2066 6965  ype='table', fie
-00007560: 6c64 733d 5b46 6972 7374 5f6d 6f64 656c  lds=[First_model
-00007570: 2e66 6972 7374 6e61 6d65 2c20 4669 7273  .firstname, Firs
-00007580: 745f 6d6f 6465 6c2e 6c61 7374 6e61 6d65  t_model.lastname
-00007590: 5d29 0a20 2020 6465 6620 6669 7273 745f  ]).   def first_
-000075a0: 7669 6577 2829 3a0a 2020 2020 2020 4064  view():.      @d
-000075b0: 6563 6f72 652e 6469 616c 6f67 2874 6974  ecore.dialog(tit
-000075c0: 6c65 3d27 4164 6420 5065 7273 6f6e 272c  le='Add Person',
-000075d0: 2069 636f 6e3d 276d 6469 2d70 6c75 7327   icon='mdi-plus'
-000075e0: 2c20 7479 7065 3d27 7374 616e 6461 7264  , type='standard
-000075f0: 272c 2064 6973 706c 6179 3d27 6472 6177  ', display='draw
-00007600: 6572 272c 2061 6374 6976 6174 6f72 3d27  er', activator='
-00007610: 6465 6661 756c 742d 6d65 6e75 2729 0a20  default-menu'). 
-00007620: 2020 2020 2064 6566 2066 6972 7374 5f64       def first_d
-00007630: 6961 6c6f 6728 293a 0a20 2020 2020 2020  ialog():.       
-00007640: 2020 4064 6563 6f72 652e 7769 6467 6574    @decore.widget
-00007650: 2874 6974 6c65 3d27 4164 6420 5065 7273  (title='Add Pers
-00007660: 6f6e 2046 6f72 6d27 2c20 6963 6f6e 3d27  on Form', icon='
-00007670: 6d64 692d 6163 636f 756e 7427 2c20 7479  mdi-account', ty
-00007680: 7065 3d27 666f 726d 272c 2066 6965 6c64  pe='form', field
-00007690: 733d 5b46 6972 7374 5f6d 6f64 656c 2e66  s=[First_model.f
-000076a0: 6972 7374 6e61 6d65 2c20 4669 7273 745f  irstname, First_
-000076b0: 6d6f 6465 6c2e 6c61 7374 6e61 6d65 5d29  model.lastname])
-000076c0: 0a20 2020 2020 2020 2020 6465 6620 6669  .         def fi
-000076d0: 7273 745f 7769 6467 6574 2829 3a0a 2020  rst_widget():.  
-000076e0: 2020 2020 2020 2020 2020 4064 6563 6f72            @decor
-000076f0: 652e 6163 7469 6f6e 2874 6974 6c65 3d27  e.action(title='
-00007700: 5361 7665 2050 6572 736f 6e27 2c20 6963  Save Person', ic
-00007710: 6f6e 3d27 6d64 692d 636f 6e74 656e 742d  on='mdi-content-
-00007720: 7361 7665 272c 2074 7970 653d 2773 7562  save', type='sub
-00007730: 6d69 7427 290a 2020 2020 2020 2020 2020  mit').          
-00007740: 2020 6465 6620 6669 7273 745f 6163 7469    def first_acti
-00007750: 6f6e 2873 656c 662c 2064 6174 6129 3a0a  on(self, data):.
-00007760: 2020 2020 2020 2020 2020 2020 2020 2069                 i
-00007770: 7465 6d20 3d20 4669 7273 745f 6d6f 6465  tem = First_mode
-00007780: 6c28 290a 2020 2020 2020 2020 2020 2020  l().            
-00007790: 2020 2069 7465 6d2e 7469 746c 6520 3d20     item.title = 
-000077a0: 6461 7461 5b27 6669 7273 746e 616d 6527  data['firstname'
-000077b0: 5d20 2b20 2720 2720 2b20 6461 7461 5b27  ] + ' ' + data['
-000077c0: 6c61 7374 6e61 6d65 275d 0a20 2020 2020  lastname'].     
-000077d0: 2020 2020 2020 2020 2020 6974 656d 2e66            item.f
-000077e0: 6972 7374 6e61 6d65 203d 2064 6174 615b  irstname = data[
-000077f0: 2766 6972 7374 6e61 6d65 275d 0a20 2020  'firstname'].   
-00007800: 2020 2020 2020 2020 2020 2020 6974 656d              item
-00007810: 2e6c 6173 746e 616d 6520 3d20 6461 7461  .lastname = data
-00007820: 5b27 6c61 7374 6e61 6d65 275d 0a20 2020  ['lastname'].   
-00007830: 2020 2020 2020 2020 2020 2020 6966 2069              if i
-00007840: 7465 6d2e 7361 7665 2829 3a0a 2020 2020  tem.save():.    
-00007850: 2020 2020 2020 2020 2020 2020 2020 7265                re
-00007860: 7475 726e 2054 7275 652c 2069 7465 6d2e  turn True, item.
-00007870: 7469 746c 6520 2b20 2720 7361 7665 6420  title + ' saved 
-00007880: 7375 6363 6573 7366 756c 6c79 270a 2020  successfully'.  
-00007890: 2020 2020 2020 2020 2020 2020 2065 6c73               els
-000078a0: 653a 0a20 2020 2020 2020 2020 2020 2020  e:.             
-000078b0: 2020 2020 2072 6574 7572 6e20 4661 6c73       return Fals
-000078c0: 652c 2069 7465 6d2e 6572 726f 7294 6807  e, item.error.h.
-000078d0: 5d94 6811 5857 0400 0066 726f 6d20 6465  ].h.XW...from de
-000078e0: 636f 7265 5f62 6173 6520 696d 706f 7274  core_base import
-000078f0: 2064 6563 6f72 650a 6672 6f6d 206d 6f64   decore.from mod
-00007900: 656c 732e 6669 7273 745f 6d6f 6465 6c20  els.first_model 
-00007910: 696d 706f 7274 2046 6972 7374 5f6d 6f64  import First_mod
-00007920: 656c 0a0a 4064 6563 6f72 652e 6261 7365  el..@decore.base
-00007930: 2874 6974 6c65 3d27 4d79 2046 6972 7374  (title='My First
-00007940: 2042 6173 6527 2c20 6963 6f6e 3d27 6d64   Base', icon='md
-00007950: 692d 686f 6d65 272c 206d 6f64 656c 3d46  i-home', model=F
-00007960: 6972 7374 5f6d 6f64 656c 290a 636c 6173  irst_model).clas
-00007970: 7320 4669 7273 745f 6261 7365 3a0a 2020  s First_base:.  
-00007980: 2040 6465 636f 7265 2e76 6965 7728 7469   @decore.view(ti
-00007990: 746c 653d 2750 6572 736f 6e27 2c20 6963  tle='Person', ic
-000079a0: 6f6e 3d27 6d64 692d 6163 636f 756e 7427  on='mdi-account'
-000079b0: 2c20 7479 7065 3d27 7461 626c 6527 2c20  , type='table', 
-000079c0: 6669 656c 6473 3d5b 4669 7273 745f 6d6f  fields=[First_mo
-000079d0: 6465 6c2e 6669 7273 746e 616d 652c 2046  del.firstname, F
-000079e0: 6972 7374 5f6d 6f64 656c 2e6c 6173 746e  irst_model.lastn
-000079f0: 616d 655d 290a 2020 2064 6566 2066 6972  ame]).   def fir
-00007a00: 7374 5f76 6965 7728 293a 0a20 2020 2020  st_view():.     
-00007a10: 2040 6465 636f 7265 2e64 6961 6c6f 6728   @decore.dialog(
-00007a20: 7469 746c 653d 2741 6464 2050 6572 736f  title='Add Perso
-00007a30: 6e27 2c20 6963 6f6e 3d27 6d64 692d 706c  n', icon='mdi-pl
-00007a40: 7573 272c 2074 7970 653d 2773 7461 6e64  us', type='stand
-00007a50: 6172 6427 2c20 6469 7370 6c61 793d 2764  ard', display='d
-00007a60: 7261 7765 7227 2c20 6163 7469 7661 746f  rawer', activato
-00007a70: 723d 2764 6566 6175 6c74 2d6d 656e 7527  r='default-menu'
-00007a80: 290a 2020 2020 2020 6465 6620 6669 7273  ).      def firs
-00007a90: 745f 6469 616c 6f67 2829 3a0a 2020 2020  t_dialog():.    
-00007aa0: 2020 2020 2040 6465 636f 7265 2e77 6964       @decore.wid
-00007ab0: 6765 7428 7469 746c 653d 2741 6464 2050  get(title='Add P
-00007ac0: 6572 736f 6e20 466f 726d 272c 2069 636f  erson Form', ico
-00007ad0: 6e3d 276d 6469 2d61 6363 6f75 6e74 272c  n='mdi-account',
-00007ae0: 2074 7970 653d 2766 6f72 6d27 2c20 6669   type='form', fi
-00007af0: 656c 6473 3d5b 4669 7273 745f 6d6f 6465  elds=[First_mode
-00007b00: 6c2e 6669 7273 746e 616d 652c 2046 6972  l.firstname, Fir
-00007b10: 7374 5f6d 6f64 656c 2e6c 6173 746e 616d  st_model.lastnam
-00007b20: 655d 290a 2020 2020 2020 2020 2064 6566  e]).         def
-00007b30: 2066 6972 7374 5f77 6964 6765 7428 293a   first_widget():
-00007b40: 0a20 2020 2020 2020 2020 2020 2040 6465  .            @de
-00007b50: 636f 7265 2e61 6374 696f 6e28 7469 746c  core.action(titl
-00007b60: 653d 2753 6176 6520 5065 7273 6f6e 272c  e='Save Person',
-00007b70: 2069 636f 6e3d 276d 6469 2d63 6f6e 7465   icon='mdi-conte
-00007b80: 6e74 2d73 6176 6527 2c20 7479 7065 3d27  nt-save', type='
-00007b90: 7375 626d 6974 2729 0a20 2020 2020 2020  submit').       
-00007ba0: 2020 2020 2064 6566 2066 6972 7374 5f61       def first_a
-00007bb0: 6374 696f 6e28 7365 6c66 2c20 6461 7461  ction(self, data
-00007bc0: 293a 0a20 2020 2020 2020 2020 2020 2020  ):.             
-00007bd0: 2020 6974 656d 203d 2046 6972 7374 5f6d    item = First_m
-00007be0: 6f64 656c 2829 0a20 2020 2020 2020 2020  odel().         
-00007bf0: 2020 2020 2020 6974 656d 2e74 6974 6c65        item.title
-00007c00: 203d 2064 6174 615b 2766 6972 7374 6e61   = data['firstna
-00007c10: 6d65 275d 202b 2027 2027 202b 2064 6174  me'] + ' ' + dat
-00007c20: 615b 276c 6173 746e 616d 6527 5d0a 2020  a['lastname'].  
-00007c30: 2020 2020 2020 2020 2020 2020 2069 7465               ite
-00007c40: 6d2e 6669 7273 746e 616d 6520 3d20 6461  m.firstname = da
-00007c50: 7461 5b27 6669 7273 746e 616d 6527 5d0a  ta['firstname'].
-00007c60: 2020 2020 2020 2020 2020 2020 2020 2069                 i
-00007c70: 7465 6d2e 6c61 7374 6e61 6d65 203d 2064  tem.lastname = d
-00007c80: 6174 615b 276c 6173 746e 616d 6527 5d0a  ata['lastname'].
-00007c90: 2020 2020 2020 2020 2020 2020 2020 2069                 i
-00007ca0: 6620 6974 656d 2e73 6176 6528 293a 0a20  f item.save():. 
-00007cb0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00007cc0: 2072 6574 7572 6e20 5472 7565 2c20 6974   return True, it
-00007cd0: 656d 2e74 6974 6c65 202b 2027 2073 6176  em.title + ' sav
-00007ce0: 6564 2073 7563 6365 7373 6675 6c6c 7927  ed successfully'
-00007cf0: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-00007d00: 656c 7365 3a0a 2020 2020 2020 2020 2020  else:.          
-00007d10: 2020 2020 2020 2020 7265 7475 726e 2046          return F
-00007d20: 616c 7365 2c20 6974 656d 2e65 7272 6f72  alse, item.error
-00007d30: 9485 9481 947d 9468 166a 4307 0000 7362  .....}.h.jC...sb
-00007d40: 6168 177d 9428 6819 5d94 681b 5d94 681d  ah.}.(h.].h.].h.
-00007d50: 5d94 681f 5d94 6821 5d94 6823 6824 6a27  ].h.].h!].h#h$j'
-00007d60: 0200 0089 6a28 0200 008c 0670 7974 686f  ....j(.....pytho
-00007d70: 6e94 6a2a 0200 007d 9475 6825 6a17 0200  n.j*...}.uh%j...
-00007d80: 0068 2768 5068 294b bf68 166a e006 0000  .h'hPh)K.h.j....
-00007d90: 6826 6803 7562 6a48 0400 0029 8194 7d94  h&h.ubjH...)..}.
-00007da0: 2868 058c b054 6f20 6372 6561 7465 2061  (h...To create a
-00007db0: 2072 6563 6f72 6420 7769 7468 2064 6563   record with dec
-00007dc0: 6f72 6520 4261 7365 2c20 7765 206e 6565  ore Base, we nee
-00007dd0: 6420 746f 2063 7265 6174 6520 616e 2069  d to create an i
-00007de0: 6e73 7461 6e63 6520 6f66 2074 6865 206d  nstance of the m
-00007df0: 6f64 656c 2e20 496e 206f 7572 2063 6173  odel. In our cas
-00007e00: 6520 2a2a 4669 7273 745f 6d6f 6465 6c2a  e **First_model*
-00007e10: 2a2e 2054 6865 2069 6e73 7461 6e63 6520  *. The instance 
-00007e20: 6973 2066 696c 6c65 6420 7769 7468 2074  is filled with t
-00007e30: 6865 2064 6174 6120 6672 6f6d 2074 6865  he data from the
-00007e40: 2066 6f72 6d20 616e 6420 7468 656e 2073   form and then s
-00007e50: 6176 6564 2e94 6807 5d94 6852 2981 947d  aved..h.].hR)..}
-00007e60: 9428 6805 6a55 0700 0068 075d 9428 6811  .(h.jU...h.].(h.
-00007e70: 8c5d 546f 2063 7265 6174 6520 6120 7265  .]To create a re
-00007e80: 636f 7264 2077 6974 6820 6465 636f 7265  cord with decore
-00007e90: 2042 6173 652c 2077 6520 6e65 6564 2074   Base, we need t
-00007ea0: 6f20 6372 6561 7465 2061 6e20 696e 7374  o create an inst
-00007eb0: 616e 6365 206f 6620 7468 6520 6d6f 6465  ance of the mode
-00007ec0: 6c2e 2049 6e20 6f75 7220 6361 7365 2094  l. In our case .
-00007ed0: 8594 8194 7d94 2868 166a 5707 0000 6826  ....}.(h.jW...h&
-00007ee0: 6803 6827 4e68 294e 7562 6866 2981 947d  h.h'Nh)Nubhf)..}
-00007ef0: 9428 6805 8c0f 2a2a 4669 7273 745f 6d6f  .(h...**First_mo
-00007f00: 6465 6c2a 2a94 6807 5d94 6811 8c0b 4669  del**.h.].h...Fi
-00007f10: 7273 745f 6d6f 6465 6c94 8594 8194 7d94  rst_model.....}.
-00007f20: 2868 166a 5e07 0000 6826 6803 6827 4e68  (h.j^...h&h.h'Nh
-00007f30: 294e 7562 6168 177d 9428 6819 5d94 681b  )Nubah.}.(h.].h.
-00007f40: 5d94 681d 5d94 681f 5d94 6821 5d94 7568  ].h.].h.].h!].uh
-00007f50: 2568 6568 166a 5707 0000 7562 6811 8c44  %heh.jW...ubh..D
-00007f60: 2e20 5468 6520 696e 7374 616e 6365 2069  . The instance i
-00007f70: 7320 6669 6c6c 6564 2077 6974 6820 7468  s filled with th
-00007f80: 6520 6461 7461 2066 726f 6d20 7468 6520  e data from the 
-00007f90: 666f 726d 2061 6e64 2074 6865 6e20 7361  form and then sa
-00007fa0: 7665 642e 9485 9481 947d 9428 6816 6a57  ved......}.(h.jW
-00007fb0: 0700 0068 2668 0368 274e 6829 4e75 6265  ...h&h.h'Nh)Nube
-00007fc0: 6817 7d94 2868 195d 9468 1b5d 9468 1d5d  h.}.(h.].h.].h.]
-00007fd0: 9468 1f5d 9468 215d 9475 6825 6851 6827  .h.].h!].uh%hQh'
-00007fe0: 6850 6829 4bd8 6816 6a53 0700 0075 6261  hPh)K.h.jS...uba
-00007ff0: 6817 7d94 2868 195d 9468 1b5d 9468 1d5d  h.}.(h.].h.].h.]
-00008000: 9468 1f5d 9468 215d 9475 6825 6a47 0400  .h.].h!].uh%jG..
-00008010: 0068 166a e006 0000 6826 6803 6827 6850  .h.j....h&h.h'hP
-00008020: 6829 4e75 6268 098c 0777 6172 6e69 6e67  h)Nubh...warning
-00008030: 9493 9429 8194 7d94 2868 058c 9954 6865  ...)..}.(h...The
-00008040: 2066 6965 6c64 202a 2a74 6974 6c65 2a2a   field **title**
-00008050: 2077 6173 2069 6e68 6572 6974 6564 2066   was inherited f
-00008060: 726f 6d20 7468 6520 636c 6173 7320 2a2a  rom the class **
-00008070: 4465 666f 726d 5f6d 6f64 656c 2a2a 2061  Deform_model** a
-00008080: 6e64 206d 7573 7420 6265 2075 7365 6420  nd must be used 
-00008090: 666f 7220 6561 6368 2072 6563 6f72 6420  for each record 
-000080a0: 6372 6561 7469 6f6e 2e20 4f74 6865 7277  creation. Otherw
-000080b0: 6973 6520 7468 6520 6974 656d 2077 696c  ise the item wil
-000080c0: 6c20 6661 696c 2074 6865 2076 616c 6964  l fail the valid
-000080d0: 6174 696f 6e2e 9468 075d 9468 5229 8194  ation..h.].hR)..
-000080e0: 7d94 2868 056a 8007 0000 6807 5d94 2868  }.(h.j....h.].(h
-000080f0: 118c 0a54 6865 2066 6965 6c64 2094 8594  ...The field ...
-00008100: 8194 7d94 2868 166a 8207 0000 6826 6803  ..}.(h.j....h&h.
-00008110: 6827 4e68 294e 7562 6866 2981 947d 9428  h'Nh)Nubhf)..}.(
-00008120: 6805 8c09 2a2a 7469 746c 652a 2a94 6807  h...**title**.h.
-00008130: 5d94 6811 8c05 7469 746c 6594 8594 8194  ].h...title.....
-00008140: 7d94 2868 166a 8907 0000 6826 6803 6827  }.(h.j....h&h.h'
-00008150: 4e68 294e 7562 6168 177d 9428 6819 5d94  Nh)Nubah.}.(h.].
-00008160: 681b 5d94 681d 5d94 681f 5d94 6821 5d94  h.].h.].h.].h!].
-00008170: 7568 2568 6568 166a 8207 0000 7562 6811  uh%heh.j....ubh.
-00008180: 8c1e 2077 6173 2069 6e68 6572 6974 6564  .. was inherited
-00008190: 2066 726f 6d20 7468 6520 636c 6173 7320   from the class 
-000081a0: 9485 9481 947d 9428 6816 6a82 0700 0068  .....}.(h.j....h
-000081b0: 2668 0368 274e 6829 4e75 6268 6629 8194  &h.h'Nh)Nubhf)..
-000081c0: 7d94 2868 058c 102a 2a44 6566 6f72 6d5f  }.(h...**Deform_
-000081d0: 6d6f 6465 6c2a 2a94 6807 5d94 6811 8c0c  model**.h.].h...
-000081e0: 4465 666f 726d 5f6d 6f64 656c 9485 9481  Deform_model....
-000081f0: 947d 9428 6816 6a9b 0700 0068 2668 0368  .}.(h.j....h&h.h
-00008200: 274e 6829 4e75 6261 6817 7d94 2868 195d  'Nh)Nubah.}.(h.]
-00008210: 9468 1b5d 9468 1d5d 9468 1f5d 9468 215d  .h.].h.].h.].h!]
-00008220: 9475 6825 6865 6816 6a82 0700 0075 6268  .uh%heh.j....ubh
-00008230: 118c 5820 616e 6420 6d75 7374 2062 6520  ..X and must be 
-00008240: 7573 6564 2066 6f72 2065 6163 6820 7265  used for each re
-00008250: 636f 7264 2063 7265 6174 696f 6e2e 204f  cord creation. O
-00008260: 7468 6572 7769 7365 2074 6865 2069 7465  therwise the ite
-00008270: 6d20 7769 6c6c 2066 6169 6c20 7468 6520  m will fail the 
-00008280: 7661 6c69 6461 7469 6f6e 2e94 8594 8194  validation......
-00008290: 7d94 2868 166a 8207 0000 6826 6803 6827  }.(h.j....h&h.h'
-000082a0: 4e68 294e 7562 6568 177d 9428 6819 5d94  Nh)Nubeh.}.(h.].
-000082b0: 681b 5d94 681d 5d94 681f 5d94 6821 5d94  h.].h.].h.].h!].
-000082c0: 7568 2568 5168 2768 5068 294b db68 166a  uh%hQh'hPh)K.h.j
-000082d0: 7e07 0000 7562 6168 177d 9428 6819 5d94  ~...ubah.}.(h.].
-000082e0: 681b 5d94 681d 5d94 681f 5d94 6821 5d94  h.].h.].h.].h!].
-000082f0: 7568 256a 7c07 0000 6816 6ae0 0600 0068  uh%j|...h.j....h
-00008300: 2668 0368 2768 5068 294e 7562 6568 177d  &h.h'hPh)Nubeh.}
-00008310: 9428 6819 5d94 8c06 6163 7469 6f6e 9461  .(h.]...action.a
-00008320: 681b 5d94 681d 5d94 8c06 6163 7469 6f6e  h.].h.]...action
-00008330: 9461 681f 5d94 6821 5d94 7568 2568 2a68  .ah.].h!].uh%h*h
-00008340: 166a 2103 0000 6826 6803 6827 6850 6829  .j!...h&h.h'hPh)
-00008350: 4bba 7562 6568 177d 9428 6819 5d94 8c05  K.ubeh.}.(h.]...
-00008360: 7573 6167 6594 6168 1b5d 9468 1d5d 948c  usage.ah.].h.]..
-00008370: 0575 7361 6765 9461 681f 5d94 6821 5d94  .usage.ah.].h!].
-00008380: 7568 2568 2a68 166a 9201 0000 6826 6803  uh%h*h.j....h&h.
-00008390: 6827 6850 6829 4b3c 7562 682b 2981 947d  h'hPh)K<ubh+)..}
-000083a0: 9428 6805 6806 6807 5d94 2868 3029 8194  .(h.h.h.].(h0)..
-000083b0: 7d94 2868 058c 1a52 756e 2c20 4465 7665  }.(h...Run, Deve
-000083c0: 6c6f 706d 656e 7420 616e 6420 4275 696c  lopment and Buil
-000083d0: 6494 6807 5d94 6811 8c1a 5275 6e2c 2044  d.h.].h...Run, D
-000083e0: 6576 656c 6f70 6d65 6e74 2061 6e64 2042  evelopment and B
-000083f0: 7569 6c64 9485 9481 947d 9428 6816 6acc  uild.....}.(h.j.
-00008400: 0700 0068 2668 0368 274e 6829 4e75 6261  ...h&h.h'Nh)Nuba
-00008410: 6817 7d94 2868 195d 9468 1b5d 9468 1d5d  h.}.(h.].h.].h.]
-00008420: 9468 1f5d 9468 215d 9475 6825 682f 6816  .h.].h!].uh%h/h.
-00008430: 6ac9 0700 0068 2668 0368 2768 5068 294b  j....h&h.h'hPh)K
-00008440: de75 6268 5229 8194 7d94 2868 058c 7154  .ubhR)..}.(h..qT
-00008450: 6f20 7374 6172 7420 6f6e 6c79 2079 6f75  o start only you
-00008460: 7220 6170 706c 6963 6174 696f 6e2c 2072  r application, r
-00008470: 756e 2060 6070 7974 686f 6e20 6170 702e  un ``python app.
-00008480: 7079 6060 2069 6e20 796f 7572 2070 726f  py`` in your pro
-00008490: 6a65 6374 2072 6f6f 7420 6469 7265 6374  ject root direct
-000084a0: 6f72 792e 2055 7365 2074 6865 2074 6572  ory. Use the ter
-000084b0: 6d69 6e61 6c20 696e 2076 7363 6f64 652e  minal in vscode.
-000084c0: 9468 075d 9428 6811 8c24 546f 2073 7461  .h.].(h..$To sta
-000084d0: 7274 206f 6e6c 7920 796f 7572 2061 7070  rt only your app
-000084e0: 6c69 6361 7469 6f6e 2c20 7275 6e20 9485  lication, run ..
-000084f0: 9481 947d 9428 6816 6ada 0700 0068 2668  ...}.(h.j....h&h
-00008500: 0368 274e 6829 4e75 626a ee02 0000 2981  .h'Nh)Nubj....).
-00008510: 947d 9428 6805 8c11 6060 7079 7468 6f6e  .}.(h...``python
-00008520: 2061 7070 2e70 7960 6094 6807 5d94 6811   app.py``.h.].h.
-00008530: 8c0d 7079 7468 6f6e 2061 7070 2e70 7994  ..python app.py.
-00008540: 8594 8194 7d94 2868 166a e207 0000 6826  ....}.(h.j....h&
-00008550: 6803 6827 4e68 294e 7562 6168 177d 9428  h.h'Nh)Nubah.}.(
-00008560: 6819 5d94 681b 5d94 681d 5d94 681f 5d94  h.].h.].h.].h.].
-00008570: 6821 5d94 7568 256a ed02 0000 6816 6ada  h!].uh%j....h.j.
-00008580: 0700 0075 6268 118c 3c20 696e 2079 6f75  ...ubh..< in you
-00008590: 7220 7072 6f6a 6563 7420 726f 6f74 2064  r project root d
-000085a0: 6972 6563 746f 7279 2e20 5573 6520 7468  irectory. Use th
-000085b0: 6520 7465 726d 696e 616c 2069 6e20 7673  e terminal in vs
-000085c0: 636f 6465 2e94 8594 8194 7d94 2868 166a  code......}.(h.j
-000085d0: da07 0000 6826 6803 6827 4e68 294e 7562  ....h&h.h'Nh)Nub
-000085e0: 6568 177d 9428 6819 5d94 681b 5d94 681d  eh.}.(h.].h.].h.
-000085f0: 5d94 681f 5d94 6821 5d94 7568 2568 5168  ].h.].h!].uh%hQh
-00008600: 2768 5068 294b df68 166a c907 0000 6826  'hPh)K.h.j....h&
-00008610: 6803 7562 6852 2981 947d 9428 6805 8c34  h.ubhR)..}.(h..4
-00008620: 4f70 656e 2074 6865 2062 726f 7773 6572  Open the browser
-00008630: 2061 6e64 2074 7970 6520 6060 6874 7470   and type ``http
-00008640: 3a2f 2f6c 6f63 616c 686f 7374 3a35 3535  ://localhost:555
-00008650: 3560 602e 9468 075d 9428 6811 8c1a 4f70  5``..h.].(h...Op
-00008660: 656e 2074 6865 2062 726f 7773 6572 2061  en the browser a
-00008670: 6e64 2074 7970 6520 9485 9481 947d 9428  nd type .....}.(
-00008680: 6816 6afa 0700 0068 2668 0368 274e 6829  h.j....h&h.h'Nh)
-00008690: 4e75 626a ee02 0000 2981 947d 9428 6805  Nubj....)..}.(h.
-000086a0: 8c19 6060 6874 7470 3a2f 2f6c 6f63 616c  ..``http://local
-000086b0: 686f 7374 3a35 3535 3560 6094 6807 5d94  host:5555``.h.].
-000086c0: 6811 8c15 6874 7470 3a2f 2f6c 6f63 616c  h...http://local
-000086d0: 686f 7374 3a35 3535 3594 8594 8194 7d94  host:5555.....}.
-000086e0: 2868 166a 0208 0000 6826 6803 6827 4e68  (h.j....h&h.h'Nh
-000086f0: 294e 7562 6168 177d 9428 6819 5d94 681b  )Nubah.}.(h.].h.
-00008700: 5d94 681d 5d94 681f 5d94 6821 5d94 7568  ].h.].h.].h!].uh
-00008710: 256a ed02 0000 6816 6afa 0700 0075 6268  %j....h.j....ubh
-00008720: 118c 012e 9485 9481 947d 9428 6816 6afa  .........}.(h.j.
-00008730: 0700 0068 2668 0368 274e 6829 4e75 6265  ...h&h.h'Nh)Nube
-00008740: 6817 7d94 2868 195d 9468 1b5d 9468 1d5d  h.}.(h.].h.].h.]
-00008750: 9468 1f5d 9468 215d 9475 6825 6851 6827  .h.].h!].uh%hQh'
-00008760: 6850 6829 4be1 6816 6ac9 0700 0068 2668  hPh)K.h.j....h&h
-00008770: 0375 6268 2b29 8194 7d94 2868 0568 0668  .ubh+)..}.(h.h.h
-00008780: 075d 9428 6830 2981 947d 9428 6805 8c0b  .].(h0)..}.(h...
-00008790: 4465 7665 6c6f 706d 656e 7494 6807 5d94  Development.h.].
-000087a0: 6811 8c0b 4465 7665 6c6f 706d 656e 7494  h...Development.
-000087b0: 8594 8194 7d94 2868 166a 1d08 0000 6826  ....}.(h.j....h&
-000087c0: 6803 6827 4e68 294e 7562 6168 177d 9428  h.h'Nh)Nubah.}.(
-000087d0: 6819 5d94 681b 5d94 681d 5d94 681f 5d94  h.].h.].h.].h.].
-000087e0: 6821 5d94 7568 2568 2f68 166a 1a08 0000  h!].uh%h/h.j....
-000087f0: 6826 6803 6827 6850 6829 4be4 7562 6852  h&h.h'hPh)K.ubhR
-00008800: 2981 947d 9428 6805 8c6c 546f 2064 6576  )..}.(h..lTo dev
-00008810: 656c 6f70 2079 6f75 7220 6170 706c 6963  elop your applic
-00008820: 6174 696f 6e2c 2075 7365 2079 6f75 7220  ation, use your 
-00008830: 6465 6275 6767 6572 2077 6974 6820 7468  debugger with th
-00008840: 6520 6060 5b64 6576 5d20 6465 636f 7265  e ``[dev] decore
-00008850: 2062 6173 6520 6465 7665 6c6f 706d 656e   base developmen
-00008860: 7460 6020 7072 6f66 696c 6520 696e 2076  t`` profile in v
-00008870: 7363 6f64 652e 9468 075d 9428 6811 8c38  scode..h.].(h..8
-00008880: 546f 2064 6576 656c 6f70 2079 6f75 7220  To develop your 
-00008890: 6170 706c 6963 6174 696f 6e2c 2075 7365  application, use
-000088a0: 2079 6f75 7220 6465 6275 6767 6572 2077   your debugger w
-000088b0: 6974 6820 7468 6520 9485 9481 947d 9428  ith the .....}.(
-000088c0: 6816 6a2b 0800 0068 2668 0368 274e 6829  h.j+...h&h.h'Nh)
-000088d0: 4e75 626a ee02 0000 2981 947d 9428 6805  Nubj....)..}.(h.
-000088e0: 8c21 6060 5b64 6576 5d20 6465 636f 7265  .!``[dev] decore
-000088f0: 2062 6173 6520 6465 7665 6c6f 706d 656e   base developmen
-00008900: 7460 6094 6807 5d94 6811 8c1d 5b64 6576  t``.h.].h...[dev
-00008910: 5d20 6465 636f 7265 2062 6173 6520 6465  ] decore base de
-00008920: 7665 6c6f 706d 656e 7494 8594 8194 7d94  velopment.....}.
-00008930: 2868 166a 3308 0000 6826 6803 6827 4e68  (h.j3...h&h.h'Nh
-00008940: 294e 7562 6168 177d 9428 6819 5d94 681b  )Nubah.}.(h.].h.
-00008950: 5d94 681d 5d94 681f 5d94 6821 5d94 7568  ].h.].h.].h!].uh
-00008960: 256a ed02 0000 6816 6a2b 0800 0075 6268  %j....h.j+...ubh
-00008970: 118c 1320 7072 6f66 696c 6520 696e 2076  ... profile in v
-00008980: 7363 6f64 652e 9485 9481 947d 9428 6816  scode......}.(h.
-00008990: 6a2b 0800 0068 2668 0368 274e 6829 4e75  j+...h&h.h'Nh)Nu
-000089a0: 6265 6817 7d94 2868 195d 9468 1b5d 9468  beh.}.(h.].h.].h
-000089b0: 1d5d 9468 1f5d 9468 215d 9475 6825 6851  .].h.].h!].uh%hQ
-000089c0: 6827 6850 6829 4be5 6816 6a1a 0800 0068  h'hPh)K.h.j....h
-000089d0: 2668 0375 6268 5229 8194 7d94 2868 058c  &h.ubhR)..}.(h..
-000089e0: 344f 7065 6e20 7468 6520 6272 6f77 7365  4Open the browse
-000089f0: 7220 616e 6420 7479 7065 2060 6068 7474  r and type ``htt
-00008a00: 703a 2f2f 6c6f 6361 6c68 6f73 743a 3535  p://localhost:55
-00008a10: 3535 6060 2e94 6807 5d94 2868 118c 1a4f  55``..h.].(h...O
-00008a20: 7065 6e20 7468 6520 6272 6f77 7365 7220  pen the browser 
-00008a30: 616e 6420 7479 7065 2094 8594 8194 7d94  and type .....}.
-00008a40: 2868 166a 4b08 0000 6826 6803 6827 4e68  (h.jK...h&h.h'Nh
-00008a50: 294e 7562 6aee 0200 0029 8194 7d94 2868  )Nubj....)..}.(h
-00008a60: 058c 1960 6068 7474 703a 2f2f 6c6f 6361  ...``http://loca
-00008a70: 6c68 6f73 743a 3535 3535 6060 9468 075d  lhost:5555``.h.]
-00008a80: 9468 118c 1568 7474 703a 2f2f 6c6f 6361  .h...http://loca
-00008a90: 6c68 6f73 743a 3535 3535 9485 9481 947d  lhost:5555.....}
-00008aa0: 9428 6816 6a53 0800 0068 2668 0368 274e  .(h.jS...h&h.h'N
-00008ab0: 6829 4e75 6261 6817 7d94 2868 195d 9468  h)Nubah.}.(h.].h
-00008ac0: 1b5d 9468 1d5d 9468 1f5d 9468 215d 9475  .].h.].h.].h!].u
-00008ad0: 6825 6aed 0200 0068 166a 4b08 0000 7562  h%j....h.jK...ub
-00008ae0: 6811 8c01 2e94 8594 8194 7d94 2868 166a  h.........}.(h.j
-00008af0: 4b08 0000 6826 6803 6827 4e68 294e 7562  K...h&h.h'Nh)Nub
-00008b00: 6568 177d 9428 6819 5d94 681b 5d94 681d  eh.}.(h.].h.].h.
-00008b10: 5d94 681f 5d94 6821 5d94 7568 2568 5168  ].h.].h!].uh%hQh
-00008b20: 2768 5068 294b e768 166a 1a08 0000 6826  'hPh)K.h.j....h&
-00008b30: 6803 7562 6568 177d 9428 6819 5d94 8c0b  h.ubeh.}.(h.]...
-00008b40: 6465 7665 6c6f 706d 656e 7494 6168 1b5d  development.ah.]
-00008b50: 9468 1d5d 948c 0b64 6576 656c 6f70 6d65  .h.]...developme
-00008b60: 6e74 9461 681f 5d94 6821 5d94 7568 2568  nt.ah.].h!].uh%h
-00008b70: 2a68 166a c907 0000 6826 6803 6827 6850  *h.j....h&h.h'hP
-00008b80: 6829 4be4 7562 682b 2981 947d 9428 6805  h)K.ubh+)..}.(h.
-00008b90: 6806 6807 5d94 2868 3029 8194 7d94 2868  h.h.].(h0)..}.(h
-00008ba0: 058c 0542 7569 6c64 9468 075d 9468 118c  ...Build.h.].h..
-00008bb0: 0542 7569 6c64 9485 9481 947d 9428 6816  .Build.....}.(h.
-00008bc0: 6a76 0800 0068 2668 0368 274e 6829 4e75  jv...h&h.h'Nh)Nu
-00008bd0: 6261 6817 7d94 2868 195d 9468 1b5d 9468  bah.}.(h.].h.].h
-00008be0: 1d5d 9468 1f5d 9468 215d 9475 6825 682f  .].h.].h!].uh%h/
-00008bf0: 6816 6a73 0800 0068 2668 0368 2768 5068  h.js...h&h.h'hPh
-00008c00: 294b ea75 6268 5229 8194 7d94 2868 058c  )K.ubhR)..}.(h..
-00008c10: 7454 6f20 6275 696c 6420 796f 7572 2061  tTo build your a
-00008c20: 7070 6c69 6361 7469 6f6e 2c20 7275 6e20  pplication, run 
-00008c30: 6060 7079 7468 6f6e 2061 7070 2e70 7920  ``python app.py 
-00008c40: 2d2d 6275 696c 6460 6020 696e 2079 6f75  --build`` in you
-00008c50: 7220 7072 6f6a 6563 7420 726f 6f74 2064  r project root d
-00008c60: 6972 6563 746f 7279 2e20 5573 6520 7468  irectory. Use th
-00008c70: 6520 7465 726d 696e 616c 2069 6e20 7673  e terminal in vs
-00008c80: 636f 6465 2e94 6807 5d94 2868 118c 1f54  code..h.].(h...T
-00008c90: 6f20 6275 696c 6420 796f 7572 2061 7070  o build your app
-00008ca0: 6c69 6361 7469 6f6e 2c20 7275 6e20 9485  lication, run ..
-00008cb0: 9481 947d 9428 6816 6a84 0800 0068 2668  ...}.(h.j....h&h
-00008cc0: 0368 274e 6829 4e75 626a ee02 0000 2981  .h'Nh)Nubj....).
-00008cd0: 947d 9428 6805 8c19 6060 7079 7468 6f6e  .}.(h...``python
-00008ce0: 2061 7070 2e70 7920 2d2d 6275 696c 6460   app.py --build`
-00008cf0: 6094 6807 5d94 6811 8c15 7079 7468 6f6e  `.h.].h...python
-00008d00: 2061 7070 2e70 7920 2d2d 6275 696c 6494   app.py --build.
-00008d10: 8594 8194 7d94 2868 166a 8c08 0000 6826  ....}.(h.j....h&
-00008d20: 6803 6827 4e68 294e 7562 6168 177d 9428  h.h'Nh)Nubah.}.(
-00008d30: 6819 5d94 681b 5d94 681d 5d94 681f 5d94  h.].h.].h.].h.].
-00008d40: 6821 5d94 7568 256a ed02 0000 6816 6a84  h!].uh%j....h.j.
-00008d50: 0800 0075 6268 118c 3c20 696e 2079 6f75  ...ubh..< in you
-00008d60: 7220 7072 6f6a 6563 7420 726f 6f74 2064  r project root d
-00008d70: 6972 6563 746f 7279 2e20 5573 6520 7468  irectory. Use th
-00008d80: 6520 7465 726d 696e 616c 2069 6e20 7673  e terminal in vs
-00008d90: 636f 6465 2e94 8594 8194 7d94 2868 166a  code......}.(h.j
-00008da0: 8408 0000 6826 6803 6827 4e68 294e 7562  ....h&h.h'Nh)Nub
-00008db0: 6568 177d 9428 6819 5d94 681b 5d94 681d  eh.}.(h.].h.].h.
-00008dc0: 5d94 681f 5d94 6821 5d94 7568 2568 5168  ].h.].h!].uh%hQh
-00008dd0: 2768 5068 294b eb68 166a 7308 0000 6826  'hPh)K.h.js...h&
-00008de0: 6803 7562 6568 177d 9428 6819 5d94 8c05  h.ubeh.}.(h.]...
-00008df0: 6275 696c 6494 6168 1b5d 9468 1d5d 948c  build.ah.].h.]..
-00008e00: 0562 7569 6c64 9461 681f 5d94 6821 5d94  .build.ah.].h!].
-00008e10: 7568 2568 2a68 166a c907 0000 6826 6803  uh%h*h.j....h&h.
-00008e20: 6827 6850 6829 4bea 7562 6568 177d 9428  h'hPh)K.ubeh.}.(
-00008e30: 6819 5d94 8c19 7275 6e2d 6465 7665 6c6f  h.]...run-develo
-00008e40: 706d 656e 742d 616e 642d 6275 696c 6494  pment-and-build.
-00008e50: 6168 1b5d 9468 1d5d 948c 1a72 756e 2c20  ah.].h.]...run, 
-00008e60: 6465 7665 6c6f 706d 656e 7420 616e 6420  development and 
-00008e70: 6275 696c 6494 6168 1f5d 9468 215d 9475  build.ah.].h!].u
-00008e80: 6825 682a 6816 6a92 0100 0068 2668 0368  h%h*h.j....h&h.h
-00008e90: 2768 5068 294b de75 6265 6817 7d94 2868  'hPh)K.ubeh.}.(h
-00008ea0: 195d 948c 0b67 6574 2d73 7461 7274 6564  .]...get-started
-00008eb0: 9461 681b 5d94 681d 5d94 8c0b 6765 7420  .ah.].h.]...get 
-00008ec0: 7374 6172 7465 6494 6168 1f5d 9468 215d  started.ah.].h!]
-00008ed0: 9475 6825 682a 6816 682c 6826 6803 6827  .uh%h*h.h,h&h.h'
-00008ee0: 6850 6829 4b1a 7562 682b 2981 947d 9428  hPh)K.ubh+)..}.(
-00008ef0: 6805 6806 6807 5d94 2868 3029 8194 7d94  h.h.h.].(h0)..}.
-00008f00: 2868 058c 1253 616d 706c 6520 6170 706c  (h...Sample appl
-00008f10: 6963 6174 696f 6e94 6807 5d94 6811 8c12  ication.h.].h...
-00008f20: 5361 6d70 6c65 2061 7070 6c69 6361 7469  Sample applicati
-00008f30: 6f6e 9485 9481 947d 9428 6816 6abf 0800  on.....}.(h.j...
-00008f40: 0068 2668 0368 274e 6829 4e75 6261 6817  .h&h.h'Nh)Nubah.
-00008f50: 7d94 2868 195d 9468 1b5d 9468 1d5d 9468  }.(h.].h.].h.].h
-00008f60: 1f5d 9468 215d 9475 6825 682f 6816 6abc  .].h!].uh%h/h.j.
-00008f70: 0800 0068 2668 0368 2768 5068 294b ee75  ...h&h.h'hPh)K.u
-00008f80: 6268 5229 8194 7d94 2868 058c 9e54 6f20  bhR)..}.(h...To 
-00008f90: 6265 7474 6572 2075 6e64 6572 7374 616e  better understan
-00008fa0: 6420 686f 7720 6465 636f 7265 2062 6173  d how decore bas
-00008fb0: 6520 776f 726b 732c 2069 7420 6973 2062  e works, it is b
-00008fc0: 6573 7420 746f 206c 6f6f 6b20 6174 2074  est to look at t
-00008fd0: 6865 2073 616d 706c 6520 6170 706c 6963  he sample applic
-00008fe0: 6174 696f 6e2e 2054 6865 2061 7070 6c69  ation. The appli
-00008ff0: 6361 7469 6f6e 2072 6570 7265 7365 6e74  cation represent
-00009000: 7320 6d79 2063 6f6e 7469 6e75 6f75 7320  s my continuous 
-00009010: 6465 7665 6c6f 706d 656e 7420 6f66 2064  development of d
-00009020: 6563 6f72 6520 6261 7365 2e94 6807 5d94  ecore base..h.].
-00009030: 6811 8c9e 546f 2062 6574 7465 7220 756e  h...To better un
-00009040: 6465 7273 7461 6e64 2068 6f77 2064 6563  derstand how dec
-00009050: 6f72 6520 6261 7365 2077 6f72 6b73 2c20  ore base works, 
-00009060: 6974 2069 7320 6265 7374 2074 6f20 6c6f  it is best to lo
-00009070: 6f6b 2061 7420 7468 6520 7361 6d70 6c65  ok at the sample
-00009080: 2061 7070 6c69 6361 7469 6f6e 2e20 5468   application. Th
-00009090: 6520 6170 706c 6963 6174 696f 6e20 7265  e application re
-000090a0: 7072 6573 656e 7473 206d 7920 636f 6e74  presents my cont
-000090b0: 696e 756f 7573 2064 6576 656c 6f70 6d65  inuous developme
-000090c0: 6e74 206f 6620 6465 636f 7265 2062 6173  nt of decore bas
-000090d0: 652e 9485 9481 947d 9428 6816 6acd 0800  e......}.(h.j...
-000090e0: 0068 2668 0368 274e 6829 4e75 6261 6817  .h&h.h'Nh)Nubah.
-000090f0: 7d94 2868 195d 9468 1b5d 9468 1d5d 9468  }.(h.].h.].h.].h
-00009100: 1f5d 9468 215d 9475 6825 6851 6827 6850  .].h!].uh%hQh'hP
-00009110: 6829 4bef 6816 6abc 0800 0068 2668 0375  h)K.h.j....h&h.u
-00009120: 6268 5229 8194 7d94 2868 058c 4868 7474  bhR)..}.(h..Hhtt
-00009130: 7073 3a2f 2f67 6974 6875 622e 636f 6d2f  ps://github.com/
-00009140: 4b65 6d6f 5061 6e7a 6168 2f64 6563 6f72  KemoPanzah/decor
-00009150: 655f 4261 7365 2f74 7265 652f 6d61 7374  e_Base/tree/mast
-00009160: 6572 2f64 6563 6f72 655f 6261 7365 2f73  er/decore_base/s
-00009170: 616d 706c 6594 6807 5d94 6892 2981 947d  ample.h.].h.)..}
-00009180: 9428 6805 6add 0800 0068 075d 9468 118c  .(h.j....h.].h..
-00009190: 4868 7474 7073 3a2f 2f67 6974 6875 622e  Hhttps://github.
-000091a0: 636f 6d2f 4b65 6d6f 5061 6e7a 6168 2f64  com/KemoPanzah/d
-000091b0: 6563 6f72 655f 4261 7365 2f74 7265 652f  ecore_Base/tree/
-000091c0: 6d61 7374 6572 2f64 6563 6f72 655f 6261  master/decore_ba
-000091d0: 7365 2f73 616d 706c 6594 8594 8194 7d94  se/sample.....}.
-000091e0: 2868 166a df08 0000 6826 6803 6827 4e68  (h.j....h&h.h'Nh
-000091f0: 294e 7562 6168 177d 9428 6819 5d94 681b  )Nubah.}.(h.].h.
-00009200: 5d94 681d 5d94 681f 5d94 6821 5d94 8c06  ].h.].h.].h!]...
-00009210: 7265 6675 7269 946a dd08 0000 7568 2568  refuri.j....uh%h
-00009220: 9168 166a db08 0000 7562 6168 177d 9428  .h.j....ubah.}.(
-00009230: 6819 5d94 681b 5d94 681d 5d94 681f 5d94  h.].h.].h.].h.].
-00009240: 6821 5d94 7568 2568 5168 2768 5068 294b  h!].uh%hQh'hPh)K
-00009250: f168 166a bc08 0000 6826 6803 7562 6852  .h.j....h&h.ubhR
-00009260: 2981 947d 9428 6805 8cb0 546f 2073 796e  )..}.(h...To syn
-00009270: 6368 726f 6e69 7a65 2074 6865 2073 616d  chronize the sam
-00009280: 706c 6520 6170 706c 6963 6174 696f 6e20  ple application 
-00009290: 7769 7468 2061 2073 7562 666f 6c64 6572  with a subfolder
-000092a0: 206f 6620 7468 6520 7072 6f6a 6563 7420   of the project 
-000092b0: 726f 6f74 2064 6972 6563 746f 7279 2c20  root directory, 
-000092c0: 7275 6e20 6060 7079 7468 6f6e 2061 7070  run ``python app
-000092d0: 2e70 7920 2d2d 7361 6d70 6c65 6060 2069  .py --sample`` i
-000092e0: 6e20 796f 7572 2070 726f 6a65 6374 2072  n your project r
-000092f0: 6f6f 7420 6469 7265 6374 6f72 792e 2055  oot directory. U
-00009300: 7365 2074 6865 2074 6572 6d69 6e61 6c20  se the terminal 
-00009310: 696e 2076 7363 6f64 652e 9468 075d 9428  in vscode..h.].(
-00009320: 6811 8c5a 546f 2073 796e 6368 726f 6e69  h..ZTo synchroni
-00009330: 7a65 2074 6865 2073 616d 706c 6520 6170  ze the sample ap
-00009340: 706c 6963 6174 696f 6e20 7769 7468 2061  plication with a
-00009350: 2073 7562 666f 6c64 6572 206f 6620 7468   subfolder of th
-00009360: 6520 7072 6f6a 6563 7420 726f 6f74 2064  e project root d
-00009370: 6972 6563 746f 7279 2c20 7275 6e20 9485  irectory, run ..
-00009380: 9481 947d 9428 6816 6af3 0800 0068 2668  ...}.(h.j....h&h
-00009390: 0368 274e 6829 4e75 626a ee02 0000 2981  .h'Nh)Nubj....).
-000093a0: 947d 9428 6805 8c1a 6060 7079 7468 6f6e  .}.(h...``python
-000093b0: 2061 7070 2e70 7920 2d2d 7361 6d70 6c65   app.py --sample
-000093c0: 6060 9468 075d 9468 118c 1670 7974 686f  ``.h.].h...pytho
-000093d0: 6e20 6170 702e 7079 202d 2d73 616d 706c  n app.py --sampl
-000093e0: 6594 8594 8194 7d94 2868 166a fb08 0000  e.....}.(h.j....
-000093f0: 6826 6803 6827 4e68 294e 7562 6168 177d  h&h.h'Nh)Nubah.}
-00009400: 9428 6819 5d94 681b 5d94 681d 5d94 681f  .(h.].h.].h.].h.
-00009410: 5d94 6821 5d94 7568 256a ed02 0000 6816  ].h!].uh%j....h.
-00009420: 6af3 0800 0075 6268 118c 3c20 696e 2079  j....ubh..< in y
-00009430: 6f75 7220 7072 6f6a 6563 7420 726f 6f74  our project root
-00009440: 2064 6972 6563 746f 7279 2e20 5573 6520   directory. Use 
-00009450: 7468 6520 7465 726d 696e 616c 2069 6e20  the terminal in 
-00009460: 7673 636f 6465 2e94 8594 8194 7d94 2868  vscode......}.(h
-00009470: 166a f308 0000 6826 6803 6827 4e68 294e  .j....h&h.h'Nh)N
-00009480: 7562 6568 177d 9428 6819 5d94 681b 5d94  ubeh.}.(h.].h.].
-00009490: 681d 5d94 681f 5d94 6821 5d94 7568 2568  h.].h.].h!].uh%h
-000094a0: 5168 2768 5068 294b f368 166a bc08 0000  Qh'hPh)K.h.j....
-000094b0: 6826 6803 7562 6852 2981 947d 9428 6805  h&h.ubhR)..}.(h.
-000094c0: 8c7f 546f 2072 756e 2074 6865 2073 616d  ..To run the sam
-000094d0: 706c 6520 6170 706c 6963 6174 696f 6e20  ple application 
-000094e0: 6166 7465 7220 7379 6e63 6872 6f6e 697a  after synchroniz
-000094f0: 6174 696f 6e2c 2075 7365 2079 6f75 7220  ation, use your 
-00009500: 6465 6275 6767 6572 2077 6974 6820 7468  debugger with th
-00009510: 6520 6060 5b73 6d70 5d20 6465 636f 7265  e ``[smp] decore
-00009520: 2062 6173 6520 7361 6d70 6c65 6060 2070   base sample`` p
-00009530: 726f 6669 6c65 2069 6e20 7673 636f 6465  rofile in vscode
-00009540: 2e94 6807 5d94 2868 118c 5054 6f20 7275  ..h.].(h..PTo ru
-00009550: 6e20 7468 6520 7361 6d70 6c65 2061 7070  n the sample app
-00009560: 6c69 6361 7469 6f6e 2061 6674 6572 2073  lication after s
-00009570: 796e 6368 726f 6e69 7a61 7469 6f6e 2c20  ynchronization, 
-00009580: 7573 6520 796f 7572 2064 6562 7567 6765  use your debugge
-00009590: 7220 7769 7468 2074 6865 2094 8594 8194  r with the .....
-000095a0: 7d94 2868 166a 1309 0000 6826 6803 6827  }.(h.j....h&h.h'
-000095b0: 4e68 294e 7562 6aee 0200 0029 8194 7d94  Nh)Nubj....)..}.
-000095c0: 2868 058c 1c60 605b 736d 705d 2064 6563  (h...``[smp] dec
-000095d0: 6f72 6520 6261 7365 2073 616d 706c 6560  ore base sample`
-000095e0: 6094 6807 5d94 6811 8c18 5b73 6d70 5d20  `.h.].h...[smp] 
-000095f0: 6465 636f 7265 2062 6173 6520 7361 6d70  decore base samp
-00009600: 6c65 9485 9481 947d 9428 6816 6a1b 0900  le.....}.(h.j...
-00009610: 0068 2668 0368 274e 6829 4e75 6261 6817  .h&h.h'Nh)Nubah.
-00009620: 7d94 2868 195d 9468 1b5d 9468 1d5d 9468  }.(h.].h.].h.].h
-00009630: 1f5d 9468 215d 9475 6825 6aed 0200 0068  .].h!].uh%j....h
-00009640: 166a 1309 0000 7562 6811 8c13 2070 726f  .j....ubh... pro
-00009650: 6669 6c65 2069 6e20 7673 636f 6465 2e94  file in vscode..
-00009660: 8594 8194 7d94 2868 166a 1309 0000 6826  ....}.(h.j....h&
-00009670: 6803 6827 4e68 294e 7562 6568 177d 9428  h.h'Nh)Nubeh.}.(
-00009680: 6819 5d94 681b 5d94 681d 5d94 681f 5d94  h.].h.].h.].h.].
-00009690: 6821 5d94 7568 2568 5168 2768 5068 294b  h!].uh%hQh'hPh)K
-000096a0: f568 166a bc08 0000 6826 6803 7562 6568  .h.j....h&h.ubeh
-000096b0: 177d 9428 6819 5d94 8c12 7361 6d70 6c65  .}.(h.]...sample
-000096c0: 2d61 7070 6c69 6361 7469 6f6e 9461 681b  -application.ah.
-000096d0: 5d94 681d 5d94 8c12 7361 6d70 6c65 2061  ].h.]...sample a
-000096e0: 7070 6c69 6361 7469 6f6e 9461 681f 5d94  pplication.ah.].
-000096f0: 6821 5d94 7568 2568 2a68 1668 2c68 2668  h!].uh%h*h.h,h&h
-00009700: 0368 2768 5068 294b ee75 6268 2b29 8194  .h'hPh)K.ubh+)..
-00009710: 7d94 2868 0568 0668 075d 9428 6830 2981  }.(h.h.h.].(h0).
-00009720: 947d 9428 6805 8c05 4e6f 7465 7394 6807  .}.(h...Notes.h.
-00009730: 5d94 6811 8c05 4e6f 7465 7394 8594 8194  ].h...Notes.....
-00009740: 7d94 2868 166a 3e09 0000 6826 6803 6827  }.(h.j>...h&h.h'
-00009750: 4e68 294e 7562 6168 177d 9428 6819 5d94  Nh)Nubah.}.(h.].
-00009760: 681b 5d94 681d 5d94 681f 5d94 6821 5d94  h.].h.].h.].h!].
-00009770: 7568 2568 2f68 166a 3b09 0000 6826 6803  uh%h/h.j;...h&h.
-00009780: 6827 6850 6829 4bf8 7562 6852 2981 947d  h'hPh)K.ubhR)..}
-00009790: 9428 6805 8c46 5468 6973 2064 6f63 756d  .(h..FThis docum
-000097a0: 656e 7461 7469 6f6e 2077 6173 2074 7261  entation was tra
-000097b0: 6e73 6c61 7465 6420 6672 6f6d 2047 6572  nslated from Ger
-000097c0: 6d61 6e20 696e 746f 2045 6e67 6c69 7368  man into English
-000097d0: 2077 6974 6820 4465 6570 6c2e 9468 075d   with Deepl..h.]
-000097e0: 9468 118c 4654 6869 7320 646f 6375 6d65  .h..FThis docume
-000097f0: 6e74 6174 696f 6e20 7761 7320 7472 616e  ntation was tran
-00009800: 736c 6174 6564 2066 726f 6d20 4765 726d  slated from Germ
-00009810: 616e 2069 6e74 6f20 456e 676c 6973 6820  an into English 
-00009820: 7769 7468 2044 6565 706c 2e94 8594 8194  with Deepl......
-00009830: 7d94 2868 166a 4c09 0000 6826 6803 6827  }.(h.jL...h&h.h'
-00009840: 4e68 294e 7562 6168 177d 9428 6819 5d94  Nh)Nubah.}.(h.].
-00009850: 681b 5d94 681d 5d94 681f 5d94 6821 5d94  h.].h.].h.].h!].
-00009860: 7568 2568 5168 2768 5068 294b f968 166a  uh%hQh'hPh)K.h.j
-00009870: 3b09 0000 6826 6803 7562 6809 8c08 636f  ;...h&h.ubh...co
-00009880: 6d70 6f75 6e64 9493 9429 8194 7d94 2868  mpound...)..}.(h
-00009890: 0568 0668 075d 9468 008c 0774 6f63 7472  .h.h.].h...toctr
-000098a0: 6565 9493 9429 8194 7d94 2868 0568 0668  ee...)..}.(h.h.h
-000098b0: 075d 9468 177d 9428 6819 5d94 681b 5d94  .].h.}.(h.].h.].
-000098c0: 681d 5d94 681f 5d94 6821 5d94 6816 8c05  h.].h.].h!].h...
-000098d0: 696e 6465 7894 8c07 656e 7472 6965 7394  index...entries.
-000098e0: 5d94 8c0c 696e 636c 7564 6566 696c 6573  ]...includefiles
-000098f0: 945d 948c 086d 6178 6465 7074 6894 4b02  .]...maxdepth.K.
-00009900: 8c07 6361 7074 696f 6e94 4e8c 0467 6c6f  ..caption.N..glo
-00009910: 6294 898c 0668 6964 6465 6e94 888c 0d69  b....hidden....i
-00009920: 6e63 6c75 6465 6869 6464 656e 9489 8c08  ncludehidden....
-00009930: 6e75 6d62 6572 6564 944b 008c 0a74 6974  numbered.K...tit
-00009940: 6c65 736f 6e6c 7994 898c 0a72 6177 656e  lesonly....rawen
-00009950: 7472 6965 7394 5d94 7568 256a 5f09 0000  tries.].uh%j_...
-00009960: 6827 6828 6829 4b0b 6816 6a5c 0900 0075  h'h(h)K.h.j\...u
-00009970: 6261 6817 7d94 2868 195d 9468 1b5d 948c  bah.}.(h.].h.]..
-00009980: 0f74 6f63 7472 6565 2d77 7261 7070 6572  .toctree-wrapper
-00009990: 9461 681d 5d94 681f 5d94 6821 5d94 7568  .ah.].h.].h!].uh
-000099a0: 256a 5a09 0000 6816 6a3b 0900 0068 2668  %jZ...h.j;...h&h
-000099b0: 0368 2768 2868 294e 7562 680b 2981 947d  .h'h(h)Nubh.)..}
-000099c0: 9428 6805 8c12 496e 6469 6365 7320 616e  .(h...Indices an
-000099d0: 6420 7461 626c 6573 9468 075d 9468 118c  d tables.h.].h..
-000099e0: 1249 6e64 6963 6573 2061 6e64 2074 6162  .Indices and tab
-000099f0: 6c65 7394 8594 8194 7d94 6816 6a7f 0900  les.....}.h.j...
-00009a00: 0073 6261 6817 7d94 2868 195d 9468 1b5d  .sbah.}.(h.].h.]
-00009a10: 9468 1d5d 9468 1f5d 9468 215d 9468 2368  .h.].h.].h!].h#h
-00009a20: 2475 6825 680a 6816 6a3b 0900 0068 2668  $uh%h.h.j;...h&h
-00009a30: 0368 2768 2868 294b 0f75 6268 0b29 8194  .h'h(h)K.ubh.)..
-00009a40: 7d94 2868 058c 123d 3d3d 3d3d 3d3d 3d3d  }.(h...=========
-00009a50: 3d3d 3d3d 3d3d 3d3d 3d94 6807 5d94 6811  =========.h.].h.
-00009a60: 8c12 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d  ..==============
-00009a70: 3d3d 3d3d 9485 9481 947d 9468 166a 8d09  ====.....}.h.j..
-00009a80: 0000 7362 6168 177d 9428 6819 5d94 681b  ..sbah.}.(h.].h.
-00009a90: 5d94 681d 5d94 681f 5d94 6821 5d94 6823  ].h.].h.].h!].h#
-00009aa0: 6824 7568 2568 0a68 166a 3b09 0000 6826  h$uh%h.h.j;...h&
-00009ab0: 6803 6827 6828 6829 4b11 7562 680b 2981  h.h'h(h)K.ubh.).
-00009ac0: 947d 9428 6805 8c11 2a20 3a72 6566 3a60  .}.(h...* :ref:`
-00009ad0: 6765 6e69 6e64 6578 6094 6807 5d94 6811  genindex`.h.].h.
-00009ae0: 8c11 2a20 3a72 6566 3a60 6765 6e69 6e64  ..* :ref:`genind
-00009af0: 6578 6094 8594 8194 7d94 6816 6a9b 0900  ex`.....}.h.j...
-00009b00: 0073 6261 6817 7d94 2868 195d 9468 1b5d  .sbah.}.(h.].h.]
-00009b10: 9468 1d5d 9468 1f5d 9468 215d 9468 2368  .h.].h.].h!].h#h
-00009b20: 2475 6825 680a 6816 6a3b 0900 0068 2668  $uh%h.h.j;...h&h
-00009b30: 0368 2768 2868 294b 1275 6268 0b29 8194  .h'h(h)K.ubh.)..
-00009b40: 7d94 2868 058c 112a 203a 7265 663a 606d  }.(h...* :ref:`m
-00009b50: 6f64 696e 6465 7860 9468 075d 9468 118c  odindex`.h.].h..
-00009b60: 112a 203a 7265 663a 606d 6f64 696e 6465  .* :ref:`modinde
-00009b70: 7860 9485 9481 947d 9468 166a a909 0000  x`.....}.h.j....
-00009b80: 7362 6168 177d 9428 6819 5d94 681b 5d94  sbah.}.(h.].h.].
-00009b90: 681d 5d94 681f 5d94 6821 5d94 6823 6824  h.].h.].h!].h#h$
-00009ba0: 7568 2568 0a68 166a 3b09 0000 6826 6803  uh%h.h.j;...h&h.
-00009bb0: 6827 6828 6829 4b13 7562 680b 2981 947d  h'h(h)K.ubh.)..}
-00009bc0: 9428 6805 8c0f 2a20 3a72 6566 3a60 7365  .(h...* :ref:`se
-00009bd0: 6172 6368 6094 6807 5d94 6811 8c0f 2a20  arch`.h.].h...* 
-00009be0: 3a72 6566 3a60 7365 6172 6368 6094 8594  :ref:`search`...
-00009bf0: 8194 7d94 6816 6ab7 0900 0073 6261 6817  ..}.h.j....sbah.
-00009c00: 7d94 2868 195d 9468 1b5d 9468 1d5d 9468  }.(h.].h.].h.].h
-00009c10: 1f5d 9468 215d 9468 2368 2475 6825 680a  .].h!].h#h$uh%h.
-00009c20: 6816 6a3b 0900 0068 2668 0368 2768 2868  h.j;...h&h.h'h(h
-00009c30: 294b 1475 6265 6817 7d94 2868 195d 948c  )K.ubeh.}.(h.]..
-00009c40: 056e 6f74 6573 9461 681b 5d94 681d 5d94  .notes.ah.].h.].
-00009c50: 8c05 6e6f 7465 7394 6168 1f5d 9468 215d  ..notes.ah.].h!]
-00009c60: 9475 6825 682a 6816 682c 6826 6803 6827  .uh%h*h.h,h&h.h'
-00009c70: 6850 6829 4bf8 7562 6568 177d 9428 6819  hPh)K.ubeh.}.(h.
-00009c80: 5d94 8c07 7765 6c63 6f6d 6594 6168 1b5d  ]...welcome.ah.]
-00009c90: 9468 1d5d 948c 0777 656c 636f 6d65 9461  .h.]...welcome.a
-00009ca0: 681f 5d94 6821 5d94 7568 2568 2a68 1668  h.].h!].uh%h*h.h
-00009cb0: 0368 2668 0368 2768 2868 294b 0775 6265  .h&h.h'h(h)K.ube
-00009cc0: 6817 7d94 2868 195d 9468 1b5d 9468 1d5d  h.}.(h.].h.].h.]
-00009cd0: 9468 1f5d 9468 215d 948c 0673 6f75 7263  .h.].h!]...sourc
-00009ce0: 6594 6828 7568 2568 018c 0e63 7572 7265  e.h(uh%h...curre
-00009cf0: 6e74 5f73 6f75 7263 6594 4e8c 0c63 7572  nt_source.N..cur
-00009d00: 7265 6e74 5f6c 696e 6594 4e8c 0873 6574  rent_line.N..set
-00009d10: 7469 6e67 7394 8c11 646f 6375 7469 6c73  tings...docutils
-00009d20: 2e66 726f 6e74 656e 6494 8c06 5661 6c75  .frontend...Valu
-00009d30: 6573 9493 9429 8194 7d94 2868 2f4e 8c09  es...)..}.(h/N..
-00009d40: 6765 6e65 7261 746f 7294 4e8c 0964 6174  generator.N..dat
-00009d50: 6573 7461 6d70 944e 8c0b 736f 7572 6365  estamp.N..source
-00009d60: 5f6c 696e 6b94 4e8c 0a73 6f75 7263 655f  _link.N..source_
-00009d70: 7572 6c94 4e8c 0d74 6f63 5f62 6163 6b6c  url.N..toc_backl
-00009d80: 696e 6b73 948c 0565 6e74 7279 948c 1266  inks...entry...f
-00009d90: 6f6f 746e 6f74 655f 6261 636b 6c69 6e6b  ootnote_backlink
-00009da0: 7394 4b01 8c0d 7365 6374 6e75 6d5f 7866  s.K...sectnum_xf
-00009db0: 6f72 6d94 4b01 8c0e 7374 7269 705f 636f  orm.K...strip_co
-00009dc0: 6d6d 656e 7473 944e 8c1b 7374 7269 705f  mments.N..strip_
-00009dd0: 656c 656d 656e 7473 5f77 6974 685f 636c  elements_with_cl
-00009de0: 6173 7365 7394 4e8c 0d73 7472 6970 5f63  asses.N..strip_c
-00009df0: 6c61 7373 6573 944e 8c0c 7265 706f 7274  lasses.N..report
-00009e00: 5f6c 6576 656c 944b 028c 0a68 616c 745f  _level.K...halt_
-00009e10: 6c65 7665 6c94 4b05 8c11 6578 6974 5f73  level.K...exit_s
-00009e20: 7461 7475 735f 6c65 7665 6c94 4b05 8c05  tatus_level.K...
-00009e30: 6465 6275 6794 4e8c 0e77 6172 6e69 6e67  debug.N..warning
-00009e40: 5f73 7472 6561 6d94 4e8c 0974 7261 6365  _stream.N..trace
-00009e50: 6261 636b 9488 8c0e 696e 7075 745f 656e  back....input_en
-00009e60: 636f 6469 6e67 948c 0975 7466 2d38 2d73  coding...utf-8-s
-00009e70: 6967 948c 1c69 6e70 7574 5f65 6e63 6f64  ig...input_encod
-00009e80: 696e 675f 6572 726f 725f 6861 6e64 6c65  ing_error_handle
-00009e90: 7294 8c06 7374 7269 6374 948c 0f6f 7574  r...strict...out
-00009ea0: 7075 745f 656e 636f 6469 6e67 948c 0575  put_encoding...u
-00009eb0: 7466 2d38 948c 1d6f 7574 7075 745f 656e  tf-8...output_en
-00009ec0: 636f 6469 6e67 5f65 7272 6f72 5f68 616e  coding_error_han
-00009ed0: 646c 6572 946a f809 0000 8c0e 6572 726f  dler.j......erro
-00009ee0: 725f 656e 636f 6469 6e67 948c 0575 7466  r_encoding...utf
-00009ef0: 2d38 948c 1c65 7272 6f72 5f65 6e63 6f64  -8...error_encod
-00009f00: 696e 675f 6572 726f 725f 6861 6e64 6c65  ing_error_handle
-00009f10: 7294 8c10 6261 636b 736c 6173 6872 6570  r...backslashrep
-00009f20: 6c61 6365 948c 0d6c 616e 6775 6167 655f  lace...language_
-00009f30: 636f 6465 948c 0265 6e94 8c13 7265 636f  code...en...reco
-00009f40: 7264 5f64 6570 656e 6465 6e63 6965 7394  rd_dependencies.
-00009f50: 4e8c 0663 6f6e 6669 6794 4e8c 0969 645f  N..config.N..id_
-00009f60: 7072 6566 6978 9468 068c 0e61 7574 6f5f  prefix.h...auto_
-00009f70: 6964 5f70 7265 6669 7894 8c02 6964 948c  id_prefix...id..
-00009f80: 0d64 756d 705f 7365 7474 696e 6773 944e  .dump_settings.N
-00009f90: 8c0e 6475 6d70 5f69 6e74 6572 6e61 6c73  ..dump_internals
-00009fa0: 944e 8c0f 6475 6d70 5f74 7261 6e73 666f  .N..dump_transfo
-00009fb0: 726d 7394 4e8c 0f64 756d 705f 7073 6575  rms.N..dump_pseu
-00009fc0: 646f 5f78 6d6c 944e 8c10 6578 706f 7365  do_xml.N..expose
-00009fd0: 5f69 6e74 6572 6e61 6c73 944e 8c0e 7374  _internals.N..st
-00009fe0: 7269 6374 5f76 6973 6974 6f72 944e 8c0f  rict_visitor.N..
-00009ff0: 5f64 6973 6162 6c65 5f63 6f6e 6669 6794  _disable_config.
-0000a000: 4e8c 075f 736f 7572 6365 9468 288c 0c5f  N.._source.h(.._
-0000a010: 6465 7374 696e 6174 696f 6e94 4e8c 0d5f  destination.N.._
-0000a020: 636f 6e66 6967 5f66 696c 6573 945d 948c  config_files.]..
-0000a030: 1666 696c 655f 696e 7365 7274 696f 6e5f  .file_insertion_
-0000a040: 656e 6162 6c65 6494 888c 0b72 6177 5f65  enabled....raw_e
-0000a050: 6e61 626c 6564 944b 018c 116c 696e 655f  nabled.K...line_
-0000a060: 6c65 6e67 7468 5f6c 696d 6974 944d 1027  length_limit.M.'
-0000a070: 8c0e 7065 705f 7265 6665 7265 6e63 6573  ..pep_references
-0000a080: 944e 8c0c 7065 705f 6261 7365 5f75 726c  .N..pep_base_url
-0000a090: 948c 1868 7474 7073 3a2f 2f70 6570 732e  ...https://peps.
-0000a0a0: 7079 7468 6f6e 2e6f 7267 2f94 8c15 7065  python.org/...pe
-0000a0b0: 705f 6669 6c65 5f75 726c 5f74 656d 706c  p_file_url_templ
-0000a0c0: 6174 6594 8c08 7065 702d 2530 3464 948c  ate...pep-%04d..
-0000a0d0: 0e72 6663 5f72 6566 6572 656e 6365 7394  .rfc_references.
-0000a0e0: 4e8c 0c72 6663 5f62 6173 655f 7572 6c94  N..rfc_base_url.
-0000a0f0: 8c26 6874 7470 733a 2f2f 6461 7461 7472  .&https://datatr
-0000a100: 6163 6b65 722e 6965 7466 2e6f 7267 2f64  acker.ietf.org/d
-0000a110: 6f63 2f68 746d 6c2f 948c 0974 6162 5f77  oc/html/...tab_w
-0000a120: 6964 7468 944b 088c 1d74 7269 6d5f 666f  idth.K...trim_fo
-0000a130: 6f74 6e6f 7465 5f72 6566 6572 656e 6365  otnote_reference
-0000a140: 5f73 7061 6365 9489 8c10 7379 6e74 6178  _space....syntax
-0000a150: 5f68 6967 686c 6967 6874 948c 046c 6f6e  _highlight...lon
-0000a160: 6794 8c0c 736d 6172 745f 7175 6f74 6573  g...smart_quotes
-0000a170: 9488 8c13 736d 6172 7471 756f 7465 735f  ....smartquotes_
-0000a180: 6c6f 6361 6c65 7394 5d94 8c1d 6368 6172  locales.]...char
-0000a190: 6163 7465 725f 6c65 7665 6c5f 696e 6c69  acter_level_inli
-0000a1a0: 6e65 5f6d 6172 6b75 7094 898c 0e64 6f63  ne_markup....doc
-0000a1b0: 7469 746c 655f 7866 6f72 6d94 898c 0d64  title_xform....d
-0000a1c0: 6f63 696e 666f 5f78 666f 726d 944b 018c  ocinfo_xform.K..
-0000a1d0: 1273 6563 7473 7562 7469 746c 655f 7866  .sectsubtitle_xf
-0000a1e0: 6f72 6d94 898c 0d69 6d61 6765 5f6c 6f61  orm....image_loa
-0000a1f0: 6469 6e67 948c 046c 696e 6b94 8c10 656d  ding...link...em
-0000a200: 6265 645f 7374 796c 6573 6865 6574 9489  bed_stylesheet..
-0000a210: 8c15 636c 6f61 6b5f 656d 6169 6c5f 6164  ..cloak_email_ad
-0000a220: 6472 6573 7365 7394 888c 1173 6563 7469  dresses....secti
-0000a230: 6f6e 5f73 656c 665f 6c69 6e6b 9489 8c03  on_self_link....
-0000a240: 656e 7694 4e75 628c 0872 6570 6f72 7465  env.Nub..reporte
-0000a250: 7294 4e8c 1069 6e64 6972 6563 745f 7461  r.N..indirect_ta
-0000a260: 7267 6574 7394 5d94 8c11 7375 6273 7469  rgets.]...substi
-0000a270: 7475 7469 6f6e 5f64 6566 7394 7d94 8c12  tution_defs.}...
-0000a280: 7375 6273 7469 7475 7469 6f6e 5f6e 616d  substitution_nam
-0000a290: 6573 947d 948c 0872 6566 6e61 6d65 7394  es.}...refnames.
-0000a2a0: 7d94 8c06 7265 6669 6473 947d 948c 076e  }...refids.}...n
-0000a2b0: 616d 6569 6473 947d 9428 6ad2 0900 006a  ameids.}.(j....j
-0000a2c0: cf09 0000 68dd 68da 68af 68ac 6a8f 0100  ....h.h.h.h.j...
-0000a2d0: 006a 8c01 0000 6a80 0100 006a 7d01 0000  .j....j....j}...
-0000a2e0: 6ab9 0800 006a b608 0000 6a61 0200 006a  j....j....ja...j
-0000a2f0: 5e02 0000 6a4e 0200 006a 4b02 0000 6a1e  ^...jN...jK...j.
-0000a300: 0300 006a 1b03 0000 6ac6 0700 006a c307  ...j....j....j..
-0000a310: 0000 6ae2 0400 006a df04 0000 6aaa 0500  ..j....j....j...
-0000a320: 006a a705 0000 6a21 0600 006a 1e06 0000  .j....j!...j....
-0000a330: 6a98 0600 006a 9506 0000 6add 0600 006a  j....j....j....j
-0000a340: da06 0000 6abe 0700 006a bb07 0000 6ab1  ....j....j....j.
-0000a350: 0800 006a ae08 0000 6a70 0800 006a 6d08  ...j....jp...jm.
-0000a360: 0000 6aa9 0800 006a a608 0000 6a38 0900  ..j....j....j8..
-0000a370: 006a 3509 0000 6aca 0900 006a c709 0000  .j5...j....j....
-0000a380: 758c 096e 616d 6574 7970 6573 947d 9428  u..nametypes.}.(
-0000a390: 6ad2 0900 0089 68dd 8968 af88 6a8f 0100  j.....h..h..j...
-0000a3a0: 0089 6a80 0100 0088 6ab9 0800 0089 6a61  ..j.....j.....ja
-0000a3b0: 0200 0089 6a4e 0200 0088 6a1e 0300 0089  ....jN....j.....
-0000a3c0: 6ac6 0700 0089 6ae2 0400 0089 6aaa 0500  j.....j.....j...
-0000a3d0: 0089 6a21 0600 0089 6a98 0600 0089 6add  ..j!....j.....j.
-0000a3e0: 0600 0089 6abe 0700 0089 6ab1 0800 0089  ....j.....j.....
-0000a3f0: 6a70 0800 0089 6aa9 0800 0089 6a38 0900  jp....j.....j8..
-0000a400: 0089 6aca 0900 0089 7568 197d 9428 6acf  ..j.....uh.}.(j.
-0000a410: 0900 0068 2c68 da68 3f68 ac68 a66a 8c01  ...h,h.h?h.h.j..
-0000a420: 0000 68e0 6a7d 0100 006a 7701 0000 6ab6  ..h.j}...jw...j.
-0000a430: 0800 006a 9201 0000 6a5e 0200 006a ea01  ...j....j^...j..
-0000a440: 0000 6a4b 0200 006a 4502 0000 6a1b 0300  ..jK...jE...j...
-0000a450: 006a 6402 0000 6ac3 0700 006a 2103 0000  .jd...j....j!...
-0000a460: 6adf 0400 006a 0804 0000 6aa7 0500 006a  j....j....j....j
-0000a470: e504 0000 6a1e 0600 006a ad05 0000 6a95  ....j....j....j.
-0000a480: 0600 006a 2406 0000 6ada 0600 006a 9b06  ...j$...j....j..
-0000a490: 0000 6abb 0700 006a e006 0000 6aae 0800  ..j....j....j...
-0000a4a0: 006a c907 0000 6a6d 0800 006a 1a08 0000  .j....jm...j....
-0000a4b0: 6aa6 0800 006a 7308 0000 6a35 0900 006a  j....js...j5...j
-0000a4c0: bc08 0000 6ac7 0900 006a 3b09 0000 758c  ....j....j;...u.
-0000a4d0: 0d66 6f6f 746e 6f74 655f 7265 6673 947d  .footnote_refs.}
-0000a4e0: 948c 0d63 6974 6174 696f 6e5f 7265 6673  ...citation_refs
-0000a4f0: 947d 948c 0d61 7574 6f66 6f6f 746e 6f74  .}...autofootnot
-0000a500: 6573 945d 948c 1161 7574 6f66 6f6f 746e  es.]...autofootn
-0000a510: 6f74 655f 7265 6673 945d 948c 1073 796d  ote_refs.]...sym
-0000a520: 626f 6c5f 666f 6f74 6e6f 7465 7394 5d94  bol_footnotes.].
-0000a530: 8c14 7379 6d62 6f6c 5f66 6f6f 746e 6f74  ..symbol_footnot
-0000a540: 655f 7265 6673 945d 948c 0966 6f6f 746e  e_refs.]...footn
-0000a550: 6f74 6573 945d 948c 0963 6974 6174 696f  otes.]...citatio
-0000a560: 6e73 945d 948c 1261 7574 6f66 6f6f 746e  ns.]...autofootn
-0000a570: 6f74 655f 7374 6172 7494 4b01 8c15 7379  ote_start.K...sy
-0000a580: 6d62 6f6c 5f66 6f6f 746e 6f74 655f 7374  mbol_footnote_st
-0000a590: 6172 7494 4b00 8c0a 6964 5f63 6f75 6e74  art.K...id_count
-0000a5a0: 6572 948c 0b63 6f6c 6c65 6374 696f 6e73  er...collections
-0000a5b0: 948c 0743 6f75 6e74 6572 9493 947d 9485  ...Counter...}..
-0000a5c0: 9452 948c 0e70 6172 7365 5f6d 6573 7361  .R...parse_messa
-0000a5d0: 6765 7394 5d94 8c12 7472 616e 7366 6f72  ges.]...transfor
-0000a5e0: 6d5f 6d65 7373 6167 6573 945d 948c 0b74  m_messages.]...t
-0000a5f0: 7261 6e73 666f 726d 6572 944e 8c0b 696e  ransformer.N..in
-0000a600: 636c 7564 655f 6c6f 6794 5d94 8c09 696e  clude_log.]...in
-0000a610: 6465 782e 7273 7494 284e 4e4e 4e74 9486  dex.rst.(NNNNt..
-0000a620: 9461 8c0a 6465 636f 7261 7469 6f6e 944e  .a..decoration.N
-0000a630: 6826 6803 7562 2e                        h&h.ub.
+000053c0: 6829 4e75 6268 098c 0777 6172 6e69 6e67  h)Nubh...warning
+000053d0: 9493 9429 8194 7d94 2868 0558 6b01 0000  ...)..}.(h.Xk...
+000053e0: 496e 206f 7264 6572 2066 6f72 2074 6865  In order for the
+000053f0: 2050 7974 686f 6e20 696e 7465 7270 7265   Python interpre
+00005400: 7465 7220 746f 2062 6520 6162 6c65 2074  ter to be able t
+00005410: 6f20 7072 6f63 6573 7320 7468 6520 6261  o process the ba
+00005420: 7365 2063 6c61 7373 6573 2c20 7765 2068  se classes, we h
+00005430: 6176 6520 746f 2069 6d70 6f72 7420 7468  ave to import th
+00005440: 656d 2069 6e74 6f20 7468 6520 5f5f 696e  em into the __in
+00005450: 6974 5f5f 2e70 7920 6669 6c65 2069 6e20  it__.py file in 
+00005460: 7468 6520 2a2a 6261 7365 732a 2a20 6469  the **bases** di
+00005470: 7265 6374 6f72 792e 2054 6865 206f 7264  rectory. The ord
+00005480: 6572 206f 6620 7468 6520 696e 6469 7669  er of the indivi
+00005490: 6475 616c 2069 6d70 6f72 7473 2061 6c73  dual imports als
+000054a0: 6f20 6465 7465 726d 696e 6573 2074 6865  o determines the
+000054b0: 206f 7264 6572 2069 6e20 2a2a 6465 636f   order in **deco
+000054c0: 7265 2046 726f 6e74 2a2a 2e0a 0a57 6520  re Front**...We 
+000054d0: 6564 6974 2074 6865 202a 2a5f 5f69 6e69  edit the **__ini
+000054e0: 745f 5f2e 7079 2a2a 2066 696c 6520 616e  t__.py** file an
+000054f0: 6420 696e 7365 7274 2074 6865 2066 6f6c  d insert the fol
+00005500: 6c6f 7769 6e67 2063 6f64 653a 0a0a 2e2e  lowing code:....
+00005510: 2063 6f64 652d 626c 6f63 6b3a 3a20 7079   code-block:: py
+00005520: 7468 6f6e 0a0a 2020 2066 726f 6d20 2e66  thon..   from .f
+00005530: 6972 7374 5f62 6173 6520 696d 706f 7274  irst_base import
+00005540: 2046 6972 7374 5f62 6173 6594 6807 5d94   First_base.h.].
+00005550: 2868 5229 8194 7d94 2868 058c eb49 6e20  (hR)..}.(h...In 
+00005560: 6f72 6465 7220 666f 7220 7468 6520 5079  order for the Py
+00005570: 7468 6f6e 2069 6e74 6572 7072 6574 6572  thon interpreter
+00005580: 2074 6f20 6265 2061 626c 6520 746f 2070   to be able to p
+00005590: 726f 6365 7373 2074 6865 2062 6173 6520  rocess the base 
+000055a0: 636c 6173 7365 732c 2077 6520 6861 7665  classes, we have
+000055b0: 2074 6f20 696d 706f 7274 2074 6865 6d20   to import them 
+000055c0: 696e 746f 2074 6865 205f 5f69 6e69 745f  into the __init_
+000055d0: 5f2e 7079 2066 696c 6520 696e 2074 6865  _.py file in the
+000055e0: 202a 2a62 6173 6573 2a2a 2064 6972 6563   **bases** direc
+000055f0: 746f 7279 2e20 5468 6520 6f72 6465 7220  tory. The order 
+00005600: 6f66 2074 6865 2069 6e64 6976 6964 7561  of the individua
+00005610: 6c20 696d 706f 7274 7320 616c 736f 2064  l imports also d
+00005620: 6574 6572 6d69 6e65 7320 7468 6520 6f72  etermines the or
+00005630: 6465 7220 696e 202a 2a64 6563 6f72 6520  der in **decore 
+00005640: 4672 6f6e 742a 2a2e 9468 075d 9428 6811  Front**..h.].(h.
+00005650: 8c84 496e 206f 7264 6572 2066 6f72 2074  ..In order for t
+00005660: 6865 2050 7974 686f 6e20 696e 7465 7270  he Python interp
+00005670: 7265 7465 7220 746f 2062 6520 6162 6c65  reter to be able
+00005680: 2074 6f20 7072 6f63 6573 7320 7468 6520   to process the 
+00005690: 6261 7365 2063 6c61 7373 6573 2c20 7765  base classes, we
+000056a0: 2068 6176 6520 746f 2069 6d70 6f72 7420   have to import 
+000056b0: 7468 656d 2069 6e74 6f20 7468 6520 5f5f  them into the __
+000056c0: 696e 6974 5f5f 2e70 7920 6669 6c65 2069  init__.py file i
+000056d0: 6e20 7468 6520 9485 9481 947d 9428 6816  n the .....}.(h.
+000056e0: 6aab 0500 0068 2668 0368 274e 6829 4e75  j....h&h.h'Nh)Nu
+000056f0: 6268 6629 8194 7d94 2868 058c 092a 2a62  bhf)..}.(h...**b
+00005700: 6173 6573 2a2a 9468 075d 9468 118c 0562  ases**.h.].h...b
+00005710: 6173 6573 9485 9481 947d 9428 6816 6ab3  ases.....}.(h.j.
+00005720: 0500 0068 2668 0368 274e 6829 4e75 6261  ...h&h.h'Nh)Nuba
+00005730: 6817 7d94 2868 195d 9468 1b5d 9468 1d5d  h.}.(h.].h.].h.]
+00005740: 9468 1f5d 9468 215d 9475 6825 6865 6816  .h.].h!].uh%heh.
+00005750: 6aab 0500 0075 6268 118c 4d20 6469 7265  j....ubh..M dire
+00005760: 6374 6f72 792e 2054 6865 206f 7264 6572  ctory. The order
+00005770: 206f 6620 7468 6520 696e 6469 7669 6475   of the individu
+00005780: 616c 2069 6d70 6f72 7473 2061 6c73 6f20  al imports also 
+00005790: 6465 7465 726d 696e 6573 2074 6865 206f  determines the o
+000057a0: 7264 6572 2069 6e20 9485 9481 947d 9428  rder in .....}.(
+000057b0: 6816 6aab 0500 0068 2668 0368 274e 6829  h.j....h&h.h'Nh)
+000057c0: 4e75 6268 6629 8194 7d94 2868 058c 102a  Nubhf)..}.(h...*
+000057d0: 2a64 6563 6f72 6520 4672 6f6e 742a 2a94  *decore Front**.
+000057e0: 6807 5d94 6811 8c0c 6465 636f 7265 2046  h.].h...decore F
+000057f0: 726f 6e74 9485 9481 947d 9428 6816 6ac5  ront.....}.(h.j.
+00005800: 0500 0068 2668 0368 274e 6829 4e75 6261  ...h&h.h'Nh)Nuba
+00005810: 6817 7d94 2868 195d 9468 1b5d 9468 1d5d  h.}.(h.].h.].h.]
+00005820: 9468 1f5d 9468 215d 9475 6825 6865 6816  .h.].h!].uh%heh.
+00005830: 6aab 0500 0075 6268 118c 012e 9485 9481  j....ubh........
+00005840: 947d 9428 6816 6aab 0500 0068 2668 0368  .}.(h.j....h&h.h
+00005850: 274e 6829 4e75 6265 6817 7d94 2868 195d  'Nh)Nubeh.}.(h.]
+00005860: 9468 1b5d 9468 1d5d 9468 1f5d 9468 215d  .h.].h.].h.].h!]
+00005870: 9475 6825 6851 6827 6850 6829 4b7d 6816  .uh%hQh'hPh)K}h.
+00005880: 6aa7 0500 0075 6268 5229 8194 7d94 2868  j....ubhR)..}.(h
+00005890: 058c 3f57 6520 6564 6974 2074 6865 202a  ..?We edit the *
+000058a0: 2a5f 5f69 6e69 745f 5f2e 7079 2a2a 2066  *__init__.py** f
+000058b0: 696c 6520 616e 6420 696e 7365 7274 2074  ile and insert t
+000058c0: 6865 2066 6f6c 6c6f 7769 6e67 2063 6f64  he following cod
+000058d0: 653a 9468 075d 9428 6811 8c0c 5765 2065  e:.h.].(h...We e
+000058e0: 6469 7420 7468 6520 9485 9481 947d 9428  dit the .....}.(
+000058f0: 6816 6add 0500 0068 2668 0368 274e 6829  h.j....h&h.h'Nh)
+00005900: 4e75 6268 6629 8194 7d94 2868 058c 0f2a  Nubhf)..}.(h...*
+00005910: 2a5f 5f69 6e69 745f 5f2e 7079 2a2a 9468  *__init__.py**.h
+00005920: 075d 9468 118c 0b5f 5f69 6e69 745f 5f2e  .].h...__init__.
+00005930: 7079 9485 9481 947d 9428 6816 6ae5 0500  py.....}.(h.j...
+00005940: 0068 2668 0368 274e 6829 4e75 6261 6817  .h&h.h'Nh)Nubah.
+00005950: 7d94 2868 195d 9468 1b5d 9468 1d5d 9468  }.(h.].h.].h.].h
+00005960: 1f5d 9468 215d 9475 6825 6865 6816 6add  .].h!].uh%heh.j.
+00005970: 0500 0075 6268 118c 2420 6669 6c65 2061  ...ubh..$ file a
+00005980: 6e64 2069 6e73 6572 7420 7468 6520 666f  nd insert the fo
+00005990: 6c6c 6f77 696e 6720 636f 6465 3a94 8594  llowing code:...
+000059a0: 8194 7d94 2868 166a dd05 0000 6826 6803  ..}.(h.j....h&h.
+000059b0: 6827 4e68 294e 7562 6568 177d 9428 6819  h'Nh)Nubeh.}.(h.
+000059c0: 5d94 681b 5d94 681d 5d94 681f 5d94 6821  ].h.].h.].h.].h!
+000059d0: 5d94 7568 2568 5168 2768 5068 294b 7f68  ].uh%hQh'hPh)K.h
+000059e0: 166a a705 0000 7562 6a18 0200 0029 8194  .j....ubj....)..
+000059f0: 7d94 2868 058c 2266 726f 6d20 2e66 6972  }.(h.."from .fir
+00005a00: 7374 5f62 6173 6520 696d 706f 7274 2046  st_base import F
+00005a10: 6972 7374 5f62 6173 6594 6807 5d94 6811  irst_base.h.].h.
+00005a20: 8c22 6672 6f6d 202e 6669 7273 745f 6261  ."from .first_ba
+00005a30: 7365 2069 6d70 6f72 7420 4669 7273 745f  se import First_
+00005a40: 6261 7365 9485 9481 947d 9468 166a fd05  base.....}.h.j..
+00005a50: 0000 7362 6168 177d 9428 6819 5d94 681b  ..sbah.}.(h.].h.
+00005a60: 5d94 681d 5d94 681f 5d94 6821 5d94 6823  ].h.].h.].h!].h#
+00005a70: 6824 6a27 0200 0089 6a28 0200 008c 0670  h$j'....j(.....p
+00005a80: 7974 686f 6e94 6a2a 0200 007d 9475 6825  ython.j*...}.uh%
+00005a90: 6a17 0200 0068 2768 5068 294b 8168 166a  j....h'hPh)K.h.j
+00005aa0: a705 0000 7562 6568 177d 9428 6819 5d94  ....ubeh.}.(h.].
+00005ab0: 681b 5d94 681d 5d94 681f 5d94 6821 5d94  h.].h.].h.].h!].
+00005ac0: 7568 256a a505 0000 6816 6ae5 0400 0068  uh%j....h.j....h
+00005ad0: 2668 0368 274e 6829 4e75 6265 6817 7d94  &h.h'Nh)Nubeh.}.
+00005ae0: 2868 195d 948c 0462 6173 6594 6168 1b5d  (h.]...base.ah.]
+00005af0: 9468 1d5d 948c 0462 6173 6594 6168 1f5d  .h.]...base.ah.]
+00005b00: 9468 215d 9475 6825 682a 6816 6a21 0300  .h!].uh%h*h.j!..
+00005b10: 0068 2668 0368 2768 5068 294b 6a75 6268  .h&h.h'hPh)Kjubh
+00005b20: 2b29 8194 7d94 2868 0568 0668 075d 9428  +)..}.(h.h.h.].(
+00005b30: 6830 2981 947d 9428 6805 8c04 5669 6577  h0)..}.(h...View
+00005b40: 9468 075d 9468 118c 0456 6965 7794 8594  .h.].h...View...
+00005b50: 8194 7d94 2868 166a 1e06 0000 6826 6803  ..}.(h.j....h&h.
+00005b60: 6827 4e68 294e 7562 6168 177d 9428 6819  h'Nh)Nubah.}.(h.
+00005b70: 5d94 681b 5d94 681d 5d94 681f 5d94 6821  ].h.].h.].h.].h!
+00005b80: 5d94 7568 2568 2f68 166a 1b06 0000 6826  ].uh%h/h.j....h&
+00005b90: 6803 6827 6850 6829 4b86 7562 6852 2981  h.h'hPh)K.ubhR).
+00005ba0: 947d 9428 6805 8c6a 5669 6577 7320 6172  .}.(h..jViews ar
+00005bb0: 6520 7573 6564 2062 7920 7468 6520 6465  e used by the de
+00005bc0: 636f 7265 2061 7070 6c69 6361 7469 6f6e  core application
+00005bd0: 2074 6f20 7072 6573 656e 7420 7468 6520   to present the 
+00005be0: 6461 7461 2073 6574 7320 696e 2074 6865  data sets in the
+00005bf0: 202a 2a64 6563 6f72 6520 4672 6f6e 742a   **decore Front*
+00005c00: 2a20 7765 6220 6170 706c 6963 6174 696f  * web applicatio
+00005c10: 6e2e 9468 075d 9428 6811 8c49 5669 6577  n..h.].(h..IView
+00005c20: 7320 6172 6520 7573 6564 2062 7920 7468  s are used by th
+00005c30: 6520 6465 636f 7265 2061 7070 6c69 6361  e decore applica
+00005c40: 7469 6f6e 2074 6f20 7072 6573 656e 7420  tion to present 
+00005c50: 7468 6520 6461 7461 2073 6574 7320 696e  the data sets in
+00005c60: 2074 6865 2094 8594 8194 7d94 2868 166a   the .....}.(h.j
+00005c70: 2c06 0000 6826 6803 6827 4e68 294e 7562  ,...h&h.h'Nh)Nub
+00005c80: 6866 2981 947d 9428 6805 8c10 2a2a 6465  hf)..}.(h...**de
+00005c90: 636f 7265 2046 726f 6e74 2a2a 9468 075d  core Front**.h.]
+00005ca0: 9468 118c 0c64 6563 6f72 6520 4672 6f6e  .h...decore Fron
+00005cb0: 7494 8594 8194 7d94 2868 166a 3406 0000  t.....}.(h.j4...
+00005cc0: 6826 6803 6827 4e68 294e 7562 6168 177d  h&h.h'Nh)Nubah.}
+00005cd0: 9428 6819 5d94 681b 5d94 681d 5d94 681f  .(h.].h.].h.].h.
+00005ce0: 5d94 6821 5d94 7568 2568 6568 166a 2c06  ].h!].uh%heh.j,.
+00005cf0: 0000 7562 6811 8c11 2077 6562 2061 7070  ..ubh... web app
+00005d00: 6c69 6361 7469 6f6e 2e94 8594 8194 7d94  lication......}.
+00005d10: 2868 166a 2c06 0000 6826 6803 6827 4e68  (h.j,...h&h.h'Nh
+00005d20: 294e 7562 6568 177d 9428 6819 5d94 681b  )Nubeh.}.(h.].h.
+00005d30: 5d94 681d 5d94 681f 5d94 6821 5d94 7568  ].h.].h.].h!].uh
+00005d40: 2568 5168 2768 5068 294b 8768 166a 1b06  %hQh'hPh)K.h.j..
+00005d50: 0000 6826 6803 7562 6852 2981 947d 9428  ..h&h.ubhR)..}.(
+00005d60: 6805 8c6c 5769 7468 2074 6865 2076 6965  h..lWith the vie
+00005d70: 7720 6465 636f 7261 746f 7220 7765 2063  w decorator we c
+00005d80: 616e 206e 6f77 2063 7265 6174 6520 6120  an now create a 
+00005d90: 7669 6577 2063 6f6d 706f 6e65 6e74 2061  view component a
+00005da0: 6e64 206c 696e 6b20 6974 2074 6f20 7468  nd link it to th
+00005db0: 6520 7072 6576 696f 7573 6c79 2063 7265  e previously cre
+00005dc0: 6174 6564 2062 6173 6520 636c 6173 732e  ated base class.
+00005dd0: 9468 075d 9468 118c 6c57 6974 6820 7468  .h.].h..lWith th
+00005de0: 6520 7669 6577 2064 6563 6f72 6174 6f72  e view decorator
+00005df0: 2077 6520 6361 6e20 6e6f 7720 6372 6561   we can now crea
+00005e00: 7465 2061 2076 6965 7720 636f 6d70 6f6e  te a view compon
+00005e10: 656e 7420 616e 6420 6c69 6e6b 2069 7420  ent and link it 
+00005e20: 746f 2074 6865 2070 7265 7669 6f75 736c  to the previousl
+00005e30: 7920 6372 6561 7465 6420 6261 7365 2063  y created base c
+00005e40: 6c61 7373 2e94 8594 8194 7d94 2868 166a  lass......}.(h.j
+00005e50: 4c06 0000 6826 6803 6827 4e68 294e 7562  L...h&h.h'Nh)Nub
+00005e60: 6168 177d 9428 6819 5d94 681b 5d94 681d  ah.}.(h.].h.].h.
+00005e70: 5d94 681f 5d94 6821 5d94 7568 2568 5168  ].h.].h!].uh%hQh
+00005e80: 2768 5068 294b 8968 166a 1b06 0000 6826  'hPh)K.h.j....h&
+00005e90: 6803 7562 6852 2981 947d 9428 6805 8c4c  h.ubhR)..}.(h..L
+00005ea0: 5765 206e 6f77 2065 6469 7420 7468 6520  We now edit the 
+00005eb0: 2a2a 6669 7273 745f 6261 7365 2e70 792a  **first_base.py*
+00005ec0: 2a20 6669 6c65 2061 6761 696e 2061 6e64  * file again and
+00005ed0: 2065 7874 656e 6420 7468 6520 636f 6465   extend the code
+00005ee0: 2061 7320 666f 6c6c 6f77 733a 9468 075d   as follows:.h.]
+00005ef0: 9428 6811 8c10 5765 206e 6f77 2065 6469  .(h...We now edi
+00005f00: 7420 7468 6520 9485 9481 947d 9428 6816  t the .....}.(h.
+00005f10: 6a5a 0600 0068 2668 0368 274e 6829 4e75  jZ...h&h.h'Nh)Nu
+00005f20: 6268 6629 8194 7d94 2868 058c 112a 2a66  bhf)..}.(h...**f
+00005f30: 6972 7374 5f62 6173 652e 7079 2a2a 9468  irst_base.py**.h
+00005f40: 075d 9468 118c 0d66 6972 7374 5f62 6173  .].h...first_bas
+00005f50: 652e 7079 9485 9481 947d 9428 6816 6a62  e.py.....}.(h.jb
+00005f60: 0600 0068 2668 0368 274e 6829 4e75 6261  ...h&h.h'Nh)Nuba
+00005f70: 6817 7d94 2868 195d 9468 1b5d 9468 1d5d  h.}.(h.].h.].h.]
+00005f80: 9468 1f5d 9468 215d 9475 6825 6865 6816  .h.].h!].uh%heh.
+00005f90: 6a5a 0600 0075 6268 118c 2b20 6669 6c65  jZ...ubh..+ file
+00005fa0: 2061 6761 696e 2061 6e64 2065 7874 656e   again and exten
+00005fb0: 6420 7468 6520 636f 6465 2061 7320 666f  d the code as fo
+00005fc0: 6c6c 6f77 733a 9485 9481 947d 9428 6816  llows:.....}.(h.
+00005fd0: 6a5a 0600 0068 2668 0368 274e 6829 4e75  jZ...h&h.h'Nh)Nu
+00005fe0: 6265 6817 7d94 2868 195d 9468 1b5d 9468  beh.}.(h.].h.].h
+00005ff0: 1d5d 9468 1f5d 9468 215d 9475 6825 6851  .].h.].h!].uh%hQ
+00006000: 6827 6850 6829 4b8b 6816 6a1b 0600 0068  h'hPh)K.h.j....h
+00006010: 2668 0375 626a 1802 0000 2981 947d 9428  &h.ubj....)..}.(
+00006020: 6805 583a 0100 0066 726f 6d20 6465 636f  h.X:...from deco
+00006030: 7265 5f62 6173 6520 696d 706f 7274 2064  re_base import d
+00006040: 6563 6f72 650a 6672 6f6d 206d 6f64 656c  ecore.from model
+00006050: 732e 6669 7273 745f 6d6f 6465 6c20 696d  s.first_model im
+00006060: 706f 7274 2046 6972 7374 5f6d 6f64 656c  port First_model
+00006070: 0a0a 4064 6563 6f72 652e 6261 7365 2874  ..@decore.base(t
+00006080: 6974 6c65 3d27 4669 7273 7420 4261 7365  itle='First Base
+00006090: 272c 2069 636f 6e3d 276d 6469 2d68 6f6d  ', icon='mdi-hom
+000060a0: 6527 2c20 6d6f 6465 6c3d 4669 7273 745f  e', model=First_
+000060b0: 6d6f 6465 6c29 0a63 6c61 7373 2046 6972  model).class Fir
+000060c0: 7374 5f62 6173 653a 0a20 2020 4064 6563  st_base:.   @dec
+000060d0: 6f72 652e 7669 6577 2874 6974 6c65 3d27  ore.view(title='
+000060e0: 4669 7273 7420 5669 6577 272c 2069 636f  First View', ico
+000060f0: 6e3d 276d 6469 2d68 6f6d 6527 2c20 7479  n='mdi-home', ty
+00006100: 7065 3d27 7461 626c 6527 2c20 6669 656c  pe='table', fiel
+00006110: 6473 3d5b 4669 7273 745f 6d6f 6465 6c2e  ds=[First_model.
+00006120: 6669 7273 746e 616d 652c 2046 6972 7374  firstname, First
+00006130: 5f6d 6f64 656c 2e6c 6173 746e 616d 655d  _model.lastname]
+00006140: 290a 2020 2064 6566 2066 6972 7374 5f76  ).   def first_v
+00006150: 6965 7728 293a 0a20 2020 2020 2070 6173  iew():.      pas
+00006160: 7394 6807 5d94 6811 583a 0100 0066 726f  s.h.].h.X:...fro
+00006170: 6d20 6465 636f 7265 5f62 6173 6520 696d  m decore_base im
+00006180: 706f 7274 2064 6563 6f72 650a 6672 6f6d  port decore.from
+00006190: 206d 6f64 656c 732e 6669 7273 745f 6d6f   models.first_mo
+000061a0: 6465 6c20 696d 706f 7274 2046 6972 7374  del import First
+000061b0: 5f6d 6f64 656c 0a0a 4064 6563 6f72 652e  _model..@decore.
+000061c0: 6261 7365 2874 6974 6c65 3d27 4669 7273  base(title='Firs
+000061d0: 7420 4261 7365 272c 2069 636f 6e3d 276d  t Base', icon='m
+000061e0: 6469 2d68 6f6d 6527 2c20 6d6f 6465 6c3d  di-home', model=
+000061f0: 4669 7273 745f 6d6f 6465 6c29 0a63 6c61  First_model).cla
+00006200: 7373 2046 6972 7374 5f62 6173 653a 0a20  ss First_base:. 
+00006210: 2020 4064 6563 6f72 652e 7669 6577 2874    @decore.view(t
+00006220: 6974 6c65 3d27 4669 7273 7420 5669 6577  itle='First View
+00006230: 272c 2069 636f 6e3d 276d 6469 2d68 6f6d  ', icon='mdi-hom
+00006240: 6527 2c20 7479 7065 3d27 7461 626c 6527  e', type='table'
+00006250: 2c20 6669 656c 6473 3d5b 4669 7273 745f  , fields=[First_
+00006260: 6d6f 6465 6c2e 6669 7273 746e 616d 652c  model.firstname,
+00006270: 2046 6972 7374 5f6d 6f64 656c 2e6c 6173   First_model.las
+00006280: 746e 616d 655d 290a 2020 2064 6566 2066  tname]).   def f
+00006290: 6972 7374 5f76 6965 7728 293a 0a20 2020  irst_view():.   
+000062a0: 2020 2070 6173 7394 8594 8194 7d94 6816     pass.....}.h.
+000062b0: 6a7a 0600 0073 6261 6817 7d94 2868 195d  jz...sbah.}.(h.]
+000062c0: 9468 1b5d 9468 1d5d 9468 1f5d 9468 215d  .h.].h.].h.].h!]
+000062d0: 9468 2368 246a 2702 0000 896a 2802 0000  .h#h$j'....j(...
+000062e0: 8c06 7079 7468 6f6e 946a 2a02 0000 7d94  ..python.j*...}.
+000062f0: 7568 256a 1702 0000 6827 6850 6829 4b8d  uh%j....h'hPh)K.
+00006300: 6816 6a1b 0600 0068 2668 0375 6265 6817  h.j....h&h.ubeh.
+00006310: 7d94 2868 195d 948c 0476 6965 7794 6168  }.(h.]...view.ah
+00006320: 1b5d 9468 1d5d 948c 0476 6965 7794 6168  .].h.]...view.ah
+00006330: 1f5d 9468 215d 9475 6825 682a 6816 6a21  .].h!].uh%h*h.j!
+00006340: 0300 0068 2668 0368 2768 5068 294b 8675  ...h&h.h'hPh)K.u
+00006350: 6268 2b29 8194 7d94 2868 0568 0668 075d  bh+)..}.(h.h.h.]
+00006360: 9428 6830 2981 947d 9428 6805 8c06 4469  .(h0)..}.(h...Di
+00006370: 616c 6f67 9468 075d 9468 118c 0644 6961  alog.h.].h...Dia
+00006380: 6c6f 6794 8594 8194 7d94 2868 166a 9506  log.....}.(h.j..
+00006390: 0000 6826 6803 6827 4e68 294e 7562 6168  ..h&h.h'Nh)Nubah
+000063a0: 177d 9428 6819 5d94 681b 5d94 681d 5d94  .}.(h.].h.].h.].
+000063b0: 681f 5d94 6821 5d94 7568 2568 2f68 166a  h.].h!].uh%h/h.j
+000063c0: 9206 0000 6826 6803 6827 6850 6829 4b99  ....h&h.h'hPh)K.
+000063d0: 7562 6852 2981 947d 9428 6805 8cfb 4469  ubhR)..}.(h...Di
+000063e0: 616c 6f67 7320 6172 6520 7468 6520 7375  alogs are the su
+000063f0: 7070 6f72 7469 6e67 2065 6c65 6d65 6e74  pporting element
+00006400: 7320 666f 7220 7769 6467 6574 7320 696e  s for widgets in
+00006410: 2074 6865 202a 2a64 6563 6f72 6520 4672   the **decore Fr
+00006420: 6f6e 742a 2a20 7765 6220 6170 706c 6963  ont** web applic
+00006430: 6174 696f 6e2e 2054 6865 7920 6361 6e20  ation. They can 
+00006440: 6f6e 6c79 2062 6520 6164 6465 6420 746f  only be added to
+00006450: 2076 6965 7773 2061 6e64 2063 6f6e 7472   views and contr
+00006460: 6f6c 2074 6865 2076 6973 6962 696c 6974  ol the visibilit
+00006470: 7920 616e 6420 6469 7370 6c61 7920 7374  y and display st
+00006480: 796c 6520 6f66 2063 6869 6c64 2065 6c65  yle of child ele
+00006490: 6d65 6e74 732e 2044 6961 6c6f 6773 2061  ments. Dialogs a
+000064a0: 6c73 6f20 6765 7420 636f 6e74 726f 6c20  lso get control 
+000064b0: 6f76 6572 2074 6865 2073 7562 6d69 7420  over the submit 
+000064c0: 6675 6e63 7469 6f6e 7320 6f66 2074 6865  functions of the
+000064d0: 2077 6964 6765 7473 2e94 6807 5d94 2868   widgets..h.].(h
+000064e0: 118c 3744 6961 6c6f 6773 2061 7265 2074  ..7Dialogs are t
+000064f0: 6865 2073 7570 706f 7274 696e 6720 656c  he supporting el
+00006500: 656d 656e 7473 2066 6f72 2077 6964 6765  ements for widge
+00006510: 7473 2069 6e20 7468 6520 9485 9481 947d  ts in the .....}
+00006520: 9428 6816 6aa3 0600 0068 2668 0368 274e  .(h.j....h&h.h'N
+00006530: 6829 4e75 6268 6629 8194 7d94 2868 058c  h)Nubhf)..}.(h..
+00006540: 102a 2a64 6563 6f72 6520 4672 6f6e 742a  .**decore Front*
+00006550: 2a94 6807 5d94 6811 8c0c 6465 636f 7265  *.h.].h...decore
+00006560: 2046 726f 6e74 9485 9481 947d 9428 6816   Front.....}.(h.
+00006570: 6aab 0600 0068 2668 0368 274e 6829 4e75  j....h&h.h'Nh)Nu
+00006580: 6261 6817 7d94 2868 195d 9468 1b5d 9468  bah.}.(h.].h.].h
+00006590: 1d5d 9468 1f5d 9468 215d 9475 6825 6865  .].h.].h!].uh%he
+000065a0: 6816 6aa3 0600 0075 6268 118c b420 7765  h.j....ubh... we
+000065b0: 6220 6170 706c 6963 6174 696f 6e2e 2054  b application. T
+000065c0: 6865 7920 6361 6e20 6f6e 6c79 2062 6520  hey can only be 
+000065d0: 6164 6465 6420 746f 2076 6965 7773 2061  added to views a
+000065e0: 6e64 2063 6f6e 7472 6f6c 2074 6865 2076  nd control the v
+000065f0: 6973 6962 696c 6974 7920 616e 6420 6469  isibility and di
+00006600: 7370 6c61 7920 7374 796c 6520 6f66 2063  splay style of c
+00006610: 6869 6c64 2065 6c65 6d65 6e74 732e 2044  hild elements. D
+00006620: 6961 6c6f 6773 2061 6c73 6f20 6765 7420  ialogs also get 
+00006630: 636f 6e74 726f 6c20 6f76 6572 2074 6865  control over the
+00006640: 2073 7562 6d69 7420 6675 6e63 7469 6f6e   submit function
+00006650: 7320 6f66 2074 6865 2077 6964 6765 7473  s of the widgets
+00006660: 2e94 8594 8194 7d94 2868 166a a306 0000  ......}.(h.j....
+00006670: 6826 6803 6827 4e68 294e 7562 6568 177d  h&h.h'Nh)Nubeh.}
+00006680: 9428 6819 5d94 681b 5d94 681d 5d94 681f  .(h.].h.].h.].h.
+00006690: 5d94 6821 5d94 7568 2568 5168 2768 5068  ].h!].uh%hQh'hPh
+000066a0: 294b 9a68 166a 9206 0000 6826 6803 7562  )K.h.j....h&h.ub
+000066b0: 6852 2981 947d 9428 6805 8c55 496e 206f  hR)..}.(h..UIn o
+000066c0: 7572 2063 6173 652c 2077 6520 6372 6561  ur case, we crea
+000066d0: 7465 2061 2064 6961 6f6c 6720 746f 2063  te a diaolg to c
+000066e0: 7265 6174 6520 6120 6e65 7720 7065 7273  reate a new pers
+000066f0: 6f6e 2077 6974 6820 6669 7273 7420 6e61  on with first na
+00006700: 6d65 2061 6e64 206c 6173 7420 6e61 6d65  me and last name
+00006710: 2e94 6807 5d94 6811 8c55 496e 206f 7572  ..h.].h..UIn our
+00006720: 2063 6173 652c 2077 6520 6372 6561 7465   case, we create
+00006730: 2061 2064 6961 6f6c 6720 746f 2063 7265   a diaolg to cre
+00006740: 6174 6520 6120 6e65 7720 7065 7273 6f6e  ate a new person
+00006750: 2077 6974 6820 6669 7273 7420 6e61 6d65   with first name
+00006760: 2061 6e64 206c 6173 7420 6e61 6d65 2e94   and last name..
+00006770: 8594 8194 7d94 2868 166a c306 0000 6826  ....}.(h.j....h&
+00006780: 6803 6827 4e68 294e 7562 6168 177d 9428  h.h'Nh)Nubah.}.(
+00006790: 6819 5d94 681b 5d94 681d 5d94 681f 5d94  h.].h.].h.].h.].
+000067a0: 6821 5d94 7568 2568 5168 2768 5068 294b  h!].uh%hQh'hPh)K
+000067b0: 9c68 166a 9206 0000 6826 6803 7562 6852  .h.j....h&h.ubhR
+000067c0: 2981 947d 9428 6805 8c4f 4865 7265 2077  )..}.(h..OHere w
+000067d0: 6520 676f 202e 2e2e 2061 6761 696e 2074  e go ... again t
+000067e0: 6865 2066 696c 6520 2a2a 6669 7273 745f  he file **first_
+000067f0: 6261 7365 2e70 792a 2a20 616e 6420 6578  base.py** and ex
+00006800: 7465 6e64 2074 6865 2063 6f64 6520 6173  tend the code as
+00006810: 2066 6f6c 6c6f 7773 3a94 6807 5d94 2868   follows:.h.].(h
+00006820: 118c 1e48 6572 6520 7765 2067 6f20 e280  ...Here we go ..
+00006830: a620 6167 6169 6e20 7468 6520 6669 6c65  . again the file
+00006840: 2094 8594 8194 7d94 2868 166a d106 0000   .....}.(h.j....
+00006850: 6826 6803 6827 4e68 294e 7562 6866 2981  h&h.h'Nh)Nubhf).
+00006860: 947d 9428 6805 8c11 2a2a 6669 7273 745f  .}.(h...**first_
+00006870: 6261 7365 2e70 792a 2a94 6807 5d94 6811  base.py**.h.].h.
+00006880: 8c0d 6669 7273 745f 6261 7365 2e70 7994  ..first_base.py.
+00006890: 8594 8194 7d94 2868 166a d906 0000 6826  ....}.(h.j....h&
+000068a0: 6803 6827 4e68 294e 7562 6168 177d 9428  h.h'Nh)Nubah.}.(
+000068b0: 6819 5d94 681b 5d94 681d 5d94 681f 5d94  h.].h.].h.].h.].
+000068c0: 6821 5d94 7568 2568 6568 166a d106 0000  h!].uh%heh.j....
+000068d0: 7562 6811 8c20 2061 6e64 2065 7874 656e  ubh..  and exten
+000068e0: 6420 7468 6520 636f 6465 2061 7320 666f  d the code as fo
+000068f0: 6c6c 6f77 733a 9485 9481 947d 9428 6816  llows:.....}.(h.
+00006900: 6ad1 0600 0068 2668 0368 274e 6829 4e75  j....h&h.h'Nh)Nu
+00006910: 6265 6817 7d94 2868 195d 9468 1b5d 9468  beh.}.(h.].h.].h
+00006920: 1d5d 9468 1f5d 9468 215d 9475 6825 6851  .].h.].h!].uh%hQ
+00006930: 6827 6850 6829 4b9e 6816 6a92 0600 0068  h'hPh)K.h.j....h
+00006940: 2668 0375 626a 1802 0000 2981 947d 9428  &h.ubj....)..}.(
+00006950: 6805 58d0 0100 0066 726f 6d20 6465 636f  h.X....from deco
+00006960: 7265 5f62 6173 6520 696d 706f 7274 2064  re_base import d
+00006970: 6563 6f72 650a 6672 6f6d 206d 6f64 656c  ecore.from model
+00006980: 732e 6669 7273 745f 6d6f 6465 6c20 696d  s.first_model im
+00006990: 706f 7274 2046 6972 7374 5f6d 6f64 656c  port First_model
+000069a0: 0a0a 4064 6563 6f72 652e 6261 7365 2874  ..@decore.base(t
+000069b0: 6974 6c65 3d27 4d79 2046 6972 7374 2042  itle='My First B
+000069c0: 6173 6527 2c20 6963 6f6e 3d27 6d64 692d  ase', icon='mdi-
+000069d0: 686f 6d65 272c 206d 6f64 656c 3d46 6972  home', model=Fir
+000069e0: 7374 5f6d 6f64 656c 290a 636c 6173 7320  st_model).class 
+000069f0: 4669 7273 745f 6261 7365 3a0a 2020 2040  First_base:.   @
+00006a00: 6465 636f 7265 2e76 6965 7728 7469 746c  decore.view(titl
+00006a10: 653d 2750 6572 736f 6e27 2c20 6963 6f6e  e='Person', icon
+00006a20: 3d27 6d64 692d 6163 636f 756e 7427 2c20  ='mdi-account', 
+00006a30: 7479 7065 3d27 7461 626c 6527 2c20 6669  type='table', fi
+00006a40: 656c 6473 3d5b 4669 7273 745f 6d6f 6465  elds=[First_mode
+00006a50: 6c2e 6669 7273 746e 616d 652c 2046 6972  l.firstname, Fir
+00006a60: 7374 5f6d 6f64 656c 2e6c 6173 746e 616d  st_model.lastnam
+00006a70: 655d 290a 2020 2064 6566 2066 6972 7374  e]).   def first
+00006a80: 5f76 6965 7728 293a 0a20 2020 2020 2040  _view():.      @
+00006a90: 6465 636f 7265 2e64 6961 6c6f 6728 7469  decore.dialog(ti
+00006aa0: 746c 653d 2741 6464 2050 6572 736f 6e27  tle='Add Person'
+00006ab0: 2c20 6963 6f6e 3d27 6d64 692d 706c 7573  , icon='mdi-plus
+00006ac0: 272c 2074 7970 653d 2773 7461 6e64 6172  ', type='standar
+00006ad0: 6427 2c20 6469 7370 6c61 793d 2764 7261  d', display='dra
+00006ae0: 7765 7227 2c20 6163 7469 7661 746f 723d  wer', activator=
+00006af0: 2764 6566 6175 6c74 2d6d 656e 7527 290a  'default-menu').
+00006b00: 2020 2020 2020 6465 6620 6669 7273 745f        def first_
+00006b10: 6469 616c 6f67 2829 3a0a 2020 2020 2020  dialog():.      
+00006b20: 2020 2070 6173 7394 6807 5d94 6811 58d0     pass.h.].h.X.
+00006b30: 0100 0066 726f 6d20 6465 636f 7265 5f62  ...from decore_b
+00006b40: 6173 6520 696d 706f 7274 2064 6563 6f72  ase import decor
+00006b50: 650a 6672 6f6d 206d 6f64 656c 732e 6669  e.from models.fi
+00006b60: 7273 745f 6d6f 6465 6c20 696d 706f 7274  rst_model import
+00006b70: 2046 6972 7374 5f6d 6f64 656c 0a0a 4064   First_model..@d
+00006b80: 6563 6f72 652e 6261 7365 2874 6974 6c65  ecore.base(title
+00006b90: 3d27 4d79 2046 6972 7374 2042 6173 6527  ='My First Base'
+00006ba0: 2c20 6963 6f6e 3d27 6d64 692d 686f 6d65  , icon='mdi-home
+00006bb0: 272c 206d 6f64 656c 3d46 6972 7374 5f6d  ', model=First_m
+00006bc0: 6f64 656c 290a 636c 6173 7320 4669 7273  odel).class Firs
+00006bd0: 745f 6261 7365 3a0a 2020 2040 6465 636f  t_base:.   @deco
+00006be0: 7265 2e76 6965 7728 7469 746c 653d 2750  re.view(title='P
+00006bf0: 6572 736f 6e27 2c20 6963 6f6e 3d27 6d64  erson', icon='md
+00006c00: 692d 6163 636f 756e 7427 2c20 7479 7065  i-account', type
+00006c10: 3d27 7461 626c 6527 2c20 6669 656c 6473  ='table', fields
+00006c20: 3d5b 4669 7273 745f 6d6f 6465 6c2e 6669  =[First_model.fi
+00006c30: 7273 746e 616d 652c 2046 6972 7374 5f6d  rstname, First_m
+00006c40: 6f64 656c 2e6c 6173 746e 616d 655d 290a  odel.lastname]).
+00006c50: 2020 2064 6566 2066 6972 7374 5f76 6965     def first_vie
+00006c60: 7728 293a 0a20 2020 2020 2040 6465 636f  w():.      @deco
+00006c70: 7265 2e64 6961 6c6f 6728 7469 746c 653d  re.dialog(title=
+00006c80: 2741 6464 2050 6572 736f 6e27 2c20 6963  'Add Person', ic
+00006c90: 6f6e 3d27 6d64 692d 706c 7573 272c 2074  on='mdi-plus', t
+00006ca0: 7970 653d 2773 7461 6e64 6172 6427 2c20  ype='standard', 
+00006cb0: 6469 7370 6c61 793d 2764 7261 7765 7227  display='drawer'
+00006cc0: 2c20 6163 7469 7661 746f 723d 2764 6566  , activator='def
+00006cd0: 6175 6c74 2d6d 656e 7527 290a 2020 2020  ault-menu').    
+00006ce0: 2020 6465 6620 6669 7273 745f 6469 616c    def first_dial
+00006cf0: 6f67 2829 3a0a 2020 2020 2020 2020 2070  og():.         p
+00006d00: 6173 7394 8594 8194 7d94 6816 6af1 0600  ass.....}.h.j...
+00006d10: 0073 6261 6817 7d94 2868 195d 9468 1b5d  .sbah.}.(h.].h.]
+00006d20: 9468 1d5d 9468 1f5d 9468 215d 9468 2368  .h.].h.].h!].h#h
+00006d30: 246a 2702 0000 896a 2802 0000 8c06 7079  $j'....j(.....py
+00006d40: 7468 6f6e 946a 2a02 0000 7d94 7568 256a  thon.j*...}.uh%j
+00006d50: 1702 0000 6827 6850 6829 4ba0 6816 6a92  ....h'hPh)K.h.j.
+00006d60: 0600 0068 2668 0375 6265 6817 7d94 2868  ...h&h.ubeh.}.(h
+00006d70: 195d 948c 0664 6961 6c6f 6794 6168 1b5d  .]...dialog.ah.]
+00006d80: 9468 1d5d 948c 0664 6961 6c6f 6794 6168  .h.]...dialog.ah
+00006d90: 1f5d 9468 215d 9475 6825 682a 6816 6a21  .].h!].uh%h*h.j!
+00006da0: 0300 0068 2668 0368 2768 5068 294b 9975  ...h&h.h'hPh)K.u
+00006db0: 6268 2b29 8194 7d94 2868 0568 0668 075d  bh+)..}.(h.h.h.]
+00006dc0: 9428 6830 2981 947d 9428 6805 8c06 5769  .(h0)..}.(h...Wi
+00006dd0: 6467 6574 9468 075d 9468 118c 0657 6964  dget.h.].h...Wid
+00006de0: 6765 7494 8594 8194 7d94 2868 166a 0c07  get.....}.(h.j..
+00006df0: 0000 6826 6803 6827 4e68 294e 7562 6168  ..h&h.h'Nh)Nubah
+00006e00: 177d 9428 6819 5d94 681b 5d94 681d 5d94  .}.(h.].h.].h.].
+00006e10: 681f 5d94 6821 5d94 7568 2568 2f68 166a  h.].h!].uh%h/h.j
+00006e20: 0907 0000 6826 6803 6827 6850 6829 4bae  ....h&h.h'hPh)K.
+00006e30: 7562 6852 2981 947d 9428 6805 8c88 5769  ubhR)..}.(h...Wi
+00006e40: 6467 6574 7320 6172 6520 636f 6d70 6f6e  dgets are compon
+00006e50: 656e 7473 2077 6974 6820 7768 6963 6820  ents with which 
+00006e60: 7765 2063 616e 2070 6572 666f 726d 2069  we can perform i
+00006e70: 6e74 6572 6163 7469 6f6e 7320 6f6e 2074  nteractions on t
+00006e80: 6865 2073 696e 676c 6520 7265 636f 7264  he single record
+00006e90: 2e20 5468 6579 2063 616e 206f 6e6c 7920  . They can only 
+00006ea0: 6265 2061 6464 6564 2074 6f20 6469 616c  be added to dial
+00006eb0: 6f67 7320 616e 6420 6172 6520 7374 6163  ogs and are stac
+00006ec0: 6b61 626c 652e 9468 075d 9468 118c 8857  kable..h.].h...W
+00006ed0: 6964 6765 7473 2061 7265 2063 6f6d 706f  idgets are compo
+00006ee0: 6e65 6e74 7320 7769 7468 2077 6869 6368  nents with which
+00006ef0: 2077 6520 6361 6e20 7065 7266 6f72 6d20   we can perform 
+00006f00: 696e 7465 7261 6374 696f 6e73 206f 6e20  interactions on 
+00006f10: 7468 6520 7369 6e67 6c65 2072 6563 6f72  the single recor
+00006f20: 642e 2054 6865 7920 6361 6e20 6f6e 6c79  d. They can only
+00006f30: 2062 6520 6164 6465 6420 746f 2064 6961   be added to dia
+00006f40: 6c6f 6773 2061 6e64 2061 7265 2073 7461  logs and are sta
+00006f50: 636b 6162 6c65 2e94 8594 8194 7d94 2868  ckable......}.(h
+00006f60: 166a 1a07 0000 6826 6803 6827 4e68 294e  .j....h&h.h'Nh)N
+00006f70: 7562 6168 177d 9428 6819 5d94 681b 5d94  ubah.}.(h.].h.].
+00006f80: 681d 5d94 681f 5d94 6821 5d94 7568 2568  h.].h.].h!].uh%h
+00006f90: 5168 2768 5068 294b af68 166a 0907 0000  Qh'hPh)K.h.j....
+00006fa0: 6826 6803 7562 6852 2981 947d 9428 6805  h&h.ubhR)..}.(h.
+00006fb0: 8c51 5768 6174 2077 6520 6e65 6564 206e  .QWhat we need n
+00006fc0: 6f77 2069 7320 746f 2063 7265 6174 6520  ow is to create 
+00006fd0: 616e 2069 6e70 7574 2066 6f72 6d20 746f  an input form to
+00006fe0: 2065 6e74 6572 2074 6865 2064 6174 6120   enter the data 
+00006ff0: 666f 7220 7468 6520 6e65 7720 7065 7273  for the new pers
+00007000: 6f6e 2e94 6807 5d94 6811 8c51 5768 6174  on..h.].h..QWhat
+00007010: 2077 6520 6e65 6564 206e 6f77 2069 7320   we need now is 
+00007020: 746f 2063 7265 6174 6520 616e 2069 6e70  to create an inp
+00007030: 7574 2066 6f72 6d20 746f 2065 6e74 6572  ut form to enter
+00007040: 2074 6865 2064 6174 6120 666f 7220 7468   the data for th
+00007050: 6520 6e65 7720 7065 7273 6f6e 2e94 8594  e new person....
+00007060: 8194 7d94 2868 166a 2807 0000 6826 6803  ..}.(h.j(...h&h.
+00007070: 6827 4e68 294e 7562 6168 177d 9428 6819  h'Nh)Nubah.}.(h.
+00007080: 5d94 681b 5d94 681d 5d94 681f 5d94 6821  ].h.].h.].h.].h!
+00007090: 5d94 7568 2568 5168 2768 5068 294b b168  ].uh%hQh'hPh)K.h
+000070a0: 166a 0907 0000 6826 6803 7562 6a18 0200  .j....h&h.ubj...
+000070b0: 0029 8194 7d94 2868 0558 7802 0000 6672  .)..}.(h.Xx...fr
+000070c0: 6f6d 2064 6563 6f72 655f 6261 7365 2069  om decore_base i
+000070d0: 6d70 6f72 7420 6465 636f 7265 0a66 726f  mport decore.fro
+000070e0: 6d20 6d6f 6465 6c73 2e66 6972 7374 5f6d  m models.first_m
+000070f0: 6f64 656c 2069 6d70 6f72 7420 4669 7273  odel import Firs
+00007100: 745f 6d6f 6465 6c0a 0a40 6465 636f 7265  t_model..@decore
+00007110: 2e62 6173 6528 7469 746c 653d 274d 7920  .base(title='My 
+00007120: 4669 7273 7420 4261 7365 272c 2069 636f  First Base', ico
+00007130: 6e3d 276d 6469 2d68 6f6d 6527 2c20 6d6f  n='mdi-home', mo
+00007140: 6465 6c3d 4669 7273 745f 6d6f 6465 6c29  del=First_model)
+00007150: 0a63 6c61 7373 2046 6972 7374 5f62 6173  .class First_bas
+00007160: 653a 0a20 2020 4064 6563 6f72 652e 7669  e:.   @decore.vi
+00007170: 6577 2874 6974 6c65 3d27 5065 7273 6f6e  ew(title='Person
+00007180: 272c 2069 636f 6e3d 276d 6469 2d61 6363  ', icon='mdi-acc
+00007190: 6f75 6e74 272c 2074 7970 653d 2774 6162  ount', type='tab
+000071a0: 6c65 272c 2066 6965 6c64 733d 5b46 6972  le', fields=[Fir
+000071b0: 7374 5f6d 6f64 656c 2e66 6972 7374 6e61  st_model.firstna
+000071c0: 6d65 2c20 4669 7273 745f 6d6f 6465 6c2e  me, First_model.
+000071d0: 6c61 7374 6e61 6d65 5d29 0a20 2020 6465  lastname]).   de
+000071e0: 6620 6669 7273 745f 7669 6577 2829 3a0a  f first_view():.
+000071f0: 2020 2020 2020 4064 6563 6f72 652e 6469        @decore.di
+00007200: 616c 6f67 2874 6974 6c65 3d27 4164 6420  alog(title='Add 
+00007210: 5065 7273 6f6e 272c 2069 636f 6e3d 276d  Person', icon='m
+00007220: 6469 2d70 6c75 7327 2c20 7479 7065 3d27  di-plus', type='
+00007230: 7374 616e 6461 7264 272c 2064 6973 706c  standard', displ
+00007240: 6179 3d27 6472 6177 6572 272c 2061 6374  ay='drawer', act
+00007250: 6976 6174 6f72 3d27 6465 6661 756c 742d  ivator='default-
+00007260: 6d65 6e75 2729 0a20 2020 2020 2064 6566  menu').      def
+00007270: 2066 6972 7374 5f64 6961 6c6f 6728 293a   first_dialog():
+00007280: 0a20 2020 2020 2020 2020 4064 6563 6f72  .         @decor
+00007290: 652e 7769 6467 6574 2874 6974 6c65 3d27  e.widget(title='
+000072a0: 4164 6420 5065 7273 6f6e 2046 6f72 6d27  Add Person Form'
+000072b0: 2c20 6963 6f6e 3d27 6d64 692d 6163 636f  , icon='mdi-acco
+000072c0: 756e 7427 2c20 7479 7065 3d27 666f 726d  unt', type='form
+000072d0: 272c 2066 6965 6c64 733d 5b46 6972 7374  ', fields=[First
+000072e0: 5f6d 6f64 656c 2e66 6972 7374 6e61 6d65  _model.firstname
+000072f0: 2c20 4669 7273 745f 6d6f 6465 6c2e 6c61  , First_model.la
+00007300: 7374 6e61 6d65 5d29 0a20 2020 2020 2020  stname]).       
+00007310: 2020 6465 6620 6669 7273 745f 7769 6467    def first_widg
+00007320: 6574 2829 3a0a 2020 2020 2020 2020 2020  et():.          
+00007330: 2020 7061 7373 9468 075d 9468 1158 7802    pass.h.].h.Xx.
+00007340: 0000 6672 6f6d 2064 6563 6f72 655f 6261  ..from decore_ba
+00007350: 7365 2069 6d70 6f72 7420 6465 636f 7265  se import decore
+00007360: 0a66 726f 6d20 6d6f 6465 6c73 2e66 6972  .from models.fir
+00007370: 7374 5f6d 6f64 656c 2069 6d70 6f72 7420  st_model import 
+00007380: 4669 7273 745f 6d6f 6465 6c0a 0a40 6465  First_model..@de
+00007390: 636f 7265 2e62 6173 6528 7469 746c 653d  core.base(title=
+000073a0: 274d 7920 4669 7273 7420 4261 7365 272c  'My First Base',
+000073b0: 2069 636f 6e3d 276d 6469 2d68 6f6d 6527   icon='mdi-home'
+000073c0: 2c20 6d6f 6465 6c3d 4669 7273 745f 6d6f  , model=First_mo
+000073d0: 6465 6c29 0a63 6c61 7373 2046 6972 7374  del).class First
+000073e0: 5f62 6173 653a 0a20 2020 4064 6563 6f72  _base:.   @decor
+000073f0: 652e 7669 6577 2874 6974 6c65 3d27 5065  e.view(title='Pe
+00007400: 7273 6f6e 272c 2069 636f 6e3d 276d 6469  rson', icon='mdi
+00007410: 2d61 6363 6f75 6e74 272c 2074 7970 653d  -account', type=
+00007420: 2774 6162 6c65 272c 2066 6965 6c64 733d  'table', fields=
+00007430: 5b46 6972 7374 5f6d 6f64 656c 2e66 6972  [First_model.fir
+00007440: 7374 6e61 6d65 2c20 4669 7273 745f 6d6f  stname, First_mo
+00007450: 6465 6c2e 6c61 7374 6e61 6d65 5d29 0a20  del.lastname]). 
+00007460: 2020 6465 6620 6669 7273 745f 7669 6577    def first_view
+00007470: 2829 3a0a 2020 2020 2020 4064 6563 6f72  ():.      @decor
+00007480: 652e 6469 616c 6f67 2874 6974 6c65 3d27  e.dialog(title='
+00007490: 4164 6420 5065 7273 6f6e 272c 2069 636f  Add Person', ico
+000074a0: 6e3d 276d 6469 2d70 6c75 7327 2c20 7479  n='mdi-plus', ty
+000074b0: 7065 3d27 7374 616e 6461 7264 272c 2064  pe='standard', d
+000074c0: 6973 706c 6179 3d27 6472 6177 6572 272c  isplay='drawer',
+000074d0: 2061 6374 6976 6174 6f72 3d27 6465 6661   activator='defa
+000074e0: 756c 742d 6d65 6e75 2729 0a20 2020 2020  ult-menu').     
+000074f0: 2064 6566 2066 6972 7374 5f64 6961 6c6f   def first_dialo
+00007500: 6728 293a 0a20 2020 2020 2020 2020 4064  g():.         @d
+00007510: 6563 6f72 652e 7769 6467 6574 2874 6974  ecore.widget(tit
+00007520: 6c65 3d27 4164 6420 5065 7273 6f6e 2046  le='Add Person F
+00007530: 6f72 6d27 2c20 6963 6f6e 3d27 6d64 692d  orm', icon='mdi-
+00007540: 6163 636f 756e 7427 2c20 7479 7065 3d27  account', type='
+00007550: 666f 726d 272c 2066 6965 6c64 733d 5b46  form', fields=[F
+00007560: 6972 7374 5f6d 6f64 656c 2e66 6972 7374  irst_model.first
+00007570: 6e61 6d65 2c20 4669 7273 745f 6d6f 6465  name, First_mode
+00007580: 6c2e 6c61 7374 6e61 6d65 5d29 0a20 2020  l.lastname]).   
+00007590: 2020 2020 2020 6465 6620 6669 7273 745f        def first_
+000075a0: 7769 6467 6574 2829 3a0a 2020 2020 2020  widget():.      
+000075b0: 2020 2020 2020 7061 7373 9485 9481 947d        pass.....}
+000075c0: 9468 166a 3607 0000 7362 6168 177d 9428  .h.j6...sbah.}.(
+000075d0: 6819 5d94 681b 5d94 681d 5d94 681f 5d94  h.].h.].h.].h.].
+000075e0: 6821 5d94 6823 6824 6a27 0200 0089 6a28  h!].h#h$j'....j(
+000075f0: 0200 008c 0670 7974 686f 6e94 6a2a 0200  .....python.j*..
+00007600: 007d 9475 6825 6a17 0200 0068 2768 5068  .}.uh%j....h'hPh
+00007610: 294b b368 166a 0907 0000 6826 6803 7562  )K.h.j....h&h.ub
+00007620: 6568 177d 9428 6819 5d94 8c06 7769 6467  eh.}.(h.]...widg
+00007630: 6574 9461 681b 5d94 681d 5d94 8c06 7769  et.ah.].h.]...wi
+00007640: 6467 6574 9461 681f 5d94 6821 5d94 7568  dget.ah.].h!].uh
+00007650: 2568 2a68 166a 2103 0000 6826 6803 6827  %h*h.j!...h&h.h'
+00007660: 6850 6829 4bae 7562 682b 2981 947d 9428  hPh)K.ubh+)..}.(
+00007670: 6805 6806 6807 5d94 2868 3029 8194 7d94  h.h.h.].(h0)..}.
+00007680: 2868 058c 0641 6374 696f 6e94 6807 5d94  (h...Action.h.].
+00007690: 6811 8c06 4163 7469 6f6e 9485 9481 947d  h...Action.....}
+000076a0: 9428 6816 6a51 0700 0068 2668 0368 274e  .(h.jQ...h&h.h'N
+000076b0: 6829 4e75 6261 6817 7d94 2868 195d 9468  h)Nubah.}.(h.].h
+000076c0: 1b5d 9468 1d5d 9468 1f5d 9468 215d 9475  .].h.].h.].h!].u
+000076d0: 6825 682f 6816 6a4e 0700 0068 2668 0368  h%h/h.jN...h&h.h
+000076e0: 2768 5068 294b c375 6268 5229 8194 7d94  'hPh)K.ubhR)..}.
+000076f0: 2868 058c b141 6374 696f 6e73 2061 7265  (h...Actions are
+00007700: 206d 6574 686f 6473 2077 6974 6820 7768   methods with wh
+00007710: 6963 6820 2a2a 6465 636f 7265 2046 726f  ich **decore Fro
+00007720: 6e74 2a2a 2063 616e 2063 6f6d 6d75 6e69  nt** can communi
+00007730: 6361 7465 2077 6974 6820 2a2a 6465 636f  cate with **deco
+00007740: 7265 2042 6173 652a 2a2e 2054 6865 7920  re Base**. They 
+00007750: 6361 6e20 6265 2061 6464 6564 2074 6f20  can be added to 
+00007760: 7669 6577 7320 616e 6420 7769 6467 6574  views and widget
+00007770: 7320 616e 6420 6172 6520 7468 6520 6f6e  s and are the on
+00007780: 6c79 2072 6561 6c20 636c 6173 7320 6d65  ly real class me
+00007790: 7468 6f64 7320 696e 2074 6865 206d 6574  thods in the met
+000077a0: 6120 6b69 742e 9468 075d 9428 6811 8c1f  a kit..h.].(h...
+000077b0: 4163 7469 6f6e 7320 6172 6520 6d65 7468  Actions are meth
+000077c0: 6f64 7320 7769 7468 2077 6869 6368 2094  ods with which .
+000077d0: 8594 8194 7d94 2868 166a 5f07 0000 6826  ....}.(h.j_...h&
+000077e0: 6803 6827 4e68 294e 7562 6866 2981 947d  h.h'Nh)Nubhf)..}
+000077f0: 9428 6805 8c10 2a2a 6465 636f 7265 2046  .(h...**decore F
+00007800: 726f 6e74 2a2a 9468 075d 9468 118c 0c64  ront**.h.].h...d
+00007810: 6563 6f72 6520 4672 6f6e 7494 8594 8194  ecore Front.....
+00007820: 7d94 2868 166a 6707 0000 6826 6803 6827  }.(h.jg...h&h.h'
+00007830: 4e68 294e 7562 6168 177d 9428 6819 5d94  Nh)Nubah.}.(h.].
+00007840: 681b 5d94 681d 5d94 681f 5d94 6821 5d94  h.].h.].h.].h!].
+00007850: 7568 2568 6568 166a 5f07 0000 7562 6811  uh%heh.j_...ubh.
+00007860: 8c16 2063 616e 2063 6f6d 6d75 6e69 6361  .. can communica
+00007870: 7465 2077 6974 6820 9485 9481 947d 9428  te with .....}.(
+00007880: 6816 6a5f 0700 0068 2668 0368 274e 6829  h.j_...h&h.h'Nh)
+00007890: 4e75 6268 6629 8194 7d94 2868 058c 0f2a  Nubhf)..}.(h...*
+000078a0: 2a64 6563 6f72 6520 4261 7365 2a2a 9468  *decore Base**.h
+000078b0: 075d 9468 118c 0b64 6563 6f72 6520 4261  .].h...decore Ba
+000078c0: 7365 9485 9481 947d 9428 6816 6a79 0700  se.....}.(h.jy..
+000078d0: 0068 2668 0368 274e 6829 4e75 6261 6817  .h&h.h'Nh)Nubah.
+000078e0: 7d94 2868 195d 9468 1b5d 9468 1d5d 9468  }.(h.].h.].h.].h
+000078f0: 1f5d 9468 215d 9475 6825 6865 6816 6a5f  .].h!].uh%heh.j_
+00007900: 0700 0075 6268 118c 5d2e 2054 6865 7920  ...ubh..]. They 
+00007910: 6361 6e20 6265 2061 6464 6564 2074 6f20  can be added to 
+00007920: 7669 6577 7320 616e 6420 7769 6467 6574  views and widget
+00007930: 7320 616e 6420 6172 6520 7468 6520 6f6e  s and are the on
+00007940: 6c79 2072 6561 6c20 636c 6173 7320 6d65  ly real class me
+00007950: 7468 6f64 7320 696e 2074 6865 206d 6574  thods in the met
+00007960: 6120 6b69 742e 9485 9481 947d 9428 6816  a kit......}.(h.
+00007970: 6a5f 0700 0068 2668 0368 274e 6829 4e75  j_...h&h.h'Nh)Nu
+00007980: 6265 6817 7d94 2868 195d 9468 1b5d 9468  beh.}.(h.].h.].h
+00007990: 1d5d 9468 1f5d 9468 215d 9475 6825 6851  .].h.].h!].uh%hQ
+000079a0: 6827 6850 6829 4bc4 6816 6a4e 0700 0068  h'hPh)K.h.jN...h
+000079b0: 2668 0375 6268 5229 8194 7d94 2868 058c  &h.ubhR)..}.(h..
+000079c0: 6e57 6520 6e6f 7720 6e65 6564 2061 6e20  nWe now need an 
+000079d0: 6163 7469 6f6e 2074 6f20 7374 6f72 6520  action to store 
+000079e0: 7468 6520 6461 7461 206f 6620 7468 6520  the data of the 
+000079f0: 6e65 7720 7065 7273 6f6e 2061 6e64 2065  new person and e
+00007a00: 7874 656e 6420 7468 6520 636f 6465 2069  xtend the code i
+00007a10: 6e20 2a2a 6669 7273 745f 6261 7365 2e70  n **first_base.p
+00007a20: 792a 2a20 6173 2066 6f6c 6c6f 7773 3a94  y** as follows:.
+00007a30: 6807 5d94 2868 118c 5157 6520 6e6f 7720  h.].(h..QWe now 
+00007a40: 6e65 6564 2061 6e20 6163 7469 6f6e 2074  need an action t
+00007a50: 6f20 7374 6f72 6520 7468 6520 6461 7461  o store the data
+00007a60: 206f 6620 7468 6520 6e65 7720 7065 7273   of the new pers
+00007a70: 6f6e 2061 6e64 2065 7874 656e 6420 7468  on and extend th
+00007a80: 6520 636f 6465 2069 6e20 9485 9481 947d  e code in .....}
+00007a90: 9428 6816 6a91 0700 0068 2668 0368 274e  .(h.j....h&h.h'N
+00007aa0: 6829 4e75 6268 6629 8194 7d94 2868 058c  h)Nubhf)..}.(h..
+00007ab0: 112a 2a66 6972 7374 5f62 6173 652e 7079  .**first_base.py
+00007ac0: 2a2a 9468 075d 9468 118c 0d66 6972 7374  **.h.].h...first
+00007ad0: 5f62 6173 652e 7079 9485 9481 947d 9428  _base.py.....}.(
+00007ae0: 6816 6a99 0700 0068 2668 0368 274e 6829  h.j....h&h.h'Nh)
+00007af0: 4e75 6261 6817 7d94 2868 195d 9468 1b5d  Nubah.}.(h.].h.]
+00007b00: 9468 1d5d 9468 1f5d 9468 215d 9475 6825  .h.].h.].h!].uh%
+00007b10: 6865 6816 6a91 0700 0075 6268 118c 0c20  heh.j....ubh... 
+00007b20: 6173 2066 6f6c 6c6f 7773 3a94 8594 8194  as follows:.....
+00007b30: 7d94 2868 166a 9107 0000 6826 6803 6827  }.(h.j....h&h.h'
+00007b40: 4e68 294e 7562 6568 177d 9428 6819 5d94  Nh)Nubeh.}.(h.].
+00007b50: 681b 5d94 681d 5d94 681f 5d94 6821 5d94  h.].h.].h.].h!].
+00007b60: 7568 2568 5168 2768 5068 294b c668 166a  uh%hQh'hPh)K.h.j
+00007b70: 4e07 0000 6826 6803 7562 6a18 0200 0029  N...h&h.ubj....)
+00007b80: 8194 7d94 2868 0558 5704 0000 6672 6f6d  ..}.(h.XW...from
+00007b90: 2064 6563 6f72 655f 6261 7365 2069 6d70   decore_base imp
+00007ba0: 6f72 7420 6465 636f 7265 0a66 726f 6d20  ort decore.from 
+00007bb0: 6d6f 6465 6c73 2e66 6972 7374 5f6d 6f64  models.first_mod
+00007bc0: 656c 2069 6d70 6f72 7420 4669 7273 745f  el import First_
+00007bd0: 6d6f 6465 6c0a 0a40 6465 636f 7265 2e62  model..@decore.b
+00007be0: 6173 6528 7469 746c 653d 274d 7920 4669  ase(title='My Fi
+00007bf0: 7273 7420 4261 7365 272c 2069 636f 6e3d  rst Base', icon=
+00007c00: 276d 6469 2d68 6f6d 6527 2c20 6d6f 6465  'mdi-home', mode
+00007c10: 6c3d 4669 7273 745f 6d6f 6465 6c29 0a63  l=First_model).c
+00007c20: 6c61 7373 2046 6972 7374 5f62 6173 653a  lass First_base:
+00007c30: 0a20 2020 4064 6563 6f72 652e 7669 6577  .   @decore.view
+00007c40: 2874 6974 6c65 3d27 5065 7273 6f6e 272c  (title='Person',
+00007c50: 2069 636f 6e3d 276d 6469 2d61 6363 6f75   icon='mdi-accou
+00007c60: 6e74 272c 2074 7970 653d 2774 6162 6c65  nt', type='table
+00007c70: 272c 2066 6965 6c64 733d 5b46 6972 7374  ', fields=[First
+00007c80: 5f6d 6f64 656c 2e66 6972 7374 6e61 6d65  _model.firstname
+00007c90: 2c20 4669 7273 745f 6d6f 6465 6c2e 6c61  , First_model.la
+00007ca0: 7374 6e61 6d65 5d29 0a20 2020 6465 6620  stname]).   def 
+00007cb0: 6669 7273 745f 7669 6577 2829 3a0a 2020  first_view():.  
+00007cc0: 2020 2020 4064 6563 6f72 652e 6469 616c      @decore.dial
+00007cd0: 6f67 2874 6974 6c65 3d27 4164 6420 5065  og(title='Add Pe
+00007ce0: 7273 6f6e 272c 2069 636f 6e3d 276d 6469  rson', icon='mdi
+00007cf0: 2d70 6c75 7327 2c20 7479 7065 3d27 7374  -plus', type='st
+00007d00: 616e 6461 7264 272c 2064 6973 706c 6179  andard', display
+00007d10: 3d27 6472 6177 6572 272c 2061 6374 6976  ='drawer', activ
+00007d20: 6174 6f72 3d27 6465 6661 756c 742d 6d65  ator='default-me
+00007d30: 6e75 2729 0a20 2020 2020 2064 6566 2066  nu').      def f
+00007d40: 6972 7374 5f64 6961 6c6f 6728 293a 0a20  irst_dialog():. 
+00007d50: 2020 2020 2020 2020 4064 6563 6f72 652e          @decore.
+00007d60: 7769 6467 6574 2874 6974 6c65 3d27 4164  widget(title='Ad
+00007d70: 6420 5065 7273 6f6e 2046 6f72 6d27 2c20  d Person Form', 
+00007d80: 6963 6f6e 3d27 6d64 692d 6163 636f 756e  icon='mdi-accoun
+00007d90: 7427 2c20 7479 7065 3d27 666f 726d 272c  t', type='form',
+00007da0: 2066 6965 6c64 733d 5b46 6972 7374 5f6d   fields=[First_m
+00007db0: 6f64 656c 2e66 6972 7374 6e61 6d65 2c20  odel.firstname, 
+00007dc0: 4669 7273 745f 6d6f 6465 6c2e 6c61 7374  First_model.last
+00007dd0: 6e61 6d65 5d29 0a20 2020 2020 2020 2020  name]).         
+00007de0: 6465 6620 6669 7273 745f 7769 6467 6574  def first_widget
+00007df0: 2829 3a0a 2020 2020 2020 2020 2020 2020  ():.            
+00007e00: 4064 6563 6f72 652e 6163 7469 6f6e 2874  @decore.action(t
+00007e10: 6974 6c65 3d27 5361 7665 2050 6572 736f  itle='Save Perso
+00007e20: 6e27 2c20 6963 6f6e 3d27 6d64 692d 636f  n', icon='mdi-co
+00007e30: 6e74 656e 742d 7361 7665 272c 2074 7970  ntent-save', typ
+00007e40: 653d 2773 7562 6d69 7427 290a 2020 2020  e='submit').    
+00007e50: 2020 2020 2020 2020 6465 6620 6669 7273          def firs
+00007e60: 745f 6163 7469 6f6e 2873 656c 662c 2064  t_action(self, d
+00007e70: 6174 6129 3a0a 2020 2020 2020 2020 2020  ata):.          
+00007e80: 2020 2020 2069 7465 6d20 3d20 4669 7273       item = Firs
+00007e90: 745f 6d6f 6465 6c28 290a 2020 2020 2020  t_model().      
+00007ea0: 2020 2020 2020 2020 2069 7465 6d2e 7469           item.ti
+00007eb0: 746c 6520 3d20 6461 7461 5b27 6669 7273  tle = data['firs
+00007ec0: 746e 616d 6527 5d20 2b20 2720 2720 2b20  tname'] + ' ' + 
+00007ed0: 6461 7461 5b27 6c61 7374 6e61 6d65 275d  data['lastname']
+00007ee0: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+00007ef0: 6974 656d 2e66 6972 7374 6e61 6d65 203d  item.firstname =
+00007f00: 2064 6174 615b 2766 6972 7374 6e61 6d65   data['firstname
+00007f10: 275d 0a20 2020 2020 2020 2020 2020 2020  '].             
+00007f20: 2020 6974 656d 2e6c 6173 746e 616d 6520    item.lastname 
+00007f30: 3d20 6461 7461 5b27 6c61 7374 6e61 6d65  = data['lastname
+00007f40: 275d 0a20 2020 2020 2020 2020 2020 2020  '].             
+00007f50: 2020 6966 2069 7465 6d2e 7361 7665 2829    if item.save()
+00007f60: 3a0a 2020 2020 2020 2020 2020 2020 2020  :.              
+00007f70: 2020 2020 7265 7475 726e 2054 7275 652c      return True,
+00007f80: 2069 7465 6d2e 7469 746c 6520 2b20 2720   item.title + ' 
+00007f90: 7361 7665 6420 7375 6363 6573 7366 756c  saved successful
+00007fa0: 6c79 270a 2020 2020 2020 2020 2020 2020  ly'.            
+00007fb0: 2020 2065 6c73 653a 0a20 2020 2020 2020     else:.       
+00007fc0: 2020 2020 2020 2020 2020 2072 6574 7572             retur
+00007fd0: 6e20 4661 6c73 652c 2069 7465 6d2e 6572  n False, item.er
+00007fe0: 726f 7294 6807 5d94 6811 5857 0400 0066  ror.h.].h.XW...f
+00007ff0: 726f 6d20 6465 636f 7265 5f62 6173 6520  rom decore_base 
+00008000: 696d 706f 7274 2064 6563 6f72 650a 6672  import decore.fr
+00008010: 6f6d 206d 6f64 656c 732e 6669 7273 745f  om models.first_
+00008020: 6d6f 6465 6c20 696d 706f 7274 2046 6972  model import Fir
+00008030: 7374 5f6d 6f64 656c 0a0a 4064 6563 6f72  st_model..@decor
+00008040: 652e 6261 7365 2874 6974 6c65 3d27 4d79  e.base(title='My
+00008050: 2046 6972 7374 2042 6173 6527 2c20 6963   First Base', ic
+00008060: 6f6e 3d27 6d64 692d 686f 6d65 272c 206d  on='mdi-home', m
+00008070: 6f64 656c 3d46 6972 7374 5f6d 6f64 656c  odel=First_model
+00008080: 290a 636c 6173 7320 4669 7273 745f 6261  ).class First_ba
+00008090: 7365 3a0a 2020 2040 6465 636f 7265 2e76  se:.   @decore.v
+000080a0: 6965 7728 7469 746c 653d 2750 6572 736f  iew(title='Perso
+000080b0: 6e27 2c20 6963 6f6e 3d27 6d64 692d 6163  n', icon='mdi-ac
+000080c0: 636f 756e 7427 2c20 7479 7065 3d27 7461  count', type='ta
+000080d0: 626c 6527 2c20 6669 656c 6473 3d5b 4669  ble', fields=[Fi
+000080e0: 7273 745f 6d6f 6465 6c2e 6669 7273 746e  rst_model.firstn
+000080f0: 616d 652c 2046 6972 7374 5f6d 6f64 656c  ame, First_model
+00008100: 2e6c 6173 746e 616d 655d 290a 2020 2064  .lastname]).   d
+00008110: 6566 2066 6972 7374 5f76 6965 7728 293a  ef first_view():
+00008120: 0a20 2020 2020 2040 6465 636f 7265 2e64  .      @decore.d
+00008130: 6961 6c6f 6728 7469 746c 653d 2741 6464  ialog(title='Add
+00008140: 2050 6572 736f 6e27 2c20 6963 6f6e 3d27   Person', icon='
+00008150: 6d64 692d 706c 7573 272c 2074 7970 653d  mdi-plus', type=
+00008160: 2773 7461 6e64 6172 6427 2c20 6469 7370  'standard', disp
+00008170: 6c61 793d 2764 7261 7765 7227 2c20 6163  lay='drawer', ac
+00008180: 7469 7661 746f 723d 2764 6566 6175 6c74  tivator='default
+00008190: 2d6d 656e 7527 290a 2020 2020 2020 6465  -menu').      de
+000081a0: 6620 6669 7273 745f 6469 616c 6f67 2829  f first_dialog()
+000081b0: 3a0a 2020 2020 2020 2020 2040 6465 636f  :.         @deco
+000081c0: 7265 2e77 6964 6765 7428 7469 746c 653d  re.widget(title=
+000081d0: 2741 6464 2050 6572 736f 6e20 466f 726d  'Add Person Form
+000081e0: 272c 2069 636f 6e3d 276d 6469 2d61 6363  ', icon='mdi-acc
+000081f0: 6f75 6e74 272c 2074 7970 653d 2766 6f72  ount', type='for
+00008200: 6d27 2c20 6669 656c 6473 3d5b 4669 7273  m', fields=[Firs
+00008210: 745f 6d6f 6465 6c2e 6669 7273 746e 616d  t_model.firstnam
+00008220: 652c 2046 6972 7374 5f6d 6f64 656c 2e6c  e, First_model.l
+00008230: 6173 746e 616d 655d 290a 2020 2020 2020  astname]).      
+00008240: 2020 2064 6566 2066 6972 7374 5f77 6964     def first_wid
+00008250: 6765 7428 293a 0a20 2020 2020 2020 2020  get():.         
+00008260: 2020 2040 6465 636f 7265 2e61 6374 696f     @decore.actio
+00008270: 6e28 7469 746c 653d 2753 6176 6520 5065  n(title='Save Pe
+00008280: 7273 6f6e 272c 2069 636f 6e3d 276d 6469  rson', icon='mdi
+00008290: 2d63 6f6e 7465 6e74 2d73 6176 6527 2c20  -content-save', 
+000082a0: 7479 7065 3d27 7375 626d 6974 2729 0a20  type='submit'). 
+000082b0: 2020 2020 2020 2020 2020 2064 6566 2066             def f
+000082c0: 6972 7374 5f61 6374 696f 6e28 7365 6c66  irst_action(self
+000082d0: 2c20 6461 7461 293a 0a20 2020 2020 2020  , data):.       
+000082e0: 2020 2020 2020 2020 6974 656d 203d 2046          item = F
+000082f0: 6972 7374 5f6d 6f64 656c 2829 0a20 2020  irst_model().   
+00008300: 2020 2020 2020 2020 2020 2020 6974 656d              item
+00008310: 2e74 6974 6c65 203d 2064 6174 615b 2766  .title = data['f
+00008320: 6972 7374 6e61 6d65 275d 202b 2027 2027  irstname'] + ' '
+00008330: 202b 2064 6174 615b 276c 6173 746e 616d   + data['lastnam
+00008340: 6527 5d0a 2020 2020 2020 2020 2020 2020  e'].            
+00008350: 2020 2069 7465 6d2e 6669 7273 746e 616d     item.firstnam
+00008360: 6520 3d20 6461 7461 5b27 6669 7273 746e  e = data['firstn
+00008370: 616d 6527 5d0a 2020 2020 2020 2020 2020  ame'].          
+00008380: 2020 2020 2069 7465 6d2e 6c61 7374 6e61       item.lastna
+00008390: 6d65 203d 2064 6174 615b 276c 6173 746e  me = data['lastn
+000083a0: 616d 6527 5d0a 2020 2020 2020 2020 2020  ame'].          
+000083b0: 2020 2020 2069 6620 6974 656d 2e73 6176       if item.sav
+000083c0: 6528 293a 0a20 2020 2020 2020 2020 2020  e():.           
+000083d0: 2020 2020 2020 2072 6574 7572 6e20 5472         return Tr
+000083e0: 7565 2c20 6974 656d 2e74 6974 6c65 202b  ue, item.title +
+000083f0: 2027 2073 6176 6564 2073 7563 6365 7373   ' saved success
+00008400: 6675 6c6c 7927 0a20 2020 2020 2020 2020  fully'.         
+00008410: 2020 2020 2020 656c 7365 3a0a 2020 2020        else:.    
+00008420: 2020 2020 2020 2020 2020 2020 2020 7265                re
+00008430: 7475 726e 2046 616c 7365 2c20 6974 656d  turn False, item
+00008440: 2e65 7272 6f72 9485 9481 947d 9468 166a  .error.....}.h.j
+00008450: b107 0000 7362 6168 177d 9428 6819 5d94  ....sbah.}.(h.].
+00008460: 681b 5d94 681d 5d94 681f 5d94 6821 5d94  h.].h.].h.].h!].
+00008470: 6823 6824 6a27 0200 0089 6a28 0200 008c  h#h$j'....j(....
+00008480: 0670 7974 686f 6e94 6a2a 0200 007d 9475  .python.j*...}.u
+00008490: 6825 6a17 0200 0068 2768 5068 294b c868  h%j....h'hPh)K.h
+000084a0: 166a 4e07 0000 6826 6803 7562 6a48 0400  .jN...h&h.ubjH..
+000084b0: 0029 8194 7d94 2868 058c b054 6f20 6372  .)..}.(h...To cr
+000084c0: 6561 7465 2061 2072 6563 6f72 6420 7769  eate a record wi
+000084d0: 7468 2064 6563 6f72 6520 4261 7365 2c20  th decore Base, 
+000084e0: 7765 206e 6565 6420 746f 2063 7265 6174  we need to creat
+000084f0: 6520 616e 2069 6e73 7461 6e63 6520 6f66  e an instance of
+00008500: 2074 6865 206d 6f64 656c 2e20 496e 206f   the model. In o
+00008510: 7572 2063 6173 6520 2a2a 4669 7273 745f  ur case **First_
+00008520: 6d6f 6465 6c2a 2a2e 2054 6865 2069 6e73  model**. The ins
+00008530: 7461 6e63 6520 6973 2066 696c 6c65 6420  tance is filled 
+00008540: 7769 7468 2074 6865 2064 6174 6120 6672  with the data fr
+00008550: 6f6d 2074 6865 2066 6f72 6d20 616e 6420  om the form and 
+00008560: 7468 656e 2073 6176 6564 2e94 6807 5d94  then saved..h.].
+00008570: 6852 2981 947d 9428 6805 6ac3 0700 0068  hR)..}.(h.j....h
+00008580: 075d 9428 6811 8c5d 546f 2063 7265 6174  .].(h..]To creat
+00008590: 6520 6120 7265 636f 7264 2077 6974 6820  e a record with 
+000085a0: 6465 636f 7265 2042 6173 652c 2077 6520  decore Base, we 
+000085b0: 6e65 6564 2074 6f20 6372 6561 7465 2061  need to create a
+000085c0: 6e20 696e 7374 616e 6365 206f 6620 7468  n instance of th
+000085d0: 6520 6d6f 6465 6c2e 2049 6e20 6f75 7220  e model. In our 
+000085e0: 6361 7365 2094 8594 8194 7d94 2868 166a  case .....}.(h.j
+000085f0: c507 0000 6826 6803 6827 4e68 294e 7562  ....h&h.h'Nh)Nub
+00008600: 6866 2981 947d 9428 6805 8c0f 2a2a 4669  hf)..}.(h...**Fi
+00008610: 7273 745f 6d6f 6465 6c2a 2a94 6807 5d94  rst_model**.h.].
+00008620: 6811 8c0b 4669 7273 745f 6d6f 6465 6c94  h...First_model.
+00008630: 8594 8194 7d94 2868 166a cc07 0000 6826  ....}.(h.j....h&
+00008640: 6803 6827 4e68 294e 7562 6168 177d 9428  h.h'Nh)Nubah.}.(
+00008650: 6819 5d94 681b 5d94 681d 5d94 681f 5d94  h.].h.].h.].h.].
+00008660: 6821 5d94 7568 2568 6568 166a c507 0000  h!].uh%heh.j....
+00008670: 7562 6811 8c44 2e20 5468 6520 696e 7374  ubh..D. The inst
+00008680: 616e 6365 2069 7320 6669 6c6c 6564 2077  ance is filled w
+00008690: 6974 6820 7468 6520 6461 7461 2066 726f  ith the data fro
+000086a0: 6d20 7468 6520 666f 726d 2061 6e64 2074  m the form and t
+000086b0: 6865 6e20 7361 7665 642e 9485 9481 947d  hen saved......}
+000086c0: 9428 6816 6ac5 0700 0068 2668 0368 274e  .(h.j....h&h.h'N
+000086d0: 6829 4e75 6265 6817 7d94 2868 195d 9468  h)Nubeh.}.(h.].h
+000086e0: 1b5d 9468 1d5d 9468 1f5d 9468 215d 9475  .].h.].h.].h!].u
+000086f0: 6825 6851 6827 6850 6829 4be1 6816 6ac1  h%hQh'hPh)K.h.j.
+00008700: 0700 0075 6261 6817 7d94 2868 195d 9468  ...ubah.}.(h.].h
+00008710: 1b5d 9468 1d5d 9468 1f5d 9468 215d 9475  .].h.].h.].h!].u
+00008720: 6825 6a47 0400 0068 166a 4e07 0000 6826  h%jG...h.jN...h&
+00008730: 6803 6827 6850 6829 4e75 626a a605 0000  h.h'hPh)Nubj....
+00008740: 2981 947d 9428 6805 8c99 5468 6520 6669  )..}.(h...The fi
+00008750: 656c 6420 2a2a 7469 746c 652a 2a20 7761  eld **title** wa
+00008760: 7320 696e 6865 7269 7465 6420 6672 6f6d  s inherited from
+00008770: 2074 6865 2063 6c61 7373 202a 2a44 6566   the class **Def
+00008780: 6f72 6d5f 6d6f 6465 6c2a 2a20 616e 6420  orm_model** and 
+00008790: 6d75 7374 2062 6520 7573 6564 2066 6f72  must be used for
+000087a0: 2065 6163 6820 7265 636f 7264 2063 7265   each record cre
+000087b0: 6174 696f 6e2e 204f 7468 6572 7769 7365  ation. Otherwise
+000087c0: 2074 6865 2069 7465 6d20 7769 6c6c 2066   the item will f
+000087d0: 6169 6c20 7468 6520 7661 6c69 6461 7469  ail the validati
+000087e0: 6f6e 2e94 6807 5d94 6852 2981 947d 9428  on..h.].hR)..}.(
+000087f0: 6805 6aec 0700 0068 075d 9428 6811 8c0a  h.j....h.].(h...
+00008800: 5468 6520 6669 656c 6420 9485 9481 947d  The field .....}
+00008810: 9428 6816 6aee 0700 0068 2668 0368 274e  .(h.j....h&h.h'N
+00008820: 6829 4e75 6268 6629 8194 7d94 2868 058c  h)Nubhf)..}.(h..
+00008830: 092a 2a74 6974 6c65 2a2a 9468 075d 9468  .**title**.h.].h
+00008840: 118c 0574 6974 6c65 9485 9481 947d 9428  ...title.....}.(
+00008850: 6816 6af5 0700 0068 2668 0368 274e 6829  h.j....h&h.h'Nh)
+00008860: 4e75 6261 6817 7d94 2868 195d 9468 1b5d  Nubah.}.(h.].h.]
+00008870: 9468 1d5d 9468 1f5d 9468 215d 9475 6825  .h.].h.].h!].uh%
+00008880: 6865 6816 6aee 0700 0075 6268 118c 1e20  heh.j....ubh... 
+00008890: 7761 7320 696e 6865 7269 7465 6420 6672  was inherited fr
+000088a0: 6f6d 2074 6865 2063 6c61 7373 2094 8594  om the class ...
+000088b0: 8194 7d94 2868 166a ee07 0000 6826 6803  ..}.(h.j....h&h.
+000088c0: 6827 4e68 294e 7562 6866 2981 947d 9428  h'Nh)Nubhf)..}.(
+000088d0: 6805 8c10 2a2a 4465 666f 726d 5f6d 6f64  h...**Deform_mod
+000088e0: 656c 2a2a 9468 075d 9468 118c 0c44 6566  el**.h.].h...Def
+000088f0: 6f72 6d5f 6d6f 6465 6c94 8594 8194 7d94  orm_model.....}.
+00008900: 2868 166a 0708 0000 6826 6803 6827 4e68  (h.j....h&h.h'Nh
+00008910: 294e 7562 6168 177d 9428 6819 5d94 681b  )Nubah.}.(h.].h.
+00008920: 5d94 681d 5d94 681f 5d94 6821 5d94 7568  ].h.].h.].h!].uh
+00008930: 2568 6568 166a ee07 0000 7562 6811 8c58  %heh.j....ubh..X
+00008940: 2061 6e64 206d 7573 7420 6265 2075 7365   and must be use
+00008950: 6420 666f 7220 6561 6368 2072 6563 6f72  d for each recor
+00008960: 6420 6372 6561 7469 6f6e 2e20 4f74 6865  d creation. Othe
+00008970: 7277 6973 6520 7468 6520 6974 656d 2077  rwise the item w
+00008980: 696c 6c20 6661 696c 2074 6865 2076 616c  ill fail the val
+00008990: 6964 6174 696f 6e2e 9485 9481 947d 9428  idation......}.(
+000089a0: 6816 6aee 0700 0068 2668 0368 274e 6829  h.j....h&h.h'Nh)
+000089b0: 4e75 6265 6817 7d94 2868 195d 9468 1b5d  Nubeh.}.(h.].h.]
+000089c0: 9468 1d5d 9468 1f5d 9468 215d 9475 6825  .h.].h.].h!].uh%
+000089d0: 6851 6827 6850 6829 4be4 6816 6aea 0700  hQh'hPh)K.h.j...
+000089e0: 0075 6261 6817 7d94 2868 195d 9468 1b5d  .ubah.}.(h.].h.]
+000089f0: 9468 1d5d 9468 1f5d 9468 215d 9475 6825  .h.].h.].h!].uh%
+00008a00: 6aa5 0500 0068 166a 4e07 0000 6826 6803  j....h.jN...h&h.
+00008a10: 6827 6850 6829 4e75 6265 6817 7d94 2868  h'hPh)Nubeh.}.(h
+00008a20: 195d 948c 0661 6374 696f 6e94 6168 1b5d  .]...action.ah.]
+00008a30: 9468 1d5d 948c 0661 6374 696f 6e94 6168  .h.]...action.ah
+00008a40: 1f5d 9468 215d 9475 6825 682a 6816 6a21  .].h!].uh%h*h.j!
+00008a50: 0300 0068 2668 0368 2768 5068 294b c375  ...h&h.h'hPh)K.u
+00008a60: 6265 6817 7d94 2868 195d 948c 0575 7361  beh.}.(h.]...usa
+00008a70: 6765 9461 681b 5d94 681d 5d94 8c05 7573  ge.ah.].h.]...us
+00008a80: 6167 6594 6168 1f5d 9468 215d 9475 6825  age.ah.].h!].uh%
+00008a90: 682a 6816 6a92 0100 0068 2668 0368 2768  h*h.j....h&h.h'h
+00008aa0: 5068 294b 3c75 6268 2b29 8194 7d94 2868  Ph)K<ubh+)..}.(h
+00008ab0: 0568 0668 075d 9428 6830 2981 947d 9428  .h.h.].(h0)..}.(
+00008ac0: 6805 8c1a 5275 6e2c 2044 6576 656c 6f70  h...Run, Develop
+00008ad0: 6d65 6e74 2061 6e64 2042 7569 6c64 9468  ment and Build.h
+00008ae0: 075d 9468 118c 1a52 756e 2c20 4465 7665  .].h...Run, Deve
+00008af0: 6c6f 706d 656e 7420 616e 6420 4275 696c  lopment and Buil
+00008b00: 6494 8594 8194 7d94 2868 166a 3808 0000  d.....}.(h.j8...
+00008b10: 6826 6803 6827 4e68 294e 7562 6168 177d  h&h.h'Nh)Nubah.}
+00008b20: 9428 6819 5d94 681b 5d94 681d 5d94 681f  .(h.].h.].h.].h.
+00008b30: 5d94 6821 5d94 7568 2568 2f68 166a 3508  ].h!].uh%h/h.j5.
+00008b40: 0000 6826 6803 6827 6850 6829 4be7 7562  ..h&h.h'hPh)K.ub
+00008b50: 6852 2981 947d 9428 6805 8c71 546f 2073  hR)..}.(h..qTo s
+00008b60: 7461 7274 206f 6e6c 7920 796f 7572 2061  tart only your a
+00008b70: 7070 6c69 6361 7469 6f6e 2c20 7275 6e20  pplication, run 
+00008b80: 6060 7079 7468 6f6e 2061 7070 2e70 7960  ``python app.py`
+00008b90: 6020 696e 2079 6f75 7220 7072 6f6a 6563  ` in your projec
+00008ba0: 7420 726f 6f74 2064 6972 6563 746f 7279  t root directory
+00008bb0: 2e20 5573 6520 7468 6520 7465 726d 696e  . Use the termin
+00008bc0: 616c 2069 6e20 7673 636f 6465 2e94 6807  al in vscode..h.
+00008bd0: 5d94 2868 118c 2454 6f20 7374 6172 7420  ].(h..$To start 
+00008be0: 6f6e 6c79 2079 6f75 7220 6170 706c 6963  only your applic
+00008bf0: 6174 696f 6e2c 2072 756e 2094 8594 8194  ation, run .....
+00008c00: 7d94 2868 166a 4608 0000 6826 6803 6827  }.(h.jF...h&h.h'
+00008c10: 4e68 294e 7562 6aee 0200 0029 8194 7d94  Nh)Nubj....)..}.
+00008c20: 2868 058c 1160 6070 7974 686f 6e20 6170  (h...``python ap
+00008c30: 702e 7079 6060 9468 075d 9468 118c 0d70  p.py``.h.].h...p
+00008c40: 7974 686f 6e20 6170 702e 7079 9485 9481  ython app.py....
+00008c50: 947d 9428 6816 6a4e 0800 0068 2668 0368  .}.(h.jN...h&h.h
+00008c60: 274e 6829 4e75 6261 6817 7d94 2868 195d  'Nh)Nubah.}.(h.]
+00008c70: 9468 1b5d 9468 1d5d 9468 1f5d 9468 215d  .h.].h.].h.].h!]
+00008c80: 9475 6825 6aed 0200 0068 166a 4608 0000  .uh%j....h.jF...
+00008c90: 7562 6811 8c3c 2069 6e20 796f 7572 2070  ubh..< in your p
+00008ca0: 726f 6a65 6374 2072 6f6f 7420 6469 7265  roject root dire
+00008cb0: 6374 6f72 792e 2055 7365 2074 6865 2074  ctory. Use the t
+00008cc0: 6572 6d69 6e61 6c20 696e 2076 7363 6f64  erminal in vscod
+00008cd0: 652e 9485 9481 947d 9428 6816 6a46 0800  e......}.(h.jF..
+00008ce0: 0068 2668 0368 274e 6829 4e75 6265 6817  .h&h.h'Nh)Nubeh.
+00008cf0: 7d94 2868 195d 9468 1b5d 9468 1d5d 9468  }.(h.].h.].h.].h
+00008d00: 1f5d 9468 215d 9475 6825 6851 6827 6850  .].h!].uh%hQh'hP
+00008d10: 6829 4be8 6816 6a35 0800 0068 2668 0375  h)K.h.j5...h&h.u
+00008d20: 6268 5229 8194 7d94 2868 058c 344f 7065  bhR)..}.(h..4Ope
+00008d30: 6e20 7468 6520 6272 6f77 7365 7220 616e  n the browser an
+00008d40: 6420 7479 7065 2060 6068 7474 703a 2f2f  d type ``http://
+00008d50: 6c6f 6361 6c68 6f73 743a 3535 3535 6060  localhost:5555``
+00008d60: 2e94 6807 5d94 2868 118c 1a4f 7065 6e20  ..h.].(h...Open 
+00008d70: 7468 6520 6272 6f77 7365 7220 616e 6420  the browser and 
+00008d80: 7479 7065 2094 8594 8194 7d94 2868 166a  type .....}.(h.j
+00008d90: 6608 0000 6826 6803 6827 4e68 294e 7562  f...h&h.h'Nh)Nub
+00008da0: 6aee 0200 0029 8194 7d94 2868 058c 1960  j....)..}.(h...`
+00008db0: 6068 7474 703a 2f2f 6c6f 6361 6c68 6f73  `http://localhos
+00008dc0: 743a 3535 3535 6060 9468 075d 9468 118c  t:5555``.h.].h..
+00008dd0: 1568 7474 703a 2f2f 6c6f 6361 6c68 6f73  .http://localhos
+00008de0: 743a 3535 3535 9485 9481 947d 9428 6816  t:5555.....}.(h.
+00008df0: 6a6e 0800 0068 2668 0368 274e 6829 4e75  jn...h&h.h'Nh)Nu
+00008e00: 6261 6817 7d94 2868 195d 9468 1b5d 9468  bah.}.(h.].h.].h
+00008e10: 1d5d 9468 1f5d 9468 215d 9475 6825 6aed  .].h.].h!].uh%j.
+00008e20: 0200 0068 166a 6608 0000 7562 6811 8c01  ...h.jf...ubh...
+00008e30: 2e94 8594 8194 7d94 2868 166a 6608 0000  ......}.(h.jf...
+00008e40: 6826 6803 6827 4e68 294e 7562 6568 177d  h&h.h'Nh)Nubeh.}
+00008e50: 9428 6819 5d94 681b 5d94 681d 5d94 681f  .(h.].h.].h.].h.
+00008e60: 5d94 6821 5d94 7568 2568 5168 2768 5068  ].h!].uh%hQh'hPh
+00008e70: 294b ea68 166a 3508 0000 6826 6803 7562  )K.h.j5...h&h.ub
+00008e80: 682b 2981 947d 9428 6805 6806 6807 5d94  h+)..}.(h.h.h.].
+00008e90: 2868 3029 8194 7d94 2868 058c 0b44 6576  (h0)..}.(h...Dev
+00008ea0: 656c 6f70 6d65 6e74 9468 075d 9468 118c  elopment.h.].h..
+00008eb0: 0b44 6576 656c 6f70 6d65 6e74 9485 9481  .Development....
+00008ec0: 947d 9428 6816 6a89 0800 0068 2668 0368  .}.(h.j....h&h.h
+00008ed0: 274e 6829 4e75 6261 6817 7d94 2868 195d  'Nh)Nubah.}.(h.]
+00008ee0: 9468 1b5d 9468 1d5d 9468 1f5d 9468 215d  .h.].h.].h.].h!]
+00008ef0: 9475 6825 682f 6816 6a86 0800 0068 2668  .uh%h/h.j....h&h
+00008f00: 0368 2768 5068 294b ed75 6268 5229 8194  .h'hPh)K.ubhR)..
+00008f10: 7d94 2868 058c 6c54 6f20 6465 7665 6c6f  }.(h..lTo develo
+00008f20: 7020 796f 7572 2061 7070 6c69 6361 7469  p your applicati
+00008f30: 6f6e 2c20 7573 6520 796f 7572 2064 6562  on, use your deb
+00008f40: 7567 6765 7220 7769 7468 2074 6865 2060  ugger with the `
+00008f50: 605b 6465 765d 2064 6563 6f72 6520 6261  `[dev] decore ba
+00008f60: 7365 2064 6576 656c 6f70 6d65 6e74 6060  se development``
+00008f70: 2070 726f 6669 6c65 2069 6e20 7673 636f   profile in vsco
+00008f80: 6465 2e94 6807 5d94 2868 118c 3854 6f20  de..h.].(h..8To 
+00008f90: 6465 7665 6c6f 7020 796f 7572 2061 7070  develop your app
+00008fa0: 6c69 6361 7469 6f6e 2c20 7573 6520 796f  lication, use yo
+00008fb0: 7572 2064 6562 7567 6765 7220 7769 7468  ur debugger with
+00008fc0: 2074 6865 2094 8594 8194 7d94 2868 166a   the .....}.(h.j
+00008fd0: 9708 0000 6826 6803 6827 4e68 294e 7562  ....h&h.h'Nh)Nub
+00008fe0: 6aee 0200 0029 8194 7d94 2868 058c 2160  j....)..}.(h..!`
+00008ff0: 605b 6465 765d 2064 6563 6f72 6520 6261  `[dev] decore ba
+00009000: 7365 2064 6576 656c 6f70 6d65 6e74 6060  se development``
+00009010: 9468 075d 9468 118c 1d5b 6465 765d 2064  .h.].h...[dev] d
+00009020: 6563 6f72 6520 6261 7365 2064 6576 656c  ecore base devel
+00009030: 6f70 6d65 6e74 9485 9481 947d 9428 6816  opment.....}.(h.
+00009040: 6a9f 0800 0068 2668 0368 274e 6829 4e75  j....h&h.h'Nh)Nu
+00009050: 6261 6817 7d94 2868 195d 9468 1b5d 9468  bah.}.(h.].h.].h
+00009060: 1d5d 9468 1f5d 9468 215d 9475 6825 6aed  .].h.].h!].uh%j.
+00009070: 0200 0068 166a 9708 0000 7562 6811 8c13  ...h.j....ubh...
+00009080: 2070 726f 6669 6c65 2069 6e20 7673 636f   profile in vsco
+00009090: 6465 2e94 8594 8194 7d94 2868 166a 9708  de......}.(h.j..
+000090a0: 0000 6826 6803 6827 4e68 294e 7562 6568  ..h&h.h'Nh)Nubeh
+000090b0: 177d 9428 6819 5d94 681b 5d94 681d 5d94  .}.(h.].h.].h.].
+000090c0: 681f 5d94 6821 5d94 7568 2568 5168 2768  h.].h!].uh%hQh'h
+000090d0: 5068 294b ee68 166a 8608 0000 6826 6803  Ph)K.h.j....h&h.
+000090e0: 7562 6852 2981 947d 9428 6805 8c34 4f70  ubhR)..}.(h..4Op
+000090f0: 656e 2074 6865 2062 726f 7773 6572 2061  en the browser a
+00009100: 6e64 2074 7970 6520 6060 6874 7470 3a2f  nd type ``http:/
+00009110: 2f6c 6f63 616c 686f 7374 3a35 3535 3560  /localhost:5555`
+00009120: 602e 9468 075d 9428 6811 8c1a 4f70 656e  `..h.].(h...Open
+00009130: 2074 6865 2062 726f 7773 6572 2061 6e64   the browser and
+00009140: 2074 7970 6520 9485 9481 947d 9428 6816   type .....}.(h.
+00009150: 6ab7 0800 0068 2668 0368 274e 6829 4e75  j....h&h.h'Nh)Nu
+00009160: 626a ee02 0000 2981 947d 9428 6805 8c19  bj....)..}.(h...
+00009170: 6060 6874 7470 3a2f 2f6c 6f63 616c 686f  ``http://localho
+00009180: 7374 3a35 3535 3560 6094 6807 5d94 6811  st:5555``.h.].h.
+00009190: 8c15 6874 7470 3a2f 2f6c 6f63 616c 686f  ..http://localho
+000091a0: 7374 3a35 3535 3594 8594 8194 7d94 2868  st:5555.....}.(h
+000091b0: 166a bf08 0000 6826 6803 6827 4e68 294e  .j....h&h.h'Nh)N
+000091c0: 7562 6168 177d 9428 6819 5d94 681b 5d94  ubah.}.(h.].h.].
+000091d0: 681d 5d94 681f 5d94 6821 5d94 7568 256a  h.].h.].h!].uh%j
+000091e0: ed02 0000 6816 6ab7 0800 0075 6268 118c  ....h.j....ubh..
+000091f0: 012e 9485 9481 947d 9428 6816 6ab7 0800  .......}.(h.j...
+00009200: 0068 2668 0368 274e 6829 4e75 6265 6817  .h&h.h'Nh)Nubeh.
+00009210: 7d94 2868 195d 9468 1b5d 9468 1d5d 9468  }.(h.].h.].h.].h
+00009220: 1f5d 9468 215d 9475 6825 6851 6827 6850  .].h!].uh%hQh'hP
+00009230: 6829 4bf0 6816 6a86 0800 0068 2668 0375  h)K.h.j....h&h.u
+00009240: 6265 6817 7d94 2868 195d 948c 0b64 6576  beh.}.(h.]...dev
+00009250: 656c 6f70 6d65 6e74 9461 681b 5d94 681d  elopment.ah.].h.
+00009260: 5d94 8c0b 6465 7665 6c6f 706d 656e 7494  ]...development.
+00009270: 6168 1f5d 9468 215d 9475 6825 682a 6816  ah.].h!].uh%h*h.
+00009280: 6a35 0800 0068 2668 0368 2768 5068 294b  j5...h&h.h'hPh)K
+00009290: ed75 6268 2b29 8194 7d94 2868 0568 0668  .ubh+)..}.(h.h.h
+000092a0: 075d 9428 6830 2981 947d 9428 6805 8c05  .].(h0)..}.(h...
+000092b0: 4275 696c 6494 6807 5d94 6811 8c05 4275  Build.h.].h...Bu
+000092c0: 696c 6494 8594 8194 7d94 2868 166a e208  ild.....}.(h.j..
+000092d0: 0000 6826 6803 6827 4e68 294e 7562 6168  ..h&h.h'Nh)Nubah
+000092e0: 177d 9428 6819 5d94 681b 5d94 681d 5d94  .}.(h.].h.].h.].
+000092f0: 681f 5d94 6821 5d94 7568 2568 2f68 166a  h.].h!].uh%h/h.j
+00009300: df08 0000 6826 6803 6827 6850 6829 4bf3  ....h&h.h'hPh)K.
+00009310: 7562 6852 2981 947d 9428 6805 8c74 546f  ubhR)..}.(h..tTo
+00009320: 2062 7569 6c64 2079 6f75 7220 6170 706c   build your appl
+00009330: 6963 6174 696f 6e2c 2072 756e 2060 6070  ication, run ``p
+00009340: 7974 686f 6e20 6170 702e 7079 202d 2d62  ython app.py --b
+00009350: 7569 6c64 6060 2069 6e20 796f 7572 2070  uild`` in your p
+00009360: 726f 6a65 6374 2072 6f6f 7420 6469 7265  roject root dire
+00009370: 6374 6f72 792e 2055 7365 2074 6865 2074  ctory. Use the t
+00009380: 6572 6d69 6e61 6c20 696e 2076 7363 6f64  erminal in vscod
+00009390: 652e 9468 075d 9428 6811 8c1f 546f 2062  e..h.].(h...To b
+000093a0: 7569 6c64 2079 6f75 7220 6170 706c 6963  uild your applic
+000093b0: 6174 696f 6e2c 2072 756e 2094 8594 8194  ation, run .....
+000093c0: 7d94 2868 166a f008 0000 6826 6803 6827  }.(h.j....h&h.h'
+000093d0: 4e68 294e 7562 6aee 0200 0029 8194 7d94  Nh)Nubj....)..}.
+000093e0: 2868 058c 1960 6070 7974 686f 6e20 6170  (h...``python ap
+000093f0: 702e 7079 202d 2d62 7569 6c64 6060 9468  p.py --build``.h
+00009400: 075d 9468 118c 1570 7974 686f 6e20 6170  .].h...python ap
+00009410: 702e 7079 202d 2d62 7569 6c64 9485 9481  p.py --build....
+00009420: 947d 9428 6816 6af8 0800 0068 2668 0368  .}.(h.j....h&h.h
+00009430: 274e 6829 4e75 6261 6817 7d94 2868 195d  'Nh)Nubah.}.(h.]
+00009440: 9468 1b5d 9468 1d5d 9468 1f5d 9468 215d  .h.].h.].h.].h!]
+00009450: 9475 6825 6aed 0200 0068 166a f008 0000  .uh%j....h.j....
+00009460: 7562 6811 8c3c 2069 6e20 796f 7572 2070  ubh..< in your p
+00009470: 726f 6a65 6374 2072 6f6f 7420 6469 7265  roject root dire
+00009480: 6374 6f72 792e 2055 7365 2074 6865 2074  ctory. Use the t
+00009490: 6572 6d69 6e61 6c20 696e 2076 7363 6f64  erminal in vscod
+000094a0: 652e 9485 9481 947d 9428 6816 6af0 0800  e......}.(h.j...
+000094b0: 0068 2668 0368 274e 6829 4e75 6265 6817  .h&h.h'Nh)Nubeh.
+000094c0: 7d94 2868 195d 9468 1b5d 9468 1d5d 9468  }.(h.].h.].h.].h
+000094d0: 1f5d 9468 215d 9475 6825 6851 6827 6850  .].h!].uh%hQh'hP
+000094e0: 6829 4bf4 6816 6adf 0800 0068 2668 0375  h)K.h.j....h&h.u
+000094f0: 6265 6817 7d94 2868 195d 948c 0562 7569  beh.}.(h.]...bui
+00009500: 6c64 9461 681b 5d94 681d 5d94 8c05 6275  ld.ah.].h.]...bu
+00009510: 696c 6494 6168 1f5d 9468 215d 9475 6825  ild.ah.].h!].uh%
+00009520: 682a 6816 6a35 0800 0068 2668 0368 2768  h*h.j5...h&h.h'h
+00009530: 5068 294b f375 6265 6817 7d94 2868 195d  Ph)K.ubeh.}.(h.]
+00009540: 948c 1972 756e 2d64 6576 656c 6f70 6d65  ...run-developme
+00009550: 6e74 2d61 6e64 2d62 7569 6c64 9461 681b  nt-and-build.ah.
+00009560: 5d94 681d 5d94 8c1a 7275 6e2c 2064 6576  ].h.]...run, dev
+00009570: 656c 6f70 6d65 6e74 2061 6e64 2062 7569  elopment and bui
+00009580: 6c64 9461 681f 5d94 6821 5d94 7568 2568  ld.ah.].h!].uh%h
+00009590: 2a68 166a 9201 0000 6826 6803 6827 6850  *h.j....h&h.h'hP
+000095a0: 6829 4be7 7562 6568 177d 9428 6819 5d94  h)K.ubeh.}.(h.].
+000095b0: 8c0b 6765 742d 7374 6172 7465 6494 6168  ..get-started.ah
+000095c0: 1b5d 9468 1d5d 948c 0b67 6574 2073 7461  .].h.]...get sta
+000095d0: 7274 6564 9461 681f 5d94 6821 5d94 7568  rted.ah.].h!].uh
+000095e0: 2568 2a68 1668 2c68 2668 0368 2768 5068  %h*h.h,h&h.h'hPh
+000095f0: 294b 1a75 6268 2b29 8194 7d94 2868 0568  )K.ubh+)..}.(h.h
+00009600: 0668 075d 9428 6830 2981 947d 9428 6805  .h.].(h0)..}.(h.
+00009610: 8c12 5361 6d70 6c65 2061 7070 6c69 6361  ..Sample applica
+00009620: 7469 6f6e 9468 075d 9468 118c 1253 616d  tion.h.].h...Sam
+00009630: 706c 6520 6170 706c 6963 6174 696f 6e94  ple application.
+00009640: 8594 8194 7d94 2868 166a 2b09 0000 6826  ....}.(h.j+...h&
+00009650: 6803 6827 4e68 294e 7562 6168 177d 9428  h.h'Nh)Nubah.}.(
+00009660: 6819 5d94 681b 5d94 681d 5d94 681f 5d94  h.].h.].h.].h.].
+00009670: 6821 5d94 7568 2568 2f68 166a 2809 0000  h!].uh%h/h.j(...
+00009680: 6826 6803 6827 6850 6829 4bf7 7562 6852  h&h.h'hPh)K.ubhR
+00009690: 2981 947d 9428 6805 8c9e 546f 2062 6574  )..}.(h...To bet
+000096a0: 7465 7220 756e 6465 7273 7461 6e64 2068  ter understand h
+000096b0: 6f77 2064 6563 6f72 6520 6261 7365 2077  ow decore base w
+000096c0: 6f72 6b73 2c20 6974 2069 7320 6265 7374  orks, it is best
+000096d0: 2074 6f20 6c6f 6f6b 2061 7420 7468 6520   to look at the 
+000096e0: 7361 6d70 6c65 2061 7070 6c69 6361 7469  sample applicati
+000096f0: 6f6e 2e20 5468 6520 6170 706c 6963 6174  on. The applicat
+00009700: 696f 6e20 7265 7072 6573 656e 7473 206d  ion represents m
+00009710: 7920 636f 6e74 696e 756f 7573 2064 6576  y continuous dev
+00009720: 656c 6f70 6d65 6e74 206f 6620 6465 636f  elopment of deco
+00009730: 7265 2062 6173 652e 9468 075d 9468 118c  re base..h.].h..
+00009740: 9e54 6f20 6265 7474 6572 2075 6e64 6572  .To better under
+00009750: 7374 616e 6420 686f 7720 6465 636f 7265  stand how decore
+00009760: 2062 6173 6520 776f 726b 732c 2069 7420   base works, it 
+00009770: 6973 2062 6573 7420 746f 206c 6f6f 6b20  is best to look 
+00009780: 6174 2074 6865 2073 616d 706c 6520 6170  at the sample ap
+00009790: 706c 6963 6174 696f 6e2e 2054 6865 2061  plication. The a
+000097a0: 7070 6c69 6361 7469 6f6e 2072 6570 7265  pplication repre
+000097b0: 7365 6e74 7320 6d79 2063 6f6e 7469 6e75  sents my continu
+000097c0: 6f75 7320 6465 7665 6c6f 706d 656e 7420  ous development 
+000097d0: 6f66 2064 6563 6f72 6520 6261 7365 2e94  of decore base..
+000097e0: 8594 8194 7d94 2868 166a 3909 0000 6826  ....}.(h.j9...h&
+000097f0: 6803 6827 4e68 294e 7562 6168 177d 9428  h.h'Nh)Nubah.}.(
+00009800: 6819 5d94 681b 5d94 681d 5d94 681f 5d94  h.].h.].h.].h.].
+00009810: 6821 5d94 7568 2568 5168 2768 5068 294b  h!].uh%hQh'hPh)K
+00009820: f868 166a 2809 0000 6826 6803 7562 6852  .h.j(...h&h.ubhR
+00009830: 2981 947d 9428 6805 8c48 6874 7470 733a  )..}.(h..Hhttps:
+00009840: 2f2f 6769 7468 7562 2e63 6f6d 2f4b 656d  //github.com/Kem
+00009850: 6f50 616e 7a61 682f 6465 636f 7265 5f42  oPanzah/decore_B
+00009860: 6173 652f 7472 6565 2f6d 6173 7465 722f  ase/tree/master/
+00009870: 6465 636f 7265 5f62 6173 652f 7361 6d70  decore_base/samp
+00009880: 6c65 9468 075d 9468 9229 8194 7d94 2868  le.h.].h.)..}.(h
+00009890: 056a 4909 0000 6807 5d94 6811 8c48 6874  .jI...h.].h..Hht
+000098a0: 7470 733a 2f2f 6769 7468 7562 2e63 6f6d  tps://github.com
+000098b0: 2f4b 656d 6f50 616e 7a61 682f 6465 636f  /KemoPanzah/deco
+000098c0: 7265 5f42 6173 652f 7472 6565 2f6d 6173  re_Base/tree/mas
+000098d0: 7465 722f 6465 636f 7265 5f62 6173 652f  ter/decore_base/
+000098e0: 7361 6d70 6c65 9485 9481 947d 9428 6816  sample.....}.(h.
+000098f0: 6a4b 0900 0068 2668 0368 274e 6829 4e75  jK...h&h.h'Nh)Nu
+00009900: 6261 6817 7d94 2868 195d 9468 1b5d 9468  bah.}.(h.].h.].h
+00009910: 1d5d 9468 1f5d 9468 215d 948c 0672 6566  .].h.].h!]...ref
+00009920: 7572 6994 6a49 0900 0075 6825 6891 6816  uri.jI...uh%h.h.
+00009930: 6a47 0900 0075 6261 6817 7d94 2868 195d  jG...ubah.}.(h.]
+00009940: 9468 1b5d 9468 1d5d 9468 1f5d 9468 215d  .h.].h.].h.].h!]
+00009950: 9475 6825 6851 6827 6850 6829 4bfa 6816  .uh%hQh'hPh)K.h.
+00009960: 6a28 0900 0068 2668 0375 6268 5229 8194  j(...h&h.ubhR)..
+00009970: 7d94 2868 058c b054 6f20 7379 6e63 6872  }.(h...To synchr
+00009980: 6f6e 697a 6520 7468 6520 7361 6d70 6c65  onize the sample
+00009990: 2061 7070 6c69 6361 7469 6f6e 2077 6974   application wit
+000099a0: 6820 6120 7375 6266 6f6c 6465 7220 6f66  h a subfolder of
+000099b0: 2074 6865 2070 726f 6a65 6374 2072 6f6f   the project roo
+000099c0: 7420 6469 7265 6374 6f72 792c 2072 756e  t directory, run
+000099d0: 2060 6070 7974 686f 6e20 6170 702e 7079   ``python app.py
+000099e0: 202d 2d73 616d 706c 6560 6020 696e 2079   --sample`` in y
+000099f0: 6f75 7220 7072 6f6a 6563 7420 726f 6f74  our project root
+00009a00: 2064 6972 6563 746f 7279 2e20 5573 6520   directory. Use 
+00009a10: 7468 6520 7465 726d 696e 616c 2069 6e20  the terminal in 
+00009a20: 7673 636f 6465 2e94 6807 5d94 2868 118c  vscode..h.].(h..
+00009a30: 5a54 6f20 7379 6e63 6872 6f6e 697a 6520  ZTo synchronize 
+00009a40: 7468 6520 7361 6d70 6c65 2061 7070 6c69  the sample appli
+00009a50: 6361 7469 6f6e 2077 6974 6820 6120 7375  cation with a su
+00009a60: 6266 6f6c 6465 7220 6f66 2074 6865 2070  bfolder of the p
+00009a70: 726f 6a65 6374 2072 6f6f 7420 6469 7265  roject root dire
+00009a80: 6374 6f72 792c 2072 756e 2094 8594 8194  ctory, run .....
+00009a90: 7d94 2868 166a 5f09 0000 6826 6803 6827  }.(h.j_...h&h.h'
+00009aa0: 4e68 294e 7562 6aee 0200 0029 8194 7d94  Nh)Nubj....)..}.
+00009ab0: 2868 058c 1a60 6070 7974 686f 6e20 6170  (h...``python ap
+00009ac0: 702e 7079 202d 2d73 616d 706c 6560 6094  p.py --sample``.
+00009ad0: 6807 5d94 6811 8c16 7079 7468 6f6e 2061  h.].h...python a
+00009ae0: 7070 2e70 7920 2d2d 7361 6d70 6c65 9485  pp.py --sample..
+00009af0: 9481 947d 9428 6816 6a67 0900 0068 2668  ...}.(h.jg...h&h
+00009b00: 0368 274e 6829 4e75 6261 6817 7d94 2868  .h'Nh)Nubah.}.(h
+00009b10: 195d 9468 1b5d 9468 1d5d 9468 1f5d 9468  .].h.].h.].h.].h
+00009b20: 215d 9475 6825 6aed 0200 0068 166a 5f09  !].uh%j....h.j_.
+00009b30: 0000 7562 6811 8c3c 2069 6e20 796f 7572  ..ubh..< in your
+00009b40: 2070 726f 6a65 6374 2072 6f6f 7420 6469   project root di
+00009b50: 7265 6374 6f72 792e 2055 7365 2074 6865  rectory. Use the
+00009b60: 2074 6572 6d69 6e61 6c20 696e 2076 7363   terminal in vsc
+00009b70: 6f64 652e 9485 9481 947d 9428 6816 6a5f  ode......}.(h.j_
+00009b80: 0900 0068 2668 0368 274e 6829 4e75 6265  ...h&h.h'Nh)Nube
+00009b90: 6817 7d94 2868 195d 9468 1b5d 9468 1d5d  h.}.(h.].h.].h.]
+00009ba0: 9468 1f5d 9468 215d 9475 6825 6851 6827  .h.].h!].uh%hQh'
+00009bb0: 6850 6829 4bfc 6816 6a28 0900 0068 2668  hPh)K.h.j(...h&h
+00009bc0: 0375 6268 5229 8194 7d94 2868 058c 7f54  .ubhR)..}.(h...T
+00009bd0: 6f20 7275 6e20 7468 6520 7361 6d70 6c65  o run the sample
+00009be0: 2061 7070 6c69 6361 7469 6f6e 2061 6674   application aft
+00009bf0: 6572 2073 796e 6368 726f 6e69 7a61 7469  er synchronizati
+00009c00: 6f6e 2c20 7573 6520 796f 7572 2064 6562  on, use your deb
+00009c10: 7567 6765 7220 7769 7468 2074 6865 2060  ugger with the `
+00009c20: 605b 736d 705d 2064 6563 6f72 6520 6261  `[smp] decore ba
+00009c30: 7365 2073 616d 706c 6560 6020 7072 6f66  se sample`` prof
+00009c40: 696c 6520 696e 2076 7363 6f64 652e 9468  ile in vscode..h
+00009c50: 075d 9428 6811 8c50 546f 2072 756e 2074  .].(h..PTo run t
+00009c60: 6865 2073 616d 706c 6520 6170 706c 6963  he sample applic
+00009c70: 6174 696f 6e20 6166 7465 7220 7379 6e63  ation after sync
+00009c80: 6872 6f6e 697a 6174 696f 6e2c 2075 7365  hronization, use
+00009c90: 2079 6f75 7220 6465 6275 6767 6572 2077   your debugger w
+00009ca0: 6974 6820 7468 6520 9485 9481 947d 9428  ith the .....}.(
+00009cb0: 6816 6a7f 0900 0068 2668 0368 274e 6829  h.j....h&h.h'Nh)
+00009cc0: 4e75 626a ee02 0000 2981 947d 9428 6805  Nubj....)..}.(h.
+00009cd0: 8c1c 6060 5b73 6d70 5d20 6465 636f 7265  ..``[smp] decore
+00009ce0: 2062 6173 6520 7361 6d70 6c65 6060 9468   base sample``.h
+00009cf0: 075d 9468 118c 185b 736d 705d 2064 6563  .].h...[smp] dec
+00009d00: 6f72 6520 6261 7365 2073 616d 706c 6594  ore base sample.
+00009d10: 8594 8194 7d94 2868 166a 8709 0000 6826  ....}.(h.j....h&
+00009d20: 6803 6827 4e68 294e 7562 6168 177d 9428  h.h'Nh)Nubah.}.(
+00009d30: 6819 5d94 681b 5d94 681d 5d94 681f 5d94  h.].h.].h.].h.].
+00009d40: 6821 5d94 7568 256a ed02 0000 6816 6a7f  h!].uh%j....h.j.
+00009d50: 0900 0075 6268 118c 1320 7072 6f66 696c  ...ubh... profil
+00009d60: 6520 696e 2076 7363 6f64 652e 9485 9481  e in vscode.....
+00009d70: 947d 9428 6816 6a7f 0900 0068 2668 0368  .}.(h.j....h&h.h
+00009d80: 274e 6829 4e75 6265 6817 7d94 2868 195d  'Nh)Nubeh.}.(h.]
+00009d90: 9468 1b5d 9468 1d5d 9468 1f5d 9468 215d  .h.].h.].h.].h!]
+00009da0: 9475 6825 6851 6827 6850 6829 4bfe 6816  .uh%hQh'hPh)K.h.
+00009db0: 6a28 0900 0068 2668 0375 6265 6817 7d94  j(...h&h.ubeh.}.
+00009dc0: 2868 195d 948c 1273 616d 706c 652d 6170  (h.]...sample-ap
+00009dd0: 706c 6963 6174 696f 6e94 6168 1b5d 9468  plication.ah.].h
+00009de0: 1d5d 948c 1273 616d 706c 6520 6170 706c  .]...sample appl
+00009df0: 6963 6174 696f 6e94 6168 1f5d 9468 215d  ication.ah.].h!]
+00009e00: 9475 6825 682a 6816 682c 6826 6803 6827  .uh%h*h.h,h&h.h'
+00009e10: 6850 6829 4bf7 7562 682b 2981 947d 9428  hPh)K.ubh+)..}.(
+00009e20: 6805 6806 6807 5d94 2868 3029 8194 7d94  h.h.h.].(h0)..}.
+00009e30: 2868 058c 054e 6f74 6573 9468 075d 9468  (h...Notes.h.].h
+00009e40: 118c 054e 6f74 6573 9485 9481 947d 9428  ...Notes.....}.(
+00009e50: 6816 6aaa 0900 0068 2668 0368 274e 6829  h.j....h&h.h'Nh)
+00009e60: 4e75 6261 6817 7d94 2868 195d 9468 1b5d  Nubah.}.(h.].h.]
+00009e70: 9468 1d5d 9468 1f5d 9468 215d 9475 6825  .h.].h.].h!].uh%
+00009e80: 682f 6816 6aa7 0900 0068 2668 0368 2768  h/h.j....h&h.h'h
+00009e90: 5068 294d 0101 7562 6852 2981 947d 9428  Ph)M..ubhR)..}.(
+00009ea0: 6805 8c46 5468 6973 2064 6f63 756d 656e  h..FThis documen
+00009eb0: 7461 7469 6f6e 2077 6173 2074 7261 6e73  tation was trans
+00009ec0: 6c61 7465 6420 6672 6f6d 2047 6572 6d61  lated from Germa
+00009ed0: 6e20 696e 746f 2045 6e67 6c69 7368 2077  n into English w
+00009ee0: 6974 6820 4465 6570 6c2e 9468 075d 9468  ith Deepl..h.].h
+00009ef0: 118c 4654 6869 7320 646f 6375 6d65 6e74  ..FThis document
+00009f00: 6174 696f 6e20 7761 7320 7472 616e 736c  ation was transl
+00009f10: 6174 6564 2066 726f 6d20 4765 726d 616e  ated from German
+00009f20: 2069 6e74 6f20 456e 676c 6973 6820 7769   into English wi
+00009f30: 7468 2044 6565 706c 2e94 8594 8194 7d94  th Deepl......}.
+00009f40: 2868 166a b809 0000 6826 6803 6827 4e68  (h.j....h&h.h'Nh
+00009f50: 294e 7562 6168 177d 9428 6819 5d94 681b  )Nubah.}.(h.].h.
+00009f60: 5d94 681d 5d94 681f 5d94 6821 5d94 7568  ].h.].h.].h!].uh
+00009f70: 2568 5168 2768 5068 294d 0201 6816 6aa7  %hQh'hPh)M..h.j.
+00009f80: 0900 0068 2668 0375 6268 098c 0863 6f6d  ...h&h.ubh...com
+00009f90: 706f 756e 6494 9394 2981 947d 9428 6805  pound...)..}.(h.
+00009fa0: 6806 6807 5d94 6800 8c07 746f 6374 7265  h.h.].h...toctre
+00009fb0: 6594 9394 2981 947d 9428 6805 6806 6807  e...)..}.(h.h.h.
+00009fc0: 5d94 6817 7d94 2868 195d 9468 1b5d 9468  ].h.}.(h.].h.].h
+00009fd0: 1d5d 9468 1f5d 9468 215d 9468 168c 0569  .].h.].h!].h...i
+00009fe0: 6e64 6578 948c 0765 6e74 7269 6573 945d  ndex...entries.]
+00009ff0: 948c 0c69 6e63 6c75 6465 6669 6c65 7394  ...includefiles.
+0000a000: 5d94 8c08 6d61 7864 6570 7468 944b 028c  ]...maxdepth.K..
+0000a010: 0763 6170 7469 6f6e 944e 8c04 676c 6f62  .caption.N..glob
+0000a020: 9489 8c06 6869 6464 656e 9488 8c0d 696e  ....hidden....in
+0000a030: 636c 7564 6568 6964 6465 6e94 898c 086e  cludehidden....n
+0000a040: 756d 6265 7265 6494 4b00 8c0a 7469 746c  umbered.K...titl
+0000a050: 6573 6f6e 6c79 9489 8c0a 7261 7765 6e74  esonly....rawent
+0000a060: 7269 6573 945d 9475 6825 6acb 0900 0068  ries.].uh%j....h
+0000a070: 2768 2868 294b 0b68 166a c809 0000 7562  'h(h)K.h.j....ub
+0000a080: 6168 177d 9428 6819 5d94 681b 5d94 8c0f  ah.}.(h.].h.]...
+0000a090: 746f 6374 7265 652d 7772 6170 7065 7294  toctree-wrapper.
+0000a0a0: 6168 1d5d 9468 1f5d 9468 215d 9475 6825  ah.].h.].h!].uh%
+0000a0b0: 6ac6 0900 0068 166a a709 0000 6826 6803  j....h.j....h&h.
+0000a0c0: 6827 6828 6829 4e75 6268 0b29 8194 7d94  h'h(h)Nubh.)..}.
+0000a0d0: 2868 058c 1249 6e64 6963 6573 2061 6e64  (h...Indices and
+0000a0e0: 2074 6162 6c65 7394 6807 5d94 6811 8c12   tables.h.].h...
+0000a0f0: 496e 6469 6365 7320 616e 6420 7461 626c  Indices and tabl
+0000a100: 6573 9485 9481 947d 9468 166a eb09 0000  es.....}.h.j....
+0000a110: 7362 6168 177d 9428 6819 5d94 681b 5d94  sbah.}.(h.].h.].
+0000a120: 681d 5d94 681f 5d94 6821 5d94 6823 6824  h.].h.].h!].h#h$
+0000a130: 7568 2568 0a68 166a a709 0000 6826 6803  uh%h.h.j....h&h.
+0000a140: 6827 6828 6829 4b0f 7562 680b 2981 947d  h'h(h)K.ubh.)..}
+0000a150: 9428 6805 8c12 3d3d 3d3d 3d3d 3d3d 3d3d  .(h...==========
+0000a160: 3d3d 3d3d 3d3d 3d3d 9468 075d 9468 118c  ========.h.].h..
+0000a170: 123d 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d  .===============
+0000a180: 3d3d 3d94 8594 8194 7d94 6816 6af9 0900  ===.....}.h.j...
+0000a190: 0073 6261 6817 7d94 2868 195d 9468 1b5d  .sbah.}.(h.].h.]
+0000a1a0: 9468 1d5d 9468 1f5d 9468 215d 9468 2368  .h.].h.].h!].h#h
+0000a1b0: 2475 6825 680a 6816 6aa7 0900 0068 2668  $uh%h.h.j....h&h
+0000a1c0: 0368 2768 2868 294b 1175 6268 0b29 8194  .h'h(h)K.ubh.)..
+0000a1d0: 7d94 2868 058c 112a 203a 7265 663a 6067  }.(h...* :ref:`g
+0000a1e0: 656e 696e 6465 7860 9468 075d 9468 118c  enindex`.h.].h..
+0000a1f0: 112a 203a 7265 663a 6067 656e 696e 6465  .* :ref:`geninde
+0000a200: 7860 9485 9481 947d 9468 166a 070a 0000  x`.....}.h.j....
+0000a210: 7362 6168 177d 9428 6819 5d94 681b 5d94  sbah.}.(h.].h.].
+0000a220: 681d 5d94 681f 5d94 6821 5d94 6823 6824  h.].h.].h!].h#h$
+0000a230: 7568 2568 0a68 166a a709 0000 6826 6803  uh%h.h.j....h&h.
+0000a240: 6827 6828 6829 4b12 7562 680b 2981 947d  h'h(h)K.ubh.)..}
+0000a250: 9428 6805 8c11 2a20 3a72 6566 3a60 6d6f  .(h...* :ref:`mo
+0000a260: 6469 6e64 6578 6094 6807 5d94 6811 8c11  dindex`.h.].h...
+0000a270: 2a20 3a72 6566 3a60 6d6f 6469 6e64 6578  * :ref:`modindex
+0000a280: 6094 8594 8194 7d94 6816 6a15 0a00 0073  `.....}.h.j....s
+0000a290: 6261 6817 7d94 2868 195d 9468 1b5d 9468  bah.}.(h.].h.].h
+0000a2a0: 1d5d 9468 1f5d 9468 215d 9468 2368 2475  .].h.].h!].h#h$u
+0000a2b0: 6825 680a 6816 6aa7 0900 0068 2668 0368  h%h.h.j....h&h.h
+0000a2c0: 2768 2868 294b 1375 6268 0b29 8194 7d94  'h(h)K.ubh.)..}.
+0000a2d0: 2868 058c 0f2a 203a 7265 663a 6073 6561  (h...* :ref:`sea
+0000a2e0: 7263 6860 9468 075d 9468 118c 0f2a 203a  rch`.h.].h...* :
+0000a2f0: 7265 663a 6073 6561 7263 6860 9485 9481  ref:`search`....
+0000a300: 947d 9468 166a 230a 0000 7362 6168 177d  .}.h.j#...sbah.}
+0000a310: 9428 6819 5d94 681b 5d94 681d 5d94 681f  .(h.].h.].h.].h.
+0000a320: 5d94 6821 5d94 6823 6824 7568 2568 0a68  ].h!].h#h$uh%h.h
+0000a330: 166a a709 0000 6826 6803 6827 6828 6829  .j....h&h.h'h(h)
+0000a340: 4b14 7562 6568 177d 9428 6819 5d94 8c05  K.ubeh.}.(h.]...
+0000a350: 6e6f 7465 7394 6168 1b5d 9468 1d5d 948c  notes.ah.].h.]..
+0000a360: 056e 6f74 6573 9461 681f 5d94 6821 5d94  .notes.ah.].h!].
+0000a370: 7568 2568 2a68 1668 2c68 2668 0368 2768  uh%h*h.h,h&h.h'h
+0000a380: 5068 294d 0101 7562 6568 177d 9428 6819  Ph)M..ubeh.}.(h.
+0000a390: 5d94 8c07 7765 6c63 6f6d 6594 6168 1b5d  ]...welcome.ah.]
+0000a3a0: 9468 1d5d 948c 0777 656c 636f 6d65 9461  .h.]...welcome.a
+0000a3b0: 681f 5d94 6821 5d94 7568 2568 2a68 1668  h.].h!].uh%h*h.h
+0000a3c0: 0368 2668 0368 2768 2868 294b 0775 6265  .h&h.h'h(h)K.ube
+0000a3d0: 6817 7d94 2868 195d 9468 1b5d 9468 1d5d  h.}.(h.].h.].h.]
+0000a3e0: 9468 1f5d 9468 215d 948c 0673 6f75 7263  .h.].h!]...sourc
+0000a3f0: 6594 6828 7568 2568 018c 0e63 7572 7265  e.h(uh%h...curre
+0000a400: 6e74 5f73 6f75 7263 6594 4e8c 0c63 7572  nt_source.N..cur
+0000a410: 7265 6e74 5f6c 696e 6594 4e8c 0873 6574  rent_line.N..set
+0000a420: 7469 6e67 7394 8c11 646f 6375 7469 6c73  tings...docutils
+0000a430: 2e66 726f 6e74 656e 6494 8c06 5661 6c75  .frontend...Valu
+0000a440: 6573 9493 9429 8194 7d94 2868 2f4e 8c09  es...)..}.(h/N..
+0000a450: 6765 6e65 7261 746f 7294 4e8c 0964 6174  generator.N..dat
+0000a460: 6573 7461 6d70 944e 8c0b 736f 7572 6365  estamp.N..source
+0000a470: 5f6c 696e 6b94 4e8c 0a73 6f75 7263 655f  _link.N..source_
+0000a480: 7572 6c94 4e8c 0d74 6f63 5f62 6163 6b6c  url.N..toc_backl
+0000a490: 696e 6b73 948c 0565 6e74 7279 948c 1266  inks...entry...f
+0000a4a0: 6f6f 746e 6f74 655f 6261 636b 6c69 6e6b  ootnote_backlink
+0000a4b0: 7394 4b01 8c0d 7365 6374 6e75 6d5f 7866  s.K...sectnum_xf
+0000a4c0: 6f72 6d94 4b01 8c0e 7374 7269 705f 636f  orm.K...strip_co
+0000a4d0: 6d6d 656e 7473 944e 8c1b 7374 7269 705f  mments.N..strip_
+0000a4e0: 656c 656d 656e 7473 5f77 6974 685f 636c  elements_with_cl
+0000a4f0: 6173 7365 7394 4e8c 0d73 7472 6970 5f63  asses.N..strip_c
+0000a500: 6c61 7373 6573 944e 8c0c 7265 706f 7274  lasses.N..report
+0000a510: 5f6c 6576 656c 944b 028c 0a68 616c 745f  _level.K...halt_
+0000a520: 6c65 7665 6c94 4b05 8c11 6578 6974 5f73  level.K...exit_s
+0000a530: 7461 7475 735f 6c65 7665 6c94 4b05 8c05  tatus_level.K...
+0000a540: 6465 6275 6794 4e8c 0e77 6172 6e69 6e67  debug.N..warning
+0000a550: 5f73 7472 6561 6d94 4e8c 0974 7261 6365  _stream.N..trace
+0000a560: 6261 636b 9488 8c0e 696e 7075 745f 656e  back....input_en
+0000a570: 636f 6469 6e67 948c 0975 7466 2d38 2d73  coding...utf-8-s
+0000a580: 6967 948c 1c69 6e70 7574 5f65 6e63 6f64  ig...input_encod
+0000a590: 696e 675f 6572 726f 725f 6861 6e64 6c65  ing_error_handle
+0000a5a0: 7294 8c06 7374 7269 6374 948c 0f6f 7574  r...strict...out
+0000a5b0: 7075 745f 656e 636f 6469 6e67 948c 0575  put_encoding...u
+0000a5c0: 7466 2d38 948c 1d6f 7574 7075 745f 656e  tf-8...output_en
+0000a5d0: 636f 6469 6e67 5f65 7272 6f72 5f68 616e  coding_error_han
+0000a5e0: 646c 6572 946a 640a 0000 8c0e 6572 726f  dler.jd.....erro
+0000a5f0: 725f 656e 636f 6469 6e67 948c 0575 7466  r_encoding...utf
+0000a600: 2d38 948c 1c65 7272 6f72 5f65 6e63 6f64  -8...error_encod
+0000a610: 696e 675f 6572 726f 725f 6861 6e64 6c65  ing_error_handle
+0000a620: 7294 8c10 6261 636b 736c 6173 6872 6570  r...backslashrep
+0000a630: 6c61 6365 948c 0d6c 616e 6775 6167 655f  lace...language_
+0000a640: 636f 6465 948c 0265 6e94 8c13 7265 636f  code...en...reco
+0000a650: 7264 5f64 6570 656e 6465 6e63 6965 7394  rd_dependencies.
+0000a660: 4e8c 0663 6f6e 6669 6794 4e8c 0969 645f  N..config.N..id_
+0000a670: 7072 6566 6978 9468 068c 0e61 7574 6f5f  prefix.h...auto_
+0000a680: 6964 5f70 7265 6669 7894 8c02 6964 948c  id_prefix...id..
+0000a690: 0d64 756d 705f 7365 7474 696e 6773 944e  .dump_settings.N
+0000a6a0: 8c0e 6475 6d70 5f69 6e74 6572 6e61 6c73  ..dump_internals
+0000a6b0: 944e 8c0f 6475 6d70 5f74 7261 6e73 666f  .N..dump_transfo
+0000a6c0: 726d 7394 4e8c 0f64 756d 705f 7073 6575  rms.N..dump_pseu
+0000a6d0: 646f 5f78 6d6c 944e 8c10 6578 706f 7365  do_xml.N..expose
+0000a6e0: 5f69 6e74 6572 6e61 6c73 944e 8c0e 7374  _internals.N..st
+0000a6f0: 7269 6374 5f76 6973 6974 6f72 944e 8c0f  rict_visitor.N..
+0000a700: 5f64 6973 6162 6c65 5f63 6f6e 6669 6794  _disable_config.
+0000a710: 4e8c 075f 736f 7572 6365 9468 288c 0c5f  N.._source.h(.._
+0000a720: 6465 7374 696e 6174 696f 6e94 4e8c 0d5f  destination.N.._
+0000a730: 636f 6e66 6967 5f66 696c 6573 945d 948c  config_files.]..
+0000a740: 1666 696c 655f 696e 7365 7274 696f 6e5f  .file_insertion_
+0000a750: 656e 6162 6c65 6494 888c 0b72 6177 5f65  enabled....raw_e
+0000a760: 6e61 626c 6564 944b 018c 116c 696e 655f  nabled.K...line_
+0000a770: 6c65 6e67 7468 5f6c 696d 6974 944d 1027  length_limit.M.'
+0000a780: 8c0e 7065 705f 7265 6665 7265 6e63 6573  ..pep_references
+0000a790: 944e 8c0c 7065 705f 6261 7365 5f75 726c  .N..pep_base_url
+0000a7a0: 948c 1868 7474 7073 3a2f 2f70 6570 732e  ...https://peps.
+0000a7b0: 7079 7468 6f6e 2e6f 7267 2f94 8c15 7065  python.org/...pe
+0000a7c0: 705f 6669 6c65 5f75 726c 5f74 656d 706c  p_file_url_templ
+0000a7d0: 6174 6594 8c08 7065 702d 2530 3464 948c  ate...pep-%04d..
+0000a7e0: 0e72 6663 5f72 6566 6572 656e 6365 7394  .rfc_references.
+0000a7f0: 4e8c 0c72 6663 5f62 6173 655f 7572 6c94  N..rfc_base_url.
+0000a800: 8c26 6874 7470 733a 2f2f 6461 7461 7472  .&https://datatr
+0000a810: 6163 6b65 722e 6965 7466 2e6f 7267 2f64  acker.ietf.org/d
+0000a820: 6f63 2f68 746d 6c2f 948c 0974 6162 5f77  oc/html/...tab_w
+0000a830: 6964 7468 944b 088c 1d74 7269 6d5f 666f  idth.K...trim_fo
+0000a840: 6f74 6e6f 7465 5f72 6566 6572 656e 6365  otnote_reference
+0000a850: 5f73 7061 6365 9489 8c10 7379 6e74 6178  _space....syntax
+0000a860: 5f68 6967 686c 6967 6874 948c 046c 6f6e  _highlight...lon
+0000a870: 6794 8c0c 736d 6172 745f 7175 6f74 6573  g...smart_quotes
+0000a880: 9488 8c13 736d 6172 7471 756f 7465 735f  ....smartquotes_
+0000a890: 6c6f 6361 6c65 7394 5d94 8c1d 6368 6172  locales.]...char
+0000a8a0: 6163 7465 725f 6c65 7665 6c5f 696e 6c69  acter_level_inli
+0000a8b0: 6e65 5f6d 6172 6b75 7094 898c 0e64 6f63  ne_markup....doc
+0000a8c0: 7469 746c 655f 7866 6f72 6d94 898c 0d64  title_xform....d
+0000a8d0: 6f63 696e 666f 5f78 666f 726d 944b 018c  ocinfo_xform.K..
+0000a8e0: 1273 6563 7473 7562 7469 746c 655f 7866  .sectsubtitle_xf
+0000a8f0: 6f72 6d94 898c 0d69 6d61 6765 5f6c 6f61  orm....image_loa
+0000a900: 6469 6e67 948c 046c 696e 6b94 8c10 656d  ding...link...em
+0000a910: 6265 645f 7374 796c 6573 6865 6574 9489  bed_stylesheet..
+0000a920: 8c15 636c 6f61 6b5f 656d 6169 6c5f 6164  ..cloak_email_ad
+0000a930: 6472 6573 7365 7394 888c 1173 6563 7469  dresses....secti
+0000a940: 6f6e 5f73 656c 665f 6c69 6e6b 9489 8c03  on_self_link....
+0000a950: 656e 7694 4e75 628c 0872 6570 6f72 7465  env.Nub..reporte
+0000a960: 7294 4e8c 1069 6e64 6972 6563 745f 7461  r.N..indirect_ta
+0000a970: 7267 6574 7394 5d94 8c11 7375 6273 7469  rgets.]...substi
+0000a980: 7475 7469 6f6e 5f64 6566 7394 7d94 8c12  tution_defs.}...
+0000a990: 7375 6273 7469 7475 7469 6f6e 5f6e 616d  substitution_nam
+0000a9a0: 6573 947d 948c 0872 6566 6e61 6d65 7394  es.}...refnames.
+0000a9b0: 7d94 8c06 7265 6669 6473 947d 948c 076e  }...refids.}...n
+0000a9c0: 616d 6569 6473 947d 9428 6a3e 0a00 006a  ameids.}.(j>...j
+0000a9d0: 3b0a 0000 68dd 68da 68af 68ac 6a8f 0100  ;...h.h.h.h.j...
+0000a9e0: 006a 8c01 0000 6a80 0100 006a 7d01 0000  .j....j....j}...
+0000a9f0: 6a25 0900 006a 2209 0000 6a61 0200 006a  j%...j"...ja...j
+0000aa00: 5e02 0000 6a4e 0200 006a 4b02 0000 6a1e  ^...jN...jK...j.
+0000aa10: 0300 006a 1b03 0000 6a32 0800 006a 2f08  ...j....j2...j/.
+0000aa20: 0000 6ae2 0400 006a df04 0000 6a18 0600  ..j....j....j...
+0000aa30: 006a 1506 0000 6a8f 0600 006a 8c06 0000  .j....j....j....
+0000aa40: 6a06 0700 006a 0307 0000 6a4b 0700 006a  j....j....jK...j
+0000aa50: 4807 0000 6a2a 0800 006a 2708 0000 6a1d  H...j*...j'...j.
+0000aa60: 0900 006a 1a09 0000 6adc 0800 006a d908  ...j....j....j..
+0000aa70: 0000 6a15 0900 006a 1209 0000 6aa4 0900  ..j....j....j...
+0000aa80: 006a a109 0000 6a36 0a00 006a 330a 0000  .j....j6...j3...
+0000aa90: 758c 096e 616d 6574 7970 6573 947d 9428  u..nametypes.}.(
+0000aaa0: 6a3e 0a00 0089 68dd 8968 af88 6a8f 0100  j>....h..h..j...
+0000aab0: 0089 6a80 0100 0088 6a25 0900 0089 6a61  ..j.....j%....ja
+0000aac0: 0200 0089 6a4e 0200 0088 6a1e 0300 0089  ....jN....j.....
+0000aad0: 6a32 0800 0089 6ae2 0400 0089 6a18 0600  j2....j.....j...
+0000aae0: 0089 6a8f 0600 0089 6a06 0700 0089 6a4b  ..j.....j.....jK
+0000aaf0: 0700 0089 6a2a 0800 0089 6a1d 0900 0089  ....j*....j.....
+0000ab00: 6adc 0800 0089 6a15 0900 0089 6aa4 0900  j.....j.....j...
+0000ab10: 0089 6a36 0a00 0089 7568 197d 9428 6a3b  ..j6....uh.}.(j;
+0000ab20: 0a00 0068 2c68 da68 3f68 ac68 a66a 8c01  ...h,h.h?h.h.j..
+0000ab30: 0000 68e0 6a7d 0100 006a 7701 0000 6a22  ..h.j}...jw...j"
+0000ab40: 0900 006a 9201 0000 6a5e 0200 006a ea01  ...j....j^...j..
+0000ab50: 0000 6a4b 0200 006a 4502 0000 6a1b 0300  ..jK...jE...j...
+0000ab60: 006a 6402 0000 6a2f 0800 006a 2103 0000  .jd...j/...j!...
+0000ab70: 6adf 0400 006a 0804 0000 6a15 0600 006a  j....j....j....j
+0000ab80: e504 0000 6a8c 0600 006a 1b06 0000 6a03  ....j....j....j.
+0000ab90: 0700 006a 9206 0000 6a48 0700 006a 0907  ...j....jH...j..
+0000aba0: 0000 6a27 0800 006a 4e07 0000 6a1a 0900  ..j'...jN...j...
+0000abb0: 006a 3508 0000 6ad9 0800 006a 8608 0000  .j5...j....j....
+0000abc0: 6a12 0900 006a df08 0000 6aa1 0900 006a  j....j....j....j
+0000abd0: 2809 0000 6a33 0a00 006a a709 0000 758c  (...j3...j....u.
+0000abe0: 0d66 6f6f 746e 6f74 655f 7265 6673 947d  .footnote_refs.}
+0000abf0: 948c 0d63 6974 6174 696f 6e5f 7265 6673  ...citation_refs
+0000ac00: 947d 948c 0d61 7574 6f66 6f6f 746e 6f74  .}...autofootnot
+0000ac10: 6573 945d 948c 1161 7574 6f66 6f6f 746e  es.]...autofootn
+0000ac20: 6f74 655f 7265 6673 945d 948c 1073 796d  ote_refs.]...sym
+0000ac30: 626f 6c5f 666f 6f74 6e6f 7465 7394 5d94  bol_footnotes.].
+0000ac40: 8c14 7379 6d62 6f6c 5f66 6f6f 746e 6f74  ..symbol_footnot
+0000ac50: 655f 7265 6673 945d 948c 0966 6f6f 746e  e_refs.]...footn
+0000ac60: 6f74 6573 945d 948c 0963 6974 6174 696f  otes.]...citatio
+0000ac70: 6e73 945d 948c 1261 7574 6f66 6f6f 746e  ns.]...autofootn
+0000ac80: 6f74 655f 7374 6172 7494 4b01 8c15 7379  ote_start.K...sy
+0000ac90: 6d62 6f6c 5f66 6f6f 746e 6f74 655f 7374  mbol_footnote_st
+0000aca0: 6172 7494 4b00 8c0a 6964 5f63 6f75 6e74  art.K...id_count
+0000acb0: 6572 948c 0b63 6f6c 6c65 6374 696f 6e73  er...collections
+0000acc0: 948c 0743 6f75 6e74 6572 9493 947d 9485  ...Counter...}..
+0000acd0: 9452 948c 0e70 6172 7365 5f6d 6573 7361  .R...parse_messa
+0000ace0: 6765 7394 5d94 8c12 7472 616e 7366 6f72  ges.]...transfor
+0000acf0: 6d5f 6d65 7373 6167 6573 945d 948c 0b74  m_messages.]...t
+0000ad00: 7261 6e73 666f 726d 6572 944e 8c0b 696e  ransformer.N..in
+0000ad10: 636c 7564 655f 6c6f 6794 5d94 8c09 696e  clude_log.]...in
+0000ad20: 6465 782e 7273 7494 284e 4e4e 4e74 9486  dex.rst.(NNNNt..
+0000ad30: 9461 8c0a 6465 636f 7261 7469 6f6e 944e  .a..decoration.N
+0000ad40: 6826 6803 7562 2e                        h&h.ub.
```

### Comparing `decore_Base-0.0.20/docs/page/html/_static/basic.css` & `decore_Base-0.0.21/docs/page/html/_static/basic.css`

 * *Files identical despite different names*

### Comparing `decore_Base-0.0.20/docs/page/html/_static/clipboard.min.js` & `decore_Base-0.0.21/docs/page/html/_static/clipboard.min.js`

 * *Files identical despite different names*

### Comparing `decore_Base-0.0.20/docs/page/html/_static/copybutton.css` & `decore_Base-0.0.21/docs/page/html/_static/copybutton.css`

 * *Files identical despite different names*

### Comparing `decore_Base-0.0.20/docs/page/html/_static/copybutton.js` & `decore_Base-0.0.21/docs/page/html/_static/copybutton.js`

 * *Files identical despite different names*

### Comparing `decore_Base-0.0.20/docs/page/html/_static/copybutton_funcs.js` & `decore_Base-0.0.21/docs/page/html/_static/copybutton_funcs.js`

 * *Files identical despite different names*

### Comparing `decore_Base-0.0.20/docs/page/html/_static/doctools.js` & `decore_Base-0.0.21/docs/page/html/_static/doctools.js`

 * *Files identical despite different names*

### Comparing `decore_Base-0.0.20/docs/page/html/_static/favicon.ico` & `decore_Base-0.0.21/docs/page/html/_static/favicon.ico`

 * *Files identical despite different names*

### Comparing `decore_Base-0.0.20/docs/page/html/_static/language_data.js` & `decore_Base-0.0.21/docs/page/html/_static/language_data.js`

 * *Files identical despite different names*

### Comparing `decore_Base-0.0.20/docs/page/html/_static/logo.png` & `decore_Base-0.0.21/docs/page/html/_static/logo.png`

 * *Files identical despite different names*

### Comparing `decore_Base-0.0.20/docs/page/html/_static/pygments.css` & `decore_Base-0.0.21/docs/page/html/_static/pygments.css`

 * *Files identical despite different names*

### Comparing `decore_Base-0.0.20/docs/page/html/_static/scripts/bootstrap.js` & `decore_Base-0.0.21/docs/page/html/_static/scripts/bootstrap.js`

 * *Files identical despite different names*

### Comparing `decore_Base-0.0.20/docs/page/html/_static/scripts/bootstrap.js.map` & `decore_Base-0.0.21/docs/page/html/_static/scripts/bootstrap.js.map`

 * *Files identical despite different names*

### Comparing `decore_Base-0.0.20/docs/page/html/_static/scripts/pydata-sphinx-theme.js` & `decore_Base-0.0.21/docs/page/html/_static/scripts/pydata-sphinx-theme.js`

 * *Files identical despite different names*

### Comparing `decore_Base-0.0.20/docs/page/html/_static/scripts/pydata-sphinx-theme.js.map` & `decore_Base-0.0.21/docs/page/html/_static/scripts/pydata-sphinx-theme.js.map`

 * *Files identical despite different names*

### Comparing `decore_Base-0.0.20/docs/page/html/_static/searchtools.js` & `decore_Base-0.0.21/docs/page/html/_static/searchtools.js`

 * *Files identical despite different names*

### Comparing `decore_Base-0.0.20/docs/page/html/_static/sphinx_highlight.js` & `decore_Base-0.0.21/docs/page/html/_static/sphinx_highlight.js`

 * *Files identical despite different names*

### Comparing `decore_Base-0.0.20/docs/page/html/_static/styles/bootstrap.css` & `decore_Base-0.0.21/docs/page/html/_static/styles/bootstrap.css`

 * *Files identical despite different names*

### Comparing `decore_Base-0.0.20/docs/page/html/_static/styles/pydata-sphinx-theme.css` & `decore_Base-0.0.21/docs/page/html/_static/styles/pydata-sphinx-theme.css`

 * *Files identical despite different names*

### Comparing `decore_Base-0.0.20/docs/page/html/_static/vendor/fontawesome/6.1.2/LICENSE.txt` & `decore_Base-0.0.21/docs/page/html/_static/vendor/fontawesome/6.1.2/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `decore_Base-0.0.20/docs/page/html/_static/vendor/fontawesome/6.1.2/css/all.min.css` & `decore_Base-0.0.21/docs/page/html/_static/vendor/fontawesome/6.1.2/css/all.min.css`

 * *Files identical despite different names*

### Comparing `decore_Base-0.0.20/docs/page/html/_static/vendor/fontawesome/6.1.2/webfonts/fa-brands-400.ttf` & `decore_Base-0.0.21/docs/page/html/_static/vendor/fontawesome/6.1.2/webfonts/fa-brands-400.ttf`

 * *Files identical despite different names*

### Comparing `decore_Base-0.0.20/docs/page/html/_static/vendor/fontawesome/6.1.2/webfonts/fa-brands-400.woff2` & `decore_Base-0.0.21/docs/page/html/_static/vendor/fontawesome/6.1.2/webfonts/fa-brands-400.woff2`

 * *Files identical despite different names*

### Comparing `decore_Base-0.0.20/docs/page/html/_static/vendor/fontawesome/6.1.2/webfonts/fa-regular-400.ttf` & `decore_Base-0.0.21/docs/page/html/_static/vendor/fontawesome/6.1.2/webfonts/fa-regular-400.ttf`

 * *Files identical despite different names*

### Comparing `decore_Base-0.0.20/docs/page/html/_static/vendor/fontawesome/6.1.2/webfonts/fa-regular-400.woff2` & `decore_Base-0.0.21/docs/page/html/_static/vendor/fontawesome/6.1.2/webfonts/fa-regular-400.woff2`

 * *Files identical despite different names*

### Comparing `decore_Base-0.0.20/docs/page/html/_static/vendor/fontawesome/6.1.2/webfonts/fa-solid-900.ttf` & `decore_Base-0.0.21/docs/page/html/_static/vendor/fontawesome/6.1.2/webfonts/fa-solid-900.ttf`

 * *Files identical despite different names*

### Comparing `decore_Base-0.0.20/docs/page/html/_static/vendor/fontawesome/6.1.2/webfonts/fa-solid-900.woff2` & `decore_Base-0.0.21/docs/page/html/_static/vendor/fontawesome/6.1.2/webfonts/fa-solid-900.woff2`

 * *Files identical despite different names*

### Comparing `decore_Base-0.0.20/docs/page/html/_static/vendor/fontawesome/6.1.2/webfonts/fa-v4compatibility.ttf` & `decore_Base-0.0.21/docs/page/html/_static/vendor/fontawesome/6.1.2/webfonts/fa-v4compatibility.ttf`

 * *Files identical despite different names*

### Comparing `decore_Base-0.0.20/docs/page/html/_static/vendor/fontawesome/6.1.2/webfonts/fa-v4compatibility.woff2` & `decore_Base-0.0.21/docs/page/html/_static/vendor/fontawesome/6.1.2/webfonts/fa-v4compatibility.woff2`

 * *Files identical despite different names*

### Comparing `decore_Base-0.0.20/docs/page/html/_static/webpack-macros.html` & `decore_Base-0.0.21/docs/page/html/_static/webpack-macros.html`

 * *Files identical despite different names*

### Comparing `decore_Base-0.0.20/docs/page/html/decore.html` & `decore_Base-0.0.21/docs/page/html/search.html`

 * *Files 6% similar despite different names*

```diff
@@ -3,17 +3,15 @@
 <!DOCTYPE html>
 
 
 <html lang="en" >
 
   <head>
     <meta charset="utf-8" />
-    <meta name="viewport" content="width=device-width, initial-scale=1.0" /><meta name="generator" content="Docutils 0.19: https://docutils.sourceforge.io/" />
-    <link href="_static/favicon.ico" rel="icon" type="image/x-icon">
-    <title>Decorator reference &#8212; decore Base | UI fastly 0.0.18 documentation</title>
+    <meta name="viewport" content="width=device-width, initial-scale=1.0" /><title>Search - decore Base | UI fastly 0.0.18 documentation</title>
   
   
   
   <script data-cfasync="false">
     document.documentElement.dataset.mode = localStorage.getItem("mode") || "";
     document.documentElement.dataset.theme = localStorage.getItem("theme") || "light";
   </script>
@@ -38,17 +36,20 @@
 <link rel="preload" as="script" href="_static/scripts/pydata-sphinx-theme.js?digest=e353d410970836974a52" />
 
     <script data-url_root="./" id="documentation_options" src="_static/documentation_options.js"></script>
     <script src="_static/doctools.js"></script>
     <script src="_static/sphinx_highlight.js"></script>
     <script src="_static/clipboard.min.js"></script>
     <script src="_static/copybutton.js"></script>
-    <script>DOCUMENTATION_OPTIONS.pagename = 'decore';</script>
+    <script>DOCUMENTATION_OPTIONS.pagename = 'search';</script>
+  <script src="_static/searchtools.js"></script>
+  <script src="_static/language_data.js"></script>
+  <script src="searchindex.js"></script>
     <link rel="index" title="Index" href="genindex.html" />
-    <link rel="search" title="Search" href="search.html" />
+    <link rel="search" title="Search" href="#" />
   <meta name="viewport" content="width=device-width, initial-scale=1"/>
   <meta name="docsearch:language" content="en"/>
   </head>
   
   
   <body data-bs-spy="scroll" data-bs-target=".bd-toc-nav" data-offset="180" data-bs-root-margin="0px 0px -60%" data-default-mode="">
 
@@ -68,15 +69,15 @@
           id="__secondary"/>
   <label class="overlay overlay-secondary" for="__secondary"></label>
   
   <div class="search-button__wrapper">
     <div class="search-button__overlay"></div>
     <div class="search-button__search-container">
 <form class="bd-search d-flex align-items-center"
-      action="search.html"
+      action="#"
       method="get">
   <i class="fa-solid fa-magnifying-glass"></i>
   <input type="search"
          class="form-control"
          name="q"
          id="search-input"
          placeholder="Search the docs ..."
@@ -178,18 +179,14 @@
   </button>
 `);
 </script>
     </div>
   
 
   
-    <label class="sidebar-toggle secondary-toggle" for="__secondary">
-      <span class="fa-solid fa-outdent"></span>
-    </label>
-  
 </div>
 
     </nav>
   
   <div class="bd-container">
     <div class="bd-container__inner bd-page-width">
       
@@ -246,55 +243,54 @@
       
       <main id="main-content" class="bd-main">
         
         
           <div class="bd-content">
             <div class="bd-article-container">
               
-              <div class="bd-header-article">
-<div class="header-article-items header-article__inner">
-  
-    <div class="header-article-items__start">
-      
-        <div class="header-article-item">
-
-
-
-<nav aria-label="Breadcrumbs">
-  <ul class="bd-breadcrumbs" role="navigation" aria-label="Breadcrumb">
-    
-    <li class="breadcrumb-item breadcrumb-home">
-      <a href="index.html" class="nav-link" aria-label="Home">
-        <i class="fa-solid fa-home"></i>
-      </a>
-    </li>
-    <li class="breadcrumb-item active" aria-current="page">Decorator reference</li>
-  </ul>
-</nav>
-</div>
-      
-    </div>
-  
-  
-</div>
-</div>
-              
+              <div class="bd-header-article"></div>
               
               
-                
-<div id="searchbox"></div>
-                <article class="bd-article" role="main">
-                  
-  <section id="module-decore_base.decore">
-<span id="decorator-reference"></span><h1>Decorator reference<a class="headerlink" href="#module-decore_base.decore" title="Permalink to this heading">#</a></h1>
-</section>
-
+  <div class="bd-search-container">
+    <h1>Search</h1>
+    <noscript>
+      <div class="admonition error">
+        <p class="admonition-title">Error</p>
+        <p>Please activate JavaScript to enable the search functionality.</p>
+      </div>
+    </noscript>
+    
+<form class="bd-search d-flex align-items-center"
+      action="#"
+      method="get">
+  <i class="fa-solid fa-magnifying-glass"></i>
+  <input type="search"
+         class="form-control"
+         name="q"
+         id="search-input"
+         placeholder="Search the docs ..."
+         aria-label="Search the docs ..."
+         autocomplete="off"
+         autocorrect="off"
+         autocapitalize="off"
+         spellcheck="false"/>
+  <span class="search-button__kbd-shortcut"><kbd class="kbd-shortcut__modifier">Ctrl</kbd>+<kbd>K</kbd></span>
+</form>
+    <div id="search-results"></div>
+  </div>
+  <script>
+    // Activate the search field on page load
+    let searchInput = document.querySelector("form.bd-search input");
+    if (searchInput) {
+        searchInput.focus();
+        searchInput.select();
+        console.log("[PST]: Set focus on search field.");
+    }
+  </script>
 
-                </article>
-              
               
               
                 <footer class="bd-footer-article">
                   
 <div class="footer-article-items footer-article__inner">
   
     <div class="footer-article-item"><!-- Previous / next buttons -->
@@ -305,26 +301,14 @@
 
                 </footer>
               
             </div>
             
             
               
-                <div class="bd-sidebar-secondary bd-toc"><div class="sidebar-secondary-items sidebar-secondary__inner">
-
-  <div class="sidebar-secondary-item">
-  <div class="tocsection sourcelink">
-    <a href="_sources/decore.rst.txt">
-      <i class="fa-solid fa-file-lines"></i> Show Source
-    </a>
-  </div>
-</div>
-
-</div></div>
-              
             
           </div>
           <footer class="bd-footer-content">
             
           </footer>
         
       </main>
```

#### html2text {}

```diff
@@ -12,26 +12,24 @@
 
 
 
 
 
 
 
-
 Skip_to_main_content ⁰  ⁰
  [Unknown INPUT type] Ctrl+K
 
 [Logo_image]
 decore Base | UI fastly
 Site Navigation
-
 Site Navigation
-    * Decorator reference
-
-****** Decorator reference# ******
+****** Search ******
+Error
+Please activate JavaScript to enable the search functionality.
+ [Unknown INPUT type] Ctrl+K
 
- Show_Source
 
 
 Â© Copyright 2023, Jean Rohark.
 Created using Sphinx 6.2.1.
 Built with the PyData_Sphinx_Theme 0.13.3.
```

### Comparing `decore_Base-0.0.20/docs/page/html/genindex.html` & `decore_Base-0.0.21/docs/page/html/genindex.html`

 * *Files 4% similar despite different names*

```diff
@@ -253,55 +253,16 @@
 <div id="searchbox"></div>
                 <article class="bd-article" role="main">
                   
 
 <h1 id="index">Index</h1>
 
 <div class="genindex-jumpbox">
- <a href="#D"><strong>D</strong></a>
- | <a href="#M"><strong>M</strong></a>
  
 </div>
-<h2 id="D">D</h2>
-<table style="width: 100%" class="indextable genindextable"><tr>
-  <td style="width: 33%; vertical-align: top;"><ul>
-      <li>
-    decore_base.classes.decore_model
-
-      <ul>
-        <li><a href="model.html#module-decore_base.classes.decore_model">module</a>
-</li>
-      </ul></li>
-  </ul></td>
-  <td style="width: 33%; vertical-align: top;"><ul>
-      <li>
-    decore_base.decore
-
-      <ul>
-        <li><a href="decore.html#module-decore_base.decore">module</a>
-</li>
-      </ul></li>
-  </ul></td>
-</tr></table>
-
-<h2 id="M">M</h2>
-<table style="width: 100%" class="indextable genindextable"><tr>
-  <td style="width: 33%; vertical-align: top;"><ul>
-      <li>
-    module
-
-      <ul>
-        <li><a href="model.html#module-decore_base.classes.decore_model">decore_base.classes.decore_model</a>
-</li>
-        <li><a href="decore.html#module-decore_base.decore">decore_base.decore</a>
-</li>
-      </ul></li>
-  </ul></td>
-</tr></table>
-
 
 
                 </article>
               
               
               
                 <footer class="bd-footer-article">
```

#### html2text {}

```diff
@@ -20,21 +20,13 @@
  [Unknown INPUT type] Ctrl+K
 
 [Logo_image]
 decore Base | UI fastly
 Site Navigation
 Site Navigation
 ****** Index ******
-D | M
-***** D *****
-    * decore_base.classes.decore_model     * decore_base.decore
-          o module                               o module
-***** M *****
-    * module
-          o decore_base.classes.decore_model
-          o decore_base.decore
 
 
 
 Â© Copyright 2023, Jean Rohark.
 Created using Sphinx 6.2.1.
 Built with the PyData_Sphinx_Theme 0.13.3.
```

### Comparing `decore_Base-0.0.20/docs/page/html/index.html` & `decore_Base-0.0.21/docs/page/html/index.html`

 * *Files 2% similar despite different names*

```diff
@@ -351,14 +351,22 @@
    <span class="k">pass</span>
 </pre></div>
 </div>
 <div class="admonition note">
 <p class="admonition-title">Note</p>
 <p>To use the previously created model, we import it into the Base class and pass it to the <code class="docutils literal notranslate"><span class="pre">model</span></code> parameter.</p>
 </div>
+<div class="admonition warning">
+<p class="admonition-title">Warning</p>
+<p>In order for the Python interpreter to be able to process the base classes, we have to import them into the __init__.py file in the <strong>bases</strong> directory. The order of the individual imports also determines the order in <strong>decore Front</strong>.</p>
+<p>We edit the <strong>__init__.py</strong> file and insert the following code:</p>
+<div class="highlight-python notranslate"><div class="highlight"><pre><span></span><span class="kn">from</span> <span class="nn">.first_base</span> <span class="kn">import</span> <span class="n">First_base</span>
+</pre></div>
+</div>
+</div>
 </section>
 <section id="view">
 <h4>View<a class="headerlink" href="#view" title="Permalink to this heading">#</a></h4>
 <p>Views are used by the decore application to present the data sets in the <strong>decore Front</strong> web application.</p>
 <p>With the view decorator we can now create a view component and link it to the previously created base class.</p>
 <p>We now edit the <strong>first_base.py</strong> file again and extend the code as follows:</p>
 <div class="highlight-python notranslate"><div class="highlight"><pre><span></span><span class="kn">from</span> <span class="nn">decore_base</span> <span class="kn">import</span> <span class="n">decore</span>
```

#### html2text {}

```diff
@@ -123,14 +123,20 @@
 
 @decore.base(title='First Base', icon='mdi-home', model=First_model)
 class First_base:
    pass
 Note
 To use the previously created model, we import it into the Base class and pass
 it to the model parameter.
+Warning
+In order for the Python interpreter to be able to process the base classes, we
+have to import them into the __init__.py file in the bases directory. The order
+of the individual imports also determines the order in decore Front.
+We edit the __init__.py file and insert the following code:
+from .first_base import First_base
 
 *** View# ***
 Views are used by the decore application to present the data sets in the decore
 Front web application.
 With the view decorator we can now create a view component and link it to the
 previously created base class.
 We now edit the first_base.py file again and extend the code as follows:
```

### Comparing `decore_Base-0.0.20/docs/state/keybase.kdbx` & `decore_Base-0.0.21/docs/state/keybase.kdbx`

 * *Files identical despite different names*

### Comparing `decore_Base-0.0.20/docs/state/querybase.db` & `decore_Base-0.0.21/docs/state/querybase.db`

 * *Files identical despite different names*

### Comparing `decore_Base-0.0.20/requirements.txt` & `decore_Base-0.0.21/requirements.txt`

 * *Files identical despite different names*

### Comparing `decore_Base-0.0.20/setup.cfg` & `decore_Base-0.0.21/setup.cfg`

 * *Files identical despite different names*

