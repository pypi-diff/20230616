# Comparing `tmp/itertable-2.1.0.tar.gz` & `tmp/itertable-2.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/itertable-2.1.0.tar", last modified: Wed Jun 22 01:41:27 2022, max compression
+gzip compressed data, was "itertable-2.2.0.tar", last modified: Fri Jun 16 16:02:52 2023, max compression
```

## Comparing `itertable-2.1.0.tar` & `itertable-2.2.0.tar`

### file list

```diff
@@ -1,80 +1,73 @@
-drwxr-xr-x   0 sheppard  (1000) sheppard  (1000)        0 2022-06-22 01:41:27.000000 itertable-2.1.0/
--rw-r--r--   0 sheppard  (1000) sheppard  (1000)       66 2022-06-22 01:41:10.000000 itertable-2.1.0/.gitignore
-drwxr-xr-x   0 sheppard  (1000) sheppard  (1000)        0 2022-06-22 01:41:27.000000 itertable-2.1.0/tests/
--rw-r--r--   0 sheppard  (1000) sheppard  (1000)     3122 2022-06-22 01:41:10.000000 itertable-2.1.0/tests/test_netloader.py
--rw-r--r--   0 sheppard  (1000) sheppard  (1000)     3260 2022-06-22 01:41:10.000000 itertable-2.1.0/tests/test_write.py
--rw-r--r--   0 sheppard  (1000) sheppard  (1000)     5085 2022-06-22 01:41:10.000000 itertable-2.1.0/tests/test_load_file.py
--rw-r--r--   0 sheppard  (1000) sheppard  (1000)     1433 2022-06-22 01:41:10.000000 itertable-2.1.0/tests/test_custom.py
--rw-r--r--   0 sheppard  (1000) sheppard  (1000)      895 2022-06-22 01:41:10.000000 itertable-2.1.0/tests/test_dataframe.py
--rw-r--r--   0 sheppard  (1000) sheppard  (1000)      942 2022-06-22 01:41:10.000000 itertable-2.1.0/tests/base.py
--rw-r--r--   0 sheppard  (1000) sheppard  (1000)     1996 2022-06-22 01:41:10.000000 itertable-2.1.0/tests/test_gis.py
--rw-r--r--   0 sheppard  (1000) sheppard  (1000)     2301 2022-06-22 01:41:10.000000 itertable-2.1.0/tests/test_zip.py
--rw-r--r--   0 sheppard  (1000) sheppard  (1000)      574 2022-06-22 01:41:10.000000 itertable-2.1.0/tests/test_gis_dataframe.py
--rw-r--r--   0 sheppard  (1000) sheppard  (1000)        0 2022-06-22 01:41:10.000000 itertable-2.1.0/tests/__init__.py
--rw-r--r--   0 sheppard  (1000) sheppard  (1000)     1420 2022-06-22 01:41:10.000000 itertable-2.1.0/tests/test_extra_data.py
-drwxr-xr-x   0 sheppard  (1000) sheppard  (1000)        0 2022-06-22 01:41:27.000000 itertable-2.1.0/tests/files/
--rw-r--r--   0 sheppard  (1000) sheppard  (1000)      116 2022-06-22 01:41:10.000000 itertable-2.1.0/tests/files/test.shx
--rw-r--r--   0 sheppard  (1000) sheppard  (1000)     4067 2022-06-22 01:41:10.000000 itertable-2.1.0/tests/files/testxlsx.zip
--rw-r--r--   0 sheppard  (1000) sheppard  (1000)      280 2022-06-22 01:41:10.000000 itertable-2.1.0/tests/files/custom.xml
--rw-r--r--   0 sheppard  (1000) sheppard  (1000)      234 2022-06-22 01:41:10.000000 itertable-2.1.0/tests/files/custom.json
--rw-r--r--   0 sheppard  (1000) sheppard  (1000)       23 2022-06-22 01:41:10.000000 itertable-2.1.0/tests/files/.gitignore
--rw-r--r--   0 sheppard  (1000) sheppard  (1000)      185 2022-06-22 01:41:10.000000 itertable-2.1.0/tests/files/test.xml
--rw-r--r--   0 sheppard  (1000) sheppard  (1000)       80 2022-06-22 01:41:10.000000 itertable-2.1.0/tests/files/test2.csv
--rw-r--r--   0 sheppard  (1000) sheppard  (1000)      107 2022-06-22 01:41:10.000000 itertable-2.1.0/tests/files/test.json
--rw-r--r--   0 sheppard  (1000) sheppard  (1000)     4580 2022-06-22 01:41:10.000000 itertable-2.1.0/tests/files/test.xlsx
--rw-r--r--   0 sheppard  (1000) sheppard  (1000)     5632 2022-06-22 01:41:10.000000 itertable-2.1.0/tests/files/test.xls
--rw-r--r--   0 sheppard  (1000) sheppard  (1000)     8828 2022-06-22 01:41:10.000000 itertable-2.1.0/tests/files/nodata.xlsx
--rw-r--r--   0 sheppard  (1000) sheppard  (1000)      192 2022-06-22 01:41:10.000000 itertable-2.1.0/tests/files/testcsv.zip
--rw-r--r--   0 sheppard  (1000) sheppard  (1000)      240 2022-06-22 01:41:10.000000 itertable-2.1.0/tests/files/test.dbf
--rw-r--r--   0 sheppard  (1000) sheppard  (1000)     9768 2022-06-22 01:41:10.000000 itertable-2.1.0/tests/files/noextra.xlsx
--rw-r--r--   0 sheppard  (1000) sheppard  (1000)      259 2022-06-22 01:41:10.000000 itertable-2.1.0/tests/files/custom2.json
--rw-r--r--   0 sheppard  (1000) sheppard  (1000)     1614 2022-06-22 01:41:10.000000 itertable-2.1.0/tests/files/test.geojson
--rw-r--r--   0 sheppard  (1000) sheppard  (1000)      143 2022-06-22 01:41:10.000000 itertable-2.1.0/tests/files/test.prj
--rw-r--r--   0 sheppard  (1000) sheppard  (1000)      388 2022-06-22 01:41:10.000000 itertable-2.1.0/tests/files/test.shp
--rw-r--r--   0 sheppard  (1000) sheppard  (1000)        0 2022-06-22 01:41:10.000000 itertable-2.1.0/tests/files/nodata.csv
--rw-r--r--   0 sheppard  (1000) sheppard  (1000)       26 2022-06-22 01:41:10.000000 itertable-2.1.0/tests/files/test.csv
--rw-r--r--   0 sheppard  (1000) sheppard  (1000)       39 2022-06-22 01:41:10.000000 itertable-2.1.0/tests/files/test3.csv
--rw-r--r--   0 sheppard  (1000) sheppard  (1000)      390 2022-06-22 01:41:10.000000 itertable-2.1.0/tests/files/testmulti.zip
--rw-r--r--   0 sheppard  (1000) sheppard  (1000)     9816 2022-06-22 01:41:10.000000 itertable-2.1.0/tests/files/extra.xlsx
--rw-r--r--   0 sheppard  (1000) sheppard  (1000)     3209 2022-06-22 01:41:10.000000 itertable-2.1.0/CODE_OF_CONDUCT.md
--rw-r--r--   0 sheppard  (1000) sheppard  (1000)     1083 2022-06-22 01:41:10.000000 itertable-2.1.0/LICENSE
--rw-r--r--   0 sheppard  (1000) sheppard  (1000)     6306 2022-06-22 01:41:10.000000 itertable-2.1.0/README.md
-drwxr-xr-x   0 sheppard  (1000) sheppard  (1000)        0 2022-06-22 01:41:27.000000 itertable-2.1.0/docs/
--rw-r--r--   0 sheppard  (1000) sheppard  (1000)     3395 2022-06-22 01:41:10.000000 itertable-2.1.0/docs/gis.md
--rw-r--r--   0 sheppard  (1000) sheppard  (1000)     9838 2022-06-22 01:41:10.000000 itertable-2.1.0/docs/parsers.md
--rw-r--r--   0 sheppard  (1000) sheppard  (1000)     3665 2022-06-22 01:41:10.000000 itertable-2.1.0/docs/loaders.md
--rw-r--r--   0 sheppard  (1000) sheppard  (1000)     4864 2022-06-22 01:41:10.000000 itertable-2.1.0/docs/base.md
--rw-r--r--   0 sheppard  (1000) sheppard  (1000)     3641 2022-06-22 01:41:10.000000 itertable-2.1.0/docs/about.md
--rw-r--r--   0 sheppard  (1000) sheppard  (1000)     4612 2022-06-22 01:41:10.000000 itertable-2.1.0/docs/mappers.md
-drwxr-xr-x   0 sheppard  (1000) sheppard  (1000)        0 2022-06-22 01:41:27.000000 itertable-2.1.0/.github/
-drwxr-xr-x   0 sheppard  (1000) sheppard  (1000)        0 2022-06-22 01:41:27.000000 itertable-2.1.0/.github/workflows/
--rw-r--r--   0 sheppard  (1000) sheppard  (1000)     1397 2022-06-22 01:41:10.000000 itertable-2.1.0/.github/workflows/test.yml
-drwxr-xr-x   0 sheppard  (1000) sheppard  (1000)        0 2022-06-22 01:41:27.000000 itertable-2.1.0/itertable.egg-info/
--rw-r--r--   0 sheppard  (1000) sheppard  (1000)       10 2022-06-22 01:41:27.000000 itertable-2.1.0/itertable.egg-info/top_level.txt
--rw-r--r--   0 sheppard  (1000) sheppard  (1000)        1 2022-06-22 01:41:27.000000 itertable-2.1.0/itertable.egg-info/dependency_links.txt
--rw-r--r--   0 sheppard  (1000) sheppard  (1000)     1484 2022-06-22 01:41:27.000000 itertable-2.1.0/itertable.egg-info/SOURCES.txt
--rw-r--r--   0 sheppard  (1000) sheppard  (1000)       86 2022-06-22 01:41:27.000000 itertable-2.1.0/itertable.egg-info/requires.txt
--rw-r--r--   0 sheppard  (1000) sheppard  (1000)     8464 2022-06-22 01:41:27.000000 itertable-2.1.0/itertable.egg-info/PKG-INFO
--rw-r--r--   0 sheppard  (1000) sheppard  (1000)       38 2022-06-22 01:41:27.000000 itertable-2.1.0/setup.cfg
--rw-r--r--   0 sheppard  (1000) sheppard  (1000)     1554 2022-06-22 01:41:10.000000 itertable-2.1.0/setup.py
-drwxr-xr-x   0 sheppard  (1000) sheppard  (1000)        0 2022-06-22 01:41:27.000000 itertable-2.1.0/itertable/
--rw-r--r--   0 sheppard  (1000) sheppard  (1000)       65 2022-06-22 01:41:10.000000 itertable-2.1.0/itertable/__main__.py
--rw-r--r--   0 sheppard  (1000) sheppard  (1000)     2413 2022-06-22 01:41:10.000000 itertable-2.1.0/itertable/commands.py
--rw-r--r--   0 sheppard  (1000) sheppard  (1000)     1262 2022-06-22 01:41:10.000000 itertable-2.1.0/itertable/exceptions.py
--rw-r--r--   0 sheppard  (1000) sheppard  (1000)     4986 2022-06-22 01:41:10.000000 itertable-2.1.0/itertable/loaders.py
--rw-r--r--   0 sheppard  (1000) sheppard  (1000)      173 2022-06-22 01:41:10.000000 itertable-2.1.0/itertable/version.py
-drwxr-xr-x   0 sheppard  (1000) sheppard  (1000)        0 2022-06-22 01:41:27.000000 itertable-2.1.0/itertable/parsers/
--rw-r--r--   0 sheppard  (1000) sheppard  (1000)     3753 2022-06-22 01:41:10.000000 itertable-2.1.0/itertable/parsers/text.py
--rw-r--r--   0 sheppard  (1000) sheppard  (1000)     9104 2022-06-22 01:41:10.000000 itertable-2.1.0/itertable/parsers/xls.py
--rw-r--r--   0 sheppard  (1000) sheppard  (1000)     2245 2022-06-22 01:41:10.000000 itertable-2.1.0/itertable/parsers/readers.py
--rw-r--r--   0 sheppard  (1000) sheppard  (1000)      176 2022-06-22 01:41:10.000000 itertable-2.1.0/itertable/parsers/base.py
--rw-r--r--   0 sheppard  (1000) sheppard  (1000)      205 2022-06-22 01:41:10.000000 itertable-2.1.0/itertable/parsers/__init__.py
--rw-r--r--   0 sheppard  (1000) sheppard  (1000)     5645 2022-06-22 01:41:10.000000 itertable-2.1.0/itertable/util.py
--rw-r--r--   0 sheppard  (1000) sheppard  (1000)     6527 2022-06-22 01:41:10.000000 itertable-2.1.0/itertable/base.py
-drwxr-xr-x   0 sheppard  (1000) sheppard  (1000)        0 2022-06-22 01:41:27.000000 itertable-2.1.0/itertable/gis/
--rw-r--r--   0 sheppard  (1000) sheppard  (1000)     4792 2022-06-22 01:41:10.000000 itertable-2.1.0/itertable/gis/mixins.py
--rw-r--r--   0 sheppard  (1000) sheppard  (1000)      964 2022-06-22 01:41:10.000000 itertable-2.1.0/itertable/gis/__init__.py
--rw-r--r--   0 sheppard  (1000) sheppard  (1000)     5807 2022-06-22 01:41:10.000000 itertable-2.1.0/itertable/mappers.py
--rw-r--r--   0 sheppard  (1000) sheppard  (1000)     2094 2022-06-22 01:41:10.000000 itertable-2.1.0/itertable/__init__.py
--rw-r--r--   0 sheppard  (1000) sheppard  (1000)     1192 2022-06-22 01:41:10.000000 itertable-2.1.0/CONTRIBUTING.md
--rw-r--r--   0 sheppard  (1000) sheppard  (1000)     8464 2022-06-22 01:41:27.000000 itertable-2.1.0/PKG-INFO
+drwxr-xr-x   0 sheppard  (1000) sheppard  (1000)        0 2023-06-16 16:02:52.160252 itertable-2.2.0/
+drwxr-xr-x   0 sheppard  (1000) sheppard  (1000)        0 2023-06-16 16:02:51.675261 itertable-2.2.0/.github/
+drwxr-xr-x   0 sheppard  (1000) sheppard  (1000)        0 2023-06-16 16:02:51.732240 itertable-2.2.0/.github/workflows/
+-rw-r--r--   0 sheppard  (1000) sheppard  (1000)     1491 2023-06-16 15:59:03.000000 itertable-2.2.0/.github/workflows/test.yml
+-rw-r--r--   0 sheppard  (1000) sheppard  (1000)       66 2023-06-16 15:59:03.000000 itertable-2.2.0/.gitignore
+-rw-r--r--   0 sheppard  (1000) sheppard  (1000)     3209 2023-06-16 15:59:03.000000 itertable-2.2.0/CODE_OF_CONDUCT.md
+-rw-r--r--   0 sheppard  (1000) sheppard  (1000)     1412 2023-06-16 15:59:03.000000 itertable-2.2.0/CONTRIBUTING.md
+-rw-r--r--   0 sheppard  (1000) sheppard  (1000)     1083 2023-06-16 15:59:03.000000 itertable-2.2.0/LICENSE
+-rw-r--r--   0 sheppard  (1000) sheppard  (1000)     3449 2023-06-16 16:02:52.157267 itertable-2.2.0/PKG-INFO
+-rw-r--r--   0 sheppard  (1000) sheppard  (1000)     2028 2023-06-16 15:59:03.000000 itertable-2.2.0/README.md
+drwxr-xr-x   0 sheppard  (1000) sheppard  (1000)        0 2023-06-16 16:02:51.806254 itertable-2.2.0/itertable/
+-rw-r--r--   0 sheppard  (1000) sheppard  (1000)     2153 2023-06-16 15:59:03.000000 itertable-2.2.0/itertable/__init__.py
+-rw-r--r--   0 sheppard  (1000) sheppard  (1000)       65 2023-06-16 15:59:03.000000 itertable-2.2.0/itertable/__main__.py
+-rw-r--r--   0 sheppard  (1000) sheppard  (1000)     6536 2023-06-16 15:59:03.000000 itertable-2.2.0/itertable/base.py
+-rw-r--r--   0 sheppard  (1000) sheppard  (1000)     2413 2023-06-16 15:59:03.000000 itertable-2.2.0/itertable/commands.py
+-rw-r--r--   0 sheppard  (1000) sheppard  (1000)     1265 2023-06-16 15:59:03.000000 itertable-2.2.0/itertable/exceptions.py
+drwxr-xr-x   0 sheppard  (1000) sheppard  (1000)        0 2023-06-16 16:02:51.848238 itertable-2.2.0/itertable/gis/
+-rw-r--r--   0 sheppard  (1000) sheppard  (1000)      947 2023-06-16 15:59:03.000000 itertable-2.2.0/itertable/gis/__init__.py
+-rw-r--r--   0 sheppard  (1000) sheppard  (1000)     4951 2023-06-16 15:59:03.000000 itertable-2.2.0/itertable/gis/mixins.py
+-rw-r--r--   0 sheppard  (1000) sheppard  (1000)     5030 2023-06-16 15:59:03.000000 itertable-2.2.0/itertable/loaders.py
+-rw-r--r--   0 sheppard  (1000) sheppard  (1000)     5794 2023-06-16 15:59:03.000000 itertable-2.2.0/itertable/mappers.py
+drwxr-xr-x   0 sheppard  (1000) sheppard  (1000)        0 2023-06-16 16:02:51.886221 itertable-2.2.0/itertable/parsers/
+-rw-r--r--   0 sheppard  (1000) sheppard  (1000)      205 2023-06-16 15:59:03.000000 itertable-2.2.0/itertable/parsers/__init__.py
+-rw-r--r--   0 sheppard  (1000) sheppard  (1000)      176 2023-06-16 15:59:03.000000 itertable-2.2.0/itertable/parsers/base.py
+-rw-r--r--   0 sheppard  (1000) sheppard  (1000)     2298 2023-06-16 15:59:03.000000 itertable-2.2.0/itertable/parsers/readers.py
+-rw-r--r--   0 sheppard  (1000) sheppard  (1000)     3755 2023-06-16 15:59:03.000000 itertable-2.2.0/itertable/parsers/text.py
+-rw-r--r--   0 sheppard  (1000) sheppard  (1000)     9201 2023-06-16 15:59:03.000000 itertable-2.2.0/itertable/parsers/xls.py
+-rw-r--r--   0 sheppard  (1000) sheppard  (1000)     5665 2023-06-16 15:59:03.000000 itertable-2.2.0/itertable/util.py
+-rw-r--r--   0 sheppard  (1000) sheppard  (1000)      160 2023-06-16 16:02:51.000000 itertable-2.2.0/itertable/version.py
+drwxr-xr-x   0 sheppard  (1000) sheppard  (1000)        0 2023-06-16 16:02:51.835241 itertable-2.2.0/itertable.egg-info/
+-rw-r--r--   0 sheppard  (1000) sheppard  (1000)     3449 2023-06-16 16:02:51.000000 itertable-2.2.0/itertable.egg-info/PKG-INFO
+-rw-r--r--   0 sheppard  (1000) sheppard  (1000)     1403 2023-06-16 16:02:51.000000 itertable-2.2.0/itertable.egg-info/SOURCES.txt
+-rw-r--r--   0 sheppard  (1000) sheppard  (1000)        1 2023-06-16 16:02:51.000000 itertable-2.2.0/itertable.egg-info/dependency_links.txt
+-rw-r--r--   0 sheppard  (1000) sheppard  (1000)       85 2023-06-16 16:02:51.000000 itertable-2.2.0/itertable.egg-info/requires.txt
+-rw-r--r--   0 sheppard  (1000) sheppard  (1000)       10 2023-06-16 16:02:51.000000 itertable-2.2.0/itertable.egg-info/top_level.txt
+-rw-r--r--   0 sheppard  (1000) sheppard  (1000)     1633 2023-06-16 15:59:27.000000 itertable-2.2.0/pyproject.toml
+-rw-r--r--   0 sheppard  (1000) sheppard  (1000)       38 2023-06-16 16:02:52.164259 itertable-2.2.0/setup.cfg
+drwxr-xr-x   0 sheppard  (1000) sheppard  (1000)        0 2023-06-16 16:02:51.959263 itertable-2.2.0/tests/
+-rw-r--r--   0 sheppard  (1000) sheppard  (1000)        0 2023-06-16 15:59:03.000000 itertable-2.2.0/tests/__init__.py
+-rw-r--r--   0 sheppard  (1000) sheppard  (1000)      997 2023-06-16 15:59:03.000000 itertable-2.2.0/tests/base.py
+drwxr-xr-x   0 sheppard  (1000) sheppard  (1000)        0 2023-06-16 16:02:52.149238 itertable-2.2.0/tests/files/
+-rw-r--r--   0 sheppard  (1000) sheppard  (1000)       23 2023-06-16 15:59:03.000000 itertable-2.2.0/tests/files/.gitignore
+-rw-r--r--   0 sheppard  (1000) sheppard  (1000)      234 2023-06-16 15:59:03.000000 itertable-2.2.0/tests/files/custom.json
+-rw-r--r--   0 sheppard  (1000) sheppard  (1000)      280 2023-06-16 15:59:03.000000 itertable-2.2.0/tests/files/custom.xml
+-rw-r--r--   0 sheppard  (1000) sheppard  (1000)      259 2023-06-16 15:59:03.000000 itertable-2.2.0/tests/files/custom2.json
+-rw-r--r--   0 sheppard  (1000) sheppard  (1000)     9816 2023-06-16 15:59:04.000000 itertable-2.2.0/tests/files/extra.xlsx
+-rw-r--r--   0 sheppard  (1000) sheppard  (1000)        0 2023-06-16 15:59:04.000000 itertable-2.2.0/tests/files/nodata.csv
+-rw-r--r--   0 sheppard  (1000) sheppard  (1000)     8828 2023-06-16 15:59:04.000000 itertable-2.2.0/tests/files/nodata.xlsx
+-rw-r--r--   0 sheppard  (1000) sheppard  (1000)     9768 2023-06-16 15:59:04.000000 itertable-2.2.0/tests/files/noextra.xlsx
+-rw-r--r--   0 sheppard  (1000) sheppard  (1000)       26 2023-06-16 15:59:04.000000 itertable-2.2.0/tests/files/test.csv
+-rw-r--r--   0 sheppard  (1000) sheppard  (1000)      240 2023-06-16 15:59:04.000000 itertable-2.2.0/tests/files/test.dbf
+-rw-r--r--   0 sheppard  (1000) sheppard  (1000)     1614 2023-06-16 15:59:04.000000 itertable-2.2.0/tests/files/test.geojson
+-rw-r--r--   0 sheppard  (1000) sheppard  (1000)      107 2023-06-16 15:59:04.000000 itertable-2.2.0/tests/files/test.json
+-rw-r--r--   0 sheppard  (1000) sheppard  (1000)      143 2023-06-16 15:59:04.000000 itertable-2.2.0/tests/files/test.prj
+-rw-r--r--   0 sheppard  (1000) sheppard  (1000)      388 2023-06-16 15:59:04.000000 itertable-2.2.0/tests/files/test.shp
+-rw-r--r--   0 sheppard  (1000) sheppard  (1000)      116 2023-06-16 15:59:04.000000 itertable-2.2.0/tests/files/test.shx
+-rw-r--r--   0 sheppard  (1000) sheppard  (1000)     5632 2023-06-16 15:59:04.000000 itertable-2.2.0/tests/files/test.xls
+-rw-r--r--   0 sheppard  (1000) sheppard  (1000)     4580 2023-06-16 15:59:04.000000 itertable-2.2.0/tests/files/test.xlsx
+-rw-r--r--   0 sheppard  (1000) sheppard  (1000)      185 2023-06-16 15:59:04.000000 itertable-2.2.0/tests/files/test.xml
+-rw-r--r--   0 sheppard  (1000) sheppard  (1000)       80 2023-06-16 15:59:04.000000 itertable-2.2.0/tests/files/test2.csv
+-rw-r--r--   0 sheppard  (1000) sheppard  (1000)       39 2023-06-16 15:59:04.000000 itertable-2.2.0/tests/files/test3.csv
+-rw-r--r--   0 sheppard  (1000) sheppard  (1000)      192 2023-06-16 15:59:04.000000 itertable-2.2.0/tests/files/testcsv.zip
+-rw-r--r--   0 sheppard  (1000) sheppard  (1000)      390 2023-06-16 15:59:04.000000 itertable-2.2.0/tests/files/testmulti.zip
+-rw-r--r--   0 sheppard  (1000) sheppard  (1000)     4067 2023-06-16 15:59:04.000000 itertable-2.2.0/tests/files/testxlsx.zip
+-rw-r--r--   0 sheppard  (1000) sheppard  (1000)     1433 2023-06-16 15:59:04.000000 itertable-2.2.0/tests/test_custom.py
+-rw-r--r--   0 sheppard  (1000) sheppard  (1000)      895 2023-06-16 15:59:04.000000 itertable-2.2.0/tests/test_dataframe.py
+-rw-r--r--   0 sheppard  (1000) sheppard  (1000)     1420 2023-06-16 15:59:04.000000 itertable-2.2.0/tests/test_extra_data.py
+-rw-r--r--   0 sheppard  (1000) sheppard  (1000)     2030 2023-06-16 15:59:04.000000 itertable-2.2.0/tests/test_gis.py
+-rw-r--r--   0 sheppard  (1000) sheppard  (1000)      574 2023-06-16 15:59:04.000000 itertable-2.2.0/tests/test_gis_dataframe.py
+-rw-r--r--   0 sheppard  (1000) sheppard  (1000)     5085 2023-06-16 15:59:04.000000 itertable-2.2.0/tests/test_load_file.py
+-rw-r--r--   0 sheppard  (1000) sheppard  (1000)     3126 2023-06-16 15:59:04.000000 itertable-2.2.0/tests/test_netloader.py
+-rw-r--r--   0 sheppard  (1000) sheppard  (1000)     3345 2023-06-16 15:59:04.000000 itertable-2.2.0/tests/test_write.py
+-rw-r--r--   0 sheppard  (1000) sheppard  (1000)     2319 2023-06-16 15:59:04.000000 itertable-2.2.0/tests/test_zip.py
```

### filetype from file(1)

```diff
@@ -1 +1 @@
-POSIX tar archive (GNU)
+POSIX tar archive
```

### Comparing `itertable-2.1.0/tests/test_netloader.py` & `itertable-2.2.0/tests/test_netloader.py`

 * *Files 7% similar despite different names*

```diff
@@ -13,15 +13,15 @@
     def setUp(self):
         httpretty.enable()
 
         httpretty.register_uri(
             httpretty.GET,
             "http://example.com/test.csv",
             body="one,two,three\n1,2,3\n4,5,6",
-            content_type="text/csv"
+            content_type="text/csv",
         )
         httpretty.register_uri(
             httpretty.GET,
             "http://example.com/fail.txt",
             body="Not Found",
             content_type="text/plain",
             status=404,
@@ -41,58 +41,61 @@
     def test_load_csv(self):
         self.check_instance(TestIter())
 
     def test_load_url(self):
         self.check_instance(load_url("http://example.com/test.csv"))
 
     def test_load_csv_params(self):
-        self.check_instance(TestIter(params={'test': 1}))
+        self.check_instance(TestIter(params={"test": 1}))
         qs = httpretty.last_request().querystring
-        self.assertEqual(qs, {'test': ['1']})
+        self.assertEqual(qs, {"test": ["1"]})
 
         self.check_instance(TestIter(params="test=1"))
         qs = httpretty.last_request().querystring
-        self.assertEqual(qs, {'test': ['1']})
+        self.assertEqual(qs, {"test": ["1"]})
 
         self.check_instance(TestIter(params=None))
         qs = httpretty.last_request().querystring
         self.assertEqual(qs, {})
 
     def test_debug_string(self):
         instance = TestIter(debug=True)
         self.assertEqual(
             instance.debug_string, "GET: http://example.com/test.csv"
         )
-        instance = TestIter(params={'test': 1}, debug=True)
+        instance = TestIter(params={"test": 1}, debug=True)
         self.assertEqual(
             instance.debug_string, "GET: http://example.com/test.csv?test=1"
         )
 
     def test_load_csv_auth(self):
         class AuthTestIter(CsvNetIter):
             url = "http://example.com/test.csv"
             username = "user"
             password = "pass"
+
         self.check_instance(AuthTestIter())
         headers = httpretty.last_request().headers
         auth = "Basic dXNlcjpwYXNz"  # b64encode("user:pass")
-        self.assertEqual(headers.get('Authorization', None), auth)
+        self.assertEqual(headers.get("Authorization", None), auth)
 
     def test_load_csv_pickle(self):
         instance = TestIter()
         self.check_instance(instance)
         instance = pickle.loads(pickle.dumps(instance))
         self.check_instance(instance)
 
     def test_load_fail(self):
         class TestIter(CsvNetIter):
             url = "http://example.com/fail.txt"
+
         with self.assertRaises(LoadFailed) as cm:
             TestIter()
         self.assertEqual(str(cm.exception), "Not Found")
 
     def test_load_fail_html(self):
         class TestIter(CsvNetIter):
             url = "http://example.com/fail.html"
+
         with self.assertRaises(LoadFailed) as cm:
             TestIter()
         self.assertEqual(str(cm.exception), "Not Found")
```

### Comparing `itertable-2.1.0/tests/test_write.py` & `itertable-2.2.0/tests/test_write.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,26 +1,33 @@
 from itertable import load_file
 from itertable import (
-    CsvFileIter, JsonFileIter, XmlFileIter, OldExcelFileIter, ExcelFileIter
+    CsvFileIter,
+    JsonFileIter,
+    XmlFileIter,
+    OldExcelFileIter,
+    ExcelFileIter,
 )
 from .base import IterTestCase
 
 
 class LoadFileTestCase(IterTestCase):
     def setUp(self):
-        self.data = [{
-            'one': 1,
-            'two': 2,
-            'three': 3,
-        }, {
-            'one': 4,
-            'two': 5,
-            'three': 6,
-        }]
-        self.types = ('csv', 'json', 'xml', 'xls', 'xlsx')
+        self.data = [
+            {
+                "one": 1,
+                "two": 2,
+                "three": 3,
+            },
+            {
+                "one": 4,
+                "two": 5,
+                "three": 6,
+            },
+        ]
+        self.types = ("csv", "json", "xml", "xls", "xlsx")
         self.classes = (
             CsvFileIter,
             JsonFileIter,
             XmlFileIter,
             OldExcelFileIter,
             ExcelFileIter,
         )
@@ -32,19 +39,18 @@
         for ext, cls in zip(self.types, self.classes):
             filename = self.get_filename("output", ext, True)
 
             # Create an empty instance of the class
             instance = cls(
                 filename=filename,
                 require_existing=False,
-                field_names=['one', 'two', 'three'],
-
+                field_names=["one", "two", "three"],
                 # These only apply to XmlFileIter, will be ignored by others
                 root_tag="root",
-                item_tag="item"
+                item_tag="item",
             )
 
             # Add rows to the instance using list-style BaseIter.append()
             for row in self.data:
                 instance.append(instance.create(**row))
 
             # Save the instance, which should write to output.[ext]
@@ -70,29 +76,30 @@
                 # Load source data into Iter instance
                 source_instance = source_cls(filename=source_file)
 
                 # Create empty instance of the destination Iter class
                 dest_instance = dest_cls(
                     filename=dest_file,
                     require_existing=False,
-                    field_names=['one', 'two', 'three'],
+                    field_names=["one", "two", "three"],
                     root_tag="root",
                     item_tag="item",
                 )
 
                 # The Sync
                 getattr(source_instance, mode)(dest_instance)
 
                 # Load the destination file again and check contents
                 self.check_instance(load_file(dest_file))
 
     def test_copy_io(self):
-        self.duplicate('copy', lambda d: d)
+        self.duplicate("copy", lambda d: d)
 
     def test_sync_io(self):
-        self.duplicate('sync', self.with_key_field)
+        self.duplicate("sync", self.with_key_field)
 
     def with_key_field(self, cls):
         class new_class(cls):
             key_field = "one"
+
         new_class.__name__ = "Dict" + cls.__name__
         return new_class
```

### Comparing `itertable-2.1.0/tests/test_load_file.py` & `itertable-2.2.0/tests/test_load_file.py`

 * *Files 8% similar despite different names*

```diff
@@ -9,49 +9,49 @@
     import magic
 except ImportError:
     magic = None
 
 
 class LoadFileTestCase(IterTestCase):
     def setUp(self):
-        self.types = ('csv', 'json', 'xml', 'xls', 'xlsx')
+        self.types = ("csv", "json", "xml", "xls", "xlsx")
 
     def test_load_file(self):
         for ext in self.types:
             filename = self.get_filename("test", ext)
             instance = load_file(filename)
             self.check_instance(instance)
 
     def test_load_file_object(self):
         for ext in self.types:
             filename = self.get_filename("test", ext)
-            if ext in ('xls', 'xlsx'):
-                mode = 'rb'
+            if ext in ("xls", "xlsx"):
+                mode = "rb"
             else:
-                mode = 'r'
+                mode = "r"
             with open(filename, mode) as f:
                 instance = load_file(f)
             self.check_instance(instance)
 
     def test_load_file_object_binary(self):
         for ext in self.types:
             filename = self.get_filename("test", ext)
-            with open(filename, 'rb') as f:
+            with open(filename, "rb") as f:
                 instance = load_file(f)
             self.check_instance(instance)
 
     @unittest.skipUnless(magic, "magic required for buffer-based detection")
     def test_load_file_object_no_name(self):
         for ext in self.types:
             filename = self.get_filename("test", ext)
-            if ext in ('xls', 'xlsx'):
-                mode = 'rb'
+            if ext in ("xls", "xlsx"):
+                mode = "rb"
                 IO = io.BytesIO
             else:
-                mode = 'r'
+                mode = "r"
                 IO = io.StringIO
 
             with open(filename, mode) as f:
                 obj = IO(f.read())
 
             instance = load_file(obj)
             self.check_instance(instance)
@@ -60,15 +60,15 @@
         class FileLike:
             name = "test.csv"
 
             def read(self, *args, **kwargs):
                 return "one,two,three\n1,2,3\n4,5,6"
 
             def __iter__(self):
-                yield from self.read().split('\n')
+                yield from self.read().split("\n")
 
         instance = load_file(FileLike())
         self.check_instance(instance)
 
     def test_load_non_file(self):
         with self.assertRaises(AssertionError):
             load_file([{"value": "not a file"}])
@@ -83,17 +83,17 @@
         instance = load_file(filename)
         self.check_instance(instance)
         self.assertTrue(hasattr(instance[0], "μ"))
         self.assertEqual(instance[0].μ, "test")
 
     def test_load_xlsx_sheets(self):
         filename = self.get_filename("test", "xlsx")
-        instance = load_file(filename, options={'sheet_name': None})
+        instance = load_file(filename, options={"sheet_name": None})
         self.assertEqual(len(instance), 1)
-        self.assertEqual(instance[0].name, 'Sheet1')
+        self.assertEqual(instance[0].name, "Sheet1")
         self.check_instance(instance[0].data)
 
     def test_load_nodata(self):
         filename = self.get_filename("nodata", "csv")
         instance = load_file(filename)
         with self.assertRaises(NoData) as cm:
             instance[0]
@@ -104,31 +104,31 @@
         instance = load_file(filename)
         with self.assertRaises(NoData) as cm:
             instance[0]
         self.assertEqual(str(cm.exception), "No data returned!")
 
     def test_load_nodata_excel_sheets(self):
         filename = self.get_filename("nodata", "xlsx")
-        instance = load_file(filename, options={'sheet_name': None})
+        instance = load_file(filename, options={"sheet_name": None})
         self.assertEqual(len(instance), 1)
-        self.assertEqual(instance[0].name, 'Sheet1')
+        self.assertEqual(instance[0].name, "Sheet1")
         sheet = instance[0].data
         with self.assertRaises(NoData) as cm:
             sheet[0]
         self.assertEqual(str(cm.exception), "No data returned!")
 
     def test_load_non_existing(self):
         filename = self.get_filename("nonexisting", "csv")
         with self.assertRaises(LoadFailed) as cm:
             load_file(filename)
         self.assertEqual(str(cm.exception), "No such file or directory")
 
     def test_load_init_empty(self):
         filename = self.get_filename("nonexisting", "csv")
-        instance = load_file(filename, options={'require_existing': False})
+        instance = load_file(filename, options={"require_existing": False})
         with self.assertRaises(NoData) as cm:
             instance[0]
         self.assertEqual(str(cm.exception), "No data returned!")
 
     def test_pickle(self):
         for ext in self.types:
             filename = self.get_filename("test", ext)
```

### Comparing `itertable-2.1.0/tests/test_custom.py` & `itertable-2.2.0/tests/test_custom.py`

 * *Files identical despite different names*

### Comparing `itertable-2.1.0/tests/test_dataframe.py` & `itertable-2.2.0/tests/test_dataframe.py`

 * *Files 2% similar despite different names*

```diff
@@ -26,9 +26,9 @@
         self.assertEqual(val, 6)
 
     def test_csv_dataframe(self):
         io = load_string(self.csv_data)
         df = io.as_dataframe()
         self.assertEqual(len(df), 2)
 
-        val = df[df.two == '2'].three[0]
-        self.assertEqual(val, '3')
+        val = df[df.two == "2"].three[0]
+        self.assertEqual(val, "3")
```

### Comparing `itertable-2.1.0/tests/test_gis.py` & `itertable-2.2.0/tests/test_gis.py`

 * *Files 12% similar despite different names*

```diff
@@ -6,15 +6,18 @@
 
 class GisTestCase(IterTestCase):
     def setUp(self):
         self.points = [
             Point(-93.278, 44.976),
             Point(-93.247, 44.973),
         ]
-        self.types = ('geojson', 'shp',)
+        self.types = (
+            "geojson",
+            "shp",
+        )
 
     def test_shapeio(self):
         for ext in self.types:
             filename = self.get_filename("test", ext)
             instance = ShapeIter(filename=filename)
             self.check_instance(instance)
 
@@ -43,14 +46,14 @@
                 self.assertEqual(val, data[key])
                 self.assertTrue(row.geometry.contains(point))
 
     def get_filename(self, filename, ext, remove_existing=False):
         filename = super(GisTestCase, self).get_filename(
             filename, ext, remove_existing
         )
-        if ext == 'shp' and remove_existing:
-            for ext in ('dbf', 'shx', 'prj'):
+        if ext == "shp" and remove_existing:
+            for ext in ("dbf", "shx", "prj"):
                 try:
-                    unlink(filename.replace('shp', ext))
+                    unlink(filename.replace("shp", ext))
                 except OSError:
                     pass
         return filename
```

### Comparing `itertable-2.1.0/tests/test_zip.py` & `itertable-2.2.0/tests/test_zip.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,10 +1,14 @@
 from itertable import (
-    ZipFileLoader, ZipNetLoader,
-    CsvParser, ExcelParser, TupleMapper, BaseIter
+    ZipFileLoader,
+    ZipNetLoader,
+    CsvParser,
+    ExcelParser,
+    TupleMapper,
+    BaseIter,
 )
 from .base import IterTestCase
 from itertable.exceptions import LoadFailed
 import httpretty
 
 
 class CsvZipFileIter(ZipFileLoader, CsvParser, TupleMapper, BaseIter):
@@ -59,15 +63,15 @@
         zipfile = open(filename, "rb")
         zipdata = zipfile.read()
         zipfile.close()
         httpretty.register_uri(
             httpretty.GET,
             "http://example.com/%s.zip" % name,
             body=zipdata,
-            content_type="application/zip"
+            content_type="application/zip",
         )
 
     def tearDown(self):
         httpretty.disable()
         httpretty.reset()
 
     def test_load_zip(self):
```

### Comparing `itertable-2.1.0/tests/test_gis_dataframe.py` & `itertable-2.2.0/tests/test_gis_dataframe.py`

 * *Files identical despite different names*

### Comparing `itertable-2.1.0/tests/test_extra_data.py` & `itertable-2.2.0/tests/test_extra_data.py`

 * *Files identical despite different names*

### Comparing `itertable-2.1.0/tests/files/testxlsx.zip` & `itertable-2.2.0/tests/files/testxlsx.zip`

 * *Files identical despite different names*

### Comparing `itertable-2.1.0/tests/files/test.xlsx` & `itertable-2.2.0/tests/files/test.xlsx`

 * *Files identical despite different names*

### Comparing `itertable-2.1.0/tests/files/test.xls` & `itertable-2.2.0/tests/files/test.xls`

 * *Files identical despite different names*

### Comparing `itertable-2.1.0/tests/files/nodata.xlsx` & `itertable-2.2.0/tests/files/nodata.xlsx`

 * *Files identical despite different names*

### Comparing `itertable-2.1.0/tests/files/noextra.xlsx` & `itertable-2.2.0/tests/files/noextra.xlsx`

 * *Files identical despite different names*

### Comparing `itertable-2.1.0/tests/files/test.geojson` & `itertable-2.2.0/tests/files/test.geojson`

 * *Files identical despite different names*

### Comparing `itertable-2.1.0/tests/files/extra.xlsx` & `itertable-2.2.0/tests/files/extra.xlsx`

 * *Files identical despite different names*

### Comparing `itertable-2.1.0/CODE_OF_CONDUCT.md` & `itertable-2.2.0/CODE_OF_CONDUCT.md`

 * *Files identical despite different names*

### Comparing `itertable-2.1.0/LICENSE` & `itertable-2.2.0/LICENSE`

 * *Files identical despite different names*

### Comparing `itertable-2.1.0/.github/workflows/test.yml` & `itertable-2.2.0/.github/workflows/test.yml`

 * *Files 5% similar despite different names*

```diff
@@ -1,38 +1,41 @@
 name: Tests
 
 on: [push, pull_request]
 
 jobs:
   build:
     name: Python ${{ matrix.python-version }}, ${{ matrix.variant }}
-    runs-on: ubuntu-20.04
+    runs-on: ubuntu-22.04
     strategy:
       matrix:
-        python-version: ["3.10", 3.9, 3.8, 3.7]
+        python-version: ["3.11", "3.10", 3.9, 3.8, 3.7]
         variant: [no-magic]
         include:
-          - python-version: "3.10"
+          - python-version: "3.11"
             variant: magic
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
         python -m pip install flake8 wheel httpretty beautifulsoup4
         python -m pip install requests openpyxl click
         python -m pip install Shapely Fiona pandas geopandas xlrd xlwt
     - name: Install python-magic
       if: ${{ matrix.variant == 'magic' }}
       run: python -m pip install python-magic
     - name: Lint with flake8
       run: |
         # stop the build if there are Python syntax errors or undefined names
         flake8 . --count --select=E9,F63,F7,F82 --show-source --statistics
         # exit-zero treats all errors as warnings. The GitHub editor is 127 chars wide
         flake8 . --count --exit-zero --max-complexity=10 --max-line-length=127 --statistics
     - name: Test with unittest
       run: python -m unittest discover -s tests -t . -v
+    - name: Test build
+      run: python -m build
```

### Comparing `itertable-2.1.0/itertable.egg-info/SOURCES.txt` & `itertable-2.2.0/itertable.egg-info/SOURCES.txt`

 * *Files 9% similar despite different names*

```diff
@@ -1,20 +1,14 @@
 .gitignore
 CODE_OF_CONDUCT.md
 CONTRIBUTING.md
 LICENSE
 README.md
-setup.py
+pyproject.toml
 .github/workflows/test.yml
-docs/about.md
-docs/base.md
-docs/gis.md
-docs/loaders.md
-docs/mappers.md
-docs/parsers.md
 itertable/__init__.py
 itertable/__main__.py
 itertable/base.py
 itertable/commands.py
 itertable/exceptions.py
 itertable/loaders.py
 itertable/mappers.py
```

### Comparing `itertable-2.1.0/itertable/commands.py` & `itertable-2.2.0/itertable/commands.py`

 * *Files 19% similar despite different names*

```diff
@@ -2,17 +2,17 @@
 from .exceptions import IterException
 import click
 import os
 import importlib
 
 
 @click.command()
-@click.argument('source')
-@click.argument('source_options', required=False)
-@click.option('--format', '-f', default='csv', help='Output format')
+@click.argument("source")
+@click.argument("source_options", required=False)
+@click.option("--format", "-f", default="csv", help="Output format")
 def cat(source, source_options, format):
     """
     Display contents of a file or IterTable class.  SOURCE can be either a
     filename or a Python path.  SOURCE_OPTIONS is an optional string
     specifying init options in "name=value" format, separated by commas.
 
     The data will be printed to the terminal in CSV form, unless the format is
@@ -27,32 +27,32 @@
     python3 -m itertable http://example.com/example.csv
     python3 -m itertable itertable.CsvNetIter "url=http://example.com/example.csv"
     """  # noqa
 
     # Parse option string
     options = {}
     if source_options:
-        for opt in source_options.split(','):
-            key, val = opt.split('=')
+        for opt in source_options.split(","):
+            key, val = opt.split("=")
             if val.isdigit():
                 val = int(val)
             options[key] = val
 
     if os.path.exists(source):
         try:
             input = load_file(source, options=options)
         except IterException as e:
             raise click.ClickException(str(e))
-    elif 'http' in source and '://' in source:
+    elif "http" in source and "://" in source:
         try:
             input = load_url(source, options=options)
         except IterException as e:
             raise click.ClickException(str(e))
     else:
-        parts = source.split('.')
+        parts = source.split(".")
         class_name = parts[-1]
         module_name = ".".join(parts[:-1])
         try:
             module = importlib.import_module(module_name)
             Iter = getattr(module, class_name)
             input = flattened(Iter, **options)
         except (ImportError, ValueError, AttributeError, IterException) as e:
@@ -65,9 +65,9 @@
         OutputIter = CsvStringIter
         init = ""
     output = OutputIter(data=input.data, string=init)
     output.data = input.data
     output.save()
     result = output.string
     if output.binary:
-        result = result.decode('utf-8')
+        result = result.decode("utf-8")
     print(result)
```

### Comparing `itertable-2.1.0/itertable/exceptions.py` & `itertable-2.2.0/itertable/exceptions.py`

 * *Files 9% similar despite different names*

```diff
@@ -19,33 +19,36 @@
         self.path = path
         self.code = code
 
     def __str__(self):
         if self.args and self.args[0]:
             text = self.args[0]
             has_html = False
-            for tag in '<html', '<body', '<div':
+            for tag in "<html", "<body", "<div":
                 if tag in text or tag.upper() in text:
                     has_html = True
             if has_html and BeautifulSoup:
                 html = BeautifulSoup(text).body
                 if html:
-                    text = html.get_text('\n')
+                    text = html.get_text("\n")
             return text
         elif self.code is not None:
             return "%s Error" % self.code
         return super(LoadFailed, self).__str__()
 
 
 class ParseFailed(IterException):
     """Error parsing data!"""
+
     pass
 
 
 class MappingFailed(IterException):
     """Error processing data!"""
+
     pass
 
 
 class NoData(IterException):
     """No data returned!"""
+
     pass
```

### Comparing `itertable-2.1.0/itertable/loaders.py` & `itertable-2.2.0/itertable/loaders.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,34 +1,38 @@
 from __future__ import print_function
 import requests
 from io import StringIO, BytesIO
-from .version import VERSION
 from .exceptions import LoadFailed
 from zipfile import ZipFile
 
+try:
+    from .version import VERSION
+except ImportError:
+    VERSION = "0.0.0"
+
 
 class BaseLoader(object):
-    no_pickle_loader = ['file']
+    no_pickle_loader = ["file"]
     empty_file = None
 
     def load(self):
         raise NotImplementedError
 
 
 class FileLoader(BaseLoader):
     filename = None
     require_existing = True
 
     @property
     def read_mode(self):
-        return 'rb' if self.binary else 'r'
+        return "rb" if self.binary else "r"
 
     @property
     def write_mode(self):
-        return 'wb+' if self.binary else 'w+'
+        return "wb+" if self.binary else "w+"
 
     def load(self):
         try:
             self.file = open(self.filename, self.read_mode)
             self.empty_file = False
         except OSError as e:
             if self.require_existing:
@@ -51,21 +55,19 @@
 
 class Zipper(object):
     inner_filename = None
     inner_binary = False
 
     def unzip_file(self):
         zipfile = ZipFile(self.file)
-        inner_file = zipfile.read(
-            self.get_inner_filename(zipfile)
-        )
+        inner_file = zipfile.read(self.get_inner_filename(zipfile))
         if self.inner_binary:
             self.file = BytesIO(inner_file)
         else:
-            self.file = StringIO(inner_file.decode('utf-8'))
+            self.file = StringIO(inner_file.decode("utf-8"))
         zipfile.fp.close()
         zipfile.close()
 
     def get_inner_filename(self, zipfile):
         if self.inner_filename:
             return self.inner_filename
         names = zipfile.namelist()
@@ -90,15 +92,15 @@
 
     @property
     def _io_class(self):
         return BytesIO if self.binary else StringIO
 
     def load(self):
         if self.binary and not self.string:
-            self.string = b''
+            self.string = b""
         self.file = self._io_class(self.string)
 
     def save(self):
         file = self._io_class()
         self.dump(file)
         self.string = file.getvalue()
         file.close()
@@ -113,59 +115,61 @@
     url = None
     client = requests
 
     @property
     def user_agent(self):
         return "IterTable/%s (%s)" % (
             VERSION,
-            requests.utils.default_user_agent()
+            requests.utils.default_user_agent(),
         )
 
     @property
     def headers(self):
         return {
-            'User-Agent': self.user_agent,
+            "User-Agent": self.user_agent,
         }
 
     def load(self, **kwargs):
         result = self.GET()
         self.file = self._io_class(result)
 
     def req(self, url=None, method=None, params=None, body=None, headers={}):
         if url is None:
             url = self.url
             if url is None:
                 raise LoadFailed("No URL provided")
 
         if params is None:
-            params = getattr(self, 'params', None)
+            params = getattr(self, "params", None)
 
         if isinstance(params, str):
-            url += '?' + params
+            url += "?" + params
             params = None
 
         if self.debug:
             if params:
                 from requests.compat import urlencode
-                debug_url = url + '?' + urlencode(params, doseq=True)
+
+                debug_url = url + "?" + urlencode(params, doseq=True)
             else:
                 debug_url = url
             self.debug_string = "%s: %s" % (method, debug_url)
             print(self.debug_string)
 
         if self.username is not None and self.password is not None:
             auth = (self.username, self.password)
         else:
             auth = None
 
         all_headers = self.headers.copy()
         all_headers.update(headers)
 
         resp = self.client.request(
-            method, url,
+            method,
+            url,
             params=params,
             headers=all_headers,
             auth=auth,
             data=body,
         )
         resp.connection.close()
 
@@ -178,24 +182,24 @@
 
         if self.binary:
             return resp.content
         else:
             return resp.text
 
     def GET(self, **kwargs):
-        return self.req(method='GET', **kwargs)
+        return self.req(method="GET", **kwargs)
 
     def POST(self, **kwargs):
-        return self.req(method='POST', **kwargs)
+        return self.req(method="POST", **kwargs)
 
     def PUT(self, **kwargs):
-        return self.req(method='PUT', **kwargs)
+        return self.req(method="PUT", **kwargs)
 
     def DELETE(self, **kwargs):
-        return self.req(method='DELETE', **kwargs)
+        return self.req(method="DELETE", **kwargs)
 
 
 class ZipNetLoader(Zipper, NetLoader):
     binary = True
 
     def load(self):
         super(ZipNetLoader, self).load()
```

### Comparing `itertable-2.1.0/itertable/parsers/text.py` & `itertable-2.2.0/itertable/parsers/text.py`

 * *Files 4% similar despite different names*

```diff
@@ -6,15 +6,15 @@
 from .base import BaseParser, TableParser
 from ..exceptions import ParseFailed
 
 
 class CsvParser(TableParser):
     delimiter = ","
     quotechar = '"'
-    no_pickle_parser = ['csvdata']
+    no_pickle_parser = ["csvdata"]
     binary = False
 
     def parse(self):
         # Like DictReader, assume explicit field definition means CSV does not
         # contain column headers.
         fields = self.get_field_names()
         if self.start_row is None:
@@ -40,24 +40,25 @@
             self.header_row = self.csvdata.header_row
         self.data = [row for row in self.csvdata]
         self.extra_data = {}
 
     def reader_class(self):
         class Reader(SkipPreludeReader):
             max_header_row = self.max_header_row
+
         return Reader
 
     def dump(self, file=None):
         if file is None:
             file = self.file
         csvout = csv.DictWriter(
             file,
             self.get_field_names(),
             delimiter=self.delimiter,
-            quotechar=self.quotechar
+            quotechar=self.quotechar,
         )
         csvout.writeheader()
         for row in self.data:
             csvout.writerow(row)
 
 
 class JsonParser(BaseParser):
@@ -65,29 +66,29 @@
     namespace = None
     binary = False
 
     def parse(self):
         try:
             obj = json.load(self.file)
             if self.namespace:
-                for key in self.namespace.split('.'):
+                for key in self.namespace.split("."):
                     obj = obj[key]
             self.data = list(map(self.parse_item, obj))
         except ValueError:
             raise ParseFailed
 
     def parse_item(self, item):
         return item
 
     def dump(self, file=None):
         if file is None:
             file = self.file
         obj = list(map(self.dump_item, self.data))
         if self.namespace:
-            for key in reversed(self.namespace.split('.')):
+            for key in reversed(self.namespace.split(".")):
                 obj = {key: obj}
         json.dump(obj, file, indent=self.indent)
 
     def dump_item(self, item):
         return item
 
 
@@ -116,15 +117,15 @@
 
     def dump(self, file=None):
         if file is None:
             file = self.file
         root = ET.Element(self.root_tag)
         for item in self.data:
             root.append(self.dump_item(item))
-        output = ET.tostring(root).decode('utf-8')
+        output = ET.tostring(root).decode("utf-8")
         file.write(output)
 
     def dump_item(self, item):
         el = ET.Element(self.item_tag)
         for key in self.get_field_names():
             if key not in item or item[key] is None:
                 continue
```

### Comparing `itertable-2.1.0/itertable/parsers/xls.py` & `itertable-2.2.0/itertable/parsers/xls.py`

 * *Files 2% similar despite different names*

```diff
@@ -5,35 +5,38 @@
 
 class WorkbookParser(TableParser):
     workbook = None
     worksheet = None
     sheet_name = 0
     start_row = None
     column_count = None
-    no_pickle_parser = ['workbook', 'worksheet']
+    no_pickle_parser = ["workbook", "worksheet"]
     binary = True
 
-    date_format = 'yyyy-mm-dd'
-    time_format = 'hh:mm:ss'
-    datetime_format = 'yyyy-mm-dd hh:mm:ss'
+    date_format = "yyyy-mm-dd"
+    time_format = "hh:mm:ss"
+    datetime_format = "yyyy-mm-dd hh:mm:ss"
 
     def parse(self):
         if not self.workbook:
             self.parse_workbook()
 
         if self.sheet_name is None:
             SpreadsheetIter = type(self)
-            self.data = [{
-                'name': name,
-                'data': SpreadsheetIter(
-                    loaded=True,
-                    workbook=self.workbook,
-                    sheet_name=name,
-                )
-            } for name in self.sheet_names]
+            self.data = [
+                {
+                    "name": name,
+                    "data": SpreadsheetIter(
+                        loaded=True,
+                        workbook=self.workbook,
+                        sheet_name=name,
+                    ),
+                }
+                for name in self.sheet_names
+            ]
             return
 
         sheet_name = self.sheet_name
         if isinstance(self.sheet_name, int):
             sheet_name = self.sheet_names[sheet_name]
 
         self.parse_worksheet(sheet_name)
@@ -41,15 +44,15 @@
         if self.header_row is None:
             if self.start_row is not None:
                 self.header_row = self.start_row - 1
             else:
                 self.column_count = 0
 
                 def checkval(cell):
-                    if cell.value is not None and cell.value != '':
+                    if cell.value is not None and cell.value != "":
                         return True
                     return False
 
                 search_rows = min(len(self.worksheet) - 1, self.max_header_row)
                 for row in range(search_rows, -1, -1):
                     count = len(list(filter(checkval, self.worksheet[row])))
                     if count >= self.column_count:
@@ -59,37 +62,37 @@
         if self.header_row is None:
             return
 
         if self.start_row is None:
             self.start_row = self.header_row + 1
 
         if self.field_names is None:
-            rows = self.worksheet[self.header_row:self.start_row]
+            rows = self.worksheet[self.header_row : self.start_row]
             self.field_names = [
-                str(c.value) or 'c%s' % i for i, c in enumerate(rows[0])
+                str(c.value) or "c%s" % i for i, c in enumerate(rows[0])
             ]
             for row in rows[1:]:
                 for i, c in enumerate(row):
                     self.field_names[i] += "\n" + str(c.value)
 
             seen_fields = set()
             for i, field in enumerate(self.field_names):
                 if field in seen_fields:
                     field += str(i)
                     self.field_names[i] = field
                 seen_fields.add(field)
 
-        self.data = list(map(self.parse_row, self.worksheet[self.start_row:]))
+        self.data = list(map(self.parse_row, self.worksheet[self.start_row :]))
 
         self.extra_data = {}
         if self.header_row > 0:
             for r in range(0, self.header_row):
                 for c, cell in enumerate(self.worksheet[r]):
                     val = self.get_value(cell)
-                    if val is not None and val != '':
+                    if val is not None and val != "":
                         self.extra_data.setdefault(r, {})
                         self.extra_data[r][c] = val
 
     def parse_workbook(self):
         raise NotImplementedError
 
     @property
@@ -99,17 +102,19 @@
     def get_sheet_by_name(self, name):
         raise NotImplementedError
 
     def parse_worksheet(self, name):
         raise NotImplementedError
 
     def parse_row(self, row):
-        return {name: self.get_value(row[i])
-                for i, name in enumerate(self.get_field_names())
-                if i < len(row)}
+        return {
+            name: self.get_value(row[i])
+            for i, name in enumerate(self.get_field_names())
+            if i < len(row)
+        }
 
     def get_value(self, cell):
         raise NotImplementedError
 
     def dump(self, file=None):
         if file is None:
             file = self.file
@@ -123,15 +128,15 @@
 
     def calc_width(self, val):
         val = str(val) if val is not None else ""
         size = 0
         for c in val:
             if c in ".,;:'\"iIlt1":
                 size += 0.5
-            elif c in 'MW':
+            elif c in "MW":
                 size += 1.3
             elif c.isupper():
                 size += 1.2
             elif c.islower():
                 size += 1
             else:
                 size += 1.1
@@ -155,14 +160,15 @@
 
     def parse_worksheet(self, name):
         worksheet = self.get_sheet_by_name(name)
         self.worksheet = [worksheet.row(i) for i in range(worksheet.nrows)]
 
     def get_value(self, cell):
         import xlrd
+
         if cell.ctype == xlrd.XL_CELL_DATE:
             time, date = math.modf(cell.value)
             tpl = xlrd.xldate_as_tuple(cell.value, self.workbook.datemode)
             if date and time:
                 return datetime.datetime(*tpl)
             elif date:
                 return datetime.date(*tpl[0:3])
@@ -172,52 +178,53 @@
 
     def calc_width(self, val):
         val = str(val) if val is not None else ""
         size = 0
         for c in val:
             if c in ".,;:'\"iIlt1":
                 size += 0.5
-            elif c in 'MW':
+            elif c in "MW":
                 size += 1.3
             elif c.isupper():
                 size += 1.2
             elif c.islower():
                 size += 1
             else:
                 size += 1.1
         return size
 
     def open_worksheet(self, file):
         import xlwt
+
         workbook = xlwt.Workbook()
-        worksheet = workbook.add_sheet('Sheet 1')
+        worksheet = workbook.add_sheet("Sheet 1")
 
         formats = {
             datetime.date: xlwt.Style.easyxf(
                 num_format_str=self.date_format,
             ),
             datetime.time: xlwt.Style.easyxf(
                 num_format_str=self.time_format,
             ),
             datetime.datetime: xlwt.Style.easyxf(
                 num_format_str=self.datetime_format,
             ),
-            'header': xlwt.Style.easyxf(
+            "header": xlwt.Style.easyxf(
                 "font: bold on; borders: bottom thick;"
             ),
         }
 
         widths = {}
 
         def write(r, c, val):
             widths.setdefault(c, 0)
             widths[c] = max(widths[c], self.calc_width(val))
             fmt = formats.get(type(val))
             if not fmt and r == 0:
-                fmt = formats['header']
+                fmt = formats["header"]
             if fmt:
                 worksheet.write(r, c, val, fmt)
             else:
                 worksheet.write(r, c, val)
 
         def close():
             for c, width in widths.items():
@@ -226,14 +233,15 @@
 
         return write, close
 
 
 class ExcelParser(WorkbookParser):
     def parse_workbook(self):
         import openpyxl
+
         self.workbook = openpyxl.open(self.file, data_only=True)
 
     @property
     def sheet_names(self):
         return self.workbook.sheetnames
 
     def get_sheet_by_name(self, name):
@@ -248,48 +256,49 @@
         if isinstance(value, datetime.datetime):
             if value.time() == datetime.time(0, 0):
                 return value.date()
         return value
 
     def open_worksheet(self, file):
         from openpyxl import Workbook, styles, utils
+
         workbook = Workbook()
         worksheet = workbook.active
 
         formats = {
             datetime.date: styles.NamedStyle(
-                name='date',
+                name="date",
                 number_format=self.date_format,
             ),
             datetime.time: styles.NamedStyle(
-                name='time',
+                name="time",
                 number_format=self.time_format,
             ),
             datetime.datetime: styles.NamedStyle(
-                name='datetime',
+                name="datetime",
                 number_format=self.datetime_format,
             ),
-            'header': styles.NamedStyle(
-                name='header',
+            "header": styles.NamedStyle(
+                name="header",
                 font=styles.Font(bold=True),
-                border=styles.Border(bottom=styles.Side(style='thick'))
+                border=styles.Border(bottom=styles.Side(style="thick")),
             ),
         }
         widths = {}
 
         def write(r, c, val):
             widths.setdefault(c, 0)
             widths[c] = max(widths[c], self.calc_width(val))
             cell = worksheet.cell(r + 1, c + 1, val)
 
             fmt = formats.get(type(val))
             if fmt:
                 cell.style = fmt
             elif r == 0:
-                cell.style = formats['header']
+                cell.style = formats["header"]
 
         def close():
             for c, width in widths.items():
                 col = utils.get_column_letter(c + 1)
                 worksheet.column_dimensions[col].width = width
             workbook.save(self.filename)
```

### Comparing `itertable-2.1.0/itertable/parsers/readers.py` & `itertable-2.2.0/itertable/parsers/readers.py`

 * *Files 4% similar despite different names*

```diff
@@ -5,16 +5,24 @@
     """
     A specialized version of DictReader that attempts to find where the "real"
     CSV data is in a file that may contain a prelude of non-CSV text.
     """
 
     max_header_row = 20
 
-    def __init__(self, f, fieldnames=None, restkey=None, restval=None,
-                 dialect="excel", *args, **kwds):
+    def __init__(
+        self,
+        f,
+        fieldnames=None,
+        restkey=None,
+        restval=None,
+        dialect="excel",
+        *args,
+        **kwds
+    ):
         # Preserve file since we're going to start reading it
         self._file = f
 
         # Preserve reader options since we'll need to make another one
         readeropts = [f, dialect]
         readeropts.extend(args)
         self._readeropts = (readeropts, kwds)
@@ -35,15 +43,15 @@
             try:
                 rows.append(next(data))
             except StopIteration:
                 pass
         header_row, field_names = self.choose_header(rows)
 
         # Reset file and advance reader so it starts in the right spot
-        if hasattr(self._file, 'seek'):
+        if hasattr(self._file, "seek"):
             self._file.seek(0)
         for i in range(header_row + 1):
             try:
                 next(self.reader)
             except StopIteration:
                 pass
```

### Comparing `itertable-2.1.0/itertable/util.py` & `itertable-2.2.0/itertable/util.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,73 +1,80 @@
 from .base import BaseIter
 from .loaders import FileLoader, NetLoader, StringLoader
 from .parsers import (
-    CsvParser, JsonParser, XmlParser, ExcelParser, OldExcelParser
+    CsvParser,
+    JsonParser,
+    XmlParser,
+    ExcelParser,
+    OldExcelParser,
 )
 from .mappers import TupleMapper
 from .exceptions import ParseFailed
 import mimetypes
 import io
 
+xlsx = "application/vnd.openxmlformats-officedocument.spreadsheetml.sheet"
+
 PARSERS = {
-    'application/vnd.ms-excel': OldExcelParser,
-    'application/CDFV2': OldExcelParser,
-    'application/vnd.openxmlformats-officedocument.spreadsheetml.sheet':
-    ExcelParser,
-    'application/octet-stream': ExcelParser,
-    'text/csv': CsvParser,
-    'application/csv': CsvParser,
-    'application/json': JsonParser,
-    'application/xml': XmlParser,
-    'text/xml': XmlParser,
+    "application/vnd.ms-excel": OldExcelParser,
+    "application/CDFV2": OldExcelParser,
+    xlsx: ExcelParser,
+    "application/octet-stream": ExcelParser,
+    "text/csv": CsvParser,
+    "application/csv": CsvParser,
+    "application/json": JsonParser,
+    "application/xml": XmlParser,
+    "text/xml": XmlParser,
 }
 
 BINARY_TYPES = set(key for key, cls in PARSERS.items() if cls.binary)
 TEXT_TYPES = set(key for key, cls in PARSERS.items() if not cls.binary)
 
 # Save generated classes to avoid recreating them
 _iter_classes = {}
 
 
-def make_iter(loader, parser, mapper=TupleMapper,
-              name=None, module="itertable"):
+def make_iter(
+    loader, parser, mapper=TupleMapper, name=None, module="itertable"
+):
     """
     Mix the specified loader, parser, and mapper classes into a usable Iter
     """
     key = (loader, parser, mapper)
     if key in _iter_classes:
         return _iter_classes[key]
 
     if name is None:
-        lname = parser.__name__.replace('Parser', '')
-        pname = loader.__name__.replace('Loader', '')
+        lname = parser.__name__.replace("Parser", "")
+        pname = loader.__name__.replace("Loader", "")
         if mapper == TupleMapper:
             mname = ""
         else:
-            mname = mapper.__name__.replace('Mapper', '')
+            mname = mapper.__name__.replace("Mapper", "")
         name = lname + pname + mname + "Iter"
     cls = type(name, (loader, parser, mapper, BaseIter), {})
     cls.__module__ = module
     _iter_classes[key] = cls
     return cls
 
 
 def guess_type(filename, buffer=None):
     mimetype, encoding = mimetypes.guess_type(filename)
     if mimetype is None:
         try:
             import magic
+
             if buffer:
                 mimetype = magic.from_buffer(buffer, mime=True)
-                if mimetype == 'text/plain':
-                    if buffer.startswith('{') or buffer.startswith('['):
+                if mimetype == "text/plain":
+                    if buffer.startswith("{") or buffer.startswith("["):
                         mimetype = "application/json"
-                    elif buffer.startswith('<'):
+                    elif buffer.startswith("<"):
                         mimetype = "application/xml"
-                    elif ',' in buffer:
+                    elif "," in buffer:
                         mimetype = "text/csv"
             else:
                 mimetype = magic.from_file(filename, mime=True)
         except ImportError:
             pass
     return mimetype
 
@@ -76,19 +83,19 @@
     if options is None:
         options = {}
 
     if isinstance(filename, str):
         mimetype = guess_type(filename)
     else:
         file = filename
-        assert hasattr(file, 'read'), "Use load_file() with path or file obj"
+        assert hasattr(file, "read"), "Use load_file() with path or file obj"
         buffer = file.read(2048)
-        if hasattr(file, 'seek'):
+        if hasattr(file, "seek"):
             file.seek(0)
-        filename = getattr(file, 'name', '__unknown__')
+        filename = getattr(file, "name", "__unknown__")
         mimetype = guess_type(filename, buffer=buffer)
 
         if mimetype in TEXT_TYPES and isinstance(buffer, bytes):
             bfile = file
             file = io.StringIO(bfile.read().decode())
             bfile.close()
 
@@ -109,45 +116,46 @@
     parser = PARSERS[mimetype]
     loader = NetLoader
     Iter = make_iter(loader, parser, mapper)
     return Iter(url=url, **options)
 
 
 def load_string(string, mapper=TupleMapper, options={}):
-    if string.startswith('<'):
+    if string.startswith("<"):
         parser = XmlParser
-    elif string.startswith('[') or (
-            string.startswith('{') and 'namespace' in options):
+    elif string.startswith("[") or (
+        string.startswith("{") and "namespace" in options
+    ):
         parser = JsonParser
-    elif ',' in string:
+    elif "," in string:
         parser = CsvParser
     else:
         raise Exception("Could not determine parser for string!")
 
     loader = StringLoader
     Iter = make_iter(loader, parser, mapper)
     if Iter.binary:
-        string = string.encode('utf-8')
+        string = string.encode("utf-8")
     return Iter(string=string, **options)
 
 
 class FlatIter(TupleMapper, BaseIter):
     """
     Denormalizes a nested Iter structure (e.g. an array of individual time
     series) into a single iterable.  Each row in the top level Iter should have
     an attribute (typically 'data') pointing to an inner Iter.  Both the top
     level Iter class and the inner class should extend TupleMapper.
     """
 
     iter_class = None
-    inner_attr = 'data'
+    inner_attr = "data"
 
     def __init__(self, *args, **kwargs):
-        self.iter_class = kwargs.pop('iter_class', self.iter_class)
-        self.inner_attr = kwargs.pop('inner_attr', self.inner_attr)
+        self.iter_class = kwargs.pop("iter_class", self.iter_class)
+        self.inner_attr = kwargs.pop("inner_attr", self.inner_attr)
         if self.iter_class is None:
             raise Exception("An Iter class must be specified")
 
         # Pass remaining arguments
         self.nested_iter = self.iter_class(*args, **kwargs)
         self.data = list(self.unpack_iter())
```

### Comparing `itertable-2.1.0/itertable/base.py` & `itertable-2.2.0/itertable/base.py`

 * *Files 2% similar despite different names*

```diff
@@ -18,21 +18,21 @@
         if not self.loaded:
             self.load()
             self.loaded = True
 
         if self.parsed:
             return
 
-        if getattr(self, 'empty_file', False):
+        if getattr(self, "empty_file", False):
             self.data = []
         else:
             self.parse()
-            if hasattr(self, 'file'):
+            if hasattr(self, "file"):
                 f = self.file
-                if hasattr(f, 'close') and not getattr(f, 'closed', False):
+                if hasattr(f, "close") and not getattr(f, "closed", False):
                     f.close()
 
         self.parsed = True
 
     def load(self):
         "Open a resource (defined by loader mixins)"
         # self.file = ...
@@ -43,38 +43,38 @@
         Parse a resource (defined by parser mixins).
         Result should be an iterable of dicts.
         """
         # self.data = some_parse_method(self.file)
         pass
 
     def dump(self, file=None):
-        ""
+        """"""
         if file is None:
             file = self.file
         file.write(str(self.data))
 
     def save(self):
-        ""
+        """"""
         self.dump(self.file)
 
     field_names = None
     scan_fields = False
     _auto_field_names = None
 
     def get_field_names(self):
         "Returns a list of raw fields to expect (defined by parser mixins)"
         if self.field_names is not None:
             # Support specifying field_names as string (like namedtuple does)
             if isinstance(self.field_names, str):
-                return self.field_names.replace(',', ' ').split()
+                return self.field_names.replace(",", " ").split()
             else:
                 return self.field_names
 
         # If no defined field names, try to retrieve from data
-        if not getattr(self, 'data', None):
+        if not getattr(self, "data", None):
             return None
 
         if self._auto_field_names:
             return self._auto_field_names
 
         if self.scan_fields:
             # Scan all rows for field names
@@ -106,15 +106,15 @@
         return uitem
 
     def compute_index(self, recompute=False):
         key_field = self.get_key_field()
         if key_field is None:
             return None
 
-        if getattr(self, '_index_cache', None) is not None and not recompute:
+        if getattr(self, "_index_cache", None) is not None and not recompute:
             return self._index_cache
 
         index = {}
         for i, item in enumerate(self.data):
             uitem = self.usable_item(item)
             if isinstance(uitem, dict):
                 key = uitem.get(key_field, None)
@@ -198,18 +198,18 @@
     no_pickle = []
     no_pickle_loader = []
     no_pickle_mapper = []
     no_pickle_parser = []
 
     def get_no_pickle(self):
         return (
-            self.no_pickle +
-            self.no_pickle_loader +
-            self.no_pickle_mapper +
-            self.no_pickle_parser
+            self.no_pickle
+            + self.no_pickle_loader
+            + self.no_pickle_mapper
+            + self.no_pickle_parser
         )
 
     def __getstate__(self):
         """
         Don't include auto-created and unpicklable properties in state.
         """
         state = self.__dict__.copy()
@@ -218,14 +218,15 @@
         return state
 
     def item_dict(self, item):
         return item
 
     def as_dataframe(self):
         from pandas import DataFrame
+
         key = self.get_key_field()
         if key:
             data = [self.item_dict(row) for row in self.values()]
         else:
             data = [self.item_dict(row) for row in self]
         df = DataFrame(data)
         if key:
```

### Comparing `itertable-2.1.0/itertable/gis/mixins.py` & `itertable-2.2.0/itertable/gis/mixins.py`

 * *Files 10% similar despite different names*

```diff
@@ -6,17 +6,18 @@
 from ..mappers import TupleMapper
 
 
 class FionaLoaderParser(FileLoader, BaseParser):
     """
     Composite loader & parser mixin for GIS data, powered by Fiona
     """
+
     layer_id = None
     meta = {}
-    key_field = 'id'
+    key_field = "id"
 
     def load(self):
         try:
             self.layers = fiona.listlayers(self.filename)
         except OSError as e:
             if self.require_existing:
                 raise LoadFailed(
@@ -30,123 +31,135 @@
             if self.require_existing:
                 raise LoadFailed(str(e))
             else:
                 self.empty_file = True
 
         if self.empty_file:
             driver = guess_driver(self.filename)
-            self.meta = {'driver': driver}
+            self.meta = {"driver": driver}
             self.empty_file = True
 
     def parse(self):
         # If multiple layers, parse all of them (!)
         if len(self.layers) > 1 and self.layer_id is None:
             cls = type(self)
-            self.data = [{
-                'id': id,
-                'name': name,
-                'data': cls(filename=self.filename, layer_id=id)
-            } for id, name in enumerate(self.layers)]
+            self.data = [
+                {
+                    "id": id,
+                    "name": name,
+                    "data": cls(filename=self.filename, layer_id=id),
+                }
+                for id, name in enumerate(self.layers)
+            ]
         else:
             # One layer, load & parse GIS data
             with fiona.open(self.filename, layer=self.layer_id) as f:
                 self.meta = f.meta
-                if 'id' in f.meta.get('schema', {}).get('properties', {}):
+                if "id" in f.meta.get("schema", {}).get("properties", {}):
                     # TODO: Is this correct?
-                    del f.meta['schema']['properties']['id']
+                    del f.meta["schema"]["properties"]["id"]
                 self.data = list(map(self.parse_feature, f))
 
     def parse_feature(self, f):
         # Flatten Fiona's GeoJSON-style representation into something more
         # amenable to namedtuple-ing
-        feat = {key: value for key, value in f['properties'].items()}
-        if 'id' not in feat and 'ID' not in feat:
-            feat['id'] = f['id']
-        feat['geometry'] = f['geometry']
+        feat = {key: value for key, value in f["properties"].items()}
+        if "id" not in feat and "ID" not in feat:
+            feat["id"] = f["id"]
+        feat["geometry"] = f["geometry"]
         return feat
 
     def dump_feature(self, feat, i):
         # Undo aforementioned flattening
         return {
-            'id': feat.get('id', feat.get('ID', i)),
-            'geometry': feat['geometry'],
-            'properties': {
-                key: value for key, value in feat.items()
-                if key not in ('geometry', 'id',)
-            }
+            "id": feat.get("id", feat.get("ID", i)),
+            "geometry": feat["geometry"],
+            "properties": {
+                key: value
+                for key, value in feat.items()
+                if key
+                not in (
+                    "geometry",
+                    "id",
+                )
+            },
         }
 
     def dump(self):
         # Dump and save the dataset at the same time via Fiona
         pass
 
     def save(self):
-        with fiona.open(self.filename, 'w', **self.meta) as f:
+        with fiona.open(self.filename, "w", **self.meta) as f:
             for i, feat in enumerate(self.data):
                 f.write(self.dump_feature(feat, i))
 
 
 class GisMapper(TupleMapper):
     """
     GIS-aware tuple mapper
     """
+
     def as_dataframe(self):
         # Mimic BaseIter.as_dataframe() but with GeoDataFrame
         # (also, key_field is always set)
         from geopandas import GeoDataFrame
+
         key = self.get_key_field()
         data = [self.item_dict(row) for row in self.values()]
         df = GeoDataFrame(data)
         df.set_index(key, inplace=True)
         return df
 
     def item_dict(self, uitem):
         # Turn usable item into GeoDataFrame-friendly dict
         data = uitem._asdict()
-        data['geometry'] = geometry.shape(data['geometry'])
+        data["geometry"] = geometry.shape(data["geometry"])
         return data
 
 
 class ShapeMapper(GisMapper):
     """
     Map Fiona's GeoJSON-style geometries to and from Shapely shapes
     """
+
     def map_value(self, field, value):
         value = super(ShapeMapper, self).map_value(field, value)
-        if field == 'geometry':
+        if field == "geometry":
             value = geometry.shape(value)
         return value
 
     def unmap_value(self, field, value):
-        if field == 'geometry':
+        if field == "geometry":
             value = geometry.mapping(value)
         return super(ShapeMapper, self).unmap_value(field, value)
 
     def item_dict(self, uitem):
         return uitem._asdict()
 
 
 class WktMapper(ShapeMapper):
     """
     Map geometries to and from WKT (good for Django integration)
     """
+
     def map_value(self, field, value):
         value = super(WktMapper, self).map_value(field, value)
-        if field == 'geometry':
+        if field == "geometry":
             value = wkt.dumps(value)
         return value
 
     def unmap_value(self, field, value):
-        if field == 'geometry':
+        if field == "geometry":
             value = wkt.loads(value)
         return super(WktMapper, self).unmap_value(field, value)
 
     def item_dict(self, uitem):
         data = uitem._asdict()
-        data['geometry'] = wkt.loads(data['geometry'])
+        data["geometry"] = wkt.loads(data["geometry"])
         return data
 
 
 def guess_driver(filename):
     if filename.endswith(".shp"):
         return "ESRI Shapefile"
     else:
```

### Comparing `itertable-2.1.0/itertable/gis/__init__.py` & `itertable-2.2.0/itertable/gis/__init__.py`

 * *Files 11% similar despite different names*

```diff
@@ -2,26 +2,26 @@
 from ..base import BaseIter
 
 
 class MetaSyncIter(BaseIter):
     """
     Custom sync() to handle transfering Fiona metadata (except for driver)
     """
+
     def sync(self, other, save=True):
-        driver = other.meta.get('driver', None)
+        driver = other.meta.get("driver", None)
         other.meta = self.meta.copy()
         if driver:
-            other.meta['driver'] = driver
+            other.meta["driver"] = driver
         super(MetaSyncIter, self).sync(other, save)
 
     def get_field_names(self):
         if self.field_names is None and self.meta is not None:
-            return (
-                ['id', 'geometry']
-                + list(self.meta['schema']['properties'].keys())
+            return ["id", "geometry"] + list(
+                self.meta["schema"]["properties"].keys()
             )
         return super(MetaSyncIter, self).get_field_names()
 
 
 class GisIter(FionaLoaderParser, GisMapper, MetaSyncIter):
     pass
```

### Comparing `itertable-2.1.0/itertable/mappers.py` & `itertable-2.2.0/itertable/mappers.py`

 * *Files 8% similar despite different names*

```diff
@@ -64,58 +64,57 @@
         for v in self.value_map:
             if self.value_map[v] == value:
                 return v
         return value
 
 
 class TupleMapper(DictMapper):
-    no_pickle_mapper = ['_tuple_class', '_tuple_prototype']
+    no_pickle_mapper = ["_tuple_class", "_tuple_prototype"]
 
     @property
     def field_map(self):
         field_names = self.get_field_names()
-        if not field_names and not getattr(self, 'data', None):
+        if not field_names and not getattr(self, "data", None):
             raise NoData
 
         # FIXME: check for duplicates
-        if not hasattr(self, '_field_map'):
+        if not hasattr(self, "_field_map"):
             items = [
-                (field, self.tuple_field_name(field))
-                for field in field_names
+                (field, self.tuple_field_name(field)) for field in field_names
             ]
             self._field_map = OrderedDict(items)
         return self._field_map
 
     def tuple_field_name(self, field):
         field = self.clean_field_name(field)
-        field = re.sub(r'\W', '', field.lower())
+        field = re.sub(r"\W", "", field.lower())
         # normalize identifiers for consistency with namedtuple
         # http://bugs.python.org/issue23091
-        field = normalize('NFKC', field)
+        field = normalize("NFKC", field)
         return field
 
     def clean_field_name(self, field):
         return field
 
     @property
     def tuple_class(self):
         "Returns a class to use for individual items"
 
-        if not hasattr(self, '_tuple_class'):
+        if not hasattr(self, "_tuple_class"):
             cls = namedtuple(
-                self.__class__.__name__ + 'Tuple',
-                list(self.field_map.values())
+                self.__class__.__name__ + "Tuple",
+                list(self.field_map.values()),
             )
             self._tuple_class = cls
 
         return self._tuple_class
 
     @property
     def tuple_prototype(self):
-        if not hasattr(self, '_tuple_prototype'):
+        if not hasattr(self, "_tuple_prototype"):
             vals = {field: None for field in self.field_map.values()}
             self._tuple_prototype = self.tuple_class(**vals)
         return self._tuple_prototype
 
     def usable_item(self, item):
         mapped = super(TupleMapper, self).usable_item(item)
         try:
@@ -132,44 +131,46 @@
 
     def create(self, **kwargs):
         return self.tuple_prototype._replace(**kwargs)
 
 
 def parse_iso8601(val):
     # See http://bugs.python.org/issue15873
-    if hasattr(datetime, 'fromisoformat'):
+    if hasattr(datetime, "fromisoformat"):
         return datetime.fromisoformat(val)
     try:
         from django.utils.dateparse import parse_datetime
     except ImportError:
         try:
             from iso8601 import parse_date as parse_datetime
         except ImportError:
-            raise Exception('No suitable iso8601 parser found!')
+            raise Exception("No suitable iso8601 parser found!")
     try:
         result = parse_datetime(val)
     except Exception:
         result = None
     if result is None:
         raise ValueError("Could not parse %s as iso8601 date!" % val)
     return result
 
 
 def make_date_mapper(fmt):
     """
     Generate functions to use for mapping strings to dates
     """
+
     def mapper(val):
-        if fmt == 'iso8601':
+        if fmt == "iso8601":
             return parse_iso8601(val)
         val = datetime.strptime(val, fmt)
-        if '%Y' in fmt or '%y' in fmt:
+        if "%Y" in fmt or "%y" in fmt:
             return val
         else:
             return val.time()
+
     return mapper
 
 
 class TimeSeriesMapper(TupleMapper):
     date_formats = None
     map_floats = True
     map_functions = []
```

### Comparing `itertable-2.1.0/itertable/__init__.py` & `itertable-2.2.0/itertable/__init__.py`

 * *Files 19% similar despite different names*

```diff
@@ -28,66 +28,60 @@
 
 from .util import (
     make_iter,
     load_file,
     load_url,
     load_string,
     guess_type,
-    flattened
+    flattened,
 )
 
-from .version import VERSION
+try:
+    from .version import __version__ as VERSION
+except ImportError:
+    VERSION = "0.0.0"
 
 
 __all__ = (
-    'BaseIter',
-
-    'BaseLoader',
-    'FileLoader',
-    'Zipper',
-    'ZipFileLoader',
-    'StringLoader',
-    'NetLoader',
-    'ZipNetLoader',
-
-    'CsvParser',
-    'JsonParser',
-    'XmlParser',
-    'ExcelParser',
-    'OldExcelParser',
-
-    'BaseMapper',
-    'DictMapper',
-    'TupleMapper',
-    'TimeSeriesMapper',
-    'make_date_mapper',
-
-    'make_iter',
-    'load_file',
-    'load_url',
-    'load_string',
-    'guess_type',
-    'flattened',
-
-    'VERSION',
-
-    'CsvFileIter',
-    'CsvNetIter',
-    'CsvStringIter',
-
-    'JsonFileIter',
-    'JsonNetIter',
-    'JsonStringIter',
-
-    'XmlFileIter',
-    'XmlNetIter',
-    'XmlStringIter',
-
-    'OldExcelFileIter',
-    'ExcelFileIter',
+    "BaseIter",
+    "BaseLoader",
+    "FileLoader",
+    "Zipper",
+    "ZipFileLoader",
+    "StringLoader",
+    "NetLoader",
+    "ZipNetLoader",
+    "CsvParser",
+    "JsonParser",
+    "XmlParser",
+    "ExcelParser",
+    "OldExcelParser",
+    "BaseMapper",
+    "DictMapper",
+    "TupleMapper",
+    "TimeSeriesMapper",
+    "make_date_mapper",
+    "make_iter",
+    "load_file",
+    "load_url",
+    "load_string",
+    "guess_type",
+    "flattened",
+    "VERSION",
+    "CsvFileIter",
+    "CsvNetIter",
+    "CsvStringIter",
+    "JsonFileIter",
+    "JsonNetIter",
+    "JsonStringIter",
+    "XmlFileIter",
+    "XmlNetIter",
+    "XmlStringIter",
+    "OldExcelFileIter",
+    "ExcelFileIter",
 )
 
 # Some useful pre-mixed classes
 CsvFileIter = make_iter(FileLoader, CsvParser)
 CsvNetIter = make_iter(NetLoader, CsvParser)
 CsvStringIter = make_iter(StringLoader, CsvParser)
 
@@ -102,14 +96,15 @@
 OldExcelFileIter = make_iter(FileLoader, OldExcelParser)
 ExcelFileIter = make_iter(FileLoader, ExcelParser)
 OldExcelNetIter = make_iter(NetLoader, OldExcelParser)
 ExcelNetIter = make_iter(NetLoader, ExcelParser)
 
 try:
     from .gis import GisIter, ShapeIter, WktIter
+
     __all__ += (
-        'GisIter',
-        'ShapeIter',
-        'WktIter',
+        "GisIter",
+        "ShapeIter",
+        "WktIter",
     )
 except ImportError:
     pass
```

