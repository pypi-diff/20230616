# Comparing `tmp/gcocf-0.9.2.tar.gz` & `tmp/gcocf-0.9.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "gcocf-0.9.2.tar", last modified: Fri Jan  1 00:00:00 2016, max compression
+gzip compressed data, was "gcocf-0.9.3.tar", last modified: Fri Jan  1 00:00:00 2016, max compression
```

## Comparing `gcocf-0.9.2.tar` & `gcocf-0.9.3.tar`

### file list

```diff
@@ -1,30 +1,30 @@
--rw-r--r--   0        0        0      124 2023-06-16 16:17:19.674608 gcocf-0.9.2/.example.envrc
--rw-r--r--   0        0        0      669 2023-06-16 16:17:19.674608 gcocf-0.9.2/.github/ISSUE_TEMPLATE/bug_report.md
--rw-r--r--   0        0        0      644 2023-06-16 16:17:19.674608 gcocf-0.9.2/.github/ISSUE_TEMPLATE/feature_request.md
--rw-r--r--   0        0        0      501 2023-06-16 16:17:19.674608 gcocf-0.9.2/.github/dependabot.yml
--rw-r--r--   0        0        0     1076 2023-06-16 16:17:19.674608 gcocf-0.9.2/.github/pull_request_template.md
--rw-r--r--   0        0        0     1701 2023-06-16 16:17:19.674608 gcocf-0.9.2/.github/workflows/Testing.yml
--rw-r--r--   0        0        0       87 2023-06-16 16:17:19.674608 gcocf-0.9.2/.gitignore
--rw-r--r--   0        0        0     5224 2023-06-16 16:17:19.674608 gcocf-0.9.2/CODE_OF_CONDUCT.md
--rw-r--r--   0        0        0      203 2023-06-16 16:17:19.674608 gcocf-0.9.2/CONTRIBUTING.md
--rw-r--r--   0        0        0      274 2023-06-16 16:17:19.674608 gcocf-0.9.2/Dockerfile
--rw-r--r--   0        0        0      144 2023-06-16 16:17:19.674608 gcocf-0.9.2/GCoCF/__init__.py
--rwxr-xr-x   0        0        0    10880 2023-06-16 16:17:19.674608 gcocf-0.9.2/GCoCF/__main__.py
--rw-r--r--   0        0        0     2224 2023-06-16 16:17:19.674608 gcocf-0.9.2/GCoCF/api.py
--rw-r--r--   0        0        0     6488 2023-06-16 16:17:19.674608 gcocf-0.9.2/GCoCF/formatters.py
--rw-r--r--   0        0        0     2369 2023-06-16 16:17:19.674608 gcocf-0.9.2/GCoCF/locales/messages.pot
--rw-r--r--   0        0        0    11947 2023-06-16 16:17:19.674608 gcocf-0.9.2/GCoCF/models.py
--rw-r--r--   0        0        0     1009 2023-06-16 16:17:19.674608 gcocf-0.9.2/GCoCF/notifiers.py
--rw-r--r--   0        0        0     1378 2023-06-16 16:17:19.674608 gcocf-0.9.2/GCoCF/utils.py
--rw-r--r--   0        0        0     1070 2023-06-16 16:17:19.678608 gcocf-0.9.2/LICENSE.txt
--rw-r--r--   0        0        0       34 2023-06-16 16:17:19.678608 gcocf-0.9.2/README.md
--rw-r--r--   0        0        0     2495 2023-06-16 16:17:19.678608 gcocf-0.9.2/SECURITY.md
--rw-r--r--   0        0        0    41692 2023-06-16 16:17:19.678608 gcocf-0.9.2/data/full_destruction.json
--rw-r--r--   0        0        0    77643 2023-06-16 16:17:19.678608 gcocf-0.9.2/data/inWar_40.json
--rw-r--r--   0        0        0     1059 2023-06-16 16:17:19.678608 gcocf-0.9.2/data/notInWar.json
--rw-r--r--   0        0        0    24207 2023-06-16 16:17:19.678608 gcocf-0.9.2/data/op_full_destruction.json
--rw-r--r--   0        0        0    98300 2023-06-16 16:17:19.678608 gcocf-0.9.2/data/warEnded_50.json
--rw-r--r--   0        0        0      831 2023-06-16 16:17:19.678608 gcocf-0.9.2/pyproject.toml
--rw-r--r--   0        0        0       54 2023-06-16 16:17:19.678608 gcocf-0.9.2/requirements.txt
--rw-r--r--   0        0        0    11544 2023-06-16 16:17:19.678608 gcocf-0.9.2/test_everything.py
--rw-r--r--   0        0        0      874 1970-01-01 00:00:00.000000 gcocf-0.9.2/PKG-INFO
+-rw-r--r--   0        0        0      124 2023-06-16 16:20:07.894043 gcocf-0.9.3/.example.envrc
+-rw-r--r--   0        0        0      669 2023-06-16 16:20:07.894043 gcocf-0.9.3/.github/ISSUE_TEMPLATE/bug_report.md
+-rw-r--r--   0        0        0      644 2023-06-16 16:20:07.894043 gcocf-0.9.3/.github/ISSUE_TEMPLATE/feature_request.md
+-rw-r--r--   0        0        0      501 2023-06-16 16:20:07.894043 gcocf-0.9.3/.github/dependabot.yml
+-rw-r--r--   0        0        0     1076 2023-06-16 16:20:07.894043 gcocf-0.9.3/.github/pull_request_template.md
+-rw-r--r--   0        0        0     1691 2023-06-16 16:20:07.894043 gcocf-0.9.3/.github/workflows/Testing.yml
+-rw-r--r--   0        0        0       87 2023-06-16 16:20:07.894043 gcocf-0.9.3/.gitignore
+-rw-r--r--   0        0        0     5224 2023-06-16 16:20:07.894043 gcocf-0.9.3/CODE_OF_CONDUCT.md
+-rw-r--r--   0        0        0      203 2023-06-16 16:20:07.894043 gcocf-0.9.3/CONTRIBUTING.md
+-rw-r--r--   0        0        0      274 2023-06-16 16:20:07.894043 gcocf-0.9.3/Dockerfile
+-rw-r--r--   0        0        0      144 2023-06-16 16:20:07.894043 gcocf-0.9.3/GCoCF/__init__.py
+-rwxr-xr-x   0        0        0    10880 2023-06-16 16:20:07.894043 gcocf-0.9.3/GCoCF/__main__.py
+-rw-r--r--   0        0        0     2224 2023-06-16 16:20:07.894043 gcocf-0.9.3/GCoCF/api.py
+-rw-r--r--   0        0        0     6488 2023-06-16 16:20:07.894043 gcocf-0.9.3/GCoCF/formatters.py
+-rw-r--r--   0        0        0     2369 2023-06-16 16:20:07.894043 gcocf-0.9.3/GCoCF/locales/messages.pot
+-rw-r--r--   0        0        0    11947 2023-06-16 16:20:07.894043 gcocf-0.9.3/GCoCF/models.py
+-rw-r--r--   0        0        0     1009 2023-06-16 16:20:07.894043 gcocf-0.9.3/GCoCF/notifiers.py
+-rw-r--r--   0        0        0     1378 2023-06-16 16:20:07.894043 gcocf-0.9.3/GCoCF/utils.py
+-rw-r--r--   0        0        0     1070 2023-06-16 16:20:07.894043 gcocf-0.9.3/LICENSE.txt
+-rw-r--r--   0        0        0       34 2023-06-16 16:20:07.894043 gcocf-0.9.3/README.md
+-rw-r--r--   0        0        0     2495 2023-06-16 16:20:07.894043 gcocf-0.9.3/SECURITY.md
+-rw-r--r--   0        0        0    41692 2023-06-16 16:20:07.894043 gcocf-0.9.3/data/full_destruction.json
+-rw-r--r--   0        0        0    77643 2023-06-16 16:20:07.894043 gcocf-0.9.3/data/inWar_40.json
+-rw-r--r--   0        0        0     1059 2023-06-16 16:20:07.894043 gcocf-0.9.3/data/notInWar.json
+-rw-r--r--   0        0        0    24207 2023-06-16 16:20:07.894043 gcocf-0.9.3/data/op_full_destruction.json
+-rw-r--r--   0        0        0    98300 2023-06-16 16:20:07.898043 gcocf-0.9.3/data/warEnded_50.json
+-rw-r--r--   0        0        0      832 2023-06-16 16:20:07.898043 gcocf-0.9.3/pyproject.toml
+-rw-r--r--   0        0        0       54 2023-06-16 16:20:07.898043 gcocf-0.9.3/requirements.txt
+-rw-r--r--   0        0        0    11544 2023-06-16 16:20:07.898043 gcocf-0.9.3/test_everything.py
+-rw-r--r--   0        0        0      875 1970-01-01 00:00:00.000000 gcocf-0.9.3/PKG-INFO
```

### Comparing `gcocf-0.9.2/.github/ISSUE_TEMPLATE/bug_report.md` & `gcocf-0.9.3/.github/ISSUE_TEMPLATE/bug_report.md`

 * *Files identical despite different names*

### Comparing `gcocf-0.9.2/.github/ISSUE_TEMPLATE/feature_request.md` & `gcocf-0.9.3/.github/ISSUE_TEMPLATE/feature_request.md`

 * *Files identical despite different names*

### Comparing `gcocf-0.9.2/.github/pull_request_template.md` & `gcocf-0.9.3/.github/pull_request_template.md`

 * *Files identical despite different names*

### Comparing `gcocf-0.9.2/.github/workflows/Testing.yml` & `gcocf-0.9.3/.github/workflows/Testing.yml`

 * *Files 1% similar despite different names*

```diff
@@ -7,15 +7,15 @@
     cancel-in-progress: true
 
 jobs:
   build-and-test:
     runs-on: ubuntu-latest
     strategy:
       matrix:
-        python-version: [3.7, 3.9, 3.11]
+        python-version: [3.11]
 
     steps:
       - uses: actions/checkout@v3
 
       - name: Set up Python ${{ matrix.python-version }}
         uses: actions/setup-python@v3.1.4
         with:
```

### Comparing `gcocf-0.9.2/CODE_OF_CONDUCT.md` & `gcocf-0.9.3/CODE_OF_CONDUCT.md`

 * *Files identical despite different names*

### Comparing `gcocf-0.9.2/GCoCF/__main__.py` & `gcocf-0.9.3/GCoCF/__main__.py`

 * *Files identical despite different names*

### Comparing `gcocf-0.9.2/GCoCF/api.py` & `gcocf-0.9.3/GCoCF/api.py`

 * *Files identical despite different names*

### Comparing `gcocf-0.9.2/GCoCF/formatters.py` & `gcocf-0.9.3/GCoCF/formatters.py`

 * *Files identical despite different names*

### Comparing `gcocf-0.9.2/GCoCF/locales/messages.pot` & `gcocf-0.9.3/GCoCF/locales/messages.pot`

 * *Files identical despite different names*

### Comparing `gcocf-0.9.2/GCoCF/models.py` & `gcocf-0.9.3/GCoCF/models.py`

 * *Files identical despite different names*

### Comparing `gcocf-0.9.2/GCoCF/notifiers.py` & `gcocf-0.9.3/GCoCF/notifiers.py`

 * *Files identical despite different names*

### Comparing `gcocf-0.9.2/GCoCF/utils.py` & `gcocf-0.9.3/GCoCF/utils.py`

 * *Files identical despite different names*

### Comparing `gcocf-0.9.2/LICENSE.txt` & `gcocf-0.9.3/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `gcocf-0.9.2/SECURITY.md` & `gcocf-0.9.3/SECURITY.md`

 * *Files identical despite different names*

### Comparing `gcocf-0.9.2/data/full_destruction.json` & `gcocf-0.9.3/data/full_destruction.json`

 * *Files identical despite different names*

### Comparing `gcocf-0.9.2/data/inWar_40.json` & `gcocf-0.9.3/data/inWar_40.json`

 * *Files identical despite different names*

### Comparing `gcocf-0.9.2/data/notInWar.json` & `gcocf-0.9.3/data/notInWar.json`

 * *Files identical despite different names*

### Comparing `gcocf-0.9.2/data/op_full_destruction.json` & `gcocf-0.9.3/data/op_full_destruction.json`

 * *Files identical despite different names*

### Comparing `gcocf-0.9.2/data/warEnded_50.json` & `gcocf-0.9.3/data/warEnded_50.json`

 * *Files identical despite different names*

### Comparing `gcocf-0.9.2/pyproject.toml` & `gcocf-0.9.3/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 build-backend = 'flit.buildapi'
 
 [tool.flit.metadata]
 module = 'GCoCF'
 author = 'Gustavo Schip'
 author-email = 'gustavoschip@proton.me'
 home-page = 'https://github.com/GILLESMaster/GCoCF'
-requires-python = '>=3.5'
+requires-python = '>=3.11'
 classifiers = [
     'Environment :: Console',
     'Natural Language :: English',
     'Development Status :: 4 - Beta',
     'Programming Language :: Python :: 3',
     'Intended Audience :: End Users/Desktop',
     'License :: OSI Approved :: MIT License']
```

### Comparing `gcocf-0.9.2/test_everything.py` & `gcocf-0.9.3/test_everything.py`

 * *Files identical despite different names*

### Comparing `gcocf-0.9.2/PKG-INFO` & `gcocf-0.9.3/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,16 +1,16 @@
 Metadata-Version: 2.1
 Name: GCoCF
-Version: 0.9.2
+Version: 0.9.3
 Summary: Clash of Clans war moniting for Discord.
 Home-page: https://github.com/GILLESMaster/GCoCF
 Keywords: coc clashofclans discord
 Author: Gustavo Schip
 Author-email: gustavoschip@proton.me
-Requires-Python: >=3.5
+Requires-Python: >=3.11
 Description-Content-Type: text/markdown
 Classifier: Environment :: Console
 Classifier: Natural Language :: English
 Classifier: Development Status :: 4 - Beta
 Classifier: Programming Language :: Python :: 3
 Classifier: Intended Audience :: End Users/Desktop
 Classifier: License :: OSI Approved :: MIT License
```

