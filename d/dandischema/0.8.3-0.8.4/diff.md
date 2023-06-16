# Comparing `tmp/dandischema-0.8.3.tar.gz` & `tmp/dandischema-0.8.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "/home/runner/work/dandi-schema/dandi-schema/dandischema/dist/.tmp-5ukzi4l3/dandischema-0.8.3.tar", last modified: Mon Apr 17 17:43:00 2023, max compression
+gzip compressed data, was "/home/runner/work/dandi-schema/dandi-schema/dandischema/dist/.tmp-fhv13_ye/dandischema-0.8.4.tar", last modified: Fri Jun 16 13:43:20 2023, max compression
```

## Comparing `dandischema-0.8.3.tar` & `dandischema-0.8.4.tar`

### file list

```diff
@@ -1,53 +1,53 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-17 17:43:00.000000 dandischema-0.8.3/
--rw-r--r--   0 runner    (1001) docker     (123)    20913 2023-04-17 17:42:50.000000 dandischema-0.8.3/CHANGELOG.md
--rw-r--r--   0 runner    (1001) docker     (123)    11357 2023-04-17 17:42:25.000000 dandischema-0.8.3/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)       72 2023-04-17 17:42:25.000000 dandischema-0.8.3/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     2637 2023-04-17 17:43:00.000000 dandischema-0.8.3/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1515 2023-04-17 17:42:25.000000 dandischema-0.8.3/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-17 17:43:00.000000 dandischema-0.8.3/dandischema/
--rw-r--r--   0 runner    (1001) docker     (123)       74 2023-04-17 17:42:25.000000 dandischema-0.8.3/dandischema/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)       22 2023-04-17 17:43:00.000000 dandischema-0.8.3/dandischema/_version.py
--rw-r--r--   0 runner    (1001) docker     (123)      604 2023-04-17 17:42:25.000000 dandischema-0.8.3/dandischema/consts.py
--rw-r--r--   0 runner    (1001) docker     (123)     8570 2023-04-17 17:42:25.000000 dandischema-0.8.3/dandischema/datacite.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-17 17:43:00.000000 dandischema-0.8.3/dandischema/digests/
--rw-r--r--   0 runner    (1001) docker     (123)       37 2023-04-17 17:42:25.000000 dandischema-0.8.3/dandischema/digests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     6657 2023-04-17 17:42:25.000000 dandischema-0.8.3/dandischema/digests/dandietag.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-17 17:43:00.000000 dandischema-0.8.3/dandischema/digests/tests/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-17 17:42:25.000000 dandischema-0.8.3/dandischema/digests/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4687 2023-04-17 17:42:25.000000 dandischema-0.8.3/dandischema/digests/tests/test_dandietag.py
--rw-r--r--   0 runner    (1001) docker     (123)    10162 2023-04-17 17:42:25.000000 dandischema-0.8.3/dandischema/digests/tests/test_zarr.py
--rw-r--r--   0 runner    (1001) docker     (123)     6819 2023-04-17 17:42:25.000000 dandischema-0.8.3/dandischema/digests/zarr.py
--rw-r--r--   0 runner    (1001) docker     (123)      530 2023-04-17 17:42:25.000000 dandischema-0.8.3/dandischema/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (123)    13880 2023-04-17 17:42:25.000000 dandischema-0.8.3/dandischema/metadata.py
--rw-r--r--   0 runner    (1001) docker     (123)    50471 2023-04-17 17:42:25.000000 dandischema-0.8.3/dandischema/models.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-17 17:42:25.000000 dandischema-0.8.3/dandischema/py.typed
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-17 17:43:00.000000 dandischema-0.8.3/dandischema/tests/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-17 17:42:25.000000 dandischema-0.8.3/dandischema/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      397 2023-04-17 17:42:25.000000 dandischema-0.8.3/dandischema/tests/conftest.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-17 17:43:00.000000 dandischema-0.8.3/dandischema/tests/data/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-17 17:43:00.000000 dandischema-0.8.3/dandischema/tests/data/metadata/
--rw-r--r--   0 runner    (1001) docker     (123)     2641 2023-04-17 17:42:25.000000 dandischema-0.8.3/dandischema/tests/data/metadata/asset3_01.json
--rw-r--r--   0 runner    (1001) docker     (123)     2638 2023-04-17 17:42:25.000000 dandischema-0.8.3/dandischema/tests/data/metadata/asset3_02.json
--rw-r--r--   0 runner    (1001) docker     (123)     2481 2023-04-17 17:42:25.000000 dandischema-0.8.3/dandischema/tests/data/metadata/asset4_01.json
--rw-r--r--   0 runner    (1001) docker     (123)     2481 2023-04-17 17:42:25.000000 dandischema-0.8.3/dandischema/tests/data/metadata/asset4_02.json
--rw-r--r--   0 runner    (1001) docker     (123)     2271 2023-04-17 17:42:25.000000 dandischema-0.8.3/dandischema/tests/data/metadata/asset_001.json
--rw-r--r--   0 runner    (1001) docker     (123)    13458 2023-04-17 17:42:25.000000 dandischema-0.8.3/dandischema/tests/data/metadata/meta_000004.json
--rw-r--r--   0 runner    (1001) docker     (123)    18070 2023-04-17 17:42:25.000000 dandischema-0.8.3/dandischema/tests/data/metadata/meta_000004old.json
--rw-r--r--   0 runner    (1001) docker     (123)     5322 2023-04-17 17:42:25.000000 dandischema-0.8.3/dandischema/tests/data/metadata/meta_000008.json
--rw-r--r--   0 runner    (1001) docker     (123)    17082 2023-04-17 17:42:25.000000 dandischema-0.8.3/dandischema/tests/test_datacite.py
--rw-r--r--   0 runner    (1001) docker     (123)    21361 2023-04-17 17:42:25.000000 dandischema-0.8.3/dandischema/tests/test_metadata.py
--rw-r--r--   0 runner    (1001) docker     (123)    22314 2023-04-17 17:42:25.000000 dandischema-0.8.3/dandischema/tests/test_models.py
--rw-r--r--   0 runner    (1001) docker     (123)     1236 2023-04-17 17:42:25.000000 dandischema-0.8.3/dandischema/tests/test_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)      148 2023-04-17 17:42:25.000000 dandischema-0.8.3/dandischema/tests/utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     1283 2023-04-17 17:42:25.000000 dandischema-0.8.3/dandischema/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-17 17:43:00.000000 dandischema-0.8.3/dandischema.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     2637 2023-04-17 17:43:00.000000 dandischema-0.8.3/dandischema.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1321 2023-04-17 17:43:00.000000 dandischema-0.8.3/dandischema.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-17 17:43:00.000000 dandischema-0.8.3/dandischema.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-17 17:42:33.000000 dandischema-0.8.3/dandischema.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)      197 2023-04-17 17:43:00.000000 dandischema-0.8.3/dandischema.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       12 2023-04-17 17:43:00.000000 dandischema-0.8.3/dandischema.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)      791 2023-04-17 17:42:25.000000 dandischema-0.8.3/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)     1940 2023-04-17 17:43:00.000000 dandischema-0.8.3/setup.cfg
--rwxr-xr-x   0 runner    (1001) docker     (123)      696 2023-04-17 17:42:25.000000 dandischema-0.8.3/setup.py
--rw-r--r--   0 runner    (1001) docker     (123)      617 2023-04-17 17:42:25.000000 dandischema-0.8.3/tox.ini
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 13:43:20.000000 dandischema-0.8.4/
+-rw-r--r--   0 runner    (1001) docker     (123)    21695 2023-06-16 13:43:11.000000 dandischema-0.8.4/CHANGELOG.md
+-rw-r--r--   0 runner    (1001) docker     (123)    11357 2023-06-16 13:42:47.000000 dandischema-0.8.4/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)       72 2023-06-16 13:42:47.000000 dandischema-0.8.4/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     2637 2023-06-16 13:43:20.000000 dandischema-0.8.4/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1515 2023-06-16 13:42:47.000000 dandischema-0.8.4/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 13:43:20.000000 dandischema-0.8.4/dandischema/
+-rw-r--r--   0 runner    (1001) docker     (123)       74 2023-06-16 13:42:47.000000 dandischema-0.8.4/dandischema/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)       22 2023-06-16 13:43:20.000000 dandischema-0.8.4/dandischema/_version.py
+-rw-r--r--   0 runner    (1001) docker     (123)      604 2023-06-16 13:42:47.000000 dandischema-0.8.4/dandischema/consts.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9049 2023-06-16 13:42:47.000000 dandischema-0.8.4/dandischema/datacite.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 13:43:20.000000 dandischema-0.8.4/dandischema/digests/
+-rw-r--r--   0 runner    (1001) docker     (123)       37 2023-06-16 13:42:47.000000 dandischema-0.8.4/dandischema/digests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6657 2023-06-16 13:42:47.000000 dandischema-0.8.4/dandischema/digests/dandietag.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 13:43:20.000000 dandischema-0.8.4/dandischema/digests/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-16 13:42:47.000000 dandischema-0.8.4/dandischema/digests/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4687 2023-06-16 13:42:47.000000 dandischema-0.8.4/dandischema/digests/tests/test_dandietag.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10162 2023-06-16 13:42:47.000000 dandischema-0.8.4/dandischema/digests/tests/test_zarr.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6819 2023-06-16 13:42:47.000000 dandischema-0.8.4/dandischema/digests/zarr.py
+-rw-r--r--   0 runner    (1001) docker     (123)      530 2023-06-16 13:42:47.000000 dandischema-0.8.4/dandischema/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13880 2023-06-16 13:42:47.000000 dandischema-0.8.4/dandischema/metadata.py
+-rw-r--r--   0 runner    (1001) docker     (123)    50471 2023-06-16 13:42:47.000000 dandischema-0.8.4/dandischema/models.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-16 13:42:47.000000 dandischema-0.8.4/dandischema/py.typed
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 13:43:20.000000 dandischema-0.8.4/dandischema/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-16 13:42:47.000000 dandischema-0.8.4/dandischema/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      397 2023-06-16 13:42:47.000000 dandischema-0.8.4/dandischema/tests/conftest.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 13:43:20.000000 dandischema-0.8.4/dandischema/tests/data/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 13:43:20.000000 dandischema-0.8.4/dandischema/tests/data/metadata/
+-rw-r--r--   0 runner    (1001) docker     (123)     2641 2023-06-16 13:42:47.000000 dandischema-0.8.4/dandischema/tests/data/metadata/asset3_01.json
+-rw-r--r--   0 runner    (1001) docker     (123)     2638 2023-06-16 13:42:47.000000 dandischema-0.8.4/dandischema/tests/data/metadata/asset3_02.json
+-rw-r--r--   0 runner    (1001) docker     (123)     2481 2023-06-16 13:42:47.000000 dandischema-0.8.4/dandischema/tests/data/metadata/asset4_01.json
+-rw-r--r--   0 runner    (1001) docker     (123)     2481 2023-06-16 13:42:47.000000 dandischema-0.8.4/dandischema/tests/data/metadata/asset4_02.json
+-rw-r--r--   0 runner    (1001) docker     (123)     2271 2023-06-16 13:42:47.000000 dandischema-0.8.4/dandischema/tests/data/metadata/asset_001.json
+-rw-r--r--   0 runner    (1001) docker     (123)    13458 2023-06-16 13:42:47.000000 dandischema-0.8.4/dandischema/tests/data/metadata/meta_000004.json
+-rw-r--r--   0 runner    (1001) docker     (123)    18070 2023-06-16 13:42:47.000000 dandischema-0.8.4/dandischema/tests/data/metadata/meta_000004old.json
+-rw-r--r--   0 runner    (1001) docker     (123)     5322 2023-06-16 13:42:47.000000 dandischema-0.8.4/dandischema/tests/data/metadata/meta_000008.json
+-rw-r--r--   0 runner    (1001) docker     (123)    18946 2023-06-16 13:42:47.000000 dandischema-0.8.4/dandischema/tests/test_datacite.py
+-rw-r--r--   0 runner    (1001) docker     (123)    21361 2023-06-16 13:42:47.000000 dandischema-0.8.4/dandischema/tests/test_metadata.py
+-rw-r--r--   0 runner    (1001) docker     (123)    22314 2023-06-16 13:42:47.000000 dandischema-0.8.4/dandischema/tests/test_models.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1236 2023-06-16 13:42:47.000000 dandischema-0.8.4/dandischema/tests/test_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)      148 2023-06-16 13:42:47.000000 dandischema-0.8.4/dandischema/tests/utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1283 2023-06-16 13:42:47.000000 dandischema-0.8.4/dandischema/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 13:43:20.000000 dandischema-0.8.4/dandischema.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     2637 2023-06-16 13:43:20.000000 dandischema-0.8.4/dandischema.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1321 2023-06-16 13:43:20.000000 dandischema-0.8.4/dandischema.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-16 13:43:20.000000 dandischema-0.8.4/dandischema.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-16 13:42:53.000000 dandischema-0.8.4/dandischema.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)      207 2023-06-16 13:43:20.000000 dandischema-0.8.4/dandischema.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       12 2023-06-16 13:43:20.000000 dandischema-0.8.4/dandischema.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      791 2023-06-16 13:42:47.000000 dandischema-0.8.4/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)     1946 2023-06-16 13:43:20.000000 dandischema-0.8.4/setup.cfg
+-rwxr-xr-x   0 runner    (1001) docker     (123)      696 2023-06-16 13:42:47.000000 dandischema-0.8.4/setup.py
+-rw-r--r--   0 runner    (1001) docker     (123)      617 2023-06-16 13:42:47.000000 dandischema-0.8.4/tox.ini
```

### Comparing `dandischema-0.8.3/CHANGELOG.md` & `dandischema-0.8.4/CHANGELOG.md`

 * *Files 2% similar despite different names*

```diff
@@ -1,7 +1,26 @@
+# 0.8.4 (Fri Jun 16 2023)
+
+#### 🐛 Bug Fix
+
+- added funderidtype and support for funder and sponsor roles to datacite metadata [#167](https://github.com/dandi/dandi-schema/pull/167) ([@satra](https://github.com/satra) [@pre-commit-ci[bot]](https://github.com/pre-commit-ci[bot]) [@djarecka](https://github.com/djarecka))
+
+#### 🧪 Tests
+
+- Add mypy to test extra_requires since needed for type hints testing [#174](https://github.com/dandi/dandi-schema/pull/174) ([@yarikoptic](https://github.com/yarikoptic))
+
+#### Authors: 4
+
+- [@pre-commit-ci[bot]](https://github.com/pre-commit-ci[bot])
+- Dorota Jarecka ([@djarecka](https://github.com/djarecka))
+- Satrajit Ghosh ([@satra](https://github.com/satra))
+- Yaroslav Halchenko ([@yarikoptic](https://github.com/yarikoptic))
+
+---
+
 # 0.8.3 (Mon Apr 17 2023)
 
 #### 🏠 Internal
 
 - [pre-commit.ci] pre-commit autoupdate [#170](https://github.com/dandi/dandi-schema/pull/170) ([@pre-commit-ci[bot]](https://github.com/pre-commit-ci[bot]))
 
 #### 🔩 Dependency Updates
```

### Comparing `dandischema-0.8.3/LICENSE` & `dandischema-0.8.4/LICENSE`

 * *Files identical despite different names*

### Comparing `dandischema-0.8.3/PKG-INFO` & `dandischema-0.8.4/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dandischema
-Version: 0.8.3
+Version: 0.8.4
 Summary: Schemata for DANDI archive project
 Home-page: http://dandiarchive.org
 Author: DANDI developers
 Author-email: team@dandiarchive.org
 Maintainer: Yaroslav O. Halchenko
 Maintainer-email: debian@onerussian.com
 License: Apache 2.0
```

### Comparing `dandischema-0.8.3/README.md` & `dandischema-0.8.4/README.md`

 * *Files identical despite different names*

### Comparing `dandischema-0.8.3/dandischema/consts.py` & `dandischema-0.8.4/dandischema/consts.py`

 * *Files identical despite different names*

### Comparing `dandischema-0.8.3/dandischema/datacite.py` & `dandischema-0.8.4/dandischema/datacite.py`

 * *Files 3% similar despite different names*

```diff
@@ -106,24 +106,34 @@
         for el in meta.license
     ]
     attributes["schemaVersion"] = "http://datacite.org/schema/kernel-4"
 
     contributors = []
     creators = []
     for contr_el in meta.contributor:
-        if contr_el.roleName and RoleType("dcite:Sponsor") in contr_el.roleName:
+        if contr_el.roleName and (
+            RoleType("dcite:Sponsor") in contr_el.roleName
+            or RoleType("dcite:Funder") in contr_el.roleName
+        ):
             # no info about "funderIdentifierType", "awardUri", "awardTitle"
             dict_fund = {"funderName": contr_el.name}
             if contr_el.identifier:
                 dict_fund["funderIdentifier"] = contr_el.identifier
+                funderidtype = "Other"
+                if "ror.org" in contr_el.identifier:
+                    funderidtype = "ROR"
+                dict_fund["funderIdentifierType"] = funderidtype
             if contr_el.awardNumber:
                 dict_fund["awardNumber"] = contr_el.awardNumber
             attributes.setdefault("fundingReferences", []).append(dict_fund)
             # if no more roles, it shouldn't be added to creators or contributors
-            contr_el.roleName.remove(RoleType("dcite:Sponsor"))
+            if RoleType("dcite:Sponsor") in contr_el.roleName:
+                contr_el.roleName.remove(RoleType("dcite:Sponsor"))
+            if RoleType("dcite:Funder") in contr_el.roleName:
+                contr_el.roleName.remove(RoleType("dcite:Funder"))
             if not contr_el.roleName:
                 continue
 
         contr_dict: Dict[str, Any] = {
             "name": contr_el.name,
             "contributorName": contr_el.name,
             "schemeURI": "orcid.org",
```

### Comparing `dandischema-0.8.3/dandischema/digests/dandietag.py` & `dandischema-0.8.4/dandischema/digests/dandietag.py`

 * *Files identical despite different names*

### Comparing `dandischema-0.8.3/dandischema/digests/tests/test_dandietag.py` & `dandischema-0.8.4/dandischema/digests/tests/test_dandietag.py`

 * *Files identical despite different names*

### Comparing `dandischema-0.8.3/dandischema/digests/tests/test_zarr.py` & `dandischema-0.8.4/dandischema/digests/tests/test_zarr.py`

 * *Files identical despite different names*

### Comparing `dandischema-0.8.3/dandischema/digests/zarr.py` & `dandischema-0.8.4/dandischema/digests/zarr.py`

 * *Files identical despite different names*

### Comparing `dandischema-0.8.3/dandischema/exceptions.py` & `dandischema-0.8.4/dandischema/exceptions.py`

 * *Files identical despite different names*

### Comparing `dandischema-0.8.3/dandischema/metadata.py` & `dandischema-0.8.4/dandischema/metadata.py`

 * *Files identical despite different names*

### Comparing `dandischema-0.8.3/dandischema/models.py` & `dandischema-0.8.4/dandischema/models.py`

 * *Files identical despite different names*

### Comparing `dandischema-0.8.3/dandischema/tests/data/metadata/asset3_01.json` & `dandischema-0.8.4/dandischema/tests/data/metadata/asset3_01.json`

 * *Files identical despite different names*

### Comparing `dandischema-0.8.3/dandischema/tests/data/metadata/asset3_02.json` & `dandischema-0.8.4/dandischema/tests/data/metadata/asset3_02.json`

 * *Files identical despite different names*

### Comparing `dandischema-0.8.3/dandischema/tests/data/metadata/asset4_01.json` & `dandischema-0.8.4/dandischema/tests/data/metadata/asset4_01.json`

 * *Files identical despite different names*

### Comparing `dandischema-0.8.3/dandischema/tests/data/metadata/asset4_02.json` & `dandischema-0.8.4/dandischema/tests/data/metadata/asset4_02.json`

 * *Files identical despite different names*

### Comparing `dandischema-0.8.3/dandischema/tests/data/metadata/asset_001.json` & `dandischema-0.8.4/dandischema/tests/data/metadata/asset_001.json`

 * *Files identical despite different names*

### Comparing `dandischema-0.8.3/dandischema/tests/data/metadata/meta_000004.json` & `dandischema-0.8.4/dandischema/tests/data/metadata/meta_000004.json`

 * *Files identical despite different names*

### Comparing `dandischema-0.8.3/dandischema/tests/data/metadata/meta_000004old.json` & `dandischema-0.8.4/dandischema/tests/data/metadata/meta_000004old.json`

 * *Files identical despite different names*

### Comparing `dandischema-0.8.3/dandischema/tests/data/metadata/meta_000008.json` & `dandischema-0.8.4/dandischema/tests/data/metadata/meta_000008.json`

 * *Files identical despite different names*

### Comparing `dandischema-0.8.3/dandischema/tests/test_datacite.py` & `dandischema-0.8.4/dandischema/tests/test_datacite.py`

 * *Files 4% similar despite different names*

```diff
@@ -219,14 +219,68 @@
                 ],
             },
             {
                 "creators": (1, {"name": "A_last, A_first"}),
                 "fundingReferences": (1, {"funderName": "B_last, B_first"}),
             },
         ),
+        # Add a sponsor with an identifier
+        (
+            {
+                "contributor": [
+                    {
+                        "name": "A_last, A_first",
+                        "roleName": [RoleType("dcite:ContactPerson")],
+                    },
+                    {
+                        "name": "B_last, B_first",
+                        "identifier": "0000-0001-0000-0000",
+                        "roleName": [RoleType("dcite:Sponsor")],
+                    },
+                ],
+            },
+            {
+                "creators": (1, {"name": "A_last, A_first"}),
+                "fundingReferences": (
+                    1,
+                    {
+                        "funderName": "B_last, B_first",
+                        "funderIdentifier": "0000-0001-0000-0000",
+                        "funderIdentifierType": "Other",
+                    },
+                ),
+            },
+        ),
+        # should also work with Funder role
+        (
+            {
+                "contributor": [
+                    {
+                        "name": "A_last, A_first",
+                        "roleName": [RoleType("dcite:ContactPerson")],
+                    },
+                    {
+                        "name": "B_last, B_first",
+                        "identifier": "0000-0001-0000-0000",
+                        "roleName": [RoleType("dcite:Funder")],
+                    },
+                ],
+            },
+            {
+                "creators": (1, {"name": "A_last, A_first"}),
+                "fundingReferences": (
+                    1,
+                    {
+                        "funderName": "B_last, B_first",
+                        "funderIdentifier": "0000-0001-0000-0000",
+                        "funderIdentifierType": "Other",
+                    },
+                ),
+            },
+        ),
         # additional contributor with 2 roles: Author and Software (doesn't exist in datacite)
         # the person should be in creators and contributors (with contributorType Other)
         # Adding Orcid ID to the identifier to one of the contributors
         (
             {
                 "contributor": [
                     {
```

### Comparing `dandischema-0.8.3/dandischema/tests/test_metadata.py` & `dandischema-0.8.4/dandischema/tests/test_metadata.py`

 * *Files identical despite different names*

### Comparing `dandischema-0.8.3/dandischema/tests/test_models.py` & `dandischema-0.8.4/dandischema/tests/test_models.py`

 * *Files identical despite different names*

### Comparing `dandischema-0.8.3/dandischema/tests/test_utils.py` & `dandischema-0.8.4/dandischema/tests/test_utils.py`

 * *Files identical despite different names*

### Comparing `dandischema-0.8.3/dandischema/utils.py` & `dandischema-0.8.4/dandischema/utils.py`

 * *Files identical despite different names*

### Comparing `dandischema-0.8.3/dandischema.egg-info/PKG-INFO` & `dandischema-0.8.4/dandischema.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dandischema
-Version: 0.8.3
+Version: 0.8.4
 Summary: Schemata for DANDI archive project
 Home-page: http://dandiarchive.org
 Author: DANDI developers
 Author-email: team@dandiarchive.org
 Maintainer: Yaroslav O. Halchenko
 Maintainer-email: debian@onerussian.com
 License: Apache 2.0
```

### Comparing `dandischema-0.8.3/dandischema.egg-info/SOURCES.txt` & `dandischema-0.8.4/dandischema.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `dandischema-0.8.3/pyproject.toml` & `dandischema-0.8.4/pyproject.toml`

 * *Files identical despite different names*

### Comparing `dandischema-0.8.3/setup.cfg` & `dandischema-0.8.4/setup.cfg`

 * *Files 4% similar despite different names*

```diff
@@ -41,14 +41,15 @@
 include = dandischema*
 
 [options.extras_require]
 style = 
 	flake8
 	pre-commit
 test = 
+	mypy
 	pytest
 	pytest-cov
 all = 
 	%(style)s
 	%(test)s
 
 [flake8]
```

### Comparing `dandischema-0.8.3/setup.py` & `dandischema-0.8.4/setup.py`

 * *Files identical despite different names*

### Comparing `dandischema-0.8.3/tox.ini` & `dandischema-0.8.4/tox.ini`

 * *Files identical despite different names*

