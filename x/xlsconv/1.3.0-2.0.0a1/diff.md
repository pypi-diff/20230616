# Comparing `tmp/xlsconv-1.3.0.tar.gz` & `tmp/xlsconv-2.0.0a1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/xlsconv-1.3.0.tar", last modified: Tue Apr  5 04:41:24 2022, max compression
+gzip compressed data, was "xlsconv-2.0.0a1.tar", last modified: Fri Jun 16 18:20:17 2023, max compression
```

## Comparing `xlsconv-1.3.0.tar` & `xlsconv-2.0.0a1.tar`

### file list

```diff
@@ -1,89 +1,56 @@
-drwxr-xr-x   0 sheppard  (1000) sheppard  (1000)        0 2022-04-05 04:41:24.000000 xlsconv-1.3.0/
--rw-r--r--   0 sheppard  (1000) sheppard  (1000)       51 2022-04-05 04:37:34.000000 xlsconv-1.3.0/.gitignore
-drwxr-xr-x   0 sheppard  (1000) sheppard  (1000)        0 2022-04-05 04:41:24.000000 xlsconv-1.3.0/tests/
--rw-r--r--   0 sheppard  (1000) sheppard  (1000)     1716 2022-04-05 04:37:34.000000 xlsconv-1.3.0/tests/test_survey.py
--rw-r--r--   0 sheppard  (1000) sheppard  (1000)        0 2022-04-05 04:37:34.000000 xlsconv-1.3.0/tests/__init__.py
-drwxr-xr-x   0 sheppard  (1000) sheppard  (1000)        0 2022-04-05 04:41:24.000000 xlsconv-1.3.0/tests/files/
--rw-r--r--   0 sheppard  (1000) sheppard  (1000)      625 2022-04-05 04:37:34.000000 xlsconv-1.3.0/tests/files/select.csv
-drwxr-xr-x   0 sheppard  (1000) sheppard  (1000)        0 2022-04-05 04:41:24.000000 xlsconv-1.3.0/tests/files/nestedfk/
--rw-r--r--   0 sheppard  (1000) sheppard  (1000)       94 2022-04-05 04:37:34.000000 xlsconv-1.3.0/tests/files/nestedfk/admin.py
--rw-r--r--   0 sheppard  (1000) sheppard  (1000)     6599 2022-04-05 04:37:34.000000 xlsconv-1.3.0/tests/files/nestedfk/edit.html
--rw-r--r--   0 sheppard  (1000) sheppard  (1000)      890 2022-04-05 04:37:34.000000 xlsconv-1.3.0/tests/files/nestedfk/models.py
--rw-r--r--   0 sheppard  (1000) sheppard  (1000)      147 2022-04-05 04:37:34.000000 xlsconv-1.3.0/tests/files/nestedfk/wizard.py
--rw-r--r--   0 sheppard  (1000) sheppard  (1000)      249 2022-04-05 04:37:34.000000 xlsconv-1.3.0/tests/files/nestedfk/rest.py
--rw-r--r--   0 sheppard  (1000) sheppard  (1000)     2748 2022-04-05 04:37:34.000000 xlsconv-1.3.0/tests/files/nestedfk/list.html
--rw-r--r--   0 sheppard  (1000) sheppard  (1000)      730 2022-04-05 04:37:34.000000 xlsconv-1.3.0/tests/files/nestedfk/serializers.py
--rw-r--r--   0 sheppard  (1000) sheppard  (1000)     1620 2022-04-05 04:37:34.000000 xlsconv-1.3.0/tests/files/nestedfk/detail.html
--rw-r--r--   0 sheppard  (1000) sheppard  (1000)       76 2022-04-05 04:37:34.000000 xlsconv-1.3.0/tests/files/nestedfk/popup.html
-drwxr-xr-x   0 sheppard  (1000) sheppard  (1000)        0 2022-04-05 04:41:24.000000 xlsconv-1.3.0/tests/files/input_types/
--rw-r--r--   0 sheppard  (1000) sheppard  (1000)      123 2022-04-05 04:37:34.000000 xlsconv-1.3.0/tests/files/input_types/admin.py
--rw-r--r--   0 sheppard  (1000) sheppard  (1000)    12345 2022-04-05 04:37:34.000000 xlsconv-1.3.0/tests/files/input_types/edit.html
--rw-r--r--   0 sheppard  (1000) sheppard  (1000)     2324 2022-04-05 04:37:34.000000 xlsconv-1.3.0/tests/files/input_types/models.py
--rw-r--r--   0 sheppard  (1000) sheppard  (1000)       85 2022-04-05 04:37:34.000000 xlsconv-1.3.0/tests/files/input_types/wizard.py
--rw-r--r--   0 sheppard  (1000) sheppard  (1000)      514 2022-04-05 04:37:34.000000 xlsconv-1.3.0/tests/files/input_types/rest.py
--rw-r--r--   0 sheppard  (1000) sheppard  (1000)     3039 2022-04-05 04:37:34.000000 xlsconv-1.3.0/tests/files/input_types/list.html
--rw-r--r--   0 sheppard  (1000) sheppard  (1000)      245 2022-04-05 04:37:34.000000 xlsconv-1.3.0/tests/files/input_types/serializers.py
--rw-r--r--   0 sheppard  (1000) sheppard  (1000)     1902 2022-04-05 04:37:34.000000 xlsconv-1.3.0/tests/files/input_types/detail.html
--rw-r--r--   0 sheppard  (1000) sheppard  (1000)       77 2022-04-05 04:37:34.000000 xlsconv-1.3.0/tests/files/input_types/popup.html
-drwxr-xr-x   0 sheppard  (1000) sheppard  (1000)        0 2022-04-05 04:41:24.000000 xlsconv-1.3.0/tests/files/select/
--rw-r--r--   0 sheppard  (1000) sheppard  (1000)       90 2022-04-05 04:37:34.000000 xlsconv-1.3.0/tests/files/select/admin.py
--rw-r--r--   0 sheppard  (1000) sheppard  (1000)     4020 2022-04-05 04:37:34.000000 xlsconv-1.3.0/tests/files/select/edit.html
--rw-r--r--   0 sheppard  (1000) sheppard  (1000)     1414 2022-04-05 04:37:34.000000 xlsconv-1.3.0/tests/files/select/models.py
--rw-r--r--   0 sheppard  (1000) sheppard  (1000)       77 2022-04-05 04:37:34.000000 xlsconv-1.3.0/tests/files/select/wizard.py
--rw-r--r--   0 sheppard  (1000) sheppard  (1000)      166 2022-04-05 04:37:34.000000 xlsconv-1.3.0/tests/files/select/rest.py
--rw-r--r--   0 sheppard  (1000) sheppard  (1000)     2736 2022-04-05 04:37:34.000000 xlsconv-1.3.0/tests/files/select/list.html
--rw-r--r--   0 sheppard  (1000) sheppard  (1000)      233 2022-04-05 04:37:34.000000 xlsconv-1.3.0/tests/files/select/serializers.py
--rw-r--r--   0 sheppard  (1000) sheppard  (1000)      991 2022-04-05 04:37:34.000000 xlsconv-1.3.0/tests/files/select/detail.html
--rw-r--r--   0 sheppard  (1000) sheppard  (1000)       74 2022-04-05 04:37:34.000000 xlsconv-1.3.0/tests/files/select/popup.html
--rw-r--r--   0 sheppard  (1000) sheppard  (1000)     8704 2022-04-05 04:37:34.000000 xlsconv-1.3.0/tests/files/input_types.xls
--rw-r--r--   0 sheppard  (1000) sheppard  (1000)      456 2022-04-05 04:37:34.000000 xlsconv-1.3.0/tests/files/repeat.csv
--rw-r--r--   0 sheppard  (1000) sheppard  (1000)      345 2022-04-05 04:37:34.000000 xlsconv-1.3.0/tests/files/nestedfk.csv
-drwxr-xr-x   0 sheppard  (1000) sheppard  (1000)        0 2022-04-05 04:41:24.000000 xlsconv-1.3.0/tests/files/repeat/
--rw-r--r--   0 sheppard  (1000) sheppard  (1000)       90 2022-04-05 04:37:34.000000 xlsconv-1.3.0/tests/files/repeat/admin.py
--rw-r--r--   0 sheppard  (1000) sheppard  (1000)     5402 2022-04-05 04:37:34.000000 xlsconv-1.3.0/tests/files/repeat/edit.html
--rw-r--r--   0 sheppard  (1000) sheppard  (1000)     1114 2022-04-05 04:37:34.000000 xlsconv-1.3.0/tests/files/repeat/models.py
--rw-r--r--   0 sheppard  (1000) sheppard  (1000)      139 2022-04-05 04:37:34.000000 xlsconv-1.3.0/tests/files/repeat/wizard.py
--rw-r--r--   0 sheppard  (1000) sheppard  (1000)      241 2022-04-05 04:37:34.000000 xlsconv-1.3.0/tests/files/repeat/rest.py
--rw-r--r--   0 sheppard  (1000) sheppard  (1000)     2736 2022-04-05 04:37:34.000000 xlsconv-1.3.0/tests/files/repeat/list.html
--rw-r--r--   0 sheppard  (1000) sheppard  (1000)     1305 2022-04-05 04:37:34.000000 xlsconv-1.3.0/tests/files/repeat/serializers.py
--rw-r--r--   0 sheppard  (1000) sheppard  (1000)     2065 2022-04-05 04:37:34.000000 xlsconv-1.3.0/tests/files/repeat/detail.html
--rw-r--r--   0 sheppard  (1000) sheppard  (1000)       74 2022-04-05 04:37:34.000000 xlsconv-1.3.0/tests/files/repeat/popup.html
--rw-r--r--   0 sheppard  (1000) sheppard  (1000)     3209 2022-04-05 04:37:34.000000 xlsconv-1.3.0/CODE_OF_CONDUCT.md
--rw-r--r--   0 sheppard  (1000) sheppard  (1000)     1106 2022-04-05 04:37:34.000000 xlsconv-1.3.0/LICENSE
--rw-r--r--   0 sheppard  (1000) sheppard  (1000)     5992 2022-04-05 04:37:34.000000 xlsconv-1.3.0/README.md
-drwxr-xr-x   0 sheppard  (1000) sheppard  (1000)        0 2022-04-05 04:41:24.000000 xlsconv-1.3.0/.github/
-drwxr-xr-x   0 sheppard  (1000) sheppard  (1000)        0 2022-04-05 04:41:24.000000 xlsconv-1.3.0/.github/workflows/
--rw-r--r--   0 sheppard  (1000) sheppard  (1000)     1076 2022-04-05 04:37:34.000000 xlsconv-1.3.0/.github/workflows/test.yml
-drwxr-xr-x   0 sheppard  (1000) sheppard  (1000)        0 2022-04-05 04:41:24.000000 xlsconv-1.3.0/xlsconv/
-drwxr-xr-x   0 sheppard  (1000) sheppard  (1000)        0 2022-04-05 04:41:24.000000 xlsconv-1.3.0/xlsconv/templates/
--rw-r--r--   0 sheppard  (1000) sheppard  (1000)     2783 2022-04-05 04:37:34.000000 xlsconv-1.3.0/xlsconv/templates/edit.html
-drwxr-xr-x   0 sheppard  (1000) sheppard  (1000)        0 2022-04-05 04:41:24.000000 xlsconv-1.3.0/xlsconv/templates/fields/
--rw-r--r--   0 sheppard  (1000) sheppard  (1000)     1750 2022-04-05 04:37:34.000000 xlsconv-1.3.0/xlsconv/templates/fields/photo.html
--rw-r--r--   0 sheppard  (1000) sheppard  (1000)      562 2022-04-05 04:37:34.000000 xlsconv-1.3.0/xlsconv/templates/fields/input.html
--rw-r--r--   0 sheppard  (1000) sheppard  (1000)      661 2022-04-05 04:37:34.000000 xlsconv-1.3.0/xlsconv/templates/fields/html_field.html
--rw-r--r--   0 sheppard  (1000) sheppard  (1000)      662 2022-04-05 04:37:34.000000 xlsconv-1.3.0/xlsconv/templates/fields/select.html
--rw-r--r--   0 sheppard  (1000) sheppard  (1000)      608 2022-04-05 04:37:34.000000 xlsconv-1.3.0/xlsconv/templates/fields/radio.html
--rw-r--r--   0 sheppard  (1000) sheppard  (1000)      590 2022-04-05 04:37:34.000000 xlsconv-1.3.0/xlsconv/templates/fields/foreignkey.html
--rw-r--r--   0 sheppard  (1000) sheppard  (1000)      405 2022-04-05 04:37:34.000000 xlsconv-1.3.0/xlsconv/templates/fields/geo.html
--rw-r--r--   0 sheppard  (1000) sheppard  (1000)      387 2022-04-05 04:37:34.000000 xlsconv-1.3.0/xlsconv/templates/fields/textarea.html
--rw-r--r--   0 sheppard  (1000) sheppard  (1000)      164 2022-04-05 04:37:34.000000 xlsconv-1.3.0/xlsconv/templates/fields/note.html
--rw-r--r--   0 sheppard  (1000) sheppard  (1000)     3184 2022-04-05 04:37:34.000000 xlsconv-1.3.0/xlsconv/templates/list.html
--rw-r--r--   0 sheppard  (1000) sheppard  (1000)     2905 2022-04-05 04:37:34.000000 xlsconv-1.3.0/xlsconv/templates/detail.html
--rw-r--r--   0 sheppard  (1000) sheppard  (1000)       95 2022-04-05 04:37:34.000000 xlsconv-1.3.0/xlsconv/templates/popup.html
--rw-r--r--   0 sheppard  (1000) sheppard  (1000)     4220 2022-04-05 04:37:34.000000 xlsconv-1.3.0/xlsconv/html.py
--rw-r--r--   0 sheppard  (1000) sheppard  (1000)     3172 2022-04-05 04:37:34.000000 xlsconv-1.3.0/xlsconv/ast.py
--rw-r--r--   0 sheppard  (1000) sheppard  (1000)      367 2022-04-05 04:37:34.000000 xlsconv-1.3.0/xlsconv/renderer.py
--rw-r--r--   0 sheppard  (1000) sheppard  (1000)    17296 2022-04-05 04:37:34.000000 xlsconv-1.3.0/xlsconv/django.py
--rw-r--r--   0 sheppard  (1000) sheppard  (1000)     2200 2022-04-05 04:37:34.000000 xlsconv-1.3.0/xlsconv/parser.py
--rw-r--r--   0 sheppard  (1000) sheppard  (1000)      270 2022-04-05 04:37:34.000000 xlsconv-1.3.0/xlsconv/__init__.py
--rw-r--r--   0 sheppard  (1000) sheppard  (1000)       38 2022-04-05 04:41:24.000000 xlsconv-1.3.0/setup.cfg
--rw-r--r--   0 sheppard  (1000) sheppard  (1000)     1693 2022-04-05 04:37:34.000000 xlsconv-1.3.0/setup.py
-drwxr-xr-x   0 sheppard  (1000) sheppard  (1000)        0 2022-04-05 04:41:24.000000 xlsconv-1.3.0/xlsconv.egg-info/
--rw-r--r--   0 sheppard  (1000) sheppard  (1000)        8 2022-04-05 04:41:24.000000 xlsconv-1.3.0/xlsconv.egg-info/top_level.txt
--rw-r--r--   0 sheppard  (1000) sheppard  (1000)        1 2022-04-05 04:41:24.000000 xlsconv-1.3.0/xlsconv.egg-info/dependency_links.txt
--rw-r--r--   0 sheppard  (1000) sheppard  (1000)      105 2022-04-05 04:41:24.000000 xlsconv-1.3.0/xlsconv.egg-info/entry_points.txt
--rw-r--r--   0 sheppard  (1000) sheppard  (1000)     2109 2022-04-05 04:41:24.000000 xlsconv-1.3.0/xlsconv.egg-info/SOURCES.txt
--rw-r--r--   0 sheppard  (1000) sheppard  (1000)       34 2022-04-05 04:41:24.000000 xlsconv-1.3.0/xlsconv.egg-info/requires.txt
--rw-r--r--   0 sheppard  (1000) sheppard  (1000)     7534 2022-04-05 04:41:24.000000 xlsconv-1.3.0/xlsconv.egg-info/PKG-INFO
--rw-r--r--   0 sheppard  (1000) sheppard  (1000)     3314 2022-04-05 04:37:34.000000 xlsconv-1.3.0/CONTRIBUTING.md
--rw-r--r--   0 sheppard  (1000) sheppard  (1000)     7534 2022-04-05 04:41:24.000000 xlsconv-1.3.0/PKG-INFO
+drwxr-xr-x   0 sheppard  (1000) sheppard  (1000)        0 2023-06-16 18:20:17.376063 xlsconv-2.0.0a1/
+drwxr-xr-x   0 sheppard  (1000) sheppard  (1000)        0 2023-06-16 18:20:17.092082 xlsconv-2.0.0a1/.github/
+drwxr-xr-x   0 sheppard  (1000) sheppard  (1000)        0 2023-06-16 18:20:17.146066 xlsconv-2.0.0a1/.github/workflows/
+-rw-r--r--   0 sheppard  (1000) sheppard  (1000)     1218 2023-06-16 18:18:42.000000 xlsconv-2.0.0a1/.github/workflows/test.yml
+-rw-r--r--   0 sheppard  (1000) sheppard  (1000)       51 2023-06-16 18:18:42.000000 xlsconv-2.0.0a1/.gitignore
+-rw-r--r--   0 sheppard  (1000) sheppard  (1000)     3209 2023-06-16 18:18:42.000000 xlsconv-2.0.0a1/CODE_OF_CONDUCT.md
+-rw-r--r--   0 sheppard  (1000) sheppard  (1000)     3276 2023-06-16 18:18:42.000000 xlsconv-2.0.0a1/CONTRIBUTING.md
+-rw-r--r--   0 sheppard  (1000) sheppard  (1000)     1106 2023-06-16 18:18:42.000000 xlsconv-2.0.0a1/LICENSE
+-rw-r--r--   0 sheppard  (1000) sheppard  (1000)     6372 2023-06-16 18:20:17.374058 xlsconv-2.0.0a1/PKG-INFO
+-rw-r--r--   0 sheppard  (1000) sheppard  (1000)     5041 2023-06-16 18:18:42.000000 xlsconv-2.0.0a1/README.md
+-rw-r--r--   0 sheppard  (1000) sheppard  (1000)     1443 2023-06-16 18:18:42.000000 xlsconv-2.0.0a1/pyproject.toml
+-rw-r--r--   0 sheppard  (1000) sheppard  (1000)       38 2023-06-16 18:20:17.378055 xlsconv-2.0.0a1/setup.cfg
+drwxr-xr-x   0 sheppard  (1000) sheppard  (1000)        0 2023-06-16 18:20:17.159066 xlsconv-2.0.0a1/tests/
+-rw-r--r--   0 sheppard  (1000) sheppard  (1000)        0 2023-06-16 18:18:42.000000 xlsconv-2.0.0a1/tests/__init__.py
+drwxr-xr-x   0 sheppard  (1000) sheppard  (1000)        0 2023-06-16 18:20:17.188073 xlsconv-2.0.0a1/tests/files/
+drwxr-xr-x   0 sheppard  (1000) sheppard  (1000)        0 2023-06-16 18:20:17.234098 xlsconv-2.0.0a1/tests/files/input_types/
+-rw-r--r--   0 sheppard  (1000) sheppard  (1000)      123 2023-06-16 18:18:42.000000 xlsconv-2.0.0a1/tests/files/input_types/admin.py
+-rw-r--r--   0 sheppard  (1000) sheppard  (1000)     2324 2023-06-16 18:18:42.000000 xlsconv-2.0.0a1/tests/files/input_types/models.py
+-rw-r--r--   0 sheppard  (1000) sheppard  (1000)      508 2023-06-16 18:18:42.000000 xlsconv-2.0.0a1/tests/files/input_types/rest.py
+-rw-r--r--   0 sheppard  (1000) sheppard  (1000)      205 2023-06-16 18:18:42.000000 xlsconv-2.0.0a1/tests/files/input_types/serializers.py
+-rw-r--r--   0 sheppard  (1000) sheppard  (1000)       85 2023-06-16 18:18:42.000000 xlsconv-2.0.0a1/tests/files/input_types/wizard.py
+-rw-r--r--   0 sheppard  (1000) sheppard  (1000)     8704 2023-06-16 18:18:42.000000 xlsconv-2.0.0a1/tests/files/input_types.xls
+drwxr-xr-x   0 sheppard  (1000) sheppard  (1000)        0 2023-06-16 18:20:17.280106 xlsconv-2.0.0a1/tests/files/nestedfk/
+-rw-r--r--   0 sheppard  (1000) sheppard  (1000)       94 2023-06-16 18:18:42.000000 xlsconv-2.0.0a1/tests/files/nestedfk/admin.py
+-rw-r--r--   0 sheppard  (1000) sheppard  (1000)      890 2023-06-16 18:18:42.000000 xlsconv-2.0.0a1/tests/files/nestedfk/models.py
+-rw-r--r--   0 sheppard  (1000) sheppard  (1000)      243 2023-06-16 18:18:42.000000 xlsconv-2.0.0a1/tests/files/nestedfk/rest.py
+-rw-r--r--   0 sheppard  (1000) sheppard  (1000)      617 2023-06-16 18:18:42.000000 xlsconv-2.0.0a1/tests/files/nestedfk/serializers.py
+-rw-r--r--   0 sheppard  (1000) sheppard  (1000)      147 2023-06-16 18:18:42.000000 xlsconv-2.0.0a1/tests/files/nestedfk/wizard.py
+-rw-r--r--   0 sheppard  (1000) sheppard  (1000)      345 2023-06-16 18:18:42.000000 xlsconv-2.0.0a1/tests/files/nestedfk.csv
+drwxr-xr-x   0 sheppard  (1000) sheppard  (1000)        0 2023-06-16 18:20:17.315078 xlsconv-2.0.0a1/tests/files/repeat/
+-rw-r--r--   0 sheppard  (1000) sheppard  (1000)       90 2023-06-16 18:18:42.000000 xlsconv-2.0.0a1/tests/files/repeat/admin.py
+-rw-r--r--   0 sheppard  (1000) sheppard  (1000)     1114 2023-06-16 18:18:42.000000 xlsconv-2.0.0a1/tests/files/repeat/models.py
+-rw-r--r--   0 sheppard  (1000) sheppard  (1000)      235 2023-06-16 18:18:42.000000 xlsconv-2.0.0a1/tests/files/repeat/rest.py
+-rw-r--r--   0 sheppard  (1000) sheppard  (1000)     1131 2023-06-16 18:18:42.000000 xlsconv-2.0.0a1/tests/files/repeat/serializers.py
+-rw-r--r--   0 sheppard  (1000) sheppard  (1000)      139 2023-06-16 18:18:42.000000 xlsconv-2.0.0a1/tests/files/repeat/wizard.py
+-rw-r--r--   0 sheppard  (1000) sheppard  (1000)      456 2023-06-16 18:18:42.000000 xlsconv-2.0.0a1/tests/files/repeat.csv
+drwxr-xr-x   0 sheppard  (1000) sheppard  (1000)        0 2023-06-16 18:20:17.338067 xlsconv-2.0.0a1/tests/files/select/
+-rw-r--r--   0 sheppard  (1000) sheppard  (1000)       90 2023-06-16 18:18:42.000000 xlsconv-2.0.0a1/tests/files/select/admin.py
+-rw-r--r--   0 sheppard  (1000) sheppard  (1000)     1414 2023-06-16 18:18:42.000000 xlsconv-2.0.0a1/tests/files/select/models.py
+-rw-r--r--   0 sheppard  (1000) sheppard  (1000)      160 2023-06-16 18:18:42.000000 xlsconv-2.0.0a1/tests/files/select/rest.py
+-rw-r--r--   0 sheppard  (1000) sheppard  (1000)      193 2023-06-16 18:18:42.000000 xlsconv-2.0.0a1/tests/files/select/serializers.py
+-rw-r--r--   0 sheppard  (1000) sheppard  (1000)       77 2023-06-16 18:18:42.000000 xlsconv-2.0.0a1/tests/files/select/wizard.py
+-rw-r--r--   0 sheppard  (1000) sheppard  (1000)      625 2023-06-16 18:18:42.000000 xlsconv-2.0.0a1/tests/files/select.csv
+-rw-r--r--   0 sheppard  (1000) sheppard  (1000)     1133 2023-06-16 18:18:42.000000 xlsconv-2.0.0a1/tests/test_survey.py
+drwxr-xr-x   0 sheppard  (1000) sheppard  (1000)        0 2023-06-16 18:20:17.351068 xlsconv-2.0.0a1/xlsconv/
+-rw-r--r--   0 sheppard  (1000) sheppard  (1000)      150 2023-06-16 18:18:42.000000 xlsconv-2.0.0a1/xlsconv/__init__.py
+-rw-r--r--   0 sheppard  (1000) sheppard  (1000)     3172 2023-06-16 18:18:42.000000 xlsconv-2.0.0a1/xlsconv/ast.py
+-rw-r--r--   0 sheppard  (1000) sheppard  (1000)    16940 2023-06-16 18:18:42.000000 xlsconv-2.0.0a1/xlsconv/django.py
+-rw-r--r--   0 sheppard  (1000) sheppard  (1000)     2200 2023-06-16 18:18:42.000000 xlsconv-2.0.0a1/xlsconv/parser.py
+drwxr-xr-x   0 sheppard  (1000) sheppard  (1000)        0 2023-06-16 18:20:17.371063 xlsconv-2.0.0a1/xlsconv.egg-info/
+-rw-r--r--   0 sheppard  (1000) sheppard  (1000)     6372 2023-06-16 18:20:16.000000 xlsconv-2.0.0a1/xlsconv.egg-info/PKG-INFO
+-rw-r--r--   0 sheppard  (1000) sheppard  (1000)     1125 2023-06-16 18:20:17.000000 xlsconv-2.0.0a1/xlsconv.egg-info/SOURCES.txt
+-rw-r--r--   0 sheppard  (1000) sheppard  (1000)        1 2023-06-16 18:20:16.000000 xlsconv-2.0.0a1/xlsconv.egg-info/dependency_links.txt
+-rw-r--r--   0 sheppard  (1000) sheppard  (1000)       51 2023-06-16 18:20:16.000000 xlsconv-2.0.0a1/xlsconv.egg-info/entry_points.txt
+-rw-r--r--   0 sheppard  (1000) sheppard  (1000)       25 2023-06-16 18:20:16.000000 xlsconv-2.0.0a1/xlsconv.egg-info/requires.txt
+-rw-r--r--   0 sheppard  (1000) sheppard  (1000)        8 2023-06-16 18:20:16.000000 xlsconv-2.0.0a1/xlsconv.egg-info/top_level.txt
```

### filetype from file(1)

```diff
@@ -1 +1 @@
-POSIX tar archive (GNU)
+POSIX tar archive
```

### Comparing `xlsconv-1.3.0/tests/test_survey.py` & `xlsconv-2.0.0a1/tests/test_survey.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,11 +1,10 @@
 import unittest
-from xlsconv import xls2django, xls2html
+from xlsconv import xls2django
 from xlsconv.django import TEMPLATE_NAMES as django_templates
-from xlsconv.html import TEMPLATE_NAMES as html_templates
 import os
 
 
 class SurveyTestCase(unittest.TestCase):
     files_dir = os.path.join(os.path.dirname(__file__), "files")
     maxDiff = None
 
@@ -22,31 +21,18 @@
             actual_python = xls2django(
                 self.get_path("%s.%s" % (name, ext)),
                 template,
             )
             expected_python = self.get_contents("%s/%s.py" % (name, template))
             self.assertEqual(expected_python, actual_python)
 
-    def check_html(self, name, ext):
-        for template in html_templates:
-            actual_html = xls2html(
-                self.get_path("%s.%s" % (name, ext)),
-                template,
-            )
-            expected_html = self.get_contents("%s/%s.html" % (name, template))
-            self.assertEqual(expected_html, actual_html)
-
     def test_input_types(self):
         self.check_django("input_types", "xls")
-        self.check_html("input_types", "xls")
 
     def test_select(self):
         self.check_django("select", "csv")
-        self.check_html("select", "csv")
 
     def test_repeat(self):
         self.check_django("repeat", "csv")
-        self.check_html("repeat", "csv")
 
     def test_nestedfk(self):
         self.check_django("nestedfk", "csv")
-        self.check_html("nestedfk", "csv")
```

### Comparing `xlsconv-1.3.0/tests/files/select.csv` & `xlsconv-2.0.0a1/tests/files/select.csv`

 * *Files identical despite different names*

### Comparing `xlsconv-1.3.0/tests/files/nestedfk/models.py` & `xlsconv-2.0.0a1/tests/files/nestedfk/models.py`

 * *Files identical despite different names*

### Comparing `xlsconv-1.3.0/tests/files/nestedfk/serializers.py` & `xlsconv-2.0.0a1/tests/files/nestedfk/serializers.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,24 +1,25 @@
-from wq.db.patterns import serializers as patterns
-from .models import Nestedfk, Item, Nested
+from wq.db import rest
+from .models import Nestedfk, Item
 
 
-class ItemSerializer(patterns.AttachmentSerializer):
-    class Meta(patterns.AttachmentSerializer.Meta):
+class ItemSerializer(rest.ModelSerializer):
+    class Meta:
         model = Item
         exclude = ("nestedfk",)
-        object_field = "nestedfk"
-        wq_config = {
-            "initial": 3,
-        }
         wq_field_config = {}
 
 
-class NestedfkSerializer(patterns.AttachedModelSerializer):
-    items = ItemSerializer(many=True)
+class NestedfkSerializer(rest.ModelSerializer):
+    items = ItemSerializer(
+        many=True,
+        wq_config={
+            "initial": 3,
+        },
+    )
 
     class Meta:
         model = Nestedfk
         fields = "__all__"
         wq_field_config = {}
         wq_fieldsets = {
             "": {"label": "General", "fields": ["name"]},
```

### Comparing `xlsconv-1.3.0/tests/files/input_types/models.py` & `xlsconv-2.0.0a1/tests/files/input_types/models.py`

 * *Files identical despite different names*

### Comparing `xlsconv-1.3.0/tests/files/select/models.py` & `xlsconv-2.0.0a1/tests/files/select/models.py`

 * *Files identical despite different names*

### Comparing `xlsconv-1.3.0/tests/files/input_types.xls` & `xlsconv-2.0.0a1/tests/files/input_types.xls`

 * *Files identical despite different names*

### Comparing `xlsconv-1.3.0/tests/files/repeat/models.py` & `xlsconv-2.0.0a1/tests/files/repeat/models.py`

 * *Files identical despite different names*

### Comparing `xlsconv-1.3.0/CODE_OF_CONDUCT.md` & `xlsconv-2.0.0a1/CODE_OF_CONDUCT.md`

 * *Files identical despite different names*

### Comparing `xlsconv-1.3.0/LICENSE` & `xlsconv-2.0.0a1/LICENSE`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 The MIT License (MIT)
 
-Copyright (c) 2016-2020 S. Andrew Sheppard, https://wq.io/
+Copyright (c) 2016-2023 S. Andrew Sheppard, https://wq.io/
 
 Permission is hereby granted, free of charge, to any person obtaining a copy
 of this software and associated documentation files (the "Software"), to deal
 in the Software without restriction, including without limitation the rights
 to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
 copies of the Software, and to permit persons to whom the Software is
 furnished to do so, subject to the following conditions:
```

### Comparing `xlsconv-1.3.0/README.md` & `xlsconv-2.0.0a1/PKG-INFO`

 * *Files 15% similar despite different names*

```diff
@@ -1,7 +1,36 @@
+Metadata-Version: 2.1
+Name: xlsconv
+Version: 2.0.0a1
+Summary: Tool to convert ODK-style XLSForms into Django models or use with wq (https://wq.io/)
+Author-email: "S. Andrew Sheppard" <andrew@wq.io>
+License: MIT
+Project-URL: Homepage, https://github.com/wq/xlsform-converter
+Project-URL: Documentation, https://wq.io/
+Project-URL: Source, https://github.com/wq/xlsform-converter
+Project-URL: Release Notes, https://github.com/wq/xlsform-converter/releases
+Project-URL: Issues, https://github.com/wq/xlsform-converter/issues
+Project-URL: CI, https://github.com/wq/xlsform-converter/actions/workflows/test.yml
+Classifier: Development Status :: 5 - Production/Stable
+Classifier: Environment :: Web Environment
+Classifier: License :: OSI Approved :: MIT License
+Classifier: Natural Language :: English
+Classifier: Programming Language :: Python :: 3
+Classifier: Programming Language :: Python :: 3.7
+Classifier: Programming Language :: Python :: 3.8
+Classifier: Programming Language :: Python :: 3.9
+Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
+Classifier: Topic :: Software Development :: Code Generators
+Classifier: Framework :: Django
+Classifier: Topic :: Text Processing :: Markup :: HTML
+Requires-Python: >=3.7
+Description-Content-Type: text/markdown
+License-File: LICENSE
+
 # xlsform-converter (xlsconv)
 
 xlsform-converter converts surveys defined via the [XLSForm standard] into [Django models] and configuration.  This makes it possible to re-use the powerful form building tools provided by the [Open Data Kit ecosystem][ecosystem], while leveraging Django's robust support for relational databases like [PostgreSQL].
 
 xlsform-converter is designed to facilitate the rapid development of offline-capable data collection apps via the [wq framework].  The ultimate goal is to provide full compatibility with the form authoring tools provided by [ODK][ecosystem] and [KoboToolbox] (etc.).  Note that this is not the same as full XForm compatibility: the client and server components of wq ([wq.app] and [wq.db]) use a JSON-based [REST API] to exchange data and are not directly compatible with their ODK Analogues (ODK Collect and ODK Aggregate, respectively).
 
 For the database itself, the key distinction from other XLSForm tools (including those powered by Django, like KoboToolbox) is that xlsform-converter converts the xlsform fields directly into a Django model definition, rather than representing the entire XForm standard within Django.  This means that each row in an XLSForm "survey" tab is mapped to (usually) a single column in a simple relational database table.  Repeat questions are handled by creating a second model with a `ForeignKey` to the parent survey model.
@@ -26,26 +55,18 @@
 
 ### Included Templates
 
 xlsform-converter uses ASTs and templates to generate the following Django/wq project files from a given XLSForm (for example, [this file](https://github.com/wq/xlsform-converter/raw/main/tests/files/input_types.xls)).
 
 #### Django Apps
    - [`models.py`](https://github.com/wq/xlsform-converter/blob/main/tests/files/input_types/models.py)
-   - [`admin.py`](https://github.com/wq/xlsform-converter/blob/main/tests/files/input_types/admin.py) (for use with [`django.contrib.admin`](https://docs.djangoproject.com/en/4.0/ref/contrib/admin/))
+   - [`admin.py`](https://github.com/wq/xlsform-converter/blob/main/tests/files/input_types/admin.py) (for use with [`django.contrib.admin`](https://docs.djangoproject.com/en/4.2/ref/contrib/admin/))
    - [`wizard.py`](https://github.com/wq/xlsform-converter/blob/main/tests/files/input_types/wizard.py) (for use with [Django Data Wizard](https://github.com/wq/django-data-wizard))
    - [`rest.py`](https://github.com/wq/xlsform-converter/blob/main/tests/files/input_types/rest.py) (for use with [`wq.db.rest`](https://wq.io/wq.db/rest))
-   - [`serializers.py`](https://github.com/wq/xlsform-converter/blob/main/files/input_types/serializers.py) (for use with `wq.db.rest`)
-
-#### Mustache Templates (deprecated)
-   - [`edit.html`](https://github.com/wq/xlsform-converter/blob/main/xlsconv/templates/edit.html)
-   - [`detail.html`](https://github.com/wq/xlsform-converter/blob/main/xlsconv/templates/detail.html)
-   - [`list.html`](https://github.com/wq/xlsform-converter/blob/main/xlsconv/templates/list.html)
-   - [`popup.html`](https://github.com/wq/xlsform-converter/blob/main/xlsconv/templates/popup.html) (for use with [@wq/map](https://wq.io/@wq/map))
-
-> Note that these Mustache templates are only designed for use with wq's jQuery Mobile renderer, used by default in 1.2 and earlier.  As of [wq 1.3](https://wq.io/releases/wq-1.3.0), the corresponding screens are generated at runtime via [@wq/react](https://wq.io/@wq/react)'s built in React [views](https://wq.io/views/).  These Mustache templates will be dropped in 2.0, together with all backwards combility with 1.2.
+   - [`serializers.py`](https://github.com/wq/xlsform-converter/blob/main/tests/files/input_types/serializers.py) (for use with `wq.db.rest`)
 
 ### Usage
 
 If you are using wq, you may be interested in [wq.create], which uses xlsconv internally for the `wq addform` command.  Otherwise, you can use xlsconv directly with the following command-line API:
 
 ```bash
 # Recommended: create virtual environment
@@ -59,16 +80,15 @@
 xls2django my-odk-survey.xls > myapp/models.py
 
 # Use the rest.py template (or admin.py, or serializers.py)
 xls2django my-odk-survey.xls rest > myapp/models.py
 ```
 
 [XLSForm standard]: https://xlsform.org/
-[Django models]: https://docs.djangoproject.com/en/1.9/topics/db/models/
-[Mustache templates]: https://wq.io/docs/templates
+[Django models]: https://docs.djangoproject.com/en/4.2/topics/db/models/
 [ecosystem]: https://getodk.org/about/ecosystem.html
 [KoboToolbox]: https://www.kobotoolbox.org/
 [PostgreSQL]: http://www.postgresql.org/
 [wq framework]: https://wq.io/
 [wq.app]: https://wq.io/wq.app/
 [wq.db]: https://wq.io/wq.db/
 [REST API]: https://wq.io/wq.db/url-structure
```

### Comparing `xlsconv-1.3.0/.github/workflows/test.yml` & `xlsconv-2.0.0a1/.github/workflows/test.yml`

 * *Files 12% similar despite different names*

```diff
@@ -1,30 +1,38 @@
 name: Tests
 
 on: [push, pull_request]
 
 jobs:
   build:
     name: py=${{ matrix.python-version }}
-    runs-on: ubuntu-20.04
+    runs-on: ubuntu-22.04
     strategy:
       matrix:
-        python-version: [3.6, 3.7, 3.8, 3.9]
+        python-version:
+          - 3.7
+          - 3.8
+          - 3.9
+          - "3.10"
+          - "3.11"
     steps:
     - uses: actions/checkout@v2
     - name: Set up Python ${{ matrix.python-version }}
       uses: actions/setup-python@v2
       with:
         python-version: ${{ matrix.python-version }}
     - name: Install dependencies
       run: |
         python -m pip install --upgrade pip
+        python -m pip install build
         python -m pip install flake8 wheel
-        python -m pip install pyxform astunparse black pystache
+        python -m pip install pyxform astunparse black
     - name: Lint with flake8
       run: |
         # stop the build if there are Python syntax errors or undefined names
         flake8 xlsconv tests --count --select=E9,F63,F7,F82 --show-source --statistics
         # exit-zero treats all errors as warnings. The GitHub editor is 127 chars wide
         flake8 xlsconv tests --count --exit-zero --max-complexity=10 --max-line-length=127 --statistics
     - name: Test with unittest
       run: python -m unittest discover -s tests -t . -v
+    - name: Test build
+      run: python -m build
```

### Comparing `xlsconv-1.3.0/xlsconv/ast.py` & `xlsconv-2.0.0a1/xlsconv/ast.py`

 * *Files identical despite different names*

### Comparing `xlsconv-1.3.0/xlsconv/django.py` & `xlsconv-2.0.0a1/xlsconv/django.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,9 +1,8 @@
 from .parser import parse_xls, generate_names
-from .renderer import render
 from .ast import (
     ast_module,
     ast_import,
     ast_assign,
     ast_expr,
     ast_call,
     ast_name,
@@ -83,15 +82,15 @@
             node = node.parent
         return node
 
     @property
     def models(self):
         models = [self.class_name]
         for field in self.children:
-            if field.children:
+            if field.children and field.config.get("wq:many"):
                 models += field.models
         return models
 
     def as_admin(self):
         module = "django.contrib"
         register_args = [ast_name(self.class_name)]
         if self.config.get("has_geo"):
@@ -299,15 +298,15 @@
             ast_import("wq.db", "rest"),
             ast_import(".models", self.class_name),
             ast_import(".serializers", serializer) if serializer else None,
             ast_newline(),
             ast_newline(),
             ast_expr(
                 ast_call(
-                    "rest.router.register_model",
+                    "rest.router.register",
                     ast_name(self.class_name),
                     **kwargs,
                 )
             ),
         )
 
     def as_wizard(self):
@@ -326,15 +325,15 @@
             ast_newline(),
             ast_expr(ast_call("data_wizard.register", *args)),
         )
 
     def as_serializers(self):
         serializers = self.as_serializer()
         return ast_module(
-            ast_import("wq.db.patterns", "serializers", "patterns"),
+            ast_import("wq.db", "rest"),
             ast_import(".models", self.models),
             *serializers,
         )
 
     def as_serializer(self):
         nested_serializers = []
         nested_fields = []
@@ -347,14 +346,15 @@
                     nested_serializers += field.as_serializer()
                     nested_fields.append(
                         ast_assign(
                             field.name,
                             ast_call(
                                 f"{field.class_name}Serializer",
                                 many=True,
+                                wq_config=ast_dict(initial=3),
                             ),
                         )
                     )
                 else:
                     fieldset = {
                         "label": field.config.get("label"),
                     }
@@ -385,29 +385,21 @@
         else:
             wq_fieldsets = None
 
         return [
             *nested_serializers,
             ast_class(
                 f"{self.class_name}Serializer",
-                [
-                    "patterns.AttachmentSerializer"
-                    if self.parent
-                    else "patterns.AttachedModelSerializer"
-                ],
+                ["rest.ModelSerializer"],
                 *nested_fields,
                 ast_class(
                     "Meta",
-                    ["patterns.AttachmentSerializer.Meta"],
+                    [],
                     ast_assign("model", ast_name(self.class_name)),
                     ast_assign("exclude", (self.parent.name,)),
-                    ast_assign("object_field", self.parent.name),
-                    ast_assign("wq_config", ast_dict(initial=3))
-                    if self.config.get("wq:many")
-                    else None,
                     ast_assign("wq_field_config", wq_field_config),
                     ast_assign("wq_fieldsets", wq_fieldsets),
                 )
                 if self.parent
                 else ast_class(
                     "Meta",
                     [],
@@ -513,20 +505,19 @@
 
 
 def xls2django(file_or_name, template_name=DEFAULT_TEMPLATE):
     xform_json = parse_xls(file_or_name)
     context = django_context(xform_json)
     transform = TEMPLATES.get(template_name)
 
-    if transform:
-        tree = transform(Node(**context["form"]))
-        code = unparse(tree)
-    else:
-        code = render(context, template_name)
+    if not transform:
+        raise Exception(f"Unrecognized type {template_name}")
 
+    tree = transform(Node(**context["form"]))
+    code = unparse(tree)
     return black.format_str(code, mode=black.FileMode())
 
 
 def main():
     import sys
 
     print(xls2django(*sys.argv[1:]))
```

### Comparing `xlsconv-1.3.0/xlsconv/parser.py` & `xlsconv-2.0.0a1/xlsconv/parser.py`

 * *Files identical despite different names*

### Comparing `xlsconv-1.3.0/xlsconv.egg-info/SOURCES.txt` & `xlsconv-2.0.0a1/xlsconv.egg-info/SOURCES.txt`

 * *Files 23% similar despite different names*

```diff
@@ -1,74 +1,43 @@
 .gitignore
 CODE_OF_CONDUCT.md
 CONTRIBUTING.md
 LICENSE
 README.md
-setup.py
+pyproject.toml
 .github/workflows/test.yml
 tests/__init__.py
 tests/test_survey.py
 tests/files/input_types.xls
 tests/files/nestedfk.csv
 tests/files/repeat.csv
 tests/files/select.csv
 tests/files/input_types/admin.py
-tests/files/input_types/detail.html
-tests/files/input_types/edit.html
-tests/files/input_types/list.html
 tests/files/input_types/models.py
-tests/files/input_types/popup.html
 tests/files/input_types/rest.py
 tests/files/input_types/serializers.py
 tests/files/input_types/wizard.py
 tests/files/nestedfk/admin.py
-tests/files/nestedfk/detail.html
-tests/files/nestedfk/edit.html
-tests/files/nestedfk/list.html
 tests/files/nestedfk/models.py
-tests/files/nestedfk/popup.html
 tests/files/nestedfk/rest.py
 tests/files/nestedfk/serializers.py
 tests/files/nestedfk/wizard.py
 tests/files/repeat/admin.py
-tests/files/repeat/detail.html
-tests/files/repeat/edit.html
-tests/files/repeat/list.html
 tests/files/repeat/models.py
-tests/files/repeat/popup.html
 tests/files/repeat/rest.py
 tests/files/repeat/serializers.py
 tests/files/repeat/wizard.py
 tests/files/select/admin.py
-tests/files/select/detail.html
-tests/files/select/edit.html
-tests/files/select/list.html
 tests/files/select/models.py
-tests/files/select/popup.html
 tests/files/select/rest.py
 tests/files/select/serializers.py
 tests/files/select/wizard.py
 xlsconv/__init__.py
 xlsconv/ast.py
 xlsconv/django.py
-xlsconv/html.py
 xlsconv/parser.py
-xlsconv/renderer.py
 xlsconv.egg-info/PKG-INFO
 xlsconv.egg-info/SOURCES.txt
 xlsconv.egg-info/dependency_links.txt
 xlsconv.egg-info/entry_points.txt
 xlsconv.egg-info/requires.txt
-xlsconv.egg-info/top_level.txt
-xlsconv/templates/detail.html
-xlsconv/templates/edit.html
-xlsconv/templates/list.html
-xlsconv/templates/popup.html
-xlsconv/templates/fields/foreignkey.html
-xlsconv/templates/fields/geo.html
-xlsconv/templates/fields/html_field.html
-xlsconv/templates/fields/input.html
-xlsconv/templates/fields/note.html
-xlsconv/templates/fields/photo.html
-xlsconv/templates/fields/radio.html
-xlsconv/templates/fields/select.html
-xlsconv/templates/fields/textarea.html
+xlsconv.egg-info/top_level.txt
```

### Comparing `xlsconv-1.3.0/xlsconv.egg-info/PKG-INFO` & `xlsconv-2.0.0a1/xlsconv.egg-info/PKG-INFO`

 * *Files 20% similar despite different names*

```diff
@@ -1,98 +1,95 @@
 Metadata-Version: 2.1
 Name: xlsconv
-Version: 1.3.0
-Summary: Tool to convert ODK-style XLSForms into Django models and HTML templates for use with wq (https://wq.io/)
-Home-page: https://github.com/wq/xlsform-converter
-Author: S. Andrew Sheppard
-Author-email: andrew@wq.io
+Version: 2.0.0a1
+Summary: Tool to convert ODK-style XLSForms into Django models or use with wq (https://wq.io/)
+Author-email: "S. Andrew Sheppard" <andrew@wq.io>
 License: MIT
-Description: # xlsform-converter (xlsconv)
-        
-        xlsform-converter converts surveys defined via the [XLSForm standard] into [Django models] and configuration.  This makes it possible to re-use the powerful form building tools provided by the [Open Data Kit ecosystem][ecosystem], while leveraging Django's robust support for relational databases like [PostgreSQL].
-        
-        xlsform-converter is designed to facilitate the rapid development of offline-capable data collection apps via the [wq framework].  The ultimate goal is to provide full compatibility with the form authoring tools provided by [ODK][ecosystem] and [KoboToolbox] (etc.).  Note that this is not the same as full XForm compatibility: the client and server components of wq ([wq.app] and [wq.db]) use a JSON-based [REST API] to exchange data and are not directly compatible with their ODK Analogues (ODK Collect and ODK Aggregate, respectively).
-        
-        For the database itself, the key distinction from other XLSForm tools (including those powered by Django, like KoboToolbox) is that xlsform-converter converts the xlsform fields directly into a Django model definition, rather than representing the entire XForm standard within Django.  This means that each row in an XLSForm "survey" tab is mapped to (usually) a single column in a simple relational database table.  Repeat questions are handled by creating a second model with a `ForeignKey` to the parent survey model.
-        
-        > For a more thorough comparison of XLSForm tools, see <https://wq.io/overview/survey123-vs-kobotoolbox-vs-wq>.
-        
-        xlsform-converter also supports a couple of additional "constraints" that are not part of the XLSForm standard:
-        
-         * `wq:ForeignKey('app.ModelName')`: Create a foreign key to an existing Django model (presumably not defined in the spreadsheet).  This is effectively a more relational version of `select_one_external`.
-         * `wq:initial(3)`: Very similar to `repeat_count`, but only set for new records.
-         * `wq:length(5)`: Text field maximum length (similar to a `string-length` constraint)
-        
-        [![Latest PyPI Release](https://img.shields.io/pypi/v/xlsconv.svg)](https://pypi.org/project/xlsconv)
-        [![Release Notes](https://img.shields.io/github/release/wq/xlsform-converter.svg)](https://github.com/wq/xlsform-converter/releases)
-        [![License](https://img.shields.io/pypi/l/xlsconv.svg)](https://github.com/wq/xlsform-converter/blob/main/LICENSE)
-        [![GitHub Stars](https://img.shields.io/github/stars/wq/xlsform-converter.svg)](https://github.com/wq/xlsform-converter/stargazers)
-        [![GitHub Forks](https://img.shields.io/github/forks/wq/xlsform-converter.svg)](https://github.com/wq/xlsform-converter/network)
-        [![GitHub Issues](https://img.shields.io/github/issues/wq/xlsform-converter.svg)](https://github.com/wq/xlsform-converter/issues)
-        
-        [![Tests](https://github.com/wq/xlsform-converter/actions/workflows/test.yml/badge.svg)](https://github.com/wq/xlsform-converter/actions/workflows/test.yml)
-        [![Python Support](https://img.shields.io/pypi/pyversions/xlsconv.svg)](https://pypi.python.org/pypi/xlsconv)
-        
-        ### Included Templates
-        
-        xlsform-converter uses ASTs and templates to generate the following Django/wq project files from a given XLSForm (for example, [this file](https://github.com/wq/xlsform-converter/raw/main/tests/files/input_types.xls)).
-        
-        #### Django Apps
-           - [`models.py`](https://github.com/wq/xlsform-converter/blob/main/tests/files/input_types/models.py)
-           - [`admin.py`](https://github.com/wq/xlsform-converter/blob/main/tests/files/input_types/admin.py) (for use with [`django.contrib.admin`](https://docs.djangoproject.com/en/4.0/ref/contrib/admin/))
-           - [`wizard.py`](https://github.com/wq/xlsform-converter/blob/main/tests/files/input_types/wizard.py) (for use with [Django Data Wizard](https://github.com/wq/django-data-wizard))
-           - [`rest.py`](https://github.com/wq/xlsform-converter/blob/main/tests/files/input_types/rest.py) (for use with [`wq.db.rest`](https://wq.io/wq.db/rest))
-           - [`serializers.py`](https://github.com/wq/xlsform-converter/blob/main/files/input_types/serializers.py) (for use with `wq.db.rest`)
-        
-        #### Mustache Templates (deprecated)
-           - [`edit.html`](https://github.com/wq/xlsform-converter/blob/main/xlsconv/templates/edit.html)
-           - [`detail.html`](https://github.com/wq/xlsform-converter/blob/main/xlsconv/templates/detail.html)
-           - [`list.html`](https://github.com/wq/xlsform-converter/blob/main/xlsconv/templates/list.html)
-           - [`popup.html`](https://github.com/wq/xlsform-converter/blob/main/xlsconv/templates/popup.html) (for use with [@wq/map](https://wq.io/@wq/map))
-        
-        > Note that these Mustache templates are only designed for use with wq's jQuery Mobile renderer, used by default in 1.2 and earlier.  As of [wq 1.3](https://wq.io/releases/wq-1.3.0), the corresponding screens are generated at runtime via [@wq/react](https://wq.io/@wq/react)'s built in React [views](https://wq.io/views/).  These Mustache templates will be dropped in 2.0, together with all backwards combility with 1.2.
-        
-        ### Usage
-        
-        If you are using wq, you may be interested in [wq.create], which uses xlsconv internally for the `wq addform` command.  Otherwise, you can use xlsconv directly with the following command-line API:
-        
-        ```bash
-        # Recommended: create virtual environment
-        # python3 -m venv venv
-        # . venv/bin/activate
-        
-        # Install xlsconv
-        pip install xlsconv
-        
-        # Use the default models.py template
-        xls2django my-odk-survey.xls > myapp/models.py
-        
-        # Use the rest.py template (or admin.py, or serializers.py)
-        xls2django my-odk-survey.xls rest > myapp/models.py
-        ```
-        
-        [XLSForm standard]: https://xlsform.org/
-        [Django models]: https://docs.djangoproject.com/en/1.9/topics/db/models/
-        [Mustache templates]: https://wq.io/docs/templates
-        [ecosystem]: https://getodk.org/about/ecosystem.html
-        [KoboToolbox]: https://www.kobotoolbox.org/
-        [PostgreSQL]: http://www.postgresql.org/
-        [wq framework]: https://wq.io/
-        [wq.app]: https://wq.io/wq.app/
-        [wq.db]: https://wq.io/wq.db/
-        [REST API]: https://wq.io/wq.db/url-structure
-        [wq.create]: https://wq.io/wq.create/
-        
-Platform: UNKNOWN
+Project-URL: Homepage, https://github.com/wq/xlsform-converter
+Project-URL: Documentation, https://wq.io/
+Project-URL: Source, https://github.com/wq/xlsform-converter
+Project-URL: Release Notes, https://github.com/wq/xlsform-converter/releases
+Project-URL: Issues, https://github.com/wq/xlsform-converter/issues
+Project-URL: CI, https://github.com/wq/xlsform-converter/actions/workflows/test.yml
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Environment :: Web Environment
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Natural Language :: English
 Classifier: Programming Language :: Python :: 3
-Classifier: Programming Language :: Python :: 3.6
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
+Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
 Classifier: Topic :: Software Development :: Code Generators
 Classifier: Framework :: Django
 Classifier: Topic :: Text Processing :: Markup :: HTML
+Requires-Python: >=3.7
 Description-Content-Type: text/markdown
+License-File: LICENSE
+
+# xlsform-converter (xlsconv)
+
+xlsform-converter converts surveys defined via the [XLSForm standard] into [Django models] and configuration.  This makes it possible to re-use the powerful form building tools provided by the [Open Data Kit ecosystem][ecosystem], while leveraging Django's robust support for relational databases like [PostgreSQL].
+
+xlsform-converter is designed to facilitate the rapid development of offline-capable data collection apps via the [wq framework].  The ultimate goal is to provide full compatibility with the form authoring tools provided by [ODK][ecosystem] and [KoboToolbox] (etc.).  Note that this is not the same as full XForm compatibility: the client and server components of wq ([wq.app] and [wq.db]) use a JSON-based [REST API] to exchange data and are not directly compatible with their ODK Analogues (ODK Collect and ODK Aggregate, respectively).
+
+For the database itself, the key distinction from other XLSForm tools (including those powered by Django, like KoboToolbox) is that xlsform-converter converts the xlsform fields directly into a Django model definition, rather than representing the entire XForm standard within Django.  This means that each row in an XLSForm "survey" tab is mapped to (usually) a single column in a simple relational database table.  Repeat questions are handled by creating a second model with a `ForeignKey` to the parent survey model.
+
+> For a more thorough comparison of XLSForm tools, see <https://wq.io/overview/survey123-vs-kobotoolbox-vs-wq>.
+
+xlsform-converter also supports a couple of additional "constraints" that are not part of the XLSForm standard:
+
+ * `wq:ForeignKey('app.ModelName')`: Create a foreign key to an existing Django model (presumably not defined in the spreadsheet).  This is effectively a more relational version of `select_one_external`.
+ * `wq:initial(3)`: Very similar to `repeat_count`, but only set for new records.
+ * `wq:length(5)`: Text field maximum length (similar to a `string-length` constraint)
+
+[![Latest PyPI Release](https://img.shields.io/pypi/v/xlsconv.svg)](https://pypi.org/project/xlsconv)
+[![Release Notes](https://img.shields.io/github/release/wq/xlsform-converter.svg)](https://github.com/wq/xlsform-converter/releases)
+[![License](https://img.shields.io/pypi/l/xlsconv.svg)](https://github.com/wq/xlsform-converter/blob/main/LICENSE)
+[![GitHub Stars](https://img.shields.io/github/stars/wq/xlsform-converter.svg)](https://github.com/wq/xlsform-converter/stargazers)
+[![GitHub Forks](https://img.shields.io/github/forks/wq/xlsform-converter.svg)](https://github.com/wq/xlsform-converter/network)
+[![GitHub Issues](https://img.shields.io/github/issues/wq/xlsform-converter.svg)](https://github.com/wq/xlsform-converter/issues)
+
+[![Tests](https://github.com/wq/xlsform-converter/actions/workflows/test.yml/badge.svg)](https://github.com/wq/xlsform-converter/actions/workflows/test.yml)
+[![Python Support](https://img.shields.io/pypi/pyversions/xlsconv.svg)](https://pypi.python.org/pypi/xlsconv)
+
+### Included Templates
+
+xlsform-converter uses ASTs and templates to generate the following Django/wq project files from a given XLSForm (for example, [this file](https://github.com/wq/xlsform-converter/raw/main/tests/files/input_types.xls)).
+
+#### Django Apps
+   - [`models.py`](https://github.com/wq/xlsform-converter/blob/main/tests/files/input_types/models.py)
+   - [`admin.py`](https://github.com/wq/xlsform-converter/blob/main/tests/files/input_types/admin.py) (for use with [`django.contrib.admin`](https://docs.djangoproject.com/en/4.2/ref/contrib/admin/))
+   - [`wizard.py`](https://github.com/wq/xlsform-converter/blob/main/tests/files/input_types/wizard.py) (for use with [Django Data Wizard](https://github.com/wq/django-data-wizard))
+   - [`rest.py`](https://github.com/wq/xlsform-converter/blob/main/tests/files/input_types/rest.py) (for use with [`wq.db.rest`](https://wq.io/wq.db/rest))
+   - [`serializers.py`](https://github.com/wq/xlsform-converter/blob/main/tests/files/input_types/serializers.py) (for use with `wq.db.rest`)
+
+### Usage
+
+If you are using wq, you may be interested in [wq.create], which uses xlsconv internally for the `wq addform` command.  Otherwise, you can use xlsconv directly with the following command-line API:
+
+```bash
+# Recommended: create virtual environment
+# python3 -m venv venv
+# . venv/bin/activate
+
+# Install xlsconv
+pip install xlsconv
+
+# Use the default models.py template
+xls2django my-odk-survey.xls > myapp/models.py
+
+# Use the rest.py template (or admin.py, or serializers.py)
+xls2django my-odk-survey.xls rest > myapp/models.py
+```
+
+[XLSForm standard]: https://xlsform.org/
+[Django models]: https://docs.djangoproject.com/en/4.2/topics/db/models/
+[ecosystem]: https://getodk.org/about/ecosystem.html
+[KoboToolbox]: https://www.kobotoolbox.org/
+[PostgreSQL]: http://www.postgresql.org/
+[wq framework]: https://wq.io/
+[wq.app]: https://wq.io/wq.app/
+[wq.db]: https://wq.io/wq.db/
+[REST API]: https://wq.io/wq.db/url-structure
+[wq.create]: https://wq.io/wq.create/
```

### Comparing `xlsconv-1.3.0/CONTRIBUTING.md` & `xlsconv-2.0.0a1/CONTRIBUTING.md`

 * *Files 16% similar despite different names*

```diff
@@ -1,68 +1,70 @@
 # Contributing Guidelines
 
 Thanks for contributing to the wq framework!  Here are some guidelines to help you get started.
 
 ## Questions
 
-Feel free to use the issue tracker to ask questions!  We don't currently have a separate mailing list or active chat tool.  However, note that as wq grows we may eventually move questions to a separate tool.
+Questions and ideas can be submitted to the main [wq discussion board](https://github.com/wq/wq/discussions).
 
 ## Bug Reports
 
 wq is a highly modular framework and the code is split across several repositories.  If you are unsure where to report an issue, feel free to use the top-level [wq repository](https://github.com/wq/wq/issues).  Otherwise, enter your issue on the repository that most closely matches the component you are using.
 
  * [wq](https://github.com/wq/wq/issues): General API design & documentation
  * [wq.app](https://github.com/wq/wq.app/issues): JavaScript client & build tool
+ * [wq.build](https://github.com/wq/wq.build/issues): CLI & Project build tools
+ * [wq.create](https://github.com/wq/wq.create/issues): `wq create` command & project templates
  * [wq.db](https://github.com/wq/wq.db/issues): Web server & REST API (Django REST Framework)
- * [wq.start](https://github.com/wq/wq.start/issues): `wq start` command & questions about getting started
- * [xlsconv](https://github.com/wq/xlsform-converter/issues): XLSForm converter and default HTML templates
+ * [xlsconv](https://github.com/wq/xlsform-converter/issues): XLSForm converter
 
 Don't worry about getting the repository exactly right - many issues span multiple repositories and we can always reference the fix back to the original ticket.
 
 ## Pull Requests
 
 Pull requests are very welcome and will be reviewed and merged as time allows.  To speed up reviews, try to include the following whenever possible:
  * Reference the issue that the PR fixes (e.g. [#22](https://github.com/wq/wq/issues/22) or [wq/wq#22](https://github.com/wq/wq/issues/22) if in a different repository).
  * Failing test case fixed by the PR
- * If the PR provides new functionality to wq, a separate PR updating the [wq documentation](https://github.com/wq/wq/tree/master/docs).
+ * If the PR provides new functionality, a separate PR updating the [wq documentation](https://github.com/wq/wq/tree/main/docs).
  * Ensure the PR passes lint and unit tests.  This happens automatically, but you can also run these locally with the following commands:
  
 ```bash 
-./runtests.sh # run the test suite
-LINT=1 ./runtests.sh # run code style checking
+python -m unittest discover -s tests -t . # run the test suite
+flake8 # run code style checking
 ```
 
 If you would like help implementing any part of your PR, feel free to enable write access and we'll take a look as time allows.
  
 ## Development & Testing
 
 Small changes and documentation fixes can usually be done using Github's online file editors.  For larger changes, we recommend the following workflow.
 
-Because wq is split across several repositories, we recommend installing the entire suite from PyPI, starting a test project, and then cloning the specific module you want to update.  For example, to work on [wq.db](https://github.com/wq/wq.db), clone it to your account and then do something like this:
+Because wq is split across several repositories, we recommend installing the `wq` package, starting a test project, and then cloning the specific module you want to update.  For example, to work on [wq.db](https://github.com/wq/wq.db), clone it to your account and then do something like this:
 
 ### Initial Setup
 ```bash
 # Initialize workspace & test project
 WORKSPACE=~/devel/
 mkdir $WORKSPACE && cd $WORKSPACE
 python3 -m venv venv
 . venv/bin/activate
 pip install --upgrade pip
 pip install wq
-wq start -d test.wq.io testproject .
+wq create -d test.wq.io testproject .
 
 # Clone wq.db from fork
 git clone git@github.com:[my-username]/wq.db.git
 cd wq.db
 git checkout -b my-wqdb-branch
 ```
+
 ### Ongoing Development
 ```bash
 cd $WORKSPACE/wq.db
-vim rest/some_file.py # (make changes to wq.db)
-./runtests.sh # run the test suite
-LINT=1 ./runtests.sh # run code style checking
+vim wq/db/rest/some_file.py # (make changes to wq.db)
+python -m unittest discover -s tests -t . # run the test suite
+flake8 # run code style checking
 
 pip install --upgrade .  # overwrites PyPI wq.db with local version
 cd $WORKSPACE/
 ./deploy.sh 0.0.$RANDOM
 ```
```

